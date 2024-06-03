# Comparing `tmp/bwalign-1.3.6.tar.gz` & `tmp/bwalign-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bwalign-1.3.6.tar", last modified: Mon Jun  3 09:21:15 2024, max compression
+gzip compressed data, was "bwalign-1.3.7.tar", last modified: Mon Jun  3 09:24:16 2024, max compression
```

## Comparing `bwalign-1.3.6.tar` & `bwalign-1.3.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 09:21:15.543909 bwalign-1.3.6/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 09:21:15.542433 bwalign-1.3.6/PKG-INFO
--rw-r--r--   0 adrianlayer   (501) staff       (20)     1744 2024-05-29 18:41:22.000000 bwalign-1.3.6/README.md
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 09:21:15.534617 bwalign-1.3.6/bwalign/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      142 2024-06-03 09:21:04.000000 bwalign-1.3.6/bwalign/__init__.py
--rw-r--r--   0 adrianlayer   (501) staff       (20)     2026 2024-06-03 09:20:35.000000 bwalign-1.3.6/bwalign/main.py
--rw-r--r--   0 adrianlayer   (501) staff       (20)    18798 2024-06-03 07:10:20.000000 bwalign-1.3.6/bwalign/utils.py
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 09:21:15.541309 bwalign-1.3.6/bwalign.egg-info/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 09:21:15.000000 bwalign-1.3.6/bwalign.egg-info/PKG-INFO
--rw-r--r--   0 adrianlayer   (501) staff       (20)      259 2024-06-03 09:21:15.000000 bwalign-1.3.6/bwalign.egg-info/SOURCES.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)        1 2024-06-03 09:21:15.000000 bwalign-1.3.6/bwalign.egg-info/dependency_links.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       46 2024-06-03 09:21:15.000000 bwalign-1.3.6/bwalign.egg-info/entry_points.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       21 2024-06-03 09:21:15.000000 bwalign-1.3.6/bwalign.egg-info/requires.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)        8 2024-06-03 09:21:15.000000 bwalign-1.3.6/bwalign.egg-info/top_level.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       38 2024-06-03 09:21:15.544111 bwalign-1.3.6/setup.cfg
--rw-r--r--   0 adrianlayer   (501) staff       (20)     1224 2024-06-03 09:21:05.000000 bwalign-1.3.6/setup.py
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 09:24:16.763116 bwalign-1.3.7/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 09:24:16.762039 bwalign-1.3.7/PKG-INFO
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     1744 2024-05-29 18:41:22.000000 bwalign-1.3.7/README.md
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 09:24:16.754275 bwalign-1.3.7/bwalign/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      142 2024-06-03 09:23:54.000000 bwalign-1.3.7/bwalign/__init__.py
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     2036 2024-06-03 09:23:45.000000 bwalign-1.3.7/bwalign/main.py
+-rw-r--r--   0 adrianlayer   (501) staff       (20)    18798 2024-06-03 07:10:20.000000 bwalign-1.3.7/bwalign/utils.py
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 09:24:16.760258 bwalign-1.3.7/bwalign.egg-info/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 09:24:16.000000 bwalign-1.3.7/bwalign.egg-info/PKG-INFO
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      259 2024-06-03 09:24:16.000000 bwalign-1.3.7/bwalign.egg-info/SOURCES.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)        1 2024-06-03 09:24:16.000000 bwalign-1.3.7/bwalign.egg-info/dependency_links.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       46 2024-06-03 09:24:16.000000 bwalign-1.3.7/bwalign.egg-info/entry_points.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       21 2024-06-03 09:24:16.000000 bwalign-1.3.7/bwalign.egg-info/requires.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)        8 2024-06-03 09:24:16.000000 bwalign-1.3.7/bwalign.egg-info/top_level.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       38 2024-06-03 09:24:16.763261 bwalign-1.3.7/setup.cfg
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     1224 2024-06-03 09:23:51.000000 bwalign-1.3.7/setup.py
```

### Comparing `bwalign-1.3.6/PKG-INFO` & `bwalign-1.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bwalign
-Version: 1.3.6
+Version: 1.3.7
 Summary: A burrows-wheeler seed and extend aligner
 Home-page: https://github.com/NabilHKhoury/bwalign
 Author: ['Adrian Layer, Nabil Khoury, Yasmin Jabir']
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `bwalign-1.3.6/README.md` & `bwalign-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `bwalign-1.3.6/bwalign/main.py` & `bwalign-1.3.7/bwalign/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .utils import *
 import pysam
 import argparse
-import tqdm
+from tqdm import tqdm
 
 def main():
     parser = argparse.ArgumentParser(description="Run BWA alignment with specified reference genome and FASTQ file.")
     parser.add_argument("reference_genome", type=str, help="Path to the reference genome file")
     parser.add_argument("fastq_file", type=str, help="Path to the FASTQ file")
     args = parser.parse_args()
```

### Comparing `bwalign-1.3.6/bwalign/utils.py` & `bwalign-1.3.7/bwalign/utils.py`

 * *Files identical despite different names*

### Comparing `bwalign-1.3.6/bwalign.egg-info/PKG-INFO` & `bwalign-1.3.7/bwalign.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bwalign
-Version: 1.3.6
+Version: 1.3.7
 Summary: A burrows-wheeler seed and extend aligner
 Home-page: https://github.com/NabilHKhoury/bwalign
 Author: ['Adrian Layer, Nabil Khoury, Yasmin Jabir']
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `bwalign-1.3.6/setup.py` & `bwalign-1.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='bwalign',
-    version='1.3.6',    
+    version='1.3.7',    
     description='A burrows-wheeler seed and extend aligner',
     url='https://github.com/NabilHKhoury/bwalign',
     author=['Adrian Layer, Nabil Khoury, Yasmin Jabir'],
     license='MIT',
     packages=find_packages(),
     install_requires=['biopython',
                       'pysam',
```

