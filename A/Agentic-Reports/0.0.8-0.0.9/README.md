# Comparing `tmp/Agentic-Reports-0.0.8.tar.gz` & `tmp/Agentic-Reports-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Agentic-Reports-0.0.8.tar", last modified: Mon Jun  3 02:32:02 2024, max compression
+gzip compressed data, was "Agentic-Reports-0.0.9.tar", last modified: Mon Jun  3 02:40:52 2024, max compression
```

## Comparing `Agentic-Reports-0.0.8.tar` & `Agentic-Reports-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-06-03 02:32:02.882483 Agentic-Reports-0.0.8/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-06-03 02:32:02.882483 Agentic-Reports-0.0.8/Agentic_Reports.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)    12387 2024-06-03 02:32:02.000000 Agentic-Reports-0.0.8/Agentic_Reports.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      262 2024-06-03 02:32:02.000000 Agentic-Reports-0.0.8/Agentic_Reports.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-06-03 02:32:02.000000 Agentic-Reports-0.0.8/Agentic_Reports.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       47 2024-06-03 02:32:02.000000 Agentic-Reports-0.0.8/Agentic_Reports.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       56 2024-06-03 02:32:02.000000 Agentic-Reports-0.0.8/Agentic_Reports.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-06-03 02:32:02.000000 Agentic-Reports-0.0.8/Agentic_Reports.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1060 2024-06-02 14:41:22.000000 Agentic-Reports-0.0.8/LICENSE
--rw-r--r--   0 codespace  (1000) codespace  (1000)    12387 2024-06-03 02:32:02.882483 Agentic-Reports-0.0.8/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11459 2024-06-03 02:31:55.000000 Agentic-Reports-0.0.8/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-06-03 02:32:02.882483 Agentic-Reports-0.0.8/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1405 2024-06-03 02:31:59.000000 Agentic-Reports-0.0.8/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-06-03 02:40:52.766510 Agentic-Reports-0.0.9/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-06-03 02:40:52.758510 Agentic-Reports-0.0.9/Agentic_Reports.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)    12387 2024-06-03 02:40:52.000000 Agentic-Reports-0.0.9/Agentic_Reports.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      262 2024-06-03 02:40:52.000000 Agentic-Reports-0.0.9/Agentic_Reports.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-06-03 02:40:52.000000 Agentic-Reports-0.0.9/Agentic_Reports.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       47 2024-06-03 02:40:52.000000 Agentic-Reports-0.0.9/Agentic_Reports.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       56 2024-06-03 02:40:52.000000 Agentic-Reports-0.0.9/Agentic_Reports.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-06-03 02:40:52.000000 Agentic-Reports-0.0.9/Agentic_Reports.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1060 2024-06-02 14:41:22.000000 Agentic-Reports-0.0.9/LICENSE
+-rw-r--r--   0 codespace  (1000) codespace  (1000)    12387 2024-06-03 02:40:52.766510 Agentic-Reports-0.0.9/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11459 2024-06-03 02:31:55.000000 Agentic-Reports-0.0.9/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-06-03 02:40:52.766510 Agentic-Reports-0.0.9/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1405 2024-06-03 02:40:48.000000 Agentic-Reports-0.0.9/setup.py
```

### Comparing `Agentic-Reports-0.0.8/Agentic_Reports.egg-info/PKG-INFO` & `Agentic-Reports-0.0.9/Agentic_Reports.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Agentic-Reports
-Version: 0.0.8
+Version: 0.0.9
 Summary: Agent Reporting using Exa.ai API.
 Home-page: https://github.com/ruvnet/agentic-reports
 Author: rUv
 Author-email: null@ruv.net
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `Agentic-Reports-0.0.8/LICENSE` & `Agentic-Reports-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Agentic-Reports-0.0.8/PKG-INFO` & `Agentic-Reports-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Agentic-Reports
-Version: 0.0.8
+Version: 0.0.9
 Summary: Agent Reporting using Exa.ai API.
 Home-page: https://github.com/ruvnet/agentic-reports
 Author: rUv
 Author-email: null@ruv.net
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `Agentic-Reports-0.0.8/README.md` & `Agentic-Reports-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `Agentic-Reports-0.0.8/setup.py` & `Agentic-Reports-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def read_long_description():
     this_directory = Path(__file__).parent
     long_description = (this_directory / "README.md").read_text()
     return long_description
 
 setup(
     name='Agentic-Reports',
-    version='0.0.8',
+    version='0.0.9',
     packages=find_packages(include=['app', 'app.*']),
     install_requires=[
         'twine',
         'setuptools',
         'wheel',
         'flake8',
         'black',
```

