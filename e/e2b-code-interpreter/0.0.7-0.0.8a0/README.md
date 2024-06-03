# Comparing `tmp/e2b_code_interpreter-0.0.7.tar.gz` & `tmp/e2b_code_interpreter-0.0.8a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2b_code_interpreter-0.0.7.tar", max compression
+gzip compressed data, was "e2b_code_interpreter-0.0.8a0.tar", max compression
```

## Comparing `e2b_code_interpreter-0.0.7.tar` & `e2b_code_interpreter-0.0.8a0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2331 2024-05-23 09:16:43.243391 e2b_code_interpreter-0.0.7/README.md
--rw-r--r--   0        0        0      149 2024-05-23 09:16:43.243391 e2b_code_interpreter-0.0.7/e2b_code_interpreter/__init__.py
--rw-r--r--   0        0        0    11080 2024-05-23 09:16:43.243391 e2b_code_interpreter-0.0.7/e2b_code_interpreter/main.py
--rw-r--r--   0        0        0     8759 2024-05-23 09:16:43.243391 e2b_code_interpreter-0.0.7/e2b_code_interpreter/messaging.py
--rw-r--r--   0        0        0     7884 2024-05-23 09:16:43.243391 e2b_code_interpreter-0.0.7/e2b_code_interpreter/models.py
--rw-r--r--   0        0        0      766 2024-05-23 09:17:15.003308 e2b_code_interpreter-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     3246 1970-01-01 00:00:00.000000 e2b_code_interpreter-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     2331 2024-06-03 09:31:46.125432 e2b_code_interpreter-0.0.8a0/README.md
+-rw-r--r--   0        0        0      149 2024-06-03 09:31:46.125432 e2b_code_interpreter-0.0.8a0/e2b_code_interpreter/__init__.py
+-rw-r--r--   0        0        0    14048 2024-06-03 09:31:46.125432 e2b_code_interpreter-0.0.8a0/e2b_code_interpreter/main.py
+-rw-r--r--   0        0        0     8884 2024-06-03 09:31:46.129432 e2b_code_interpreter-0.0.8a0/e2b_code_interpreter/messaging.py
+-rw-r--r--   0        0        0     7961 2024-06-03 09:31:46.129432 e2b_code_interpreter-0.0.8a0/e2b_code_interpreter/models.py
+-rw-r--r--   0        0        0      768 2024-06-03 09:32:01.249514 e2b_code_interpreter-0.0.8a0/pyproject.toml
+-rw-r--r--   0        0        0     3248 1970-01-01 00:00:00.000000 e2b_code_interpreter-0.0.8a0/PKG-INFO
```

### Comparing `e2b_code_interpreter-0.0.7/README.md` & `e2b_code_interpreter-0.0.8a0/README.md`

 * *Files identical despite different names*

### Comparing `e2b_code_interpreter-0.0.7/e2b_code_interpreter/main.py` & `e2b_code_interpreter-0.0.8a0/e2b_code_interpreter/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from __future__ import annotations
 
+import json
 import logging
 import threading
+import uuid
+
 import requests
 
 from concurrent.futures import Future
 from typing import Any, Callable, List, Optional, Dict
 
 from e2b import EnvVars, ProcessMessage, Sandbox
 from e2b.constants import TIMEOUT
@@ -56,14 +59,17 @@
     def __init__(self, sandbox: CodeInterpreter, timeout: Optional[float] = TIMEOUT):
         self._sandbox = sandbox
         self._kernel_id_set = Future()
         self._start_connecting_to_default_kernel(timeout=timeout)
         self._connected_kernels: Dict[str, Future[JupyterKernelWebSocket]] = {}
         self._default_kernel_id: Optional[str] = None
 
+    def get_default_url(self) -> str:
+        return f"https://{self._sandbox.get_hostname(8888)}/doc/tree/RTC:default.ipynb"
+
     def exec_cell(
         self,
         code: str,
         kernel_id: Optional[str] = None,
         on_stdout: Optional[Callable[[ProcessMessage], Any]] = None,
         on_stderr: Optional[Callable[[ProcessMessage], Any]] = None,
         on_result: Optional[Callable[[Result], Any]] = None,
@@ -87,82 +93,152 @@
         logger.debug(f"Executing code in kernel {kernel_id}")
 
         if ws_future:
             logger.debug(f"Using existing websocket connection to kernel {kernel_id}")
             ws = ws_future.result(timeout=timeout)
         else:
             logger.debug(f"Creating new websocket connection to kernel {kernel_id}")
-            ws = self._connect_to_kernel_ws(kernel_id, timeout=timeout)
+            ws = self._connect_to_kernel_ws(kernel_id, None, timeout=timeout)
 
-        session_id = ws.send_execution_message(code, on_stdout, on_stderr, on_result)
+        message_id = ws.send_execution_message(code, on_stdout, on_stderr, on_result)
         logger.debug(
-            f"Sent execution message to kernel {kernel_id}, session_id: {session_id}"
+            f"Sent execution message to kernel {kernel_id}, message_id: {message_id}"
         )
 
-        result = ws.get_result(session_id, timeout=timeout)
+        result = ws.get_result(message_id, timeout=timeout)
         logger.debug(
-            f"Received result from kernel {kernel_id}, session_id: {session_id}, result: {result}"
+            f"Received result from kernel {kernel_id}, message_id: {message_id}, result: {result}"
         )
 
+        nb = self._sandbox.filesystem.read(f"/home/user/default.ipynb", timeout=timeout)
+        nb_parsed = json.loads(nb)
+        cell = {
+            "cell_type": "code",
+            "metadata": {},
+            "source": code,
+        }
+
+        outputs = []
+        if result.logs.stdout:
+            outputs.append(
+                {"output_type": "stream", "name": "stdout", "text": result.logs.stdout}
+            )
+        if result.logs.stderr:
+            outputs.append(
+                {"output_type": "stream", "name": "stderr", "text": result.logs.stderr}
+            )
+
+        if result.results:
+            outputs = [
+                {
+                    "output_type": (
+                        "execute_result" if r.is_main_result else "display_data"
+                    ),
+                    "data": r.raw,
+                    "metadata": {},
+                }
+                for r in result.results
+            ]
+
+        cell["execution_count"] = result.execution_count
+        cell["outputs"] = outputs
+
+        if nb_parsed["cells"] and not nb_parsed["cells"][-1]["source"]:
+            nb_parsed["cells"][-1] = cell
+        else:
+            nb_parsed["cells"].append(cell)
+
+        self._sandbox.filesystem.write(
+            f"/home/user/default.ipynb", json.dumps(nb_parsed), timeout=timeout
+        )
         return result
 
     @property
     def default_kernel_id(self) -> str:
         """
         Get the default kernel id
 
         :return: Default kernel id
         """
         if not self._default_kernel_id:
             logger.debug("Waiting for default kernel id")
             self._default_kernel_id = self._kernel_id_set.result()
 
         return self._default_kernel_id
-
-    def create_kernel(
-        self,
-        cwd: str = "/home/user",
-        kernel_name: Optional[str] = None,
-        timeout: Optional[float] = TIMEOUT,
-    ) -> str:
-        """
-        Creates a new kernel, this can be useful if you want to have multiple independent code execution environments.
-
-        The kernel can be optionally configured to start in a specific working directory and/or
-        with a specific kernel name. If no kernel name is provided, the default kernel will be used.
-        Once the kernel is created, this method establishes a WebSocket connection to the new kernel for
-        real-time communication.
-
-        :param cwd: Sets the current working directory for the kernel. Defaults to "/home/user".
-        :param kernel_name:
-            Specifies which kernel should be used, useful if you have multiple kernel types.
-            If not provided, the default kernel will be used.
-        :param timeout: Timeout for the kernel creation request.
-        :return: Kernel id of the created kernel
-        """
-        data = {"path": cwd}
-        if kernel_name:
-            data["kernel_name"] = kernel_name
-        logger.debug(f"Creating kernel with data: {data}")
-
-        response = requests.post(
-            f"{self._sandbox.get_protocol()}://{self._sandbox.get_hostname(8888)}/api/kernels",
-            json=data,
-            timeout=timeout,
-        )
-        if not response.ok:
-            raise KernelException(f"Failed to create kernel: {response.text}")
-
-        kernel_id = response.json()["id"]
-        logger.debug(f"Created kernel {kernel_id}")
-
-        threading.Thread(
-            target=self._connect_to_kernel_ws, args=(kernel_id, timeout)
-        ).start()
-        return kernel_id
+    #
+    # def create_kernel(
+    #     self,
+    #     name: str,
+    #     path: str = "/home/user",
+    #     kernel_name: str = "python3",
+    #     timeout: Optional[float] = TIMEOUT,
+    # ) -> str:
+    #     """
+    #     Creates a new kernel, this can be useful if you want to have multiple independent code execution environments.
+    #
+    #     The kernel can be optionally configured to start in a specific working directory and/or
+    #     with a specific kernel name. If no kernel name is provided, the default kernel will be used.
+    #     Once the kernel is created, this method establishes a WebSocket connection to the new kernel for
+    #     real-time communication.
+    #
+    #     :param name: Name of the kernel
+    #     :param path: Sets the current working directory for the kernel. Defaults to "/home/user".
+    #     :param kernel_name: Specifies which kernel should be used, useful if you have multiple kernel types.
+    #     :param timeout: Timeout for the kernel creation request.
+    #     :return: Kernel id of the created kernel
+    #     """
+    #
+    #     x = {
+    #         "metadata": {
+    #             "signature": "hex-digest",
+    #             "kernel_info": {"name": kernel_name},
+    #             "language_info": {
+    #                 "name": kernel_name,
+    #                 "version": "3.10.14",
+    #             },  # TODO: get version
+    #         },
+    #         "nbformat": 4,
+    #         "nbformat_minor": 0,
+    #         "cells": [],
+    #     }
+    #
+    #     self._sandbox.filesystem.write(
+    #         f"/home/user/default.ipynb", json.dumps(x), timeout=timeout
+    #     )
+    #     self._sandbox.process.start("chmod 777 /home/user/default.ipynb")
+    #
+    #     data = {
+    #         "name": name,
+    #         "kernel": {"name": kernel_name},
+    #         "notebook": {"name": "default.ipynb"},
+    #         "path": path,
+    #         "type": "notebook",
+    #     }
+    #
+    #     logger.debug(f"Creating kernel with data: {data}")
+    #
+    #     response = requests.post(
+    #         f"{self._sandbox.get_protocol()}://{self._sandbox.get_hostname(8888)}/api/sessions",
+    #         json=data,
+    #         timeout=timeout,
+    #     )
+    #     if not response.ok:
+    #         raise KernelException(f"Failed to create kernel: {response.text}")
+    #
+    #     response_data = response.json()
+    #     kernel_id = response_data["kernel"]["id"]
+    #     session_id = response_data["id"]
+    #
+    #     logger.debug(f"Created kernel {kernel_id}, session {session_id}")
+    #
+    #     threading.Thread(
+    #         target=self._connect_to_kernel_ws, args=(kernel_id, session_id, timeout)
+    #     ).start()
+    #
+    #     return kernel_id
 
     def restart_kernel(
         self, kernel_id: Optional[str] = None, timeout: Optional[float] = TIMEOUT
     ) -> None:
         """
         Restarts an existing Jupyter kernel. This can be useful to reset the kernel's state or to recover from errors.
 
@@ -182,88 +258,98 @@
         )
         if not response.ok:
             raise KernelException(f"Failed to restart kernel {kernel_id}")
 
         logger.debug(f"Restarted kernel {kernel_id}")
 
         threading.Thread(
-            target=self._connect_to_kernel_ws, args=(kernel_id, timeout)
+            target=self._connect_to_kernel_ws, args=(kernel_id, None, timeout)
         ).start()
-
-    def shutdown_kernel(
-        self, kernel_id: Optional[str] = None, timeout: Optional[float] = TIMEOUT
-    ) -> None:
-        """
-        Shuts down an existing Jupyter kernel. This method is used to gracefully terminate a kernel's process.
-
-        :param kernel_id: The unique identifier of the kernel to shutdown. If not provided, the default kernel is shutdown.
-        :param timeout: The timeout for the kernel shutdown request.
-        """
-        kernel_id = kernel_id or self.default_kernel_id
-        logger.debug(f"Shutting down kernel {kernel_id}")
-
-        self._connected_kernels[kernel_id].result().close()
-        del self._connected_kernels[kernel_id]
-        logger.debug(f"Closed websocket connection to kernel {kernel_id}")
-
-        response = requests.delete(
-            f"{self._sandbox.get_protocol()}://{self._sandbox.get_hostname(8888)}/api/kernels/{kernel_id}",
-            timeout=timeout,
-        )
-        if not response.ok:
-            raise KernelException(f"Failed to shutdown kernel {kernel_id}")
-
-        logger.debug(f"Shutdown kernel {kernel_id}")
-
-    def list_kernels(self, timeout: Optional[float] = TIMEOUT) -> List[str]:
-        """
-        Lists all available Jupyter kernels.
-
-        This method fetches a list of all currently available Jupyter kernels from the server. It can be used
-        to retrieve the IDs of all kernels that are currently running or available for connection.
-
-        :param timeout: The timeout for the kernel list request.
-        :return: List of kernel ids
-        """
-        response = requests.get(
-            f"{self._sandbox.get_protocol()}://{self._sandbox.get_hostname(8888)}/api/kernels",
-            timeout=timeout,
-        )
-
-        if not response.ok:
-            raise KernelException(f"Failed to list kernels: {response.text}")
-
-        return [kernel["id"] for kernel in response.json()]
+    #
+    # def shutdown_kernel(
+    #     self, kernel_id: Optional[str] = None, timeout: Optional[float] = TIMEOUT
+    # ) -> None:
+    #     """
+    #     Shuts down an existing Jupyter kernel. This method is used to gracefully terminate a kernel's process.
+    #
+    #     :param kernel_id: The unique identifier of the kernel to shutdown. If not provided, the default kernel is shutdown.
+    #     :param timeout: The timeout for the kernel shutdown request.
+    #     """
+    #     kernel_id = kernel_id or self.default_kernel_id
+    #     logger.debug(f"Shutting down kernel {kernel_id}")
+    #
+    #     self._connected_kernels[kernel_id].result().close()
+    #     del self._connected_kernels[kernel_id]
+    #     logger.debug(f"Closed websocket connection to kernel {kernel_id}")
+    #
+    #     response = requests.delete(
+    #         f"{self._sandbox.get_protocol()}://{self._sandbox.get_hostname(8888)}/api/kernels/{kernel_id}",
+    #         timeout=timeout,
+    #     )
+    #     if not response.ok:
+    #         raise KernelException(f"Failed to shutdown kernel {kernel_id}")
+    #
+    #     logger.debug(f"Shutdown kernel {kernel_id}")
+    #
+    # def list_kernels(self, timeout: Optional[float] = TIMEOUT) -> List[str]:
+    #     """
+    #     Lists all available Jupyter kernels.
+    #
+    #     This method fetches a list of all currently available Jupyter kernels from the server. It can be used
+    #     to retrieve the IDs of all kernels that are currently running or available for connection.
+    #
+    #     :param timeout: The timeout for the kernel list request.
+    #     :return: List of kernel ids
+    #     """
+    #     response = requests.get(
+    #         f"{self._sandbox.get_protocol()}://{self._sandbox.get_hostname(8888)}/api/kernels",
+    #         timeout=timeout,
+    #     )
+    #
+    #     if not response.ok:
+    #         raise KernelException(f"Failed to list kernels: {response.text}")
+    #
+    #     return [kernel["id"] for kernel in response.json()]
 
     def close(self):
         """
         Close all the websocket connections to the kernels. It doesn't shutdown the kernels.
         """
         logger.debug("Closing all websocket connections")
         for ws in self._connected_kernels.values():
             ws.result().close()
 
     def _connect_to_kernel_ws(
-        self, kernel_id: str, timeout: Optional[float] = TIMEOUT
+        self,
+        kernel_id: str,
+        session_id: Optional[str],
+        timeout: Optional[float] = TIMEOUT,
     ) -> JupyterKernelWebSocket:
         """
         Establishes a WebSocket connection to a specified Jupyter kernel.
 
         :param kernel_id: Kernel id
+        :param session_id: Session id
         :param timeout: The timeout for the kernel connection request.
 
         :return: Websocket connection
         """
+        if not session_id:
+            session_id = uuid.uuid4()
+
         logger.debug(f"Connecting to kernel's ({kernel_id}) websocket")
         future = Future()
         self._connected_kernels[kernel_id] = future
 
+        session_id = session_id or str(uuid.uuid4())
         ws = JupyterKernelWebSocket(
             url=f"{self._sandbox.get_protocol('ws')}://{self._sandbox.get_hostname(8888)}/api/kernels/{kernel_id}/channels",
+            session_id=session_id,
         )
+
         ws.connect(timeout=timeout)
         logger.debug(f"Connected to kernel's ({kernel_id}) websocket.")
 
         future.set_result(ws)
         return ws
 
     def _start_connecting_to_default_kernel(
@@ -272,19 +358,22 @@
         """
         Start connecting to the default kernel in a separate thread to avoid blocking the main thread.
         :param timeout: Timeout for the call
         """
         logger.debug("Starting to connect to the default kernel")
 
         def setup_default_kernel():
-            kernel_id = self._sandbox.filesystem.read(
-                "/root/.jupyter/kernel_id", timeout=timeout
+            session_info = self._sandbox.filesystem.read(
+                "/root/.jupyter/.session_info", timeout=timeout
             )
-            if kernel_id is None and not self._sandbox.is_open:
+
+            if session_info is None and not self._sandbox.is_open:
                 return
 
-            kernel_id = kernel_id.strip()
+            data = json.loads(session_info)
+            kernel_id = data["kernel"]["id"]
+            session_id = data["id"]
             logger.debug(f"Default kernel id: {kernel_id}")
-            self._connect_to_kernel_ws(kernel_id, timeout=timeout)
+            self._connect_to_kernel_ws(kernel_id, session_id, timeout=timeout)
             self._kernel_id_set.set_result(kernel_id)
 
         threading.Thread(target=setup_default_kernel).start()
```

### Comparing `e2b_code_interpreter-0.0.7/e2b_code_interpreter/messaging.py` & `e2b_code_interpreter-0.0.8a0/e2b_code_interpreter/messaging.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 class CellExecution:
     """
     Represents the execution of a cell in the Jupyter kernel.
     It's an internal class used by JupyterKernelWebSocket.
     """
 
     input_accepted: bool = False
+
     on_stdout: Optional[Callable[[ProcessMessage], Any]] = None
     on_stderr: Optional[Callable[[ProcessMessage], Any]] = None
     on_result: Optional[Callable[[Result], Any]] = None
 
     def __init__(
         self,
         on_stdout: Optional[Callable[[ProcessMessage], Any]] = None,
@@ -40,16 +41,17 @@
         self.on_stdout = on_stdout
         self.on_stderr = on_stderr
         self.on_result = on_result
 
 
 class JupyterKernelWebSocket:
 
-    def __init__(self, url: str):
+    def __init__(self, url: str, session_id: str):
         self.url = url
+        self.session_id = session_id
         self._cells: Dict[str, CellExecution] = {}
         self._waiting_for_replies: Dict[str, DeferredFuture] = {}
         self._queue_in = Queue()
         self._queue_out = Queue()
         self._stopped = threading.Event()
 
     def process_messages(self):
@@ -97,31 +99,30 @@
                 raise TimeoutException("WebSocket failed to start")
         except BaseException as e:
             self.close()
             raise Exception(f"WebSocket failed to start: {e}") from e
 
         logger.debug("WebSocket started")
 
-    @staticmethod
-    def _get_execute_request(msg_id: str, code: str) -> str:
+    def _get_execute_request(self, msg_id: str, code: str) -> str:
         return json.dumps(
             {
                 "header": {
                     "msg_id": msg_id,
                     "username": "e2b",
-                    "session": str(uuid.uuid4()),
+                    "session": self.session_id,
                     "msg_type": "execute_request",
                     "version": "5.3",
                 },
                 "parent_header": {},
                 "metadata": {},
                 "content": {
                     "code": code,
                     "silent": False,
-                    "store_history": False,
+                    "store_history": True,
                     "user_expressions": {},
                     "allow_stdin": False,
                 },
             }
         )
 
     def send_execution_message(
@@ -233,14 +234,15 @@
                     traceback_raw=data["content"]["traceback"],
                 )
             elif data["content"]["status"] == "ok":
                 pass
 
         elif data["msg_type"] == "execute_input":
             logger.debug(f"Input accepted for {parent_msg_ig}")
+            cell.partial_result.execution_count = data["content"]["execution_count"]
             cell.input_accepted = True
         else:
             logger.warning(f"[UNHANDLED MESSAGE TYPE]: {data['msg_type']}")
 
     def close(self):
         logger.debug("Closing WebSocket")
         self._stopped.set()
```

### Comparing `e2b_code_interpreter-0.0.7/e2b_code_interpreter/models.py` & `e2b_code_interpreter-0.0.8a0/e2b_code_interpreter/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,14 +218,16 @@
 
     results: List[Result] = []
     "List of the result of the cell (interactively interpreted last line), display calls (e.g. matplotlib plots)."
     logs: Logs = Logs()
     "Logs printed to stdout and stderr during execution."
     error: Optional[Error] = None
     "Error object if an error occurred, None otherwise."
+    execution_count: Optional[int] = None
+    "Execution count of the cell."
 
     @property
     def text(self) -> Optional[str]:
         """
         Returns the text representation of the result.
 
         :return: The text representation of the result.
@@ -245,15 +247,15 @@
         """
         Serializes the results to JSON.
         This method is used by the Pydantic JSON encoder.
         """
         serialized = []
         for result in results:
             serialized_dict = {key: result[key] for key in result.formats()}
-            serialized_dict['text'] = result.text
+            serialized_dict["text"] = result.text
             serialized.append(serialized_dict)
         return serialized
 
 
 class KernelException(Exception):
     """
     Exception raised when a kernel operation fails.
```

### Comparing `e2b_code_interpreter-0.0.7/pyproject.toml` & `e2b_code_interpreter-0.0.8a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "e2b-code-interpreter"
-version = "0.0.7"
+version = "0.0.8a0"
 description = "E2B Code Interpreter - Stateful code execution"
 authors = ["e2b <hello@e2b.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://e2b.dev/"
 repository = "https://github.com/e2b-dev/e2b-code-interpreter/tree/python"
 packages = [{ include = "e2b_code_interpreter" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 pydantic = ">1, <3"
 websocket-client = "^1.7.0"
-e2b = ">=0.17.0"
+e2b = ">=0.17.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.3.0"
 pytest = "^7.4.0"
 python-dotenv = "^1.0.0"
 pytest-dotenv = "^0.5.2"
```

### Comparing `e2b_code_interpreter-0.0.7/PKG-INFO` & `e2b_code_interpreter-0.0.8a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: e2b-code-interpreter
-Version: 0.0.7
+Version: 0.0.8a0
 Summary: E2B Code Interpreter - Stateful code execution
 Home-page: https://e2b.dev/
 License: Apache-2.0
 Author: e2b
 Author-email: hello@e2b.dev
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: e2b (>=0.17.0)
+Requires-Dist: e2b (>=0.17.1)
 Requires-Dist: pydantic (>1,<3)
 Requires-Dist: websocket-client (>=1.7.0,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/e2b-dev/code-interpreter/issues
 Project-URL: Repository, https://github.com/e2b-dev/e2b-code-interpreter/tree/python
 Description-Content-Type: text/markdown
 
 # Code interpreter extension for Python
```

