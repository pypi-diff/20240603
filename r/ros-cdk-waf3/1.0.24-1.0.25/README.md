# Comparing `tmp/ros-cdk-waf3-1.0.24.tar.gz` & `tmp/ros-cdk-waf3-1.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-waf3-1.0.24.tar", last modified: Wed Apr 10 02:42:35 2024, max compression
+gzip compressed data, was "dist/ros-cdk-waf3-1.0.25.tar", last modified: Mon Jun  3 10:17:45 2024, max compression
```

## Comparing `ros-cdk-waf3-1.0.24.tar` & `ros-cdk-waf3-1.0.25.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 02:42:35.000000 ros-cdk-waf3-1.0.24/
--rw-r--r--   0 root         (0) root         (0)    10279 2024-04-10 02:42:35.000000 ros-cdk-waf3-1.0.24/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-10 02:42:35.000000 ros-cdk-waf3-1.0.24/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2024-04-10 02:42:35.000000 ros-cdk-waf3-1.0.24/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1296 2024-04-10 02:42:35.000000 ros-cdk-waf3-1.0.24/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      182 2024-04-10 02:42:35.000000 ros-cdk-waf3-1.0.24/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2024-04-10 02:42:35.000000 ros-cdk-waf3-1.0.24/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 02:42:35.000000 ros-cdk-waf3-1.0.24/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1882 2024-04-10 02:42:35.000000 ros-cdk-waf3-1.0.24/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 02:42:35.000000 ros-cdk-waf3-1.0.24/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 02:42:35.000000 ros-cdk-waf3-1.0.24/src/ros_cdk_waf3/
--rw-r--r--   0 root         (0) root         (0)    89634 2024-04-10 02:42:35.000000 ros-cdk-waf3-1.0.24/src/ros_cdk_waf3/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 02:42:35.000000 ros-cdk-waf3-1.0.24/src/ros_cdk_waf3/_jsii/
--rw-r--r--   0 root         (0) root         (0)      408 2024-04-10 02:42:35.000000 ros-cdk-waf3-1.0.24/src/ros_cdk_waf3/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    47288 2024-04-10 02:42:35.000000 ros-cdk-waf3-1.0.24/src/ros_cdk_waf3/_jsii/ros-cdk-waf3@1.0.24.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 02:42:35.000000 ros-cdk-waf3-1.0.24/src/ros_cdk_waf3/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 02:42:35.000000 ros-cdk-waf3-1.0.24/src/ros_cdk_waf3.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1296 2024-04-10 02:42:35.000000 ros-cdk-waf3-1.0.24/src/ros_cdk_waf3.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      411 2024-04-10 02:42:35.000000 ros-cdk-waf3-1.0.24/src/ros_cdk_waf3.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 02:42:35.000000 ros-cdk-waf3-1.0.24/src/ros_cdk_waf3.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      110 2024-04-10 02:42:35.000000 ros-cdk-waf3-1.0.24/src/ros_cdk_waf3.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-10 02:42:35.000000 ros-cdk-waf3-1.0.24/src/ros_cdk_waf3.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 10:17:45.000000 ros-cdk-waf3-1.0.25/
+-rw-r--r--   0 root         (0) root         (0)    10279 2024-06-03 10:17:45.000000 ros-cdk-waf3-1.0.25/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2024-06-03 10:17:45.000000 ros-cdk-waf3-1.0.25/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2024-06-03 10:17:45.000000 ros-cdk-waf3-1.0.25/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1296 2024-06-03 10:17:45.000000 ros-cdk-waf3-1.0.25/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      182 2024-06-03 10:17:45.000000 ros-cdk-waf3-1.0.25/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2024-06-03 10:17:45.000000 ros-cdk-waf3-1.0.25/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-06-03 10:17:45.000000 ros-cdk-waf3-1.0.25/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1883 2024-06-03 10:17:45.000000 ros-cdk-waf3-1.0.25/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 10:17:45.000000 ros-cdk-waf3-1.0.25/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 10:17:45.000000 ros-cdk-waf3-1.0.25/src/ros_cdk_waf3/
+-rw-r--r--   0 root         (0) root         (0)    89776 2024-06-03 10:17:45.000000 ros-cdk-waf3-1.0.25/src/ros_cdk_waf3/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 10:17:45.000000 ros-cdk-waf3-1.0.25/src/ros_cdk_waf3/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      408 2024-06-03 10:17:45.000000 ros-cdk-waf3-1.0.25/src/ros_cdk_waf3/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51346 2024-06-03 10:17:45.000000 ros-cdk-waf3-1.0.25/src/ros_cdk_waf3/_jsii/ros-cdk-waf3@1.0.25.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 10:17:45.000000 ros-cdk-waf3-1.0.25/src/ros_cdk_waf3/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 10:17:45.000000 ros-cdk-waf3-1.0.25/src/ros_cdk_waf3.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1296 2024-06-03 10:17:45.000000 ros-cdk-waf3-1.0.25/src/ros_cdk_waf3.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      411 2024-06-03 10:17:45.000000 ros-cdk-waf3-1.0.25/src/ros_cdk_waf3.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 10:17:45.000000 ros-cdk-waf3-1.0.25/src/ros_cdk_waf3.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      111 2024-06-03 10:17:45.000000 ros-cdk-waf3-1.0.25/src/ros_cdk_waf3.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-06-03 10:17:45.000000 ros-cdk-waf3-1.0.25/src/ros_cdk_waf3.egg-info/top_level.txt
```

### Comparing `ros-cdk-waf3-1.0.24/LICENSE` & `ros-cdk-waf3-1.0.25/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-waf3-1.0.24/PKG-INFO` & `ros-cdk-waf3-1.0.25/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-waf3
-Version: 1.0.24
+Version: 1.0.25
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS WAF3 Construct Library
```

### Comparing `ros-cdk-waf3-1.0.24/setup.py` & `ros-cdk-waf3-1.0.25/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-waf3",
-    "version": "1.0.24",
+    "version": "1.0.25",
     "description": "Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com",
     "license": "Apache-2.0",
     "url": "https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git",
     "long_description_content_type": "text/markdown",
     "author": "ROS Development Team",
     "bdist_wheel": {
         "universal": true
@@ -22,26 +22,26 @@
     },
     "packages": [
         "ros_cdk_waf3",
         "ros_cdk_waf3._jsii"
     ],
     "package_data": {
         "ros_cdk_waf3._jsii": [
-            "ros-cdk-waf3@1.0.24.jsii.tgz"
+            "ros-cdk-waf3@1.0.25.jsii.tgz"
         ],
         "ros_cdk_waf3": [
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

### Comparing `ros-cdk-waf3-1.0.24/src/ros_cdk_waf3/__init__.py` & `ros-cdk-waf3-1.0.25/src/ros_cdk_waf3/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 
 class Instance(
     _ros_cdk_core_7adfd82f.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-waf3.Instance",
 ):
-    '''This class encapsulates and extends the ROS resource type ``ALIYUN::WAF3::Instance``.
+    '''This class encapsulates and extends the ROS resource type ``ALIYUN::WAF3::Instance``, which is used to create a Web Application Firewall (WAF) 3.0 instance.
 
     :Note:
 
     This class may have some new functions to facilitate development, so it is recommended to use this class instead of ``RosInstance``for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-waf3-instance
     '''
 
@@ -466,15 +466,15 @@
 
 
 class RosInstance(
     _ros_cdk_core_7adfd82f.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-waf3.RosInstance",
 ):
-    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::WAF3::Instance``.
+    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::WAF3::Instance``, which is used to create a Web Application Firewall (WAF) 3.0 instance.
 
     :Note:
 
     This class does not contain additional functions, so it is recommended to use the ``Instance`` class instead of this class for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-waf3-instance
     '''
```

### Comparing `ros-cdk-waf3-1.0.24/src/ros_cdk_waf3.egg-info/PKG-INFO` & `ros-cdk-waf3-1.0.25/src/ros_cdk_waf3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-waf3
-Version: 1.0.24
+Version: 1.0.25
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS WAF3 Construct Library
```

