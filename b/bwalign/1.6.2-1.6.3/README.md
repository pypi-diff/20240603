# Comparing `tmp/bwalign-1.6.2.tar.gz` & `tmp/bwalign-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bwalign-1.6.2.tar", last modified: Mon Jun  3 11:07:08 2024, max compression
+gzip compressed data, was "bwalign-1.6.3.tar", last modified: Mon Jun  3 11:21:39 2024, max compression
```

## Comparing `bwalign-1.6.2.tar` & `bwalign-1.6.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 11:07:08.715441 bwalign-1.6.2/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 11:07:08.712947 bwalign-1.6.2/PKG-INFO
--rw-r--r--   0 adrianlayer   (501) staff       (20)     1744 2024-05-29 18:41:22.000000 bwalign-1.6.2/README.md
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 11:07:08.705874 bwalign-1.6.2/bwalign/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      142 2024-06-03 11:06:55.000000 bwalign-1.6.2/bwalign/__init__.py
--rw-r--r--   0 adrianlayer   (501) staff       (20)     2230 2024-06-03 11:06:29.000000 bwalign-1.6.2/bwalign/main.py
--rw-r--r--   0 adrianlayer   (501) staff       (20)    18476 2024-06-03 10:32:24.000000 bwalign-1.6.2/bwalign/utils.py
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 11:07:08.711660 bwalign-1.6.2/bwalign.egg-info/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 11:07:08.000000 bwalign-1.6.2/bwalign.egg-info/PKG-INFO
--rw-r--r--   0 adrianlayer   (501) staff       (20)      259 2024-06-03 11:07:08.000000 bwalign-1.6.2/bwalign.egg-info/SOURCES.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)        1 2024-06-03 11:07:08.000000 bwalign-1.6.2/bwalign.egg-info/dependency_links.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       46 2024-06-03 11:07:08.000000 bwalign-1.6.2/bwalign.egg-info/entry_points.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       21 2024-06-03 11:07:08.000000 bwalign-1.6.2/bwalign.egg-info/requires.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)        8 2024-06-03 11:07:08.000000 bwalign-1.6.2/bwalign.egg-info/top_level.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       38 2024-06-03 11:07:08.715674 bwalign-1.6.2/setup.cfg
--rw-r--r--   0 adrianlayer   (501) staff       (20)     1224 2024-06-03 11:06:52.000000 bwalign-1.6.2/setup.py
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 11:21:39.230229 bwalign-1.6.3/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 11:21:39.229374 bwalign-1.6.3/PKG-INFO
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     1744 2024-05-29 18:41:22.000000 bwalign-1.6.3/README.md
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 11:21:39.219212 bwalign-1.6.3/bwalign/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      142 2024-06-03 11:21:18.000000 bwalign-1.6.3/bwalign/__init__.py
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     2228 2024-06-03 11:21:12.000000 bwalign-1.6.3/bwalign/main.py
+-rw-r--r--   0 adrianlayer   (501) staff       (20)    18518 2024-06-03 11:20:34.000000 bwalign-1.6.3/bwalign/utils.py
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 11:21:39.226788 bwalign-1.6.3/bwalign.egg-info/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 11:21:39.000000 bwalign-1.6.3/bwalign.egg-info/PKG-INFO
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      259 2024-06-03 11:21:39.000000 bwalign-1.6.3/bwalign.egg-info/SOURCES.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)        1 2024-06-03 11:21:39.000000 bwalign-1.6.3/bwalign.egg-info/dependency_links.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       46 2024-06-03 11:21:39.000000 bwalign-1.6.3/bwalign.egg-info/entry_points.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       21 2024-06-03 11:21:39.000000 bwalign-1.6.3/bwalign.egg-info/requires.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)        8 2024-06-03 11:21:39.000000 bwalign-1.6.3/bwalign.egg-info/top_level.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       38 2024-06-03 11:21:39.230383 bwalign-1.6.3/setup.cfg
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     1224 2024-06-03 11:21:16.000000 bwalign-1.6.3/setup.py
```

### Comparing `bwalign-1.6.2/PKG-INFO` & `bwalign-1.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bwalign
-Version: 1.6.2
+Version: 1.6.3
 Summary: A burrows-wheeler seed and extend aligner
 Home-page: https://github.com/NabilHKhoury/bwalign
 Author: ['Adrian Layer, Nabil Khoury, Yasmin Jabir']
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `bwalign-1.6.2/README.md` & `bwalign-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `bwalign-1.6.2/bwalign/main.py` & `bwalign-1.6.3/bwalign/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,21 +40,21 @@
             
             #create a SAM entry for the aligned read
             a = pysam.AlignedSegment()
             a.query_name = read_id
             a.query_sequence = read_seq
             a.flag = 0
             a.reference_id = 0
-            if score > float('-inf'):
-                a.reference_start = best_idx
-                a.mapping_quality = calculate_mapping_quality(score, read_length)
-                a.cigarstring = calculate_cigar(alignment_s, alignment_t)
-            else:
+            if alignment_s == None:
                 a.reference_start = 0
                 a.mapping_quality = 0
                 a.cigarstring = '0M'
+            else:
+                a.reference_start = best_idx
+                a.mapping_quality = calculate_mapping_quality(score, read_length)
+                a.cigarstring = calculate_cigar(alignment_s, alignment_t)
             a.query_qualities = qual_scores
             
             samfile.write(a)
 
 if __name__ == "__main__":
     main()
```

### Comparing `bwalign-1.6.2/bwalign/utils.py` & `bwalign-1.6.3/bwalign/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,28 +146,30 @@
     """
     For each index in the seeds list, generates an affine alignment (50x50) for each seed index.
     By the end, returns position in ref and score of max scoring alignment. The alignment
     will be between the entire read and a length 50 segment of the reference starting at
     the calculated position. Version 2 of this function now also returns the alignments 
     themselves of the read and respective 50 base segment of the ref genome.
     """
+    if len(seed_idxes) == 0:
+        return None
     best_score = float('-inf')
     best_idx = -1
     best_seed = -1
     for i in range(0, len(seed_idxes)):
         for ref_idx in seed_idxes[i]:
             ref_segment = ref[ref_idx - i:ref_idx - i + read_length]
             score = banded_alignment(match_reward, mismatch_penalty, indel_penalty, band_width,
                                             ref_segment, read)
             if score > best_score:
                 best_score = score
                 best_idx = ref_idx
                 best_seed = i
     best_ref_seg = ref[best_idx - best_seed:best_idx - best_seed + read_length]
-    best_idx, s_align, t_align = BandedAlignmentWithBackTrack(match_reward, mismatch_penalty, indel_penalty, band_width,
+    _, s_align, t_align = BandedAlignmentWithBackTrack(match_reward, mismatch_penalty, indel_penalty, band_width,
                                                               best_ref_seg, read)
     return best_idx, best_score, s_align, t_align
 
 ### SEED GENERATION
 
 # SUFFIX ARRAY CONSTRUCTION
```

### Comparing `bwalign-1.6.2/bwalign.egg-info/PKG-INFO` & `bwalign-1.6.3/bwalign.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bwalign
-Version: 1.6.2
+Version: 1.6.3
 Summary: A burrows-wheeler seed and extend aligner
 Home-page: https://github.com/NabilHKhoury/bwalign
 Author: ['Adrian Layer, Nabil Khoury, Yasmin Jabir']
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `bwalign-1.6.2/setup.py` & `bwalign-1.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='bwalign',
-    version='1.6.2',    
+    version='1.6.3',    
     description='A burrows-wheeler seed and extend aligner',
     url='https://github.com/NabilHKhoury/bwalign',
     author=['Adrian Layer, Nabil Khoury, Yasmin Jabir'],
     license='MIT',
     packages=find_packages(),
     install_requires=['biopython',
                       'pysam',
```

