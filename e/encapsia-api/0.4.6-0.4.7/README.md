# Comparing `tmp/encapsia_api-0.4.6.tar.gz` & `tmp/encapsia_api-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encapsia_api-0.4.6.tar", max compression
+gzip compressed data, was "encapsia_api-0.4.7.tar", max compression
```

## Comparing `encapsia_api-0.4.6.tar` & `encapsia_api-0.4.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1078 2022-01-07 06:44:29.651749 encapsia_api-0.4.6/LICENSE
--rw-r--r--   0        0        0     2863 2023-05-05 07:11:44.945138 encapsia_api-0.4.6/README.md
--rw-r--r--   0        0        0      595 2024-04-01 09:06:52.985905 encapsia_api-0.4.6/encapsia_api/__init__.py
--rw-r--r--   0        0        0     1877 2024-04-01 09:01:54.171375 encapsia_api-0.4.6/encapsia_api/analytics.py
--rw-r--r--   0        0        0     2858 2024-04-01 09:01:54.171375 encapsia_api-0.4.6/encapsia_api/credentials.py
--rw-r--r--   0        0        0     3035 2024-04-01 09:16:18.078304 encapsia_api-0.4.6/encapsia_api/lib.py
--rw-r--r--   0        0        0     6254 2024-04-01 09:05:22.241159 encapsia_api-0.4.6/encapsia_api/package.py
--rw-r--r--   0        0        0     3406 2024-04-01 09:05:22.185158 encapsia_api-0.4.6/encapsia_api/plugin.py
--rw-r--r--   0        0        0        0 2023-10-13 07:21:41.780961 encapsia_api-0.4.6/encapsia_api/py.typed
--rw-r--r--   0        0        0     3987 2024-04-01 09:01:54.171375 encapsia_api-0.4.6/encapsia_api/resilient_request.py
--rw-r--r--   0        0        0    33035 2024-04-01 09:28:35.087754 encapsia_api-0.4.6/encapsia_api/rest.py
--rw-r--r--   0        0        0        0 2023-10-13 07:21:41.780961 encapsia_api-0.4.6/encapsia_api/tests/__init__.py
--rw-r--r--   0        0        0     3516 2023-05-05 07:11:44.949138 encapsia_api-0.4.6/encapsia_api/tests/test_credentials.py
--rw-r--r--   0        0        0     6432 2024-04-01 09:32:49.605609 encapsia_api-0.4.6/encapsia_api/tests/test_package.py
--rw-r--r--   0        0        0      536 2023-05-05 07:11:44.949138 encapsia_api-0.4.6/encapsia_api/tests/test_plugin.py
--rw-r--r--   0        0        0     9154 2024-04-01 09:01:54.171375 encapsia_api-0.4.6/encapsia_api/tests/test_resilient_request.py
--rw-r--r--   0        0        0     7067 2024-04-01 09:34:17.498249 encapsia_api-0.4.6/encapsia_api/tests/test_rest.py
--rw-r--r--   0        0        0      566 2024-04-01 09:01:54.171375 encapsia_api-0.4.6/encapsia_api/util.py
--rw-r--r--   0        0        0     3509 2024-04-01 09:18:05.279109 encapsia_api-0.4.6/pyproject.toml
--rw-r--r--   0        0        0     3760 1970-01-01 00:00:00.000000 encapsia_api-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0     1078 2022-01-07 06:44:29.651749 encapsia_api-0.4.7/LICENSE
+-rw-r--r--   0        0        0     2863 2023-05-05 07:11:44.945138 encapsia_api-0.4.7/README.md
+-rw-r--r--   0        0        0      595 2024-06-03 09:20:11.058783 encapsia_api-0.4.7/encapsia_api/__init__.py
+-rw-r--r--   0        0        0     1877 2024-04-01 09:01:54.171375 encapsia_api-0.4.7/encapsia_api/analytics.py
+-rw-r--r--   0        0        0     2858 2024-04-01 09:01:54.171375 encapsia_api-0.4.7/encapsia_api/credentials.py
+-rw-r--r--   0        0        0     3035 2024-04-01 09:16:18.078304 encapsia_api-0.4.7/encapsia_api/lib.py
+-rw-r--r--   0        0        0     6254 2024-04-01 09:05:22.241159 encapsia_api-0.4.7/encapsia_api/package.py
+-rw-r--r--   0        0        0     3406 2024-04-01 09:05:22.185158 encapsia_api-0.4.7/encapsia_api/plugin.py
+-rw-r--r--   0        0        0        0 2023-10-13 07:21:41.780961 encapsia_api-0.4.7/encapsia_api/py.typed
+-rw-r--r--   0        0        0     3987 2024-04-01 09:01:54.171375 encapsia_api-0.4.7/encapsia_api/resilient_request.py
+-rw-r--r--   0        0        0    33035 2024-04-01 09:28:35.087754 encapsia_api-0.4.7/encapsia_api/rest.py
+-rw-r--r--   0        0        0        0 2023-10-13 07:21:41.780961 encapsia_api-0.4.7/encapsia_api/tests/__init__.py
+-rw-r--r--   0        0        0     3516 2023-05-05 07:11:44.949138 encapsia_api-0.4.7/encapsia_api/tests/test_credentials.py
+-rw-r--r--   0        0        0     6432 2024-04-01 09:32:49.605609 encapsia_api-0.4.7/encapsia_api/tests/test_package.py
+-rw-r--r--   0        0        0      536 2023-05-05 07:11:44.949138 encapsia_api-0.4.7/encapsia_api/tests/test_plugin.py
+-rw-r--r--   0        0        0     9154 2024-04-01 09:01:54.171375 encapsia_api-0.4.7/encapsia_api/tests/test_resilient_request.py
+-rw-r--r--   0        0        0     7067 2024-04-01 09:34:17.498249 encapsia_api-0.4.7/encapsia_api/tests/test_rest.py
+-rw-r--r--   0        0        0      566 2024-04-01 09:01:54.171375 encapsia_api-0.4.7/encapsia_api/util.py
+-rw-r--r--   0        0        0     3509 2024-06-03 09:19:51.358821 encapsia_api-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0     3760 1970-01-01 00:00:00.000000 encapsia_api-0.4.7/PKG-INFO
```

### Comparing `encapsia_api-0.4.6/LICENSE` & `encapsia_api-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.6/README.md` & `encapsia_api-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.6/encapsia_api/__init__.py` & `encapsia_api-0.4.7/encapsia_api/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #: Keep in sync with git tag and package version in pyproject.toml.
-__version__ = "0.4.6"
+__version__ = "0.4.7"
 
 
 class EncapsiaApiError(RuntimeError):
     def __init__(self, message, payload=None):
         super().__init__(message)
         self.message = message
         self.payload = payload
```

### Comparing `encapsia_api-0.4.6/encapsia_api/analytics.py` & `encapsia_api-0.4.7/encapsia_api/analytics.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.6/encapsia_api/credentials.py` & `encapsia_api-0.4.7/encapsia_api/credentials.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.6/encapsia_api/lib.py` & `encapsia_api-0.4.7/encapsia_api/lib.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.6/encapsia_api/package.py` & `encapsia_api-0.4.7/encapsia_api/package.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.6/encapsia_api/plugin.py` & `encapsia_api-0.4.7/encapsia_api/plugin.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.6/encapsia_api/resilient_request.py` & `encapsia_api-0.4.7/encapsia_api/resilient_request.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.6/encapsia_api/rest.py` & `encapsia_api-0.4.7/encapsia_api/rest.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.6/encapsia_api/tests/test_credentials.py` & `encapsia_api-0.4.7/encapsia_api/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.6/encapsia_api/tests/test_package.py` & `encapsia_api-0.4.7/encapsia_api/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.6/encapsia_api/tests/test_plugin.py` & `encapsia_api-0.4.7/encapsia_api/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.6/encapsia_api/tests/test_resilient_request.py` & `encapsia_api-0.4.7/encapsia_api/tests/test_resilient_request.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.6/encapsia_api/tests/test_rest.py` & `encapsia_api-0.4.7/encapsia_api/tests/test_rest.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.6/encapsia_api/util.py` & `encapsia_api-0.4.7/encapsia_api/util.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.6/pyproject.toml` & `encapsia_api-0.4.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "encapsia-api"
-version = "0.4.6"
+version = "0.4.7"
 description = "Client API for talking to an Encapsia system."
 readme = "README.md"
 authors = ["Timothy Corbett-Clark <timothy.corbettclark@gmail.com>"]
 maintainers = ["Petre Mierluțiu <petre.mierlutiu@aixial.com>"]
 license = "MIT"
 keywords = ["encapsia", "eSource", "EDC", "Clinical Trials"]
 homepage = "https://github.com/Encapsia/encapsia-api"
```

### Comparing `encapsia_api-0.4.6/PKG-INFO` & `encapsia_api-0.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encapsia-api
-Version: 0.4.6
+Version: 0.4.7
 Summary: Client API for talking to an Encapsia system.
 Home-page: https://github.com/Encapsia/encapsia-api
 License: MIT
 Keywords: encapsia,eSource,EDC,Clinical Trials
 Author: Timothy Corbett-Clark
 Author-email: timothy.corbettclark@gmail.com
 Maintainer: Petre Mierluțiu
```

