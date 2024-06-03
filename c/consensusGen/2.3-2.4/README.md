# Comparing `tmp/consensusgen-2.3.tar.gz` & `tmp/consensusgen-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "consensusgen-2.3.tar", last modified: Mon Jun  3 13:28:37 2024, max compression
+gzip compressed data, was "consensusgen-2.4.tar", last modified: Mon Jun  3 13:35:03 2024, max compression
```

## Comparing `consensusgen-2.3.tar` & `consensusgen-2.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:28:37.507058 consensusgen-2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-06-03 13:28:13.000000 consensusgen-2.3/LICENCE.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:28:13.000000 consensusgen-2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-06-03 13:28:37.507058 consensusgen-2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-06-03 13:28:13.000000 consensusgen-2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:28:37.507058 consensusgen-2.3/consensusGen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-06-03 13:28:37.000000 consensusgen-2.3/consensusGen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-06-03 13:28:37.000000 consensusgen-2.3/consensusGen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 13:28:37.000000 consensusgen-2.3/consensusGen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-06-03 13:28:37.000000 consensusgen-2.3/consensusGen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-06-03 13:28:37.000000 consensusgen-2.3/consensusGen.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:28:37.507058 consensusgen-2.3/consensusgen/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-06-03 13:28:13.000000 consensusgen-2.3/consensusgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11295 2024-06-03 13:28:13.000000 consensusgen-2.3/consensusgen/consensusGen.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 13:28:37.507058 consensusgen-2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-06-03 13:28:13.000000 consensusgen-2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:35:03.955932 consensusgen-2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-06-03 13:34:47.000000 consensusgen-2.4/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:34:47.000000 consensusgen-2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-06-03 13:35:03.955932 consensusgen-2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-06-03 13:34:47.000000 consensusgen-2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:35:03.955932 consensusgen-2.4/consensusGen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-06-03 13:35:03.000000 consensusgen-2.4/consensusGen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-06-03 13:35:03.000000 consensusgen-2.4/consensusGen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 13:35:03.000000 consensusgen-2.4/consensusGen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-06-03 13:35:03.000000 consensusgen-2.4/consensusGen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-06-03 13:35:03.000000 consensusgen-2.4/consensusGen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:35:03.955932 consensusgen-2.4/consensusgen/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-06-03 13:34:47.000000 consensusgen-2.4/consensusgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11305 2024-06-03 13:34:47.000000 consensusgen-2.4/consensusgen/consensusGen.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 13:35:03.955932 consensusgen-2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-06-03 13:34:47.000000 consensusgen-2.4/setup.py
```

### Comparing `consensusgen-2.3/LICENCE.md` & `consensusgen-2.4/LICENCE.md`

 * *Files identical despite different names*

### Comparing `consensusgen-2.3/PKG-INFO` & `consensusgen-2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consensusGen
-Version: 2.3
+Version: 2.4
 Summary: Genetic algorithm for consensus building
 Home-page: https://pypi.org/project/consensusGen/
 Author: RomainCoulon (Romain Coulon)
 Author-email: <romain.coulon@bipm.org>
 Project-URL: Documentation, https://github.com/RomainCoulon/consensusGen/
 Keywords: genetic algorithm,inter-laboratory comparison,consenus building
 Classifier: Development Status :: 4 - Beta
```

### Comparing `consensusgen-2.3/consensusGen.egg-info/PKG-INFO` & `consensusgen-2.4/consensusGen.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consensusGen
-Version: 2.3
+Version: 2.4
 Summary: Genetic algorithm for consensus building
 Home-page: https://pypi.org/project/consensusGen/
 Author: RomainCoulon (Romain Coulon)
 Author-email: <romain.coulon@bipm.org>
 Project-URL: Documentation, https://github.com/RomainCoulon/consensusGen/
 Keywords: genetic algorithm,inter-laboratory comparison,consenus building
 Classifier: Development Status :: 4 - Beta
```

### Comparing `consensusgen-2.3/consensusgen/consensusGen.py` & `consensusgen-2.4/consensusgen/consensusGen.py`

 * *Files 1% similar despite different names*

```diff
@@ -321,13 +321,13 @@
         gen0 = gen1
         popSize0 = popSize
 
     return ref_val, unc_ref_val, phen00, phen1, weights, unc_weights
 
 
 # Example usage (replace with actual function call and data):
-l = ["A", "B", "C", "D", "E", "F", "G"]
-X = [10.1, 11, 14, 10, 10.5, 9.8, 5.1]
-u = [1, 1, 1, 2, 1, 1.5, 3]
-result = consensusGen(X, u, ng=3, ni=10000, threshold=1)
-displayResult(X, u, result, lab=l)
+# l = ["A", "B", "C", "D", "E", "F", "G"]
+# X = [10.1, 11, 14, 10, 10.5, 9.8, 5.1]
+# u = [1, 1, 1, 2, 1, 1.5, 3]
+# result = consensusGen(X, u, ng=3, ni=10000, threshold=1)
+# displayResult(X, u, result, lab=l)
```

### Comparing `consensusgen-2.3/setup.py` & `consensusgen-2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
 
-VERSION = "2.3"
+VERSION = "2.4"
 
 
 
 DESCRIPTION = "Genetic algorithm for consensus building"
 
 with open("README.md", "r") as f:
     long_description = f.read()
```

