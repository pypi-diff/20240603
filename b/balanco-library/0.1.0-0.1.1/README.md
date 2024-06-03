# Comparing `tmp/balanco_library-0.1.0.tar.gz` & `tmp/balanco_library-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balanco_library-0.1.0.tar", last modified: Mon Jun  3 09:08:16 2024, max compression
+gzip compressed data, was "balanco_library-0.1.1.tar", last modified: Mon Jun  3 09:47:26 2024, max compression
```

## Comparing `balanco_library-0.1.0.tar` & `balanco_library-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 elias      (502) staff       (20)        0 2024-06-03 09:08:16.942862 balanco_library-0.1.0/
--rw-r--r--   0 elias      (502) staff       (20)    11357 2024-01-12 15:15:09.000000 balanco_library-0.1.0/LICENSE
--rw-r--r--   0 elias      (502) staff       (20)       18 2024-06-03 07:45:37.000000 balanco_library-0.1.0/MANIFEST.in
--rw-r--r--   0 elias      (502) staff       (20)      548 2024-06-03 09:08:16.942435 balanco_library-0.1.0/PKG-INFO
--rw-r--r--   0 elias      (502) staff       (20)       59 2024-06-03 07:46:37.000000 balanco_library-0.1.0/README.md
-drwxr-xr-x   0 elias      (502) staff       (20)        0 2024-06-03 09:08:16.936636 balanco_library-0.1.0/balanco/
--rw-r--r--   0 elias      (502) staff       (20)       40 2024-06-03 07:40:31.000000 balanco_library-0.1.0/balanco/__init__.py
-drwxr-xr-x   0 elias      (502) staff       (20)        0 2024-06-03 09:08:16.941383 balanco_library-0.1.0/balanco_library.egg-info/
--rw-r--r--   0 elias      (502) staff       (20)      548 2024-06-03 09:08:16.000000 balanco_library-0.1.0/balanco_library.egg-info/PKG-INFO
--rw-r--r--   0 elias      (502) staff       (20)      214 2024-06-03 09:08:16.000000 balanco_library-0.1.0/balanco_library.egg-info/SOURCES.txt
--rw-r--r--   0 elias      (502) staff       (20)        1 2024-06-03 09:08:16.000000 balanco_library-0.1.0/balanco_library.egg-info/dependency_links.txt
--rw-r--r--   0 elias      (502) staff       (20)        8 2024-06-03 09:08:16.000000 balanco_library-0.1.0/balanco_library.egg-info/top_level.txt
--rw-r--r--   0 elias      (502) staff       (20)       38 2024-06-03 09:08:16.943035 balanco_library-0.1.0/setup.cfg
--rw-r--r--   0 elias      (502) staff       (20)      641 2024-06-03 09:03:56.000000 balanco_library-0.1.0/setup.py
+drwxr-xr-x   0 elias      (502) staff       (20)        0 2024-06-03 09:47:26.355935 balanco_library-0.1.1/
+-rw-r--r--   0 elias      (502) staff       (20)    11357 2024-01-12 15:15:09.000000 balanco_library-0.1.1/LICENSE
+-rw-r--r--   0 elias      (502) staff       (20)       18 2024-06-03 07:45:37.000000 balanco_library-0.1.1/MANIFEST.in
+-rw-r--r--   0 elias      (502) staff       (20)      548 2024-06-03 09:47:26.355250 balanco_library-0.1.1/PKG-INFO
+-rw-r--r--   0 elias      (502) staff       (20)       59 2024-06-03 07:46:37.000000 balanco_library-0.1.1/README.md
+drwxr-xr-x   0 elias      (502) staff       (20)        0 2024-06-03 09:47:26.349953 balanco_library-0.1.1/balanco/
+-rw-r--r--   0 elias      (502) staff       (20)      124 2024-06-03 09:45:54.000000 balanco_library-0.1.1/balanco/__init__.py
+drwxr-xr-x   0 elias      (502) staff       (20)        0 2024-06-03 09:47:26.354260 balanco_library-0.1.1/balanco_library.egg-info/
+-rw-r--r--   0 elias      (502) staff       (20)      548 2024-06-03 09:47:26.000000 balanco_library-0.1.1/balanco_library.egg-info/PKG-INFO
+-rw-r--r--   0 elias      (502) staff       (20)      214 2024-06-03 09:47:26.000000 balanco_library-0.1.1/balanco_library.egg-info/SOURCES.txt
+-rw-r--r--   0 elias      (502) staff       (20)        1 2024-06-03 09:47:26.000000 balanco_library-0.1.1/balanco_library.egg-info/dependency_links.txt
+-rw-r--r--   0 elias      (502) staff       (20)        8 2024-06-03 09:47:26.000000 balanco_library-0.1.1/balanco_library.egg-info/top_level.txt
+-rw-r--r--   0 elias      (502) staff       (20)       38 2024-06-03 09:47:26.356369 balanco_library-0.1.1/setup.cfg
+-rw-r--r--   0 elias      (502) staff       (20)      641 2024-06-03 09:46:29.000000 balanco_library-0.1.1/setup.py
```

### Comparing `balanco_library-0.1.0/LICENSE` & `balanco_library-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `balanco_library-0.1.0/PKG-INFO` & `balanco_library-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balanco_library
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple example package
 Home-page: https://github.com/balanco-elias/balanco_library
 Author: Elias Isopahkala
 Author-email: elias.isopahkala@balanco.fi
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `balanco_library-0.1.0/balanco_library.egg-info/PKG-INFO` & `balanco_library-0.1.1/balanco_library.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balanco-library
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple example package
 Home-page: https://github.com/balanco-elias/balanco_library
 Author: Elias Isopahkala
 Author-email: elias.isopahkala@balanco.fi
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `balanco_library-0.1.0/setup.py` & `balanco_library-0.1.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='balanco_library',
-    version='0.1.0',
+    version='0.1.1',
     author='Elias Isopahkala',
     author_email='elias.isopahkala@balanco.fi',
     description='A simple example package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/balanco-elias/balanco_library',  # Update with your repo URL
     packages=find_packages(),
```

