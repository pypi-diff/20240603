# Comparing `tmp/bwalign-1.2.5.tar.gz` & `tmp/bwalign-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bwalign-1.2.5.tar", last modified: Mon Jun  3 09:04:11 2024, max compression
+gzip compressed data, was "bwalign-1.3.5.tar", last modified: Mon Jun  3 09:16:31 2024, max compression
```

## Comparing `bwalign-1.2.5.tar` & `bwalign-1.3.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 09:04:11.622376 bwalign-1.2.5/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      914 2024-06-03 09:04:11.621253 bwalign-1.2.5/PKG-INFO
--rw-r--r--   0 adrianlayer   (501) staff       (20)     1744 2024-05-29 18:41:22.000000 bwalign-1.2.5/README.md
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 09:04:11.612939 bwalign-1.2.5/bwalign/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      142 2024-06-03 09:03:11.000000 bwalign-1.2.5/bwalign/__init__.py
--rw-r--r--   0 adrianlayer   (501) staff       (20)     2008 2024-06-03 09:00:28.000000 bwalign-1.2.5/bwalign/main.py
--rw-r--r--   0 adrianlayer   (501) staff       (20)    18798 2024-06-03 07:10:20.000000 bwalign-1.2.5/bwalign/utils.py
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 09:04:11.618817 bwalign-1.2.5/bwalign.egg-info/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      914 2024-06-03 09:04:11.000000 bwalign-1.2.5/bwalign.egg-info/PKG-INFO
--rw-r--r--   0 adrianlayer   (501) staff       (20)      259 2024-06-03 09:04:11.000000 bwalign-1.2.5/bwalign.egg-info/SOURCES.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)        1 2024-06-03 09:04:11.000000 bwalign-1.2.5/bwalign.egg-info/dependency_links.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       46 2024-06-03 09:04:11.000000 bwalign-1.2.5/bwalign.egg-info/entry_points.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       16 2024-06-03 09:04:11.000000 bwalign-1.2.5/bwalign.egg-info/requires.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)        8 2024-06-03 09:04:11.000000 bwalign-1.2.5/bwalign.egg-info/top_level.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       38 2024-06-03 09:04:11.622578 bwalign-1.2.5/setup.cfg
--rw-r--r--   0 adrianlayer   (501) staff       (20)     1194 2024-06-03 09:03:13.000000 bwalign-1.2.5/setup.py
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 09:16:31.221291 bwalign-1.3.5/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 09:16:31.220287 bwalign-1.3.5/PKG-INFO
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     1744 2024-05-29 18:41:22.000000 bwalign-1.3.5/README.md
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 09:16:31.209208 bwalign-1.3.5/bwalign/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      142 2024-06-03 09:16:04.000000 bwalign-1.3.5/bwalign/__init__.py
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     2036 2024-06-03 09:15:41.000000 bwalign-1.3.5/bwalign/main.py
+-rw-r--r--   0 adrianlayer   (501) staff       (20)    18798 2024-06-03 07:10:20.000000 bwalign-1.3.5/bwalign/utils.py
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 09:16:31.217363 bwalign-1.3.5/bwalign.egg-info/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 09:16:31.000000 bwalign-1.3.5/bwalign.egg-info/PKG-INFO
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      259 2024-06-03 09:16:31.000000 bwalign-1.3.5/bwalign.egg-info/SOURCES.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)        1 2024-06-03 09:16:31.000000 bwalign-1.3.5/bwalign.egg-info/dependency_links.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       46 2024-06-03 09:16:31.000000 bwalign-1.3.5/bwalign.egg-info/entry_points.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       21 2024-06-03 09:16:31.000000 bwalign-1.3.5/bwalign.egg-info/requires.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)        8 2024-06-03 09:16:31.000000 bwalign-1.3.5/bwalign.egg-info/top_level.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       38 2024-06-03 09:16:31.221497 bwalign-1.3.5/setup.cfg
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     1224 2024-06-03 09:16:07.000000 bwalign-1.3.5/setup.py
```

### Comparing `bwalign-1.2.5/PKG-INFO` & `bwalign-1.3.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bwalign
-Version: 1.2.5
+Version: 1.3.5
 Summary: A burrows-wheeler seed and extend aligner
 Home-page: https://github.com/NabilHKhoury/bwalign
 Author: ['Adrian Layer, Nabil Khoury, Yasmin Jabir']
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
@@ -16,7 +16,8 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: biopython
 Requires-Dist: pysam
+Requires-Dist: tqdm
```

### Comparing `bwalign-1.2.5/README.md` & `bwalign-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `bwalign-1.2.5/bwalign/main.py` & `bwalign-1.3.5/bwalign/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .utils import *
 import pysam
 import argparse
+from time import tqdm
 
 def main():
     parser = argparse.ArgumentParser(description="Run BWA alignment with specified reference genome and FASTQ file.")
     parser.add_argument("reference_genome", type=str, help="Path to the reference genome file")
     parser.add_argument("fastq_file", type=str, help="Path to the FASTQ file")
     args = parser.parse_args()
     
@@ -28,15 +29,15 @@
     header = {
         'HD': {'VN': '1.0', 'SO': 'unsorted'},
         'SQ': [{'SN': ref_id, 'LN': len(reference)}]
     }
     
     #write to sam FILE
     with pysam.AlignmentFile("output.sam", "w", header=header) as samfile:
-        for read_id, read_seq, qual_scores in reads:
+        for read_id, read_seq, qual_scores in tqdm(reads):
             
             seed_idxes = generate_seeds(str(read_seq), bwt, 19, psa, first_occurrences, checkpoint_arrs, ranks)
             best_idx, score, alignment_s, alignment_t = compute_max_seed(str(reference), str(read_seq), seed_idxes, 2, 1, 2, 1, read_length)
 
             #create a SAM entry for the aligned read
             a = pysam.AlignedSegment()
             a.query_name = read_id
```

### Comparing `bwalign-1.2.5/bwalign/utils.py` & `bwalign-1.3.5/bwalign/utils.py`

 * *Files identical despite different names*

### Comparing `bwalign-1.2.5/bwalign.egg-info/PKG-INFO` & `bwalign-1.3.5/bwalign.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bwalign
-Version: 1.2.5
+Version: 1.3.5
 Summary: A burrows-wheeler seed and extend aligner
 Home-page: https://github.com/NabilHKhoury/bwalign
 Author: ['Adrian Layer, Nabil Khoury, Yasmin Jabir']
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
@@ -16,7 +16,8 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: biopython
 Requires-Dist: pysam
+Requires-Dist: tqdm
```

### Comparing `bwalign-1.2.5/setup.py` & `bwalign-1.3.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='bwalign',
-    version='1.2.5',    
+    version='1.3.5',    
     description='A burrows-wheeler seed and extend aligner',
     url='https://github.com/NabilHKhoury/bwalign',
     author=['Adrian Layer, Nabil Khoury, Yasmin Jabir'],
     license='MIT',
     packages=find_packages(),
     install_requires=['biopython',
-                      'pysam',                
+                      'pysam',
+                      'tqdm',                
                       ],
     entry_points={
         'console_scripts': [
             'bwalign=bwalign.main:main',
         ],
     },
```

