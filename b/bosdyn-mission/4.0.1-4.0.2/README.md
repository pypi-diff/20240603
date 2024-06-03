# Comparing `tmp/bosdyn_mission-4.0.1-py3-none-any.whl.zip` & `tmp/bosdyn_mission-4.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
 Zip file size: 16379 bytes, number of entries: 12
--rw-r--r--  2.0 unx      330 b- defN 24-Apr-12 01:43 bosdyn/__init__.py
--rw-r--r--  2.0 unx      483 b- defN 24-Apr-12 01:43 bosdyn/mission/__init__.py
--rw-r--r--  2.0 unx    22437 b- defN 24-Apr-12 01:43 bosdyn/mission/client.py
--rw-r--r--  2.0 unx      435 b- defN 24-Apr-12 01:43 bosdyn/mission/constants.py
--rw-r--r--  2.0 unx     3941 b- defN 24-Apr-12 01:43 bosdyn/mission/exceptions.py
--rw-r--r--  2.0 unx    12190 b- defN 24-Apr-12 01:43 bosdyn/mission/remote_client.py
--rw-r--r--  2.0 unx     1508 b- defN 24-Apr-12 01:43 bosdyn/mission/server_util.py
--rw-r--r--  2.0 unx    15616 b- defN 24-Apr-12 01:43 bosdyn/mission/util.py
--rw-r--r--  2.0 unx     1760 b- defN 24-Apr-12 01:44 bosdyn_mission-4.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-12 01:44 bosdyn_mission-4.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-Apr-12 01:44 bosdyn_mission-4.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      986 b- defN 24-Apr-12 01:44 bosdyn_mission-4.0.1.dist-info/RECORD
+-rw-r--r--  2.0 unx      330 b- defN 24-May-28 15:21 bosdyn/__init__.py
+-rw-r--r--  2.0 unx      483 b- defN 24-May-28 15:21 bosdyn/mission/__init__.py
+-rw-r--r--  2.0 unx    22437 b- defN 24-May-28 15:21 bosdyn/mission/client.py
+-rw-r--r--  2.0 unx      435 b- defN 24-May-28 15:21 bosdyn/mission/constants.py
+-rw-r--r--  2.0 unx     3941 b- defN 24-May-28 15:21 bosdyn/mission/exceptions.py
+-rw-r--r--  2.0 unx    12190 b- defN 24-May-28 15:21 bosdyn/mission/remote_client.py
+-rw-r--r--  2.0 unx     1508 b- defN 24-May-28 15:21 bosdyn/mission/server_util.py
+-rw-r--r--  2.0 unx    15616 b- defN 24-May-28 15:21 bosdyn/mission/util.py
+-rw-r--r--  2.0 unx     1760 b- defN 24-May-28 15:22 bosdyn_mission-4.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-28 15:22 bosdyn_mission-4.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-May-28 15:22 bosdyn_mission-4.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      986 b- defN 24-May-28 15:22 bosdyn_mission-4.0.2.dist-info/RECORD
 12 files, 59785 bytes uncompressed, 14723 bytes compressed:  75.4%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: bosdyn/mission/server_util.py
 Comment: 
 
 Filename: bosdyn/mission/util.py
 Comment: 
 
-Filename: bosdyn_mission-4.0.1.dist-info/METADATA
+Filename: bosdyn_mission-4.0.2.dist-info/METADATA
 Comment: 
 
-Filename: bosdyn_mission-4.0.1.dist-info/WHEEL
+Filename: bosdyn_mission-4.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: bosdyn_mission-4.0.1.dist-info/top_level.txt
+Filename: bosdyn_mission-4.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: bosdyn_mission-4.0.1.dist-info/RECORD
+Filename: bosdyn_mission-4.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `bosdyn_mission-4.0.1.dist-info/METADATA` & `bosdyn_mission-4.0.2.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: bosdyn-mission
-Version: 4.0.1
+Version: 4.0.2
 Summary: Boston Dynamics mission code
 Home-page: https://dev.bostondynamics.com/
 Author: Boston Dynamics
 Author-email: support@bostondynamics.com
 Project-URL: Documentation, https://dev.bostondynamics.com/
 Project-URL: Source, https://github.com/boston-dynamics/spot-sdk/
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: bosdyn-client (==4.0.1)
-Requires-Dist: bosdyn-api (==4.0.1)
+Requires-Dist: bosdyn-client (==4.0.2)
+Requires-Dist: bosdyn-api (==4.0.2)
 
 <!--
 Copyright (c) 2023 Boston Dynamics, Inc.  All rights reserved.
 
 Downloading, reproducing, distributing or otherwise using the SDK Software
 is subject to the terms and conditions of the Boston Dynamics Software
 Development Kit License (20191101-BDSDK-SL).
```

## Comparing `bosdyn_mission-4.0.1.dist-info/RECORD` & `bosdyn_mission-4.0.2.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -2,11 +2,11 @@
 bosdyn/mission/__init__.py,sha256=_BpC0ZVGQ5yH5S8rt_DrTMQkAuxzTn5YlPvwDzeFXdQ,483
 bosdyn/mission/client.py,sha256=_jjFZ1FCDNaKKcJ0pzHZ6suADTKcaaXHqp0GV5691M8,22437
 bosdyn/mission/constants.py,sha256=oSsl0XR1-fNzHASGNqs541YEO8qi64eewvbY9ICKaxE,435
 bosdyn/mission/exceptions.py,sha256=UqGT0XK3zA6Bgwo_7KNC44yi_MvW9h3c8_pHKML8ELQ,3941
 bosdyn/mission/remote_client.py,sha256=quGWyqLzpASgrR6MlnEPoRFCmnTMSBZ6tmr-Wyy9YW0,12190
 bosdyn/mission/server_util.py,sha256=_ts77W8yGq9BXhgOWwtMCXaxDjUxoorEPk1-YooEUNA,1508
 bosdyn/mission/util.py,sha256=30_LIam0ve6JTXZfXmZyza0Vey1FC3LHln81rUeAm_w,15616
-bosdyn_mission-4.0.1.dist-info/METADATA,sha256=foyspudk4oRuRkFkE5T6MklXqahIP4E2_c9GTSx48Wo,1760
-bosdyn_mission-4.0.1.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-bosdyn_mission-4.0.1.dist-info/top_level.txt,sha256=an2OWgx1ej2jFjmBjPWNQ68ZglvUfKhmXWW-WhTtDmA,7
-bosdyn_mission-4.0.1.dist-info/RECORD,,
+bosdyn_mission-4.0.2.dist-info/METADATA,sha256=jkozFK0zIcH1ObqTtwhwqv_ZHrh-eH1ZYa85vdhSglU,1760
+bosdyn_mission-4.0.2.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+bosdyn_mission-4.0.2.dist-info/top_level.txt,sha256=an2OWgx1ej2jFjmBjPWNQ68ZglvUfKhmXWW-WhTtDmA,7
+bosdyn_mission-4.0.2.dist-info/RECORD,,
```

