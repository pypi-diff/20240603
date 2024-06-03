# Comparing `tmp/dargs-0.4.5.tar.gz` & `tmp/dargs-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/dargs/dargs/dist/.tmp-3umrb0v1/dargs-0.4.5.tar", last modified: Sat Apr  6 04:45:34 2024, max compression
+gzip compressed data, was "/home/runner/work/dargs/dargs/dist/.tmp-6pynmvcl/dargs-0.4.6.tar", last modified: Mon Jun  3 06:49:53 2024, max compression
```

## Comparing `dargs-0.4.5.tar` & `dargs-0.4.6.tar`

### file list

```diff
@@ -1,48 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:45:34.000000 dargs-0.4.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:45:34.000000 dargs-0.4.5/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-06 04:45:16.000000 dargs-0.4.5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:45:34.000000 dargs-0.4.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-06 04:45:16.000000 dargs-0.4.5/.github/workflows/mirror_gitee.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-06 04:45:16.000000 dargs-0.4.5/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-06 04:45:16.000000 dargs-0.4.5/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-06 04:45:16.000000 dargs-0.4.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-06 04:45:16.000000 dargs-0.4.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-06 04:45:16.000000 dargs-0.4.5/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-06 04:45:16.000000 dargs-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11040 2024-04-06 04:45:34.000000 dargs-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-06 04:45:16.000000 dargs-0.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-06 04:45:16.000000 dargs-0.4.5/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:45:34.000000 dargs-0.4.5/dargs/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-06 04:45:16.000000 dargs-0.4.5/dargs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-06 04:45:33.000000 dargs-0.4.5/dargs/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    37717 2024-04-06 04:45:16.000000 dargs-0.4.5/dargs/dargs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-04-06 04:45:16.000000 dargs-0.4.5/dargs/notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-04-06 04:45:16.000000 dargs-0.4.5/dargs/sphinx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:45:34.000000 dargs-0.4.5/dargs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11040 2024-04-06 04:45:33.000000 dargs-0.4.5/dargs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-06 04:45:33.000000 dargs-0.4.5/dargs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 04:45:33.000000 dargs-0.4.5/dargs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-06 04:45:33.000000 dargs-0.4.5/dargs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-06 04:45:33.000000 dargs-0.4.5/dargs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:45:34.000000 dargs-0.4.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-06 04:45:16.000000 dargs-0.4.5/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-06 04:45:16.000000 dargs-0.4.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-06 04:45:16.000000 dargs-0.4.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-06 04:45:16.000000 dargs-0.4.5/docs/credits.rst
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-06 04:45:16.000000 dargs-0.4.5/docs/dpgui.rst
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-06 04:45:16.000000 dargs-0.4.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-06 04:45:16.000000 dargs-0.4.5/docs/intro.md
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-06 04:45:16.000000 dargs-0.4.5/docs/nb.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-06 04:45:16.000000 dargs-0.4.5/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-06 04:45:16.000000 dargs-0.4.5/docs/sphinx.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-06 04:45:16.000000 dargs-0.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 04:45:34.000000 dargs-0.4.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:45:34.000000 dargs-0.4.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-06 04:45:16.000000 dargs-0.4.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 04:45:16.000000 dargs-0.4.5/tests/context.py
--rw-r--r--   0 runner    (1001) docker     (127)    38837 2024-04-06 04:45:16.000000 dargs-0.4.5/tests/dpmdargs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11647 2024-04-06 04:45:16.000000 dargs-0.4.5/tests/test_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    10740 2024-04-06 04:45:16.000000 dargs-0.4.5/tests/test_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8613 2024-04-06 04:45:16.000000 dargs-0.4.5/tests/test_docgen.py
--rw-r--r--   0 runner    (1001) docker     (127)     6837 2024-04-06 04:45:16.000000 dargs-0.4.5/tests/test_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-06 04:45:16.000000 dargs-0.4.5/tests/test_notebook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:49:53.000000 dargs-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-06-03 06:49:37.000000 dargs-0.4.6/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-06-03 06:49:37.000000 dargs-0.4.6/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:49:53.000000 dargs-0.4.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-06-03 06:49:37.000000 dargs-0.4.6/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:49:53.000000 dargs-0.4.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-06-03 06:49:37.000000 dargs-0.4.6/.github/workflows/mirror_gitee.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-06-03 06:49:37.000000 dargs-0.4.6/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-06-03 06:49:37.000000 dargs-0.4.6/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-06-03 06:49:37.000000 dargs-0.4.6/.github/workflows/type-check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-06-03 06:49:37.000000 dargs-0.4.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-06-03 06:49:37.000000 dargs-0.4.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-06-03 06:49:37.000000 dargs-0.4.6/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-06-03 06:49:37.000000 dargs-0.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11557 2024-06-03 06:49:53.000000 dargs-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-06-03 06:49:37.000000 dargs-0.4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-06-03 06:49:37.000000 dargs-0.4.6/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:49:53.000000 dargs-0.4.6/dargs/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-06-03 06:49:37.000000 dargs-0.4.6/dargs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-06-03 06:49:53.000000 dargs-0.4.6/dargs/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38165 2024-06-03 06:49:37.000000 dargs-0.4.6/dargs/dargs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-06-03 06:49:37.000000 dargs-0.4.6/dargs/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10200 2024-06-03 06:49:37.000000 dargs-0.4.6/dargs/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 06:49:37.000000 dargs-0.4.6/dargs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6893 2024-06-03 06:49:37.000000 dargs-0.4.6/dargs/sphinx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:49:53.000000 dargs-0.4.6/dargs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11557 2024-06-03 06:49:53.000000 dargs-0.4.6/dargs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-06-03 06:49:53.000000 dargs-0.4.6/dargs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 06:49:53.000000 dargs-0.4.6/dargs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-06-03 06:49:53.000000 dargs-0.4.6/dargs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-03 06:49:53.000000 dargs-0.4.6/dargs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:49:53.000000 dargs-0.4.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-03 06:49:37.000000 dargs-0.4.6/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-06-03 06:49:37.000000 dargs-0.4.6/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-06-03 06:49:37.000000 dargs-0.4.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-06-03 06:49:37.000000 dargs-0.4.6/docs/credits.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-06-03 06:49:37.000000 dargs-0.4.6/docs/dpgui.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-06-03 06:49:37.000000 dargs-0.4.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-06-03 06:49:37.000000 dargs-0.4.6/docs/intro.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-06-03 06:49:37.000000 dargs-0.4.6/docs/json_schema.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-06-03 06:49:37.000000 dargs-0.4.6/docs/nb.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-06-03 06:49:37.000000 dargs-0.4.6/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-06-03 06:49:37.000000 dargs-0.4.6/docs/sphinx.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-06-03 06:49:37.000000 dargs-0.4.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 06:49:53.000000 dargs-0.4.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:49:53.000000 dargs-0.4.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-06-03 06:49:37.000000 dargs-0.4.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 06:49:37.000000 dargs-0.4.6/tests/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39141 2024-06-03 06:49:37.000000 dargs-0.4.6/tests/dpmdargs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11683 2024-06-03 06:49:37.000000 dargs-0.4.6/tests/test_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10776 2024-06-03 06:49:37.000000 dargs-0.4.6/tests/test_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8649 2024-06-03 06:49:37.000000 dargs-0.4.6/tests/test_docgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-06-03 06:49:37.000000 dargs-0.4.6/tests/test_json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6873 2024-06-03 06:49:37.000000 dargs-0.4.6/tests/test_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-06-03 06:49:37.000000 dargs-0.4.6/tests/test_notebook.py
```

### Comparing `dargs-0.4.5/.github/workflows/python-publish.yml` & `dargs-0.4.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `dargs-0.4.5/.github/workflows/test.yml` & `dargs-0.4.6/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `dargs-0.4.5/.gitignore` & `dargs-0.4.6/.gitignore`

 * *Files identical despite different names*

### Comparing `dargs-0.4.5/.pre-commit-config.yaml` & `dargs-0.4.6/.pre-commit-config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
 repos:
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
     -   id: trailing-whitespace
     -   id: end-of-file-fixer
     -   id: check-yaml
     -   id: check-json
     -   id: check-added-large-files
     -   id: check-merge-conflict
     -   id: check-symlinks
     -   id: check-toml
 # Python
 -   repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.5
+    rev: v0.4.5
     hooks:
     - id: ruff
       args: [ --fix ]
     - id: ruff-format
 # numpydoc
 -   repo: https://github.com/Carreau/velin
     rev: 0.0.12
```

### Comparing `dargs-0.4.5/LICENSE` & `dargs-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dargs-0.4.5/PKG-INFO` & `dargs-0.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dargs
-Version: 0.4.5
+Version: 0.4.6
 Summary: Process arguments for the deep modeling project.
 Author: DeepModeling
 Author-email: Yixiao Chen <yixiaoc@princeton.edu>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -174,14 +174,15 @@
 Project-URL: documentation, https://docs.deepmodeling.com/projects/dargs
 Project-URL: repository, https://github.com/deepmodeling/dargs
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
+Provides-Extra: typecheck
 License-File: LICENSE
 
 # Argument checking for python programs
 
 [![conda-forge](https://img.shields.io/conda/dn/conda-forge/dargs?color=red&label=conda-forge&logo=conda-forge)](https://anaconda.org/conda-forge/dargs)
 [![pip install](https://img.shields.io/pypi/dm/dargs?label=pip%20install&logo=pypi)](https://pypi.org/project/dargs)
 [![Documentation Status](https://readthedocs.org/projects/dargs/badge/)](https://dargs.readthedocs.io/)
@@ -202,7 +203,14 @@
 ignore the leading key comparing to the base version.
 
 When targeting to html rendering, additional anchor can be made for cross reference.
 Set `make_anchor=True` when calling `gendoc` function and use standard ref syntax in rst.
 The id is the same as the argument path. Variant types would be in square brackets.
 
 Please refer to test files for detailed usage.
+
+## Additional features
+
+- [PEP 484](https://peps.python.org/pep-0484/) type annotations
+- Native integration with [Sphinx](https://github.com/sphinx-doc/sphinx), [DP-GUI](https://github.com/deepmodeling/dpgui), and [Jupyter Notebook](https://jupyter.org/)
+- JSON encoder for `Argument` and `Variant` classes
+- Generate [JSON schema](https://json-schema.org/) from an `Argument`, which can be further integrated with JSON editors such as [Visual Studio Code](https://code.visualstudio.com/)
```

### Comparing `dargs-0.4.5/README.md` & `dargs-0.4.6/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -20,7 +20,14 @@
 ignore the leading key comparing to the base version.
 
 When targeting to html rendering, additional anchor can be made for cross reference.
 Set `make_anchor=True` when calling `gendoc` function and use standard ref syntax in rst.
 The id is the same as the argument path. Variant types would be in square brackets.
 
 Please refer to test files for detailed usage.
+
+## Additional features
+
+- [PEP 484](https://peps.python.org/pep-0484/) type annotations
+- Native integration with [Sphinx](https://github.com/sphinx-doc/sphinx), [DP-GUI](https://github.com/deepmodeling/dpgui), and [Jupyter Notebook](https://jupyter.org/)
+- JSON encoder for `Argument` and `Variant` classes
+- Generate [JSON schema](https://json-schema.org/) from an `Argument`, which can be further integrated with JSON editors such as [Visual Studio Code](https://code.visualstudio.com/)
```

### Comparing `dargs-0.4.5/dargs/dargs.py` & `dargs-0.4.6/dargs/dargs.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,22 +12,24 @@
 `sub_variants` to mimic the union behavior in the type structure.
 
 Due to the complexity of *Variant* structure, it is implemented into a
 separate class `Variant` so that multiple choices can be handled correctly.
 We also need to pay special attention to flat the keys of its choices.
 """
 
+from __future__ import annotations
+
 import difflib
 import fnmatch
 import json
 import re
 from copy import deepcopy
 from enum import Enum
 from textwrap import indent
-from typing import Any, Callable, Dict, Iterable, List, Optional, Union
+from typing import Any, Callable, Iterable, List
 
 try:
     from typing import get_origin
 except ImportError:
     from typing_extensions import get_origin
 
 import typeguard
@@ -50,17 +52,15 @@
     NONE = 0  # for no value in dict (when optional)
     EMPTY_DICT = 1  # for empty dict as default value
 
 
 class ArgumentError(Exception):
     """Base error class for invalid argument values in argchecking."""
 
-    def __init__(
-        self, path: Union[None, str, List[str]] = None, message: Optional[str] = None
-    ):
+    def __init__(self, path: None | str | list[str] = None, message: str | None = None):
         super().__init__(message)
         if path is None:
             path = ""
         if not isinstance(path, str):
             path = "/".join(path)
         self.path = path.strip("/")
         self.message = message
@@ -135,45 +135,47 @@
 
     for more detailed examples, please check the unit tests.
     """
 
     def __init__(
         self,
         name: str,
-        dtype: Union[None, type, Iterable[type]],
-        sub_fields: Optional[Iterable["Argument"]] = None,
-        sub_variants: Optional[Iterable["Variant"]] = None,
+        dtype: None | type | Iterable[type | Any | None],
+        sub_fields: Iterable[Argument] | None = None,
+        sub_variants: Iterable[Variant] | None = None,
         repeat: bool = False,
         optional: bool = False,
         default: Any = _Flags.NONE,
-        alias: Optional[Iterable[str]] = None,
-        extra_check: Optional[Callable[[Any], bool]] = None,
+        alias: Iterable[str] | None = None,
+        extra_check: Callable[[Any], bool] | None = None,
         doc: str = "",
         fold_subdoc: bool = False,
         extra_check_errmsg: str = "",
     ):
         self.name = name
-        self.dtype = dtype
-        self.sub_fields: Dict[str, "Argument"] = {}
-        self.sub_variants: Dict[str, "Variant"] = {}
+        self.sub_fields: dict[str, Argument] = {}
+        self.sub_variants: dict[str, Variant] = {}
         self.repeat = repeat
         self.optional = optional
         self.default = default
-        self.alias = alias if alias is not None else []
+        self.alias = tuple(alias) if alias is not None else []
         self.extra_check = extra_check
         self.doc = doc
         self.fold_subdoc = fold_subdoc
         self.extra_check_errmsg = extra_check_errmsg
+        # handle the format of dtype, makeit a tuple
+        self.dtype = self._reorg_dtype(dtype)
         # adding subfields and subvariants
         self.extend_subfields(sub_fields)
         self.extend_subvariants(sub_variants)
-        # handle the format of dtype, makeit a tuple
-        self._reorg_dtype()
 
-    def __eq__(self, other: "Argument") -> bool:
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, Argument):
+            return NotImplemented
+
         # do not compare doc and default
         # since they do not enter to the type checking
         def fkey(f):
             return f.name
 
         def vkey(v):
             return v.flag_name
@@ -186,15 +188,15 @@
             and self.repeat == other.repeat
             and self.optional == other.optional
         )
 
     def __repr__(self) -> str:
         return f"<Argument {self.name}: {' | '.join(self._get_type_name(dd) for dd in self.dtype)}>"
 
-    def __getitem__(self, key: str) -> "Argument":
+    def __getitem__(self, key: str) -> Argument:
         key = key.lstrip("/")
         if key in ("", "."):
             return self
         if key.startswith("["):
             vkey, rkey = key[1:].split("]", 1)
             if vkey.count("=") == 1:
                 fkey, ckey = vkey.split("=")
@@ -212,97 +214,97 @@
 
     @property
     def I(self):  # noqa:E743
         # return a dummy argument that only has self as a sub field
         # can be used in indexing
         return Argument("_", dict, [self])
 
-    def _reorg_dtype(self):
+    def _reorg_dtype(
+        self, dtype: None | type | Any | Iterable[type | Any | None]
+    ) -> tuple[type | Any | None, ...]:
         if (
-            isinstance(self.dtype, type)
-            or isinstance(get_origin(self.dtype), type)
-            or self.dtype is None
+            isinstance(dtype, type)
+            or isinstance(get_origin(dtype), type)
+            or dtype is None
         ):
-            self.dtype = [self.dtype]
+            dtype = [dtype]
+        assert dtype is not None
         # remove duplicate
-        self.dtype = {
+        dtype = {
             dt if type(dt) is type or type(get_origin(dt)) is type else type(dt)
-            for dt in self.dtype
+            for dt in dtype
         }
         # check conner cases
         if self.sub_fields or self.sub_variants:
-            self.dtype.add(list if self.repeat else dict)
+            dtype.add(list if self.repeat else dict)
         if (
             self.optional
             and self.default is not _Flags.NONE
-            and all(not isinstance_annotation(self.default, tt) for tt in self.dtype)
+            and all(not isinstance_annotation(self.default, tt) for tt in dtype)
         ):
-            self.dtype.add(type(self.default))
+            dtype.add(type(self.default))
         # and make it compatible with `isinstance`
-        self.dtype = tuple(self.dtype)
+        return tuple(dtype)
 
-    def set_dtype(self, dtype: Union[None, type, Iterable[type]]):
+    def set_dtype(self, dtype: None | type | Iterable[type]):
         """Change the dtype of the current Argument."""
-        self.dtype = dtype
-        self._reorg_dtype()
+        self.dtype = self._reorg_dtype(dtype)
 
     def set_repeat(self, repeat: bool = True):
         """Change the repeat attribute of the current Argument."""
         self.repeat = repeat
-        self._reorg_dtype()
+        self.dtype = self._reorg_dtype(self.dtype)
 
-    def extend_subfields(self, sub_fields: Optional[Iterable["Argument"]]):
+    def extend_subfields(self, sub_fields: Iterable[Argument] | None):
         """Add a list of sub fields to the current Argument."""
         if sub_fields is None:
             return
         assert all(isinstance(s, Argument) for s in sub_fields)
         update_nodup(
             self.sub_fields,
             ((s.name, s) for s in sub_fields),
             err_msg=f"building Argument `{self.name}`",
         )
-        self._reorg_dtype()
+        self.dtype = self._reorg_dtype(self.dtype)
 
-    def add_subfield(self, name: Union[str, "Argument"], *args, **kwargs) -> "Argument":
+    def add_subfield(self, name: str | Argument, *args, **kwargs) -> Argument:
         """Add a sub field to the current Argument."""
         if isinstance(name, Argument):
             newarg = name
         else:
             newarg = Argument(name, *args, **kwargs)
         self.extend_subfields([newarg])
         return newarg
 
-    def extend_subvariants(self, sub_variants: Optional[Iterable["Variant"]]):
+    def extend_subvariants(self, sub_variants: Iterable[Variant] | None):
         """Add a list of sub variants to the current Argument."""
         if sub_variants is None:
             return
         assert all(isinstance(s, Variant) for s in sub_variants)
         update_nodup(
             self.sub_variants,
             ((s.flag_name, s) for s in sub_variants),
             exclude=self.sub_fields.keys(),
             err_msg=f"building Argument `{self.name}`",
         )
-        self._reorg_dtype()
+        self.dtype = self._reorg_dtype(self.dtype)
 
-    def add_subvariant(
-        self, flag_name: Union[str, "Variant"], *args, **kwargs
-    ) -> "Variant":
+    def add_subvariant(self, flag_name: str | Variant, *args, **kwargs) -> Variant:
         """Add a sub variant to the current Argument."""
         if isinstance(flag_name, Variant):
             newvrnt = flag_name
         else:
             newvrnt = Variant(flag_name, *args, **kwargs)
         self.extend_subvariants([newvrnt])
         return newvrnt
 
     # above are creation part
     # below are general traverse part
 
-    def flatten_sub(self, value: dict, path=None) -> Dict[str, "Argument"]:
+    def flatten_sub(self, value: dict, path=None) -> dict[str, Argument]:
         sub_dicts = [self.sub_fields]
         sub_dicts.extend(
             vrnt.flatten_sub(value, path) for vrnt in self.sub_variants.values()
         )
         flat_subs = {}
         update_nodup(
             flat_subs, *sub_dicts, err_msg=f"flattening variants of {self.name}"
@@ -312,15 +314,15 @@
     def traverse(
         self,
         argdict: dict,
         key_hook: HookArgKType = _DUMMYHOOK,
         value_hook: HookArgVType = _DUMMYHOOK,
         sub_hook: HookArgKType = _DUMMYHOOK,
         variant_hook: HookVrntType = _DUMMYHOOK,
-        path: Optional[List[str]] = None,
+        path: list[str] | None = None,
     ):
         # first, do something with the key
         # then, take out the vaule and do something with it
         if path is None:
             path = []
         key_hook(self, argdict, path)
         if self.name in argdict:
@@ -335,15 +337,15 @@
     def traverse_value(
         self,
         value: Any,
         key_hook: HookArgKType = _DUMMYHOOK,
         value_hook: HookArgVType = _DUMMYHOOK,
         sub_hook: HookArgKType = _DUMMYHOOK,
         variant_hook: HookVrntType = _DUMMYHOOK,
-        path: Optional[List[str]] = None,
+        path: list[str] | None = None,
     ):
         # this is not private, and can be called directly
         # in the condition where there is no leading key
         if path is None:
             path = []
         if isinstance(value, dict):
             self._traverse_sub(
@@ -363,15 +365,15 @@
     def _traverse_sub(
         self,
         value: dict,
         key_hook: HookArgKType = _DUMMYHOOK,
         value_hook: HookArgVType = _DUMMYHOOK,
         sub_hook: HookArgKType = _DUMMYHOOK,
         variant_hook: HookVrntType = _DUMMYHOOK,
-        path: Optional[List[str]] = None,
+        path: list[str] | None = None,
     ):
         assert isinstance(value, dict)
         if path is None:
             path = [self.name]
         sub_hook(self, value, path)
         for subvrnt in self.sub_variants.values():
             variant_hook(subvrnt, value, path)
@@ -454,19 +456,23 @@
             raise ArgumentValueError(
                 path,
                 f"key `{self.name}` gets bad value "
                 "that fails to pass its extra checking. " + self.extra_check_errmsg,
             )
 
     def _check_strict(self, value: dict, path=None):
-        allowed_keys = self.flatten_sub(value, path).keys()
+        allowed_keys = set(self.flatten_sub(value, path).keys())
         # curpath = [*path, self.name]
         if not len(allowed_keys):
             # no allowed keys defined, allow any keys
             return
+        # A special case to allow $schema in any dict to be compatible with vscode + json schema
+        # https://code.visualstudio.com/docs/languages/json#_mapping-in-the-json
+        # considering usually it's not a typo of users when they use $schema
+        allowed_keys.add("$schema")
         for name in value.keys():
             if name not in allowed_keys:
                 dym_message = did_you_mean(name, allowed_keys)
                 raise ArgumentKeyError(
                     path,
                     f"undefined key `{name}` is not allowed in strict mode. {dym_message}",
                 )
@@ -476,15 +482,15 @@
 
     def normalize(
         self,
         argdict: dict,
         inplace: bool = False,
         do_default: bool = True,
         do_alias: bool = True,
-        trim_pattern: Optional[str] = None,
+        trim_pattern: str | None = None,
     ):
         """Modify `argdict` so that it meets the Argument structure.
 
         Normalization can add default values to optional args,
         substitute alias by its standard names, and discard unnecessary
         args following given pattern.
 
@@ -529,15 +535,15 @@
 
     def normalize_value(
         self,
         value: Any,
         inplace: bool = False,
         do_default: bool = True,
         do_alias: bool = True,
-        trim_pattern: Optional[str] = None,
+        trim_pattern: str | None = None,
     ):
         """Modify the value so that it meets the Argument structure.
 
         Same as `normalize({self.name: value})[self.name]`.
 
         Parameters
         ----------
@@ -596,55 +602,56 @@
                 if alias in argdict:
                     argdict[self.name] = argdict.pop(alias)
                     return
 
     # above are normalizing part
     # below are doc generation part
 
-    def gen_doc(self, path: Optional[List[str]] = None, **kwargs) -> str:
+    def gen_doc(self, path: list[str] | None = None, **kwargs) -> str:
         """Generate doc string for the current Argument."""
         # the actual indentation is done here, and ONLY here
         if path is None:
             path = []
         sub_paths = [*path, self.name]
         doc_list = [
             self.gen_doc_head(sub_paths, **kwargs),
             indent(self.gen_doc_path(sub_paths, **kwargs), INDENT),
             indent(self.gen_doc_body(sub_paths, **kwargs), INDENT),
         ]
         return "\n".join(filter(None, doc_list))
 
-    def gen_doc_head(self, path: Optional[List[str]] = None, **kwargs) -> str:
+    def gen_doc_head(self, path: list[str] | None = None, **kwargs) -> str:
         typesig = "| type: " + " | ".join(
             [f"``{self._get_type_name(dt)}``" for dt in self.dtype]
         )
         if self.optional:
             typesig += ", optional"
             if self.default == "":
                 typesig += ", default: (empty string)"
             elif self.default is not _Flags.NONE:
                 typesig += f", default: ``{self.default}``"
         if self.alias:
             typesig += f", alias{'es' if len(self.alias) > 1 else ''}: "
             typesig += ", ".join(f"*{al}*" for al in self.alias)
         head = f"{self.name}: "
         if kwargs.get("use_sphinx_domain", False):
+            assert path is not None
             head = f".. dargs:argument:: {self.name}:\n   :path: {'/'.join(path)}\n"
         head += f"\n{indent(typesig, INDENT)}"
         if kwargs.get("make_anchor"):
             head = f"{make_rst_refid(path)}\n" + head
         return head
 
-    def gen_doc_path(self, path: Optional[List[str]] = None, **kwargs) -> str:
+    def gen_doc_path(self, path: list[str] | None = None, **kwargs) -> str:
         if path is None:
             path = [self.name]
         pathdoc = f"| argument path: ``{'/'.join(path)}``\n"
         return pathdoc
 
-    def gen_doc_body(self, path: Optional[List[str]] = None, **kwargs) -> str:
+    def gen_doc_body(self, path: list[str] | None = None, **kwargs) -> str:
         body_list = []
         if self.doc:
             body_list.append(self.doc + "\n")
         if not self.fold_subdoc:
             if self.repeat:
                 body_list.append(
                     "This argument takes a list with "
@@ -694,58 +701,60 @@
     -----
     This class should only be used in sub variants of the `Argument` class.
     """
 
     def __init__(
         self,
         flag_name: str,
-        choices: Optional[Iterable["Argument"]] = None,
+        choices: Iterable[Argument] | None = None,
         optional: bool = False,
         default_tag: str = "",  # this is indeed necessary in case of optional
         doc: str = "",
     ):
         self.flag_name = flag_name
-        self.choice_dict: Dict[str, Argument] = {}
-        self.choice_alias: Dict[str, str] = {}
+        self.choice_dict: dict[str, Argument] = {}
+        self.choice_alias: dict[str, str] = {}
         self.extend_choices(choices)
         self.optional = optional
         if optional and not default_tag:
             raise ValueError("default_tag is needed if optional is set to be True")
         self.set_default(default_tag)
         self.doc = doc
 
-    def __eq__(self, other: "Variant") -> bool:
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, Variant):
+            return NotImplemented
         # do not compare doc
         return (
             self.flag_name == other.flag_name
             and self.choice_dict == other.choice_dict
             and self.optional == other.optional
             and self.default_tag == other.default_tag
         )
 
     def __repr__(self) -> str:
         return (
             f"<Variant {self.flag_name} in {{ {', '.join(self.choice_dict.keys())} }}>"
         )
 
-    def __getitem__(self, key: str) -> "Argument":
+    def __getitem__(self, key: str) -> Argument:
         return self.choice_dict[key]
 
-    def set_default(self, default_tag: Union[bool, str]):
+    def set_default(self, default_tag: bool | str):
         """Change the default tag of the current Variant."""
         if not default_tag:
             self.optional = False
             self.default_tag = ""
         else:
             if default_tag not in self.choice_dict:
                 raise ValueError(f"trying to set invalid default_tag `{default_tag}`")
             self.optional = True
             self.default_tag = default_tag
 
-    def extend_choices(self, choices: Optional[Iterable["Argument"]]):
+    def extend_choices(self, choices: Iterable[Argument] | None):
         """Add a list of choice Arguments to the current Variant."""
         # choices is a list of arguments
         # whose name is treated as the switch tag
         # we convert it into a dict for better reference
         # and avoid duplicate tags
         if choices is None:
             return
@@ -760,19 +769,19 @@
             *[[(a, c.name) for a in c.alias] for c in choices],
             exclude={self.flag_name, *self.choice_dict.keys()},
             err_msg=f"building alias dict for Variant with flag `{self.flag_name}`",
         )
 
     def add_choice(
         self,
-        tag: Union[str, "Argument"],
-        _dtype: Union[None, type, Iterable[type]] = dict,
+        tag: str | Argument,
+        _dtype: None | type | Iterable[type] = dict,
         *args,
         **kwargs,
-    ) -> "Argument":
+    ) -> Argument:
         """Add a choice Argument to the current Variant."""
         if isinstance(tag, Argument):
             newarg = tag
         else:
             newarg = Argument(tag, _dtype, *args, **kwargs)
         self.extend_choices([newarg])
         return newarg
@@ -790,15 +799,15 @@
             extra_check=None,
             doc=f"dummy Argument converted from Variant {self.flag_name}",
         )
 
     # above are creation part
     # below are helpers for traversing
 
-    def get_choice(self, argdict: dict, path=None) -> "Argument":
+    def get_choice(self, argdict: dict, path=None) -> Argument:
         if self.flag_name in argdict:
             tag = argdict[self.flag_name]
             if tag in self.choice_dict:
                 return self.choice_dict[tag]
             elif tag in self.choice_alias:
                 return self.choice_dict[self.choice_alias[tag]]
             else:
@@ -815,15 +824,15 @@
         else:
             raise ArgumentKeyError(
                 path,
                 f"key `{self.flag_name}` is required "
                 "to choose variant but not found.",
             )
 
-    def flatten_sub(self, argdict: dict, path=None) -> Dict[str, "Argument"]:
+    def flatten_sub(self, argdict: dict, path=None) -> dict[str, Argument]:
         choice = self.get_choice(argdict, path)
         fields = {
             self.flag_name: self.dummy_argument(),  # as a placeholder
             **choice.flatten_sub(argdict, path),
         }
         return fields
 
@@ -833,24 +842,25 @@
             if tag not in self.choice_dict and tag in self.choice_alias:
                 argdict[self.flag_name] = self.choice_alias[tag]
 
     # above are traversing part
     # below are doc generation part
 
     def gen_doc(
-        self, path: Optional[List[str]] = None, showflag: bool = False, **kwargs
+        self, path: list[str] | None = None, showflag: bool = False, **kwargs
     ) -> str:
         body_list = [""]
         body_list.append(
             f"Depending on the value of *{self.flag_name}*, "
             "different sub args are accepted. \n"
         )
         body_list.append(self.gen_doc_flag(path, showflag=showflag, **kwargs))
         fnstr = f"*{self.flag_name}*"
         if kwargs.get("make_link"):
+            assert path is not None
             if not kwargs.get("make_anchor"):
                 raise ValueError("`make_link` only works with `make_anchor` set")
             fnstr, target = make_ref_pair([*path, self.flag_name], fnstr, "flag")
             body_list.append(target + "\n")
         for choice in self.choice_dict.values():
             body_list.append("")
             choice_path = self._make_cpath(choice.name, path, showflag)
@@ -868,15 +878,15 @@
                     f"When {fnstr} is set to ``{choice.name}``{c_alias}: \n",
                     choice.gen_doc_body(choice_path, **kwargs),
                 ]
             )
         body = "\n".join(body_list)
         return body
 
-    def gen_doc_flag(self, path: Optional[List[str]] = None, **kwargs) -> str:
+    def gen_doc_flag(self, path: list[str] | None = None, **kwargs) -> str:
         headdoc = f"{self.flag_name}:"
         typedoc = "| type: ``str`` (flag key)"
         if self.optional:
             typedoc += f", default: ``{self.default_tag}``"
         typedoc = indent(typedoc, INDENT)
         if path is None:
             path = []
@@ -913,15 +923,15 @@
             "",
             realdoc,
             targetdoc,
         ]
         return "\n".join([x for x in allparts if x is not None])
 
     def _make_cpath(
-        self, cname: str, path: Optional[List[str]] = None, showflag: bool = False
+        self, cname: str, path: list[str] | None = None, showflag: bool = False
     ):
         f_str = f"{self.flag_name}=" if showflag else ""
         c_str = f"[{f_str}{cname}]"
         cpath = [*path[:-1], path[-1] + c_str] if path else [c_str]
         return cpath
 
 
@@ -945,17 +955,17 @@
     if text:
         target = f".. |{ref}| replace:: {text}\n" + target
     return inline, target
 
 
 def update_nodup(
     this: dict,
-    *others: Union[dict, Iterable[tuple]],
-    exclude: Optional[Iterable] = None,
-    err_msg: Optional[str] = None,
+    *others: dict | Iterable[tuple],
+    exclude: Iterable | None = None,
+    err_msg: str | None = None,
 ):
     for pair in others:
         if isinstance(pair, dict):
             pair = pair.items()
         for k, v in pair:
             if k in this or (exclude and k in exclude):
                 raise ValueError(
@@ -965,15 +975,15 @@
             this[k] = v
     return this
 
 
 def trim_by_pattern(
     argdict: dict,
     pattern: str,
-    reserved: Optional[List[str]] = None,
+    reserved: Iterable[str] | None = None,
     use_regex: bool = False,
 ):
     rep = fnmatch.translate(pattern) if not use_regex else pattern
     rem = re.compile(rep)
     if reserved:
         conflict = list(filter(rem.match, reserved))
         if conflict:
@@ -1003,60 +1013,60 @@
     """Extended JSON Encoder to encode Argument object.
 
     Examples
     --------
     >>> json.dumps(some_arg, cls=ArgumentEncoder)
     """
 
-    def default(self, obj) -> Dict[str, Union[str, bool, List]]:
+    def default(self, o) -> Any:
         """Generate a dict containing argument information, making it ready to be encoded
         to JSON string.
 
         Notes
         -----
         All object in the dict should be JSON serializable.
 
         Returns
         -------
-        dict: Dict
-            a dict containing argument information
+        Any
+            any; for Argument and Variant, returns a dict containing argument information
         """
-        if isinstance(obj, Argument):
+        if isinstance(o, Argument):
             output = {
                 "object": "Argument",
-                "name": obj.name,
-                "type": obj.dtype,
-                "optional": obj.optional,
-                "alias": obj.alias,
-                "doc": obj.doc,
-                "repeat": obj.repeat,
-                "sub_fields": obj.sub_fields,
-                "sub_variants": obj.sub_variants,
+                "name": o.name,
+                "type": o.dtype,
+                "optional": o.optional,
+                "alias": o.alias,
+                "doc": o.doc,
+                "repeat": o.repeat,
+                "sub_fields": o.sub_fields,
+                "sub_variants": o.sub_variants,
             }
-            if obj.optional and obj.default is not _Flags.NONE:
-                output["default"] = obj.default
+            if o.optional and o.default is not _Flags.NONE:
+                output["default"] = o.default
             return output
-        elif isinstance(obj, Variant):
+        elif isinstance(o, Variant):
             return {
                 "object": "Variant",
-                "flag_name": obj.flag_name,
-                "optional": obj.optional,
-                "default_tag": obj.default_tag,
-                "choice_dict": obj.choice_dict,
-                "choice_alias": obj.choice_alias,
-                "doc": obj.doc,
+                "flag_name": o.flag_name,
+                "optional": o.optional,
+                "default_tag": o.default_tag,
+                "choice_dict": o.choice_dict,
+                "choice_alias": o.choice_alias,
+                "doc": o.doc,
             }
-        elif isinstance(get_origin(obj), type):
-            return get_origin(obj).__name__
-        elif isinstance(obj, type):
-            return obj.__name__
-        return json.JSONEncoder.default(self, obj)
+        elif isinstance(get_origin(o), type):
+            return get_origin(o).__name__
+        elif isinstance(o, type):
+            return o.__name__
+        return json.JSONEncoder.default(self, o)
 
 
-def did_you_mean(choice: str, choices: List[str]) -> str:
+def did_you_mean(choice: str, choices: Iterable[str]) -> str:
     """Get did you mean message.
 
     Parameters
     ----------
     choice : str
         the user's wrong choice
     choices : list[str]
```

### Comparing `dargs-0.4.5/dargs/notebook.py` & `dargs-0.4.6/dargs/notebook.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,17 +13,19 @@
 ...     "test_variant": "test_variant_argument",
 ...     "_comment": "This is an example data"
 ... }
 ... """
 >>> JSON(jstr, _test_argument())
 '''
 
+from __future__ import annotations
+
 import json
 import re
-from typing import List, Union
+from typing import Any
 
 from IPython.display import HTML, display
 
 from dargs import Argument, Variant
 
 __all__ = ["JSON"]
 
@@ -83,28 +85,28 @@
 .dargs-codeblock .dargs-key .dargs-doc .dargs-doc-code {
   color: #bbbbff;
 }
 </style>
 """
 
 
-def JSON(data: Union[dict, str], arg: Union[Argument, List[Argument]]):
+def JSON(data: dict | str, arg: Argument | list[Argument]):
     """Display JSON data with Argument in the Jupyter Notebook.
 
     Parameters
     ----------
     data : dict or str
         The JSON data to be displayed, either JSON string or a dict.
     arg : dargs.Argument or list[dargs.Argument]
         The Argument that describes the JSON data.
     """
     display(HTML(print_html(data, arg)))
 
 
-def print_html(data: Union[dict, str], arg: Union[Argument, List[Argument]]) -> str:
+def print_html(data: Any, arg: Argument | list[Argument]) -> str:
     """Print HTML string with Argument in the Jupyter Notebook.
 
     Parameters
     ----------
     data : dict or str
         The JSON data to be displayed, either JSON string or a dict.
     arg : dargs.Argument or list[dargs.Argument]
@@ -138,19 +140,19 @@
 
     It is used to print the data with Argument in the Jupyter Notebook.
 
     Parameters
     ----------
     data : dict
         The data to be displayed.
-    arg : dargs.Argument
+    arg : Union[dargs.Argument, dargs.Variant]
         The Argument that describes the data.
     """
 
-    def __init__(self, data: dict, arg: Argument):
+    def __init__(self, data: dict, arg: Argument | Variant):
         self.data = data
         self.arg = arg
         self.subdata = []
         self._init_subdata()
 
     def _init_subdata(self):
         """Initialize sub ArgumentData."""
```

### Comparing `dargs-0.4.5/dargs/sphinx.py` & `dargs-0.4.6/dargs/sphinx.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,33 +16,38 @@
     .. dargs::
        :module: dargs.sphinx
        :func: _test_argument
 
 where `_test_argument` returns an :class:`Argument <dargs.Argument>`. A :class:`list` of :class:`Argument <dargs.Argument>` is also accepted.
 """
 
+from __future__ import annotations
+
 import sys
-from typing import ClassVar, List
+from typing import TYPE_CHECKING, Any, Callable, ClassVar, List
 
 from docutils.parsers.rst import Directive
 from docutils.parsers.rst.directives import unchanged
 from sphinx import addnodes
 from sphinx.directives import ObjectDescription
 from sphinx.domains import Domain, ObjType
 from sphinx.roles import XRefRole
 from sphinx.util.nodes import make_refnode
 
 from .dargs import Argument, Variant
 
+if TYPE_CHECKING:
+    from sphinx.util.typing import RoleFunction
+
 
 class DargsDirective(Directive):
     """dargs directive."""
 
     has_content: ClassVar[bool] = True
-    option_spec: ClassVar[dict] = {
+    option_spec: ClassVar[dict[str, Callable[[str], Any]] | None] = {
         "module": unchanged,
         "func": unchanged,
     }
 
     def run(self):
         if "module" in self.options and "func" in self.options:
             module_name = self.options["module"]
@@ -128,25 +133,25 @@
     Includes:
     - dargs::argument directive
     - dargs::argument role
     """
 
     name: ClassVar[str] = "dargs"
     label: ClassVar[str] = "dargs"
-    object_types: ClassVar[dict] = {
+    object_types: ClassVar[dict[str, ObjType]] = {  # type: ignore
         "argument": ObjType("argument", "argument"),
     }
-    directives: ClassVar[dict] = {
+    directives: ClassVar[dict[str, type[Directive]]] = {  # type: ignore
         "argument": DargsObject,
     }
-    roles: ClassVar[dict] = {
+    roles: ClassVar[dict[str, RoleFunction | XRefRole]] = {  # type: ignore
         "argument": XRefRole(),
     }
 
-    initial_data: ClassVar[dict] = {
+    initial_data: ClassVar[dict] = {  # type: ignore
         "arguments": {},  # fullname -> docname, objtype
     }
 
     def resolve_xref(self, env, fromdocname, builder, typ, target, node, contnode):
         """Resolve cross-references."""
         targetid = f"{typ}:{target}"
         obj = self.data["arguments"].get(targetid)
@@ -199,15 +204,15 @@
                     ),
                 ],
             ),
         ],
     )
 
 
-def _test_arguments() -> List[Argument]:
+def _test_arguments() -> list[Argument]:
     """Returns a list of arguments."""
     return [
         Argument(name="test1", dtype=int, doc="Argument 1"),
         Argument(name="test2", dtype=[float, None], doc="Argument 2"),
         Argument(
             name="test3",
             dtype=List[str],
```

### Comparing `dargs-0.4.5/dargs.egg-info/PKG-INFO` & `dargs-0.4.6/dargs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dargs
-Version: 0.4.5
+Version: 0.4.6
 Summary: Process arguments for the deep modeling project.
 Author: DeepModeling
 Author-email: Yixiao Chen <yixiaoc@princeton.edu>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -174,14 +174,15 @@
 Project-URL: documentation, https://docs.deepmodeling.com/projects/dargs
 Project-URL: repository, https://github.com/deepmodeling/dargs
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
+Provides-Extra: typecheck
 License-File: LICENSE
 
 # Argument checking for python programs
 
 [![conda-forge](https://img.shields.io/conda/dn/conda-forge/dargs?color=red&label=conda-forge&logo=conda-forge)](https://anaconda.org/conda-forge/dargs)
 [![pip install](https://img.shields.io/pypi/dm/dargs?label=pip%20install&logo=pypi)](https://pypi.org/project/dargs)
 [![Documentation Status](https://readthedocs.org/projects/dargs/badge/)](https://dargs.readthedocs.io/)
@@ -202,7 +203,14 @@
 ignore the leading key comparing to the base version.
 
 When targeting to html rendering, additional anchor can be made for cross reference.
 Set `make_anchor=True` when calling `gendoc` function and use standard ref syntax in rst.
 The id is the same as the argument path. Variant types would be in square brackets.
 
 Please refer to test files for detailed usage.
+
+## Additional features
+
+- [PEP 484](https://peps.python.org/pep-0484/) type annotations
+- Native integration with [Sphinx](https://github.com/sphinx-doc/sphinx), [DP-GUI](https://github.com/deepmodeling/dpgui), and [Jupyter Notebook](https://jupyter.org/)
+- JSON encoder for `Argument` and `Variant` classes
+- Generate [JSON schema](https://json-schema.org/) from an `Argument`, which can be further integrated with JSON editors such as [Visual Studio Code](https://code.visualstudio.com/)
```

### Comparing `dargs-0.4.5/dargs.egg-info/SOURCES.txt` & `dargs-0.4.6/dargs.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,46 @@
+.git_archival.txt
+.gitattributes
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yaml
 LICENSE
 README.md
 codecov.yml
 pyproject.toml
 .github/dependabot.yml
 .github/workflows/mirror_gitee.yml
 .github/workflows/python-publish.yml
 .github/workflows/test.yml
+.github/workflows/type-check.yml
 dargs/__init__.py
 dargs/_version.py
 dargs/dargs.py
+dargs/json_schema.py
 dargs/notebook.py
+dargs/py.typed
 dargs/sphinx.py
 dargs.egg-info/PKG-INFO
 dargs.egg-info/SOURCES.txt
 dargs.egg-info/dependency_links.txt
 dargs.egg-info/requires.txt
 dargs.egg-info/top_level.txt
 docs/.gitignore
 docs/Makefile
 docs/conf.py
 docs/credits.rst
 docs/dpgui.rst
 docs/index.rst
 docs/intro.md
+docs/json_schema.md
 docs/nb.ipynb
 docs/requirements.txt
 docs/sphinx.rst
 tests/__init__.py
 tests/context.py
 tests/dpmdargs.py
 tests/test_checker.py
 tests/test_creation.py
 tests/test_docgen.py
+tests/test_json_schema.py
 tests/test_normalizer.py
 tests/test_notebook.py
```

### Comparing `dargs-0.4.5/docs/Makefile` & `dargs-0.4.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dargs-0.4.5/docs/conf.py` & `dargs-0.4.6/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 # -- Path setup --------------------------------------------------------------
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
+from __future__ import annotations
+
 import os
 import sys
 from datetime import date
 
 sys.path.insert(0, os.path.abspath(".."))
```

### Comparing `dargs-0.4.5/docs/dpgui.rst` & `dargs-0.4.6/docs/dpgui.rst`

 * *Files identical despite different names*

### Comparing `dargs-0.4.5/docs/intro.md` & `dargs-0.4.6/docs/intro.md`

 * *Files 27% similar despite different names*

```diff
@@ -20,7 +20,14 @@
 ignore the leading key comparing to the base version.
 
 When targeting to html rendering, additional anchor can be made for cross reference.
 Set `make_anchor=True` when calling `gendoc` function and use standard ref syntax in rst.
 The id is the same as the argument path. Variant types would be in square brackets.
 
 Please refer to test files for detailed usage.
+
+## Additional features
+
+- [PEP 484](https://peps.python.org/pep-0484/) type annotations
+- Native integration with [Sphinx](https://github.com/sphinx-doc/sphinx), [DP-GUI](https://github.com/deepmodeling/dpgui), and [Jupyter Notebook](https://jupyter.org/)
+- JSON encoder for `Argument` and `Variant` classes
+- Generate [JSON schema](https://json-schema.org/) from an `Argument`, which can be further integrated with JSON editors such as [Visual Studio Code](https://code.visualstudio.com/)
```

### Comparing `dargs-0.4.5/docs/nb.ipynb` & `dargs-0.4.6/docs/nb.ipynb`

 * *Files identical despite different names*

### Comparing `dargs-0.4.5/docs/sphinx.rst` & `dargs-0.4.6/docs/sphinx.rst`

 * *Files identical despite different names*

### Comparing `dargs-0.4.5/pyproject.toml` & `dargs-0.4.6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools>=61", "setuptools_scm[toml]>=6.2"]
+requires = ["setuptools>=61", "setuptools_scm[toml]>=7"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dargs"
 dynamic = ["version"]
 description = "Process arguments for the deep modeling project."
 authors = [
@@ -26,14 +26,20 @@
 Homepage = "https://github.com/deepmodeling/dargs"
 documentation = "https://docs.deepmodeling.com/projects/dargs"
 repository = "https://github.com/deepmodeling/dargs"
 
 [project.optional-dependencies]
 test = [
     "ipython",
+    "jsonschema",
+]
+typecheck = [
+    "basedpyright==1.12.2",
+    "sphinx",
+    "ipython",
 ]
 
 [tool.setuptools.packages.find]
 include = ["dargs*"]
 
 [tool.setuptools_scm]
 write_to = "dargs/_version.py"
@@ -43,14 +49,15 @@
     "E", # errors
     "F", # pyflakes
     "D", # pydocstyle
     "UP", # pyupgrade
     "C4", # flake8-comprehensions
     "RUF", # ruff
     "I", # isort
+    "TCH", # flake8-type-checking
 ]
 
 ignore = [
     "E501", # line too long
     "F841", # local variable is assigned to but never used
     "E741", # ambiguous variable name
     "E402", # module level import not at top of file
@@ -64,7 +71,13 @@
     "D401", # TODO: first line should be in imperative mood
     "D404", # TODO: first word of the docstring should not be This
 ]
 ignore-init-module-imports = true
 
 [tool.ruff.lint.pydocstyle]
 convention = "numpy"
+
+[tool.ruff.lint.isort]
+required-imports = ["from __future__ import annotations"]
+
+[tool.pyright]
+include = ["dargs"]
```

### Comparing `dargs-0.4.5/tests/dpmdargs.py` & `dargs-0.4.6/tests/dpmdargs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from dargs import Argument, Variant, dargs
 
 ACTIVATION_FN_DICT = {
     "relu": None,
     "relu6": None,
     "softplus": None,
     "sigmoid": None,
@@ -210,15 +212,15 @@
             list,
             [],
             [
                 Variant(
                     "type",
                     [
                         Argument("loc_frame", dict, descrpt_local_frame_args()),
-                        Argument("se_a", dict, descrpt_se_a_args()),
+                        Argument("se_e2_a", dict, descrpt_se_a_args(), alias=["se_a"]),
                         Argument("se_r", dict, descrpt_se_r_args()),
                         Argument(
                             "se_a_3be", dict, descrpt_se_a_3be_args(), alias=["se_at"]
                         ),
                         Argument(
                             "se_a_tpe",
                             dict,
@@ -758,16 +760,27 @@
     base = Argument("base", dict, [ma, lra, la, ta])
     data = base.normalize_value(data, trim_pattern="_*")
     base.check_value(data, strict=True)
 
     return data
 
 
+def gen_args() -> Argument:
+    ma = model_args()
+    lra = learning_rate_args()
+    la = loss_args()
+    ta = training_args()
+
+    base = Argument("base", dict, [ma, lra, la, ta])
+    return base
+
+
 example_json_str = """
 {
+    "$schema": "this should be ignored by dargs",
     "_comment": " model parameters",
     "model": {
         "type_map":	["O", "H"],
         "descriptor" : {
             "type": "hybrid",
             "list": [{
                 "type":		"se_a",
```

### Comparing `dargs-0.4.5/tests/test_checker.py` & `dargs-0.4.6/tests/test_checker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import unittest
 from typing import List
 
 from dargs import Argument, Variant
 from dargs.dargs import ArgumentKeyError, ArgumentTypeError, ArgumentValueError
```

### Comparing `dargs-0.4.5/tests/test_creation.py` & `dargs-0.4.6/tests/test_creation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import unittest
 
 from dargs import Argument, Variant
 
 
 class TestCreation(unittest.TestCase):
     def test_dtype(self):
```

### Comparing `dargs-0.4.5/tests/test_docgen.py` & `dargs-0.4.6/tests/test_docgen.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import json
 import unittest
 from typing import List
 
 import dargs
 from dargs import Argument, ArgumentEncoder, Variant
```

### Comparing `dargs-0.4.5/tests/test_normalizer.py` & `dargs-0.4.6/tests/test_normalizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import unittest
 
 from dargs import Argument, Variant
 
 
 class TestNormalizer(unittest.TestCase):
     def test_default(self):
```

### Comparing `dargs-0.4.5/tests/test_notebook.py` & `dargs-0.4.6/tests/test_notebook.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import unittest
 from xml.etree import ElementTree as ET
 
 from dargs import Argument, Variant
 
 try:
     import IPython  # noqa: F401
```

