# Comparing `tmp/bwalign-1.0.4.tar.gz` & `tmp/bwalign-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bwalign-1.0.4.tar", last modified: Mon Jun  3 01:09:48 2024, max compression
+gzip compressed data, was "bwalign-1.1.4.tar", last modified: Mon Jun  3 01:32:27 2024, max compression
```

## Comparing `bwalign-1.0.4.tar` & `bwalign-1.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 01:09:48.455514 bwalign-1.0.4/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      914 2024-06-03 01:09:48.452045 bwalign-1.0.4/PKG-INFO
--rw-r--r--   0 adrianlayer   (501) staff       (20)     1744 2024-05-29 18:41:22.000000 bwalign-1.0.4/README.md
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 01:09:48.443496 bwalign-1.0.4/bwalign/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      142 2024-06-03 01:09:30.000000 bwalign-1.0.4/bwalign/__init__.py
--rw-r--r--   0 adrianlayer   (501) staff       (20)     2083 2024-06-03 01:09:18.000000 bwalign-1.0.4/bwalign/main.py
--rw-r--r--   0 adrianlayer   (501) staff       (20)    20539 2024-06-03 00:56:50.000000 bwalign-1.0.4/bwalign/utils.py
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 01:09:48.450902 bwalign-1.0.4/bwalign.egg-info/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      914 2024-06-03 01:09:48.000000 bwalign-1.0.4/bwalign.egg-info/PKG-INFO
--rw-r--r--   0 adrianlayer   (501) staff       (20)      259 2024-06-03 01:09:48.000000 bwalign-1.0.4/bwalign.egg-info/SOURCES.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)        1 2024-06-03 01:09:48.000000 bwalign-1.0.4/bwalign.egg-info/dependency_links.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       46 2024-06-03 01:09:48.000000 bwalign-1.0.4/bwalign.egg-info/entry_points.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       16 2024-06-03 01:09:48.000000 bwalign-1.0.4/bwalign.egg-info/requires.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)        8 2024-06-03 01:09:48.000000 bwalign-1.0.4/bwalign.egg-info/top_level.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       38 2024-06-03 01:09:48.455816 bwalign-1.0.4/setup.cfg
--rw-r--r--   0 adrianlayer   (501) staff       (20)     1194 2024-06-03 01:09:27.000000 bwalign-1.0.4/setup.py
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 01:32:27.110718 bwalign-1.1.4/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      914 2024-06-03 01:32:27.109878 bwalign-1.1.4/PKG-INFO
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     1744 2024-05-29 18:41:22.000000 bwalign-1.1.4/README.md
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 01:32:27.102481 bwalign-1.1.4/bwalign/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      142 2024-06-03 01:32:16.000000 bwalign-1.1.4/bwalign/__init__.py
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     2007 2024-06-03 01:31:20.000000 bwalign-1.1.4/bwalign/main.py
+-rw-r--r--   0 adrianlayer   (501) staff       (20)    20737 2024-06-03 01:30:46.000000 bwalign-1.1.4/bwalign/utils.py
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 01:32:27.108434 bwalign-1.1.4/bwalign.egg-info/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      914 2024-06-03 01:32:26.000000 bwalign-1.1.4/bwalign.egg-info/PKG-INFO
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      259 2024-06-03 01:32:27.000000 bwalign-1.1.4/bwalign.egg-info/SOURCES.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)        1 2024-06-03 01:32:26.000000 bwalign-1.1.4/bwalign.egg-info/dependency_links.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       46 2024-06-03 01:32:26.000000 bwalign-1.1.4/bwalign.egg-info/entry_points.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       16 2024-06-03 01:32:26.000000 bwalign-1.1.4/bwalign.egg-info/requires.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)        8 2024-06-03 01:32:26.000000 bwalign-1.1.4/bwalign.egg-info/top_level.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       38 2024-06-03 01:32:27.110871 bwalign-1.1.4/setup.cfg
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     1194 2024-06-03 01:32:12.000000 bwalign-1.1.4/setup.py
```

### Comparing `bwalign-1.0.4/PKG-INFO` & `bwalign-1.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bwalign
-Version: 1.0.4
+Version: 1.1.4
 Summary: A burrows-wheeler seed and extend aligner
 Home-page: https://github.com/NabilHKhoury/bwalign
 Author: ['Adrian Layer, Nabil Khoury, Yasmin Jabir']
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `bwalign-1.0.4/README.md` & `bwalign-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `bwalign-1.0.4/bwalign/main.py` & `bwalign-1.1.4/bwalign/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,17 +15,15 @@
     
     # Parse the reference genome
     ref_id, reference = parse_reference_genome(args.reference_genome)
     
     #BWT and SA
     K = 5
     ref_text = str(reference) + '$'
-    sa = suffix_array(ref_text)
-    psa = partial_suffix_array(sa, K)
-    bwt = bwt_from_suffix_array(ref_text, sa)
+    bwt, psa = bwt_psa_out(ref_text, K)
     first_occurrences = compute_first_occurrences(bwt)
     checkpoint_arrs = compute_checkpoint_arrs(bwt)
     ranks = compute_rank_arr(bwt)
     
     #header for the SAM file (based on ref)
     header = {
         'HD': {'VN': '1.0', 'SO': 'unsorted'},
```

### Comparing `bwalign-1.0.4/bwalign/utils.py` & `bwalign-1.1.4/bwalign/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -309,20 +309,27 @@
     partial = dict()
     for idx in sa:
         if sa[idx] % k == 0:
             partial[idx] = sa[idx]
     return partial
 
 ## BWT creation
+
 def bwt_from_suffix_array(text: str, suffix_array: List[int]) -> str:
     bwt = []
     for idx in suffix_array:
         bwt.append(text[idx-1])
     return ''.join(bwt)
 
+def bwt_psa_out(text: str, k: int) -> tuple[str, dict[int, int]]:
+    sa = suffix_array(text)
+    bwt = bwt_from_suffix_array(text, sa)
+    psa = partial_suffix_array(sa, k)
+    return (bwt, psa)
+
 def compute_rank_arr(bwt: str) -> list[int]:
     """
     This function generates the rank of each position in the last column given by the bwt.
     The rank is the number of occurrences of whatever character is at that position, up to
     that position. This can be done in linear time by iterating through the bwt. The ranks
     will be returned in the form of a list of ranks, obviously indices will be in-built.
     """
```

### Comparing `bwalign-1.0.4/bwalign.egg-info/PKG-INFO` & `bwalign-1.1.4/bwalign.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bwalign
-Version: 1.0.4
+Version: 1.1.4
 Summary: A burrows-wheeler seed and extend aligner
 Home-page: https://github.com/NabilHKhoury/bwalign
 Author: ['Adrian Layer, Nabil Khoury, Yasmin Jabir']
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `bwalign-1.0.4/setup.py` & `bwalign-1.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='bwalign',
-    version='1.0.4',    
+    version='1.1.4',    
     description='A burrows-wheeler seed and extend aligner',
     url='https://github.com/NabilHKhoury/bwalign',
     author=['Adrian Layer, Nabil Khoury, Yasmin Jabir'],
     license='MIT',
     packages=find_packages(),
     install_requires=['biopython',
                       'pysam',
```

