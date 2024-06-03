# Comparing `tmp/triton_copilot-0.1.3rc2.tar.gz` & `tmp/triton_copilot-0.1.3rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "triton_copilot-0.1.3rc2.tar", max compression
+gzip compressed data, was "triton_copilot-0.1.3rc3.tar", max compression
```

## Comparing `triton_copilot-0.1.3rc2.tar` & `triton_copilot-0.1.3rc3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1635 2024-05-19 18:06:06.377881 triton_copilot-0.1.3rc2/README.md
--rw-r--r--   0        0        0      436 2024-06-03 14:14:01.566935 triton_copilot-0.1.3rc2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-19 18:06:06.378471 triton_copilot-0.1.3rc2/triton_copilot/__init__.py
--rw-r--r--   0        0        0     2878 2024-06-03 08:41:34.074529 triton_copilot-0.1.3rc2/triton_copilot/build_services.py
--rw-r--r--   0        0        0    11247 2024-06-01 11:12:29.619864 triton_copilot-0.1.3rc2/triton_copilot/constants.py
--rw-r--r--   0        0        0     1854 2024-06-01 11:18:07.099737 triton_copilot-0.1.3rc2/triton_copilot/init_services.py
--rw-r--r--   0        0        0     7465 2024-06-03 09:43:20.382370 triton_copilot-0.1.3rc2/triton_copilot/main.py
--rw-r--r--   0        0        0     3089 2024-06-03 14:13:46.172735 triton_copilot-0.1.3rc2/triton_copilot/run_services.py
--rw-r--r--   0        0        0     9991 2024-06-03 09:21:59.859742 triton_copilot-0.1.3rc2/triton_copilot/template/1/model.py
--rw-r--r--   0        0        0      222 2024-06-01 08:18:21.409258 triton_copilot-0.1.3rc2/triton_copilot/template/Dockerfile
--rw-r--r--   0        0        0     7633 2024-06-03 09:23:44.263881 triton_copilot-0.1.3rc2/triton_copilot/triton_services.py
--rw-r--r--   0        0        0     2511 2024-06-03 09:54:42.607866 triton_copilot-0.1.3rc2/triton_copilot/utils.py
--rw-r--r--   0        0        0     3630 2024-06-03 08:48:06.219938 triton_copilot-0.1.3rc2/triton_copilot/validate.py
--rw-r--r--   0        0        0     2270 1970-01-01 00:00:00.000000 triton_copilot-0.1.3rc2/PKG-INFO
+-rw-r--r--   0        0        0     1635 2024-05-19 18:06:06.377881 triton_copilot-0.1.3rc3/README.md
+-rw-r--r--   0        0        0      436 2024-06-03 14:32:06.958267 triton_copilot-0.1.3rc3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-19 18:06:06.378471 triton_copilot-0.1.3rc3/triton_copilot/__init__.py
+-rw-r--r--   0        0        0     2878 2024-06-03 08:41:34.074529 triton_copilot-0.1.3rc3/triton_copilot/build_services.py
+-rw-r--r--   0        0        0    11247 2024-06-01 11:12:29.619864 triton_copilot-0.1.3rc3/triton_copilot/constants.py
+-rw-r--r--   0        0        0     1854 2024-06-01 11:18:07.099737 triton_copilot-0.1.3rc3/triton_copilot/init_services.py
+-rw-r--r--   0        0        0     7465 2024-06-03 09:43:20.382370 triton_copilot-0.1.3rc3/triton_copilot/main.py
+-rw-r--r--   0        0        0     3089 2024-06-03 14:13:46.172735 triton_copilot-0.1.3rc3/triton_copilot/run_services.py
+-rw-r--r--   0        0        0     9991 2024-06-03 09:21:59.859742 triton_copilot-0.1.3rc3/triton_copilot/template/1/model.py
+-rw-r--r--   0        0        0      222 2024-06-01 08:18:21.409258 triton_copilot-0.1.3rc3/triton_copilot/template/Dockerfile
+-rw-r--r--   0        0        0     7647 2024-06-03 14:31:59.152307 triton_copilot-0.1.3rc3/triton_copilot/triton_services.py
+-rw-r--r--   0        0        0     2511 2024-06-03 09:54:42.607866 triton_copilot-0.1.3rc3/triton_copilot/utils.py
+-rw-r--r--   0        0        0     3630 2024-06-03 08:48:06.219938 triton_copilot-0.1.3rc3/triton_copilot/validate.py
+-rw-r--r--   0        0        0     2270 1970-01-01 00:00:00.000000 triton_copilot-0.1.3rc3/PKG-INFO
```

### Comparing `triton_copilot-0.1.3rc2/README.md` & `triton_copilot-0.1.3rc3/README.md`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3rc2/triton_copilot/build_services.py` & `triton_copilot-0.1.3rc3/triton_copilot/build_services.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3rc2/triton_copilot/constants.py` & `triton_copilot-0.1.3rc3/triton_copilot/constants.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3rc2/triton_copilot/init_services.py` & `triton_copilot-0.1.3rc3/triton_copilot/init_services.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3rc2/triton_copilot/main.py` & `triton_copilot-0.1.3rc3/triton_copilot/main.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3rc2/triton_copilot/run_services.py` & `triton_copilot-0.1.3rc3/triton_copilot/run_services.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3rc2/triton_copilot/template/1/model.py` & `triton_copilot-0.1.3rc3/triton_copilot/template/1/model.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3rc2/triton_copilot/triton_services.py` & `triton_copilot-0.1.3rc3/triton_copilot/triton_services.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,15 +148,15 @@
     copy_code_to_new_dir(TEMPLATE_DIR, temp_dir)
     file = open(f"{temp_dir}/1/model.py", "r")
     lines = file.readlines()
     for i in range(len(lines)):
         lines[i] = lines[i].replace("##model_class##", load_ref.split(".")[0])
         lines[i] = lines[i].replace("##load_func##", load_ref.split(".")[1])
         lines[i] = lines[i].replace("##infer_func##", infer_ref.split(".")[1])
-        lines[i] = lines[i].replace("##file##", file_path.split("/")[-1])
+        lines[i] = lines[i].replace("##file##", file_path.split("/")[-1].split(".")[0])
         if unload_ref is not None and unload_ref != "None":
             lines[i] = lines[i].replace("##unload_func##", unload_ref.split(".")[1])
 
     if unload_ref is None or unload_ref == "None":
         lines = [line for line in lines if "finalize" not in line and "unload" not in line]
 
     file = open(f"{temp_dir}/1/model.py", "w")
```

### Comparing `triton_copilot-0.1.3rc2/triton_copilot/utils.py` & `triton_copilot-0.1.3rc3/triton_copilot/utils.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3rc2/triton_copilot/validate.py` & `triton_copilot-0.1.3rc3/triton_copilot/validate.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3rc2/PKG-INFO` & `triton_copilot-0.1.3rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triton-copilot
-Version: 0.1.3rc2
+Version: 0.1.3rc3
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

