# Comparing `tmp/bwalign-0.1.0.tar.gz` & `tmp/bwalign-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bwalign-0.1.0.tar", last modified: Wed May 29 18:18:13 2024, max compression
+gzip compressed data, was "bwalign-1.0.0.tar", last modified: Mon Jun  3 00:02:39 2024, max compression
```

## Comparing `bwalign-0.1.0.tar` & `bwalign-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-05-29 18:18:13.175334 bwalign-0.1.0/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      914 2024-05-29 18:18:13.174456 bwalign-0.1.0/PKG-INFO
--rw-r--r--   0 adrianlayer   (501) staff       (20)     1570 2024-05-27 22:52:45.000000 bwalign-0.1.0/README.md
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-05-29 18:18:13.166648 bwalign-0.1.0/bwalign/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      142 2024-05-29 18:17:36.000000 bwalign-0.1.0/bwalign/__init__.py
--rw-r--r--   0 adrianlayer   (501) staff       (20)     2079 2024-05-29 18:09:28.000000 bwalign-0.1.0/bwalign/main.py
--rw-r--r--   0 adrianlayer   (501) staff       (20)    17467 2024-05-29 18:14:57.000000 bwalign-0.1.0/bwalign/utils.py
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-05-29 18:18:13.173301 bwalign-0.1.0/bwalign.egg-info/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      914 2024-05-29 18:18:13.000000 bwalign-0.1.0/bwalign.egg-info/PKG-INFO
--rw-r--r--   0 adrianlayer   (501) staff       (20)      259 2024-05-29 18:18:13.000000 bwalign-0.1.0/bwalign.egg-info/SOURCES.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)        1 2024-05-29 18:18:13.000000 bwalign-0.1.0/bwalign.egg-info/dependency_links.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       46 2024-05-29 18:18:13.000000 bwalign-0.1.0/bwalign.egg-info/entry_points.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       16 2024-05-29 18:18:13.000000 bwalign-0.1.0/bwalign.egg-info/requires.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)        8 2024-05-29 18:18:13.000000 bwalign-0.1.0/bwalign.egg-info/top_level.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       38 2024-05-29 18:18:13.175499 bwalign-0.1.0/setup.cfg
--rw-r--r--   0 adrianlayer   (501) staff       (20)     1194 2024-05-29 18:17:32.000000 bwalign-0.1.0/setup.py
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 00:02:39.534069 bwalign-1.0.0/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      914 2024-06-03 00:02:39.531797 bwalign-1.0.0/PKG-INFO
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     1744 2024-05-29 18:41:22.000000 bwalign-1.0.0/README.md
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 00:02:39.513790 bwalign-1.0.0/bwalign/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      142 2024-06-03 00:01:19.000000 bwalign-1.0.0/bwalign/__init__.py
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     2146 2024-06-02 23:55:00.000000 bwalign-1.0.0/bwalign/main.py
+-rw-r--r--   0 adrianlayer   (501) staff       (20)    20537 2024-06-02 23:56:53.000000 bwalign-1.0.0/bwalign/utils.py
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 00:02:39.527307 bwalign-1.0.0/bwalign.egg-info/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      914 2024-06-03 00:02:39.000000 bwalign-1.0.0/bwalign.egg-info/PKG-INFO
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      259 2024-06-03 00:02:39.000000 bwalign-1.0.0/bwalign.egg-info/SOURCES.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)        1 2024-06-03 00:02:39.000000 bwalign-1.0.0/bwalign.egg-info/dependency_links.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       46 2024-06-03 00:02:39.000000 bwalign-1.0.0/bwalign.egg-info/entry_points.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       16 2024-06-03 00:02:39.000000 bwalign-1.0.0/bwalign.egg-info/requires.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)        8 2024-06-03 00:02:39.000000 bwalign-1.0.0/bwalign.egg-info/top_level.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       38 2024-06-03 00:02:39.534603 bwalign-1.0.0/setup.cfg
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     1194 2024-06-03 00:00:58.000000 bwalign-1.0.0/setup.py
```

### Comparing `bwalign-0.1.0/PKG-INFO` & `bwalign-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bwalign
-Version: 0.1.0
+Version: 1.0.0
 Summary: A burrows-wheeler seed and extend aligner
 Home-page: https://github.com/NabilHKhoury/bwalign
 Author: ['Adrian Layer, Nabil Khoury, Yasmin Jabir']
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `bwalign-0.1.0/bwalign/main.py` & `bwalign-1.0.0/bwalign/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from bwalign import utils
+import utils
 import pysam
 import argparse
 
 def main():
     parser = argparse.ArgumentParser(description="Run BWA alignment with specified reference genome and FASTQ file.")
     parser.add_argument("reference_genome", type=str, help="Path to the reference genome file")
     parser.add_argument("fastq_file", type=str, help="Path to the FASTQ file")
@@ -15,16 +15,17 @@
     
     # Parse the reference genome
     ref_id, reference = utils.parse_reference_genome(args.reference_genome)
     
     #BWT and SA
     K = 5
     ref_text = str(reference) + '$'
-    bwt = utils.burrows_wheeler_transform(ref_text)
-    psa = utils.partial_suffix_array(ref_text, K)
+    sa = utils.suffix_array(ref_text)
+    psa = utils.partial_suffix_array(sa, K)
+    bwt = utils.bwt_from_suffixarray(ref_text, sa)
     first_occurrences = utils.compute_first_occurrences(bwt)
     checkpoint_arrs = utils.compute_checkpoint_arrs(bwt)
     ranks = utils.compute_rank_arr(bwt)
     
     #header for the SAM file (based on ref)
     header = {
         'HD': {'VN': '1.0', 'SO': 'unsorted'},
@@ -41,15 +42,15 @@
             #create a SAM entry for the aligned read
             a = pysam.AlignedSegment()
             a.query_name = read_id
             a.query_sequence = read_seq
             a.flag = 0
             a.reference_id = 0
             a.reference_start = best_idx
-            a.mapping_quality = 60
+            a.mapping_quality = utils.calculate_mapping_quality(score, read_length)
             a.cigarstring = utils.calculate_cigar(alignment_s, alignment_t)
             a.query_qualities = qual_scores
             
             samfile.write(a)
 
 if __name__ == "__main__":
     main()
```

### Comparing `bwalign-0.1.0/bwalign/utils.py` & `bwalign-1.0.0/bwalign/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,30 @@
 from Bio import SeqIO
 from typing import List, Tuple
 import sys
 import random
+import math
+
+def calculate_mapping_quality(score, read_length):  
+    max_possible_score = 2 * read_length
+    
+    if score < 0:
+        return 0 
+
+    if max_possible_score > 0:
+        probability = score / max_possible_score
+    else:
+        probability = 0
+
+    if probability > 0:
+        mapping_quality = -10 * math.log10(1 - probability)
+    else:
+        mapping_quality = 0
+
+    return min(int(mapping_quality), 60)
 
 ### CIGAR STRING CREATOR
 
 def calculate_cigar(alignment_s, alignment_t):
     cigar = []
     match = 0
     ins = 0
@@ -189,36 +208,118 @@
                 best_idx = ref_idx
                 s_best_align = s_align
                 t_best_align = t_align
     return best_idx, best_score, s_best_align, t_best_align
 
 ### SEED GENERATION
 
-def burrows_wheeler_transform(text: str) -> str:
+## BWT creation
+def bwt_from_suffixarray(text: str, suffix_array: List[int]) -> str:
+    bwt = []
+    for idx in suffix_array:
+        bwt.append(text[idx-1])
+    return ''.join(bwt)
+
+# SUFFIX ARRAY CONSTRUCTION
+class suffix:
+    """
+    Class built to store suffix array indices, conserving memory.
+    """
+    def __init__(self):
+        self.index = 0
+        self.rank = [0,0]
+
+def get_rank(char: str) -> int:
+    """
+    Converts the given char to its ascii value, then subtracts 'a' from it to get a
+    clean rank value.
+    """
+    return ord(char) - ord('a')
+
+def suffix_array(text: str) -> list[int]:
     """
-    Generate the Burrows-Wheeler Transform of the given text.
+    Generates the suffix array of a given database string text using O(n(logn)^2)
+    time complexity and O(n) space. To improve to O(nlogn), can use radix sort to
+    sort the suffix lists.
+    
+    Algorithm ripped from:
+    https://www.geeksforgeeks.org/suffix-array-set-2-a-nlognlogn-algorithm/
     """
-    cyclic_rotations = []
-    for i in range(0,len(text)):
-        cyclic_rotations.append(text[i:] + text[:i])
-    M = sorted(cyclic_rotations)
-    bwt = ''
-    for rotation in M:
-        bwt = bwt + rotation[len(rotation)-1]
-    return bwt
+    
+    # get the intial array of suffixes before starting to loop through and rank them.
+    suffixes = [suffix() for _ in range(len(text))]
+    
+    # initial (k=2) ranking of suffixes
+    for i in range(0, len(text)):
+        suffixes[i].index = i
+        suffixes[i].rank[0] = get_rank(text[i])
+        if (i + 1) < len(text):
+            suffixes[i].rank[1] = get_rank(text[i+1])
+        else:
+            suffixes[i].rank[1] = -1
+    
+    # https://stackoverflow.com/questions/9376384/sort-a-list-of-tuples-depending-on-two-elements
+    suffixes = sorted(suffixes, key=lambda element: (element.rank[0], element.rank[1]))
+    
+    ind = [0] * len(text) # array to keep track of indices while computing ranks
+    
+    k = 4
+    while (k < 2 * len(text)):
+         
+        # Assigning rank and index 
+        # values to first suffix
+        rank = 0
+        prev_rank = suffixes[0].rank[0]
+        suffixes[0].rank[0] = rank
+        ind[suffixes[0].index] = 0
+ 
+        # Assigning rank to suffixes
+        for i in range(1, len(text)):
+             
+            # If first rank and next ranks are 
+            # same as that of previous suffix in
+            # array, assign the same new rank to 
+            # this suffix
+            if (suffixes[i].rank[0] == prev_rank and
+                suffixes[i].rank[1] == suffixes[i - 1].rank[1]):
+                prev_rank = suffixes[i].rank[0]
+                suffixes[i].rank[0] = rank
+                 
+            # Otherwise increment rank and assign    
+            else:  
+                prev_rank = suffixes[i].rank[0]
+                rank += 1
+                suffixes[i].rank[0] = rank
+            ind[suffixes[i].index] = i
+ 
+        # Assign next rank to every suffix
+        for i in range(len(text)):
+            nextindex = suffixes[i].index + k // 2
+            suffixes[i].rank[1] = suffixes[ind[nextindex]].rank[0] if (nextindex < len(text)) else -1
+ 
+        # Sort the suffixes according to
+        # first k characters
+        suffixes = sorted(suffixes, key = lambda element: (element.rank[0], element.rank[1]))
+ 
+        k *= 2
+        
+    to_return = []
+    for i in range(0, len(text)):
+        to_return.append(suffixes[i].index)
+        
+    return to_return
 
-def partial_suffix_array(text: str, k: int) -> dict[int, int]:
+def partial_suffix_array(sa: list[int], k: int) -> dict[int, int]:
     """
     Generate a partial suffix array for the given text and interval K.
     """
-    full_suffix_array = sorted(range(len(text)), key=lambda i: text[i:]) # taken from Nabil's bw code
     partial = dict()
-    for idx in full_suffix_array:
-        if full_suffix_array[idx] % k == 0:
-            partial[idx] = full_suffix_array[idx]
+    for idx in sa:
+        if sa[idx] % k == 0:
+            partial[idx] = sa[idx]
     return partial
 
 def compute_rank_arr(bwt: str) -> list[int]:
     """
     This function generates the rank of each position in the last column given by the bwt.
     The rank is the number of occurrences of whatever character is at that position, up to
     that position. This can be done in linear time by iterating through the bwt. The ranks
@@ -351,16 +452,14 @@
 
     :param fasta_path: Path to the FASTA file
     :return: A tuple containing the sequence ID and the sequence itself
     """
     with open(fasta_path, "r") as handle:
         for record in SeqIO.parse(handle, "fasta"):
             return record.id, str(record.seq)
-        
-
 
 def random_sequence(length: int) -> str:
     """
     Generate a random DNA sequence of the specified length.
 
     :param length: The length of the sequence
     :return: A random DNA sequence
@@ -372,15 +471,14 @@
     Generate random quality scores for a sequence of the specified length.
 
     :param length: The length of the sequence
     :return: A list of random quality scores
     """
     return ''.join(random.choices('!"#$%&\'()*+,-./0123456789:;<=>?@ABCDEFGHI', k=length))
 
-
 def random_id(length: int) -> str:
     """
     Generate a random sequence ID of the specified length.
 
     :param length: The length of the sequence ID
     :return: A random sequence ID
     """
```

### Comparing `bwalign-0.1.0/bwalign.egg-info/PKG-INFO` & `bwalign-1.0.0/bwalign.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bwalign
-Version: 0.1.0
+Version: 1.0.0
 Summary: A burrows-wheeler seed and extend aligner
 Home-page: https://github.com/NabilHKhoury/bwalign
 Author: ['Adrian Layer, Nabil Khoury, Yasmin Jabir']
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `bwalign-0.1.0/setup.py` & `bwalign-1.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='bwalign',
-    version='0.1.0',    
+    version='1.0.0',    
     description='A burrows-wheeler seed and extend aligner',
     url='https://github.com/NabilHKhoury/bwalign',
     author=['Adrian Layer, Nabil Khoury, Yasmin Jabir'],
     license='MIT',
     packages=find_packages(),
     install_requires=['biopython',
                       'pysam',
```

