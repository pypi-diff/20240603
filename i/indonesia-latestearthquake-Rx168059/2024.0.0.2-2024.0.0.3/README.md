# Comparing `tmp/indonesia_latestearthquake_rx168059-2024.0.0.2.tar.gz` & `tmp/indonesia_latestearthquake_rx168059-2024.0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indonesia_latestearthquake_rx168059-2024.0.0.2.tar", last modified: Mon Jun  3 05:16:30 2024, max compression
+gzip compressed data, was "indonesia_latestearthquake_rx168059-2024.0.0.3.tar", last modified: Mon Jun  3 05:29:22 2024, max compression
```

## Comparing `indonesia_latestearthquake_rx168059-2024.0.0.2.tar` & `indonesia_latestearthquake_rx168059-2024.0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-06-03 05:16:30.865496 indonesia_latestearthquake_rx168059-2024.0.0.2/
--rw-rw-rw-   0        0        0    35823 2024-06-02 11:16:38.000000 indonesia_latestearthquake_rx168059-2024.0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1302 2024-06-03 05:16:30.863124 indonesia_latestearthquake_rx168059-2024.0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      605 2024-06-03 05:12:18.000000 indonesia_latestearthquake_rx168059-2024.0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-06-03 05:16:30.842462 indonesia_latestearthquake_rx168059-2024.0.0.2/gempaTerkini/
--rw-rw-rw-   0        0        0     2669 2024-06-03 05:10:00.000000 indonesia_latestearthquake_rx168059-2024.0.0.2/gempaTerkini/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-03 05:16:30.860727 indonesia_latestearthquake_rx168059-2024.0.0.2/indonesia_latestearthquake_Rx168059.egg-info/
--rw-rw-rw-   0        0        0     1302 2024-06-03 05:16:30.000000 indonesia_latestearthquake_rx168059-2024.0.0.2/indonesia_latestearthquake_Rx168059.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2024-06-03 05:16:30.000000 indonesia_latestearthquake_rx168059-2024.0.0.2/indonesia_latestearthquake_Rx168059.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 05:16:30.000000 indonesia_latestearthquake_rx168059-2024.0.0.2/indonesia_latestearthquake_Rx168059.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-06-03 05:16:30.000000 indonesia_latestearthquake_rx168059-2024.0.0.2/indonesia_latestearthquake_Rx168059.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      974 2024-06-03 05:02:09.000000 indonesia_latestearthquake_rx168059-2024.0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-06-03 05:16:30.865496 indonesia_latestearthquake_rx168059-2024.0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-03 05:29:22.437391 indonesia_latestearthquake_rx168059-2024.0.0.3/
+-rw-rw-rw-   0        0        0    35823 2024-06-02 11:16:38.000000 indonesia_latestearthquake_rx168059-2024.0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1302 2024-06-03 05:29:22.437391 indonesia_latestearthquake_rx168059-2024.0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      605 2024-06-03 05:22:24.000000 indonesia_latestearthquake_rx168059-2024.0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 05:29:22.422341 indonesia_latestearthquake_rx168059-2024.0.0.3/gempaTerkini/
+-rw-rw-rw-   0        0        0     2669 2024-06-03 05:10:00.000000 indonesia_latestearthquake_rx168059-2024.0.0.3/gempaTerkini/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 05:29:22.437391 indonesia_latestearthquake_rx168059-2024.0.0.3/indonesia_latestearthquake_Rx168059.egg-info/
+-rw-rw-rw-   0        0        0     1302 2024-06-03 05:29:22.000000 indonesia_latestearthquake_rx168059-2024.0.0.3/indonesia_latestearthquake_Rx168059.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2024-06-03 05:29:22.000000 indonesia_latestearthquake_rx168059-2024.0.0.3/indonesia_latestearthquake_Rx168059.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 05:29:22.000000 indonesia_latestearthquake_rx168059-2024.0.0.3/indonesia_latestearthquake_Rx168059.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-06-03 05:29:22.000000 indonesia_latestearthquake_rx168059-2024.0.0.3/indonesia_latestearthquake_Rx168059.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      974 2024-06-03 05:22:24.000000 indonesia_latestearthquake_rx168059-2024.0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-03 05:29:22.437391 indonesia_latestearthquake_rx168059-2024.0.0.3/setup.cfg
```

### Comparing `indonesia_latestearthquake_rx168059-2024.0.0.2/LICENSE` & `indonesia_latestearthquake_rx168059-2024.0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `indonesia_latestearthquake_rx168059-2024.0.0.2/PKG-INFO` & `indonesia_latestearthquake_rx168059-2024.0.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indonesia-latestearthquake_Rx168059
-Version: 2024.0.0.2
+Version: 2024.0.0.3
 Summary: This package will get information about latest earthquake from BMKG(Indonesian Agency for Meteorological, Climatological and Geophysics)
 Author-email: Muhammad Dwi Reza <dwireza1002@gmail.com>
 Project-URL: Homepage, https://github.com/Rex-Project-Organization/IndonesiaLatestEarthQuake
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
@@ -17,17 +17,17 @@
 
 ## How It Works
 This package will scrap data from [BMKG](https://www.bmkg.go.id/) to get information about latest earthquake on indonesia
 
 This package used BeautifulSoup4 and Requests to generate JSON output that'll be used for web or mobile apps
 
 # How to Run
-"""
+```
 import gempaTerkini
 
 if __name__ == '__main__':
     result = gempaTerkini.data_extract()
     gempaTerkini.show_data(result)
-"""
+```
 
 # Author
 Muhammad Dwi Reza
```

### Comparing `indonesia_latestearthquake_rx168059-2024.0.0.2/README.md` & `indonesia_latestearthquake_rx168059-2024.0.0.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 ## How It Works
 This package will scrap data from [BMKG](https://www.bmkg.go.id/) to get information about latest earthquake on indonesia
 
 This package used BeautifulSoup4 and Requests to generate JSON output that'll be used for web or mobile apps
 
 # How to Run
-"""
+```
 import gempaTerkini
 
 if __name__ == '__main__':
     result = gempaTerkini.data_extract()
     gempaTerkini.show_data(result)
-"""
+```
 
 # Author
 Muhammad Dwi Reza
```

### Comparing `indonesia_latestearthquake_rx168059-2024.0.0.2/gempaTerkini/__init__.py` & `indonesia_latestearthquake_rx168059-2024.0.0.3/gempaTerkini/__init__.py`

 * *Files identical despite different names*

### Comparing `indonesia_latestearthquake_rx168059-2024.0.0.2/indonesia_latestearthquake_Rx168059.egg-info/PKG-INFO` & `indonesia_latestearthquake_rx168059-2024.0.0.3/indonesia_latestearthquake_Rx168059.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indonesia-latestearthquake_Rx168059
-Version: 2024.0.0.2
+Version: 2024.0.0.3
 Summary: This package will get information about latest earthquake from BMKG(Indonesian Agency for Meteorological, Climatological and Geophysics)
 Author-email: Muhammad Dwi Reza <dwireza1002@gmail.com>
 Project-URL: Homepage, https://github.com/Rex-Project-Organization/IndonesiaLatestEarthQuake
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
@@ -17,17 +17,17 @@
 
 ## How It Works
 This package will scrap data from [BMKG](https://www.bmkg.go.id/) to get information about latest earthquake on indonesia
 
 This package used BeautifulSoup4 and Requests to generate JSON output that'll be used for web or mobile apps
 
 # How to Run
-"""
+```
 import gempaTerkini
 
 if __name__ == '__main__':
     result = gempaTerkini.data_extract()
     gempaTerkini.show_data(result)
-"""
+```
 
 # Author
 Muhammad Dwi Reza
```

### Comparing `indonesia_latestearthquake_rx168059-2024.0.0.2/pyproject.toml` & `indonesia_latestearthquake_rx168059-2024.0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [build-system]
 requires = ["setuptools>=70.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "indonesia-latestearthquake_Rx168059"
-version = "2024.0.0.2"
+version = "2024.0.0.3"
 authors = [
   { name="Muhammad Dwi Reza", email="dwireza1002@gmail.com" },
 ]
 description = "This package will get information about latest earthquake from BMKG(Indonesian Agency for Meteorological, Climatological and Geophysics)"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
```

