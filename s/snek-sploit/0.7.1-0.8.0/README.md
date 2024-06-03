# Comparing `tmp/snek_sploit-0.7.1.tar.gz` & `tmp/snek_sploit-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snek_sploit-0.7.1.tar", max compression
+gzip compressed data, was "snek_sploit-0.8.0.tar", max compression
```

## Comparing `snek_sploit-0.7.1.tar` & `snek_sploit-0.8.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1069 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/LICENSE
--rw-r--r--   0        0        0     1539 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/README.md
--rw-r--r--   0        0        0      686 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     1393 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/snek_sploit/__init__.py
--rw-r--r--   0        0        0        0 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/snek_sploit/lib/__init__.py
--rw-r--r--   0        0        0     4699 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/snek_sploit/lib/context.py
--rw-r--r--   0        0        0     3004 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/snek_sploit/lib/metasploit.py
--rw-r--r--   0        0        0        0 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/snek_sploit/lib/rpc/__init__.py
--rw-r--r--   0        0        0     3086 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/snek_sploit/lib/rpc/auth.py
--rw-r--r--   0        0        0    10952 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/snek_sploit/lib/rpc/consoles.py
--rw-r--r--   0        0        0     7892 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/snek_sploit/lib/rpc/core.py
--rw-r--r--   0        0        0    12331 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/snek_sploit/lib/rpc/db.py
--rw-r--r--   0        0        0      728 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/snek_sploit/lib/rpc/health.py
--rw-r--r--   0        0        0     2676 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/snek_sploit/lib/rpc/jobs.py
--rw-r--r--   0        0        0    19865 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/snek_sploit/lib/rpc/modules.py
--rw-r--r--   0        0        0     1629 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/snek_sploit/lib/rpc/plugins.py
--rw-r--r--   0        0        0    24454 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/snek_sploit/lib/rpc/sessions.py
--rw-r--r--   0        0        0        0 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/snek_sploit/util/__init__.py
--rw-r--r--   0        0        0     1887 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/snek_sploit/util/constants.py
--rw-r--r--   0        0        0      448 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/snek_sploit/util/enums.py
--rw-r--r--   0        0        0      276 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/snek_sploit/util/exceptions.py
--rw-r--r--   0        0        0      955 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/snek_sploit/util/retry.py
--rw-r--r--   0        0        0     2439 1970-01-01 00:00:00.000000 snek_sploit-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-06-03 15:17:20.575342 snek_sploit-0.8.0/LICENSE
+-rw-r--r--   0        0        0     1539 2024-06-03 15:17:20.575342 snek_sploit-0.8.0/README.md
+-rw-r--r--   0        0        0      686 2024-06-03 15:17:20.579342 snek_sploit-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1393 2024-06-03 15:17:20.579342 snek_sploit-0.8.0/snek_sploit/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-03 15:17:20.579342 snek_sploit-0.8.0/snek_sploit/lib/__init__.py
+-rw-r--r--   0        0        0     4699 2024-06-03 15:17:20.579342 snek_sploit-0.8.0/snek_sploit/lib/context.py
+-rw-r--r--   0        0        0     3004 2024-06-03 15:17:20.579342 snek_sploit-0.8.0/snek_sploit/lib/metasploit.py
+-rw-r--r--   0        0        0        0 2024-06-03 15:17:20.579342 snek_sploit-0.8.0/snek_sploit/lib/rpc/__init__.py
+-rw-r--r--   0        0        0     3086 2024-06-03 15:17:20.579342 snek_sploit-0.8.0/snek_sploit/lib/rpc/auth.py
+-rw-r--r--   0        0        0    11202 2024-06-03 15:17:20.579342 snek_sploit-0.8.0/snek_sploit/lib/rpc/consoles.py
+-rw-r--r--   0        0        0     7892 2024-06-03 15:17:20.579342 snek_sploit-0.8.0/snek_sploit/lib/rpc/core.py
+-rw-r--r--   0        0        0    12331 2024-06-03 15:17:20.579342 snek_sploit-0.8.0/snek_sploit/lib/rpc/db.py
+-rw-r--r--   0        0        0      728 2024-06-03 15:17:20.579342 snek_sploit-0.8.0/snek_sploit/lib/rpc/health.py
+-rw-r--r--   0        0        0     2676 2024-06-03 15:17:20.579342 snek_sploit-0.8.0/snek_sploit/lib/rpc/jobs.py
+-rw-r--r--   0        0        0    19865 2024-06-03 15:17:20.579342 snek_sploit-0.8.0/snek_sploit/lib/rpc/modules.py
+-rw-r--r--   0        0        0     1629 2024-06-03 15:17:20.579342 snek_sploit-0.8.0/snek_sploit/lib/rpc/plugins.py
+-rw-r--r--   0        0        0    23073 2024-06-03 15:17:20.579342 snek_sploit-0.8.0/snek_sploit/lib/rpc/sessions.py
+-rw-r--r--   0        0        0        0 2024-06-03 15:17:20.579342 snek_sploit-0.8.0/snek_sploit/util/__init__.py
+-rw-r--r--   0        0        0     1887 2024-06-03 15:17:20.579342 snek_sploit-0.8.0/snek_sploit/util/constants.py
+-rw-r--r--   0        0        0      448 2024-06-03 15:17:20.579342 snek_sploit-0.8.0/snek_sploit/util/enums.py
+-rw-r--r--   0        0        0      276 2024-06-03 15:17:20.579342 snek_sploit-0.8.0/snek_sploit/util/exceptions.py
+-rw-r--r--   0        0        0      955 2024-06-03 15:17:20.579342 snek_sploit-0.8.0/snek_sploit/util/retry.py
+-rw-r--r--   0        0        0     2439 1970-01-01 00:00:00.000000 snek_sploit-0.8.0/PKG-INFO
```

### Comparing `snek_sploit-0.7.1/LICENSE` & `snek_sploit-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.7.1/README.md` & `snek_sploit-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.7.1/pyproject.toml` & `snek_sploit-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snek-sploit"
-version = "0.7.1"
+version = "0.8.0"
 description = "Python RPC client for Metasploit Framework"
 authors = [
     "Jiří Rája <jiri.raja@gmail.com>"
 ]
 maintainers = [
     "Jiří Rája <jiri.raja@gmail.com>"
 ]
```

### Comparing `snek_sploit-0.7.1/snek_sploit/__init__.py` & `snek_sploit-0.8.0/snek_sploit/__init__.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.7.1/snek_sploit/lib/context.py` & `snek_sploit-0.8.0/snek_sploit/lib/context.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.7.1/snek_sploit/lib/metasploit.py` & `snek_sploit-0.8.0/snek_sploit/lib/metasploit.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.7.1/snek_sploit/lib/rpc/auth.py` & `snek_sploit-0.8.0/snek_sploit/lib/rpc/auth.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.7.1/snek_sploit/lib/rpc/consoles.py` & `snek_sploit-0.8.0/snek_sploit/lib/rpc/consoles.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import random
 import string
 from dataclasses import dataclass, asdict
-from typing import List
+from typing import List, Optional, Union
 import time
 
 from snek_sploit.lib.context import ContextBase, Context
 from snek_sploit.util import constants, exceptions
 
 
 @dataclass
@@ -220,34 +220,41 @@
     def destroy(self) -> bool:
         return self._rpc.destroy(self.id)
 
     def tabs(self, line: str) -> List[str]:
         return self._rpc.tabs(self.id, line)
 
     def gather_output(
-        self, timeout: float = None, reading_delay: float = 1, end_check: str = "", end_check_hard_stop: bool = False
+        self,
+        timeout: float = None,
+        reading_delay: float = 1,
+        success_flags: Optional[Union[List[str], str]] = None,
+        success_flag_hard_stop: bool = False,
     ) -> str:
         """
         Gather output from the console.
         :param timeout: The maximum time to wait for the output
         :param reading_delay: Delay between the readings
-        :param end_check: String that is checked regularly to check whether the execution has finished
-        :param end_check_hard_stop: Whether to exit once the `end_check` is found
+        :param success_flags: Flags to indicate the gathered output is enough (one flag == stop gathering)
+        :param success_flag_hard_stop: Whether to exit once a success_flag is found
         :return: Gathered output
         """
-        if timeout is not None:
+        if isinstance(success_flags, str):
+            success_flags = [success_flags]
+
+        if timeout:
             timeout = time.time() + timeout
 
         output = ""
         end_is_nigh = False
-        while (console := self.read()).busy or console.data or not output or (end_check and not end_is_nigh):
+        while (console := self.read()).busy or console.data or not output or (success_flags and not end_is_nigh):
             output += console.data
 
-            if end_check and end_check in console.data:
-                if end_check_hard_stop:
+            if success_flags and any(flag in console.data for flag in success_flags):
+                if success_flag_hard_stop:
                     break
                 end_is_nigh = True  # In case the console is still busy, continue to gather the data
 
             if timeout and time.time() >= timeout:
                 break
 
             time.sleep(reading_delay)
@@ -262,37 +269,37 @@
         self.read()
 
     def execute(
         self,
         command: str,
         timeout: float = None,
         reading_delay: float = 1,
-        end_check: str = "",
-        generate_end_check: bool = True,
-        end_check_hard_stop: bool = False,
+        success_flags: Optional[Union[List[str], str]] = None,
+        generate_success_flag: bool = True,
+        success_flag_hard_stop: bool = False,
     ) -> str:
         """
         Execute a command or a set of commands (separated with `\n`) and gather it's output.
         By default, an end_check is generated and appended to the command to ensure the whole output is captured.
         :param command: Command that will be executed in the console.
         :param timeout: The maximum time to wait for the output
         :param reading_delay: Delay between the readings
-        :param end_check: String that is checked regularly to check whether the execution has finished
-        :param generate_end_check: If `end_check` is empty, generate a custom one and add it to the command
-        :param end_check_hard_stop: Whether to exit once the `end_check` is found and discard the rest of the output
+        :param generate_success_flag: If `success_flags` is undefined, generate a custom one and add it to the command
+        :param success_flags: Flags to indicate the gathered output is enough (one flag == stop gathering)
+        :param success_flag_hard_stop: Whether to exit once a success_flag is found
         :return: Execution output
         """
-        if not end_check and generate_end_check:
-            end_check = "".join(random.choices(string.ascii_letters + string.digits, k=20))
-            command += f"\necho '{end_check}'"
+        if not success_flags and generate_success_flag:
+            success_flags = "".join(random.choices(string.ascii_letters + string.digits, k=20))
+            command += f"\necho '{success_flags}'"
 
         self.clear_buffer()
         self.write(command)
 
-        return self.gather_output(timeout, reading_delay, end_check, end_check_hard_stop)
+        return self.gather_output(timeout, reading_delay, success_flags, success_flag_hard_stop)
 
 
 class Consoles(ContextBase):
     def __init__(self, context: Context):
         super().__init__(context)
         self.rpc = RPCConsoles(context)
```

### Comparing `snek_sploit-0.7.1/snek_sploit/lib/rpc/core.py` & `snek_sploit-0.8.0/snek_sploit/lib/rpc/core.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.7.1/snek_sploit/lib/rpc/db.py` & `snek_sploit-0.8.0/snek_sploit/lib/rpc/db.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.7.1/snek_sploit/lib/rpc/health.py` & `snek_sploit-0.8.0/snek_sploit/lib/rpc/health.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.7.1/snek_sploit/lib/rpc/jobs.py` & `snek_sploit-0.8.0/snek_sploit/lib/rpc/jobs.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.7.1/snek_sploit/lib/rpc/modules.py` & `snek_sploit-0.8.0/snek_sploit/lib/rpc/modules.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.7.1/snek_sploit/lib/rpc/plugins.py` & `snek_sploit-0.8.0/snek_sploit/lib/rpc/plugins.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.7.1/snek_sploit/lib/rpc/sessions.py` & `snek_sploit-0.8.0/snek_sploit/lib/rpc/sessions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 from abc import ABC, abstractmethod
 from typing import List, Dict, Union
 from dataclasses import dataclass, asdict
 import time
 
 from snek_sploit.lib.context import ContextBase, Context
 from snek_sploit.util import constants, exceptions
@@ -435,67 +436,35 @@
         pass
 
     @abstractmethod
     def read(self) -> str:
         pass
 
     @abstractmethod
-    def execute(
-        self,
-        command: str,
-        minimal_execution_time: float,
-        timeout: float,
-        success_flags: List[str],
-        reading_delay: float,
-    ) -> str:
+    def execute(self, command: str, timeout: float, reading_delay: float) -> str:
         pass
 
     @abstractmethod
-    def execute_in_shell(
-        self,
-        executable: str,
-        arguments: List[str],
-        minimal_execution_time: float,
-        timeout: float,
-        success_flags: List[str],
-        reading_delay: float,
-    ) -> str:
+    def execute_in_shell(self, executable: str, arguments: List[str], timeout: float, reading_delay: float) -> str:
         pass
 
-    def gather_output(
-        self,
-        minimal_execution_time: float = 3,
-        timeout: float = None,
-        success_flags: List[str] = None,
-        reading_delay: float = 1,
-    ) -> str:
+    def gather_output(self, timeout: float = None, reading_delay: float = 1) -> str:
         """
         Gather output from the session.
-        :param minimal_execution_time: The minimum amount of seconds to wait before exiting in case no output is read
         :param timeout: The maximum time to wait for the output
-        :param success_flags: Flags to indicate the gathered output is enough (one flag == stop gathering)
         :param reading_delay: Delay between the readings
         :return: Gathered output
         """
-        output = ""
-        timestamp = time.time()
-
         if timeout:
-            timeout = timestamp + max(timeout, minimal_execution_time)
-
-        minimal_execution_time = timestamp + minimal_execution_time
+            timeout = time.time() + timeout
 
-        while (data := self.read()) or (time.time() < minimal_execution_time):
+        output = ""
+        while (data := self.read()) or not output:  # All the data is returned at once
             output += data
 
-            # TODO: switch to regex?
-            # TODO: make sure at least the last 200 characters are tested, since the data can be split randomly?
-            if success_flags and any(flag in data for flag in success_flags):
-                break
-
             if timeout and time.time() >= timeout:
                 break
 
             time.sleep(reading_delay)
 
         return output
 
@@ -514,39 +483,26 @@
 
     def read(self) -> str:
         return self._rpc.shell_read(self.id)
 
     def upgrade_to_meterpreter(self, local_host: str, local_port: int) -> bool:
         return self._rpc.shell_upgrade(self.id, local_host, local_port)
 
-    def execute(
-        self,
-        command: str,
-        minimal_execution_time: float = 3,
-        timeout: float = None,
-        success_flags: List[str] = None,
-        reading_delay: float = 1,
-    ) -> str:
+    def execute(self, command: str, timeout: float = None, reading_delay: float = 1) -> str:
         self.clear_buffer()
         self.write(command)
 
-        return self.gather_output(minimal_execution_time, timeout, success_flags, reading_delay)
+        return self.gather_output(timeout, reading_delay)
 
     def execute_in_shell(
-        self,
-        executable: str,
-        arguments: List[str],
-        minimal_execution_time: float = 3,
-        timeout: float = None,
-        success_flags: List[str] = None,
-        reading_delay: float = 1,
+        self, executable: str, arguments: List[str], timeout: float = None, reading_delay: float = 1
     ) -> str:
         command = " ".join([executable, *arguments])
 
-        return self.execute(command, minimal_execution_time, timeout, success_flags, reading_delay)
+        return self.execute(command, timeout, reading_delay)
 
 
 class SessionMeterpreter(Session):
     @property
     def directory_separator(self):
         return self._rpc.meterpreter_directory_separator(self.id)
 
@@ -567,76 +523,62 @@
 
     def detach(self) -> bool:
         return self._rpc.meterpreter_session_detach(self.id)
 
     def change_transport(self, options: MeterpreterSessionTransportOptions) -> bool:
         return self._rpc.meterpreter_transport_change(self.id, options)
 
-    def execute(
-        self,
-        command: str,
-        minimal_execution_time: float = 3,
-        timeout: float = None,
-        success_flags: List[str] = None,
-        reading_delay: float = 1,
-    ) -> str:
+    def execute(self, command: str, timeout: float = None, reading_delay: float = 1) -> str:
         self.clear_buffer()
         self.write(command)
 
-        return self.gather_output(minimal_execution_time, timeout, success_flags, reading_delay)
+        return self.gather_output(timeout, reading_delay)
 
     def execute_in_shell(
         self,
         executable: str,
         arguments: List[str],
-        minimal_execution_time: float = 3,
         timeout: float = None,
-        success_flags: List[str] = None,
         reading_delay: float = 1,
     ) -> str:
-        # TODO: Remove the process ID from the output? eg. add postprocessing?
+        # TODO: Remove the process ID from the output? eg. add postprocessing? (will be in a separate method/wrapper)
         self.clear_buffer()
         self.run_single(f"execute -f {executable} -c -i -a {' '.join(arguments)}")
 
-        return self.gather_output(minimal_execution_time, timeout, success_flags, reading_delay)
+        return self.gather_output(timeout, reading_delay)
+
+    def gather_output(self, timeout: float = None, reading_delay: float = 1) -> str:
+        output = super().gather_output(timeout, reading_delay)
+        # This is primarily a hotfix for executing in a shell since it returns some info at the beginning
+        if not re.sub(r"Process \d+ created\.\nChannel \d+ created\.\n", "", output, 1):
+            output += super().gather_output(timeout, reading_delay)
+
+        return output
 
 
 class SessionRing(Session):
     def write(self, data: str) -> bool:
         self._rpc.ring_put(self.id, data)
         return True
 
     def read(self) -> str:
         return self._rpc.ring_read(self.id)
 
-    def execute(
-        self,
-        command: str,
-        minimal_execution_time: float = 3,
-        timeout: float = None,
-        success_flags: List[str] = None,
-        reading_delay: float = 1,
-    ) -> str:
+    def execute(self, command: str, timeout: float = None, reading_delay: float = 1) -> str:
         self.clear_buffer()
         self.write(command)
 
-        return self.gather_output(minimal_execution_time, timeout, success_flags, reading_delay)
+        return self.gather_output(timeout, reading_delay)
 
     def execute_in_shell(
-        self,
-        executable: str,
-        arguments: List[str],
-        minimal_execution_time: float = 3,
-        timeout: float = None,
-        success_flags: List[str] = None,
-        reading_delay: float = 1,
+        self, executable: str, arguments: List[str], timeout: float = None, reading_delay: float = 1
     ) -> str:
         command = " ".join([executable, *arguments])
 
-        return self.execute(command, minimal_execution_time, timeout, success_flags, reading_delay)
+        return self.execute(command, timeout, reading_delay)
 
 
 class Sessions(ContextBase):
     def __init__(self, context: Context):
         super().__init__(context)
         self.rpc = RPCSessions(context)
```

### Comparing `snek_sploit-0.7.1/snek_sploit/util/constants.py` & `snek_sploit-0.8.0/snek_sploit/util/constants.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.7.1/snek_sploit/util/retry.py` & `snek_sploit-0.8.0/snek_sploit/util/retry.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.7.1/PKG-INFO` & `snek_sploit-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snek-sploit
-Version: 0.7.1
+Version: 0.8.0
 Summary: Python RPC client for Metasploit Framework
 Home-page: https://github.com/SadParad1se/snek-sploit
 License: MIT
 Keywords: metasploit,msf,rpc,client
 Author: Jiří Rája
 Author-email: jiri.raja@gmail.com
 Maintainer: Jiří Rája
```

