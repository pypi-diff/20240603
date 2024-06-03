# Comparing `tmp/onprem-0.1.0.tar.gz` & `tmp/onprem-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onprem-0.1.0.tar", last modified: Wed May 29 16:25:41 2024, max compression
+gzip compressed data, was "onprem-0.1.1.tar", last modified: Mon Jun  3 13:34:01 2024, max compression
```

## Comparing `onprem-0.1.0.tar` & `onprem-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 amaiya    (1001) amaiya    (1001)        0 2024-05-29 16:25:41.790322 onprem-0.1.0/
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)     1457 2024-04-04 02:53:11.000000 onprem-0.1.0/CONTRIBUTING.md
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)    11344 2023-09-01 22:09:40.000000 onprem-0.1.0/LICENSE
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)      111 2023-08-31 21:00:21.000000 onprem-0.1.0/MANIFEST.in
--rw-r--r--   0 amaiya    (1001) amaiya    (1001)    32423 2024-05-29 16:25:41.790322 onprem-0.1.0/PKG-INFO
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)    31081 2024-05-29 15:35:32.000000 onprem-0.1.0/README.md
-drwxrwxr-x   0 amaiya    (1001) amaiya    (1001)        0 2024-05-29 16:25:41.774322 onprem-0.1.0/onprem/
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)      837 2024-05-29 16:17:57.000000 onprem-0.1.0/onprem/__init__.py
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)    11387 2024-05-29 16:17:57.000000 onprem-0.1.0/onprem/_modidx.py
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)     1370 2024-04-04 02:53:12.000000 onprem-0.1.0/onprem/console.py
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)    20212 2024-05-29 16:17:57.000000 onprem-0.1.0/onprem/core.py
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)     1582 2024-05-29 16:17:57.000000 onprem-0.1.0/onprem/guider.py
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)    12574 2024-05-29 16:17:57.000000 onprem-0.1.0/onprem/ingest.py
-drwxrwxr-x   0 amaiya    (1001) amaiya    (1001)        0 2024-05-29 16:25:41.790322 onprem-0.1.0/onprem/pipelines/
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)      158 2024-05-29 16:17:57.000000 onprem-0.1.0/onprem/pipelines/__init__.py
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)     8613 2024-05-29 16:17:57.000000 onprem-0.1.0/onprem/pipelines/classifier.py
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)     4261 2024-05-29 16:17:57.000000 onprem-0.1.0/onprem/pipelines/extractor.py
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)    10323 2024-05-29 16:17:57.000000 onprem-0.1.0/onprem/pipelines/summarizer.py
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)     2139 2024-05-29 16:17:57.000000 onprem-0.1.0/onprem/utils.py
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)    10946 2024-04-04 02:53:12.000000 onprem-0.1.0/onprem/webapp.py
-drwxrwxr-x   0 amaiya    (1001) amaiya    (1001)        0 2024-05-29 16:25:41.786322 onprem-0.1.0/onprem.egg-info/
--rw-r--r--   0 amaiya    (1001) amaiya    (1001)    32423 2024-05-29 16:25:41.000000 onprem-0.1.0/onprem.egg-info/PKG-INFO
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)      536 2024-05-29 16:25:41.000000 onprem-0.1.0/onprem.egg-info/SOURCES.txt
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)        1 2024-05-29 16:25:41.000000 onprem-0.1.0/onprem.egg-info/dependency_links.txt
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)       81 2024-05-29 16:25:41.000000 onprem-0.1.0/onprem.egg-info/entry_points.txt
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)        1 2023-08-31 21:02:33.000000 onprem-0.1.0/onprem.egg-info/not-zip-safe
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)      269 2024-05-29 16:25:41.000000 onprem-0.1.0/onprem.egg-info/requires.txt
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)        7 2024-05-29 16:25:41.000000 onprem-0.1.0/onprem.egg-info/top_level.txt
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)     1478 2024-05-29 16:00:40.000000 onprem-0.1.0/settings.ini
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)       38 2024-05-29 16:25:41.790322 onprem-0.1.0/setup.cfg
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)     2596 2023-08-31 21:00:21.000000 onprem-0.1.0/setup.py
+drwxrwxr-x   0 amaiya    (1001) amaiya    (1001)        0 2024-06-03 13:34:01.873808 onprem-0.1.1/
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)     1457 2024-04-04 02:53:11.000000 onprem-0.1.1/CONTRIBUTING.md
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)    11344 2023-09-01 22:09:40.000000 onprem-0.1.1/LICENSE
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)      111 2023-08-31 21:00:21.000000 onprem-0.1.1/MANIFEST.in
+-rw-r--r--   0 amaiya    (1001) amaiya    (1001)    32423 2024-06-03 13:34:01.873808 onprem-0.1.1/PKG-INFO
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)    31081 2024-05-29 15:35:32.000000 onprem-0.1.1/README.md
+drwxrwxr-x   0 amaiya    (1001) amaiya    (1001)        0 2024-06-03 13:34:01.869808 onprem-0.1.1/onprem/
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)      837 2024-06-03 12:27:18.000000 onprem-0.1.1/onprem/__init__.py
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)    11387 2024-06-03 12:27:18.000000 onprem-0.1.1/onprem/_modidx.py
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)     1370 2024-04-04 02:53:12.000000 onprem-0.1.1/onprem/console.py
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)    20209 2024-06-03 12:27:18.000000 onprem-0.1.1/onprem/core.py
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)     1582 2024-06-03 12:27:18.000000 onprem-0.1.1/onprem/guider.py
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)    12549 2024-06-03 12:27:18.000000 onprem-0.1.1/onprem/ingest.py
+drwxrwxr-x   0 amaiya    (1001) amaiya    (1001)        0 2024-06-03 13:34:01.873808 onprem-0.1.1/onprem/pipelines/
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)      158 2024-06-03 12:27:18.000000 onprem-0.1.1/onprem/pipelines/__init__.py
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)     8613 2024-06-03 12:27:18.000000 onprem-0.1.1/onprem/pipelines/classifier.py
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)     4577 2024-06-03 12:27:18.000000 onprem-0.1.1/onprem/pipelines/extractor.py
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)    10323 2024-06-03 12:27:18.000000 onprem-0.1.1/onprem/pipelines/summarizer.py
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)     2139 2024-06-03 12:27:18.000000 onprem-0.1.1/onprem/utils.py
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)    10946 2024-04-04 02:53:12.000000 onprem-0.1.1/onprem/webapp.py
+drwxrwxr-x   0 amaiya    (1001) amaiya    (1001)        0 2024-06-03 13:34:01.873808 onprem-0.1.1/onprem.egg-info/
+-rw-r--r--   0 amaiya    (1001) amaiya    (1001)    32423 2024-06-03 13:34:01.000000 onprem-0.1.1/onprem.egg-info/PKG-INFO
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)      536 2024-06-03 13:34:01.000000 onprem-0.1.1/onprem.egg-info/SOURCES.txt
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)        1 2024-06-03 13:34:01.000000 onprem-0.1.1/onprem.egg-info/dependency_links.txt
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)       81 2024-06-03 13:34:01.000000 onprem-0.1.1/onprem.egg-info/entry_points.txt
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)        1 2023-08-31 21:02:33.000000 onprem-0.1.1/onprem.egg-info/not-zip-safe
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)      269 2024-06-03 13:34:01.000000 onprem-0.1.1/onprem.egg-info/requires.txt
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)        7 2024-06-03 13:34:01.000000 onprem-0.1.1/onprem.egg-info/top_level.txt
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)     1478 2024-06-03 12:27:15.000000 onprem-0.1.1/settings.ini
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)       38 2024-06-03 13:34:01.873808 onprem-0.1.1/setup.cfg
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)     2596 2023-08-31 21:00:21.000000 onprem-0.1.1/setup.py
```

### Comparing `onprem-0.1.0/CONTRIBUTING.md` & `onprem-0.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `onprem-0.1.0/LICENSE` & `onprem-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `onprem-0.1.0/PKG-INFO` & `onprem-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onprem
-Version: 0.1.0
+Version: 0.1.1
 Summary: A tool for running on-premises large language models on non-public data
 Home-page: https://github.com/amaiya/onprem
 Author: Arun S. Maiya
 Author-email: arun@maiya.net
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `onprem-0.1.0/README.md` & `onprem-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `onprem-0.1.0/onprem/__init__.py` & `onprem-0.1.1/onprem/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 # reference: https://stackoverflow.com/questions/74918614/error-importing-seaborn-module-attributeerror/76760670#76760670
 import numpy as np
 def dummy_npwarn_decorator_factory():
   def npwarn_decorator(x):
     return x
   return npwarn_decorator
```

### Comparing `onprem-0.1.0/onprem/_modidx.py` & `onprem-0.1.1/onprem/_modidx.py`

 * *Files identical despite different names*

### Comparing `onprem-0.1.0/onprem/console.py` & `onprem-0.1.1/onprem/console.py`

 * *Files identical despite different names*

### Comparing `onprem-0.1.0/onprem/core.py` & `onprem-0.1.1/onprem/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         )
 
 # %% ../nbs/00_core.ipynb 5
 from . import utils as U
 
 MIN_MODEL_SIZE = 250000000
 DEFAULT_MODEL_URL = "https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF/resolve/main/mistral-7b-instruct-v0.2.Q4_K_M.gguf"
-DEFAULT_MODEL_PROMPT_TEMPLATE = "<s>[INST] {prompt} [/INST]"
+DEFAULT_MODEL_PROMPT_TEMPLATE = "[INST] {prompt} [/INST]"
 DEFAULT_LARGER_URL = "https://huggingface.co/TheBloke/WizardLM-13B-V1.2-GGUF/resolve/main/wizardlm-13b-v1.2.Q4_K_M.gguf"
 DEFAULT_EMBEDDING_MODEL = "sentence-transformers/all-MiniLM-L6-v2"
 DEFAULT_QA_PROMPT = """"Use the following pieces of context delimited by three backticks to answer the question at the end. If you don't know the answer, just say that you don't know, don't try to make up an answer.
 
 ```{context}```
 
 Question: {question}
```

### Comparing `onprem-0.1.0/onprem/guider.py` & `onprem-0.1.1/onprem/guider.py`

 * *Files identical despite different names*

### Comparing `onprem-0.1.0/onprem/ingest.py` & `onprem-0.1.1/onprem/ingest.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,13 +332,12 @@
                             client=self.chroma_client,
                             collection_metadata={"hnsw:space": "cosine"},
                             collection_name=COLLECTION_NAME,
                         )
                     else:
                         db.add_documents(lst)
         if texts:
-            db.persist()
             print(
                 f"Ingestion complete! You can now query your documents using the LLM.ask or LLM.chat methods"
             )
         db = None
         return
```

### Comparing `onprem-0.1.0/onprem/pipelines/classifier.py` & `onprem-0.1.1/onprem/pipelines/classifier.py`

 * *Files identical despite different names*

### Comparing `onprem-0.1.0/onprem/pipelines/extractor.py` & `onprem-0.1.1/onprem/pipelines/extractor.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 
     def apply(self,
               ex_prompt_template:str, 
               fpath: Optional[str] = None,
               content: Optional[str] = None,
               unit:str='paragraph',
               filter_fn: Optional[Callable] = None,
+              clean_fn: Optional[Callable] = None,
               pdf_pages:List[int]=[],
               maxchars = 2048,
               stop:list=[]
              ):
         """
         Apply the prompt to each `unit` (where a "unit" is either a paragraph or sentence) optionally filtered by `filter_fn`.
         Results are stored in a `pandas.Dataframe`.
@@ -55,14 +56,16 @@
         - *ex_prompt_template*: A prompt to apply to each `unit` in document. Should have a single variable, `{text}`.
                                Example: `"Extract universities from the following text delimited by ###:\n\n###{text}###"`
         - *fpath*: A path to to a single file of interest (e.g., a PDF or MS Word document). Mutually-exclusive with `content`.
         - *content*: Text content of a document of interest.  Mutually-exclusive with `fpath`.
         - *unit*: One of {'sentence', 'paragraph'}. 
         - *filter_fn*: A function that accepts a sentence or paragraph and returns `True` if prompt should be applied to it.
                        If `filter_fn` returns False, the text is ignored and excluded from results.
+        - *clean_fn*: A function that accepts a sentence or paragraph and returns "cleaned" version of the text.
+                      If `filter_fn` exists, only applied to texts for which `filter_fn` returns True.
         - *pdf_pages*: If `fpath` is a PDF document, only apply prompt to text on page numbers listed in `pdf_pages`.
                        Page numbers start with 1, not 0 (e.g., `pdf_pages=[1,2,3]` for first three pages).
                        If list is empty, prompt is applied to every page.
         - *maxchars*: units (i.e., paragraphs or sentences) larger than `maxhcars` split.
         - *stop*: list of characters to trigger the LLM to stop generating.
 
 
@@ -90,14 +93,15 @@
         
         # segment
         chunks = segment(content)
         extractions = []
         texts = []
         for chunk in chunks:
             if filter_fn and not filter_fn(chunk): continue
+            if clean_fn: chunk = clean_fn(chunk)
             prompt = extraction_prompt.format(text=chunk)
             extractions.append(self.llm.prompt(prompt, stop=stop))
             texts.append(chunk)
         df = pd.DataFrame({'Extractions':extractions, 'Texts':texts})
         return df
             
         return results
```

### Comparing `onprem-0.1.0/onprem/pipelines/summarizer.py` & `onprem-0.1.1/onprem/pipelines/summarizer.py`

 * *Files identical despite different names*

### Comparing `onprem-0.1.0/onprem/utils.py` & `onprem-0.1.1/onprem/utils.py`

 * *Files identical despite different names*

### Comparing `onprem-0.1.0/onprem/webapp.py` & `onprem-0.1.1/onprem/webapp.py`

 * *Files identical despite different names*

### Comparing `onprem-0.1.0/onprem.egg-info/PKG-INFO` & `onprem-0.1.1/onprem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onprem
-Version: 0.1.0
+Version: 0.1.1
 Summary: A tool for running on-premises large language models on non-public data
 Home-page: https://github.com/amaiya/onprem
 Author: Arun S. Maiya
 Author-email: arun@maiya.net
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `onprem-0.1.0/onprem.egg-info/SOURCES.txt` & `onprem-0.1.1/onprem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onprem-0.1.0/settings.ini` & `onprem-0.1.1/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = onprem
 lib_name = %(repo)s
-version = 0.1.0
+version = 0.1.1
 min_python = 3.8
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = onprem
```

### Comparing `onprem-0.1.0/setup.py` & `onprem-0.1.1/setup.py`

 * *Files identical despite different names*

