# Comparing `tmp/shipyard_census-0.2.0.tar.gz` & `tmp/shipyard_census-0.2.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_census-0.2.0.tar", max compression
+gzip compressed data, was "shipyard_census-0.2.0a0.tar", max compression
```

## Comparing `shipyard_census-0.2.0.tar` & `shipyard_census-0.2.0a0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      578 2024-05-31 15:22:57.316548 shipyard_census-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       33 2023-05-12 18:48:21.825204 shipyard_census-0.2.0/shipyard_census/__init__.py
--rw-r--r--   0        0        0     5783 2024-05-31 15:22:57.317188 shipyard_census-0.2.0/shipyard_census/census.py
--rw-r--r--   0        0        0        0 2024-02-05 20:53:35.432394 shipyard_census-0.2.0/shipyard_census/cli/__init__.py
--rw-r--r--   0        0        0      182 2024-02-05 20:53:35.432711 shipyard_census-0.2.0/shipyard_census/cli/authtest.py
--rw-r--r--   0        0        0     2454 2024-05-31 15:22:57.317797 shipyard_census-0.2.0/shipyard_census/cli/trigger_sync_cli.py
--rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 shipyard_census-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      580 2024-05-31 01:56:12.726350 shipyard_census-0.2.0a0/pyproject.toml
+-rw-r--r--   0        0        0       33 2023-05-12 18:48:21.825204 shipyard_census-0.2.0a0/shipyard_census/__init__.py
+-rw-r--r--   0        0        0     5783 2024-05-31 01:15:56.800033 shipyard_census-0.2.0a0/shipyard_census/census.py
+-rw-r--r--   0        0        0        0 2024-02-05 20:53:35.432394 shipyard_census-0.2.0a0/shipyard_census/cli/__init__.py
+-rw-r--r--   0        0        0      182 2024-02-05 20:53:35.432711 shipyard_census-0.2.0a0/shipyard_census/cli/authtest.py
+-rw-r--r--   0        0        0     2454 2024-05-31 01:15:56.800384 shipyard_census-0.2.0a0/shipyard_census/cli/trigger_sync_cli.py
+-rw-r--r--   0        0        0      618 1970-01-01 00:00:00.000000 shipyard_census-0.2.0a0/PKG-INFO
```

### Comparing `shipyard_census-0.2.0/pyproject.toml` & `shipyard_census-0.2.0a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-census"
-version = "0.2.0"
+version = "0.2.0a0"
 description = "A local client for connecting and working with Census"
 authors = ["JR <johnathan.rodriguez@shipyardapp.com>", "wrp801 <wespoulsen@gmail.com>"]
 license = "Apache 2.0"
 #readme = "README.md"
 packages = [{ include = "shipyard_census" }]
 
 [tool.poetry.dependencies]
```

### Comparing `shipyard_census-0.2.0/shipyard_census/census.py` & `shipyard_census-0.2.0a0/shipyard_census/census.py`

 * *Files identical despite different names*

### Comparing `shipyard_census-0.2.0/shipyard_census/cli/trigger_sync_cli.py` & `shipyard_census-0.2.0a0/shipyard_census/cli/trigger_sync_cli.py`

 * *Files identical despite different names*

### Comparing `shipyard_census-0.2.0/PKG-INFO` & `shipyard_census-0.2.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-census
-Version: 0.2.0
+Version: 0.2.0a0
 Summary: A local client for connecting and working with Census
 License: Apache 2.0
 Author: JR
 Author-email: johnathan.rodriguez@shipyardapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

