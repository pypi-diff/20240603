# Comparing `tmp/protarrow-0.4.0.tar.gz` & `tmp/protarrow-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protarrow-0.4.0.tar", max compression
+gzip compressed data, was "protarrow-0.5.2.tar", max compression
```

## Comparing `protarrow-0.4.0.tar` & `protarrow-0.5.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    10140 2024-04-11 12:53:22.158708 protarrow-0.4.0/LICENSE
--rw-r--r--   0        0        0       95 2024-04-11 12:53:22.158708 protarrow-0.4.0/NOTICE
--rw-r--r--   0        0        0     3022 2024-04-11 12:53:22.158708 protarrow-0.4.0/README.md
--rw-r--r--   0        0        0      754 2024-04-11 12:53:40.562839 protarrow-0.4.0/protarrow/__init__.py
--rw-r--r--   0        0        0    20762 2024-04-11 12:53:22.158708 protarrow-0.4.0/protarrow/arrow_to_proto.py
--rw-r--r--   0        0        0     7813 2024-04-11 12:53:22.158708 protarrow-0.4.0/protarrow/cast_to_proto.py
--rw-r--r--   0        0        0     1564 2024-04-11 12:53:22.158708 protarrow-0.4.0/protarrow/common.py
--rw-r--r--   0        0        0     4621 2024-04-11 12:53:22.158708 protarrow-0.4.0/protarrow/message_extractor.py
--rw-r--r--   0        0        0    18323 2024-04-11 12:53:22.158708 protarrow-0.4.0/protarrow/proto_to_arrow.py
--rw-r--r--   0        0        0     1979 2024-04-11 12:53:40.562839 protarrow-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4084 1970-01-01 00:00:00.000000 protarrow-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    10140 2024-06-03 08:00:08.727357 protarrow-0.5.2/LICENSE
+-rw-r--r--   0        0        0      111 2024-06-03 08:00:08.727357 protarrow-0.5.2/NOTICE
+-rw-r--r--   0        0        0     3037 2024-06-03 08:00:08.727357 protarrow-0.5.2/README.md
+-rw-r--r--   0        0        0      754 2024-06-03 08:00:22.239492 protarrow-0.5.2/protarrow/__init__.py
+-rw-r--r--   0        0        0    20762 2024-06-03 08:00:08.731356 protarrow-0.5.2/protarrow/arrow_to_proto.py
+-rw-r--r--   0        0        0     7813 2024-06-03 08:00:08.731356 protarrow-0.5.2/protarrow/cast_to_proto.py
+-rw-r--r--   0        0        0     1564 2024-06-03 08:00:08.731356 protarrow-0.5.2/protarrow/common.py
+-rw-r--r--   0        0        0     4621 2024-06-03 08:00:08.731356 protarrow-0.5.2/protarrow/message_extractor.py
+-rw-r--r--   0        0        0    18323 2024-06-03 08:00:08.731356 protarrow-0.5.2/protarrow/proto_to_arrow.py
+-rw-r--r--   0        0        0     1979 2024-06-03 08:00:22.239492 protarrow-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     4100 1970-01-01 00:00:00.000000 protarrow-0.5.2/PKG-INFO
```

### Comparing `protarrow-0.4.0/LICENSE` & `protarrow-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `protarrow-0.4.0/README.md` & `protarrow-0.5.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 [![Downloads][downloads-month-image]][downloads-month-url]
 [![Code style: black][codestyle-image]][codestyle-url]
 [![snyk][snyk-image]][snyk-url]
 
 
 # Protarrow
 
-**Protarrow** is a python library for converting from protobuf to arrow and back.
+**Protarrow** is a python library for converting from Protocol Buffers to Apache Arrow and back.
 
 It is used at [Tradewell Technologies](https://www.tradewelltech.co/), 
 to share data between transactional and analytical applications,
 with little boilerplate code and zero data loss.
 
 # Installation
```

### Comparing `protarrow-0.4.0/protarrow/__init__.py` & `protarrow-0.5.2/protarrow/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from protarrow.proto_to_arrow import (
     message_type_to_schema,
     message_type_to_struct_type,
     messages_to_record_batch,
     messages_to_table,
 )
 
-__version__ = "0.4.0"
+__version__ = "0.5.2"
 __all__ = [
     "MessageExtractor",
     "ProtarrowConfig",
     "cast_record_batch",
     "cast_struct_array",
     "cast_table",
     "message_type_to_schema",
```

### Comparing `protarrow-0.4.0/protarrow/arrow_to_proto.py` & `protarrow-0.5.2/protarrow/arrow_to_proto.py`

 * *Files identical despite different names*

### Comparing `protarrow-0.4.0/protarrow/cast_to_proto.py` & `protarrow-0.5.2/protarrow/cast_to_proto.py`

 * *Files identical despite different names*

### Comparing `protarrow-0.4.0/protarrow/common.py` & `protarrow-0.5.2/protarrow/common.py`

 * *Files identical despite different names*

### Comparing `protarrow-0.4.0/protarrow/message_extractor.py` & `protarrow-0.5.2/protarrow/message_extractor.py`

 * *Files identical despite different names*

### Comparing `protarrow-0.4.0/protarrow/proto_to_arrow.py` & `protarrow-0.5.2/protarrow/proto_to_arrow.py`

 * *Files identical despite different names*

### Comparing `protarrow-0.4.0/pyproject.toml` & `protarrow-0.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 
 [tool.poetry]
 name = "protarrow"
-version = "0.4.0"
+version = "0.5.2"
 description = "Convert from protobuf to arrow and back"
 authors = ["Tradewell Tech <engineering@tradewelltech.co>"]
 maintainers = ["0x26res <0x26res@gmail.com>"]
 packages = [
     { include = "protarrow" }
 ]
 readme = "README.md"
 license = "Apache-2.0"
 repository = "https://github.com/tradewelltech/protarrow"
 documentation = "https://protarrow.readthedocs.io/en/latest/"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 keywords = ["apache-arrow", "protobuf", "data"]
 
 [tool.poetry.dependencies]
 googleapis-common-protos = ">=1.53.0"
-protobuf = ">=3.20.1"
+protobuf = ">=3.20.1,<5"
 pyarrow = ">=12.0.0"
-python = ">=3.8,<3.12"
+python = ">=3.9,<4"
 
 [tool.poetry.group.dev.dependencies]
 Jinja2 = ">=3.1.2"
 black = ">=22.10.0"
 coverage = ">=6.5.0"
 flake8 = ">=5.0.4"
 git-changelog = ">=2.2.0"
@@ -44,15 +44,14 @@
 pip-tools = ">=6.12.1"
 pre-commit = ">=2.20.0"
 pylint = ">=2.15.0"
 pytest = ">=7.2.0"
 pytest-benchmark = ">=4.0.0"
 pytest-xdist = ">=3.1.0"
 
-
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.black]
 target-version =  ["py39"]
 exclude = "venv/|tox/|protarrow_protos/.*"
```

### Comparing `protarrow-0.4.0/PKG-INFO` & `protarrow-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: protarrow
-Version: 0.4.0
+Version: 0.5.2
 Summary: Convert from protobuf to arrow and back
 Home-page: https://github.com/tradewelltech/protarrow
 License: Apache-2.0
 Keywords: apache-arrow,protobuf,data
 Author: Tradewell Tech
 Author-email: engineering@tradewelltech.co
 Maintainer: 0x26res
 Maintainer-email: 0x26res@gmail.com
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.9,<4
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: googleapis-common-protos (>=1.53.0)
-Requires-Dist: protobuf (>=3.20.1)
+Requires-Dist: protobuf (>=3.20.1,<5)
 Requires-Dist: pyarrow (>=12.0.0)
 Project-URL: Documentation, https://protarrow.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/tradewelltech/protarrow
 Description-Content-Type: text/markdown
 
 [![PyPI Version][pypi-image]][pypi-url]
 [![Python Version][versions-image]][versions-url]
@@ -36,15 +36,15 @@
 [![Downloads][downloads-month-image]][downloads-month-url]
 [![Code style: black][codestyle-image]][codestyle-url]
 [![snyk][snyk-image]][snyk-url]
 
 
 # Protarrow
 
-**Protarrow** is a python library for converting from protobuf to arrow and back.
+**Protarrow** is a python library for converting from Protocol Buffers to Apache Arrow and back.
 
 It is used at [Tradewell Technologies](https://www.tradewelltech.co/), 
 to share data between transactional and analytical applications,
 with little boilerplate code and zero data loss.
 
 # Installation
```

