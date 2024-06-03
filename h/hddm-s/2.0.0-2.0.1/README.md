# Comparing `tmp/hddm_s-2.0.0.tar.gz` & `tmp/hddm_s-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hddm_s-2.0.0.tar", last modified: Mon Jun  3 14:13:40 2024, max compression
+gzip compressed data, was "hddm_s-2.0.1.tar", last modified: Mon Jun  3 14:18:17 2024, max compression
```

## Comparing `hddm_s-2.0.0.tar` & `hddm_s-2.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:13:40.859241 hddm_s-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-06-03 14:13:33.000000 hddm_s-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-06-03 14:13:33.000000 hddm_s-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-06-03 14:13:40.859241 hddm_s-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-06-03 14:13:33.000000 hddm_s-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:13:40.859241 hddm_s-2.0.0/hddm_s/
--rw-r--r--   0 runner    (1001) docker     (127)    16558 2024-06-03 14:13:33.000000 hddm_s-2.0.0/hddm_s/event.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:13:40.859241 hddm_s-2.0.0/hddm_s.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-06-03 14:13:40.000000 hddm_s-2.0.0/hddm_s.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-06-03 14:13:40.000000 hddm_s-2.0.0/hddm_s.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 14:13:40.000000 hddm_s-2.0.0/hddm_s.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-03 14:13:40.000000 hddm_s-2.0.0/hddm_s.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-06-03 14:13:33.000000 hddm_s-2.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:13:40.859241 hddm_s-2.0.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-06-03 14:13:33.000000 hddm_s-2.0.0/scripts/install_cmake.bat
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 14:13:40.859241 hddm_s-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-06-03 14:13:33.000000 hddm_s-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:18:17.756699 hddm_s-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-06-03 14:18:13.000000 hddm_s-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-06-03 14:18:13.000000 hddm_s-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-06-03 14:18:17.756699 hddm_s-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-06-03 14:18:13.000000 hddm_s-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:18:17.756699 hddm_s-2.0.1/hddm_s/
+-rw-r--r--   0 runner    (1001) docker     (127)    16558 2024-06-03 14:18:13.000000 hddm_s-2.0.1/hddm_s/event.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:18:17.756699 hddm_s-2.0.1/hddm_s.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-06-03 14:18:17.000000 hddm_s-2.0.1/hddm_s.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-06-03 14:18:17.000000 hddm_s-2.0.1/hddm_s.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 14:18:17.000000 hddm_s-2.0.1/hddm_s.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-03 14:18:17.000000 hddm_s-2.0.1/hddm_s.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-06-03 14:18:13.000000 hddm_s-2.0.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:18:17.756699 hddm_s-2.0.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-06-03 14:18:13.000000 hddm_s-2.0.1/scripts/install_cmake.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 14:18:17.756699 hddm_s-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-06-03 14:18:13.000000 hddm_s-2.0.1/setup.py
```

### Comparing `hddm_s-2.0.0/LICENSE` & `hddm_s-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hddm_s-2.0.0/PKG-INFO` & `hddm_s-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hddm_s
-Version: 2.0.0
+Version: 2.0.1
 Summary: methods for reading and writing GlueX simulated event data
 Home-page: https://github.com/rjones30/hddm_s
 Author: Richard T. Jones
 Author-email: "Richard T. Jones" <richard.t.jones@uconn.edu>
 Maintainer-email: "Richard T. Jones" <richard.t.jones@uconn.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/rjones30/hddm_s
```

### Comparing `hddm_s-2.0.0/README.md` & `hddm_s-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `hddm_s-2.0.0/hddm_s/event.xml` & `hddm_s-2.0.1/hddm_s/event.xml`

 * *Files identical despite different names*

### Comparing `hddm_s-2.0.0/hddm_s.egg-info/PKG-INFO` & `hddm_s-2.0.1/hddm_s.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hddm_s
-Version: 2.0.0
+Version: 2.0.1
 Summary: methods for reading and writing GlueX simulated event data
 Home-page: https://github.com/rjones30/hddm_s
 Author: Richard T. Jones
 Author-email: "Richard T. Jones" <richard.t.jones@uconn.edu>
 Maintainer-email: "Richard T. Jones" <richard.t.jones@uconn.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/rjones30/hddm_s
```

### Comparing `hddm_s-2.0.0/pyproject.toml` & `hddm_s-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 38.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hddm_s"
-version = "2.0.0"
+version = "2.0.1"
 requires-python = ">= 3.6"
 authors = [
   {name = "Richard T. Jones", email = "richard.t.jones@uconn.edu"},
 ]
 maintainers = [
   {name = "Richard T. Jones", email = "richard.t.jones@uconn.edu"},
 ]
```

### Comparing `hddm_s-2.0.0/setup.py` & `hddm_s-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
   "bzip2.tag": "",
   "xerces-c.url": "https://github.com/rjones30/xerces-c.git",
   "xerces-c.tag": "",
   "hdf5.url": "https://github.com/HDFGroup/hdf5.git",
   "hdf5.tag": "tags/hdf5-1_10_8",
   "pthread-win32.url": "https://github.com/GerHobbelt/pthread-win32.git",
   "pthread-win32.tag": "version-3.1.0-release",
-  "cpr.url": "https://github.com/cpr.git",
+  "cpr.url": "https://github.com/rjones30/cpr.git",
   "cpr.tag": "",
   "xrootd.url": "https://github.com/rjones30/xrootd.git",
   "xrootd.tag": "stable-4.12-for-hddm",
   "HDDM.url": "https://github.com/rjones30/HDDM.git",
   "HDDM.tag": "streaming_input",
 }
 
@@ -170,15 +170,15 @@
                            "bz2_static",
                            "z_static",
                            "xerces-c",
                            "pthread",
                           ]
 setuptools.setup(
     name = "hddm_s",
-    version = "2.0.0",
+    version = "2.0.1",
     url = "https://github.com/rjones30/hddm_s",
     author = "Richard T. Jones",
     description = "i/o module for GlueX simulated events",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     packages = templates.keys(),
     package_data = templates,
```

