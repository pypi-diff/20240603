# Comparing `tmp/balanco_library-0.1.2.tar.gz` & `tmp/balanco_library-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balanco_library-0.1.2.tar", last modified: Mon Jun  3 11:19:37 2024, max compression
+gzip compressed data, was "balanco_library-0.2.0.tar", last modified: Mon Jun  3 11:22:09 2024, max compression
```

## Comparing `balanco_library-0.1.2.tar` & `balanco_library-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 elias      (502) staff       (20)        0 2024-06-03 11:19:37.774274 balanco_library-0.1.2/
--rw-r--r--   0 elias      (502) staff       (20)    11357 2024-01-12 15:15:09.000000 balanco_library-0.1.2/LICENSE
--rw-r--r--   0 elias      (502) staff       (20)       18 2024-06-03 07:45:37.000000 balanco_library-0.1.2/MANIFEST.in
--rw-r--r--   0 elias      (502) staff       (20)      548 2024-06-03 11:19:37.773953 balanco_library-0.1.2/PKG-INFO
--rw-r--r--   0 elias      (502) staff       (20)       59 2024-06-03 07:46:37.000000 balanco_library-0.1.2/README.md
-drwxr-xr-x   0 elias      (502) staff       (20)        0 2024-06-03 11:19:37.769240 balanco_library-0.1.2/balanco/
--rw-r--r--   0 elias      (502) staff       (20)      225 2024-06-03 11:15:42.000000 balanco_library-0.1.2/balanco/__init__.py
--rw-r--r--   0 elias      (502) staff       (20)      182 2024-06-03 11:18:02.000000 balanco_library-0.1.2/balanco/koho.py
-drwxr-xr-x   0 elias      (502) staff       (20)        0 2024-06-03 11:19:37.773244 balanco_library-0.1.2/balanco_library.egg-info/
--rw-r--r--   0 elias      (502) staff       (20)      548 2024-06-03 11:19:37.000000 balanco_library-0.1.2/balanco_library.egg-info/PKG-INFO
--rw-r--r--   0 elias      (502) staff       (20)      268 2024-06-03 11:19:37.000000 balanco_library-0.1.2/balanco_library.egg-info/SOURCES.txt
--rw-r--r--   0 elias      (502) staff       (20)        1 2024-06-03 11:19:37.000000 balanco_library-0.1.2/balanco_library.egg-info/dependency_links.txt
--rw-r--r--   0 elias      (502) staff       (20)        9 2024-06-03 11:19:37.000000 balanco_library-0.1.2/balanco_library.egg-info/requires.txt
--rw-r--r--   0 elias      (502) staff       (20)        8 2024-06-03 11:19:37.000000 balanco_library-0.1.2/balanco_library.egg-info/top_level.txt
--rw-r--r--   0 elias      (502) staff       (20)       38 2024-06-03 11:19:37.774522 balanco_library-0.1.2/setup.cfg
--rw-r--r--   0 elias      (502) staff       (20)      691 2024-06-03 11:19:14.000000 balanco_library-0.1.2/setup.py
+drwxr-xr-x   0 elias      (502) staff       (20)        0 2024-06-03 11:22:09.150293 balanco_library-0.2.0/
+-rw-r--r--   0 elias      (502) staff       (20)    11357 2024-01-12 15:15:09.000000 balanco_library-0.2.0/LICENSE
+-rw-r--r--   0 elias      (502) staff       (20)       18 2024-06-03 07:45:37.000000 balanco_library-0.2.0/MANIFEST.in
+-rw-r--r--   0 elias      (502) staff       (20)      548 2024-06-03 11:22:09.149639 balanco_library-0.2.0/PKG-INFO
+-rw-r--r--   0 elias      (502) staff       (20)       59 2024-06-03 07:46:37.000000 balanco_library-0.2.0/README.md
+drwxr-xr-x   0 elias      (502) staff       (20)        0 2024-06-03 11:22:09.144911 balanco_library-0.2.0/balanco/
+-rw-r--r--   0 elias      (502) staff       (20)      225 2024-06-03 11:15:42.000000 balanco_library-0.2.0/balanco/__init__.py
+-rw-r--r--   0 elias      (502) staff       (20)      182 2024-06-03 11:18:02.000000 balanco_library-0.2.0/balanco/koho.py
+drwxr-xr-x   0 elias      (502) staff       (20)        0 2024-06-03 11:22:09.148829 balanco_library-0.2.0/balanco_library.egg-info/
+-rw-r--r--   0 elias      (502) staff       (20)      548 2024-06-03 11:22:09.000000 balanco_library-0.2.0/balanco_library.egg-info/PKG-INFO
+-rw-r--r--   0 elias      (502) staff       (20)      268 2024-06-03 11:22:09.000000 balanco_library-0.2.0/balanco_library.egg-info/SOURCES.txt
+-rw-r--r--   0 elias      (502) staff       (20)        1 2024-06-03 11:22:09.000000 balanco_library-0.2.0/balanco_library.egg-info/dependency_links.txt
+-rw-r--r--   0 elias      (502) staff       (20)        9 2024-06-03 11:22:09.000000 balanco_library-0.2.0/balanco_library.egg-info/requires.txt
+-rw-r--r--   0 elias      (502) staff       (20)        8 2024-06-03 11:22:09.000000 balanco_library-0.2.0/balanco_library.egg-info/top_level.txt
+-rw-r--r--   0 elias      (502) staff       (20)       38 2024-06-03 11:22:09.150606 balanco_library-0.2.0/setup.cfg
+-rw-r--r--   0 elias      (502) staff       (20)      691 2024-06-03 11:21:59.000000 balanco_library-0.2.0/setup.py
```

### Comparing `balanco_library-0.1.2/LICENSE` & `balanco_library-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `balanco_library-0.1.2/PKG-INFO` & `balanco_library-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balanco_library
-Version: 0.1.2
+Version: 0.2.0
 Summary: A simple example package
 Home-page: https://github.com/balanco-elias/balanco_library
 Author: Elias Isopahkala
 Author-email: elias.isopahkala@balanco.fi
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `balanco_library-0.1.2/balanco_library.egg-info/PKG-INFO` & `balanco_library-0.2.0/balanco_library.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balanco-library
-Version: 0.1.2
+Version: 0.2.0
 Summary: A simple example package
 Home-page: https://github.com/balanco-elias/balanco_library
 Author: Elias Isopahkala
 Author-email: elias.isopahkala@balanco.fi
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

