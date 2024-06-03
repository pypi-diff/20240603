# Comparing `tmp/crazy_thursday-2024.6.2.1.tar.gz` & `tmp/crazy_thursday-2024.6.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crazy_thursday-2024.6.2.1.tar", last modified: Sun Jun  2 05:29:29 2024, max compression
+gzip compressed data, was "crazy_thursday-2024.6.3.0.tar", last modified: Sun Jun  2 17:29:42 2024, max compression
```

## Comparing `crazy_thursday-2024.6.2.1.tar` & `crazy_thursday-2024.6.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:29:29.496639 crazy_thursday-2024.6.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-06-02 05:29:20.000000 crazy_thursday-2024.6.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-06-02 05:29:29.496639 crazy_thursday-2024.6.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-06-02 05:29:20.000000 crazy_thursday-2024.6.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:29:29.492639 crazy_thursday-2024.6.2.1/crazy_thursday/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-02 05:29:25.000000 crazy_thursday-2024.6.2.1/crazy_thursday/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-06-02 05:29:20.000000 crazy_thursday-2024.6.2.1/crazy_thursday/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-06-02 05:29:25.000000 crazy_thursday-2024.6.2.1/crazy_thursday/corpus.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-02 05:29:20.000000 crazy_thursday-2024.6.2.1/crazy_thursday/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:29:29.496639 crazy_thursday-2024.6.2.1/crazy_thursday.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-06-02 05:29:29.000000 crazy_thursday-2024.6.2.1/crazy_thursday.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-06-02 05:29:29.000000 crazy_thursday-2024.6.2.1/crazy_thursday.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 05:29:29.000000 crazy_thursday-2024.6.2.1/crazy_thursday.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-06-02 05:29:29.000000 crazy_thursday-2024.6.2.1/crazy_thursday.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-02 05:29:29.000000 crazy_thursday-2024.6.2.1/crazy_thursday.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-02 05:29:29.000000 crazy_thursday-2024.6.2.1/crazy_thursday.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:29:29.496639 crazy_thursday-2024.6.2.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 05:29:20.000000 crazy_thursday-2024.6.2.1/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-06-02 05:29:20.000000 crazy_thursday-2024.6.2.1/scripts/get_issues.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-06-02 05:29:20.000000 crazy_thursday-2024.6.2.1/scripts/update_curpus.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 05:29:29.496639 crazy_thursday-2024.6.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-06-02 05:29:20.000000 crazy_thursday-2024.6.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:29:42.354337 crazy_thursday-2024.6.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-06-02 17:29:34.000000 crazy_thursday-2024.6.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-06-02 17:29:42.354337 crazy_thursday-2024.6.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-06-02 17:29:34.000000 crazy_thursday-2024.6.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:29:42.354337 crazy_thursday-2024.6.3.0/crazy_thursday/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-02 17:29:38.000000 crazy_thursday-2024.6.3.0/crazy_thursday/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-06-02 17:29:34.000000 crazy_thursday-2024.6.3.0/crazy_thursday/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-06-02 17:29:37.000000 crazy_thursday-2024.6.3.0/crazy_thursday/corpus.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-02 17:29:34.000000 crazy_thursday-2024.6.3.0/crazy_thursday/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:29:42.354337 crazy_thursday-2024.6.3.0/crazy_thursday.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-06-02 17:29:42.000000 crazy_thursday-2024.6.3.0/crazy_thursday.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-06-02 17:29:42.000000 crazy_thursday-2024.6.3.0/crazy_thursday.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 17:29:42.000000 crazy_thursday-2024.6.3.0/crazy_thursday.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-06-02 17:29:42.000000 crazy_thursday-2024.6.3.0/crazy_thursday.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-02 17:29:42.000000 crazy_thursday-2024.6.3.0/crazy_thursday.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-02 17:29:42.000000 crazy_thursday-2024.6.3.0/crazy_thursday.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:29:42.354337 crazy_thursday-2024.6.3.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 17:29:34.000000 crazy_thursday-2024.6.3.0/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-06-02 17:29:34.000000 crazy_thursday-2024.6.3.0/scripts/get_issues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-06-02 17:29:34.000000 crazy_thursday-2024.6.3.0/scripts/update_curpus.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 17:29:42.354337 crazy_thursday-2024.6.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-06-02 17:29:34.000000 crazy_thursday-2024.6.3.0/setup.py
```

### Comparing `crazy_thursday-2024.6.2.1/LICENSE` & `crazy_thursday-2024.6.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crazy_thursday-2024.6.2.1/PKG-INFO` & `crazy_thursday-2024.6.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crazy-thursday
-Version: 2024.6.2.1
+Version: 2024.6.3.0
 Summary: a cli tool to print crazy thursday article
 Home-page: https://github.com/zqmillet/sphinx-console
 Author: kinopico
 Author-email: zqmillet@qq.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: rich==12.5.1
```

### Comparing `crazy_thursday-2024.6.2.1/README.md` & `crazy_thursday-2024.6.3.0/README.md`

 * *Files identical despite different names*

### Comparing `crazy_thursday-2024.6.2.1/crazy_thursday/__main__.py` & `crazy_thursday-2024.6.3.0/crazy_thursday/__main__.py`

 * *Files identical despite different names*

### Comparing `crazy_thursday-2024.6.2.1/crazy_thursday/corpus.jsonl` & `crazy_thursday-2024.6.3.0/crazy_thursday/corpus.jsonl`

 * *Files identical despite different names*

### Comparing `crazy_thursday-2024.6.2.1/crazy_thursday.egg-info/PKG-INFO` & `crazy_thursday-2024.6.3.0/crazy_thursday.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crazy-thursday
-Version: 2024.6.2.1
+Version: 2024.6.3.0
 Summary: a cli tool to print crazy thursday article
 Home-page: https://github.com/zqmillet/sphinx-console
 Author: kinopico
 Author-email: zqmillet@qq.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: rich==12.5.1
```

### Comparing `crazy_thursday-2024.6.2.1/scripts/get_issues.py` & `crazy_thursday-2024.6.3.0/scripts/get_issues.py`

 * *Files identical despite different names*

### Comparing `crazy_thursday-2024.6.2.1/scripts/update_curpus.py` & `crazy_thursday-2024.6.3.0/scripts/update_curpus.py`

 * *Files identical despite different names*

### Comparing `crazy_thursday-2024.6.2.1/setup.py` & `crazy_thursday-2024.6.3.0/setup.py`

 * *Files identical despite different names*

