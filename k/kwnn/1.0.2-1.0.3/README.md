# Comparing `tmp/kwnn-1.0.2.tar.gz` & `tmp/kwnn-1.0.3.tar.gz`

## Comparing `kwnn-1.0.2.tar` & `kwnn-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 kwnn-1.0.2/src/kwnn/__init__.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 kwnn-1.0.2/src/kwnn/_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kwnn-1.0.2/src/kwnn/_models.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 kwnn-1.0.2/src/kwnn/_resource.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 kwnn-1.0.2/src/kwnn/resources/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 kwnn-1.0.2/src/kwnn/resources/chat/__init__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 kwnn-1.0.2/src/kwnn/resources/chat/chat.py
--rw-r--r--   0        0        0     6048 2020-02-02 00:00:00.000000 kwnn-1.0.2/src/kwnn/resources/chat/completions.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 kwnn-1.0.2/src/kwnn/types/__init__.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 kwnn-1.0.2/src/kwnn/types/chat/__init__.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 kwnn-1.0.2/src/kwnn/types/chat/chat_completion.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 kwnn-1.0.2/src/kwnn/types/chat/chat_completion_chunk.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 kwnn-1.0.2/tests/test.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 kwnn-1.0.2/.gitignore
--rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 kwnn-1.0.2/LICENSE
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 kwnn-1.0.2/README.md
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 kwnn-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 kwnn-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 kwnn-1.0.3/src/kwnn/__init__.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 kwnn-1.0.3/src/kwnn/_client.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 kwnn-1.0.3/src/kwnn/_exception.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kwnn-1.0.3/src/kwnn/_models.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 kwnn-1.0.3/src/kwnn/_resource.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 kwnn-1.0.3/src/kwnn/resources/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 kwnn-1.0.3/src/kwnn/resources/chat/__init__.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 kwnn-1.0.3/src/kwnn/resources/chat/chat.py
+-rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 kwnn-1.0.3/src/kwnn/resources/chat/completions.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 kwnn-1.0.3/src/kwnn/types/__init__.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 kwnn-1.0.3/src/kwnn/types/chat/__init__.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 kwnn-1.0.3/src/kwnn/types/chat/chat_completion.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 kwnn-1.0.3/src/kwnn/types/chat/chat_completion_chunk.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 kwnn-1.0.3/tests/test.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 kwnn-1.0.3/.gitignore
+-rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 kwnn-1.0.3/LICENSE
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 kwnn-1.0.3/README.md
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 kwnn-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 kwnn-1.0.3/PKG-INFO
```

### Comparing `kwnn-1.0.2/src/kwnn/__init__.py` & `kwnn-1.0.3/src/kwnn/__init__.py`

 * *Files identical despite different names*

### Comparing `kwnn-1.0.2/src/kwnn/resources/chat/completions.py` & `kwnn-1.0.3/src/kwnn/resources/chat/completions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,17 @@
-from typing import overload, Union, Generator, Optional
+from typing import (
+    # overload,
+    Union,
+    Generator,
+    Optional,
+)
 from typing_extensions import Literal
 from ..._resource import SyncAPIResource
 from ...types.chat import ChatCompletion, ChatCompletionChunk
+from ..._exception import KwnnException
 
 # from openai._utils import required_args
 import json
 import httpx
 
 
 class Completions(SyncAPIResource):
@@ -30,65 +36,82 @@
 
     def create(
         self,
         *,
         cid: Optional[str] = None,
         content: str,
         stream: Literal[True, False] = False,
-    ):
+    ) -> Union[ChatCompletion, Generator[ChatCompletionChunk, None, None]]:
         try:
             data = {"cid": cid, "content": content, "stream": stream}
             if not cid:
                 del data["cid"]
 
             if stream:
-                return self._create_stream(data)
+                return self._createChatCompletionChunk(data)
             else:
-                return self._create_single_response(data)
+                return self._createChatCompletion(data)
+        except KwnnException as e:
+            raise e
         except Exception as e:
             raise e
 
-    def _create_stream(self, data) -> Generator[ChatCompletionChunk, None, None]:
+    def _createChatCompletionChunk(
+        self, data
+    ) -> Generator[ChatCompletionChunk, None, None]:
         with self._client._request.stream(
             "POST",
-            "api/v1/chat",
+            "/chat",
             json=data,
         ) as response:
+            self._error(response, stream=True)
             for chunk in response.iter_bytes():
                 chunk = chunk.decode("utf-8")
-                chunk = json.loads(chunk)
 
-                if chunk.get("code", None) is None:
-                    raise Exception("Invalid response")
-                if chunk.get("code") > 0:
-                    raise Exception(chunk.get("message"))
+                json_response = json.loads(chunk)
+                self._app_error(json_response, response)
 
-                chunk = chunk.get("data")
+                chunk = json_response.get("data")
 
                 yield ChatCompletionChunk(**chunk)
 
-    def _create_single_response(self, data) -> ChatCompletion:
+    def _createChatCompletion(self, data) -> ChatCompletion:
         response = self._client._request.post(
-            "/api/v1/chat",
+            "/chat",
             json=data,
         )
 
-        if response.status_code != httpx.codes.OK:
-            raise Exception(response.text)
+        self._error(response)
 
-        response = response.json()
-        if response.get("code", None) is None:
-            raise Exception("Invalid response")
-        if response.get("code") > 0:
-            raise Exception(response.get("message"))
+        json_response = response.json()
+        self._app_error(json_response, response)
 
-        response = response.get("data")
+        response = json_response.get("data")
 
         return ChatCompletion(**response)
 
+    def _error(self, response, stream: bool = False):
+        if response.status_code != httpx.codes.OK:
+            try:
+                json_response = response.json()
+                self._app_error(json_response, response)
+            except KwnnException as e:
+                raise e
+            except Exception:
+                pass
+
+            if not stream:
+                raise Exception(response.text)
+
+    def _app_error(self, json_response, response):
+        if json_response.get("code", None) is None:
+            raise KwnnException(response.status_code, response.text)
+        if json_response.get("code") > 0:
+            raise KwnnException(json_response.get("code"), json_response.get("message"))
+
     # def create(
     #     self,
     #     *,
     #     cid: Optional[str] = None,
     #     content: str,
     #     stream: bool = False,
     # ):
```

### Comparing `kwnn-1.0.2/.gitignore` & `kwnn-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `kwnn-1.0.2/LICENSE` & `kwnn-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kwnn-1.0.2/README.md` & `kwnn-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `kwnn-1.0.2/pyproject.toml` & `kwnn-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "kwnn"
-version = "1.0.2"
+version = "1.0.3"
 authors = [{ name = "Jimmy zou", email = "author@example.com" }]
 description = "kwniu.com ai sdk"
 readme = "README.md"
 license = "Apache-2.0"
 requires-python = ">= 3.7.1"
 dependencies = [
     "httpx>=0.23.0, <1",
```

### Comparing `kwnn-1.0.2/PKG-INFO` & `kwnn-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.3
+Metadata-Version: 2.1
 Name: kwnn
-Version: 1.0.2
+Version: 1.0.3
 Summary: kwniu.com ai sdk
 Project-URL: Homepage, https://github.com/
 Project-URL: Issues, https://github.com/
 Author-email: Jimmy zou <author@example.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
```

