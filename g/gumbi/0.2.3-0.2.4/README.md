# Comparing `tmp/gumbi-0.2.3.tar.gz` & `tmp/gumbi-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gumbi-0.2.3.tar", last modified: Mon Jun  3 01:58:12 2024, max compression
+gzip compressed data, was "gumbi-0.2.4.tar", last modified: Mon Jun  3 12:48:52 2024, max compression
```

## Comparing `gumbi-0.2.3.tar` & `gumbi-0.2.4.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-03 01:58:12.681445 gumbi-0.2.3/
--rw-r--r--   0 john      (1000) john      (1000)    11357 2024-01-03 05:03:41.000000 gumbi-0.2.3/LICENSE
--rw-r--r--   0 john      (1000) john      (1000)      235 2024-01-03 05:03:41.000000 gumbi-0.2.3/MANIFEST.in
--rw-r--r--   0 john      (1000) john      (1000)     3242 2024-06-03 01:58:12.681445 gumbi-0.2.3/PKG-INFO
--rw-r--r--   0 john      (1000) john      (1000)     2225 2024-01-03 05:03:41.000000 gumbi-0.2.3/README.md
--rw-r--r--   0 john      (1000) john      (1000)        6 2024-06-03 01:58:04.000000 gumbi-0.2.3/VERSION
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-03 01:58:12.681445 gumbi-0.2.3/docs/
--rw-r--r--   0 john      (1000) john      (1000)      122 2024-01-03 05:03:41.000000 gumbi-0.2.3/docs/requirements.txt
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-03 01:58:12.681445 gumbi-0.2.3/docs/source/
--rw-r--r--   0 john      (1000) john      (1000)     2829 2024-01-03 05:03:41.000000 gumbi-0.2.3/docs/source/conf.py
--rw-r--r--   0 john      (1000) john      (1000)      620 2024-01-03 05:03:41.000000 gumbi-0.2.3/docs/source/index.rst
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-03 01:58:12.681445 gumbi-0.2.3/docs/source/notebooks/
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-03 01:58:12.681445 gumbi-0.2.3/docs/source/notebooks/examples/
--rw-r--r--   0 john      (1000) john      (1000)  1505160 2024-01-03 05:03:41.000000 gumbi-0.2.3/docs/source/notebooks/examples/Cars_Dataset.ipynb
--rw-r--r--   0 john      (1000) john      (1000)  2084410 2024-05-31 21:25:49.000000 gumbi-0.2.3/docs/source/notebooks/examples/Latent_GP.ipynb
--rw-r--r--   0 john      (1000) john      (1000)   423694 2024-01-03 05:03:41.000000 gumbi-0.2.3/docs/source/notebooks/examples/Multioutput_Regression.ipynb
--rw-r--r--   0 john      (1000) john      (1000)   440843 2024-01-03 05:03:41.000000 gumbi-0.2.3/docs/source/notebooks/examples/Simple_Regression.ipynb
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-03 01:58:12.681445 gumbi-0.2.3/docs/source/notebooks/getting_started/
--rw-r--r--   0 john      (1000) john      (1000)    41212 2024-01-03 05:03:41.000000 gumbi-0.2.3/docs/source/notebooks/getting_started/introduction.ipynb
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-03 01:58:12.681445 gumbi-0.2.3/gumbi/
--rw-r--r--   0 john      (1000) john      (1000)      430 2024-05-31 19:44:55.000000 gumbi-0.2.3/gumbi/__init__.py
--rw-r--r--   0 john      (1000) john      (1000)    35001 2024-05-31 21:13:11.000000 gumbi-0.2.3/gumbi/aggregation.py
--rw-r--r--   0 john      (1000) john      (1000)     1177 2024-05-31 19:45:21.000000 gumbi-0.2.3/gumbi/array_utils.py
--rw-r--r--   0 john      (1000) john      (1000)    57761 2024-01-10 20:10:43.000000 gumbi-0.2.3/gumbi/arrays.py
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-03 01:58:12.681445 gumbi-0.2.3/gumbi/data/
--rw-r--r--   0 john      (1000) john      (1000)   552642 2024-01-03 05:03:41.000000 gumbi-0.2.3/gumbi/data/Example_DataSet.pkl
--rw-r--r--   0 john      (1000) john      (1000)      136 2024-01-03 05:03:41.000000 gumbi-0.2.3/gumbi/data/__init__.py
--rw-r--r--   0 john      (1000) john      (1000)    16993 2024-01-03 05:03:41.000000 gumbi-0.2.3/gumbi/plotting.py
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-03 01:58:12.681445 gumbi-0.2.3/gumbi/regression/
--rw-r--r--   0 john      (1000) john      (1000)      124 2024-01-03 05:03:41.000000 gumbi-0.2.3/gumbi/regression/__init__.py
--rw-r--r--   0 john      (1000) john      (1000)    52482 2024-06-02 00:26:25.000000 gumbi-0.2.3/gumbi/regression/base.py
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-03 01:58:12.681445 gumbi-0.2.3/gumbi/regression/pymc/
--rw-r--r--   0 john      (1000) john      (1000)    38937 2024-06-03 01:57:42.000000 gumbi-0.2.3/gumbi/regression/pymc/GP.py
--rw-r--r--   0 john      (1000) john      (1000)        0 2024-01-03 05:03:41.000000 gumbi-0.2.3/gumbi/regression/pymc/__init__.py
--rw-r--r--   0 john      (1000) john      (1000)     1858 2024-01-03 05:03:41.000000 gumbi-0.2.3/gumbi/regression/pymc/extras.py
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-03 01:58:12.681445 gumbi-0.2.3/gumbi/style/
--rw-r--r--   0 john      (1000) john      (1000)      236 2024-01-03 05:03:41.000000 gumbi-0.2.3/gumbi/style/__init__.py
--rw-r--r--   0 john      (1000) john      (1000)    33984 2024-01-03 05:03:41.000000 gumbi-0.2.3/gumbi/style/breve_presentation.mplstyle
--rw-r--r--   0 john      (1000) john      (1000)    33956 2024-01-03 05:03:41.000000 gumbi-0.2.3/gumbi/style/futura_presentation.mplstyle
--rw-r--r--   0 john      (1000) john      (1000)    33945 2024-01-03 05:03:41.000000 gumbi-0.2.3/gumbi/style/presentation.mplstyle
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-03 01:58:12.681445 gumbi-0.2.3/gumbi/utils/
--rw-r--r--   0 john      (1000) john      (1000)       76 2024-01-03 05:03:41.000000 gumbi-0.2.3/gumbi/utils/__init__.py
--rw-r--r--   0 john      (1000) john      (1000)     2031 2024-01-03 05:03:41.000000 gumbi-0.2.3/gumbi/utils/generic_utils.py
--rw-r--r--   0 john      (1000) john      (1000)     1920 2024-05-31 19:45:39.000000 gumbi-0.2.3/gumbi/utils/gp_utils.py
--rw-r--r--   0 john      (1000) john      (1000)     6044 2024-05-31 15:00:57.000000 gumbi-0.2.3/gumbi/utils/misc.py
--rw-r--r--   0 john      (1000) john      (1000)     1414 2024-01-03 05:03:41.000000 gumbi-0.2.3/gumbi/utils/pymc_utils.py
--rw-r--r--   0 john      (1000) john      (1000)      222 2024-01-03 05:03:41.000000 gumbi-0.2.3/gumbi/versions.py
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-03 01:58:12.681445 gumbi-0.2.3/gumbi.egg-info/
--rw-r--r--   0 john      (1000) john      (1000)     3242 2024-06-03 01:58:12.000000 gumbi-0.2.3/gumbi.egg-info/PKG-INFO
--rw-r--r--   0 john      (1000) john      (1000)     1269 2024-06-03 01:58:12.000000 gumbi-0.2.3/gumbi.egg-info/SOURCES.txt
--rw-r--r--   0 john      (1000) john      (1000)        1 2024-06-03 01:58:12.000000 gumbi-0.2.3/gumbi.egg-info/dependency_links.txt
--rw-r--r--   0 john      (1000) john      (1000)       77 2024-06-03 01:58:12.000000 gumbi-0.2.3/gumbi.egg-info/requires.txt
--rw-r--r--   0 john      (1000) john      (1000)       12 2024-06-03 01:58:12.000000 gumbi-0.2.3/gumbi.egg-info/top_level.txt
--rw-r--r--   0 john      (1000) john      (1000)      213 2024-01-03 05:03:41.000000 gumbi-0.2.3/pyproject.toml
--rw-r--r--   0 john      (1000) john      (1000)      104 2024-01-03 05:03:41.000000 gumbi-0.2.3/requirements.txt
--rw-r--r--   0 john      (1000) john      (1000)      205 2024-06-03 01:58:12.681445 gumbi-0.2.3/setup.cfg
--rw-r--r--   0 john      (1000) john      (1000)     1799 2024-06-02 00:31:10.000000 gumbi-0.2.3/setup.py
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-03 01:58:12.681445 gumbi-0.2.3/tests/
--rw-r--r--   0 john      (1000) john      (1000)        0 2024-01-03 05:03:41.000000 gumbi-0.2.3/tests/__init__.py
--rw-r--r--   0 john      (1000) john      (1000)      615 2024-01-03 05:03:41.000000 gumbi-0.2.3/tests/conftest.py
--rw-r--r--   0 john      (1000) john      (1000)     3983 2024-01-03 05:03:41.000000 gumbi-0.2.3/tests/test_aggregation.py
--rw-r--r--   0 john      (1000) john      (1000)     6873 2024-01-03 05:03:41.000000 gumbi-0.2.3/tests/test_arrays.py
--rw-r--r--   0 john      (1000) john      (1000)     4031 2024-01-03 05:03:41.000000 gumbi-0.2.3/tests/test_plots.py
--rw-r--r--   0 john      (1000) john      (1000)     6391 2024-01-03 05:03:41.000000 gumbi-0.2.3/tests/test_regression.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-03 12:48:51.992640 gumbi-0.2.4/
+-rw-r--r--   0 john      (1000) john      (1000)    11357 2024-01-03 05:03:41.000000 gumbi-0.2.4/LICENSE
+-rw-r--r--   0 john      (1000) john      (1000)      235 2024-01-03 05:03:41.000000 gumbi-0.2.4/MANIFEST.in
+-rw-r--r--   0 john      (1000) john      (1000)     3242 2024-06-03 12:48:51.992640 gumbi-0.2.4/PKG-INFO
+-rw-r--r--   0 john      (1000) john      (1000)     2225 2024-01-03 05:03:41.000000 gumbi-0.2.4/README.md
+-rw-r--r--   0 john      (1000) john      (1000)        6 2024-06-03 12:48:47.000000 gumbi-0.2.4/VERSION
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-03 12:48:51.982640 gumbi-0.2.4/docs/
+-rw-r--r--   0 john      (1000) john      (1000)      122 2024-01-03 05:03:41.000000 gumbi-0.2.4/docs/requirements.txt
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-03 12:48:51.982640 gumbi-0.2.4/docs/source/
+-rw-r--r--   0 john      (1000) john      (1000)     2829 2024-01-03 05:03:41.000000 gumbi-0.2.4/docs/source/conf.py
+-rw-r--r--   0 john      (1000) john      (1000)      620 2024-01-03 05:03:41.000000 gumbi-0.2.4/docs/source/index.rst
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-03 12:48:51.982640 gumbi-0.2.4/docs/source/notebooks/
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-03 12:48:51.992640 gumbi-0.2.4/docs/source/notebooks/examples/
+-rw-r--r--   0 john      (1000) john      (1000)  1505160 2024-01-03 05:03:41.000000 gumbi-0.2.4/docs/source/notebooks/examples/Cars_Dataset.ipynb
+-rw-r--r--   0 john      (1000) john      (1000)  2084410 2024-05-31 21:25:49.000000 gumbi-0.2.4/docs/source/notebooks/examples/Latent_GP.ipynb
+-rw-r--r--   0 john      (1000) john      (1000)   423694 2024-01-03 05:03:41.000000 gumbi-0.2.4/docs/source/notebooks/examples/Multioutput_Regression.ipynb
+-rw-r--r--   0 john      (1000) john      (1000)   440843 2024-01-03 05:03:41.000000 gumbi-0.2.4/docs/source/notebooks/examples/Simple_Regression.ipynb
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-03 12:48:51.992640 gumbi-0.2.4/docs/source/notebooks/getting_started/
+-rw-r--r--   0 john      (1000) john      (1000)    41212 2024-01-03 05:03:41.000000 gumbi-0.2.4/docs/source/notebooks/getting_started/introduction.ipynb
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-03 12:48:51.992640 gumbi-0.2.4/gumbi/
+-rw-r--r--   0 john      (1000) john      (1000)      430 2024-05-31 19:44:55.000000 gumbi-0.2.4/gumbi/__init__.py
+-rw-r--r--   0 john      (1000) john      (1000)    35001 2024-05-31 21:13:11.000000 gumbi-0.2.4/gumbi/aggregation.py
+-rw-r--r--   0 john      (1000) john      (1000)     1177 2024-05-31 19:45:21.000000 gumbi-0.2.4/gumbi/array_utils.py
+-rw-r--r--   0 john      (1000) john      (1000)    57761 2024-01-10 20:10:43.000000 gumbi-0.2.4/gumbi/arrays.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-03 12:48:51.992640 gumbi-0.2.4/gumbi/data/
+-rw-r--r--   0 john      (1000) john      (1000)   552642 2024-01-03 05:03:41.000000 gumbi-0.2.4/gumbi/data/Example_DataSet.pkl
+-rw-r--r--   0 john      (1000) john      (1000)      136 2024-01-03 05:03:41.000000 gumbi-0.2.4/gumbi/data/__init__.py
+-rw-r--r--   0 john      (1000) john      (1000)    16993 2024-01-03 05:03:41.000000 gumbi-0.2.4/gumbi/plotting.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-03 12:48:51.992640 gumbi-0.2.4/gumbi/regression/
+-rw-r--r--   0 john      (1000) john      (1000)      124 2024-01-03 05:03:41.000000 gumbi-0.2.4/gumbi/regression/__init__.py
+-rw-r--r--   0 john      (1000) john      (1000)    52523 2024-06-03 12:47:53.000000 gumbi-0.2.4/gumbi/regression/base.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-03 12:48:51.992640 gumbi-0.2.4/gumbi/regression/pymc/
+-rw-r--r--   0 john      (1000) john      (1000)    38937 2024-06-03 01:57:42.000000 gumbi-0.2.4/gumbi/regression/pymc/GP.py
+-rw-r--r--   0 john      (1000) john      (1000)        0 2024-01-03 05:03:41.000000 gumbi-0.2.4/gumbi/regression/pymc/__init__.py
+-rw-r--r--   0 john      (1000) john      (1000)     1858 2024-01-03 05:03:41.000000 gumbi-0.2.4/gumbi/regression/pymc/extras.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-03 12:48:51.992640 gumbi-0.2.4/gumbi/style/
+-rw-r--r--   0 john      (1000) john      (1000)      236 2024-01-03 05:03:41.000000 gumbi-0.2.4/gumbi/style/__init__.py
+-rw-r--r--   0 john      (1000) john      (1000)    33984 2024-01-03 05:03:41.000000 gumbi-0.2.4/gumbi/style/breve_presentation.mplstyle
+-rw-r--r--   0 john      (1000) john      (1000)    33956 2024-01-03 05:03:41.000000 gumbi-0.2.4/gumbi/style/futura_presentation.mplstyle
+-rw-r--r--   0 john      (1000) john      (1000)    33945 2024-01-03 05:03:41.000000 gumbi-0.2.4/gumbi/style/presentation.mplstyle
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-03 12:48:51.992640 gumbi-0.2.4/gumbi/utils/
+-rw-r--r--   0 john      (1000) john      (1000)       76 2024-01-03 05:03:41.000000 gumbi-0.2.4/gumbi/utils/__init__.py
+-rw-r--r--   0 john      (1000) john      (1000)     2031 2024-01-03 05:03:41.000000 gumbi-0.2.4/gumbi/utils/generic_utils.py
+-rw-r--r--   0 john      (1000) john      (1000)     1920 2024-05-31 19:45:39.000000 gumbi-0.2.4/gumbi/utils/gp_utils.py
+-rw-r--r--   0 john      (1000) john      (1000)     6044 2024-05-31 15:00:57.000000 gumbi-0.2.4/gumbi/utils/misc.py
+-rw-r--r--   0 john      (1000) john      (1000)     1414 2024-01-03 05:03:41.000000 gumbi-0.2.4/gumbi/utils/pymc_utils.py
+-rw-r--r--   0 john      (1000) john      (1000)      222 2024-01-03 05:03:41.000000 gumbi-0.2.4/gumbi/versions.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-03 12:48:51.992640 gumbi-0.2.4/gumbi.egg-info/
+-rw-r--r--   0 john      (1000) john      (1000)     3242 2024-06-03 12:48:51.000000 gumbi-0.2.4/gumbi.egg-info/PKG-INFO
+-rw-r--r--   0 john      (1000) john      (1000)     1269 2024-06-03 12:48:51.000000 gumbi-0.2.4/gumbi.egg-info/SOURCES.txt
+-rw-r--r--   0 john      (1000) john      (1000)        1 2024-06-03 12:48:51.000000 gumbi-0.2.4/gumbi.egg-info/dependency_links.txt
+-rw-r--r--   0 john      (1000) john      (1000)       77 2024-06-03 12:48:51.000000 gumbi-0.2.4/gumbi.egg-info/requires.txt
+-rw-r--r--   0 john      (1000) john      (1000)       12 2024-06-03 12:48:51.000000 gumbi-0.2.4/gumbi.egg-info/top_level.txt
+-rw-r--r--   0 john      (1000) john      (1000)      213 2024-01-03 05:03:41.000000 gumbi-0.2.4/pyproject.toml
+-rw-r--r--   0 john      (1000) john      (1000)      104 2024-01-03 05:03:41.000000 gumbi-0.2.4/requirements.txt
+-rw-r--r--   0 john      (1000) john      (1000)      205 2024-06-03 12:48:51.992640 gumbi-0.2.4/setup.cfg
+-rw-r--r--   0 john      (1000) john      (1000)     1799 2024-06-02 00:31:10.000000 gumbi-0.2.4/setup.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-06-03 12:48:51.992640 gumbi-0.2.4/tests/
+-rw-r--r--   0 john      (1000) john      (1000)        0 2024-01-03 05:03:41.000000 gumbi-0.2.4/tests/__init__.py
+-rw-r--r--   0 john      (1000) john      (1000)      615 2024-01-03 05:03:41.000000 gumbi-0.2.4/tests/conftest.py
+-rw-r--r--   0 john      (1000) john      (1000)     3983 2024-01-03 05:03:41.000000 gumbi-0.2.4/tests/test_aggregation.py
+-rw-r--r--   0 john      (1000) john      (1000)     6873 2024-01-03 05:03:41.000000 gumbi-0.2.4/tests/test_arrays.py
+-rw-r--r--   0 john      (1000) john      (1000)     4031 2024-01-03 05:03:41.000000 gumbi-0.2.4/tests/test_plots.py
+-rw-r--r--   0 john      (1000) john      (1000)     6391 2024-01-03 05:03:41.000000 gumbi-0.2.4/tests/test_regression.py
```

### Comparing `gumbi-0.2.3/LICENSE` & `gumbi-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.3/PKG-INFO` & `gumbi-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gumbi
-Version: 0.2.3
+Version: 0.2.4
 Summary: Gaussian Process Model Building Interface
 Home-page: https://github.com/JohnGoertz/Gumbi
 Author: John Goertz
 Author-email: 
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

### Comparing `gumbi-0.2.3/README.md` & `gumbi-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.3/docs/source/conf.py` & `gumbi-0.2.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.3/docs/source/index.rst` & `gumbi-0.2.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.3/docs/source/notebooks/examples/Cars_Dataset.ipynb` & `gumbi-0.2.4/docs/source/notebooks/examples/Cars_Dataset.ipynb`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.3/docs/source/notebooks/examples/Latent_GP.ipynb` & `gumbi-0.2.4/docs/source/notebooks/examples/Latent_GP.ipynb`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.3/docs/source/notebooks/examples/Multioutput_Regression.ipynb` & `gumbi-0.2.4/docs/source/notebooks/examples/Multioutput_Regression.ipynb`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.3/docs/source/notebooks/examples/Simple_Regression.ipynb` & `gumbi-0.2.4/docs/source/notebooks/examples/Simple_Regression.ipynb`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.3/docs/source/notebooks/getting_started/introduction.ipynb` & `gumbi-0.2.4/docs/source/notebooks/getting_started/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.3/gumbi/aggregation.py` & `gumbi-0.2.4/gumbi/aggregation.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.3/gumbi/array_utils.py` & `gumbi-0.2.4/gumbi/array_utils.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.3/gumbi/arrays.py` & `gumbi-0.2.4/gumbi/arrays.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.3/gumbi/data/Example_DataSet.pkl` & `gumbi-0.2.4/gumbi/data/Example_DataSet.pkl`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.3/gumbi/plotting.py` & `gumbi-0.2.4/gumbi/plotting.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.3/gumbi/regression/base.py` & `gumbi-0.2.4/gumbi/regression/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -404,18 +404,21 @@
         """
 
         df = self.get_filtered_data(standardized=False, metric=metric)
 
         # Ensure same number of observations for every output (only possible if something broke)
         assert len(set(sum(df[self.out_col] == output) for output in self.outputs)) == 1
 
-        # Assuming all parameters observed at the same points Extract the model dimensions from the dataframe for one of
-        # the parameters
-        dims = set(self.dims) - set([self.out_col])
-        dim_values = {dim: df[df[self.out_col] == self.outputs[0]].replace(self.coords)[dim].values for dim in dims}
+        # Assuming all parameters observed at the same points
+        inputs = inputs[inputs[self.out_col] == self.outputs[0]]
+        inputs = inputs.replace(self.coords)
+
+        # Extract the model dimensions from the dataframe
+        dims = [dim for dim in self.dims if dim != self.out_col]
+        dim_values = inputs[dims].to_dict(orient='list')
         X = self.parray(**dim_values, stdzd=False)
 
         # List of parrays for each output
         outputs = {output: df[df[self.out_col] == output]["Value"].values for output in self.outputs}
         y = self.parray(**outputs, stdzd=False)
 
         return X, y
```

### Comparing `gumbi-0.2.3/gumbi/regression/pymc/GP.py` & `gumbi-0.2.4/gumbi/regression/pymc/GP.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.3/gumbi/regression/pymc/extras.py` & `gumbi-0.2.4/gumbi/regression/pymc/extras.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.3/gumbi/style/breve_presentation.mplstyle` & `gumbi-0.2.4/gumbi/style/breve_presentation.mplstyle`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.3/gumbi/style/futura_presentation.mplstyle` & `gumbi-0.2.4/gumbi/style/futura_presentation.mplstyle`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.3/gumbi/style/presentation.mplstyle` & `gumbi-0.2.4/gumbi/style/presentation.mplstyle`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.3/gumbi/utils/generic_utils.py` & `gumbi-0.2.4/gumbi/utils/generic_utils.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.3/gumbi/utils/gp_utils.py` & `gumbi-0.2.4/gumbi/utils/gp_utils.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.3/gumbi/utils/misc.py` & `gumbi-0.2.4/gumbi/utils/misc.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.3/gumbi/utils/pymc_utils.py` & `gumbi-0.2.4/gumbi/utils/pymc_utils.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.3/gumbi.egg-info/PKG-INFO` & `gumbi-0.2.4/gumbi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gumbi
-Version: 0.2.3
+Version: 0.2.4
 Summary: Gaussian Process Model Building Interface
 Home-page: https://github.com/JohnGoertz/Gumbi
 Author: John Goertz
 Author-email: 
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

### Comparing `gumbi-0.2.3/gumbi.egg-info/SOURCES.txt` & `gumbi-0.2.4/gumbi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.3/setup.py` & `gumbi-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.3/tests/conftest.py` & `gumbi-0.2.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.3/tests/test_aggregation.py` & `gumbi-0.2.4/tests/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.3/tests/test_arrays.py` & `gumbi-0.2.4/tests/test_arrays.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.3/tests/test_plots.py` & `gumbi-0.2.4/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.3/tests/test_regression.py` & `gumbi-0.2.4/tests/test_regression.py`

 * *Files identical despite different names*

