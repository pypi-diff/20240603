# Comparing `tmp/livepriceofgold_usa_rx168059-2024.0.0.3.2.tar.gz` & `tmp/livepriceofgold_usa_rx168059-2024.0.0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livepriceofgold_usa_rx168059-2024.0.0.3.2.tar", last modified: Mon Jun  3 09:24:18 2024, max compression
+gzip compressed data, was "livepriceofgold_usa_rx168059-2024.0.0.3.3.tar", last modified: Mon Jun  3 09:34:36 2024, max compression
```

## Comparing `livepriceofgold_usa_rx168059-2024.0.0.3.2.tar` & `livepriceofgold_usa_rx168059-2024.0.0.3.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-06-03 09:24:18.334375 livepriceofgold_usa_rx168059-2024.0.0.3.2/
--rw-rw-rw-   0        0        0    35823 2024-06-02 14:48:06.000000 livepriceofgold_usa_rx168059-2024.0.0.3.2/LICENSE
--rw-rw-rw-   0        0        0     1296 2024-06-03 09:24:18.333679 livepriceofgold_usa_rx168059-2024.0.0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0      650 2024-06-03 08:21:39.000000 livepriceofgold_usa_rx168059-2024.0.0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2024-06-03 09:24:18.332431 livepriceofgold_usa_rx168059-2024.0.0.3.2/livepriceofgold_usa_Rx168059.egg-info/
--rw-rw-rw-   0        0        0     1296 2024-06-03 09:24:18.000000 livepriceofgold_usa_rx168059-2024.0.0.3.2/livepriceofgold_usa_Rx168059.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2024-06-03 09:24:18.000000 livepriceofgold_usa_rx168059-2024.0.0.3.2/livepriceofgold_usa_Rx168059.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 09:24:18.000000 livepriceofgold_usa_rx168059-2024.0.0.3.2/livepriceofgold_usa_Rx168059.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-06-03 09:24:18.000000 livepriceofgold_usa_rx168059-2024.0.0.3.2/livepriceofgold_usa_Rx168059.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-06-03 09:24:18.330206 livepriceofgold_usa_rx168059-2024.0.0.3.2/priceofgold/
--rw-rw-rw-   0        0        0     1845 2024-06-03 08:14:35.000000 livepriceofgold_usa_rx168059-2024.0.0.3.2/priceofgold/__init__.py
--rw-rw-rw-   0        0        0      923 2024-06-03 09:24:04.000000 livepriceofgold_usa_rx168059-2024.0.0.3.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-06-03 09:24:18.334375 livepriceofgold_usa_rx168059-2024.0.0.3.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-03 09:34:36.870337 livepriceofgold_usa_rx168059-2024.0.0.3.3/
+-rw-rw-rw-   0        0        0    35823 2024-06-02 14:48:06.000000 livepriceofgold_usa_rx168059-2024.0.0.3.3/LICENSE
+-rw-rw-rw-   0        0        0     1296 2024-06-03 09:34:36.866806 livepriceofgold_usa_rx168059-2024.0.0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0      650 2024-06-03 08:21:39.000000 livepriceofgold_usa_rx168059-2024.0.0.3.3/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 09:34:36.866806 livepriceofgold_usa_rx168059-2024.0.0.3.3/livepriceofgold_usa_Rx168059.egg-info/
+-rw-rw-rw-   0        0        0     1296 2024-06-03 09:34:36.000000 livepriceofgold_usa_rx168059-2024.0.0.3.3/livepriceofgold_usa_Rx168059.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2024-06-03 09:34:36.000000 livepriceofgold_usa_rx168059-2024.0.0.3.3/livepriceofgold_usa_Rx168059.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 09:34:36.000000 livepriceofgold_usa_rx168059-2024.0.0.3.3/livepriceofgold_usa_Rx168059.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-06-03 09:34:36.000000 livepriceofgold_usa_rx168059-2024.0.0.3.3/livepriceofgold_usa_Rx168059.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-03 09:34:36.864494 livepriceofgold_usa_rx168059-2024.0.0.3.3/priceofgold/
+-rw-rw-rw-   0        0        0     1845 2024-06-03 08:14:35.000000 livepriceofgold_usa_rx168059-2024.0.0.3.3/priceofgold/__init__.py
+-rw-rw-rw-   0        0        0      923 2024-06-03 09:34:28.000000 livepriceofgold_usa_rx168059-2024.0.0.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-03 09:34:36.870337 livepriceofgold_usa_rx168059-2024.0.0.3.3/setup.cfg
```

### Comparing `livepriceofgold_usa_rx168059-2024.0.0.3.2/LICENSE` & `livepriceofgold_usa_rx168059-2024.0.0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `livepriceofgold_usa_rx168059-2024.0.0.3.2/PKG-INFO` & `livepriceofgold_usa_rx168059-2024.0.0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livepriceofgold-usa_Rx168059
-Version: 2024.0.0.3.2
+Version: 2024.0.0.3.3
 Summary: This package will get information about USA latest gold price from livepriceofgold website
 Author-email: Muhammad Dwi Reza <dwireza1002@gmail.com>
 Project-URL: Homepage, https://github.com/Rex-Project-Organization/IndonesiaLatestEarthQuake
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
```

### Comparing `livepriceofgold_usa_rx168059-2024.0.0.3.2/README.md` & `livepriceofgold_usa_rx168059-2024.0.0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `livepriceofgold_usa_rx168059-2024.0.0.3.2/livepriceofgold_usa_Rx168059.egg-info/PKG-INFO` & `livepriceofgold_usa_rx168059-2024.0.0.3.3/livepriceofgold_usa_Rx168059.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livepriceofgold-usa_Rx168059
-Version: 2024.0.0.3.2
+Version: 2024.0.0.3.3
 Summary: This package will get information about USA latest gold price from livepriceofgold website
 Author-email: Muhammad Dwi Reza <dwireza1002@gmail.com>
 Project-URL: Homepage, https://github.com/Rex-Project-Organization/IndonesiaLatestEarthQuake
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
```

### Comparing `livepriceofgold_usa_rx168059-2024.0.0.3.2/priceofgold/__init__.py` & `livepriceofgold_usa_rx168059-2024.0.0.3.3/priceofgold/__init__.py`

 * *Files identical despite different names*

### Comparing `livepriceofgold_usa_rx168059-2024.0.0.3.2/pyproject.toml` & `livepriceofgold_usa_rx168059-2024.0.0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [build-system]
 requires = ["setuptools>=70.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "livepriceofgold-usa_Rx168059"
-version = "2024.0.0.3.2"
+version = "2024.0.0.3.3"
 authors = [
   { name="Muhammad Dwi Reza", email="dwireza1002@gmail.com" },
 ]
 description = "This package will get information about USA latest gold price from livepriceofgold website"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
```

