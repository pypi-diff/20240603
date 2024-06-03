# Comparing `tmp/treeplusrepository-0.1.5.tar.gz` & `tmp/treeplusrepository-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "treeplusrepository-0.1.5.tar", last modified: Mon Jun  3 12:42:42 2024, max compression
+gzip compressed data, was "treeplusrepository-0.1.6.tar", last modified: Mon Jun  3 12:59:15 2024, max compression
```

## Comparing `treeplusrepository-0.1.5.tar` & `treeplusrepository-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-06-03 12:42:42.957000 treeplusrepository-0.1.5/
--rw-rw-rw-   0        0        0     1029 2024-06-03 12:42:42.890000 treeplusrepository-0.1.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-06-03 12:42:42.325000 treeplusrepository-0.1.5/TREEplusrepository/
--rw-rw-rw-   0        0        0   170613 2024-06-03 12:01:14.000000 treeplusrepository-0.1.5/TREEplusrepository/TREEplus.py
--rw-rw-rw-   0        0        0       65 2024-06-03 12:26:28.000000 treeplusrepository-0.1.5/TREEplusrepository/__init__.py
--rw-rw-rw-   0        0        0     1390 2024-06-03 12:41:10.000000 treeplusrepository-0.1.5/TREEplusrepository/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-03 12:42:42.847000 treeplusrepository-0.1.5/TREEplusrepository.egg-info/
--rw-rw-rw-   0        0        0     1029 2024-06-03 12:42:41.000000 treeplusrepository-0.1.5/TREEplusrepository.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2024-06-03 12:42:41.000000 treeplusrepository-0.1.5/TREEplusrepository.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 12:42:41.000000 treeplusrepository-0.1.5/TREEplusrepository.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-06-03 12:42:41.000000 treeplusrepository-0.1.5/TREEplusrepository.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-03 12:42:42.944000 treeplusrepository-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1390 2024-06-03 12:41:03.000000 treeplusrepository-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 12:59:15.196000 treeplusrepository-0.1.6/
+-rw-rw-rw-   0        0        0      980 2024-06-03 12:59:15.133000 treeplusrepository-0.1.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-03 12:59:14.668000 treeplusrepository-0.1.6/TREEplusrepository/
+-rw-rw-rw-   0        0        0   170613 2024-06-03 12:01:14.000000 treeplusrepository-0.1.6/TREEplusrepository/TREEplus.py
+-rw-rw-rw-   0        0        0       24 2024-06-03 12:58:12.000000 treeplusrepository-0.1.6/TREEplusrepository/__init__.py
+-rw-rw-rw-   0        0        0     1338 2024-06-03 12:58:48.000000 treeplusrepository-0.1.6/TREEplusrepository/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 12:59:15.085000 treeplusrepository-0.1.6/TREEplusrepository.egg-info/
+-rw-rw-rw-   0        0        0      980 2024-06-03 12:59:13.000000 treeplusrepository-0.1.6/TREEplusrepository.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2024-06-03 12:59:14.000000 treeplusrepository-0.1.6/TREEplusrepository.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 12:59:13.000000 treeplusrepository-0.1.6/TREEplusrepository.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-06-03 12:59:13.000000 treeplusrepository-0.1.6/TREEplusrepository.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 12:59:15.188000 treeplusrepository-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1338 2024-06-03 12:58:53.000000 treeplusrepository-0.1.6/setup.py
```

### Comparing `treeplusrepository-0.1.5/PKG-INFO` & `treeplusrepository-0.1.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: TREEplusrepository
-Version: 0.1.5
+Version: 0.1.6
 Summary: Standard and Non-Standard Tree Based Methods
 Author: Daniel Fynn
 Author-email: <df390@uowmail.edu.au>
 Keywords: python,tree,CART
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 
 The library contains standard CART based methologies for growing trees, includind twoing, as well as non standard techniques two-stage techniques like fast and latent-budget tree. There is also cross validation methods for pruning the tree, and k-folds implementation. As well as a graphical interface to view the tree and information about the nodes, including visual pruning by viewing thhe decrease in deviance created by a split relative to other splits in the grown tree, and an output table containing useful information.
```

### Comparing `treeplusrepository-0.1.5/TREEplusrepository/TREEplus.py` & `treeplusrepository-0.1.6/TREEplusrepository/TREEplus.py`

 * *Files identical despite different names*

### Comparing `treeplusrepository-0.1.5/TREEplusrepository/setup.py` & `treeplusrepository-0.1.6/TREEplusrepository/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.5' 
+VERSION = '0.1.6' 
 DESCRIPTION = 'Standard and Non-Standard Tree Based Methods'
 LONG_DESCRIPTION = 'The library contains standard CART based methologies for growing trees, includind twoing, as well as non standard techniques two-stage techniques like fast and latent-budget tree. There is also cross validation methods for pruning the tree, and k-folds implementation. As well as a graphical interface to view the tree and information about the nodes, including visual pruning by viewing thhe decrease in deviance created by a split relative to other splits in the grown tree, and an output table containing useful information.'
 
 # Setting up
 setup(
         name="TREEplusrepository", 
         version=VERSION,
@@ -15,13 +15,12 @@
         packages=find_packages(),
         install_requires=[], 
         
         keywords=['python', 'tree', 'CART'],
         classifiers= [
             "Development Status :: 3 - Alpha",
             "Intended Audience :: Education",
-            "Programming Language :: Python :: 2",
             "Programming Language :: Python :: 3",
             "Operating System :: MacOS :: MacOS X",
             "Operating System :: Microsoft :: Windows",
         ]
 )
```

### Comparing `treeplusrepository-0.1.5/TREEplusrepository.egg-info/PKG-INFO` & `treeplusrepository-0.1.6/TREEplusrepository.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: TREEplusrepository
-Version: 0.1.5
+Version: 0.1.6
 Summary: Standard and Non-Standard Tree Based Methods
 Author: Daniel Fynn
 Author-email: <df390@uowmail.edu.au>
 Keywords: python,tree,CART
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 
 The library contains standard CART based methologies for growing trees, includind twoing, as well as non standard techniques two-stage techniques like fast and latent-budget tree. There is also cross validation methods for pruning the tree, and k-folds implementation. As well as a graphical interface to view the tree and information about the nodes, including visual pruning by viewing thhe decrease in deviance created by a split relative to other splits in the grown tree, and an output table containing useful information.
```

### Comparing `treeplusrepository-0.1.5/setup.py` & `treeplusrepository-0.1.6/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.5' 
+VERSION = '0.1.6' 
 DESCRIPTION = 'Standard and Non-Standard Tree Based Methods'
 LONG_DESCRIPTION = 'The library contains standard CART based methologies for growing trees, includind twoing, as well as non standard techniques two-stage techniques like fast and latent-budget tree. There is also cross validation methods for pruning the tree, and k-folds implementation. As well as a graphical interface to view the tree and information about the nodes, including visual pruning by viewing thhe decrease in deviance created by a split relative to other splits in the grown tree, and an output table containing useful information.'
 
 # Setting up
 setup(
         name="TREEplusrepository", 
         version=VERSION,
@@ -15,13 +15,12 @@
         packages=find_packages(),
         install_requires=[], 
         
         keywords=['python', 'tree', 'CART'],
         classifiers= [
             "Development Status :: 3 - Alpha",
             "Intended Audience :: Education",
-            "Programming Language :: Python :: 2",
             "Programming Language :: Python :: 3",
             "Operating System :: MacOS :: MacOS X",
             "Operating System :: Microsoft :: Windows",
         ]
 )
```

