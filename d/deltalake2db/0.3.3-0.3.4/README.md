# Comparing `tmp/deltalake2db-0.3.3.tar.gz` & `tmp/deltalake2db-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltalake2db-0.3.3.tar", max compression
+gzip compressed data, was "deltalake2db-0.3.4.tar", max compression
```

## Comparing `deltalake2db-0.3.3.tar` & `deltalake2db-0.3.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2066 2024-05-08 13:34:51.098398 deltalake2db-0.3.3/README.md
--rw-r--r--   0        0        0      343 2024-05-08 13:34:51.098398 deltalake2db-0.3.3/deltalake2db/__init__.py
--rw-r--r--   0        0        0     1225 2024-05-08 13:34:51.098398 deltalake2db-0.3.3/deltalake2db/azure_helper.py
--rw-r--r--   0        0        0    15196 2024-05-08 13:34:51.098398 deltalake2db-0.3.3/deltalake2db/duckdb.py
--rw-r--r--   0        0        0      889 2024-05-08 13:34:51.098398 deltalake2db-0.3.3/deltalake2db/filter_by_meta.py
--rw-r--r--   0        0        0     7614 2024-05-08 13:34:51.098398 deltalake2db-0.3.3/deltalake2db/polars.py
--rw-r--r--   0        0        0      963 2024-05-08 13:34:51.098398 deltalake2db-0.3.3/deltalake2db/protocol_check.py
--rw-r--r--   0        0        0     2666 2024-05-08 13:34:51.098398 deltalake2db-0.3.3/deltalake2db/sql_utils.py
--rw-r--r--   0        0        0      885 2024-05-08 13:34:51.098398 deltalake2db-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     2636 1970-01-01 00:00:00.000000 deltalake2db-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     2066 2024-06-03 13:33:02.662210 deltalake2db-0.3.4/README.md
+-rw-r--r--   0        0        0      343 2024-06-03 13:33:02.662210 deltalake2db-0.3.4/deltalake2db/__init__.py
+-rw-r--r--   0        0        0     1225 2024-06-03 13:33:02.662210 deltalake2db-0.3.4/deltalake2db/azure_helper.py
+-rw-r--r--   0        0        0    15196 2024-06-03 13:33:02.662210 deltalake2db-0.3.4/deltalake2db/duckdb.py
+-rw-r--r--   0        0        0      889 2024-06-03 13:33:02.662210 deltalake2db-0.3.4/deltalake2db/filter_by_meta.py
+-rw-r--r--   0        0        0     7614 2024-06-03 13:33:02.662210 deltalake2db-0.3.4/deltalake2db/polars.py
+-rw-r--r--   0        0        0      963 2024-06-03 13:33:02.662210 deltalake2db-0.3.4/deltalake2db/protocol_check.py
+-rw-r--r--   0        0        0     2666 2024-06-03 13:33:02.662210 deltalake2db-0.3.4/deltalake2db/sql_utils.py
+-rw-r--r--   0        0        0      883 2024-06-03 13:33:02.662210 deltalake2db-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     2636 1970-01-01 00:00:00.000000 deltalake2db-0.3.4/PKG-INFO
```

### Comparing `deltalake2db-0.3.3/README.md` & `deltalake2db-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `deltalake2db-0.3.3/deltalake2db/azure_helper.py` & `deltalake2db-0.3.4/deltalake2db/azure_helper.py`

 * *Files identical despite different names*

### Comparing `deltalake2db-0.3.3/deltalake2db/duckdb.py` & `deltalake2db-0.3.4/deltalake2db/duckdb.py`

 * *Files identical despite different names*

### Comparing `deltalake2db-0.3.3/deltalake2db/filter_by_meta.py` & `deltalake2db-0.3.4/deltalake2db/filter_by_meta.py`

 * *Files identical despite different names*

### Comparing `deltalake2db-0.3.3/deltalake2db/polars.py` & `deltalake2db-0.3.4/deltalake2db/polars.py`

 * *Files identical despite different names*

### Comparing `deltalake2db-0.3.3/deltalake2db/protocol_check.py` & `deltalake2db-0.3.4/deltalake2db/protocol_check.py`

 * *Files identical despite different names*

### Comparing `deltalake2db-0.3.3/deltalake2db/sql_utils.py` & `deltalake2db-0.3.4/deltalake2db/sql_utils.py`

 * *Files identical despite different names*

### Comparing `deltalake2db-0.3.3/pyproject.toml` & `deltalake2db-0.3.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [tool.poetry]
 name = "deltalake2db"
-version = "0.3.3"
+version = "0.3.4"
 description = ""
 authors = ["Adrian Ehrsam <adrian.ehrsam@bmsuisse.ch>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 deltalake = ">=0.16.1"
 sqlglot = ">=22.2.1"
 azure-identity = { version = "^1.16.0", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 pyright = "^1.1.352"
 polars = "^0.20.16"
-duckdb = "^0.10.1"
+duckdb = "^1.0.0"
 ruff = "^0.4.3"
 
 [tool.poetry.group.test.dependencies]
 pytest-cov = "^4.1.0"
 pytest = "^8.1.0"
 polars = "^0.20.13"
-duckdb = "^0.10.0"
+duckdb = "^1.0.0"
 docker = "^7.0.0"
 azure-storage-blob = "^12.19.1"
 python-dotenv = "^1.0.1"
 pandas = ">=1.4.2"
 azure-identity = "^1.16.0"
 
 [build-system]
```

### Comparing `deltalake2db-0.3.3/PKG-INFO` & `deltalake2db-0.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltalake2db
-Version: 0.3.3
+Version: 0.3.4
 Summary: 
 License: MIT
 Author: Adrian Ehrsam
 Author-email: adrian.ehrsam@bmsuisse.ch
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

