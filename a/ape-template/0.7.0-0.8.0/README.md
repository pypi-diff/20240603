# Comparing `tmp/ape-template-0.7.0.tar.gz` & `tmp/ape-template-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-template-0.7.0.tar", last modified: Tue Dec 19 02:47:25 2023, max compression
+gzip compressed data, was "ape-template-0.8.0.tar", last modified: Mon Jun  3 14:39:06 2024, max compression
```

## Comparing `ape-template-0.7.0.tar` & `ape-template-0.8.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:47:25.415315 ape-template-0.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:47:25.411315 ape-template-0.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:47:25.411315 ape-template-0.7.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2023-12-19 02:46:32.000000 ape-template-0.7.0/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2023-12-19 02:46:32.000000 ape-template-0.7.0/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2023-12-19 02:46:32.000000 ape-template-0.7.0/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2023-12-19 02:46:32.000000 ape-template-0.7.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      651 2023-12-19 02:46:32.000000 ape-template-0.7.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:47:25.411315 ape-template-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      620 2023-12-19 02:46:32.000000 ape-template-0.7.0/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      366 2023-12-19 02:46:32.000000 ape-template-0.7.0/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2023-12-19 02:46:32.000000 ape-template-0.7.0/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      623 2023-12-19 02:46:32.000000 ape-template-0.7.0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2023-12-19 02:46:32.000000 ape-template-0.7.0/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2023-12-19 02:46:32.000000 ape-template-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      789 2023-12-19 02:46:32.000000 ape-template-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2023-12-19 02:46:32.000000 ape-template-0.7.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2023-12-19 02:46:32.000000 ape-template-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2023-12-19 02:47:25.415315 ape-template-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2023-12-19 02:46:32.000000 ape-template-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:47:25.415315 ape-template-0.7.0/ape_template/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 02:46:32.000000 ape-template-0.7.0/ape_template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-12-19 02:46:32.000000 ape-template-0.7.0/ape_template/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 02:46:32.000000 ape-template-0.7.0/ape_template/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-19 02:47:25.000000 ape-template-0.7.0/ape_template/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:47:25.415315 ape-template-0.7.0/ape_template.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2023-12-19 02:47:25.000000 ape-template-0.7.0/ape_template.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      820 2023-12-19 02:47:25.000000 ape-template-0.7.0/ape_template.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-19 02:47:25.000000 ape-template-0.7.0/ape_template.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-12-19 02:47:25.000000 ape-template-0.7.0/ape_template.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-19 02:47:25.000000 ape-template-0.7.0/ape_template.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      753 2023-12-19 02:47:25.000000 ape-template-0.7.0/ape_template.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-19 02:47:25.000000 ape-template-0.7.0/ape_template.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2023-12-19 02:46:32.000000 ape-template-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-19 02:47:25.415315 ape-template-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2023-12-19 02:46:32.000000 ape-template-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:47:25.415315 ape-template-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 02:46:32.000000 ape-template-0.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2023-12-19 02:46:32.000000 ape-template-0.7.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2023-12-19 02:46:32.000000 ape-template-0.7.0/tests/test_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:39:06.466990 ape-template-0.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:39:06.462990 ape-template-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:39:06.466990 ape-template-0.8.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-06-03 14:38:10.000000 ape-template-0.8.0/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-06-03 14:38:10.000000 ape-template-0.8.0/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-06-03 14:38:10.000000 ape-template-0.8.0/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-06-03 14:38:10.000000 ape-template-0.8.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-06-03 14:38:10.000000 ape-template-0.8.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:39:06.466990 ape-template-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-06-03 14:38:10.000000 ape-template-0.8.0/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-06-03 14:38:10.000000 ape-template-0.8.0/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-06-03 14:38:10.000000 ape-template-0.8.0/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-06-03 14:38:10.000000 ape-template-0.8.0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-06-03 14:38:10.000000 ape-template-0.8.0/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-06-03 14:38:10.000000 ape-template-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-06-03 14:38:10.000000 ape-template-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-06-03 14:38:10.000000 ape-template-0.8.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-06-03 14:38:10.000000 ape-template-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-06-03 14:39:06.466990 ape-template-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-06-03 14:38:10.000000 ape-template-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:39:06.466990 ape-template-0.8.0/ape_template/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:38:10.000000 ape-template-0.8.0/ape_template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-06-03 14:38:10.000000 ape-template-0.8.0/ape_template/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:38:10.000000 ape-template-0.8.0/ape_template/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-03 14:39:06.000000 ape-template-0.8.0/ape_template/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:39:06.466990 ape-template-0.8.0/ape_template.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-06-03 14:39:06.000000 ape-template-0.8.0/ape_template.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-06-03 14:39:06.000000 ape-template-0.8.0/ape_template.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 14:39:06.000000 ape-template-0.8.0/ape_template.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-06-03 14:39:06.000000 ape-template-0.8.0/ape_template.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 14:39:06.000000 ape-template-0.8.0/ape_template.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-06-03 14:39:06.000000 ape-template-0.8.0/ape_template.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-03 14:39:06.000000 ape-template-0.8.0/ape_template.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-06-03 14:38:10.000000 ape-template-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-06-03 14:39:06.466990 ape-template-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-06-03 14:38:10.000000 ape-template-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:39:06.466990 ape-template-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:38:10.000000 ape-template-0.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-06-03 14:38:10.000000 ape-template-0.8.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-06-03 14:38:10.000000 ape-template-0.8.0/tests/test_template.py
```

### Comparing `ape-template-0.7.0/.github/ISSUE_TEMPLATE/bug.md` & `ape-template-0.8.0/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-template-0.7.0/.github/ISSUE_TEMPLATE/feature.md` & `ape-template-0.8.0/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-template-0.7.0/.github/ISSUE_TEMPLATE/work-item.md` & `ape-template-0.8.0/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-template-0.7.0/.github/release-drafter.yml` & `ape-template-0.8.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-template-0.7.0/.github/workflows/commitlint.yaml` & `ape-template-0.8.0/.github/workflows/commitlint.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 # NOTE: Skip check on PR so as not to confuse contributors
 # NOTE: Also install a PR title checker so we don't mess up merges
 jobs:
     check:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
           with:
               fetch-depth: 0
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install .[dev]
 
         - name: Check commit history
```

### Comparing `ape-template-0.7.0/.github/workflows/prtitle.yaml` & `ape-template-0.8.0/.github/workflows/prtitle.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,18 @@
       - synchronize
 
 jobs:
     check:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install commitizen
 
         - name: Check PR Title
```

### Comparing `ape-template-0.7.0/.github/workflows/publish.yaml` & `ape-template-0.8.0/.github/workflows/publish.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
 jobs:
   deploy:
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
 
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: "3.10"
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -e .[release]
```

### Comparing `ape-template-0.7.0/.github/workflows/test.yaml` & `ape-template-0.8.0/.github/workflows/test.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -10,18 +10,18 @@
   cancel-in-progress: true
 
 jobs:
     linting:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v2
+        - uses: actions/checkout@v4
 
         - name: Setup Python
-          uses: actions/setup-python@v2
+          uses: actions/setup-python@v5
           with:
               python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install .[lint]
 
         - name: Run Black
@@ -36,40 +36,42 @@
         - name: Run mdformat
           run: mdformat . --check
 
     type-check:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v2
+        - uses: actions/checkout@v4
 
         - name: Setup Python
-          uses: actions/setup-python@v2
+          uses: actions/setup-python@v5
           with:
               python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install .[lint,test]  # Might need test deps
 
         - name: Run MyPy
           run: mypy .
 
     functional:
         runs-on: ${{ matrix.os }}
 
         strategy:
             matrix:
-                os: [ubuntu-latest, macos-latest]   # eventually add `windows-latest`
-                python-version: [3.8, 3.9, "3.10", "3.11"]
+                # TODO: Replace with macos-latest when works again.
+                #   https://github.com/actions/setup-python/issues/808
+                os: [ubuntu-latest, macos-12]   # eventually add `windows-latest`
+                python-version: [3.9, "3.10", "3.11", "3.12"]
 
         steps:
-        - uses: actions/checkout@v2
+        - uses: actions/checkout@v4
 
         - name: Setup Python
-          uses: actions/setup-python@v2
+          uses: actions/setup-python@v5
           with:
               python-version: ${{ matrix.python-version }}
 
         - name: Install Dependencies
           run: pip install .[test]
 
         - name: Run Tests
@@ -79,18 +81,18 @@
 #    fuzzing:
 #        runs-on: ubuntu-latest
 #
 #        strategy:
 #            fail-fast: true
 #
 #        steps:
-#        - uses: actions/checkout@v2
+#        - uses: actions/checkout@v4
 #
 #        - name: Setup Python
-#          uses: actions/setup-python@v2
+#          uses: actions/setup-python@v5
 #          with:
 #              python-version: "3.10"
 #
 #        - name: Install Dependencies
 #          run: pip install .[test]
 #
 #        - name: Run Tests
```

### Comparing `ape-template-0.7.0/.gitignore` & `ape-template-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-template-0.7.0/.pre-commit-config.yaml` & `ape-template-0.8.0/.pre-commit-config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 repos:
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
     -   id: check-yaml
 
--   repo: https://github.com/pre-commit/mirrors-isort
-    rev: v5.10.1
+-   repo: https://github.com/PyCQA/isort
+    rev: 5.13.2
     hooks:
       - id: isort
 
 -   repo: https://github.com/psf/black
-    rev: 23.12.0
+    rev: 24.4.2
     hooks:
       - id: black
         name: black
 
 -   repo: https://github.com/pycqa/flake8
-    rev: 6.1.0
+    rev: 7.0.0
     hooks:
     -   id: flake8
 
 -   repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.7.1
+    rev: v1.10.0
     hooks:
     -   id: mypy
         additional_dependencies: [types-setuptools, pydantic]
 
 -   repo: https://github.com/executablebooks/mdformat
     rev: 0.7.17
     hooks:
```

### Comparing `ape-template-0.7.0/CONTRIBUTING.md` & `ape-template-0.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-template-0.7.0/LICENSE` & `ape-template-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-template-0.7.0/PKG-INFO` & `ape-template-0.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: ape-template
-Version: 0.7.0
+Version: 0.8.0
 Summary: ape-template: ape plugin for cookiecutter based templates
 Home-page: https://github.com/ApeWorX/ape-template
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8,<4
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: release
 Provides-Extra: dev
 License-File: LICENSE
 
 # Quick Start
 
 The ape-template plugin allows you to use cookiecutter to template an ape project.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-template-0.7.0/README.md` & `ape-template-0.8.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Quick Start
 
 The ape-template plugin allows you to use cookiecutter to template an ape project.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-template-0.7.0/ape_template.egg-info/PKG-INFO` & `ape-template-0.8.0/ape_template.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: ape-template
-Version: 0.7.0
+Version: 0.8.0
 Summary: ape-template: ape plugin for cookiecutter based templates
 Home-page: https://github.com/ApeWorX/ape-template
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8,<4
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: release
 Provides-Extra: dev
 License-File: LICENSE
 
 # Quick Start
 
 The ape-template plugin allows you to use cookiecutter to template an ape project.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-template-0.7.0/ape_template.egg-info/SOURCES.txt` & `ape-template-0.8.0/ape_template.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-template-0.7.0/ape_template.egg-info/requires.txt` & `ape-template-0.8.0/ape_template.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 click
 cookiecutter<2.2.0,>=2.1.1
-eth-ape<0.8,>=0.7.0
+eth-ape<0.9,>=0.8.1
 
 [dev]
 pytest>=6.0
 pytest-xdist
 pytest-cov
 hypothesis<7.0,>=6.2.0
-black<24,>=23.12.0
-mypy<2,>=1.7.1
+black<25,>=24.4.2
+mypy<2,>=1.10.0
 types-setuptools
-flake8<7,>=6.1.0
+flake8<8,>=7.0.0
 flake8-breakpoint<2,>=1.1.0
 flake8-print<6,>=5.0.0
-isort<6,>=5.10.1
+isort<6,>=5.13.2
 mdformat>=0.7.17
 mdformat-gfm>=0.3.5
 mdformat-frontmatter>=0.4.1
 mdformat-pyproject>=0.0.1
 setuptools
 wheel
 twine
 commitizen
 pre-commit
 pytest-watch
 IPython
 ipdb
 
 [lint]
-black<24,>=23.12.0
-mypy<2,>=1.7.1
+black<25,>=24.4.2
+mypy<2,>=1.10.0
 types-setuptools
-flake8<7,>=6.1.0
+flake8<8,>=7.0.0
 flake8-breakpoint<2,>=1.1.0
 flake8-print<6,>=5.0.0
-isort<6,>=5.10.1
+isort<6,>=5.13.2
 mdformat>=0.7.17
 mdformat-gfm>=0.3.5
 mdformat-frontmatter>=0.4.1
 mdformat-pyproject>=0.0.1
 
 [release]
 setuptools
```

### Comparing `ape-template-0.7.0/pyproject.toml` & `ape-template-0.8.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.black]
 line-length = 100
-target-version = ['py38', 'py39', 'py310', 'py311']
+target-version = ['py39', 'py310', 'py311', 'py312']
 include = '\.pyi?$'
 
 [tool.pytest.ini_options]
 addopts = """
     -p no:ape_test
     --cov-branch
     --cov-report term
```

### Comparing `ape-template-0.7.0/setup.py` & `ape-template-0.8.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,21 +6,21 @@
     "test": [  # `test` GitHub Action jobs uses this
         "pytest>=6.0",  # Core testing package
         "pytest-xdist",  # Multi-process runner
         "pytest-cov",  # Coverage analyzer plugin
         "hypothesis>=6.2.0,<7.0",  # Strategy-based fuzzer
     ],
     "lint": [
-        "black>=23.12.0,<24",  # Auto-formatter and linter
-        "mypy>=1.7.1,<2",  # Static type analyzer
+        "black>=24.4.2,<25",  # Auto-formatter and linter
+        "mypy>=1.10.0,<2",  # Static type analyzer
         "types-setuptools",  # Needed for mypy type shed
-        "flake8>=6.1.0,<7",  # Style linter
+        "flake8>=7.0.0,<8",  # Style linter
         "flake8-breakpoint>=1.1.0,<2",  # Detect breakpoints left in code
         "flake8-print>=5.0.0,<6",  # Detect print statements left in code
-        "isort>=5.10.1,<6",  # Import sorting linter
+        "isort>=5.13.2,<6",  # Import sorting linter
         "mdformat>=0.7.17",  # Auto-formatter for markdown
         "mdformat-gfm>=0.3.5",  # Needed for formatting GitHub-flavored markdown
         "mdformat-frontmatter>=0.4.1",  # Needed for frontmatters-style headers in issue templates
         "mdformat-pyproject>=0.0.1",  # Allows configuring in pyproject.toml
     ],
     "release": [  # `release` GitHub Action job uses this
         "setuptools",  # Installation tool
@@ -58,22 +58,22 @@
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-template",
     include_package_data=True,
     install_requires=[
         "click",  # Use same version as eth-ape
         "cookiecutter>=2.1.1,<2.2.0",
-        "eth-ape>=0.7.0,<0.8",
+        "eth-ape>=0.8.1,<0.9",
     ],
     entry_points={
         "ape_cli_subcommands": [
             "ape_template=ape_template._cli:cli",
         ],
     },
-    python_requires=">=3.8,<4",
+    python_requires=">=3.9,<4",
     extras_require=extras_require,
     py_modules=["ape_template"],
     license="Apache-2.0",
     zip_safe=False,
     keywords="ethereum",
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"ape_template": ["py.typed"]},
@@ -81,13 +81,13 @@
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Natural Language :: English",
         "Operating System :: MacOS",
         "Operating System :: POSIX",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
 )
```

### Comparing `ape-template-0.7.0/tests/conftest.py` & `ape-template-0.8.0/tests/conftest.py`

 * *Files identical despite different names*

