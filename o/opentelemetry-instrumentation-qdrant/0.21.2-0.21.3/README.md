# Comparing `tmp/opentelemetry_instrumentation_qdrant-0.21.2.tar.gz` & `tmp/opentelemetry_instrumentation_qdrant-0.21.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentelemetry_instrumentation_qdrant-0.21.2.tar", max compression
+gzip compressed data, was "opentelemetry_instrumentation_qdrant-0.21.3.tar", max compression
```

## Comparing `opentelemetry_instrumentation_qdrant-0.21.2.tar` & `opentelemetry_instrumentation_qdrant-0.21.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      572 2024-05-31 18:54:20.359480 opentelemetry_instrumentation_qdrant-0.21.2/README.md
--rw-r--r--   0        0        0     2114 2024-05-31 18:54:20.359480 opentelemetry_instrumentation_qdrant-0.21.2/opentelemetry/instrumentation/qdrant/__init__.py
--rw-r--r--   0        0        0     2943 2024-05-31 18:54:20.359480 opentelemetry_instrumentation_qdrant-0.21.2/opentelemetry/instrumentation/qdrant/async_qdrant_client_methods.json
--rw-r--r--   0        0        0       42 2024-05-31 18:54:20.359480 opentelemetry_instrumentation_qdrant-0.21.2/opentelemetry/instrumentation/qdrant/config.py
--rw-r--r--   0        0        0     2828 2024-05-31 18:54:20.359480 opentelemetry_instrumentation_qdrant-0.21.2/opentelemetry/instrumentation/qdrant/qdrant_client_methods.json
--rw-r--r--   0        0        0      740 2024-05-31 18:54:20.359480 opentelemetry_instrumentation_qdrant-0.21.2/opentelemetry/instrumentation/qdrant/utils.py
--rw-r--r--   0        0        0       23 2024-05-31 18:54:20.359480 opentelemetry_instrumentation_qdrant-0.21.2/opentelemetry/instrumentation/qdrant/version.py
--rw-r--r--   0        0        0     3783 2024-05-31 18:54:20.359480 opentelemetry_instrumentation_qdrant-0.21.2/opentelemetry/instrumentation/qdrant/wrapper.py
--rw-r--r--   0        0        0     1352 2024-05-31 18:54:50.243362 opentelemetry_instrumentation_qdrant-0.21.2/pyproject.toml
--rw-r--r--   0        0        0     1655 1970-01-01 00:00:00.000000 opentelemetry_instrumentation_qdrant-0.21.2/PKG-INFO
+-rw-r--r--   0        0        0      572 2024-06-03 09:43:21.530364 opentelemetry_instrumentation_qdrant-0.21.3/README.md
+-rw-r--r--   0        0        0     2114 2024-06-03 09:43:21.534364 opentelemetry_instrumentation_qdrant-0.21.3/opentelemetry/instrumentation/qdrant/__init__.py
+-rw-r--r--   0        0        0     2943 2024-06-03 09:43:21.534364 opentelemetry_instrumentation_qdrant-0.21.3/opentelemetry/instrumentation/qdrant/async_qdrant_client_methods.json
+-rw-r--r--   0        0        0       42 2024-06-03 09:43:21.534364 opentelemetry_instrumentation_qdrant-0.21.3/opentelemetry/instrumentation/qdrant/config.py
+-rw-r--r--   0        0        0     2828 2024-06-03 09:43:21.534364 opentelemetry_instrumentation_qdrant-0.21.3/opentelemetry/instrumentation/qdrant/qdrant_client_methods.json
+-rw-r--r--   0        0        0      740 2024-06-03 09:43:21.534364 opentelemetry_instrumentation_qdrant-0.21.3/opentelemetry/instrumentation/qdrant/utils.py
+-rw-r--r--   0        0        0       23 2024-06-03 09:43:21.534364 opentelemetry_instrumentation_qdrant-0.21.3/opentelemetry/instrumentation/qdrant/version.py
+-rw-r--r--   0        0        0     3783 2024-06-03 09:43:21.534364 opentelemetry_instrumentation_qdrant-0.21.3/opentelemetry/instrumentation/qdrant/wrapper.py
+-rw-r--r--   0        0        0     1352 2024-06-03 09:43:46.406222 opentelemetry_instrumentation_qdrant-0.21.3/pyproject.toml
+-rw-r--r--   0        0        0     1655 1970-01-01 00:00:00.000000 opentelemetry_instrumentation_qdrant-0.21.3/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_qdrant-0.21.2/README.md` & `opentelemetry_instrumentation_qdrant-0.21.3/README.md`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_qdrant-0.21.2/opentelemetry/instrumentation/qdrant/__init__.py` & `opentelemetry_instrumentation_qdrant-0.21.3/opentelemetry/instrumentation/qdrant/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_qdrant-0.21.2/opentelemetry/instrumentation/qdrant/async_qdrant_client_methods.json` & `opentelemetry_instrumentation_qdrant-0.21.3/opentelemetry/instrumentation/qdrant/async_qdrant_client_methods.json`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_qdrant-0.21.2/opentelemetry/instrumentation/qdrant/qdrant_client_methods.json` & `opentelemetry_instrumentation_qdrant-0.21.3/opentelemetry/instrumentation/qdrant/qdrant_client_methods.json`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_qdrant-0.21.2/opentelemetry/instrumentation/qdrant/utils.py` & `opentelemetry_instrumentation_qdrant-0.21.3/opentelemetry/instrumentation/qdrant/utils.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_qdrant-0.21.2/opentelemetry/instrumentation/qdrant/wrapper.py` & `opentelemetry_instrumentation_qdrant-0.21.3/opentelemetry/instrumentation/qdrant/wrapper.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_qdrant-0.21.2/pyproject.toml` & `opentelemetry_instrumentation_qdrant-0.21.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.coverage.report]
 exclude_lines = [ "if TYPE_CHECKING:" ]
 show_missing = true
 
 [tool.poetry]
 name = "opentelemetry-instrumentation-qdrant"
-version = "0.21.2"
+version = "0.21.3"
 description = "OpenTelemetry Qdrant instrumentation"
 authors = [
   "Gal Kleinman <gal@traceloop.com>",
   "Nir Gazit <nir@traceloop.com>",
   "Tomer Friedman <tomer@traceloop.com>"
 ]
 repository = "https://github.com/traceloop/openllmetry/tree/main/packages/opentelemetry-instrumentation-qdrant"
```

### Comparing `opentelemetry_instrumentation_qdrant-0.21.2/PKG-INFO` & `opentelemetry_instrumentation_qdrant-0.21.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-qdrant
-Version: 0.21.2
+Version: 0.21.3
 Summary: OpenTelemetry Qdrant instrumentation
 Home-page: https://github.com/traceloop/openllmetry/tree/main/packages/opentelemetry-instrumentation-qdrant
 License: Apache-2.0
 Author: Gal Kleinman
 Author-email: gal@traceloop.com
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 Metadata-Version: 2.1 Name: opentelemetry-instrumentation-qdrant Version:
-0.21.2 Summary: OpenTelemetry Qdrant instrumentation Home-page: https://
+0.21.3 Summary: OpenTelemetry Qdrant instrumentation Home-page: https://
 github.com/traceloop/openllmetry/tree/main/packages/opentelemetry-
 instrumentation-qdrant License: Apache-2.0 Author: Gal Kleinman Author-email:
 gal@traceloop.com Requires-Python: >=3.9,<4 Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Provides-Extra: instruments
```

