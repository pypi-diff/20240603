# Comparing `tmp/prophet_tools-0.95.tar.gz` & `tmp/prophet_tools-0.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prophet_tools-0.95.tar", last modified: Thu May 30 18:29:34 2024, max compression
+gzip compressed data, was "prophet_tools-0.96.tar", last modified: Sun Jun  2 22:25:05 2024, max compression
```

## Comparing `prophet_tools-0.95.tar` & `prophet_tools-0.96.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 18:29:34.168405 prophet_tools-0.95/
--rw-rw-rw-   0        0        0      138 2024-05-30 18:29:34.168405 prophet_tools-0.95/PKG-INFO
--rw-rw-rw-   0        0        0      179 2023-12-24 23:12:27.000000 prophet_tools-0.95/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 18:29:34.163400 prophet_tools-0.95/prophet_tools/
--rw-rw-rw-   0        0        0        0 2024-02-12 01:43:39.000000 prophet_tools-0.95/prophet_tools/__init__.py
--rw-rw-rw-   0        0        0      149 2023-12-24 23:12:27.000000 prophet_tools-0.95/prophet_tools/auto_import.py
--rw-rw-rw-   0        0        0     2025 2024-05-30 18:29:02.000000 prophet_tools-0.95/prophet_tools/file_convertors.py
--rw-rw-rw-   0        0        0      268 2024-02-12 01:41:06.000000 prophet_tools-0.95/prophet_tools/how_to_import.py
--rw-rw-rw-   0        0        0     7558 2024-05-26 18:50:56.000000 prophet_tools-0.95/prophet_tools/my_functions.py
--rw-rw-rw-   0        0        0      463 2024-02-12 01:56:50.000000 prophet_tools-0.95/prophet_tools/parsing.py
--rw-rw-rw-   0        0        0     1287 2024-05-26 18:50:17.000000 prophet_tools-0.95/prophet_tools/terminal.py
--rw-rw-rw-   0        0        0     4164 2023-12-29 20:12:13.000000 prophet_tools-0.95/prophet_tools/всё_подряд.py
-drwxrwxrwx   0        0        0        0 2024-05-30 18:29:34.167402 prophet_tools-0.95/prophet_tools.egg-info/
--rw-rw-rw-   0        0        0      138 2024-05-30 18:29:34.000000 prophet_tools-0.95/prophet_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      449 2024-05-30 18:29:34.000000 prophet_tools-0.95/prophet_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 18:29:34.000000 prophet_tools-0.95/prophet_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-02-12 01:48:06.000000 prophet_tools-0.95/prophet_tools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       14 2024-05-30 18:29:34.000000 prophet_tools-0.95/prophet_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 18:29:34.169403 prophet_tools-0.95/setup.cfg
--rw-rw-rw-   0        0        0      241 2024-05-30 18:29:25.000000 prophet_tools-0.95/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 22:25:05.650555 prophet_tools-0.96/
+-rw-rw-rw-   0        0        0      138 2024-06-02 22:25:05.650555 prophet_tools-0.96/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2023-12-24 23:12:27.000000 prophet_tools-0.96/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 22:25:05.644555 prophet_tools-0.96/prophet_tools/
+-rw-rw-rw-   0        0        0        0 2024-02-12 01:43:39.000000 prophet_tools-0.96/prophet_tools/__init__.py
+-rw-rw-rw-   0        0        0      149 2023-12-24 23:12:27.000000 prophet_tools-0.96/prophet_tools/auto_import.py
+-rw-rw-rw-   0        0        0     2025 2024-05-30 18:29:02.000000 prophet_tools-0.96/prophet_tools/file_convertors.py
+-rw-rw-rw-   0        0        0     1479 2024-06-02 22:24:33.000000 prophet_tools-0.96/prophet_tools/file_info.py
+-rw-rw-rw-   0        0        0      268 2024-02-12 01:41:06.000000 prophet_tools-0.96/prophet_tools/how_to_import.py
+-rw-rw-rw-   0        0        0     7558 2024-05-26 18:50:56.000000 prophet_tools-0.96/prophet_tools/my_functions.py
+-rw-rw-rw-   0        0        0      463 2024-02-12 01:56:50.000000 prophet_tools-0.96/prophet_tools/parsing.py
+-rw-rw-rw-   0        0        0     1287 2024-05-26 18:50:17.000000 prophet_tools-0.96/prophet_tools/terminal.py
+-rw-rw-rw-   0        0        0     4164 2023-12-29 20:12:13.000000 prophet_tools-0.96/prophet_tools/всё_подряд.py
+drwxrwxrwx   0        0        0        0 2024-06-02 22:25:05.650555 prophet_tools-0.96/prophet_tools.egg-info/
+-rw-rw-rw-   0        0        0      138 2024-06-02 22:25:05.000000 prophet_tools-0.96/prophet_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      476 2024-06-02 22:25:05.000000 prophet_tools-0.96/prophet_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 22:25:05.000000 prophet_tools-0.96/prophet_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-02-12 01:48:06.000000 prophet_tools-0.96/prophet_tools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       14 2024-06-02 22:25:05.000000 prophet_tools-0.96/prophet_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 22:25:05.651556 prophet_tools-0.96/setup.cfg
+-rw-rw-rw-   0        0        0      241 2024-06-02 22:24:57.000000 prophet_tools-0.96/setup.py
```

### Comparing `prophet_tools-0.95/prophet_tools/file_convertors.py` & `prophet_tools-0.96/prophet_tools/file_convertors.py`

 * *Files identical despite different names*

### Comparing `prophet_tools-0.95/prophet_tools/my_functions.py` & `prophet_tools-0.96/prophet_tools/my_functions.py`

 * *Files identical despite different names*

### Comparing `prophet_tools-0.95/prophet_tools/terminal.py` & `prophet_tools-0.96/prophet_tools/terminal.py`

 * *Files identical despite different names*

### Comparing `prophet_tools-0.95/prophet_tools/всё_подряд.py` & `prophet_tools-0.96/prophet_tools/всё_подряд.py`

 * *Files identical despite different names*

