# Comparing `tmp/bosdyn_scout-4.0.1-py3-none-any.whl.zip` & `tmp/bosdyn_scout-4.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 10802 bytes, number of entries: 9
--rw-r--r--  2.0 unx      330 b- defN 24-Apr-12 01:43 bosdyn/__init__.py
--rw-r--r--  2.0 unx      265 b- defN 24-Apr-12 01:43 bosdyn/scout/__init__.py
--rw-r--r--  2.0 unx    42751 b- defN 24-Apr-12 01:43 bosdyn/scout/client.py
--rw-r--r--  2.0 unx      518 b- defN 24-Apr-12 01:43 bosdyn/scout/exceptions.py
--rw-r--r--  2.0 unx    12283 b- defN 24-Apr-12 01:43 bosdyn/scout/utils.py
--rw-r--r--  2.0 unx     1932 b- defN 24-Apr-12 01:44 bosdyn_scout-4.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-12 01:44 bosdyn_scout-4.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-Apr-12 01:44 bosdyn_scout-4.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      712 b- defN 24-Apr-12 01:44 bosdyn_scout-4.0.1.dist-info/RECORD
-9 files, 58890 bytes uncompressed, 9578 bytes compressed:  83.7%
+Zip file size: 10791 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      330 b- defN 24-May-28 15:21 bosdyn/__init__.py
+-rw-r--r--  2.0 unx      265 b- defN 24-May-28 15:21 bosdyn/scout/__init__.py
+-rw-r--r--  2.0 unx    42724 b- defN 24-May-28 15:21 bosdyn/scout/client.py
+-rw-r--r--  2.0 unx      518 b- defN 24-May-28 15:21 bosdyn/scout/exceptions.py
+-rw-r--r--  2.0 unx    12283 b- defN 24-May-28 15:21 bosdyn/scout/utils.py
+-rw-r--r--  2.0 unx     1932 b- defN 24-May-28 15:22 bosdyn_scout-4.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-28 15:22 bosdyn_scout-4.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-May-28 15:22 bosdyn_scout-4.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      712 b- defN 24-May-28 15:22 bosdyn_scout-4.0.2.dist-info/RECORD
+9 files, 58863 bytes uncompressed, 9567 bytes compressed:  83.7%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: bosdyn/scout/exceptions.py
 Comment: 
 
 Filename: bosdyn/scout/utils.py
 Comment: 
 
-Filename: bosdyn_scout-4.0.1.dist-info/METADATA
+Filename: bosdyn_scout-4.0.2.dist-info/METADATA
 Comment: 
 
-Filename: bosdyn_scout-4.0.1.dist-info/WHEEL
+Filename: bosdyn_scout-4.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: bosdyn_scout-4.0.1.dist-info/top_level.txt
+Filename: bosdyn_scout-4.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: bosdyn_scout-4.0.1.dist-info/RECORD
+Filename: bosdyn_scout-4.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bosdyn/scout/client.py

```diff
@@ -3,16 +3,15 @@
 # Downloading, reproducing, distributing or otherwise using the SDK Software
 # is subject to the terms and conditions of the Boston Dynamics Software
 # Development Kit License (20191101-BDSDK-SL).
 
 """ Scout Client is a client for a single Scout instance. The client uses the Scout web API
     to send HTTPs requests to a number of REStful endpoints using the Requests library.
 """
-from collections.abc import Iterable
-from typing import Dict
+from typing import Dict, Iterable
 
 import requests
 from deprecated.sphinx import deprecated
 
 import bosdyn.scout.utils
 from bosdyn.scout.exceptions import UnauthenticatedScoutClientError
```

## Comparing `bosdyn_scout-4.0.1.dist-info/METADATA` & `bosdyn_scout-4.0.2.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bosdyn-scout
-Version: 4.0.1
+Version: 4.0.2
 Summary: Boston Dynamics API Scout Client
 Home-page: https://dev.bostondynamics.com/docs/scout/
 Author: Boston Dynamics
 Author-email: support@bostondynamics.com
 Project-URL: Documentation, https://dev.bostondynamics.com/docs/scout/
 Project-URL: Source, https://github.com/boston-dynamics/spot-sdk/
 Classifier: Programming Language :: Python :: 3.6
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: Deprecated (~=1.2.10)
-Requires-Dist: bosdyn-orbit (==4.0.1)
+Requires-Dist: bosdyn-orbit (==4.0.2)
 
 <!--
 Copyright (c) 2023 Boston Dynamics, Inc.  All rights reserved.
 
 Downloading, reproducing, distributing or otherwise using the SDK Software
 is subject to the terms and conditions of the Boston Dynamics Software
 Development Kit License (20191101-BDSDK-SL).
```

