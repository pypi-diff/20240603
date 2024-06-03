# Comparing `tmp/bwalign-1.0.2.tar.gz` & `tmp/bwalign-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bwalign-1.0.2.tar", last modified: Mon Jun  3 01:04:56 2024, max compression
+gzip compressed data, was "bwalign-1.0.3.tar", last modified: Mon Jun  3 01:08:57 2024, max compression
```

## Comparing `bwalign-1.0.2.tar` & `bwalign-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 01:04:55.999750 bwalign-1.0.2/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      914 2024-06-03 01:04:55.998833 bwalign-1.0.2/PKG-INFO
--rw-r--r--   0 adrianlayer   (501) staff       (20)     1744 2024-05-29 18:41:22.000000 bwalign-1.0.2/README.md
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 01:04:55.988659 bwalign-1.0.2/bwalign/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      142 2024-06-03 01:03:34.000000 bwalign-1.0.2/bwalign/__init__.py
--rw-r--r--   0 adrianlayer   (501) staff       (20)     2082 2024-06-03 01:02:47.000000 bwalign-1.0.2/bwalign/main.py
--rw-r--r--   0 adrianlayer   (501) staff       (20)    20539 2024-06-03 00:56:50.000000 bwalign-1.0.2/bwalign/utils.py
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 01:04:55.996709 bwalign-1.0.2/bwalign.egg-info/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      914 2024-06-03 01:04:55.000000 bwalign-1.0.2/bwalign.egg-info/PKG-INFO
--rw-r--r--   0 adrianlayer   (501) staff       (20)      259 2024-06-03 01:04:55.000000 bwalign-1.0.2/bwalign.egg-info/SOURCES.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)        1 2024-06-03 01:04:55.000000 bwalign-1.0.2/bwalign.egg-info/dependency_links.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       46 2024-06-03 01:04:55.000000 bwalign-1.0.2/bwalign.egg-info/entry_points.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       16 2024-06-03 01:04:55.000000 bwalign-1.0.2/bwalign.egg-info/requires.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)        8 2024-06-03 01:04:55.000000 bwalign-1.0.2/bwalign.egg-info/top_level.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       38 2024-06-03 01:04:56.002013 bwalign-1.0.2/setup.cfg
--rw-r--r--   0 adrianlayer   (501) staff       (20)     1194 2024-06-03 01:03:39.000000 bwalign-1.0.2/setup.py
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 01:08:57.129530 bwalign-1.0.3/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      914 2024-06-03 01:08:57.128289 bwalign-1.0.3/PKG-INFO
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     1744 2024-05-29 18:41:22.000000 bwalign-1.0.3/README.md
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 01:08:57.102749 bwalign-1.0.3/bwalign/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      142 2024-06-03 01:08:15.000000 bwalign-1.0.3/bwalign/__init__.py
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     2083 2024-06-03 01:07:06.000000 bwalign-1.0.3/bwalign/main.py
+-rw-r--r--   0 adrianlayer   (501) staff       (20)    20539 2024-06-03 00:56:50.000000 bwalign-1.0.3/bwalign/utils.py
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 01:08:57.126425 bwalign-1.0.3/bwalign.egg-info/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      914 2024-06-03 01:08:56.000000 bwalign-1.0.3/bwalign.egg-info/PKG-INFO
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      259 2024-06-03 01:08:56.000000 bwalign-1.0.3/bwalign.egg-info/SOURCES.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)        1 2024-06-03 01:08:56.000000 bwalign-1.0.3/bwalign.egg-info/dependency_links.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       46 2024-06-03 01:08:56.000000 bwalign-1.0.3/bwalign.egg-info/entry_points.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       16 2024-06-03 01:08:56.000000 bwalign-1.0.3/bwalign.egg-info/requires.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)        8 2024-06-03 01:08:56.000000 bwalign-1.0.3/bwalign.egg-info/top_level.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       38 2024-06-03 01:08:57.129769 bwalign-1.0.3/setup.cfg
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     1194 2024-06-03 01:08:17.000000 bwalign-1.0.3/setup.py
```

### Comparing `bwalign-1.0.2/PKG-INFO` & `bwalign-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bwalign
-Version: 1.0.2
+Version: 1.0.3
 Summary: A burrows-wheeler seed and extend aligner
 Home-page: https://github.com/NabilHKhoury/bwalign
 Author: ['Adrian Layer, Nabil Khoury, Yasmin Jabir']
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `bwalign-1.0.2/README.md` & `bwalign-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `bwalign-1.0.2/bwalign/main.py` & `bwalign-1.0.3/bwalign/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from utils import *
+from .utils import *
 import pysam
 import argparse
 
 def main():
     parser = argparse.ArgumentParser(description="Run BWA alignment with specified reference genome and FASTQ file.")
     parser.add_argument("reference_genome", type=str, help="Path to the reference genome file")
     parser.add_argument("fastq_file", type=str, help="Path to the FASTQ file")
```

### Comparing `bwalign-1.0.2/bwalign/utils.py` & `bwalign-1.0.3/bwalign/utils.py`

 * *Files identical despite different names*

### Comparing `bwalign-1.0.2/bwalign.egg-info/PKG-INFO` & `bwalign-1.0.3/bwalign.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bwalign
-Version: 1.0.2
+Version: 1.0.3
 Summary: A burrows-wheeler seed and extend aligner
 Home-page: https://github.com/NabilHKhoury/bwalign
 Author: ['Adrian Layer, Nabil Khoury, Yasmin Jabir']
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `bwalign-1.0.2/setup.py` & `bwalign-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='bwalign',
-    version='1.0.2',    
+    version='1.0.3',    
     description='A burrows-wheeler seed and extend aligner',
     url='https://github.com/NabilHKhoury/bwalign',
     author=['Adrian Layer, Nabil Khoury, Yasmin Jabir'],
     license='MIT',
     packages=find_packages(),
     install_requires=['biopython',
                       'pysam',
```

