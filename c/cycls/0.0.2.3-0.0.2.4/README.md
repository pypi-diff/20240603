# Comparing `tmp/cycls-0.0.2.3.tar.gz` & `tmp/cycls-0.0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cycls-0.0.2.3.tar", max compression
+gzip compressed data, was "cycls-0.0.2.4.tar", max compression
```

## Comparing `cycls-0.0.2.3.tar` & `cycls-0.0.2.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1073 2023-11-09 08:25:32.798599 cycls-0.0.2.3/LICENSE
--rw-r--r--   0        0        0     2204 2024-05-02 06:45:15.624431 cycls-0.0.2.3/README.md
--rw-r--r--   0        0        0      663 2024-05-29 22:42:44.524280 cycls-0.0.2.3/cycls/UI.py
--rw-r--r--   0        0        0      171 2024-06-02 15:40:50.122993 cycls-0.0.2.3/cycls/__init__.py
--rw-r--r--   0        0        0     7105 2024-06-02 16:24:41.473630 cycls-0.0.2.3/cycls/client.py
--rw-r--r--   0        0        0      785 2024-06-02 15:40:50.123439 cycls-0.0.2.3/cycls/configuration.py
--rw-r--r--   0        0        0      160 2024-05-18 09:30:48.833639 cycls-0.0.2.3/cycls/settings.py
--rw-r--r--   0        0        0      120 2024-05-02 06:45:15.626692 cycls-0.0.2.3/cycls/static.py
--rw-r--r--   0        0        0     6843 2024-06-03 00:19:36.572709 cycls-0.0.2.3/cycls/typings.py
--rw-r--r--   0        0        0      846 2024-06-03 00:20:43.116227 cycls-0.0.2.3/pyproject.toml
--rw-r--r--   0        0        0     3072 1970-01-01 00:00:00.000000 cycls-0.0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-11-09 08:25:32.798599 cycls-0.0.2.4/LICENSE
+-rw-r--r--   0        0        0     2204 2024-05-02 06:45:15.624431 cycls-0.0.2.4/README.md
+-rw-r--r--   0        0        0      663 2024-05-29 22:42:44.524280 cycls-0.0.2.4/cycls/UI.py
+-rw-r--r--   0        0        0      171 2024-06-02 15:40:50.122993 cycls-0.0.2.4/cycls/__init__.py
+-rw-r--r--   0        0        0     7105 2024-06-02 16:24:41.473630 cycls-0.0.2.4/cycls/client.py
+-rw-r--r--   0        0        0      785 2024-06-02 15:40:50.123439 cycls-0.0.2.4/cycls/configuration.py
+-rw-r--r--   0        0        0      160 2024-05-18 09:30:48.833639 cycls-0.0.2.4/cycls/settings.py
+-rw-r--r--   0        0        0      120 2024-05-02 06:45:15.626692 cycls-0.0.2.4/cycls/static.py
+-rw-r--r--   0        0        0     8162 2024-06-03 01:43:01.974237 cycls-0.0.2.4/cycls/typings.py
+-rw-r--r--   0        0        0      846 2024-06-03 01:43:57.972473 cycls-0.0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     3072 1970-01-01 00:00:00.000000 cycls-0.0.2.4/PKG-INFO
```

### Comparing `cycls-0.0.2.3/LICENSE` & `cycls-0.0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cycls-0.0.2.3/README.md` & `cycls-0.0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `cycls-0.0.2.3/cycls/UI.py` & `cycls-0.0.2.4/cycls/UI.py`

 * *Files identical despite different names*

### Comparing `cycls-0.0.2.3/cycls/client.py` & `cycls-0.0.2.4/cycls/client.py`

 * *Files identical despite different names*

### Comparing `cycls-0.0.2.3/cycls/configuration.py` & `cycls-0.0.2.4/cycls/configuration.py`

 * *Files identical despite different names*

### Comparing `cycls-0.0.2.3/cycls/typings.py` & `cycls-0.0.2.4/cycls/typings.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Any, TypeVar, Generator, Generic, AsyncGenerator
 from cycls import UI
 from datetime import datetime
 from socketio import AsyncClient, Client  # type: ignore[import-untyped]
 import uuid
 import httpx
 import json
+import time
 
 
 
 MessageContent = TypeVar("MessageContent", bound=UI.Text | UI.Image | None)
 
 
 class InputTypeHint(Enum):
@@ -134,39 +135,73 @@
         id = str(uuid.uuid4())
         content = UI.Text(text=message)
         data = self.send_message_data(content=content, id=id)
         httpx.post(self.url + '/chat_app/send_message', data=json.dumps(data))
 
 
 class AsyncSendStream(AsyncSendBase):
+    async def __fast_generator(self, message_stream: AsyncGenerator, index_limit:int=12, time_limit:float=2.0):
+        total_time, index, text = 0., 0, ""
+        previous_time = time.perf_counter()
+        text = ''
+        async for message in message_stream:
+            current_time = time.perf_counter()
+            time_diff = current_time - previous_time
+            text += message
+            index += 1
+            total_time += time_diff
+            if (total_time >= index_limit) | (index >= time_limit):
+                yield text
+                total_time, index, text = 0., 0, ""
+        if text:
+            yield text
+
+
+
     async def text(self, message_stream: AsyncGenerator):
         id = str(uuid.uuid4())
         timeout = httpx.Timeout(120, connect=60)
         transport = httpx.AsyncHTTPTransport(retries=1)
         async with httpx.AsyncClient(timeout=timeout, transport=transport) as client:
-            async for chunk in message_stream:
+            async for chunk in self.__fast_generator(message_stream):
                 try:
                     data = self.send_message_data(UI.Text(text=chunk), id, True)
                     await client.post(self.url+'/chat_app/send_message', json=data)
                 except Exception as e:
                     print(f'we got theis error {e}')
                     data = self.send_message_data(None, id, True, "error")
                     await client.post(self.url+'/chat_app/send_message', json=data)
                     break
         return True, id
 
 
 
 class SyncSendStream(SendBase):
+    def __fast_generator(self, message_stream: Generator, index_limit:int=12, time_limit:float=2.0):
+        total_time, index, text = 0., 0, ""
+        previous_time = time.perf_counter()
+        text = ''
+        for message in message_stream:
+            current_time = time.perf_counter()
+            time_diff = current_time - previous_time
+            text += message
+            index += 1
+            total_time += time_diff
+            if (total_time >= time_limit) | (index >= index_limit):
+                yield text
+                total_time, index, text = 0., 0, ""
+        if text:
+            yield text
+
     def text(self, message_stream: Generator):
         id = str(uuid.uuid4())
         timeout = httpx.Timeout(120, connect=60)
         transport = httpx.HTTPTransport(retries=1)
         with httpx.Client(timeout=timeout, transport=transport) as client:
-            for chunk in message_stream:
+            for chunk in self.__fast_generator(message_stream):
                 try:
                     data = self.send_message_data(UI.Text(text=chunk), id, True)
                     client.post(self.url+'/chat_app/send_message', json=data)
                 except Exception as e:
                     print(f'we got theis error {e}')
                     data = self.send_message_data(None, id, True, "error")
                     client.post(self.url+'/chat_app/send_message', json=data)
```

### Comparing `cycls-0.0.2.3/pyproject.toml` & `cycls-0.0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cycls"
-version = "0.0.2.3"
+version = "0.0.2.4"
 description = "Publish your chat app with cycls"
 authors = ["Khalid Alrasheed <khalid@cycls.io>"]
 packages = [{ include = "cycls" }]
 license = "MIT"
 readme = "README.md"
 homepage = "https://www.cycls.com/"
 documentation = "https://docs.cycls.com/"
```

### Comparing `cycls-0.0.2.3/PKG-INFO` & `cycls-0.0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cycls
-Version: 0.0.2.3
+Version: 0.0.2.4
 Summary: Publish your chat app with cycls
 Home-page: https://www.cycls.com/
 License: MIT
 Keywords: AI,chat
 Author: Khalid Alrasheed
 Author-email: khalid@cycls.io
 Requires-Python: >=3.8,<4.0
```

