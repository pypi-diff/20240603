# Comparing `tmp/imsciences-0.5.8.4.tar.gz` & `tmp/imsciences-0.5.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imsciences-0.5.8.4.tar", last modified: Thu May 23 11:52:55 2024, max compression
+gzip compressed data, was "imsciences-0.5.8.5.tar", last modified: Mon Jun  3 14:40:01 2024, max compression
```

## Comparing `imsciences-0.5.8.4.tar` & `imsciences-0.5.8.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 11:52:55.351038 imsciences-0.5.8.4/
--rw-rw-rw-   0        0        0     9976 2024-05-23 11:52:55.346582 imsciences-0.5.8.4/PKG-INFO
--rw-rw-rw-   0        0        0     9471 2024-05-17 09:27:28.000000 imsciences-0.5.8.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 11:52:55.318144 imsciences-0.5.8.4/imsciences/
--rw-rw-rw-   0        0        0       78 2024-05-20 13:24:02.000000 imsciences-0.5.8.4/imsciences/__init__.py
--rw-rw-rw-   0        0        0   103132 2024-05-23 11:51:45.000000 imsciences-0.5.8.4/imsciences/datafunctions.py
-drwxrwxrwx   0        0        0        0 2024-05-23 11:52:55.343069 imsciences-0.5.8.4/imsciences.egg-info/
--rw-rw-rw-   0        0        0     9976 2024-05-23 11:52:55.000000 imsciences-0.5.8.4/imsciences.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-05-23 11:52:55.000000 imsciences-0.5.8.4/imsciences.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 11:52:55.000000 imsciences-0.5.8.4/imsciences.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-23 11:52:55.000000 imsciences-0.5.8.4/imsciences.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-23 11:52:55.000000 imsciences-0.5.8.4/imsciences.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 11:52:55.351038 imsciences-0.5.8.4/setup.cfg
--rw-rw-rw-   0        0        0     1093 2024-05-23 11:52:15.000000 imsciences-0.5.8.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 14:40:01.679443 imsciences-0.5.8.5/
+-rw-rw-rw-   0        0        0     9999 2024-06-03 14:40:01.665419 imsciences-0.5.8.5/PKG-INFO
+-rw-rw-rw-   0        0        0     9471 2024-05-17 09:27:28.000000 imsciences-0.5.8.5/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 14:40:01.599522 imsciences-0.5.8.5/imsciences/
+-rw-rw-rw-   0        0        0       78 2024-05-20 13:24:02.000000 imsciences-0.5.8.5/imsciences/__init__.py
+-rw-rw-rw-   0        0        0   103132 2024-05-23 11:51:45.000000 imsciences-0.5.8.5/imsciences/datafunctions.py
+drwxrwxrwx   0        0        0        0 2024-06-03 14:40:01.665419 imsciences-0.5.8.5/imsciences.egg-info/
+-rw-rw-rw-   0        0        0     9999 2024-06-03 14:40:01.000000 imsciences-0.5.8.5/imsciences.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-06-03 14:40:01.000000 imsciences-0.5.8.5/imsciences.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 14:40:01.000000 imsciences-0.5.8.5/imsciences.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-06-03 14:40:01.000000 imsciences-0.5.8.5/imsciences.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-06-03 14:40:01.000000 imsciences-0.5.8.5/imsciences.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 14:40:01.679443 imsciences-0.5.8.5/setup.cfg
+-rw-rw-rw-   0        0        0     1093 2024-06-03 14:39:36.000000 imsciences-0.5.8.5/setup.py
```

### Comparing `imsciences-0.5.8.4/PKG-INFO` & `imsciences-0.5.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.8.4
+Version: 0.5.8.5
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
+Requires-Dist: pandas
 
 # IMS Package Documentation
 
 The IMS package is a python library for processing incoming data into a format that can be used for projects. IMS processing offers a variety of functions to manipulate and analyze data efficiently. Here are the functionalities provided by the package:
 
 ### 1. `get_wd_levels(levels)`
 - **Description**: Get the working directory with the option of moving up parents.
```

### Comparing `imsciences-0.5.8.4/README.md` & `imsciences-0.5.8.5/README.md`

 * *Files identical despite different names*

### Comparing `imsciences-0.5.8.4/imsciences/datafunctions.py` & `imsciences-0.5.8.5/imsciences/datafunctions.py`

 * *Files identical despite different names*

### Comparing `imsciences-0.5.8.4/imsciences.egg-info/PKG-INFO` & `imsciences-0.5.8.5/imsciences.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.8.4
+Version: 0.5.8.5
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
+Requires-Dist: pandas
 
 # IMS Package Documentation
 
 The IMS package is a python library for processing incoming data into a format that can be used for projects. IMS processing offers a variety of functions to manipulate and analyze data efficiently. Here are the functionalities provided by the package:
 
 ### 1. `get_wd_levels(levels)`
 - **Description**: Get the working directory with the option of moving up parents.
```

### Comparing `imsciences-0.5.8.4/setup.py` & `imsciences-0.5.8.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Function to read the contents of the README file
 def read_md(file_name):
     if os.path.isfile(file_name):
         with open(file_name, 'r', encoding='utf-8') as f:
             return f.read()
     return ''
 
-VERSION = '0.5.8.4'
+VERSION = '0.5.8.5'
 DESCRIPTION = 'IMS Data Processing Package'
 LONG_DESCRIPTION = read_md('README.md')  # Reading from README.md
 
 # Setting up
 setup(
     name="imsciences",
     version=VERSION,
```

