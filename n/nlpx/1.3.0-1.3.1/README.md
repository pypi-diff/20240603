# Comparing `tmp/nlpx-1.3.0.tar.gz` & `tmp/nlpx-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpx-1.3.0.tar", last modified: Mon Jun  3 06:01:21 2024, max compression
+gzip compressed data, was "nlpx-1.3.1.tar", last modified: Mon Jun  3 07:15:33 2024, max compression
```

## Comparing `nlpx-1.3.0.tar` & `nlpx-1.3.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 06:01:21.243386 nlpx-1.3.0/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-06-03 06:01:21.241851 nlpx-1.3.0/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.3.0/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 06:01:21.212703 nlpx-1.3.0/nlpx/
--rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.3.0/nlpx/__init__.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 06:01:21.224843 nlpx-1.3.0/nlpx/llm/
--rw-r--r--   0 summy      (501) staff       (20)      189 2024-05-29 11:11:04.000000 nlpx-1.3.0/nlpx/llm/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     5604 2024-05-29 00:43:58.000000 nlpx-1.3.0/nlpx/llm/_model_wrapper.py
--rw-r--r--   0 summy      (501) staff       (20)    10271 2024-05-29 11:20:44.000000 nlpx-1.3.0/nlpx/llm/_tokenize_vec.py
--rw-r--r--   0 summy      (501) staff       (20)     2383 2024-05-29 06:21:14.000000 nlpx-1.3.0/nlpx/llm/_utils.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 06:01:21.231025 nlpx-1.3.0/nlpx/models/
--rw-r--r--   0 summy      (501) staff       (20)      134 2024-06-03 05:46:26.000000 nlpx-1.3.0/nlpx/models/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     2486 2024-06-03 06:00:16.000000 nlpx-1.3.0/nlpx/models/_attention.py
--rw-r--r--   0 summy      (501) staff       (20)     4220 2024-06-03 03:04:45.000000 nlpx-1.3.0/nlpx/models/_text_cnn.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 06:01:21.237554 nlpx-1.3.0/nlpx/text_token/
--rw-r--r--   0 summy      (501) staff       (20)      316 2024-05-26 05:47:41.000000 nlpx-1.3.0/nlpx/text_token/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)    25744 2024-06-03 01:38:28.000000 nlpx-1.3.0/nlpx/text_token/_tokenizer.py
--rw-r--r--   0 summy      (501) staff       (20)    16628 2024-05-26 05:47:41.000000 nlpx-1.3.0/nlpx/text_token/_utils.py
--rw-r--r--   0 summy      (501) staff       (20)     4127 2024-05-29 06:49:09.000000 nlpx-1.3.0/nlpx/training.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 06:01:21.217419 nlpx-1.3.0/nlpx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-06-03 06:01:21.000000 nlpx-1.3.0/nlpx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      444 2024-06-03 06:01:21.000000 nlpx-1.3.0/nlpx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-06-03 06:01:21.000000 nlpx-1.3.0/nlpx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-29 11:20:51.000000 nlpx-1.3.0/nlpx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)        5 2024-06-03 06:01:21.000000 nlpx-1.3.0/nlpx.egg-info/top_level.txt
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-06-03 06:01:21.243745 nlpx-1.3.0/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1044 2024-06-03 06:01:12.000000 nlpx-1.3.0/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 07:15:33.230511 nlpx-1.3.1/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-06-03 07:15:33.229731 nlpx-1.3.1/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.3.1/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 07:15:33.194422 nlpx-1.3.1/nlpx/
+-rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.3.1/nlpx/__init__.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 07:15:33.210767 nlpx-1.3.1/nlpx/llm/
+-rw-r--r--   0 summy      (501) staff       (20)      189 2024-05-29 11:11:04.000000 nlpx-1.3.1/nlpx/llm/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     5604 2024-05-29 00:43:58.000000 nlpx-1.3.1/nlpx/llm/_model_wrapper.py
+-rw-r--r--   0 summy      (501) staff       (20)    10271 2024-05-29 11:20:44.000000 nlpx-1.3.1/nlpx/llm/_tokenize_vec.py
+-rw-r--r--   0 summy      (501) staff       (20)     2383 2024-05-29 06:21:14.000000 nlpx-1.3.1/nlpx/llm/_utils.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 07:15:33.218585 nlpx-1.3.1/nlpx/models/
+-rw-r--r--   0 summy      (501) staff       (20)      134 2024-06-03 05:46:26.000000 nlpx-1.3.1/nlpx/models/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     2492 2024-06-03 06:04:34.000000 nlpx-1.3.1/nlpx/models/_attention.py
+-rw-r--r--   0 summy      (501) staff       (20)     4220 2024-06-03 03:04:45.000000 nlpx-1.3.1/nlpx/models/_text_cnn.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 07:15:33.227180 nlpx-1.3.1/nlpx/text_token/
+-rw-r--r--   0 summy      (501) staff       (20)      316 2024-05-26 05:47:41.000000 nlpx-1.3.1/nlpx/text_token/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)    25747 2024-06-03 07:14:48.000000 nlpx-1.3.1/nlpx/text_token/_tokenizer.py
+-rw-r--r--   0 summy      (501) staff       (20)    16628 2024-05-26 05:47:41.000000 nlpx-1.3.1/nlpx/text_token/_utils.py
+-rw-r--r--   0 summy      (501) staff       (20)     4127 2024-05-29 06:49:09.000000 nlpx-1.3.1/nlpx/training.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 07:15:33.201910 nlpx-1.3.1/nlpx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-06-03 07:15:33.000000 nlpx-1.3.1/nlpx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      444 2024-06-03 07:15:33.000000 nlpx-1.3.1/nlpx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-06-03 07:15:33.000000 nlpx-1.3.1/nlpx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-06-03 07:15:33.000000 nlpx-1.3.1/nlpx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)        5 2024-06-03 07:15:33.000000 nlpx-1.3.1/nlpx.egg-info/top_level.txt
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-06-03 07:15:33.230786 nlpx-1.3.1/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1044 2024-06-03 07:15:27.000000 nlpx-1.3.1/setup.py
```

### Comparing `nlpx-1.3.0/PKG-INFO` & `nlpx-1.3.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.3.0
+Version: 1.3.1
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.3.0/nlpx/llm/_model_wrapper.py` & `nlpx-1.3.1/nlpx/llm/_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.3.0/nlpx/llm/_tokenize_vec.py` & `nlpx-1.3.1/nlpx/llm/_tokenize_vec.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.3.0/nlpx/llm/_utils.py` & `nlpx-1.3.1/nlpx/llm/_utils.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.3.0/nlpx/models/_attention.py` & `nlpx-1.3.1/nlpx/models/_attention.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 		"""
 		:param embed_dim: RNN的input_size，word embedding维度
 		:param hidden_size: RNN的hidden_size, RNN隐藏层维度
 		:param num_layers: RNN的num_layers, RNN层数
 		:param num_layers: RNN的num_layers, RNN层数
 		:param num_heads: 抽头数
 		:param rnn: 所用的RNN模型：GRU和LSTM，默认是GRU
-		:drop_out：
+		:param drop_out：
 		"""
 
 		super().__init__()
 		self.rnn = rnn(input_size=embed_dim, hidden_size=hidden_size, num_layers=num_layers, bidirectional=True,
 					   batch_first=True)
 		self.attention = MultiHeadClassifySelfAttention(hidden_size * 2, num_heads)
```

### Comparing `nlpx-1.3.0/nlpx/models/_text_cnn.py` & `nlpx-1.3.1/nlpx/models/_text_cnn.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.3.0/nlpx/text_token/_tokenizer.py` & `nlpx-1.3.1/nlpx/text_token/_tokenizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -357,15 +357,15 @@
         self.embed_dim = len(embedding[0])
         for token in reserved_token:
             embedding = [[self.do_encode(token)] * self.embed_dim] + embedding
         self.embedding = Embedding.from_pretrained(torch.tensor(embedding, dtype=torch.float))
 
     def __call__(self, sentence: Union[str, Iterable[str], Iterable[Iterable]], max_length: int = None):
         input_ids = self.batch_encode(sentence, max_length)
-        return self.encode(torch.tensor(input_ids, dtype=torch.long))
+        return self.embedding(torch.tensor(input_ids, dtype=torch.long))
 
     @classmethod
     def from_file(cls, file: str, func=load_embedding, is_large_file=False, reserved_token=[], language='cn', cut_type='word'):
         """
         :param file: embedding文件， 如：'./sgns.weibo.word.bz2'. 注意：必须是单一文件，不能是文件夹。
         :param func: 具体读取文件的处理函数，load_embedding，可替换。注意：其函数签名为 function_name(path: str, is_large_file: bool) -> [vocab], [[embedding]]
         :param is_large_file: 是否是大文件
```

### Comparing `nlpx-1.3.0/nlpx/text_token/_utils.py` & `nlpx-1.3.1/nlpx/text_token/_utils.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.3.0/nlpx/training.py` & `nlpx-1.3.1/nlpx/training.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.3.0/nlpx.egg-info/PKG-INFO` & `nlpx-1.3.1/nlpx.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.3.0
+Version: 1.3.1
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.3.0/setup.py` & `nlpx-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 setup(
     name='nlpx',
     packages=['nlpx', 'nlpx.models', 'nlpx.llm', 'nlpx.text_token'],
     description="A tool set for NLP.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.3.0',
+    version='1.3.1',
     url='https://gitee.com/summry/nlpx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['NLP'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

