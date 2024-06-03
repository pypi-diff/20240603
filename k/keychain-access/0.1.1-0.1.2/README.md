# Comparing `tmp/keychain_access-0.1.1.tar.gz` & `tmp/keychain_access-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keychain_access-0.1.1.tar", max compression
+gzip compressed data, was "keychain_access-0.1.2.tar", max compression
```

## Comparing `keychain_access-0.1.1.tar` & `keychain_access-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0      623 2024-05-23 05:34:10.620797 keychain_access-0.1.1/README.md
--rw-r--r--   0        0        0      451 2024-05-23 05:34:10.621000 keychain_access-0.1.1/keychain_access/__init__.py
--rw-r--r--   0        0        0     3119 2024-05-23 05:34:10.621263 keychain_access-0.1.1/keychain_access/core.py
--rw-r--r--   0        0        0      127 2024-05-23 05:34:10.621755 keychain_access-0.1.1/keychain_access/exceptions.py
--rw-r--r--   0        0        0        0 2024-05-23 05:34:10.621905 keychain_access-0.1.1/keychain_access/tests/__init__.py
--rw-r--r--   0        0        0     1095 2024-05-23 05:34:10.622105 keychain_access-0.1.1/keychain_access/tests/test_core.py
--rw-r--r--   0        0        0      876 2024-05-23 05:34:10.622659 keychain_access-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1256 1970-01-01 00:00:00.000000 keychain_access-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      623 2024-06-03 15:22:12.489427 keychain_access-0.1.2/README.md
+-rw-r--r--   0        0        0      451 2024-06-03 15:22:12.489579 keychain_access-0.1.2/keychain_access/__init__.py
+-rw-r--r--   0        0        0     3119 2024-06-03 15:22:12.489712 keychain_access-0.1.2/keychain_access/core.py
+-rw-r--r--   0        0        0      127 2024-06-03 15:22:12.489819 keychain_access-0.1.2/keychain_access/exceptions.py
+-rw-r--r--   0        0        0        0 2024-06-03 15:22:12.489870 keychain_access-0.1.2/keychain_access/py.typed
+-rw-r--r--   0        0        0        0 2024-06-03 15:22:12.489964 keychain_access-0.1.2/keychain_access/tests/__init__.py
+-rw-r--r--   0        0        0     1095 2024-06-03 15:22:12.490086 keychain_access-0.1.2/keychain_access/tests/test_core.py
+-rw-r--r--   0        0        0      915 2024-06-03 15:22:12.491068 keychain_access-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1256 1970-01-01 00:00:00.000000 keychain_access-0.1.2/PKG-INFO
```

### Comparing `keychain_access-0.1.1/README.md` & `keychain_access-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `keychain_access-0.1.1/keychain_access/core.py` & `keychain_access-0.1.2/keychain_access/core.py`

 * *Files identical despite different names*

### Comparing `keychain_access-0.1.1/keychain_access/tests/test_core.py` & `keychain_access-0.1.2/keychain_access/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `keychain_access-0.1.1/pyproject.toml` & `keychain_access-0.1.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "keychain-access"
-version = "0.1.1"
+version = "0.1.2"
 description = "Access to the OSX Keychain API in Python."
 authors = ["Max Muoto <maxmuoto@gmail.com>"]
 readme = "README.md"
 license = "MIT"
+include = ["keychain_access/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pyobjc = "^10.2"
 
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `keychain_access-0.1.1/PKG-INFO` & `keychain_access-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keychain-access
-Version: 0.1.1
+Version: 0.1.2
 Summary: Access to the OSX Keychain API in Python.
 License: MIT
 Author: Max Muoto
 Author-email: maxmuoto@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

