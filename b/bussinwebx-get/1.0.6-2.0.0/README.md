# Comparing `tmp/bussinwebx_get-1.0.6.tar.gz` & `tmp/bussinwebx_get-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bussinwebx_get-1.0.6.tar", last modified: Sun Jun  2 01:02:20 2024, max compression
+gzip compressed data, was "bussinwebx_get-2.0.0.tar", last modified: Sun Jun  2 22:07:45 2024, max compression
```

## Comparing `bussinwebx_get-1.0.6.tar` & `bussinwebx_get-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 01:02:20.705932 bussinwebx_get-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-06-02 01:02:16.000000 bussinwebx_get-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-06-02 01:02:20.701931 bussinwebx_get-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-06-02 01:02:16.000000 bussinwebx_get-1.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-06-02 01:02:16.000000 bussinwebx_get-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 01:02:20.705932 bussinwebx_get-1.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 01:02:20.701931 bussinwebx_get-1.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 01:02:20.701931 bussinwebx_get-1.0.6/src/bussinwebx_get/
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-06-02 01:02:16.000000 bussinwebx_get-1.0.6/src/bussinwebx_get/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 01:02:20.701931 bussinwebx_get-1.0.6/src/bussinwebx_get.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-06-02 01:02:20.000000 bussinwebx_get-1.0.6/src/bussinwebx_get.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-06-02 01:02:20.000000 bussinwebx_get-1.0.6/src/bussinwebx_get.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 01:02:20.000000 bussinwebx_get-1.0.6/src/bussinwebx_get.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-02 01:02:20.000000 bussinwebx_get-1.0.6/src/bussinwebx_get.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:07:45.085153 bussinwebx_get-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-06-02 22:07:40.000000 bussinwebx_get-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-06-02 22:07:45.085153 bussinwebx_get-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-06-02 22:07:40.000000 bussinwebx_get-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-06-02 22:07:40.000000 bussinwebx_get-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 22:07:45.085153 bussinwebx_get-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:07:45.085153 bussinwebx_get-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:07:45.085153 bussinwebx_get-2.0.0/src/bussinwebx_get/
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-06-02 22:07:40.000000 bussinwebx_get-2.0.0/src/bussinwebx_get/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:07:45.085153 bussinwebx_get-2.0.0/src/bussinwebx_get.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-06-02 22:07:45.000000 bussinwebx_get-2.0.0/src/bussinwebx_get.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-06-02 22:07:45.000000 bussinwebx_get-2.0.0/src/bussinwebx_get.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 22:07:45.000000 bussinwebx_get-2.0.0/src/bussinwebx_get.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-02 22:07:45.000000 bussinwebx_get-2.0.0/src/bussinwebx_get.egg-info/top_level.txt
```

### Comparing `bussinwebx_get-1.0.6/LICENSE` & `bussinwebx_get-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bussinwebx_get-1.0.6/PKG-INFO` & `bussinwebx_get-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: bussinwebx_get
-Version: 1.0.6
+Version: 2.0.0
 Summary: Be able to make GET requests to buss:// websites and get IPs for buss:// websites.
 Maintainer: The Odd Cell
 License: MIT License
 Project-URL: Repository, https://github.com/TheOddCell/bussinwebx-get.git
 Project-URL: Issues, https://github.com/TheOddCell/bussinwebx-get/issues
 Keywords: webx,buss,facedev
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # bussinwebx-get
 Be able to make GET requests to buss:// websites and get IPs for buss:// websites.
 
 [What is Bussin Web X (buss://)?](https://github.com/face-hh/webx)
```

### Comparing `bussinwebx_get-1.0.6/pyproject.toml` & `bussinwebx_get-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
-version = "1.0.6"
+version = "2.0.0"
 name = "bussinwebx_get"
-requires-python = ">= 3.8"
+requires-python = ">= 3.7"
 maintainers = [
   {name = "The Odd Cell"}
 ]
 description = "Be able to make GET requests to buss:// websites and get IPs for buss:// websites."
 readme = "README.md"
 license = {text = "MIT License"}
 keywords = ["webx", "buss", "facedev"]
```

### Comparing `bussinwebx_get-1.0.6/src/bussinwebx_get.egg-info/PKG-INFO` & `bussinwebx_get-2.0.0/src/bussinwebx_get.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: bussinwebx_get
-Version: 1.0.6
+Version: 2.0.0
 Summary: Be able to make GET requests to buss:// websites and get IPs for buss:// websites.
 Maintainer: The Odd Cell
 License: MIT License
 Project-URL: Repository, https://github.com/TheOddCell/bussinwebx-get.git
 Project-URL: Issues, https://github.com/TheOddCell/bussinwebx-get/issues
 Keywords: webx,buss,facedev
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # bussinwebx-get
 Be able to make GET requests to buss:// websites and get IPs for buss:// websites.
 
 [What is Bussin Web X (buss://)?](https://github.com/face-hh/webx)
```

