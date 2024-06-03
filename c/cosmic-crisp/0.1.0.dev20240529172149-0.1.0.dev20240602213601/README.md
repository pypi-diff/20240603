# Comparing `tmp/cosmic_crisp-0.1.0.dev20240529172149.tar.gz` & `tmp/cosmic_crisp-0.1.0.dev20240602213601.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmic_crisp-0.1.0.dev20240529172149.tar", max compression
+gzip compressed data, was "cosmic_crisp-0.1.0.dev20240602213601.tar", max compression
```

## Comparing `cosmic_crisp-0.1.0.dev20240529172149.tar` & `cosmic_crisp-0.1.0.dev20240602213601.tar`

### file list

```diff
@@ -1,37 +1,47 @@
--rw-r--r--   0        0        0    11356 2024-05-29 17:21:35.303923 cosmic_crisp-0.1.0.dev20240529172149/LICENSE.txt
--rw-r--r--   0        0        0       21 2024-05-29 17:21:50.804132 cosmic_crisp-0.1.0.dev20240529172149/README.md
--rw-r--r--   0        0        0      535 2024-05-29 17:21:35.303923 cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/__init__.py
--rw-r--r--   0        0        0     1073 2024-05-29 17:21:35.303923 cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/__init__.py
--rw-r--r--   0        0        0      255 2024-05-29 17:21:35.303923 cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/api/__init__.py
--rw-r--r--   0        0        0    47566 2024-05-29 17:21:35.303923 cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/api/manage_knowledge_bases_api.py
--rw-r--r--   0        0        0    37155 2024-05-29 17:21:35.303923 cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/api_client.py
--rw-r--r--   0        0        0      547 2024-05-29 17:21:35.303923 cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/apis/__init__.py
--rw-r--r--   0        0        0    17197 2024-05-29 17:21:35.303923 cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/configuration.py
--rw-r--r--   0        0        0     5292 2024-05-29 17:21:35.303923 cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/exceptions.py
--rw-r--r--   0        0        0      348 2024-05-29 17:21:35.303923 cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/model/__init__.py
--rw-r--r--   0        0        0    11827 2024-05-29 17:21:35.303923 cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/model/chat_completion_model.py
--rw-r--r--   0        0        0    12131 2024-05-29 17:21:35.303923 cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/model/choice_model.py
--rw-r--r--   0        0        0    11428 2024-05-29 17:21:35.303923 cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/model/choice_model_message.py
--rw-r--r--   0        0        0    12051 2024-05-29 17:21:35.311924 cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/model/context_ref_model.py
--rw-r--r--   0        0        0    12118 2024-05-29 17:21:35.311924 cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/model/inline_object.py
--rw-r--r--   0        0        0    11952 2024-05-29 17:21:35.311924 cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/model/inline_object1.py
--rw-r--r--   0        0        0    11850 2024-05-29 17:21:35.311924 cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/model/inline_object2.py
--rw-r--r--   0        0        0    11560 2024-05-29 17:21:35.311924 cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/model/inline_response200.py
--rw-r--r--   0        0        0    11464 2024-05-29 17:21:35.311924 cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/model/inline_response2001.py
--rw-r--r--   0        0        0    11939 2024-05-29 17:21:35.311924 cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/model/inline_response2002.py
--rw-r--r--   0        0        0    11862 2024-05-29 17:21:35.311924 cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/model/inline_response401.py
--rw-r--r--   0        0        0    12899 2024-05-29 17:21:35.311924 cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/model/inline_response401_error.py
--rw-r--r--   0        0        0    12357 2024-05-29 17:21:35.311924 cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/model/kb_file_model.py
--rw-r--r--   0        0        0    13162 2024-05-29 17:21:35.311924 cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/model/knowledge_base_model.py
--rw-r--r--   0        0        0    11557 2024-05-29 17:21:35.311924 cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/model/knowledge_bases_knowledge_base_name_search_completions_search_context.py
--rw-r--r--   0        0        0    80577 2024-05-29 17:21:35.311924 cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/model_utils.py
--rw-r--r--   0        0        0     1879 2024-05-29 17:21:35.311924 cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/models/__init__.py
--rw-r--r--   0        0        0    14244 2024-05-29 17:21:35.311924 cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/rest.py
--rw-r--r--   0        0        0       32 2024-05-29 17:21:35.311924 cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/knowledge/__init__.py
--rw-r--r--   0        0        0     1843 2024-05-29 17:21:35.311924 cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/knowledge/knowledge.py
--rw-r--r--   0        0        0      157 2024-05-29 17:21:35.311924 cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/models/__init__.py
--rw-r--r--   0        0        0     2683 2024-05-29 17:21:35.311924 cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/models/knowledge_model.py
--rw-r--r--   0        0        0       56 2024-05-29 17:21:35.311924 cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/models/search_context_model.py
--rw-r--r--   0        0        0      316 2024-05-29 17:21:35.311924 cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/models/search_result.py
--rw-r--r--   0        0        0      953 2024-05-29 17:21:50.832133 cosmic_crisp-0.1.0.dev20240529172149/pyproject.toml
--rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 cosmic_crisp-0.1.0.dev20240529172149/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-06-02 21:35:44.049373 cosmic_crisp-0.1.0.dev20240602213601/LICENSE.txt
+-rw-r--r--   0        0        0       21 2024-06-02 21:36:02.781369 cosmic_crisp-0.1.0.dev20240602213601/README.md
+-rw-r--r--   0        0        0      241 2024-06-02 21:35:44.049373 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/__init__.py
+-rw-r--r--   0        0        0     1197 2024-06-02 21:35:44.049373 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/__init__.py
+-rw-r--r--   0        0        0      264 2024-06-02 21:35:44.049373 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/api/__init__.py
+-rw-r--r--   0        0        0    18997 2024-06-02 21:35:44.049373 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/api/manage_knowledge_models_api.py
+-rw-r--r--   0        0        0    37252 2024-06-02 21:35:44.049373 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/api_client.py
+-rw-r--r--   0        0        0      559 2024-06-02 21:35:44.049373 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/apis/__init__.py
+-rw-r--r--   0        0        0    17297 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/configuration.py
+-rw-r--r--   0        0        0     5352 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/exceptions.py
+-rw-r--r--   0        0        0      348 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/model/__init__.py
+-rw-r--r--   0        0        0    12196 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/model/inline_object.py
+-rw-r--r--   0        0        0    11620 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/model/inline_response200.py
+-rw-r--r--   0        0        0    11946 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/model/inline_response401.py
+-rw-r--r--   0        0        0    12975 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/model/inline_response401_error.py
+-rw-r--r--   0        0        0    13045 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/model/knowledge_model.py
+-rw-r--r--   0        0        0    80645 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/model_utils.py
+-rw-r--r--   0        0        0      913 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/models/__init__.py
+-rw-r--r--   0        0        0    14312 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/rest.py
+-rw-r--r--   0        0        0     1169 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/__init__.py
+-rw-r--r--   0        0        0      261 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/api/__init__.py
+-rw-r--r--   0        0        0    25616 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/api/manage_knowledge_models_api.py
+-rw-r--r--   0        0        0    37272 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/api_client.py
+-rw-r--r--   0        0        0      556 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/apis/__init__.py
+-rw-r--r--   0        0        0    17292 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/configuration.py
+-rw-r--r--   0        0        0     5348 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/exceptions.py
+-rw-r--r--   0        0        0      348 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model/__init__.py
+-rw-r--r--   0        0        0    11898 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model/chat_completion_model.py
+-rw-r--r--   0        0        0    12168 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model/choice_model.py
+-rw-r--r--   0        0        0    11494 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model/choice_model_message.py
+-rw-r--r--   0        0        0    11907 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model/inline_object1.py
+-rw-r--r--   0        0        0    11532 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model/inline_response200.py
+-rw-r--r--   0        0        0    11933 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model/inline_response401.py
+-rw-r--r--   0        0        0    12965 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model/inline_response401_error.py
+-rw-r--r--   0        0        0    12874 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model/kb_file_model.py
+-rw-r--r--   0        0        0    11602 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model/knowledge_chat_knowledge_model_name_chat_completions_messages.py
+-rw-r--r--   0        0        0    80638 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model_utils.py
+-rw-r--r--   0        0        0     1364 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/models/__init__.py
+-rw-r--r--   0        0        0    14305 2024-06-02 21:35:44.053372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/rest.py
+-rw-r--r--   0        0        0       32 2024-06-02 21:35:44.057372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/knowledge/__init__.py
+-rw-r--r--   0        0        0    11249 2024-06-02 21:35:44.057372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/knowledge/knowledge.py
+-rw-r--r--   0        0        0      230 2024-06-02 21:35:44.057372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/models/__init__.py
+-rw-r--r--   0        0        0      467 2024-06-02 21:35:44.057372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/models/chat.py
+-rw-r--r--   0        0        0     1519 2024-06-02 21:35:44.057372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/models/file_model.py
+-rw-r--r--   0        0        0    12298 2024-06-02 21:35:44.057372 cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/models/knowledge_model.py
+-rw-r--r--   0        0        0      953 2024-06-02 21:36:02.805369 cosmic_crisp-0.1.0.dev20240602213601/pyproject.toml
+-rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 cosmic_crisp-0.1.0.dev20240602213601/PKG-INFO
```

### Comparing `cosmic_crisp-0.1.0.dev20240529172149/LICENSE.txt` & `cosmic_crisp-0.1.0.dev20240602213601/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/__init__.py` & `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # flake8: noqa
 
 """
     Pinecone Knowledge Engine API
 
-    Pinecone Knowledge Engine is a context engine to store and retrieve relevant knowledge  from millions of documents at scale  # noqa: E501
+    Pinecone Knowledge Engine is a context engine to store and retrieve relevant knowledge  from millions of documents at scale. This API supports creating and managing knowledge models.   # noqa: E501
 
     The version of the OpenAPI document: v1alpha
     Contact: support@pinecone.io
     Generated by: https://openapi-generator.tech
 """
 
 
 __version__ = "1.0.0"
 
 # import ApiClient
-from pinecone_plugins.knowledge.core.client.api_client import ApiClient
+from pinecone_plugins.knowledge.control.core.client.api_client import ApiClient
 
 # import Configuration
-from pinecone_plugins.knowledge.core.client.configuration import Configuration
+from pinecone_plugins.knowledge.control.core.client.configuration import Configuration
 
 # import exceptions
-from pinecone_plugins.knowledge.core.client.exceptions import PineconeException
-from pinecone_plugins.knowledge.core.client.exceptions import PineconeApiAttributeError
-from pinecone_plugins.knowledge.core.client.exceptions import PineconeApiTypeError
-from pinecone_plugins.knowledge.core.client.exceptions import PineconeApiValueError
-from pinecone_plugins.knowledge.core.client.exceptions import PineconeApiKeyError
-from pinecone_plugins.knowledge.core.client.exceptions import PineconeApiException
+from pinecone_plugins.knowledge.control.core.client.exceptions import PineconeException
+from pinecone_plugins.knowledge.control.core.client.exceptions import PineconeApiAttributeError
+from pinecone_plugins.knowledge.control.core.client.exceptions import PineconeApiTypeError
+from pinecone_plugins.knowledge.control.core.client.exceptions import PineconeApiValueError
+from pinecone_plugins.knowledge.control.core.client.exceptions import PineconeApiKeyError
+from pinecone_plugins.knowledge.control.core.client.exceptions import PineconeApiException
```

### Comparing `cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/api_client.py` & `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     Pinecone Knowledge Engine API
 
-    Pinecone Knowledge Engine is a context engine to store and retrieve relevant knowledge  from millions of documents at scale  # noqa: E501
+    Pinecone Knowledge Engine is a context engine to store and retrieve relevant knowledge  from millions of documents at scale. This API supports interactions with knowledge models.   # noqa: E501
 
     The version of the OpenAPI document: v1alpha
     Contact: support@pinecone.io
     Generated by: https://openapi-generator.tech
 """
 
 
@@ -17,18 +17,18 @@
 import os
 import re
 import typing
 from urllib.parse import quote
 from urllib3.fields import RequestField
 
 
-from pinecone_plugins.knowledge.core.client import rest
-from pinecone_plugins.knowledge.core.client.configuration import Configuration
-from pinecone_plugins.knowledge.core.client.exceptions import PineconeApiTypeError, PineconeApiValueError, PineconeApiException
-from pinecone_plugins.knowledge.core.client.model_utils import (
+from pinecone_plugins.knowledge.data.core.client import rest
+from pinecone_plugins.knowledge.data.core.client.configuration import Configuration
+from pinecone_plugins.knowledge.data.core.client.exceptions import PineconeApiTypeError, PineconeApiValueError, PineconeApiException
+from pinecone_plugins.knowledge.data.core.client.model_utils import (
     ModelNormal,
     ModelSimple,
     ModelComposed,
     check_allowed_values,
     check_validations,
     date,
     datetime,
@@ -758,19 +758,19 @@
 
         return params
 
     def __call__(self, *args, **kwargs):
         """ This method is invoked when endpoints are called
         Example:
 
-        api_instance = ManageKnowledgeBasesApi()
-        api_instance.create_knowledge_base  # this is an instance of the class Endpoint
-        api_instance.create_knowledge_base()  # this invokes api_instance.create_knowledge_base.__call__()
+        api_instance = ManageKnowledgeModelsApi()
+        api_instance.chat_completion_knowledge_model  # this is an instance of the class Endpoint
+        api_instance.chat_completion_knowledge_model()  # this invokes api_instance.chat_completion_knowledge_model.__call__()
         which then invokes the callable functions stored in that endpoint at
-        api_instance.create_knowledge_base.callable or self.callable in this class
+        api_instance.chat_completion_knowledge_model.callable or self.callable in this class
 
         """
         return self.callable(self, *args, **kwargs)
 
     def call_with_http_info(self, **kwargs):
 
         try:
```

### Comparing `cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/apis/__init__.py` & `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/apis/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 # flake8: noqa
 
 # Import all APIs into this package.
 # If you have many APIs here with many many models used in each API this may
 # raise a `RecursionError`.
 # In order to avoid this, import only the API that you directly need like:
 #
-#   from .api.manage_knowledge_bases_api import ManageKnowledgeBasesApi
+#   from .api.manage_knowledge_models_api import ManageKnowledgeModelsApi
 #
 # or import this package, but before doing it, use:
 #
 #   import sys
 #   sys.setrecursionlimit(n)
 
 # Import APIs into API package:
-from pinecone_plugins.knowledge.core.client.api.manage_knowledge_bases_api import ManageKnowledgeBasesApi
+from pinecone_plugins.knowledge.control.core.client.api.manage_knowledge_models_api import ManageKnowledgeModelsApi
```

### Comparing `cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/configuration.py` & `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
     Pinecone Knowledge Engine API
 
-    Pinecone Knowledge Engine is a context engine to store and retrieve relevant knowledge  from millions of documents at scale  # noqa: E501
+    Pinecone Knowledge Engine is a context engine to store and retrieve relevant knowledge  from millions of documents at scale. This API supports creating and managing knowledge models.   # noqa: E501
 
     The version of the OpenAPI document: v1alpha
     Contact: support@pinecone.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import copy
 import logging
 import multiprocessing
 import sys
 import urllib3
 
 from http import client as http_client
-from pinecone_plugins.knowledge.core.client.exceptions import PineconeApiValueError
+from pinecone_plugins.knowledge.control.core.client.exceptions import PineconeApiValueError
 
 
 JSON_SCHEMA_VALIDATION_KEYWORDS = {
     'multipleOf', 'maximum', 'exclusiveMaximum',
     'minimum', 'exclusiveMinimum', 'maxLength',
     'minLength', 'pattern', 'maxItems', 'minItems'
 }
@@ -86,15 +86,15 @@
           cookieAuth:         # name for the security scheme
             type: apiKey
             in: cookie
             name: JSESSIONID  # cookie name
 
     You can programmatically set the cookie:
 
-conf = pinecone_plugins.knowledge.core.client.Configuration(
+conf = pinecone_plugins.knowledge.control.core.client.Configuration(
     api_key={'cookieAuth': 'abc123'}
     api_key_prefix={'cookieAuth': 'JSESSIONID'}
 )
 
     The following cookie will be added to the HTTP request:
        Cookie: JSESSIONID abc123
     """
@@ -109,15 +109,15 @@
                  disabled_client_side_validations="",
                  server_index=None, server_variables=None,
                  server_operation_index=None, server_operation_variables=None,
                  ssl_ca_cert=None,
                  ):
         """Constructor
         """
-        self._base_path = "https://api.pinecone.io" if host is None else host
+        self._base_path = "https://api-staging.pinecone.io" if host is None else host
         """Default Base url
         """
         self.server_index = 0 if server_index is None and host is None else server_index
         self.server_operation_index = server_operation_index or {}
         """Default server index
         """
         self.server_variables = server_variables or {}
@@ -149,15 +149,15 @@
         """Password for HTTP basic authentication
         """
         self.discard_unknown_keys = discard_unknown_keys
         self.disabled_client_side_validations = disabled_client_side_validations
         self.logger = {}
         """Logging Settings
         """
-        self.logger["package_logger"] = logging.getLogger("pinecone_plugins.knowledge.core.client")
+        self.logger["package_logger"] = logging.getLogger("pinecone_plugins.knowledge.control.core.client")
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
         self.logger_format = '%(asctime)s %(levelname)s %(message)s'
         """Log format
         """
         self.logger_stream_handler = None
         """Log stream handler
         """
@@ -413,15 +413,15 @@
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
         return [
             {
-                'url': "https://api.pinecone.io",
+                'url': "https://api-staging.pinecone.io",
                 'description': "Production API endpoints",
             }
         ]
 
     def get_host_from_settings(self, index, variables=None, servers=None):
         """Gets host URL based on the index and variables
         :param index: array index of the host settings
```

### Comparing `cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/exceptions.py` & `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     Pinecone Knowledge Engine API
 
-    Pinecone Knowledge Engine is a context engine to store and retrieve relevant knowledge  from millions of documents at scale  # noqa: E501
+    Pinecone Knowledge Engine is a context engine to store and retrieve relevant knowledge  from millions of documents at scale. This API supports creating and managing knowledge models.   # noqa: E501
 
     The version of the OpenAPI document: v1alpha
     Contact: support@pinecone.io
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/model/chat_completion_model.py` & `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model/chat_completion_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Pinecone Knowledge Engine API
 
-    Pinecone Knowledge Engine is a context engine to store and retrieve relevant knowledge  from millions of documents at scale  # noqa: E501
+    Pinecone Knowledge Engine is a context engine to store and retrieve relevant knowledge  from millions of documents at scale. This API supports interactions with knowledge models.   # noqa: E501
 
     The version of the OpenAPI document: v1alpha
     Contact: support@pinecone.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from pinecone_plugins.knowledge.core.client.model_utils import (  # noqa: F401
+from pinecone_plugins.knowledge.data.core.client.model_utils import (  # noqa: F401
     PineconeApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from pinecone_plugins.knowledge.core.client.exceptions import PineconeApiAttributeError
+from pinecone_plugins.knowledge.data.core.client.exceptions import PineconeApiAttributeError
 
 
 def lazy_import():
-    from pinecone_plugins.knowledge.core.client.model.choice_model import ChoiceModel
+    from pinecone_plugins.knowledge.data.core.client.model.choice_model import ChoiceModel
     globals()['ChoiceModel'] = ChoiceModel
 
 
 class ChatCompletionModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/model/choice_model.py` & `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model/choice_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Pinecone Knowledge Engine API
 
-    Pinecone Knowledge Engine is a context engine to store and retrieve relevant knowledge  from millions of documents at scale  # noqa: E501
+    Pinecone Knowledge Engine is a context engine to store and retrieve relevant knowledge  from millions of documents at scale. This API supports interactions with knowledge models.   # noqa: E501
 
     The version of the OpenAPI document: v1alpha
     Contact: support@pinecone.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from pinecone_plugins.knowledge.core.client.model_utils import (  # noqa: F401
+from pinecone_plugins.knowledge.data.core.client.model_utils import (  # noqa: F401
     PineconeApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from pinecone_plugins.knowledge.core.client.exceptions import PineconeApiAttributeError
+from pinecone_plugins.knowledge.data.core.client.exceptions import PineconeApiAttributeError
 
 
 def lazy_import():
-    from pinecone_plugins.knowledge.core.client.model.choice_model_message import ChoiceModelMessage
+    from pinecone_plugins.knowledge.data.core.client.model.choice_model_message import ChoiceModelMessage
     globals()['ChoiceModelMessage'] = ChoiceModelMessage
 
 
 class ChoiceModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -57,19 +57,18 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('finish_reason',): {
-            'STOP': "Stop",
-            'LENGTH': "Length",
-            'TOOLCALLS': "ToolCalls",
-            'CONTENTFILTER': "ContentFilter",
-            'FUNCTIONCALL': "FunctionCall",
+            'STOP': "stop",
+            'LENGTH': "length",
+            'CONTENT_FILTER': "content_filter",
+            'FUNCTION_CALL': "function_call",
         },
     }
 
     validations = {
     }
 
     @cached_property
```

### Comparing `cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/model/choice_model_message.py` & `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model/choice_model_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 """
     Pinecone Knowledge Engine API
 
-    Pinecone Knowledge Engine is a context engine to store and retrieve relevant knowledge  from millions of documents at scale  # noqa: E501
+    Pinecone Knowledge Engine is a context engine to store and retrieve relevant knowledge  from millions of documents at scale. This API supports interactions with knowledge models.   # noqa: E501
 
     The version of the OpenAPI document: v1alpha
     Contact: support@pinecone.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from pinecone_plugins.knowledge.core.client.model_utils import (  # noqa: F401
+from pinecone_plugins.knowledge.data.core.client.model_utils import (  # noqa: F401
     PineconeApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from pinecone_plugins.knowledge.core.client.exceptions import PineconeApiAttributeError
+from pinecone_plugins.knowledge.data.core.client.exceptions import PineconeApiAttributeError
 
 
 
 class ChoiceModelMessage(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/model/context_ref_model.py` & `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model/knowledge_chat_knowledge_model_name_chat_completions_messages.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Pinecone Knowledge Engine API
 
-    Pinecone Knowledge Engine is a context engine to store and retrieve relevant knowledge  from millions of documents at scale  # noqa: E501
+    Pinecone Knowledge Engine is a context engine to store and retrieve relevant knowledge  from millions of documents at scale. This API supports interactions with knowledge models.   # noqa: E501
 
     The version of the OpenAPI document: v1alpha
     Contact: support@pinecone.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from pinecone_plugins.knowledge.core.client.model_utils import (  # noqa: F401
+from pinecone_plugins.knowledge.data.core.client.model_utils import (  # noqa: F401
     PineconeApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from pinecone_plugins.knowledge.core.client.exceptions import PineconeApiAttributeError
+from pinecone_plugins.knowledge.data.core.client.exceptions import PineconeApiAttributeError
 
 
 
-class ContextRefModel(ModelNormal):
+class KnowledgeChatKnowledgeModelNameChatCompletionsMessages(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,50 +78,37 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'id': (str,),  # noqa: E501
-            'source': (str,),  # noqa: E501
-            'text': (str,),  # noqa: E501
-            'score': (float,),  # noqa: E501
-            'path': ([str],),  # noqa: E501
+            'role': (str,),  # noqa: E501
+            'content': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
-        'source': 'source',  # noqa: E501
-        'text': 'text',  # noqa: E501
-        'score': 'score',  # noqa: E501
-        'path': 'path',  # noqa: E501
+        'role': 'role',  # noqa: E501
+        'content': 'content',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, source, text, score, path, *args, **kwargs):  # noqa: E501
-        """ContextRefModel - a model defined in OpenAPI
-
-        Args:
-            id (str):
-            source (str):
-            text (str):
-            score (float):
-            path ([str]):
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """KnowledgeChatKnowledgeModelNameChatCompletionsMessages - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -146,14 +133,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            role (str): [optional]  # noqa: E501
+            content (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -173,19 +162,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
-        self.source = source
-        self.text = text
-        self.score = score
-        self.path = path
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -198,23 +182,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, source, text, score, path, *args, **kwargs):  # noqa: E501
-        """ContextRefModel - a model defined in OpenAPI
-
-        Args:
-            id (str):
-            source (str):
-            text (str):
-            score (float):
-            path ([str]):
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """KnowledgeChatKnowledgeModelNameChatCompletionsMessages - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -239,14 +216,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            role (str): [optional]  # noqa: E501
+            content (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -264,19 +243,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
-        self.source = source
-        self.text = text
-        self.score = score
-        self.path = path
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/model/inline_object.py` & `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/model/inline_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 """
     Pinecone Knowledge Engine API
 
-    Pinecone Knowledge Engine is a context engine to store and retrieve relevant knowledge  from millions of documents at scale  # noqa: E501
+    Pinecone Knowledge Engine is a context engine to store and retrieve relevant knowledge  from millions of documents at scale. This API supports creating and managing knowledge models.   # noqa: E501
 
     The version of the OpenAPI document: v1alpha
     Contact: support@pinecone.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from pinecone_plugins.knowledge.core.client.model_utils import (  # noqa: F401
+from pinecone_plugins.knowledge.control.core.client.model_utils import (  # noqa: F401
     PineconeApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from pinecone_plugins.knowledge.core.client.exceptions import PineconeApiAttributeError
+from pinecone_plugins.knowledge.control.core.client.exceptions import PineconeApiAttributeError
 
 
 
 class InlineObject(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -107,15 +107,15 @@
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
         """InlineObject - a model defined in OpenAPI
 
         Args:
-            name (str): The name of the knowledge base. Resource name must be 1-45 characters long, start and end with an alphanumeric character, and consist only of lower case alphanumeric characters or '-'. 
+            name (str): The name of the knowledge model. Resource name must be 1-45 characters long, start and end with an alphanumeric character, and consist only of lower case alphanumeric characters or '-'. 
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -193,15 +193,15 @@
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, name, *args, **kwargs):  # noqa: E501
         """InlineObject - a model defined in OpenAPI
 
         Args:
-            name (str): The name of the knowledge base. Resource name must be 1-45 characters long, start and end with an alphanumeric character, and consist only of lower case alphanumeric characters or '-'. 
+            name (str): The name of the knowledge model. Resource name must be 1-45 characters long, start and end with an alphanumeric character, and consist only of lower case alphanumeric characters or '-'. 
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/model/inline_object1.py` & `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model/inline_response200.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 """
     Pinecone Knowledge Engine API
 
-    Pinecone Knowledge Engine is a context engine to store and retrieve relevant knowledge  from millions of documents at scale  # noqa: E501
+    Pinecone Knowledge Engine is a context engine to store and retrieve relevant knowledge  from millions of documents at scale. This API supports interactions with knowledge models.   # noqa: E501
 
     The version of the OpenAPI document: v1alpha
     Contact: support@pinecone.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from pinecone_plugins.knowledge.core.client.model_utils import (  # noqa: F401
+from pinecone_plugins.knowledge.data.core.client.model_utils import (  # noqa: F401
     PineconeApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from pinecone_plugins.knowledge.core.client.exceptions import PineconeApiAttributeError
+from pinecone_plugins.knowledge.data.core.client.exceptions import PineconeApiAttributeError
 
 
 def lazy_import():
-    from pinecone_plugins.knowledge.core.client.model.knowledge_bases_knowledge_base_name_search_completions_search_context import KnowledgeBasesKnowledgeBaseNameSearchCompletionsSearchContext
-    globals()['KnowledgeBasesKnowledgeBaseNameSearchCompletionsSearchContext'] = KnowledgeBasesKnowledgeBaseNameSearchCompletionsSearchContext
+    from pinecone_plugins.knowledge.data.core.client.model.kb_file_model import KBFileModel
+    globals()['KBFileModel'] = KBFileModel
 
 
-class InlineObject1(ModelNormal):
+class InlineResponse200(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,38 +84,35 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'search_context': ([KnowledgeBasesKnowledgeBaseNameSearchCompletionsSearchContext],),  # noqa: E501
+            'files': ([KBFileModel],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'search_context': 'search_context',  # noqa: E501
+        'files': 'files',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, search_context, *args, **kwargs):  # noqa: E501
-        """InlineObject1 - a model defined in OpenAPI
-
-        Args:
-            search_context ([KnowledgeBasesKnowledgeBaseNameSearchCompletionsSearchContext]):
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """InlineResponse200 - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -140,14 +137,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            files ([KBFileModel]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -167,15 +165,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.search_context = search_context
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -188,19 +185,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, search_context, *args, **kwargs):  # noqa: E501
-        """InlineObject1 - a model defined in OpenAPI
-
-        Args:
-            search_context ([KnowledgeBasesKnowledgeBaseNameSearchCompletionsSearchContext]):
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """InlineResponse200 - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -225,14 +219,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            files ([KBFileModel]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -250,15 +245,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.search_context = search_context
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/model/inline_object2.py` & `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model/inline_response401.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 """
     Pinecone Knowledge Engine API
 
-    Pinecone Knowledge Engine is a context engine to store and retrieve relevant knowledge  from millions of documents at scale  # noqa: E501
+    Pinecone Knowledge Engine is a context engine to store and retrieve relevant knowledge  from millions of documents at scale. This API supports interactions with knowledge models.   # noqa: E501
 
     The version of the OpenAPI document: v1alpha
     Contact: support@pinecone.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from pinecone_plugins.knowledge.core.client.model_utils import (  # noqa: F401
+from pinecone_plugins.knowledge.data.core.client.model_utils import (  # noqa: F401
     PineconeApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from pinecone_plugins.knowledge.core.client.exceptions import PineconeApiAttributeError
+from pinecone_plugins.knowledge.data.core.client.exceptions import PineconeApiAttributeError
 
 
 def lazy_import():
-    from pinecone_plugins.knowledge.core.client.model.knowledge_bases_knowledge_base_name_search_completions_search_context import KnowledgeBasesKnowledgeBaseNameSearchCompletionsSearchContext
-    globals()['KnowledgeBasesKnowledgeBaseNameSearchCompletionsSearchContext'] = KnowledgeBasesKnowledgeBaseNameSearchCompletionsSearchContext
+    from pinecone_plugins.knowledge.data.core.client.model.inline_response401_error import InlineResponse401Error
+    globals()['InlineResponse401Error'] = InlineResponse401Error
 
 
-class InlineObject2(ModelNormal):
+class InlineResponse401(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,35 +84,41 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'search_context': ([KnowledgeBasesKnowledgeBaseNameSearchCompletionsSearchContext],),  # noqa: E501
+            'status': (int,),  # noqa: E501
+            'error': (InlineResponse401Error,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'search_context': 'search_context',  # noqa: E501
+        'status': 'status',  # noqa: E501
+        'error': 'error',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """InlineObject2 - a model defined in OpenAPI
+    def _from_openapi_data(cls, status, error, *args, **kwargs):  # noqa: E501
+        """InlineResponse401 - a model defined in OpenAPI
+
+        Args:
+            status (int): The HTTP status code of the error.
+            error (InlineResponse401Error):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -137,15 +143,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            search_context ([KnowledgeBasesKnowledgeBaseNameSearchCompletionsSearchContext]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -165,14 +170,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.status = status
+        self.error = error
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -185,16 +192,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """InlineObject2 - a model defined in OpenAPI
+    def __init__(self, status, error, *args, **kwargs):  # noqa: E501
+        """InlineResponse401 - a model defined in OpenAPI
+
+        Args:
+            status (int): The HTTP status code of the error.
+            error (InlineResponse401Error):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -219,15 +230,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            search_context ([KnowledgeBasesKnowledgeBaseNameSearchCompletionsSearchContext]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -245,14 +255,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.status = status
+        self.error = error
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/model/inline_response200.py` & `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/model/inline_response200.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Pinecone Knowledge Engine API
 
-    Pinecone Knowledge Engine is a context engine to store and retrieve relevant knowledge  from millions of documents at scale  # noqa: E501
+    Pinecone Knowledge Engine is a context engine to store and retrieve relevant knowledge  from millions of documents at scale. This API supports creating and managing knowledge models.   # noqa: E501
 
     The version of the OpenAPI document: v1alpha
     Contact: support@pinecone.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from pinecone_plugins.knowledge.core.client.model_utils import (  # noqa: F401
+from pinecone_plugins.knowledge.control.core.client.model_utils import (  # noqa: F401
     PineconeApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from pinecone_plugins.knowledge.core.client.exceptions import PineconeApiAttributeError
+from pinecone_plugins.knowledge.control.core.client.exceptions import PineconeApiAttributeError
 
 
 def lazy_import():
-    from pinecone_plugins.knowledge.core.client.model.knowledge_base_model import KnowledgeBaseModel
-    globals()['KnowledgeBaseModel'] = KnowledgeBaseModel
+    from pinecone_plugins.knowledge.control.core.client.model.knowledge_model import KnowledgeModel
+    globals()['KnowledgeModel'] = KnowledgeModel
 
 
 class InlineResponse200(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -84,24 +84,24 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'knowledge_bases': ([KnowledgeBaseModel],),  # noqa: E501
+            'knowledge_models': ([KnowledgeModel],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'knowledge_bases': 'knowledge_bases',  # noqa: E501
+        'knowledge_models': 'knowledge_models',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -137,15 +137,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            knowledge_bases ([KnowledgeBaseModel]): [optional]  # noqa: E501
+            knowledge_models ([KnowledgeModel]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -219,15 +219,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            knowledge_bases ([KnowledgeBaseModel]): [optional]  # noqa: E501
+            knowledge_models ([KnowledgeModel]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/model/inline_response2001.py` & `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model/kb_file_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,41 @@
 """
     Pinecone Knowledge Engine API
 
-    Pinecone Knowledge Engine is a context engine to store and retrieve relevant knowledge  from millions of documents at scale  # noqa: E501
+    Pinecone Knowledge Engine is a context engine to store and retrieve relevant knowledge  from millions of documents at scale. This API supports interactions with knowledge models.   # noqa: E501
 
     The version of the OpenAPI document: v1alpha
     Contact: support@pinecone.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from pinecone_plugins.knowledge.core.client.model_utils import (  # noqa: F401
+from pinecone_plugins.knowledge.data.core.client.model_utils import (  # noqa: F401
     PineconeApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from pinecone_plugins.knowledge.core.client.exceptions import PineconeApiAttributeError
+from pinecone_plugins.knowledge.data.core.client.exceptions import PineconeApiAttributeError
 
 
-def lazy_import():
-    from pinecone_plugins.knowledge.core.client.model.kb_file_model import KBFileModel
-    globals()['KBFileModel'] = KBFileModel
 
-
-class InlineResponse2001(ModelNormal):
+class KBFileModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -56,63 +52,82 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
+        ('status',): {
+            'PROCESSING': "Processing",
+            'AVAILABLE': "Available",
+            'DELETING': "Deleting",
+        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'files': ([KBFileModel],),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'id': (str,),  # noqa: E501
+            'metadata': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type,),  # noqa: E501
+            'mime_type': (str,),  # noqa: E501
+            'created_on': (str,),  # noqa: E501
+            'updated_on': (str,),  # noqa: E501
+            'status': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'files': 'files',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'metadata': 'metadata',  # noqa: E501
+        'mime_type': 'mime_type',  # noqa: E501
+        'created_on': 'created_on',  # noqa: E501
+        'updated_on': 'updated_on',  # noqa: E501
+        'status': 'status',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """InlineResponse2001 - a model defined in OpenAPI
+    def _from_openapi_data(cls, name, id, *args, **kwargs):  # noqa: E501
+        """KBFileModel - a model defined in OpenAPI
+
+        Args:
+            name (str):
+            id (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -137,15 +152,19 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            files ([KBFileModel]): [optional]  # noqa: E501
+            metadata ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): [optional]  # noqa: E501
+            mime_type (str): [optional]  # noqa: E501
+            created_on (str): [optional]  # noqa: E501
+            updated_on (str): [optional]  # noqa: E501
+            status (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -165,14 +184,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.name = name
+        self.id = id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -185,16 +206,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """InlineResponse2001 - a model defined in OpenAPI
+    def __init__(self, name, id, *args, **kwargs):  # noqa: E501
+        """KBFileModel - a model defined in OpenAPI
+
+        Args:
+            name (str):
+            id (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -219,15 +244,19 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            files ([KBFileModel]): [optional]  # noqa: E501
+            metadata ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): [optional]  # noqa: E501
+            mime_type (str): [optional]  # noqa: E501
+            created_on (str): [optional]  # noqa: E501
+            updated_on (str): [optional]  # noqa: E501
+            status (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -245,14 +274,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.name = name
+        self.id = id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/model/inline_response2002.py` & `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/model/inline_response401.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 """
     Pinecone Knowledge Engine API
 
-    Pinecone Knowledge Engine is a context engine to store and retrieve relevant knowledge  from millions of documents at scale  # noqa: E501
+    Pinecone Knowledge Engine is a context engine to store and retrieve relevant knowledge  from millions of documents at scale. This API supports creating and managing knowledge models.   # noqa: E501
 
     The version of the OpenAPI document: v1alpha
     Contact: support@pinecone.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from pinecone_plugins.knowledge.core.client.model_utils import (  # noqa: F401
+from pinecone_plugins.knowledge.control.core.client.model_utils import (  # noqa: F401
     PineconeApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from pinecone_plugins.knowledge.core.client.exceptions import PineconeApiAttributeError
+from pinecone_plugins.knowledge.control.core.client.exceptions import PineconeApiAttributeError
 
 
 def lazy_import():
-    from pinecone_plugins.knowledge.core.client.model.chat_completion_model import ChatCompletionModel
-    from pinecone_plugins.knowledge.core.client.model.context_ref_model import ContextRefModel
-    globals()['ChatCompletionModel'] = ChatCompletionModel
-    globals()['ContextRefModel'] = ContextRefModel
+    from pinecone_plugins.knowledge.control.core.client.model.inline_response401_error import InlineResponse401Error
+    globals()['InlineResponse401Error'] = InlineResponse401Error
 
 
-class InlineResponse2002(ModelNormal):
+class InlineResponse401(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -86,37 +84,41 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'chat_completion': (ChatCompletionModel,),  # noqa: E501
-            'context': (ContextRefModel,),  # noqa: E501
+            'status': (int,),  # noqa: E501
+            'error': (InlineResponse401Error,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'chat_completion': 'chat_completion',  # noqa: E501
-        'context': 'context',  # noqa: E501
+        'status': 'status',  # noqa: E501
+        'error': 'error',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """InlineResponse2002 - a model defined in OpenAPI
+    def _from_openapi_data(cls, status, error, *args, **kwargs):  # noqa: E501
+        """InlineResponse401 - a model defined in OpenAPI
+
+        Args:
+            status (int): The HTTP status code of the error.
+            error (InlineResponse401Error):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -141,16 +143,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            chat_completion (ChatCompletionModel): [optional]  # noqa: E501
-            context (ContextRefModel): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -170,14 +170,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.status = status
+        self.error = error
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -190,16 +192,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """InlineResponse2002 - a model defined in OpenAPI
+    def __init__(self, status, error, *args, **kwargs):  # noqa: E501
+        """InlineResponse401 - a model defined in OpenAPI
+
+        Args:
+            status (int): The HTTP status code of the error.
+            error (InlineResponse401Error):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -224,16 +230,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            chat_completion (ChatCompletionModel): [optional]  # noqa: E501
-            context (ContextRefModel): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -251,14 +255,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.status = status
+        self.error = error
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/model/inline_response401.py` & `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/model/inline_response401_error.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,41 @@
 """
     Pinecone Knowledge Engine API
 
-    Pinecone Knowledge Engine is a context engine to store and retrieve relevant knowledge  from millions of documents at scale  # noqa: E501
+    Pinecone Knowledge Engine is a context engine to store and retrieve relevant knowledge  from millions of documents at scale. This API supports creating and managing knowledge models.   # noqa: E501
 
     The version of the OpenAPI document: v1alpha
     Contact: support@pinecone.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from pinecone_plugins.knowledge.core.client.model_utils import (  # noqa: F401
+from pinecone_plugins.knowledge.control.core.client.model_utils import (  # noqa: F401
     PineconeApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from pinecone_plugins.knowledge.core.client.exceptions import PineconeApiAttributeError
+from pinecone_plugins.knowledge.control.core.client.exceptions import PineconeApiAttributeError
 
 
-def lazy_import():
-    from pinecone_plugins.knowledge.core.client.model.inline_response401_error import InlineResponse401Error
-    globals()['InlineResponse401Error'] = InlineResponse401Error
 
-
-class InlineResponse401(ModelNormal):
+class InlineResponse401Error(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -56,69 +52,89 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
+        ('code',): {
+            'OK': "OK",
+            'UNKNOWN': "UNKNOWN",
+            'INVALID_ARGUMENT': "INVALID_ARGUMENT",
+            'DEADLINE_EXCEEDED': "DEADLINE_EXCEEDED",
+            'QUOTA_EXCEEDED': "QUOTA_EXCEEDED",
+            'NOT_FOUND': "NOT_FOUND",
+            'ALREADY_EXISTS': "ALREADY_EXISTS",
+            'PERMISSION_DENIED': "PERMISSION_DENIED",
+            'UNAUTHENTICATED': "UNAUTHENTICATED",
+            'RESOURCE_EXHAUSTED': "RESOURCE_EXHAUSTED",
+            'FAILED_PRECONDITION': "FAILED_PRECONDITION",
+            'ABORTED': "ABORTED",
+            'OUT_OF_RANGE': "OUT_OF_RANGE",
+            'UNIMPLEMENTED': "UNIMPLEMENTED",
+            'INTERNAL': "INTERNAL",
+            'UNAVAILABLE': "UNAVAILABLE",
+            'DATA_LOSS': "DATA_LOSS",
+            'FORBIDDEN': "FORBIDDEN",
+        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'status': (int,),  # noqa: E501
-            'error': (InlineResponse401Error,),  # noqa: E501
+            'code': (str,),  # noqa: E501
+            'message': (str,),  # noqa: E501
+            'details': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'status': 'status',  # noqa: E501
-        'error': 'error',  # noqa: E501
+        'code': 'code',  # noqa: E501
+        'message': 'message',  # noqa: E501
+        'details': 'details',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, status, error, *args, **kwargs):  # noqa: E501
-        """InlineResponse401 - a model defined in OpenAPI
+    def _from_openapi_data(cls, code, message, *args, **kwargs):  # noqa: E501
+        """InlineResponse401Error - a model defined in OpenAPI
 
         Args:
-            status (int): The HTTP status code of the error.
-            error (InlineResponse401Error):
+            code (str):
+            message (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -143,14 +159,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            details ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Additional information about the error. This field is not guaranteed to be present.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -170,16 +187,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.status = status
-        self.error = error
+        self.code = code
+        self.message = message
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -192,20 +209,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, status, error, *args, **kwargs):  # noqa: E501
-        """InlineResponse401 - a model defined in OpenAPI
+    def __init__(self, code, message, *args, **kwargs):  # noqa: E501
+        """InlineResponse401Error - a model defined in OpenAPI
 
         Args:
-            status (int): The HTTP status code of the error.
-            error (InlineResponse401Error):
+            code (str):
+            message (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -230,14 +247,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            details ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Additional information about the error. This field is not guaranteed to be present.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -255,16 +273,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.status = status
-        self.error = error
+        self.code = code
+        self.message = message
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/model/inline_response401_error.py` & `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model/inline_response401_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 """
     Pinecone Knowledge Engine API
 
-    Pinecone Knowledge Engine is a context engine to store and retrieve relevant knowledge  from millions of documents at scale  # noqa: E501
+    Pinecone Knowledge Engine is a context engine to store and retrieve relevant knowledge  from millions of documents at scale. This API supports interactions with knowledge models.   # noqa: E501
 
     The version of the OpenAPI document: v1alpha
     Contact: support@pinecone.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from pinecone_plugins.knowledge.core.client.model_utils import (  # noqa: F401
+from pinecone_plugins.knowledge.data.core.client.model_utils import (  # noqa: F401
     PineconeApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from pinecone_plugins.knowledge.core.client.exceptions import PineconeApiAttributeError
+from pinecone_plugins.knowledge.data.core.client.exceptions import PineconeApiAttributeError
 
 
 
 class InlineResponse401Error(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/model/kb_file_model.py` & `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/model/knowledge_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Pinecone Knowledge Engine API
 
-    Pinecone Knowledge Engine is a context engine to store and retrieve relevant knowledge  from millions of documents at scale  # noqa: E501
+    Pinecone Knowledge Engine is a context engine to store and retrieve relevant knowledge  from millions of documents at scale. This API supports creating and managing knowledge models.   # noqa: E501
 
     The version of the OpenAPI document: v1alpha
     Contact: support@pinecone.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from pinecone_plugins.knowledge.core.client.model_utils import (  # noqa: F401
+from pinecone_plugins.knowledge.control.core.client.model_utils import (  # noqa: F401
     PineconeApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from pinecone_plugins.knowledge.core.client.exceptions import PineconeApiAttributeError
+from pinecone_plugins.knowledge.control.core.client.exceptions import PineconeApiAttributeError
 
 
 
-class KBFileModel(ModelNormal):
+class KnowledgeModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -53,21 +53,26 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('status',): {
-            'PROCESSING': "Processing",
-            'AVAILABLE': "Available",
-            'DELETED': "Deleted",
+            'INITIALIZING': "Initializing",
+            'FAILED': "Failed",
+            'READY': "Ready",
+            'TERMINATING': "Terminating",
         },
     }
 
     validations = {
+        ('name',): {
+            'max_length': 45,
+            'min_length': 1,
+        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
@@ -84,46 +89,46 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'name': (str,),  # noqa: E501
-            'id': (str,),  # noqa: E501
-            'metadata': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
-            'mime_type': (str,),  # noqa: E501
             'status': (str,),  # noqa: E501
+            'metadata': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type,),  # noqa: E501
+            'created_at': (str,),  # noqa: E501
+            'updated_at': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
-        'id': 'id',  # noqa: E501
-        'metadata': 'metadata',  # noqa: E501
-        'mime_type': 'mime_type',  # noqa: E501
         'status': 'status',  # noqa: E501
+        'metadata': 'metadata',  # noqa: E501
+        'created_at': 'created_at',  # noqa: E501
+        'updated_at': 'updated_at',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, name, id, *args, **kwargs):  # noqa: E501
-        """KBFileModel - a model defined in OpenAPI
+    def _from_openapi_data(cls, name, status, *args, **kwargs):  # noqa: E501
+        """KnowledgeModel - a model defined in OpenAPI
 
         Args:
-            name (str):
-            id (str):
+            name (str): The name of the knowledge model. Resource name must be 1-45 characters long, start and end with an alphanumeric character, and consist only of lower case alphanumeric characters or '-'. 
+            status (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -148,17 +153,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            metadata ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
-            mime_type (str): [optional]  # noqa: E501
-            status (str): [optional]  # noqa: E501
+            metadata ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): [optional]  # noqa: E501
+            created_at (str): [optional]  # noqa: E501
+            updated_at (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -179,15 +184,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.name = name
-        self.id = id
+        self.status = status
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -200,20 +205,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, name, id, *args, **kwargs):  # noqa: E501
-        """KBFileModel - a model defined in OpenAPI
+    def __init__(self, name, status, *args, **kwargs):  # noqa: E501
+        """KnowledgeModel - a model defined in OpenAPI
 
         Args:
-            name (str):
-            id (str):
+            name (str): The name of the knowledge model. Resource name must be 1-45 characters long, start and end with an alphanumeric character, and consist only of lower case alphanumeric characters or '-'. 
+            status (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -238,17 +243,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            metadata ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
-            mime_type (str): [optional]  # noqa: E501
-            status (str): [optional]  # noqa: E501
+            metadata ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): [optional]  # noqa: E501
+            created_at (str): [optional]  # noqa: E501
+            updated_at (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -267,15 +272,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.name = name
-        self.id = id
+        self.status = status
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/model/knowledge_base_model.py` & `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/model/inline_object1.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 """
     Pinecone Knowledge Engine API
 
-    Pinecone Knowledge Engine is a context engine to store and retrieve relevant knowledge  from millions of documents at scale  # noqa: E501
+    Pinecone Knowledge Engine is a context engine to store and retrieve relevant knowledge  from millions of documents at scale. This API supports interactions with knowledge models.   # noqa: E501
 
     The version of the OpenAPI document: v1alpha
     Contact: support@pinecone.io
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from pinecone_plugins.knowledge.core.client.model_utils import (  # noqa: F401
+from pinecone_plugins.knowledge.data.core.client.model_utils import (  # noqa: F401
     PineconeApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
-from pinecone_plugins.knowledge.core.client.exceptions import PineconeApiAttributeError
+from pinecone_plugins.knowledge.data.core.client.exceptions import PineconeApiAttributeError
 
 
+def lazy_import():
+    from pinecone_plugins.knowledge.data.core.client.model.knowledge_chat_knowledge_model_name_chat_completions_messages import KnowledgeChatKnowledgeModelNameChatCompletionsMessages
+    globals()['KnowledgeChatKnowledgeModelNameChatCompletionsMessages'] = KnowledgeChatKnowledgeModelNameChatCompletionsMessages
 
-class KnowledgeBaseModel(ModelNormal):
+
+class InlineObject1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -52,85 +56,66 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('status',): {
-            'INITIALIZING': "Initializing",
-            'FAILED': "Failed",
-            'READY': "Ready",
-            'TERMINATING': "Terminating",
-        },
     }
 
     validations = {
-        ('name',): {
-            'max_length': 45,
-            'min_length': 1,
-        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'name': (str,),  # noqa: E501
-            'status': (str,),  # noqa: E501
-            'metadata': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
-            'ready': (bool,),  # noqa: E501
-            'created_at': (datetime,),  # noqa: E501
-            'updated_at': (datetime,),  # noqa: E501
+            'messages': ([KnowledgeChatKnowledgeModelNameChatCompletionsMessages],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'name': 'name',  # noqa: E501
-        'status': 'status',  # noqa: E501
-        'metadata': 'metadata',  # noqa: E501
-        'ready': 'ready',  # noqa: E501
-        'created_at': 'created_at',  # noqa: E501
-        'updated_at': 'updated_at',  # noqa: E501
+        'messages': 'messages',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, name, status, *args, **kwargs):  # noqa: E501
-        """KnowledgeBaseModel - a model defined in OpenAPI
+    def _from_openapi_data(cls, messages, *args, **kwargs):  # noqa: E501
+        """InlineObject1 - a model defined in OpenAPI
 
         Args:
-            name (str): The name of the knowledge base. Resource name must be 1-45 characters long, start and end with an alphanumeric character, and consist only of lower case alphanumeric characters or '-'. 
-            status (str):
+            messages ([KnowledgeChatKnowledgeModelNameChatCompletionsMessages]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -155,18 +140,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            metadata ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
-            ready (bool): [optional]  # noqa: E501
-            created_at (datetime): [optional]  # noqa: E501
-            updated_at (datetime): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -186,16 +167,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.name = name
-        self.status = status
+        self.messages = messages
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -208,20 +188,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, name, status, *args, **kwargs):  # noqa: E501
-        """KnowledgeBaseModel - a model defined in OpenAPI
+    def __init__(self, messages, *args, **kwargs):  # noqa: E501
+        """InlineObject1 - a model defined in OpenAPI
 
         Args:
-            name (str): The name of the knowledge base. Resource name must be 1-45 characters long, start and end with an alphanumeric character, and consist only of lower case alphanumeric characters or '-'. 
-            status (str):
+            messages ([KnowledgeChatKnowledgeModelNameChatCompletionsMessages]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -246,18 +225,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            metadata ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
-            ready (bool): [optional]  # noqa: E501
-            created_at (datetime): [optional]  # noqa: E501
-            updated_at (datetime): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -275,16 +250,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.name = name
-        self.status = status
+        self.messages = messages
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/model_utils.py` & `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/control/core/client/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     Pinecone Knowledge Engine API
 
-    Pinecone Knowledge Engine is a context engine to store and retrieve relevant knowledge  from millions of documents at scale  # noqa: E501
+    Pinecone Knowledge Engine is a context engine to store and retrieve relevant knowledge  from millions of documents at scale. This API supports creating and managing knowledge models.   # noqa: E501
 
     The version of the OpenAPI document: v1alpha
     Contact: support@pinecone.io
     Generated by: https://openapi-generator.tech
 """
 
 
@@ -13,15 +13,15 @@
 import inspect
 import io
 import os
 import pprint
 import re
 import tempfile
 
-from pinecone_plugins.knowledge.core.client.exceptions import (
+from pinecone_plugins.knowledge.control.core.client.exceptions import (
     PineconeApiKeyError,
     PineconeApiAttributeError,
     PineconeApiTypeError,
     PineconeApiValueError,
 )
 
 none_type = type(None)
```

### Comparing `cosmic_crisp-0.1.0.dev20240529172149/pinecone_plugins/knowledge/core/client/rest.py` & `cosmic_crisp-0.1.0.dev20240602213601/pinecone_plugins/knowledge/data/core/client/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     Pinecone Knowledge Engine API
 
-    Pinecone Knowledge Engine is a context engine to store and retrieve relevant knowledge  from millions of documents at scale  # noqa: E501
+    Pinecone Knowledge Engine is a context engine to store and retrieve relevant knowledge  from millions of documents at scale. This API supports interactions with knowledge models.   # noqa: E501
 
     The version of the OpenAPI document: v1alpha
     Contact: support@pinecone.io
     Generated by: https://openapi-generator.tech
 """
 
 
@@ -15,15 +15,15 @@
 import re
 import ssl
 import os
 from urllib.parse import urlencode
 
 import urllib3
 
-from pinecone_plugins.knowledge.core.client.exceptions import PineconeApiException, UnauthorizedException, ForbiddenException, NotFoundException, ServiceException, PineconeApiValueError
+from pinecone_plugins.knowledge.data.core.client.exceptions import PineconeApiException, UnauthorizedException, ForbiddenException, NotFoundException, ServiceException, PineconeApiValueError
 
 
 class bcolors:
     HEADER = '\033[95m'
     OKBLUE = '\033[94m'
     OKCYAN = '\033[96m'
     OKGREEN = '\033[92m'
```

### Comparing `cosmic_crisp-0.1.0.dev20240529172149/pyproject.toml` & `cosmic_crisp-0.1.0.dev20240602213601/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cosmic-crisp"
-version = "0.1.0.dev20240529172149"
+version = "0.1.0.dev20240602213601"
 packages = [
     { include = "pinecone_plugins", from = "." },
     # { include = "pinecone.plugins", from = "./pinecone" },
     # { include = "pinecone.plugins.knowledge", from = "./pinecone/plugins" }
 ]
 
 description = "Knowledge plugin for Cosmic Crisp SDK"
@@ -16,20 +16,20 @@
 keywords = []
 classifiers=[
         "License :: OSI Approved :: Apache Software License",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pinecone-plugin-interface = "^0.0.5"
+pinecone-plugin-interface = "^0.0.6"
+pytest = "^8.2.1"
 
 
 [tool.poetry.group.dev.dependencies]
-pytest = "8.0.0"
 responses = ">=0.8.1"
 pytest-cov = "^5.0.0"
 pytest-timeout = "^2.3.1"
-torrey = "^3.2.2.dev20240529142438"
+torrey = "3.2.2.dev20240602165754"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cosmic_crisp-0.1.0.dev20240529172149/PKG-INFO` & `cosmic_crisp-0.1.0.dev20240602213601/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: cosmic-crisp
-Version: 0.1.0.dev20240529172149
+Version: 0.1.0.dev20240602213601
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
-Requires-Dist: pinecone-plugin-interface (>=0.0.5,<0.0.6)
+Requires-Dist: pinecone-plugin-interface (>=0.0.6,<0.0.7)
+Requires-Dist: pytest (>=8.2.1,<9.0.0)
 Project-URL: Documentation, https://cosmic-crisp.com/docs
 Description-Content-Type: text/markdown
 
 Nothing to see here.
```

