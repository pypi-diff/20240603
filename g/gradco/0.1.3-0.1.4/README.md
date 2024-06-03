# Comparing `tmp/gradco-0.1.3.tar.gz` & `tmp/gradco-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gradco-0.1.3.tar", last modified: Wed May 22 15:07:46 2024, max compression
+gzip compressed data, was "gradco-0.1.4.tar", last modified: Mon Jun  3 10:26:45 2024, max compression
```

## Comparing `gradco-0.1.3.tar` & `gradco-0.1.4.tar`

### file list

```diff
@@ -1,76 +1,77 @@
-drwxr-xr-x   0 windels    (502) staff       (20)        0 2024-05-22 15:07:46.132481 gradco-0.1.3/
--rw-r--r--   0 windels    (502) staff       (20)      158 2023-07-04 12:55:34.000000 gradco-0.1.3/AUTHORS.rst
--rw-r--r--   0 windels    (502) staff       (20)     2978 2023-07-04 12:55:34.000000 gradco-0.1.3/CONTRIBUTING.rst
--rw-r--r--   0 windels    (502) staff       (20)       97 2023-07-04 12:55:34.000000 gradco-0.1.3/HISTORY.rst
--rw-r--r--   0 windels    (502) staff       (20)    20849 2024-05-22 15:06:18.000000 gradco-0.1.3/LICENSE
--rw-r--r--   0 windels    (502) staff       (20)      100 2023-07-04 12:55:34.000000 gradco-0.1.3/MANIFEST.in
--rw-r--r--   0 windels    (502) staff       (20)      204 2024-05-22 15:07:46.130172 gradco-0.1.3/PKG-INFO
--rw-r--r--   0 windels    (502) staff       (20)      409 2023-07-04 12:55:34.000000 gradco-0.1.3/README.rst
-drwxr-xr-x   0 windels    (502) staff       (20)        0 2024-05-22 15:07:46.092654 gradco-0.1.3/c_module/
--rw-r--r--   0 windels    (502) staff       (20)     4362 2024-02-16 11:24:52.000000 gradco-0.1.3/c_module/dense_matrix.cpp
--rw-r--r--   0 windels    (502) staff       (20)     1084 2024-02-16 11:24:52.000000 gradco-0.1.3/c_module/dense_matrix.hh
--rw-r--r--   0 windels    (502) staff       (20)     4086 2023-12-28 11:03:57.000000 gradco-0.1.3/c_module/directed_graph.cpp
--rw-r--r--   0 windels    (502) staff       (20)     1048 2023-12-27 08:52:51.000000 gradco-0.1.3/c_module/directed_graph.hh
--rw-r--r--   0 windels    (502) staff       (20)    21422 2024-02-16 11:24:52.000000 gradco-0.1.3/c_module/gradco_module.cpp
--rw-r--r--   0 windels    (502) staff       (20)      969 2024-01-17 12:42:27.000000 gradco-0.1.3/c_module/matrix.hh
--rw-r--r--   0 windels    (502) staff       (20)     4957 2024-02-16 11:24:52.000000 gradco-0.1.3/c_module/sparse_matrix.cpp
--rw-r--r--   0 windels    (502) staff       (20)     1406 2024-02-16 11:24:52.000000 gradco-0.1.3/c_module/sparse_matrix.hh
--rw-r--r--   0 windels    (502) staff       (20)     4779 2024-02-16 11:24:52.000000 gradco-0.1.3/c_module/symmetric_dense_matrix.cpp
--rw-r--r--   0 windels    (502) staff       (20)     1118 2024-02-16 11:24:52.000000 gradco-0.1.3/c_module/symmetric_dense_matrix.hh
--rw-r--r--   0 windels    (502) staff       (20)    74463 2023-12-27 08:52:51.000000 gradco-0.1.3/c_module/unordered_dense.h
-drwxr-xr-x   0 windels    (502) staff       (20)        0 2024-05-22 15:07:46.095701 gradco-0.1.3/docs/
--rw-r--r--   0 windels    (502) staff       (20)     6778 2023-07-04 12:55:34.000000 gradco-0.1.3/docs/Makefile
--rw-r--r--   0 windels    (502) staff       (20)       28 2023-07-04 12:55:34.000000 gradco-0.1.3/docs/authors.rst
--rw-r--r--   0 windels    (502) staff       (20)     8155 2023-07-04 12:55:34.000000 gradco-0.1.3/docs/conf.py
--rw-r--r--   0 windels    (502) staff       (20)       33 2023-07-04 12:55:34.000000 gradco-0.1.3/docs/contributing.rst
--rw-r--r--   0 windels    (502) staff       (20)       28 2023-07-04 12:55:34.000000 gradco-0.1.3/docs/history.rst
--rw-r--r--   0 windels    (502) staff       (20)      688 2023-07-04 12:55:34.000000 gradco-0.1.3/docs/index.rst
--rw-r--r--   0 windels    (502) staff       (20)      244 2023-07-04 12:55:34.000000 gradco-0.1.3/docs/installation.rst
--rw-r--r--   0 windels    (502) staff       (20)     6709 2023-07-04 12:55:34.000000 gradco-0.1.3/docs/make.bat
--rw-r--r--   0 windels    (502) staff       (20)       90 2023-07-04 12:55:34.000000 gradco-0.1.3/docs/usage.rst
-drwxr-xr-x   0 windels    (502) staff       (20)        0 2024-05-22 15:07:46.096747 gradco-0.1.3/generate_tests/
--rw-r--r--   0 windels    (502) staff       (20)       92 2023-07-04 12:55:34.000000 gradco-0.1.3/generate_tests/bit_array_to_graphlet_signatures_3nodes.csv
--rw-r--r--   0 windels    (502) staff       (20)     1422 2023-07-04 12:55:34.000000 gradco-0.1.3/generate_tests/bit_array_to_graphlet_signatures_4nodes.csv
--rw-r--r--   0 windels    (502) staff       (20)     9294 2023-07-04 12:55:34.000000 gradco-0.1.3/generate_tests/generate_unit_test_code.py
--rw-r--r--   0 windels    (502) staff       (20)     4613 2023-07-23 12:45:41.000000 gradco-0.1.3/generate_tests/generate_unit_test_code_orbit_adjacency.py
--rwxr-xr-x   0 windels    (502) staff       (20)   130744 2023-07-04 12:55:34.000000 gradco-0.1.3/generate_tests/orca
-drwxr-xr-x   0 windels    (502) staff       (20)        0 2024-05-22 15:07:46.129945 gradco-0.1.3/gradco.egg-info/
--rw-r--r--   0 windels    (502) staff       (20)      204 2024-05-22 15:07:46.000000 gradco-0.1.3/gradco.egg-info/PKG-INFO
--rw-r--r--   0 windels    (502) staff       (20)     1601 2024-05-22 15:07:46.000000 gradco-0.1.3/gradco.egg-info/SOURCES.txt
--rw-r--r--   0 windels    (502) staff       (20)        1 2024-05-22 15:07:46.000000 gradco-0.1.3/gradco.egg-info/dependency_links.txt
--rw-r--r--   0 windels    (502) staff       (20)       25 2024-05-22 15:07:46.000000 gradco-0.1.3/gradco.egg-info/top_level.txt
--rw-r--r--   0 windels    (502) staff       (20)    15781 2024-05-22 14:56:58.000000 gradco-0.1.3/gradco.py
--rwxr-xr-x   0 windels    (502) staff       (20)  2580760 2023-07-04 12:55:34.000000 gradco-0.1.3/ncount2
--rw-r--r--   0 windels    (502) staff       (20)      546 2024-05-22 13:05:59.000000 gradco-0.1.3/pyproject.toml
--rw-r--r--   0 windels    (502) staff       (20)    48654 2024-01-18 15:31:58.000000 gradco-0.1.3/python_count_functions.py
--rw-r--r--   0 windels    (502) staff       (20)       61 2024-05-22 15:07:46.133005 gradco-0.1.3/setup.cfg
--rw-r--r--   0 windels    (502) staff       (20)     1691 2024-05-22 15:06:47.000000 gradco-0.1.3/setup.py
-drwxr-xr-x   0 windels    (502) staff       (20)        0 2024-05-22 15:07:46.129478 gradco-0.1.3/test/
--rw-r--r--   0 windels    (502) staff       (20)        0 2023-12-20 14:53:52.000000 gradco-0.1.3/test/__init__.py
--rw-r--r--   0 windels    (502) staff       (20)   160734 2023-12-28 11:03:57.000000 gradco-0.1.3/test/test_A10_10_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   160734 2023-12-28 11:03:57.000000 gradco-0.1.3/test/test_A10_11_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   160734 2023-12-28 11:03:57.000000 gradco-0.1.3/test/test_A12_12_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   160734 2023-12-28 11:03:57.000000 gradco-0.1.3/test/test_A12_13_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   160734 2023-12-28 11:03:57.000000 gradco-0.1.3/test/test_A13_13_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   160739 2023-12-28 11:03:57.000000 gradco-0.1.3/test/test_A14_14_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.3/test/test_A1_1_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.3/test/test_A1_2_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   158721 2023-12-28 11:03:57.000000 gradco-0.1.3/test/test_A3_3_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.3/test/test_A4_4_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.3/test/test_A4_5_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.3/test/test_A5_5_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.3/test/test_A6_6_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.3/test/test_A6_7_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.3/test/test_A8_8_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   159710 2023-12-28 11:03:57.000000 gradco-0.1.3/test/test_A9_10_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   159710 2023-12-28 11:03:57.000000 gradco-0.1.3/test/test_A9_11_orca.py
--rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.3/test/test_G1_windels.py
--rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.3/test/test_G2_windels.py
--rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.3/test/test_G3_windels.py
--rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.3/test/test_G4_windels.py
--rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.3/test/test_G5_windels.py
--rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.3/test/test_G6_windels.py
--rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.3/test/test_G7_windels.py
--rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.3/test/test_G8_windels.py
--rw-r--r--   0 windels    (502) staff       (20)     5202 2024-02-16 11:24:52.000000 gradco-0.1.3/test/test_helper.py
--rw-r--r--   0 windels    (502) staff       (20)      498 2023-07-04 12:55:34.000000 gradco-0.1.3/tox.ini
+drwxr-xr-x   0 windels    (502) staff       (20)        0 2024-06-03 10:26:45.390753 gradco-0.1.4/
+-rw-r--r--   0 windels    (502) staff       (20)      158 2023-07-04 12:55:34.000000 gradco-0.1.4/AUTHORS.rst
+-rw-r--r--   0 windels    (502) staff       (20)     2978 2023-07-04 12:55:34.000000 gradco-0.1.4/CONTRIBUTING.rst
+-rw-r--r--   0 windels    (502) staff       (20)       97 2023-07-04 12:55:34.000000 gradco-0.1.4/HISTORY.rst
+-rw-r--r--   0 windels    (502) staff       (20)    20849 2024-05-22 15:06:18.000000 gradco-0.1.4/LICENSE
+-rw-r--r--   0 windels    (502) staff       (20)      100 2023-07-04 12:55:34.000000 gradco-0.1.4/MANIFEST.in
+-rw-r--r--   0 windels    (502) staff       (20)     2412 2024-06-03 10:26:45.390677 gradco-0.1.4/PKG-INFO
+-rw-r--r--   0 windels    (502) staff       (20)      409 2023-07-04 12:55:34.000000 gradco-0.1.4/README.rst
+drwxr-xr-x   0 windels    (502) staff       (20)        0 2024-06-03 10:26:45.356835 gradco-0.1.4/c_module/
+-rw-r--r--   0 windels    (502) staff       (20)     4362 2024-02-16 11:24:52.000000 gradco-0.1.4/c_module/dense_matrix.cpp
+-rw-r--r--   0 windels    (502) staff       (20)     1084 2024-02-16 11:24:52.000000 gradco-0.1.4/c_module/dense_matrix.hh
+-rw-r--r--   0 windels    (502) staff       (20)     4086 2023-12-28 11:03:57.000000 gradco-0.1.4/c_module/directed_graph.cpp
+-rw-r--r--   0 windels    (502) staff       (20)     1048 2023-12-27 08:52:51.000000 gradco-0.1.4/c_module/directed_graph.hh
+-rw-r--r--   0 windels    (502) staff       (20)    21422 2024-02-16 11:24:52.000000 gradco-0.1.4/c_module/gradco_module.cpp
+-rw-r--r--   0 windels    (502) staff       (20)      969 2024-01-17 12:42:27.000000 gradco-0.1.4/c_module/matrix.hh
+-rw-r--r--   0 windels    (502) staff       (20)     4957 2024-02-16 11:24:52.000000 gradco-0.1.4/c_module/sparse_matrix.cpp
+-rw-r--r--   0 windels    (502) staff       (20)     1406 2024-02-16 11:24:52.000000 gradco-0.1.4/c_module/sparse_matrix.hh
+-rw-r--r--   0 windels    (502) staff       (20)     4779 2024-02-16 11:24:52.000000 gradco-0.1.4/c_module/symmetric_dense_matrix.cpp
+-rw-r--r--   0 windels    (502) staff       (20)     1118 2024-02-16 11:24:52.000000 gradco-0.1.4/c_module/symmetric_dense_matrix.hh
+-rw-r--r--   0 windels    (502) staff       (20)    74463 2023-12-27 08:52:51.000000 gradco-0.1.4/c_module/unordered_dense.h
+drwxr-xr-x   0 windels    (502) staff       (20)        0 2024-06-03 10:26:45.360614 gradco-0.1.4/docs/
+-rw-r--r--   0 windels    (502) staff       (20)     6778 2023-07-04 12:55:34.000000 gradco-0.1.4/docs/Makefile
+-rw-r--r--   0 windels    (502) staff       (20)       28 2023-07-04 12:55:34.000000 gradco-0.1.4/docs/authors.rst
+-rw-r--r--   0 windels    (502) staff       (20)     8155 2023-07-04 12:55:34.000000 gradco-0.1.4/docs/conf.py
+-rw-r--r--   0 windels    (502) staff       (20)       33 2023-07-04 12:55:34.000000 gradco-0.1.4/docs/contributing.rst
+-rw-r--r--   0 windels    (502) staff       (20)       28 2023-07-04 12:55:34.000000 gradco-0.1.4/docs/history.rst
+-rw-r--r--   0 windels    (502) staff       (20)      688 2023-07-04 12:55:34.000000 gradco-0.1.4/docs/index.rst
+-rw-r--r--   0 windels    (502) staff       (20)      244 2023-07-04 12:55:34.000000 gradco-0.1.4/docs/installation.rst
+-rw-r--r--   0 windels    (502) staff       (20)     6709 2023-07-04 12:55:34.000000 gradco-0.1.4/docs/make.bat
+-rw-r--r--   0 windels    (502) staff       (20)       90 2023-07-04 12:55:34.000000 gradco-0.1.4/docs/usage.rst
+drwxr-xr-x   0 windels    (502) staff       (20)        0 2024-06-03 10:26:45.362043 gradco-0.1.4/generate_tests/
+-rw-r--r--   0 windels    (502) staff       (20)       92 2023-07-04 12:55:34.000000 gradco-0.1.4/generate_tests/bit_array_to_graphlet_signatures_3nodes.csv
+-rw-r--r--   0 windels    (502) staff       (20)     1422 2023-07-04 12:55:34.000000 gradco-0.1.4/generate_tests/bit_array_to_graphlet_signatures_4nodes.csv
+-rw-r--r--   0 windels    (502) staff       (20)     9294 2023-07-04 12:55:34.000000 gradco-0.1.4/generate_tests/generate_unit_test_code.py
+-rw-r--r--   0 windels    (502) staff       (20)     4613 2023-07-23 12:45:41.000000 gradco-0.1.4/generate_tests/generate_unit_test_code_orbit_adjacency.py
+-rwxr-xr-x   0 windels    (502) staff       (20)   130744 2023-07-04 12:55:34.000000 gradco-0.1.4/generate_tests/orca
+drwxr-xr-x   0 windels    (502) staff       (20)        0 2024-06-03 10:26:45.390401 gradco-0.1.4/gradco.egg-info/
+-rw-r--r--   0 windels    (502) staff       (20)     2412 2024-06-03 10:26:45.000000 gradco-0.1.4/gradco.egg-info/PKG-INFO
+-rw-r--r--   0 windels    (502) staff       (20)     1622 2024-06-03 10:26:45.000000 gradco-0.1.4/gradco.egg-info/SOURCES.txt
+-rw-r--r--   0 windels    (502) staff       (20)        1 2024-06-03 10:26:45.000000 gradco-0.1.4/gradco.egg-info/dependency_links.txt
+-rw-r--r--   0 windels    (502) staff       (20)       25 2024-06-03 10:26:45.000000 gradco-0.1.4/gradco.egg-info/top_level.txt
+-rw-r--r--   0 windels    (502) staff       (20)    15781 2024-05-22 14:56:58.000000 gradco-0.1.4/gradco.py
+-rwxr-xr-x   0 windels    (502) staff       (20)  2580760 2023-07-04 12:55:34.000000 gradco-0.1.4/ncount2
+-rw-r--r--   0 windels    (502) staff       (20)     2207 2024-06-03 10:26:35.000000 gradco-0.1.4/pypi_description.rst
+-rw-r--r--   0 windels    (502) staff       (20)      546 2024-05-22 13:05:59.000000 gradco-0.1.4/pyproject.toml
+-rw-r--r--   0 windels    (502) staff       (20)    48654 2024-01-18 15:31:58.000000 gradco-0.1.4/python_count_functions.py
+-rw-r--r--   0 windels    (502) staff       (20)       61 2024-06-03 10:26:45.390975 gradco-0.1.4/setup.cfg
+-rw-r--r--   0 windels    (502) staff       (20)     1843 2024-06-03 10:15:48.000000 gradco-0.1.4/setup.py
+drwxr-xr-x   0 windels    (502) staff       (20)        0 2024-06-03 10:26:45.389378 gradco-0.1.4/test/
+-rw-r--r--   0 windels    (502) staff       (20)        0 2023-12-20 14:53:52.000000 gradco-0.1.4/test/__init__.py
+-rw-r--r--   0 windels    (502) staff       (20)   160734 2023-12-28 11:03:57.000000 gradco-0.1.4/test/test_A10_10_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   160734 2023-12-28 11:03:57.000000 gradco-0.1.4/test/test_A10_11_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   160734 2023-12-28 11:03:57.000000 gradco-0.1.4/test/test_A12_12_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   160734 2023-12-28 11:03:57.000000 gradco-0.1.4/test/test_A12_13_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   160734 2023-12-28 11:03:57.000000 gradco-0.1.4/test/test_A13_13_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   160739 2023-12-28 11:03:57.000000 gradco-0.1.4/test/test_A14_14_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.4/test/test_A1_1_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.4/test/test_A1_2_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   158721 2023-12-28 11:03:57.000000 gradco-0.1.4/test/test_A3_3_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.4/test/test_A4_4_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.4/test/test_A4_5_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.4/test/test_A5_5_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.4/test/test_A6_6_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.4/test/test_A6_7_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   158686 2023-12-28 11:03:57.000000 gradco-0.1.4/test/test_A8_8_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   159710 2023-12-28 11:03:57.000000 gradco-0.1.4/test/test_A9_10_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   159710 2023-12-28 11:03:57.000000 gradco-0.1.4/test/test_A9_11_orca.py
+-rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.4/test/test_G1_windels.py
+-rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.4/test/test_G2_windels.py
+-rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.4/test/test_G3_windels.py
+-rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.4/test/test_G4_windels.py
+-rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.4/test/test_G5_windels.py
+-rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.4/test/test_G6_windels.py
+-rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.4/test/test_G7_windels.py
+-rw-r--r--   0 windels    (502) staff       (20)   177127 2023-12-27 08:52:51.000000 gradco-0.1.4/test/test_G8_windels.py
+-rw-r--r--   0 windels    (502) staff       (20)     5202 2024-02-16 11:24:52.000000 gradco-0.1.4/test/test_helper.py
+-rw-r--r--   0 windels    (502) staff       (20)      498 2023-07-04 12:55:34.000000 gradco-0.1.4/tox.ini
```

### Comparing `gradco-0.1.3/CONTRIBUTING.rst` & `gradco-0.1.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/LICENSE` & `gradco-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/c_module/dense_matrix.cpp` & `gradco-0.1.4/c_module/dense_matrix.cpp`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/c_module/dense_matrix.hh` & `gradco-0.1.4/c_module/dense_matrix.hh`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/c_module/directed_graph.cpp` & `gradco-0.1.4/c_module/directed_graph.cpp`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/c_module/directed_graph.hh` & `gradco-0.1.4/c_module/directed_graph.hh`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/c_module/gradco_module.cpp` & `gradco-0.1.4/c_module/gradco_module.cpp`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/c_module/matrix.hh` & `gradco-0.1.4/c_module/matrix.hh`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/c_module/sparse_matrix.cpp` & `gradco-0.1.4/c_module/sparse_matrix.cpp`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/c_module/sparse_matrix.hh` & `gradco-0.1.4/c_module/sparse_matrix.hh`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/c_module/symmetric_dense_matrix.cpp` & `gradco-0.1.4/c_module/symmetric_dense_matrix.cpp`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/c_module/symmetric_dense_matrix.hh` & `gradco-0.1.4/c_module/symmetric_dense_matrix.hh`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/c_module/unordered_dense.h` & `gradco-0.1.4/c_module/unordered_dense.h`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/docs/Makefile` & `gradco-0.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/docs/conf.py` & `gradco-0.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/docs/index.rst` & `gradco-0.1.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/docs/make.bat` & `gradco-0.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/generate_tests/bit_array_to_graphlet_signatures_4nodes.csv` & `gradco-0.1.4/generate_tests/bit_array_to_graphlet_signatures_4nodes.csv`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/generate_tests/generate_unit_test_code.py` & `gradco-0.1.4/generate_tests/generate_unit_test_code.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/generate_tests/generate_unit_test_code_orbit_adjacency.py` & `gradco-0.1.4/generate_tests/generate_unit_test_code_orbit_adjacency.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/generate_tests/orca` & `gradco-0.1.4/generate_tests/orca`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/gradco.egg-info/SOURCES.txt` & `gradco-0.1.4/gradco.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 CONTRIBUTING.rst
 HISTORY.rst
 LICENSE
 MANIFEST.in
 README.rst
 gradco.py
 ncount2
+pypi_description.rst
 pyproject.toml
 python_count_functions.py
 setup.cfg
 setup.py
 tox.ini
 c_module/dense_matrix.cpp
 c_module/dense_matrix.hh
```

### Comparing `gradco-0.1.3/gradco.py` & `gradco-0.1.4/gradco.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/ncount2` & `gradco-0.1.4/ncount2`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/pyproject.toml` & `gradco-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/python_count_functions.py` & `gradco-0.1.4/python_count_functions.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/setup.py` & `gradco-0.1.4/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,20 +23,24 @@
                          extra_compile_args=['-std=c++17', '-O3'],
                          )
     # c++20
     # gnu++20
     # c++2b => 23 working draft
     # gnu++2b => working draft with GNU extensions
 
+    long_description = open("pypi_description.rst").read()
+
     setup(name="gradco",  # Name of the package. Used at install: pip install gradco
-          version="0.1.3",
-          description="GRaphled-orbit ADjacency COunter (GRADCO).",
+          version="0.1.4",
+          description="GRaphlet-orbit ADjacency COunter (GRADCO).",
           author="Sam Windels",
           author_email="sam.windels@gmail.com",
           ext_modules=[c_module],
+          data_files=['pypi_description.rst'],
+          long_description=long_description,
           # Refers to gradco.py. Name of the module. Used as: import gradco
           py_modules=["gradco"],
           python_requires='>=3.10',
           license_files=('LICENSE',),
           )
```

### Comparing `gradco-0.1.3/test/test_A10_10_orca.py` & `gradco-0.1.4/test/test_A10_10_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/test/test_A10_11_orca.py` & `gradco-0.1.4/test/test_A10_11_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/test/test_A12_12_orca.py` & `gradco-0.1.4/test/test_A12_12_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/test/test_A12_13_orca.py` & `gradco-0.1.4/test/test_A12_13_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/test/test_A13_13_orca.py` & `gradco-0.1.4/test/test_A13_13_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/test/test_A14_14_orca.py` & `gradco-0.1.4/test/test_A14_14_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/test/test_A1_1_orca.py` & `gradco-0.1.4/test/test_A1_1_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/test/test_A1_2_orca.py` & `gradco-0.1.4/test/test_A1_2_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/test/test_A3_3_orca.py` & `gradco-0.1.4/test/test_A3_3_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/test/test_A4_4_orca.py` & `gradco-0.1.4/test/test_A4_4_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/test/test_A4_5_orca.py` & `gradco-0.1.4/test/test_A4_5_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/test/test_A5_5_orca.py` & `gradco-0.1.4/test/test_A5_5_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/test/test_A6_6_orca.py` & `gradco-0.1.4/test/test_A6_6_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/test/test_A6_7_orca.py` & `gradco-0.1.4/test/test_A6_7_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/test/test_A8_8_orca.py` & `gradco-0.1.4/test/test_A8_8_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/test/test_A9_10_orca.py` & `gradco-0.1.4/test/test_A9_10_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/test/test_A9_11_orca.py` & `gradco-0.1.4/test/test_A9_11_orca.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/test/test_G1_windels.py` & `gradco-0.1.4/test/test_G1_windels.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/test/test_G2_windels.py` & `gradco-0.1.4/test/test_G2_windels.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/test/test_G3_windels.py` & `gradco-0.1.4/test/test_G3_windels.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/test/test_G4_windels.py` & `gradco-0.1.4/test/test_G4_windels.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/test/test_G5_windels.py` & `gradco-0.1.4/test/test_G5_windels.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/test/test_G6_windels.py` & `gradco-0.1.4/test/test_G6_windels.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/test/test_G7_windels.py` & `gradco-0.1.4/test/test_G7_windels.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/test/test_G8_windels.py` & `gradco-0.1.4/test/test_G8_windels.py`

 * *Files identical despite different names*

### Comparing `gradco-0.1.3/test/test_helper.py` & `gradco-0.1.4/test/test_helper.py`

 * *Files identical despite different names*

