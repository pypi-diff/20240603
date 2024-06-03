# Comparing `tmp/dcs_scripts-1.0.0.tar.gz` & `tmp/dcs_scripts-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcs_scripts-1.0.0.tar", max compression
+gzip compressed data, was "dcs_scripts-1.0.1.tar", max compression
```

## Comparing `dcs_scripts-1.0.0.tar` & `dcs_scripts-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      121 2024-06-02 21:35:19.763690 dcs_scripts-1.0.0/README.md
--rw-r--r--   0        0        0        0 2024-06-02 21:35:19.767690 dcs_scripts-1.0.0/dcs_scripts/__init__.py
--rw-r--r--   0        0        0     1663 2024-06-02 21:35:19.767690 dcs_scripts-1.0.0/dcs_scripts/cli.py
--rw-r--r--   0        0        0    15569 2024-06-02 21:35:19.767690 dcs_scripts-1.0.0/dcs_scripts/utils.py
--rw-r--r--   0        0        0      675 2024-06-02 21:35:19.767690 dcs_scripts-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1076 1970-01-01 00:00:00.000000 dcs_scripts-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      121 2024-06-03 00:35:02.678542 dcs_scripts-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2024-06-03 00:35:02.678542 dcs_scripts-1.0.1/dcs_scripts/__init__.py
+-rw-r--r--   0        0        0     1663 2024-06-03 00:35:02.678542 dcs_scripts-1.0.1/dcs_scripts/cli.py
+-rw-r--r--   0        0        0     3893 2024-06-03 00:35:02.678542 dcs_scripts-1.0.1/dcs_scripts/dcs_generate_plots.py
+-rw-r--r--   0        0        0    15569 2024-06-03 00:35:02.678542 dcs_scripts-1.0.1/dcs_scripts/utils.py
+-rw-r--r--   0        0        0      675 2024-06-03 00:35:02.678542 dcs_scripts-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1076 1970-01-01 00:00:00.000000 dcs_scripts-1.0.1/PKG-INFO
```

### Comparing `dcs_scripts-1.0.0/dcs_scripts/cli.py` & `dcs_scripts-1.0.1/dcs_scripts/cli.py`

 * *Files identical despite different names*

### Comparing `dcs_scripts-1.0.0/dcs_scripts/utils.py` & `dcs_scripts-1.0.1/dcs_scripts/utils.py`

 * *Files identical despite different names*

### Comparing `dcs_scripts-1.0.0/pyproject.toml` & `dcs_scripts-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcs-scripts"
-version = "1.0.0"
+version = "1.0.1"
 description = "Helper scripts for Draycon Cell Segmentation (dcs) workflows"
 authors = ["Arun Nemani <neman014@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
```

### Comparing `dcs_scripts-1.0.0/PKG-INFO` & `dcs_scripts-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcs-scripts
-Version: 1.0.0
+Version: 1.0.1
 Summary: Helper scripts for Draycon Cell Segmentation (dcs) workflows
 License: MIT
 Author: Arun Nemani
 Author-email: neman014@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

