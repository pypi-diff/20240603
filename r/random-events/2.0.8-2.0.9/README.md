# Comparing `tmp/random_events-2.0.8.tar.gz` & `tmp/random_events-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "random_events-2.0.8.tar", last modified: Thu Mar 21 17:16:16 2024, max compression
+gzip compressed data, was "random_events-2.0.9.tar", last modified: Mon Mar 25 08:25:20 2024, max compression
```

## Comparing `random_events-2.0.8.tar` & `random_events-2.0.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:16:16.284066 random_events-2.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:16:16.256066 random_events-2.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:16:16.260066 random_events-2.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-03-21 17:16:09.000000 random_events-2.0.8/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-03-21 17:16:09.000000 random_events-2.0.8/.github/workflows/test-and-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-21 17:16:09.000000 random_events-2.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-03-21 17:16:09.000000 random_events-2.0.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-03-21 17:16:16.284066 random_events-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-21 17:16:09.000000 random_events-2.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:16:16.260066 random_events-2.0.8/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-03-21 17:16:09.000000 random_events-2.0.8/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-03-21 17:16:09.000000 random_events-2.0.8/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-03-21 17:16:09.000000 random_events-2.0.8/doc/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:16:16.264066 random_events-2.0.8/doc/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)  3771988 2024-03-21 17:16:09.000000 random_events-2.0.8/doc/notebooks/example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  3958630 2024-03-21 17:16:09.000000 random_events-2.0.8/doc/notebooks/independent_constraints.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-21 17:16:09.000000 random_events-2.0.8/doc/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:16:16.276066 random_events-2.0.8/example/
--rw-r--r--   0 runner    (1001) docker     (127)  3771988 2024-03-21 17:16:09.000000 random_events-2.0.8/example/example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  3958630 2024-03-21 17:16:09.000000 random_events-2.0.8/example/independent_constraints.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-03-21 17:16:09.000000 random_events-2.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-21 17:16:09.000000 random_events-2.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 17:16:16.284066 random_events-2.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:16:16.260066 random_events-2.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:16:16.280066 random_events-2.0.8/src/random_events/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-21 17:16:09.000000 random_events-2.0.8/src/random_events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27045 2024-03-21 17:16:09.000000 random_events-2.0.8/src/random_events/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-03-21 17:16:09.000000 random_events-2.0.8/src/random_events/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8852 2024-03-21 17:16:09.000000 random_events-2.0.8/src/random_events/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:16:16.280066 random_events-2.0.8/src/random_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-03-21 17:16:16.000000 random_events-2.0.8/src/random_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-21 17:16:16.000000 random_events-2.0.8/src/random_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 17:16:16.000000 random_events-2.0.8/src/random_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-21 17:16:16.000000 random_events-2.0.8/src/random_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-21 17:16:16.000000 random_events-2.0.8/src/random_events.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:16:16.280066 random_events-2.0.8/test/
--rw-r--r--   0 runner    (1001) docker     (127)    17678 2024-03-21 17:16:09.000000 random_events-2.0.8/test/test_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-03-21 17:16:09.000000 random_events-2.0.8/test/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:25:20.386891 random_events-2.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:25:20.362891 random_events-2.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:25:20.362891 random_events-2.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-03-25 08:25:16.000000 random_events-2.0.9/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-03-25 08:25:16.000000 random_events-2.0.9/.github/workflows/test-and-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-25 08:25:16.000000 random_events-2.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-03-25 08:25:16.000000 random_events-2.0.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-03-25 08:25:20.386891 random_events-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-25 08:25:16.000000 random_events-2.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:25:20.366891 random_events-2.0.9/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-03-25 08:25:16.000000 random_events-2.0.9/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-03-25 08:25:16.000000 random_events-2.0.9/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-03-25 08:25:16.000000 random_events-2.0.9/doc/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:25:20.370891 random_events-2.0.9/doc/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)  3771988 2024-03-25 08:25:16.000000 random_events-2.0.9/doc/notebooks/example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  3958630 2024-03-25 08:25:16.000000 random_events-2.0.9/doc/notebooks/independent_constraints.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-25 08:25:16.000000 random_events-2.0.9/doc/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:25:20.378891 random_events-2.0.9/example/
+-rw-r--r--   0 runner    (1001) docker     (127)  3771988 2024-03-25 08:25:16.000000 random_events-2.0.9/example/example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  3958630 2024-03-25 08:25:16.000000 random_events-2.0.9/example/independent_constraints.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-03-25 08:25:16.000000 random_events-2.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-25 08:25:16.000000 random_events-2.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 08:25:20.386891 random_events-2.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:25:20.362891 random_events-2.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:25:20.382891 random_events-2.0.9/src/random_events/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-25 08:25:16.000000 random_events-2.0.9/src/random_events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27045 2024-03-25 08:25:16.000000 random_events-2.0.9/src/random_events/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-03-25 08:25:16.000000 random_events-2.0.9/src/random_events/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8852 2024-03-25 08:25:16.000000 random_events-2.0.9/src/random_events/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:25:20.386891 random_events-2.0.9/src/random_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-03-25 08:25:20.000000 random_events-2.0.9/src/random_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-25 08:25:20.000000 random_events-2.0.9/src/random_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 08:25:20.000000 random_events-2.0.9/src/random_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-25 08:25:20.000000 random_events-2.0.9/src/random_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-25 08:25:20.000000 random_events-2.0.9/src/random_events.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:25:20.386891 random_events-2.0.9/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    17678 2024-03-25 08:25:16.000000 random_events-2.0.9/test/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-03-25 08:25:16.000000 random_events-2.0.9/test/test_variables.py
```

### Comparing `random_events-2.0.8/.github/workflows/publish-to-test-pypi.yml` & `random_events-2.0.9/.github/workflows/publish-to-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `random_events-2.0.8/.github/workflows/test-and-build.yml` & `random_events-2.0.9/.github/workflows/test-and-build.yml`

 * *Files identical despite different names*

### Comparing `random_events-2.0.8/.readthedocs.yaml` & `random_events-2.0.9/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `random_events-2.0.8/PKG-INFO` & `random_events-2.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: random_events
-Version: 2.0.8
+Version: 2.0.9
 Summary: Random random events for probabilistic reasoning
 Author-email: Tom Schierenbeck <tom_sch@uni-bremen.de>
 Project-URL: Source, https://github.com/tomsch420/random-events
 Project-URL: Bug Tracker, https://github.com/tomsch420/random-events/issues
 Keywords: random events,probabilistic machine learning,probability theory,variables,reasoning under uncertainty
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Requires-Dist: portion>=2.4.1
-Requires-Dist: numpy>=1.24.4
-Requires-Dist: plotly>=5.20.0
-Requires-Dist: typing_extensions>=4.10.0
+Requires-Dist: portion
+Requires-Dist: numpy
+Requires-Dist: plotly
+Requires-Dist: typing_extensions
 
 # Welcome to the Random Events package!
 
 Probabilistic Machine Learning frequently requires descriptions of random variables and events
 that are shared among many packages.
 This package provides a common interface for describing random variables and events, using
 usable and easily extensible classes.
```

### Comparing `random_events-2.0.8/doc/Makefile` & `random_events-2.0.9/doc/Makefile`

 * *Files identical despite different names*

### Comparing `random_events-2.0.8/doc/conf.py` & `random_events-2.0.9/doc/conf.py`

 * *Files identical despite different names*

### Comparing `random_events-2.0.8/doc/index.rst` & `random_events-2.0.9/doc/index.rst`

 * *Files identical despite different names*

### Comparing `random_events-2.0.8/doc/notebooks/example.ipynb` & `random_events-2.0.9/doc/notebooks/example.ipynb`

 * *Files identical despite different names*

### Comparing `random_events-2.0.8/doc/notebooks/independent_constraints.ipynb` & `random_events-2.0.9/doc/notebooks/independent_constraints.ipynb`

 * *Files identical despite different names*

### Comparing `random_events-2.0.8/example/example.ipynb` & `random_events-2.0.9/example/example.ipynb`

 * *Files identical despite different names*

### Comparing `random_events-2.0.8/example/independent_constraints.ipynb` & `random_events-2.0.9/example/independent_constraints.ipynb`

 * *Files identical despite different names*

### Comparing `random_events-2.0.8/pyproject.toml` & `random_events-2.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `random_events-2.0.8/src/random_events/events.py` & `random_events-2.0.9/src/random_events/events.py`

 * *Files identical despite different names*

### Comparing `random_events-2.0.8/src/random_events/utils.py` & `random_events-2.0.9/src/random_events/utils.py`

 * *Files identical despite different names*

### Comparing `random_events-2.0.8/src/random_events/variables.py` & `random_events-2.0.9/src/random_events/variables.py`

 * *Files identical despite different names*

### Comparing `random_events-2.0.8/src/random_events.egg-info/PKG-INFO` & `random_events-2.0.9/src/random_events.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: random_events
-Version: 2.0.8
+Version: 2.0.9
 Summary: Random random events for probabilistic reasoning
 Author-email: Tom Schierenbeck <tom_sch@uni-bremen.de>
 Project-URL: Source, https://github.com/tomsch420/random-events
 Project-URL: Bug Tracker, https://github.com/tomsch420/random-events/issues
 Keywords: random events,probabilistic machine learning,probability theory,variables,reasoning under uncertainty
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Requires-Dist: portion>=2.4.1
-Requires-Dist: numpy>=1.24.4
-Requires-Dist: plotly>=5.20.0
-Requires-Dist: typing_extensions>=4.10.0
+Requires-Dist: portion
+Requires-Dist: numpy
+Requires-Dist: plotly
+Requires-Dist: typing_extensions
 
 # Welcome to the Random Events package!
 
 Probabilistic Machine Learning frequently requires descriptions of random variables and events
 that are shared among many packages.
 This package provides a common interface for describing random variables and events, using
 usable and easily extensible classes.
```

### Comparing `random_events-2.0.8/src/random_events.egg-info/SOURCES.txt` & `random_events-2.0.9/src/random_events.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `random_events-2.0.8/test/test_events.py` & `random_events-2.0.9/test/test_events.py`

 * *Files identical despite different names*

### Comparing `random_events-2.0.8/test/test_variables.py` & `random_events-2.0.9/test/test_variables.py`

 * *Files identical despite different names*

