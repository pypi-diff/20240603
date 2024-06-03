# Comparing `tmp/pyguardpoint-1.4.1.tar.gz` & `tmp/pyguardpoint-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyguardpoint-1.4.1.tar", last modified: Fri May 31 11:49:44 2024, max compression
+gzip compressed data, was "pyguardpoint-1.4.2.tar", last modified: Mon Jun  3 14:21:12 2024, max compression
```

## Comparing `pyguardpoint-1.4.1.tar` & `pyguardpoint-1.4.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 johnowen   (501) staff       (20)        0 2024-05-31 11:49:44.119199 pyguardpoint-1.4.1/
--rw-r--r--   0 johnowen   (501) staff       (20)    11357 2024-03-13 09:54:42.000000 pyguardpoint-1.4.1/LICENSE.txt
--rw-r--r--   0 johnowen   (501) staff       (20)    10657 2024-05-31 11:49:44.118895 pyguardpoint-1.4.1/PKG-INFO
--rw-r--r--   0 johnowen   (501) staff       (20)    10243 2024-05-31 10:37:48.000000 pyguardpoint-1.4.1/README.rst
-drwxr-xr-x   0 johnowen   (501) staff       (20)        0 2024-05-31 11:49:44.114496 pyguardpoint-1.4.1/pyGuardPoint/
--rw-r--r--   0 johnowen   (501) staff       (20)     8613 2024-03-13 09:54:42.000000 pyguardpoint-1.4.1/pyGuardPoint/CustomWebsocketTransport.py
--rw-r--r--   0 johnowen   (501) staff       (20)      342 2024-03-13 09:54:42.000000 pyguardpoint-1.4.1/pyGuardPoint/__init__.py
--rw-r--r--   0 johnowen   (501) staff       (20)     2361 2024-05-30 09:25:35.000000 pyguardpoint-1.4.1/pyGuardPoint/_guardpoint_alarms.py
--rw-r--r--   0 johnowen   (501) staff       (20)     1442 2024-05-31 11:36:24.000000 pyguardpoint-1.4.1/pyGuardPoint/_guardpoint_areas.py
--rw-r--r--   0 johnowen   (501) staff       (20)    15645 2024-05-31 11:48:06.000000 pyguardpoint-1.4.1/pyGuardPoint/_guardpoint_cardholders.py
--rw-r--r--   0 johnowen   (501) staff       (20)     1340 2024-03-13 09:54:42.000000 pyguardpoint-1.4.1/pyGuardPoint/_guardpoint_cardholdertypes.py
--rw-r--r--   0 johnowen   (501) staff       (20)     7441 2024-05-31 11:48:06.000000 pyguardpoint-1.4.1/pyGuardPoint/_guardpoint_cards.py
--rw-r--r--   0 johnowen   (501) staff       (20)     2429 2024-03-13 09:54:42.000000 pyguardpoint-1.4.1/pyGuardPoint/_guardpoint_controllers.py
--rw-r--r--   0 johnowen   (501) staff       (20)     1302 2024-03-13 09:54:42.000000 pyguardpoint-1.4.1/pyGuardPoint/_guardpoint_customizedfields.py
--rw-r--r--   0 johnowen   (501) staff       (20)     1860 2024-03-13 09:54:42.000000 pyguardpoint-1.4.1/pyGuardPoint/_guardpoint_diagnostic.py
--rw-r--r--   0 johnowen   (501) staff       (20)     3016 2024-05-31 10:23:30.000000 pyguardpoint-1.4.1/pyGuardPoint/_guardpoint_events.py
--rw-r--r--   0 johnowen   (501) staff       (20)     3857 2024-03-13 09:54:42.000000 pyguardpoint-1.4.1/pyGuardPoint/_guardpoint_ouputs.py
--rw-r--r--   0 johnowen   (501) staff       (20)     1328 2024-03-13 09:54:42.000000 pyguardpoint-1.4.1/pyGuardPoint/_guardpoint_personaldetails.py
--rw-r--r--   0 johnowen   (501) staff       (20)     2292 2024-03-13 09:54:42.000000 pyguardpoint-1.4.1/pyGuardPoint/_guardpoint_readers.py
--rw-r--r--   0 johnowen   (501) staff       (20)     2763 2024-03-13 09:54:42.000000 pyguardpoint-1.4.1/pyGuardPoint/_guardpoint_scheduledmags.py
--rw-r--r--   0 johnowen   (501) staff       (20)     1524 2024-03-13 09:54:42.000000 pyguardpoint-1.4.1/pyGuardPoint/_guardpoint_securitygroups.py
--rw-r--r--   0 johnowen   (501) staff       (20)     5432 2024-03-13 09:54:42.000000 pyguardpoint-1.4.1/pyGuardPoint/_odata_filter.py
--rw-r--r--   0 johnowen   (501) staff       (20)     1566 2024-03-13 09:54:42.000000 pyguardpoint-1.4.1/pyGuardPoint/_str_match_algo.py
-drwxr-xr-x   0 johnowen   (501) staff       (20)        0 2024-05-31 11:49:44.118301 pyguardpoint-1.4.1/pyGuardPoint/gp_asyncio/
--rw-r--r--   0 johnowen   (501) staff       (20)        0 2024-03-13 09:54:42.000000 pyguardpoint-1.4.1/pyGuardPoint/gp_asyncio/__init__.py
--rw-r--r--   0 johnowen   (501) staff       (20)     2388 2024-05-30 09:17:55.000000 pyguardpoint-1.4.1/pyGuardPoint/gp_asyncio/_async_guardpoint_alarms.py
--rw-r--r--   0 johnowen   (501) staff       (20)     1266 2024-03-13 09:54:42.000000 pyguardpoint-1.4.1/pyGuardPoint/gp_asyncio/_async_guardpoint_areas.py
--rw-r--r--   0 johnowen   (501) staff       (20)    12951 2024-05-31 11:47:57.000000 pyguardpoint-1.4.1/pyGuardPoint/gp_asyncio/_async_guardpoint_cardholders.py
--rw-r--r--   0 johnowen   (501) staff       (20)     1355 2024-03-13 09:54:42.000000 pyguardpoint-1.4.1/pyGuardPoint/gp_asyncio/_async_guardpoint_cardholdertypes.py
--rw-r--r--   0 johnowen   (501) staff       (20)     6900 2024-03-13 09:54:42.000000 pyguardpoint-1.4.1/pyGuardPoint/gp_asyncio/_async_guardpoint_cards.py
--rw-r--r--   0 johnowen   (501) staff       (20)     2527 2024-03-13 09:54:42.000000 pyguardpoint-1.4.1/pyGuardPoint/gp_asyncio/_async_guardpoint_controllers.py
--rw-r--r--   0 johnowen   (501) staff       (20)     1317 2024-03-13 09:54:42.000000 pyguardpoint-1.4.1/pyGuardPoint/gp_asyncio/_async_guardpoint_customizedfields.py
--rw-r--r--   0 johnowen   (501) staff       (20)     1873 2024-03-13 09:54:42.000000 pyguardpoint-1.4.1/pyGuardPoint/gp_asyncio/_async_guardpoint_diagnostic.py
--rw-r--r--   0 johnowen   (501) staff       (20)     3043 2024-05-31 10:17:21.000000 pyguardpoint-1.4.1/pyGuardPoint/gp_asyncio/_async_guardpoint_events.py
--rw-r--r--   0 johnowen   (501) staff       (20)     3862 2024-03-13 09:54:42.000000 pyguardpoint-1.4.1/pyGuardPoint/gp_asyncio/_async_guardpoint_ouputs.py
--rw-r--r--   0 johnowen   (501) staff       (20)     1343 2024-03-13 09:54:42.000000 pyguardpoint-1.4.1/pyGuardPoint/gp_asyncio/_async_guardpoint_personaldetails.py
--rw-r--r--   0 johnowen   (501) staff       (20)     2317 2024-05-30 09:17:55.000000 pyguardpoint-1.4.1/pyGuardPoint/gp_asyncio/_async_guardpoint_readers.py
--rw-r--r--   0 johnowen   (501) staff       (20)     2763 2024-03-13 09:54:42.000000 pyguardpoint-1.4.1/pyGuardPoint/gp_asyncio/_async_guardpoint_scheduledmags.py
--rw-r--r--   0 johnowen   (501) staff       (20)     1524 2024-03-13 09:54:42.000000 pyguardpoint-1.4.1/pyGuardPoint/gp_asyncio/_async_guardpoint_securitygroups.py
--rw-r--r--   0 johnowen   (501) staff       (20)    12795 2024-05-28 14:49:38.000000 pyguardpoint-1.4.1/pyGuardPoint/gp_asyncio/guardpoint_connection_asyncio.py
--rw-r--r--   0 johnowen   (501) staff       (20)     5914 2024-05-31 11:36:24.000000 pyguardpoint-1.4.1/pyGuardPoint/guardpoint.py
--rw-r--r--   0 johnowen   (501) staff       (20)     9468 2024-05-31 11:27:33.000000 pyguardpoint-1.4.1/pyGuardPoint/guardpoint_asyncio.py
--rw-r--r--   0 johnowen   (501) staff       (20)    11292 2024-05-31 11:49:13.000000 pyguardpoint-1.4.1/pyGuardPoint/guardpoint_connection.py
--rw-r--r--   0 johnowen   (501) staff       (20)    33141 2024-05-31 11:36:24.000000 pyguardpoint-1.4.1/pyGuardPoint/guardpoint_dataclasses.py
--rw-r--r--   0 johnowen   (501) staff       (20)       97 2024-03-13 09:54:42.000000 pyguardpoint-1.4.1/pyGuardPoint/guardpoint_error.py
--rw-r--r--   0 johnowen   (501) staff       (20)     3982 2024-03-13 09:54:42.000000 pyguardpoint-1.4.1/pyGuardPoint/guardpoint_threaded.py
--rw-r--r--   0 johnowen   (501) staff       (20)     4245 2024-03-13 09:54:42.000000 pyguardpoint-1.4.1/pyGuardPoint/guardpoint_utils.py
-drwxr-xr-x   0 johnowen   (501) staff       (20)        0 2024-05-31 11:49:44.118673 pyguardpoint-1.4.1/pyGuardPoint.egg-info/
--rw-r--r--   0 johnowen   (501) staff       (20)    10657 2024-05-31 11:49:44.000000 pyguardpoint-1.4.1/pyGuardPoint.egg-info/PKG-INFO
--rw-r--r--   0 johnowen   (501) staff       (20)     2037 2024-05-31 11:49:44.000000 pyguardpoint-1.4.1/pyGuardPoint.egg-info/SOURCES.txt
--rw-r--r--   0 johnowen   (501) staff       (20)        1 2024-05-31 11:49:44.000000 pyguardpoint-1.4.1/pyGuardPoint.egg-info/dependency_links.txt
--rw-r--r--   0 johnowen   (501) staff       (20)        1 2024-05-28 15:02:25.000000 pyguardpoint-1.4.1/pyGuardPoint.egg-info/not-zip-safe
--rw-r--r--   0 johnowen   (501) staff       (20)       75 2024-05-31 11:49:44.000000 pyguardpoint-1.4.1/pyGuardPoint.egg-info/requires.txt
--rw-r--r--   0 johnowen   (501) staff       (20)       13 2024-05-31 11:49:44.000000 pyguardpoint-1.4.1/pyGuardPoint.egg-info/top_level.txt
--rw-r--r--   0 johnowen   (501) staff       (20)       38 2024-05-31 11:49:44.119235 pyguardpoint-1.4.1/setup.cfg
--rw-r--r--   0 johnowen   (501) staff       (20)      632 2024-05-31 11:49:13.000000 pyguardpoint-1.4.1/setup.py
+drwxr-xr-x   0 johnowen   (501) staff       (20)        0 2024-06-03 14:21:12.048440 pyguardpoint-1.4.2/
+-rw-r--r--   0 johnowen   (501) staff       (20)    11357 2024-03-13 09:54:42.000000 pyguardpoint-1.4.2/LICENSE.txt
+-rw-r--r--   0 johnowen   (501) staff       (20)    10657 2024-06-03 14:21:12.048220 pyguardpoint-1.4.2/PKG-INFO
+-rw-r--r--   0 johnowen   (501) staff       (20)    10243 2024-05-31 10:37:48.000000 pyguardpoint-1.4.2/README.rst
+drwxr-xr-x   0 johnowen   (501) staff       (20)        0 2024-06-03 14:21:12.043608 pyguardpoint-1.4.2/pyGuardPoint/
+-rw-r--r--   0 johnowen   (501) staff       (20)     8613 2024-03-13 09:54:42.000000 pyguardpoint-1.4.2/pyGuardPoint/CustomWebsocketTransport.py
+-rw-r--r--   0 johnowen   (501) staff       (20)      342 2024-03-13 09:54:42.000000 pyguardpoint-1.4.2/pyGuardPoint/__init__.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     2361 2024-05-30 09:25:35.000000 pyguardpoint-1.4.2/pyGuardPoint/_guardpoint_alarms.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     2033 2024-05-31 12:12:02.000000 pyguardpoint-1.4.2/pyGuardPoint/_guardpoint_areas.py
+-rw-r--r--   0 johnowen   (501) staff       (20)    19436 2024-05-31 12:12:02.000000 pyguardpoint-1.4.2/pyGuardPoint/_guardpoint_cardholders.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     1340 2024-03-13 09:54:42.000000 pyguardpoint-1.4.2/pyGuardPoint/_guardpoint_cardholdertypes.py
+-rw-r--r--   0 johnowen   (501) staff       (20)    12085 2024-05-31 12:12:02.000000 pyguardpoint-1.4.2/pyGuardPoint/_guardpoint_cards.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     2429 2024-03-13 09:54:42.000000 pyguardpoint-1.4.2/pyGuardPoint/_guardpoint_controllers.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     1302 2024-03-13 09:54:42.000000 pyguardpoint-1.4.2/pyGuardPoint/_guardpoint_customizedfields.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     1860 2024-03-13 09:54:42.000000 pyguardpoint-1.4.2/pyGuardPoint/_guardpoint_diagnostic.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     5238 2024-06-03 09:36:52.000000 pyguardpoint-1.4.2/pyGuardPoint/_guardpoint_events.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     3857 2024-03-13 09:54:42.000000 pyguardpoint-1.4.2/pyGuardPoint/_guardpoint_ouputs.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     2477 2024-05-31 12:12:02.000000 pyguardpoint-1.4.2/pyGuardPoint/_guardpoint_personaldetails.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     3957 2024-05-31 12:12:02.000000 pyguardpoint-1.4.2/pyGuardPoint/_guardpoint_readers.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     2763 2024-03-13 09:54:42.000000 pyguardpoint-1.4.2/pyGuardPoint/_guardpoint_scheduledmags.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     2475 2024-05-31 12:12:02.000000 pyguardpoint-1.4.2/pyGuardPoint/_guardpoint_securitygroups.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     5432 2024-03-13 09:54:42.000000 pyguardpoint-1.4.2/pyGuardPoint/_odata_filter.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     1566 2024-03-13 09:54:42.000000 pyguardpoint-1.4.2/pyGuardPoint/_str_match_algo.py
+drwxr-xr-x   0 johnowen   (501) staff       (20)        0 2024-06-03 14:21:12.047542 pyguardpoint-1.4.2/pyGuardPoint/gp_asyncio/
+-rw-r--r--   0 johnowen   (501) staff       (20)        0 2024-03-13 09:54:42.000000 pyguardpoint-1.4.2/pyGuardPoint/gp_asyncio/__init__.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     2388 2024-05-30 09:17:55.000000 pyguardpoint-1.4.2/pyGuardPoint/gp_asyncio/_async_guardpoint_alarms.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     1266 2024-03-13 09:54:42.000000 pyguardpoint-1.4.2/pyGuardPoint/gp_asyncio/_async_guardpoint_areas.py
+-rw-r--r--   0 johnowen   (501) staff       (20)    12951 2024-05-31 11:47:57.000000 pyguardpoint-1.4.2/pyGuardPoint/gp_asyncio/_async_guardpoint_cardholders.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     1355 2024-03-13 09:54:42.000000 pyguardpoint-1.4.2/pyGuardPoint/gp_asyncio/_async_guardpoint_cardholdertypes.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     6900 2024-03-13 09:54:42.000000 pyguardpoint-1.4.2/pyGuardPoint/gp_asyncio/_async_guardpoint_cards.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     2527 2024-03-13 09:54:42.000000 pyguardpoint-1.4.2/pyGuardPoint/gp_asyncio/_async_guardpoint_controllers.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     1317 2024-03-13 09:54:42.000000 pyguardpoint-1.4.2/pyGuardPoint/gp_asyncio/_async_guardpoint_customizedfields.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     1873 2024-03-13 09:54:42.000000 pyguardpoint-1.4.2/pyGuardPoint/gp_asyncio/_async_guardpoint_diagnostic.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     3043 2024-05-31 10:17:21.000000 pyguardpoint-1.4.2/pyGuardPoint/gp_asyncio/_async_guardpoint_events.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     3862 2024-03-13 09:54:42.000000 pyguardpoint-1.4.2/pyGuardPoint/gp_asyncio/_async_guardpoint_ouputs.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     1343 2024-03-13 09:54:42.000000 pyguardpoint-1.4.2/pyGuardPoint/gp_asyncio/_async_guardpoint_personaldetails.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     2317 2024-05-30 09:17:55.000000 pyguardpoint-1.4.2/pyGuardPoint/gp_asyncio/_async_guardpoint_readers.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     2763 2024-03-13 09:54:42.000000 pyguardpoint-1.4.2/pyGuardPoint/gp_asyncio/_async_guardpoint_scheduledmags.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     1524 2024-03-13 09:54:42.000000 pyguardpoint-1.4.2/pyGuardPoint/gp_asyncio/_async_guardpoint_securitygroups.py
+-rw-r--r--   0 johnowen   (501) staff       (20)    12795 2024-05-28 14:49:38.000000 pyguardpoint-1.4.2/pyGuardPoint/gp_asyncio/guardpoint_connection_asyncio.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     5914 2024-05-31 11:36:24.000000 pyguardpoint-1.4.2/pyGuardPoint/guardpoint.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     9468 2024-05-31 11:27:33.000000 pyguardpoint-1.4.2/pyGuardPoint/guardpoint_asyncio.py
+-rw-r--r--   0 johnowen   (501) staff       (20)    11292 2024-05-31 11:49:13.000000 pyguardpoint-1.4.2/pyGuardPoint/guardpoint_connection.py
+-rw-r--r--   0 johnowen   (501) staff       (20)    33141 2024-05-31 11:36:24.000000 pyguardpoint-1.4.2/pyGuardPoint/guardpoint_dataclasses.py
+-rw-r--r--   0 johnowen   (501) staff       (20)       97 2024-03-13 09:54:42.000000 pyguardpoint-1.4.2/pyGuardPoint/guardpoint_error.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     3982 2024-03-13 09:54:42.000000 pyguardpoint-1.4.2/pyGuardPoint/guardpoint_threaded.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     4245 2024-03-13 09:54:42.000000 pyguardpoint-1.4.2/pyGuardPoint/guardpoint_utils.py
+drwxr-xr-x   0 johnowen   (501) staff       (20)        0 2024-06-03 14:21:12.047976 pyguardpoint-1.4.2/pyGuardPoint.egg-info/
+-rw-r--r--   0 johnowen   (501) staff       (20)    10657 2024-06-03 14:21:12.000000 pyguardpoint-1.4.2/pyGuardPoint.egg-info/PKG-INFO
+-rw-r--r--   0 johnowen   (501) staff       (20)     2037 2024-06-03 14:21:12.000000 pyguardpoint-1.4.2/pyGuardPoint.egg-info/SOURCES.txt
+-rw-r--r--   0 johnowen   (501) staff       (20)        1 2024-06-03 14:21:12.000000 pyguardpoint-1.4.2/pyGuardPoint.egg-info/dependency_links.txt
+-rw-r--r--   0 johnowen   (501) staff       (20)        1 2024-05-28 15:02:25.000000 pyguardpoint-1.4.2/pyGuardPoint.egg-info/not-zip-safe
+-rw-r--r--   0 johnowen   (501) staff       (20)       75 2024-06-03 14:21:12.000000 pyguardpoint-1.4.2/pyGuardPoint.egg-info/requires.txt
+-rw-r--r--   0 johnowen   (501) staff       (20)       13 2024-06-03 14:21:12.000000 pyguardpoint-1.4.2/pyGuardPoint.egg-info/top_level.txt
+-rw-r--r--   0 johnowen   (501) staff       (20)       38 2024-06-03 14:21:12.048478 pyguardpoint-1.4.2/setup.cfg
+-rw-r--r--   0 johnowen   (501) staff       (20)      632 2024-06-03 14:20:35.000000 pyguardpoint-1.4.2/setup.py
```

### Comparing `pyguardpoint-1.4.1/LICENSE.txt` & `pyguardpoint-1.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.4.1/PKG-INFO` & `pyguardpoint-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyGuardPoint
-Version: 1.4.1
+Version: 1.4.2
 Summary: Python wrapper for GuardPoint 10 Access Control System
 Author: John Owen
 Maintainer-email: sales@sensoraccess.co.uk
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: validators
 Requires-Dist: fuzzywuzzy
```

### Comparing `pyguardpoint-1.4.1/README.rst` & `pyguardpoint-1.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.4.1/pyGuardPoint/CustomWebsocketTransport.py` & `pyguardpoint-1.4.2/pyGuardPoint/CustomWebsocketTransport.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.4.1/pyGuardPoint/_guardpoint_alarms.py` & `pyguardpoint-1.4.2/pyGuardPoint/_guardpoint_alarms.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.4.1/pyGuardPoint/_guardpoint_areas.py` & `pyguardpoint-1.4.2/pyGuardPoint/gp_asyncio/_async_guardpoint_areas.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,21 @@
-from .guardpoint_utils import GuardPointResponse
-from .guardpoint_dataclasses import Area
-from .guardpoint_error import GuardPointError, GuardPointUnauthorized
+from ..guardpoint_utils import GuardPointResponse
+from ..guardpoint_dataclasses import Area
+from ..guardpoint_error import GuardPointError, GuardPointUnauthorized
 
 
 class AreasAPI:
-    """
-    A class to interact with the Areas API.
-
-    Methods
-    -------
-    get_areas():
-        Fetches a list of areas from the API and returns them as a list of Area objects.
-    """
-    def get_areas(self):
+    async def get_areas(self):
         url = "/odata/API_Areas"
         headers = {
             'Content-Type': 'application/json',
             'Accept': 'application/json'
         }
 
-        code, json_body = self.gp_json_query("GET", headers=headers, url=url)
+        code, json_body = await self.gp_json_query("GET", headers=headers, url=url)
 
         if code != 200:
             error_msg = GuardPointResponse.extract_error_msg(json_body)
 
             if code == 401:
                 raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
             elif code == 404:  # Not Found
```

### Comparing `pyguardpoint-1.4.1/pyGuardPoint/_guardpoint_cardholders.py` & `pyguardpoint-1.4.2/pyGuardPoint/_guardpoint_cardholders.py`

 * *Files 19% similar despite different names*

```diff
@@ -33,14 +33,33 @@
         Retrieves the photo of a cardholder by UID.
 
     get_card_holders(offset: int = 0, limit: int = 10, search_terms: str = None, areas: list = None, filter_expired: bool = False, cardholder_type_name: str = None, sort_algorithm: SortAlgorithm = SortAlgorithm.SERVER_DEFAULT, threshold: int = 75, count: bool = False, earliest_last_pass: datetime = None, select_ignore_list: list = None, select_include_list: list = None, **cardholder_kwargs)
         Retrieves a list of cardholders based on various filters and search criteria.
     """
 
     def delete_card_holder(self, cardholder: Cardholder):
+        """
+        Delete a cardholder from the system.
+
+        This method deletes a cardholder identified by their UID from the system.
+        It performs a validation check on the UID to ensure it is a valid UUID.
+        If the UID is malformed, a `ValueError` is raised. The method then sends
+        a DELETE request to the API endpoint to remove the cardholder.
+
+        :param cardholder: The cardholder object to be deleted.
+        :type cardholder: Cardholder
+
+        :raises ValueError: If the cardholder UID is malformed.
+        :raises GuardPointUnauthorized: If the request is unauthorized (HTTP 401).
+        :raises GuardPointError: If the cardholder is not found (HTTP 404) or
+                                 if another error occurs.
+
+        :return: True if the cardholder was successfully deleted.
+        :rtype: bool
+        """
         if not validators.uuid(cardholder.uid):
             raise ValueError(f'Malformed Cardholder UID {cardholder.uid}')
 
         url = self.baseurl + "/odata/API_Cardholders"
         url_query_params = "(" + cardholder.uid + ")"
 
         code, json_body = self.gp_json_query("DELETE", url=(url + url_query_params))
@@ -57,27 +76,56 @@
                 raise GuardPointError(f"Cardholder Not Found")
             else:
                 raise GuardPointError(f"{error_msg}")
 
         return True
 
     def update_card_holder_area(self, cardholder_uid: str, area: Area):
+        """
+        Update the area associated with a cardholder.
+
+        This method updates the area (location) information for a given cardholder by their unique identifier (UID).
+        It validates the provided UIDs for both the cardholder and the area before performing the update.
+
+        :param cardholder_uid: The unique identifier of the cardholder.
+        :type cardholder_uid: str
+        :param area: The area object containing the new area UID.
+        :type area: Area
+        :raises ValueError: If the cardholder UID or area UID is malformed (not a valid UUID).
+        :return: The result of the cardholder update operation.
+        :rtype: Any
+        """
         if not validators.uuid(cardholder_uid):
             raise ValueError(f'Malformed Cardholder UID {cardholder_uid}')
 
         if not validators.uuid(area.uid):
             raise ValueError(f'Malformed Area UID {area.uid}')
 
         cardholder = Cardholder()
         cardholder.uid = cardholder_uid
         cardholder.insideAreaUID = area.uid
 
         return self.update_card_holder(cardholder)
 
     def update_card_holder(self, cardholder: Cardholder):
+        """
+        Update the details of a cardholder in the system.
+
+        This method updates various attributes of a cardholder, including custom fields, personal details, and associated cards.
+        It performs validation on the cardholder's UID and the UIDs of associated cards. If any attributes have changed, it sends
+        a PATCH request to update the cardholder's information in the system.
+
+        :param cardholder: The cardholder object containing updated information.
+        :type cardholder: Cardholder
+        :raises ValueError: If the cardholder UID is malformed.
+        :raises GuardPointUnauthorized: If the request is unauthorized.
+        :raises GuardPointError: If the cardholder is not found or another error occurs.
+        :return: True if the update is successful, otherwise raises an exception.
+        :rtype: bool
+        """
         if not validators.uuid(cardholder.uid):
             raise ValueError(f'Malformed Cardholder UID {cardholder.uid}')
 
         if cardholder.cardholderCustomizedField:
             if len(cardholder.cardholderCustomizedField.changed_attributes) > 0:
                 self.update_custom_fields(cardholder.uid, cardholder.cardholderCustomizedField)
 
@@ -120,34 +168,48 @@
                 raise GuardPointError(f"Cardholder Not Found")
             else:
                 raise GuardPointError(f"{error_msg}")
 
         return True
 
     def new_card_holder(self, cardholder: Cardholder, changed_only=False):
+        """
+        Create a new cardholder in the system.
+
+        This method sends a POST request to the GuardPoint API to create a new cardholder.
+        Depending on the `changed_only` flag, it can either send only the changed fields or
+        all editable and non-empty fields of the cardholder.
+
+        :param cardholder: The cardholder object to be created.
+        :type cardholder: Cardholder
+        :param changed_only: If True, only the changed fields of the cardholder will be sent.
+                             Otherwise, all editable and non-empty fields will be sent.
+        :type changed_only: bool, optional
+
+        :return: The newly created cardholder object.
+        :rtype: Cardholder
 
-        # url = "/odata/API_Cardholders/CreateFullCardholder"
+        :raises GuardPointError: If there is an error in the request or response.
+        :raises GuardPointUnauthorized: If the request is unauthorized.
+        """
         url = "/odata/API_Cardholders"
 
         headers = {
             'Content-Type': 'application/json',
             'Accept': 'application/json',
             'IgnoreNonEditable': ''
         }
 
         if changed_only:
             ch = cardholder.dict(editable_only=True, changed_only=True, non_empty_only=True)
         else:
             ch = cardholder.dict(editable_only=True, non_empty_only=True)
 
-
-        # When using CreateFullCardholder
-        # body = {'cardholder': ch}
-        # print(json.dumps(body))
         code, json_body = self.gp_json_query("POST", headers=headers, url=url, json_body=ch)
+
         # Check response body is formatted correctly
         if json_body:
             GuardPointResponse.check_odata_body_structure(json_body)
 
         if code == 201:  # HTTP CREATED
             new_cardholder = Cardholder(json_body)
             if cardholder.cardholderPersonalDetail:
@@ -202,24 +264,37 @@
         if card_code:
             # Part of the Cards_API
             return self.get_cardholder_by_card_code(card_code)
         else:
             return self._get_card_holder(uid)
 
     def get_card_holder_photo(self, uid):
+        """
+        Retrieve the photo of a cardholder given their unique identifier (UID).
+
+        This method sends a GET request to the GuardPoint API to fetch the photo of a cardholder.
+        The UID must be a valid UUID. If the UID is malformed, a ValueError is raised. If the
+        request is unauthorized, a GuardPointUnauthorized exception is raised. If the cardholder
+        photo is not found, a GuardPointError is raised.
+
+        :param uid: The unique identifier of the cardholder.
+        :type uid: str
+        :raises ValueError: If the UID is not a valid UUID.
+        :raises GuardPointUnauthorized: If the request is unauthorized.
+        :raises GuardPointError: If the cardholder photo is not found or another error occurs.
+        :return: The photo of the cardholder.
+        :rtype: str
+        """
         if not validators.uuid(uid):
             raise ValueError(f'Malformed UID {uid}')
 
         url = "/odata/API_Cardholders"
         url_query_params = "(" + uid + ")?$select=photo"
 
         code, json_body = self.gp_json_query("GET", url=(url + url_query_params))
-        # Check response body is formatted correctly
-        # if json_body:
-        #    GuardPointResponse.check_odata_body_structure(json_body)
 
         if code != 200:
             error_msg = GuardPointResponse.extract_error_msg(json_body)
 
             if code == 401:
                 raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
             elif code == 404:  # Not Found
```

### Comparing `pyguardpoint-1.4.1/pyGuardPoint/_guardpoint_cardholdertypes.py` & `pyguardpoint-1.4.2/pyGuardPoint/_guardpoint_cardholdertypes.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.4.1/pyGuardPoint/_guardpoint_cards.py` & `pyguardpoint-1.4.2/pyGuardPoint/gp_asyncio/_async_guardpoint_cards.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,16 @@
 import validators
-from .guardpoint_utils import GuardPointResponse
-from ._odata_filter import _compose_filter
-from .guardpoint_dataclasses import Card, Cardholder
-from .guardpoint_error import GuardPointError, GuardPointUnauthorized
+from ..guardpoint_utils import GuardPointResponse
+from .._odata_filter import _compose_filter
+from ..guardpoint_dataclasses import Card, Cardholder
+from ..guardpoint_error import GuardPointError, GuardPointUnauthorized
 
 
 class CardsAPI:
-    """
-    A class to interact with the Cards API, providing methods to manage card entities.
-
-    Methods
-    -------
-    get_cards(count=False, **card_kwargs)
-        Retrieve a list of cards or the count of cards based on the provided filters.
-
-    delete_card(card: Card)
-        Delete a card identified by its UID.
-
-    update_card(card: Card)
-        Update the details of an existing card.
-
-    new_card(card: Card)
-        Create a new card.
-
-    get_card(card_uid: str)
-        Retrieve a card by its UID.
-
-    get_cardholder_by_card_code(card_code)
-        Retrieve a cardholder by the card code.
-    """
-    def get_cards(self, count=False, **card_kwargs):
+    async def get_cards(self, count=False, **card_kwargs):
         # Filter arguments which have to exact match
         match_args = dict()
         for k, v in card_kwargs.items():
             if hasattr(Card, k):
                 match_args[k] = v
 
         url = "/odata/API_Cards"
@@ -44,15 +21,15 @@
 
         if count:
             url_query_params = "?$count=true&$top=0"
         else:
             filter_str = _compose_filter(exact_match=match_args)
             url_query_params = ("?" + filter_str)
 
-        code, json_body = self.gp_json_query("GET", headers=headers, url=(url+url_query_params))
+        code, json_body = await self.gp_json_query("GET", headers=headers, url=(url+url_query_params))
 
         if code != 200:
             error_msg = GuardPointResponse.extract_error_msg(json_body)
 
             if code == 401:
                 raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
             elif code == 404:  # Not Found
@@ -71,96 +48,96 @@
             return json_body['@odata.count']
 
         cards = []
         for x in json_body['value']:
             cards.append(Card(x))
         return cards
 
-    def delete_card(self, card: Card):
+    async def delete_card(self, card: Card):
         if not validators.uuid(card.uid):
             raise ValueError(f'Malformed Card UID {card.uid}')
 
         url = "/odata/API_Cards"
         url_query_params = "(" + card.uid + ")"
         headers = {
             'Content-Type': 'application/json',
             'Accept': 'application/json'
         }
 
-        code, json_body = self.gp_json_query("DELETE", headers=headers, url=(url + url_query_params))
+        code, json_body = await self.gp_json_query("DELETE", headers=headers, url=(url + url_query_params))
 
         if code != 204:  # HTTP NO_CONTENT
             error_msg = GuardPointResponse.extract_error_msg(json_body)
 
             if code == 401:
                 raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
             elif code == 404:  # Not Found
                 raise GuardPointError(f"Card Not Found")
             else:
                 raise GuardPointError(f"{error_msg}")
 
         return True
 
-    def update_card(self, card: Card):
+    async def update_card(self, card: Card):
         if not validators.uuid(card.uid):
             raise ValueError(f'Malformed Card UID {card.uid}')
 
         url = "/odata/API_Cards"
         url_query_params = f"({card.uid})"
 
         headers = {
             'Content-Type': 'application/json',
             'Accept': 'application/json',
             # 'IgnoreNonEditable': ''
         }
 
         ch = card.dict(changed_only=True)
 
-        code, json_body = self.gp_json_query("PATCH", headers=headers, url=(url + url_query_params), json_body=ch)
+        code, json_body = await self.gp_json_query("PATCH", headers=headers, url=(url + url_query_params), json_body=ch)
 
         if code != 204:  # HTTP NO_CONTENT
             error_msg = GuardPointResponse.extract_error_msg(json_body)
 
             if code == 401:
                 raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
             else:
                 raise GuardPointError(f"No body - ({code})")
 
         return True
 
-    def new_card(self, card: Card):
+    async def new_card(self, card: Card):
         url = "/odata/API_Cards"
         headers = {
             'Content-Type': 'application/json',
             'Accept': 'application/json',
         }
         body = card.dict(editable_only=True)
 
-        code, json_body = self.gp_json_query("POST", headers=headers, url=url, json_body=body)
+        code, json_body = await self.gp_json_query("POST", headers=headers, url=url, json_body=body)
 
         if code == 201:  # HTTP CREATED
             return Card(json_body)
         else:
             if "errorMessages" in json_body:
                 raise GuardPointError(json_body["errorMessages"][0]["other"])
             elif "message" in json_body:
                 raise GuardPointError(json_body['message'])
             else:
                 raise GuardPointError(str(code))
 
-    def get_card(self, card_uid: str):
+    async def get_card(self, card_uid: str):
         url = "/odata/API_Cards"
         headers = {
             'Content-Type': 'application/json',
             'Accept': 'application/json',
         }
 
         url_query_params = f"({card_uid})"
 
-        code, json_body = self.gp_json_query("GET", headers=headers, url=(url + url_query_params))
+        code, json_body = await self.gp_json_query("GET", headers=headers, url=(url + url_query_params))
 
         if code != 200:
             if isinstance(json_body, dict):
                 if 'error' in json_body:
                     raise GuardPointError(json_body['error'])
             else:
                 raise GuardPointError(str(code))
@@ -169,15 +146,15 @@
         if not isinstance(json_body, dict):
             raise GuardPointError("Badly formatted response.")
         if 'value' not in json_body:
             raise GuardPointError("Badly formatted response.")
 
         return Card(json_body['value'])
 
-    def get_cardholder_by_card_code(self, card_code):
+    async def get_cardholder_by_card_code(self, card_code):
         url = "/odata/API_Cards"
         filter_str = f"?$filter=cardcode%20eq%20'{card_code}'%20and%20status%20eq%20'Used'%20&"
         url_query_params = f"{filter_str}" \
                            f"$expand=cardholder(" \
                            "$expand=securityGroup($select=name)," \
                            "cardholderType($select=typeName)," \
                            "cards," \
@@ -187,15 +164,15 @@
                            "insideArea)" \
 
         headers = {
             'Content-Type': 'application/json',
             'Accept': 'application/json',
         }
 
-        code, json_body = self.gp_json_query("GET", headers=headers, url=(url + url_query_params))
+        code, json_body = await self.gp_json_query("GET", headers=headers, url=(url + url_query_params))
 
         if code != 200:
             if isinstance(json_body, dict):
                 if 'error' in json_body:
                     raise GuardPointError(json_body['error'])
 
         if not isinstance(json_body, dict):
```

### Comparing `pyguardpoint-1.4.1/pyGuardPoint/_guardpoint_controllers.py` & `pyguardpoint-1.4.2/pyGuardPoint/_guardpoint_controllers.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.4.1/pyGuardPoint/_guardpoint_customizedfields.py` & `pyguardpoint-1.4.2/pyGuardPoint/_guardpoint_customizedfields.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.4.1/pyGuardPoint/_guardpoint_diagnostic.py` & `pyguardpoint-1.4.2/pyGuardPoint/_guardpoint_diagnostic.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.4.1/pyGuardPoint/_guardpoint_events.py` & `pyguardpoint-1.4.2/pyGuardPoint/gp_asyncio/_async_guardpoint_events.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import validators
 
-from .guardpoint_utils import GuardPointResponse
-from .guardpoint_dataclasses import AlarmEvent, AccessEvent
-from .guardpoint_error import GuardPointError, GuardPointUnauthorized
+from ..guardpoint_utils import GuardPointResponse
+from ..guardpoint_dataclasses import AccessEvent, AlarmEvent
+from ..guardpoint_error import GuardPointError, GuardPointUnauthorized
 
 
 class EventsAPI:
-    def get_access_events(self, limit=None, offset=None):
+    async def get_access_events(self, limit=None, offset=None):
         url = f"/odata/API_AccessEventLogs"
         headers = {
             'Content-Type': 'application/json',
             'Accept': 'application/json'
         }
 
         url_query_params = "?$orderby=dateTime%20desc"
 
         if limit:
             url_query_params += "&$top=" + str(limit)
         if offset:
             url_query_params += "&$skip=" + str(offset)
 
-        code, json_body = self.gp_json_query("GET", headers=headers, url=(url + url_query_params))
+        code, json_body = await self.gp_json_query("GET", headers=headers, url=(url + url_query_params))
 
         if code != 200:
             error_msg = GuardPointResponse.extract_error_msg(json_body)
 
             if code == 401:
                 raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
             elif code == 404:  # Not Found
@@ -41,29 +41,29 @@
             raise GuardPointError("Badly formatted response.")
 
         access_events = []
         for x in json_body['value']:
             access_events.append(AccessEvent(x))
         return access_events
 
-    def get_alarm_events(self, limit=None, offset=None):
+    async def get_alarm_events(self, limit=None, offset=None):
         url = "/odata/API_AlarmEventLogs"
         headers = {
             'Content-Type': 'application/json',
             'Accept': 'application/json'
         }
 
         url_query_params = "?$orderby=dateTime%20asc"
 
         if limit:
             url_query_params += "&$top=" + str(limit)
         if offset:
             url_query_params += "&$skip=" + str(offset)
 
-        code, json_body = self.gp_json_query("GET", headers=headers, url=(url+url_query_params))
+        code, json_body = await self.gp_json_query("GET", headers=headers, url=(url+url_query_params))
 
         if code != 200:
             error_msg = GuardPointResponse.extract_error_msg(json_body)
 
             if code == 401:
                 raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
             elif code == 404:  # Not Found
```

### Comparing `pyguardpoint-1.4.1/pyGuardPoint/_guardpoint_ouputs.py` & `pyguardpoint-1.4.2/pyGuardPoint/_guardpoint_ouputs.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.4.1/pyGuardPoint/_guardpoint_personaldetails.py` & `pyguardpoint-1.4.2/pyGuardPoint/gp_asyncio/_async_guardpoint_customizedfields.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 import validators
-from .guardpoint_utils import GuardPointResponse
-from .guardpoint_error import GuardPointError, GuardPointUnauthorized
-from .guardpoint_dataclasses import CardholderPersonalDetail
+from ..guardpoint_utils import GuardPointResponse
+from ..guardpoint_error import GuardPointError, GuardPointUnauthorized
+from ..guardpoint_dataclasses import CardholderCustomizedField
 
 
-class PersonalDetailsAPI:
+class CustomizedFieldsAPI:
 
-    def update_personal_details(self, cardholder_uid: str, personal_details: CardholderPersonalDetail):
+    async def update_custom_fields(self, cardholder_uid: str, customFields: CardholderCustomizedField):
         if not validators.uuid(cardholder_uid):
             raise ValueError(f'Malformed Cardholder UID {cardholder_uid}')
 
-        url = "/odata/API_CardholderPersonalDetails"
+        url = "/odata/API_CardholderCustomizedFields"
         url_query_params = f"({cardholder_uid})"
 
         headers = {
             'Content-Type': 'application/json',
             'Accept': 'application/json',
             # 'IgnoreNonEditable': ''
         }
 
-        ch = personal_details.dict(editable_only=True, changed_only=True)
+        ch = customFields.dict(changed_only=True)
 
-        code, json_body = self.gp_json_query("PATCH", headers=headers, url=(url + url_query_params), json_body=ch)
+        code, json_body = await self.gp_json_query("PATCH", headers=headers, url=(url + url_query_params), json_body=ch)
 
         if code != 204:  # HTTP NO_CONTENT
             error_msg = GuardPointResponse.extract_error_msg(json_body)
 
             if code == 401:
                 raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
             elif code == 404:  # Not Found
                 raise GuardPointError(f"Cardholder Not Found")
             else:
                 raise GuardPointError(f"{error_msg}")
 
-        return True
+        return True
```

### Comparing `pyguardpoint-1.4.1/pyGuardPoint/_guardpoint_readers.py` & `pyguardpoint-1.4.2/pyGuardPoint/gp_asyncio/_async_guardpoint_readers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import validators
-from .guardpoint_utils import GuardPointResponse
-from .guardpoint_dataclasses import Reader
-from .guardpoint_error import GuardPointError, GuardPointUnauthorized
+from ..guardpoint_utils import GuardPointResponse
+from ..guardpoint_dataclasses import Reader
+from ..guardpoint_error import GuardPointError, GuardPointUnauthorized
 
 
 class ReadersAPI:
-    def get_readers(self, ):
+    async def get_readers(self):
         url = "/odata/API_Readers"
         headers = {
             'Content-Type': 'application/json',
             'Accept': 'application/json'
         }
 
-        code, json_body = self.gp_json_query("GET", headers=headers, url=url)
+        code, json_body = await self.gp_json_query("GET", headers=headers, url=url)
 
         if code != 200:
             error_msg = GuardPointResponse.extract_error_msg(json_body)
 
             if code == 401:
                 raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
             elif code == 404:  # Not Found
@@ -32,27 +32,27 @@
             raise GuardPointError("Badly formatted response.")
 
         readers = []
         for x in json_body['value']:
             readers.append(Reader(x))
         return readers
 
-    def get_reader(self, reader_uid: str):
+    async def get_reader(self, reader_uid: str):
         if not validators.uuid(reader_uid):
             raise ValueError(f"Malformed reader_uid: {reader_uid}")
 
         url = "/odata/API_Readers"
         headers = {
             'Content-Type': 'application/json',
             'Accept': 'application/json',
         }
 
         url_query_params = f"({reader_uid})"
 
-        code, json_body = self.gp_json_query("GET", headers=headers, url=(url + url_query_params))
+        code, json_body = await self.gp_json_query("GET", headers=headers, url=(url + url_query_params))
 
         if code != 200:
             if isinstance(json_body, dict):
                 if 'error' in json_body:
                     raise GuardPointError(json_body['error'])
             else:
                 raise GuardPointError(str(code))
```

### Comparing `pyguardpoint-1.4.1/pyGuardPoint/_guardpoint_scheduledmags.py` & `pyguardpoint-1.4.2/pyGuardPoint/_guardpoint_scheduledmags.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.4.1/pyGuardPoint/_guardpoint_securitygroups.py` & `pyguardpoint-1.4.2/pyGuardPoint/gp_asyncio/_async_guardpoint_securitygroups.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from .guardpoint_utils import GuardPointResponse
-from .guardpoint_dataclasses import SecurityGroup
-from .guardpoint_error import GuardPointError, GuardPointUnauthorized
+from ..guardpoint_utils import GuardPointResponse
+from ..guardpoint_dataclasses import SecurityGroup
+from ..guardpoint_error import GuardPointError, GuardPointUnauthorized
 
 
 class SecurityGroupsAPI:
-    def get_security_groups(self):
-        url = self.baseurl + "/odata/api_SecurityGroups"
+    async def get_security_groups(self):
+        url = "/odata/api_SecurityGroups"
         # url_query_params = "?$select=uid,name&$filter=name%20ne%20'Anytime%20Anywhere'"
         url_query_params = ""
-        code, json_body = self.gp_json_query("GET", url=(url + url_query_params))
+        code, json_body = await self.gp_json_query("GET", url=(url + url_query_params))
 
         if code != 200:
             error_msg = GuardPointResponse.extract_error_msg(json_body)
 
             if code == 401:
                 raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
             elif code == 404:  # Not Found
```

### Comparing `pyguardpoint-1.4.1/pyGuardPoint/_odata_filter.py` & `pyguardpoint-1.4.2/pyGuardPoint/_odata_filter.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.4.1/pyGuardPoint/_str_match_algo.py` & `pyguardpoint-1.4.2/pyGuardPoint/_str_match_algo.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.4.1/pyGuardPoint/gp_asyncio/_async_guardpoint_alarms.py` & `pyguardpoint-1.4.2/pyGuardPoint/gp_asyncio/_async_guardpoint_alarms.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.4.1/pyGuardPoint/gp_asyncio/_async_guardpoint_cardholders.py` & `pyguardpoint-1.4.2/pyGuardPoint/gp_asyncio/_async_guardpoint_cardholders.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.4.1/pyGuardPoint/gp_asyncio/_async_guardpoint_cardholdertypes.py` & `pyguardpoint-1.4.2/pyGuardPoint/gp_asyncio/_async_guardpoint_cardholdertypes.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.4.1/pyGuardPoint/gp_asyncio/_async_guardpoint_controllers.py` & `pyguardpoint-1.4.2/pyGuardPoint/gp_asyncio/_async_guardpoint_controllers.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.4.1/pyGuardPoint/gp_asyncio/_async_guardpoint_customizedfields.py` & `pyguardpoint-1.4.2/pyGuardPoint/gp_asyncio/_async_guardpoint_personaldetails.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 import validators
 from ..guardpoint_utils import GuardPointResponse
 from ..guardpoint_error import GuardPointError, GuardPointUnauthorized
-from ..guardpoint_dataclasses import CardholderCustomizedField
+from ..guardpoint_dataclasses import CardholderPersonalDetail
 
 
-class CustomizedFieldsAPI:
+class PersonalDetailsAPI:
 
-    async def update_custom_fields(self, cardholder_uid: str, customFields: CardholderCustomizedField):
+    async def update_personal_details(self, cardholder_uid: str, personal_details: CardholderPersonalDetail):
         if not validators.uuid(cardholder_uid):
             raise ValueError(f'Malformed Cardholder UID {cardholder_uid}')
 
-        url = "/odata/API_CardholderCustomizedFields"
+        url = "/odata/API_CardholderPersonalDetails"
         url_query_params = f"({cardholder_uid})"
 
         headers = {
             'Content-Type': 'application/json',
             'Accept': 'application/json',
             # 'IgnoreNonEditable': ''
         }
 
-        ch = customFields.dict(changed_only=True)
+        ch = personal_details.dict(editable_only=True, changed_only=True)
 
         code, json_body = await self.gp_json_query("PATCH", headers=headers, url=(url + url_query_params), json_body=ch)
 
         if code != 204:  # HTTP NO_CONTENT
             error_msg = GuardPointResponse.extract_error_msg(json_body)
 
             if code == 401:
                 raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
             elif code == 404:  # Not Found
                 raise GuardPointError(f"Cardholder Not Found")
             else:
                 raise GuardPointError(f"{error_msg}")
 
-        return True
+        return True
```

### Comparing `pyguardpoint-1.4.1/pyGuardPoint/gp_asyncio/_async_guardpoint_diagnostic.py` & `pyguardpoint-1.4.2/pyGuardPoint/gp_asyncio/_async_guardpoint_diagnostic.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.4.1/pyGuardPoint/gp_asyncio/_async_guardpoint_events.py` & `pyguardpoint-1.4.2/pyGuardPoint/_guardpoint_securitygroups.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,84 +1,60 @@
-import validators
-
-from ..guardpoint_utils import GuardPointResponse
-from ..guardpoint_dataclasses import AccessEvent, AlarmEvent
-from ..guardpoint_error import GuardPointError, GuardPointUnauthorized
-
-
-class EventsAPI:
-    async def get_access_events(self, limit=None, offset=None):
-        url = f"/odata/API_AccessEventLogs"
-        headers = {
-            'Content-Type': 'application/json',
-            'Accept': 'application/json'
-        }
-
-        url_query_params = "?$orderby=dateTime%20desc"
-
-        if limit:
-            url_query_params += "&$top=" + str(limit)
-        if offset:
-            url_query_params += "&$skip=" + str(offset)
-
-        code, json_body = await self.gp_json_query("GET", headers=headers, url=(url + url_query_params))
+from .guardpoint_utils import GuardPointResponse
+from .guardpoint_dataclasses import SecurityGroup
+from .guardpoint_error import GuardPointError, GuardPointUnauthorized
+
+
+class SecurityGroupsAPI:
+    """
+    A class to interact with the Security Groups API.
+
+    Methods
+    -------
+    get_security_groups():
+        Retrieves a list of security groups from the API.
+    """
+    def get_security_groups(self):
+        """
+        Retrieve a list of security groups from the GuardPoint API.
+
+        This method sends a GET request to the GuardPoint API to fetch security groups.
+        It handles various HTTP response codes and raises appropriate exceptions for
+        unauthorized access, not found errors, and other errors. The response is expected
+        to be a JSON object containing a list of security groups.
+
+        :raises GuardPointUnauthorized: If the API response code is 401 (Unauthorized).
+        :raises GuardPointError: If the API response code is 404 (Not Found) or any other error occurs.
+        :raises GuardPointError: If the response body is not formatted as expected.
+
+        :return: A list of SecurityGroup objects.
+        :rtype: list
+        """
+        url = self.baseurl + "/odata/api_SecurityGroups"
+        # url_query_params = "?$select=uid,name&$filter=name%20ne%20'Anytime%20Anywhere'"
+        url_query_params = ""
+        code, json_body = self.gp_json_query("GET", url=(url + url_query_params))
 
         if code != 200:
             error_msg = GuardPointResponse.extract_error_msg(json_body)
 
             if code == 401:
                 raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
             elif code == 404:  # Not Found
-                raise GuardPointError(f"Access Events Not Found")
+                raise GuardPointError(f"Security Group Not Found")
             else:
                 raise GuardPointError(f"{error_msg}")
 
         # Check response body is formatted as expected
         if not isinstance(json_body, dict):
             raise GuardPointError("Badly formatted response.")
         if 'value' not in json_body:
             raise GuardPointError("Badly formatted response.")
         if not isinstance(json_body['value'], list):
             raise GuardPointError("Badly formatted response.")
 
-        access_events = []
-        for x in json_body['value']:
-            access_events.append(AccessEvent(x))
-        return access_events
-
-    async def get_alarm_events(self, limit=None, offset=None):
-        url = "/odata/API_AlarmEventLogs"
-        headers = {
-            'Content-Type': 'application/json',
-            'Accept': 'application/json'
-        }
-
-        url_query_params = "?$orderby=dateTime%20asc"
-
-        if limit:
-            url_query_params += "&$top=" + str(limit)
-        if offset:
-            url_query_params += "&$skip=" + str(offset)
-
-        code, json_body = await self.gp_json_query("GET", headers=headers, url=(url+url_query_params))
-
-        if code != 200:
-            error_msg = GuardPointResponse.extract_error_msg(json_body)
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            elif code == 404:  # Not Found
-                raise GuardPointError(f"Alarm Events Not Found")
-            else:
-                raise GuardPointError(f"{error_msg}")
-
-        if not isinstance(json_body, dict):
-            raise GuardPointError("Badly formatted response.")
-        if 'value' not in json_body:
-            raise GuardPointError("Badly formatted response.")
-        if not isinstance(json_body['value'], list):
-            raise GuardPointError("Badly formatted response.")
-
-        alarm_events = []
-        for x in json_body['value']:
-            alarm_events.append(AlarmEvent(x))
-        return alarm_events
+        # Compose list of security groups
+        security_groups = []
+        for entry in json_body['value']:
+            if isinstance(entry, dict):
+                sg = SecurityGroup(entry)
+                security_groups.append(sg)
+        return security_groups
```

### Comparing `pyguardpoint-1.4.1/pyGuardPoint/gp_asyncio/_async_guardpoint_ouputs.py` & `pyguardpoint-1.4.2/pyGuardPoint/gp_asyncio/_async_guardpoint_ouputs.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.4.1/pyGuardPoint/gp_asyncio/_async_guardpoint_readers.py` & `pyguardpoint-1.4.2/pyGuardPoint/gp_asyncio/_async_guardpoint_scheduledmags.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,67 +1,70 @@
 import validators
 from ..guardpoint_utils import GuardPointResponse
-from ..guardpoint_dataclasses import Reader
+from ..guardpoint_dataclasses import ScheduledMag, Cardholder
 from ..guardpoint_error import GuardPointError, GuardPointUnauthorized
 
 
-class ReadersAPI:
-    async def get_readers(self):
-        url = "/odata/API_Readers"
-        headers = {
-            'Content-Type': 'application/json',
-            'Accept': 'application/json'
-        }
+class ScheduledMagsAPI:
+
+    async def get_scheduled_mags(self, cardholder: Cardholder = None):
+        url = "/odata/API_ScheduledMags"
+        if cardholder:
+            if not validators.uuid(cardholder.uid):
+                raise ValueError(f'Malformed Cardholder UID {cardholder.uid}')
+            url_query_params = f"?$filter=cardholderUid%20eq%20'{cardholder.uid}'"
+        else:
+            url_query_params = ""
 
-        code, json_body = await self.gp_json_query("GET", headers=headers, url=url)
+        code, json_body = await self.gp_json_query("GET", url=(url + url_query_params))
 
         if code != 200:
             error_msg = GuardPointResponse.extract_error_msg(json_body)
 
             if code == 401:
                 raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
             elif code == 404:  # Not Found
-                raise GuardPointError(f"Cardholder Not Found")
+                raise GuardPointError(f"MAG Not Found")
             else:
                 raise GuardPointError(f"{error_msg}")
 
+        # Check response body is formatted as expected
         if not isinstance(json_body, dict):
             raise GuardPointError("Badly formatted response.")
         if 'value' not in json_body:
             raise GuardPointError("Badly formatted response.")
         if not isinstance(json_body['value'], list):
             raise GuardPointError("Badly formatted response.")
 
-        readers = []
-        for x in json_body['value']:
-            readers.append(Reader(x))
-        return readers
-
-    async def get_reader(self, reader_uid: str):
-        if not validators.uuid(reader_uid):
-            raise ValueError(f"Malformed reader_uid: {reader_uid}")
+        # Compose list of security groups
+        scheduled_mags = []
+        for entry in json_body['value']:
+            if isinstance(entry, dict):
+                sm = ScheduledMag(entry)
+                scheduled_mags.append(sm)
+        return scheduled_mags
 
-        url = "/odata/API_Readers"
+    def add_scheduled_mag(self, scheduled_mag: ScheduledMag):
+        url = self.baseurl + "/odata/API_ScheduledMags"
         headers = {
             'Content-Type': 'application/json',
             'Accept': 'application/json',
         }
+        body = scheduled_mag.dict(editable_only=True)
 
-        url_query_params = f"({reader_uid})"
-
-        code, json_body = await self.gp_json_query("GET", headers=headers, url=(url + url_query_params))
+        code, json_body = self.gp_json_query("POST", headers=headers, url=url, json_body=body)
 
-        if code != 200:
-            if isinstance(json_body, dict):
-                if 'error' in json_body:
-                    raise GuardPointError(json_body['error'])
+        if code == 201:  # HTTP CREATED
+            return json_body['uid']
+        else:
+            if 'value' in json_body:
+                if isinstance(json_body['value'], list):
+                    json_body = json_body['value'][0]
             else:
-                raise GuardPointError(str(code))
-
-        # Check response body is formatted as expected
-        if not isinstance(json_body, dict):
-            raise GuardPointError("Badly formatted response.")
-        if 'value' not in json_body:
-            raise GuardPointError("Badly formatted response.")
-
-        return Reader(json_body['value'])
+                error_msg = GuardPointResponse.extract_error_msg(json_body)
 
+                if code == 401:
+                    raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+                elif code == 404:  # Not Found
+                    raise GuardPointError(f"Cardholder Not Found")
+                else:
+                    raise GuardPointError(f"{error_msg}")
```

### Comparing `pyguardpoint-1.4.1/pyGuardPoint/gp_asyncio/guardpoint_connection_asyncio.py` & `pyguardpoint-1.4.2/pyGuardPoint/gp_asyncio/guardpoint_connection_asyncio.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.4.1/pyGuardPoint/guardpoint.py` & `pyguardpoint-1.4.2/pyGuardPoint/guardpoint.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.4.1/pyGuardPoint/guardpoint_asyncio.py` & `pyguardpoint-1.4.2/pyGuardPoint/guardpoint_asyncio.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.4.1/pyGuardPoint/guardpoint_connection.py` & `pyguardpoint-1.4.2/pyGuardPoint/guardpoint_connection.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.4.1/pyGuardPoint/guardpoint_dataclasses.py` & `pyguardpoint-1.4.2/pyGuardPoint/guardpoint_dataclasses.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.4.1/pyGuardPoint/guardpoint_threaded.py` & `pyguardpoint-1.4.2/pyGuardPoint/guardpoint_threaded.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.4.1/pyGuardPoint/guardpoint_utils.py` & `pyguardpoint-1.4.2/pyGuardPoint/guardpoint_utils.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.4.1/pyGuardPoint.egg-info/PKG-INFO` & `pyguardpoint-1.4.2/pyGuardPoint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyGuardPoint
-Version: 1.4.1
+Version: 1.4.2
 Summary: Python wrapper for GuardPoint 10 Access Control System
 Author: John Owen
 Maintainer-email: sales@sensoraccess.co.uk
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: validators
 Requires-Dist: fuzzywuzzy
```

### Comparing `pyguardpoint-1.4.1/pyGuardPoint.egg-info/SOURCES.txt` & `pyguardpoint-1.4.2/pyGuardPoint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.4.1/setup.py` & `pyguardpoint-1.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 long_description = open('README.rst').read()
 
 setup(name="pyGuardPoint",
       packages=find_packages(),
-      version="1.4.1",
+      version="1.4.2",
       author="John Owen",
       description="Python wrapper for GuardPoint 10 Access Control System",
       long_description_content_type='text/markdown',
       long_description=long_description,
       maintainer_email="sales@sensoraccess.co.uk",
       install_requires=['validators', 'fuzzywuzzy', 'cryptography', 'pysignalr', 'websockets', 'python-Levenshtein'],
       #packages=['pyGuardPoint'],
```

