# Comparing `tmp/bwalign-1.3.7.tar.gz` & `tmp/bwalign-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bwalign-1.3.7.tar", last modified: Mon Jun  3 09:24:16 2024, max compression
+gzip compressed data, was "bwalign-1.4.7.tar", last modified: Mon Jun  3 09:48:01 2024, max compression
```

## Comparing `bwalign-1.3.7.tar` & `bwalign-1.4.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 09:24:16.763116 bwalign-1.3.7/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 09:24:16.762039 bwalign-1.3.7/PKG-INFO
--rw-r--r--   0 adrianlayer   (501) staff       (20)     1744 2024-05-29 18:41:22.000000 bwalign-1.3.7/README.md
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 09:24:16.754275 bwalign-1.3.7/bwalign/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      142 2024-06-03 09:23:54.000000 bwalign-1.3.7/bwalign/__init__.py
--rw-r--r--   0 adrianlayer   (501) staff       (20)     2036 2024-06-03 09:23:45.000000 bwalign-1.3.7/bwalign/main.py
--rw-r--r--   0 adrianlayer   (501) staff       (20)    18798 2024-06-03 07:10:20.000000 bwalign-1.3.7/bwalign/utils.py
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 09:24:16.760258 bwalign-1.3.7/bwalign.egg-info/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 09:24:16.000000 bwalign-1.3.7/bwalign.egg-info/PKG-INFO
--rw-r--r--   0 adrianlayer   (501) staff       (20)      259 2024-06-03 09:24:16.000000 bwalign-1.3.7/bwalign.egg-info/SOURCES.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)        1 2024-06-03 09:24:16.000000 bwalign-1.3.7/bwalign.egg-info/dependency_links.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       46 2024-06-03 09:24:16.000000 bwalign-1.3.7/bwalign.egg-info/entry_points.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       21 2024-06-03 09:24:16.000000 bwalign-1.3.7/bwalign.egg-info/requires.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)        8 2024-06-03 09:24:16.000000 bwalign-1.3.7/bwalign.egg-info/top_level.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       38 2024-06-03 09:24:16.763261 bwalign-1.3.7/setup.cfg
--rw-r--r--   0 adrianlayer   (501) staff       (20)     1224 2024-06-03 09:23:51.000000 bwalign-1.3.7/setup.py
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 09:48:01.316744 bwalign-1.4.7/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 09:48:01.315899 bwalign-1.4.7/PKG-INFO
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     1744 2024-05-29 18:41:22.000000 bwalign-1.4.7/README.md
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 09:48:01.306857 bwalign-1.4.7/bwalign/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      142 2024-06-03 09:47:58.000000 bwalign-1.4.7/bwalign/__init__.py
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     2037 2024-06-03 09:46:02.000000 bwalign-1.4.7/bwalign/main.py
+-rw-r--r--   0 adrianlayer   (501) staff       (20)    17425 2024-06-03 09:47:15.000000 bwalign-1.4.7/bwalign/utils.py
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 09:48:01.314506 bwalign-1.4.7/bwalign.egg-info/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 09:48:01.000000 bwalign-1.4.7/bwalign.egg-info/PKG-INFO
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      259 2024-06-03 09:48:01.000000 bwalign-1.4.7/bwalign.egg-info/SOURCES.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)        1 2024-06-03 09:48:01.000000 bwalign-1.4.7/bwalign.egg-info/dependency_links.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       46 2024-06-03 09:48:01.000000 bwalign-1.4.7/bwalign.egg-info/entry_points.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       21 2024-06-03 09:48:01.000000 bwalign-1.4.7/bwalign.egg-info/requires.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)        8 2024-06-03 09:48:01.000000 bwalign-1.4.7/bwalign.egg-info/top_level.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       38 2024-06-03 09:48:01.317384 bwalign-1.4.7/setup.cfg
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     1224 2024-06-03 09:47:55.000000 bwalign-1.4.7/setup.py
```

### Comparing `bwalign-1.3.7/PKG-INFO` & `bwalign-1.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bwalign
-Version: 1.3.7
+Version: 1.4.7
 Summary: A burrows-wheeler seed and extend aligner
 Home-page: https://github.com/NabilHKhoury/bwalign
 Author: ['Adrian Layer, Nabil Khoury, Yasmin Jabir']
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `bwalign-1.3.7/README.md` & `bwalign-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `bwalign-1.3.7/bwalign/main.py` & `bwalign-1.4.7/bwalign/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     }
     
     #write to sam FILE
     with pysam.AlignmentFile("output.sam", "w", header=header) as samfile:
         for read_id, read_seq, qual_scores in tqdm(reads):
             
             seed_idxes = generate_seeds(str(read_seq), bwt, 19, psa, first_occurrences, checkpoint_arrs, ranks)
-            best_idx, score, alignment_s, alignment_t = compute_max_seed(str(reference), str(read_seq), seed_idxes, 2, 1, 2, 1, read_length)
+            best_idx, score, alignment_s, alignment_t = compute_max_seed(str(reference), str(read_seq), seed_idxes, 2, 2, 2, 10, read_length)
 
             #create a SAM entry for the aligned read
             a = pysam.AlignedSegment()
             a.query_name = read_id
             a.query_sequence = read_seq
             a.flag = 0
             a.reference_id = 0
```

### Comparing `bwalign-1.3.7/bwalign/utils.py` & `bwalign-1.4.7/bwalign/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from Bio import SeqIO
 import random
 import numpy as np
+import sys
 
 ### MAPPING QUALITY
 
 def calculate_mapping_quality(score, read_length):  
     max_possible_score = 2 * read_length
     
     if score < 0:
@@ -57,108 +58,68 @@
     if del_ > 0:
         cigar.append(f"{del_}D")
 
     return ''.join(cigar)
 
 ### AFFINE ALIGNMENT
 
-def affine_alignment(match_reward: int, mismatch_penalty: int,
-                    gap_opening_penalty: int, gap_extension_penalty: int,
-                    s: str, t: str) -> tuple[int, str, str]:
-    len_s, len_t = len(s), len(t)
-
-    # Initialize matrices
-    lower = np.full((len_s + 1, len_t + 1),float('-inf'))#was -inf
-    middle = np.full((len_s + 1, len_t + 1),float('-inf'))
-    upper = np.full((len_s + 1, len_t + 1),float('-inf'))
-    middle[0, 0] = 0  # Starting point
-    lower[0,0] = float('-inf')#-gap_opening_penalty
-    upper[0,0] = float('-inf')#-gap_opening_penalty
-    backtrack = []
-
-    #initialize backtrack:
-    for i in range(len(s)+1):
-        row = []
-        for j in range(len(t)+1):
-            row.append("")
-        backtrack.append(row)
-
-    # Initialize the first row and column of the middle matrix to account for leading gaps
-    # Initialize the first row of the upper matrix and the first column of the lower matrix
-    for i in range(1, len_s + 1):
-        lower[i, 0] = 0 - ((i - 1) * gap_extension_penalty) - gap_opening_penalty
-        middle[i, 0] = 0 - ((i - 1) * gap_extension_penalty) - gap_opening_penalty
-        upper[i, 0] = 0 - ((i - 1) * gap_extension_penalty) - 2*gap_opening_penalty #rem *2
-        backtrack[i][0] = 'up'               
-    # No need to initialize `middle[i, 0]` here since it's already done above
-
-    for j in range(1, len_t + 1):
-        upper[0, j] = 0 - (j - 1) * gap_extension_penalty - gap_opening_penalty
-        lower[0, j] = 0 - ((j - 1) * gap_extension_penalty) - 2*gap_opening_penalty#remived x2
-        middle[0, j] = 0 - (j - 1) * gap_extension_penalty - gap_opening_penalty
-        backtrack[0][j] = 'left'
-
-    # Fill in the matrices based on the recursive formulas
-    for i in range(1, len_s + 1):
-        for j in range(1, len_t + 1):
-            char_s = s[i-1]
-            char_t = t[j-1]
-
-            # Calculate scores for each matrix
-            lower[i, j] = max(lower[i-1, j] - gap_extension_penalty,
-                          middle[i-1, j] - gap_opening_penalty)
-
-            # Update upper matrix: Max of extending a gap from upper or opening a new gap from middle
-            upper[i, j] = max(upper[i, j-1] - gap_extension_penalty,
-                              middle[i, j-1] - gap_opening_penalty)
-
-            # Update middle matrix: Max of diagonal move (match/mismatch), ending a gap from lower or upper
-            middle[i, j] = max(middle[i-1, j-1] + (match_reward if s[i-1] == t[j-1] else -mismatch_penalty),
-                               lower[i, j],
-                               upper[i, j])
-
-            #do Backtrack
-            if(middle[i, j] == middle[i-1, j-1] - mismatch_penalty):
-                backtrack[i][j] = "diag"
-            elif(middle[i, j] == upper[i,j]):
-                backtrack[i][j] = "left"
-            elif(middle[i, j] == lower[i,j]):
-                backtrack[i][j] = "up"
-            elif(middle[i, j] == middle[i-1, j-1] + match_reward):
-                backtrack[i][j] = "diag"
-
-
-
-    # Traceback to find the optimal alignment
-    alignment_s = ""
-    alignment_t = ""
-    i, j = len_s, len_t
-
-    while i > 0 or j > 0:
-        if backtrack[i][j] == 'diag' and i > 0 and j > 0 :
-            alignment_s = s[i-1] + alignment_s
-            alignment_t = t[j-1] + alignment_t
-            i, j = i-1, j-1
-        elif backtrack[i][j] == 'up' and i > 0:
-            alignment_s = s[i-1] + alignment_s
-            alignment_t = '-' + alignment_t
-            i -= 1
-        elif backtrack[i][j] == 'left' and j > 0:
-            alignment_s = '-' + alignment_s
-            alignment_t = t[j-1] + alignment_t
-            j -= 1
-
-    # Return the score of the best alignment and the alignments themselves
-    return int(middle[len_s, len_t]), alignment_s, alignment_t
+def BandedAlignment(match_reward: int, mismatch_penalty: int, indel_penalty: int,
+                    band_parameter: int, s: str, t: str) -> tuple[int, str, str]:
+    sys.setrecursionlimit(1500)
+    l = [[float('-inf')] * (len(t) + 1) for _ in range(len(s) + 1)] # score matrix
+    b = [[None] * (len(t)) for _ in range(len(s))] # backtrack matrix
+    for i in range(0, len(s) + 1):
+        for j in range(0, len(t) + 1):
+            if i == 0 and j == 0:
+                l[i][j] = 0
+            if i == 0:
+                l[i][j] = j * (-indel_penalty) # in this case, an empty string s has j indels with t.
+                continue
+            if j == 0:
+                l[i][j] = i * (-indel_penalty)
+                continue
+            if abs(j-i) < band_parameter:
+                match = -mismatch_penalty
+                if s[i-1] == t[j-1]:
+                    match = match_reward
+                l[i][j] = max(l[i-1][j] - indel_penalty, l[i][j-1] - indel_penalty, l[i-1][j-1] + match)
+                if l[i][j] == l[i-1][j] - indel_penalty:
+                    b[i-1][j-1] = 'd'
+                elif l[i][j] == l[i][j-1] - indel_penalty:
+                    b[i-1][j-1] = 'r'
+                elif l[i][j] == l[i-1][j-1] + match:
+                    b[i-1][j-1] = 'dr'
+            else:
+                continue
+    s_align, t_align = backtrack(b, s, t, len(s) - 1, len(t) - 1, band_parameter)
+    return l[len(s)][len(t)], s_align, t_align
+
+def backtrack(b: list[list[str]], s: str, t: str, i: int, j: int, band_parameter: int) -> tuple[str, str]:
+    """Traces alignment using backtracking matrix b."""
+    if i < 0 and j < 0: # if both i and j reach -1 at the same time, we can just return empty string.
+        return '',''
+    elif i < 0: # if i reaches -1 first, need to append the rest of t up to index j to t prime, and a number of '-' equal to the length of that string to s prime.
+        return '-' * (j + 1), t[0:j+1]
+    elif j < 0: # same as i < 0 condition but for j.
+        return s[0:i+1], '-' * (i + 1)
+    elif b[i][j] == 'd' and abs(j-i) < band_parameter:
+        s_prime, t_prime = backtrack(b, s, t, i-1, j, band_parameter)
+        return s_prime + s[i], t_prime + '-'
+    elif b[i][j] == 'r' and abs(j-i) < band_parameter:
+        s_prime, t_prime = backtrack(b, s, t, i, j-1, band_parameter)
+        return s_prime + '-', t_prime + t[j]
+    else:
+        s_prime, t_prime = backtrack(b, s, t, i-1, j-1, band_parameter)
+        return s_prime + s[i], t_prime + t[j]
 
 ### SEED EXTENSION
 
 def compute_max_seed(ref: str, read: str, seed_idxes: list[list[int]],
                      match_reward: int, mismatch_penalty: int,
-                     gap_opening_penalty: int, gap_extension_penalty: int,
+                     indel_penalty: int, band_width: int,
                      read_length: int) -> tuple[int, int, str, str]:
     """
     For each index in the seeds list, generates an affine alignment (50x50) for each seed index.
     By the end, returns position in ref and score of max scoring alignment. The alignment
     will be between the entire read and a length 50 segment of the reference starting at
     the calculated position. Version 2 of this function now also returns the alignments 
     themselves of the read and respective 50 base segment of the ref genome.
@@ -166,16 +127,15 @@
     best_score = float('-inf')
     best_idx = -1
     s_best_align = ''
     t_best_align = ''
     for i in range(0, len(seed_idxes)):
         for ref_idx in seed_idxes[i]:
             ref_segment = ref[ref_idx - i:ref_idx - i + read_length]
-            score, s_align, t_align, = affine_alignment(match_reward, mismatch_penalty, 
-                                            gap_opening_penalty, gap_extension_penalty,
+            score, s_align, t_align, = BandedAlignment(match_reward, mismatch_penalty, indel_penalty, band_width,
                                             ref_segment, read)
             if score > best_score:
                 best_score = score
                 best_idx = ref_idx
                 s_best_align = s_align
                 t_best_align = t_align
     return best_idx, best_score, s_best_align, t_best_align
```

### Comparing `bwalign-1.3.7/bwalign.egg-info/PKG-INFO` & `bwalign-1.4.7/bwalign.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bwalign
-Version: 1.3.7
+Version: 1.4.7
 Summary: A burrows-wheeler seed and extend aligner
 Home-page: https://github.com/NabilHKhoury/bwalign
 Author: ['Adrian Layer, Nabil Khoury, Yasmin Jabir']
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `bwalign-1.3.7/setup.py` & `bwalign-1.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='bwalign',
-    version='1.3.7',    
+    version='1.4.7',    
     description='A burrows-wheeler seed and extend aligner',
     url='https://github.com/NabilHKhoury/bwalign',
     author=['Adrian Layer, Nabil Khoury, Yasmin Jabir'],
     license='MIT',
     packages=find_packages(),
     install_requires=['biopython',
                       'pysam',
```

