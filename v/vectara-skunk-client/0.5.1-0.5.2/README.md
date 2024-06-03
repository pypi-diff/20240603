# Comparing `tmp/vectara_skunk_client-0.5.1.tar.gz` & `tmp/vectara_skunk_client-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectara_skunk_client-0.5.1.tar", last modified: Wed May 22 02:41:06 2024, max compression
+gzip compressed data, was "vectara_skunk_client-0.5.2.tar", last modified: Mon Jun  3 00:53:41 2024, max compression
```

## Comparing `vectara_skunk_client-0.5.1.tar` & `vectara_skunk_client-0.5.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 02:41:06.956835 vectara_skunk_client-0.5.1/
--rw-rw-rw-   0        0        0    34918 2023-12-21 21:26:20.000000 vectara_skunk_client-0.5.1/LICENSE.md
--rw-rw-rw-   0        0        0      911 2024-05-22 02:41:06.955835 vectara_skunk_client-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     5223 2024-04-30 03:30:49.000000 vectara_skunk_client-0.5.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-22 02:41:06.956835 vectara_skunk_client-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1830 2024-05-22 02:40:43.000000 vectara_skunk_client-0.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 02:41:06.770178 vectara_skunk_client-0.5.1/test/
--rw-rw-rw-   0        0        0     1759 2024-05-22 01:11:31.000000 vectara_skunk_client-0.5.1/test/test_core_index.py
--rw-rw-rw-   0        0        0      421 2024-05-22 01:03:28.000000 vectara_skunk_client-0.5.1/test/test_index.py
--rw-rw-rw-   0        0        0     1259 2024-05-02 01:30:04.000000 vectara_skunk_client-0.5.1/test/test_manager.py
--rw-rw-rw-   0        0        0      614 2024-01-05 23:56:06.000000 vectara_skunk_client-0.5.1/test/test_none_bool.py
--rw-rw-rw-   0        0        0     9883 2024-02-06 04:39:48.000000 vectara_skunk_client-0.5.1/test/test_query.py
--rw-rw-rw-   0        0        0      320 2024-01-12 22:21:17.000000 vectara_skunk_client-0.5.1/test/test_scratch.py
--rw-rw-rw-   0        0        0     2476 2024-01-04 21:17:59.000000 vectara_skunk_client-0.5.1/test/test_storage_quota.py
--rw-rw-rw-   0        0        0     2406 2024-01-12 21:20:02.000000 vectara_skunk_client-0.5.1/test/test_system_basic.py
--rw-rw-rw-   0        0        0     4780 2024-01-12 22:21:17.000000 vectara_skunk_client-0.5.1/test/test_util.py
-drwxrwxrwx   0        0        0        0 2024-05-22 02:41:06.929923 vectara_skunk_client-0.5.1/vectara_client/
--rw-rw-rw-   0        0        0        0 2023-12-22 03:08:32.000000 vectara_skunk_client-0.5.1/vectara_client/__init__.py
--rw-rw-rw-   0        0        0    11506 2024-04-30 04:34:01.000000 vectara_skunk_client-0.5.1/vectara_client/admin.py
--rw-rw-rw-   0        0        0     4350 2024-05-07 04:36:22.000000 vectara_skunk_client-0.5.1/vectara_client/authn.py
--rw-rw-rw-   0        0        0     2232 2024-01-12 22:54:50.000000 vectara_skunk_client-0.5.1/vectara_client/chat.py
--rw-rw-rw-   0        0        0     7769 2024-05-03 06:58:11.000000 vectara_skunk_client-0.5.1/vectara_client/config.py
--rw-rw-rw-   0        0        0     4551 2024-05-17 00:41:53.000000 vectara_skunk_client-0.5.1/vectara_client/core.py
--rw-rw-rw-   0        0        0     8885 2024-05-22 02:40:33.000000 vectara_skunk_client-0.5.1/vectara_client/corpus.py
--rw-rw-rw-   0        0        0     3173 2024-01-12 22:21:17.000000 vectara_skunk_client-0.5.1/vectara_client/dao.py
--rw-rw-rw-   0        0        0     1472 2024-01-12 22:21:17.000000 vectara_skunk_client-0.5.1/vectara_client/document.py
--rw-rw-rw-   0        0        0    12369 2024-05-22 00:57:33.000000 vectara_skunk_client-0.5.1/vectara_client/domain.py
--rw-rw-rw-   0        0        0      761 2024-04-09 05:47:51.000000 vectara_skunk_client-0.5.1/vectara_client/enums.py
--rw-rw-rw-   0        0        0        0 2024-01-04 05:06:30.000000 vectara_skunk_client-0.5.1/vectara_client/error.py
--rw-rw-rw-   0        0        0     5352 2024-05-22 00:59:33.000000 vectara_skunk_client-0.5.1/vectara_client/index.py
--rw-rw-rw-   0        0        0     1594 2024-05-02 01:29:30.000000 vectara_skunk_client-0.5.1/vectara_client/manager.py
--rw-rw-rw-   0        0        0     6086 2024-03-26 02:59:13.000000 vectara_skunk_client-0.5.1/vectara_client/query.py
--rw-rw-rw-   0        0        0     5830 2024-03-04 06:43:34.000000 vectara_skunk_client-0.5.1/vectara_client/status.py
--rw-rw-rw-   0        0        0    20575 2024-05-22 01:22:07.000000 vectara_skunk_client-0.5.1/vectara_client/util.py
-drwxrwxrwx   0        0        0        0 2024-05-22 02:41:06.954839 vectara_skunk_client-0.5.1/vectara_skunk_client.egg-info/
--rw-rw-rw-   0        0        0      911 2024-05-22 02:41:06.000000 vectara_skunk_client-0.5.1/vectara_skunk_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      861 2024-05-22 02:41:06.000000 vectara_skunk_client-0.5.1/vectara_skunk_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 02:41:06.000000 vectara_skunk_client-0.5.1/vectara_skunk_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2024-05-22 02:41:06.000000 vectara_skunk_client-0.5.1/vectara_skunk_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-22 02:41:06.000000 vectara_skunk_client-0.5.1/vectara_skunk_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-03 00:53:41.519513 vectara_skunk_client-0.5.2/
+-rw-rw-rw-   0        0        0    34918 2023-12-21 21:26:20.000000 vectara_skunk_client-0.5.2/LICENSE.md
+-rw-rw-rw-   0        0        0      911 2024-06-03 00:53:41.517363 vectara_skunk_client-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5223 2024-04-30 03:30:49.000000 vectara_skunk_client-0.5.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-03 00:53:41.519513 vectara_skunk_client-0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1830 2024-06-03 00:49:30.000000 vectara_skunk_client-0.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 00:53:41.442993 vectara_skunk_client-0.5.2/test/
+-rw-rw-rw-   0        0        0     1759 2024-05-22 01:11:31.000000 vectara_skunk_client-0.5.2/test/test_core_index.py
+-rw-rw-rw-   0        0        0      421 2024-05-22 01:03:28.000000 vectara_skunk_client-0.5.2/test/test_index.py
+-rw-rw-rw-   0        0        0     1259 2024-05-02 01:30:04.000000 vectara_skunk_client-0.5.2/test/test_manager.py
+-rw-rw-rw-   0        0        0      614 2024-01-05 23:56:06.000000 vectara_skunk_client-0.5.2/test/test_none_bool.py
+-rw-rw-rw-   0        0        0     9883 2024-02-06 04:39:48.000000 vectara_skunk_client-0.5.2/test/test_query.py
+-rw-rw-rw-   0        0        0      320 2024-01-12 22:21:17.000000 vectara_skunk_client-0.5.2/test/test_scratch.py
+-rw-rw-rw-   0        0        0     2476 2024-01-04 21:17:59.000000 vectara_skunk_client-0.5.2/test/test_storage_quota.py
+-rw-rw-rw-   0        0        0     2406 2024-01-12 21:20:02.000000 vectara_skunk_client-0.5.2/test/test_system_basic.py
+-rw-rw-rw-   0        0        0     4780 2024-01-12 22:21:17.000000 vectara_skunk_client-0.5.2/test/test_util.py
+drwxrwxrwx   0        0        0        0 2024-06-03 00:53:41.477655 vectara_skunk_client-0.5.2/vectara_client/
+-rw-rw-rw-   0        0        0        0 2023-12-22 03:08:32.000000 vectara_skunk_client-0.5.2/vectara_client/__init__.py
+-rw-rw-rw-   0        0        0    11506 2024-04-30 04:34:01.000000 vectara_skunk_client-0.5.2/vectara_client/admin.py
+-rw-rw-rw-   0        0        0     4350 2024-05-07 04:36:22.000000 vectara_skunk_client-0.5.2/vectara_client/authn.py
+-rw-rw-rw-   0        0        0     2232 2024-01-12 22:54:50.000000 vectara_skunk_client-0.5.2/vectara_client/chat.py
+-rw-rw-rw-   0        0        0     7769 2024-05-03 06:58:11.000000 vectara_skunk_client-0.5.2/vectara_client/config.py
+-rw-rw-rw-   0        0        0     4551 2024-05-17 00:41:53.000000 vectara_skunk_client-0.5.2/vectara_client/core.py
+-rw-rw-rw-   0        0        0     8885 2024-05-22 02:40:33.000000 vectara_skunk_client-0.5.2/vectara_client/corpus.py
+-rw-rw-rw-   0        0        0     3173 2024-01-12 22:21:17.000000 vectara_skunk_client-0.5.2/vectara_client/dao.py
+-rw-rw-rw-   0        0        0     1472 2024-01-12 22:21:17.000000 vectara_skunk_client-0.5.2/vectara_client/document.py
+-rw-rw-rw-   0        0        0    12420 2024-06-03 00:48:18.000000 vectara_skunk_client-0.5.2/vectara_client/domain.py
+-rw-rw-rw-   0        0        0      761 2024-04-09 05:47:51.000000 vectara_skunk_client-0.5.2/vectara_client/enums.py
+-rw-rw-rw-   0        0        0        0 2024-01-04 05:06:30.000000 vectara_skunk_client-0.5.2/vectara_client/error.py
+-rw-rw-rw-   0        0        0     5352 2024-05-22 00:59:33.000000 vectara_skunk_client-0.5.2/vectara_client/index.py
+-rw-rw-rw-   0        0        0     1594 2024-05-02 01:29:30.000000 vectara_skunk_client-0.5.2/vectara_client/manager.py
+-rw-rw-rw-   0        0        0     6086 2024-03-26 02:59:13.000000 vectara_skunk_client-0.5.2/vectara_client/query.py
+-rw-rw-rw-   0        0        0     5830 2024-03-04 06:43:34.000000 vectara_skunk_client-0.5.2/vectara_client/status.py
+-rw-rw-rw-   0        0        0    20577 2024-05-24 03:37:59.000000 vectara_skunk_client-0.5.2/vectara_client/util.py
+drwxrwxrwx   0        0        0        0 2024-06-03 00:53:41.516852 vectara_skunk_client-0.5.2/vectara_skunk_client.egg-info/
+-rw-rw-rw-   0        0        0      911 2024-06-03 00:53:41.000000 vectara_skunk_client-0.5.2/vectara_skunk_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      861 2024-06-03 00:53:41.000000 vectara_skunk_client-0.5.2/vectara_skunk_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 00:53:41.000000 vectara_skunk_client-0.5.2/vectara_skunk_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2024-06-03 00:53:41.000000 vectara_skunk_client-0.5.2/vectara_skunk_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-06-03 00:53:41.000000 vectara_skunk_client-0.5.2/vectara_skunk_client.egg-info/top_level.txt
```

### Comparing `vectara_skunk_client-0.5.1/LICENSE.md` & `vectara_skunk_client-0.5.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `vectara_skunk_client-0.5.1/PKG-INFO` & `vectara_skunk_client-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectara-skunk-client
-Version: 0.5.1
+Version: 0.5.2
 Summary: Vectara Skunk Client
 Home-page: https://github.com/davidglevy/vectara-skunk-client
 Author: David Levy
 Author-email: david.g.levy@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE v3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
```

### Comparing `vectara_skunk_client-0.5.1/README.md` & `vectara_skunk_client-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `vectara_skunk_client-0.5.1/setup.py` & `vectara_skunk_client-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         return "\n".join(lines)
 
 setup(
     name='vectara-skunk-client',
     description='Vectara Skunk Client',
     long_description=get_long_desc(),
     long_description_content_type='text/markdown',
-    version='0.5.1',
+    version='0.5.2',
     author='David Levy',
     author_email='david.g.levy@gmail.com',
     url='https://github.com/davidglevy/vectara-skunk-client',
     license='GNU AFFERO GENERAL PUBLIC LICENSE v3',
     package_dir={
         'vectara_client': 'vectara_client'
     },
```

### Comparing `vectara_skunk_client-0.5.1/test/test_core_index.py` & `vectara_skunk_client-0.5.2/test/test_core_index.py`

 * *Files identical despite different names*

### Comparing `vectara_skunk_client-0.5.1/test/test_manager.py` & `vectara_skunk_client-0.5.2/test/test_manager.py`

 * *Files identical despite different names*

### Comparing `vectara_skunk_client-0.5.1/test/test_none_bool.py` & `vectara_skunk_client-0.5.2/test/test_none_bool.py`

 * *Files identical despite different names*

### Comparing `vectara_skunk_client-0.5.1/test/test_query.py` & `vectara_skunk_client-0.5.2/test/test_query.py`

 * *Files identical despite different names*

### Comparing `vectara_skunk_client-0.5.1/test/test_storage_quota.py` & `vectara_skunk_client-0.5.2/test/test_storage_quota.py`

 * *Files identical despite different names*

### Comparing `vectara_skunk_client-0.5.1/test/test_system_basic.py` & `vectara_skunk_client-0.5.2/test/test_system_basic.py`

 * *Files identical despite different names*

### Comparing `vectara_skunk_client-0.5.1/test/test_util.py` & `vectara_skunk_client-0.5.2/test/test_util.py`

 * *Files identical despite different names*

### Comparing `vectara_skunk_client-0.5.1/vectara_client/admin.py` & `vectara_skunk_client-0.5.2/vectara_client/admin.py`

 * *Files identical despite different names*

### Comparing `vectara_skunk_client-0.5.1/vectara_client/authn.py` & `vectara_skunk_client-0.5.2/vectara_client/authn.py`

 * *Files identical despite different names*

### Comparing `vectara_skunk_client-0.5.1/vectara_client/chat.py` & `vectara_skunk_client-0.5.2/vectara_client/chat.py`

 * *Files identical despite different names*

### Comparing `vectara_skunk_client-0.5.1/vectara_client/config.py` & `vectara_skunk_client-0.5.2/vectara_client/config.py`

 * *Files identical despite different names*

### Comparing `vectara_skunk_client-0.5.1/vectara_client/core.py` & `vectara_skunk_client-0.5.2/vectara_client/core.py`

 * *Files identical despite different names*

### Comparing `vectara_skunk_client-0.5.1/vectara_client/corpus.py` & `vectara_skunk_client-0.5.2/vectara_client/corpus.py`

 * *Files identical despite different names*

### Comparing `vectara_skunk_client-0.5.1/vectara_client/dao.py` & `vectara_skunk_client-0.5.2/vectara_client/dao.py`

 * *Files identical despite different names*

### Comparing `vectara_skunk_client-0.5.1/vectara_client/document.py` & `vectara_skunk_client-0.5.2/vectara_client/document.py`

 * *Files identical despite different names*

### Comparing `vectara_skunk_client-0.5.1/vectara_client/domain.py` & `vectara_skunk_client-0.5.2/vectara_client/domain.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 from typing import List, Optional, Union
 from enum import Enum
 from vectara_client.status import Status
 from vectara_client.enums import ApiKeyStatus, ApiKeyType
 
 from dataclasses import dataclass
 
@@ -73,14 +74,15 @@
 
 @dataclass
 class ListCorpusResponse:
     corpus: List[Corpus]
     pageKey: str
     status: Optional[Status]
 
+
 @dataclass
 class ReadCorpusRequest:
     corpus_id: List[int]
     read_basic_info: bool
     read_size: bool
     read_recall: bool
     read_api_keys: bool
@@ -186,15 +188,15 @@
 @dataclass
 class Section:
     id: Optional[int]
     title: Optional[str]
     text: Optional[str]
     metadataJson: Optional[str]
     customDims: Optional[List[CustomDimension]]
-    section: Optional[List['Section']]
+    section: Optional[Section]
 
 
 @dataclass
 class Document:
     documentId: str
     title: Optional[str]
     description: Optional[str]
@@ -242,15 +244,15 @@
     DEFAULT = 0
     QUERY = 1
     RESPONSE = 2
 
 
 @dataclass
 class LinearInterpolation:
-    _lambda: Optional[float]  # Unfortunately Python dataclass attributes cannot be reserved words.
+    _lambda: Union[float, None]  # Unfortunately Python dataclass attributes cannot be reserved words.
 
 
 @dataclass
 class CorpusKey:
     corpusId: int
     customerId: Optional[int]
     semantics: Optional[str | Semantics]
@@ -284,23 +286,26 @@
 
 
 @dataclass
 class RerankingConfig:
     rerankerId: int
     mmrConfig: Optional[MMRConfig]
 
+
 @dataclass
 class ModelParams:
     maxTokens: Optional[int]
     temperature: Optional[float]
 
-    # provides even more granular control to help ensure that the summarization decreases the likelihood of repeating words. The values range from 0.0 to 1.0
+    # provides even more granular control to help ensure that the summarization decreases the likelihood
+    # of repeating words. The values range from 0.0 to 1.0
     frequencyPenalty: Optional[float]
 
-    # provides more control over whether you want the summary to include new topics. The values also range from 0.0 to 1.0.
+    # provides more control over whether you want the summary to include new topics. The values
+    # also range from 0.0 to 1.0.
     presencePenalty: Optional[float]
 
 
 @dataclass
 class ChatRequest:
     store: Optional[bool]
     conversationId: Optional[str]
@@ -352,21 +357,23 @@
 
 
 @dataclass
 class ResponseDocument:
     id: str
     metadata: List[Attribute]
 
+
 @dataclass
 class ChatResponse:
     conversationId: str
     turnId: Optional[str]
     rephrasedQuery: Optional[str]
     status: Optional[Status]
 
+
 @dataclass
 class SummaryResponse:
     text: Optional[str]
     lang: str
     prompt: str
     status: List[Status]
     chat: Optional[ChatResponse]
@@ -391,36 +398,40 @@
 
 @dataclass
 class BatchQueryResponse:
     responseSet: Optional[List[ResponseSet]]
     status: List[Status]
     metrics: Optional[PerformanceMetrics]
 
+
 @dataclass
 class CoreIndexDocumentPart:
     text: str
     context: Optional[str]
     metadata_json: Optional[str]
     custom_dims: Optional[List[CustomDimension]]
 
+
 @dataclass
 class CoreIndexDocument:
     document_id: str
     metadata_json: Optional[str]
     parts: List[CoreIndexDocumentPart]
 
+
 @dataclass
 class CoreIndexDocumentRequest:
     """
     See core_services.proto
     """
     customer_id: int
     corpus_id: int
     document: CoreIndexDocument
 
+
 @dataclass
 class CoreIndexDocumentResponse:
     """
     See core_services.proto
     """
     status: Status
     quotaConsumed: Optional[StorageQuota]
@@ -428,20 +439,21 @@
     def __post_init__(self):
         """
         Funky behavior to clear the status if it doesn't have a code
         """
         if not self.status.code:
             self.__setattr__("status", None)
 
+
 @dataclass
 class DocumentSection:
     text: Optional[str]
     context: Optional[str]
     metadata_json: Optional[str]
-    custom_dims: Optional[List[CustomDimension]]
+    section: List[DocumentSection]
 
 
 @dataclass
 class IndexDocument:
     """
     Something odd
     """
@@ -526,14 +538,15 @@
 
 
 @dataclass
 class ListDocumentItem:
     id: str
     metadata: Optional[List[Attribute]]
 
+
 @dataclass
 class DocumentDTO:
     id: str
     metadata: dict[str, Union[str, int, float, bool, List[str]]]
 
 
 @dataclass
```

### Comparing `vectara_skunk_client-0.5.1/vectara_client/enums.py` & `vectara_skunk_client-0.5.2/vectara_client/enums.py`

 * *Files identical despite different names*

### Comparing `vectara_skunk_client-0.5.1/vectara_client/index.py` & `vectara_skunk_client-0.5.2/vectara_client/index.py`

 * *Files identical despite different names*

### Comparing `vectara_skunk_client-0.5.1/vectara_client/manager.py` & `vectara_skunk_client-0.5.2/vectara_client/manager.py`

 * *Files identical despite different names*

### Comparing `vectara_skunk_client-0.5.1/vectara_client/query.py` & `vectara_skunk_client-0.5.2/vectara_client/query.py`

 * *Files identical despite different names*

### Comparing `vectara_skunk_client-0.5.1/vectara_client/status.py` & `vectara_skunk_client-0.5.2/vectara_client/status.py`

 * *Files identical despite different names*

### Comparing `vectara_skunk_client-0.5.1/vectara_client/util.py` & `vectara_skunk_client-0.5.2/vectara_client/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 
         :param method:
         :param to_class:
         :param operation: the REST operation to perform.
         :param payload: the payload which will be serialized.
         :return:
         """
+
         headers = self.auth_util.get_headers()
         headers['Content-Type'] = 'application/json'
         headers['Accept'] = 'application/json'
 
         self.logger.debug(f"Headers: {json.dumps(headers)}")
 
         self.requests.append({'operation': operation, 'payload': payload})
```

### Comparing `vectara_skunk_client-0.5.1/vectara_skunk_client.egg-info/PKG-INFO` & `vectara_skunk_client-0.5.2/vectara_skunk_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectara-skunk-client
-Version: 0.5.1
+Version: 0.5.2
 Summary: Vectara Skunk Client
 Home-page: https://github.com/davidglevy/vectara-skunk-client
 Author: David Levy
 Author-email: david.g.levy@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE v3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
```

### Comparing `vectara_skunk_client-0.5.1/vectara_skunk_client.egg-info/SOURCES.txt` & `vectara_skunk_client-0.5.2/vectara_skunk_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

