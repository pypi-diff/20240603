# Comparing `tmp/Agentic-Reports-0.0.5.tar.gz` & `tmp/Agentic-Reports-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Agentic-Reports-0.0.5.tar", last modified: Mon Jun  3 02:27:15 2024, max compression
+gzip compressed data, was "Agentic-Reports-0.0.6.tar", last modified: Mon Jun  3 02:27:40 2024, max compression
```

## Comparing `Agentic-Reports-0.0.5.tar` & `Agentic-Reports-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-06-03 02:27:15.134469 Agentic-Reports-0.0.5/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-06-03 02:27:15.134469 Agentic-Reports-0.0.5/Agentic_Reports.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)     7398 2024-06-03 02:27:15.000000 Agentic-Reports-0.0.5/Agentic_Reports.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      262 2024-06-03 02:27:15.000000 Agentic-Reports-0.0.5/Agentic_Reports.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-06-03 02:27:15.000000 Agentic-Reports-0.0.5/Agentic_Reports.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       47 2024-06-03 02:27:15.000000 Agentic-Reports-0.0.5/Agentic_Reports.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       56 2024-06-03 02:27:15.000000 Agentic-Reports-0.0.5/Agentic_Reports.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-06-03 02:27:15.000000 Agentic-Reports-0.0.5/Agentic_Reports.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1060 2024-06-02 14:41:22.000000 Agentic-Reports-0.0.5/LICENSE
--rw-r--r--   0 codespace  (1000) codespace  (1000)     7398 2024-06-03 02:27:15.134469 Agentic-Reports-0.0.5/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6470 2024-06-03 02:27:00.000000 Agentic-Reports-0.0.5/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-06-03 02:27:15.134469 Agentic-Reports-0.0.5/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1405 2024-06-03 02:27:11.000000 Agentic-Reports-0.0.5/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-06-03 02:27:40.422470 Agentic-Reports-0.0.6/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-06-03 02:27:40.422470 Agentic-Reports-0.0.6/Agentic_Reports.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     7378 2024-06-03 02:27:40.000000 Agentic-Reports-0.0.6/Agentic_Reports.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      262 2024-06-03 02:27:40.000000 Agentic-Reports-0.0.6/Agentic_Reports.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-06-03 02:27:40.000000 Agentic-Reports-0.0.6/Agentic_Reports.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       47 2024-06-03 02:27:40.000000 Agentic-Reports-0.0.6/Agentic_Reports.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       56 2024-06-03 02:27:40.000000 Agentic-Reports-0.0.6/Agentic_Reports.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-06-03 02:27:40.000000 Agentic-Reports-0.0.6/Agentic_Reports.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1060 2024-06-02 14:41:22.000000 Agentic-Reports-0.0.6/LICENSE
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     7378 2024-06-03 02:27:40.422470 Agentic-Reports-0.0.6/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6450 2024-06-03 02:27:30.000000 Agentic-Reports-0.0.6/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-06-03 02:27:40.426470 Agentic-Reports-0.0.6/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1405 2024-06-03 02:27:34.000000 Agentic-Reports-0.0.6/setup.py
```

### Comparing `Agentic-Reports-0.0.5/Agentic_Reports.egg-info/PKG-INFO` & `Agentic-Reports-0.0.6/Agentic_Reports.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Agentic-Reports
-Version: 0.0.5
+Version: 0.0.6
 Summary: Agent Reporting using Exa.ai API.
 Home-page: https://github.com/ruvnet/agentic-reports
 Author: rUv
 Author-email: null@ruv.net
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -22,17 +22,14 @@
 Requires-Dist: wheel
 Requires-Dist: flake8
 Requires-Dist: black
 Requires-Dist: pytest
 Requires-Dist: pip-upgrader
 
 # Agentic Reports
-
-# Agentic Reports
-
 ## A Comprehensive Python Library for Generating Research Reports
 
 Welcome to Agentic Reports, a Python library designed to simplify the process of generating comprehensive research reports. This library leverages the power of FastAPI, Pydantic, Pandas, and Exa to provide users with an efficient and streamlined way to create detailed reports based on various data sources.
 
 ### Technical Overview
 
 Agentic Reports uses a multi-step process to deliver detailed research reports from a variety of sources:
```

### Comparing `Agentic-Reports-0.0.5/LICENSE` & `Agentic-Reports-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Agentic-Reports-0.0.5/PKG-INFO` & `Agentic-Reports-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Agentic-Reports
-Version: 0.0.5
+Version: 0.0.6
 Summary: Agent Reporting using Exa.ai API.
 Home-page: https://github.com/ruvnet/agentic-reports
 Author: rUv
 Author-email: null@ruv.net
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -22,17 +22,14 @@
 Requires-Dist: wheel
 Requires-Dist: flake8
 Requires-Dist: black
 Requires-Dist: pytest
 Requires-Dist: pip-upgrader
 
 # Agentic Reports
-
-# Agentic Reports
-
 ## A Comprehensive Python Library for Generating Research Reports
 
 Welcome to Agentic Reports, a Python library designed to simplify the process of generating comprehensive research reports. This library leverages the power of FastAPI, Pydantic, Pandas, and Exa to provide users with an efficient and streamlined way to create detailed reports based on various data sources.
 
 ### Technical Overview
 
 Agentic Reports uses a multi-step process to deliver detailed research reports from a variety of sources:
```

### Comparing `Agentic-Reports-0.0.5/README.md` & `Agentic-Reports-0.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 # Agentic Reports
-
-# Agentic Reports
-
 ## A Comprehensive Python Library for Generating Research Reports
 
 Welcome to Agentic Reports, a Python library designed to simplify the process of generating comprehensive research reports. This library leverages the power of FastAPI, Pydantic, Pandas, and Exa to provide users with an efficient and streamlined way to create detailed reports based on various data sources.
 
 ### Technical Overview
 
 Agentic Reports uses a multi-step process to deliver detailed research reports from a variety of sources:
```

### Comparing `Agentic-Reports-0.0.5/setup.py` & `Agentic-Reports-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def read_long_description():
     this_directory = Path(__file__).parent
     long_description = (this_directory / "README.md").read_text()
     return long_description
 
 setup(
     name='Agentic-Reports',
-    version='0.0.5',
+    version='0.0.6',
     packages=find_packages(include=['app', 'app.*']),
     install_requires=[
         'twine',
         'setuptools',
         'wheel',
         'flake8',
         'black',
```

