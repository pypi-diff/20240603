# Comparing `tmp/modrinth_downloader-0.6.tar.gz` & `tmp/modrinth_downloader-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modrinth_downloader-0.6.tar", last modified: Mon Jun  3 12:32:15 2024, max compression
+gzip compressed data, was "modrinth_downloader-0.7.tar", last modified: Mon Jun  3 12:50:45 2024, max compression
```

## Comparing `modrinth_downloader-0.6.tar` & `modrinth_downloader-0.7.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 12:32:15.083449 modrinth_downloader-0.6/
--rw-r--r--   0 tim       (1000) tim       (1000)       20 2024-06-03 12:15:49.000000 modrinth_downloader-0.6/MANIFEST.in
--rw-r--r--   0 tim       (1000) tim       (1000)      426 2024-06-03 12:32:15.083449 modrinth_downloader-0.6/PKG-INFO
--rw-r--r--   0 tim       (1000) tim       (1000)       91 2024-06-02 20:53:13.000000 modrinth_downloader-0.6/README.md
--rw-r--r--   0 tim       (1000) tim       (1000)      179 2024-06-03 11:30:46.000000 modrinth_downloader-0.6/config.toml
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 12:32:15.083449 modrinth_downloader-0.6/modrinth_downloader/
--rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-06-02 20:51:42.000000 modrinth_downloader-0.6/modrinth_downloader/__init__.py
--rw-r--r--   0 tim       (1000) tim       (1000)     1523 2024-06-03 11:23:46.000000 modrinth_downloader-0.6/modrinth_downloader/api.py
--rw-r--r--   0 tim       (1000) tim       (1000)      579 2024-06-03 11:26:30.000000 modrinth_downloader-0.6/modrinth_downloader/downloader.py
--rw-r--r--   0 tim       (1000) tim       (1000)     1021 2024-06-03 11:17:58.000000 modrinth_downloader-0.6/modrinth_downloader/utils.py
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 12:32:15.083449 modrinth_downloader-0.6/modrinth_downloader.egg-info/
--rw-r--r--   0 tim       (1000) tim       (1000)      426 2024-06-03 12:32:15.000000 modrinth_downloader-0.6/modrinth_downloader.egg-info/PKG-INFO
--rw-r--r--   0 tim       (1000) tim       (1000)      513 2024-06-03 12:32:15.000000 modrinth_downloader-0.6/modrinth_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 tim       (1000) tim       (1000)        1 2024-06-03 12:32:15.000000 modrinth_downloader-0.6/modrinth_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 tim       (1000) tim       (1000)       68 2024-06-03 12:32:15.000000 modrinth_downloader-0.6/modrinth_downloader.egg-info/entry_points.txt
--rw-r--r--   0 tim       (1000) tim       (1000)       23 2024-06-03 12:32:15.000000 modrinth_downloader-0.6/modrinth_downloader.egg-info/requires.txt
--rw-r--r--   0 tim       (1000) tim       (1000)       34 2024-06-03 12:32:15.000000 modrinth_downloader-0.6/modrinth_downloader.egg-info/top_level.txt
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 12:32:15.083449 modrinth_downloader-0.6/scripts/
--rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-06-03 12:11:39.000000 modrinth_downloader-0.6/scripts/__init__.py
--rw-r--r--   0 tim       (1000) tim       (1000)     2257 2024-06-03 11:27:35.000000 modrinth_downloader-0.6/scripts/run_downloader.py
--rw-r--r--   0 tim       (1000) tim       (1000)       38 2024-06-03 12:32:15.083449 modrinth_downloader-0.6/setup.cfg
--rw-r--r--   0 tim       (1000) tim       (1000)      901 2024-06-03 12:32:08.000000 modrinth_downloader-0.6/setup.py
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 12:32:15.083449 modrinth_downloader-0.6/tests/
--rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-06-02 20:57:12.000000 modrinth_downloader-0.6/tests/__init__.py
--rw-r--r--   0 tim       (1000) tim       (1000)      341 2024-06-02 20:57:21.000000 modrinth_downloader-0.6/tests/test_downloader.py
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 12:50:45.293519 modrinth_downloader-0.7/
+-rw-r--r--   0 tim       (1000) tim       (1000)       40 2024-06-03 12:44:09.000000 modrinth_downloader-0.7/MANIFEST.in
+-rw-r--r--   0 tim       (1000) tim       (1000)      431 2024-06-03 12:50:45.293519 modrinth_downloader-0.7/PKG-INFO
+-rw-r--r--   0 tim       (1000) tim       (1000)       91 2024-06-02 20:53:13.000000 modrinth_downloader-0.7/README.md
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 12:50:45.293519 modrinth_downloader-0.7/modrinth_downloader/
+-rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-06-02 20:51:42.000000 modrinth_downloader-0.7/modrinth_downloader/__init__.py
+-rw-r--r--   0 tim       (1000) tim       (1000)     1523 2024-06-03 11:23:46.000000 modrinth_downloader-0.7/modrinth_downloader/api.py
+-rw-r--r--   0 tim       (1000) tim       (1000)      579 2024-06-03 11:26:30.000000 modrinth_downloader-0.7/modrinth_downloader/downloader.py
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 12:50:45.293519 modrinth_downloader-0.7/modrinth_downloader/scripts/
+-rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-06-03 12:11:39.000000 modrinth_downloader-0.7/modrinth_downloader/scripts/__init__.py
+-rw-r--r--   0 tim       (1000) tim       (1000)     2412 2024-06-03 12:48:29.000000 modrinth_downloader-0.7/modrinth_downloader/scripts/run_downloader.py
+-rw-r--r--   0 tim       (1000) tim       (1000)     1021 2024-06-03 11:17:58.000000 modrinth_downloader-0.7/modrinth_downloader/utils.py
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 12:50:45.293519 modrinth_downloader-0.7/modrinth_downloader.egg-info/
+-rw-r--r--   0 tim       (1000) tim       (1000)      431 2024-06-03 12:50:45.000000 modrinth_downloader-0.7/modrinth_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 tim       (1000) tim       (1000)      541 2024-06-03 12:50:45.000000 modrinth_downloader-0.7/modrinth_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)        1 2024-06-03 12:50:45.000000 modrinth_downloader-0.7/modrinth_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)       68 2024-06-03 12:50:45.000000 modrinth_downloader-0.7/modrinth_downloader.egg-info/entry_points.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)       23 2024-06-03 12:50:45.000000 modrinth_downloader-0.7/modrinth_downloader.egg-info/requires.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)       26 2024-06-03 12:50:45.000000 modrinth_downloader-0.7/modrinth_downloader.egg-info/top_level.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)       38 2024-06-03 12:50:45.293519 modrinth_downloader-0.7/setup.cfg
+-rw-r--r--   0 tim       (1000) tim       (1000)      942 2024-06-03 12:50:32.000000 modrinth_downloader-0.7/setup.py
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 12:50:45.293519 modrinth_downloader-0.7/tests/
+-rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-06-02 20:57:12.000000 modrinth_downloader-0.7/tests/__init__.py
+-rw-r--r--   0 tim       (1000) tim       (1000)      341 2024-06-02 20:57:21.000000 modrinth_downloader-0.7/tests/test_downloader.py
```

### Comparing `modrinth_downloader-0.6/modrinth_downloader/api.py` & `modrinth_downloader-0.7/modrinth_downloader/api.py`

 * *Files identical despite different names*

### Comparing `modrinth_downloader-0.6/modrinth_downloader/downloader.py` & `modrinth_downloader-0.7/modrinth_downloader/downloader.py`

 * *Files identical despite different names*

### Comparing `modrinth_downloader-0.6/modrinth_downloader/utils.py` & `modrinth_downloader-0.7/modrinth_downloader/utils.py`

 * *Files identical despite different names*

### Comparing `modrinth_downloader-0.6/scripts/run_downloader.py` & `modrinth_downloader-0.7/modrinth_downloader/scripts/run_downloader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from modrinth_downloader.downloader import *
 from modrinth_downloader.utils import *
 import argparse
 import toml
 import os
 
-config = toml.load('../config.toml')
+current_dir = os.path.dirname(os.path.abspath(__file__))
+config_path = os.path.join(current_dir, 'config.toml')
+with open(config_path, 'r') as config_file:
+    config = toml.load(config_file)
 
 config_list_path = config['paths']['lists']
 config_download_path = config['paths']['downloads']
 config_backup_path = config['paths']['backups']
 
 list_path = os.path.expanduser(config_list_path)
 download_path = os.path.expanduser(config_download_path)
```

### Comparing `modrinth_downloader-0.6/setup.py` & `modrinth_downloader-0.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name='modrinth_downloader',
-    version='0.6',
+    version='0.7',
     author='Alexander Brightwater',
-    description="Download projects modrinth",
+    description="Download projects from Modrinth",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
-    packages=find_packages(),
+    packages=find_packages(),  # Automatically find packages
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.11',
     install_requires=[
@@ -21,11 +21,11 @@
     ],
     entry_points={
         'console_scripts': [
             'modrinth_downloader=scripts.run_downloader:main',
         ],
     },
     package_data={
-        '': ['config.toml'],  # Include the config.toml file from the root directory
+        'modrinth_downloader': ['config.toml'],  # Include config.toml within the package
     },
     include_package_data=True,
 )
```

