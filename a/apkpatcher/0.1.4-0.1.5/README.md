# Comparing `tmp/apkpatcher-0.1.4.tar.gz` & `tmp/apkpatcher-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apkpatcher-0.1.4.tar", last modified: Thu May 30 07:52:33 2024, max compression
+gzip compressed data, was "apkpatcher-0.1.5.tar", last modified: Mon Jun  3 10:52:02 2024, max compression
```

## Comparing `apkpatcher-0.1.4.tar` & `apkpatcher-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 07:52:33.196462 apkpatcher-0.1.4/
--rw-rw-rw-   0 root         (0) root         (0)    18046 2024-05-30 07:52:06.000000 apkpatcher-0.1.4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      131 2024-05-30 07:52:06.000000 apkpatcher-0.1.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    23045 2024-05-30 07:52:33.196462 apkpatcher-0.1.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1581 2024-05-30 07:52:06.000000 apkpatcher-0.1.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1062 2024-05-30 07:52:06.000000 apkpatcher-0.1.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 07:52:33.196462 apkpatcher-0.1.4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 07:52:33.192462 apkpatcher-0.1.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 07:52:33.194462 apkpatcher-0.1.4/src/apkpatcher/
--rw-rw-rw-   0 root         (0) root         (0)    26590 2024-05-30 07:52:06.000000 apkpatcher-0.1.4/src/apkpatcher/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      155 2024-05-30 07:52:06.000000 apkpatcher-0.1.4/src/apkpatcher/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     3534 2024-05-30 07:52:06.000000 apkpatcher-0.1.4/src/apkpatcher/cli.py
--rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-30 07:52:06.000000 apkpatcher-0.1.4/src/apkpatcher/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 07:52:33.195462 apkpatcher-0.1.4/src/apkpatcher.egg-info/
--rw-r--r--   0 root         (0) root         (0)    23045 2024-05-30 07:52:33.000000 apkpatcher-0.1.4/src/apkpatcher.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      373 2024-05-30 07:52:33.000000 apkpatcher-0.1.4/src/apkpatcher.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 07:52:33.000000 apkpatcher-0.1.4/src/apkpatcher.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2024-05-30 07:52:33.000000 apkpatcher-0.1.4/src/apkpatcher.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       36 2024-05-30 07:52:33.000000 apkpatcher-0.1.4/src/apkpatcher.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-05-30 07:52:33.000000 apkpatcher-0.1.4/src/apkpatcher.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 10:52:02.300254 apkpatcher-0.1.5/
+-rw-rw-rw-   0 root         (0) root         (0)    18046 2024-06-03 10:51:45.000000 apkpatcher-0.1.5/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      131 2024-06-03 10:51:45.000000 apkpatcher-0.1.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    22994 2024-06-03 10:52:02.300254 apkpatcher-0.1.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1581 2024-06-03 10:51:45.000000 apkpatcher-0.1.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      969 2024-06-03 10:51:45.000000 apkpatcher-0.1.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-06-03 10:52:02.300254 apkpatcher-0.1.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 10:52:02.296254 apkpatcher-0.1.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 10:52:02.298254 apkpatcher-0.1.5/src/apkpatcher/
+-rw-rw-rw-   0 root         (0) root         (0)    26551 2024-06-03 10:51:45.000000 apkpatcher-0.1.5/src/apkpatcher/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      155 2024-06-03 10:51:45.000000 apkpatcher-0.1.5/src/apkpatcher/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3534 2024-06-03 10:51:45.000000 apkpatcher-0.1.5/src/apkpatcher/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-06-03 10:51:45.000000 apkpatcher-0.1.5/src/apkpatcher/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 10:52:02.299254 apkpatcher-0.1.5/src/apkpatcher.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    22994 2024-06-03 10:52:02.000000 apkpatcher-0.1.5/src/apkpatcher.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      373 2024-06-03 10:52:02.000000 apkpatcher-0.1.5/src/apkpatcher.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 10:52:02.000000 apkpatcher-0.1.5/src/apkpatcher.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2024-06-03 10:52:02.000000 apkpatcher-0.1.5/src/apkpatcher.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-06-03 10:52:02.000000 apkpatcher-0.1.5/src/apkpatcher.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-06-03 10:52:02.000000 apkpatcher-0.1.5/src/apkpatcher.egg-info/top_level.txt
```

### Comparing `apkpatcher-0.1.4/LICENSE` & `apkpatcher-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `apkpatcher-0.1.4/PKG-INFO` & `apkpatcher-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apkpatcher
-Version: 0.1.4
+Version: 0.1.5
 Summary: Tool use as library or in cli to patch an APK, inject some libraries inside the APK or add a custom certificate
 Author-email: "Benoit Forgette (MadSquirrel)" <benoit.forgette@ci-yow.com>
 Maintainer-email: "Benoit Forgette (MadSquirrel)" <benoit.forgette@ci-yow.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc., <http://fsf.org/>
@@ -347,17 +347,15 @@
 Project-URL: Homepage, https://ci-yow.com
 Project-URL: Repository, https://gitlab.com/MadSquirrels/mobile/apkpatcher
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: sty
-Requires-Dist: pyaxml==0.0.8
-Requires-Dist: androguard==4.1.1
+Requires-Dist: pyaxml==0.0.10
 
 # README
 
 
 ## GENERAL INFO
```

### Comparing `apkpatcher-0.1.4/README.md` & `apkpatcher-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `apkpatcher-0.1.4/pyproject.toml` & `apkpatcher-0.1.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "apkpatcher"
 dynamic = ["version", "readme"]
 dependencies = [
-  'sty',
-  'pyaxml==0.0.8',
-  'androguard==4.1.1',
+  'pyaxml==0.0.10',
 ]
 requires-python = ">=3.5"
 authors = [
   {name = "Benoit Forgette (MadSquirrel)", email = "benoit.forgette@ci-yow.com"},
 ]
 maintainers = [
   {name = "Benoit Forgette (MadSquirrel)", email = "benoit.forgette@ci-yow.com"},
@@ -24,16 +22,14 @@
   "Development Status :: 4 - Beta",
   "Programming Language :: Python"
 ]
 
 [project.entry-points.console_scripts]
 apkpatcher = "apkpatcher.cli:main"
 
-#[project.scripts]
-#apkpatcher = "apkpatcher=apkpatcher:main"
 
 
 [tool.setuptools.dynamic]
 version = {attr = "apkpatcher.conf.VERSION"}
 readme = {file = ["README.md"]}
 
 [project.urls]
```

### Comparing `apkpatcher-0.1.4/src/apkpatcher/__init__.py` & `apkpatcher-0.1.5/src/apkpatcher/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 import os
 import sys
-import json
 import time
-import signal
 import shutil
 import os.path
-import argparse
 import tempfile
 import subprocess
 import logging
 from pathlib import Path
 
-from androguard.core import axml
 from . import conf
 import pyaxml
 import xml.etree.ElementTree as ET
 import lxml
 
 def plba(filename, arch):
     p = Path(filename)
@@ -160,20 +156,20 @@
                 path_network = "res/network_security_config.xml"
                 ID = rsc.add_id_public(rsc.get_packages()[0],"xml", "network_security_config", path_network)
             else:
                 ID, path_network = ID
                 path_network = pyaxml.StringBlocks(proto=rsc.proto.stringblocks).decode_str(path_network)
 
             
-            aml = axml.AXMLPrinter(buf)
-            etree = aml.root
-            application = etree.findall("./application")[0]
+            axml, _ = pyaxml.AXML.from_axml(buf)
+            xml = axml.to_xml()
+            application = xml.findall("./application")[0]
             application.attrib["{http://schemas.android.com/apk/res/android}networkSecurityConfig"] = f"@{hex(ID)[2:]}"
             res_aml = pyaxml.axml.AXML()
-            res_aml.from_xml(etree)
+            res_aml.from_xml(xml)
 
             with open(manifest_path, 'wb') as fp:
                 fp.write(res_aml.pack())
     
             logging.info('The Network Security label was added!')
 
         return path_network
@@ -228,16 +224,16 @@
             logging.error("Couldn't find the Manifest file. Something is wrong with the apk!")
             return False
 
 
         with open(manifest_path, 'rb') as fp:
             buf = fp.read()
 
-            aml = axml.AXMLPrinter(buf)
-            etree = aml.root
+            axml, _ = pyaxml.AXML.from_axml(buf)
+            etree = axml.to_xml()
             res_aml = None
             for i in range(len(etree)):
                 if etree[i].tag == 'application' or etree[i].tag == 'uses-permission':
                     newperm = lxml.etree.Element('uses-permission')
                     newperm.attrib['{http://schemas.android.com/apk/res/android}name'] = permission
                     etree.insert(i, newperm)
                     res_aml = pyaxml.axml.AXML()
@@ -553,16 +549,16 @@
 
         if not os.path.isfile(manifest_path):
             logging.error("Couldn't find the Manifest file. Something is wrong with the apk!")
             return False
 
 
         with open(manifest_path, 'rb') as fp:
-            aml = axml.AXMLPrinter(fp.read())
-            etree = aml.root
+            axml, _ = pyaxml.AXML.from_axml(fp.read())
+            etree = axml.to_xml()
             extractNative = etree.findall("./application/[@{http://schemas.android.com/apk/res/android}extractNativeLibs='false']")
             if len(extractNative) > 0:
                 extractNative[0].attrib['{http://schemas.android.com/apk/res/android}extractNativeLibs'] = 'true'
 
         with open(manifest_path, 'wb') as fp:
             res_aml = pyaxml.axml.AXML()
             res_aml.from_xml(etree)
```

### Comparing `apkpatcher-0.1.4/src/apkpatcher/cli.py` & `apkpatcher-0.1.5/src/apkpatcher/cli.py`

 * *Files identical despite different names*

### Comparing `apkpatcher-0.1.4/src/apkpatcher.egg-info/PKG-INFO` & `apkpatcher-0.1.5/src/apkpatcher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apkpatcher
-Version: 0.1.4
+Version: 0.1.5
 Summary: Tool use as library or in cli to patch an APK, inject some libraries inside the APK or add a custom certificate
 Author-email: "Benoit Forgette (MadSquirrel)" <benoit.forgette@ci-yow.com>
 Maintainer-email: "Benoit Forgette (MadSquirrel)" <benoit.forgette@ci-yow.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc., <http://fsf.org/>
@@ -347,17 +347,15 @@
 Project-URL: Homepage, https://ci-yow.com
 Project-URL: Repository, https://gitlab.com/MadSquirrels/mobile/apkpatcher
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: sty
-Requires-Dist: pyaxml==0.0.8
-Requires-Dist: androguard==4.1.1
+Requires-Dist: pyaxml==0.0.10
 
 # README
 
 
 ## GENERAL INFO
```

