# Comparing `tmp/ci_cloudconnector-2.9.tar.gz` & `tmp/ci_cloudconnector-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ci_cloudconnector-2.9.tar", last modified: Mon Jun  3 13:31:15 2024, max compression
+gzip compressed data, was "ci_cloudconnector-3.1.tar", last modified: Mon Jun  3 13:42:05 2024, max compression
```

## Comparing `ci_cloudconnector-2.9.tar` & `ci_cloudconnector-3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-06-03 13:31:15.619028 ci_cloudconnector-2.9/
-drwxrwxrwx   0        0        0        0 2024-06-03 13:31:15.613026 ci_cloudconnector-2.9/CI_CloudConnector.egg-info/
--rw-rw-rw-   0        0        0      339 2024-06-03 13:31:15.000000 ci_cloudconnector-2.9/CI_CloudConnector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2024-06-03 13:31:15.000000 ci_cloudconnector-2.9/CI_CloudConnector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 13:31:15.000000 ci_cloudconnector-2.9/CI_CloudConnector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-06-03 13:31:15.000000 ci_cloudconnector-2.9/CI_CloudConnector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      339 2024-06-03 13:31:15.616516 ci_cloudconnector-2.9/PKG-INFO
--rw-rw-rw-   0        0        0       68 2024-06-02 07:57:17.000000 ci_cloudconnector-2.9/README.txt
--rw-rw-rw-   0        0        0    32368 2024-06-03 13:29:52.000000 ci_cloudconnector-2.9/logic.py
--rw-rw-rw-   0        0        0     8199 2024-06-03 08:47:12.000000 ci_cloudconnector-2.9/main.py
--rw-rw-rw-   0        0        0     4183 2024-06-03 13:29:16.000000 ci_cloudconnector-2.9/myservice.py
--rw-rw-rw-   0        0        0     1601 2024-06-02 05:37:40.000000 ci_cloudconnector-2.9/myservice_installer.py
--rw-rw-rw-   0        0        0       42 2024-06-03 13:31:15.619028 ci_cloudconnector-2.9/setup.cfg
--rw-rw-rw-   0        0        0      624 2024-06-03 13:29:43.000000 ci_cloudconnector-2.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 13:42:05.558918 ci_cloudconnector-3.1/
+drwxrwxrwx   0        0        0        0 2024-06-03 13:42:05.551809 ci_cloudconnector-3.1/CI_CloudConnector.egg-info/
+-rw-rw-rw-   0        0        0      339 2024-06-03 13:42:05.000000 ci_cloudconnector-3.1/CI_CloudConnector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-06-03 13:42:05.000000 ci_cloudconnector-3.1/CI_CloudConnector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 13:42:05.000000 ci_cloudconnector-3.1/CI_CloudConnector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-06-03 13:42:05.000000 ci_cloudconnector-3.1/CI_CloudConnector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      339 2024-06-03 13:42:05.554811 ci_cloudconnector-3.1/PKG-INFO
+-rw-rw-rw-   0        0        0       68 2024-06-02 07:57:17.000000 ci_cloudconnector-3.1/README.txt
+-rw-rw-rw-   0        0        0    32332 2024-06-03 13:41:42.000000 ci_cloudconnector-3.1/logic.py
+-rw-rw-rw-   0        0        0     8199 2024-06-03 08:47:12.000000 ci_cloudconnector-3.1/main.py
+-rw-rw-rw-   0        0        0     4137 2024-06-03 13:39:03.000000 ci_cloudconnector-3.1/myservice.py
+-rw-rw-rw-   0        0        0     1601 2024-06-02 05:37:40.000000 ci_cloudconnector-3.1/myservice_installer.py
+-rw-rw-rw-   0        0        0       42 2024-06-03 13:42:05.558918 ci_cloudconnector-3.1/setup.cfg
+-rw-rw-rw-   0        0        0      624 2024-06-03 13:41:50.000000 ci_cloudconnector-3.1/setup.py
```

### Comparing `ci_cloudconnector-2.9/logic.py` & `ci_cloudconnector-3.1/logic.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from datetime import datetime
 from cpppo.server.enip import address, client
 import os
 import configparser
 import requests
 import json
 
-VERSION = "2.9"
+VERSION = "3.1"
 
 # config
 CONFIG_SERVER_ADDRESS = ""
 CONFIG_USERNAME = ""
 CONFIG_PASSWORD = ""
 
 TAGS_DEFINITION_FILE_NAME = "TagsDefinition.txt"
@@ -258,18 +258,18 @@
     }
 
     if method.lower() == "post":
         headers["Content-Type"] = "application/json"
 
     try:
         if method.lower() == "post":
-            ci_print(f"{datetime.now()}, ciRequest url: {url} action: {action}, data: {data}")
+            ci_print(f"ciRequest url: {url} action: {action}, data: {data}")
             response = requests.post(url, data=data, headers=headers, verify=VERIFY_SSL)
         else:
-            ci_print(f"{datetime.now()}, ciRequest url: {url} action: {action}")
+            ci_print(f"ciRequest url: {url} action: {action}")
             response = requests.get(url, headers=headers, verify=VERIFY_SSL)
 
         if response.status_code == 403:
             CURRENT_TOKEN = ""
 
         result["isOK"] = response.status_code == 200
         result["response"] = response
```

### Comparing `ci_cloudconnector-2.9/main.py` & `ci_cloudconnector-3.1/main.py`

 * *Files identical despite different names*

### Comparing `ci_cloudconnector-2.9/myservice.py` & `ci_cloudconnector-3.1/myservice.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,29 +15,28 @@
     _svc_display_name_ = "CloudConnectorService"
     _svc_failure_actions_ = "restart/10000"  # Restart the service after 1 minute if it fails
 
     def __init__(self, args):
         logging.basicConfig(
             level=logging.INFO,
             format='%(asctime)s: %(name)s: %(funcName)s: (%(lineno)d): %(levelname)s: %(message)s',
-            datefmt='%Y-%m-%d %H:%M:%S'
         )
 
         rotating_handler = RotatingFileHandler(
             filename='CloudConnectorService.log',
             mode="a",
             maxBytes=5 * 1024 * 1024,
             backupCount=10,
             encoding=None,
             delay=0,
         )
 
         rotating_handler.setLevel(logging.INFO)
         formatter = logging.Formatter(
-            '%(asctime)s - %(name)s - %(funcName)s - (%(lineno)d) - %(levelname)s - %(message)s')
+            '%(asctime)s: %(name)s: %(funcName)s: (%(lineno)d): %(levelname)s: %(message)s')
         rotating_handler.setFormatter(formatter)
 
         logging.getLogger().addHandler(rotating_handler)
 
         # Now initialize other attributes
         win32serviceutil.ServiceFramework.__init__(self, args)
         self.stop_event = win32event.CreateEvent(None, 0, 0, None)
```

### Comparing `ci_cloudconnector-2.9/myservice_installer.py` & `ci_cloudconnector-3.1/myservice_installer.py`

 * *Files identical despite different names*

### Comparing `ci_cloudconnector-2.9/setup.py` & `ci_cloudconnector-3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logic
 from distutils.core import setup
 from setuptools import setup, find_packages
 
 setup(
     name="CI_CloudConnector",
-    version="2.9",
+    version="3.1",
     packages=find_packages(),
     py_modules=["logic", "main", "setup", "myservice", "myservice_installer"],
     description="IOT application that collects data from PLC (ModBus or AnB Ethernet/IP) and sends it to the cloud using HTTPS",
     author="Yochai",
     author_email="yochaim@contel.co.il",
     install_requires=[],
     url="https://trunovate.com/",
```

