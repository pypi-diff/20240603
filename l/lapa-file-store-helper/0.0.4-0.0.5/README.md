# Comparing `tmp/lapa_file_store_helper-0.0.4.tar.gz` & `tmp/lapa_file_store_helper-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lapa_file_store_helper-0.0.4.tar", last modified: Sun May  5 18:48:03 2024, max compression
+gzip compressed data, was "lapa_file_store_helper-0.0.5.tar", last modified: Mon Jun  3 15:24:25 2024, max compression
```

## Comparing `lapa_file_store_helper-0.0.4.tar` & `lapa_file_store_helper-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:48:03.795062 lapa_file_store_helper-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-05 18:48:03.795062 lapa_file_store_helper-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-05 18:47:55.000000 lapa_file_store_helper-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:48:03.795062 lapa_file_store_helper-0.0.4/lapa_file_store_helper/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-05 18:47:55.000000 lapa_file_store_helper-0.0.4/lapa_file_store_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-05 18:47:55.000000 lapa_file_store_helper-0.0.4/lapa_file_store_helper/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:48:03.795062 lapa_file_store_helper-0.0.4/lapa_file_store_helper/data/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-05 18:47:55.000000 lapa_file_store_helper-0.0.4/lapa_file_store_helper/data/config.ini
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-05 18:47:55.000000 lapa_file_store_helper-0.0.4/lapa_file_store_helper/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:48:03.795062 lapa_file_store_helper-0.0.4/lapa_file_store_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-05 18:48:03.000000 lapa_file_store_helper-0.0.4/lapa_file_store_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-05 18:48:03.000000 lapa_file_store_helper-0.0.4/lapa_file_store_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 18:48:03.000000 lapa_file_store_helper-0.0.4/lapa_file_store_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-05 18:48:03.000000 lapa_file_store_helper-0.0.4/lapa_file_store_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-05 18:48:03.000000 lapa_file_store_helper-0.0.4/lapa_file_store_helper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 18:48:03.795062 lapa_file_store_helper-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-05 18:47:55.000000 lapa_file_store_helper-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:24:25.549459 lapa_file_store_helper-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-06-03 15:24:25.549459 lapa_file_store_helper-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-06-03 15:24:01.000000 lapa_file_store_helper-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:24:25.549459 lapa_file_store_helper-0.0.5/lapa_file_store_helper/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-06-03 15:24:01.000000 lapa_file_store_helper-0.0.5/lapa_file_store_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-06-03 15:24:01.000000 lapa_file_store_helper-0.0.5/lapa_file_store_helper/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:24:25.549459 lapa_file_store_helper-0.0.5/lapa_file_store_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-06-03 15:24:25.000000 lapa_file_store_helper-0.0.5/lapa_file_store_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-06-03 15:24:25.000000 lapa_file_store_helper-0.0.5/lapa_file_store_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 15:24:25.000000 lapa_file_store_helper-0.0.5/lapa_file_store_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-06-03 15:24:25.000000 lapa_file_store_helper-0.0.5/lapa_file_store_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-03 15:24:25.000000 lapa_file_store_helper-0.0.5/lapa_file_store_helper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 15:24:25.549459 lapa_file_store_helper-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-06-03 15:24:01.000000 lapa_file_store_helper-0.0.5/setup.py
```

### Comparing `lapa_file_store_helper-0.0.4/lapa_file_store_helper/main.py` & `lapa_file_store_helper-0.0.5/lapa_file_store_helper/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 import os
 import urllib.parse
 from typing import BinaryIO
 
 import requests
 from kiss_headers import parse_it
 
-from lapa_file_store_helper.configuration import (
-    config_int_lapa_file_store_port,
-    config_str_lapa_file_store_ip,
-    config_str_lapa_file_store_protocol,
-)
-
 
 class LAPAFileStoreHelper:
-    def __init__(self):
+    def __init__(
+        self,
+        param_str_lapa_file_store_protocol: str = "http",
+        param_str_lapa_file_store_ip: str = "localhost",
+        param_int_lapa_file_store_port: int = 10100,
+    ):
         try:
             self.global_str_lapa_file_store_url_base = (
-                f"{config_str_lapa_file_store_protocol}://"
-                f"{config_str_lapa_file_store_ip}:{config_int_lapa_file_store_port}"
+                f"{param_str_lapa_file_store_protocol}://"
+                f"{param_str_lapa_file_store_ip}:{param_int_lapa_file_store_port}"
             )
         except Exception:
             raise
 
     def upload_file_using_file_path(
-            self,
-            file_path: str,
-            file_purpose: str | None = None,
-            system_relative_path: str = "others/misc",
+        self,
+        file_path: str,
+        file_purpose: str | None = None,
+        system_relative_path: str = "others/misc",
     ):
         try:
             endpoint = "upload_file"
             payload = {
                 "file_purpose": file_purpose,
                 "system_relative_pat": system_relative_path,
             }
@@ -45,18 +44,18 @@
                     return response.json()
                 else:
                     response.raise_for_status()
         except Exception:
             raise
 
     def upload_file_using_binary_io(
-            self,
-            file: BinaryIO,
-            file_purpose: str | None = None,
-            system_relative_path: str = "others/misc",
+        self,
+        file: BinaryIO,
+        file_purpose: str | None = None,
+        system_relative_path: str = "others/misc",
     ):
         try:
             endpoint = "upload_file"
             payload = {
                 "file_purpose": file_purpose,
                 "system_relative_path": system_relative_path,
             }
```

### Comparing `lapa_file_store_helper-0.0.4/lapa_file_store_helper.egg-info/PKG-INFO` & `lapa_file_store_helper-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lapa-file-store-helper
-Version: 0.0.4
+Name: lapa_file_store_helper
+Version: 0.0.5
 Summary: helper to access the file store layer for my personal server.
 Home-page: https://github.com/thepmsquare/lapa_file_store_helper
 Author: thePmSquare, Lav Sharma, Amish Palkar
 Author-email: thepmsquare@gmail.com, lavsharma2016@gmail.com, amishpalkar302001@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -24,24 +24,24 @@
 
 > pip install lapa_file_store_helper
 
 ## usage
 
 [reference python file](./example/example.py)
 
-## configs
-
-1. lapa_file_store_helper\data\config.ini
-
 ## env
 
 - python>=3.12.0
 
 ## changelog
 
+### v0.0.5
+
+- remove config and reconfigure variables to be as class parameters.
+
 ### v0.0.4
 
 - Added helper function for /delete_file api call.
 
 ### v0.0.3
 
 - Status code check and error raise.
```

### Comparing `lapa_file_store_helper-0.0.4/setup.py` & `lapa_file_store_helper-0.0.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,16 @@
 from setuptools import find_packages, setup
 
 package_name = "lapa_file_store_helper"
 
 setup(
     name=package_name,
-    version="0.0.4",
+    version="0.0.5",
     packages=find_packages(),
-    package_data={
-        package_name: ["data/*"],
-    },
-    install_requires=[
-        "requests>=2.31.0",
-        "kiss_headers>=2.4.3",
-        "lapa_commons>=0.0.1"
-    ],
+    install_requires=["requests>=2.31.0", "kiss_headers>=2.4.3"],
     author="thePmSquare, Lav Sharma, Amish Palkar",
     author_email="thepmsquare@gmail.com, lavsharma2016@gmail.com, amishpalkar302001@gmail.com",
     description="helper to access the file store layer for my personal server.",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     url=f"https://github.com/thepmsquare/{package_name}",
     classifiers=[
```

