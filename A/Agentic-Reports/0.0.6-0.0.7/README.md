# Comparing `tmp/Agentic-Reports-0.0.6.tar.gz` & `tmp/Agentic-Reports-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Agentic-Reports-0.0.6.tar", last modified: Mon Jun  3 02:27:40 2024, max compression
+gzip compressed data, was "Agentic-Reports-0.0.7.tar", last modified: Mon Jun  3 02:30:18 2024, max compression
```

## Comparing `Agentic-Reports-0.0.6.tar` & `Agentic-Reports-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-06-03 02:27:40.422470 Agentic-Reports-0.0.6/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-06-03 02:27:40.422470 Agentic-Reports-0.0.6/Agentic_Reports.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)     7378 2024-06-03 02:27:40.000000 Agentic-Reports-0.0.6/Agentic_Reports.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      262 2024-06-03 02:27:40.000000 Agentic-Reports-0.0.6/Agentic_Reports.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-06-03 02:27:40.000000 Agentic-Reports-0.0.6/Agentic_Reports.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       47 2024-06-03 02:27:40.000000 Agentic-Reports-0.0.6/Agentic_Reports.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       56 2024-06-03 02:27:40.000000 Agentic-Reports-0.0.6/Agentic_Reports.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-06-03 02:27:40.000000 Agentic-Reports-0.0.6/Agentic_Reports.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1060 2024-06-02 14:41:22.000000 Agentic-Reports-0.0.6/LICENSE
--rw-r--r--   0 codespace  (1000) codespace  (1000)     7378 2024-06-03 02:27:40.422470 Agentic-Reports-0.0.6/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6450 2024-06-03 02:27:30.000000 Agentic-Reports-0.0.6/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-06-03 02:27:40.426470 Agentic-Reports-0.0.6/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1405 2024-06-03 02:27:34.000000 Agentic-Reports-0.0.6/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-06-03 02:30:18.250478 Agentic-Reports-0.0.7/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-06-03 02:30:18.246478 Agentic-Reports-0.0.7/Agentic_Reports.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)    11998 2024-06-03 02:30:18.000000 Agentic-Reports-0.0.7/Agentic_Reports.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      262 2024-06-03 02:30:18.000000 Agentic-Reports-0.0.7/Agentic_Reports.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-06-03 02:30:18.000000 Agentic-Reports-0.0.7/Agentic_Reports.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       47 2024-06-03 02:30:18.000000 Agentic-Reports-0.0.7/Agentic_Reports.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       56 2024-06-03 02:30:18.000000 Agentic-Reports-0.0.7/Agentic_Reports.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-06-03 02:30:18.000000 Agentic-Reports-0.0.7/Agentic_Reports.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1060 2024-06-02 14:41:22.000000 Agentic-Reports-0.0.7/LICENSE
+-rw-r--r--   0 codespace  (1000) codespace  (1000)    11998 2024-06-03 02:30:18.250478 Agentic-Reports-0.0.7/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11070 2024-06-03 02:30:12.000000 Agentic-Reports-0.0.7/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-06-03 02:30:18.250478 Agentic-Reports-0.0.7/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1405 2024-06-03 02:30:16.000000 Agentic-Reports-0.0.7/setup.py
```

### Comparing `Agentic-Reports-0.0.6/LICENSE` & `Agentic-Reports-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Agentic-Reports-0.0.6/setup.py` & `Agentic-Reports-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def read_long_description():
     this_directory = Path(__file__).parent
     long_description = (this_directory / "README.md").read_text()
     return long_description
 
 setup(
     name='Agentic-Reports',
-    version='0.0.6',
+    version='0.0.7',
     packages=find_packages(include=['app', 'app.*']),
     install_requires=[
         'twine',
         'setuptools',
         'wheel',
         'flake8',
         'black',
```

