# Comparing `tmp/indonesia_latestearthquake_rx168059-2024.0.0.1.tar.gz` & `tmp/indonesia_latestearthquake_rx168059-2024.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indonesia_latestearthquake_rx168059-2024.0.0.1.tar", last modified: Mon Jun  3 04:48:51 2024, max compression
+gzip compressed data, was "indonesia_latestearthquake_rx168059-2024.0.0.2.tar", last modified: Mon Jun  3 05:16:30 2024, max compression
```

## Comparing `indonesia_latestearthquake_rx168059-2024.0.0.1.tar` & `indonesia_latestearthquake_rx168059-2024.0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-06-03 04:48:51.585543 indonesia_latestearthquake_rx168059-2024.0.0.1/
--rw-rw-rw-   0        0        0    35823 2024-06-02 11:16:38.000000 indonesia_latestearthquake_rx168059-2024.0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1142 2024-06-03 04:48:51.568336 indonesia_latestearthquake_rx168059-2024.0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      445 2024-06-03 04:45:14.000000 indonesia_latestearthquake_rx168059-2024.0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-06-03 04:48:51.568336 indonesia_latestearthquake_rx168059-2024.0.0.1/gempaTerkini/
--rw-rw-rw-   0        0        0     2715 2024-06-03 03:17:56.000000 indonesia_latestearthquake_rx168059-2024.0.0.1/gempaTerkini/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-03 04:48:51.568336 indonesia_latestearthquake_rx168059-2024.0.0.1/indonesia_latestearthquake_Rx168059.egg-info/
--rw-rw-rw-   0        0        0     1142 2024-06-03 04:48:51.000000 indonesia_latestearthquake_rx168059-2024.0.0.1/indonesia_latestearthquake_Rx168059.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2024-06-03 04:48:51.000000 indonesia_latestearthquake_rx168059-2024.0.0.1/indonesia_latestearthquake_Rx168059.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 04:48:51.000000 indonesia_latestearthquake_rx168059-2024.0.0.1/indonesia_latestearthquake_Rx168059.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-06-03 04:48:51.000000 indonesia_latestearthquake_rx168059-2024.0.0.1/indonesia_latestearthquake_Rx168059.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      974 2024-06-03 04:39:35.000000 indonesia_latestearthquake_rx168059-2024.0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-06-03 04:48:51.585543 indonesia_latestearthquake_rx168059-2024.0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-03 05:16:30.865496 indonesia_latestearthquake_rx168059-2024.0.0.2/
+-rw-rw-rw-   0        0        0    35823 2024-06-02 11:16:38.000000 indonesia_latestearthquake_rx168059-2024.0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1302 2024-06-03 05:16:30.863124 indonesia_latestearthquake_rx168059-2024.0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      605 2024-06-03 05:12:18.000000 indonesia_latestearthquake_rx168059-2024.0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 05:16:30.842462 indonesia_latestearthquake_rx168059-2024.0.0.2/gempaTerkini/
+-rw-rw-rw-   0        0        0     2669 2024-06-03 05:10:00.000000 indonesia_latestearthquake_rx168059-2024.0.0.2/gempaTerkini/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 05:16:30.860727 indonesia_latestearthquake_rx168059-2024.0.0.2/indonesia_latestearthquake_Rx168059.egg-info/
+-rw-rw-rw-   0        0        0     1302 2024-06-03 05:16:30.000000 indonesia_latestearthquake_rx168059-2024.0.0.2/indonesia_latestearthquake_Rx168059.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2024-06-03 05:16:30.000000 indonesia_latestearthquake_rx168059-2024.0.0.2/indonesia_latestearthquake_Rx168059.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 05:16:30.000000 indonesia_latestearthquake_rx168059-2024.0.0.2/indonesia_latestearthquake_Rx168059.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-06-03 05:16:30.000000 indonesia_latestearthquake_rx168059-2024.0.0.2/indonesia_latestearthquake_Rx168059.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      974 2024-06-03 05:02:09.000000 indonesia_latestearthquake_rx168059-2024.0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-03 05:16:30.865496 indonesia_latestearthquake_rx168059-2024.0.0.2/setup.cfg
```

### Comparing `indonesia_latestearthquake_rx168059-2024.0.0.1/LICENSE` & `indonesia_latestearthquake_rx168059-2024.0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `indonesia_latestearthquake_rx168059-2024.0.0.1/PKG-INFO` & `indonesia_latestearthquake_rx168059-2024.0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indonesia-latestearthquake_Rx168059
-Version: 2024.0.0.1
+Version: 2024.0.0.2
 Summary: This package will get information about latest earthquake from BMKG(Indonesian Agency for Meteorological, Climatological and Geophysics)
 Author-email: Muhammad Dwi Reza <dwireza1002@gmail.com>
 Project-URL: Homepage, https://github.com/Rex-Project-Organization/IndonesiaLatestEarthQuake
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
@@ -12,13 +12,22 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # IndonesiaLatestEarthQuake
 This package will get information about latest earthquake from BMKG(Indonesian Agency for Meteorological, Climatological and Geophysics)
 
 ## How It Works
-This package will scrap from [BMKG](https://www.bmkg.go.id/) to get information about latest earthquake on indonesia
+This package will scrap data from [BMKG](https://www.bmkg.go.id/) to get information about latest earthquake on indonesia
 
 This package used BeautifulSoup4 and Requests to generate JSON output that'll be used for web or mobile apps
 
+# How to Run
+"""
+import gempaTerkini
+
+if __name__ == '__main__':
+    result = gempaTerkini.data_extract()
+    gempaTerkini.show_data(result)
+"""
+
 # Author
 Muhammad Dwi Reza
```

### Comparing `indonesia_latestearthquake_rx168059-2024.0.0.1/gempaTerkini/__init__.py` & `indonesia_latestearthquake_rx168059-2024.0.0.2/gempaTerkini/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,12 +90,10 @@
         print(f'kedalaman = {datas['kedalaman']}')
         print(f'location = {datas['location']}')
         print(f'pusat = {datas['pusat']}')
         print(f'keterangan = {datas['keterangan']}')
 
 
 if __name__ == '__main__':
-
-    if __name__ == '__main__':
-        print('Aplikasi utama')
-        result = data_extract()
-        show_data(result)
+    print('Aplikasi utama')
+    result = data_extract()
+    show_data(result)
```

### Comparing `indonesia_latestearthquake_rx168059-2024.0.0.1/indonesia_latestearthquake_Rx168059.egg-info/PKG-INFO` & `indonesia_latestearthquake_rx168059-2024.0.0.2/indonesia_latestearthquake_Rx168059.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indonesia-latestearthquake_Rx168059
-Version: 2024.0.0.1
+Version: 2024.0.0.2
 Summary: This package will get information about latest earthquake from BMKG(Indonesian Agency for Meteorological, Climatological and Geophysics)
 Author-email: Muhammad Dwi Reza <dwireza1002@gmail.com>
 Project-URL: Homepage, https://github.com/Rex-Project-Organization/IndonesiaLatestEarthQuake
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
@@ -12,13 +12,22 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # IndonesiaLatestEarthQuake
 This package will get information about latest earthquake from BMKG(Indonesian Agency for Meteorological, Climatological and Geophysics)
 
 ## How It Works
-This package will scrap from [BMKG](https://www.bmkg.go.id/) to get information about latest earthquake on indonesia
+This package will scrap data from [BMKG](https://www.bmkg.go.id/) to get information about latest earthquake on indonesia
 
 This package used BeautifulSoup4 and Requests to generate JSON output that'll be used for web or mobile apps
 
+# How to Run
+"""
+import gempaTerkini
+
+if __name__ == '__main__':
+    result = gempaTerkini.data_extract()
+    gempaTerkini.show_data(result)
+"""
+
 # Author
 Muhammad Dwi Reza
```

### Comparing `indonesia_latestearthquake_rx168059-2024.0.0.1/pyproject.toml` & `indonesia_latestearthquake_rx168059-2024.0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [build-system]
 requires = ["setuptools>=70.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "indonesia-latestearthquake_Rx168059"
-version = "2024.0.0.1"
+version = "2024.0.0.2"
 authors = [
   { name="Muhammad Dwi Reza", email="dwireza1002@gmail.com" },
 ]
 description = "This package will get information about latest earthquake from BMKG(Indonesian Agency for Meteorological, Climatological and Geophysics)"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
```

