# Comparing `tmp/socketbee-0.1.3.tar.gz` & `tmp/socketbee-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketbee-0.1.3.tar", last modified: Sun Jun  2 22:13:50 2024, max compression
+gzip compressed data, was "socketbee-0.1.4.tar", last modified: Sun Jun  2 22:15:15 2024, max compression
```

## Comparing `socketbee-0.1.3.tar` & `socketbee-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 boulamakandine   (501) staff       (20)        0 2024-06-02 22:13:50.857331 socketbee-0.1.3/
--rw-r--r--   0 boulamakandine   (501) staff       (20)     1053 2024-05-13 04:59:24.000000 socketbee-0.1.3/LICENSE.md
--rw-r--r--   0 boulamakandine   (501) staff       (20)     3360 2024-06-02 22:13:50.857138 socketbee-0.1.3/PKG-INFO
--rw-r--r--   0 boulamakandine   (501) staff       (20)     2766 2024-06-02 22:13:44.000000 socketbee-0.1.3/README.md
--rw-r--r--   0 boulamakandine   (501) staff       (20)      689 2024-06-02 22:13:49.000000 socketbee-0.1.3/pyproject.toml
--rw-r--r--   0 boulamakandine   (501) staff       (20)       38 2024-06-02 22:13:50.857383 socketbee-0.1.3/setup.cfg
--rw-r--r--   0 boulamakandine   (501) staff       (20)      121 2024-05-13 04:56:07.000000 socketbee-0.1.3/setup.py
-drwxr-xr-x   0 boulamakandine   (501) staff       (20)        0 2024-06-02 22:13:50.855961 socketbee-0.1.3/socketbee/
--rw-r--r--   0 boulamakandine   (501) staff       (20)        0 2024-05-13 04:42:01.000000 socketbee-0.1.3/socketbee/__init__.py
--rw-r--r--   0 boulamakandine   (501) staff       (20)     1460 2024-05-24 19:06:50.000000 socketbee-0.1.3/socketbee/client.py
--rw-r--r--   0 boulamakandine   (501) staff       (20)        0 2024-05-13 04:42:14.000000 socketbee-0.1.3/socketbee/settings.py
-drwxr-xr-x   0 boulamakandine   (501) staff       (20)        0 2024-06-02 22:13:50.856915 socketbee-0.1.3/socketbee.egg-info/
--rw-r--r--   0 boulamakandine   (501) staff       (20)     3360 2024-06-02 22:13:50.000000 socketbee-0.1.3/socketbee.egg-info/PKG-INFO
--rw-r--r--   0 boulamakandine   (501) staff       (20)      272 2024-06-02 22:13:50.000000 socketbee-0.1.3/socketbee.egg-info/SOURCES.txt
--rw-r--r--   0 boulamakandine   (501) staff       (20)        1 2024-06-02 22:13:50.000000 socketbee-0.1.3/socketbee.egg-info/dependency_links.txt
--rw-r--r--   0 boulamakandine   (501) staff       (20)        9 2024-06-02 22:13:50.000000 socketbee-0.1.3/socketbee.egg-info/requires.txt
--rw-r--r--   0 boulamakandine   (501) staff       (20)       10 2024-06-02 22:13:50.000000 socketbee-0.1.3/socketbee.egg-info/top_level.txt
+drwxr-xr-x   0 boulamakandine   (501) staff       (20)        0 2024-06-02 22:15:15.590071 socketbee-0.1.4/
+-rw-r--r--   0 boulamakandine   (501) staff       (20)     1053 2024-05-13 04:59:24.000000 socketbee-0.1.4/LICENSE.md
+-rw-r--r--   0 boulamakandine   (501) staff       (20)     3360 2024-06-02 22:15:15.589878 socketbee-0.1.4/PKG-INFO
+-rw-r--r--   0 boulamakandine   (501) staff       (20)     2766 2024-06-02 22:13:44.000000 socketbee-0.1.4/README.md
+-rw-r--r--   0 boulamakandine   (501) staff       (20)      689 2024-06-02 22:15:14.000000 socketbee-0.1.4/pyproject.toml
+-rw-r--r--   0 boulamakandine   (501) staff       (20)       38 2024-06-02 22:15:15.590110 socketbee-0.1.4/setup.cfg
+-rw-r--r--   0 boulamakandine   (501) staff       (20)      121 2024-05-13 04:56:07.000000 socketbee-0.1.4/setup.py
+drwxr-xr-x   0 boulamakandine   (501) staff       (20)        0 2024-06-02 22:15:15.588933 socketbee-0.1.4/socketbee/
+-rw-r--r--   0 boulamakandine   (501) staff       (20)        0 2024-05-13 04:42:01.000000 socketbee-0.1.4/socketbee/__init__.py
+-rw-r--r--   0 boulamakandine   (501) staff       (20)     1460 2024-05-24 19:06:50.000000 socketbee-0.1.4/socketbee/client.py
+-rw-r--r--   0 boulamakandine   (501) staff       (20)        0 2024-05-13 04:42:14.000000 socketbee-0.1.4/socketbee/settings.py
+drwxr-xr-x   0 boulamakandine   (501) staff       (20)        0 2024-06-02 22:15:15.589691 socketbee-0.1.4/socketbee.egg-info/
+-rw-r--r--   0 boulamakandine   (501) staff       (20)     3360 2024-06-02 22:15:15.000000 socketbee-0.1.4/socketbee.egg-info/PKG-INFO
+-rw-r--r--   0 boulamakandine   (501) staff       (20)      272 2024-06-02 22:15:15.000000 socketbee-0.1.4/socketbee.egg-info/SOURCES.txt
+-rw-r--r--   0 boulamakandine   (501) staff       (20)        1 2024-06-02 22:15:15.000000 socketbee-0.1.4/socketbee.egg-info/dependency_links.txt
+-rw-r--r--   0 boulamakandine   (501) staff       (20)        9 2024-06-02 22:15:15.000000 socketbee-0.1.4/socketbee.egg-info/requires.txt
+-rw-r--r--   0 boulamakandine   (501) staff       (20)       10 2024-06-02 22:15:15.000000 socketbee-0.1.4/socketbee.egg-info/top_level.txt
```

### Comparing `socketbee-0.1.3/LICENSE.md` & `socketbee-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `socketbee-0.1.3/PKG-INFO` & `socketbee-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketbee
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python wrapper for the SocketBee.
 Author-email: "Boulama K." <boulama@otimbi.com>
 Project-URL: Homepage, https://github.com/socketbee/socketbee.py
 Project-URL: Bug Tracker, https://github.com/socketbee/socketbee.py/issues
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `socketbee-0.1.3/README.md` & `socketbee-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `socketbee-0.1.3/pyproject.toml` & `socketbee-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "socketbee"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Boulama K.", email="boulama@otimbi.com" },
 ]
 description = "A Python wrapper for the SocketBee."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `socketbee-0.1.3/socketbee/client.py` & `socketbee-0.1.4/socketbee/client.py`

 * *Files identical despite different names*

### Comparing `socketbee-0.1.3/socketbee.egg-info/PKG-INFO` & `socketbee-0.1.4/socketbee.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketbee
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python wrapper for the SocketBee.
 Author-email: "Boulama K." <boulama@otimbi.com>
 Project-URL: Homepage, https://github.com/socketbee/socketbee.py
 Project-URL: Bug Tracker, https://github.com/socketbee/socketbee.py/issues
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

