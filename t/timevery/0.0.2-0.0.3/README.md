# Comparing `tmp/timevery-0.0.2.tar.gz` & `tmp/timevery-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timevery-0.0.2.tar", last modified: Tue May 28 02:57:53 2024, max compression
+gzip compressed data, was "timevery-0.0.3.tar", last modified: Mon Jun  3 06:43:27 2024, max compression
```

## Comparing `timevery-0.0.2.tar` & `timevery-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 jinqi     (1000) jinqi     (1000)        0 2024-05-28 02:57:53.881859 timevery-0.0.2/
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)     1069 2024-05-13 10:37:19.000000 timevery-0.0.2/LICENSE
--rw-r--r--   0 jinqi     (1000) jinqi     (1000)     6185 2024-05-28 02:57:53.877859 timevery-0.0.2/PKG-INFO
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)     4516 2024-05-28 02:57:14.000000 timevery-0.0.2/README.md
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)      540 2024-05-28 02:29:51.000000 timevery-0.0.2/pyproject.toml
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)       38 2024-05-28 02:57:53.881859 timevery-0.0.2/setup.cfg
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)       38 2024-05-21 09:18:30.000000 timevery-0.0.2/setup.py
-drwxrwxr-x   0 jinqi     (1000) jinqi     (1000)        0 2024-05-28 02:57:53.877859 timevery-0.0.2/src/
-drwxrwxr-x   0 jinqi     (1000) jinqi     (1000)        0 2024-05-28 02:57:53.877859 timevery-0.0.2/src/timevery/
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)      921 2024-05-28 02:41:39.000000 timevery-0.0.2/src/timevery/__init__.py
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)     5236 2024-05-28 02:53:26.000000 timevery-0.0.2/src/timevery/timer.py
-drwxrwxr-x   0 jinqi     (1000) jinqi     (1000)        0 2024-05-28 02:57:53.877859 timevery-0.0.2/src/timevery.egg-info/
--rw-r--r--   0 jinqi     (1000) jinqi     (1000)     6185 2024-05-28 02:57:53.000000 timevery-0.0.2/src/timevery.egg-info/PKG-INFO
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)      267 2024-05-28 02:57:53.000000 timevery-0.0.2/src/timevery.egg-info/SOURCES.txt
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)        1 2024-05-28 02:57:53.000000 timevery-0.0.2/src/timevery.egg-info/dependency_links.txt
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)        5 2024-05-28 02:57:53.000000 timevery-0.0.2/src/timevery.egg-info/requires.txt
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)        9 2024-05-28 02:57:53.000000 timevery-0.0.2/src/timevery.egg-info/top_level.txt
+drwxrwxr-x   0 jinqi     (1000) jinqi     (1000)        0 2024-06-03 06:43:27.294249 timevery-0.0.3/
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)     1069 2024-05-13 10:37:19.000000 timevery-0.0.3/LICENSE
+-rw-r--r--   0 jinqi     (1000) jinqi     (1000)     7947 2024-06-03 06:43:27.294249 timevery-0.0.3/PKG-INFO
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)     6278 2024-06-03 06:30:52.000000 timevery-0.0.3/README.md
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)      540 2024-06-03 06:20:05.000000 timevery-0.0.3/pyproject.toml
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)       38 2024-06-03 06:43:27.294249 timevery-0.0.3/setup.cfg
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)       38 2024-05-21 09:18:30.000000 timevery-0.0.3/setup.py
+drwxrwxr-x   0 jinqi     (1000) jinqi     (1000)        0 2024-06-03 06:43:27.294249 timevery-0.0.3/src/
+drwxrwxr-x   0 jinqi     (1000) jinqi     (1000)        0 2024-06-03 06:43:27.294249 timevery-0.0.3/src/timevery/
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)      921 2024-05-28 02:41:39.000000 timevery-0.0.3/src/timevery/__init__.py
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)     6320 2024-06-03 06:21:08.000000 timevery-0.0.3/src/timevery/timer.py
+drwxrwxr-x   0 jinqi     (1000) jinqi     (1000)        0 2024-06-03 06:43:27.294249 timevery-0.0.3/src/timevery.egg-info/
+-rw-r--r--   0 jinqi     (1000) jinqi     (1000)     7947 2024-06-03 06:43:27.000000 timevery-0.0.3/src/timevery.egg-info/PKG-INFO
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)      267 2024-06-03 06:43:27.000000 timevery-0.0.3/src/timevery.egg-info/SOURCES.txt
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)        1 2024-06-03 06:43:27.000000 timevery-0.0.3/src/timevery.egg-info/dependency_links.txt
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)        5 2024-06-03 06:43:27.000000 timevery-0.0.3/src/timevery.egg-info/requires.txt
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)        9 2024-06-03 06:43:27.000000 timevery-0.0.3/src/timevery.egg-info/top_level.txt
```

### Comparing `timevery-0.0.2/LICENSE` & `timevery-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `timevery-0.0.2/PKG-INFO` & `timevery-0.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timevery
-Version: 0.0.2
+Version: 0.0.3
 Summary: Monitor the time cost of your code easily.
 Author-email: Shi Changshan <changshanshi@outlook.com>
 License: MIT License
         
         Copyright (c) 2024 ShiChangshan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -169,10 +169,49 @@
         Locate started.
         located
         Elapsed time of Locate: 1.0011 seconds.
     ```
 
     </details>
 
+## API
+
+### `Timer`
+
+- `Timer()`
+
+    ```python
+    class Timer(ContextDecorator):
+        def __init__(
+            self,
+            name: Optional[str] = "Timer",
+            text: Optional[str] = "Elapsed time of {name}: {seconds:0.4f} seconds. ",
+            initial_text: Union[bool, str] = False,
+            show_freq: Optional[bool] = False,
+            show_report: Optional[bool] = False,
+            logger: Optional[Callable] = print,
+            time_function: Optional[Callable] = time.perf_counter,
+        ):
+            """Create a Timer.
+
+            Args:
+                name (Optional[str], optional): Timer's name. Defaults to "Timer".
+                text (Optional[str]): Then text shown when `stop()` or `lap()` is called.
+                    Defaults to "Elapsed time of {name}: {seconds:0.4f} seconds. ".
+                    Available substitutions: {name}, {milliseconds}, {seconds}, {minutes}.
+                initial_text (Union[bool, str], optional): The text shown when `start()` is called. Defaults to False.
+                show_freq (Optional[str]): Show frequency when `stop()` is called if is True. Defaults to False.
+                show_report (Optional[str]): Show report when `stop()` is called if is True. Defaults to False.
+                logger (Optional[Callable], optional): Callable to show logs. Defaults to `print`.
+                time_function (Optional[Callable], optional): The function can return a number to indicate the time it be called.
+                    Defaults to `time.perf_counter()` in seconds. `time.time()`, `time.monotonic()`, `time.process_time()` are also available.
+            """
+    ```
+
+- `Timer.start()`
+- `Timer.stop()`
+- `Timer.lap(name: Optional[str] = None)`
+- `Timer.report()`
+
 ## Acknowledgement
 
 Thanks to [this tutorial](https://realpython.com/python-timer/) and the [`codetiming`](https://github.com/realpython/codetiming) for the inspiration.
```

### Comparing `timevery-0.0.2/pyproject.toml` & `timevery-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "timevery"
-version = "0.0.2"
+version = "0.0.3"
 description = "Monitor the time cost of your code easily."
 readme = "README.md"
 authors = [{name = "Shi Changshan", email = "changshanshi@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
```

### Comparing `timevery-0.0.2/src/timevery/__init__.py` & `timevery-0.0.3/src/timevery/__init__.py`

 * *Files identical despite different names*

### Comparing `timevery-0.0.2/src/timevery.egg-info/PKG-INFO` & `timevery-0.0.3/src/timevery.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timevery
-Version: 0.0.2
+Version: 0.0.3
 Summary: Monitor the time cost of your code easily.
 Author-email: Shi Changshan <changshanshi@outlook.com>
 License: MIT License
         
         Copyright (c) 2024 ShiChangshan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -169,10 +169,49 @@
         Locate started.
         located
         Elapsed time of Locate: 1.0011 seconds.
     ```
 
     </details>
 
+## API
+
+### `Timer`
+
+- `Timer()`
+
+    ```python
+    class Timer(ContextDecorator):
+        def __init__(
+            self,
+            name: Optional[str] = "Timer",
+            text: Optional[str] = "Elapsed time of {name}: {seconds:0.4f} seconds. ",
+            initial_text: Union[bool, str] = False,
+            show_freq: Optional[bool] = False,
+            show_report: Optional[bool] = False,
+            logger: Optional[Callable] = print,
+            time_function: Optional[Callable] = time.perf_counter,
+        ):
+            """Create a Timer.
+
+            Args:
+                name (Optional[str], optional): Timer's name. Defaults to "Timer".
+                text (Optional[str]): Then text shown when `stop()` or `lap()` is called.
+                    Defaults to "Elapsed time of {name}: {seconds:0.4f} seconds. ".
+                    Available substitutions: {name}, {milliseconds}, {seconds}, {minutes}.
+                initial_text (Union[bool, str], optional): The text shown when `start()` is called. Defaults to False.
+                show_freq (Optional[str]): Show frequency when `stop()` is called if is True. Defaults to False.
+                show_report (Optional[str]): Show report when `stop()` is called if is True. Defaults to False.
+                logger (Optional[Callable], optional): Callable to show logs. Defaults to `print`.
+                time_function (Optional[Callable], optional): The function can return a number to indicate the time it be called.
+                    Defaults to `time.perf_counter()` in seconds. `time.time()`, `time.monotonic()`, `time.process_time()` are also available.
+            """
+    ```
+
+- `Timer.start()`
+- `Timer.stop()`
+- `Timer.lap(name: Optional[str] = None)`
+- `Timer.report()`
+
 ## Acknowledgement
 
 Thanks to [this tutorial](https://realpython.com/python-timer/) and the [`codetiming`](https://github.com/realpython/codetiming) for the inspiration.
```

