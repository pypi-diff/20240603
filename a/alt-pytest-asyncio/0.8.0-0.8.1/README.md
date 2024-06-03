# Comparing `tmp/alt_pytest_asyncio-0.8.0.tar.gz` & `tmp/alt_pytest_asyncio-0.8.1.tar.gz`

## Comparing `alt_pytest_asyncio-0.8.0.tar` & `alt_pytest_asyncio-0.8.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.8.0/alt_pytest_asyncio/__init__.py
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.8.0/alt_pytest_asyncio/async_converters.py
--rw-r--r--   0        0        0     9299 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.8.0/alt_pytest_asyncio/plugin.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.8.0/alt_pytest_asyncio/version.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.8.0/.gitignore
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.8.0/LICENSE
--rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.8.0/README.rst
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     7833 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.8.1/alt_pytest_asyncio/__init__.py
+-rw-r--r--   0        0        0     9006 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.8.1/alt_pytest_asyncio/async_converters.py
+-rw-r--r--   0        0        0     9270 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.8.1/alt_pytest_asyncio/plugin.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.8.1/alt_pytest_asyncio/version.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.8.1/.gitignore
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.8.1/LICENSE
+-rw-r--r--   0        0        0     7282 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.8.1/README.rst
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     7961 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.8.1/PKG-INFO
```

### Comparing `alt_pytest_asyncio-0.8.0/alt_pytest_asyncio/__init__.py` & `alt_pytest_asyncio-0.8.1/alt_pytest_asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `alt_pytest_asyncio-0.8.0/alt_pytest_asyncio/async_converters.py` & `alt_pytest_asyncio-0.8.1/alt_pytest_asyncio/async_converters.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
             run(cm.__next__)
         except StopIteration:
             pass
 
     fixturedef.func = run_fixture
 
 
-def converted_async_test(ctx, test_tasks, func, timeout, *args, **kwargs):
+def converted_async_test(ctx, test_tasks, func, timeout, /, *args, **kwargs):
     """Used to replace async tests"""
     __tracebackhide__ = True
 
     info = {}
     loop = asyncio.get_event_loop_policy().get_event_loop()
 
     def look_at_task(t):
```

### Comparing `alt_pytest_asyncio-0.8.0/alt_pytest_asyncio/plugin.py` & `alt_pytest_asyncio-0.8.1/alt_pytest_asyncio/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,19 +85,19 @@
 
             original = pyfuncitem.obj
 
             @wraps(original)
             def run_obj(*args, **kwargs):
                 try:
                     self.ctx.run(lambda: None)
-                    run = lambda func, *a, **kw: self.ctx.run(func, *a, **kw)
+                    run = lambda func: self.ctx.run(func)
                 except RuntimeError:
-                    run = lambda func, *a, **kw: func(*a, **kw)
+                    run = lambda func: func()
 
-                run(original, *args, **kwargs)
+                run(partial(original, *args, **kwargs))
 
             pyfuncitem.obj = run_obj
 
         yield
 
 
 def cancel_all_tasks(loop, ignore_errors_from_tasks=None):
```

### Comparing `alt_pytest_asyncio-0.8.0/LICENSE` & `alt_pytest_asyncio-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alt_pytest_asyncio-0.8.0/README.rst` & `alt_pytest_asyncio-0.8.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,18 @@
 
 Like pytest-asyncio it supports async tests, coroutine fixtures and async
 generator fixtures.
 
 Changelog
 ---------
 
+0.8.1 - 3 June 2024
+    * Remove a namespace conflict that restricted what names could be used as
+      parametrize arguments.
+
 0.8.0 - 1 June 2024
     * Provide simple support for tests being aware of asyncio.Context
     * Remove support for python less than 3.11
     * Added support for asyncio ContextVars
 
 0.7.2 - 1 October 2023
     * Timeouts don't take affect if the debugger is active
```

### Comparing `alt_pytest_asyncio-0.8.0/pyproject.toml` & `alt_pytest_asyncio-0.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `alt_pytest_asyncio-0.8.0/PKG-INFO` & `alt_pytest_asyncio-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: alt-pytest-asyncio
-Version: 0.8.0
+Version: 0.8.1
 Summary: Alternative pytest plugin to pytest-asyncio
 Project-URL: Homepage, https://github.com/delfick/alt-pytest-asyncio
 Author-email: Stephen Moore <delfick755@gmail.com>
 License: MIT
 License-File: LICENSE
 Classifier: Framework :: Pytest
 Classifier: Topic :: Software Development :: Testing
@@ -36,14 +36,18 @@
 
 Like pytest-asyncio it supports async tests, coroutine fixtures and async
 generator fixtures.
 
 Changelog
 ---------
 
+0.8.1 - 3 June 2024
+    * Remove a namespace conflict that restricted what names could be used as
+      parametrize arguments.
+
 0.8.0 - 1 June 2024
     * Provide simple support for tests being aware of asyncio.Context
     * Remove support for python less than 3.11
     * Added support for asyncio ContextVars
 
 0.7.2 - 1 October 2023
     * Timeouts don't take affect if the debugger is active
```

