# Comparing `tmp/graphclass-0.0.21.tar.gz` & `tmp/graphclass-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphclass-0.0.21.tar", last modified: Mon Jun  3 10:02:03 2024, max compression
+gzip compressed data, was "graphclass-0.0.23.tar", last modified: Mon Jun  3 11:43:33 2024, max compression
```

## Comparing `graphclass-0.0.21.tar` & `graphclass-0.0.23.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:02:03.179946 graphclass-0.0.21/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:02:03.175945 graphclass-0.0.21/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:02:03.175945 graphclass-0.0.21/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-06-03 10:01:52.000000 graphclass-0.0.21/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-06-03 10:01:52.000000 graphclass-0.0.21/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-06-03 10:01:52.000000 graphclass-0.0.21/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-06-03 10:02:03.179946 graphclass-0.0.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-06-03 10:01:52.000000 graphclass-0.0.21/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:02:03.175945 graphclass-0.0.21/doc/
--rw-r--r--   0 runner    (1001) docker     (127)    34662 2024-06-03 10:01:52.000000 graphclass-0.0.21/doc/GraphDemo.png
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-06-03 10:01:52.000000 graphclass-0.0.21/doc/GraphDemo.py
--rw-r--r--   0 runner    (1001) docker     (127)   105831 2024-06-03 10:01:52.000000 graphclass-0.0.21/doc/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-06-03 10:01:52.000000 graphclass-0.0.21/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 10:02:03.179946 graphclass-0.0.21/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:02:03.175945 graphclass-0.0.21/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:02:03.175945 graphclass-0.0.21/src/drawing/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-06-03 10:01:52.000000 graphclass-0.0.21/src/drawing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-06-03 10:02:03.000000 graphclass-0.0.21/src/drawing/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5700 2024-06-03 10:01:52.000000 graphclass-0.0.21/src/drawing/drawing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:02:03.179946 graphclass-0.0.21/src/graphclass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-06-03 10:02:03.000000 graphclass-0.0.21/src/graphclass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-06-03 10:02:03.000000 graphclass-0.0.21/src/graphclass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 10:02:03.000000 graphclass-0.0.21/src/graphclass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-03 10:02:03.000000 graphclass-0.0.21/src/graphclass.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:43:33.941732 graphclass-0.0.23/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:43:33.937732 graphclass-0.0.23/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:43:33.941732 graphclass-0.0.23/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-06-03 11:43:23.000000 graphclass-0.0.23/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-03 11:43:23.000000 graphclass-0.0.23/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-06-03 11:43:23.000000 graphclass-0.0.23/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-06-03 11:43:33.941732 graphclass-0.0.23/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-06-03 11:43:23.000000 graphclass-0.0.23/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:43:33.941732 graphclass-0.0.23/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)    34662 2024-06-03 11:43:23.000000 graphclass-0.0.23/doc/GraphDemo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-06-03 11:43:23.000000 graphclass-0.0.23/doc/GraphDemo.py
+-rw-r--r--   0 runner    (1001) docker     (127)   105831 2024-06-03 11:43:23.000000 graphclass-0.0.23/doc/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-06-03 11:43:23.000000 graphclass-0.0.23/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 11:43:33.941732 graphclass-0.0.23/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:43:33.941732 graphclass-0.0.23/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:43:33.941732 graphclass-0.0.23/src/graphclass/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-06-03 11:43:23.000000 graphclass-0.0.23/src/graphclass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-06-03 11:43:33.000000 graphclass-0.0.23/src/graphclass/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5700 2024-06-03 11:43:23.000000 graphclass-0.0.23/src/graphclass/graphclass.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:43:33.941732 graphclass-0.0.23/src/graphclass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-06-03 11:43:33.000000 graphclass-0.0.23/src/graphclass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-06-03 11:43:33.000000 graphclass-0.0.23/src/graphclass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 11:43:33.000000 graphclass-0.0.23/src/graphclass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-03 11:43:33.000000 graphclass-0.0.23/src/graphclass.egg-info/top_level.txt
```

### Comparing `graphclass-0.0.21/.github/workflows/publish.yml` & `graphclass-0.0.23/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `graphclass-0.0.21/LICENSE` & `graphclass-0.0.23/LICENSE`

 * *Files identical despite different names*

### Comparing `graphclass-0.0.21/PKG-INFO` & `graphclass-0.0.23/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,17 @@
-Metadata-Version: 2.1
-Name: graphclass
-Version: 0.0.21
-Summary: Drawing graphs by graphviz with class approach
-Author-email: nummulith <nummulith@gmail.com>
-License: MIT
-Project-URL: Homepage, https://github.com/nummulith/drawing
-Keywords: drawing,graph,graphviz
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [ReadMe.md](../ReadMe.md) \ [Graph Drawing Utility](Graph_Drawing_Utility.md)
 
 <table style="width: 100%">
   <thead>
     <tr>
         <th>
             <h1>Graph Drawing Utility</h1>
         </th>
         <th>
-            <img src="https://raw.githubusercontent.com/Nummulith/drawing/main/doc/logo.png" width="100" height="100">
+            <img src="https://raw.githubusercontent.com/Nummulith/graphclass/main/doc/logo.png" width="100" height="100">
         </th>
     </tr>
   </thead>
 </table>
 
 ## Overview
 The **Graph Drawing Utility** project provides a versatile tool for visualizing object relationships. This utility is designed to be seamlessly integrated into projects, allowing users to dynamically represent and explore the connections between objects.
@@ -44,10 +29,10 @@
 add_link: Creates a connection between objects using arrows.
 
 ## Graph Rendering:
 The utility enables users to visualize the constructed object graph, providing a clear representation of the established relationships.
 
 ## Example
 
-[Source code](https://raw.githubusercontent.com/Nummulith/drawing/main/doc/GraphDemo.py)
+[Source code](https://raw.githubusercontent.com/Nummulith/graphclass/main/doc/GraphDemo.py)
 
-<img src="https://raw.githubusercontent.com/Nummulith/drawing/main/doc/GraphDemo.png">
+<img src="https://raw.githubusercontent.com/Nummulith/graphclass/main/doc/GraphDemo.png">
```

#### html2text {}

```diff
@@ -1,25 +1,18 @@
-Metadata-Version: 2.1 Name: graphclass Version: 0.0.21 Summary: Drawing graphs
-by graphviz with class approach Author-email: nummulith
-gmail.com> License: MIT Project-URL: Homepage, https://github.com/nummulith/
-drawing Keywords: drawing,graph,graphviz Classifier: Programming Language ::
-Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
-Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
-Type: text/markdown License-File: LICENSE [ReadMe.md](../ReadMe.md) \ [Graph
-Drawing Utility](Graph_Drawing_Utility.md)
+[ReadMe.md](../ReadMe.md) \ [Graph Drawing Utility](Graph_Drawing_Utility.md)
 ************ GGrraapphh DDrraawwiinngg UUttiilliittyy ************ [[hhttttppss::////rraaww..ggiitthhuubbuusseerrccoonntteenntt..ccoomm//
-                                    NNuummmmuulliitthh//ddrraawwiinngg//mmaaiinn//ddoocc//llooggoo..ppnngg]]
+                                    NNuummmmuulliitthh//ggrraapphhccllaassss//mmaaiinn//ddoocc//llooggoo..ppnngg]]
 ## Overview The **Graph Drawing Utility** project provides a versatile tool for
 visualizing object relationships. This utility is designed to be seamlessly
 integrated into projects, allowing users to dynamically represent and explore
 the connections between objects. ## Adding objects Users can add objects to the
 graph using the add_item method. ## Adding views The item_view method provides
 a means to inspect the details of individual objects, facilitating a deeper
 understanding of the interconnected elements. Relationship Establishment: ##
 Adding relations Users can establish relationships between objects using three
 types: add_parent: Defines an ownership relationship, clustering owned objects
 together. add_link: Creates a connection between objects using arrows. ## Graph
 Rendering: The utility enables users to visualize the constructed object graph,
 providing a clear representation of the established relationships. ## Example
-[Source code](https://raw.githubusercontent.com/Nummulith/drawing/main/doc/
-GraphDemo.py)[https://raw.githubusercontent.com/Nummulith/drawing/main/doc/
+[Source code](https://raw.githubusercontent.com/Nummulith/graphclass/main/doc/
+GraphDemo.py)[https://raw.githubusercontent.com/Nummulith/graphclass/main/doc/
 GraphDemo.png]
```

### Comparing `graphclass-0.0.21/doc/GraphDemo.png` & `graphclass-0.0.23/doc/GraphDemo.png`

 * *Files identical despite different names*

### Comparing `graphclass-0.0.21/doc/GraphDemo.py` & `graphclass-0.0.23/doc/GraphDemo.py`

 * *Files identical despite different names*

### Comparing `graphclass-0.0.21/doc/logo.png` & `graphclass-0.0.23/doc/logo.png`

 * *Files identical despite different names*

### Comparing `graphclass-0.0.21/pyproject.toml` & `graphclass-0.0.23/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -16,11 +16,11 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/nummulith/drawing"
+"Homepage" = "https://github.com/nummulith/graphclass"
 
 [tool.setuptools_scm]
-write_to = "src/drawing/_version.py"
+write_to = "src/graphclass/_version.py"
```

### Comparing `graphclass-0.0.21/src/drawing/drawing.py` & `graphclass-0.0.23/src/graphclass/graphclass.py`

 * *Files identical despite different names*

