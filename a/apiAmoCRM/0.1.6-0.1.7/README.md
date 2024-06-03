# Comparing `tmp/apiamocrm-0.1.6.tar.gz` & `tmp/apiamocrm-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apiamocrm-0.1.6.tar", last modified: Fri May 31 05:30:00 2024, max compression
+gzip compressed data, was "apiamocrm-0.1.7.tar", last modified: Mon Jun  3 08:32:19 2024, max compression
```

## Comparing `apiamocrm-0.1.6.tar` & `apiamocrm-0.1.7.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 05:30:00.772991 apiamocrm-0.1.6/
--rw-rw-rw-   0        0        0      438 2024-05-31 05:30:00.770997 apiamocrm-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-30 09:48:06.000000 apiamocrm-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 05:30:00.753488 apiamocrm-0.1.6/amoApi/
--rw-rw-rw-   0        0        0     6353 2024-05-29 09:02:42.000000 apiamocrm-0.1.6/amoApi/API.py
--rw-rw-rw-   0        0        0        0 2024-05-30 10:16:29.000000 apiamocrm-0.1.6/amoApi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 05:30:00.755995 apiamocrm-0.1.6/amoApi/amoEntities/
--rw-rw-rw-   0        0        0     1612 2024-05-28 06:33:36.000000 apiamocrm-0.1.6/amoApi/amoEntities/Contact.py
--rw-rw-rw-   0        0        0     3338 2024-05-29 08:28:40.000000 apiamocrm-0.1.6/amoApi/amoEntities/Lead.py
--rw-rw-rw-   0        0        0        0 2024-05-30 10:19:41.000000 apiamocrm-0.1.6/amoApi/amoEntities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 05:30:00.762980 apiamocrm-0.1.6/amoChatApi/
--rw-rw-rw-   0        0        0     5038 2024-05-30 03:55:43.000000 apiamocrm-0.1.6/amoChatApi/API.py
--rw-rw-rw-   0        0        0      138 2024-05-28 08:25:22.000000 apiamocrm-0.1.6/amoChatApi/Message.py
--rw-rw-rw-   0        0        0     1876 2024-05-29 07:38:48.000000 apiamocrm-0.1.6/amoChatApi/Payload.py
--rw-rw-rw-   0        0        0      384 2024-05-28 08:33:26.000000 apiamocrm-0.1.6/amoChatApi/TextMessage.py
--rw-rw-rw-   0        0        0        0 2024-05-30 10:16:39.000000 apiamocrm-0.1.6/amoChatApi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 05:30:00.769999 apiamocrm-0.1.6/apiAmoCRM.egg-info/
--rw-rw-rw-   0        0        0      438 2024-05-31 05:30:00.000000 apiamocrm-0.1.6/apiAmoCRM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      414 2024-05-31 05:30:00.000000 apiamocrm-0.1.6/apiAmoCRM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 05:30:00.000000 apiamocrm-0.1.6/apiAmoCRM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-31 05:30:00.000000 apiamocrm-0.1.6/apiAmoCRM.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-31 05:30:00.000000 apiamocrm-0.1.6/apiAmoCRM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 05:30:00.772991 apiamocrm-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      633 2024-05-31 05:29:59.000000 apiamocrm-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:32:19.047186 apiamocrm-0.1.7/
+-rw-rw-rw-   0        0        0      438 2024-06-03 08:32:19.045024 apiamocrm-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-30 09:48:06.000000 apiamocrm-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 08:32:19.020634 apiamocrm-0.1.7/amoApi/
+-rw-rw-rw-   0        0        0     6486 2024-06-03 04:08:24.000000 apiamocrm-0.1.7/amoApi/API.py
+-rw-rw-rw-   0        0        0        0 2024-05-30 10:16:29.000000 apiamocrm-0.1.7/amoApi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:32:19.025140 apiamocrm-0.1.7/amoApi/amoEntities/
+-rw-rw-rw-   0        0        0     3427 2024-06-03 03:55:35.000000 apiamocrm-0.1.7/amoApi/amoEntities/Contact.py
+-rw-rw-rw-   0        0        0     3318 2024-06-03 03:51:25.000000 apiamocrm-0.1.7/amoApi/amoEntities/Lead.py
+-rw-rw-rw-   0        0        0        0 2024-05-30 10:19:41.000000 apiamocrm-0.1.7/amoApi/amoEntities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:32:19.034150 apiamocrm-0.1.7/amoChatApi/
+-rw-rw-rw-   0        0        0     5109 2024-06-03 08:28:50.000000 apiamocrm-0.1.7/amoChatApi/API.py
+-rw-rw-rw-   0        0        0      138 2024-06-03 04:11:23.000000 apiamocrm-0.1.7/amoChatApi/AbstractMessage.py
+-rw-rw-rw-   0        0        0     2011 2024-06-03 08:29:32.000000 apiamocrm-0.1.7/amoChatApi/Payload.py
+-rw-rw-rw-   0        0        0      994 2024-06-03 08:30:59.000000 apiamocrm-0.1.7/amoChatApi/PhotoMessage.py
+-rw-rw-rw-   0        0        0      392 2024-06-03 04:11:18.000000 apiamocrm-0.1.7/amoChatApi/TextMessage.py
+-rw-rw-rw-   0        0        0        0 2024-05-30 10:16:39.000000 apiamocrm-0.1.7/amoChatApi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:32:19.044028 apiamocrm-0.1.7/apiAmoCRM.egg-info/
+-rw-rw-rw-   0        0        0      438 2024-06-03 08:32:18.000000 apiamocrm-0.1.7/apiAmoCRM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      449 2024-06-03 08:32:18.000000 apiamocrm-0.1.7/apiAmoCRM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 08:32:18.000000 apiamocrm-0.1.7/apiAmoCRM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-06-03 08:32:18.000000 apiamocrm-0.1.7/apiAmoCRM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-06-03 08:32:18.000000 apiamocrm-0.1.7/apiAmoCRM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 08:32:19.047186 apiamocrm-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      633 2024-06-03 04:09:01.000000 apiamocrm-0.1.7/setup.py
```

### Comparing `apiamocrm-0.1.6/amoApi/API.py` & `apiamocrm-0.1.7/amoApi/API.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import requests
 from amoApi.amoEntities.Lead import Lead
 import json
 from typing import List
+from amoApi.amoEntities.Contact import Contact
 
 
 class API:
     def __init__(self, token:str, url:str):
         self._auth(token, url)
 
     def _delete(self, method: str, headers=None, body=None) -> json:
@@ -108,16 +109,18 @@
         body[0]["_embedded"] = {}
         body[0]["_embedded"]["contacts"] = contacts
         headers = {"Authorization": "Bearer " + self._token}
         r = requests.post(self._url + "leads/complex", json=body, headers=headers)
         lead = Lead()
         lead.id = json.loads(r.text)[0]["id"]
         return lead
-    def get_contact(self, id:int, params:dict):
-        return self._get("contacts/"+str(id), parameters=params)
+    def get_contact(self, id:int, params:dict = {}):
+        params["with"] = "leads"
+        contact = Contact(self, self._get("contacts/" + str(id), parameters=params))
+        return contact
     def get_contact_links(self, contacts_id: List[int] = None, chats_id: List[str] = None):
         params = {}
         if not contacts_id is None:
             params["contact_id"] = contacts_id
         if not chats_id is None:
             params["chat_id"] = chats_id
         return self._get("contacts/chats", parameters=params)
@@ -157,8 +160,8 @@
     def create_source(self, name:str, id:str):
         body = [{"name":name, "external_id": id}]
         return self._post("sources", body=body)
     def delete_source(self, id:int):
         body = [{"id":id}]
         return self._delete("sources", body=body)
     def get_sources(self):
-        return self._get("sources")
+        return self._get("sources")
```

### Comparing `apiamocrm-0.1.6/amoApi/amoEntities/Lead.py` & `apiamocrm-0.1.7/amoApi/amoEntities/Lead.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from amoApi.amoEntities.Contact import Contact
 import json
 from typing import List
 class Lead:
-    def __init__(self, api=None):
-        self._json_lead = {}
+    def __init__(self, api=None, json_lead:json = {}):
+        self._json_lead = json_lead
         self.api = api
 
     def add_text_note(self, text: str):
         self.api.add_lead_text_note(lead=self, text=text)
 
     def from_json(self, json: json):
         self._json_lead = json
```

### Comparing `apiamocrm-0.1.6/amoChatApi/API.py` & `apiamocrm-0.1.7/amoChatApi/API.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,8 +111,10 @@
             'X-Signature': signature,
         }
         response = requests.post(send_or_edit_message_url, data=request_body, headers=headers)
         return response
 
     def create_new_text_message(self):
         return Payload(self)
+    def create_new_photo_message(self):
+        return Payload(self)
```

### Comparing `apiamocrm-0.1.6/amoChatApi/Payload.py` & `apiamocrm-0.1.7/amoChatApi/Payload.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import time
 from amoChatApi.TextMessage import TextMessage
+from amoChatApi.PhotoMessage import PhotoMessage
 class Payload:
     def __init__(self, api, type = "text"):
         self._json_payload = {"payload":{}}
         self.set_timestamp(int(time.time()))
         self.api = api
         self.set_silent(False)
         self.set_event_type("new_message")
         if type == "text":
             self.message:TextMessage = TextMessage()
+        if type == "photo":
+            self.message:PhotoMessage = PhotoMessage()
     def set_event_type(self, type:str):
         self._json_payload["event_type"] = type
     def set_timestamp(self, timestamp:int):
         self._json_payload["payload"]["timestamp"] = timestamp
         self.set_msec_timestamp(timestamp*1000)
     def set_msec_timestamp(self, msec_timestamp:int):
         self._json_payload["payload"]["msec_timestamp"] = msec_timestamp
```

### Comparing `apiamocrm-0.1.6/setup.py` & `apiamocrm-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='apiAmoCRM',
-    version='0.1.6',
+    version='0.1.7',
     packages=find_packages(),
     install_requires=[
         "requests",
     ],
     author='wlovem',
     author_email='wlovemrock@gmail.com',
     description='Api for amoCRM',
```

