# Comparing `tmp/hf_download-0.1.tar.gz` & `tmp/hf_download-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hf_download-0.1.tar", last modified: Mon Jun  3 07:15:52 2024, max compression
+gzip compressed data, was "hf_download-0.2.tar", last modified: Mon Jun  3 07:24:23 2024, max compression
```

## Comparing `hf_download-0.1.tar` & `hf_download-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 jfk       (1000) jfk       (1000)        0 2024-06-03 07:15:52.850180 hf_download-0.1/
--rw-rw-r--   0 jfk       (1000) jfk       (1000)    11357 2024-06-03 02:36:11.000000 hf_download-0.1/LICENSE
--rw-rw-r--   0 jfk       (1000) jfk       (1000)     1298 2024-06-03 07:15:52.850180 hf_download-0.1/PKG-INFO
--rw-rw-r--   0 jfk       (1000) jfk       (1000)      814 2024-06-03 07:05:41.000000 hf_download-0.1/README.md
-drwxrwxr-x   0 jfk       (1000) jfk       (1000)        0 2024-06-03 07:15:52.850180 hf_download-0.1/hf_download/
--rw-rw-r--   0 jfk       (1000) jfk       (1000)        0 2024-06-03 00:45:51.000000 hf_download-0.1/hf_download/__init__.py
--rw-rw-r--   0 jfk       (1000) jfk       (1000)     1106 2024-06-03 05:18:58.000000 hf_download-0.1/hf_download/downloader.py
-drwxrwxr-x   0 jfk       (1000) jfk       (1000)        0 2024-06-03 07:15:52.850180 hf_download-0.1/hf_download.egg-info/
--rw-rw-r--   0 jfk       (1000) jfk       (1000)     1298 2024-06-03 07:15:52.000000 hf_download-0.1/hf_download.egg-info/PKG-INFO
--rw-rw-r--   0 jfk       (1000) jfk       (1000)      288 2024-06-03 07:15:52.000000 hf_download-0.1/hf_download.egg-info/SOURCES.txt
--rw-rw-r--   0 jfk       (1000) jfk       (1000)        1 2024-06-03 07:15:52.000000 hf_download-0.1/hf_download.egg-info/dependency_links.txt
--rw-rw-r--   0 jfk       (1000) jfk       (1000)       61 2024-06-03 07:15:52.000000 hf_download-0.1/hf_download.egg-info/entry_points.txt
--rw-rw-r--   0 jfk       (1000) jfk       (1000)       16 2024-06-03 07:15:52.000000 hf_download-0.1/hf_download.egg-info/requires.txt
--rw-rw-r--   0 jfk       (1000) jfk       (1000)       12 2024-06-03 07:15:52.000000 hf_download-0.1/hf_download.egg-info/top_level.txt
--rw-rw-r--   0 jfk       (1000) jfk       (1000)       38 2024-06-03 07:15:52.850180 hf_download-0.1/setup.cfg
--rw-rw-r--   0 jfk       (1000) jfk       (1000)      784 2024-06-03 07:10:48.000000 hf_download-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:24:23.534352 hf_download-0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-06-03 07:24:14.000000 hf_download-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-06-03 07:24:23.534352 hf_download-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-06-03 07:24:14.000000 hf_download-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:24:23.530352 hf_download-0.2/hf_download/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 07:24:14.000000 hf_download-0.2/hf_download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-06-03 07:24:14.000000 hf_download-0.2/hf_download/downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:24:23.534352 hf_download-0.2/hf_download.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-06-03 07:24:23.000000 hf_download-0.2/hf_download.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-06-03 07:24:23.000000 hf_download-0.2/hf_download.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 07:24:23.000000 hf_download-0.2/hf_download.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-06-03 07:24:23.000000 hf_download-0.2/hf_download.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-03 07:24:23.000000 hf_download-0.2/hf_download.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-06-03 07:24:23.000000 hf_download-0.2/hf_download.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 07:24:23.534352 hf_download-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-06-03 07:24:14.000000 hf_download-0.2/setup.py
```

### Comparing `hf_download-0.1/LICENSE` & `hf_download-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hf_download-0.1/README.md` & `hf_download-0.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Hugging Face Downloader
 
 A tool to download models from Hugging Face.
 
 ## Link to PyPI
 
-You can find this package on PyPI: [huggingface_downloader](https://pypi.org/project/huggingface_downloader/)
+You can find this package on PyPI: [hf_downloader](https://pypi.org/project/hf_downloader/)
 
 ## Installation
 
 ```bash
-pip install huggingface_downloader
+pip install hf_downloader
 ```
 
 ## Usage
 
 ```bash
 hf_download user/repo filename
 ```
```

### Comparing `hf_download-0.1/hf_download/downloader.py` & `hf_download-0.2/hf_download/downloader.py`

 * *Files identical despite different names*

### Comparing `hf_download-0.1/setup.py` & `hf_download-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="hf_download",
-    version="0.1",
+    version="0.2",
     packages=find_packages(),
     install_requires=[
         "huggingface_hub",
     ],
     entry_points={
         "console_scripts": [
             "hf_download=hf_download.downloader:main",
```

