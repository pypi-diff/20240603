# Comparing `tmp/modrinth_downloader-0.7.tar.gz` & `tmp/modrinth_downloader-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modrinth_downloader-0.7.tar", last modified: Mon Jun  3 12:50:45 2024, max compression
+gzip compressed data, was "modrinth_downloader-0.8.tar", last modified: Mon Jun  3 13:03:14 2024, max compression
```

## Comparing `modrinth_downloader-0.7.tar` & `modrinth_downloader-0.8.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 12:50:45.293519 modrinth_downloader-0.7/
--rw-r--r--   0 tim       (1000) tim       (1000)       40 2024-06-03 12:44:09.000000 modrinth_downloader-0.7/MANIFEST.in
--rw-r--r--   0 tim       (1000) tim       (1000)      431 2024-06-03 12:50:45.293519 modrinth_downloader-0.7/PKG-INFO
--rw-r--r--   0 tim       (1000) tim       (1000)       91 2024-06-02 20:53:13.000000 modrinth_downloader-0.7/README.md
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 12:50:45.293519 modrinth_downloader-0.7/modrinth_downloader/
--rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-06-02 20:51:42.000000 modrinth_downloader-0.7/modrinth_downloader/__init__.py
--rw-r--r--   0 tim       (1000) tim       (1000)     1523 2024-06-03 11:23:46.000000 modrinth_downloader-0.7/modrinth_downloader/api.py
--rw-r--r--   0 tim       (1000) tim       (1000)      579 2024-06-03 11:26:30.000000 modrinth_downloader-0.7/modrinth_downloader/downloader.py
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 12:50:45.293519 modrinth_downloader-0.7/modrinth_downloader/scripts/
--rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-06-03 12:11:39.000000 modrinth_downloader-0.7/modrinth_downloader/scripts/__init__.py
--rw-r--r--   0 tim       (1000) tim       (1000)     2412 2024-06-03 12:48:29.000000 modrinth_downloader-0.7/modrinth_downloader/scripts/run_downloader.py
--rw-r--r--   0 tim       (1000) tim       (1000)     1021 2024-06-03 11:17:58.000000 modrinth_downloader-0.7/modrinth_downloader/utils.py
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 12:50:45.293519 modrinth_downloader-0.7/modrinth_downloader.egg-info/
--rw-r--r--   0 tim       (1000) tim       (1000)      431 2024-06-03 12:50:45.000000 modrinth_downloader-0.7/modrinth_downloader.egg-info/PKG-INFO
--rw-r--r--   0 tim       (1000) tim       (1000)      541 2024-06-03 12:50:45.000000 modrinth_downloader-0.7/modrinth_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 tim       (1000) tim       (1000)        1 2024-06-03 12:50:45.000000 modrinth_downloader-0.7/modrinth_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 tim       (1000) tim       (1000)       68 2024-06-03 12:50:45.000000 modrinth_downloader-0.7/modrinth_downloader.egg-info/entry_points.txt
--rw-r--r--   0 tim       (1000) tim       (1000)       23 2024-06-03 12:50:45.000000 modrinth_downloader-0.7/modrinth_downloader.egg-info/requires.txt
--rw-r--r--   0 tim       (1000) tim       (1000)       26 2024-06-03 12:50:45.000000 modrinth_downloader-0.7/modrinth_downloader.egg-info/top_level.txt
--rw-r--r--   0 tim       (1000) tim       (1000)       38 2024-06-03 12:50:45.293519 modrinth_downloader-0.7/setup.cfg
--rw-r--r--   0 tim       (1000) tim       (1000)      942 2024-06-03 12:50:32.000000 modrinth_downloader-0.7/setup.py
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 12:50:45.293519 modrinth_downloader-0.7/tests/
--rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-06-02 20:57:12.000000 modrinth_downloader-0.7/tests/__init__.py
--rw-r--r--   0 tim       (1000) tim       (1000)      341 2024-06-02 20:57:21.000000 modrinth_downloader-0.7/tests/test_downloader.py
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 13:03:14.273566 modrinth_downloader-0.8/
+-rw-r--r--   0 tim       (1000) tim       (1000)       48 2024-06-03 13:00:27.000000 modrinth_downloader-0.8/MANIFEST.in
+-rw-r--r--   0 tim       (1000) tim       (1000)      431 2024-06-03 13:03:14.273566 modrinth_downloader-0.8/PKG-INFO
+-rw-r--r--   0 tim       (1000) tim       (1000)       91 2024-06-02 20:53:13.000000 modrinth_downloader-0.8/README.md
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 13:03:14.273566 modrinth_downloader-0.8/modrinth_downloader/
+-rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-06-02 20:51:42.000000 modrinth_downloader-0.8/modrinth_downloader/__init__.py
+-rw-r--r--   0 tim       (1000) tim       (1000)     1523 2024-06-03 11:23:46.000000 modrinth_downloader-0.8/modrinth_downloader/api.py
+-rw-r--r--   0 tim       (1000) tim       (1000)      579 2024-06-03 11:26:30.000000 modrinth_downloader-0.8/modrinth_downloader/downloader.py
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 13:03:14.273566 modrinth_downloader-0.8/modrinth_downloader/scripts/
+-rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-06-03 12:11:39.000000 modrinth_downloader-0.8/modrinth_downloader/scripts/__init__.py
+-rw-r--r--   0 tim       (1000) tim       (1000)      179 2024-06-03 11:30:46.000000 modrinth_downloader-0.8/modrinth_downloader/scripts/config.toml
+-rw-r--r--   0 tim       (1000) tim       (1000)     2412 2024-06-03 12:48:29.000000 modrinth_downloader-0.8/modrinth_downloader/scripts/run_downloader.py
+-rw-r--r--   0 tim       (1000) tim       (1000)     1021 2024-06-03 11:17:58.000000 modrinth_downloader-0.8/modrinth_downloader/utils.py
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 13:03:14.273566 modrinth_downloader-0.8/modrinth_downloader.egg-info/
+-rw-r--r--   0 tim       (1000) tim       (1000)      431 2024-06-03 13:03:14.000000 modrinth_downloader-0.8/modrinth_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 tim       (1000) tim       (1000)      581 2024-06-03 13:03:14.000000 modrinth_downloader-0.8/modrinth_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)        1 2024-06-03 13:03:14.000000 modrinth_downloader-0.8/modrinth_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)       88 2024-06-03 13:03:14.000000 modrinth_downloader-0.8/modrinth_downloader.egg-info/entry_points.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)       23 2024-06-03 13:03:14.000000 modrinth_downloader-0.8/modrinth_downloader.egg-info/requires.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)       26 2024-06-03 13:03:14.000000 modrinth_downloader-0.8/modrinth_downloader.egg-info/top_level.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)       38 2024-06-03 13:03:14.273566 modrinth_downloader-0.8/setup.cfg
+-rw-r--r--   0 tim       (1000) tim       (1000)      970 2024-06-03 13:02:50.000000 modrinth_downloader-0.8/setup.py
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 13:03:14.273566 modrinth_downloader-0.8/tests/
+-rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-06-02 20:57:12.000000 modrinth_downloader-0.8/tests/__init__.py
+-rw-r--r--   0 tim       (1000) tim       (1000)      341 2024-06-02 20:57:21.000000 modrinth_downloader-0.8/tests/test_downloader.py
```

### Comparing `modrinth_downloader-0.7/modrinth_downloader/api.py` & `modrinth_downloader-0.8/modrinth_downloader/api.py`

 * *Files identical despite different names*

### Comparing `modrinth_downloader-0.7/modrinth_downloader/downloader.py` & `modrinth_downloader-0.8/modrinth_downloader/downloader.py`

 * *Files identical despite different names*

### Comparing `modrinth_downloader-0.7/modrinth_downloader/scripts/run_downloader.py` & `modrinth_downloader-0.8/modrinth_downloader/scripts/run_downloader.py`

 * *Files identical despite different names*

### Comparing `modrinth_downloader-0.7/modrinth_downloader/utils.py` & `modrinth_downloader-0.8/modrinth_downloader/utils.py`

 * *Files identical despite different names*

### Comparing `modrinth_downloader-0.7/modrinth_downloader.egg-info/SOURCES.txt` & `modrinth_downloader-0.8/modrinth_downloader.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -8,10 +8,11 @@
 modrinth_downloader.egg-info/PKG-INFO
 modrinth_downloader.egg-info/SOURCES.txt
 modrinth_downloader.egg-info/dependency_links.txt
 modrinth_downloader.egg-info/entry_points.txt
 modrinth_downloader.egg-info/requires.txt
 modrinth_downloader.egg-info/top_level.txt
 modrinth_downloader/scripts/__init__.py
+modrinth_downloader/scripts/config.toml
 modrinth_downloader/scripts/run_downloader.py
 tests/__init__.py
 tests/test_downloader.py
```

### Comparing `modrinth_downloader-0.7/setup.py` & `modrinth_downloader-0.8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='modrinth_downloader',
-    version='0.7',
+    version='0.8',
     author='Alexander Brightwater',
     description="Download projects from Modrinth",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),  # Automatically find packages
     classifiers=[
         'Programming Language :: Python :: 3',
@@ -17,15 +17,15 @@
     install_requires=[
         'requests',
         'toml',
         'argparse',
     ],
     entry_points={
         'console_scripts': [
-            'modrinth_downloader=scripts.run_downloader:main',
+            'modrinth_downloader=modrinth_downloader.scripts.run_downloader:main',
         ],
     },
     package_data={
-        'modrinth_downloader': ['config.toml'],  # Include config.toml within the package
+        'modrinth_downloader.scripts': ['config.toml'],  # Include config.toml within the package
     },
     include_package_data=True,
 )
```

