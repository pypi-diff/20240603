# Comparing `tmp/ataskq-0.5.1.tar.gz` & `tmp/ataskq-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ataskq-0.5.1.tar", last modified: Sun Apr 21 07:22:24 2024, max compression
+gzip compressed data, was "ataskq-6.0.0.tar", last modified: Mon Jun  3 13:22:32 2024, max compression
```

## Comparing `ataskq-0.5.1.tar` & `ataskq-6.0.0.tar`

### file list

```diff
@@ -1,49 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 07:22:24.629826 ataskq-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-21 07:22:11.000000 ataskq-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-21 07:22:24.629826 ataskq-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-21 07:22:11.000000 ataskq-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 07:22:24.625826 ataskq-0.5.1/ataskq/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12687 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/ataskq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 07:22:24.625826 ataskq-0.5.1/ataskq/handler/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17044 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/handler/db_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/handler/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/handler/postgresql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/handler/rest_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/handler/sqlite3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/imodel.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    15869 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 07:22:24.625826 ataskq-0.5.1/ataskq/server/
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/server/form_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6085 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 07:22:24.629826 ataskq-0.5.1/ataskq/server/www/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 07:22:24.629826 ataskq-0.5.1/ataskq/server/www/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    24285 2024-04-21 07:22:19.000000 ataskq-0.5.1/ataskq/server/www/assets/index-MiCEdQXI.js
--rw-r--r--   0 runner    (1001) docker     (127)    70928 2024-04-21 07:22:19.000000 ataskq-0.5.1/ataskq/server/www/assets/index-MiCEdQXI.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-21 07:22:19.000000 ataskq-0.5.1/ataskq/server/www/assets/index-_NWmBfbC.css
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-21 07:22:19.000000 ataskq-0.5.1/ataskq/server/www/ataskq-32.png
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-21 07:22:19.000000 ataskq-0.5.1/ataskq/server/www/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-21 07:22:19.000000 ataskq-0.5.1/ataskq/server/www/index.html
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-21 07:22:19.000000 ataskq-0.5.1/ataskq/server/www/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 07:22:24.629826 ataskq-0.5.1/ataskq/tasks_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/tasks_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/tasks_utils/counter_task.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/tasks_utils/write_to_file_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/test_0.py
--rw-r--r--   0 runner    (1001) docker     (127)    16313 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/test_ataskq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/test_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-21 07:22:19.000000 ataskq-0.5.1/ataskq/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 07:22:24.629826 ataskq-0.5.1/ataskq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-21 07:22:24.000000 ataskq-0.5.1/ataskq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-21 07:22:24.000000 ataskq-0.5.1/ataskq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 07:22:24.000000 ataskq-0.5.1/ataskq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-21 07:22:24.000000 ataskq-0.5.1/ataskq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-21 07:22:19.000000 ataskq-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 07:22:24.629826 ataskq-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:22:32.219138 ataskq-6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-06-03 13:22:11.000000 ataskq-6.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-06-03 13:22:32.219138 ataskq-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-06-03 13:22:11.000000 ataskq-6.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:22:32.215138 ataskq-6.0.0/ataskq/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-06-03 13:22:11.000000 ataskq-6.0.0/ataskq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-06-03 13:22:11.000000 ataskq-6.0.0/ataskq/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:22:32.215138 ataskq-6.0.0/ataskq/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-06-03 13:22:11.000000 ataskq-6.0.0/ataskq/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-06-03 13:22:11.000000 ataskq-6.0.0/ataskq/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-06-03 13:22:11.000000 ataskq-6.0.0/ataskq/config/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-06-03 13:22:11.000000 ataskq-6.0.0/ataskq/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-06-03 13:22:11.000000 ataskq-6.0.0/ataskq/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:22:32.215138 ataskq-6.0.0/ataskq/handler/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-06-03 13:22:11.000000 ataskq-6.0.0/ataskq/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17169 2024-06-03 13:22:11.000000 ataskq-6.0.0/ataskq/handler/db_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7419 2024-06-03 13:22:11.000000 ataskq-6.0.0/ataskq/handler/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-06-03 13:22:11.000000 ataskq-6.0.0/ataskq/handler/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-06-03 13:22:11.000000 ataskq-6.0.0/ataskq/handler/rest_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-06-03 13:22:11.000000 ataskq-6.0.0/ataskq/handler/sqlite3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-06-03 13:22:11.000000 ataskq-6.0.0/ataskq/imodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-06-03 13:22:11.000000 ataskq-6.0.0/ataskq/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15975 2024-06-03 13:22:11.000000 ataskq-6.0.0/ataskq/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-06-03 13:22:11.000000 ataskq-6.0.0/ataskq/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:22:32.215138 ataskq-6.0.0/ataskq/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-06-03 13:22:11.000000 ataskq-6.0.0/ataskq/server/background.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-06-03 13:22:11.000000 ataskq-6.0.0/ataskq/server/form_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-06-03 13:22:11.000000 ataskq-6.0.0/ataskq/server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:22:32.215138 ataskq-6.0.0/ataskq/server/www/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:22:32.219138 ataskq-6.0.0/ataskq/server/www/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    24285 2024-06-03 13:22:19.000000 ataskq-6.0.0/ataskq/server/www/assets/index-MiCEdQXI.js
+-rw-r--r--   0 runner    (1001) docker     (127)    70928 2024-06-03 13:22:19.000000 ataskq-6.0.0/ataskq/server/www/assets/index-MiCEdQXI.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-06-03 13:22:19.000000 ataskq-6.0.0/ataskq/server/www/assets/index-_NWmBfbC.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-06-03 13:22:19.000000 ataskq-6.0.0/ataskq/server/www/ataskq-32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-06-03 13:22:19.000000 ataskq-6.0.0/ataskq/server/www/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-06-03 13:22:19.000000 ataskq-6.0.0/ataskq/server/www/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-03 13:22:19.000000 ataskq-6.0.0/ataskq/server/www/version.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12029 2024-06-03 13:22:11.000000 ataskq-6.0.0/ataskq/taskq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:22:32.219138 ataskq-6.0.0/ataskq/tasks_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-06-03 13:22:11.000000 ataskq-6.0.0/ataskq/tasks_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-06-03 13:22:11.000000 ataskq-6.0.0/ataskq/tasks_utils/counter_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-06-03 13:22:11.000000 ataskq-6.0.0/ataskq/tasks_utils/write_to_file_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-06-03 13:22:11.000000 ataskq-6.0.0/ataskq/test_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17785 2024-06-03 13:22:11.000000 ataskq-6.0.0/ataskq/test_ataskq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-06-03 13:22:11.000000 ataskq-6.0.0/ataskq/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-06-03 13:22:11.000000 ataskq-6.0.0/ataskq/test_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-06-03 13:22:11.000000 ataskq-6.0.0/ataskq/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-06-03 13:22:11.000000 ataskq-6.0.0/ataskq/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-06-03 13:22:11.000000 ataskq-6.0.0/ataskq/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-06-03 13:22:19.000000 ataskq-6.0.0/ataskq/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:22:32.219138 ataskq-6.0.0/ataskq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-06-03 13:22:32.000000 ataskq-6.0.0/ataskq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-06-03 13:22:32.000000 ataskq-6.0.0/ataskq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 13:22:32.000000 ataskq-6.0.0/ataskq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-03 13:22:32.000000 ataskq-6.0.0/ataskq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-06-03 13:22:19.000000 ataskq-6.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 13:22:32.219138 ataskq-6.0.0/setup.cfg
```

### Comparing `ataskq-0.5.1/LICENSE` & `ataskq-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ataskq-0.5.1/PKG-INFO` & `ataskq-6.0.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: ataskq
-Version: 0.5.1
-Summary: An in process task queue for distributed computing systems.
+Version: 6.0.0
+Summary: Easily create and run tasks (=function calls) with almost seamless transition between Local development and Distributed deployment.
 Project-URL: Homepage, https://github.com/innoviz-swt/a-task-queue
 Project-URL: Issues, https://github.com/innoviz-swt/a-task-queue/issues
 Keywords: python,task,queue,distributed systems,distributed computing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # a-task-queue
-An in process task queue for distributed computing systems.
+Easily create and run tasks (=function calls) with almost seamless transition between Local development and Distributed deployment."
 
 ## Usage
 ```python
 from ataskq import TaskQ, Task, targs
 
 # create  job
 tr = TaskQ().create_job()
@@ -28,15 +28,15 @@
 tr.add_tasks([
     Task(entrypoint='ataskq.tasks_utils.hello_world'),
     Task(entrypoint='ataskq.tasks_utils.dummy_args_task', targs=targs(
         'arg0', 'arg1', kwarg1=10, kwarg2='this is kwarg2')),
 ])
 
 # run the tasks
-tr.run() # to run in parallel add num_processes=N
+tr.run() # to run in parallel add concurrency=N
 ```
 
 more example can be found [here](./examples)
 
 ## Contributer
 setup project git hooks
 ```
```

### Comparing `ataskq-0.5.1/ataskq/ataskq.py` & `ataskq-6.0.0/ataskq/taskq.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,79 +5,69 @@
 from importlib import import_module
 from multiprocessing import Process
 from inspect import signature
 import time
 from typing import Dict, List
 from datetime import datetime
 
-from .env import (
-    ATASKQ_CONNECTION,
-    ATASKQ_MONITOR_PULSE_INTERVAL,
-    ATASKQ_TASK_PULSE_TIMEOUT,
-    ATASKQ_TASK_PULL_INTERVAL,
-    ATASKQ_TASK_WAIT_TIMEOUT,
-)
+
 from .logger import Logger
 from .models import EStatus, Job, StateKWArg, Task, EntryPointRuntimeError
 from .monitor import MonitorThread
-from .handler import Handler, DBHandler, from_connection_str, EAction
+from .handler import Handler, DBHandler, from_config, EAction
+from .config import load_config
 
 
 def targs(*args, **kwargs):
     return (args, kwargs)
 
 
 class TaskQ(Logger):
     def __init__(
         self,
         job_id=None,
-        conn=ATASKQ_CONNECTION,
-        run_task_raise_exception=False,
-        task_wait_timeout=ATASKQ_TASK_WAIT_TIMEOUT,
-        task_pull_intervnal=ATASKQ_TASK_PULL_INTERVAL,
-        monitor_pulse_interval=ATASKQ_MONITOR_PULSE_INTERVAL,
-        task_pulse_timeout=ATASKQ_TASK_PULSE_TIMEOUT,
-        max_jobs: int = None,
-        logger: Union[logging.Logger, None] = None,
+        handler: Handler = None,
+        logger: Union[str, logging.Logger, None] = None,
+        config=None,
     ) -> None:
-        """
-        Args:
-        task_pull_intervnal: pulling interval for task to complete in seconds.
-        task_pulse_timeout: update interval for pulse in seconds while taks is running.
-        monitor_timeout_internal: timeout for task last monitor pulse in seconds, if passed before getting next task, set to Failure.
-        run_task_raise_exception: if True, run_task will raise exception when task fails. This is for debugging purpose only and will fail production flow.
-        """
         super().__init__(logger)
 
+        # init config
+        self._config = load_config(config)
+
         # init db handler
-        # todo: hanlder shouldn't get job_id
-        self._handler: Handler = (
-            conn if isinstance(conn, Handler) else from_connection_str(conn=conn, logger=self._logger)
-        )
+        # todo: handler shouldn't get job_id
+        if handler is None:
+            self._handler: Handler = from_config(
+                config=config,
+                logger=self._logger,
+            )
+        else:
+            self._handler = handler
 
         # get job
         if job_id is not None:
-            job = Job.get(self._job_id, self._handler)
+            try:
+                job = Job.get(job_id, _handler=self._handler)
+            except Exception as ex:
+                raise Exception(f"Failed to fetch job (job_id={job_id}).") from ex
         else:
             job = None
         self._job = job
 
-        self._run_task_raise_exception = run_task_raise_exception
-        self._task_wait_timeout = task_wait_timeout
-        self._task_pull_interval = task_pull_intervnal
-        self._monitor_pulse_interval = monitor_pulse_interval
-        self._task_pulse_timeout = task_pulse_timeout
-        self._max_jobs = max_jobs
-
         # state kwargs for jobs
         self._state_kwargs: Dict[str:object] = dict()
 
         self._running = False
 
     @property
+    def config(self):
+        return self._config
+
+    @property
     def job(self):
         return self._job
 
     @property
     def job_id(self):
         return self._job.job_id
 
@@ -103,18 +93,18 @@
 
     def create_job(self, name=None, description=None):
         assert self._job is None, "job already assigned to current taskq, run clear_job to create new job."
 
         job = Job(name=name, description=description).create(_handler=self._handler)
         self._job = job
 
-        if self._max_jobs is not None:
+        if self.config["db"]["max_jobs"] is not None:
             # keep max jbos
             Job.delete_all(
-                _where=f"job_id NOT IN (SELECT job_id FROM jobs ORDER BY job_id DESC limit {self._max_jobs})",
+                _where=f"job_id NOT IN (SELECT job_id FROM jobs ORDER BY job_id DESC limit {self.config['db']['max_jobs']})",
                 _handler=self.handler,
             )
 
         return self
 
     def delete_job(self):
         self.job.delete(_handler=self.handler)
@@ -159,18 +149,20 @@
         ret = Task.count_all(
             _where=f"job_id = {self.job_id} AND level < {level} AND status in ('{EStatus.PENDING}')",
             _handler=self._handler,
         )
         return ret
 
     def _run_task(self, task: Task):
+        self.info(f"Running task '{task}'")
+
         # get entry point func to execute
         ep = task.entrypoint
         if ep == "ataskq.skip_run_task":
-            self.info(f"task '{task.task_id}' is marked as 'skip_run_task', skipping run task.")
+            self.info(f"task '{task}' is marked as 'skip_run_task', skipping run task.")
             return
 
         assert "." in ep, "entry point must be inside a module."
         module_name, func_name = ep.rsplit(".", 1)
         try:
             m = import_module(module_name)
         except ImportError as ex:
@@ -182,15 +174,15 @@
         assert callable(func), f"entry point is not callable, '{module_name},{func}'."
 
         # get targs
         if task.targs is not None:
             try:
                 targs = pickle.loads(task.targs)
             except Exception as ex:
-                if self._run_task_raise_exception:  # for debug purposes only
+                if self.config["run"]["raise_exception"]:  # for debug purposes only
                     self.warning("Getting tasks args failed.")
                     self.update_task_status(task, EStatus.FAILURE)
                     raise ex
 
                 self.warning("Getting tasks args failed.", exc_info=True)
                 self.update_task_status(task, EStatus.FAILURE)
 
@@ -213,84 +205,88 @@
                 self._logger.info(f"Initializing state kwarg '{name}'")
                 try:
                     self._state_kwargs[name] = state_kwarg.call()
                 except EntryPointRuntimeError as ex:
                     self._logger.info(f"Failed to initialize state kwarg '{name}'")
                     self.update_task_status(task, EStatus.FAILURE)
 
-                    if self._run_task_raise_exception:
+                    if self.config["run"]["raise_exception"]:
                         raise ex
                     return
             # state kwargs already inistliazed
             self._logger.info(f"Update kwarg '{name}' with state kwargs")
             targs[1][name] = self._state_kwargs[name]
 
         # update task start time
         self.update_task_start_time(task)
 
         # run task
-        monitor = MonitorThread(task, self, pulse_interval=self._monitor_pulse_interval)
+        monitor = MonitorThread(task, self, pulse_interval=self.config["monitor"]["pulse_interval"])
         monitor.start()
 
         try:
             func(*targs[0], **targs[1])
             status = EStatus.SUCCESS
         except Exception as ex:
-            if self._run_task_raise_exception:  # for debug purposes only
-                self.warning("Running task entry point failed with exception.")
+            msg = f"Running task '{task}' failed with exception."
+            if self.config["run"]["raise_exception"]:  # for debug purposes only
+                self.warning(msg)
                 self.update_task_status(task, EStatus.FAILURE)
                 monitor.stop()
                 monitor.join()
                 raise ex
 
-            self.warning("Running task entry point failed with exception.", exc_info=True)
+            self.warning(msg, exc_info=True)
             status = EStatus.FAILURE
 
         monitor.stop()
         monitor.join()
         self.update_task_status(task, status)
 
     @staticmethod
     def init_state_kwarg(self, state_kwarg: StateKWArg):
         return
 
-    def _take_next_task(self, level):
-        assert self._job is not None, "job must be assigned to taskq before taking next task."
+    def _take_next_task(self, level=None):
         level_start = level.start if level is not None else None
         level_stop = level.stop if level is not None else None
 
-        return self._handler.take_next_task(self.job_id, level_start, level_stop)
+        job_id = self.job_id if self.job is not None else None
+        return self._handler.take_next_task(job_id=job_id, level_start=level_start, level_stop=level_stop)
 
     def _run(self, level):
+        self.info(f"Started task pulling loop.")
         # make sure all state kwargs for job have key in self._state_kwargs, later to be used in _run_task
         state_kwargs_db = self.job.get_state_kwargs(self._handler)
         for skw in state_kwargs_db:
             if skw.name not in self._state_kwargs:
                 self._state_kwargs[skw.name] = skw
 
         # check for error code
         task_pull_start = time.time()
         while True:
             # if the taskq handler is db handler, the taskq performs background tasks before each run
-            if isinstance(self._handler, DBHandler):
-                self._handler.fail_pulse_timeout_tasks(self._task_pulse_timeout)
+            if self.config["run"]["fail_pulse_timeout"] and isinstance(self._handler, DBHandler):
+                self._handler.fail_pulse_timeout_tasks(self.config["monitor"]["pulse_timeout"])
             # grab tasks and set them in Q
             action, task = self._take_next_task(level)
 
             # handle no task available
             if action == EAction.STOP:
                 break
             if action == EAction.RUN_TASK:
                 self._run_task(task)
             elif action == EAction.WAIT:
-                if self._task_wait_timeout is not None and time.time() - task_pull_start > self._task_wait_timeout:
-                    raise Exception(f"task pull timeout of '{self._task_wait_timeout}' sec reached.")
+                if (
+                    wait_timeout := self.config["run"]["wait_timeout"]
+                ) is not None and time.time() - task_pull_start > wait_timeout:
+                    raise Exception(f"task pull timeout of '{wait_timeout}' sec reached.")
 
-                self.debug(f"waiting for {self._task_pull_interval} sec before taking next task")
-                time.sleep(self._task_pull_interval)
+                self.debug(f'waiting for {self.config["run"]["pull_interval"]} sec before taking next task')
+                time.sleep(self.config["run"]["pull_interval"])
 
     def assert_level(self, level):
         if isinstance(level, int):
             level = range(level, level + 1)
         elif isinstance(level, (list, tuple)):
             assert len(level) == 2, "level of type list or tuple must have length of 2"
             level = range(level[0], level[1])
@@ -299,35 +295,35 @@
 
         # check all task < level.start are done
         count = self.count_pending_tasks_below_level(level.start)
         assert count == 0, f"all tasks below level must be done before running tasks at levels {level}"
 
         return level
 
-    def run(self, num_processes=None, level=None):
+    def run(self, concurrency=None, level=None):
         if level is not None:
             level = self.assert_level(level)
 
         self._running = True
 
         # default to run in current process
-        if num_processes is None:
+        if concurrency is None:
             self._run(level)
             self._running = False
             return
 
-        assert isinstance(num_processes, (int, float))
+        assert isinstance(concurrency, (int, float))
 
-        if isinstance(num_processes, float):
-            assert 0.0 <= num_processes <= 1.0
-            nprocesses = int(multiprocessing.cpu_count() * num_processes)
-        elif num_processes < 0:
-            nprocesses = multiprocessing.cpu_count() - num_processes
+        if isinstance(concurrency, float):
+            assert 0.0 <= concurrency <= 1.0
+            nprocesses = int(multiprocessing.cpu_count() * concurrency)
+        elif concurrency < 0:
+            nprocesses = multiprocessing.cpu_count() - concurrency
         else:
-            nprocesses = num_processes
+            nprocesses = concurrency
 
         # set processes and Q
         processes = [Process(target=self._run, args=(level,)) for i in range(nprocesses)]
         [p.start() for p in processes]
 
         # join all processes
         [p.join() for p in processes]
@@ -337,11 +333,11 @@
         for p in processes:
             if p.exitcode != 0:
                 fail = True
                 self.error(f"Process '{p.pid}' failed with exitcode '{p.exitcode}'")
 
         self._running = False
 
-        if self._run_task_raise_exception and fail:
+        if self.config["run"]["raise_exception"] and fail:
             raise Exception("Some processes failed, see logs for details")
 
         return self
```

### Comparing `ataskq-0.5.1/ataskq/conftest.py` & `ataskq-6.0.0/ataskq/conftest.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 from pytest import fixture
 import os
 import pytest
+import copy
+
+from .config import load_config
+from .env import ATASKQ_CONFIG
 
 if os.getenv("_PYTEST_RAISE", "0") != "0":
 
     @pytest.hookimpl(tryfirst=True)
     def pytest_exception_interact(call):
         raise call.excinfo.value
 
@@ -22,17 +26,17 @@
 END $$;
 """
 
 
 def drop_pg_tables(conn):
     assert "pg" in conn
     import psycopg2
-    from ataskq.handler.postgresql import from_connection_str
+    from ataskq.handler.postgresql import PostgresqlDBHandler
 
-    connection = from_connection_str(conn)
+    connection = PostgresqlDBHandler.from_connection_str(conn)
     db_conn = psycopg2.connect(
         host=connection.host, database=connection.database, user=connection.user, password=connection.password
     )
     c = db_conn.cursor()
     c.execute(truncate_query("tasks"))
     c.execute(truncate_query("state_kwargs"))
     c.execute(truncate_query("jobs"))
@@ -40,22 +44,23 @@
     # c.execute('DROP TABLE IF EXISTS state_kwargs;')
     # c.execute('DROP TABLE IF EXISTS jobs;')
     db_conn.commit()
     db_conn.close()
 
 
 @fixture
-def conn(tmp_path):
-    conn = os.getenv("ATASKQ_CONNECTION", "sqlite://{tmp_path}/ataskq.db.sqlite3")
+def config(tmp_path):
+    config = load_config(ATASKQ_CONFIG or "test")
+    conn = config["connection"]
     if "sqlite" in conn:
-        conn = conn.format(tmp_path=tmp_path)
+        config["connection"] = conn.format(tmp_path=tmp_path)
     elif "pg" in conn:
         # connect and clear all db tables
         drop_pg_tables(conn)
     elif "http" in conn:
-        server_conn = os.getenv("ATASKQ_SERVER_CONNECTION", "pg://postgres:postgres@localhost/postgres")
-        assert "pg" in server_conn, "rest api test must be with posgres server"
+        server_conn = os.getenv("TEST_SERVER_CONNECTION", "pg://postgres:postgres@localhost/postgres")
+        assert "pg" in server_conn, "rest apigi test must be with posgres server"
         drop_pg_tables(server_conn)
     else:
         raise Exception(f"Unkown connection format '{conn}'")
 
-    return conn
+    return copy.deepcopy(config)
```

### Comparing `ataskq-0.5.1/ataskq/handler/db_handler.py` & `ataskq-6.0.0/ataskq/handler/db_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 from datetime import datetime, timedelta
-from typing import List, Tuple
-from pathlib import Path
-from io import TextIOWrapper
+from typing import List
 from abc import abstractmethod
 from datetime import datetime
 
 from .handler import Handler, get_query_kwargs
 from ..imodel import IModel
-from ..env import ATASKQ_DB_INIT_ON_HANDLER_INIT, ATASKQ_DB_LIMIT_DEFAULT
 from .. import __schema_version__
 
 CONNECTION_LOG = [None]
 
 
 def set_connection_log(log):
     CONNECTION_LOG[0] = log
@@ -88,18 +85,17 @@
     if _offset is not None:
         query_str += f" OFFSET {_offset}"
 
     return query_str
 
 
 class DBHandler(Handler):
-    def __init__(self, init_db=ATASKQ_DB_INIT_ON_HANDLER_INIT, logger=None) -> None:
-        super().__init__(logger)
-
-        if init_db:
+    def __init__(self, **kwargs) -> None:
+        super().__init__(**kwargs)
+        if self.config["handler"]["db_init"]:
             self.init_db()
 
     @property
     def db_path(self):
         raise Exception(f"'{self.__class__.__name__}' db doesn't support db path property'")
 
     def count_all(self, model_cls: IModel, **kwargs):
@@ -302,17 +298,17 @@
             #   "summary_cookie JSON, "
             "job_id INTEGER NOT NULL, "
             "CONSTRAINT fk_job_id FOREIGN KEY (job_id) REFERENCES jobs(job_id) ON DELETE CASCADE"
             ")"
         )
 
     @transaction_decorator()
-    def count_query(
-        self, c, model_cls: IModel, _where: str = None, _limit: int = ATASKQ_DB_LIMIT_DEFAULT, _offset: int = 0
-    ):
+    def count_query(self, c, model_cls: IModel, _where: str = None, _limit: int = None, _offset: int = 0):
+        if _limit is None:
+            _limit = self.config["api"]["limit"]
         query_str = f"SELECT COUNT(*) FROM {model_cls.table_key()}"
         query_str = expand_query_str(query_str, _where=_where, _limit=_limit, _offset=_offset)
 
         c.execute(query_str)
 
         row = c.fetchone()
         return row[0]
@@ -320,17 +316,19 @@
     @transaction_decorator()
     def select_query(
         self,
         c,
         model_cls: IModel,
         _where: str = None,
         _order_by=None,
-        _limit: int = ATASKQ_DB_LIMIT_DEFAULT,
+        _limit: int = None,
         _offset: int = 0,
     ):
+        if _limit is None:
+            _limit = self.config["api"]["limit"]
         query_str = f"SELECT * FROM {model_cls.table_key()}"
         if _order_by is None:
             _order_by = f"{model_cls.table_key()}.{model_cls.id_key()} ASC"
         query_str = expand_query_str(query_str, _where=_where, _order_by=_order_by, _limit=_limit, _offset=_offset)
 
         c.execute(query_str)
         rows = c.fetchall()
@@ -339,46 +337,50 @@
         return rows, col_names, query_str
 
     ##################
     # Custom Queries #
     ##################
 
     @transaction_decorator(exclusive=True)
-    def take_next_task(self, c, job_id, level_start, level_stop):
+    def take_next_task(self, c, job_id: int = None, level_start: int = None, level_stop: int = None):
         # imported here to avoid circular dependency
         from ..models import Task, EStatus
-        from .handler import Handler, EAction
+        from .handler import EAction
 
         # todo: add FOR UPDATE in the queries postgresql
         level_query = ""
         if level_start:
             level_query += f" AND level >= {level_start}"
         if level_stop:
             level_query += f" AND level < {level_stop}"
 
         # get pending task with minimum level
+        job_query = ""
+        if job_id is not None:
+            job_query += f" AND job_id = {job_id}"
+
         query = (
-            f"SELECT * FROM tasks WHERE job_id = {job_id} AND status IN ('{EStatus.PENDING}'){level_query} AND level = "
-            f"(SELECT MIN(level) FROM tasks WHERE job_id = {job_id} AND status IN ('{EStatus.PENDING}'){level_query})"
-            f" {self.for_update}"
+            f"SELECT * FROM tasks WHERE status IN ('{EStatus.PENDING}'){job_query}{level_query} AND level = "
+            f"(SELECT MIN(level) FROM tasks WHERE status IN ('{EStatus.PENDING}'){job_query}{level_query})"
+            f" ORDER BY job_id ASC, task_id ASC {self.for_update}"
         )
         query = query.strip()
 
         c.execute(query)
         row = c.fetchone()
         if row is None:
             ptask = None
         else:
             col_names = [description[0] for description in c.description]
             ptask = self.from_interface(Task, dict(zip(col_names, row)))
 
         # get running task with minimum level
         query = (
-            f"SELECT * FROM tasks WHERE job_id = {job_id} AND status IN ('{EStatus.RUNNING}'){level_query} AND level = "
-            f"(SELECT MIN(level) FROM tasks WHERE job_id = {job_id} AND status IN ('{EStatus.RUNNING}'){level_query})"
+            f"SELECT * FROM tasks WHERE status IN ('{EStatus.RUNNING}'){job_query}{level_query} AND level = "
+            f"(SELECT MIN(level) FROM tasks WHERE status IN ('{EStatus.RUNNING}'){job_query}{level_query})"
             f" {self.for_update}"
         )
         query = query.strip()
         c.execute(query)
         row = c.fetchone()
         if row is None:
             rtask = None
@@ -429,21 +431,23 @@
         return action, task
 
     @transaction_decorator()
     def tasks_status(
         self,
         c,
         job_id,
-        _where: str = None,
         _order_by: str = None,
-        _limit: int = ATASKQ_DB_LIMIT_DEFAULT,
+        _limit: int = None,
         _offset: int = 0,
     ):
         from ..models import EStatus
 
+        if _limit is None:
+            _limit = self.config["api"]["limit"]
+
         query_str = (
             "SELECT level, name,"
             "COUNT(*) as total, "
             + ",".join([f"SUM(CASE WHEN status = '{status}' THEN 1 ELSE 0 END) AS {status} " for status in EStatus])
             + f"FROM tasks WHERE job_id = {job_id} "
             "GROUP BY level, name"
         )
@@ -457,19 +461,20 @@
         rows = c.fetchall()
         col_names = [description[0] for description in c.description]
 
         ret = [dict(zip(col_names, row)) for row in rows]
         return ret
 
     @transaction_decorator()
-    def jobs_status(
-        self, c, _where: str = None, _order_by: str = None, _limit: int = ATASKQ_DB_LIMIT_DEFAULT, _offset: int = 0
-    ):
+    def jobs_status(self, c, _order_by: str = None, _limit: int = None, _offset: int = 0):
         from ..models import EStatus
 
+        if _limit is None:
+            _limit = self.config["api"]["limit"]
+
         query_str = (
             "SELECT jobs.job_id, jobs.name, jobs.description, jobs.priority, "
             "COUNT(*) as tasks, "
             + ", ".join([f"SUM(CASE WHEN status = '{status}' THEN 1 ELSE 0 END) AS {status}" for status in EStatus])
             + f" FROM jobs "
             "LEFT JOIN tasks ON jobs.job_id = tasks.job_id "
             "GROUP BY jobs.job_id"
```

### Comparing `ataskq-0.5.1/ataskq/handler/handler.py` & `ataskq-6.0.0/ataskq/handler/handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from abc import abstractmethod
 from typing import Union, List, Dict
 from datetime import datetime
 from enum import Enum
 
+from ..env import ATASKQ_CONFIG
 from ..logger import Logger
+from ..config import load_config
 from ..imodel import IModel, IModelSerializer
 
 __STRTIME_FORMAT__ = "%Y-%m-%d %H:%M:%S.%f"
 
 
 def get_query_kwargs(kwargs):
     _where = ""
@@ -58,17 +60,30 @@
     STOP = "stop"
 
     def __str__(self) -> str:
         return self.value
 
 
 class Handler(IModelSerializer, Logger):
-    def __init__(self, logger: Logger = None):
+    def __init__(self, config=ATASKQ_CONFIG, logger: Logger = None):
         Logger.__init__(self, logger)
 
+        # init config
+        self._config = load_config(config)
+        self._connection = self.from_connection_str(self._config["connection"])
+
+    @property
+    def config(self):
+        return self._config
+
+    @staticmethod
+    @abstractmethod
+    def from_connection_str(conn):
+        pass
+
     ######################
     # interface handlers #
     ######################
 
     @classmethod
     def i2m(cls, model_cls, kwargs: Union[dict, List[dict]]) -> Union[dict, List[dict]]:
         """interface to model"""
@@ -151,23 +166,23 @@
         ikwargs = self.m2i(model_cls, mkwargs)
         self._update(model_cls, model_id, **ikwargs)
 
     ##########
     # Custom #
     ##########
     @abstractmethod
-    def take_next_task(self, job_id, level: Union[int, None]) -> tuple:
+    def take_next_task(self, job_id=None, level_start: int = None, level_stop: int = None) -> tuple:
         pass
 
     @abstractmethod
-    def tasks_status(self, job_id) -> List[dict]:
+    def tasks_status(self, job_id, _order_by: str = None, _limit: int = None, _offset: int = 0) -> List[dict]:
         pass
 
     @abstractmethod
-    def jobs_status(self) -> List[dict]:
+    def jobs_status(self, _order_by: str = None, _limit: int = None, _offset: int = 0) -> List[dict]:
         pass
 
 
 __HANDLERS__: Dict[str, object] = dict()
 
 
 def register_handler(name, handler: Handler):
@@ -188,24 +203,25 @@
             raise RuntimeError("No registered interface handlers")
         return None
     elif len(__HANDLERS__) == 1:
         return list(__HANDLERS__.values())[0]
     else:
         assert (
             name is not None
-        ), f"more than 1 type hander registered, please specify hanlder name. registered handlers: {list(__HANDLERS__.keys())}"
+        ), f"more than 1 type hander registered, please specify handler name. registered handlers: {list(__HANDLERS__.keys())}"
         assert (
             name in __HANDLERS__
         ), f"no handler named '{name}' is registered. registered handlers: {list(__HANDLERS__.keys())}"
         return __HANDLERS__[name]
 
 
-def from_connection_str(conn=None, **kwargs) -> Handler:
-    if conn is None:
-        conn = ""
+def from_config(config=ATASKQ_CONFIG, **kwargs) -> Handler:
+    # expand config in factory and not inside handler
+    config = load_config(config)
+    conn = config["connection"]
 
     sep = "://"
     sep_index = conn.find(sep)
     if sep_index == -1:
         raise RuntimeError("connection must be of format <type>://<connection string>")
     handler_type = conn[:sep_index]
 
@@ -214,23 +230,24 @@
         raise RuntimeError("missing handler type, connection must be of format <type>://<connection string>")
 
     connection_str = conn[sep_index + len(sep) :]
     if not connection_str:
         raise RuntimeError("missing connection string, connection must be of format <type>://<connection string>")
 
     # get db type handler
+    kwargs["config"] = config
     if handler_type == "sqlite":
         from .sqlite3 import SQLite3DBHandler
 
-        handler = SQLite3DBHandler(conn, **kwargs)
+        handler = SQLite3DBHandler(**kwargs)
     elif handler_type == "pg":
         from .postgresql import PostgresqlDBHandler
 
-        handler = PostgresqlDBHandler(conn, **kwargs)
+        handler = PostgresqlDBHandler(**kwargs)
     elif handler_type == "http" or handler_type == "https":
         from .rest_handler import RESTHandler
 
-        handler = RESTHandler(conn, **kwargs)
+        handler = RESTHandler(**kwargs)
     else:
         raise Exception(f"unsupported handler type '{handler_type}', type must be one of ['sqlite', 'pg', 'http']")
 
     return handler
```

### Comparing `ataskq-0.5.1/ataskq/handler/postgresql.py` & `ataskq-6.0.0/ataskq/handler/postgresql.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,61 +1,60 @@
 import re
-from typing import NamedTuple
+from typing import NamedTuple, Union
 from datetime import datetime
 
 try:
     import psycopg2
 except ModuleNotFoundError:
     raise Exception("'psycopg2' is reuiqred for using atasgq postgresql adapter.")
 
 from .db_handler import DBHandler
 from .handler import to_datetime, from_datetime
 
 
 class PostgresConnection(NamedTuple):
-    user: None or str
-    password: None or str
+    user: Union[None, str]
+    password: Union[None, str]
     host: str
     port: int
     database: str
 
     def __str__(self):
         if self.user:
             userspec = f"{self.user}" + (self.password and f":{self.password}") + "@"
 
         return f"pg://{userspec}{self.host}:{self.port}/{self.database}"
 
 
-def from_connection_str(conn):
-    # https://www.postgresql.org/docs/current/libpq-connect.html#LIBPQ-CONNSTRING-URIS
-    # todo: add params spec support
-    format = "pg://[user[:password]@][host][:port][/database]"
-    pattern = r"pg://(?P<user>[^:@]+)(:(?P<password>[^@]+))?@?(?P<host>[^:/]+)(:(?P<port>\d+))?/(?P<database>.+)$"
-
-    match = re.match(pattern, conn)
-
-    if not match:
-        raise Exception(f"db must be in '{format}', ex: 'pg://user:password@localhost:5432/mydb'")
-
-    user = match.group("user")
-    password = match.group("password")
-    host = match.group("host")
-    port = match.group("port")
-    database = match.group("database")
-    ret = PostgresConnection(user=user, password=password, host=host, port=port, database=database)
-
-    return ret
-
-
 class PostgresqlDBHandler(DBHandler):
-    def __init__(self, conn=None, **kwargs) -> None:
-        self._connection = from_connection_str(conn)
+    def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)
 
     @staticmethod
+    def from_connection_str(conn):
+        # https://www.postgresql.org/docs/current/libpq-connect.html#LIBPQ-CONNSTRING-URIS
+        # todo: add params spec support
+        format = "pg://[user[:password]@][host][:port][/database]"
+        pattern = r"pg://(?P<user>[^:@]+)(:(?P<password>[^@]+))?@?(?P<host>[^:/]+)(:(?P<port>\d+))?/(?P<database>.+)$"
+
+        match = re.match(pattern, conn)
+
+        if not match:
+            raise Exception(f"db must be in '{format}', ex: 'pg://user:password@localhost:5432/mydb'")
+
+        user = match.group("user")
+        password = match.group("password")
+        host = match.group("host")
+        port = match.group("port")
+        database = match.group("database")
+        ret = PostgresConnection(user=user, password=password, host=host, port=port, database=database)
+
+        return ret
+
+    @staticmethod
     def m2i_serialize():
         type_handlers = {
             datetime: lambda v: from_datetime(v),
         }
 
         return type_handlers
```

### Comparing `ataskq-0.5.1/ataskq/handler/rest_handler.py` & `ataskq-6.0.0/ataskq/handler/rest_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,25 +16,24 @@
 class RESTConnection(NamedTuple):
     url: Union[None, str]
 
     def __str__(self):
         return {self.url}
 
 
-def from_connection_str(conn):
-    ret = RESTConnection(url=conn)
-
-    return ret
-
-
 class RESTHandler(Handler):
     # todo: remove max jobs
-    def __init__(self, conn=None, logger=None) -> None:
-        self._connection = from_connection_str(conn)
-        super().__init__(logger)
+    def __init__(self, **kwargs) -> None:
+        super().__init__(**kwargs)
+
+    @staticmethod
+    def from_connection_str(conn):
+        ret = RESTConnection(url=conn)
+
+        return ret
 
     @staticmethod
     def m2i_serialize():
         type_handlers = {
             datetime: lambda v: from_datetime(v),
             Enum: lambda v: v.value,
             bytes: lambda v: base64.b64encode(v).decode("ascii"),
@@ -120,28 +119,26 @@
     def update_all(self, model_cls: IModel, **ikwargs):
         self.rest_put(f"{model_cls.table_key()}", json=ikwargs)
 
     ##################
     # Custom Queries #
     ##################
 
-    def take_next_task(self, job_id, level_start, level_stop) -> Tuple:
+    def take_next_task(self, **kwargs) -> Tuple:
         from ..models import Task
 
-        res = self.rest_get(
-            "custom_query/take_next_task", params=dict(job_id=job_id, level_start=level_start, level_stop=level_stop)
-        )
+        res = self.rest_get("custom_query/take_next_task", params=kwargs)
 
         action = EAction(res["action"])
         task = self.from_interface(Task, res["task"]) if res["task"] is not None else None
 
         return (action, task)
 
-    def tasks_status(self, job_id):
-        res = self.rest_get(f"custom_query/tasks_status/{job_id}")
+    def tasks_status(self, job_id, **kwargs):
+        res = self.rest_get(f"custom_query/tasks_status/{job_id}", data=kwargs)
 
         return res
 
-    def jobs_status(self):
-        res = self.rest_get(f"custom_query/jobs_status")
+    def jobs_status(self, **kwargs):
+        res = self.rest_get(f"custom_query/jobs_status", data=kwargs)
 
         return res
```

### Comparing `ataskq-0.5.1/ataskq/handler/sqlite3.py` & `ataskq-6.0.0/ataskq/handler/sqlite3.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,32 +11,31 @@
 class SqliteConnection(NamedTuple):
     path: str
 
     def __str__(self):
         return f"sqlite://{self.path}"
 
 
-def from_connection_str(conn):
-    format = "sqlite://path"
-    pattern = r"sqlite://(?P<path>.+)$"
-    match = re.match(pattern, conn)
-
-    if not match:
-        raise Exception(f"conn must be in '{format}', ex: 'sqlite://ataskq.db.sqlite3'")
+class SQLite3DBHandler(DBHandler):
+    def __init__(self, **kwargs) -> None:
+        super().__init__(**kwargs)
 
-    path = match.group("path")
-    ret = SqliteConnection(path=path)
+    @staticmethod
+    def from_connection_str(conn):
+        format = "sqlite://path"
+        pattern = r"sqlite://(?P<path>.+)$"
+        match = re.match(pattern, conn)
 
-    return ret
+        if not match:
+            raise Exception(f"conn must be in '{format}', ex: 'sqlite://ataskq.db.sqlite3'")
 
+        path = match.group("path")
+        ret = SqliteConnection(path=path)
 
-class SQLite3DBHandler(DBHandler):
-    def __init__(self, conn=None, **kwargs) -> None:
-        self._connection = from_connection_str(conn)
-        super().__init__(**kwargs)
+        return ret
 
     @staticmethod
     def m2i_serialize():
         type_handlers = {
             datetime: lambda v: from_datetime(v),
         }
```

### Comparing `ataskq-0.5.1/ataskq/imodel.py` & `ataskq-6.0.0/ataskq/imodel.py`

 * *Files identical despite different names*

### Comparing `ataskq-0.5.1/ataskq/models.py` & `ataskq-6.0.0/ataskq/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -441,14 +441,17 @@
     def table_key():
         return "tasks"
 
     def __init__(self, **kwargs) -> None:
         EntryPoint.init(kwargs)
         Model.__init__(self, **kwargs)
 
+    def __str__(self):
+        return f"{self.name}({self.task_id})" if self.name else f"{self.task_id}"
+
 
 class StateKWArg(Model, EntryPoint):
     state_kwargs_id: int
     name: str
     entrypoint: str
     targs: bytes
     description: str
```

### Comparing `ataskq-0.5.1/ataskq/monitor.py` & `ataskq-6.0.0/ataskq/monitor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-import socket
 from threading import Thread, Event
-import time
 
 from .models import Task, EStatus
 
 
 class MonitorThread(Thread):
     # task runner is .task_runner TaskRunner, avoiding circular import
     def __init__(self, task: Task, ataskq, pulse_interval: float = 60) -> None:
+        from .taskq import TaskQ  # here to avoid circular dependency
+
         super().__init__(daemon=True)
         self._stop_event = Event()
         self._task = task
-        self._ataskq = ataskq
+        self._ataskq: TaskQ = ataskq
         self._pulse_interval = pulse_interval
 
     def run(self) -> None:
-        self._ataskq.info(f"Running monitor thread for task id '{self._task.task_id}'")
+        self._ataskq.info(f"Running monitor thread for task '{self._task}'")
         while not self._stop_event.is_set():
             self._ataskq.update_task_status(self._task, EStatus.RUNNING)
             self._stop_event.wait(self._pulse_interval)
 
     def stop(self):
         self._stop_event.set()
```

### Comparing `ataskq-0.5.1/ataskq/server/form_utils.py` & `ataskq-6.0.0/ataskq/server/form_utils.py`

 * *Files identical despite different names*

### Comparing `ataskq-0.5.1/ataskq/server/server.py` & `ataskq-6.0.0/ataskq/server/server.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,68 +2,33 @@
 import asyncio
 from pathlib import Path
 
 from fastapi import FastAPI, Request, Depends
 from fastapi.responses import FileResponse, RedirectResponse
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.staticfiles import StaticFiles
-from contextlib import asynccontextmanager
 
 
-from ataskq.handler import from_connection_str
-from ataskq.handler import DBHandler
+from ataskq.handler import DBHandler, from_config
 from ataskq.handler.rest_handler import RESTHandler as rh
 from ataskq.models import Model, __MODELS__
-from ataskq.env import (
-    ATASKQ_SERVER_CONNECTION,
-    ATASKQ_SERVER_TASK_PULSE_TIMEOUT_MONITOR_INTERVAL,
-    ATASKQ_TASK_PULSE_TIMEOUT,
-)
+from ataskq.env import ATASKQ_SERVER_CONFIG
 
 # from .form_utils import form_data_array
 
 logger = logging.getLogger("uvicorn")
-logger.info(f"ATASKQ_SERVER_CONNECTION: {ATASKQ_SERVER_CONNECTION}")
-logger.info(f"ATASKQ_TASK_PULSE_TIMEOUT: {ATASKQ_TASK_PULSE_TIMEOUT}")
-logger.info(f"ATASKQ_SERVER_TASK_PULSE_TIMEOUT_MONITOR_INTERVAL: {ATASKQ_SERVER_TASK_PULSE_TIMEOUT_MONITOR_INTERVAL}")
 
 
 # DB Handler
-
-
 def db_handler() -> DBHandler:
-    return from_connection_str(ATASKQ_SERVER_CONNECTION)
-
-
-async def set_timout_tasks_task():
-    dbh = db_handler()
-    while True:
-        logger.debug("Set Timeout Tasks")
-        dbh.fail_pulse_timeout_tasks(ATASKQ_TASK_PULSE_TIMEOUT)
-        await asyncio.sleep(ATASKQ_SERVER_TASK_PULSE_TIMEOUT_MONITOR_INTERVAL)
-
-
-@asynccontextmanager
-async def lifespan(app: FastAPI):
-    logger.info("enter lifspan")
-
-    logger.info("init db")
-    db_handler().init_db()
-
-    task = asyncio.create_task(set_timout_tasks_task())
+    return from_config(ATASKQ_SERVER_CONFIG or "server")
 
-    # Load the ML model
-    yield
-    # Clean up the ML models and release the resources
-    logger.info("cancel task")
-    task.cancel()
-    logger.info("exit lifspan")
 
+app = FastAPI()
 
-app = FastAPI(lifespan=lifespan)
 
 # allow all cors
 app.add_middleware(
     CORSMiddleware,
     allow_origins=["*"],
     allow_credentials=True,
     allow_methods=["*"],
@@ -103,21 +68,19 @@
 
 
 ####################
 # Custom Query API #
 ####################
 @app.get("/api/custom_query/take_next_task")
 async def take_next_task(
-    job_id: int,
-    level_start: int = None,
-    level_stop: int = None,
+    request: Request,
     dbh: DBHandler = Depends(db_handler),
 ):
     # take next task
-    action, task = dbh.take_next_task(job_id, level_start, level_stop)
+    action, task = dbh.take_next_task(**request.query_params)
     task = rh.to_interface(task) if task is not None else None
 
     return dict(action=action, task=task)
 
 
 @app.get("/api/custom_query/jobs_status")
 async def jobs_status(request: Request, dbh: DBHandler = Depends(db_handler)):
```

### Comparing `ataskq-0.5.1/ataskq/server/www/assets/index-MiCEdQXI.js` & `ataskq-6.0.0/ataskq/server/www/assets/index-MiCEdQXI.js`

 * *Files identical despite different names*

### Comparing `ataskq-0.5.1/ataskq/server/www/assets/index-MiCEdQXI.js.map` & `ataskq-6.0.0/ataskq/server/www/assets/index-MiCEdQXI.js.map`

 * *Files identical despite different names*

### Comparing `ataskq-0.5.1/ataskq/server/www/assets/index-_NWmBfbC.css` & `ataskq-6.0.0/ataskq/server/www/assets/index-_NWmBfbC.css`

 * *Files identical despite different names*

### Comparing `ataskq-0.5.1/ataskq/server/www/ataskq-32.png` & `ataskq-6.0.0/ataskq/server/www/ataskq-32.png`

 * *Files identical despite different names*

### Comparing `ataskq-0.5.1/ataskq/server/www/favicon.ico` & `ataskq-6.0.0/ataskq/server/www/favicon.ico`

 * *Files identical despite different names*

### Comparing `ataskq-0.5.1/ataskq/server/www/index.html` & `ataskq-6.0.0/ataskq/server/www/index.html`

 * *Files identical despite different names*

### Comparing `ataskq-0.5.1/ataskq/tasks_utils/counter_task.py` & `ataskq-6.0.0/ataskq/tasks_utils/counter_task.py`

 * *Files identical despite different names*

### Comparing `ataskq-0.5.1/ataskq/test_ataskq.py` & `ataskq-6.0.0/ataskq/test_ataskq.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,68 @@
 from pathlib import Path
 from datetime import datetime, timedelta
 from copy import copy
 
 import pytest
 
-from ataskq import TaskQ, StateKWArg, Job, Task, targs, EStatus
-from ataskq.handler import DBHandler
-from ataskq.handler import EAction, from_connection_str
+from . import TaskQ, StateKWArg, Job, Task, targs, EStatus
+from .handler import DBHandler
+from .handler import EAction, from_config
 
 from .tasks_utils import dummy_args_task
 
 
+def non_decreasing(L):
+    return all(x <= y for x, y in zip(L, L[1:]))
+
+
+def non_increasing(L):
+    return all(x >= y for x, y in zip(L, L[1:]))
+
+
+def monotonic(L):
+    return non_decreasing(L) or non_increasing(L)
+
+
 @pytest.fixture
-def jtaskq(conn) -> TaskQ:
-    return TaskQ(conn=conn).create_job()
+def jtaskq(config) -> TaskQ:
+    return TaskQ(config=config).create_job()
 
 
-def test_create_job(conn):
-    taskq = TaskQ(conn=conn).create_job()
+def test_create_job(config):
+    taskq = TaskQ(config=config).create_job()
     assert isinstance(taskq, TaskQ)
 
+    conn = config["connection"]
     if "sqlite" in conn:
         assert Path(taskq.handler.db_path).exists()
         assert Path(taskq.handler.db_path).is_file()
     elif "pg" in conn:
         pass
     elif "http" in conn:
         pass
     else:
         raise Exception(f"unknown db type in connection string '{conn}'")
 
 
-def test_job_default_name(conn):
-    job = TaskQ(conn=conn).create_job().job
+def test_job_default_name(config):
+    job = TaskQ(config=config).create_job().job
     assert job.name is None
 
 
-def test_job_custom_name(conn):
-    job = TaskQ(conn=conn).create_job(name="my_job").job
+def test_job_custom_name(config):
+    job = TaskQ(config=config).create_job(name="my_job").job
     assert job.name == "my_job"
 
 
-def test_task_job_delete_cascade(conn):
+def test_task_job_delete_cascade(config):
     # test that deleting a job deletes all its tasks
-    handler = from_connection_str(conn=conn)
-    taskq1: TaskQ = TaskQ(conn=handler).create_job(name="job1")
-    taskq2: TaskQ = TaskQ(conn=handler).create_job(name="job2")
+    handler = from_config(config)
+    taskq1: TaskQ = TaskQ(handler=handler).create_job(name="job1")
+    taskq2: TaskQ = TaskQ(handler=handler).create_job(name="job2")
     assert Job.count_all(_handler=handler) == 2
 
     taskq1.add_tasks(
         [
             Task(entrypoint=""),
             Task(entrypoint=""),
             Task(entrypoint=""),
@@ -74,19 +87,19 @@
     assert Task.count_all(_handler=handler) == 3
     assert len(taskq1.get_tasks()) == 3
 
     taskq1.delete_job()
     assert Task.count_all(_handler=handler) == 0
 
 
-def test_state_kwargs_job_delete_cascade(conn):
+def test_state_kwargs_job_delete_cascade(config):
     # todo: test should ne under ataskq
-    handler = from_connection_str(conn=conn)
-    taskq1: TaskQ = TaskQ(conn=handler).create_job(name="job1")
-    taskq2: TaskQ = TaskQ(conn=handler).create_job(name="job2")
+    handler = from_config(config)
+    taskq1: TaskQ = TaskQ(handler=handler).create_job(name="job1")
+    taskq2: TaskQ = TaskQ(handler=handler).create_job(name="job2")
     assert len(Job.get_all(_handler=handler)) == 2
 
     taskq1.add_state_kwargs(
         [
             StateKWArg(entrypoint=""),
             StateKWArg(entrypoint=""),
             StateKWArg(entrypoint=""),
@@ -112,15 +125,15 @@
     assert len(taskq1.get_state_kwargs()) == 3
 
     taskq1.delete_job()
     assert len(StateKWArg.get_all(_handler=handler)) == 0
 
 
 def test_update_task_start_time(jtaskq):
-    in_task1 = Task(entrypoint="ataskq.tasks_utils.dummy_args_task", level=1, name="task1")
+    in_task1 = Task(entrypoint=dummy_args_task, level=1, name="task1")
 
     jtaskq.add_tasks(
         [
             in_task1,
         ]
     )
 
@@ -138,15 +151,15 @@
     tasks = jtaskq.get_tasks()
     assert len(tasks) == 1  # sanity
     task: Task = tasks[0]
     assert task.start_time == start_time
 
 
 def test_update_task_status(jtaskq):
-    in_task1 = Task(entrypoint="ataskq.tasks_utils.dummy_args_task", level=1, name="task1")
+    in_task1 = Task(entrypoint=dummy_args_task, level=1, name="task1")
 
     jtaskq.add_tasks(
         [
             in_task1,
         ]
     )
 
@@ -179,42 +192,66 @@
     assert len(tasks) == 1  # sanity
     task: Task = tasks[0]
     assert task.status == EStatus.SUCCESS
     assert task.pulse_time == now
     assert task.done_time == now
 
 
-def _compare_task_taken(task1: Task, task2: Task, job_id=None):
+def _compare_tasks(task1: Task, task2: Task, job_id=None):
     if job_id:
         assert task1.job_id == job_id
     assert task1.job_id == task2.job_id
     assert task1.name == task2.name
     assert task1.description == task2.description
     assert task1.level == task2.level
     assert task1.entrypoint == task2.entrypoint
     assert task1.targs == task2.targs
 
 
+def test_get_tasks(jtaskq):
+    in_task1 = Task(entrypoint=dummy_args_task, level=1, name="task1")
+    in_task2 = Task(entrypoint=dummy_args_task, level=2, name="task2")
+    in_task3 = Task(entrypoint=dummy_args_task, level=3, name="task3")
+
+    jtaskq.add_tasks(
+        [
+            in_task3,
+            in_task2,
+            in_task1,
+        ]
+    )
+
+    tasks = jtaskq.get_tasks()
+    assert len(tasks) == 3
+    for t in tasks:
+        if t.level == 1:
+            _compare_tasks(in_task1, t)
+        elif t.level == 2:
+            _compare_tasks(in_task2, t)
+        elif t.level == 3:
+            _compare_tasks(in_task3, t)
+
+
 def test_take_next_task_sanity(jtaskq):
-    in_task1 = Task(entrypoint="ataskq.tasks_utils.dummy_args_task", level=1, name="task1")
+    in_task1 = Task(entrypoint=dummy_args_task, level=1, name="task1")
 
     jtaskq.add_tasks(
         [
             in_task1,
         ]
     )
 
     action, task = jtaskq._take_next_task(level=None)
     assert action == EAction.RUN_TASK
-    _compare_task_taken(in_task1, task)
+    _compare_tasks(in_task1, task)
 
 
 def test_take_next_task(jtaskq):
-    in_task1 = Task(entrypoint="ataskq.tasks_utils.dummy_args_task", level=1, name="task1")
-    in_task2 = Task(entrypoint="ataskq.tasks_utils.dummy_args_task", level=2, name="task2")
+    in_task1 = Task(entrypoint=dummy_args_task, level=1, name="task1")
+    in_task2 = Task(entrypoint=dummy_args_task, level=2, name="task2")
     in_task3 = copy(in_task1)
 
     jtaskq.add_tasks(
         [
             in_task2,
             in_task1,
             in_task3,
@@ -223,38 +260,38 @@
 
     tids = []
 
     action, task = jtaskq._take_next_task(level=None)
     assert action == EAction.RUN_TASK
     assert task.task_id not in tids
     tids.append(task.task_id)
-    _compare_task_taken(in_task1, task)
+    _compare_tasks(in_task1, task)
 
     action, task = jtaskq._take_next_task(level=None)
     assert action == EAction.RUN_TASK
     assert task.task_id not in tids
     tids.append(task.task_id)
-    _compare_task_taken(in_task3, task)  # note in_task3 is copy of in_task1
+    _compare_tasks(in_task3, task)  # note in_task3 is copy of in_task1
 
     action, task = jtaskq._take_next_task(level=None)
     assert action == EAction.WAIT
     assert task is None
 
 
-def test_take_next_task_2_jobs(conn):
+def test_take_next_task_2_jobs(config):
     # todo: test should ne under ataskq
-    handler = from_connection_str(conn=conn)
-    taskq1: TaskQ = TaskQ(conn=handler).create_job(name="job1")
-    taskq2: TaskQ = TaskQ(conn=handler).create_job(name="job2")
-
-    in_task1 = Task(entrypoint="ataskq.tasks_utils.dummy_args_task", level=2, name="taska")
-    in_task2 = Task(entrypoint="ataskq.tasks_utils.dummy_args_task", level=1, name="taskb")
-    in_task3 = Task(entrypoint="ataskq.tasks_utils.dummy_args_task", level=1, name="taskb")
-    in_task4 = Task(entrypoint="ataskq.tasks_utils.dummy_args_task", level=1, name="taskd")
-    in_task5 = Task(entrypoint="ataskq.tasks_utils.dummy_args_task", level=2, name="taske")
+    handler = from_config(config)
+    taskq1: TaskQ = TaskQ(handler=handler).create_job(name="job1")
+    taskq2: TaskQ = TaskQ(handler=handler).create_job(name="job2")
+
+    in_task1 = Task(entrypoint=dummy_args_task, level=2, name="taska")
+    in_task2 = Task(entrypoint=dummy_args_task, level=1, name="taskb")
+    in_task3 = Task(entrypoint=dummy_args_task, level=1, name="taskb")
+    in_task4 = Task(entrypoint=dummy_args_task, level=1, name="taskd")
+    in_task5 = Task(entrypoint=dummy_args_task, level=2, name="taske")
 
     taskq1.add_tasks(
         [
             in_task2,
             in_task1,
             in_task3,
         ]
@@ -273,73 +310,103 @@
 
     # sanity check
     assert len(Job.get_all(_handler=handler)) == 2
     assert len(taskq1.get_tasks()) == 3
     assert len(Job.get_all(_handler=handler)) == 2
     assert len(taskq2.get_tasks()) == 2
 
-    # db handler 1
+    # taskq 1
     action, task = taskq1._take_next_task(level=None)
     assert action == EAction.RUN_TASK
     assert task.task_id not in tids
     tids.append(task.task_id)
-    _compare_task_taken(in_task2, task, job_id=jid1)
+    _compare_tasks(in_task2, task, job_id=jid1)
     tids.append(task.task_id)
 
     action, task = taskq1._take_next_task(level=None)
     assert action == EAction.RUN_TASK
     assert task.task_id not in tids
     tids.append(task.task_id)
-    _compare_task_taken(in_task3, task, job_id=jid1)  # note in_task3 is copy of in_task1
+    _compare_tasks(in_task3, task, job_id=jid1)  # note in_task3 is copy of in_task1
 
     action, task = taskq1._take_next_task(level=None)
     assert action == EAction.WAIT
     assert task is None
 
-    # db handler 2
+    # taskq 2
     action, task = taskq2._take_next_task(level=None)
     assert action == EAction.RUN_TASK
     assert task.task_id not in tids
     tids.append(task.task_id)
-    _compare_task_taken(in_task4, task, job_id=jid2)
+    _compare_tasks(in_task4, task, job_id=jid2)
     tids.append(task.task_id)
 
     action, task = taskq2._take_next_task(level=None)
     assert action == EAction.WAIT
     assert task is None
 
 
-def test_get_tasks(jtaskq):
-    in_task1 = Task(entrypoint=dummy_args_task, level=1, name="task1")
-    in_task2 = Task(entrypoint=dummy_args_task, level=2, name="task2")
-    in_task3 = Task(entrypoint=dummy_args_task, level=3, name="task3")
+def test_take_next_all_jobs(tmp_path, config):
+    handler = from_config(config)
+    taskq1: TaskQ = TaskQ(handler=handler).create_job(name="job1")
+    taskq2: TaskQ = TaskQ(handler=handler).create_job(name="job2")
 
-    jtaskq.add_tasks(
+    def init_task(name):
+        return Task(entrypoint=dummy_args_task, name=name)
+
+    in_task1 = init_task("job1 - task1")
+    in_task2 = init_task("job1 - task2")
+    taskq1.add_tasks(
         [
-            in_task3,
-            in_task2,
             in_task1,
+            in_task2,
         ]
     )
 
-    tasks = jtaskq.get_tasks()
-    assert len(tasks) == 3
-    for t in tasks:
-        if t.level == 1:
-            _compare_task_taken(in_task1, t)
-        elif t.level == 2:
-            _compare_task_taken(in_task2, t)
-        elif t.level == 3:
-            _compare_task_taken(in_task3, t)
+    in_task4 = init_task("job2 - task4")
+    in_task5 = init_task("job2 - task5")
+    taskq2.add_tasks(
+        [
+            in_task4,
+            in_task5,
+        ]
+    )
+
+    in_task3 = init_task("job1 - task3")
+    taskq1.add_tasks(
+        [
+            in_task3,
+        ]
+    )
+
+    jid1 = taskq1.job_id
+    jid2 = taskq2.job_id
+
+    # sanity check
+    assert len(Job.get_all(_handler=handler)) == 2
+    assert len(taskq1.get_tasks()) == 3
+    assert len(Job.get_all(_handler=handler)) == 2
+    assert len(taskq2.get_tasks()) == 2
+
+    taskq = TaskQ(config=config)
+    in_tasks = [in_task1, in_task2, in_task3, in_task4, in_task5]
+    in_jids = [jid1, jid1, jid1, jid2, jid2]
+    for t, jid in zip(in_tasks, in_jids):
+        action, task = taskq._take_next_task()
+        assert action == EAction.RUN_TASK
+        assert task.task_id == t.task_id
+        _compare_tasks(t, task, job_id=jid)
+
+    assert not monotonic([t.task_id for t in in_tasks])
 
 
-def test_run_default(conn, tmp_path: Path):
+def test_run_default(config, tmp_path: Path):
     filepath = tmp_path / "file.txt"
 
-    taskq = TaskQ(conn=conn).create_job()
+    taskq = TaskQ(config=config).create_job()
 
     taskq.add_tasks(
         [
             Task(entrypoint="ataskq.tasks_utils.write_to_file_tasks.write_to_file", targs=targs(filepath, "task 0\n")),
             Task(entrypoint="ataskq.tasks_utils.write_to_file_tasks.write_to_file", targs=targs(filepath, "task 1\n")),
             Task(entrypoint="ataskq.tasks_utils.write_to_file_tasks.write_to_file", targs=targs(filepath, "task 2\n")),
         ]
@@ -347,43 +414,45 @@
 
     taskq.run()
 
     assert filepath.exists()
     assert filepath.read_text() == "task 0\n" "task 1\n" "task 2\n"
 
 
-def test_run_task_raise_exception(conn):
+def test_run_task_raise_exception(config):
     # no exception raised
     try:
-        taskq: TaskQ = TaskQ(conn=conn, run_task_raise_exception=False).create_job()
+        config["run"]["raise_exception"] = False
+        taskq: TaskQ = TaskQ(config=config).create_job()
         taskq.add_tasks(
             [
                 Task(entrypoint="ataskq.tasks_utils.exception_task", targs=targs(message="task failed")),
             ]
         )
         taskq.run()
     except Exception:
         assert False, "exception_task raises exception with run_task_raise_exception=False"
 
     # exception raised
-    taskq: TaskQ = TaskQ(conn=conn, run_task_raise_exception=True).create_job()
+    config["run"]["raise_exception"] = True
+    taskq: TaskQ = TaskQ(config=config).create_job()
     taskq.add_tasks(
         [
             Task(entrypoint="ataskq.tasks_utils.exception_task", targs=targs(message="task failed")),
         ]
     )
     with pytest.raises(Exception) as excinfo:
         taskq.run()
     assert excinfo.value.args[0] == "task failed"
 
 
-def test_run_2_processes(conn, tmp_path: Path):
+def test_run_2_processes(config, tmp_path: Path):
     filepath = tmp_path / "file.txt"
 
-    taskq = TaskQ(conn=conn).create_job()
+    taskq = TaskQ(config=config).create_job()
 
     taskq.add_tasks(
         [
             Task(
                 entrypoint="ataskq.tasks_utils.write_to_file_tasks.write_to_file_mp_lock",
                 targs=targs(filepath, "task 0\n"),
             ),
@@ -394,28 +463,28 @@
             Task(
                 entrypoint="ataskq.tasks_utils.write_to_file_tasks.write_to_file_mp_lock",
                 targs=targs(filepath, "task 2\n"),
             ),
         ]
     )
 
-    taskq.run(num_processes=2)
+    taskq.run(concurrency=2)
 
     assert filepath.exists()
     text = filepath.read_text()
     assert "task 0\n" in text
     assert "task 1\n" in text
     assert "task 1\n" in text
 
 
 @pytest.mark.parametrize("num_processes", [None, 2])
-def test_run_by_level(conn, tmp_path: Path, num_processes: int):
+def test_run_by_level(config, tmp_path: Path, num_processes: int):
     filepath = tmp_path / "file.txt"
 
-    taskq = TaskQ(conn=conn).create_job()
+    taskq = TaskQ(config=config).create_job()
 
     taskq.add_tasks(
         [
             Task(
                 level=0,
                 entrypoint="ataskq.tasks_utils.write_to_file_tasks.write_to_file_mp_lock",
                 targs=targs(filepath, "task 0\n"),
@@ -437,78 +506,82 @@
             ),
         ]
     )
 
     assert taskq.count_pending_tasks_below_level(3) == 4
 
     assert taskq.count_pending_tasks_below_level(1) == 1
-    taskq.run(level=0, num_processes=num_processes)
+    taskq.run(level=0, concurrency=num_processes)
     taskq.count_pending_tasks_below_level(1) == 0
     assert filepath.exists()
     text = filepath.read_text()
     assert "task 0\n" in text
 
     assert taskq.count_pending_tasks_below_level(2) == 2
-    taskq.run(level=1, num_processes=num_processes)
+    taskq.run(level=1, concurrency=num_processes)
     taskq.count_pending_tasks_below_level(2) == 0
     text = filepath.read_text()
     assert "task 0\n" in text
     assert "task 1\n" in text
     assert "task 2\n" in text
 
     assert taskq.count_pending_tasks_below_level(3) == 1
-    taskq.run(level=2, num_processes=num_processes)
+    taskq.run(level=2, concurrency=num_processes)
     taskq.count_pending_tasks_below_level(3) == 0
     text = filepath.read_text()
     assert "task 0\n" in text
     assert "task 1\n" in text
     assert "task 2\n" in text
     assert "task 3\n" in text
 
 
-def test_monitor_pulse_failure(conn):
+def test_monitor_pulse_failure(config):
     # set monitor pulse longer than timeout
-    taskq = TaskQ(conn=conn, monitor_pulse_interval=10, task_pulse_timeout=1.5).create_job()
+    config["monitor"]["pulse_interval"] = 2
+    config["monitor"]["pulse_timeout"] = 1.5
+    taskq = TaskQ(config=config).create_job()
     taskq.add_tasks(
         [
             # reserved keyward for ignored task for testing
             Task(entrypoint="ataskq.skip_run_task", targs=targs("task will fail")),
-            Task(entrypoint="ataskq.tasks_utils.dummy_args_task", targs=targs("task will success")),
+            Task(entrypoint=dummy_args_task, targs=targs("task will success")),
         ]
     )
     start = datetime.now()
     taskq.run()
     stop = datetime.now()
 
     tasks = taskq.get_tasks()
 
     assert tasks[0].status == EStatus.FAILURE
     assert tasks[1].status == EStatus.SUCCESS
     assert stop - start > timedelta(seconds=1.5)
 
 
-def test_task_wait_timeout(conn):
+def test_task_wait_timeout(config):
     # set monitor pulse longer than timeout
-    taskq = TaskQ(conn=conn, run_task_raise_exception=True, task_wait_timeout=0).create_job()
+    config["run"]["raise_exception"] = True
+    config["run"]["wait_timeout"] = 0
+    taskq = TaskQ(config=config).create_job()
     taskq.add_tasks(
         [
-            Task(entrypoint="ataskq.tasks_utils.dummy_args_task", level=1, targs=targs("task will success", sleep=0.2)),
-            Task(entrypoint="ataskq.tasks_utils.dummy_args_task", level=2, targs=targs("task will success")),
+            Task(entrypoint=dummy_args_task, level=1, targs=targs("task will success", sleep=0.2)),
+            Task(entrypoint=dummy_args_task, level=2, targs=targs("task will success")),
         ]
     )
 
     with pytest.raises(Exception) as excinfo:
-        taskq.run(num_processes=2)
+        taskq.run(concurrency=2)
     assert excinfo.value.args[0] == "Some processes failed, see logs for details"
 
 
-def test_run_with_state_kwargs(conn):
+def test_run_with_state_kwargs(config):
     from ataskq.tasks_utils.counter_task import counter_kwarg, counter_task
 
-    taskq = TaskQ(conn=conn, run_task_raise_exception=True).create_job()
+    taskq = TaskQ(config=config).create_job()
 
     taskq.add_state_kwargs(
         [
             StateKWArg(entrypoint=counter_kwarg, name="counter"),
         ]
     )
 
@@ -517,17 +590,18 @@
             Task(entrypoint=counter_task, targs=targs(print_counter=True)),
         ]
     )
 
     taskq.run()
 
 
-def test_max_jobs(conn):
+def test_max_jobs(config):
     max_jobs = 10
-    taskq = TaskQ(conn=conn, max_jobs=max_jobs)
+    config["db"]["max_jobs"] = max_jobs
+    taskq = TaskQ(config=config)
     if not isinstance(taskq.handler, DBHandler):
         pytest.skip()
 
     jobs_id = []
     for i in range(max_jobs * 2):
         taskq.clear_job()
         taskq.create_job(name=f"job{i}")
```

### Comparing `ataskq-0.5.1/ataskq/test_handler.py` & `ataskq-6.0.0/ataskq/test_handler.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 # todo: add queries order_by tests
 
-from pathlib import Path
-from copy import copy
-from datetime import datetime
-
 import pytest
 
-from .handler import Handler, from_connection_str
+from .config import load_config
+from .handler import Handler, from_config
 from .handler.db_handler import DBHandler, transaction_decorator
 from .handler import register_handler
 
 
 @pytest.fixture
-def handler(conn) -> Handler:
-    handler = from_connection_str(conn)
+def handler(config) -> Handler:
+    handler = from_config(config)
     register_handler("test_handler", handler)
     return handler
 
 
 class ForTestDBHandler:
     def __init__(self, handler):
         self._handler = handler
@@ -40,16 +37,17 @@
 
     handler = ForTestDBHandler(handler)
     with pytest.raises(Exception) as excinfo:
         handler.invalid()
     assert "syntax error" in str(excinfo.value)
 
 
-def test_db_format(conn, handler):
+def test_db_format(config, handler):
     assert isinstance(handler, Handler)
+    conn = config["connection"]
 
     if "sqlite" in conn:
         from .handler.sqlite3 import SQLite3DBHandler
 
         assert isinstance(handler, SQLite3DBHandler)
         assert "ataskq.db" in handler.db_path
     elif "pg" in conn:
@@ -62,21 +60,21 @@
         assert isinstance(handler, RESTHandler)
     else:
         raise Exception(f"unknown handler type in connection string '{conn}'")
 
 
 def test_db_invalid_format_no_sep():
     with pytest.raises(RuntimeError) as excinfo:
-        from_connection_str(conn=f"sqlite")
+        from_config(config=load_config({"connection": "sqlite"}, environ=False))
     assert "connection must be of format <type>://<connection string>" == str(excinfo.value)
 
 
 def test_db_invalid_format_no_type():
     with pytest.raises(RuntimeError) as excinfo:
-        from_connection_str(conn=f"://ataskq.db")
+        from_config(load_config({"connection": f"://ataskq.db"}, environ=False))
     assert "missing handler type, connection must be of format <type>://<connection string>" == str(excinfo.value)
 
 
 def test_db_invalid_format_no_connectino():
     with pytest.raises(RuntimeError) as excinfo:
-        from_connection_str(conn=f"sqlite://")
+        from_config(load_config({"connection": "sqlite://"}, environ=False))
     assert "missing connection string, connection must be of format <type>://<connection string>" == str(excinfo.value)
```

### Comparing `ataskq-0.5.1/ataskq/test_models.py` & `ataskq-6.0.0/ataskq/test_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pytest
 
 from .models import Model, __MODELS__, Job
-from .handler import Handler, from_connection_str, register_handler, unregister_handler
+from .handler import Handler, from_config, register_handler, unregister_handler
 
 
 @pytest.fixture(scope="function")
-def handler(conn):
-    handler = from_connection_str(conn)
+def handler(config):
+    handler = from_config(config)
     register_handler("test_handler", handler)
     yield handler
     unregister_handler("test_handler")
 
 
 @pytest.fixture
 def jhandler(handler) -> Handler:
@@ -121,15 +121,15 @@
 MODEL_CHILD = [
     (model_cls, child_cls, parent_key)
     for model_cls in __MODELS__.values()
     for child_cls, parent_key in model_cls.children().items()
 ]
 
 
-@pytest.mark.parametrize("model_cls, child_cls, parent_key", [MODEL_CHILD[0]])
+@pytest.mark.parametrize("model_cls, child_cls, parent_key", MODEL_CHILD)
 def test_add_get_children(handler, model_cls: Model, child_cls, parent_key):
     m1 = create(model_cls)
     children = [init(child_cls, **{parent_key: None}) for i in range(3)]
     m1.add_children(child_cls, children)
 
     m2 = create(model_cls)
     children = [init(child_cls, **{parent_key: None}) for i in range(4)]
```

### Comparing `ataskq-0.5.1/ataskq/test_queries.py` & `ataskq-6.0.0/ataskq/test_queries.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 import pytest
 
-from .ataskq import TaskQ, Task
-from .handler import from_connection_str
+from . import TaskQ, Task
+from .handler import from_config
 
 
 @pytest.fixture()
-def job_ids(conn):
+def job_ids(config):
     ret = []
 
-    taskq = TaskQ(conn=conn).create_job(name="job1")
+    taskq = TaskQ(config=config).create_job(name="job1")
     taskq.add_tasks(
         [
             Task(name="n1", entrypoint=""),
             Task(name="n1", entrypoint=""),
             Task(name="n2", entrypoint=""),
         ]
     )
     ret.append(taskq.job_id)
 
-    taskq = TaskQ(conn=conn).create_job(name="job2")
+    taskq = TaskQ(config=config).create_job(name="job2")
     taskq.add_tasks(
         [
             Task(name="n3", entrypoint=""),
             Task(name="n4", entrypoint=""),
             Task(name="n4", entrypoint=""),
         ]
     )
     ret.append(taskq.job_id)
 
     return ret
 
 
 @pytest.fixture()
-def handler(conn):
-    return from_connection_str(conn)
+def handler(config):
+    return from_config(config)
 
 
 def test_tasks_status(handler, job_ids):
     # job 1
     status = handler.tasks_status(job_ids[0])
 
     assert len(status) == 2
```

### Comparing `ataskq-0.5.1/ataskq.egg-info/PKG-INFO` & `ataskq-6.0.0/ataskq.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: ataskq
-Version: 0.5.1
-Summary: An in process task queue for distributed computing systems.
+Version: 6.0.0
+Summary: Easily create and run tasks (=function calls) with almost seamless transition between Local development and Distributed deployment.
 Project-URL: Homepage, https://github.com/innoviz-swt/a-task-queue
 Project-URL: Issues, https://github.com/innoviz-swt/a-task-queue/issues
 Keywords: python,task,queue,distributed systems,distributed computing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # a-task-queue
-An in process task queue for distributed computing systems.
+Easily create and run tasks (=function calls) with almost seamless transition between Local development and Distributed deployment."
 
 ## Usage
 ```python
 from ataskq import TaskQ, Task, targs
 
 # create  job
 tr = TaskQ().create_job()
@@ -28,15 +28,15 @@
 tr.add_tasks([
     Task(entrypoint='ataskq.tasks_utils.hello_world'),
     Task(entrypoint='ataskq.tasks_utils.dummy_args_task', targs=targs(
         'arg0', 'arg1', kwarg1=10, kwarg2='this is kwarg2')),
 ])
 
 # run the tasks
-tr.run() # to run in parallel add num_processes=N
+tr.run() # to run in parallel add concurrency=N
 ```
 
 more example can be found [here](./examples)
 
 ## Contributer
 setup project git hooks
 ```
```

### Comparing `ataskq-0.5.1/ataskq.egg-info/SOURCES.txt` & `ataskq-6.0.0/ataskq.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 LICENSE
 README.md
 pyproject.toml
 ataskq/__init__.py
-ataskq/ataskq.py
+ataskq/__main__.py
 ataskq/conftest.py
 ataskq/env.py
 ataskq/imodel.py
 ataskq/logger.py
 ataskq/models.py
 ataskq/monitor.py
+ataskq/taskq.py
 ataskq/test_0.py
 ataskq/test_ataskq.py
+ataskq/test_config.py
 ataskq/test_handler.py
+ataskq/test_main.py
 ataskq/test_models.py
 ataskq/test_queries.py
 ataskq/version.py
 ataskq.egg-info/PKG-INFO
 ataskq.egg-info/SOURCES.txt
 ataskq.egg-info/dependency_links.txt
 ataskq.egg-info/top_level.txt
+ataskq/config/__init__.py
+ataskq/config/config.py
+ataskq/config/load.py
 ataskq/handler/__init__.py
 ataskq/handler/db_handler.py
 ataskq/handler/handler.py
 ataskq/handler/postgresql.py
 ataskq/handler/rest_handler.py
 ataskq/handler/sqlite3.py
+ataskq/server/background.py
 ataskq/server/form_utils.py
 ataskq/server/server.py
 ataskq/server/www/ataskq-32.png
 ataskq/server/www/favicon.ico
 ataskq/server/www/index.html
 ataskq/server/www/version.txt
 ataskq/server/www/assets/index-MiCEdQXI.js
```

