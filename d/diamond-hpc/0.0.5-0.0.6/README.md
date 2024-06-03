# Comparing `tmp/diamond-hpc-0.0.5.tar.gz` & `tmp/diamond-hpc-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diamond-hpc-0.0.5.tar", last modified: Sat Jun  1 19:44:56 2024, max compression
+gzip compressed data, was "diamond-hpc-0.0.6.tar", last modified: Mon Jun  3 15:25:13 2024, max compression
```

## Comparing `diamond-hpc-0.0.5.tar` & `diamond-hpc-0.0.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-06-01 19:44:56.023372 diamond-hpc-0.0.5/
--rw-r--r--   0 hotine    (1000) hotine    (1000)     1069 2024-05-21 23:35:15.000000 diamond-hpc-0.0.5/LICENSE
--rw-r--r--   0 hotine    (1000) hotine    (1000)     1789 2024-06-01 19:44:56.023372 diamond-hpc-0.0.5/PKG-INFO
--rw-r--r--   0 hotine    (1000) hotine    (1000)     1282 2024-05-31 19:26:48.000000 diamond-hpc-0.0.5/README.md
-drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-06-01 19:44:56.023372 diamond-hpc-0.0.5/diamond/
--rw-r--r--   0 hotine    (1000) hotine    (1000)        0 2024-05-21 23:35:15.000000 diamond-hpc-0.0.5/diamond/__init__.py
-drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-06-01 19:44:56.023372 diamond-hpc-0.0.5/diamond/container/
--rw-r--r--   0 hotine    (1000) hotine    (1000)        0 2024-05-21 23:35:15.000000 diamond-hpc-0.0.5/diamond/container/__init__.py
--rw-r--r--   0 hotine    (1000) hotine    (1000)     7107 2024-05-21 23:35:15.000000 diamond-hpc-0.0.5/diamond/container/container.py
-drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-06-01 19:44:56.023372 diamond-hpc-0.0.5/diamond/container/custom_image_builder/
--rw-r--r--   0 hotine    (1000) hotine    (1000)       55 2024-05-21 23:35:15.000000 diamond-hpc-0.0.5/diamond/container/custom_image_builder/__init__.py
-drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-06-01 19:44:56.023372 diamond-hpc-0.0.5/diamond/container/custom_image_builder/exception/
--rw-r--r--   0 hotine    (1000) hotine    (1000)      142 2024-05-21 23:35:15.000000 diamond-hpc-0.0.5/diamond/container/custom_image_builder/exception/ImageBuilderException.py
--rw-r--r--   0 hotine    (1000) hotine    (1000)      143 2024-05-21 23:35:15.000000 diamond-hpc-0.0.5/diamond/container/custom_image_builder/exception/RegisterImageException.py
--rw-r--r--   0 hotine    (1000) hotine    (1000)        0 2024-05-21 23:35:15.000000 diamond-hpc-0.0.5/diamond/container/custom_image_builder/exception/__init__.py
--rw-r--r--   0 hotine    (1000) hotine    (1000)     7174 2024-05-28 00:38:00.000000 diamond-hpc-0.0.5/diamond/container/custom_image_builder/image_builder.py
-drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-06-01 19:44:56.023372 diamond-hpc-0.0.5/diamond/diamond_client/
--rw-r--r--   0 hotine    (1000) hotine    (1000)        0 2024-05-28 00:38:00.000000 diamond-hpc-0.0.5/diamond/diamond_client/__init__.py
--rw-r--r--   0 hotine    (1000) hotine    (1000)     3010 2024-06-01 19:44:07.000000 diamond-hpc-0.0.5/diamond/diamond_client/diamond_client.py
-drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-06-01 19:44:56.023372 diamond-hpc-0.0.5/diamond/diamond_client/templates/
--rw-r--r--   0 hotine    (1000) hotine    (1000)      772 2024-05-28 00:38:00.000000 diamond-hpc-0.0.5/diamond/diamond_client/templates/task_template
-drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-06-01 19:44:56.023372 diamond-hpc-0.0.5/diamond/wrapper/
--rw-r--r--   0 hotine    (1000) hotine    (1000)        0 2024-05-21 23:35:15.000000 diamond-hpc-0.0.5/diamond/wrapper/__init__.py
--rw-r--r--   0 hotine    (1000) hotine    (1000)     2285 2024-06-01 19:43:36.000000 diamond-hpc-0.0.5/diamond/wrapper/wrapper.py
-drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-06-01 19:44:56.023372 diamond-hpc-0.0.5/diamond_hpc.egg-info/
--rw-r--r--   0 hotine    (1000) hotine    (1000)     1789 2024-06-01 19:44:56.000000 diamond-hpc-0.0.5/diamond_hpc.egg-info/PKG-INFO
--rw-r--r--   0 hotine    (1000) hotine    (1000)      814 2024-06-01 19:44:56.000000 diamond-hpc-0.0.5/diamond_hpc.egg-info/SOURCES.txt
--rw-r--r--   0 hotine    (1000) hotine    (1000)        1 2024-06-01 19:44:56.000000 diamond-hpc-0.0.5/diamond_hpc.egg-info/dependency_links.txt
--rw-r--r--   0 hotine    (1000) hotine    (1000)       61 2024-06-01 19:44:56.000000 diamond-hpc-0.0.5/diamond_hpc.egg-info/entry_points.txt
--rw-r--r--   0 hotine    (1000) hotine    (1000)       71 2024-06-01 19:44:56.000000 diamond-hpc-0.0.5/diamond_hpc.egg-info/requires.txt
--rw-r--r--   0 hotine    (1000) hotine    (1000)        8 2024-06-01 19:44:56.000000 diamond-hpc-0.0.5/diamond_hpc.egg-info/top_level.txt
--rw-r--r--   0 hotine    (1000) hotine    (1000)       38 2024-06-01 19:44:56.023372 diamond-hpc-0.0.5/setup.cfg
--rw-r--r--   0 hotine    (1000) hotine    (1000)      971 2024-06-01 19:44:25.000000 diamond-hpc-0.0.5/setup.py
+drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-06-03 15:25:13.712169 diamond-hpc-0.0.6/
+-rw-r--r--   0 hotine    (1000) hotine    (1000)     1069 2024-05-21 23:35:15.000000 diamond-hpc-0.0.6/LICENSE
+-rw-r--r--   0 hotine    (1000) hotine    (1000)     1789 2024-06-03 15:25:13.712169 diamond-hpc-0.0.6/PKG-INFO
+-rw-r--r--   0 hotine    (1000) hotine    (1000)     1282 2024-05-31 19:26:48.000000 diamond-hpc-0.0.6/README.md
+drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-06-03 15:25:13.712169 diamond-hpc-0.0.6/diamond/
+-rw-r--r--   0 hotine    (1000) hotine    (1000)        0 2024-05-21 23:35:15.000000 diamond-hpc-0.0.6/diamond/__init__.py
+drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-06-03 15:25:13.712169 diamond-hpc-0.0.6/diamond/container/
+-rw-r--r--   0 hotine    (1000) hotine    (1000)        0 2024-05-21 23:35:15.000000 diamond-hpc-0.0.6/diamond/container/__init__.py
+-rw-r--r--   0 hotine    (1000) hotine    (1000)     7107 2024-05-21 23:35:15.000000 diamond-hpc-0.0.6/diamond/container/container.py
+drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-06-03 15:25:13.712169 diamond-hpc-0.0.6/diamond/container/custom_image_builder/
+-rw-r--r--   0 hotine    (1000) hotine    (1000)       55 2024-05-21 23:35:15.000000 diamond-hpc-0.0.6/diamond/container/custom_image_builder/__init__.py
+drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-06-03 15:25:13.712169 diamond-hpc-0.0.6/diamond/container/custom_image_builder/exception/
+-rw-r--r--   0 hotine    (1000) hotine    (1000)      142 2024-05-21 23:35:15.000000 diamond-hpc-0.0.6/diamond/container/custom_image_builder/exception/ImageBuilderException.py
+-rw-r--r--   0 hotine    (1000) hotine    (1000)      143 2024-05-21 23:35:15.000000 diamond-hpc-0.0.6/diamond/container/custom_image_builder/exception/RegisterImageException.py
+-rw-r--r--   0 hotine    (1000) hotine    (1000)        0 2024-05-21 23:35:15.000000 diamond-hpc-0.0.6/diamond/container/custom_image_builder/exception/__init__.py
+-rw-r--r--   0 hotine    (1000) hotine    (1000)     7174 2024-05-28 00:38:00.000000 diamond-hpc-0.0.6/diamond/container/custom_image_builder/image_builder.py
+drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-06-03 15:25:13.712169 diamond-hpc-0.0.6/diamond/diamond_client/
+-rw-r--r--   0 hotine    (1000) hotine    (1000)        0 2024-05-28 00:38:00.000000 diamond-hpc-0.0.6/diamond/diamond_client/__init__.py
+-rw-r--r--   0 hotine    (1000) hotine    (1000)     3010 2024-06-03 15:14:30.000000 diamond-hpc-0.0.6/diamond/diamond_client/diamond_client.py
+drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-06-03 15:25:13.712169 diamond-hpc-0.0.6/diamond/diamond_client/templates/
+-rw-r--r--   0 hotine    (1000) hotine    (1000)      772 2024-05-28 00:38:00.000000 diamond-hpc-0.0.6/diamond/diamond_client/templates/task_template
+drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-06-03 15:25:13.712169 diamond-hpc-0.0.6/diamond/wrapper/
+-rw-r--r--   0 hotine    (1000) hotine    (1000)        0 2024-05-21 23:35:15.000000 diamond-hpc-0.0.6/diamond/wrapper/__init__.py
+-rw-r--r--   0 hotine    (1000) hotine    (1000)     2285 2024-06-03 15:14:30.000000 diamond-hpc-0.0.6/diamond/wrapper/wrapper.py
+drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-06-03 15:25:13.712169 diamond-hpc-0.0.6/diamond_hpc.egg-info/
+-rw-r--r--   0 hotine    (1000) hotine    (1000)     1789 2024-06-03 15:25:13.000000 diamond-hpc-0.0.6/diamond_hpc.egg-info/PKG-INFO
+-rw-r--r--   0 hotine    (1000) hotine    (1000)      814 2024-06-03 15:25:13.000000 diamond-hpc-0.0.6/diamond_hpc.egg-info/SOURCES.txt
+-rw-r--r--   0 hotine    (1000) hotine    (1000)        1 2024-06-03 15:25:13.000000 diamond-hpc-0.0.6/diamond_hpc.egg-info/dependency_links.txt
+-rw-r--r--   0 hotine    (1000) hotine    (1000)       61 2024-06-03 15:25:13.000000 diamond-hpc-0.0.6/diamond_hpc.egg-info/entry_points.txt
+-rw-r--r--   0 hotine    (1000) hotine    (1000)      109 2024-06-03 15:25:13.000000 diamond-hpc-0.0.6/diamond_hpc.egg-info/requires.txt
+-rw-r--r--   0 hotine    (1000) hotine    (1000)        8 2024-06-03 15:25:13.000000 diamond-hpc-0.0.6/diamond_hpc.egg-info/top_level.txt
+-rw-r--r--   0 hotine    (1000) hotine    (1000)       38 2024-06-03 15:25:13.712169 diamond-hpc-0.0.6/setup.cfg
+-rw-r--r--   0 hotine    (1000) hotine    (1000)     1031 2024-06-03 15:22:14.000000 diamond-hpc-0.0.6/setup.py
```

### Comparing `diamond-hpc-0.0.5/LICENSE` & `diamond-hpc-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `diamond-hpc-0.0.5/PKG-INFO` & `diamond-hpc-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diamond-hpc
-Version: 0.0.5
+Version: 0.0.6
 Summary: Diamond is a Python package for running tasks on HPC.
 Home-page: https://github.com/Diamond-Proj/Diamond
 Author: Haotian XIE, Gengcong YANG
 Author-email: hotinexie@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `diamond-hpc-0.0.5/README.md` & `diamond-hpc-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `diamond-hpc-0.0.5/diamond/container/container.py` & `diamond-hpc-0.0.6/diamond/container/container.py`

 * *Files identical despite different names*

### Comparing `diamond-hpc-0.0.5/diamond/container/custom_image_builder/image_builder.py` & `diamond-hpc-0.0.6/diamond/container/custom_image_builder/image_builder.py`

 * *Files identical despite different names*

### Comparing `diamond-hpc-0.0.5/diamond/diamond_client/diamond_client.py` & `diamond-hpc-0.0.6/diamond/diamond_client/diamond_client.py`

 * *Files identical despite different names*

### Comparing `diamond-hpc-0.0.5/diamond/diamond_client/templates/task_template` & `diamond-hpc-0.0.6/diamond/diamond_client/templates/task_template`

 * *Files identical despite different names*

### Comparing `diamond-hpc-0.0.5/diamond/wrapper/wrapper.py` & `diamond-hpc-0.0.6/diamond/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `diamond-hpc-0.0.5/diamond_hpc.egg-info/PKG-INFO` & `diamond-hpc-0.0.6/diamond_hpc.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diamond-hpc
-Version: 0.0.5
+Version: 0.0.6
 Summary: Diamond is a Python package for running tasks on HPC.
 Home-page: https://github.com/Diamond-Proj/Diamond
 Author: Haotian XIE, Gengcong YANG
 Author-email: hotinexie@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `diamond-hpc-0.0.5/diamond_hpc.egg-info/SOURCES.txt` & `diamond-hpc-0.0.6/diamond_hpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `diamond-hpc-0.0.5/setup.py` & `diamond-hpc-0.0.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="diamond-hpc",
-    version="0.0.5",
+    version="0.0.6",
     author="Haotian XIE, Gengcong YANG",
     author_email="hotinexie@gmail.com",
     description="Diamond is a Python package for running tasks on HPC.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Diamond-Proj/Diamond",
     packages=find_packages(),
@@ -16,17 +16,19 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         "click>=8.1.3",
-        "globus_compute_sdk>=2.20.0",
+        "globus_compute_sdk>=2.21.0",
+        "globus_sdk>=3.41.0",
         "Jinja2>=3.1.4",
         "Requests>=2.32.2",
+        "setuptools>=59.6.0",
     ],
     entry_points={
         'console_scripts': [
             'diamond-hpc=diamond.wrapper.wrapper:cli',
         ],
     },
     python_requires='>=3.8',
```

