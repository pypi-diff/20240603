# Comparing `tmp/bwalign-1.4.7.tar.gz` & `tmp/bwalign-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bwalign-1.4.7.tar", last modified: Mon Jun  3 09:48:01 2024, max compression
+gzip compressed data, was "bwalign-1.5.7.tar", last modified: Mon Jun  3 10:19:47 2024, max compression
```

## Comparing `bwalign-1.4.7.tar` & `bwalign-1.5.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 09:48:01.316744 bwalign-1.4.7/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 09:48:01.315899 bwalign-1.4.7/PKG-INFO
--rw-r--r--   0 adrianlayer   (501) staff       (20)     1744 2024-05-29 18:41:22.000000 bwalign-1.4.7/README.md
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 09:48:01.306857 bwalign-1.4.7/bwalign/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      142 2024-06-03 09:47:58.000000 bwalign-1.4.7/bwalign/__init__.py
--rw-r--r--   0 adrianlayer   (501) staff       (20)     2037 2024-06-03 09:46:02.000000 bwalign-1.4.7/bwalign/main.py
--rw-r--r--   0 adrianlayer   (501) staff       (20)    17425 2024-06-03 09:47:15.000000 bwalign-1.4.7/bwalign/utils.py
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 09:48:01.314506 bwalign-1.4.7/bwalign.egg-info/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 09:48:01.000000 bwalign-1.4.7/bwalign.egg-info/PKG-INFO
--rw-r--r--   0 adrianlayer   (501) staff       (20)      259 2024-06-03 09:48:01.000000 bwalign-1.4.7/bwalign.egg-info/SOURCES.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)        1 2024-06-03 09:48:01.000000 bwalign-1.4.7/bwalign.egg-info/dependency_links.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       46 2024-06-03 09:48:01.000000 bwalign-1.4.7/bwalign.egg-info/entry_points.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       21 2024-06-03 09:48:01.000000 bwalign-1.4.7/bwalign.egg-info/requires.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)        8 2024-06-03 09:48:01.000000 bwalign-1.4.7/bwalign.egg-info/top_level.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       38 2024-06-03 09:48:01.317384 bwalign-1.4.7/setup.cfg
--rw-r--r--   0 adrianlayer   (501) staff       (20)     1224 2024-06-03 09:47:55.000000 bwalign-1.4.7/setup.py
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 10:19:47.849565 bwalign-1.5.7/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 10:19:47.848808 bwalign-1.5.7/PKG-INFO
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     1744 2024-05-29 18:41:22.000000 bwalign-1.5.7/README.md
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 10:19:47.840550 bwalign-1.5.7/bwalign/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      142 2024-06-03 10:19:36.000000 bwalign-1.5.7/bwalign/__init__.py
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     2037 2024-06-03 09:46:02.000000 bwalign-1.5.7/bwalign/main.py
+-rw-r--r--   0 adrianlayer   (501) staff       (20)    18374 2024-06-03 10:18:37.000000 bwalign-1.5.7/bwalign/utils.py
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 10:19:47.847791 bwalign-1.5.7/bwalign.egg-info/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 10:19:47.000000 bwalign-1.5.7/bwalign.egg-info/PKG-INFO
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      259 2024-06-03 10:19:47.000000 bwalign-1.5.7/bwalign.egg-info/SOURCES.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)        1 2024-06-03 10:19:47.000000 bwalign-1.5.7/bwalign.egg-info/dependency_links.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       46 2024-06-03 10:19:47.000000 bwalign-1.5.7/bwalign.egg-info/entry_points.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       21 2024-06-03 10:19:47.000000 bwalign-1.5.7/bwalign.egg-info/requires.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)        8 2024-06-03 10:19:47.000000 bwalign-1.5.7/bwalign.egg-info/top_level.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       38 2024-06-03 10:19:47.851764 bwalign-1.5.7/setup.cfg
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     1224 2024-06-03 10:19:34.000000 bwalign-1.5.7/setup.py
```

### Comparing `bwalign-1.4.7/PKG-INFO` & `bwalign-1.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bwalign
-Version: 1.4.7
+Version: 1.5.7
 Summary: A burrows-wheeler seed and extend aligner
 Home-page: https://github.com/NabilHKhoury/bwalign
 Author: ['Adrian Layer, Nabil Khoury, Yasmin Jabir']
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `bwalign-1.4.7/README.md` & `bwalign-1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `bwalign-1.4.7/bwalign/main.py` & `bwalign-1.5.7/bwalign/main.py`

 * *Files identical despite different names*

### Comparing `bwalign-1.4.7/bwalign/utils.py` & `bwalign-1.5.7/bwalign/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,17 +56,39 @@
     if ins > 0:
         cigar.append(f"{ins}I")
     if del_ > 0:
         cigar.append(f"{del_}D")
 
     return ''.join(cigar)
 
-### AFFINE ALIGNMENT
+### BANDED ALIGNMENT
 
-def BandedAlignment(match_reward: int, mismatch_penalty: int, indel_penalty: int,
+def banded_alignment(mr: int, mmp: int, indp: int, bp: int, s: str, t: str) -> int:
+    l = np.full((len(s)+1,len(t)+1), -np.inf)
+    for i in range(0, len(s) + 1):
+        for j in range(0, len(t) + 1):
+            if i == 0 and j == 0:
+                l[i,j] = 0
+                continue
+            elif i == 0:
+                l[i,j] = j * (-indp)
+                continue
+            elif j == 0:
+                l[i,j] = i * (-indp)
+                continue
+            if abs(j-i) < bp:
+                match = -mmp
+                if s[i-1] == t[j-1]:
+                    match = mr
+                l[i,j] = max(l[i-1][j] - indp, l[i][j-1] - indp, l[i-1][j-1] + match)
+            else:
+                continue
+    return int(l[len(s),len(t)])
+
+def BandedAlignmentWithBackTrack(match_reward: int, mismatch_penalty: int, indel_penalty: int,
                     band_parameter: int, s: str, t: str) -> tuple[int, str, str]:
     sys.setrecursionlimit(1500)
     l = [[float('-inf')] * (len(t) + 1) for _ in range(len(s) + 1)] # score matrix
     b = [[None] * (len(t)) for _ in range(len(s))] # backtrack matrix
     for i in range(0, len(s) + 1):
         for j in range(0, len(t) + 1):
             if i == 0 and j == 0:
@@ -122,27 +144,28 @@
     By the end, returns position in ref and score of max scoring alignment. The alignment
     will be between the entire read and a length 50 segment of the reference starting at
     the calculated position. Version 2 of this function now also returns the alignments 
     themselves of the read and respective 50 base segment of the ref genome.
     """
     best_score = float('-inf')
     best_idx = -1
-    s_best_align = ''
-    t_best_align = ''
+    best_seed = -1
     for i in range(0, len(seed_idxes)):
         for ref_idx in seed_idxes[i]:
             ref_segment = ref[ref_idx - i:ref_idx - i + read_length]
-            score, s_align, t_align, = BandedAlignment(match_reward, mismatch_penalty, indel_penalty, band_width,
+            score = banded_alignment(match_reward, mismatch_penalty, indel_penalty, band_width,
                                             ref_segment, read)
             if score > best_score:
                 best_score = score
                 best_idx = ref_idx
-                s_best_align = s_align
-                t_best_align = t_align
-    return best_idx, best_score, s_best_align, t_best_align
+                best_seed = i
+    best_ref_seg = ref[best_idx - best_seed:best_idx - best_seed + read_length]
+    best_idx, s_align, t_align = BandedAlignmentWithBackTrack(match_reward, mismatch_penalty, indel_penalty, band_width,
+                                                              best_ref_seg, read)
+    return best_idx, best_score, s_align, t_align
 
 ### SEED GENERATION
 
 # SUFFIX ARRAY CONSTRUCTION
 
 class suffix:
     """
```

### Comparing `bwalign-1.4.7/bwalign.egg-info/PKG-INFO` & `bwalign-1.5.7/bwalign.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bwalign
-Version: 1.4.7
+Version: 1.5.7
 Summary: A burrows-wheeler seed and extend aligner
 Home-page: https://github.com/NabilHKhoury/bwalign
 Author: ['Adrian Layer, Nabil Khoury, Yasmin Jabir']
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `bwalign-1.4.7/setup.py` & `bwalign-1.5.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='bwalign',
-    version='1.4.7',    
+    version='1.5.7',    
     description='A burrows-wheeler seed and extend aligner',
     url='https://github.com/NabilHKhoury/bwalign',
     author=['Adrian Layer, Nabil Khoury, Yasmin Jabir'],
     license='MIT',
     packages=find_packages(),
     install_requires=['biopython',
                       'pysam',
```

