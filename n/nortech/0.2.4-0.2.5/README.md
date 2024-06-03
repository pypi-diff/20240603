# Comparing `tmp/nortech-0.2.4.tar.gz` & `tmp/nortech-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nortech-0.2.4.tar", max compression
+gzip compressed data, was "nortech-0.2.5.tar", max compression
```

## Comparing `nortech-0.2.4.tar` & `nortech-0.2.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    11357 2023-11-28 16:36:24.114062 nortech-0.2.4/LICENSE
--rw-r--r--   0        0        0     6241 2024-05-31 10:24:25.877447 nortech-0.2.4/README.md
--rw-r--r--   0        0        0        0 2023-12-03 13:52:48.203137 nortech-0.2.4/nortech/__init__.py
--rw-r--r--   0        0        0      264 2023-12-04 16:14:37.723473 nortech-0.2.4/nortech/datatools/__init__.py
--rw-r--r--   0        0        0        0 2023-12-03 14:29:51.232877 nortech-0.2.4/nortech/datatools/handlers/__init__.py
--rw-r--r--   0        0        0     2851 2024-05-31 09:47:25.221601 nortech-0.2.4/nortech/datatools/handlers/pandas.py
--rw-r--r--   0        0        0     5969 2023-12-04 17:38:36.825041 nortech-0.2.4/nortech/datatools/handlers/polars.py
--rw-r--r--   0        0        0     5471 2024-05-31 10:11:10.216887 nortech-0.2.4/nortech/datatools/repositories/S3.py
--rw-r--r--   0        0        0        0 2023-12-03 14:29:43.016646 nortech-0.2.4/nortech/datatools/repositories/__init__.py
--rw-r--r--   0        0        0        0 2023-12-03 14:29:26.578689 nortech-0.2.4/nortech/datatools/services/__init__.py
--rw-r--r--   0        0        0      609 2023-12-04 16:16:14.399442 nortech-0.2.4/nortech/datatools/services/config.py
--rw-r--r--   0        0        0        0 2023-12-03 14:10:29.817430 nortech-0.2.4/nortech/datatools/values/__init__.py
--rw-r--r--   0        0        0      537 2024-05-31 10:26:38.885861 nortech-0.2.4/nortech/datatools/values/errors.py
--rw-r--r--   0        0        0     2342 2024-05-31 10:27:03.038918 nortech-0.2.4/nortech/datatools/values/signals.py
--rw-r--r--   0        0        0      510 2024-05-29 12:39:38.725679 nortech-0.2.4/nortech/derivers/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 09:45:01.205309 nortech-0.2.4/nortech/derivers/gateways/__init__.py
--rw-r--r--   0        0        0     2755 2024-05-29 15:03:27.253913 nortech-0.2.4/nortech/derivers/gateways/customer_api.py
--rw-r--r--   0        0        0        0 2024-05-29 09:45:01.206598 nortech-0.2.4/nortech/derivers/handlers/__init__.py
--rw-r--r--   0        0        0     5678 2024-05-31 15:47:46.141001 nortech-0.2.4/nortech/derivers/handlers/deriver.py
--rw-r--r--   0        0        0        0 2024-05-29 09:45:01.203764 nortech-0.2.4/nortech/derivers/repositories/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 09:45:01.201516 nortech-0.2.4/nortech/derivers/services/__init__.py
--rw-r--r--   0        0        0      131 2024-05-29 09:45:01.201714 nortech-0.2.4/nortech/derivers/services/logger.py
--rw-r--r--   0        0        0     5431 2024-05-29 10:26:08.670198 nortech-0.2.4/nortech/derivers/services/operators.py
--rw-r--r--   0        0        0      276 2024-05-29 10:47:12.127163 nortech-0.2.4/nortech/derivers/services/physical_units.py
--rw-r--r--   0        0        0     4631 2024-05-31 16:44:52.060454 nortech-0.2.4/nortech/derivers/services/schema.py
--rw-r--r--   0        0        0     2288 2024-05-29 09:46:25.353623 nortech-0.2.4/nortech/derivers/services/visualize.py
--rw-r--r--   0        0        0        0 2024-05-29 09:45:01.197564 nortech-0.2.4/nortech/derivers/values/__init__.py
--rw-r--r--   0        0        0     2153 2024-05-31 15:51:09.054235 nortech-0.2.4/nortech/derivers/values/instance.py
--rw-r--r--   0        0        0     3918 2024-05-29 09:46:25.353139 nortech-0.2.4/nortech/derivers/values/physical_units.py
--rw-r--r--   0        0        0      351 2024-05-29 09:45:01.197672 nortech-0.2.4/nortech/derivers/values/physical_units_schema.py
--rw-r--r--   0        0        0     6007 2024-05-29 09:46:25.349173 nortech-0.2.4/nortech/derivers/values/schema.py
--rw-r--r--   0        0        0      842 2024-05-31 16:44:59.198630 nortech-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     7329 1970-01-01 00:00:00.000000 nortech-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-11-28 16:36:24.114062 nortech-0.2.5/LICENSE
+-rw-r--r--   0        0        0     6241 2024-05-31 10:24:25.877447 nortech-0.2.5/README.md
+-rw-r--r--   0        0        0        0 2023-12-03 13:52:48.203137 nortech-0.2.5/nortech/__init__.py
+-rw-r--r--   0        0        0      264 2023-12-04 16:14:37.723473 nortech-0.2.5/nortech/datatools/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-03 14:29:51.232877 nortech-0.2.5/nortech/datatools/handlers/__init__.py
+-rw-r--r--   0        0        0     2851 2024-05-31 09:47:25.221601 nortech-0.2.5/nortech/datatools/handlers/pandas.py
+-rw-r--r--   0        0        0     5969 2023-12-04 17:38:36.825041 nortech-0.2.5/nortech/datatools/handlers/polars.py
+-rw-r--r--   0        0        0     5471 2024-05-31 10:11:10.216887 nortech-0.2.5/nortech/datatools/repositories/S3.py
+-rw-r--r--   0        0        0        0 2023-12-03 14:29:43.016646 nortech-0.2.5/nortech/datatools/repositories/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-03 14:29:26.578689 nortech-0.2.5/nortech/datatools/services/__init__.py
+-rw-r--r--   0        0        0      609 2023-12-04 16:16:14.399442 nortech-0.2.5/nortech/datatools/services/config.py
+-rw-r--r--   0        0        0        0 2023-12-03 14:10:29.817430 nortech-0.2.5/nortech/datatools/values/__init__.py
+-rw-r--r--   0        0        0      537 2024-05-31 10:26:38.885861 nortech-0.2.5/nortech/datatools/values/errors.py
+-rw-r--r--   0        0        0     2611 2024-06-03 12:45:30.736635 nortech-0.2.5/nortech/datatools/values/signals.py
+-rw-r--r--   0        0        0      510 2024-05-29 12:39:38.725679 nortech-0.2.5/nortech/derivers/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 09:45:01.205309 nortech-0.2.5/nortech/derivers/gateways/__init__.py
+-rw-r--r--   0        0        0     2755 2024-05-29 15:03:27.253913 nortech-0.2.5/nortech/derivers/gateways/customer_api.py
+-rw-r--r--   0        0        0        0 2024-05-29 09:45:01.206598 nortech-0.2.5/nortech/derivers/handlers/__init__.py
+-rw-r--r--   0        0        0     5678 2024-05-31 15:47:46.141001 nortech-0.2.5/nortech/derivers/handlers/deriver.py
+-rw-r--r--   0        0        0        0 2024-05-29 09:45:01.203764 nortech-0.2.5/nortech/derivers/repositories/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 09:45:01.201516 nortech-0.2.5/nortech/derivers/services/__init__.py
+-rw-r--r--   0        0        0      131 2024-05-29 09:45:01.201714 nortech-0.2.5/nortech/derivers/services/logger.py
+-rw-r--r--   0        0        0     5431 2024-05-29 10:26:08.670198 nortech-0.2.5/nortech/derivers/services/operators.py
+-rw-r--r--   0        0        0      276 2024-05-29 10:47:12.127163 nortech-0.2.5/nortech/derivers/services/physical_units.py
+-rw-r--r--   0        0        0     4631 2024-05-31 16:45:12.253055 nortech-0.2.5/nortech/derivers/services/schema.py
+-rw-r--r--   0        0        0     2288 2024-05-29 09:46:25.353623 nortech-0.2.5/nortech/derivers/services/visualize.py
+-rw-r--r--   0        0        0        0 2024-05-29 09:45:01.197564 nortech-0.2.5/nortech/derivers/values/__init__.py
+-rw-r--r--   0        0        0     2153 2024-05-31 15:51:09.054235 nortech-0.2.5/nortech/derivers/values/instance.py
+-rw-r--r--   0        0        0     3918 2024-05-29 09:46:25.353139 nortech-0.2.5/nortech/derivers/values/physical_units.py
+-rw-r--r--   0        0        0      351 2024-05-29 09:45:01.197672 nortech-0.2.5/nortech/derivers/values/physical_units_schema.py
+-rw-r--r--   0        0        0     6007 2024-05-29 09:46:25.349173 nortech-0.2.5/nortech/derivers/values/schema.py
+-rw-r--r--   0        0        0      842 2024-06-03 12:45:42.673062 nortech-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     7329 1970-01-01 00:00:00.000000 nortech-0.2.5/PKG-INFO
```

### Comparing `nortech-0.2.4/LICENSE` & `nortech-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nortech-0.2.4/README.md` & `nortech-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `nortech-0.2.4/nortech/datatools/handlers/pandas.py` & `nortech-0.2.5/nortech/datatools/handlers/pandas.py`

 * *Files identical despite different names*

### Comparing `nortech-0.2.4/nortech/datatools/handlers/polars.py` & `nortech-0.2.5/nortech/datatools/handlers/polars.py`

 * *Files identical despite different names*

### Comparing `nortech-0.2.4/nortech/datatools/repositories/S3.py` & `nortech-0.2.5/nortech/datatools/repositories/S3.py`

 * *Files identical despite different names*

### Comparing `nortech-0.2.4/nortech/datatools/services/config.py` & `nortech-0.2.5/nortech/datatools/services/config.py`

 * *Files identical despite different names*

### Comparing `nortech-0.2.4/nortech/datatools/values/errors.py` & `nortech-0.2.5/nortech/datatools/values/errors.py`

 * *Files identical despite different names*

### Comparing `nortech-0.2.4/nortech/derivers/gateways/customer_api.py` & `nortech-0.2.5/nortech/derivers/gateways/customer_api.py`

 * *Files identical despite different names*

### Comparing `nortech-0.2.4/nortech/derivers/handlers/deriver.py` & `nortech-0.2.5/nortech/derivers/handlers/deriver.py`

 * *Files identical despite different names*

### Comparing `nortech-0.2.4/nortech/derivers/services/operators.py` & `nortech-0.2.5/nortech/derivers/services/operators.py`

 * *Files identical despite different names*

### Comparing `nortech-0.2.4/nortech/derivers/services/schema.py` & `nortech-0.2.5/nortech/derivers/services/schema.py`

 * *Files identical despite different names*

### Comparing `nortech-0.2.4/nortech/derivers/services/visualize.py` & `nortech-0.2.5/nortech/derivers/services/visualize.py`

 * *Files identical despite different names*

### Comparing `nortech-0.2.4/nortech/derivers/values/instance.py` & `nortech-0.2.5/nortech/derivers/values/instance.py`

 * *Files identical despite different names*

### Comparing `nortech-0.2.4/nortech/derivers/values/physical_units.py` & `nortech-0.2.5/nortech/derivers/values/physical_units.py`

 * *Files identical despite different names*

### Comparing `nortech-0.2.4/nortech/derivers/values/schema.py` & `nortech-0.2.5/nortech/derivers/values/schema.py`

 * *Files identical despite different names*

### Comparing `nortech-0.2.4/pyproject.toml` & `nortech-0.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nortech"
-version = "0.2.4"
+version = "0.2.5"
 description = "The official Python library for Nortech AI"
 authors = ["Nortech AI <info@nortech.ai>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://nortech.ai/"
 repository = "https://github.com/Nortech-ai/nortech-python"
```

### Comparing `nortech-0.2.4/PKG-INFO` & `nortech-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nortech
-Version: 0.2.4
+Version: 0.2.5
 Summary: The official Python library for Nortech AI
 Home-page: https://nortech.ai/
 License: Apache-2.0
 Author: Nortech AI
 Author-email: info@nortech.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

