# Comparing `tmp/cosmic_crisp-0.1.0.dev20240603124937.tar.gz` & `tmp/cosmic_crisp-0.1.0.dev20240603133038.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmic_crisp-0.1.0.dev20240603124937.tar", max compression
+gzip compressed data, was "cosmic_crisp-0.1.0.dev20240603133038.tar", max compression
```

## Comparing `cosmic_crisp-0.1.0.dev20240603124937.tar` & `cosmic_crisp-0.1.0.dev20240603133038.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0    11356 2024-06-03 12:49:18.082223 cosmic_crisp-0.1.0.dev20240603124937/LICENSE.txt
--rw-r--r--   0        0        0       21 2024-06-03 12:49:38.514130 cosmic_crisp-0.1.0.dev20240603124937/README.md
--rw-r--r--   0        0        0      241 2024-06-03 12:49:18.082223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/__init__.py
--rw-r--r--   0        0        0     1197 2024-06-03 12:49:18.082223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/__init__.py
--rw-r--r--   0        0        0      264 2024-06-03 12:49:18.082223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/api/__init__.py
--rw-r--r--   0        0        0    18997 2024-06-03 12:49:18.082223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/api/manage_knowledge_models_api.py
--rw-r--r--   0        0        0    37252 2024-06-03 12:49:18.082223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/api_client.py
--rw-r--r--   0        0        0      559 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/apis/__init__.py
--rw-r--r--   0        0        0    17297 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/configuration.py
--rw-r--r--   0        0        0     5352 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/exceptions.py
--rw-r--r--   0        0        0      348 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/model/__init__.py
--rw-r--r--   0        0        0    12196 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/model/inline_object.py
--rw-r--r--   0        0        0    11620 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/model/inline_response200.py
--rw-r--r--   0        0        0    11946 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/model/inline_response401.py
--rw-r--r--   0        0        0    12975 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/model/inline_response401_error.py
--rw-r--r--   0        0        0    13045 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/model/knowledge_model.py
--rw-r--r--   0        0        0    80645 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/model_utils.py
--rw-r--r--   0        0        0      913 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/models/__init__.py
--rw-r--r--   0        0        0    14312 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/rest.py
--rw-r--r--   0        0        0     1169 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/__init__.py
--rw-r--r--   0        0        0      261 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/api/__init__.py
--rw-r--r--   0        0        0    25616 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/api/manage_knowledge_models_api.py
--rw-r--r--   0        0        0    37272 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/api_client.py
--rw-r--r--   0        0        0      556 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/apis/__init__.py
--rw-r--r--   0        0        0    17292 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/configuration.py
--rw-r--r--   0        0        0     5348 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/exceptions.py
--rw-r--r--   0        0        0      348 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model/__init__.py
--rw-r--r--   0        0        0    11898 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model/chat_completion_model.py
--rw-r--r--   0        0        0    12168 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model/choice_model.py
--rw-r--r--   0        0        0    11494 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model/choice_model_message.py
--rw-r--r--   0        0        0    11907 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model/inline_object1.py
--rw-r--r--   0        0        0    11532 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model/inline_response200.py
--rw-r--r--   0        0        0    11933 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model/inline_response401.py
--rw-r--r--   0        0        0    12965 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model/inline_response401_error.py
--rw-r--r--   0        0        0    12874 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model/kb_file_model.py
--rw-r--r--   0        0        0    11602 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model/knowledge_chat_knowledge_model_name_chat_completions_messages.py
--rw-r--r--   0        0        0    80638 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model_utils.py
--rw-r--r--   0        0        0     1364 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/models/__init__.py
--rw-r--r--   0        0        0    14305 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/rest.py
--rw-r--r--   0        0        0       32 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/knowledge/__init__.py
--rw-r--r--   0        0        0    11333 2024-06-03 12:49:18.086223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/knowledge/knowledge.py
--rw-r--r--   0        0        0      230 2024-06-03 12:49:18.090223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/models/__init__.py
--rw-r--r--   0        0        0      467 2024-06-03 12:49:18.090223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/models/chat.py
--rw-r--r--   0        0        0     1519 2024-06-03 12:49:18.090223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/models/file_model.py
--rw-r--r--   0        0        0    12375 2024-06-03 12:49:18.090223 cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/models/knowledge_model.py
--rw-r--r--   0        0        0      953 2024-06-03 12:49:38.538130 cosmic_crisp-0.1.0.dev20240603124937/pyproject.toml
--rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 cosmic_crisp-0.1.0.dev20240603124937/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-06-03 13:30:17.331732 cosmic_crisp-0.1.0.dev20240603133038/LICENSE.txt
+-rw-r--r--   0        0        0       21 2024-06-03 13:30:39.543948 cosmic_crisp-0.1.0.dev20240603133038/README.md
+-rw-r--r--   0        0        0      241 2024-06-03 13:30:17.331732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/__init__.py
+-rw-r--r--   0        0        0     1197 2024-06-03 13:30:17.331732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/control/core/client/__init__.py
+-rw-r--r--   0        0        0      264 2024-06-03 13:30:17.331732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/control/core/client/api/__init__.py
+-rw-r--r--   0        0        0    18997 2024-06-03 13:30:17.331732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/control/core/client/api/manage_knowledge_models_api.py
+-rw-r--r--   0        0        0    37252 2024-06-03 13:30:17.331732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/control/core/client/api_client.py
+-rw-r--r--   0        0        0      559 2024-06-03 13:30:17.331732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/control/core/client/apis/__init__.py
+-rw-r--r--   0        0        0    17297 2024-06-03 13:30:17.331732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/control/core/client/configuration.py
+-rw-r--r--   0        0        0     5352 2024-06-03 13:30:17.331732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/control/core/client/exceptions.py
+-rw-r--r--   0        0        0      348 2024-06-03 13:30:17.331732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/control/core/client/model/__init__.py
+-rw-r--r--   0        0        0    12196 2024-06-03 13:30:17.331732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/control/core/client/model/inline_object.py
+-rw-r--r--   0        0        0    11620 2024-06-03 13:30:17.331732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/control/core/client/model/inline_response200.py
+-rw-r--r--   0        0        0    11946 2024-06-03 13:30:17.331732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/control/core/client/model/inline_response401.py
+-rw-r--r--   0        0        0    12975 2024-06-03 13:30:17.331732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/control/core/client/model/inline_response401_error.py
+-rw-r--r--   0        0        0    13045 2024-06-03 13:30:17.331732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/control/core/client/model/knowledge_model.py
+-rw-r--r--   0        0        0    80645 2024-06-03 13:30:17.331732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/control/core/client/model_utils.py
+-rw-r--r--   0        0        0      913 2024-06-03 13:30:17.331732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/control/core/client/models/__init__.py
+-rw-r--r--   0        0        0    14312 2024-06-03 13:30:17.331732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/control/core/client/rest.py
+-rw-r--r--   0        0        0     1169 2024-06-03 13:30:17.331732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/data/core/client/__init__.py
+-rw-r--r--   0        0        0      261 2024-06-03 13:30:17.331732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/data/core/client/api/__init__.py
+-rw-r--r--   0        0        0    25616 2024-06-03 13:30:17.331732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/data/core/client/api/manage_knowledge_models_api.py
+-rw-r--r--   0        0        0    37272 2024-06-03 13:30:17.331732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/data/core/client/api_client.py
+-rw-r--r--   0        0        0      556 2024-06-03 13:30:17.331732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/data/core/client/apis/__init__.py
+-rw-r--r--   0        0        0    17292 2024-06-03 13:30:17.331732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/data/core/client/configuration.py
+-rw-r--r--   0        0        0     5348 2024-06-03 13:30:17.331732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/data/core/client/exceptions.py
+-rw-r--r--   0        0        0      348 2024-06-03 13:30:17.331732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/data/core/client/model/__init__.py
+-rw-r--r--   0        0        0    11898 2024-06-03 13:30:17.331732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/data/core/client/model/chat_completion_model.py
+-rw-r--r--   0        0        0    12168 2024-06-03 13:30:17.335732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/data/core/client/model/choice_model.py
+-rw-r--r--   0        0        0    11494 2024-06-03 13:30:17.335732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/data/core/client/model/choice_model_message.py
+-rw-r--r--   0        0        0    11907 2024-06-03 13:30:17.335732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/data/core/client/model/inline_object1.py
+-rw-r--r--   0        0        0    11532 2024-06-03 13:30:17.335732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/data/core/client/model/inline_response200.py
+-rw-r--r--   0        0        0    11933 2024-06-03 13:30:17.335732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/data/core/client/model/inline_response401.py
+-rw-r--r--   0        0        0    12965 2024-06-03 13:30:17.335732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/data/core/client/model/inline_response401_error.py
+-rw-r--r--   0        0        0    12874 2024-06-03 13:30:17.335732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/data/core/client/model/kb_file_model.py
+-rw-r--r--   0        0        0    11602 2024-06-03 13:30:17.335732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/data/core/client/model/knowledge_chat_knowledge_model_name_chat_completions_messages.py
+-rw-r--r--   0        0        0    80638 2024-06-03 13:30:17.335732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/data/core/client/model_utils.py
+-rw-r--r--   0        0        0     1364 2024-06-03 13:30:17.335732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/data/core/client/models/__init__.py
+-rw-r--r--   0        0        0    14305 2024-06-03 13:30:17.335732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/data/core/client/rest.py
+-rw-r--r--   0        0        0       32 2024-06-03 13:30:17.335732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/knowledge/__init__.py
+-rw-r--r--   0        0        0    11333 2024-06-03 13:30:17.335732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/knowledge/knowledge.py
+-rw-r--r--   0        0        0      230 2024-06-03 13:30:17.335732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/models/__init__.py
+-rw-r--r--   0        0        0      467 2024-06-03 13:30:17.335732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/models/chat.py
+-rw-r--r--   0        0        0     1519 2024-06-03 13:30:17.335732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/models/file_model.py
+-rw-r--r--   0        0        0    14909 2024-06-03 13:30:17.335732 cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/models/knowledge_model.py
+-rw-r--r--   0        0        0      953 2024-06-03 13:30:39.567948 cosmic_crisp-0.1.0.dev20240603133038/pyproject.toml
+-rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 cosmic_crisp-0.1.0.dev20240603133038/PKG-INFO
```

### Comparing `cosmic_crisp-0.1.0.dev20240603124937/LICENSE.txt` & `cosmic_crisp-0.1.0.dev20240603133038/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/__init__.py` & `cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/control/core/client/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/api/manage_knowledge_models_api.py` & `cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/control/core/client/api/manage_knowledge_models_api.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/api_client.py` & `cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/control/core/client/api_client.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/apis/__init__.py` & `cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/control/core/client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/configuration.py` & `cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/control/core/client/configuration.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/exceptions.py` & `cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/control/core/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/model/inline_object.py` & `cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/control/core/client/model/inline_object.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/model/inline_response200.py` & `cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/control/core/client/model/inline_response200.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/model/inline_response401.py` & `cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/control/core/client/model/inline_response401.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/model/inline_response401_error.py` & `cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/control/core/client/model/inline_response401_error.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/model/knowledge_model.py` & `cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/control/core/client/model/knowledge_model.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/model_utils.py` & `cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/control/core/client/model_utils.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/models/__init__.py` & `cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/control/core/client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/control/core/client/rest.py` & `cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/control/core/client/rest.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/__init__.py` & `cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/data/core/client/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/api/manage_knowledge_models_api.py` & `cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/data/core/client/api/manage_knowledge_models_api.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/api_client.py` & `cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/data/core/client/api_client.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/apis/__init__.py` & `cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/data/core/client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/configuration.py` & `cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/data/core/client/configuration.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/exceptions.py` & `cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/data/core/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model/chat_completion_model.py` & `cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/data/core/client/model/chat_completion_model.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model/choice_model.py` & `cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/data/core/client/model/choice_model.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model/choice_model_message.py` & `cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/data/core/client/model/choice_model_message.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model/inline_object1.py` & `cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/data/core/client/model/inline_object1.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model/inline_response200.py` & `cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/data/core/client/model/inline_response200.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model/inline_response401.py` & `cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/data/core/client/model/inline_response401.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model/inline_response401_error.py` & `cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/data/core/client/model/inline_response401_error.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model/kb_file_model.py` & `cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/data/core/client/model/kb_file_model.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model/knowledge_chat_knowledge_model_name_chat_completions_messages.py` & `cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/data/core/client/model/knowledge_chat_knowledge_model_name_chat_completions_messages.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/model_utils.py` & `cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/data/core/client/model_utils.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/models/__init__.py` & `cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/data/core/client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/data/core/client/rest.py` & `cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/data/core/client/rest.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/knowledge/knowledge.py` & `cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/knowledge/knowledge.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/models/file_model.py` & `cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/models/file_model.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240603124937/pinecone_plugins/knowledge/models/knowledge_model.py` & `cosmic_crisp-0.1.0.dev20240603133038/pinecone_plugins/knowledge/models/knowledge_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         self.knowledge_data_api = client_builder(ApiClient, DataApiClient, 'unstable', host=host)
         # initialize types so they can be accessed
         self.name = self.knowledge_model.name
         self.created_at = self.knowledge_model.created_at
         self.updated_at = self.knowledge_model.updated_at
         self.metadata = self.knowledge_model.metadata
         self.status = self.knowledge_model.status
+        self.ctxs = []
 
     def __str__(self):
         return str(self.knowledge_model)
     
     def __repr__(self):
         return repr(self.knowledge_model)
 
@@ -276,8 +277,66 @@
 
         context = ChatRequest(messages=chat_context)
         search_result = self.knowledge_data_api.chat_completion_knowledge_model(
             knowledge_model_name=self.name, 
             inline_object1=context
         )
         results = ChatResultModel(chat_result=search_result)
-        return search_result 
+        return search_result 
+
+    def stateful_chat(self, content: str) -> ChatResultModel: 
+        """
+        Performs a stateful chat completion request to the following knowledge model. It will automatically add previous interactions with this method
+        to be used with this request. 
+
+        :param content: The query to be made
+        :type content: str 
+        
+        :return: ChatResultModel with the following format:
+            {
+                "choices": [
+                    {
+                    "finish_reason": "stop",
+                    "index": 0,
+                    "message": {
+                        "content": "The 2020 World Series was played in Texas at Globe Life Field in Arlington.",
+                        "role": "assistant"
+                    },
+                    "logprobs": null
+                    }
+                ],
+                "id": "chatcmpl-7QyqpwdfhqwajicIEznoc6Q47XAyW",
+                "model": "gpt-3.5-turbo-0613",
+            }
+        
+        Example:
+        >>> from pinecone_plugins.knowledge.models import ChatContextModel
+        >>> km = (...).knowledge.Model("planets-km")
+        >>> chat_context = [ChatContextModel(role='user', content='How old is the earth')]
+        >>> resp = km.stateful_chat(chat_context=chat_context)
+        >>> print(resp)
+        {'choices': [{'finish_reason': 'stop',
+              'index': 0,
+              'message': {'content': 'The age of the Earth is estimated to be '
+                                     'about 4.54 billion years, based on '
+                                     'evidence from radiometric age dating of '
+                                     'meteorite material and Earth rocks, as '
+                                     'well as lunar samples. This estimate has '
+                                     'a margin of error of about 1%.',
+                          'role': 'assistant'}}],
+        'id': 'chatcmpl-9VmkSD9s7rfP28uScLlheookaSwcB',
+        'model': 'planets-km'}
+        """
+        ctx = ChatContext(role="user", content=content)
+        self.ctxs.append(ctx)
+
+        context = ChatRequest(messages=self.ctxs)
+        chat_result = self.knowledge_data_api.chat_completion_knowledge_model(
+            knowledge_model_name=self.name,
+            inline_object1=context
+        )
+        
+
+        # append the result to ctx
+        ctx = ChatContext(role=chat_result.choices[0].message.role, content=chat_result.choices[0].message.content)
+        self.ctxs.append(ctx)
+        return chat_result
```

### Comparing `cosmic_crisp-0.1.0.dev20240603124937/pyproject.toml` & `cosmic_crisp-0.1.0.dev20240603133038/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cosmic-crisp"
-version = "0.1.0.dev20240603124937"
+version = "0.1.0.dev20240603133038"
 packages = [
     { include = "pinecone_plugins", from = "." },
     # { include = "pinecone.plugins", from = "./pinecone" },
     # { include = "pinecone.plugins.knowledge", from = "./pinecone/plugins" }
 ]
 
 description = "Knowledge plugin for Cosmic Crisp SDK"
```

### Comparing `cosmic_crisp-0.1.0.dev20240603124937/PKG-INFO` & `cosmic_crisp-0.1.0.dev20240603133038/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cosmic-crisp
-Version: 0.1.0.dev20240603124937
+Version: 0.1.0.dev20240603133038
 Summary: Knowledge plugin for Cosmic Crisp SDK
 Home-page: https://www.cosmic-crisp.com
 License: Apache-2.0
 Author: Cosmic Crisp Systems, Inc.
 Author-email: support@cosmic-crisp.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

