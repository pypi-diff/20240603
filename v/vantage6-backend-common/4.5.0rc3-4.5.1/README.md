# Comparing `tmp/vantage6-backend-common-4.5.0rc3.tar.gz` & `tmp/vantage6-backend-common-4.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-backend-common-4.5.0rc3.tar", last modified: Wed May 22 15:04:59 2024, max compression
+gzip compressed data, was "vantage6-backend-common-4.5.1.tar", last modified: Mon Jun  3 09:42:57 2024, max compression
```

## Comparing `vantage6-backend-common-4.5.0rc3.tar` & `vantage6-backend-common-4.5.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:59.137293 vantage6-backend-common-4.5.0rc3/
--rw-r--r--   0 runner    (1001) docker     (127)     9723 2024-05-22 15:04:59.137293 vantage6-backend-common-4.5.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 15:04:59.137293 vantage6-backend-common-4.5.0rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-22 15:04:46.000000 vantage6-backend-common-4.5.0rc3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:59.137293 vantage6-backend-common-4.5.0rc3/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:59.137293 vantage6-backend-common-4.5.0rc3/vantage6/backend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:59.137293 vantage6-backend-common-4.5.0rc3/vantage6/backend/common/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:04:46.000000 vantage6-backend-common-4.5.0rc3/vantage6/backend/common/__build__
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-22 15:04:46.000000 vantage6-backend-common-4.5.0rc3/vantage6/backend/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-22 15:04:46.000000 vantage6-backend-common-4.5.0rc3/vantage6/backend/common/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-22 15:04:46.000000 vantage6-backend-common-4.5.0rc3/vantage6/backend/common/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:59.137293 vantage6-backend-common-4.5.0rc3/vantage6/backend/common/resource/
--rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-05-22 15:04:46.000000 vantage6-backend-common-4.5.0rc3/vantage6/backend/common/resource/output_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     9014 2024-05-22 15:04:46.000000 vantage6-backend-common-4.5.0rc3/vantage6/backend/common/resource/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-22 15:04:46.000000 vantage6-backend-common-4.5.0rc3/vantage6/backend/common/services_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-22 15:04:46.000000 vantage6-backend-common-4.5.0rc3/vantage6/backend/common/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:59.137293 vantage6-backend-common-4.5.0rc3/vantage6_backend_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9723 2024-05-22 15:04:59.000000 vantage6-backend-common-4.5.0rc3/vantage6_backend_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-22 15:04:59.000000 vantage6-backend-common-4.5.0rc3/vantage6_backend_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:04:59.000000 vantage6-backend-common-4.5.0rc3/vantage6_backend_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-22 15:04:59.000000 vantage6-backend-common-4.5.0rc3/vantage6_backend_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 15:04:59.000000 vantage6-backend-common-4.5.0rc3/vantage6_backend_common.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:42:57.225593 vantage6-backend-common-4.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     9720 2024-06-03 09:42:57.225593 vantage6-backend-common-4.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 09:42:57.225593 vantage6-backend-common-4.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-06-03 09:42:43.000000 vantage6-backend-common-4.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:42:57.221593 vantage6-backend-common-4.5.1/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:42:57.221593 vantage6-backend-common-4.5.1/vantage6/backend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:42:57.225593 vantage6-backend-common-4.5.1/vantage6/backend/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 09:42:43.000000 vantage6-backend-common-4.5.1/vantage6/backend/common/__build__
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-06-03 09:42:43.000000 vantage6-backend-common-4.5.1/vantage6/backend/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-06-03 09:42:43.000000 vantage6-backend-common-4.5.1/vantage6/backend/common/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-06-03 09:42:43.000000 vantage6-backend-common-4.5.1/vantage6/backend/common/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:42:57.225593 vantage6-backend-common-4.5.1/vantage6/backend/common/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-06-03 09:42:43.000000 vantage6-backend-common-4.5.1/vantage6/backend/common/resource/output_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9014 2024-06-03 09:42:43.000000 vantage6-backend-common-4.5.1/vantage6/backend/common/resource/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-06-03 09:42:43.000000 vantage6-backend-common-4.5.1/vantage6/backend/common/services_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-06-03 09:42:43.000000 vantage6-backend-common-4.5.1/vantage6/backend/common/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:42:57.225593 vantage6-backend-common-4.5.1/vantage6_backend_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9720 2024-06-03 09:42:57.000000 vantage6-backend-common-4.5.1/vantage6_backend_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-06-03 09:42:57.000000 vantage6-backend-common-4.5.1/vantage6_backend_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 09:42:57.000000 vantage6-backend-common-4.5.1/vantage6_backend_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-06-03 09:42:57.000000 vantage6-backend-common-4.5.1/vantage6_backend_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-03 09:42:57.000000 vantage6-backend-common-4.5.1/vantage6_backend_common.egg-info/top_level.txt
```

### Comparing `vantage6-backend-common-4.5.0rc3/PKG-INFO` & `vantage6-backend-common-4.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-backend-common
-Version: 4.5.0rc3
+Version: 4.5.1
 Summary: Vantage6 common backend functionalities
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-backend-common Version: 4.5.0rc3 Summary:
+Metadata-Version: 2.1 Name: vantage6-backend-common Version: 4.5.1 Summary:
 Vantage6 common backend functionalities Home-page: https://github.com/vantage6/
 vantage6 Requires-Python: >=3.10 Description-Content-Type: text/markdown
 Provides-Extra: dev
                                     ************
                                _[[_vv_aa_nn_tt_aa_gg_ee_66_]] ************
       ******** AA PPrriivvaaccyy EEnnhhaanncciinngg TTeecchhnnoollooggyy ((PPEETT)) OOppeerraattiioonnss ppllaattffoorrmm ********
    ******** [[!![[RReelleeaassee]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
```

### Comparing `vantage6-backend-common-4.5.0rc3/setup.py` & `vantage6-backend-common-4.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `vantage6-backend-common-4.5.0rc3/vantage6/backend/common/_version.py` & `vantage6-backend-common-4.5.1/vantage6/backend/common/_version.py`

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

### Comparing `vantage6-backend-common-4.5.0rc3/vantage6/backend/common/resource/output_schema.py` & `vantage6-backend-common-4.5.1/vantage6/backend/common/resource/output_schema.py`

 * *Files identical despite different names*

### Comparing `vantage6-backend-common-4.5.0rc3/vantage6/backend/common/resource/pagination.py` & `vantage6-backend-common-4.5.1/vantage6/backend/common/resource/pagination.py`

 * *Files identical despite different names*

### Comparing `vantage6-backend-common-4.5.0rc3/vantage6/backend/common/services_resources.py` & `vantage6-backend-common-4.5.1/vantage6/backend/common/services_resources.py`

 * *Files identical despite different names*

### Comparing `vantage6-backend-common-4.5.0rc3/vantage6_backend_common.egg-info/PKG-INFO` & `vantage6-backend-common-4.5.1/vantage6_backend_common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-backend-common
-Version: 4.5.0rc3
+Version: 4.5.1
 Summary: Vantage6 common backend functionalities
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-backend-common Version: 4.5.0rc3 Summary:
+Metadata-Version: 2.1 Name: vantage6-backend-common Version: 4.5.1 Summary:
 Vantage6 common backend functionalities Home-page: https://github.com/vantage6/
 vantage6 Requires-Python: >=3.10 Description-Content-Type: text/markdown
 Provides-Extra: dev
                                     ************
                                _[[_vv_aa_nn_tt_aa_gg_ee_66_]] ************
       ******** AA PPrriivvaaccyy EEnnhhaanncciinngg TTeecchhnnoollooggyy ((PPEETT)) OOppeerraattiioonnss ppllaattffoorrmm ********
    ******** [[!![[RReelleeaassee]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
```

### Comparing `vantage6-backend-common-4.5.0rc3/vantage6_backend_common.egg-info/SOURCES.txt` & `vantage6-backend-common-4.5.1/vantage6_backend_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

