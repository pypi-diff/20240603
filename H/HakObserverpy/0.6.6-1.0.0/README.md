# Comparing `tmp/HakObserverpy-0.6.6.tar.gz` & `tmp/HakObserverpy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HakObserverpy-0.6.6.tar", last modified: Sat Jun  1 10:16:57 2024, max compression
+gzip compressed data, was "HakObserverpy-1.0.0.tar", last modified: Mon Jun  3 14:29:01 2024, max compression
```

## Comparing `HakObserverpy-0.6.6.tar` & `HakObserverpy-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 10:16:57.280000 HakObserverpy-0.6.6/
-drwxrwxrwx   0        0        0        0 2024-06-01 10:16:57.214000 HakObserverpy-0.6.6/HakObserverpy/
--rw-rw-rw-   0        0        0     6190 2024-06-01 10:05:27.000000 HakObserverpy-0.6.6/HakObserverpy/HakObserverpy.py
--rw-rw-rw-   0        0        0      283 2024-06-01 10:05:30.000000 HakObserverpy-0.6.6/HakObserverpy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 10:16:57.262000 HakObserverpy-0.6.6/HakObserverpy.egg-info/
--rw-rw-rw-   0        0        0      705 2024-06-01 10:16:57.000000 HakObserverpy-0.6.6/HakObserverpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2024-06-01 10:16:57.000000 HakObserverpy-0.6.6/HakObserverpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 10:16:57.000000 HakObserverpy-0.6.6/HakObserverpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-06-01 10:16:57.000000 HakObserverpy-0.6.6/HakObserverpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-06-01 10:16:57.000000 HakObserverpy-0.6.6/HakObserverpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      705 2024-06-01 10:16:57.268000 HakObserverpy-0.6.6/PKG-INFO
--rw-rw-rw-   0        0        0      280 2024-05-13 09:19:09.000000 HakObserverpy-0.6.6/README.md
--rw-rw-rw-   0        0        0       42 2024-06-01 10:16:57.279000 HakObserverpy-0.6.6/setup.cfg
--rw-rw-rw-   0        0        0     1044 2024-06-01 10:05:24.000000 HakObserverpy-0.6.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 14:29:01.940000 HakObserverpy-1.0.0/
+drwxrwxrwx   0        0        0        0 2024-06-03 14:29:01.873000 HakObserverpy-1.0.0/HakObserverpy/
+-rw-rw-rw-   0        0        0     6190 2024-06-03 14:28:48.000000 HakObserverpy-1.0.0/HakObserverpy/HakObserverpy.py
+-rw-rw-rw-   0        0        0      337 2024-06-03 14:28:52.000000 HakObserverpy-1.0.0/HakObserverpy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 14:29:01.928000 HakObserverpy-1.0.0/HakObserverpy.egg-info/
+-rw-rw-rw-   0        0        0      705 2024-06-03 14:29:01.000000 HakObserverpy-1.0.0/HakObserverpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2024-06-03 14:29:01.000000 HakObserverpy-1.0.0/HakObserverpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 14:29:01.000000 HakObserverpy-1.0.0/HakObserverpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-06-03 14:29:01.000000 HakObserverpy-1.0.0/HakObserverpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-06-03 14:29:01.000000 HakObserverpy-1.0.0/HakObserverpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      705 2024-06-03 14:29:01.935000 HakObserverpy-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2024-06-03 14:28:45.000000 HakObserverpy-1.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-03 14:29:01.939000 HakObserverpy-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1044 2024-06-03 14:28:58.000000 HakObserverpy-1.0.0/setup.py
```

### Comparing `HakObserverpy-0.6.6/HakObserverpy/HakObserverpy.py` & `HakObserverpy-1.0.0/HakObserverpy/HakObserverpy.py`

 * *Files identical despite different names*

### Comparing `HakObserverpy-0.6.6/HakObserverpy.egg-info/PKG-INFO` & `HakObserverpy-1.0.0/HakObserverpy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HakObserverpy
-Version: 0.6.6
+Version: 1.0.0
 Summary: A package connect endpoints to the Hakware Application
 Home-page: UNKNOWN
 Author: Jacob O'Brien
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `HakObserverpy-0.6.6/PKG-INFO` & `HakObserverpy-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HakObserverpy
-Version: 0.6.6
+Version: 1.0.0
 Summary: A package connect endpoints to the Hakware Application
 Home-page: UNKNOWN
 Author: Jacob O'Brien
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `HakObserverpy-0.6.6/setup.py` & `HakObserverpy-1.0.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import platform
 from setuptools import setup, find_packages
 
 setup(
     name='HakObserverpy',  # Your package name
-    version='0.6.6',  # Start with a version number
+    version='1.0.0',  # Start with a version number
     description='A package connect endpoints to the Hakware Application',  # Short description
     long_description=open('README.md').read(),  # Long description from README
     long_description_content_type='text/markdown',
     author='Jacob O\'Brien',  # Your name
     # author_email='your.email@example.com',  # Your email
     # url='https://github.com/your-username/XGRCPy',  # Your package's URL (if applicable)
     packages=find_packages(),  # Find all sub-packages
```

