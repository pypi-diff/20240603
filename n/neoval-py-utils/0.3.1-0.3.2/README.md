# Comparing `tmp/neoval_py_utils-0.3.1.tar.gz` & `tmp/neoval_py_utils-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neoval_py_utils-0.3.1.tar", max compression
+gzip compressed data, was "neoval_py_utils-0.3.2.tar", max compression
```

## Comparing `neoval_py_utils-0.3.1.tar` & `neoval_py_utils-0.3.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     6396 2024-04-12 02:46:39.723303 neoval_py_utils-0.3.1/README.md
--rw-r--r--   0        0        0     2818 2024-04-12 02:46:40.635305 neoval_py_utils-0.3.1/pyproject.toml
--rw-r--r--   0        0        0       35 2024-04-12 02:46:39.723303 neoval_py_utils-0.3.1/src/neoval_py_utils/__init__.py
--rw-r--r--   0        0        0     6131 2024-04-12 02:46:39.723303 neoval_py_utils-0.3.1/src/neoval_py_utils/exporter.py
--rwxr-xr-x   0        0        0     3869 2024-04-12 02:46:39.723303 neoval_py_utils-0.3.1/src/neoval_py_utils/ipdb.py
--rw-r--r--   0        0        0      553 2024-04-12 02:46:39.723303 neoval_py_utils-0.3.1/src/neoval_py_utils/ipdb_build_event.py
--rwxr-xr-x   0        0        0    21941 2024-04-12 02:46:39.723303 neoval_py_utils-0.3.1/src/neoval_py_utils/ipdb_builder.py
--rw-r--r--   0        0        0     4191 2024-04-12 02:46:39.723303 neoval_py_utils-0.3.1/src/neoval_py_utils/template.py
--rw-r--r--   0        0        0     3045 2024-04-12 02:46:39.723303 neoval_py_utils-0.3.1/src/neoval_py_utils/utils.py
--rw-r--r--   0        0        0     7099 1970-01-01 00:00:00.000000 neoval_py_utils-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     6396 2024-06-03 03:49:45.945531 neoval_py_utils-0.3.2/README.md
+-rw-r--r--   0        0        0     2818 2024-06-03 03:49:47.185548 neoval_py_utils-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0       35 2024-06-03 03:49:45.945531 neoval_py_utils-0.3.2/src/neoval_py_utils/__init__.py
+-rw-r--r--   0        0        0     6131 2024-06-03 03:49:45.945531 neoval_py_utils-0.3.2/src/neoval_py_utils/exporter.py
+-rwxr-xr-x   0        0        0     3869 2024-06-03 03:49:45.945531 neoval_py_utils-0.3.2/src/neoval_py_utils/ipdb.py
+-rw-r--r--   0        0        0      553 2024-06-03 03:49:45.945531 neoval_py_utils-0.3.2/src/neoval_py_utils/ipdb_build_event.py
+-rwxr-xr-x   0        0        0    21941 2024-06-03 03:49:45.945531 neoval_py_utils-0.3.2/src/neoval_py_utils/ipdb_builder.py
+-rw-r--r--   0        0        0     4191 2024-06-03 03:49:45.945531 neoval_py_utils-0.3.2/src/neoval_py_utils/template.py
+-rw-r--r--   0        0        0     3045 2024-06-03 03:49:45.945531 neoval_py_utils-0.3.2/src/neoval_py_utils/utils.py
+-rw-r--r--   0        0        0     7092 1970-01-01 00:00:00.000000 neoval_py_utils-0.3.2/PKG-INFO
```

### Comparing `neoval_py_utils-0.3.1/README.md` & `neoval_py_utils-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `neoval_py_utils-0.3.1/pyproject.toml` & `neoval_py_utils-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neoval-py-utils"
-version = "0.3.1"
+version = "0.3.2"
 description = ""
 authors = ["Neoval <data@neoval.io>"]
 readme = "README.md"
 packages = [{include = "neoval_py_utils", from = "src"}]
 
 
 [tool.poetry.scripts]
@@ -16,15 +16,15 @@
 google-cloud-bigquery = "*"
 polars = "*"
 pyarrow= "*"
 taskipy = "^1.12.2"
 jinja2 = "^3.1.2"
 pyyaml = "^6.0.1"
 typer = "^0.9.0"
-duckdb = "^0.9.2"
+duckdb = "0.10.*"
 
 [tool.poetry.group.dev.dependencies]
 black = "*"
 ruff = "*"
 pytest = "*"
 pytest-xdist = "*"
 pytest-cov = "*"
```

### Comparing `neoval_py_utils-0.3.1/src/neoval_py_utils/exporter.py` & `neoval_py_utils-0.3.2/src/neoval_py_utils/exporter.py`

 * *Files identical despite different names*

### Comparing `neoval_py_utils-0.3.1/src/neoval_py_utils/ipdb.py` & `neoval_py_utils-0.3.2/src/neoval_py_utils/ipdb.py`

 * *Files identical despite different names*

### Comparing `neoval_py_utils-0.3.1/src/neoval_py_utils/ipdb_build_event.py` & `neoval_py_utils-0.3.2/src/neoval_py_utils/ipdb_build_event.py`

 * *Files identical despite different names*

### Comparing `neoval_py_utils-0.3.1/src/neoval_py_utils/ipdb_builder.py` & `neoval_py_utils-0.3.2/src/neoval_py_utils/ipdb_builder.py`

 * *Files identical despite different names*

### Comparing `neoval_py_utils-0.3.1/src/neoval_py_utils/template.py` & `neoval_py_utils-0.3.2/src/neoval_py_utils/template.py`

 * *Files identical despite different names*

### Comparing `neoval_py_utils-0.3.1/src/neoval_py_utils/utils.py` & `neoval_py_utils-0.3.2/src/neoval_py_utils/utils.py`

 * *Files identical despite different names*

### Comparing `neoval_py_utils-0.3.1/PKG-INFO` & `neoval_py_utils-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: neoval-py-utils
-Version: 0.3.1
+Version: 0.3.2
 Summary: 
 Author: Neoval
 Author-email: data@neoval.io
 Requires-Python: >=3.10,<=3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: duckdb (>=0.9.2,<0.10.0)
+Requires-Dist: duckdb (==0.10.*)
 Requires-Dist: google-cloud-bigquery
 Requires-Dist: google-cloud-storage
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: polars
 Requires-Dist: pyarrow
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: taskipy (>=1.12.2,<2.0.0)
```

