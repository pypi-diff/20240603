# Comparing `tmp/digitalhub_runtime_python-0.5.0b5.tar.gz` & `tmp/digitalhub_runtime_python-0.5.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitalhub_runtime_python-0.5.0b5.tar", last modified: Mon May 27 14:12:45 2024, max compression
+gzip compressed data, was "digitalhub_runtime_python-0.5.0b6.tar", last modified: Mon Jun  3 07:26:54 2024, max compression
```

## Comparing `digitalhub_runtime_python-0.5.0b5.tar` & `digitalhub_runtime_python-0.5.0b6.tar`

### file list

```diff
@@ -1,41 +1,40 @@
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-27 14:12:45.724020 digitalhub_runtime_python-0.5.0b5/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    11585 2024-05-20 07:16:51.000000 digitalhub_runtime_python-0.5.0b5/LICENSE.txt
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)    13937 2024-05-27 14:12:45.724020 digitalhub_runtime_python-0.5.0b5/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       17 2024-05-20 07:16:51.000000 digitalhub_runtime_python-0.5.0b5/README.md
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-27 14:12:45.720020 digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1299 2024-05-27 11:24:04.000000 digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-27 14:12:45.720020 digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python/entities/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 07:16:51.000000 digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python/entities/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-27 14:12:45.720020 digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python/entities/functions/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 07:16:51.000000 digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python/entities/functions/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      205 2024-05-20 07:16:51.000000 digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python/entities/functions/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3771 2024-05-27 14:03:59.000000 digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python/entities/functions/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      195 2024-05-20 07:16:51.000000 digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python/entities/functions/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-27 14:12:45.720020 digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python/entities/runs/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 07:16:51.000000 digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python/entities/runs/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      180 2024-05-21 13:57:59.000000 digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python/entities/runs/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1332 2024-05-27 12:55:19.000000 digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python/entities/runs/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      172 2024-05-21 13:58:16.000000 digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python/entities/runs/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-27 14:12:45.720020 digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python/entities/tasks/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 07:16:51.000000 digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python/entities/tasks/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      261 2024-05-22 12:59:26.000000 digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python/entities/tasks/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      437 2024-05-27 12:36:00.000000 digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python/entities/tasks/models.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2565 2024-05-27 14:03:59.000000 digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python/entities/tasks/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      245 2024-05-22 12:59:46.000000 digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python/entities/tasks/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-27 14:12:45.720020 digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python/runtimes/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 07:16:51.000000 digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python/runtimes/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3822 2024-05-27 14:03:59.000000 digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python/runtimes/runtime.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-27 14:12:45.724020 digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python/utils/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5356 2024-05-27 14:03:59.000000 digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python/utils/configuration.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      431 2024-05-23 13:20:09.000000 digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python/utils/functions.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4263 2024-05-23 09:43:32.000000 digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python/utils/inputs.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4680 2024-05-27 11:34:44.000000 digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python/utils/outputs.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1660 2024-05-27 11:24:04.000000 digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python/utils/utils.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-27 14:12:45.724020 digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python.egg-info/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)    13937 2024-05-27 14:12:45.000000 digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python.egg-info/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1359 2024-05-27 14:12:45.000000 digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python.egg-info/SOURCES.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-05-27 14:12:45.000000 digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python.egg-info/dependency_links.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       28 2024-05-27 14:12:45.000000 digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python.egg-info/requires.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       26 2024-05-27 14:12:45.000000 digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python.egg-info/top_level.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1271 2024-05-27 14:08:33.000000 digitalhub_runtime_python-0.5.0b5/pyproject.toml
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-05-27 14:12:45.724020 digitalhub_runtime_python-0.5.0b5/setup.cfg
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-06-03 07:26:54.989973 digitalhub_runtime_python-0.5.0b6/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    11585 2024-05-20 07:16:51.000000 digitalhub_runtime_python-0.5.0b6/LICENSE.txt
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)    13937 2024-06-03 07:26:54.989973 digitalhub_runtime_python-0.5.0b6/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       17 2024-05-20 07:16:51.000000 digitalhub_runtime_python-0.5.0b6/README.md
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-06-03 07:26:54.985973 digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1299 2024-05-27 11:24:04.000000 digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-06-03 07:26:54.985973 digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python/entities/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 07:16:51.000000 digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python/entities/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-06-03 07:26:54.985973 digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python/entities/functions/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 07:16:51.000000 digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python/entities/functions/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      205 2024-05-20 07:16:51.000000 digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python/entities/functions/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3771 2024-05-30 06:51:22.000000 digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python/entities/functions/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      195 2024-05-20 07:16:51.000000 digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python/entities/functions/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-06-03 07:26:54.985973 digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python/entities/runs/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 07:16:51.000000 digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python/entities/runs/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      180 2024-05-21 13:57:59.000000 digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python/entities/runs/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1332 2024-05-30 06:30:52.000000 digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python/entities/runs/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      172 2024-05-21 13:58:16.000000 digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python/entities/runs/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-06-03 07:26:54.989973 digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python/entities/tasks/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 07:16:51.000000 digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python/entities/tasks/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      261 2024-05-22 12:59:26.000000 digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python/entities/tasks/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      437 2024-05-27 12:36:00.000000 digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python/entities/tasks/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2565 2024-05-30 06:51:22.000000 digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python/entities/tasks/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      245 2024-05-22 12:59:46.000000 digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python/entities/tasks/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-06-03 07:26:54.989973 digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python/runtimes/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 07:16:51.000000 digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python/runtimes/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4160 2024-05-31 13:20:04.000000 digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python/runtimes/runtime.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-06-03 07:26:54.989973 digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python/utils/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5356 2024-05-30 06:51:22.000000 digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python/utils/configuration.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4263 2024-05-23 09:43:32.000000 digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python/utils/inputs.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5433 2024-05-31 13:19:29.000000 digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python/utils/outputs.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1660 2024-05-31 12:16:51.000000 digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python/utils/utils.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-06-03 07:26:54.989973 digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python.egg-info/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)    13937 2024-06-03 07:26:54.000000 digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python.egg-info/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1314 2024-06-03 07:26:54.000000 digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-06-03 07:26:54.000000 digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       28 2024-06-03 07:26:54.000000 digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python.egg-info/requires.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       26 2024-06-03 07:26:54.000000 digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python.egg-info/top_level.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1271 2024-06-03 07:25:28.000000 digitalhub_runtime_python-0.5.0b6/pyproject.toml
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-06-03 07:26:54.989973 digitalhub_runtime_python-0.5.0b6/setup.cfg
```

### Comparing `digitalhub_runtime_python-0.5.0b5/LICENSE.txt` & `digitalhub_runtime_python-0.5.0b6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `digitalhub_runtime_python-0.5.0b5/PKG-INFO` & `digitalhub_runtime_python-0.5.0b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub-runtime-python
-Version: 0.5.0b5
+Version: 0.5.0b6
 Summary: Python runtime for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 License:                               Apache License
                                 Version 2.0, January 2004
                              http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python/__init__.py` & `digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python/__init__.py`

 * *Files identical despite different names*

### Comparing `digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python/entities/functions/spec.py` & `digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python/entities/functions/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python/entities/runs/spec.py` & `digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python/entities/runs/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python/entities/tasks/spec.py` & `digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python/entities/tasks/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python/runtimes/runtime.py` & `digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python/runtimes/runtime.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import Callable
 
 from digitalhub_core.runtimes.base import Runtime
 from digitalhub_core.utils.logger import LOGGER
 from digitalhub_runtime_python.utils.configuration import get_function_from_source
 from digitalhub_runtime_python.utils.functions import run_python
 from digitalhub_runtime_python.utils.inputs import get_inputs_parameters
-from digitalhub_runtime_python.utils.outputs import build_status
+from digitalhub_runtime_python.utils.outputs import build_status, parse_outputs
 
 
 class RuntimePython(Runtime):
     """
     Runtime Python class.
     """
 
@@ -59,35 +59,41 @@
 
         Returns
         -------
         dict
             Status of the executed run.
         """
         LOGGER.info("Validating task.")
-        action = self._validate_task(run)
-        executable = self._get_executable(action)
+        self._validate_task(run)
 
         LOGGER.info("Starting task.")
         spec = run.get("spec")
         project = run.get("project")
 
         LOGGER.info("Collecting inputs.")
         fnc_args = self._collect_inputs(spec)
 
         LOGGER.info("Configuring execution.")
-        fnc = self._configure_execution(spec)
+        fnc, wrapped = self._configure_execution(spec)
 
         LOGGER.info("Executing run.")
-        results = self._execute(executable, fnc, project, **fnc_args)
+        if wrapped:
+            results: dict = self._execute(fnc, project, **fnc_args)
+        else:
+            exec_result = self._execute(fnc, **fnc_args)
+            LOGGER.info("Collecting outputs.")
+            results = parse_outputs(exec_result,
+                                    list(spec.get("outputs", {})),
+                                    list(spec.get("values", [])),
+                                    project)
 
-        LOGGER.info("Collecting outputs.")
         status = build_status(
             results,
-            spec.get("outputs", {}),
-            spec.get("values", {}),
+            spec.get("outputs"),
+            spec.get("values"),
         )
 
         # Return run status
         LOGGER.info("Task completed, returning run status.")
         return status
 
     @staticmethod
@@ -137,25 +143,27 @@
             self.tmp_path,
         )
 
     ####################
     # Configuration
     ####################
 
-    def _configure_execution(self, spec: dict) -> Callable:
+    def _configure_execution(self, spec: dict) -> tuple[Callable, bool]:
         """
         Configure execution.
 
         Parameters
         ----------
         spec : dict
             Run spec.
 
         Returns
         -------
         Callable
             Function to execute.
         """
-        return get_function_from_source(
+        fnc = get_function_from_source(
             self.root_path,
             spec.get("source", {}),
         )
+        return fnc, hasattr(fnc, '__wrapped__')
+
```

### Comparing `digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python/utils/configuration.py` & `digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python/utils/inputs.py` & `digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python/utils/inputs.py`

 * *Files identical despite different names*

### Comparing `digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python/utils/outputs.py` & `digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python/utils/outputs.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,14 +48,42 @@
 
         else:
             objects[name] = build_and_load_artifact(name, project_name, item)
 
     return objects
 
 
+def parse_outputs(results: Any, run_outputs: list, run_values: list, project_name: str) -> dict:
+    """
+    Parse outputs.
+
+    Parameters
+    ----------
+    results : Any
+        Function outputs.
+    project : Project
+        Project object.
+
+    Returns
+    -------
+    dict
+        Function outputs.
+    """
+    results_list = listify_results(results)
+    out_list = []
+    for idx, item in enumerate(results_list):
+        try:
+            if isinstance(item, (str, int, float, bool, bytes)):
+                out_list.append(run_values.pop(0))
+            else:
+                out_list.append(run_outputs.pop(0))
+        except IndexError:
+            out_list.append(f"output_{idx}")
+    return collect_outputs(results, out_list, project_name)
+
 def listify_results(results: Any) -> list:
     """
     Listify results.
 
     Parameters
     ----------
     results : Any
```

### Comparing `digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python/utils/utils.py` & `digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python/utils/utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python.egg-info/PKG-INFO` & `digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub-runtime-python
-Version: 0.5.0b5
+Version: 0.5.0b6
 Summary: Python runtime for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 License:                               Apache License
                                 Version 2.0, January 2004
                              http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `digitalhub_runtime_python-0.5.0b5/digitalhub_runtime_python.egg-info/SOURCES.txt` & `digitalhub_runtime_python-0.5.0b6/digitalhub_runtime_python.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,11 +20,10 @@
 digitalhub_runtime_python/entities/tasks/metadata.py
 digitalhub_runtime_python/entities/tasks/models.py
 digitalhub_runtime_python/entities/tasks/spec.py
 digitalhub_runtime_python/entities/tasks/status.py
 digitalhub_runtime_python/runtimes/__init__.py
 digitalhub_runtime_python/runtimes/runtime.py
 digitalhub_runtime_python/utils/configuration.py
-digitalhub_runtime_python/utils/functions.py
 digitalhub_runtime_python/utils/inputs.py
 digitalhub_runtime_python/utils/outputs.py
 digitalhub_runtime_python/utils/utils.py
```

### Comparing `digitalhub_runtime_python-0.5.0b5/pyproject.toml` & `digitalhub_runtime_python-0.5.0b6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digitalhub-runtime-python"
-version = "0.5.0b5"
+version = "0.5.0b6"
 description = "Python runtime for DHCore"
 readme = "README.md"
 authors = [
     { name = "Fondazione Bruno Kessler", email = "dslab@fbk.eu" },
     { name = "Matteo Martini", email = "mmartini@fbk.eu" }
 ]
 license = { file = "LICENSE.txt" }
@@ -35,15 +35,15 @@
 [tool.ruff.extend-per-file-ignores]
 "__init__.py" = ["F401"]
 
 [tool.ruff.pydocstyle]
 convention = "numpy"
 
 [tool.bumpver]
-current_version = "0.5.0b5"
+current_version = "0.5.0b6"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = false
 tag             = false
 push            = false
 
 [tool.bumpver.file_patterns]
```

