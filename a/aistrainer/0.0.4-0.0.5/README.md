# Comparing `tmp/aistrainer-0.0.4.tar.gz` & `tmp/aistrainer-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aistrainer-0.0.4.tar", last modified: Mon Jun  3 08:35:42 2024, max compression
+gzip compressed data, was "aistrainer-0.0.5.tar", last modified: Mon Jun  3 09:23:31 2024, max compression
```

## Comparing `aistrainer-0.0.4.tar` & `aistrainer-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-06-03 08:35:42.813174 aistrainer-0.0.4/
--rw-r--r--   0 man4j     (1000) man4j     (1000)     1074 2024-05-24 14:22:02.000000 aistrainer-0.0.4/LICENSE
--rw-r--r--   0 man4j     (1000) man4j     (1000)     7270 2024-06-03 08:35:42.813174 aistrainer-0.0.4/PKG-INFO
--rw-r--r--   0 man4j     (1000) man4j     (1000)     6560 2024-06-03 08:35:04.000000 aistrainer-0.0.4/README.md
--rw-r--r--   0 man4j     (1000) man4j     (1000)      741 2024-06-03 08:35:11.000000 aistrainer-0.0.4/pyproject.toml
--rw-r--r--   0 man4j     (1000) man4j     (1000)       38 2024-06-03 08:35:42.813174 aistrainer-0.0.4/setup.cfg
-drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-06-03 08:35:42.813174 aistrainer-0.0.4/src/
-drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-06-03 08:35:42.813174 aistrainer-0.0.4/src/aistrainer/
--rw-r--r--   0 man4j     (1000) man4j     (1000)    10328 2024-05-28 11:25:03.000000 aistrainer-0.0.4/src/aistrainer/aistrainer.py
--rw-r--r--   0 man4j     (1000) man4j     (1000)     1830 2024-05-24 09:19:49.000000 aistrainer-0.0.4/src/aistrainer/models.py
-drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-06-03 08:35:42.813174 aistrainer-0.0.4/src/aistrainer.egg-info/
--rw-r--r--   0 man4j     (1000) man4j     (1000)     7270 2024-06-03 08:35:42.000000 aistrainer-0.0.4/src/aistrainer.egg-info/PKG-INFO
--rw-r--r--   0 man4j     (1000) man4j     (1000)      275 2024-06-03 08:35:42.000000 aistrainer-0.0.4/src/aistrainer.egg-info/SOURCES.txt
--rw-r--r--   0 man4j     (1000) man4j     (1000)        1 2024-06-03 08:35:42.000000 aistrainer-0.0.4/src/aistrainer.egg-info/dependency_links.txt
--rw-r--r--   0 man4j     (1000) man4j     (1000)       90 2024-06-03 08:35:42.000000 aistrainer-0.0.4/src/aistrainer.egg-info/requires.txt
--rw-r--r--   0 man4j     (1000) man4j     (1000)       11 2024-06-03 08:35:42.000000 aistrainer-0.0.4/src/aistrainer.egg-info/top_level.txt
+drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-06-03 09:23:31.838386 aistrainer-0.0.5/
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     1074 2024-05-24 14:22:02.000000 aistrainer-0.0.5/LICENSE
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     7270 2024-06-03 09:23:31.838386 aistrainer-0.0.5/PKG-INFO
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     6560 2024-06-03 08:35:04.000000 aistrainer-0.0.5/README.md
+-rw-r--r--   0 man4j     (1000) man4j     (1000)      741 2024-06-03 09:23:27.000000 aistrainer-0.0.5/pyproject.toml
+-rw-r--r--   0 man4j     (1000) man4j     (1000)       38 2024-06-03 09:23:31.838386 aistrainer-0.0.5/setup.cfg
+drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-06-03 09:23:31.838386 aistrainer-0.0.5/src/
+drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-06-03 09:23:31.838386 aistrainer-0.0.5/src/aistrainer/
+-rw-r--r--   0 man4j     (1000) man4j     (1000)    10345 2024-06-03 09:23:16.000000 aistrainer-0.0.5/src/aistrainer/aistrainer.py
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     1830 2024-05-24 09:19:49.000000 aistrainer-0.0.5/src/aistrainer/models.py
+drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-06-03 09:23:31.838386 aistrainer-0.0.5/src/aistrainer.egg-info/
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     7270 2024-06-03 09:23:31.000000 aistrainer-0.0.5/src/aistrainer.egg-info/PKG-INFO
+-rw-r--r--   0 man4j     (1000) man4j     (1000)      275 2024-06-03 09:23:31.000000 aistrainer-0.0.5/src/aistrainer.egg-info/SOURCES.txt
+-rw-r--r--   0 man4j     (1000) man4j     (1000)        1 2024-06-03 09:23:31.000000 aistrainer-0.0.5/src/aistrainer.egg-info/dependency_links.txt
+-rw-r--r--   0 man4j     (1000) man4j     (1000)       90 2024-06-03 09:23:31.000000 aistrainer-0.0.5/src/aistrainer.egg-info/requires.txt
+-rw-r--r--   0 man4j     (1000) man4j     (1000)       11 2024-06-03 09:23:31.000000 aistrainer-0.0.5/src/aistrainer.egg-info/top_level.txt
```

### Comparing `aistrainer-0.0.4/LICENSE` & `aistrainer-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aistrainer-0.0.4/PKG-INFO` & `aistrainer-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aistrainer
-Version: 0.0.4
+Version: 0.0.5
 Summary: AI Specialization Trainer for LLM models
 Author-email: Vladimir Petrukhin <man4j@ya.ru>
 Project-URL: Homepage, https://github.com/Equiron-AI/aistrainer
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aistrainer-0.0.4/README.md` & `aistrainer-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `aistrainer-0.0.4/pyproject.toml` & `aistrainer-0.0.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aistrainer"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Vladimir Petrukhin", email="man4j@ya.ru" },
 ]
 description = "AI Specialization Trainer for LLM models"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `aistrainer-0.0.4/src/aistrainer/aistrainer.py` & `aistrainer-0.0.5/src/aistrainer/aistrainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
             logger.info(self.eval_dataset)
         else:
             self.train_dataset = dataset
 
         logger.info("Train dataset:")
         logger.info(self.train_dataset)
 
-    def train(self, adapter_name, rank=16, lora_alpha=32, num_train_epochs=1, batch_size=4, gradient_steps=2):
+    def train(self, adapter_name, rank=16, lora_alpha=32, rs_lora=True, num_train_epochs=1, batch_size=4, gradient_steps=2):
         if not self.train_dataset:
             raise Exception("Dataset is not initialized")
         evaluation_strategy = "no"
         eval_steps = None
         eval_dataset = None
 
         if self.eval:
@@ -143,15 +143,15 @@
                                  per_device_eval_batch_size=batch_size,
                                  gradient_accumulation_steps=gradient_steps,
                                  eval_accumulation_steps=1,
                                  deepspeed=self.deepspeed)
 
         lora_config = LoraConfig(r=rank,
                                  lora_alpha=lora_alpha,
-                                 use_rslora=True,
+                                 use_rslora=rs_lora,
                                  target_modules=self.model_config.target_modules,
                                  lora_dropout=0.05,
                                  # use_dora=True,
                                  # init_lora_weights="pissa",
                                  task_type="CAUSAL_LM")
 
         base_model = self.load_base_model()
```

### Comparing `aistrainer-0.0.4/src/aistrainer/models.py` & `aistrainer-0.0.5/src/aistrainer/models.py`

 * *Files identical despite different names*

### Comparing `aistrainer-0.0.4/src/aistrainer.egg-info/PKG-INFO` & `aistrainer-0.0.5/src/aistrainer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aistrainer
-Version: 0.0.4
+Version: 0.0.5
 Summary: AI Specialization Trainer for LLM models
 Author-email: Vladimir Petrukhin <man4j@ya.ru>
 Project-URL: Homepage, https://github.com/Equiron-AI/aistrainer
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

