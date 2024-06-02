# Comparing `tmp/quick_python_project-0.4.2.tar.gz` & `tmp/quick_python_project-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quick_python_project-0.4.2.tar", last modified: Fri Apr 12 02:45:15 2024, max compression
+gzip compressed data, was "quick_python_project-1.0.0.tar", last modified: Sun Jun  2 21:34:52 2024, max compression
```

## Comparing `quick_python_project-0.4.2.tar` & `quick_python_project-1.0.0.tar`

### file list

```diff
@@ -1,40 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:45:15.136037 quick_python_project-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-12 02:45:10.000000 quick_python_project-0.4.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:45:15.128037 quick_python_project-0.4.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:45:15.132037 quick_python_project-0.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-12 02:45:10.000000 quick_python_project-0.4.2/.github/workflows/cd.yml
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-12 02:45:10.000000 quick_python_project-0.4.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-12 02:45:10.000000 quick_python_project-0.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-12 02:45:10.000000 quick_python_project-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-12 02:45:10.000000 quick_python_project-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-12 02:45:15.136037 quick_python_project-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-12 02:45:10.000000 quick_python_project-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-12 02:45:10.000000 quick_python_project-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 02:45:15.136037 quick_python_project-0.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:45:15.128037 quick_python_project-0.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:45:15.132037 quick_python_project-0.4.2/src/quick_python_project/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 02:45:10.000000 quick_python_project-0.4.2/src/quick_python_project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9188 2024-04-12 02:45:10.000000 quick_python_project-0.4.2/src/quick_python_project/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-04-12 02:45:10.000000 quick_python_project-0.4.2/src/quick_python_project/project_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:45:15.132037 quick_python_project-0.4.2/src/quick_python_project/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-12 02:45:10.000000 quick_python_project-0.4.2/src/quick_python_project/templates/template_.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-12 02:45:10.000000 quick_python_project-0.4.2/src/quick_python_project/templates/template_README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 02:45:10.000000 quick_python_project-0.4.2/src/quick_python_project/templates/template___init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-12 02:45:10.000000 quick_python_project-0.4.2/src/quick_python_project/templates/template_config.json
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-12 02:45:10.000000 quick_python_project-0.4.2/src/quick_python_project/templates/template_hatchling_pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-12 02:45:10.000000 quick_python_project-0.4.2/src/quick_python_project/templates/template_main.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-12 02:45:10.000000 quick_python_project-0.4.2/src/quick_python_project/templates/template_poetry_pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-12 02:45:10.000000 quick_python_project-0.4.2/src/quick_python_project/templates/template_setuptools_pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-12 02:45:15.000000 quick_python_project-0.4.2/src/quick_python_project/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:45:15.136037 quick_python_project-0.4.2/src/quick_python_project.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-12 02:45:15.000000 quick_python_project-0.4.2/src/quick_python_project.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-12 02:45:15.000000 quick_python_project-0.4.2/src/quick_python_project.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 02:45:15.000000 quick_python_project-0.4.2/src/quick_python_project.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-12 02:45:15.000000 quick_python_project-0.4.2/src/quick_python_project.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-12 02:45:15.000000 quick_python_project-0.4.2/src/quick_python_project.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-12 02:45:15.000000 quick_python_project-0.4.2/src/quick_python_project.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:45:15.136037 quick_python_project-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 02:45:10.000000 quick_python_project-0.4.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-04-12 02:45:10.000000 quick_python_project-0.4.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-04-12 02:45:10.000000 quick_python_project-0.4.2/tests/test_project_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-12 02:45:10.000000 quick_python_project-0.4.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:34:52.155588 quick_python_project-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-06-02 21:34:47.000000 quick_python_project-1.0.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:34:52.151588 quick_python_project-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:34:52.151588 quick_python_project-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-06-02 21:34:47.000000 quick_python_project-1.0.0/.github/workflows/cd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-06-02 21:34:47.000000 quick_python_project-1.0.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-06-02 21:34:47.000000 quick_python_project-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-06-02 21:34:47.000000 quick_python_project-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-06-02 21:34:47.000000 quick_python_project-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-06-02 21:34:52.155588 quick_python_project-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-06-02 21:34:47.000000 quick_python_project-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-06-02 21:34:47.000000 quick_python_project-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 21:34:52.155588 quick_python_project-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:34:52.151588 quick_python_project-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:34:52.155588 quick_python_project-1.0.0/src/quick_python_project/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 21:34:47.000000 quick_python_project-1.0.0/src/quick_python_project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-06-02 21:34:47.000000 quick_python_project-1.0.0/src/quick_python_project/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-06-02 21:34:47.000000 quick_python_project-1.0.0/src/quick_python_project/project_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:34:52.155588 quick_python_project-1.0.0/src/quick_python_project/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-06-02 21:34:47.000000 quick_python_project-1.0.0/src/quick_python_project/templates/template_.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-06-02 21:34:47.000000 quick_python_project-1.0.0/src/quick_python_project/templates/template_README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 21:34:47.000000 quick_python_project-1.0.0/src/quick_python_project/templates/template___init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-06-02 21:34:47.000000 quick_python_project-1.0.0/src/quick_python_project/templates/template_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-06-02 21:34:47.000000 quick_python_project-1.0.0/src/quick_python_project/templates/template_pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-02 21:34:52.000000 quick_python_project-1.0.0/src/quick_python_project/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:34:52.155588 quick_python_project-1.0.0/src/quick_python_project.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-06-02 21:34:52.000000 quick_python_project-1.0.0/src/quick_python_project.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-06-02 21:34:52.000000 quick_python_project-1.0.0/src/quick_python_project.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 21:34:52.000000 quick_python_project-1.0.0/src/quick_python_project.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-02 21:34:52.000000 quick_python_project-1.0.0/src/quick_python_project.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-06-02 21:34:52.000000 quick_python_project-1.0.0/src/quick_python_project.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-06-02 21:34:52.000000 quick_python_project-1.0.0/src/quick_python_project.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:34:52.155588 quick_python_project-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 21:34:47.000000 quick_python_project-1.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-06-02 21:34:47.000000 quick_python_project-1.0.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-06-02 21:34:47.000000 quick_python_project-1.0.0/tests/test_project_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-06-02 21:34:47.000000 quick_python_project-1.0.0/tox.ini
```

### Comparing `quick_python_project-0.4.2/.coveragerc` & `quick_python_project-1.0.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `quick_python_project-0.4.2/.github/workflows/cd.yml` & `quick_python_project-1.0.0/.github/workflows/cd.yml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       id-token: write
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python
       uses: actions/setup-python@v5
       with:
-        python-version: '3.11'  # Specify the Python version explicitly
+        python-version: '3.12'  # Specify the Python version explicitly
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install build
     - name: Build
       run: |
           python -m build
```

### Comparing `quick_python_project-0.4.2/.github/workflows/ci.yml` & `quick_python_project-1.0.0/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 jobs:
   build:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [windows-latest, ubuntu-latest, macos-latest]
-        python-version: ['3.9', '3.10', '3.11']
+        python-version: ['3.9', '3.10', '3.11', '3.12']
 
     steps:
     - uses: actions/checkout@v4
     - name: "Set up Python ${{ matrix.python-version }}"
       uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `quick_python_project-0.4.2/.gitignore` & `quick_python_project-1.0.0/src/quick_python_project/templates/template_.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -122,12 +122,8 @@
 
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
-.pyre/
-
-# project specific files
-default_values.json
-version.py
+.pyre/
```

### Comparing `quick_python_project-0.4.2/LICENSE` & `quick_python_project-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quick_python_project-0.4.2/pyproject.toml` & `quick_python_project-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `quick_python_project-0.4.2/src/quick_python_project/templates/template_.gitignore` & `quick_python_project-1.0.0/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -122,8 +122,15 @@
 
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
-.pyre/
+.pyre/
+
+# project specific files
+default_values.json
+version.py
+
+# Even Better TOML
+.taplo.toml
```

### Comparing `quick_python_project-0.4.2/src/quick_python_project/templates/template_hatchling_pyproject.toml` & `quick_python_project-1.0.0/src/quick_python_project/templates/template_pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+requires = ["setuptools", "wheel", "setuptools_scm"]
+build-backend = "setuptools.build_meta"
 
-[tool.hatchling]
+[tool.setuptools_scm]
 write_to = "src/PLACEHOLDER_NAME/version.py"
 version_scheme = "release-branch-semver"
-include-package-data = true
-platforms = ["any"]
-license-files = ["LICENSE"]
 
 [project]
 name = "PLACEHOLDER_NAME"
 description = "A CLI tool to create empty Python projects"
 authors = [{name = "<USERNAME>", email = "<USERNAME@example>"}]
 license = {text = "MIT"}
-dynamic = ["version"]
+version = "0.1.0"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 requires-python = "PYTHON_VERSION"
 dependencies = []
@@ -32,11 +29,16 @@
 
 [project.scripts]
 PLACEHOLDER_CMD = "PLACEHOLDER_NAME.main:main"
 
 [project.urls]
 homepage = "https://example.com"
 
-[tool.hatchling.packages.find]
+[tool.setuptools]
+include-package-data = true
+platforms = ["any"]
+license-files = ["LICENSE"]
+
+[tool.setuptools.packages.find]
 exclude = ["tests"]
 namespaces = true
-where = ["src"]
+where = ["src"]
```

### Comparing `quick_python_project-0.4.2/src/quick_python_project.egg-info/SOURCES.txt` & `quick_python_project-1.0.0/src/quick_python_project.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,12 @@
 src/quick_python_project.egg-info/dependency_links.txt
 src/quick_python_project.egg-info/entry_points.txt
 src/quick_python_project.egg-info/requires.txt
 src/quick_python_project.egg-info/top_level.txt
 src/quick_python_project/templates/template_.gitignore
 src/quick_python_project/templates/template_README.md
 src/quick_python_project/templates/template___init__.py
-src/quick_python_project/templates/template_config.json
-src/quick_python_project/templates/template_hatchling_pyproject.toml
 src/quick_python_project/templates/template_main.py
-src/quick_python_project/templates/template_poetry_pyproject.toml
-src/quick_python_project/templates/template_setuptools_pyproject.toml
+src/quick_python_project/templates/template_pyproject.toml
 tests/__init__.py
 tests/test_cli.py
 tests/test_project_generation.py
```

