# Comparing `tmp/ngo-1.0.1.tar.gz` & `tmp/ngo-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngo-1.0.1.tar", last modified: Tue Mar 19 14:36:48 2024, max compression
+gzip compressed data, was "ngo-1.0.2.tar", last modified: Mon Jun  3 12:53:42 2024, max compression
```

## Comparing `ngo-1.0.1.tar` & `ngo-1.0.2.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:36:48.763271 ngo-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-19 14:36:44.000000 ngo-1.0.1/.envrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:36:48.751270 ngo-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:36:48.751270 ngo-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-03-19 14:36:44.000000 ngo-1.0.1/.github/workflows/buildwheel.yml
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-19 14:36:44.000000 ngo-1.0.1/.github/workflows/cd-pre.yml
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-19 14:36:44.000000 ngo-1.0.1/.github/workflows/cd.yml
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-19 14:36:44.000000 ngo-1.0.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-03-19 14:36:44.000000 ngo-1.0.1/.github/workflows/publish-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-03-19 14:36:44.000000 ngo-1.0.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-03-19 14:36:44.000000 ngo-1.0.1/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-03-19 14:36:44.000000 ngo-1.0.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-03-19 14:36:44.000000 ngo-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-19 14:36:44.000000 ngo-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-03-19 14:36:44.000000 ngo-1.0.1/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-03-19 14:36:44.000000 ngo-1.0.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-03-19 14:36:44.000000 ngo-1.0.1/DEVELOPMENT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-19 14:36:44.000000 ngo-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-03-19 14:36:48.763271 ngo-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-03-19 14:36:44.000000 ngo-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-03-19 14:36:44.000000 ngo-1.0.1/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-03-19 14:36:44.000000 ngo-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 14:36:48.763271 ngo-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:36:48.751270 ngo-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:36:48.755271 ngo-1.0.1/src/ngo/
--rw-r--r--   0 runner    (1001) docker     (127)     7164 2024-03-19 14:36:44.000000 ngo-1.0.1/src/ngo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-03-19 14:36:44.000000 ngo-1.0.1/src/ngo/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-03-19 14:36:44.000000 ngo-1.0.1/src/ngo/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    13490 2024-03-19 14:36:44.000000 ngo-1.0.1/src/ngo/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)    29338 2024-03-19 14:36:44.000000 ngo-1.0.1/src/ngo/dependency.py
--rw-r--r--   0 runner    (1001) docker     (127)    22383 2024-03-19 14:36:44.000000 ngo-1.0.1/src/ngo/inline.py
--rw-r--r--   0 runner    (1001) docker     (127)    15092 2024-03-19 14:36:44.000000 ngo-1.0.1/src/ngo/literal_duplication.py
--rw-r--r--   0 runner    (1001) docker     (127)    29603 2024-03-19 14:36:44.000000 ngo-1.0.1/src/ngo/math_simplification.py
--rw-r--r--   0 runner    (1001) docker     (127)    30773 2024-03-19 14:36:44.000000 ngo-1.0.1/src/ngo/minmax_aggregates.py
--rw-r--r--   0 runner    (1001) docker     (127)    18227 2024-03-19 14:36:44.000000 ngo-1.0.1/src/ngo/normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4772 2024-03-19 14:36:44.000000 ngo-1.0.1/src/ngo/projection.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 14:36:44.000000 ngo-1.0.1/src/ngo/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    17958 2024-03-19 14:36:44.000000 ngo-1.0.1/src/ngo/sum_aggregates.py
--rw-r--r--   0 runner    (1001) docker     (127)    19870 2024-03-19 14:36:44.000000 ngo-1.0.1/src/ngo/symmetry.py
--rw-r--r--   0 runner    (1001) docker     (127)    11819 2024-03-19 14:36:44.000000 ngo-1.0.1/src/ngo/unused.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:36:48.755271 ngo-1.0.1/src/ngo/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-19 14:36:44.000000 ngo-1.0.1/src/ngo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36434 2024-03-19 14:36:44.000000 ngo-1.0.1/src/ngo/utils/ast.py
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-03-19 14:36:44.000000 ngo-1.0.1/src/ngo/utils/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-03-19 14:36:44.000000 ngo-1.0.1/src/ngo/utils/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:36:48.759271 ngo-1.0.1/src/ngo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-03-19 14:36:48.000000 ngo-1.0.1/src/ngo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-03-19 14:36:48.000000 ngo-1.0.1/src/ngo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 14:36:48.000000 ngo-1.0.1/src/ngo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-19 14:36:48.000000 ngo-1.0.1/src/ngo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-19 14:36:48.000000 ngo-1.0.1/src/ngo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-19 14:36:48.000000 ngo-1.0.1/src/ngo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:36:48.759271 ngo-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 14:36:44.000000 ngo-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 14:36:44.000000 ngo-1.0.1/tests/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-03-19 14:36:44.000000 ngo-1.0.1/tests/test_ast.py
--rw-r--r--   0 runner    (1001) docker     (127)     7693 2024-03-19 14:36:44.000000 ngo-1.0.1/tests/test_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)    16645 2024-03-19 14:36:44.000000 ngo-1.0.1/tests/test_dependency.py
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-03-19 14:36:44.000000 ngo-1.0.1/tests/test_global.py
--rw-r--r--   0 runner    (1001) docker     (127)    16139 2024-03-19 14:36:44.000000 ngo-1.0.1/tests/test_inline.py
--rw-r--r--   0 runner    (1001) docker     (127)    12538 2024-03-19 14:36:44.000000 ngo-1.0.1/tests/test_literal_duplication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-03-19 14:36:44.000000 ngo-1.0.1/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)    21250 2024-03-19 14:36:44.000000 ngo-1.0.1/tests/test_math_simplification.py
--rw-r--r--   0 runner    (1001) docker     (127)    63568 2024-03-19 14:36:44.000000 ngo-1.0.1/tests/test_minmax_aggregates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-03-19 14:36:44.000000 ngo-1.0.1/tests/test_normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-03-19 14:36:44.000000 ngo-1.0.1/tests/test_projection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-03-19 14:36:44.000000 ngo-1.0.1/tests/test_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)    16369 2024-03-19 14:36:44.000000 ngo-1.0.1/tests/test_sum_aggregates.py
--rw-r--r--   0 runner    (1001) docker     (127)     8280 2024-03-19 14:36:44.000000 ngo-1.0.1/tests/test_symmetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     8708 2024-03-19 14:36:44.000000 ngo-1.0.1/tests/test_unused.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:53:42.256006 ngo-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-06-03 12:53:18.000000 ngo-1.0.2/.envrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:53:42.240007 ngo-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:53:42.244006 ngo-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-06-03 12:53:18.000000 ngo-1.0.2/.github/workflows/buildwheel.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-06-03 12:53:18.000000 ngo-1.0.2/.github/workflows/cd-pre.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-06-03 12:53:18.000000 ngo-1.0.2/.github/workflows/cd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-06-03 12:53:18.000000 ngo-1.0.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-06-03 12:53:18.000000 ngo-1.0.2/.github/workflows/publish-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-06-03 12:53:18.000000 ngo-1.0.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-06-03 12:53:18.000000 ngo-1.0.2/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-06-03 12:53:18.000000 ngo-1.0.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-06-03 12:53:18.000000 ngo-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-06-03 12:53:18.000000 ngo-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-06-03 12:53:18.000000 ngo-1.0.2/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-06-03 12:53:18.000000 ngo-1.0.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-06-03 12:53:18.000000 ngo-1.0.2/DEVELOPMENT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-06-03 12:53:18.000000 ngo-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-06-03 12:53:42.256006 ngo-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-06-03 12:53:18.000000 ngo-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-06-03 12:53:18.000000 ngo-1.0.2/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-06-03 12:53:18.000000 ngo-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 12:53:42.256006 ngo-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:53:42.240007 ngo-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:53:42.248006 ngo-1.0.2/src/ngo/
+-rw-r--r--   0 runner    (1001) docker     (127)     7164 2024-06-03 12:53:18.000000 ngo-1.0.2/src/ngo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-06-03 12:53:18.000000 ngo-1.0.2/src/ngo/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-06-03 12:53:18.000000 ngo-1.0.2/src/ngo/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13490 2024-06-03 12:53:18.000000 ngo-1.0.2/src/ngo/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29338 2024-06-03 12:53:18.000000 ngo-1.0.2/src/ngo/dependency.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22383 2024-06-03 12:53:18.000000 ngo-1.0.2/src/ngo/inline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15092 2024-06-03 12:53:18.000000 ngo-1.0.2/src/ngo/literal_duplication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29603 2024-06-03 12:53:18.000000 ngo-1.0.2/src/ngo/math_simplification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30773 2024-06-03 12:53:18.000000 ngo-1.0.2/src/ngo/minmax_aggregates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18060 2024-06-03 12:53:18.000000 ngo-1.0.2/src/ngo/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4772 2024-06-03 12:53:18.000000 ngo-1.0.2/src/ngo/projection.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:53:18.000000 ngo-1.0.2/src/ngo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    18048 2024-06-03 12:53:18.000000 ngo-1.0.2/src/ngo/sum_aggregates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19870 2024-06-03 12:53:18.000000 ngo-1.0.2/src/ngo/symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11764 2024-06-03 12:53:18.000000 ngo-1.0.2/src/ngo/unused.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:53:42.248006 ngo-1.0.2/src/ngo/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-06-03 12:53:18.000000 ngo-1.0.2/src/ngo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36434 2024-06-03 12:53:18.000000 ngo-1.0.2/src/ngo/utils/ast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-06-03 12:53:18.000000 ngo-1.0.2/src/ngo/utils/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-06-03 12:53:18.000000 ngo-1.0.2/src/ngo/utils/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:53:42.252006 ngo-1.0.2/src/ngo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-06-03 12:53:42.000000 ngo-1.0.2/src/ngo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-06-03 12:53:42.000000 ngo-1.0.2/src/ngo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 12:53:42.000000 ngo-1.0.2/src/ngo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-06-03 12:53:42.000000 ngo-1.0.2/src/ngo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-06-03 12:53:42.000000 ngo-1.0.2/src/ngo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-06-03 12:53:42.000000 ngo-1.0.2/src/ngo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:53:42.252006 ngo-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:53:18.000000 ngo-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:53:18.000000 ngo-1.0.2/tests/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-06-03 12:53:18.000000 ngo-1.0.2/tests/test_ast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7693 2024-06-03 12:53:18.000000 ngo-1.0.2/tests/test_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16645 2024-06-03 12:53:18.000000 ngo-1.0.2/tests/test_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-06-03 12:53:18.000000 ngo-1.0.2/tests/test_global.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16139 2024-06-03 12:53:18.000000 ngo-1.0.2/tests/test_inline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12538 2024-06-03 12:53:18.000000 ngo-1.0.2/tests/test_literal_duplication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-06-03 12:53:18.000000 ngo-1.0.2/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21250 2024-06-03 12:53:18.000000 ngo-1.0.2/tests/test_math_simplification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63568 2024-06-03 12:53:18.000000 ngo-1.0.2/tests/test_minmax_aggregates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-06-03 12:53:18.000000 ngo-1.0.2/tests/test_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-06-03 12:53:18.000000 ngo-1.0.2/tests/test_projection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-06-03 12:53:18.000000 ngo-1.0.2/tests/test_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16369 2024-06-03 12:53:18.000000 ngo-1.0.2/tests/test_sum_aggregates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8280 2024-06-03 12:53:18.000000 ngo-1.0.2/tests/test_symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8708 2024-06-03 12:53:18.000000 ngo-1.0.2/tests/test_unused.py
```

### Comparing `ngo-1.0.1/.github/workflows/buildwheel.yml` & `ngo-1.0.2/.github/workflows/buildwheel.yml`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.x"
 
       - name: Install pypa/build
         run: >-
           python3 -m
           pip install
```

### Comparing `ngo-1.0.1/.github/workflows/publish-docs.yml` & `ngo-1.0.2/.github/workflows/publish-docs.yml`

 * *Files 17% similar despite different names*

```diff
@@ -23,26 +23,26 @@
   deploy:
     environment:
       name: github-pages
       url: ${{ steps.deployment.outputs.page_url }}
     runs-on: ubuntu-latest
     steps:
       - name: Checkout
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
       - name: Setup Pages
-        uses: actions/configure-pages@v3
+        uses: actions/configure-pages@v4
       - name: "setup python 3.11"
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: 3.11
       - name: install nox
         run: python -m pip install nox
       - name: create docs
         run: nox -s doc
       - name: Upload artifact
-        uses: actions/upload-pages-artifact@v2
+        uses: actions/upload-pages-artifact@v3
         with:
           # Upload docs folder
           path: 'docs'
       - name: Deploy to GitHub Pages
         id: deployment
-        uses: actions/deploy-pages@v2
+        uses: actions/deploy-pages@v4
```

### Comparing `ngo-1.0.1/.github/workflows/publish-to-pypi.yml` & `ngo-1.0.2/.github/workflows/publish-to-test-pypi.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,27 @@
-name: Publish to Pypi
+name: Publish to TestPypi
 
 on:
   # Creates a reusable workflow
   workflow_call:
   # Allows you to run this workflow manually from the Actions tab
   workflow_dispatch:
 
 jobs:
   build:
     uses: ./.github/workflows/buildwheel.yml
-  pypi-publish:
-    name: Publish to PyPI
+  test-publish:
+    name: Publish to TestPyPI
     needs: [build]
     permissions:
       id-token: write
-    environment:
-      name: release
-      url: https://pypi.org/p/ngo
+    environment: test-release
     runs-on: ubuntu-latest
     steps:
       - uses: actions/download-artifact@v4
         with:
           name: wheel
           path: dist
-      - name: Publish package distributions to PyPI
+      - name: Publish package distributions to TestPyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
-          verbose: true
-          repository-url: https://upload.pypi.org/legacy/
+          repository-url: https://test.pypi.org/legacy/
```

### Comparing `ngo-1.0.1/.github/workflows/test.yml` & `ngo-1.0.2/.github/workflows/test.yml`

 * *Files 17% similar despite different names*

```diff
@@ -16,18 +16,18 @@
     strategy:
       fail-fast: false
       matrix:
         os: ['ubuntu-latest', 'macos-latest', 'windows-latest']
 
     steps:
     - name: "checkout repository"
-      uses: actions/checkout@v3
+      uses: actions/checkout@v4
 
     - name: "setup python 3.11"
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: 3.11
   
     - name: install nox
       run: python -m pip install nox
 
     - name: run tests
```

### Comparing `ngo-1.0.1/CHANGELOG` & `ngo-1.0.2/CHANGELOG`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+1.0.2
+ - removed errornous print statement that gave different versions of the optimized encoding (BUGFIX)
 1.0.1
  - change setup to pyproject.toml only
  - bugfix #inf/#sup calculation as aggregate boundaries
  - bugfix aggregates as disjunctions
  - performance improvements
 1.0.0
  - update to clingo release 5.7.1
```

### Comparing `ngo-1.0.1/CONTRIBUTING.md` & `ngo-1.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ngo-1.0.1/DEVELOPMENT.md` & `ngo-1.0.2/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `ngo-1.0.1/LICENSE` & `ngo-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ngo-1.0.1/PKG-INFO` & `ngo-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngo
-Version: 1.0.1
+Version: 1.0.2
 Summary: Optimizes non ground logic programs.
 Author-email: Max Ostrowski <max.ostrowski@potassco.com>
 License: MIT License
         
         Copyright (c) 2023 Max Ostrowski
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,14 +22,16 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://potassco.org/ngo
+Project-URL: Documentation, https://potassco.org/ngo
+Project-URL: Repository, http://github.com/potassco/ngo
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: clingo<6.0,>=5.7.1
 Requires-Dist: networkx>=3.1
 Requires-Dist: sympy>=1.12
 Provides-Extra: format
```

### Comparing `ngo-1.0.1/noxfile.py` & `ngo-1.0.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `ngo-1.0.1/pyproject.toml` & `ngo-1.0.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -20,14 +20,16 @@
     "clingo>=5.7.1,<6.0",
     "networkx>=3.1",
     "sympy>=1.12",
 ]
 
 [project.urls]
 Homepage = "https://potassco.org/ngo"
+Documentation = "https://potassco.org/ngo"
+Repository = "http://github.com/potassco/ngo"
 
 [project.optional-dependencies]
 format = [ "black", "isort"]
 lint = [ "pylint", "ngo[test]" ]
 typecheck = [ "types-setuptools", "mypy", "networkx-stubs", "ngo[test]" ]
 test = [ "pytest", "coverage" ]
 doc = [ "pdoc" ]
```

### Comparing `ngo-1.0.1/src/ngo/__init__.py` & `ngo-1.0.2/src/ngo/__init__.py`

 * *Files identical despite different names*

### Comparing `ngo-1.0.1/src/ngo/__main__.py` & `ngo-1.0.2/src/ngo/__main__.py`

 * *Files identical despite different names*

### Comparing `ngo-1.0.1/src/ngo/api.py` & `ngo-1.0.2/src/ngo/api.py`

 * *Files identical despite different names*

### Comparing `ngo-1.0.1/src/ngo/cleanup.py` & `ngo-1.0.2/src/ngo/cleanup.py`

 * *Files identical despite different names*

### Comparing `ngo-1.0.1/src/ngo/dependency.py` & `ngo-1.0.2/src/ngo/dependency.py`

 * *Files identical despite different names*

### Comparing `ngo-1.0.1/src/ngo/inline.py` & `ngo-1.0.2/src/ngo/inline.py`

 * *Files identical despite different names*

### Comparing `ngo-1.0.1/src/ngo/literal_duplication.py` & `ngo-1.0.2/src/ngo/literal_duplication.py`

 * *Files identical despite different names*

### Comparing `ngo-1.0.1/src/ngo/math_simplification.py` & `ngo-1.0.2/src/ngo/math_simplification.py`

 * *Files identical despite different names*

### Comparing `ngo-1.0.1/src/ngo/minmax_aggregates.py` & `ngo-1.0.2/src/ngo/minmax_aggregates.py`

 * *Files identical despite different names*

### Comparing `ngo-1.0.1/src/ngo/normalize.py` & `ngo-1.0.2/src/ngo/normalize.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,16 +163,16 @@
 
     newprg: list[AST] = []
 
     def replace(bodyagg: AST) -> AST:
         """remove all #inf <= agg and agg =< #sup"""
         if bodyagg.left_guard and bodyagg.left_guard.term.ast_type == ASTType.SymbolicTerm:
             if (
-            bodyagg.left_guard.comparison == ComparisonOperator.LessEqual
-            and bodyagg.left_guard.term.symbol == Infimum
+                bodyagg.left_guard.comparison == ComparisonOperator.LessEqual
+                and bodyagg.left_guard.term.symbol == Infimum
             ) or (
                 bodyagg.left_guard.comparison == ComparisonOperator.GreaterEqual
                 and bodyagg.left_guard.term.symbol == Supremum
             ):
                 bodyagg = bodyagg.update(left_guard=None)
         if bodyagg.right_guard and bodyagg.right_guard.term.ast_type == ASTType.SymbolicTerm:
             if (
@@ -186,17 +186,14 @@
 
         if bodyagg.right_guard and bodyagg.left_guard is None:
             bodyagg = bodyagg.update(
                 left_guard=Guard(rhs2lhs_comparison(bodyagg.right_guard.comparison), bodyagg.right_guard.term),
                 right_guard=None,
             )
 
-        #if bodyagg.left_guard is None and bodyagg.right_guard is None:
-        #    return Literal(LOC, Sign.NoSign, BooleanConstant(True)) # cant replace atom with literal
-
         return bodyagg
 
     for stm in prg:
         newprg.append(transform_ast(stm, "BodyAggregate", replace))
     return newprg
```

### Comparing `ngo-1.0.1/src/ngo/projection.py` & `ngo-1.0.2/src/ngo/projection.py`

 * *Files identical despite different names*

### Comparing `ngo-1.0.1/src/ngo/sum_aggregates.py` & `ngo-1.0.2/src/ngo/sum_aggregates.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,25 +164,27 @@
     def _get_trigger(self, minimize_var: AST, body: list[AST]) -> Optional[tuple[AST, int, AnnotatedPredicate]]:
         for lit in body:
             if is_conditional(lit):  # currently not supported, happens in soft constraints
                 return None
             if not is_predicate(lit):
                 continue
             symbol = lit.atom.symbol
+            trigger_index = None
             for next_anon_pred in self._atmost_preds:
                 if next_anon_pred.pred == Predicate(symbol.name, len(symbol.arguments)):
                     anon_are_anonymous = True
                     for i in next_anon_pred.annotated_positions:
                         if symbol.arguments[i] == Variable(LOC, "_"):
                             continue
                         if symbol.arguments[i] == minimize_var:
                             trigger_index = i
                             continue
                         anon_are_anonymous = False
                     if anon_are_anonymous:
+                        assert trigger_index is not None
                         return (lit, trigger_index, next_anon_pred)
         return None
 
     @staticmethod
     def _element_passes(elem: AST, elements: list[AST]) -> bool:
         """True if element in sum aggregate is simple enough to be replaced inside chaining"""
         if elem.terms[0].ast_type != ASTType.Variable:  # only this variable as weight is allowed
```

### Comparing `ngo-1.0.1/src/ngo/symmetry.py` & `ngo-1.0.2/src/ngo/symmetry.py`

 * *Files identical despite different names*

### Comparing `ngo-1.0.1/src/ngo/unused.py` & `ngo-1.0.2/src/ngo/unused.py`

 * *Files 0% similar despite different names*

```diff
@@ -271,10 +271,8 @@
             self.analyze_usage(prg)
             prg = self.project_unused(prg)
             prg = self.remove_unused(prg)
             prg = self.remove_single_copies(prg)
             if prg == new_prg:
                 break
             new_prg = prg
-            for stm in prg:
-                print(stm)
         return prg
```

### Comparing `ngo-1.0.1/src/ngo/utils/ast.py` & `ngo-1.0.2/src/ngo/utils/ast.py`

 * *Files identical despite different names*

### Comparing `ngo-1.0.1/src/ngo/utils/globals.py` & `ngo-1.0.2/src/ngo/utils/globals.py`

 * *Files identical despite different names*

### Comparing `ngo-1.0.1/src/ngo/utils/parser.py` & `ngo-1.0.2/src/ngo/utils/parser.py`

 * *Files identical despite different names*

### Comparing `ngo-1.0.1/src/ngo.egg-info/PKG-INFO` & `ngo-1.0.2/src/ngo.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngo
-Version: 1.0.1
+Version: 1.0.2
 Summary: Optimizes non ground logic programs.
 Author-email: Max Ostrowski <max.ostrowski@potassco.com>
 License: MIT License
         
         Copyright (c) 2023 Max Ostrowski
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,14 +22,16 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://potassco.org/ngo
+Project-URL: Documentation, https://potassco.org/ngo
+Project-URL: Repository, http://github.com/potassco/ngo
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: clingo<6.0,>=5.7.1
 Requires-Dist: networkx>=3.1
 Requires-Dist: sympy>=1.12
 Provides-Extra: format
```

### Comparing `ngo-1.0.1/src/ngo.egg-info/SOURCES.txt` & `ngo-1.0.2/src/ngo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ngo-1.0.1/tests/test_ast.py` & `ngo-1.0.2/tests/test_ast.py`

 * *Files identical despite different names*

### Comparing `ngo-1.0.1/tests/test_cleanup.py` & `ngo-1.0.2/tests/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `ngo-1.0.1/tests/test_dependency.py` & `ngo-1.0.2/tests/test_dependency.py`

 * *Files identical despite different names*

### Comparing `ngo-1.0.1/tests/test_global.py` & `ngo-1.0.2/tests/test_global.py`

 * *Files identical despite different names*

### Comparing `ngo-1.0.1/tests/test_inline.py` & `ngo-1.0.2/tests/test_inline.py`

 * *Files identical despite different names*

### Comparing `ngo-1.0.1/tests/test_literal_duplication.py` & `ngo-1.0.2/tests/test_literal_duplication.py`

 * *Files identical despite different names*

### Comparing `ngo-1.0.1/tests/test_main.py` & `ngo-1.0.2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `ngo-1.0.1/tests/test_math_simplification.py` & `ngo-1.0.2/tests/test_math_simplification.py`

 * *Files identical despite different names*

### Comparing `ngo-1.0.1/tests/test_minmax_aggregates.py` & `ngo-1.0.2/tests/test_minmax_aggregates.py`

 * *Files identical despite different names*

### Comparing `ngo-1.0.1/tests/test_normalize.py` & `ngo-1.0.2/tests/test_normalize.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 #false :- N != #sum { 1,0,bend(AUX): bend(AUX), AUX = ((T+1)..(T1-1)) }; bends(T,T1,N).""",
         ),
         (
             """
 #false :- #inf <= { bend(((T+1)..(T1-1))) } <= #sup; a.
 """,
             """#program base.
-#false :- #sum { 1,0,bend(AUX): bend(AUX), AUX = ((T+1)..(T1-1)) }; a.""", # weird corner case, wait for preprocessor
+#false :- #sum { 1,0,bend(AUX): bend(AUX), AUX = ((T+1)..(T1-1)) }; a.""",  # weird corner case, wait for preprocessor
         ),
     ],
 )
 def test_preprocess(input_: str, output: str) -> None:
     """test preprocessing"""
     ast: list[AST] = []
     parse_string(input_, ast.append)
```

### Comparing `ngo-1.0.1/tests/test_projection.py` & `ngo-1.0.2/tests/test_projection.py`

 * *Files identical despite different names*

### Comparing `ngo-1.0.1/tests/test_regression.py` & `ngo-1.0.2/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `ngo-1.0.1/tests/test_sum_aggregates.py` & `ngo-1.0.2/tests/test_sum_aggregates.py`

 * *Files identical despite different names*

### Comparing `ngo-1.0.1/tests/test_symmetry.py` & `ngo-1.0.2/tests/test_symmetry.py`

 * *Files identical despite different names*

### Comparing `ngo-1.0.1/tests/test_unused.py` & `ngo-1.0.2/tests/test_unused.py`

 * *Files identical despite different names*

