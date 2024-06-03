# Comparing `tmp/wandb_workspaces-0.1.2.tar.gz` & `tmp/wandb_workspaces-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wandb_workspaces-0.1.2.tar", max compression
+gzip compressed data, was "wandb_workspaces-0.1.3.tar", max compression
```

## Comparing `wandb_workspaces-0.1.2.tar` & `wandb_workspaces-0.1.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    10940 2024-06-03 13:55:29.894456 wandb_workspaces-0.1.2/LICENSE
--rw-r--r--   0        0        0     2348 2024-06-03 13:58:45.095474 wandb_workspaces-0.1.2/README.md
--rw-r--r--   0        0        0     2644 2024-06-03 13:58:07.213241 wandb_workspaces-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       53 2024-06-03 13:55:29.912407 wandb_workspaces-0.1.2/wandb_workspaces/__init__.py
--rw-r--r--   0        0        0     7747 2024-06-03 13:55:29.957910 wandb_workspaces-0.1.2/wandb_workspaces/expr.py
--rw-r--r--   0        0        0        0 2024-06-03 13:55:29.941725 wandb_workspaces-0.1.2/wandb_workspaces/reports/__init__.py
--rw-r--r--   0        0        0      870 2024-06-03 13:55:29.921991 wandb_workspaces-0.1.2/wandb_workspaces/reports/v1/__init__.py
--rw-r--r--   0        0        0    53756 2024-06-03 13:55:29.920460 wandb_workspaces-0.1.2/wandb_workspaces/reports/v1/_blocks.py
--rw-r--r--   0        0        0     2136 2024-06-03 13:55:29.941122 wandb_workspaces-0.1.2/wandb_workspaces/reports/v1/_helpers.py
--rw-r--r--   0        0        0    48383 2024-06-03 13:55:29.919703 wandb_workspaces-0.1.2/wandb_workspaces/reports/v1/_panels.py
--rw-r--r--   0        0        0    18139 2024-06-03 13:55:29.940500 wandb_workspaces-0.1.2/wandb_workspaces/reports/v1/_templates.py
--rw-r--r--   0        0        0      430 2024-06-03 13:55:29.940340 wandb_workspaces-0.1.2/wandb_workspaces/reports/v1/blocks.py
--rw-r--r--   0        0        0       55 2024-06-03 13:55:29.940652 wandb_workspaces-0.1.2/wandb_workspaces/reports/v1/helpers.py
--rw-r--r--   0        0        0     1291 2024-06-03 13:55:29.921086 wandb_workspaces-0.1.2/wandb_workspaces/reports/v1/mutations.py
--rw-r--r--   0        0        0      337 2024-06-03 13:55:29.941275 wandb_workspaces-0.1.2/wandb_workspaces/reports/v1/panels.py
--rw-r--r--   0        0        0     9375 2024-06-03 13:55:29.940970 wandb_workspaces-0.1.2/wandb_workspaces/reports/v1/report.py
--rw-r--r--   0        0        0     4983 2024-06-03 13:55:29.921807 wandb_workspaces-0.1.2/wandb_workspaces/reports/v1/runset.py
--rw-r--r--   0        0        0      161 2024-06-03 13:55:29.940180 wandb_workspaces-0.1.2/wandb_workspaces/reports/v1/templates.py
--rw-r--r--   0        0        0    11950 2024-06-03 13:55:29.920883 wandb_workspaces-0.1.2/wandb_workspaces/reports/v1/util.py
--rw-r--r--   0        0        0     4282 2024-06-03 13:55:29.921428 wandb_workspaces-0.1.2/wandb_workspaces/reports/v1/validators.py
--rw-r--r--   0        0        0      384 2024-06-03 13:55:29.948066 wandb_workspaces-0.1.2/wandb_workspaces/reports/v2/__init__.py
--rw-r--r--   0        0        0      382 2024-06-03 13:55:29.957353 wandb_workspaces-0.1.2/wandb_workspaces/reports/v2/blocks.py
--rw-r--r--   0        0        0     8246 2024-06-03 13:55:29.947714 wandb_workspaces-0.1.2/wandb_workspaces/reports/v2/expr_parsing.py
--rw-r--r--   0        0        0     1329 2024-06-03 13:55:29.957503 wandb_workspaces-0.1.2/wandb_workspaces/reports/v2/gql.py
--rw-r--r--   0        0        0    57726 2024-06-03 13:55:29.947902 wandb_workspaces-0.1.2/wandb_workspaces/reports/v2/interface.py
--rw-r--r--   0        0        0    27528 2024-06-03 13:55:29.946794 wandb_workspaces-0.1.2/wandb_workspaces/reports/v2/internal.py
--rw-r--r--   0        0        0       85 2024-06-03 13:55:29.946523 wandb_workspaces-0.1.2/wandb_workspaces/reports/v2/metrics.py
--rw-r--r--   0        0        0      266 2024-06-03 13:55:29.957674 wandb_workspaces-0.1.2/wandb_workspaces/reports/v2/panels.py
--rw-r--r--   0        0        0        0 2024-06-03 13:55:29.913052 wandb_workspaces-0.1.2/wandb_workspaces/utils/__init__.py
--rw-r--r--   0        0        0     2540 2024-06-03 13:55:29.912946 wandb_workspaces-0.1.2/wandb_workspaces/utils/data_generation.py
--rw-r--r--   0        0        0     1284 2024-06-03 13:55:29.914469 wandb_workspaces-0.1.2/wandb_workspaces/utils/invertable_dict.py
--rw-r--r--   0        0        0     1806 2024-06-03 13:55:29.912753 wandb_workspaces-0.1.2/wandb_workspaces/utils/validators.py
--rw-r--r--   0        0        0       87 2024-06-03 13:55:29.917467 wandb_workspaces-0.1.2/wandb_workspaces/workspaces/__init__.py
--rw-r--r--   0        0        0       84 2024-06-03 13:55:29.918957 wandb_workspaces-0.1.2/wandb_workspaces/workspaces/errors.py
--rw-r--r--   0        0        0    20505 2024-06-03 13:55:29.917255 wandb_workspaces-0.1.2/wandb_workspaces/workspaces/interface.py
--rw-r--r--   0        0        0     6939 2024-06-03 13:55:29.916493 wandb_workspaces-0.1.2/wandb_workspaces/workspaces/internal.py
--rw-r--r--   0        0        0     3750 1970-01-01 00:00:00.000000 wandb_workspaces-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    10940 2024-06-03 13:55:29.894456 wandb_workspaces-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2348 2024-06-03 13:58:45.095474 wandb_workspaces-0.1.3/README.md
+-rw-r--r--   0        0        0     2644 2024-06-03 14:01:27.670817 wandb_workspaces-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       53 2024-06-03 13:55:29.912407 wandb_workspaces-0.1.3/wandb_workspaces/__init__.py
+-rw-r--r--   0        0        0     7747 2024-06-03 13:55:29.957910 wandb_workspaces-0.1.3/wandb_workspaces/expr.py
+-rw-r--r--   0        0        0        0 2024-06-03 13:55:29.941725 wandb_workspaces-0.1.3/wandb_workspaces/reports/__init__.py
+-rw-r--r--   0        0        0      870 2024-06-03 13:55:29.921991 wandb_workspaces-0.1.3/wandb_workspaces/reports/v1/__init__.py
+-rw-r--r--   0        0        0    53756 2024-06-03 13:55:29.920460 wandb_workspaces-0.1.3/wandb_workspaces/reports/v1/_blocks.py
+-rw-r--r--   0        0        0     2136 2024-06-03 13:55:29.941122 wandb_workspaces-0.1.3/wandb_workspaces/reports/v1/_helpers.py
+-rw-r--r--   0        0        0    48383 2024-06-03 13:55:29.919703 wandb_workspaces-0.1.3/wandb_workspaces/reports/v1/_panels.py
+-rw-r--r--   0        0        0    18139 2024-06-03 13:55:29.940500 wandb_workspaces-0.1.3/wandb_workspaces/reports/v1/_templates.py
+-rw-r--r--   0        0        0      430 2024-06-03 13:55:29.940340 wandb_workspaces-0.1.3/wandb_workspaces/reports/v1/blocks.py
+-rw-r--r--   0        0        0       55 2024-06-03 13:55:29.940652 wandb_workspaces-0.1.3/wandb_workspaces/reports/v1/helpers.py
+-rw-r--r--   0        0        0     1291 2024-06-03 13:55:29.921086 wandb_workspaces-0.1.3/wandb_workspaces/reports/v1/mutations.py
+-rw-r--r--   0        0        0      337 2024-06-03 13:55:29.941275 wandb_workspaces-0.1.3/wandb_workspaces/reports/v1/panels.py
+-rw-r--r--   0        0        0     9375 2024-06-03 13:55:29.940970 wandb_workspaces-0.1.3/wandb_workspaces/reports/v1/report.py
+-rw-r--r--   0        0        0     4983 2024-06-03 13:55:29.921807 wandb_workspaces-0.1.3/wandb_workspaces/reports/v1/runset.py
+-rw-r--r--   0        0        0      161 2024-06-03 13:55:29.940180 wandb_workspaces-0.1.3/wandb_workspaces/reports/v1/templates.py
+-rw-r--r--   0        0        0    11950 2024-06-03 13:55:29.920883 wandb_workspaces-0.1.3/wandb_workspaces/reports/v1/util.py
+-rw-r--r--   0        0        0     4282 2024-06-03 13:55:29.921428 wandb_workspaces-0.1.3/wandb_workspaces/reports/v1/validators.py
+-rw-r--r--   0        0        0      384 2024-06-03 13:55:29.948066 wandb_workspaces-0.1.3/wandb_workspaces/reports/v2/__init__.py
+-rw-r--r--   0        0        0      382 2024-06-03 13:55:29.957353 wandb_workspaces-0.1.3/wandb_workspaces/reports/v2/blocks.py
+-rw-r--r--   0        0        0     8246 2024-06-03 13:55:29.947714 wandb_workspaces-0.1.3/wandb_workspaces/reports/v2/expr_parsing.py
+-rw-r--r--   0        0        0     1329 2024-06-03 13:55:29.957503 wandb_workspaces-0.1.3/wandb_workspaces/reports/v2/gql.py
+-rw-r--r--   0        0        0    57726 2024-06-03 13:55:29.947902 wandb_workspaces-0.1.3/wandb_workspaces/reports/v2/interface.py
+-rw-r--r--   0        0        0    27528 2024-06-03 13:55:29.946794 wandb_workspaces-0.1.3/wandb_workspaces/reports/v2/internal.py
+-rw-r--r--   0        0        0       85 2024-06-03 13:55:29.946523 wandb_workspaces-0.1.3/wandb_workspaces/reports/v2/metrics.py
+-rw-r--r--   0        0        0      266 2024-06-03 13:55:29.957674 wandb_workspaces-0.1.3/wandb_workspaces/reports/v2/panels.py
+-rw-r--r--   0        0        0        0 2024-06-03 13:55:29.913052 wandb_workspaces-0.1.3/wandb_workspaces/utils/__init__.py
+-rw-r--r--   0        0        0     2540 2024-06-03 13:55:29.912946 wandb_workspaces-0.1.3/wandb_workspaces/utils/data_generation.py
+-rw-r--r--   0        0        0     1284 2024-06-03 13:55:29.914469 wandb_workspaces-0.1.3/wandb_workspaces/utils/invertable_dict.py
+-rw-r--r--   0        0        0     1806 2024-06-03 13:55:29.912753 wandb_workspaces-0.1.3/wandb_workspaces/utils/validators.py
+-rw-r--r--   0        0        0       87 2024-06-03 13:55:29.917467 wandb_workspaces-0.1.3/wandb_workspaces/workspaces/__init__.py
+-rw-r--r--   0        0        0       84 2024-06-03 13:55:29.918957 wandb_workspaces-0.1.3/wandb_workspaces/workspaces/errors.py
+-rw-r--r--   0        0        0    20505 2024-06-03 13:55:29.917255 wandb_workspaces-0.1.3/wandb_workspaces/workspaces/interface.py
+-rw-r--r--   0        0        0     6939 2024-06-03 13:55:29.916493 wandb_workspaces-0.1.3/wandb_workspaces/workspaces/internal.py
+-rw-r--r--   0        0        0     3750 1970-01-01 00:00:00.000000 wandb_workspaces-0.1.3/PKG-INFO
```

### Comparing `wandb_workspaces-0.1.2/LICENSE` & `wandb_workspaces-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wandb_workspaces-0.1.2/README.md` & `wandb_workspaces-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `wandb_workspaces-0.1.2/pyproject.toml` & `wandb_workspaces-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 license = "Apache-2.0"
 name = "wandb-workspaces"
-version = "0.1.2"
+version = "0.1.3"
 description = "A library for programatically working with the Weights & Biases UI."
 authors = ["Weights & Biases <support@wandb.com>"]
 readme = "README.md"
 homepage = "https://github.com/wandb/wandb-workspaces"
 repository = "https://github.com/wandb/wandb-workspaces"
 documentation = "https://docs.wandb.ai/"
 classifiers = [
```

### Comparing `wandb_workspaces-0.1.2/wandb_workspaces/expr.py` & `wandb_workspaces-0.1.3/wandb_workspaces/expr.py`

 * *Files identical despite different names*

### Comparing `wandb_workspaces-0.1.2/wandb_workspaces/reports/v1/__init__.py` & `wandb_workspaces-0.1.3/wandb_workspaces/reports/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `wandb_workspaces-0.1.2/wandb_workspaces/reports/v1/_blocks.py` & `wandb_workspaces-0.1.3/wandb_workspaces/reports/v1/_blocks.py`

 * *Files identical despite different names*

### Comparing `wandb_workspaces-0.1.2/wandb_workspaces/reports/v1/_helpers.py` & `wandb_workspaces-0.1.3/wandb_workspaces/reports/v1/_helpers.py`

 * *Files identical despite different names*

### Comparing `wandb_workspaces-0.1.2/wandb_workspaces/reports/v1/_panels.py` & `wandb_workspaces-0.1.3/wandb_workspaces/reports/v1/_panels.py`

 * *Files identical despite different names*

### Comparing `wandb_workspaces-0.1.2/wandb_workspaces/reports/v1/_templates.py` & `wandb_workspaces-0.1.3/wandb_workspaces/reports/v1/_templates.py`

 * *Files identical despite different names*

### Comparing `wandb_workspaces-0.1.2/wandb_workspaces/reports/v1/mutations.py` & `wandb_workspaces-0.1.3/wandb_workspaces/reports/v1/mutations.py`

 * *Files identical despite different names*

### Comparing `wandb_workspaces-0.1.2/wandb_workspaces/reports/v1/report.py` & `wandb_workspaces-0.1.3/wandb_workspaces/reports/v1/report.py`

 * *Files identical despite different names*

### Comparing `wandb_workspaces-0.1.2/wandb_workspaces/reports/v1/runset.py` & `wandb_workspaces-0.1.3/wandb_workspaces/reports/v1/runset.py`

 * *Files identical despite different names*

### Comparing `wandb_workspaces-0.1.2/wandb_workspaces/reports/v1/util.py` & `wandb_workspaces-0.1.3/wandb_workspaces/reports/v1/util.py`

 * *Files identical despite different names*

### Comparing `wandb_workspaces-0.1.2/wandb_workspaces/reports/v1/validators.py` & `wandb_workspaces-0.1.3/wandb_workspaces/reports/v1/validators.py`

 * *Files identical despite different names*

### Comparing `wandb_workspaces-0.1.2/wandb_workspaces/reports/v2/expr_parsing.py` & `wandb_workspaces-0.1.3/wandb_workspaces/reports/v2/expr_parsing.py`

 * *Files identical despite different names*

### Comparing `wandb_workspaces-0.1.2/wandb_workspaces/reports/v2/gql.py` & `wandb_workspaces-0.1.3/wandb_workspaces/reports/v2/gql.py`

 * *Files identical despite different names*

### Comparing `wandb_workspaces-0.1.2/wandb_workspaces/reports/v2/interface.py` & `wandb_workspaces-0.1.3/wandb_workspaces/reports/v2/interface.py`

 * *Files identical despite different names*

### Comparing `wandb_workspaces-0.1.2/wandb_workspaces/reports/v2/internal.py` & `wandb_workspaces-0.1.3/wandb_workspaces/reports/v2/internal.py`

 * *Files identical despite different names*

### Comparing `wandb_workspaces-0.1.2/wandb_workspaces/utils/data_generation.py` & `wandb_workspaces-0.1.3/wandb_workspaces/utils/data_generation.py`

 * *Files identical despite different names*

### Comparing `wandb_workspaces-0.1.2/wandb_workspaces/utils/invertable_dict.py` & `wandb_workspaces-0.1.3/wandb_workspaces/utils/invertable_dict.py`

 * *Files identical despite different names*

### Comparing `wandb_workspaces-0.1.2/wandb_workspaces/utils/validators.py` & `wandb_workspaces-0.1.3/wandb_workspaces/utils/validators.py`

 * *Files identical despite different names*

### Comparing `wandb_workspaces-0.1.2/wandb_workspaces/workspaces/interface.py` & `wandb_workspaces-0.1.3/wandb_workspaces/workspaces/interface.py`

 * *Files identical despite different names*

### Comparing `wandb_workspaces-0.1.2/wandb_workspaces/workspaces/internal.py` & `wandb_workspaces-0.1.3/wandb_workspaces/workspaces/internal.py`

 * *Files identical despite different names*

### Comparing `wandb_workspaces-0.1.2/PKG-INFO` & `wandb_workspaces-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wandb-workspaces
-Version: 0.1.2
+Version: 0.1.3
 Summary: A library for programatically working with the Weights & Biases UI.
 Home-page: https://github.com/wandb/wandb-workspaces
 License: Apache-2.0
 Author: Weights & Biases
 Author-email: support@wandb.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

