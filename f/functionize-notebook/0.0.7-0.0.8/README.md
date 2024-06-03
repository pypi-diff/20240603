# Comparing `tmp/functionize_notebook-0.0.7.tar.gz` & `tmp/functionize_notebook-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "functionize_notebook-0.0.7.tar", last modified: Mon May 27 04:40:46 2024, max compression
+gzip compressed data, was "functionize_notebook-0.0.8.tar", last modified: Mon Jun  3 05:13:50 2024, max compression
```

## Comparing `functionize_notebook-0.0.7.tar` & `functionize_notebook-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 04:40:46.095242 functionize_notebook-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-27 04:40:36.000000 functionize_notebook-0.0.7/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-27 04:40:36.000000 functionize_notebook-0.0.7/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-27 04:40:36.000000 functionize_notebook-0.0.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-27 04:40:36.000000 functionize_notebook-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-27 04:40:46.095242 functionize_notebook-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-27 04:40:36.000000 functionize_notebook-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 04:40:46.095242 functionize_notebook-0.0.7/functionize_notebook.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-27 04:40:46.000000 functionize_notebook-0.0.7/functionize_notebook.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-27 04:40:46.000000 functionize_notebook-0.0.7/functionize_notebook.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 04:40:46.000000 functionize_notebook-0.0.7/functionize_notebook.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-27 04:40:46.000000 functionize_notebook-0.0.7/functionize_notebook.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-27 04:40:46.000000 functionize_notebook-0.0.7/functionize_notebook.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 04:40:46.095242 functionize_notebook-0.0.7/notebook_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-05-27 04:40:36.000000 functionize_notebook-0.0.7/notebook_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 04:40:46.095242 functionize_notebook-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-27 04:40:36.000000 functionize_notebook-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:13:50.482311 functionize_notebook-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-06-03 05:13:46.000000 functionize_notebook-0.0.8/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-06-03 05:13:46.000000 functionize_notebook-0.0.8/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-06-03 05:13:46.000000 functionize_notebook-0.0.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-06-03 05:13:46.000000 functionize_notebook-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-06-03 05:13:50.482311 functionize_notebook-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-06-03 05:13:46.000000 functionize_notebook-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:13:50.482311 functionize_notebook-0.0.8/functionize_notebook.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-06-03 05:13:50.000000 functionize_notebook-0.0.8/functionize_notebook.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-06-03 05:13:50.000000 functionize_notebook-0.0.8/functionize_notebook.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 05:13:50.000000 functionize_notebook-0.0.8/functionize_notebook.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-06-03 05:13:50.000000 functionize_notebook-0.0.8/functionize_notebook.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-06-03 05:13:50.000000 functionize_notebook-0.0.8/functionize_notebook.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:13:50.482311 functionize_notebook-0.0.8/notebook_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-06-03 05:13:46.000000 functionize_notebook-0.0.8/notebook_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 05:13:50.482311 functionize_notebook-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-06-03 05:13:46.000000 functionize_notebook-0.0.8/setup.py
```

### Comparing `functionize_notebook-0.0.7/LICENSE.txt` & `functionize_notebook-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `functionize_notebook-0.0.7/PKG-INFO` & `functionize_notebook-0.0.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: functionize-notebook
-Version: 0.0.7
+Version: 0.0.8
 Summary: run notebook like a function
-Home-page: https://github.com/BuiHoangTu/functionize-notebook/tree/release
+Home-page: https://github.com/BuiHoangTu/functionize-notebook/
 Author: Bui Hoang Tu
 Author-email: bhtu.work@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: AUTHORS.md
 Requires-Dist: nbformat
 Requires-Dist: nbconvert
+Requires-Dist: ipykernel
+Requires-Dist: dill
 
 functionize-notebook
 ========
 
 `functionize-notebook` allows you to wrap `jupyter-notebook` and use it like a function. It 
 allows passing input and output. It is **not** multi-thread safe.
```

### Comparing `functionize_notebook-0.0.7/README.md` & `functionize_notebook-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `functionize_notebook-0.0.7/functionize_notebook.egg-info/PKG-INFO` & `functionize_notebook-0.0.8/functionize_notebook.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: functionize-notebook
-Version: 0.0.7
+Version: 0.0.8
 Summary: run notebook like a function
-Home-page: https://github.com/BuiHoangTu/functionize-notebook/tree/release
+Home-page: https://github.com/BuiHoangTu/functionize-notebook/
 Author: Bui Hoang Tu
 Author-email: bhtu.work@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: AUTHORS.md
 Requires-Dist: nbformat
 Requires-Dist: nbconvert
+Requires-Dist: ipykernel
+Requires-Dist: dill
 
 functionize-notebook
 ========
 
 `functionize-notebook` allows you to wrap `jupyter-notebook` and use it like a function. It 
 allows passing input and output. It is **not** multi-thread safe.
```

### Comparing `functionize_notebook-0.0.7/notebook_wrapper/__init__.py` & `functionize_notebook-0.0.8/notebook_wrapper/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import pickle
+import dill as pickle
 import tempfile
 from datetime import datetime
 from pathlib import Path
 from time import sleep
 from typing import Any, List
 
 import nbformat
@@ -141,15 +141,15 @@
                 inputIndex = i
                 break
             pass
 
         newCell = nbbase.new_code_cell(
             source="""
                 from pathlib import Path
-                import pickle
+                import dill as pickle
                 
                 inputVariables = pickle.loads(Path("%s").read_bytes())
                 for key, value in inputVariables.items():
                     globals()[key] = value
                     pass
             """
             % inputPath
@@ -163,15 +163,15 @@
         if isinstance(self.outputVariable, List):
             requestVars = "[" + ",".join(self.outputVariable) + "]"
         else:
             requestVars = self.outputVariable
         newCell = nbbase.new_code_cell(
             source="""
                 from pathlib import Path
-                import pickle
+                import dill as pickle
                 
                 outputVariable = %s
                 Path("%s").write_bytes(pickle.dumps(outputVariable))
             """
             % (requestVars, outputPath)
         )
```

### Comparing `functionize_notebook-0.0.7/setup.py` & `functionize_notebook-0.0.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 
 
 setup(
     name="functionize-notebook",
     version=version,
     author="Bui Hoang Tu",
     author_email="bhtu.work@gmail.com",
-    url="https://github.com/BuiHoangTu/functionize-notebook/tree/release",
+    url="https://github.com/BuiHoangTu/functionize-notebook/",
     license="MIT",
     packages=find_packages(),
     package_dir={"notebook_wrapper": "notebook_wrapper"},
     description="run notebook like a function",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
-    install_requires=["nbformat", "nbconvert"],
+    install_requires=["nbformat", "nbconvert", "ipykernel", "dill"],
     classifiers=[
         "License :: OSI Approved :: MIT License",
     ],
 )
```

