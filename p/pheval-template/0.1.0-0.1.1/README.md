# Comparing `tmp/pheval_template-0.1.0.tar.gz` & `tmp/pheval_template-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pheval_template-0.1.0.tar", max compression
+gzip compressed data, was "pheval_template-0.1.1.tar", max compression
```

## Comparing `pheval_template-0.1.0.tar` & `pheval_template-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     2672 2024-05-28 11:17:59.660236 pheval_template-0.1.0/README.md
--rw-r--r--   0        0        0      811 2024-05-28 11:17:59.664236 pheval_template-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-28 11:17:59.664236 pheval_template-0.1.0/src/pheval_template/__init__.py
--rw-r--r--   0        0        0        0 2024-05-28 11:17:59.664236 pheval_template-0.1.0/src/pheval_template/post_process/__init__.py
--rw-r--r--   0        0        0      506 2024-05-28 11:17:59.664236 pheval_template-0.1.0/src/pheval_template/post_process/post_process.py
--rw-r--r--   0        0        0     3765 2024-05-28 11:17:59.664236 pheval_template-0.1.0/src/pheval_template/post_process/post_process_results_format.py
--rw-r--r--   0        0        0        0 2024-05-28 11:17:59.664236 pheval_template-0.1.0/src/pheval_template/prepare/__init__.py
--rw-r--r--   0        0        0        0 2024-05-28 11:17:59.664236 pheval_template-0.1.0/src/pheval_template/run/__init__.py
--rw-r--r--   0        0        0     2989 2024-05-28 11:17:59.664236 pheval_template-0.1.0/src/pheval_template/run/fake_predictor.py
--rw-r--r--   0        0        0      420 2024-05-28 11:17:59.664236 pheval_template-0.1.0/src/pheval_template/run/run.py
--rw-r--r--   0        0        0      755 2024-05-28 11:17:59.664236 pheval_template-0.1.0/src/pheval_template/run/run_tool.py
--rw-r--r--   0        0        0     1012 2024-05-28 11:17:59.664236 pheval_template-0.1.0/src/pheval_template/runner.py
--rw-r--r--   0        0        0     3111 1970-01-01 00:00:00.000000 pheval_template-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2672 2024-06-03 11:36:21.776039 pheval_template-0.1.1/README.md
+-rw-r--r--   0        0        0      818 2024-06-03 11:36:21.776039 pheval_template-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-06-03 11:36:21.776039 pheval_template-0.1.1/src/pheval_template/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-03 11:36:21.776039 pheval_template-0.1.1/src/pheval_template/post_process/__init__.py
+-rw-r--r--   0        0        0      506 2024-06-03 11:36:21.776039 pheval_template-0.1.1/src/pheval_template/post_process/post_process.py
+-rw-r--r--   0        0        0     3765 2024-06-03 11:36:21.780039 pheval_template-0.1.1/src/pheval_template/post_process/post_process_results_format.py
+-rw-r--r--   0        0        0        0 2024-06-03 11:36:21.780039 pheval_template-0.1.1/src/pheval_template/prepare/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-03 11:36:21.780039 pheval_template-0.1.1/src/pheval_template/run/__init__.py
+-rw-r--r--   0        0        0     2989 2024-06-03 11:36:21.780039 pheval_template-0.1.1/src/pheval_template/run/fake_predictor.py
+-rw-r--r--   0        0        0      420 2024-06-03 11:36:21.780039 pheval_template-0.1.1/src/pheval_template/run/run.py
+-rw-r--r--   0        0        0      755 2024-06-03 11:36:21.780039 pheval_template-0.1.1/src/pheval_template/run/run_tool.py
+-rw-r--r--   0        0        0     1012 2024-06-03 11:36:21.780039 pheval_template-0.1.1/src/pheval_template/runner.py
+-rw-r--r--   0        0        0     3162 1970-01-01 00:00:00.000000 pheval_template-0.1.1/PKG-INFO
```

### Comparing `pheval_template-0.1.0/README.md` & `pheval_template-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pheval_template-0.1.0/pyproject.toml` & `pheval_template-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "pheval-template"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Yasemin Bridges <y.bridges@qmul.ac.uk>"]
 readme = "README.md"
 packages = [{include = "pheval_template", from = "src"}]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = ">=3.9,<4.0.0"
 pheval = "^0.3.2"
 
 
 [tool.poetry.plugins."pheval.plugins"]
 template = "pheval_template.runner:TemplatePhEvalRunner"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `pheval_template-0.1.0/src/pheval_template/post_process/post_process_results_format.py` & `pheval_template-0.1.1/src/pheval_template/post_process/post_process_results_format.py`

 * *Files identical despite different names*

### Comparing `pheval_template-0.1.0/src/pheval_template/run/fake_predictor.py` & `pheval_template-0.1.1/src/pheval_template/run/fake_predictor.py`

 * *Files identical despite different names*

### Comparing `pheval_template-0.1.0/src/pheval_template/run/run_tool.py` & `pheval_template-0.1.1/src/pheval_template/run/run_tool.py`

 * *Files identical despite different names*

### Comparing `pheval_template-0.1.0/src/pheval_template/runner.py` & `pheval_template-0.1.1/src/pheval_template/runner.py`

 * *Files identical despite different names*

### Comparing `pheval_template-0.1.0/PKG-INFO` & `pheval_template-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pheval-template
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Yasemin Bridges
 Author-email: y.bridges@qmul.ac.uk
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pheval (>=0.3.2,<0.4.0)
 Description-Content-Type: text/markdown
 
 # Template Runner for PhEval
```

