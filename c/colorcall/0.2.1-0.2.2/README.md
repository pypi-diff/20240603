# Comparing `tmp/colorcall-0.2.1.tar.gz` & `tmp/colorcall-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colorcall-0.2.1.tar", last modified: Fri May 31 09:17:20 2024, max compression
+gzip compressed data, was "colorcall-0.2.2.tar", last modified: Mon Jun  3 03:10:05 2024, max compression
```

## Comparing `colorcall-0.2.1.tar` & `colorcall-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 09:17:20.114108 colorcall-0.2.1/
--rw-r--r--   0 root         (0) root         (0)     1013 2024-05-31 09:17:20.114108 colorcall-0.2.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 09:17:20.110108 colorcall-0.2.1/colorcall/
--rw-rw-r--   0 root         (0) root         (0)      584 2024-05-31 09:17:19.000000 colorcall-0.2.1/colorcall/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1172 2024-05-31 09:12:50.000000 colorcall-0.2.1/colorcall/colorizer.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-31 06:18:56.000000 colorcall-0.2.1/colorcall/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 09:17:20.114108 colorcall-0.2.1/colorcall.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1013 2024-05-31 09:17:20.000000 colorcall-0.2.1/colorcall.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      204 2024-05-31 09:17:20.000000 colorcall-0.2.1/colorcall.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 09:17:20.000000 colorcall-0.2.1/colorcall.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-31 09:17:20.000000 colorcall-0.2.1/colorcall.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-31 09:17:20.114108 colorcall-0.2.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      595 2024-05-31 07:47:09.000000 colorcall-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 03:10:05.034549 colorcall-0.2.2/
+-rw-r--r--   0 root         (0) root         (0)     1052 2024-06-03 03:10:05.034549 colorcall-0.2.2/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      743 2024-06-03 03:00:10.000000 colorcall-0.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 03:10:05.030549 colorcall-0.2.2/colorcall/
+-rw-rw-r--   0 root         (0) root         (0)      584 2024-06-03 03:10:04.000000 colorcall-0.2.2/colorcall/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1172 2024-05-31 09:12:50.000000 colorcall-0.2.2/colorcall/colorizer.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-05-31 06:18:56.000000 colorcall-0.2.2/colorcall/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 03:10:05.034549 colorcall-0.2.2/colorcall.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1052 2024-06-03 03:10:05.000000 colorcall-0.2.2/colorcall.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      214 2024-06-03 03:10:05.000000 colorcall-0.2.2/colorcall.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 03:10:05.000000 colorcall-0.2.2/colorcall.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-06-03 03:10:05.000000 colorcall-0.2.2/colorcall.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-06-03 03:10:05.034549 colorcall-0.2.2/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      628 2024-06-03 03:03:41.000000 colorcall-0.2.2/setup.py
```

### Comparing `colorcall-0.2.1/PKG-INFO` & `colorcall-0.2.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: colorcall
-Version: 0.2.1
-Summary: Color call your caracal
-Home-page: https://github.com/Sw1mmeR/colorcall/tree/main
-Author: Mikle Sedrakyan
-License: UNKNOWN
-Platform: UNKNOWN
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-
 ![Logo](https://mykaleidoscope.ru/x/uploads/posts/2022-09/1663623253_4-mykaleidoscope-ru-p-zloi-karakal-pinterest-4.jpg)
 
 # Colorcall
 
 Color call your caracal!
 
 
@@ -37,9 +26,8 @@
 )
 ```
 ```python
 from colorcall import FontStyle, rgb, basic
 
 print(basic("This is bold", style=FontStyle.bold))
 print(rgb("This is italic", style=FontStyle.italic))
-```
-
+```
```

### Comparing `colorcall-0.2.1/colorcall/__init__.py` & `colorcall-0.2.2/colorcall/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .colorizer import Color, FontStyle, _cprint, basic, rgb
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 
 
 def black(text: str) -> None:
     _cprint(text, Color.black)
 
 
 def red(text: str) -> None:
```

### Comparing `colorcall-0.2.1/colorcall/colorizer.py` & `colorcall-0.2.2/colorcall/colorizer.py`

 * *Files identical despite different names*

### Comparing `colorcall-0.2.1/colorcall.egg-info/PKG-INFO` & `colorcall-0.2.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: colorcall
-Version: 0.2.1
+Version: 0.2.2
 Summary: Color call your caracal
 Home-page: https://github.com/Sw1mmeR/colorcall/tree/main
 Author: Mikle Sedrakyan
+Author-email: scriptdefender@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 ![Logo](https://mykaleidoscope.ru/x/uploads/posts/2022-09/1663623253_4-mykaleidoscope-ru-p-zloi-karakal-pinterest-4.jpg)
```

