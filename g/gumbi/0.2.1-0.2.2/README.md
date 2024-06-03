# Comparing `tmp/gumbi-0.2.1.tar.gz` & `tmp/gumbi-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gumbi-0.2.1.tar", last modified: Mon May  1 01:21:06 2023, max compression
+gzip compressed data, was "gumbi-0.2.2.tar", last modified: Sun Jun  2 00:30:20 2024, max compression
```

## Comparing `gumbi-0.2.1.tar` & `gumbi-0.2.2.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:21:06.287999 gumbi-0.2.1/
--rw-r--r--   0 john      (1000) john      (1000)    11357 2022-10-14 20:45:47.000000 gumbi-0.2.1/LICENSE
--rw-r--r--   0 john      (1000) john      (1000)      235 2022-10-14 20:45:47.000000 gumbi-0.2.1/MANIFEST.in
--rw-r--r--   0 john      (1000) john      (1000)     3045 2023-05-01 01:21:06.287999 gumbi-0.2.1/PKG-INFO
--rw-r--r--   0 john      (1000) john      (1000)     2225 2023-05-01 01:03:42.000000 gumbi-0.2.1/README.md
--rw-r--r--   0 john      (1000) john      (1000)        5 2023-05-01 01:20:41.000000 gumbi-0.2.1/VERSION
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:21:06.222998 gumbi-0.2.1/docs/
--rw-r--r--   0 john      (1000) john      (1000)      122 2023-05-01 01:03:42.000000 gumbi-0.2.1/docs/requirements.txt
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:21:06.222998 gumbi-0.2.1/docs/source/
--rw-r--r--   0 john      (1000) john      (1000)     2829 2023-05-01 01:03:42.000000 gumbi-0.2.1/docs/source/conf.py
--rw-r--r--   0 john      (1000) john      (1000)      620 2022-10-14 20:45:47.000000 gumbi-0.2.1/docs/source/index.rst
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:21:06.212165 gumbi-0.2.1/docs/source/notebooks/
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:21:06.266332 gumbi-0.2.1/docs/source/notebooks/examples/
--rw-r--r--   0 john      (1000) john      (1000)  1505160 2023-05-01 01:03:42.000000 gumbi-0.2.1/docs/source/notebooks/examples/Cars_Dataset.ipynb
--rw-r--r--   0 john      (1000) john      (1000)  2084410 2023-05-01 01:03:42.000000 gumbi-0.2.1/docs/source/notebooks/examples/Latent_GP.ipynb
--rw-r--r--   0 john      (1000) john      (1000)   423694 2023-05-01 01:03:42.000000 gumbi-0.2.1/docs/source/notebooks/examples/Multioutput_Regression.ipynb
--rw-r--r--   0 john      (1000) john      (1000)   440843 2023-05-01 01:03:42.000000 gumbi-0.2.1/docs/source/notebooks/examples/Simple_Regression.ipynb
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:21:06.277165 gumbi-0.2.1/docs/source/notebooks/getting_started/
--rw-r--r--   0 john      (1000) john      (1000)    41212 2023-05-01 01:20:41.000000 gumbi-0.2.1/docs/source/notebooks/getting_started/introduction.ipynb
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:21:06.277165 gumbi-0.2.1/gumbi/
--rw-r--r--   0 john      (1000) john      (1000)      402 2023-05-01 01:03:42.000000 gumbi-0.2.1/gumbi/__init__.py
--rw-r--r--   0 john      (1000) john      (1000)    33679 2023-04-30 03:43:08.000000 gumbi-0.2.1/gumbi/aggregation.py
--rw-r--r--   0 john      (1000) john      (1000)    57752 2023-05-01 01:03:42.000000 gumbi-0.2.1/gumbi/arrays.py
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:21:06.287999 gumbi-0.2.1/gumbi/data/
--rw-r--r--   0 john      (1000) john      (1000)   552642 2022-10-14 20:45:47.000000 gumbi-0.2.1/gumbi/data/Example_DataSet.pkl
--rw-r--r--   0 john      (1000) john      (1000)      136 2022-10-14 20:45:47.000000 gumbi-0.2.1/gumbi/data/__init__.py
--rw-r--r--   0 john      (1000) john      (1000)    16993 2023-05-01 01:03:42.000000 gumbi-0.2.1/gumbi/plotting.py
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:21:06.287999 gumbi-0.2.1/gumbi/regression/
--rw-r--r--   0 john      (1000) john      (1000)      124 2023-05-01 01:03:42.000000 gumbi-0.2.1/gumbi/regression/__init__.py
--rw-r--r--   0 john      (1000) john      (1000)    52481 2023-04-10 19:27:45.000000 gumbi-0.2.1/gumbi/regression/base.py
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:21:06.287999 gumbi-0.2.1/gumbi/regression/pymc/
--rw-r--r--   0 john      (1000) john      (1000)    37223 2023-05-01 01:20:41.000000 gumbi-0.2.1/gumbi/regression/pymc/GP.py
--rw-r--r--   0 john      (1000) john      (1000)        0 2023-05-01 01:03:42.000000 gumbi-0.2.1/gumbi/regression/pymc/__init__.py
--rw-r--r--   0 john      (1000) john      (1000)     1858 2023-05-01 01:03:42.000000 gumbi-0.2.1/gumbi/regression/pymc/extras.py
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:21:06.287999 gumbi-0.2.1/gumbi/style/
--rw-r--r--   0 john      (1000) john      (1000)      236 2022-10-14 20:45:47.000000 gumbi-0.2.1/gumbi/style/__init__.py
--rw-r--r--   0 john      (1000) john      (1000)    33984 2022-10-14 20:45:47.000000 gumbi-0.2.1/gumbi/style/breve_presentation.mplstyle
--rw-r--r--   0 john      (1000) john      (1000)    33956 2022-10-14 20:45:47.000000 gumbi-0.2.1/gumbi/style/futura_presentation.mplstyle
--rw-r--r--   0 john      (1000) john      (1000)    33945 2022-10-14 20:45:47.000000 gumbi-0.2.1/gumbi/style/presentation.mplstyle
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:21:06.287999 gumbi-0.2.1/gumbi/utils/
--rw-r--r--   0 john      (1000) john      (1000)       76 2022-10-14 20:45:47.000000 gumbi-0.2.1/gumbi/utils/__init__.py
--rw-r--r--   0 john      (1000) john      (1000)     2031 2022-10-14 20:45:47.000000 gumbi-0.2.1/gumbi/utils/generic_utils.py
--rw-r--r--   0 john      (1000) john      (1000)      385 2022-10-14 20:45:47.000000 gumbi-0.2.1/gumbi/utils/gp_utils.py
--rw-r--r--   0 john      (1000) john      (1000)     3214 2022-10-14 20:45:47.000000 gumbi-0.2.1/gumbi/utils/misc.py
--rw-r--r--   0 john      (1000) john      (1000)     1414 2023-05-01 01:03:42.000000 gumbi-0.2.1/gumbi/utils/pymc_utils.py
--rw-r--r--   0 john      (1000) john      (1000)      222 2022-10-14 20:45:47.000000 gumbi-0.2.1/gumbi/versions.py
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:21:06.277165 gumbi-0.2.1/gumbi.egg-info/
--rw-r--r--   0 john      (1000) john      (1000)     3045 2023-05-01 01:21:06.000000 gumbi-0.2.1/gumbi.egg-info/PKG-INFO
--rw-r--r--   0 john      (1000) john      (1000)     1248 2023-05-01 01:21:06.000000 gumbi-0.2.1/gumbi.egg-info/SOURCES.txt
--rw-r--r--   0 john      (1000) john      (1000)        1 2023-05-01 01:21:06.000000 gumbi-0.2.1/gumbi.egg-info/dependency_links.txt
--rw-r--r--   0 john      (1000) john      (1000)       77 2023-05-01 01:21:06.000000 gumbi-0.2.1/gumbi.egg-info/requires.txt
--rw-r--r--   0 john      (1000) john      (1000)       12 2023-05-01 01:21:06.000000 gumbi-0.2.1/gumbi.egg-info/top_level.txt
--rw-r--r--   0 john      (1000) john      (1000)      213 2022-10-14 20:45:47.000000 gumbi-0.2.1/pyproject.toml
--rw-r--r--   0 john      (1000) john      (1000)      104 2023-05-01 01:03:42.000000 gumbi-0.2.1/requirements.txt
--rw-r--r--   0 john      (1000) john      (1000)      199 2023-05-01 01:21:06.287999 gumbi-0.2.1/setup.cfg
--rw-r--r--   0 john      (1000) john      (1000)     1679 2023-05-01 01:03:42.000000 gumbi-0.2.1/setup.py
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:21:06.287999 gumbi-0.2.1/tests/
--rw-r--r--   0 john      (1000) john      (1000)        0 2022-10-14 20:45:47.000000 gumbi-0.2.1/tests/__init__.py
--rw-r--r--   0 john      (1000) john      (1000)      615 2022-10-14 20:45:47.000000 gumbi-0.2.1/tests/conftest.py
--rw-r--r--   0 john      (1000) john      (1000)     3983 2022-10-14 20:45:47.000000 gumbi-0.2.1/tests/test_aggregation.py
--rw-r--r--   0 john      (1000) john      (1000)     6873 2023-05-01 01:03:42.000000 gumbi-0.2.1/tests/test_arrays.py
--rw-r--r--   0 john      (1000) john      (1000)     4031 2023-05-01 01:03:42.000000 gumbi-0.2.1/tests/test_plots.py
--rw-r--r--   0 john      (1000) john      (1000)     6391 2023-05-01 01:03:42.000000 gumbi-0.2.1/tests/test_regression.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-02 00:30:20.747202 gumbi-0.2.2/
+-rw-r--r--   0 john      (1000) john      (1000)    11357 2024-01-03 05:03:41.000000 gumbi-0.2.2/LICENSE
+-rw-r--r--   0 john      (1000) john      (1000)      235 2024-01-03 05:03:41.000000 gumbi-0.2.2/MANIFEST.in
+-rw-r--r--   0 john      (1000) john      (1000)     3242 2024-06-02 00:30:20.747202 gumbi-0.2.2/PKG-INFO
+-rw-r--r--   0 john      (1000) john      (1000)     2225 2024-01-03 05:03:41.000000 gumbi-0.2.2/README.md
+-rw-r--r--   0 john      (1000) john      (1000)        5 2024-06-02 00:27:06.000000 gumbi-0.2.2/VERSION
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-02 00:30:20.737202 gumbi-0.2.2/docs/
+-rw-r--r--   0 john      (1000) john      (1000)      122 2024-01-03 05:03:41.000000 gumbi-0.2.2/docs/requirements.txt
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-02 00:30:20.737202 gumbi-0.2.2/docs/source/
+-rw-r--r--   0 john      (1000) john      (1000)     2829 2024-01-03 05:03:41.000000 gumbi-0.2.2/docs/source/conf.py
+-rw-r--r--   0 john      (1000) john      (1000)      620 2024-01-03 05:03:41.000000 gumbi-0.2.2/docs/source/index.rst
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-02 00:30:20.727202 gumbi-0.2.2/docs/source/notebooks/
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-02 00:30:20.737202 gumbi-0.2.2/docs/source/notebooks/examples/
+-rw-r--r--   0 john      (1000) john      (1000)  1505160 2024-01-03 05:03:41.000000 gumbi-0.2.2/docs/source/notebooks/examples/Cars_Dataset.ipynb
+-rw-r--r--   0 john      (1000) john      (1000)  2084410 2024-05-31 21:25:49.000000 gumbi-0.2.2/docs/source/notebooks/examples/Latent_GP.ipynb
+-rw-r--r--   0 john      (1000) john      (1000)   423694 2024-01-03 05:03:41.000000 gumbi-0.2.2/docs/source/notebooks/examples/Multioutput_Regression.ipynb
+-rw-r--r--   0 john      (1000) john      (1000)   440843 2024-01-03 05:03:41.000000 gumbi-0.2.2/docs/source/notebooks/examples/Simple_Regression.ipynb
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-02 00:30:20.737202 gumbi-0.2.2/docs/source/notebooks/getting_started/
+-rw-r--r--   0 john      (1000) john      (1000)    41212 2024-01-03 05:03:41.000000 gumbi-0.2.2/docs/source/notebooks/getting_started/introduction.ipynb
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-02 00:30:20.737202 gumbi-0.2.2/gumbi/
+-rw-r--r--   0 john      (1000) john      (1000)      430 2024-05-31 19:44:55.000000 gumbi-0.2.2/gumbi/__init__.py
+-rw-r--r--   0 john      (1000) john      (1000)    35001 2024-05-31 21:13:11.000000 gumbi-0.2.2/gumbi/aggregation.py
+-rw-r--r--   0 john      (1000) john      (1000)     1177 2024-05-31 19:45:21.000000 gumbi-0.2.2/gumbi/array_utils.py
+-rw-r--r--   0 john      (1000) john      (1000)    57761 2024-01-10 20:10:43.000000 gumbi-0.2.2/gumbi/arrays.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-02 00:30:20.737202 gumbi-0.2.2/gumbi/data/
+-rw-r--r--   0 john      (1000) john      (1000)   552642 2024-01-03 05:03:41.000000 gumbi-0.2.2/gumbi/data/Example_DataSet.pkl
+-rw-r--r--   0 john      (1000) john      (1000)      136 2024-01-03 05:03:41.000000 gumbi-0.2.2/gumbi/data/__init__.py
+-rw-r--r--   0 john      (1000) john      (1000)    16993 2024-01-03 05:03:41.000000 gumbi-0.2.2/gumbi/plotting.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-02 00:30:20.737202 gumbi-0.2.2/gumbi/regression/
+-rw-r--r--   0 john      (1000) john      (1000)      124 2024-01-03 05:03:41.000000 gumbi-0.2.2/gumbi/regression/__init__.py
+-rw-r--r--   0 john      (1000) john      (1000)    52482 2024-06-02 00:26:25.000000 gumbi-0.2.2/gumbi/regression/base.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-02 00:30:20.737202 gumbi-0.2.2/gumbi/regression/pymc/
+-rw-r--r--   0 john      (1000) john      (1000)    38929 2024-05-31 20:12:23.000000 gumbi-0.2.2/gumbi/regression/pymc/GP.py
+-rw-r--r--   0 john      (1000) john      (1000)        0 2024-01-03 05:03:41.000000 gumbi-0.2.2/gumbi/regression/pymc/__init__.py
+-rw-r--r--   0 john      (1000) john      (1000)     1858 2024-01-03 05:03:41.000000 gumbi-0.2.2/gumbi/regression/pymc/extras.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-02 00:30:20.737202 gumbi-0.2.2/gumbi/style/
+-rw-r--r--   0 john      (1000) john      (1000)      236 2024-01-03 05:03:41.000000 gumbi-0.2.2/gumbi/style/__init__.py
+-rw-r--r--   0 john      (1000) john      (1000)    33984 2024-01-03 05:03:41.000000 gumbi-0.2.2/gumbi/style/breve_presentation.mplstyle
+-rw-r--r--   0 john      (1000) john      (1000)    33956 2024-01-03 05:03:41.000000 gumbi-0.2.2/gumbi/style/futura_presentation.mplstyle
+-rw-r--r--   0 john      (1000) john      (1000)    33945 2024-01-03 05:03:41.000000 gumbi-0.2.2/gumbi/style/presentation.mplstyle
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-02 00:30:20.737202 gumbi-0.2.2/gumbi/utils/
+-rw-r--r--   0 john      (1000) john      (1000)       76 2024-01-03 05:03:41.000000 gumbi-0.2.2/gumbi/utils/__init__.py
+-rw-r--r--   0 john      (1000) john      (1000)     2031 2024-01-03 05:03:41.000000 gumbi-0.2.2/gumbi/utils/generic_utils.py
+-rw-r--r--   0 john      (1000) john      (1000)     1920 2024-05-31 19:45:39.000000 gumbi-0.2.2/gumbi/utils/gp_utils.py
+-rw-r--r--   0 john      (1000) john      (1000)     6044 2024-05-31 15:00:57.000000 gumbi-0.2.2/gumbi/utils/misc.py
+-rw-r--r--   0 john      (1000) john      (1000)     1414 2024-01-03 05:03:41.000000 gumbi-0.2.2/gumbi/utils/pymc_utils.py
+-rw-r--r--   0 john      (1000) john      (1000)      222 2024-01-03 05:03:41.000000 gumbi-0.2.2/gumbi/versions.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-02 00:30:20.747202 gumbi-0.2.2/gumbi.egg-info/
+-rw-r--r--   0 john      (1000) john      (1000)     3242 2024-06-02 00:30:20.000000 gumbi-0.2.2/gumbi.egg-info/PKG-INFO
+-rw-r--r--   0 john      (1000) john      (1000)     1269 2024-06-02 00:30:20.000000 gumbi-0.2.2/gumbi.egg-info/SOURCES.txt
+-rw-r--r--   0 john      (1000) john      (1000)        1 2024-06-02 00:30:20.000000 gumbi-0.2.2/gumbi.egg-info/dependency_links.txt
+-rw-r--r--   0 john      (1000) john      (1000)       77 2024-06-02 00:30:20.000000 gumbi-0.2.2/gumbi.egg-info/requires.txt
+-rw-r--r--   0 john      (1000) john      (1000)       12 2024-06-02 00:30:20.000000 gumbi-0.2.2/gumbi.egg-info/top_level.txt
+-rw-r--r--   0 john      (1000) john      (1000)      213 2024-01-03 05:03:41.000000 gumbi-0.2.2/pyproject.toml
+-rw-r--r--   0 john      (1000) john      (1000)      104 2024-01-03 05:03:41.000000 gumbi-0.2.2/requirements.txt
+-rw-r--r--   0 john      (1000) john      (1000)      205 2024-06-02 00:30:20.747202 gumbi-0.2.2/setup.cfg
+-rw-r--r--   0 john      (1000) john      (1000)     1735 2024-06-02 00:30:14.000000 gumbi-0.2.2/setup.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-02 00:30:20.747202 gumbi-0.2.2/tests/
+-rw-r--r--   0 john      (1000) john      (1000)        0 2024-01-03 05:03:41.000000 gumbi-0.2.2/tests/__init__.py
+-rw-r--r--   0 john      (1000) john      (1000)      615 2024-01-03 05:03:41.000000 gumbi-0.2.2/tests/conftest.py
+-rw-r--r--   0 john      (1000) john      (1000)     3983 2024-01-03 05:03:41.000000 gumbi-0.2.2/tests/test_aggregation.py
+-rw-r--r--   0 john      (1000) john      (1000)     6873 2024-01-03 05:03:41.000000 gumbi-0.2.2/tests/test_arrays.py
+-rw-r--r--   0 john      (1000) john      (1000)     4031 2024-01-03 05:03:41.000000 gumbi-0.2.2/tests/test_plots.py
+-rw-r--r--   0 john      (1000) john      (1000)     6391 2024-01-03 05:03:41.000000 gumbi-0.2.2/tests/test_regression.py
```

### Comparing `gumbi-0.2.1/LICENSE` & `gumbi-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.1/PKG-INFO` & `gumbi-0.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gumbi
-Version: 0.2.1
+Version: 0.2.2
 Summary: Gaussian Process Model Building Interface
 Home-page: https://github.com/JohnGoertz/Gumbi
 Author: John Goertz
 Author-email: 
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -17,14 +17,22 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas>=1.2.3
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: seaborn
+Requires-Dist: matplotlib
+Requires-Dist: pymc>=5.3.1
+Requires-Dist: arviz
+Requires-Dist: uncertainties
 
 # Gumbi: Gaussian Process Model Building Interface
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/JohnGoertz/Gumbi/HEAD)
 
 ## Overview
```

### Comparing `gumbi-0.2.1/README.md` & `gumbi-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.1/docs/source/conf.py` & `gumbi-0.2.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.1/docs/source/index.rst` & `gumbi-0.2.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.1/docs/source/notebooks/examples/Cars_Dataset.ipynb` & `gumbi-0.2.2/docs/source/notebooks/examples/Cars_Dataset.ipynb`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.1/docs/source/notebooks/examples/Latent_GP.ipynb` & `gumbi-0.2.2/docs/source/notebooks/examples/Latent_GP.ipynb`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.1/docs/source/notebooks/examples/Multioutput_Regression.ipynb` & `gumbi-0.2.2/docs/source/notebooks/examples/Multioutput_Regression.ipynb`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.1/docs/source/notebooks/examples/Simple_Regression.ipynb` & `gumbi-0.2.2/docs/source/notebooks/examples/Simple_Regression.ipynb`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.1/docs/source/notebooks/getting_started/introduction.ipynb` & `gumbi-0.2.2/docs/source/notebooks/getting_started/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.1/gumbi/aggregation.py` & `gumbi-0.2.2/gumbi/aggregation.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,58 +5,68 @@
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 
 import numpy as np
 import pandas as pd
 from scipy.special import expit, logit
 
-from .utils import skip
+from .utils import skip, listify
 
 __all__ = ["Standardizer", "TidyData", "WideData", "DataSet"]
 
 
 class Standardizer(dict):
     r"""Container for dict of mean (μ) and variance (σ2) for every parameter.
 
-    :class:`Standardizer` objects allow transformation and normalization of datasets. The main methods are :meth:`stdz`,
-    which attempts to coerce the values of a given variable to a standard normal distribution (`z-scores`), and its
-    complement :meth:`unstdz`. The steps are
+    :class:`Standardizer` objects allow transformation and normalization of
+    datasets. The main methods are :meth:`stdz`, which attempts to coerce the
+    values of a given variable to a standard normal distribution (`z-scores`),
+    and its complement :meth:`unstdz`. The steps are
 
     .. math::
         \mathbf{\text{tidy}} \rightarrow \text{transform} \rightarrow \text{mean-center} \rightarrow \text{scale}
         \rightarrow \mathbf{\text{tidy.z}}
 
-    For example, reaction `rate` must clearly be strictly positive, so we use a `log` transformation so that it behaves
-    as a normally-distributed random variable. We then mean-center and scale this transformed value to obtain `z-scores`
-    indicating how similar a given estimate is to all the other estimates we've observed. `Standardizer` stores the
-    transforms and population mean and variance for every parameter, allowing us to convert back and forth
-    between natural space (:math:`rate`), transformed space (:math:`\text{ln}\; rate`), and standardized space
-    (:math:`\left( \text{ln}\; rate  - \mu_{\text{ln}\; rate} \right)/\sigma_{\text{ln}\; rate}`).
-
-    Typically, a :class:`Standardizer` will be constructed from a dataframe (:meth:`from_DataFrame`),
-    but the individual means and variances can be provided at instantiation as well. Note, however,
-    that these should be the mean/std of the *transformed* variable. For example, if `r` should be treated as
-    log-normal with a natural-space mean of 1 and variance of 0.1, the right way to instantiate the class
-    would be `Standardizer(d={'μ': 0, 'σ2': 0.1}, log_vars=['d'])`.
+    For example, reaction `rate` must clearly be strictly positive, so we use a
+    `log` transformation so that it behaves as a normally-distributed random
+    variable. We then mean-center and scale this transformed value to obtain
+    `z-scores` indicating how similar a given estimate is to all the other
+    estimates we've observed. `Standardizer` stores the transforms and
+    population mean and variance for every parameter, allowing us to convert
+    back and forth between natural space (:math:`rate`), transformed space
+    (:math:`\text{ln}\; rate`), and standardized space (:math:`\left(
+    \text{ln}\; rate  - \mu_{\text{ln}\; rate} \right)/\sigma_{\text{ln}\;
+    rate}`).
+
+    Typically, a :class:`Standardizer` will be constructed from a dataframe
+    (:meth:`from_DataFrame`), but the individual means and variances can be
+    provided at instantiation as well. Note, however, that these should be the
+    mean/std of the *transformed* variable. For example, if `r` should be
+    treated as log-normal with a natural-space mean of 1 and variance of 0.1,
+    the right way to instantiate the class would be `Standardizer(d={'μ': 0,
+    'σ2': 0.1}, log_vars=['d'])`.
 
 
     Notes
     -----
-    :class:`Standardizer` is just a `dictionary <https://docs.python.org/3/tutorial/datastructures.html#dictionaries>`_
-    with some extra methods and defaults, so standard dictionary methods like :meth:`dict.update` still work.
+    :class:`Standardizer` is just a `dictionary
+    <https://docs.python.org/3/tutorial/datastructures.html#dictionaries>`_ with
+    some extra methods and defaults, so standard dictionary methods like
+    :meth:`dict.update` still work.
 
 
     Parameters
     ----------
     log_vars: list, optional
         List of input and output variables to be treated as log-normal.
     logit_vars: list, optional
         List of input and output variables to be treated as logit-normal.
     **kwargs
-        Mean and variance of each variable as a dictionary, e.g. d={'μ': 0, 'σ2': 0.1}
+        Mean and variance of each variable as a dictionary, e.g. d={'μ': 0,
+        'σ2': 0.1}
 
 
     Examples
     --------
     >>> import numpy as np
     >>> import pandas as pd
     >>> from gumbi import Standardizer
@@ -105,17 +115,18 @@
     1    2.191924
     2    3.474117
     3    4.383848
     Name: r, dtype: float64
 
     """
 
-    # TODO: Standardizer: make transform suggestions based on provided tidy? e.g., all>0 -> log/exp
+    # TODO: Standardizer: make transform suggestions based on provided tidy?
+    # e.g., all>0 -> log/exp
 
-    def __init__(self, log_vars=None, logit_vars=None, **kwargs):
+    def __init__(self, log_vars=None, logit_vars=None, isotropic_vars=None, **kwargs):
         self.validate(kwargs)
         for name, stats in kwargs.items():
             if "σ2" not in stats:
                 stats["σ2"] = stats["σ"] ** 2
                 del stats["σ"]
         super().__init__(**kwargs)
         self._transforms = {var: [skip, skip] for var in kwargs.keys()}
@@ -125,16 +136,17 @@
                 raise TypeError("log_vars must be a list or str")
             self._transforms.update({var: [np.log, np.exp] for var in log_vars})
         if logit_vars is not None:
             logit_vars = [logit_vars] if isinstance(logit_vars, str) else logit_vars
             if not isinstance(logit_vars, list):
                 raise TypeError("logit_vars must be a list or str")
             self._transforms.update({var: [logit, expit] for var in logit_vars})
-        self._log_vars = log_vars if log_vars is not None else []
-        self._logit_vars = logit_vars if logit_vars is not None else []
+        self._log_vars = listify(log_vars)
+        self._logit_vars = listify(logit_vars)
+        self._isotropic_vars = listify(isotropic_vars)
 
     def __or__(self, __dct) -> Standardizer:
         # new_dct = super().__or__(__dct)  # Use when Python>=3.9
         new_dct = {**self, **__dct}
         stdzr = Standardizer(**new_dct)
         if isinstance(__dct, Standardizer):
             stdzr.transforms = {
@@ -189,15 +201,16 @@
         if not isinstance(var_list, list):
             raise TypeError("logit_vars must be a list or str")
         self._logit_vars = var_list
         self._transforms.update({var: [logit, expit] for var in var_list})  # Fix once Python >= 3.9
 
     @property
     def transforms(self) -> dict:
-        """Collection of forward and reverse transform functions for each variable"""
+        """Collection of forward and reverse transform functions for each
+        variable"""
         return self._transforms
 
     @transforms.setter
     def transforms(self, dct) -> dict:
         self._transforms = dct
         self._log_vars = [v for v, lst in dct.items() if lst[0] is np.log]
         self._logit_vars = [v for v, lst in dct.items() if lst[0] is logit]
@@ -205,46 +218,68 @@
     @classmethod
     def validate(cls, dct: dict):
         """Ensures provided dictionary has all required attributes"""
         assert all("μ" in sub.keys() for sub in dct.values())
         assert all(("σ" in sub.keys() or "σ2" in sub.keys()) for sub in dct.values())
 
     @classmethod
-    def from_DataFrame(cls, df: pd.DataFrame, log_vars=None, logit_vars=None):
+    def from_DataFrame(cls, df: pd.DataFrame, log_vars=None, logit_vars=None, isotropic_vars=None):
         """Construct from wide-form DataFrame"""
+        isotropic_vars = listify(isotropic_vars)
+        
         float_columns = df.dtypes[df.dtypes == "float64"].index.to_list()
+        anis_columns = [col for col in float_columns if col not in isotropic_vars]
 
         new = cls(log_vars=log_vars, logit_vars=logit_vars)
 
-        dct = (
-            df[float_columns]
-            .apply(new.transform)
-            .agg([np.mean, np.var])
-            .rename(index={"mean": "μ", "var": "σ2"})
-            .to_dict()
-        )
+        if anis_columns:
+            anis_dct = (
+                df[anis_columns]
+                .apply(new.transform)
+                .agg(["mean", "var"])
+                .rename(index={"mean": "μ", "var": "σ2"})
+                .to_dict()
+            )
+        else:
+            anis_dct = {}
+
+        if isotropic_vars:        
+            iso_df = (
+                df[isotropic_vars]
+                .apply(new.transform)
+            )
 
-        return new | dct
+            iso_μ = iso_df.values.mean()
+            iso_σ2 = iso_df.values.var()
+            
+            iso_dct = {col : {"μ": iso_μ, "σ2": iso_σ2} for col in isotropic_vars}
+        else:
+            iso_dct = {}
+
+        return new | anis_dct | iso_dct
 
     def transform(self, name: str | pd.Series, μ: float = None, σ2: float = None) -> float | tuple | pd.Series:
         """Transforms a parameter, distribution, or Series
 
         Parameters
         ----------
         name: str or pd.Series
-            Name of parameter. If a Series is supplied, the name of the series must be the parameter name.
+            Name of parameter. If a Series is supplied, the name of the series
+            must be the parameter name.
         μ: float, optional
-            Value of parameter or mean of parameter distribution. Only optional if first argument is a Series.
+            Value of parameter or mean of parameter distribution. Only optional
+            if first argument is a Series.
         σ2: float, optional
             Variance of parameter distribution.
 
         Returns
         -------
         float, tuple, or pd.Series
-            Transformed parameter, (mean, variance) of untransformed distribution, or untransformed Series
+            Transformed parameter, (mean, variance) of untransformed
+            distribution, or untransformed Series
         """
         if isinstance(name, pd.Series):
             series = name
             return self._transform_value(series.name, series)
         elif μ is None:
             raise ValueError("μ cannot be None")
         if σ2 is None:
@@ -254,75 +289,85 @@
 
     def untransform(self, name: str | pd.Series, μ: float = None, σ2: float = None) -> float | tuple | pd.Series:
         """Untransforms a parameter, distribution, or Series
 
         Parameters
         ----------
         name: str or pd.Series
-            Name of parameter. If a Series is supplied, the name of the series must be the parameter name.
+            Name of parameter. If a Series is supplied, the name of the series
+            must be the parameter name.
         μ: float, optional
-            Value of parameter or mean of parameter distribution. Only optional if first argument is a Series.
+            Value of parameter or mean of parameter distribution. Only optional
+            if first argument is a Series.
         σ2: float, optional
             Variance of parameter distribution.
 
         Returns
         -------
         float, tuple, or pd.Series
-            Untransformed parameter, (mean, variance) of untransformed distribution, or untransformed Series
+            Untransformed parameter, (mean, variance) of untransformed
+            distribution, or untransformed Series
         """
         if isinstance(name, pd.Series):
             series = name
             return self._untransform_value(series.name, series)
         if σ2 is None:
             return self._untransform_value(name, μ)
         else:
             return self._untransform_dist(name, μ, σ2)
 
     def stdz(self, name: str | pd.Series, μ: float = None, σ2: float = None) -> float | tuple | pd.Series:
-        """Transforms, mean-centers, and scales a parameter, distribution, or Series
+        """Transforms, centers, and scales a parameter, distribution, or Series
 
         Parameters
         ----------
         name: str or pd.Series
-            Name of parameter. If a Series is supplied, the name of the series must be the parameter name.
+            Name of parameter. If a Series is supplied, the name of the series
+            must be the parameter name.
         μ: float, optional
-            Value of parameter or mean of parameter distribution. Only optional if first argument is a Series.
+            Value of parameter or mean of parameter distribution. Only optional
+            if first argument is a Series.
         σ2: float, optional
             Variance of parameter distribution.
 
         Returns
         -------
         float, tuple, or pd.Series
-            Standardized parameter, (mean, variance) of standardized distribution, or standardized Series
+            Standardized parameter, (mean, variance) of standardized
+            distribution, or standardized Series
         """
 
         if isinstance(name, pd.Series):
             series = name
             return self._stdz_value(series.name, series)
         if σ2 is None:
             return self._stdz_value(name, μ)
         else:
             return self._stdz_dist(name, μ, σ2)
 
     def unstdz(self, name: str | pd.Series, μ: float = None, σ2: float = None) -> float | tuple | pd.Series:
-        """Untransforms, un-centers, and un-scales a parameter, distribution, or Series
+        """Untransforms, un-centers, and un-scales a parameter, distribution, or
+        Series
 
         Parameters
         ----------
         name: str or pd.Series
-            Name of parameter. If a Series is supplied, the name of the series must be the parameter name.
+            Name of parameter. If a Series is supplied, the name of the series
+            must be the parameter name.
         μ: float, optional
-            Value of parameter or mean of parameter distribution. Only optional if first argument is a Series.
+            Value of parameter or mean of parameter distribution. Only optional
+            if first argument is a Series.
         σ2: float, optional
             Variance of parameter distribution.
 
         Returns
         -------
         float, tuple, or pd.Series
-            Unstandardized parameter, (mean, variance) of unstandardized distribution, or unstandardized Series
+            Unstandardized parameter, (mean, variance) of unstandardized
+            distribution, or unstandardized Series
         """
 
         if isinstance(name, pd.Series):
             series = name
             return self._unstdz_value(series.name, series)
         if σ2 is None:
             return self._unstdz_value(name, μ)
@@ -341,55 +386,61 @@
         return x_
 
     def _stdz_value(self, name: str, x: float) -> float:
         x_ = self.transform(name, x)
         μ = self.get(name, {"μ": 0})["μ"]
         σ2 = self.get(name, {"σ2": 1})["σ2"]
         σ = np.sqrt(σ2)
-        return (x_ - μ) / σ
+        return np.divide((x_ - μ), σ)
 
     def _unstdz_value(self, name: str, z: float) -> float:
         μ = self.get(name, {"μ": 0})["μ"]
         σ2 = self.get(name, {"σ2": 1})["σ2"]
         σ = np.sqrt(σ2)
-        x_ = z * σ + μ
+        x_ = np.multiply(z, σ) + μ
         return self.untransform(name, x_)
 
     @property
     def mean_transforms(self):
         """Function that transforms the mean of a distribution.
 
-        These transform's should follow scipy's conventions such that a distribution can be defined in the given
-        space by passing (loc=μ, scale=σ2**0.5). For a lognormal variable, an RV defined as ``lognorm(loc=μ,
-        scale=σ2**0.5)`` in "natural" space is equivalent to ``norm(loc=np.log(μ), scale=σ2**0.5)`` in log space,
-        so this transform should return ``np.log(μ)`` when converting from natural to log space, and ``np.exp(μ)``
-        when converting from log to natural space. Similarly for a logit-normal variable, an RV defined as
-        ``logitnorm(loc=μ, scale=σ2**0.5))`` in natural space is equivalent to ``norm(loc=logit(μ), scale=σ2**0.5)``
-        in logit space, so this transform should return ``logit(μ)`` when converting from natural to logit space,
-        and ``expit(μ)`` when converting from logit to natural space.
+        These transform's should follow scipy's conventions such that a
+        distribution can be defined in the given space by passing (loc=μ,
+        scale=σ2**0.5). For a lognormal variable, an RV defined as
+        ``lognorm(loc=μ, scale=σ2**0.5)`` in "natural" space is equivalent to
+        ``norm(loc=np.log(μ), scale=σ2**0.5)`` in log space, so this transform
+        should return ``np.log(μ)`` when converting from natural to log space,
+        and ``np.exp(μ)`` when converting from log to natural space. Similarly
+        for a logit-normal variable, an RV defined as ``logitnorm(loc=μ,
+        scale=σ2**0.5))`` in natural space is equivalent to ``norm(loc=logit(μ),
+        scale=σ2**0.5)`` in logit space, so this transform should return
+        ``logit(μ)`` when converting from natural to logit space, and
+        ``expit(μ)`` when converting from logit to natural space.
         """
 
         # Forward and reverse transform for each variable type
         transforms = {
             skip: [lambda μ, σ2: μ, lambda μ, σ2: μ],
-            # Note these are no longer strictly mean and variance. They are defined to be compatible with
-            # scipy.stats.lognormal definition
+            # Note these are no longer strictly mean and variance. They are
+            # defined to be compatible with scipy.stats.lognormal definition
             np.log: [lambda μ, σ2: np.log(μ), lambda μ, σ2: np.exp(μ)],
             logit: [lambda μ, σ2: logit(μ), lambda μ, σ2: expit(μ)],
         }
         return transforms
 
     @property
     def var_transforms(self):
         """Function that transforms the variance of a distribution.
 
-        These transform's should follow scipy's conventions such that a distribution can be defined in the given
-        space by passing (loc=μ, scale=σ2**0.5). Accordingly, since both log-normal and logit-normal variables are
-        defined in terms of the scale (standard deviation) in their respective transformed spaces, this function
-        simply returns the variance unchanged in these cases.
+        These transform's should follow scipy's conventions such that a
+        distribution can be defined in the given space by passing (loc=μ,
+        scale=σ2**0.5). Accordingly, since both log-normal and logit-normal
+        variables are defined in terms of the scale (standard deviation) in
+        their respective transformed spaces, this function simply returns the
+        variance unchanged in these cases.
         """
 
         # Forward and reverse transform for each variable type
         transforms = {
             skip: [lambda μ, σ2: σ2, lambda μ, σ2: σ2],
             np.log: [lambda μ, σ2: σ2, lambda μ, σ2: σ2],
             logit: [lambda μ, σ2: σ2, lambda μ, σ2: σ2],
@@ -438,14 +489,15 @@
 class MetaFrame(pd.DataFrame, ABC):
     """Abstract Base Class for :class:`WideData` and :class:`TidyData`."""
 
     df: pd.DataFrame
     outputs: list
     log_vars: list = None
     logit_vars: list = None
+    isotropic_vars: list = None
     names_column: str = "Variable"
     values_column: str = "Value"
     stdzr: Standardizer = None
 
     _metadata = [
         "df",
         "outputs",
@@ -455,15 +507,15 @@
         "values_column",
         "stdzr",
     ]
 
     def __post_init__(self):
         super(MetaFrame, self).__init__(self.df)
         if self.stdzr is None:
-            self.stdzr = Standardizer.from_DataFrame(self.df, log_vars=self.log_vars, logit_vars=self.logit_vars)
+            self.stdzr = Standardizer.from_DataFrame(self.df, log_vars=self.log_vars, logit_vars=self.logit_vars, isotropic_vars=self.isotropic_vars)
         else:
             self.log_vars = self.stdzr.log_vars
             self.logit_vars = self.stdzr.logit_vars
         del self.df
 
     def __repr__(self):
         cls = self.__class__.__name__
@@ -492,15 +544,16 @@
     @abstractmethod
     def t(self) -> pd.DataFrame:
         """Transformed data values."""
         pass
 
     @property
     def specs(self) -> dict:
-        """Provides keyword arguments for easy instantiation of a similar object."""
+        """Provides keyword arguments for easy instantiation of a similar
+        object."""
         return dict(
             outputs=self.outputs,
             names_column=self.names_column,
             values_column=self.values_column,
             stdzr=self.stdzr,
             log_vars=self.log_vars,
             logit_vars=self.logit_vars,
@@ -533,37 +586,43 @@
         wide = (
             tidy.pivot(index=inputs, columns=names_column, values=values_column).reset_index().rename_axis(columns=None)
         )
         return wide
 
 
 class WideData(MetaFrame):
-    """Container for wide-form tabular data, allowing simple access to standardized and/or transformed values.
+    """Container for wide-form tabular data, allowing simple access to
+    standardized and/or transformed values.
 
-    Note that :class:`WideData` is instantiated with a **wide-form** dataframe. This class is not intended to be
-    instantiated directly, use :class:`DataSet` instead. :class:`WideData` subclasses pandas' DataFrame,
-    which everyone says is a bad idea, so be prepared for unexpected behavior if instantiated directly. Namely, in-place
-    modifications return a :class:`WideData` type correctly, but slices return a `pd.DataFrame` type.
+    Note that :class:`WideData` is instantiated with a **wide-form** dataframe.
+    This class is not intended to be instantiated directly, use :class:`DataSet`
+    instead. :class:`WideData` subclasses pandas' DataFrame, which everyone says
+    is a bad idea, so be prepared for unexpected behavior if instantiated
+    directly. Namely, in-place modifications return a :class:`WideData` type
+    correctly, but slices return a `pd.DataFrame` type.
 
     Parameters
     ----------
     data: pd.DataFrame
         A wide-form dataframe.
     outputs: list
         Columns of `data` to be treated as outputs.
     names_column: str, default 'Variable'
         Name to be used in tidy view for column containing output names.
     values_column: str, default 'Value'
         Name to be used in tidy view for column containing output values.
     log_vars: list, optional
-        List of input and output variables to be treated as log-normal. Ignored if `stdzr` is supplied.
+        List of input and output variables to be treated as log-normal. Ignored
+        if `stdzr` is supplied.
     logit_vars: list, optional
-        List of input and output variables to be treated as logit-normal. Ignored if `stdzr` is supplied.
+        List of input and output variables to be treated as logit-normal.
+        Ignored if `stdzr` is supplied.
     stdzr: Standardizer, optional
-        An :class:`Standardizer` instance. If not supplied, one will be created automatically.
+        An :class:`Standardizer` instance. If not supplied, one will be created
+        automatically.
     """
 
     @property
     def z(self) -> pd.DataFrame:
         """Standardized data values."""
         df_ = self.copy()
         cols = self.outputs + self.float_inputs
@@ -590,52 +649,59 @@
         outputs=None,
         names_column="Variable",
         values_column="Value",
         stdzr=None,
         log_vars=None,
         logit_vars=None,
     ):
-        """Constructs `WideData` from a tidy-form dataframe. See :class:`WideData` for explanation of arguments."""
+        """Constructs `WideData` from a tidy-form dataframe. See
+        :class:`WideData` for explanation of arguments."""
         outputs = outputs if outputs is not None else list(tidy[names_column].unique())
         wide = cls._tidy_to_wide_(tidy, names_column=names_column, values_column=values_column)
         return cls(
             wide,
             outputs=outputs,
             names_column=names_column,
             values_column=values_column,
             stdzr=stdzr,
             log_vars=log_vars,
             logit_vars=logit_vars,
         )
 
 
 class TidyData(MetaFrame):
-    """Container for tidy-form tabular data, allowing simple access to standardized and/or transformed values.
+    """Container for tidy-form tabular data, allowing simple access to
+    standardized and/or transformed values.
 
-    Note that :class:`TidyData` is instantiated with a **wide-form** dataframe. This class is not intended to be
-    instantiated directly, use :class:`DataSet` instead. :class:`TidyData` subclasses pandas' DataFrame,
-    which everyone says is a bad idea, so be prepared for unexpected behavior if instantiated directly. Namely, in-place
-    modifications return a :class:`TidyData` type correctly, but slices return a `pd.DataFrame` type.
+    Note that :class:`TidyData` is instantiated with a **wide-form** dataframe.
+    This class is not intended to be instantiated directly, use :class:`DataSet`
+    instead. :class:`TidyData` subclasses pandas' DataFrame, which everyone says
+    is a bad idea, so be prepared for unexpected behavior if instantiated
+    directly. Namely, in-place modifications return a :class:`TidyData` type
+    correctly, but slices return a `pd.DataFrame` type.
 
     Parameters
     ----------
     data: pd.DataFrame
         A wide-form dataframe.
     outputs: list
         Columns of `data` to be treated as outputs.
     names_column: str, default 'Variable'
         Name to be used in tidy view for column containing output names.
     values_column: str, default 'Value'
         Name to be used in tidy view for column containing output values.
     log_vars: list, optional
-        List of input and output variables to be treated as log-normal. Ignored if `stdzr` is supplied.
+        List of input and output variables to be treated as log-normal. Ignored
+        if `stdzr` is supplied.
     logit_vars: list, optional
-        List of input and output variables to be treated as logit-normal. Ignored if `stdzr` is supplied.
+        List of input and output variables to be treated as logit-normal.
+        Ignored if `stdzr` is supplied.
     stdzr: Standardizer, optional
-        An :class:`Standardizer` instance. If not supplied, one will be created automatically.
+        An :class:`Standardizer` instance. If not supplied, one will be created
+        automatically.
     """
 
     def __post_init__(self):
         tidy = self._wide_to_tidy_(
             self.df,
             outputs=self.outputs,
             names_column=self.names_column,
@@ -675,52 +741,67 @@
         wide_df = self._tidy_to_wide_(self, names_column=self.names_column, values_column=self.values_column)
         wide = WideData(wide_df, **self.specs)
         return wide
 
 
 @dataclass
 class DataSet:
-    """Container for tabular data, allowing simple access to standardized values and wide or tidy dataframe formats.
+    """Container for tabular data, allowing simple access to standardized values
+    and wide or tidy dataframe formats.
 
-    :class:`DataSet` is instantiated with a **wide-form** dataframe, with all outputs of a given observation in a
-    single row, but allows easy access to the corresponding **tidy** dataframe, with each output in a separate row (
-    the :meth:`from_tidy` also allows construction from tidy data`). The titles of the tidy-form columns for the
-    output names and their values are supplied at instantiation, defaulting to "Variable" and "Value". For example,
-    say we have an observation at position (x,y) with measurements of i, j, and k. The wide-form dataframe would have
-    one column for each of x, y, i, j, and k, while the tidy-form dataframe would have a column for each of x and y,
-    a "Variable" column where each row contains either "i", "j", or "k" as strings, and a "Value" column containing
-    the corresponding measurement. Wide data is more space-efficient and perhaps more intuitive to construct and
-    inspect, while tidy data more clearly distinguishes inputs and outputs. These views are accessible through the
-    :attr:`wide` and :attr:`tidy` attributes as instances of :class:`WideData` and :class:`TidyData`, respectively.
-
-    As a container for :class:`WideData` and :class:`TidyData`, this class also provides simple access to
-    standardized values of the data through `wide.z` and `tidy.z` or transformed values through `wide.t` and
-    `tidy.t`. A :class:`Standardizer` instance can be supplied as a keyword argument, otherwise one will be
-    constructed automatically from the supplied dataframe with the supplied values of `log_vars` and `logit_vars`.
-    Unlike :class:`WideData` and :class:`TidyData`, the :attr:`wide` and :attr:`tidy` attributes of a *DataSet* can
-    be altered and sliced while retaining their functionality, with a cursory integrity check. The
-    :class:`Standardizer` instance can be updated with :meth:`update_stdzr`, for example following manipulation of
-    the data or alteration of :attr:`log_vars` and :attr:`logit_vars`.
+    :class:`DataSet` is instantiated with a **wide-form** dataframe, with all
+    outputs of a given observation in a single row, but allows easy access to
+    the corresponding **tidy** dataframe, with each output in a separate row (
+    the :meth:`from_tidy` also allows construction from tidy data`). The titles
+    of the tidy-form columns for the output names and their values are supplied
+    at instantiation, defaulting to "Variable" and "Value". For example, say we
+    have an observation at position (x,y) with measurements of i, j, and k. The
+    wide-form dataframe would have one column for each of x, y, i, j, and k,
+    while the tidy-form dataframe would have a column for each of x and y, a
+    "Variable" column where each row contains either "i", "j", or "k" as
+    strings, and a "Value" column containing the corresponding measurement. Wide
+    data is more space-efficient and perhaps more intuitive to construct and
+    inspect, while tidy data more clearly distinguishes inputs and outputs.
+    These views are accessible through the :attr:`wide` and :attr:`tidy`
+    attributes as instances of :class:`WideData` and :class:`TidyData`,
+    respectively.
+
+    As a container for :class:`WideData` and :class:`TidyData`, this class also
+    provides simple access to standardized values of the data through `wide.z`
+    and `tidy.z` or transformed values through `wide.t` and `tidy.t`. A
+    :class:`Standardizer` instance can be supplied as a keyword argument,
+    otherwise one will be constructed automatically from the supplied dataframe
+    with the supplied values of `log_vars` and `logit_vars`. Unlike
+    :class:`WideData` and :class:`TidyData`, the :attr:`wide` and :attr:`tidy`
+    attributes of a *DataSet* can be altered and sliced while retaining their
+    functionality, with a cursory integrity check. The :class:`Standardizer`
+    instance can be updated with :meth:`update_stdzr`, for example following
+    manipulation of the data or alteration of :attr:`log_vars` and
+    :attr:`logit_vars`.
 
     Parameters
     ----------
     data: pd.DataFrame
-        A wide-form dataframe. See class method :meth:`from_tidy` for instantiation from tidy data.
+        A wide-form dataframe. See class method :meth:`from_tidy` for
+        instantiation from tidy data.
     outputs: list
         Columns of `data` to be treated as outputs.
     names_column: str, default 'Variable'
         Name to be used in tidy view for column containing output names.
     values_column: str, default 'Value'
         Name to be used in tidy view for column containing output values.
     log_vars: list, optional
-        List of input and output variables to be treated as log-normal. Ignored if `stdzr` is supplied.
+        List of input and output variables to be treated as log-normal. Ignored
+        if `stdzr` is supplied.
     logit_vars: list, optional
-        List of input and output variables to be treated as logit-normal. Ignored if `stdzr` is supplied.
+        List of input and output variables to be treated as logit-normal.
+        Ignored if `stdzr` is supplied.
     stdzr: Standardizer, optional
-        An :class:`Standardizer` instance. If not supplied, one will be created automatically.
+        An :class:`Standardizer` instance. If not supplied, one will be created
+        automatically.
 
     Examples
     --------
     >>> df = pd.read_pickle(test_data / 'estimates_test_data.pkl')
     >>> ds = DataSet.from_tidy(df, names_column='Parameter', log_vars=['Y', 'c', 'b'], logit_vars=['X', 'e'])
     >>> ds
     DataSet:
@@ -742,19 +823,20 @@
 
     data: pd.DataFrame
     outputs: list
     names_column: str = "Variable"
     values_column: str = "Value"
     log_vars: list = None
     logit_vars: list = None
+    isotropic_vars: list = None
     stdzr: Standardizer = None
 
     def __post_init__(self):
         if self.stdzr is None:
-            self.stdzr = Standardizer.from_DataFrame(self.wide, log_vars=self.log_vars, logit_vars=self.logit_vars)
+            self.stdzr = Standardizer.from_DataFrame(self.wide, log_vars=self.log_vars, logit_vars=self.logit_vars, isotropic_vars=self.isotropic_vars)
         else:
             self.log_vars = self.stdzr.log_vars
             self.logit_vars = self.stdzr.logit_vars
 
     def __repr__(self):
         wide_shape = "[{0} rows x {1} columns]".format(*self.wide.shape)
         tidy_shape = "[{0} rows x {1} columns]".format(*self.tidy.shape)
@@ -767,15 +849,16 @@
                 f"inputs: {self.inputs}",
             ]
         )
         return summary
 
     @property
     def specs(self):
-        """Provides keyword arguments for easy instantiation of a similar :class:`DataSet`."""
+        """Provides keyword arguments for easy instantiation of a similar
+        :class:`DataSet`."""
         return dict(
             outputs=self.outputs,
             names_column=self.names_column,
             values_column=self.values_column,
             stdzr=self.stdzr,
             log_vars=self.log_vars,
             logit_vars=self.logit_vars,
@@ -822,15 +905,16 @@
         outputs=None,
         names_column="Variable",
         values_column="Value",
         stdzr=None,
         log_vars=None,
         logit_vars=None,
     ):
-        """Constructs a `DataSet` from a tidy-form dataframe. See :class:`DataSet` for explanation of arguments."""
+        """Constructs a `DataSet` from a tidy-form dataframe. See
+        :class:`DataSet` for explanation of arguments."""
         assert all(
             [col in tidy.columns for col in [names_column, values_column]]
         ), f"Dataframe must have both columns {[names_column, values_column]}"
         specs = dict(
             outputs=outputs,
             names_column=names_column,
             values_column=values_column,
@@ -848,23 +932,25 @@
         outputs=None,
         names_column="Variable",
         values_column="Value",
         stdzr=None,
         log_vars=None,
         logit_vars=None,
     ):
-        """Constructs a `DataSet` from a wide-form dataframe. See :class:`DataSet` for explanation of arguments."""
+        """Constructs a `DataSet` from a wide-form dataframe. See
+        :class:`DataSet` for explanation of arguments."""
         return cls(
             wide,
             outputs=outputs,
             names_column=names_column,
             values_column=values_column,
             stdzr=stdzr,
             log_vars=log_vars,
             logit_vars=logit_vars,
         )
 
     def update_stdzr(self):
-        """Updates internal :class:`Standardizer` with current data, :attr:`log_vars`, and :attr:`logit_vars`."""
+        """Updates internal :class:`Standardizer` with current data,
+        :attr:`log_vars`, and :attr:`logit_vars`."""
         self.stdzr.update(
-            Standardizer.from_DataFrame(self.wide, log_vars=self.log_vars, logit_vars=self.logit_vars)
+            Standardizer.from_DataFrame(self.wide, log_vars=self.log_vars, logit_vars=self.logit_vars, isotropic_vars=self.isotropic_vars)
         )  # Fix once Python >= 3.9
```

### Comparing `gumbi-0.2.1/gumbi/arrays.py` & `gumbi-0.2.2/gumbi/arrays.py`

 * *Files 0% similar despite different names*

```diff
@@ -660,28 +660,28 @@
             # name = '('+', '.join(names)+')'
         return UncertainArray(name, **{dim: new[dim] for dim in new.dtype.names})
 
     def nlpd(self, target) -> float:
         """Negative log posterior density"""
         return -np.log(self.dist.pdf(target))
 
-    def EI(self, target, best_yet, k=1) -> float:
-        """Expected improvement
+    def vEI(self, target, best_yet, k=1) -> float:
+        """Vector expected improvement
 
         Taken from https://github.com/akuhren/target_vector_estimation
 
         Parameters
         ----------
         target : float
         best_yet : float
         k : int
 
         Returns
         -------
-        EI : float
+        vEI : float
         """
 
         nc = ((target - self.μ) ** 2) / self.σ2
 
         h1_nx = ncx2.cdf((best_yet / self.σ2), k, nc)
         h2_nx = ncx2.cdf((best_yet / self.σ2), (k + 2), nc)
         h3_nx = ncx2.cdf((best_yet / self.σ2), (k + 4), nc)
```

### Comparing `gumbi-0.2.1/gumbi/data/Example_DataSet.pkl` & `gumbi-0.2.2/gumbi/data/Example_DataSet.pkl`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.1/gumbi/plotting.py` & `gumbi-0.2.2/gumbi/plotting.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.1/gumbi/regression/base.py` & `gumbi-0.2.2/gumbi/regression/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from gumbi.aggregation import DataSet
 from gumbi.arrays import MVUncertainParameterArray as mvuparray
 from gumbi.arrays import ParameterArray as parray
 from gumbi.arrays import UncertainParameterArray as uparray
 from gumbi.arrays import *
 from gumbi.utils.misc import assert_in, assert_is_subset
 
-# from gumbi.utils.gp_utils import get_ℓ_prior
+# from gumbi.utils.gp_utils import get_ls_prior
 
 __all__ = ["Regressor"]
 
 
 class Regressor(ABC):
     r"""Surface learning and prediction.
 
@@ -519,15 +519,15 @@
 
             # Get model coordinates for each output to be predicted
             param_coords = [self.categorical_coords[self.out_col][p] for p in output]
 
             # Convert input points to tall array and tile once for each output, adding the respective coordinate
             tall_points = parray.vstack([points.add_layers(**{self.out_col: coord})[:, None] for coord in param_coords])
         else:
-            # If self.out_col is not in categorical_dims, it must be in filter_dims, and only one is possible Convert
+            # If self.out_col is not in categorical_dims, it must be in filter_dims, and only one is possible. Convert
             # input points to tall array
             param_coords = None
             tall_points = points[:, None]
 
         # Combine standardized coordinates into an ordinary tall numpy array for prediction
         points_array = np.hstack([tall_points[dim].z.values() for dim in self.dims])
 
@@ -795,15 +795,15 @@
         df = df[df[self.out_col] == output]
         observed = self.parray(**{output: df["Values"]}, stdzd=False)
 
         target = self.parray(**{output: target}, stdzd=False)
         best_yet = np.min(np.sqrt(np.mean(np.square(observed.z - target.z))))
 
         if acquisition == "EI":
-            self.proposal_surface = self.predictions.z.EI(target.z, best_yet.z)
+            self.proposal_surface = self.predictions.z.vEI(target.z, best_yet.z)
         elif acquisition == "PD":
             self.proposal_surface = self.predictions.z.nlpd(target.z)
 
         self.proposal_idx = np.argmax(self.proposal_surface)
         self.proposal = self.predictions_X.ravel()[self.proposal_idx]
 
         return self.proposal
```

### Comparing `gumbi-0.2.1/gumbi/regression/pymc/GP.py` & `gumbi-0.2.2/gumbi/regression/pymc/GP.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from gumbi.aggregation import DataSet
 from gumbi.arrays import (  # noqa: F401
     MVUncertainParameterArray,
     ParameterArray,
     UncertainParameterArray,
 )
-from gumbi.utils.gp_utils import get_ℓ_prior
+from gumbi.utils.gp_utils import get_ls_prior
 from gumbi.utils.misc import assert_in
 
 from ..base import Regressor
 
 __all__ = ["GP"]
 
 
@@ -23,99 +23,118 @@
 
     See Also
     --------
     :class:`Regressor`
 
     Notes
     -----
-    The GP class is built from a dataframe in the form of a :class:`DataSet` object. The output(s) are taken from
-    :attr:`DataSet.outputs` and the corresponding column in the tidy data frame taken from :attr:`DataSet.names_column`.
-    This column will be generically referred to as the `output_column` in this documentation, but can take any value
-    specifed when the :class:`DataSet` is constructed. The model inputs are constructed by filtering this dataframe,
-    extracting column values, and converting these to numerical input coordinates. The main entry point will be
-    :meth:`fit`, which parses the dimensions of the model with :meth:`specify_model`, extracts numerical input
-    coordinates with :meth:`get_structured_data`, compiles the Pymc model with :meth:`build_model`, and finally learns
-    the hyperparameters with :meth:`find_MAP`.
+    The GP class is built from a dataframe in the form of a :class:`DataSet`
+    object. The output(s) are taken from :attr:`DataSet.outputs` and the
+    corresponding column in the tidy data frame taken from
+    :attr:`DataSet.names_column`. This column will be generically referred to as
+    the `output_column` in this documentation, but can take any value specifed
+    when the :class:`DataSet` is constructed. The model inputs are constructed
+    by filtering this dataframe, extracting column values, and converting these
+    to numerical input coordinates. The main entry point will be :meth:`fit`,
+    which parses the dimensions of the model with :meth:`specify_model`,
+    extracts numerical input coordinates with :meth:`get_structured_data`,
+    compiles the Pymc model with :meth:`build_model`, and finally learns the
+    hyperparameters with :meth:`find_MAP`.
 
     Dimensions fall into several categories:
 
-    * Filter dimensions, those with only one level, are used to subset the dataframe but are not included as explicit
-      inputs to the model. These are not specified explicitly, but rather any continuous or categorical dimension with
-      only one level is treated as a filter dimension.
+    * Filter dimensions, those with only one level, are used to subset the
+      dataframe but are not included as explicit inputs to the model. These are
+      not specified explicitly, but rather any continuous or categorical
+      dimension with only one level is treated as a filter dimension.
 
-    * Continuous dimensions are treated as explicit coordinates and given a Radial Basis Function kernel
+    * Continuous dimensions are treated as explicit coordinates and given a
+      Radial Basis Function kernel
 
-      * Linear dimensions (which must be a subset of `continuous_dims`) have an additional linear kernel.
+      * Linear dimensions (which must be a subset of `continuous_dims`) have an
+        additional linear kernel.
 
     * Coregion dimensions imply a distinct but correlated output for each level
 
-      * If more than one output is specified, the `output_column` is treated as a categorical dim.
+      * If more than one output is specified, the `output_column` is treated as
+        a categorical dim.
 
     A non-additive model has the form:
 
     .. math::
 
-        y &\sim \text{Normal} \left( \mu, \sigma \right) \\ mu &\sim \mathcal{GP} \left( K \right) \\ K &= \left(
-        K^\text{cont}+K^\text{lin} \right) K^\text{coreg}_\text{outputs} \prod_{n} K^\text{coreg}_{n} \\ K^\text{cont}
-        &= \text{RBF} \left( \ell_{i}, \eta \right) \\ K^\text{lin} &= \text{LIN} \left( c_{j}, \tau \right) \\
-        K^\text{coreg} &= \text{Coreg} \left( \boldsymbol{W}, \kappa \right) \\ \sigma &\sim \text{Exponential} \left( 1
-        \right) \\
-
-    Where :math:`i` denotes a continuous dimension, :math:`j` denotes a linear dimension, and :math:`n` denotes a
-    categorical dimension (excluding the `output_column`). :math:`K^\text{cont}` and :math:`K^\text{lin}` each consist
-    of a joint kernel encompassing all continuous and linear dimensions, respectively, whereas
-    :math:`K^\text{coreg}_{n}` is a distinct kernel for a given categorical dimension.
+        y &\sim \text{Normal} \left( \mu, \sigma \right) \\ mu &\sim
+        \mathcal{GP} \left( K \right) \\ K &= \left( K^\text{cont}+K^\text{lin}
+        \right) K^\text{coreg}_\text{outputs} \prod_{n} K^\text{coreg}_{n} \\
+        K^\text{cont} &= \text{RBF} \left( \ell_{i}, \eta \right) \\
+        K^\text{lin} &= \text{LIN} \left( c_{j}, \tau \right) \\ K^\text{coreg}
+        &= \text{Coreg} \left( \boldsymbol{W}, \kappa \right) \\ \sigma &\sim
+        \text{Exponential} \left( 1 \right) \\
+
+    Where :math:`i` denotes a continuous dimension, :math:`j` denotes a linear
+    dimension, and :math:`n` denotes a categorical dimension (excluding the
+    `output_column`). :math:`K^\text{cont}` and :math:`K^\text{lin}` each
+    consist of a joint kernel encompassing all continuous and linear dimensions,
+    respectively, whereas :math:`K^\text{coreg}_{n}` is a distinct kernel for a
+    given categorical dimension.
 
     The additive model has the form:
 
     .. math::
 
-        mu &\sim \mathcal{GP}\left( K^\text{global} \right) + \sum_{n} \mathcal{GP}\left( K_{n} \right) \\
-        K^\text{global} &= \left( K^\text{cont}+K^\text{lin} \right) K^\text{coreg}_\text{outputs} \\ K_{n} &= \left(
-        K^\text{cont}_{n}+K^\text{lin}_{n} \right) K^\text{coreg}_\text{outputs} K^\text{coreg}_{n} \\
-
-    Note that, in the additive model, :math:`K^\text{cont}_{n}` and :math:`K^\text{lin}_{n}` still consist of only the
-    continuous and linear dimensions, respectively, but have unique priors corresponding to each categorical dimension.
-    However, there is only one :math:`K^\text{coreg}_\text{outputs}` kernel.
+        mu &\sim \mathcal{GP}\left( K^\text{global} \right) + \sum_{n}
+        \mathcal{GP}\left( K_{n} \right) \\ K^\text{global} &= \left(
+        K^\text{cont}+K^\text{lin} \right) K^\text{coreg}_\text{outputs} \\
+        K_{n} &= \left( K^\text{cont}_{n}+K^\text{lin}_{n} \right)
+        K^\text{coreg}_\text{outputs} K^\text{coreg}_{n} \\
+
+    Note that, in the additive model, :math:`K^\text{cont}_{n}` and
+    :math:`K^\text{lin}_{n}` still consist of only the continuous and linear
+    dimensions, respectively, but have unique priors corresponding to each
+    categorical dimension. However, there is only one
+    :math:`K^\text{coreg}_\text{outputs}` kernel.
 
     Parameters
     ----------
     dataset : DataSet
         Data for fitting.
     outputs : str or list of str, default None
-        Name(s) of output(s) to learn. If ``None``, uses all values from ``outputs`` attribute of *dataset*.
+        Name(s) of output(s) to learn. If ``None``, uses all values from
+        ``outputs`` attribute of *dataset*.
     seed : int
         Random seed
 
     Examples
     --------
-    A GP object is created from a :class:`DataSet` and can be fit immediately with the default dimension configuration
-    (regressing `r` with RBF + linear kernels for `X` and `Y`):
+    A GP object is created from a :class:`DataSet` and can be fit immediately
+    with the default dimension configuration (regressing `r` with RBF + linear
+    kernels for `X` and `Y`):
 
     >>> import gumbi as gmb
     >>> df = pd.read_pickle(gmb.data.example_dataset)
     >>> outputs=['a', 'b', 'c', 'd', 'e', 'f']
     >>> ds = gmb.DataSet(df, outputs=outputs, log_vars=['Y', 'b', 'c', 'd', 'f'], logit_vars=['X', 'e'])
     >>> gp = gmb.GP(ds, outputs='d').fit()
 
     Note that last line is equivalent to
 
     >>> gp = gmb.GP(ds, outputs='d')
     >>> gp.specify_model()
     >>> gp.build_model()
     >>> gp.find_MAP()
 
-    The model can be specified with various continuous, linear, and categorical dimensions. `X` and `Y` are always
-    included in both ``continuous_dims`` and ``linear_dims``.
+    The model can be specified with various continuous, linear, and categorical
+    dimensions. `X` and `Y` are always included in both ``continuous_dims`` and
+    ``linear_dims``.
 
     >>> gp.specify_model(continuous_dims='lg10_Z', linear_dims='lg10_Z', categorical_dims='Pair')
     >>> gmb.GP(ds).fit(continuous_dims='lg10_Z', linear_dims='lg10_Z', categorical_dims='Pair')  # equivalent
 
-    After the model is fit, define a grid of points at which to make predictions. The result is a
-    :class:`ParameterArray`:
+    After the model is fit, define a grid of points at which to make
+    predictions. The result is a :class:`ParameterArray`:
 
     >>> gp.prepare_grid()
     >>> gp.grid_points
     ('X', 'Y'): [(0.075     ,  10.) (0.08358586,  10.) (0.09217172,  10.) ...
      (0.90782828, 800.) (0.91641414, 800.) (0.925     , 800.)]
 
     Make predictions, returning an :class:`UncertainParameterArray`
@@ -126,16 +145,17 @@
                     (0.70728502, 0.16073197) ... (0.70727954, 0.16073197)
                     (0.7072809 , 0.16073197) (0.70728058, 0.16073197)]
                    ...
                    [(0.70749247, 0.1607318 ) (0.70773573, 0.16073116)
                     (0.70806603, 0.16072949) ... (0.70728449, 0.16073197)
                     (0.70728194, 0.16073197) (0.7072807 , 0.16073197)]]
 
-    The `uparray` makes it easy to calculate standard statistics in natural or transformed/standardized space while
-    maintaining the original shape of the array:
+    The `uparray` makes it easy to calculate standard statistics in natural or
+    transformed/standardized space while maintaining the original shape of the
+    array:
 
     >>> gp.predictions.z.dist.ppf(0.025)
     array([[-3.1887916 , -3.18878491, -3.18876601, ..., -3.18879744,
             -3.18878966, -3.18879146],
            ...,
            [-3.1875742 , -3.18617286, -3.18426272, ..., -3.18876906,
             -3.18878366, -3.18879081]])
@@ -173,23 +193,27 @@
     seed : int
         Random seed
     continuous_dims : list of str
         Columns of dataframe used as continuous dimensions
     linear_dims : list of str
         Subset of continuous dimensions to apply an additional linear kernel.
     continuous_levels : dict
-        Values considered within each continuous column as ``{dim: [level1, level2]}``
+        Values considered within each continuous column as ``{dim: [level1,
+        level2]}``
     continuous_coords : dict
-        Numerical coordinates of each continuous level within each continuous dimension as ``{dim: {level: coord}}``
+        Numerical coordinates of each continuous level within each continuous
+        dimension as ``{dim: {level: coord}}``
     categorical_dims : list of str
         Columns of dataframe used as categorical dimensions
     categorical_levels : dict
-        Values considered within each categorical column as ``{dim: [level1, level2]}``
+        Values considered within each categorical column as ``{dim: [level1,
+        level2]}``
     categorical_coords : dict
-        Numerical coordinates of each categorical level within each categorical dimension as ``{dim: {level: coord}}``
+        Numerical coordinates of each categorical level within each categorical
+        dimension as ``{dim: {level: coord}}``
     additive : bool
         Whether to treat categorical dimensions as additive or joint
     filter_dims : dict
         Dictionary of column-value pairs used to filter dataset before fitting
     X : array
         A 2D tall array of input coordinates.
     y : array
@@ -242,73 +266,91 @@
         continuous_kernel="ExpQuad",
         period=None,
         heteroskedastic_inputs=False,
         heteroskedastic_outputs=True,
         sparse=False,
         n_u=100,
         ARD=True,
+        ls_bounds=None,
+        mass=0.98,
         spec_kwargs=None,
         build_kwargs=None,
         MAP_kwargs=None,
     ):
         """Fits a GP surface
 
-        Parses inputs, compiles a Pymc model, then finds the MAP value for the hyperparameters. `{}_dims` arguments
-        indicate the columns of the dataframe to be included in the model, with `{}_levels` indicating which values of
-        those columns are to be included (``None`` implies all values).
-
-        If ``additive==True``, the model is constructed as the sum of a global GP and a distinct GP for each categorical
-        dimension. Each of these GPs, including the global GP, consists of an RBF+linear kernel multiplied by a coregion
-        kernel for the `output_column` if necessary. Although the same continuous kernel structure is used for each GP
-        in this model, unique priors are assigned to each distinct kernel. However, there is always only one coregion
-        kernel for the `output_column`. The kernel for each dimension-specific GP is further multiplied by a coregion
-        kernel that provides an output for each level in that dimension.
+        Parses inputs, compiles a Pymc model, then finds the MAP value for the
+        hyperparameters. `{}_dims` arguments indicate the columns of the
+        dataframe to be included in the model, with `{}_levels` indicating which
+        values of those columns are to be included (``None`` implies all
+        values).
+
+        If ``additive==True``, the model is constructed as the sum of a global
+        GP and a distinct GP for each categorical dimension. Each of these GPs,
+        including the global GP, consists of an RBF+linear kernel multiplied by
+        a coregion kernel for the `output_column` if necessary. Although the
+        same continuous kernel structure is used for each GP in this model,
+        unique priors are assigned to each distinct kernel. However, there is
+        always only one coregion kernel for the `output_column`. The kernel for
+        each dimension-specific GP is further multiplied by a coregion kernel
+        that provides an output for each level in that dimension.
 
         See Also
         --------
         :meth:`build_model`
 
         Parameters
         ----------
         outputs : str or list of str, default None
             Name(s) of output(s) to learn. If ``None``, :attr:`outputs` is used.
         linear_dims : str or list of str, optional
-            Subset of continuous dimensions to apply an additional linear kernel. If ``None``, defaults to
-            ``['Y','X']``.
+            Subset of continuous dimensions to apply an additional linear
+            kernel. If ``None``, defaults to ``['Y','X']``.
         continuous_dims : str or list of str, optional
             Columns of dataframe used as continuous dimensions.
         continuous_levels : str, list, or dict, optional
-            Values considered within each continuous column as ``{dim: [level1, level2]}``.
+            Values considered within each continuous column as ``{dim: [level1,
+            level2]}``.
         continuous_coords : list or dict, optional
-            Numerical coordinates of each continuous level within each continuous dimension as ``{dim: {level:
-            coord}}``.
+            Numerical coordinates of each continuous level within each
+            continuous dimension as ``{dim: {level: coord}}``.
         categorical_dims : str or list of str, optional
             Columns of dataframe used as categorical dimensions.
         categorical_levels : str, list, or dict, optional
-            Values considered within each categorical column as ``{dim: [level1, level2]}``.
+            Values considered within each categorical column as ``{dim: [level1,
+            level2]}``.
         additive : bool, default False
             Whether to treat categorical_dims as additive or joint (default).
         seed : int, optional.
-            Random seed for model instantiation. If ``None``, :attr:`seed` is used.
-        continuous_kernel : {'ExpQuad', 'Matern32', 'Matern52', 'Exponential', or 'Cosine'}
-            Covariance function to use for continuous dimensions. See `pymc docs`_ for more details.
+            Random seed for model instantiation. If ``None``, :attr:`seed` is
+            used.
+        continuous_kernel : {'ExpQuad', 'Matern32', 'Matern52', 'Exponential',
+        or 'Cosine'}
+            Covariance function to use for continuous dimensions. See `pymc
+            docs`_ for more details.
         period : ParameterArray, optional
-            A single parray of length 1 with one layer for each `continuous_dims` by name containing the period of the kernel, if periodic-like kernel is used.
+            A single parray of length 1 with one layer for each
+            `continuous_dims` by name containing the period of the kernel, if
+            periodic-like kernel is used.
         heteroskedastic_inputs: bool, default False
-            Whether to allow heteroskedasticity along continuous dimensions (input-dependent noise)
+            Whether to allow heteroskedasticity along continuous dimensions
+            (input-dependent noise)
         heteroskedastic_outputs: bool, default True
-            Whether to allow heteroskedasticity between multiple outputs (output-dependent noise). `Not yet implemented`
+            Whether to allow heteroskedasticity between multiple outputs
+            (output-dependent noise). `Not yet implemented`
         sparse: bool, default False
             Whether to use a `sparse approximation`_ to the GP.
         n_u: int, default 100
-            Number of inducing points to use for the sparse approximation, if required.
+            Number of inducing points to use for the sparse approximation, if
+            required.
         ARD: bool, default True
-            Whether to use "Automatic Relevance Determination" in the continuous kernel. If _True_, each continuous
-            dimension receives its own lengthscale; otherwise a single lengthscale is used for all continuous
-            dimensions.
+            Whether to use "Automatic Relevance Determination" in the continuous
+            kernel. If _True_, each continuous dimension receives its own
+            lengthscale; otherwise a single lengthscale is used for all
+            continuous dimensions.
 
         **MAP_kwargs
             Additional keyword arguments passed to :func:`pm.find_MAP`.
 
         Returns
         -------
         self : :class:`GP`
@@ -331,65 +373,63 @@
             continuous_kernel=continuous_kernel,
             period=period,
             heteroskedastic_inputs=heteroskedastic_inputs,
             heteroskedastic_outputs=heteroskedastic_outputs,
             sparse=sparse,
             n_u=n_u,
             ARD=ARD,
+            ls_bounds=ls_bounds,
+            mass=mass,
             **(build_kwargs or {}),
         )
 
         self.find_MAP(**(MAP_kwargs or {}))
 
         return self
 
     def _make_continuous_cov(
         self,
         continuous_cov_func,
         D_in,
         idx_s,
         n_s,
-        ℓ_μ,
-        ℓ_σ,
+        ls_params,
         ARD=True,
         period=None,
         **kernel_kwargs,
     ):
         shape = n_s if ARD else 1
 
-        shape = n_s if ARD else 1
-
         if period is not None:
             zperiods = [period.z[dim + "_z"].values() for dim in self.continuous_dims]
             kernel_kwargs["period"] = np.array(zperiods).squeeze()
 
         def continuous_cov(suffix):
-            # ℓ = pm.InverseGamma(f'ℓ_{suffix}', mu=ℓ_μ, sigma=ℓ_σ, shape=shape)
-            ℓ = pm.Gamma(f"ℓ_{suffix}", alpha=2, beta=1, shape=shape)
+            ls = pm.InverseGamma(f"ls_{suffix}", **ls_params, shape=shape)
+            # ls = pm.Gamma(f"ls_{suffix}", alpha=2, beta=1, shape=shape)
             η = pm.Gamma(f"η_{suffix}", alpha=2, beta=1)
-            cov = η**2 * continuous_cov_func(input_dim=D_in, active_dims=idx_s, ls=ℓ, **kernel_kwargs)
+            cov = η**2 * continuous_cov_func(input_dim=D_in, active_dims=idx_s, ls=ls, **kernel_kwargs)
 
             return cov
 
         return continuous_cov
 
     def _make_periodic_cov(
         self,
         continuous_cov_func,
         D_in,
         idx_s,
         n_s,
-        ℓ_μ,
-        ℓ_σ,
+        ls_params,
         period,
         ARD=True,
         **kernel_kwargs,
     ):
         continuous_kernel_factory = self._make_continuous_cov(
-            continuous_cov_func, 2, None, n_s, ℓ_μ, ℓ_σ, ARD=ARD, **kernel_kwargs
+            continuous_cov_func, 2, None, n_s, ls_params, ARD=ARD, **kernel_kwargs
         )
 
         zperiods = [period.z[dim + "_z"].values() for dim in self.continuous_dims]
         zperiods = np.array(zperiods).squeeze() if len(zperiods) > 1 else zperiods[0]
 
         def mapping(x, zperiods):
             c = 2.0 * np.pi * (1.0 / zperiods)
@@ -431,14 +471,16 @@
         continuous_kernel="ExpQuad",
         period=None,
         heteroskedastic_inputs=False,
         heteroskedastic_outputs=True,
         sparse=False,
         n_u=100,
         ARD=True,
+        ls_bounds=None,
+        mass=0.98,
     ):
         r"""Compile a marginalized pymc model for the GP.
 
         Each dimension in :attr:`continuous_dims` is combined in an ExpQuad kernel with a principled
         :math:`\text{InverseGamma}` prior for each lengthscale (as `suggested by Michael Betancourt`_) and a
         :math:`\text{Gamma}\left(2, 1\right)` prior for variance.
 
@@ -493,16 +535,25 @@
             "seed": seed,
             "continuous_kernel": continuous_kernel,
             "heteroskedastic_inputs": heteroskedastic_inputs,
             "heteroskedastic_outputs": heteroskedastic_outputs,
             "sparse": sparse,
             "n_u": n_u,
         }
-
-        gp_dict = self._construct_kernels(X, continuous_kernel, seed, sparse, latent=False, ARD=ARD, period=period)
+        gp_dict = self._construct_kernels(
+            X,
+            continuous_kernel,
+            seed,
+            sparse,
+            latent=False,
+            ARD=ARD,
+            ls_bounds=ls_bounds,
+            mass=mass,
+            period=period,
+        )
 
         with self.model:
             # From https://docs.pymc.io/notebooks/GP-Marginal.html OR a covariance function for the noise can be given
             # noise_l = pm.Gamma("noise_l", alpha=2, beta=2) cov_func_noise = pm.gp.cov.Exponential(1, noise_l) +
             # pm.gp.cov.WhiteNoise(sigma=0.1) y_ = gp.marginal_likelihood("y", X=X, y=y, sigma=cov_func_noise)
 
             # GP is heteroskedastic across outputs by default, but homoskedastic across continuous dimensions
@@ -566,28 +617,51 @@
             "s": [self.dims.index(dim) for dim in self.continuous_dims],
             "c": [self.dims.index(dim) for dim in self.categorical_dims],
             "p": self.dims.index(self.out_col) if self.out_col in self.dims else None,
         }
 
         return dim_indexes
 
-    def _prepare_lengthscales(self, X):
-        X_s = X[:, self._get_dim_indexes()["s"]]
+    # def _prepare_lengthscales(self, X, ARD=False):
+    #     X_s = X[:, self._get_dim_indexes()["s"]]
+
+    #     ls_μ, ls_σ = [stat for stat in np.array([get_ls_prior(dim) for dim in X_s.T]).T]
+    #     return ls_μ, ls_σ
 
-        ℓ_μ, ℓ_σ = [stat for stat in np.array([get_ℓ_prior(dim) for dim in X_s.T]).T]
-        return ℓ_μ, ℓ_σ
+    def _prepare_lengthscales(self, X, *, ARD, ls_bounds=None, mass=0.98):
+        X_s = X[:, self._get_dim_indexes()["s"]]
+        
+        if ls_bounds is not None:
+            zbounds = [
+                [b if not np.isnan(b) else None for b in ls_bounds[dim].z.values().squeeze()]
+                if dim in ls_bounds.names else (None, None)
+                for dim in self.continuous_dims
+            ]
+            lower, upper = list(zip(*zbounds))
+        else:
+            lower, upper = None, None
+            
+        if not ARD and len(lower) != 1 or len(upper) != 1:
+            raise ValueError("Bounds must be specified for only a single dimension if ARD is False")
+        ls_params = get_ls_prior(X_s, ARD=ARD, lower=lower, upper=upper, mass=mass)
+
+        # ls_μ, ls_σ = [stat for stat in np.array([get_ls_prior(dim) for dim in X_s.T]).T]
+        # return ls_μ, ls_σ
+        return ls_params
 
     def _construct_kernels(
         self,
         X,
         continuous_kernel,
         seed,
         sparse,
         latent,
         ARD=True,
+        ls_bounds=None,
+        mass=0.98,
         period=None,
     ):
         continuous_kernels = [
             "ExpQuad",
             # "RatQuad",
             "Matern12",
             "Matern32",
@@ -608,23 +682,22 @@
 
         continuous_cov_func = getattr(pm.gp.cov, continuous_kernel)
 
         D_in = len(self.dims)
 
         ns = self._get_dim_counts()
         idxs = self._get_dim_indexes()
-        ℓ_μ, ℓ_σ = self._prepare_lengthscales(X)
+        ls_params = self._prepare_lengthscales(X, ARD=ARD, ls_bounds=ls_bounds, mass=mass)
 
         continuous_cov = kernel_factory(
             continuous_cov_func,
             D_in,
             idxs["s"],
             ns["s"],
-            ℓ_μ,
-            ℓ_σ,
+            ls_params,
             ARD=ARD,
             period=period,
         )
         linear_cov = self._make_linear_cov(D_in, idxs["l"], ns["l"])
         coreg_cov = self._make_coreg_cov(D_in, seed)
 
         pm_gp = self._choose_implementation(sparse=sparse, latent=latent)
@@ -684,14 +757,17 @@
 
     def build_latent(
         self,
         seed=None,
         continuous_kernel="ExpQuad",
         prior_name="latent_prior",
         ARD=True,
+        lower=None,
+        upper=None,
+        mass=0.98,
     ):
         if self.additive:
             raise NotImplementedError("Additive/latent GPs are not yet implemented")
 
         X, y = self.get_shaped_data("mean")
         D_in = len(self.dims)
         assert X.shape[1] == D_in
@@ -705,14 +781,17 @@
         gp_dict = self._construct_kernels(
             X,
             continuous_kernel,
             seed,
             sparse=False,
             latent=True,
             ARD=ARD,
+            lower=lower,
+            upper=upper,
+            mass=mass,
         )
 
         with self.model:
             self.prior = gp_dict["total"].prior(prior_name, X=X)
 
         return self
 
@@ -779,15 +858,15 @@
             predictions = self.gp_dict[additive_level].predict(
                 points_array, point=self.MAP, diag=True, pred_noise=with_noise, **kwargs
             )
 
         return predictions
 
     def _recursively_append(self, var_name, suffix="_", increment_var=True):
-        if var_name in [v.name for v in self.model.vars]:
+        if var_name in self.model.named_vars:
             if increment_var:
                 var_name += suffix
                 return self._recursively_append(var_name)
             else:
                 raise ValueError(f'The variable name "{var_name}" already exists in model.')
         else:
             return var_name
@@ -846,15 +925,15 @@
 
         with self.model:
             _ = self.gp_dict[additive_level].conditional(var_name, points_array)
 
         with self.model:
             samples = pm.sample_posterior_predictive(*args, source, var_names=[var_name], **kwargs)
 
-        self.predictions = self.parray(**{var_name: samples[var_name]}, stdzd=True)
+        self.predictions = self.parray(**{output: samples[var_name]}, stdzd=True)
         self.predictions_X = points
 
         return self.predictions
 
     def draw_grid_samples(
         self,
         *args,
```

### Comparing `gumbi-0.2.1/gumbi/regression/pymc/extras.py` & `gumbi-0.2.2/gumbi/regression/pymc/extras.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.1/gumbi/style/breve_presentation.mplstyle` & `gumbi-0.2.2/gumbi/style/breve_presentation.mplstyle`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.1/gumbi/style/futura_presentation.mplstyle` & `gumbi-0.2.2/gumbi/style/futura_presentation.mplstyle`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.1/gumbi/style/presentation.mplstyle` & `gumbi-0.2.2/gumbi/style/presentation.mplstyle`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.1/gumbi/utils/generic_utils.py` & `gumbi-0.2.2/gumbi/utils/generic_utils.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.1/gumbi/utils/pymc_utils.py` & `gumbi-0.2.2/gumbi/utils/pymc_utils.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.1/gumbi.egg-info/PKG-INFO` & `gumbi-0.2.2/gumbi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gumbi
-Version: 0.2.1
+Version: 0.2.2
 Summary: Gaussian Process Model Building Interface
 Home-page: https://github.com/JohnGoertz/Gumbi
 Author: John Goertz
 Author-email: 
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -17,14 +17,22 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas>=1.2.3
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: seaborn
+Requires-Dist: matplotlib
+Requires-Dist: pymc>=5.3.1
+Requires-Dist: arviz
+Requires-Dist: uncertainties
 
 # Gumbi: Gaussian Process Model Building Interface
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/JohnGoertz/Gumbi/HEAD)
 
 ## Overview
```

### Comparing `gumbi-0.2.1/gumbi.egg-info/SOURCES.txt` & `gumbi-0.2.2/gumbi.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 docs/source/notebooks/examples/Cars_Dataset.ipynb
 docs/source/notebooks/examples/Latent_GP.ipynb
 docs/source/notebooks/examples/Multioutput_Regression.ipynb
 docs/source/notebooks/examples/Simple_Regression.ipynb
 docs/source/notebooks/getting_started/introduction.ipynb
 gumbi/__init__.py
 gumbi/aggregation.py
+gumbi/array_utils.py
 gumbi/arrays.py
 gumbi/plotting.py
 gumbi/versions.py
 gumbi.egg-info/PKG-INFO
 gumbi.egg-info/SOURCES.txt
 gumbi.egg-info/dependency_links.txt
 gumbi.egg-info/requires.txt
```

### Comparing `gumbi-0.2.1/setup.py` & `gumbi-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+"""
+Instructions for building the package.
+
+
+"""
+
 import pathlib as pl
 
 from setuptools import find_packages, setup
 
 DISTNAME = "gumbi"
 DESCRIPTION = "Gaussian Process Model Building Interface"
 AUTHOR = "John Goertz"
```

### Comparing `gumbi-0.2.1/tests/conftest.py` & `gumbi-0.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.1/tests/test_aggregation.py` & `gumbi-0.2.2/tests/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.1/tests/test_arrays.py` & `gumbi-0.2.2/tests/test_arrays.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.1/tests/test_plots.py` & `gumbi-0.2.2/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.1/tests/test_regression.py` & `gumbi-0.2.2/tests/test_regression.py`

 * *Files identical despite different names*

