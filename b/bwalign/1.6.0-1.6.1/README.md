# Comparing `tmp/bwalign-1.6.0.tar.gz` & `tmp/bwalign-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bwalign-1.6.0.tar", last modified: Mon Jun  3 10:29:01 2024, max compression
+gzip compressed data, was "bwalign-1.6.1.tar", last modified: Mon Jun  3 10:32:56 2024, max compression
```

## Comparing `bwalign-1.6.0.tar` & `bwalign-1.6.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 10:29:01.142655 bwalign-1.6.0/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 10:29:01.141772 bwalign-1.6.0/PKG-INFO
--rw-r--r--   0 adrianlayer   (501) staff       (20)     1744 2024-05-29 18:41:22.000000 bwalign-1.6.0/README.md
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 10:29:01.133422 bwalign-1.6.0/bwalign/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      142 2024-06-03 10:28:40.000000 bwalign-1.6.0/bwalign/__init__.py
--rw-r--r--   0 adrianlayer   (501) staff       (20)     2233 2024-06-03 10:28:30.000000 bwalign-1.6.0/bwalign/main.py
--rw-r--r--   0 adrianlayer   (501) staff       (20)    18374 2024-06-03 10:18:37.000000 bwalign-1.6.0/bwalign/utils.py
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 10:29:01.140738 bwalign-1.6.0/bwalign.egg-info/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 10:29:01.000000 bwalign-1.6.0/bwalign.egg-info/PKG-INFO
--rw-r--r--   0 adrianlayer   (501) staff       (20)      259 2024-06-03 10:29:01.000000 bwalign-1.6.0/bwalign.egg-info/SOURCES.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)        1 2024-06-03 10:29:01.000000 bwalign-1.6.0/bwalign.egg-info/dependency_links.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       46 2024-06-03 10:29:01.000000 bwalign-1.6.0/bwalign.egg-info/entry_points.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       21 2024-06-03 10:29:01.000000 bwalign-1.6.0/bwalign.egg-info/requires.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)        8 2024-06-03 10:29:01.000000 bwalign-1.6.0/bwalign.egg-info/top_level.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       38 2024-06-03 10:29:01.142857 bwalign-1.6.0/setup.cfg
--rw-r--r--   0 adrianlayer   (501) staff       (20)     1224 2024-06-03 10:28:37.000000 bwalign-1.6.0/setup.py
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 10:32:56.229006 bwalign-1.6.1/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 10:32:56.228011 bwalign-1.6.1/PKG-INFO
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     1744 2024-05-29 18:41:22.000000 bwalign-1.6.1/README.md
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 10:32:56.219534 bwalign-1.6.1/bwalign/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      142 2024-06-03 10:32:36.000000 bwalign-1.6.1/bwalign/__init__.py
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     2233 2024-06-03 10:28:30.000000 bwalign-1.6.1/bwalign/main.py
+-rw-r--r--   0 adrianlayer   (501) staff       (20)    18476 2024-06-03 10:32:24.000000 bwalign-1.6.1/bwalign/utils.py
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 10:32:56.226963 bwalign-1.6.1/bwalign.egg-info/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 10:32:56.000000 bwalign-1.6.1/bwalign.egg-info/PKG-INFO
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      259 2024-06-03 10:32:56.000000 bwalign-1.6.1/bwalign.egg-info/SOURCES.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)        1 2024-06-03 10:32:56.000000 bwalign-1.6.1/bwalign.egg-info/dependency_links.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       46 2024-06-03 10:32:56.000000 bwalign-1.6.1/bwalign.egg-info/entry_points.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       21 2024-06-03 10:32:56.000000 bwalign-1.6.1/bwalign.egg-info/requires.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)        8 2024-06-03 10:32:56.000000 bwalign-1.6.1/bwalign.egg-info/top_level.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       38 2024-06-03 10:32:56.229154 bwalign-1.6.1/setup.cfg
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     1224 2024-06-03 10:32:32.000000 bwalign-1.6.1/setup.py
```

### Comparing `bwalign-1.6.0/PKG-INFO` & `bwalign-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bwalign
-Version: 1.6.0
+Version: 1.6.1
 Summary: A burrows-wheeler seed and extend aligner
 Home-page: https://github.com/NabilHKhoury/bwalign
 Author: ['Adrian Layer, Nabil Khoury, Yasmin Jabir']
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `bwalign-1.6.0/README.md` & `bwalign-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `bwalign-1.6.0/bwalign/main.py` & `bwalign-1.6.1/bwalign/main.py`

 * *Files identical despite different names*

### Comparing `bwalign-1.6.0/bwalign/utils.py` & `bwalign-1.6.1/bwalign/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,19 @@
             if abs(j-i) < bp:
                 match = -mmp
                 if s[i-1] == t[j-1]:
                     match = mr
                 l[i,j] = max(l[i-1][j] - indp, l[i][j-1] - indp, l[i-1][j-1] + match)
             else:
                 continue
-    return int(l[len(s),len(t)])
+    score = l[len(s),len(t)]
+    if score > float('-inf'):
+        return int(l[len(s),len(t)])
+    else:
+        return float('-inf')
 
 def BandedAlignmentWithBackTrack(match_reward: int, mismatch_penalty: int, indel_penalty: int,
                     band_parameter: int, s: str, t: str) -> tuple[int, str, str]:
     sys.setrecursionlimit(1500)
     l = [[float('-inf')] * (len(t) + 1) for _ in range(len(s) + 1)] # score matrix
     b = [[None] * (len(t)) for _ in range(len(s))] # backtrack matrix
     for i in range(0, len(s) + 1):
```

### Comparing `bwalign-1.6.0/bwalign.egg-info/PKG-INFO` & `bwalign-1.6.1/bwalign.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bwalign
-Version: 1.6.0
+Version: 1.6.1
 Summary: A burrows-wheeler seed and extend aligner
 Home-page: https://github.com/NabilHKhoury/bwalign
 Author: ['Adrian Layer, Nabil Khoury, Yasmin Jabir']
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `bwalign-1.6.0/setup.py` & `bwalign-1.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='bwalign',
-    version='1.6.0',    
+    version='1.6.1',    
     description='A burrows-wheeler seed and extend aligner',
     url='https://github.com/NabilHKhoury/bwalign',
     author=['Adrian Layer, Nabil Khoury, Yasmin Jabir'],
     license='MIT',
     packages=find_packages(),
     install_requires=['biopython',
                       'pysam',
```

