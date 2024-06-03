# Comparing `tmp/cycls-0.0.2.2.tar.gz` & `tmp/cycls-0.0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cycls-0.0.2.2.tar", max compression
+gzip compressed data, was "cycls-0.0.2.3.tar", max compression
```

## Comparing `cycls-0.0.2.2.tar` & `cycls-0.0.2.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1073 2023-11-09 08:25:32.798599 cycls-0.0.2.2/LICENSE
--rw-r--r--   0        0        0     2204 2024-05-02 06:45:15.624431 cycls-0.0.2.2/README.md
--rw-r--r--   0        0        0      663 2024-05-29 22:42:44.524280 cycls-0.0.2.2/cycls/UI.py
--rw-r--r--   0        0        0      171 2024-06-02 15:40:50.122993 cycls-0.0.2.2/cycls/__init__.py
--rw-r--r--   0        0        0     7105 2024-06-02 16:24:41.473630 cycls-0.0.2.2/cycls/client.py
--rw-r--r--   0        0        0      785 2024-06-02 15:40:50.123439 cycls-0.0.2.2/cycls/configuration.py
--rw-r--r--   0        0        0      160 2024-05-18 09:30:48.833639 cycls-0.0.2.2/cycls/settings.py
--rw-r--r--   0        0        0      120 2024-05-02 06:45:15.626692 cycls-0.0.2.2/cycls/static.py
--rw-r--r--   0        0        0     7293 2024-06-02 18:40:34.534018 cycls-0.0.2.2/cycls/typings.py
--rw-r--r--   0        0        0      846 2024-06-02 18:45:56.503225 cycls-0.0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3072 1970-01-01 00:00:00.000000 cycls-0.0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-11-09 08:25:32.798599 cycls-0.0.2.3/LICENSE
+-rw-r--r--   0        0        0     2204 2024-05-02 06:45:15.624431 cycls-0.0.2.3/README.md
+-rw-r--r--   0        0        0      663 2024-05-29 22:42:44.524280 cycls-0.0.2.3/cycls/UI.py
+-rw-r--r--   0        0        0      171 2024-06-02 15:40:50.122993 cycls-0.0.2.3/cycls/__init__.py
+-rw-r--r--   0        0        0     7105 2024-06-02 16:24:41.473630 cycls-0.0.2.3/cycls/client.py
+-rw-r--r--   0        0        0      785 2024-06-02 15:40:50.123439 cycls-0.0.2.3/cycls/configuration.py
+-rw-r--r--   0        0        0      160 2024-05-18 09:30:48.833639 cycls-0.0.2.3/cycls/settings.py
+-rw-r--r--   0        0        0      120 2024-05-02 06:45:15.626692 cycls-0.0.2.3/cycls/static.py
+-rw-r--r--   0        0        0     6843 2024-06-03 00:19:36.572709 cycls-0.0.2.3/cycls/typings.py
+-rw-r--r--   0        0        0      846 2024-06-03 00:20:43.116227 cycls-0.0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3072 1970-01-01 00:00:00.000000 cycls-0.0.2.3/PKG-INFO
```

### Comparing `cycls-0.0.2.2/LICENSE` & `cycls-0.0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cycls-0.0.2.2/README.md` & `cycls-0.0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `cycls-0.0.2.2/cycls/UI.py` & `cycls-0.0.2.3/cycls/UI.py`

 * *Files identical despite different names*

### Comparing `cycls-0.0.2.2/cycls/client.py` & `cycls-0.0.2.3/cycls/client.py`

 * *Files identical despite different names*

### Comparing `cycls-0.0.2.2/cycls/configuration.py` & `cycls-0.0.2.3/cycls/configuration.py`

 * *Files identical despite different names*

### Comparing `cycls-0.0.2.2/cycls/typings.py` & `cycls-0.0.2.3/cycls/typings.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from datetime import datetime
 from socketio import AsyncClient, Client  # type: ignore[import-untyped]
 import uuid
 import httpx
 import json
 
 
+
 MessageContent = TypeVar("MessageContent", bound=UI.Text | UI.Image | None)
 
 
 class InputTypeHint(Enum):
     EMPTY = auto()
     MESSAGE = auto()
     CONVERSATION_ID = auto()
@@ -136,48 +137,43 @@
         httpx.post(self.url + '/chat_app/send_message', data=json.dumps(data))
 
 
 class AsyncSendStream(AsyncSendBase):
     async def text(self, message_stream: AsyncGenerator):
         id = str(uuid.uuid4())
         timeout = httpx.Timeout(120, connect=60)
-        async with httpx.AsyncClient(timeout=timeout) as client:
-            async with client.stream("POST", self.url+'/chat_app/send_message') as response:
-                async for chunk in message_stream:
-                    try:
-                        await response.aclose()
-                        data = self.send_message_data(UI.Text(text=chunk), id, True)
-                        async with client.stream("POST", self.url+'/chat_app/send_message', data=json.dumps(data) ) as response:
-                            pass
-                    except Exception as e:
-                        print(f'we got theis error {e}')
-                        data = self.send_message_data(None, id, True, "error")
-                        async with client.stream("POST", self.url+'/chat_app/send_message', data=json.dumps(data) ) as response:
-                            break
+        transport = httpx.AsyncHTTPTransport(retries=1)
+        async with httpx.AsyncClient(timeout=timeout, transport=transport) as client:
+            async for chunk in message_stream:
+                try:
+                    data = self.send_message_data(UI.Text(text=chunk), id, True)
+                    await client.post(self.url+'/chat_app/send_message', json=data)
+                except Exception as e:
+                    print(f'we got theis error {e}')
+                    data = self.send_message_data(None, id, True, "error")
+                    await client.post(self.url+'/chat_app/send_message', json=data)
+                    break
         return True, id
 
 
 
 class SyncSendStream(SendBase):
     def text(self, message_stream: Generator):
         id = str(uuid.uuid4())
         timeout = httpx.Timeout(120, connect=60)
-        with httpx.Client(timeout=timeout) as client:
-            with client.stream("POST", self.url+'/chat_app/send_message') as response:
-                for chunk in message_stream:
-                    try:
-                        response.close()
-                        data = self.send_message_data(UI.Text(text=chunk), id, True)
-                        with client.stream("POST", self.url+'/chat_app/send_message', data=json.dumps(data)) as response:
-                            pass
-                    except Exception as e:
-                        data = self.send_message_data(None, id, True, "error")
-                        print(f'we got an error {e}')
-                        with client.stream("POST", self.url+'/chat_app/send_message', data=json.dumps(data)) as response:
-                            break
+        transport = httpx.HTTPTransport(retries=1)
+        with httpx.Client(timeout=timeout, transport=transport) as client:
+            for chunk in message_stream:
+                try:
+                    data = self.send_message_data(UI.Text(text=chunk), id, True)
+                    client.post(self.url+'/chat_app/send_message', json=data)
+                except Exception as e:
+                    print(f'we got theis error {e}')
+                    data = self.send_message_data(None, id, True, "error")
+                    client.post(self.url+'/chat_app/send_message', json=data)
         return True, id
 
 
 
 class UserMessage(BaseModel):
     message: Message
     session: ConversationSession
```

### Comparing `cycls-0.0.2.2/pyproject.toml` & `cycls-0.0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cycls"
-version = "0.0.2.2"
+version = "0.0.2.3"
 description = "Publish your chat app with cycls"
 authors = ["Khalid Alrasheed <khalid@cycls.io>"]
 packages = [{ include = "cycls" }]
 license = "MIT"
 readme = "README.md"
 homepage = "https://www.cycls.com/"
 documentation = "https://docs.cycls.com/"
```

### Comparing `cycls-0.0.2.2/PKG-INFO` & `cycls-0.0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cycls
-Version: 0.0.2.2
+Version: 0.0.2.3
 Summary: Publish your chat app with cycls
 Home-page: https://www.cycls.com/
 License: MIT
 Keywords: AI,chat
 Author: Khalid Alrasheed
 Author-email: khalid@cycls.io
 Requires-Python: >=3.8,<4.0
```

