# Comparing `tmp/nlpx-1.2.9.tar.gz` & `tmp/nlpx-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpx-1.2.9.tar", last modified: Wed May 29 11:20:51 2024, max compression
+gzip compressed data, was "nlpx-1.3.0.tar", last modified: Mon Jun  3 06:01:21 2024, max compression
```

## Comparing `nlpx-1.2.9.tar` & `nlpx-1.3.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-29 11:20:51.951256 nlpx-1.2.9/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-29 11:20:51.950554 nlpx-1.2.9/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.2.9/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-29 11:20:51.923580 nlpx-1.2.9/nlpx/
--rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.2.9/nlpx/__init__.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-29 11:20:51.938811 nlpx-1.2.9/nlpx/llm/
--rw-r--r--   0 summy      (501) staff       (20)      189 2024-05-29 11:11:04.000000 nlpx-1.2.9/nlpx/llm/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     5604 2024-05-29 00:43:58.000000 nlpx-1.2.9/nlpx/llm/_model_wrapper.py
--rw-r--r--   0 summy      (501) staff       (20)    10271 2024-05-29 11:20:44.000000 nlpx-1.2.9/nlpx/llm/_tokenize_vec.py
--rw-r--r--   0 summy      (501) staff       (20)     2383 2024-05-29 06:21:14.000000 nlpx-1.2.9/nlpx/llm/_utils.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-29 11:20:51.942583 nlpx-1.2.9/nlpx/models/
--rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-24 23:09:44.000000 nlpx-1.2.9/nlpx/models/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     3848 2024-05-28 13:54:23.000000 nlpx-1.2.9/nlpx/models/_text_cnn.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-29 11:20:51.948530 nlpx-1.2.9/nlpx/text_token/
--rw-r--r--   0 summy      (501) staff       (20)      316 2024-05-26 05:47:41.000000 nlpx-1.2.9/nlpx/text_token/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)    25732 2024-05-26 06:13:27.000000 nlpx-1.2.9/nlpx/text_token/_tokenizer.py
--rw-r--r--   0 summy      (501) staff       (20)    16628 2024-05-26 05:47:41.000000 nlpx-1.2.9/nlpx/text_token/_utils.py
--rw-r--r--   0 summy      (501) staff       (20)     4127 2024-05-29 06:49:09.000000 nlpx-1.2.9/nlpx/training.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-29 11:20:51.929315 nlpx-1.2.9/nlpx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-29 11:20:51.000000 nlpx-1.2.9/nlpx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      418 2024-05-29 11:20:51.000000 nlpx-1.2.9/nlpx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-29 11:20:51.000000 nlpx-1.2.9/nlpx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-29 11:20:51.000000 nlpx-1.2.9/nlpx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-29 11:20:51.000000 nlpx-1.2.9/nlpx.egg-info/top_level.txt
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-29 11:20:51.951487 nlpx-1.2.9/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1044 2024-05-29 11:20:44.000000 nlpx-1.2.9/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 06:01:21.243386 nlpx-1.3.0/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-06-03 06:01:21.241851 nlpx-1.3.0/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.3.0/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 06:01:21.212703 nlpx-1.3.0/nlpx/
+-rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.3.0/nlpx/__init__.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 06:01:21.224843 nlpx-1.3.0/nlpx/llm/
+-rw-r--r--   0 summy      (501) staff       (20)      189 2024-05-29 11:11:04.000000 nlpx-1.3.0/nlpx/llm/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     5604 2024-05-29 00:43:58.000000 nlpx-1.3.0/nlpx/llm/_model_wrapper.py
+-rw-r--r--   0 summy      (501) staff       (20)    10271 2024-05-29 11:20:44.000000 nlpx-1.3.0/nlpx/llm/_tokenize_vec.py
+-rw-r--r--   0 summy      (501) staff       (20)     2383 2024-05-29 06:21:14.000000 nlpx-1.3.0/nlpx/llm/_utils.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 06:01:21.231025 nlpx-1.3.0/nlpx/models/
+-rw-r--r--   0 summy      (501) staff       (20)      134 2024-06-03 05:46:26.000000 nlpx-1.3.0/nlpx/models/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     2486 2024-06-03 06:00:16.000000 nlpx-1.3.0/nlpx/models/_attention.py
+-rw-r--r--   0 summy      (501) staff       (20)     4220 2024-06-03 03:04:45.000000 nlpx-1.3.0/nlpx/models/_text_cnn.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 06:01:21.237554 nlpx-1.3.0/nlpx/text_token/
+-rw-r--r--   0 summy      (501) staff       (20)      316 2024-05-26 05:47:41.000000 nlpx-1.3.0/nlpx/text_token/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)    25744 2024-06-03 01:38:28.000000 nlpx-1.3.0/nlpx/text_token/_tokenizer.py
+-rw-r--r--   0 summy      (501) staff       (20)    16628 2024-05-26 05:47:41.000000 nlpx-1.3.0/nlpx/text_token/_utils.py
+-rw-r--r--   0 summy      (501) staff       (20)     4127 2024-05-29 06:49:09.000000 nlpx-1.3.0/nlpx/training.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-03 06:01:21.217419 nlpx-1.3.0/nlpx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-06-03 06:01:21.000000 nlpx-1.3.0/nlpx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      444 2024-06-03 06:01:21.000000 nlpx-1.3.0/nlpx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-06-03 06:01:21.000000 nlpx-1.3.0/nlpx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-29 11:20:51.000000 nlpx-1.3.0/nlpx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)        5 2024-06-03 06:01:21.000000 nlpx-1.3.0/nlpx.egg-info/top_level.txt
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-06-03 06:01:21.243745 nlpx-1.3.0/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1044 2024-06-03 06:01:12.000000 nlpx-1.3.0/setup.py
```

### Comparing `nlpx-1.2.9/PKG-INFO` & `nlpx-1.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.2.9
+Version: 1.3.0
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.2.9/nlpx/llm/_model_wrapper.py` & `nlpx-1.3.0/nlpx/llm/_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.9/nlpx/llm/_tokenize_vec.py` & `nlpx-1.3.0/nlpx/llm/_tokenize_vec.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.9/nlpx/llm/_utils.py` & `nlpx-1.3.0/nlpx/llm/_utils.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.9/nlpx/models/_text_cnn.py` & `nlpx-1.3.0/nlpx/models/_text_cnn.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 import torch
 from torch import nn
 from torch.nn import functional as F
 
 
 class TextCNN(nn.Module):
 
-    def __init__(self, word_dim: int, kernel_sizes=(2, 3, 4), cnn_channels: int = 64, out_features: int = 2,
+    def __init__(self, embed_dim: int, kernel_sizes=(2, 3, 4), cnn_channels: int = 64, out_features: int = 2,
                  activation=nn.ReLU(inplace=True), num_hidden_layer: int = 0, batch_norm=False, layer_norm=False,
                  drop_out: float = 0.0):
         """ TextCNN model
         Parameters
         ----------
-        word_dim: int, dim of word, in_channels of cnn
+        embed_dim: int, dim of embedding, in_channels of cnn
         cnn_channels: int, out_channels of cnn
         kernel_sizes: size of each cnn kernel
         out_features: dim of output
         activation:
         num_hidden_layer:
         drop_out:
 
         Examples
         --------
         >>> import torch
         >>> from nlpx.models import TextCNN
         >>> X = torch.randn(batch_size, 10, word_dim)
         >>> targets = torch.randint(0, num_classes, (batch_size,))
-        >>> model = TextCNN(word_dim, cnn_channels=64, kernel_sizes=(2, 3, 4), out_features=num_classes)
+        >>> model = TextCNN(embed_dim, cnn_channels=64, kernel_sizes=(2, 3, 4), out_features=num_classes)
         >>> output = model(X)
         >>> loss, output = model(X, targets)
         """
+
         super().__init__()
         if batch_norm:
             self.convs = nn.ModuleList([
                 nn.Sequential(
-                    nn.Conv1d(in_channels=word_dim, out_channels=cnn_channels, kernel_size=kernel_size, bias=False),
+                    nn.Conv1d(in_channels=embed_dim, out_channels=cnn_channels, kernel_size=kernel_size, bias=False),
                     nn.BatchNorm1d(num_features=cnn_channels),
                     activation,  # inplace为True，将会改变输入的数据 ，否则不会改变原输入，只会产生新的输出
                     nn.AdaptiveMaxPool1d(1)
                 ) for kernel_size in kernel_sizes
             ])
         else:
             self.convs = nn.ModuleList([
                 nn.Sequential(
-                    nn.Conv1d(in_channels=word_dim, out_channels=cnn_channels, kernel_size=kernel_size, bias=False),
+                    nn.Conv1d(in_channels=embed_dim, out_channels=cnn_channels, kernel_size=kernel_size, bias=False),
                     activation,  # inplace为True，将会改变输入的数据 ，否则不会改变原输入，只会产生新的输出
                     nn.AdaptiveMaxPool1d(1)
                 ) for kernel_size in kernel_sizes
             ])
 
         self.num_hidden_layer = num_hidden_layer
         num_features = cnn_channels * len(kernel_sizes)
@@ -72,26 +73,34 @@
             self.fc = nn.Sequential(
                 nn.Dropout(drop_out),
                 self.fc
             )
 
     def forward(self, inputs, labels=None):
         """
-        :param inputs: [(batch, sentence, word_dim)]
+        :param inputs: [(batch_size, sentence_length, embed_dim)]
         :param labels: [long]
         """
+
+        # Conv1d期望输入的形状是：(batch_size, embed_dim, sentence_length)
         input_embeddings = inputs.transpose(2, 1)
-        out = torch.cat([conv(input_embeddings) for conv in self.convs], dim=1)
-        out = out.transpose(2, 1)
+
+        # conv输出的形状是：(batch_size, cnn_channels, 1)
+        # output的形状是：(batch_size, cnn_channels * len(kernel_sizes), 1)
+        output = torch.cat([conv(input_embeddings) for conv in self.convs], dim=1)
+
+        # 确保张量是连续的
+        output = output.contiguous()
+        # output：(batch_size, cnn_channels * len(kernel_sizes))
+        output = output.view(inputs.size(0), -1)
 
         if self.num_hidden_layer and self.num_hidden_layer > 0:
             for hidden_layer in self.hidden_layers:
-                out = hidden_layer(out)
+                output = hidden_layer(output)
 
-        out = self.fc(out)
-        logits = out.squeeze(1)
+        logits = self.fc(output)
 
         if labels is None:
             return logits
-        else:
-            loss = F.cross_entropy(logits, labels)
-            return loss, logits
+
+        loss = F.cross_entropy(logits, labels)
+        return loss, logits
```

### Comparing `nlpx-1.2.9/nlpx/text_token/_tokenizer.py` & `nlpx-1.3.0/nlpx/text_token/_tokenizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -350,17 +350,17 @@
             assert Path(file).is_file(), 'file必须是具体文件,不能是文件夹'
             vocab, embedding = func(file, is_large_file)
         elif not vocab or not embedding:
             raise ValueError('参数"path"为空的情况下，"vocab"和"embedding"不能为空.')
         super().__init__(vocab=vocab, reserved_token=reserved_token, language=language, cut_type=cut_type)
         reserved_token = self.reserved_token.copy()
         reserved_token.reverse()
-        self.dim = len(embedding[0])
+        self.embed_dim = len(embedding[0])
         for token in reserved_token:
-            embedding = [[self.do_encode(token)] * self.dim] + embedding
+            embedding = [[self.do_encode(token)] * self.embed_dim] + embedding
         self.embedding = Embedding.from_pretrained(torch.tensor(embedding, dtype=torch.float))
 
     def __call__(self, sentence: Union[str, Iterable[str], Iterable[Iterable]], max_length: int = None):
         input_ids = self.batch_encode(sentence, max_length)
         return self.encode(torch.tensor(input_ids, dtype=torch.long))
 
     @classmethod
```

### Comparing `nlpx-1.2.9/nlpx/text_token/_utils.py` & `nlpx-1.3.0/nlpx/text_token/_utils.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.9/nlpx/training.py` & `nlpx-1.3.0/nlpx/training.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.9/nlpx.egg-info/PKG-INFO` & `nlpx-1.3.0/nlpx.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.2.9
+Version: 1.3.0
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.2.9/setup.py` & `nlpx-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 setup(
     name='nlpx',
     packages=['nlpx', 'nlpx.models', 'nlpx.llm', 'nlpx.text_token'],
     description="A tool set for NLP.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.2.9',
+    version='1.3.0',
     url='https://gitee.com/summry/nlpx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['NLP'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

