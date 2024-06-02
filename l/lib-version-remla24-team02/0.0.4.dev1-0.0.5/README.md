# Comparing `tmp/lib_version_remla24_team02-0.0.4.dev1.tar.gz` & `tmp/lib_version_remla24_team02-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_version_remla24_team02-0.0.4.dev1.tar", last modified: Mon May 13 10:43:01 2024, max compression
+gzip compressed data, was "lib_version_remla24_team02-0.0.5.tar", last modified: Sun Jun  2 22:47:56 2024, max compression
```

## Comparing `lib_version_remla24_team02-0.0.4.dev1.tar` & `lib_version_remla24_team02-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:43:01.264797 lib_version_remla24_team02-0.0.4.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-13 10:42:53.000000 lib_version_remla24_team02-0.0.4.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-13 10:43:01.264797 lib_version_remla24_team02-0.0.4.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-13 10:42:53.000000 lib_version_remla24_team02-0.0.4.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:43:01.264797 lib_version_remla24_team02-0.0.4.dev1/lib_version_remla24_team02/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-13 10:42:53.000000 lib_version_remla24_team02-0.0.4.dev1/lib_version_remla24_team02/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-13 10:42:53.000000 lib_version_remla24_team02-0.0.4.dev1/lib_version_remla24_team02/version_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:43:01.264797 lib_version_remla24_team02-0.0.4.dev1/lib_version_remla24_team02.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-13 10:43:01.000000 lib_version_remla24_team02-0.0.4.dev1/lib_version_remla24_team02.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-13 10:43:01.000000 lib_version_remla24_team02-0.0.4.dev1/lib_version_remla24_team02.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 10:43:01.000000 lib_version_remla24_team02-0.0.4.dev1/lib_version_remla24_team02.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-13 10:43:01.000000 lib_version_remla24_team02-0.0.4.dev1/lib_version_remla24_team02.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 10:43:01.264797 lib_version_remla24_team02-0.0.4.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-13 10:43:01.000000 lib_version_remla24_team02-0.0.4.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:47:56.123867 lib_version_remla24_team02-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-06-02 22:47:41.000000 lib_version_remla24_team02-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-06-02 22:47:56.119867 lib_version_remla24_team02-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-06-02 22:47:41.000000 lib_version_remla24_team02-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:47:56.119867 lib_version_remla24_team02-0.0.5/lib_version_remla24_team02/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-06-02 22:47:41.000000 lib_version_remla24_team02-0.0.5/lib_version_remla24_team02/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-06-02 22:47:41.000000 lib_version_remla24_team02-0.0.5/lib_version_remla24_team02/version_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:47:56.119867 lib_version_remla24_team02-0.0.5/lib_version_remla24_team02.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-06-02 22:47:56.000000 lib_version_remla24_team02-0.0.5/lib_version_remla24_team02.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-06-02 22:47:56.000000 lib_version_remla24_team02-0.0.5/lib_version_remla24_team02.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 22:47:56.000000 lib_version_remla24_team02-0.0.5/lib_version_remla24_team02.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-06-02 22:47:56.000000 lib_version_remla24_team02-0.0.5/lib_version_remla24_team02.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 22:47:56.123867 lib_version_remla24_team02-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-06-02 22:47:55.000000 lib_version_remla24_team02-0.0.5/setup.py
```

### Comparing `lib_version_remla24_team02-0.0.4.dev1/LICENSE` & `lib_version_remla24_team02-0.0.5/LICENSE`

 * *Files identical despite different names*

