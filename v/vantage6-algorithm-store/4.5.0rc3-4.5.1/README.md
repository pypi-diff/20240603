# Comparing `tmp/vantage6-algorithm-store-4.5.0rc3.tar.gz` & `tmp/vantage6-algorithm-store-4.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-algorithm-store-4.5.0rc3.tar", last modified: Wed May 22 15:05:00 2024, max compression
+gzip compressed data, was "vantage6-algorithm-store-4.5.1.tar", last modified: Mon Jun  3 09:42:58 2024, max compression
```

## Comparing `vantage6-algorithm-store-4.5.0rc3.tar` & `vantage6-algorithm-store-4.5.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:05:00.093293 vantage6-algorithm-store-4.5.0rc3/
--rw-r--r--   0 runner    (1001) docker     (127)     9709 2024-05-22 15:05:00.093293 vantage6-algorithm-store-4.5.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 15:05:00.097293 vantage6-algorithm-store-4.5.0rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:05:00.089293 vantage6-algorithm-store-4.5.0rc3/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:05:00.089293 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:05:00.089293 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/__build__
--rw-r--r--   0 runner    (1001) docker     (127)    13224 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/default_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:05:00.093293 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/argument.py
--rw-r--r--   0 runner    (1001) docker     (127)    13848 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:05:00.093293 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/common/
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/common/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/common/ui_visualization_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/database.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/developer_algorithm_association.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/review.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/role.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/role_rule_association.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/ui_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/vantage6_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     8951 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/permission.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:05:00.093293 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/resource/
--rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21490 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/resource/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/resource/role.py
--rw-r--r--   0 runner    (1001) docker     (127)     7809 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/resource/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:05:00.093293 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/resource/schema/
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/resource/schema/input_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/resource/schema/output_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    12971 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/resource/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     7064 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/resource/vantage6_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/resource/version.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:05:00.093293 vantage6-algorithm-store-4.5.0rc3/vantage6_algorithm_store.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9709 2024-05-22 15:05:00.000000 vantage6-algorithm-store-4.5.0rc3/vantage6_algorithm_store.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-22 15:05:00.000000 vantage6-algorithm-store-4.5.0rc3/vantage6_algorithm_store.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:05:00.000000 vantage6-algorithm-store-4.5.0rc3/vantage6_algorithm_store.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-22 15:05:00.000000 vantage6-algorithm-store-4.5.0rc3/vantage6_algorithm_store.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 15:05:00.000000 vantage6-algorithm-store-4.5.0rc3/vantage6_algorithm_store.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:42:58.125595 vantage6-algorithm-store-4.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     9706 2024-06-03 09:42:58.125595 vantage6-algorithm-store-4.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 09:42:58.125595 vantage6-algorithm-store-4.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-06-03 09:42:43.000000 vantage6-algorithm-store-4.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:42:58.117595 vantage6-algorithm-store-4.5.1/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:42:58.117595 vantage6-algorithm-store-4.5.1/vantage6/algorithm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:42:58.117595 vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 09:42:43.000000 vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/__build__
+-rw-r--r--   0 runner    (1001) docker     (127)    13276 2024-06-03 09:42:43.000000 vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-06-03 09:42:43.000000 vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-06-03 09:42:43.000000 vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-06-03 09:42:43.000000 vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/default_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-06-03 09:42:43.000000 vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:42:58.121595 vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-06-03 09:42:43.000000 vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-06-03 09:42:43.000000 vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/model/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-06-03 09:42:43.000000 vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/model/argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13848 2024-06-03 09:42:43.000000 vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/model/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:42:58.121595 vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/model/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-06-03 09:42:43.000000 vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/model/common/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-06-03 09:42:43.000000 vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/model/common/ui_visualization_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-06-03 09:42:43.000000 vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/model/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-06-03 09:42:43.000000 vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/model/developer_algorithm_association.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-06-03 09:42:43.000000 vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/model/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-06-03 09:42:43.000000 vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/model/permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-06-03 09:42:43.000000 vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/model/review.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-06-03 09:42:43.000000 vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/model/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-06-03 09:42:43.000000 vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/model/role_rule_association.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-06-03 09:42:43.000000 vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/model/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-06-03 09:42:43.000000 vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/model/ui_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-06-03 09:42:43.000000 vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-06-03 09:42:43.000000 vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/model/vantage6_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8951 2024-06-03 09:42:43.000000 vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/permission.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:42:58.121595 vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-06-03 09:42:43.000000 vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21490 2024-06-03 09:42:43.000000 vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/resource/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-06-03 09:42:43.000000 vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/resource/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7809 2024-06-03 09:42:43.000000 vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/resource/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:42:58.121595 vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/resource/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-06-03 09:42:43.000000 vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/resource/schema/input_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-06-03 09:42:43.000000 vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/resource/schema/output_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12971 2024-06-03 09:42:43.000000 vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/resource/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7064 2024-06-03 09:42:43.000000 vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/resource/vantage6_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-06-03 09:42:43.000000 vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/resource/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-06-03 09:42:43.000000 vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:42:58.121595 vantage6-algorithm-store-4.5.1/vantage6_algorithm_store.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9706 2024-06-03 09:42:58.000000 vantage6-algorithm-store-4.5.1/vantage6_algorithm_store.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-06-03 09:42:58.000000 vantage6-algorithm-store-4.5.1/vantage6_algorithm_store.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 09:42:58.000000 vantage6-algorithm-store-4.5.1/vantage6_algorithm_store.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-06-03 09:42:58.000000 vantage6-algorithm-store-4.5.1/vantage6_algorithm_store.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-03 09:42:58.000000 vantage6-algorithm-store-4.5.1/vantage6_algorithm_store.egg-info/top_level.txt
```

### Comparing `vantage6-algorithm-store-4.5.0rc3/PKG-INFO` & `vantage6-algorithm-store-4.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-algorithm-store
-Version: 4.5.0rc3
+Version: 4.5.1
 Summary: Vantage6 algorithm store
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-algorithm-store Version: 4.5.0rc3 Summary:
+Metadata-Version: 2.1 Name: vantage6-algorithm-store Version: 4.5.1 Summary:
 Vantage6 algorithm store Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.10 Description-Content-Type: text/markdown Provides-Extra:
 dev
                                     ************
                                _[[_vv_aa_nn_tt_aa_gg_ee_66_]] ************
       ******** AA PPrriivvaaccyy EEnnhhaanncciinngg TTeecchhnnoollooggyy ((PPEETT)) OOppeerraattiioonnss ppllaattffoorrmm ********
    ******** [[!![[RReelleeaassee]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
```

### Comparing `vantage6-algorithm-store-4.5.0rc3/setup.py` & `vantage6-algorithm-store-4.5.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         "Flask-Cors==4.0.1",
         "Flask-Principal==0.4.0",
         "flask-marshmallow==0.15.0",
         "Flask-RESTful==0.3.10",
         "gevent==23.9.1",
         "jsonschema==4.21.1",
         "marshmallow==3.19.0",
-        "requests==2.31.0",
+        "requests==2.32.2",
         "schema==0.7.5",
         "SQLAlchemy==1.4.46",
         "werkzeug==3.0.3",
         f'vantage6 == {version_ns["__version__"]}',
         f'vantage6-common == {version_ns["__version__"]}',
     ],
     extras_require={"dev": ["coverage==6.4.4"]},
```

### Comparing `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/__init__.py` & `vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,25 +36,27 @@
 from vantage6.common import logger_name
 from vantage6.common.globals import APPNAME
 from vantage6.backend.common.resource.output_schema import BaseHATEOASModelSchema
 from vantage6.backend.common.globals import HOST_URI_ENV
 
 # TODO move this to common, then remove dependency on CLI in algorithm store
 from vantage6.cli.context.algorithm_store import AlgorithmStoreContext
-from vantage6.algorithm.store._version import __version__
 from vantage6.algorithm.store.globals import API_PATH
 from vantage6.algorithm.store.globals import RESOURCES, SERVER_MODULE_NAME
 
 # TODO the following are simply copies of the same files in the server - refactor
 from vantage6.algorithm.store.model.base import Base, DatabaseSessionManager, Database
 from vantage6.algorithm.store import db
 
 # TODO move server imports to common / refactor
 from vantage6.algorithm.store.permission import PermissionManager
 
+# make sure the version is available
+from vantage6.algorithm.store._version import __version__  # noqa: F401
+
 module_name = logger_name(__name__)
 log = logging.getLogger(module_name)
 
 
 class AlgorithmStoreApp:
     """
     Vantage6 server instance.
```

### Comparing `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/_version.py` & `vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/_version.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, "__build__")) as fp:
     __build__ = json.load(fp)
 
 # Module version
-version_info = (4, 5, 0, "candidate", __build__, 0)
+version_info = (4, 5, 1, "final", __build__, 0)
 
 # Module version stage suffix map
 _specifier_ = {"alpha": "a", "beta": "b", "candidate": "rc", "final": ""}
 version = f"{version_info[0]}.{version_info[1]}.{version_info[2]}"
 pre_release = (
     ""
     if version_info[3] == "final"
```

### Comparing `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/db.py` & `vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/db.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/default_roles.py` & `vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/default_roles.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/globals.py` & `vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/globals.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/__init__.py` & `vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/model/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/algorithm.py` & `vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/model/algorithm.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/argument.py` & `vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/model/argument.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/base.py` & `vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/model/base.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/common/enums.py` & `vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/model/common/enums.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/common/ui_visualization_schemas.py` & `vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/model/common/ui_visualization_schemas.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/database.py` & `vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/model/database.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/function.py` & `vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/model/function.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/permission.py` & `vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/model/permission.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/review.py` & `vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/model/review.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/role.py` & `vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/model/role.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/role_rule_association.py` & `vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/model/role_rule_association.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/rule.py` & `vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/model/rule.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/ui_visualization.py` & `vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/model/ui_visualization.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/user.py` & `vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/model/user.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/vantage6_server.py` & `vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/model/vantage6_server.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/permission.py` & `vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/permission.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/resource/__init__.py` & `vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/resource/algorithm.py` & `vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/resource/algorithm.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/resource/role.py` & `vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/resource/role.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/resource/rule.py` & `vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/resource/rule.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/resource/schema/input_schema.py` & `vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/resource/schema/input_schema.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/resource/schema/output_schema.py` & `vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/resource/schema/output_schema.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/resource/user.py` & `vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/resource/user.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/resource/vantage6_server.py` & `vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/resource/vantage6_server.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/resource/version.py` & `vantage6-algorithm-store-4.5.1/vantage6/algorithm/store/resource/version.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.5.0rc3/vantage6_algorithm_store.egg-info/PKG-INFO` & `vantage6-algorithm-store-4.5.1/vantage6_algorithm_store.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-algorithm-store
-Version: 4.5.0rc3
+Version: 4.5.1
 Summary: Vantage6 algorithm store
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-algorithm-store Version: 4.5.0rc3 Summary:
+Metadata-Version: 2.1 Name: vantage6-algorithm-store Version: 4.5.1 Summary:
 Vantage6 algorithm store Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.10 Description-Content-Type: text/markdown Provides-Extra:
 dev
                                     ************
                                _[[_vv_aa_nn_tt_aa_gg_ee_66_]] ************
       ******** AA PPrriivvaaccyy EEnnhhaanncciinngg TTeecchhnnoollooggyy ((PPEETT)) OOppeerraattiioonnss ppllaattffoorrmm ********
    ******** [[!![[RReelleeaassee]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
```

### Comparing `vantage6-algorithm-store-4.5.0rc3/vantage6_algorithm_store.egg-info/SOURCES.txt` & `vantage6-algorithm-store-4.5.1/vantage6_algorithm_store.egg-info/SOURCES.txt`

 * *Files identical despite different names*

