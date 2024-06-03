# Comparing `tmp/nlpx-1.3.1.tar.gz` & `tmp/nlpx-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpx-1.3.1.tar", last modified: Mon Jun  3 07:15:33 2024, max compression
+gzip compressed data, was "nlpx-1.3.2.tar", last modified: Mon Jun  3 07:31:13 2024, max compression
```

## Comparing `nlpx-1.3.1.tar` & `nlpx-1.3.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 07:15:33.230511 nlpx-1.3.1/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-06-03 07:15:33.229731 nlpx-1.3.1/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.3.1/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 07:15:33.194422 nlpx-1.3.1/nlpx/
--rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.3.1/nlpx/__init__.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 07:15:33.210767 nlpx-1.3.1/nlpx/llm/
--rw-r--r--   0 summy      (501) staff       (20)      189 2024-05-29 11:11:04.000000 nlpx-1.3.1/nlpx/llm/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     5604 2024-05-29 00:43:58.000000 nlpx-1.3.1/nlpx/llm/_model_wrapper.py
--rw-r--r--   0 summy      (501) staff       (20)    10271 2024-05-29 11:20:44.000000 nlpx-1.3.1/nlpx/llm/_tokenize_vec.py
--rw-r--r--   0 summy      (501) staff       (20)     2383 2024-05-29 06:21:14.000000 nlpx-1.3.1/nlpx/llm/_utils.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 07:15:33.218585 nlpx-1.3.1/nlpx/models/
--rw-r--r--   0 summy      (501) staff       (20)      134 2024-06-03 05:46:26.000000 nlpx-1.3.1/nlpx/models/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     2492 2024-06-03 06:04:34.000000 nlpx-1.3.1/nlpx/models/_attention.py
--rw-r--r--   0 summy      (501) staff       (20)     4220 2024-06-03 03:04:45.000000 nlpx-1.3.1/nlpx/models/_text_cnn.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 07:15:33.227180 nlpx-1.3.1/nlpx/text_token/
--rw-r--r--   0 summy      (501) staff       (20)      316 2024-05-26 05:47:41.000000 nlpx-1.3.1/nlpx/text_token/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)    25747 2024-06-03 07:14:48.000000 nlpx-1.3.1/nlpx/text_token/_tokenizer.py
--rw-r--r--   0 summy      (501) staff       (20)    16628 2024-05-26 05:47:41.000000 nlpx-1.3.1/nlpx/text_token/_utils.py
--rw-r--r--   0 summy      (501) staff       (20)     4127 2024-05-29 06:49:09.000000 nlpx-1.3.1/nlpx/training.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 07:15:33.201910 nlpx-1.3.1/nlpx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-06-03 07:15:33.000000 nlpx-1.3.1/nlpx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      444 2024-06-03 07:15:33.000000 nlpx-1.3.1/nlpx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-06-03 07:15:33.000000 nlpx-1.3.1/nlpx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-06-03 07:15:33.000000 nlpx-1.3.1/nlpx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)        5 2024-06-03 07:15:33.000000 nlpx-1.3.1/nlpx.egg-info/top_level.txt
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-06-03 07:15:33.230786 nlpx-1.3.1/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1044 2024-06-03 07:15:27.000000 nlpx-1.3.1/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 07:31:13.528470 nlpx-1.3.2/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-06-03 07:31:13.527641 nlpx-1.3.2/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.3.2/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 07:31:13.495669 nlpx-1.3.2/nlpx/
+-rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.3.2/nlpx/__init__.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 07:31:13.506792 nlpx-1.3.2/nlpx/llm/
+-rw-r--r--   0 summy      (501) staff       (20)      189 2024-05-29 11:11:04.000000 nlpx-1.3.2/nlpx/llm/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     5876 2024-06-03 07:31:09.000000 nlpx-1.3.2/nlpx/llm/_model_wrapper.py
+-rw-r--r--   0 summy      (501) staff       (20)    10271 2024-05-29 11:20:44.000000 nlpx-1.3.2/nlpx/llm/_tokenize_vec.py
+-rw-r--r--   0 summy      (501) staff       (20)     2383 2024-05-29 06:21:14.000000 nlpx-1.3.2/nlpx/llm/_utils.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 07:31:13.517526 nlpx-1.3.2/nlpx/models/
+-rw-r--r--   0 summy      (501) staff       (20)      134 2024-06-03 05:46:26.000000 nlpx-1.3.2/nlpx/models/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     2492 2024-06-03 06:04:34.000000 nlpx-1.3.2/nlpx/models/_attention.py
+-rw-r--r--   0 summy      (501) staff       (20)     4220 2024-06-03 03:04:45.000000 nlpx-1.3.2/nlpx/models/_text_cnn.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 07:31:13.525066 nlpx-1.3.2/nlpx/text_token/
+-rw-r--r--   0 summy      (501) staff       (20)      316 2024-05-26 05:47:41.000000 nlpx-1.3.2/nlpx/text_token/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)    25747 2024-06-03 07:14:48.000000 nlpx-1.3.2/nlpx/text_token/_tokenizer.py
+-rw-r--r--   0 summy      (501) staff       (20)    16628 2024-05-26 05:47:41.000000 nlpx-1.3.2/nlpx/text_token/_utils.py
+-rw-r--r--   0 summy      (501) staff       (20)     4127 2024-05-29 06:49:09.000000 nlpx-1.3.2/nlpx/training.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 07:31:13.502046 nlpx-1.3.2/nlpx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-06-03 07:31:13.000000 nlpx-1.3.2/nlpx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      444 2024-06-03 07:31:13.000000 nlpx-1.3.2/nlpx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-06-03 07:31:13.000000 nlpx-1.3.2/nlpx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-06-03 07:31:13.000000 nlpx-1.3.2/nlpx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)        5 2024-06-03 07:31:13.000000 nlpx-1.3.2/nlpx.egg-info/top_level.txt
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-06-03 07:31:13.528994 nlpx-1.3.2/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1044 2024-06-03 07:31:09.000000 nlpx-1.3.2/setup.py
```

### Comparing `nlpx-1.3.1/PKG-INFO` & `nlpx-1.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.3.1
+Version: 1.3.2
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.3.1/nlpx/llm/_model_wrapper.py` & `nlpx-1.3.2/nlpx/llm/_model_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from torch import optim
 from pathlib import Path
 from typing import Union, List
 from torch.nn import functional as F
 from torch.utils.data import DataLoader, TensorDataset, Dataset
 
 from nlpx.training import Trainer, SimpleTrainer, evaluate
+from nlpx.text_token import TokenEmbedding
 from ._tokenize_vec import TokenizeVec
 
 
 class ModelWrapper:
 
 	def __init__(self, model_path: Union[str, Path] = None, classes: List[str] = None,
 					device=torch.device('cuda:0' if torch.cuda.is_available() else 'cpu')):
@@ -67,15 +68,15 @@
 
 	def load(self, model_path: Union[str, Path] = './best_model.pt'):
 		self.model = torch.load(model_path, map_location=self.device)
 
 
 class SimpleModelWrapper(ModelWrapper):
 
-	def __init__(self, tokenize_vec: TokenizeVec, model_path: Union[str, Path] = None, classes: List[str] = None,
+	def __init__(self, tokenize_vec, model_path: Union[str, Path] = None, classes: List[str] = None,
 				device=torch.device('cuda:0' if torch.cuda.is_available() else 'cpu')):
 		super().__init__(model_path, classes, device)
 		self.tokenize_vec = tokenize_vec
 
 	def train(self, model, texts: List[str], y: Union[torch.LongTensor, List, np.ndarray], max_length: int = 0,
 			  eval_size=0.2, random_state=None, collate_fn=None,max_iter=100,
 			  optimizer=optim.AdamW, learning_rate=0.001, T_max: int = 0,
@@ -121,12 +122,16 @@
 		X = self.get_vec(texts, max_length, n_jobs=n_jobs)
 		if isinstance(y, List) or isinstance(y, np.ndarray):
 			y = torch.tensor(y, dtype=torch.long)
 		eval_set = TensorDataset(X, y)
 		return super().evaluate(eval_set, batch_size=batch_size, num_workers=num_workers, collate_fn=collate_fn)
 
 	def get_vec(self, texts: List[str], max_length: int, n_jobs: int):
-		return self.tokenize_vec.parallel_encode_plus(texts, max_length=max_length, padding='max_length',
-														truncation=True, add_special_tokens=True,
-														return_token_type_ids=True,return_attention_mask=True,
-														return_tensors='pt', n_jobs=n_jobs)
+		if isinstance(self.tokenize_vec, TokenizeVec):
+			return self.tokenize_vec.parallel_encode_plus(texts, max_length=max_length, padding='max_length',
+															truncation=True, add_special_tokens=True,
+															return_token_type_ids=True,return_attention_mask=True,
+															return_tensors='pt', n_jobs=n_jobs)
+		elif isinstance(self.tokenize_vec, TokenEmbedding):
+			return self.tokenize_vec(texts, max_length)
 
+		raise ValueError("Invalid tokenize_vec, it must be a TokenEmbedding or TokenizeVec".)
```

### Comparing `nlpx-1.3.1/nlpx/llm/_tokenize_vec.py` & `nlpx-1.3.2/nlpx/llm/_tokenize_vec.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.3.1/nlpx/llm/_utils.py` & `nlpx-1.3.2/nlpx/llm/_utils.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.3.1/nlpx/models/_attention.py` & `nlpx-1.3.2/nlpx/models/_attention.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.3.1/nlpx/models/_text_cnn.py` & `nlpx-1.3.2/nlpx/models/_text_cnn.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.3.1/nlpx/text_token/_tokenizer.py` & `nlpx-1.3.2/nlpx/text_token/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.3.1/nlpx/text_token/_utils.py` & `nlpx-1.3.2/nlpx/text_token/_utils.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.3.1/nlpx/training.py` & `nlpx-1.3.2/nlpx/training.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.3.1/nlpx.egg-info/PKG-INFO` & `nlpx-1.3.2/nlpx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.3.1
+Version: 1.3.2
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.3.1/setup.py` & `nlpx-1.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 setup(
     name='nlpx',
     packages=['nlpx', 'nlpx.models', 'nlpx.llm', 'nlpx.text_token'],
     description="A tool set for NLP.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.3.1',
+    version='1.3.2',
     url='https://gitee.com/summry/nlpx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['NLP'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

