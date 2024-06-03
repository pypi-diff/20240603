# Comparing `tmp/cdk-cloudformation-spot-elastigroup-group-1.0.3a7.tar.gz` & `tmp/cdk-cloudformation-spot-elastigroup-group-1.0.4a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/__w/cdk-cloudformation/cdk-cloudformation/packages/@cdk-cloudformation/spot-elastigroup-group/dist/python/cdk-cloudformation-s", last modified: Fri Feb  3 17:32:41 2023, max compression
+gzip compressed data, was "cdk-cloudformation-spot-elastigroup-group-1.0.4a7.tar", last modified: Mon Jun  3 06:28:49 2024, max compression
```

## Comparing `cdk-cloudformation-spot-elastigroup-group-1.0.3a7.tar` & `cdk-cloudformation-spot-elastigroup-group-1.0.4a7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-03 17:32:41.000000 cdk-cloudformation-spot-elastigroup-group-1.0.3a7/
--rw-r--r--   0 superchain  (1001) superchain  (1001)    11358 2023-02-03 17:32:34.000000 cdk-cloudformation-spot-elastigroup-group-1.0.3a7/LICENSE
--rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2023-02-03 17:32:34.000000 cdk-cloudformation-spot-elastigroup-group-1.0.3a7/MANIFEST.in
--rw-r--r--   0 superchain  (1001) superchain  (1001)     2865 2023-02-03 17:32:41.000000 cdk-cloudformation-spot-elastigroup-group-1.0.3a7/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)     1900 2023-02-03 17:32:34.000000 cdk-cloudformation-spot-elastigroup-group-1.0.3a7/README.md
--rw-r--r--   0 superchain  (1001) superchain  (1001)      236 2023-02-03 17:32:34.000000 cdk-cloudformation-spot-elastigroup-group-1.0.3a7/pyproject.toml
--rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2023-02-03 17:32:41.000000 cdk-cloudformation-spot-elastigroup-group-1.0.3a7/setup.cfg
--rw-r--r--   0 superchain  (1001) superchain  (1001)     1917 2023-02-03 17:32:34.000000 cdk-cloudformation-spot-elastigroup-group-1.0.3a7/setup.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-03 17:32:41.000000 cdk-cloudformation-spot-elastigroup-group-1.0.3a7/src/
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-03 17:32:41.000000 cdk-cloudformation-spot-elastigroup-group-1.0.3a7/src/cdk_cloudformation_spot_elastigroup_group/
--rw-r--r--   0 superchain  (1001) superchain  (1001)   139225 2023-02-03 17:32:34.000000 cdk-cloudformation-spot-elastigroup-group-1.0.3a7/src/cdk_cloudformation_spot_elastigroup_group/__init__.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-03 17:32:41.000000 cdk-cloudformation-spot-elastigroup-group-1.0.3a7/src/cdk_cloudformation_spot_elastigroup_group/_jsii/
--rw-r--r--   0 superchain  (1001) superchain  (1001)      460 2023-02-03 17:32:34.000000 cdk-cloudformation-spot-elastigroup-group-1.0.3a7/src/cdk_cloudformation_spot_elastigroup_group/_jsii/__init__.py
--rw-r--r--   0 superchain  (1001) superchain  (1001)    36839 2023-02-03 17:32:34.000000 cdk-cloudformation-spot-elastigroup-group-1.0.3a7/src/cdk_cloudformation_spot_elastigroup_group/_jsii/spot-elastigroup-group@1.0.3-alpha.7.jsii.tgz
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-02-03 17:32:34.000000 cdk-cloudformation-spot-elastigroup-group-1.0.3a7/src/cdk_cloudformation_spot_elastigroup_group/py.typed
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-03 17:32:41.000000 cdk-cloudformation-spot-elastigroup-group-1.0.3a7/src/cdk_cloudformation_spot_elastigroup_group.egg-info/
--rw-r--r--   0 superchain  (1001) superchain  (1001)     2865 2023-02-03 17:32:40.000000 cdk-cloudformation-spot-elastigroup-group-1.0.3a7/src/cdk_cloudformation_spot_elastigroup_group.egg-info/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)      672 2023-02-03 17:32:41.000000 cdk-cloudformation-spot-elastigroup-group-1.0.3a7/src/cdk_cloudformation_spot_elastigroup_group.egg-info/SOURCES.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-02-03 17:32:40.000000 cdk-cloudformation-spot-elastigroup-group-1.0.3a7/src/cdk_cloudformation_spot_elastigroup_group.egg-info/dependency_links.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)      113 2023-02-03 17:32:41.000000 cdk-cloudformation-spot-elastigroup-group-1.0.3a7/src/cdk_cloudformation_spot_elastigroup_group.egg-info/requires.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)       42 2023-02-03 17:32:41.000000 cdk-cloudformation-spot-elastigroup-group-1.0.3a7/src/cdk_cloudformation_spot_elastigroup_group.egg-info/top_level.txt
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2024-06-03 06:28:49.480059 cdk-cloudformation-spot-elastigroup-group-1.0.4a7/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    11358 2024-06-03 06:28:37.000000 cdk-cloudformation-spot-elastigroup-group-1.0.4a7/LICENSE
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2024-06-03 06:28:37.000000 cdk-cloudformation-spot-elastigroup-group-1.0.4a7/MANIFEST.in
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     2846 2024-06-03 06:28:49.480059 cdk-cloudformation-spot-elastigroup-group-1.0.4a7/PKG-INFO
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     1900 2024-06-03 06:28:37.000000 cdk-cloudformation-spot-elastigroup-group-1.0.4a7/README.md
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      234 2024-06-03 06:28:37.000000 cdk-cloudformation-spot-elastigroup-group-1.0.4a7/pyproject.toml
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2024-06-03 06:28:49.480059 cdk-cloudformation-spot-elastigroup-group-1.0.4a7/setup.cfg
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     1917 2024-06-03 06:28:37.000000 cdk-cloudformation-spot-elastigroup-group-1.0.4a7/setup.py
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2024-06-03 06:28:49.472059 cdk-cloudformation-spot-elastigroup-group-1.0.4a7/src/
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2024-06-03 06:28:49.476059 cdk-cloudformation-spot-elastigroup-group-1.0.4a7/src/cdk_cloudformation_spot_elastigroup_group/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)   439693 2024-06-03 06:28:37.000000 cdk-cloudformation-spot-elastigroup-group-1.0.4a7/src/cdk_cloudformation_spot_elastigroup_group/__init__.py
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2024-06-03 06:28:49.480059 cdk-cloudformation-spot-elastigroup-group-1.0.4a7/src/cdk_cloudformation_spot_elastigroup_group/_jsii/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      536 2024-06-03 06:28:37.000000 cdk-cloudformation-spot-elastigroup-group-1.0.4a7/src/cdk_cloudformation_spot_elastigroup_group/_jsii/__init__.py
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    72093 2024-06-03 06:28:37.000000 cdk-cloudformation-spot-elastigroup-group-1.0.4a7/src/cdk_cloudformation_spot_elastigroup_group/_jsii/spot-elastigroup-group@1.0.4-alpha.7.jsii.tgz
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2024-06-03 06:28:37.000000 cdk-cloudformation-spot-elastigroup-group-1.0.4a7/src/cdk_cloudformation_spot_elastigroup_group/py.typed
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2024-06-03 06:28:49.476059 cdk-cloudformation-spot-elastigroup-group-1.0.4a7/src/cdk_cloudformation_spot_elastigroup_group.egg-info/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     2846 2024-06-03 06:28:49.000000 cdk-cloudformation-spot-elastigroup-group-1.0.4a7/src/cdk_cloudformation_spot_elastigroup_group.egg-info/PKG-INFO
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      672 2024-06-03 06:28:49.000000 cdk-cloudformation-spot-elastigroup-group-1.0.4a7/src/cdk_cloudformation_spot_elastigroup_group.egg-info/SOURCES.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2024-06-03 06:28:49.000000 cdk-cloudformation-spot-elastigroup-group-1.0.4a7/src/cdk_cloudformation_spot_elastigroup_group.egg-info/dependency_links.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      112 2024-06-03 06:28:49.000000 cdk-cloudformation-spot-elastigroup-group-1.0.4a7/src/cdk_cloudformation_spot_elastigroup_group.egg-info/requires.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       42 2024-06-03 06:28:49.000000 cdk-cloudformation-spot-elastigroup-group-1.0.4a7/src/cdk_cloudformation_spot_elastigroup_group.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cdk-cloudformation-spot-elastigroup-group-1.0.3a7/LICENSE` & `cdk-cloudformation-spot-elastigroup-group-1.0.4a7/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-cloudformation-spot-elastigroup-group-1.0.3a7/PKG-INFO` & `cdk-cloudformation-spot-elastigroup-group-1.0.4a7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: cdk-cloudformation-spot-elastigroup-group
-Version: 1.0.3a7
+Version: 1.0.4a7
 Summary: The Spot Elastigroup Resource allows you to create, update, manage, and delete Spot Elastigroups easily with CloudFormation
 Home-page: https://github.com/cdklabs/cdk-cloudformation.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-cloudformation.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: License :: OSI Approved
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # spot-elastigroup-group
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Spot::Elastigroup::Group` v1.0.3.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Spot::Elastigroup::Group` v1.0.4.
 
 ## Description
 
 The Spot Elastigroup Resource allows you to create, update, manage, and delete Spot Elastigroups easily with CloudFormation
 
 ## Usage
 
@@ -51,15 +50,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `Spot::Elastigroup::Group`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fspot-elastigroup-group+v1.0.3).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fspot-elastigroup-group+v1.0.4).
 * Issues related to `Spot::Elastigroup::Group` should be reported to the [publisher](undefined).
 
 ## License
 
 Distributed under the Apache-2.0 License.
-
-
```

### Comparing `cdk-cloudformation-spot-elastigroup-group-1.0.3a7/README.md` & `cdk-cloudformation-spot-elastigroup-group-1.0.4a7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # spot-elastigroup-group
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Spot::Elastigroup::Group` v1.0.3.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Spot::Elastigroup::Group` v1.0.4.
 
 ## Description
 
 The Spot Elastigroup Resource allows you to create, update, manage, and delete Spot Elastigroups easily with CloudFormation
 
 ## Usage
 
@@ -28,13 +28,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `Spot::Elastigroup::Group`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fspot-elastigroup-group+v1.0.3).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fspot-elastigroup-group+v1.0.4).
 * Issues related to `Spot::Elastigroup::Group` should be reported to the [publisher](undefined).
 
 ## License
 
 Distributed under the Apache-2.0 License.
```

### Comparing `cdk-cloudformation-spot-elastigroup-group-1.0.3a7/setup.py` & `cdk-cloudformation-spot-elastigroup-group-1.0.4a7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-cloudformation-spot-elastigroup-group",
-    "version": "1.0.3.a7",
+    "version": "1.0.4.a7",
     "description": "The Spot Elastigroup Resource allows you to create, update, manage, and delete Spot Elastigroups easily with CloudFormation",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/cdk-cloudformation.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,37 +22,37 @@
     },
     "packages": [
         "cdk_cloudformation_spot_elastigroup_group",
         "cdk_cloudformation_spot_elastigroup_group._jsii"
     ],
     "package_data": {
         "cdk_cloudformation_spot_elastigroup_group._jsii": [
-            "spot-elastigroup-group@1.0.3-alpha.7.jsii.tgz"
+            "spot-elastigroup-group@1.0.4-alpha.7.jsii.tgz"
         ],
         "cdk_cloudformation_spot_elastigroup_group": [
             "py.typed"
         ]
     },
-    "python_requires": "~=3.7",
+    "python_requires": "~=3.8",
     "install_requires": [
-        "aws-cdk-lib>=2.63.0, <3.0.0",
-        "constructs>=10.1.239, <11.0.0",
-        "jsii>=1.74.0, <2.0.0",
+        "aws-cdk-lib>=2.144.0, <3.0.0",
+        "constructs>=10.3.0, <11.0.0",
+        "jsii>=1.98.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "License :: OSI Approved"
     ],
     "scripts": []
 }
 """
 )
```

### Comparing `cdk-cloudformation-spot-elastigroup-group-1.0.3a7/src/cdk_cloudformation_spot_elastigroup_group.egg-info/PKG-INFO` & `cdk-cloudformation-spot-elastigroup-group-1.0.4a7/src/cdk_cloudformation_spot_elastigroup_group.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: cdk-cloudformation-spot-elastigroup-group
-Version: 1.0.3a7
+Version: 1.0.4a7
 Summary: The Spot Elastigroup Resource allows you to create, update, manage, and delete Spot Elastigroups easily with CloudFormation
 Home-page: https://github.com/cdklabs/cdk-cloudformation.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-cloudformation.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: License :: OSI Approved
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # spot-elastigroup-group
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Spot::Elastigroup::Group` v1.0.3.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Spot::Elastigroup::Group` v1.0.4.
 
 ## Description
 
 The Spot Elastigroup Resource allows you to create, update, manage, and delete Spot Elastigroups easily with CloudFormation
 
 ## Usage
 
@@ -51,15 +50,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `Spot::Elastigroup::Group`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fspot-elastigroup-group+v1.0.3).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fspot-elastigroup-group+v1.0.4).
 * Issues related to `Spot::Elastigroup::Group` should be reported to the [publisher](undefined).
 
 ## License
 
 Distributed under the Apache-2.0 License.
-
-
```

### Comparing `cdk-cloudformation-spot-elastigroup-group-1.0.3a7/src/cdk_cloudformation_spot_elastigroup_group.egg-info/SOURCES.txt` & `cdk-cloudformation-spot-elastigroup-group-1.0.4a7/src/cdk_cloudformation_spot_elastigroup_group.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cdk_cloudformation_spot_elastigroup_group/py.typed
 src/cdk_cloudformation_spot_elastigroup_group.egg-info/PKG-INFO
 src/cdk_cloudformation_spot_elastigroup_group.egg-info/SOURCES.txt
 src/cdk_cloudformation_spot_elastigroup_group.egg-info/dependency_links.txt
 src/cdk_cloudformation_spot_elastigroup_group.egg-info/requires.txt
 src/cdk_cloudformation_spot_elastigroup_group.egg-info/top_level.txt
 src/cdk_cloudformation_spot_elastigroup_group/_jsii/__init__.py
-src/cdk_cloudformation_spot_elastigroup_group/_jsii/spot-elastigroup-group@1.0.3-alpha.7.jsii.tgz
+src/cdk_cloudformation_spot_elastigroup_group/_jsii/spot-elastigroup-group@1.0.4-alpha.7.jsii.tgz
```

