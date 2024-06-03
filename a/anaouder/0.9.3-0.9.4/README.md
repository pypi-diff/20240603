# Comparing `tmp/anaouder-0.9.3.tar.gz` & `tmp/anaouder-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anaouder-0.9.3.tar", last modified: Sun Jun  2 16:34:24 2024, max compression
+gzip compressed data, was "anaouder-0.9.4.tar", last modified: Mon Jun  3 08:16:42 2024, max compression
```

## Comparing `anaouder-0.9.3.tar` & `anaouder-0.9.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-06-02 16:34:24.869675 anaouder-0.9.3/
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     2208 2024-06-02 16:11:42.000000 anaouder-0.9.3/CHANGELOG.md
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     1078 2023-03-09 20:15:12.000000 anaouder-0.9.3/LICENSE
--rw-r--r--   0 gweltaz   (1000) gweltaz   (1000)     6544 2024-06-02 16:34:24.868675 anaouder-0.9.3/PKG-INFO
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     5609 2024-05-13 11:51:35.000000 anaouder-0.9.3/README-fr.md
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     4965 2024-05-17 14:24:32.000000 anaouder-0.9.3/README.md
-drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-06-02 16:34:24.854676 anaouder-0.9.3/anaouder/
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)      180 2023-10-21 14:25:36.000000 anaouder-0.9.3/anaouder/__init__.py
--rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)    11584 2024-05-15 07:55:00.000000 anaouder-0.9.3/anaouder/adskrivan.py
-drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-06-02 16:34:24.860675 anaouder-0.9.3/anaouder/asr/
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)        0 2023-05-20 06:43:27.000000 anaouder-0.9.3/anaouder/asr/__init__.py
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)       74 2023-05-20 06:43:27.000000 anaouder-0.9.3/anaouder/asr/inorm_units.tsv
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3711 2024-06-02 16:13:08.000000 anaouder-0.9.3/anaouder/asr/models.py
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     6255 2024-05-13 10:09:57.000000 anaouder-0.9.3/anaouder/asr/post_processing.py
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     2797 2024-03-05 10:58:22.000000 anaouder-0.9.3/anaouder/asr/postproc_sub.tsv
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     4870 2024-05-14 16:45:26.000000 anaouder-0.9.3/anaouder/asr/recognizer.py
-drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-06-02 16:34:24.861675 anaouder-0.9.3/anaouder/audio/
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     5690 2024-05-17 20:18:57.000000 anaouder-0.9.3/anaouder/audio/__init__.py
-drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-06-02 16:34:24.865675 anaouder-0.9.3/anaouder/dicts/
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     2769 2023-10-21 14:25:36.000000 anaouder-0.9.3/anaouder/dicts/__init__.py
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3263 2024-03-05 10:58:22.000000 anaouder-0.9.3/anaouder/dicts/acronyms.tsv
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     5601 2024-03-05 10:58:22.000000 anaouder-0.9.3/anaouder/dicts/corrected_tokens.tsv
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3328 2024-03-05 10:58:22.000000 anaouder-0.9.3/anaouder/dicts/noun_f.tsv
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     4439 2024-03-05 10:58:22.000000 anaouder-0.9.3/anaouder/dicts/noun_m.tsv
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)    18304 2024-03-05 10:58:22.000000 anaouder-0.9.3/anaouder/dicts/proper_nouns_phon.tsv
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3415 2024-03-05 10:58:22.000000 anaouder-0.9.3/anaouder/dicts/standard_tokens.tsv
--rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)      206 2023-11-30 08:14:18.000000 anaouder-0.9.3/anaouder/istitlan.py
--rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)    11135 2024-03-09 15:05:10.000000 anaouder-0.9.3/anaouder/linennan.py
--rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)     3688 2024-03-09 16:46:02.000000 anaouder-0.9.3/anaouder/mikro.py
--rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)     1185 2023-11-10 20:39:34.000000 anaouder-0.9.3/anaouder/normalizan.py
-drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-06-02 16:34:24.867675 anaouder-0.9.3/anaouder/text/
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3446 2023-11-10 20:39:34.000000 anaouder-0.9.3/anaouder/text/__init__.py
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     4275 2023-05-23 13:01:08.000000 anaouder-0.9.3/anaouder/text/definitions.py
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)    13824 2023-11-10 20:39:34.000000 anaouder-0.9.3/anaouder/text/inverse_normalizer.py
--rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)    10825 2023-10-21 14:25:37.000000 anaouder-0.9.3/anaouder/text/normalizer.py
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)    18371 2023-10-21 14:25:37.000000 anaouder-0.9.3/anaouder/text/tokenizer.py
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3687 2023-10-21 14:25:37.000000 anaouder-0.9.3/anaouder/text/utils.py
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     5396 2024-05-13 08:15:45.000000 anaouder-0.9.3/anaouder/utils.py
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)       17 2024-06-02 16:12:15.000000 anaouder-0.9.3/anaouder/version.py
-drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-06-02 16:34:24.868675 anaouder-0.9.3/anaouder.egg-info/
--rw-r--r--   0 gweltaz   (1000) gweltaz   (1000)     6544 2024-06-02 16:34:24.000000 anaouder-0.9.3/anaouder.egg-info/PKG-INFO
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)      987 2024-06-02 16:34:24.000000 anaouder-0.9.3/anaouder.egg-info/SOURCES.txt
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)        1 2024-06-02 16:34:24.000000 anaouder-0.9.3/anaouder.egg-info/dependency_links.txt
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)      188 2024-06-02 16:34:24.000000 anaouder-0.9.3/anaouder.egg-info/entry_points.txt
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)       73 2024-06-02 16:34:24.000000 anaouder-0.9.3/anaouder.egg-info/requires.txt
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)        9 2024-06-02 16:34:24.000000 anaouder-0.9.3/anaouder.egg-info/top_level.txt
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)       38 2024-06-02 16:34:24.869675 anaouder-0.9.3/setup.cfg
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     2083 2024-06-02 16:33:31.000000 anaouder-0.9.3/setup.py
+drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-06-03 08:16:42.055354 anaouder-0.9.4/
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     2208 2024-06-03 08:16:16.000000 anaouder-0.9.4/CHANGELOG.md
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     1078 2023-03-09 20:15:12.000000 anaouder-0.9.4/LICENSE
+-rw-r--r--   0 gweltaz   (1000) gweltaz   (1000)     6544 2024-06-03 08:16:42.054354 anaouder-0.9.4/PKG-INFO
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     5609 2024-05-13 11:51:35.000000 anaouder-0.9.4/README-fr.md
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     4965 2024-05-17 14:24:32.000000 anaouder-0.9.4/README.md
+drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-06-03 08:16:42.045348 anaouder-0.9.4/anaouder/
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)      180 2023-10-21 14:25:36.000000 anaouder-0.9.4/anaouder/__init__.py
+-rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)    11584 2024-05-15 07:55:00.000000 anaouder-0.9.4/anaouder/adskrivan.py
+drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-06-03 08:16:42.048350 anaouder-0.9.4/anaouder/asr/
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)        0 2023-05-20 06:43:27.000000 anaouder-0.9.4/anaouder/asr/__init__.py
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)       74 2023-05-20 06:43:27.000000 anaouder-0.9.4/anaouder/asr/inorm_units.tsv
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3711 2024-06-02 16:13:08.000000 anaouder-0.9.4/anaouder/asr/models.py
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     6255 2024-05-13 10:09:57.000000 anaouder-0.9.4/anaouder/asr/post_processing.py
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     2797 2024-03-05 10:58:22.000000 anaouder-0.9.4/anaouder/asr/postproc_sub.tsv
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     4870 2024-05-14 16:45:26.000000 anaouder-0.9.4/anaouder/asr/recognizer.py
+drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-06-03 08:16:42.048350 anaouder-0.9.4/anaouder/audio/
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     5690 2024-05-17 20:18:57.000000 anaouder-0.9.4/anaouder/audio/__init__.py
+drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-06-03 08:16:42.050351 anaouder-0.9.4/anaouder/dicts/
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     2769 2023-10-21 14:25:36.000000 anaouder-0.9.4/anaouder/dicts/__init__.py
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3263 2024-03-05 10:58:22.000000 anaouder-0.9.4/anaouder/dicts/acronyms.tsv
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     5601 2024-03-05 10:58:22.000000 anaouder-0.9.4/anaouder/dicts/corrected_tokens.tsv
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3328 2024-03-05 10:58:22.000000 anaouder-0.9.4/anaouder/dicts/noun_f.tsv
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     4439 2024-03-05 10:58:22.000000 anaouder-0.9.4/anaouder/dicts/noun_m.tsv
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)    18304 2024-03-05 10:58:22.000000 anaouder-0.9.4/anaouder/dicts/proper_nouns_phon.tsv
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3415 2024-03-05 10:58:22.000000 anaouder-0.9.4/anaouder/dicts/standard_tokens.tsv
+-rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)      206 2023-11-30 08:14:18.000000 anaouder-0.9.4/anaouder/istitlan.py
+-rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)    11135 2024-03-09 15:05:10.000000 anaouder-0.9.4/anaouder/linennan.py
+-rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)     3688 2024-03-09 16:46:02.000000 anaouder-0.9.4/anaouder/mikro.py
+-rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)     1185 2023-11-10 20:39:34.000000 anaouder-0.9.4/anaouder/normalizan.py
+drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-06-03 08:16:42.053353 anaouder-0.9.4/anaouder/text/
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3446 2023-11-10 20:39:34.000000 anaouder-0.9.4/anaouder/text/__init__.py
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     4275 2023-05-23 13:01:08.000000 anaouder-0.9.4/anaouder/text/definitions.py
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)    13824 2023-11-10 20:39:34.000000 anaouder-0.9.4/anaouder/text/inverse_normalizer.py
+-rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)    10825 2023-10-21 14:25:37.000000 anaouder-0.9.4/anaouder/text/normalizer.py
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)    18371 2023-10-21 14:25:37.000000 anaouder-0.9.4/anaouder/text/tokenizer.py
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3687 2023-10-21 14:25:37.000000 anaouder-0.9.4/anaouder/text/utils.py
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     5396 2024-05-13 08:15:45.000000 anaouder-0.9.4/anaouder/utils.py
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)       17 2024-06-03 08:16:04.000000 anaouder-0.9.4/anaouder/version.py
+drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-06-03 08:16:42.053353 anaouder-0.9.4/anaouder.egg-info/
+-rw-r--r--   0 gweltaz   (1000) gweltaz   (1000)     6544 2024-06-03 08:16:42.000000 anaouder-0.9.4/anaouder.egg-info/PKG-INFO
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)      987 2024-06-03 08:16:42.000000 anaouder-0.9.4/anaouder.egg-info/SOURCES.txt
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)        1 2024-06-03 08:16:42.000000 anaouder-0.9.4/anaouder.egg-info/dependency_links.txt
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)      188 2024-06-03 08:16:42.000000 anaouder-0.9.4/anaouder.egg-info/entry_points.txt
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)       73 2024-06-03 08:16:42.000000 anaouder-0.9.4/anaouder.egg-info/requires.txt
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)        9 2024-06-03 08:16:42.000000 anaouder-0.9.4/anaouder.egg-info/top_level.txt
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)       38 2024-06-03 08:16:42.055354 anaouder-0.9.4/setup.cfg
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     2083 2024-06-02 16:33:31.000000 anaouder-0.9.4/setup.py
```

### Comparing `anaouder-0.9.3/CHANGELOG.md` & `anaouder-0.9.4/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
-## [0.9.3] - 2024-06-02
+## [0.9.4] - 2024-06-03
 
 - Fixed model selection when outputing to a txt file.
 - Fixed inference with progress bar for MKV files.
 - Fixed MacOS compatibility issue when downloading models.
 
 ## [0.9.2] - 2024-05-14
```

### Comparing `anaouder-0.9.3/LICENSE` & `anaouder-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.3/PKG-INFO` & `anaouder-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anaouder
-Version: 0.9.3
+Version: 0.9.4
 Summary: Breton language speech-to-text tools
 Home-page: https://github.com/gweltou/vosk-br
 Author: Gweltaz Duval-Guennoc
 Author-email: gweltou@hotmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `anaouder-0.9.3/README-fr.md` & `anaouder-0.9.4/README-fr.md`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.3/README.md` & `anaouder-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.3/anaouder/adskrivan.py` & `anaouder-0.9.4/anaouder/adskrivan.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.3/anaouder/asr/models.py` & `anaouder-0.9.4/anaouder/asr/models.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.3/anaouder/asr/post_processing.py` & `anaouder-0.9.4/anaouder/asr/post_processing.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.3/anaouder/asr/postproc_sub.tsv` & `anaouder-0.9.4/anaouder/asr/postproc_sub.tsv`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.3/anaouder/asr/recognizer.py` & `anaouder-0.9.4/anaouder/asr/recognizer.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.3/anaouder/audio/__init__.py` & `anaouder-0.9.4/anaouder/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.3/anaouder/dicts/__init__.py` & `anaouder-0.9.4/anaouder/dicts/__init__.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.3/anaouder/dicts/acronyms.tsv` & `anaouder-0.9.4/anaouder/dicts/acronyms.tsv`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.3/anaouder/dicts/corrected_tokens.tsv` & `anaouder-0.9.4/anaouder/dicts/corrected_tokens.tsv`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.3/anaouder/dicts/noun_f.tsv` & `anaouder-0.9.4/anaouder/dicts/noun_f.tsv`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.3/anaouder/dicts/noun_m.tsv` & `anaouder-0.9.4/anaouder/dicts/noun_m.tsv`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.3/anaouder/dicts/proper_nouns_phon.tsv` & `anaouder-0.9.4/anaouder/dicts/proper_nouns_phon.tsv`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.3/anaouder/dicts/standard_tokens.tsv` & `anaouder-0.9.4/anaouder/dicts/standard_tokens.tsv`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.3/anaouder/linennan.py` & `anaouder-0.9.4/anaouder/linennan.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.3/anaouder/mikro.py` & `anaouder-0.9.4/anaouder/mikro.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.3/anaouder/normalizan.py` & `anaouder-0.9.4/anaouder/normalizan.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.3/anaouder/text/__init__.py` & `anaouder-0.9.4/anaouder/text/__init__.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.3/anaouder/text/definitions.py` & `anaouder-0.9.4/anaouder/text/definitions.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.3/anaouder/text/inverse_normalizer.py` & `anaouder-0.9.4/anaouder/text/inverse_normalizer.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.3/anaouder/text/normalizer.py` & `anaouder-0.9.4/anaouder/text/normalizer.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.3/anaouder/text/tokenizer.py` & `anaouder-0.9.4/anaouder/text/tokenizer.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.3/anaouder/text/utils.py` & `anaouder-0.9.4/anaouder/text/utils.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.3/anaouder/utils.py` & `anaouder-0.9.4/anaouder/utils.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.3/anaouder.egg-info/PKG-INFO` & `anaouder-0.9.4/anaouder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anaouder
-Version: 0.9.3
+Version: 0.9.4
 Summary: Breton language speech-to-text tools
 Home-page: https://github.com/gweltou/vosk-br
 Author: Gweltaz Duval-Guennoc
 Author-email: gweltou@hotmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `anaouder-0.9.3/anaouder.egg-info/SOURCES.txt` & `anaouder-0.9.4/anaouder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.3/setup.py` & `anaouder-0.9.4/setup.py`

 * *Files identical despite different names*

