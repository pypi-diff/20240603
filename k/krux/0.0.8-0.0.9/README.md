# Comparing `tmp/krux-0.0.8.tar.gz` & `tmp/krux-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/krux-0.0.8.tar", last modified: Mon Oct 22 02:51:47 2018, max compression
+gzip compressed data, was "dist/krux-0.0.9.tar", last modified: Mon Oct 22 06:22:10 2018, max compression
```

## Comparing `krux-0.0.8.tar` & `krux-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,29 @@
-drwxrwxr-x   0 dodo      (1000) dodo      (1000)        0 2018-10-22 02:51:47.000000 krux-0.0.8/
-drwxrwxr-x   0 dodo      (1000) dodo      (1000)        0 2018-10-22 02:51:47.000000 krux-0.0.8/krux/
-drwxrwxr-x   0 dodo      (1000) dodo      (1000)        0 2018-10-22 02:51:47.000000 krux-0.0.8/krux/types/
--rw-r--r--   0 dodo      (1000) dodo      (1000)       69 2018-07-04 05:57:37.000000 krux-0.0.8/krux/types/__init__.py
--rw-r--r--   0 dodo      (1000) dodo      (1000)      764 2018-07-04 05:57:01.000000 krux-0.0.8/krux/types/null.py
--rw-r--r--   0 dodo      (1000) dodo      (1000)      344 2018-07-04 05:57:01.000000 krux-0.0.8/krux/types/singleton.py
--rw-r--r--   0 dodo      (1000) dodo      (1000)       38 2018-07-04 05:51:06.000000 krux-0.0.8/krux/__init__.py
-drwxrwxr-x   0 dodo      (1000) dodo      (1000)        0 2018-10-22 02:51:47.000000 krux-0.0.8/krux/random/
--rw-r--r--   0 dodo      (1000) dodo      (1000)       43 2018-07-09 05:52:02.000000 krux-0.0.8/krux/random/__init__.py
--rw-r--r--   0 dodo      (1000) dodo      (1000)     1375 2018-10-10 03:13:20.000000 krux-0.0.8/krux/random/uuid.py
-drwxrwxr-x   0 dodo      (1000) dodo      (1000)        0 2018-10-22 02:51:47.000000 krux-0.0.8/krux/converters/
--rw-r--r--   0 dodo      (1000) dodo      (1000)      110 2018-09-27 02:22:56.000000 krux-0.0.8/krux/converters/__init__.py
--rw-rw-r--   0 dodo      (1000) dodo      (1000)      329 2018-09-19 02:53:06.000000 krux-0.0.8/krux/converters/misc.py
--rw-rw-r--   0 dodo      (1000) dodo      (1000)      375 2018-09-27 02:23:52.000000 krux-0.0.8/krux/converters/structure.py
--rw-r--r--   0 dodo      (1000) dodo      (1000)     4269 2018-07-25 09:21:59.000000 krux-0.0.8/krux/converters/string_related.py
-drwxrwxr-x   0 dodo      (1000) dodo      (1000)        0 2018-10-22 02:51:47.000000 krux-0.0.8/krux/regex/
--rw-rw-r--   0 dodo      (1000) dodo      (1000)     1949 2018-10-22 02:45:20.000000 krux-0.0.8/krux/regex/grep.py
--rw-rw-r--   0 dodo      (1000) dodo      (1000)       92 2018-10-19 10:02:22.000000 krux-0.0.8/krux/regex/__init__.py
--rw-rw-r--   0 dodo      (1000) dodo      (1000)       25 2018-10-19 10:06:33.000000 krux-0.0.8/krux/regex/exceptions.py
--rw-rw-r--   0 dodo      (1000) dodo      (1000)      587 2018-10-19 10:00:48.000000 krux-0.0.8/krux/regex/pattern.py
-drwxrwxr-x   0 dodo      (1000) dodo      (1000)        0 2018-10-22 02:51:47.000000 krux-0.0.8/krux.egg-info/
--rw-r--r--   0 dodo      (1000) dodo      (1000)       11 2018-10-22 02:51:47.000000 krux-0.0.8/krux.egg-info/top_level.txt
--rw-r--r--   0 dodo      (1000) dodo      (1000)      405 2018-10-22 02:51:47.000000 krux-0.0.8/krux.egg-info/PKG-INFO
--rw-r--r--   0 dodo      (1000) dodo      (1000)        1 2018-10-22 02:51:47.000000 krux-0.0.8/krux.egg-info/dependency_links.txt
--rw-r--r--   0 dodo      (1000) dodo      (1000)      501 2018-10-22 02:51:47.000000 krux-0.0.8/krux.egg-info/SOURCES.txt
--rw-rw-r--   0 dodo      (1000) dodo      (1000)      405 2018-10-22 02:51:47.000000 krux-0.0.8/PKG-INFO
--rw-rw-r--   0 dodo      (1000) dodo      (1000)       38 2018-10-22 02:51:47.000000 krux-0.0.8/setup.cfg
--rw-r--r--   0 dodo      (1000) dodo      (1000)       32 2018-07-04 05:49:07.000000 krux-0.0.8/README.md
-drwxrwxr-x   0 dodo      (1000) dodo      (1000)        0 2018-10-22 02:51:47.000000 krux-0.0.8/tests/
--rw-r--r--   0 dodo      (1000) dodo      (1000)        0 2018-07-25 08:45:49.000000 krux-0.0.8/tests/__init__.py
--rw-r--r--   0 dodo      (1000) dodo      (1000)     1274 2018-07-25 09:15:41.000000 krux-0.0.8/tests/test_str2obj.py
--rw-r--r--   0 dodo      (1000) dodo      (1000)      655 2018-10-22 02:51:35.000000 krux-0.0.8/setup.py
+drwxrwxr-x   0 dodo      (1000) dodo      (1000)        0 2018-10-22 06:22:10.000000 krux-0.0.9/
+drwxrwxr-x   0 dodo      (1000) dodo      (1000)        0 2018-10-22 06:22:10.000000 krux-0.0.9/krux/
+drwxrwxr-x   0 dodo      (1000) dodo      (1000)        0 2018-10-22 06:22:10.000000 krux-0.0.9/krux/types/
+-rw-r--r--   0 dodo      (1000) dodo      (1000)       69 2018-07-04 05:57:37.000000 krux-0.0.9/krux/types/__init__.py
+-rw-r--r--   0 dodo      (1000) dodo      (1000)      764 2018-07-04 05:57:01.000000 krux-0.0.9/krux/types/null.py
+-rw-r--r--   0 dodo      (1000) dodo      (1000)      344 2018-07-04 05:57:01.000000 krux-0.0.9/krux/types/singleton.py
+-rw-r--r--   0 dodo      (1000) dodo      (1000)       38 2018-07-04 05:51:06.000000 krux-0.0.9/krux/__init__.py
+drwxrwxr-x   0 dodo      (1000) dodo      (1000)        0 2018-10-22 06:22:10.000000 krux-0.0.9/krux/random/
+-rw-r--r--   0 dodo      (1000) dodo      (1000)       43 2018-07-09 05:52:02.000000 krux-0.0.9/krux/random/__init__.py
+-rw-r--r--   0 dodo      (1000) dodo      (1000)     1375 2018-10-10 03:13:20.000000 krux-0.0.9/krux/random/uuid.py
+drwxrwxr-x   0 dodo      (1000) dodo      (1000)        0 2018-10-22 06:22:10.000000 krux-0.0.9/krux/converters/
+-rw-r--r--   0 dodo      (1000) dodo      (1000)      110 2018-09-27 02:22:56.000000 krux-0.0.9/krux/converters/__init__.py
+-rw-rw-r--   0 dodo      (1000) dodo      (1000)      329 2018-09-19 02:53:06.000000 krux-0.0.9/krux/converters/misc.py
+-rw-rw-r--   0 dodo      (1000) dodo      (1000)      375 2018-09-27 02:23:52.000000 krux-0.0.9/krux/converters/structure.py
+-rw-r--r--   0 dodo      (1000) dodo      (1000)     4269 2018-07-25 09:21:59.000000 krux-0.0.9/krux/converters/string_related.py
+drwxrwxr-x   0 dodo      (1000) dodo      (1000)        0 2018-10-22 06:22:10.000000 krux-0.0.9/krux/regex/
+-rw-rw-r--   0 dodo      (1000) dodo      (1000)     3857 2018-10-22 06:20:15.000000 krux-0.0.9/krux/regex/__init__.py
+drwxrwxr-x   0 dodo      (1000) dodo      (1000)        0 2018-10-22 06:22:10.000000 krux-0.0.9/krux.egg-info/
+-rw-r--r--   0 dodo      (1000) dodo      (1000)       11 2018-10-22 06:22:10.000000 krux-0.0.9/krux.egg-info/top_level.txt
+-rw-r--r--   0 dodo      (1000) dodo      (1000)      405 2018-10-22 06:22:10.000000 krux-0.0.9/krux.egg-info/PKG-INFO
+-rw-r--r--   0 dodo      (1000) dodo      (1000)        1 2018-10-22 06:22:10.000000 krux-0.0.9/krux.egg-info/dependency_links.txt
+-rw-r--r--   0 dodo      (1000) dodo      (1000)      435 2018-10-22 06:22:10.000000 krux-0.0.9/krux.egg-info/SOURCES.txt
+-rw-rw-r--   0 dodo      (1000) dodo      (1000)      405 2018-10-22 06:22:10.000000 krux-0.0.9/PKG-INFO
+-rw-rw-r--   0 dodo      (1000) dodo      (1000)       38 2018-10-22 06:22:10.000000 krux-0.0.9/setup.cfg
+-rw-r--r--   0 dodo      (1000) dodo      (1000)       32 2018-07-04 05:49:07.000000 krux-0.0.9/README.md
+drwxrwxr-x   0 dodo      (1000) dodo      (1000)        0 2018-10-22 06:22:10.000000 krux-0.0.9/tests/
+-rw-r--r--   0 dodo      (1000) dodo      (1000)        0 2018-07-25 08:45:49.000000 krux-0.0.9/tests/__init__.py
+-rw-r--r--   0 dodo      (1000) dodo      (1000)     1274 2018-07-25 09:15:41.000000 krux-0.0.9/tests/test_str2obj.py
+-rw-r--r--   0 dodo      (1000) dodo      (1000)      655 2018-10-22 06:22:05.000000 krux-0.0.9/setup.py
```

### Comparing `krux-0.0.8/krux/types/null.py` & `krux-0.0.9/krux/types/null.py`

 * *Files identical despite different names*

### Comparing `krux-0.0.8/krux/random/uuid.py` & `krux-0.0.9/krux/random/uuid.py`

 * *Files identical despite different names*

### Comparing `krux-0.0.8/krux/converters/string_related.py` & `krux-0.0.9/krux/converters/string_related.py`

 * *Files identical despite different names*

### Comparing `krux-0.0.8/tests/test_str2obj.py` & `krux-0.0.9/tests/test_str2obj.py`

 * *Files identical despite different names*

### Comparing `krux-0.0.8/setup.py` & `krux-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # with open("README.md", "r") as fh:
 #     long_description = fh.read()
 
 
 setuptools.setup(
     name="krux",
-    version="0.0.8",
+    version="0.0.9",
     author="claydodo and his little friends (xiao huo ban)",
     author_email="claydodo@foxmail.com",
     description="misc utils",
     # long_description=long_description,
     # long_description_content_type="text/markdown",
     url="https://github.com/claydodo/krux",
     packages=setuptools.find_packages(),
```

