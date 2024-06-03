# Comparing `tmp/morphdb_utils-0.2.2.tar.gz` & `tmp/morphdb_utils-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morphdb_utils-0.2.2.tar", max compression
+gzip compressed data, was "morphdb_utils-0.2.3.tar", max compression
```

## Comparing `morphdb_utils-0.2.2.tar` & `morphdb_utils-0.2.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      777 2024-06-03 04:58:03.705605 morphdb_utils-0.2.2/README.md
--rw-r--r--   0        0        0        0 2024-05-02 05:57:33.264458 morphdb_utils-0.2.2/morphdb_utils/__init__.py
--rw-r--r--   0        0        0     3969 2024-06-03 04:53:18.220528 morphdb_utils-0.2.2/morphdb_utils/annotations.py
--rw-r--r--   0        0        0    14710 2024-05-29 09:08:49.283069 morphdb_utils-0.2.2/morphdb_utils/api.py
--rw-r--r--   0        0        0      429 2024-05-28 08:55:19.783177 morphdb_utils-0.2.2/morphdb_utils/logging.py
--rw-r--r--   0        0        0        0 2024-05-02 05:57:33.265042 morphdb_utils-0.2.2/morphdb_utils/py.typed
--rw-r--r--   0        0        0     1766 2024-05-29 09:08:48.461741 morphdb_utils-0.2.2/morphdb_utils/type.py
--rw-r--r--   0        0        0      824 2024-06-03 04:58:18.788325 morphdb_utils-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1467 1970-01-01 00:00:00.000000 morphdb_utils-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      777 2024-06-03 04:58:03.705605 morphdb_utils-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-02 05:57:33.264458 morphdb_utils-0.2.3/morphdb_utils/__init__.py
+-rw-r--r--   0        0        0     3969 2024-06-03 04:53:18.220528 morphdb_utils-0.2.3/morphdb_utils/annotations.py
+-rw-r--r--   0        0        0    14710 2024-05-29 09:08:49.283069 morphdb_utils-0.2.3/morphdb_utils/api.py
+-rw-r--r--   0        0        0      429 2024-05-28 08:55:19.783177 morphdb_utils-0.2.3/morphdb_utils/logging.py
+-rw-r--r--   0        0        0        0 2024-05-02 05:57:33.265042 morphdb_utils-0.2.3/morphdb_utils/py.typed
+-rw-r--r--   0        0        0     1766 2024-05-29 09:08:48.461741 morphdb_utils-0.2.3/morphdb_utils/type.py
+-rw-r--r--   0        0        0      824 2024-06-03 05:03:35.330395 morphdb_utils-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1467 1970-01-01 00:00:00.000000 morphdb_utils-0.2.3/PKG-INFO
```

### Comparing `morphdb_utils-0.2.2/README.md` & `morphdb_utils-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `morphdb_utils-0.2.2/morphdb_utils/annotations.py` & `morphdb_utils-0.2.3/morphdb_utils/annotations.py`

 * *Files identical despite different names*

### Comparing `morphdb_utils-0.2.2/morphdb_utils/api.py` & `morphdb_utils-0.2.3/morphdb_utils/api.py`

 * *Files identical despite different names*

### Comparing `morphdb_utils-0.2.2/morphdb_utils/type.py` & `morphdb_utils-0.2.3/morphdb_utils/type.py`

 * *Files identical despite different names*

### Comparing `morphdb_utils-0.2.2/pyproject.toml` & `morphdb_utils-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "morphdb-utils"
-version = "0.2.2"
+version = "0.2.3"
 description = ""
 authors = ["shibatanaoto <naoto.shibata510@gmail.com>"]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `morphdb_utils-0.2.2/PKG-INFO` & `morphdb_utils-0.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morphdb-utils
-Version: 0.2.2
+Version: 0.2.3
 Summary: 
 Author: shibatanaoto
 Author-email: naoto.shibata510@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

