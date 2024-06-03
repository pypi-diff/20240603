# Comparing `tmp/streamstats_access-0.1.4.tar.gz` & `tmp/streamstats_access-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamstats_access-0.1.4.tar", last modified: Mon Jun  3 13:09:49 2024, max compression
+gzip compressed data, was "streamstats_access-0.1.5.tar", last modified: Mon Jun  3 13:35:40 2024, max compression
```

## Comparing `streamstats_access-0.1.4.tar` & `streamstats_access-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-06-03 13:09:49.411061 streamstats_access-0.1.4/
--rw-rw-rw-   0        0        0     1096 2024-06-02 19:52:29.000000 streamstats_access-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     4431 2024-06-03 13:09:49.408048 streamstats_access-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2167 2024-06-03 11:58:04.000000 streamstats_access-0.1.4/README.md
--rw-rw-rw-   0        0        0     1370 2024-06-03 13:09:35.000000 streamstats_access-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-06-03 13:09:49.411061 streamstats_access-0.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-06-03 13:09:49.370707 streamstats_access-0.1.4/streamstats_access/
-drwxrwxrwx   0        0        0        0 2024-06-03 13:09:49.406536 streamstats_access-0.1.4/streamstats_access/streamstats_access.egg-info/
--rw-rw-rw-   0        0        0     4431 2024-06-03 13:09:49.000000 streamstats_access-0.1.4/streamstats_access/streamstats_access.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2024-06-03 13:09:49.000000 streamstats_access-0.1.4/streamstats_access/streamstats_access.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 13:09:49.000000 streamstats_access-0.1.4/streamstats_access/streamstats_access.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 13:09:49.000000 streamstats_access-0.1.4/streamstats_access/streamstats_access.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-03 13:35:40.608171 streamstats_access-0.1.5/
+-rw-rw-rw-   0        0        0     1096 2024-06-02 19:52:29.000000 streamstats_access-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     4431 2024-06-03 13:35:40.607170 streamstats_access-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2167 2024-06-03 11:58:04.000000 streamstats_access-0.1.5/README.md
+-rw-rw-rw-   0        0        0     1361 2024-06-03 13:34:25.000000 streamstats_access-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-03 13:35:40.609172 streamstats_access-0.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-03 13:35:40.578958 streamstats_access-0.1.5/testscott/
+drwxrwxrwx   0        0        0        0 2024-06-03 13:35:40.606173 streamstats_access-0.1.5/testscott/streamstats_access.egg-info/
+-rw-rw-rw-   0        0        0     4431 2024-06-03 13:35:40.000000 streamstats_access-0.1.5/testscott/streamstats_access.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2024-06-03 13:35:40.000000 streamstats_access-0.1.5/testscott/streamstats_access.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 13:35:40.000000 streamstats_access-0.1.5/testscott/streamstats_access.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 13:35:40.000000 streamstats_access-0.1.5/testscott/streamstats_access.egg-info/top_level.txt
```

### Comparing `streamstats_access-0.1.4/LICENSE` & `streamstats_access-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `streamstats_access-0.1.4/PKG-INFO` & `streamstats_access-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamstats_access
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python package to access and process data from the USGS StreamStats API.
 Author-email: Scott Lawson <scott.lawson@uvm.edu>
 License: MIT License
         
         Copyright (c) 2024 streamstats_access
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `streamstats_access-0.1.4/README.md` & `streamstats_access-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `streamstats_access-0.1.4/pyproject.toml` & `streamstats_access-0.1.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "streamstats_access"
-version = "0.1.4"
+version = "0.1.5"
 description = "A Python package to access and process data from the USGS StreamStats API."
 authors = [
     { name="Scott Lawson", email="scott.lawson@uvm.edu" }
 ]
 license = { file="LICENSE" }
 readme = "README.md"
 keywords = ["USGS", "StreamStats", "API", "Geospatial", "Hydrology", "statistics", "watershed characteristics", "water resources", "data retrieval"]
@@ -37,11 +37,11 @@
 dev = [
     "black",
     "flake8",
     "pytest",
 ]
 
 [tool.setuptools.packages]
-find = {where = ["streamstats_access"]}
+find = {where = ["testscott"]}
 
 [tool.black]
 line-length = 88
```

### Comparing `streamstats_access-0.1.4/streamstats_access/streamstats_access.egg-info/PKG-INFO` & `streamstats_access-0.1.5/testscott/streamstats_access.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamstats_access
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python package to access and process data from the USGS StreamStats API.
 Author-email: Scott Lawson <scott.lawson@uvm.edu>
 License: MIT License
         
         Copyright (c) 2024 streamstats_access
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

