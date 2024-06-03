# Comparing `tmp/hemanth_hello_world-0.7.tar.gz` & `tmp/hemanth_hello_world-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hemanth_hello_world-0.7.tar", last modified: Mon Jun  3 03:12:06 2024, max compression
+gzip compressed data, was "hemanth_hello_world-0.8.tar", last modified: Mon Jun  3 03:31:38 2024, max compression
```

## Comparing `hemanth_hello_world-0.7.tar` & `hemanth_hello_world-0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 hemanth   (1000) hemanth   (1000)        0 2024-06-03 03:12:06.938212 hemanth_hello_world-0.7/
--rw-r--r--   0 hemanth   (1000) hemanth   (1000)       22 2024-06-02 21:04:57.000000 hemanth_hello_world-0.7/LICENSE
--rw-r--r--   0 hemanth   (1000) hemanth   (1000)       53 2024-06-02 21:04:42.000000 hemanth_hello_world-0.7/MANIFEST.in
--rw-r--r--   0 hemanth   (1000) hemanth   (1000)      341 2024-06-03 03:12:06.938212 hemanth_hello_world-0.7/PKG-INFO
--rw-r--r--   0 hemanth   (1000) hemanth   (1000)       59 2024-06-02 18:39:29.000000 hemanth_hello_world-0.7/README.md
-drwxr-xr-x   0 hemanth   (1000) hemanth   (1000)        0 2024-06-03 03:12:06.928213 hemanth_hello_world-0.7/hemanth_hello_world/
--rw-r--r--   0 hemanth   (1000) hemanth   (1000)       56 2024-06-03 03:04:55.000000 hemanth_hello_world-0.7/hemanth_hello_world/__init__.py
--rw-r--r--   0 hemanth   (1000) hemanth   (1000)      479 2024-06-03 03:04:40.000000 hemanth_hello_world-0.7/hemanth_hello_world/cli.py
-drwxr-xr-x   0 hemanth   (1000) hemanth   (1000)        0 2024-06-03 03:12:06.928213 hemanth_hello_world-0.7/hemanth_hello_world.egg-info/
--rw-r--r--   0 hemanth   (1000) hemanth   (1000)      341 2024-06-03 03:12:06.000000 hemanth_hello_world-0.7/hemanth_hello_world.egg-info/PKG-INFO
--rw-r--r--   0 hemanth   (1000) hemanth   (1000)      351 2024-06-03 03:12:06.000000 hemanth_hello_world-0.7/hemanth_hello_world.egg-info/SOURCES.txt
--rw-r--r--   0 hemanth   (1000) hemanth   (1000)        1 2024-06-03 03:12:06.000000 hemanth_hello_world-0.7/hemanth_hello_world.egg-info/dependency_links.txt
--rw-r--r--   0 hemanth   (1000) hemanth   (1000)       58 2024-06-03 03:12:06.000000 hemanth_hello_world-0.7/hemanth_hello_world.egg-info/entry_points.txt
--rw-r--r--   0 hemanth   (1000) hemanth   (1000)       20 2024-06-03 03:12:06.000000 hemanth_hello_world-0.7/hemanth_hello_world.egg-info/top_level.txt
--rw-r--r--   0 hemanth   (1000) hemanth   (1000)       79 2024-06-03 03:12:06.938212 hemanth_hello_world-0.7/setup.cfg
--rw-r--r--   0 hemanth   (1000) hemanth   (1000)      668 2024-06-03 03:11:45.000000 hemanth_hello_world-0.7/setup.py
-drwxr-xr-x   0 hemanth   (1000) hemanth   (1000)        0 2024-06-03 03:12:06.928213 hemanth_hello_world-0.7/tests/
--rw-r--r--   0 hemanth   (1000) hemanth   (1000)      131 2024-06-02 21:15:47.000000 hemanth_hello_world-0.7/tests/test_hello_world.py
+drwxr-xr-x   0 hemanth   (1000) hemanth   (1000)        0 2024-06-03 03:31:38.307974 hemanth_hello_world-0.8/
+-rw-r--r--   0 hemanth   (1000) hemanth   (1000)       22 2024-06-02 21:04:57.000000 hemanth_hello_world-0.8/LICENSE
+-rw-r--r--   0 hemanth   (1000) hemanth   (1000)       53 2024-06-02 21:04:42.000000 hemanth_hello_world-0.8/MANIFEST.in
+-rw-r--r--   0 hemanth   (1000) hemanth   (1000)      341 2024-06-03 03:31:38.307974 hemanth_hello_world-0.8/PKG-INFO
+-rw-r--r--   0 hemanth   (1000) hemanth   (1000)       59 2024-06-02 18:39:29.000000 hemanth_hello_world-0.8/README.md
+drwxr-xr-x   0 hemanth   (1000) hemanth   (1000)        0 2024-06-03 03:31:38.307974 hemanth_hello_world-0.8/hemanth_hello_world/
+-rw-r--r--   0 hemanth   (1000) hemanth   (1000)       64 2024-06-03 03:28:42.000000 hemanth_hello_world-0.8/hemanth_hello_world/__init__.py
+-rw-r--r--   0 hemanth   (1000) hemanth   (1000)      479 2024-06-03 03:29:17.000000 hemanth_hello_world-0.8/hemanth_hello_world/cli.py
+drwxr-xr-x   0 hemanth   (1000) hemanth   (1000)        0 2024-06-03 03:31:38.307974 hemanth_hello_world-0.8/hemanth_hello_world.egg-info/
+-rw-r--r--   0 hemanth   (1000) hemanth   (1000)      341 2024-06-03 03:31:38.000000 hemanth_hello_world-0.8/hemanth_hello_world.egg-info/PKG-INFO
+-rw-r--r--   0 hemanth   (1000) hemanth   (1000)      351 2024-06-03 03:31:38.000000 hemanth_hello_world-0.8/hemanth_hello_world.egg-info/SOURCES.txt
+-rw-r--r--   0 hemanth   (1000) hemanth   (1000)        1 2024-06-03 03:31:38.000000 hemanth_hello_world-0.8/hemanth_hello_world.egg-info/dependency_links.txt
+-rw-r--r--   0 hemanth   (1000) hemanth   (1000)       58 2024-06-03 03:31:38.000000 hemanth_hello_world-0.8/hemanth_hello_world.egg-info/entry_points.txt
+-rw-r--r--   0 hemanth   (1000) hemanth   (1000)       20 2024-06-03 03:31:38.000000 hemanth_hello_world-0.8/hemanth_hello_world.egg-info/top_level.txt
+-rw-r--r--   0 hemanth   (1000) hemanth   (1000)       79 2024-06-03 03:31:38.307974 hemanth_hello_world-0.8/setup.cfg
+-rw-r--r--   0 hemanth   (1000) hemanth   (1000)      668 2024-06-03 03:30:59.000000 hemanth_hello_world-0.8/setup.py
+drwxr-xr-x   0 hemanth   (1000) hemanth   (1000)        0 2024-06-03 03:31:38.307974 hemanth_hello_world-0.8/tests/
+-rw-r--r--   0 hemanth   (1000) hemanth   (1000)      131 2024-06-02 21:15:47.000000 hemanth_hello_world-0.8/tests/test_hello_world.py
```

