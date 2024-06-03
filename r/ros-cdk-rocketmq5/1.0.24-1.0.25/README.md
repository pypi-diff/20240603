# Comparing `tmp/ros-cdk-rocketmq5-1.0.24.tar.gz` & `tmp/ros-cdk-rocketmq5-1.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-rocketmq5-1.0.24.tar", last modified: Wed Apr 10 03:20:40 2024, max compression
+gzip compressed data, was "dist/ros-cdk-rocketmq5-1.0.25.tar", last modified: Mon Jun  3 10:41:37 2024, max compression
```

## Comparing `ros-cdk-rocketmq5-1.0.24.tar` & `ros-cdk-rocketmq5-1.0.25.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:20:40.000000 ros-cdk-rocketmq5-1.0.24/
--rw-r--r--   0 root         (0) root         (0)    10279 2024-04-10 03:20:39.000000 ros-cdk-rocketmq5-1.0.24/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-10 03:20:39.000000 ros-cdk-rocketmq5-1.0.24/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2024-04-10 03:20:39.000000 ros-cdk-rocketmq5-1.0.24/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1316 2024-04-10 03:20:40.000000 ros-cdk-rocketmq5-1.0.24/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      197 2024-04-10 03:20:39.000000 ros-cdk-rocketmq5-1.0.24/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2024-04-10 03:20:39.000000 ros-cdk-rocketmq5-1.0.24/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 03:20:40.000000 ros-cdk-rocketmq5-1.0.24/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1952 2024-04-10 03:20:39.000000 ros-cdk-rocketmq5-1.0.24/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:20:40.000000 ros-cdk-rocketmq5-1.0.24/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:20:40.000000 ros-cdk-rocketmq5-1.0.24/src/ros_cdk_rocketmq5/
--rw-r--r--   0 root         (0) root         (0)   127336 2024-04-10 03:20:39.000000 ros-cdk-rocketmq5-1.0.24/src/ros_cdk_rocketmq5/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:20:40.000000 ros-cdk-rocketmq5-1.0.24/src/ros_cdk_rocketmq5/_jsii/
--rw-r--r--   0 root         (0) root         (0)      431 2024-04-10 03:20:39.000000 ros-cdk-rocketmq5-1.0.24/src/ros_cdk_rocketmq5/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    60520 2024-04-10 03:20:39.000000 ros-cdk-rocketmq5-1.0.24/src/ros_cdk_rocketmq5/_jsii/ros-cdk-rocketmq5@1.0.24.jsii.tgz
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:20:40.000000 ros-cdk-rocketmq5-1.0.24/src/ros_cdk_rocketmq5/datasource/
--rw-r--r--   0 root         (0) root         (0)    16489 2024-04-10 03:20:39.000000 ros-cdk-rocketmq5-1.0.24/src/ros_cdk_rocketmq5/datasource/__init__.py
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 03:20:39.000000 ros-cdk-rocketmq5-1.0.24/src/ros_cdk_rocketmq5/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:20:40.000000 ros-cdk-rocketmq5-1.0.24/src/ros_cdk_rocketmq5.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1316 2024-04-10 03:20:40.000000 ros-cdk-rocketmq5-1.0.24/src/ros_cdk_rocketmq5.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      506 2024-04-10 03:20:40.000000 ros-cdk-rocketmq5-1.0.24/src/ros_cdk_rocketmq5.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 03:20:40.000000 ros-cdk-rocketmq5-1.0.24/src/ros_cdk_rocketmq5.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      110 2024-04-10 03:20:40.000000 ros-cdk-rocketmq5-1.0.24/src/ros_cdk_rocketmq5.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-04-10 03:20:40.000000 ros-cdk-rocketmq5-1.0.24/src/ros_cdk_rocketmq5.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 10:41:37.000000 ros-cdk-rocketmq5-1.0.25/
+-rw-r--r--   0 root         (0) root         (0)    10279 2024-06-03 10:41:37.000000 ros-cdk-rocketmq5-1.0.25/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2024-06-03 10:41:37.000000 ros-cdk-rocketmq5-1.0.25/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2024-06-03 10:41:37.000000 ros-cdk-rocketmq5-1.0.25/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1316 2024-06-03 10:41:37.000000 ros-cdk-rocketmq5-1.0.25/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      197 2024-06-03 10:41:37.000000 ros-cdk-rocketmq5-1.0.25/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2024-06-03 10:41:37.000000 ros-cdk-rocketmq5-1.0.25/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-06-03 10:41:37.000000 ros-cdk-rocketmq5-1.0.25/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1953 2024-06-03 10:41:37.000000 ros-cdk-rocketmq5-1.0.25/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 10:41:37.000000 ros-cdk-rocketmq5-1.0.25/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 10:41:37.000000 ros-cdk-rocketmq5-1.0.25/src/ros_cdk_rocketmq5/
+-rw-r--r--   0 root         (0) root         (0)   130059 2024-06-03 10:41:37.000000 ros-cdk-rocketmq5-1.0.25/src/ros_cdk_rocketmq5/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 10:41:37.000000 ros-cdk-rocketmq5-1.0.25/src/ros_cdk_rocketmq5/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      431 2024-06-03 10:41:37.000000 ros-cdk-rocketmq5-1.0.25/src/ros_cdk_rocketmq5/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63546 2024-06-03 10:41:37.000000 ros-cdk-rocketmq5-1.0.25/src/ros_cdk_rocketmq5/_jsii/ros-cdk-rocketmq5@1.0.25.jsii.tgz
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 10:41:37.000000 ros-cdk-rocketmq5-1.0.25/src/ros_cdk_rocketmq5/datasource/
+-rw-r--r--   0 root         (0) root         (0)    16489 2024-06-03 10:41:37.000000 ros-cdk-rocketmq5-1.0.25/src/ros_cdk_rocketmq5/datasource/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 10:41:37.000000 ros-cdk-rocketmq5-1.0.25/src/ros_cdk_rocketmq5/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 10:41:37.000000 ros-cdk-rocketmq5-1.0.25/src/ros_cdk_rocketmq5.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1316 2024-06-03 10:41:37.000000 ros-cdk-rocketmq5-1.0.25/src/ros_cdk_rocketmq5.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      506 2024-06-03 10:41:37.000000 ros-cdk-rocketmq5-1.0.25/src/ros_cdk_rocketmq5.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 10:41:37.000000 ros-cdk-rocketmq5-1.0.25/src/ros_cdk_rocketmq5.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      111 2024-06-03 10:41:37.000000 ros-cdk-rocketmq5-1.0.25/src/ros_cdk_rocketmq5.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-06-03 10:41:37.000000 ros-cdk-rocketmq5-1.0.25/src/ros_cdk_rocketmq5.egg-info/top_level.txt
```

### Comparing `ros-cdk-rocketmq5-1.0.24/LICENSE` & `ros-cdk-rocketmq5-1.0.25/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-rocketmq5-1.0.24/PKG-INFO` & `ros-cdk-rocketmq5-1.0.25/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-rocketmq5
-Version: 1.0.24
+Version: 1.0.25
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS ROCKETMQ5 Construct Library
```

### Comparing `ros-cdk-rocketmq5-1.0.24/setup.py` & `ros-cdk-rocketmq5-1.0.25/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-rocketmq5",
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
         "ros_cdk_rocketmq5",
         "ros_cdk_rocketmq5._jsii",
         "ros_cdk_rocketmq5.datasource"
     ],
     "package_data": {
         "ros_cdk_rocketmq5._jsii": [
-            "ros-cdk-rocketmq5@1.0.24.jsii.tgz"
+            "ros-cdk-rocketmq5@1.0.25.jsii.tgz"
         ],
         "ros_cdk_rocketmq5": [
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

### Comparing `ros-cdk-rocketmq5-1.0.24/src/ros_cdk_rocketmq5/__init__.py` & `ros-cdk-rocketmq5-1.0.25/src/ros_cdk_rocketmq5/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 
 class ConsumerGroup(
     _ros_cdk_core_7adfd82f.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-rocketmq5.ConsumerGroup",
 ):
-    '''This class encapsulates and extends the ROS resource type ``ALIYUN::ROCKETMQ5::ConsumerGroup``.
+    '''This class encapsulates and extends the ROS resource type ``ALIYUN::ROCKETMQ5::ConsumerGroup``, which is used to create a consumer group in ApsaraMQ for RocketMQ 5.0.
 
     :Note:
 
     This class may have some new functions to facilitate development, so it is recommended to use this class instead of ``RosConsumerGroup``for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-rocketmq5-consumergroup
     '''
 
@@ -570,15 +570,15 @@
 
 
 class RosConsumerGroup(
     _ros_cdk_core_7adfd82f.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-rocketmq5.RosConsumerGroup",
 ):
-    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::ROCKETMQ5::ConsumerGroup``.
+    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::ROCKETMQ5::ConsumerGroup``, which is used to create a consumer group in ApsaraMQ for RocketMQ 5.0.
 
     :Note:
 
     This class does not contain additional functions, so it is recommended to use the ``ConsumerGroup`` class instead of this class for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-rocketmq5-consumergroup
     '''
 
@@ -1489,57 +1489,95 @@
             return "ProductInfoProperty(%s)" % ", ".join(
                 k + "=" + repr(v) for k, v in self._values.items()
             )
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-rocketmq5.RosInstance.VpcInfoProperty",
         jsii_struct_bases=[],
-        name_mapping={"vpc_id": "vpcId", "v_switch_id": "vSwitchId"},
+        name_mapping={
+            "vpc_id": "vpcId",
+            "security_group_id": "securityGroupId",
+            "v_switch_id": "vSwitchId",
+            "v_switch_ids": "vSwitchIds",
+        },
     )
     class VpcInfoProperty:
         def __init__(
             self,
             *,
             vpc_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-            v_switch_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+            security_group_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+            v_switch_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+            v_switch_ids: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Sequence[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]]] = None,
         ) -> None:
             '''
             :param vpc_id: 
+            :param security_group_id: 
             :param v_switch_id: 
+            :param v_switch_ids: 
             '''
             if __debug__:
                 type_hints = typing.get_type_hints(_typecheckingstub__ab194163ad2d0abb0b5eeb404a371273f2bf2f4fe8d941e9e4c77d928e96021c)
                 check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+                check_type(argname="argument security_group_id", value=security_group_id, expected_type=type_hints["security_group_id"])
                 check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+                check_type(argname="argument v_switch_ids", value=v_switch_ids, expected_type=type_hints["v_switch_ids"])
             self._values: typing.Dict[builtins.str, typing.Any] = {
                 "vpc_id": vpc_id,
-                "v_switch_id": v_switch_id,
             }
+            if security_group_id is not None:
+                self._values["security_group_id"] = security_group_id
+            if v_switch_id is not None:
+                self._values["v_switch_id"] = v_switch_id
+            if v_switch_ids is not None:
+                self._values["v_switch_ids"] = v_switch_ids
 
         @builtins.property
         def vpc_id(
             self,
         ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
             '''
             :Property: vpcId: ID of the VPC associated with the instance to be created.
             '''
             result = self._values.get("vpc_id")
             assert result is not None, "Required property 'vpc_id' is missing"
             return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
 
         @builtins.property
+        def security_group_id(
+            self,
+        ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+            '''
+            :Property: securityGroupId: ID of the security group associated with the instance to be created. Required when creating serverless.
+            '''
+            result = self._values.get("security_group_id")
+            return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+        @builtins.property
         def v_switch_id(
             self,
-        ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
             '''
             :Property: vSwitchId: ID of the vSwitch associated with the instance to be created.
             '''
             result = self._values.get("v_switch_id")
-            assert result is not None, "Required property 'v_switch_id' is missing"
-            return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+            return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+        @builtins.property
+        def v_switch_ids(
+            self,
+        ) -> typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]]]:
+            '''
+            :Property:
+
+            vSwitchIds: IDs of the vSwitchs associated with the instance to be created.
+            **Note**: Only one is required for VSwitchIds and VSwitchId. When both are filled in, VSwitchIds overwrites VSwitchId.
+            '''
+            result = self._values.get("v_switch_ids")
+            return typing.cast(typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]]], result)
 
         def __eq__(self, rhs: typing.Any) -> builtins.bool:
             return isinstance(rhs, self.__class__) and rhs._values == self._values
 
         def __ne__(self, rhs: typing.Any) -> builtins.bool:
             return not (rhs == self)
 
@@ -2595,15 +2633,17 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__ab194163ad2d0abb0b5eeb404a371273f2bf2f4fe8d941e9e4c77d928e96021c(
     *,
     vpc_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
-    v_switch_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    security_group_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    v_switch_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    v_switch_ids: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Sequence[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__5fd32fec669d4d859c4cb0dfdc36c63bb55d4d6b52bfa45105234248621d43dc(
     *,
     internet_info: typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Union[RosInstance.InternetInfoProperty, typing.Dict[builtins.str, typing.Any]]],
```

### Comparing `ros-cdk-rocketmq5-1.0.24/src/ros_cdk_rocketmq5/datasource/__init__.py` & `ros-cdk-rocketmq5-1.0.25/src/ros_cdk_rocketmq5/datasource/__init__.py`

 * *Files identical despite different names*

### Comparing `ros-cdk-rocketmq5-1.0.24/src/ros_cdk_rocketmq5.egg-info/PKG-INFO` & `ros-cdk-rocketmq5-1.0.25/src/ros_cdk_rocketmq5.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-rocketmq5
-Version: 1.0.24
+Version: 1.0.25
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS ROCKETMQ5 Construct Library
```

