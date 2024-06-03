# Comparing `tmp/bwalign-1.6.4.tar.gz` & `tmp/bwalign-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bwalign-1.6.4.tar", last modified: Mon Jun  3 11:31:15 2024, max compression
+gzip compressed data, was "bwalign-1.6.5.tar", last modified: Mon Jun  3 11:46:53 2024, max compression
```

## Comparing `bwalign-1.6.4.tar` & `bwalign-1.6.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 11:31:15.648918 bwalign-1.6.4/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 11:31:15.648024 bwalign-1.6.4/PKG-INFO
--rw-r--r--   0 adrianlayer   (501) staff       (20)     1744 2024-05-29 18:41:22.000000 bwalign-1.6.4/README.md
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 11:31:15.638998 bwalign-1.6.4/bwalign/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      142 2024-06-03 11:31:05.000000 bwalign-1.6.4/bwalign/__init__.py
--rw-r--r--   0 adrianlayer   (501) staff       (20)     2231 2024-06-03 11:30:53.000000 bwalign-1.6.4/bwalign/main.py
--rw-r--r--   0 adrianlayer   (501) staff       (20)    18538 2024-06-03 11:27:05.000000 bwalign-1.6.4/bwalign/utils.py
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 11:31:15.646607 bwalign-1.6.4/bwalign.egg-info/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 11:31:15.000000 bwalign-1.6.4/bwalign.egg-info/PKG-INFO
--rw-r--r--   0 adrianlayer   (501) staff       (20)      259 2024-06-03 11:31:15.000000 bwalign-1.6.4/bwalign.egg-info/SOURCES.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)        1 2024-06-03 11:31:15.000000 bwalign-1.6.4/bwalign.egg-info/dependency_links.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       46 2024-06-03 11:31:15.000000 bwalign-1.6.4/bwalign.egg-info/entry_points.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       21 2024-06-03 11:31:15.000000 bwalign-1.6.4/bwalign.egg-info/requires.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)        8 2024-06-03 11:31:15.000000 bwalign-1.6.4/bwalign.egg-info/top_level.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       38 2024-06-03 11:31:15.649127 bwalign-1.6.4/setup.cfg
--rw-r--r--   0 adrianlayer   (501) staff       (20)     1224 2024-06-03 11:31:01.000000 bwalign-1.6.4/setup.py
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 11:46:53.240819 bwalign-1.6.5/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 11:46:53.239730 bwalign-1.6.5/PKG-INFO
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     1744 2024-05-29 18:41:22.000000 bwalign-1.6.5/README.md
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 11:46:53.195885 bwalign-1.6.5/bwalign/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      142 2024-06-03 11:46:37.000000 bwalign-1.6.5/bwalign/__init__.py
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     2231 2024-06-03 11:46:28.000000 bwalign-1.6.5/bwalign/main.py
+-rw-r--r--   0 adrianlayer   (501) staff       (20)    18601 2024-06-03 11:46:18.000000 bwalign-1.6.5/bwalign/utils.py
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 11:46:53.230768 bwalign-1.6.5/bwalign.egg-info/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 11:46:52.000000 bwalign-1.6.5/bwalign.egg-info/PKG-INFO
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      259 2024-06-03 11:46:53.000000 bwalign-1.6.5/bwalign.egg-info/SOURCES.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)        1 2024-06-03 11:46:52.000000 bwalign-1.6.5/bwalign.egg-info/dependency_links.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       46 2024-06-03 11:46:52.000000 bwalign-1.6.5/bwalign.egg-info/entry_points.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       21 2024-06-03 11:46:52.000000 bwalign-1.6.5/bwalign.egg-info/requires.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)        8 2024-06-03 11:46:52.000000 bwalign-1.6.5/bwalign.egg-info/top_level.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       38 2024-06-03 11:46:53.241109 bwalign-1.6.5/setup.cfg
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     1224 2024-06-03 11:46:34.000000 bwalign-1.6.5/setup.py
```

### Comparing `bwalign-1.6.4/PKG-INFO` & `bwalign-1.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bwalign
-Version: 1.6.4
+Version: 1.6.5
 Summary: A burrows-wheeler seed and extend aligner
 Home-page: https://github.com/NabilHKhoury/bwalign
 Author: ['Adrian Layer, Nabil Khoury, Yasmin Jabir']
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `bwalign-1.6.4/README.md` & `bwalign-1.6.5/README.md`

 * *Files identical despite different names*

### Comparing `bwalign-1.6.4/bwalign/main.py` & `bwalign-1.6.5/bwalign/main.py`

 * *Files identical despite different names*

### Comparing `bwalign-1.6.4/bwalign/utils.py` & `bwalign-1.6.5/bwalign/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,18 @@
         return 0 
 
     if max_possible_score > 0:
         probability = score / max_possible_score
     else:
         probability = 0
 
-    if probability > 0:
-        mapping_quality = -10 * np.log10(1 - probability)
+    if probability == 1:
+        return max_possible_score
+    elif probability > 0:
+        mapping_quality = -10 * np.log10(1.0 - probability)
     else:
         mapping_quality = 0
 
     return min(int(mapping_quality), 60)
 
 ### CIGAR STRING CREATOR
```

### Comparing `bwalign-1.6.4/bwalign.egg-info/PKG-INFO` & `bwalign-1.6.5/bwalign.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bwalign
-Version: 1.6.4
+Version: 1.6.5
 Summary: A burrows-wheeler seed and extend aligner
 Home-page: https://github.com/NabilHKhoury/bwalign
 Author: ['Adrian Layer, Nabil Khoury, Yasmin Jabir']
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `bwalign-1.6.4/setup.py` & `bwalign-1.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='bwalign',
-    version='1.6.4',    
+    version='1.6.5',    
     description='A burrows-wheeler seed and extend aligner',
     url='https://github.com/NabilHKhoury/bwalign',
     author=['Adrian Layer, Nabil Khoury, Yasmin Jabir'],
     license='MIT',
     packages=find_packages(),
     install_requires=['biopython',
                       'pysam',
```

