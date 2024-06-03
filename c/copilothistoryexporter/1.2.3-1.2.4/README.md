# Comparing `tmp/copilothistoryexporter-1.2.3.tar.gz` & `tmp/copilothistoryexporter-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copilothistoryexporter-1.2.3.tar", last modified: Mon Jun  3 12:59:35 2024, max compression
+gzip compressed data, was "copilothistoryexporter-1.2.4.tar", last modified: Mon Jun  3 13:01:57 2024, max compression
```

## Comparing `copilothistoryexporter-1.2.3.tar` & `copilothistoryexporter-1.2.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 12:59:35.717752 copilothistoryexporter-1.2.3/
--rw-r--r--   0 mustafakilic   (501) staff       (20)     1073 2024-06-01 16:20:49.000000 copilothistoryexporter-1.2.3/LICENCE
--rw-r--r--   0 mustafakilic   (501) staff       (20)     2752 2024-06-03 12:59:35.717550 copilothistoryexporter-1.2.3/PKG-INFO
--rw-r--r--   0 mustafakilic   (501) staff       (20)     2232 2024-06-02 16:13:30.000000 copilothistoryexporter-1.2.3/README.md
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 12:59:35.713896 copilothistoryexporter-1.2.3/che/
--rw-r--r--   0 mustafakilic   (501) staff       (20)       65 2024-06-03 09:58:49.000000 copilothistoryexporter-1.2.3/che/__init__.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)     1387 2024-06-03 10:05:51.000000 copilothistoryexporter-1.2.3/che/binding.py
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 12:59:35.715994 copilothistoryexporter-1.2.3/che/intercept/
--rw-r--r--   0 mustafakilic   (501) staff       (20)        1 2024-06-03 10:12:16.000000 copilothistoryexporter-1.2.3/che/intercept/__init__.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      489 2024-06-03 10:11:44.000000 copilothistoryexporter-1.2.3/che/intercept/cache.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      585 2024-06-03 10:13:30.000000 copilothistoryexporter-1.2.3/che/intercept/chain.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      395 2024-06-02 16:13:00.000000 copilothistoryexporter-1.2.3/che/intercept/conversation.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      190 2024-06-03 10:12:37.000000 copilothistoryexporter-1.2.3/che/intercept/interceptor.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      330 2024-06-03 10:14:18.000000 copilothistoryexporter-1.2.3/che/intercept/markdown.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      236 2024-06-03 10:12:47.000000 copilothistoryexporter-1.2.3/che/intercept/request.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      578 2024-06-03 10:14:50.000000 copilothistoryexporter-1.2.3/che/intercept/vote.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      710 2024-06-03 12:05:26.000000 copilothistoryexporter-1.2.3/che/main.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)     2367 2024-06-03 10:13:00.000000 copilothistoryexporter-1.2.3/che/utils.py
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 12:59:35.717310 copilothistoryexporter-1.2.3/copilothistoryexporter.egg-info/
--rw-r--r--   0 mustafakilic   (501) staff       (20)     2752 2024-06-03 12:59:35.000000 copilothistoryexporter-1.2.3/copilothistoryexporter.egg-info/PKG-INFO
--rw-r--r--   0 mustafakilic   (501) staff       (20)      570 2024-06-03 12:59:35.000000 copilothistoryexporter-1.2.3/copilothistoryexporter.egg-info/SOURCES.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)        1 2024-06-03 12:59:35.000000 copilothistoryexporter-1.2.3/copilothistoryexporter.egg-info/dependency_links.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)       76 2024-06-03 12:59:35.000000 copilothistoryexporter-1.2.3/copilothistoryexporter.egg-info/entry_points.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)       31 2024-06-03 12:59:35.000000 copilothistoryexporter-1.2.3/copilothistoryexporter.egg-info/requires.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)        4 2024-06-03 12:59:35.000000 copilothistoryexporter-1.2.3/copilothistoryexporter.egg-info/top_level.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)      652 2024-06-03 12:58:35.000000 copilothistoryexporter-1.2.3/pyproject.toml
--rw-r--r--   0 mustafakilic   (501) staff       (20)       38 2024-06-03 12:59:35.717800 copilothistoryexporter-1.2.3/setup.cfg
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 13:01:57.068870 copilothistoryexporter-1.2.4/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     1073 2024-06-01 16:20:49.000000 copilothistoryexporter-1.2.4/LICENCE
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     2752 2024-06-03 13:01:57.068570 copilothistoryexporter-1.2.4/PKG-INFO
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     2232 2024-06-02 16:13:30.000000 copilothistoryexporter-1.2.4/README.md
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 13:01:57.065204 copilothistoryexporter-1.2.4/che/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       65 2024-06-03 09:58:49.000000 copilothistoryexporter-1.2.4/che/__init__.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     1387 2024-06-03 10:05:51.000000 copilothistoryexporter-1.2.4/che/binding.py
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 13:01:57.067213 copilothistoryexporter-1.2.4/che/intercept/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)        1 2024-06-03 10:12:16.000000 copilothistoryexporter-1.2.4/che/intercept/__init__.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      489 2024-06-03 10:11:44.000000 copilothistoryexporter-1.2.4/che/intercept/cache.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      585 2024-06-03 10:13:30.000000 copilothistoryexporter-1.2.4/che/intercept/chain.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      395 2024-06-02 16:13:00.000000 copilothistoryexporter-1.2.4/che/intercept/conversation.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      190 2024-06-03 10:12:37.000000 copilothistoryexporter-1.2.4/che/intercept/interceptor.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      330 2024-06-03 10:14:18.000000 copilothistoryexporter-1.2.4/che/intercept/markdown.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      236 2024-06-03 10:12:47.000000 copilothistoryexporter-1.2.4/che/intercept/request.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      578 2024-06-03 10:14:50.000000 copilothistoryexporter-1.2.4/che/intercept/vote.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      710 2024-06-03 12:05:26.000000 copilothistoryexporter-1.2.4/che/main.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     2367 2024-06-03 10:13:00.000000 copilothistoryexporter-1.2.4/che/utils.py
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 13:01:57.068270 copilothistoryexporter-1.2.4/copilothistoryexporter.egg-info/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     2752 2024-06-03 13:01:57.000000 copilothistoryexporter-1.2.4/copilothistoryexporter.egg-info/PKG-INFO
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      570 2024-06-03 13:01:57.000000 copilothistoryexporter-1.2.4/copilothistoryexporter.egg-info/SOURCES.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)        1 2024-06-03 13:01:57.000000 copilothistoryexporter-1.2.4/copilothistoryexporter.egg-info/dependency_links.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       38 2024-06-03 13:01:57.000000 copilothistoryexporter-1.2.4/copilothistoryexporter.egg-info/entry_points.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       31 2024-06-03 13:01:57.000000 copilothistoryexporter-1.2.4/copilothistoryexporter.egg-info/requires.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)        4 2024-06-03 13:01:57.000000 copilothistoryexporter-1.2.4/copilothistoryexporter.egg-info/top_level.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      614 2024-06-03 13:01:54.000000 copilothistoryexporter-1.2.4/pyproject.toml
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       38 2024-06-03 13:01:57.068930 copilothistoryexporter-1.2.4/setup.cfg
```

### Comparing `copilothistoryexporter-1.2.3/LICENCE` & `copilothistoryexporter-1.2.4/LICENCE`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.2.3/PKG-INFO` & `copilothistoryexporter-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copilothistoryexporter
-Version: 1.2.3
+Version: 1.2.4
 Summary: Copilot History Exporter
 Author-email: enciyo <enciyomk61@gmail.com>
 Project-URL: Homepage, https://github.com/enciyo/gh-copilot-history-export
 Project-URL: Source, https://github.com/enciyo/gh-copilot-history-export
 Project-URL: Documentation, https://github.com/enciyo/gh-copilot-history-export
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `copilothistoryexporter-1.2.3/README.md` & `copilothistoryexporter-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.2.3/che/binding.py` & `copilothistoryexporter-1.2.4/che/binding.py`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.2.3/che/intercept/chain.py` & `copilothistoryexporter-1.2.4/che/intercept/chain.py`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.2.3/che/intercept/vote.py` & `copilothistoryexporter-1.2.4/che/intercept/vote.py`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.2.3/che/main.py` & `copilothistoryexporter-1.2.4/che/main.py`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.2.3/che/utils.py` & `copilothistoryexporter-1.2.4/che/utils.py`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.2.3/copilothistoryexporter.egg-info/PKG-INFO` & `copilothistoryexporter-1.2.4/copilothistoryexporter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copilothistoryexporter
-Version: 1.2.3
+Version: 1.2.4
 Summary: Copilot History Exporter
 Author-email: enciyo <enciyomk61@gmail.com>
 Project-URL: Homepage, https://github.com/enciyo/gh-copilot-history-export
 Project-URL: Source, https://github.com/enciyo/gh-copilot-history-export
 Project-URL: Documentation, https://github.com/enciyo/gh-copilot-history-export
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `copilothistoryexporter-1.2.3/copilothistoryexporter.egg-info/SOURCES.txt` & `copilothistoryexporter-1.2.4/copilothistoryexporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

