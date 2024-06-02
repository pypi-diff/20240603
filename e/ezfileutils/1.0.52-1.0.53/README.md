# Comparing `tmp/ezfileutils-1.0.52.tar.gz` & `tmp/ezfileutils-1.0.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezfileutils-1.0.52.tar", last modified: Thu Feb 29 19:24:28 2024, max compression
+gzip compressed data, was "ezfileutils-1.0.53.tar", last modified: Sun Jun  2 22:23:16 2024, max compression
```

## Comparing `ezfileutils-1.0.52.tar` & `ezfileutils-1.0.53.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-02-29 19:24:28.008216 ezfileutils-1.0.52/
--rw-rw-rw-   0        0        0     3617 2024-02-29 19:24:28.007216 ezfileutils-1.0.52/PKG-INFO
--rw-rw-rw-   0        0        0     3317 2024-02-29 19:24:21.000000 ezfileutils-1.0.52/README.md
-drwxrwxrwx   0        0        0        0 2024-02-29 19:24:28.002214 ezfileutils-1.0.52/ezfileutils/
--rw-rw-rw-   0        0        0       28 2024-02-29 18:33:29.000000 ezfileutils-1.0.52/ezfileutils/__init__.py
--rw-rw-rw-   0        0        0    22689 2024-02-29 17:56:01.000000 ezfileutils-1.0.52/ezfileutils/ezfileutils.py
-drwxrwxrwx   0        0        0        0 2024-02-29 19:24:28.006214 ezfileutils-1.0.52/ezfileutils.egg-info/
--rw-rw-rw-   0        0        0     3617 2024-02-29 19:24:27.000000 ezfileutils-1.0.52/ezfileutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2024-02-29 19:24:27.000000 ezfileutils-1.0.52/ezfileutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-29 19:24:27.000000 ezfileutils-1.0.52/ezfileutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-02-29 19:24:27.000000 ezfileutils-1.0.52/ezfileutils.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       12 2024-02-29 19:24:27.000000 ezfileutils-1.0.52/ezfileutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-29 19:24:28.008216 ezfileutils-1.0.52/setup.cfg
--rw-rw-rw-   0        0        0      687 2024-02-29 19:22:23.000000 ezfileutils-1.0.52/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 22:23:16.417363 ezfileutils-1.0.53/
+-rw-rw-rw-   0        0        0     3617 2024-06-02 22:23:16.416410 ezfileutils-1.0.53/PKG-INFO
+-rw-rw-rw-   0        0        0     3317 2024-02-29 19:24:21.000000 ezfileutils-1.0.53/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 22:23:16.404422 ezfileutils-1.0.53/ezfileutils/
+-rw-rw-rw-   0        0        0       28 2024-02-29 18:33:29.000000 ezfileutils-1.0.53/ezfileutils/__init__.py
+-rw-rw-rw-   0        0        0    22689 2024-02-29 17:56:01.000000 ezfileutils-1.0.53/ezfileutils/ezfileutils.py
+drwxrwxrwx   0        0        0        0 2024-06-02 22:23:16.414852 ezfileutils-1.0.53/ezfileutils.egg-info/
+-rw-rw-rw-   0        0        0     3617 2024-06-02 22:23:16.000000 ezfileutils-1.0.53/ezfileutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2024-06-02 22:23:16.000000 ezfileutils-1.0.53/ezfileutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 22:23:16.000000 ezfileutils-1.0.53/ezfileutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-06-02 22:23:16.000000 ezfileutils-1.0.53/ezfileutils.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       12 2024-06-02 22:23:16.000000 ezfileutils-1.0.53/ezfileutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 22:23:16.417363 ezfileutils-1.0.53/setup.cfg
+-rw-rw-rw-   0        0        0      687 2024-06-02 22:23:04.000000 ezfileutils-1.0.53/setup.py
```

### Comparing `ezfileutils-1.0.52/PKG-INFO` & `ezfileutils-1.0.53/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezfileutils
-Version: 1.0.52
+Version: 1.0.53
 Summary: A Python utility script for common file operations.
 Author: subbsandwich
 Author-email: tanagitanagiakori@gmail.com
 Description-Content-Type: text/markdown
 
 
 # ezfileutils
```

### Comparing `ezfileutils-1.0.52/README.md` & `ezfileutils-1.0.53/README.md`

 * *Files identical despite different names*

### Comparing `ezfileutils-1.0.52/ezfileutils/ezfileutils.py` & `ezfileutils-1.0.53/ezfileutils/ezfileutils.py`

 * *Files identical despite different names*

### Comparing `ezfileutils-1.0.52/ezfileutils.egg-info/PKG-INFO` & `ezfileutils-1.0.53/ezfileutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezfileutils
-Version: 1.0.52
+Version: 1.0.53
 Summary: A Python utility script for common file operations.
 Author: subbsandwich
 Author-email: tanagitanagiakori@gmail.com
 Description-Content-Type: text/markdown
 
 
 # ezfileutils
```

### Comparing `ezfileutils-1.0.52/setup.py` & `ezfileutils-1.0.53/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='ezfileutils',
-    version='1.0.52',
+    version='1.0.53',
     description='A Python utility script for common file operations.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='subbsandwich',
     author_email='tanagitanagiakori@gmail.com',
     packages=find_packages(),
     install_requires=[],
```

