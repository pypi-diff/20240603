# Comparing `tmp/bwalign-1.2.4.tar.gz` & `tmp/bwalign-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bwalign-1.2.4.tar", last modified: Mon Jun  3 07:11:13 2024, max compression
+gzip compressed data, was "bwalign-1.2.5.tar", last modified: Mon Jun  3 09:04:11 2024, max compression
```

## Comparing `bwalign-1.2.4.tar` & `bwalign-1.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 07:11:13.071480 bwalign-1.2.4/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      914 2024-06-03 07:11:13.069680 bwalign-1.2.4/PKG-INFO
--rw-r--r--   0 adrianlayer   (501) staff       (20)     1744 2024-05-29 18:41:22.000000 bwalign-1.2.4/README.md
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 07:11:13.059922 bwalign-1.2.4/bwalign/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      142 2024-06-03 07:10:59.000000 bwalign-1.2.4/bwalign/__init__.py
--rw-r--r--   0 adrianlayer   (501) staff       (20)     2007 2024-06-03 01:39:28.000000 bwalign-1.2.4/bwalign/main.py
--rw-r--r--   0 adrianlayer   (501) staff       (20)    18798 2024-06-03 07:10:20.000000 bwalign-1.2.4/bwalign/utils.py
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 07:11:13.068310 bwalign-1.2.4/bwalign.egg-info/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      914 2024-06-03 07:11:12.000000 bwalign-1.2.4/bwalign.egg-info/PKG-INFO
--rw-r--r--   0 adrianlayer   (501) staff       (20)      259 2024-06-03 07:11:12.000000 bwalign-1.2.4/bwalign.egg-info/SOURCES.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)        1 2024-06-03 07:11:12.000000 bwalign-1.2.4/bwalign.egg-info/dependency_links.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       46 2024-06-03 07:11:12.000000 bwalign-1.2.4/bwalign.egg-info/entry_points.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       16 2024-06-03 07:11:12.000000 bwalign-1.2.4/bwalign.egg-info/requires.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)        8 2024-06-03 07:11:12.000000 bwalign-1.2.4/bwalign.egg-info/top_level.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       38 2024-06-03 07:11:13.071917 bwalign-1.2.4/setup.cfg
--rw-r--r--   0 adrianlayer   (501) staff       (20)     1194 2024-06-03 07:10:52.000000 bwalign-1.2.4/setup.py
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 09:04:11.622376 bwalign-1.2.5/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      914 2024-06-03 09:04:11.621253 bwalign-1.2.5/PKG-INFO
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     1744 2024-05-29 18:41:22.000000 bwalign-1.2.5/README.md
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 09:04:11.612939 bwalign-1.2.5/bwalign/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      142 2024-06-03 09:03:11.000000 bwalign-1.2.5/bwalign/__init__.py
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     2008 2024-06-03 09:00:28.000000 bwalign-1.2.5/bwalign/main.py
+-rw-r--r--   0 adrianlayer   (501) staff       (20)    18798 2024-06-03 07:10:20.000000 bwalign-1.2.5/bwalign/utils.py
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 09:04:11.618817 bwalign-1.2.5/bwalign.egg-info/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      914 2024-06-03 09:04:11.000000 bwalign-1.2.5/bwalign.egg-info/PKG-INFO
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      259 2024-06-03 09:04:11.000000 bwalign-1.2.5/bwalign.egg-info/SOURCES.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)        1 2024-06-03 09:04:11.000000 bwalign-1.2.5/bwalign.egg-info/dependency_links.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       46 2024-06-03 09:04:11.000000 bwalign-1.2.5/bwalign.egg-info/entry_points.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       16 2024-06-03 09:04:11.000000 bwalign-1.2.5/bwalign.egg-info/requires.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)        8 2024-06-03 09:04:11.000000 bwalign-1.2.5/bwalign.egg-info/top_level.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       38 2024-06-03 09:04:11.622578 bwalign-1.2.5/setup.cfg
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     1194 2024-06-03 09:03:13.000000 bwalign-1.2.5/setup.py
```

### Comparing `bwalign-1.2.4/PKG-INFO` & `bwalign-1.2.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bwalign
-Version: 1.2.4
+Version: 1.2.5
 Summary: A burrows-wheeler seed and extend aligner
 Home-page: https://github.com/NabilHKhoury/bwalign
 Author: ['Adrian Layer, Nabil Khoury, Yasmin Jabir']
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `bwalign-1.2.4/README.md` & `bwalign-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `bwalign-1.2.4/bwalign/main.py` & `bwalign-1.2.5/bwalign/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         'SQ': [{'SN': ref_id, 'LN': len(reference)}]
     }
     
     #write to sam FILE
     with pysam.AlignmentFile("output.sam", "w", header=header) as samfile:
         for read_id, read_seq, qual_scores in reads:
             
-            seed_idxes = generate_seeds(str(read_seq), bwt, 8, psa, first_occurrences, checkpoint_arrs, ranks)
+            seed_idxes = generate_seeds(str(read_seq), bwt, 19, psa, first_occurrences, checkpoint_arrs, ranks)
             best_idx, score, alignment_s, alignment_t = compute_max_seed(str(reference), str(read_seq), seed_idxes, 2, 1, 2, 1, read_length)
 
             #create a SAM entry for the aligned read
             a = pysam.AlignedSegment()
             a.query_name = read_id
             a.query_sequence = read_seq
             a.flag = 0
```

### Comparing `bwalign-1.2.4/bwalign/utils.py` & `bwalign-1.2.5/bwalign/utils.py`

 * *Files identical despite different names*

### Comparing `bwalign-1.2.4/bwalign.egg-info/PKG-INFO` & `bwalign-1.2.5/bwalign.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bwalign
-Version: 1.2.4
+Version: 1.2.5
 Summary: A burrows-wheeler seed and extend aligner
 Home-page: https://github.com/NabilHKhoury/bwalign
 Author: ['Adrian Layer, Nabil Khoury, Yasmin Jabir']
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `bwalign-1.2.4/setup.py` & `bwalign-1.2.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='bwalign',
-    version='1.2.4',    
+    version='1.2.5',    
     description='A burrows-wheeler seed and extend aligner',
     url='https://github.com/NabilHKhoury/bwalign',
     author=['Adrian Layer, Nabil Khoury, Yasmin Jabir'],
     license='MIT',
     packages=find_packages(),
     install_requires=['biopython',
                       'pysam',
```

