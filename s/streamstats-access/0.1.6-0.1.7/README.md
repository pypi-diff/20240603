# Comparing `tmp/streamstats_access-0.1.6.tar.gz` & `tmp/streamstats_access-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamstats_access-0.1.6.tar", last modified: Mon Jun  3 13:47:54 2024, max compression
+gzip compressed data, was "streamstats_access-0.1.7.tar", last modified: Mon Jun  3 14:01:25 2024, max compression
```

## Comparing `streamstats_access-0.1.6.tar` & `streamstats_access-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-06-03 13:47:54.963910 streamstats_access-0.1.6/
--rw-rw-rw-   0        0        0     1096 2024-06-02 19:52:29.000000 streamstats_access-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     4431 2024-06-03 13:47:54.962911 streamstats_access-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     2167 2024-06-03 11:58:04.000000 streamstats_access-0.1.6/README.md
--rw-rw-rw-   0        0        0     1355 2024-06-03 13:47:28.000000 streamstats_access-0.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-06-03 13:47:54.963910 streamstats_access-0.1.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-06-03 13:47:54.933917 streamstats_access-0.1.6/streamstats_access/
--rw-rw-rw-   0        0        0      736 2024-06-02 19:08:30.000000 streamstats_access-0.1.6/streamstats_access/__init__.py
--rw-rw-rw-   0        0        0     2306 2024-06-02 18:15:59.000000 streamstats_access-0.1.6/streamstats_access/api_client.py
--rw-rw-rw-   0        0        0     5048 2024-06-02 19:54:10.000000 streamstats_access-0.1.6/streamstats_access/batch_query.py
--rw-rw-rw-   0        0        0      526 2024-06-02 18:15:59.000000 streamstats_access-0.1.6/streamstats_access/config.py
--rw-rw-rw-   0        0        0     4671 2024-06-02 18:15:59.000000 streamstats_access-0.1.6/streamstats_access/endpoints.py
--rw-rw-rw-   0        0        0     8001 2024-06-02 18:15:59.000000 streamstats_access-0.1.6/streamstats_access/models.py
--rw-rw-rw-   0        0        0     2537 2024-06-02 19:14:28.000000 streamstats_access-0.1.6/streamstats_access/utils.py
-drwxrwxrwx   0        0        0        0 2024-06-03 13:47:54.961908 streamstats_access-0.1.6/streamstats_access.egg-info/
--rw-rw-rw-   0        0        0     4431 2024-06-03 13:47:54.000000 streamstats_access-0.1.6/streamstats_access.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      416 2024-06-03 13:47:54.000000 streamstats_access-0.1.6/streamstats_access.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 13:47:54.000000 streamstats_access-0.1.6/streamstats_access.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-06-03 13:47:54.000000 streamstats_access-0.1.6/streamstats_access.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-03 14:01:25.315818 streamstats_access-0.1.7/
+-rw-rw-rw-   0        0        0     1096 2024-06-02 19:52:29.000000 streamstats_access-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     4622 2024-06-03 14:01:25.313804 streamstats_access-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2167 2024-06-03 11:58:04.000000 streamstats_access-0.1.7/README.md
+-rw-rw-rw-   0        0        0     1364 2024-06-03 14:01:19.000000 streamstats_access-0.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-03 14:01:25.315818 streamstats_access-0.1.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-03 14:01:25.276444 streamstats_access-0.1.7/streamstats_access/
+-rw-rw-rw-   0        0        0      736 2024-06-02 19:08:30.000000 streamstats_access-0.1.7/streamstats_access/__init__.py
+-rw-rw-rw-   0        0        0     2306 2024-06-02 18:15:59.000000 streamstats_access-0.1.7/streamstats_access/api_client.py
+-rw-rw-rw-   0        0        0     5048 2024-06-02 19:54:10.000000 streamstats_access-0.1.7/streamstats_access/batch_query.py
+-rw-rw-rw-   0        0        0      526 2024-06-02 18:15:59.000000 streamstats_access-0.1.7/streamstats_access/config.py
+-rw-rw-rw-   0        0        0     4671 2024-06-02 18:15:59.000000 streamstats_access-0.1.7/streamstats_access/endpoints.py
+-rw-rw-rw-   0        0        0     8001 2024-06-02 18:15:59.000000 streamstats_access-0.1.7/streamstats_access/models.py
+-rw-rw-rw-   0        0        0     2537 2024-06-02 19:14:28.000000 streamstats_access-0.1.7/streamstats_access/utils.py
+drwxrwxrwx   0        0        0        0 2024-06-03 14:01:25.312598 streamstats_access-0.1.7/streamstats_access.egg-info/
+-rw-rw-rw-   0        0        0     4622 2024-06-03 14:01:25.000000 streamstats_access-0.1.7/streamstats_access.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2024-06-03 14:01:25.000000 streamstats_access-0.1.7/streamstats_access.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 14:01:25.000000 streamstats_access-0.1.7/streamstats_access.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-06-03 14:01:25.000000 streamstats_access-0.1.7/streamstats_access.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-06-03 14:01:25.000000 streamstats_access-0.1.7/streamstats_access.egg-info/top_level.txt
```

### Comparing `streamstats_access-0.1.6/LICENSE` & `streamstats_access-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `streamstats_access-0.1.6/PKG-INFO` & `streamstats_access-0.1.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamstats_access
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python package to access and process data from the USGS StreamStats API.
 Author-email: Scott Lawson <scott.lawson@uvm.edu>
 License: MIT License
         
         Copyright (c) 2024 streamstats_access
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -35,14 +35,20 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: GIS
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiohttp>=3.8.1
+Requires-Dist: geopandas>=0.9.0
+Requires-Dist: pandas>=1.3.0
+Provides-Extra: dev
+Requires-Dist: twine; extra == "dev"
+Requires-Dist: build; extra == "dev"
 
 # streamstats_access: Python access to the USGS Streamstats API
 <p align=center>
 <img src="images/logo_nobg_txt.png" alt="StreamStats API Python library" width="350">
 </p>
 
 ## Overview
```

### Comparing `streamstats_access-0.1.6/README.md` & `streamstats_access-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `streamstats_access-0.1.6/pyproject.toml` & `streamstats_access-0.1.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "streamstats_access"
-version = "0.1.6"
+version = "0.1.7"
 description = "A Python package to access and process data from the USGS StreamStats API."
 authors = [
     { name="Scott Lawson", email="scott.lawson@uvm.edu" }
 ]
 license = { file="LICENSE" }
 readme = "README.md"
 keywords = ["USGS", "StreamStats", "API", "Geospatial", "Hydrology", "statistics", "watershed characteristics", "water resources", "data retrieval"]
@@ -19,29 +19,28 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Scientific/Engineering :: GIS",
 ]
+dependencies = [
+    "aiohttp >= 3.8.1",
+    "geopandas >= 0.9.0",
+    "pandas >= 1.3.0",
+]
 
 [project.urls]
 "Homepage" = "https://github.com/sclaw/streamstats_access"
 "Bug Tracker" = "https://github.com/sclaw/streamstats_access/issues"
 
-[dependencies]
-aiohttp = "^3.8.1"
-geopandas = "^0.9.0"
-pandas = "^1.3.0"
-
-[optional-dependencies]
+[project.optional-dependencies]
 dev = [
-    "black",
-    "flake8",
-    "pytest",
+    "twine",
+    "build"
 ]
 
 [tool.setuptools]
 packages = ["streamstats_access"]
 
 [tool.black]
 line-length = 88
```

### Comparing `streamstats_access-0.1.6/streamstats_access/__init__.py` & `streamstats_access-0.1.7/streamstats_access/__init__.py`

 * *Files identical despite different names*

### Comparing `streamstats_access-0.1.6/streamstats_access/api_client.py` & `streamstats_access-0.1.7/streamstats_access/api_client.py`

 * *Files identical despite different names*

### Comparing `streamstats_access-0.1.6/streamstats_access/batch_query.py` & `streamstats_access-0.1.7/streamstats_access/batch_query.py`

 * *Files identical despite different names*

### Comparing `streamstats_access-0.1.6/streamstats_access/config.py` & `streamstats_access-0.1.7/streamstats_access/config.py`

 * *Files identical despite different names*

### Comparing `streamstats_access-0.1.6/streamstats_access/endpoints.py` & `streamstats_access-0.1.7/streamstats_access/endpoints.py`

 * *Files identical despite different names*

### Comparing `streamstats_access-0.1.6/streamstats_access/models.py` & `streamstats_access-0.1.7/streamstats_access/models.py`

 * *Files identical despite different names*

### Comparing `streamstats_access-0.1.6/streamstats_access/utils.py` & `streamstats_access-0.1.7/streamstats_access/utils.py`

 * *Files identical despite different names*

### Comparing `streamstats_access-0.1.6/streamstats_access.egg-info/PKG-INFO` & `streamstats_access-0.1.7/streamstats_access.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamstats_access
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python package to access and process data from the USGS StreamStats API.
 Author-email: Scott Lawson <scott.lawson@uvm.edu>
 License: MIT License
         
         Copyright (c) 2024 streamstats_access
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -35,14 +35,20 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: GIS
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiohttp>=3.8.1
+Requires-Dist: geopandas>=0.9.0
+Requires-Dist: pandas>=1.3.0
+Provides-Extra: dev
+Requires-Dist: twine; extra == "dev"
+Requires-Dist: build; extra == "dev"
 
 # streamstats_access: Python access to the USGS Streamstats API
 <p align=center>
 <img src="images/logo_nobg_txt.png" alt="StreamStats API Python library" width="350">
 </p>
 
 ## Overview
```

