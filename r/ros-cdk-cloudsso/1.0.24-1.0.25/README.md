# Comparing `tmp/ros-cdk-cloudsso-1.0.24.tar.gz` & `tmp/ros-cdk-cloudsso-1.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-cloudsso-1.0.24.tar", last modified: Wed Apr 10 03:49:28 2024, max compression
+gzip compressed data, was "dist/ros-cdk-cloudsso-1.0.25.tar", last modified: Mon Jun  3 10:10:12 2024, max compression
```

## Comparing `ros-cdk-cloudsso-1.0.24.tar` & `ros-cdk-cloudsso-1.0.25.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:49:28.000000 ros-cdk-cloudsso-1.0.24/
--rw-r--r--   0 root         (0) root         (0)    10279 2024-04-10 03:49:28.000000 ros-cdk-cloudsso-1.0.24/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-10 03:49:28.000000 ros-cdk-cloudsso-1.0.24/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2024-04-10 03:49:28.000000 ros-cdk-cloudsso-1.0.24/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1312 2024-04-10 03:49:28.000000 ros-cdk-cloudsso-1.0.24/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      194 2024-04-10 03:49:28.000000 ros-cdk-cloudsso-1.0.24/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2024-04-10 03:49:28.000000 ros-cdk-cloudsso-1.0.24/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 03:49:28.000000 ros-cdk-cloudsso-1.0.24/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1906 2024-04-10 03:49:28.000000 ros-cdk-cloudsso-1.0.24/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:49:28.000000 ros-cdk-cloudsso-1.0.24/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:49:28.000000 ros-cdk-cloudsso-1.0.24/src/ros_cdk_cloudsso/
--rw-r--r--   0 root         (0) root         (0)   328921 2024-04-10 03:49:28.000000 ros-cdk-cloudsso-1.0.24/src/ros_cdk_cloudsso/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:49:28.000000 ros-cdk-cloudsso-1.0.24/src/ros_cdk_cloudsso/_jsii/
--rw-r--r--   0 root         (0) root         (0)      429 2024-04-10 03:49:28.000000 ros-cdk-cloudsso-1.0.24/src/ros_cdk_cloudsso/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    83244 2024-04-10 03:49:28.000000 ros-cdk-cloudsso-1.0.24/src/ros_cdk_cloudsso/_jsii/ros-cdk-cloudsso@1.0.24.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 03:49:28.000000 ros-cdk-cloudsso-1.0.24/src/ros_cdk_cloudsso/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:49:28.000000 ros-cdk-cloudsso-1.0.24/src/ros_cdk_cloudsso.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1312 2024-04-10 03:49:28.000000 ros-cdk-cloudsso-1.0.24/src/ros_cdk_cloudsso.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      451 2024-04-10 03:49:28.000000 ros-cdk-cloudsso-1.0.24/src/ros_cdk_cloudsso.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 03:49:28.000000 ros-cdk-cloudsso-1.0.24/src/ros_cdk_cloudsso.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      110 2024-04-10 03:49:28.000000 ros-cdk-cloudsso-1.0.24/src/ros_cdk_cloudsso.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-04-10 03:49:28.000000 ros-cdk-cloudsso-1.0.24/src/ros_cdk_cloudsso.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 10:10:12.000000 ros-cdk-cloudsso-1.0.25/
+-rw-r--r--   0 root         (0) root         (0)    10279 2024-06-03 10:10:11.000000 ros-cdk-cloudsso-1.0.25/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2024-06-03 10:10:11.000000 ros-cdk-cloudsso-1.0.25/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2024-06-03 10:10:11.000000 ros-cdk-cloudsso-1.0.25/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1312 2024-06-03 10:10:12.000000 ros-cdk-cloudsso-1.0.25/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      194 2024-06-03 10:10:11.000000 ros-cdk-cloudsso-1.0.25/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2024-06-03 10:10:11.000000 ros-cdk-cloudsso-1.0.25/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-06-03 10:10:12.000000 ros-cdk-cloudsso-1.0.25/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1907 2024-06-03 10:10:11.000000 ros-cdk-cloudsso-1.0.25/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 10:10:12.000000 ros-cdk-cloudsso-1.0.25/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 10:10:12.000000 ros-cdk-cloudsso-1.0.25/src/ros_cdk_cloudsso/
+-rw-r--r--   0 root         (0) root         (0)   330681 2024-06-03 10:10:11.000000 ros-cdk-cloudsso-1.0.25/src/ros_cdk_cloudsso/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 10:10:12.000000 ros-cdk-cloudsso-1.0.25/src/ros_cdk_cloudsso/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      429 2024-06-03 10:10:11.000000 ros-cdk-cloudsso-1.0.25/src/ros_cdk_cloudsso/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    88179 2024-06-03 10:10:11.000000 ros-cdk-cloudsso-1.0.25/src/ros_cdk_cloudsso/_jsii/ros-cdk-cloudsso@1.0.25.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 10:10:11.000000 ros-cdk-cloudsso-1.0.25/src/ros_cdk_cloudsso/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 10:10:12.000000 ros-cdk-cloudsso-1.0.25/src/ros_cdk_cloudsso.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1312 2024-06-03 10:10:12.000000 ros-cdk-cloudsso-1.0.25/src/ros_cdk_cloudsso.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      451 2024-06-03 10:10:12.000000 ros-cdk-cloudsso-1.0.25/src/ros_cdk_cloudsso.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 10:10:12.000000 ros-cdk-cloudsso-1.0.25/src/ros_cdk_cloudsso.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      111 2024-06-03 10:10:12.000000 ros-cdk-cloudsso-1.0.25/src/ros_cdk_cloudsso.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-06-03 10:10:12.000000 ros-cdk-cloudsso-1.0.25/src/ros_cdk_cloudsso.egg-info/top_level.txt
```

### Comparing `ros-cdk-cloudsso-1.0.24/LICENSE` & `ros-cdk-cloudsso-1.0.25/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-cloudsso-1.0.24/PKG-INFO` & `ros-cdk-cloudsso-1.0.25/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-cloudsso
-Version: 1.0.24
+Version: 1.0.25
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS CLOUDSSO Construct Library
```

### Comparing `ros-cdk-cloudsso-1.0.24/setup.py` & `ros-cdk-cloudsso-1.0.25/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-cloudsso",
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
         "ros_cdk_cloudsso",
         "ros_cdk_cloudsso._jsii"
     ],
     "package_data": {
         "ros_cdk_cloudsso._jsii": [
-            "ros-cdk-cloudsso@1.0.24.jsii.tgz"
+            "ros-cdk-cloudsso@1.0.25.jsii.tgz"
         ],
         "ros_cdk_cloudsso": [
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

### Comparing `ros-cdk-cloudsso-1.0.24/src/ros_cdk_cloudsso/__init__.py` & `ros-cdk-cloudsso-1.0.25/src/ros_cdk_cloudsso/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 
 class AccessAssignment(
     _ros_cdk_core_7adfd82f.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-cloudsso.AccessAssignment",
 ):
-    '''This class encapsulates and extends the ROS resource type ``ALIYUN::CloudSSO::AccessAssignment``.
+    '''This class encapsulates and extends the ROS resource type ``ALIYUN::CloudSSO::AccessAssignment``, which is used to assign access permissions on an account in your resource directory to a user or group by using an access configuration.
 
     :Note:
 
     This class may have some new functions to facilitate development, so it is recommended to use this class instead of ``RosAccessAssignment``for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-cloudsso-accessassignment
     '''
 
@@ -236,15 +236,15 @@
 
 
 class AccessConfiguration(
     _ros_cdk_core_7adfd82f.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-cloudsso.AccessConfiguration",
 ):
-    '''This class encapsulates and extends the ROS resource type ``ALIYUN::CloudSSO::AccessConfiguration``.
+    '''This class encapsulates and extends the ROS resource type ``ALIYUN::CloudSSO::AccessConfiguration``, which is used to create an access configuration.
 
     :Note:
 
     This class may have some new functions to facilitate development, so it is recommended to use this class instead of ``RosAccessConfiguration``for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-cloudsso-accessconfiguration
     '''
 
@@ -444,15 +444,15 @@
 
 
 class AccessConfigurationProvision(
     _ros_cdk_core_7adfd82f.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-cloudsso.AccessConfigurationProvision",
 ):
-    '''This class encapsulates and extends the ROS resource type ``ALIYUN::CloudSSO::AccessConfigurationProvision``.
+    '''This class encapsulates and extends the ROS resource type ``ALIYUN::CloudSSO::AccessConfigurationProvision``, which is used to provision an access configuration for an account in your resource directory.
 
     :Note:
 
     This class may have some new functions to facilitate development, so it is recommended to use this class instead of ``RosAccessConfigurationProvision``for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-cloudsso-accessconfigurationprovision
     '''
 
@@ -620,15 +620,15 @@
 
 
 class Directory(
     _ros_cdk_core_7adfd82f.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-cloudsso.Directory",
 ):
-    '''This class encapsulates and extends the ROS resource type ``ALIYUN::CloudSSO::Directory``.
+    '''This class encapsulates and extends the ROS resource type ``ALIYUN::CloudSSO::Directory``, which is used to create a directory.
 
     :Note:
 
     This class may have some new functions to facilitate development, so it is recommended to use this class instead of ``RosDirectory``for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-cloudsso-directory
     '''
 
@@ -760,15 +760,15 @@
 
 
 class Group(
     _ros_cdk_core_7adfd82f.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-cloudsso.Group",
 ):
-    '''This class encapsulates and extends the ROS resource type ``ALIYUN::CloudSSO::Group``.
+    '''This class encapsulates and extends the ROS resource type ``ALIYUN::CloudSSO::Group``, which is used to create a group in CloudSSO.
 
     :Note:
 
     This class may have some new functions to facilitate development, so it is recommended to use this class instead of ``RosGroup``for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-cloudsso-group
     '''
 
@@ -932,15 +932,15 @@
 
 
 class PermissionPolicyToAccessConfigurationAddition(
     _ros_cdk_core_7adfd82f.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-cloudsso.PermissionPolicyToAccessConfigurationAddition",
 ):
-    '''This class encapsulates and extends the ROS resource type ``ALIYUN::CloudSSO::PermissionPolicyToAccessConfigurationAddition``.
+    '''This class encapsulates and extends the ROS resource type ``ALIYUN::CloudSSO::PermissionPolicyToAccessConfigurationAddition``, which is used to add a policy to an access configuration.
 
     :Note:
 
     This class may have some new functions to facilitate development, so it is recommended to use this class instead of ``RosPermissionPolicyToAccessConfigurationAddition``for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-cloudsso-permissionpolicytoaccessconfigurationaddition
     '''
 
@@ -1136,15 +1136,15 @@
 
 
 class RosAccessAssignment(
     _ros_cdk_core_7adfd82f.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-cloudsso.RosAccessAssignment",
 ):
-    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::CloudSSO::AccessAssignment``.
+    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::CloudSSO::AccessAssignment``, which is used to assign access permissions on an account in your resource directory to a user or group by using an access configuration.
 
     :Note:
 
     This class does not contain additional functions, so it is recommended to use the ``AccessAssignment`` class instead of this class for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-cloudsso-accessassignment
     '''
 
@@ -1466,15 +1466,15 @@
 
 
 class RosAccessConfiguration(
     _ros_cdk_core_7adfd82f.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-cloudsso.RosAccessConfiguration",
 ):
-    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::CloudSSO::AccessConfiguration``.
+    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::CloudSSO::AccessConfiguration``, which is used to create an access configuration.
 
     :Note:
 
     This class does not contain additional functions, so it is recommended to use the ``AccessConfiguration`` class instead of this class for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-cloudsso-accessconfiguration
     '''
 
@@ -1788,15 +1788,15 @@
 
 
 class RosAccessConfigurationProvision(
     _ros_cdk_core_7adfd82f.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-cloudsso.RosAccessConfigurationProvision",
 ):
-    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::CloudSSO::AccessConfigurationProvision``.
+    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::CloudSSO::AccessConfigurationProvision``, which is used to provision an access configuration for an account in your resource directory.
 
     :Note:
 
     This class does not contain additional functions, so it is recommended to use the ``AccessConfigurationProvision`` class instead of this class for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-cloudsso-accessconfigurationprovision
     '''
 
@@ -2036,15 +2036,15 @@
 
 
 class RosDirectory(
     _ros_cdk_core_7adfd82f.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-cloudsso.RosDirectory",
 ):
-    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::CloudSSO::Directory``.
+    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::CloudSSO::Directory``, which is used to create a directory.
 
     :Note:
 
     This class does not contain additional functions, so it is recommended to use the ``Directory`` class instead of this class for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-cloudsso-directory
     '''
 
@@ -2191,15 +2191,15 @@
 
 
 class RosGroup(
     _ros_cdk_core_7adfd82f.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-cloudsso.RosGroup",
 ):
-    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::CloudSSO::Group``.
+    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::CloudSSO::Group``, which is used to create a group in CloudSSO.
 
     :Note:
 
     This class does not contain additional functions, so it is recommended to use the ``Group`` class instead of this class for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-cloudsso-group
     '''
 
@@ -2425,15 +2425,15 @@
 
 
 class RosPermissionPolicyToAccessConfigurationAddition(
     _ros_cdk_core_7adfd82f.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-cloudsso.RosPermissionPolicyToAccessConfigurationAddition",
 ):
-    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::CloudSSO::PermissionPolicyToAccessConfigurationAddition``.
+    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::CloudSSO::PermissionPolicyToAccessConfigurationAddition``, which is used to add a policy to an access configuration.
 
     :Note:
 
     This class does not contain additional functions, so it is recommended to use the ``PermissionPolicyToAccessConfigurationAddition`` class instead of this class for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-cloudsso-permissionpolicytoaccessconfigurationaddition
     '''
 
@@ -2737,15 +2737,15 @@
 
 
 class RosSAMLIdentityProvider(
     _ros_cdk_core_7adfd82f.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-cloudsso.RosSAMLIdentityProvider",
 ):
-    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::CloudSSO::SAMLIdentityProvider``.
+    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::CloudSSO::SAMLIdentityProvider``, which is used to configure the information about a Security Assertion Markup Language (SAML) identity provider (IdP).
 
     :Note:
 
     This class does not contain additional functions, so it is recommended to use the ``SAMLIdentityProvider`` class instead of this class for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-cloudsso-samlidentityprovider
     '''
 
@@ -3119,15 +3119,15 @@
 
 
 class RosSCIMServerCredential(
     _ros_cdk_core_7adfd82f.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-cloudsso.RosSCIMServerCredential",
 ):
-    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::CloudSSO::SCIMServerCredential``.
+    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::CloudSSO::SCIMServerCredential``, which is used to create a System for Cross-domain Identity Management (SCIM) credential.
 
     :Note:
 
     This class does not contain additional functions, so it is recommended to use the ``SCIMServerCredential`` class instead of this class for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-cloudsso-scimservercredential
     '''
 
@@ -3320,15 +3320,15 @@
 
 
 class RosSCIMSynchronization(
     _ros_cdk_core_7adfd82f.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-cloudsso.RosSCIMSynchronization",
 ):
-    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::CloudSSO::SCIMSynchronization``.
+    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::CloudSSO::SCIMSynchronization``, which is used to enable or disable System for Cross-domain Identity Management (SCIM) synchronization.
 
     :Note:
 
     This class does not contain additional functions, so it is recommended to use the ``SCIMSynchronization`` class instead of this class for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-cloudsso-scimsynchronization
     '''
 
@@ -3508,15 +3508,15 @@
 
 
 class RosUser(
     _ros_cdk_core_7adfd82f.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-cloudsso.RosUser",
 ):
-    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::CloudSSO::User``.
+    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::CloudSSO::User``, which is used to create a user.
 
     :Note:
 
     This class does not contain additional functions, so it is recommended to use the ``User`` class instead of this class for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-cloudsso-user
     '''
 
@@ -3962,15 +3962,15 @@
 
 
 class RosUserProvision(
     _ros_cdk_core_7adfd82f.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-cloudsso.RosUserProvision",
 ):
-    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::CloudSSO::UserProvision``.
+    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::CloudSSO::UserProvision``, which is used to create a Resource Access Management (RAM) user provisioning.
 
     :Note:
 
     This class does not contain additional functions, so it is recommended to use the ``UserProvision`` class instead of this class for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-cloudsso-userprovision
     '''
 
@@ -4402,15 +4402,15 @@
 
 
 class RosUserToGroupAddition(
     _ros_cdk_core_7adfd82f.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-cloudsso.RosUserToGroupAddition",
 ):
-    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::CloudSSO::UserToGroupAddition``.
+    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::CloudSSO::UserToGroupAddition``, which is used to add a user to a group.
 
     :Note:
 
     This class does not contain additional functions, so it is recommended to use the ``UserToGroupAddition`` class instead of this class for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-cloudsso-usertogroupaddition
     '''
 
@@ -4610,15 +4610,15 @@
 
 
 class SAMLIdentityProvider(
     _ros_cdk_core_7adfd82f.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-cloudsso.SAMLIdentityProvider",
 ):
-    '''This class encapsulates and extends the ROS resource type ``ALIYUN::CloudSSO::SAMLIdentityProvider``.
+    '''This class encapsulates and extends the ROS resource type ``ALIYUN::CloudSSO::SAMLIdentityProvider``, which is used to configure the information about a Security Assertion Markup Language (SAML) identity provider (IdP).
 
     :Note:
 
     This class may have some new functions to facilitate development, so it is recommended to use this class instead of ``RosSAMLIdentityProvider``for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-cloudsso-samlidentityprovider
     '''
 
@@ -4841,15 +4841,15 @@
 
 
 class SCIMServerCredential(
     _ros_cdk_core_7adfd82f.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-cloudsso.SCIMServerCredential",
 ):
-    '''This class encapsulates and extends the ROS resource type ``ALIYUN::CloudSSO::SCIMServerCredential``.
+    '''This class encapsulates and extends the ROS resource type ``ALIYUN::CloudSSO::SCIMServerCredential``, which is used to create a System for Cross-domain Identity Management (SCIM) credential.
 
     :Note:
 
     This class may have some new functions to facilitate development, so it is recommended to use this class instead of ``RosSCIMServerCredential``for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-cloudsso-scimservercredential
     '''
 
@@ -5002,15 +5002,15 @@
 
 
 class SCIMSynchronization(
     _ros_cdk_core_7adfd82f.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-cloudsso.SCIMSynchronization",
 ):
-    '''This class encapsulates and extends the ROS resource type ``ALIYUN::CloudSSO::SCIMSynchronization``.
+    '''This class encapsulates and extends the ROS resource type ``ALIYUN::CloudSSO::SCIMSynchronization``, which is used to enable or disable System for Cross-domain Identity Management (SCIM) synchronization.
 
     :Note:
 
     This class may have some new functions to facilitate development, so it is recommended to use this class instead of ``RosSCIMSynchronization``for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-cloudsso-scimsynchronization
     '''
 
@@ -5154,15 +5154,15 @@
 
 
 class User(
     _ros_cdk_core_7adfd82f.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-cloudsso.User",
 ):
-    '''This class encapsulates and extends the ROS resource type ``ALIYUN::CloudSSO::User``.
+    '''This class encapsulates and extends the ROS resource type ``ALIYUN::CloudSSO::User``, which is used to create a user.
 
     :Note:
 
     This class may have some new functions to facilitate development, so it is recommended to use this class instead of ``RosUser``for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-cloudsso-user
     '''
 
@@ -5416,15 +5416,15 @@
 
 
 class UserProvision(
     _ros_cdk_core_7adfd82f.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-cloudsso.UserProvision",
 ):
-    '''This class encapsulates and extends the ROS resource type ``ALIYUN::CloudSSO::UserProvision``.
+    '''This class encapsulates and extends the ROS resource type ``ALIYUN::CloudSSO::UserProvision``, which is used to create a Resource Access Management (RAM) user provisioning.
 
     :Note:
 
     This class may have some new functions to facilitate development, so it is recommended to use this class instead of ``RosUserProvision``for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-cloudsso-userprovision
     '''
 
@@ -5681,15 +5681,15 @@
 
 
 class UserToGroupAddition(
     _ros_cdk_core_7adfd82f.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-cloudsso.UserToGroupAddition",
 ):
-    '''This class encapsulates and extends the ROS resource type ``ALIYUN::CloudSSO::UserToGroupAddition``.
+    '''This class encapsulates and extends the ROS resource type ``ALIYUN::CloudSSO::UserToGroupAddition``, which is used to add a user to a group.
 
     :Note:
 
     This class may have some new functions to facilitate development, so it is recommended to use this class instead of ``RosUserToGroupAddition``for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-cloudsso-usertogroupaddition
     '''
```

### Comparing `ros-cdk-cloudsso-1.0.24/src/ros_cdk_cloudsso.egg-info/PKG-INFO` & `ros-cdk-cloudsso-1.0.25/src/ros_cdk_cloudsso.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-cloudsso
-Version: 1.0.24
+Version: 1.0.25
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS CLOUDSSO Construct Library
```

