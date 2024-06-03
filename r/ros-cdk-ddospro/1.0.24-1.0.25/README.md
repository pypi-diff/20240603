# Comparing `tmp/ros-cdk-ddospro-1.0.24.tar.gz` & `tmp/ros-cdk-ddospro-1.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-ddospro-1.0.24.tar", last modified: Wed Apr 10 03:10:30 2024, max compression
+gzip compressed data, was "dist/ros-cdk-ddospro-1.0.25.tar", last modified: Mon Jun  3 11:16:44 2024, max compression
```

## Comparing `ros-cdk-ddospro-1.0.24.tar` & `ros-cdk-ddospro-1.0.25.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/
--rw-r--r--   0 root         (0) root         (0)    10279 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1308 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      191 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1900 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/src/ros_cdk_ddospro/
--rw-r--r--   0 root         (0) root         (0)   120981 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/src/ros_cdk_ddospro/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/src/ros_cdk_ddospro/_jsii/
--rw-r--r--   0 root         (0) root         (0)      427 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/src/ros_cdk_ddospro/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    47859 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/src/ros_cdk_ddospro/_jsii/ros-cdk-ddospro@1.0.24.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/src/ros_cdk_ddospro/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/src/ros_cdk_ddospro.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1308 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/src/ros_cdk_ddospro.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      441 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/src/ros_cdk_ddospro.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/src/ros_cdk_ddospro.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      110 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/src/ros_cdk_ddospro.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/src/ros_cdk_ddospro.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:16:44.000000 ros-cdk-ddospro-1.0.25/
+-rw-r--r--   0 root         (0) root         (0)    10279 2024-06-03 11:16:44.000000 ros-cdk-ddospro-1.0.25/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2024-06-03 11:16:44.000000 ros-cdk-ddospro-1.0.25/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2024-06-03 11:16:44.000000 ros-cdk-ddospro-1.0.25/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1308 2024-06-03 11:16:44.000000 ros-cdk-ddospro-1.0.25/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      191 2024-06-03 11:16:44.000000 ros-cdk-ddospro-1.0.25/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2024-06-03 11:16:44.000000 ros-cdk-ddospro-1.0.25/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-06-03 11:16:44.000000 ros-cdk-ddospro-1.0.25/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1901 2024-06-03 11:16:44.000000 ros-cdk-ddospro-1.0.25/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:16:44.000000 ros-cdk-ddospro-1.0.25/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:16:44.000000 ros-cdk-ddospro-1.0.25/src/ros_cdk_ddospro/
+-rw-r--r--   0 root         (0) root         (0)   210834 2024-06-03 11:16:44.000000 ros-cdk-ddospro-1.0.25/src/ros_cdk_ddospro/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:16:44.000000 ros-cdk-ddospro-1.0.25/src/ros_cdk_ddospro/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      427 2024-06-03 11:16:44.000000 ros-cdk-ddospro-1.0.25/src/ros_cdk_ddospro/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    69894 2024-06-03 11:16:44.000000 ros-cdk-ddospro-1.0.25/src/ros_cdk_ddospro/_jsii/ros-cdk-ddospro@1.0.25.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 11:16:44.000000 ros-cdk-ddospro-1.0.25/src/ros_cdk_ddospro/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:16:44.000000 ros-cdk-ddospro-1.0.25/src/ros_cdk_ddospro.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1308 2024-06-03 11:16:44.000000 ros-cdk-ddospro-1.0.25/src/ros_cdk_ddospro.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      441 2024-06-03 11:16:44.000000 ros-cdk-ddospro-1.0.25/src/ros_cdk_ddospro.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 11:16:44.000000 ros-cdk-ddospro-1.0.25/src/ros_cdk_ddospro.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      111 2024-06-03 11:16:44.000000 ros-cdk-ddospro-1.0.25/src/ros_cdk_ddospro.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-06-03 11:16:44.000000 ros-cdk-ddospro-1.0.25/src/ros_cdk_ddospro.egg-info/top_level.txt
```

### Comparing `ros-cdk-ddospro-1.0.24/LICENSE` & `ros-cdk-ddospro-1.0.25/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-ddospro-1.0.24/PKG-INFO` & `ros-cdk-ddospro-1.0.25/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-ddospro
-Version: 1.0.24
+Version: 1.0.25
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS DDOSPRO Construct Library
```

### Comparing `ros-cdk-ddospro-1.0.24/setup.py` & `ros-cdk-ddospro-1.0.25/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-ddospro",
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
         "ros_cdk_ddospro",
         "ros_cdk_ddospro._jsii"
     ],
     "package_data": {
         "ros_cdk_ddospro._jsii": [
-            "ros-cdk-ddospro@1.0.24.jsii.tgz"
+            "ros-cdk-ddospro@1.0.25.jsii.tgz"
         ],
         "ros_cdk_ddospro": [
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

### Comparing `ros-cdk-ddospro-1.0.24/src/ros_cdk_ddospro/__init__.py` & `ros-cdk-ddospro-1.0.25/src/ros_cdk_ddospro/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,20 +20,224 @@
 from typeguard import check_type
 
 from ._jsii import *
 
 import ros_cdk_core as _ros_cdk_core_7adfd82f
 
 
+class Port(
+    _ros_cdk_core_7adfd82f.Resource,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@alicloud/ros-cdk-ddospro.Port",
+):
+    '''This class encapsulates and extends the ROS resource type ``ALIYUN::DDoSPro::Port``.
+
+    :Note:
+
+    This class may have some new functions to facilitate development, so it is recommended to use this class instead of ``RosPort``for a more convenient development experience.
+    See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-ddospro-port
+    '''
+
+    def __init__(
+        self,
+        scope: _ros_cdk_core_7adfd82f.Construct,
+        id: builtins.str,
+        props: typing.Union["PortProps", typing.Dict[builtins.str, typing.Any]],
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
+            type_hints = typing.get_type_hints(_typecheckingstub__3f70c2d2847e542843c1d8d77eba744a3e024f669e64a97cb155f8d0117b18b4)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
+        jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
+
+    @builtins.property
+    @jsii.member(jsii_name="attrFrontendPort")
+    def attr_frontend_port(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+        '''Attribute FrontendPort: The forwarding port.'''
+        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrFrontendPort"))
+
+    @builtins.property
+    @jsii.member(jsii_name="enableResourcePropertyConstraint")
+    def _enable_resource_property_constraint(self) -> builtins.bool:
+        return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
+
+    @_enable_resource_property_constraint.setter
+    def _enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__91dafd6d09b28f08d954e82cb5ee3ab2ad6396a435e21ff614d5ddae910800f9)
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
+            type_hints = typing.get_type_hints(_typecheckingstub__fd3de6e1292475f86d1433e5bace8055f5104f4debafb0df2ec34ed6247205b1)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "id", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="props")
+    def _props(self) -> "PortProps":
+        return typing.cast("PortProps", jsii.get(self, "props"))
+
+    @_props.setter
+    def _props(self, value: "PortProps") -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__b008bc42c33b5ec2fdba150358962f414f3a844172ffec5998c399db0633e642)
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
+            type_hints = typing.get_type_hints(_typecheckingstub__e7d387b2cd84046a76a7a810c20eb19864438702fb9519c2fa42c6e021b8ea30)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "scope", value)
+
+
+@jsii.data_type(
+    jsii_type="@alicloud/ros-cdk-ddospro.PortProps",
+    jsii_struct_bases=[],
+    name_mapping={
+        "frontend_protocol": "frontendProtocol",
+        "instance_id": "instanceId",
+        "real_servers": "realServers",
+        "backend_port": "backendPort",
+        "frontend_port": "frontendPort",
+    },
+)
+class PortProps:
+    def __init__(
+        self,
+        *,
+        frontend_protocol: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+        instance_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+        real_servers: typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Sequence[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]],
+        backend_port: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+        frontend_port: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    ) -> None:
+        '''Properties for defining a ``Port``.
+
+        See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-ddospro-port
+
+        :param frontend_protocol: Property frontendProtocol: The type of the protocol. Valid values: tcp udp
+        :param instance_id: Property instanceId: The ID of the Anti-DDoS Pro or Anti-DDoS Premium instance to which the port forwarding rule belongs.
+        :param real_servers: Property realServers: An array that consists of the IP addresses of origin servers.
+        :param backend_port: Property backendPort: The port of the origin server. Valid values: 0 to 65535.
+        :param frontend_port: Property frontendPort: The forwarding port. Valid values: 0 to 65535.
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__907744fc156a231aebd7307dad220a1be51c48da2aaf6d35ea3fee309e7ac498)
+            check_type(argname="argument frontend_protocol", value=frontend_protocol, expected_type=type_hints["frontend_protocol"])
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+            check_type(argname="argument real_servers", value=real_servers, expected_type=type_hints["real_servers"])
+            check_type(argname="argument backend_port", value=backend_port, expected_type=type_hints["backend_port"])
+            check_type(argname="argument frontend_port", value=frontend_port, expected_type=type_hints["frontend_port"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "frontend_protocol": frontend_protocol,
+            "instance_id": instance_id,
+            "real_servers": real_servers,
+        }
+        if backend_port is not None:
+            self._values["backend_port"] = backend_port
+        if frontend_port is not None:
+            self._values["frontend_port"] = frontend_port
+
+    @builtins.property
+    def frontend_protocol(
+        self,
+    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''Property frontendProtocol: The type of the protocol.
+
+        Valid values:
+        tcp
+        udp
+        '''
+        result = self._values.get("frontend_protocol")
+        assert result is not None, "Required property 'frontend_protocol' is missing"
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+    @builtins.property
+    def instance_id(
+        self,
+    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''Property instanceId: The ID of the Anti-DDoS Pro or Anti-DDoS Premium instance to which the port forwarding rule belongs.'''
+        result = self._values.get("instance_id")
+        assert result is not None, "Required property 'instance_id' is missing"
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+    @builtins.property
+    def real_servers(
+        self,
+    ) -> typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]]:
+        '''Property realServers: An array that consists of the IP addresses of origin servers.'''
+        result = self._values.get("real_servers")
+        assert result is not None, "Required property 'real_servers' is missing"
+        return typing.cast(typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]], result)
+
+    @builtins.property
+    def backend_port(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''Property backendPort: The port of the origin server.
+
+        Valid values: 0 to 65535.
+        '''
+        result = self._values.get("backend_port")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+    @builtins.property
+    def frontend_port(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''Property frontendPort: The forwarding port.
+
+        Valid values: 0 to 65535.
+        '''
+        result = self._values.get("frontend_port")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "PortProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
 class PremiumInstance(
     _ros_cdk_core_7adfd82f.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-ddospro.PremiumInstance",
 ):
-    '''This class encapsulates and extends the ROS resource type ``ALIYUN::DDoSPro::PremiumInstance``.
+    '''This class encapsulates and extends the ROS resource type ``ALIYUN::DDoSPro::PremiumInstance``, which is used to create an Anti-DDoS Proxy (Outside Chinese Mainland) instance.
 
     :Note:
 
     This class may have some new functions to facilitate development, so it is recommended to use this class instead of ``RosPremiumInstance``for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-ddospro-premiuminstance
     '''
 
@@ -341,15 +545,15 @@
 
 
 class ProInstance(
     _ros_cdk_core_7adfd82f.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-ddospro.ProInstance",
 ):
-    '''This class encapsulates and extends the ROS resource type ``ALIYUN::DDoSPro::ProInstance``.
+    '''This class encapsulates and extends the ROS resource type ``ALIYUN::DDoSPro::ProInstance``, which is used to create an Anti-DDoS Proxy (Chinese Mainland) instance.
 
     :Note:
 
     This class may have some new functions to facilitate development, so it is recommended to use this class instead of ``RosProInstance``for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-ddospro-proinstance
     '''
 
@@ -702,20 +906,320 @@
 
     def __repr__(self) -> str:
         return "ProInstanceProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
+class RosPort(
+    _ros_cdk_core_7adfd82f.RosResource,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@alicloud/ros-cdk-ddospro.RosPort",
+):
+    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::DDoSPro::Port``.
+
+    :Note:
+
+    This class does not contain additional functions, so it is recommended to use the ``Port`` class instead of this class for a more convenient development experience.
+    See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-ddospro-port
+    '''
+
+    def __init__(
+        self,
+        scope: _ros_cdk_core_7adfd82f.Construct,
+        id: builtins.str,
+        props: typing.Union["RosPortProps", typing.Dict[builtins.str, typing.Any]],
+        enable_resource_property_constraint: builtins.bool,
+    ) -> None:
+        '''
+        :param scope: - scope in which this resource is defined.
+        :param id: - scoped id of the resource.
+        :param props: - resource properties.
+        :param enable_resource_property_constraint: -
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__95f58b3961978a678cb526ddf1d9e63dfcd302d754f72f3251108bdd9b6b181e)
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
+            type_hints = typing.get_type_hints(_typecheckingstub__51bde9afd2129ec87892e5568da2293106c5beee25f324118999c46020c8d0e0)
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
+    @jsii.member(jsii_name="attrFrontendPort")
+    def attr_frontend_port(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+        '''
+        :Attribute: FrontendPort: The forwarding port.
+        '''
+        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrFrontendPort"))
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
+            type_hints = typing.get_type_hints(_typecheckingstub__773bc27b9fc469e411f4c2fbceeb3822e12c7ae3200c509f393048bfc0056e2d)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "enableResourcePropertyConstraint", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="frontendProtocol")
+    def frontend_protocol(
+        self,
+    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''
+        :Property:
+
+        frontendProtocol: The type of the protocol. Valid values:
+        tcp
+        udp
+        '''
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], jsii.get(self, "frontendProtocol"))
+
+    @frontend_protocol.setter
+    def frontend_protocol(
+        self,
+        value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__3edc74c43574f6bd8385c61317ce5d1c99f9c6f9680fd0c1da8b3616650a9418)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "frontendProtocol", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="instanceId")
+    def instance_id(
+        self,
+    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''
+        :Property: instanceId: The ID of the Anti-DDoS Pro or Anti-DDoS Premium instance to which the port forwarding rule belongs.
+        '''
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], jsii.get(self, "instanceId"))
+
+    @instance_id.setter
+    def instance_id(
+        self,
+        value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__43db68d39f39808599075609b859dc00712761f0b1f3dd60d67a0e64fae1c1c8)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "instanceId", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="realServers")
+    def real_servers(
+        self,
+    ) -> typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]]:
+        '''
+        :Property: realServers: An array that consists of the IP addresses of origin servers.
+        '''
+        return typing.cast(typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]], jsii.get(self, "realServers"))
+
+    @real_servers.setter
+    def real_servers(
+        self,
+        value: typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__df6314c4b38aeacd729ef9087c64142c497dc811abebab6883731142af835e24)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "realServers", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="backendPort")
+    def backend_port(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''
+        :Property: backendPort: The port of the origin server. Valid values: 0 to 65535.
+        '''
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "backendPort"))
+
+    @backend_port.setter
+    def backend_port(
+        self,
+        value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__8fc5ac86ed13c1a1e4d5ac4d75b9d084045b364d472e1f1e38c170ceb4b97f47)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "backendPort", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="frontendPort")
+    def frontend_port(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''
+        :Property: frontendPort: The forwarding port. Valid values: 0 to 65535.
+        '''
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "frontendPort"))
+
+    @frontend_port.setter
+    def frontend_port(
+        self,
+        value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__28884777e4811b3a408c94c5511c9d3864129a09951f6d2a62457bb8c01326a3)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "frontendPort", value)
+
+
+@jsii.data_type(
+    jsii_type="@alicloud/ros-cdk-ddospro.RosPortProps",
+    jsii_struct_bases=[],
+    name_mapping={
+        "frontend_protocol": "frontendProtocol",
+        "instance_id": "instanceId",
+        "real_servers": "realServers",
+        "backend_port": "backendPort",
+        "frontend_port": "frontendPort",
+    },
+)
+class RosPortProps:
+    def __init__(
+        self,
+        *,
+        frontend_protocol: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+        instance_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+        real_servers: typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Sequence[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]],
+        backend_port: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+        frontend_port: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    ) -> None:
+        '''Properties for defining a ``RosPort``.
+
+        See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-ddospro-port
+
+        :param frontend_protocol: 
+        :param instance_id: 
+        :param real_servers: 
+        :param backend_port: 
+        :param frontend_port: 
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__19e84d824c2563111a3e1265cecc3b8ecd6f9fda05fabe200ccc24cf5b32318c)
+            check_type(argname="argument frontend_protocol", value=frontend_protocol, expected_type=type_hints["frontend_protocol"])
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+            check_type(argname="argument real_servers", value=real_servers, expected_type=type_hints["real_servers"])
+            check_type(argname="argument backend_port", value=backend_port, expected_type=type_hints["backend_port"])
+            check_type(argname="argument frontend_port", value=frontend_port, expected_type=type_hints["frontend_port"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "frontend_protocol": frontend_protocol,
+            "instance_id": instance_id,
+            "real_servers": real_servers,
+        }
+        if backend_port is not None:
+            self._values["backend_port"] = backend_port
+        if frontend_port is not None:
+            self._values["frontend_port"] = frontend_port
+
+    @builtins.property
+    def frontend_protocol(
+        self,
+    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''
+        :Property:
+
+        frontendProtocol: The type of the protocol. Valid values:
+        tcp
+        udp
+        '''
+        result = self._values.get("frontend_protocol")
+        assert result is not None, "Required property 'frontend_protocol' is missing"
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+    @builtins.property
+    def instance_id(
+        self,
+    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''
+        :Property: instanceId: The ID of the Anti-DDoS Pro or Anti-DDoS Premium instance to which the port forwarding rule belongs.
+        '''
+        result = self._values.get("instance_id")
+        assert result is not None, "Required property 'instance_id' is missing"
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+    @builtins.property
+    def real_servers(
+        self,
+    ) -> typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]]:
+        '''
+        :Property: realServers: An array that consists of the IP addresses of origin servers.
+        '''
+        result = self._values.get("real_servers")
+        assert result is not None, "Required property 'real_servers' is missing"
+        return typing.cast(typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]], result)
+
+    @builtins.property
+    def backend_port(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''
+        :Property: backendPort: The port of the origin server. Valid values: 0 to 65535.
+        '''
+        result = self._values.get("backend_port")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+    @builtins.property
+    def frontend_port(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''
+        :Property: frontendPort: The forwarding port. Valid values: 0 to 65535.
+        '''
+        result = self._values.get("frontend_port")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "RosPortProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
 class RosPremiumInstance(
     _ros_cdk_core_7adfd82f.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-ddospro.RosPremiumInstance",
 ):
-    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::DDoSPro::PremiumInstance``.
+    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::DDoSPro::PremiumInstance``, which is used to create an Anti-DDoS Proxy (Outside Chinese Mainland) instance.
 
     :Note:
 
     This class does not contain additional functions, so it is recommended to use the ``PremiumInstance`` class instead of this class for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-ddospro-premiuminstance
     '''
 
@@ -1332,15 +1836,15 @@
 
 
 class RosProInstance(
     _ros_cdk_core_7adfd82f.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-ddospro.RosProInstance",
 ):
-    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::DDoSPro::ProInstance``.
+    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::DDoSPro::ProInstance``, which is used to create an Anti-DDoS Proxy (Chinese Mainland) instance.
 
     :Note:
 
     This class does not contain additional functions, so it is recommended to use the ``ProInstance`` class instead of this class for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-ddospro-proinstance
     '''
 
@@ -2064,27 +2568,1064 @@
 
     def __repr__(self) -> str:
         return "RosProInstanceProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
+class RosSceneDefensePolicy(
+    _ros_cdk_core_7adfd82f.RosResource,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@alicloud/ros-cdk-ddospro.RosSceneDefensePolicy",
+):
+    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::DDoSPro::SceneDefensePolicy``.
+
+    :Note:
+
+    This class does not contain additional functions, so it is recommended to use the ``SceneDefensePolicy`` class instead of this class for a more convenient development experience.
+    See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-ddospro-scenedefensepolicy
+    '''
+
+    def __init__(
+        self,
+        scope: _ros_cdk_core_7adfd82f.Construct,
+        id: builtins.str,
+        props: typing.Union["RosSceneDefensePolicyProps", typing.Dict[builtins.str, typing.Any]],
+        enable_resource_property_constraint: builtins.bool,
+    ) -> None:
+        '''
+        :param scope: - scope in which this resource is defined.
+        :param id: - scoped id of the resource.
+        :param props: - resource properties.
+        :param enable_resource_property_constraint: -
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__c1756817e5470835ce70e52ce71e0da06d5355d242707ac9e4d6564830214744)
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
+            type_hints = typing.get_type_hints(_typecheckingstub__10877624c40ac4a6d8f5d908aedb30d2485f56960436d4a89e03c824fb1a8513)
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
+    @jsii.member(jsii_name="attrName")
+    def attr_name(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+        '''
+        :Attribute: Name: The name of the policy.
+        '''
+        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrName"))
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
+            type_hints = typing.get_type_hints(_typecheckingstub__4c236ba3393f24baf7936c92334f84202c5c9c09244e4512a10d82ac69fe7a28)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "enableResourcePropertyConstraint", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="endTime")
+    def end_time(self) -> typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''
+        :Property: endTime: The end time of the policy. This value is a UNIX timestamp. Units: milliseconds.
+        '''
+        return typing.cast(typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable], jsii.get(self, "endTime"))
+
+    @end_time.setter
+    def end_time(
+        self,
+        value: typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__ed53a0d4517ba1ad2639e70b4635f37a23e5ba3786f97a10682265b17ba36fbc)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "endTime", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="name")
+    def name(self) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''
+        :Property: name: The name of the policy.
+        '''
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], jsii.get(self, "name"))
+
+    @name.setter
+    def name(
+        self,
+        value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__6f3a028fcafc037007dafb6c106ce38356cd75ec29bec1a160e54afce2002107)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "name", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="startTime")
+    def start_time(
+        self,
+    ) -> typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''
+        :Property: startTime: The start time of the policy. This value is a UNIX timestamp. Units: milliseconds.
+        '''
+        return typing.cast(typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable], jsii.get(self, "startTime"))
+
+    @start_time.setter
+    def start_time(
+        self,
+        value: typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__3bdabd778dc2fef602ae352d5af634d61baceab6f10d50c2a9a409023933e147)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "startTime", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="template")
+    def template(
+        self,
+    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''
+        :Property:
+
+        template: The template of the policy. Valid values:
+        promotion: important activity
+        bypass: all traffic forwarded
+        '''
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], jsii.get(self, "template"))
+
+    @template.setter
+    def template(
+        self,
+        value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__dcd0b375d29eef514c53faafe927bb1e6c256f6d5eff7c0b9b5ce83f9ebf46b2)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "template", value)
+
+
+@jsii.data_type(
+    jsii_type="@alicloud/ros-cdk-ddospro.RosSceneDefensePolicyProps",
+    jsii_struct_bases=[],
+    name_mapping={
+        "end_time": "endTime",
+        "name": "name",
+        "start_time": "startTime",
+        "template": "template",
+    },
+)
+class RosSceneDefensePolicyProps:
+    def __init__(
+        self,
+        *,
+        end_time: typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable],
+        name: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+        start_time: typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable],
+        template: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    ) -> None:
+        '''Properties for defining a ``RosSceneDefensePolicy``.
+
+        See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-ddospro-scenedefensepolicy
+
+        :param end_time: 
+        :param name: 
+        :param start_time: 
+        :param template: 
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__8625addc2cb7cc74e1f6bd8c069c274eb1750600d0c8a559cfc061638decc206)
+            check_type(argname="argument end_time", value=end_time, expected_type=type_hints["end_time"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument start_time", value=start_time, expected_type=type_hints["start_time"])
+            check_type(argname="argument template", value=template, expected_type=type_hints["template"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "end_time": end_time,
+            "name": name,
+            "start_time": start_time,
+            "template": template,
+        }
+
+    @builtins.property
+    def end_time(self) -> typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''
+        :Property: endTime: The end time of the policy. This value is a UNIX timestamp. Units: milliseconds.
+        '''
+        result = self._values.get("end_time")
+        assert result is not None, "Required property 'end_time' is missing"
+        return typing.cast(typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+    @builtins.property
+    def name(self) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''
+        :Property: name: The name of the policy.
+        '''
+        result = self._values.get("name")
+        assert result is not None, "Required property 'name' is missing"
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+    @builtins.property
+    def start_time(
+        self,
+    ) -> typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''
+        :Property: startTime: The start time of the policy. This value is a UNIX timestamp. Units: milliseconds.
+        '''
+        result = self._values.get("start_time")
+        assert result is not None, "Required property 'start_time' is missing"
+        return typing.cast(typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+    @builtins.property
+    def template(
+        self,
+    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''
+        :Property:
+
+        template: The template of the policy. Valid values:
+        promotion: important activity
+        bypass: all traffic forwarded
+        '''
+        result = self._values.get("template")
+        assert result is not None, "Required property 'template' is missing"
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "RosSceneDefensePolicyProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+class RosSchedulerRule(
+    _ros_cdk_core_7adfd82f.RosResource,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@alicloud/ros-cdk-ddospro.RosSchedulerRule",
+):
+    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::DDoSPro::SchedulerRule``.
+
+    :Note:
+
+    This class does not contain additional functions, so it is recommended to use the ``SchedulerRule`` class instead of this class for a more convenient development experience.
+    See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-ddospro-schedulerrule
+    '''
+
+    def __init__(
+        self,
+        scope: _ros_cdk_core_7adfd82f.Construct,
+        id: builtins.str,
+        props: typing.Union["RosSchedulerRuleProps", typing.Dict[builtins.str, typing.Any]],
+        enable_resource_property_constraint: builtins.bool,
+    ) -> None:
+        '''
+        :param scope: - scope in which this resource is defined.
+        :param id: - scoped id of the resource.
+        :param props: - resource properties.
+        :param enable_resource_property_constraint: -
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__60d7d56fe23e71859342593f2659f2a0880b0a528284a704533719ab2a5a6afa)
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
+            type_hints = typing.get_type_hints(_typecheckingstub__fdfe932b810ddbf2234a04107688f8d11c91cd79938f4ae4ee79ea7b834cc4f8)
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
+    @jsii.member(jsii_name="attrRuleName")
+    def attr_rule_name(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+        '''
+        :Attribute: RuleName: The name of the rule.
+        '''
+        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrRuleName"))
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
+            type_hints = typing.get_type_hints(_typecheckingstub__2cf1ed8abb21815fb04fb23b6523c73e866acf5d94bb14e3f4fb6a8ea9a4f250)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "enableResourcePropertyConstraint", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="ruleName")
+    def rule_name(
+        self,
+    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''
+        :Property: ruleName: The name of the rule.
+        '''
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], jsii.get(self, "ruleName"))
+
+    @rule_name.setter
+    def rule_name(
+        self,
+        value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__755af63a3d4d6f036f0cde3a666fafa09e3a80a1f25b8bba2ea988cb91ed0642)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "ruleName", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="rules")
+    def rules(self) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''
+        :Property:
+
+        rules: The details of the scheduling rule. This parameter is a JSON string. The following list describes the fields in the value of the parameter:
+        Type: the address type of the interaction resource that you want to use in the scheduling rule. This field is required and must be of the string type. Valid values: A: IP address. CNAME: domain name
+        Value: the address of the interaction resource that you want to use in the scheduling rule. This field is required and must be of the string type.
+        Priority: the priority of the scheduling rule. This field is required and must be of the integer type. Valid values: 0 to 100. A larger value indicates a higher priority.
+        ValueType: the type of the interaction resource that you want to use in the scheduling rule. This field is required and must be of the integer type. Valid values: 1: the IP address of the Anti-DDoS Pro or Anti-DDoS Premium instance. 2: the IP address of the interaction resource in the tiered protection scenario. 3: the IP address that is used to accelerate access in the network acceleration scenario. 5: the domain name that is configured in Alibaba Cloud CDN (CDN) in the CDN interaction scenario. 6 the IP address of the interaction resource in the cloud service interaction scenario
+        RegionId: the region where the interaction resource is deployed. This parameter must be specified when ValueType is set to 2. The value must be of the string type.
+        '''
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], jsii.get(self, "rules"))
+
+    @rules.setter
+    def rules(
+        self,
+        value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__25833a1ebbfbdbba810d83857e97c86feeaa5c86b3ace4eaaec390a0837a4782)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "rules", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="ruleType")
+    def rule_type(
+        self,
+    ) -> typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''
+        :Property:
+
+        ruleType: The type of the custom defense rule. Valid values:
+        2: tiered protection
+        3: network acceleration
+        5: CDN interaction
+        6: cloud service interaction
+        8: secure acceleration
+        '''
+        return typing.cast(typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable], jsii.get(self, "ruleType"))
+
+    @rule_type.setter
+    def rule_type(
+        self,
+        value: typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__36bd17e92e34915d373b70c24b5d5818fcaf8a1610fb5855c922ba0aab7fb49a)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "ruleType", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="param")
+    def param(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''
+        :Property:
+
+        param: The details of the CDN interaction rule. This parameter is a JSON string. The following list describes the fields in the value of the parameter:
+        ParamType: the type of the scheduling rule. This field is required and must be of the string type. Set the value to cdn. This indicates that you want to modify a CDN interaction rule.
+        ParamData: the values of parameters that you want to modify for the CDN interaction rule. This field is required and must be of the map type. ParamData contains the following parameters: Domain: the accelerated domain in CDN. This parameter is required and must be of the string type; Cname: the CNAME that is assigned to the accelerated domain. This parameter is required and must be of the string type; AccessQps: the queries per second (QPS) threshold that is used to switch service traffic to Anti-DDoS Pro or Anti-DDoS Premium. This parameter is required and must be of the integer type; UpstreamQps: the QPS threshold that is used to switch service traffic to CDN. This parameter is optional and must be of the integer type.
+        '''
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "param"))
+
+    @param.setter
+    def param(
+        self,
+        value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__269cef1b9a3ea9580b02bdd7b1882e5a5d0682a57d3958b4f249a8f3f7c09cd3)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "param", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="resourceGroupId")
+    def resource_group_id(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''
+        :Property: resourceGroupId: The ID of the resource group to which the instance belongs in Resource Management. This parameter is empty by default, which indicates that the instance belongs to the default resource group.
+        '''
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], jsii.get(self, "resourceGroupId"))
+
+    @resource_group_id.setter
+    def resource_group_id(
+        self,
+        value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__c8e87eed91d6d64e6f8e45ece62deed0fef32d1363b053c12156dc9002576459)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "resourceGroupId", value)
+
+
+@jsii.data_type(
+    jsii_type="@alicloud/ros-cdk-ddospro.RosSchedulerRuleProps",
+    jsii_struct_bases=[],
+    name_mapping={
+        "rule_name": "ruleName",
+        "rules": "rules",
+        "rule_type": "ruleType",
+        "param": "param",
+        "resource_group_id": "resourceGroupId",
+    },
+)
+class RosSchedulerRuleProps:
+    def __init__(
+        self,
+        *,
+        rule_name: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+        rules: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+        rule_type: typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable],
+        param: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+        resource_group_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    ) -> None:
+        '''Properties for defining a ``RosSchedulerRule``.
+
+        See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-ddospro-schedulerrule
+
+        :param rule_name: 
+        :param rules: 
+        :param rule_type: 
+        :param param: 
+        :param resource_group_id: 
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__06878d13277cfd5d033015d37e320f287798899ac9d4657b17c84326a57526f8)
+            check_type(argname="argument rule_name", value=rule_name, expected_type=type_hints["rule_name"])
+            check_type(argname="argument rules", value=rules, expected_type=type_hints["rules"])
+            check_type(argname="argument rule_type", value=rule_type, expected_type=type_hints["rule_type"])
+            check_type(argname="argument param", value=param, expected_type=type_hints["param"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "rule_name": rule_name,
+            "rules": rules,
+            "rule_type": rule_type,
+        }
+        if param is not None:
+            self._values["param"] = param
+        if resource_group_id is not None:
+            self._values["resource_group_id"] = resource_group_id
+
+    @builtins.property
+    def rule_name(
+        self,
+    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''
+        :Property: ruleName: The name of the rule.
+        '''
+        result = self._values.get("rule_name")
+        assert result is not None, "Required property 'rule_name' is missing"
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+    @builtins.property
+    def rules(self) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''
+        :Property:
+
+        rules: The details of the scheduling rule. This parameter is a JSON string. The following list describes the fields in the value of the parameter:
+        Type: the address type of the interaction resource that you want to use in the scheduling rule. This field is required and must be of the string type. Valid values: A: IP address. CNAME: domain name
+        Value: the address of the interaction resource that you want to use in the scheduling rule. This field is required and must be of the string type.
+        Priority: the priority of the scheduling rule. This field is required and must be of the integer type. Valid values: 0 to 100. A larger value indicates a higher priority.
+        ValueType: the type of the interaction resource that you want to use in the scheduling rule. This field is required and must be of the integer type. Valid values: 1: the IP address of the Anti-DDoS Pro or Anti-DDoS Premium instance. 2: the IP address of the interaction resource in the tiered protection scenario. 3: the IP address that is used to accelerate access in the network acceleration scenario. 5: the domain name that is configured in Alibaba Cloud CDN (CDN) in the CDN interaction scenario. 6 the IP address of the interaction resource in the cloud service interaction scenario
+        RegionId: the region where the interaction resource is deployed. This parameter must be specified when ValueType is set to 2. The value must be of the string type.
+        '''
+        result = self._values.get("rules")
+        assert result is not None, "Required property 'rules' is missing"
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+    @builtins.property
+    def rule_type(
+        self,
+    ) -> typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''
+        :Property:
+
+        ruleType: The type of the custom defense rule. Valid values:
+        2: tiered protection
+        3: network acceleration
+        5: CDN interaction
+        6: cloud service interaction
+        8: secure acceleration
+        '''
+        result = self._values.get("rule_type")
+        assert result is not None, "Required property 'rule_type' is missing"
+        return typing.cast(typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+    @builtins.property
+    def param(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''
+        :Property:
+
+        param: The details of the CDN interaction rule. This parameter is a JSON string. The following list describes the fields in the value of the parameter:
+        ParamType: the type of the scheduling rule. This field is required and must be of the string type. Set the value to cdn. This indicates that you want to modify a CDN interaction rule.
+        ParamData: the values of parameters that you want to modify for the CDN interaction rule. This field is required and must be of the map type. ParamData contains the following parameters: Domain: the accelerated domain in CDN. This parameter is required and must be of the string type; Cname: the CNAME that is assigned to the accelerated domain. This parameter is required and must be of the string type; AccessQps: the queries per second (QPS) threshold that is used to switch service traffic to Anti-DDoS Pro or Anti-DDoS Premium. This parameter is required and must be of the integer type; UpstreamQps: the QPS threshold that is used to switch service traffic to CDN. This parameter is optional and must be of the integer type.
+        '''
+        result = self._values.get("param")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+    @builtins.property
+    def resource_group_id(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''
+        :Property: resourceGroupId: The ID of the resource group to which the instance belongs in Resource Management. This parameter is empty by default, which indicates that the instance belongs to the default resource group.
+        '''
+        result = self._values.get("resource_group_id")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "RosSchedulerRuleProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+class SceneDefensePolicy(
+    _ros_cdk_core_7adfd82f.Resource,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@alicloud/ros-cdk-ddospro.SceneDefensePolicy",
+):
+    '''This class encapsulates and extends the ROS resource type ``ALIYUN::DDoSPro::SceneDefensePolicy``.
+
+    :Note:
+
+    This class may have some new functions to facilitate development, so it is recommended to use this class instead of ``RosSceneDefensePolicy``for a more convenient development experience.
+    See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-ddospro-scenedefensepolicy
+    '''
+
+    def __init__(
+        self,
+        scope: _ros_cdk_core_7adfd82f.Construct,
+        id: builtins.str,
+        props: typing.Union["SceneDefensePolicyProps", typing.Dict[builtins.str, typing.Any]],
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
+            type_hints = typing.get_type_hints(_typecheckingstub__93a34aee76f73af63930ed237104de4318437451980b4d2a33bfd0008789e36a)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
+        jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
+
+    @builtins.property
+    @jsii.member(jsii_name="attrName")
+    def attr_name(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+        '''Attribute Name: The name of the policy.'''
+        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrName"))
+
+    @builtins.property
+    @jsii.member(jsii_name="enableResourcePropertyConstraint")
+    def _enable_resource_property_constraint(self) -> builtins.bool:
+        return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
+
+    @_enable_resource_property_constraint.setter
+    def _enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__091bb1aa84ae6c132d1c5e7832ede437b03efeae2f62863c89f3d33fb528860c)
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
+            type_hints = typing.get_type_hints(_typecheckingstub__a76d70f282f547d53e9b141d7047869bfd592d7ab08c961d780fac0c3778247e)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "id", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="props")
+    def _props(self) -> "SceneDefensePolicyProps":
+        return typing.cast("SceneDefensePolicyProps", jsii.get(self, "props"))
+
+    @_props.setter
+    def _props(self, value: "SceneDefensePolicyProps") -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__4db93203395771cc895257245c9c2daeddaf3e9c49acb76dca9041c837e12d41)
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
+            type_hints = typing.get_type_hints(_typecheckingstub__2091551606d1fcc71ccec8dff5318e86b02d6a7777a18564bc5cd6d483d0b111)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "scope", value)
+
+
+@jsii.data_type(
+    jsii_type="@alicloud/ros-cdk-ddospro.SceneDefensePolicyProps",
+    jsii_struct_bases=[],
+    name_mapping={
+        "end_time": "endTime",
+        "name": "name",
+        "start_time": "startTime",
+        "template": "template",
+    },
+)
+class SceneDefensePolicyProps:
+    def __init__(
+        self,
+        *,
+        end_time: typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable],
+        name: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+        start_time: typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable],
+        template: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    ) -> None:
+        '''Properties for defining a ``SceneDefensePolicy``.
+
+        See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-ddospro-scenedefensepolicy
+
+        :param end_time: Property endTime: The end time of the policy. This value is a UNIX timestamp. Units: milliseconds.
+        :param name: Property name: The name of the policy.
+        :param start_time: Property startTime: The start time of the policy. This value is a UNIX timestamp. Units: milliseconds.
+        :param template: Property template: The template of the policy. Valid values: promotion: important activity bypass: all traffic forwarded
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__7893eeae669d9101b3de6e4f33d023b50eb9d26ea21f6a1dd5f49c57a7aca6f0)
+            check_type(argname="argument end_time", value=end_time, expected_type=type_hints["end_time"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument start_time", value=start_time, expected_type=type_hints["start_time"])
+            check_type(argname="argument template", value=template, expected_type=type_hints["template"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "end_time": end_time,
+            "name": name,
+            "start_time": start_time,
+            "template": template,
+        }
+
+    @builtins.property
+    def end_time(self) -> typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''Property endTime: The end time of the policy.
+
+        This value is a UNIX timestamp. Units: milliseconds.
+        '''
+        result = self._values.get("end_time")
+        assert result is not None, "Required property 'end_time' is missing"
+        return typing.cast(typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+    @builtins.property
+    def name(self) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''Property name: The name of the policy.'''
+        result = self._values.get("name")
+        assert result is not None, "Required property 'name' is missing"
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+    @builtins.property
+    def start_time(
+        self,
+    ) -> typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''Property startTime: The start time of the policy.
+
+        This value is a UNIX timestamp. Units: milliseconds.
+        '''
+        result = self._values.get("start_time")
+        assert result is not None, "Required property 'start_time' is missing"
+        return typing.cast(typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+    @builtins.property
+    def template(
+        self,
+    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''Property template: The template of the policy.
+
+        Valid values:
+        promotion: important activity
+        bypass: all traffic forwarded
+        '''
+        result = self._values.get("template")
+        assert result is not None, "Required property 'template' is missing"
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "SceneDefensePolicyProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+class SchedulerRule(
+    _ros_cdk_core_7adfd82f.Resource,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@alicloud/ros-cdk-ddospro.SchedulerRule",
+):
+    '''This class encapsulates and extends the ROS resource type ``ALIYUN::DDoSPro::SchedulerRule``.
+
+    :Note:
+
+    This class may have some new functions to facilitate development, so it is recommended to use this class instead of ``RosSchedulerRule``for a more convenient development experience.
+    See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-ddospro-schedulerrule
+    '''
+
+    def __init__(
+        self,
+        scope: _ros_cdk_core_7adfd82f.Construct,
+        id: builtins.str,
+        props: typing.Union["SchedulerRuleProps", typing.Dict[builtins.str, typing.Any]],
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
+            type_hints = typing.get_type_hints(_typecheckingstub__31f5d9eab941d81a2abcb3f5f715b90b5f0d85ecb4853c191e37ea6c870e3162)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
+        jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
+
+    @builtins.property
+    @jsii.member(jsii_name="attrRuleName")
+    def attr_rule_name(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+        '''Attribute RuleName: The name of the rule.'''
+        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrRuleName"))
+
+    @builtins.property
+    @jsii.member(jsii_name="enableResourcePropertyConstraint")
+    def _enable_resource_property_constraint(self) -> builtins.bool:
+        return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
+
+    @_enable_resource_property_constraint.setter
+    def _enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__8821798621ada7c68595fc43f21586dc0f1f0020933d3d94f5bb363c0cd4a723)
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
+            type_hints = typing.get_type_hints(_typecheckingstub__53306e52b717825e64a230a11bc56cf6890d78b8d0c5cf3c0d6da52c6714c8d4)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "id", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="props")
+    def _props(self) -> "SchedulerRuleProps":
+        return typing.cast("SchedulerRuleProps", jsii.get(self, "props"))
+
+    @_props.setter
+    def _props(self, value: "SchedulerRuleProps") -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__fe01e31a1a5e3fcf131921951b3ef8582015836b8c8b5ed400cc94d3d2981cec)
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
+            type_hints = typing.get_type_hints(_typecheckingstub__ce314eaf5b495abf604989b4e3d94aef93f9ee422d84719178515948be8c2f4e)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "scope", value)
+
+
+@jsii.data_type(
+    jsii_type="@alicloud/ros-cdk-ddospro.SchedulerRuleProps",
+    jsii_struct_bases=[],
+    name_mapping={
+        "rule_name": "ruleName",
+        "rules": "rules",
+        "rule_type": "ruleType",
+        "param": "param",
+        "resource_group_id": "resourceGroupId",
+    },
+)
+class SchedulerRuleProps:
+    def __init__(
+        self,
+        *,
+        rule_name: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+        rules: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+        rule_type: typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable],
+        param: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+        resource_group_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    ) -> None:
+        '''Properties for defining a ``SchedulerRule``.
+
+        See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-ddospro-schedulerrule
+
+        :param rule_name: Property ruleName: The name of the rule.
+        :param rules: Property rules: The details of the scheduling rule. This parameter is a JSON string. The following list describes the fields in the value of the parameter: Type: the address type of the interaction resource that you want to use in the scheduling rule. This field is required and must be of the string type. Valid values: A: IP address. CNAME: domain name Value: the address of the interaction resource that you want to use in the scheduling rule. This field is required and must be of the string type. Priority: the priority of the scheduling rule. This field is required and must be of the integer type. Valid values: 0 to 100. A larger value indicates a higher priority. ValueType: the type of the interaction resource that you want to use in the scheduling rule. This field is required and must be of the integer type. Valid values: 1: the IP address of the Anti-DDoS Pro or Anti-DDoS Premium instance. 2: the IP address of the interaction resource in the tiered protection scenario. 3: the IP address that is used to accelerate access in the network acceleration scenario. 5: the domain name that is configured in Alibaba Cloud CDN (CDN) in the CDN interaction scenario. 6 the IP address of the interaction resource in the cloud service interaction scenario RegionId: the region where the interaction resource is deployed. This parameter must be specified when ValueType is set to 2. The value must be of the string type.
+        :param rule_type: Property ruleType: The type of the custom defense rule. Valid values: 2: tiered protection 3: network acceleration 5: CDN interaction 6: cloud service interaction 8: secure acceleration
+        :param param: Property param: The details of the CDN interaction rule. This parameter is a JSON string. The following list describes the fields in the value of the parameter: ParamType: the type of the scheduling rule. This field is required and must be of the string type. Set the value to cdn. This indicates that you want to modify a CDN interaction rule. ParamData: the values of parameters that you want to modify for the CDN interaction rule. This field is required and must be of the map type. ParamData contains the following parameters: Domain: the accelerated domain in CDN. This parameter is required and must be of the string type; Cname: the CNAME that is assigned to the accelerated domain. This parameter is required and must be of the string type; AccessQps: the queries per second (QPS) threshold that is used to switch service traffic to Anti-DDoS Pro or Anti-DDoS Premium. This parameter is required and must be of the integer type; UpstreamQps: the QPS threshold that is used to switch service traffic to CDN. This parameter is optional and must be of the integer type.
+        :param resource_group_id: Property resourceGroupId: The ID of the resource group to which the instance belongs in Resource Management. This parameter is empty by default, which indicates that the instance belongs to the default resource group.
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__ae883677c2fecd1eb05796cf13851174931a00543295d96f8dd079adb632b060)
+            check_type(argname="argument rule_name", value=rule_name, expected_type=type_hints["rule_name"])
+            check_type(argname="argument rules", value=rules, expected_type=type_hints["rules"])
+            check_type(argname="argument rule_type", value=rule_type, expected_type=type_hints["rule_type"])
+            check_type(argname="argument param", value=param, expected_type=type_hints["param"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "rule_name": rule_name,
+            "rules": rules,
+            "rule_type": rule_type,
+        }
+        if param is not None:
+            self._values["param"] = param
+        if resource_group_id is not None:
+            self._values["resource_group_id"] = resource_group_id
+
+    @builtins.property
+    def rule_name(
+        self,
+    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''Property ruleName: The name of the rule.'''
+        result = self._values.get("rule_name")
+        assert result is not None, "Required property 'rule_name' is missing"
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+    @builtins.property
+    def rules(self) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''Property rules: The details of the scheduling rule.
+
+        This parameter is a JSON string. The following list describes the fields in the value of the parameter:
+        Type: the address type of the interaction resource that you want to use in the scheduling rule. This field is required and must be of the string type. Valid values: A: IP address. CNAME: domain name
+        Value: the address of the interaction resource that you want to use in the scheduling rule. This field is required and must be of the string type.
+        Priority: the priority of the scheduling rule. This field is required and must be of the integer type. Valid values: 0 to 100. A larger value indicates a higher priority.
+        ValueType: the type of the interaction resource that you want to use in the scheduling rule. This field is required and must be of the integer type. Valid values: 1: the IP address of the Anti-DDoS Pro or Anti-DDoS Premium instance. 2: the IP address of the interaction resource in the tiered protection scenario. 3: the IP address that is used to accelerate access in the network acceleration scenario. 5: the domain name that is configured in Alibaba Cloud CDN (CDN) in the CDN interaction scenario. 6 the IP address of the interaction resource in the cloud service interaction scenario
+        RegionId: the region where the interaction resource is deployed. This parameter must be specified when ValueType is set to 2. The value must be of the string type.
+        '''
+        result = self._values.get("rules")
+        assert result is not None, "Required property 'rules' is missing"
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+    @builtins.property
+    def rule_type(
+        self,
+    ) -> typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''Property ruleType: The type of the custom defense rule.
+
+        Valid values:
+        2: tiered protection
+        3: network acceleration
+        5: CDN interaction
+        6: cloud service interaction
+        8: secure acceleration
+        '''
+        result = self._values.get("rule_type")
+        assert result is not None, "Required property 'rule_type' is missing"
+        return typing.cast(typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+    @builtins.property
+    def param(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''Property param: The details of the CDN interaction rule.
+
+        This parameter is a JSON string. The following list describes the fields in the value of the parameter:
+        ParamType: the type of the scheduling rule. This field is required and must be of the string type. Set the value to cdn. This indicates that you want to modify a CDN interaction rule.
+        ParamData: the values of parameters that you want to modify for the CDN interaction rule. This field is required and must be of the map type. ParamData contains the following parameters: Domain: the accelerated domain in CDN. This parameter is required and must be of the string type; Cname: the CNAME that is assigned to the accelerated domain. This parameter is required and must be of the string type; AccessQps: the queries per second (QPS) threshold that is used to switch service traffic to Anti-DDoS Pro or Anti-DDoS Premium. This parameter is required and must be of the integer type; UpstreamQps: the QPS threshold that is used to switch service traffic to CDN. This parameter is optional and must be of the integer type.
+        '''
+        result = self._values.get("param")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+    @builtins.property
+    def resource_group_id(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+        '''Property resourceGroupId: The ID of the resource group to which the instance belongs in Resource Management.
+
+        This parameter is empty by default, which indicates that the instance belongs to the default resource group.
+        '''
+        result = self._values.get("resource_group_id")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "SchedulerRuleProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
 __all__ = [
+    "Port",
+    "PortProps",
     "PremiumInstance",
     "PremiumInstanceProps",
     "ProInstance",
     "ProInstanceProps",
+    "RosPort",
+    "RosPortProps",
     "RosPremiumInstance",
     "RosPremiumInstanceProps",
     "RosProInstance",
     "RosProInstanceProps",
+    "RosSceneDefensePolicy",
+    "RosSceneDefensePolicyProps",
+    "RosSchedulerRule",
+    "RosSchedulerRuleProps",
+    "SceneDefensePolicy",
+    "SceneDefensePolicyProps",
+    "SchedulerRule",
+    "SchedulerRuleProps",
 ]
 
 publication.publish()
 
+def _typecheckingstub__3f70c2d2847e542843c1d8d77eba744a3e024f669e64a97cb155f8d0117b18b4(
+    scope: _ros_cdk_core_7adfd82f.Construct,
+    id: builtins.str,
+    props: typing.Union[PortProps, typing.Dict[builtins.str, typing.Any]],
+    enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__91dafd6d09b28f08d954e82cb5ee3ab2ad6396a435e21ff614d5ddae910800f9(
+    value: builtins.bool,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__fd3de6e1292475f86d1433e5bace8055f5104f4debafb0df2ec34ed6247205b1(
+    value: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__b008bc42c33b5ec2fdba150358962f414f3a844172ffec5998c399db0633e642(
+    value: PortProps,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__e7d387b2cd84046a76a7a810c20eb19864438702fb9519c2fa42c6e021b8ea30(
+    value: _ros_cdk_core_7adfd82f.Construct,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__907744fc156a231aebd7307dad220a1be51c48da2aaf6d35ea3fee309e7ac498(
+    *,
+    frontend_protocol: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    instance_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    real_servers: typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Sequence[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]],
+    backend_port: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    frontend_port: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__5ca97bab53a387dbc815509b75afca7dd13ee8cd546d393eafe27c56326f51f8(
     scope: _ros_cdk_core_7adfd82f.Construct,
     id: builtins.str,
     props: typing.Optional[typing.Union[PremiumInstanceProps, typing.Dict[builtins.str, typing.Any]]] = None,
     enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
 ) -> None:
     """Type checking stubs"""
@@ -2179,14 +3720,76 @@
     service_bandwidth: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     service_partner: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     tags: typing.Optional[typing.Sequence[typing.Union[RosProInstance.TagsProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__95f58b3961978a678cb526ddf1d9e63dfcd302d754f72f3251108bdd9b6b181e(
+    scope: _ros_cdk_core_7adfd82f.Construct,
+    id: builtins.str,
+    props: typing.Union[RosPortProps, typing.Dict[builtins.str, typing.Any]],
+    enable_resource_property_constraint: builtins.bool,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__51bde9afd2129ec87892e5568da2293106c5beee25f324118999c46020c8d0e0(
+    props: typing.Mapping[builtins.str, typing.Any],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__773bc27b9fc469e411f4c2fbceeb3822e12c7ae3200c509f393048bfc0056e2d(
+    value: builtins.bool,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__3edc74c43574f6bd8385c61317ce5d1c99f9c6f9680fd0c1da8b3616650a9418(
+    value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__43db68d39f39808599075609b859dc00712761f0b1f3dd60d67a0e64fae1c1c8(
+    value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__df6314c4b38aeacd729ef9087c64142c497dc811abebab6883731142af835e24(
+    value: typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.List[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__8fc5ac86ed13c1a1e4d5ac4d75b9d084045b364d472e1f1e38c170ceb4b97f47(
+    value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__28884777e4811b3a408c94c5511c9d3864129a09951f6d2a62457bb8c01326a3(
+    value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__19e84d824c2563111a3e1265cecc3b8ecd6f9fda05fabe200ccc24cf5b32318c(
+    *,
+    frontend_protocol: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    instance_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    real_servers: typing.Union[_ros_cdk_core_7adfd82f.IResolvable, typing.Sequence[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]],
+    backend_port: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    frontend_port: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__a99e16ce9cfb5e0990d1e19a0ed74921a9a224b5d6f16b65a595dd882fa5dd0e(
     scope: _ros_cdk_core_7adfd82f.Construct,
     id: builtins.str,
     props: typing.Union[RosPremiumInstanceProps, typing.Dict[builtins.str, typing.Any]],
     enable_resource_property_constraint: builtins.bool,
 ) -> None:
     """Type checking stubs"""
@@ -2416,7 +4019,211 @@
     port_count: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     service_bandwidth: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     service_partner: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     tags: typing.Optional[typing.Sequence[typing.Union[RosProInstance.TagsProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
+
+def _typecheckingstub__c1756817e5470835ce70e52ce71e0da06d5355d242707ac9e4d6564830214744(
+    scope: _ros_cdk_core_7adfd82f.Construct,
+    id: builtins.str,
+    props: typing.Union[RosSceneDefensePolicyProps, typing.Dict[builtins.str, typing.Any]],
+    enable_resource_property_constraint: builtins.bool,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__10877624c40ac4a6d8f5d908aedb30d2485f56960436d4a89e03c824fb1a8513(
+    props: typing.Mapping[builtins.str, typing.Any],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__4c236ba3393f24baf7936c92334f84202c5c9c09244e4512a10d82ac69fe7a28(
+    value: builtins.bool,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__ed53a0d4517ba1ad2639e70b4635f37a23e5ba3786f97a10682265b17ba36fbc(
+    value: typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__6f3a028fcafc037007dafb6c106ce38356cd75ec29bec1a160e54afce2002107(
+    value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__3bdabd778dc2fef602ae352d5af634d61baceab6f10d50c2a9a409023933e147(
+    value: typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__dcd0b375d29eef514c53faafe927bb1e6c256f6d5eff7c0b9b5ce83f9ebf46b2(
+    value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__8625addc2cb7cc74e1f6bd8c069c274eb1750600d0c8a559cfc061638decc206(
+    *,
+    end_time: typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable],
+    name: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    start_time: typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable],
+    template: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__60d7d56fe23e71859342593f2659f2a0880b0a528284a704533719ab2a5a6afa(
+    scope: _ros_cdk_core_7adfd82f.Construct,
+    id: builtins.str,
+    props: typing.Union[RosSchedulerRuleProps, typing.Dict[builtins.str, typing.Any]],
+    enable_resource_property_constraint: builtins.bool,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__fdfe932b810ddbf2234a04107688f8d11c91cd79938f4ae4ee79ea7b834cc4f8(
+    props: typing.Mapping[builtins.str, typing.Any],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__2cf1ed8abb21815fb04fb23b6523c73e866acf5d94bb14e3f4fb6a8ea9a4f250(
+    value: builtins.bool,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__755af63a3d4d6f036f0cde3a666fafa09e3a80a1f25b8bba2ea988cb91ed0642(
+    value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__25833a1ebbfbdbba810d83857e97c86feeaa5c86b3ace4eaaec390a0837a4782(
+    value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__36bd17e92e34915d373b70c24b5d5818fcaf8a1610fb5855c922ba0aab7fb49a(
+    value: typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__269cef1b9a3ea9580b02bdd7b1882e5a5d0682a57d3958b4f249a8f3f7c09cd3(
+    value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__c8e87eed91d6d64e6f8e45ece62deed0fef32d1363b053c12156dc9002576459(
+    value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__06878d13277cfd5d033015d37e320f287798899ac9d4657b17c84326a57526f8(
+    *,
+    rule_name: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    rules: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    rule_type: typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable],
+    param: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    resource_group_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__93a34aee76f73af63930ed237104de4318437451980b4d2a33bfd0008789e36a(
+    scope: _ros_cdk_core_7adfd82f.Construct,
+    id: builtins.str,
+    props: typing.Union[SceneDefensePolicyProps, typing.Dict[builtins.str, typing.Any]],
+    enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__091bb1aa84ae6c132d1c5e7832ede437b03efeae2f62863c89f3d33fb528860c(
+    value: builtins.bool,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__a76d70f282f547d53e9b141d7047869bfd592d7ab08c961d780fac0c3778247e(
+    value: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__4db93203395771cc895257245c9c2daeddaf3e9c49acb76dca9041c837e12d41(
+    value: SceneDefensePolicyProps,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__2091551606d1fcc71ccec8dff5318e86b02d6a7777a18564bc5cd6d483d0b111(
+    value: _ros_cdk_core_7adfd82f.Construct,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__7893eeae669d9101b3de6e4f33d023b50eb9d26ea21f6a1dd5f49c57a7aca6f0(
+    *,
+    end_time: typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable],
+    name: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    start_time: typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable],
+    template: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__31f5d9eab941d81a2abcb3f5f715b90b5f0d85ecb4853c191e37ea6c870e3162(
+    scope: _ros_cdk_core_7adfd82f.Construct,
+    id: builtins.str,
+    props: typing.Union[SchedulerRuleProps, typing.Dict[builtins.str, typing.Any]],
+    enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__8821798621ada7c68595fc43f21586dc0f1f0020933d3d94f5bb363c0cd4a723(
+    value: builtins.bool,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__53306e52b717825e64a230a11bc56cf6890d78b8d0c5cf3c0d6da52c6714c8d4(
+    value: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__fe01e31a1a5e3fcf131921951b3ef8582015836b8c8b5ed400cc94d3d2981cec(
+    value: SchedulerRuleProps,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__ce314eaf5b495abf604989b4e3d94aef93f9ee422d84719178515948be8c2f4e(
+    value: _ros_cdk_core_7adfd82f.Construct,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__ae883677c2fecd1eb05796cf13851174931a00543295d96f8dd079adb632b060(
+    *,
+    rule_name: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    rules: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    rule_type: typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable],
+    param: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    resource_group_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
```

### Comparing `ros-cdk-ddospro-1.0.24/src/ros_cdk_ddospro.egg-info/PKG-INFO` & `ros-cdk-ddospro-1.0.25/src/ros_cdk_ddospro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-ddospro
-Version: 1.0.24
+Version: 1.0.25
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS DDOSPRO Construct Library
```

