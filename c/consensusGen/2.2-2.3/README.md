# Comparing `tmp/consensusgen-2.2.tar.gz` & `tmp/consensusgen-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "consensusgen-2.2.tar", last modified: Mon Jun  3 13:23:14 2024, max compression
+gzip compressed data, was "consensusgen-2.3.tar", last modified: Mon Jun  3 13:28:37 2024, max compression
```

## Comparing `consensusgen-2.2.tar` & `consensusgen-2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:23:14.383695 consensusgen-2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-06-03 13:22:58.000000 consensusgen-2.2/LICENCE.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:22:58.000000 consensusgen-2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-06-03 13:23:14.383695 consensusgen-2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-06-03 13:22:58.000000 consensusgen-2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:23:14.383695 consensusgen-2.2/consensusGen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-06-03 13:23:14.000000 consensusgen-2.2/consensusGen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-06-03 13:23:14.000000 consensusgen-2.2/consensusGen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 13:23:14.000000 consensusgen-2.2/consensusGen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-03 13:23:14.000000 consensusgen-2.2/consensusGen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-06-03 13:23:14.000000 consensusgen-2.2/consensusGen.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:23:14.383695 consensusgen-2.2/consensusgen/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-06-03 13:22:58.000000 consensusgen-2.2/consensusgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-06-03 13:22:58.000000 consensusgen-2.2/consensusgen/consensusGen.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 13:23:14.383695 consensusgen-2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-06-03 13:22:58.000000 consensusgen-2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:28:37.507058 consensusgen-2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-06-03 13:28:13.000000 consensusgen-2.3/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:28:13.000000 consensusgen-2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-06-03 13:28:37.507058 consensusgen-2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-06-03 13:28:13.000000 consensusgen-2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:28:37.507058 consensusgen-2.3/consensusGen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-06-03 13:28:37.000000 consensusgen-2.3/consensusGen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-06-03 13:28:37.000000 consensusgen-2.3/consensusGen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 13:28:37.000000 consensusgen-2.3/consensusGen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-06-03 13:28:37.000000 consensusgen-2.3/consensusGen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-06-03 13:28:37.000000 consensusgen-2.3/consensusGen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:28:37.507058 consensusgen-2.3/consensusgen/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-06-03 13:28:13.000000 consensusgen-2.3/consensusgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11295 2024-06-03 13:28:13.000000 consensusgen-2.3/consensusgen/consensusGen.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 13:28:37.507058 consensusgen-2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-06-03 13:28:13.000000 consensusgen-2.3/setup.py
```

### Comparing `consensusgen-2.2/LICENCE.md` & `consensusgen-2.3/LICENCE.md`

 * *Files identical despite different names*

### Comparing `consensusgen-2.2/PKG-INFO` & `consensusgen-2.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consensusGen
-Version: 2.2
+Version: 2.3
 Summary: Genetic algorithm for consensus building
 Home-page: https://pypi.org/project/consensusGen/
 Author: RomainCoulon (Romain Coulon)
 Author-email: <romain.coulon@bipm.org>
 Project-URL: Documentation, https://github.com/RomainCoulon/consensusGen/
 Keywords: genetic algorithm,inter-laboratory comparison,consenus building
 Classifier: Development Status :: 4 - Beta
@@ -17,15 +17,14 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Scientific/Engineering :: Physics
 Description-Content-Type: text/markdown
 License-File: LICENCE.md
 Requires-Dist: numpy
 Requires-Dist: matplotlib
-Requires-Dist: math
 
 # consensusGen
 
 `consensusGen.py` is a Python code implementing an genetic algorithm allowing to build a consensus value from measurement results of an inter-laboratory comparison. 
 
 Details are provided in [Romain Coulon and Steven Judge 2021 Metrologia 58 065007](https://doi.org/10.1088/1681-7575/ac31c0)
```

### Comparing `consensusgen-2.2/consensusGen.egg-info/PKG-INFO` & `consensusgen-2.3/consensusGen.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consensusGen
-Version: 2.2
+Version: 2.3
 Summary: Genetic algorithm for consensus building
 Home-page: https://pypi.org/project/consensusGen/
 Author: RomainCoulon (Romain Coulon)
 Author-email: <romain.coulon@bipm.org>
 Project-URL: Documentation, https://github.com/RomainCoulon/consensusGen/
 Keywords: genetic algorithm,inter-laboratory comparison,consenus building
 Classifier: Development Status :: 4 - Beta
@@ -17,15 +17,14 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Scientific/Engineering :: Physics
 Description-Content-Type: text/markdown
 License-File: LICENCE.md
 Requires-Dist: numpy
 Requires-Dist: matplotlib
-Requires-Dist: math
 
 # consensusGen
 
 `consensusGen.py` is a Python code implementing an genetic algorithm allowing to build a consensus value from measurement results of an inter-laboratory comparison. 
 
 Details are provided in [Romain Coulon and Steven Judge 2021 Metrologia 58 065007](https://doi.org/10.1088/1681-7575/ac31c0)
```

### Comparing `consensusgen-2.2/consensusgen/consensusGen.py` & `consensusgen-2.3/consensusgen/consensusGen.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 @author: romain.coulon
 """
 
 import numpy as np
 import matplotlib.pyplot as plt
 from collections import Counter
-import math
 
 def cosine_similarity(seq1, seq2):
     
     freq1 = Counter(seq1)
     freq2 = Counter(seq2)
     
     # Get the set of all unique genes
@@ -22,16 +21,16 @@
     vec1 = [freq1.get(gene, 0) for gene in genes]
     vec2 = [freq2.get(gene, 0) for gene in genes]
     
     # Calculate dot product
     dot_product = sum(v1 * v2 for v1, v2 in zip(vec1, vec2))
     
     # Calculate magnitudes
-    magnitude1 = math.sqrt(sum(v1 ** 2 for v1 in vec1))
-    magnitude2 = math.sqrt(sum(v2 ** 2 for v2 in vec2))
+    magnitude1 = np.sqrt(sum(v1 ** 2 for v1 in vec1))
+    magnitude2 = np.sqrt(sum(v2 ** 2 for v2 in vec2))
     
     if not magnitude1 or not magnitude2:
         return 0.0
     
     # Calculate cosine similarity
     return dot_product / (magnitude1 * magnitude2)
 
@@ -322,13 +321,13 @@
         gen0 = gen1
         popSize0 = popSize
 
     return ref_val, unc_ref_val, phen00, phen1, weights, unc_weights
 
 
 # Example usage (replace with actual function call and data):
-# l = ["A", "B", "C", "D", "E", "F", "G"]
-# X = [10.1, 11, 14, 10, 10.5, 9.8, 5.1]
-# u = [1, 1, 1, 2, 1, 1.5, 3]
-# result = consensusGen(X, u, ng=3, ni=10000, threshold=1)
-# displayResult(X, u, result, lab=l)
+l = ["A", "B", "C", "D", "E", "F", "G"]
+X = [10.1, 11, 14, 10, 10.5, 9.8, 5.1]
+u = [1, 1, 1, 2, 1, 1.5, 3]
+result = consensusGen(X, u, ng=3, ni=10000, threshold=1)
+displayResult(X, u, result, lab=l)
```

### Comparing `consensusgen-2.2/setup.py` & `consensusgen-2.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = "2.2"
+
+VERSION = "2.3"
+
 
 
 DESCRIPTION = "Genetic algorithm for consensus building"
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
@@ -19,15 +21,15 @@
     description = DESCRIPTION,
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://pypi.org/project/consensusGen/",
     py_modules=['consensusGen'], 
     project_urls={'Documentation': 'https://github.com/RomainCoulon/consensusGen/',},
     packages = find_packages(),
-    install_requires = ["numpy","matplotlib","math"],
+    install_requires = ["numpy","matplotlib"],
     keywords = ["genetic algorithm","inter-laboratory comparison","consenus building"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Natural Language :: French",
```

