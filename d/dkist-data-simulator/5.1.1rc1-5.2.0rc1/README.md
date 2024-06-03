# Comparing `tmp/dkist_data_simulator-5.1.1rc1.tar.gz` & `tmp/dkist_data_simulator-5.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist_data_simulator-5.1.1rc1.tar", last modified: Mon Feb 26 11:15:13 2024, max compression
+gzip compressed data, was "dkist_data_simulator-5.2.0rc1.tar", last modified: Mon Jun  3 15:30:34 2024, max compression
```

## Comparing `dkist_data_simulator-5.1.1rc1.tar` & `dkist_data_simulator-5.2.0rc1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-26 11:15:13.992626 dkist_data_simulator-5.1.1rc1/
--rw-rw-rw-   0 root         (0) root         (0)     3308 2024-02-26 11:14:49.000000 dkist_data_simulator-5.1.1rc1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      825 2024-02-26 11:14:49.000000 dkist_data_simulator-5.1.1rc1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      338 2024-02-26 11:14:49.000000 dkist_data_simulator-5.1.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5507 2024-02-26 11:15:13.992626 dkist_data_simulator-5.1.1rc1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4650 2024-02-26 11:14:49.000000 dkist_data_simulator-5.1.1rc1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1461 2024-02-26 11:14:49.000000 dkist_data_simulator-5.1.1rc1/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-26 11:15:13.984626 dkist_data_simulator-5.1.1rc1/dkist_data_simulator/
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-02-26 11:14:49.000000 dkist_data_simulator-5.1.1rc1/dkist_data_simulator/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-26 11:15:13.984626 dkist_data_simulator-5.1.1rc1/dkist_data_simulator/data/
--rw-rw-rw-   0 root         (0) root         (0)      245 2024-02-26 11:14:49.000000 dkist_data_simulator-5.1.1rc1/dkist_data_simulator/data/README.rst
--rw-rw-rw-   0 root         (0) root         (0)    16872 2024-02-26 11:14:49.000000 dkist_data_simulator-5.1.1rc1/dkist_data_simulator/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)      907 2024-02-26 11:14:49.000000 dkist_data_simulator-5.1.1rc1/dkist_data_simulator/expansions.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-26 11:14:49.000000 dkist_data_simulator-5.1.1rc1/dkist_data_simulator/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    11013 2024-02-26 11:14:49.000000 dkist_data_simulator-5.1.1rc1/dkist_data_simulator/schemas.py
--rw-rw-rw-   0 root         (0) root         (0)     8118 2024-02-26 11:14:49.000000 dkist_data_simulator-5.1.1rc1/dkist_data_simulator/spec122.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-26 11:15:13.988626 dkist_data_simulator-5.1.1rc1/dkist_data_simulator/spec214/
--rw-rw-rw-   0 root         (0) root         (0)       20 2024-02-26 11:14:49.000000 dkist_data_simulator-5.1.1rc1/dkist_data_simulator/spec214/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    27769 2024-02-26 11:14:49.000000 dkist_data_simulator-5.1.1rc1/dkist_data_simulator/spec214/core.py
--rw-rw-rw-   0 root         (0) root         (0)    18798 2024-02-26 11:14:49.000000 dkist_data_simulator-5.1.1rc1/dkist_data_simulator/spec214/cryo.py
--rw-rw-rw-   0 root         (0) root         (0)     4989 2024-02-26 11:14:49.000000 dkist_data_simulator-5.1.1rc1/dkist_data_simulator/spec214/dlnirsp.py
--rw-rw-rw-   0 root         (0) root         (0)     7981 2024-02-26 11:14:49.000000 dkist_data_simulator-5.1.1rc1/dkist_data_simulator/spec214/vbi.py
--rw-rw-rw-   0 root         (0) root         (0)     8152 2024-02-26 11:14:49.000000 dkist_data_simulator-5.1.1rc1/dkist_data_simulator/spec214/visp.py
--rw-rw-rw-   0 root         (0) root         (0)     3584 2024-02-26 11:14:49.000000 dkist_data_simulator-5.1.1rc1/dkist_data_simulator/spec214/vtf.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-26 11:15:13.988626 dkist_data_simulator-5.1.1rc1/dkist_data_simulator/tests/
--rw-rw-rw-   0 root         (0) root         (0)       44 2024-02-26 11:14:49.000000 dkist_data_simulator-5.1.1rc1/dkist_data_simulator/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1012 2024-02-26 11:14:49.000000 dkist_data_simulator-5.1.1rc1/dkist_data_simulator/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     1808 2024-02-26 11:14:49.000000 dkist_data_simulator-5.1.1rc1/dkist_data_simulator/tests/test_122.py
--rw-rw-rw-   0 root         (0) root         (0)    15556 2024-02-26 11:14:49.000000 dkist_data_simulator-5.1.1rc1/dkist_data_simulator/tests/test_214.py
--rw-rw-rw-   0 root         (0) root         (0)     8128 2024-02-26 11:14:49.000000 dkist_data_simulator-5.1.1rc1/dkist_data_simulator/tests/test_214_inventory.py
--rw-rw-rw-   0 root         (0) root         (0)     5458 2024-02-26 11:14:49.000000 dkist_data_simulator-5.1.1rc1/dkist_data_simulator/tests/test_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     2689 2024-02-26 11:14:49.000000 dkist_data_simulator-5.1.1rc1/dkist_data_simulator/util.py
--rw-rw-rw-   0 root         (0) root         (0)      348 2024-02-26 11:15:13.000000 dkist_data_simulator-5.1.1rc1/dkist_data_simulator/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-26 11:15:13.988626 dkist_data_simulator-5.1.1rc1/dkist_data_simulator.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5507 2024-02-26 11:15:13.000000 dkist_data_simulator-5.1.1rc1/dkist_data_simulator.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1341 2024-02-26 11:15:13.000000 dkist_data_simulator-5.1.1rc1/dkist_data_simulator.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-02-26 11:15:13.000000 dkist_data_simulator-5.1.1rc1/dkist_data_simulator.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-02-26 11:15:13.000000 dkist_data_simulator-5.1.1rc1/dkist_data_simulator.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      218 2024-02-26 11:15:13.000000 dkist_data_simulator-5.1.1rc1/dkist_data_simulator.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       21 2024-02-26 11:15:13.000000 dkist_data_simulator-5.1.1rc1/dkist_data_simulator.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-26 11:15:13.988626 dkist_data_simulator-5.1.1rc1/docs/
--rw-rw-rw-   0 root         (0) root         (0)      634 2024-02-26 11:14:49.000000 dkist_data_simulator-5.1.1rc1/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     2629 2024-02-26 11:14:49.000000 dkist_data_simulator-5.1.1rc1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      307 2024-02-26 11:14:49.000000 dkist_data_simulator-5.1.1rc1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      760 2024-02-26 11:14:49.000000 dkist_data_simulator-5.1.1rc1/docs/make.bat
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-26 11:15:13.988626 dkist_data_simulator-5.1.1rc1/examples/
--rwxrwxrwx   0 root         (0) root         (0)     4098 2024-02-26 11:14:49.000000 dkist_data_simulator-5.1.1rc1/examples/vtf_crisp_5d.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-26 11:15:13.988626 dkist_data_simulator-5.1.1rc1/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1482 2024-02-26 11:14:49.000000 dkist_data_simulator-5.1.1rc1/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      372 2024-02-26 11:14:49.000000 dkist_data_simulator-5.1.1rc1/licenses/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1659 2024-02-26 11:14:49.000000 dkist_data_simulator-5.1.1rc1/licenses/TEMPLATE_LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      326 2024-02-26 11:14:49.000000 dkist_data_simulator-5.1.1rc1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     2744 2024-02-26 11:15:13.992626 dkist_data_simulator-5.1.1rc1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      607 2024-02-26 11:14:49.000000 dkist_data_simulator-5.1.1rc1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1556 2024-02-26 11:14:49.000000 dkist_data_simulator-5.1.1rc1/tox.ini
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-03 15:30:34.687080 dkist_data_simulator-5.2.0rc1/
+-rw-rw-rw-   0 root         (0) root         (0)     3308 2024-06-03 15:30:19.000000 dkist_data_simulator-5.2.0rc1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      825 2024-06-03 15:30:19.000000 dkist_data_simulator-5.2.0rc1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      338 2024-06-03 15:30:19.000000 dkist_data_simulator-5.2.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5501 2024-06-03 15:30:34.687080 dkist_data_simulator-5.2.0rc1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4647 2024-06-03 15:30:19.000000 dkist_data_simulator-5.2.0rc1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2024-06-03 15:30:19.000000 dkist_data_simulator-5.2.0rc1/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-03 15:30:34.679080 dkist_data_simulator-5.2.0rc1/dkist_data_simulator/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-06-03 15:30:19.000000 dkist_data_simulator-5.2.0rc1/dkist_data_simulator/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-03 15:30:34.683080 dkist_data_simulator-5.2.0rc1/dkist_data_simulator/data/
+-rw-rw-rw-   0 root         (0) root         (0)      245 2024-06-03 15:30:19.000000 dkist_data_simulator-5.2.0rc1/dkist_data_simulator/data/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)    16872 2024-06-03 15:30:19.000000 dkist_data_simulator-5.2.0rc1/dkist_data_simulator/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)      907 2024-06-03 15:30:19.000000 dkist_data_simulator-5.2.0rc1/dkist_data_simulator/expansions.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-03 15:30:19.000000 dkist_data_simulator-5.2.0rc1/dkist_data_simulator/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    11013 2024-06-03 15:30:19.000000 dkist_data_simulator-5.2.0rc1/dkist_data_simulator/schemas.py
+-rw-rw-rw-   0 root         (0) root         (0)     8118 2024-06-03 15:30:19.000000 dkist_data_simulator-5.2.0rc1/dkist_data_simulator/spec122.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-03 15:30:34.683080 dkist_data_simulator-5.2.0rc1/dkist_data_simulator/spec214/
+-rw-rw-rw-   0 root         (0) root         (0)       20 2024-06-03 15:30:19.000000 dkist_data_simulator-5.2.0rc1/dkist_data_simulator/spec214/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    27769 2024-06-03 15:30:19.000000 dkist_data_simulator-5.2.0rc1/dkist_data_simulator/spec214/core.py
+-rw-rw-rw-   0 root         (0) root         (0)    18798 2024-06-03 15:30:19.000000 dkist_data_simulator-5.2.0rc1/dkist_data_simulator/spec214/cryo.py
+-rw-rw-rw-   0 root         (0) root         (0)     8982 2024-06-03 15:30:19.000000 dkist_data_simulator-5.2.0rc1/dkist_data_simulator/spec214/dlnirsp.py
+-rw-rw-rw-   0 root         (0) root         (0)     8034 2024-06-03 15:30:19.000000 dkist_data_simulator-5.2.0rc1/dkist_data_simulator/spec214/vbi.py
+-rw-rw-rw-   0 root         (0) root         (0)     8152 2024-06-03 15:30:20.000000 dkist_data_simulator-5.2.0rc1/dkist_data_simulator/spec214/visp.py
+-rw-rw-rw-   0 root         (0) root         (0)     3584 2024-06-03 15:30:20.000000 dkist_data_simulator-5.2.0rc1/dkist_data_simulator/spec214/vtf.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-03 15:30:34.683080 dkist_data_simulator-5.2.0rc1/dkist_data_simulator/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2024-06-03 15:30:20.000000 dkist_data_simulator-5.2.0rc1/dkist_data_simulator/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1012 2024-06-03 15:30:20.000000 dkist_data_simulator-5.2.0rc1/dkist_data_simulator/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1808 2024-06-03 15:30:20.000000 dkist_data_simulator-5.2.0rc1/dkist_data_simulator/tests/test_122.py
+-rw-rw-rw-   0 root         (0) root         (0)    17112 2024-06-03 15:30:20.000000 dkist_data_simulator-5.2.0rc1/dkist_data_simulator/tests/test_214.py
+-rw-rw-rw-   0 root         (0) root         (0)     8234 2024-06-03 15:30:20.000000 dkist_data_simulator-5.2.0rc1/dkist_data_simulator/tests/test_214_inventory.py
+-rw-rw-rw-   0 root         (0) root         (0)     5458 2024-06-03 15:30:20.000000 dkist_data_simulator-5.2.0rc1/dkist_data_simulator/tests/test_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     2689 2024-06-03 15:30:20.000000 dkist_data_simulator-5.2.0rc1/dkist_data_simulator/util.py
+-rw-rw-rw-   0 root         (0) root         (0)      348 2024-06-03 15:30:34.000000 dkist_data_simulator-5.2.0rc1/dkist_data_simulator/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-03 15:30:34.687080 dkist_data_simulator-5.2.0rc1/dkist_data_simulator.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5501 2024-06-03 15:30:34.000000 dkist_data_simulator-5.2.0rc1/dkist_data_simulator.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2024-06-03 15:30:34.000000 dkist_data_simulator-5.2.0rc1/dkist_data_simulator.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-06-03 15:30:34.000000 dkist_data_simulator-5.2.0rc1/dkist_data_simulator.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-06-03 15:30:34.000000 dkist_data_simulator-5.2.0rc1/dkist_data_simulator.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      215 2024-06-03 15:30:34.000000 dkist_data_simulator-5.2.0rc1/dkist_data_simulator.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       21 2024-06-03 15:30:34.000000 dkist_data_simulator-5.2.0rc1/dkist_data_simulator.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-03 15:30:34.683080 dkist_data_simulator-5.2.0rc1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      634 2024-06-03 15:30:20.000000 dkist_data_simulator-5.2.0rc1/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     2629 2024-06-03 15:30:20.000000 dkist_data_simulator-5.2.0rc1/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      307 2024-06-03 15:30:20.000000 dkist_data_simulator-5.2.0rc1/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      760 2024-06-03 15:30:20.000000 dkist_data_simulator-5.2.0rc1/docs/make.bat
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-03 15:30:34.683080 dkist_data_simulator-5.2.0rc1/examples/
+-rwxrwxrwx   0 root         (0) root         (0)     4098 2024-06-03 15:30:20.000000 dkist_data_simulator-5.2.0rc1/examples/vtf_crisp_5d.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-03 15:30:34.683080 dkist_data_simulator-5.2.0rc1/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2024-06-03 15:30:20.000000 dkist_data_simulator-5.2.0rc1/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      372 2024-06-03 15:30:20.000000 dkist_data_simulator-5.2.0rc1/licenses/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1659 2024-06-03 15:30:20.000000 dkist_data_simulator-5.2.0rc1/licenses/TEMPLATE_LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      326 2024-06-03 15:30:20.000000 dkist_data_simulator-5.2.0rc1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     2741 2024-06-03 15:30:34.687080 dkist_data_simulator-5.2.0rc1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      607 2024-06-03 15:30:20.000000 dkist_data_simulator-5.2.0rc1/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1556 2024-06-03 15:30:20.000000 dkist_data_simulator-5.2.0rc1/tox.ini
```

### Comparing `dkist_data_simulator-5.1.1rc1/.gitignore` & `dkist_data_simulator-5.2.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-5.1.1rc1/.pre-commit-config.yaml` & `dkist_data_simulator-5.2.0rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-5.1.1rc1/PKG-INFO` & `dkist_data_simulator-5.2.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: dkist_data_simulator
-Version: 5.1.1rc1
+Version: 5.2.0rc1
 Summary: A header generator and FITS file creator for DKIST data.
 Home-page: 
 Author: AURA / NSO
 Author-email: stuart@cadair.com
 License: BSD 3-Clause
 License-File: licenses/LICENSE.rst
-Requires-Dist: dkist-fits-specifications>=4.1.1rc1
+Requires-Dist: dkist-fits-specifications>=4.1.1
 Requires-Dist: hashids
 Requires-Dist: tqdm
 Requires-Dist: sunpy
 Requires-Dist: astropy
 Requires-Dist: scipy
 Provides-Extra: all
 Provides-Extra: test
@@ -33,15 +33,15 @@
 
 Using
 -----
 
 Generating Pesudo Random Data
 #############################
 
-The simplest way to generate data is to to use the `dkist_data_simulator.spec122.Spec122Dataset` or `dkist_data_simulator.spec214.Spec214Dataset` classes.
+The simplest way to generate data is to use the `dkist_data_simulator.spec122.Spec122Dataset` or `dkist_data_simulator.spec214.Spec214Dataset` classes.
 
 To generate a header::
 
   >>> from dkist_data_simulator.spec122 import Spec122Dataset
   >>> ds = Spec122Dataset(dataset_shape=(1, 512, 512), array_shape=(1, 512, 512), time_delta=10)
   >>> ds.header()
```

### Comparing `dkist_data_simulator-5.1.1rc1/README.rst` & `dkist_data_simulator-5.2.0rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 Using
 -----
 
 Generating Pesudo Random Data
 #############################
 
-The simplest way to generate data is to to use the `dkist_data_simulator.spec122.Spec122Dataset` or `dkist_data_simulator.spec214.Spec214Dataset` classes.
+The simplest way to generate data is to use the `dkist_data_simulator.spec122.Spec122Dataset` or `dkist_data_simulator.spec214.Spec214Dataset` classes.
 
 To generate a header::
 
   >>> from dkist_data_simulator.spec122 import Spec122Dataset
   >>> ds = Spec122Dataset(dataset_shape=(1, 512, 512), array_shape=(1, 512, 512), time_delta=10)
   >>> ds.header()
```

### Comparing `dkist_data_simulator-5.1.1rc1/bitbucket-pipelines.yml` & `dkist_data_simulator-5.2.0rc1/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-5.1.1rc1/dkist_data_simulator/dataset.py` & `dkist_data_simulator-5.2.0rc1/dkist_data_simulator/dataset.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-5.1.1rc1/dkist_data_simulator/expansions.py` & `dkist_data_simulator-5.2.0rc1/dkist_data_simulator/expansions.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-5.1.1rc1/dkist_data_simulator/schemas.py` & `dkist_data_simulator-5.2.0rc1/dkist_data_simulator/schemas.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-5.1.1rc1/dkist_data_simulator/spec122.py` & `dkist_data_simulator-5.2.0rc1/dkist_data_simulator/spec122.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-5.1.1rc1/dkist_data_simulator/spec214/core.py` & `dkist_data_simulator-5.2.0rc1/dkist_data_simulator/spec214/core.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-5.1.1rc1/dkist_data_simulator/spec214/cryo.py` & `dkist_data_simulator-5.2.0rc1/dkist_data_simulator/spec214/cryo.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-5.1.1rc1/dkist_data_simulator/spec214/dlnirsp.py` & `dkist_data_simulator-5.2.0rc1/dkist_data_simulator/spec214/vtf.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,154 +1,114 @@
-from random import choice
-from typing import Any
-
 import astropy.units as u
 import numpy as np
 from astropy.wcs import WCS
-from dkist_fits_specifications.utils.spec_processors.polarimetric_requiredness import (
-    POLARIMETRIC_HEADER_REQUIREMENTS,
-)
 
-from .core import Spec214Dataset, Spec214Schema
+from dkist_data_simulator.dataset import key_function
+from dkist_data_simulator.spec214.core import Spec214Dataset
 
 
-class BaseDLNIRSPDataset(Spec214Dataset):
+class BaseVTFDataset(Spec214Dataset):
     """
-    A base class for DL-NIRSP datasets.
+    A base class for VTF datasets.
     """
 
     def __init__(
         self,
-        n_exposures,
+        n_wave,
+        n_repeats,
         n_stokes,
         time_delta,
         *,
         linewave,
-        array_shape=(100, 100, 100)
+        detector_shape=(4096, 4096)
     ):
-        if not n_exposures:
+        if not n_wave or not n_repeats:
             raise NotImplementedError(
-                "Support for less than 4D DLNIRSP datasets is not implemented."
+                "Support for less than 4D VTF datasets is not implemented."
             )
 
-        array_shape = list(array_shape)
+        array_shape = list(detector_shape)
 
-        dataset_shape_rev = list(array_shape) + [n_exposures]
+        dataset_shape_rev = list(detector_shape) + [n_wave, n_repeats]
         if n_stokes > 1:
             dataset_shape_rev += [n_stokes]
 
-        # These keys need to be passed to super().__init__ so the file schema is updated with the correct
-        # polarimetric requiredness
-        polarimetric_keys = self.get_polarimetric_keys(n_stokes)
-
         super().__init__(
             dataset_shape_rev[::-1],
             array_shape,
             time_delta=time_delta,
-            instrument="dlnirsp",
-            **polarimetric_keys
+            instrument="vtf",
         )
 
         self.add_constant_key("DTYPE1", "SPATIAL")
         self.add_constant_key("DPNAME1", "spatial x")
         self.add_constant_key("DWNAME1", "helioprojective longitude")
         self.add_constant_key("DUNIT1", "arcsec")
 
         self.add_constant_key("DTYPE2", "SPATIAL")
         self.add_constant_key("DPNAME2", "spatial y")
         self.add_constant_key("DWNAME2", "helioprojective latitude")
         self.add_constant_key("DUNIT2", "arcsec")
 
         self.add_constant_key("DTYPE3", "SPECTRAL")
-        self.add_constant_key("DPNAME3", "wavelength")
+        self.add_constant_key("DPNAME3", "scan position")
         self.add_constant_key("DWNAME3", "wavelength")
         self.add_constant_key("DUNIT3", "nm")
 
         self.add_constant_key("DTYPE4", "TEMPORAL")
-        self.add_constant_key("DPNAME4", "exposure number")
+        self.add_constant_key("DPNAME4", "scan repeat number")
         self.add_constant_key("DWNAME4", "time")
         self.add_constant_key("DUNIT4", "s")
 
         if n_stokes > 1:
             self.add_constant_key("DTYPE5", "STOKES")
             self.add_constant_key("DPNAME5", "stokes")
             self.add_constant_key("DWNAME5", "stokes")
             self.add_constant_key("DUNIT5", "")
             self.stokes_file_axis = 0
 
+        self.linewave = linewave
         self.add_constant_key("LINEWAV", linewave.to_value(u.nm))
 
-        for key, value in polarimetric_keys.items():
-            self.add_constant_key(key, value)
-
-        # TODO: What is this value??
-        self.plate_scale = (
-            10 * u.arcsec / u.pix,
-            10 * u.arcsec / u.pix,
-            1 * u.nm / u.pix,
-        )
+        # TODO: Check this value is right
+        self.plate_scale = 0.012 * u.arcsec / u.pix
         self.n_stokes = n_stokes
 
-    def get_polarimetric_keys(self, n_stokes) -> dict[str, Any]:
+    @key_function("FRAMEWAV")
+    def framewav(self, key: str):
         """
-        Given the number of stokes parameters, update the header to correspond to polarimetric or non-polarimetric data.
+        Add a random framewav around the line centre
         """
-        # Just a dummy schema so we can generate values.
-        file_schema = Spec214Schema(
-            instrument="dlnirsp", naxis=3, dnaxis=4, deaxes=2, daaxes=2, nspeclns=1
-        )
-        polarimetric_keys = dict()
-        for key, polarimetric_choices in POLARIMETRIC_HEADER_REQUIREMENTS[
-            "dl-nirsp"
-        ].items():
-            if n_stokes > 1:
-                value = choice(polarimetric_choices)
-
-            else:
-                key_schema = file_schema[key]
-                value = key_schema.generate_value()
-                while value in polarimetric_choices:
-                    # Keep trying until we get something non-polarimetric
-                    value = key_schema.generate_value()
-
-            polarimetric_keys[key] = value
-
-        return polarimetric_keys
-
-
-class SimpleDLNIRSPDataset(BaseDLNIRSPDataset):
-    """
-    A simple five dimensional DLNIRSP dataset with a HPC grid aligned to the pixel axes.
-    """
-
-    name = "dlnirsp-simple"
+        return self.linewave.to_value(u.nm) - (np.random.random() - 0.5) * 10
 
     @property
     def non_temporal_file_axes(self):
         if self.n_stokes > 1:
             # This is the index in file shape so third file dimension
             return (0,)
         return super().non_temporal_file_axes
 
+
+class SimpleVTFDataset(BaseVTFDataset):
+    """
+    A simple five dimensional VTF dataset with a HPC grid aligned to the pixel axes.
+    """
+
+    name = "vtf-simple"
+
     @property
     def data(self):
         return np.random.random(self.array_shape)
 
     @property
     def fits_wcs(self):
-        if self.array_ndim != 3:
-            raise ValueError(
-                "DLNIRSP dataset generator expects a three dimensional FITS WCS."
-            )
+        if self.array_ndim != 2:
+            raise ValueError("VTF dataset generator expects two dimensional FITS WCS.")
 
         w = WCS(naxis=self.array_ndim)
-        w.wcs.crpix = (
-            self.array_shape[2] / 2,
-            self.array_shape[1] / 2,
-            self.array_shape[0] / 2,
-        )
-        w.wcs.crval = 0, 0, 0
-        w.wcs.cdelt = [self.plate_scale[i].value for i in range(self.array_ndim)]
-        w.wcs.cunit = "arcsec", "arcsec", "nm"
-        w.wcs.ctype = "HPLN-TAN", "HPLT-TAN", "AWAV"
+        w.wcs.crpix = self.array_shape[1] / 2, self.array_shape[0] / 2
+        w.wcs.crval = 0, 0
+        w.wcs.cdelt = [self.plate_scale.to_value(u.arcsec / u.pix) for i in range(2)]
+        w.wcs.cunit = "arcsec", "arcsec"
+        w.wcs.ctype = "HPLN-TAN", "HPLT-TAN"
         w.wcs.pc = np.identity(self.array_ndim)
         return w
```

### Comparing `dkist_data_simulator-5.1.1rc1/dkist_data_simulator/spec214/vbi.py` & `dkist_data_simulator-5.2.0rc1/dkist_data_simulator/spec214/vbi.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,14 +196,15 @@
         "MINDEX2",
         "VBISTP",
     )
     def moasic_keys(self, key: str):
         axis_length = 3
         if key == "VBISTP":
             return int(self.current_camera_pos)
+        # TODO: These should be referencing VBISTPAT
         if key == "MINDEX1":
             return int((self.current_camera_pos - 1) % axis_length + 1)
         if key == "MINDEX2":
             return int((self.current_camera_pos - 1) // axis_length + 1)
 
         constant_keys = {
             "MAXIS": 2,
```

### Comparing `dkist_data_simulator-5.1.1rc1/dkist_data_simulator/spec214/visp.py` & `dkist_data_simulator-5.2.0rc1/dkist_data_simulator/spec214/visp.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-5.1.1rc1/dkist_data_simulator/tests/conftest.py` & `dkist_data_simulator-5.2.0rc1/dkist_data_simulator/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-5.1.1rc1/dkist_data_simulator/tests/test_122.py` & `dkist_data_simulator-5.2.0rc1/dkist_data_simulator/tests/test_122.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-5.1.1rc1/dkist_data_simulator/tests/test_214.py` & `dkist_data_simulator-5.2.0rc1/dkist_data_simulator/tests/test_214.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,18 @@
 
 from dkist_data_simulator.spec214.cryo import (
     SimpleCryonirspCIDataset,
     SimpleCryonirspSPDataset,
     TimeDependentCryonirspCIDataset,
     TimeDependentCryonirspSPDataset,
 )
-from dkist_data_simulator.spec214.dlnirsp import SimpleDLNIRSPDataset
+from dkist_data_simulator.spec214.dlnirsp import (
+    MosaicedDLNIRSPDataset,
+    SimpleDLNIRSPDataset,
+)
 from dkist_data_simulator.spec214.vbi import (
     MosaicedVBIBlueDataset,
     SimpleVBIDataset,
     TimeDependentVBIDataset,
 )
 from dkist_data_simulator.spec214.visp import (
     SimpleVISPDataset,
@@ -314,14 +317,57 @@
     # but we have to compensate for the fact that in FITS convention 1 is the
     # "midpoint" of this range
     start = n_raster / 2 + 1
     end = -1 * (n_raster / 2 - 1)
     assert np.allclose(h_table["CRPIX3"], np.arange(start, end, -1))
 
 
+def test_dlnirsp_mosaic():
+    n_X_tiles = 2
+    n_Y_tiles = 3
+    ds = MosaicedDLNIRSPDataset(
+        n_mosaic_repeats=3,
+        n_X_tiles=n_X_tiles,
+        n_Y_tiles=n_Y_tiles,
+        n_stokes=4,
+        time_delta=10,
+        linewave=400 * u.nm,
+        array_shape=(10, 10, 10),
+    )
+    headers = ds.generate_headers()
+    h_table = Table(headers)
+
+    n_pos = n_X_tiles * n_Y_tiles
+
+    # Assert that between index 1 and 2 we have 9 unique positions
+    tile_grouped = h_table.group_by(("MINDEX1", "MINDEX2"))
+    assert len(tile_grouped.groups) == n_pos
+
+    for tile in tile_grouped.groups:
+        assert not (tile["CRVAL1"] == tile["CRVAL1"][0]).all()
+        assert not (tile["CRVAL2"] == tile["CRVAL2"][0]).all()
+        assert (tile["CRPIX1"] == tile["CRPIX1"][0]).all()
+        assert (tile["CRPIX2"] == tile["CRPIX2"][0]).all()
+
+    assert (h_table["MAXIS"] == 2).all()
+    assert (h_table["MAXIS1"] == n_X_tiles).all()
+    assert (h_table["MAXIS2"] == n_Y_tiles).all()
+
+    # Assert some things about each timestep
+    time_grouped = h_table.group_by(("DINDEX4"))
+    assert len(time_grouped.groups) == 3
+
+    for time in time_grouped.groups:
+        # Don't test the 3rd (wavelength) axis, because we expect that to be the same
+        assert not (time["CRPIX1"] == time["CRPIX1"][0]).all()
+        assert not (time["CRPIX2"] == time["CRPIX2"][0]).all()
+        assert not (time["MINDEX1"] == time["MINDEX1"][0]).all()
+        assert not (time["MINDEX2"] == time["MINDEX2"][0]).all()
+
+
 @pytest.mark.parametrize(
     "dataset_class, non_stokes_args",
     [
         pytest.param(
             SimpleCryonirspSPDataset,
             {
                 "n_meas": 1,
@@ -341,15 +387,15 @@
                 "time_delta": 0.5,
                 "linewave": 1083.0 * u.nm,
             },
             id="Cryo CI",
         ),
         pytest.param(
             SimpleDLNIRSPDataset,
-            {"n_exposures": 1, "time_delta": 0.5, "linewave": 1083.0 * u.nm},
+            {"n_mosaic_repeats": 1, "time_delta": 0.5, "linewave": 1083.0 * u.nm},
             id="DL-NIRSP",
         ),
         pytest.param(
             SimpleVISPDataset,
             {"n_maps": 1, "n_steps": 1, "time_delta": 0.5, "linewave": 630.0 * u.nm},
             id="ViSP",
         ),
@@ -410,15 +456,15 @@
                 "linewave": 1083.0 * u.nm,
             },
             id="Cryo CI",
         ),
         pytest.param(
             SimpleDLNIRSPDataset,
             {
-                "n_exposures": 1,
+                "n_mosaic_repeats": 1,
                 "n_stokes": 4,
                 "time_delta": 0.5,
                 "linewave": 1083.0 * u.nm,
             },
             id="DL-NIRSP",
         ),
         pytest.param(
```

### Comparing `dkist_data_simulator-5.1.1rc1/dkist_data_simulator/tests/test_214_inventory.py` & `dkist_data_simulator-5.2.0rc1/dkist_data_simulator/tests/test_214_inventory.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,15 +23,18 @@
 
 from dkist_data_simulator.dataset import key_function
 from dkist_data_simulator.spec214 import Spec214Dataset
 from dkist_data_simulator.spec214.cryo import (
     SimpleCryonirspCIDataset,
     SimpleCryonirspSPDataset,
 )
-from dkist_data_simulator.spec214.dlnirsp import SimpleDLNIRSPDataset
+from dkist_data_simulator.spec214.dlnirsp import (
+    MosaicedDLNIRSPDataset,
+    SimpleDLNIRSPDataset,
+)
 from dkist_data_simulator.spec214.vbi import MosaicedVBIBlueDataset, SimpleVBIDataset
 from dkist_data_simulator.spec214.visp import SimpleVISPDataset
 from dkist_data_simulator.spec214.vtf import SimpleVTFDataset
 
 
 class DatasetTest214(Spec214Dataset):
     @property
@@ -53,15 +56,24 @@
     def framewav(self, key: str):
         """
         Add a random framewav around the line centre
         """
         return (np.random.random() - 0.5) * 100
 
 
-INVENTORY_LT_0_18 = Version(dkist_inventory.__version__) < Version("0.18.dev0")
+def inventory_version_skip(version):
+    """
+    Return a pytest mark based on a version of dkist-inventory.
+
+    This is just pytest.mark.skipif but for a dynamic version.
+    """
+    return pytest.mark.skipif(
+        Version(dkist_inventory.__version__) < Version(version),
+        reason=f"dkist-inventory must have a version higher than {version}",
+    )
 
 
 @pytest.mark.parametrize(
     "ds",
     (
         pytest.param(
             DatasetTest214(
@@ -103,137 +115,131 @@
                 n_steps=3,
                 n_maps=3,
                 n_stokes=4,
                 time_delta=10,
                 linewave=500 * u.m,
             ),
             id="SimpleCryonirspSPDataset-polarized-single-meas",
-            marks=pytest.mark.skipif(
-                INVENTORY_LT_0_18, reason="needs dkist_inventory 1.18"
-            ),
+            marks=inventory_version_skip("0.18.dev0"),
         ),
         pytest.param(
             SimpleCryonirspSPDataset(
                 n_meas=2,
                 n_steps=3,
                 n_maps=3,
                 n_stokes=4,
                 time_delta=10,
                 linewave=500 * u.m,
             ),
             id="SimpleCryonirspSPDataset-polarized-multiple-meas",
-            marks=pytest.mark.skipif(
-                INVENTORY_LT_0_18, reason="needs dkist_inventory 1.18"
-            ),
+            marks=inventory_version_skip("0.18.dev0"),
         ),
         pytest.param(
             SimpleCryonirspSPDataset(
                 n_meas=1,
                 n_steps=3,
                 n_maps=3,
                 n_stokes=1,
                 time_delta=10,
                 linewave=500 * u.m,
             ),
             id="SimpleCryonirspSPDataset-single-meas",
-            marks=pytest.mark.skipif(
-                INVENTORY_LT_0_18, reason="needs dkist_inventory 1.18"
-            ),
+            marks=inventory_version_skip("0.18.dev0"),
         ),
         pytest.param(
             SimpleCryonirspSPDataset(
                 n_meas=2,
                 n_steps=3,
                 n_maps=3,
                 n_stokes=1,
                 time_delta=10,
                 linewave=500 * u.m,
             ),
             id="SimpleCryonirspSPDataset-multiple-meas",
-            marks=pytest.mark.skipif(
-                INVENTORY_LT_0_18, reason="needs dkist_inventory 1.18"
-            ),
+            marks=inventory_version_skip("0.18.dev0"),
         ),
         pytest.param(
             SimpleCryonirspCIDataset(
                 n_meas=1,
                 n_steps=3,
                 n_maps=3,
                 n_stokes=4,
                 time_delta=10,
                 linewave=500 * u.m,
             ),
             id="SimpleCryonirspCIDataset-polarized-single-meas",
-            marks=pytest.mark.skipif(
-                INVENTORY_LT_0_18, reason="needs dkist_inventory 1.18"
-            ),
+            marks=inventory_version_skip("0.18.dev0"),
         ),
         pytest.param(
             SimpleCryonirspCIDataset(
                 n_meas=2,
                 n_steps=3,
                 n_maps=3,
                 n_stokes=4,
                 time_delta=10,
                 linewave=500 * u.m,
             ),
             id="SimpleCryonirspCIDataset-polarized-multiple-meas",
-            marks=pytest.mark.skipif(
-                INVENTORY_LT_0_18, reason="needs dkist_inventory 1.18"
-            ),
+            marks=inventory_version_skip("0.18.dev0"),
         ),
         pytest.param(
             SimpleCryonirspCIDataset(
                 n_meas=1,
                 n_steps=3,
                 n_maps=3,
                 n_stokes=1,
                 time_delta=10,
                 linewave=500 * u.m,
             ),
             id="SimpleCryonirspCIDataset-single-meas",
-            marks=pytest.mark.skipif(
-                INVENTORY_LT_0_18, reason="needs dkist_inventory 1.18"
-            ),
+            marks=inventory_version_skip("0.18.dev0"),
         ),
         pytest.param(
             SimpleCryonirspCIDataset(
                 n_meas=2,
                 n_steps=3,
                 n_maps=3,
                 n_stokes=1,
                 time_delta=10,
                 linewave=500 * u.m,
             ),
             id="SimpleCryonirspCIDataset-multiple-meas",
-            marks=pytest.mark.skipif(
-                INVENTORY_LT_0_18, reason="needs dkist_inventory 1.18"
-            ),
+            marks=inventory_version_skip("0.18.dev0"),
         ),
         pytest.param(
             SimpleDLNIRSPDataset(
-                n_exposures=3, n_stokes=4, time_delta=10, linewave=400 * u.nm
+                n_mosaic_repeats=3, n_stokes=4, time_delta=10, linewave=400 * u.nm
             ),
             id="SimpleDLNIRSPDataset-polarized",
-            marks=pytest.mark.skipif(
-                INVENTORY_LT_0_18, reason="needs dkist_inventory 1.18"
-            ),
+            marks=inventory_version_skip("0.18.dev0"),
         ),
         pytest.param(
             SimpleDLNIRSPDataset(
-                n_exposures=3, n_stokes=0, time_delta=10, linewave=400 * u.nm
+                n_mosaic_repeats=3, n_stokes=0, time_delta=10, linewave=400 * u.nm
             ),
             id="SimpleDLNIRSPDataset",
-            marks=pytest.mark.skipif(
-                INVENTORY_LT_0_18, reason="needs dkist_inventory 1.18"
-            ),
+            marks=inventory_version_skip("0.18.dev0"),
         ),
         pytest.param(
             MosaicedVBIBlueDataset(n_time=2, time_delta=10, linewave=400 * u.nm),
             id="MosaicedVBIBlueDataset",
+            marks=inventory_version_skip("1.4.0.dev0"),
+        ),
+        pytest.param(
+            MosaicedDLNIRSPDataset(
+                n_mosaic_repeats=3,
+                n_X_tiles=2,
+                n_Y_tiles=2,
+                n_stokes=4,
+                time_delta=1,
+                linewave=1083 * u.nm,
+                array_shape=(10, 10, 10),
+            ),
+            id="MosaicedDLNIRSPDataset",
+            marks=inventory_version_skip("1.4.0.dev0"),
         ),
     ),
 )
 def test_generate_214(ds):
     headers = ds.generate_headers()
 
     # Assert that the datasets generated here pass through gwcs generation and inventory creation.
```

### Comparing `dkist_data_simulator-5.1.1rc1/dkist_data_simulator/tests/test_dataset.py` & `dkist_data_simulator-5.2.0rc1/dkist_data_simulator/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-5.1.1rc1/dkist_data_simulator/util.py` & `dkist_data_simulator-5.2.0rc1/dkist_data_simulator/util.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-5.1.1rc1/dkist_data_simulator.egg-info/PKG-INFO` & `dkist_data_simulator-5.2.0rc1/dkist_data_simulator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: dkist_data_simulator
-Version: 5.1.1rc1
+Version: 5.2.0rc1
 Summary: A header generator and FITS file creator for DKIST data.
 Home-page: 
 Author: AURA / NSO
 Author-email: stuart@cadair.com
 License: BSD 3-Clause
 License-File: licenses/LICENSE.rst
-Requires-Dist: dkist-fits-specifications>=4.1.1rc1
+Requires-Dist: dkist-fits-specifications>=4.1.1
 Requires-Dist: hashids
 Requires-Dist: tqdm
 Requires-Dist: sunpy
 Requires-Dist: astropy
 Requires-Dist: scipy
 Provides-Extra: all
 Provides-Extra: test
@@ -33,15 +33,15 @@
 
 Using
 -----
 
 Generating Pesudo Random Data
 #############################
 
-The simplest way to generate data is to to use the `dkist_data_simulator.spec122.Spec122Dataset` or `dkist_data_simulator.spec214.Spec214Dataset` classes.
+The simplest way to generate data is to use the `dkist_data_simulator.spec122.Spec122Dataset` or `dkist_data_simulator.spec214.Spec214Dataset` classes.
 
 To generate a header::
 
   >>> from dkist_data_simulator.spec122 import Spec122Dataset
   >>> ds = Spec122Dataset(dataset_shape=(1, 512, 512), array_shape=(1, 512, 512), time_delta=10)
   >>> ds.header()
```

### Comparing `dkist_data_simulator-5.1.1rc1/dkist_data_simulator.egg-info/SOURCES.txt` & `dkist_data_simulator-5.2.0rc1/dkist_data_simulator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-5.1.1rc1/docs/Makefile` & `dkist_data_simulator-5.2.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-5.1.1rc1/docs/conf.py` & `dkist_data_simulator-5.2.0rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-5.1.1rc1/docs/make.bat` & `dkist_data_simulator-5.2.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-5.1.1rc1/examples/vtf_crisp_5d.py` & `dkist_data_simulator-5.2.0rc1/examples/vtf_crisp_5d.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-5.1.1rc1/licenses/LICENSE.rst` & `dkist_data_simulator-5.2.0rc1/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-5.1.1rc1/licenses/TEMPLATE_LICENSE.rst` & `dkist_data_simulator-5.2.0rc1/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-5.1.1rc1/setup.cfg` & `dkist_data_simulator-5.2.0rc1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 [options]
 zip_safe = False
 packages = find:
 python_requires > = 3.9
 setup_requires = setuptools_scm
 install_requires = 
-	dkist-fits-specifications >= 4.1.1rc1
+	dkist-fits-specifications >= 4.1.1
 	hashids
 	tqdm
 	sunpy
 	astropy
 	scipy
 
 [options.extras_require]
```

### Comparing `dkist_data_simulator-5.1.1rc1/setup.py` & `dkist_data_simulator-5.2.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-5.1.1rc1/tox.ini` & `dkist_data_simulator-5.2.0rc1/tox.ini`

 * *Files identical despite different names*

