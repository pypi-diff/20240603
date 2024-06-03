# Comparing `tmp/jupyterlite-0.4.0a2.tar.gz` & `tmp/jupyterlite-0.4.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Fri May 31 13:26:32 2024, max compression
+gzip compressed data, last modified: Mon Jun  3 14:27:47 2024, max compression
```

## Comparing `jupyterlite-0.4.0a2.tar` & `jupyterlite-0.4.0a3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       56 2024-05-31 13:26:32.000000 jupyterlite-0.4.0a2/jupyterlite/__init__.py
--rw-r--r--   0        0        0       81 2024-05-31 13:26:32.000000 jupyterlite-0.4.0a2/jupyterlite/__main__.py
--rw-r--r--   0        0        0      354 2024-05-31 13:26:32.000000 jupyterlite-0.4.0a2/jupyterlite/constants.py
--rw-r--r--   0        0        0      331 2024-05-31 13:26:32.000000 jupyterlite-0.4.0a2/jupyterlite/addons/base.py
--rw-r--r--   0        0        0     2189 2024-05-31 13:26:32.000000 jupyterlite-0.4.0a2/.gitignore
--rw-r--r--   0        0        0     1524 2024-05-31 13:26:32.000000 jupyterlite-0.4.0a2/LICENSE
--rw-r--r--   0        0        0     5688 2024-05-31 13:26:32.000000 jupyterlite-0.4.0a2/README.md
--rw-r--r--   0        0        0     1995 2024-05-31 13:26:32.000000 jupyterlite-0.4.0a2/pyproject.toml
--rw-r--r--   0        0        0     9542 2024-05-31 13:26:32.000000 jupyterlite-0.4.0a2/PKG-INFO
+-rw-r--r--   0        0        0       56 2024-06-03 14:27:47.000000 jupyterlite-0.4.0a3/jupyterlite/__init__.py
+-rw-r--r--   0        0        0       81 2024-06-03 14:27:47.000000 jupyterlite-0.4.0a3/jupyterlite/__main__.py
+-rw-r--r--   0        0        0      354 2024-06-03 14:27:47.000000 jupyterlite-0.4.0a3/jupyterlite/constants.py
+-rw-r--r--   0        0        0      331 2024-06-03 14:27:47.000000 jupyterlite-0.4.0a3/jupyterlite/addons/base.py
+-rw-r--r--   0        0        0     2189 2024-06-03 14:27:47.000000 jupyterlite-0.4.0a3/.gitignore
+-rw-r--r--   0        0        0     1524 2024-06-03 14:27:47.000000 jupyterlite-0.4.0a3/LICENSE
+-rw-r--r--   0        0        0     5688 2024-06-03 14:27:47.000000 jupyterlite-0.4.0a3/README.md
+-rw-r--r--   0        0        0     1995 2024-06-03 14:27:47.000000 jupyterlite-0.4.0a3/pyproject.toml
+-rw-r--r--   0        0        0     9542 2024-06-03 14:27:47.000000 jupyterlite-0.4.0a3/PKG-INFO
```

### Comparing `jupyterlite-0.4.0a2/.gitignore` & `jupyterlite-0.4.0a3/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlite-0.4.0a2/LICENSE` & `jupyterlite-0.4.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlite-0.4.0a2/README.md` & `jupyterlite-0.4.0a3/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlite-0.4.0a2/pyproject.toml` & `jupyterlite-0.4.0a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "jupyterlite"
 authors = [
     {name = "JupyterLite Contributors"},
 ]
 dependencies = [
-    "jupyterlite-core >=0.4.0a2",
+    "jupyterlite-core >=0.4.0a3",
 ]
 keywords = [
     "browser",
     "js",
     "jupyter",
     "jupyterlab",
     "notebook",
```

### Comparing `jupyterlite-0.4.0a2/PKG-INFO` & `jupyterlite-0.4.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyterlite
-Version: 0.4.0a2
+Version: 0.4.0a3
 Dynamic: Summary
 Project-URL: Source, https://github.com/jupyterlite/jupyterlite
 Author: JupyterLite Contributors
 License: BSD 3-Clause License
         
         Copyright (c) 2022, JupyterLite Contributors
         All rights reserved.
@@ -48,15 +48,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Pre-processors
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Requires-Python: >=3.8
-Requires-Dist: jupyterlite-core>=0.4.0a2
+Requires-Dist: jupyterlite-core>=0.4.0a3
 Provides-Extra: all
 Requires-Dist: jsonschema>=3; extra == 'all'
 Requires-Dist: jupyter-server; extra == 'all'
 Requires-Dist: jupyterlab-server<3,>=2.8.1; extra == 'all'
 Requires-Dist: jupyterlab<4.3,>=4.2.1; extra == 'all'
 Requires-Dist: libarchive-c>=4.0; extra == 'all'
 Requires-Dist: notebook<7.3,>=7.2.0; extra == 'all'
```

