# Comparing `tmp/morphdb_utils-0.2.3.tar.gz` & `tmp/morphdb_utils-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morphdb_utils-0.2.3.tar", max compression
+gzip compressed data, was "morphdb_utils-0.2.4.tar", max compression
```

## Comparing `morphdb_utils-0.2.3.tar` & `morphdb_utils-0.2.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      777 2024-06-03 04:58:03.705605 morphdb_utils-0.2.3/README.md
--rw-r--r--   0        0        0        0 2024-05-02 05:57:33.264458 morphdb_utils-0.2.3/morphdb_utils/__init__.py
--rw-r--r--   0        0        0     3969 2024-06-03 04:53:18.220528 morphdb_utils-0.2.3/morphdb_utils/annotations.py
--rw-r--r--   0        0        0    14710 2024-05-29 09:08:49.283069 morphdb_utils-0.2.3/morphdb_utils/api.py
--rw-r--r--   0        0        0      429 2024-05-28 08:55:19.783177 morphdb_utils-0.2.3/morphdb_utils/logging.py
--rw-r--r--   0        0        0        0 2024-05-02 05:57:33.265042 morphdb_utils-0.2.3/morphdb_utils/py.typed
--rw-r--r--   0        0        0     1766 2024-05-29 09:08:48.461741 morphdb_utils-0.2.3/morphdb_utils/type.py
--rw-r--r--   0        0        0      824 2024-06-03 05:03:35.330395 morphdb_utils-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1467 1970-01-01 00:00:00.000000 morphdb_utils-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      777 2024-06-03 04:58:03.705605 morphdb_utils-0.2.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-02 05:57:33.264458 morphdb_utils-0.2.4/morphdb_utils/__init__.py
+-rw-r--r--   0        0        0     3947 2024-06-03 05:58:54.302939 morphdb_utils-0.2.4/morphdb_utils/annotations.py
+-rw-r--r--   0        0        0    14710 2024-05-29 09:08:49.283069 morphdb_utils-0.2.4/morphdb_utils/api.py
+-rw-r--r--   0        0        0      429 2024-05-28 08:55:19.783177 morphdb_utils-0.2.4/morphdb_utils/logging.py
+-rw-r--r--   0        0        0        0 2024-05-02 05:57:33.265042 morphdb_utils-0.2.4/morphdb_utils/py.typed
+-rw-r--r--   0        0        0     1766 2024-05-29 09:08:48.461741 morphdb_utils-0.2.4/morphdb_utils/type.py
+-rw-r--r--   0        0        0      824 2024-06-03 05:58:59.656536 morphdb_utils-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1467 1970-01-01 00:00:00.000000 morphdb_utils-0.2.4/PKG-INFO
```

### Comparing `morphdb_utils-0.2.3/README.md` & `morphdb_utils-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `morphdb_utils-0.2.3/morphdb_utils/annotations.py` & `morphdb_utils-0.2.4/morphdb_utils/annotations.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import base64
 import io
 import os
-from typing import Literal, Optional
+from typing import Callable, Literal, Optional
 
 import matplotlib.figure  # type: ignore
 import pandas as pd  # type: ignore
 import plotly  # type: ignore
 import plotly.io as pio  # type: ignore
 
 # enum type: export format
@@ -53,25 +53,24 @@
             },
         )
         buf.seek(0)
         return buf.getvalue()
 
 
 def transform(output: Optional[str] = None):
-    """decorator for main functions of morph's Python Cell.
-    This decorator basically does nothing but indicates that the function perform some tabluar transformation
-    and returns pandas DataFrame.
+    """Decorator for main functions of Morph's Python Cell.
+    This decorator indicates that the function performs some tabular transformation
+    and returns a pandas DataFrame.
     """
 
-    def decorator(func):
+    def decorator(func: Callable):
         def wrapper(*args, **kwargs):
             result = func(*args, **kwargs)
-            print(result)
             assert isinstance(result, pd.DataFrame)
-            return result
+            return result, output
 
         return wrapper
 
     return decorator
 
 
 def visualize(library: Literal["matplotlib", "plotly"]):
```

### Comparing `morphdb_utils-0.2.3/morphdb_utils/api.py` & `morphdb_utils-0.2.4/morphdb_utils/api.py`

 * *Files identical despite different names*

### Comparing `morphdb_utils-0.2.3/morphdb_utils/type.py` & `morphdb_utils-0.2.4/morphdb_utils/type.py`

 * *Files identical despite different names*

### Comparing `morphdb_utils-0.2.3/pyproject.toml` & `morphdb_utils-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "morphdb-utils"
-version = "0.2.3"
+version = "0.2.4"
 description = ""
 authors = ["shibatanaoto <naoto.shibata510@gmail.com>"]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `morphdb_utils-0.2.3/PKG-INFO` & `morphdb_utils-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morphdb-utils
-Version: 0.2.3
+Version: 0.2.4
 Summary: 
 Author: shibatanaoto
 Author-email: naoto.shibata510@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

