# Comparing `tmp/treeplusrepository-0.1.tar.gz` & `tmp/treeplusrepository-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "treeplusrepository-0.1.tar", last modified: Mon Jun  3 11:34:32 2024, max compression
+gzip compressed data, was "treeplusrepository-0.1.1.tar", last modified: Mon Jun  3 11:43:59 2024, max compression
```

## Comparing `treeplusrepository-0.1.tar` & `treeplusrepository-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-06-03 11:34:32.756000 treeplusrepository-0.1/
--rw-rw-rw-   0        0        0     1027 2024-06-03 11:34:32.736000 treeplusrepository-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-06-03 11:34:32.616000 treeplusrepository-0.1/TREEplusrepository/
--rw-rw-rw-   0        0        0   170607 2024-06-03 10:03:28.000000 treeplusrepository-0.1/TREEplusrepository/TREEplus.py
--rw-rw-rw-   0        0        0       33 2024-06-03 11:09:45.000000 treeplusrepository-0.1/TREEplusrepository/__init__.py
--rw-rw-rw-   0        0        0     1388 2024-06-03 11:34:25.000000 treeplusrepository-0.1/TREEplusrepository/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-03 11:34:32.721000 treeplusrepository-0.1/TREEplusrepository.egg-info/
--rw-rw-rw-   0        0        0     1027 2024-06-03 11:34:32.000000 treeplusrepository-0.1/TREEplusrepository.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2024-06-03 11:34:32.000000 treeplusrepository-0.1/TREEplusrepository.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 11:34:32.000000 treeplusrepository-0.1/TREEplusrepository.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-06-03 11:34:32.000000 treeplusrepository-0.1/TREEplusrepository.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-03 11:34:32.754000 treeplusrepository-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1388 2024-06-03 11:34:28.000000 treeplusrepository-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 11:43:59.980000 treeplusrepository-0.1.1/
+-rw-rw-rw-   0        0        0     1029 2024-06-03 11:43:59.911000 treeplusrepository-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-03 11:43:59.434000 treeplusrepository-0.1.1/TREEplusrepository/
+-rw-rw-rw-   0        0        0   170607 2024-06-03 10:03:28.000000 treeplusrepository-0.1.1/TREEplusrepository/TREEplus.py
+-rw-rw-rw-   0        0        0       42 2024-06-03 11:42:10.000000 treeplusrepository-0.1.1/TREEplusrepository/__init__.py
+-rw-rw-rw-   0        0        0     1390 2024-06-03 11:43:49.000000 treeplusrepository-0.1.1/TREEplusrepository/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 11:43:59.862000 treeplusrepository-0.1.1/TREEplusrepository.egg-info/
+-rw-rw-rw-   0        0        0     1029 2024-06-03 11:43:58.000000 treeplusrepository-0.1.1/TREEplusrepository.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2024-06-03 11:43:58.000000 treeplusrepository-0.1.1/TREEplusrepository.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 11:43:58.000000 treeplusrepository-0.1.1/TREEplusrepository.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-06-03 11:43:58.000000 treeplusrepository-0.1.1/TREEplusrepository.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 11:43:59.970000 treeplusrepository-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1390 2024-06-03 11:43:44.000000 treeplusrepository-0.1.1/setup.py
```

### Comparing `treeplusrepository-0.1/PKG-INFO` & `treeplusrepository-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TREEplusrepository
-Version: 0.1
+Version: 0.1.1
 Summary: Standard and Non-Standard Tree Based Methods
 Author: Daniel Fynn
 Author-email: <df390@uowmail.edu.au>
 Keywords: python,tree,CART
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `treeplusrepository-0.1/TREEplusrepository/TREEplus.py` & `treeplusrepository-0.1.1/TREEplusrepository/TREEplus.py`

 * *Files identical despite different names*

### Comparing `treeplusrepository-0.1/TREEplusrepository/setup.py` & `treeplusrepository-0.1.1/TREEplusrepository/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1' 
+VERSION = '0.1.1' 
 DESCRIPTION = 'Standard and Non-Standard Tree Based Methods'
 LONG_DESCRIPTION = 'The library contains standard CART based methologies for growing trees, includind twoing, as well as non standard techniques two-stage techniques like fast and latent-budget tree. There is also cross validation methods for pruning the tree, and k-folds implementation. As well as a graphical interface to view the tree and information about the nodes, including visual pruning by viewing thhe decrease in deviance created by a split relative to other splits in the grown tree, and an output table containing useful information.'
 
 # Setting up
 setup(
         name="TREEplusrepository", 
         version=VERSION,
```

### Comparing `treeplusrepository-0.1/TREEplusrepository.egg-info/PKG-INFO` & `treeplusrepository-0.1.1/TREEplusrepository.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TREEplusrepository
-Version: 0.1
+Version: 0.1.1
 Summary: Standard and Non-Standard Tree Based Methods
 Author: Daniel Fynn
 Author-email: <df390@uowmail.edu.au>
 Keywords: python,tree,CART
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `treeplusrepository-0.1/setup.py` & `treeplusrepository-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1' 
+VERSION = '0.1.1' 
 DESCRIPTION = 'Standard and Non-Standard Tree Based Methods'
 LONG_DESCRIPTION = 'The library contains standard CART based methologies for growing trees, includind twoing, as well as non standard techniques two-stage techniques like fast and latent-budget tree. There is also cross validation methods for pruning the tree, and k-folds implementation. As well as a graphical interface to view the tree and information about the nodes, including visual pruning by viewing thhe decrease in deviance created by a split relative to other splits in the grown tree, and an output table containing useful information.'
 
 # Setting up
 setup(
         name="TREEplusrepository", 
         version=VERSION,
```

