# Comparing `tmp/pydnarepeatfinder-0.2.5.tar.gz` & `tmp/pydnarepeatfinder-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydnarepeatfinder-0.2.5.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "pydnarepeatfinder-0.2.6.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `pydnarepeatfinder-0.2.5.tar` & `pydnarepeatfinder-0.2.6.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0      562 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.5/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1184 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.5/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1091 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     3078 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.5/.gitignore
--rw-r--r--   0        0        0      328 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.5/CMakeLists.txt
--rw-r--r--   0        0        0     1068 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.5/LICENSE
--rw-r--r--   0        0        0      303 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.5/README.md
--rw-r--r--   0        0        0      506 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.5/pydna_repeatfinder/__init__.py
--rw-r--r--   0        0        0      125 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.5/pydna_repeatfinder/_version.py
--rw-r--r--   0        0        0     2837 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.5/pydna_repeatfinder/cli.py
--rw-r--r--   0        0        0     1828 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.5/pydna_repeatfinder/colours.py
--rw-r--r--   0        0        0      531 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.5/pydna_repeatfinder/rob_error.py
--rw-r--r--   0        0        0     3503 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.5/pydna_repeatfinder/sequences.py
--rw-r--r--   0        0        0     1309 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     9545 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.5/src/repeatFinder.cpp
--rw-r--r--   0        0        0      538 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.5/src/repeatFinder.h
--rw-r--r--   0        0        0      212 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.5/tests/test.fasta
--rw-r--r--   0        0        0      967 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      562 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.6/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1184 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.6/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1091 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.6/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     3078 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.6/.gitignore
+-rw-r--r--   0        0        0    21622 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.6/.pylintrc
+-rw-r--r--   0        0        0      328 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.6/CMakeLists.txt
+-rw-r--r--   0        0        0     1068 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.6/LICENSE
+-rw-r--r--   0        0        0      303 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.6/README.md
+-rw-r--r--   0        0        0      506 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.6/pydna_repeatfinder/__init__.py
+-rw-r--r--   0        0        0      125 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.6/pydna_repeatfinder/_version.py
+-rw-r--r--   0        0        0     2837 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.6/pydna_repeatfinder/cli.py
+-rw-r--r--   0        0        0     1828 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.6/pydna_repeatfinder/colours.py
+-rw-r--r--   0        0        0      531 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.6/pydna_repeatfinder/rob_error.py
+-rw-r--r--   0        0        0     3503 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.6/pydna_repeatfinder/sequences.py
+-rw-r--r--   0        0        0     1326 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     9545 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.6/src/repeatFinder.cpp
+-rw-r--r--   0        0        0      538 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.6/src/repeatFinder.h
+-rw-r--r--   0        0        0      212 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.6/tests/test.fasta
+-rw-r--r--   0        0        0      967 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.6/PKG-INFO
```

### Comparing `pydnarepeatfinder-0.2.5/.github/workflows/pylint.yml` & `pydnarepeatfinder-0.2.6/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `pydnarepeatfinder-0.2.5/.github/workflows/python-package.yml` & `pydnarepeatfinder-0.2.6/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `pydnarepeatfinder-0.2.5/.github/workflows/python-publish.yml` & `pydnarepeatfinder-0.2.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pydnarepeatfinder-0.2.5/.gitignore` & `pydnarepeatfinder-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pydnarepeatfinder-0.2.5/LICENSE` & `pydnarepeatfinder-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pydnarepeatfinder-0.2.5/pydna_repeatfinder/cli.py` & `pydnarepeatfinder-0.2.6/pydna_repeatfinder/cli.py`

 * *Files identical despite different names*

### Comparing `pydnarepeatfinder-0.2.5/pydna_repeatfinder/colours.py` & `pydnarepeatfinder-0.2.6/pydna_repeatfinder/colours.py`

 * *Files identical despite different names*

### Comparing `pydnarepeatfinder-0.2.5/pydna_repeatfinder/rob_error.py` & `pydnarepeatfinder-0.2.6/pydna_repeatfinder/rob_error.py`

 * *Files identical despite different names*

### Comparing `pydnarepeatfinder-0.2.5/pydna_repeatfinder/sequences.py` & `pydnarepeatfinder-0.2.6/pydna_repeatfinder/sequences.py`

 * *Files identical despite different names*

### Comparing `pydnarepeatfinder-0.2.5/pyproject.toml` & `pydnarepeatfinder-0.2.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["scikit-build-core"]
 build-backend = "scikit_build_core.build"
 
 [project]
 name = "PyDNARepeatFinder"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
   {name = "Rob Edwards", email = "raedwards@gmail.com"}
 ]
 maintainers = [
   {name = "Rob Edwards", email = "raedwards@gmail.com"}
 ]
 
@@ -24,22 +24,22 @@
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: C",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
 ]
 
 [project.scripts]
-pydna_repeatfinder = "pydna_repeatfinder.cli:run"
+pydna_repeatfinder = "PyDNARepeatFinder.cli:run"
 
 [[tool.scikit-build.generate]]
 path = "pydna_repeatfinder/_version.py"
 template = '''
 version = "${version}"
 '''
 
 [tool.scikit-build]
 # Setting py-api to "cp37" would build ABI3 wheels for Python 3.7+.  If CPython
 # is less than this value, or on PyPy, this will be ignored.  Setting the api to
 # "py3" or "py2.py3" would build wheels that don't depend on Python (ctypes,
 # etc).
 # wheel.py-api = "cp37"
-# wheel.packages = []
+wheel.packages = ["pydna_repeatfinder"]
```

### Comparing `pydnarepeatfinder-0.2.5/src/repeatFinder.cpp` & `pydnarepeatfinder-0.2.6/src/repeatFinder.cpp`

 * *Files identical despite different names*

### Comparing `pydnarepeatfinder-0.2.5/src/repeatFinder.h` & `pydnarepeatfinder-0.2.6/src/repeatFinder.h`

 * *Files identical despite different names*

### Comparing `pydnarepeatfinder-0.2.5/PKG-INFO` & `pydnarepeatfinder-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDNARepeatFinder
-Version: 0.2.5
+Version: 0.2.6
 Summary: Rapidly identify repeats in a DNA sequence
 Author-Email: Rob Edwards <raedwards@gmail.com>
 Maintainer-Email: Rob Edwards <raedwards@gmail.com>
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

