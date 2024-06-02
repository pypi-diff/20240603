# Comparing `tmp/polylatlib-1.0.2.tar.gz` & `tmp/polylatlib-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polylatlib-1.0.2.tar", max compression
+gzip compressed data, was "polylatlib-1.0.3.tar", max compression
```

## Comparing `polylatlib-1.0.2.tar` & `polylatlib-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1072 2024-02-05 21:50:26.820394 polylatlib-1.0.2/LICENSE
--rw-r--r--   0        0        0      941 2024-02-05 21:50:26.820394 polylatlib-1.0.2/README.md
--rw-r--r--   0        0        0      511 2024-02-05 21:50:26.820394 polylatlib-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      121 2024-02-05 21:50:26.820394 polylatlib-1.0.2/src/polylatlib/__init__.py
--rw-r--r--   0        0        0       81 2024-02-05 21:50:26.820394 polylatlib-1.0.2/src/polylatlib/classes/__init__.py
--rw-r--r--   0        0        0    41080 2024-02-05 21:50:26.820394 polylatlib-1.0.2/src/polylatlib/classes/base_shapes.py
--rw-r--r--   0        0        0     4329 2024-02-05 21:50:26.820394 polylatlib-1.0.2/src/polylatlib/classes/nonregular.py
--rw-r--r--   0        0        0    21954 2024-02-05 21:50:26.820394 polylatlib-1.0.2/src/polylatlib/classes/regular.py
--rw-r--r--   0        0        0     1525 2024-02-05 21:50:26.820394 polylatlib-1.0.2/src/polylatlib/exception.py
--rw-r--r--   0        0        0     1364 2024-02-05 21:50:26.820394 polylatlib-1.0.2/src/polylatlib/functions.py
--rw-r--r--   0        0        0     1770 1970-01-01 00:00:00.000000 polylatlib-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-06-02 23:10:45.265320 polylatlib-1.0.3/LICENSE
+-rw-r--r--   0        0        0      941 2024-06-02 23:10:45.265320 polylatlib-1.0.3/README.md
+-rw-r--r--   0        0        0      511 2024-06-02 23:10:45.265320 polylatlib-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      121 2024-06-02 23:10:45.265320 polylatlib-1.0.3/src/polylatlib/__init__.py
+-rw-r--r--   0        0        0       81 2024-06-02 23:10:45.265320 polylatlib-1.0.3/src/polylatlib/classes/__init__.py
+-rw-r--r--   0        0        0    41080 2024-06-02 23:10:45.265320 polylatlib-1.0.3/src/polylatlib/classes/base_shapes.py
+-rw-r--r--   0        0        0     4329 2024-06-02 23:10:45.265320 polylatlib-1.0.3/src/polylatlib/classes/nonregular.py
+-rw-r--r--   0        0        0    21954 2024-06-02 23:10:45.265320 polylatlib-1.0.3/src/polylatlib/classes/regular.py
+-rw-r--r--   0        0        0     1525 2024-06-02 23:10:45.265320 polylatlib-1.0.3/src/polylatlib/exception.py
+-rw-r--r--   0        0        0     1364 2024-06-02 23:10:45.265320 polylatlib-1.0.3/src/polylatlib/functions.py
+-rw-r--r--   0        0        0     1770 1970-01-01 00:00:00.000000 polylatlib-1.0.3/PKG-INFO
```

### Comparing `polylatlib-1.0.2/LICENSE` & `polylatlib-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `polylatlib-1.0.2/README.md` & `polylatlib-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `polylatlib-1.0.2/src/polylatlib/classes/base_shapes.py` & `polylatlib-1.0.3/src/polylatlib/classes/base_shapes.py`

 * *Files identical despite different names*

### Comparing `polylatlib-1.0.2/src/polylatlib/classes/nonregular.py` & `polylatlib-1.0.3/src/polylatlib/classes/nonregular.py`

 * *Files identical despite different names*

### Comparing `polylatlib-1.0.2/src/polylatlib/classes/regular.py` & `polylatlib-1.0.3/src/polylatlib/classes/regular.py`

 * *Files identical despite different names*

### Comparing `polylatlib-1.0.2/src/polylatlib/exception.py` & `polylatlib-1.0.3/src/polylatlib/exception.py`

 * *Files identical despite different names*

### Comparing `polylatlib-1.0.2/src/polylatlib/functions.py` & `polylatlib-1.0.3/src/polylatlib/functions.py`

 * *Files identical despite different names*

### Comparing `polylatlib-1.0.2/PKG-INFO` & `polylatlib-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: polylatlib
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python library providing the functionality to generate, work with, view, and manipulate polygons and their lattices in the 2D space.
-Home-page: https://github.com/RexGreenway/PolyLatLib
+Home-page: https://github.com/rexgreenway/polylatlib
 License: GPL-3.0-or-later
 Author: Rex Greenway
-Author-email: rexgreenway@gmail.com
+Author-email: rexgreenway@proton.me
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: matplotlib (>=3.8.2,<4.0.0)
-Project-URL: Repository, https://github.com/RexGreenway/PolyLatLib
+Project-URL: Repository, https://github.com/rexgreenway/polylatlib
 Description-Content-Type: text/markdown
 
 PolyLatLib
 =================
 By Rex Greenway
 
 This project aims to allow for the investigation of shapes in the R x R Cartesian Plane and their lattices. This Python library provides the functionality to generate, work with, view, and manipulate polygons in the 2D space and, for applciable shapes, generate the corresponding lattice.
```

