# Comparing `tmp/python_iterutils-0.0.3.tar.gz` & `tmp/python_iterutils-0.0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_iterutils-0.0.3.tar", max compression
+gzip compressed data, was "python_iterutils-0.0.3.1.tar", max compression
```

## Comparing `python_iterutils-0.0.3.tar` & `python_iterutils-0.0.3.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_iterutils-0.0.3/LICENSE
--rwxr-xr-x   0        0        0     4535 2024-06-03 12:07:34.395955 python_iterutils-0.0.3/iterutils/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_iterutils-0.0.3/iterutils/py.typed
--rw-r--r--   0        0        0     1185 2024-06-03 12:07:52.077422 python_iterutils-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      208 2024-05-15 13:48:16.668636 python_iterutils-0.0.3/readme.md
--rw-r--r--   0        0        0     1382 1970-01-01 00:00:00.000000 python_iterutils-0.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_iterutils-0.0.3.1/LICENSE
+-rwxr-xr-x   0        0        0     4565 2024-06-03 12:08:17.796501 python_iterutils-0.0.3.1/iterutils/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_iterutils-0.0.3.1/iterutils/py.typed
+-rw-r--r--   0        0        0     1187 2024-06-03 12:08:35.433978 python_iterutils-0.0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      208 2024-05-15 13:48:16.668636 python_iterutils-0.0.3.1/readme.md
+-rw-r--r--   0        0        0     1384 1970-01-01 00:00:00.000000 python_iterutils-0.0.3.1/PKG-INFO
```

### Comparing `python_iterutils-0.0.3/LICENSE` & `python_iterutils-0.0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_iterutils-0.0.3/iterutils/__init__.py` & `python_iterutils-0.0.3.1/iterutils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,16 @@
             if callnext:
                 try:
                     callnext(e)
                 except (StopIteration, GeneratorExit):
                     break
     except BaseException as e:
         if callable(callexit):
-            callexit(it, e)
+            if not callexit(it, e):
+                raise
         else:
             raise
     finally:
         if callable(callexit):
             callexit(it, None)
```

### Comparing `python_iterutils-0.0.3/pyproject.toml` & `python_iterutils-0.0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-iterutils"
-version = "0.0.3"
+version = "0.0.3.1"
 description = "Python another itertools."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-iterutils"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-iterutils"
 keywords = ["iterable", "iterutils"]
```

### Comparing `python_iterutils-0.0.3/PKG-INFO` & `python_iterutils-0.0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-iterutils
-Version: 0.0.3
+Version: 0.0.3.1
 Summary: Python another itertools.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-iterutils
 License: MIT
 Keywords: iterable,iterutils
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
```

