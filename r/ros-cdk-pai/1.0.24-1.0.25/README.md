# Comparing `tmp/ros-cdk-pai-1.0.24.tar.gz` & `tmp/ros-cdk-pai-1.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-pai-1.0.24.tar", last modified: Wed Apr 10 04:39:47 2024, max compression
+gzip compressed data, was "dist/ros-cdk-pai-1.0.25.tar", last modified: Mon Jun  3 10:32:02 2024, max compression
```

## Comparing `ros-cdk-pai-1.0.24.tar` & `ros-cdk-pai-1.0.25.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:39:47.000000 ros-cdk-pai-1.0.24/
--rw-r--r--   0 root         (0) root         (0)    10279 2024-04-10 04:39:47.000000 ros-cdk-pai-1.0.24/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-10 04:39:47.000000 ros-cdk-pai-1.0.24/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2024-04-10 04:39:47.000000 ros-cdk-pai-1.0.24/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1292 2024-04-10 04:39:47.000000 ros-cdk-pai-1.0.24/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      179 2024-04-10 04:39:47.000000 ros-cdk-pai-1.0.24/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2024-04-10 04:39:47.000000 ros-cdk-pai-1.0.24/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 04:39:47.000000 ros-cdk-pai-1.0.24/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1910 2024-04-10 04:39:47.000000 ros-cdk-pai-1.0.24/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:39:47.000000 ros-cdk-pai-1.0.24/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:39:47.000000 ros-cdk-pai-1.0.24/src/ros_cdk_pai/
--rw-r--r--   0 root         (0) root         (0)   136527 2024-04-10 04:39:47.000000 ros-cdk-pai-1.0.24/src/ros_cdk_pai/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:39:47.000000 ros-cdk-pai-1.0.24/src/ros_cdk_pai/_jsii/
--rw-r--r--   0 root         (0) root         (0)      406 2024-04-10 04:39:47.000000 ros-cdk-pai-1.0.24/src/ros_cdk_pai/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75506 2024-04-10 04:39:47.000000 ros-cdk-pai-1.0.24/src/ros_cdk_pai/_jsii/ros-cdk-pai@1.0.24.jsii.tgz
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:39:47.000000 ros-cdk-pai-1.0.24/src/ros_cdk_pai/datasource/
--rw-r--r--   0 root         (0) root         (0)    60610 2024-04-10 04:39:47.000000 ros-cdk-pai-1.0.24/src/ros_cdk_pai/datasource/__init__.py
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 04:39:47.000000 ros-cdk-pai-1.0.24/src/ros_cdk_pai/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:39:47.000000 ros-cdk-pai-1.0.24/src/ros_cdk_pai.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1292 2024-04-10 04:39:47.000000 ros-cdk-pai-1.0.24/src/ros_cdk_pai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2024-04-10 04:39:47.000000 ros-cdk-pai-1.0.24/src/ros_cdk_pai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 04:39:47.000000 ros-cdk-pai-1.0.24/src/ros_cdk_pai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      110 2024-04-10 04:39:47.000000 ros-cdk-pai-1.0.24/src/ros_cdk_pai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-04-10 04:39:47.000000 ros-cdk-pai-1.0.24/src/ros_cdk_pai.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 10:32:02.000000 ros-cdk-pai-1.0.25/
+-rw-r--r--   0 root         (0) root         (0)    10279 2024-06-03 10:32:02.000000 ros-cdk-pai-1.0.25/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2024-06-03 10:32:02.000000 ros-cdk-pai-1.0.25/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2024-06-03 10:32:02.000000 ros-cdk-pai-1.0.25/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1292 2024-06-03 10:32:02.000000 ros-cdk-pai-1.0.25/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      179 2024-06-03 10:32:02.000000 ros-cdk-pai-1.0.25/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2024-06-03 10:32:02.000000 ros-cdk-pai-1.0.25/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-06-03 10:32:02.000000 ros-cdk-pai-1.0.25/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1911 2024-06-03 10:32:02.000000 ros-cdk-pai-1.0.25/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 10:32:02.000000 ros-cdk-pai-1.0.25/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 10:32:02.000000 ros-cdk-pai-1.0.25/src/ros_cdk_pai/
+-rw-r--r--   0 root         (0) root         (0)   250477 2024-06-03 10:32:02.000000 ros-cdk-pai-1.0.25/src/ros_cdk_pai/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 10:32:02.000000 ros-cdk-pai-1.0.25/src/ros_cdk_pai/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      406 2024-06-03 10:32:02.000000 ros-cdk-pai-1.0.25/src/ros_cdk_pai/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    96112 2024-06-03 10:32:02.000000 ros-cdk-pai-1.0.25/src/ros_cdk_pai/_jsii/ros-cdk-pai@1.0.25.jsii.tgz
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 10:32:02.000000 ros-cdk-pai-1.0.25/src/ros_cdk_pai/datasource/
+-rw-r--r--   0 root         (0) root         (0)    60610 2024-06-03 10:32:02.000000 ros-cdk-pai-1.0.25/src/ros_cdk_pai/datasource/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 10:32:02.000000 ros-cdk-pai-1.0.25/src/ros_cdk_pai/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 10:32:02.000000 ros-cdk-pai-1.0.25/src/ros_cdk_pai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1292 2024-06-03 10:32:02.000000 ros-cdk-pai-1.0.25/src/ros_cdk_pai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2024-06-03 10:32:02.000000 ros-cdk-pai-1.0.25/src/ros_cdk_pai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 10:32:02.000000 ros-cdk-pai-1.0.25/src/ros_cdk_pai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      111 2024-06-03 10:32:02.000000 ros-cdk-pai-1.0.25/src/ros_cdk_pai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-06-03 10:32:02.000000 ros-cdk-pai-1.0.25/src/ros_cdk_pai.egg-info/top_level.txt
```

### Comparing `ros-cdk-pai-1.0.24/LICENSE` & `ros-cdk-pai-1.0.25/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-pai-1.0.24/PKG-INFO` & `ros-cdk-pai-1.0.25/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-pai
-Version: 1.0.24
+Version: 1.0.25
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS PAI Construct Library
```

### Comparing `ros-cdk-pai-1.0.24/setup.py` & `ros-cdk-pai-1.0.25/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-pai",
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
         "ros_cdk_pai",
         "ros_cdk_pai._jsii",
         "ros_cdk_pai.datasource"
     ],
     "package_data": {
         "ros_cdk_pai._jsii": [
-            "ros-cdk-pai@1.0.24.jsii.tgz"
+            "ros-cdk-pai@1.0.25.jsii.tgz"
         ],
         "ros_cdk_pai": [
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

### Comparing `ros-cdk-pai-1.0.24/src/ros_cdk_pai/__init__.py` & `ros-cdk-pai-1.0.25/src/ros_cdk_pai/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -2005,14 +2005,1348 @@
 
     def __repr__(self) -> str:
         return "RosWorkspaceProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
+class RosWorkspaceResourceDlc(
+    _ros_cdk_core_7adfd82f.RosResource,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@alicloud/ros-cdk-pai.RosWorkspaceResourceDlc",
+):
+    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::PAI::WorkspaceResourceDlc``.
+
+    :Note:
+
+    This class does not contain additional functions, so it is recommended to use the ``WorkspaceResourceDlc`` class instead of this class for a more convenient development experience.
+    See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-pai-workspaceresourcedlc
+    '''
+
+    def __init__(
+        self,
+        scope: _ros_cdk_core_7adfd82f.Construct,
+        id: builtins.str,
+        props: typing.Union["RosWorkspaceResourceDlcProps", typing.Dict[builtins.str, typing.Any]],
+        enable_resource_property_constraint: builtins.bool,
+    ) -> None:
+        '''
+        :param scope: - scope in which this resource is defined.
+        :param id: - scoped id of the resource.
+        :param props: - resource properties.
+        :param enable_resource_property_constraint: -
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__ea471a7c5a468bef4fbe3da7e68f4dc188887b43f7aa5af028489e058c6bb75c)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
+        jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
+
+    @jsii.member(jsii_name="renderProperties")
+    def _render_properties(
+        self,
+        props: typing.Mapping[builtins.str, typing.Any],
+    ) -> typing.Mapping[builtins.str, typing.Any]:
+        '''
+        :param props: -
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__880f6f3ac266a1fb510823f94b53f269bb495e4fe76e18aaf23b873fb85cbc54)
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+        return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.invoke(self, "renderProperties", [props]))
+
+    @jsii.python.classproperty
+    @jsii.member(jsii_name="ROS_RESOURCE_TYPE_NAME")
+    def ROS_RESOURCE_TYPE_NAME(cls) -> builtins.str:
+        '''The resource type name for this resource class.'''
+        return typing.cast(builtins.str, jsii.sget(cls, "ROS_RESOURCE_TYPE_NAME"))
+
+    @builtins.property
+    @jsii.member(jsii_name="attrCreateTime")
+    def attr_create_time(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+        '''
+        :Attribute: CreateTime: The creation time of the resource.
+        '''
+        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrCreateTime"))
+
+    @builtins.property
+    @jsii.member(jsii_name="attrGroupName")
+    def attr_group_name(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+        '''
+        :Attribute: GroupName: Resource group name. If you want to obtain a resource group name, see [ListResources].
+        '''
+        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrGroupName"))
+
+    @builtins.property
+    @jsii.member(jsii_name="attrIsDefault")
+    def attr_is_default(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+        '''
+        :Attribute: IsDefault: Indicates whether it is the default resource. Currently, this parameter only supports the input of true and does not support false.
+        '''
+        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrIsDefault"))
+
+    @builtins.property
+    @jsii.member(jsii_name="attrResources")
+    def attr_resources(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+        '''
+        :Attribute: Resources: Resource List.
+        '''
+        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrResources"))
+
+    @builtins.property
+    @jsii.member(jsii_name="rosProperties")
+    def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
+        return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
+
+    @builtins.property
+    @jsii.member(jsii_name="enableResourcePropertyConstraint")
+    def enable_resource_property_constraint(self) -> builtins.bool:
+        return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
+
+    @enable_resource_property_constraint.setter
+    def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__bd53872479e3c25b6c5bf40f49be3c3142ce169ab5c654cc83d020869026da40)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "enableResourcePropertyConstraint", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="groupName")
+    def group_name(
+        self,
+    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''
+        :Property: groupName: Resource group name. If you want to obtain a resource group name, see [ListResources].
+        '''
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], jsii.get(self, "groupName"))
+
+    @group_name.setter
+    def group_name(
+        self,
+        value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__62ffc6de5eef8f8c7deb4bd47fba77afaf8f75da950cb755ea9749786bce401a)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "groupName", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="resources")
+    def resources(
+        self,
+    ) -> typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, "RosWorkspaceResourceDlc.ResourcesProperty"]]]:
+        '''
+        :Property: resources: Resource List.
+        '''
+        return typing.cast(typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, "RosWorkspaceResourceDlc.ResourcesProperty"]]], jsii.get(self, "resources"))
+
+    @resources.setter
+    def resources(
+        self,
+        value: typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, "RosWorkspaceResourceDlc.ResourcesProperty"]]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__851f8fec11054543e2700b9f4236d062bd022ebdabab1932c9f76df752b554b1)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "resources", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="workspaceId")
+    def workspace_id(
+        self,
+    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''
+        :Property: workspaceId: The ID of the workspace to which the workspace belongs.
+        '''
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], jsii.get(self, "workspaceId"))
+
+    @workspace_id.setter
+    def workspace_id(
+        self,
+        value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__a02cb6e32cd7d71600381b6de6c52bbc9c54c46998d1cbdc7e053603a61b038a)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "workspaceId", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="isDefault")
+    def is_default(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''
+        :Property: isDefault: Indicates whether it is the default resource. Currently, this parameter only supports the input of true and does not support false.
+        '''
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "isDefault"))
+
+    @is_default.setter
+    def is_default(
+        self,
+        value: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__3cd28cac9cfc4c04e9236d83f6baa1a2bc767cb752186ebc1640ea0573ff31a6)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "isDefault", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="option")
+    def option(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''
+        :Property:
+
+        option: Create behavior that supports the following values:
+
+        - CreateAndAttach: Create resource and bind to workspace
+        - Attach: bind resource to workspace.
+        '''
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "option"))
+
+    @option.setter
+    def option(
+        self,
+        value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__c2278990b8b85d56ab86bac7c23b334be02aadfa5eaf74feaaa2c38216caae21)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "option", value)
+
+    @jsii.data_type(
+        jsii_type="@alicloud/ros-cdk-pai.RosWorkspaceResourceDlc.ResourcesProperty",
+        jsii_struct_bases=[],
+        name_mapping={
+            "env_type": "envType",
+            "workspace_resource_name": "workspaceResourceName",
+            "workspace_resource_workspace_id": "workspaceResourceWorkspaceId",
+            "spec": "spec",
+        },
+    )
+    class ResourcesProperty:
+        def __init__(
+            self,
+            *,
+            env_type: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+            workspace_resource_name: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+            workspace_resource_workspace_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+            spec: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Mapping[builtins.str, typing.Any]]] = None,
+        ) -> None:
+            '''
+            :param env_type: 
+            :param workspace_resource_name: 
+            :param workspace_resource_workspace_id: 
+            :param spec: 
+            '''
+            if __debug__:
+                type_hints = typing.get_type_hints(_typecheckingstub__3b63c737a049056c6be56bdb83efec08ab424dc639b21a4ad5124e241f87be64)
+                check_type(argname="argument env_type", value=env_type, expected_type=type_hints["env_type"])
+                check_type(argname="argument workspace_resource_name", value=workspace_resource_name, expected_type=type_hints["workspace_resource_name"])
+                check_type(argname="argument workspace_resource_workspace_id", value=workspace_resource_workspace_id, expected_type=type_hints["workspace_resource_workspace_id"])
+                check_type(argname="argument spec", value=spec, expected_type=type_hints["spec"])
+            self._values: typing.Dict[builtins.str, typing.Any] = {
+                "env_type": env_type,
+                "workspace_resource_name": workspace_resource_name,
+                "workspace_resource_workspace_id": workspace_resource_workspace_id,
+            }
+            if spec is not None:
+                self._values["spec"] = spec
+
+        @builtins.property
+        def env_type(
+            self,
+        ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+            '''
+            :Property:
+
+            envType: Environment, Support:
+
+            - dev: Development
+            - prod: Production.
+            '''
+            result = self._values.get("env_type")
+            assert result is not None, "Required property 'env_type' is missing"
+            return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+        @builtins.property
+        def workspace_resource_name(
+            self,
+        ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+            '''
+            :Property: workspaceResourceName: Resource name, 3 to 28 characters in length, unique within each locale. Starts with the required letter and can contain only letters, numbers, and underscores (_).
+            '''
+            result = self._values.get("workspace_resource_name")
+            assert result is not None, "Required property 'workspace_resource_name' is missing"
+            return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+        @builtins.property
+        def workspace_resource_workspace_id(
+            self,
+        ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+            '''
+            :Property: workspaceResourceWorkspaceId: ID of the workspace to which the resource information belongs.
+            '''
+            result = self._values.get("workspace_resource_workspace_id")
+            assert result is not None, "Required property 'workspace_resource_workspace_id' is missing"
+            return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+        @builtins.property
+        def spec(
+            self,
+        ) -> typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Mapping[builtins.str, typing.Any]]]:
+            '''
+            :Property: spec: Resource Specifications.
+            '''
+            result = self._values.get("spec")
+            return typing.cast(typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Mapping[builtins.str, typing.Any]]], result)
+
+        def __eq__(self, rhs: typing.Any) -> builtins.bool:
+            return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+        def __ne__(self, rhs: typing.Any) -> builtins.bool:
+            return not (rhs == self)
+
+        def __repr__(self) -> str:
+            return "ResourcesProperty(%s)" % ", ".join(
+                k + "=" + repr(v) for k, v in self._values.items()
+            )
+
+
+@jsii.data_type(
+    jsii_type="@alicloud/ros-cdk-pai.RosWorkspaceResourceDlcProps",
+    jsii_struct_bases=[],
+    name_mapping={
+        "group_name": "groupName",
+        "resources": "resources",
+        "workspace_id": "workspaceId",
+        "is_default": "isDefault",
+        "option": "option",
+    },
+)
+class RosWorkspaceResourceDlcProps:
+    def __init__(
+        self,
+        *,
+        group_name: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+        resources: typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Sequence[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Union[RosWorkspaceResourceDlc.ResourcesProperty, typing.Dict[builtins.str, typing.Any]]]]],
+        workspace_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+        is_default: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+        option: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    ) -> None:
+        '''Properties for defining a ``RosWorkspaceResourceDlc``.
+
+        See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-pai-workspaceresourcedlc
+
+        :param group_name: 
+        :param resources: 
+        :param workspace_id: 
+        :param is_default: 
+        :param option: 
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__ebe3af48413265457d30902f743d3ada3ff1f69c0081c3fe7bf7d63bc0a3ca88)
+            check_type(argname="argument group_name", value=group_name, expected_type=type_hints["group_name"])
+            check_type(argname="argument resources", value=resources, expected_type=type_hints["resources"])
+            check_type(argname="argument workspace_id", value=workspace_id, expected_type=type_hints["workspace_id"])
+            check_type(argname="argument is_default", value=is_default, expected_type=type_hints["is_default"])
+            check_type(argname="argument option", value=option, expected_type=type_hints["option"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "group_name": group_name,
+            "resources": resources,
+            "workspace_id": workspace_id,
+        }
+        if is_default is not None:
+            self._values["is_default"] = is_default
+        if option is not None:
+            self._values["option"] = option
+
+    @builtins.property
+    def group_name(
+        self,
+    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''
+        :Property: groupName: Resource group name. If you want to obtain a resource group name, see [ListResources].
+        '''
+        result = self._values.get("group_name")
+        assert result is not None, "Required property 'group_name' is missing"
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+    @builtins.property
+    def resources(
+        self,
+    ) -> typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, RosWorkspaceResourceDlc.ResourcesProperty]]]:
+        '''
+        :Property: resources: Resource List.
+        '''
+        result = self._values.get("resources")
+        assert result is not None, "Required property 'resources' is missing"
+        return typing.cast(typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, RosWorkspaceResourceDlc.ResourcesProperty]]], result)
+
+    @builtins.property
+    def workspace_id(
+        self,
+    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''
+        :Property: workspaceId: The ID of the workspace to which the workspace belongs.
+        '''
+        result = self._values.get("workspace_id")
+        assert result is not None, "Required property 'workspace_id' is missing"
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+    @builtins.property
+    def is_default(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''
+        :Property: isDefault: Indicates whether it is the default resource. Currently, this parameter only supports the input of true and does not support false.
+        '''
+        result = self._values.get("is_default")
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+    @builtins.property
+    def option(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''
+        :Property:
+
+        option: Create behavior that supports the following values:
+
+        - CreateAndAttach: Create resource and bind to workspace
+        - Attach: bind resource to workspace.
+        '''
+        result = self._values.get("option")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "RosWorkspaceResourceDlcProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+class RosWorkspaceResourceFlink(
+    _ros_cdk_core_7adfd82f.RosResource,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@alicloud/ros-cdk-pai.RosWorkspaceResourceFlink",
+):
+    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::PAI::WorkspaceResourceFlink``.
+
+    :Note:
+
+    This class does not contain additional functions, so it is recommended to use the ``WorkspaceResourceFlink`` class instead of this class for a more convenient development experience.
+    See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-pai-workspaceresourceflink
+    '''
+
+    def __init__(
+        self,
+        scope: _ros_cdk_core_7adfd82f.Construct,
+        id: builtins.str,
+        props: typing.Union["RosWorkspaceResourceFlinkProps", typing.Dict[builtins.str, typing.Any]],
+        enable_resource_property_constraint: builtins.bool,
+    ) -> None:
+        '''
+        :param scope: - scope in which this resource is defined.
+        :param id: - scoped id of the resource.
+        :param props: - resource properties.
+        :param enable_resource_property_constraint: -
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__578e83686f72937307c5eaff49925ac4609f7af1a907878ecbfa0a2f841c738a)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
+        jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
+
+    @jsii.member(jsii_name="renderProperties")
+    def _render_properties(
+        self,
+        props: typing.Mapping[builtins.str, typing.Any],
+    ) -> typing.Mapping[builtins.str, typing.Any]:
+        '''
+        :param props: -
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__50e901a2952ba52b6a10bc49b7e5b3189d80075f43b1e615ae6e13998ef08ad7)
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+        return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.invoke(self, "renderProperties", [props]))
+
+    @jsii.python.classproperty
+    @jsii.member(jsii_name="ROS_RESOURCE_TYPE_NAME")
+    def ROS_RESOURCE_TYPE_NAME(cls) -> builtins.str:
+        '''The resource type name for this resource class.'''
+        return typing.cast(builtins.str, jsii.sget(cls, "ROS_RESOURCE_TYPE_NAME"))
+
+    @builtins.property
+    @jsii.member(jsii_name="attrCreateTime")
+    def attr_create_time(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+        '''
+        :Attribute: CreateTime: The creation time of the resource.
+        '''
+        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrCreateTime"))
+
+    @builtins.property
+    @jsii.member(jsii_name="attrGroupName")
+    def attr_group_name(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+        '''
+        :Attribute: GroupName: Resource group name. If you want to obtain a resource group name, see [ListResources](~~ 449143 ~~).
+        '''
+        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrGroupName"))
+
+    @builtins.property
+    @jsii.member(jsii_name="attrIsDefault")
+    def attr_is_default(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+        '''
+        :Attribute: IsDefault: Indicates whether it is the default resource. Currently, this parameter only supports the input of true and does not support false.
+        '''
+        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrIsDefault"))
+
+    @builtins.property
+    @jsii.member(jsii_name="attrResources")
+    def attr_resources(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+        '''
+        :Attribute: Resources: Resource List.
+        '''
+        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrResources"))
+
+    @builtins.property
+    @jsii.member(jsii_name="rosProperties")
+    def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
+        return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
+
+    @builtins.property
+    @jsii.member(jsii_name="enableResourcePropertyConstraint")
+    def enable_resource_property_constraint(self) -> builtins.bool:
+        return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
+
+    @enable_resource_property_constraint.setter
+    def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__9d1c9fa6b40ab37ba09aef6151f1e66e229d437080ed99bb6cf8089e85fd86c1)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "enableResourcePropertyConstraint", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="groupName")
+    def group_name(
+        self,
+    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''
+        :Property: groupName: Resource group name. If you want to obtain a resource group name, see [ListResources].
+        '''
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], jsii.get(self, "groupName"))
+
+    @group_name.setter
+    def group_name(
+        self,
+        value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__ca323975d7fc5f1d16a657130dc599c4f908c298b936a0d169d12df4d844e558)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "groupName", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="resources")
+    def resources(
+        self,
+    ) -> typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, "RosWorkspaceResourceFlink.ResourcesProperty"]]]:
+        '''
+        :Property: resources: Resource List.
+        '''
+        return typing.cast(typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, "RosWorkspaceResourceFlink.ResourcesProperty"]]], jsii.get(self, "resources"))
+
+    @resources.setter
+    def resources(
+        self,
+        value: typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, "RosWorkspaceResourceFlink.ResourcesProperty"]]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__79dfa340d3c04d62dab1f2e4805ac4e24350f4232085e4080aead4afee0fefe4)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "resources", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="workspaceId")
+    def workspace_id(
+        self,
+    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''
+        :Property: workspaceId: The ID of the workspace to which the workspace belongs.
+        '''
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], jsii.get(self, "workspaceId"))
+
+    @workspace_id.setter
+    def workspace_id(
+        self,
+        value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__d2fdbf156aa98caf320eedfe08a20588da72a316c3be60f39a2c78dcf88f9304)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "workspaceId", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="isDefault")
+    def is_default(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''
+        :Property: isDefault: Indicates whether it is the default resource. Currently, this parameter only supports the input of true and does not support false.
+        '''
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "isDefault"))
+
+    @is_default.setter
+    def is_default(
+        self,
+        value: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__d7df214b7927ddd30a219d7422b60c2669d86f9096b9ad198de745404e3a3e06)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "isDefault", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="option")
+    def option(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''
+        :Property:
+
+        option: Create behavior that supports the following values:
+
+        - CreateAndAttach: Create resource and bind to workspace
+        - Attach: bind resource to workspace.
+        '''
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "option"))
+
+    @option.setter
+    def option(
+        self,
+        value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__d6cfa95eb1a0fc9d5a6cf49da807d4d6154105dfd0ad6ebc8d1ec394a59961ac)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "option", value)
+
+    @jsii.data_type(
+        jsii_type="@alicloud/ros-cdk-pai.RosWorkspaceResourceFlink.ResourcesProperty",
+        jsii_struct_bases=[],
+        name_mapping={
+            "env_type": "envType",
+            "workspace_resource_name": "workspaceResourceName",
+            "workspace_resource_workspace_id": "workspaceResourceWorkspaceId",
+            "spec": "spec",
+        },
+    )
+    class ResourcesProperty:
+        def __init__(
+            self,
+            *,
+            env_type: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+            workspace_resource_name: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+            workspace_resource_workspace_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+            spec: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Mapping[builtins.str, typing.Any]]] = None,
+        ) -> None:
+            '''
+            :param env_type: 
+            :param workspace_resource_name: 
+            :param workspace_resource_workspace_id: 
+            :param spec: 
+            '''
+            if __debug__:
+                type_hints = typing.get_type_hints(_typecheckingstub__89ca36c747cdfe0629d41004d514da825f4cecde19a50efd3dad85f13cc21e5d)
+                check_type(argname="argument env_type", value=env_type, expected_type=type_hints["env_type"])
+                check_type(argname="argument workspace_resource_name", value=workspace_resource_name, expected_type=type_hints["workspace_resource_name"])
+                check_type(argname="argument workspace_resource_workspace_id", value=workspace_resource_workspace_id, expected_type=type_hints["workspace_resource_workspace_id"])
+                check_type(argname="argument spec", value=spec, expected_type=type_hints["spec"])
+            self._values: typing.Dict[builtins.str, typing.Any] = {
+                "env_type": env_type,
+                "workspace_resource_name": workspace_resource_name,
+                "workspace_resource_workspace_id": workspace_resource_workspace_id,
+            }
+            if spec is not None:
+                self._values["spec"] = spec
+
+        @builtins.property
+        def env_type(
+            self,
+        ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+            '''
+            :Property:
+
+            envType: Environment, Support:
+
+            - dev: Development
+            - prod: Production.
+            '''
+            result = self._values.get("env_type")
+            assert result is not None, "Required property 'env_type' is missing"
+            return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+        @builtins.property
+        def workspace_resource_name(
+            self,
+        ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+            '''
+            :Property: workspaceResourceName: Resource name, 3 to 28 characters in length, unique within each locale. Starts with the required letter and can contain only letters, numbers, and underscores (_).
+            '''
+            result = self._values.get("workspace_resource_name")
+            assert result is not None, "Required property 'workspace_resource_name' is missing"
+            return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+        @builtins.property
+        def workspace_resource_workspace_id(
+            self,
+        ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+            '''
+            :Property: workspaceResourceWorkspaceId: ID of the workspace to which the resource information belongs.
+            '''
+            result = self._values.get("workspace_resource_workspace_id")
+            assert result is not None, "Required property 'workspace_resource_workspace_id' is missing"
+            return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+        @builtins.property
+        def spec(
+            self,
+        ) -> typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Mapping[builtins.str, typing.Any]]]:
+            '''
+            :Property: spec: Resource Specifications.
+            '''
+            result = self._values.get("spec")
+            return typing.cast(typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Mapping[builtins.str, typing.Any]]], result)
+
+        def __eq__(self, rhs: typing.Any) -> builtins.bool:
+            return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+        def __ne__(self, rhs: typing.Any) -> builtins.bool:
+            return not (rhs == self)
+
+        def __repr__(self) -> str:
+            return "ResourcesProperty(%s)" % ", ".join(
+                k + "=" + repr(v) for k, v in self._values.items()
+            )
+
+
+@jsii.data_type(
+    jsii_type="@alicloud/ros-cdk-pai.RosWorkspaceResourceFlinkProps",
+    jsii_struct_bases=[],
+    name_mapping={
+        "group_name": "groupName",
+        "resources": "resources",
+        "workspace_id": "workspaceId",
+        "is_default": "isDefault",
+        "option": "option",
+    },
+)
+class RosWorkspaceResourceFlinkProps:
+    def __init__(
+        self,
+        *,
+        group_name: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+        resources: typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Sequence[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Union[RosWorkspaceResourceFlink.ResourcesProperty, typing.Dict[builtins.str, typing.Any]]]]],
+        workspace_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+        is_default: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+        option: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    ) -> None:
+        '''Properties for defining a ``RosWorkspaceResourceFlink``.
+
+        See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-pai-workspaceresourceflink
+
+        :param group_name: 
+        :param resources: 
+        :param workspace_id: 
+        :param is_default: 
+        :param option: 
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__57bfe40c04abe5e6fe19e91814ee8956f205f1f3fa2b27ecfbe7b2f455a8f03e)
+            check_type(argname="argument group_name", value=group_name, expected_type=type_hints["group_name"])
+            check_type(argname="argument resources", value=resources, expected_type=type_hints["resources"])
+            check_type(argname="argument workspace_id", value=workspace_id, expected_type=type_hints["workspace_id"])
+            check_type(argname="argument is_default", value=is_default, expected_type=type_hints["is_default"])
+            check_type(argname="argument option", value=option, expected_type=type_hints["option"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "group_name": group_name,
+            "resources": resources,
+            "workspace_id": workspace_id,
+        }
+        if is_default is not None:
+            self._values["is_default"] = is_default
+        if option is not None:
+            self._values["option"] = option
+
+    @builtins.property
+    def group_name(
+        self,
+    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''
+        :Property: groupName: Resource group name. If you want to obtain a resource group name, see [ListResources].
+        '''
+        result = self._values.get("group_name")
+        assert result is not None, "Required property 'group_name' is missing"
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+    @builtins.property
+    def resources(
+        self,
+    ) -> typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, RosWorkspaceResourceFlink.ResourcesProperty]]]:
+        '''
+        :Property: resources: Resource List.
+        '''
+        result = self._values.get("resources")
+        assert result is not None, "Required property 'resources' is missing"
+        return typing.cast(typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, RosWorkspaceResourceFlink.ResourcesProperty]]], result)
+
+    @builtins.property
+    def workspace_id(
+        self,
+    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''
+        :Property: workspaceId: The ID of the workspace to which the workspace belongs.
+        '''
+        result = self._values.get("workspace_id")
+        assert result is not None, "Required property 'workspace_id' is missing"
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+    @builtins.property
+    def is_default(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''
+        :Property: isDefault: Indicates whether it is the default resource. Currently, this parameter only supports the input of true and does not support false.
+        '''
+        result = self._values.get("is_default")
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+    @builtins.property
+    def option(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''
+        :Property:
+
+        option: Create behavior that supports the following values:
+
+        - CreateAndAttach: Create resource and bind to workspace
+        - Attach: bind resource to workspace.
+        '''
+        result = self._values.get("option")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "RosWorkspaceResourceFlinkProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+class RosWorkspaceResourceMaxCompute(
+    _ros_cdk_core_7adfd82f.RosResource,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@alicloud/ros-cdk-pai.RosWorkspaceResourceMaxCompute",
+):
+    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::PAI::WorkspaceResourceMaxCompute``.
+
+    :Note:
+
+    This class does not contain additional functions, so it is recommended to use the ``WorkspaceResourceMaxCompute`` class instead of this class for a more convenient development experience.
+    See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-pai-workspaceresourcemaxcompute
+    '''
+
+    def __init__(
+        self,
+        scope: _ros_cdk_core_7adfd82f.Construct,
+        id: builtins.str,
+        props: typing.Union["RosWorkspaceResourceMaxComputeProps", typing.Dict[builtins.str, typing.Any]],
+        enable_resource_property_constraint: builtins.bool,
+    ) -> None:
+        '''
+        :param scope: - scope in which this resource is defined.
+        :param id: - scoped id of the resource.
+        :param props: - resource properties.
+        :param enable_resource_property_constraint: -
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__b2f66acdef9422d08230176a5b72b7f5ffcd09e7423e28e62bfae4e5ebb3d1e8)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
+        jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
+
+    @jsii.member(jsii_name="renderProperties")
+    def _render_properties(
+        self,
+        props: typing.Mapping[builtins.str, typing.Any],
+    ) -> typing.Mapping[builtins.str, typing.Any]:
+        '''
+        :param props: -
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__b0915637f1ed1f6490dc4cf208d921579edb493622a7a2aacf5c07188c363642)
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+        return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.invoke(self, "renderProperties", [props]))
+
+    @jsii.python.classproperty
+    @jsii.member(jsii_name="ROS_RESOURCE_TYPE_NAME")
+    def ROS_RESOURCE_TYPE_NAME(cls) -> builtins.str:
+        '''The resource type name for this resource class.'''
+        return typing.cast(builtins.str, jsii.sget(cls, "ROS_RESOURCE_TYPE_NAME"))
+
+    @builtins.property
+    @jsii.member(jsii_name="attrCreateTime")
+    def attr_create_time(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+        '''
+        :Attribute: CreateTime: The creation time of the resource.
+        '''
+        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrCreateTime"))
+
+    @builtins.property
+    @jsii.member(jsii_name="attrGroupName")
+    def attr_group_name(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+        '''
+        :Attribute: GroupName: Resource group name. If you want to obtain a resource group name, see [ListResources](~~ 449143 ~~).
+        '''
+        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrGroupName"))
+
+    @builtins.property
+    @jsii.member(jsii_name="attrIsDefault")
+    def attr_is_default(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+        '''
+        :Attribute: IsDefault: Indicates whether it is the default resource. Currently, this parameter only supports the input of true and does not support false.
+        '''
+        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrIsDefault"))
+
+    @builtins.property
+    @jsii.member(jsii_name="attrResources")
+    def attr_resources(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+        '''
+        :Attribute: Resources: Resource List.
+        '''
+        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrResources"))
+
+    @builtins.property
+    @jsii.member(jsii_name="rosProperties")
+    def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
+        return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
+
+    @builtins.property
+    @jsii.member(jsii_name="enableResourcePropertyConstraint")
+    def enable_resource_property_constraint(self) -> builtins.bool:
+        return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
+
+    @enable_resource_property_constraint.setter
+    def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__3e020f1431efd6202810928f260ad1f7a6cc98c572186a0974c23d9be1f39231)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "enableResourcePropertyConstraint", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="groupName")
+    def group_name(
+        self,
+    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''
+        :Property: groupName: Resource group name. If you want to obtain a resource group name.
+        '''
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], jsii.get(self, "groupName"))
+
+    @group_name.setter
+    def group_name(
+        self,
+        value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__9201de5fa777a55754433585aef86290a7eea5e417e3c4e366351d8324b5af9c)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "groupName", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="resources")
+    def resources(
+        self,
+    ) -> typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, "RosWorkspaceResourceMaxCompute.ResourcesProperty"]]]:
+        '''
+        :Property: resources: Resource List.
+        '''
+        return typing.cast(typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, "RosWorkspaceResourceMaxCompute.ResourcesProperty"]]], jsii.get(self, "resources"))
+
+    @resources.setter
+    def resources(
+        self,
+        value: typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, "RosWorkspaceResourceMaxCompute.ResourcesProperty"]]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__04ea2d9563b588f5231d2d9c450110738c227aa293b3544800dcea6316ead8ce)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "resources", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="workspaceId")
+    def workspace_id(
+        self,
+    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''
+        :Property: workspaceId: The ID of the workspace to which the workspace belongs.
+        '''
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], jsii.get(self, "workspaceId"))
+
+    @workspace_id.setter
+    def workspace_id(
+        self,
+        value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__7395f30834464169f2d941232a6f6ab2de6666ef318e4b0ddda3ef3536bc45fe)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "workspaceId", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="isDefault")
+    def is_default(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''
+        :Property: isDefault: Indicates whether it is the default resource. Currently, this parameter only supports the input of true and does not support false.
+        '''
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "isDefault"))
+
+    @is_default.setter
+    def is_default(
+        self,
+        value: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__ea06bb30d84c99805226cf5f24f9bb434100e07f7513660da1d08ca7cd5a0ce4)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "isDefault", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="option")
+    def option(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''
+        :Property:
+
+        option: Create behavior that supports the following values:
+
+        - CreateAndAttach: Create resource and bind to workspace
+        - Attach: bind resource to workspace.
+        '''
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "option"))
+
+    @option.setter
+    def option(
+        self,
+        value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__78300066522bbb82d6f5389c93bb95b7b0ddf71df2b55fdbc95b90ffa6677d28)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "option", value)
+
+    @jsii.data_type(
+        jsii_type="@alicloud/ros-cdk-pai.RosWorkspaceResourceMaxCompute.QuotasProperty",
+        jsii_struct_bases=[],
+        name_mapping={"quota_id": "quotaId"},
+    )
+    class QuotasProperty:
+        def __init__(
+            self,
+            *,
+            quota_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+        ) -> None:
+            '''
+            :param quota_id: 
+            '''
+            if __debug__:
+                type_hints = typing.get_type_hints(_typecheckingstub__a70ae00332f2bfed57c993bdf06e7efc8435125887165aa32a8edcb286a675d1)
+                check_type(argname="argument quota_id", value=quota_id, expected_type=type_hints["quota_id"])
+            self._values: typing.Dict[builtins.str, typing.Any] = {
+                "quota_id": quota_id,
+            }
+
+        @builtins.property
+        def quota_id(
+            self,
+        ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+            '''
+            :Property:
+
+            quotaId: The resource quota ID.
+            Obtain the ID of the Quota through ListQuotas.
+            '''
+            result = self._values.get("quota_id")
+            assert result is not None, "Required property 'quota_id' is missing"
+            return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+        def __eq__(self, rhs: typing.Any) -> builtins.bool:
+            return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+        def __ne__(self, rhs: typing.Any) -> builtins.bool:
+            return not (rhs == self)
+
+        def __repr__(self) -> str:
+            return "QuotasProperty(%s)" % ", ".join(
+                k + "=" + repr(v) for k, v in self._values.items()
+            )
+
+    @jsii.data_type(
+        jsii_type="@alicloud/ros-cdk-pai.RosWorkspaceResourceMaxCompute.ResourcesProperty",
+        jsii_struct_bases=[],
+        name_mapping={
+            "env_type": "envType",
+            "workspace_resource_name": "workspaceResourceName",
+            "workspace_resource_workspace_id": "workspaceResourceWorkspaceId",
+            "quotas": "quotas",
+            "spec": "spec",
+        },
+    )
+    class ResourcesProperty:
+        def __init__(
+            self,
+            *,
+            env_type: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+            workspace_resource_name: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+            workspace_resource_workspace_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+            quotas: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Sequence[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Union["RosWorkspaceResourceMaxCompute.QuotasProperty", typing.Dict[builtins.str, typing.Any]]]]]] = None,
+            spec: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Mapping[builtins.str, typing.Any]]] = None,
+        ) -> None:
+            '''
+            :param env_type: 
+            :param workspace_resource_name: 
+            :param workspace_resource_workspace_id: 
+            :param quotas: 
+            :param spec: 
+            '''
+            if __debug__:
+                type_hints = typing.get_type_hints(_typecheckingstub__6957cb7eb7fe278e12e47aee5f6cd93edb8f6a9976848a38f6ab123bd66380b6)
+                check_type(argname="argument env_type", value=env_type, expected_type=type_hints["env_type"])
+                check_type(argname="argument workspace_resource_name", value=workspace_resource_name, expected_type=type_hints["workspace_resource_name"])
+                check_type(argname="argument workspace_resource_workspace_id", value=workspace_resource_workspace_id, expected_type=type_hints["workspace_resource_workspace_id"])
+                check_type(argname="argument quotas", value=quotas, expected_type=type_hints["quotas"])
+                check_type(argname="argument spec", value=spec, expected_type=type_hints["spec"])
+            self._values: typing.Dict[builtins.str, typing.Any] = {
+                "env_type": env_type,
+                "workspace_resource_name": workspace_resource_name,
+                "workspace_resource_workspace_id": workspace_resource_workspace_id,
+            }
+            if quotas is not None:
+                self._values["quotas"] = quotas
+            if spec is not None:
+                self._values["spec"] = spec
+
+        @builtins.property
+        def env_type(
+            self,
+        ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+            '''
+            :Property:
+
+            envType: Environment, Support:
+
+            - dev: Development
+            - prod: Production.
+            '''
+            result = self._values.get("env_type")
+            assert result is not None, "Required property 'env_type' is missing"
+            return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+        @builtins.property
+        def workspace_resource_name(
+            self,
+        ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+            '''
+            :Property: workspaceResourceName: Resource name, 3 to 28 characters in length, unique within each locale. Starts with the required letter and can contain only letters, numbers, and underscores (_).
+            '''
+            result = self._values.get("workspace_resource_name")
+            assert result is not None, "Required property 'workspace_resource_name' is missing"
+            return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+        @builtins.property
+        def workspace_resource_workspace_id(
+            self,
+        ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+            '''
+            :Property: workspaceResourceWorkspaceId: ID of the workspace to which the resource information belongs.
+            '''
+            result = self._values.get("workspace_resource_workspace_id")
+            assert result is not None, "Required property 'workspace_resource_workspace_id' is missing"
+            return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+        @builtins.property
+        def quotas(
+            self,
+        ) -> typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, "RosWorkspaceResourceMaxCompute.QuotasProperty"]]]]:
+            '''
+            :Property: quotas: The list of resource quotas. Currently, only MaxCompute resources have resource quotas.
+            '''
+            result = self._values.get("quotas")
+            return typing.cast(typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, "RosWorkspaceResourceMaxCompute.QuotasProperty"]]]], result)
+
+        @builtins.property
+        def spec(
+            self,
+        ) -> typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Mapping[builtins.str, typing.Any]]]:
+            '''
+            :Property: spec: Resource Specifications.
+            '''
+            result = self._values.get("spec")
+            return typing.cast(typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Mapping[builtins.str, typing.Any]]], result)
+
+        def __eq__(self, rhs: typing.Any) -> builtins.bool:
+            return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+        def __ne__(self, rhs: typing.Any) -> builtins.bool:
+            return not (rhs == self)
+
+        def __repr__(self) -> str:
+            return "ResourcesProperty(%s)" % ", ".join(
+                k + "=" + repr(v) for k, v in self._values.items()
+            )
+
+
+@jsii.data_type(
+    jsii_type="@alicloud/ros-cdk-pai.RosWorkspaceResourceMaxComputeProps",
+    jsii_struct_bases=[],
+    name_mapping={
+        "group_name": "groupName",
+        "resources": "resources",
+        "workspace_id": "workspaceId",
+        "is_default": "isDefault",
+        "option": "option",
+    },
+)
+class RosWorkspaceResourceMaxComputeProps:
+    def __init__(
+        self,
+        *,
+        group_name: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+        resources: typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Sequence[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Union[RosWorkspaceResourceMaxCompute.ResourcesProperty, typing.Dict[builtins.str, typing.Any]]]]],
+        workspace_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+        is_default: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+        option: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    ) -> None:
+        '''Properties for defining a ``RosWorkspaceResourceMaxCompute``.
+
+        See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-pai-workspaceresourcemaxcompute
+
+        :param group_name: 
+        :param resources: 
+        :param workspace_id: 
+        :param is_default: 
+        :param option: 
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__79d876bae6e4a2d418971fcf603e4262414b3c2431be6929353adf44d387cdb3)
+            check_type(argname="argument group_name", value=group_name, expected_type=type_hints["group_name"])
+            check_type(argname="argument resources", value=resources, expected_type=type_hints["resources"])
+            check_type(argname="argument workspace_id", value=workspace_id, expected_type=type_hints["workspace_id"])
+            check_type(argname="argument is_default", value=is_default, expected_type=type_hints["is_default"])
+            check_type(argname="argument option", value=option, expected_type=type_hints["option"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "group_name": group_name,
+            "resources": resources,
+            "workspace_id": workspace_id,
+        }
+        if is_default is not None:
+            self._values["is_default"] = is_default
+        if option is not None:
+            self._values["option"] = option
+
+    @builtins.property
+    def group_name(
+        self,
+    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''
+        :Property: groupName: Resource group name. If you want to obtain a resource group name.
+        '''
+        result = self._values.get("group_name")
+        assert result is not None, "Required property 'group_name' is missing"
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+    @builtins.property
+    def resources(
+        self,
+    ) -> typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, RosWorkspaceResourceMaxCompute.ResourcesProperty]]]:
+        '''
+        :Property: resources: Resource List.
+        '''
+        result = self._values.get("resources")
+        assert result is not None, "Required property 'resources' is missing"
+        return typing.cast(typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, RosWorkspaceResourceMaxCompute.ResourcesProperty]]], result)
+
+    @builtins.property
+    def workspace_id(
+        self,
+    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''
+        :Property: workspaceId: The ID of the workspace to which the workspace belongs.
+        '''
+        result = self._values.get("workspace_id")
+        assert result is not None, "Required property 'workspace_id' is missing"
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+    @builtins.property
+    def is_default(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''
+        :Property: isDefault: Indicates whether it is the default resource. Currently, this parameter only supports the input of true and does not support false.
+        '''
+        result = self._values.get("is_default")
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+    @builtins.property
+    def option(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''
+        :Property:
+
+        option: Create behavior that supports the following values:
+
+        - CreateAndAttach: Create resource and bind to workspace
+        - Attach: bind resource to workspace.
+        '''
+        result = self._values.get("option")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "RosWorkspaceResourceMaxComputeProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
 class Service(
     _ros_cdk_core_7adfd82f.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-pai.Service",
 ):
     '''This class encapsulates and extends the ROS resource type ``ALIYUN::PAI::Service``, which is used to create an Elastic Algorithm Service (EAS) service in Machine Learning Platform for AI (PAI).
 
@@ -2603,27 +3937,708 @@
 
     def __repr__(self) -> str:
         return "WorkspaceProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
+class WorkspaceResourceDlc(
+    _ros_cdk_core_7adfd82f.Resource,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@alicloud/ros-cdk-pai.WorkspaceResourceDlc",
+):
+    '''This class encapsulates and extends the ROS resource type ``ALIYUN::PAI::WorkspaceResourceDlc``.
+
+    :Note:
+
+    This class may have some new functions to facilitate development, so it is recommended to use this class instead of ``RosWorkspaceResourceDlc``for a more convenient development experience.
+    See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-pai-workspaceresourcedlc
+    '''
+
+    def __init__(
+        self,
+        scope: _ros_cdk_core_7adfd82f.Construct,
+        id: builtins.str,
+        props: typing.Union["WorkspaceResourceDlcProps", typing.Dict[builtins.str, typing.Any]],
+        enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
+    ) -> None:
+        '''Param scope - scope in which this resource is defined Param id    - scoped id of the resource Param props - resource properties.
+
+        :param scope: -
+        :param id: -
+        :param props: -
+        :param enable_resource_property_constraint: -
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__63546df8d66955b67df555773ed9b3e606b14a29fa6965fa2268998acb0a4d2c)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
+        jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
+
+    @builtins.property
+    @jsii.member(jsii_name="attrCreateTime")
+    def attr_create_time(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+        '''Attribute CreateTime: The creation time of the resource.'''
+        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrCreateTime"))
+
+    @builtins.property
+    @jsii.member(jsii_name="attrGroupName")
+    def attr_group_name(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+        '''Attribute GroupName: Resource group name.
+
+        If you want to obtain a resource group name, see [ListResources].
+        '''
+        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrGroupName"))
+
+    @builtins.property
+    @jsii.member(jsii_name="attrIsDefault")
+    def attr_is_default(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+        '''Attribute IsDefault: Indicates whether it is the default resource.
+
+        Currently, this parameter only supports the input of true and does not support false.
+        '''
+        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrIsDefault"))
+
+    @builtins.property
+    @jsii.member(jsii_name="attrResources")
+    def attr_resources(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+        '''Attribute Resources: Resource List.'''
+        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrResources"))
+
+    @builtins.property
+    @jsii.member(jsii_name="enableResourcePropertyConstraint")
+    def _enable_resource_property_constraint(self) -> builtins.bool:
+        return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
+
+    @_enable_resource_property_constraint.setter
+    def _enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__b2e77be23910d6eaa1d2612e1be0705e0ad7ca00854964d5b724361b18130f6e)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "enableResourcePropertyConstraint", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="id")
+    def _id(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "id"))
+
+    @_id.setter
+    def _id(self, value: builtins.str) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__b491f94a2c96872728f06d0ec790e0960b0a8d84b33ef042a6ad652f6bb91b65)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "id", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="props")
+    def _props(self) -> "WorkspaceResourceDlcProps":
+        return typing.cast("WorkspaceResourceDlcProps", jsii.get(self, "props"))
+
+    @_props.setter
+    def _props(self, value: "WorkspaceResourceDlcProps") -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__8909d882b3436ed61f4d9b4420fc4139e1f5f166bdd283c60e4f92fc2e86d51b)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "props", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="scope")
+    def _scope(self) -> _ros_cdk_core_7adfd82f.Construct:
+        return typing.cast(_ros_cdk_core_7adfd82f.Construct, jsii.get(self, "scope"))
+
+    @_scope.setter
+    def _scope(self, value: _ros_cdk_core_7adfd82f.Construct) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__4311a55046d911a5c4a52e8cea970d74f74f2ede436c089fd9f6d2055695b3da)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "scope", value)
+
+
+@jsii.data_type(
+    jsii_type="@alicloud/ros-cdk-pai.WorkspaceResourceDlcProps",
+    jsii_struct_bases=[],
+    name_mapping={
+        "group_name": "groupName",
+        "resources": "resources",
+        "workspace_id": "workspaceId",
+        "is_default": "isDefault",
+        "option": "option",
+    },
+)
+class WorkspaceResourceDlcProps:
+    def __init__(
+        self,
+        *,
+        group_name: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+        resources: typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Sequence[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Union[RosWorkspaceResourceDlc.ResourcesProperty, typing.Dict[builtins.str, typing.Any]]]]],
+        workspace_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+        is_default: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+        option: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    ) -> None:
+        '''Properties for defining a ``WorkspaceResourceDlc``.
+
+        See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-pai-workspaceresourcedlc
+
+        :param group_name: Property groupName: Resource group name. If you want to obtain a resource group name, see [ListResources].
+        :param resources: Property resources: Resource List.
+        :param workspace_id: Property workspaceId: The ID of the workspace to which the workspace belongs.
+        :param is_default: Property isDefault: Indicates whether it is the default resource. Currently, this parameter only supports the input of true and does not support false.
+        :param option: Property option: Create behavior that supports the following values: - CreateAndAttach: Create resource and bind to workspace - Attach: bind resource to workspace.
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__3917c991494a5fc0d57517a4ee0c19b1bce8a252f645321b2fd27c50a275619e)
+            check_type(argname="argument group_name", value=group_name, expected_type=type_hints["group_name"])
+            check_type(argname="argument resources", value=resources, expected_type=type_hints["resources"])
+            check_type(argname="argument workspace_id", value=workspace_id, expected_type=type_hints["workspace_id"])
+            check_type(argname="argument is_default", value=is_default, expected_type=type_hints["is_default"])
+            check_type(argname="argument option", value=option, expected_type=type_hints["option"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "group_name": group_name,
+            "resources": resources,
+            "workspace_id": workspace_id,
+        }
+        if is_default is not None:
+            self._values["is_default"] = is_default
+        if option is not None:
+            self._values["option"] = option
+
+    @builtins.property
+    def group_name(
+        self,
+    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''Property groupName: Resource group name.
+
+        If you want to obtain a resource group name, see [ListResources].
+        '''
+        result = self._values.get("group_name")
+        assert result is not None, "Required property 'group_name' is missing"
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+    @builtins.property
+    def resources(
+        self,
+    ) -> typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, RosWorkspaceResourceDlc.ResourcesProperty]]]:
+        '''Property resources: Resource List.'''
+        result = self._values.get("resources")
+        assert result is not None, "Required property 'resources' is missing"
+        return typing.cast(typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, RosWorkspaceResourceDlc.ResourcesProperty]]], result)
+
+    @builtins.property
+    def workspace_id(
+        self,
+    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''Property workspaceId: The ID of the workspace to which the workspace belongs.'''
+        result = self._values.get("workspace_id")
+        assert result is not None, "Required property 'workspace_id' is missing"
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+    @builtins.property
+    def is_default(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''Property isDefault: Indicates whether it is the default resource.
+
+        Currently, this parameter only supports the input of true and does not support false.
+        '''
+        result = self._values.get("is_default")
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+    @builtins.property
+    def option(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''Property option: Create behavior that supports the following values: - CreateAndAttach: Create resource and bind to workspace - Attach: bind resource to workspace.'''
+        result = self._values.get("option")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "WorkspaceResourceDlcProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+class WorkspaceResourceFlink(
+    _ros_cdk_core_7adfd82f.Resource,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@alicloud/ros-cdk-pai.WorkspaceResourceFlink",
+):
+    '''This class encapsulates and extends the ROS resource type ``ALIYUN::PAI::WorkspaceResourceFlink``.
+
+    :Note:
+
+    This class may have some new functions to facilitate development, so it is recommended to use this class instead of ``RosWorkspaceResourceFlink``for a more convenient development experience.
+    See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-pai-workspaceresourceflink
+    '''
+
+    def __init__(
+        self,
+        scope: _ros_cdk_core_7adfd82f.Construct,
+        id: builtins.str,
+        props: typing.Union["WorkspaceResourceFlinkProps", typing.Dict[builtins.str, typing.Any]],
+        enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
+    ) -> None:
+        '''Param scope - scope in which this resource is defined Param id    - scoped id of the resource Param props - resource properties.
+
+        :param scope: -
+        :param id: -
+        :param props: -
+        :param enable_resource_property_constraint: -
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__d5b9e69bed1379fdc4949798c4d44070a7080094d18830e1c579f33e6452ce7f)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
+        jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
+
+    @builtins.property
+    @jsii.member(jsii_name="attrCreateTime")
+    def attr_create_time(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+        '''Attribute CreateTime: The creation time of the resource.'''
+        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrCreateTime"))
+
+    @builtins.property
+    @jsii.member(jsii_name="attrGroupName")
+    def attr_group_name(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+        '''Attribute GroupName: Resource group name.
+
+        If you want to obtain a resource group name, see [ListResources](~~ 449143 ~~).
+        '''
+        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrGroupName"))
+
+    @builtins.property
+    @jsii.member(jsii_name="attrIsDefault")
+    def attr_is_default(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+        '''Attribute IsDefault: Indicates whether it is the default resource.
+
+        Currently, this parameter only supports the input of true and does not support false.
+        '''
+        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrIsDefault"))
+
+    @builtins.property
+    @jsii.member(jsii_name="attrResources")
+    def attr_resources(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+        '''Attribute Resources: Resource List.'''
+        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrResources"))
+
+    @builtins.property
+    @jsii.member(jsii_name="enableResourcePropertyConstraint")
+    def _enable_resource_property_constraint(self) -> builtins.bool:
+        return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
+
+    @_enable_resource_property_constraint.setter
+    def _enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__2170fed5ac5e403e2feb921aea28a4405b3dd2643be8f3d7eb0a23e7275a7e73)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "enableResourcePropertyConstraint", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="id")
+    def _id(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "id"))
+
+    @_id.setter
+    def _id(self, value: builtins.str) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__fc58b88436fb418853c8c9bc7279ac5ba4d358df14ea01b75c1231112a14572e)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "id", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="props")
+    def _props(self) -> "WorkspaceResourceFlinkProps":
+        return typing.cast("WorkspaceResourceFlinkProps", jsii.get(self, "props"))
+
+    @_props.setter
+    def _props(self, value: "WorkspaceResourceFlinkProps") -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__a506dca17a95bac049ff03f35fa6a873d23e5e7935e22b1d56bb618abb26c2cb)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "props", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="scope")
+    def _scope(self) -> _ros_cdk_core_7adfd82f.Construct:
+        return typing.cast(_ros_cdk_core_7adfd82f.Construct, jsii.get(self, "scope"))
+
+    @_scope.setter
+    def _scope(self, value: _ros_cdk_core_7adfd82f.Construct) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__06d9b68da69ac1a9092cb958008d7fb8fef18a3aa9274105d7c6030e35dd330f)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "scope", value)
+
+
+@jsii.data_type(
+    jsii_type="@alicloud/ros-cdk-pai.WorkspaceResourceFlinkProps",
+    jsii_struct_bases=[],
+    name_mapping={
+        "group_name": "groupName",
+        "resources": "resources",
+        "workspace_id": "workspaceId",
+        "is_default": "isDefault",
+        "option": "option",
+    },
+)
+class WorkspaceResourceFlinkProps:
+    def __init__(
+        self,
+        *,
+        group_name: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+        resources: typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Sequence[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Union[RosWorkspaceResourceFlink.ResourcesProperty, typing.Dict[builtins.str, typing.Any]]]]],
+        workspace_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+        is_default: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+        option: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    ) -> None:
+        '''Properties for defining a ``WorkspaceResourceFlink``.
+
+        See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-pai-workspaceresourceflink
+
+        :param group_name: Property groupName: Resource group name. If you want to obtain a resource group name, see [ListResources].
+        :param resources: Property resources: Resource List.
+        :param workspace_id: Property workspaceId: The ID of the workspace to which the workspace belongs.
+        :param is_default: Property isDefault: Indicates whether it is the default resource. Currently, this parameter only supports the input of true and does not support false.
+        :param option: Property option: Create behavior that supports the following values: - CreateAndAttach: Create resource and bind to workspace - Attach: bind resource to workspace.
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__5924305a2db5d17a14e3fe49854a4bc6182d2bc1c2aed0825602d70b8f5524a5)
+            check_type(argname="argument group_name", value=group_name, expected_type=type_hints["group_name"])
+            check_type(argname="argument resources", value=resources, expected_type=type_hints["resources"])
+            check_type(argname="argument workspace_id", value=workspace_id, expected_type=type_hints["workspace_id"])
+            check_type(argname="argument is_default", value=is_default, expected_type=type_hints["is_default"])
+            check_type(argname="argument option", value=option, expected_type=type_hints["option"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "group_name": group_name,
+            "resources": resources,
+            "workspace_id": workspace_id,
+        }
+        if is_default is not None:
+            self._values["is_default"] = is_default
+        if option is not None:
+            self._values["option"] = option
+
+    @builtins.property
+    def group_name(
+        self,
+    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''Property groupName: Resource group name.
+
+        If you want to obtain a resource group name, see [ListResources].
+        '''
+        result = self._values.get("group_name")
+        assert result is not None, "Required property 'group_name' is missing"
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+    @builtins.property
+    def resources(
+        self,
+    ) -> typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, RosWorkspaceResourceFlink.ResourcesProperty]]]:
+        '''Property resources: Resource List.'''
+        result = self._values.get("resources")
+        assert result is not None, "Required property 'resources' is missing"
+        return typing.cast(typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, RosWorkspaceResourceFlink.ResourcesProperty]]], result)
+
+    @builtins.property
+    def workspace_id(
+        self,
+    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''Property workspaceId: The ID of the workspace to which the workspace belongs.'''
+        result = self._values.get("workspace_id")
+        assert result is not None, "Required property 'workspace_id' is missing"
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+    @builtins.property
+    def is_default(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''Property isDefault: Indicates whether it is the default resource.
+
+        Currently, this parameter only supports the input of true and does not support false.
+        '''
+        result = self._values.get("is_default")
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+    @builtins.property
+    def option(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''Property option: Create behavior that supports the following values: - CreateAndAttach: Create resource and bind to workspace - Attach: bind resource to workspace.'''
+        result = self._values.get("option")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "WorkspaceResourceFlinkProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+class WorkspaceResourceMaxCompute(
+    _ros_cdk_core_7adfd82f.Resource,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@alicloud/ros-cdk-pai.WorkspaceResourceMaxCompute",
+):
+    '''This class encapsulates and extends the ROS resource type ``ALIYUN::PAI::WorkspaceResourceMaxCompute``.
+
+    :Note:
+
+    This class may have some new functions to facilitate development, so it is recommended to use this class instead of ``RosWorkspaceResourceMaxCompute``for a more convenient development experience.
+    See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-pai-workspaceresourcemaxcompute
+    '''
+
+    def __init__(
+        self,
+        scope: _ros_cdk_core_7adfd82f.Construct,
+        id: builtins.str,
+        props: typing.Union["WorkspaceResourceMaxComputeProps", typing.Dict[builtins.str, typing.Any]],
+        enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
+    ) -> None:
+        '''Param scope - scope in which this resource is defined Param id    - scoped id of the resource Param props - resource properties.
+
+        :param scope: -
+        :param id: -
+        :param props: -
+        :param enable_resource_property_constraint: -
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__1530a477af8fa885fabd8e57e28b063f8ab481885c416331a825df2674e429ec)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
+        jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
+
+    @builtins.property
+    @jsii.member(jsii_name="attrCreateTime")
+    def attr_create_time(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+        '''Attribute CreateTime: The creation time of the resource.'''
+        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrCreateTime"))
+
+    @builtins.property
+    @jsii.member(jsii_name="attrGroupName")
+    def attr_group_name(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+        '''Attribute GroupName: Resource group name.
+
+        If you want to obtain a resource group name, see [ListResources](~~ 449143 ~~).
+        '''
+        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrGroupName"))
+
+    @builtins.property
+    @jsii.member(jsii_name="attrIsDefault")
+    def attr_is_default(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+        '''Attribute IsDefault: Indicates whether it is the default resource.
+
+        Currently, this parameter only supports the input of true and does not support false.
+        '''
+        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrIsDefault"))
+
+    @builtins.property
+    @jsii.member(jsii_name="attrResources")
+    def attr_resources(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+        '''Attribute Resources: Resource List.'''
+        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrResources"))
+
+    @builtins.property
+    @jsii.member(jsii_name="enableResourcePropertyConstraint")
+    def _enable_resource_property_constraint(self) -> builtins.bool:
+        return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
+
+    @_enable_resource_property_constraint.setter
+    def _enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__78010a4c30ec573aac3e19517d32d650b56daabf86c5d2877b17c0868667aa38)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "enableResourcePropertyConstraint", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="id")
+    def _id(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "id"))
+
+    @_id.setter
+    def _id(self, value: builtins.str) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__08a94bde773100209e54a8611607d738d92cfb1848dd41a0db36f1fe00b27dbe)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "id", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="props")
+    def _props(self) -> "WorkspaceResourceMaxComputeProps":
+        return typing.cast("WorkspaceResourceMaxComputeProps", jsii.get(self, "props"))
+
+    @_props.setter
+    def _props(self, value: "WorkspaceResourceMaxComputeProps") -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__218434528a74c7ee997833274c04c37e6484b84c5d56b41245176b2bf927fad5)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "props", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="scope")
+    def _scope(self) -> _ros_cdk_core_7adfd82f.Construct:
+        return typing.cast(_ros_cdk_core_7adfd82f.Construct, jsii.get(self, "scope"))
+
+    @_scope.setter
+    def _scope(self, value: _ros_cdk_core_7adfd82f.Construct) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__3fc0acfb2105bbfcf22891f163c061fb8bb140372076f07d2b7ee5531409958d)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "scope", value)
+
+
+@jsii.data_type(
+    jsii_type="@alicloud/ros-cdk-pai.WorkspaceResourceMaxComputeProps",
+    jsii_struct_bases=[],
+    name_mapping={
+        "group_name": "groupName",
+        "resources": "resources",
+        "workspace_id": "workspaceId",
+        "is_default": "isDefault",
+        "option": "option",
+    },
+)
+class WorkspaceResourceMaxComputeProps:
+    def __init__(
+        self,
+        *,
+        group_name: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+        resources: typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Sequence[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Union[RosWorkspaceResourceMaxCompute.ResourcesProperty, typing.Dict[builtins.str, typing.Any]]]]],
+        workspace_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+        is_default: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+        option: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    ) -> None:
+        '''Properties for defining a ``WorkspaceResourceMaxCompute``.
+
+        See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-pai-workspaceresourcemaxcompute
+
+        :param group_name: Property groupName: Resource group name. If you want to obtain a resource group name.
+        :param resources: Property resources: Resource List.
+        :param workspace_id: Property workspaceId: The ID of the workspace to which the workspace belongs.
+        :param is_default: Property isDefault: Indicates whether it is the default resource. Currently, this parameter only supports the input of true and does not support false.
+        :param option: Property option: Create behavior that supports the following values: - CreateAndAttach: Create resource and bind to workspace - Attach: bind resource to workspace.
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__ff9cc3cfa518240282e1cbec3a481d8ea60e2139f3e61fedb6529c4bec25bca6)
+            check_type(argname="argument group_name", value=group_name, expected_type=type_hints["group_name"])
+            check_type(argname="argument resources", value=resources, expected_type=type_hints["resources"])
+            check_type(argname="argument workspace_id", value=workspace_id, expected_type=type_hints["workspace_id"])
+            check_type(argname="argument is_default", value=is_default, expected_type=type_hints["is_default"])
+            check_type(argname="argument option", value=option, expected_type=type_hints["option"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "group_name": group_name,
+            "resources": resources,
+            "workspace_id": workspace_id,
+        }
+        if is_default is not None:
+            self._values["is_default"] = is_default
+        if option is not None:
+            self._values["option"] = option
+
+    @builtins.property
+    def group_name(
+        self,
+    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''Property groupName: Resource group name.
+
+        If you want to obtain a resource group name.
+        '''
+        result = self._values.get("group_name")
+        assert result is not None, "Required property 'group_name' is missing"
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+    @builtins.property
+    def resources(
+        self,
+    ) -> typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, RosWorkspaceResourceMaxCompute.ResourcesProperty]]]:
+        '''Property resources: Resource List.'''
+        result = self._values.get("resources")
+        assert result is not None, "Required property 'resources' is missing"
+        return typing.cast(typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, RosWorkspaceResourceMaxCompute.ResourcesProperty]]], result)
+
+    @builtins.property
+    def workspace_id(
+        self,
+    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''Property workspaceId: The ID of the workspace to which the workspace belongs.'''
+        result = self._values.get("workspace_id")
+        assert result is not None, "Required property 'workspace_id' is missing"
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+    @builtins.property
+    def is_default(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''Property isDefault: Indicates whether it is the default resource.
+
+        Currently, this parameter only supports the input of true and does not support false.
+        '''
+        result = self._values.get("is_default")
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+    @builtins.property
+    def option(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''Property option: Create behavior that supports the following values: - CreateAndAttach: Create resource and bind to workspace - Attach: bind resource to workspace.'''
+        result = self._values.get("option")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "WorkspaceResourceMaxComputeProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
 __all__ = [
     "Dataset",
     "DatasetProps",
     "RosDataset",
     "RosDatasetProps",
     "RosService",
     "RosServiceProps",
     "RosWorkspace",
     "RosWorkspaceProps",
+    "RosWorkspaceResourceDlc",
+    "RosWorkspaceResourceDlcProps",
+    "RosWorkspaceResourceFlink",
+    "RosWorkspaceResourceFlinkProps",
+    "RosWorkspaceResourceMaxCompute",
+    "RosWorkspaceResourceMaxComputeProps",
     "Service",
     "ServiceProps",
     "Workspace",
     "WorkspaceProps",
+    "WorkspaceResourceDlc",
+    "WorkspaceResourceDlcProps",
+    "WorkspaceResourceFlink",
+    "WorkspaceResourceFlinkProps",
+    "WorkspaceResourceMaxCompute",
+    "WorkspaceResourceMaxComputeProps",
     "datasource",
 ]
 
 publication.publish()
 
 # Loading modules to ensure their types are registered with the jsii runtime library
 from . import datasource
@@ -2881,14 +4896,238 @@
     env_types: typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Sequence[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]],
     workspace_name: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
     display_name: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__ea471a7c5a468bef4fbe3da7e68f4dc188887b43f7aa5af028489e058c6bb75c(
+    scope: _ros_cdk_core_7adfd82f.Construct,
+    id: builtins.str,
+    props: typing.Union[RosWorkspaceResourceDlcProps, typing.Dict[builtins.str, typing.Any]],
+    enable_resource_property_constraint: builtins.bool,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__880f6f3ac266a1fb510823f94b53f269bb495e4fe76e18aaf23b873fb85cbc54(
+    props: typing.Mapping[builtins.str, typing.Any],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__bd53872479e3c25b6c5bf40f49be3c3142ce169ab5c654cc83d020869026da40(
+    value: builtins.bool,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__62ffc6de5eef8f8c7deb4bd47fba77afaf8f75da950cb755ea9749786bce401a(
+    value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__851f8fec11054543e2700b9f4236d062bd022ebdabab1932c9f76df752b554b1(
+    value: typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, RosWorkspaceResourceDlc.ResourcesProperty]]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__a02cb6e32cd7d71600381b6de6c52bbc9c54c46998d1cbdc7e053603a61b038a(
+    value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__3cd28cac9cfc4c04e9236d83f6baa1a2bc767cb752186ebc1640ea0573ff31a6(
+    value: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__c2278990b8b85d56ab86bac7c23b334be02aadfa5eaf74feaaa2c38216caae21(
+    value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__3b63c737a049056c6be56bdb83efec08ab424dc639b21a4ad5124e241f87be64(
+    *,
+    env_type: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    workspace_resource_name: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    workspace_resource_workspace_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    spec: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Mapping[builtins.str, typing.Any]]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__ebe3af48413265457d30902f743d3ada3ff1f69c0081c3fe7bf7d63bc0a3ca88(
+    *,
+    group_name: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    resources: typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Sequence[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Union[RosWorkspaceResourceDlc.ResourcesProperty, typing.Dict[builtins.str, typing.Any]]]]],
+    workspace_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    is_default: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    option: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__578e83686f72937307c5eaff49925ac4609f7af1a907878ecbfa0a2f841c738a(
+    scope: _ros_cdk_core_7adfd82f.Construct,
+    id: builtins.str,
+    props: typing.Union[RosWorkspaceResourceFlinkProps, typing.Dict[builtins.str, typing.Any]],
+    enable_resource_property_constraint: builtins.bool,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__50e901a2952ba52b6a10bc49b7e5b3189d80075f43b1e615ae6e13998ef08ad7(
+    props: typing.Mapping[builtins.str, typing.Any],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__9d1c9fa6b40ab37ba09aef6151f1e66e229d437080ed99bb6cf8089e85fd86c1(
+    value: builtins.bool,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__ca323975d7fc5f1d16a657130dc599c4f908c298b936a0d169d12df4d844e558(
+    value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__79dfa340d3c04d62dab1f2e4805ac4e24350f4232085e4080aead4afee0fefe4(
+    value: typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, RosWorkspaceResourceFlink.ResourcesProperty]]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__d2fdbf156aa98caf320eedfe08a20588da72a316c3be60f39a2c78dcf88f9304(
+    value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__d7df214b7927ddd30a219d7422b60c2669d86f9096b9ad198de745404e3a3e06(
+    value: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__d6cfa95eb1a0fc9d5a6cf49da807d4d6154105dfd0ad6ebc8d1ec394a59961ac(
+    value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__89ca36c747cdfe0629d41004d514da825f4cecde19a50efd3dad85f13cc21e5d(
+    *,
+    env_type: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    workspace_resource_name: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    workspace_resource_workspace_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    spec: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Mapping[builtins.str, typing.Any]]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__57bfe40c04abe5e6fe19e91814ee8956f205f1f3fa2b27ecfbe7b2f455a8f03e(
+    *,
+    group_name: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    resources: typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Sequence[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Union[RosWorkspaceResourceFlink.ResourcesProperty, typing.Dict[builtins.str, typing.Any]]]]],
+    workspace_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    is_default: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    option: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__b2f66acdef9422d08230176a5b72b7f5ffcd09e7423e28e62bfae4e5ebb3d1e8(
+    scope: _ros_cdk_core_7adfd82f.Construct,
+    id: builtins.str,
+    props: typing.Union[RosWorkspaceResourceMaxComputeProps, typing.Dict[builtins.str, typing.Any]],
+    enable_resource_property_constraint: builtins.bool,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__b0915637f1ed1f6490dc4cf208d921579edb493622a7a2aacf5c07188c363642(
+    props: typing.Mapping[builtins.str, typing.Any],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__3e020f1431efd6202810928f260ad1f7a6cc98c572186a0974c23d9be1f39231(
+    value: builtins.bool,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__9201de5fa777a55754433585aef86290a7eea5e417e3c4e366351d8324b5af9c(
+    value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__04ea2d9563b588f5231d2d9c450110738c227aa293b3544800dcea6316ead8ce(
+    value: typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, RosWorkspaceResourceMaxCompute.ResourcesProperty]]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__7395f30834464169f2d941232a6f6ab2de6666ef318e4b0ddda3ef3536bc45fe(
+    value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__ea06bb30d84c99805226cf5f24f9bb434100e07f7513660da1d08ca7cd5a0ce4(
+    value: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__78300066522bbb82d6f5389c93bb95b7b0ddf71df2b55fdbc95b90ffa6677d28(
+    value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__a70ae00332f2bfed57c993bdf06e7efc8435125887165aa32a8edcb286a675d1(
+    *,
+    quota_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__6957cb7eb7fe278e12e47aee5f6cd93edb8f6a9976848a38f6ab123bd66380b6(
+    *,
+    env_type: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    workspace_resource_name: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    workspace_resource_workspace_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    quotas: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Sequence[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Union[RosWorkspaceResourceMaxCompute.QuotasProperty, typing.Dict[builtins.str, typing.Any]]]]]] = None,
+    spec: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Mapping[builtins.str, typing.Any]]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__79d876bae6e4a2d418971fcf603e4262414b3c2431be6929353adf44d387cdb3(
+    *,
+    group_name: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    resources: typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Sequence[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Union[RosWorkspaceResourceMaxCompute.ResourcesProperty, typing.Dict[builtins.str, typing.Any]]]]],
+    workspace_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    is_default: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    option: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__8322efa66b3ef76d8c8ece2e6b2c98ce0b62c9d22deb3d2028b7ccb124bda821(
     scope: _ros_cdk_core_7adfd82f.Construct,
     id: builtins.str,
     props: typing.Union[ServiceProps, typing.Dict[builtins.str, typing.Any]],
     enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
 ) -> None:
     """Type checking stubs"""
@@ -2965,7 +5204,139 @@
     description: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
     env_types: typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Sequence[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]],
     workspace_name: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
     display_name: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
+
+def _typecheckingstub__63546df8d66955b67df555773ed9b3e606b14a29fa6965fa2268998acb0a4d2c(
+    scope: _ros_cdk_core_7adfd82f.Construct,
+    id: builtins.str,
+    props: typing.Union[WorkspaceResourceDlcProps, typing.Dict[builtins.str, typing.Any]],
+    enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__b2e77be23910d6eaa1d2612e1be0705e0ad7ca00854964d5b724361b18130f6e(
+    value: builtins.bool,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__b491f94a2c96872728f06d0ec790e0960b0a8d84b33ef042a6ad652f6bb91b65(
+    value: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__8909d882b3436ed61f4d9b4420fc4139e1f5f166bdd283c60e4f92fc2e86d51b(
+    value: WorkspaceResourceDlcProps,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__4311a55046d911a5c4a52e8cea970d74f74f2ede436c089fd9f6d2055695b3da(
+    value: _ros_cdk_core_7adfd82f.Construct,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__3917c991494a5fc0d57517a4ee0c19b1bce8a252f645321b2fd27c50a275619e(
+    *,
+    group_name: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    resources: typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Sequence[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Union[RosWorkspaceResourceDlc.ResourcesProperty, typing.Dict[builtins.str, typing.Any]]]]],
+    workspace_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    is_default: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    option: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__d5b9e69bed1379fdc4949798c4d44070a7080094d18830e1c579f33e6452ce7f(
+    scope: _ros_cdk_core_7adfd82f.Construct,
+    id: builtins.str,
+    props: typing.Union[WorkspaceResourceFlinkProps, typing.Dict[builtins.str, typing.Any]],
+    enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__2170fed5ac5e403e2feb921aea28a4405b3dd2643be8f3d7eb0a23e7275a7e73(
+    value: builtins.bool,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__fc58b88436fb418853c8c9bc7279ac5ba4d358df14ea01b75c1231112a14572e(
+    value: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__a506dca17a95bac049ff03f35fa6a873d23e5e7935e22b1d56bb618abb26c2cb(
+    value: WorkspaceResourceFlinkProps,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__06d9b68da69ac1a9092cb958008d7fb8fef18a3aa9274105d7c6030e35dd330f(
+    value: _ros_cdk_core_7adfd82f.Construct,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__5924305a2db5d17a14e3fe49854a4bc6182d2bc1c2aed0825602d70b8f5524a5(
+    *,
+    group_name: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    resources: typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Sequence[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Union[RosWorkspaceResourceFlink.ResourcesProperty, typing.Dict[builtins.str, typing.Any]]]]],
+    workspace_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    is_default: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    option: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__1530a477af8fa885fabd8e57e28b063f8ab481885c416331a825df2674e429ec(
+    scope: _ros_cdk_core_7adfd82f.Construct,
+    id: builtins.str,
+    props: typing.Union[WorkspaceResourceMaxComputeProps, typing.Dict[builtins.str, typing.Any]],
+    enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__78010a4c30ec573aac3e19517d32d650b56daabf86c5d2877b17c0868667aa38(
+    value: builtins.bool,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__08a94bde773100209e54a8611607d738d92cfb1848dd41a0db36f1fe00b27dbe(
+    value: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__218434528a74c7ee997833274c04c37e6484b84c5d56b41245176b2bf927fad5(
+    value: WorkspaceResourceMaxComputeProps,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__3fc0acfb2105bbfcf22891f163c061fb8bb140372076f07d2b7ee5531409958d(
+    value: _ros_cdk_core_7adfd82f.Construct,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__ff9cc3cfa518240282e1cbec3a481d8ea60e2139f3e61fedb6529c4bec25bca6(
+    *,
+    group_name: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    resources: typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Sequence[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Union[RosWorkspaceResourceMaxCompute.ResourcesProperty, typing.Dict[builtins.str, typing.Any]]]]],
+    workspace_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    is_default: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    option: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
```

### Comparing `ros-cdk-pai-1.0.24/src/ros_cdk_pai/datasource/__init__.py` & `ros-cdk-pai-1.0.25/src/ros_cdk_pai/datasource/__init__.py`

 * *Files identical despite different names*

### Comparing `ros-cdk-pai-1.0.24/src/ros_cdk_pai.egg-info/PKG-INFO` & `ros-cdk-pai-1.0.25/src/ros_cdk_pai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-pai
-Version: 1.0.24
+Version: 1.0.25
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS PAI Construct Library
```

