# Comparing `tmp/bwalign-1.0.3.tar.gz` & `tmp/bwalign-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bwalign-1.0.3.tar", last modified: Mon Jun  3 01:08:57 2024, max compression
+gzip compressed data, was "bwalign-1.0.4.tar", last modified: Mon Jun  3 01:09:48 2024, max compression
```

## Comparing `bwalign-1.0.3.tar` & `bwalign-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 01:08:57.129530 bwalign-1.0.3/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      914 2024-06-03 01:08:57.128289 bwalign-1.0.3/PKG-INFO
--rw-r--r--   0 adrianlayer   (501) staff       (20)     1744 2024-05-29 18:41:22.000000 bwalign-1.0.3/README.md
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 01:08:57.102749 bwalign-1.0.3/bwalign/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      142 2024-06-03 01:08:15.000000 bwalign-1.0.3/bwalign/__init__.py
--rw-r--r--   0 adrianlayer   (501) staff       (20)     2083 2024-06-03 01:07:06.000000 bwalign-1.0.3/bwalign/main.py
--rw-r--r--   0 adrianlayer   (501) staff       (20)    20539 2024-06-03 00:56:50.000000 bwalign-1.0.3/bwalign/utils.py
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 01:08:57.126425 bwalign-1.0.3/bwalign.egg-info/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      914 2024-06-03 01:08:56.000000 bwalign-1.0.3/bwalign.egg-info/PKG-INFO
--rw-r--r--   0 adrianlayer   (501) staff       (20)      259 2024-06-03 01:08:56.000000 bwalign-1.0.3/bwalign.egg-info/SOURCES.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)        1 2024-06-03 01:08:56.000000 bwalign-1.0.3/bwalign.egg-info/dependency_links.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       46 2024-06-03 01:08:56.000000 bwalign-1.0.3/bwalign.egg-info/entry_points.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       16 2024-06-03 01:08:56.000000 bwalign-1.0.3/bwalign.egg-info/requires.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)        8 2024-06-03 01:08:56.000000 bwalign-1.0.3/bwalign.egg-info/top_level.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       38 2024-06-03 01:08:57.129769 bwalign-1.0.3/setup.cfg
--rw-r--r--   0 adrianlayer   (501) staff       (20)     1194 2024-06-03 01:08:17.000000 bwalign-1.0.3/setup.py
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 01:09:48.455514 bwalign-1.0.4/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      914 2024-06-03 01:09:48.452045 bwalign-1.0.4/PKG-INFO
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     1744 2024-05-29 18:41:22.000000 bwalign-1.0.4/README.md
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 01:09:48.443496 bwalign-1.0.4/bwalign/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      142 2024-06-03 01:09:30.000000 bwalign-1.0.4/bwalign/__init__.py
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     2083 2024-06-03 01:09:18.000000 bwalign-1.0.4/bwalign/main.py
+-rw-r--r--   0 adrianlayer   (501) staff       (20)    20539 2024-06-03 00:56:50.000000 bwalign-1.0.4/bwalign/utils.py
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 01:09:48.450902 bwalign-1.0.4/bwalign.egg-info/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      914 2024-06-03 01:09:48.000000 bwalign-1.0.4/bwalign.egg-info/PKG-INFO
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      259 2024-06-03 01:09:48.000000 bwalign-1.0.4/bwalign.egg-info/SOURCES.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)        1 2024-06-03 01:09:48.000000 bwalign-1.0.4/bwalign.egg-info/dependency_links.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       46 2024-06-03 01:09:48.000000 bwalign-1.0.4/bwalign.egg-info/entry_points.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       16 2024-06-03 01:09:48.000000 bwalign-1.0.4/bwalign.egg-info/requires.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)        8 2024-06-03 01:09:48.000000 bwalign-1.0.4/bwalign.egg-info/top_level.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       38 2024-06-03 01:09:48.455816 bwalign-1.0.4/setup.cfg
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     1194 2024-06-03 01:09:27.000000 bwalign-1.0.4/setup.py
```

### Comparing `bwalign-1.0.3/PKG-INFO` & `bwalign-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bwalign
-Version: 1.0.3
+Version: 1.0.4
 Summary: A burrows-wheeler seed and extend aligner
 Home-page: https://github.com/NabilHKhoury/bwalign
 Author: ['Adrian Layer, Nabil Khoury, Yasmin Jabir']
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `bwalign-1.0.3/README.md` & `bwalign-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `bwalign-1.0.3/bwalign/main.py` & `bwalign-1.0.4/bwalign/main.py`

 * *Files identical despite different names*

### Comparing `bwalign-1.0.3/bwalign/utils.py` & `bwalign-1.0.4/bwalign/utils.py`

 * *Files identical despite different names*

### Comparing `bwalign-1.0.3/bwalign.egg-info/PKG-INFO` & `bwalign-1.0.4/bwalign.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bwalign
-Version: 1.0.3
+Version: 1.0.4
 Summary: A burrows-wheeler seed and extend aligner
 Home-page: https://github.com/NabilHKhoury/bwalign
 Author: ['Adrian Layer, Nabil Khoury, Yasmin Jabir']
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `bwalign-1.0.3/setup.py` & `bwalign-1.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='bwalign',
-    version='1.0.3',    
+    version='1.0.4',    
     description='A burrows-wheeler seed and extend aligner',
     url='https://github.com/NabilHKhoury/bwalign',
     author=['Adrian Layer, Nabil Khoury, Yasmin Jabir'],
     license='MIT',
     packages=find_packages(),
     install_requires=['biopython',
                       'pysam',
```

