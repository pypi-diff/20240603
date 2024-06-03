# Comparing `tmp/bwalign-1.0.0.tar.gz` & `tmp/bwalign-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bwalign-1.0.0.tar", last modified: Mon Jun  3 00:02:39 2024, max compression
+gzip compressed data, was "bwalign-1.0.1.tar", last modified: Mon Jun  3 00:50:15 2024, max compression
```

## Comparing `bwalign-1.0.0.tar` & `bwalign-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 00:02:39.534069 bwalign-1.0.0/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      914 2024-06-03 00:02:39.531797 bwalign-1.0.0/PKG-INFO
--rw-r--r--   0 adrianlayer   (501) staff       (20)     1744 2024-05-29 18:41:22.000000 bwalign-1.0.0/README.md
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 00:02:39.513790 bwalign-1.0.0/bwalign/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      142 2024-06-03 00:01:19.000000 bwalign-1.0.0/bwalign/__init__.py
--rw-r--r--   0 adrianlayer   (501) staff       (20)     2146 2024-06-02 23:55:00.000000 bwalign-1.0.0/bwalign/main.py
--rw-r--r--   0 adrianlayer   (501) staff       (20)    20537 2024-06-02 23:56:53.000000 bwalign-1.0.0/bwalign/utils.py
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 00:02:39.527307 bwalign-1.0.0/bwalign.egg-info/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      914 2024-06-03 00:02:39.000000 bwalign-1.0.0/bwalign.egg-info/PKG-INFO
--rw-r--r--   0 adrianlayer   (501) staff       (20)      259 2024-06-03 00:02:39.000000 bwalign-1.0.0/bwalign.egg-info/SOURCES.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)        1 2024-06-03 00:02:39.000000 bwalign-1.0.0/bwalign.egg-info/dependency_links.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       46 2024-06-03 00:02:39.000000 bwalign-1.0.0/bwalign.egg-info/entry_points.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       16 2024-06-03 00:02:39.000000 bwalign-1.0.0/bwalign.egg-info/requires.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)        8 2024-06-03 00:02:39.000000 bwalign-1.0.0/bwalign.egg-info/top_level.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       38 2024-06-03 00:02:39.534603 bwalign-1.0.0/setup.cfg
--rw-r--r--   0 adrianlayer   (501) staff       (20)     1194 2024-06-03 00:00:58.000000 bwalign-1.0.0/setup.py
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 00:50:15.734359 bwalign-1.0.1/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      914 2024-06-03 00:50:15.733477 bwalign-1.0.1/PKG-INFO
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     1744 2024-05-29 18:41:22.000000 bwalign-1.0.1/README.md
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 00:50:15.726035 bwalign-1.0.1/bwalign/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      142 2024-06-03 00:49:05.000000 bwalign-1.0.1/bwalign/__init__.py
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     2156 2024-06-03 00:47:46.000000 bwalign-1.0.1/bwalign/main.py
+-rw-r--r--   0 adrianlayer   (501) staff       (20)    20539 2024-06-03 00:30:17.000000 bwalign-1.0.1/bwalign/utils.py
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 00:50:15.731790 bwalign-1.0.1/bwalign.egg-info/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      914 2024-06-03 00:50:15.000000 bwalign-1.0.1/bwalign.egg-info/PKG-INFO
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      259 2024-06-03 00:50:15.000000 bwalign-1.0.1/bwalign.egg-info/SOURCES.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)        1 2024-06-03 00:50:15.000000 bwalign-1.0.1/bwalign.egg-info/dependency_links.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       46 2024-06-03 00:50:15.000000 bwalign-1.0.1/bwalign.egg-info/entry_points.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       16 2024-06-03 00:50:15.000000 bwalign-1.0.1/bwalign.egg-info/requires.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)        8 2024-06-03 00:50:15.000000 bwalign-1.0.1/bwalign.egg-info/top_level.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       38 2024-06-03 00:50:15.734520 bwalign-1.0.1/setup.cfg
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     1194 2024-06-03 00:49:07.000000 bwalign-1.0.1/setup.py
```

### Comparing `bwalign-1.0.0/PKG-INFO` & `bwalign-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bwalign
-Version: 1.0.0
+Version: 1.0.1
 Summary: A burrows-wheeler seed and extend aligner
 Home-page: https://github.com/NabilHKhoury/bwalign
 Author: ['Adrian Layer, Nabil Khoury, Yasmin Jabir']
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `bwalign-1.0.0/README.md` & `bwalign-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `bwalign-1.0.0/bwalign/main.py` & `bwalign-1.0.1/bwalign/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import utils
+import utils as utils
 import pysam
 import argparse
 
 def main():
     parser = argparse.ArgumentParser(description="Run BWA alignment with specified reference genome and FASTQ file.")
     parser.add_argument("reference_genome", type=str, help="Path to the reference genome file")
     parser.add_argument("fastq_file", type=str, help="Path to the FASTQ file")
@@ -17,15 +17,15 @@
     ref_id, reference = utils.parse_reference_genome(args.reference_genome)
     
     #BWT and SA
     K = 5
     ref_text = str(reference) + '$'
     sa = utils.suffix_array(ref_text)
     psa = utils.partial_suffix_array(sa, K)
-    bwt = utils.bwt_from_suffixarray(ref_text, sa)
+    bwt = utils.bwt_from_suffix_array(ref_text, sa)
     first_occurrences = utils.compute_first_occurrences(bwt)
     checkpoint_arrs = utils.compute_checkpoint_arrs(bwt)
     ranks = utils.compute_rank_arr(bwt)
     
     #header for the SAM file (based on ref)
     header = {
         'HD': {'VN': '1.0', 'SO': 'unsorted'},
```

### Comparing `bwalign-1.0.0/bwalign/utils.py` & `bwalign-1.0.1/bwalign/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,22 +208,16 @@
                 best_idx = ref_idx
                 s_best_align = s_align
                 t_best_align = t_align
     return best_idx, best_score, s_best_align, t_best_align
 
 ### SEED GENERATION
 
-## BWT creation
-def bwt_from_suffixarray(text: str, suffix_array: List[int]) -> str:
-    bwt = []
-    for idx in suffix_array:
-        bwt.append(text[idx-1])
-    return ''.join(bwt)
-
 # SUFFIX ARRAY CONSTRUCTION
+
 class suffix:
     """
     Class built to store suffix array indices, conserving memory.
     """
     def __init__(self):
         self.index = 0
         self.rank = [0,0]
@@ -314,14 +308,21 @@
     """
     partial = dict()
     for idx in sa:
         if sa[idx] % k == 0:
             partial[idx] = sa[idx]
     return partial
 
+## BWT creation
+def bwt_from_suffix_array(text: str, suffix_array: List[int]) -> str:
+    bwt = []
+    for idx in suffix_array:
+        bwt.append(text[idx-1])
+    return ''.join(bwt)
+
 def compute_rank_arr(bwt: str) -> list[int]:
     """
     This function generates the rank of each position in the last column given by the bwt.
     The rank is the number of occurrences of whatever character is at that position, up to
     that position. This can be done in linear time by iterating through the bwt. The ranks
     will be returned in the form of a list of ranks, obviously indices will be in-built.
     """
```

### Comparing `bwalign-1.0.0/bwalign.egg-info/PKG-INFO` & `bwalign-1.0.1/bwalign.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bwalign
-Version: 1.0.0
+Version: 1.0.1
 Summary: A burrows-wheeler seed and extend aligner
 Home-page: https://github.com/NabilHKhoury/bwalign
 Author: ['Adrian Layer, Nabil Khoury, Yasmin Jabir']
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `bwalign-1.0.0/setup.py` & `bwalign-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='bwalign',
-    version='1.0.0',    
+    version='1.0.1',    
     description='A burrows-wheeler seed and extend aligner',
     url='https://github.com/NabilHKhoury/bwalign',
     author=['Adrian Layer, Nabil Khoury, Yasmin Jabir'],
     license='MIT',
     packages=find_packages(),
     install_requires=['biopython',
                       'pysam',
```

