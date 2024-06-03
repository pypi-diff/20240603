# Comparing `tmp/nlpx-1.3.2.tar.gz` & `tmp/nlpx-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpx-1.3.2.tar", last modified: Mon Jun  3 07:31:13 2024, max compression
+gzip compressed data, was "nlpx-1.3.3.tar", last modified: Mon Jun  3 07:36:05 2024, max compression
```

## Comparing `nlpx-1.3.2.tar` & `nlpx-1.3.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 07:31:13.528470 nlpx-1.3.2/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-06-03 07:31:13.527641 nlpx-1.3.2/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.3.2/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 07:31:13.495669 nlpx-1.3.2/nlpx/
--rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.3.2/nlpx/__init__.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 07:31:13.506792 nlpx-1.3.2/nlpx/llm/
--rw-r--r--   0 summy      (501) staff       (20)      189 2024-05-29 11:11:04.000000 nlpx-1.3.2/nlpx/llm/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     5876 2024-06-03 07:31:09.000000 nlpx-1.3.2/nlpx/llm/_model_wrapper.py
--rw-r--r--   0 summy      (501) staff       (20)    10271 2024-05-29 11:20:44.000000 nlpx-1.3.2/nlpx/llm/_tokenize_vec.py
--rw-r--r--   0 summy      (501) staff       (20)     2383 2024-05-29 06:21:14.000000 nlpx-1.3.2/nlpx/llm/_utils.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 07:31:13.517526 nlpx-1.3.2/nlpx/models/
--rw-r--r--   0 summy      (501) staff       (20)      134 2024-06-03 05:46:26.000000 nlpx-1.3.2/nlpx/models/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     2492 2024-06-03 06:04:34.000000 nlpx-1.3.2/nlpx/models/_attention.py
--rw-r--r--   0 summy      (501) staff       (20)     4220 2024-06-03 03:04:45.000000 nlpx-1.3.2/nlpx/models/_text_cnn.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 07:31:13.525066 nlpx-1.3.2/nlpx/text_token/
--rw-r--r--   0 summy      (501) staff       (20)      316 2024-05-26 05:47:41.000000 nlpx-1.3.2/nlpx/text_token/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)    25747 2024-06-03 07:14:48.000000 nlpx-1.3.2/nlpx/text_token/_tokenizer.py
--rw-r--r--   0 summy      (501) staff       (20)    16628 2024-05-26 05:47:41.000000 nlpx-1.3.2/nlpx/text_token/_utils.py
--rw-r--r--   0 summy      (501) staff       (20)     4127 2024-05-29 06:49:09.000000 nlpx-1.3.2/nlpx/training.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 07:31:13.502046 nlpx-1.3.2/nlpx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-06-03 07:31:13.000000 nlpx-1.3.2/nlpx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      444 2024-06-03 07:31:13.000000 nlpx-1.3.2/nlpx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-06-03 07:31:13.000000 nlpx-1.3.2/nlpx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-06-03 07:31:13.000000 nlpx-1.3.2/nlpx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)        5 2024-06-03 07:31:13.000000 nlpx-1.3.2/nlpx.egg-info/top_level.txt
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-06-03 07:31:13.528994 nlpx-1.3.2/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1044 2024-06-03 07:31:09.000000 nlpx-1.3.2/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 07:36:05.359459 nlpx-1.3.3/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-06-03 07:36:05.358759 nlpx-1.3.3/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.3.3/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 07:36:05.326712 nlpx-1.3.3/nlpx/
+-rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.3.3/nlpx/__init__.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 07:36:05.339631 nlpx-1.3.3/nlpx/llm/
+-rw-r--r--   0 summy      (501) staff       (20)      189 2024-05-29 11:11:04.000000 nlpx-1.3.3/nlpx/llm/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     5913 2024-06-03 07:35:31.000000 nlpx-1.3.3/nlpx/llm/_model_wrapper.py
+-rw-r--r--   0 summy      (501) staff       (20)    10271 2024-05-29 11:20:44.000000 nlpx-1.3.3/nlpx/llm/_tokenize_vec.py
+-rw-r--r--   0 summy      (501) staff       (20)     2383 2024-05-29 06:21:14.000000 nlpx-1.3.3/nlpx/llm/_utils.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 07:36:05.345834 nlpx-1.3.3/nlpx/models/
+-rw-r--r--   0 summy      (501) staff       (20)      134 2024-06-03 05:46:26.000000 nlpx-1.3.3/nlpx/models/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     2492 2024-06-03 06:04:34.000000 nlpx-1.3.3/nlpx/models/_attention.py
+-rw-r--r--   0 summy      (501) staff       (20)     4220 2024-06-03 03:04:45.000000 nlpx-1.3.3/nlpx/models/_text_cnn.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 07:36:05.355874 nlpx-1.3.3/nlpx/text_token/
+-rw-r--r--   0 summy      (501) staff       (20)      316 2024-05-26 05:47:41.000000 nlpx-1.3.3/nlpx/text_token/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)    25747 2024-06-03 07:14:48.000000 nlpx-1.3.3/nlpx/text_token/_tokenizer.py
+-rw-r--r--   0 summy      (501) staff       (20)    16628 2024-05-26 05:47:41.000000 nlpx-1.3.3/nlpx/text_token/_utils.py
+-rw-r--r--   0 summy      (501) staff       (20)     4127 2024-05-29 06:49:09.000000 nlpx-1.3.3/nlpx/training.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 07:36:05.332820 nlpx-1.3.3/nlpx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-06-03 07:36:05.000000 nlpx-1.3.3/nlpx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      444 2024-06-03 07:36:05.000000 nlpx-1.3.3/nlpx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-06-03 07:36:05.000000 nlpx-1.3.3/nlpx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-06-03 07:31:13.000000 nlpx-1.3.3/nlpx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)        5 2024-06-03 07:36:05.000000 nlpx-1.3.3/nlpx.egg-info/top_level.txt
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-06-03 07:36:05.359847 nlpx-1.3.3/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1044 2024-06-03 07:36:00.000000 nlpx-1.3.3/setup.py
```

### Comparing `nlpx-1.3.2/PKG-INFO` & `nlpx-1.3.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.3.2
+Version: 1.3.3
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.3.2/nlpx/llm/_model_wrapper.py` & `nlpx-1.3.3/nlpx/llm/_model_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,16 +68,16 @@
 
 	def load(self, model_path: Union[str, Path] = './best_model.pt'):
 		self.model = torch.load(model_path, map_location=self.device)
 
 
 class SimpleModelWrapper(ModelWrapper):
 
-	def __init__(self, tokenize_vec, model_path: Union[str, Path] = None, classes: List[str] = None,
-				device=torch.device('cuda:0' if torch.cuda.is_available() else 'cpu')):
+	def __init__(self, tokenize_vec: Union[TokenizeVec, TokenEmbedding], model_path: Union[str, Path] = None,
+				 classes: List[str] = None, device=torch.device('cuda:0' if torch.cuda.is_available() else 'cpu')):
 		super().__init__(model_path, classes, device)
 		self.tokenize_vec = tokenize_vec
 
 	def train(self, model, texts: List[str], y: Union[torch.LongTensor, List, np.ndarray], max_length: int = 0,
 			  eval_size=0.2, random_state=None, collate_fn=None,max_iter=100,
 			  optimizer=optim.AdamW, learning_rate=0.001, T_max: int = 0,
 			  batch_size=8, eval_batch_size=16,
@@ -130,8 +130,8 @@
 			return self.tokenize_vec.parallel_encode_plus(texts, max_length=max_length, padding='max_length',
 															truncation=True, add_special_tokens=True,
 															return_token_type_ids=True,return_attention_mask=True,
 															return_tensors='pt', n_jobs=n_jobs)
 		elif isinstance(self.tokenize_vec, TokenEmbedding):
 			return self.tokenize_vec(texts, max_length)
 
-		raise ValueError("Invalid tokenize_vec, it must be a TokenEmbedding or TokenizeVec".)
+		raise ValueError("Invalid tokenize_vec, it must be a TokenizeVec or TokenEmbedding.")
```

### Comparing `nlpx-1.3.2/nlpx/llm/_tokenize_vec.py` & `nlpx-1.3.3/nlpx/llm/_tokenize_vec.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.3.2/nlpx/llm/_utils.py` & `nlpx-1.3.3/nlpx/llm/_utils.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.3.2/nlpx/models/_attention.py` & `nlpx-1.3.3/nlpx/models/_attention.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.3.2/nlpx/models/_text_cnn.py` & `nlpx-1.3.3/nlpx/models/_text_cnn.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.3.2/nlpx/text_token/_tokenizer.py` & `nlpx-1.3.3/nlpx/text_token/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.3.2/nlpx/text_token/_utils.py` & `nlpx-1.3.3/nlpx/text_token/_utils.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.3.2/nlpx/training.py` & `nlpx-1.3.3/nlpx/training.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.3.2/nlpx.egg-info/PKG-INFO` & `nlpx-1.3.3/nlpx.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.3.2
+Version: 1.3.3
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.3.2/setup.py` & `nlpx-1.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 setup(
     name='nlpx',
     packages=['nlpx', 'nlpx.models', 'nlpx.llm', 'nlpx.text_token'],
     description="A tool set for NLP.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.3.2',
+    version='1.3.3',
     url='https://gitee.com/summry/nlpx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['NLP'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

