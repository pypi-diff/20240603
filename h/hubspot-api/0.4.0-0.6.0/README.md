# Comparing `tmp/hubspot-api-0.4.0.tar.gz` & `tmp/hubspot-api-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hubspot-api-0.4.0.tar", last modified: Mon Feb 26 20:46:20 2024, max compression
+gzip compressed data, was "hubspot-api-0.6.0.tar", last modified: Mon Jun  3 09:39:39 2024, max compression
```

## Comparing `hubspot-api-0.4.0.tar` & `hubspot-api-0.6.0.tar`

### file list

```diff
@@ -1,21 +1,12 @@
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2024-02-26 20:46:20.772601 hubspot-api-0.4.0/
--rw-r--r--   0 erik       (501) staff       (20)     3460 2024-02-26 20:46:20.772464 hubspot-api-0.4.0/PKG-INFO
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2024-02-26 20:46:20.770866 hubspot-api-0.4.0/hubspot_api/
--rw-r--r--   0 erik       (501) staff       (20)      696 2024-02-15 20:26:37.000000 hubspot-api-0.4.0/hubspot_api/__init__.py
--rw-r--r--   0 erik       (501) staff       (20)     2405 2024-02-26 20:43:19.000000 hubspot-api-0.4.0/hubspot_api/api_client.py
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2024-02-26 20:46:20.772236 hubspot-api-0.4.0/hubspot_api/classes/
--rw-r--r--   0 erik       (501) staff       (20)        0 2024-02-06 10:31:42.000000 hubspot-api-0.4.0/hubspot_api/classes/__init__.py
--rw-r--r--   0 erik       (501) staff       (20)     3080 2024-02-26 20:43:36.000000 hubspot-api-0.4.0/hubspot_api/classes/ably.py
--rw-r--r--   0 erik       (501) staff       (20)     1647 2024-02-24 13:46:12.000000 hubspot-api-0.4.0/hubspot_api/classes/agents.py
--rw-r--r--   0 erik       (501) staff       (20)     3319 2024-02-26 20:42:18.000000 hubspot-api-0.4.0/hubspot_api/classes/message.py
--rw-r--r--   0 erik       (501) staff       (20)     8280 2024-02-26 20:12:50.000000 hubspot-api-0.4.0/hubspot_api/classes/threads.py
--rw-r--r--   0 erik       (501) staff       (20)     5598 2024-02-26 12:55:44.000000 hubspot-api-0.4.0/hubspot_api/conversations.py
--rw-r--r--   0 erik       (501) staff       (20)     4236 2024-02-26 20:43:28.000000 hubspot-api-0.4.0/hubspot_api/login.py
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2024-02-26 20:46:20.771532 hubspot-api-0.4.0/hubspot_api.egg-info/
--rw-r--r--   0 erik       (501) staff       (20)     3460 2024-02-26 20:46:20.000000 hubspot-api-0.4.0/hubspot_api.egg-info/PKG-INFO
--rw-r--r--   0 erik       (501) staff       (20)      434 2024-02-26 20:46:20.000000 hubspot-api-0.4.0/hubspot_api.egg-info/SOURCES.txt
--rw-r--r--   0 erik       (501) staff       (20)        1 2024-02-26 20:46:20.000000 hubspot-api-0.4.0/hubspot_api.egg-info/dependency_links.txt
--rw-r--r--   0 erik       (501) staff       (20)        9 2024-02-26 20:46:20.000000 hubspot-api-0.4.0/hubspot_api.egg-info/requires.txt
--rw-r--r--   0 erik       (501) staff       (20)       12 2024-02-26 20:46:20.000000 hubspot-api-0.4.0/hubspot_api.egg-info/top_level.txt
--rw-r--r--   0 erik       (501) staff       (20)       38 2024-02-26 20:46:20.772668 hubspot-api-0.4.0/setup.cfg
--rw-r--r--   0 erik       (501) staff       (20)     1094 2024-02-26 20:45:47.000000 hubspot-api-0.4.0/setup.py
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2024-06-03 09:39:39.150467 hubspot-api-0.6.0/
+-rw-r--r--   0 erik       (501) staff       (20)     3460 2024-06-03 09:39:39.150356 hubspot-api-0.6.0/PKG-INFO
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2024-06-03 09:39:39.149544 hubspot-api-0.6.0/hubspot_api/
+-rw-r--r--   0 erik       (501) staff       (20)     1217 2024-06-03 09:37:44.000000 hubspot-api-0.6.0/hubspot_api/__init__.py
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2024-06-03 09:39:39.150193 hubspot-api-0.6.0/hubspot_api.egg-info/
+-rw-r--r--   0 erik       (501) staff       (20)     3460 2024-06-03 09:39:39.000000 hubspot-api-0.6.0/hubspot_api.egg-info/PKG-INFO
+-rw-r--r--   0 erik       (501) staff       (20)      206 2024-06-03 09:39:39.000000 hubspot-api-0.6.0/hubspot_api.egg-info/SOURCES.txt
+-rw-r--r--   0 erik       (501) staff       (20)        1 2024-06-03 09:39:39.000000 hubspot-api-0.6.0/hubspot_api.egg-info/dependency_links.txt
+-rw-r--r--   0 erik       (501) staff       (20)        9 2024-06-03 09:39:39.000000 hubspot-api-0.6.0/hubspot_api.egg-info/requires.txt
+-rw-r--r--   0 erik       (501) staff       (20)       12 2024-06-03 09:39:39.000000 hubspot-api-0.6.0/hubspot_api.egg-info/top_level.txt
+-rw-r--r--   0 erik       (501) staff       (20)       38 2024-06-03 09:39:39.150507 hubspot-api-0.6.0/setup.cfg
+-rw-r--r--   0 erik       (501) staff       (20)     1094 2024-06-03 09:38:03.000000 hubspot-api-0.6.0/setup.py
```

### Comparing `hubspot-api-0.4.0/PKG-INFO` & `hubspot-api-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubspot-api
-Version: 0.4.0
+Version: 0.6.0
 Summary: Python library to interact with HubSpot's Private API
 Home-page: https://github.com/Erol444/hubspot-api
 Author: Erol444
 Author-email: erol123444@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hubspot-api-0.4.0/hubspot_api.egg-info/PKG-INFO` & `hubspot-api-0.6.0/hubspot_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubspot-api
-Version: 0.4.0
+Version: 0.6.0
 Summary: Python library to interact with HubSpot's Private API
 Home-page: https://github.com/Erol444/hubspot-api
 Author: Erol444
 Author-email: erol123444@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hubspot-api-0.4.0/setup.py` & `hubspot-api-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 root = Path(__file__).parent.resolve()
 readme_file = root / 'readme.md'
 long_description = readme_file.read_text(encoding='utf-8')
 
 setup(
     name="hubspot-api",
-    version="0.4.0",
+    version="0.6.0",
     description="Python library to interact with HubSpot's Private API",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Erol444",
     author_email="erol123444@gmail.com",
     url="https://github.com/Erol444/hubspot-api",
     packages=find_packages(),
```

