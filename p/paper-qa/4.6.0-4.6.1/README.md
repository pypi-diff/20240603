# Comparing `tmp/paper_qa-4.6.0.tar.gz` & `tmp/paper_qa-4.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper_qa-4.6.0.tar", last modified: Sat Apr 27 01:40:28 2024, max compression
+gzip compressed data, was "paper_qa-4.6.1.tar", last modified: Mon Jun  3 01:45:52 2024, max compression
```

## Comparing `paper_qa-4.6.0.tar` & `paper_qa-4.6.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:40:28.187847 paper_qa-4.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-27 01:38:35.000000 paper_qa-4.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    31195 2024-04-27 01:40:28.187847 paper_qa-4.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16388 2024-04-27 01:38:35.000000 paper_qa-4.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-27 01:38:35.000000 paper_qa-4.6.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:40:28.183847 paper_qa-4.6.0/paper_qa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    31195 2024-04-27 01:40:28.000000 paper_qa-4.6.0/paper_qa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-27 01:40:28.000000 paper_qa-4.6.0/paper_qa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 01:40:28.000000 paper_qa-4.6.0/paper_qa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-27 01:40:28.000000 paper_qa-4.6.0/paper_qa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-27 01:40:28.000000 paper_qa-4.6.0/paper_qa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:40:28.183847 paper_qa-4.6.0/paperqa/
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-27 01:38:35.000000 paper_qa-4.6.0/paperqa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:40:28.183847 paper_qa-4.6.0/paperqa/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-27 01:38:35.000000 paper_qa-4.6.0/paperqa/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12603 2024-04-27 01:38:35.000000 paper_qa-4.6.0/paperqa/contrib/zotero.py
--rw-r--r--   0 runner    (1001) docker     (127)    32138 2024-04-27 01:38:35.000000 paper_qa-4.6.0/paperqa/docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    32006 2024-04-27 01:38:35.000000 paper_qa-4.6.0/paperqa/llms.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-27 01:38:35.000000 paper_qa-4.6.0/paperqa/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-27 01:38:35.000000 paper_qa-4.6.0/paperqa/prompts.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 01:38:35.000000 paper_qa-4.6.0/paperqa/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-04-27 01:38:35.000000 paper_qa-4.6.0/paperqa/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8262 2024-04-27 01:38:35.000000 paper_qa-4.6.0/paperqa/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-04-27 01:38:35.000000 paper_qa-4.6.0/paperqa/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-27 01:38:35.000000 paper_qa-4.6.0/paperqa/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-04-27 01:38:35.000000 paper_qa-4.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 01:40:28.187847 paper_qa-4.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:40:28.183847 paper_qa-4.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    63137 2024-04-27 01:38:35.000000 paper_qa-4.6.0/tests/test_paperqa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:45:52.773338 paper_qa-4.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-06-03 01:43:27.000000 paper_qa-4.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    31235 2024-06-03 01:45:52.769338 paper_qa-4.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16388 2024-06-03 01:43:27.000000 paper_qa-4.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-06-03 01:43:27.000000 paper_qa-4.6.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:45:52.769338 paper_qa-4.6.1/paper_qa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    31235 2024-06-03 01:45:52.000000 paper_qa-4.6.1/paper_qa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-06-03 01:45:52.000000 paper_qa-4.6.1/paper_qa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 01:45:52.000000 paper_qa-4.6.1/paper_qa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-06-03 01:45:52.000000 paper_qa-4.6.1/paper_qa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-03 01:45:52.000000 paper_qa-4.6.1/paper_qa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:45:52.769338 paper_qa-4.6.1/paperqa/
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-06-03 01:43:27.000000 paper_qa-4.6.1/paperqa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:45:52.769338 paper_qa-4.6.1/paperqa/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-03 01:43:27.000000 paper_qa-4.6.1/paperqa/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12603 2024-06-03 01:43:27.000000 paper_qa-4.6.1/paperqa/contrib/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32883 2024-06-03 01:43:27.000000 paper_qa-4.6.1/paperqa/docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33684 2024-06-03 01:43:27.000000 paper_qa-4.6.1/paperqa/llms.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-06-03 01:43:27.000000 paper_qa-4.6.1/paperqa/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-06-03 01:43:27.000000 paper_qa-4.6.1/paperqa/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 01:43:27.000000 paper_qa-4.6.1/paperqa/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-06-03 01:43:27.000000 paper_qa-4.6.1/paperqa/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8262 2024-06-03 01:43:27.000000 paper_qa-4.6.1/paperqa/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-06-03 01:43:27.000000 paper_qa-4.6.1/paperqa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-06-03 01:43:27.000000 paper_qa-4.6.1/paperqa/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-06-03 01:43:27.000000 paper_qa-4.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 01:45:52.773338 paper_qa-4.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:45:52.769338 paper_qa-4.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    64213 2024-06-03 01:43:27.000000 paper_qa-4.6.1/tests/test_paperqa.py
```

### Comparing `paper_qa-4.6.0/LICENSE` & `paper_qa-4.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `paper_qa-4.6.0/PKG-INFO` & `paper_qa-4.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 4.6.0
+Version: 4.6.1
 Summary: LLM Chain for answering questions from docs
 Author-email: Andrew White <white.d.andrew@gmail.com>
 Maintainer-email: James Braza <jamesbraza@gmail.com>, Andrew White <white.d.andrew@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -233,14 +233,15 @@
 Requires-Dist: langchain-community; extra == "dev"
 Requires-Dist: langchain-openai; extra == "dev"
 Requires-Dist: pymupdf; extra == "dev"
 Requires-Dist: python-dotenv; extra == "dev"
 Requires-Dist: pyzotero; extra == "dev"
 Requires-Dist: requests; extra == "dev"
 Requires-Dist: sentence_transformers; extra == "dev"
+Requires-Dist: voyageai; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: types-requests; extra == "dev"
 Requires-Dist: types-setuptools; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest-sugar; extra == "dev"
```

### Comparing `paper_qa-4.6.0/README.md` & `paper_qa-4.6.1/README.md`

 * *Files identical despite different names*

### Comparing `paper_qa-4.6.0/paper_qa.egg-info/PKG-INFO` & `paper_qa-4.6.1/paper_qa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 4.6.0
+Version: 4.6.1
 Summary: LLM Chain for answering questions from docs
 Author-email: Andrew White <white.d.andrew@gmail.com>
 Maintainer-email: James Braza <jamesbraza@gmail.com>, Andrew White <white.d.andrew@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -233,14 +233,15 @@
 Requires-Dist: langchain-community; extra == "dev"
 Requires-Dist: langchain-openai; extra == "dev"
 Requires-Dist: pymupdf; extra == "dev"
 Requires-Dist: python-dotenv; extra == "dev"
 Requires-Dist: pyzotero; extra == "dev"
 Requires-Dist: requests; extra == "dev"
 Requires-Dist: sentence_transformers; extra == "dev"
+Requires-Dist: voyageai; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: types-requests; extra == "dev"
 Requires-Dist: types-setuptools; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest-sugar; extra == "dev"
```

### Comparing `paper_qa-4.6.0/paperqa/__init__.py` & `paper_qa-4.6.1/paperqa/__init__.py`

 * *Files identical despite different names*

### Comparing `paper_qa-4.6.0/paperqa/contrib/zotero.py` & `paper_qa-4.6.1/paperqa/contrib/zotero.py`

 * *Files identical despite different names*

### Comparing `paper_qa-4.6.0/paperqa/docs.py` & `paper_qa-4.6.1/paperqa/docs.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,21 +10,30 @@
 from pathlib import Path
 from typing import Any, BinaryIO, Callable, Coroutine, cast
 from uuid import UUID, uuid4
 
 from openai import AsyncOpenAI
 from pydantic import BaseModel, ConfigDict, Field, model_validator
 
+try:
+    import voyageai
+
+    USE_VOYAGE = True
+except ImportError:
+    USE_VOYAGE = False
+
+
 from .llms import (
     HybridEmbeddingModel,
     LLMModel,
     NumpyVectorStore,
     OpenAIEmbeddingModel,
     OpenAILLMModel,
     VectorStore,
+    VoyageAIEmbeddingModel,
     get_score,
     llm_model_factory,
     vector_store_factory,
 )
 from .paths import PAPERQA_DIR
 from .readers import read_doc
 from .types import (
@@ -194,26 +203,41 @@
         self,
         client: Any | None = None,
         embedding_client: Any | None = None,
     ):
         if client is None and isinstance(self.llm_model, OpenAILLMModel):
             client = AsyncOpenAI()
         self._client = client
-        if embedding_client is None:  # noqa: SIM102
+        if embedding_client is None:
             # check if we have an openai embedding model in use
             if isinstance(self.texts_index.embedding_model, OpenAIEmbeddingModel) or (
                 isinstance(self.texts_index.embedding_model, HybridEmbeddingModel)
                 and any(
                     isinstance(m, OpenAIEmbeddingModel)
                     for m in self.texts_index.embedding_model.models
                 )
             ):
                 embedding_client = (
                     client if isinstance(client, AsyncOpenAI) else AsyncOpenAI()
                 )
+            elif USE_VOYAGE and (
+                isinstance(self.texts_index.embedding_model, VoyageAIEmbeddingModel)
+                or (
+                    isinstance(self.texts_index.embedding_model, HybridEmbeddingModel)
+                    and any(
+                        isinstance(m, VoyageAIEmbeddingModel)
+                        for m in self.texts_index.embedding_model.models
+                    )
+                )
+            ):
+                embedding_client = (
+                    client
+                    if isinstance(client, voyageai.AsyncClient)
+                    else voyageai.AsyncClient()
+                )
         self._embedding_client = embedding_client
         Docs.make_llm_names_consistent(self)
 
     def _get_unique_name(self, docname: str) -> str:
         """Create a unique name given proposed name."""
         suffix = ""
         while docname + suffix in self.docnames:
```

### Comparing `paper_qa-4.6.0/paperqa/llms.py` & `paper_qa-4.6.1/paperqa/llms.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import asyncio
 import datetime
 import re
 from abc import ABC, abstractmethod
+from enum import Enum
 from inspect import signature
 from typing import Any, AsyncGenerator, Callable, Coroutine, Sequence, cast
 
 import numpy as np
 import tiktoken
 from openai import AsyncOpenAI
 from pydantic import BaseModel, ConfigDict, Field, model_validator
@@ -61,15 +62,15 @@
         return "chat"
     if model_name.startswith("gpt-3.5"):
         return "chat"
     return "completion"
 
 
 def is_openai_model(model_name) -> bool:
-    return model_name.startswith(("gpt-", "babbage", "davinci"))
+    return model_name.startswith(("gpt-", "babbage", "davinci", "ft:gpt-"))
 
 
 def process_llm_config(
     llm_config: dict, max_token_name: str = "max_tokens"  # noqa: S107
 ) -> dict:
     """Remove model_type and try to set max_tokens."""
     result = {k: v for k, v in llm_config.items() if k != "model_type"}
@@ -102,17 +103,25 @@
             input=texts[i : i + batch_size],
             encoding_format="float",
         )
         embeddings.extend([e.embedding for e in response.data])
     return embeddings
 
 
+class EmbeddingModes(str, Enum):
+    DOCUMENT = "document"
+    QUERY = "query"
+
+
 class EmbeddingModel(ABC, BaseModel):
     name: str
 
+    def set_mode(self, mode: EmbeddingModes) -> None:
+        """Several embedding models have a 'mode' or prompt which affects output."""
+
     @abstractmethod
     async def embed_documents(self, client: Any, texts: list[str]) -> list[list[float]]:
         pass
 
 
 class OpenAIEmbeddingModel(EmbeddingModel):
     name: str = Field(default="text-embedding-ada-002")
@@ -145,14 +154,41 @@
     async def embed_documents(self, client, texts):
         all_embeds = await asyncio.gather(
             *[m.embed_documents(client, texts) for m in self.models]
         )
         return np.concatenate(all_embeds, axis=1)
 
 
+class VoyageAIEmbeddingModel(EmbeddingModel):
+    """A wrapper around Voyage AI's client lib."""
+
+    name: str = Field(default="voyage-large-2")
+    embedding_type: EmbeddingModes = Field(default=EmbeddingModes.DOCUMENT)
+    batch_size: int = 10
+
+    def set_mode(self, mode: EmbeddingModes):
+        self.embedding_type = mode
+
+    async def embed_documents(self, client: Any, texts: list[str]) -> list[list[float]]:
+        if client is None:
+            raise ValueError(
+                "Your client is None - did you forget to set it after pickling?"
+            )
+        N = len(texts)
+        embeddings = []
+        for i in range(0, N, self.batch_size):
+            response = await client.embed(
+                texts[i : i + self.batch_size],
+                model=self.name,
+                input_type=self.embedding_type.value,
+            )
+            embeddings.extend(response.embeddings)
+        return embeddings
+
+
 class LLMModel(ABC, BaseModel):
     llm_type: str | None = None
     name: str
     model_config = ConfigDict(extra="forbid")
 
     async def acomplete(self, client: Any, prompt: str) -> str:
         raise NotImplementedError
@@ -611,17 +647,24 @@
 
     async def similarity_search(
         self, client: Any, query: str, k: int
     ) -> tuple[Sequence[Embeddable], list[float]]:
         k = min(k, len(self.texts))
         if k == 0:
             return [], []
+
+        # this will only affect models that embedding prompts
+        self.embedding_model.set_mode(EmbeddingModes.QUERY)
+
         np_query = np.array(
             (await self.embedding_model.embed_documents(client, [query]))[0]
         )
+
+        self.embedding_model.set_mode(EmbeddingModes.DOCUMENT)
+
         similarity_scores = cosine_similarity(
             np_query.reshape(1, -1), self._embeddings_matrix
         )[0]
         similarity_scores = np.nan_to_num(similarity_scores, nan=-np.inf)
         # minus so descending
         # we could use arg-partition here
         # but a lot of algorithms expect a sorted list
@@ -838,19 +881,26 @@
 
 
 def embedding_model_factory(embedding: str, **kwargs) -> EmbeddingModel:
     if embedding == "langchain":
         return LangchainEmbeddingModel(**kwargs)
     if embedding == "sentence-transformers":
         return SentenceTransformerEmbeddingModel(**kwargs)
+    if embedding.startswith("voyage"):
+        return VoyageAIEmbeddingModel(name=embedding, **kwargs)
     if embedding.startswith("hybrid"):
         embedding_model_name = "-".join(embedding.split("-")[1:])
+        dense_model = (
+            OpenAIEmbeddingModel(name=embedding_model_name)
+            if not embedding_model_name.startswith("voyage")
+            else VoyageAIEmbeddingModel(name=embedding_model_name, **kwargs)
+        )
         return HybridEmbeddingModel(
             models=[
-                OpenAIEmbeddingModel(name=embedding_model_name),
+                dense_model,
                 SparseEmbeddingModel(**kwargs),
             ]
         )
     if embedding == "sparse":
         return SparseEmbeddingModel(**kwargs)
     return OpenAIEmbeddingModel(name=embedding, **kwargs)
```

### Comparing `paper_qa-4.6.0/paperqa/prompts.py` & `paper_qa-4.6.1/paperqa/prompts.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,28 +43,30 @@
     "(if the question requires timely information).\n\n"
     "Question: {question}\n\n"
     "Papers: {papers}\n\n"
     "Selected keys:"
 )
 citation_prompt = (
     "Provide the citation for the following text in MLA Format. "
+    "Do not write an introductory sentence. "
     "If reporting date accessed, the current year is 2024\n\n"
     "{text}\n\n"
     "Citation:"
 )
 
 default_system_prompt = (
     "Answer in a direct and concise tone. "
     "Your audience is an expert, so be highly specific. "
-    "If there are ambiguous terms or acronyms, first define them. "
+    "If there are ambiguous terms or acronyms, first define them."
 )
 
+# NOTE: we use double curly braces here so it's not considered an f-string template
 summary_json_system_prompt = """\
 Provide a summary of the relevant information that could help answer the question based on the excerpt. Respond with the following JSON format:
 
 {{
   "summary": "...",
   "relevance_score": "..."
 }}
 
-where `summary` is relevant information from text - {summary_length} words and `relevance_score` is the relevance of `summary` to answer question (out of 10)
+where `summary` is relevant information from text - {summary_length} words and `relevance_score` is the relevance of `summary` to answer question (out of 10).
 """  # noqa: E501
```

### Comparing `paper_qa-4.6.0/paperqa/readers.py` & `paper_qa-4.6.1/paperqa/readers.py`

 * *Files identical despite different names*

### Comparing `paper_qa-4.6.0/paperqa/types.py` & `paper_qa-4.6.1/paperqa/types.py`

 * *Files identical despite different names*

### Comparing `paper_qa-4.6.0/paperqa/utils.py` & `paper_qa-4.6.1/paperqa/utils.py`

 * *Files identical despite different names*

### Comparing `paper_qa-4.6.0/pyproject.toml` & `paper_qa-4.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     {email = "jamesbraza@gmail.com", name = "James Braza"},
     {email = "white.d.andrew@gmail.com", name = "Andrew White"},
 ]
 name = "paper-qa"
 readme = "README.md"
 requires-python = ">=3.8"
 urls = {repository = "https://github.com/whitead/paper-qa"}
-version = "4.6.0"
+version = "4.6.1"
 
 [tool.codespell]
 check-filenames = true
 check-hidden = true
 # SEE: https://github.com/codespell-project/codespell/issues/1212#issuecomment-1744768533
 ignore-regex = ".{1024}|.*codespell-ignore.*"
 ignore-words-list = "aadd,ser"
```

### Comparing `paper_qa-4.6.0/tests/test_paperqa.py` & `paper_qa-4.6.1/tests/test_paperqa.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     LangchainEmbeddingModel,
     LangchainLLMModel,
     LangchainVectorStore,
     LLMModel,
     OpenAIEmbeddingModel,
     OpenAILLMModel,
     SparseEmbeddingModel,
+    VoyageAIEmbeddingModel,
     get_score,
     guess_model_type,
     is_openai_model,
 )
 from paperqa.readers import read_doc
 from paperqa.utils import (
     get_citenames,
@@ -48,14 +49,15 @@
 
 
 def test_is_openai_model():
     assert is_openai_model("gpt-3.5-turbo")
     assert is_openai_model("babbage-002")
     assert is_openai_model("gpt-4-1106-preview")
     assert is_openai_model("davinci-002")
+    assert is_openai_model("ft:gpt-3.5-turbo-0125:my-org::ABC123")
     assert not is_openai_model("llama")
     assert not is_openai_model("labgpt")
     assert not is_openai_model("mixtral-7B")
 
 
 def test_guess_model_type():
     assert guess_model_type("gpt-3.5-turbo") == "chat"
@@ -581,21 +583,22 @@
         Answer(question="For which state was Bates a governor?"),
         detailed_citations=True,
     )
     assert "From WikiMedia Foundation, 2023, Accessed now" in evidence.context
     os.remove(doc_path)
 
 
-def test_json_evidence():
+def test_json_evidence() -> None:
     doc_path = "example.html"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
-        r = requests.get(  # noqa: S113
-            "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)"
+        r = requests.get(
+            "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)", timeout=30.0
         )
+        r.raise_for_status()
         f.write(r.text)
     summary_llm = OpenAILLMModel(
         config={
             "model": "gpt-3.5-turbo-1106",
             "response_format": {"type": "json_object"},
             "temperature": 0.0,
         }
@@ -983,14 +986,42 @@
     docs.add_url(
         "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)",
         citation="WikiMedia Foundation, 2023, Accessed now",
         dockey="test",
     )
 
 
+@pytest.mark.skipif(
+    not os.environ.get("VOYAGE_API_KEY"),
+    reason="Voyage embeddings require a VOYAGE_API_KEY",
+)
+def test_voyage_embeddings():
+    from voyageai import AsyncClient
+
+    docs = Docs(
+        texts_index=NumpyVectorStore(
+            embedding_model=VoyageAIEmbeddingModel(name="voyage-2")
+        ),
+        docs_index=NumpyVectorStore(
+            embedding_model=VoyageAIEmbeddingModel(name="voyage-2")
+        ),
+        embedding_client=AsyncClient(),
+    )
+    assert docs._embedding_client is not None
+
+    docs.add_url(
+        "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)",
+        citation="WikiMedia Foundation, 2023, Accessed now",
+        dockey="test",
+    )
+    assert docs.docs["test"].embedding, "Embedding should not be None"
+    assert any(docs.docs["test"].embedding), "Embeddings are not present"
+    assert len(docs.docs["test"].embedding) == 1024, "Wrong voyage-2 embedding shape"
+
+
 @pytest.mark.asyncio()
 async def test_langchain_vector_store():
     from langchain_community.vectorstores.faiss import FAISS
     from langchain_openai import OpenAIEmbeddings
 
     some_texts = [
         Text(
```

