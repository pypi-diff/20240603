# Comparing `tmp/pdfdol-0.1.5.tar.gz` & `tmp/pdfdol-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfdol-0.1.5.tar", last modified: Thu May 23 12:27:36 2024, max compression
+gzip compressed data, was "pdfdol-0.1.6.tar", last modified: Mon Jun  3 12:47:45 2024, max compression
```

## Comparing `pdfdol-0.1.5.tar` & `pdfdol-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:27:36.323398 pdfdol-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-23 12:27:12.000000 pdfdol-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-23 12:27:36.323398 pdfdol-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-23 12:27:12.000000 pdfdol-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:27:36.319398 pdfdol-0.1.5/pdfdol/
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-23 12:27:12.000000 pdfdol-0.1.5/pdfdol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-23 12:27:12.000000 pdfdol-0.1.5/pdfdol/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:27:36.323398 pdfdol-0.1.5/pdfdol/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-23 12:27:12.000000 pdfdol-0.1.5/pdfdol/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-23 12:27:12.000000 pdfdol-0.1.5/pdfdol/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-23 12:27:12.000000 pdfdol-0.1.5/pdfdol/tests/utils_for_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-05-23 12:27:16.000000 pdfdol-0.1.5/pdfdol/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:27:36.323398 pdfdol-0.1.5/pdfdol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-23 12:27:36.000000 pdfdol-0.1.5/pdfdol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-23 12:27:36.000000 pdfdol-0.1.5/pdfdol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 12:27:36.000000 pdfdol-0.1.5/pdfdol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 12:27:36.000000 pdfdol-0.1.5/pdfdol.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 12:27:36.000000 pdfdol-0.1.5/pdfdol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-23 12:27:36.000000 pdfdol-0.1.5/pdfdol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-23 12:27:36.323398 pdfdol-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-23 12:27:12.000000 pdfdol-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:47:45.787601 pdfdol-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-06-03 12:46:58.000000 pdfdol-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-06-03 12:47:45.787601 pdfdol-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-06-03 12:46:58.000000 pdfdol-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:47:45.787601 pdfdol-0.1.6/pdfdol/
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-06-03 12:46:58.000000 pdfdol-0.1.6/pdfdol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-06-03 12:46:58.000000 pdfdol-0.1.6/pdfdol/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:47:45.787601 pdfdol-0.1.6/pdfdol/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-06-03 12:46:58.000000 pdfdol-0.1.6/pdfdol/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-06-03 12:46:58.000000 pdfdol-0.1.6/pdfdol/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-06-03 12:46:58.000000 pdfdol-0.1.6/pdfdol/tests/utils_for_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-06-03 12:47:16.000000 pdfdol-0.1.6/pdfdol/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:47:45.787601 pdfdol-0.1.6/pdfdol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-06-03 12:47:45.000000 pdfdol-0.1.6/pdfdol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-06-03 12:47:45.000000 pdfdol-0.1.6/pdfdol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 12:47:45.000000 pdfdol-0.1.6/pdfdol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 12:47:45.000000 pdfdol-0.1.6/pdfdol.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-03 12:47:45.000000 pdfdol-0.1.6/pdfdol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-03 12:47:45.000000 pdfdol-0.1.6/pdfdol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-06-03 12:47:45.787601 pdfdol-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-06-03 12:46:58.000000 pdfdol-0.1.6/setup.py
```

### Comparing `pdfdol-0.1.5/LICENSE` & `pdfdol-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pdfdol-0.1.5/PKG-INFO` & `pdfdol-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfdol
-Version: 0.1.5
+Version: 0.1.6
 Summary: Data Object Layer for PDF data
 Author: OtoSense
 License: mit
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pdfdol-0.1.5/README.md` & `pdfdol-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pdfdol-0.1.5/pdfdol/base.py` & `pdfdol-0.1.6/pdfdol/base.py`

 * *Files identical despite different names*

### Comparing `pdfdol-0.1.5/pdfdol.egg-info/PKG-INFO` & `pdfdol-0.1.6/pdfdol.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfdol
-Version: 0.1.5
+Version: 0.1.6
 Summary: Data Object Layer for PDF data
 Author: OtoSense
 License: mit
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

