# Comparing `tmp/pyslsqp-0.1.0a0.tar.gz` & `tmp/pyslsqp-0.1.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyslsqp-0.1.0a0.tar", last modified: Sun Jun  2 00:36:50 2024, max compression
+gzip compressed data, was "pyslsqp-0.1.0b0.tar", last modified: Sun Jun  2 01:08:57 2024, max compression
```

## Comparing `pyslsqp-0.1.0a0.tar` & `pyslsqp-0.1.0b0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:36:50.344170 pyslsqp-0.1.0a0/
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-06-02 00:36:50.344170 pyslsqp-0.1.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:36:50.340170 pyslsqp-0.1.0a0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:36:50.340170 pyslsqp-0.1.0a0/docs/src/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/docs/src/api.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:36:50.340170 pyslsqp-0.1.0a0/docs/src/api_pages/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/docs/src/api_pages/optimize.md
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/docs/src/api_pages/postprocessing.md
--rw-r--r--   0 runner    (1001) docker     (127)   230110 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/docs/src/basic.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/docs/src/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/docs/src/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/docs/src/getting_started.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:36:50.340170 pyslsqp-0.1.0a0/docs/src/images/
--rw-r--r--   0 runner    (1001) docker     (127)   274879 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/docs/src/images/lsdolab.png
--rw-r--r--   0 runner    (1001) docker     (127)   944007 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/docs/src/images/lsdolab_website.png
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/docs/src/license.md
--rw-r--r--   0 runner    (1001) docker     (127)   141033 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/docs/src/postprocessing.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/docs/src/references.bib
--rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/docs/src/welcome.md
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/meson.build
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:36:50.344170 pyslsqp-0.1.0a0/pyslsqp/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/pyslsqp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46786 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/pyslsqp/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/pyslsqp/meson.build
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/pyslsqp/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    17620 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/pyslsqp/save_and_load.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:36:50.344170 pyslsqp-0.1.0a0/pyslsqp/slsqp/
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/pyslsqp/slsqp/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/pyslsqp/slsqp/slsqp.pyf
--rw-r--r--   0 runner    (1001) docker     (127)    69941 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/pyslsqp/slsqp/slsqp_optmz.f
--rw-r--r--   0 runner    (1001) docker     (127)    10879 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/pyslsqp/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:36:50.344170 pyslsqp-0.1.0a0/pyslsqp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-06-02 00:36:50.000000 pyslsqp-0.1.0a0/pyslsqp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-06-02 00:36:50.000000 pyslsqp-0.1.0a0/pyslsqp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 00:36:50.000000 pyslsqp-0.1.0a0/pyslsqp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-06-02 00:36:50.000000 pyslsqp-0.1.0a0/pyslsqp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-06-02 00:36:50.000000 pyslsqp-0.1.0a0/pyslsqp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 00:36:50.344170 pyslsqp-0.1.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:36:50.344170 pyslsqp-0.1.0a0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/tests/test_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/tests/test_docstring_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)    15734 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/tests/test_optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/tests/test_save_and_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/tests/testing_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 01:08:57.300764 pyslsqp-0.1.0b0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-06-02 01:08:51.000000 pyslsqp-0.1.0b0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-06-02 01:08:51.000000 pyslsqp-0.1.0b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11031 2024-06-02 01:08:57.300764 pyslsqp-0.1.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7575 2024-06-02 01:08:51.000000 pyslsqp-0.1.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 01:08:57.296764 pyslsqp-0.1.0b0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-06-02 01:08:51.000000 pyslsqp-0.1.0b0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-06-02 01:08:51.000000 pyslsqp-0.1.0b0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-06-02 01:08:51.000000 pyslsqp-0.1.0b0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-06-02 01:08:51.000000 pyslsqp-0.1.0b0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 01:08:57.296764 pyslsqp-0.1.0b0/docs/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-06-02 01:08:51.000000 pyslsqp-0.1.0b0/docs/src/api.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 01:08:57.296764 pyslsqp-0.1.0b0/docs/src/api_pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-06-02 01:08:51.000000 pyslsqp-0.1.0b0/docs/src/api_pages/optimize.md
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-06-02 01:08:51.000000 pyslsqp-0.1.0b0/docs/src/api_pages/postprocessing.md
+-rw-r--r--   0 runner    (1001) docker     (127)   230110 2024-06-02 01:08:51.000000 pyslsqp-0.1.0b0/docs/src/basic.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-06-02 01:08:51.000000 pyslsqp-0.1.0b0/docs/src/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 01:08:51.000000 pyslsqp-0.1.0b0/docs/src/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-06-02 01:08:51.000000 pyslsqp-0.1.0b0/docs/src/getting_started.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 01:08:57.296764 pyslsqp-0.1.0b0/docs/src/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   274879 2024-06-02 01:08:51.000000 pyslsqp-0.1.0b0/docs/src/images/lsdolab.png
+-rw-r--r--   0 runner    (1001) docker     (127)   944007 2024-06-02 01:08:51.000000 pyslsqp-0.1.0b0/docs/src/images/lsdolab_website.png
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-06-02 01:08:51.000000 pyslsqp-0.1.0b0/docs/src/license.md
+-rw-r--r--   0 runner    (1001) docker     (127)   141033 2024-06-02 01:08:51.000000 pyslsqp-0.1.0b0/docs/src/postprocessing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-06-02 01:08:51.000000 pyslsqp-0.1.0b0/docs/src/references.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-06-02 01:08:51.000000 pyslsqp-0.1.0b0/docs/src/welcome.md
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-06-02 01:08:51.000000 pyslsqp-0.1.0b0/meson.build
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-06-02 01:08:51.000000 pyslsqp-0.1.0b0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 01:08:57.300764 pyslsqp-0.1.0b0/pyslsqp/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-06-02 01:08:51.000000 pyslsqp-0.1.0b0/pyslsqp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46786 2024-06-02 01:08:51.000000 pyslsqp-0.1.0b0/pyslsqp/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-06-02 01:08:51.000000 pyslsqp-0.1.0b0/pyslsqp/meson.build
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-06-02 01:08:51.000000 pyslsqp-0.1.0b0/pyslsqp/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17620 2024-06-02 01:08:51.000000 pyslsqp-0.1.0b0/pyslsqp/save_and_load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 01:08:57.300764 pyslsqp-0.1.0b0/pyslsqp/slsqp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-06-02 01:08:51.000000 pyslsqp-0.1.0b0/pyslsqp/slsqp/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-06-02 01:08:51.000000 pyslsqp-0.1.0b0/pyslsqp/slsqp/slsqp.pyf
+-rw-r--r--   0 runner    (1001) docker     (127)    69941 2024-06-02 01:08:51.000000 pyslsqp-0.1.0b0/pyslsqp/slsqp/slsqp_optmz.f
+-rw-r--r--   0 runner    (1001) docker     (127)    10879 2024-06-02 01:08:51.000000 pyslsqp-0.1.0b0/pyslsqp/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 01:08:57.300764 pyslsqp-0.1.0b0/pyslsqp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11031 2024-06-02 01:08:57.000000 pyslsqp-0.1.0b0/pyslsqp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-06-02 01:08:57.000000 pyslsqp-0.1.0b0/pyslsqp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 01:08:57.000000 pyslsqp-0.1.0b0/pyslsqp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-06-02 01:08:57.000000 pyslsqp-0.1.0b0/pyslsqp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-06-02 01:08:57.000000 pyslsqp-0.1.0b0/pyslsqp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 01:08:57.300764 pyslsqp-0.1.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-06-02 01:08:51.000000 pyslsqp-0.1.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 01:08:57.300764 pyslsqp-0.1.0b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-06-02 01:08:51.000000 pyslsqp-0.1.0b0/tests/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-06-02 01:08:51.000000 pyslsqp-0.1.0b0/tests/test_docstring_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15734 2024-06-02 01:08:51.000000 pyslsqp-0.1.0b0/tests/test_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-06-02 01:08:51.000000 pyslsqp-0.1.0b0/tests/test_save_and_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-06-02 01:08:51.000000 pyslsqp-0.1.0b0/tests/testing_utils.py
```

### Comparing `pyslsqp-0.1.0a0/LICENSE.txt` & `pyslsqp-0.1.0b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0a0/PKG-INFO` & `pyslsqp-0.1.0b0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslsqp
-Version: 0.1.0a0
+Version: 0.1.0b0
 Summary: A transparent Python interface to the SLSQP optimization algorithm, with advanced features and visualization capabilities.
 Author-email: Anugrah Jo Joshy <ajoshy.ucsd@gmail.com>
 Maintainer-email: Anugrah Jo Joshy <ajoshy.ucsd@gmail.com>
 License: Copyright (c) 2024, Anugrah Jo Joshy.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -70,17 +70,18 @@
 [![Pypi](https://img.shields.io/pypi/v/PySLSQP)](https://pypi.org/project/PySLSQP/)
 [![PyPI version][10]][11]
 [![PyPI Monthly Downloads][12]][11]
 -->
 
 [![GitHub Actions Test Badge](https://github.com/anugrahjo/PySLSQP/actions/workflows/build_install_test.yml/badge.svg)](https://github.com/anugrahjo/PySLSQP/actions)
 [![Coverage Status](https://coveralls.io/repos/github/anugrahjo/PySLSQP/badge.svg?branch=main)](https://coveralls.io/github/anugrahjo/PySLSQP?branch=main)
+[![Documentation Status](https://readthedocs.org/projects/pyslsqp/badge/?version=latest)](https://pyslsqp.readthedocs.io/en/latest/?badge=main)
 [![Pypi version](https://img.shields.io/pypi/v/pyslsqp)](https://pypi.org/project/pyslsqp/)
-[![Forks](https://img.shields.io/github/forks/anugrahjo/PySLSQP.svg)](https://github.com/anugrahjo/PySLSQP/network)
-[![Issues](https://img.shields.io/github/issues/anugrahjo/PySLSQP.svg)](https://github.com/anugrahjo/PySLSQP/issues)
+<!-- [![Forks](https://img.shields.io/github/forks/anugrahjo/PySLSQP.svg)](https://github.com/anugrahjo/PySLSQP/network) -->
+<!-- [![Issues](https://img.shields.io/github/issues/anugrahjo/PySLSQP.svg)](https://github.com/anugrahjo/PySLSQP/issues) -->
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://github.com/anugrahjo/PySLSQP/blob/main/LICENSE.txt)
 
 The SLSQP algorithm is designed to solve nonlinear programming (NLP) problems.
 PySLSQP is a Python package that wrraps the original SLSQP algorithm 
 implemented in Fortran by Dieter Kraft.
 While the Fortran code is sourced from 
 [`scipy.optimize.minimize`](https://docs.scipy.org/doc/scipy/reference/optimize.minimize-slsqp.html), 
@@ -137,21 +138,25 @@
 
 ## Installation
 
 To install the latest release of PySLSQP on PyPI, run on the terminal or command line
 ```sh
 pip install pyslsqp
 ```
+Precompiled wheels for common Ubuntu and macOS architectures are available on PyPI.
+However, if the wheel for your system's architecture is not available, or if you are a Windows user,
+the above installation will compile the source distribution directly on your machine.
+In such scenarios, if your Fortran compilers aren't compatible, you may encounter compilation errors.
 
 To install the latest commit from the main branch, run
 ```sh
 pip install git+https://github.com/anugrahjo/PySLSQP.git@main
 ```
-<!-- Note that this will compile the package locally on your computer.
-Therefore, this is  not recommended unless you are a developer and wants to edit the package for your use. -->
+Note that this installation method will compile the Fortran sources locally on your machine.
+Therefore, we only recommend this method if you are a developer looking to modify the package for your own use case.
 
 To upgrade PySLSQP from an older version to the latest released version on PyPI, run
 ```sh
 pip install --upgrade pyslsqp
 ```
 
 To uninstall PySLSQP, run
```

### Comparing `pyslsqp-0.1.0a0/README.md` & `pyslsqp-0.1.0b0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 [![Pypi](https://img.shields.io/pypi/v/PySLSQP)](https://pypi.org/project/PySLSQP/)
 [![PyPI version][10]][11]
 [![PyPI Monthly Downloads][12]][11]
 -->
 
 [![GitHub Actions Test Badge](https://github.com/anugrahjo/PySLSQP/actions/workflows/build_install_test.yml/badge.svg)](https://github.com/anugrahjo/PySLSQP/actions)
 [![Coverage Status](https://coveralls.io/repos/github/anugrahjo/PySLSQP/badge.svg?branch=main)](https://coveralls.io/github/anugrahjo/PySLSQP?branch=main)
+[![Documentation Status](https://readthedocs.org/projects/pyslsqp/badge/?version=latest)](https://pyslsqp.readthedocs.io/en/latest/?badge=main)
 [![Pypi version](https://img.shields.io/pypi/v/pyslsqp)](https://pypi.org/project/pyslsqp/)
-[![Forks](https://img.shields.io/github/forks/anugrahjo/PySLSQP.svg)](https://github.com/anugrahjo/PySLSQP/network)
-[![Issues](https://img.shields.io/github/issues/anugrahjo/PySLSQP.svg)](https://github.com/anugrahjo/PySLSQP/issues)
+<!-- [![Forks](https://img.shields.io/github/forks/anugrahjo/PySLSQP.svg)](https://github.com/anugrahjo/PySLSQP/network) -->
+<!-- [![Issues](https://img.shields.io/github/issues/anugrahjo/PySLSQP.svg)](https://github.com/anugrahjo/PySLSQP/issues) -->
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://github.com/anugrahjo/PySLSQP/blob/main/LICENSE.txt)
 
 The SLSQP algorithm is designed to solve nonlinear programming (NLP) problems.
 PySLSQP is a Python package that wrraps the original SLSQP algorithm 
 implemented in Fortran by Dieter Kraft.
 While the Fortran code is sourced from 
 [`scipy.optimize.minimize`](https://docs.scipy.org/doc/scipy/reference/optimize.minimize-slsqp.html), 
@@ -72,21 +73,25 @@
 
 ## Installation
 
 To install the latest release of PySLSQP on PyPI, run on the terminal or command line
 ```sh
 pip install pyslsqp
 ```
+Precompiled wheels for common Ubuntu and macOS architectures are available on PyPI.
+However, if the wheel for your system's architecture is not available, or if you are a Windows user,
+the above installation will compile the source distribution directly on your machine.
+In such scenarios, if your Fortran compilers aren't compatible, you may encounter compilation errors.
 
 To install the latest commit from the main branch, run
 ```sh
 pip install git+https://github.com/anugrahjo/PySLSQP.git@main
 ```
-<!-- Note that this will compile the package locally on your computer.
-Therefore, this is  not recommended unless you are a developer and wants to edit the package for your use. -->
+Note that this installation method will compile the Fortran sources locally on your machine.
+Therefore, we only recommend this method if you are a developer looking to modify the package for your own use case.
 
 To upgrade PySLSQP from an older version to the latest released version on PyPI, run
 ```sh
 pip install --upgrade pyslsqp
 ```
 
 To uninstall PySLSQP, run
```

### Comparing `pyslsqp-0.1.0a0/docs/Makefile` & `pyslsqp-0.1.0b0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0a0/docs/conf.py` & `pyslsqp-0.1.0b0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0a0/docs/make.bat` & `pyslsqp-0.1.0b0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0a0/docs/src/api_pages/postprocessing.md` & `pyslsqp-0.1.0b0/docs/src/api_pages/postprocessing.md`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0a0/docs/src/basic.ipynb` & `pyslsqp-0.1.0b0/docs/src/basic.ipynb`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0a0/docs/src/getting_started.md` & `pyslsqp-0.1.0b0/docs/src/getting_started.md`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0a0/docs/src/images/lsdolab.png` & `pyslsqp-0.1.0b0/docs/src/images/lsdolab.png`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0a0/docs/src/images/lsdolab_website.png` & `pyslsqp-0.1.0b0/docs/src/images/lsdolab_website.png`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0a0/docs/src/postprocessing.ipynb` & `pyslsqp-0.1.0b0/docs/src/postprocessing.ipynb`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0a0/docs/src/references.bib` & `pyslsqp-0.1.0b0/docs/src/references.bib`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0a0/docs/src/welcome.md` & `pyslsqp-0.1.0b0/docs/src/welcome.md`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0a0/meson.build` & `pyslsqp-0.1.0b0/meson.build`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0a0/pyproject.toml` & `pyslsqp-0.1.0b0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0a0/pyslsqp/main.py` & `pyslsqp-0.1.0b0/pyslsqp/main.py`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0a0/pyslsqp/meson.build` & `pyslsqp-0.1.0b0/pyslsqp/meson.build`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0a0/pyslsqp/save_and_load.py` & `pyslsqp-0.1.0b0/pyslsqp/save_and_load.py`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0a0/pyslsqp/slsqp/LICENSE.txt` & `pyslsqp-0.1.0b0/pyslsqp/slsqp/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0a0/pyslsqp/slsqp/slsqp.pyf` & `pyslsqp-0.1.0b0/pyslsqp/slsqp/slsqp.pyf`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0a0/pyslsqp/slsqp/slsqp_optmz.f` & `pyslsqp-0.1.0b0/pyslsqp/slsqp/slsqp_optmz.f`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0a0/pyslsqp/visualize.py` & `pyslsqp-0.1.0b0/pyslsqp/visualize.py`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0a0/pyslsqp.egg-info/PKG-INFO` & `pyslsqp-0.1.0b0/pyslsqp.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslsqp
-Version: 0.1.0a0
+Version: 0.1.0b0
 Summary: A transparent Python interface to the SLSQP optimization algorithm, with advanced features and visualization capabilities.
 Author-email: Anugrah Jo Joshy <ajoshy.ucsd@gmail.com>
 Maintainer-email: Anugrah Jo Joshy <ajoshy.ucsd@gmail.com>
 License: Copyright (c) 2024, Anugrah Jo Joshy.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -70,17 +70,18 @@
 [![Pypi](https://img.shields.io/pypi/v/PySLSQP)](https://pypi.org/project/PySLSQP/)
 [![PyPI version][10]][11]
 [![PyPI Monthly Downloads][12]][11]
 -->
 
 [![GitHub Actions Test Badge](https://github.com/anugrahjo/PySLSQP/actions/workflows/build_install_test.yml/badge.svg)](https://github.com/anugrahjo/PySLSQP/actions)
 [![Coverage Status](https://coveralls.io/repos/github/anugrahjo/PySLSQP/badge.svg?branch=main)](https://coveralls.io/github/anugrahjo/PySLSQP?branch=main)
+[![Documentation Status](https://readthedocs.org/projects/pyslsqp/badge/?version=latest)](https://pyslsqp.readthedocs.io/en/latest/?badge=main)
 [![Pypi version](https://img.shields.io/pypi/v/pyslsqp)](https://pypi.org/project/pyslsqp/)
-[![Forks](https://img.shields.io/github/forks/anugrahjo/PySLSQP.svg)](https://github.com/anugrahjo/PySLSQP/network)
-[![Issues](https://img.shields.io/github/issues/anugrahjo/PySLSQP.svg)](https://github.com/anugrahjo/PySLSQP/issues)
+<!-- [![Forks](https://img.shields.io/github/forks/anugrahjo/PySLSQP.svg)](https://github.com/anugrahjo/PySLSQP/network) -->
+<!-- [![Issues](https://img.shields.io/github/issues/anugrahjo/PySLSQP.svg)](https://github.com/anugrahjo/PySLSQP/issues) -->
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://github.com/anugrahjo/PySLSQP/blob/main/LICENSE.txt)
 
 The SLSQP algorithm is designed to solve nonlinear programming (NLP) problems.
 PySLSQP is a Python package that wrraps the original SLSQP algorithm 
 implemented in Fortran by Dieter Kraft.
 While the Fortran code is sourced from 
 [`scipy.optimize.minimize`](https://docs.scipy.org/doc/scipy/reference/optimize.minimize-slsqp.html), 
@@ -137,21 +138,25 @@
 
 ## Installation
 
 To install the latest release of PySLSQP on PyPI, run on the terminal or command line
 ```sh
 pip install pyslsqp
 ```
+Precompiled wheels for common Ubuntu and macOS architectures are available on PyPI.
+However, if the wheel for your system's architecture is not available, or if you are a Windows user,
+the above installation will compile the source distribution directly on your machine.
+In such scenarios, if your Fortran compilers aren't compatible, you may encounter compilation errors.
 
 To install the latest commit from the main branch, run
 ```sh
 pip install git+https://github.com/anugrahjo/PySLSQP.git@main
 ```
-<!-- Note that this will compile the package locally on your computer.
-Therefore, this is  not recommended unless you are a developer and wants to edit the package for your use. -->
+Note that this installation method will compile the Fortran sources locally on your machine.
+Therefore, we only recommend this method if you are a developer looking to modify the package for your own use case.
 
 To upgrade PySLSQP from an older version to the latest released version on PyPI, run
 ```sh
 pip install --upgrade pyslsqp
 ```
 
 To uninstall PySLSQP, run
```

### Comparing `pyslsqp-0.1.0a0/pyslsqp.egg-info/SOURCES.txt` & `pyslsqp-0.1.0b0/pyslsqp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0a0/setup.py` & `pyslsqp-0.1.0b0/setup.py`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0a0/tests/test_docs.py` & `pyslsqp-0.1.0b0/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0a0/tests/test_docstring_examples.py` & `pyslsqp-0.1.0b0/tests/test_docstring_examples.py`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0a0/tests/test_optimize.py` & `pyslsqp-0.1.0b0/tests/test_optimize.py`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0a0/tests/test_save_and_load.py` & `pyslsqp-0.1.0b0/tests/test_save_and_load.py`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0a0/tests/testing_utils.py` & `pyslsqp-0.1.0b0/tests/testing_utils.py`

 * *Files identical despite different names*

