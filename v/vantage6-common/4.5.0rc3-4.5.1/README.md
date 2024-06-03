# Comparing `tmp/vantage6-common-4.5.0rc3.tar.gz` & `tmp/vantage6-common-4.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-common-4.5.0rc3.tar", last modified: Wed May 22 15:04:56 2024, max compression
+gzip compressed data, was "vantage6-common-4.5.1.tar", last modified: Mon Jun  3 09:42:55 2024, max compression
```

## Comparing `vantage6-common-4.5.0rc3.tar` & `vantage6-common-4.5.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:56.885278 vantage6-common-4.5.0rc3/
--rw-r--r--   0 runner    (1001) docker     (127)     9691 2024-05-22 15:04:56.885278 vantage6-common-4.5.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 15:04:56.885278 vantage6-common-4.5.0rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:56.877278 vantage6-common-4.5.0rc3/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:56.881278 vantage6-common-4.5.0rc3/vantage6/common/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/vantage6/common/__build__
--rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/vantage6/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/vantage6/common/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:56.881278 vantage6-common-4.5.0rc3/vantage6/common/client/
--rw-r--r--   0 runner    (1001) docker     (127)    19098 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/vantage6/common/client/client_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/vantage6/common/client/deserialization.py
--rw-r--r--   0 runner    (1001) docker     (127)    12452 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/vantage6/common/client/node_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/vantage6/common/client/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/vantage6/common/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/vantage6/common/configuration_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    18258 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/vantage6/common/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:56.881278 vantage6-common-4.5.0rc3/vantage6/common/docker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/vantage6/common/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8446 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/vantage6/common/docker/addons.py
--rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/vantage6/common/docker/network_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    12308 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/vantage6/common/encryption.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/vantage6/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/vantage6/common/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/vantage6/common/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/vantage6/common/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/vantage6/common/task_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/vantage6/common/utest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:56.881278 vantage6-common-4.5.0rc3/vantage6_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9691 2024-05-22 15:04:56.000000 vantage6-common-4.5.0rc3/vantage6_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-22 15:04:56.000000 vantage6-common-4.5.0rc3/vantage6_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:04:56.000000 vantage6-common-4.5.0rc3/vantage6_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-22 15:04:56.000000 vantage6-common-4.5.0rc3/vantage6_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 15:04:56.000000 vantage6-common-4.5.0rc3/vantage6_common.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:42:55.033587 vantage6-common-4.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-06-03 09:42:55.033587 vantage6-common-4.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 09:42:55.033587 vantage6-common-4.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-06-03 09:42:43.000000 vantage6-common-4.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:42:55.029587 vantage6-common-4.5.1/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:42:55.029587 vantage6-common-4.5.1/vantage6/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 09:42:43.000000 vantage6-common-4.5.1/vantage6/common/__build__
+-rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-06-03 09:42:43.000000 vantage6-common-4.5.1/vantage6/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-06-03 09:42:43.000000 vantage6-common-4.5.1/vantage6/common/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:42:55.029587 vantage6-common-4.5.1/vantage6/common/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    19104 2024-06-03 09:42:43.000000 vantage6-common-4.5.1/vantage6/common/client/client_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-06-03 09:42:43.000000 vantage6-common-4.5.1/vantage6/common/client/deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12452 2024-06-03 09:42:43.000000 vantage6-common-4.5.1/vantage6/common/client/node_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-06-03 09:42:43.000000 vantage6-common-4.5.1/vantage6/common/client/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-06-03 09:42:43.000000 vantage6-common-4.5.1/vantage6/common/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-06-03 09:42:43.000000 vantage6-common-4.5.1/vantage6/common/configuration_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18258 2024-06-03 09:42:43.000000 vantage6-common-4.5.1/vantage6/common/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:42:55.033587 vantage6-common-4.5.1/vantage6/common/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:42:43.000000 vantage6-common-4.5.1/vantage6/common/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8446 2024-06-03 09:42:43.000000 vantage6-common-4.5.1/vantage6/common/docker/addons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-06-03 09:42:43.000000 vantage6-common-4.5.1/vantage6/common/docker/network_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12308 2024-06-03 09:42:43.000000 vantage6-common-4.5.1/vantage6/common/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-06-03 09:42:43.000000 vantage6-common-4.5.1/vantage6/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-06-03 09:42:43.000000 vantage6-common-4.5.1/vantage6/common/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-06-03 09:42:43.000000 vantage6-common-4.5.1/vantage6/common/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-06-03 09:42:43.000000 vantage6-common-4.5.1/vantage6/common/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-06-03 09:42:43.000000 vantage6-common-4.5.1/vantage6/common/task_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-06-03 09:42:43.000000 vantage6-common-4.5.1/vantage6/common/utest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:42:55.033587 vantage6-common-4.5.1/vantage6_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-06-03 09:42:54.000000 vantage6-common-4.5.1/vantage6_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-06-03 09:42:55.000000 vantage6-common-4.5.1/vantage6_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 09:42:54.000000 vantage6-common-4.5.1/vantage6_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-06-03 09:42:54.000000 vantage6-common-4.5.1/vantage6_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-03 09:42:54.000000 vantage6-common-4.5.1/vantage6_common.egg-info/top_level.txt
```

### Comparing `vantage6-common-4.5.0rc3/PKG-INFO` & `vantage6-common-4.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-common
-Version: 4.5.0rc3
+Version: 4.5.1
 Summary: Vantage6 common
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-common Version: 4.5.0rc3 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-common Version: 4.5.1 Summary: Vantage6
 common Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.10
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ************
                                _[[_vv_aa_nn_tt_aa_gg_ee_66_]] ************
       ******** AA PPrriivvaaccyy EEnnhhaanncciinngg TTeecchhnnoollooggyy ((PPEETT)) OOppeerraattiioonnss ppllaattffoorrmm ********
    ******** [[!![[RReelleeaassee]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
 rreelleeaassee..yymmll//bbaaddggee..ssvvgg))]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
```

### Comparing `vantage6-common-4.5.0rc3/setup.py` & `vantage6-common-4.5.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         "cryptography==42.0.4",
         "docker==6.1.2",
         "pyfiglet==0.8.post1",
         "PyJWT==2.6.0",
         "PyYAML==6.0.1",
         "python-dateutil==2.8.2",
         "qrcode==7.3.1",
-        "requests==2.31.0",
+        "requests==2.32.2",
         "schema==0.7.5",
     ],
     extras_require={
         "dev": [
             "black",
             "pre-commit",
         ]
```

### Comparing `vantage6-common-4.5.0rc3/vantage6/common/__init__.py` & `vantage6-common-4.5.1/vantage6/common/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 import typing
 import uuid
 
 from colorama import init, Fore, Style
 
 from vantage6.common.globals import APPNAME, STRING_ENCODING
 
+# make sure the version is available
+from vantage6.common._version import __version__  # noqa: F401
+
 
 # init colorstuff
 init()
 
 
 def logger_name(special__name__: str):
     """
```

### Comparing `vantage6-common-4.5.0rc3/vantage6/common/_version.py` & `vantage6-common-4.5.1/vantage6/common/_version.py`

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

### Comparing `vantage6-common-4.5.0rc3/vantage6/common/client/client_base.py` & `vantage6-common-4.5.1/vantage6/common/client/client_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -560,15 +560,15 @@
         Returns
         -------
         bool
             Whether the algorithm store is properly setup
         """
         if is_for_algorithm_store:
             try:
-                int(self.store.id)
+                int(self.store.store_id)
                 return True
             except AttributeError:
                 self.log.error(
                     "Algorithm store not set. Please set the algorithm store first with"
                     " `client.store.set()`."
                 )
                 return False
```

### Comparing `vantage6-common-4.5.0rc3/vantage6/common/client/node_client.py` & `vantage6-common-4.5.1/vantage6/common/client/node_client.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.5.0rc3/vantage6/common/client/utils.py` & `vantage6-common-4.5.1/vantage6/common/client/utils.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.5.0rc3/vantage6/common/colors.py` & `vantage6-common-4.5.1/vantage6/common/colors.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.5.0rc3/vantage6/common/configuration_manager.py` & `vantage6-common-4.5.1/vantage6/common/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.5.0rc3/vantage6/common/context.py` & `vantage6-common-4.5.1/vantage6/common/context.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.5.0rc3/vantage6/common/docker/addons.py` & `vantage6-common-4.5.1/vantage6/common/docker/addons.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.5.0rc3/vantage6/common/docker/network_manager.py` & `vantage6-common-4.5.1/vantage6/common/docker/network_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.5.0rc3/vantage6/common/encryption.py` & `vantage6-common-4.5.1/vantage6/common/encryption.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.5.0rc3/vantage6/common/globals.py` & `vantage6-common-4.5.1/vantage6/common/globals.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.5.0rc3/vantage6/common/log.py` & `vantage6-common-4.5.1/vantage6/common/log.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.5.0rc3/vantage6/common/serialization.py` & `vantage6-common-4.5.1/vantage6/common/serialization.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.5.0rc3/vantage6/common/task_status.py` & `vantage6-common-4.5.1/vantage6/common/task_status.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.5.0rc3/vantage6/common/utest.py` & `vantage6-common-4.5.1/vantage6/common/utest.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.5.0rc3/vantage6_common.egg-info/PKG-INFO` & `vantage6-common-4.5.1/vantage6_common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-common
-Version: 4.5.0rc3
+Version: 4.5.1
 Summary: Vantage6 common
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-common Version: 4.5.0rc3 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-common Version: 4.5.1 Summary: Vantage6
 common Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.10
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ************
                                _[[_vv_aa_nn_tt_aa_gg_ee_66_]] ************
       ******** AA PPrriivvaaccyy EEnnhhaanncciinngg TTeecchhnnoollooggyy ((PPEETT)) OOppeerraattiioonnss ppllaattffoorrmm ********
    ******** [[!![[RReelleeaassee]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
 rreelleeaassee..yymmll//bbaaddggee..ssvvgg))]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
```

### Comparing `vantage6-common-4.5.0rc3/vantage6_common.egg-info/SOURCES.txt` & `vantage6-common-4.5.1/vantage6_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

