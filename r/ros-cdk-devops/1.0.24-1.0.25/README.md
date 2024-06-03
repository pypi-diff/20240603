# Comparing `tmp/ros-cdk-devops-1.0.24.tar.gz` & `tmp/ros-cdk-devops-1.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-devops-1.0.24.tar", last modified: Wed Apr 10 04:33:57 2024, max compression
+gzip compressed data, was "dist/ros-cdk-devops-1.0.25.tar", last modified: Mon Jun  3 11:12:09 2024, max compression
```

## Comparing `ros-cdk-devops-1.0.24.tar` & `ros-cdk-devops-1.0.25.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:33:57.000000 ros-cdk-devops-1.0.24/
--rw-r--r--   0 root         (0) root         (0)    10279 2024-04-10 04:33:56.000000 ros-cdk-devops-1.0.24/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-10 04:33:56.000000 ros-cdk-devops-1.0.24/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2024-04-10 04:33:56.000000 ros-cdk-devops-1.0.24/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1304 2024-04-10 04:33:57.000000 ros-cdk-devops-1.0.24/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      188 2024-04-10 04:33:56.000000 ros-cdk-devops-1.0.24/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2024-04-10 04:33:56.000000 ros-cdk-devops-1.0.24/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 04:33:57.000000 ros-cdk-devops-1.0.24/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1894 2024-04-10 04:33:56.000000 ros-cdk-devops-1.0.24/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:33:57.000000 ros-cdk-devops-1.0.24/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:33:57.000000 ros-cdk-devops-1.0.24/src/ros_cdk_devops/
--rw-r--r--   0 root         (0) root         (0)   105052 2024-04-10 04:33:56.000000 ros-cdk-devops-1.0.24/src/ros_cdk_devops/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:33:57.000000 ros-cdk-devops-1.0.24/src/ros_cdk_devops/_jsii/
--rw-r--r--   0 root         (0) root         (0)      425 2024-04-10 04:33:56.000000 ros-cdk-devops-1.0.24/src/ros_cdk_devops/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45894 2024-04-10 04:33:56.000000 ros-cdk-devops-1.0.24/src/ros_cdk_devops/_jsii/ros-cdk-devops@1.0.24.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 04:33:56.000000 ros-cdk-devops-1.0.24/src/ros_cdk_devops/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:33:57.000000 ros-cdk-devops-1.0.24/src/ros_cdk_devops.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1304 2024-04-10 04:33:57.000000 ros-cdk-devops-1.0.24/src/ros_cdk_devops.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      431 2024-04-10 04:33:57.000000 ros-cdk-devops-1.0.24/src/ros_cdk_devops.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 04:33:57.000000 ros-cdk-devops-1.0.24/src/ros_cdk_devops.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      110 2024-04-10 04:33:57.000000 ros-cdk-devops-1.0.24/src/ros_cdk_devops.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-04-10 04:33:57.000000 ros-cdk-devops-1.0.24/src/ros_cdk_devops.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:12:09.000000 ros-cdk-devops-1.0.25/
+-rw-r--r--   0 root         (0) root         (0)    10279 2024-06-03 11:12:09.000000 ros-cdk-devops-1.0.25/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2024-06-03 11:12:09.000000 ros-cdk-devops-1.0.25/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2024-06-03 11:12:09.000000 ros-cdk-devops-1.0.25/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1304 2024-06-03 11:12:09.000000 ros-cdk-devops-1.0.25/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      188 2024-06-03 11:12:09.000000 ros-cdk-devops-1.0.25/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2024-06-03 11:12:09.000000 ros-cdk-devops-1.0.25/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-06-03 11:12:09.000000 ros-cdk-devops-1.0.25/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1895 2024-06-03 11:12:09.000000 ros-cdk-devops-1.0.25/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:12:09.000000 ros-cdk-devops-1.0.25/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:12:09.000000 ros-cdk-devops-1.0.25/src/ros_cdk_devops/
+-rw-r--r--   0 root         (0) root         (0)   155756 2024-06-03 11:12:09.000000 ros-cdk-devops-1.0.25/src/ros_cdk_devops/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:12:09.000000 ros-cdk-devops-1.0.25/src/ros_cdk_devops/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      425 2024-06-03 11:12:09.000000 ros-cdk-devops-1.0.25/src/ros_cdk_devops/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56189 2024-06-03 11:12:09.000000 ros-cdk-devops-1.0.25/src/ros_cdk_devops/_jsii/ros-cdk-devops@1.0.25.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 11:12:09.000000 ros-cdk-devops-1.0.25/src/ros_cdk_devops/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:12:09.000000 ros-cdk-devops-1.0.25/src/ros_cdk_devops.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1304 2024-06-03 11:12:09.000000 ros-cdk-devops-1.0.25/src/ros_cdk_devops.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      431 2024-06-03 11:12:09.000000 ros-cdk-devops-1.0.25/src/ros_cdk_devops.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 11:12:09.000000 ros-cdk-devops-1.0.25/src/ros_cdk_devops.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      111 2024-06-03 11:12:09.000000 ros-cdk-devops-1.0.25/src/ros_cdk_devops.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-06-03 11:12:09.000000 ros-cdk-devops-1.0.25/src/ros_cdk_devops.egg-info/top_level.txt
```

### Comparing `ros-cdk-devops-1.0.24/LICENSE` & `ros-cdk-devops-1.0.25/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-devops-1.0.24/PKG-INFO` & `ros-cdk-devops-1.0.25/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-devops
-Version: 1.0.24
+Version: 1.0.25
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS DEVOPS Construct Library
```

### Comparing `ros-cdk-devops-1.0.24/setup.py` & `ros-cdk-devops-1.0.25/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-devops",
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
         "ros_cdk_devops",
         "ros_cdk_devops._jsii"
     ],
     "package_data": {
         "ros_cdk_devops._jsii": [
-            "ros-cdk-devops@1.0.24.jsii.tgz"
+            "ros-cdk-devops@1.0.25.jsii.tgz"
         ],
         "ros_cdk_devops": [
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

### Comparing `ros-cdk-devops-1.0.24/src/ros_cdk_devops/__init__.py` & `ros-cdk-devops-1.0.25/src/ros_cdk_devops/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,14 +20,289 @@
 from typeguard import check_type
 
 from ._jsii import *
 
 import ros_cdk_core as _ros_cdk_core_7adfd82f
 
 
+class HostGroup(
+    _ros_cdk_core_7adfd82f.Resource,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@alicloud/ros-cdk-devops.HostGroup",
+):
+    '''This class encapsulates and extends the ROS resource type ``ALIYUN::DEVOPS::HostGroup``.
+
+    :Note:
+
+    This class may have some new functions to facilitate development, so it is recommended to use this class instead of ``RosHostGroup``for a more convenient development experience.
+    See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-devops-hostgroup
+    '''
+
+    def __init__(
+        self,
+        scope: _ros_cdk_core_7adfd82f.Construct,
+        id: builtins.str,
+        props: typing.Union["HostGroupProps", typing.Dict[builtins.str, typing.Any]],
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
+            type_hints = typing.get_type_hints(_typecheckingstub__d57d664cd9856802b0eafdcdfc868df58424b0f6865e48fa0cfdef1b0edfe430)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
+        jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
+
+    @builtins.property
+    @jsii.member(jsii_name="attrHostGroupId")
+    def attr_host_group_id(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+        '''Attribute HostGroupId: The id of the host group.'''
+        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrHostGroupId"))
+
+    @builtins.property
+    @jsii.member(jsii_name="enableResourcePropertyConstraint")
+    def _enable_resource_property_constraint(self) -> builtins.bool:
+        return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
+
+    @_enable_resource_property_constraint.setter
+    def _enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__6ee7c5ba5b674bb6b0c2574a544f90904abd14d7b0a55062f84f41b1b4f55704)
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
+            type_hints = typing.get_type_hints(_typecheckingstub__93a3dd2c14ab056517e5a1d17bc1dc4928a6c69008f3c9747cacb62fffa88ec7)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "id", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="props")
+    def _props(self) -> "HostGroupProps":
+        return typing.cast("HostGroupProps", jsii.get(self, "props"))
+
+    @_props.setter
+    def _props(self, value: "HostGroupProps") -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__aee5e2d1b71f25ecd7a68fdf61a9826522f920533cd4a720a84d6a7b1533d631)
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
+            type_hints = typing.get_type_hints(_typecheckingstub__e0a64f2c2aedb570147001a8ecf480c3504691cc599c3a0aad531f0c2b7876aa)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "scope", value)
+
+
+@jsii.data_type(
+    jsii_type="@alicloud/ros-cdk-devops.HostGroupProps",
+    jsii_struct_bases=[],
+    name_mapping={
+        "name": "name",
+        "organization_id": "organizationId",
+        "service_connection_id": "serviceConnectionId",
+        "aliyun_region": "aliyunRegion",
+        "ecs_label_key": "ecsLabelKey",
+        "ecs_label_value": "ecsLabelValue",
+        "ecs_type": "ecsType",
+        "env_id": "envId",
+        "machine_infos": "machineInfos",
+        "tag_ids": "tagIds",
+        "type": "type",
+    },
+)
+class HostGroupProps:
+    def __init__(
+        self,
+        *,
+        name: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+        organization_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+        service_connection_id: typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable],
+        aliyun_region: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+        ecs_label_key: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+        ecs_label_value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+        ecs_type: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+        env_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+        machine_infos: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Sequence[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Union["RosHostGroup.MachineInfosProperty", typing.Dict[builtins.str, typing.Any]]]]]] = None,
+        tag_ids: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Sequence[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]]] = None,
+        type: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    ) -> None:
+        '''Properties for defining a ``HostGroup``.
+
+        See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-devops-hostgroup
+
+        :param name: Property name: Host group name.
+        :param organization_id: Property organizationId: Corporate identity, also known as enterprise id, can obtain in cloud effect access links.
+        :param service_connection_id: Property serviceConnectionId: Service connection.
+        :param aliyun_region: Property aliyunRegion: The aliyun region.
+        :param ecs_label_key: Property ecsLabelKey: The tag key of the ECS.
+        :param ecs_label_value: Property ecsLabelValue: The tag value of the ECS.
+        :param ecs_type: Property ecsType: The type of ECS, currently only supports ECS_ALIYUN.
+        :param env_id: Property envId: Environment id.
+        :param machine_infos: Property machineInfos: The machine infos.
+        :param tag_ids: Property tagIds: The ids of tag.
+        :param type: Property type: Host group type, currently only supports ECS.
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__479b32c1718b7fc7c26bca41898094ff529fc13c791e8ec57615a728d8c090be)
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument organization_id", value=organization_id, expected_type=type_hints["organization_id"])
+            check_type(argname="argument service_connection_id", value=service_connection_id, expected_type=type_hints["service_connection_id"])
+            check_type(argname="argument aliyun_region", value=aliyun_region, expected_type=type_hints["aliyun_region"])
+            check_type(argname="argument ecs_label_key", value=ecs_label_key, expected_type=type_hints["ecs_label_key"])
+            check_type(argname="argument ecs_label_value", value=ecs_label_value, expected_type=type_hints["ecs_label_value"])
+            check_type(argname="argument ecs_type", value=ecs_type, expected_type=type_hints["ecs_type"])
+            check_type(argname="argument env_id", value=env_id, expected_type=type_hints["env_id"])
+            check_type(argname="argument machine_infos", value=machine_infos, expected_type=type_hints["machine_infos"])
+            check_type(argname="argument tag_ids", value=tag_ids, expected_type=type_hints["tag_ids"])
+            check_type(argname="argument type", value=type, expected_type=type_hints["type"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "name": name,
+            "organization_id": organization_id,
+            "service_connection_id": service_connection_id,
+        }
+        if aliyun_region is not None:
+            self._values["aliyun_region"] = aliyun_region
+        if ecs_label_key is not None:
+            self._values["ecs_label_key"] = ecs_label_key
+        if ecs_label_value is not None:
+            self._values["ecs_label_value"] = ecs_label_value
+        if ecs_type is not None:
+            self._values["ecs_type"] = ecs_type
+        if env_id is not None:
+            self._values["env_id"] = env_id
+        if machine_infos is not None:
+            self._values["machine_infos"] = machine_infos
+        if tag_ids is not None:
+            self._values["tag_ids"] = tag_ids
+        if type is not None:
+            self._values["type"] = type
+
+    @builtins.property
+    def name(self) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''Property name: Host group name.'''
+        result = self._values.get("name")
+        assert result is not None, "Required property 'name' is missing"
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+    @builtins.property
+    def organization_id(
+        self,
+    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''Property organizationId: Corporate identity, also known as enterprise id, can obtain in cloud effect access links.'''
+        result = self._values.get("organization_id")
+        assert result is not None, "Required property 'organization_id' is missing"
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+    @builtins.property
+    def service_connection_id(
+        self,
+    ) -> typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''Property serviceConnectionId: Service connection.'''
+        result = self._values.get("service_connection_id")
+        assert result is not None, "Required property 'service_connection_id' is missing"
+        return typing.cast(typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+    @builtins.property
+    def aliyun_region(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''Property aliyunRegion: The aliyun region.'''
+        result = self._values.get("aliyun_region")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+    @builtins.property
+    def ecs_label_key(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''Property ecsLabelKey: The tag key of the ECS.'''
+        result = self._values.get("ecs_label_key")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+    @builtins.property
+    def ecs_label_value(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''Property ecsLabelValue: The tag value of the ECS.'''
+        result = self._values.get("ecs_label_value")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+    @builtins.property
+    def ecs_type(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''Property ecsType: The type of ECS, currently only supports ECS_ALIYUN.'''
+        result = self._values.get("ecs_type")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+    @builtins.property
+    def env_id(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''Property envId: Environment id.'''
+        result = self._values.get("env_id")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+    @builtins.property
+    def machine_infos(
+        self,
+    ) -> typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, "RosHostGroup.MachineInfosProperty"]]]]:
+        '''Property machineInfos: The machine infos.'''
+        result = self._values.get("machine_infos")
+        return typing.cast(typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, "RosHostGroup.MachineInfosProperty"]]]], result)
+
+    @builtins.property
+    def tag_ids(
+        self,
+    ) -> typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]]]:
+        '''Property tagIds: The ids of tag.'''
+        result = self._values.get("tag_ids")
+        return typing.cast(typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]]], result)
+
+    @builtins.property
+    def type(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''Property type: Host group type, currently only supports ECS.'''
+        result = self._values.get("type")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "HostGroupProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
 class Pipeline(
     _ros_cdk_core_7adfd82f.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-devops.Pipeline",
 ):
     '''This class encapsulates and extends the ROS resource type ``ALIYUN::DEVOPS::Pipeline``, which is used to create a pipeline.
 
@@ -574,14 +849,611 @@
 
     def __repr__(self) -> str:
         return "PipelineRunProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
+class RosHostGroup(
+    _ros_cdk_core_7adfd82f.RosResource,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@alicloud/ros-cdk-devops.RosHostGroup",
+):
+    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::DEVOPS::HostGroup``.
+
+    :Note:
+
+    This class does not contain additional functions, so it is recommended to use the ``HostGroup`` class instead of this class for a more convenient development experience.
+    See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-devops-hostgroup
+    '''
+
+    def __init__(
+        self,
+        scope: _ros_cdk_core_7adfd82f.Construct,
+        id: builtins.str,
+        props: typing.Union["RosHostGroupProps", typing.Dict[builtins.str, typing.Any]],
+        enable_resource_property_constraint: builtins.bool,
+    ) -> None:
+        '''
+        :param scope: - scope in which this resource is defined.
+        :param id: - scoped id of the resource.
+        :param props: - resource properties.
+        :param enable_resource_property_constraint: -
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__b4860cfe5cd458ab67e95e319ed56f8e68df738f346bd5820d127c20032bf0a1)
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
+            type_hints = typing.get_type_hints(_typecheckingstub__9cf5261897cc0b6de015b6775116f7aee1ff54e5cd0415193e139cfe8d09bf9f)
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
+    @jsii.member(jsii_name="attrHostGroupId")
+    def attr_host_group_id(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+        '''
+        :Attribute: HostGroupId: The id of the host group.
+        '''
+        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrHostGroupId"))
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
+            type_hints = typing.get_type_hints(_typecheckingstub__64b17f2ca7575201f9716c84ad7c9b12897fec04f8bddc01dfc408e94d0bdb6b)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "enableResourcePropertyConstraint", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="name")
+    def name(self) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''
+        :Property: name: Host group name.
+        '''
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], jsii.get(self, "name"))
+
+    @name.setter
+    def name(
+        self,
+        value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__d2c9ea8bddd864def280d048c36405159b03c531bfa54f32cf2e5d200bf60d87)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "name", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="organizationId")
+    def organization_id(
+        self,
+    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''
+        :Property: organizationId: Corporate identity, also known as enterprise id, can obtain in cloud effect access links.
+        '''
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], jsii.get(self, "organizationId"))
+
+    @organization_id.setter
+    def organization_id(
+        self,
+        value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__3339522019649fed954962ec2a55d4d56c3b7a18d6cc51d6f1ab5cf716371ff3)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "organizationId", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="serviceConnectionId")
+    def service_connection_id(
+        self,
+    ) -> typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''
+        :Property: serviceConnectionId: Service connection.
+        '''
+        return typing.cast(typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable], jsii.get(self, "serviceConnectionId"))
+
+    @service_connection_id.setter
+    def service_connection_id(
+        self,
+        value: typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__49f7b1978f7a3c444b7d90f44184124cc5e050c34c9c87884e7264e3a73e967c)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "serviceConnectionId", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="aliyunRegion")
+    def aliyun_region(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''
+        :Property: aliyunRegion: The aliyun region.
+        '''
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "aliyunRegion"))
+
+    @aliyun_region.setter
+    def aliyun_region(
+        self,
+        value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__247a785ce199458e2f2b120e91c5b3c84a640e4b05bbdf157e4fdeef94196f6b)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "aliyunRegion", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="ecsLabelKey")
+    def ecs_label_key(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''
+        :Property: ecsLabelKey: The tag key of the ECS.
+        '''
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "ecsLabelKey"))
+
+    @ecs_label_key.setter
+    def ecs_label_key(
+        self,
+        value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__7536c21064c05ddf81558496361ca1384abceb347055d3809bdc469858912548)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "ecsLabelKey", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="ecsLabelValue")
+    def ecs_label_value(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''
+        :Property: ecsLabelValue: The tag value of the ECS.
+        '''
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "ecsLabelValue"))
+
+    @ecs_label_value.setter
+    def ecs_label_value(
+        self,
+        value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__0348bf0eaf495f85c22cff22603a0d089813d561995788c11697b61cc77b2e05)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "ecsLabelValue", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="ecsType")
+    def ecs_type(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''
+        :Property: ecsType: The type of ECS, currently only supports ECS_ALIYUN.
+        '''
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "ecsType"))
+
+    @ecs_type.setter
+    def ecs_type(
+        self,
+        value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__a027dbacd9ef0270930e64a4379a3a2a867bfa3930d41c0616703c3329d32df3)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "ecsType", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="envId")
+    def env_id(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''
+        :Property: envId: Environment id.
+        '''
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "envId"))
+
+    @env_id.setter
+    def env_id(
+        self,
+        value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__5512b04622312f47bf834113425f008a7ba942680cae5590b66c99b8b533153b)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "envId", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="machineInfos")
+    def machine_infos(
+        self,
+    ) -> typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, "RosHostGroup.MachineInfosProperty"]]]]:
+        '''
+        :Property: machineInfos: The machine infos
+        '''
+        return typing.cast(typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, "RosHostGroup.MachineInfosProperty"]]]], jsii.get(self, "machineInfos"))
+
+    @machine_infos.setter
+    def machine_infos(
+        self,
+        value: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, "RosHostGroup.MachineInfosProperty"]]]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__4253055fd9144e6bbecfb684ac33197d5f13c545e1016727a0632ecbdc4a5e43)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "machineInfos", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="tagIds")
+    def tag_ids(
+        self,
+    ) -> typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]]]:
+        '''
+        :Property: tagIds: The ids of tag.
+        '''
+        return typing.cast(typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]]], jsii.get(self, "tagIds"))
+
+    @tag_ids.setter
+    def tag_ids(
+        self,
+        value: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__5820e2fb1d986915bd4d8d6d0ed502e151628d5ff04b2a2bd31643e20026311a)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "tagIds", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="type")
+    def type(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''
+        :Property: type: Host group type, currently only supports ECS.
+        '''
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "type"))
+
+    @type.setter
+    def type(
+        self,
+        value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__adc7db31bceb8771965c8e008fe6056debb3fadd7d3499579ef673fcdb6df5d8)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "type", value)
+
+    @jsii.data_type(
+        jsii_type="@alicloud/ros-cdk-devops.RosHostGroup.MachineInfosProperty",
+        jsii_struct_bases=[],
+        name_mapping={
+            "machine_sn": "machineSn",
+            "aliyun_region_id": "aliyunRegionId",
+            "instance_name": "instanceName",
+            "ip": "ip",
+        },
+    )
+    class MachineInfosProperty:
+        def __init__(
+            self,
+            *,
+            machine_sn: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+            aliyun_region_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+            instance_name: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+            ip: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+        ) -> None:
+            '''
+            :param machine_sn: 
+            :param aliyun_region_id: 
+            :param instance_name: 
+            :param ip: 
+            '''
+            if __debug__:
+                type_hints = typing.get_type_hints(_typecheckingstub__caacd68bb2744f1fbf24679c60f6270537bc1470452a6a5ef4cdb6c796885072)
+                check_type(argname="argument machine_sn", value=machine_sn, expected_type=type_hints["machine_sn"])
+                check_type(argname="argument aliyun_region_id", value=aliyun_region_id, expected_type=type_hints["aliyun_region_id"])
+                check_type(argname="argument instance_name", value=instance_name, expected_type=type_hints["instance_name"])
+                check_type(argname="argument ip", value=ip, expected_type=type_hints["ip"])
+            self._values: typing.Dict[builtins.str, typing.Any] = {
+                "machine_sn": machine_sn,
+            }
+            if aliyun_region_id is not None:
+                self._values["aliyun_region_id"] = aliyun_region_id
+            if instance_name is not None:
+                self._values["instance_name"] = instance_name
+            if ip is not None:
+                self._values["ip"] = ip
+
+        @builtins.property
+        def machine_sn(
+            self,
+        ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+            '''
+            :Property: machineSn: The id of the instance.
+            '''
+            result = self._values.get("machine_sn")
+            assert result is not None, "Required property 'machine_sn' is missing"
+            return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+        @builtins.property
+        def aliyun_region_id(
+            self,
+        ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+            '''
+            :Property: aliyunRegionId: The aliyun region of the instance.
+            '''
+            result = self._values.get("aliyun_region_id")
+            return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+        @builtins.property
+        def instance_name(
+            self,
+        ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+            '''
+            :Property: instanceName: The name of the instance.
+            '''
+            result = self._values.get("instance_name")
+            return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+        @builtins.property
+        def ip(
+            self,
+        ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+            '''
+            :Property: ip: The ip address of the instance.
+            '''
+            result = self._values.get("ip")
+            return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+        def __eq__(self, rhs: typing.Any) -> builtins.bool:
+            return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+        def __ne__(self, rhs: typing.Any) -> builtins.bool:
+            return not (rhs == self)
+
+        def __repr__(self) -> str:
+            return "MachineInfosProperty(%s)" % ", ".join(
+                k + "=" + repr(v) for k, v in self._values.items()
+            )
+
+
+@jsii.data_type(
+    jsii_type="@alicloud/ros-cdk-devops.RosHostGroupProps",
+    jsii_struct_bases=[],
+    name_mapping={
+        "name": "name",
+        "organization_id": "organizationId",
+        "service_connection_id": "serviceConnectionId",
+        "aliyun_region": "aliyunRegion",
+        "ecs_label_key": "ecsLabelKey",
+        "ecs_label_value": "ecsLabelValue",
+        "ecs_type": "ecsType",
+        "env_id": "envId",
+        "machine_infos": "machineInfos",
+        "tag_ids": "tagIds",
+        "type": "type",
+    },
+)
+class RosHostGroupProps:
+    def __init__(
+        self,
+        *,
+        name: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+        organization_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+        service_connection_id: typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable],
+        aliyun_region: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+        ecs_label_key: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+        ecs_label_value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+        ecs_type: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+        env_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+        machine_infos: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Sequence[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Union[RosHostGroup.MachineInfosProperty, typing.Dict[builtins.str, typing.Any]]]]]] = None,
+        tag_ids: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Sequence[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]]] = None,
+        type: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    ) -> None:
+        '''Properties for defining a ``RosHostGroup``.
+
+        See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-devops-hostgroup
+
+        :param name: 
+        :param organization_id: 
+        :param service_connection_id: 
+        :param aliyun_region: 
+        :param ecs_label_key: 
+        :param ecs_label_value: 
+        :param ecs_type: 
+        :param env_id: 
+        :param machine_infos: 
+        :param tag_ids: 
+        :param type: 
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__7206d2a0eab7e2006c690d939586cb056fb7f8d42fb647fadccb497c05e507b0)
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument organization_id", value=organization_id, expected_type=type_hints["organization_id"])
+            check_type(argname="argument service_connection_id", value=service_connection_id, expected_type=type_hints["service_connection_id"])
+            check_type(argname="argument aliyun_region", value=aliyun_region, expected_type=type_hints["aliyun_region"])
+            check_type(argname="argument ecs_label_key", value=ecs_label_key, expected_type=type_hints["ecs_label_key"])
+            check_type(argname="argument ecs_label_value", value=ecs_label_value, expected_type=type_hints["ecs_label_value"])
+            check_type(argname="argument ecs_type", value=ecs_type, expected_type=type_hints["ecs_type"])
+            check_type(argname="argument env_id", value=env_id, expected_type=type_hints["env_id"])
+            check_type(argname="argument machine_infos", value=machine_infos, expected_type=type_hints["machine_infos"])
+            check_type(argname="argument tag_ids", value=tag_ids, expected_type=type_hints["tag_ids"])
+            check_type(argname="argument type", value=type, expected_type=type_hints["type"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "name": name,
+            "organization_id": organization_id,
+            "service_connection_id": service_connection_id,
+        }
+        if aliyun_region is not None:
+            self._values["aliyun_region"] = aliyun_region
+        if ecs_label_key is not None:
+            self._values["ecs_label_key"] = ecs_label_key
+        if ecs_label_value is not None:
+            self._values["ecs_label_value"] = ecs_label_value
+        if ecs_type is not None:
+            self._values["ecs_type"] = ecs_type
+        if env_id is not None:
+            self._values["env_id"] = env_id
+        if machine_infos is not None:
+            self._values["machine_infos"] = machine_infos
+        if tag_ids is not None:
+            self._values["tag_ids"] = tag_ids
+        if type is not None:
+            self._values["type"] = type
+
+    @builtins.property
+    def name(self) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''
+        :Property: name: Host group name.
+        '''
+        result = self._values.get("name")
+        assert result is not None, "Required property 'name' is missing"
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+    @builtins.property
+    def organization_id(
+        self,
+    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''
+        :Property: organizationId: Corporate identity, also known as enterprise id, can obtain in cloud effect access links.
+        '''
+        result = self._values.get("organization_id")
+        assert result is not None, "Required property 'organization_id' is missing"
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+    @builtins.property
+    def service_connection_id(
+        self,
+    ) -> typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''
+        :Property: serviceConnectionId: Service connection.
+        '''
+        result = self._values.get("service_connection_id")
+        assert result is not None, "Required property 'service_connection_id' is missing"
+        return typing.cast(typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+    @builtins.property
+    def aliyun_region(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''
+        :Property: aliyunRegion: The aliyun region.
+        '''
+        result = self._values.get("aliyun_region")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+    @builtins.property
+    def ecs_label_key(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''
+        :Property: ecsLabelKey: The tag key of the ECS.
+        '''
+        result = self._values.get("ecs_label_key")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+    @builtins.property
+    def ecs_label_value(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''
+        :Property: ecsLabelValue: The tag value of the ECS.
+        '''
+        result = self._values.get("ecs_label_value")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+    @builtins.property
+    def ecs_type(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''
+        :Property: ecsType: The type of ECS, currently only supports ECS_ALIYUN.
+        '''
+        result = self._values.get("ecs_type")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+    @builtins.property
+    def env_id(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''
+        :Property: envId: Environment id.
+        '''
+        result = self._values.get("env_id")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+    @builtins.property
+    def machine_infos(
+        self,
+    ) -> typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, RosHostGroup.MachineInfosProperty]]]]:
+        '''
+        :Property: machineInfos: The machine infos
+        '''
+        result = self._values.get("machine_infos")
+        return typing.cast(typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, RosHostGroup.MachineInfosProperty]]]], result)
+
+    @builtins.property
+    def tag_ids(
+        self,
+    ) -> typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]]]:
+        '''
+        :Property: tagIds: The ids of tag.
+        '''
+        result = self._values.get("tag_ids")
+        return typing.cast(typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]]], result)
+
+    @builtins.property
+    def type(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''
+        :Property: type: Host group type, currently only supports ECS.
+        '''
+        result = self._values.get("type")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "RosHostGroupProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
 class RosPipeline(
     _ros_cdk_core_7adfd82f.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-devops.RosPipeline",
 ):
     '''This class is a base encapsulation around the ROS resource type ``ALIYUN::DEVOPS::Pipeline``, which is used to create a pipeline.
 
@@ -1863,34 +2735,88 @@
     def __repr__(self) -> str:
         return "VariableGroupProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 __all__ = [
+    "HostGroup",
+    "HostGroupProps",
     "Pipeline",
     "PipelineProps",
     "PipelineRelations",
     "PipelineRelationsProps",
     "PipelineRun",
     "PipelineRunProps",
+    "RosHostGroup",
+    "RosHostGroupProps",
     "RosPipeline",
     "RosPipelineProps",
     "RosPipelineRelations",
     "RosPipelineRelationsProps",
     "RosPipelineRun",
     "RosPipelineRunProps",
     "RosVariableGroup",
     "RosVariableGroupProps",
     "VariableGroup",
     "VariableGroupProps",
 ]
 
 publication.publish()
 
+def _typecheckingstub__d57d664cd9856802b0eafdcdfc868df58424b0f6865e48fa0cfdef1b0edfe430(
+    scope: _ros_cdk_core_7adfd82f.Construct,
+    id: builtins.str,
+    props: typing.Union[HostGroupProps, typing.Dict[builtins.str, typing.Any]],
+    enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__6ee7c5ba5b674bb6b0c2574a544f90904abd14d7b0a55062f84f41b1b4f55704(
+    value: builtins.bool,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__93a3dd2c14ab056517e5a1d17bc1dc4928a6c69008f3c9747cacb62fffa88ec7(
+    value: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__aee5e2d1b71f25ecd7a68fdf61a9826522f920533cd4a720a84d6a7b1533d631(
+    value: HostGroupProps,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__e0a64f2c2aedb570147001a8ecf480c3504691cc599c3a0aad531f0c2b7876aa(
+    value: _ros_cdk_core_7adfd82f.Construct,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__479b32c1718b7fc7c26bca41898094ff529fc13c791e8ec57615a728d8c090be(
+    *,
+    name: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    organization_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    service_connection_id: typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable],
+    aliyun_region: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    ecs_label_key: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    ecs_label_value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    ecs_type: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    env_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    machine_infos: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Sequence[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Union[RosHostGroup.MachineInfosProperty, typing.Dict[builtins.str, typing.Any]]]]]] = None,
+    tag_ids: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Sequence[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]]] = None,
+    type: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__41075a0ab71478dc9168b0be94b7354d99ac937ac95f5d59a0c4504e2db8ee69(
     scope: _ros_cdk_core_7adfd82f.Construct,
     id: builtins.str,
     props: typing.Union[PipelineProps, typing.Dict[builtins.str, typing.Any]],
     enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
 ) -> None:
     """Type checking stubs"""
@@ -2012,14 +2938,128 @@
     params: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Mapping[builtins.str, typing.Any]]] = None,
     sync: typing.Optional[typing.Union[builtins.bool, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     timeout: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__b4860cfe5cd458ab67e95e319ed56f8e68df738f346bd5820d127c20032bf0a1(
+    scope: _ros_cdk_core_7adfd82f.Construct,
+    id: builtins.str,
+    props: typing.Union[RosHostGroupProps, typing.Dict[builtins.str, typing.Any]],
+    enable_resource_property_constraint: builtins.bool,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__9cf5261897cc0b6de015b6775116f7aee1ff54e5cd0415193e139cfe8d09bf9f(
+    props: typing.Mapping[builtins.str, typing.Any],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__64b17f2ca7575201f9716c84ad7c9b12897fec04f8bddc01dfc408e94d0bdb6b(
+    value: builtins.bool,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__d2c9ea8bddd864def280d048c36405159b03c531bfa54f32cf2e5d200bf60d87(
+    value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__3339522019649fed954962ec2a55d4d56c3b7a18d6cc51d6f1ab5cf716371ff3(
+    value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__49f7b1978f7a3c444b7d90f44184124cc5e050c34c9c87884e7264e3a73e967c(
+    value: typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__247a785ce199458e2f2b120e91c5b3c84a640e4b05bbdf157e4fdeef94196f6b(
+    value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__7536c21064c05ddf81558496361ca1384abceb347055d3809bdc469858912548(
+    value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__0348bf0eaf495f85c22cff22603a0d089813d561995788c11697b61cc77b2e05(
+    value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__a027dbacd9ef0270930e64a4379a3a2a867bfa3930d41c0616703c3329d32df3(
+    value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__5512b04622312f47bf834113425f008a7ba942680cae5590b66c99b8b533153b(
+    value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__4253055fd9144e6bbecfb684ac33197d5f13c545e1016727a0632ecbdc4a5e43(
+    value: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, RosHostGroup.MachineInfosProperty]]]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__5820e2fb1d986915bd4d8d6d0ed502e151628d5ff04b2a2bd31643e20026311a(
+    value: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__adc7db31bceb8771965c8e008fe6056debb3fadd7d3499579ef673fcdb6df5d8(
+    value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__caacd68bb2744f1fbf24679c60f6270537bc1470452a6a5ef4cdb6c796885072(
+    *,
+    machine_sn: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    aliyun_region_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    instance_name: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    ip: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__7206d2a0eab7e2006c690d939586cb056fb7f8d42fb647fadccb497c05e507b0(
+    *,
+    name: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    organization_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    service_connection_id: typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable],
+    aliyun_region: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    ecs_label_key: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    ecs_label_value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    ecs_type: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    env_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    machine_infos: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Sequence[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Union[RosHostGroup.MachineInfosProperty, typing.Dict[builtins.str, typing.Any]]]]]] = None,
+    tag_ids: typing.Optional[typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Sequence[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]]] = None,
+    type: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__8bf3079d64432f73b0c8b9399684f7971e0a02556d241cf412884eccb72c9fdf(
     scope: _ros_cdk_core_7adfd82f.Construct,
     id: builtins.str,
     props: typing.Union[RosPipelineProps, typing.Dict[builtins.str, typing.Any]],
     enable_resource_property_constraint: builtins.bool,
 ) -> None:
     """Type checking stubs"""
```

### Comparing `ros-cdk-devops-1.0.24/src/ros_cdk_devops.egg-info/PKG-INFO` & `ros-cdk-devops-1.0.25/src/ros_cdk_devops.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-devops
-Version: 1.0.24
+Version: 1.0.25
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS DEVOPS Construct Library
```

