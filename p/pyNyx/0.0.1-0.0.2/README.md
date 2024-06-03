# Comparing `tmp/pynyx-0.0.1.tar.gz` & `tmp/pynyx-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynyx-0.0.1.tar", max compression
+gzip compressed data, was "pynyx-0.0.2.tar", max compression
```

## Comparing `pynyx-0.0.1.tar` & `pynyx-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       69 2024-06-03 14:31:01.095731 pynyx-0.0.1/README.md
--rw-r--r--   0        0        0     1090 2024-06-03 13:31:48.166409 pynyx-0.0.1/nyx/cli.py
--rw-r--r--   0        0        0      113 2024-06-02 14:05:00.737983 pynyx-0.0.1/nyx/exceptions.py
--rw-r--r--   0        0        0      869 2024-06-03 14:39:42.638142 pynyx-0.0.1/nyx/main.py
--rw-r--r--   0        0        0     8430 2024-06-03 13:32:23.694684 pynyx-0.0.1/nyx/model.py
--rw-r--r--   0        0        0      381 2024-06-03 14:43:09.745219 pynyx-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      600 1970-01-01 00:00:00.000000 pynyx-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       69 2024-06-03 14:31:01.095731 pynyx-0.0.2/README.md
+-rw-r--r--   0        0        0     1090 2024-06-03 13:31:48.166409 pynyx-0.0.2/nyx/cli.py
+-rw-r--r--   0        0        0      113 2024-06-02 14:05:00.737983 pynyx-0.0.2/nyx/exceptions.py
+-rw-r--r--   0        0        0      869 2024-06-03 14:39:42.638142 pynyx-0.0.2/nyx/main.py
+-rw-r--r--   0        0        0     8430 2024-06-03 13:32:23.694684 pynyx-0.0.2/nyx/model.py
+-rw-r--r--   0        0        0      432 2024-06-03 15:04:13.928551 pynyx-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      600 1970-01-01 00:00:00.000000 pynyx-0.0.2/PKG-INFO
```

### Comparing `pynyx-0.0.1/nyx/cli.py` & `pynyx-0.0.2/nyx/cli.py`

 * *Files identical despite different names*

### Comparing `pynyx-0.0.1/nyx/main.py` & `pynyx-0.0.2/nyx/main.py`

 * *Files identical despite different names*

### Comparing `pynyx-0.0.1/nyx/model.py` & `pynyx-0.0.2/nyx/model.py`

 * *Files identical despite different names*

### Comparing `pynyx-0.0.1/PKG-INFO` & `pynyx-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyNyx
-Version: 0.0.1
+Version: 0.0.2
 Summary: nyx rules processing and conversion tools
 License: MIT
 Author: arblade
 Author-email: raphael.arblade@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

