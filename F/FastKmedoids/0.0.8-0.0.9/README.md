# Comparing `tmp/fastkmedoids-0.0.8.tar.gz` & `tmp/fastkmedoids-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastkmedoids-0.0.8.tar", last modified: Sun Jun  2 06:35:09 2024, max compression
+gzip compressed data, was "fastkmedoids-0.0.9.tar", last modified: Sun Jun  2 06:39:20 2024, max compression
```

## Comparing `fastkmedoids-0.0.8.tar` & `fastkmedoids-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 06:35:09.606778 fastkmedoids-0.0.8/
-drwxrwxrwx   0        0        0        0 2024-06-02 06:35:09.602823 fastkmedoids-0.0.8/FastKmedoids.egg-info/
--rw-rw-rw-   0        0        0      894 2024-06-02 06:35:09.000000 fastkmedoids-0.0.8/FastKmedoids.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2024-06-02 06:35:09.000000 fastkmedoids-0.0.8/FastKmedoids.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 06:35:09.000000 fastkmedoids-0.0.8/FastKmedoids.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-06-02 06:35:09.000000 fastkmedoids-0.0.8/FastKmedoids.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 06:35:09.000000 fastkmedoids-0.0.8/FastKmedoids.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-12-09 15:06:56.000000 fastkmedoids-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      894 2024-06-02 06:35:09.604465 fastkmedoids-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      208 2024-02-14 16:49:17.000000 fastkmedoids-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2024-06-02 06:35:09.606778 fastkmedoids-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      951 2024-06-02 06:34:37.000000 fastkmedoids-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 06:39:20.711563 fastkmedoids-0.0.9/
+drwxrwxrwx   0        0        0        0 2024-06-02 06:39:20.662956 fastkmedoids-0.0.9/FastKmedoids/
+-rw-rw-rw-   0        0        0      184 2024-03-25 15:05:18.000000 fastkmedoids-0.0.9/FastKmedoids/__init__.py
+-rw-rw-rw-   0        0        0     5428 2024-04-20 10:49:42.000000 fastkmedoids-0.0.9/FastKmedoids/data.py
+-rw-rw-rw-   0        0        0     1355 2024-04-19 21:47:46.000000 fastkmedoids-0.0.9/FastKmedoids/metrics.py
+-rw-rw-rw-   0        0        0    27139 2024-05-04 14:31:47.000000 fastkmedoids-0.0.9/FastKmedoids/models.py
+-rw-rw-rw-   0        0        0    11982 2024-05-01 22:28:06.000000 fastkmedoids-0.0.9/FastKmedoids/plots.py
+drwxrwxrwx   0        0        0        0 2024-06-02 06:39:20.710687 fastkmedoids-0.0.9/FastKmedoids.egg-info/
+-rw-rw-rw-   0        0        0      894 2024-06-02 06:39:20.000000 fastkmedoids-0.0.9/FastKmedoids.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2024-06-02 06:39:20.000000 fastkmedoids-0.0.9/FastKmedoids.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 06:39:20.000000 fastkmedoids-0.0.9/FastKmedoids.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-06-02 06:39:20.000000 fastkmedoids-0.0.9/FastKmedoids.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-06-02 06:39:20.000000 fastkmedoids-0.0.9/FastKmedoids.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-12-09 15:06:56.000000 fastkmedoids-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      894 2024-06-02 06:39:20.711563 fastkmedoids-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2024-02-14 16:49:17.000000 fastkmedoids-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-02 06:39:20.711563 fastkmedoids-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      951 2024-06-02 06:38:37.000000 fastkmedoids-0.0.9/setup.py
```

### Comparing `fastkmedoids-0.0.8/FastKmedoids.egg-info/PKG-INFO` & `fastkmedoids-0.0.9/FastKmedoids.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FastKmedoids
-Version: 0.0.8
+Version: 0.0.9
 Summary: This is a package to implement a fast and powerful version of the Kmedoids clustering algorithm, which is built on the Generalised Gower distance, already available in the PyDistances package
 Home-page: https://github.com/FabioScielzoOrtiz/FastKmedoids_Package
 Author: Fabio Scielzo Ortiz
 Author-email: fabioscielzo98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fastkmedoids-0.0.8/LICENSE` & `fastkmedoids-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fastkmedoids-0.0.8/PKG-INFO` & `fastkmedoids-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FastKmedoids
-Version: 0.0.8
+Version: 0.0.9
 Summary: This is a package to implement a fast and powerful version of the Kmedoids clustering algorithm, which is built on the Generalised Gower distance, already available in the PyDistances package
 Home-page: https://github.com/FabioScielzoOrtiz/FastKmedoids_Package
 Author: Fabio Scielzo Ortiz
 Author-email: fabioscielzo98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fastkmedoids-0.0.8/setup.py` & `fastkmedoids-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="FastKmedoids",
-    version="0.0.8",
+    version="0.0.9",
     author="Fabio Scielzo Ortiz",
     author_email="fabioscielzo98@gmail.com",
     description="This is a package to implement a fast and powerful version of the Kmedoids clustering algorithm, which is built on the Generalised Gower distance, already available in the PyDistances package",    long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/FabioScielzoOrtiz/FastKmedoids_Package",  # add your project URL here
     packages=find_packages(),
     classifiers=[
```

