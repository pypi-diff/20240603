# Comparing `tmp/quotesgeneratorapi_wrapper-0.4.0.tar.gz` & `tmp/quotesgeneratorapi_wrapper-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quotesgeneratorapi_wrapper-0.4.0.tar", max compression
+gzip compressed data, was "quotesgeneratorapi_wrapper-0.5.0.tar", max compression
```

## Comparing `quotesgeneratorapi_wrapper-0.4.0.tar` & `quotesgeneratorapi_wrapper-0.5.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1080 2024-03-05 18:28:23.204977 quotesgeneratorapi_wrapper-0.4.0/LICENSE
--rw-r--r--   0        0        0       57 2024-04-24 21:09:15.061957 quotesgeneratorapi_wrapper-0.4.0/README.md
--rw-r--r--   0        0        0      373 2024-04-24 21:11:18.098693 quotesgeneratorapi_wrapper-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-14 20:50:25.840847 quotesgeneratorapi_wrapper-0.4.0/quotesgeneratorapi_wrapper/__init__.py
--rw-r--r--   0        0        0      491 2024-04-14 21:21:56.700740 quotesgeneratorapi_wrapper-0.4.0/quotesgeneratorapi_wrapper/quotesgenerator.py
--rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 quotesgeneratorapi_wrapper-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-03-05 18:28:23.204977 quotesgeneratorapi_wrapper-0.5.0/LICENSE
+-rw-r--r--   0        0        0       58 2024-04-24 21:12:13.761678 quotesgeneratorapi_wrapper-0.5.0/README.md
+-rw-r--r--   0        0        0      373 2024-04-24 21:12:20.057579 quotesgeneratorapi_wrapper-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-14 20:50:25.840847 quotesgeneratorapi_wrapper-0.5.0/quotesgeneratorapi_wrapper/__init__.py
+-rw-r--r--   0        0        0      491 2024-04-14 21:21:56.700740 quotesgeneratorapi_wrapper-0.5.0/quotesgeneratorapi_wrapper/quotesgenerator.py
+-rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 quotesgeneratorapi_wrapper-0.5.0/PKG-INFO
```

### Comparing `quotesgeneratorapi_wrapper-0.4.0/LICENSE` & `quotesgeneratorapi_wrapper-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quotesgeneratorapi_wrapper-0.4.0/PKG-INFO` & `quotesgeneratorapi_wrapper-0.5.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quotesgeneratorapi-wrapper
-Version: 0.4.0
+Version: 0.5.0
 Summary: A wrapper for quotes from API Ninjas
 License: MIT
 Author: tct123
 Author-email: 42028373+tct123@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,8 +13,8 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Quotesgeneratorapi
-A wrapper for quotes from API Ninjas
+A wrapper for quotes from API Ninjas.
```

