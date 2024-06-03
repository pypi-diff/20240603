# Comparing `tmp/modrinth_downloader-0.3.tar.gz` & `tmp/modrinth_downloader-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modrinth_downloader-0.3.tar", last modified: Mon Jun  3 12:12:08 2024, max compression
+gzip compressed data, was "modrinth_downloader-0.4.tar", last modified: Mon Jun  3 12:16:12 2024, max compression
```

## Comparing `modrinth_downloader-0.3.tar` & `modrinth_downloader-0.4.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 12:12:08.633374 modrinth_downloader-0.3/
--rw-r--r--   0 tim       (1000) tim       (1000)      426 2024-06-03 12:12:08.633374 modrinth_downloader-0.3/PKG-INFO
--rw-r--r--   0 tim       (1000) tim       (1000)       91 2024-06-02 20:53:13.000000 modrinth_downloader-0.3/README.md
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 12:12:08.633374 modrinth_downloader-0.3/modrinth_downloader/
--rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-06-02 20:51:42.000000 modrinth_downloader-0.3/modrinth_downloader/__init__.py
--rw-r--r--   0 tim       (1000) tim       (1000)     1523 2024-06-03 11:23:46.000000 modrinth_downloader-0.3/modrinth_downloader/api.py
--rw-r--r--   0 tim       (1000) tim       (1000)      579 2024-06-03 11:26:30.000000 modrinth_downloader-0.3/modrinth_downloader/downloader.py
--rw-r--r--   0 tim       (1000) tim       (1000)     1021 2024-06-03 11:17:58.000000 modrinth_downloader-0.3/modrinth_downloader/utils.py
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 12:12:08.633374 modrinth_downloader-0.3/modrinth_downloader.egg-info/
--rw-r--r--   0 tim       (1000) tim       (1000)      426 2024-06-03 12:12:08.000000 modrinth_downloader-0.3/modrinth_downloader.egg-info/PKG-INFO
--rw-r--r--   0 tim       (1000) tim       (1000)      489 2024-06-03 12:12:08.000000 modrinth_downloader-0.3/modrinth_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 tim       (1000) tim       (1000)        1 2024-06-03 12:12:08.000000 modrinth_downloader-0.3/modrinth_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 tim       (1000) tim       (1000)       68 2024-06-03 12:12:08.000000 modrinth_downloader-0.3/modrinth_downloader.egg-info/entry_points.txt
--rw-r--r--   0 tim       (1000) tim       (1000)       23 2024-06-03 12:12:08.000000 modrinth_downloader-0.3/modrinth_downloader.egg-info/requires.txt
--rw-r--r--   0 tim       (1000) tim       (1000)       34 2024-06-03 12:12:08.000000 modrinth_downloader-0.3/modrinth_downloader.egg-info/top_level.txt
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 12:12:08.633374 modrinth_downloader-0.3/scripts/
--rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-06-03 12:11:39.000000 modrinth_downloader-0.3/scripts/__init__.py
--rw-r--r--   0 tim       (1000) tim       (1000)     2257 2024-06-03 11:27:35.000000 modrinth_downloader-0.3/scripts/run_downloader.py
--rw-r--r--   0 tim       (1000) tim       (1000)       38 2024-06-03 12:12:08.633374 modrinth_downloader-0.3/setup.cfg
--rw-r--r--   0 tim       (1000) tim       (1000)      755 2024-06-03 12:12:00.000000 modrinth_downloader-0.3/setup.py
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 12:12:08.633374 modrinth_downloader-0.3/tests/
--rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-06-02 20:57:12.000000 modrinth_downloader-0.3/tests/__init__.py
--rw-r--r--   0 tim       (1000) tim       (1000)      341 2024-06-02 20:57:21.000000 modrinth_downloader-0.3/tests/test_downloader.py
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 12:16:12.443391 modrinth_downloader-0.4/
+-rw-r--r--   0 tim       (1000) tim       (1000)       20 2024-06-03 12:15:49.000000 modrinth_downloader-0.4/MANIFEST.in
+-rw-r--r--   0 tim       (1000) tim       (1000)      426 2024-06-03 12:16:12.443391 modrinth_downloader-0.4/PKG-INFO
+-rw-r--r--   0 tim       (1000) tim       (1000)       91 2024-06-02 20:53:13.000000 modrinth_downloader-0.4/README.md
+-rw-r--r--   0 tim       (1000) tim       (1000)      179 2024-06-03 11:30:46.000000 modrinth_downloader-0.4/config.toml
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 12:16:12.443391 modrinth_downloader-0.4/modrinth_downloader/
+-rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-06-02 20:51:42.000000 modrinth_downloader-0.4/modrinth_downloader/__init__.py
+-rw-r--r--   0 tim       (1000) tim       (1000)     1523 2024-06-03 11:23:46.000000 modrinth_downloader-0.4/modrinth_downloader/api.py
+-rw-r--r--   0 tim       (1000) tim       (1000)      579 2024-06-03 11:26:30.000000 modrinth_downloader-0.4/modrinth_downloader/downloader.py
+-rw-r--r--   0 tim       (1000) tim       (1000)     1021 2024-06-03 11:17:58.000000 modrinth_downloader-0.4/modrinth_downloader/utils.py
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 12:16:12.443391 modrinth_downloader-0.4/modrinth_downloader.egg-info/
+-rw-r--r--   0 tim       (1000) tim       (1000)      426 2024-06-03 12:16:12.000000 modrinth_downloader-0.4/modrinth_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 tim       (1000) tim       (1000)      513 2024-06-03 12:16:12.000000 modrinth_downloader-0.4/modrinth_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)        1 2024-06-03 12:16:12.000000 modrinth_downloader-0.4/modrinth_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)       68 2024-06-03 12:16:12.000000 modrinth_downloader-0.4/modrinth_downloader.egg-info/entry_points.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)       23 2024-06-03 12:16:12.000000 modrinth_downloader-0.4/modrinth_downloader.egg-info/requires.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)       34 2024-06-03 12:16:12.000000 modrinth_downloader-0.4/modrinth_downloader.egg-info/top_level.txt
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 12:16:12.443391 modrinth_downloader-0.4/scripts/
+-rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-06-03 12:11:39.000000 modrinth_downloader-0.4/scripts/__init__.py
+-rw-r--r--   0 tim       (1000) tim       (1000)     2257 2024-06-03 11:27:35.000000 modrinth_downloader-0.4/scripts/run_downloader.py
+-rw-r--r--   0 tim       (1000) tim       (1000)       38 2024-06-03 12:16:12.443391 modrinth_downloader-0.4/setup.cfg
+-rw-r--r--   0 tim       (1000) tim       (1000)      845 2024-06-03 12:16:03.000000 modrinth_downloader-0.4/setup.py
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 12:16:12.443391 modrinth_downloader-0.4/tests/
+-rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-06-02 20:57:12.000000 modrinth_downloader-0.4/tests/__init__.py
+-rw-r--r--   0 tim       (1000) tim       (1000)      341 2024-06-02 20:57:21.000000 modrinth_downloader-0.4/tests/test_downloader.py
```

### Comparing `modrinth_downloader-0.3/modrinth_downloader/api.py` & `modrinth_downloader-0.4/modrinth_downloader/api.py`

 * *Files identical despite different names*

### Comparing `modrinth_downloader-0.3/modrinth_downloader/downloader.py` & `modrinth_downloader-0.4/modrinth_downloader/downloader.py`

 * *Files identical despite different names*

### Comparing `modrinth_downloader-0.3/modrinth_downloader/utils.py` & `modrinth_downloader-0.4/modrinth_downloader/utils.py`

 * *Files identical despite different names*

### Comparing `modrinth_downloader-0.3/scripts/run_downloader.py` & `modrinth_downloader-0.4/scripts/run_downloader.py`

 * *Files identical despite different names*

### Comparing `modrinth_downloader-0.3/setup.py` & `modrinth_downloader-0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='modrinth_downloader',
-    version='0.3',
+    version='0.4',
     author='Alexander Brightwater',
     description="Download projects modrinth",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
@@ -20,8 +20,11 @@
         'argparse',
     ],
     entry_points={
         'console_scripts': [
             'modrinth_downloader=scripts.run_downloader:main',
         ],
     },
+    package_data={
+        '': ['config.toml'],  # Include the config.toml file
+    },
 )
```

