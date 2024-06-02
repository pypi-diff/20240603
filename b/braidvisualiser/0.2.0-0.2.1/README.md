# Comparing `tmp/braidvisualiser-0.2.0.tar.gz` & `tmp/braidvisualiser-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "braidvisualiser-0.2.0.tar", max compression
+gzip compressed data, was "braidvisualiser-0.2.1.tar", max compression
```

## Comparing `braidvisualiser-0.2.0.tar` & `braidvisualiser-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1072 2024-01-12 22:50:15.558573 braidvisualiser-0.2.0/LICENSE
--rw-r--r--   0        0        0      421 2024-01-12 22:50:15.558573 braidvisualiser-0.2.0/README.md
--rw-r--r--   0        0        0      486 2024-01-12 22:50:15.558573 braidvisualiser-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       29 2024-01-12 22:50:15.558573 braidvisualiser-0.2.0/src/braidvisualiser/__init__.py
--rw-r--r--   0        0        0     7048 2024-01-12 22:50:15.558573 braidvisualiser-0.2.0/src/braidvisualiser/braid.py
--rw-r--r--   0        0        0     1015 1970-01-01 00:00:00.000000 braidvisualiser-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-06-02 23:15:44.324566 braidvisualiser-0.2.1/LICENSE
+-rw-r--r--   0        0        0      421 2024-06-02 23:15:44.324566 braidvisualiser-0.2.1/README.md
+-rw-r--r--   0        0        0      486 2024-06-02 23:15:44.324566 braidvisualiser-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       29 2024-06-02 23:15:44.324566 braidvisualiser-0.2.1/src/braidvisualiser/__init__.py
+-rw-r--r--   0        0        0     7048 2024-06-02 23:15:44.324566 braidvisualiser-0.2.1/src/braidvisualiser/braid.py
+-rw-r--r--   0        0        0     1015 1970-01-01 00:00:00.000000 braidvisualiser-0.2.1/PKG-INFO
```

### Comparing `braidvisualiser-0.2.0/LICENSE` & `braidvisualiser-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `braidvisualiser-0.2.0/src/braidvisualiser/braid.py` & `braidvisualiser-0.2.1/src/braidvisualiser/braid.py`

 * *Files identical despite different names*

### Comparing `braidvisualiser-0.2.0/PKG-INFO` & `braidvisualiser-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: braidvisualiser
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python library providing functionality for the creation and rendering of Artin braids.
 License: MIT
 Author: Rex Greenway
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

