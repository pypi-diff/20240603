# Comparing `tmp/spaceone-dashboard-2.0.dev8.tar.gz` & `tmp/spaceone-dashboard-2.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spaceone-dashboard-2.0.dev8.tar", last modified: Wed Dec 20 08:01:06 2023, max compression
+gzip compressed data, was "spaceone-dashboard-2.0.dev9.tar", last modified: Wed Dec 20 08:10:29 2023, max compression
```

## Comparing `spaceone-dashboard-2.0.dev8.tar` & `spaceone-dashboard-2.0.dev9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 08:01:06.919552 spaceone-dashboard-2.0.dev8/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2023-12-20 08:01:06.919552 spaceone-dashboard-2.0.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-20 08:01:06.919552 spaceone-dashboard-2.0.dev8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2023-12-20 08:00:57.000000 spaceone-dashboard-2.0.dev8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 08:01:06.915552 spaceone-dashboard-2.0.dev8/spaceone/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-12-20 08:00:57.000000 spaceone-dashboard-2.0.dev8/spaceone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 08:01:06.915552 spaceone-dashboard-2.0.dev8/spaceone/dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 08:00:57.000000 spaceone-dashboard-2.0.dev8/spaceone/dashboard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 08:01:06.915552 spaceone-dashboard-2.0.dev8/spaceone/dashboard/conf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 08:00:57.000000 spaceone-dashboard-2.0.dev8/spaceone/dashboard/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2023-12-20 08:00:57.000000 spaceone-dashboard-2.0.dev8/spaceone/dashboard/conf/global_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 08:01:06.915552 spaceone-dashboard-2.0.dev8/spaceone/dashboard/connector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 08:00:57.000000 spaceone-dashboard-2.0.dev8/spaceone/dashboard/connector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 08:01:06.915552 spaceone-dashboard-2.0.dev8/spaceone/dashboard/error/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-12-20 08:00:57.000000 spaceone-dashboard-2.0.dev8/spaceone/dashboard/error/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2023-12-20 08:00:57.000000 spaceone-dashboard-2.0.dev8/spaceone/dashboard/error/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 08:01:06.915552 spaceone-dashboard-2.0.dev8/spaceone/dashboard/info/
--rw-r--r--   0 runner    (1001) docker     (127)      308 2023-12-20 08:00:57.000000 spaceone-dashboard-2.0.dev8/spaceone/dashboard/info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2023-12-20 08:00:57.000000 spaceone-dashboard-2.0.dev8/spaceone/dashboard/info/common_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2023-12-20 08:00:57.000000 spaceone-dashboard-2.0.dev8/spaceone/dashboard/info/private_dashboard_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2023-12-20 08:00:57.000000 spaceone-dashboard-2.0.dev8/spaceone/dashboard/info/private_dashboard_version_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2023-12-20 08:00:57.000000 spaceone-dashboard-2.0.dev8/spaceone/dashboard/info/public_dashboard_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2023-12-20 08:00:57.000000 spaceone-dashboard-2.0.dev8/spaceone/dashboard/info/public_dashboard_version_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 08:01:06.915552 spaceone-dashboard-2.0.dev8/spaceone/dashboard/interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 08:00:57.000000 spaceone-dashboard-2.0.dev8/spaceone/dashboard/interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 08:01:06.919552 spaceone-dashboard-2.0.dev8/spaceone/dashboard/interface/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2023-12-20 08:00:57.000000 spaceone-dashboard-2.0.dev8/spaceone/dashboard/interface/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4340 2023-12-20 08:00:57.000000 spaceone-dashboard-2.0.dev8/spaceone/dashboard/interface/grpc/private_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     4310 2023-12-20 08:00:57.000000 spaceone-dashboard-2.0.dev8/spaceone/dashboard/interface/grpc/public_dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 08:01:06.919552 spaceone-dashboard-2.0.dev8/spaceone/dashboard/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 08:00:57.000000 spaceone-dashboard-2.0.dev8/spaceone/dashboard/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 08:01:06.919552 spaceone-dashboard-2.0.dev8/spaceone/dashboard/manager/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2023-12-20 08:00:57.000000 spaceone-dashboard-2.0.dev8/spaceone/dashboard/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2023-12-20 08:00:57.000000 spaceone-dashboard-2.0.dev8/spaceone/dashboard/manager/identity_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2023-12-20 08:00:57.000000 spaceone-dashboard-2.0.dev8/spaceone/dashboard/manager/private_dashboard_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2023-12-20 08:00:57.000000 spaceone-dashboard-2.0.dev8/spaceone/dashboard/manager/private_dashboard_version_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2023-12-20 08:00:57.000000 spaceone-dashboard-2.0.dev8/spaceone/dashboard/manager/public_dashboard_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2023-12-20 08:00:57.000000 spaceone-dashboard-2.0.dev8/spaceone/dashboard/manager/public_dashboard_version_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 08:01:06.919552 spaceone-dashboard-2.0.dev8/spaceone/dashboard/model/
--rw-r--r--   0 runner    (1001) docker     (127)      356 2023-12-20 08:00:57.000000 spaceone-dashboard-2.0.dev8/spaceone/dashboard/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2023-12-20 08:00:57.000000 spaceone-dashboard-2.0.dev8/spaceone/dashboard/model/private_dashboard_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2023-12-20 08:00:57.000000 spaceone-dashboard-2.0.dev8/spaceone/dashboard/model/private_dashboard_version_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2023-12-20 08:00:57.000000 spaceone-dashboard-2.0.dev8/spaceone/dashboard/model/public_dashboard_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2023-12-20 08:00:57.000000 spaceone-dashboard-2.0.dev8/spaceone/dashboard/model/public_dashboard_version_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 08:01:06.919552 spaceone-dashboard-2.0.dev8/spaceone/dashboard/service/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2023-12-20 08:00:57.000000 spaceone-dashboard-2.0.dev8/spaceone/dashboard/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15628 2023-12-20 08:00:57.000000 spaceone-dashboard-2.0.dev8/spaceone/dashboard/service/private_dashboard_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    16081 2023-12-20 08:00:57.000000 spaceone-dashboard-2.0.dev8/spaceone/dashboard/service/public_dashboard_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 08:01:06.919552 spaceone-dashboard-2.0.dev8/spaceone_dashboard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2023-12-20 08:01:06.000000 spaceone-dashboard-2.0.dev8/spaceone_dashboard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2023-12-20 08:01:06.000000 spaceone-dashboard-2.0.dev8/spaceone_dashboard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-20 08:01:06.000000 spaceone-dashboard-2.0.dev8/spaceone_dashboard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-20 08:01:06.000000 spaceone-dashboard-2.0.dev8/spaceone_dashboard.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-12-20 08:01:06.000000 spaceone-dashboard-2.0.dev8/spaceone_dashboard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-20 08:01:06.000000 spaceone-dashboard-2.0.dev8/spaceone_dashboard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 08:10:29.767278 spaceone-dashboard-2.0.dev9/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2023-12-20 08:10:29.767278 spaceone-dashboard-2.0.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-20 08:10:29.767278 spaceone-dashboard-2.0.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2023-12-20 08:10:21.000000 spaceone-dashboard-2.0.dev9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 08:10:29.763278 spaceone-dashboard-2.0.dev9/spaceone/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2023-12-20 08:10:21.000000 spaceone-dashboard-2.0.dev9/spaceone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 08:10:29.763278 spaceone-dashboard-2.0.dev9/spaceone/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 08:10:21.000000 spaceone-dashboard-2.0.dev9/spaceone/dashboard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 08:10:29.763278 spaceone-dashboard-2.0.dev9/spaceone/dashboard/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 08:10:21.000000 spaceone-dashboard-2.0.dev9/spaceone/dashboard/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2023-12-20 08:10:21.000000 spaceone-dashboard-2.0.dev9/spaceone/dashboard/conf/global_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 08:10:29.763278 spaceone-dashboard-2.0.dev9/spaceone/dashboard/connector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 08:10:21.000000 spaceone-dashboard-2.0.dev9/spaceone/dashboard/connector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 08:10:29.763278 spaceone-dashboard-2.0.dev9/spaceone/dashboard/error/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2023-12-20 08:10:21.000000 spaceone-dashboard-2.0.dev9/spaceone/dashboard/error/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2023-12-20 08:10:21.000000 spaceone-dashboard-2.0.dev9/spaceone/dashboard/error/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 08:10:29.763278 spaceone-dashboard-2.0.dev9/spaceone/dashboard/info/
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2023-12-20 08:10:21.000000 spaceone-dashboard-2.0.dev9/spaceone/dashboard/info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2023-12-20 08:10:21.000000 spaceone-dashboard-2.0.dev9/spaceone/dashboard/info/common_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2023-12-20 08:10:21.000000 spaceone-dashboard-2.0.dev9/spaceone/dashboard/info/private_dashboard_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2023-12-20 08:10:21.000000 spaceone-dashboard-2.0.dev9/spaceone/dashboard/info/private_dashboard_version_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2023-12-20 08:10:21.000000 spaceone-dashboard-2.0.dev9/spaceone/dashboard/info/public_dashboard_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2023-12-20 08:10:21.000000 spaceone-dashboard-2.0.dev9/spaceone/dashboard/info/public_dashboard_version_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 08:10:29.763278 spaceone-dashboard-2.0.dev9/spaceone/dashboard/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 08:10:21.000000 spaceone-dashboard-2.0.dev9/spaceone/dashboard/interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 08:10:29.763278 spaceone-dashboard-2.0.dev9/spaceone/dashboard/interface/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2023-12-20 08:10:21.000000 spaceone-dashboard-2.0.dev9/spaceone/dashboard/interface/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2023-12-20 08:10:21.000000 spaceone-dashboard-2.0.dev9/spaceone/dashboard/interface/grpc/private_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4310 2023-12-20 08:10:21.000000 spaceone-dashboard-2.0.dev9/spaceone/dashboard/interface/grpc/public_dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 08:10:29.763278 spaceone-dashboard-2.0.dev9/spaceone/dashboard/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 08:10:21.000000 spaceone-dashboard-2.0.dev9/spaceone/dashboard/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 08:10:29.767278 spaceone-dashboard-2.0.dev9/spaceone/dashboard/manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2023-12-20 08:10:21.000000 spaceone-dashboard-2.0.dev9/spaceone/dashboard/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2023-12-20 08:10:21.000000 spaceone-dashboard-2.0.dev9/spaceone/dashboard/manager/identity_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2023-12-20 08:10:21.000000 spaceone-dashboard-2.0.dev9/spaceone/dashboard/manager/private_dashboard_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2023-12-20 08:10:21.000000 spaceone-dashboard-2.0.dev9/spaceone/dashboard/manager/private_dashboard_version_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2023-12-20 08:10:21.000000 spaceone-dashboard-2.0.dev9/spaceone/dashboard/manager/public_dashboard_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2023-12-20 08:10:21.000000 spaceone-dashboard-2.0.dev9/spaceone/dashboard/manager/public_dashboard_version_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 08:10:29.767278 spaceone-dashboard-2.0.dev9/spaceone/dashboard/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2023-12-20 08:10:21.000000 spaceone-dashboard-2.0.dev9/spaceone/dashboard/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2023-12-20 08:10:21.000000 spaceone-dashboard-2.0.dev9/spaceone/dashboard/model/private_dashboard_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2023-12-20 08:10:21.000000 spaceone-dashboard-2.0.dev9/spaceone/dashboard/model/private_dashboard_version_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2023-12-20 08:10:21.000000 spaceone-dashboard-2.0.dev9/spaceone/dashboard/model/public_dashboard_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2023-12-20 08:10:21.000000 spaceone-dashboard-2.0.dev9/spaceone/dashboard/model/public_dashboard_version_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 08:10:29.767278 spaceone-dashboard-2.0.dev9/spaceone/dashboard/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2023-12-20 08:10:21.000000 spaceone-dashboard-2.0.dev9/spaceone/dashboard/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15628 2023-12-20 08:10:21.000000 spaceone-dashboard-2.0.dev9/spaceone/dashboard/service/private_dashboard_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16081 2023-12-20 08:10:21.000000 spaceone-dashboard-2.0.dev9/spaceone/dashboard/service/public_dashboard_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 08:10:29.767278 spaceone-dashboard-2.0.dev9/spaceone_dashboard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2023-12-20 08:10:29.000000 spaceone-dashboard-2.0.dev9/spaceone_dashboard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2023-12-20 08:10:29.000000 spaceone-dashboard-2.0.dev9/spaceone_dashboard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-20 08:10:29.000000 spaceone-dashboard-2.0.dev9/spaceone_dashboard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-20 08:10:29.000000 spaceone-dashboard-2.0.dev9/spaceone_dashboard.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2023-12-20 08:10:29.000000 spaceone-dashboard-2.0.dev9/spaceone_dashboard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-20 08:10:29.000000 spaceone-dashboard-2.0.dev9/spaceone_dashboard.egg-info/top_level.txt
```

### Comparing `spaceone-dashboard-2.0.dev8/setup.py` & `spaceone-dashboard-2.0.dev9/setup.py`

 * *Files identical despite different names*

### Comparing `spaceone-dashboard-2.0.dev8/spaceone/dashboard/conf/global_conf.py` & `spaceone-dashboard-2.0.dev9/spaceone/dashboard/conf/global_conf.py`

 * *Files identical despite different names*

### Comparing `spaceone-dashboard-2.0.dev8/spaceone/dashboard/info/private_dashboard_info.py` & `spaceone-dashboard-2.0.dev9/spaceone/dashboard/info/private_dashboard_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 def PrivateDashboardInfo(dashboard_vo: PrivateDashboard, minimal=False):
     info = {
         "private_dashboard_id": dashboard_vo.private_dashboard_id,
         "name": dashboard_vo.name,
         "version": dashboard_vo.version,
         "labels": change_list_value_type(dashboard_vo.labels),
         "user_id": dashboard_vo.user_id,
+        "workspace_id": dashboard_vo.workspace_id,
         "domain_id": dashboard_vo.domain_id,
     }
 
     if not minimal:
         info.update(
             {
                 "layouts": change_list_value_type(dashboard_vo.layouts)
```

### Comparing `spaceone-dashboard-2.0.dev8/spaceone/dashboard/info/private_dashboard_version_info.py` & `spaceone-dashboard-2.0.dev9/spaceone/dashboard/info/private_dashboard_version_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-dashboard-2.0.dev8/spaceone/dashboard/info/public_dashboard_info.py` & `spaceone-dashboard-2.0.dev9/spaceone/dashboard/info/public_dashboard_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-dashboard-2.0.dev8/spaceone/dashboard/info/public_dashboard_version_info.py` & `spaceone-dashboard-2.0.dev9/spaceone/dashboard/info/public_dashboard_version_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-dashboard-2.0.dev8/spaceone/dashboard/interface/grpc/private_dashboard.py` & `spaceone-dashboard-2.0.dev9/spaceone/dashboard/interface/grpc/private_dashboard.py`

 * *Files identical despite different names*

### Comparing `spaceone-dashboard-2.0.dev8/spaceone/dashboard/interface/grpc/public_dashboard.py` & `spaceone-dashboard-2.0.dev9/spaceone/dashboard/interface/grpc/public_dashboard.py`

 * *Files identical despite different names*

### Comparing `spaceone-dashboard-2.0.dev8/spaceone/dashboard/manager/identity_manager.py` & `spaceone-dashboard-2.0.dev9/spaceone/dashboard/manager/identity_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-dashboard-2.0.dev8/spaceone/dashboard/manager/private_dashboard_manager.py` & `spaceone-dashboard-2.0.dev9/spaceone/dashboard/manager/private_dashboard_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-dashboard-2.0.dev8/spaceone/dashboard/manager/private_dashboard_version_manager.py` & `spaceone-dashboard-2.0.dev9/spaceone/dashboard/manager/private_dashboard_version_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-dashboard-2.0.dev8/spaceone/dashboard/manager/public_dashboard_manager.py` & `spaceone-dashboard-2.0.dev9/spaceone/dashboard/manager/public_dashboard_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-dashboard-2.0.dev8/spaceone/dashboard/manager/public_dashboard_version_manager.py` & `spaceone-dashboard-2.0.dev9/spaceone/dashboard/manager/public_dashboard_version_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-dashboard-2.0.dev8/spaceone/dashboard/model/private_dashboard_model.py` & `spaceone-dashboard-2.0.dev9/spaceone/dashboard/model/private_dashboard_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     layouts = ListField(default=[])
     variables = DictField(default={})
     settings = DictField(default={})
     variables_schema = DictField(default={})
     labels = ListField(StringField())
     tags = DictField(default={})
     user_id = StringField(max_length=40)
+    workspace_id = StringField(max_length=40)
     domain_id = StringField(max_length=40)
     created_at = DateTimeField(auto_now_add=True)
     updated_at = DateTimeField(auto_now=True)
 
     meta = {
         "updatable_fields": [
             "name",
@@ -32,21 +33,23 @@
             "tags",
         ],
         "minimal_fields": [
             "private_dashboard_id",
             "name",
             "version",
             "user_id",
+            "workspace_id",
             "domain_id",
         ],
         "ordering": ["name"],
         "indexes": [
             "name",
             "labels",
             "user_id",
+            "workspace_id",
             "domain_id",
         ],
     }
 
     @classmethod
     def create(cls, data):
         dashboard_vos = cls.filter(name=data["name"], domain_id=data["domain_id"])
```

### Comparing `spaceone-dashboard-2.0.dev8/spaceone/dashboard/model/private_dashboard_version_model.py` & `spaceone-dashboard-2.0.dev9/spaceone/dashboard/model/private_dashboard_version_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-dashboard-2.0.dev8/spaceone/dashboard/model/public_dashboard_model.py` & `spaceone-dashboard-2.0.dev9/spaceone/dashboard/model/public_dashboard_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-dashboard-2.0.dev8/spaceone/dashboard/model/public_dashboard_version_model.py` & `spaceone-dashboard-2.0.dev9/spaceone/dashboard/model/public_dashboard_version_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-dashboard-2.0.dev8/spaceone/dashboard/service/private_dashboard_service.py` & `spaceone-dashboard-2.0.dev9/spaceone/dashboard/service/private_dashboard_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-dashboard-2.0.dev8/spaceone/dashboard/service/public_dashboard_service.py` & `spaceone-dashboard-2.0.dev9/spaceone/dashboard/service/public_dashboard_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-dashboard-2.0.dev8/spaceone_dashboard.egg-info/SOURCES.txt` & `spaceone-dashboard-2.0.dev9/spaceone_dashboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

