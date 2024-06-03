# Comparing `tmp/Agentic-Reports-0.0.2.tar.gz` & `tmp/Agentic-Reports-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Agentic-Reports-0.0.2.tar", last modified: Mon Jun  3 02:07:51 2024, max compression
+gzip compressed data, was "Agentic-Reports-0.0.4.tar", last modified: Mon Jun  3 02:18:09 2024, max compression
```

## Comparing `Agentic-Reports-0.0.2.tar` & `Agentic-Reports-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-06-03 02:07:51.590410 Agentic-Reports-0.0.2/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-06-03 02:07:51.586410 Agentic-Reports-0.0.2/Agentic_Reports.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)     7063 2024-06-03 02:07:51.000000 Agentic-Reports-0.0.2/Agentic_Reports.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      262 2024-06-03 02:07:51.000000 Agentic-Reports-0.0.2/Agentic_Reports.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-06-03 02:07:51.000000 Agentic-Reports-0.0.2/Agentic_Reports.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       47 2024-06-03 02:07:51.000000 Agentic-Reports-0.0.2/Agentic_Reports.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       56 2024-06-03 02:07:51.000000 Agentic-Reports-0.0.2/Agentic_Reports.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-06-03 02:07:51.000000 Agentic-Reports-0.0.2/Agentic_Reports.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1060 2024-06-02 14:41:22.000000 Agentic-Reports-0.0.2/LICENSE
--rw-r--r--   0 codespace  (1000) codespace  (1000)     7063 2024-06-03 02:07:51.590410 Agentic-Reports-0.0.2/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6136 2024-06-03 02:06:50.000000 Agentic-Reports-0.0.2/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-06-03 02:07:51.590410 Agentic-Reports-0.0.2/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1405 2024-06-03 02:07:45.000000 Agentic-Reports-0.0.2/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-06-03 02:18:09.390441 Agentic-Reports-0.0.4/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-06-03 02:18:09.386441 Agentic-Reports-0.0.4/Agentic_Reports.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     3897 2024-06-03 02:18:09.000000 Agentic-Reports-0.0.4/Agentic_Reports.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      262 2024-06-03 02:18:09.000000 Agentic-Reports-0.0.4/Agentic_Reports.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-06-03 02:18:09.000000 Agentic-Reports-0.0.4/Agentic_Reports.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       47 2024-06-03 02:18:09.000000 Agentic-Reports-0.0.4/Agentic_Reports.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       56 2024-06-03 02:18:09.000000 Agentic-Reports-0.0.4/Agentic_Reports.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-06-03 02:18:09.000000 Agentic-Reports-0.0.4/Agentic_Reports.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1060 2024-06-02 14:41:22.000000 Agentic-Reports-0.0.4/LICENSE
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     3897 2024-06-03 02:18:09.390441 Agentic-Reports-0.0.4/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2969 2024-06-03 02:17:10.000000 Agentic-Reports-0.0.4/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-06-03 02:18:09.390441 Agentic-Reports-0.0.4/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1405 2024-06-03 02:18:03.000000 Agentic-Reports-0.0.4/setup.py
```

### Comparing `Agentic-Reports-0.0.2/LICENSE` & `Agentic-Reports-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Agentic-Reports-0.0.2/setup.py` & `Agentic-Reports-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def read_long_description():
     this_directory = Path(__file__).parent
     long_description = (this_directory / "README.md").read_text()
     return long_description
 
 setup(
     name='Agentic-Reports',
-    version='0.0.2',
+    version='0.0.4',
     packages=find_packages(include=['app', 'app.*']),
     install_requires=[
         'twine',
         'setuptools',
         'wheel',
         'flake8',
         'black',
```

