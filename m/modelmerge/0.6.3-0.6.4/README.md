# Comparing `tmp/modelmerge-0.6.3.tar.gz` & `tmp/modelmerge-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelmerge-0.6.3.tar", last modified: Thu May 30 13:30:41 2024, max compression
+gzip compressed data, was "modelmerge-0.6.4.tar", last modified: Mon Jun  3 14:28:32 2024, max compression
```

## Comparing `modelmerge-0.6.3.tar` & `modelmerge-0.6.4.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:30:41.018096 modelmerge-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-30 13:30:30.000000 modelmerge-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-30 13:30:41.018096 modelmerge-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-30 13:30:30.000000 modelmerge-0.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 13:30:41.018096 modelmerge-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-30 13:30:30.000000 modelmerge-0.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:30:41.006096 modelmerge-0.6.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:30:41.006096 modelmerge-0.6.3/src/ModelMerge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:30:30.000000 modelmerge-0.6.3/src/ModelMerge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:30:41.010096 modelmerge-0.6.3/src/ModelMerge/models/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-30 13:30:30.000000 modelmerge-0.6.3/src/ModelMerge/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-05-30 13:30:30.000000 modelmerge-0.6.3/src/ModelMerge/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    25957 2024-05-30 13:30:30.000000 modelmerge-0.6.3/src/ModelMerge/models/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)    16024 2024-05-30 13:30:30.000000 modelmerge-0.6.3/src/ModelMerge/models/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)     5981 2024-05-30 13:30:30.000000 modelmerge-0.6.3/src/ModelMerge/models/genimi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-05-30 13:30:30.000000 modelmerge-0.6.3/src/ModelMerge/models/groq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:30:41.010096 modelmerge-0.6.3/src/ModelMerge/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-30 13:30:30.000000 modelmerge-0.6.3/src/ModelMerge/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-30 13:30:30.000000 modelmerge-0.6.3/src/ModelMerge/plugins/arXiv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7238 2024-05-30 13:30:30.000000 modelmerge-0.6.3/src/ModelMerge/plugins/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11027 2024-05-30 13:30:30.000000 modelmerge-0.6.3/src/ModelMerge/plugins/flight.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-30 13:30:30.000000 modelmerge-0.6.3/src/ModelMerge/plugins/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-30 13:30:30.000000 modelmerge-0.6.3/src/ModelMerge/plugins/run_python.py
--rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-05-30 13:30:30.000000 modelmerge-0.6.3/src/ModelMerge/plugins/tarvel.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-30 13:30:30.000000 modelmerge-0.6.3/src/ModelMerge/plugins/today.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-30 13:30:30.000000 modelmerge-0.6.3/src/ModelMerge/plugins/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11903 2024-05-30 13:30:30.000000 modelmerge-0.6.3/src/ModelMerge/plugins/websearch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:30:41.010096 modelmerge-0.6.3/src/ModelMerge/tools/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-30 13:30:30.000000 modelmerge-0.6.3/src/ModelMerge/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-05-30 13:30:30.000000 modelmerge-0.6.3/src/ModelMerge/tools/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-30 13:30:30.000000 modelmerge-0.6.3/src/ModelMerge/tools/claude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:30:41.010096 modelmerge-0.6.3/src/ModelMerge/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:30:30.000000 modelmerge-0.6.3/src/ModelMerge/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10807 2024-05-30 13:30:30.000000 modelmerge-0.6.3/src/ModelMerge/utils/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-05-30 13:30:30.000000 modelmerge-0.6.3/src/ModelMerge/utils/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:30:41.014096 modelmerge-0.6.3/src/modelmerge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-30 13:30:40.000000 modelmerge-0.6.3/src/modelmerge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-30 13:30:40.000000 modelmerge-0.6.3/src/modelmerge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 13:30:40.000000 modelmerge-0.6.3/src/modelmerge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-30 13:30:40.000000 modelmerge-0.6.3/src/modelmerge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-30 13:30:40.000000 modelmerge-0.6.3/src/modelmerge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:30:41.014096 modelmerge-0.6.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 13:30:30.000000 modelmerge-0.6.3/test/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-30 13:30:30.000000 modelmerge-0.6.3/test/test_API.py
--rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-05-30 13:30:30.000000 modelmerge-0.6.3/test/test_Web_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-30 13:30:30.000000 modelmerge-0.6.3/test/test_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-30 13:30:30.000000 modelmerge-0.6.3/test/test_claude_zh_char.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-30 13:30:30.000000 modelmerge-0.6.3/test/test_ddg_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-30 13:30:30.000000 modelmerge-0.6.3/test/test_download_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-30 13:30:30.000000 modelmerge-0.6.3/test/test_get_token_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-30 13:30:30.000000 modelmerge-0.6.3/test/test_google_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-30 13:30:30.000000 modelmerge-0.6.3/test/test_jieba.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-30 13:30:30.000000 modelmerge-0.6.3/test/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-05-30 13:30:30.000000 modelmerge-0.6.3/test/test_langchain_search_old.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-30 13:30:30.000000 modelmerge-0.6.3/test/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-05-30 13:30:30.000000 modelmerge-0.6.3/test/test_ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-30 13:30:30.000000 modelmerge-0.6.3/test/test_py_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-05-30 13:30:30.000000 modelmerge-0.6.3/test/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-30 13:30:30.000000 modelmerge-0.6.3/test/test_tikitoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-30 13:30:30.000000 modelmerge-0.6.3/test/test_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-30 13:30:30.000000 modelmerge-0.6.3/test/test_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-30 13:30:30.000000 modelmerge-0.6.3/test/test_whisper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:28:32.458840 modelmerge-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-06-03 14:28:23.000000 modelmerge-0.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-06-03 14:28:32.458840 modelmerge-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-06-03 14:28:23.000000 modelmerge-0.6.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 14:28:32.458840 modelmerge-0.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-06-03 14:28:23.000000 modelmerge-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:28:32.450840 modelmerge-0.6.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:28:32.450840 modelmerge-0.6.4/src/ModelMerge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:28:23.000000 modelmerge-0.6.4/src/ModelMerge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:28:32.450840 modelmerge-0.6.4/src/ModelMerge/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-06-03 14:28:23.000000 modelmerge-0.6.4/src/ModelMerge/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-06-03 14:28:23.000000 modelmerge-0.6.4/src/ModelMerge/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25957 2024-06-03 14:28:23.000000 modelmerge-0.6.4/src/ModelMerge/models/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16024 2024-06-03 14:28:23.000000 modelmerge-0.6.4/src/ModelMerge/models/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5981 2024-06-03 14:28:23.000000 modelmerge-0.6.4/src/ModelMerge/models/genimi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-06-03 14:28:23.000000 modelmerge-0.6.4/src/ModelMerge/models/groq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:28:32.450840 modelmerge-0.6.4/src/ModelMerge/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-06-03 14:28:23.000000 modelmerge-0.6.4/src/ModelMerge/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-06-03 14:28:23.000000 modelmerge-0.6.4/src/ModelMerge/plugins/arXiv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7238 2024-06-03 14:28:23.000000 modelmerge-0.6.4/src/ModelMerge/plugins/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11027 2024-06-03 14:28:23.000000 modelmerge-0.6.4/src/ModelMerge/plugins/flight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-06-03 14:28:23.000000 modelmerge-0.6.4/src/ModelMerge/plugins/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-06-03 14:28:23.000000 modelmerge-0.6.4/src/ModelMerge/plugins/run_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-06-03 14:28:23.000000 modelmerge-0.6.4/src/ModelMerge/plugins/tarvel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-06-03 14:28:23.000000 modelmerge-0.6.4/src/ModelMerge/plugins/today.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-06-03 14:28:23.000000 modelmerge-0.6.4/src/ModelMerge/plugins/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11903 2024-06-03 14:28:23.000000 modelmerge-0.6.4/src/ModelMerge/plugins/websearch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:28:32.454840 modelmerge-0.6.4/src/ModelMerge/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-06-03 14:28:23.000000 modelmerge-0.6.4/src/ModelMerge/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-06-03 14:28:23.000000 modelmerge-0.6.4/src/ModelMerge/tools/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-06-03 14:28:23.000000 modelmerge-0.6.4/src/ModelMerge/tools/claude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:28:32.454840 modelmerge-0.6.4/src/ModelMerge/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:28:23.000000 modelmerge-0.6.4/src/ModelMerge/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10807 2024-06-03 14:28:23.000000 modelmerge-0.6.4/src/ModelMerge/utils/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-06-03 14:28:23.000000 modelmerge-0.6.4/src/ModelMerge/utils/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:28:32.458840 modelmerge-0.6.4/src/modelmerge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-06-03 14:28:32.000000 modelmerge-0.6.4/src/modelmerge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-06-03 14:28:32.000000 modelmerge-0.6.4/src/modelmerge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 14:28:32.000000 modelmerge-0.6.4/src/modelmerge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-06-03 14:28:32.000000 modelmerge-0.6.4/src/modelmerge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-03 14:28:32.000000 modelmerge-0.6.4/src/modelmerge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:28:32.458840 modelmerge-0.6.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-06-03 14:28:23.000000 modelmerge-0.6.4/test/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-06-03 14:28:23.000000 modelmerge-0.6.4/test/test_API.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-06-03 14:28:23.000000 modelmerge-0.6.4/test/test_Web_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-06-03 14:28:23.000000 modelmerge-0.6.4/test/test_aiwaves.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-06-03 14:28:23.000000 modelmerge-0.6.4/test/test_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-06-03 14:28:23.000000 modelmerge-0.6.4/test/test_claude_zh_char.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-06-03 14:28:23.000000 modelmerge-0.6.4/test/test_ddg_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-06-03 14:28:23.000000 modelmerge-0.6.4/test/test_download_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-06-03 14:28:23.000000 modelmerge-0.6.4/test/test_get_token_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-06-03 14:28:23.000000 modelmerge-0.6.4/test/test_google_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-06-03 14:28:23.000000 modelmerge-0.6.4/test/test_jieba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-06-03 14:28:23.000000 modelmerge-0.6.4/test/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-06-03 14:28:23.000000 modelmerge-0.6.4/test/test_langchain_search_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-06-03 14:28:23.000000 modelmerge-0.6.4/test/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-06-03 14:28:23.000000 modelmerge-0.6.4/test/test_ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-06-03 14:28:23.000000 modelmerge-0.6.4/test/test_py_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-06-03 14:28:23.000000 modelmerge-0.6.4/test/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-06-03 14:28:23.000000 modelmerge-0.6.4/test/test_tikitoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-06-03 14:28:23.000000 modelmerge-0.6.4/test/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-06-03 14:28:23.000000 modelmerge-0.6.4/test/test_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-06-03 14:28:23.000000 modelmerge-0.6.4/test/test_whisper.py
```

### Comparing `modelmerge-0.6.3/LICENSE` & `modelmerge-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.3/PKG-INFO` & `modelmerge-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.6.3
+Version: 0.6.4
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: pytz
 Requires-Dist: PyExecJS
 Requires-Dist: requests
```

### Comparing `modelmerge-0.6.3/README.md` & `modelmerge-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.3/src/ModelMerge/models/base.py` & `modelmerge-0.6.4/src/ModelMerge/models/base.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.3/src/ModelMerge/models/chatgpt.py` & `modelmerge-0.6.4/src/ModelMerge/models/chatgpt.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.3/src/ModelMerge/models/claude.py` & `modelmerge-0.6.4/src/ModelMerge/models/claude.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.3/src/ModelMerge/models/genimi.py` & `modelmerge-0.6.4/src/ModelMerge/models/genimi.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.3/src/ModelMerge/models/groq.py` & `modelmerge-0.6.4/src/ModelMerge/models/groq.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.3/src/ModelMerge/plugins/arXiv.py` & `modelmerge-0.6.4/src/ModelMerge/plugins/arXiv.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.3/src/ModelMerge/plugins/config.py` & `modelmerge-0.6.4/src/ModelMerge/plugins/config.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.3/src/ModelMerge/plugins/flight.py` & `modelmerge-0.6.4/src/ModelMerge/plugins/flight.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.3/src/ModelMerge/plugins/image.py` & `modelmerge-0.6.4/src/ModelMerge/plugins/image.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.3/src/ModelMerge/plugins/tarvel.py` & `modelmerge-0.6.4/src/ModelMerge/plugins/tarvel.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,16 +74,16 @@
     routes = soup.find_all('a', href=True, string=True)
     urls = []
     for route in routes:
         urls.append(route['href'])
     return urls
 
 def get_mafengwo_all_text(soup):
-    all_text = soup.get_text()
-    return all_text
+    # all_text = soup.get_text()
+    # return all_text
     # print(soup)
     # exit(0)
     all_text = "<travel_plan>\n\n"
     title = soup.find('h1').text.strip()
     all_text += "旅游方案：{title}\n\n".format(title=title)
     days = soup.find_all('div', class_='day-item')
     all_text += "以下是路线概览：\n\n"
```

### Comparing `modelmerge-0.6.3/src/ModelMerge/plugins/websearch.py` & `modelmerge-0.6.4/src/ModelMerge/plugins/websearch.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.3/src/ModelMerge/tools/chatgpt.py` & `modelmerge-0.6.4/src/ModelMerge/tools/chatgpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,19 +143,19 @@
         "name": "get_Round_trip_flight_price",
         "description": "Get round-trip ticket prices between two cities for the next six months",
         "parameters": {
             "type": "object",
             "properties": {
                 "departcity": {
                     "type": "string",
-                    "description": "the chinese name of departure city"
+                    "description": "the chinese name of departure city. e.g. 上海"
                 },
                 "arrivalcity": {
                     "type": "string",
-                    "description": "the chinese name of arrival city"
+                    "description": "the chinese name of arrival city. e.g. 北京"
                 }
             },
             "required": [
                 "departcity",
                 "arrivalcity"
             ]
         }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `modelmerge-0.6.3/src/ModelMerge/tools/claude.py` & `modelmerge-0.6.4/src/ModelMerge/tools/claude.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.3/src/ModelMerge/utils/prompt.py` & `modelmerge-0.6.4/src/ModelMerge/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.3/src/ModelMerge/utils/scripts.py` & `modelmerge-0.6.4/src/ModelMerge/utils/scripts.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.3/src/modelmerge.egg-info/PKG-INFO` & `modelmerge-0.6.4/src/modelmerge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.6.3
+Version: 0.6.4
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: pytz
 Requires-Dist: PyExecJS
 Requires-Dist: requests
```

### Comparing `modelmerge-0.6.3/src/modelmerge.egg-info/SOURCES.txt` & `modelmerge-0.6.4/src/modelmerge.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 src/modelmerge.egg-info/SOURCES.txt
 src/modelmerge.egg-info/dependency_links.txt
 src/modelmerge.egg-info/requires.txt
 src/modelmerge.egg-info/top_level.txt
 test/test.py
 test/test_API.py
 test/test_Web_crawler.py
+test/test_aiwaves.py
 test/test_class.py
 test/test_claude_zh_char.py
 test/test_ddg_search.py
 test/test_download_pdf.py
 test/test_get_token_dict.py
 test/test_google_search.py
 test/test_jieba.py
```

### Comparing `modelmerge-0.6.3/test/test_Web_crawler.py` & `modelmerge-0.6.4/test/test_Web_crawler.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.3/test/test_claude_zh_char.py` & `modelmerge-0.6.4/test/test_claude_zh_char.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.3/test/test_ddg_search.py` & `modelmerge-0.6.4/test/test_ddg_search.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.3/test/test_download_pdf.py` & `modelmerge-0.6.4/test/test_download_pdf.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.3/test/test_get_token_dict.py` & `modelmerge-0.6.4/test/test_get_token_dict.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.3/test/test_google_search.py` & `modelmerge-0.6.4/test/test_google_search.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.3/test/test_jieba.py` & `modelmerge-0.6.4/test/test_jieba.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.3/test/test_json.py` & `modelmerge-0.6.4/test/test_json.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.3/test/test_langchain_search_old.py` & `modelmerge-0.6.4/test/test_langchain_search_old.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.3/test/test_logging.py` & `modelmerge-0.6.4/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.3/test/test_ollama.py` & `modelmerge-0.6.4/test/test_ollama.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.3/test/test_py_run.py` & `modelmerge-0.6.4/test/test_py_run.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.3/test/test_requests.py` & `modelmerge-0.6.4/test/test_requests.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.3/test/test_tikitoken.py` & `modelmerge-0.6.4/test/test_tikitoken.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.3/test/test_token.py` & `modelmerge-0.6.4/test/test_token.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.3/test/test_url.py` & `modelmerge-0.6.4/test/test_url.py`

 * *Files identical despite different names*

