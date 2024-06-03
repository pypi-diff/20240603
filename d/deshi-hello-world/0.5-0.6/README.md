# Comparing `tmp/deshi_hello_world-0.5.tar.gz` & `tmp/deshi_hello_world-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deshi_hello_world-0.5.tar", last modified: Mon Jun  3 02:28:50 2024, max compression
+gzip compressed data, was "deshi_hello_world-0.6.tar", last modified: Mon Jun  3 03:00:21 2024, max compression
```

## Comparing `deshi_hello_world-0.5.tar` & `deshi_hello_world-0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 deshi     (1000) deshi     (1000)        0 2024-06-03 02:28:50.327871 deshi_hello_world-0.5/
--rw-r--r--   0 deshi     (1000) deshi     (1000)      171 2024-06-03 02:28:50.327871 deshi_hello_world-0.5/PKG-INFO
--rw-r--r--   0 deshi     (1000) deshi     (1000)       33 2024-06-02 18:42:56.000000 deshi_hello_world-0.5/README.md
-drwxr-xr-x   0 deshi     (1000) deshi     (1000)        0 2024-06-03 02:28:50.317871 deshi_hello_world-0.5/deshi_hello_world/
--rw-r--r--   0 deshi     (1000) deshi     (1000)       90 2024-06-03 02:08:08.000000 deshi_hello_world-0.5/deshi_hello_world/__init__.py
--rw-r--r--   0 deshi     (1000) deshi     (1000)      213 2024-06-02 20:55:43.000000 deshi_hello_world-0.5/deshi_hello_world/cli.py
-drwxr-xr-x   0 deshi     (1000) deshi     (1000)        0 2024-06-03 02:28:50.317871 deshi_hello_world-0.5/deshi_hello_world.egg-info/
--rw-r--r--   0 deshi     (1000) deshi     (1000)      171 2024-06-03 02:28:50.000000 deshi_hello_world-0.5/deshi_hello_world.egg-info/PKG-INFO
--rw-r--r--   0 deshi     (1000) deshi     (1000)      357 2024-06-03 02:28:50.000000 deshi_hello_world-0.5/deshi_hello_world.egg-info/SOURCES.txt
--rw-r--r--   0 deshi     (1000) deshi     (1000)        1 2024-06-03 02:28:50.000000 deshi_hello_world-0.5/deshi_hello_world.egg-info/dependency_links.txt
--rw-r--r--   0 deshi     (1000) deshi     (1000)       66 2024-06-03 02:28:50.000000 deshi_hello_world-0.5/deshi_hello_world.egg-info/entry_points.txt
--rw-r--r--   0 deshi     (1000) deshi     (1000)        6 2024-06-03 02:28:50.000000 deshi_hello_world-0.5/deshi_hello_world.egg-info/requires.txt
--rw-r--r--   0 deshi     (1000) deshi     (1000)       18 2024-06-03 02:28:50.000000 deshi_hello_world-0.5/deshi_hello_world.egg-info/top_level.txt
--rw-r--r--   0 deshi     (1000) deshi     (1000)       79 2024-06-03 02:28:50.327871 deshi_hello_world-0.5/setup.cfg
--rw-r--r--   0 deshi     (1000) deshi     (1000)      432 2024-06-03 02:27:36.000000 deshi_hello_world-0.5/setup.py
-drwxr-xr-x   0 deshi     (1000) deshi     (1000)        0 2024-06-03 02:28:50.317871 deshi_hello_world-0.5/tests/
--rw-r--r--   0 deshi     (1000) deshi     (1000)      148 2024-06-03 02:26:29.000000 deshi_hello_world-0.5/tests/test_hello_world.py
+drwxr-xr-x   0 deshi     (1000) deshi     (1000)        0 2024-06-03 03:00:21.837399 deshi_hello_world-0.6/
+-rw-r--r--   0 deshi     (1000) deshi     (1000)      208 2024-06-03 03:00:21.837399 deshi_hello_world-0.6/PKG-INFO
+-rw-r--r--   0 deshi     (1000) deshi     (1000)       33 2024-06-02 18:42:56.000000 deshi_hello_world-0.6/README.md
+drwxr-xr-x   0 deshi     (1000) deshi     (1000)        0 2024-06-03 03:00:21.837399 deshi_hello_world-0.6/deshi_hello_world/
+-rw-r--r--   0 deshi     (1000) deshi     (1000)      138 2024-06-03 02:59:49.000000 deshi_hello_world-0.6/deshi_hello_world/__init__.py
+-rw-r--r--   0 deshi     (1000) deshi     (1000)      553 2024-06-03 02:59:51.000000 deshi_hello_world-0.6/deshi_hello_world/cli.py
+drwxr-xr-x   0 deshi     (1000) deshi     (1000)        0 2024-06-03 03:00:21.837399 deshi_hello_world-0.6/deshi_hello_world.egg-info/
+-rw-r--r--   0 deshi     (1000) deshi     (1000)      208 2024-06-03 03:00:21.000000 deshi_hello_world-0.6/deshi_hello_world.egg-info/PKG-INFO
+-rw-r--r--   0 deshi     (1000) deshi     (1000)      357 2024-06-03 03:00:21.000000 deshi_hello_world-0.6/deshi_hello_world.egg-info/SOURCES.txt
+-rw-r--r--   0 deshi     (1000) deshi     (1000)        1 2024-06-03 03:00:21.000000 deshi_hello_world-0.6/deshi_hello_world.egg-info/dependency_links.txt
+-rw-r--r--   0 deshi     (1000) deshi     (1000)      104 2024-06-03 03:00:21.000000 deshi_hello_world-0.6/deshi_hello_world.egg-info/entry_points.txt
+-rw-r--r--   0 deshi     (1000) deshi     (1000)        6 2024-06-03 03:00:21.000000 deshi_hello_world-0.6/deshi_hello_world.egg-info/requires.txt
+-rw-r--r--   0 deshi     (1000) deshi     (1000)       18 2024-06-03 03:00:21.000000 deshi_hello_world-0.6/deshi_hello_world.egg-info/top_level.txt
+-rw-r--r--   0 deshi     (1000) deshi     (1000)       79 2024-06-03 03:00:21.837399 deshi_hello_world-0.6/setup.cfg
+-rw-r--r--   0 deshi     (1000) deshi     (1000)      519 2024-06-03 03:00:04.000000 deshi_hello_world-0.6/setup.py
+drwxr-xr-x   0 deshi     (1000) deshi     (1000)        0 2024-06-03 03:00:21.837399 deshi_hello_world-0.6/tests/
+-rw-r--r--   0 deshi     (1000) deshi     (1000)      153 2024-06-03 02:39:21.000000 deshi_hello_world-0.6/tests/test_hello_world.py
```

