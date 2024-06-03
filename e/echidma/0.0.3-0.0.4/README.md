# Comparing `tmp/echidma-0.0.3.tar.gz` & `tmp/echidma-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echidma-0.0.3.tar", last modified: Fri May 31 06:01:02 2024, max compression
+gzip compressed data, was "echidma-0.0.4.tar", last modified: Mon Jun  3 02:32:12 2024, max compression
```

## Comparing `echidma-0.0.3.tar` & `echidma-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)        0 2024-05-31 06:01:02.467719 echidma-0.0.3/
--rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)     1071 2024-05-28 22:21:10.000000 echidma-0.0.3/LICENSE
--rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)      576 2024-05-31 06:01:02.467423 echidma-0.0.3/PKG-INFO
--rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)      197 2024-05-30 05:14:43.000000 echidma-0.0.3/README.md
-drwxr-xr-x   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)        0 2024-05-31 06:01:02.464209 echidma-0.0.3/echidma/
--rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)      121 2024-05-30 23:29:41.000000 echidma-0.0.3/echidma/__init__.py
-drwxr-xr-x   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)        0 2024-05-31 06:01:02.465584 echidma-0.0.3/echidma/caching/
--rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)       35 2024-05-28 22:55:50.000000 echidma-0.0.3/echidma/caching/__init__.py
--rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)      461 2024-05-29 04:37:47.000000 echidma-0.0.3/echidma/caching/chunk_cache.py
-drwxr-xr-x   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)        0 2024-05-31 06:01:02.466268 echidma-0.0.3/echidma/config_management/
--rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)       41 2024-05-28 22:54:08.000000 echidma-0.0.3/echidma/config_management/__init__.py
--rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)     4341 2024-05-31 02:53:16.000000 echidma-0.0.3/echidma/config_management/config_manager.py
--rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)     2314 2024-05-30 23:44:05.000000 echidma-0.0.3/echidma/indexer_base.py
--rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)      735 2024-05-30 23:03:19.000000 echidma-0.0.3/echidma/indexer_h5.py
--rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)     1663 2024-05-31 02:56:56.000000 echidma-0.0.3/echidma/indexer_memmap.py
-drwxr-xr-x   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)        0 2024-05-31 06:01:02.467068 echidma-0.0.3/echidma.egg-info/
--rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)      576 2024-05-31 06:01:02.000000 echidma-0.0.3/echidma.egg-info/PKG-INFO
--rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)      428 2024-05-31 06:01:02.000000 echidma-0.0.3/echidma.egg-info/SOURCES.txt
--rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)        1 2024-05-31 06:01:02.000000 echidma-0.0.3/echidma.egg-info/dependency_links.txt
--rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)       86 2024-05-31 06:01:02.000000 echidma-0.0.3/echidma.egg-info/requires.txt
--rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)        8 2024-05-31 06:01:02.000000 echidma-0.0.3/echidma.egg-info/top_level.txt
--rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)       86 2024-05-30 22:22:28.000000 echidma-0.0.3/pyproject.toml
--rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)       38 2024-05-31 06:01:02.467781 echidma-0.0.3/setup.cfg
--rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)      938 2024-05-31 05:14:47.000000 echidma-0.0.3/setup.py
+drwxr-xr-x   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)        0 2024-06-03 02:32:12.585386 echidma-0.0.4/
+-rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)     1071 2024-05-28 22:21:10.000000 echidma-0.0.4/LICENSE
+-rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)      576 2024-06-03 02:32:12.585068 echidma-0.0.4/PKG-INFO
+-rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)      197 2024-05-30 05:14:43.000000 echidma-0.0.4/README.md
+drwxr-xr-x   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)        0 2024-06-03 02:32:12.580360 echidma-0.0.4/echidma/
+-rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)      121 2024-05-30 23:29:41.000000 echidma-0.0.4/echidma/__init__.py
+drwxr-xr-x   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)        0 2024-06-03 02:32:12.582764 echidma-0.0.4/echidma/caching/
+-rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)       35 2024-05-28 22:55:50.000000 echidma-0.0.4/echidma/caching/__init__.py
+-rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)      461 2024-05-29 04:37:47.000000 echidma-0.0.4/echidma/caching/chunk_cache.py
+drwxr-xr-x   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)        0 2024-06-03 02:32:12.583677 echidma-0.0.4/echidma/config_management/
+-rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)       41 2024-05-28 22:54:08.000000 echidma-0.0.4/echidma/config_management/__init__.py
+-rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)     4341 2024-05-31 02:53:16.000000 echidma-0.0.4/echidma/config_management/config_manager.py
+-rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)     2314 2024-05-30 23:44:05.000000 echidma-0.0.4/echidma/indexer_base.py
+-rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)      735 2024-05-30 23:03:19.000000 echidma-0.0.4/echidma/indexer_h5.py
+-rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)     1663 2024-05-31 02:56:56.000000 echidma-0.0.4/echidma/indexer_memmap.py
+drwxr-xr-x   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)        0 2024-06-03 02:32:12.584457 echidma-0.0.4/echidma.egg-info/
+-rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)      576 2024-06-03 02:32:12.000000 echidma-0.0.4/echidma.egg-info/PKG-INFO
+-rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)      428 2024-06-03 02:32:12.000000 echidma-0.0.4/echidma.egg-info/SOURCES.txt
+-rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)        1 2024-06-03 02:32:12.000000 echidma-0.0.4/echidma.egg-info/dependency_links.txt
+-rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)       86 2024-06-03 02:32:12.000000 echidma-0.0.4/echidma.egg-info/requires.txt
+-rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)        8 2024-06-03 02:32:12.000000 echidma-0.0.4/echidma.egg-info/top_level.txt
+-rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)       86 2024-05-30 22:22:28.000000 echidma-0.0.4/pyproject.toml
+-rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)       38 2024-06-03 02:32:12.585444 echidma-0.0.4/setup.cfg
+-rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)      938 2024-06-03 02:32:05.000000 echidma-0.0.4/setup.py
```

### Comparing `echidma-0.0.3/LICENSE` & `echidma-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `echidma-0.0.3/PKG-INFO` & `echidma-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echidma
-Version: 0.0.3
+Version: 0.0.4
 Summary: Embarrassingly Chunky Hard Indexed Data Memory Access
 Home-page: https://github.com/lpin0002/ECHIDMA
 Author: Liam Pinchbeck
 Author-email: Liam.Pinchbeck@monash.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
```

### Comparing `echidma-0.0.3/echidma/config_management/config_manager.py` & `echidma-0.0.4/echidma/config_management/config_manager.py`

 * *Files identical despite different names*

### Comparing `echidma-0.0.3/echidma/indexer_base.py` & `echidma-0.0.4/echidma/indexer_base.py`

 * *Files identical despite different names*

### Comparing `echidma-0.0.3/echidma/indexer_h5.py` & `echidma-0.0.4/echidma/indexer_h5.py`

 * *Files identical despite different names*

### Comparing `echidma-0.0.3/echidma/indexer_memmap.py` & `echidma-0.0.4/echidma/indexer_memmap.py`

 * *Files identical despite different names*

### Comparing `echidma-0.0.3/echidma.egg-info/PKG-INFO` & `echidma-0.0.4/echidma.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echidma
-Version: 0.0.3
+Version: 0.0.4
 Summary: Embarrassingly Chunky Hard Indexed Data Memory Access
 Home-page: https://github.com/lpin0002/ECHIDMA
 Author: Liam Pinchbeck
 Author-email: Liam.Pinchbeck@monash.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
```

### Comparing `echidma-0.0.3/setup.py` & `echidma-0.0.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 setup(name='echidma',
       description='Embarrassingly Chunky Hard Indexed Data Memory Access',
       url='https://github.com/lpin0002/ECHIDMA',
       author='Liam Pinchbeck',
       author_email='Liam.Pinchbeck@monash.edu',
       license="MIT",
-      version='0.0.3',
+      version='0.0.4',
       packages=find_packages(),
 
       # For a lot of the DM spectral classes we require that dict types are ordered
       python_requires='>=3.6',
       install_requires=["scipy==1.11.3",
                         "tqdm>=4.65.0",
                         "numpy>=1.23",
```

