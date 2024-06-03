# Comparing `tmp/morphdb_utils-0.2.1.tar.gz` & `tmp/morphdb_utils-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morphdb_utils-0.2.1.tar", max compression
+gzip compressed data, was "morphdb_utils-0.2.2.tar", max compression
```

## Comparing `morphdb_utils-0.2.1.tar` & `morphdb_utils-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      396 2024-05-28 08:58:13.260511 morphdb_utils-0.2.1/README.md
--rw-r--r--   0        0        0        0 2024-05-02 05:57:33.264458 morphdb_utils-0.2.1/morphdb_utils/__init__.py
--rw-r--r--   0        0        0     3507 2024-05-28 08:55:19.780238 morphdb_utils-0.2.1/morphdb_utils/annotations.py
--rw-r--r--   0        0        0    14710 2024-05-29 09:08:49.283069 morphdb_utils-0.2.1/morphdb_utils/api.py
--rw-r--r--   0        0        0      429 2024-05-28 08:55:19.783177 morphdb_utils-0.2.1/morphdb_utils/logging.py
--rw-r--r--   0        0        0        0 2024-05-02 05:57:33.265042 morphdb_utils-0.2.1/morphdb_utils/py.typed
--rw-r--r--   0        0        0     1766 2024-05-29 09:08:48.461741 morphdb_utils-0.2.1/morphdb_utils/type.py
--rw-r--r--   0        0        0      824 2024-05-29 09:10:08.743606 morphdb_utils-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1086 1970-01-01 00:00:00.000000 morphdb_utils-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      777 2024-06-03 04:58:03.705605 morphdb_utils-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-02 05:57:33.264458 morphdb_utils-0.2.2/morphdb_utils/__init__.py
+-rw-r--r--   0        0        0     3969 2024-06-03 04:53:18.220528 morphdb_utils-0.2.2/morphdb_utils/annotations.py
+-rw-r--r--   0        0        0    14710 2024-05-29 09:08:49.283069 morphdb_utils-0.2.2/morphdb_utils/api.py
+-rw-r--r--   0        0        0      429 2024-05-28 08:55:19.783177 morphdb_utils-0.2.2/morphdb_utils/logging.py
+-rw-r--r--   0        0        0        0 2024-05-02 05:57:33.265042 morphdb_utils-0.2.2/morphdb_utils/py.typed
+-rw-r--r--   0        0        0     1766 2024-05-29 09:08:48.461741 morphdb_utils-0.2.2/morphdb_utils/type.py
+-rw-r--r--   0        0        0      824 2024-06-03 04:58:18.788325 morphdb_utils-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1467 1970-01-01 00:00:00.000000 morphdb_utils-0.2.2/PKG-INFO
```

### Comparing `morphdb_utils-0.2.1/morphdb_utils/annotations.py` & `morphdb_utils-0.2.2/morphdb_utils/annotations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import base64
 import io
 import os
-from typing import Literal
+from typing import Literal, Optional
 
 import matplotlib.figure  # type: ignore
 import pandas as pd  # type: ignore
 import plotly  # type: ignore
 import plotly.io as pio  # type: ignore
 
 # enum type: export format
@@ -52,26 +52,30 @@
                 "displaylogo": False,
             },
         )
         buf.seek(0)
         return buf.getvalue()
 
 
-def transform(func):
+def transform(output: Optional[str] = None):
     """decorator for main functions of morph's Python Cell.
     This decorator basically does nothing but indicates that the function perform some tabluar transformation
     and returns pandas DataFrame.
     """
 
-    def wrapper(*args, **kwargs):
-        result = func(*args, **kwargs)
-        assert isinstance(result, pd.DataFrame)
-        return result
+    def decorator(func):
+        def wrapper(*args, **kwargs):
+            result = func(*args, **kwargs)
+            print(result)
+            assert isinstance(result, pd.DataFrame)
+            return result
 
-    return wrapper
+        return wrapper
+
+    return decorator
 
 
 def visualize(library: Literal["matplotlib", "plotly"]):
     """decorator for main functions of morph's Python Cell.
     This decorator indicates that the function perform some visualization and returns Figure object.
     the Figure object will be converted to HTML string and returned.
 
@@ -106,7 +110,20 @@
 
     def wrapper(*args, **kwargs):
         result = func(*args, **kwargs)
         assert isinstance(result, str)
         return result
 
     return wrapper
+
+
+def api(func):
+    """decorator for main functions of morph's Python Cell.
+    This decorator indicates that the function perform some API call and returns JSON string.
+    """
+
+    def wrapper(*args, **kwargs):
+        result = func(*args, **kwargs)
+        assert isinstance(result, dict)
+        return result
+
+    return wrapper
```

### Comparing `morphdb_utils-0.2.1/morphdb_utils/api.py` & `morphdb_utils-0.2.2/morphdb_utils/api.py`

 * *Files identical despite different names*

### Comparing `morphdb_utils-0.2.1/morphdb_utils/type.py` & `morphdb_utils-0.2.2/morphdb_utils/type.py`

 * *Files identical despite different names*

### Comparing `morphdb_utils-0.2.1/pyproject.toml` & `morphdb_utils-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "morphdb-utils"
-version = "0.2.1"
+version = "0.2.2"
 description = ""
 authors = ["shibatanaoto <naoto.shibata510@gmail.com>"]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `morphdb_utils-0.2.1/PKG-INFO` & `morphdb_utils-0.2.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morphdb-utils
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 Author: shibatanaoto
 Author-email: naoto.shibata510@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -29,7 +29,24 @@
 
 This project uses [pre-commit](https://pre-commit.com/) to enforce code quality and consistency. To install the pre-commit hooks, run the following command:
 
 ```shell
 pre-commit install
 ```
 
+## How to Publish
+
+This project uses [poetry](https://python-poetry.org/) to manage dependencies and packaging. To publish a new version of the package, run the following command:
+
+First, update the version in `pyproject.toml` file.
+
+```shell
+poetry version patch
+git commit -am "Bump version"
+git push origin develop
+```
+
+```shell
+git checkout develop
+poetry publish --build
+```
+
```

