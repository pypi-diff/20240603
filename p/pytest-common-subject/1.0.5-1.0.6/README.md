# Comparing `tmp/pytest-common-subject-1.0.5.tar.gz` & `tmp/pytest-common-subject-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-common-subject-1.0.5.tar", last modified: Thu Nov 12 22:17:21 2020, max compression
+gzip compressed data, was "pytest-common-subject-1.0.6.tar", max compression
```

## Comparing `pytest-common-subject-1.0.5.tar` & `pytest-common-subject-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0      846 2020-11-12 22:17:12.533761 pytest-common-subject-1.0.5/CHANGELOG.md
--rw-r--r--   0        0        0     1074 2020-08-03 16:15:39.453000 pytest-common-subject-1.0.5/LICENSE
--rw-r--r--   0        0        0     1074 2020-08-03 16:15:39.453000 pytest-common-subject-1.0.5/LICENSE
--rw-r--r--   0        0        0     1653 2019-05-26 17:07:24.696377 pytest-common-subject-1.0.5/README.md
--rw-r--r--   0        0        0     1210 2020-11-12 22:17:12.333757 pytest-common-subject-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      812 2019-04-22 17:56:41.740216 pytest-common-subject-1.0.5/pytest.ini
--rw-r--r--   0        0        0      413 2019-04-22 20:55:10.751917 pytest-common-subject-1.0.5/pytest_common_subject/__init__.py
--rw-r--r--   0        0        0      122 2019-04-22 17:31:38.330022 pytest-common-subject-1.0.5/pytest_common_subject/exceptions.py
--rw-r--r--   0        0        0     1158 2019-05-26 16:46:27.202519 pytest-common-subject-1.0.5/pytest_common_subject/fixtures.py
--rw-r--r--   0        0        0     7388 2019-04-22 17:54:36.691049 pytest-common-subject-1.0.5/pytest_common_subject/mixins.py
--rw-r--r--   0        0        0      173 2020-08-03 23:53:55.793424 pytest-common-subject-1.0.5/pytest_common_subject/plugin.py
--rw-r--r--   0        0        0      705 2019-04-22 18:00:49.434634 pytest-common-subject-1.0.5/pytest_common_subject/util.py
--rw-r--r--   0        0        0        0 2019-04-22 17:40:20.315015 pytest-common-subject-1.0.5/tests/__init__.py
--rw-r--r--   0        0        0     4313 2019-04-22 17:54:36.695049 pytest-common-subject-1.0.5/tests/test_mixins.py
--rw-r--r--   0        0        0     1418 2020-11-12 22:13:47.293970 pytest-common-subject-1.0.5/tox.ini
--rw-r--r--   0        0        0     2697 2020-11-12 22:17:21.496015 pytest-common-subject-1.0.5/setup.py
--rw-r--r--   0        0        0     2522 2020-11-12 22:17:21.496246 pytest-common-subject-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0      979 2022-05-15 19:54:30.737564 pytest-common-subject-1.0.6/CHANGELOG.md
+-rw-r--r--   0        0        0     1074 2022-05-15 19:44:30.901174 pytest-common-subject-1.0.6/LICENSE
+-rw-r--r--   0        0        0     1653 2022-05-15 19:44:30.901174 pytest-common-subject-1.0.6/README.md
+-rw-r--r--   0        0        0     1210 2022-05-15 19:54:30.337556 pytest-common-subject-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0      812 2022-05-15 19:44:30.901174 pytest-common-subject-1.0.6/pytest.ini
+-rw-r--r--   0        0        0      413 2022-05-15 19:44:30.901174 pytest-common-subject-1.0.6/pytest_common_subject/__init__.py
+-rw-r--r--   0        0        0      122 2022-05-15 19:44:30.901174 pytest-common-subject-1.0.6/pytest_common_subject/exceptions.py
+-rw-r--r--   0        0        0     1158 2022-05-15 19:44:30.901174 pytest-common-subject-1.0.6/pytest_common_subject/fixtures.py
+-rw-r--r--   0        0        0     7388 2022-05-15 19:44:30.901174 pytest-common-subject-1.0.6/pytest_common_subject/mixins.py
+-rw-r--r--   0        0        0      173 2022-05-15 19:44:30.901174 pytest-common-subject-1.0.6/pytest_common_subject/plugin.py
+-rw-r--r--   0        0        0      705 2022-05-15 19:44:30.901174 pytest-common-subject-1.0.6/pytest_common_subject/util.py
+-rw-r--r--   0        0        0        0 2022-05-15 19:44:30.901174 pytest-common-subject-1.0.6/tests/__init__.py
+-rw-r--r--   0        0        0     4313 2022-05-15 19:44:30.901174 pytest-common-subject-1.0.6/tests/test_mixins.py
+-rw-r--r--   0        0        0      837 2022-05-15 19:48:59.042779 pytest-common-subject-1.0.6/tox.ini
+-rw-r--r--   0        0        0     2697 2022-05-15 19:54:41.878358 pytest-common-subject-1.0.6/setup.py
+-rw-r--r--   0        0        0     2623 2022-05-15 19:54:41.878574 pytest-common-subject-1.0.6/PKG-INFO
```

### Comparing `pytest-common-subject-1.0.5/LICENSE` & `pytest-common-subject-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-common-subject-1.0.5/README.md` & `pytest-common-subject-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pytest-common-subject-1.0.5/pyproject.toml` & `pytest-common-subject-1.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'pytest-common-subject'
-version = "1.0.5"
+version = "1.0.6"
 description = 'pytest framework for testing different aspects of a common method'
 license = 'MIT'
 
 authors = [
     'Zach "theY4Kman" Kanzler <they4kman@gmail.com>'
 ]
 
@@ -25,15 +25,15 @@
 
 
 [tool.poetry.dependencies]
 # Typing annotations are used
 # XXX: for whatever reason, poetry doesn't like `>=3.6` — the additional pin allows locking to work
 python = '^3.6, >= 3.6'
 
-pytest = '>=3.6, <7'
+pytest = '>=3.6, <8'
 pytest-lambda = '>=0.1.0'
 pytest-fixture-order = '^0.1.2'
 lazy-object-proxy = '^1.3.1'
 
 
 [tool.poetry.dev-dependencies]
 tox = "^3.12"
```

### Comparing `pytest-common-subject-1.0.5/pytest.ini` & `pytest-common-subject-1.0.6/pytest.ini`

 * *Files identical despite different names*

### Comparing `pytest-common-subject-1.0.5/pytest_common_subject/fixtures.py` & `pytest-common-subject-1.0.6/pytest_common_subject/fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest-common-subject-1.0.5/pytest_common_subject/mixins.py` & `pytest-common-subject-1.0.6/pytest_common_subject/mixins.py`

 * *Files identical despite different names*

### Comparing `pytest-common-subject-1.0.5/pytest_common_subject/util.py` & `pytest-common-subject-1.0.6/pytest_common_subject/util.py`

 * *Files identical despite different names*

### Comparing `pytest-common-subject-1.0.5/tests/test_mixins.py` & `pytest-common-subject-1.0.6/tests/test_mixins.py`

 * *Files identical despite different names*

### Comparing `pytest-common-subject-1.0.5/setup.py` & `pytest-common-subject-1.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 
 modules = \
 ['pytest', 'tox', 'LICENSE', 'CHANGELOG']
 install_requires = \
 ['lazy-object-proxy>=1.3.1,<2.0.0',
  'pytest-fixture-order>=0.1.2,<0.2.0',
  'pytest-lambda>=0.1.0',
- 'pytest>=3.6,<7']
+ 'pytest>=3.6,<8']
 
 entry_points = \
 {'pytest11': ['common_subject = pytest_common_subject.plugin']}
 
 setup_kwargs = {
     'name': 'pytest-common-subject',
-    'version': '1.0.5',
+    'version': '1.0.6',
     'description': 'pytest framework for testing different aspects of a common method',
     'long_description': '# pytest-common-subject\n[![pytest-common-subject PyPI version](https://badge.fury.io/py/pytest-common-subject.svg)](https://pypi.python.org/pypi/pytest-common-subject/)\n[![pytest-common-subject PyPI pyversions](https://img.shields.io/pypi/pyversions/pytest-common-subject.svg)](https://pypi.python.org/pypi/pytest-common-subject/)\n[![pytest-common-subject PyPI license](https://img.shields.io/pypi/l/pytest-common-subject.svg)](https://pypi.python.org/pypi/pytest-common-subject/)\n\n**pytest-common-subject** is a "framework" for organizing tests to reduce boilerplate while writing, improve skimmability when reading, and bolster parallelization when executing the suite.\n\nTo utilize this framework, we first choose a single function that our group of tests will all call — in other words, an entry point, or a _common subject_. This function will be automatically called before each of our tests, with args and kwargs that can be customized by overriding fixtures — enabling child test classes to make HTTP requests as a different user, or to use a different cache backend, or to change the value of a monkeypatched method.\n\nThe return value of the chosen function will be passed as a fixture to each test. To reap the full benefits of the framework, create separate tests to verify different aspects of the return value. Was the response status code a 200? Did the response contain the expected data? Were the expected rows created in the database? By using separate tests for each of these aspects, we can pinpoint and correct multiple bugs at once, instead of getting sucked into a fix-test-fix cycle with its chorus of "oh, bother, not again!"\n',
     'author': 'Zach "theY4Kman" Kanzler',
     'author_email': 'they4kman@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/theY4Kman/pytest-common-subject',
```

### Comparing `pytest-common-subject-1.0.5/PKG-INFO` & `pytest-common-subject-1.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: pytest-common-subject
-Version: 1.0.5
+Version: 1.0.6
 Summary: pytest framework for testing different aspects of a common method
 Home-page: https://github.com/theY4Kman/pytest-common-subject
 License: MIT
 Keywords: pytest
 Author: Zach "theY4Kman" Kanzler
 Author-email: they4kman@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: lazy-object-proxy (>=1.3.1,<2.0.0)
-Requires-Dist: pytest (>=3.6,<7)
+Requires-Dist: pytest (>=3.6,<8)
 Requires-Dist: pytest-fixture-order (>=0.1.2,<0.2.0)
 Requires-Dist: pytest-lambda (>=0.1.0)
 Project-URL: Repository, https://github.com/theY4Kman/pytest-common-subject
 Description-Content-Type: text/markdown
 
 # pytest-common-subject
 [![pytest-common-subject PyPI version](https://badge.fury.io/py/pytest-common-subject.svg)](https://pypi.python.org/pypi/pytest-common-subject/)
```

