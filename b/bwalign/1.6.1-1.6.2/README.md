# Comparing `tmp/bwalign-1.6.1.tar.gz` & `tmp/bwalign-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bwalign-1.6.1.tar", last modified: Mon Jun  3 10:32:56 2024, max compression
+gzip compressed data, was "bwalign-1.6.2.tar", last modified: Mon Jun  3 11:07:08 2024, max compression
```

## Comparing `bwalign-1.6.1.tar` & `bwalign-1.6.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 10:32:56.229006 bwalign-1.6.1/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 10:32:56.228011 bwalign-1.6.1/PKG-INFO
--rw-r--r--   0 adrianlayer   (501) staff       (20)     1744 2024-05-29 18:41:22.000000 bwalign-1.6.1/README.md
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 10:32:56.219534 bwalign-1.6.1/bwalign/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      142 2024-06-03 10:32:36.000000 bwalign-1.6.1/bwalign/__init__.py
--rw-r--r--   0 adrianlayer   (501) staff       (20)     2233 2024-06-03 10:28:30.000000 bwalign-1.6.1/bwalign/main.py
--rw-r--r--   0 adrianlayer   (501) staff       (20)    18476 2024-06-03 10:32:24.000000 bwalign-1.6.1/bwalign/utils.py
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 10:32:56.226963 bwalign-1.6.1/bwalign.egg-info/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 10:32:56.000000 bwalign-1.6.1/bwalign.egg-info/PKG-INFO
--rw-r--r--   0 adrianlayer   (501) staff       (20)      259 2024-06-03 10:32:56.000000 bwalign-1.6.1/bwalign.egg-info/SOURCES.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)        1 2024-06-03 10:32:56.000000 bwalign-1.6.1/bwalign.egg-info/dependency_links.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       46 2024-06-03 10:32:56.000000 bwalign-1.6.1/bwalign.egg-info/entry_points.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       21 2024-06-03 10:32:56.000000 bwalign-1.6.1/bwalign.egg-info/requires.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)        8 2024-06-03 10:32:56.000000 bwalign-1.6.1/bwalign.egg-info/top_level.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       38 2024-06-03 10:32:56.229154 bwalign-1.6.1/setup.cfg
--rw-r--r--   0 adrianlayer   (501) staff       (20)     1224 2024-06-03 10:32:32.000000 bwalign-1.6.1/setup.py
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 11:07:08.715441 bwalign-1.6.2/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 11:07:08.712947 bwalign-1.6.2/PKG-INFO
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     1744 2024-05-29 18:41:22.000000 bwalign-1.6.2/README.md
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 11:07:08.705874 bwalign-1.6.2/bwalign/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      142 2024-06-03 11:06:55.000000 bwalign-1.6.2/bwalign/__init__.py
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     2230 2024-06-03 11:06:29.000000 bwalign-1.6.2/bwalign/main.py
+-rw-r--r--   0 adrianlayer   (501) staff       (20)    18476 2024-06-03 10:32:24.000000 bwalign-1.6.2/bwalign/utils.py
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 11:07:08.711660 bwalign-1.6.2/bwalign.egg-info/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 11:07:08.000000 bwalign-1.6.2/bwalign.egg-info/PKG-INFO
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      259 2024-06-03 11:07:08.000000 bwalign-1.6.2/bwalign.egg-info/SOURCES.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)        1 2024-06-03 11:07:08.000000 bwalign-1.6.2/bwalign.egg-info/dependency_links.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       46 2024-06-03 11:07:08.000000 bwalign-1.6.2/bwalign.egg-info/entry_points.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       21 2024-06-03 11:07:08.000000 bwalign-1.6.2/bwalign.egg-info/requires.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)        8 2024-06-03 11:07:08.000000 bwalign-1.6.2/bwalign.egg-info/top_level.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       38 2024-06-03 11:07:08.715674 bwalign-1.6.2/setup.cfg
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     1224 2024-06-03 11:06:52.000000 bwalign-1.6.2/setup.py
```

### Comparing `bwalign-1.6.1/PKG-INFO` & `bwalign-1.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bwalign
-Version: 1.6.1
+Version: 1.6.2
 Summary: A burrows-wheeler seed and extend aligner
 Home-page: https://github.com/NabilHKhoury/bwalign
 Author: ['Adrian Layer, Nabil Khoury, Yasmin Jabir']
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `bwalign-1.6.1/README.md` & `bwalign-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `bwalign-1.6.1/bwalign/main.py` & `bwalign-1.6.2/bwalign/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             
             #create a SAM entry for the aligned read
             a = pysam.AlignedSegment()
             a.query_name = read_id
             a.query_sequence = read_seq
             a.flag = 0
             a.reference_id = 0
-            if best_idx > float('-inf'):
+            if score > float('-inf'):
                 a.reference_start = best_idx
                 a.mapping_quality = calculate_mapping_quality(score, read_length)
                 a.cigarstring = calculate_cigar(alignment_s, alignment_t)
             else:
                 a.reference_start = 0
                 a.mapping_quality = 0
                 a.cigarstring = '0M'
```

### Comparing `bwalign-1.6.1/bwalign/utils.py` & `bwalign-1.6.2/bwalign/utils.py`

 * *Files identical despite different names*

### Comparing `bwalign-1.6.1/bwalign.egg-info/PKG-INFO` & `bwalign-1.6.2/bwalign.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bwalign
-Version: 1.6.1
+Version: 1.6.2
 Summary: A burrows-wheeler seed and extend aligner
 Home-page: https://github.com/NabilHKhoury/bwalign
 Author: ['Adrian Layer, Nabil Khoury, Yasmin Jabir']
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `bwalign-1.6.1/setup.py` & `bwalign-1.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='bwalign',
-    version='1.6.1',    
+    version='1.6.2',    
     description='A burrows-wheeler seed and extend aligner',
     url='https://github.com/NabilHKhoury/bwalign',
     author=['Adrian Layer, Nabil Khoury, Yasmin Jabir'],
     license='MIT',
     packages=find_packages(),
     install_requires=['biopython',
                       'pysam',
```

