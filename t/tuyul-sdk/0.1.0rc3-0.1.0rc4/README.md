# Comparing `tmp/tuyul_sdk-0.1.0rc3.tar.gz` & `tmp/tuyul_sdk-0.1.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuyul_sdk-0.1.0rc3.tar", max compression
+gzip compressed data, was "tuyul_sdk-0.1.0rc4.tar", max compression
```

## Comparing `tuyul_sdk-0.1.0rc3.tar` & `tuyul_sdk-0.1.0rc4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      628 2024-06-02 09:16:58.553243 tuyul_sdk-0.1.0rc3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-31 02:26:37.717294 tuyul_sdk-0.1.0rc3/README.md
--rw-r--r--   0        0        0      125 2024-05-31 03:57:46.818106 tuyul_sdk-0.1.0rc3/tuyul_sdk/__init__.py
--rw-r--r--   0        0        0      303 2024-05-31 03:14:55.963434 tuyul_sdk-0.1.0rc3/tuyul_sdk/_Cipher/__init__.py
--rw-r--r--   0        0        0     6029 2024-05-31 05:48:34.784524 tuyul_sdk-0.1.0rc3/tuyul_sdk/_Cipher/AES.py
--rw-r--r--   0        0        0     1559 2024-05-31 02:38:39.120584 tuyul_sdk-0.1.0rc3/tuyul_sdk/_Cipher/Password.py
--rw-r--r--   0        0        0      526 2024-05-31 05:51:39.453523 tuyul_sdk-0.1.0rc3/tuyul_sdk/_Cipher/Salt.py
--rw-r--r--   0        0        0      101 2024-05-31 03:28:50.075893 tuyul_sdk-0.1.0rc3/tuyul_sdk/_Connection/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 20:21:44.103798 tuyul_sdk-0.1.0rc3/tuyul_sdk/_Connection/_certificate/__init__.py
--rw-r--r--   0        0        0   286252 2024-03-18 20:21:44.105798 tuyul_sdk-0.1.0rc3/tuyul_sdk/_Connection/_certificate/cacert.pem
--rw-r--r--   0        0        0     1581 2024-05-31 03:28:19.129050 tuyul_sdk-0.1.0rc3/tuyul_sdk/_Connection/httpx.py
--rw-r--r--   0        0        0     1294 2024-05-31 03:28:24.109127 tuyul_sdk-0.1.0rc3/tuyul_sdk/_Connection/requests.py
--rw-r--r--   0        0        0     4286 2024-05-31 03:18:09.960902 tuyul_sdk-0.1.0rc3/tuyul_sdk/_Connection/utils.py
--rw-r--r--   0        0        0     2795 2024-06-02 07:24:30.149304 tuyul_sdk-0.1.0rc3/tuyul_sdk/_Database.py
--rw-r--r--   0        0        0     2386 2024-06-02 09:16:41.682027 tuyul_sdk-0.1.0rc3/tuyul_sdk/_Gmail/__init__.py
--rw-r--r--   0        0        0     2893 2024-06-02 08:39:07.245267 tuyul_sdk-0.1.0rc3/tuyul_sdk/_Gmail/Utils.py
--rw-r--r--   0        0        0       93 2024-05-30 02:34:28.449126 tuyul_sdk-0.1.0rc3/tuyul_sdk/sql.py
--rw-r--r--   0        0        0      366 2024-05-31 03:59:01.720591 tuyul_sdk-0.1.0rc3/tuyul_sdk/Utils/__init__.py
--rw-r--r--   0        0        0      454 2024-03-30 18:29:45.577779 tuyul_sdk-0.1.0rc3/tuyul_sdk/Utils/_Color.py
--rw-r--r--   0        0        0     3669 2024-05-31 02:45:00.849778 tuyul_sdk-0.1.0rc3/tuyul_sdk/Utils/_hexbytes.py
--rw-r--r--   0        0        0      509 2024-03-18 20:21:43.622544 tuyul_sdk-0.1.0rc3/tuyul_sdk/Utils/_input.py
--rw-r--r--   0        0        0      719 2024-03-18 20:21:43.623543 tuyul_sdk-0.1.0rc3/tuyul_sdk/Utils/_Line.py
--rw-r--r--   0        0        0      826 2024-05-26 07:36:03.091067 tuyul_sdk-0.1.0rc3/tuyul_sdk/Utils/_Log.py
--rw-r--r--   0        0        0     2373 2024-05-26 07:35:32.143357 tuyul_sdk-0.1.0rc3/tuyul_sdk/Utils/_Progress.py
--rw-r--r--   0        0        0      229 2024-05-26 07:33:25.053372 tuyul_sdk-0.1.0rc3/tuyul_sdk/Utils/_Reset.py
--rw-r--r--   0        0        0     3000 2024-05-26 07:32:31.114228 tuyul_sdk-0.1.0rc3/tuyul_sdk/Utils/_UserAgent.py
--rw-r--r--   0        0        0      974 1970-01-01 00:00:00.000000 tuyul_sdk-0.1.0rc3/setup.py
--rw-r--r--   0        0        0      872 1970-01-01 00:00:00.000000 tuyul_sdk-0.1.0rc3/PKG-INFO
+-rw-r--r--   0        0        0      628 2024-06-02 09:18:37.841138 tuyul_sdk-0.1.0rc4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-31 02:26:37.717294 tuyul_sdk-0.1.0rc4/README.md
+-rw-r--r--   0        0        0      148 2024-06-02 09:18:26.530522 tuyul_sdk-0.1.0rc4/tuyul_sdk/__init__.py
+-rw-r--r--   0        0        0      303 2024-05-31 03:14:55.963434 tuyul_sdk-0.1.0rc4/tuyul_sdk/_Cipher/__init__.py
+-rw-r--r--   0        0        0     6029 2024-05-31 05:48:34.784524 tuyul_sdk-0.1.0rc4/tuyul_sdk/_Cipher/AES.py
+-rw-r--r--   0        0        0     1559 2024-05-31 02:38:39.120584 tuyul_sdk-0.1.0rc4/tuyul_sdk/_Cipher/Password.py
+-rw-r--r--   0        0        0      526 2024-05-31 05:51:39.453523 tuyul_sdk-0.1.0rc4/tuyul_sdk/_Cipher/Salt.py
+-rw-r--r--   0        0        0      101 2024-05-31 03:28:50.075893 tuyul_sdk-0.1.0rc4/tuyul_sdk/_Connection/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-18 20:21:44.103798 tuyul_sdk-0.1.0rc4/tuyul_sdk/_Connection/_certificate/__init__.py
+-rw-r--r--   0        0        0   286252 2024-03-18 20:21:44.105798 tuyul_sdk-0.1.0rc4/tuyul_sdk/_Connection/_certificate/cacert.pem
+-rw-r--r--   0        0        0     1581 2024-05-31 03:28:19.129050 tuyul_sdk-0.1.0rc4/tuyul_sdk/_Connection/httpx.py
+-rw-r--r--   0        0        0     1294 2024-05-31 03:28:24.109127 tuyul_sdk-0.1.0rc4/tuyul_sdk/_Connection/requests.py
+-rw-r--r--   0        0        0     4286 2024-05-31 03:18:09.960902 tuyul_sdk-0.1.0rc4/tuyul_sdk/_Connection/utils.py
+-rw-r--r--   0        0        0     2795 2024-06-02 07:24:30.149304 tuyul_sdk-0.1.0rc4/tuyul_sdk/_Database.py
+-rw-r--r--   0        0        0     2318 2024-06-02 09:18:23.153633 tuyul_sdk-0.1.0rc4/tuyul_sdk/_Gmail/__init__.py
+-rw-r--r--   0        0        0     2893 2024-06-02 08:39:07.245267 tuyul_sdk-0.1.0rc4/tuyul_sdk/_Gmail/Utils.py
+-rw-r--r--   0        0        0       93 2024-05-30 02:34:28.449126 tuyul_sdk-0.1.0rc4/tuyul_sdk/sql.py
+-rw-r--r--   0        0        0      366 2024-05-31 03:59:01.720591 tuyul_sdk-0.1.0rc4/tuyul_sdk/Utils/__init__.py
+-rw-r--r--   0        0        0      454 2024-03-30 18:29:45.577779 tuyul_sdk-0.1.0rc4/tuyul_sdk/Utils/_Color.py
+-rw-r--r--   0        0        0     3669 2024-05-31 02:45:00.849778 tuyul_sdk-0.1.0rc4/tuyul_sdk/Utils/_hexbytes.py
+-rw-r--r--   0        0        0      509 2024-03-18 20:21:43.622544 tuyul_sdk-0.1.0rc4/tuyul_sdk/Utils/_input.py
+-rw-r--r--   0        0        0      719 2024-03-18 20:21:43.623543 tuyul_sdk-0.1.0rc4/tuyul_sdk/Utils/_Line.py
+-rw-r--r--   0        0        0      826 2024-05-26 07:36:03.091067 tuyul_sdk-0.1.0rc4/tuyul_sdk/Utils/_Log.py
+-rw-r--r--   0        0        0     2373 2024-05-26 07:35:32.143357 tuyul_sdk-0.1.0rc4/tuyul_sdk/Utils/_Progress.py
+-rw-r--r--   0        0        0      229 2024-05-26 07:33:25.053372 tuyul_sdk-0.1.0rc4/tuyul_sdk/Utils/_Reset.py
+-rw-r--r--   0        0        0     3000 2024-05-26 07:32:31.114228 tuyul_sdk-0.1.0rc4/tuyul_sdk/Utils/_UserAgent.py
+-rw-r--r--   0        0        0      974 1970-01-01 00:00:00.000000 tuyul_sdk-0.1.0rc4/setup.py
+-rw-r--r--   0        0        0      872 1970-01-01 00:00:00.000000 tuyul_sdk-0.1.0rc4/PKG-INFO
```

### Comparing `tuyul_sdk-0.1.0rc3/pyproject.toml` & `tuyul_sdk-0.1.0rc4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tuyul-sdk"
-version = "0.1.0rc3"
+version = "0.1.0rc4"
 description = ""
 authors = ["DesKaOne <DesKaOne@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "tuyul_sdk"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `tuyul_sdk-0.1.0rc3/tuyul_sdk/_Cipher/AES.py` & `tuyul_sdk-0.1.0rc4/tuyul_sdk/_Cipher/AES.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.1.0rc3/tuyul_sdk/_Cipher/Password.py` & `tuyul_sdk-0.1.0rc4/tuyul_sdk/_Cipher/Password.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.1.0rc3/tuyul_sdk/_Cipher/Salt.py` & `tuyul_sdk-0.1.0rc4/tuyul_sdk/_Cipher/Salt.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.1.0rc3/tuyul_sdk/_Connection/_certificate/cacert.pem` & `tuyul_sdk-0.1.0rc4/tuyul_sdk/_Connection/_certificate/cacert.pem`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.1.0rc3/tuyul_sdk/_Connection/httpx.py` & `tuyul_sdk-0.1.0rc4/tuyul_sdk/_Connection/httpx.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.1.0rc3/tuyul_sdk/_Connection/requests.py` & `tuyul_sdk-0.1.0rc4/tuyul_sdk/_Connection/requests.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.1.0rc3/tuyul_sdk/_Connection/utils.py` & `tuyul_sdk-0.1.0rc4/tuyul_sdk/_Connection/utils.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.1.0rc3/tuyul_sdk/_Database.py` & `tuyul_sdk-0.1.0rc4/tuyul_sdk/_Database.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.1.0rc3/tuyul_sdk/_Gmail/__init__.py` & `tuyul_sdk-0.1.0rc4/tuyul_sdk/_Gmail/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,8 @@
 import base64
-import json
-import re
-import time
-from bs4 import BeautifulSoup
 from typing import Any, List, Union
 
 from google.oauth2.credentials import Credentials
 from googleapiclient.discovery import build
 
 from .Utils import Utils
```

### Comparing `tuyul_sdk-0.1.0rc3/tuyul_sdk/_Gmail/Utils.py` & `tuyul_sdk-0.1.0rc4/tuyul_sdk/_Gmail/Utils.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.1.0rc3/tuyul_sdk/Utils/_hexbytes.py` & `tuyul_sdk-0.1.0rc4/tuyul_sdk/Utils/_hexbytes.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.1.0rc3/tuyul_sdk/Utils/_Line.py` & `tuyul_sdk-0.1.0rc4/tuyul_sdk/Utils/_Line.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.1.0rc3/tuyul_sdk/Utils/_Log.py` & `tuyul_sdk-0.1.0rc4/tuyul_sdk/Utils/_Log.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.1.0rc3/tuyul_sdk/Utils/_Progress.py` & `tuyul_sdk-0.1.0rc4/tuyul_sdk/Utils/_Progress.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.1.0rc3/tuyul_sdk/Utils/_UserAgent.py` & `tuyul_sdk-0.1.0rc4/tuyul_sdk/Utils/_UserAgent.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.1.0rc3/setup.py` & `tuyul_sdk-0.1.0rc4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
  'requests==2.31.0',
  'sqlalchemy-utils==0.41.2',
  'sqlalchemy==2.0.30',
  'urllib3==1.26.15']
 
 setup_kwargs = {
     'name': 'tuyul-sdk',
-    'version': '0.1.0rc3',
+    'version': '0.1.0rc4',
     'description': '',
     'long_description': '',
     'author': 'DesKaOne',
     'author_email': 'DesKaOne@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `tuyul_sdk-0.1.0rc3/PKG-INFO` & `tuyul_sdk-0.1.0rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuyul-sdk
-Version: 0.1.0rc3
+Version: 0.1.0rc4
 Summary: 
 Author: DesKaOne
 Author-email: DesKaOne@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

