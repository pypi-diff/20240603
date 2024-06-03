# Comparing `tmp/treeplusrepository-0.1.2.tar.gz` & `tmp/treeplusrepository-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "treeplusrepository-0.1.2.tar", last modified: Mon Jun  3 12:03:03 2024, max compression
+gzip compressed data, was "treeplusrepository-0.1.3.tar", last modified: Mon Jun  3 12:17:06 2024, max compression
```

## Comparing `treeplusrepository-0.1.2.tar` & `treeplusrepository-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-06-03 12:03:03.932000 treeplusrepository-0.1.2/
--rw-rw-rw-   0        0        0     1029 2024-06-03 12:03:03.837000 treeplusrepository-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-06-03 12:03:03.441000 treeplusrepository-0.1.2/TREEplusrepository/
--rw-rw-rw-   0        0        0   170613 2024-06-03 12:01:14.000000 treeplusrepository-0.1.2/TREEplusrepository/TREEplus.py
--rw-rw-rw-   0        0        0       42 2024-06-03 11:42:10.000000 treeplusrepository-0.1.2/TREEplusrepository/__init__.py
--rw-rw-rw-   0        0        0     1390 2024-06-03 12:02:49.000000 treeplusrepository-0.1.2/TREEplusrepository/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-03 12:03:03.794000 treeplusrepository-0.1.2/TREEplusrepository.egg-info/
--rw-rw-rw-   0        0        0     1029 2024-06-03 12:03:02.000000 treeplusrepository-0.1.2/TREEplusrepository.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2024-06-03 12:03:02.000000 treeplusrepository-0.1.2/TREEplusrepository.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 12:03:02.000000 treeplusrepository-0.1.2/TREEplusrepository.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-06-03 12:03:02.000000 treeplusrepository-0.1.2/TREEplusrepository.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-03 12:03:03.923000 treeplusrepository-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1390 2024-06-03 12:02:45.000000 treeplusrepository-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 12:17:06.488000 treeplusrepository-0.1.3/
+-rw-rw-rw-   0        0        0     1029 2024-06-03 12:17:06.427000 treeplusrepository-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-03 12:17:05.991000 treeplusrepository-0.1.3/TREEplusrepository/
+-rw-rw-rw-   0        0        0   170613 2024-06-03 12:01:14.000000 treeplusrepository-0.1.3/TREEplusrepository/TREEplus.py
+-rw-rw-rw-   0        0        0       35 2024-06-03 12:16:46.000000 treeplusrepository-0.1.3/TREEplusrepository/__init__.py
+-rw-rw-rw-   0        0        0     1390 2024-06-03 12:16:21.000000 treeplusrepository-0.1.3/TREEplusrepository/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 12:17:06.385000 treeplusrepository-0.1.3/TREEplusrepository.egg-info/
+-rw-rw-rw-   0        0        0     1029 2024-06-03 12:17:05.000000 treeplusrepository-0.1.3/TREEplusrepository.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2024-06-03 12:17:05.000000 treeplusrepository-0.1.3/TREEplusrepository.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 12:17:05.000000 treeplusrepository-0.1.3/TREEplusrepository.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-06-03 12:17:05.000000 treeplusrepository-0.1.3/TREEplusrepository.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 12:17:06.483000 treeplusrepository-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1390 2024-06-03 12:16:26.000000 treeplusrepository-0.1.3/setup.py
```

### Comparing `treeplusrepository-0.1.2/PKG-INFO` & `treeplusrepository-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TREEplusrepository
-Version: 0.1.2
+Version: 0.1.3
 Summary: Standard and Non-Standard Tree Based Methods
 Author: Daniel Fynn
 Author-email: <df390@uowmail.edu.au>
 Keywords: python,tree,CART
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `treeplusrepository-0.1.2/TREEplusrepository/TREEplus.py` & `treeplusrepository-0.1.3/TREEplusrepository/TREEplus.py`

 * *Files identical despite different names*

### Comparing `treeplusrepository-0.1.2/TREEplusrepository/setup.py` & `treeplusrepository-0.1.3/TREEplusrepository/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.2' 
+VERSION = '0.1.3' 
 DESCRIPTION = 'Standard and Non-Standard Tree Based Methods'
 LONG_DESCRIPTION = 'The library contains standard CART based methologies for growing trees, includind twoing, as well as non standard techniques two-stage techniques like fast and latent-budget tree. There is also cross validation methods for pruning the tree, and k-folds implementation. As well as a graphical interface to view the tree and information about the nodes, including visual pruning by viewing thhe decrease in deviance created by a split relative to other splits in the grown tree, and an output table containing useful information.'
 
 # Setting up
 setup(
         name="TREEplusrepository", 
         version=VERSION,
```

### Comparing `treeplusrepository-0.1.2/TREEplusrepository.egg-info/PKG-INFO` & `treeplusrepository-0.1.3/TREEplusrepository.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TREEplusrepository
-Version: 0.1.2
+Version: 0.1.3
 Summary: Standard and Non-Standard Tree Based Methods
 Author: Daniel Fynn
 Author-email: <df390@uowmail.edu.au>
 Keywords: python,tree,CART
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `treeplusrepository-0.1.2/setup.py` & `treeplusrepository-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.2' 
+VERSION = '0.1.3' 
 DESCRIPTION = 'Standard and Non-Standard Tree Based Methods'
 LONG_DESCRIPTION = 'The library contains standard CART based methologies for growing trees, includind twoing, as well as non standard techniques two-stage techniques like fast and latent-budget tree. There is also cross validation methods for pruning the tree, and k-folds implementation. As well as a graphical interface to view the tree and information about the nodes, including visual pruning by viewing thhe decrease in deviance created by a split relative to other splits in the grown tree, and an output table containing useful information.'
 
 # Setting up
 setup(
         name="TREEplusrepository", 
         version=VERSION,
```

