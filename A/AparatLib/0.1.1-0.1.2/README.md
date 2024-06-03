# Comparing `tmp/aparatlib-0.1.1.tar.gz` & `tmp/aparatlib-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aparatlib-0.1.1.tar", last modified: Sun Jun  2 10:55:58 2024, max compression
+gzip compressed data, was "aparatlib-0.1.2.tar", last modified: Mon Jun  3 09:25:48 2024, max compression
```

## Comparing `aparatlib-0.1.1.tar` & `aparatlib-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 10:55:58.994670 aparatlib-0.1.1/
-drwxrwxrwx   0        0        0        0 2024-06-02 10:55:58.993688 aparatlib-0.1.1/AparatLib.egg-info/
--rw-rw-rw-   0        0        0      707 2024-06-02 10:55:58.000000 aparatlib-0.1.1/AparatLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2024-06-02 10:55:58.000000 aparatlib-0.1.1/AparatLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 10:55:58.000000 aparatlib-0.1.1/AparatLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-06-02 10:55:58.000000 aparatlib-0.1.1/AparatLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-06-02 10:55:58.000000 aparatlib-0.1.1/AparatLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1090 2024-06-02 06:49:28.000000 aparatlib-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      707 2024-06-02 10:55:58.993688 aparatlib-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      404 2024-06-02 10:47:18.000000 aparatlib-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-06-02 10:55:58.990132 aparatlib-0.1.1/aparat/
--rw-rw-rw-   0        0        0       52 2024-06-02 06:45:10.000000 aparatlib-0.1.1/aparat/__init__.py
--rw-rw-rw-   0        0        0     9131 2024-06-02 09:34:21.000000 aparatlib-0.1.1/aparat/aparat.py
--rw-rw-rw-   0        0        0       42 2024-06-02 10:55:58.994670 aparatlib-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1241 2024-06-02 10:55:54.000000 aparatlib-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-02 10:55:58.992212 aparatlib-0.1.1/tests/
--rw-rw-rw-   0        0        0        0 2024-06-02 06:44:06.000000 aparatlib-0.1.1/tests/__init__.py
--rw-rw-rw-   0        0        0      977 2024-06-02 09:38:58.000000 aparatlib-0.1.1/tests/test_aparat.py
+drwxrwxrwx   0        0        0        0 2024-06-03 09:25:48.804809 aparatlib-0.1.2/
+drwxrwxrwx   0        0        0        0 2024-06-03 09:25:48.802796 aparatlib-0.1.2/AparatLib.egg-info/
+-rw-rw-rw-   0        0        0      924 2024-06-03 09:25:48.000000 aparatlib-0.1.2/AparatLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-06-03 09:25:48.000000 aparatlib-0.1.2/AparatLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 09:25:48.000000 aparatlib-0.1.2/AparatLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-06-03 09:25:48.000000 aparatlib-0.1.2/AparatLib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-06-03 09:25:48.000000 aparatlib-0.1.2/AparatLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1090 2024-06-02 06:49:28.000000 aparatlib-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      924 2024-06-03 09:25:48.802796 aparatlib-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      404 2024-06-02 10:47:18.000000 aparatlib-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 09:25:48.799918 aparatlib-0.1.2/aparat/
+-rw-rw-rw-   0        0        0       52 2024-06-02 06:45:10.000000 aparatlib-0.1.2/aparat/__init__.py
+-rw-rw-rw-   0        0        0    17528 2024-06-03 09:22:03.000000 aparatlib-0.1.2/aparat/aparat.py
+-rw-rw-rw-   0        0        0       42 2024-06-03 09:25:48.804809 aparatlib-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      790 2024-06-03 09:25:11.000000 aparatlib-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 09:25:48.800839 aparatlib-0.1.2/tests/
+-rw-rw-rw-   0        0        0        0 2024-06-02 06:44:06.000000 aparatlib-0.1.2/tests/__init__.py
+-rw-rw-rw-   0        0        0      977 2024-06-02 09:38:58.000000 aparatlib-0.1.2/tests/test_aparat.py
```

### Comparing `aparatlib-0.1.1/LICENSE` & `aparatlib-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aparatlib-0.1.1/tests/test_aparat.py` & `aparatlib-0.1.2/tests/test_aparat.py`

 * *Files identical despite different names*

