# Comparing `tmp/abstract_municipalities-0.0.0.1.tar.gz` & `tmp/abstract_municipalities-0.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_municipalities-0.0.0.1.tar", last modified: Mon Jun  3 01:05:43 2024, max compression
+gzip compressed data, was "abstract_municipalities-0.0.0.2.tar", last modified: Mon Jun  3 01:21:22 2024, max compression
```

## Comparing `abstract_municipalities-0.0.0.1.tar` & `abstract_municipalities-0.0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-06-03 01:05:43.103829 abstract_municipalities-0.0.0.1/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      481 2024-06-03 01:05:43.103829 abstract_municipalities-0.0.0.1/PKG-INFO
--rw-rw-rw-   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_municipalities-0.0.0.1/README.md
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-06-03 01:05:43.103829 abstract_municipalities-0.0.0.1/setup.cfg
--rw-rw-rw-   0 gamook    (1000) gamook    (1000)      914 2024-06-03 00:28:34.000000 abstract_municipalities-0.0.0.1/setup.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-06-03 01:05:43.099829 abstract_municipalities-0.0.0.1/src/
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-06-03 01:05:43.103829 abstract_municipalities-0.0.0.1/src/abstractMunicipalities/
--rw-rw-rw-   0 gamook    (1000) gamook    (1000)       52 2024-06-03 00:26:55.000000 abstract_municipalities-0.0.0.1/src/abstractMunicipalities/__init__.py
--rw-rw-rw-   0 gamook    (1000) gamook    (1000)    25872 2024-06-03 00:16:35.000000 abstract_municipalities-0.0.0.1/src/abstractMunicipalities/cities.py
--rw-rw-rw-   0 gamook    (1000) gamook    (1000)     2776 2024-06-03 00:25:59.000000 abstract_municipalities-0.0.0.1/src/abstractMunicipalities/states.py
--rw-rw-rw-   0 gamook    (1000) gamook    (1000)  2246571 2024-06-03 00:47:22.000000 abstract_municipalities-0.0.0.1/src/abstractMunicipalities/zipCodes.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-06-03 01:05:43.103829 abstract_municipalities-0.0.0.1/src/abstract_municipalities.egg-info/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      481 2024-06-03 01:05:43.000000 abstract_municipalities-0.0.0.1/src/abstract_municipalities.egg-info/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      374 2024-06-03 01:05:43.000000 abstract_municipalities-0.0.0.1/src/abstract_municipalities.egg-info/SOURCES.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-06-03 01:05:43.000000 abstract_municipalities-0.0.0.1/src/abstract_municipalities.egg-info/dependency_links.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       23 2024-06-03 01:05:43.000000 abstract_municipalities-0.0.0.1/src/abstract_municipalities.egg-info/top_level.txt
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-06-03 01:21:22.194965 abstract_municipalities-0.0.0.2/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      481 2024-06-03 01:21:22.194965 abstract_municipalities-0.0.0.2/PKG-INFO
+-rw-rw-rw-   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_municipalities-0.0.0.2/README.md
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-06-03 01:21:22.194965 abstract_municipalities-0.0.0.2/setup.cfg
+-rw-rw-rw-   0 gamook    (1000) gamook    (1000)      914 2024-06-03 01:07:10.000000 abstract_municipalities-0.0.0.2/setup.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-06-03 01:21:22.190965 abstract_municipalities-0.0.0.2/src/
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-06-03 01:21:22.194965 abstract_municipalities-0.0.0.2/src/abstractMunicipalities/
+-rw-rw-rw-   0 gamook    (1000) gamook    (1000)       82 2024-06-03 01:06:45.000000 abstract_municipalities-0.0.0.2/src/abstractMunicipalities/__init__.py
+-rw-rw-rw-   0 gamook    (1000) gamook    (1000)    25872 2024-06-03 00:16:35.000000 abstract_municipalities-0.0.0.2/src/abstractMunicipalities/cities.py
+-rw-rw-rw-   0 gamook    (1000) gamook    (1000)     2776 2024-06-03 00:25:59.000000 abstract_municipalities-0.0.0.2/src/abstractMunicipalities/states.py
+-rw-rw-rw-   0 gamook    (1000) gamook    (1000)  2246571 2024-06-03 00:47:22.000000 abstract_municipalities-0.0.0.2/src/abstractMunicipalities/zipCodes.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-06-03 01:21:22.194965 abstract_municipalities-0.0.0.2/src/abstract_municipalities.egg-info/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      481 2024-06-03 01:21:22.000000 abstract_municipalities-0.0.0.2/src/abstract_municipalities.egg-info/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      374 2024-06-03 01:21:22.000000 abstract_municipalities-0.0.0.2/src/abstract_municipalities.egg-info/SOURCES.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-06-03 01:21:22.000000 abstract_municipalities-0.0.0.2/src/abstract_municipalities.egg-info/dependency_links.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       23 2024-06-03 01:21:22.000000 abstract_municipalities-0.0.0.2/src/abstract_municipalities.egg-info/top_level.txt
```

### Comparing `abstract_municipalities-0.0.0.1/setup.py` & `abstract_municipalities-0.0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_municipalities',
-    version='0.0.0.1',
+    version='0.0.0.2',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description="",
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
           'Development Status :: 3 - Alpha',
```

### Comparing `abstract_municipalities-0.0.0.1/src/abstractMunicipalities/cities.py` & `abstract_municipalities-0.0.0.2/src/abstractMunicipalities/cities.py`

 * *Files identical despite different names*

### Comparing `abstract_municipalities-0.0.0.1/src/abstractMunicipalities/states.py` & `abstract_municipalities-0.0.0.2/src/abstractMunicipalities/states.py`

 * *Files identical despite different names*

### Comparing `abstract_municipalities-0.0.0.1/src/abstractMunicipalities/zipCodes.py` & `abstract_municipalities-0.0.0.2/src/abstractMunicipalities/zipCodes.py`

 * *Files identical despite different names*

