# Comparing `tmp/hyperchain-0.1.2.tar.gz` & `tmp/hyperchain-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperchain-0.1.2.tar", last modified: Wed Mar 13 15:24:56 2024, max compression
+gzip compressed data, was "hyperchain-0.1.3.tar", last modified: Mon Jun  3 13:10:13 2024, max compression
```

## Comparing `hyperchain-0.1.2.tar` & `hyperchain-0.1.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:24:56.646991 hyperchain-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-13 15:24:46.000000 hyperchain-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-13 15:24:46.000000 hyperchain-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-03-13 15:24:56.646991 hyperchain-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-03-13 15:24:46.000000 hyperchain-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:24:56.638991 hyperchain-0.1.2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-03-13 15:24:46.000000 hyperchain-0.1.2/examples/example_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-03-13 15:24:46.000000 hyperchain-0.1.2/examples/example_chat_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-03-13 15:24:46.000000 hyperchain-0.1.2/examples/example_cross_platform.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-03-13 15:24:46.000000 hyperchain-0.1.2/examples/example_function_map.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-13 15:24:46.000000 hyperchain-0.1.2/examples/example_masked_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-03-13 15:24:46.000000 hyperchain-0.1.2/examples/example_run_multiple.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-13 15:24:46.000000 hyperchain-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-03-13 15:24:56.646991 hyperchain-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-13 15:24:46.000000 hyperchain-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:24:56.638991 hyperchain-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:24:56.638991 hyperchain-0.1.2/src/hyperchain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 15:24:46.000000 hyperchain-0.1.2/src/hyperchain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:24:56.642991 hyperchain-0.1.2/src/hyperchain/chain/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-13 15:24:46.000000 hyperchain-0.1.2/src/hyperchain/chain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-03-13 15:24:46.000000 hyperchain-0.1.2/src/hyperchain/chain/chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-03-13 15:24:46.000000 hyperchain-0.1.2/src/hyperchain/chain/chain_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     7192 2024-03-13 15:24:46.000000 hyperchain-0.1.2/src/hyperchain/chain/chain_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-03-13 15:24:46.000000 hyperchain-0.1.2/src/hyperchain/chain/function_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-03-13 15:24:46.000000 hyperchain-0.1.2/src/hyperchain/chain/function_map_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-03-13 15:24:46.000000 hyperchain-0.1.2/src/hyperchain/chain/llm_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:24:56.642991 hyperchain-0.1.2/src/hyperchain/llm_runners/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-13 15:24:46.000000 hyperchain-0.1.2/src/hyperchain/llm_runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-13 15:24:46.000000 hyperchain-0.1.2/src/hyperchain/llm_runners/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-03-13 15:24:46.000000 hyperchain-0.1.2/src/hyperchain/llm_runners/hf_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-03-13 15:24:46.000000 hyperchain-0.1.2/src/hyperchain/llm_runners/llm_result.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      531 2024-03-13 15:24:46.000000 hyperchain-0.1.2/src/hyperchain/llm_runners/llm_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-03-13 15:24:46.000000 hyperchain-0.1.2/src/hyperchain/llm_runners/masked_model_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    15727 2024-03-13 15:24:46.000000 hyperchain-0.1.2/src/hyperchain/llm_runners/openai_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:24:56.646991 hyperchain-0.1.2/src/hyperchain/llm_runners/response_length_prediction/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 15:24:46.000000 hyperchain-0.1.2/src/hyperchain/llm_runners/response_length_prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-03-13 15:24:46.000000 hyperchain-0.1.2/src/hyperchain/llm_runners/response_length_prediction/automatas.py
--rw-r--r--   0 runner    (1001) docker     (127)   303505 2024-03-13 15:24:46.000000 hyperchain-0.1.2/src/hyperchain/llm_runners/response_length_prediction/parts_of_speech.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-03-13 15:24:46.000000 hyperchain-0.1.2/src/hyperchain/llm_runners/response_length_prediction/prediction.py
--rw-r--r--   0 runner    (1001) docker     (127)   640379 2024-03-13 15:24:46.000000 hyperchain-0.1.2/src/hyperchain/llm_runners/response_length_prediction/svr_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-03-13 15:24:46.000000 hyperchain-0.1.2/src/hyperchain/llm_runners/response_length_prediction/task_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-03-13 15:24:46.000000 hyperchain-0.1.2/src/hyperchain/llm_runners/response_length_prediction/task_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-03-13 15:24:46.000000 hyperchain-0.1.2/src/hyperchain/llm_runners/response_length_prediction/word_tagging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-03-13 15:24:46.000000 hyperchain-0.1.2/src/hyperchain/llm_runners/t5_model_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-13 15:24:46.000000 hyperchain-0.1.2/src/hyperchain/llm_runners/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:24:56.646991 hyperchain-0.1.2/src/hyperchain/prompt_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-13 15:24:46.000000 hyperchain-0.1.2/src/hyperchain/prompt_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-03-13 15:24:46.000000 hyperchain-0.1.2/src/hyperchain/prompt_templates/base_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-03-13 15:24:46.000000 hyperchain-0.1.2/src/hyperchain/prompt_templates/chat_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-03-13 15:24:46.000000 hyperchain-0.1.2/src/hyperchain/prompt_templates/mask_to_sentinel_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-03-13 15:24:46.000000 hyperchain-0.1.2/src/hyperchain/prompt_templates/string_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:24:56.646991 hyperchain-0.1.2/src/hyperchain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-03-13 15:24:56.000000 hyperchain-0.1.2/src/hyperchain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-03-13 15:24:56.000000 hyperchain-0.1.2/src/hyperchain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 15:24:56.000000 hyperchain-0.1.2/src/hyperchain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-13 15:24:56.000000 hyperchain-0.1.2/src/hyperchain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-13 15:24:56.000000 hyperchain-0.1.2/src/hyperchain.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:10:13.629151 hyperchain-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-06-03 13:10:02.000000 hyperchain-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-06-03 13:10:02.000000 hyperchain-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-06-03 13:10:13.629151 hyperchain-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-06-03 13:10:02.000000 hyperchain-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:10:13.621151 hyperchain-0.1.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-06-03 13:10:02.000000 hyperchain-0.1.3/examples/example_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-06-03 13:10:02.000000 hyperchain-0.1.3/examples/example_chat_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-06-03 13:10:02.000000 hyperchain-0.1.3/examples/example_cross_platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-06-03 13:10:02.000000 hyperchain-0.1.3/examples/example_function_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-06-03 13:10:02.000000 hyperchain-0.1.3/examples/example_masked_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-06-03 13:10:02.000000 hyperchain-0.1.3/examples/example_run_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-06-03 13:10:02.000000 hyperchain-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-06-03 13:10:13.629151 hyperchain-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-06-03 13:10:02.000000 hyperchain-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:10:13.617151 hyperchain-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:10:13.621151 hyperchain-0.1.3/src/hyperchain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:10:02.000000 hyperchain-0.1.3/src/hyperchain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:10:13.621151 hyperchain-0.1.3/src/hyperchain/chain/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-06-03 13:10:02.000000 hyperchain-0.1.3/src/hyperchain/chain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-06-03 13:10:02.000000 hyperchain-0.1.3/src/hyperchain/chain/chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-06-03 13:10:02.000000 hyperchain-0.1.3/src/hyperchain/chain/chain_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7314 2024-06-03 13:10:02.000000 hyperchain-0.1.3/src/hyperchain/chain/chain_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-06-03 13:10:02.000000 hyperchain-0.1.3/src/hyperchain/chain/function_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-06-03 13:10:02.000000 hyperchain-0.1.3/src/hyperchain/chain/function_map_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-06-03 13:10:02.000000 hyperchain-0.1.3/src/hyperchain/chain/llm_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:10:13.625151 hyperchain-0.1.3/src/hyperchain/llm_runners/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-06-03 13:10:02.000000 hyperchain-0.1.3/src/hyperchain/llm_runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-06-03 13:10:02.000000 hyperchain-0.1.3/src/hyperchain/llm_runners/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-06-03 13:10:02.000000 hyperchain-0.1.3/src/hyperchain/llm_runners/hf_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-06-03 13:10:02.000000 hyperchain-0.1.3/src/hyperchain/llm_runners/llm_result.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      531 2024-06-03 13:10:02.000000 hyperchain-0.1.3/src/hyperchain/llm_runners/llm_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-06-03 13:10:02.000000 hyperchain-0.1.3/src/hyperchain/llm_runners/masked_model_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15727 2024-06-03 13:10:02.000000 hyperchain-0.1.3/src/hyperchain/llm_runners/openai_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:10:13.625151 hyperchain-0.1.3/src/hyperchain/llm_runners/response_length_prediction/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:10:02.000000 hyperchain-0.1.3/src/hyperchain/llm_runners/response_length_prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-06-03 13:10:02.000000 hyperchain-0.1.3/src/hyperchain/llm_runners/response_length_prediction/automatas.py
+-rw-r--r--   0 runner    (1001) docker     (127)   303505 2024-06-03 13:10:02.000000 hyperchain-0.1.3/src/hyperchain/llm_runners/response_length_prediction/parts_of_speech.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-06-03 13:10:02.000000 hyperchain-0.1.3/src/hyperchain/llm_runners/response_length_prediction/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (127)   640379 2024-06-03 13:10:02.000000 hyperchain-0.1.3/src/hyperchain/llm_runners/response_length_prediction/svr_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-06-03 13:10:02.000000 hyperchain-0.1.3/src/hyperchain/llm_runners/response_length_prediction/task_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-06-03 13:10:02.000000 hyperchain-0.1.3/src/hyperchain/llm_runners/response_length_prediction/task_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-06-03 13:10:02.000000 hyperchain-0.1.3/src/hyperchain/llm_runners/response_length_prediction/word_tagging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-06-03 13:10:02.000000 hyperchain-0.1.3/src/hyperchain/llm_runners/t5_model_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-06-03 13:10:02.000000 hyperchain-0.1.3/src/hyperchain/llm_runners/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:10:13.629151 hyperchain-0.1.3/src/hyperchain/prompt_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-06-03 13:10:02.000000 hyperchain-0.1.3/src/hyperchain/prompt_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-06-03 13:10:02.000000 hyperchain-0.1.3/src/hyperchain/prompt_templates/base_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-06-03 13:10:02.000000 hyperchain-0.1.3/src/hyperchain/prompt_templates/chat_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-06-03 13:10:02.000000 hyperchain-0.1.3/src/hyperchain/prompt_templates/mask_to_sentinel_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-06-03 13:10:02.000000 hyperchain-0.1.3/src/hyperchain/prompt_templates/string_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:10:13.629151 hyperchain-0.1.3/src/hyperchain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-06-03 13:10:13.000000 hyperchain-0.1.3/src/hyperchain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-06-03 13:10:13.000000 hyperchain-0.1.3/src/hyperchain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 13:10:13.000000 hyperchain-0.1.3/src/hyperchain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-06-03 13:10:13.000000 hyperchain-0.1.3/src/hyperchain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-03 13:10:13.000000 hyperchain-0.1.3/src/hyperchain.egg-info/top_level.txt
```

### Comparing `hyperchain-0.1.2/LICENSE` & `hyperchain-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperchain-0.1.2/PKG-INFO` & `hyperchain-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperchain
-Version: 0.1.2
+Version: 0.1.3
 Summary: A high-performance LLM chaining framework for python
 Author: Damian Ziaber
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai>=1.0.0
 Requires-Dist: tiktoken
 Requires-Dist: scipy
```

### Comparing `hyperchain-0.1.2/README.md` & `hyperchain-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `hyperchain-0.1.2/examples/example_chain.py` & `hyperchain-0.1.3/examples/example_chain.py`

 * *Files identical despite different names*

### Comparing `hyperchain-0.1.2/examples/example_chat_chain.py` & `hyperchain-0.1.3/examples/example_chat_chain.py`

 * *Files identical despite different names*

### Comparing `hyperchain-0.1.2/examples/example_cross_platform.py` & `hyperchain-0.1.3/examples/example_cross_platform.py`

 * *Files identical despite different names*

### Comparing `hyperchain-0.1.2/examples/example_function_map.py` & `hyperchain-0.1.3/examples/example_function_map.py`

 * *Files identical despite different names*

### Comparing `hyperchain-0.1.2/examples/example_masked_code.py` & `hyperchain-0.1.3/examples/example_masked_code.py`

 * *Files identical despite different names*

### Comparing `hyperchain-0.1.2/examples/example_run_multiple.py` & `hyperchain-0.1.3/examples/example_run_multiple.py`

 * *Files identical despite different names*

### Comparing `hyperchain-0.1.2/setup.cfg` & `hyperchain-0.1.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hyperchain
-version = 0.1.2
+version = 0.1.3
 description = A high-performance LLM chaining framework for python
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Damian Ziaber
 
 [options]
 packages = find:
```

### Comparing `hyperchain-0.1.2/src/hyperchain/chain/chain.py` & `hyperchain-0.1.3/src/hyperchain/chain/chain.py`

 * *Files identical despite different names*

### Comparing `hyperchain-0.1.2/src/hyperchain/chain/chain_result.py` & `hyperchain-0.1.3/src/hyperchain/chain/chain_result.py`

 * *Files 27% similar despite different names*

```diff
@@ -24,16 +24,23 @@
         if name == "next_result":
             return self.next_result
         
         if name in self.output_dict:
             return str(self.output_dict[name])
         
         return None
+    
+    def __getitem__(self, key):
+        return self.output_dict[key]
 
 
 class ChainResultList(list):
     def __getstate__(self): return self.__dict__
 
     def __setstate__(self, state): self.__dict__ = state
 
     def __getattr__(self, name):
-        return [chain.__getattr__(name) for chain in self]
+        return [chain.__getattr__(name) for chain in self]
+    
+    def __getitem__(self, key):
+        return [chain[key] for chain in self]
+
```

### Comparing `hyperchain-0.1.2/src/hyperchain/chain/chain_sequence.py` & `hyperchain-0.1.3/src/hyperchain/chain/chain_sequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,17 @@
                 previous_result.next_result = result
             
             previous_result = result
 
         return previous_result
     
     async def async_run_multiple(self, *inputs_list: Any) -> ChainResult:
+        if len(inputs_list) == 1:
+            return ChainResultList([await self.async_run(**(inputs_list[0]))])
+        
         sequence_elements = chains_to_sequence_elements(self.chains, len(inputs_list))
         
         inputs_list_with_priority = [PriorityDict(inputs_dict, -1) for inputs_dict in inputs_list]
 
         await asyncio.gather(*[element.notify_done(inputs_list_with_priority) for element in sequence_elements])
 
         previous_result = [None for _ in range(len(inputs_list))]
```

### Comparing `hyperchain-0.1.2/src/hyperchain/chain/function_chain.py` & `hyperchain-0.1.3/src/hyperchain/chain/function_chain.py`

 * *Files identical despite different names*

### Comparing `hyperchain-0.1.2/src/hyperchain/chain/function_map_chain.py` & `hyperchain-0.1.3/src/hyperchain/chain/function_map_chain.py`

 * *Files identical despite different names*

### Comparing `hyperchain-0.1.2/src/hyperchain/chain/llm_chain.py` & `hyperchain-0.1.3/src/hyperchain/chain/llm_chain.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,24 +25,28 @@
     _wait_until = 0
 
     def __init__(
         self,
         template: Template,
         llm_runner: LLMRunner,
         output_name: str = "result",
+        is_blocked_by_LLMs = True
     ):
         if isinstance(template, str):
             template = StringTemplate(input_string=template)
         
         self.template = template
         self.llm_runner = llm_runner
         self.output_name = output_name
 
-        self.output_keys = [output_name]
+        self.output_keys = [output_name, "_local_model_blocking"]
+        
         self.required_keys = template.required_keys
+        if is_blocked_by_LLMs and self.required_keys is not None:
+            self.required_keys += ["_local_model_blocking"]
 
     async def _run_with_error_handling(self, task):
         handlers = self.llm_runner._get_error_handlers()
         while True:
             holds_a_lock = False
             try:
                 await self._error_handling_lock.acquire()
```

### Comparing `hyperchain-0.1.2/src/hyperchain/llm_runners/error_handler.py` & `hyperchain-0.1.3/src/hyperchain/llm_runners/error_handler.py`

 * *Files identical despite different names*

### Comparing `hyperchain-0.1.2/src/hyperchain/llm_runners/hf_runner.py` & `hyperchain-0.1.3/src/hyperchain/llm_runners/hf_runner.py`

 * *Files identical despite different names*

### Comparing `hyperchain-0.1.2/src/hyperchain/llm_runners/llm_result.py` & `hyperchain-0.1.3/src/hyperchain/llm_runners/llm_result.py`

 * *Files identical despite different names*

### Comparing `hyperchain-0.1.2/src/hyperchain/llm_runners/llm_runner.py` & `hyperchain-0.1.3/src/hyperchain/llm_runners/llm_runner.py`

 * *Files identical despite different names*

### Comparing `hyperchain-0.1.2/src/hyperchain/llm_runners/masked_model_runner.py` & `hyperchain-0.1.3/src/hyperchain/llm_runners/masked_model_runner.py`

 * *Files identical despite different names*

### Comparing `hyperchain-0.1.2/src/hyperchain/llm_runners/openai_runner.py` & `hyperchain-0.1.3/src/hyperchain/llm_runners/openai_runner.py`

 * *Files identical despite different names*

### Comparing `hyperchain-0.1.2/src/hyperchain/llm_runners/response_length_prediction/automatas.py` & `hyperchain-0.1.3/src/hyperchain/llm_runners/response_length_prediction/automatas.py`

 * *Files identical despite different names*

### Comparing `hyperchain-0.1.2/src/hyperchain/llm_runners/response_length_prediction/parts_of_speech.py` & `hyperchain-0.1.3/src/hyperchain/llm_runners/response_length_prediction/parts_of_speech.py`

 * *Files identical despite different names*

### Comparing `hyperchain-0.1.2/src/hyperchain/llm_runners/response_length_prediction/prediction.py` & `hyperchain-0.1.3/src/hyperchain/llm_runners/response_length_prediction/prediction.py`

 * *Files identical despite different names*

### Comparing `hyperchain-0.1.2/src/hyperchain/llm_runners/response_length_prediction/svr_data.py` & `hyperchain-0.1.3/src/hyperchain/llm_runners/response_length_prediction/svr_data.py`

 * *Files identical despite different names*

### Comparing `hyperchain-0.1.2/src/hyperchain/llm_runners/response_length_prediction/task_extraction.py` & `hyperchain-0.1.3/src/hyperchain/llm_runners/response_length_prediction/task_extraction.py`

 * *Files identical despite different names*

### Comparing `hyperchain-0.1.2/src/hyperchain/llm_runners/response_length_prediction/task_parsing.py` & `hyperchain-0.1.3/src/hyperchain/llm_runners/response_length_prediction/task_parsing.py`

 * *Files identical despite different names*

### Comparing `hyperchain-0.1.2/src/hyperchain/llm_runners/response_length_prediction/word_tagging.py` & `hyperchain-0.1.3/src/hyperchain/llm_runners/response_length_prediction/word_tagging.py`

 * *Files identical despite different names*

### Comparing `hyperchain-0.1.2/src/hyperchain/llm_runners/t5_model_runner.py` & `hyperchain-0.1.3/src/hyperchain/llm_runners/t5_model_runner.py`

 * *Files identical despite different names*

### Comparing `hyperchain-0.1.2/src/hyperchain/prompt_templates/base_template.py` & `hyperchain-0.1.3/src/hyperchain/prompt_templates/base_template.py`

 * *Files identical despite different names*

### Comparing `hyperchain-0.1.2/src/hyperchain/prompt_templates/chat_template.py` & `hyperchain-0.1.3/src/hyperchain/prompt_templates/chat_template.py`

 * *Files identical despite different names*

### Comparing `hyperchain-0.1.2/src/hyperchain/prompt_templates/mask_to_sentinel_template.py` & `hyperchain-0.1.3/src/hyperchain/prompt_templates/mask_to_sentinel_template.py`

 * *Files identical despite different names*

### Comparing `hyperchain-0.1.2/src/hyperchain/prompt_templates/string_template.py` & `hyperchain-0.1.3/src/hyperchain/prompt_templates/string_template.py`

 * *Files identical despite different names*

### Comparing `hyperchain-0.1.2/src/hyperchain.egg-info/PKG-INFO` & `hyperchain-0.1.3/src/hyperchain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperchain
-Version: 0.1.2
+Version: 0.1.3
 Summary: A high-performance LLM chaining framework for python
 Author: Damian Ziaber
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai>=1.0.0
 Requires-Dist: tiktoken
 Requires-Dist: scipy
```

### Comparing `hyperchain-0.1.2/src/hyperchain.egg-info/SOURCES.txt` & `hyperchain-0.1.3/src/hyperchain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

