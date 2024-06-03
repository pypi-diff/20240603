# Comparing `tmp/ci_cloudconnector-2.6.tar.gz` & `tmp/ci_cloudconnector-2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ci_cloudconnector-2.6.tar", last modified: Sun Jun  2 07:51:00 2024, max compression
+gzip compressed data, was "ci_cloudconnector-2.7.tar", last modified: Mon Jun  3 13:14:41 2024, max compression
```

## Comparing `ci_cloudconnector-2.6.tar` & `ci_cloudconnector-2.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 07:51:00.806654 ci_cloudconnector-2.6/
-drwxrwxrwx   0        0        0        0 2024-06-02 07:51:00.796869 ci_cloudconnector-2.6/CI_CloudConnector.egg-info/
--rw-rw-rw-   0        0        0      357 2024-06-02 07:51:00.000000 ci_cloudconnector-2.6/CI_CloudConnector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2024-06-02 07:51:00.000000 ci_cloudconnector-2.6/CI_CloudConnector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 07:51:00.000000 ci_cloudconnector-2.6/CI_CloudConnector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-06-02 07:51:00.000000 ci_cloudconnector-2.6/CI_CloudConnector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      357 2024-06-02 07:51:00.796869 ci_cloudconnector-2.6/PKG-INFO
--rw-rw-rw-   0        0        0       86 2024-05-23 13:47:51.000000 ci_cloudconnector-2.6/README.txt
--rw-rw-rw-   0        0        0    36705 2024-06-02 07:50:04.000000 ci_cloudconnector-2.6/logic.py
--rw-rw-rw-   0        0        0     8242 2024-06-02 07:38:52.000000 ci_cloudconnector-2.6/main.py
--rw-rw-rw-   0        0        0     4188 2024-06-02 07:49:25.000000 ci_cloudconnector-2.6/myservice.py
--rw-rw-rw-   0        0        0     1601 2024-06-02 05:37:40.000000 ci_cloudconnector-2.6/myservice_installer.py
--rw-rw-rw-   0        0        0       42 2024-06-02 07:51:00.806654 ci_cloudconnector-2.6/setup.cfg
--rw-rw-rw-   0        0        0      813 2024-06-02 07:50:09.000000 ci_cloudconnector-2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 13:14:41.137160 ci_cloudconnector-2.7/
+drwxrwxrwx   0        0        0        0 2024-06-03 13:14:41.129462 ci_cloudconnector-2.7/CI_CloudConnector.egg-info/
+-rw-rw-rw-   0        0        0      339 2024-06-03 13:14:40.000000 ci_cloudconnector-2.7/CI_CloudConnector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-06-03 13:14:41.000000 ci_cloudconnector-2.7/CI_CloudConnector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 13:14:40.000000 ci_cloudconnector-2.7/CI_CloudConnector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-06-03 13:14:40.000000 ci_cloudconnector-2.7/CI_CloudConnector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      339 2024-06-03 13:14:41.133185 ci_cloudconnector-2.7/PKG-INFO
+-rw-rw-rw-   0        0        0       68 2024-06-02 07:57:17.000000 ci_cloudconnector-2.7/README.txt
+-rw-rw-rw-   0        0        0    32556 2024-06-03 13:13:55.000000 ci_cloudconnector-2.7/logic.py
+-rw-rw-rw-   0        0        0     8199 2024-06-03 08:47:12.000000 ci_cloudconnector-2.7/main.py
+-rw-rw-rw-   0        0        0     4188 2024-06-02 07:54:00.000000 ci_cloudconnector-2.7/myservice.py
+-rw-rw-rw-   0        0        0     1601 2024-06-02 05:37:40.000000 ci_cloudconnector-2.7/myservice_installer.py
+-rw-rw-rw-   0        0        0       42 2024-06-03 13:14:41.137968 ci_cloudconnector-2.7/setup.cfg
+-rw-rw-rw-   0        0        0      813 2024-06-03 13:13:50.000000 ci_cloudconnector-2.7/setup.py
```

### Comparing `ci_cloudconnector-2.6/logic.py` & `ci_cloudconnector-2.7/logic.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,65 +1,55 @@
-
 import logging, time, datetime, sys, socket, random, tzlocal, glob, fnmatch
 import platform
+from collections import deque
 from datetime import datetime
 from cpppo.server.enip import address, client
 import os
 import configparser
 import requests
 import json
 
-
-VER = "2.6"
-
-TagsDefenitionFileName = "TagsDefenition.txt"
-TagsValuesFileName = "[NEW]TagsValues"
-TagsValueDir = "TagValues"
-HomeDir = "CI_LC"
-GetTagsFromServerMinRateSeconds = 10
-GetCloudVersionFromServerMinRateSeconds = 10
-g_VerifySSL = False  # True = do not allow un verified connection , False = Allow
+VERSION = "2.7"
 
 # config
-cfg_server_address = ""
-cfg_username = ""
-cfg_password = ""
-cfg_max_files = ""
-cfg_log_level = ""
-
-
-sugestedUpdateVersion = ""
-configFile = "config.ini"
-ScanRateLastRead = {}
-currentToken = ""
-g_connectorTypeName = ""
-g_lastGetTagsFromServer = None
-g_lastGetCloudVersionFromServer = None
+CONFIG_SERVER_ADDRESS = ""
+CONFIG_USERNAME = ""
+CONFIG_PASSWORD = ""
+
+TAGS_DEFINITION_FILE_NAME = "TagsDefinition.txt"
+GET_TAGS_FROM_SERVER_MIN_RATE_SECONDS = 10
+GET_CLOUD_VERSION_FROM_SERVER_MIN_RATE_SECONDS = 10
+VERIFY_SSL = False  # True = do not allow un verified connection , False = Allow
+
+SUGGESTED_UPDATE_VERSION = ""
+CONFIG_FILE = "config.ini"
+SCAN_RATE_LAST_READ = {}
+CURRENT_TOKEN = ""
+CONNECTOR_TYPE_NAME = ""
+LAST_GET_TAGS_FROM_SERVER = None
+LAST_GET_CLOUD_VERSION_FROM_SERVER = None
 
 def enum(**enums):
     return type("Enum", (), enums)
 
 TagStatus = enum(Invalid=10, Valid=20)
 
 # Retrieve the logger instance
 logger = logging.getLogger(__name__)
 
 
 # ============================
-def read_last_rows_from_log(maxNumberOfRows=10):
+def read_last_rows_from_log(max_number_of_rows=10):
     log_file_path = "CloudConnectorService.log"
-    last_rows = []
-    i = maxNumberOfRows
-    for line in reversed(open(log_file_path, "r").readlines()):
-        last_rows.append(line.rstrip())
-        i = i - 1
-        if i <= 0:
-            return last_rows
-    return last_rows
+    if os.path.exists(log_file_path):
+        with open(log_file_path, "r") as file:
+            last_rows = deque(file, maxlen=max_number_of_rows)
 
+        return list(map(str.rstrip, last_rows))
+    return None
 
 # ============================
 def setLogLevel(lvl):
     try:
         if str(lvl) in ["CRITICAL", "ERROR", "WARNING", "INFO", "DEBUG", "NOTSET"]:
             lvl = logging.getLevelName(str(lvl))
 
@@ -85,15 +75,15 @@
     except Exception as e:
         logger.warning(f"An error occurred while logging: {e}")
 
 
 # ============================
 def SendLogToServer(log):
     try:
-        ret = addCloudConnectorLog(log, datetime.now())
+        addCloudConnectorLog(log, datetime.now())
         return
     except Exception as e:
         return
 
 
 
 # ============================
@@ -111,88 +101,76 @@
         ci_print(f"Error in handleError: {inner_err}", "ERROR")
 
 
 # ============================
 def getAliveFile():
     ret = None
     try:
-        file_path = "/" + HomeDir + "/lc_pid.txt"
+        file_path = "lc_pid.txt"
         with open(file_path, "r") as file:
             ret = json.load(file)
     except Exception as e:
         handleError("Error reading alive file: %s", e)
     return ret
 
 
 # ============================
 
 def initialize_config(overwrite=False):
 
-    global cfg_server_address
-    global cfg_username
-    global cfg_password
-    global cfg_max_files
-    global cfg_log_level
+    global CONFIG_SERVER_ADDRESS
+    global CONFIG_USERNAME
+    global CONFIG_PASSWORD
 
-    try:
-        file_path = f"/{HomeDir}/{configFile}"
 
-        log_levels_info = " , other options (DEBUG , INFO , WARNING , ERROR)"
+    try:
+        file_path = f"{CONFIG_FILE}"
 
         if os.path.exists(file_path) and not overwrite:
             config = configparser.ConfigParser()
             config.read(file_path)
 
-            cfg_server_address = config.get("Server", "Address")
-            cfg_username = config.get("Server", "username")
-            cfg_password = config.get("Server", "password")
-            cfg_max_files = config.get("Server", "maxFiles")
-            log_level = config.get("Logging", "Level", fallback=cfg_log_level)
+            CONFIG_SERVER_ADDRESS = config.get("Server", "Address")
+            CONFIG_USERNAME = config.get("Server", "username")
+            CONFIG_PASSWORD = config.get("Server", "password")
 
 
-            ci_print(f"Server Address: {cfg_server_address}", "INFO")
-            ci_print(f"Username: {cfg_username}", "INFO")
-            ci_print(f"Password: {cfg_password}", "INFO")
-            ci_print(f"Max Files: {cfg_max_files}", "INFO")
+            ci_print(f"Server Address: {CONFIG_SERVER_ADDRESS}", "INFO")
+            ci_print(f"Username: {CONFIG_USERNAME}", "INFO")
+            ci_print(f"Password: {CONFIG_PASSWORD}", "INFO")
             ci_print(f"VERSION: {getLocalVersion()}")
 
         else:
             ci_print(f"Config not found or overwrite is True, creating new one in {file_path}", "INFO")
             config = configparser.ConfigParser()
             config.add_section("Server")
             config.add_section("Logging")
 
             def get_input(prompt, current_value):
                 value = input(prompt + f" (Currently: {current_value}): ")
                 return value if value else current_value
 
-            cfg_server_address = get_input("Enter Server Address (e.g., https://localhost:63483)", cfg_server_address)
-            cfg_username = get_input("Enter new user name", cfg_username)
-            cfg_password = get_input("Enter password", cfg_password)
-            cfg_max_files = get_input("Enter Max Files", cfg_max_files)
-            cfg_log_level = get_input(f"Enter Logging Level {log_levels_info}", cfg_log_level)
-
-            config.set("Server", "Address", cfg_server_address)
-            config.set("Server", "username", cfg_username)
-            config.set("Server", "password", cfg_password)
-            config.set("Server", "maxFiles", cfg_max_files)
-            config.set("Logging", "Level", cfg_log_level)
+            CONFIG_SERVER_ADDRESS = get_input("Enter Server Address (e.g., https://localhost:63483)", CONFIG_SERVER_ADDRESS)
+            CONFIG_USERNAME = get_input("Enter new user name", CONFIG_USERNAME)
+            CONFIG_PASSWORD = get_input("Enter password", CONFIG_PASSWORD)
+
+            config.set("Server", "Address", CONFIG_SERVER_ADDRESS)
+            config.set("Server", "username", CONFIG_USERNAME)
+            config.set("Server", "password", CONFIG_PASSWORD)
 
 
             with open(file_path, "w") as configfile:
                 config.write(configfile)
 
             initialize_config()  # Reload the config after updating
 
     except Exception as inst:
         handleError("Error in initialize_config", inst)
 
 
-
-
 # ============================
 def reboot():
 
     try:
         if platform.system() == "Windows":
             ci_print("Reboot not supported on Windows.", "INFO")
             #subprocess.run(["shutdown", "/r", "/t", "0"], check=True)
@@ -203,56 +181,55 @@
         handleError("Error in reboot", ex)
 
 
 
 # Cloud Functions
 # ============================
 
-
-cfg_server_address = "your_server_address"
-g_VerifySSL = True
-currentToken = ""
-cfg_username = "your_username"
-cfg_password = "your_password"
+CONFIG_SERVER_ADDRESS = "your_server_address"
+VERIFY_SSL = True
+CURRENT_TOKEN = ""
+CONFIG_USERNAME = "your_username"
+CONFIG_PASSWORD = "your_password"
 
 
 def get_cloud_token():
 
-    global cfg_server_address
-    global g_VerifySSL
-    global currentToken
+    global CONFIG_SERVER_ADDRESS
+    global VERIFY_SSL
+    global CURRENT_TOKEN
 
-    if currentToken:
-        return currentToken
+    if CURRENT_TOKEN:
+        return CURRENT_TOKEN
 
-    url = f"{cfg_server_address}/api/CloudConnector/Token"
+    url = f"{CONFIG_SERVER_ADDRESS}/api/CloudConnector/Token"
 
     try:
         response = requests.post(
             url,
             data={
                 "grant_type": "password",
-                "username": cfg_username,
-                "password": cfg_password,
+                "username": CONFIG_USERNAME,
+                "password": CONFIG_PASSWORD,
             },
             headers={
                 "User-Agent": "python",
                 "Content-Type": "application/x-www-form-urlencoded",
             },
-            verify=g_VerifySSL,
+            verify=VERIFY_SSL,
         )
 
         response.raise_for_status()  # Raises an HTTPError for bad responses
         data = response.text
 
         jsonData = json.loads(data)
         token = jsonData.get("access_token", "")
 
         if token:
-            currentToken = token
+            CURRENT_TOKEN = token
 
     except requests.exceptions.RequestException as e:
         handleError("Error getting Token", e)
         token = ""
     except json.JSONDecodeError as e:
         handleError("Error decoding token response", e)
         token = ""
@@ -260,156 +237,144 @@
         handleError("Token not found in response", e)
         token = ""
 
     return token
 
 
 # ============================
-# make http request to cloud if fails set currentToken='' so it will be initialized next time
+# make http request to cloud if fails set CURRENT_TOKEN='' so it will be initialized next time
 # ============================
-def ciRequest(url, data, postGet="get", method="", token=""):
-    print(f"{datetime.now()}, START CIRequest {method}, VERSION: {VER}")
+def ciRequest(url, data, method="get", action="", token=""):
+    print(f"{datetime.datetime.now()}, START CIRequest {action}, VERSION: {VERSION}")
 
-    ans = {}
-    ans["isOK"] = False
-    global currentToken
-    ansIsSucessful = False
-    try:
-        if token == "":
-            print("Skipping " + method + " - no Token")
-            ans["isOK"] = False
-            return ans;
+    result = {"isOK": False}
+    global CURRENT_TOKEN
+
+    if not token:
+        ci_print(f"Skipping {action} - no Token")
+        return result
+
+    headers = {
+        "Authorization": f"Bearer {token}",
+        "Accept": "text/plain"
+    }
+
+    if method.lower() == "post":
+        headers["Content-Type"] = "application/json"
+
+    try:
+        if method.lower() == "post":
+            response = requests.post(url, data=data, headers=headers, verify=VERIFY_SSL)
         else:
-            if postGet == "post":
-                response = requests.post(
-                    url,
-                    data,
-                    headers={
-                        "Content-Type": "application/json",
-                        "Accept": "text/plain",
-                        "Authorization": "bearer %s" % token,
-                    },
-                    verify=g_VerifySSL,
-                )
-            else:
-                response = requests.get(
-                    url,
-                    data=None,
-                    headers={"Authorization": "bearer %s" % token},
-                    verify=g_VerifySSL,
-                )
+            response = requests.get(url, headers=headers, verify=VERIFY_SSL)
 
-            if response.status_code == 403:
-                currentToken = ""
-            ansIsSucessful = True
-    except Exception as err:
-        handleError("Error in ciRequest " + method, err)
-        currentToken = ""
-        ansIsSucessful = False
+        if response.status_code == 403:
+            CURRENT_TOKEN = ""
 
-    ans["isOK"] = ansIsSucessful
-    ans["response"] = response
-    return ans
+        result["isOK"] = response.status_code == 200
+        result["response"] = response
+
+    except Exception as err:
+        handleError(f"Error in ci_request {action}", err)
+        CURRENT_TOKEN = ""
 
+    return result
 
 
 # ============================
 def get_cloud_version():
 
-    global GetCloudVersionFromServerMinRateSeconds
-    global g_lastGetCloudVersionFromServer
-    global currentToken
-    global VER
-    global sugestedUpdateVersion
+    global GET_CLOUD_VERSION_FROM_SERVER_MIN_RATE_SECONDS
+    global LAST_GET_CLOUD_VERSION_FROM_SERVER
+    global CURRENT_TOKEN
+    global VERSION
+    global SUGGESTED_UPDATE_VERSION
 
-    if currentToken == "":
-        currentToken = get_cloud_token()
+    if CURRENT_TOKEN == "":
+        CURRENT_TOKEN = get_cloud_token()
 
-    token = currentToken
+    token = CURRENT_TOKEN
 
     tags = None
 
     try:
         now = datetime.now()
         getVersionTimePass = 0
 
-        if g_lastGetCloudVersionFromServer:
-            getVersionTimePass = (now - g_lastGetCloudVersionFromServer).total_seconds()
+        if LAST_GET_CLOUD_VERSION_FROM_SERVER:
+            getVersionTimePass = (now - LAST_GET_CLOUD_VERSION_FROM_SERVER).total_seconds()
 
-        if getVersionTimePass == 0 or getVersionTimePass > GetCloudVersionFromServerMinRateSeconds:
+        if getVersionTimePass == 0 or getVersionTimePass > GET_CLOUD_VERSION_FROM_SERVER_MIN_RATE_SECONDS:
 
             handleNewRequests()
 
-            g_lastGetCloudVersionFromServer = datetime.now()
+            LAST_GET_CLOUD_VERSION_FROM_SERVER = datetime.now()
             ip_address = socket.gethostbyname(socket.gethostname())
-            url = f"{cfg_server_address}/api/CloudConnector/GetVersion/?version={VER}&IpAddress={ip_address}"
+            url = f"{CONFIG_SERVER_ADDRESS}/api/CloudConnector/GetVersion/?version={VERSION}&IpAddress={ip_address}"
 
             ret = ciRequest(url, None, "get", "getCloudVersion", token)
             response = ret["response"]
 
             if not ret["isOK"]:
                 return ""
 
             ans = json.loads(response.text)
             update_to_version = ans[0]
 
-            sugestedUpdateVersion = update_to_version
+            SUGGESTED_UPDATE_VERSION = update_to_version
 
-            if bool(update_to_version) != "" and bool(update_to_version != VER):
-                ci_print(f"Local Version: {VER} but Server suggests Other Version: {update_to_version}", "INFO")
+            if bool(update_to_version) != "" and bool(update_to_version != VERSION):
+                ci_print(f"Local Version: {VERSION} but Server suggests Other Version: {update_to_version}", "INFO")
 
     except Exception as err:
         print(str(err))
         handleError("Error getting Version from cloud", err)
-        sugestedUpdateVersion = ""
+        SUGGESTED_UPDATE_VERSION = ""
 
-    return sugestedUpdateVersion
+    return SUGGESTED_UPDATE_VERSION
 
 
 # ============================
 def get_cloud_tags(token=""):
 
-    global g_lastGetTagsFromServer
-    global GetTagsFromServerMinRateSeconds
-
-    tags = None
+    global LAST_GET_TAGS_FROM_SERVER
+    global GET_TAGS_FROM_SERVER_MIN_RATE_SECONDS
 
     try:
-        IpAddress = socket.gethostbyname(socket.gethostname())
-        url = f"{cfg_server_address}/api/CloudConnector/GetTags/"
+        url = f"{CONFIG_SERVER_ADDRESS}/api/CloudConnector/GetTags/"
 
         tags = None
 
         now = datetime.now()
         getTagsTimePass = 0
 
-        if g_lastGetTagsFromServer:
-            getTagsTimePass = (now - g_lastGetTagsFromServer).total_seconds()
+        if LAST_GET_TAGS_FROM_SERVER:
+            getTagsTimePass = (now - LAST_GET_TAGS_FROM_SERVER).total_seconds()
 
-        if getTagsTimePass == 0 or getTagsTimePass > GetTagsFromServerMinRateSeconds:
+        if getTagsTimePass == 0 or getTagsTimePass > GET_TAGS_FROM_SERVER_MIN_RATE_SECONDS:
             ret = ciRequest(url, None, "get", "getCloudTags", token)
             if ret and ret["isOK"] == True:
                 response = ret["response"]
-                g_lastGetTagsFromServer = datetime.now()
+                LAST_GET_TAGS_FROM_SERVER = datetime.now()
                 ans = json.loads(response.text)
                 arranged_tags = arrange_tags_by_scan_time(ans["Tags"])
                 tags = {"Tags": arranged_tags}
 
-                with open(TagsDefenitionFileName, "w") as f:
+                with open(TAGS_DEFINITION_FILE_NAME, "w") as f:
                     json.dump(tags, f)
 
             else:
                 ci_print("Failed to retrieve Tags from Cloud server", "WARNING")
     except Exception as inst:
         print(str(inst))
         handleError("Error getting tags from cloud", inst)
         tags = None
 
     if tags == None:
-        tags = getTagsDefenitionFromFile()
+        tags = get_tags_definition_from_file()
 
     return tags
 
 
 # ============================
 def arrange_tags_by_scan_time(tags):
     ans = {}
@@ -444,109 +409,100 @@
             ci_print(msg, "INFO")
 
     except Exception as inst:
         handleError("Error in printTags", inst)
 
 
 # ============================
-def setCloudTags(tagValues, token=""):
-    print('setCloudTags')
+def set_cloud_tags(tag_values, token=""):
     global TagStatus
-    updatedSuccessfully = False
-    try:
-        # url = HTTP_PREFIX + '://'+cfg_server_address+'/api/CloudConnector/SetCounterHistory/'
-        url = cfg_server_address + "/api/CloudConnector/SetCounterHistory/"
+    updated_successfully = False
 
+    try:
+        url = f"{CONFIG_SERVER_ADDRESS}/api/CloudConnector/SetCounterHistory/"
         payload = []
-        for index in range(len(tagValues)):
-            TagId = tagValues[index]["TagId"]
-            timeStamp = str(tagValues[index]["time"])
-
-            value = tagValues[index]["value"]
-            status = TagStatus.Invalid
-            if str(tagValues[index]["status"]) == "20":
-                status = TagStatus.Valid
 
-
-            tagVal = {
-                "TagId": TagId,
-                "TimeStmp": timeStamp,
+        for tag in tag_values:
+            tag_id = tag.get("TagId")
+            timestamp = str(tag.get("time"))
+            value = tag.get("value")
+            status = TagStatus.Valid if str(tag.get("status")) == "20" else TagStatus.Invalid
+
+            tag_val = {
+                "TagId": tag_id,
+                "TimeStmp": timestamp,
                 "StatusCE": status,
                 "Value": value,
             }
-            payload.append(tagVal)
+            payload.append(tag_val)
+
+        ci_print(f'setCloudTags: {payload}', "INFO")
 
-        ci_print('setCloudTags: ' + str(payload), "INFO")
         ret = ciRequest(url, json.dumps(payload), "post", "setCloudTags", token)
         response = ret["response"]
 
-        updatedSuccessfully = response.status_code == 200
+        updated_successfully = response.status_code == 200
 
     except Exception as inst:
         handleError("Error setting tags in cloud", inst)
         return False
 
-    return updatedSuccessfully
+    return updated_successfully
 
 
 # ============================
 def sendLogFileToCloud(numberOfRows=10, timestamp="", requestId=""):
 
     try:
         requestId = str(requestId)
         lines = read_last_rows_from_log(numberOfRows)
         for line in lines:
-            # print "line:" + line
             addCloudConnectorLog(line, timestamp, str(requestId))
     except Exception as inst:
         handleError("sendLogFileToCloud: Error setting tags in cloud", inst)
         return False
 
 
 # ============================
-def addCloudConnectorLog(log, timeStamp="", requestId=""):
+def addCloudConnectorLog(log, timestamp="", request_id=""):
 
-    global currentToken
-    if timeStamp == "":
-        timeStamp = datetime.now()
-    updatedSuccessfully = False
+    global CURRENT_TOKEN
+    if timestamp == "":
+        timestamp = datetime.now()
 
-    token = currentToken
+    token = CURRENT_TOKEN
     if token == "":
-        print("no token skip addCloudConnectorLog", "INFO")
         return
+
+
     try:
-        url = cfg_server_address + "/api/CloudConnector/SetCounterLog/"
+        url = CONFIG_SERVER_ADDRESS + "/api/CloudConnector/SetCounterLog/"
 
         payload = []
-        logData = {"Log": log, "TimeStamp": str(timeStamp), "RequestId": requestId}
-        payload.append(logData)
-        # print str(payload)
+        payload = [{"Log": log, "TimeStamp": str(timestamp), "RequestId": request_id}]
         ret = ciRequest(url, json.dumps(payload), "post", "SetConnectorLog", token)
         response = ret["response"]
 
-        updatedSuccessfully = response.status_code == 200
+        return response.status_code == 200
 
     except Exception as inst:
         handleError("Exception in addCloudConnectorLog", inst)
         return False
 
-    return updatedSuccessfully
-
 
 # ============================
 def getCloudConnectorRequests():
 
-    global currentToken
-    token = currentToken
+    global CURRENT_TOKEN
+    token = CURRENT_TOKEN
 
 
     ans = None
     try:
-        url = cfg_server_address + "/api/CloudConnector/GetCloudConnectorRequests/"
+        url = CONFIG_SERVER_ADDRESS + "/api/CloudConnector/GetCloudConnectorRequests/"
         ret = ciRequest(url, None, "get", "GetCloudConnectorRequests", token)
 
         response = ret["response"]
         if ret["isOK"] == True:
             ans = json.loads(response.text)
     except Exception as inst:
         handleError("Error getting requests from cloud", inst)
@@ -554,24 +510,24 @@
 
     return ans
 
 
 # ============================
 def updateCloudConnectorRequests(requestId, status):
 
-    global currentToken
+    global CURRENT_TOKEN
     updatedSuccessfully = False
 
-    token = currentToken
+    token = CURRENT_TOKEN
     if token == "":
         ci_print("no token skip updateCloudConnectorRequests", "WARNING")
         return
     try:
         url = (
-            cfg_server_address
+            CONFIG_SERVER_ADDRESS
             + "/api/CloudConnector/SetCounterRequestStatus/?requestId="
             + str(requestId)
             + "&status="
             + str(status)
         )
 
         ret = ciRequest(url, "", "post", "SetCounterRequestStatus", token)
@@ -851,192 +807,117 @@
     ci_print("Count " + str(len(tagValues)) + " Tags", "INFO")
     for index in range(len(tagValues)):
         ci_print(str(tagValues[index]), "INFO")
 
 
 # ============================
 def getLocalVersion():
-    return VER
+    return VERSION
 
 
 # ============================
 def getServerSugestedVersion():
-    return sugestedUpdateVersion
+    return SUGGESTED_UPDATE_VERSION
 
 
 # ============================
 # Tag Files Functions
 # ============================
-def writeTagsDefenitionToFile(tags):
 
+def write_tags_definition_to_file(tags):
     try:
-
-        f = open(TagsDefenitionFileName, "w")
-        json.dump(tags, f)
-        f.close()
-        return
-    except Exception as inst:
-        handleError("Error in writeTagsDefenitionToFile", inst)
+        with open(TAGS_DEFINITION_FILE_NAME, "w") as f:
+            json.dump(tags, f)
+    except Exception as e:
+        handleError("Error in write_tags_definition_to_file", e)
 
 
 # ============================
-def getTagsDefenitionFromFile():
 
+def get_tags_definition_from_file():
     try:
-        f2 = open(TagsDefenitionFileName, "r")
-        tags = json.load(f2)
-        f2.close()
+        with open(TAGS_DEFINITION_FILE_NAME, "r") as f:
+            tags = json.load(f)
         return tags
-    except Exception as inst:
-        handleError("Error in getTagsDefenitionFromFile", inst)
-
+    except Exception as e:
+        handleError("Error in get_tags_definition_from_file", e)
 
 # ============================
-def delTagsDefenitionFile():
-
-    try:
-        os.remove(TagsDefenitionFileName)
-        return
-    except Exception as inst:
-        handleError("Error in delTagsDefenitionFile", inst)
 
 
-# ============================
-def getTagsValuesFromFile(fileName):
-
+def get_tags_values_from_file(file_path):
     try:
-        f2 = open(fileName, "r")
-        vals = json.load(f2)
-        f2.close()
-
-        return vals
-    except Exception as inst:
-        handleError("Error in getTagsValuesFromFile", inst)
+        with open(file_path, "r") as file:
+            values = json.load(file)
+        return values
+    except Exception as e:
+        handleError("Error in get_tags_values_from_file", e)
 
 
 # ============================
-def saveValuesToFile(values, fileName):
+def save_values_to_file(values, fileName):
 
     try:
-        numOfFiles = len(
-            fnmatch.filter(os.listdir("/" + HomeDir + "/" + TagsValueDir), "*.txt")
+        file_name = (
+                "[NEW]TagsValuesFile"
+                + datetime.now().strftime("%Y%m%d-%H%M%S%f")
+                + ".txt"
         )
-
-        if numOfFiles < 10000:
-            if fileName == "":
-                fileName = (
-                    TagsValuesFileName
-                    + datetime.now().strftime("%Y%m%d-%H%M%S%f")
-                    + ".txt"
-                )
-            # fileName = "./" + TagsValueDir + '/' + fileName
-            fileName = "/" + HomeDir + "/" + TagsValueDir + "/" + fileName
-
-            # write tags to file
-            f = open(fileName, "w")
+        with open(file_name, "w") as f:
             json.dump(values, f)
-            f.close()
-            time.sleep(1)  # prevent two files in same ms
-        else:
-            ci_print("Too many files in folder!!!", "WARNING")
-    except Exception as inst:
-        handleError("Error in saveValuesToFile", inst)
 
-# ============================
-def handleValuesFile(fileName, token=""):
+        time.sleep(1)
 
-    try:
-        values = getTagsValuesFromFile(fileName)
-        isOk = setCloudTags(values, token)
-        if isOk:
-            os.remove(fileName)
-            return True
-        else:
-            # errFile = replaceFileName(fileName,"ERR")
-            errFile = fileName.replace("/[NEW]", "/ERR/[ERR]")
-            os.rename(fileName, errFile)
     except Exception as inst:
-        handleError("Error in handleValuesFile", inst)
-    return False
+        handleError("Error in save_values_to_file", inst)
 
 # ============================
-def handleAllValuesFiles(token=""):
+def handle_values_file(file_name, token=""):
 
     try:
-        i = 0
-        dirpath = "/" + HomeDir + "/" + TagsValueDir + "/"
-        filesSortedByTime = [
-            s for s in os.listdir(dirpath) if os.path.isfile(os.path.join(dirpath, s))
-        ]
-        filesSortedByTime.sort(key=lambda s: os.path.getmtime(os.path.join(dirpath, s)))
-
-        for file in filesSortedByTime:
-            if file.endswith(".txt") and file.startswith("[NEW]"):
-                i = i + 1
-                handleValuesFile("/" + HomeDir + "/" + TagsValueDir + "/" + file, token)
-
-
-    except Exception as inst:
-        ci_print("Error handleAllValuesFiles " + str(inst))
-
-
-# ============================
-def create_directories_if_missing():
-    try:
-        # Create HomeDir if missing
-
-        dirName = "/" + HomeDir + "/"
-        d = os.path.dirname(dirName)
-
-        home_dir_path = os.path.join("/", HomeDir)
-        if not os.path.exists(home_dir_path):
-            os.makedirs(home_dir_path)
-            ci_print(f"Created directory: {home_dir_path}", "INFO")
+        values = get_tags_values_from_file(file_name)
+        if values:
+            isOk = set_cloud_tags(values, token)
+            if isOk:
+                os.remove(file_name)
+                return True
+            else:
 
-        # Create TagsValueDir if missing
-        tags_value_dir_path = os.path.join(home_dir_path, TagsValueDir)
-        if not os.path.exists(tags_value_dir_path):
-            os.makedirs(tags_value_dir_path)
-            ci_print(f"Created directory: {tags_value_dir_path}", "INFO")
+                # Create error directory if it does not exist
+                err_dir = os.path.join(os.path.dirname(file_name), "ERR")
+                if not os.path.exists(err_dir):
+                    os.makedirs(err_dir)
+
+                # Construct the new error file path
+                base_name = os.path.basename(file_name)
+                err_file = os.path.join(err_dir, base_name.replace("[NEW]", "[ERR]"))
 
-        # Create ERR directory inside TagsValueDir if missing
-        err_dir_path = os.path.join(tags_value_dir_path, "ERR")
-        if not os.path.exists(err_dir_path):
-            os.makedirs(err_dir_path)
-            ci_print(f"Created directory: {err_dir_path}", "INFO")
+                # Rename (move) the file to the error directory
+                os.rename(file_name, err_file)
 
     except Exception as e:
-        ci_print(f"Error in create_directories_if_missing: {e}")
-
+        handleError("Error in handle_values_file", e)
+    return False
 
 # ============================
-# Remove oldest file
-# ============================
-def removeOldestFile():
-
-    global cfg_max_files
+def handle_all_values_files(token=""):
 
     try:
-        dirName = "/" + HomeDir + "/" + TagsValueDir + "/"
-        dir = os.path.dirname(dirName)
-        if os.path.exists(dir):
-            list_of_files = glob.glob(dirName + '*.txt')
-            num_of_files = len(list_of_files)
-            maxFiles = int(cfg_max_files)
+        dir_path = os.getcwd()
+        files_starting_with_tags_values_file = [
+            file for file in os.listdir(dir_path) if file.startswith("[NEW]TagsValuesFile")
+        ]
+        files_starting_with_tags_values_file.sort(key=lambda s: os.path.getmtime(os.path.join(dir_path, s)))
 
-            if maxFiles < num_of_files & num_of_files > 0:
-                # In case more than one file is exceeding cfg_max_files.
-                # Used for initial case where num of files is much bigger than config MaxFiles.
-                for x in range(maxFiles, num_of_files):
-                    oldest_file = min(list_of_files, key=os.path.getctime)
-                    os.remove(oldest_file)
-                    list_of_files.remove(oldest_file)
+        for file in files_starting_with_tags_values_file:
+            if file.endswith(".txt") and file.startswith("[NEW]"):
+                handle_values_file(os.path.join(dir_path, file), token)
 
-    except Exception as inst:
-        handleError("Error in removeOldestFile", inst)
+    except Exception as e:
+        handleError("Error in handle_all_values_files", e)
 
 
 def arrange_by_connector_type(tags_def):
     arranged_tags = {}
 
     for tag in tags_def:
         connector_type = tag.get('connectorTypeName', '')  # Provide a default value if key doesn't exist
@@ -1047,35 +928,35 @@
     return arranged_tags
 
 # ============================
 # Main Loop
 # ============================
 def Main():
 
-    global ScanRateLastRead
-    global currentToken
+    global SCAN_RATE_LAST_READ
+    global CURRENT_TOKEN
     try:
 
-        if currentToken == "":
-            currentToken = get_cloud_token()
+        if CURRENT_TOKEN == "":
+            CURRENT_TOKEN = get_cloud_token()
         # currently must get tags from cloud to init server before setting values
-        tagsDefScanRatesAns = get_cloud_tags(currentToken)
+        tagsDefScanRatesAns = get_cloud_tags(CURRENT_TOKEN)
         tagsDefScanRates = tagsDefScanRatesAns["Tags"]
 
         for scanRate in tagsDefScanRates:
 
             if scanRate in (None, 'null'):
                 continue
 
             scanRateInt = int(scanRate)
             scanRateStr = str(scanRate)
             diff = 0
-            if scanRateStr in ScanRateLastRead:
+            if scanRateStr in SCAN_RATE_LAST_READ:
                 now = datetime.now()
-                diff = (now - ScanRateLastRead[scanRateStr]).total_seconds()
+                diff = (now - SCAN_RATE_LAST_READ[scanRateStr]).total_seconds()
                 # print ('diff = -------' + str(diff))
 
 
             if diff + 3 > scanRateInt or diff == 0:
 
 
                 tagsDef = tagsDefScanRates[scanRate]
@@ -1098,30 +979,23 @@
                                 ci_print("Ethernet Empty values ::1", "ERROR")
                                 values = readEtherNetIP_Tags(arranged_tags[connector_type])
                                 if values == []:
                                     time.sleep(1)
                                     ci_print("Ethernet Empty values ::2", "ERROR")
                                     values = readEtherNetIP_Tags(arranged_tags[connector_type])
 
-                    #if len(values) > 0:
-                    #    ci_print(f'ScanRate: {scanRate}, DIFF: {diff}, Values: {values}')
-                    #else:
-                    #    ci_print(f'ScanRate: {scanRate}, DIFF: {diff}, No Values')
-
                     if values:
-                        saveValuesToFile(values, "")
-                        removeOldestFile()
-
+                        save_values_to_file(values, "")
                         now = datetime.now()
-                        ScanRateLastRead[scanRateStr] = now
+                        SCAN_RATE_LAST_READ[scanRateStr] = now
 
 
-        if currentToken != "":
-            handleAllValuesFiles(currentToken)
+        if CURRENT_TOKEN != "":
+            handle_all_values_files(CURRENT_TOKEN)
         else:
             ci_print("No Token, skipping upload step", "WARNING")
     except Exception as inst:
         handleError("Error in Main", inst)
-        currentToken = ""
+        CURRENT_TOKEN = ""
```

### Comparing `ci_cloudconnector-2.6/main.py` & `ci_cloudconnector-2.7/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,15 +226,14 @@
     observer.schedule(event_handler, path=os.path.dirname(main_file), recursive=False)
 
     observer.start()
     return observer
 
 
 def init():
-    logic.create_directories_if_missing()
     logic.initialize_config()
     set_service_restart_delay("CloudConnectorService", 10000)
 
 
 
 def serviceStop():
     global service_stop
```

### Comparing `ci_cloudconnector-2.6/myservice.py` & `ci_cloudconnector-2.7/myservice.py`

 * *Files identical despite different names*

### Comparing `ci_cloudconnector-2.6/myservice_installer.py` & `ci_cloudconnector-2.7/myservice_installer.py`

 * *Files identical despite different names*

### Comparing `ci_cloudconnector-2.6/setup.py` & `ci_cloudconnector-2.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     return ans
 
 
 
 setup(
     name="CI_CloudConnector",
-    version="2.6",
+    version="2.7",
     packages=find_packages(),
     py_modules=["logic", "main", "setup", "myservice", "myservice_installer"],
     description="IOT application that collects data from PLC (ModBus or AnB Ethernet/IP) and sends it to the cloud using HTTPS",
     author="Yochai",
     author_email="yochaim@contel.co.il",
     install_requires=[],
     url="https://trunovate.com/",
```

