# Comparing `tmp/hddm_r-2.0.0.tar.gz` & `tmp/hddm_r-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hddm_r-2.0.0.tar", last modified: Mon Jun  3 13:51:11 2024, max compression
+gzip compressed data, was "hddm_r-2.0.1.tar", last modified: Mon Jun  3 14:06:20 2024, max compression
```

## Comparing `hddm_r-2.0.0.tar` & `hddm_r-2.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:11.379332 hddm_r-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-06-03 13:51:01.000000 hddm_r-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-06-03 13:51:01.000000 hddm_r-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-06-03 13:51:11.379332 hddm_r-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-06-03 13:51:01.000000 hddm_r-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:11.379332 hddm_r-2.0.0/hddm_r/
--rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-06-03 13:51:01.000000 hddm_r-2.0.0/hddm_r/rest.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:11.379332 hddm_r-2.0.0/hddm_r.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-06-03 13:51:11.000000 hddm_r-2.0.0/hddm_r.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-06-03 13:51:11.000000 hddm_r-2.0.0/hddm_r.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 13:51:11.000000 hddm_r-2.0.0/hddm_r.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-06-03 13:51:11.000000 hddm_r-2.0.0/hddm_r.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-06-03 13:51:01.000000 hddm_r-2.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:11.379332 hddm_r-2.0.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-06-03 13:51:01.000000 hddm_r-2.0.0/scripts/install_cmake.bat
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 13:51:11.379332 hddm_r-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8345 2024-06-03 13:51:01.000000 hddm_r-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:06:20.586717 hddm_r-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-06-03 14:06:13.000000 hddm_r-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-06-03 14:06:13.000000 hddm_r-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-06-03 14:06:20.586717 hddm_r-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-06-03 14:06:13.000000 hddm_r-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:06:20.582717 hddm_r-2.0.1/hddm_r/
+-rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-06-03 14:06:13.000000 hddm_r-2.0.1/hddm_r/rest.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:06:20.586717 hddm_r-2.0.1/hddm_r.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-06-03 14:06:20.000000 hddm_r-2.0.1/hddm_r.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-06-03 14:06:20.000000 hddm_r-2.0.1/hddm_r.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 14:06:20.000000 hddm_r-2.0.1/hddm_r.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-03 14:06:20.000000 hddm_r-2.0.1/hddm_r.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-06-03 14:06:13.000000 hddm_r-2.0.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:06:20.586717 hddm_r-2.0.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-06-03 14:06:13.000000 hddm_r-2.0.1/scripts/install_cmake.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 14:06:20.586717 hddm_r-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8373 2024-06-03 14:06:13.000000 hddm_r-2.0.1/setup.py
```

### Comparing `hddm_r-2.0.0/LICENSE` & `hddm_r-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hddm_r-2.0.0/PKG-INFO` & `hddm_r-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hddm_r
-Version: 2.0.0
+Version: 2.0.1
 Summary: methods for reading and writing GlueX reconstructed event data
 Home-page: https://github.com/rjones30/hddm_r
 Author: Richard T. Jones
 Author-email: "Richard T. Jones" <richard.t.jones@uconn.edu>
 Maintainer-email: "Richard T. Jones" <richard.t.jones@uconn.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/rjones30/hddm_r
```

### Comparing `hddm_r-2.0.0/README.md` & `hddm_r-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `hddm_r-2.0.0/hddm_r/rest.xml` & `hddm_r-2.0.1/hddm_r/rest.xml`

 * *Files identical despite different names*

### Comparing `hddm_r-2.0.0/hddm_r.egg-info/PKG-INFO` & `hddm_r-2.0.1/hddm_r.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hddm_r
-Version: 2.0.0
+Version: 2.0.1
 Summary: methods for reading and writing GlueX reconstructed event data
 Home-page: https://github.com/rjones30/hddm_r
 Author: Richard T. Jones
 Author-email: "Richard T. Jones" <richard.t.jones@uconn.edu>
 Maintainer-email: "Richard T. Jones" <richard.t.jones@uconn.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/rjones30/hddm_r
```

### Comparing `hddm_r-2.0.0/pyproject.toml` & `hddm_r-2.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 38.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hddm_r"
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

### Comparing `hddm_r-2.0.0/setup.py` & `hddm_r-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,15 +170,15 @@
                            "bz2_static",
                            "z_static",
                            "xerces-c",
                            "pthread",
                           ]
 setuptools.setup(
     name = "hddm_r",
-    version = "2.0.0",
+    version = "2.0.1",
     url = "https://github.com/rjones30/hddm_r",
     author = "Richard T. Jones",
     description = "i/o module for GlueX reconstructed events",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     packages = templates.keys(),
     package_data = templates,
@@ -194,16 +194,17 @@
     #  "xrootd",
     #],
     ext_modules = [
       CMakeExtension("zlib"),
       CMakeExtension("bzip2"),
       CMakeExtension("xerces-c"),
       CMakeExtension("hdf5"),
-      #CMakeExtension("xrootd"),
       CMakeExtension("pthread-win32"),
+      CMakeExtension("cpr"),
+      CMakeExtension("xrootd"),
       CMakeExtension("HDDM"),
       setuptools.Extension("hddm_r",
            include_dirs = extension_include_dirs,
            library_dirs = extension_library_dirs,
            libraries = extension_libraries,
            extra_compile_args = ["-std=c++11", "-DHDF5_SUPPORT"],
            sources = ["hddm_r/hddm_r++.cpp", "hddm_r/pyhddm_r.cpp"]),
```

