# Comparing `tmp/py_optional-1.3.1.tar.gz` & `tmp/py_optional-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_optional-1.3.1.tar", max compression
+gzip compressed data, was "py_optional-1.3.2.tar", max compression
```

## Comparing `py_optional-1.3.1.tar` & `py_optional-1.3.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1213 2024-06-02 16:53:52.676008 py_optional-1.3.1/AUTHORS.md
--rw-r--r--   0        0        0     1075 2024-06-02 16:53:52.676008 py_optional-1.3.1/LICENSE
--rw-r--r--   0        0        0     2512 2024-06-02 16:53:52.676008 py_optional-1.3.1/README.md
--rw-r--r--   0        0        0      327 2024-06-02 16:53:52.680008 py_optional-1.3.1/optional/__init__.py
--rw-r--r--   0        0        0      109 2024-06-02 16:53:52.680008 py_optional-1.3.1/optional/exceptions.py
--rw-r--r--   0        0        0     8606 2024-06-02 16:53:52.680008 py_optional-1.3.1/optional/optional.py
--rw-r--r--   0        0        0     3762 2024-06-02 16:53:52.680008 py_optional-1.3.1/optional/optional_property.py
--rw-r--r--   0        0        0        0 2024-06-02 16:53:52.680008 py_optional-1.3.1/optional/py.typed
--rw-r--r--   0        0        0      881 2024-06-02 16:54:07.344114 py_optional-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     3132 1970-01-01 00:00:00.000000 py_optional-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1213 2024-06-03 11:38:51.663079 py_optional-1.3.2/AUTHORS.md
+-rw-r--r--   0        0        0     1075 2024-06-03 11:38:51.663079 py_optional-1.3.2/LICENSE
+-rw-r--r--   0        0        0     2512 2024-06-03 11:38:51.663079 py_optional-1.3.2/README.md
+-rw-r--r--   0        0        0      327 2024-06-03 11:38:51.663079 py_optional-1.3.2/optional/__init__.py
+-rw-r--r--   0        0        0      109 2024-06-03 11:38:51.663079 py_optional-1.3.2/optional/exceptions.py
+-rw-r--r--   0        0        0     8606 2024-06-03 11:38:51.663079 py_optional-1.3.2/optional/optional.py
+-rw-r--r--   0        0        0     3762 2024-06-03 11:38:51.663079 py_optional-1.3.2/optional/optional_property.py
+-rw-r--r--   0        0        0        0 2024-06-03 11:38:51.663079 py_optional-1.3.2/optional/py.typed
+-rw-r--r--   0        0        0      861 2024-06-03 11:39:06.035244 py_optional-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     3112 1970-01-01 00:00:00.000000 py_optional-1.3.2/PKG-INFO
```

### Comparing `py_optional-1.3.1/AUTHORS.md` & `py_optional-1.3.2/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `py_optional-1.3.1/LICENSE` & `py_optional-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py_optional-1.3.1/README.md` & `py_optional-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `py_optional-1.3.1/optional/optional.py` & `py_optional-1.3.2/optional/optional.py`

 * *Files identical despite different names*

### Comparing `py_optional-1.3.1/optional/optional_property.py` & `py_optional-1.3.2/optional/optional_property.py`

 * *Files identical despite different names*

### Comparing `py_optional-1.3.1/pyproject.toml` & `py_optional-1.3.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "py-optional"
-version = "1.3.1"
-description = "Tools to convert SQLAlchemy models to Pydantic models"
+version = "1.3.2"
+description = "Optional value pattern for python"
 authors = ["Francisco Del Roio <francipvb@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "optional" }]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
```

### Comparing `py_optional-1.3.1/PKG-INFO` & `py_optional-1.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: py-optional
-Version: 1.3.1
-Summary: Tools to convert SQLAlchemy models to Pydantic models
+Version: 1.3.2
+Summary: Optional value pattern for python
 License: MIT
 Author: Francisco Del Roio
 Author-email: francipvb@hotmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

