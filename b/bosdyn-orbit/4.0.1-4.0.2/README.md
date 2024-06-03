# Comparing `tmp/bosdyn_orbit-4.0.1-py3-none-any.whl.zip` & `tmp/bosdyn_orbit-4.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 11228 bytes, number of entries: 9
--rw-r--r--  2.0 unx      330 b- defN 24-Apr-12 01:43 bosdyn/__init__.py
--rw-r--r--  2.0 unx      266 b- defN 24-Apr-12 01:43 bosdyn/orbit/__init__.py
--rw-r--r--  2.0 unx    40158 b- defN 24-Apr-12 01:43 bosdyn/orbit/client.py
--rw-r--r--  2.0 unx      711 b- defN 24-Apr-12 01:43 bosdyn/orbit/exceptions.py
--rw-r--r--  2.0 unx    13666 b- defN 24-Apr-12 01:43 bosdyn/orbit/utils.py
--rw-r--r--  2.0 unx     1894 b- defN 24-Apr-12 01:44 bosdyn_orbit-4.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-12 01:44 bosdyn_orbit-4.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-Apr-12 01:44 bosdyn_orbit-4.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      712 b- defN 24-Apr-12 01:44 bosdyn_orbit-4.0.1.dist-info/RECORD
-9 files, 57836 bytes uncompressed, 10004 bytes compressed:  82.7%
+Zip file size: 11218 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      330 b- defN 24-May-28 15:21 bosdyn/__init__.py
+-rw-r--r--  2.0 unx      266 b- defN 24-May-28 15:21 bosdyn/orbit/__init__.py
+-rw-r--r--  2.0 unx    40131 b- defN 24-May-28 15:21 bosdyn/orbit/client.py
+-rw-r--r--  2.0 unx      711 b- defN 24-May-28 15:21 bosdyn/orbit/exceptions.py
+-rw-r--r--  2.0 unx    13666 b- defN 24-May-28 15:21 bosdyn/orbit/utils.py
+-rw-r--r--  2.0 unx     1894 b- defN 24-May-28 15:22 bosdyn_orbit-4.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-28 15:22 bosdyn_orbit-4.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-May-28 15:22 bosdyn_orbit-4.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      712 b- defN 24-May-28 15:22 bosdyn_orbit-4.0.2.dist-info/RECORD
+9 files, 57809 bytes uncompressed, 9994 bytes compressed:  82.7%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: bosdyn/orbit/exceptions.py
 Comment: 
 
 Filename: bosdyn/orbit/utils.py
 Comment: 
 
-Filename: bosdyn_orbit-4.0.1.dist-info/METADATA
+Filename: bosdyn_orbit-4.0.2.dist-info/METADATA
 Comment: 
 
-Filename: bosdyn_orbit-4.0.1.dist-info/WHEEL
+Filename: bosdyn_orbit-4.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: bosdyn_orbit-4.0.1.dist-info/top_level.txt
+Filename: bosdyn_orbit-4.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: bosdyn_orbit-4.0.1.dist-info/RECORD
+Filename: bosdyn_orbit-4.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bosdyn/orbit/client.py

```diff
@@ -2,16 +2,15 @@
 #
 # Downloading, reproducing, distributing or otherwise using the SDK Software
 # is subject to the terms and conditions of the Boston Dynamics Software
 # Development Kit License (20191101-BDSDK-SL).
 
 """ The client uses a web API to send HTTPs requests to a number of REStful endpoints using the Requests library.
 """
-from collections.abc import Iterable
-from typing import Dict
+from typing import Dict, Iterable
 
 import requests
 
 import bosdyn.orbit.utils as utils
 from bosdyn.orbit.exceptions import UnauthenticatedClientError
 
 DEFAULT_HEADERS = {'Accept': 'application/json'}
```

## Comparing `bosdyn_orbit-4.0.1.dist-info/METADATA` & `bosdyn_orbit-4.0.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bosdyn-orbit
-Version: 4.0.1
+Version: 4.0.2
 Summary: Boston Dynamics API Orbit Client
 Home-page: https://dev.bostondynamics.com/docs/orbit/
 Author: Boston Dynamics
 Author-email: support@bostondynamics.com
 Project-URL: Documentation, https://dev.bostondynamics.com/docs/orbit/
 Project-URL: Source, https://github.com/boston-dynamics/spot-sdk/
 Classifier: Programming Language :: Python :: 3.6
```

## Comparing `bosdyn_orbit-4.0.1.dist-info/RECORD` & `bosdyn_orbit-4.0.2.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 bosdyn/__init__.py,sha256=CMQioQKK1NlMk3kZuY49b_Aw-JyvDeOtuqOCAul1I0s,330
 bosdyn/orbit/__init__.py,sha256=L_VSEXjtWZNHVHs3Jdr_TF2pJ2ju2yysAi0-YZsbJoU,266
-bosdyn/orbit/client.py,sha256=Xdt2FgY-Oo-cpMOf-tAGw9kA1n7eVVOMVOxuubvFhAw,40158
+bosdyn/orbit/client.py,sha256=7WoQodp9bgIiyB2o7bmqd9snj6ny5rfYPnUJuj0B-qA,40131
 bosdyn/orbit/exceptions.py,sha256=eaeHSlGh27JlZUEjcpLKxR1CNdW6Twp4e685pUgEjyQ,711
 bosdyn/orbit/utils.py,sha256=i9nEEpdceD3HecLQKw7jQGQ5qR7bNWwMrcsxVpt4TJ4,13666
-bosdyn_orbit-4.0.1.dist-info/METADATA,sha256=gcp7BUE6R0nw2CV9tMTHtN8TLLUiKCLr2jCTRdHE3qA,1894
-bosdyn_orbit-4.0.1.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-bosdyn_orbit-4.0.1.dist-info/top_level.txt,sha256=an2OWgx1ej2jFjmBjPWNQ68ZglvUfKhmXWW-WhTtDmA,7
-bosdyn_orbit-4.0.1.dist-info/RECORD,,
+bosdyn_orbit-4.0.2.dist-info/METADATA,sha256=D67foMlISF1YFDIArtpTRv6uwRF4KD0a-jlPWQ8N7PU,1894
+bosdyn_orbit-4.0.2.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+bosdyn_orbit-4.0.2.dist-info/top_level.txt,sha256=an2OWgx1ej2jFjmBjPWNQ68ZglvUfKhmXWW-WhTtDmA,7
+bosdyn_orbit-4.0.2.dist-info/RECORD,,
```

