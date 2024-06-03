# Comparing `tmp/py_optional-1.3.0.tar.gz` & `tmp/py_optional-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_optional-1.3.0.tar", max compression
+gzip compressed data, was "py_optional-1.3.1.tar", max compression
```

## Comparing `py_optional-1.3.0.tar` & `py_optional-1.3.1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1075 2024-06-02 16:41:07.321659 py_optional-1.3.0/LICENSE
--rw-r--r--   0        0        0     2512 2024-06-02 16:41:07.321659 py_optional-1.3.0/README.md
--rw-r--r--   0        0        0      327 2024-06-02 16:41:07.325659 py_optional-1.3.0/optional/__init__.py
--rw-r--r--   0        0        0      109 2024-06-02 16:41:07.325659 py_optional-1.3.0/optional/exceptions.py
--rw-r--r--   0        0        0     8606 2024-06-02 16:41:07.325659 py_optional-1.3.0/optional/optional.py
--rw-r--r--   0        0        0     3762 2024-06-02 16:41:07.325659 py_optional-1.3.0/optional/optional_property.py
--rw-r--r--   0        0        0        0 2024-06-02 16:41:07.325659 py_optional-1.3.0/optional/py.typed
--rw-r--r--   0        0        0      881 2024-06-02 16:41:22.401882 py_optional-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 py_optional-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1213 2024-06-02 16:53:52.676008 py_optional-1.3.1/AUTHORS.md
+-rw-r--r--   0        0        0     1075 2024-06-02 16:53:52.676008 py_optional-1.3.1/LICENSE
+-rw-r--r--   0        0        0     2512 2024-06-02 16:53:52.676008 py_optional-1.3.1/README.md
+-rw-r--r--   0        0        0      327 2024-06-02 16:53:52.680008 py_optional-1.3.1/optional/__init__.py
+-rw-r--r--   0        0        0      109 2024-06-02 16:53:52.680008 py_optional-1.3.1/optional/exceptions.py
+-rw-r--r--   0        0        0     8606 2024-06-02 16:53:52.680008 py_optional-1.3.1/optional/optional.py
+-rw-r--r--   0        0        0     3762 2024-06-02 16:53:52.680008 py_optional-1.3.1/optional/optional_property.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:53:52.680008 py_optional-1.3.1/optional/py.typed
+-rw-r--r--   0        0        0      881 2024-06-02 16:54:07.344114 py_optional-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3132 1970-01-01 00:00:00.000000 py_optional-1.3.1/PKG-INFO
```

### Comparing `py_optional-1.3.0/LICENSE` & `py_optional-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_optional-1.3.0/README.md` & `py_optional-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `py_optional-1.3.0/optional/optional.py` & `py_optional-1.3.1/optional/optional.py`

 * *Files identical despite different names*

### Comparing `py_optional-1.3.0/optional/optional_property.py` & `py_optional-1.3.1/optional/optional_property.py`

 * *Files identical despite different names*

### Comparing `py_optional-1.3.0/pyproject.toml` & `py_optional-1.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-optional"
-version = "1.3.0"
+version = "1.3.1"
 description = "Tools to convert SQLAlchemy models to Pydantic models"
 authors = ["Francisco Del Roio <francipvb@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "optional" }]
 
 [tool.poetry.dependencies]
```

### Comparing `py_optional-1.3.0/PKG-INFO` & `py_optional-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: py-optional
-Version: 1.3.0
+Version: 1.3.1
 Summary: Tools to convert SQLAlchemy models to Pydantic models
 License: MIT
 Author: Francisco Del Roio
 Author-email: francipvb@hotmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # py-optional
 
 [![Coverage Status](https://coveralls.io/repos/github/francipvb/py-optional/badge.svg?branch=develop)](https://coveralls.io/github/francipvb/py-optional?branch=develop)
 [![Coverage Status](https://coveralls.io/repos/github/francipvb/py-optional/badge.svg?branch=main)](https://coveralls.io/github/francipvb/py-optional?branch=main)
```

