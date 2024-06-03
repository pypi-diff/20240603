# Comparing `tmp/morphdb_utils-0.2.5.tar.gz` & `tmp/morphdb_utils-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morphdb_utils-0.2.5.tar", max compression
+gzip compressed data, was "morphdb_utils-0.2.6.tar", max compression
```

## Comparing `morphdb_utils-0.2.5.tar` & `morphdb_utils-0.2.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      777 2024-06-03 04:58:03.705605 morphdb_utils-0.2.5/README.md
--rw-r--r--   0        0        0        0 2024-05-02 05:57:33.264458 morphdb_utils-0.2.5/morphdb_utils/__init__.py
--rw-r--r--   0        0        0     4014 2024-06-03 06:24:45.543931 morphdb_utils-0.2.5/morphdb_utils/annotations.py
--rw-r--r--   0        0        0    14710 2024-05-29 09:08:49.283069 morphdb_utils-0.2.5/morphdb_utils/api.py
--rw-r--r--   0        0        0      429 2024-05-28 08:55:19.783177 morphdb_utils-0.2.5/morphdb_utils/logging.py
--rw-r--r--   0        0        0        0 2024-05-02 05:57:33.265042 morphdb_utils-0.2.5/morphdb_utils/py.typed
--rw-r--r--   0        0        0     1766 2024-05-29 09:08:48.461741 morphdb_utils-0.2.5/morphdb_utils/type.py
--rw-r--r--   0        0        0      824 2024-06-03 06:24:52.659485 morphdb_utils-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     1467 1970-01-01 00:00:00.000000 morphdb_utils-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      777 2024-06-03 04:58:03.705605 morphdb_utils-0.2.6/README.md
+-rw-r--r--   0        0        0        0 2024-05-02 05:57:33.264458 morphdb_utils-0.2.6/morphdb_utils/__init__.py
+-rw-r--r--   0        0        0     4446 2024-06-03 07:02:55.818478 morphdb_utils-0.2.6/morphdb_utils/annotations.py
+-rw-r--r--   0        0        0    14710 2024-05-29 09:08:49.283069 morphdb_utils-0.2.6/morphdb_utils/api.py
+-rw-r--r--   0        0        0      429 2024-05-28 08:55:19.783177 morphdb_utils-0.2.6/morphdb_utils/logging.py
+-rw-r--r--   0        0        0        0 2024-05-02 05:57:33.265042 morphdb_utils-0.2.6/morphdb_utils/py.typed
+-rw-r--r--   0        0        0     1766 2024-05-29 09:08:48.461741 morphdb_utils-0.2.6/morphdb_utils/type.py
+-rw-r--r--   0        0        0      824 2024-06-03 07:04:13.642840 morphdb_utils-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     1467 1970-01-01 00:00:00.000000 morphdb_utils-0.2.6/PKG-INFO
```

### Comparing `morphdb_utils-0.2.5/README.md` & `morphdb_utils-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `morphdb_utils-0.2.5/morphdb_utils/annotations.py` & `morphdb_utils-0.2.6/morphdb_utils/annotations.py`

 * *Files 7% similar despite different names*

```diff
@@ -70,60 +70,69 @@
             return result, extras
 
         return wrapper
 
     return decorator
 
 
-def visualize(library: Literal["matplotlib", "plotly"]):
+def visualize(library: Literal["matplotlib", "plotly"], output: Optional[str] = None):
     """decorator for main functions of morph's Python Cell.
     This decorator indicates that the function perform some visualization and returns Figure object.
     the Figure object will be converted to HTML string and returned.
 
     Args:
         library (Literal["matplotlib", "plotly"]): library used for visualization. either "matplotlib" or "plotly"
     """
 
     def decorator(func):
         def wrapper(*args, **kwargs):
             result = func(*args, **kwargs)
+            extras: Dict[str, Any] = {"output": output}
 
             # post process
             format = os.getenv("MORPH_VISUALIZATION_FORMAT", "html")
             if library == "matplotlib":
                 assert isinstance(result, matplotlib.figure.Figure)
-                return _get_html_from_mpl_image(result, format)
+                return _get_html_from_mpl_image(result, format), extras
             elif library == "plotly":
                 assert isinstance(result, plotly.graph_objs._figure.Figure)
-                return _get_html_from_plotly_image(result, format)
+                return _get_html_from_plotly_image(result, format), extras
             else:
                 raise ValueError("library should be either 'matplotlib' or 'plotly'")
 
         return wrapper
 
     return decorator
 
 
-def report(func):
+def report(output: Optional[str] = None):
     """decorator for main functions of morph's Python Cell.
     This decorator indicates that the function perform some reporting and returns markdown string.
     """
 
-    def wrapper(*args, **kwargs):
-        result = func(*args, **kwargs)
-        assert isinstance(result, str)
-        return result
+    def decorator(func: Callable):
+        def wrapper(*args, **kwargs):
+            result = func(*args, **kwargs)
+            assert isinstance(result, str)
+            extras: Dict[str, Any] = {"output": output}
+            return result, extras
 
-    return wrapper
+        return wrapper
+
+    return decorator
 
 
-def api(func):
+def api(output: Optional[str] = None):
     """decorator for main functions of morph's Python Cell.
     This decorator indicates that the function perform some API call and returns JSON string.
     """
 
-    def wrapper(*args, **kwargs):
-        result = func(*args, **kwargs)
-        assert isinstance(result, dict)
-        return result
+    def decorator(func: Callable):
+        def wrapper(*args, **kwargs):
+            result = func(*args, **kwargs)
+            assert isinstance(result, dict)
+            extras: Dict[str, Any] = {"output": output}
+            return result, extras
 
-    return wrapper
+        return wrapper
+
+    return decorator
```

### Comparing `morphdb_utils-0.2.5/morphdb_utils/api.py` & `morphdb_utils-0.2.6/morphdb_utils/api.py`

 * *Files identical despite different names*

### Comparing `morphdb_utils-0.2.5/morphdb_utils/type.py` & `morphdb_utils-0.2.6/morphdb_utils/type.py`

 * *Files identical despite different names*

### Comparing `morphdb_utils-0.2.5/pyproject.toml` & `morphdb_utils-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "morphdb-utils"
-version = "0.2.5"
+version = "0.2.6"
 description = ""
 authors = ["shibatanaoto <naoto.shibata510@gmail.com>"]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `morphdb_utils-0.2.5/PKG-INFO` & `morphdb_utils-0.2.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morphdb-utils
-Version: 0.2.5
+Version: 0.2.6
 Summary: 
 Author: shibatanaoto
 Author-email: naoto.shibata510@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

