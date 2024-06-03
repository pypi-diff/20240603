# Comparing `tmp/antigranular-0.2.9.tar.gz` & `tmp/antigranular-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antigranular-0.2.9.tar", max compression
+gzip compressed data, was "antigranular-0.3.0.tar", max compression
```

## Comparing `antigranular-0.2.9.tar` & `antigranular-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0      548 2023-09-28 19:46:26.629201 antigranular-0.2.9/antigranular/__init__.py
--rw-r--r--   0        0        0    19143 2023-09-28 19:46:01.661854 antigranular-0.2.9/antigranular/client.py
--rw-r--r--   0        0        0      907 2023-09-28 19:45:26.404541 antigranular-0.2.9/antigranular/config/config.py
--rw-r--r--   0        0        0     3025 2023-09-28 19:45:26.404541 antigranular-0.2.9/antigranular/enclave_client/mock_client.py
--rw-r--r--   0        0        0      803 2023-09-28 19:45:26.404541 antigranular-0.2.9/antigranular/enclave_client/oblv_client.py
--rw-r--r--   0        0        0     1053 2023-09-28 19:45:26.414300 antigranular-0.2.9/antigranular/magics/errors.py
--rw-r--r--   0        0        0     6781 2023-09-28 19:45:26.414300 antigranular-0.2.9/antigranular/magics/magics.py
--rw-r--r--   0        0        0        0 2023-09-28 19:45:26.419417 antigranular-0.2.9/antigranular/models/__init__.py
--rw-r--r--   0        0        0      661 2023-09-28 19:45:26.424517 antigranular-0.2.9/antigranular/models/models.py
--rw-r--r--   0        0        0      149 2023-09-28 19:45:26.427544 antigranular-0.2.9/antigranular/utils/error_print.py
--rw-r--r--   0        0        0      304 2023-09-28 19:45:26.427544 antigranular-0.2.9/antigranular/utils/print_request_id.py
--rw-r--r--   0        0        0    11558 2023-09-28 19:45:26.375641 antigranular-0.2.9/LICENSE
--rw-r--r--   0        0        0      818 2023-09-28 19:46:06.374994 antigranular-0.2.9/pyproject.toml
--rw-r--r--   0        0        0     4252 2023-09-28 19:45:26.387544 antigranular-0.2.9/README.md
--rw-r--r--   0        0        0     5118 1970-01-01 00:00:00.000000 antigranular-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-09-13 06:32:34.950269 antigranular-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4168 2023-12-18 12:01:27.266790 antigranular-0.3.0/README.md
+-rw-r--r--   0        0        0      521 2024-06-03 08:02:02.308766 antigranular-0.3.0/antigranular/__init__.py
+-rw-r--r--   0        0        0    21478 2024-06-03 08:01:42.678772 antigranular-0.3.0/antigranular/client.py
+-rw-r--r--   0        0        0      882 2023-12-18 12:26:41.546765 antigranular-0.3.0/antigranular/config/config.py
+-rw-r--r--   0        0        0     2933 2023-12-18 12:26:48.956765 antigranular-0.3.0/antigranular/enclave_client/mock_client.py
+-rw-r--r--   0        0        0      777 2023-12-18 12:28:16.196762 antigranular-0.3.0/antigranular/enclave_client/oblv_client.py
+-rw-r--r--   0        0        0     1019 2023-09-13 06:32:34.950269 antigranular-0.3.0/antigranular/magics/errors.py
+-rw-r--r--   0        0        0     7016 2024-06-03 08:01:42.678772 antigranular-0.3.0/antigranular/magics/magics.py
+-rw-r--r--   0        0        0        0 2023-09-13 06:32:34.950269 antigranular-0.3.0/antigranular/models/__init__.py
+-rw-r--r--   0        0        0      728 2023-12-06 02:14:02.876124 antigranular-0.3.0/antigranular/models/models.py
+-rw-r--r--   0        0        0      140 2023-09-13 06:32:34.950269 antigranular-0.3.0/antigranular/utils/error_print.py
+-rw-r--r--   0        0        0     1183 2023-12-06 02:13:59.226127 antigranular-0.3.0/antigranular/utils/loading_animation.py
+-rw-r--r--   0        0        0      299 2023-12-06 02:13:59.226127 antigranular-0.3.0/antigranular/utils/print_request_id.py
+-rw-r--r--   0        0        0     1347 2024-06-03 08:01:52.688768 antigranular-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5561 1970-01-01 00:00:00.000000 antigranular-0.3.0/PKG-INFO
```

### Comparing `antigranular-0.2.9/antigranular/config/config.py` & `antigranular-0.3.0/antigranular/config/config.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-"""
-Configuration file for the AG Client.
-"""
-
-AG_EXEC_TIMEOUT = 600  # In seconds
-
-# OAuth Server address to use for authentication
-AG_OAUTH_URL = "https://auth.antigranular.com/oauth/token"
-
-# AG Audience URL as set on OAuth Server
-AG_AUDIENCE_URL = "https://www.antigranular.com"
-
-# Deployed AG Enclave Server URL for competitions, datasets
-AG_ENCLAVE_URL = "https://api.antigranular.com"
-
-# Deployed AG Enclave Server Port - 443 for HTTPS.
-AG_ENCLAVE_PORT = 443
-
-AG_SRV_INFO_URL = "https://portal.antigranular.com/server_info"
-
-AG_PCRS = {
-    "PCR0": "827d1e6374194549061272703b34aa2618d50e856f48541a0bba1a92bf60ba86f4de141b4a5cc448b089c44a4d5fa825",
-    "PCR1": "bcdf05fefccaa8e55bf2c8d6dee9e79bbff31e34bf28a99aa19e6b29c37ee80b214a414b7607236edf26fcb78654e63f",
-    "PCR2": "b2ff57dcc660eb5ab6de9de6c830d2b94c6de592288ee1602477b922797915c81cf151678947207cf0d1fd05be57490b",
-}
+"""
+Configuration file for the AG Client.
+"""
+
+AG_EXEC_TIMEOUT = 600  # In seconds
+
+# OAuth Server address to use for authentication
+AG_OAUTH_URL = "https://auth.antigranular.com/oauth/token"
+
+# AG Audience URL as set on OAuth Server
+AG_AUDIENCE_URL = "https://www.antigranular.com"
+
+# Deployed AG Enclave Server URL for competitions, datasets
+AG_ENCLAVE_URL = "https://api.antigranular.com"
+
+# Deployed AG Enclave Server Port - 443 for HTTPS.
+AG_ENCLAVE_PORT = 443
+
+AG_SRV_INFO_URL = "https://portal.antigranular.com/server_info"
+
+AG_PCRS = {
+    "PCR0": "827d1e6374194549061272703b34aa2618d50e856f48541a0bba1a92bf60ba86f4de141b4a5cc448b089c44a4d5fa825",
+    "PCR1": "bcdf05fefccaa8e55bf2c8d6dee9e79bbff31e34bf28a99aa19e6b29c37ee80b214a414b7607236edf26fcb78654e63f",
+    "PCR2": "b2ff57dcc660eb5ab6de9de6c830d2b94c6de592288ee1602477b922797915c81cf151678947207cf0d1fd05be57490b",
+}
```

### Comparing `antigranular-0.2.9/antigranular/enclave_client/oblv_client.py` & `antigranular-0.3.0/antigranular/enclave_client/oblv_client.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import oblv_client
-from ..config import config
-import uuid
-
-
-def get_oblv_client(ag_client_id, ag_client_secret):
-    """
-    Connect to AG Enclave Server and initialize the Oblv client, AG Enclave Server URL and port from config.
-    """
-    enclave_client = oblv_client.Enclave(
-        config.AG_ENCLAVE_URL,
-        config.AG_ENCLAVE_PORT,
-        False,
-        str(uuid.uuid4()),
-        pcr0=config.AG_PCRS["PCR0"],
-        pcr1=config.AG_PCRS["PCR1"],
-        pcr2=config.AG_PCRS["PCR2"],
-        auth_type="oauth",  # hardcoding OAuth for AG Client
-        client_id=ag_client_id,
-        client_secret=ag_client_secret,
-        oauth_audience=config.AG_AUDIENCE_URL,
-        oauth_url=config.AG_OAUTH_URL,
-    )
-
-    enclave_client.attest()
-    return enclave_client
+import oblv_client
+from ..config import config
+import uuid
+
+
+def get_oblv_client(ag_client_id, ag_client_secret):
+    """
+    Connect to AG Enclave Server and initialize the Oblv client, AG Enclave Server URL and port from config.
+    """
+    enclave_client = oblv_client.Enclave(
+        config.AG_ENCLAVE_URL,
+        config.AG_ENCLAVE_PORT,
+        False,
+        str(uuid.uuid4()),
+        pcr0=config.AG_PCRS["PCR0"],
+        pcr1=config.AG_PCRS["PCR1"],
+        pcr2=config.AG_PCRS["PCR2"],
+        auth_type="oauth",  # hardcoding OAuth for AG Client
+        client_id=ag_client_id,
+        client_secret=ag_client_secret,
+        oauth_audience=config.AG_AUDIENCE_URL,
+        oauth_url=config.AG_OAUTH_URL,
+    )
+
+    enclave_client.attest()
+    return enclave_client
```

### Comparing `antigranular-0.2.9/antigranular/magics/errors.py` & `antigranular-0.3.0/antigranular/magics/errors.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-import os
-import signal
-from IPython import get_ipython
-from IPython.core.ultratb import AutoFormattedTB
-
-class AGRuntimeError(Exception):
-    def __init__(self, etype="Error", evalue="AG Runtime Error", msg=None):
-        self.error_data = f"{etype}:\n{evalue}"
-        self.tb = evalue
-
-    def __str__(self):
-        error_msg = f"{self.error_data}"
-        if self.tb:
-            error_msg += f"\nServer Traceback:\n{self.tb}"
-        return error_msg
-
-
-class AGTimeOutError(Exception):
-    def __init__(self, etype="Error", evalue="AG TimeOut Error", msg=None):
-        self.error_data = f"{etype}:\n{evalue}"
-        self.tb = "Client TimeOut while waiting for server output"
-
-    def __str__(self):
-        error_msg = f"{self.error_data}"
-        if self.tb:
-            error_msg += f"\nServer Traceback:\n{self.tb}"
-        return error_msg
-
-
-def custom_exc(shell, etype, evalue, tb, tb_offset=None):
-    return
-
-# Use our custom exception handler
-get_ipython().set_custom_exc((AGRuntimeError,), custom_exc)
+import os
+import signal
+from IPython import get_ipython
+from IPython.core.ultratb import AutoFormattedTB
+
+class AGRuntimeError(Exception):
+    def __init__(self, etype="Error", evalue="AG Runtime Error", msg=None):
+        self.error_data = f"{etype}:\n{evalue}"
+        self.tb = evalue
+
+    def __str__(self):
+        error_msg = f"{self.error_data}"
+        if self.tb:
+            error_msg += f"\nServer Traceback:\n{self.tb}"
+        return error_msg
+
+
+class AGTimeOutError(Exception):
+    def __init__(self, etype="Error", evalue="AG TimeOut Error", msg=None):
+        self.error_data = f"{etype}:\n{evalue}"
+        self.tb = "Client TimeOut while waiting for server output"
+
+    def __str__(self):
+        error_msg = f"{self.error_data}"
+        if self.tb:
+            error_msg += f"\nServer Traceback:\n{self.tb}"
+        return error_msg
+
+
+def custom_exc(shell, etype, evalue, tb, tb_offset=None):
+    return
+
+# Use our custom exception handler
+get_ipython().set_custom_exc((AGRuntimeError,), custom_exc)
```

### Comparing `antigranular-0.2.9/antigranular/magics/magics.py` & `antigranular-0.3.0/antigranular/magics/magics.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,185 +1,192 @@
-from IPython.display import display, HTML
-from IPython.core.magic import (
-    Magics,
-    magics_class,
-    line_cell_magic,
-)
-from IPython import get_ipython
-
-import json
-import base64
-import pickle
-import time
-from typing import Union
-from requests import HTTPError
-
-from ..enclave_client.mock_client import MockEnclaveClient
-from ..enclave_client.oblv_client import oblv_client
-from ..utils.error_print import eprint
-from .errors import AGRuntimeError, AGTimeOutError
-from ..config import config
-from ..utils.print_request_id import print_request_id
-
-@magics_class
-class AGMagic(Magics):
-    """
-    Provides %%ag cell magic and private python code execution on Antigranular server
-    """
-
-    session_id: str
-    # user_name: str
-    ag_server: Union[oblv_client.Enclave, MockEnclaveClient]
-
-    @classmethod
-    def load_oblv_client(cls, ag_server, session_id):
-        cls.ag_server = ag_server
-        cls.session_id = session_id
-        # cls.user_name = user_name
-
-    @line_cell_magic
-    def ag(self, line, cell=None):
-        """
-        Executes the provided code on the Antigranular server.
-
-        Parameters:
-            line (str): The code in a single line.
-            cell (str): The code in a cell format.
-
-        Returns:
-            None
-        """
-        if cell is None:
-            print("Please call ag as a cell magic using '%%ag'")
-            return
-        else:
-            try:
-                self.execute(cell)
-            # except any exception
-            except KeyboardInterrupt:
-                res = self.interrupt_kernel()
-                if res["status"] == "ok":
-                    # return interrupt message
-                    eprint("Kernel interrupted successfully")
-                else:
-                    eprint("Error while interrupting kernel")
-                    eprint(res)
-
-    def execute(self, code: str):
-        """
-        Executes the code on the Antigranular server.
-
-        Parameters:
-            code (str): The code to be executed.
-
-        Returns:
-            None
-        """
-        try:
-            res = self.ag_server.post(
-                f"{self.ag_server.url}:{self.ag_server.port}/sessions/execute",
-                json={"session_id": self.session_id, "code": code},
-            )
-        except Exception as err:
-            raise ConnectionError(f"Error calling /execute: {str(err)}")
-        else:
-            if res.status_code != 200:
-                raise HTTPError(
-                    print_request_id(f"Error while requesting AG server to execute the code, HTTP status code: {res.status_code}, message: {res.text}", res)
-                )
-            self.get_output()
-
-    def interrupt_kernel(self) -> dict:
-        try:
-            res = self.ag_server.post(
-                f"{self.ag_server.url}:{self.ag_server.port}/sessions/interrupt-kernel",
-                json={"session_id": self.session_id},
-            )
-        except Exception as err:
-            raise ConnectionError(
-                f"Error calling /sessions/interrupt-kernel: {str(err)}"
-            )
-        else:
-            if res.status_code != 200:
-                raise HTTPError(
-                    print_request_id(f"Error while requesting AG server to interrupt the kernel, HTTP status code: {res.status_code}, message: {res.text}", res)
-                )
-            return json.loads(res.text)
-
-    def get_output(self):
-        """
-        Retrieves the code execution output from the Antigranular server.
-        """
-        count = 1
-
-        while True:
-            if count > config.AG_EXEC_TIMEOUT:
-                eprint("Error : AG execution timeout.")
-                break
-            try:
-                res = self.ag_server.get(
-                    f"{self.ag_server.url}:{self.ag_server.port}/sessions/output",
-                    params={"session_id": self.session_id},
-                )
-            except Exception as err:
-                raise ConnectionError(
-                    f"Error during code execution on AG Server: {str(err)}"
-                )
-            if res.status_code != 200:
-                raise HTTPError(
-                    print_request_id(f"Error while requesting AG server for output, HTTP status code: {res.status_code}, message: {res.text}", res)
-                )
-            kernel_messages = json.loads(res.text)["output_list"]
-            for message in kernel_messages:
-                if message["msg_type"] == "status":
-                    if message["content"]["execution_state"] == "idle":
-                        return
-                elif message["msg_type"] == "stream":
-                    if message["content"]["name"] == "stdout":
-                        print(message["content"]["text"])
-                    elif message["content"]["name"] == "stderr":
-                        eprint(message["content"]["text"])
-
-                elif message["msg_type"] == "error":
-                    tb_str = ""
-                    for tb in message["content"]["traceback"]:
-                        tb_str += tb
-
-                    print(tb_str)
-                    raise AGRuntimeError(
-                        etype=str(message["content"]["evalue"]),
-                        evalue="RuntimeError",
-                        msg=tb_str,
-                    )
-
-                elif message["msg_type"] == "ag_export_value":
-                    try:
-                        user_ns = get_ipython().user_ns
-                        data = message["content"]
-                        for name, value in data.items():
-                            user_ns[name] = pickle.loads(base64.b64decode(value))
-                            print(
-                                "Setting up exported variable in local environment:",
-                                name,
-                            )
-
-                    except Exception as err:
-                        raise ValueError(
-                            f"Error while parsing export values message: {str(err)}"
-                        )
-            time.sleep(1)
-            count += 1
-
-    @staticmethod
-    def load_ag_magic():
-        """
-        Loads the AGMagic class as a magic in the IPython session.
-        """
-        ipython = get_ipython()
-        if ipython is None:
-            raise RuntimeError(
-                "This function can only be called from an IPython session"
-            )
-        ipython.register_magics(AGMagic)
-        print(
-            "Cell magic '%%ag' registered successfully, use `%%ag` in a notebook cell to execute your python code on Antigranular private python server"
-        )
+from IPython.display import display, HTML
+from IPython.core.magic import (
+    Magics,
+    magics_class,
+    line_cell_magic,
+)
+from IPython import get_ipython
+
+import json
+import base64
+import pickle
+import time
+from typing import Union
+from requests import HTTPError
+
+from ..enclave_client.mock_client import MockEnclaveClient
+from ..enclave_client.oblv_client import oblv_client
+from ..utils.error_print import eprint
+from .errors import AGRuntimeError, AGTimeOutError
+from ..config import config
+from ..utils.print_request_id import print_request_id
+
+@magics_class
+class AGMagic(Magics):
+    """
+    Provides %%ag cell magic and private python code execution on Antigranular server
+    """
+
+    session_id: str
+    # user_name: str
+    ag_server: Union[oblv_client.Enclave, MockEnclaveClient]
+
+    @classmethod
+    def load_oblv_client(cls, ag_server, session_id):
+        cls.ag_server = ag_server
+        cls.session_id = session_id
+        # cls.user_name = user_name
+
+    @line_cell_magic
+    def ag(self, line, cell=None):
+        """
+        Executes the provided code on the Antigranular server.
+
+        Parameters:
+            line (str): The code in a single line.
+            cell (str): The code in a cell format.
+
+        Returns:
+            None
+        """
+        if cell is None:
+            print("Please call ag as a cell magic using '%%ag'")
+            return
+        else:
+            try:
+                self.execute(cell)
+            # except any exception
+            except KeyboardInterrupt:
+                res = self.interrupt_kernel()
+                if res["status"] == "ok":
+                    # return interrupt message
+                    eprint("Kernel interrupted successfully")
+                else:
+                    eprint("Error while interrupting kernel")
+                    eprint(res)
+
+    def execute(self, code: str):
+        """
+        Executes the code on the Antigranular server.
+
+        Parameters:
+            code (str): The code to be executed.
+
+        Returns:
+            None
+        """
+        try:
+            res = self.ag_server.post(
+                f"{self.ag_server.url}:{self.ag_server.port}/sessions/execute",
+                json={"session_id": self.session_id, "code": code},
+            )
+            res_body_dict = json.loads(res.body)
+        except Exception as err:
+            raise ConnectionError(f"Error calling /execute: {str(err)}")
+        else:
+            if res.status_code != 200:
+                raise HTTPError(
+                    print_request_id(f"Error while requesting AG server to execute the code, HTTP status code: {res.status_code}, message: {res.text}", res)
+                )
+            self.get_output(res_body_dict.get('message_id'))
+
+    def interrupt_kernel(self) -> dict:
+        try:
+            res = self.ag_server.post(
+                f"{self.ag_server.url}:{self.ag_server.port}/sessions/interrupt-kernel",
+                json={"session_id": self.session_id},
+            )
+        except Exception as err:
+            raise ConnectionError(
+                f"Error calling /sessions/interrupt-kernel: {str(err)}"
+            )
+        else:
+            if res.status_code != 200:
+                raise HTTPError(
+                    print_request_id(f"Error while requesting AG server to interrupt the kernel, HTTP status code: {res.status_code}, message: {res.text}", res)
+                )
+            return json.loads(res.text)
+
+    def get_output(self, message_id: str):
+        """
+        Retrieves the code execution output from the Antigranular server.
+        """
+        count = 1
+        idle_state_reached = False
+
+        while True:
+            if count > config.AG_EXEC_TIMEOUT:
+                eprint("Error : AG execution timeout.")
+                break
+
+            if idle_state_reached:
+                return
+
+            try:
+                res = self.ag_server.get(
+                    f"{self.ag_server.url}:{self.ag_server.port}/sessions/output",
+                    params={"session_id": self.session_id},
+                )
+            except Exception as err:
+                raise ConnectionError(
+                    f"Error during code execution on AG Server: {str(err)}"
+                )
+            if res.status_code != 200:
+                raise HTTPError(
+                    print_request_id(f"Error while requesting AG server for output, HTTP status code: {res.status_code}, message: {res.text}", res)
+                )
+            kernel_messages = json.loads(res.text)["output_list"]
+            for message in kernel_messages:
+                if message.get("parent_header", {}).get("msg_id") == message_id:
+                    if message["msg_type"] == "status":
+                        if message["content"]["execution_state"] == "idle":
+                            idle_state_reached = True
+                    elif message["msg_type"] == "stream":
+                        if message["content"]["name"] == "stdout":
+                            print(message["content"]["text"])
+                        elif message["content"]["name"] == "stderr":
+                            eprint(message["content"]["text"])
+
+                    elif message["msg_type"] == "error":
+                        tb_str = ""
+                        for tb in message["content"]["traceback"]:
+                            tb_str += tb
+
+                        print(tb_str)
+                        raise AGRuntimeError(
+                            etype=str(message["content"]["evalue"]),
+                            evalue="RuntimeError",
+                            msg=tb_str,
+                        )
+
+                    elif message["msg_type"] == "ag_export_value":
+                        try:
+                            user_ns = get_ipython().user_ns
+                            data = message["content"]
+                            for name, value in data.items():
+                                user_ns[name] = pickle.loads(base64.b64decode(value))
+                                print(
+                                    "Setting up exported variable in local environment:",
+                                    name,
+                                )
+
+                        except Exception as err:
+                            raise ValueError(
+                                f"Error while parsing export values message: {str(err)}"
+                            )
+            time.sleep(1)
+            count += 1
+
+    @staticmethod
+    def load_ag_magic():
+        """
+        Loads the AGMagic class as a magic in the IPython session.
+        """
+        ipython = get_ipython()
+        if ipython is None:
+            raise RuntimeError(
+                "This function can only be called from an IPython session"
+            )
+        ipython.register_magics(AGMagic)
+        print(
+            "Cell magic '%%ag' registered successfully, use `%%ag` in a notebook cell to execute your python code on Antigranular private python server"
+        )
```

### Comparing `antigranular-0.2.9/LICENSE` & `antigranular-0.3.0/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `antigranular-0.2.9/README.md` & `antigranular-0.3.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-# Privacy Unleashed: Working with Antigranular
-Antigranular is a community-led, open-source platform that combines confidential computing with differential privacy. This integration fosters a secure environment to handle and fully utilize unseen data.
-### Connect to Antigranular 
-You can activate Antigranular using the magic command `%%ag`. Any code that follows `%%ag` will run on our remote server. This server operates under restricted conditions, allowing only methods that guarantee differential privacy.
-
-Install the Antigranular package using `pip`:
-```python
-!pip install antigranular
-```
-Import the `Antigranular` library:
-```python
-import antigranular as ag
-```
-To connect to the AG Enclave Server, use your client credentials and either a dataset or competition ID:
-```python
-ag_client = ag.login(user_id="<user_id>", user_secret="<user_secret>",  competition="<competition_name>")
-```
-or
-```python
-ag_client = ag.login(user_id="<user_id>", user_secret="<user_secret>", dataset="<dataset_name>")
-```
-A succesful login will register the cell magic `%%ag`. 
-
-### Loading Private Datasets 
-Private datasets can be loaded as `PrivateDataFrames` and `PrivateSeries` using the `ag_utils` library. `ag_utils` is a package locally installed on the remote server, which eliminates the need to install anything other than the antigranular package.
-
-The `load_dataset()` method allows for obtaining a dictionary of private objects. The structure of the response dictionary, along with the dataset path and private object names, will be specified during the competition.
-```python
-%%ag
-from op_pandas import PrivateDataFrame, PrivateSeries
-from ag_utils import load_dataset 
-"""
-Sample response structure
-{
-    train_x : priv_train_x,
-    train_y : priv_train_y,
-    test_x : priv_test_x
-}
-"""
-# Obtaining the dictionary containing private objects
-response = load_dataset("<path_to_dataset>")
-
-# Unpacking the response dictionary
-train_x = response["train_x"]
-train_y = response["train_y"]
-test_x = response["test_x"]
-```
-### Exporting Objects
-Since the code following `%%ag` runs in a highly restricted environment, it's necessary to export differentially private objects to the local environment for further analysis. The `export` method in `ag_utils` allows data objects to be exported.
-##### **API info**: `export(obj, variable_name:str)`
-
-This command exports the remote object to the local environment and assigns it to the specified variable name. Note that `PrivateSeries` and `PrivateDataFrame` objects cannot be exported and will raise an error if you attempt to do so.
-
-```python 
-%%ag
-from ag_utils import export
-train_info = train_x.describe(eps=1)
-export(train_info , 'variable_name')
-```
-Once exported, you can perform any kind of data analysis on the differentially private object.
-
-```python
-# Local code block
-print(variable_name)
---------------------------------------
-                    Age         Salary
-    count  99987.000000   99987.000000
-    mean      38.435953  120009.334336
-    std       12.167379   46255.486093
-    min       18.257448   40048.259037
-    25%       27.185189   80057.639960
-    50%       38.210860  120380.291216
-    75%       49.147724  159835.637091
-    max       59.282932  199920.664706
-```
-
-## Libraries Supported
-
-
-- **`pandas`**: An adaptable data manipulation library offering efficient data structures and tools for data analysis and manipulation.
-
-- **`op_pandas`**: A wrapped library specifically designed for differentially private data manipulation within the Pandas framework. It enhances privacy-preserving techniques and enables privacy-aware data processing.
-
-- **`op_diffprivlib`**: A differentially private library that provides various privacy-preserving algorithms and mechanisms for machine learning and data analysis tasks.
-
-- **`op_smartnoise`**: A library focused on privacy-preserving analysis using the SmartNoise framework. It provides tools for differential privacy and secure computation.
-
+#### Privacy Unleashed: Working with Antigranular
+Antigranular is a community-led, open-source platform that combines confidential computing with differential privacy. This integration fosters a secure environment to handle and fully utilize unseen data.
+### Connect to Antigranular 
+You can activate Antigranular using the magic command `%%ag`. Any code that follows `%%ag` will run on our remote server. This server operates under restricted conditions, allowing only methods that guarantee differential privacy.
+
+Install the Antigranular package using `pip`:
+```python
+!pip install antigranular
+```
+Import the `Antigranular` library:
+```python
+import antigranular as ag
+```
+To connect to the AG Enclave Server, use your client credentials and either a dataset or competition ID:
+```python
+ag_client = ag.login(user_id="<user_id>", user_secret="<user_secret>",  competition="<competition_name>")
+```
+or
+```python
+ag_client = ag.login(user_id="<user_id>", user_secret="<user_secret>", dataset="<dataset_name>")
+```
+A succesful login will register the cell magic `%%ag`. 
+
+### Loading Private Datasets 
+Private datasets can be loaded as `PrivateDataFrames` and `PrivateSeries` using the `ag_utils` library. `ag_utils` is a package locally installed on the remote server, which eliminates the need to install anything other than the antigranular package.
+
+The `load_dataset()` method allows for obtaining a dictionary of private objects. The structure of the response dictionary, along with the dataset path and private object names, will be specified during the competition.
+```python
+%%ag
+from op_pandas import PrivateDataFrame, PrivateSeries
+from ag_utils import load_dataset 
+"""
+Sample response structure
+{
+    train_x : priv_train_x,
+    train_y : priv_train_y,
+    test_x : priv_test_x
+}
+"""
+# Obtaining the dictionary containing private objects
+response = load_dataset("<path_to_dataset>")
+
+# Unpacking the response dictionary
+train_x = response["train_x"]
+train_y = response["train_y"]
+test_x = response["test_x"]
+```
+### Exporting Objects
+Since the code following `%%ag` runs in a highly restricted environment, it's necessary to export differentially private objects to the local environment for further analysis. The `export` method in `ag_utils` allows data objects to be exported.
+##### **API info**: `export(obj, variable_name:str)`
+
+This command exports the remote object to the local environment and assigns it to the specified variable name. Note that `PrivateSeries` and `PrivateDataFrame` objects cannot be exported and will raise an error if you attempt to do so.
+
+```python 
+%%ag
+from ag_utils import export
+train_info = train_x.describe(eps=1)
+export(train_info , 'variable_name')
+```
+Once exported, you can perform any kind of data analysis on the differentially private object.
+
+```python
+# Local code block
+print(variable_name)
+--------------------------------------
+                    Age         Salary
+    count  99987.000000   99987.000000
+    mean      38.435953  120009.334336
+    std       12.167379   46255.486093
+    min       18.257448   40048.259037
+    25%       27.185189   80057.639960
+    50%       38.210860  120380.291216
+    75%       49.147724  159835.637091
+    max       59.282932  199920.664706
+```
+
+## Libraries Supported
+
+
+- **`pandas`**: An adaptable data manipulation library offering efficient data structures and tools for data analysis and manipulation.
+
+- **`op_pandas`**: A wrapped library specifically designed for differentially private data manipulation within the Pandas framework. It enhances privacy-preserving techniques and enables privacy-aware data processing.
+
+- **`op_diffprivlib`**: A differentially private library that provides various privacy-preserving algorithms and mechanisms for machine learning and data analysis tasks.
+
+- **`op_smartnoise`**: A library focused on privacy-preserving analysis using the SmartNoise framework. It provides tools for differential privacy and secure computation.
+
 - **`op_opendp`**: A library that offers differentially private data analysis and algorithms based on the OpenDP project. It provides privacy-preserving methods and tools for statistical analysis.
```

### Comparing `antigranular-0.2.9/PKG-INFO` & `antigranular-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 Metadata-Version: 2.1
 Name: antigranular
-Version: 0.2.9
+Version: 0.3.0
 Summary: Antigranular is a community-driven, open-source platform that merges confidential computing and differential privacy. This creates a secure environment for handling and unlocking the full potential of unseen data..
 Author: Oblivious Software
 Author-email: support@oblivious.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: diffprivlib (>=0.6.2,<0.7.0)
+Provides-Extra: ml-frameworks
 Requires-Dist: ipython (>=7.34.0,<8.0.0)
+Requires-Dist: numpy (>=1.19.0,<2.0.0) ; python_version >= "3.8" and python_version < "3.12"
+Requires-Dist: numpy (>=1.26.0,<2.0.0) ; python_version >= "3.12" and python_version < "4.0"
 Requires-Dist: oblv-client (>=0.1.15,<0.2.0)
-Requires-Dist: onnx (>=1.14.0,<2.0.0)
-Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: onnx (>=1.15.0,<2.0.0) ; python_version >= "3.8" and python_version < "3.12"
+Requires-Dist: pandas (>=1.5.3,<2.0.0) ; python_version >= "3.8" and python_version < "3.12"
+Requires-Dist: pandas (>=2.1.4,<3.0.0) ; python_version >= "3.12" and python_version <= "4.0"
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: torch (>=1.10.0,<2.0.0) ; extra == "ml-frameworks"
 Description-Content-Type: text/markdown
 
-# Privacy Unleashed: Working with Antigranular
+#### Privacy Unleashed: Working with Antigranular
 Antigranular is a community-led, open-source platform that combines confidential computing with differential privacy. This integration fosters a secure environment to handle and fully utilize unseen data.
 ### Connect to Antigranular 
 You can activate Antigranular using the magic command `%%ag`. Any code that follows `%%ag` will run on our remote server. This server operates under restricted conditions, allowing only methods that guarantee differential privacy.
 
 Install the Antigranular package using `pip`:
 ```python
 !pip install antigranular
```

