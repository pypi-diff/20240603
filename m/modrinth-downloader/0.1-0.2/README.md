# Comparing `tmp/modrinth_downloader-0.1.tar.gz` & `tmp/modrinth_downloader-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modrinth_downloader-0.1.tar", last modified: Mon Jun  3 11:40:39 2024, max compression
+gzip compressed data, was "modrinth_downloader-0.2.tar", last modified: Mon Jun  3 11:59:31 2024, max compression
```

## Comparing `modrinth_downloader-0.1.tar` & `modrinth_downloader-0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 11:40:39.463258 modrinth_downloader-0.1/
--rw-r--r--   0 tim       (1000) tim       (1000)      426 2024-06-03 11:40:39.463258 modrinth_downloader-0.1/PKG-INFO
--rw-r--r--   0 tim       (1000) tim       (1000)       91 2024-06-02 20:53:13.000000 modrinth_downloader-0.1/README.md
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 11:40:39.463258 modrinth_downloader-0.1/modrinth_downloader/
--rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-06-02 20:51:42.000000 modrinth_downloader-0.1/modrinth_downloader/__init__.py
--rw-r--r--   0 tim       (1000) tim       (1000)     1523 2024-06-03 11:23:46.000000 modrinth_downloader-0.1/modrinth_downloader/api.py
--rw-r--r--   0 tim       (1000) tim       (1000)      579 2024-06-03 11:26:30.000000 modrinth_downloader-0.1/modrinth_downloader/downloader.py
--rw-r--r--   0 tim       (1000) tim       (1000)     1021 2024-06-03 11:17:58.000000 modrinth_downloader-0.1/modrinth_downloader/utils.py
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 11:40:39.463258 modrinth_downloader-0.1/modrinth_downloader.egg-info/
--rw-r--r--   0 tim       (1000) tim       (1000)      426 2024-06-03 11:40:39.000000 modrinth_downloader-0.1/modrinth_downloader.egg-info/PKG-INFO
--rw-r--r--   0 tim       (1000) tim       (1000)      443 2024-06-03 11:40:39.000000 modrinth_downloader-0.1/modrinth_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 tim       (1000) tim       (1000)        1 2024-06-03 11:40:39.000000 modrinth_downloader-0.1/modrinth_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 tim       (1000) tim       (1000)       68 2024-06-03 11:40:39.000000 modrinth_downloader-0.1/modrinth_downloader.egg-info/entry_points.txt
--rw-r--r--   0 tim       (1000) tim       (1000)       33 2024-06-03 11:40:39.000000 modrinth_downloader-0.1/modrinth_downloader.egg-info/requires.txt
--rw-r--r--   0 tim       (1000) tim       (1000)       26 2024-06-03 11:40:39.000000 modrinth_downloader-0.1/modrinth_downloader.egg-info/top_level.txt
--rw-r--r--   0 tim       (1000) tim       (1000)       38 2024-06-03 11:40:39.463258 modrinth_downloader-0.1/setup.cfg
--rw-r--r--   0 tim       (1000) tim       (1000)      788 2024-06-03 11:39:05.000000 modrinth_downloader-0.1/setup.py
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 11:40:39.463258 modrinth_downloader-0.1/tests/
--rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-06-02 20:57:12.000000 modrinth_downloader-0.1/tests/__init__.py
--rw-r--r--   0 tim       (1000) tim       (1000)      341 2024-06-02 20:57:21.000000 modrinth_downloader-0.1/tests/test_downloader.py
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 11:59:31.023330 modrinth_downloader-0.2/
+-rw-r--r--   0 tim       (1000) tim       (1000)      426 2024-06-03 11:59:31.023330 modrinth_downloader-0.2/PKG-INFO
+-rw-r--r--   0 tim       (1000) tim       (1000)       91 2024-06-02 20:53:13.000000 modrinth_downloader-0.2/README.md
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 11:59:31.023330 modrinth_downloader-0.2/modrinth_downloader/
+-rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-06-02 20:51:42.000000 modrinth_downloader-0.2/modrinth_downloader/__init__.py
+-rw-r--r--   0 tim       (1000) tim       (1000)     1523 2024-06-03 11:23:46.000000 modrinth_downloader-0.2/modrinth_downloader/api.py
+-rw-r--r--   0 tim       (1000) tim       (1000)      579 2024-06-03 11:26:30.000000 modrinth_downloader-0.2/modrinth_downloader/downloader.py
+-rw-r--r--   0 tim       (1000) tim       (1000)     1021 2024-06-03 11:17:58.000000 modrinth_downloader-0.2/modrinth_downloader/utils.py
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 11:59:31.023330 modrinth_downloader-0.2/modrinth_downloader.egg-info/
+-rw-r--r--   0 tim       (1000) tim       (1000)      426 2024-06-03 11:59:31.000000 modrinth_downloader-0.2/modrinth_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 tim       (1000) tim       (1000)      443 2024-06-03 11:59:31.000000 modrinth_downloader-0.2/modrinth_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)        1 2024-06-03 11:59:31.000000 modrinth_downloader-0.2/modrinth_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)       68 2024-06-03 11:59:31.000000 modrinth_downloader-0.2/modrinth_downloader.egg-info/entry_points.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)       23 2024-06-03 11:59:31.000000 modrinth_downloader-0.2/modrinth_downloader.egg-info/requires.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)       26 2024-06-03 11:59:31.000000 modrinth_downloader-0.2/modrinth_downloader.egg-info/top_level.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)       38 2024-06-03 11:59:31.023330 modrinth_downloader-0.2/setup.cfg
+-rw-r--r--   0 tim       (1000) tim       (1000)      755 2024-06-03 11:56:27.000000 modrinth_downloader-0.2/setup.py
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-06-03 11:59:31.023330 modrinth_downloader-0.2/tests/
+-rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-06-02 20:57:12.000000 modrinth_downloader-0.2/tests/__init__.py
+-rw-r--r--   0 tim       (1000) tim       (1000)      341 2024-06-02 20:57:21.000000 modrinth_downloader-0.2/tests/test_downloader.py
```

### Comparing `modrinth_downloader-0.1/modrinth_downloader/api.py` & `modrinth_downloader-0.2/modrinth_downloader/api.py`

 * *Files identical despite different names*

### Comparing `modrinth_downloader-0.1/modrinth_downloader/downloader.py` & `modrinth_downloader-0.2/modrinth_downloader/downloader.py`

 * *Files identical despite different names*

### Comparing `modrinth_downloader-0.1/modrinth_downloader/utils.py` & `modrinth_downloader-0.2/modrinth_downloader/utils.py`

 * *Files identical despite different names*

### Comparing `modrinth_downloader-0.1/setup.py` & `modrinth_downloader-0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='modrinth_downloader',
-    version='0.1',
+    version='0.2',
     author='Alexander Brightwater',
     description="Download projects modrinth",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
@@ -14,16 +14,14 @@
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.11',
     install_requires=[
         'requests',
         'toml',
         'argparse',
-        'os',
-        'shutil'
     ],
     entry_points={
         'console_scripts': [
             'modrinth_downloader=scripts.run_downloader:main',
         ],
     },
 )
```

