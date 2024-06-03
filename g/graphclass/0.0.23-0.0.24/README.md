# Comparing `tmp/graphclass-0.0.23.tar.gz` & `tmp/graphclass-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphclass-0.0.23.tar", last modified: Mon Jun  3 11:43:33 2024, max compression
+gzip compressed data, was "graphclass-0.0.24.tar", last modified: Mon Jun  3 11:58:22 2024, max compression
```

## Comparing `graphclass-0.0.23.tar` & `graphclass-0.0.24.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:43:33.941732 graphclass-0.0.23/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:43:33.937732 graphclass-0.0.23/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:43:33.941732 graphclass-0.0.23/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-06-03 11:43:23.000000 graphclass-0.0.23/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-03 11:43:23.000000 graphclass-0.0.23/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-06-03 11:43:23.000000 graphclass-0.0.23/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-06-03 11:43:33.941732 graphclass-0.0.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-06-03 11:43:23.000000 graphclass-0.0.23/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:43:33.941732 graphclass-0.0.23/doc/
--rw-r--r--   0 runner    (1001) docker     (127)    34662 2024-06-03 11:43:23.000000 graphclass-0.0.23/doc/GraphDemo.png
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-06-03 11:43:23.000000 graphclass-0.0.23/doc/GraphDemo.py
--rw-r--r--   0 runner    (1001) docker     (127)   105831 2024-06-03 11:43:23.000000 graphclass-0.0.23/doc/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-06-03 11:43:23.000000 graphclass-0.0.23/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 11:43:33.941732 graphclass-0.0.23/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:43:33.941732 graphclass-0.0.23/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:43:33.941732 graphclass-0.0.23/src/graphclass/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-06-03 11:43:23.000000 graphclass-0.0.23/src/graphclass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-06-03 11:43:33.000000 graphclass-0.0.23/src/graphclass/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5700 2024-06-03 11:43:23.000000 graphclass-0.0.23/src/graphclass/graphclass.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:43:33.941732 graphclass-0.0.23/src/graphclass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-06-03 11:43:33.000000 graphclass-0.0.23/src/graphclass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-06-03 11:43:33.000000 graphclass-0.0.23/src/graphclass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 11:43:33.000000 graphclass-0.0.23/src/graphclass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-03 11:43:33.000000 graphclass-0.0.23/src/graphclass.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:58:22.666782 graphclass-0.0.24/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:58:22.662782 graphclass-0.0.24/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:58:22.666782 graphclass-0.0.24/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-06-03 11:58:12.000000 graphclass-0.0.24/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-03 11:58:12.000000 graphclass-0.0.24/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-06-03 11:58:12.000000 graphclass-0.0.24/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-06-03 11:58:22.666782 graphclass-0.0.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-06-03 11:58:12.000000 graphclass-0.0.24/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:58:22.666782 graphclass-0.0.24/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)    34662 2024-06-03 11:58:12.000000 graphclass-0.0.24/doc/GraphDemo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-06-03 11:58:12.000000 graphclass-0.0.24/doc/GraphDemo.py
+-rw-r--r--   0 runner    (1001) docker     (127)   105831 2024-06-03 11:58:12.000000 graphclass-0.0.24/doc/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-06-03 11:58:12.000000 graphclass-0.0.24/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 11:58:22.666782 graphclass-0.0.24/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:58:22.662782 graphclass-0.0.24/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:58:22.666782 graphclass-0.0.24/src/graphclass/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-06-03 11:58:12.000000 graphclass-0.0.24/src/graphclass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-06-03 11:58:22.000000 graphclass-0.0.24/src/graphclass/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5700 2024-06-03 11:58:12.000000 graphclass-0.0.24/src/graphclass/graphclass.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:58:22.666782 graphclass-0.0.24/src/graphclass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-06-03 11:58:22.000000 graphclass-0.0.24/src/graphclass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-06-03 11:58:22.000000 graphclass-0.0.24/src/graphclass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 11:58:22.000000 graphclass-0.0.24/src/graphclass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-03 11:58:22.000000 graphclass-0.0.24/src/graphclass.egg-info/top_level.txt
```

### Comparing `graphclass-0.0.23/.github/workflows/publish.yml` & `graphclass-0.0.24/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `graphclass-0.0.23/LICENSE` & `graphclass-0.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `graphclass-0.0.23/PKG-INFO` & `graphclass-0.0.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphclass
-Version: 0.0.23
+Version: 0.0.24
 Summary: Drawing graphs by graphviz with class approach
 Author-email: nummulith <nummulith@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/nummulith/graphclass
 Keywords: drawing,graph,graphviz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: graphclass Version: 0.0.23 Summary: Drawing graphs
+Metadata-Version: 2.1 Name: graphclass Version: 0.0.24 Summary: Drawing graphs
 by graphviz with class approach Author-email: nummulith
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/nummulith/
 graphclass Keywords: drawing,graph,graphviz Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE [ReadMe.md](../ReadMe.md) \ [Graph
 Drawing Utility](Graph_Drawing_Utility.md)
```

### Comparing `graphclass-0.0.23/README.md` & `graphclass-0.0.24/README.md`

 * *Files identical despite different names*

### Comparing `graphclass-0.0.23/doc/GraphDemo.png` & `graphclass-0.0.24/doc/GraphDemo.png`

 * *Files identical despite different names*

### Comparing `graphclass-0.0.23/doc/GraphDemo.py` & `graphclass-0.0.24/doc/GraphDemo.py`

 * *Files identical despite different names*

### Comparing `graphclass-0.0.23/doc/logo.png` & `graphclass-0.0.24/doc/logo.png`

 * *Files identical despite different names*

### Comparing `graphclass-0.0.23/pyproject.toml` & `graphclass-0.0.24/pyproject.toml`

 * *Files identical despite different names*

### Comparing `graphclass-0.0.23/src/graphclass/graphclass.py` & `graphclass-0.0.24/src/graphclass/graphclass.py`

 * *Files identical despite different names*

### Comparing `graphclass-0.0.23/src/graphclass.egg-info/PKG-INFO` & `graphclass-0.0.24/src/graphclass.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphclass
-Version: 0.0.23
+Version: 0.0.24
 Summary: Drawing graphs by graphviz with class approach
 Author-email: nummulith <nummulith@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/nummulith/graphclass
 Keywords: drawing,graph,graphviz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: graphclass Version: 0.0.23 Summary: Drawing graphs
+Metadata-Version: 2.1 Name: graphclass Version: 0.0.24 Summary: Drawing graphs
 by graphviz with class approach Author-email: nummulith
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/nummulith/
 graphclass Keywords: drawing,graph,graphviz Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE [ReadMe.md](../ReadMe.md) \ [Graph
 Drawing Utility](Graph_Drawing_Utility.md)
```

