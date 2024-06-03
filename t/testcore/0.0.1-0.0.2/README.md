# Comparing `tmp/testcore-0.0.1.tar.gz` & `tmp/testcore-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testcore-0.0.1.tar", last modified: Mon Jun  3 12:11:50 2024, max compression
+gzip compressed data, was "testcore-0.0.2.tar", last modified: Mon Jun  3 13:45:23 2024, max compression
```

## Comparing `testcore-0.0.1.tar` & `testcore-0.0.2.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:11:50.424636 testcore-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-06-03 12:11:38.000000 testcore-0.0.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:11:50.416636 testcore-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:11:50.420636 testcore-0.0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-06-03 12:11:38.000000 testcore-0.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-06-03 12:11:38.000000 testcore-0.0.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-06-03 12:11:38.000000 testcore-0.0.1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:11:50.420636 testcore-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-06-03 12:11:38.000000 testcore-0.0.1/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-06-03 12:11:38.000000 testcore-0.0.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-06-03 12:11:38.000000 testcore-0.0.1/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-06-03 12:11:38.000000 testcore-0.0.1/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-06-03 12:11:38.000000 testcore-0.0.1/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-06-03 12:11:38.000000 testcore-0.0.1/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-06-03 12:11:38.000000 testcore-0.0.1/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-06-03 12:11:38.000000 testcore-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-06-03 12:11:38.000000 testcore-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-06-03 12:11:38.000000 testcore-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-06-03 12:11:50.424636 testcore-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-06-03 12:11:38.000000 testcore-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:11:50.420636 testcore-0.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-06-03 12:11:38.000000 testcore-0.0.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-06-03 12:11:38.000000 testcore-0.0.1/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-06-03 12:11:38.000000 testcore-0.0.1/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-06-03 12:11:38.000000 testcore-0.0.1/docs/ethopy.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:11:50.420636 testcore-0.0.1/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-06-03 12:11:38.000000 testcore-0.0.1/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-03 12:11:38.000000 testcore-0.0.1/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-06-03 12:11:38.000000 testcore-0.0.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-06-03 12:11:38.000000 testcore-0.0.1/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:11:50.420636 testcore-0.0.1/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-06-03 12:11:38.000000 testcore-0.0.1/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-06-03 12:11:38.000000 testcore-0.0.1/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:11:50.420636 testcore-0.0.1/ethopy/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-06-03 12:11:38.000000 testcore-0.0.1/ethopy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-06-03 12:11:38.000000 testcore-0.0.1/ethopy/common.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-06-03 12:11:38.000000 testcore-0.0.1/ethopy/ethopy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-06-03 12:11:38.000000 testcore-0.0.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-06-03 12:11:38.000000 testcore-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-06-03 12:11:38.000000 testcore-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-06-03 12:11:38.000000 testcore-0.0.1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 12:11:50.424636 testcore-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:11:50.424636 testcore-0.0.1/testcore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-06-03 12:11:50.000000 testcore-0.0.1/testcore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-06-03 12:11:50.000000 testcore-0.0.1/testcore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 12:11:50.000000 testcore-0.0.1/testcore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-06-03 12:11:50.000000 testcore-0.0.1/testcore.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-06-03 12:11:50.000000 testcore-0.0.1/testcore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-03 12:11:50.000000 testcore-0.0.1/testcore.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:11:50.424636 testcore-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-06-03 12:11:38.000000 testcore-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-06-03 12:11:38.000000 testcore-0.0.1/tests/test_ethopy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:45:23.536132 testcore-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-06-03 13:45:04.000000 testcore-0.0.2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:45:23.528132 testcore-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:45:23.532132 testcore-0.0.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-06-03 13:45:04.000000 testcore-0.0.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-06-03 13:45:04.000000 testcore-0.0.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-06-03 13:45:04.000000 testcore-0.0.2/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:45:23.532132 testcore-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-06-03 13:45:04.000000 testcore-0.0.2/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-06-03 13:45:04.000000 testcore-0.0.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-06-03 13:45:04.000000 testcore-0.0.2/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-06-03 13:45:04.000000 testcore-0.0.2/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-06-03 13:45:04.000000 testcore-0.0.2/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-06-03 13:45:04.000000 testcore-0.0.2/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-06-03 13:45:04.000000 testcore-0.0.2/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-06-03 13:45:04.000000 testcore-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-06-03 13:45:04.000000 testcore-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-06-03 13:45:04.000000 testcore-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-06-03 13:45:23.536132 testcore-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-06-03 13:45:04.000000 testcore-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:45:23.532132 testcore-0.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-06-03 13:45:04.000000 testcore-0.0.2/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-06-03 13:45:04.000000 testcore-0.0.2/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-06-03 13:45:04.000000 testcore-0.0.2/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-06-03 13:45:04.000000 testcore-0.0.2/docs/ethopy.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:45:23.536132 testcore-0.0.2/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-06-03 13:45:04.000000 testcore-0.0.2/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-03 13:45:04.000000 testcore-0.0.2/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-06-03 13:45:04.000000 testcore-0.0.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-06-03 13:45:04.000000 testcore-0.0.2/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:45:23.536132 testcore-0.0.2/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-06-03 13:45:04.000000 testcore-0.0.2/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-06-03 13:45:04.000000 testcore-0.0.2/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:45:23.536132 testcore-0.0.2/ethopy/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-06-03 13:45:04.000000 testcore-0.0.2/ethopy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-06-03 13:45:04.000000 testcore-0.0.2/ethopy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-06-03 13:45:04.000000 testcore-0.0.2/ethopy/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-06-03 13:45:04.000000 testcore-0.0.2/ethopy/ethopy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-06-03 13:45:04.000000 testcore-0.0.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-06-03 13:45:04.000000 testcore-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-06-03 13:45:04.000000 testcore-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-06-03 13:45:04.000000 testcore-0.0.2/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 13:45:23.536132 testcore-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:45:23.536132 testcore-0.0.2/testcore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-06-03 13:45:23.000000 testcore-0.0.2/testcore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-06-03 13:45:23.000000 testcore-0.0.2/testcore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 13:45:23.000000 testcore-0.0.2/testcore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-06-03 13:45:23.000000 testcore-0.0.2/testcore.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-06-03 13:45:23.000000 testcore-0.0.2/testcore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-03 13:45:23.000000 testcore-0.0.2/testcore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:45:23.536132 testcore-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-06-03 13:45:04.000000 testcore-0.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-06-03 13:45:04.000000 testcore-0.0.2/tests/test_ethopy.py
```

### Comparing `testcore-0.0.1/.github/workflows/docs-build.yml` & `testcore-0.0.2/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `testcore-0.0.1/.github/workflows/docs.yml` & `testcore-0.0.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `testcore-0.0.1/.github/workflows/installation.yml` & `testcore-0.0.2/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `testcore-0.0.1/.github/workflows/macos.yml` & `testcore-0.0.2/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `testcore-0.0.1/.github/workflows/pypi.yml` & `testcore-0.0.2/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `testcore-0.0.1/.github/workflows/ubuntu.yml` & `testcore-0.0.2/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `testcore-0.0.1/.github/workflows/windows.yml` & `testcore-0.0.2/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `testcore-0.0.1/.gitignore` & `testcore-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `testcore-0.0.1/LICENSE` & `testcore-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `testcore-0.0.1/PKG-INFO` & `testcore-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testcore
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Author-email: Alex Evangelou <admin@example.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/alexevag/testcore
 Keywords: testcore
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `testcore-0.0.1/README.md` & `testcore-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `testcore-0.0.1/docs/contributing.md` & `testcore-0.0.2/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `testcore-0.0.1/docs/installation.md` & `testcore-0.0.2/docs/installation.md`

 * *Files identical despite different names*

### Comparing `testcore-0.0.1/mkdocs.yml` & `testcore-0.0.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `testcore-0.0.1/pyproject.toml` & `testcore-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "testcore"
-version = "0.0.1"
+version = "0.0.2"
 dynamic = [
     "dependencies",
 ]
 description = "Python Boilerplate contains all the boilerplate you need to create a Python package."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -48,15 +48,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.0.1"
+current_version = "0.0.2"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

### Comparing `testcore-0.0.1/testcore.egg-info/PKG-INFO` & `testcore-0.0.2/testcore.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testcore
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Author-email: Alex Evangelou <admin@example.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/alexevag/testcore
 Keywords: testcore
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `testcore-0.0.1/testcore.egg-info/SOURCES.txt` & `testcore-0.0.2/testcore.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 docs/faq.md
 docs/index.md
 docs/installation.md
 docs/usage.md
 docs/examples/intro.ipynb
 docs/overrides/main.html
 ethopy/__init__.py
+ethopy/__main__.py
 ethopy/common.py
 ethopy/ethopy.py
 testcore.egg-info/PKG-INFO
 testcore.egg-info/SOURCES.txt
 testcore.egg-info/dependency_links.txt
 testcore.egg-info/entry_points.txt
 testcore.egg-info/requires.txt
```

