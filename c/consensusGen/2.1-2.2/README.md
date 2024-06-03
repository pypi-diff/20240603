# Comparing `tmp/consensusgen-2.1.tar.gz` & `tmp/consensusgen-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "consensusgen-2.1.tar", last modified: Mon Jun  3 13:02:52 2024, max compression
+gzip compressed data, was "consensusgen-2.2.tar", last modified: Mon Jun  3 13:23:14 2024, max compression
```

## Comparing `consensusgen-2.1.tar` & `consensusgen-2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:02:52.052130 consensusgen-2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-06-03 13:02:30.000000 consensusgen-2.1/LICENCE.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:02:30.000000 consensusgen-2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-06-03 13:02:52.048130 consensusgen-2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-06-03 13:02:30.000000 consensusgen-2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:02:52.048130 consensusgen-2.1/consensusGen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-06-03 13:02:52.000000 consensusgen-2.1/consensusGen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-06-03 13:02:52.000000 consensusgen-2.1/consensusGen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 13:02:52.000000 consensusgen-2.1/consensusGen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-03 13:02:52.000000 consensusgen-2.1/consensusGen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-06-03 13:02:52.000000 consensusgen-2.1/consensusGen.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:02:52.048130 consensusgen-2.1/consensusgen/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 13:02:30.000000 consensusgen-2.1/consensusgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-06-03 13:02:30.000000 consensusgen-2.1/consensusgen/consensusGen.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 13:02:52.052130 consensusgen-2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-06-03 13:02:30.000000 consensusgen-2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:23:14.383695 consensusgen-2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-06-03 13:22:58.000000 consensusgen-2.2/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:22:58.000000 consensusgen-2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-06-03 13:23:14.383695 consensusgen-2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-06-03 13:22:58.000000 consensusgen-2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:23:14.383695 consensusgen-2.2/consensusGen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-06-03 13:23:14.000000 consensusgen-2.2/consensusGen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-06-03 13:23:14.000000 consensusgen-2.2/consensusGen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 13:23:14.000000 consensusgen-2.2/consensusGen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-03 13:23:14.000000 consensusgen-2.2/consensusGen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-06-03 13:23:14.000000 consensusgen-2.2/consensusGen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:23:14.383695 consensusgen-2.2/consensusgen/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-06-03 13:22:58.000000 consensusgen-2.2/consensusgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-06-03 13:22:58.000000 consensusgen-2.2/consensusgen/consensusGen.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 13:23:14.383695 consensusgen-2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-06-03 13:22:58.000000 consensusgen-2.2/setup.py
```

### Comparing `consensusgen-2.1/LICENCE.md` & `consensusgen-2.2/LICENCE.md`

 * *Files identical despite different names*

### Comparing `consensusgen-2.1/PKG-INFO` & `consensusgen-2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consensusGen
-Version: 2.1
+Version: 2.2
 Summary: Genetic algorithm for consensus building
 Home-page: https://pypi.org/project/consensusGen/
 Author: RomainCoulon (Romain Coulon)
 Author-email: <romain.coulon@bipm.org>
 Project-URL: Documentation, https://github.com/RomainCoulon/consensusGen/
 Keywords: genetic algorithm,inter-laboratory comparison,consenus building
 Classifier: Development Status :: 4 - Beta
```

### Comparing `consensusgen-2.1/consensusGen.egg-info/PKG-INFO` & `consensusgen-2.2/consensusGen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consensusGen
-Version: 2.1
+Version: 2.2
 Summary: Genetic algorithm for consensus building
 Home-page: https://pypi.org/project/consensusGen/
 Author: RomainCoulon (Romain Coulon)
 Author-email: <romain.coulon@bipm.org>
 Project-URL: Documentation, https://github.com/RomainCoulon/consensusGen/
 Keywords: genetic algorithm,inter-laboratory comparison,consenus building
 Classifier: Development Status :: 4 - Beta
```

### Comparing `consensusgen-2.1/consensusgen/consensusGen.py` & `consensusgen-2.2/consensusgen/consensusGen.py`

 * *Files identical despite different names*

### Comparing `consensusgen-2.1/setup.py` & `consensusgen-2.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = "2.1"
+VERSION = "2.2"
 
 
 DESCRIPTION = "Genetic algorithm for consensus building"
 
 with open("README.md", "r") as f:
     long_description = f.read()
```

