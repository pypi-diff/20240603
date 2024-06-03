# Comparing `tmp/easyfileops-0.1.60.tar.gz` & `tmp/easyfileops-0.1.70.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyfileops-0.1.60.tar", last modified: Sat Jun  1 20:50:15 2024, max compression
+gzip compressed data, was "easyfileops-0.1.70.tar", last modified: Mon Jun  3 06:33:17 2024, max compression
```

## Comparing `easyfileops-0.1.60.tar` & `easyfileops-0.1.70.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 20:50:15.466295 easyfileops-0.1.60/
-drwxrwxrwx   0        0        0        0 2024-06-01 20:50:15.448711 easyfileops-0.1.60/EasyFileOps/
--rw-rw-rw-   0        0        0        0 2024-06-01 20:12:49.000000 easyfileops-0.1.60/EasyFileOps/__init__.py
--rw-rw-rw-   0        0        0     8301 2024-06-01 20:27:46.000000 easyfileops-0.1.60/EasyFileOps/file.py
-drwxrwxrwx   0        0        0        0 2024-06-01 20:50:15.463868 easyfileops-0.1.60/EasyFileOps.egg-info/
--rw-rw-rw-   0        0        0      157 2024-06-01 20:50:15.000000 easyfileops-0.1.60/EasyFileOps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2024-06-01 20:50:15.000000 easyfileops-0.1.60/EasyFileOps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 20:50:15.000000 easyfileops-0.1.60/EasyFileOps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-06-01 20:50:15.000000 easyfileops-0.1.60/EasyFileOps.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      157 2024-06-01 20:50:15.463868 easyfileops-0.1.60/PKG-INFO
--rw-rw-rw-   0        0        0     1748 2024-06-01 20:27:46.000000 easyfileops-0.1.60/README.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 20:50:15.466295 easyfileops-0.1.60/setup.cfg
--rw-rw-rw-   0        0        0      255 2024-06-01 20:50:09.000000 easyfileops-0.1.60/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 06:33:17.903072 easyfileops-0.1.70/
+drwxrwxrwx   0        0        0        0 2024-06-03 06:33:17.869978 easyfileops-0.1.70/EasyFileOps/
+-rw-rw-rw-   0        0        0     8219 2024-06-03 06:33:02.000000 easyfileops-0.1.70/EasyFileOps/__init__.py
+-rw-rw-rw-   0        0        0     7986 2024-06-03 06:32:50.000000 easyfileops-0.1.70/EasyFileOps/file.py
+drwxrwxrwx   0        0        0        0 2024-06-03 06:33:17.900078 easyfileops-0.1.70/EasyFileOps.egg-info/
+-rw-rw-rw-   0        0        0      157 2024-06-03 06:33:17.000000 easyfileops-0.1.70/EasyFileOps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2024-06-03 06:33:17.000000 easyfileops-0.1.70/EasyFileOps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 06:33:17.000000 easyfileops-0.1.70/EasyFileOps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-06-03 06:33:17.000000 easyfileops-0.1.70/EasyFileOps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      157 2024-06-03 06:33:17.901079 easyfileops-0.1.70/PKG-INFO
+-rw-rw-rw-   0        0        0     1666 2024-06-03 06:32:14.000000 easyfileops-0.1.70/README.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 06:33:17.903072 easyfileops-0.1.70/setup.cfg
+-rw-rw-rw-   0        0        0      255 2024-06-03 06:31:32.000000 easyfileops-0.1.70/setup.py
```

### Comparing `easyfileops-0.1.60/EasyFileOps/file.py` & `easyfileops-0.1.70/EasyFileOps/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,14 @@
 DOCUMENTATION OF EasyFileOps
 ###
 ###
 You can install EasyFileOps via pip:
 pip install EasyFileOps
 ###
 ###
-Importing:
-from EasyFileOps import file as efo (or any name you want)
-###
-###
 EasyFileOps main method is file
 Parameters of file:
 filename (str) - Here write a file name to operate on
 option (str) - Available options: r, r+, rb, rb+, readline, readlines, readable, w, w+, wb, wb+, writelines, writable,
 a, a+, ab, ab+, seekable, flush, detach, fileno, truncate, isatty, split, splitlines
 towrite (str or bytes (optional)) - Content to write in operating file
 seek (int (optional)) - Position in operating file before performing the operation
```

### Comparing `easyfileops-0.1.60/README.txt` & `easyfileops-0.1.70/README.txt`

 * *Files 22% similar despite different names*

```diff
@@ -3,18 +3,14 @@
 DOCUMENTATION OF EasyFileOps
 ###
 ###
 You can install EasyFileOps via pip:
 pip install EasyFileOps
 ###
 ###
-Importing:
-from EasyFileOps import file as efo (or any name you want)
-###
-###
 EasyFileOps main method is file
 Parameters of file:
 filename (str) - Here write a file name to operate on
 option (str) - Available options: r, r+, rb, rb+, readline, readlines, readable, w, w+, wb, wb+, writelines, writable,
 a, a+, ab, ab+, seekable, flush, detach, fileno, truncate, isatty, split, splitlines
 towrite (str or bytes (optional)) - Content to write in operating file
 seek (int (optional)) - Position in operating file before performing the operation
```

