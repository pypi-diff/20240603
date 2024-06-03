# Comparing `tmp/bwalign-1.5.8.tar.gz` & `tmp/bwalign-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bwalign-1.5.8.tar", last modified: Mon Jun  3 10:24:25 2024, max compression
+gzip compressed data, was "bwalign-1.5.9.tar", last modified: Mon Jun  3 10:26:39 2024, max compression
```

## Comparing `bwalign-1.5.8.tar` & `bwalign-1.5.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 10:24:25.186432 bwalign-1.5.8/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 10:24:25.185320 bwalign-1.5.8/PKG-INFO
--rw-r--r--   0 adrianlayer   (501) staff       (20)     1744 2024-05-29 18:41:22.000000 bwalign-1.5.8/README.md
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 10:24:25.178007 bwalign-1.5.8/bwalign/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      142 2024-06-03 10:24:07.000000 bwalign-1.5.8/bwalign/__init__.py
--rw-r--r--   0 adrianlayer   (501) staff       (20)     2236 2024-06-03 10:23:56.000000 bwalign-1.5.8/bwalign/main.py
--rw-r--r--   0 adrianlayer   (501) staff       (20)    18374 2024-06-03 10:18:37.000000 bwalign-1.5.8/bwalign/utils.py
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 10:24:25.184259 bwalign-1.5.8/bwalign.egg-info/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 10:24:25.000000 bwalign-1.5.8/bwalign.egg-info/PKG-INFO
--rw-r--r--   0 adrianlayer   (501) staff       (20)      259 2024-06-03 10:24:25.000000 bwalign-1.5.8/bwalign.egg-info/SOURCES.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)        1 2024-06-03 10:24:25.000000 bwalign-1.5.8/bwalign.egg-info/dependency_links.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       46 2024-06-03 10:24:25.000000 bwalign-1.5.8/bwalign.egg-info/entry_points.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       21 2024-06-03 10:24:25.000000 bwalign-1.5.8/bwalign.egg-info/requires.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)        8 2024-06-03 10:24:25.000000 bwalign-1.5.8/bwalign.egg-info/top_level.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       38 2024-06-03 10:24:25.186583 bwalign-1.5.8/setup.cfg
--rw-r--r--   0 adrianlayer   (501) staff       (20)     1224 2024-06-03 10:24:04.000000 bwalign-1.5.8/setup.py
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 10:26:39.266760 bwalign-1.5.9/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 10:26:39.265496 bwalign-1.5.9/PKG-INFO
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     1744 2024-05-29 18:41:22.000000 bwalign-1.5.9/README.md
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 10:26:39.255826 bwalign-1.5.9/bwalign/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      142 2024-06-03 10:26:29.000000 bwalign-1.5.9/bwalign/__init__.py
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     2235 2024-06-03 10:26:14.000000 bwalign-1.5.9/bwalign/main.py
+-rw-r--r--   0 adrianlayer   (501) staff       (20)    18374 2024-06-03 10:18:37.000000 bwalign-1.5.9/bwalign/utils.py
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 10:26:39.264038 bwalign-1.5.9/bwalign.egg-info/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 10:26:39.000000 bwalign-1.5.9/bwalign.egg-info/PKG-INFO
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      259 2024-06-03 10:26:39.000000 bwalign-1.5.9/bwalign.egg-info/SOURCES.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)        1 2024-06-03 10:26:39.000000 bwalign-1.5.9/bwalign.egg-info/dependency_links.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       46 2024-06-03 10:26:39.000000 bwalign-1.5.9/bwalign.egg-info/entry_points.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       21 2024-06-03 10:26:39.000000 bwalign-1.5.9/bwalign.egg-info/requires.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)        8 2024-06-03 10:26:39.000000 bwalign-1.5.9/bwalign.egg-info/top_level.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       38 2024-06-03 10:26:39.266917 bwalign-1.5.9/setup.cfg
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     1224 2024-06-03 10:26:30.000000 bwalign-1.5.9/setup.py
```

### Comparing `bwalign-1.5.8/PKG-INFO` & `bwalign-1.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bwalign
-Version: 1.5.8
+Version: 1.5.9
 Summary: A burrows-wheeler seed and extend aligner
 Home-page: https://github.com/NabilHKhoury/bwalign
 Author: ['Adrian Layer, Nabil Khoury, Yasmin Jabir']
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `bwalign-1.5.8/README.md` & `bwalign-1.5.9/README.md`

 * *Files identical despite different names*

### Comparing `bwalign-1.5.8/bwalign/main.py` & `bwalign-1.5.9/bwalign/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,21 +40,21 @@
             
             #create a SAM entry for the aligned read
             a = pysam.AlignedSegment()
             a.query_name = read_id
             a.query_sequence = read_seq
             a.flag = 0
             a.reference_id = 0
-            if best_idx == float('-inf'):
-                a.reference_start = -1
-                a.mapping_quality = -1
-                a.cigarstring = '0M'
-            else:
+            if best_idx > float('-inf'):
                 a.reference_start = best_idx
                 a.mapping_quality = calculate_mapping_quality(score, read_length)
                 a.cigarstring = calculate_cigar(alignment_s, alignment_t)
+            else:
+                a.reference_start = -1
+                a.mapping_quality = -1
+                a.cigarstring = '0M'
             a.query_qualities = qual_scores
             
             samfile.write(a)
 
 if __name__ == "__main__":
     main()
```

### Comparing `bwalign-1.5.8/bwalign/utils.py` & `bwalign-1.5.9/bwalign/utils.py`

 * *Files identical despite different names*

### Comparing `bwalign-1.5.8/bwalign.egg-info/PKG-INFO` & `bwalign-1.5.9/bwalign.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bwalign
-Version: 1.5.8
+Version: 1.5.9
 Summary: A burrows-wheeler seed and extend aligner
 Home-page: https://github.com/NabilHKhoury/bwalign
 Author: ['Adrian Layer, Nabil Khoury, Yasmin Jabir']
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `bwalign-1.5.8/setup.py` & `bwalign-1.5.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='bwalign',
-    version='1.5.8',    
+    version='1.5.9',    
     description='A burrows-wheeler seed and extend aligner',
     url='https://github.com/NabilHKhoury/bwalign',
     author=['Adrian Layer, Nabil Khoury, Yasmin Jabir'],
     license='MIT',
     packages=find_packages(),
     install_requires=['biopython',
                       'pysam',
```

