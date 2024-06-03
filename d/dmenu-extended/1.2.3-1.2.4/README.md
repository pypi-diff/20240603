# Comparing `tmp/dmenu_extended-1.2.3.tar.gz` & `tmp/dmenu_extended-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmenu_extended-1.2.3.tar", last modified: Thu May 30 12:55:43 2024, max compression
+gzip compressed data, was "dmenu_extended-1.2.4.tar", last modified: Mon Jun  3 04:51:15 2024, max compression
```

## Comparing `dmenu_extended-1.2.3.tar` & `dmenu_extended-1.2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-30 12:55:43.137175 dmenu_extended-1.2.3/
--rw-rw-r--   0 mark      (1000) mark      (1000)     1084 2024-04-30 21:06:12.000000 dmenu_extended-1.2.3/LICENSE
--rw-r--r--   0 mark      (1000) mark      (1000)    18293 2024-05-30 12:55:43.137175 dmenu_extended-1.2.3/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)    16417 2024-05-30 10:50:15.000000 dmenu_extended-1.2.3/README.md
--rw-rw-r--   0 mark      (1000) mark      (1000)      950 2024-05-30 12:55:29.000000 dmenu_extended-1.2.3/pyproject.toml
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-05-30 12:55:43.137175 dmenu_extended-1.2.3/setup.cfg
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-30 12:55:43.136175 dmenu_extended-1.2.3/src/
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-30 12:55:43.136175 dmenu_extended-1.2.3/src/dmenu_extended/
--rw-rw-r--   0 mark      (1000) mark      (1000)       20 2024-04-30 21:06:12.000000 dmenu_extended-1.2.3/src/dmenu_extended/__init__.py
--rwxrwxr-x   0 mark      (1000) mark      (1000)     6733 2024-04-30 21:06:12.000000 dmenu_extended-1.2.3/src/dmenu_extended/install_systemd_service.py
--rwxrwxr-x   0 mark      (1000) mark      (1000)    88884 2024-05-30 12:55:29.000000 dmenu_extended-1.2.3/src/dmenu_extended/main.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-30 12:55:43.137175 dmenu_extended-1.2.3/src/dmenu_extended.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)    18293 2024-05-30 12:55:43.000000 dmenu_extended-1.2.3/src/dmenu_extended.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      447 2024-05-30 12:55:43.000000 dmenu_extended-1.2.3/src/dmenu_extended.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-05-30 12:55:43.000000 dmenu_extended-1.2.3/src/dmenu_extended.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)      208 2024-05-30 12:55:43.000000 dmenu_extended-1.2.3/src/dmenu_extended.egg-info/entry_points.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       17 2024-05-30 12:55:43.000000 dmenu_extended-1.2.3/src/dmenu_extended.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       15 2024-05-30 12:55:43.000000 dmenu_extended-1.2.3/src/dmenu_extended.egg-info/top_level.txt
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-30 12:55:43.137175 dmenu_extended-1.2.3/tests/
--rwxrwxr-x   0 mark      (1000) mark      (1000)     2603 2024-04-30 21:06:12.000000 dmenu_extended-1.2.3/tests/test_install_systemd_service.py
--rwxrwxr-x   0 mark      (1000) mark      (1000)     2679 2024-04-30 21:06:12.000000 dmenu_extended-1.2.3/tests/test_main.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-06-03 04:51:15.779499 dmenu_extended-1.2.4/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1084 2024-04-30 21:06:12.000000 dmenu_extended-1.2.4/LICENSE
+-rw-r--r--   0 mark      (1000) mark      (1000)    18293 2024-06-03 04:51:15.779499 dmenu_extended-1.2.4/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)    16417 2024-05-30 10:50:15.000000 dmenu_extended-1.2.4/README.md
+-rw-rw-r--   0 mark      (1000) mark      (1000)      950 2024-06-03 04:48:44.000000 dmenu_extended-1.2.4/pyproject.toml
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-06-03 04:51:15.779499 dmenu_extended-1.2.4/setup.cfg
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-06-03 04:51:15.777499 dmenu_extended-1.2.4/src/
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-06-03 04:51:15.778499 dmenu_extended-1.2.4/src/dmenu_extended/
+-rw-rw-r--   0 mark      (1000) mark      (1000)       20 2024-04-30 21:06:12.000000 dmenu_extended-1.2.4/src/dmenu_extended/__init__.py
+-rwxrwxr-x   0 mark      (1000) mark      (1000)     6733 2024-04-30 21:06:12.000000 dmenu_extended-1.2.4/src/dmenu_extended/install_systemd_service.py
+-rwxrwxr-x   0 mark      (1000) mark      (1000)    89042 2024-06-03 04:48:44.000000 dmenu_extended-1.2.4/src/dmenu_extended/main.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-06-03 04:51:15.779499 dmenu_extended-1.2.4/src/dmenu_extended.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)    18293 2024-06-03 04:51:15.000000 dmenu_extended-1.2.4/src/dmenu_extended.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      447 2024-06-03 04:51:15.000000 dmenu_extended-1.2.4/src/dmenu_extended.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-06-03 04:51:15.000000 dmenu_extended-1.2.4/src/dmenu_extended.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)      208 2024-06-03 04:51:15.000000 dmenu_extended-1.2.4/src/dmenu_extended.egg-info/entry_points.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       17 2024-06-03 04:51:15.000000 dmenu_extended-1.2.4/src/dmenu_extended.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       15 2024-06-03 04:51:15.000000 dmenu_extended-1.2.4/src/dmenu_extended.egg-info/top_level.txt
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-06-03 04:51:15.779499 dmenu_extended-1.2.4/tests/
+-rwxrwxr-x   0 mark      (1000) mark      (1000)     2603 2024-04-30 21:06:12.000000 dmenu_extended-1.2.4/tests/test_install_systemd_service.py
+-rwxrwxr-x   0 mark      (1000) mark      (1000)     2679 2024-04-30 21:06:12.000000 dmenu_extended-1.2.4/tests/test_main.py
```

### Comparing `dmenu_extended-1.2.3/LICENSE` & `dmenu_extended-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dmenu_extended-1.2.3/PKG-INFO` & `dmenu_extended-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmenu_extended
-Version: 1.2.3
+Version: 1.2.4
 Summary: A wrapper for dmenu that implements plugins and fast file/folder searching
 Author-email: Mark Hedley Jones <markhedleyjones@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2013 Mark Hedley Jones
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
```

### Comparing `dmenu_extended-1.2.3/README.md` & `dmenu_extended-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `dmenu_extended-1.2.3/pyproject.toml` & `dmenu_extended-1.2.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dmenu_extended"
-version = "1.2.3"
+version = "1.2.4"
 authors = [
   { name="Mark Hedley Jones", email="markhedleyjones@gmail.com" },
 ]
 description = "A wrapper for dmenu that implements plugins and fast file/folder searching"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `dmenu_extended-1.2.3/src/dmenu_extended/install_systemd_service.py` & `dmenu_extended-1.2.4/src/dmenu_extended/install_systemd_service.py`

 * *Files identical despite different names*

### Comparing `dmenu_extended-1.2.3/src/dmenu_extended/main.py` & `dmenu_extended-1.2.4/src/dmenu_extended/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -782,31 +782,34 @@
             tmp = []
             foundError = False
             if self.debug:
                 print("Non-printable characters detected in cache: ")
             for item in items:
                 clean = True
                 for char in item:
-                    if char not in string.printable:
+                    if not str.isprintable(char):
                         clean = False
                         foundError = True
                         if self.debug:
-                            print("Culprit: " + item)
+                            print(
+                                "Culprit: "
+                                + item.encode("unicode_escape").decode("utf-8")
+                            )
                 if clean:
                     tmp.append(item)
             if foundError:
                 if self.debug:
                     print("")
                     print(
                         "Caching performance will be affected while these items remain"
                     )
                     print("Offending items have been excluded from cache")
                 with open(path, "wb") as f:
                     for item in tmp:
-                        f.write(item + "\n")
+                        f.write(item.encode("unicode_escape") + b"\n")
                 return 2
             else:
                 if self.debug:
                     print("Unknown error saving data cache")
                 return 0
 
     def cache_open(self, path):
```

### Comparing `dmenu_extended-1.2.3/src/dmenu_extended.egg-info/PKG-INFO` & `dmenu_extended-1.2.4/src/dmenu_extended.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmenu_extended
-Version: 1.2.3
+Version: 1.2.4
 Summary: A wrapper for dmenu that implements plugins and fast file/folder searching
 Author-email: Mark Hedley Jones <markhedleyjones@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2013 Mark Hedley Jones
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
```

### Comparing `dmenu_extended-1.2.3/tests/test_install_systemd_service.py` & `dmenu_extended-1.2.4/tests/test_install_systemd_service.py`

 * *Files identical despite different names*

### Comparing `dmenu_extended-1.2.3/tests/test_main.py` & `dmenu_extended-1.2.4/tests/test_main.py`

 * *Files identical despite different names*

