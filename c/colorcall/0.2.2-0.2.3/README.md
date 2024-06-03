# Comparing `tmp/colorcall-0.2.2.tar.gz` & `tmp/colorcall-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colorcall-0.2.2.tar", last modified: Mon Jun  3 03:10:05 2024, max compression
+gzip compressed data, was "colorcall-0.2.3.tar", last modified: Mon Jun  3 03:37:38 2024, max compression
```

## Comparing `colorcall-0.2.2.tar` & `colorcall-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 03:10:05.034549 colorcall-0.2.2/
--rw-r--r--   0 root         (0) root         (0)     1052 2024-06-03 03:10:05.034549 colorcall-0.2.2/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      743 2024-06-03 03:00:10.000000 colorcall-0.2.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 03:10:05.030549 colorcall-0.2.2/colorcall/
--rw-rw-r--   0 root         (0) root         (0)      584 2024-06-03 03:10:04.000000 colorcall-0.2.2/colorcall/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1172 2024-05-31 09:12:50.000000 colorcall-0.2.2/colorcall/colorizer.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-31 06:18:56.000000 colorcall-0.2.2/colorcall/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 03:10:05.034549 colorcall-0.2.2/colorcall.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1052 2024-06-03 03:10:05.000000 colorcall-0.2.2/colorcall.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      214 2024-06-03 03:10:05.000000 colorcall-0.2.2/colorcall.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 03:10:05.000000 colorcall-0.2.2/colorcall.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-06-03 03:10:05.000000 colorcall-0.2.2/colorcall.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-06-03 03:10:05.034549 colorcall-0.2.2/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      628 2024-06-03 03:03:41.000000 colorcall-0.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 03:37:38.767497 colorcall-0.2.3/
+-rw-rw-r--   0 root         (0) root         (0)     1072 2024-05-31 10:08:42.000000 colorcall-0.2.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1074 2024-06-03 03:37:38.767497 colorcall-0.2.3/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      743 2024-06-03 03:00:10.000000 colorcall-0.2.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 03:37:38.767497 colorcall-0.2.3/colorcall/
+-rw-rw-r--   0 root         (0) root         (0)      584 2024-06-03 03:37:38.000000 colorcall-0.2.3/colorcall/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1172 2024-05-31 09:12:50.000000 colorcall-0.2.3/colorcall/colorizer.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-05-31 06:18:56.000000 colorcall-0.2.3/colorcall/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 03:37:38.767497 colorcall-0.2.3/colorcall.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1074 2024-06-03 03:37:38.000000 colorcall-0.2.3/colorcall.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      222 2024-06-03 03:37:38.000000 colorcall-0.2.3/colorcall.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 03:37:38.000000 colorcall-0.2.3/colorcall.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-06-03 03:37:38.000000 colorcall-0.2.3/colorcall.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-06-03 03:37:38.767497 colorcall-0.2.3/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      660 2024-06-03 03:37:35.000000 colorcall-0.2.3/setup.py
```

### Comparing `colorcall-0.2.2/PKG-INFO` & `colorcall-0.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: colorcall
-Version: 0.2.2
+Version: 0.2.3
 Summary: Color call your caracal
 Home-page: https://github.com/Sw1mmeR/colorcall/tree/main
 Author: Mikle Sedrakyan
 Author-email: scriptdefender@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 ![Logo](https://mykaleidoscope.ru/x/uploads/posts/2022-09/1663623253_4-mykaleidoscope-ru-p-zloi-karakal-pinterest-4.jpg)
 
 # Colorcall
 
 Color call your caracal!
```

### Comparing `colorcall-0.2.2/README.md` & `colorcall-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `colorcall-0.2.2/colorcall/__init__.py` & `colorcall-0.2.3/colorcall/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .colorizer import Color, FontStyle, _cprint, basic, rgb
 
-__version__ = "0.2.2"
+__version__ = "0.2.3"
 
 
 def black(text: str) -> None:
     _cprint(text, Color.black)
 
 
 def red(text: str) -> None:
```

### Comparing `colorcall-0.2.2/colorcall/colorizer.py` & `colorcall-0.2.3/colorcall/colorizer.py`

 * *Files identical despite different names*

### Comparing `colorcall-0.2.2/colorcall.egg-info/PKG-INFO` & `colorcall-0.2.3/colorcall.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: colorcall
-Version: 0.2.2
+Version: 0.2.3
 Summary: Color call your caracal
 Home-page: https://github.com/Sw1mmeR/colorcall/tree/main
 Author: Mikle Sedrakyan
 Author-email: scriptdefender@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 ![Logo](https://mykaleidoscope.ru/x/uploads/posts/2022-09/1663623253_4-mykaleidoscope-ru-p-zloi-karakal-pinterest-4.jpg)
 
 # Colorcall
 
 Color call your caracal!
```

### Comparing `colorcall-0.2.2/setup.py` & `colorcall-0.2.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 setup(
     name=colorcall.__name__,
     version=colorcall.__version__,
     author="Mikle Sedrakyan",
     author_email="scriptdefender@yandex.ru",
     description="Color call your caracal",
     include_package_data=True,
+    license_files=("LICENSE",),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Sw1mmeR/colorcall/tree/main",
     packages=find_packages(),
     package_data={
         colorcall.__name__: ["py.typed"],
     },
```

