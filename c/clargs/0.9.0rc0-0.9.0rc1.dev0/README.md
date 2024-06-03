# Comparing `tmp/clargs-0.9.0rc0.tar.gz` & `tmp/clargs-0.9.0rc1.dev0.tar.gz`

## Comparing `clargs-0.9.0rc0.tar` & `clargs-0.9.0rc1.dev0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 clargs-0.9.0rc0/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 clargs-0.9.0rc0/.github/workflows/run-tests-and-build.yml
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 clargs-0.9.0rc0/examples/0_basic.py
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 clargs-0.9.0rc0/examples/1_flags.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 clargs-0.9.0rc0/examples/2_show_defaults.py
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 clargs-0.9.0rc0/examples/3_list.py
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 clargs-0.9.0rc0/examples/4_parse_groups.py
--rw-r--r--   0        0        0    20371 2020-02-02 00:00:00.000000 clargs-0.9.0rc0/examples/5_logging.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 clargs-0.9.0rc0/examples/6_validation.py
--rwxr-xr-x   0        0        0     1986 2020-02-02 00:00:00.000000 clargs-0.9.0rc0/examples/__generate_example_output__.sh
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 clargs-0.9.0rc0/src/clargs/__about__.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 clargs-0.9.0rc0/src/clargs/__init__.py
--rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 clargs-0.9.0rc0/src/clargs/aap_from_data.py
--rw-r--r--   0        0        0    10061 2020-02-02 00:00:00.000000 clargs-0.9.0rc0/src/clargs/clargs.py
--rw-r--r--   0        0        0     5585 2020-02-02 00:00:00.000000 clargs-0.9.0rc0/src/clargs/docsparser.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 clargs-0.9.0rc0/src/clargs/helper_types.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 clargs-0.9.0rc0/tests/__init__.py
--rw-r--r--   0        0        0     6520 2020-02-02 00:00:00.000000 clargs-0.9.0rc0/tests/test_docsparser.py
--rw-r--r--   0        0        0    26301 2020-02-02 00:00:00.000000 clargs-0.9.0rc0/tests/test_simple.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 clargs-0.9.0rc0/tests/test_validation.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 clargs-0.9.0rc0/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 clargs-0.9.0rc0/LICENSE.txt
--rw-r--r--   0        0        0     8880 2020-02-02 00:00:00.000000 clargs-0.9.0rc0/README.md
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 clargs-0.9.0rc0/pyproject.toml
--rw-r--r--   0        0        0     9836 2020-02-02 00:00:00.000000 clargs-0.9.0rc0/PKG-INFO
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 clargs-0.9.0rc1.dev0/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 clargs-0.9.0rc1.dev0/.github/workflows/run-tests-and-build.yml
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 clargs-0.9.0rc1.dev0/examples/0_basic.py
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 clargs-0.9.0rc1.dev0/examples/1_flags.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 clargs-0.9.0rc1.dev0/examples/2_show_defaults.py
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 clargs-0.9.0rc1.dev0/examples/3_list.py
+-rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 clargs-0.9.0rc1.dev0/examples/4_parse_groups.py
+-rw-r--r--   0        0        0    20371 2020-02-02 00:00:00.000000 clargs-0.9.0rc1.dev0/examples/5_logging.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 clargs-0.9.0rc1.dev0/examples/6_validation.py
+-rwxr-xr-x   0        0        0     1986 2020-02-02 00:00:00.000000 clargs-0.9.0rc1.dev0/examples/__generate_example_output__.sh
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 clargs-0.9.0rc1.dev0/src/clargs/__about__.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 clargs-0.9.0rc1.dev0/src/clargs/__init__.py
+-rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 clargs-0.9.0rc1.dev0/src/clargs/aap_from_data.py
+-rw-r--r--   0        0        0    10076 2020-02-02 00:00:00.000000 clargs-0.9.0rc1.dev0/src/clargs/clargs.py
+-rw-r--r--   0        0        0     5585 2020-02-02 00:00:00.000000 clargs-0.9.0rc1.dev0/src/clargs/docsparser.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 clargs-0.9.0rc1.dev0/src/clargs/helper_types.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 clargs-0.9.0rc1.dev0/tests/__init__.py
+-rw-r--r--   0        0        0     6520 2020-02-02 00:00:00.000000 clargs-0.9.0rc1.dev0/tests/test_docsparser.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 clargs-0.9.0rc1.dev0/tests/test_future_annotations.py
+-rw-r--r--   0        0        0    26301 2020-02-02 00:00:00.000000 clargs-0.9.0rc1.dev0/tests/test_simple.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 clargs-0.9.0rc1.dev0/tests/test_validation.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 clargs-0.9.0rc1.dev0/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 clargs-0.9.0rc1.dev0/LICENSE.txt
+-rw-r--r--   0        0        0     8880 2020-02-02 00:00:00.000000 clargs-0.9.0rc1.dev0/README.md
+-rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 clargs-0.9.0rc1.dev0/pyproject.toml
+-rw-r--r--   0        0        0     9798 2020-02-02 00:00:00.000000 clargs-0.9.0rc1.dev0/PKG-INFO
```

### Comparing `clargs-0.9.0rc0/.github/workflows/publish.yaml` & `clargs-0.9.0rc1.dev0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `clargs-0.9.0rc0/.github/workflows/run-tests-and-build.yml` & `clargs-0.9.0rc1.dev0/.github/workflows/run-tests-and-build.yml`

 * *Files identical despite different names*

### Comparing `clargs-0.9.0rc0/examples/0_basic.py` & `clargs-0.9.0rc1.dev0/examples/0_basic.py`

 * *Files identical despite different names*

### Comparing `clargs-0.9.0rc0/examples/1_flags.py` & `clargs-0.9.0rc1.dev0/examples/1_flags.py`

 * *Files identical despite different names*

### Comparing `clargs-0.9.0rc0/examples/2_show_defaults.py` & `clargs-0.9.0rc1.dev0/examples/2_show_defaults.py`

 * *Files identical despite different names*

### Comparing `clargs-0.9.0rc0/examples/3_list.py` & `clargs-0.9.0rc1.dev0/examples/3_list.py`

 * *Files identical despite different names*

### Comparing `clargs-0.9.0rc0/examples/4_parse_groups.py` & `clargs-0.9.0rc1.dev0/examples/4_parse_groups.py`

 * *Files identical despite different names*

### Comparing `clargs-0.9.0rc0/examples/5_logging.py` & `clargs-0.9.0rc1.dev0/examples/5_logging.py`

 * *Files identical despite different names*

### Comparing `clargs-0.9.0rc0/examples/6_validation.py` & `clargs-0.9.0rc1.dev0/examples/6_validation.py`

 * *Files identical despite different names*

### Comparing `clargs-0.9.0rc0/examples/__generate_example_output__.sh` & `clargs-0.9.0rc1.dev0/examples/__generate_example_output__.sh`

 * *Files identical despite different names*

### Comparing `clargs-0.9.0rc0/src/clargs/__init__.py` & `clargs-0.9.0rc1.dev0/src/clargs/__init__.py`

 * *Files identical despite different names*

### Comparing `clargs-0.9.0rc0/src/clargs/aap_from_data.py` & `clargs-0.9.0rc1.dev0/src/clargs/aap_from_data.py`

 * *Files identical despite different names*

### Comparing `clargs-0.9.0rc0/src/clargs/clargs.py` & `clargs-0.9.0rc1.dev0/src/clargs/clargs.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,15 +201,15 @@
             prefix_chars=prefix_chars,
         )
         self.add_to_parser(parser, func)
         return parser
 
     def add_to_parser(self, parser: argparse.ArgumentParser, func: t.Callable) -> None:
         parser.set_defaults(_clargs_func_=func)
-        signature = inspect.signature(func)
+        signature = inspect.signature(func, eval_str=True)
         docstring = inspect.getdoc(func) or ""
         paramdescriptions = {
             p.name: p.description
             for p in docsparser.get_parameter_info_from_docstring(docstring)
         }
         args_and_aap_s: t.Sequence[t.Tuple[t.Sequence[str], AddArgumentParameters]] = [
             aap_from_data.AapFromData.from_param_and_settings(
```

### Comparing `clargs-0.9.0rc0/src/clargs/docsparser.py` & `clargs-0.9.0rc1.dev0/src/clargs/docsparser.py`

 * *Files identical despite different names*

### Comparing `clargs-0.9.0rc0/src/clargs/helper_types.py` & `clargs-0.9.0rc1.dev0/src/clargs/helper_types.py`

 * *Files identical despite different names*

### Comparing `clargs-0.9.0rc0/tests/test_docsparser.py` & `clargs-0.9.0rc1.dev0/tests/test_docsparser.py`

 * *Files identical despite different names*

### Comparing `clargs-0.9.0rc0/tests/test_simple.py` & `clargs-0.9.0rc1.dev0/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `clargs-0.9.0rc0/tests/test_validation.py` & `clargs-0.9.0rc1.dev0/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `clargs-0.9.0rc0/LICENSE.txt` & `clargs-0.9.0rc1.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `clargs-0.9.0rc0/README.md` & `clargs-0.9.0rc1.dev0/README.md`

 * *Files identical despite different names*

### Comparing `clargs-0.9.0rc0/pyproject.toml` & `clargs-0.9.0rc1.dev0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 requires-python = ">=3.10"
 license = "MIT"
 keywords = []
 authors = [
   { name = "Claude", email = "pypi@claude.nl" },
 ]
 classifiers = [
-  "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
   "License :: OSI Approved :: MIT License",
```

### Comparing `clargs-0.9.0rc0/PKG-INFO` & `clargs-0.9.0rc1.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.3
 Name: clargs
-Version: 0.9.0rc0
+Version: 0.9.0rc1.dev0
 Summary: Easily generate commandline apps from your functions, based on type hints
 Project-URL: Documentation, https://github.com/reinhrst/clargs#readme
 Project-URL: Issues, https://github.com/reinhrst/clargs/issues
 Project-URL: Source, https://github.com/reinhrst/clargs
 Author-email: Claude <pypi@claude.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
-Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

