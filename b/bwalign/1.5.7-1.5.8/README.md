# Comparing `tmp/bwalign-1.5.7.tar.gz` & `tmp/bwalign-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bwalign-1.5.7.tar", last modified: Mon Jun  3 10:19:47 2024, max compression
+gzip compressed data, was "bwalign-1.5.8.tar", last modified: Mon Jun  3 10:24:25 2024, max compression
```

## Comparing `bwalign-1.5.7.tar` & `bwalign-1.5.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 10:19:47.849565 bwalign-1.5.7/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 10:19:47.848808 bwalign-1.5.7/PKG-INFO
--rw-r--r--   0 adrianlayer   (501) staff       (20)     1744 2024-05-29 18:41:22.000000 bwalign-1.5.7/README.md
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 10:19:47.840550 bwalign-1.5.7/bwalign/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      142 2024-06-03 10:19:36.000000 bwalign-1.5.7/bwalign/__init__.py
--rw-r--r--   0 adrianlayer   (501) staff       (20)     2037 2024-06-03 09:46:02.000000 bwalign-1.5.7/bwalign/main.py
--rw-r--r--   0 adrianlayer   (501) staff       (20)    18374 2024-06-03 10:18:37.000000 bwalign-1.5.7/bwalign/utils.py
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 10:19:47.847791 bwalign-1.5.7/bwalign.egg-info/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 10:19:47.000000 bwalign-1.5.7/bwalign.egg-info/PKG-INFO
--rw-r--r--   0 adrianlayer   (501) staff       (20)      259 2024-06-03 10:19:47.000000 bwalign-1.5.7/bwalign.egg-info/SOURCES.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)        1 2024-06-03 10:19:47.000000 bwalign-1.5.7/bwalign.egg-info/dependency_links.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       46 2024-06-03 10:19:47.000000 bwalign-1.5.7/bwalign.egg-info/entry_points.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       21 2024-06-03 10:19:47.000000 bwalign-1.5.7/bwalign.egg-info/requires.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)        8 2024-06-03 10:19:47.000000 bwalign-1.5.7/bwalign.egg-info/top_level.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       38 2024-06-03 10:19:47.851764 bwalign-1.5.7/setup.cfg
--rw-r--r--   0 adrianlayer   (501) staff       (20)     1224 2024-06-03 10:19:34.000000 bwalign-1.5.7/setup.py
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 10:24:25.186432 bwalign-1.5.8/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 10:24:25.185320 bwalign-1.5.8/PKG-INFO
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     1744 2024-05-29 18:41:22.000000 bwalign-1.5.8/README.md
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 10:24:25.178007 bwalign-1.5.8/bwalign/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      142 2024-06-03 10:24:07.000000 bwalign-1.5.8/bwalign/__init__.py
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     2236 2024-06-03 10:23:56.000000 bwalign-1.5.8/bwalign/main.py
+-rw-r--r--   0 adrianlayer   (501) staff       (20)    18374 2024-06-03 10:18:37.000000 bwalign-1.5.8/bwalign/utils.py
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 10:24:25.184259 bwalign-1.5.8/bwalign.egg-info/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 10:24:25.000000 bwalign-1.5.8/bwalign.egg-info/PKG-INFO
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      259 2024-06-03 10:24:25.000000 bwalign-1.5.8/bwalign.egg-info/SOURCES.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)        1 2024-06-03 10:24:25.000000 bwalign-1.5.8/bwalign.egg-info/dependency_links.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       46 2024-06-03 10:24:25.000000 bwalign-1.5.8/bwalign.egg-info/entry_points.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       21 2024-06-03 10:24:25.000000 bwalign-1.5.8/bwalign.egg-info/requires.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)        8 2024-06-03 10:24:25.000000 bwalign-1.5.8/bwalign.egg-info/top_level.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       38 2024-06-03 10:24:25.186583 bwalign-1.5.8/setup.cfg
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     1224 2024-06-03 10:24:04.000000 bwalign-1.5.8/setup.py
```

### Comparing `bwalign-1.5.7/PKG-INFO` & `bwalign-1.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bwalign
-Version: 1.5.7
+Version: 1.5.8
 Summary: A burrows-wheeler seed and extend aligner
 Home-page: https://github.com/NabilHKhoury/bwalign
 Author: ['Adrian Layer, Nabil Khoury, Yasmin Jabir']
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `bwalign-1.5.7/README.md` & `bwalign-1.5.8/README.md`

 * *Files identical despite different names*

### Comparing `bwalign-1.5.7/bwalign/main.py` & `bwalign-1.5.8/bwalign/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,23 +33,28 @@
     
     #write to sam FILE
     with pysam.AlignmentFile("output.sam", "w", header=header) as samfile:
         for read_id, read_seq, qual_scores in tqdm(reads):
             
             seed_idxes = generate_seeds(str(read_seq), bwt, 19, psa, first_occurrences, checkpoint_arrs, ranks)
             best_idx, score, alignment_s, alignment_t = compute_max_seed(str(reference), str(read_seq), seed_idxes, 2, 2, 2, 10, read_length)
-
+            
             #create a SAM entry for the aligned read
             a = pysam.AlignedSegment()
             a.query_name = read_id
             a.query_sequence = read_seq
             a.flag = 0
             a.reference_id = 0
-            a.reference_start = best_idx
-            a.mapping_quality = calculate_mapping_quality(score, read_length)
-            a.cigarstring = calculate_cigar(alignment_s, alignment_t)
+            if best_idx == float('-inf'):
+                a.reference_start = -1
+                a.mapping_quality = -1
+                a.cigarstring = '0M'
+            else:
+                a.reference_start = best_idx
+                a.mapping_quality = calculate_mapping_quality(score, read_length)
+                a.cigarstring = calculate_cigar(alignment_s, alignment_t)
             a.query_qualities = qual_scores
             
             samfile.write(a)
 
 if __name__ == "__main__":
     main()
```

### Comparing `bwalign-1.5.7/bwalign/utils.py` & `bwalign-1.5.8/bwalign/utils.py`

 * *Files identical despite different names*

### Comparing `bwalign-1.5.7/bwalign.egg-info/PKG-INFO` & `bwalign-1.5.8/bwalign.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bwalign
-Version: 1.5.7
+Version: 1.5.8
 Summary: A burrows-wheeler seed and extend aligner
 Home-page: https://github.com/NabilHKhoury/bwalign
 Author: ['Adrian Layer, Nabil Khoury, Yasmin Jabir']
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `bwalign-1.5.7/setup.py` & `bwalign-1.5.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='bwalign',
-    version='1.5.7',    
+    version='1.5.8',    
     description='A burrows-wheeler seed and extend aligner',
     url='https://github.com/NabilHKhoury/bwalign',
     author=['Adrian Layer, Nabil Khoury, Yasmin Jabir'],
     license='MIT',
     packages=find_packages(),
     install_requires=['biopython',
                       'pysam',
```

