# Comparing `tmp/ci_cloudconnector-2.8.tar.gz` & `tmp/ci_cloudconnector-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ci_cloudconnector-2.8.tar", last modified: Mon Jun  3 13:21:50 2024, max compression
+gzip compressed data, was "ci_cloudconnector-2.9.tar", last modified: Mon Jun  3 13:31:15 2024, max compression
```

## Comparing `ci_cloudconnector-2.8.tar` & `ci_cloudconnector-2.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-06-03 13:21:50.988298 ci_cloudconnector-2.8/
-drwxrwxrwx   0        0        0        0 2024-06-03 13:21:50.983466 ci_cloudconnector-2.8/CI_CloudConnector.egg-info/
--rw-rw-rw-   0        0        0      339 2024-06-03 13:21:50.000000 ci_cloudconnector-2.8/CI_CloudConnector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2024-06-03 13:21:50.000000 ci_cloudconnector-2.8/CI_CloudConnector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 13:21:50.000000 ci_cloudconnector-2.8/CI_CloudConnector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-06-03 13:21:50.000000 ci_cloudconnector-2.8/CI_CloudConnector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      339 2024-06-03 13:21:50.985437 ci_cloudconnector-2.8/PKG-INFO
--rw-rw-rw-   0        0        0       68 2024-06-02 07:57:17.000000 ci_cloudconnector-2.8/README.txt
--rw-rw-rw-   0        0        0    32327 2024-06-03 13:21:25.000000 ci_cloudconnector-2.8/logic.py
--rw-rw-rw-   0        0        0     8199 2024-06-03 08:47:12.000000 ci_cloudconnector-2.8/main.py
--rw-rw-rw-   0        0        0     4188 2024-06-02 07:54:00.000000 ci_cloudconnector-2.8/myservice.py
--rw-rw-rw-   0        0        0     1601 2024-06-02 05:37:40.000000 ci_cloudconnector-2.8/myservice_installer.py
--rw-rw-rw-   0        0        0       42 2024-06-03 13:21:50.988359 ci_cloudconnector-2.8/setup.cfg
--rw-rw-rw-   0        0        0      813 2024-06-03 13:21:19.000000 ci_cloudconnector-2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 13:31:15.619028 ci_cloudconnector-2.9/
+drwxrwxrwx   0        0        0        0 2024-06-03 13:31:15.613026 ci_cloudconnector-2.9/CI_CloudConnector.egg-info/
+-rw-rw-rw-   0        0        0      339 2024-06-03 13:31:15.000000 ci_cloudconnector-2.9/CI_CloudConnector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-06-03 13:31:15.000000 ci_cloudconnector-2.9/CI_CloudConnector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 13:31:15.000000 ci_cloudconnector-2.9/CI_CloudConnector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-06-03 13:31:15.000000 ci_cloudconnector-2.9/CI_CloudConnector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      339 2024-06-03 13:31:15.616516 ci_cloudconnector-2.9/PKG-INFO
+-rw-rw-rw-   0        0        0       68 2024-06-02 07:57:17.000000 ci_cloudconnector-2.9/README.txt
+-rw-rw-rw-   0        0        0    32368 2024-06-03 13:29:52.000000 ci_cloudconnector-2.9/logic.py
+-rw-rw-rw-   0        0        0     8199 2024-06-03 08:47:12.000000 ci_cloudconnector-2.9/main.py
+-rw-rw-rw-   0        0        0     4183 2024-06-03 13:29:16.000000 ci_cloudconnector-2.9/myservice.py
+-rw-rw-rw-   0        0        0     1601 2024-06-02 05:37:40.000000 ci_cloudconnector-2.9/myservice_installer.py
+-rw-rw-rw-   0        0        0       42 2024-06-03 13:31:15.619028 ci_cloudconnector-2.9/setup.cfg
+-rw-rw-rw-   0        0        0      624 2024-06-03 13:29:43.000000 ci_cloudconnector-2.9/setup.py
```

### Comparing `ci_cloudconnector-2.8/logic.py` & `ci_cloudconnector-2.9/logic.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from datetime import datetime
 from cpppo.server.enip import address, client
 import os
 import configparser
 import requests
 import json
 
-VERSION = "2.8"
+VERSION = "2.9"
 
 # config
 CONFIG_SERVER_ADDRESS = ""
 CONFIG_USERNAME = ""
 CONFIG_PASSWORD = ""
 
 TAGS_DEFINITION_FILE_NAME = "TagsDefinition.txt"
@@ -66,15 +66,15 @@
         elif level == "INFO":
             logger.info(msg)
         elif level == "ERROR":
             logger.error(msg)
         elif level == "WARNING":
             logger.warning(msg)
         else:
-            logger.warning(msg)
+            logger.info(msg)
 
     except Exception as e:
         logger.warning(f"An error occurred while logging: {e}")
 
 
 # ============================
 def SendLogToServer(log):
@@ -240,15 +240,14 @@
     return token
 
 
 # ============================
 # make http request to cloud if fails set CURRENT_TOKEN='' so it will be initialized next time
 # ============================
 def ciRequest(url, data, method="get", action="", token=""):
-    print(f"{datetime.now()}, START CIRequest {action}, VERSION: {VERSION}")
 
     result = {"isOK": False}
     global CURRENT_TOKEN
 
     if not token:
         ci_print(f"Skipping {action} - no Token")
         return result
@@ -259,16 +258,18 @@
     }
 
     if method.lower() == "post":
         headers["Content-Type"] = "application/json"
 
     try:
         if method.lower() == "post":
+            ci_print(f"{datetime.now()}, ciRequest url: {url} action: {action}, data: {data}")
             response = requests.post(url, data=data, headers=headers, verify=VERIFY_SSL)
         else:
+            ci_print(f"{datetime.now()}, ciRequest url: {url} action: {action}")
             response = requests.get(url, headers=headers, verify=VERIFY_SSL)
 
         if response.status_code == 403:
             CURRENT_TOKEN = ""
 
         result["isOK"] = response.status_code == 200
         result["response"] = response
@@ -431,16 +432,14 @@
                 "TagId": tag_id,
                 "TimeStmp": timestamp,
                 "StatusCE": status,
                 "Value": value,
             }
             payload.append(tag_val)
 
-        ci_print(f'setCloudTags: {payload}', "INFO")
-
         ret = ciRequest(url, json.dumps(payload), "post", "setCloudTags", token)
         response = ret["response"]
 
         updated_successfully = response.status_code == 200
 
     except Exception as inst:
         handleError("Error setting tags in cloud", inst)
```

### Comparing `ci_cloudconnector-2.8/main.py` & `ci_cloudconnector-2.9/main.py`

 * *Files identical despite different names*

### Comparing `ci_cloudconnector-2.8/myservice.py` & `ci_cloudconnector-2.9/myservice.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     _svc_name_ = "CloudConnectorService"
     _svc_display_name_ = "CloudConnectorService"
     _svc_failure_actions_ = "restart/10000"  # Restart the service after 1 minute if it fails
 
     def __init__(self, args):
         logging.basicConfig(
             level=logging.INFO,
-            format='%(asctime)s - %(name)s - %(funcName)s - (%(lineno)d) - %(levelname)s - %(message)s',
+            format='%(asctime)s: %(name)s: %(funcName)s: (%(lineno)d): %(levelname)s: %(message)s',
             datefmt='%Y-%m-%d %H:%M:%S'
         )
 
         rotating_handler = RotatingFileHandler(
             filename='CloudConnectorService.log',
             mode="a",
             maxBytes=5 * 1024 * 1024,
```

### Comparing `ci_cloudconnector-2.8/myservice_installer.py` & `ci_cloudconnector-2.9/myservice_installer.py`

 * *Files identical despite different names*

### Comparing `ci_cloudconnector-2.8/setup.py` & `ci_cloudconnector-2.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,14 @@
 import logic
 from distutils.core import setup
 from setuptools import setup, find_packages
 
-def getVersion():
-    ans = ""
-    try:
-        ans = logic.getLocalVersion()
-    except Exception as inst:
-        print("Error getting version") + str(inst)
-
-    return ans
-
-
-
 setup(
     name="CI_CloudConnector",
-    version="2.8",
+    version="2.9",
     packages=find_packages(),
     py_modules=["logic", "main", "setup", "myservice", "myservice_installer"],
     description="IOT application that collects data from PLC (ModBus or AnB Ethernet/IP) and sends it to the cloud using HTTPS",
     author="Yochai",
     author_email="yochaim@contel.co.il",
     install_requires=[],
     url="https://trunovate.com/",
```

