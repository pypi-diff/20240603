# Comparing `tmp/financeager-1.3.7.tar.gz` & `tmp/financeager-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "financeager-1.3.7.tar", last modified: Tue Apr  2 18:31:45 2024, max compression
+gzip compressed data, was "financeager-1.3.8.tar", last modified: Mon Jun  3 12:50:43 2024, max compression
```

## Comparing `financeager-1.3.7.tar` & `financeager-1.3.8.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:31:45.898477 financeager-1.3.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:31:45.890477 financeager-1.3.7/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-02 18:31:29.000000 financeager-1.3.7/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:31:45.894477 financeager-1.3.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-02 18:31:29.000000 financeager-1.3.7/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-02 18:31:29.000000 financeager-1.3.7/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-02 18:31:29.000000 financeager-1.3.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-02 18:31:29.000000 financeager-1.3.7/.gitlint
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-02 18:31:29.000000 financeager-1.3.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13591 2024-04-02 18:31:29.000000 financeager-1.3.7/Changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-02 18:31:29.000000 financeager-1.3.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-02 18:31:29.000000 financeager-1.3.7/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    15279 2024-04-02 18:31:45.898477 financeager-1.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13432 2024-04-02 18:31:29.000000 financeager-1.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:31:45.894477 financeager-1.3.7/examples/
--rw-r--r--   0 runner    (1001) docker     (127)   214498 2024-04-02 18:31:29.000000 financeager-1.3.7/examples/quickstart.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:31:45.894477 financeager-1.3.7/financeager/
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-02 18:31:29.000000 financeager-1.3.7/financeager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16375 2024-04-02 18:31:29.000000 financeager-1.3.7/financeager/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-02 18:31:29.000000 financeager-1.3.7/financeager/clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-04-02 18:31:29.000000 financeager-1.3.7/financeager/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-04-02 18:31:29.000000 financeager-1.3.7/financeager/entries.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-02 18:31:29.000000 financeager-1.3.7/financeager/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-04-02 18:31:29.000000 financeager-1.3.7/financeager/listing.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-02 18:31:29.000000 financeager-1.3.7/financeager/localserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-02 18:31:29.000000 financeager-1.3.7/financeager/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    20048 2024-04-02 18:31:29.000000 financeager-1.3.7/financeager/pocket.py
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-04-02 18:31:29.000000 financeager-1.3.7/financeager/rich.py
--rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-04-02 18:31:29.000000 financeager-1.3.7/financeager/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:31:45.898477 financeager-1.3.7/financeager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15279 2024-04-02 18:31:45.000000 financeager-1.3.7/financeager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-02 18:31:45.000000 financeager-1.3.7/financeager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 18:31:45.000000 financeager-1.3.7/financeager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-02 18:31:45.000000 financeager-1.3.7/financeager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-02 18:31:45.000000 financeager-1.3.7/financeager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 18:31:45.000000 financeager-1.3.7/financeager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-02 18:31:29.000000 financeager-1.3.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 18:31:45.898477 financeager-1.3.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:31:45.898477 financeager-1.3.7/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:31:29.000000 financeager-1.3.7/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20845 2024-04-02 18:31:29.000000 financeager-1.3.7/test/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-02 18:31:29.000000 financeager-1.3.7/test/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-02 18:31:29.000000 financeager-1.3.7/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-02 18:31:29.000000 financeager-1.3.7/test/test_entries.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-02 18:31:29.000000 financeager-1.3.7/test/test_listing.py
--rw-r--r--   0 runner    (1001) docker     (127)    23123 2024-04-02 18:31:29.000000 financeager-1.3.7/test/test_pocket.py
--rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-04-02 18:31:29.000000 financeager-1.3.7/test/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:50:43.582606 financeager-1.3.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:50:43.574606 financeager-1.3.8/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-06-03 12:50:28.000000 financeager-1.3.8/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:50:43.574606 financeager-1.3.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-06-03 12:50:28.000000 financeager-1.3.8/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-06-03 12:50:28.000000 financeager-1.3.8/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-06-03 12:50:28.000000 financeager-1.3.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-06-03 12:50:28.000000 financeager-1.3.8/.gitlint
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-06-03 12:50:28.000000 financeager-1.3.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13761 2024-06-03 12:50:28.000000 financeager-1.3.8/Changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-06-03 12:50:28.000000 financeager-1.3.8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-06-03 12:50:28.000000 financeager-1.3.8/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    15387 2024-06-03 12:50:43.582606 financeager-1.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13432 2024-06-03 12:50:28.000000 financeager-1.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:50:43.574606 financeager-1.3.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)   214498 2024-06-03 12:50:28.000000 financeager-1.3.8/examples/quickstart.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:50:43.578606 financeager-1.3.8/financeager/
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-06-03 12:50:28.000000 financeager-1.3.8/financeager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16531 2024-06-03 12:50:28.000000 financeager-1.3.8/financeager/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-06-03 12:50:28.000000 financeager-1.3.8/financeager/clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-06-03 12:50:28.000000 financeager-1.3.8/financeager/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-06-03 12:50:28.000000 financeager-1.3.8/financeager/entries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-06-03 12:50:28.000000 financeager-1.3.8/financeager/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-06-03 12:50:28.000000 financeager-1.3.8/financeager/listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-06-03 12:50:28.000000 financeager-1.3.8/financeager/localserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-06-03 12:50:28.000000 financeager-1.3.8/financeager/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20048 2024-06-03 12:50:28.000000 financeager-1.3.8/financeager/pocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-06-03 12:50:28.000000 financeager-1.3.8/financeager/rich.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-06-03 12:50:28.000000 financeager-1.3.8/financeager/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:50:43.578606 financeager-1.3.8/financeager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15387 2024-06-03 12:50:43.000000 financeager-1.3.8/financeager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-06-03 12:50:43.000000 financeager-1.3.8/financeager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 12:50:43.000000 financeager-1.3.8/financeager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-06-03 12:50:43.000000 financeager-1.3.8/financeager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-06-03 12:50:43.000000 financeager-1.3.8/financeager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-06-03 12:50:43.000000 financeager-1.3.8/financeager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-06-03 12:50:28.000000 financeager-1.3.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 12:50:43.582606 financeager-1.3.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:50:43.578606 financeager-1.3.8/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:50:28.000000 financeager-1.3.8/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20845 2024-06-03 12:50:28.000000 financeager-1.3.8/test/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-06-03 12:50:28.000000 financeager-1.3.8/test/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-06-03 12:50:28.000000 financeager-1.3.8/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-06-03 12:50:28.000000 financeager-1.3.8/test/test_entries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-06-03 12:50:28.000000 financeager-1.3.8/test/test_listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23123 2024-06-03 12:50:28.000000 financeager-1.3.8/test/test_pocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-06-03 12:50:28.000000 financeager-1.3.8/test/test_server.py
```

### Comparing `financeager-1.3.7/.github/workflows/ci.yml` & `financeager-1.3.8/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `financeager-1.3.7/.github/workflows/release.yml` & `financeager-1.3.8/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `financeager-1.3.7/.pre-commit-config.yaml` & `financeager-1.3.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `financeager-1.3.7/Changelog.md` & `financeager-1.3.8/Changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,20 @@
 ## [unreleased]
 ### Added
 ### Changed
 ### Fixed
 ### Removed
 ### Deprecated
 
+## [v1.3.8] - 2024-06-03
+### Fixed
+- Replace usage of deprecated `pkg_resources` module.
+### Changed
+- Update dependencies `argcomplete` and `marshmallow`. (#218, #219)
+
 ## [v1.3.7] - 2024-04-02
 ### Changed
 - Update dependencies `rich`, `python-dateutil`, `argcomplete` and `marshmallow`. (#206, #209, #211, #212, #215)
 
 ## [v1.3.6] - 2024-02-16
 ### Changed
 - Update dependencies `argcomplete` and `marshmallow`. (#197, #203)
```

### Comparing `financeager-1.3.7/LICENSE.md` & `financeager-1.3.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `financeager-1.3.7/Makefile` & `financeager-1.3.8/Makefile`

 * *Files identical despite different names*

### Comparing `financeager-1.3.7/PKG-INFO` & `financeager-1.3.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: financeager
-Version: 1.3.7
+Version: 1.3.8
 Summary: command line tool for organizing finances
 Author-email: Philipp Metzner <beth.aleph@yahoo.de>
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/pylipp/financeager/issues
 Project-URL: Documentation, https://github.com/pylipp/financeager
 Project-URL: Homepage, https://github.com/pylipp/financeager
 Project-URL: Source Code, https://github.com/pylipp/financeager
@@ -22,27 +22,28 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Database
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: appdirs==1.4.4
-Requires-Dist: argcomplete==3.2.3
-Requires-Dist: marshmallow==3.21.1
+Requires-Dist: argcomplete==3.3.0
+Requires-Dist: marshmallow==3.21.2
 Requires-Dist: python-dateutil==2.9.0.post0
 Requires-Dist: rich==13.7.1
 Requires-Dist: tinydb==4.8.0
 Provides-Extra: develop
-Requires-Dist: black==24.2.0; extra == "develop"
-Requires-Dist: coverage==7.4.4; extra == "develop"
+Requires-Dist: black==24.4.2; extra == "develop"
+Requires-Dist: coverage==7.5.3; extra == "develop"
 Requires-Dist: flake8==7.0.0; extra == "develop"
 Requires-Dist: flake8-pyproject==1.2.3; extra == "develop"
 Requires-Dist: gitlint-core==0.19.1; extra == "develop"
 Requires-Dist: isort==5.13.2; extra == "develop"
-Requires-Dist: pre-commit==3.5.0; extra == "develop"
+Requires-Dist: pre-commit==3.7.1; python_version >= "3.9" and extra == "develop"
+Requires-Dist: pre-commit==3.5.0; python_version < "3.9" and extra == "develop"
 Provides-Extra: packaging
 Requires-Dist: build; extra == "packaging"
 
 [![pypi](https://badge.fury.io/py/financeager.svg)](https://pypi.org/project/flake8-pytest-style)
 [![Python: 3.8+](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://pypi.org/project/financeager)
 [![Downloads](https://img.shields.io/pypi/dm/financeager.svg)](https://pypistats.org/packages/flake8-pytest-style)
 ![Build Status](https://github.com/pylipp/financeager/workflows/CI/badge.svg)
```

### Comparing `financeager-1.3.7/README.md` & `financeager-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `financeager-1.3.7/examples/quickstart.svg` & `financeager-1.3.8/examples/quickstart.svg`

 * *Files identical despite different names*

### Comparing `financeager-1.3.7/financeager/__init__.py` & `financeager-1.3.8/financeager/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import os.path
+from importlib.metadata import version
 from logging import DEBUG, WARN, Formatter, StreamHandler, getLogger, handlers
 
 import appdirs
 
 # versioning information
-from pkg_resources import get_distribution
-
-__version__ = get_distribution(__name__).version
+__version__ = version(__name__)
 
 #
 # Global constants
 #
 
 # default name of database
 DEFAULT_POCKET_NAME = "main"
```

### Comparing `financeager-1.3.7/financeager/cli.py` & `financeager-1.3.8/financeager/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 # PYTHON_ARGCOMPLETE_OK
 import argparse
 import os
 import sys
 import time
 from datetime import datetime
+from importlib.metadata import entry_points
 
 import argcomplete
-import pkg_resources
 from dateutil import parser as du_parser
 from rich.console import Console
 
 import financeager
 
 from . import (
     POCKET_DATE_FORMAT,
@@ -46,17 +46,20 @@
     'run()'.
     """
     os.makedirs(financeager.DATA_DIR, exist_ok=True)
 
     # Adding the FileHandler here avoids cluttering the log during tests
     setup_log_file_handler()
 
-    plugins = [
-        ep.load()() for ep in pkg_resources.iter_entry_points("financeager.services")
-    ]
+    group = "financeager.services"
+    try:
+        plugins = [ep.load()() for ep in entry_points().select(group=group)]
+    except AttributeError:
+        # Python 3.8
+        plugins = [ep.load()() for ep in entry_points().get(group, [])]
 
     args = _parse_command(plugins=plugins)
     try:
         configuration = config.Configuration(
             args.pop("config_filepath"), plugins=plugins
         )
         exit_code = run(configuration=configuration, plugins=plugins, **args)
```

### Comparing `financeager-1.3.7/financeager/clients.py` & `financeager-1.3.8/financeager/clients.py`

 * *Files identical despite different names*

### Comparing `financeager-1.3.7/financeager/config.py` & `financeager-1.3.8/financeager/config.py`

 * *Files identical despite different names*

### Comparing `financeager-1.3.7/financeager/entries.py` & `financeager-1.3.8/financeager/entries.py`

 * *Files identical despite different names*

### Comparing `financeager-1.3.7/financeager/exceptions.py` & `financeager-1.3.8/financeager/exceptions.py`

 * *Files identical despite different names*

### Comparing `financeager-1.3.7/financeager/listing.py` & `financeager-1.3.8/financeager/listing.py`

 * *Files identical despite different names*

### Comparing `financeager-1.3.7/financeager/localserver.py` & `financeager-1.3.8/financeager/localserver.py`

 * *Files identical despite different names*

### Comparing `financeager-1.3.7/financeager/plugin.py` & `financeager-1.3.8/financeager/plugin.py`

 * *Files identical despite different names*

### Comparing `financeager-1.3.7/financeager/pocket.py` & `financeager-1.3.8/financeager/pocket.py`

 * *Files identical despite different names*

### Comparing `financeager-1.3.7/financeager/rich.py` & `financeager-1.3.8/financeager/rich.py`

 * *Files identical despite different names*

### Comparing `financeager-1.3.7/financeager/server.py` & `financeager-1.3.8/financeager/server.py`

 * *Files identical despite different names*

### Comparing `financeager-1.3.7/financeager.egg-info/PKG-INFO` & `financeager-1.3.8/financeager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: financeager
-Version: 1.3.7
+Version: 1.3.8
 Summary: command line tool for organizing finances
 Author-email: Philipp Metzner <beth.aleph@yahoo.de>
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/pylipp/financeager/issues
 Project-URL: Documentation, https://github.com/pylipp/financeager
 Project-URL: Homepage, https://github.com/pylipp/financeager
 Project-URL: Source Code, https://github.com/pylipp/financeager
@@ -22,27 +22,28 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Database
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: appdirs==1.4.4
-Requires-Dist: argcomplete==3.2.3
-Requires-Dist: marshmallow==3.21.1
+Requires-Dist: argcomplete==3.3.0
+Requires-Dist: marshmallow==3.21.2
 Requires-Dist: python-dateutil==2.9.0.post0
 Requires-Dist: rich==13.7.1
 Requires-Dist: tinydb==4.8.0
 Provides-Extra: develop
-Requires-Dist: black==24.2.0; extra == "develop"
-Requires-Dist: coverage==7.4.4; extra == "develop"
+Requires-Dist: black==24.4.2; extra == "develop"
+Requires-Dist: coverage==7.5.3; extra == "develop"
 Requires-Dist: flake8==7.0.0; extra == "develop"
 Requires-Dist: flake8-pyproject==1.2.3; extra == "develop"
 Requires-Dist: gitlint-core==0.19.1; extra == "develop"
 Requires-Dist: isort==5.13.2; extra == "develop"
-Requires-Dist: pre-commit==3.5.0; extra == "develop"
+Requires-Dist: pre-commit==3.7.1; python_version >= "3.9" and extra == "develop"
+Requires-Dist: pre-commit==3.5.0; python_version < "3.9" and extra == "develop"
 Provides-Extra: packaging
 Requires-Dist: build; extra == "packaging"
 
 [![pypi](https://badge.fury.io/py/financeager.svg)](https://pypi.org/project/flake8-pytest-style)
 [![Python: 3.8+](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://pypi.org/project/financeager)
 [![Downloads](https://img.shields.io/pypi/dm/financeager.svg)](https://pypistats.org/packages/flake8-pytest-style)
 ![Build Status](https://github.com/pylipp/financeager/workflows/CI/badge.svg)
```

### Comparing `financeager-1.3.7/financeager.egg-info/SOURCES.txt` & `financeager-1.3.8/financeager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `financeager-1.3.7/pyproject.toml` & `financeager-1.3.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -14,16 +14,16 @@
   "commandline",
   "finances",
 ]
 license = {text = "GPLv3"}
 authors = [{ name = "Philipp Metzner", email = "beth.aleph@yahoo.de" }]
 dependencies = [
   "appdirs==1.4.4",
-  "argcomplete==3.2.3",
-  "marshmallow==3.21.1",
+  "argcomplete==3.3.0",
+  "marshmallow==3.21.2",
   "python-dateutil==2.9.0.post0",
   "rich==13.7.1",
   "tinydb==4.8.0",
 ]
 dynamic = [
   "version",
 ]
@@ -41,21 +41,22 @@
   "Programming Language :: Python :: 3.12",
   "Topic :: Office/Business :: Financial",
   "Topic :: Database",
   "Topic :: Utilities",
 ]
 [project.optional-dependencies]
 develop = [
-  "black==24.2.0",
-  "coverage==7.4.4",
+  "black==24.4.2",
+  "coverage==7.5.3",
   'flake8==7.0.0',
   "flake8-pyproject==1.2.3",
   "gitlint-core==0.19.1",
   'isort==5.13.2',
-  'pre-commit==3.5.0',
+  'pre-commit==3.7.1; python_version >= "3.9"',
+  'pre-commit==3.5.0; python_version < "3.9"',
 ]
 packaging = [
   "build",
 ]
 
 [project.urls]
 "Bug Tracker" = "https://github.com/pylipp/financeager/issues"
```

### Comparing `financeager-1.3.7/test/test_cli.py` & `financeager-1.3.8/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `financeager-1.3.7/test/test_clients.py` & `financeager-1.3.8/test/test_clients.py`

 * *Files identical despite different names*

### Comparing `financeager-1.3.7/test/test_config.py` & `financeager-1.3.8/test/test_config.py`

 * *Files identical despite different names*

### Comparing `financeager-1.3.7/test/test_entries.py` & `financeager-1.3.8/test/test_entries.py`

 * *Files identical despite different names*

### Comparing `financeager-1.3.7/test/test_listing.py` & `financeager-1.3.8/test/test_listing.py`

 * *Files identical despite different names*

### Comparing `financeager-1.3.7/test/test_pocket.py` & `financeager-1.3.8/test/test_pocket.py`

 * *Files identical despite different names*

### Comparing `financeager-1.3.7/test/test_server.py` & `financeager-1.3.8/test/test_server.py`

 * *Files identical despite different names*

