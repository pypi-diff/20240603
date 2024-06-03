# Comparing `tmp/square_logger-1.0.5.tar.gz` & `tmp/square_logger-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "square_logger-1.0.5.tar", last modified: Sun Mar 10 09:43:25 2024, max compression
+gzip compressed data, was "square_logger-1.0.6.tar", last modified: Mon Jun  3 14:57:13 2024, max compression
```

## Comparing `square_logger-1.0.5.tar` & `square_logger-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 09:43:25.458617 square_logger-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-10 09:43:25.458617 square_logger-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-10 09:43:16.000000 square_logger-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-10 09:43:25.458617 square_logger-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-10 09:43:16.000000 square_logger-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 09:43:25.454617 square_logger-1.0.5/square_logger/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-10 09:43:16.000000 square_logger-1.0.5/square_logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-03-10 09:43:16.000000 square_logger-1.0.5/square_logger/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 09:43:25.458617 square_logger-1.0.5/square_logger/data/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-10 09:43:16.000000 square_logger-1.0.5/square_logger/data/config.ini
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-03-10 09:43:16.000000 square_logger-1.0.5/square_logger/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 09:43:25.454617 square_logger-1.0.5/square_logger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-10 09:43:25.000000 square_logger-1.0.5/square_logger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-10 09:43:25.000000 square_logger-1.0.5/square_logger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-10 09:43:25.000000 square_logger-1.0.5/square_logger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-10 09:43:25.000000 square_logger-1.0.5/square_logger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-10 09:43:25.000000 square_logger-1.0.5/square_logger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:57:13.635748 square_logger-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-06-03 14:57:13.635748 square_logger-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-06-03 14:57:01.000000 square_logger-1.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 14:57:13.635748 square_logger-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-06-03 14:57:01.000000 square_logger-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:57:13.631748 square_logger-1.0.6/square_logger/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-06-03 14:57:01.000000 square_logger-1.0.6/square_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-06-03 14:57:01.000000 square_logger-1.0.6/square_logger/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:57:13.635748 square_logger-1.0.6/square_logger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-06-03 14:57:13.000000 square_logger-1.0.6/square_logger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-06-03 14:57:13.000000 square_logger-1.0.6/square_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 14:57:13.000000 square_logger-1.0.6/square_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-03 14:57:13.000000 square_logger-1.0.6/square_logger.egg-info/top_level.txt
```

### Comparing `square_logger-1.0.5/PKG-INFO` & `square_logger-1.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: square_logger
-Version: 1.0.5
+Version: 1.0.6
 Summary: python logger for my personal use.
 Home-page: https://github.com/thepmsquare/square_logger
 Author: thePmSquare, Amish Palkar
 Author-email: thepmsquare@gmail.com, amishpalkar302001@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `square_logger-1.0.5/setup.py` & `square_logger-1.0.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name="square_logger",
-    version="1.0.5",
+    version="1.0.6",
     packages=find_packages(),
-    package_data={
-        "square_logger": ["data/*"],
-    },
-    install_requires=["lapa_commons>=0.0.1"],
+    install_requires=[],
     author="thePmSquare, Amish Palkar",
     author_email="thepmsquare@gmail.com, amishpalkar302001@gmail.com",
     description="python logger for my personal use.",
     url="https://github.com/thepmsquare/square_logger",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
```

### Comparing `square_logger-1.0.5/square_logger.egg-info/PKG-INFO` & `square_logger-1.0.6/square_logger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: square-logger
-Version: 1.0.5
+Version: 1.0.6
 Summary: python logger for my personal use.
 Home-page: https://github.com/thepmsquare/square_logger
 Author: thePmSquare, Amish Palkar
 Author-email: thepmsquare@gmail.com, amishpalkar302001@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

