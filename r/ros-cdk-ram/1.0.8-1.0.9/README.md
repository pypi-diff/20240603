# Comparing `tmp/ros-cdk-ram-1.0.8.tar.gz` & `tmp/ros-cdk-ram-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-ram-1.0.8.tar", last modified: Thu Jul 14 02:43:33 2022, max compression
+gzip compressed data, was "dist/ros-cdk-ram-1.0.9.tar", last modified: Fri Sep 23 12:31:17 2022, max compression
```

## Comparing `ros-cdk-ram-1.0.8.tar` & `ros-cdk-ram-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:43:33.000000 ros-cdk-ram-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:43:33.000000 ros-cdk-ram-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:43:33.000000 ros-cdk-ram-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:43:33.000000 ros-cdk-ram-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:43:33.000000 ros-cdk-ram-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      179 2022-07-14 02:43:33.000000 ros-cdk-ram-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:43:33.000000 ros-cdk-ram-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:43:33.000000 ros-cdk-ram-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1794 2022-07-14 02:43:33.000000 ros-cdk-ram-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:43:33.000000 ros-cdk-ram-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:43:33.000000 ros-cdk-ram-1.0.8/src/ros_cdk_ram/
--rw-r--r--   0 root         (0) root         (0)   254329 2022-07-14 02:43:33.000000 ros-cdk-ram-1.0.8/src/ros_cdk_ram/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:43:33.000000 ros-cdk-ram-1.0.8/src/ros_cdk_ram/_jsii/
--rw-r--r--   0 root         (0) root         (0)      370 2022-07-14 02:43:33.000000 ros-cdk-ram-1.0.8/src/ros_cdk_ram/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    99358 2022-07-14 02:43:33.000000 ros-cdk-ram-1.0.8/src/ros_cdk_ram/_jsii/ros-cdk-ram@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:43:33.000000 ros-cdk-ram-1.0.8/src/ros_cdk_ram/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:43:33.000000 ros-cdk-ram-1.0.8/src/ros_cdk_ram.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:43:33.000000 ros-cdk-ram-1.0.8/src/ros_cdk_ram.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      400 2022-07-14 02:43:33.000000 ros-cdk-ram-1.0.8/src/ros_cdk_ram.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:43:33.000000 ros-cdk-ram-1.0.8/src/ros_cdk_ram.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:43:33.000000 ros-cdk-ram-1.0.8/src/ros_cdk_ram.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-07-14 02:43:33.000000 ros-cdk-ram-1.0.8/src/ros_cdk_ram.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:31:17.000000 ros-cdk-ram-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 12:31:16.000000 ros-cdk-ram-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 12:31:16.000000 ros-cdk-ram-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 12:31:16.000000 ros-cdk-ram-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 12:31:17.000000 ros-cdk-ram-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      179 2022-09-23 12:31:16.000000 ros-cdk-ram-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 12:31:16.000000 ros-cdk-ram-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 12:31:17.000000 ros-cdk-ram-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2022-09-23 12:31:16.000000 ros-cdk-ram-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:31:17.000000 ros-cdk-ram-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:31:17.000000 ros-cdk-ram-1.0.9/src/ros_cdk_ram/
+-rw-r--r--   0 root         (0) root         (0)   307270 2022-09-23 12:31:16.000000 ros-cdk-ram-1.0.9/src/ros_cdk_ram/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:31:17.000000 ros-cdk-ram-1.0.9/src/ros_cdk_ram/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      404 2022-09-23 12:31:16.000000 ros-cdk-ram-1.0.9/src/ros_cdk_ram/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    99426 2022-09-23 12:31:16.000000 ros-cdk-ram-1.0.9/src/ros_cdk_ram/_jsii/ros-cdk-ram@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:31:16.000000 ros-cdk-ram-1.0.9/src/ros_cdk_ram/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:31:17.000000 ros-cdk-ram-1.0.9/src/ros_cdk_ram.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 12:31:17.000000 ros-cdk-ram-1.0.9/src/ros_cdk_ram.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      400 2022-09-23 12:31:17.000000 ros-cdk-ram-1.0.9/src/ros_cdk_ram.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:31:17.000000 ros-cdk-ram-1.0.9/src/ros_cdk_ram.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 12:31:17.000000 ros-cdk-ram-1.0.9/src/ros_cdk_ram.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-09-23 12:31:17.000000 ros-cdk-ram-1.0.9/src/ros_cdk_ram.egg-info/top_level.txt
```

### Comparing `ros-cdk-ram-1.0.8/LICENSE` & `ros-cdk-ram-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-ram-1.0.8/PKG-INFO` & `ros-cdk-ram-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-ram
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS RAM Construct Library
```

### Comparing `ros-cdk-ram-1.0.8/setup.py` & `ros-cdk-ram-1.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-ram",
-    "version": "1.0.8",
+    "version": "1.0.9",
     "description": "Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com",
     "license": "Apache-2.0",
     "url": "https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git",
     "long_description_content_type": "text/markdown",
     "author": "ROS Development Team",
     "bdist_wheel": {
         "universal": true
@@ -22,26 +22,27 @@
     },
     "packages": [
         "ros_cdk_ram",
         "ros_cdk_ram._jsii"
     ],
     "package_data": {
         "ros_cdk_ram._jsii": [
-            "ros-cdk-ram@1.0.8.jsii.tgz"
+            "ros-cdk-ram@1.0.9.jsii.tgz"
         ],
         "ros_cdk_ram": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "constructs>=3.0.4, <4.0.0",
-        "jsii>=1.62.0, <2.0.0",
+        "jsii>=1.68.0, <2.0.0",
         "publication>=0.0.3",
-        "ros-cdk-core>=1.0.6, <2.0.0"
+        "ros-cdk-core>=1.0.6, <2.0.0",
+        "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
```

### Comparing `ros-cdk-ram-1.0.8/src/ros_cdk_ram/__init__.py` & `ros-cdk-ram-1.0.9/src/ros_cdk_ram/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 import enum
 import typing
 
 import jsii
 import publication
 import typing_extensions
 
+from typeguard import check_type
+
 from ._jsii import *
 
 import ros_cdk_core
 
 
 class AccessKey(
     ros_cdk_core.Resource,
@@ -29,43 +31,49 @@
 ):
     '''A ROS resource type:  ``ALIYUN::RAM::AccessKey``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "AccessKeyProps",
+        props: typing.Union["AccessKeyProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::RAM::AccessKey``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AccessKey.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAccessKeyId")
     def attr_access_key_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute AccessKeyId: Id of access key.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAccessKeyId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAccessKeySecret")
     def attr_access_key_secret(self) -> ros_cdk_core.IResolvable:
         '''Attribute AccessKeySecret: Secret of access key.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAccessKeySecret"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrStatus")
     def attr_status(self) -> ros_cdk_core.IResolvable:
         '''Attribute Status: Status of access key.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrStatus"))
 
 
 @jsii.data_type(
@@ -79,14 +87,17 @@
         *,
         user_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::RAM::AccessKey``.
 
         :param user_name: Property userName: Specifies the user name, containing up to 64 characters.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AccessKeyProps.__init__)
+            check_type(argname="argument user_name", value=user_name, expected_type=type_hints["user_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "user_name": user_name,
         }
 
     @builtins.property
     def user_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''Property userName: Specifies the user name, containing up to 64 characters.'''
@@ -113,28 +124,34 @@
 ):
     '''A ROS resource type:  ``ALIYUN::RAM::AttachPolicyToRole``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "AttachPolicyToRoleProps",
+        props: typing.Union["AttachPolicyToRoleProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::RAM::AttachPolicyToRole``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AttachPolicyToRole.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-ram.AttachPolicyToRoleProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -153,14 +170,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::RAM::AttachPolicyToRole``.
 
         :param policy_name: Property policyName: Authorization policy name.
         :param policy_type: Property policyType: Authorization policy type. Value: "System" or "Custom".
         :param role_name: Property roleName: Role name.Example: dev.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AttachPolicyToRoleProps.__init__)
+            check_type(argname="argument policy_name", value=policy_name, expected_type=type_hints["policy_name"])
+            check_type(argname="argument policy_type", value=policy_type, expected_type=type_hints["policy_type"])
+            check_type(argname="argument role_name", value=role_name, expected_type=type_hints["role_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "policy_name": policy_name,
             "policy_type": policy_type,
             "role_name": role_name,
         }
 
     @builtins.property
@@ -206,28 +228,34 @@
 ):
     '''A ROS resource type:  ``ALIYUN::RAM::AttachPolicyToUser``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "AttachPolicyToUserProps",
+        props: typing.Union["AttachPolicyToUserProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::RAM::AttachPolicyToUser``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AttachPolicyToUser.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-ram.AttachPolicyToUserProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -246,14 +274,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::RAM::AttachPolicyToUser``.
 
         :param policy_name: Property policyName: Authorization policy name.
         :param policy_type: Property policyType: Authorization policy type. Value: "System" or "Custom".
         :param user_name: Property userName: User name.Example: dev.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AttachPolicyToUserProps.__init__)
+            check_type(argname="argument policy_name", value=policy_name, expected_type=type_hints["policy_name"])
+            check_type(argname="argument policy_type", value=policy_type, expected_type=type_hints["policy_type"])
+            check_type(argname="argument user_name", value=user_name, expected_type=type_hints["user_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "policy_name": policy_name,
             "policy_type": policy_type,
             "user_name": user_name,
         }
 
     @builtins.property
@@ -299,31 +332,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::RAM::Group``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "GroupProps",
+        props: typing.Union["GroupProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::RAM::Group``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Group.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrGroupName")
     def attr_group_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute GroupName: Id of ram group.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrGroupName"))
 
 
 @jsii.data_type(
@@ -340,25 +379,32 @@
 class GroupProps:
     def __init__(
         self,
         *,
         group_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         comments: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         deletion_force: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-        policies: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosGroup.PoliciesProperty"]]]] = None,
-        policy_attachments: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosGroup.PolicyAttachmentsProperty"]] = None,
+        policies: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosGroup.PoliciesProperty", typing.Dict[str, typing.Any]]]]]] = None,
+        policy_attachments: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosGroup.PolicyAttachmentsProperty", typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::RAM::Group``.
 
         :param group_name: Property groupName: Specifies the group name, containing up to 64 characters.
         :param comments: Property comments: Remark information, up to 128 characters or Chinese characters.
         :param deletion_force: Property deletionForce: Whether force detach the policies attached to the group. Default value is false.
         :param policies: Property policies: Describes what actions are allowed on what resources.
         :param policy_attachments: Property policyAttachments: System and custom policy names to attach.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(GroupProps.__init__)
+            check_type(argname="argument group_name", value=group_name, expected_type=type_hints["group_name"])
+            check_type(argname="argument comments", value=comments, expected_type=type_hints["comments"])
+            check_type(argname="argument deletion_force", value=deletion_force, expected_type=type_hints["deletion_force"])
+            check_type(argname="argument policies", value=policies, expected_type=type_hints["policies"])
+            check_type(argname="argument policy_attachments", value=policy_attachments, expected_type=type_hints["policy_attachments"])
         self._values: typing.Dict[str, typing.Any] = {
             "group_name": group_name,
         }
         if comments is not None:
             self._values["comments"] = comments
         if deletion_force is not None:
             self._values["deletion_force"] = deletion_force
@@ -428,31 +474,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::RAM::ManagedPolicy``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ManagedPolicyProps",
+        props: typing.Union["ManagedPolicyProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::RAM::ManagedPolicy``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ManagedPolicy.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPolicyName")
     def attr_policy_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute PolicyName: When the logical ID of this resource is provided to the Ref intrinsic function, Ref returns the ARN.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPolicyName"))
 
 
 @jsii.data_type(
@@ -471,29 +523,38 @@
 class ManagedPolicyProps:
     def __init__(
         self,
         *,
         policy_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         groups: typing.Optional[typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable]] = None,
-        policy_document: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosManagedPolicy.PolicyDocumentProperty"]] = None,
+        policy_document: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosManagedPolicy.PolicyDocumentProperty", typing.Dict[str, typing.Any]]]] = None,
         policy_document_unchecked: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]] = None,
         roles: typing.Optional[typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable]] = None,
         users: typing.Optional[typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::RAM::ManagedPolicy``.
 
         :param policy_name: Property policyName: Specifies the authorization policy name, containing up to 128 characters.
         :param description: Property description: Specifies the authorization policy description, containing up to 1024 characters.
         :param groups: Property groups: The names of groups to attach to this policy.
         :param policy_document: Property policyDocument: A policy document that describes what actions are allowed on which resources.
         :param policy_document_unchecked: Property policyDocumentUnchecked: A policy document that describes what actions are allowed on which resources. If it is specified, PolicyDocument will be ignored.
         :param roles: Property roles: The names of roles to attach to this policy.
         :param users: Property users: The names of users to attach to this policy.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ManagedPolicyProps.__init__)
+            check_type(argname="argument policy_name", value=policy_name, expected_type=type_hints["policy_name"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument groups", value=groups, expected_type=type_hints["groups"])
+            check_type(argname="argument policy_document", value=policy_document, expected_type=type_hints["policy_document"])
+            check_type(argname="argument policy_document_unchecked", value=policy_document_unchecked, expected_type=type_hints["policy_document_unchecked"])
+            check_type(argname="argument roles", value=roles, expected_type=type_hints["roles"])
+            check_type(argname="argument users", value=users, expected_type=type_hints["users"])
         self._values: typing.Dict[str, typing.Any] = {
             "policy_name": policy_name,
         }
         if description is not None:
             self._values["description"] = description
         if groups is not None:
             self._values["groups"] = groups
@@ -583,31 +644,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::RAM::RamAccountAlias``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RamAccountAliasProps",
+        props: typing.Union["RamAccountAliasProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::RAM::RamAccountAlias``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RamAccountAlias.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAccountAlias")
     def attr_account_alias(self) -> ros_cdk_core.IResolvable:
         '''Attribute AccountAlias: The alias of the Alibaba Cloud account.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAccountAlias"))
 
 
 @jsii.data_type(
@@ -621,14 +688,17 @@
         *,
         account_alias: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::RAM::RamAccountAlias``.
 
         :param account_alias: Property accountAlias: The alias of the Alibaba Cloud account. The alias must be 1 to 50 characters in length, and can contain lowercase letters, digits, hyphens (-), periods (.) and underscores (_). Note It cannot start or end with a hyphen (-).The default domain name cannot start or end with a hyphen (-) and cannot have two consecutive hyphens (-).
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RamAccountAliasProps.__init__)
+            check_type(argname="argument account_alias", value=account_alias, expected_type=type_hints["account_alias"])
         self._values: typing.Dict[str, typing.Any] = {
             "account_alias": account_alias,
         }
 
     @builtins.property
     def account_alias(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''Property accountAlias: The alias of the Alibaba Cloud account.
@@ -661,43 +731,49 @@
 ):
     '''A ROS resource type:  ``ALIYUN::RAM::Role``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RoleProps",
+        props: typing.Union["RoleProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::RAM::Role``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Role.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrArn")
     def attr_arn(self) -> ros_cdk_core.IResolvable:
         '''Attribute Arn: Name of alicloud resource.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrArn"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRoleId")
     def attr_role_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute RoleId: Id of ram role.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRoleId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRoleName")
     def attr_role_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute RoleName: Name of ram role.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRoleName"))
 
 
 @jsii.data_type(
@@ -713,32 +789,41 @@
         "policy_attachments": "policyAttachments",
     },
 )
 class RoleProps:
     def __init__(
         self,
         *,
-        assume_role_policy_document: typing.Union[ros_cdk_core.IResolvable, "RosRole.AssumeRolePolicyDocumentProperty"],
+        assume_role_policy_document: typing.Union[ros_cdk_core.IResolvable, typing.Union["RosRole.AssumeRolePolicyDocumentProperty", typing.Dict[str, typing.Any]]],
         role_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         deletion_force: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         max_session_duration: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-        policies: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosRole.PoliciesProperty"]]]] = None,
-        policy_attachments: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosRole.PolicyAttachmentsProperty"]] = None,
+        policies: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosRole.PoliciesProperty", typing.Dict[str, typing.Any]]]]]] = None,
+        policy_attachments: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosRole.PolicyAttachmentsProperty", typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::RAM::Role``.
 
         :param assume_role_policy_document: Property assumeRolePolicyDocument: The RAM assume role policy that is associated with this role.
         :param role_name: Property roleName: Specifies the role name, containing up to 64 characters.
         :param deletion_force: Property deletionForce: Whether force detach the policies attached to the role. Default value is false.
         :param description: Property description: Remark information, up to 1024 characters or Chinese characters.
         :param max_session_duration: Property maxSessionDuration: The maximum session duration of the RAM role. Valid values: 3600 to 43200. Unit: seconds. Default value: 3600. The default value is used if the parameter is not specified.
         :param policies: Property policies: Describes what actions are allowed on what resources.
         :param policy_attachments: Property policyAttachments: System and custom policy names to attach.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RoleProps.__init__)
+            check_type(argname="argument assume_role_policy_document", value=assume_role_policy_document, expected_type=type_hints["assume_role_policy_document"])
+            check_type(argname="argument role_name", value=role_name, expected_type=type_hints["role_name"])
+            check_type(argname="argument deletion_force", value=deletion_force, expected_type=type_hints["deletion_force"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument max_session_duration", value=max_session_duration, expected_type=type_hints["max_session_duration"])
+            check_type(argname="argument policies", value=policies, expected_type=type_hints["policies"])
+            check_type(argname="argument policy_attachments", value=policy_attachments, expected_type=type_hints["policy_attachments"])
         self._values: typing.Dict[str, typing.Any] = {
             "assume_role_policy_document": assume_role_policy_document,
             "role_name": role_name,
         }
         if deletion_force is not None:
             self._values["deletion_force"] = deletion_force
         if description is not None:
@@ -832,93 +917,108 @@
 ):
     '''A ROS template type:  ``ALIYUN::RAM::AccessKey``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosAccessKeyProps",
+        props: typing.Union["RosAccessKeyProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::RAM::AccessKey``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAccessKey.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
     @jsii.member(jsii_name="renderProperties")
     def _render_properties(
         self,
         props: typing.Mapping[builtins.str, typing.Any],
     ) -> typing.Mapping[builtins.str, typing.Any]:
         '''
         :param props: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAccessKey._render_properties)
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.invoke(self, "renderProperties", [props]))
 
-    @jsii.python.classproperty # type: ignore[misc]
+    @jsii.python.classproperty
     @jsii.member(jsii_name="ROS_RESOURCE_TYPE_NAME")
     def ROS_RESOURCE_TYPE_NAME(cls) -> builtins.str:
         '''The resource type name for this resource class.'''
         return typing.cast(builtins.str, jsii.sget(cls, "ROS_RESOURCE_TYPE_NAME"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAccessKeyId")
     def attr_access_key_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AccessKeyId: Id of access key.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAccessKeyId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAccessKeySecret")
     def attr_access_key_secret(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AccessKeySecret: Secret of access key.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAccessKeySecret"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrStatus")
     def attr_status(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Status: Status of access key.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrStatus"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccessKey, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="userName")
     def user_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: userName: Specifies the user name, containing up to 64 characters.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "userName"))
 
     @user_name.setter
     def user_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccessKey, "user_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "userName", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-ram.RosAccessKeyProps",
     jsii_struct_bases=[],
     name_mapping={"user_name": "userName"},
@@ -929,14 +1029,17 @@
         *,
         user_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::RAM::AccessKey``.
 
         :param user_name: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAccessKeyProps.__init__)
+            check_type(argname="argument user_name", value=user_name, expected_type=type_hints["user_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "user_name": user_name,
         }
 
     @builtins.property
     def user_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
@@ -965,100 +1068,121 @@
 ):
     '''A ROS template type:  ``ALIYUN::RAM::AttachPolicyToRole``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosAttachPolicyToRoleProps",
+        props: typing.Union["RosAttachPolicyToRoleProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::RAM::AttachPolicyToRole``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAttachPolicyToRole.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
     @jsii.member(jsii_name="renderProperties")
     def _render_properties(
         self,
         props: typing.Mapping[builtins.str, typing.Any],
     ) -> typing.Mapping[builtins.str, typing.Any]:
         '''
         :param props: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAttachPolicyToRole._render_properties)
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.invoke(self, "renderProperties", [props]))
 
-    @jsii.python.classproperty # type: ignore[misc]
+    @jsii.python.classproperty
     @jsii.member(jsii_name="ROS_RESOURCE_TYPE_NAME")
     def ROS_RESOURCE_TYPE_NAME(cls) -> builtins.str:
         '''The resource type name for this resource class.'''
         return typing.cast(builtins.str, jsii.sget(cls, "ROS_RESOURCE_TYPE_NAME"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         '''A factory method that creates a new instance of this class from an object containing the properties of this ROS resource.'''
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAttachPolicyToRole, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="policyName")
     def policy_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: policyName: Authorization policy name.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "policyName"))
 
     @policy_name.setter
     def policy_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAttachPolicyToRole, "policy_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "policyName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="policyType")
     def policy_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: policyType: Authorization policy type. Value: "System" or "Custom".
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "policyType"))
 
     @policy_type.setter
     def policy_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAttachPolicyToRole, "policy_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "policyType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="roleName")
     def role_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: roleName: Role name.Example: dev.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "roleName"))
 
     @role_name.setter
     def role_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAttachPolicyToRole, "role_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "roleName", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-ram.RosAttachPolicyToRoleProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -1077,14 +1201,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::RAM::AttachPolicyToRole``.
 
         :param policy_name: 
         :param policy_type: 
         :param role_name: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAttachPolicyToRoleProps.__init__)
+            check_type(argname="argument policy_name", value=policy_name, expected_type=type_hints["policy_name"])
+            check_type(argname="argument policy_type", value=policy_type, expected_type=type_hints["policy_type"])
+            check_type(argname="argument role_name", value=role_name, expected_type=type_hints["role_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "policy_name": policy_name,
             "policy_type": policy_type,
             "role_name": role_name,
         }
 
     @builtins.property
@@ -1133,100 +1262,121 @@
 ):
     '''A ROS template type:  ``ALIYUN::RAM::AttachPolicyToUser``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosAttachPolicyToUserProps",
+        props: typing.Union["RosAttachPolicyToUserProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::RAM::AttachPolicyToUser``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAttachPolicyToUser.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
     @jsii.member(jsii_name="renderProperties")
     def _render_properties(
         self,
         props: typing.Mapping[builtins.str, typing.Any],
     ) -> typing.Mapping[builtins.str, typing.Any]:
         '''
         :param props: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAttachPolicyToUser._render_properties)
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.invoke(self, "renderProperties", [props]))
 
-    @jsii.python.classproperty # type: ignore[misc]
+    @jsii.python.classproperty
     @jsii.member(jsii_name="ROS_RESOURCE_TYPE_NAME")
     def ROS_RESOURCE_TYPE_NAME(cls) -> builtins.str:
         '''The resource type name for this resource class.'''
         return typing.cast(builtins.str, jsii.sget(cls, "ROS_RESOURCE_TYPE_NAME"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         '''A factory method that creates a new instance of this class from an object containing the properties of this ROS resource.'''
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAttachPolicyToUser, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="policyName")
     def policy_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: policyName: Authorization policy name.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "policyName"))
 
     @policy_name.setter
     def policy_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAttachPolicyToUser, "policy_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "policyName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="policyType")
     def policy_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: policyType: Authorization policy type. Value: "System" or "Custom".
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "policyType"))
 
     @policy_type.setter
     def policy_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAttachPolicyToUser, "policy_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "policyType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="userName")
     def user_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: userName: User name.Example: dev.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "userName"))
 
     @user_name.setter
     def user_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAttachPolicyToUser, "user_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "userName", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-ram.RosAttachPolicyToUserProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -1245,14 +1395,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::RAM::AttachPolicyToUser``.
 
         :param policy_name: 
         :param policy_type: 
         :param user_name: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAttachPolicyToUserProps.__init__)
+            check_type(argname="argument policy_name", value=policy_name, expected_type=type_hints["policy_name"])
+            check_type(argname="argument policy_type", value=policy_type, expected_type=type_hints["policy_type"])
+            check_type(argname="argument user_name", value=user_name, expected_type=type_hints["user_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "policy_name": policy_name,
             "policy_type": policy_type,
             "user_name": user_name,
         }
 
     @builtins.property
@@ -1301,145 +1456,172 @@
 ):
     '''A ROS template type:  ``ALIYUN::RAM::Group``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosGroupProps",
+        props: typing.Union["RosGroupProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::RAM::Group``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosGroup.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
     @jsii.member(jsii_name="renderProperties")
     def _render_properties(
         self,
         props: typing.Mapping[builtins.str, typing.Any],
     ) -> typing.Mapping[builtins.str, typing.Any]:
         '''
         :param props: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosGroup._render_properties)
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.invoke(self, "renderProperties", [props]))
 
-    @jsii.python.classproperty # type: ignore[misc]
+    @jsii.python.classproperty
     @jsii.member(jsii_name="ROS_RESOURCE_TYPE_NAME")
     def ROS_RESOURCE_TYPE_NAME(cls) -> builtins.str:
         '''The resource type name for this resource class.'''
         return typing.cast(builtins.str, jsii.sget(cls, "ROS_RESOURCE_TYPE_NAME"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrGroupName")
     def attr_group_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: GroupName: Id of ram group.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrGroupName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroup, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="groupName")
     def group_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: groupName: Specifies the group name, containing up to 64 characters.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "groupName"))
 
     @group_name.setter
     def group_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroup, "group_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "groupName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="comments")
     def comments(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: comments: Remark information, up to 128 characters or Chinese characters.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "comments"))
 
     @comments.setter
     def comments(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroup, "comments").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "comments", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="deletionForce")
     def deletion_force(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: deletionForce: Whether force detach the policies attached to the group. Default value is false.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "deletionForce"))
 
     @deletion_force.setter
     def deletion_force(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroup, "deletion_force").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "deletionForce", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="policies")
     def policies(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosGroup.PoliciesProperty"]]]]:
         '''
         :Property: policies: Describes what actions are allowed on what resources.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosGroup.PoliciesProperty"]]]], jsii.get(self, "policies"))
 
     @policies.setter
     def policies(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosGroup.PoliciesProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroup, "policies").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "policies", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="policyAttachments")
     def policy_attachments(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosGroup.PolicyAttachmentsProperty"]]:
         '''
         :Property: policyAttachments: System and custom policy names to attach.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosGroup.PolicyAttachmentsProperty"]], jsii.get(self, "policyAttachments"))
 
     @policy_attachments.setter
     def policy_attachments(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosGroup.PolicyAttachmentsProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroup, "policy_attachments").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "policyAttachments", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-ram.RosGroup.PoliciesProperty",
         jsii_struct_bases=[],
         name_mapping={
             "policy_document": "policyDocument",
@@ -1447,23 +1629,28 @@
             "description": "description",
         },
     )
     class PoliciesProperty:
         def __init__(
             self,
             *,
-            policy_document: typing.Union[ros_cdk_core.IResolvable, "RosGroup.PolicyDocumentProperty"],
+            policy_document: typing.Union[ros_cdk_core.IResolvable, typing.Union["RosGroup.PolicyDocumentProperty", typing.Dict[str, typing.Any]]],
             policy_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param policy_document: 
             :param policy_name: 
             :param description: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosGroup.PoliciesProperty.__init__)
+                check_type(argname="argument policy_document", value=policy_document, expected_type=type_hints["policy_document"])
+                check_type(argname="argument policy_name", value=policy_name, expected_type=type_hints["policy_name"])
+                check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             self._values: typing.Dict[str, typing.Any] = {
                 "policy_document": policy_document,
                 "policy_name": policy_name,
             }
             if description is not None:
                 self._values["description"] = description
 
@@ -1520,14 +1707,18 @@
             custom: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
             system: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         ) -> None:
             '''
             :param custom: 
             :param system: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosGroup.PolicyAttachmentsProperty.__init__)
+                check_type(argname="argument custom", value=custom, expected_type=type_hints["custom"])
+                check_type(argname="argument system", value=system, expected_type=type_hints["system"])
             self._values: typing.Dict[str, typing.Any] = {}
             if custom is not None:
                 self._values["custom"] = custom
             if system is not None:
                 self._values["system"] = system
 
         @builtins.property
@@ -1566,21 +1757,25 @@
         jsii_struct_bases=[],
         name_mapping={"statement": "statement", "version": "version"},
     )
     class PolicyDocumentProperty:
         def __init__(
             self,
             *,
-            statement: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosGroup.StatementProperty"]]],
+            statement: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosGroup.StatementProperty", typing.Dict[str, typing.Any]]]]],
             version: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param statement: 
             :param version: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosGroup.PolicyDocumentProperty.__init__)
+                check_type(argname="argument statement", value=statement, expected_type=type_hints["statement"])
+                check_type(argname="argument version", value=version, expected_type=type_hints["version"])
             self._values: typing.Dict[str, typing.Any] = {
                 "statement": statement,
                 "version": version,
             }
 
         @builtins.property
         def statement(
@@ -1634,14 +1829,20 @@
         ) -> None:
             '''
             :param action: 
             :param condition: 
             :param effect: 
             :param resource: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosGroup.StatementProperty.__init__)
+                check_type(argname="argument action", value=action, expected_type=type_hints["action"])
+                check_type(argname="argument condition", value=condition, expected_type=type_hints["condition"])
+                check_type(argname="argument effect", value=effect, expected_type=type_hints["effect"])
+                check_type(argname="argument resource", value=resource, expected_type=type_hints["resource"])
             self._values: typing.Dict[str, typing.Any] = {}
             if action is not None:
                 self._values["action"] = action
             if condition is not None:
                 self._values["condition"] = condition
             if effect is not None:
                 self._values["effect"] = effect
@@ -1714,25 +1915,32 @@
 class RosGroupProps:
     def __init__(
         self,
         *,
         group_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         comments: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         deletion_force: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-        policies: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosGroup.PoliciesProperty]]]] = None,
-        policy_attachments: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosGroup.PolicyAttachmentsProperty]] = None,
+        policies: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosGroup.PoliciesProperty, typing.Dict[str, typing.Any]]]]]] = None,
+        policy_attachments: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosGroup.PolicyAttachmentsProperty, typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::RAM::Group``.
 
         :param group_name: 
         :param comments: 
         :param deletion_force: 
         :param policies: 
         :param policy_attachments: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosGroupProps.__init__)
+            check_type(argname="argument group_name", value=group_name, expected_type=type_hints["group_name"])
+            check_type(argname="argument comments", value=comments, expected_type=type_hints["comments"])
+            check_type(argname="argument deletion_force", value=deletion_force, expected_type=type_hints["deletion_force"])
+            check_type(argname="argument policies", value=policies, expected_type=type_hints["policies"])
+            check_type(argname="argument policy_attachments", value=policy_attachments, expected_type=type_hints["policy_attachments"])
         self._values: typing.Dict[str, typing.Any] = {
             "group_name": group_name,
         }
         if comments is not None:
             self._values["comments"] = comments
         if deletion_force is not None:
             self._values["deletion_force"] = deletion_force
@@ -1809,197 +2017,234 @@
 ):
     '''A ROS template type:  ``ALIYUN::RAM::ManagedPolicy``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosManagedPolicyProps",
+        props: typing.Union["RosManagedPolicyProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::RAM::ManagedPolicy``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosManagedPolicy.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
     @jsii.member(jsii_name="renderProperties")
     def _render_properties(
         self,
         props: typing.Mapping[builtins.str, typing.Any],
     ) -> typing.Mapping[builtins.str, typing.Any]:
         '''
         :param props: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosManagedPolicy._render_properties)
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.invoke(self, "renderProperties", [props]))
 
-    @jsii.python.classproperty # type: ignore[misc]
+    @jsii.python.classproperty
     @jsii.member(jsii_name="ROS_RESOURCE_TYPE_NAME")
     def ROS_RESOURCE_TYPE_NAME(cls) -> builtins.str:
         '''The resource type name for this resource class.'''
         return typing.cast(builtins.str, jsii.sget(cls, "ROS_RESOURCE_TYPE_NAME"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPolicyName")
     def attr_policy_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PolicyName: When the logical ID of this resource is provided to the Ref intrinsic function, Ref returns the ARN.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPolicyName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedPolicy, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="policyName")
     def policy_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: policyName: Specifies the authorization policy name, containing up to 128 characters.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "policyName"))
 
     @policy_name.setter
     def policy_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedPolicy, "policy_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "policyName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: Specifies the authorization policy description, containing up to 1024 characters.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedPolicy, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="groups")
     def groups(
         self,
     ) -> typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]]:
         '''
         :Property: groups: The names of groups to attach to this policy.
         '''
         return typing.cast(typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]], jsii.get(self, "groups"))
 
     @groups.setter
     def groups(
         self,
         value: typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedPolicy, "groups").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "groups", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="policyDocument")
     def policy_document(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosManagedPolicy.PolicyDocumentProperty"]]:
         '''
         :Property: policyDocument: A policy document that describes what actions are allowed on which resources.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosManagedPolicy.PolicyDocumentProperty"]], jsii.get(self, "policyDocument"))
 
     @policy_document.setter
     def policy_document(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosManagedPolicy.PolicyDocumentProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedPolicy, "policy_document").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "policyDocument", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="policyDocumentUnchecked")
     def policy_document_unchecked(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]]:
         '''
         :Property: policyDocumentUnchecked: A policy document that describes what actions are allowed on which resources. If it is specified, PolicyDocument will be ignored.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]], jsii.get(self, "policyDocumentUnchecked"))
 
     @policy_document_unchecked.setter
     def policy_document_unchecked(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedPolicy, "policy_document_unchecked").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "policyDocumentUnchecked", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="roles")
     def roles(
         self,
     ) -> typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]]:
         '''
         :Property: roles: The names of roles to attach to this policy.
         '''
         return typing.cast(typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]], jsii.get(self, "roles"))
 
     @roles.setter
     def roles(
         self,
         value: typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedPolicy, "roles").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "roles", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="users")
     def users(
         self,
     ) -> typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]]:
         '''
         :Property: users: The names of users to attach to this policy.
         '''
         return typing.cast(typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]], jsii.get(self, "users"))
 
     @users.setter
     def users(
         self,
         value: typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedPolicy, "users").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "users", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-ram.RosManagedPolicy.PolicyDocumentProperty",
         jsii_struct_bases=[],
         name_mapping={"statement": "statement", "version": "version"},
     )
     class PolicyDocumentProperty:
         def __init__(
             self,
             *,
-            statement: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosManagedPolicy.StatementProperty"]]],
+            statement: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosManagedPolicy.StatementProperty", typing.Dict[str, typing.Any]]]]],
             version: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param statement: 
             :param version: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosManagedPolicy.PolicyDocumentProperty.__init__)
+                check_type(argname="argument statement", value=statement, expected_type=type_hints["statement"])
+                check_type(argname="argument version", value=version, expected_type=type_hints["version"])
             self._values: typing.Dict[str, typing.Any] = {
                 "statement": statement,
                 "version": version,
             }
 
         @builtins.property
         def statement(
@@ -2053,14 +2298,20 @@
         ) -> None:
             '''
             :param action: 
             :param condition: 
             :param effect: 
             :param resource: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosManagedPolicy.StatementProperty.__init__)
+                check_type(argname="argument action", value=action, expected_type=type_hints["action"])
+                check_type(argname="argument condition", value=condition, expected_type=type_hints["condition"])
+                check_type(argname="argument effect", value=effect, expected_type=type_hints["effect"])
+                check_type(argname="argument resource", value=resource, expected_type=type_hints["resource"])
             self._values: typing.Dict[str, typing.Any] = {}
             if action is not None:
                 self._values["action"] = action
             if condition is not None:
                 self._values["condition"] = condition
             if effect is not None:
                 self._values["effect"] = effect
@@ -2135,29 +2386,38 @@
 class RosManagedPolicyProps:
     def __init__(
         self,
         *,
         policy_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         groups: typing.Optional[typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable]] = None,
-        policy_document: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosManagedPolicy.PolicyDocumentProperty]] = None,
+        policy_document: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosManagedPolicy.PolicyDocumentProperty, typing.Dict[str, typing.Any]]]] = None,
         policy_document_unchecked: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]] = None,
         roles: typing.Optional[typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable]] = None,
         users: typing.Optional[typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::RAM::ManagedPolicy``.
 
         :param policy_name: 
         :param description: 
         :param groups: 
         :param policy_document: 
         :param policy_document_unchecked: 
         :param roles: 
         :param users: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosManagedPolicyProps.__init__)
+            check_type(argname="argument policy_name", value=policy_name, expected_type=type_hints["policy_name"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument groups", value=groups, expected_type=type_hints["groups"])
+            check_type(argname="argument policy_document", value=policy_document, expected_type=type_hints["policy_document"])
+            check_type(argname="argument policy_document_unchecked", value=policy_document_unchecked, expected_type=type_hints["policy_document_unchecked"])
+            check_type(argname="argument roles", value=roles, expected_type=type_hints["roles"])
+            check_type(argname="argument users", value=users, expected_type=type_hints["users"])
         self._values: typing.Dict[str, typing.Any] = {
             "policy_name": policy_name,
         }
         if description is not None:
             self._values["description"] = description
         if groups is not None:
             self._values["groups"] = groups
@@ -2258,56 +2518,65 @@
 ):
     '''A ROS template type:  ``ALIYUN::RAM::RamAccountAlias``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosRamAccountAliasProps",
+        props: typing.Union["RosRamAccountAliasProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::RAM::RamAccountAlias``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosRamAccountAlias.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
     @jsii.member(jsii_name="renderProperties")
     def _render_properties(
         self,
         props: typing.Mapping[builtins.str, typing.Any],
     ) -> typing.Mapping[builtins.str, typing.Any]:
         '''
         :param props: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosRamAccountAlias._render_properties)
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.invoke(self, "renderProperties", [props]))
 
-    @jsii.python.classproperty # type: ignore[misc]
+    @jsii.python.classproperty
     @jsii.member(jsii_name="ROS_RESOURCE_TYPE_NAME")
     def ROS_RESOURCE_TYPE_NAME(cls) -> builtins.str:
         '''The resource type name for this resource class.'''
         return typing.cast(builtins.str, jsii.sget(cls, "ROS_RESOURCE_TYPE_NAME"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAccountAlias")
     def attr_account_alias(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AccountAlias: The alias of the Alibaba Cloud account.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAccountAlias"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="accountAlias")
     def account_alias(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         accountAlias: The alias of the Alibaba Cloud account.
         The alias must be 1 to 50 characters in length, and can contain lowercase letters,
@@ -2318,23 +2587,29 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "accountAlias"))
 
     @account_alias.setter
     def account_alias(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRamAccountAlias, "account_alias").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "accountAlias", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRamAccountAlias, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-ram.RosRamAccountAliasProps",
     jsii_struct_bases=[],
     name_mapping={"account_alias": "accountAlias"},
@@ -2345,14 +2620,17 @@
         *,
         account_alias: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::RAM::RamAccountAlias``.
 
         :param account_alias: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosRamAccountAliasProps.__init__)
+            check_type(argname="argument account_alias", value=account_alias, expected_type=type_hints["account_alias"])
         self._values: typing.Dict[str, typing.Any] = {
             "account_alias": account_alias,
         }
 
     @builtins.property
     def account_alias(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
@@ -2387,147 +2665,171 @@
 ):
     '''A ROS template type:  ``ALIYUN::RAM::Role``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosRoleProps",
+        props: typing.Union["RosRoleProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::RAM::Role``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosRole.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
     @jsii.member(jsii_name="renderProperties")
     def _render_properties(
         self,
         props: typing.Mapping[builtins.str, typing.Any],
     ) -> typing.Mapping[builtins.str, typing.Any]:
         '''
         :param props: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosRole._render_properties)
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.invoke(self, "renderProperties", [props]))
 
-    @jsii.python.classproperty # type: ignore[misc]
+    @jsii.python.classproperty
     @jsii.member(jsii_name="ROS_RESOURCE_TYPE_NAME")
     def ROS_RESOURCE_TYPE_NAME(cls) -> builtins.str:
         '''The resource type name for this resource class.'''
         return typing.cast(builtins.str, jsii.sget(cls, "ROS_RESOURCE_TYPE_NAME"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrArn")
     def attr_arn(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Arn: Name of alicloud resource.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrArn"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRoleId")
     def attr_role_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: RoleId: Id of ram role.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRoleId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRoleName")
     def attr_role_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: RoleName: Name of ram role.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRoleName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="assumeRolePolicyDocument")
     def assume_role_policy_document(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, "RosRole.AssumeRolePolicyDocumentProperty"]:
         '''
         :Property: assumeRolePolicyDocument: The RAM assume role policy that is associated with this role.
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, "RosRole.AssumeRolePolicyDocumentProperty"], jsii.get(self, "assumeRolePolicyDocument"))
 
     @assume_role_policy_document.setter
     def assume_role_policy_document(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, "RosRole.AssumeRolePolicyDocumentProperty"],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRole, "assume_role_policy_document").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "assumeRolePolicyDocument", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRole, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="roleName")
     def role_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: roleName: Specifies the role name, containing up to 64 characters.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "roleName"))
 
     @role_name.setter
     def role_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRole, "role_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "roleName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="deletionForce")
     def deletion_force(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: deletionForce: Whether force detach the policies attached to the role. Default value is false.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "deletionForce"))
 
     @deletion_force.setter
     def deletion_force(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRole, "deletion_force").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "deletionForce", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: Remark information, up to 1024 characters or Chinese characters.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRole, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="maxSessionDuration")
     def max_session_duration(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2538,66 +2840,79 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "maxSessionDuration"))
 
     @max_session_duration.setter
     def max_session_duration(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRole, "max_session_duration").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "maxSessionDuration", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="policies")
     def policies(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosRole.PoliciesProperty"]]]]:
         '''
         :Property: policies: Describes what actions are allowed on what resources.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosRole.PoliciesProperty"]]]], jsii.get(self, "policies"))
 
     @policies.setter
     def policies(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosRole.PoliciesProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRole, "policies").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "policies", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="policyAttachments")
     def policy_attachments(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosRole.PolicyAttachmentsProperty"]]:
         '''
         :Property: policyAttachments: System and custom policy names to attach.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosRole.PolicyAttachmentsProperty"]], jsii.get(self, "policyAttachments"))
 
     @policy_attachments.setter
     def policy_attachments(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosRole.PolicyAttachmentsProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRole, "policy_attachments").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "policyAttachments", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-ram.RosRole.AssumeRolePolicyDocumentProperty",
         jsii_struct_bases=[],
         name_mapping={"statement": "statement", "version": "version"},
     )
     class AssumeRolePolicyDocumentProperty:
         def __init__(
             self,
             *,
-            statement: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosRole.StatementProperty"]]],
+            statement: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosRole.StatementProperty", typing.Dict[str, typing.Any]]]]],
             version: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param statement: 
             :param version: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosRole.AssumeRolePolicyDocumentProperty.__init__)
+                check_type(argname="argument statement", value=statement, expected_type=type_hints["statement"])
+                check_type(argname="argument version", value=version, expected_type=type_hints["version"])
             self._values: typing.Dict[str, typing.Any] = {
                 "statement": statement,
                 "version": version,
             }
 
         @builtins.property
         def statement(
@@ -2702,14 +3017,37 @@
             :param string_equals: 
             :param string_equals_ignore_case: 
             :param string_like: 
             :param string_not_equals: 
             :param string_not_equals_ignore_case: 
             :param string_not_like: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosRole.ConditionProperty.__init__)
+                check_type(argname="argument bool", value=bool, expected_type=type_hints["bool"])
+                check_type(argname="argument date_equals", value=date_equals, expected_type=type_hints["date_equals"])
+                check_type(argname="argument date_greater_than", value=date_greater_than, expected_type=type_hints["date_greater_than"])
+                check_type(argname="argument date_greater_than_equals", value=date_greater_than_equals, expected_type=type_hints["date_greater_than_equals"])
+                check_type(argname="argument date_less_than", value=date_less_than, expected_type=type_hints["date_less_than"])
+                check_type(argname="argument date_less_than_equals", value=date_less_than_equals, expected_type=type_hints["date_less_than_equals"])
+                check_type(argname="argument date_not_equals", value=date_not_equals, expected_type=type_hints["date_not_equals"])
+                check_type(argname="argument ip_address", value=ip_address, expected_type=type_hints["ip_address"])
+                check_type(argname="argument not_ip_address", value=not_ip_address, expected_type=type_hints["not_ip_address"])
+                check_type(argname="argument numeric_equals", value=numeric_equals, expected_type=type_hints["numeric_equals"])
+                check_type(argname="argument numeric_greater_than", value=numeric_greater_than, expected_type=type_hints["numeric_greater_than"])
+                check_type(argname="argument numeric_greater_than_equals", value=numeric_greater_than_equals, expected_type=type_hints["numeric_greater_than_equals"])
+                check_type(argname="argument numeric_less_than", value=numeric_less_than, expected_type=type_hints["numeric_less_than"])
+                check_type(argname="argument numeric_less_than_equals", value=numeric_less_than_equals, expected_type=type_hints["numeric_less_than_equals"])
+                check_type(argname="argument numeric_not_equals", value=numeric_not_equals, expected_type=type_hints["numeric_not_equals"])
+                check_type(argname="argument string_equals", value=string_equals, expected_type=type_hints["string_equals"])
+                check_type(argname="argument string_equals_ignore_case", value=string_equals_ignore_case, expected_type=type_hints["string_equals_ignore_case"])
+                check_type(argname="argument string_like", value=string_like, expected_type=type_hints["string_like"])
+                check_type(argname="argument string_not_equals", value=string_not_equals, expected_type=type_hints["string_not_equals"])
+                check_type(argname="argument string_not_equals_ignore_case", value=string_not_equals_ignore_case, expected_type=type_hints["string_not_equals_ignore_case"])
+                check_type(argname="argument string_not_like", value=string_not_like, expected_type=type_hints["string_not_like"])
             self._values: typing.Dict[str, typing.Any] = {}
             if bool is not None:
                 self._values["bool"] = bool
             if date_equals is not None:
                 self._values["date_equals"] = date_equals
             if date_greater_than is not None:
                 self._values["date_greater_than"] = date_greater_than
@@ -2980,23 +3318,28 @@
             "description": "description",
         },
     )
     class PoliciesProperty:
         def __init__(
             self,
             *,
-            policy_document: typing.Union[ros_cdk_core.IResolvable, "RosRole.PolicyDocumentProperty"],
+            policy_document: typing.Union[ros_cdk_core.IResolvable, typing.Union["RosRole.PolicyDocumentProperty", typing.Dict[str, typing.Any]]],
             policy_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param policy_document: 
             :param policy_name: 
             :param description: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosRole.PoliciesProperty.__init__)
+                check_type(argname="argument policy_document", value=policy_document, expected_type=type_hints["policy_document"])
+                check_type(argname="argument policy_name", value=policy_name, expected_type=type_hints["policy_name"])
+                check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             self._values: typing.Dict[str, typing.Any] = {
                 "policy_document": policy_document,
                 "policy_name": policy_name,
             }
             if description is not None:
                 self._values["description"] = description
 
@@ -3053,14 +3396,18 @@
             custom: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
             system: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         ) -> None:
             '''
             :param custom: 
             :param system: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosRole.PolicyAttachmentsProperty.__init__)
+                check_type(argname="argument custom", value=custom, expected_type=type_hints["custom"])
+                check_type(argname="argument system", value=system, expected_type=type_hints["system"])
             self._values: typing.Dict[str, typing.Any] = {}
             if custom is not None:
                 self._values["custom"] = custom
             if system is not None:
                 self._values["system"] = system
 
         @builtins.property
@@ -3099,21 +3446,25 @@
         jsii_struct_bases=[],
         name_mapping={"statement": "statement", "version": "version"},
     )
     class PolicyDocumentProperty:
         def __init__(
             self,
             *,
-            statement: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosRole.PolicyDocumentStatementProperty"]]],
+            statement: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosRole.PolicyDocumentStatementProperty", typing.Dict[str, typing.Any]]]]],
             version: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param statement: 
             :param version: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosRole.PolicyDocumentProperty.__init__)
+                check_type(argname="argument statement", value=statement, expected_type=type_hints["statement"])
+                check_type(argname="argument version", value=version, expected_type=type_hints["version"])
             self._values: typing.Dict[str, typing.Any] = {
                 "statement": statement,
                 "version": version,
             }
 
         @builtins.property
         def statement(
@@ -3167,14 +3518,20 @@
         ) -> None:
             '''
             :param action: 
             :param condition: 
             :param effect: 
             :param resource: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosRole.PolicyDocumentStatementProperty.__init__)
+                check_type(argname="argument action", value=action, expected_type=type_hints["action"])
+                check_type(argname="argument condition", value=condition, expected_type=type_hints["condition"])
+                check_type(argname="argument effect", value=effect, expected_type=type_hints["effect"])
+                check_type(argname="argument resource", value=resource, expected_type=type_hints["resource"])
             self._values: typing.Dict[str, typing.Any] = {}
             if action is not None:
                 self._values["action"] = action
             if condition is not None:
                 self._values["condition"] = condition
             if effect is not None:
                 self._values["effect"] = effect
@@ -3246,14 +3603,19 @@
             service: typing.Optional[typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param federated: 
             :param ram: 
             :param service: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosRole.PrincipalProperty.__init__)
+                check_type(argname="argument federated", value=federated, expected_type=type_hints["federated"])
+                check_type(argname="argument ram", value=ram, expected_type=type_hints["ram"])
+                check_type(argname="argument service", value=service, expected_type=type_hints["service"])
             self._values: typing.Dict[str, typing.Any] = {}
             if federated is not None:
                 self._values["federated"] = federated
             if ram is not None:
                 self._values["ram"] = ram
             if service is not None:
                 self._values["service"] = service
@@ -3310,24 +3672,30 @@
         },
     )
     class StatementProperty:
         def __init__(
             self,
             *,
             action: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-            condition: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosRole.ConditionProperty"]] = None,
+            condition: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosRole.ConditionProperty", typing.Dict[str, typing.Any]]]] = None,
             effect: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-            principal: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosRole.PrincipalProperty"]] = None,
+            principal: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosRole.PrincipalProperty", typing.Dict[str, typing.Any]]]] = None,
         ) -> None:
             '''
             :param action: 
             :param condition: 
             :param effect: 
             :param principal: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosRole.StatementProperty.__init__)
+                check_type(argname="argument action", value=action, expected_type=type_hints["action"])
+                check_type(argname="argument condition", value=condition, expected_type=type_hints["condition"])
+                check_type(argname="argument effect", value=effect, expected_type=type_hints["effect"])
+                check_type(argname="argument principal", value=principal, expected_type=type_hints["principal"])
             self._values: typing.Dict[str, typing.Any] = {}
             if action is not None:
                 self._values["action"] = action
             if condition is not None:
                 self._values["condition"] = condition
             if effect is not None:
                 self._values["effect"] = effect
@@ -3399,32 +3767,41 @@
         "policy_attachments": "policyAttachments",
     },
 )
 class RosRoleProps:
     def __init__(
         self,
         *,
-        assume_role_policy_document: typing.Union[ros_cdk_core.IResolvable, RosRole.AssumeRolePolicyDocumentProperty],
+        assume_role_policy_document: typing.Union[ros_cdk_core.IResolvable, typing.Union[RosRole.AssumeRolePolicyDocumentProperty, typing.Dict[str, typing.Any]]],
         role_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         deletion_force: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         max_session_duration: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-        policies: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosRole.PoliciesProperty]]]] = None,
-        policy_attachments: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosRole.PolicyAttachmentsProperty]] = None,
+        policies: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosRole.PoliciesProperty, typing.Dict[str, typing.Any]]]]]] = None,
+        policy_attachments: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosRole.PolicyAttachmentsProperty, typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::RAM::Role``.
 
         :param assume_role_policy_document: 
         :param role_name: 
         :param deletion_force: 
         :param description: 
         :param max_session_duration: 
         :param policies: 
         :param policy_attachments: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosRoleProps.__init__)
+            check_type(argname="argument assume_role_policy_document", value=assume_role_policy_document, expected_type=type_hints["assume_role_policy_document"])
+            check_type(argname="argument role_name", value=role_name, expected_type=type_hints["role_name"])
+            check_type(argname="argument deletion_force", value=deletion_force, expected_type=type_hints["deletion_force"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument max_session_duration", value=max_session_duration, expected_type=type_hints["max_session_duration"])
+            check_type(argname="argument policies", value=policies, expected_type=type_hints["policies"])
+            check_type(argname="argument policy_attachments", value=policy_attachments, expected_type=type_hints["policy_attachments"])
         self._values: typing.Dict[str, typing.Any] = {
             "assume_role_policy_document": assume_role_policy_document,
             "role_name": role_name,
         }
         if deletion_force is not None:
             self._values["deletion_force"] = deletion_force
         if description is not None:
@@ -3529,138 +3906,162 @@
 ):
     '''A ROS template type:  ``ALIYUN::RAM::SAMLProvider``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosSAMLProviderProps",
+        props: typing.Union["RosSAMLProviderProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::RAM::SAMLProvider``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosSAMLProvider.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
     @jsii.member(jsii_name="renderProperties")
     def _render_properties(
         self,
         props: typing.Mapping[builtins.str, typing.Any],
     ) -> typing.Mapping[builtins.str, typing.Any]:
         '''
         :param props: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosSAMLProvider._render_properties)
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.invoke(self, "renderProperties", [props]))
 
-    @jsii.python.classproperty # type: ignore[misc]
+    @jsii.python.classproperty
     @jsii.member(jsii_name="ROS_RESOURCE_TYPE_NAME")
     def ROS_RESOURCE_TYPE_NAME(cls) -> builtins.str:
         '''The resource type name for this resource class.'''
         return typing.cast(builtins.str, jsii.sget(cls, "ROS_RESOURCE_TYPE_NAME"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrArn")
     def attr_arn(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Arn: ARN.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrArn"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSamlProviderName")
     def attr_saml_provider_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: SAMLProviderName: IdP Name.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSamlProviderName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSAMLProvider, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="samlProviderName")
     def saml_provider_name(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: samlProviderName: IdP Name. The IdP name can contain a maximum of 128 characters and only letters, numbers, and the following special characters are accepted: hyphens (-), periods (.), and underscores (_). It cannot start or end with a special character.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "samlProviderName"))
 
     @saml_provider_name.setter
     def saml_provider_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSAMLProvider, "saml_provider_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "samlProviderName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: The description can contain a maximum of 256 characters.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSAMLProvider, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="samlMetadataDocument")
     def saml_metadata_document(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: samlMetadataDocument: SAML metadata document. The content must be 1 to 102,400 bytes in length.You must specify one of the SAMLMetadataDocument and SAMLMetadataDocumentURL properties, but you cannot specify both of them.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "samlMetadataDocument"))
 
     @saml_metadata_document.setter
     def saml_metadata_document(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSAMLProvider, "saml_metadata_document").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "samlMetadataDocument", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="samlMetadataDocumentUrl")
     def saml_metadata_document_url(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: samlMetadataDocumentUrl: The URL for the file that contains the SAML metadata document. The URL must point to a document located in an HTTP or HTTPS web server or an Alibaba Cloud OSS bucket. Examples: oss://ros/document/demo and oss://ros/document/demo?RegionId=cn-hangzhou. The URL can be up to 1,024 bytes in length.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "samlMetadataDocumentUrl"))
 
     @saml_metadata_document_url.setter
     def saml_metadata_document_url(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSAMLProvider, "saml_metadata_document_url").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "samlMetadataDocumentUrl", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-ram.RosSAMLProviderProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -3682,14 +4083,20 @@
         '''Properties for defining a ``ALIYUN::RAM::SAMLProvider``.
 
         :param saml_provider_name: 
         :param description: 
         :param saml_metadata_document: 
         :param saml_metadata_document_url: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosSAMLProviderProps.__init__)
+            check_type(argname="argument saml_provider_name", value=saml_provider_name, expected_type=type_hints["saml_provider_name"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument saml_metadata_document", value=saml_metadata_document, expected_type=type_hints["saml_metadata_document"])
+            check_type(argname="argument saml_metadata_document_url", value=saml_metadata_document_url, expected_type=type_hints["saml_metadata_document_url"])
         self._values: typing.Dict[str, typing.Any] = {
             "saml_provider_name": saml_provider_name,
         }
         if description is not None:
             self._values["description"] = description
         if saml_metadata_document is not None:
             self._values["saml_metadata_document"] = saml_metadata_document
@@ -3756,113 +4163,125 @@
 ):
     '''A ROS template type:  ``ALIYUN::RAM::SecurityPreference``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosSecurityPreferenceProps",
+        props: typing.Union["RosSecurityPreferenceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::RAM::SecurityPreference``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosSecurityPreference.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
     @jsii.member(jsii_name="renderProperties")
     def _render_properties(
         self,
         props: typing.Mapping[builtins.str, typing.Any],
     ) -> typing.Mapping[builtins.str, typing.Any]:
         '''
         :param props: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosSecurityPreference._render_properties)
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.invoke(self, "renderProperties", [props]))
 
-    @jsii.python.classproperty # type: ignore[misc]
+    @jsii.python.classproperty
     @jsii.member(jsii_name="ROS_RESOURCE_TYPE_NAME")
     def ROS_RESOURCE_TYPE_NAME(cls) -> builtins.str:
         '''The resource type name for this resource class.'''
         return typing.cast(builtins.str, jsii.sget(cls, "ROS_RESOURCE_TYPE_NAME"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAllowUserToChangePassword")
     def attr_allow_user_to_change_password(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AllowUserToChangePassword: Specifies whether RAM users can change their passwords.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAllowUserToChangePassword"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAllowUserToManageAccessKeys")
     def attr_allow_user_to_manage_access_keys(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AllowUserToManageAccessKeys: Specifies whether RAM users can manage their AccessKey pairs.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAllowUserToManageAccessKeys"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAllowUserToManageMfaDevices")
     def attr_allow_user_to_manage_mfa_devices(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AllowUserToManageMFADevices: Specifies whether RAM users can manage their MFA devices.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAllowUserToManageMfaDevices"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAllowUserToManagePublicKeys")
     def attr_allow_user_to_manage_public_keys(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AllowUserToManagePublicKeys: Specifies whether RAM users can manage their public keys.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAllowUserToManagePublicKeys"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEnableSaveMfaTicket")
     def attr_enable_save_mfa_ticket(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: EnableSaveMFATicket: Specifies whether RAM users can save multi-factor authentication (MFA) security codes during logon.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEnableSaveMfaTicket"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLoginNetworkMasks")
     def attr_login_network_masks(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: LoginNetworkMasks: The subnet mask that specifies the IP addresses from which logon to the console is allowed.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLoginNetworkMasks"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLoginSessionDuration")
     def attr_login_session_duration(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: LoginSessionDuration: The validity period of the logon session of the RAM user.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLoginSessionDuration"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSecurityPreference, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="allowUserToChangePassword")
     def allow_user_to_change_password(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3873,17 +4292,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "allowUserToChangePassword"))
 
     @allow_user_to_change_password.setter
     def allow_user_to_change_password(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSecurityPreference, "allow_user_to_change_password").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "allowUserToChangePassword", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="allowUserToManageAccessKeys")
     def allow_user_to_manage_access_keys(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3894,17 +4316,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "allowUserToManageAccessKeys"))
 
     @allow_user_to_manage_access_keys.setter
     def allow_user_to_manage_access_keys(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSecurityPreference, "allow_user_to_manage_access_keys").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "allowUserToManageAccessKeys", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="allowUserToManageMfaDevices")
     def allow_user_to_manage_mfa_devices(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3915,17 +4340,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "allowUserToManageMfaDevices"))
 
     @allow_user_to_manage_mfa_devices.setter
     def allow_user_to_manage_mfa_devices(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSecurityPreference, "allow_user_to_manage_mfa_devices").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "allowUserToManageMfaDevices", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="allowUserToManagePublicKeys")
     def allow_user_to_manage_public_keys(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3937,17 +4365,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "allowUserToManagePublicKeys"))
 
     @allow_user_to_manage_public_keys.setter
     def allow_user_to_manage_public_keys(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSecurityPreference, "allow_user_to_manage_public_keys").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "allowUserToManagePublicKeys", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableSaveMfaTicket")
     def enable_save_mfa_ticket(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3960,17 +4391,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "enableSaveMfaTicket"))
 
     @enable_save_mfa_ticket.setter
     def enable_save_mfa_ticket(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSecurityPreference, "enable_save_mfa_ticket").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableSaveMfaTicket", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="loginNetworkMasks")
     def login_network_masks(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3990,17 +4424,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "loginNetworkMasks"))
 
     @login_network_masks.setter
     def login_network_masks(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSecurityPreference, "login_network_masks").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "loginNetworkMasks", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="loginSessionDuration")
     def login_session_duration(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -4010,14 +4447,17 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "loginSessionDuration"))
 
     @login_session_duration.setter
     def login_session_duration(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSecurityPreference, "login_session_duration").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "loginSessionDuration", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-ram.RosSecurityPreferenceProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -4048,14 +4488,23 @@
         :param allow_user_to_manage_access_keys: 
         :param allow_user_to_manage_mfa_devices: 
         :param allow_user_to_manage_public_keys: 
         :param enable_save_mfa_ticket: 
         :param login_network_masks: 
         :param login_session_duration: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosSecurityPreferenceProps.__init__)
+            check_type(argname="argument allow_user_to_change_password", value=allow_user_to_change_password, expected_type=type_hints["allow_user_to_change_password"])
+            check_type(argname="argument allow_user_to_manage_access_keys", value=allow_user_to_manage_access_keys, expected_type=type_hints["allow_user_to_manage_access_keys"])
+            check_type(argname="argument allow_user_to_manage_mfa_devices", value=allow_user_to_manage_mfa_devices, expected_type=type_hints["allow_user_to_manage_mfa_devices"])
+            check_type(argname="argument allow_user_to_manage_public_keys", value=allow_user_to_manage_public_keys, expected_type=type_hints["allow_user_to_manage_public_keys"])
+            check_type(argname="argument enable_save_mfa_ticket", value=enable_save_mfa_ticket, expected_type=type_hints["enable_save_mfa_ticket"])
+            check_type(argname="argument login_network_masks", value=login_network_masks, expected_type=type_hints["login_network_masks"])
+            check_type(argname="argument login_session_duration", value=login_session_duration, expected_type=type_hints["login_session_duration"])
         self._values: typing.Dict[str, typing.Any] = {}
         if allow_user_to_change_password is not None:
             self._values["allow_user_to_change_password"] = allow_user_to_change_password
         if allow_user_to_manage_access_keys is not None:
             self._values["allow_user_to_manage_access_keys"] = allow_user_to_manage_access_keys
         if allow_user_to_manage_mfa_devices is not None:
             self._values["allow_user_to_manage_mfa_devices"] = allow_user_to_manage_mfa_devices
@@ -4196,254 +4645,296 @@
 ):
     '''A ROS template type:  ``ALIYUN::RAM::User``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosUserProps",
+        props: typing.Union["RosUserProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::RAM::User``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosUser.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
     @jsii.member(jsii_name="renderProperties")
     def _render_properties(
         self,
         props: typing.Mapping[builtins.str, typing.Any],
     ) -> typing.Mapping[builtins.str, typing.Any]:
         '''
         :param props: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosUser._render_properties)
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.invoke(self, "renderProperties", [props]))
 
-    @jsii.python.classproperty # type: ignore[misc]
+    @jsii.python.classproperty
     @jsii.member(jsii_name="ROS_RESOURCE_TYPE_NAME")
     def ROS_RESOURCE_TYPE_NAME(cls) -> builtins.str:
         '''The resource type name for this resource class.'''
         return typing.cast(builtins.str, jsii.sget(cls, "ROS_RESOURCE_TYPE_NAME"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCreateDate")
     def attr_create_date(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: CreateDate: Create date of ram user.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCreateDate"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLastLoginDate")
     def attr_last_login_date(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: LastLoginDate: Last login date of ram user.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLastLoginDate"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrUserId")
     def attr_user_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: UserId: Id of ram user.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrUserId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrUserName")
     def attr_user_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: UserName: Name of ram user.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrUserName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosUser, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="userName")
     def user_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: userName: Specifies the user name, containing up to 64 characters.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "userName"))
 
     @user_name.setter
     def user_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosUser, "user_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "userName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="comments")
     def comments(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: comments: Comments of ram user.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "comments"))
 
     @comments.setter
     def comments(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosUser, "comments").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "comments", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="deletionForce")
     def deletion_force(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: deletionForce: Whether force detach the policies and groups attached to the user. Default value is false.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "deletionForce"))
 
     @deletion_force.setter
     def deletion_force(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosUser, "deletion_force").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "deletionForce", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="displayName")
     def display_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: displayName: Display name, up to 128 characters or Chinese characters.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "displayName"))
 
     @display_name.setter
     def display_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosUser, "display_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "displayName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="email")
     def email(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: email: Email of ram user.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "email"))
 
     @email.setter
     def email(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosUser, "email").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "email", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="groups")
     def groups(
         self,
     ) -> typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]]:
         '''
         :Property: groups: A name of a group to which you want to add the user.
         '''
         return typing.cast(typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]], jsii.get(self, "groups"))
 
     @groups.setter
     def groups(
         self,
         value: typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosUser, "groups").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "groups", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="loginProfile")
     def login_profile(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosUser.LoginProfileProperty"]]:
         '''
         :Property: loginProfile: Creates a login profile for users so that they can access the AliCloud Management Console.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosUser.LoginProfileProperty"]], jsii.get(self, "loginProfile"))
 
     @login_profile.setter
     def login_profile(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosUser.LoginProfileProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosUser, "login_profile").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "loginProfile", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="mobilePhone")
     def mobile_phone(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: mobilePhone: Phone number of ram user.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "mobilePhone"))
 
     @mobile_phone.setter
     def mobile_phone(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosUser, "mobile_phone").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "mobilePhone", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="policies")
     def policies(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosUser.PoliciesProperty"]]]]:
         '''
         :Property: policies: Describes what actions are allowed on what resources.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosUser.PoliciesProperty"]]]], jsii.get(self, "policies"))
 
     @policies.setter
     def policies(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosUser.PoliciesProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosUser, "policies").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "policies", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="policyAttachments")
     def policy_attachments(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosUser.PolicyAttachmentsProperty"]]:
         '''
         :Property: policyAttachments: System and custom policy names to attach.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosUser.PolicyAttachmentsProperty"]], jsii.get(self, "policyAttachments"))
 
     @policy_attachments.setter
     def policy_attachments(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosUser.PolicyAttachmentsProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosUser, "policy_attachments").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "policyAttachments", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-ram.RosUser.LoginProfileProperty",
         jsii_struct_bases=[],
         name_mapping={
             "mfa_bind_required": "mfaBindRequired",
@@ -4460,14 +4951,19 @@
             password_reset_required: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param mfa_bind_required: 
             :param password: 
             :param password_reset_required: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosUser.LoginProfileProperty.__init__)
+                check_type(argname="argument mfa_bind_required", value=mfa_bind_required, expected_type=type_hints["mfa_bind_required"])
+                check_type(argname="argument password", value=password, expected_type=type_hints["password"])
+                check_type(argname="argument password_reset_required", value=password_reset_required, expected_type=type_hints["password_reset_required"])
             self._values: typing.Dict[str, typing.Any] = {}
             if mfa_bind_required is not None:
                 self._values["mfa_bind_required"] = mfa_bind_required
             if password is not None:
                 self._values["password"] = password
             if password_reset_required is not None:
                 self._values["password_reset_required"] = password_reset_required
@@ -4522,23 +5018,28 @@
             "description": "description",
         },
     )
     class PoliciesProperty:
         def __init__(
             self,
             *,
-            policy_document: typing.Union[ros_cdk_core.IResolvable, "RosUser.PolicyDocumentProperty"],
+            policy_document: typing.Union[ros_cdk_core.IResolvable, typing.Union["RosUser.PolicyDocumentProperty", typing.Dict[str, typing.Any]]],
             policy_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param policy_document: 
             :param policy_name: 
             :param description: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosUser.PoliciesProperty.__init__)
+                check_type(argname="argument policy_document", value=policy_document, expected_type=type_hints["policy_document"])
+                check_type(argname="argument policy_name", value=policy_name, expected_type=type_hints["policy_name"])
+                check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             self._values: typing.Dict[str, typing.Any] = {
                 "policy_document": policy_document,
                 "policy_name": policy_name,
             }
             if description is not None:
                 self._values["description"] = description
 
@@ -4595,14 +5096,18 @@
             custom: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
             system: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         ) -> None:
             '''
             :param custom: 
             :param system: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosUser.PolicyAttachmentsProperty.__init__)
+                check_type(argname="argument custom", value=custom, expected_type=type_hints["custom"])
+                check_type(argname="argument system", value=system, expected_type=type_hints["system"])
             self._values: typing.Dict[str, typing.Any] = {}
             if custom is not None:
                 self._values["custom"] = custom
             if system is not None:
                 self._values["system"] = system
 
         @builtins.property
@@ -4641,21 +5146,25 @@
         jsii_struct_bases=[],
         name_mapping={"statement": "statement", "version": "version"},
     )
     class PolicyDocumentProperty:
         def __init__(
             self,
             *,
-            statement: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosUser.StatementProperty"]]],
+            statement: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosUser.StatementProperty", typing.Dict[str, typing.Any]]]]],
             version: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param statement: 
             :param version: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosUser.PolicyDocumentProperty.__init__)
+                check_type(argname="argument statement", value=statement, expected_type=type_hints["statement"])
+                check_type(argname="argument version", value=version, expected_type=type_hints["version"])
             self._values: typing.Dict[str, typing.Any] = {
                 "statement": statement,
                 "version": version,
             }
 
         @builtins.property
         def statement(
@@ -4709,14 +5218,20 @@
         ) -> None:
             '''
             :param action: 
             :param condition: 
             :param effect: 
             :param resource: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosUser.StatementProperty.__init__)
+                check_type(argname="argument action", value=action, expected_type=type_hints["action"])
+                check_type(argname="argument condition", value=condition, expected_type=type_hints["condition"])
+                check_type(argname="argument effect", value=effect, expected_type=type_hints["effect"])
+                check_type(argname="argument resource", value=resource, expected_type=type_hints["resource"])
             self._values: typing.Dict[str, typing.Any] = {}
             if action is not None:
                 self._values["action"] = action
             if condition is not None:
                 self._values["condition"] = condition
             if effect is not None:
                 self._values["effect"] = effect
@@ -4797,32 +5312,44 @@
         *,
         user_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         comments: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         deletion_force: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         display_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         email: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         groups: typing.Optional[typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable]] = None,
-        login_profile: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosUser.LoginProfileProperty]] = None,
+        login_profile: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosUser.LoginProfileProperty, typing.Dict[str, typing.Any]]]] = None,
         mobile_phone: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        policies: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosUser.PoliciesProperty]]]] = None,
-        policy_attachments: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosUser.PolicyAttachmentsProperty]] = None,
+        policies: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosUser.PoliciesProperty, typing.Dict[str, typing.Any]]]]]] = None,
+        policy_attachments: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosUser.PolicyAttachmentsProperty, typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::RAM::User``.
 
         :param user_name: 
         :param comments: 
         :param deletion_force: 
         :param display_name: 
         :param email: 
         :param groups: 
         :param login_profile: 
         :param mobile_phone: 
         :param policies: 
         :param policy_attachments: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosUserProps.__init__)
+            check_type(argname="argument user_name", value=user_name, expected_type=type_hints["user_name"])
+            check_type(argname="argument comments", value=comments, expected_type=type_hints["comments"])
+            check_type(argname="argument deletion_force", value=deletion_force, expected_type=type_hints["deletion_force"])
+            check_type(argname="argument display_name", value=display_name, expected_type=type_hints["display_name"])
+            check_type(argname="argument email", value=email, expected_type=type_hints["email"])
+            check_type(argname="argument groups", value=groups, expected_type=type_hints["groups"])
+            check_type(argname="argument login_profile", value=login_profile, expected_type=type_hints["login_profile"])
+            check_type(argname="argument mobile_phone", value=mobile_phone, expected_type=type_hints["mobile_phone"])
+            check_type(argname="argument policies", value=policies, expected_type=type_hints["policies"])
+            check_type(argname="argument policy_attachments", value=policy_attachments, expected_type=type_hints["policy_attachments"])
         self._values: typing.Dict[str, typing.Any] = {
             "user_name": user_name,
         }
         if comments is not None:
             self._values["comments"] = comments
         if deletion_force is not None:
             self._values["deletion_force"] = deletion_force
@@ -4959,85 +5486,103 @@
 ):
     '''A ROS template type:  ``ALIYUN::RAM::UserToGroupAddition``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosUserToGroupAdditionProps",
+        props: typing.Union["RosUserToGroupAdditionProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::RAM::UserToGroupAddition``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosUserToGroupAddition.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
     @jsii.member(jsii_name="renderProperties")
     def _render_properties(
         self,
         props: typing.Mapping[builtins.str, typing.Any],
     ) -> typing.Mapping[builtins.str, typing.Any]:
         '''
         :param props: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosUserToGroupAddition._render_properties)
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.invoke(self, "renderProperties", [props]))
 
-    @jsii.python.classproperty # type: ignore[misc]
+    @jsii.python.classproperty
     @jsii.member(jsii_name="ROS_RESOURCE_TYPE_NAME")
     def ROS_RESOURCE_TYPE_NAME(cls) -> builtins.str:
         '''The resource type name for this resource class.'''
         return typing.cast(builtins.str, jsii.sget(cls, "ROS_RESOURCE_TYPE_NAME"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         '''A factory method that creates a new instance of this class from an object containing the properties of this ROS resource.'''
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosUserToGroupAddition, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="groupName")
     def group_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: groupName: Specifies the group name, containing up to 64 characters.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "groupName"))
 
     @group_name.setter
     def group_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosUserToGroupAddition, "group_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "groupName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="users")
     def users(self) -> typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]:
         '''
         :Property: users: list name of a users to which you want to add the group.
         '''
         return typing.cast(typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable], jsii.get(self, "users"))
 
     @users.setter
     def users(
         self,
         value: typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosUserToGroupAddition, "users").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "users", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-ram.RosUserToGroupAdditionProps",
     jsii_struct_bases=[],
     name_mapping={"group_name": "groupName", "users": "users"},
@@ -5050,14 +5595,18 @@
         users: typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::RAM::UserToGroupAddition``.
 
         :param group_name: 
         :param users: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosUserToGroupAdditionProps.__init__)
+            check_type(argname="argument group_name", value=group_name, expected_type=type_hints["group_name"])
+            check_type(argname="argument users", value=users, expected_type=type_hints["users"])
         self._values: typing.Dict[str, typing.Any] = {
             "group_name": group_name,
             "users": users,
         }
 
     @builtins.property
     def group_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -5096,37 +5645,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::RAM::SAMLProvider``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "SAMLProviderProps",
+        props: typing.Union["SAMLProviderProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::RAM::SAMLProvider``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(SAMLProvider.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrArn")
     def attr_arn(self) -> ros_cdk_core.IResolvable:
         '''Attribute Arn: ARN.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrArn"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSamlProviderName")
     def attr_saml_provider_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute SAMLProviderName: IdP Name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSamlProviderName"))
 
 
 @jsii.data_type(
@@ -5151,14 +5706,20 @@
         '''Properties for defining a ``ALIYUN::RAM::SAMLProvider``.
 
         :param saml_provider_name: Property samlProviderName: IdP Name. The IdP name can contain a maximum of 128 characters and only letters, numbers, and the following special characters are accepted: hyphens (-), periods (.), and underscores (_). It cannot start or end with a special character.
         :param description: Property description: The description can contain a maximum of 256 characters.
         :param saml_metadata_document: Property samlMetadataDocument: SAML metadata document. The content must be 1 to 102,400 bytes in length.You must specify one of the SAMLMetadataDocument and SAMLMetadataDocumentURL properties, but you cannot specify both of them.
         :param saml_metadata_document_url: Property samlMetadataDocumentUrl: The URL for the file that contains the SAML metadata document. The URL must point to a document located in an HTTP or HTTPS web server or an Alibaba Cloud OSS bucket. Examples: oss://ros/document/demo and oss://ros/document/demo?RegionId=cn-hangzhou. The URL can be up to 1,024 bytes in length.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(SAMLProviderProps.__init__)
+            check_type(argname="argument saml_provider_name", value=saml_provider_name, expected_type=type_hints["saml_provider_name"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument saml_metadata_document", value=saml_metadata_document, expected_type=type_hints["saml_metadata_document"])
+            check_type(argname="argument saml_metadata_document_url", value=saml_metadata_document_url, expected_type=type_hints["saml_metadata_document_url"])
         self._values: typing.Dict[str, typing.Any] = {
             "saml_provider_name": saml_provider_name,
         }
         if description is not None:
             self._values["description"] = description
         if saml_metadata_document is not None:
             self._values["saml_metadata_document"] = saml_metadata_document
@@ -5226,67 +5787,73 @@
 ):
     '''A ROS resource type:  ``ALIYUN::RAM::SecurityPreference``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: typing.Optional["SecurityPreferenceProps"] = None,
+        props: typing.Optional[typing.Union["SecurityPreferenceProps", typing.Dict[str, typing.Any]]] = None,
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::RAM::SecurityPreference``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(SecurityPreference.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAllowUserToChangePassword")
     def attr_allow_user_to_change_password(self) -> ros_cdk_core.IResolvable:
         '''Attribute AllowUserToChangePassword: Specifies whether RAM users can change their passwords.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAllowUserToChangePassword"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAllowUserToManageAccessKeys")
     def attr_allow_user_to_manage_access_keys(self) -> ros_cdk_core.IResolvable:
         '''Attribute AllowUserToManageAccessKeys: Specifies whether RAM users can manage their AccessKey pairs.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAllowUserToManageAccessKeys"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAllowUserToManageMfaDevices")
     def attr_allow_user_to_manage_mfa_devices(self) -> ros_cdk_core.IResolvable:
         '''Attribute AllowUserToManageMFADevices: Specifies whether RAM users can manage their MFA devices.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAllowUserToManageMfaDevices"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAllowUserToManagePublicKeys")
     def attr_allow_user_to_manage_public_keys(self) -> ros_cdk_core.IResolvable:
         '''Attribute AllowUserToManagePublicKeys: Specifies whether RAM users can manage their public keys.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAllowUserToManagePublicKeys"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEnableSaveMfaTicket")
     def attr_enable_save_mfa_ticket(self) -> ros_cdk_core.IResolvable:
         '''Attribute EnableSaveMFATicket: Specifies whether RAM users can save multi-factor authentication (MFA) security codes during logon.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEnableSaveMfaTicket"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLoginNetworkMasks")
     def attr_login_network_masks(self) -> ros_cdk_core.IResolvable:
         '''Attribute LoginNetworkMasks: The subnet mask that specifies the IP addresses from which logon to the console is allowed.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLoginNetworkMasks"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLoginSessionDuration")
     def attr_login_session_duration(self) -> ros_cdk_core.IResolvable:
         '''Attribute LoginSessionDuration: The validity period of the logon session of the RAM user.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLoginSessionDuration"))
 
 
 @jsii.data_type(
@@ -5320,14 +5887,23 @@
         :param allow_user_to_manage_access_keys: Property allowUserToManageAccessKeys: Specifies whether RAM users can manage their AccessKey pairs. Valid values: true: RAM users can manage their AccessKey pairs. false: RAM users cannot manage their AccessKey pairs. This is the default value.
         :param allow_user_to_manage_mfa_devices: Property allowUserToManageMfaDevices: Specifies whether RAM users can manage their MFA devices. Valid values: true: RAM users can manage their MFA devices. This is the default value. false: RAM users cannot manage their MFA devices.
         :param allow_user_to_manage_public_keys: Property allowUserToManagePublicKeys: Specifies whether RAM users can manage their public keys. Valid values: true: RAM users can manage their public keys. false: RAM users cannot manage their public keys. This is the default value. Note This parameter is valid only for the Japan site.
         :param enable_save_mfa_ticket: Property enableSaveMfaTicket: Specifies whether RAM users can save multi-factor authentication (MFA) security codes during logon. The security codes are valid for 7 days. Valid values: true: RAM users can save MFA security codes during logon. false: RAM users cannot save MFA security codes during logon. This is the default value.
         :param login_network_masks: Property loginNetworkMasks: The subnet mask that specifies the IP addresses from which logon to the console is allowed. This parameter applies to password-based logon and single sign-on (SSO). However, this parameter does not apply to API calls that are authenticated based on AccessKey pairs. If a subnet mask is specified, RAM users can log on to the console only by using the IP addresses in the subnet. If you do not specify a subnet mask, RAM users can log on to the console by using all IP addresses. If you want to specify multiple subnet masks, separate the subnet masks with semicolons (;). Example: 192.168.0.0/16;10.0.0.0/8. A maximum of 25 subnet masks can be set. The total length of the subnet masks can be 1 to 512 characters.
         :param login_session_duration: Property loginSessionDuration: The validity period of the logon session of the RAM user. Valid values: 6 to 24. Default value: 6. Unit: hours.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(SecurityPreferenceProps.__init__)
+            check_type(argname="argument allow_user_to_change_password", value=allow_user_to_change_password, expected_type=type_hints["allow_user_to_change_password"])
+            check_type(argname="argument allow_user_to_manage_access_keys", value=allow_user_to_manage_access_keys, expected_type=type_hints["allow_user_to_manage_access_keys"])
+            check_type(argname="argument allow_user_to_manage_mfa_devices", value=allow_user_to_manage_mfa_devices, expected_type=type_hints["allow_user_to_manage_mfa_devices"])
+            check_type(argname="argument allow_user_to_manage_public_keys", value=allow_user_to_manage_public_keys, expected_type=type_hints["allow_user_to_manage_public_keys"])
+            check_type(argname="argument enable_save_mfa_ticket", value=enable_save_mfa_ticket, expected_type=type_hints["enable_save_mfa_ticket"])
+            check_type(argname="argument login_network_masks", value=login_network_masks, expected_type=type_hints["login_network_masks"])
+            check_type(argname="argument login_session_duration", value=login_session_duration, expected_type=type_hints["login_session_duration"])
         self._values: typing.Dict[str, typing.Any] = {}
         if allow_user_to_change_password is not None:
             self._values["allow_user_to_change_password"] = allow_user_to_change_password
         if allow_user_to_manage_access_keys is not None:
             self._values["allow_user_to_manage_access_keys"] = allow_user_to_manage_access_keys
         if allow_user_to_manage_mfa_devices is not None:
             self._values["allow_user_to_manage_mfa_devices"] = allow_user_to_manage_mfa_devices
@@ -5458,49 +6034,55 @@
 ):
     '''A ROS resource type:  ``ALIYUN::RAM::User``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "UserProps",
+        props: typing.Union["UserProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::RAM::User``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(User.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCreateDate")
     def attr_create_date(self) -> ros_cdk_core.IResolvable:
         '''Attribute CreateDate: Create date of ram user.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCreateDate"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLastLoginDate")
     def attr_last_login_date(self) -> ros_cdk_core.IResolvable:
         '''Attribute LastLoginDate: Last login date of ram user.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLastLoginDate"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrUserId")
     def attr_user_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute UserId: Id of ram user.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrUserId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrUserName")
     def attr_user_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute UserName: Name of ram user.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrUserName"))
 
 
 @jsii.data_type(
@@ -5525,32 +6107,44 @@
         *,
         user_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         comments: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         deletion_force: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         display_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         email: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         groups: typing.Optional[typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable]] = None,
-        login_profile: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosUser.LoginProfileProperty]] = None,
+        login_profile: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosUser.LoginProfileProperty, typing.Dict[str, typing.Any]]]] = None,
         mobile_phone: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        policies: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosUser.PoliciesProperty]]]] = None,
-        policy_attachments: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosUser.PolicyAttachmentsProperty]] = None,
+        policies: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosUser.PoliciesProperty, typing.Dict[str, typing.Any]]]]]] = None,
+        policy_attachments: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosUser.PolicyAttachmentsProperty, typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::RAM::User``.
 
         :param user_name: Property userName: Specifies the user name, containing up to 64 characters.
         :param comments: Property comments: Comments of ram user.
         :param deletion_force: Property deletionForce: Whether force detach the policies and groups attached to the user. Default value is false.
         :param display_name: Property displayName: Display name, up to 128 characters or Chinese characters.
         :param email: Property email: Email of ram user.
         :param groups: Property groups: A name of a group to which you want to add the user.
         :param login_profile: Property loginProfile: Creates a login profile for users so that they can access the AliCloud Management Console.
         :param mobile_phone: Property mobilePhone: Phone number of ram user.
         :param policies: Property policies: Describes what actions are allowed on what resources.
         :param policy_attachments: Property policyAttachments: System and custom policy names to attach.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(UserProps.__init__)
+            check_type(argname="argument user_name", value=user_name, expected_type=type_hints["user_name"])
+            check_type(argname="argument comments", value=comments, expected_type=type_hints["comments"])
+            check_type(argname="argument deletion_force", value=deletion_force, expected_type=type_hints["deletion_force"])
+            check_type(argname="argument display_name", value=display_name, expected_type=type_hints["display_name"])
+            check_type(argname="argument email", value=email, expected_type=type_hints["email"])
+            check_type(argname="argument groups", value=groups, expected_type=type_hints["groups"])
+            check_type(argname="argument login_profile", value=login_profile, expected_type=type_hints["login_profile"])
+            check_type(argname="argument mobile_phone", value=mobile_phone, expected_type=type_hints["mobile_phone"])
+            check_type(argname="argument policies", value=policies, expected_type=type_hints["policies"])
+            check_type(argname="argument policy_attachments", value=policy_attachments, expected_type=type_hints["policy_attachments"])
         self._values: typing.Dict[str, typing.Any] = {
             "user_name": user_name,
         }
         if comments is not None:
             self._values["comments"] = comments
         if deletion_force is not None:
             self._values["deletion_force"] = deletion_force
@@ -5670,28 +6264,34 @@
 ):
     '''A ROS resource type:  ``ALIYUN::RAM::UserToGroupAddition``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "UserToGroupAdditionProps",
+        props: typing.Union["UserToGroupAdditionProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::RAM::UserToGroupAddition``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(UserToGroupAddition.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-ram.UserToGroupAdditionProps",
     jsii_struct_bases=[],
     name_mapping={"group_name": "groupName", "users": "users"},
@@ -5704,14 +6304,18 @@
         users: typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::RAM::UserToGroupAddition``.
 
         :param group_name: Property groupName: Specifies the group name, containing up to 64 characters.
         :param users: Property users: list name of a users to which you want to add the group.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(UserToGroupAdditionProps.__init__)
+            check_type(argname="argument group_name", value=group_name, expected_type=type_hints["group_name"])
+            check_type(argname="argument users", value=users, expected_type=type_hints["users"])
         self._values: typing.Dict[str, typing.Any] = {
             "group_name": group_name,
             "users": users,
         }
 
     @builtins.property
     def group_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
```

### Comparing `ros-cdk-ram-1.0.8/src/ros_cdk_ram.egg-info/PKG-INFO` & `ros-cdk-ram-1.0.9/src/ros_cdk_ram.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-ram
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS RAM Construct Library
```

