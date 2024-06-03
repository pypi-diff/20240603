# Comparing `tmp/glbuild-0.1.3.tar.gz` & `tmp/glbuild-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glbuild-0.1.3.tar", max compression
+gzip compressed data, was "glbuild-0.1.4.tar", max compression
```

## Comparing `glbuild-0.1.3.tar` & `glbuild-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1071 2024-05-30 13:28:15.046874 glbuild-0.1.3/LICENSE
--rw-r--r--   0        0        0      907 2024-05-30 13:28:15.046874 glbuild-0.1.3/README.md
--rw-r--r--   0        0        0       77 2024-05-30 13:28:15.046874 glbuild-0.1.3/glbuild/__init__.py
--rw-r--r--   0        0        0       23 2024-05-30 13:28:15.046874 glbuild-0.1.3/glbuild/cli/__init__.py
--rw-r--r--   0        0        0     1024 2024-05-30 13:28:15.046874 glbuild-0.1.3/glbuild/cli/main.py
--rw-r--r--   0        0        0       39 2024-05-30 13:28:15.046874 glbuild-0.1.3/glbuild/collector/__init__.py
--rw-r--r--   0        0        0     1082 2024-05-30 13:28:15.046874 glbuild-0.1.3/glbuild/collector/progress.py
--rw-r--r--   0        0        0      124 2024-05-30 13:28:15.046874 glbuild-0.1.3/glbuild/constants.py
--rw-r--r--   0        0        0     7391 2024-05-30 13:28:15.047874 glbuild-0.1.3/glbuild/glbuild.py
--rw-r--r--   0        0        0       23 2024-05-30 13:28:15.047874 glbuild-0.1.3/glbuild/utils/__init__.py
--rw-r--r--   0        0        0    32235 2024-05-30 13:28:15.047874 glbuild-0.1.3/glbuild/utils/tempfile.py
--rw-r--r--   0        0        0     2180 2024-05-30 13:28:15.047874 glbuild-0.1.3/glbuild/utils/utils.py
--rw-r--r--   0        0        0      932 2024-05-30 13:28:15.048874 glbuild-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1832 1970-01-01 00:00:00.000000 glbuild-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-06-03 15:31:25.353510 glbuild-0.1.4/LICENSE
+-rw-r--r--   0        0        0      907 2024-06-03 15:31:25.353510 glbuild-0.1.4/README.md
+-rw-r--r--   0        0        0       77 2024-06-03 15:31:25.353510 glbuild-0.1.4/glbuild/__init__.py
+-rw-r--r--   0        0        0       23 2024-06-03 15:31:25.353510 glbuild-0.1.4/glbuild/cli/__init__.py
+-rw-r--r--   0        0        0     1024 2024-06-03 15:31:25.353510 glbuild-0.1.4/glbuild/cli/main.py
+-rw-r--r--   0        0        0       39 2024-06-03 15:31:25.354510 glbuild-0.1.4/glbuild/collector/__init__.py
+-rw-r--r--   0        0        0     1082 2024-06-03 15:31:25.354510 glbuild-0.1.4/glbuild/collector/progress.py
+-rw-r--r--   0        0        0      124 2024-06-03 15:31:25.354510 glbuild-0.1.4/glbuild/constants.py
+-rw-r--r--   0        0        0     7391 2024-06-03 15:31:25.354510 glbuild-0.1.4/glbuild/glbuild.py
+-rw-r--r--   0        0        0       23 2024-06-03 15:31:25.354510 glbuild-0.1.4/glbuild/utils/__init__.py
+-rw-r--r--   0        0        0    32235 2024-06-03 15:31:25.354510 glbuild-0.1.4/glbuild/utils/tempfile.py
+-rw-r--r--   0        0        0     2180 2024-06-03 15:31:25.354510 glbuild-0.1.4/glbuild/utils/utils.py
+-rw-r--r--   0        0        0      949 2024-06-03 15:31:25.355510 glbuild-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1871 1970-01-01 00:00:00.000000 glbuild-0.1.4/PKG-INFO
```

### Comparing `glbuild-0.1.3/LICENSE` & `glbuild-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `glbuild-0.1.3/README.md` & `glbuild-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `glbuild-0.1.3/glbuild/cli/main.py` & `glbuild-0.1.4/glbuild/cli/main.py`

 * *Files identical despite different names*

### Comparing `glbuild-0.1.3/glbuild/collector/progress.py` & `glbuild-0.1.4/glbuild/collector/progress.py`

 * *Files identical despite different names*

### Comparing `glbuild-0.1.3/glbuild/glbuild.py` & `glbuild-0.1.4/glbuild/glbuild.py`

 * *Files identical despite different names*

### Comparing `glbuild-0.1.3/glbuild/utils/tempfile.py` & `glbuild-0.1.4/glbuild/utils/tempfile.py`

 * *Files identical despite different names*

### Comparing `glbuild-0.1.3/glbuild/utils/utils.py` & `glbuild-0.1.4/glbuild/utils/utils.py`

 * *Files identical despite different names*

### Comparing `glbuild-0.1.3/pyproject.toml` & `glbuild-0.1.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "glbuild"
-version = "0.1.3"
+version = "0.1.4"
 description = "Gitlab build jobs data collector. CLI tool and Python package."
 authors = [ "Henri Aïdasso <ahenrij@gmail.com>",]
 license = "LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -17,14 +17,15 @@
 pydantic-settings = "^2.2.1"
 tqdm = "^4.66.4"
 python-gitlab = "^4.5.0"
 pandas = "^2.2.2"
 requests = "^2.31.0"
 types-requests = "^2.31.0.20240406"
 types-toml = "^0.10.8.20240310"
+toml = "^0.10.2"
 
 [tool.poetry.scripts]
 glbuild = "glbuild.cli.main:cli"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.2.0"
 pytest-cov = "^5.0.0"
```

### Comparing `glbuild-0.1.3/PKG-INFO` & `glbuild-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glbuild
-Version: 0.1.3
+Version: 0.1.4
 Summary: Gitlab build jobs data collector. CLI tool and Python package.
 License: LICENSE
 Author: Henri Aïdasso
 Author-email: ahenrij@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
 Requires-Dist: python-gitlab (>=4.5.0,<5.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: tqdm (>=4.66.4,<5.0.0)
 Requires-Dist: types-requests (>=2.31.0.20240406,<3.0.0.0)
 Requires-Dist: types-toml (>=0.10.8.20240310,<0.11.0.0)
 Description-Content-Type: text/markdown
 
 # glbuild
```

