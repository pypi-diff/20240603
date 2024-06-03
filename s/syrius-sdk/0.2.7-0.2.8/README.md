# Comparing `tmp/syrius_sdk-0.2.7.tar.gz` & `tmp/syrius_sdk-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syrius_sdk-0.2.7.tar", max compression
+gzip compressed data, was "syrius_sdk-0.2.8.tar", max compression
```

## Comparing `syrius_sdk-0.2.7.tar` & `syrius_sdk-0.2.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0       22 2024-05-14 13:38:45.266651 syrius_sdk-0.2.7/README.md
--rw-r--r--   0        0        0     1222 2024-05-14 13:38:45.266651 syrius_sdk-0.2.7/pyproject.toml
--rw-r--r--   0        0        0       23 2024-05-14 13:38:45.270652 syrius_sdk-0.2.7/syrius/__init__.py
--rw-r--r--   0        0        0      122 2024-05-14 13:38:45.270652 syrius_sdk-0.2.7/syrius/__version__.py
--rw-r--r--   0        0        0     2974 2024-05-14 13:38:45.270652 syrius_sdk-0.2.7/syrius/api.py
--rw-r--r--   0        0        0      235 2024-05-14 13:38:45.270652 syrius_sdk-0.2.7/syrius/commands/ArrayFilterByCommand.py
--rw-r--r--   0        0        0      210 2024-05-14 13:38:45.270652 syrius_sdk-0.2.7/syrius/commands/ArrayKeyValueCommand.py
--rw-r--r--   0        0        0      200 2024-05-14 13:38:45.270652 syrius_sdk-0.2.7/syrius/commands/ArrayLengthCommand.py
--rw-r--r--   0        0        0      251 2024-05-14 13:38:45.270652 syrius_sdk-0.2.7/syrius/commands/ArrayOfKeyValueToArrayCommand.py
--rw-r--r--   0        0        0      270 2024-05-14 13:38:45.270652 syrius_sdk-0.2.7/syrius/commands/ArrayReduceByKeyCommand.py
--rw-r--r--   0        0        0      304 2024-05-14 13:38:45.270652 syrius_sdk-0.2.7/syrius/commands/ArraysMergeByKeyCommand.py
--rw-r--r--   0        0        0      198 2024-05-14 13:38:45.270652 syrius_sdk-0.2.7/syrius/commands/CurrencyFormatterCommand.py
--rw-r--r--   0        0        0      338 2024-05-14 13:38:45.270652 syrius_sdk-0.2.7/syrius/commands/FileTextExtractCommand.py
--rw-r--r--   0        0        0      524 2024-05-14 13:38:45.270652 syrius_sdk-0.2.7/syrius/commands/FileUploadCommand.py
--rw-r--r--   0        0        0      217 2024-05-14 13:38:45.270652 syrius_sdk-0.2.7/syrius/commands/GrtCommand.py
--rw-r--r--   0        0        0      164 2024-05-14 13:38:45.270652 syrius_sdk-0.2.7/syrius/commands/IfCommand.py
--rw-r--r--   0        0        0      249 2024-05-14 13:38:45.270652 syrius_sdk-0.2.7/syrius/commands/LoopInputCommand.py
--rw-r--r--   0        0        0      408 2024-05-14 13:38:45.270652 syrius_sdk-0.2.7/syrius/commands/OpenAICompletionCommand.py
--rw-r--r--   0        0        0      235 2024-05-14 13:38:45.270652 syrius_sdk-0.2.7/syrius/commands/PdfHighlighterCommand.py
--rw-r--r--   0        0        0      166 2024-05-14 13:38:45.270652 syrius_sdk-0.2.7/syrius/commands/PdfToMarkdownCommand.py
--rw-r--r--   0        0        0      247 2024-05-14 13:38:45.270652 syrius_sdk-0.2.7/syrius/commands/SectionRemoverCommand.py
--rw-r--r--   0        0        0      248 2024-05-14 13:38:45.270652 syrius_sdk-0.2.7/syrius/commands/SectionSplitterCommand.py
--rw-r--r--   0        0        0      275 2024-05-14 13:38:45.270652 syrius_sdk-0.2.7/syrius/commands/SentencesSplitterCommand.py
--rw-r--r--   0        0        0      239 2024-05-14 13:38:45.270652 syrius_sdk-0.2.7/syrius/commands/TemplateCommand.py
--rw-r--r--   0        0        0      190 2024-05-14 13:38:45.270652 syrius_sdk-0.2.7/syrius/commands/UnstructuredCommand.py
--rw-r--r--   0        0        0     1091 2024-05-14 13:38:45.270652 syrius_sdk-0.2.7/syrius/commands/__init__.py
--rw-r--r--   0        0        0     1326 2024-05-14 13:38:45.270652 syrius_sdk-0.2.7/syrius/commands/abstract.py
--rw-r--r--   0        0        0      172 2024-05-14 13:38:45.270652 syrius_sdk-0.2.7/syrius/exceptions.py
--rw-r--r--   0        0        0     1375 2024-05-14 13:38:45.270652 syrius_sdk-0.2.7/syrius/flow.py
--rw-r--r--   0        0        0      431 2024-05-14 13:38:45.270652 syrius_sdk-0.2.7/syrius/loops/ForCommand.py
--rw-r--r--   0        0        0        0 2024-05-14 13:38:45.270652 syrius_sdk-0.2.7/syrius/loops/__init__.py
--rw-r--r--   0        0        0      963 2024-05-14 13:38:45.270652 syrius_sdk-0.2.7/syrius/types.py
--rw-r--r--   0        0        0      913 1970-01-01 00:00:00.000000 syrius_sdk-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0       22 2024-06-03 09:25:25.799972 syrius_sdk-0.2.8/README.md
+-rw-r--r--   0        0        0     1222 2024-06-03 09:25:25.799972 syrius_sdk-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0       23 2024-06-03 09:25:25.799972 syrius_sdk-0.2.8/syrius/__init__.py
+-rw-r--r--   0        0        0      122 2024-06-03 09:25:25.799972 syrius_sdk-0.2.8/syrius/__version__.py
+-rw-r--r--   0        0        0     2974 2024-06-03 09:25:25.799972 syrius_sdk-0.2.8/syrius/api.py
+-rw-r--r--   0        0        0      235 2024-06-03 09:25:25.799972 syrius_sdk-0.2.8/syrius/commands/ArrayFilterByCommand.py
+-rw-r--r--   0        0        0      210 2024-06-03 09:25:25.799972 syrius_sdk-0.2.8/syrius/commands/ArrayKeyValueCommand.py
+-rw-r--r--   0        0        0      200 2024-06-03 09:25:25.799972 syrius_sdk-0.2.8/syrius/commands/ArrayLengthCommand.py
+-rw-r--r--   0        0        0      251 2024-06-03 09:25:25.799972 syrius_sdk-0.2.8/syrius/commands/ArrayOfKeyValueToArrayCommand.py
+-rw-r--r--   0        0        0      270 2024-06-03 09:25:25.799972 syrius_sdk-0.2.8/syrius/commands/ArrayReduceByKeyCommand.py
+-rw-r--r--   0        0        0      304 2024-06-03 09:25:25.799972 syrius_sdk-0.2.8/syrius/commands/ArraysMergeByKeyCommand.py
+-rw-r--r--   0        0        0      198 2024-06-03 09:25:25.799972 syrius_sdk-0.2.8/syrius/commands/CurrencyFormatterCommand.py
+-rw-r--r--   0        0        0      448 2024-06-03 09:25:25.799972 syrius_sdk-0.2.8/syrius/commands/FileTextExtractCommand.py
+-rw-r--r--   0        0        0      524 2024-06-03 09:25:25.799972 syrius_sdk-0.2.8/syrius/commands/FileUploadCommand.py
+-rw-r--r--   0        0        0      217 2024-06-03 09:25:25.799972 syrius_sdk-0.2.8/syrius/commands/GrtCommand.py
+-rw-r--r--   0        0        0      164 2024-06-03 09:25:25.799972 syrius_sdk-0.2.8/syrius/commands/IfCommand.py
+-rw-r--r--   0        0        0      249 2024-06-03 09:25:25.799972 syrius_sdk-0.2.8/syrius/commands/LoopInputCommand.py
+-rw-r--r--   0        0        0      408 2024-06-03 09:25:25.799972 syrius_sdk-0.2.8/syrius/commands/OpenAICompletionCommand.py
+-rw-r--r--   0        0        0      235 2024-06-03 09:25:25.799972 syrius_sdk-0.2.8/syrius/commands/PdfHighlighterCommand.py
+-rw-r--r--   0        0        0      166 2024-06-03 09:25:25.799972 syrius_sdk-0.2.8/syrius/commands/PdfToMarkdownCommand.py
+-rw-r--r--   0        0        0      247 2024-06-03 09:25:25.799972 syrius_sdk-0.2.8/syrius/commands/SectionRemoverCommand.py
+-rw-r--r--   0        0        0      248 2024-06-03 09:25:25.799972 syrius_sdk-0.2.8/syrius/commands/SectionSplitterCommand.py
+-rw-r--r--   0        0        0      275 2024-06-03 09:25:25.799972 syrius_sdk-0.2.8/syrius/commands/SentencesSplitterCommand.py
+-rw-r--r--   0        0        0      239 2024-06-03 09:25:25.799972 syrius_sdk-0.2.8/syrius/commands/TemplateCommand.py
+-rw-r--r--   0        0        0      190 2024-06-03 09:25:25.799972 syrius_sdk-0.2.8/syrius/commands/UnstructuredCommand.py
+-rw-r--r--   0        0        0     1091 2024-06-03 09:25:25.799972 syrius_sdk-0.2.8/syrius/commands/__init__.py
+-rw-r--r--   0        0        0     1326 2024-06-03 09:25:25.803973 syrius_sdk-0.2.8/syrius/commands/abstract.py
+-rw-r--r--   0        0        0      172 2024-06-03 09:25:25.803973 syrius_sdk-0.2.8/syrius/exceptions.py
+-rw-r--r--   0        0        0     1375 2024-06-03 09:25:25.803973 syrius_sdk-0.2.8/syrius/flow.py
+-rw-r--r--   0        0        0      431 2024-06-03 09:25:25.803973 syrius_sdk-0.2.8/syrius/loops/ForCommand.py
+-rw-r--r--   0        0        0        0 2024-06-03 09:25:25.803973 syrius_sdk-0.2.8/syrius/loops/__init__.py
+-rw-r--r--   0        0        0      963 2024-06-03 09:25:25.803973 syrius_sdk-0.2.8/syrius/types.py
+-rw-r--r--   0        0        0      913 1970-01-01 00:00:00.000000 syrius_sdk-0.2.8/PKG-INFO
```

### Comparing `syrius_sdk-0.2.7/pyproject.toml` & `syrius_sdk-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "syrius-sdk"
-version = "0.2.7"
+version = "0.2.8"
 description = "The Python SDK for Syrius Flow Engine"
 license = "BSD-3-Clause"
 authors = ["Andrea Mucci <andrea@clariteia.com>"]
 readme = "README.md"
 packages= [{include = "syrius"}]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `syrius_sdk-0.2.7/syrius/api.py` & `syrius_sdk-0.2.8/syrius/api.py`

 * *Files identical despite different names*

### Comparing `syrius_sdk-0.2.7/syrius/commands/FileUploadCommand.py` & `syrius_sdk-0.2.8/syrius/commands/FileUploadCommand.py`

 * *Files identical despite different names*

### Comparing `syrius_sdk-0.2.7/syrius/commands/__init__.py` & `syrius_sdk-0.2.8/syrius/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `syrius_sdk-0.2.7/syrius/commands/abstract.py` & `syrius_sdk-0.2.8/syrius/commands/abstract.py`

 * *Files identical despite different names*

### Comparing `syrius_sdk-0.2.7/syrius/flow.py` & `syrius_sdk-0.2.8/syrius/flow.py`

 * *Files identical despite different names*

### Comparing `syrius_sdk-0.2.7/syrius/types.py` & `syrius_sdk-0.2.8/syrius/types.py`

 * *Files identical despite different names*

### Comparing `syrius_sdk-0.2.7/PKG-INFO` & `syrius_sdk-0.2.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syrius-sdk
-Version: 0.2.7
+Version: 0.2.8
 Summary: The Python SDK for Syrius Flow Engine
 License: BSD-3-Clause
 Author: Andrea Mucci
 Author-email: andrea@clariteia.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

