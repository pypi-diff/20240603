# Comparing `tmp/logos_sdk-0.0.25.dev1.tar.gz` & `tmp/logos_sdk-0.0.25.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logos_sdk-0.0.25.dev1.tar", last modified: Thu May 30 11:26:29 2024, max compression
+gzip compressed data, was "logos_sdk-0.0.25.dev2.tar", last modified: Mon Jun  3 13:18:01 2024, max compression
```

## Comparing `logos_sdk-0.0.25.dev1.tar` & `logos_sdk-0.0.25.dev2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 W          (501) staff       (20)        0 2024-05-30 11:26:29.996153 logos_sdk-0.0.25.dev1/
--rw-r--r--   0 W          (501) staff       (20)     1061 2024-05-16 14:39:43.000000 logos_sdk-0.0.25.dev1/LICENSE
--rw-r--r--   0 W          (501) staff       (20)     9586 2024-05-30 11:26:29.996058 logos_sdk-0.0.25.dev1/PKG-INFO
--rw-r--r--   0 W          (501) staff       (20)     8935 2024-05-30 10:55:15.000000 logos_sdk-0.0.25.dev1/README.md
-drwxr-xr-x   0 W          (501) staff       (20)        0 2024-05-30 11:26:29.990126 logos_sdk-0.0.25.dev1/logos_sdk/
--rw-r--r--   0 W          (501) staff       (20)      116 2024-05-16 14:06:44.000000 logos_sdk-0.0.25.dev1/logos_sdk/__init__.py
-drwxr-xr-x   0 W          (501) staff       (20)        0 2024-05-30 11:26:29.991608 logos_sdk-0.0.25.dev1/logos_sdk/big_query/
--rw-r--r--   0 W          (501) staff       (20)     5498 2024-05-20 07:25:33.000000 logos_sdk-0.0.25.dev1/logos_sdk/big_query/BigQuery.py
--rw-r--r--   0 W          (501) staff       (20)      745 2024-01-08 11:17:31.000000 logos_sdk-0.0.25.dev1/logos_sdk/big_query/__init__.py
-drwxr-xr-x   0 W          (501) staff       (20)        0 2024-05-30 11:26:29.992270 logos_sdk-0.0.25.dev1/logos_sdk/logging/
--rw-r--r--   0 W          (501) staff       (20)     2557 2024-05-16 14:06:44.000000 logos_sdk-0.0.25.dev1/logos_sdk/logging/LogosLogger.py
--rw-r--r--   0 W          (501) staff       (20)     2818 2023-09-13 09:34:42.000000 logos_sdk-0.0.25.dev1/logos_sdk/logging/__init__.py
-drwxr-xr-x   0 W          (501) staff       (20)        0 2024-05-30 11:26:29.995474 logos_sdk-0.0.25.dev1/logos_sdk/services/
--rw-r--r--   0 W          (501) staff       (20)    14319 2024-05-16 14:19:15.000000 logos_sdk-0.0.25.dev1/logos_sdk/services/CampaignManager.py
--rw-r--r--   0 W          (501) staff       (20)     7036 2024-05-16 14:06:44.000000 logos_sdk-0.0.25.dev1/logos_sdk/services/Collabim.py
--rw-r--r--   0 W          (501) staff       (20)    15566 2024-05-29 06:52:17.000000 logos_sdk-0.0.25.dev1/logos_sdk/services/DV360.py
--rw-r--r--   0 W          (501) staff       (20)    15646 2024-05-16 13:55:20.000000 logos_sdk-0.0.25.dev1/logos_sdk/services/Facebook.py
--rw-r--r--   0 W          (501) staff       (20)     5600 2024-05-16 13:55:20.000000 logos_sdk-0.0.25.dev1/logos_sdk/services/GoogleAds.py
--rw-r--r--   0 W          (501) staff       (20)    12483 2024-05-16 13:55:20.000000 logos_sdk-0.0.25.dev1/logos_sdk/services/GoogleSheets.py
--rw-r--r--   0 W          (501) staff       (20)     1151 2024-05-16 13:55:20.000000 logos_sdk-0.0.25.dev1/logos_sdk/services/MarketMiner.py
--rw-r--r--   0 W          (501) staff       (20)     6129 2024-05-16 13:55:20.000000 logos_sdk-0.0.25.dev1/logos_sdk/services/MerchantCenter.py
--rw-r--r--   0 W          (501) staff       (20)     6899 2024-05-16 13:55:20.000000 logos_sdk-0.0.25.dev1/logos_sdk/services/MicrosoftAdvertising.py
--rw-r--r--   0 W          (501) staff       (20)    11621 2024-05-16 13:55:20.000000 logos_sdk-0.0.25.dev1/logos_sdk/services/Sklik.py
--rw-r--r--   0 W          (501) staff       (20)     1110 2024-05-16 14:19:15.000000 logos_sdk-0.0.25.dev1/logos_sdk/services/__init__.py
-drwxr-xr-x   0 W          (501) staff       (20)        0 2024-05-30 11:26:29.995730 logos_sdk-0.0.25.dev1/logos_sdk.egg-info/
--rw-r--r--   0 W          (501) staff       (20)     9586 2024-05-30 11:26:29.000000 logos_sdk-0.0.25.dev1/logos_sdk.egg-info/PKG-INFO
--rw-r--r--   0 W          (501) staff       (20)      717 2024-05-30 11:26:29.000000 logos_sdk-0.0.25.dev1/logos_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 W          (501) staff       (20)        1 2024-05-30 11:26:29.000000 logos_sdk-0.0.25.dev1/logos_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 W          (501) staff       (20)      135 2024-05-30 11:26:29.000000 logos_sdk-0.0.25.dev1/logos_sdk.egg-info/requires.txt
--rw-r--r--   0 W          (501) staff       (20)       10 2024-05-30 11:26:29.000000 logos_sdk-0.0.25.dev1/logos_sdk.egg-info/top_level.txt
--rw-r--r--   0 W          (501) staff       (20)       79 2024-05-30 11:26:29.996336 logos_sdk-0.0.25.dev1/setup.cfg
--rw-r--r--   0 W          (501) staff       (20)     1194 2024-05-29 12:13:05.000000 logos_sdk-0.0.25.dev1/setup.py
+drwxr-xr-x   0 W          (501) staff       (20)        0 2024-06-03 13:18:01.638735 logos_sdk-0.0.25.dev2/
+-rw-r--r--   0 W          (501) staff       (20)     1061 2024-05-16 14:39:43.000000 logos_sdk-0.0.25.dev2/LICENSE
+-rw-r--r--   0 W          (501) staff       (20)     9586 2024-06-03 13:18:01.638535 logos_sdk-0.0.25.dev2/PKG-INFO
+-rw-r--r--   0 W          (501) staff       (20)     8935 2024-05-30 10:55:15.000000 logos_sdk-0.0.25.dev2/README.md
+drwxr-xr-x   0 W          (501) staff       (20)        0 2024-06-03 13:18:01.632732 logos_sdk-0.0.25.dev2/logos_sdk/
+-rw-r--r--   0 W          (501) staff       (20)      116 2024-05-16 14:06:44.000000 logos_sdk-0.0.25.dev2/logos_sdk/__init__.py
+drwxr-xr-x   0 W          (501) staff       (20)        0 2024-06-03 13:18:01.633936 logos_sdk-0.0.25.dev2/logos_sdk/big_query/
+-rw-r--r--   0 W          (501) staff       (20)     5498 2024-05-20 07:25:33.000000 logos_sdk-0.0.25.dev2/logos_sdk/big_query/BigQuery.py
+-rw-r--r--   0 W          (501) staff       (20)      745 2024-01-08 11:17:31.000000 logos_sdk-0.0.25.dev2/logos_sdk/big_query/__init__.py
+drwxr-xr-x   0 W          (501) staff       (20)        0 2024-06-03 13:18:01.634507 logos_sdk-0.0.25.dev2/logos_sdk/logging/
+-rw-r--r--   0 W          (501) staff       (20)     2557 2024-05-16 14:06:44.000000 logos_sdk-0.0.25.dev2/logos_sdk/logging/LogosLogger.py
+-rw-r--r--   0 W          (501) staff       (20)     2818 2023-09-13 09:34:42.000000 logos_sdk-0.0.25.dev2/logos_sdk/logging/__init__.py
+drwxr-xr-x   0 W          (501) staff       (20)        0 2024-06-03 13:18:01.637940 logos_sdk-0.0.25.dev2/logos_sdk/services/
+-rw-r--r--   0 W          (501) staff       (20)    14319 2024-05-16 14:19:15.000000 logos_sdk-0.0.25.dev2/logos_sdk/services/CampaignManager.py
+-rw-r--r--   0 W          (501) staff       (20)     7036 2024-05-16 14:06:44.000000 logos_sdk-0.0.25.dev2/logos_sdk/services/Collabim.py
+-rw-r--r--   0 W          (501) staff       (20)    15566 2024-05-29 06:52:17.000000 logos_sdk-0.0.25.dev2/logos_sdk/services/DV360.py
+-rw-r--r--   0 W          (501) staff       (20)    15646 2024-05-16 13:55:20.000000 logos_sdk-0.0.25.dev2/logos_sdk/services/Facebook.py
+-rw-r--r--   0 W          (501) staff       (20)     6243 2024-06-03 13:16:23.000000 logos_sdk-0.0.25.dev2/logos_sdk/services/GoogleAds.py
+-rw-r--r--   0 W          (501) staff       (20)    12483 2024-05-16 13:55:20.000000 logos_sdk-0.0.25.dev2/logos_sdk/services/GoogleSheets.py
+-rw-r--r--   0 W          (501) staff       (20)     1151 2024-05-16 13:55:20.000000 logos_sdk-0.0.25.dev2/logos_sdk/services/MarketMiner.py
+-rw-r--r--   0 W          (501) staff       (20)     6129 2024-05-16 13:55:20.000000 logos_sdk-0.0.25.dev2/logos_sdk/services/MerchantCenter.py
+-rw-r--r--   0 W          (501) staff       (20)     6899 2024-05-16 13:55:20.000000 logos_sdk-0.0.25.dev2/logos_sdk/services/MicrosoftAdvertising.py
+-rw-r--r--   0 W          (501) staff       (20)    11621 2024-05-16 13:55:20.000000 logos_sdk-0.0.25.dev2/logos_sdk/services/Sklik.py
+-rw-r--r--   0 W          (501) staff       (20)     1110 2024-05-16 14:19:15.000000 logos_sdk-0.0.25.dev2/logos_sdk/services/__init__.py
+drwxr-xr-x   0 W          (501) staff       (20)        0 2024-06-03 13:18:01.638198 logos_sdk-0.0.25.dev2/logos_sdk.egg-info/
+-rw-r--r--   0 W          (501) staff       (20)     9586 2024-06-03 13:18:01.000000 logos_sdk-0.0.25.dev2/logos_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 W          (501) staff       (20)      717 2024-06-03 13:18:01.000000 logos_sdk-0.0.25.dev2/logos_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 W          (501) staff       (20)        1 2024-06-03 13:18:01.000000 logos_sdk-0.0.25.dev2/logos_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 W          (501) staff       (20)      135 2024-06-03 13:18:01.000000 logos_sdk-0.0.25.dev2/logos_sdk.egg-info/requires.txt
+-rw-r--r--   0 W          (501) staff       (20)       10 2024-06-03 13:18:01.000000 logos_sdk-0.0.25.dev2/logos_sdk.egg-info/top_level.txt
+-rw-r--r--   0 W          (501) staff       (20)       79 2024-06-03 13:18:01.638940 logos_sdk-0.0.25.dev2/setup.cfg
+-rw-r--r--   0 W          (501) staff       (20)     1194 2024-05-29 12:13:05.000000 logos_sdk-0.0.25.dev2/setup.py
```

### Comparing `logos_sdk-0.0.25.dev1/LICENSE` & `logos_sdk-0.0.25.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `logos_sdk-0.0.25.dev1/PKG-INFO` & `logos_sdk-0.0.25.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logos-sdk
-Version: 0.0.25.dev1
+Version: 0.0.25.dev2
 Summary: SDK for Logos platform
 Home-page: https://bitbucket.org/databy/logos-sdk-pip/src/master/
 Author: Databy.io
 Author-email: admin@proficio.cz
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `logos_sdk-0.0.25.dev1/README.md` & `logos_sdk-0.0.25.dev2/README.md`

 * *Files identical despite different names*

### Comparing `logos_sdk-0.0.25.dev1/logos_sdk/big_query/BigQuery.py` & `logos_sdk-0.0.25.dev2/logos_sdk/big_query/BigQuery.py`

 * *Files identical despite different names*

### Comparing `logos_sdk-0.0.25.dev1/logos_sdk/big_query/__init__.py` & `logos_sdk-0.0.25.dev2/logos_sdk/big_query/__init__.py`

 * *Files identical despite different names*

### Comparing `logos_sdk-0.0.25.dev1/logos_sdk/logging/LogosLogger.py` & `logos_sdk-0.0.25.dev2/logos_sdk/logging/LogosLogger.py`

 * *Files identical despite different names*

### Comparing `logos_sdk-0.0.25.dev1/logos_sdk/logging/__init__.py` & `logos_sdk-0.0.25.dev2/logos_sdk/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `logos_sdk-0.0.25.dev1/logos_sdk/services/CampaignManager.py` & `logos_sdk-0.0.25.dev2/logos_sdk/services/CampaignManager.py`

 * *Files identical despite different names*

### Comparing `logos_sdk-0.0.25.dev1/logos_sdk/services/Collabim.py` & `logos_sdk-0.0.25.dev2/logos_sdk/services/Collabim.py`

 * *Files identical despite different names*

### Comparing `logos_sdk-0.0.25.dev1/logos_sdk/services/DV360.py` & `logos_sdk-0.0.25.dev2/logos_sdk/services/DV360.py`

 * *Files identical despite different names*

### Comparing `logos_sdk-0.0.25.dev1/logos_sdk/services/Facebook.py` & `logos_sdk-0.0.25.dev2/logos_sdk/services/Facebook.py`

 * *Files identical despite different names*

### Comparing `logos_sdk-0.0.25.dev1/logos_sdk/services/GoogleAds.py` & `logos_sdk-0.0.25.dev2/logos_sdk/services/GoogleAds.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from requests import request
+from requests.exceptions import Timeout
 from typing import List, Union, Dict
 from logos_sdk.services import get_headers
 from http import HTTPStatus
 from dotenv import load_dotenv
 import os
+import time
+import random
 
 
 class GoogleAdsServiceException(Exception):
     pass
 
 
 class GoogleAdsService:
@@ -15,14 +18,26 @@
         load_dotenv()
         self._URL = url or os.environ.get("GOOGLE_ADS_SERVICE_PATH")
         self._SEARCH_STREAM = self._URL + "/search-stream"
         self._SEARCH = self._URL + "/search"
         self._EXCLUDE_FOR_ACCOUNT = self._URL + "/exclude-for-account"
         self._EXCLUDE_FOR_AD_GROUP = self._URL + "/exclude-for-ad-group"
 
+    @staticmethod
+    def fetch_with_retry_on_timeout(url, json, headers):
+        for attempt in range(5):
+            try:
+                return request("post", url, json=json, headers=headers, timeout=25)
+            except Timeout:
+                delay = 2 * (2 ** attempt) + random.randint(0, 9)
+                print(f"there was a timeout when contacting the service, going to sleep for {delay} seconds")
+                time.sleep(delay)
+
+        raise Exception("The service is not able to reply within 30 seconds.")
+
     def search_stream(
         self,
         query: str,
         queried_account_id: str,
         secret_id: str,
     ) -> List[Union[List, Dict]]:
         """
@@ -34,15 +49,15 @@
         body = {
             "query": query,
             "queried_account_id": queried_account_id,
             "secret_id": secret_id,
         }
 
         header = get_headers(self._SEARCH_STREAM)
-        response = request("post", url=self._SEARCH_STREAM, json=body, headers=header)
+        response = self.fetch_with_retry_on_timeout(url=self._SEARCH_STREAM, json=body, headers=header)
 
         if response.status_code == HTTPStatus.OK:
             service_response = response.json()
             return service_response["data"]
         else:
             raise GoogleAdsServiceException(response.content)
 
@@ -65,15 +80,15 @@
             "queried_account_id": queried_account_id,
             "secret_id": secret_id,
             "page_token": None,
             "page_size": page_size,
         }
 
         header = get_headers(self._SEARCH)
-        response = request("post", url=self._SEARCH, json=body, headers=header)
+        response = self.fetch_with_retry_on_timeout(url=self._SEARCH, json=body, headers=header)
 
         if response.status_code != HTTPStatus.OK:
             raise GoogleAdsServiceException(response.content)
 
         service_response = response.json()
         yield service_response["data"]["results"]
```

### Comparing `logos_sdk-0.0.25.dev1/logos_sdk/services/GoogleSheets.py` & `logos_sdk-0.0.25.dev2/logos_sdk/services/GoogleSheets.py`

 * *Files identical despite different names*

### Comparing `logos_sdk-0.0.25.dev1/logos_sdk/services/MarketMiner.py` & `logos_sdk-0.0.25.dev2/logos_sdk/services/MarketMiner.py`

 * *Files identical despite different names*

### Comparing `logos_sdk-0.0.25.dev1/logos_sdk/services/MerchantCenter.py` & `logos_sdk-0.0.25.dev2/logos_sdk/services/MerchantCenter.py`

 * *Files identical despite different names*

### Comparing `logos_sdk-0.0.25.dev1/logos_sdk/services/MicrosoftAdvertising.py` & `logos_sdk-0.0.25.dev2/logos_sdk/services/MicrosoftAdvertising.py`

 * *Files identical despite different names*

### Comparing `logos_sdk-0.0.25.dev1/logos_sdk/services/Sklik.py` & `logos_sdk-0.0.25.dev2/logos_sdk/services/Sklik.py`

 * *Files identical despite different names*

### Comparing `logos_sdk-0.0.25.dev1/logos_sdk/services/__init__.py` & `logos_sdk-0.0.25.dev2/logos_sdk/services/__init__.py`

 * *Files identical despite different names*

### Comparing `logos_sdk-0.0.25.dev1/logos_sdk.egg-info/PKG-INFO` & `logos_sdk-0.0.25.dev2/logos_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logos-sdk
-Version: 0.0.25.dev1
+Version: 0.0.25.dev2
 Summary: SDK for Logos platform
 Home-page: https://bitbucket.org/databy/logos-sdk-pip/src/master/
 Author: Databy.io
 Author-email: admin@proficio.cz
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `logos_sdk-0.0.25.dev1/logos_sdk.egg-info/SOURCES.txt` & `logos_sdk-0.0.25.dev2/logos_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logos_sdk-0.0.25.dev1/setup.py` & `logos_sdk-0.0.25.dev2/setup.py`

 * *Files identical despite different names*

