# Comparing `tmp/ros-cdk-dms-1.0.8.tar.gz` & `tmp/ros-cdk-dms-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-dms-1.0.8.tar", last modified: Thu Jul 14 02:17:33 2022, max compression
+gzip compressed data, was "dist/ros-cdk-dms-1.0.9.tar", last modified: Fri Sep 23 10:48:35 2022, max compression
```

## Comparing `ros-cdk-dms-1.0.8.tar` & `ros-cdk-dms-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:17:33.000000 ros-cdk-dms-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:17:32.000000 ros-cdk-dms-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:17:32.000000 ros-cdk-dms-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:17:32.000000 ros-cdk-dms-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:17:33.000000 ros-cdk-dms-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      179 2022-07-14 02:17:32.000000 ros-cdk-dms-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:17:32.000000 ros-cdk-dms-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:17:33.000000 ros-cdk-dms-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1794 2022-07-14 02:17:32.000000 ros-cdk-dms-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:17:33.000000 ros-cdk-dms-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:17:33.000000 ros-cdk-dms-1.0.8/src/ros_cdk_dms/
--rw-r--r--   0 root         (0) root         (0)    73596 2022-07-14 02:17:32.000000 ros-cdk-dms-1.0.8/src/ros_cdk_dms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:17:33.000000 ros-cdk-dms-1.0.8/src/ros_cdk_dms/_jsii/
--rw-r--r--   0 root         (0) root         (0)      370 2022-07-14 02:17:32.000000 ros-cdk-dms-1.0.8/src/ros_cdk_dms/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45154 2022-07-14 02:17:32.000000 ros-cdk-dms-1.0.8/src/ros_cdk_dms/_jsii/ros-cdk-dms@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:17:32.000000 ros-cdk-dms-1.0.8/src/ros_cdk_dms/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:17:33.000000 ros-cdk-dms-1.0.8/src/ros_cdk_dms.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:17:32.000000 ros-cdk-dms-1.0.8/src/ros_cdk_dms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      400 2022-07-14 02:17:32.000000 ros-cdk-dms-1.0.8/src/ros_cdk_dms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:17:32.000000 ros-cdk-dms-1.0.8/src/ros_cdk_dms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:17:32.000000 ros-cdk-dms-1.0.8/src/ros_cdk_dms.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-07-14 02:17:32.000000 ros-cdk-dms-1.0.8/src/ros_cdk_dms.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:48:35.000000 ros-cdk-dms-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 10:48:35.000000 ros-cdk-dms-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 10:48:35.000000 ros-cdk-dms-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 10:48:35.000000 ros-cdk-dms-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 10:48:35.000000 ros-cdk-dms-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      179 2022-09-23 10:48:35.000000 ros-cdk-dms-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 10:48:35.000000 ros-cdk-dms-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 10:48:35.000000 ros-cdk-dms-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2022-09-23 10:48:35.000000 ros-cdk-dms-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:48:35.000000 ros-cdk-dms-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:48:35.000000 ros-cdk-dms-1.0.9/src/ros_cdk_dms/
+-rw-r--r--   0 root         (0) root         (0)    87607 2022-09-23 10:48:35.000000 ros-cdk-dms-1.0.9/src/ros_cdk_dms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:48:35.000000 ros-cdk-dms-1.0.9/src/ros_cdk_dms/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      404 2022-09-23 10:48:35.000000 ros-cdk-dms-1.0.9/src/ros_cdk_dms/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45221 2022-09-23 10:48:35.000000 ros-cdk-dms-1.0.9/src/ros_cdk_dms/_jsii/ros-cdk-dms@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 10:48:35.000000 ros-cdk-dms-1.0.9/src/ros_cdk_dms/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:48:35.000000 ros-cdk-dms-1.0.9/src/ros_cdk_dms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 10:48:35.000000 ros-cdk-dms-1.0.9/src/ros_cdk_dms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      400 2022-09-23 10:48:35.000000 ros-cdk-dms-1.0.9/src/ros_cdk_dms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 10:48:35.000000 ros-cdk-dms-1.0.9/src/ros_cdk_dms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 10:48:35.000000 ros-cdk-dms-1.0.9/src/ros_cdk_dms.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-09-23 10:48:35.000000 ros-cdk-dms-1.0.9/src/ros_cdk_dms.egg-info/top_level.txt
```

### Comparing `ros-cdk-dms-1.0.8/LICENSE` & `ros-cdk-dms-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-dms-1.0.8/PKG-INFO` & `ros-cdk-dms-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-dms
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS DMS Construct Library
```

### Comparing `ros-cdk-dms-1.0.8/setup.py` & `ros-cdk-dms-1.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-dms",
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
         "ros_cdk_dms",
         "ros_cdk_dms._jsii"
     ],
     "package_data": {
         "ros_cdk_dms._jsii": [
-            "ros-cdk-dms@1.0.8.jsii.tgz"
+            "ros-cdk-dms@1.0.9.jsii.tgz"
         ],
         "ros_cdk_dms": [
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

### Comparing `ros-cdk-dms-1.0.8/src/ros_cdk_dms/__init__.py` & `ros-cdk-dms-1.0.9/src/ros_cdk_dms/__init__.py`

 * *Files 20% similar despite different names*

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
 
 
 class Instance(
     ros_cdk_core.Resource,
@@ -29,43 +31,49 @@
 ):
     '''A ROS resource type:  ``ALIYUN::DMS::Instance``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "InstanceProps",
+        props: typing.Union["InstanceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::DMS::Instance``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Instance.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHost")
     def attr_host(self) -> ros_cdk_core.IResolvable:
         '''Attribute Host: The endpoint of the database instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHost"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceId: The ID of the database instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPort")
     def attr_port(self) -> ros_cdk_core.IResolvable:
         '''Attribute Port: The connection port of the database instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPort"))
 
 
 @jsii.data_type(
@@ -141,14 +149,37 @@
         :param ddl_online: Property ddlOnline: [Important] Specifies whether to enable the online data description language (DDL) service. Currently, this service is available only for the MySQL and PolarDB databases. 0: The service is disabled. 1: The native online DDL service prevails. 2: Data change without table locking provided by DMS prevails.
         :param ecs_instance_id: Property ecsInstanceId: The ID of the ECS instance to which the database instance belongs. Note You must specify this parameter if the InstanceSource parameter is set to ECS_OWN.
         :param ecs_region: Property ecsRegion: The region where the database instance resides. Note You must specify this parameter if the InstanceSource parameter is set to ECS_OWN or VPC_IDC.
         :param sid: Property sid: The system ID (SID) of the database instance. Note You must specify this parameter if the InstanceType parameter is set to PostgreSQL or Oracle.
         :param use_dsql: Property useDsql: Specifies whether to enable cross-database query for the database instance. Valid values: 0: disabled 1: enabled
         :param vpc_id: Property vpcId: The ID of the VPC to which the database instance belongs. Note You must specify this parameter if the InstanceSource parameter is set to VPC_IDC.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(InstanceProps.__init__)
+            check_type(argname="argument database_password", value=database_password, expected_type=type_hints["database_password"])
+            check_type(argname="argument database_user", value=database_user, expected_type=type_hints["database_user"])
+            check_type(argname="argument dba_uid", value=dba_uid, expected_type=type_hints["dba_uid"])
+            check_type(argname="argument env_type", value=env_type, expected_type=type_hints["env_type"])
+            check_type(argname="argument export_timeout", value=export_timeout, expected_type=type_hints["export_timeout"])
+            check_type(argname="argument host", value=host, expected_type=type_hints["host"])
+            check_type(argname="argument instance_alias", value=instance_alias, expected_type=type_hints["instance_alias"])
+            check_type(argname="argument instance_source", value=instance_source, expected_type=type_hints["instance_source"])
+            check_type(argname="argument instance_type", value=instance_type, expected_type=type_hints["instance_type"])
+            check_type(argname="argument network_type", value=network_type, expected_type=type_hints["network_type"])
+            check_type(argname="argument port", value=port, expected_type=type_hints["port"])
+            check_type(argname="argument query_timeout", value=query_timeout, expected_type=type_hints["query_timeout"])
+            check_type(argname="argument safe_rule", value=safe_rule, expected_type=type_hints["safe_rule"])
+            check_type(argname="argument tid", value=tid, expected_type=type_hints["tid"])
+            check_type(argname="argument data_link_name", value=data_link_name, expected_type=type_hints["data_link_name"])
+            check_type(argname="argument ddl_online", value=ddl_online, expected_type=type_hints["ddl_online"])
+            check_type(argname="argument ecs_instance_id", value=ecs_instance_id, expected_type=type_hints["ecs_instance_id"])
+            check_type(argname="argument ecs_region", value=ecs_region, expected_type=type_hints["ecs_region"])
+            check_type(argname="argument sid", value=sid, expected_type=type_hints["sid"])
+            check_type(argname="argument use_dsql", value=use_dsql, expected_type=type_hints["use_dsql"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "database_password": database_password,
             "database_user": database_user,
             "dba_uid": dba_uid,
             "env_type": env_type,
             "export_timeout": export_timeout,
             "host": host,
@@ -424,102 +455,117 @@
 ):
     '''A ROS template type:  ``ALIYUN::DMS::Instance``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosInstanceProps",
+        props: typing.Union["RosInstanceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::DMS::Instance``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosInstance.__init__)
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
+            type_hints = typing.get_type_hints(RosInstance._render_properties)
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
     @jsii.member(jsii_name="attrHost")
     def attr_host(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Host: The endpoint of the database instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHost"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InstanceId: The ID of the database instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPort")
     def attr_port(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Port: The connection port of the database instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="databasePassword")
     def database_password(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: databasePassword: The logon password of the database instance.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "databasePassword"))
 
     @database_password.setter
     def database_password(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "database_password").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "databasePassword", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="databaseUser")
     def database_user(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: databaseUser: The logon username of the database instance.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "databaseUser"))
 
     @database_user.setter
     def database_user(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "database_user").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "databaseUser", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbaUid")
     def dba_uid(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         dbaUid: The Alibaba Cloud unique ID (UID) of the database administrator (DBA) of the database
         instance.
@@ -531,26 +577,32 @@
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "dbaUid"))
 
     @dba_uid.setter
     def dba_uid(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "dba_uid").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbaUid", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="envType")
     def env_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         envType: The type of the environment to which the database instance belongs. Valid values:
         product: the production environment.
@@ -559,44 +611,53 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "envType"))
 
     @env_type.setter
     def env_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "env_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "envType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="exportTimeout")
     def export_timeout(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: exportTimeout: The timeout period for exporting the database instance. Unit: seconds.
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "exportTimeout"))
 
     @export_timeout.setter
     def export_timeout(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "export_timeout").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "exportTimeout", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="host")
     def host(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: host: The endpoint of the database instance.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "host"))
 
     @host.setter
     def host(self, value: typing.Union[builtins.str, ros_cdk_core.IResolvable]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "host").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "host", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceAlias")
     def instance_alias(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         instanceAlias: The alias of the database instance. The alias helps you quickly find the required
         instance.
@@ -604,17 +665,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "instanceAlias"))
 
     @instance_alias.setter
     def instance_alias(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "instance_alias").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceAlias", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceSource")
     def instance_source(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         instanceSource: The source of the database instance. Valid values:
         PUBLIC_OWN: an on-premises database built on the public network.
@@ -626,32 +690,38 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "instanceSource"))
 
     @instance_source.setter
     def instance_source(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "instance_source").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceSource", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceType")
     def instance_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: instanceType: The type of the database instance. Valid values: MySQL, SQLServer, PostgreSQL, Oracle, DRDS, OceanBase, Mongo, Redis
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "instanceType"))
 
     @instance_type.setter
     def instance_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "instance_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="networkType")
     def network_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         networkType: The network type of the database instance. Valid values:
         CLASSIC
@@ -660,44 +730,53 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "networkType"))
 
     @network_type.setter
     def network_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "network_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "networkType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="port")
     def port(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: port: The connection port of the database instance.
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "port"))
 
     @port.setter
     def port(self, value: typing.Union[jsii.Number, ros_cdk_core.IResolvable]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "port").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "port", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="queryTimeout")
     def query_timeout(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: queryTimeout: The timeout period for querying the database instance. Unit: seconds.
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "queryTimeout"))
 
     @query_timeout.setter
     def query_timeout(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "query_timeout").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "queryTimeout", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="safeRule")
     def safe_rule(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         safeRule: The security rule of the database instance. Enter the name of the security rule for
         your enterprise.
@@ -708,17 +787,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "safeRule"))
 
     @safe_rule.setter
     def safe_rule(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "safe_rule").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "safeRule", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tid")
     def tid(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         tid: The ID of the tenant.
         Note To query the ID, log on to the DMS Enterprise console and choose System Management
@@ -727,34 +809,40 @@
         Instance Management or System Management > User Management. The ID of the tenant
         appears in the Service Specification section.
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "tid"))
 
     @tid.setter
     def tid(self, value: typing.Union[jsii.Number, ros_cdk_core.IResolvable]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "tid").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tid", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dataLinkName")
     def data_link_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: dataLinkName: The name of the data link for cross-database query.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "dataLinkName"))
 
     @data_link_name.setter
     def data_link_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "data_link_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dataLinkName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ddlOnline")
     def ddl_online(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -767,17 +855,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "ddlOnline"))
 
     @ddl_online.setter
     def ddl_online(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "ddl_online").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ddlOnline", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ecsInstanceId")
     def ecs_instance_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -787,17 +878,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "ecsInstanceId"))
 
     @ecs_instance_id.setter
     def ecs_instance_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "ecs_instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ecsInstanceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ecsRegion")
     def ecs_region(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -807,17 +901,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "ecsRegion"))
 
     @ecs_region.setter
     def ecs_region(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "ecs_region").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ecsRegion", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="sid")
     def sid(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -827,17 +924,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "sid"))
 
     @sid.setter
     def sid(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "sid").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "sid", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="useDsql")
     def use_dsql(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -849,17 +949,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "useDsql"))
 
     @use_dsql.setter
     def use_dsql(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "use_dsql").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "useDsql", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpcId")
     def vpc_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -869,14 +972,17 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "vpcId"))
 
     @vpc_id.setter
     def vpc_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "vpc_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-dms.RosInstanceProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -949,14 +1055,37 @@
         :param ddl_online: 
         :param ecs_instance_id: 
         :param ecs_region: 
         :param sid: 
         :param use_dsql: 
         :param vpc_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosInstanceProps.__init__)
+            check_type(argname="argument database_password", value=database_password, expected_type=type_hints["database_password"])
+            check_type(argname="argument database_user", value=database_user, expected_type=type_hints["database_user"])
+            check_type(argname="argument dba_uid", value=dba_uid, expected_type=type_hints["dba_uid"])
+            check_type(argname="argument env_type", value=env_type, expected_type=type_hints["env_type"])
+            check_type(argname="argument export_timeout", value=export_timeout, expected_type=type_hints["export_timeout"])
+            check_type(argname="argument host", value=host, expected_type=type_hints["host"])
+            check_type(argname="argument instance_alias", value=instance_alias, expected_type=type_hints["instance_alias"])
+            check_type(argname="argument instance_source", value=instance_source, expected_type=type_hints["instance_source"])
+            check_type(argname="argument instance_type", value=instance_type, expected_type=type_hints["instance_type"])
+            check_type(argname="argument network_type", value=network_type, expected_type=type_hints["network_type"])
+            check_type(argname="argument port", value=port, expected_type=type_hints["port"])
+            check_type(argname="argument query_timeout", value=query_timeout, expected_type=type_hints["query_timeout"])
+            check_type(argname="argument safe_rule", value=safe_rule, expected_type=type_hints["safe_rule"])
+            check_type(argname="argument tid", value=tid, expected_type=type_hints["tid"])
+            check_type(argname="argument data_link_name", value=data_link_name, expected_type=type_hints["data_link_name"])
+            check_type(argname="argument ddl_online", value=ddl_online, expected_type=type_hints["ddl_online"])
+            check_type(argname="argument ecs_instance_id", value=ecs_instance_id, expected_type=type_hints["ecs_instance_id"])
+            check_type(argname="argument ecs_region", value=ecs_region, expected_type=type_hints["ecs_region"])
+            check_type(argname="argument sid", value=sid, expected_type=type_hints["sid"])
+            check_type(argname="argument use_dsql", value=use_dsql, expected_type=type_hints["use_dsql"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "database_password": database_password,
             "database_user": database_user,
             "dba_uid": dba_uid,
             "env_type": env_type,
             "export_timeout": export_timeout,
             "host": host,
@@ -1260,207 +1389,237 @@
 ):
     '''A ROS template type:  ``ALIYUN::DMS::User``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosUserProps",
+        props: typing.Union["RosUserProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::DMS::User``.
 
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
     @jsii.member(jsii_name="attrMobile")
     def attr_mobile(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Mobile: UserMobile
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMobile"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrParentUid")
     def attr_parent_uid(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ParentUid: ParentAliYunUid
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrParentUid"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRoleIds")
     def attr_role_ids(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: RoleIds: UserRoleId
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRoleIds"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRoleNames")
     def attr_role_names(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: RoleNames: UserRole
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRoleNames"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrUid")
     def attr_uid(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Uid: UserAliYunUid
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrUid"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrUserId")
     def attr_user_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: UserId: UserId
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrUserId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrUserName")
     def attr_user_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: UserName: UserNickName
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
     @jsii.member(jsii_name="uid")
     def uid(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: uid: UserAliYunUid
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "uid"))
 
     @uid.setter
     def uid(self, value: typing.Union[builtins.str, ros_cdk_core.IResolvable]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosUser, "uid").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "uid", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="mobile")
     def mobile(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: mobile: UserMobile
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "mobile"))
 
     @mobile.setter
     def mobile(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosUser, "mobile").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "mobile", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="roleNames")
     def role_names(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property: roleNames: UserRole
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "roleNames"))
 
     @role_names.setter
     def role_names(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosUser, "role_names").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "roleNames", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="status")
     def status(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: status: UserStatus
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "status"))
 
     @status.setter
     def status(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosUser, "status").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "status", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tid")
     def tid(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: tid:
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "tid"))
 
     @tid.setter
     def tid(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosUser, "tid").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tid", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="userName")
     def user_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: userName: UserNickName
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "userName"))
 
     @user_name.setter
     def user_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosUser, "user_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "userName", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-dms.RosUserProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -1488,14 +1647,22 @@
         :param uid: 
         :param mobile: 
         :param role_names: 
         :param status: 
         :param tid: 
         :param user_name: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosUserProps.__init__)
+            check_type(argname="argument uid", value=uid, expected_type=type_hints["uid"])
+            check_type(argname="argument mobile", value=mobile, expected_type=type_hints["mobile"])
+            check_type(argname="argument role_names", value=role_names, expected_type=type_hints["role_names"])
+            check_type(argname="argument status", value=status, expected_type=type_hints["status"])
+            check_type(argname="argument tid", value=tid, expected_type=type_hints["tid"])
+            check_type(argname="argument user_name", value=user_name, expected_type=type_hints["user_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "uid": uid,
         }
         if mobile is not None:
             self._values["mobile"] = mobile
         if role_names is not None:
             self._values["role_names"] = role_names
@@ -1584,67 +1751,73 @@
 ):
     '''A ROS resource type:  ``ALIYUN::DMS::User``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "UserProps",
+        props: typing.Union["UserProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::DMS::User``.
 
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
     @jsii.member(jsii_name="attrMobile")
     def attr_mobile(self) -> ros_cdk_core.IResolvable:
         '''Attribute Mobile: UserMobile.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMobile"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrParentUid")
     def attr_parent_uid(self) -> ros_cdk_core.IResolvable:
         '''Attribute ParentUid: ParentAliYunUid.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrParentUid"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRoleIds")
     def attr_role_ids(self) -> ros_cdk_core.IResolvable:
         '''Attribute RoleIds: UserRoleId.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRoleIds"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRoleNames")
     def attr_role_names(self) -> ros_cdk_core.IResolvable:
         '''Attribute RoleNames: UserRole.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRoleNames"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrUid")
     def attr_uid(self) -> ros_cdk_core.IResolvable:
         '''Attribute Uid: UserAliYunUid.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrUid"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrUserId")
     def attr_user_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute UserId: UserId.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrUserId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrUserName")
     def attr_user_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute UserName: UserNickName.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrUserName"))
 
 
 @jsii.data_type(
@@ -1675,14 +1848,22 @@
         :param uid: Property uid: UserAliYunUid.
         :param mobile: Property mobile: UserMobile.
         :param role_names: Property roleNames: UserRole.
         :param status: Property status: UserStatus.
         :param tid: Property tid:.
         :param user_name: Property userName: UserNickName.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(UserProps.__init__)
+            check_type(argname="argument uid", value=uid, expected_type=type_hints["uid"])
+            check_type(argname="argument mobile", value=mobile, expected_type=type_hints["mobile"])
+            check_type(argname="argument role_names", value=role_names, expected_type=type_hints["role_names"])
+            check_type(argname="argument status", value=status, expected_type=type_hints["status"])
+            check_type(argname="argument tid", value=tid, expected_type=type_hints["tid"])
+            check_type(argname="argument user_name", value=user_name, expected_type=type_hints["user_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "uid": uid,
         }
         if mobile is not None:
             self._values["mobile"] = mobile
         if role_names is not None:
             self._values["role_names"] = role_names
```

### Comparing `ros-cdk-dms-1.0.8/src/ros_cdk_dms.egg-info/PKG-INFO` & `ros-cdk-dms-1.0.9/src/ros_cdk_dms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-dms
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS DMS Construct Library
```

