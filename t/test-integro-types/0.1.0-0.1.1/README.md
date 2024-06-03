# Comparing `tmp/test_integro_types-0.1.0.tar.gz` & `tmp/test_integro_types-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_integro_types-0.1.0.tar", max compression
+gzip compressed data, was "test_integro_types-0.1.1.tar", max compression
```

## Comparing `test_integro_types-0.1.0.tar` & `test_integro_types-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       53 2024-05-21 03:14:44.902033 test_integro_types-0.1.0/README.md
--rw-r--r--   0        0        0      582 2024-06-03 12:10:01.584739 test_integro_types-0.1.0/integro_api/schemas/__init__.py
--rw-r--r--   0        0        0     1691 2024-06-03 12:25:07.332013 test_integro_types-0.1.0/integro_api/schemas/api_connection.py
--rw-r--r--   0        0        0      966 2024-06-03 12:10:05.736950 test_integro_types-0.1.0/integro_api/schemas/api_provider.py
--rw-r--r--   0        0        0     1267 2024-06-03 09:49:09.220487 test_integro_types-0.1.0/integro_api/schemas/event.py
--rw-r--r--   0        0        0      915 2024-06-03 09:49:09.220487 test_integro_types-0.1.0/integro_api/schemas/job.py
--rw-r--r--   0        0        0     4193 2024-06-03 12:25:07.332013 test_integro_types-0.1.0/integro_api/schemas/sync.py
--rw-r--r--   0        0        0     1823 2024-06-03 12:16:22.685249 test_integro_types-0.1.0/integro_api/schemas/sync_role_settings_definition.py
--rw-r--r--   0        0        0      239 2024-06-03 09:49:09.220487 test_integro_types-0.1.0/integro_api/schemas/user.py
--rw-r--r--   0        0        0     1895 2024-06-03 09:49:09.220487 test_integro_types-0.1.0/integro_api/schemas/utils.py
--rw-r--r--   0        0        0     1311 2024-06-03 12:41:54.881388 test_integro_types-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      888 1970-01-01 00:00:00.000000 test_integro_types-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       53 2024-05-21 03:14:44.902033 test_integro_types-0.1.1/README.md
+-rw-r--r--   0        0        0      582 2024-06-03 12:10:01.584739 test_integro_types-0.1.1/integro_api/schemas/__init__.py
+-rw-r--r--   0        0        0     1691 2024-06-03 12:25:07.332013 test_integro_types-0.1.1/integro_api/schemas/api_connection.py
+-rw-r--r--   0        0        0      966 2024-06-03 12:10:05.736950 test_integro_types-0.1.1/integro_api/schemas/api_provider.py
+-rw-r--r--   0        0        0     1267 2024-06-03 09:49:09.220487 test_integro_types-0.1.1/integro_api/schemas/event.py
+-rw-r--r--   0        0        0      915 2024-06-03 09:49:09.220487 test_integro_types-0.1.1/integro_api/schemas/job.py
+-rw-r--r--   0        0        0     4193 2024-06-03 12:25:07.332013 test_integro_types-0.1.1/integro_api/schemas/sync.py
+-rw-r--r--   0        0        0     1823 2024-06-03 12:16:22.685249 test_integro_types-0.1.1/integro_api/schemas/sync_role_settings_definition.py
+-rw-r--r--   0        0        0      239 2024-06-03 09:49:09.220487 test_integro_types-0.1.1/integro_api/schemas/user.py
+-rw-r--r--   0        0        0     1895 2024-06-03 09:49:09.220487 test_integro_types-0.1.1/integro_api/schemas/utils.py
+-rw-r--r--   0        0        0     1320 2024-06-03 12:43:12.626531 test_integro_types-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      888 1970-01-01 00:00:00.000000 test_integro_types-0.1.1/PKG-INFO
```

### Comparing `test_integro_types-0.1.0/integro_api/schemas/__init__.py` & `test_integro_types-0.1.1/integro_api/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `test_integro_types-0.1.0/integro_api/schemas/api_connection.py` & `test_integro_types-0.1.1/integro_api/schemas/api_connection.py`

 * *Files identical despite different names*

### Comparing `test_integro_types-0.1.0/integro_api/schemas/api_provider.py` & `test_integro_types-0.1.1/integro_api/schemas/api_provider.py`

 * *Files identical despite different names*

### Comparing `test_integro_types-0.1.0/integro_api/schemas/event.py` & `test_integro_types-0.1.1/integro_api/schemas/event.py`

 * *Files identical despite different names*

### Comparing `test_integro_types-0.1.0/integro_api/schemas/job.py` & `test_integro_types-0.1.1/integro_api/schemas/job.py`

 * *Files identical despite different names*

### Comparing `test_integro_types-0.1.0/integro_api/schemas/sync.py` & `test_integro_types-0.1.1/integro_api/schemas/sync.py`

 * *Files identical despite different names*

### Comparing `test_integro_types-0.1.0/integro_api/schemas/sync_role_settings_definition.py` & `test_integro_types-0.1.1/integro_api/schemas/sync_role_settings_definition.py`

 * *Files identical despite different names*

### Comparing `test_integro_types-0.1.0/integro_api/schemas/utils.py` & `test_integro_types-0.1.1/integro_api/schemas/utils.py`

 * *Files identical despite different names*

### Comparing `test_integro_types-0.1.0/pyproject.toml` & `test_integro_types-0.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -7,19 +7,21 @@
 
 [tool.isort]
 line_length = 100
 profile = "black"
 
 [tool.poetry]
 name = "test_integro_types"
-version = "0.1.0"
+version = "0.1.1"
 description = "Types for Integro"
 authors = ["William Sawyer <william@situ.com.au>"]
 readme = "README.md"
-packages = [{ include = "schemas", from = "integro_api", to = "integro_types" }]
+packages = [
+    { include = "*", from = "integro_api/schemas", to = "integro_types" },
+]
 
 [tool.poetry.dependencies]
 python = "^3.10.0"
 
 awslambdaric = "^2.0.11"
 datamodel-code-generator = "^0.25.6"
 fastapi = "^0.111.0"
```

### Comparing `test_integro_types-0.1.0/PKG-INFO` & `test_integro_types-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test_integro_types
-Version: 0.1.0
+Version: 0.1.1
 Summary: Types for Integro
 Author: William Sawyer
 Author-email: william@situ.com.au
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

