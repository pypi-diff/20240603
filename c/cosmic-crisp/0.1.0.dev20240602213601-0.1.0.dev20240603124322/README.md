# Comparing `tmp/cosmic_crisp-0.1.0.dev20240602213601.tar.gz` & `tmp/cosmic_crisp-0.1.0.dev20240603124322.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmic_crisp-0.1.0.dev20240602213601.tar", max compression
+gzip compressed data, was "cosmic_crisp-0.1.0.dev20240603124322.tar", max compression
```

## Comparing `cosmic_crisp-0.1.0.dev20240602213601.tar` & `cosmic_crisp-0.1.0.dev20240603124322.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0    11356 2024-06-02 21:35:44.049373 cosmic_crisp-0.1.0.dev20240602213601/LICENSE.txt
--rw-r--r--   0        0        0       21 2024-06-02 21:36:02.781369 cosmic_crisp-0.1.0.dev20240602213601/README.md
--rw-r--r--   0        0        0      241 2024-06-02 21:35:44.049373 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/__init__.py
--rw-r--r--   0        0        0     1197 2024-06-02 21:35:44.049373 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/__init__.py
--rw-r--r--   0        0        0      264 2024-06-02 21:35:44.049373 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/api/__init__.py
--rw-r--r--   0        0        0    18997 2024-06-02 21:35:44.049373 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/api/manage_knowledge_models_api.py
--rw-r--r--   0        0        0    37252 2024-06-02 21:35:44.049373 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/api_client.py
--rw-r--r--   0        0        0      559 2024-06-02 21:35:44.049373 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/apis/__init__.py
--rw-r--r--   0        0        0    17297 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/configuration.py
--rw-r--r--   0        0        0     5352 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/exceptions.py
--rw-r--r--   0        0        0      348 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/model/__init__.py
--rw-r--r--   0        0        0    12196 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/model/inline_object.py
--rw-r--r--   0        0        0    11620 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/model/inline_response200.py
--rw-r--r--   0        0        0    11946 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/model/inline_response401.py
--rw-r--r--   0        0        0    12975 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/model/inline_response401_error.py
--rw-r--r--   0        0        0    13045 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/model/knowledge_model.py
--rw-r--r--   0        0        0    80645 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/model_utils.py
--rw-r--r--   0        0        0      913 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/models/__init__.py
--rw-r--r--   0        0        0    14312 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/rest.py
--rw-r--r--   0        0        0     1169 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/__init__.py
--rw-r--r--   0        0        0      261 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/api/__init__.py
--rw-r--r--   0        0        0    25616 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/api/manage_knowledge_models_api.py
--rw-r--r--   0        0        0    37272 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/api_client.py
--rw-r--r--   0        0        0      556 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/apis/__init__.py
--rw-r--r--   0        0        0    17292 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/configuration.py
--rw-r--r--   0        0        0     5348 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/exceptions.py
--rw-r--r--   0        0        0      348 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model/__init__.py
--rw-r--r--   0        0        0    11898 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model/chat_completion_model.py
--rw-r--r--   0        0        0    12168 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model/choice_model.py
--rw-r--r--   0        0        0    11494 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model/choice_model_message.py
--rw-r--r--   0        0        0    11907 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model/inline_object1.py
--rw-r--r--   0        0        0    11532 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model/inline_response200.py
--rw-r--r--   0        0        0    11933 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model/inline_response401.py
--rw-r--r--   0        0        0    12965 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model/inline_response401_error.py
--rw-r--r--   0        0        0    12874 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model/kb_file_model.py
--rw-r--r--   0        0        0    11602 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model/knowledge_chat_knowledge_model_name_chat_completions_messages.py
--rw-r--r--   0        0        0    80638 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model_utils.py
--rw-r--r--   0        0        0     1364 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/models/__init__.py
--rw-r--r--   0        0        0    14305 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/rest.py
--rw-r--r--   0        0        0       32 2024-06-02 21:35:44.057372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/knowledge/__init__.py
--rw-r--r--   0        0        0    11249 2024-06-02 21:35:44.057372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/knowledge/knowledge.py
--rw-r--r--   0        0        0      230 2024-06-02 21:35:44.057372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/models/__init__.py
--rw-r--r--   0        0        0      467 2024-06-02 21:35:44.057372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/models/chat.py
--rw-r--r--   0        0        0     1519 2024-06-02 21:35:44.057372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/models/file_model.py
--rw-r--r--   0        0        0    12298 2024-06-02 21:35:44.057372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/models/knowledge_model.py
--rw-r--r--   0        0        0      953 2024-06-02 21:36:02.805369 cosmic_crisp-0.1.0.dev20240602213601/pyproject.toml
--rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 cosmic_crisp-0.1.0.dev20240602213601/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-06-03 12:43:01.638692 cosmic_crisp-0.1.0.dev20240603124322/LICENSE.txt
+-rw-r--r--   0        0        0       21 2024-06-03 12:43:23.302859 cosmic_crisp-0.1.0.dev20240603124322/README.md
+-rw-r--r--   0        0        0      241 2024-06-03 12:43:01.638692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/__init__.py
+-rw-r--r--   0        0        0     1197 2024-06-03 12:43:01.638692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/__init__.py
+-rw-r--r--   0        0        0      264 2024-06-03 12:43:01.638692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/api/__init__.py
+-rw-r--r--   0        0        0    18997 2024-06-03 12:43:01.638692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/api/manage_knowledge_models_api.py
+-rw-r--r--   0        0        0    37252 2024-06-03 12:43:01.638692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/api_client.py
+-rw-r--r--   0        0        0      559 2024-06-03 12:43:01.638692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/apis/__init__.py
+-rw-r--r--   0        0        0    17297 2024-06-03 12:43:01.638692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/configuration.py
+-rw-r--r--   0        0        0     5352 2024-06-03 12:43:01.638692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/exceptions.py
+-rw-r--r--   0        0        0      348 2024-06-03 12:43:01.638692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/model/__init__.py
+-rw-r--r--   0        0        0    12196 2024-06-03 12:43:01.638692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/model/inline_object.py
+-rw-r--r--   0        0        0    11620 2024-06-03 12:43:01.638692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/model/inline_response200.py
+-rw-r--r--   0        0        0    11946 2024-06-03 12:43:01.638692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/model/inline_response401.py
+-rw-r--r--   0        0        0    12975 2024-06-03 12:43:01.638692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/model/inline_response401_error.py
+-rw-r--r--   0        0        0    13045 2024-06-03 12:43:01.638692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/model/knowledge_model.py
+-rw-r--r--   0        0        0    80645 2024-06-03 12:43:01.638692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/model_utils.py
+-rw-r--r--   0        0        0      913 2024-06-03 12:43:01.638692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/models/__init__.py
+-rw-r--r--   0        0        0    14312 2024-06-03 12:43:01.638692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/rest.py
+-rw-r--r--   0        0        0     1169 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/__init__.py
+-rw-r--r--   0        0        0      261 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/api/__init__.py
+-rw-r--r--   0        0        0    25616 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/api/manage_knowledge_models_api.py
+-rw-r--r--   0        0        0    37272 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/api_client.py
+-rw-r--r--   0        0        0      556 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/apis/__init__.py
+-rw-r--r--   0        0        0    17292 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/configuration.py
+-rw-r--r--   0        0        0     5348 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/exceptions.py
+-rw-r--r--   0        0        0      348 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model/__init__.py
+-rw-r--r--   0        0        0    11898 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model/chat_completion_model.py
+-rw-r--r--   0        0        0    12168 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model/choice_model.py
+-rw-r--r--   0        0        0    11494 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model/choice_model_message.py
+-rw-r--r--   0        0        0    11907 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model/inline_object1.py
+-rw-r--r--   0        0        0    11532 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model/inline_response200.py
+-rw-r--r--   0        0        0    11933 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model/inline_response401.py
+-rw-r--r--   0        0        0    12965 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model/inline_response401_error.py
+-rw-r--r--   0        0        0    12874 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model/kb_file_model.py
+-rw-r--r--   0        0        0    11602 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model/knowledge_chat_knowledge_model_name_chat_completions_messages.py
+-rw-r--r--   0        0        0    80638 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model_utils.py
+-rw-r--r--   0        0        0     1364 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/models/__init__.py
+-rw-r--r--   0        0        0    14305 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/rest.py
+-rw-r--r--   0        0        0       32 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/knowledge/__init__.py
+-rw-r--r--   0        0        0    11249 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/knowledge/knowledge.py
+-rw-r--r--   0        0        0      230 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/models/__init__.py
+-rw-r--r--   0        0        0      467 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/models/chat.py
+-rw-r--r--   0        0        0     1519 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/models/file_model.py
+-rw-r--r--   0        0        0    12298 2024-06-03 12:43:01.642692 cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/models/knowledge_model.py
+-rw-r--r--   0        0        0      953 2024-06-03 12:43:23.322859 cosmic_crisp-0.1.0.dev20240603124322/pyproject.toml
+-rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 cosmic_crisp-0.1.0.dev20240603124322/PKG-INFO
```

### Comparing `cosmic_crisp-0.1.0.dev20240602213601/LICENSE.txt` & `cosmic_crisp-0.1.0.dev20240603124322/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/__init__.py` & `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/api/manage_knowledge_models_api.py` & `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/api/manage_knowledge_models_api.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/api_client.py` & `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/api_client.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/apis/__init__.py` & `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/configuration.py` & `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/configuration.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/exceptions.py` & `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/model/inline_object.py` & `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/model/inline_object.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/model/inline_response200.py` & `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/model/inline_response200.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/model/inline_response401.py` & `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/model/inline_response401.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/model/inline_response401_error.py` & `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/model/inline_response401_error.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/model/knowledge_model.py` & `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/model/knowledge_model.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/model_utils.py` & `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/model_utils.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/models/__init__.py` & `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/rest.py` & `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/control/core/client/rest.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/__init__.py` & `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/api/manage_knowledge_models_api.py` & `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/api/manage_knowledge_models_api.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/api_client.py` & `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/api_client.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/apis/__init__.py` & `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/configuration.py` & `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/configuration.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/exceptions.py` & `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model/chat_completion_model.py` & `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model/chat_completion_model.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model/choice_model.py` & `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model/choice_model.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model/choice_model_message.py` & `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model/choice_model_message.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model/inline_object1.py` & `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model/inline_object1.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model/inline_response200.py` & `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model/inline_response200.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model/inline_response401.py` & `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model/inline_response401.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model/inline_response401_error.py` & `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model/inline_response401_error.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model/kb_file_model.py` & `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model/kb_file_model.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model/knowledge_chat_knowledge_model_name_chat_completions_messages.py` & `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model/knowledge_chat_knowledge_model_name_chat_completions_messages.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model_utils.py` & `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/model_utils.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/models/__init__.py` & `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/rest.py` & `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/data/core/client/rest.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/knowledge/knowledge.py` & `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/knowledge/knowledge.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/models/file_model.py` & `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/models/file_model.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/models/knowledge_model.py` & `cosmic_crisp-0.1.0.dev20240603124322/pinecone_plugins/knowledge/models/knowledge_model.py`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240602213601/pyproject.toml` & `cosmic_crisp-0.1.0.dev20240603124322/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cosmic-crisp"
-version = "0.1.0.dev20240602213601"
+version = "0.1.0.dev20240603124322"
 packages = [
     { include = "pinecone_plugins", from = "." },
     # { include = "pinecone.plugins", from = "./pinecone" },
     # { include = "pinecone.plugins.knowledge", from = "./pinecone/plugins" }
 ]
 
 description = "Knowledge plugin for Cosmic Crisp SDK"
@@ -17,18 +17,18 @@
 classifiers=[
         "License :: OSI Approved :: Apache Software License",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pinecone-plugin-interface = "^0.0.6"
-pytest = "^8.2.1"
 
 
 [tool.poetry.group.dev.dependencies]
+pytest = "^8.2.1"
 responses = ">=0.8.1"
 pytest-cov = "^5.0.0"
 pytest-timeout = "^2.3.1"
 torrey = "3.2.2.dev20240602165754"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `cosmic_crisp-0.1.0.dev20240602213601/PKG-INFO` & `cosmic_crisp-0.1.0.dev20240603124322/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: cosmic-crisp
-Version: 0.1.0.dev20240602213601
+Version: 0.1.0.dev20240603124322
 Summary: Knowledge plugin for Cosmic Crisp SDK
 Home-page: https://www.cosmic-crisp.com
 License: Apache-2.0
 Author: Cosmic Crisp Systems, Inc.
 Author-email: support@cosmic-crisp.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pinecone-plugin-interface (>=0.0.6,<0.0.7)
-Requires-Dist: pytest (>=8.2.1,<9.0.0)
 Project-URL: Documentation, https://cosmic-crisp.com/docs
 Description-Content-Type: text/markdown
 
 Nothing to see here.
```
