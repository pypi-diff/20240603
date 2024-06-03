# Comparing `tmp/cmdstanpy-1.2.2.tar.gz` & `tmp/cmdstanpy-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmdstanpy-1.2.2.tar", last modified: Tue Mar 26 16:30:53 2024, max compression
+gzip compressed data, was "cmdstanpy-1.2.3.tar", last modified: Mon Jun  3 15:16:58 2024, max compression
```

## Comparing `cmdstanpy-1.2.2.tar` & `cmdstanpy-1.2.3.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:30:53.886464 cmdstanpy-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-03-26 16:26:51.000000 cmdstanpy-1.2.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-26 16:30:51.000000 cmdstanpy-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-03-26 16:30:53.886464 cmdstanpy-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-03-26 16:26:51.000000 cmdstanpy-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:30:53.878464 cmdstanpy-1.2.2/cmdstanpy/
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-03-26 16:30:51.000000 cmdstanpy-1.2.2/cmdstanpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-26 16:30:51.000000 cmdstanpy-1.2.2/cmdstanpy/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    39752 2024-03-26 16:30:51.000000 cmdstanpy-1.2.2/cmdstanpy/cmdstan_args.py
--rw-r--r--   0 runner    (1001) docker     (127)    20806 2024-03-26 16:30:51.000000 cmdstanpy-1.2.2/cmdstanpy/compilation.py
--rw-r--r--   0 runner    (1001) docker     (127)    23514 2024-03-26 16:26:51.000000 cmdstanpy-1.2.2/cmdstanpy/install_cmdstan.py
--rw-r--r--   0 runner    (1001) docker     (127)    11627 2024-03-26 16:26:51.000000 cmdstanpy-1.2.2/cmdstanpy/install_cxx_toolchain.py
--rw-r--r--   0 runner    (1001) docker     (127)    89660 2024-03-26 16:30:51.000000 cmdstanpy-1.2.2/cmdstanpy/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-03-26 16:26:51.000000 cmdstanpy-1.2.2/cmdstanpy/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 16:26:51.000000 cmdstanpy-1.2.2/cmdstanpy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:30:53.882465 cmdstanpy-1.2.2/cmdstanpy/stanfit/
--rw-r--r--   0 runner    (1001) docker     (127)    10356 2024-03-26 16:26:51.000000 cmdstanpy-1.2.2/cmdstanpy/stanfit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26049 2024-03-26 16:26:51.000000 cmdstanpy-1.2.2/cmdstanpy/stanfit/gq.py
--rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-03-26 16:26:51.000000 cmdstanpy-1.2.2/cmdstanpy/stanfit/laplace.py
--rw-r--r--   0 runner    (1001) docker     (127)    31566 2024-03-26 16:26:51.000000 cmdstanpy-1.2.2/cmdstanpy/stanfit/mcmc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-03-26 16:26:51.000000 cmdstanpy-1.2.2/cmdstanpy/stanfit/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    10458 2024-03-26 16:26:51.000000 cmdstanpy-1.2.2/cmdstanpy/stanfit/mle.py
--rw-r--r--   0 runner    (1001) docker     (127)     8278 2024-03-26 16:26:51.000000 cmdstanpy-1.2.2/cmdstanpy/stanfit/pathfinder.py
--rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-03-26 16:26:51.000000 cmdstanpy-1.2.2/cmdstanpy/stanfit/runset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8502 2024-03-26 16:26:51.000000 cmdstanpy-1.2.2/cmdstanpy/stanfit/vb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:30:53.882465 cmdstanpy-1.2.2/cmdstanpy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-03-26 16:26:51.000000 cmdstanpy-1.2.2/cmdstanpy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19196 2024-03-26 16:26:51.000000 cmdstanpy-1.2.2/cmdstanpy/utils/cmdstan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-03-26 16:26:51.000000 cmdstanpy-1.2.2/cmdstanpy/utils/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-03-26 16:26:51.000000 cmdstanpy-1.2.2/cmdstanpy/utils/data_munging.py
--rw-r--r--   0 runner    (1001) docker     (127)     7099 2024-03-26 16:26:51.000000 cmdstanpy-1.2.2/cmdstanpy/utils/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-26 16:26:51.000000 cmdstanpy-1.2.2/cmdstanpy/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-03-26 16:26:51.000000 cmdstanpy-1.2.2/cmdstanpy/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    16190 2024-03-26 16:26:51.000000 cmdstanpy-1.2.2/cmdstanpy/utils/stancsv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:30:53.886464 cmdstanpy-1.2.2/cmdstanpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-03-26 16:30:53.000000 cmdstanpy-1.2.2/cmdstanpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-03-26 16:30:53.000000 cmdstanpy-1.2.2/cmdstanpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 16:30:53.000000 cmdstanpy-1.2.2/cmdstanpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-26 16:30:53.000000 cmdstanpy-1.2.2/cmdstanpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-26 16:30:53.000000 cmdstanpy-1.2.2/cmdstanpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-26 16:30:53.000000 cmdstanpy-1.2.2/cmdstanpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-03-26 16:30:51.000000 cmdstanpy-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 16:30:53.886464 cmdstanpy-1.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:30:53.886464 cmdstanpy-1.2.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)    25267 2024-03-26 16:26:51.000000 cmdstanpy-1.2.2/test/test_cmdstan_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     9097 2024-03-26 16:26:51.000000 cmdstanpy-1.2.2/test/test_compiler_opts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-03-26 16:26:51.000000 cmdstanpy-1.2.2/test/test_compliance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-03-26 16:26:51.000000 cmdstanpy-1.2.2/test/test_cxx_installation.py
--rw-r--r--   0 runner    (1001) docker     (127)    27310 2024-03-26 16:26:51.000000 cmdstanpy-1.2.2/test/test_generate_quantities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-03-26 16:26:51.000000 cmdstanpy-1.2.2/test/test_install_cmdstan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-03-26 16:26:51.000000 cmdstanpy-1.2.2/test/test_laplace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-03-26 16:26:51.000000 cmdstanpy-1.2.2/test/test_log_prob.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-03-26 16:26:51.000000 cmdstanpy-1.2.2/test/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    19705 2024-03-26 16:26:51.000000 cmdstanpy-1.2.2/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    21620 2024-03-26 16:26:51.000000 cmdstanpy-1.2.2/test/test_optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-03-26 16:30:51.000000 cmdstanpy-1.2.2/test/test_pathfinder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-03-26 16:26:51.000000 cmdstanpy-1.2.2/test/test_runset.py
--rw-r--r--   0 runner    (1001) docker     (127)    67104 2024-03-26 16:30:51.000000 cmdstanpy-1.2.2/test/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)    22746 2024-03-26 16:26:51.000000 cmdstanpy-1.2.2/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-03-26 16:26:51.000000 cmdstanpy-1.2.2/test/test_variational.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:16:58.155508 cmdstanpy-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-06-03 15:13:08.000000 cmdstanpy-1.2.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-06-03 15:13:08.000000 cmdstanpy-1.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-06-03 15:16:58.155508 cmdstanpy-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-06-03 15:13:08.000000 cmdstanpy-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:16:58.143508 cmdstanpy-1.2.3/cmdstanpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-06-03 15:13:08.000000 cmdstanpy-1.2.3/cmdstanpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-06-03 15:16:55.000000 cmdstanpy-1.2.3/cmdstanpy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39752 2024-06-03 15:13:08.000000 cmdstanpy-1.2.3/cmdstanpy/cmdstan_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20806 2024-06-03 15:13:08.000000 cmdstanpy-1.2.3/cmdstanpy/compilation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23553 2024-06-03 15:16:55.000000 cmdstanpy-1.2.3/cmdstanpy/install_cmdstan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11704 2024-06-03 15:16:55.000000 cmdstanpy-1.2.3/cmdstanpy/install_cxx_toolchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89660 2024-06-03 15:13:08.000000 cmdstanpy-1.2.3/cmdstanpy/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-06-03 15:13:08.000000 cmdstanpy-1.2.3/cmdstanpy/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:13:08.000000 cmdstanpy-1.2.3/cmdstanpy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:16:58.147508 cmdstanpy-1.2.3/cmdstanpy/stanfit/
+-rw-r--r--   0 runner    (1001) docker     (127)    10356 2024-06-03 15:13:08.000000 cmdstanpy-1.2.3/cmdstanpy/stanfit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26049 2024-06-03 15:13:08.000000 cmdstanpy-1.2.3/cmdstanpy/stanfit/gq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-06-03 15:13:08.000000 cmdstanpy-1.2.3/cmdstanpy/stanfit/laplace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31566 2024-06-03 15:13:08.000000 cmdstanpy-1.2.3/cmdstanpy/stanfit/mcmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-06-03 15:13:08.000000 cmdstanpy-1.2.3/cmdstanpy/stanfit/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10458 2024-06-03 15:13:08.000000 cmdstanpy-1.2.3/cmdstanpy/stanfit/mle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8322 2024-06-03 15:16:55.000000 cmdstanpy-1.2.3/cmdstanpy/stanfit/pathfinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-06-03 15:16:55.000000 cmdstanpy-1.2.3/cmdstanpy/stanfit/runset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8502 2024-06-03 15:13:08.000000 cmdstanpy-1.2.3/cmdstanpy/stanfit/vb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:16:58.147508 cmdstanpy-1.2.3/cmdstanpy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-06-03 15:13:08.000000 cmdstanpy-1.2.3/cmdstanpy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19196 2024-06-03 15:13:08.000000 cmdstanpy-1.2.3/cmdstanpy/utils/cmdstan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-06-03 15:13:08.000000 cmdstanpy-1.2.3/cmdstanpy/utils/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-06-03 15:13:08.000000 cmdstanpy-1.2.3/cmdstanpy/utils/data_munging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7099 2024-06-03 15:13:08.000000 cmdstanpy-1.2.3/cmdstanpy/utils/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-06-03 15:13:08.000000 cmdstanpy-1.2.3/cmdstanpy/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-06-03 15:13:08.000000 cmdstanpy-1.2.3/cmdstanpy/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16254 2024-06-03 15:16:55.000000 cmdstanpy-1.2.3/cmdstanpy/utils/stancsv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:16:58.151508 cmdstanpy-1.2.3/cmdstanpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-06-03 15:16:58.000000 cmdstanpy-1.2.3/cmdstanpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-06-03 15:16:58.000000 cmdstanpy-1.2.3/cmdstanpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 15:16:58.000000 cmdstanpy-1.2.3/cmdstanpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-06-03 15:16:58.000000 cmdstanpy-1.2.3/cmdstanpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-06-03 15:16:58.000000 cmdstanpy-1.2.3/cmdstanpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-03 15:16:58.000000 cmdstanpy-1.2.3/cmdstanpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-06-03 15:13:08.000000 cmdstanpy-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 15:16:58.155508 cmdstanpy-1.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:16:58.151508 cmdstanpy-1.2.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    25267 2024-06-03 15:13:08.000000 cmdstanpy-1.2.3/test/test_cmdstan_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9097 2024-06-03 15:13:08.000000 cmdstanpy-1.2.3/test/test_compiler_opts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-06-03 15:13:08.000000 cmdstanpy-1.2.3/test/test_compliance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-06-03 15:13:08.000000 cmdstanpy-1.2.3/test/test_cxx_installation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27310 2024-06-03 15:13:08.000000 cmdstanpy-1.2.3/test/test_generate_quantities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-06-03 15:13:08.000000 cmdstanpy-1.2.3/test/test_install_cmdstan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-06-03 15:13:08.000000 cmdstanpy-1.2.3/test/test_laplace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-06-03 15:13:08.000000 cmdstanpy-1.2.3/test/test_log_prob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-06-03 15:13:08.000000 cmdstanpy-1.2.3/test/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19705 2024-06-03 15:13:08.000000 cmdstanpy-1.2.3/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21649 2024-06-03 15:16:55.000000 cmdstanpy-1.2.3/test/test_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-06-03 15:13:08.000000 cmdstanpy-1.2.3/test/test_pathfinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-06-03 15:13:08.000000 cmdstanpy-1.2.3/test/test_runset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67147 2024-06-03 15:16:55.000000 cmdstanpy-1.2.3/test/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22746 2024-06-03 15:13:08.000000 cmdstanpy-1.2.3/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-06-03 15:13:08.000000 cmdstanpy-1.2.3/test/test_variational.py
```

### Comparing `cmdstanpy-1.2.2/LICENSE.md` & `cmdstanpy-1.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cmdstanpy-1.2.2/PKG-INFO` & `cmdstanpy-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmdstanpy
-Version: 1.2.2
+Version: 1.2.3
 Summary: Python interface to CmdStan
 Author: Stan Dev Team
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/stan-dev/cmdstanpy
 Project-URL: Bug Tracker, https://github.com/stan-dev/cmdstanpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `cmdstanpy-1.2.2/README.md` & `cmdstanpy-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `cmdstanpy-1.2.2/cmdstanpy/__init__.py` & `cmdstanpy-1.2.3/cmdstanpy/__init__.py`

 * *Files identical despite different names*

### Comparing `cmdstanpy-1.2.2/cmdstanpy/cmdstan_args.py` & `cmdstanpy-1.2.3/cmdstanpy/cmdstan_args.py`

 * *Files identical despite different names*

### Comparing `cmdstanpy-1.2.2/cmdstanpy/compilation.py` & `cmdstanpy-1.2.3/cmdstanpy/compilation.py`

 * *Files identical despite different names*

### Comparing `cmdstanpy-1.2.2/cmdstanpy/install_cmdstan.py` & `cmdstanpy-1.2.3/cmdstanpy/install_cmdstan.py`

 * *Files 1% similar despite different names*

```diff
@@ -519,14 +519,16 @@
     print('Download successful, file: {}'.format(file_tmp))
     try:
         print('Extracting distribution')
         tar = tarfile.open(file_tmp)
         first = tar.next()
         if first is not None:
             top_dir = first.name
+        else:
+            top_dir = ''
         cmdstan_dir = f'cmdstan-{version}'
         if top_dir != cmdstan_dir:
             raise CmdStanInstallError(
                 'tarfile should contain top-level dir {},'
                 'but found dir {} instead.'.format(cmdstan_dir, top_dir)
             )
         target = os.getcwd()
```

### Comparing `cmdstanpy-1.2.2/cmdstanpy/install_cxx_toolchain.py` & `cmdstanpy-1.2.3/cmdstanpy/install_cxx_toolchain.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,16 +231,18 @@
 def get_toolchain_name() -> str:
     """Return toolchain name."""
     if platform.system() == 'Windows':
         return 'RTools'
     return ''
 
 
+# TODO(2.0): drop 3.5 support
 def get_url(version: str) -> str:
     """Return URL for toolchain."""
+    url = ''
     if platform.system() == 'Windows':
         if version == '4.0':
             # pylint: disable=line-too-long
             if IS_64BITS:
                 url = 'https://cran.r-project.org/bin/windows/Rtools/rtools40-x86_64.exe'  # noqa: disable=E501
             else:
                 url = 'https://cran.r-project.org/bin/windows/Rtools/rtools40-i686.exe'  # noqa: disable=E501
@@ -273,14 +275,16 @@
     version = normalize_version(version)
     print("C++ toolchain '{}' version: {}".format(toolchain, version))
 
     url = get_url(version)
 
     if 'verbose' in args:
         verbose = args['verbose']
+    else:
+        verbose = False
 
     install_dir = args['dir']
     if install_dir is None:
         install_dir = os.path.expanduser(os.path.join('~', _DOT_CMDSTAN))
     validate_dir(install_dir)
     print('Install directory: {}'.format(install_dir))
```

### Comparing `cmdstanpy-1.2.2/cmdstanpy/model.py` & `cmdstanpy-1.2.3/cmdstanpy/model.py`

 * *Files identical despite different names*

### Comparing `cmdstanpy-1.2.2/cmdstanpy/progress.py` & `cmdstanpy-1.2.3/cmdstanpy/progress.py`

 * *Files identical despite different names*

### Comparing `cmdstanpy-1.2.2/cmdstanpy/stanfit/__init__.py` & `cmdstanpy-1.2.3/cmdstanpy/stanfit/__init__.py`

 * *Files identical despite different names*

### Comparing `cmdstanpy-1.2.2/cmdstanpy/stanfit/gq.py` & `cmdstanpy-1.2.3/cmdstanpy/stanfit/gq.py`

 * *Files identical despite different names*

### Comparing `cmdstanpy-1.2.2/cmdstanpy/stanfit/laplace.py` & `cmdstanpy-1.2.3/cmdstanpy/stanfit/laplace.py`

 * *Files identical despite different names*

### Comparing `cmdstanpy-1.2.2/cmdstanpy/stanfit/mcmc.py` & `cmdstanpy-1.2.3/cmdstanpy/stanfit/mcmc.py`

 * *Files identical despite different names*

### Comparing `cmdstanpy-1.2.2/cmdstanpy/stanfit/metadata.py` & `cmdstanpy-1.2.3/cmdstanpy/stanfit/metadata.py`

 * *Files identical despite different names*

### Comparing `cmdstanpy-1.2.2/cmdstanpy/stanfit/mle.py` & `cmdstanpy-1.2.3/cmdstanpy/stanfit/mle.py`

 * *Files identical despite different names*

### Comparing `cmdstanpy-1.2.2/cmdstanpy/stanfit/pathfinder.py` & `cmdstanpy-1.2.3/cmdstanpy/stanfit/pathfinder.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,16 +210,18 @@
     def is_resampled(self) -> bool:
         """
         Returns True if the draws were resampled from several Pathfinder
         approximations, False otherwise.
         """
         return (  # type: ignore
             self._metadata.cmdstan_config.get("num_paths", 4) > 1
-            and self._metadata.cmdstan_config.get('psis_resample', 1) == 1
-            and self._metadata.cmdstan_config.get('calculate_lp', 1) == 1
+            and self._metadata.cmdstan_config.get('psis_resample', 1)
+            in (1, 'true')
+            and self._metadata.cmdstan_config.get('calculate_lp', 1)
+            in (1, 'true')
         )
 
     def save_csvfiles(self, dir: Optional[str] = None) -> None:
         """
         Move output CSV files to specified directory.  If files were
         written to the temporary session directory, clean filename.
         E.g., save 'bernoulli-201912081451-1-5nm6as7u.csv' as
```

### Comparing `cmdstanpy-1.2.2/cmdstanpy/stanfit/runset.py` & `cmdstanpy-1.2.3/cmdstanpy/stanfit/runset.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,48 +57,48 @@
                 prefix=args.model_name, dir=_TMPDIR
             )
 
         # output files prefix: ``<model_name>-<YYYYMMDDHHMM>_<chain_id>``
         self._base_outfile = (
             f'{args.model_name}-{datetime.now().strftime(time_fmt)}'
         )
-        # per-process console messages
+        # per-process outputs
         self._stdout_files = [''] * self._num_procs
+        self._profile_files = [''] * self._num_procs  # optional
         if one_process_per_chain:
             for i in range(chains):
                 self._stdout_files[i] = self.file_path("-stdout.txt", id=i)
+                if args.save_profile:
+                    self._profile_files[i] = self.file_path(
+                        ".csv", extra="-profile", id=chain_ids[i]
+                    )
         else:
             self._stdout_files[0] = self.file_path("-stdout.txt")
+            if args.save_profile:
+                self._profile_files[0] = self.file_path(
+                    ".csv", extra="-profile"
+                )
 
         # per-chain output files
         self._csv_files: List[str] = [''] * chains
         self._diagnostic_files = [''] * chains  # optional
-        self._profile_files = [''] * chains  # optional
 
         if chains == 1:
             self._csv_files[0] = self.file_path(".csv")
             if args.save_latent_dynamics:
                 self._diagnostic_files[0] = self.file_path(
                     ".csv", extra="-diagnostic"
                 )
-            if args.save_profile:
-                self._profile_files[0] = self.file_path(
-                    ".csv", extra="-profile"
-                )
         else:
             for i in range(chains):
                 self._csv_files[i] = self.file_path(".csv", id=chain_ids[i])
                 if args.save_latent_dynamics:
                     self._diagnostic_files[i] = self.file_path(
                         ".csv", extra="-diagnostic", id=chain_ids[i]
                     )
-                if args.save_profile:
-                    self._profile_files[i] = self.file_path(
-                        ".csv", extra="-profile", id=chain_ids[i]
-                    )
 
     def __repr__(self) -> str:
         repr = 'RunSet: chains={}, chain_ids={}, num_processes={}'.format(
             self._chains, self._chain_ids, self._num_procs
         )
         repr = '{}\n cmd (chain 1):\n\t{}'.format(repr, self.cmd(0))
         repr = '{}\n retcodes={}'.format(repr, self._retcodes)
```

### Comparing `cmdstanpy-1.2.2/cmdstanpy/stanfit/vb.py` & `cmdstanpy-1.2.3/cmdstanpy/stanfit/vb.py`

 * *Files identical despite different names*

### Comparing `cmdstanpy-1.2.2/cmdstanpy/utils/__init__.py` & `cmdstanpy-1.2.3/cmdstanpy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cmdstanpy-1.2.2/cmdstanpy/utils/cmdstan.py` & `cmdstanpy-1.2.3/cmdstanpy/utils/cmdstan.py`

 * *Files identical despite different names*

### Comparing `cmdstanpy-1.2.2/cmdstanpy/utils/command.py` & `cmdstanpy-1.2.3/cmdstanpy/utils/command.py`

 * *Files identical despite different names*

### Comparing `cmdstanpy-1.2.2/cmdstanpy/utils/data_munging.py` & `cmdstanpy-1.2.3/cmdstanpy/utils/data_munging.py`

 * *Files identical despite different names*

### Comparing `cmdstanpy-1.2.2/cmdstanpy/utils/filesystem.py` & `cmdstanpy-1.2.3/cmdstanpy/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `cmdstanpy-1.2.2/cmdstanpy/utils/logging.py` & `cmdstanpy-1.2.3/cmdstanpy/utils/logging.py`

 * *Files identical despite different names*

### Comparing `cmdstanpy-1.2.2/cmdstanpy/utils/stancsv.py` & `cmdstanpy-1.2.3/cmdstanpy/utils/stancsv.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     if meta['draws_sampling'] != draws_sampling:
         raise ValueError(
             'bad Stan CSV file {}, expected {} draws, found {}'.format(
                 path, draws_sampling, meta['draws_sampling']
             )
         )
     if save_warmup:
-        if not ('save_warmup' in meta and meta['save_warmup'] == 1):
+        if not ('save_warmup' in meta and meta['save_warmup'] in (1, 'true')):
             raise ValueError(
                 'bad Stan CSV file {}, '
                 'config error, expected save_warmup = 1'.format(path)
             )
         if meta['draws_warmup'] != draws_warmup:
             raise ValueError(
                 'bad Stan CSV file {}, '
@@ -112,14 +112,15 @@
                     )
                 )
             xs = line.split(',')
             if save_iters:
                 all_iters[i, :] = [float(x) for x in xs]
             if i == iters - 1:
                 mle: np.ndarray = np.array(xs, dtype=float)
+    # pylint: disable=possibly-used-before-assignment
     dict['mle'] = mle
     if save_iters:
         dict['all_iters'] = all_iters
     return dict
 
 
 def scan_generic_csv(path: str) -> Dict[str, Any]:
```

### Comparing `cmdstanpy-1.2.2/cmdstanpy.egg-info/PKG-INFO` & `cmdstanpy-1.2.3/cmdstanpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmdstanpy
-Version: 1.2.2
+Version: 1.2.3
 Summary: Python interface to CmdStan
 Author: Stan Dev Team
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/stan-dev/cmdstanpy
 Project-URL: Bug Tracker, https://github.com/stan-dev/cmdstanpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `cmdstanpy-1.2.2/cmdstanpy.egg-info/SOURCES.txt` & `cmdstanpy-1.2.3/cmdstanpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cmdstanpy-1.2.2/pyproject.toml` & `cmdstanpy-1.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cmdstanpy-1.2.2/test/test_cmdstan_args.py` & `cmdstanpy-1.2.3/test/test_cmdstan_args.py`

 * *Files identical despite different names*

### Comparing `cmdstanpy-1.2.2/test/test_compiler_opts.py` & `cmdstanpy-1.2.3/test/test_compiler_opts.py`

 * *Files identical despite different names*

### Comparing `cmdstanpy-1.2.2/test/test_compliance.py` & `cmdstanpy-1.2.3/test/test_compliance.py`

 * *Files identical despite different names*

### Comparing `cmdstanpy-1.2.2/test/test_cxx_installation.py` & `cmdstanpy-1.2.3/test/test_cxx_installation.py`

 * *Files identical despite different names*

### Comparing `cmdstanpy-1.2.2/test/test_generate_quantities.py` & `cmdstanpy-1.2.3/test/test_generate_quantities.py`

 * *Files identical despite different names*

### Comparing `cmdstanpy-1.2.2/test/test_install_cmdstan.py` & `cmdstanpy-1.2.3/test/test_install_cmdstan.py`

 * *Files identical despite different names*

### Comparing `cmdstanpy-1.2.2/test/test_laplace.py` & `cmdstanpy-1.2.3/test/test_laplace.py`

 * *Files identical despite different names*

### Comparing `cmdstanpy-1.2.2/test/test_log_prob.py` & `cmdstanpy-1.2.3/test/test_log_prob.py`

 * *Files identical despite different names*

### Comparing `cmdstanpy-1.2.2/test/test_metadata.py` & `cmdstanpy-1.2.3/test/test_metadata.py`

 * *Files identical despite different names*

### Comparing `cmdstanpy-1.2.2/test/test_model.py` & `cmdstanpy-1.2.3/test/test_model.py`

 * *Files identical despite different names*

### Comparing `cmdstanpy-1.2.2/test/test_optimize.py` & `cmdstanpy-1.2.3/test/test_optimize.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,20 +258,21 @@
         tol_rel_grad=1e7,
         tol_param=1e-8,
         history_size=5,
         save_iterations=True,
     )
     vars_iters = multidim_mle_iters.stan_variables(inc_iterations=True)
     assert len(vars_iters) == len(multidim_mle_iters.metadata.stan_vars)
+    assert 'frac_60' in vars_iters
+    n_iter = vars_iters['frac_60'].shape[0]
+    assert n_iter > 1
     assert 'y_rep' in vars_iters
-    assert vars_iters['y_rep'].shape == (8, 5, 4, 3)
+    assert vars_iters['y_rep'].shape == (n_iter, 5, 4, 3)
     assert 'beta' in vars_iters
-    assert vars_iters['beta'].shape == (8, 2)
-    assert 'frac_60' in vars_iters
-    assert vars_iters['frac_60'].shape == (8,)
+    assert vars_iters['beta'].shape == (n_iter, 2)
 
 
 def test_optimize_good() -> None:
     stan = os.path.join(DATAFILES_PATH, 'bernoulli.stan')
     model = CmdStanModel(stan_file=stan)
     jdata = os.path.join(DATAFILES_PATH, 'bernoulli.data.json')
     jinit = os.path.join(DATAFILES_PATH, 'bernoulli.init.json')
```

### Comparing `cmdstanpy-1.2.2/test/test_pathfinder.py` & `cmdstanpy-1.2.3/test/test_pathfinder.py`

 * *Files identical despite different names*

### Comparing `cmdstanpy-1.2.2/test/test_runset.py` & `cmdstanpy-1.2.3/test/test_runset.py`

 * *Files identical despite different names*

### Comparing `cmdstanpy-1.2.2/test/test_sample.py` & `cmdstanpy-1.2.3/test/test_sample.py`

 * *Files 2% similar despite different names*

```diff
@@ -1744,41 +1744,44 @@
     for i in range(bern_fit.runset.chains):
         diagnostics_file = bern_fit.runset.diagnostic_files[i]
         assert os.path.exists(diagnostics_file)
 
 
 def test_save_profile() -> None:
     stan = os.path.join(DATAFILES_PATH, 'profile_likelihood.stan')
-    profile_model = CmdStanModel(stan_file=stan)
+    profile_model = CmdStanModel(
+        stan_file=stan, cpp_options={"STAN_THREADS": '1'}, force_compile=True
+    )
+
     profile_fit = profile_model.sample(
         chains=2,
         parallel_chains=2,
+        force_one_process_per_chain=True,
         seed=12345,
         iter_warmup=100,
         iter_sampling=200,
         save_profile=True,
     )
-    for i in range(profile_fit.runset.chains):
-        profile_file = profile_fit.runset.profile_files[i]
+    assert len(profile_fit.runset.profile_files) == 2
+    for profile_file in profile_fit.runset.profile_files:
         assert os.path.exists(profile_file)
 
     profile_fit = profile_model.sample(
         chains=2,
         parallel_chains=2,
+        force_one_process_per_chain=False,
         seed=12345,
+        iter_warmup=100,
         iter_sampling=200,
-        save_latent_dynamics=True,
         save_profile=True,
     )
 
-    for i in range(profile_fit.runset.chains):
-        profile_file = profile_fit.runset.profile_files[i]
+    assert len(profile_fit.runset.profile_files) == 1
+    for profile_file in profile_fit.runset.profile_files:
         assert os.path.exists(profile_file)
-        diagnostics_file = profile_fit.runset.diagnostic_files[i]
-        assert os.path.exists(diagnostics_file)
 
 
 def test_xarray_draws() -> None:
     stan = os.path.join(DATAFILES_PATH, 'bernoulli.stan')
     jdata = os.path.join(DATAFILES_PATH, 'bernoulli.data.json')
     bern_model = CmdStanModel(stan_file=stan)
     bern_fit = bern_model.sample(
```

### Comparing `cmdstanpy-1.2.2/test/test_utils.py` & `cmdstanpy-1.2.3/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `cmdstanpy-1.2.2/test/test_variational.py` & `cmdstanpy-1.2.3/test/test_variational.py`

 * *Files identical despite different names*

