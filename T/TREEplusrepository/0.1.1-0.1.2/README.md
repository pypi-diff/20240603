# Comparing `tmp/treeplusrepository-0.1.1.tar.gz` & `tmp/treeplusrepository-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "treeplusrepository-0.1.1.tar", last modified: Mon Jun  3 11:43:59 2024, max compression
+gzip compressed data, was "treeplusrepository-0.1.2.tar", last modified: Mon Jun  3 12:03:03 2024, max compression
```

## Comparing `treeplusrepository-0.1.1.tar` & `treeplusrepository-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-06-03 11:43:59.980000 treeplusrepository-0.1.1/
--rw-rw-rw-   0        0        0     1029 2024-06-03 11:43:59.911000 treeplusrepository-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-06-03 11:43:59.434000 treeplusrepository-0.1.1/TREEplusrepository/
--rw-rw-rw-   0        0        0   170607 2024-06-03 10:03:28.000000 treeplusrepository-0.1.1/TREEplusrepository/TREEplus.py
--rw-rw-rw-   0        0        0       42 2024-06-03 11:42:10.000000 treeplusrepository-0.1.1/TREEplusrepository/__init__.py
--rw-rw-rw-   0        0        0     1390 2024-06-03 11:43:49.000000 treeplusrepository-0.1.1/TREEplusrepository/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-03 11:43:59.862000 treeplusrepository-0.1.1/TREEplusrepository.egg-info/
--rw-rw-rw-   0        0        0     1029 2024-06-03 11:43:58.000000 treeplusrepository-0.1.1/TREEplusrepository.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2024-06-03 11:43:58.000000 treeplusrepository-0.1.1/TREEplusrepository.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 11:43:58.000000 treeplusrepository-0.1.1/TREEplusrepository.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-06-03 11:43:58.000000 treeplusrepository-0.1.1/TREEplusrepository.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-03 11:43:59.970000 treeplusrepository-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1390 2024-06-03 11:43:44.000000 treeplusrepository-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 12:03:03.932000 treeplusrepository-0.1.2/
+-rw-rw-rw-   0        0        0     1029 2024-06-03 12:03:03.837000 treeplusrepository-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-03 12:03:03.441000 treeplusrepository-0.1.2/TREEplusrepository/
+-rw-rw-rw-   0        0        0   170613 2024-06-03 12:01:14.000000 treeplusrepository-0.1.2/TREEplusrepository/TREEplus.py
+-rw-rw-rw-   0        0        0       42 2024-06-03 11:42:10.000000 treeplusrepository-0.1.2/TREEplusrepository/__init__.py
+-rw-rw-rw-   0        0        0     1390 2024-06-03 12:02:49.000000 treeplusrepository-0.1.2/TREEplusrepository/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 12:03:03.794000 treeplusrepository-0.1.2/TREEplusrepository.egg-info/
+-rw-rw-rw-   0        0        0     1029 2024-06-03 12:03:02.000000 treeplusrepository-0.1.2/TREEplusrepository.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2024-06-03 12:03:02.000000 treeplusrepository-0.1.2/TREEplusrepository.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 12:03:02.000000 treeplusrepository-0.1.2/TREEplusrepository.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-06-03 12:03:02.000000 treeplusrepository-0.1.2/TREEplusrepository.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 12:03:03.923000 treeplusrepository-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1390 2024-06-03 12:02:45.000000 treeplusrepository-0.1.2/setup.py
```

### Comparing `treeplusrepository-0.1.1/PKG-INFO` & `treeplusrepository-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TREEplusrepository
-Version: 0.1.1
+Version: 0.1.2
 Summary: Standard and Non-Standard Tree Based Methods
 Author: Daniel Fynn
 Author-email: <df390@uowmail.edu.au>
 Keywords: python,tree,CART
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `treeplusrepository-0.1.1/TREEplusrepository/TREEplus.py` & `treeplusrepository-0.1.2/TREEplusrepository/TREEplus.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-Copyright 2024 Daniel Fynn
-This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
-
-This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
+#Copyright 2024 Daniel Fynn
+#This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+#
+#This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+#
+#You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
 
 import itertools #base library
 import math #base library
 import numpy as np # use numpy arraysfrom
 from  statistics import mean,variance,mode #base library
 from anytree import Node, RenderTree, NodeMixin
 from collections import Counter #base library
```

### Comparing `treeplusrepository-0.1.1/TREEplusrepository/setup.py` & `treeplusrepository-0.1.2/TREEplusrepository/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.1' 
+VERSION = '0.1.2' 
 DESCRIPTION = 'Standard and Non-Standard Tree Based Methods'
 LONG_DESCRIPTION = 'The library contains standard CART based methologies for growing trees, includind twoing, as well as non standard techniques two-stage techniques like fast and latent-budget tree. There is also cross validation methods for pruning the tree, and k-folds implementation. As well as a graphical interface to view the tree and information about the nodes, including visual pruning by viewing thhe decrease in deviance created by a split relative to other splits in the grown tree, and an output table containing useful information.'
 
 # Setting up
 setup(
         name="TREEplusrepository", 
         version=VERSION,
```

### Comparing `treeplusrepository-0.1.1/TREEplusrepository.egg-info/PKG-INFO` & `treeplusrepository-0.1.2/TREEplusrepository.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TREEplusrepository
-Version: 0.1.1
+Version: 0.1.2
 Summary: Standard and Non-Standard Tree Based Methods
 Author: Daniel Fynn
 Author-email: <df390@uowmail.edu.au>
 Keywords: python,tree,CART
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `treeplusrepository-0.1.1/setup.py` & `treeplusrepository-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.1' 
+VERSION = '0.1.2' 
 DESCRIPTION = 'Standard and Non-Standard Tree Based Methods'
 LONG_DESCRIPTION = 'The library contains standard CART based methologies for growing trees, includind twoing, as well as non standard techniques two-stage techniques like fast and latent-budget tree. There is also cross validation methods for pruning the tree, and k-folds implementation. As well as a graphical interface to view the tree and information about the nodes, including visual pruning by viewing thhe decrease in deviance created by a split relative to other splits in the grown tree, and an output table containing useful information.'
 
 # Setting up
 setup(
         name="TREEplusrepository", 
         version=VERSION,
```

