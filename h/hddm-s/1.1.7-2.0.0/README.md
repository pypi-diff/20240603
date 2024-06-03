# Comparing `tmp/hddm_s-1.1.7.tar.gz` & `tmp/hddm_s-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hddm_s-1.1.7.tar", last modified: Mon Jun  3 12:06:40 2024, max compression
+gzip compressed data, was "hddm_s-2.0.0.tar", last modified: Mon Jun  3 14:13:40 2024, max compression
```

## Comparing `hddm_s-1.1.7.tar` & `hddm_s-2.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:06:40.892019 hddm_s-1.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-06-03 12:06:36.000000 hddm_s-1.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-06-03 12:06:36.000000 hddm_s-1.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-06-03 12:06:40.892019 hddm_s-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-06-03 12:06:36.000000 hddm_s-1.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:06:40.892019 hddm_s-1.1.7/hddm_s/
--rw-r--r--   0 runner    (1001) docker     (127)    16558 2024-06-03 12:06:36.000000 hddm_s-1.1.7/hddm_s/event.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:06:40.892019 hddm_s-1.1.7/hddm_s.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-06-03 12:06:40.000000 hddm_s-1.1.7/hddm_s.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-06-03 12:06:40.000000 hddm_s-1.1.7/hddm_s.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 12:06:40.000000 hddm_s-1.1.7/hddm_s.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-06-03 12:06:40.000000 hddm_s-1.1.7/hddm_s.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-06-03 12:06:36.000000 hddm_s-1.1.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:06:40.892019 hddm_s-1.1.7/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-06-03 12:06:36.000000 hddm_s-1.1.7/scripts/install_cmake.bat
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 12:06:40.892019 hddm_s-1.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8327 2024-06-03 12:06:36.000000 hddm_s-1.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:13:40.859241 hddm_s-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-06-03 14:13:33.000000 hddm_s-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-06-03 14:13:33.000000 hddm_s-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-06-03 14:13:40.859241 hddm_s-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-06-03 14:13:33.000000 hddm_s-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:13:40.859241 hddm_s-2.0.0/hddm_s/
+-rw-r--r--   0 runner    (1001) docker     (127)    16558 2024-06-03 14:13:33.000000 hddm_s-2.0.0/hddm_s/event.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:13:40.859241 hddm_s-2.0.0/hddm_s.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-06-03 14:13:40.000000 hddm_s-2.0.0/hddm_s.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-06-03 14:13:40.000000 hddm_s-2.0.0/hddm_s.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 14:13:40.000000 hddm_s-2.0.0/hddm_s.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-03 14:13:40.000000 hddm_s-2.0.0/hddm_s.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-06-03 14:13:33.000000 hddm_s-2.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:13:40.859241 hddm_s-2.0.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-06-03 14:13:33.000000 hddm_s-2.0.0/scripts/install_cmake.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 14:13:40.859241 hddm_s-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-06-03 14:13:33.000000 hddm_s-2.0.0/setup.py
```

### Comparing `hddm_s-1.1.7/LICENSE` & `hddm_s-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hddm_s-1.1.7/hddm_s/event.xml` & `hddm_s-2.0.0/hddm_s/event.xml`

 * *Files identical despite different names*

### Comparing `hddm_s-1.1.7/pyproject.toml` & `hddm_s-2.0.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 38.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hddm_s"
-version = "1.1.7"
+version = "2.0.0"
 requires-python = ">= 3.6"
 authors = [
   {name = "Richard T. Jones", email = "richard.t.jones@uconn.edu"},
 ]
 maintainers = [
   {name = "Richard T. Jones", email = "richard.t.jones@uconn.edu"},
 ]
```

### Comparing `hddm_s-1.1.7/setup.py` & `hddm_s-2.0.0/setup.py`

 * *Files 2% similar despite different names*

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
     name = "hddm_s",
-    version = "1.1.7",
+    version = "2.0.0",
     url = "https://github.com/rjones30/hddm_s",
     author = "Richard T. Jones",
     description = "i/o module for GlueX simulated events",
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
       setuptools.Extension("hddm_s",
            include_dirs = extension_include_dirs,
            library_dirs = extension_library_dirs,
            libraries = extension_libraries,
            extra_compile_args = ["-std=c++11", "-DHDF5_SUPPORT"],
            sources = ["hddm_s/hddm_s++.cpp", "hddm_s/pyhddm_s.cpp"]),
```

