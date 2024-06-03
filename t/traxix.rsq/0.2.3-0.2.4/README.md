# Comparing `tmp/traxix.rsq-0.2.3.tar.gz` & `tmp/traxix.rsq-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traxix.rsq-0.2.3.tar", last modified: Wed Sep  1 14:25:04 2021, max compression
+gzip compressed data, was "traxix.rsq-0.2.4.tar", last modified: Mon Jun  3 13:20:44 2024, max compression
```

## Comparing `traxix.rsq-0.2.3.tar` & `traxix.rsq-0.2.4.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxr-x   0 trax      (1000) trax      (1000)        0 2021-09-01 14:25:04.505005 traxix.rsq-0.2.3/
--rw-rw-r--   0 trax      (1000) trax      (1000)       86 2021-08-10 15:04:58.000000 traxix.rsq-0.2.3/MANIFEST.in
--rw-rw-r--   0 trax      (1000) trax      (1000)      246 2021-09-01 14:25:04.505005 traxix.rsq-0.2.3/PKG-INFO
--rw-rw-r--   0 trax      (1000) trax      (1000)      971 2021-08-10 14:51:37.000000 traxix.rsq-0.2.3/README.md
--rw-rw-r--   0 trax      (1000) trax      (1000)       46 2021-08-26 10:39:50.000000 traxix.rsq-0.2.3/requirements-dev.txt
--rw-rw-r--   0 trax      (1000) trax      (1000)       51 2021-08-30 07:19:50.000000 traxix.rsq-0.2.3/requirements.txt
--rwxrwxr-x   0 trax      (1000) trax      (1000)      116 2021-08-10 15:06:03.000000 traxix.rsq-0.2.3/rsq
--rw-rw-r--   0 trax      (1000) trax      (1000)      205 2021-09-01 14:25:04.505005 traxix.rsq-0.2.3/setup.cfg
--rw-rw-r--   0 trax      (1000) trax      (1000)      604 2021-09-01 14:24:24.000000 traxix.rsq-0.2.3/setup.py
-drwxrwxr-x   0 trax      (1000) trax      (1000)        0 2021-09-01 14:25:04.505005 traxix.rsq-0.2.3/traxix/
--rw-rw-r--   0 trax      (1000) trax      (1000)        0 2021-08-10 14:43:52.000000 traxix.rsq-0.2.3/traxix/__init__.py
--rw-rw-r--   0 trax      (1000) trax      (1000)     4947 2021-08-29 08:08:41.000000 traxix.rsq-0.2.3/traxix/rsq.py
-drwxrwxr-x   0 trax      (1000) trax      (1000)        0 2021-09-01 14:25:04.505005 traxix.rsq-0.2.3/traxix.rsq.egg-info/
--rw-rw-r--   0 trax      (1000) trax      (1000)      246 2021-09-01 14:25:04.000000 traxix.rsq-0.2.3/traxix.rsq.egg-info/PKG-INFO
--rw-rw-r--   0 trax      (1000) trax      (1000)      284 2021-09-01 14:25:04.000000 traxix.rsq-0.2.3/traxix.rsq.egg-info/SOURCES.txt
--rw-rw-r--   0 trax      (1000) trax      (1000)        1 2021-09-01 14:25:04.000000 traxix.rsq-0.2.3/traxix.rsq.egg-info/dependency_links.txt
--rw-rw-r--   0 trax      (1000) trax      (1000)      104 2021-09-01 14:25:04.000000 traxix.rsq-0.2.3/traxix.rsq.egg-info/requires.txt
--rw-rw-r--   0 trax      (1000) trax      (1000)        7 2021-09-01 14:25:04.000000 traxix.rsq-0.2.3/traxix.rsq.egg-info/top_level.txt
+drwxrwxr-x   0 trax      (1000) trax      (1000)        0 2024-06-03 13:20:44.565078 traxix.rsq-0.2.4/
+-rw-rw-r--   0 trax      (1000) trax      (1000)       86 2024-06-03 13:18:30.000000 traxix.rsq-0.2.4/MANIFEST.in
+-rw-r--r--   0 trax      (1000) trax      (1000)      520 2024-06-03 13:20:44.565078 traxix.rsq-0.2.4/PKG-INFO
+-rw-rw-r--   0 trax      (1000) trax      (1000)      971 2024-06-03 13:18:30.000000 traxix.rsq-0.2.4/README.md
+-rw-rw-r--   0 trax      (1000) trax      (1000)       46 2024-06-03 13:18:30.000000 traxix.rsq-0.2.4/requirements-dev.txt
+-rw-rw-r--   0 trax      (1000) trax      (1000)       42 2024-06-03 13:18:30.000000 traxix.rsq-0.2.4/requirements.txt
+-rwxrwxr-x   0 trax      (1000) trax      (1000)      116 2024-06-03 13:18:30.000000 traxix.rsq-0.2.4/rsq
+-rw-rw-r--   0 trax      (1000) trax      (1000)      205 2024-06-03 13:20:44.565078 traxix.rsq-0.2.4/setup.cfg
+-rw-rw-r--   0 trax      (1000) trax      (1000)      603 2024-06-03 13:20:42.000000 traxix.rsq-0.2.4/setup.py
+drwxrwxr-x   0 trax      (1000) trax      (1000)        0 2024-06-03 13:20:44.565078 traxix.rsq-0.2.4/tests/
+-rw-rw-r--   0 trax      (1000) trax      (1000)     4596 2024-06-03 13:18:30.000000 traxix.rsq-0.2.4/tests/test_rsq.py
+drwxrwxr-x   0 trax      (1000) trax      (1000)        0 2024-06-03 13:20:44.565078 traxix.rsq-0.2.4/traxix/
+-rw-rw-r--   0 trax      (1000) trax      (1000)        0 2024-06-03 13:18:30.000000 traxix.rsq-0.2.4/traxix/__init__.py
+-rw-rw-r--   0 trax      (1000) trax      (1000)     4947 2024-06-03 13:18:30.000000 traxix.rsq-0.2.4/traxix/rsq.py
+drwxrwxr-x   0 trax      (1000) trax      (1000)        0 2024-06-03 13:20:44.565078 traxix.rsq-0.2.4/traxix.rsq.egg-info/
+-rw-r--r--   0 trax      (1000) trax      (1000)      520 2024-06-03 13:20:44.000000 traxix.rsq-0.2.4/traxix.rsq.egg-info/PKG-INFO
+-rw-rw-r--   0 trax      (1000) trax      (1000)      302 2024-06-03 13:20:44.000000 traxix.rsq-0.2.4/traxix.rsq.egg-info/SOURCES.txt
+-rw-rw-r--   0 trax      (1000) trax      (1000)        1 2024-06-03 13:20:44.000000 traxix.rsq-0.2.4/traxix.rsq.egg-info/dependency_links.txt
+-rw-rw-r--   0 trax      (1000) trax      (1000)       95 2024-06-03 13:20:44.000000 traxix.rsq-0.2.4/traxix.rsq.egg-info/requires.txt
+-rw-rw-r--   0 trax      (1000) trax      (1000)        7 2024-06-03 13:20:44.000000 traxix.rsq-0.2.4/traxix.rsq.egg-info/top_level.txt
```

### Comparing `traxix.rsq-0.2.3/README.md` & `traxix.rsq-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `traxix.rsq-0.2.3/setup.py` & `traxix.rsq-0.2.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-from setuptools import setup, find_namespace_packages
-
+from setuptools import find_namespace_packages, setup
 
 with open("requirements.txt") as f:
     required = f.read().splitlines()
     requirements_dev = open("requirements-dev.txt").read().splitlines()
 
     setup(
         name="traxix.rsq",
-        version="0.2.3",
+        version="0.2.4",
         url="https://gitlab.com/traxix/python/rsq",
         packages=find_namespace_packages(include=["traxix"]),
         scripts=["rsq"],
         license="GPLv3",
         author="trax Omar Givernaud",
         author_email="o.givernaud@gmail.com",
         install_requires=required,
```

### Comparing `traxix.rsq-0.2.3/traxix/rsq.py` & `traxix.rsq-0.2.4/traxix/rsq.py`

 * *Files identical despite different names*

