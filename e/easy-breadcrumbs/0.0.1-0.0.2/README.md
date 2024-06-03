# Comparing `tmp/easy_breadcrumbs-0.0.1.tar.gz` & `tmp/easy_breadcrumbs-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_breadcrumbs-0.0.1.tar", last modified: Mon Jun  3 05:29:48 2024, max compression
+gzip compressed data, was "easy_breadcrumbs-0.0.2.tar", last modified: Mon Jun  3 05:39:12 2024, max compression
```

## Comparing `easy_breadcrumbs-0.0.1.tar` & `easy_breadcrumbs-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,28 @@
-drwxr-xr-x   0 primestr  (1000) primestr  (1000)        0 2024-06-03 05:29:48.455040 easy_breadcrumbs-0.0.1/
--rw-r--r--   0 primestr  (1000) primestr  (1000)     1069 2024-06-03 04:58:49.000000 easy_breadcrumbs-0.0.1/LICENSE
--rw-r--r--   0 primestr  (1000) primestr  (1000)      971 2024-06-03 05:29:48.451707 easy_breadcrumbs-0.0.1/PKG-INFO
--rw-r--r--   0 primestr  (1000) primestr  (1000)       37 2024-06-03 04:56:09.000000 easy_breadcrumbs-0.0.1/README.md
-drwxr-xr-x   0 primestr  (1000) primestr  (1000)        0 2024-06-03 05:29:48.448373 easy_breadcrumbs-0.0.1/breadcrumbs/
--rw-r--r--   0 primestr  (1000) primestr  (1000)        0 2024-06-03 04:39:37.000000 easy_breadcrumbs-0.0.1/breadcrumbs/__init__.py
--rw-r--r--   0 primestr  (1000) primestr  (1000)      187 2024-06-03 04:43:14.000000 easy_breadcrumbs-0.0.1/breadcrumbs/apps.py
--rw-r--r--   0 primestr  (1000) primestr  (1000)      263 2024-06-03 04:44:21.000000 easy_breadcrumbs-0.0.1/breadcrumbs/context_processors.py
--rw-r--r--   0 primestr  (1000) primestr  (1000)      445 2024-06-03 04:44:21.000000 easy_breadcrumbs-0.0.1/breadcrumbs/mixins.py
--rw-r--r--   0 primestr  (1000) primestr  (1000)     1712 2024-06-03 04:54:23.000000 easy_breadcrumbs-0.0.1/breadcrumbs/service.py
-drwxr-xr-x   0 primestr  (1000) primestr  (1000)        0 2024-06-03 05:29:48.448373 easy_breadcrumbs-0.0.1/breadcrumbs/templatetags/
--rw-r--r--   0 primestr  (1000) primestr  (1000)        0 2024-06-03 04:40:32.000000 easy_breadcrumbs-0.0.1/breadcrumbs/templatetags/__init__.py
--rw-r--r--   0 primestr  (1000) primestr  (1000)      249 2024-06-03 05:28:20.000000 easy_breadcrumbs-0.0.1/breadcrumbs/templatetags/breadcrumbs.py
-drwxr-xr-x   0 primestr  (1000) primestr  (1000)        0 2024-06-03 05:29:48.448373 easy_breadcrumbs-0.0.1/breadcrumbs/tests/
--rw-r--r--   0 primestr  (1000) primestr  (1000)        0 2024-06-03 04:41:55.000000 easy_breadcrumbs-0.0.1/breadcrumbs/tests/__init__.py
--rw-r--r--   0 primestr  (1000) primestr  (1000)      256 2024-06-03 04:50:59.000000 easy_breadcrumbs-0.0.1/breadcrumbs/utils.py
-drwxr-xr-x   0 primestr  (1000) primestr  (1000)        0 2024-06-03 05:29:48.451707 easy_breadcrumbs-0.0.1/easy_breadcrumbs.egg-info/
--rw-r--r--   0 primestr  (1000) primestr  (1000)      971 2024-06-03 05:29:48.000000 easy_breadcrumbs-0.0.1/easy_breadcrumbs.egg-info/PKG-INFO
--rw-r--r--   0 primestr  (1000) primestr  (1000)      476 2024-06-03 05:29:48.000000 easy_breadcrumbs-0.0.1/easy_breadcrumbs.egg-info/SOURCES.txt
--rw-r--r--   0 primestr  (1000) primestr  (1000)        1 2024-06-03 05:29:48.000000 easy_breadcrumbs-0.0.1/easy_breadcrumbs.egg-info/dependency_links.txt
--rw-r--r--   0 primestr  (1000) primestr  (1000)       12 2024-06-03 05:29:48.000000 easy_breadcrumbs-0.0.1/easy_breadcrumbs.egg-info/requires.txt
--rw-r--r--   0 primestr  (1000) primestr  (1000)       12 2024-06-03 05:29:48.000000 easy_breadcrumbs-0.0.1/easy_breadcrumbs.egg-info/top_level.txt
--rw-r--r--   0 primestr  (1000) primestr  (1000)       38 2024-06-03 05:29:48.455040 easy_breadcrumbs-0.0.1/setup.cfg
--rw-r--r--   0 primestr  (1000) primestr  (1000)     1189 2024-06-03 05:29:41.000000 easy_breadcrumbs-0.0.1/setup.py
+drwxr-xr-x   0 primestr  (1000) primestr  (1000)        0 2024-06-03 05:39:12.112512 easy_breadcrumbs-0.0.2/
+-rw-r--r--   0 primestr  (1000) primestr  (1000)     1069 2024-06-03 04:58:49.000000 easy_breadcrumbs-0.0.2/LICENSE
+-rw-r--r--   0 primestr  (1000) primestr  (1000)       42 2024-06-03 05:37:54.000000 easy_breadcrumbs-0.0.2/MANIFEST.in
+-rw-r--r--   0 primestr  (1000) primestr  (1000)      971 2024-06-03 05:39:12.112512 easy_breadcrumbs-0.0.2/PKG-INFO
+-rw-r--r--   0 primestr  (1000) primestr  (1000)       37 2024-06-03 04:56:09.000000 easy_breadcrumbs-0.0.2/README.md
+drwxr-xr-x   0 primestr  (1000) primestr  (1000)        0 2024-06-03 05:39:12.112512 easy_breadcrumbs-0.0.2/breadcrumbs/
+-rw-r--r--   0 primestr  (1000) primestr  (1000)        0 2024-06-03 04:39:37.000000 easy_breadcrumbs-0.0.2/breadcrumbs/__init__.py
+-rw-r--r--   0 primestr  (1000) primestr  (1000)      187 2024-06-03 04:43:14.000000 easy_breadcrumbs-0.0.2/breadcrumbs/apps.py
+-rw-r--r--   0 primestr  (1000) primestr  (1000)      263 2024-06-03 04:44:21.000000 easy_breadcrumbs-0.0.2/breadcrumbs/context_processors.py
+-rw-r--r--   0 primestr  (1000) primestr  (1000)      445 2024-06-03 04:44:21.000000 easy_breadcrumbs-0.0.2/breadcrumbs/mixins.py
+-rw-r--r--   0 primestr  (1000) primestr  (1000)     1712 2024-06-03 04:54:23.000000 easy_breadcrumbs-0.0.2/breadcrumbs/service.py
+drwxr-xr-x   0 primestr  (1000) primestr  (1000)        0 2024-06-03 05:39:12.109179 easy_breadcrumbs-0.0.2/breadcrumbs/templates/
+drwxr-xr-x   0 primestr  (1000) primestr  (1000)        0 2024-06-03 05:39:12.112512 easy_breadcrumbs-0.0.2/breadcrumbs/templates/breadcrumbs/
+-rw-r--r--   0 primestr  (1000) primestr  (1000)      375 2024-06-03 04:52:35.000000 easy_breadcrumbs-0.0.2/breadcrumbs/templates/breadcrumbs/breadcrumbs.html
+drwxr-xr-x   0 primestr  (1000) primestr  (1000)        0 2024-06-03 05:39:12.112512 easy_breadcrumbs-0.0.2/breadcrumbs/templatetags/
+-rw-r--r--   0 primestr  (1000) primestr  (1000)        0 2024-06-03 04:40:32.000000 easy_breadcrumbs-0.0.2/breadcrumbs/templatetags/__init__.py
+-rw-r--r--   0 primestr  (1000) primestr  (1000)      227 2024-06-03 05:34:26.000000 easy_breadcrumbs-0.0.2/breadcrumbs/templatetags/breadcrumbs.py
+drwxr-xr-x   0 primestr  (1000) primestr  (1000)        0 2024-06-03 05:39:12.112512 easy_breadcrumbs-0.0.2/breadcrumbs/tests/
+-rw-r--r--   0 primestr  (1000) primestr  (1000)        0 2024-06-03 04:41:55.000000 easy_breadcrumbs-0.0.2/breadcrumbs/tests/__init__.py
+-rw-r--r--   0 primestr  (1000) primestr  (1000)      256 2024-06-03 04:50:59.000000 easy_breadcrumbs-0.0.2/breadcrumbs/utils.py
+drwxr-xr-x   0 primestr  (1000) primestr  (1000)        0 2024-06-03 05:39:12.112512 easy_breadcrumbs-0.0.2/easy_breadcrumbs.egg-info/
+-rw-r--r--   0 primestr  (1000) primestr  (1000)      971 2024-06-03 05:39:12.000000 easy_breadcrumbs-0.0.2/easy_breadcrumbs.egg-info/PKG-INFO
+-rw-r--r--   0 primestr  (1000) primestr  (1000)      539 2024-06-03 05:39:12.000000 easy_breadcrumbs-0.0.2/easy_breadcrumbs.egg-info/SOURCES.txt
+-rw-r--r--   0 primestr  (1000) primestr  (1000)        1 2024-06-03 05:39:12.000000 easy_breadcrumbs-0.0.2/easy_breadcrumbs.egg-info/dependency_links.txt
+-rw-r--r--   0 primestr  (1000) primestr  (1000)       12 2024-06-03 05:39:12.000000 easy_breadcrumbs-0.0.2/easy_breadcrumbs.egg-info/requires.txt
+-rw-r--r--   0 primestr  (1000) primestr  (1000)       12 2024-06-03 05:39:12.000000 easy_breadcrumbs-0.0.2/easy_breadcrumbs.egg-info/top_level.txt
+-rw-r--r--   0 primestr  (1000) primestr  (1000)       38 2024-06-03 05:39:12.112512 easy_breadcrumbs-0.0.2/setup.cfg
+-rw-r--r--   0 primestr  (1000) primestr  (1000)     1189 2024-06-03 05:39:08.000000 easy_breadcrumbs-0.0.2/setup.py
```

### Comparing `easy_breadcrumbs-0.0.1/LICENSE` & `easy_breadcrumbs-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_breadcrumbs-0.0.1/PKG-INFO` & `easy_breadcrumbs-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-breadcrumbs
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Django app to add breadcrumbs to your project.
 Home-page: https://github.com/PrimeStr/easy-breadcrumbs
 Author: Maxim Golovin
 Author-email: boss@primestr.ru
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `easy_breadcrumbs-0.0.1/breadcrumbs/service.py` & `easy_breadcrumbs-0.0.2/breadcrumbs/service.py`

 * *Files identical despite different names*

### Comparing `easy_breadcrumbs-0.0.1/easy_breadcrumbs.egg-info/PKG-INFO` & `easy_breadcrumbs-0.0.2/easy_breadcrumbs.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-breadcrumbs
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Django app to add breadcrumbs to your project.
 Home-page: https://github.com/PrimeStr/easy-breadcrumbs
 Author: Maxim Golovin
 Author-email: boss@primestr.ru
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `easy_breadcrumbs-0.0.1/setup.py` & `easy_breadcrumbs-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='easy-breadcrumbs',
-    version='0.0.1',
+    version='0.0.2',
     packages=find_packages(),
     include_package_data=True,
     license='MIT License',
     description='A Django app to add breadcrumbs to your project.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/PrimeStr/easy-breadcrumbs',
```

