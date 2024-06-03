# Comparing `tmp/ci_cloudconnector-2.7.tar.gz` & `tmp/ci_cloudconnector-2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ci_cloudconnector-2.7.tar", last modified: Mon Jun  3 13:14:41 2024, max compression
+gzip compressed data, was "ci_cloudconnector-2.8.tar", last modified: Mon Jun  3 13:21:50 2024, max compression
```

## Comparing `ci_cloudconnector-2.7.tar` & `ci_cloudconnector-2.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-06-03 13:14:41.137160 ci_cloudconnector-2.7/
-drwxrwxrwx   0        0        0        0 2024-06-03 13:14:41.129462 ci_cloudconnector-2.7/CI_CloudConnector.egg-info/
--rw-rw-rw-   0        0        0      339 2024-06-03 13:14:40.000000 ci_cloudconnector-2.7/CI_CloudConnector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2024-06-03 13:14:41.000000 ci_cloudconnector-2.7/CI_CloudConnector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 13:14:40.000000 ci_cloudconnector-2.7/CI_CloudConnector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-06-03 13:14:40.000000 ci_cloudconnector-2.7/CI_CloudConnector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      339 2024-06-03 13:14:41.133185 ci_cloudconnector-2.7/PKG-INFO
--rw-rw-rw-   0        0        0       68 2024-06-02 07:57:17.000000 ci_cloudconnector-2.7/README.txt
--rw-rw-rw-   0        0        0    32556 2024-06-03 13:13:55.000000 ci_cloudconnector-2.7/logic.py
--rw-rw-rw-   0        0        0     8199 2024-06-03 08:47:12.000000 ci_cloudconnector-2.7/main.py
--rw-rw-rw-   0        0        0     4188 2024-06-02 07:54:00.000000 ci_cloudconnector-2.7/myservice.py
--rw-rw-rw-   0        0        0     1601 2024-06-02 05:37:40.000000 ci_cloudconnector-2.7/myservice_installer.py
--rw-rw-rw-   0        0        0       42 2024-06-03 13:14:41.137968 ci_cloudconnector-2.7/setup.cfg
--rw-rw-rw-   0        0        0      813 2024-06-03 13:13:50.000000 ci_cloudconnector-2.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 13:21:50.988298 ci_cloudconnector-2.8/
+drwxrwxrwx   0        0        0        0 2024-06-03 13:21:50.983466 ci_cloudconnector-2.8/CI_CloudConnector.egg-info/
+-rw-rw-rw-   0        0        0      339 2024-06-03 13:21:50.000000 ci_cloudconnector-2.8/CI_CloudConnector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-06-03 13:21:50.000000 ci_cloudconnector-2.8/CI_CloudConnector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 13:21:50.000000 ci_cloudconnector-2.8/CI_CloudConnector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-06-03 13:21:50.000000 ci_cloudconnector-2.8/CI_CloudConnector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      339 2024-06-03 13:21:50.985437 ci_cloudconnector-2.8/PKG-INFO
+-rw-rw-rw-   0        0        0       68 2024-06-02 07:57:17.000000 ci_cloudconnector-2.8/README.txt
+-rw-rw-rw-   0        0        0    32327 2024-06-03 13:21:25.000000 ci_cloudconnector-2.8/logic.py
+-rw-rw-rw-   0        0        0     8199 2024-06-03 08:47:12.000000 ci_cloudconnector-2.8/main.py
+-rw-rw-rw-   0        0        0     4188 2024-06-02 07:54:00.000000 ci_cloudconnector-2.8/myservice.py
+-rw-rw-rw-   0        0        0     1601 2024-06-02 05:37:40.000000 ci_cloudconnector-2.8/myservice_installer.py
+-rw-rw-rw-   0        0        0       42 2024-06-03 13:21:50.988359 ci_cloudconnector-2.8/setup.cfg
+-rw-rw-rw-   0        0        0      813 2024-06-03 13:21:19.000000 ci_cloudconnector-2.8/setup.py
```

### Comparing `ci_cloudconnector-2.7/logic.py` & `ci_cloudconnector-2.8/logic.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from datetime import datetime
 from cpppo.server.enip import address, client
 import os
 import configparser
 import requests
 import json
 
-VERSION = "2.7"
+VERSION = "2.8"
 
 # config
 CONFIG_SERVER_ADDRESS = ""
 CONFIG_USERNAME = ""
 CONFIG_PASSWORD = ""
 
 TAGS_DEFINITION_FILE_NAME = "TagsDefinition.txt"
@@ -240,15 +240,15 @@
     return token
 
 
 # ============================
 # make http request to cloud if fails set CURRENT_TOKEN='' so it will be initialized next time
 # ============================
 def ciRequest(url, data, method="get", action="", token=""):
-    print(f"{datetime.datetime.now()}, START CIRequest {action}, VERSION: {VERSION}")
+    print(f"{datetime.now()}, START CIRequest {action}, VERSION: {VERSION}")
 
     result = {"isOK": False}
     global CURRENT_TOKEN
 
     if not token:
         ci_print(f"Skipping {action} - no Token")
         return result
@@ -548,22 +548,19 @@
 
     try:
         requests = getCloudConnectorRequests()
         if requests:
 
             for request in requests:
                 try:
-                    # print 'request[Type]=' + str(request['Type'])
                     if request["Type"] == 1:  # send logs
-                        # print "Handling request " + str(request)
                         requestData = json.loads(request["Data"])
                         rownCount = requestData["Rows"]
                         ret = updateCloudConnectorRequests(request["Id"], 2)  # in process
                         requestData = json.loads(request["Data"])
-                        # print "--------request['Id']===" + str(request['Id'])
                         sendLogFileToCloud(rownCount, "", request["Id"])
                         ret = updateCloudConnectorRequests(request["Id"], 3)  # Done
                     if request["Type"] == 2:  # change logs level
                         ci_print(
                             "Handling change log level request " + str(request), "INFO"
                         )
                         requestData = json.loads(request["Data"])
@@ -768,15 +765,14 @@
 def readSimulation_Tags(tags_definitions):
 
     ans = []
     arranged_tags = arrange_tags_by_plc(tags_definitions)
 
     ci_print("Start Read readSimulation_Tags", "INFO")
 
-
     try:
 
         for plc_address, tags_def_list in arranged_tags.items():
             for index, tag_def in enumerate(tags_def_list):
                 try:
                     TagId = int(tag_def.get("TagId"))
                     value = random.uniform(-10, 10)
```

### Comparing `ci_cloudconnector-2.7/main.py` & `ci_cloudconnector-2.8/main.py`

 * *Files identical despite different names*

### Comparing `ci_cloudconnector-2.7/myservice.py` & `ci_cloudconnector-2.8/myservice.py`

 * *Files identical despite different names*

### Comparing `ci_cloudconnector-2.7/myservice_installer.py` & `ci_cloudconnector-2.8/myservice_installer.py`

 * *Files identical despite different names*

### Comparing `ci_cloudconnector-2.7/setup.py` & `ci_cloudconnector-2.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     return ans
 
 
 
 setup(
     name="CI_CloudConnector",
-    version="2.7",
+    version="2.8",
     packages=find_packages(),
     py_modules=["logic", "main", "setup", "myservice", "myservice_installer"],
     description="IOT application that collects data from PLC (ModBus or AnB Ethernet/IP) and sends it to the cloud using HTTPS",
     author="Yochai",
     author_email="yochaim@contel.co.il",
     install_requires=[],
     url="https://trunovate.com/",
```

