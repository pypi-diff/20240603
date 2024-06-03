# Comparing `tmp/ros-cdk-paidswapi-1.0.24.tar.gz` & `tmp/ros-cdk-paidswapi-1.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-paidswapi-1.0.24.tar", last modified: Wed Apr 10 04:14:11 2024, max compression
+gzip compressed data, was "dist/ros-cdk-paidswapi-1.0.25.tar", last modified: Mon Jun  3 11:47:39 2024, max compression
```

## Comparing `ros-cdk-paidswapi-1.0.24.tar` & `ros-cdk-paidswapi-1.0.25.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:14:11.000000 ros-cdk-paidswapi-1.0.24/
--rw-r--r--   0 root         (0) root         (0)    10279 2024-04-10 04:14:11.000000 ros-cdk-paidswapi-1.0.24/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-10 04:14:11.000000 ros-cdk-paidswapi-1.0.24/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2024-04-10 04:14:11.000000 ros-cdk-paidswapi-1.0.24/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1316 2024-04-10 04:14:11.000000 ros-cdk-paidswapi-1.0.24/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      197 2024-04-10 04:14:11.000000 ros-cdk-paidswapi-1.0.24/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2024-04-10 04:14:11.000000 ros-cdk-paidswapi-1.0.24/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 04:14:11.000000 ros-cdk-paidswapi-1.0.24/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1952 2024-04-10 04:14:11.000000 ros-cdk-paidswapi-1.0.24/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:14:11.000000 ros-cdk-paidswapi-1.0.24/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:14:11.000000 ros-cdk-paidswapi-1.0.24/src/ros_cdk_paidswapi/
--rw-r--r--   0 root         (0) root         (0)    63322 2024-04-10 04:14:11.000000 ros-cdk-paidswapi-1.0.24/src/ros_cdk_paidswapi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:14:11.000000 ros-cdk-paidswapi-1.0.24/src/ros_cdk_paidswapi/_jsii/
--rw-r--r--   0 root         (0) root         (0)      431 2024-04-10 04:14:11.000000 ros-cdk-paidswapi-1.0.24/src/ros_cdk_paidswapi/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45008 2024-04-10 04:14:11.000000 ros-cdk-paidswapi-1.0.24/src/ros_cdk_paidswapi/_jsii/ros-cdk-paidswapi@1.0.24.jsii.tgz
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:14:11.000000 ros-cdk-paidswapi-1.0.24/src/ros_cdk_paidswapi/datasource/
--rw-r--r--   0 root         (0) root         (0)    25471 2024-04-10 04:14:11.000000 ros-cdk-paidswapi-1.0.24/src/ros_cdk_paidswapi/datasource/__init__.py
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 04:14:11.000000 ros-cdk-paidswapi-1.0.24/src/ros_cdk_paidswapi/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:14:11.000000 ros-cdk-paidswapi-1.0.24/src/ros_cdk_paidswapi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1316 2024-04-10 04:14:11.000000 ros-cdk-paidswapi-1.0.24/src/ros_cdk_paidswapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      506 2024-04-10 04:14:11.000000 ros-cdk-paidswapi-1.0.24/src/ros_cdk_paidswapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 04:14:11.000000 ros-cdk-paidswapi-1.0.24/src/ros_cdk_paidswapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      110 2024-04-10 04:14:11.000000 ros-cdk-paidswapi-1.0.24/src/ros_cdk_paidswapi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-04-10 04:14:11.000000 ros-cdk-paidswapi-1.0.24/src/ros_cdk_paidswapi.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:47:39.000000 ros-cdk-paidswapi-1.0.25/
+-rw-r--r--   0 root         (0) root         (0)    10279 2024-06-03 11:47:38.000000 ros-cdk-paidswapi-1.0.25/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2024-06-03 11:47:38.000000 ros-cdk-paidswapi-1.0.25/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2024-06-03 11:47:38.000000 ros-cdk-paidswapi-1.0.25/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1316 2024-06-03 11:47:39.000000 ros-cdk-paidswapi-1.0.25/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      197 2024-06-03 11:47:38.000000 ros-cdk-paidswapi-1.0.25/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2024-06-03 11:47:38.000000 ros-cdk-paidswapi-1.0.25/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-06-03 11:47:39.000000 ros-cdk-paidswapi-1.0.25/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1953 2024-06-03 11:47:38.000000 ros-cdk-paidswapi-1.0.25/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:47:39.000000 ros-cdk-paidswapi-1.0.25/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:47:39.000000 ros-cdk-paidswapi-1.0.25/src/ros_cdk_paidswapi/
+-rw-r--r--   0 root         (0) root         (0)    63322 2024-06-03 11:47:38.000000 ros-cdk-paidswapi-1.0.25/src/ros_cdk_paidswapi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:47:39.000000 ros-cdk-paidswapi-1.0.25/src/ros_cdk_paidswapi/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      431 2024-06-03 11:47:38.000000 ros-cdk-paidswapi-1.0.25/src/ros_cdk_paidswapi/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    47435 2024-06-03 11:47:38.000000 ros-cdk-paidswapi-1.0.25/src/ros_cdk_paidswapi/_jsii/ros-cdk-paidswapi@1.0.25.jsii.tgz
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:47:39.000000 ros-cdk-paidswapi-1.0.25/src/ros_cdk_paidswapi/datasource/
+-rw-r--r--   0 root         (0) root         (0)    25471 2024-06-03 11:47:38.000000 ros-cdk-paidswapi-1.0.25/src/ros_cdk_paidswapi/datasource/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 11:47:38.000000 ros-cdk-paidswapi-1.0.25/src/ros_cdk_paidswapi/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:47:39.000000 ros-cdk-paidswapi-1.0.25/src/ros_cdk_paidswapi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1316 2024-06-03 11:47:39.000000 ros-cdk-paidswapi-1.0.25/src/ros_cdk_paidswapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      506 2024-06-03 11:47:39.000000 ros-cdk-paidswapi-1.0.25/src/ros_cdk_paidswapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 11:47:39.000000 ros-cdk-paidswapi-1.0.25/src/ros_cdk_paidswapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      111 2024-06-03 11:47:39.000000 ros-cdk-paidswapi-1.0.25/src/ros_cdk_paidswapi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-06-03 11:47:39.000000 ros-cdk-paidswapi-1.0.25/src/ros_cdk_paidswapi.egg-info/top_level.txt
```

### Comparing `ros-cdk-paidswapi-1.0.24/LICENSE` & `ros-cdk-paidswapi-1.0.25/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-paidswapi-1.0.24/PKG-INFO` & `ros-cdk-paidswapi-1.0.25/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-paidswapi
-Version: 1.0.24
+Version: 1.0.25
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS PAIDSWAPI Construct Library
```

### Comparing `ros-cdk-paidswapi-1.0.24/setup.py` & `ros-cdk-paidswapi-1.0.25/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-paidswapi",
-    "version": "1.0.24",
+    "version": "1.0.25",
     "description": "Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com",
     "license": "Apache-2.0",
     "url": "https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git",
     "long_description_content_type": "text/markdown",
     "author": "ROS Development Team",
     "bdist_wheel": {
         "universal": true
@@ -23,26 +23,26 @@
     "packages": [
         "ros_cdk_paidswapi",
         "ros_cdk_paidswapi._jsii",
         "ros_cdk_paidswapi.datasource"
     ],
     "package_data": {
         "ros_cdk_paidswapi._jsii": [
-            "ros-cdk-paidswapi@1.0.24.jsii.tgz"
+            "ros-cdk-paidswapi@1.0.25.jsii.tgz"
         ],
         "ros_cdk_paidswapi": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "constructs>=3.0.4, <4.0.0",
         "jsii>1.12.0, <=1.85.0",
         "publication>=0.0.3",
-        "ros-cdk-core>=1.0.6, <2.0.0",
+        "ros-cdk-core>=1.0.27, <2.0.0",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
```

### Comparing `ros-cdk-paidswapi-1.0.24/src/ros_cdk_paidswapi/__init__.py` & `ros-cdk-paidswapi-1.0.25/src/ros_cdk_paidswapi/__init__.py`

 * *Files identical despite different names*

### Comparing `ros-cdk-paidswapi-1.0.24/src/ros_cdk_paidswapi/datasource/__init__.py` & `ros-cdk-paidswapi-1.0.25/src/ros_cdk_paidswapi/datasource/__init__.py`

 * *Files identical despite different names*

### Comparing `ros-cdk-paidswapi-1.0.24/src/ros_cdk_paidswapi.egg-info/PKG-INFO` & `ros-cdk-paidswapi-1.0.25/src/ros_cdk_paidswapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-paidswapi
-Version: 1.0.24
+Version: 1.0.25
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS PAIDSWAPI Construct Library
```

