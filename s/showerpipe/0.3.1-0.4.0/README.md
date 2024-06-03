# Comparing `tmp/showerpipe-0.3.1.tar.gz` & `tmp/showerpipe-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "showerpipe-0.3.1.tar", last modified: Wed Oct  4 11:34:24 2023, max compression
+gzip compressed data, was "showerpipe-0.4.0.tar", last modified: Mon Jun  3 09:36:46 2024, max compression
```

## Comparing `showerpipe-0.3.1.tar` & `showerpipe-0.4.0.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 11:34:24.258855 showerpipe-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 11:34:24.250856 showerpipe-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 11:34:24.254855 showerpipe-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-10-04 11:34:12.000000 showerpipe-0.3.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      660 2023-10-04 11:34:12.000000 showerpipe-0.3.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      994 2023-10-04 11:34:12.000000 showerpipe-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2023-10-04 11:34:12.000000 showerpipe-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      236 2023-10-04 11:34:12.000000 showerpipe-0.3.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2023-10-04 11:34:12.000000 showerpipe-0.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4917 2023-10-04 11:34:24.258855 showerpipe-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2023-10-04 11:34:12.000000 showerpipe-0.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 11:34:24.254855 showerpipe-0.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2023-10-04 11:34:12.000000 showerpipe-0.3.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      288 2023-10-04 11:34:12.000000 showerpipe-0.3.1/docs/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      804 2023-10-04 11:34:12.000000 showerpipe-0.3.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 11:34:24.254855 showerpipe-0.3.1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 11:34:24.254855 showerpipe-0.3.1/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 11:34:12.000000 showerpipe-0.3.1/docs/source/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 11:34:24.254855 showerpipe-0.3.1/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 11:34:12.000000 showerpipe-0.3.1/docs/source/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      151 2023-10-04 11:34:12.000000 showerpipe-0.3.1/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2023-10-04 11:34:12.000000 showerpipe-0.3.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2023-10-04 11:34:12.000000 showerpipe-0.3.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      130 2023-10-04 11:34:12.000000 showerpipe-0.3.1/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2023-10-04 11:34:12.000000 showerpipe-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-04 11:34:24.258855 showerpipe-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-10-04 11:34:12.000000 showerpipe-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 11:34:24.254855 showerpipe-0.3.1/showerpipe/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2023-10-04 11:34:12.000000 showerpipe-0.3.1/showerpipe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-10-04 11:34:24.000000 showerpipe-0.3.1/showerpipe/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2023-10-04 11:34:12.000000 showerpipe-0.3.1/showerpipe/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    19516 2023-10-04 11:34:12.000000 showerpipe-0.3.1/showerpipe/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12490 2023-10-04 11:34:12.000000 showerpipe-0.3.1/showerpipe/lhe.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 11:34:12.000000 showerpipe-0.3.1/showerpipe/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 11:34:24.254855 showerpipe-0.3.1/showerpipe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4917 2023-10-04 11:34:24.000000 showerpipe-0.3.1/showerpipe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      696 2023-10-04 11:34:24.000000 showerpipe-0.3.1/showerpipe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-04 11:34:24.000000 showerpipe-0.3.1/showerpipe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      141 2023-10-04 11:34:24.000000 showerpipe-0.3.1/showerpipe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-10-04 11:34:24.000000 showerpipe-0.3.1/showerpipe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 11:34:24.254855 showerpipe-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6845 2023-10-04 11:34:12.000000 showerpipe-0.3.1/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)   135055 2023-10-04 11:34:12.000000 showerpipe-0.3.1/tests/tt_bb_100.lhe.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:36:46.945200 showerpipe-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:36:46.937200 showerpipe-0.4.0/.conda/
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-06-03 09:36:42.000000 showerpipe-0.4.0/.conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:36:46.937200 showerpipe-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:36:46.937200 showerpipe-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-06-03 09:36:42.000000 showerpipe-0.4.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-06-03 09:36:42.000000 showerpipe-0.4.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-06-03 09:36:42.000000 showerpipe-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-06-03 09:36:42.000000 showerpipe-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-06-03 09:36:42.000000 showerpipe-0.4.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-06-03 09:36:42.000000 showerpipe-0.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-06-03 09:36:46.945200 showerpipe-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-06-03 09:36:42.000000 showerpipe-0.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:36:46.937200 showerpipe-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-06-03 09:36:42.000000 showerpipe-0.4.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-06-03 09:36:42.000000 showerpipe-0.4.0/docs/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-06-03 09:36:42.000000 showerpipe-0.4.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:36:46.941200 showerpipe-0.4.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:36:46.941200 showerpipe-0.4.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:36:42.000000 showerpipe-0.4.0/docs/source/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:36:46.941200 showerpipe-0.4.0/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:36:42.000000 showerpipe-0.4.0/docs/source/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-06-03 09:36:42.000000 showerpipe-0.4.0/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-06-03 09:36:42.000000 showerpipe-0.4.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-06-03 09:36:42.000000 showerpipe-0.4.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-06-03 09:36:42.000000 showerpipe-0.4.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-06-03 09:36:42.000000 showerpipe-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 09:36:46.945200 showerpipe-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-06-03 09:36:42.000000 showerpipe-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:36:46.941200 showerpipe-0.4.0/showerpipe/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-06-03 09:36:42.000000 showerpipe-0.4.0/showerpipe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-03 09:36:46.000000 showerpipe-0.4.0/showerpipe/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-06-03 09:36:42.000000 showerpipe-0.4.0/showerpipe/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19516 2024-06-03 09:36:42.000000 showerpipe-0.4.0/showerpipe/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15726 2024-06-03 09:36:42.000000 showerpipe-0.4.0/showerpipe/lhe.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:36:42.000000 showerpipe-0.4.0/showerpipe/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:36:46.941200 showerpipe-0.4.0/showerpipe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-06-03 09:36:46.000000 showerpipe-0.4.0/showerpipe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-06-03 09:36:46.000000 showerpipe-0.4.0/showerpipe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 09:36:46.000000 showerpipe-0.4.0/showerpipe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-06-03 09:36:46.000000 showerpipe-0.4.0/showerpipe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-03 09:36:46.000000 showerpipe-0.4.0/showerpipe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:36:46.941200 showerpipe-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6845 2024-06-03 09:36:42.000000 showerpipe-0.4.0/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)   135055 2024-06-03 09:36:42.000000 showerpipe-0.4.0/tests/tt_bb_100.lhe.gz
```

### Comparing `showerpipe-0.3.1/.github/workflows/publish-to-pypi.yml` & `showerpipe-0.4.0/.github/workflows/publish-to-pypi.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Publish Python
+name: Publish PyPI
 
 on:
   push:
     tags:
       - '*'
 
 jobs:
```

### Comparing `showerpipe-0.3.1/.github/workflows/tests.yml` & `showerpipe-0.4.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `showerpipe-0.3.1/.gitignore` & `showerpipe-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `showerpipe-0.3.1/.pre-commit-config.yaml` & `showerpipe-0.4.0/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # See https://pre-commit.com/hooks.html for more hooks
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
-      - id: check-yaml
       - id: check-added-large-files
       - id: check-merge-conflict
       - id: debug-statements
       - id: name-tests-test
         args: ["--pytest-test-first"]
       - id: no-commit-to-branch
         args: ["--branch", "main", "--branch", "develop"]
```

### Comparing `showerpipe-0.3.1/LICENSE.txt` & `showerpipe-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `showerpipe-0.3.1/PKG-INFO` & `showerpipe-0.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: showerpipe
-Version: 0.3.1
+Version: 0.4.0
 Summary: Data pipeline tools for particle shower and hadronisation.
 Author: Jacan Chaplais
 Maintainer: Jacan Chaplais
 License: BSD 3-Clause License
         
         Copyright (c) 2021, Jacan Chaplais.
         All rights reserved.
@@ -65,50 +65,41 @@
 
 Currently wraps interface for Pythia 8, with plans for Herwig and
 Ariadne in future releases.
 
 Installation
 ------------
 
-This package requires Pythia 8 to be installed on your system, and
-available in your ``PYTHONPATH``.
+Using conda (Recommended)
+~~~~~~~~~~~~~~~~~~~~~~~~~
 
-It also requires the ``PYTHIA8DATA`` environment variable to be set.
-This is the path to the ``xmldoc/`` directory under Pythia’s ``share``
-directory. You can do something like this in your shell config:
+The easiest solution is to just install via conda:
 
 .. code:: bash
 
-   export PYTHIA8DATA=/home/$USER/pythia82xx/share/Pythia8/xmldoc
-
-Without an existing Pythia installation (using conda)
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+   conda install -c jacanchaplais showerpipe
 
-If this is not already the case, a very convenient solution is to
-install it via ``conda``. This is fast, and automatically sets the
-``PYTHIA8DATA`` environment variable when you activate the virtual
-environment. An environment file is provided in the root of this repo,
-which will install all requirements and then showerpipe, automatically.
-The virtual environment can be created using:
+Pythia will be included as a dependency, and all relevant paths and
+environment variables will be properly set.
 
-.. code:: bash
+Using existing Pythia installation
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-   conda env create -f environment.yml
+If Pythia 8 is already installed on your system, and available in your
+``PYTHONPATH``, you can just install this package via ``pip``.
 
-If you have an existing conda environment, you can update it by
-activating the environment and then using:
+It also requires the ``PYTHIA8DATA`` environment variable to be set.
+This is the path to the ``xmldoc/`` directory under Pythia’s ``share``
+directory. You can do something like this in your shell config:
 
 .. code:: bash
 
-   conda env update -f environment.yml --prune
-
-With existing Pythia installation
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+   export PYTHIA8DATA=/home/$USER/pythia82xx/share/Pythia8/xmldoc
 
-Simply:
+With everything set up properly, simply run:
 
 .. code:: bash
 
    pip install showerpipe
 
 .. |PyPI version| image:: https://img.shields.io/pypi/v/showerpipe.svg
    :target: https://pypi.org/project/showerpipe/
```

### Comparing `showerpipe-0.3.1/README.rst` & `showerpipe-0.4.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -8,50 +8,41 @@
 
 Currently wraps interface for Pythia 8, with plans for Herwig and
 Ariadne in future releases.
 
 Installation
 ------------
 
-This package requires Pythia 8 to be installed on your system, and
-available in your ``PYTHONPATH``.
+Using conda (Recommended)
+~~~~~~~~~~~~~~~~~~~~~~~~~
 
-It also requires the ``PYTHIA8DATA`` environment variable to be set.
-This is the path to the ``xmldoc/`` directory under Pythia’s ``share``
-directory. You can do something like this in your shell config:
+The easiest solution is to just install via conda:
 
 .. code:: bash
 
-   export PYTHIA8DATA=/home/$USER/pythia82xx/share/Pythia8/xmldoc
-
-Without an existing Pythia installation (using conda)
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+   conda install -c jacanchaplais showerpipe
 
-If this is not already the case, a very convenient solution is to
-install it via ``conda``. This is fast, and automatically sets the
-``PYTHIA8DATA`` environment variable when you activate the virtual
-environment. An environment file is provided in the root of this repo,
-which will install all requirements and then showerpipe, automatically.
-The virtual environment can be created using:
+Pythia will be included as a dependency, and all relevant paths and
+environment variables will be properly set.
 
-.. code:: bash
+Using existing Pythia installation
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-   conda env create -f environment.yml
+If Pythia 8 is already installed on your system, and available in your
+``PYTHONPATH``, you can just install this package via ``pip``.
 
-If you have an existing conda environment, you can update it by
-activating the environment and then using:
+It also requires the ``PYTHIA8DATA`` environment variable to be set.
+This is the path to the ``xmldoc/`` directory under Pythia’s ``share``
+directory. You can do something like this in your shell config:
 
 .. code:: bash
 
-   conda env update -f environment.yml --prune
-
-With existing Pythia installation
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+   export PYTHIA8DATA=/home/$USER/pythia82xx/share/Pythia8/xmldoc
 
-Simply:
+With everything set up properly, simply run:
 
 .. code:: bash
 
    pip install showerpipe
 
 .. |PyPI version| image:: https://img.shields.io/pypi/v/showerpipe.svg
    :target: https://pypi.org/project/showerpipe/
```

### Comparing `showerpipe-0.3.1/docs/Makefile` & `showerpipe-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `showerpipe-0.3.1/docs/make.bat` & `showerpipe-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `showerpipe-0.3.1/docs/source/conf.py` & `showerpipe-0.4.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `showerpipe-0.3.1/pyproject.toml` & `showerpipe-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `showerpipe-0.3.1/showerpipe/base.py` & `showerpipe-0.4.0/showerpipe/base.py`

 * *Files identical despite different names*

### Comparing `showerpipe-0.3.1/showerpipe/generator.py` & `showerpipe-0.4.0/showerpipe/generator.py`

 * *Files identical despite different names*

### Comparing `showerpipe-0.3.1/showerpipe/lhe.py` & `showerpipe-0.4.0/showerpipe/lhe.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,34 +2,45 @@
 ``showerpipe.lhe``
 ==================
 
 The ShowerPipe Les Houches functions utilise xml parsing techniques to
 redistribute and repeat hard events, outputting valid lhe files.
 """
 
-from typing import Union, Iterator, Optional, Callable
+import dataclasses as dc
+import gzip
 import io
+import itertools as it
 import re
-import gzip
 import shutil
-from contextlib import contextmanager, ExitStack
 import tempfile
-from pathlib import Path
+from contextlib import ExitStack, contextmanager
 from copy import deepcopy
-from itertools import chain
 from functools import cached_property
-from xml.sax.saxutils import unescape
+from pathlib import Path
+from typing import Callable, Iterator, Optional, Union
 from urllib.parse import urlparse
 from urllib.request import urlopen
+from xml.sax.saxutils import unescape
 
+import numpy as np
+import numpy.typing as npt
 from lxml import etree  # type: ignore
 from lxml.etree import ElementBase
 
-
-__all__ = ["source_adapter", "load_lhe", "count_events", "split", "LheData"]
+__all__ = [
+    "source_adapter",
+    "load_lhe",
+    "count_events",
+    "split",
+    "LheData",
+    "LheData",
+    "event_iter_text",
+    "event_iter",
+]
 
 _LHE_STORAGE = Union[Path, str, bytes]
 
 _parse_kwargs = dict(
     resolve_entities=False,
     remove_comments=False,
     strip_cdata=False,
@@ -64,17 +75,17 @@
     is_url = False
     out_io: io.BufferedIOBase
     if is_str:
         is_url = bool(urlparse(source).netloc)  # type: ignore
     if is_path:
         path = Path(source)  # type: ignore
         try:
-            with io.open(path, "r") as lhe_filecheck:
+            with open(path) as lhe_filecheck:
                 lhe_filecheck.read(1)
-            out_io = io.open(path, "rb")
+            out_io = open(path, "rb")
             yield out_io
         except UnicodeDecodeError:
             out_io = gzip.open(path, "rb")
             out_io.read(1)
             out_io.seek(0)
             yield out_io
         finally:
@@ -118,15 +129,15 @@
 
 
 def _get_mg_info(header_element: ElementBase) -> ElementBase:
     return header_element.find("MGGenerationInfo")
 
 
 def _read_num_events(mg_info: ElementBase) -> int:
-    re_num = re.findall("\d+", mg_info.text)
+    re_num = re.findall(r"\d+", mg_info.text)
     num_events = int(re_num[0])
     return num_events
 
 
 def _update_num_events(mg_info: ElementBase, new_num: int) -> ElementBase:
     mg_info = deepcopy(mg_info)
     prev_num = _read_num_events(mg_info)
@@ -384,22 +395,128 @@
     def _event_duplicator(
         self,
         repeats: int,
         inplace: bool,
         dup_strat: Callable[[Iterator[ElementBase]], Iterator[ElementBase]],
     ) -> Optional[bytes]:
         tiled_lists = (self._event_iter for _ in range(repeats))
-        dup_events = chain.from_iterable(dup_strat(tiled_lists))
+        dup_events = it.chain.from_iterable(dup_strat(tiled_lists))
         dup_event_copies = map(deepcopy, dup_events)
         root = self._build_root(dup_event_copies)
         header = root[0]
         mg_info = _get_mg_info(header_element=header)
         prev_num = self.num_events
         new_num = prev_num * repeats
         header.replace(mg_info, _update_num_events(mg_info, new_num))
         if inplace is True:
             self._root = root
             if self.num_events is not None:
                 del self.num_events
             return None
         else:
             return _root_to_bytes(root)
+
+
+@dc.dataclass
+class LheEvent:
+    """Data structure holding Les Houches event data.
+
+    :group: LesHouches
+
+    .. versionadded:: 0.4.0
+
+    Attributes
+    ----------
+    pdg : ndarray[int32]
+        PDG / MCPID identification codes for particle species.
+    pmu : ndarray[float64]
+        Four-momenta of particles, in (px, py, pz, E) order.
+    status : ndarray[int16]
+        Codes referring to the role of particles in the event, **eg.**
+        beam particle, incoming, outgoing, **etc.**
+    helicity : ndarray[int16]
+        Spin polarity of the particles.
+    color : ndarray[int32]
+        Color / anti-color code pairs of the particles.
+    """
+
+    pdg: npt.NDArray[np.int32]
+    pmu: npt.NDArray[np.float64]
+    status: npt.NDArray[np.int16]
+    helicity: npt.NDArray[np.int16]
+    color: npt.NDArray[np.int32]
+
+
+def _event_text_parse(event_text: str) -> LheEvent:
+    schema = {
+        "pdg": {"idx": 0, "dtype": np.int32},
+        "status": {"idx": 1, "dtype": np.int16},
+        "color": {"idx": slice(4, 6), "dtype": np.int32},
+        "pmu": {"idx": slice(6, 10), "dtype": np.float64},
+        "helicity": {"idx": 12, "dtype": np.int16},
+    }
+    lines = event_text.strip().split("\n")[1:]
+    data = np.loadtxt(iter(lines), dtype=np.float64)
+    return LheEvent(
+        **{
+            name: data[:, meta["idx"]].astype(meta["dtype"])
+            for name, meta in schema.items()
+        }
+    )
+
+
+def event_iter_text(source: _LHE_STORAGE) -> Iterator[str]:
+    """Iterates over a LHE file, yielding the text contained within an
+    event block.
+    See https://arxiv.org/abs/hep-ph/0109068 for the data layout.
+
+    :group: LesHouches
+
+    .. versionadded:: 0.4.0
+
+    Parameters
+    ----------
+    source : Pathlike, string, or bytes
+        The variable or filepath containing the LHE data. May be a path,
+        url, string, or bytes object. Gzip compression is allowed.
+
+    Yields
+    ------
+    str
+        The text block contained in each successive event.
+    """
+    with source_adapter(source) as xml_source:
+        event_parser = etree.iterparse(
+            source=xml_source, tag=("event",), **_parse_kwargs
+        )
+        for _, event in event_parser:
+            yield event.text.strip()
+
+
+def event_iter(source: _LHE_STORAGE) -> Iterator[LheEvent]:
+    """Iterates over a LHE file, yielding ``LheEvent`` objects,
+    providing attribute access to numpy arrays, containing particle
+    data.
+
+    :group: LesHouches
+
+    .. versionadded:: 0.4.0
+
+    Parameters
+    ----------
+    source : Pathlike, string, or bytes
+        The variable or filepath containing the LHE data. May be a path,
+        url, string, or bytes object. Gzip compression is allowed.
+
+    Yields
+    ------
+    LheEvent
+        Numpy interface to the event data.
+
+    Notes
+    -----
+    This is a wrapper around ``event_iter_text()``, but provides only a
+    subset of the fields available as attributes. For more complete data
+    you may wish to use ``event_iter_text()`` and parse the strings
+    yourself.
+    """
+    yield from map(_event_text_parse, event_iter_text(source))
```

### Comparing `showerpipe-0.3.1/showerpipe.egg-info/PKG-INFO` & `showerpipe-0.4.0/showerpipe.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: showerpipe
-Version: 0.3.1
+Version: 0.4.0
 Summary: Data pipeline tools for particle shower and hadronisation.
 Author: Jacan Chaplais
 Maintainer: Jacan Chaplais
 License: BSD 3-Clause License
         
         Copyright (c) 2021, Jacan Chaplais.
         All rights reserved.
@@ -65,50 +65,41 @@
 
 Currently wraps interface for Pythia 8, with plans for Herwig and
 Ariadne in future releases.
 
 Installation
 ------------
 
-This package requires Pythia 8 to be installed on your system, and
-available in your ``PYTHONPATH``.
+Using conda (Recommended)
+~~~~~~~~~~~~~~~~~~~~~~~~~
 
-It also requires the ``PYTHIA8DATA`` environment variable to be set.
-This is the path to the ``xmldoc/`` directory under Pythia’s ``share``
-directory. You can do something like this in your shell config:
+The easiest solution is to just install via conda:
 
 .. code:: bash
 
-   export PYTHIA8DATA=/home/$USER/pythia82xx/share/Pythia8/xmldoc
-
-Without an existing Pythia installation (using conda)
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+   conda install -c jacanchaplais showerpipe
 
-If this is not already the case, a very convenient solution is to
-install it via ``conda``. This is fast, and automatically sets the
-``PYTHIA8DATA`` environment variable when you activate the virtual
-environment. An environment file is provided in the root of this repo,
-which will install all requirements and then showerpipe, automatically.
-The virtual environment can be created using:
+Pythia will be included as a dependency, and all relevant paths and
+environment variables will be properly set.
 
-.. code:: bash
+Using existing Pythia installation
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-   conda env create -f environment.yml
+If Pythia 8 is already installed on your system, and available in your
+``PYTHONPATH``, you can just install this package via ``pip``.
 
-If you have an existing conda environment, you can update it by
-activating the environment and then using:
+It also requires the ``PYTHIA8DATA`` environment variable to be set.
+This is the path to the ``xmldoc/`` directory under Pythia’s ``share``
+directory. You can do something like this in your shell config:
 
 .. code:: bash
 
-   conda env update -f environment.yml --prune
-
-With existing Pythia installation
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+   export PYTHIA8DATA=/home/$USER/pythia82xx/share/Pythia8/xmldoc
 
-Simply:
+With everything set up properly, simply run:
 
 .. code:: bash
 
    pip install showerpipe
 
 .. |PyPI version| image:: https://img.shields.io/pypi/v/showerpipe.svg
    :target: https://pypi.org/project/showerpipe/
```

### Comparing `showerpipe-0.3.1/showerpipe.egg-info/SOURCES.txt` & `showerpipe-0.4.0/showerpipe.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 .pre-commit-config.yaml
 .readthedocs.yaml
 LICENSE.txt
 README.rst
 environment.yml
 pyproject.toml
 setup.py
+.conda/meta.yaml
 .github/workflows/publish-to-pypi.yml
 .github/workflows/tests.yml
 docs/Makefile
 docs/environment.yml
 docs/make.bat
 docs/source/api.rst
 docs/source/conf.py
```

### Comparing `showerpipe-0.3.1/tests/test_generator.py` & `showerpipe-0.4.0/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `showerpipe-0.3.1/tests/tt_bb_100.lhe.gz` & `showerpipe-0.4.0/tests/tt_bb_100.lhe.gz`

 * *Files identical despite different names*

