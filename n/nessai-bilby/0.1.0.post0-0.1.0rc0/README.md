# Comparing `tmp/nessai_bilby-0.1.0.post0.tar.gz` & `tmp/nessai_bilby-0.1.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nessai_bilby-0.1.0.post0.tar", last modified: Mon Jun  3 08:30:35 2024, max compression
+gzip compressed data, was "nessai_bilby-0.1.0rc0.tar", last modified: Fri May 31 10:37:29 2024, max compression
```

## Comparing `nessai_bilby-0.1.0.post0.tar` & `nessai_bilby-0.1.0rc0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:30:35.920266 nessai_bilby-0.1.0.post0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:30:35.916266 nessai_bilby-0.1.0.post0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:30:35.916266 nessai_bilby-0.1.0.post0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-06-03 08:30:28.000000 nessai_bilby-0.1.0.post0/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-06-03 08:30:28.000000 nessai_bilby-0.1.0.post0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-06-03 08:30:28.000000 nessai_bilby-0.1.0.post0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-06-03 08:30:28.000000 nessai_bilby-0.1.0.post0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-06-03 08:30:28.000000 nessai_bilby-0.1.0.post0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-06-03 08:30:35.920266 nessai_bilby-0.1.0.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-06-03 08:30:28.000000 nessai_bilby-0.1.0.post0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-06-03 08:30:28.000000 nessai_bilby-0.1.0.post0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 08:30:35.920266 nessai_bilby-0.1.0.post0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:30:35.916266 nessai_bilby-0.1.0.post0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:30:35.916266 nessai_bilby-0.1.0.post0/src/nessai_bilby/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-06-03 08:30:28.000000 nessai_bilby-0.1.0.post0/src/nessai_bilby/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-06-03 08:30:28.000000 nessai_bilby-0.1.0.post0/src/nessai_bilby/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10744 2024-06-03 08:30:28.000000 nessai_bilby-0.1.0.post0/src/nessai_bilby/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:30:35.920266 nessai_bilby-0.1.0.post0/src/nessai_bilby.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-06-03 08:30:35.000000 nessai_bilby-0.1.0.post0/src/nessai_bilby.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-06-03 08:30:35.000000 nessai_bilby-0.1.0.post0/src/nessai_bilby.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 08:30:35.000000 nessai_bilby-0.1.0.post0/src/nessai_bilby.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-06-03 08:30:35.000000 nessai_bilby-0.1.0.post0/src/nessai_bilby.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-06-03 08:30:35.000000 nessai_bilby-0.1.0.post0/src/nessai_bilby.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-03 08:30:35.000000 nessai_bilby-0.1.0.post0/src/nessai_bilby.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:30:35.920266 nessai_bilby-0.1.0.post0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-06-03 08:30:28.000000 nessai_bilby-0.1.0.post0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-06-03 08:30:28.000000 nessai_bilby-0.1.0.post0/tests/test_bilby_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-06-03 08:30:28.000000 nessai_bilby-0.1.0.post0/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-06-03 08:30:28.000000 nessai_bilby-0.1.0.post0/tests/test_sampler_class.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:37:29.422508 nessai_bilby-0.1.0rc0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:37:29.418508 nessai_bilby-0.1.0rc0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:37:29.418508 nessai_bilby-0.1.0rc0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-31 10:37:24.000000 nessai_bilby-0.1.0rc0/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-31 10:37:24.000000 nessai_bilby-0.1.0rc0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-31 10:37:24.000000 nessai_bilby-0.1.0rc0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-31 10:37:24.000000 nessai_bilby-0.1.0rc0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-31 10:37:24.000000 nessai_bilby-0.1.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-31 10:37:29.422508 nessai_bilby-0.1.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-31 10:37:24.000000 nessai_bilby-0.1.0rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-31 10:37:24.000000 nessai_bilby-0.1.0rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 10:37:29.422508 nessai_bilby-0.1.0rc0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:37:29.418508 nessai_bilby-0.1.0rc0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:37:29.422508 nessai_bilby-0.1.0rc0/src/nessai_bilby/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-31 10:37:24.000000 nessai_bilby-0.1.0rc0/src/nessai_bilby/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-05-31 10:37:24.000000 nessai_bilby-0.1.0rc0/src/nessai_bilby/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10744 2024-05-31 10:37:24.000000 nessai_bilby-0.1.0rc0/src/nessai_bilby/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:37:29.422508 nessai_bilby-0.1.0rc0/src/nessai_bilby.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-31 10:37:29.000000 nessai_bilby-0.1.0rc0/src/nessai_bilby.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-31 10:37:29.000000 nessai_bilby-0.1.0rc0/src/nessai_bilby.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 10:37:29.000000 nessai_bilby-0.1.0rc0/src/nessai_bilby.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-31 10:37:29.000000 nessai_bilby-0.1.0rc0/src/nessai_bilby.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-31 10:37:29.000000 nessai_bilby-0.1.0rc0/src/nessai_bilby.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-31 10:37:29.000000 nessai_bilby-0.1.0rc0/src/nessai_bilby.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:37:29.422508 nessai_bilby-0.1.0rc0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-31 10:37:24.000000 nessai_bilby-0.1.0rc0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-31 10:37:24.000000 nessai_bilby-0.1.0rc0/tests/test_bilby_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-31 10:37:24.000000 nessai_bilby-0.1.0rc0/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-31 10:37:24.000000 nessai_bilby-0.1.0rc0/tests/test_sampler_class.py
```

### Comparing `nessai_bilby-0.1.0.post0/.github/workflows/publish.yml` & `nessai_bilby-0.1.0rc0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `nessai_bilby-0.1.0.post0/.github/workflows/tests.yml` & `nessai_bilby-0.1.0rc0/.github/workflows/tests.yml`

 * *Files 21% similar despite different names*

```diff
@@ -8,27 +8,21 @@
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
 
 jobs:
   unittests:
-    name: Unit tests - Python ${{ matrix.python-version }} (${{ matrix.os }})
+    name: Unit tests - Python ${{ matrix.python-version }}
 
     strategy:
       fail-fast: false
       matrix:
-        os: [ubuntu-latest]
         python-version: ["3.9", "3.10", "3.11", "3.12"]
-        include:
-          - os: windows-latest
-            python-version: 3.11
-          - os: macos-latest
-            python-version: 3.11
-    runs-on: ${{ matrix.os }}
+    runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `nessai_bilby-0.1.0.post0/.gitignore` & `nessai_bilby-0.1.0rc0/.gitignore`

 * *Files identical despite different names*

### Comparing `nessai_bilby-0.1.0.post0/LICENSE` & `nessai_bilby-0.1.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `nessai_bilby-0.1.0.post0/PKG-INFO` & `nessai_bilby-0.1.0rc0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nessai-bilby
-Version: 0.1.0.post0
+Version: 0.1.0rc0
 Summary: Interface and plugin for using nessai in bilby
 Author-email: "Michael J. Williams" <michaeljw1@googlemail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `nessai_bilby-0.1.0.post0/README.md` & `nessai_bilby-0.1.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `nessai_bilby-0.1.0.post0/pyproject.toml` & `nessai_bilby-0.1.0rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nessai_bilby-0.1.0.post0/src/nessai_bilby/model.py` & `nessai_bilby-0.1.0rc0/src/nessai_bilby/model.py`

 * *Files identical despite different names*

### Comparing `nessai_bilby-0.1.0.post0/src/nessai_bilby/plugin.py` & `nessai_bilby-0.1.0rc0/src/nessai_bilby/plugin.py`

 * *Files identical despite different names*

### Comparing `nessai_bilby-0.1.0.post0/src/nessai_bilby.egg-info/PKG-INFO` & `nessai_bilby-0.1.0rc0/src/nessai_bilby.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nessai-bilby
-Version: 0.1.0.post0
+Version: 0.1.0rc0
 Summary: Interface and plugin for using nessai in bilby
 Author-email: "Michael J. Williams" <michaeljw1@googlemail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `nessai_bilby-0.1.0.post0/src/nessai_bilby.egg-info/SOURCES.txt` & `nessai_bilby-0.1.0rc0/src/nessai_bilby.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nessai_bilby-0.1.0.post0/tests/conftest.py` & `nessai_bilby-0.1.0rc0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nessai_bilby-0.1.0.post0/tests/test_bilby_integration.py` & `nessai_bilby-0.1.0rc0/tests/test_bilby_integration.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,14 @@
         nlive=100,
         stopping=5.0,
         sampler="nessai",
         injection_parameters={"x": 0.0, "y": 0.0},
         analytic_priors=True,
         seed=1234,
         nessai_likelihood_constraint=likelihood_constraint,
-        n_pool=None,
     )
 
 
 def test_sampling_inessai(
     bilby_gaussian_likelihood_and_priors,
     tmp_path,
     likelihood_constraint,
@@ -52,9 +51,8 @@
         priors=priors,
         nlive=100,
         min_samples=10,
         sampler="inessai",
         injection_parameters={"x": 0.0, "y": 0.0},
         seed=1234,
         nessai_likelihood_constraint=likelihood_constraint,
-        n_pool=None,
     )
```

### Comparing `nessai_bilby-0.1.0.post0/tests/test_model.py` & `nessai_bilby-0.1.0rc0/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `nessai_bilby-0.1.0.post0/tests/test_sampler_class.py` & `nessai_bilby-0.1.0rc0/tests/test_sampler_class.py`

 * *Files identical despite different names*

