# Comparing `tmp/copilothistoryexporter-1.2.1.tar.gz` & `tmp/copilothistoryexporter-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copilothistoryexporter-1.2.1.tar", last modified: Mon Jun  3 10:55:00 2024, max compression
+gzip compressed data, was "copilothistoryexporter-1.2.2.tar", last modified: Mon Jun  3 11:23:54 2024, max compression
```

## Comparing `copilothistoryexporter-1.2.1.tar` & `copilothistoryexporter-1.2.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 10:55:00.314552 copilothistoryexporter-1.2.1/
--rw-r--r--   0 mustafakilic   (501) staff       (20)     1073 2024-06-01 16:20:49.000000 copilothistoryexporter-1.2.1/LICENCE
--rw-r--r--   0 mustafakilic   (501) staff       (20)     2752 2024-06-03 10:55:00.314335 copilothistoryexporter-1.2.1/PKG-INFO
--rw-r--r--   0 mustafakilic   (501) staff       (20)     2232 2024-06-02 16:13:30.000000 copilothistoryexporter-1.2.1/README.md
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 10:55:00.312193 copilothistoryexporter-1.2.1/che/
--rw-r--r--   0 mustafakilic   (501) staff       (20)       65 2024-06-03 09:58:49.000000 copilothistoryexporter-1.2.1/che/__init__.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)     1387 2024-06-03 10:05:51.000000 copilothistoryexporter-1.2.1/che/binding.py
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 10:55:00.313199 copilothistoryexporter-1.2.1/che/intercept/
--rw-r--r--   0 mustafakilic   (501) staff       (20)        1 2024-06-03 10:12:16.000000 copilothistoryexporter-1.2.1/che/intercept/__init__.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      489 2024-06-03 10:11:44.000000 copilothistoryexporter-1.2.1/che/intercept/cache.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      585 2024-06-03 10:13:30.000000 copilothistoryexporter-1.2.1/che/intercept/chain.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      395 2024-06-02 16:13:00.000000 copilothistoryexporter-1.2.1/che/intercept/conversation.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      190 2024-06-03 10:12:37.000000 copilothistoryexporter-1.2.1/che/intercept/interceptor.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      330 2024-06-03 10:14:18.000000 copilothistoryexporter-1.2.1/che/intercept/markdown.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      236 2024-06-03 10:12:47.000000 copilothistoryexporter-1.2.1/che/intercept/request.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      578 2024-06-03 10:14:50.000000 copilothistoryexporter-1.2.1/che/intercept/vote.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      703 2024-06-03 10:53:57.000000 copilothistoryexporter-1.2.1/che/main.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)     2367 2024-06-03 10:13:00.000000 copilothistoryexporter-1.2.1/che/utils.py
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 10:55:00.314133 copilothistoryexporter-1.2.1/copilothistoryexporter.egg-info/
--rw-r--r--   0 mustafakilic   (501) staff       (20)     2752 2024-06-03 10:55:00.000000 copilothistoryexporter-1.2.1/copilothistoryexporter.egg-info/PKG-INFO
--rw-r--r--   0 mustafakilic   (501) staff       (20)      570 2024-06-03 10:55:00.000000 copilothistoryexporter-1.2.1/copilothistoryexporter.egg-info/SOURCES.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)        1 2024-06-03 10:55:00.000000 copilothistoryexporter-1.2.1/copilothistoryexporter.egg-info/dependency_links.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)       80 2024-06-03 10:55:00.000000 copilothistoryexporter-1.2.1/copilothistoryexporter.egg-info/entry_points.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)       31 2024-06-03 10:55:00.000000 copilothistoryexporter-1.2.1/copilothistoryexporter.egg-info/requires.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)        4 2024-06-03 10:55:00.000000 copilothistoryexporter-1.2.1/copilothistoryexporter.egg-info/top_level.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)      656 2024-06-03 10:54:42.000000 copilothistoryexporter-1.2.1/pyproject.toml
--rw-r--r--   0 mustafakilic   (501) staff       (20)       38 2024-06-03 10:55:00.314598 copilothistoryexporter-1.2.1/setup.cfg
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 11:23:54.561156 copilothistoryexporter-1.2.2/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     1073 2024-06-01 16:20:49.000000 copilothistoryexporter-1.2.2/LICENCE
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     2752 2024-06-03 11:23:54.560988 copilothistoryexporter-1.2.2/PKG-INFO
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     2232 2024-06-02 16:13:30.000000 copilothistoryexporter-1.2.2/README.md
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 11:23:54.557898 copilothistoryexporter-1.2.2/che/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       65 2024-06-03 09:58:49.000000 copilothistoryexporter-1.2.2/che/__init__.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     1387 2024-06-03 10:05:51.000000 copilothistoryexporter-1.2.2/che/binding.py
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 11:23:54.559799 copilothistoryexporter-1.2.2/che/intercept/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)        1 2024-06-03 10:12:16.000000 copilothistoryexporter-1.2.2/che/intercept/__init__.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      489 2024-06-03 10:11:44.000000 copilothistoryexporter-1.2.2/che/intercept/cache.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      585 2024-06-03 10:13:30.000000 copilothistoryexporter-1.2.2/che/intercept/chain.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      395 2024-06-02 16:13:00.000000 copilothistoryexporter-1.2.2/che/intercept/conversation.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      190 2024-06-03 10:12:37.000000 copilothistoryexporter-1.2.2/che/intercept/interceptor.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      330 2024-06-03 10:14:18.000000 copilothistoryexporter-1.2.2/che/intercept/markdown.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      236 2024-06-03 10:12:47.000000 copilothistoryexporter-1.2.2/che/intercept/request.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      578 2024-06-03 10:14:50.000000 copilothistoryexporter-1.2.2/che/intercept/vote.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      708 2024-06-03 11:22:47.000000 copilothistoryexporter-1.2.2/che/main.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     2367 2024-06-03 10:13:00.000000 copilothistoryexporter-1.2.2/che/utils.py
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 11:23:54.560818 copilothistoryexporter-1.2.2/copilothistoryexporter.egg-info/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     2752 2024-06-03 11:23:54.000000 copilothistoryexporter-1.2.2/copilothistoryexporter.egg-info/PKG-INFO
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      570 2024-06-03 11:23:54.000000 copilothistoryexporter-1.2.2/copilothistoryexporter.egg-info/SOURCES.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)        1 2024-06-03 11:23:54.000000 copilothistoryexporter-1.2.2/copilothistoryexporter.egg-info/dependency_links.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       80 2024-06-03 11:23:54.000000 copilothistoryexporter-1.2.2/copilothistoryexporter.egg-info/entry_points.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       31 2024-06-03 11:23:54.000000 copilothistoryexporter-1.2.2/copilothistoryexporter.egg-info/requires.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)        4 2024-06-03 11:23:54.000000 copilothistoryexporter-1.2.2/copilothistoryexporter.egg-info/top_level.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      656 2024-06-03 11:23:51.000000 copilothistoryexporter-1.2.2/pyproject.toml
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       38 2024-06-03 11:23:54.561189 copilothistoryexporter-1.2.2/setup.cfg
```

### Comparing `copilothistoryexporter-1.2.1/LICENCE` & `copilothistoryexporter-1.2.2/LICENCE`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.2.1/PKG-INFO` & `copilothistoryexporter-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copilothistoryexporter
-Version: 1.2.1
+Version: 1.2.2
 Summary: Copilot History Exporter
 Author-email: enciyo <enciyomk61@gmail.com>
 Project-URL: Homepage, https://github.com/enciyo/gh-copilot-history-export
 Project-URL: Source, https://github.com/enciyo/gh-copilot-history-export
 Project-URL: Documentation, https://github.com/enciyo/gh-copilot-history-export
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `copilothistoryexporter-1.2.1/README.md` & `copilothistoryexporter-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.2.1/che/binding.py` & `copilothistoryexporter-1.2.2/che/binding.py`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.2.1/che/intercept/chain.py` & `copilothistoryexporter-1.2.2/che/intercept/chain.py`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.2.1/che/intercept/vote.py` & `copilothistoryexporter-1.2.2/che/intercept/vote.py`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.2.1/che/utils.py` & `copilothistoryexporter-1.2.2/che/utils.py`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.2.1/copilothistoryexporter.egg-info/PKG-INFO` & `copilothistoryexporter-1.2.2/copilothistoryexporter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copilothistoryexporter
-Version: 1.2.1
+Version: 1.2.2
 Summary: Copilot History Exporter
 Author-email: enciyo <enciyomk61@gmail.com>
 Project-URL: Homepage, https://github.com/enciyo/gh-copilot-history-export
 Project-URL: Source, https://github.com/enciyo/gh-copilot-history-export
 Project-URL: Documentation, https://github.com/enciyo/gh-copilot-history-export
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `copilothistoryexporter-1.2.1/copilothistoryexporter.egg-info/SOURCES.txt` & `copilothistoryexporter-1.2.2/copilothistoryexporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.2.1/pyproject.toml` & `copilothistoryexporter-1.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "copilothistoryexporter"
 description = "Copilot History Exporter"
-version = "1.2.1"
+version = "1.2.2"
 requires-python = ">=3.11"
 readme = "README.md"
 authors = [{ name = "enciyo", email = "enciyomk61@gmail.com" }]
 
 dependencies = [
     "click~=8.1.7",
     "mitmproxy~=10.3.0"
```

