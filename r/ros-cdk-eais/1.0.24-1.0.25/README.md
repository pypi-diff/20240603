# Comparing `tmp/ros-cdk-eais-1.0.24.tar.gz` & `tmp/ros-cdk-eais-1.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-eais-1.0.24.tar", last modified: Wed Apr 10 04:16:33 2024, max compression
+gzip compressed data, was "dist/ros-cdk-eais-1.0.25.tar", last modified: Mon Jun  3 11:54:52 2024, max compression
```

## Comparing `ros-cdk-eais-1.0.24.tar` & `ros-cdk-eais-1.0.25.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:16:33.000000 ros-cdk-eais-1.0.24/
--rw-r--r--   0 root         (0) root         (0)    10279 2024-04-10 04:16:33.000000 ros-cdk-eais-1.0.24/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-10 04:16:33.000000 ros-cdk-eais-1.0.24/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2024-04-10 04:16:33.000000 ros-cdk-eais-1.0.24/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1296 2024-04-10 04:16:33.000000 ros-cdk-eais-1.0.24/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      182 2024-04-10 04:16:33.000000 ros-cdk-eais-1.0.24/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2024-04-10 04:16:33.000000 ros-cdk-eais-1.0.24/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 04:16:33.000000 ros-cdk-eais-1.0.24/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1917 2024-04-10 04:16:33.000000 ros-cdk-eais-1.0.24/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:16:33.000000 ros-cdk-eais-1.0.24/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:16:33.000000 ros-cdk-eais-1.0.24/src/ros_cdk_eais/
--rw-r--r--   0 root         (0) root         (0)    68951 2024-04-10 04:16:33.000000 ros-cdk-eais-1.0.24/src/ros_cdk_eais/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:16:33.000000 ros-cdk-eais-1.0.24/src/ros_cdk_eais/_jsii/
--rw-r--r--   0 root         (0) root         (0)      408 2024-04-10 04:16:33.000000 ros-cdk-eais-1.0.24/src/ros_cdk_eais/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    49123 2024-04-10 04:16:33.000000 ros-cdk-eais-1.0.24/src/ros_cdk_eais/_jsii/ros-cdk-eais@1.0.24.jsii.tgz
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:16:33.000000 ros-cdk-eais-1.0.24/src/ros_cdk_eais/datasource/
--rw-r--r--   0 root         (0) root         (0)    48031 2024-04-10 04:16:33.000000 ros-cdk-eais-1.0.24/src/ros_cdk_eais/datasource/__init__.py
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 04:16:33.000000 ros-cdk-eais-1.0.24/src/ros_cdk_eais/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:16:33.000000 ros-cdk-eais-1.0.24/src/ros_cdk_eais.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1296 2024-04-10 04:16:33.000000 ros-cdk-eais-1.0.24/src/ros_cdk_eais.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      451 2024-04-10 04:16:33.000000 ros-cdk-eais-1.0.24/src/ros_cdk_eais.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 04:16:33.000000 ros-cdk-eais-1.0.24/src/ros_cdk_eais.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      110 2024-04-10 04:16:33.000000 ros-cdk-eais-1.0.24/src/ros_cdk_eais.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-10 04:16:33.000000 ros-cdk-eais-1.0.24/src/ros_cdk_eais.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:54:52.000000 ros-cdk-eais-1.0.25/
+-rw-r--r--   0 root         (0) root         (0)    10279 2024-06-03 11:54:52.000000 ros-cdk-eais-1.0.25/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2024-06-03 11:54:52.000000 ros-cdk-eais-1.0.25/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2024-06-03 11:54:52.000000 ros-cdk-eais-1.0.25/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1296 2024-06-03 11:54:52.000000 ros-cdk-eais-1.0.25/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      182 2024-06-03 11:54:52.000000 ros-cdk-eais-1.0.25/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2024-06-03 11:54:52.000000 ros-cdk-eais-1.0.25/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-06-03 11:54:52.000000 ros-cdk-eais-1.0.25/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1918 2024-06-03 11:54:52.000000 ros-cdk-eais-1.0.25/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:54:52.000000 ros-cdk-eais-1.0.25/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:54:52.000000 ros-cdk-eais-1.0.25/src/ros_cdk_eais/
+-rw-r--r--   0 root         (0) root         (0)    68951 2024-06-03 11:54:52.000000 ros-cdk-eais-1.0.25/src/ros_cdk_eais/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:54:52.000000 ros-cdk-eais-1.0.25/src/ros_cdk_eais/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      408 2024-06-03 11:54:52.000000 ros-cdk-eais-1.0.25/src/ros_cdk_eais/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51372 2024-06-03 11:54:52.000000 ros-cdk-eais-1.0.25/src/ros_cdk_eais/_jsii/ros-cdk-eais@1.0.25.jsii.tgz
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:54:52.000000 ros-cdk-eais-1.0.25/src/ros_cdk_eais/datasource/
+-rw-r--r--   0 root         (0) root         (0)    48255 2024-06-03 11:54:52.000000 ros-cdk-eais-1.0.25/src/ros_cdk_eais/datasource/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 11:54:52.000000 ros-cdk-eais-1.0.25/src/ros_cdk_eais/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:54:52.000000 ros-cdk-eais-1.0.25/src/ros_cdk_eais.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1296 2024-06-03 11:54:52.000000 ros-cdk-eais-1.0.25/src/ros_cdk_eais.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      451 2024-06-03 11:54:52.000000 ros-cdk-eais-1.0.25/src/ros_cdk_eais.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 11:54:52.000000 ros-cdk-eais-1.0.25/src/ros_cdk_eais.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      111 2024-06-03 11:54:52.000000 ros-cdk-eais-1.0.25/src/ros_cdk_eais.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-06-03 11:54:52.000000 ros-cdk-eais-1.0.25/src/ros_cdk_eais.egg-info/top_level.txt
```

### Comparing `ros-cdk-eais-1.0.24/LICENSE` & `ros-cdk-eais-1.0.25/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-eais-1.0.24/PKG-INFO` & `ros-cdk-eais-1.0.25/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-eais
-Version: 1.0.24
+Version: 1.0.25
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS EAIS Construct Library
```

### Comparing `ros-cdk-eais-1.0.24/setup.py` & `ros-cdk-eais-1.0.25/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-eais",
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
         "ros_cdk_eais",
         "ros_cdk_eais._jsii",
         "ros_cdk_eais.datasource"
     ],
     "package_data": {
         "ros_cdk_eais._jsii": [
-            "ros-cdk-eais@1.0.24.jsii.tgz"
+            "ros-cdk-eais@1.0.25.jsii.tgz"
         ],
         "ros_cdk_eais": [
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

### Comparing `ros-cdk-eais-1.0.24/src/ros_cdk_eais/__init__.py` & `ros-cdk-eais-1.0.25/src/ros_cdk_eais/__init__.py`

 * *Files identical despite different names*

### Comparing `ros-cdk-eais-1.0.24/src/ros_cdk_eais/datasource/__init__.py` & `ros-cdk-eais-1.0.25/src/ros_cdk_eais/datasource/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 class Instance(
     _ros_cdk_core_7adfd82f.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-eais.datasource.Instance",
 ):
-    '''This class encapsulates and extends the ROS resource type ``DATASOURCE::EAIS::Instance``.
+    '''This class encapsulates and extends the ROS resource type ``DATASOURCE::EAIS::Instance``, which is used to query the information about a created Elastic Accelerated Computing Instances (EAIS) instance.
 
     :Note:
 
     This class may have some new functions to facilitate development, so it is recommended to use this class instead of ``RosInstance``for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/datasource-eais-instance
     '''
 
@@ -401,15 +401,15 @@
 
 
 class RosInstance(
     _ros_cdk_core_7adfd82f.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-eais.datasource.RosInstance",
 ):
-    '''This class is a base encapsulation around the ROS resource type ``DATASOURCE::EAIS::Instance``.
+    '''This class is a base encapsulation around the ROS resource type ``DATASOURCE::EAIS::Instance``, which is used to query the information about a created Elastic Accelerated Computing Instances (EAIS) instance.
 
     :Note:
 
     This class does not contain additional functions, so it is recommended to use the ``Instance`` class instead of this class for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/datasource-eais-instance
     '''
```

### Comparing `ros-cdk-eais-1.0.24/src/ros_cdk_eais.egg-info/PKG-INFO` & `ros-cdk-eais-1.0.25/src/ros_cdk_eais.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-eais
-Version: 1.0.24
+Version: 1.0.25
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS EAIS Construct Library
```

