# Comparing `tmp/hddm_s-1.1.5.tar.gz` & `tmp/hddm_s-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hddm_s-1.1.5.tar", last modified: Mon Jun  3 10:21:32 2024, max compression
+gzip compressed data, was "hddm_s-1.1.6.tar", last modified: Mon Jun  3 10:55:46 2024, max compression
```

## Comparing `hddm_s-1.1.5.tar` & `hddm_s-1.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:21:32.816021 hddm_s-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-06-03 10:21:28.000000 hddm_s-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-06-03 10:21:28.000000 hddm_s-1.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-06-03 10:21:32.816021 hddm_s-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-06-03 10:21:28.000000 hddm_s-1.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:21:32.816021 hddm_s-1.1.5/hddm_s/
--rw-r--r--   0 runner    (1001) docker     (127)    16558 2024-06-03 10:21:28.000000 hddm_s-1.1.5/hddm_s/event.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:21:32.816021 hddm_s-1.1.5/hddm_s.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-06-03 10:21:32.000000 hddm_s-1.1.5/hddm_s.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-06-03 10:21:32.000000 hddm_s-1.1.5/hddm_s.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 10:21:32.000000 hddm_s-1.1.5/hddm_s.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-06-03 10:21:32.000000 hddm_s-1.1.5/hddm_s.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-06-03 10:21:28.000000 hddm_s-1.1.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:21:32.816021 hddm_s-1.1.5/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-06-03 10:21:28.000000 hddm_s-1.1.5/scripts/install_cmake.bat
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 10:21:32.816021 hddm_s-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8327 2024-06-03 10:21:28.000000 hddm_s-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:55:46.902834 hddm_s-1.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-06-03 10:55:41.000000 hddm_s-1.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-06-03 10:55:41.000000 hddm_s-1.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-06-03 10:55:46.902834 hddm_s-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-06-03 10:55:41.000000 hddm_s-1.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:55:46.902834 hddm_s-1.1.6/hddm_s/
+-rw-r--r--   0 runner    (1001) docker     (127)    16558 2024-06-03 10:55:41.000000 hddm_s-1.1.6/hddm_s/event.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:55:46.902834 hddm_s-1.1.6/hddm_s.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-06-03 10:55:46.000000 hddm_s-1.1.6/hddm_s.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-06-03 10:55:46.000000 hddm_s-1.1.6/hddm_s.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 10:55:46.000000 hddm_s-1.1.6/hddm_s.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-06-03 10:55:46.000000 hddm_s-1.1.6/hddm_s.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-06-03 10:55:41.000000 hddm_s-1.1.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:55:46.902834 hddm_s-1.1.6/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-06-03 10:55:41.000000 hddm_s-1.1.6/scripts/install_cmake.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 10:55:46.902834 hddm_s-1.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8327 2024-06-03 10:55:41.000000 hddm_s-1.1.6/setup.py
```

### Comparing `hddm_s-1.1.5/LICENSE` & `hddm_s-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hddm_s-1.1.5/PKG-INFO` & `hddm_s-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hddm_s
-Version: 1.1.5
+Version: 1.1.6
 Summary: methods for reading and writing GlueX simulated event data
 Home-page: https://github.com/rjones30/hddm_s
 Author: Richard T. Jones
 Author-email: "Richard T. Jones" <richard.t.jones@uconn.edu>
 Maintainer-email: "Richard T. Jones" <richard.t.jones@uconn.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/rjones30/hddm_s
```

### Comparing `hddm_s-1.1.5/README.md` & `hddm_s-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `hddm_s-1.1.5/hddm_s/event.xml` & `hddm_s-1.1.6/hddm_s/event.xml`

 * *Files identical despite different names*

### Comparing `hddm_s-1.1.5/hddm_s.egg-info/PKG-INFO` & `hddm_s-1.1.6/hddm_s.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hddm_s
-Version: 1.1.5
+Version: 1.1.6
 Summary: methods for reading and writing GlueX simulated event data
 Home-page: https://github.com/rjones30/hddm_s
 Author: Richard T. Jones
 Author-email: "Richard T. Jones" <richard.t.jones@uconn.edu>
 Maintainer-email: "Richard T. Jones" <richard.t.jones@uconn.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/rjones30/hddm_s
```

### Comparing `hddm_s-1.1.5/pyproject.toml` & `hddm_s-1.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 38.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hddm_s"
-version = "1.1.5"
+version = "1.1.6"
 requires-python = ">= 3.6"
 authors = [
   {name = "Richard T. Jones", email = "richard.t.jones@uconn.edu"},
 ]
 maintainers = [
   {name = "Richard T. Jones", email = "richard.t.jones@uconn.edu"},
 ]
```

### Comparing `hddm_s-1.1.5/setup.py` & `hddm_s-1.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,15 @@
                            "bz2_static",
                            "z_static",
                            "xerces-c",
                            "pthread",
                           ]
 setuptools.setup(
     name = "hddm_s",
-    version = "1.1.5",
+    version = "1.1.6",
     url = "https://github.com/rjones30/hddm_s",
     author = "Richard T. Jones",
     description = "i/o module for GlueX simulated events",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     packages = templates.keys(),
     package_data = templates,
```

