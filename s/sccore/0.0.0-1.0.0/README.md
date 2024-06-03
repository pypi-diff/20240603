# Comparing `tmp/sccore-0.0.0.tar.gz` & `tmp/sccore-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sccore-0.0.0.tar", last modified: Tue May 21 09:17:17 2024, max compression
+gzip compressed data, was "sccore-1.0.0.tar", last modified: Mon Jun  3 02:43:38 2024, max compression
```

## Comparing `sccore-0.0.0.tar` & `sccore-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:17:17.403787 sccore-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-21 09:17:17.403787 sccore-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-21 09:16:59.000000 sccore-0.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:17:17.399787 sccore-0.0.0/sccore/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:16:59.000000 sccore-0.0.0/sccore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:17:17.403787 sccore-0.0.0/sccore/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:16:59.000000 sccore-0.0.0/sccore/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-21 09:16:59.000000 sccore-0.0.0/sccore/cli/create_genome.py
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-05-21 09:16:59.000000 sccore-0.0.0/sccore/cli/create_test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     9235 2024-05-21 09:16:59.000000 sccore-0.0.0/sccore/parse_protocol.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1922 2024-05-21 09:16:59.000000 sccore-0.0.0/sccore/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:17:17.403787 sccore-0.0.0/sccore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-21 09:17:17.000000 sccore-0.0.0/sccore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-21 09:17:17.000000 sccore-0.0.0/sccore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:17:17.000000 sccore-0.0.0/sccore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-21 09:17:17.000000 sccore-0.0.0/sccore.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-21 09:17:17.000000 sccore-0.0.0/sccore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-21 09:17:17.000000 sccore-0.0.0/sccore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 09:17:17.403787 sccore-0.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:43:38.050881 sccore-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-06-03 02:43:38.050881 sccore-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-06-03 02:43:20.000000 sccore-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:43:38.046882 sccore-1.0.0/sccore/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-03 02:43:20.000000 sccore-1.0.0/sccore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:43:38.046882 sccore-1.0.0/sccore/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 02:43:20.000000 sccore-1.0.0/sccore/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-06-03 02:43:20.000000 sccore-1.0.0/sccore/cli/create_genome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5935 2024-06-03 02:43:20.000000 sccore-1.0.0/sccore/cli/create_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-06-03 02:43:20.000000 sccore-1.0.0/sccore/cli/format_bc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-06-03 02:43:20.000000 sccore-1.0.0/sccore/cli/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9235 2024-06-03 02:43:20.000000 sccore-1.0.0/sccore/parse_protocol.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2314 2024-06-03 02:43:20.000000 sccore-1.0.0/sccore/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:43:38.046882 sccore-1.0.0/sccore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-06-03 02:43:38.000000 sccore-1.0.0/sccore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-06-03 02:43:38.000000 sccore-1.0.0/sccore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 02:43:38.000000 sccore-1.0.0/sccore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-06-03 02:43:38.000000 sccore-1.0.0/sccore.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-06-03 02:43:38.000000 sccore-1.0.0/sccore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-03 02:43:38.000000 sccore-1.0.0/sccore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 02:43:38.050881 sccore-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-06-03 02:43:20.000000 sccore-1.0.0/setup.py
```

### Comparing `sccore-0.0.0/sccore/cli/create_genome.py` & `sccore-1.0.0/sccore/cli/create_genome.py`

 * *Files identical despite different names*

### Comparing `sccore-0.0.0/sccore/parse_protocol.py` & `sccore-1.0.0/sccore/parse_protocol.py`

 * *Files identical despite different names*

### Comparing `sccore-0.0.0/sccore/utils.py` & `sccore-1.0.0/sccore/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from collections import defaultdict
 import gzip
 import json
 import logging
 import sys
 import time
 from datetime import timedelta
 from functools import wraps
@@ -18,14 +19,21 @@
 
 def read_one_col(fn):
     """read one column file into list"""
     with openfile(fn) as f:
         return [x.strip() for x in f]
 
 
+def write_one_col(a: list, fn):
+    """write list into one column file"""
+    with openfile(fn, "wt") as f:
+        f.write("\n".join(a))
+        f.write("\n")
+
+
 def fastq_str(name, seq, qual):
     """return fastq read string"""
     return f"@{name}\n{seq}\n+\n{qual}\n"
 
 
 def get_logger(name, level=logging.INFO):
     """out to stderr"""
@@ -39,14 +47,21 @@
 
 
 def write_json(data, fn):
     with open(fn, "w") as f:
         json.dump(data, f, indent=4)
 
 
+def nested_defaultdict(dim=3, val_type=int):
+    if dim == 1:
+        return defaultdict(val_type)
+    else:
+        return defaultdict(lambda: nested_defaultdict(dim - 1, val_type=val_type))
+
+
 def add_log(func):
     """
     logging start and done.
     """
     log_formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
 
     module = func.__module__
```

