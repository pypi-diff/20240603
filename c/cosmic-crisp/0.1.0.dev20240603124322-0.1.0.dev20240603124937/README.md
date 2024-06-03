# Comparing `tmp/cosmic_crisp-0.1.0.dev20240603124322.tar.gz` & `tmp/cosmic_crisp-0.1.0.dev20240603124937.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmic_crisp-0.1.0.dev20240603124322.tar", max compression
+gzip compressed data, was "cosmic_crisp-0.1.0.dev20240603124937.tar", max compression
```

## Comparing `cosmic_crisp-0.1.0.dev20240603124322.tar` & `cosmic_crisp-0.1.0.dev20240603124937.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0    11356 2024-06-03 12:43:01.638692 cosmic_crisp-0.1.0.dev20240603124322/LICENSE.txt
--rw-r--r--   0        0        0       21 2024-06-03 12:43:23.302859 cosmic_crisp-0.1.0.dev20240603124322/README.md
--rw-r--r--   0        0        0      241 2024-06-03 12:43:01.638692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/__init__.py
--rw-r--r--   0        0        0     1197 2024-06-03 12:43:01.638692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/__init__.py
--rw-r--r--   0        0        0      264 2024-06-03 12:43:01.638692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/api/__init__.py
--rw-r--r--   0        0        0    18997 2024-06-03 12:43:01.638692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/api/manage_knowledge_models_api.py
--rw-r--r--   0        0        0    37252 2024-06-03 12:43:01.638692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/api_client.py
--rw-r--r--   0        0        0      559 2024-06-03 12:43:01.638692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/apis/__init__.py
--rw-r--r--   0        0        0    17297 2024-06-03 12:43:01.638692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/configuration.py
--rw-r--r--   0        0        0     5352 2024-06-03 12:43:01.638692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/exceptions.py
--rw-r--r--   0        0        0      348 2024-06-03 12:43:01.638692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/model/__init__.py
--rw-r--r--   0        0        0    12196 2024-06-03 12:43:01.638692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/model/inline_object.py
--rw-r--r--   0        0        0    11620 2024-06-03 12:43:01.638692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/model/inline_response200.py
--rw-r--r--   0        0        0    11946 2024-06-03 12:43:01.638692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/model/inline_response401.py
--rw-r--r--   0        0        0    12975 2024-06-03 12:43:01.638692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/model/inline_response401_error.py
--rw-r--r--   0        0        0    13045 2024-06-03 12:43:01.638692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/model/knowledge_model.py
--rw-r--r--   0        0        0    80645 2024-06-03 12:43:01.638692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/model_utils.py
--rw-r--r--   0        0        0      913 2024-06-03 12:43:01.638692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/models/__init__.py
--rw-r--r--   0        0        0    14312 2024-06-03 12:43:01.638692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/rest.py
--rw-r--r--   0        0        0     1169 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/__init__.py
--rw-r--r--   0        0        0      261 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/api/__init__.py
--rw-r--r--   0        0        0    25616 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/api/manage_knowledge_models_api.py
--rw-r--r--   0        0        0    37272 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/api_client.py
--rw-r--r--   0        0        0      556 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/apis/__init__.py
--rw-r--r--   0        0        0    17292 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/configuration.py
--rw-r--r--   0        0        0     5348 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/exceptions.py
--rw-r--r--   0        0        0      348 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model/__init__.py
--rw-r--r--   0        0        0    11898 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model/chat_completion_model.py
--rw-r--r--   0        0        0    12168 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model/choice_model.py
--rw-r--r--   0        0        0    11494 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model/choice_model_message.py
--rw-r--r--   0        0        0    11907 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model/inline_object1.py
--rw-r--r--   0        0        0    11532 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model/inline_response200.py
--rw-r--r--   0        0        0    11933 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model/inline_response401.py
--rw-r--r--   0        0        0    12965 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model/inline_response401_error.py
--rw-r--r--   0        0        0    12874 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model/kb_file_model.py
--rw-r--r--   0        0        0    11602 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model/knowledge_chat_knowledge_model_name_chat_completions_messages.py
--rw-r--r--   0        0        0    80638 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model_utils.py
--rw-r--r--   0        0        0     1364 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/models/__init__.py
--rw-r--r--   0        0        0    14305 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/rest.py
--rw-r--r--   0        0        0       32 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/knowledge/__init__.py
--rw-r--r--   0        0        0    11249 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/knowledge/knowledge.py
--rw-r--r--   0        0        0      230 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/models/__init__.py
--rw-r--r--   0        0        0      467 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/models/chat.py
--rw-r--r--   0        0        0     1519 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/models/file_model.py
--rw-r--r--   0        0        0    12298 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/models/knowledge_model.py
--rw-r--r--   0        0        0      953 2024-06-03 12:43:23.322859 cosmic_crisp-0.1.0.dev20240603124322/pyproject.toml
--rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 cosmic_crisp-0.1.0.dev20240603124322/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-06-03 12:49:18.082223 cosmic_crisp-0.1.0.dev20240603124937/LICENSE.txt
+-rw-r--r--   0        0        0       21 2024-06-03 12:49:38.514130 cosmic_crisp-0.1.0.dev20240603124937/README.md
+-rw-r--r--   0        0        0      241 2024-06-03 12:49:18.082223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/__init__.py
+-rw-r--r--   0        0        0     1197 2024-06-03 12:49:18.082223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/__init__.py
+-rw-r--r--   0        0        0      264 2024-06-03 12:49:18.082223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/api/__init__.py
+-rw-r--r--   0        0        0    18997 2024-06-03 12:49:18.082223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/api/manage_knowledge_models_api.py
+-rw-r--r--   0        0        0    37252 2024-06-03 12:49:18.082223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/api_client.py
+-rw-r--r--   0        0        0      559 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/apis/__init__.py
+-rw-r--r--   0        0        0    17297 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/configuration.py
+-rw-r--r--   0        0        0     5352 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/exceptions.py
+-rw-r--r--   0        0        0      348 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/model/__init__.py
+-rw-r--r--   0        0        0    12196 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/model/inline_object.py
+-rw-r--r--   0        0        0    11620 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/model/inline_response200.py
+-rw-r--r--   0        0        0    11946 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/model/inline_response401.py
+-rw-r--r--   0        0        0    12975 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/model/inline_response401_error.py
+-rw-r--r--   0        0        0    13045 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/model/knowledge_model.py
+-rw-r--r--   0        0        0    80645 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/model_utils.py
+-rw-r--r--   0        0        0      913 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/models/__init__.py
+-rw-r--r--   0        0        0    14312 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/rest.py
+-rw-r--r--   0        0        0     1169 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/__init__.py
+-rw-r--r--   0        0        0      261 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/api/__init__.py
+-rw-r--r--   0        0        0    25616 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/api/manage_knowledge_models_api.py
+-rw-r--r--   0        0        0    37272 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/api_client.py
+-rw-r--r--   0        0        0      556 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/apis/__init__.py
+-rw-r--r--   0        0        0    17292 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/configuration.py
+-rw-r--r--   0        0        0     5348 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/exceptions.py
+-rw-r--r--   0        0        0      348 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model/__init__.py
+-rw-r--r--   0        0        0    11898 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model/chat_completion_model.py
+-rw-r--r--   0        0        0    12168 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model/choice_model.py
+-rw-r--r--   0        0        0    11494 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model/choice_model_message.py
+-rw-r--r--   0        0        0    11907 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model/inline_object1.py
+-rw-r--r--   0        0        0    11532 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model/inline_response200.py
+-rw-r--r--   0        0        0    11933 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model/inline_response401.py
+-rw-r--r--   0        0        0    12965 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model/inline_response401_error.py
+-rw-r--r--   0        0        0    12874 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model/kb_file_model.py
+-rw-r--r--   0        0        0    11602 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model/knowledge_chat_knowledge_model_name_chat_completions_messages.py
+-rw-r--r--   0        0        0    80638 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model_utils.py
+-rw-r--r--   0        0        0     1364 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/models/__init__.py
+-rw-r--r--   0        0        0    14305 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/rest.py
+-rw-r--r--   0        0        0       32 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/knowledge/__init__.py
+-rw-r--r--   0        0        0    11333 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/knowledge/knowledge.py
+-rw-r--r--   0        0        0      230 2024-06-03 12:49:18.090223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/models/__init__.py
+-rw-r--r--   0        0        0      467 2024-06-03 12:49:18.090223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/models/chat.py
+-rw-r--r--   0        0        0     1519 2024-06-03 12:49:18.090223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/models/file_model.py
+-rw-r--r--   0        0        0    12375 2024-06-03 12:49:18.090223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/models/knowledge_model.py
+-rw-r--r--   0        0        0      953 2024-06-03 12:49:38.538130 cosmic_crisp-0.1.0.dev20240603124937/pyproject.toml
+-rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 cosmic_crisp-0.1.0.dev20240603124937/PKG-INFO
```

### Comparing `cosmic_crisp-0.1.0.dev20240603124322/LICENSE.txt` & `cosmic_crisp-0.1.0.dev20240603124937/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/__init__.py` & `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/api/manage_knowledge_models_api.py` & `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/api/manage_knowledge_models_api.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/api_client.py` & `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/api_client.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/apis/__init__.py` & `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/configuration.py` & `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/configuration.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/exceptions.py` & `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/model/inline_object.py` & `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/model/inline_object.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/model/inline_response200.py` & `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/model/inline_response200.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/model/inline_response401.py` & `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/model/inline_response401.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/model/inline_response401_error.py` & `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/model/inline_response401_error.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/model/knowledge_model.py` & `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/model/knowledge_model.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/model_utils.py` & `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/model_utils.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/models/__init__.py` & `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/rest.py` & `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/rest.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/__init__.py` & `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/api/manage_knowledge_models_api.py` & `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/api/manage_knowledge_models_api.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/api_client.py` & `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/api_client.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/apis/__init__.py` & `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/configuration.py` & `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/configuration.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/exceptions.py` & `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model/chat_completion_model.py` & `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model/chat_completion_model.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model/choice_model.py` & `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model/choice_model.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model/choice_model_message.py` & `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model/choice_model_message.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model/inline_object1.py` & `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model/inline_object1.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model/inline_response200.py` & `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model/inline_response200.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model/inline_response401.py` & `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model/inline_response401.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model/inline_response401_error.py` & `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model/inline_response401_error.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model/kb_file_model.py` & `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model/kb_file_model.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model/knowledge_chat_knowledge_model_name_chat_completions_messages.py` & `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model/knowledge_chat_knowledge_model_name_chat_completions_messages.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model_utils.py` & `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model_utils.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/models/__init__.py` & `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/rest.py` & `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/rest.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/knowledge/knowledge.py` & `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/knowledge/knowledge.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import time
+import os 
 from typing import Optional, Dict, List
 
 from pinecone_plugin_interface import PineconePlugin
 
 from pinecone_plugins.knowledge.control.core.client.api.manage_knowledge_models_api import ManageKnowledgeModelsApi as ControlApiClient 
 from pinecone_plugins.knowledge.control.core.client.model.inline_object import InlineObject as CreateModelRequest
 from pinecone_plugins.knowledge.control.core.client import ApiClient
@@ -20,15 +21,16 @@
 
     :param client_builder: A `pinecone.utils` closure of setup_openapi_client, configured and built in the Pinecone class.
     :type client_builder: `(type(OpenApiClient), type(ClientApiClass), str, **kwargs)->ClientApiClass`, required
     """
     def __init__(self, config, client_builder):
         self.config = config
 
-        self.knowledge_control_api = client_builder(ApiClient, ControlApiClient, 'unstable', host="https://api-staging.pinecone.io")
+        host = os.getenv("PINECONE_PLUGIN_KNOWLEDGE_CONTROL_HOST", "https://api-staging.pinecone.io")
+        self.knowledge_control_api = client_builder(ApiClient, ControlApiClient, 'unstable', host=host)
         self.client_builder = client_builder
 
     def create_model(
         self, 
         knowledge_model_name: str, 
         metadata: dict[str, any] = {}, 
         timeout: Optional[int] = None,
```

### Comparing `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/models/file_model.py` & `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/models/file_model.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/models/knowledge_model.py` & `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/models/knowledge_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 from pinecone_plugins.knowledge.models.file_model import FileModel
 
 from .chat import ChatResultModel, ChatContextModel
 
 class KnowledgeModel:
     def __init__(self, knowledge_model: OpenAIKnowledgeModel, client_builder):
         self.knowledge_model = knowledge_model
-        self.knowledge_data_api = client_builder(ApiClient, DataApiClient, 'unstable', host="staging-data.ke.pinecone.io")
-
+        host = os.getenv("PINECONE_PLUGIN_KNOWLEDGE_DATA_HOST", "https://staging-data.ke.pinecone.io")
+        self.knowledge_data_api = client_builder(ApiClient, DataApiClient, 'unstable', host=host)
         # initialize types so they can be accessed
         self.name = self.knowledge_model.name
         self.created_at = self.knowledge_model.created_at
         self.updated_at = self.knowledge_model.updated_at
         self.metadata = self.knowledge_model.metadata
         self.status = self.knowledge_model.status
```

### Comparing `cosmic_crisp-0.1.0.dev20240603124322/pyproject.toml` & `cosmic_crisp-0.1.0.dev20240603124937/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cosmic-crisp"
-version = "0.1.0.dev20240603124322"
+version = "0.1.0.dev20240603124937"
 packages = [
     { include = "pinecone_plugins", from = "." },
     # { include = "pinecone.plugins", from = "./pinecone" },
     # { include = "pinecone.plugins.knowledge", from = "./pinecone/plugins" }
 ]
 
 description = "Knowledge plugin for Cosmic Crisp SDK"
```

### Comparing `cosmic_crisp-0.1.0.dev20240603124322/PKG-INFO` & `cosmic_crisp-0.1.0.dev20240603124937/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cosmic-crisp
-Version: 0.1.0.dev20240603124322
+Version: 0.1.0.dev20240603124937
 Summary: Knowledge plugin for Cosmic Crisp SDK
 Home-page: https://www.cosmic-crisp.com
 License: Apache-2.0
 Author: Cosmic Crisp Systems, Inc.
 Author-email: support@cosmic-crisp.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```
