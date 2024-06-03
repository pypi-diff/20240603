# Comparing `tmp/bwalign-1.1.4.tar.gz` & `tmp/bwalign-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bwalign-1.1.4.tar", last modified: Mon Jun  3 01:32:27 2024, max compression
+gzip compressed data, was "bwalign-1.2.4.tar", last modified: Mon Jun  3 07:11:13 2024, max compression
```

## Comparing `bwalign-1.1.4.tar` & `bwalign-1.2.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 01:32:27.110718 bwalign-1.1.4/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      914 2024-06-03 01:32:27.109878 bwalign-1.1.4/PKG-INFO
--rw-r--r--   0 adrianlayer   (501) staff       (20)     1744 2024-05-29 18:41:22.000000 bwalign-1.1.4/README.md
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 01:32:27.102481 bwalign-1.1.4/bwalign/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      142 2024-06-03 01:32:16.000000 bwalign-1.1.4/bwalign/__init__.py
--rw-r--r--   0 adrianlayer   (501) staff       (20)     2007 2024-06-03 01:31:20.000000 bwalign-1.1.4/bwalign/main.py
--rw-r--r--   0 adrianlayer   (501) staff       (20)    20737 2024-06-03 01:30:46.000000 bwalign-1.1.4/bwalign/utils.py
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 01:32:27.108434 bwalign-1.1.4/bwalign.egg-info/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      914 2024-06-03 01:32:26.000000 bwalign-1.1.4/bwalign.egg-info/PKG-INFO
--rw-r--r--   0 adrianlayer   (501) staff       (20)      259 2024-06-03 01:32:27.000000 bwalign-1.1.4/bwalign.egg-info/SOURCES.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)        1 2024-06-03 01:32:26.000000 bwalign-1.1.4/bwalign.egg-info/dependency_links.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       46 2024-06-03 01:32:26.000000 bwalign-1.1.4/bwalign.egg-info/entry_points.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       16 2024-06-03 01:32:26.000000 bwalign-1.1.4/bwalign.egg-info/requires.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)        8 2024-06-03 01:32:26.000000 bwalign-1.1.4/bwalign.egg-info/top_level.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       38 2024-06-03 01:32:27.110871 bwalign-1.1.4/setup.cfg
--rw-r--r--   0 adrianlayer   (501) staff       (20)     1194 2024-06-03 01:32:12.000000 bwalign-1.1.4/setup.py
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 07:11:13.071480 bwalign-1.2.4/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      914 2024-06-03 07:11:13.069680 bwalign-1.2.4/PKG-INFO
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     1744 2024-05-29 18:41:22.000000 bwalign-1.2.4/README.md
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 07:11:13.059922 bwalign-1.2.4/bwalign/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      142 2024-06-03 07:10:59.000000 bwalign-1.2.4/bwalign/__init__.py
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     2007 2024-06-03 01:39:28.000000 bwalign-1.2.4/bwalign/main.py
+-rw-r--r--   0 adrianlayer   (501) staff       (20)    18798 2024-06-03 07:10:20.000000 bwalign-1.2.4/bwalign/utils.py
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 07:11:13.068310 bwalign-1.2.4/bwalign.egg-info/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      914 2024-06-03 07:11:12.000000 bwalign-1.2.4/bwalign.egg-info/PKG-INFO
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      259 2024-06-03 07:11:12.000000 bwalign-1.2.4/bwalign.egg-info/SOURCES.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)        1 2024-06-03 07:11:12.000000 bwalign-1.2.4/bwalign.egg-info/dependency_links.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       46 2024-06-03 07:11:12.000000 bwalign-1.2.4/bwalign.egg-info/entry_points.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       16 2024-06-03 07:11:12.000000 bwalign-1.2.4/bwalign.egg-info/requires.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)        8 2024-06-03 07:11:12.000000 bwalign-1.2.4/bwalign.egg-info/top_level.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       38 2024-06-03 07:11:13.071917 bwalign-1.2.4/setup.cfg
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     1194 2024-06-03 07:10:52.000000 bwalign-1.2.4/setup.py
```

### Comparing `bwalign-1.1.4/PKG-INFO` & `bwalign-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bwalign
-Version: 1.1.4
+Version: 1.2.4
 Summary: A burrows-wheeler seed and extend aligner
 Home-page: https://github.com/NabilHKhoury/bwalign
 Author: ['Adrian Layer, Nabil Khoury, Yasmin Jabir']
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `bwalign-1.1.4/README.md` & `bwalign-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `bwalign-1.1.4/bwalign/main.py` & `bwalign-1.2.4/bwalign/main.py`

 * *Files identical despite different names*

### Comparing `bwalign-1.1.4/bwalign/utils.py` & `bwalign-1.2.4/bwalign/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from Bio import SeqIO
-from typing import List, Tuple
-import sys
 import random
-import math
+import numpy as np
+
+### MAPPING QUALITY
 
 def calculate_mapping_quality(score, read_length):  
     max_possible_score = 2 * read_length
     
     if score < 0:
         return 0 
 
     if max_possible_score > 0:
         probability = score / max_possible_score
     else:
         probability = 0
 
     if probability > 0:
-        mapping_quality = -10 * math.log10(1 - probability)
+        mapping_quality = -10 * np.log10(1 - probability)
     else:
         mapping_quality = 0
 
     return min(int(mapping_quality), 60)
 
 ### CIGAR STRING CREATOR
 
@@ -55,134 +55,104 @@
     if ins > 0:
         cigar.append(f"{ins}I")
     if del_ > 0:
         cigar.append(f"{del_}D")
 
     return ''.join(cigar)
 
-### CIGAR STRING CREATOR
-
-def calculate_cigar(alignment_s, alignment_t):
-    cigar = []
-    match = 0
-    ins = 0
-    del_ = 0
-
-    for s, t in zip(alignment_s, alignment_t):
-        if s == '-' and t != '-':  #del in quer
-            if match > 0:
-                cigar.append(f"{match}M") 
-                match = 0
-            del_ += 1
-        elif s != '-' and t == '-':  #insertion
-            if match > 0:
-                cigar.append(f"{match}M")
-                match = 0
-            ins += 1
-        else:  # Match or mismatch
-            if ins > 0:
-                cigar.append(f"{ins}I")  
-                ins = 0
-            if del_ > 0:
-                cigar.append(f"{del_}D")
-                del_ = 0
-            match += 1
-
-    if match > 0:
-        cigar.append(f"{match}M")
-    if ins > 0:
-        cigar.append(f"{ins}I")
-    if del_ > 0:
-        cigar.append(f"{del_}D")
-
-    return ''.join(cigar)
-
 ### AFFINE ALIGNMENT
 
-def AffineAlignment(match_reward: int, mismatch_penalty: int,
+def affine_alignment(match_reward: int, mismatch_penalty: int,
                     gap_opening_penalty: int, gap_extension_penalty: int,
                     s: str, t: str) -> tuple[int, str, str]:
-    """Generates the affine alignment of two strings s and t."""
-    sys.setrecursionlimit(1500)
-    lower = [[0] * (len(t) + 1) for _ in range(len(s) + 1)] # insertions matrix
-    upper = [[0] * (len(t) + 1) for _ in range(len(s) + 1)] # deletions matrix
-    middle = [[0] * (len(t) + 1) for _ in range(len(s) + 1)] # match/mismatch matrix
-    b_lower = [[None] * (len(t)) for _ in range(len(s))] # backtrack insertions
-    b_upper = [[None] * (len(t)) for _ in range(len(s))] # backtrack deletions
-    b_middle = [[None] * (len(t)) for _ in range(len(s))] # backtrack ms/mms
-    for i in range(0, len(s) + 1):
-        for j in range(0, len(t) + 1):
-            # set base cases for middle using gap opening and extension penalties, base for lower and upper is -infinity.
-            if i == 0 and j == 0:
-                lower[i][j], upper[i][j] = float('-inf'), float('-inf')
-                continue
-            elif i == 0:
-                lower[i][j], middle[i][j] = float('-inf'), -gap_opening_penalty - ((j-1) * gap_extension_penalty)
-                continue
-            elif j == 0:
-                upper[i][j], middle[i][j] = float('-inf'), -gap_opening_penalty - ((i-1) * gap_extension_penalty)
-                continue
-            
-            # test for match
-            match = -mismatch_penalty
-            if s[i-1] == t[j-1]:
-                match = match_reward
-            
-            lower[i][j] = max(lower[i-1][j] - gap_extension_penalty, middle[i-1][j] - gap_opening_penalty)
-            upper[i][j] = max(upper[i][j-1] - gap_extension_penalty, middle[i][j-1] - gap_opening_penalty)
-            middle[i][j] = max(lower[i][j], upper[i][j], middle[i-1][j-1] + match)
-            if lower[i][j] == lower[i-1][j] - gap_extension_penalty:
-                b_lower[i-1][j-1] = 'd'
-            elif lower[i][j] == middle[i-1][j] - gap_opening_penalty:
-                b_lower[i-1][j-1] = 'open'
-            if upper[i][j] == upper[i][j-1] - gap_extension_penalty:
-                b_upper[i-1][j-1] = 'r'
-            elif upper[i][j] == middle[i][j-1] - gap_opening_penalty:
-                b_upper[i-1][j-1] = 'open'
-            if middle[i][j] == lower[i][j]:
-                b_middle[i-1][j-1] = 'in_close'
-            elif middle[i][j] == upper[i][j]:
-                b_middle[i-1][j-1] = 'del_close'
-            elif middle[i][j] == middle[i-1][j-1] + match:
-                b_middle[i-1][j-1] = 'dr'
-    s_align, t_align = backtrack(s, t, b_lower, b_upper, b_middle, len(s) - 1, len(t) - 1, 'middle')
-    return max(lower[len(s)][len(t)], middle[len(s)][len(t)], upper[len(s)][len(t)]), s_align, t_align
-                
-def backtrack(s: str, t: str, b_lower: list[list[str]], b_upper: list[list[str]], b_middle: list[list[str]], i: int, j: int, LEVEL: str) -> tuple[str,str]:
-    if i < 0 and j < 0: # if both i and j reach -1 at the same time, we can just return empty string.
-        return '',''
-    elif i < 0: # if i reaches -1 first, need to append the rest of t up to index j to t prime, and a number of '-' equal to the length of that string to s prime.
-        return '-' * (j + 1), t[0:j+1]
-    elif j < 0: # same as i < 0 condition but for j.
-        return s[0:i+1], '-' * (i + 1)
-    # my use of the LEVEL variable tells us which matrix this call is backtracking in.
-    if LEVEL == 'middle':
-        if b_middle[i][j] == 'in_close':
-            s_prime, t_prime = backtrack(s, t, b_lower, b_upper, b_middle, i, j, 'lower')
-            return s_prime, t_prime
-        elif b_middle[i][j] == 'del_close':
-            s_prime, t_prime = backtrack(s, t, b_lower, b_upper, b_middle, i, j, 'upper')
-            return s_prime, t_prime
-        elif b_middle[i][j] == 'dr':
-            s_prime, t_prime = backtrack(s, t, b_lower, b_upper, b_middle, i-1, j-1, 'middle')
-            return s_prime + s[i], t_prime + t[j]
-    elif LEVEL == 'lower':
-        if b_lower[i][j] == 'd':
-            s_prime, t_prime = backtrack(s, t, b_lower, b_upper, b_middle, i-1, j, 'lower')
-            return s_prime + s[i], t_prime + '-'
-        elif b_lower[i][j] == 'open':
-            s_prime, t_prime = backtrack(s, t, b_lower, b_upper, b_middle, i-1, j, 'middle')
-            return s_prime + s[i], t_prime + '-'
-    elif LEVEL == 'upper':
-        if b_upper[i][j] == 'r':
-            s_prime, t_prime = backtrack(s, t, b_lower, b_upper, b_middle, i, j-1, 'upper')
-            return s_prime + '-', t_prime + t[j]
-        elif b_upper[i][j] == 'open':
-            s_prime, t_prime = backtrack(s, t, b_lower, b_upper, b_middle, i, j-1, 'middle')
-            return s_prime + '-', t_prime + t[j]
+    len_s, len_t = len(s), len(t)
+
+    # Initialize matrices
+    lower = np.full((len_s + 1, len_t + 1),float('-inf'))#was -inf
+    middle = np.full((len_s + 1, len_t + 1),float('-inf'))
+    upper = np.full((len_s + 1, len_t + 1),float('-inf'))
+    middle[0, 0] = 0  # Starting point
+    lower[0,0] = float('-inf')#-gap_opening_penalty
+    upper[0,0] = float('-inf')#-gap_opening_penalty
+    backtrack = []
+
+    #initialize backtrack:
+    for i in range(len(s)+1):
+        row = []
+        for j in range(len(t)+1):
+            row.append("")
+        backtrack.append(row)
+
+    # Initialize the first row and column of the middle matrix to account for leading gaps
+    # Initialize the first row of the upper matrix and the first column of the lower matrix
+    for i in range(1, len_s + 1):
+        lower[i, 0] = 0 - ((i - 1) * gap_extension_penalty) - gap_opening_penalty
+        middle[i, 0] = 0 - ((i - 1) * gap_extension_penalty) - gap_opening_penalty
+        upper[i, 0] = 0 - ((i - 1) * gap_extension_penalty) - 2*gap_opening_penalty #rem *2
+        backtrack[i][0] = 'up'               
+    # No need to initialize `middle[i, 0]` here since it's already done above
+
+    for j in range(1, len_t + 1):
+        upper[0, j] = 0 - (j - 1) * gap_extension_penalty - gap_opening_penalty
+        lower[0, j] = 0 - ((j - 1) * gap_extension_penalty) - 2*gap_opening_penalty#remived x2
+        middle[0, j] = 0 - (j - 1) * gap_extension_penalty - gap_opening_penalty
+        backtrack[0][j] = 'left'
+
+    # Fill in the matrices based on the recursive formulas
+    for i in range(1, len_s + 1):
+        for j in range(1, len_t + 1):
+            char_s = s[i-1]
+            char_t = t[j-1]
+
+            # Calculate scores for each matrix
+            lower[i, j] = max(lower[i-1, j] - gap_extension_penalty,
+                          middle[i-1, j] - gap_opening_penalty)
+
+            # Update upper matrix: Max of extending a gap from upper or opening a new gap from middle
+            upper[i, j] = max(upper[i, j-1] - gap_extension_penalty,
+                              middle[i, j-1] - gap_opening_penalty)
+
+            # Update middle matrix: Max of diagonal move (match/mismatch), ending a gap from lower or upper
+            middle[i, j] = max(middle[i-1, j-1] + (match_reward if s[i-1] == t[j-1] else -mismatch_penalty),
+                               lower[i, j],
+                               upper[i, j])
+
+            #do Backtrack
+            if(middle[i, j] == middle[i-1, j-1] - mismatch_penalty):
+                backtrack[i][j] = "diag"
+            elif(middle[i, j] == upper[i,j]):
+                backtrack[i][j] = "left"
+            elif(middle[i, j] == lower[i,j]):
+                backtrack[i][j] = "up"
+            elif(middle[i, j] == middle[i-1, j-1] + match_reward):
+                backtrack[i][j] = "diag"
+
+
+
+    # Traceback to find the optimal alignment
+    alignment_s = ""
+    alignment_t = ""
+    i, j = len_s, len_t
+
+    while i > 0 or j > 0:
+        if backtrack[i][j] == 'diag' and i > 0 and j > 0 :
+            alignment_s = s[i-1] + alignment_s
+            alignment_t = t[j-1] + alignment_t
+            i, j = i-1, j-1
+        elif backtrack[i][j] == 'up' and i > 0:
+            alignment_s = s[i-1] + alignment_s
+            alignment_t = '-' + alignment_t
+            i -= 1
+        elif backtrack[i][j] == 'left' and j > 0:
+            alignment_s = '-' + alignment_s
+            alignment_t = t[j-1] + alignment_t
+            j -= 1
+
+    # Return the score of the best alignment and the alignments themselves
+    return int(middle[len_s, len_t]), alignment_s, alignment_t
 
 ### SEED EXTENSION
 
 def compute_max_seed(ref: str, read: str, seed_idxes: list[list[int]],
                      match_reward: int, mismatch_penalty: int,
                      gap_opening_penalty: int, gap_extension_penalty: int,
                      read_length: int) -> tuple[int, int, str, str]:
@@ -196,15 +166,15 @@
     best_score = float('-inf')
     best_idx = -1
     s_best_align = ''
     t_best_align = ''
     for i in range(0, len(seed_idxes)):
         for ref_idx in seed_idxes[i]:
             ref_segment = ref[ref_idx - i:ref_idx - i + read_length]
-            score, s_align, t_align, = AffineAlignment(match_reward, mismatch_penalty, 
+            score, s_align, t_align, = affine_alignment(match_reward, mismatch_penalty, 
                                             gap_opening_penalty, gap_extension_penalty,
                                             ref_segment, read)
             if score > best_score:
                 best_score = score
                 best_idx = ref_idx
                 s_best_align = s_align
                 t_best_align = t_align
@@ -310,15 +280,15 @@
     for idx in sa:
         if sa[idx] % k == 0:
             partial[idx] = sa[idx]
     return partial
 
 ## BWT creation
 
-def bwt_from_suffix_array(text: str, suffix_array: List[int]) -> str:
+def bwt_from_suffix_array(text: str, suffix_array: list[int]) -> str:
     bwt = []
     for idx in suffix_array:
         bwt.append(text[idx-1])
     return ''.join(bwt)
 
 def bwt_psa_out(text: str, k: int) -> tuple[str, dict[int, int]]:
     sa = suffix_array(text)
@@ -435,29 +405,29 @@
         start, end = bw_better_match_pattern(bwt, kmer, first_occurrences, checkpoint_arrs)
         idxes = compute_idxes_from_top_bot(start, end, psa, bwt, ranks, first_occurrences)
         seed_idxes.append(idxes)
     return seed_idxes
 
 ### FASTQ PARSING
 
-def parse_fastq(fastq_path: str) -> List[Tuple[str, str, List[int]]]:
+def parse_fastq(fastq_path: str) -> list[tuple[str, str, list[int]]]:
     """
     Parse a FASTQ file and return a list of tuples where each tuple contains the
     sequence ID, the sequence itself, and the quality scores.
     
     :param fastq_path: Path to the FASTQ file
     :return: A list of tuples where each tuple contains the sequence ID, the sequence itself, and the quality scores
     """
     fastq_list = []
     with open(fastq_path, "r") as handle:
         for record in SeqIO.parse(handle, "fastq"):
             fastq_list.append((record.id, str(record.seq), record.letter_annotations["phred_quality"]))
     return fastq_list
 
-def parse_reference_genome(fasta_path: str) -> Tuple[str, str]:
+def parse_reference_genome(fasta_path: str) -> tuple[str, str]:
     """
     Parse a FASTA file containing a reference genome and return a tuple containing
     the sequence ID and the sequence itself.
 
     :param fasta_path: Path to the FASTA file
     :return: A tuple containing the sequence ID and the sequence itself
     """
@@ -470,15 +440,15 @@
     Generate a random DNA sequence of the specified length.
 
     :param length: The length of the sequence
     :return: A random DNA sequence
     """
     return ''.join(random.choices('ACGT', k=length))
 
-def random_quality_scores(length: int) -> List[int]:
+def random_quality_scores(length: int) -> list[int]:
     """
     Generate random quality scores for a sequence of the specified length.
 
     :param length: The length of the sequence
     :return: A list of random quality scores
     """
     return ''.join(random.choices('!"#$%&\'()*+,-./0123456789:;<=>?@ABCDEFGHI', k=length))
```

### Comparing `bwalign-1.1.4/bwalign.egg-info/PKG-INFO` & `bwalign-1.2.4/bwalign.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bwalign
-Version: 1.1.4
+Version: 1.2.4
 Summary: A burrows-wheeler seed and extend aligner
 Home-page: https://github.com/NabilHKhoury/bwalign
 Author: ['Adrian Layer, Nabil Khoury, Yasmin Jabir']
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `bwalign-1.1.4/setup.py` & `bwalign-1.2.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='bwalign',
-    version='1.1.4',    
+    version='1.2.4',    
     description='A burrows-wheeler seed and extend aligner',
     url='https://github.com/NabilHKhoury/bwalign',
     author=['Adrian Layer, Nabil Khoury, Yasmin Jabir'],
     license='MIT',
     packages=find_packages(),
     install_requires=['biopython',
                       'pysam',
```

