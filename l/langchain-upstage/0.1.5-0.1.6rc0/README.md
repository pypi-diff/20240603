# Comparing `tmp/langchain_upstage-0.1.5.tar.gz` & `tmp/langchain_upstage-0.1.6rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_upstage-0.1.5.tar", max compression
+gzip compressed data, was "langchain_upstage-0.1.6rc0.tar", max compression
```

## Comparing `langchain_upstage-0.1.5.tar` & `langchain_upstage-0.1.6rc0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1072 2024-05-16 02:51:35.663231 langchain_upstage-0.1.5/LICENSE
--rw-r--r--   0        0        0      979 2024-05-16 02:51:35.663231 langchain_upstage-0.1.5/README.md
--rw-r--r--   0        0        0      567 2024-05-16 02:51:35.663231 langchain_upstage-0.1.5/langchain_upstage/__init__.py
--rw-r--r--   0        0        0     3848 2024-05-16 02:51:35.663231 langchain_upstage-0.1.5/langchain_upstage/chat_models.py
--rw-r--r--   0        0        0     9556 2024-05-16 02:51:35.663231 langchain_upstage-0.1.5/langchain_upstage/embeddings.py
--rw-r--r--   0        0        0     8945 2024-05-16 02:51:35.663231 langchain_upstage-0.1.5/langchain_upstage/layout_analysis.py
--rw-r--r--   0        0        0    13042 2024-05-16 02:51:35.663231 langchain_upstage-0.1.5/langchain_upstage/layout_analysis_parsers.py
--rw-r--r--   0        0        0        0 2024-05-16 02:51:35.663231 langchain_upstage-0.1.5/langchain_upstage/py.typed
--rw-r--r--   0        0        0     4323 2024-05-16 02:51:35.663231 langchain_upstage-0.1.5/langchain_upstage/tools/groundedness_check.py
--rw-r--r--   0        0        0     2738 2024-05-16 02:51:35.663231 langchain_upstage-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1892 1970-01-01 00:00:00.000000 langchain_upstage-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-06-03 13:42:02.050261 langchain_upstage-0.1.6rc0/LICENSE
+-rw-r--r--   0        0        0      965 2024-06-03 13:42:02.050261 langchain_upstage-0.1.6rc0/README.md
+-rw-r--r--   0        0        0      567 2024-06-03 13:42:02.050261 langchain_upstage-0.1.6rc0/langchain_upstage/__init__.py
+-rw-r--r--   0        0        0     4216 2024-06-03 13:42:02.050261 langchain_upstage-0.1.6rc0/langchain_upstage/chat_models.py
+-rw-r--r--   0        0        0     9675 2024-06-03 13:42:02.054261 langchain_upstage-0.1.6rc0/langchain_upstage/embeddings.py
+-rw-r--r--   0        0        0     8945 2024-06-03 13:42:02.054261 langchain_upstage-0.1.6rc0/langchain_upstage/layout_analysis.py
+-rw-r--r--   0        0        0    13144 2024-06-03 13:42:02.054261 langchain_upstage-0.1.6rc0/langchain_upstage/layout_analysis_parsers.py
+-rw-r--r--   0        0        0        0 2024-06-03 13:42:02.054261 langchain_upstage-0.1.6rc0/langchain_upstage/py.typed
+-rw-r--r--   0        0        0     4323 2024-06-03 13:42:02.054261 langchain_upstage-0.1.6rc0/langchain_upstage/tools/groundedness_check.py
+-rw-r--r--   0        0        0     2987 2024-06-03 13:42:02.054261 langchain_upstage-0.1.6rc0/pyproject.toml
+-rw-r--r--   0        0        0     1893 1970-01-01 00:00:00.000000 langchain_upstage-0.1.6rc0/PKG-INFO
```

### Comparing `langchain_upstage-0.1.5/LICENSE` & `langchain_upstage-0.1.6rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_upstage-0.1.5/README.md` & `langchain_upstage-0.1.6rc0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -17,9 +17,9 @@
 
 See a [usage example](https://python.langchain.com/docs/integrations/chat/upstage)
 
 ## Embeddings
 
 See a [usage example](https://python.langchain.com/docs/integrations/text_embedding/upstage)
 
-Use `solar-1-mini-embedding` as the default model for embeddings. Do not add suffixes such as `-query` or `-passage` to the model name.
+Use `solar-embedding-1-large` model for embeddings. Do not add suffixes such as `-query` or `-passage` to the model name.
 `UpstageEmbeddings` will automatically add the suffixes based on the method called.
```

### Comparing `langchain_upstage-0.1.5/langchain_upstage/__init__.py` & `langchain_upstage-0.1.6rc0/langchain_upstage/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_upstage-0.1.5/langchain_upstage/chat_models.py` & `langchain_upstage-0.1.6rc0/langchain_upstage/chat_models.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,15 @@
     Any,
     Dict,
     List,
     Optional,
 )
 
 import openai
+from langchain_core.language_models.chat_models import LangSmithParams
 from langchain_core.pydantic_v1 import Field, SecretStr, root_validator
 from langchain_core.utils import (
     convert_to_secret_str,
     get_from_dict_or_env,
 )
 from langchain_openai.chat_models.base import BaseChatOpenAI
 
@@ -48,14 +49,22 @@
         return attributes
 
     @property
     def _llm_type(self) -> str:
         """Return type of chat model."""
         return "upstage-chat"
 
+    def _get_ls_params(
+        self, stop: Optional[List[str]] = None, **kwargs: Any
+    ) -> LangSmithParams:
+        """Get the parameters used to invoke the model."""
+        params = super()._get_ls_params(stop=stop, **kwargs)
+        params["ls_provider"] = "upstage"
+        return params
+
     model_name: str = Field(default="solar-1-mini-chat", alias="model")
     """Model name to use."""
     upstage_api_key: Optional[SecretStr] = Field(default=None, alias="api_key")
     """Automatically inferred from env are `UPSTAGE_API_KEY` if not provided."""
     upstage_api_base: Optional[str] = Field(
         default="https://api.upstage.ai/v1/solar", alias="base_url"
     )
```

### Comparing `langchain_upstage-0.1.5/langchain_upstage/embeddings.py` & `langchain_upstage-0.1.6rc0/langchain_upstage/embeddings.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     pass it as a named parameter to the constructor.
 
     Example:
         .. code-block:: python
 
             from langchain_upstage import UpstageEmbeddings
 
-            model = UpstageEmbeddings()
+            model = UpstageEmbeddings(model='solar-embedding-1-large')
     """
 
     client: Any = Field(default=None, exclude=True)  #: :meta private:
     async_client: Any = Field(default=None, exclude=True)  #: :meta private:
     model: str = Field(...)
     """Embeddings model name to use. Do not add suffixes like `-query` and `-passage`.
     Instead, use 'solar-embedding-1-large' for example.
@@ -196,14 +196,16 @@
 
         Returns:
             List of embeddings, one for each text.
         """
         assert (
             self.embed_batch_size <= MAX_EMBED_BATCH_SIZE
         ), f"The embed_batch_size should not be larger than {MAX_EMBED_BATCH_SIZE}."
+        if not texts:
+            return []
         params = self._invocation_params
         params["model"] = params["model"] + "-passage"
         embeddings = []
 
         batch_size = min(self.embed_batch_size, len(texts))
         for i in range(0, len(texts), batch_size):
             batch = texts[i : i + batch_size]
@@ -238,14 +240,16 @@
 
         Returns:
             List of embeddings, one for each text.
         """
         assert (
             self.embed_batch_size <= MAX_EMBED_BATCH_SIZE
         ), f"The embed_batch_size should not be larger than {MAX_EMBED_BATCH_SIZE}."
+        if not texts:
+            return []
         params = self._invocation_params
         params["model"] = params["model"] + "-passage"
         embeddings = []
 
         batch_size = min(self.embed_batch_size, len(texts))
         for i in range(0, len(texts), batch_size):
             batch = texts[i : i + batch_size]
```

### Comparing `langchain_upstage-0.1.5/langchain_upstage/layout_analysis.py` & `langchain_upstage-0.1.6rc0/langchain_upstage/layout_analysis.py`

 * *Files identical despite different names*

### Comparing `langchain_upstage-0.1.5/langchain_upstage/layout_analysis_parsers.py` & `langchain_upstage-0.1.6rc0/langchain_upstage/layout_analysis_parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,27 +177,30 @@
             response = requests.post(
                 LAYOUT_ANALYSIS_URL, headers=headers, files=files, data=options
             )
             response.raise_for_status()
 
             result = response.json().get("elements", [])
 
+            elements = [
+                element for element in result if element["category"] not in self.exclude
+            ]
+
+            return elements
+
         except requests.RequestException as req_err:
             # Handle any request-related exceptions
             print(f"Request Exception: {req_err}")
+            raise ValueError(f"Failed to send request: {req_err}")
         except json.JSONDecodeError as json_err:
             # Handle JSON decode errors
             print(f"JSON Decode Error: {json_err}")
             raise ValueError(f"Failed to decode JSON response: {json_err}")
 
-        elements = [
-            element for element in result if element["category"] not in self.exclude
-        ]
-
-        return elements
+        return []
 
     def _split_and_request(
         self,
         full_docs: fitzDocument,
         start_page: int,
         num_pages: int = DEFAULT_NUMBER_OF_PAGE,
     ) -> List:
```

### Comparing `langchain_upstage-0.1.5/langchain_upstage/tools/groundedness_check.py` & `langchain_upstage-0.1.6rc0/langchain_upstage/tools/groundedness_check.py`

 * *Files identical despite different names*

### Comparing `langchain_upstage-0.1.5/PKG-INFO` & `langchain_upstage-0.1.6rc0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: langchain-upstage
-Version: 0.1.5
+Version: 0.1.6rc0
 Summary: An integration package connecting Upstage and LangChain
-Home-page: https://github.com/langchain-ai/langchain
+Home-page: https://github.com/langchain-ai/langchain-upstage
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: langchain-core (>=0.1.52,<0.3)
+Requires-Dist: langchain-core (>=0.2.2,<0.3)
 Requires-Dist: langchain-openai (>=0.1.3,<0.2.0)
 Requires-Dist: pymupdf (>=1.24.1,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Project-URL: Repository, https://github.com/langchain-ai/langchain
-Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/upstage
+Project-URL: Repository, https://github.com/langchain-ai/langchain-upstage
+Project-URL: Source Code, https://github.com/langchain-ai/langchain-upstage/tree/main/libs/upstage
 Description-Content-Type: text/markdown
 
 # langchain-upstage
 
 This package contains the LangChain integrations for [Upstage](https://upstage.ai) through their [APIs](https://developers.upstage.ai/docs/getting-started/models).
 
 ## Installation and Setup
@@ -38,10 +38,10 @@
 
 See a [usage example](https://python.langchain.com/docs/integrations/chat/upstage)
 
 ## Embeddings
 
 See a [usage example](https://python.langchain.com/docs/integrations/text_embedding/upstage)
 
-Use `solar-1-mini-embedding` as the default model for embeddings. Do not add suffixes such as `-query` or `-passage` to the model name.
+Use `solar-embedding-1-large` model for embeddings. Do not add suffixes such as `-query` or `-passage` to the model name.
 `UpstageEmbeddings` will automatically add the suffixes based on the method called.
```

