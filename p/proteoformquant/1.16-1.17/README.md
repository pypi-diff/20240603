# Comparing `tmp/proteoformquant-1.16.tar.gz` & `tmp/proteoformquant-1.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteoformquant-1.16.tar", last modified: Mon Jun  3 08:53:36 2024, max compression
+gzip compressed data, was "proteoformquant-1.17.tar", last modified: Mon Jun  3 08:53:41 2024, max compression
```

## Comparing `proteoformquant-1.16.tar` & `proteoformquant-1.17.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 agrimaud (332419330) agrimaud (332419330)        0 2024-06-03 08:53:36.128833 proteoformquant-1.16/
--rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)        0 2024-05-29 07:53:15.000000 proteoformquant-1.16/MANIFEST.in
--rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)     5283 2024-06-03 08:53:36.128833 proteoformquant-1.16/PKG-INFO
-drwxrwxr-x   0 agrimaud (332419330) agrimaud (332419330)        0 2024-06-03 08:53:36.128833 proteoformquant-1.16/proteoformquant.egg-info/
--rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)     5283 2024-06-03 08:53:36.000000 proteoformquant-1.16/proteoformquant.egg-info/PKG-INFO
--rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)     1070 2024-06-03 08:53:36.000000 proteoformquant-1.16/proteoformquant.egg-info/SOURCES.txt
--rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)        1 2024-06-03 08:53:36.000000 proteoformquant-1.16/proteoformquant.egg-info/dependency_links.txt
--rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)       57 2024-06-03 08:53:36.000000 proteoformquant-1.16/proteoformquant.egg-info/entry_points.txt
--rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)      349 2024-06-03 08:53:36.000000 proteoformquant-1.16/proteoformquant.egg-info/requires.txt
--rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)       16 2024-06-03 08:53:36.000000 proteoformquant-1.16/proteoformquant.egg-info/top_level.txt
--rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)       38 2024-06-03 08:53:36.128833 proteoformquant-1.16/setup.cfg
--rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)     3372 2024-05-29 07:53:15.000000 proteoformquant-1.16/setup.py
+drwxrwxr-x   0 agrimaud (332419330) agrimaud (332419330)        0 2024-06-03 08:53:41.856828 proteoformquant-1.17/
+-rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)        0 2024-05-29 07:53:15.000000 proteoformquant-1.17/MANIFEST.in
+-rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)     5283 2024-06-03 08:53:41.856828 proteoformquant-1.17/PKG-INFO
+drwxrwxr-x   0 agrimaud (332419330) agrimaud (332419330)        0 2024-06-03 08:53:41.856828 proteoformquant-1.17/proteoformquant.egg-info/
+-rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)     5283 2024-06-03 08:53:41.000000 proteoformquant-1.17/proteoformquant.egg-info/PKG-INFO
+-rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)     1070 2024-06-03 08:53:41.000000 proteoformquant-1.17/proteoformquant.egg-info/SOURCES.txt
+-rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)        1 2024-06-03 08:53:41.000000 proteoformquant-1.17/proteoformquant.egg-info/dependency_links.txt
+-rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)       57 2024-06-03 08:53:41.000000 proteoformquant-1.17/proteoformquant.egg-info/entry_points.txt
+-rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)      349 2024-06-03 08:53:41.000000 proteoformquant-1.17/proteoformquant.egg-info/requires.txt
+-rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)       16 2024-06-03 08:53:41.000000 proteoformquant-1.17/proteoformquant.egg-info/top_level.txt
+-rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)       38 2024-06-03 08:53:41.856828 proteoformquant-1.17/setup.cfg
+-rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)     3372 2024-05-29 07:53:15.000000 proteoformquant-1.17/setup.py
```

### Comparing `proteoformquant-1.16/PKG-INFO` & `proteoformquant-1.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteoformquant
-Version: 1.16
+Version: 1.17
 Summary: A python command line tool for the quantification of peptidoform/proteoforms
 Home-page: 
 Author: Arthur Grimaud
 Author-email: arthur582@hotmail.fr
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `proteoformquant-1.16/proteoformquant.egg-info/PKG-INFO` & `proteoformquant-1.17/proteoformquant.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteoformquant
-Version: 1.16
+Version: 1.17
 Summary: A python command line tool for the quantification of peptidoform/proteoforms
 Home-page: 
 Author: Arthur Grimaud
 Author-email: arthur582@hotmail.fr
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `proteoformquant-1.16/proteoformquant.egg-info/SOURCES.txt` & `proteoformquant-1.17/proteoformquant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `proteoformquant-1.16/setup.py` & `proteoformquant-1.17/setup.py`

 * *Files identical despite different names*

