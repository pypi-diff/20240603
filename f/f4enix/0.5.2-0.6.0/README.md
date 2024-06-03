# Comparing `tmp/f4enix-0.5.2.tar.gz` & `tmp/f4enix-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f4enix-0.5.2.tar", last modified: Thu Apr 18 07:01:58 2024, max compression
+gzip compressed data, was "f4enix-0.6.0.tar", last modified: Mon Jun  3 06:55:48 2024, max compression
```

## Comparing `f4enix-0.5.2.tar` & `f4enix-0.6.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:01:58.716752 f4enix-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)    13969 2024-04-18 07:01:54.000000 f4enix-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-18 07:01:54.000000 f4enix-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-04-18 07:01:58.716752 f4enix-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-18 07:01:54.000000 f4enix-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:01:58.708752 f4enix-0.5.2/f4enix/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:01:58.712752 f4enix-0.5.2/f4enix/input/
--rw-r--r--   0 runner    (1001) docker     (127)    51583 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/input/MCNPinput.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/input/auxiliary.py
--rw-r--r--   0 runner    (1001) docker     (127)    19352 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/input/d1suned.py
--rw-r--r--   0 runner    (1001) docker     (127)    16003 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/input/elite.py
--rw-r--r--   0 runner    (1001) docker     (127)    16354 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/input/libmanager.py
--rw-r--r--   0 runner    (1001) docker     (127)    46251 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/input/materials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:01:58.712752 f4enix-0.5.2/f4enix/input/ww_gvr/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/input/ww_gvr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/input/ww_gvr/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8651 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/input/ww_gvr/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8833 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/input/ww_gvr/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/input/ww_gvr/meshgrids.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/input/ww_gvr/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/input/ww_gvr/ratios_calculation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/input/ww_gvr/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16274 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/input/ww_gvr/weight_window.py
--rw-r--r--   0 runner    (1001) docker     (127)    11918 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/input/ww_gvr/ww_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    13244 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/input/xsdirpyne.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:01:58.716752 f4enix-0.5.2/f4enix/output/
--rw-r--r--   0 runner    (1001) docker     (127)    20866 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/output/MCNPoutput.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/output/cuv_sampling_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    15777 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/output/eeout.py
--rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/output/fispact_legacy_out.py
--rw-r--r--   0 runner    (1001) docker     (127)    51433 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/output/mctal.py
--rw-r--r--   0 runner    (1001) docker     (127)    18915 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/output/meshinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)    73563 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/output/meshtal.py
--rw-r--r--   0 runner    (1001) docker     (127)    33393 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/output/plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)    19766 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/output/rssa.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:01:58.716752 f4enix-0.5.2/f4enix/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    19154 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/resources/Isotopes.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17456 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/resources/activation_libs.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)  1119446 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/resources/xsdir.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:01:58.716752 f4enix-0.5.2/f4enix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-04-18 07:01:58.000000 f4enix-0.5.2/f4enix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-18 07:01:58.000000 f4enix-0.5.2/f4enix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 07:01:58.000000 f4enix-0.5.2/f4enix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-18 07:01:58.000000 f4enix-0.5.2/f4enix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 07:01:58.000000 f4enix-0.5.2/f4enix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-18 07:01:54.000000 f4enix-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-18 07:01:58.720752 f4enix-0.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:01:58.716752 f4enix-0.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-18 07:01:54.000000 f4enix-0.5.2/tests/test_cuv_sampling_error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:55:48.119968 f4enix-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    13969 2024-06-03 06:55:43.000000 f4enix-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-03 06:55:43.000000 f4enix-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-06-03 06:55:48.119968 f4enix-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-06-03 06:55:43.000000 f4enix-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:55:48.111968 f4enix-0.6.0/f4enix/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-06-03 06:55:43.000000 f4enix-0.6.0/f4enix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-03 06:55:43.000000 f4enix-0.6.0/f4enix/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-06-03 06:55:43.000000 f4enix-0.6.0/f4enix/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:55:48.115968 f4enix-0.6.0/f4enix/input/
+-rw-r--r--   0 runner    (1001) docker     (127)    51579 2024-06-03 06:55:43.000000 f4enix-0.6.0/f4enix/input/MCNPinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 06:55:43.000000 f4enix-0.6.0/f4enix/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-06-03 06:55:43.000000 f4enix-0.6.0/f4enix/input/auxiliary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19352 2024-06-03 06:55:43.000000 f4enix-0.6.0/f4enix/input/d1suned.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16003 2024-06-03 06:55:43.000000 f4enix-0.6.0/f4enix/input/elite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16344 2024-06-03 06:55:43.000000 f4enix-0.6.0/f4enix/input/libmanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46242 2024-06-03 06:55:43.000000 f4enix-0.6.0/f4enix/input/materials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:55:48.115968 f4enix-0.6.0/f4enix/input/ww_gvr/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-06-03 06:55:43.000000 f4enix-0.6.0/f4enix/input/ww_gvr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-06-03 06:55:43.000000 f4enix-0.6.0/f4enix/input/ww_gvr/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8651 2024-06-03 06:55:43.000000 f4enix-0.6.0/f4enix/input/ww_gvr/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8889 2024-06-03 06:55:43.000000 f4enix-0.6.0/f4enix/input/ww_gvr/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-06-03 06:55:43.000000 f4enix-0.6.0/f4enix/input/ww_gvr/meshgrids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-06-03 06:55:43.000000 f4enix-0.6.0/f4enix/input/ww_gvr/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-06-03 06:55:43.000000 f4enix-0.6.0/f4enix/input/ww_gvr/ratios_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-06-03 06:55:43.000000 f4enix-0.6.0/f4enix/input/ww_gvr/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16274 2024-06-03 06:55:43.000000 f4enix-0.6.0/f4enix/input/ww_gvr/weight_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11875 2024-06-03 06:55:43.000000 f4enix-0.6.0/f4enix/input/ww_gvr/ww_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13244 2024-06-03 06:55:43.000000 f4enix-0.6.0/f4enix/input/xsdirpyne.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:55:48.119968 f4enix-0.6.0/f4enix/output/
+-rw-r--r--   0 runner    (1001) docker     (127)    20866 2024-06-03 06:55:43.000000 f4enix-0.6.0/f4enix/output/MCNPoutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 06:55:43.000000 f4enix-0.6.0/f4enix/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-06-03 06:55:43.000000 f4enix-0.6.0/f4enix/output/cuv_sampling_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15777 2024-06-03 06:55:43.000000 f4enix-0.6.0/f4enix/output/eeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-06-03 06:55:43.000000 f4enix-0.6.0/f4enix/output/fispact_legacy_out.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51433 2024-06-03 06:55:43.000000 f4enix-0.6.0/f4enix/output/mctal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18915 2024-06-03 06:55:43.000000 f4enix-0.6.0/f4enix/output/meshinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73559 2024-06-03 06:55:43.000000 f4enix-0.6.0/f4enix/output/meshtal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33473 2024-06-03 06:55:43.000000 f4enix-0.6.0/f4enix/output/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19766 2024-06-03 06:55:43.000000 f4enix-0.6.0/f4enix/output/rssa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:55:48.119968 f4enix-0.6.0/f4enix/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    19154 2024-06-03 06:55:43.000000 f4enix-0.6.0/f4enix/resources/Isotopes.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 06:55:43.000000 f4enix-0.6.0/f4enix/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17456 2024-06-03 06:55:43.000000 f4enix-0.6.0/f4enix/resources/activation_libs.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)  1119446 2024-06-03 06:55:43.000000 f4enix-0.6.0/f4enix/resources/xsdir.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:55:48.119968 f4enix-0.6.0/f4enix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-06-03 06:55:48.000000 f4enix-0.6.0/f4enix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-06-03 06:55:48.000000 f4enix-0.6.0/f4enix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 06:55:48.000000 f4enix-0.6.0/f4enix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-06-03 06:55:48.000000 f4enix-0.6.0/f4enix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-03 06:55:48.000000 f4enix-0.6.0/f4enix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-06-03 06:55:43.000000 f4enix-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-06-03 06:55:48.119968 f4enix-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:55:48.119968 f4enix-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-06-03 06:55:43.000000 f4enix-0.6.0/tests/test_cuv_sampling_error.py
```

### Comparing `f4enix-0.5.2/LICENSE` & `f4enix-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.2/PKG-INFO` & `f4enix-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: f4enix
-Version: 0.5.2
+Version: 0.6.0
 Summary: API for Monte Carlo input and output parsing
 Author: F4E neutronics team
 Author-email: sc-radiationtransport@f4e.europa.eu
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: appdirs
 Requires-Dist: asttokens
 Requires-Dist: attrs
 Requires-Dist: backcall
 Requires-Dist: charset-normalizer
@@ -74,15 +74,15 @@
 [![Testing linux](https://github.com/Radiation-Transport/F4Enix/actions/workflows/AutomatedTests_linux.yml/badge.svg?branch=main)](https://github.com/Radiation-Transport/F4Enix/actions/workflows/AutomatedTests_linux.yml)
 [![PyPi version](https://badgen.net/pypi/v/f4enix/)](https://pypi.org/project/f4enix)
 [![Documentation Status](https://readthedocs.org/projects/f4enix/badge/?version=latest)](https://f4enix.readthedocs.io/en/latest/?badge=latest)
 
 # F4Enix
 Parser for Monte Carlo simulations input and output files
 
-**Pyhton >3.10!**
+**Pyhton >3.9!**
 
 Both Windows and Linux supported.
 
 Go to [F4Enix official documentation](https://f4enix.readthedocs.io/en/latest/) to get
 more information on the library capabilities, examples and much more.
 
 ## Install
@@ -95,15 +95,15 @@
 ### Troubleshooting and developer mode
 If any unexpected issue is encountered during installation, the first step for
 its resolution would be to create a new fresh virtual environment.
 In conda this would be done with:
 ```
 conda create -n <env_name> python=3.10
 ```
-Please remeber that python versions lower than 3.10 are not supported.
+Please remember that python versions lower than 3.10 are not supported.
 
 ### Developer mode installation
 There are many situations (especially while being an active developer) where it may be useful to install f4enix in developer mode. In order to do so, navigate to the
 F4Eparser folder and type the following to be sure that your pip is
 up to date (optional):
 ```
 python -m pip install --upgrade pip setuptools wheel
```

### Comparing `f4enix-0.5.2/README.md` & `f4enix-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [![Testing linux](https://github.com/Radiation-Transport/F4Enix/actions/workflows/AutomatedTests_linux.yml/badge.svg?branch=main)](https://github.com/Radiation-Transport/F4Enix/actions/workflows/AutomatedTests_linux.yml)
 [![PyPi version](https://badgen.net/pypi/v/f4enix/)](https://pypi.org/project/f4enix)
 [![Documentation Status](https://readthedocs.org/projects/f4enix/badge/?version=latest)](https://f4enix.readthedocs.io/en/latest/?badge=latest)
 
 # F4Enix
 Parser for Monte Carlo simulations input and output files
 
-**Pyhton >3.10!**
+**Pyhton >3.9!**
 
 Both Windows and Linux supported.
 
 Go to [F4Enix official documentation](https://f4enix.readthedocs.io/en/latest/) to get
 more information on the library capabilities, examples and much more.
 
 ## Install
@@ -23,15 +23,15 @@
 ### Troubleshooting and developer mode
 If any unexpected issue is encountered during installation, the first step for
 its resolution would be to create a new fresh virtual environment.
 In conda this would be done with:
 ```
 conda create -n <env_name> python=3.10
 ```
-Please remeber that python versions lower than 3.10 are not supported.
+Please remember that python versions lower than 3.10 are not supported.
 
 ### Developer mode installation
 There are many situations (especially while being an active developer) where it may be useful to install f4enix in developer mode. In order to do so, navigate to the
 F4Eparser folder and type the following to be sure that your pip is
 up to date (optional):
 ```
 python -m pip install --upgrade pip setuptools wheel
```

### Comparing `f4enix-0.5.2/f4enix/constants.py` & `f4enix-0.6.0/f4enix/constants.py`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.2/f4enix/input/MCNPinput.py` & `f4enix-0.6.0/f4enix/input/MCNPinput.py`

 * *Files 0% similar despite different names*

```diff
@@ -724,15 +724,15 @@
                 if extract_fillers:
                     fill = c.get_f()
                     if fill is not None:
                         uni_set.add(fill)
             # if one wants to extract also lower levels, loop over universes
             # and collect their cells
             if extract_fillers:
-                for key, c in self.cells.items():
+                for _, c in self.cells.items():
                     if c.get_u() in uni_set:
                         new_set.add(c.values[0][0])
             # get the new set with the cells to be checked
             cell_set = new_set - cell_set
             # check if loop is to be repeated
             if cell_set:
                 again = True
@@ -826,15 +826,15 @@
         original_density*factor
 
         Parameters
         ----------
         factor : float
             scaling factors for the densities
         """
-        for key, cell in self.cells.items():
+        for _, cell in self.cells.items():
             if not cell._get_value_by_type("mat") == 0:
                 density = cell.get_d()
                 newdensity = "{:.5e}".format(density * factor)
                 cell.set_d(newdensity)
 
     def get_cells_summary(self) -> pd.DataFrame:
         """Get a summary of infos for each cell
```

### Comparing `f4enix-0.5.2/f4enix/input/auxiliary.py` & `f4enix-0.6.0/f4enix/input/auxiliary.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 Unless required by applicable law or agreed to in writing, software distributed
 under the Licence is distributed on an “AS IS” basis, WITHOUT WARRANTIES OR
 CONDITIONS OF ANY KIND, either express or implied. See the Licence permissions
 and limitations under the Licence.
 """
 
 from numjuggler.parser import Card
-from f4enix.constants import PAT_COMMENT, PAT_DOLLAR_COMMENT, PAT_COMMENT_TEXT
+from f4enix.constants import PAT_DOLLAR_COMMENT, PAT_COMMENT_TEXT
 import re
 import os
 
 _surrogates = re.compile(r"[\uDC80-\uDCFF]")
 
 
 def get_comments(card: Card) -> str:
```

### Comparing `f4enix-0.5.2/f4enix/input/d1suned.py` & `f4enix-0.6.0/f4enix/input/d1suned.py`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.2/f4enix/input/elite.py` & `f4enix-0.6.0/f4enix/input/elite.py`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.2/f4enix/input/libmanager.py` & `f4enix-0.6.0/f4enix/input/libmanager.py`

 * *Files 0% similar despite different names*

```diff
@@ -455,15 +455,15 @@
         reactions : list[tuple[str, str]]
             contains tuple of (MT, daughter).
 
         """
         reactions = []
         try:
             df = self.reactions[lib].set_index('Parent')
-            isotopename, formula = self.get_zaidname(parent)
+            _, formula = self.get_zaidname(parent)
             formulazaid = formula.replace('-', '')  # eliminate the '-'
             # collect and provide as tuples
             subset = df.loc[formulazaid]
             try:
                 for _, row in subset.iterrows():
                     MT = str(int(row['MT']))
                     daughter = row['Daughter']
```

### Comparing `f4enix-0.5.2/f4enix/input/materials.py` & `f4enix-0.6.0/f4enix/input/materials.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
         """
         Generate an Element object starting from a list of zaids.
         It will collapse multiple instance of a zaid into a single one
 
         Parameters
         ----------
         zaidList : list
-            list of zaids constituing the element.
+            list of zaids constituting the element.
 
         Returns
         -------
         None.
 
         Attributes
         ----------
@@ -410,15 +410,15 @@
         for zaid in self.zaidList:
             if zaid.element not in elements.keys():
                 elements[zaid.element] = [zaid]
             else:
                 elements[zaid.element].append(zaid)
 
         elemList = []
-        for element_tag, zaids in elements.items():
+        for _, zaids in elements.items():
             elemList.append(Element(zaids))
 
         self.elements = elemList
 
     def to_text(self) -> str:
         """
         Write to text in MNCP format the submaterial
```

### Comparing `f4enix-0.5.2/f4enix/input/ww_gvr/cli.py` & `f4enix-0.6.0/f4enix/input/ww_gvr/cli.py`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.2/f4enix/input/ww_gvr/geometry.py` & `f4enix-0.6.0/f4enix/input/ww_gvr/geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+from __future__ import annotations
+
 """
 This module contains the Geometry class, which is used to create a pyvista grid
 from the coarse and fine vectors of a WW file. It also contains the methods to
 fill the grid with the values of the WW file and to plot it.
 """
+
 from pathlib import Path
-from typing import Dict, List
+from typing import Dict, List, Union
 
 import numpy as np
 import pyvista as pv
 from numpy.typing import NDArray
 from pyvista.plotting.plotter import Plotter
 
 from f4enix.input.ww_gvr.meshgrids import create_cartesian_grid, create_cylindrical_grid
@@ -146,23 +149,23 @@
 
     @property
     def b2_vectors(self) -> Vectors:
         """Returns a Vectors object of the vectors in the b2 format of the WW file"""
         return compose_b2_vectors(self._coarse_vectors, self._fine_vectors)
 
     @property
-    def director_1(self) -> List[float] | None:
+    def director_1(self) -> Union[List[float], None]:
         """
         Returns the director 1 vector (axis) of the cylinder if the grid is
         cylindrical.
         """
         return self._director_1
 
     @property
-    def director_2(self) -> List[float] | None:
+    def director_2(self) -> Union[List[float], None]:
         """
         Returns the director 2 vector (radius) of the cylinder if the grid is
         cylindrical.
         """
         return self._director_2
 
     @property
```

### Comparing `f4enix-0.5.2/f4enix/input/ww_gvr/meshgrids.py` & `f4enix-0.6.0/f4enix/input/ww_gvr/meshgrids.py`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.2/f4enix/input/ww_gvr/models.py` & `f4enix-0.6.0/f4enix/input/ww_gvr/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,18 @@
+from __future__ import annotations
+
 """
 Classes and types used throughout the package.
 """
+
+
 from dataclasses import dataclass
 from enum import Enum
 from pathlib import Path
-from typing import Dict, List
+from typing import Dict, List, Union
 
 import numpy as np
 from numpy.typing import NDArray
 
 
 class CoordinateType(Enum):
     CARTESIAN = "cartesian"
@@ -16,15 +20,15 @@
 
 
 class ParticleType(Enum):
     NEUTRON = "neutron"
     PHOTON = "photon"
 
 
-@dataclass(kw_only=True)
+@dataclass()
 class Vectors:
     """
     A group of three vectors in the form of a Numpy NDArray. They are used to define 3D
     meshes.
     """
 
     vector_i: NDArray  # Vector defining i direction
@@ -40,12 +44,12 @@
             np.testing.assert_array_almost_equal(self.vector_j, other.vector_j)
             np.testing.assert_array_almost_equal(self.vector_k, other.vector_k)
             return True
         except AssertionError:
             return False
 
 
-Pathlike = str | Path
+Pathlike = Union[str, Path]
 NestedList = List[List[float]]
 ValuesByEnergy = Dict[float, np.ndarray]
 ValuesByParticle = Dict[ParticleType, ValuesByEnergy]
 EnergiesByParticle = Dict[ParticleType, List[float]]
```

### Comparing `f4enix-0.5.2/f4enix/input/ww_gvr/ratios_calculation.py` & `f4enix-0.6.0/f4enix/input/ww_gvr/ratios_calculation.py`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.2/f4enix/input/ww_gvr/utils.py` & `f4enix-0.6.0/f4enix/input/ww_gvr/utils.py`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.2/f4enix/input/ww_gvr/weight_window.py` & `f4enix-0.6.0/f4enix/input/ww_gvr/weight_window.py`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.2/f4enix/input/ww_gvr/ww_parser.py` & `f4enix-0.6.0/f4enix/input/ww_gvr/ww_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 """
 Classes and functions to read WW files.
 """
+
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any, Dict, List, TextIO
 
 import numpy as np
 from numpy import float64
 from numpy.typing import NDArray
 
 from f4enix.input.ww_gvr.models import NestedList, Vectors
 from f4enix.input.ww_gvr.utils import compose_b2_vectors
 from f4enix.output.meshtal import Fmesh, Meshtal
 
 
-@dataclass(kw_only=True)
+@dataclass()
 class WWHeader:
-    if_: int = 1  # File type. Always 1, unused.
-    iv: int = 1  # Time-dependent windows flag. 1/2 = no/yes
+    if_: int  # File type. Always 1, unused.
+    iv: int  # Time-dependent windows flag. 1/2 = no/yes
     ni: int  # Number of particle types
     nr: int  # 10/16/16 = cartesian/cylindrical/spherical coord
     probid: str  # Date and time of run
     ne: List[int]  # Number of energy windows of each particle
     nfx: int  # Number of fine meshses in i
     nfy: int  # Number of fine meshses in j
     nfz: int  # Number of fine meshses in k
     origin: List[float]  #  Bottom left corner for cart, bottom center for cyl
     ncx: int  # Number of coarse meshses in i
     ncy: int  # Number of coarse meshses in j
     ncz: int  # Number of coarse meshses in k
 
 
-@dataclass(kw_only=True)
+@dataclass()
 class WWHeaderCyl(WWHeader):
     director_1: List[float]  # Vector defining the director 1
     director_2: List[float]  # Vector defining the director 2
 
 
-@dataclass(kw_only=True)
+@dataclass()
 class ParseResult:
     header: WWHeader
     b2_vectors: Vectors
     energies: NestedList
     values: NestedList
```

### Comparing `f4enix-0.5.2/f4enix/input/xsdirpyne.py` & `f4enix-0.6.0/f4enix/input/xsdirpyne.py`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.2/f4enix/output/MCNPoutput.py` & `f4enix-0.6.0/f4enix/output/MCNPoutput.py`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.2/f4enix/output/cuv_sampling_error.py` & `f4enix-0.6.0/f4enix/output/cuv_sampling_error.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import IO, Dict, Tuple
+from __future__ import annotations
+from typing import IO, Dict, Tuple, Union
 
 import numpy as np
 import pyvista as pv
 
 from f4enix.input.ww_gvr.models import Pathlike
 
 
@@ -36,15 +37,15 @@
 
     return voxel_cell_errors
 
 
 def _read_voxel(infile: IO, voxel_sampling_points: int) -> Tuple[int, Dict[int, float]]:
     first_line_words = infile.readline().split()
     # 1-based index on the file, we want 0-based
-    voxel_id = int(first_line_words[0]) - 1  
+    voxel_id = int(first_line_words[0]) - 1
     amount_of_cells = int(first_line_words[5])
 
     cell_errors = {}
     for _ in range(amount_of_cells):
         words = infile.readline().split()
         cell_id = int(words[0])
         cell_error = calculate_volume_sampling_error(
@@ -63,17 +64,17 @@
     partial_volume: float, voxel_sampling_points: int
 ) -> float:
     return (
         (partial_volume - partial_volume**2) / (voxel_sampling_points)
     ) ** 0.5 / partial_volume
 
 
-pyvista_grid = (
-    pv.StructuredGrid | pv.UnstructuredGrid | pv.PolyData | pv.RectilinearGrid
-)
+pyvista_grid = Union[
+    pv.StructuredGrid, pv.UnstructuredGrid, pv.PolyData, pv.RectilinearGrid
+]
 
 
 def add_sampling_error_to_vtk(
     grid: pyvista_grid, cuv_file_path: Pathlike, voxel_sampling_points: int
 ) -> pyvista_grid:
     """
     Add a new array to the grid with the volume sampling error. In the case of a voxel
```

### Comparing `f4enix-0.5.2/f4enix/output/eeout.py` & `f4enix-0.6.0/f4enix/output/eeout.py`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.2/f4enix/output/fispact_legacy_out.py` & `f4enix-0.6.0/f4enix/output/fispact_legacy_out.py`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.2/f4enix/output/mctal.py` & `f4enix-0.6.0/f4enix/output/mctal.py`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.2/f4enix/output/meshinfo.py` & `f4enix-0.6.0/f4enix/output/meshinfo.py`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.2/f4enix/output/meshtal.py` & `f4enix-0.6.0/f4enix/output/meshtal.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 # return a list of each nth charaters of a string
 def _splitn(string: str, n: int) -> list[str]:
     return [string[i: i + n].strip() for i in range(0, len(string), n)]
 
 
 # Salta lineas (definida en cien sitios)
 def _skipLines(f, n):
-    for iskip in range(n):
+    for _ in range(n):
         f.readline()
     return
 
 
 # # read cell list from file for CUV filtering option
 # def get_clist(fn: os.PathLike) -> list(int):
 #     f = open(fn, "rt")
```

### Comparing `f4enix-0.5.2/f4enix/output/plotter.py` & `f4enix-0.6.0/f4enix/output/plotter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 """
 Plotter classes and methods for neutronics outputs.
 
 For the moment it allows only to plot slices of meshes.
 """
 
 """
@@ -19,37 +21,34 @@
 
 import os
 import pyvista as pv
 import numpy as np
 import logging
 import docx
 
+from typing import Union
 from docx.shared import Inches, Mm
 from docx.enum.text import WD_ALIGN_PARAGRAPH
 from docx.enum.section import WD_ORIENT
 from PIL import Image, ImageOps
 import io
 from copy import deepcopy
 from abc import ABC, abstractmethod
 import matplotlib.pyplot as plt
 from matplotlib.ticker import PercentFormatter
 
-
-from pathlib import Path
-
 from math import radians, degrees
 from f4enix.constants import TID_CATEGORIES, TNF_CATEGORIES, SDDR_CATEGORIES
 
-pv.set_plot_theme('document')
+pv.set_plot_theme("document")
 
 
 class MeshPlotter:
 
-    def __init__(self, mesh: pv.PolyData, stl: pv.PolyData = None
-                 ) -> None:
+    def __init__(self, mesh: pv.PolyData, stl: pv.PolyData = None) -> None:
         """Object responsible for the plotting of meshes.
 
         Allows slicing in different orientation and plotting of slices.
 
         Parameters
         ----------
         mesh : pv.PolyData
@@ -117,39 +116,41 @@
             shadow=True,
             # n_labels=7,
             italic=True,
             fmt="%.e",
             font_family="arial",
             vertical=True,
             position_x=0.85,
-            position_y=0.25)
+            position_y=0.25,
+        )
 
     def _get_plotter(self) -> pv.Plotter:
         # Initiate the plotter with all default actions if needed
         pl = pv.Plotter(off_screen=True)
         # TODO horizontal bar may be issue here
         pl.add_axes(viewport=(0.8, 0, 1, 0.2))
         # pl.set_background('white')
 
         return pl
 
-    def slice(self, slice_param: list[list]
-              ) -> list[tuple[str, pv.PolyData, pv.PolyData | None]]:
+    def slice(
+        self, slice_param: list[list]
+    ) -> list[tuple[str, pv.PolyData, Union[pv.PolyData, None]]]:
         """Perform arbitrary general slicing providing origin and normal
         vectors.
 
         Parameters
         ----------
         slice_param : list[list]
             matrix of parameters to be provided, one row for each slice.
              [[name, x, y, z, normx, normy, normz], ...]
 
         Returns
         -------
-        list[tuple[str, pv.PolyData, pv.PolyData | None]]
+        list[tuple[str, pv.PolyData, Union[pv.PolyData, None]]]
             contains a list of (slice name, mesh slice, stl slice).
             the names are assigned according to slicing logic.
             In case of no stl assigned to the plotter, the stl slice will be
             equal to None.
 
         """
 
@@ -167,62 +168,65 @@
             else:
                 stl_slice = None
 
             outp.append((name, mesh_slice, stl_slice))
 
         return outp
 
-    def slice_on_axis(self, axis: str, n: int
-                      ) -> list[tuple[str, pv.PolyData, pv.PolyData | None]]:
+    def slice_on_axis(
+        self, axis: str, n: int
+    ) -> list[tuple[str, pv.PolyData, Union[pv.PolyData, None]]]:
         """Creates a series of slice of the mesh distributed equally along the
         specified axis. Stl file will be sliced accordingly if present
 
         Parameters
         ----------
         axis : str
             either 'x', 'y' or 'z'
         n : int
             number of divisions
 
         Returns
         -------
-        list[tuple[str, pv.PolyData, pv.PolyData | None]]
+        list[tuple[str, pv.PolyData, Union[pv.PolyData, None]]]
             contains a list of (slice name, mesh slice, stl slice).
             the names are assigned according to slicing logic.
             In case of no stl assigned to the plotter, the stl slice will be
             equal to None.
 
         """
         # Use the automatic slicing from pyvista
-        idxs = {'x': 0, 'y': 1, 'z': 2}
+        idxs = {"x": 0, "y": 1, "z": 2}
 
         # perform the slices
         slices = self.mesh.slice_along_axis(n, axis=axis)
         # get the corresponding stl slices if needed
         if self._has_stl:
             stl_slices = self._get_stl_slices(slices)
 
         outp = []
         # build the output
         for i, mslice in enumerate(slices):
             # TODO maybe a smarter function here
-            name = 'P{} = {}'.format(axis, round(mslice.center[idxs[axis]], 1))
+            name = "P{} = {}".format(axis, round(mslice.center[idxs[axis]], 1))
             if self._has_stl:
                 stl_slice = stl_slices[i]
             else:
                 stl_slice = None
 
             outp.append((name, mslice, stl_slice))
 
         return outp
 
-    def slice_toroidal(self, theta_increment: float,
-                       center: list = [0, 0, 0],
-                       min_max_theta: tuple[float, float] = None,
-                       ) -> list[tuple[str, pv.PolyData, pv.PolyData | None]]:
+    def slice_toroidal(
+        self,
+        theta_increment: float,
+        center: list = [0, 0, 0],
+        min_max_theta: tuple[float, float] = None,
+    ) -> list[tuple[str, pv.PolyData, Union[pv.PolyData, None]]]:
         """Create a series of slices of the mesh distributed toroidally equally
         around the vertical axis (z). Stl file will be sliced accordingly if
         present
 
         Parameters
         ----------
         theta_increment : float
@@ -230,89 +234,90 @@
         center : list, optional
             x, y, z point to be used as center for the
             slicing, by default [0, 0, 0].
         min_max_theta : tuple(float, float), optional
             specify a minimum and max theta for the plots (degrees).
             This may help
             avoiding slices in empty regions in partial models if the mesh
-            is not properly rotated. By default is None, meaning that the 
+            is not properly rotated. By default is None, meaning that the
             slicing will start at theta = 0 and finish at theta = pi.
 
         Returns
         -------
-        list[tuple[str, pv.PolyData, pv.PolyData | None]]
+        list[tuple[str, pv.PolyData, Union[pv.PolyData, None]]]
             contains a list of (slice name, mesh slice, stl slice).
             the names are assigned according to slicing logic.
             In case of no stl assigned to the plotter, the stl slice will be
             equal to None.
         """
 
         center = np.array(center)
         increment = radians(theta_increment)
         mesh_slices = []
 
         if min_max_theta is None:
             angles = np.arange(0, np.pi, increment)
         else:
-            angles = np.arange(radians(min_max_theta[0]),
-                               radians(min_max_theta[1]),
-                               increment)
+            angles = np.arange(
+                radians(min_max_theta[0]), radians(min_max_theta[1]), increment
+            )
 
         for theta in angles:
-            normal = np.array(
-                [np.cos(theta), np.sin(theta), 0.0]).dot(np.pi / 2.0)
+            normal = np.array([np.cos(theta), np.sin(theta), 0.0]).dot(np.pi / 2.0)
 
             mesh_slice = self.mesh.slice(origin=center, normal=normal)
 
             # try to access its normal, if it has it, it is not empty
             try:
                 mesh_slice.cell_normals[0]
             except KeyError:
                 # it means that nothing can be sliced here because the
                 # the slice is empty
                 logging.warning(
-                    'No slice can be done at theta={} deg'.format(degrees(theta)))
+                    "No slice can be done at theta={} deg".format(degrees(theta))
+                )
                 continue
 
             mesh_slices.append(mesh_slice)
 
         if self._has_stl:
             stl_slices = self._get_stl_slices(mesh_slices)
 
         outp = []
         # build the output
         for i, mslice in enumerate(mesh_slices):
-            name = 'theta = {} deg'.format(round(degrees(angles[i]), 1))
+            name = "theta = {} deg".format(round(degrees(angles[i]), 1))
             if self._has_stl:
                 stl_slice = stl_slices[i]
             else:
                 stl_slice = None
 
             outp.append((name, mslice, stl_slice))
 
         return outp
 
-    def plot_slices(self,
-                    slices: list[tuple[str, pv.PolyData, pv.PolyData | None]],
-                    array_name: str,
-                    outpath: os.PathLike = None,
-                    min_max: tuple[float] = None,
-                    log_scale: bool = True,
-                    stl_color: str = 'white',
-                    n_colors: int = 256,
-                    scale_quality: float = 3,
-                    scale_title: str = None,
-                    custom_categories: str = None
-                    ) -> list[tuple[str, Image.Image]]:
+    def plot_slices(
+        self,
+        slices: list[tuple[str, pv.PolyData, Union[pv.PolyData, None]]],
+        array_name: str,
+        outpath: os.PathLike = None,
+        min_max: tuple[float] = None,
+        log_scale: bool = True,
+        stl_color: str = "white",
+        n_colors: int = 256,
+        scale_quality: float = 3,
+        scale_title: str = None,
+        custom_categories: str = None,
+    ) -> list[tuple[str, Image.Image]]:
         """Plot a series of slices to an outpath folder. The slices names
         are used as file names.
 
         Parameters
         ----------
-        slices : list[tuple[str, pv.PolyData, pv.PolyData  |  None]]
+        slices : list[tuple[str, pv.PolyData, Union[pv.PolyData, None]]]
             list of slices to be plotted. Usually produced with MeshPlotter
             methods.
         array_name : str
             name of the scalar array to be plotted
         outpath : os.PathLike, optional
             path to the directory that will contain all the plots. This folder
             must be already created. Files with the same name will be
@@ -342,71 +347,80 @@
         Raises
         ------
         ValueError
             if the path do not exists
         """
         # Check if a categorical plot is requested
         if custom_categories is not None:
-            if custom_categories == 'SDDR':
+            if custom_categories == "SDDR":
                 ctg = SDDR_CATEGORIES
-            elif custom_categories == 'TNF':
+            elif custom_categories == "TNF":
                 ctg = TNF_CATEGORIES
-            elif custom_categories == 'TID':
+            elif custom_categories == "TID":
                 ctg = TID_CATEGORIES
             else:
                 raise ValueError(
-                    '{} are not valid custom categories'.format(
-                        custom_categories))
+                    "{} are not valid custom categories".format(custom_categories)
+                )
 
         # Check that outpath exists
         if outpath is not None:
             if not os.path.exists(outpath):
-                raise ValueError('{} does not exists'.format(outpath))
+                raise ValueError("{} does not exists".format(outpath))
 
         images = []
 
         scalar_bar_args = deepcopy(self.legend_args)
         if scale_title is not None:
-            scalar_bar_args['title'] = scale_title
+            scalar_bar_args["title"] = scale_title
 
         # get a number of labels that pairs with the number of colors
         # works only with even numbers
         if n_colors < 30 and n_colors % 2 == 0:
-            scalar_bar_args['n_labels'] = int(n_colors/2+1)
+            scalar_bar_args["n_labels"] = int(n_colors / 2 + 1)
 
         for i, (name, mesh_slice, stl_slice) in enumerate(slices):
 
             pl = self._get_plotter()
             if custom_categories is not None:
                 # Add category label to the mesh
                 colors = self._add_categorization(
-                    mesh_slice, array_name, ctg['values'], ctg['categories'],
-                    ctg['colors'], name=custom_categories)
+                    mesh_slice,
+                    array_name,
+                    ctg["values"],
+                    ctg["categories"],
+                    ctg["colors"],
+                    name=custom_categories,
+                )
                 scalars = custom_categories
                 cmap = colors
                 below_color = None
                 above_color = None
                 lscale = False
                 categories = True
             else:
                 scalars = array_name
-                cmap = 'jet'
-                below_color = 'grey'
-                above_color = 'purple'
+                cmap = "jet"
+                below_color = "grey"
+                above_color = "purple"
                 lscale = log_scale
                 categories = False
 
-            pl.add_mesh(mesh_slice, scalars=scalars,
-                        scalar_bar_args=scalar_bar_args,
-                        log_scale=lscale,
-                        below_color=below_color,
-                        above_color=above_color,
-                        clim=min_max, cmap=cmap,
-                        n_colors=n_colors,
-                        categories=categories)
+            pl.add_mesh(
+                mesh_slice,
+                scalars=scalars,
+                scalar_bar_args=scalar_bar_args,
+                log_scale=lscale,
+                below_color=below_color,
+                above_color=above_color,
+                clim=min_max,
+                cmap=cmap,
+                n_colors=n_colors,
+                categories=categories,
+            )
             if stl_slice is not None:
                 pl.add_mesh(stl_slice, color=stl_color)
 
             # if i == 0:
             #     # ensure that all pictures will have the same bounds
             #     bounds = np.array(mesh_slice.bounds)*0.8
             bounds = np.array(mesh_slice.bounds)
@@ -417,38 +431,39 @@
             im = Image.fromarray(pl.screenshot(None, return_img=True))
             bbox = ImageOps.invert(im).getbbox()
             trimmed = im.crop(bbox)
 
             images.append((name, trimmed))
 
             if outpath is not None:
-                filename = os.path.join(outpath, '{}.png'.format(name))
+                filename = os.path.join(outpath, "{}.png".format(name))
                 pl.screenshot(filename, scale=scale_quality)
 
         return images
 
     @staticmethod
-    def _set_perpendicular_camera(mesh_slice: pv.PolyData,
-                                  pl: pv.Plotter,
-                                  bounds: list = None) -> None:
+    def _set_perpendicular_camera(
+        mesh_slice: pv.PolyData, pl: pv.Plotter, bounds: list = None
+    ) -> None:
         # align camera: focus on center, position at center + normal
         center = mesh_slice.center
         pl.camera.focal_point = center
         pl.camera.position = center - mesh_slice.cell_normals[0]
         # reset camera to put entire mesh in view
         if bounds is None:
             pl.reset_camera()
         else:
             # help put Y up in case of PZ plots
             if bounds[-2] == bounds[-1]:
                 pl.set_viewup([0, 1, 0])
             pl.reset_camera(bounds=bounds)
 
-    def _get_stl_slices(self, mesh_slices: list[pv.PolyData]
-                        ) -> list[pv.PolyData] | None:
+    def _get_stl_slices(
+        self, mesh_slices: list[pv.PolyData]
+    ) -> Union[list[pv.PolyData], None]:
         stl_slices = []
         # get the correspondent stl_slices
         for mesh_slice in mesh_slices:
             # check it is not empty
             if len(mesh_slice[mesh_slice.array_names[0]]) == 0:
                 stl_slices.append(None)
                 continue
@@ -458,27 +473,32 @@
             if stl_slice.bounds is None:
                 # This may happen if the stl is smaller than the mesh
                 stl_slices.append(None)
                 continue
             # give a very small translation in order to not be exactly
             # coincident, using the normal should be sufficient
             # but it needs to be properly scaled
-            scale = np.abs(mesh_slice.points).mean()*1e-3
-            stl_slice.translate(-norm*scale, inplace=True)
+            scale = np.abs(mesh_slice.points).mean() * 1e-3
+            stl_slice.translate(-norm * scale, inplace=True)
             stl_slices.append(stl_slice)
 
         return stl_slices
 
     @staticmethod
-    def _add_categorization(mesh: pv.PolyData, array_name: str,
-                            vals: list[float], categories: list[str],
-                            colors: list[str], name='label') -> list[str]:
+    def _add_categorization(
+        mesh: pv.PolyData,
+        array_name: str,
+        vals: list[float],
+        categories: list[str],
+        colors: list[str],
+        name="label",
+    ) -> list[str]:
 
         values = mesh[array_name]
-        labels = np.empty(len(values), dtype='<U10')
+        labels = np.empty(len(values), dtype="<U10")
 
         # categories = list(range(0, len(vals)+1))
         labels[:] = categories[-1]
 
         vals.reverse()
         categories.reverse()
         for val, ctg in zip(vals, categories):
@@ -503,16 +523,15 @@
     #             return np.cross(v, [0, 1, 0])
 
     #     return np.cross(v, [1, 0, 0])
 
 
 class Atlas:
 
-    def __init__(self, name: str = 'atlas',
-                 landscape: str = True) -> None:
+    def __init__(self, name: str = "atlas", landscape: str = True) -> None:
         """Class to handle the generation of the Atlas.
 
         Parameters
         ----------
         name : str, optional
             atlas name, by default 'atlas'
         landscape : str, optional
@@ -531,15 +550,15 @@
             to change it, it is recommended to use either the
             docx.shared.Inches or docx.shared.Inches.Mm conversion method.
 
         Examples
         --------
         Build an atlas adding sections manually (recommended, since images
         do not need to be saved to the disk). The images can be produced using
-        py:method:`f4enix.output.plotter.MeshPlotter.plot_slices`. Both a 
+        py:method:`f4enix.output.plotter.MeshPlotter.plot_slices`. Both a
         Word and PDF version are saved.
 
         >>> from f4enix.output.plotter import Atlas
         ... atlas = Atlas('Some title for the atlas')
         ... # reduce for instance the default width for the images
         ... atlas.default_width = atlas.default_width*0.9
         ... # add a section to the atlas containing images produced with
@@ -559,32 +578,37 @@
         # set default width
         section = self.doc.sections[-1]
         margin = 10  # mm
         section.top_margin = Mm(margin)
         section.bottom_margin = Mm(margin)
         section.left_margin = Mm(margin)
         section.right_margin = Mm(margin)
-        width = (section.page_width -
-                 section.left_margin -
-                 section.right_margin)/36000*0.9  # mm
+        width = (
+            (section.page_width - section.left_margin - section.right_margin)
+            / 36000
+            * 0.9
+        )  # mm
         self.default_width = Mm(width)
 
     def _insert_img(self, img: os.PathLike, width=None) -> None:
         if width is None:
             width = self.default_width
         self.doc.add_picture(img, width=width)
         # self.doc.add_picture(img, height=Inches(7.5))
         last_paragraph = self.doc.paragraphs[-1]
         last_paragraph.alignment = WD_ALIGN_PARAGRAPH.CENTER
 
-    def add_section(self, section_name: str,
-                    images: list[tuple[str, Image.Image]],
-                    level: int = 1,
-                    include_section_name: bool = True,
-                    disclaimer: str = None) -> None:
+    def add_section(
+        self,
+        section_name: str,
+        images: list[tuple[str, Image.Image]],
+        level: int = 1,
+        include_section_name: bool = True,
+        disclaimer: str = None,
+    ) -> None:
         """Add a section of plots to the Atlas.
 
         add a chapter to atlas, the level can be decided.
 
         Parameters
         ----------
         section_name : str
@@ -603,21 +627,21 @@
 
         """
 
         self.doc.add_heading(section_name, level=level)
 
         for name, image in images:
             if include_section_name:
-                name = '{} - {}'.format(name, section_name)
+                name = "{} - {}".format(name, section_name)
             if disclaimer is not None:
-                name = name + ' ' + disclaimer
-            self.doc.add_heading(name, level=level+1)
+                name = name + " " + disclaimer
+            self.doc.add_heading(name, level=level + 1)
             # Get a binary stream for pythondocx
             imdata = io.BytesIO()
-            image.save(imdata, format='png')
+            image.save(imdata, format="png")
             imdata.seek(0)
             self._insert_img(imdata)
             # Clean the buffer
             del imdata
 
     def build_from_root(self, root_path: os.PathLike) -> None:
         """Given a root folder, build an atlas with all the pictures found
@@ -645,56 +669,60 @@
             paths = []
             for file in files:
                 paths.append(os.path.join(folderpath, file))
 
             for filepath in sorted(paths, key=os.path.getmtime):
                 heading = os.path.basename(filepath)[:-4]
                 ext = os.path.basename(filepath)[-3:]
-                if ext not in ['jpg', 'png', 'tif']:
+                if ext not in ["jpg", "png", "tif"]:
                     continue
 
                 self.doc.add_heading(heading, level=2)
                 self._insert_img(filepath)
 
     def _change_orientation(self) -> docx.section.Section:
         current_section = self.doc.sections[-1]
-        new_width, new_height = (current_section.page_height,
-                                 current_section.page_width)
+        new_width, new_height = (
+            current_section.page_height,
+            current_section.page_width,
+        )
         new_section = self.doc.add_section()
         new_section.orientation = WD_ORIENT.LANDSCAPE
         new_section.page_width = new_width
         new_section.page_height = new_height
 
         return new_section
 
-    def save(self, outpath: os.PathLike,
-             # pdfprint: bool = True
-             ) -> None:
+    def save(
+        self,
+        outpath: os.PathLike,
+        # pdfprint: bool = True
+    ) -> None:
         """
         Save word atlas and possibly export PDF
 
         Parameters
         ----------
         outpath : os.PathLike
             path to the folder where to save the atlas(es)
 
         Returns
         -------
         None.
 
         """
-        outpath_word = os.path.join(outpath, self.name+'.docx')
+        outpath_word = os.path.join(outpath, self.name + ".docx")
         # outpath_pdf = os.path.join(outpath, self.name+'.pdf')
 
         try:
             self.doc.save(outpath_word)
         except FileNotFoundError as e:
-            print(' The following is the original exception:')
+            print(" The following is the original exception:")
             print(e)
-            print('\n it may be due to invalid characters in the file name')
+            print("\n it may be due to invalid characters in the file name")
 
         # if pdfprint:
         #     in_file = outpath_word
         #     out_file = outpath_pdf
 
         #     try:
         #         word = win32com.client.Dispatch('Word.Application')
@@ -765,16 +793,17 @@
     #     shading_elm_1 = parse_xml(r'<w:shd {} w:fill="'.format(nsdecls('w')) +
     #                               color + r'"/>')
     #     cell._tc.get_or_add_tcPr().append(shading_elm_1)
 
 
 class Plotter2D(ABC):
 
-    def __init__(self, suptitle: str = None, xlabel: str = None,
-                 ylabel: str = None) -> None:
+    def __init__(
+        self, suptitle: str = None, xlabel: str = None, ylabel: str = None
+    ) -> None:
         """Abstract class for the definition of 2D plots.
 
         Parameters
         ----------
         suptitle : str, optional
             title of the plot, by default None
         xlabel : str, optional
@@ -796,51 +825,60 @@
             colors used in the plots. They compose a color-blind friendly
             palette.
 
         """
         fig, ax = plt.subplots()
 
         # Some default actions
-        ax.grid(alpha=0.6, which='both')
+        ax.grid(alpha=0.6, which="both")
         if suptitle is not None:
             ax.set_title(suptitle)
         if ylabel is not None:
             ax.set_ylabel(ylabel)
         if xlabel is not None:
             ax.set_xlabel(xlabel)
 
         # store the default
         self.fig = fig
         self.ax = ax
 
         # May be improved in the future with additional markers and colors
         # plot decorators
-        self.markers = ['o', 's', 'D', '^', 'X', 'p', 'd', '*']*50
-        self.lines = ['-', '--', '-.', ':']*50
+        self.markers = ["o", "s", "D", "^", "X", "p", "d", "*"] * 50
+        self.lines = ["-", "--", "-.", ":"] * 50
         # Color-blind friendly palette
-        self.colors = ['#377eb8', '#ff7f00', '#4daf4a', '#f781bf', '#a65628',
-                       '#984ea3', '#999999', '#e41a1c', '#dede00']*50
-        logging.debug('plotter initialized')
+        self.colors = [
+            "#377eb8",
+            "#ff7f00",
+            "#4daf4a",
+            "#f781bf",
+            "#a65628",
+            "#984ea3",
+            "#999999",
+            "#e41a1c",
+            "#dede00",
+        ] * 50
+        logging.debug("plotter initialized")
 
     @abstractmethod
     def plot(self) -> None:
         pass
 
     def save(self, outpath: os.PathLike) -> None:
-        self.fig.savefig(outpath, dpi=300, bbox_inches='tight')
-        logging.info('plot has been saved at {}'.format(outpath))
+        self.fig.savefig(outpath, dpi=300, bbox_inches="tight")
+        logging.info("plot has been saved at {}".format(outpath))
 
 
 class CDFplot(Plotter2D):
-    def __init__(self, suptitle: str = None,
-                 xlabel: str = None,
-                 ylabel: str = None) -> None:
+    def __init__(
+        self, suptitle: str = None, xlabel: str = None, ylabel: str = None
+    ) -> None:
         """Plotter for cumulative distributions.
 
-        all datasets of observations are automatically binnned and plotted as 
+        all datasets of observations are automatically binnned and plotted as
         (unfilled) histograms.
 
         Parameters
         ----------
         suptitle : str, optional
             title of the plot, by default None
         xlabel : str, optional
@@ -861,18 +899,24 @@
         colors : list[str]
             colors used in the plots. They compose a color-blind friendly
             palette.
 
         """
         super().__init__(suptitle, xlabel, ylabel)
 
-    def plot(self, values_list: list, bins: int = 10,
-             datalabels: list[str] = None, perc: bool = True,
-             outside_legend: bool = False, cut_y: float = None,
-             cut_x: float = None) -> None:
+    def plot(
+        self,
+        values_list: list,
+        bins: int = 10,
+        datalabels: list[str] = None,
+        perc: bool = True,
+        outside_legend: bool = False,
+        cut_y: float = None,
+        cut_x: float = None,
+    ) -> None:
         """plot the comulative distributions as discrete steps
 
         Parameters
         ----------
         values_list : list
             list of list of values containing the occurencies to be analyzed
         bins : int, optional
@@ -892,33 +936,39 @@
             cut the x axis to a specific value, by default is None.
         """
         # check that the length of labels is consisting
         if datalabels is not None:
             try:
                 assert len(datalabels) == len(values_list)
             except AssertionError:
-                msg = 'leghth of values ({}) is different from lenght of labels ({})'
+                msg = "leghth of values ({}) is different from lenght of labels ({})"
                 raise ValueError(msg.format(len(values_list), len(datalabels)))
 
         for i, values in enumerate(values_list):
             if datalabels is not None:
                 label = datalabels[i]
             else:
                 label = None
 
-            self.ax.hist(values, bins=bins, histtype='step',
-                         weights=np.ones(len(values))/len(values),
-                         cumulative=True, label=label, linestyle=self.lines[i],
-                         color=self.colors[i])
+            self.ax.hist(
+                values,
+                bins=bins,
+                histtype="step",
+                weights=np.ones(len(values)) / len(values),
+                cumulative=True,
+                label=label,
+                linestyle=self.lines[i],
+                color=self.colors[i],
+            )
             if perc:
                 self.ax.yaxis.set_major_formatter(PercentFormatter(1))
 
         if outside_legend:
             self.ax.legend(framealpha=1, bbox_to_anchor=(1, 1))
         else:
-            self.ax.legend(loc='lower right', framealpha=1)
+            self.ax.legend(loc="lower right", framealpha=1)
 
         if cut_y is not None:
             self.ax.set_ylim(top=cut_y)
         if cut_x is not None:
             self.ax.set_xlim(right=cut_x)
-        logging.info('CDF was plotted')
+        logging.info("CDF was plotted")
```

### Comparing `f4enix-0.5.2/f4enix/output/rssa.py` & `f4enix-0.6.0/f4enix/output/rssa.py`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.2/f4enix/resources/Isotopes.txt` & `f4enix-0.6.0/f4enix/resources/Isotopes.txt`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.2/f4enix/resources/activation_libs.xlsx` & `f4enix-0.6.0/f4enix/resources/activation_libs.xlsx`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.2/f4enix/resources/xsdir.txt` & `f4enix-0.6.0/f4enix/resources/xsdir.txt`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.2/f4enix.egg-info/PKG-INFO` & `f4enix-0.6.0/f4enix.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: f4enix
-Version: 0.5.2
+Version: 0.6.0
 Summary: API for Monte Carlo input and output parsing
 Author: F4E neutronics team
 Author-email: sc-radiationtransport@f4e.europa.eu
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: appdirs
 Requires-Dist: asttokens
 Requires-Dist: attrs
 Requires-Dist: backcall
 Requires-Dist: charset-normalizer
@@ -74,15 +74,15 @@
 [![Testing linux](https://github.com/Radiation-Transport/F4Enix/actions/workflows/AutomatedTests_linux.yml/badge.svg?branch=main)](https://github.com/Radiation-Transport/F4Enix/actions/workflows/AutomatedTests_linux.yml)
 [![PyPi version](https://badgen.net/pypi/v/f4enix/)](https://pypi.org/project/f4enix)
 [![Documentation Status](https://readthedocs.org/projects/f4enix/badge/?version=latest)](https://f4enix.readthedocs.io/en/latest/?badge=latest)
 
 # F4Enix
 Parser for Monte Carlo simulations input and output files
 
-**Pyhton >3.10!**
+**Pyhton >3.9!**
 
 Both Windows and Linux supported.
 
 Go to [F4Enix official documentation](https://f4enix.readthedocs.io/en/latest/) to get
 more information on the library capabilities, examples and much more.
 
 ## Install
@@ -95,15 +95,15 @@
 ### Troubleshooting and developer mode
 If any unexpected issue is encountered during installation, the first step for
 its resolution would be to create a new fresh virtual environment.
 In conda this would be done with:
 ```
 conda create -n <env_name> python=3.10
 ```
-Please remeber that python versions lower than 3.10 are not supported.
+Please remember that python versions lower than 3.10 are not supported.
 
 ### Developer mode installation
 There are many situations (especially while being an active developer) where it may be useful to install f4enix in developer mode. In order to do so, navigate to the
 F4Eparser folder and type the following to be sure that your pip is
 up to date (optional):
 ```
 python -m pip install --upgrade pip setuptools wheel
```

### Comparing `f4enix-0.5.2/f4enix.egg-info/SOURCES.txt` & `f4enix-0.6.0/f4enix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.2/f4enix.egg-info/requires.txt` & `f4enix-0.6.0/f4enix.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.2/setup.cfg` & `f4enix-0.6.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 [options]
 packages = 
 	f4enix
 	f4enix.input
 	f4enix.input.ww_gvr
 	f4enix.output
 	f4enix.resources
-python_requires = >= 3.10
+python_requires = >= 3.9
 install_requires = 
 	appdirs
 	asttokens
 	attrs
 	backcall
 	charset-normalizer
 	colorama
```

### Comparing `f4enix-0.5.2/tests/test_cuv_sampling_error.py` & `f4enix-0.6.0/tests/test_cuv_sampling_error.py`

 * *Files identical despite different names*

