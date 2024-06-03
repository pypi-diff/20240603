# Comparing `tmp/deshi_hello_world-0.8.tar.gz` & `tmp/deshi_hello_world-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deshi_hello_world-0.8.tar", last modified: Mon Jun  3 03:19:46 2024, max compression
+gzip compressed data, was "deshi_hello_world-0.9.tar", last modified: Mon Jun  3 03:30:09 2024, max compression
```

## Comparing `deshi_hello_world-0.8.tar` & `deshi_hello_world-0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 deshi     (1000) deshi     (1000)        0 2024-06-03 03:19:46.217100 deshi_hello_world-0.8/
--rw-r--r--   0 deshi     (1000) deshi     (1000)      208 2024-06-03 03:19:46.217100 deshi_hello_world-0.8/PKG-INFO
--rw-r--r--   0 deshi     (1000) deshi     (1000)       33 2024-06-02 18:42:56.000000 deshi_hello_world-0.8/README.md
-drwxr-xr-x   0 deshi     (1000) deshi     (1000)        0 2024-06-03 03:19:46.217100 deshi_hello_world-0.8/deshi_hello_world/
--rw-r--r--   0 deshi     (1000) deshi     (1000)      138 2024-06-03 03:03:20.000000 deshi_hello_world-0.8/deshi_hello_world/__init__.py
--rw-r--r--   0 deshi     (1000) deshi     (1000)      559 2024-06-03 03:03:16.000000 deshi_hello_world-0.8/deshi_hello_world/cli.py
-drwxr-xr-x   0 deshi     (1000) deshi     (1000)        0 2024-06-03 03:19:46.217100 deshi_hello_world-0.8/deshi_hello_world.egg-info/
--rw-r--r--   0 deshi     (1000) deshi     (1000)      208 2024-06-03 03:19:46.000000 deshi_hello_world-0.8/deshi_hello_world.egg-info/PKG-INFO
--rw-r--r--   0 deshi     (1000) deshi     (1000)      357 2024-06-03 03:19:46.000000 deshi_hello_world-0.8/deshi_hello_world.egg-info/SOURCES.txt
--rw-r--r--   0 deshi     (1000) deshi     (1000)        1 2024-06-03 03:19:46.000000 deshi_hello_world-0.8/deshi_hello_world.egg-info/dependency_links.txt
--rw-r--r--   0 deshi     (1000) deshi     (1000)       74 2024-06-03 03:19:46.000000 deshi_hello_world-0.8/deshi_hello_world.egg-info/entry_points.txt
--rw-r--r--   0 deshi     (1000) deshi     (1000)        6 2024-06-03 03:19:46.000000 deshi_hello_world-0.8/deshi_hello_world.egg-info/requires.txt
--rw-r--r--   0 deshi     (1000) deshi     (1000)       18 2024-06-03 03:19:46.000000 deshi_hello_world-0.8/deshi_hello_world.egg-info/top_level.txt
--rw-r--r--   0 deshi     (1000) deshi     (1000)       79 2024-06-03 03:19:46.217100 deshi_hello_world-0.8/setup.cfg
--rw-r--r--   0 deshi     (1000) deshi     (1000)      476 2024-06-03 03:19:40.000000 deshi_hello_world-0.8/setup.py
-drwxr-xr-x   0 deshi     (1000) deshi     (1000)        0 2024-06-03 03:19:46.217100 deshi_hello_world-0.8/tests/
--rw-r--r--   0 deshi     (1000) deshi     (1000)      153 2024-06-03 02:39:21.000000 deshi_hello_world-0.8/tests/test_hello_world.py
+drwxr-xr-x   0 deshi     (1000) deshi     (1000)        0 2024-06-03 03:30:08.996939 deshi_hello_world-0.9/
+-rw-r--r--   0 deshi     (1000) deshi     (1000)      208 2024-06-03 03:30:08.996939 deshi_hello_world-0.9/PKG-INFO
+-rw-r--r--   0 deshi     (1000) deshi     (1000)       33 2024-06-02 18:42:56.000000 deshi_hello_world-0.9/README.md
+drwxr-xr-x   0 deshi     (1000) deshi     (1000)        0 2024-06-03 03:30:08.996939 deshi_hello_world-0.9/deshi_hello_world/
+-rw-r--r--   0 deshi     (1000) deshi     (1000)      235 2024-06-03 03:29:43.000000 deshi_hello_world-0.9/deshi_hello_world/__init__.py
+-rw-r--r--   0 deshi     (1000) deshi     (1000)      669 2024-06-03 03:29:30.000000 deshi_hello_world-0.9/deshi_hello_world/cli.py
+drwxr-xr-x   0 deshi     (1000) deshi     (1000)        0 2024-06-03 03:30:08.996939 deshi_hello_world-0.9/deshi_hello_world.egg-info/
+-rw-r--r--   0 deshi     (1000) deshi     (1000)      208 2024-06-03 03:30:08.000000 deshi_hello_world-0.9/deshi_hello_world.egg-info/PKG-INFO
+-rw-r--r--   0 deshi     (1000) deshi     (1000)      357 2024-06-03 03:30:08.000000 deshi_hello_world-0.9/deshi_hello_world.egg-info/SOURCES.txt
+-rw-r--r--   0 deshi     (1000) deshi     (1000)        1 2024-06-03 03:30:08.000000 deshi_hello_world-0.9/deshi_hello_world.egg-info/dependency_links.txt
+-rw-r--r--   0 deshi     (1000) deshi     (1000)       74 2024-06-03 03:30:08.000000 deshi_hello_world-0.9/deshi_hello_world.egg-info/entry_points.txt
+-rw-r--r--   0 deshi     (1000) deshi     (1000)        6 2024-06-03 03:30:08.000000 deshi_hello_world-0.9/deshi_hello_world.egg-info/requires.txt
+-rw-r--r--   0 deshi     (1000) deshi     (1000)       18 2024-06-03 03:30:08.000000 deshi_hello_world-0.9/deshi_hello_world.egg-info/top_level.txt
+-rw-r--r--   0 deshi     (1000) deshi     (1000)       79 2024-06-03 03:30:08.996939 deshi_hello_world-0.9/setup.cfg
+-rw-r--r--   0 deshi     (1000) deshi     (1000)      476 2024-06-03 03:30:03.000000 deshi_hello_world-0.9/setup.py
+drwxr-xr-x   0 deshi     (1000) deshi     (1000)        0 2024-06-03 03:30:08.996939 deshi_hello_world-0.9/tests/
+-rw-r--r--   0 deshi     (1000) deshi     (1000)      153 2024-06-03 02:39:21.000000 deshi_hello_world-0.9/tests/test_hello_world.py
```

