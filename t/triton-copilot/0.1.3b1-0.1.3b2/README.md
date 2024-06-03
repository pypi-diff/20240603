# Comparing `tmp/triton_copilot-0.1.3b1.tar.gz` & `tmp/triton_copilot-0.1.3b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "triton_copilot-0.1.3b1.tar", max compression
+gzip compressed data, was "triton_copilot-0.1.3b2.tar", max compression
```

## Comparing `triton_copilot-0.1.3b1.tar` & `triton_copilot-0.1.3b2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1635 2024-05-19 18:06:06.377881 triton_copilot-0.1.3b1/README.md
--rw-r--r--   0        0        0      436 2024-06-03 09:00:32.106073 triton_copilot-0.1.3b1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-19 18:06:06.378471 triton_copilot-0.1.3b1/triton_copilot/__init__.py
--rw-r--r--   0        0        0     2878 2024-06-03 08:41:34.074529 triton_copilot-0.1.3b1/triton_copilot/build_services.py
--rw-r--r--   0        0        0    11247 2024-06-01 11:12:29.619864 triton_copilot-0.1.3b1/triton_copilot/constants.py
--rw-r--r--   0        0        0     1854 2024-06-01 11:18:07.099737 triton_copilot-0.1.3b1/triton_copilot/init_services.py
--rw-r--r--   0        0        0     6919 2024-06-03 08:41:49.569415 triton_copilot-0.1.3b1/triton_copilot/main.py
--rw-r--r--   0        0        0     2596 2024-06-01 14:59:11.248679 triton_copilot-0.1.3b1/triton_copilot/run_services.py
--rw-r--r--   0        0        0     9979 2024-06-01 14:59:11.249479 triton_copilot-0.1.3b1/triton_copilot/template/1/model.py
--rw-r--r--   0        0        0      222 2024-06-01 08:18:21.409258 triton_copilot-0.1.3b1/triton_copilot/template/Dockerfile
--rw-r--r--   0        0        0     7596 2024-06-03 08:48:06.209093 triton_copilot-0.1.3b1/triton_copilot/triton_services.py
--rw-r--r--   0        0        0     1875 2024-06-03 09:00:16.273040 triton_copilot-0.1.3b1/triton_copilot/utils.py
--rw-r--r--   0        0        0     3630 2024-06-03 08:48:06.219938 triton_copilot-0.1.3b1/triton_copilot/validate.py
--rw-r--r--   0        0        0     2269 1970-01-01 00:00:00.000000 triton_copilot-0.1.3b1/PKG-INFO
+-rw-r--r--   0        0        0     1635 2024-05-19 18:06:06.377881 triton_copilot-0.1.3b2/README.md
+-rw-r--r--   0        0        0      436 2024-06-03 09:03:23.752735 triton_copilot-0.1.3b2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-19 18:06:06.378471 triton_copilot-0.1.3b2/triton_copilot/__init__.py
+-rw-r--r--   0        0        0     2878 2024-06-03 08:41:34.074529 triton_copilot-0.1.3b2/triton_copilot/build_services.py
+-rw-r--r--   0        0        0    11247 2024-06-01 11:12:29.619864 triton_copilot-0.1.3b2/triton_copilot/constants.py
+-rw-r--r--   0        0        0     1854 2024-06-01 11:18:07.099737 triton_copilot-0.1.3b2/triton_copilot/init_services.py
+-rw-r--r--   0        0        0     6919 2024-06-03 08:41:49.569415 triton_copilot-0.1.3b2/triton_copilot/main.py
+-rw-r--r--   0        0        0     2596 2024-06-01 14:59:11.248679 triton_copilot-0.1.3b2/triton_copilot/run_services.py
+-rw-r--r--   0        0        0     9979 2024-06-01 14:59:11.249479 triton_copilot-0.1.3b2/triton_copilot/template/1/model.py
+-rw-r--r--   0        0        0      222 2024-06-01 08:18:21.409258 triton_copilot-0.1.3b2/triton_copilot/template/Dockerfile
+-rw-r--r--   0        0        0     7596 2024-06-03 08:48:06.209093 triton_copilot-0.1.3b2/triton_copilot/triton_services.py
+-rw-r--r--   0        0        0     1886 2024-06-03 09:03:12.073987 triton_copilot-0.1.3b2/triton_copilot/utils.py
+-rw-r--r--   0        0        0     3630 2024-06-03 08:48:06.219938 triton_copilot-0.1.3b2/triton_copilot/validate.py
+-rw-r--r--   0        0        0     2269 1970-01-01 00:00:00.000000 triton_copilot-0.1.3b2/PKG-INFO
```

### Comparing `triton_copilot-0.1.3b1/README.md` & `triton_copilot-0.1.3b2/README.md`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3b1/triton_copilot/build_services.py` & `triton_copilot-0.1.3b2/triton_copilot/build_services.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3b1/triton_copilot/constants.py` & `triton_copilot-0.1.3b2/triton_copilot/constants.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3b1/triton_copilot/init_services.py` & `triton_copilot-0.1.3b2/triton_copilot/init_services.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3b1/triton_copilot/main.py` & `triton_copilot-0.1.3b2/triton_copilot/main.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3b1/triton_copilot/run_services.py` & `triton_copilot-0.1.3b2/triton_copilot/run_services.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3b1/triton_copilot/template/1/model.py` & `triton_copilot-0.1.3b2/triton_copilot/template/1/model.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3b1/triton_copilot/triton_services.py` & `triton_copilot-0.1.3b2/triton_copilot/triton_services.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3b1/triton_copilot/utils.py` & `triton_copilot-0.1.3b2/triton_copilot/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import os
+import shutil
+
 import anthropic
 from openai import OpenAI
 import pkg_resources
+import shutil
 
 TEMPLATE_DIR = pkg_resources.resource_filename("triton_copilot", "template/")
 
 
 def copy_code_to_new_dir(src, dest):
     os.system(f"cp -r {src}/* {dest}")
-    os.removedirs(f"{dest}/temp")
+    shutil.rmtree(f"{dest}/temp")
 
 
 def save_config(output, directory):
     with open(os.path.join(directory, "config.pbtxt"), "w") as f:
         f.write(output)
 
 
@@ -60,12 +63,11 @@
 def rename_dir(directory, new_name):
     new_dir_name = "/".join(directory.split("/")[:-1] + [new_name])
     os.rename(directory, new_dir_name)
     return new_dir_name
 
 
 def cleanup(directory):
-    import shutil
     try:
         shutil.rmtree(directory)  # Delete the directory and its contents recursively
     except FileNotFoundError:
         pass
```

### Comparing `triton_copilot-0.1.3b1/triton_copilot/validate.py` & `triton_copilot-0.1.3b2/triton_copilot/validate.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3b1/PKG-INFO` & `triton_copilot-0.1.3b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triton-copilot
-Version: 0.1.3b1
+Version: 0.1.3b2
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```
