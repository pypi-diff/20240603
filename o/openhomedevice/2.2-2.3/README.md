# Comparing `tmp/openhomedevice-2.2.tar.gz` & `tmp/openhomedevice-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openhomedevice-2.2.tar", last modified: Tue Jun 27 19:27:26 2023, max compression
+gzip compressed data, was "openhomedevice-2.3.tar", last modified: Sun Jun  2 22:17:49 2024, max compression
```

## Comparing `openhomedevice-2.2.tar` & `openhomedevice-2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 barry      (502) staff       (20)        0 2023-06-27 19:27:26.756592 openhomedevice-2.2/
--rw-r--r--   0 barry      (502) staff       (20)     1076 2023-06-12 20:59:11.000000 openhomedevice-2.2/LICENSE.txt
--rw-r--r--   0 barry      (502) staff       (20)     7238 2023-06-27 19:27:26.756750 openhomedevice-2.2/PKG-INFO
--rw-r--r--   0 barry      (502) staff       (20)     6590 2023-06-27 19:20:23.000000 openhomedevice-2.2/README.md
-drwxr-xr-x   0 barry      (502) staff       (20)        0 2023-06-27 19:27:26.753014 openhomedevice-2.2/openhomedevice/
--rw-r--r--   0 barry      (502) staff       (20)       43 2023-06-12 20:59:11.000000 openhomedevice-2.2/openhomedevice/__init__.py
--rw-r--r--   0 barry      (502) staff       (20)    10536 2023-06-27 19:26:31.000000 openhomedevice-2.2/openhomedevice/device.py
--rw-r--r--   0 barry      (502) staff       (20)     6482 2023-06-12 20:59:11.000000 openhomedevice-2.2/openhomedevice/didl_lite.py
-drwxr-xr-x   0 barry      (502) staff       (20)        0 2023-06-27 19:27:26.756093 openhomedevice-2.2/openhomedevice.egg-info/
--rw-r--r--   0 barry      (502) staff       (20)     7238 2023-06-27 19:27:26.000000 openhomedevice-2.2/openhomedevice.egg-info/PKG-INFO
--rw-r--r--   0 barry      (502) staff       (20)      309 2023-06-27 19:27:26.000000 openhomedevice-2.2/openhomedevice.egg-info/SOURCES.txt
--rw-r--r--   0 barry      (502) staff       (20)        1 2023-06-27 19:27:26.000000 openhomedevice-2.2/openhomedevice.egg-info/dependency_links.txt
--rw-r--r--   0 barry      (502) staff       (20)       36 2023-06-27 19:27:26.000000 openhomedevice-2.2/openhomedevice.egg-info/requires.txt
--rw-r--r--   0 barry      (502) staff       (20)       15 2023-06-27 19:27:26.000000 openhomedevice-2.2/openhomedevice.egg-info/top_level.txt
--rw-r--r--   0 barry      (502) staff       (20)       79 2023-06-27 19:27:26.757273 openhomedevice-2.2/setup.cfg
--rw-r--r--   0 barry      (502) staff       (20)      914 2023-06-27 19:21:27.000000 openhomedevice-2.2/setup.py
+drwxr-xr-x   0 barry      (502) staff       (20)        0 2024-06-02 22:17:49.790745 openhomedevice-2.3/
+-rw-r--r--   0 barry      (502) staff       (20)     1076 2024-06-02 21:52:46.000000 openhomedevice-2.3/LICENSE.txt
+-rw-r--r--   0 barry      (502) staff       (20)     7201 2024-06-02 22:17:49.790977 openhomedevice-2.3/PKG-INFO
+-rw-r--r--   0 barry      (502) staff       (20)     6590 2024-06-02 21:52:46.000000 openhomedevice-2.3/README.md
+drwxr-xr-x   0 barry      (502) staff       (20)        0 2024-06-02 22:17:49.786125 openhomedevice-2.3/openhomedevice/
+-rw-r--r--   0 barry      (502) staff       (20)       43 2024-06-02 21:52:46.000000 openhomedevice-2.3/openhomedevice/__init__.py
+-rw-r--r--   0 barry      (502) staff       (20)    10536 2024-06-02 21:52:46.000000 openhomedevice-2.3/openhomedevice/device.py
+-rw-r--r--   0 barry      (502) staff       (20)     6404 2024-06-02 22:10:26.000000 openhomedevice-2.3/openhomedevice/didl_lite.py
+drwxr-xr-x   0 barry      (502) staff       (20)        0 2024-06-02 22:17:49.790137 openhomedevice-2.3/openhomedevice.egg-info/
+-rw-r--r--   0 barry      (502) staff       (20)     7201 2024-06-02 22:17:49.000000 openhomedevice-2.3/openhomedevice.egg-info/PKG-INFO
+-rw-r--r--   0 barry      (502) staff       (20)      309 2024-06-02 22:17:49.000000 openhomedevice-2.3/openhomedevice.egg-info/SOURCES.txt
+-rw-r--r--   0 barry      (502) staff       (20)        1 2024-06-02 22:17:49.000000 openhomedevice-2.3/openhomedevice.egg-info/dependency_links.txt
+-rw-r--r--   0 barry      (502) staff       (20)       36 2024-06-02 22:17:49.000000 openhomedevice-2.3/openhomedevice.egg-info/requires.txt
+-rw-r--r--   0 barry      (502) staff       (20)       15 2024-06-02 22:17:49.000000 openhomedevice-2.3/openhomedevice.egg-info/top_level.txt
+-rw-r--r--   0 barry      (502) staff       (20)       79 2024-06-02 22:17:49.791626 openhomedevice-2.3/setup.cfg
+-rw-r--r--   0 barry      (502) staff       (20)      914 2024-06-02 22:17:17.000000 openhomedevice-2.3/setup.py
```

### Comparing `openhomedevice-2.2/LICENSE.txt` & `openhomedevice-2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openhomedevice-2.2/PKG-INFO` & `openhomedevice-2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: openhomedevice
-Version: 2.2
+Version: 2.3
 Summary: Provides an API for requesting information from an Openhome device
 Home-page: https://github.com/bazwilliams/openhomedevice
+Download-URL: https://github.com/bazwilliams/openhomedevice/tarball/2.1
 Author: Barry John Williams
 Author-email: barry@bjw.me.uk
-License: UNKNOWN
-Download-URL: https://github.com/bazwilliams/openhomedevice/tarball/2.1
 Keywords: upnp,dlna,openhome,linn,ds,music,render,async
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -251,9 +249,7 @@
 
 Update version in `setup.py`
 
 ```sh
 python3 setup.py sdist
 twine upload dist/*
 ```
-
-
```

### Comparing `openhomedevice-2.2/README.md` & `openhomedevice-2.3/README.md`

 * *Files identical despite different names*

### Comparing `openhomedevice-2.2/openhomedevice/device.py` & `openhomedevice-2.3/openhomedevice/device.py`

 * *Files identical despite different names*

### Comparing `openhomedevice-2.2/openhomedevice/didl_lite.py` & `openhomedevice-2.3/openhomedevice/didl_lite.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 import re
 
 import xml.etree.ElementTree as etree
 
 
-def escape(str):
-    str = str.replace("&", "&amp;")
-    return str
-
-
 def generate_string(track_details):
     title = track_details.get("title", "") or ""
     uri = track_details.get("uri", "") or ""
     albumArtwork = track_details.get("albumArtwork", "") or ""
 
     return (
         '<DIDL-Lite xmlns:dc="http://purl.org/dc/elements/1.1/" '
@@ -30,15 +25,15 @@
 def parse(metadata):
     track_details = {}
 
     if metadata is None:
         return track_details
 
     try:
-        et = etree.fromstring(escape(metadata)).find(
+        et = etree.fromstring(metadata).find(
             "DIDL-Lite:item",
             {"DIDL-Lite": "urn:schemas-upnp-org:metadata-1-0/DIDL-Lite/"},
         )
     except:
         return track_details
 
     if et is None:
```

### Comparing `openhomedevice-2.2/openhomedevice.egg-info/PKG-INFO` & `openhomedevice-2.3/openhomedevice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: openhomedevice
-Version: 2.2
+Version: 2.3
 Summary: Provides an API for requesting information from an Openhome device
 Home-page: https://github.com/bazwilliams/openhomedevice
+Download-URL: https://github.com/bazwilliams/openhomedevice/tarball/2.1
 Author: Barry John Williams
 Author-email: barry@bjw.me.uk
-License: UNKNOWN
-Download-URL: https://github.com/bazwilliams/openhomedevice/tarball/2.1
 Keywords: upnp,dlna,openhome,linn,ds,music,render,async
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -251,9 +249,7 @@
 
 Update version in `setup.py`
 
 ```sh
 python3 setup.py sdist
 twine upload dist/*
 ```
-
-
```

### Comparing `openhomedevice-2.2/setup.py` & `openhomedevice-2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
   name = 'openhomedevice',
-  version = '2.2',
+  version = '2.3',
   author = 'Barry John Williams',
   author_email = 'barry@bjw.me.uk',
   description='Provides an API for requesting information from an Openhome device',
   long_description=long_description,
   long_description_content_type="text/markdown",
   url='https://github.com/bazwilliams/openhomedevice',
   packages=setuptools.find_packages(),
```

