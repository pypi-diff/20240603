# Comparing `tmp/digitalhub-0.5.0b5.tar.gz` & `tmp/digitalhub-0.5.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitalhub-0.5.0b5.tar", last modified: Wed May 29 09:47:49 2024, max compression
+gzip compressed data, was "digitalhub-0.5.0b6.tar", last modified: Mon Jun  3 07:26:12 2024, max compression
```

## Comparing `digitalhub-0.5.0b5.tar` & `digitalhub-0.5.0b6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-29 09:47:49.625300 digitalhub-0.5.0b5/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    11585 2023-08-23 08:29:57.000000 digitalhub-0.5.0b5/LICENSE.txt
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)    14712 2024-05-29 09:47:49.625300 digitalhub-0.5.0b5/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      510 2024-04-23 09:36:04.000000 digitalhub-0.5.0b5/README.md
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-29 09:47:49.617300 digitalhub-0.5.0b5/digitalhub/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2218 2024-05-27 14:03:58.000000 digitalhub-0.5.0b5/digitalhub/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-29 09:47:49.625300 digitalhub-0.5.0b5/digitalhub.egg-info/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)    14712 2024-05-29 09:47:49.000000 digitalhub-0.5.0b5/digitalhub.egg-info/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      421 2024-05-29 09:47:49.000000 digitalhub-0.5.0b5/digitalhub.egg-info/SOURCES.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-05-29 09:47:49.000000 digitalhub-0.5.0b5/digitalhub.egg-info/dependency_links.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      162 2024-05-29 09:47:49.000000 digitalhub-0.5.0b5/digitalhub.egg-info/requires.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       41 2024-05-29 09:47:49.000000 digitalhub-0.5.0b5/digitalhub.egg-info/top_level.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1551 2024-05-28 11:34:48.000000 digitalhub-0.5.0b5/pyproject.toml
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-05-29 09:47:49.625300 digitalhub-0.5.0b5/setup.cfg
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-29 09:47:49.625300 digitalhub-0.5.0b5/test/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2511 2024-05-09 07:33:31.000000 digitalhub-0.5.0b5/test/test_crud_artifacts.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2504 2024-05-09 07:33:31.000000 digitalhub-0.5.0b5/test/test_crud_dataitems.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2769 2024-05-09 07:33:31.000000 digitalhub-0.5.0b5/test/test_crud_functions.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2220 2024-05-09 07:33:31.000000 digitalhub-0.5.0b5/test/test_crud_runs.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2111 2024-05-09 07:33:31.000000 digitalhub-0.5.0b5/test/test_crud_tasks.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1269 2024-03-22 13:56:51.000000 digitalhub-0.5.0b5/test/test_imports.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1086 2024-03-25 07:51:29.000000 digitalhub-0.5.0b5/test/testkfp.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      622 2024-05-27 11:24:20.000000 digitalhub-0.5.0b5/test/testkfp_pipeline.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-06-03 07:26:12.045620 digitalhub-0.5.0b6/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    11585 2023-08-23 08:29:57.000000 digitalhub-0.5.0b6/LICENSE.txt
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)    14712 2024-06-03 07:26:12.045620 digitalhub-0.5.0b6/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      510 2024-04-23 09:36:04.000000 digitalhub-0.5.0b6/README.md
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-06-03 07:26:12.041620 digitalhub-0.5.0b6/digitalhub/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2218 2024-05-30 06:51:21.000000 digitalhub-0.5.0b6/digitalhub/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-06-03 07:26:12.045620 digitalhub-0.5.0b6/digitalhub.egg-info/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)    14712 2024-06-03 07:26:12.000000 digitalhub-0.5.0b6/digitalhub.egg-info/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      421 2024-06-03 07:26:12.000000 digitalhub-0.5.0b6/digitalhub.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-06-03 07:26:12.000000 digitalhub-0.5.0b6/digitalhub.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      162 2024-06-03 07:26:12.000000 digitalhub-0.5.0b6/digitalhub.egg-info/requires.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       41 2024-06-03 07:26:12.000000 digitalhub-0.5.0b6/digitalhub.egg-info/top_level.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1551 2024-06-03 07:25:28.000000 digitalhub-0.5.0b6/pyproject.toml
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-06-03 07:26:12.045620 digitalhub-0.5.0b6/setup.cfg
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-06-03 07:26:12.041620 digitalhub-0.5.0b6/test/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2511 2024-05-09 07:33:31.000000 digitalhub-0.5.0b6/test/test_crud_artifacts.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2504 2024-05-09 07:33:31.000000 digitalhub-0.5.0b6/test/test_crud_dataitems.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2769 2024-05-09 07:33:31.000000 digitalhub-0.5.0b6/test/test_crud_functions.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2220 2024-05-09 07:33:31.000000 digitalhub-0.5.0b6/test/test_crud_runs.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2111 2024-05-09 07:33:31.000000 digitalhub-0.5.0b6/test/test_crud_tasks.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1269 2024-03-22 13:56:51.000000 digitalhub-0.5.0b6/test/test_imports.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1086 2024-03-25 07:51:29.000000 digitalhub-0.5.0b6/test/testkfp.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      622 2024-05-27 11:24:20.000000 digitalhub-0.5.0b6/test/testkfp_pipeline.py
```

### Comparing `digitalhub-0.5.0b5/LICENSE.txt` & `digitalhub-0.5.0b6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `digitalhub-0.5.0b5/PKG-INFO` & `digitalhub-0.5.0b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub
-Version: 0.5.0b5
+Version: 0.5.0b6
 Summary: Python SDK for DigitalHub
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 License:                               Apache License
                                 Version 2.0, January 2004
                              http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `digitalhub-0.5.0b5/digitalhub/__init__.py` & `digitalhub-0.5.0b6/digitalhub/__init__.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.5.0b5/digitalhub.egg-info/PKG-INFO` & `digitalhub-0.5.0b6/digitalhub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub
-Version: 0.5.0b5
+Version: 0.5.0b6
 Summary: Python SDK for DigitalHub
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 License:                               Apache License
                                 Version 2.0, January 2004
                              http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `digitalhub-0.5.0b5/pyproject.toml` & `digitalhub-0.5.0b6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digitalhub"
-version = "0.5.0b5"
+version = "0.5.0b6"
 description = "Python SDK for DigitalHub"
 readme = "README.md"
 authors = [
     { name = "Fondazione Bruno Kessler", email = "dslab@fbk.eu" },
     { name = "Matteo Martini", email = "mmartini@fbk.eu" }
 ]
 license = { file = "LICENSE.txt" }
@@ -46,15 +46,15 @@
 [tool.ruff.extend-per-file-ignores]
 "__init__.py" = ["F401"]
 
 [tool.ruff.pydocstyle]
 convention = "numpy"
 
 [tool.bumpver]
-current_version = "0.5.0b5"
+current_version = "0.5.0b6"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = false
 tag             = false
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `digitalhub-0.5.0b5/test/test_crud_artifacts.py` & `digitalhub-0.5.0b6/test/test_crud_artifacts.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.5.0b5/test/test_crud_dataitems.py` & `digitalhub-0.5.0b6/test/test_crud_dataitems.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.5.0b5/test/test_crud_functions.py` & `digitalhub-0.5.0b6/test/test_crud_functions.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.5.0b5/test/test_crud_runs.py` & `digitalhub-0.5.0b6/test/test_crud_runs.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.5.0b5/test/test_crud_tasks.py` & `digitalhub-0.5.0b6/test/test_crud_tasks.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.5.0b5/test/test_imports.py` & `digitalhub-0.5.0b6/test/test_imports.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.5.0b5/test/testkfp.py` & `digitalhub-0.5.0b6/test/testkfp.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.5.0b5/test/testkfp_pipeline.py` & `digitalhub-0.5.0b6/test/testkfp_pipeline.py`

 * *Files identical despite different names*

