# Comparing `tmp/copilothistoryexporter-1.1.2.tar.gz` & `tmp/copilothistoryexporter-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copilothistoryexporter-1.1.2.tar", last modified: Mon Jun  3 07:47:54 2024, max compression
+gzip compressed data, was "copilothistoryexporter-1.2.1.tar", last modified: Mon Jun  3 10:55:00 2024, max compression
```

## Comparing `copilothistoryexporter-1.1.2.tar` & `copilothistoryexporter-1.2.1.tar`

### file list

```diff
@@ -1,33 +1,27 @@
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 07:47:54.516232 copilothistoryexporter-1.1.2/
--rw-r--r--   0 mustafakilic   (501) staff       (20)     1073 2024-06-01 16:20:49.000000 copilothistoryexporter-1.1.2/LICENCE
--rw-r--r--   0 mustafakilic   (501) staff       (20)     2752 2024-06-03 07:47:54.516029 copilothistoryexporter-1.1.2/PKG-INFO
--rw-r--r--   0 mustafakilic   (501) staff       (20)     2232 2024-06-02 16:13:30.000000 copilothistoryexporter-1.1.2/README.md
--rw-r--r--   0 mustafakilic   (501) staff       (20)      656 2024-06-03 07:47:21.000000 copilothistoryexporter-1.1.2/pyproject.toml
--rw-r--r--   0 mustafakilic   (501) staff       (20)       38 2024-06-03 07:47:54.516276 copilothistoryexporter-1.1.2/setup.cfg
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 07:47:54.513205 copilothistoryexporter-1.1.2/src/
--rw-r--r--   0 mustafakilic   (501) staff       (20)        0 2024-06-03 06:01:46.000000 copilothistoryexporter-1.1.2/src/__init__.py
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 07:47:54.513622 copilothistoryexporter-1.1.2/src/copilothistoryexporter/
--rw-r--r--   0 mustafakilic   (501) staff       (20)        0 2024-06-03 06:01:46.000000 copilothistoryexporter-1.1.2/src/copilothistoryexporter/__init__.py
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 07:47:54.514576 copilothistoryexporter-1.1.2/src/copilothistoryexporter/addons/
--rw-r--r--   0 mustafakilic   (501) staff       (20)        0 2024-06-03 05:45:17.000000 copilothistoryexporter-1.1.2/src/copilothistoryexporter/addons/__init__.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)     1516 2024-06-03 07:04:53.000000 copilothistoryexporter-1.1.2/src/copilothistoryexporter/addons/binding.py
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 07:47:54.515380 copilothistoryexporter-1.1.2/src/copilothistoryexporter/intercp/
--rw-r--r--   0 mustafakilic   (501) staff       (20)        0 2024-06-03 06:01:46.000000 copilothistoryexporter-1.1.2/src/copilothistoryexporter/intercp/__init__.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      517 2024-06-03 07:05:36.000000 copilothistoryexporter-1.1.2/src/copilothistoryexporter/intercp/cache.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      652 2024-06-03 07:05:46.000000 copilothistoryexporter-1.1.2/src/copilothistoryexporter/intercp/chain.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      205 2024-06-03 07:05:50.000000 copilothistoryexporter-1.1.2/src/copilothistoryexporter/intercp/interceptor.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      362 2024-06-03 07:05:56.000000 copilothistoryexporter-1.1.2/src/copilothistoryexporter/intercp/markdown.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      606 2024-06-03 07:06:02.000000 copilothistoryexporter-1.1.2/src/copilothistoryexporter/intercp/vote.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)     1158 2024-06-03 07:06:39.000000 copilothistoryexporter-1.1.2/src/copilothistoryexporter/main.py
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 07:47:54.515643 copilothistoryexporter-1.1.2/src/copilothistoryexporter/model/
--rw-r--r--   0 mustafakilic   (501) staff       (20)      395 2024-06-02 16:13:00.000000 copilothistoryexporter-1.1.2/src/copilothistoryexporter/model/conversation.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      251 2024-06-03 07:06:09.000000 copilothistoryexporter-1.1.2/src/copilothistoryexporter/model/request.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)       92 2024-06-02 16:13:00.000000 copilothistoryexporter-1.1.2/src/copilothistoryexporter/sample.md
--rw-r--r--   0 mustafakilic   (501) staff       (20)     2383 2024-06-03 07:06:54.000000 copilothistoryexporter-1.1.2/src/copilothistoryexporter/utils.py
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 07:47:54.515808 copilothistoryexporter-1.1.2/src/copilothistoryexporter.egg-info/
--rw-r--r--   0 mustafakilic   (501) staff       (20)     2752 2024-06-03 07:47:54.000000 copilothistoryexporter-1.1.2/src/copilothistoryexporter.egg-info/PKG-INFO
--rw-r--r--   0 mustafakilic   (501) staff       (20)      956 2024-06-03 07:47:54.000000 copilothistoryexporter-1.1.2/src/copilothistoryexporter.egg-info/SOURCES.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)        1 2024-06-03 07:47:54.000000 copilothistoryexporter-1.1.2/src/copilothistoryexporter.egg-info/dependency_links.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)       80 2024-06-03 07:47:54.000000 copilothistoryexporter-1.1.2/src/copilothistoryexporter.egg-info/entry_points.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)       31 2024-06-03 07:47:54.000000 copilothistoryexporter-1.1.2/src/copilothistoryexporter.egg-info/requires.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)       32 2024-06-03 07:47:54.000000 copilothistoryexporter-1.1.2/src/copilothistoryexporter.egg-info/top_level.txt
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 10:55:00.314552 copilothistoryexporter-1.2.1/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     1073 2024-06-01 16:20:49.000000 copilothistoryexporter-1.2.1/LICENCE
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     2752 2024-06-03 10:55:00.314335 copilothistoryexporter-1.2.1/PKG-INFO
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     2232 2024-06-02 16:13:30.000000 copilothistoryexporter-1.2.1/README.md
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 10:55:00.312193 copilothistoryexporter-1.2.1/che/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       65 2024-06-03 09:58:49.000000 copilothistoryexporter-1.2.1/che/__init__.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     1387 2024-06-03 10:05:51.000000 copilothistoryexporter-1.2.1/che/binding.py
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 10:55:00.313199 copilothistoryexporter-1.2.1/che/intercept/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)        1 2024-06-03 10:12:16.000000 copilothistoryexporter-1.2.1/che/intercept/__init__.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      489 2024-06-03 10:11:44.000000 copilothistoryexporter-1.2.1/che/intercept/cache.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      585 2024-06-03 10:13:30.000000 copilothistoryexporter-1.2.1/che/intercept/chain.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      395 2024-06-02 16:13:00.000000 copilothistoryexporter-1.2.1/che/intercept/conversation.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      190 2024-06-03 10:12:37.000000 copilothistoryexporter-1.2.1/che/intercept/interceptor.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      330 2024-06-03 10:14:18.000000 copilothistoryexporter-1.2.1/che/intercept/markdown.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      236 2024-06-03 10:12:47.000000 copilothistoryexporter-1.2.1/che/intercept/request.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      578 2024-06-03 10:14:50.000000 copilothistoryexporter-1.2.1/che/intercept/vote.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      703 2024-06-03 10:53:57.000000 copilothistoryexporter-1.2.1/che/main.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     2367 2024-06-03 10:13:00.000000 copilothistoryexporter-1.2.1/che/utils.py
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 10:55:00.314133 copilothistoryexporter-1.2.1/copilothistoryexporter.egg-info/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     2752 2024-06-03 10:55:00.000000 copilothistoryexporter-1.2.1/copilothistoryexporter.egg-info/PKG-INFO
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      570 2024-06-03 10:55:00.000000 copilothistoryexporter-1.2.1/copilothistoryexporter.egg-info/SOURCES.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)        1 2024-06-03 10:55:00.000000 copilothistoryexporter-1.2.1/copilothistoryexporter.egg-info/dependency_links.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       80 2024-06-03 10:55:00.000000 copilothistoryexporter-1.2.1/copilothistoryexporter.egg-info/entry_points.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       31 2024-06-03 10:55:00.000000 copilothistoryexporter-1.2.1/copilothistoryexporter.egg-info/requires.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)        4 2024-06-03 10:55:00.000000 copilothistoryexporter-1.2.1/copilothistoryexporter.egg-info/top_level.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      656 2024-06-03 10:54:42.000000 copilothistoryexporter-1.2.1/pyproject.toml
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       38 2024-06-03 10:55:00.314598 copilothistoryexporter-1.2.1/setup.cfg
```

### Comparing `copilothistoryexporter-1.1.2/LICENCE` & `copilothistoryexporter-1.2.1/LICENCE`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.1.2/PKG-INFO` & `copilothistoryexporter-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copilothistoryexporter
-Version: 1.1.2
+Version: 1.2.1
 Summary: Copilot History Exporter
 Author-email: enciyo <enciyomk61@gmail.com>
 Project-URL: Homepage, https://github.com/enciyo/gh-copilot-history-export
 Project-URL: Source, https://github.com/enciyo/gh-copilot-history-export
 Project-URL: Documentation, https://github.com/enciyo/gh-copilot-history-export
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `copilothistoryexporter-1.1.2/README.md` & `copilothistoryexporter-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.1.2/pyproject.toml` & `copilothistoryexporter-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "copilothistoryexporter"
 description = "Copilot History Exporter"
-version = "1.1.2"
+version = "1.2.1"
 requires-python = ">=3.11"
 readme = "README.md"
 authors = [{ name = "enciyo", email = "enciyomk61@gmail.com" }]
 
 dependencies = [
     "click~=8.1.7",
     "mitmproxy~=10.3.0"
```

### Comparing `copilothistoryexporter-1.1.2/src/copilothistoryexporter/addons/binding.py` & `copilothistoryexporter-1.2.1/che/binding.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 import re
 
 from mitmproxy import http
 
-
-from copilothistoryexporter.intercp.chain import InterceptorChain
-from copilothistoryexporter.model.conversation import Conversation
-from copilothistoryexporter.model.request import Request
-
+from che.intercept.conversation import Conversation
+from che.intercept.request import Request
+from che.intercept.chain import InterceptorChain
 
 LISTEN_URL = "https://api.githubcopilot.com/chat/completions"
-LISTEN_URL_RATING = "https://copilot-telemetry.githubusercontent.com/telemetry"
 
 chain = InterceptorChain()
 
 
 def get_message_from_response(data) -> list[Conversation]:
     user_contents = [message['content'] for message in data['messages'] if message['role'] == 'user']
     if user_contents.__len__() == 1 and data.get("intent_content", None) is None:
```

### Comparing `copilothistoryexporter-1.1.2/src/copilothistoryexporter/intercp/cache.py` & `copilothistoryexporter-1.2.1/che/intercept/vote.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from copilothistoryexporter import utils
-from copilothistoryexporter.intercp.interceptor import Interceptor
-from copilothistoryexporter.model.request import Request
+from che.intercept.interceptor import Interceptor
+from che.intercept.request import Request
+from che.utils import get_json_files, write_to_json_file
 
 
-class CacheInterceptor(Interceptor):
+class VoteInterceptor(Interceptor):
     def process(self, request: Request):
-        conversations = utils.get_json_files()
-        if request.conversation.prompt != "ignore":
-            conversations.append(request.conversation.to_dict())
-            print("Cache updated")
-
-        utils.write_to_json_file(conversations)
-
+        prompt = request.conversation.prompt
+        if prompt == "vote:good" or prompt == "vote:bad":
+            conversations = get_json_files()
+            conversations[-1]["rating"] = "***" if prompt == "vote:good" else "*"
+            write_to_json_file(conversations)
+            request.conversation.prompt = "ignore"
         return request
```

### Comparing `copilothistoryexporter-1.1.2/src/copilothistoryexporter/intercp/chain.py` & `copilothistoryexporter-1.2.1/che/intercept/chain.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from copilothistoryexporter.intercp.cache import CacheInterceptor
-from copilothistoryexporter.intercp.markdown import MarkdownInterceptor
-from copilothistoryexporter.intercp.vote import VoteInterceptor
-from copilothistoryexporter.model.request import Request
-
+from che.intercept.cache import CacheInterceptor
+from che.intercept.markdown import MarkdownInterceptor
+from che.intercept.vote import VoteInterceptor
+from che.intercept.request import Request
 
 class InterceptorChain:
     def __init__(self):
         self.interceptors = [
             VoteInterceptor(),
             CacheInterceptor(),
             MarkdownInterceptor()
```

### Comparing `copilothistoryexporter-1.1.2/src/copilothistoryexporter/utils.py` & `copilothistoryexporter-1.2.1/che/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import json
 import os
-
 import subprocess
 
-from copilothistoryexporter.model.conversation import Conversation
+from che.intercept.conversation import Conversation
 
 
 class SharedValues:
     WORKSPACE = ""
 
     @staticmethod
     def change_workspace(src: str):
```

### Comparing `copilothistoryexporter-1.1.2/src/copilothistoryexporter.egg-info/PKG-INFO` & `copilothistoryexporter-1.2.1/copilothistoryexporter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copilothistoryexporter
-Version: 1.1.2
+Version: 1.2.1
 Summary: Copilot History Exporter
 Author-email: enciyo <enciyomk61@gmail.com>
 Project-URL: Homepage, https://github.com/enciyo/gh-copilot-history-export
 Project-URL: Source, https://github.com/enciyo/gh-copilot-history-export
 Project-URL: Documentation, https://github.com/enciyo/gh-copilot-history-export
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

