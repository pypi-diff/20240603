# Comparing `tmp/timmytimesheet-0.1.tar.gz` & `tmp/timmytimesheet-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timmytimesheet-0.1.tar", last modified: Mon Jun  3 05:13:38 2024, max compression
+gzip compressed data, was "timmytimesheet-0.1.1.tar", last modified: Mon Jun  3 05:19:30 2024, max compression
```

## Comparing `timmytimesheet-0.1.tar` & `timmytimesheet-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 chenry     (501) staff       (20)        0 2024-06-03 05:13:38.155991 timmytimesheet-0.1/
--rw-r--r--   0 chenry     (501) staff       (20)      316 2024-06-03 05:13:38.155819 timmytimesheet-0.1/PKG-INFO
--rw-r--r--   0 chenry     (501) staff       (20)      810 2024-06-01 03:56:36.000000 timmytimesheet-0.1/README.md
-drwxr-xr-x   0 chenry     (501) staff       (20)        0 2024-06-03 05:13:38.154139 timmytimesheet-0.1/common/
--rw-r--r--   0 chenry     (501) staff       (20)     1317 2024-06-01 03:56:36.000000 timmytimesheet-0.1/common/DBHolder.py
--rw-r--r--   0 chenry     (501) staff       (20)     9592 2024-06-01 03:56:36.000000 timmytimesheet-0.1/common/TimeEntry.py
--rw-r--r--   0 chenry     (501) staff       (20)     3810 2024-06-01 05:03:53.000000 timmytimesheet-0.1/common/TimeSheet.py
--rw-r--r--   0 chenry     (501) staff       (20)        0 2024-05-28 05:04:55.000000 timmytimesheet-0.1/common/__init__.py
--rw-r--r--   0 chenry     (501) staff       (20)       38 2024-06-03 05:13:38.156025 timmytimesheet-0.1/setup.cfg
--rw-r--r--   0 chenry     (501) staff       (20)      665 2024-06-03 05:13:27.000000 timmytimesheet-0.1/setup.py
-drwxr-xr-x   0 chenry     (501) staff       (20)        0 2024-06-03 05:13:38.154522 timmytimesheet-0.1/tests/
--rw-r--r--   0 chenry     (501) staff       (20)        0 2024-05-28 05:05:06.000000 timmytimesheet-0.1/tests/__init__.py
--rw-r--r--   0 chenry     (501) staff       (20)     9522 2024-06-01 03:56:36.000000 timmytimesheet-0.1/tests/test_TimeEntry.py
--rw-r--r--   0 chenry     (501) staff       (20)     2428 2024-06-01 05:04:57.000000 timmytimesheet-0.1/tests/test_TimeSheet.py
-drwxr-xr-x   0 chenry     (501) staff       (20)        0 2024-06-03 05:13:38.154806 timmytimesheet-0.1/timmy/
--rw-r--r--   0 chenry     (501) staff       (20)        0 2024-06-03 04:30:47.000000 timmytimesheet-0.1/timmy/__init__.py
--rwxr-xr-x   0 chenry     (501) staff       (20)     2347 2024-06-03 04:40:39.000000 timmytimesheet-0.1/timmy/main.py
-drwxr-xr-x   0 chenry     (501) staff       (20)        0 2024-06-03 05:13:38.155616 timmytimesheet-0.1/timmytimesheet.egg-info/
--rw-r--r--   0 chenry     (501) staff       (20)      316 2024-06-03 05:13:38.000000 timmytimesheet-0.1/timmytimesheet.egg-info/PKG-INFO
--rw-r--r--   0 chenry     (501) staff       (20)      424 2024-06-03 05:13:38.000000 timmytimesheet-0.1/timmytimesheet.egg-info/SOURCES.txt
--rw-r--r--   0 chenry     (501) staff       (20)        1 2024-06-03 05:13:38.000000 timmytimesheet-0.1/timmytimesheet.egg-info/dependency_links.txt
--rw-r--r--   0 chenry     (501) staff       (20)       46 2024-06-03 05:13:38.000000 timmytimesheet-0.1/timmytimesheet.egg-info/entry_points.txt
--rw-r--r--   0 chenry     (501) staff       (20)       11 2024-06-03 05:13:38.000000 timmytimesheet-0.1/timmytimesheet.egg-info/requires.txt
--rw-r--r--   0 chenry     (501) staff       (20)       19 2024-06-03 05:13:38.000000 timmytimesheet-0.1/timmytimesheet.egg-info/top_level.txt
+drwxr-xr-x   0 chenry     (501) staff       (20)        0 2024-06-03 05:19:30.102187 timmytimesheet-0.1.1/
+-rw-r--r--   0 chenry     (501) staff       (20)      318 2024-06-03 05:19:30.101999 timmytimesheet-0.1.1/PKG-INFO
+-rw-r--r--   0 chenry     (501) staff       (20)      810 2024-06-01 03:56:36.000000 timmytimesheet-0.1.1/README.md
+drwxr-xr-x   0 chenry     (501) staff       (20)        0 2024-06-03 05:19:30.100230 timmytimesheet-0.1.1/common/
+-rw-r--r--   0 chenry     (501) staff       (20)     1317 2024-06-01 03:56:36.000000 timmytimesheet-0.1.1/common/DBHolder.py
+-rw-r--r--   0 chenry     (501) staff       (20)     9592 2024-06-01 03:56:36.000000 timmytimesheet-0.1.1/common/TimeEntry.py
+-rw-r--r--   0 chenry     (501) staff       (20)     3810 2024-06-01 05:03:53.000000 timmytimesheet-0.1.1/common/TimeSheet.py
+-rw-r--r--   0 chenry     (501) staff       (20)        0 2024-05-28 05:04:55.000000 timmytimesheet-0.1.1/common/__init__.py
+-rw-r--r--   0 chenry     (501) staff       (20)       38 2024-06-03 05:19:30.102220 timmytimesheet-0.1.1/setup.cfg
+-rw-r--r--   0 chenry     (501) staff       (20)      662 2024-06-03 05:19:11.000000 timmytimesheet-0.1.1/setup.py
+drwxr-xr-x   0 chenry     (501) staff       (20)        0 2024-06-03 05:19:30.100665 timmytimesheet-0.1.1/tests/
+-rw-r--r--   0 chenry     (501) staff       (20)        0 2024-05-28 05:05:06.000000 timmytimesheet-0.1.1/tests/__init__.py
+-rw-r--r--   0 chenry     (501) staff       (20)     9522 2024-06-01 03:56:36.000000 timmytimesheet-0.1.1/tests/test_TimeEntry.py
+-rw-r--r--   0 chenry     (501) staff       (20)     2428 2024-06-01 05:04:57.000000 timmytimesheet-0.1.1/tests/test_TimeSheet.py
+drwxr-xr-x   0 chenry     (501) staff       (20)        0 2024-06-03 05:19:30.100971 timmytimesheet-0.1.1/timmy/
+-rw-r--r--   0 chenry     (501) staff       (20)        0 2024-06-03 04:30:47.000000 timmytimesheet-0.1.1/timmy/__init__.py
+-rwxr-xr-x   0 chenry     (501) staff       (20)     2347 2024-06-03 04:40:39.000000 timmytimesheet-0.1.1/timmy/main.py
+drwxr-xr-x   0 chenry     (501) staff       (20)        0 2024-06-03 05:19:30.101770 timmytimesheet-0.1.1/timmytimesheet.egg-info/
+-rw-r--r--   0 chenry     (501) staff       (20)      318 2024-06-03 05:19:30.000000 timmytimesheet-0.1.1/timmytimesheet.egg-info/PKG-INFO
+-rw-r--r--   0 chenry     (501) staff       (20)      424 2024-06-03 05:19:30.000000 timmytimesheet-0.1.1/timmytimesheet.egg-info/SOURCES.txt
+-rw-r--r--   0 chenry     (501) staff       (20)        1 2024-06-03 05:19:30.000000 timmytimesheet-0.1.1/timmytimesheet.egg-info/dependency_links.txt
+-rw-r--r--   0 chenry     (501) staff       (20)       41 2024-06-03 05:19:30.000000 timmytimesheet-0.1.1/timmytimesheet.egg-info/entry_points.txt
+-rw-r--r--   0 chenry     (501) staff       (20)       11 2024-06-03 05:19:30.000000 timmytimesheet-0.1.1/timmytimesheet.egg-info/requires.txt
+-rw-r--r--   0 chenry     (501) staff       (20)       19 2024-06-03 05:19:30.000000 timmytimesheet-0.1.1/timmytimesheet.egg-info/top_level.txt
```

### Comparing `timmytimesheet-0.1/README.md` & `timmytimesheet-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `timmytimesheet-0.1/common/DBHolder.py` & `timmytimesheet-0.1.1/common/DBHolder.py`

 * *Files identical despite different names*

### Comparing `timmytimesheet-0.1/common/TimeEntry.py` & `timmytimesheet-0.1.1/common/TimeEntry.py`

 * *Files identical despite different names*

### Comparing `timmytimesheet-0.1/common/TimeSheet.py` & `timmytimesheet-0.1.1/common/TimeSheet.py`

 * *Files identical despite different names*

### Comparing `timmytimesheet-0.1/setup.py` & `timmytimesheet-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
         name = "timmytimesheet",
-        version = "0.1",
+        version = "0.1.1",
         description = "a basic timesheeting cli",
         author="jumper385 (Henry Chen)",
         install_package_data=True,
         install_requires = [
             "typer[all]"],
         packages = find_packages(),
         keywords = ["timesheeting"],
         entry_points = {
             'console_scripts': [
-                'timmy-time=timmy.main:app']},
+                'timmy=timmy.main:app']},
         classifiers = [
             'Programming Language :: Python :: 3',
             'License :: OSI Approved :: MIT License',
             'Operating System :: OS Independent',
             ])
```

### Comparing `timmytimesheet-0.1/tests/test_TimeEntry.py` & `timmytimesheet-0.1.1/tests/test_TimeEntry.py`

 * *Files identical despite different names*

### Comparing `timmytimesheet-0.1/tests/test_TimeSheet.py` & `timmytimesheet-0.1.1/tests/test_TimeSheet.py`

 * *Files identical despite different names*

### Comparing `timmytimesheet-0.1/timmy/main.py` & `timmytimesheet-0.1.1/timmy/main.py`

 * *Files identical despite different names*

