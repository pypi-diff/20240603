# Comparing `tmp/copilothistoryexporter-1.1.0.tar.gz` & `tmp/copilothistoryexporter-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copilothistoryexporter-1.1.0.tar", last modified: Mon Jun  3 07:11:15 2024, max compression
+gzip compressed data, was "copilothistoryexporter-1.1.1.tar", last modified: Mon Jun  3 07:20:20 2024, max compression
```

## Comparing `copilothistoryexporter-1.1.0.tar` & `copilothistoryexporter-1.1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 07:11:15.213134 copilothistoryexporter-1.1.0/
--rw-r--r--   0 mustafakilic   (501) staff       (20)     1073 2024-06-01 16:20:49.000000 copilothistoryexporter-1.1.0/LICENCE
--rw-r--r--   0 mustafakilic   (501) staff       (20)     2761 2024-06-03 07:11:15.212929 copilothistoryexporter-1.1.0/PKG-INFO
--rw-r--r--   0 mustafakilic   (501) staff       (20)     2232 2024-06-02 16:13:30.000000 copilothistoryexporter-1.1.0/README.md
--rw-r--r--   0 mustafakilic   (501) staff       (20)      657 2024-06-03 07:00:53.000000 copilothistoryexporter-1.1.0/pyproject.toml
--rw-r--r--   0 mustafakilic   (501) staff       (20)       38 2024-06-03 07:11:15.213172 copilothistoryexporter-1.1.0/setup.cfg
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 07:11:15.210313 copilothistoryexporter-1.1.0/src/
--rw-r--r--   0 mustafakilic   (501) staff       (20)        0 2024-06-03 06:01:46.000000 copilothistoryexporter-1.1.0/src/__init__.py
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 07:11:15.210761 copilothistoryexporter-1.1.0/src/copilothistoryexporter/
--rw-r--r--   0 mustafakilic   (501) staff       (20)        0 2024-06-03 06:01:46.000000 copilothistoryexporter-1.1.0/src/copilothistoryexporter/__init__.py
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 07:11:15.211655 copilothistoryexporter-1.1.0/src/copilothistoryexporter/addons/
--rw-r--r--   0 mustafakilic   (501) staff       (20)        0 2024-06-03 05:45:17.000000 copilothistoryexporter-1.1.0/src/copilothistoryexporter/addons/__init__.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)     1516 2024-06-03 07:04:53.000000 copilothistoryexporter-1.1.0/src/copilothistoryexporter/addons/binding.py
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 07:11:15.212344 copilothistoryexporter-1.1.0/src/copilothistoryexporter/intercp/
--rw-r--r--   0 mustafakilic   (501) staff       (20)        0 2024-06-03 06:01:46.000000 copilothistoryexporter-1.1.0/src/copilothistoryexporter/intercp/__init__.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      517 2024-06-03 07:05:36.000000 copilothistoryexporter-1.1.0/src/copilothistoryexporter/intercp/cache.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      652 2024-06-03 07:05:46.000000 copilothistoryexporter-1.1.0/src/copilothistoryexporter/intercp/chain.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      205 2024-06-03 07:05:50.000000 copilothistoryexporter-1.1.0/src/copilothistoryexporter/intercp/interceptor.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      362 2024-06-03 07:05:56.000000 copilothistoryexporter-1.1.0/src/copilothistoryexporter/intercp/markdown.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      606 2024-06-03 07:06:02.000000 copilothistoryexporter-1.1.0/src/copilothistoryexporter/intercp/vote.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)     1158 2024-06-03 07:06:39.000000 copilothistoryexporter-1.1.0/src/copilothistoryexporter/main.py
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 07:11:15.212583 copilothistoryexporter-1.1.0/src/copilothistoryexporter/model/
--rw-r--r--   0 mustafakilic   (501) staff       (20)      395 2024-06-02 16:13:00.000000 copilothistoryexporter-1.1.0/src/copilothistoryexporter/model/conversation.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      251 2024-06-03 07:06:09.000000 copilothistoryexporter-1.1.0/src/copilothistoryexporter/model/request.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)       92 2024-06-02 16:13:00.000000 copilothistoryexporter-1.1.0/src/copilothistoryexporter/sample.md
--rw-r--r--   0 mustafakilic   (501) staff       (20)     2383 2024-06-03 07:06:54.000000 copilothistoryexporter-1.1.0/src/copilothistoryexporter/utils.py
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 07:11:15.212738 copilothistoryexporter-1.1.0/src/copilothistoryexporter.egg-info/
--rw-r--r--   0 mustafakilic   (501) staff       (20)     2761 2024-06-03 07:11:15.000000 copilothistoryexporter-1.1.0/src/copilothistoryexporter.egg-info/PKG-INFO
--rw-r--r--   0 mustafakilic   (501) staff       (20)      956 2024-06-03 07:11:15.000000 copilothistoryexporter-1.1.0/src/copilothistoryexporter.egg-info/SOURCES.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)        1 2024-06-03 07:11:15.000000 copilothistoryexporter-1.1.0/src/copilothistoryexporter.egg-info/dependency_links.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)       80 2024-06-03 07:11:15.000000 copilothistoryexporter-1.1.0/src/copilothistoryexporter.egg-info/entry_points.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)       25 2024-06-03 07:11:15.000000 copilothistoryexporter-1.1.0/src/copilothistoryexporter.egg-info/requires.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)       32 2024-06-03 07:11:15.000000 copilothistoryexporter-1.1.0/src/copilothistoryexporter.egg-info/top_level.txt
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 07:20:20.203122 copilothistoryexporter-1.1.1/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     1073 2024-06-01 16:20:49.000000 copilothistoryexporter-1.1.1/LICENCE
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     2761 2024-06-03 07:20:20.202944 copilothistoryexporter-1.1.1/PKG-INFO
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     2232 2024-06-02 16:13:30.000000 copilothistoryexporter-1.1.1/README.md
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      657 2024-06-03 07:19:36.000000 copilothistoryexporter-1.1.1/pyproject.toml
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       38 2024-06-03 07:20:20.203160 copilothistoryexporter-1.1.1/setup.cfg
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 07:20:20.200132 copilothistoryexporter-1.1.1/src/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)        0 2024-06-03 06:01:46.000000 copilothistoryexporter-1.1.1/src/__init__.py
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 07:20:20.200587 copilothistoryexporter-1.1.1/src/copilothistoryexporter/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)        0 2024-06-03 06:01:46.000000 copilothistoryexporter-1.1.1/src/copilothistoryexporter/__init__.py
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 07:20:20.201586 copilothistoryexporter-1.1.1/src/copilothistoryexporter/addons/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)        0 2024-06-03 05:45:17.000000 copilothistoryexporter-1.1.1/src/copilothistoryexporter/addons/__init__.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     1516 2024-06-03 07:04:53.000000 copilothistoryexporter-1.1.1/src/copilothistoryexporter/addons/binding.py
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 07:20:20.202320 copilothistoryexporter-1.1.1/src/copilothistoryexporter/intercp/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)        0 2024-06-03 06:01:46.000000 copilothistoryexporter-1.1.1/src/copilothistoryexporter/intercp/__init__.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      517 2024-06-03 07:05:36.000000 copilothistoryexporter-1.1.1/src/copilothistoryexporter/intercp/cache.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      652 2024-06-03 07:05:46.000000 copilothistoryexporter-1.1.1/src/copilothistoryexporter/intercp/chain.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      205 2024-06-03 07:05:50.000000 copilothistoryexporter-1.1.1/src/copilothistoryexporter/intercp/interceptor.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      362 2024-06-03 07:05:56.000000 copilothistoryexporter-1.1.1/src/copilothistoryexporter/intercp/markdown.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      606 2024-06-03 07:06:02.000000 copilothistoryexporter-1.1.1/src/copilothistoryexporter/intercp/vote.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     1158 2024-06-03 07:06:39.000000 copilothistoryexporter-1.1.1/src/copilothistoryexporter/main.py
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 07:20:20.202568 copilothistoryexporter-1.1.1/src/copilothistoryexporter/model/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      395 2024-06-02 16:13:00.000000 copilothistoryexporter-1.1.1/src/copilothistoryexporter/model/conversation.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      251 2024-06-03 07:06:09.000000 copilothistoryexporter-1.1.1/src/copilothistoryexporter/model/request.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       92 2024-06-02 16:13:00.000000 copilothistoryexporter-1.1.1/src/copilothistoryexporter/sample.md
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     2383 2024-06-03 07:06:54.000000 copilothistoryexporter-1.1.1/src/copilothistoryexporter/utils.py
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 07:20:20.202741 copilothistoryexporter-1.1.1/src/copilothistoryexporter.egg-info/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     2761 2024-06-03 07:20:20.000000 copilothistoryexporter-1.1.1/src/copilothistoryexporter.egg-info/PKG-INFO
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      956 2024-06-03 07:20:20.000000 copilothistoryexporter-1.1.1/src/copilothistoryexporter.egg-info/SOURCES.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)        1 2024-06-03 07:20:20.000000 copilothistoryexporter-1.1.1/src/copilothistoryexporter.egg-info/dependency_links.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       80 2024-06-03 07:20:20.000000 copilothistoryexporter-1.1.1/src/copilothistoryexporter.egg-info/entry_points.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       25 2024-06-03 07:20:20.000000 copilothistoryexporter-1.1.1/src/copilothistoryexporter.egg-info/requires.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       32 2024-06-03 07:20:20.000000 copilothistoryexporter-1.1.1/src/copilothistoryexporter.egg-info/top_level.txt
```

### Comparing `copilothistoryexporter-1.1.0/LICENCE` & `copilothistoryexporter-1.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.1.0/PKG-INFO` & `copilothistoryexporter-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: copilothistoryexporter
-Version: 1.1.0
+Version: 1.1.1
 Summary: Copilot History Exporter
 Author-email: enciyo <enciyomk61@gmail.com>
 Project-URL: Homepage, https://github.com/enciyo/gh-copilot-history-export
 Project-URL: Source, https://github.com/enciyo/gh-copilot-history-export
 Project-URL: Documentation, https://github.com/enciyo/gh-copilot-history-export
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENCE
 Requires-Dist: requests
 Requires-Dist: click
 Requires-Dist: mitmproxy
 
 # Github Copilot Chat History Export
```

### Comparing `copilothistoryexporter-1.1.0/README.md` & `copilothistoryexporter-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.1.0/pyproject.toml` & `copilothistoryexporter-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "copilothistoryexporter"
 description = "Copilot History Exporter"
-version = "1.1.0"
-requires-python = ">=3.10"
+version = "1.1.1"
+requires-python = ">=3.11"
 readme = "README.md"
 authors = [{ name = "enciyo", email = "enciyomk61@gmail.com" }]
 
 dependencies = [
     "requests",
     "click",
     "mitmproxy"
```

### Comparing `copilothistoryexporter-1.1.0/src/copilothistoryexporter/addons/binding.py` & `copilothistoryexporter-1.1.1/src/copilothistoryexporter/addons/binding.py`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.1.0/src/copilothistoryexporter/intercp/cache.py` & `copilothistoryexporter-1.1.1/src/copilothistoryexporter/intercp/cache.py`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.1.0/src/copilothistoryexporter/intercp/chain.py` & `copilothistoryexporter-1.1.1/src/copilothistoryexporter/intercp/chain.py`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.1.0/src/copilothistoryexporter/intercp/vote.py` & `copilothistoryexporter-1.1.1/src/copilothistoryexporter/intercp/vote.py`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.1.0/src/copilothistoryexporter/main.py` & `copilothistoryexporter-1.1.1/src/copilothistoryexporter/main.py`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.1.0/src/copilothistoryexporter/utils.py` & `copilothistoryexporter-1.1.1/src/copilothistoryexporter/utils.py`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.1.0/src/copilothistoryexporter.egg-info/PKG-INFO` & `copilothistoryexporter-1.1.1/src/copilothistoryexporter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: copilothistoryexporter
-Version: 1.1.0
+Version: 1.1.1
 Summary: Copilot History Exporter
 Author-email: enciyo <enciyomk61@gmail.com>
 Project-URL: Homepage, https://github.com/enciyo/gh-copilot-history-export
 Project-URL: Source, https://github.com/enciyo/gh-copilot-history-export
 Project-URL: Documentation, https://github.com/enciyo/gh-copilot-history-export
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENCE
 Requires-Dist: requests
 Requires-Dist: click
 Requires-Dist: mitmproxy
 
 # Github Copilot Chat History Export
```

### Comparing `copilothistoryexporter-1.1.0/src/copilothistoryexporter.egg-info/SOURCES.txt` & `copilothistoryexporter-1.1.1/src/copilothistoryexporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

