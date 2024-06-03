# Comparing `tmp/zaiscikit-0.1.0.tar.gz` & `tmp/zaiscikit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zaiscikit-0.1.0.tar", last modified: Mon Jun  3 08:39:01 2024, max compression
+gzip compressed data, was "zaiscikit-0.1.1.tar", last modified: Mon Jun  3 08:43:11 2024, max compression
```

## Comparing `zaiscikit-0.1.0.tar` & `zaiscikit-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-06-03 08:39:01.329643 zaiscikit-0.1.0/
--rw-rw-rw-   0        0        0       36 2024-06-03 08:11:06.000000 zaiscikit-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1453 2024-06-03 08:39:01.329643 zaiscikit-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1023 2024-06-03 07:12:29.000000 zaiscikit-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-06-03 08:39:01.310643 zaiscikit-0.1.0/ZAIScikit/
--rw-rw-rw-   0        0        0        0 2024-06-03 08:04:21.000000 zaiscikit-0.1.0/ZAIScikit/__init__.py
--rw-rw-rw-   0        0        0     5006 2024-06-03 06:51:05.000000 zaiscikit-0.1.0/ZAIScikit/bagging.py
--rw-rw-rw-   0        0        0     7325 2024-06-03 07:04:47.000000 zaiscikit-0.1.0/ZAIScikit/boosting.py
--rw-rw-rw-   0        0        0    11090 2024-06-03 06:48:53.000000 zaiscikit-0.1.0/ZAIScikit/decision_tree.py
--rw-rw-rw-   0        0        0     4154 2024-06-03 06:35:23.000000 zaiscikit-0.1.0/ZAIScikit/encoding.py
--rw-rw-rw-   0        0        0     6376 2024-06-03 06:35:23.000000 zaiscikit-0.1.0/ZAIScikit/feature_selection.py
--rw-rw-rw-   0        0        0     3090 2024-06-03 06:35:23.000000 zaiscikit-0.1.0/ZAIScikit/grid_search.py
--rw-rw-rw-   0        0        0     7496 2024-06-03 07:07:24.000000 zaiscikit-0.1.0/ZAIScikit/imputation.py
--rw-rw-rw-   0        0        0     3650 2024-06-03 04:53:53.000000 zaiscikit-0.1.0/ZAIScikit/kmeans.py
--rw-rw-rw-   0        0        0     7189 2024-06-03 07:07:20.000000 zaiscikit-0.1.0/ZAIScikit/linear_models.py
--rw-rw-rw-   0        0        0     6862 2024-06-03 06:35:23.000000 zaiscikit-0.1.0/ZAIScikit/metrics.py
--rw-rw-rw-   0        0        0     8353 2024-06-03 06:47:44.000000 zaiscikit-0.1.0/ZAIScikit/mlp.py
--rw-rw-rw-   0        0        0     5518 2024-06-03 06:35:23.000000 zaiscikit-0.1.0/ZAIScikit/naive_bayes.py
--rw-rw-rw-   0        0        0     1435 2024-06-03 06:35:23.000000 zaiscikit-0.1.0/ZAIScikit/nearest_neighbors.py
--rw-rw-rw-   0        0        0     1782 2024-06-03 04:53:23.000000 zaiscikit-0.1.0/ZAIScikit/pca.py
--rw-rw-rw-   0        0        0     1435 2024-06-03 07:01:04.000000 zaiscikit-0.1.0/ZAIScikit/scaler.py
--rw-rw-rw-   0        0        0     6961 2024-06-03 07:01:04.000000 zaiscikit-0.1.0/ZAIScikit/sklearn_base.py
--rw-rw-rw-   0        0        0     3402 2024-06-03 07:07:48.000000 zaiscikit-0.1.0/ZAIScikit/splitting.py
--rw-rw-rw-   0        0        0      475 2024-06-03 03:43:39.000000 zaiscikit-0.1.0/ZAIScikit/utilities.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:39:01.328645 zaiscikit-0.1.0/ZAIScikit.egg-info/
--rw-rw-rw-   0        0        0     1453 2024-06-03 08:39:01.000000 zaiscikit-0.1.0/ZAIScikit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      616 2024-06-03 08:39:01.000000 zaiscikit-0.1.0/ZAIScikit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 08:39:01.000000 zaiscikit-0.1.0/ZAIScikit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-06-03 08:39:01.000000 zaiscikit-0.1.0/ZAIScikit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-06-03 08:39:01.330645 zaiscikit-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      617 2024-06-03 08:06:50.000000 zaiscikit-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:43:11.370916 zaiscikit-0.1.1/
+-rw-rw-rw-   0        0        0     1090 2024-06-03 08:41:54.000000 zaiscikit-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0       36 2024-06-03 08:11:06.000000 zaiscikit-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1476 2024-06-03 08:43:11.370916 zaiscikit-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1023 2024-06-03 07:12:29.000000 zaiscikit-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 08:43:11.353919 zaiscikit-0.1.1/ZAIScikit/
+-rw-rw-rw-   0        0        0        0 2024-06-03 08:04:21.000000 zaiscikit-0.1.1/ZAIScikit/__init__.py
+-rw-rw-rw-   0        0        0     5006 2024-06-03 06:51:05.000000 zaiscikit-0.1.1/ZAIScikit/bagging.py
+-rw-rw-rw-   0        0        0     7325 2024-06-03 07:04:47.000000 zaiscikit-0.1.1/ZAIScikit/boosting.py
+-rw-rw-rw-   0        0        0    11090 2024-06-03 06:48:53.000000 zaiscikit-0.1.1/ZAIScikit/decision_tree.py
+-rw-rw-rw-   0        0        0     4154 2024-06-03 06:35:23.000000 zaiscikit-0.1.1/ZAIScikit/encoding.py
+-rw-rw-rw-   0        0        0     6376 2024-06-03 06:35:23.000000 zaiscikit-0.1.1/ZAIScikit/feature_selection.py
+-rw-rw-rw-   0        0        0     3090 2024-06-03 06:35:23.000000 zaiscikit-0.1.1/ZAIScikit/grid_search.py
+-rw-rw-rw-   0        0        0     7496 2024-06-03 07:07:24.000000 zaiscikit-0.1.1/ZAIScikit/imputation.py
+-rw-rw-rw-   0        0        0     3650 2024-06-03 04:53:53.000000 zaiscikit-0.1.1/ZAIScikit/kmeans.py
+-rw-rw-rw-   0        0        0     7189 2024-06-03 07:07:20.000000 zaiscikit-0.1.1/ZAIScikit/linear_models.py
+-rw-rw-rw-   0        0        0     6862 2024-06-03 06:35:23.000000 zaiscikit-0.1.1/ZAIScikit/metrics.py
+-rw-rw-rw-   0        0        0     8353 2024-06-03 06:47:44.000000 zaiscikit-0.1.1/ZAIScikit/mlp.py
+-rw-rw-rw-   0        0        0     5518 2024-06-03 06:35:23.000000 zaiscikit-0.1.1/ZAIScikit/naive_bayes.py
+-rw-rw-rw-   0        0        0     1435 2024-06-03 06:35:23.000000 zaiscikit-0.1.1/ZAIScikit/nearest_neighbors.py
+-rw-rw-rw-   0        0        0     1782 2024-06-03 04:53:23.000000 zaiscikit-0.1.1/ZAIScikit/pca.py
+-rw-rw-rw-   0        0        0     1435 2024-06-03 07:01:04.000000 zaiscikit-0.1.1/ZAIScikit/scaler.py
+-rw-rw-rw-   0        0        0     6961 2024-06-03 07:01:04.000000 zaiscikit-0.1.1/ZAIScikit/sklearn_base.py
+-rw-rw-rw-   0        0        0     3402 2024-06-03 07:07:48.000000 zaiscikit-0.1.1/ZAIScikit/splitting.py
+-rw-rw-rw-   0        0        0      475 2024-06-03 03:43:39.000000 zaiscikit-0.1.1/ZAIScikit/utilities.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:43:11.369919 zaiscikit-0.1.1/ZAIScikit.egg-info/
+-rw-rw-rw-   0        0        0     1476 2024-06-03 08:43:11.000000 zaiscikit-0.1.1/ZAIScikit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      624 2024-06-03 08:43:11.000000 zaiscikit-0.1.1/ZAIScikit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 08:43:11.000000 zaiscikit-0.1.1/ZAIScikit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-06-03 08:43:11.000000 zaiscikit-0.1.1/ZAIScikit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-06-03 08:43:11.372919 zaiscikit-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      617 2024-06-03 08:43:05.000000 zaiscikit-0.1.1/setup.py
```

### Comparing `zaiscikit-0.1.0/PKG-INFO` & `zaiscikit-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: ZAIScikit
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Machine learning library
 Home-page: https://github.com/Zakaria-El-Maachi/ZAI-Scikit
 Author: Zakaria
 Author-email: zakaria.elmaachi19@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Z-MachineLearningLibrary
 Our Personal Machine Learning Library
 
 This is a Machine Learning library that Abderrahmane Baidoune, Imane Rahali I would like to build in order to further our understanding of the algorithms and implement them from scratch with the help of numpy, no more.
 
 Thus, optimization is not a concern to us, nor is documentation or code readability. Having said that, we will, and have tried to devote some effort to it !
```

### Comparing `zaiscikit-0.1.0/README.md` & `zaiscikit-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `zaiscikit-0.1.0/ZAIScikit/bagging.py` & `zaiscikit-0.1.1/ZAIScikit/bagging.py`

 * *Files identical despite different names*

### Comparing `zaiscikit-0.1.0/ZAIScikit/boosting.py` & `zaiscikit-0.1.1/ZAIScikit/boosting.py`

 * *Files identical despite different names*

### Comparing `zaiscikit-0.1.0/ZAIScikit/decision_tree.py` & `zaiscikit-0.1.1/ZAIScikit/decision_tree.py`

 * *Files identical despite different names*

### Comparing `zaiscikit-0.1.0/ZAIScikit/encoding.py` & `zaiscikit-0.1.1/ZAIScikit/encoding.py`

 * *Files identical despite different names*

### Comparing `zaiscikit-0.1.0/ZAIScikit/feature_selection.py` & `zaiscikit-0.1.1/ZAIScikit/feature_selection.py`

 * *Files identical despite different names*

### Comparing `zaiscikit-0.1.0/ZAIScikit/grid_search.py` & `zaiscikit-0.1.1/ZAIScikit/grid_search.py`

 * *Files identical despite different names*

### Comparing `zaiscikit-0.1.0/ZAIScikit/imputation.py` & `zaiscikit-0.1.1/ZAIScikit/imputation.py`

 * *Files identical despite different names*

### Comparing `zaiscikit-0.1.0/ZAIScikit/kmeans.py` & `zaiscikit-0.1.1/ZAIScikit/kmeans.py`

 * *Files identical despite different names*

### Comparing `zaiscikit-0.1.0/ZAIScikit/linear_models.py` & `zaiscikit-0.1.1/ZAIScikit/linear_models.py`

 * *Files identical despite different names*

### Comparing `zaiscikit-0.1.0/ZAIScikit/metrics.py` & `zaiscikit-0.1.1/ZAIScikit/metrics.py`

 * *Files identical despite different names*

### Comparing `zaiscikit-0.1.0/ZAIScikit/mlp.py` & `zaiscikit-0.1.1/ZAIScikit/mlp.py`

 * *Files identical despite different names*

### Comparing `zaiscikit-0.1.0/ZAIScikit/naive_bayes.py` & `zaiscikit-0.1.1/ZAIScikit/naive_bayes.py`

 * *Files identical despite different names*

### Comparing `zaiscikit-0.1.0/ZAIScikit/nearest_neighbors.py` & `zaiscikit-0.1.1/ZAIScikit/nearest_neighbors.py`

 * *Files identical despite different names*

### Comparing `zaiscikit-0.1.0/ZAIScikit/pca.py` & `zaiscikit-0.1.1/ZAIScikit/pca.py`

 * *Files identical despite different names*

### Comparing `zaiscikit-0.1.0/ZAIScikit/scaler.py` & `zaiscikit-0.1.1/ZAIScikit/scaler.py`

 * *Files identical despite different names*

### Comparing `zaiscikit-0.1.0/ZAIScikit/sklearn_base.py` & `zaiscikit-0.1.1/ZAIScikit/sklearn_base.py`

 * *Files identical despite different names*

### Comparing `zaiscikit-0.1.0/ZAIScikit/splitting.py` & `zaiscikit-0.1.1/ZAIScikit/splitting.py`

 * *Files identical despite different names*

### Comparing `zaiscikit-0.1.0/ZAIScikit.egg-info/PKG-INFO` & `zaiscikit-0.1.1/ZAIScikit.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: ZAIScikit
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Machine learning library
 Home-page: https://github.com/Zakaria-El-Maachi/ZAI-Scikit
 Author: Zakaria
 Author-email: zakaria.elmaachi19@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Z-MachineLearningLibrary
 Our Personal Machine Learning Library
 
 This is a Machine Learning library that Abderrahmane Baidoune, Imane Rahali I would like to build in order to further our understanding of the algorithms and implement them from scratch with the help of numpy, no more.
 
 Thus, optimization is not a concern to us, nor is documentation or code readability. Having said that, we will, and have tried to devote some effort to it !
```

### Comparing `zaiscikit-0.1.0/ZAIScikit.egg-info/SOURCES.txt` & `zaiscikit-0.1.1/ZAIScikit.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 ZAIScikit/__init__.py
 ZAIScikit/bagging.py
 ZAIScikit/boosting.py
```

### Comparing `zaiscikit-0.1.0/setup.py` & `zaiscikit-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ZAIScikit',
-    version='0.1.0',
+    version='0.1.1',
     author='Zakaria',
     author_email='zakaria.elmaachi19@gmail.com',
     description='A Machine learning library',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Zakaria-El-Maachi/ZAI-Scikit',
     packages=find_packages(),
```

