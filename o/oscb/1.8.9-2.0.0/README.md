# Comparing `tmp/oscb-1.8.9.tar.gz` & `tmp/oscb-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oscb-1.8.9.tar", last modified: Wed May  1 01:48:10 2024, max compression
+gzip compressed data, was "oscb-2.0.0.tar", last modified: Mon Jun  3 14:41:13 2024, max compression
```

## Comparing `oscb-1.8.9.tar` & `oscb-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 01:48:10.602944 oscb-1.8.9/
--rw-rw-rw-   0        0        0       26 2024-05-01 01:43:58.000000 oscb-1.8.9/MANIFEST.in
--rw-rw-rw-   0        0        0      658 2024-05-01 01:48:10.601946 oscb-1.8.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-01 01:48:10.542994 oscb-1.8.9/oscb/
--rw-rw-rw-   0        0        0       57 2024-04-29 02:09:08.000000 oscb-1.8.9/oscb/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 01:48:10.600946 oscb-1.8.9/oscb/download_dataset/
--rw-rw-rw-   0        0        0       99 2024-04-30 00:21:20.000000 oscb-1.8.9/oscb/download_dataset/__init__.py
--rw-rw-rw-   0        0        0      193 2024-04-23 23:03:07.000000 oscb-1.8.9/oscb/download_dataset/download_file.py
--rw-rw-rw-   0        0        0     2529 2024-04-23 23:06:51.000000 oscb-1.8.9/oscb/download_dataset/download_utils.py
--rw-rw-rw-   0        0        0      650 2024-05-01 01:47:35.000000 oscb-1.8.9/oscb/version.py
-drwxrwxrwx   0        0        0        0 2024-05-01 01:48:10.574046 oscb-1.8.9/oscb.egg-info/
--rw-rw-rw-   0        0        0      658 2024-05-01 01:48:10.000000 oscb-1.8.9/oscb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-05-01 01:48:10.000000 oscb-1.8.9/oscb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 01:48:10.000000 oscb-1.8.9/oscb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      134 2024-05-01 01:48:10.000000 oscb-1.8.9/oscb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-01 01:48:10.000000 oscb-1.8.9/oscb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 01:48:10.602944 oscb-1.8.9/setup.cfg
--rw-rw-rw-   0        0        0     1801 2024-05-01 01:47:21.000000 oscb-1.8.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 14:41:13.108213 oscb-2.0.0/
+-rw-rw-rw-   0        0        0        2 2024-05-01 03:40:15.000000 oscb-2.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      658 2024-06-03 14:41:13.107257 oscb-2.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-03 14:41:13.052646 oscb-2.0.0/oscb/
+-rw-rw-rw-   0        0        0      100 2024-05-30 16:02:49.000000 oscb-2.0.0/oscb/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 14:41:13.102653 oscb-2.0.0/oscb/clustering/
+-rw-rw-rw-   0        0        0       43 2024-05-30 16:01:51.000000 oscb-2.0.0/oscb/clustering/__init__.py
+-rw-rw-rw-   0        0        0     1826 2024-05-30 16:21:10.000000 oscb-2.0.0/oscb/clustering/clustering_analysis.py
+-rw-rw-rw-   0        0        0      274 2024-05-30 16:19:37.000000 oscb-2.0.0/oscb/clustering/run_clustering.py
+drwxrwxrwx   0        0        0        0 2024-06-03 14:41:13.105702 oscb-2.0.0/oscb/download_dataset/
+-rw-rw-rw-   0        0        0       99 2024-04-30 00:21:20.000000 oscb-2.0.0/oscb/download_dataset/__init__.py
+-rw-rw-rw-   0        0        0      193 2024-04-23 23:03:07.000000 oscb-2.0.0/oscb/download_dataset/download_file.py
+-rw-rw-rw-   0        0        0     2529 2024-04-23 23:06:51.000000 oscb-2.0.0/oscb/download_dataset/download_utils.py
+-rw-rw-rw-   0        0        0      650 2024-05-01 03:45:25.000000 oscb-2.0.0/oscb/version.py
+drwxrwxrwx   0        0        0        0 2024-06-03 14:41:13.096660 oscb-2.0.0/oscb.egg-info/
+-rw-rw-rw-   0        0        0      658 2024-06-03 14:41:12.000000 oscb-2.0.0/oscb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      406 2024-06-03 14:41:12.000000 oscb-2.0.0/oscb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 14:41:12.000000 oscb-2.0.0/oscb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      148 2024-06-03 14:41:12.000000 oscb-2.0.0/oscb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-06-03 14:41:12.000000 oscb-2.0.0/oscb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 14:41:13.108213 oscb-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1117 2024-06-03 14:39:54.000000 oscb-2.0.0/setup.py
```

### Comparing `oscb-1.8.9/PKG-INFO` & `oscb-2.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: oscb
-Version: 1.8.9
+Version: 2.0.0
 Summary: Description of your package
 Home-page: https://github.com/your_username/oscb
-Author: OSCB TEAM
+Author: Your Name
 Author-email: your.email@example.com
 Keywords: sample setuptools development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `oscb-1.8.9/oscb/download_dataset/download_utils.py` & `oscb-2.0.0/oscb/download_dataset/download_utils.py`

 * *Files identical despite different names*

### Comparing `oscb-1.8.9/oscb/version.py` & `oscb-2.0.0/oscb/version.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import logging
 from threading import Thread
 
-__version__ = '1.8.9'
+__version__ = '2.0.0'
 
 try:
     os.environ['OUTDATED_IGNORE'] = '1'
     from outdated import check_outdated  # noqa
 except ImportError:
     check_outdated = None
```

### Comparing `oscb-1.8.9/oscb.egg-info/PKG-INFO` & `oscb-2.0.0/oscb.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: oscb
-Version: 1.8.9
+Version: 2.0.0
 Summary: Description of your package
 Home-page: https://github.com/your_username/oscb
-Author: OSCB TEAM
+Author: Your Name
 Author-email: your.email@example.com
 Keywords: sample setuptools development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

