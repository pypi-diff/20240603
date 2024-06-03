# Comparing `tmp/deshi_hello_world-0.7.tar.gz` & `tmp/deshi_hello_world-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deshi_hello_world-0.7.tar", last modified: Mon Jun  3 03:03:43 2024, max compression
+gzip compressed data, was "deshi_hello_world-0.8.tar", last modified: Mon Jun  3 03:19:46 2024, max compression
```

## Comparing `deshi_hello_world-0.7.tar` & `deshi_hello_world-0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 deshi     (1000) deshi     (1000)        0 2024-06-03 03:03:43.037346 deshi_hello_world-0.7/
--rw-r--r--   0 deshi     (1000) deshi     (1000)      208 2024-06-03 03:03:43.037346 deshi_hello_world-0.7/PKG-INFO
--rw-r--r--   0 deshi     (1000) deshi     (1000)       33 2024-06-02 18:42:56.000000 deshi_hello_world-0.7/README.md
-drwxr-xr-x   0 deshi     (1000) deshi     (1000)        0 2024-06-03 03:03:43.037346 deshi_hello_world-0.7/deshi_hello_world/
--rw-r--r--   0 deshi     (1000) deshi     (1000)      138 2024-06-03 03:03:20.000000 deshi_hello_world-0.7/deshi_hello_world/__init__.py
--rw-r--r--   0 deshi     (1000) deshi     (1000)      559 2024-06-03 03:03:16.000000 deshi_hello_world-0.7/deshi_hello_world/cli.py
-drwxr-xr-x   0 deshi     (1000) deshi     (1000)        0 2024-06-03 03:03:43.037346 deshi_hello_world-0.7/deshi_hello_world.egg-info/
--rw-r--r--   0 deshi     (1000) deshi     (1000)      208 2024-06-03 03:03:42.000000 deshi_hello_world-0.7/deshi_hello_world.egg-info/PKG-INFO
--rw-r--r--   0 deshi     (1000) deshi     (1000)      357 2024-06-03 03:03:43.000000 deshi_hello_world-0.7/deshi_hello_world.egg-info/SOURCES.txt
--rw-r--r--   0 deshi     (1000) deshi     (1000)        1 2024-06-03 03:03:42.000000 deshi_hello_world-0.7/deshi_hello_world.egg-info/dependency_links.txt
--rw-r--r--   0 deshi     (1000) deshi     (1000)      116 2024-06-03 03:03:43.000000 deshi_hello_world-0.7/deshi_hello_world.egg-info/entry_points.txt
--rw-r--r--   0 deshi     (1000) deshi     (1000)        6 2024-06-03 03:03:43.000000 deshi_hello_world-0.7/deshi_hello_world.egg-info/requires.txt
--rw-r--r--   0 deshi     (1000) deshi     (1000)       18 2024-06-03 03:03:43.000000 deshi_hello_world-0.7/deshi_hello_world.egg-info/top_level.txt
--rw-r--r--   0 deshi     (1000) deshi     (1000)       79 2024-06-03 03:03:43.037346 deshi_hello_world-0.7/setup.cfg
--rw-r--r--   0 deshi     (1000) deshi     (1000)      531 2024-06-03 03:03:37.000000 deshi_hello_world-0.7/setup.py
-drwxr-xr-x   0 deshi     (1000) deshi     (1000)        0 2024-06-03 03:03:43.037346 deshi_hello_world-0.7/tests/
--rw-r--r--   0 deshi     (1000) deshi     (1000)      153 2024-06-03 02:39:21.000000 deshi_hello_world-0.7/tests/test_hello_world.py
+drwxr-xr-x   0 deshi     (1000) deshi     (1000)        0 2024-06-03 03:19:46.217100 deshi_hello_world-0.8/
+-rw-r--r--   0 deshi     (1000) deshi     (1000)      208 2024-06-03 03:19:46.217100 deshi_hello_world-0.8/PKG-INFO
+-rw-r--r--   0 deshi     (1000) deshi     (1000)       33 2024-06-02 18:42:56.000000 deshi_hello_world-0.8/README.md
+drwxr-xr-x   0 deshi     (1000) deshi     (1000)        0 2024-06-03 03:19:46.217100 deshi_hello_world-0.8/deshi_hello_world/
+-rw-r--r--   0 deshi     (1000) deshi     (1000)      138 2024-06-03 03:03:20.000000 deshi_hello_world-0.8/deshi_hello_world/__init__.py
+-rw-r--r--   0 deshi     (1000) deshi     (1000)      559 2024-06-03 03:03:16.000000 deshi_hello_world-0.8/deshi_hello_world/cli.py
+drwxr-xr-x   0 deshi     (1000) deshi     (1000)        0 2024-06-03 03:19:46.217100 deshi_hello_world-0.8/deshi_hello_world.egg-info/
+-rw-r--r--   0 deshi     (1000) deshi     (1000)      208 2024-06-03 03:19:46.000000 deshi_hello_world-0.8/deshi_hello_world.egg-info/PKG-INFO
+-rw-r--r--   0 deshi     (1000) deshi     (1000)      357 2024-06-03 03:19:46.000000 deshi_hello_world-0.8/deshi_hello_world.egg-info/SOURCES.txt
+-rw-r--r--   0 deshi     (1000) deshi     (1000)        1 2024-06-03 03:19:46.000000 deshi_hello_world-0.8/deshi_hello_world.egg-info/dependency_links.txt
+-rw-r--r--   0 deshi     (1000) deshi     (1000)       74 2024-06-03 03:19:46.000000 deshi_hello_world-0.8/deshi_hello_world.egg-info/entry_points.txt
+-rw-r--r--   0 deshi     (1000) deshi     (1000)        6 2024-06-03 03:19:46.000000 deshi_hello_world-0.8/deshi_hello_world.egg-info/requires.txt
+-rw-r--r--   0 deshi     (1000) deshi     (1000)       18 2024-06-03 03:19:46.000000 deshi_hello_world-0.8/deshi_hello_world.egg-info/top_level.txt
+-rw-r--r--   0 deshi     (1000) deshi     (1000)       79 2024-06-03 03:19:46.217100 deshi_hello_world-0.8/setup.cfg
+-rw-r--r--   0 deshi     (1000) deshi     (1000)      476 2024-06-03 03:19:40.000000 deshi_hello_world-0.8/setup.py
+drwxr-xr-x   0 deshi     (1000) deshi     (1000)        0 2024-06-03 03:19:46.217100 deshi_hello_world-0.8/tests/
+-rw-r--r--   0 deshi     (1000) deshi     (1000)      153 2024-06-03 02:39:21.000000 deshi_hello_world-0.8/tests/test_hello_world.py
```

### Comparing `deshi_hello_world-0.7/deshi_hello_world/cli.py` & `deshi_hello_world-0.8/deshi_hello_world/cli.py`

 * *Files identical despite different names*

