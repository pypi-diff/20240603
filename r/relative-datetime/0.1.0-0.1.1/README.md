# Comparing `tmp/relative_datetime-0.1.0.tar.gz` & `tmp/relative_datetime-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relative_datetime-0.1.0.tar", last modified: Mon Jun  3 09:01:55 2024, max compression
+gzip compressed data, was "relative_datetime-0.1.1.tar", last modified: Mon Jun  3 09:16:44 2024, max compression
```

## Comparing `relative_datetime-0.1.0.tar` & `relative_datetime-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 mihir      (501) staff       (20)        0 2024-06-03 09:01:55.245930 relative_datetime-0.1.0/
--rw-r--r--   0 mihir      (501) staff       (20)     1063 2024-06-03 08:59:18.000000 relative_datetime-0.1.0/LICENSE
--rw-r--r--   0 mihir      (501) staff       (20)       34 2024-06-03 08:59:18.000000 relative_datetime-0.1.0/MANIFEST.in
--rw-r--r--   0 mihir      (501) staff       (20)     1148 2024-06-03 09:01:55.245707 relative_datetime-0.1.0/PKG-INFO
--rw-r--r--   0 mihir      (501) staff       (20)      590 2024-06-03 08:59:18.000000 relative_datetime-0.1.0/README.md
-drwxr-xr-x   0 mihir      (501) staff       (20)        0 2024-06-03 09:01:55.244040 relative_datetime-0.1.0/relative_datetime/
--rw-r--r--   0 mihir      (501) staff       (20)       42 2024-06-03 08:59:18.000000 relative_datetime-0.1.0/relative_datetime/__init__.py
--rw-r--r--   0 mihir      (501) staff       (20)     1433 2024-06-03 08:59:18.000000 relative_datetime-0.1.0/relative_datetime/datetime_utils.py
-drwxr-xr-x   0 mihir      (501) staff       (20)        0 2024-06-03 09:01:55.245465 relative_datetime-0.1.0/relative_datetime.egg-info/
--rw-r--r--   0 mihir      (501) staff       (20)     1148 2024-06-03 09:01:55.000000 relative_datetime-0.1.0/relative_datetime.egg-info/PKG-INFO
--rw-r--r--   0 mihir      (501) staff       (20)      337 2024-06-03 09:01:55.000000 relative_datetime-0.1.0/relative_datetime.egg-info/SOURCES.txt
--rw-r--r--   0 mihir      (501) staff       (20)        1 2024-06-03 09:01:55.000000 relative_datetime-0.1.0/relative_datetime.egg-info/dependency_links.txt
--rw-r--r--   0 mihir      (501) staff       (20)       21 2024-06-03 09:01:55.000000 relative_datetime-0.1.0/relative_datetime.egg-info/requires.txt
--rw-r--r--   0 mihir      (501) staff       (20)       18 2024-06-03 09:01:55.000000 relative_datetime-0.1.0/relative_datetime.egg-info/top_level.txt
--rw-r--r--   0 mihir      (501) staff       (20)       38 2024-06-03 09:01:55.245987 relative_datetime-0.1.0/setup.cfg
--rw-r--r--   0 mihir      (501) staff       (20)      738 2024-06-03 08:59:18.000000 relative_datetime-0.1.0/setup.py
-drwxr-xr-x   0 mihir      (501) staff       (20)        0 2024-06-03 09:01:55.245208 relative_datetime-0.1.0/tests/
--rw-r--r--   0 mihir      (501) staff       (20)      757 2024-06-03 08:59:18.000000 relative_datetime-0.1.0/tests/test_datetime_utils.py
+drwxr-xr-x   0 mihir      (501) staff       (20)        0 2024-06-03 09:16:44.695200 relative_datetime-0.1.1/
+-rw-r--r--   0 mihir      (501) staff       (20)     1063 2024-06-03 08:59:18.000000 relative_datetime-0.1.1/LICENSE
+-rw-r--r--   0 mihir      (501) staff       (20)       34 2024-06-03 08:59:18.000000 relative_datetime-0.1.1/MANIFEST.in
+-rw-r--r--   0 mihir      (501) staff       (20)     5447 2024-06-03 09:16:44.694894 relative_datetime-0.1.1/PKG-INFO
+-rw-r--r--   0 mihir      (501) staff       (20)     4889 2024-06-03 09:14:57.000000 relative_datetime-0.1.1/README.md
+drwxr-xr-x   0 mihir      (501) staff       (20)        0 2024-06-03 09:16:44.693058 relative_datetime-0.1.1/relative_datetime/
+-rw-r--r--   0 mihir      (501) staff       (20)       42 2024-06-03 08:59:18.000000 relative_datetime-0.1.1/relative_datetime/__init__.py
+-rw-r--r--   0 mihir      (501) staff       (20)     1433 2024-06-03 08:59:18.000000 relative_datetime-0.1.1/relative_datetime/datetime_utils.py
+drwxr-xr-x   0 mihir      (501) staff       (20)        0 2024-06-03 09:16:44.694533 relative_datetime-0.1.1/relative_datetime.egg-info/
+-rw-r--r--   0 mihir      (501) staff       (20)     5447 2024-06-03 09:16:44.000000 relative_datetime-0.1.1/relative_datetime.egg-info/PKG-INFO
+-rw-r--r--   0 mihir      (501) staff       (20)      337 2024-06-03 09:16:44.000000 relative_datetime-0.1.1/relative_datetime.egg-info/SOURCES.txt
+-rw-r--r--   0 mihir      (501) staff       (20)        1 2024-06-03 09:16:44.000000 relative_datetime-0.1.1/relative_datetime.egg-info/dependency_links.txt
+-rw-r--r--   0 mihir      (501) staff       (20)       21 2024-06-03 09:16:44.000000 relative_datetime-0.1.1/relative_datetime.egg-info/requires.txt
+-rw-r--r--   0 mihir      (501) staff       (20)       18 2024-06-03 09:16:44.000000 relative_datetime-0.1.1/relative_datetime.egg-info/top_level.txt
+-rw-r--r--   0 mihir      (501) staff       (20)       38 2024-06-03 09:16:44.695268 relative_datetime-0.1.1/setup.cfg
+-rw-r--r--   0 mihir      (501) staff       (20)      738 2024-06-03 09:16:38.000000 relative_datetime-0.1.1/setup.py
+drwxr-xr-x   0 mihir      (501) staff       (20)        0 2024-06-03 09:16:44.694259 relative_datetime-0.1.1/tests/
+-rw-r--r--   0 mihir      (501) staff       (20)      757 2024-06-03 08:59:18.000000 relative_datetime-0.1.1/tests/test_datetime_utils.py
```

### Comparing `relative_datetime-0.1.0/LICENSE` & `relative_datetime-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `relative_datetime-0.1.0/relative_datetime/datetime_utils.py` & `relative_datetime-0.1.1/relative_datetime/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `relative_datetime-0.1.0/setup.py` & `relative_datetime-0.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='relative-datetime',
-    version='0.1.0',
+    version='0.1.1',
     description='A Python library to get relative datetime strings and parse datetime strings.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Mihir Khandekar',
     author_email='mihirkhandekar@gmail.com',
     url='https://github.com/mihirkhandekar/relative-datetime',
     packages=find_packages(),
```

### Comparing `relative_datetime-0.1.0/tests/test_datetime_utils.py` & `relative_datetime-0.1.1/tests/test_datetime_utils.py`

 * *Files identical despite different names*

