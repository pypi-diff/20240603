# Comparing `tmp/mzhfunc-0.1.1.tar.gz` & `tmp/mzhfunc-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mzhfunc-0.1.1.tar", last modified: Mon Jun  3 00:55:20 2024, max compression
+gzip compressed data, was "mzhfunc-0.1.2.tar", last modified: Mon Jun  3 01:32:27 2024, max compression
```

## Comparing `mzhfunc-0.1.1.tar` & `mzhfunc-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-06-03 00:55:20.639139 mzhfunc-0.1.1/
-drwxrwxrwx   0        0        0        0 2024-06-03 00:55:20.638166 mzhfunc-0.1.1/MzhFunc.egg-info/
--rw-rw-rw-   0        0        0      397 2024-06-03 00:55:20.000000 mzhfunc-0.1.1/MzhFunc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      171 2024-06-03 00:55:20.000000 mzhfunc-0.1.1/MzhFunc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 00:55:20.000000 mzhfunc-0.1.1/MzhFunc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        3 2024-06-03 00:55:20.000000 mzhfunc-0.1.1/MzhFunc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      397 2024-06-03 00:55:20.639139 mzhfunc-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-06-01 16:57:53.000000 mzhfunc-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-06-03 00:55:20.637193 mzhfunc-0.1.1/db/
--rw-rw-rw-   0        0        0    12418 2024-06-02 15:37:07.000000 mzhfunc-0.1.1/db/MzhFunc.py
--rw-rw-rw-   0        0        0      211 2024-06-02 15:37:07.000000 mzhfunc-0.1.1/db/__init__.py
--rw-rw-rw-   0        0        0       42 2024-06-03 00:55:20.639139 mzhfunc-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     2028 2024-06-03 00:50:55.000000 mzhfunc-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 01:32:27.115087 mzhfunc-0.1.2/
+drwxrwxrwx   0        0        0        0 2024-06-03 01:32:27.113443 mzhfunc-0.1.2/MzhFunc.egg-info/
+-rw-rw-rw-   0        0        0      397 2024-06-03 01:32:27.000000 mzhfunc-0.1.2/MzhFunc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      171 2024-06-03 01:32:27.000000 mzhfunc-0.1.2/MzhFunc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 01:32:27.000000 mzhfunc-0.1.2/MzhFunc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        3 2024-06-03 01:32:27.000000 mzhfunc-0.1.2/MzhFunc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      397 2024-06-03 01:32:27.114417 mzhfunc-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-06-01 16:57:53.000000 mzhfunc-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 01:32:27.112470 mzhfunc-0.1.2/db/
+-rw-rw-rw-   0        0        0    12418 2024-06-02 15:37:07.000000 mzhfunc-0.1.2/db/MzhFunc.py
+-rw-rw-rw-   0        0        0      211 2024-06-02 15:37:07.000000 mzhfunc-0.1.2/db/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-06-03 01:32:27.115087 mzhfunc-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     2028 2024-06-03 00:50:55.000000 mzhfunc-0.1.2/setup.py
```

### Comparing `mzhfunc-0.1.1/db/MzhFunc.py` & `mzhfunc-0.1.2/db/MzhFunc.py`

 * *Files identical despite different names*

### Comparing `mzhfunc-0.1.1/setup.py` & `mzhfunc-0.1.2/setup.py`

 * *Files identical despite different names*

