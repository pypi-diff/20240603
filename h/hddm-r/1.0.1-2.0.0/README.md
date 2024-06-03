# Comparing `tmp/hddm_r-1.0.1.tar.gz` & `tmp/hddm_r-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hddm_r-1.0.1.tar", last modified: Mon Jun  3 13:36:53 2024, max compression
+gzip compressed data, was "hddm_r-2.0.0.tar", last modified: Mon Jun  3 13:51:11 2024, max compression
```

## Comparing `hddm_r-1.0.1.tar` & `hddm_r-2.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:36:53.329321 hddm_r-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-06-03 13:36:44.000000 hddm_r-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-06-03 13:36:44.000000 hddm_r-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-06-03 13:36:53.329321 hddm_r-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-06-03 13:36:44.000000 hddm_r-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:36:53.329321 hddm_r-1.0.1/hddm_r/
--rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-06-03 13:36:44.000000 hddm_r-1.0.1/hddm_r/rest.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:36:53.329321 hddm_r-1.0.1/hddm_r.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-06-03 13:36:53.000000 hddm_r-1.0.1/hddm_r.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-06-03 13:36:53.000000 hddm_r-1.0.1/hddm_r.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 13:36:53.000000 hddm_r-1.0.1/hddm_r.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-06-03 13:36:53.000000 hddm_r-1.0.1/hddm_r.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-06-03 13:36:44.000000 hddm_r-1.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:36:53.329321 hddm_r-1.0.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-06-03 13:36:44.000000 hddm_r-1.0.1/scripts/install_cmake.bat
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 13:36:53.329321 hddm_r-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8330 2024-06-03 13:36:44.000000 hddm_r-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:11.379332 hddm_r-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-06-03 13:51:01.000000 hddm_r-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-06-03 13:51:01.000000 hddm_r-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-06-03 13:51:11.379332 hddm_r-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-06-03 13:51:01.000000 hddm_r-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:11.379332 hddm_r-2.0.0/hddm_r/
+-rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-06-03 13:51:01.000000 hddm_r-2.0.0/hddm_r/rest.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:11.379332 hddm_r-2.0.0/hddm_r.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-06-03 13:51:11.000000 hddm_r-2.0.0/hddm_r.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-06-03 13:51:11.000000 hddm_r-2.0.0/hddm_r.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 13:51:11.000000 hddm_r-2.0.0/hddm_r.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-06-03 13:51:11.000000 hddm_r-2.0.0/hddm_r.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-06-03 13:51:01.000000 hddm_r-2.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:11.379332 hddm_r-2.0.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-06-03 13:51:01.000000 hddm_r-2.0.0/scripts/install_cmake.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 13:51:11.379332 hddm_r-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8345 2024-06-03 13:51:01.000000 hddm_r-2.0.0/setup.py
```

### Comparing `hddm_r-1.0.1/LICENSE` & `hddm_r-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hddm_r-1.0.1/PKG-INFO` & `hddm_r-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hddm_r
-Version: 1.0.1
+Version: 2.0.0
 Summary: methods for reading and writing GlueX reconstructed event data
 Home-page: https://github.com/rjones30/hddm_r
 Author: Richard T. Jones
 Author-email: "Richard T. Jones" <richard.t.jones@uconn.edu>
 Maintainer-email: "Richard T. Jones" <richard.t.jones@uconn.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/rjones30/hddm_r
```

### Comparing `hddm_r-1.0.1/README.md` & `hddm_r-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `hddm_r-1.0.1/hddm_r/rest.xml` & `hddm_r-2.0.0/hddm_r/rest.xml`

 * *Files identical despite different names*

### Comparing `hddm_r-1.0.1/hddm_r.egg-info/PKG-INFO` & `hddm_r-2.0.0/hddm_r.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hddm_r
-Version: 1.0.1
+Version: 2.0.0
 Summary: methods for reading and writing GlueX reconstructed event data
 Home-page: https://github.com/rjones30/hddm_r
 Author: Richard T. Jones
 Author-email: "Richard T. Jones" <richard.t.jones@uconn.edu>
 Maintainer-email: "Richard T. Jones" <richard.t.jones@uconn.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/rjones30/hddm_r
```

### Comparing `hddm_r-1.0.1/pyproject.toml` & `hddm_r-2.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 38.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hddm_r"
-version = "1.0.1"
+version = "2.0.0"
 requires-python = ">= 3.6"
 authors = [
   {name = "Richard T. Jones", email = "richard.t.jones@uconn.edu"},
 ]
 maintainers = [
   {name = "Richard T. Jones", email = "richard.t.jones@uconn.edu"},
 ]
```

### Comparing `hddm_r-1.0.1/setup.py` & `hddm_r-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   "pthread-win32.url": "https://github.com/GerHobbelt/pthread-win32.git",
   "pthread-win32.tag": "version-3.1.0-release",
   "cpr.url": "https://github.com/cpr.git",
   "cpr.tag": "",
   "xrootd.url": "https://github.com/rjones30/xrootd.git",
   "xrootd.tag": "stable-4.12-for-hddm",
   "HDDM.url": "https://github.com/rjones30/HDDM.git",
-  "HDDM.tag": "",
+  "HDDM.tag": "streaming_input",
 }
 
 class CMakeExtension(setuptools.Extension):
 
     def __init__(self, name):
         super().__init__(name, sources=[])
 
@@ -170,15 +170,15 @@
                            "bz2_static",
                            "z_static",
                            "xerces-c",
                            "pthread",
                           ]
 setuptools.setup(
     name = "hddm_r",
-    version = "1.0.1",
+    version = "2.0.0",
     url = "https://github.com/rjones30/hddm_r",
     author = "Richard T. Jones",
     description = "i/o module for GlueX reconstructed events",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     packages = templates.keys(),
     package_data = templates,
```

