# Comparing `tmp/tileclipper-1.0.1.tar.gz` & `tmp/tileclipper-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tileclipper-1.0.1.tar", last modified: Tue Jan 23 10:10:32 2024, max compression
+gzip compressed data, was "tileclipper-1.0.2.tar", last modified: Mon Jun  3 09:35:09 2024, max compression
```

## Comparing `tileclipper-1.0.1.tar` & `tileclipper-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 10:10:32.208066 tileclipper-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-01-23 10:10:14.000000 tileclipper-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-01-23 10:10:32.208066 tileclipper-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-01-23 10:10:14.000000 tileclipper-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-23 10:10:32.208066 tileclipper-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-01-23 10:10:14.000000 tileclipper-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 10:10:32.204066 tileclipper-1.0.1/tileclipper/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-23 10:10:14.000000 tileclipper-1.0.1/tileclipper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8465 2024-01-23 10:10:14.000000 tileclipper-1.0.1/tileclipper/clipper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 10:10:32.208066 tileclipper-1.0.1/tileclipper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-01-23 10:10:32.000000 tileclipper-1.0.1/tileclipper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-01-23 10:10:32.000000 tileclipper-1.0.1/tileclipper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-23 10:10:32.000000 tileclipper-1.0.1/tileclipper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-01-23 10:10:32.000000 tileclipper-1.0.1/tileclipper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-23 10:10:32.000000 tileclipper-1.0.1/tileclipper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:35:09.304189 tileclipper-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-03 09:34:54.000000 tileclipper-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-06-03 09:35:09.304189 tileclipper-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-06-03 09:34:54.000000 tileclipper-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 09:35:09.304189 tileclipper-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-06-03 09:34:54.000000 tileclipper-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:35:09.304189 tileclipper-1.0.2/tileclipper/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-06-03 09:34:54.000000 tileclipper-1.0.2/tileclipper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-06-03 09:34:54.000000 tileclipper-1.0.2/tileclipper/clipper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:35:09.304189 tileclipper-1.0.2/tileclipper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-06-03 09:35:09.000000 tileclipper-1.0.2/tileclipper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-06-03 09:35:09.000000 tileclipper-1.0.2/tileclipper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 09:35:09.000000 tileclipper-1.0.2/tileclipper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-06-03 09:35:09.000000 tileclipper-1.0.2/tileclipper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-06-03 09:35:09.000000 tileclipper-1.0.2/tileclipper.egg-info/top_level.txt
```

### Comparing `tileclipper-1.0.1/LICENSE` & `tileclipper-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tileclipper-1.0.1/PKG-INFO` & `tileclipper-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tileclipper
-Version: 1.0.1
+Version: 1.0.2
 Summary: The `TileClipper` package enables users to download map tiles within a specified bounding box from a tile server
 Home-page: https://github.com/sijandh35/tileclipper
 Author: Sijan Dhungana
 Author-email: sijandhungana35@gmail.com
 License: GPLv3
 Keywords: map,tile,clip,download,tileclipper
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tileclipper-1.0.1/README.md` & `tileclipper-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tileclipper-1.0.1/setup.py` & `tileclipper-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='tileclipper',
-    version='1.0.1',
+    version='1.0.2',
     description='The `TileClipper` package enables users to download map tiles within a specified bounding box from a tile server',
     author='Sijan Dhungana',
     author_email='sijandhungana35@gmail.com',
     packages=find_packages(),
     package_data={'tileclipper': ['tileclipper/docs/user_guide.md']},
     license='GPLv3',
     url='https://github.com/sijandh35/tileclipper',
```

### Comparing `tileclipper-1.0.1/tileclipper.egg-info/PKG-INFO` & `tileclipper-1.0.2/tileclipper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tileclipper
-Version: 1.0.1
+Version: 1.0.2
 Summary: The `TileClipper` package enables users to download map tiles within a specified bounding box from a tile server
 Home-page: https://github.com/sijandh35/tileclipper
 Author: Sijan Dhungana
 Author-email: sijandhungana35@gmail.com
 License: GPLv3
 Keywords: map,tile,clip,download,tileclipper
 Classifier: Development Status :: 3 - Alpha
```

