# Comparing `tmp/ebcpy-0.3.8.tar.gz` & `tmp/ebcpy-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebcpy-0.3.8.tar", last modified: Wed Sep 27 17:17:20 2023, max compression
+gzip compressed data, was "ebcpy-0.4.1.tar", last modified: Mon Jun  3 08:19:48 2024, max compression
```

## Comparing `ebcpy-0.3.8.tar` & `ebcpy-0.4.1.tar`

### file list

```diff
@@ -1,30 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 17:17:20.885149 ebcpy-0.3.8/
--rw-rw-rw-   0 root         (0) root         (0)     1613 2023-09-27 17:03:30.000000 ebcpy-0.3.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6552 2023-09-27 17:17:20.885149 ebcpy-0.3.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5514 2023-09-27 17:03:30.000000 ebcpy-0.3.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 17:17:20.885149 ebcpy-0.3.8/ebcpy/
--rw-rw-rw-   0 root         (0) root         (0)      313 2023-09-27 17:03:30.000000 ebcpy-0.3.8/ebcpy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22850 2023-09-27 17:03:30.000000 ebcpy-0.3.8/ebcpy/data_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 17:17:20.885149 ebcpy-0.3.8/ebcpy/modelica/
--rw-rw-rw-   0 root         (0) root         (0)     5695 2023-09-27 17:03:30.000000 ebcpy-0.3.8/ebcpy/modelica/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5817 2023-09-27 17:03:30.000000 ebcpy-0.3.8/ebcpy/modelica/manipulate_ds.py
--rw-rw-rw-   0 root         (0) root         (0)    13728 2023-09-27 17:03:30.000000 ebcpy-0.3.8/ebcpy/modelica/simres.py
--rw-rw-rw-   0 root         (0) root         (0)    19180 2023-09-27 17:03:30.000000 ebcpy-0.3.8/ebcpy/optimization.py
--rw-rw-rw-   0 root         (0) root         (0)    24847 2023-09-27 17:03:30.000000 ebcpy-0.3.8/ebcpy/preprocessing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 17:17:20.885149 ebcpy-0.3.8/ebcpy/simulationapi/
--rw-rw-rw-   0 root         (0) root         (0)    22093 2023-09-27 17:03:30.000000 ebcpy-0.3.8/ebcpy/simulationapi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    49673 2023-09-27 17:03:30.000000 ebcpy-0.3.8/ebcpy/simulationapi/dymola_api.py
--rw-rw-rw-   0 root         (0) root         (0)    15301 2023-09-27 17:03:30.000000 ebcpy-0.3.8/ebcpy/simulationapi/fmu.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 17:17:20.885149 ebcpy-0.3.8/ebcpy/utils/
--rw-rw-rw-   0 root         (0) root         (0)     1384 2023-09-27 17:03:30.000000 ebcpy-0.3.8/ebcpy/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8478 2023-09-27 17:03:30.000000 ebcpy-0.3.8/ebcpy/utils/conversion.py
--rw-rw-rw-   0 root         (0) root         (0)    13538 2023-09-27 17:03:30.000000 ebcpy-0.3.8/ebcpy/utils/reproduction.py
--rw-rw-rw-   0 root         (0) root         (0)     6737 2023-09-27 17:03:30.000000 ebcpy-0.3.8/ebcpy/utils/statistics_analyzer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 17:17:20.885149 ebcpy-0.3.8/ebcpy.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6552 2023-09-27 17:17:20.000000 ebcpy-0.3.8/ebcpy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      553 2023-09-27 17:17:20.000000 ebcpy-0.3.8/ebcpy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-27 17:17:20.000000 ebcpy-0.3.8/ebcpy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      238 2023-09-27 17:17:20.000000 ebcpy-0.3.8/ebcpy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-09-27 17:17:20.000000 ebcpy-0.3.8/ebcpy.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-09-27 17:17:20.885149 ebcpy-0.3.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2647 2023-09-27 17:03:30.000000 ebcpy-0.3.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 08:19:48.067281 ebcpy-0.4.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2024-06-03 08:18:21.000000 ebcpy-0.4.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6881 2024-06-03 08:19:48.067281 ebcpy-0.4.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5298 2024-06-03 08:18:21.000000 ebcpy-0.4.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 08:19:48.059281 ebcpy-0.4.1/ebcpy/
+-rw-rw-rw-   0 root         (0) root         (0)      313 2024-06-03 08:18:21.000000 ebcpy-0.4.1/ebcpy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    24053 2024-06-03 08:18:21.000000 ebcpy-0.4.1/ebcpy/data_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 08:19:48.063281 ebcpy-0.4.1/ebcpy/modelica/
+-rw-rw-rw-   0 root         (0) root         (0)     5695 2024-06-03 08:18:21.000000 ebcpy-0.4.1/ebcpy/modelica/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6146 2024-06-03 08:18:21.000000 ebcpy-0.4.1/ebcpy/modelica/manipulate_ds.py
+-rw-rw-rw-   0 root         (0) root         (0)    14002 2024-06-03 08:18:21.000000 ebcpy-0.4.1/ebcpy/modelica/simres.py
+-rw-rw-rw-   0 root         (0) root         (0)    20297 2024-06-03 08:18:21.000000 ebcpy-0.4.1/ebcpy/optimization.py
+-rw-rw-rw-   0 root         (0) root         (0)    25969 2024-06-03 08:18:21.000000 ebcpy-0.4.1/ebcpy/preprocessing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 08:19:48.063281 ebcpy-0.4.1/ebcpy/simulationapi/
+-rw-rw-rw-   0 root         (0) root         (0)    24229 2024-06-03 08:18:21.000000 ebcpy-0.4.1/ebcpy/simulationapi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    56537 2024-06-03 08:18:21.000000 ebcpy-0.4.1/ebcpy/simulationapi/dymola_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    15617 2024-06-03 08:18:21.000000 ebcpy-0.4.1/ebcpy/simulationapi/fmu.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 08:19:48.063281 ebcpy-0.4.1/ebcpy/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     1647 2024-06-03 08:18:21.000000 ebcpy-0.4.1/ebcpy/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8478 2024-06-03 08:18:21.000000 ebcpy-0.4.1/ebcpy/utils/conversion.py
+-rw-rw-rw-   0 root         (0) root         (0)    13538 2024-06-03 08:18:21.000000 ebcpy-0.4.1/ebcpy/utils/reproduction.py
+-rw-rw-rw-   0 root         (0) root         (0)     6737 2024-06-03 08:18:21.000000 ebcpy-0.4.1/ebcpy/utils/statistics_analyzer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 08:19:48.067281 ebcpy-0.4.1/ebcpy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6881 2024-06-03 08:19:48.000000 ebcpy-0.4.1/ebcpy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      724 2024-06-03 08:19:48.000000 ebcpy-0.4.1/ebcpy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 08:19:48.000000 ebcpy-0.4.1/ebcpy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      246 2024-06-03 08:19:48.000000 ebcpy-0.4.1/ebcpy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-06-03 08:19:48.000000 ebcpy-0.4.1/ebcpy.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       79 2024-06-03 08:19:48.067281 ebcpy-0.4.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2655 2024-06-03 08:18:21.000000 ebcpy-0.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 08:19:48.067281 ebcpy-0.4.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    13844 2024-06-03 08:18:21.000000 ebcpy-0.4.1/tests/test_data_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     1773 2024-06-03 08:18:21.000000 ebcpy-0.4.1/tests/test_examples.py
+-rw-rw-rw-   0 root         (0) root         (0)     5412 2024-06-03 08:18:21.000000 ebcpy-0.4.1/tests/test_modelica.py
+-rw-rw-rw-   0 root         (0) root         (0)     6052 2024-06-03 08:18:21.000000 ebcpy-0.4.1/tests/test_optimizer.py
+-rw-rw-rw-   0 root         (0) root         (0)    10815 2024-06-03 08:18:21.000000 ebcpy-0.4.1/tests/test_preprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)    12138 2024-06-03 08:18:21.000000 ebcpy-0.4.1/tests/test_simulationapi.py
+-rw-rw-rw-   0 root         (0) root         (0)    12312 2024-06-03 08:18:21.000000 ebcpy-0.4.1/tests/test_utils.py
```

### Comparing `ebcpy-0.3.8/LICENSE` & `ebcpy-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ebcpy-0.3.8/PKG-INFO` & `ebcpy-0.4.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,51 @@
 Metadata-Version: 2.1
 Name: ebcpy
-Version: 0.3.8
+Version: 0.4.1
 Summary: Python Library used for different python modules for the analysis and optimization of energy systems, buildings and indoor climate 
 Home-page: https://github.com/RWTH-EBC/ebcpy
+Download-URL: https://github.com/RWTH-EBC/ebcpy/archive/refs/tags/0.4.1.tar.gz
 Author: RWTH Aachen University, E.ON Energy Research Center, Institute of Energy Efficient Buildings and Indoor Climate
 Author-email: fabian.wuellhorst@eonerc.rwth-aachen.de
 License: BSD 3-Clause
-Download-URL: https://github.com/RWTH-EBC/ebcpy/archive/refs/tags/0.3.8.tar.gz
 Keywords: simulation,building,energy,time-series-data,comfort,black-box optimization
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
-Provides-Extra: full
 License-File: LICENSE
+Requires-Dist: numpy>=1.19.5
+Requires-Dist: matplotlib>=3.3.4
+Requires-Dist: scipy>=1.5.4
+Requires-Dist: pandas>=1.1.5
+Requires-Dist: scikit-learn>=0.24.2
+Requires-Dist: fmpy<0.3.17,>=0.2.27
+Requires-Dist: pydantic>=2.0
+Requires-Dist: h5py>=3.1.0
+Requires-Dist: tables>=3.6.1
+Provides-Extra: full
+Requires-Dist: openpyxl>=3.0.5; extra == "full"
+Requires-Dist: xlrd>=2.0.1; extra == "full"
+Requires-Dist: pymoo==0.5.0; extra == "full"
+Requires-Dist: GitPython>=3.1.27; extra == "full"
+Requires-Dist: pyarrow>=11.0.0; extra == "full"
+Requires-Dist: fastparquet>=2023.1.0; extra == "full"
 
 ![E.ON EBC RWTH Aachen University](./docs/EBC_Logo.png)
 
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.03861/status.svg)](https://doi.org/10.21105/joss.03861)
-[![pylint](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/pylint/pylint.svg )](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/pylint/pylint.html)
-[![documentation](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/docs/doc.svg)](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/docs/index.html)
-[![coverage](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/coverage/badge.svg)](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/coverage)
+[![pylint](https://rwth-ebc.github.io/ebcpy/master/pylint/pylint.svg )](https://rwth-ebc.github.io/ebcpy/master/pylint/pylint.html)
+[![documentation](https://rwth-ebc.github.io/ebcpy/master/docs/doc.svg)](https://rwth-ebc.github.io/ebcpy/master/docs/index.html)
+[![coverage](https://rwth-ebc.github.io/ebcpy/master/coverage/badge.svg)](https://rwth-ebc.github.io/ebcpy/master/coverage)
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
-[![build](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/build/build.svg)](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/build/build.svg)
+[![build](https://rwth-ebc.github.io/ebcpy/master/build/build.svg)](https://rwth-ebc.github.io/ebcpy/master/build/build.svg)
 
 
 # ebcpy
 
 This **PY**thon package provides generic functions and classes commonly
 used for the analysis and optimization of **e**nergy systems, **b**uildings and indoor **c**limate (**EBC**).
 
@@ -39,15 +53,15 @@
 
 * `TimeSeriesData`
 * `SimulationAPI`'s
 * Optimization wrapper
 * Pre-/Postprocessing
 * Modelica utilities
 
-It was developed together with `AixCaliBuHA`, a framework for an automated calibration of dynamic building and HVAC models. During this development, we found several interfaces relevant to further reserach. We thus decoupled these interfaces into `ebcpy` and used the framework, for instance in the design optimization of heat pump systems ([link](https://www.sciencedirect.com/science/article/abs/pii/S0196890421010645?via%3Dihub)).
+It was developed together with `AixCaliBuHA`, a framework for an automated calibration of dynamic building and HVAC models. During this development, we found several interfaces relevant to further research. We thus decoupled these interfaces into `ebcpy` and used the framework, for instance in the design optimization of heat pump systems ([link](https://www.sciencedirect.com/science/article/abs/pii/S0196890421010645?via%3Dihub)).
 
 # Installation
 
 To install, simply run
 ```
 pip install ebcpy
 ```
@@ -146,13 +160,11 @@
 # From float to datetime
 tsd.to_datetime_index()
 # To clean your data and create a common frequency:
 tsd.clean_and_space_equally(desired_freq="1s")
 ```
 
 # Documentation
-Visit our official [Documentation](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/docs/index.html).
+Visit our official [Documentation](https://rwth-ebc.github.io/ebcpy/master/docs/index.html).
 
 # Problems?
 Please [raise an issue here](https://github.com/RWTH-EBC/ebcpy/issues/new).
-
-
```

### Comparing `ebcpy-0.3.8/README.md` & `ebcpy-0.4.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ![E.ON EBC RWTH Aachen University](./docs/EBC_Logo.png)
 
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.03861/status.svg)](https://doi.org/10.21105/joss.03861)
-[![pylint](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/pylint/pylint.svg )](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/pylint/pylint.html)
-[![documentation](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/docs/doc.svg)](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/docs/index.html)
-[![coverage](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/coverage/badge.svg)](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/coverage)
+[![pylint](https://rwth-ebc.github.io/ebcpy/master/pylint/pylint.svg )](https://rwth-ebc.github.io/ebcpy/master/pylint/pylint.html)
+[![documentation](https://rwth-ebc.github.io/ebcpy/master/docs/doc.svg)](https://rwth-ebc.github.io/ebcpy/master/docs/index.html)
+[![coverage](https://rwth-ebc.github.io/ebcpy/master/coverage/badge.svg)](https://rwth-ebc.github.io/ebcpy/master/coverage)
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
-[![build](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/build/build.svg)](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/build/build.svg)
+[![build](https://rwth-ebc.github.io/ebcpy/master/build/build.svg)](https://rwth-ebc.github.io/ebcpy/master/build/build.svg)
 
 
 # ebcpy
 
 This **PY**thon package provides generic functions and classes commonly
 used for the analysis and optimization of **e**nergy systems, **b**uildings and indoor **c**limate (**EBC**).
 
@@ -17,15 +17,15 @@
 
 * `TimeSeriesData`
 * `SimulationAPI`'s
 * Optimization wrapper
 * Pre-/Postprocessing
 * Modelica utilities
 
-It was developed together with `AixCaliBuHA`, a framework for an automated calibration of dynamic building and HVAC models. During this development, we found several interfaces relevant to further reserach. We thus decoupled these interfaces into `ebcpy` and used the framework, for instance in the design optimization of heat pump systems ([link](https://www.sciencedirect.com/science/article/abs/pii/S0196890421010645?via%3Dihub)).
+It was developed together with `AixCaliBuHA`, a framework for an automated calibration of dynamic building and HVAC models. During this development, we found several interfaces relevant to further research. We thus decoupled these interfaces into `ebcpy` and used the framework, for instance in the design optimization of heat pump systems ([link](https://www.sciencedirect.com/science/article/abs/pii/S0196890421010645?via%3Dihub)).
 
 # Installation
 
 To install, simply run
 ```
 pip install ebcpy
 ```
@@ -124,11 +124,11 @@
 # From float to datetime
 tsd.to_datetime_index()
 # To clean your data and create a common frequency:
 tsd.clean_and_space_equally(desired_freq="1s")
 ```
 
 # Documentation
-Visit our official [Documentation](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/docs/index.html).
+Visit our official [Documentation](https://rwth-ebc.github.io/ebcpy/master/docs/index.html).
 
 # Problems?
 Please [raise an issue here](https://github.com/RWTH-EBC/ebcpy/issues/new).
```

### Comparing `ebcpy-0.3.8/ebcpy/data_types.py` & `ebcpy-0.4.1/ebcpy/data_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,15 +78,18 @@
         Name of the sheet you want to load data from. Required keyword
         argument when loading a xlsx-file.
     :keyword str default_tag:
         Which value to use as tag. Default is 'raw'
     :keyword str engine:
         Chose the engine for reading .parquet files. Default is 'pyarrow'
         Other option is 'fastparquet' (python>=3.9).
-
+    :keyword list variable_names:
+        List of variable names to load from .mat file. If you
+        know which variables you want to plot, this may speed up
+        loading significantly, and reduce memory size drastically.
 
     Examples:
 
     First let's see the usage for a common dataframe.
 
     >>> import numpy as np
     >>> import pandas as pd
@@ -245,17 +248,18 @@
                                "specified to save a .hdf file")
             pd.DataFrame(self).to_hdf(filepath, key=kwargs.get("key"))
 
         elif filepath.suffix == ".csv":
             pd.DataFrame(self).to_csv(filepath, sep=kwargs.get("sep", ","))
         elif ".parquet" in filepath.name:
             parquet_split = filepath.name.split(".parquet")
-            pd.DataFrame(self).to_parquet(filepath, engine=kwargs.get('engine', 'pyarrow'),
-                                          compression=parquet_split[-1][1:] if parquet_split[-1] else None,
-                                          index=True)
+            pd.DataFrame(self).to_parquet(
+                filepath, engine=kwargs.get('engine', 'pyarrow'),
+                compression=parquet_split[-1][1:] if parquet_split[-1] else None,
+                index=True)
         else:
             raise TypeError("Given file-format is not supported."
                             "You can only store TimeSeriesData as .hdf, .csv, .parquet, "
                             "and .parquet.COMPRESSION_NAME with additional compression options")
 
     def to_df(self, force_single_index=False):
         """
@@ -313,15 +317,19 @@
             df = pd.read_csv(
                 file,
                 sep=self._loader_kwargs.get("sep", ","),
                 index_col=self._loader_kwargs.get("index_col", 0),
                 header=self._loader_kwargs.get("header", _hea_def)
             )
         elif file.suffix == ".mat":
-            df = sr.mat_to_pandas(fname=file, with_unit=False)
+            df = sr.mat_to_pandas(
+                fname=file,
+                with_unit=False,
+                names=self._loader_kwargs.get("variable_names")
+            )
         elif file.suffix in ['.xlsx', '.xls', '.odf', '.ods', '.odt']:
             sheet_name = self._loader_kwargs.get("sheet_name")
             if sheet_name is None:
                 raise KeyError("sheet_name is a required keyword argument to load xlsx-files."
                                "Please pass a string to specify the name "
                                "of the sheet you want to load.")
             df = pd.read_excel(io=file, sheet_name=sheet_name)
@@ -411,60 +419,81 @@
             return _ret
         if return_type.lower() in ['numpy', 'scipy', 'sp', 'np']:
             return _ret.to_numpy()
         if return_type.lower() == 'control':
             return _ret.to_numpy().transpose()
         raise TypeError("Unknown return type")
 
-    def to_datetime_index(self, unit_of_index="s", origin=datetime.now()):
+    def to_datetime_index(self, unit_of_index="s", origin=datetime.now(), inplace: bool = True):
         """
         Convert the current index to a float based index using
         ebcpy.preprocessing.convert_index_to_datetime_index()
 
         :param str unit_of_index: default 's'
             The unit of the given index. Used to convert to
             total_seconds later on.
         :param datetime.datetime origin:
             The reference datetime object for the first index.
             Default is the current system time.
+        :param bool inplace:
+            If True, performs operation inplace and returns None.
+        :return: df
+            Copy of DataFrame with correct index for usage in this
+            framework.
+
         """
-        preprocessing.convert_index_to_datetime_index(df=self,
-                                                      unit_of_index=unit_of_index,
-                                                      origin=origin)
+        return preprocessing.convert_index_to_datetime_index(df=self,
+                                                             unit_of_index=unit_of_index,
+                                                             origin=origin,
+                                                             inplace=inplace)
 
-    def to_float_index(self, offset=0):
+    def to_float_index(self, offset=0, inplace: bool = True):
         """
         Convert the current index to a float based index using
         ebcpy.preprocessing.convert_datetime_index_to_float_index()
 
         :param float offset:
             Offset in seconds
+        :param bool inplace:
+            If True, performs operation inplace and returns None.
+        :return: pd.DataFrame df:
+            DataFrame with correct index.
         """
         if not isinstance(self.index, pd.DatetimeIndex):
             return
-        preprocessing.convert_datetime_index_to_float_index(df=self,
-                                                            offset=offset)
 
-    def clean_and_space_equally(self, desired_freq):
+        return preprocessing.convert_datetime_index_to_float_index(df=self,
+                                                                   offset=offset,
+                                                                   inplace=inplace)
+
+    def clean_and_space_equally(self, desired_freq, inplace: bool = True):
         """
         Call to the preprocessing function
         ebcpy.preprocessing.clean_and_space_equally_time_series()
         See the docstring of this function to know what is happening.
 
         :param str desired_freq:
             Frequency to determine number of elements in processed dataframe.
             Options are for example:
             - s: second-based
             - 5s: Every 5 seconds
             - 6min: Every 6 minutes
             This also works for h, d, m, y, ms etc.
+        :param bool inplace:
+            If True, performs operation inplace and returns None.
+        :return: pd.DataFrame
+            Cleaned and equally spaced data-frame
         """
         df = preprocessing.clean_and_space_equally_time_series(df=self,
                                                                desired_freq=desired_freq)
-        super().__init__(df)
+        if inplace:
+            super().__init__(df)
+            return None
+        else:
+            return df
 
     def low_pass_filter(self, crit_freq, filter_order, variable,
                         tag=None, new_tag="low_pass_filter"):
         """
         Call to the preprocessing function
         ebcpy.preprocessing.low_pass_filter()
         See the docstring of this function to know what is happening.
```

### Comparing `ebcpy-0.3.8/ebcpy/modelica/__init__.py` & `ebcpy-0.4.1/ebcpy/modelica/__init__.py`

 * *Files identical despite different names*

### Comparing `ebcpy-0.3.8/ebcpy/modelica/manipulate_ds.py` & `ebcpy-0.4.1/ebcpy/modelica/manipulate_ds.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Functions to manipulate (or extract information of) the
 dsfinal.txt and dsin.txt files created by Modelica."""
 
 from io import StringIO
+import re
+
 import pandas as pd
 
 
 def convert_ds_file_to_dataframe(filename):
     """
     Function to convert a given dsfinal or dsfin file to a DataFrame.
     The index is the name of the variable. Further,
@@ -33,25 +35,32 @@
     column 6: Data type of variable and flags according to dsBaseType
 
     :param str,os.path.normpath filename:
         Filepath to the dsfinal or dsinto be loaded.
     :return: pd.DataFrame
         Converted DataFrame
     """
-    # Define relevant parameters
-    number_line_initial_name = 104  # Line where the string char initialName(,) is always stored
-
     # Open file and get relevant content by splitting the lines.
     with open(filename, "r") as file:
         content = file.read().split("\n")
 
     # Gets the X out of 'char initialName(X,Y)'
-    size_initial_names = int(content[number_line_initial_name].split("(")[-1].split(",")[0])
+    pattern_size_initial_name = r'^char initialName\((\d+),(\d+)\)$'
+    for number_line_initial_name, line in enumerate(content):
+        match_size_initial_name = re.match(pattern_size_initial_name, line)
+        if match_size_initial_name:
+            size_initial_names = int(match_size_initial_name.string.split("(")[-1].split(",")[0])
+            break
+    else:
+        raise ValueError("Could not find initial names in file")
+
     # Number of line below line "double initialValue(X,Y)"
     number_line_initial_value = number_line_initial_name + size_initial_names + 3
+    if "double initialValue" in content[number_line_initial_value]:
+        number_line_initial_value += 1
 
     # Check if two or on-line dsfinal / dsin
     if "#" in content[number_line_initial_value]:
         step_size = 1
     else:
         step_size = 2
```

### Comparing `ebcpy-0.3.8/ebcpy/modelica/simres.py` & `ebcpy-0.4.1/ebcpy/modelica/simres.py`

 * *Files 4% similar despite different names*

```diff
@@ -290,14 +290,18 @@
     if aliases is None:
         aliases = {}
 
     # Create the list of variable names.
     if names:
         if 'Time' not in names:
             names.append('Time')
+        non_existing_variables = list(set(names).difference(_variables.keys()))
+        if non_existing_variables:
+            raise KeyError(f"The following variable names are not in the given .mat file: "
+                           f"{', '.join(non_existing_variables)}")
     else:
         names = _variables.keys()
 
     # Create a dictionary of names and values.
     times = _variables['Time'].values()
     data = {}
     for name in names:
```

### Comparing `ebcpy-0.3.8/ebcpy/optimization.py` & `ebcpy-0.4.1/ebcpy/optimization.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Base-module for the whole optimization pacakge.
 Used to define Base-Classes such as Optimizer and
 Calibrator."""
 
 import os
+from pathlib import Path
+import warnings
 from typing import List, Tuple, Union
 from collections import namedtuple
 from abc import abstractmethod
 import numpy as np
 from ebcpy.utils import setup_logger
 # pylint: disable=import-outside-toplevel
 # pylint: disable=broad-except
@@ -20,15 +22,15 @@
     The main feature of this class is the common interface
     for different available solvers in python. This makes the
     testing of different solvers and methods more easy.
     For available frameworks/solvers, check the function
     self.optimize().
 
 
-    :param str,os.path.normpath cd:
+    :param str,Path working_directory:
         Directory for storing all output of optimization via a logger.
     :keyword list bounds:
         The boundaries for the optimization variables.
     """
 
     # Used to display number of obj-function-calls
     _counter = 0
@@ -36,22 +38,25 @@
     _current_iterate = np.array([])
     # Used to access the best iterate if an optimization step fails
     _current_best_iterate = {"Objective": np.inf}
     # List storing every objective value for plotting and logging.
     # Can be used, but will enlarge runtime
     _obj_his = []
 
-    def __init__(self, cd=None, **kwargs):
+    def __init__(self, working_directory: Union[Path, str] = None, **kwargs):
         """Instantiate class parameters"""
-        if cd is None:
-            self._cd = None
+        if working_directory is None and "cd" in kwargs:
+            warnings.warn("cd was renamed to working_directory in all classes. Use working_directory instead.", category=DeprecationWarning)
+            self.working_directory = kwargs["cd"]
+        elif working_directory is None:
+            self._working_directory = None
         else:
-            self.cd = cd
+            self.working_directory = working_directory
 
-        self.logger = setup_logger(cd=self.cd, name=self.__class__.__name__)
+        self.logger = setup_logger(working_directory=self.working_directory, name=self.__class__.__name__)
         # Set kwargs
         self.bounds = kwargs.get("bounds", None)
 
     @abstractmethod
     def obj(self, xk, *args):
         """
         Base objective function. Overload this function and create your own
@@ -89,23 +94,35 @@
         """
         return ["scipy_minimize",
                 "scipy_differential_evolution",
                 "dlib_minimize",
                 "pymoo"]
 
     @property
-    def cd(self) -> str:
+    def working_directory(self) -> Path:
         """The current working directory"""
-        return self._cd
+        return self._working_directory
 
-    @cd.setter
-    def cd(self, cd: str):
+    @working_directory.setter
+    def working_directory(self, working_directory: Union[Path, str]):
         """Set current working directory"""
-        os.makedirs(cd, exist_ok=True)
-        self._cd = cd
+        if isinstance(working_directory, str):
+            working_directory = Path(working_directory)
+        os.makedirs(working_directory, exist_ok=True)
+        self._working_directory = working_directory
+
+    @property
+    def cd(self) -> Path:
+        warnings.warn("cd was renamed to working_directory in all classes. Use working_directory instead instead.", category=DeprecationWarning)
+        return self.working_directory
+
+    @cd.setter
+    def cd(self, cd: Union[Path, str]):
+        warnings.warn("cd was renamed to working_directory in all classes. Use working_directory instead instead.", category=DeprecationWarning)
+        self.working_directory = cd
 
     @property
     def bounds(self) -> List[Union[Tuple, List]]:
         """The boundaries of the optimization problem."""
         return self._bounds
 
     @bounds.setter
```

### Comparing `ebcpy-0.3.8/ebcpy/preprocessing.py` & `ebcpy-0.4.1/ebcpy/preprocessing.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,15 +76,16 @@
     # Set mean values in rows that were duplicates before
     for idx, values in zip(double_ind, mean_values):
         df_dropped.loc[idx] = values
 
     return df_dropped
 
 
-def convert_index_to_datetime_index(df, unit_of_index="s", origin=datetime.now()):
+def convert_index_to_datetime_index(df, unit_of_index="s", origin=datetime.now(),
+                                    inplace: bool = False):
     """
     Converts the index of the given DataFrame to a
     pandas.core.indexes.datetimes.DatetimeIndex.
 
     :param pd.DataFrame df:
         dataframe with index not being a DateTime.
         Only numeric indexes are supported. Every integer
@@ -92,16 +93,18 @@
         is in seocnds.
     :param str unit_of_index: default 's'
         The unit of the given index. Used to convert to
         total_seconds later on.
     :param datetime.datetime origin:
         The reference datetime object for the first index.
         Default is the current system time.
+    :param bool inplace:
+        If True, performs operation inplace and returns None.
     :return: df
-        DataFrame with correct index for usage in this
+        Copy of DataFrame with correct index for usage in this
         framework.
 
     Example:
 
     >>> import pandas as pd
     >>> df = pd.DataFrame(np.ones([3, 4]), columns=list('ABCD'))
     >>> print(df)
@@ -113,48 +116,54 @@
                            A    B    C    D
     2007-01-01 00:00:00  1.0  1.0  1.0  1.0
     2007-01-01 00:00:01  1.0  1.0  1.0  1.0
     2007-01-01 00:00:02  1.0  1.0  1.0  1.0
 
     """
     # Check for unit of given index. Maybe one uses hour-based data.
-    _unit_conversion_to_seconds = {"ms": 1e-3,
+    _unit_conversion_to_seconds = {"ms": 1e3,
                                    "s": 1,
-                                   "min": 1/60,
-                                   "h": 1/3600,
-                                   "d": 1/86400}
+                                   "min": 1 / 60,
+                                   "h": 1 / 3600,
+                                   "d": 1 / 86400}
     if unit_of_index not in _unit_conversion_to_seconds:
         raise ValueError("Given unit_of_index is not supported.")
     _unit_factor_to_seconds = _unit_conversion_to_seconds.get(unit_of_index)
 
-    #Convert
+    # Convert
     old_index = df.index.copy()
     # Check if already converted:
     if isinstance(old_index, pd.DatetimeIndex):
         return df
     # Convert strings to numeric values.
     old_index = pd.to_numeric(old_index)
     # Convert to seconds.
     old_index /= _unit_factor_to_seconds
     # Alter the index
-    df.index = pd.to_datetime(old_index, unit="s", origin=origin)
+    index = pd.to_datetime(old_index, unit="s", origin=origin)
+    if inplace:
+        df.index = index
+        return None
+    df_copy = df.copy()
+    df_copy.index = index
+    return df_copy
 
-    return df
 
-
-def convert_datetime_index_to_float_index(df, offset=0):
+def convert_datetime_index_to_float_index(df, offset=0, inplace: bool = False):
     """
     Convert a datetime-based index to FloatIndex (in seconds).
     Seconds are used as a standard unit as simulation software
     outputs data in seconds (e.g. Modelica)
 
     :param pd.DataFrame df:
         DataFrame to be converted to FloatIndex
     :param float offset:
         Offset in seconds
+    :param bool inplace:
+        If True, performs operation inplace and returns None.
     :return: pd.DataFrame df:
         DataFrame with correct index
 
     Example:
 
     >>> import pandas as pd
     >>> df = pd.DataFrame(np.ones([3, 4]), columns=list('ABCD'))
@@ -169,17 +178,21 @@
     1.0  1.0  1.0  1.0  1.0
     2.0  1.0  1.0  1.0  1.0
     """
     # Check correct input
     if not isinstance(df.index, pd.DatetimeIndex):
         raise IndexError("Given DataFrame has no DatetimeIndex, conversion not possible")
 
-    new_index = pd.to_timedelta(df.index - df.index[0]).total_seconds()
-    df.index = np.round(new_index, 4) + offset
-    return df
+    new_index = np.round(pd.to_timedelta(df.index - df.index[0]).total_seconds(), 4) + offset
+    if inplace:
+        df.index = new_index
+        return None
+    df_copy = df.copy()
+    df_copy.index = new_index
+    return df_copy
 
 
 def time_based_weighted_mean(df):
     """
     Creates the weighted mean according to time index that does not need to be equidistant.
     Further info:
     https://stackoverflow.com/questions/26343252/create-a-weighted-mean-for-a-irregular-timeseries-in-pandas
@@ -203,28 +216,28 @@
     >>> print(time_based_weighted_mean(df=df))
     [  3.55  13.55]
     """
 
     if not isinstance(df.index, pd.DatetimeIndex):
         raise IndexError(f"df.index must be DatetimeIndex, but it is {type(df.index)}.")
 
-    time_delta = [(x-y).total_seconds() for x, y in zip(df.index[1:], df.index[:-1])]
-    weights = [x+y for x, y in zip([0] + time_delta, time_delta + [0])]
+    time_delta = [(x - y).total_seconds() for x, y in zip(df.index[1:], df.index[:-1])]
+    weights = [x + y for x, y in zip([0] + time_delta, time_delta + [0])]
     # Create empty numpy array
     res = np.empty(len(df.columns))
     res[:] = np.nan
     for i, col_name in enumerate(df.columns):
         res[i] = np.average(df[col_name], weights=weights)
     return res
 
 
 def clean_and_space_equally_time_series(df, desired_freq, confidence_warning=0.95):
     """
     Function for cleaning of the given dataFrame and interpolating
-    based on the the given desired frequency. Linear interpolation
+    based on the given desired frequency. Linear interpolation
     is used.
 
     :param pd.DataFrame df:
         Unclean DataFrame. Needs to have a pd.DateTimeIndex
     :param str desired_freq:
         Frequency to determine number of elements in processed dataframe.
         Options are for example:
@@ -255,108 +268,110 @@
     >>> plt.show()
 
     .. versionchanged:: 0.1.7
     """
     # Convert indexes to datetime_index:
     if not isinstance(df.index, pd.DatetimeIndex):
         if isinstance(df, data_types.TimeSeriesData):
-            raise TypeError("DataFrame needs a DateTimeIndex for executing this function. "
-                            "Call to_datetime_index() to convert any index to "
+            raise TypeError("TimeSeriesData needs a DateTimeIndex for executing this function. "
+                            "Call convert_index_to_datetime_index() to convert any index to "
                             "a DateTimeIndex")
         # Else
         raise TypeError("DataFrame needs a DateTimeIndex for executing this function. "
                         "Call convert_index_to_datetime_index() to convert any index to "
                         "a DateTimeIndex")
-    #%% Check DataFrame for NANs
+    # %% Check DataFrame for NANs
     # Create a pandas Series with number of invalid values for each column of df
     series_with_na = df.isnull().sum()
     for name in series_with_na.index:
         if series_with_na.loc[name] > 0:
             # Print only columns with invalid values
             logger.info("%s has following number of invalid "
                         "values\n %s", name, series_with_na.loc[name])
     # Drop all rows where at least one NA exists
-    df = df.dropna(how='any')
+    df_temp = df.dropna(how='any')
 
     # Check if DataFrame still has non-numeric-values:
-    if not all(df.apply(lambda s: pd.to_numeric(s, errors='coerce').notnull().all())):
+    if not all(df_temp.apply(lambda s: pd.to_numeric(s, errors='coerce').notnull().all())):
         raise ValueError("Given DataFrame contains non-numeric values.")
 
     # Merge duplicate rows using mean.
-    df = build_average_on_duplicate_rows(df)
+    df_temp = build_average_on_duplicate_rows(df_temp)
 
     # Make user warning for two cases: Upsampling and data input without a freq:
     # Check if the frequency differs
-    old_freq, old_freq_std = get_df_index_frequency_mean_and_std(df_index=df.index)
+    old_freq, old_freq_std, old_freq_sem, time_steps = get_df_index_frequency_mean_and_std(
+        df_index=df_temp.index,
+        verbose=True)
     if old_freq_std > 0:
         _ns_to_s = 1e9
-        # Construct a frequency by converting it first to int, then to timedelta back again:
-        _artificial_freq = old_freq / _ns_to_s
+        # Calculate confidence interval of the mean value of the old frequency
         cfd_int = st.t.interval(confidence_warning,
-                                len(_artificial_freq)-1,
-                                loc=np.mean(_artificial_freq),
-                                scale=st.sem(_artificial_freq))
-        # Convert back to timedelta
-        cfd_int = pd.to_timedelta(cfd_int)
+                                time_steps - 1,
+                                loc=old_freq,
+                                scale=old_freq_sem)
+        # Convert to timedelta
+        cfd_int = pd.to_timedelta((cfd_int[0] * _ns_to_s, cfd_int[1] * _ns_to_s))
         _td_freq = pd.to_timedelta(desired_freq)
         if (_td_freq < cfd_int[0]) or (_td_freq > cfd_int[1]):
             in_seconds = np.array(cfd_int.values.tolist()) / _ns_to_s  # From nanoseconds
             warnings.warn(f"Input data has no frequency, but the desired frequency "
                           f"{_td_freq.value / _ns_to_s} seconds is outside the given "
-                          f"confidence interval {in_seconds} (in seconds). "
+                          f"confidence interval {in_seconds} (in seconds) "
                           "Carefully check the result to see if you "
                           "introduced errors to the data.")
 
-    #%% Re-sampling to new frequency with linear interpolation
+    # %% Re-sampling to new frequency with linear interpolation
     # Create new equally spaced DatetimeIndex. Last entry is always < df.index[-1]
     time_index = pd.date_range(start=df.index[0], end=df.index[-1], freq=desired_freq)
     new_freq, _ = get_df_index_frequency_mean_and_std(df_index=time_index)
 
     # Check if the user is trying to upsample the data:
     if old_freq_std == 0:
         if new_freq > old_freq:
             warnings.warn("You are upsampling your data. This may be dangerous. "
                           "Carefully check the result to see if you introduced errors to the data.")
 
     # Create an empty data frame
     # If multi-columns is used, first get the old index and make it empty:
-    multi_cols = df.columns
+    multi_cols = df_temp.columns
     if isinstance(multi_cols, pd.MultiIndex):
         empty_multi_cols = pd.MultiIndex.from_product([[] for _ in range(multi_cols.nlevels)],
                                                       names=multi_cols.names)
         df_time_temp = pd.DataFrame(index=time_index, columns=empty_multi_cols)
     else:
         df_time_temp = pd.DataFrame(index=time_index)
 
     # Insert temporary time_index into df. fill_value = 0 can only be used,
     # since all NaNs should be eliminated prior
-    df = df.radd(df_time_temp, axis='index', fill_value=0)
+    df_temp = df_temp.radd(df_time_temp, axis='index', fill_value=0)
     del df_time_temp
 
     # Interpolate linearly according to time index
-    df.interpolate(method='time', axis=0, inplace=True)
+    df_temp.interpolate(method='time', axis=0, inplace=True)
     # Determine Timedelta between current first index entry
     # in df and the first index entry that would be created
     # when applying df.resample() without loffset
-    delta_time = df.index[0] - df.resample(rule=desired_freq).first().first(desired_freq).index[0]
+    delta_time = df.index[0] - \
+                 df_temp.resample(rule=desired_freq).first().first(desired_freq).index[0]
     # Resample to equally spaced index.
     # All fields should already have a value. Thus NaNs and maybe +/- infs
     # should have been filtered beforehand.
 
     # Check if given dataframe was a TimeSeriesData object and of so, convert it as such
-    if isinstance(df, data_types.TimeSeriesData):
-        df = df.resample(rule=desired_freq).first()
-        df.index = df.index + to_offset(delta_time)
-        df = data_types.TimeSeriesData(df)
+    if isinstance(df_temp, data_types.TimeSeriesData):
+        df_temp = df_temp.resample(rule=desired_freq).first()
+        df_temp.index = df_temp.index + to_offset(delta_time)
+        df_temp = data_types.TimeSeriesData(df_temp)
     else:
-        df = df.resample(rule=desired_freq).first()
-        df.index = df.index + to_offset(delta_time)
+        df_temp = df_temp.resample(rule=desired_freq).first()
+        df_temp.index = df_temp.index + to_offset(delta_time)
     del delta_time
 
-    return df
+    return df_temp
 
 
 def low_pass_filter(data, crit_freq, filter_order):
     """
     Create a low pass filter with given order and frequency.
 
     :param numpy.ndarray data:
@@ -391,15 +406,15 @@
     return output
 
 
 def moving_average(data, window):
     """
     Creates a pandas Series as moving average of the input series.
 
-    :param pd.Series values:
+    :param pd.Series data:
         For dataframe e.g. df['a_col_name'].values
     :param int window:
         sample rate of input
     :return: numpy.array
         shape has (###,). First and last points of input Series are extrapolated as constant
         values (hold first and last point).
 
@@ -412,27 +427,27 @@
     >>> plt.plot(moving_average(series, 10), label="window=10")
     >>> plt.plot(moving_average(series, 50), label="window=50")
     >>> plt.plot(moving_average(series, 100), label="window=100")
     >>> plt.legend()
     >>> plt.show()
 
     """
-    if len(data.shape) > 1: # Check if given data has multiple dimensions
+    if len(data.shape) > 1:  # Check if given data has multiple dimensions
         if data.shape[1] == 1:
             data = data[:, 0]  # Resize to 1D-Array
         else:
             raise ValueError("Given data has multiple dimensions. "
                              "Only one-dimensional arrays are supported in this function.")
     window = int(window)
     weights = np.repeat(1.0, window) / window
     sma = np.convolve(data, weights, 'valid')
     # Create array with first entries and window/2 elements
-    fill_start = np.full((int(np.floor(window/2)), 1), sma[0])
+    fill_start = np.full((int(np.floor(window / 2)), 1), sma[0])
     # Same with last value of -data-
-    fill_end = np.full((int(np.ceil(window/2)) - 1, 1), sma[-1])
+    fill_end = np.full((int(np.ceil(window / 2)) - 1, 1), sma[-1])
     # Stack the arrays
     sma = np.concatenate((fill_start[:, 0], sma, fill_end[:, 0]), axis=0)
     return sma
 
 
 def create_on_off_signal(df, col_names, threshold, col_names_new,
                          tags="raw", new_tag="converted_signal"):
@@ -447,22 +462,22 @@
         Threshold for all column-names (single float) or
         a list with specific thresholds for specific columns.
     :param list col_names_new:
         New name for the signal-column
     :param str,list tags:
         If a 2-Level DataFrame for TimeSeriesData is used, one has to
         specify the tag of the variables. Default value is to use the "raw"
-        tag set in the TimeSeriesClass. However one can specify a list
+        tag set in the TimeSeriesClass. However, one can specify a list
         (Different tag for each variable), or on can pass a string
         (same tags for all given variables)
     :param str new_tag:
         The tag the newly created variable will hold. This can be used to
         indicate where the signal was converted from.
     :return: pd.DataFrame
-        Now with the created signals.
+        Copy of DataFrame with the created signals added.
 
     Example:
 
     >>> import matplotlib.pyplot as plt
     >>> import numpy as np
     >>> df = pd.DataFrame({"P_el": np.sin(np.linspace(-20, 20, 10000))*100})
     >>> df = create_on_off_signal(df, col_names=["P_el"],
@@ -476,31 +491,33 @@
     if isinstance(threshold, list):
         if len(col_names) != len(threshold):
             raise IndexError(f"Given lists differ in length. col_names: {len(col_names)}, "
                              f"threshold: {len(threshold)}")
     else:
         threshold = [threshold for _ in enumerate(col_names)]
     # Do on_off signal creation for all desired columns
+    df_copy = df.copy()
     if isinstance(df.columns, pd.MultiIndex):
         # Convert given tags to a list
         if isinstance(tags, str):
             tags = [tags for _ in enumerate(col_names)]
 
         for i, _ in enumerate(col_names):
             # Create zero-array
-            df.loc[:, (col_names_new[i], new_tag)] = 0.0
+            df_copy.loc[:, (col_names_new[i], new_tag)] = 0.0
             # Change all values to 1.0 according to threshold
-            df.loc[df[col_names[i], tags[i]] >= threshold[i], (col_names_new[i], new_tag)] = 1.0
+            df_copy.loc[
+                df_copy[col_names[i], tags[i]] >= threshold[i], (col_names_new[i], new_tag)] = 1.0
     else:
         for i, _ in enumerate(col_names):
             # Create zero-array
-            df.loc[:, col_names_new[i]] = 0.0
+            df_copy.loc[:, col_names_new[i]] = 0.0
             # Change all values to 1.0 according to threshold
-            df.loc[df[col_names[i]] >= threshold[i], col_names_new[i]] = 1.0
-    return df
+            df_copy.loc[df_copy[col_names[i]] >= threshold[i], col_names_new[i]] = 1.0
+    return df_copy
 
 
 def number_lines_totally_na(df):
     """
     Returns the number of rows in the given dataframe
     that are filled with NaN-values.
 
@@ -551,15 +568,15 @@
     >>> normal_dis = np.random.normal(0, 1, 1000)
     >>> res = z_score(normal_dis, limit=2)
     >>> values = normal_dis[res]
 
     """
     mean = np.mean(x)
     standard_deviation = np.std(x)
-    z_score_value = (x-mean)/standard_deviation
+    z_score_value = (x - mean) / standard_deviation
     return np.where(np.abs(z_score_value) > limit)[0]
 
 
 def modified_z_score(x, limit=3.5):
     """
     Calculate the modified z-score using the median
     and median average deviation of the given data.
@@ -576,16 +593,16 @@
     >>> import numpy as np
     >>> normal_dis = np.random.normal(0, 1, 1000)
     >>> res = modified_z_score(normal_dis, limit=2)
     >>> values = normal_dis[res]
 
     """
     median = np.median(x)
-    median_average_deviation = np.median(np.abs(x-median))
-    z_score_mod = 0.6745*(x-median)/median_average_deviation
+    median_average_deviation = np.median(np.abs(x - median))
+    z_score_mod = 0.6745 * (x - median) / median_average_deviation
     return np.where(np.abs(z_score_mod) > limit)[0]
 
 
 def interquartile_range(x):
     """
     Calculate interquartile range of given array.
     Returns the indices of values outside of the interquartile range.
@@ -641,24 +658,33 @@
     >>> ret = cross_validation(x, y)
     >>> len(ret)
     4
     """
     return model_selection.train_test_split(x, y, test_size=test_size)
 
 
-def get_df_index_frequency_mean_and_std(df_index: pd.Index):
+def get_df_index_frequency_mean_and_std(df_index: pd.Index, verbose: bool = False):
     """
     Function to get the mean and std of the index-frequency.
     If the index is a DatetimeIndex, the seconds are converted from nanoseconds
     to seconds.
     Else, seconds are assumed as values.
 
+    :param pd.Index df_index:
+        Time index.
+    :param bool verbose:
+        Default false. If true, additional to the mean value and standard deviation,
+        the standard error of the mean and number of time steps are returned.
+
     :returns:
         float: Mean value
         float: Standard deviation
     """
 
     if isinstance(df_index, pd.DatetimeIndex):
-        index_in_s = df_index.to_series().diff().dropna().values.astype(np.int64) * 1e-9
+        index_in_s = df_index.to_series().diff().dropna().values.astype(np.float64) * 1e-9
+    else:
+        index_in_s = df_index.to_series().diff().dropna().values.astype(np.float64)
+    if verbose:
+        return np.mean(index_in_s), np.std(index_in_s), st.sem(index_in_s), len(index_in_s)
     else:
-        index_in_s = df_index.to_series().diff().dropna().values.astype(np.int64)
-    return np.mean(index_in_s), np.std(index_in_s)
+        return np.mean(index_in_s), np.std(index_in_s)
```

### Comparing `ebcpy-0.3.8/ebcpy/simulationapi/__init__.py` & `ebcpy-0.4.1/ebcpy/simulationapi/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 """
 import pathlib
 import warnings
 import os
 import sys
 import itertools
 import time
+from pathlib import Path
 from datetime import timedelta
 from typing import Dict, Union, TypeVar, Any, List
 from abc import abstractmethod
 import multiprocessing as mp
 
 import pydantic
 from pydantic import BaseModel, Field, field_validator
@@ -141,15 +142,15 @@
 SimulationSetupClass = TypeVar("SimulationSetupClass", bound=SimulationSetup)
 
 
 class SimulationAPI:
     """Base-class for simulation apis. Every simulation-api class
     must inherit from this class. It defines the structure of each class.
 
-    :param str,os.path.normpath cd:
+    :param str,Path working_directory:
         Working directory path
     :param str model_name:
         Name of the model being simulated.
     :keyword int n_cpu:
         Number of cores to be used by simulation.
         If None is given, single core will be used.
         Maximum number equals the cpu count of the device.
@@ -158,21 +159,26 @@
 
     """
     _sim_setup_class: SimulationSetupClass = SimulationSetup
     _items_to_drop = [
         'pool',
     ]
 
-    def __init__(self, cd, model_name, **kwargs):
+    def __init__(self, working_directory: Union[Path, str], model_name: str, **kwargs):
         # Private helper attrs for multiprocessing
         self._n_sim_counter = 0
         self._n_sim_total = 0
         self._progress_int = 0
+        # Handle deprecation warning
+        self.working_directory = working_directory
+        self.logger = setup_logger(
+            working_directory=self.working_directory,
+            name=self.__class__.__name__
+        )
         # Setup the logger
-        self.logger = setup_logger(cd=cd, name=self.__class__.__name__)
         self.logger.info(f'{"-" * 25}Initializing class {self.__class__.__name__}{"-" * 25}')
         # Check multiprocessing
         self.n_cpu = kwargs.get("n_cpu", 1)
         if self.n_cpu > mp.cpu_count():
             raise ValueError(f"Given n_cpu '{self.n_cpu}' is greater "
                              "than the available number of "
                              f"cpus on your machine '{mp.cpu_count()}'")
@@ -181,20 +187,20 @@
             self.pool = mp.Pool(processes=self.n_cpu)
             self.use_mp = True
         else:
             self.pool = None
             self.use_mp = False
         # Setup the model
         self._sim_setup = self._sim_setup_class()
-        self.cd = cd
         self.inputs: Dict[str, Variable] = {}       # Inputs of model
         self.outputs: Dict[str, Variable] = {}      # Outputs of model
         self.parameters: Dict[str, Variable] = {}   # Parameter of model
         self.states: Dict[str, Variable] = {}       # States of model
         self.result_names = []
+        self._model_name = None
         self.model_name = model_name
 
     # MP-Functions
     @property
     def worker_idx(self):
         """Index of the current worker"""
         _id = mp.current_process()._identity
@@ -254,15 +260,15 @@
             - 'time_series': Returns a DataFrame with the results and does not store anything.
             Only variables specified in result_names will be returned.
             - 'last_point': Returns only the last point of the simulation.
             Relevant for integral metrics like energy consumption.
             Only variables specified in result_names will be returned.
             - 'savepath': Returns the savepath where the results are stored.
             Depending on the API, different kwargs may be used to specify file type etc.
-        :keyword str,os.path.normpath savepath:
+        :keyword str,Path savepath:
             If path is provided, the relevant simulation results will be saved
             in the given directory. For multiple parameter variations also a list
             of savepaths for each parameterset can be specified.
             The savepaths for each parameter set must be unique.
             Only relevant if return_option equals 'savepath' .
         :keyword str result_file_name:
             Name of the result file. Default is 'resultFile'.
@@ -288,40 +294,52 @@
             dataframe for each set is returned in a list
         """
         # Convert inputs to equally sized objects of lists:
         if parameters is None:
             parameters = [{}]
         if isinstance(parameters, dict):
             parameters = [parameters]
+
+        if return_option not in ["time_series", "savepath", "last_point"]:
+            raise ValueError(f"Given return option '{return_option}' is not supported.")
+
         new_kwargs = {}
         kwargs["return_option"] = return_option  # Update with arg
+        n_simulations = len(parameters)
         # Handle special case for saving files:
-        if return_option == "savepath" and len(parameters) > 1:
+        if return_option == "savepath" and n_simulations > 1:
             savepath = kwargs.get("savepath", [])
-            if isinstance(savepath, (str, os.PathLike)):
-                savepath = [savepath] * len(parameters)
+            if isinstance(savepath, (str, os.PathLike, Path)):
+                savepath = [savepath] * n_simulations
             result_file_name = kwargs.get("result_file_name", [])
-            if (len(set(savepath)) != len(parameters) and
-                    len(set(result_file_name)) != len(parameters)):
-                raise TypeError(
+            if isinstance(result_file_name, str):
+                result_file_name = [result_file_name] * n_simulations
+            if len(savepath) != len(result_file_name):
+                raise ValueError("Given savepath and result_file_name "
+                                 "have not the same length.")
+            joined_save_paths = []
+            for _single_save_path, _single_result_name in zip(savepath, result_file_name):
+                joined_save_paths.append(os.path.join(_single_save_path, _single_result_name))
+            if len(set(joined_save_paths)) != n_simulations:
+                raise ValueError(
                     "Simulating multiple parameter set's on "
-                    "the same savepath will overwrite old "
-                    "results or even cause errors. "
-                    "Specify a result_file_name or savepath for each "
-                    "parameter combination"
+                    "the same combination of savepath and result_file_name "
+                    "will override results or even cause errors. "
+                    "Specify a unique result_file_name-savepath combination "
+                    "for each parameter combination"
                 )
         for key, value in kwargs.items():
             if isinstance(value, list):
-                if len(value) != len(parameters):
+                if len(value) != n_simulations:
                     raise ValueError(f"Mismatch in multiprocessing of "
-                                     f"given parameters ({len(parameters)}) "
+                                     f"given parameters ({n_simulations}) "
                                      f"and given {key} ({len(value)})")
                 new_kwargs[key] = value
             else:
-                new_kwargs[key] = [value] * len(parameters)
+                new_kwargs[key] = [value] * n_simulations
         kwargs = []
         for _idx, _parameters in enumerate(parameters):
             kwargs.append(
                 {"parameters": _parameters,
                  **{key: value[_idx] for key, value in new_kwargs.items()}
                  }
             )
@@ -350,15 +368,15 @@
             sys.stderr.write("\r")
         else:
             results = [self._single_simulation(kwargs={
                 "parameters": _single_kwargs["parameters"],
                 "return_option": _single_kwargs["return_option"],
                 **_single_kwargs
             }) for _single_kwargs in kwargs]
-        self.logger.info(f"Finished {len(parameters)} simulations on {self.n_cpu} processes in "
+        self.logger.info(f"Finished {n_simulations} simulations on {self.n_cpu} processes in "
                          f"{timedelta(seconds=int(time.time() - t_sim_start))}")
         if len(results) == 1:
             return results[0]
         return results
 
     def _remaining_time(self, t1):
         """
@@ -427,19 +445,22 @@
 
     @property
     def model_name(self) -> str:
         """Name of the model being simulated"""
         return self._model_name
 
     @model_name.setter
-    def model_name(self, model_name):
+    def model_name(self, model_name: str):
         """
         Set new model_name and trigger further functions
         to load parameters etc.
         """
+        # Only update if the model_name actually changes
+        if self._model_name == model_name:
+            return
         self._model_name = model_name
         # Only update model if it's the first setup. On multiprocessing,
         # all objects are duplicated and thus this setter is triggered again.
         # This if statement catches this case.
         if self.worker_idx and self.use_mp:
             return
         # Empty all variables again.
@@ -462,28 +483,47 @@
         """
         Reimplement this to change variables etc.
         based on the new model.
         """
         raise NotImplementedError(f'{self.__class__.__name__}._update_model '
                                   f'function is not defined')
 
-    def set_cd(self, cd):
+    def set_working_directory(self, working_directory: Union[Path, str]):
         """Base function for changing the current working directory."""
-        self.cd = cd
+        self.working_directory = working_directory
 
     @property
-    def cd(self) -> str:
+    def working_directory(self) -> Path:
         """Get the current working directory"""
-        return self._cd
+        return self._working_directory
 
-    @cd.setter
-    def cd(self, cd: str):
+    @working_directory.setter
+    def working_directory(self, working_directory: Union[Path, str]):
         """Set the current working directory"""
-        os.makedirs(cd, exist_ok=True)
-        self._cd = cd
+        if isinstance(working_directory, str):
+            working_directory = Path(working_directory)
+        os.makedirs(working_directory, exist_ok=True)
+        self._working_directory = working_directory
+
+    def set_cd(self, cd: Union[Path, str]):
+        warnings.warn("cd was renamed to working_directory in all classes. "
+                      "Use working_directory instead instead.", category=DeprecationWarning)
+        self.working_directory = cd
+
+    @property
+    def cd(self) -> Path:
+        warnings.warn("cd was renamed to working_directory in all classes. "
+                      "Use working_directory instead instead.", category=DeprecationWarning)
+        return self.working_directory
+
+    @cd.setter
+    def cd(self, cd: Union[Path, str]):
+        warnings.warn("cd was renamed to working_directory in all classes. "
+                      "Use working_directory instead instead.", category=DeprecationWarning)
+        self.working_directory = cd
 
     @property
     def result_names(self) -> List[str]:
         """
         The variables names which to store in results.
 
         Returns:
```

### Comparing `ebcpy-0.3.8/ebcpy/simulationapi/dymola_api.py` & `ebcpy-0.4.1/ebcpy/simulationapi/dymola_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 """Module containing the DymolaAPI used for simulation
 of Modelica-Models."""
 
 import sys
 import os
 import shutil
-import pathlib
+import uuid
 import warnings
 import atexit
 import json
+import time
+import socket
+from pathlib import Path
+from contextlib import closing
 from typing import Union, List
+
 from pydantic import Field
 import pandas as pd
+
 from ebcpy import TimeSeriesData
 from ebcpy.modelica import manipulate_ds
 from ebcpy.simulationapi import SimulationSetup, SimulationAPI, \
     SimulationSetupClass, Variable
 from ebcpy.utils.conversion import convert_tsd_to_modelica_txt
 
 
@@ -36,34 +42,31 @@
                         "Radau", "Dopri45", "Dopri853", "Sdirk34hw"]
 
 
 class DymolaAPI(SimulationAPI):
     """
     API to a Dymola instance.
 
-    :param str,os.path.normpath cd:
+    :param str,Path working_directory:
         Dirpath for the current working directory of dymola
     :param str model_name:
-        Name of the model to be simulated
+        Name of the model to be simulated.
+        If None, it has to be provided prior to or when calling simulate().
     :param list packages:
         List with path's to the packages needed to simulate the model
     :keyword Boolean show_window:
         True to show the Dymola window. Default is False
     :keyword Boolean modify_structural_parameters:
         True to automatically set the structural parameters of the
         simulation model via Modelica modifiers. Default is True.
         See also the keyword ``structural_parameters``
         of the ``simulate`` function.
     :keyword Boolean equidistant_output:
         If True (Default), Dymola stores variables in an
         equisdistant output and does not store variables at events.
-    :keyword str dymola_path:
-         Path to the dymola installation on the device. Necessary
-         e.g. on linux, if we can't find the path automatically.
-         Example: ``dymola_path="C://Program Files//Dymola 2020x"``
     :keyword int n_restart:
         Number of iterations after which Dymola should restart.
         This is done to free memory. Default value -1. For values
         below 1 Dymola does not restart.
     :keyword bool extract_variables:
         If True (the default), all variables of the model will be extracted
         on init of this class.
@@ -82,34 +85,51 @@
         If given, the script is executed before closing Dymola.
     :keyword str dymola_version:
         Version of Dymola to use.
         If not given, newest version will be used.
         If given, the Version needs to be equal to the folder name
         of your installation.
 
-        **Example:** If you have two version installed at
+        **Example:** If you have two versions installed at
 
         - ``C://Program Files//Dymola 2021`` and
         - ``C://Program Files//Dymola 2020x``
 
         and you want to use Dymola 2020x, specify
         ``dymola_version='Dymola 2020x'``.
 
         This parameter is overwritten if ``dymola_path`` is specified.
+    :keyword str dymola_path:
+         Path to the dymola installation on the device. Necessary
+         e.g. on linux, if we can't find the path automatically.
+         Example: ``dymola_path="C://Program Files//Dymola 2020x"``
     :keyword str dymola_interface_path:
-        Only relevant for the case when the dymola-exe path
+        Direct path to the .egg-file of the dymola interface.
+        Only relevant when the dymola_path
         differs from the interface path.
+    :keyword str dymola_exe_path:
+        Direct path to the dymola executable.
+        Only relevant if the dymola installation do not follow
+        the official guideline.
+    :keyword float time_delay_between_starts:
+        If starting multiple Dymola instances on multiple
+        cores, a time delay between each start avoids weird
+        behaviour, such as requiring to set the C-Compiler again
+        as Dymola overrides the default .dymx setup file.
+        If you start e.g. 20 instances and specify `time_delay_between_starts=5`,
+        each 5 seconds one instance will start, taking in total
+        100 seconds. Default is no delay.
 
     Example:
 
     >>> import os
     >>> from ebcpy import DymolaAPI
     >>> # Specify the model name
     >>> model_name = "Modelica.Thermal.FluidHeatFlow.Examples.PumpAndValve"
-    >>> dym_api = DymolaAPI(cd=os.getcwd(),
+    >>> dym_api = DymolaAPI(working_directory=os.getcwd(),
     >>>                     model_name=model_name,
     >>>                     packages=[],
     >>>                     show_window=True)
     >>> dym_api.sim_setup = {"start_time": 100,
     >>>                      "stop_time": 200}
     >>> dym_api.simulate()
     >>> dym_api.close()
@@ -125,31 +145,41 @@
         "dymola_path",
         "equidistant_output",
         "n_restart",
         "debug",
         "mos_script_pre",
         "mos_script_post",
         "dymola_version",
-        "dymola_interface_path"
+        "dymola_interface_path",
+        "dymola_exe_path",
+        "time_delay_between_starts"
     ]
 
-    def __init__(self, cd, model_name, packages=None, **kwargs):
+    def __init__(
+            self,
+            working_directory: Union[Path, str],
+            model_name: str = None,
+            packages: List[Union[Path, str]] = None,
+            **kwargs
+    ):
         """Instantiate class objects."""
         self.dymola = None  # Avoid key-error in get-state. Instance attribute needs to be there.
         # Update kwargs with regard to what kwargs are supported.
         self.extract_variables = kwargs.pop("extract_variables", True)
         self.fully_initialized = False
         self.debug = kwargs.pop("debug", False)
         self.show_window = kwargs.pop("show_window", False)
         self.modify_structural_parameters = kwargs.pop("modify_structural_parameters", True)
         self.equidistant_output = kwargs.pop("equidistant_output", True)
         self.mos_script_pre = kwargs.pop("mos_script_pre", None)
         self.mos_script_post = kwargs.pop("mos_script_post", None)
         self.dymola_version = kwargs.pop("dymola_version", None)
         self.dymola_interface_path = kwargs.pop("dymola_interface_path", None)
+        self.dymola_exe_path = kwargs.pop("dymola_exe_path", None)
+        _time_delay_between_starts = kwargs.pop("time_delay_between_starts", 0)
         for mos_script in [self.mos_script_pre, self.mos_script_post]:
             if mos_script is not None:
                 if not os.path.isfile(mos_script):
                     raise FileNotFoundError(
                         f"Given mos_script '{mos_script}' does "
                         f"not exist."
                     )
@@ -161,55 +191,55 @@
 
         # Convert to modelica path
         if self.mos_script_pre is not None:
             self.mos_script_pre = self._make_modelica_normpath(self.mos_script_pre)
         if self.mos_script_post is not None:
             self.mos_script_post = self._make_modelica_normpath(self.mos_script_post)
 
-        super().__init__(cd=cd,
+        super().__init__(working_directory=working_directory,
                          model_name=model_name,
                          n_cpu=kwargs.pop("n_cpu", 1))
 
         # First import the dymola-interface
         dymola_path = kwargs.pop("dymola_path", None)
         if dymola_path is not None:
             if not os.path.exists(dymola_path):
                 raise FileNotFoundError(f"Given path '{dymola_path}' can not be found on "
                                         "your machine.")
-            _dym_install = dymola_path
         else:
             # Get the dymola-install-path:
             _dym_installations = self.get_dymola_install_paths()
             if _dym_installations:
                 if self.dymola_version:
-                    _found_version = False
-                    for _dym_install in _dym_installations:
-                        if _dym_install.endswith(self.dymola_version):
-                            _found_version = True
-                            break
-                    if not _found_version:
-                        raise ValueError(
-                            f"Given dymola_version '{self.dymola_version}' not found in "
-                            f"the list of dymola installations {_dym_installations}"
-                        )
+                    dymola_path = _get_dymola_path_of_version(
+                        dymola_installations=_dym_installations,
+                        dymola_version=self.dymola_version
+                    )
                 else:
-                    _dym_install = _dym_installations[0]  # 0 is the newest
-                self.logger.info("Using dymola installation at %s", _dym_install)
+                    dymola_path = _dym_installations[0]  # 0 is the newest
+                self.logger.info("Using dymola installation at %s", dymola_path)
             else:
-                raise FileNotFoundError("Could not find a dymola-interface on your machine.")
-        self.dymola_exe_path = self.get_dymola_path(_dym_install)
+                if self.dymola_exe_path is None or self.dymola_interface_path is None:
+                    raise FileNotFoundError(
+                        "Could not find dymola on your machine. "
+                        "Thus, not able to find the `dymola_exe_path` and `dymola_interface_path`. "
+                        "Either specify both or pass an existing `dymola_path`."
+                    )
+        self.dymola_path = dymola_path
+        if self.dymola_exe_path is None:
+            self.dymola_exe_path = self.get_dymola_exe_path(dymola_path)
         self.logger.info("Using dymola.exe: %s", self.dymola_exe_path)
         if self.dymola_interface_path is None:
-            self.dymola_interface_path = self.get_dymola_interface_path(_dym_install)
+            self.dymola_interface_path = self.get_dymola_interface_path(dymola_path)
         self.logger.info("Using dymola interface: %s", self.dymola_interface_path)
 
         self.packages = []
         if packages is not None:
             for package in packages:
-                if isinstance(package, pathlib.Path):
+                if isinstance(package, Path):
                     self.packages.append(str(package))
                 elif isinstance(package, str):
                     self.packages.append(package)
                 else:
                     raise TypeError(f"Given package is of type {type(package)}"
                                     f" but should be any valid path.")
 
@@ -220,31 +250,41 @@
             raise TypeError(f"n_restart has to be type int but "
                             f"is of type {type(self.n_restart)}")
 
         self._dummy_dymola_instance = None  # Ensure self._close_dummy gets the attribute.
         if self.n_restart > 0:
             self.logger.info("Open blank placeholder Dymola instance to ensure"
                              " a licence during Dymola restarts")
-            self._dummy_dymola_instance = self._open_dymola_interface()
+            # Use standard port allocation, should always work
+            self._dummy_dymola_instance = self._open_dymola_interface(port=-1)
             atexit.register(self._close_dummy)
 
         # List storing structural parameters for later modifying the simulation-name.
         # Parameter for raising a warning if to many dymola-instances are running
         self._critical_number_instances = 10 + self.n_cpu
         # Register the function now in case of an error.
         if not self.debug:
             atexit.register(self.close)
         if self.use_mp:
-            self.pool.map(self._setup_dymola_interface, [True for _ in range(self.n_cpu)])
+            ports = _get_n_available_ports(n_ports=self.n_cpu)
+            self.pool.map(
+                self._setup_dymola_interface,
+                [dict(use_mp=True, port=port, time_delay=i * _time_delay_between_starts)
+                 for i, port in enumerate(ports)]
+            )
         # For translation etc. always setup a default dymola instance
-        self.dymola = self._setup_dymola_interface(use_mp=False)
+        self.dymola = self._setup_dymola_interface(dict(use_mp=False))
+        if not self.license_is_available():
+            warnings.warn("You have no licence to use Dymola. "
+                          "Hence you can only simulate models with 8 or less equations.")
 
         self.fully_initialized = True
         # Trigger on init.
-        self._update_model()
+        if model_name is not None:
+            self._update_model()
         # Set result_names to output variables.
         self.result_names = list(self.outputs.keys())
 
         # Check if some kwargs are still present. If so, inform the user about
         # false usage of kwargs:
         if kwargs:
             self.logger.error(
@@ -317,29 +357,39 @@
                 parameters = [parameters] * len(model_names)
             if parameters is None:
                 parameters = [{}] * len(model_names)
         return super().simulate(parameters=parameters, return_option=return_option, **kwargs)
 
     def _single_simulation(self, kwargs):
         # Unpack kwargs
-        show_eventlog = kwargs.get("show_eventlog", False)
-        squeeze = kwargs.get("squeeze", True)
-        result_file_name = kwargs.get("result_file_name", 'resultFile')
-        parameters = kwargs.get("parameters")
-        return_option = kwargs.get("return_option")
-        model_names = kwargs.get("model_names")
-        inputs = kwargs.get("inputs", None)
-        fail_on_error = kwargs.get("fail_on_error", True)
-        structural_parameters = kwargs.get("structural_parameters", [])
+        show_eventlog = kwargs.pop("show_eventlog", False)
+        squeeze = kwargs.pop("squeeze", True)
+        result_file_name = kwargs.pop("result_file_name", 'resultFile')
+        parameters = kwargs.pop("parameters")
+        return_option = kwargs.pop("return_option")
+        model_names = kwargs.pop("model_names", None)
+        inputs = kwargs.pop("inputs", None)
+        fail_on_error = kwargs.pop("fail_on_error", True)
+        structural_parameters = kwargs.pop("structural_parameters", [])
+        table_name = kwargs.pop("table_name", None)
+        file_name = kwargs.pop("file_name", None)
+        savepath = kwargs.pop("savepath", None)
+        if kwargs:
+            self.logger.error(
+                "You passed the following kwargs which "
+                "are not part of the supported kwargs and "
+                "have thus no effect: %s.", " ,".join(list(kwargs.keys())))
 
         # Handle multiprocessing
         if self.use_mp:
             idx_worker = self.worker_idx
             if self.dymola is None:
-                self._setup_dymola_interface(use_mp=True)
+                # This should not affect #119, as this rarely happens. Thus, the
+                # method used in the DymolaInterface should work.
+                self._setup_dymola_interface(dict(use_mp=True))
 
         # Handle eventlog
         if show_eventlog:
             self.dymola.experimentSetupOutput(events=True)
             self.dymola.ExecuteCommand("Advanced.Debug.LogEvents = true")
             self.dymola.ExecuteCommand("Advanced.Debug.LogEventsInitialization = true")
 
@@ -359,14 +409,21 @@
                     "If you do expect them, please raise an issue to add the "
                     "option when using the model_names keyword.")
                 self.logger.info(
                     "Difference: %s",
                     " ,".join(list(set(_res_names).difference(self.result_names)))
                 )
 
+        if self.model_name is None:
+            raise ValueError(
+                "You neither passed a model_name when "
+                "starting DymolaAPI, nor when calling simulate. "
+                "Can't simulate no model."
+            )
+
         # Handle parameters:
         if parameters is None:
             parameters = {}
             unsupported_parameters = False
         else:
             unsupported_parameters = self.check_unsupported_variables(
                 variables=list(parameters.keys()),
@@ -412,18 +469,15 @@
             raise TypeError("Dymola only accepts float values. "
                             "Could bot automatically convert the given "
                             "parameter values to float.") from err
 
         # Handle inputs
         if inputs is not None:
             # Unpack additional kwargs
-            try:
-                table_name = kwargs["table_name"]
-                file_name = kwargs["file_name"]
-            except KeyError as err:
+            if table_name is None or file_name is None:
                 raise KeyError("For inputs to be used by DymolaAPI.simulate, you "
                                "have to specify the 'table_name' and the 'file_name' "
                                "as keyword arguments of the function. These must match"
                                "the values 'tableName' and 'fileName' in the CombiTimeTable"
                                " model in your modelica code.") from err
             # Generate the input in the correct format
             offset = self.sim_setup.start_time - inputs.index[0]
@@ -502,15 +556,15 @@
 
         if not res[0]:
             self.logger.error("Simulation failed!")
             self.logger.error("The last error log from Dymola:")
             log = self.dymola.getLastErrorLog()
             # Only print first part as output is sometimes to verbose.
             self.logger.error(log[:10000])
-            dslog_path = os.path.join(self.cd, 'dslog.txt')
+            dslog_path = self.working_directory.joinpath('dslog.txt')
             try:
                 with open(dslog_path, "r") as dslog_file:
                     dslog_content = dslog_file.read()
                     self.logger.error(dslog_content)
             except Exception:
                 dslog_content = "Not retreivable. Open it yourself."
             msg = f"Simulation failed: Reason according " \
@@ -519,32 +573,34 @@
                 raise Exception(msg)
             # Don't raise and return None
             self.logger.error(msg)
             return None
 
         if return_option == "savepath":
             _save_name_dsres = f"{result_file_name}.mat"
-            savepath = kwargs.pop("savepath", None)
-            # Get the cd of the current dymola instance
+            # Get the working_directory of the current dymola instance
             self.dymola.cd()
             # Get the value and convert it to a 100 % fitting str-path
-            dymola_cd = str(pathlib.Path(self.dymola.getLastErrorLog().replace("\n", "")))
-            if savepath is None or str(savepath) == dymola_cd:
-                return os.path.join(dymola_cd, _save_name_dsres)
+            dymola_working_directory = str(Path(self.dymola.getLastErrorLog().replace("\n", "")))
+            if savepath is None or str(savepath) == dymola_working_directory:
+                return os.path.join(dymola_working_directory, _save_name_dsres)
             os.makedirs(savepath, exist_ok=True)
-            for filename in [_save_name_dsres, "dslog.txt", "dsfinal.txt"]:
+            for filename in [_save_name_dsres]:
+                # Copying dslogs and dsfinals can lead to errors,
+                # as the names are not unique
+                # for filename in [_save_name_dsres, "dslog.txt", "dsfinal.txt"]:
                 # Delete existing files
                 try:
                     os.remove(os.path.join(savepath, filename))
                 except OSError:
                     pass
                 # Move files
-                shutil.copy(os.path.join(dymola_cd, filename),
+                shutil.copy(os.path.join(dymola_working_directory, filename),
                             os.path.join(savepath, filename))
-                os.remove(os.path.join(dymola_cd, filename))
+                os.remove(os.path.join(dymola_working_directory, filename))
             return os.path.join(savepath, _save_name_dsres)
 
         data = res[1]  # Get data
         if return_option == "last_point":
             results = []
             for ini_val_set in data:
                 results.append({result_name: ini_val_set[idx][-1] for idx, result_name
@@ -642,27 +698,34 @@
             raise ValueError("Given function is not yet supported for multiprocessing")
         res = self.dymola.importInitial(dsName=filepath)
         if res:
             self.logger.info("Successfully loaded dsfinal.txt")
         else:
             raise Exception("Could not load dsfinal into Dymola.")
 
-    @SimulationAPI.cd.setter
-    def cd(self, cd):
+    @SimulationAPI.working_directory.setter
+    def working_directory(self, working_directory: Union[Path, str]):
         """Set the working directory to the given path"""
-        self._cd = cd
+        if isinstance(working_directory, str):
+            working_directory = Path(working_directory)
+        self._working_directory = working_directory
         if self.dymola is None:  # Not yet started
             return
-        # Also set the cd in the dymola api
+        # Also set the working_directory in the dymola api
         self.set_dymola_cd(dymola=self.dymola,
-                           cd=cd)
+                           cd=working_directory)
         if self.use_mp:
-            self.logger.warning("Won't set the cd for all workers, "
+            self.logger.warning("Won't set the working_directory for all workers, "
                                 "not yet implemented.")
 
+    @SimulationAPI.cd.setter
+    def cd(self, cd):
+        warnings.warn("cd was renamed to working_directory in all classes. Use working_directory instead.", category=DeprecationWarning)
+        self.working_directory = cd
+
     def set_dymola_cd(self, dymola, cd):
         """
         Set the cd of the Dymola Instance.
         Before calling the Function, create the path and
         convert to a modelica-normpath.
         """
         os.makedirs(cd, exist_ok=True)
@@ -736,17 +799,21 @@
             elif row["5"] == "5":
                 self.inputs[idx] = _var_ebcpy
             elif row["5"] == "4":
                 self.outputs[idx] = _var_ebcpy
             else:
                 self.states[idx] = _var_ebcpy
 
-    def _setup_dymola_interface(self, use_mp):
+    def _setup_dymola_interface(self, kwargs: dict):
         """Load all packages and change the current working directory"""
-        dymola = self._open_dymola_interface()
+        use_mp = kwargs["use_mp"]
+        port = kwargs.get("port", -1)
+        time_delay = kwargs.get("time_delay", 0)
+        time.sleep(time_delay)
+        dymola = self._open_dymola_interface(port=port)
         self._check_dymola_instances()
         if use_mp:
             cd = os.path.join(self.cd, f"worker_{self.worker_idx}")
         else:
             cd = self.cd
         # Execute the mos-script if given:
         if self.mos_script_pre is not None:
@@ -766,31 +833,36 @@
         self.logger.info("Loaded modules")
         if self.equidistant_output:
             # Change the Simulation Output, to ensure all
             # simulation results have the same array shape.
             # Events can also cause errors in the shape.
             dymola.experimentSetupOutput(equidistant=True,
                                          events=False)
-        if not dymola.RequestOption("Standard"):
-            warnings.warn("You have no licence to use Dymola. "
-                          "Hence you can only simulate models with 8 or less equations.")
         if use_mp:
             DymolaAPI.dymola = dymola
             return None
         return dymola
 
-    def _open_dymola_interface(self):
+    def license_is_available(self, option: str = "Standard"):
+        """Check if license is available"""
+        if self.dymola is None:
+            warnings.warn("You want to check the license before starting dymola, this is not supported.")
+            return False
+        return self.dymola.RequestOption(option)
+
+    def _open_dymola_interface(self, port):
         """Open an instance of dymola and return the API-Object"""
         if self.dymola_interface_path not in sys.path:
             sys.path.insert(0, self.dymola_interface_path)
         try:
             from dymola.dymola_interface import DymolaInterface
             from dymola.dymola_exception import DymolaConnectionException
             return DymolaInterface(showwindow=self.show_window,
-                                   dymolapath=self.dymola_exe_path)
+                                   dymolapath=self.dymola_exe_path,
+                                   port=port)
         except ImportError as error:
             raise ImportError("Given dymola-interface could not be "
                               "loaded:\n %s" % self.dymola_interface_path) from error
         except DymolaConnectionException as error:
             raise ConnectionError(error) from error
 
     def to_dict(self):
@@ -820,33 +892,33 @@
         packages = self.dymola.ExecuteCommand(
             'ModelManagement.Structure.AST.Misc.ClassesInPackage("")'
         )
         if packages is None:
             self.logger.error("Could not load packages from Dymola, using self.packages")
             packages = []
             for pack in self.packages:
-                pack = pathlib.Path(pack)
+                pack = Path(pack)
                 if pack.name == "package.mo":
                     packages.append(pack.parent.name)
         valid_packages = []
         for pack in packages:
             current_package = f"modelica://{pack}/package.order"
             pack_path = self.dymola.ExecuteCommand(
                 f'Modelica.Utilities.Files.loadResource("{current_package}")'
             )
             if not isinstance(pack_path, str):
                 self.logger.error("Could not load model resource for package %s", pack)
             if os.path.isfile(pack_path):
-                valid_packages.append(pathlib.Path(pack_path).parent)
+                valid_packages.append(Path(pack_path).parent)
         return valid_packages
 
     def save_for_reproduction(
             self,
             title: str,
-            path: pathlib.Path = None,
+            path: Path = None,
             files: list = None,
             save_total_model: bool = True,
             export_fmu: bool = True,
             **kwargs
     ):
         """
         Additionally to the basic reproduction, add info
@@ -907,19 +979,37 @@
         files.append(ReproductionFile(
             filename="Dymola/Modelica_packages.txt",
             content="\n".join(package_infos)
         ))
         # Total model
         if save_total_model:
             _total_model_name = f"Dymola/{self.model_name.replace('.', '_')}_total.mo"
-            _total_model = pathlib.Path(self.cd).joinpath(_total_model_name)
+            _total_model = Path(self.cd).joinpath(_total_model_name)
             os.makedirs(_total_model.parent, exist_ok=True)  # Create to ensure model can be saved.
+            if "(" in self.model_name:
+                # Create temporary model:
+                temp_model_file = Path(self.cd).joinpath(f"temp_total_model_{uuid.uuid4()}.mo")
+                temp_mode_name = f"{self.model_name.split('(')[0].split('.')[-1]}WithModifier"
+                with open(temp_model_file, "w") as file:
+                    file.write(f"model {temp_mode_name}\n  extends {self.model_name};\nend {temp_mode_name};")
+                res = self.dymola.openModel(str(temp_model_file), changeDirectory=False)
+                if not res:
+                    self.logger.error(
+                        "Could not create separate model for model with modifiers: %s",
+                        self.model_name
+                    )
+                    model_name_to_save = self.model_name
+                else:
+                    model_name_to_save = temp_mode_name
+                os.remove(temp_model_file)
+            else:
+                model_name_to_save = self.model_name
             res = self.dymola.saveTotalModel(
                 fileName=str(_total_model),
-                modelName=self.model_name
+                modelName=model_name_to_save
             )
             if res:
                 files.append(ReproductionFile(
                     filename=_total_model_name,
                     content=_total_model.read_text()
                 ))
                 os.remove(_total_model)
@@ -956,30 +1046,30 @@
         )
         if not res:
             msg = "Could not export fmu: %s" % self.dymola.getLastErrorLog()
             self.logger.error(msg)
             if fail_on_error:
                 raise Exception(msg)
         else:
-            path = pathlib.Path(self.cd).joinpath(res + ".fmu")
+            path = Path(self.cd).joinpath(res + ".fmu")
             return path
 
     @staticmethod
     def _make_modelica_normpath(path):
         """
         Convert given path to a path readable in dymola.
         If the base path does not exist, create it.
 
         :param str,os.path.normpath path:
             Either a file or a folder path. The base to this
             path is created in non existent.
         :return: str
             Path readable in dymola
         """
-        if isinstance(path, pathlib.Path):
+        if isinstance(path, Path):
             path = str(path)
 
         path = path.replace("\\", "/")
         # Search for e.g. "D:testzone" and replace it with D:/testzone
         loc = path.find(":")
         if path[loc + 1] != "/" and loc != -1:
             path = path.replace(":", ":/")
@@ -1002,15 +1092,15 @@
         if not os.path.isfile(egg_file):
             raise FileNotFoundError(f"The given dymola installation directory "
                                     f"'{dymola_install_dir}' has no "
                                     f"dymola-interface egg-file.")
         return egg_file
 
     @staticmethod
-    def get_dymola_path(dymola_install_dir, dymola_name=None):
+    def get_dymola_exe_path(dymola_install_dir, dymola_name=None):
         """
         Function to get the path of the dymola exe-file
         on the current used machine.
 
         :param str dymola_install_dir:
             The dymola installation folder. Example:
             "C://Program Files//Dymola 2020"
@@ -1158,11 +1248,80 @@
 
     def _check_restart(self):
         """Restart Dymola every n_restart iterations in order to free memory"""
 
         if self.sim_counter == self.n_restart:
             self.logger.info("Closing and restarting Dymola to free memory")
             self.close()
-            self._dummy_dymola_instance = self._setup_dymola_interface(use_mp=False)
+            self._dummy_dymola_instance = self._setup_dymola_interface(dict(use_mp=False))
             self.sim_counter = 1
         else:
             self.sim_counter += 1
+
+
+def _get_dymola_path_of_version(dymola_installations: list, dymola_version: str):
+    """
+    Helper function to get the path associated to the dymola_version
+    from the list of all installations
+    """
+    for dymola_path in dymola_installations:
+        if dymola_path.endswith(dymola_version):
+            return dymola_path
+    # If still here, version was not found
+    raise ValueError(
+        f"Given dymola_version '{dymola_version}' not found in "
+        f"the list of dymola installations {dymola_installations}"
+    )
+
+
+def _get_n_available_ports(n_ports: int, start_range: int = 44000, end_range: int = 44400):
+    """
+    Get a specified number of available network ports within a given range.
+
+    This function uses socket connections to check the availability of ports within the specified range.
+    If the required number of open ports is found, it returns a list of those ports. If not, it raises
+    a ConnectionError with a descriptive message indicating the failure to find the necessary ports.
+
+    Parameters:
+    - n_ports (int): The number of open ports to find.
+    - start_range (int, optional):
+        The starting port of the range to check (inclusive).
+        Default is 44000.
+    - end_range (int, optional):
+        The ending port of the range to check (exclusive).
+        Default is 44400.
+
+    Returns:
+    - list of int:
+        A list containing the available ports.
+        The length of the list is equal to 'n_ports'.
+
+    Raises:
+    - ConnectionError:
+        If the required number of open ports cannot
+        be found within the specified range.
+
+    Example:
+
+    ```
+    try:
+        open_ports = _get_n_available_ports(3, start_range=50000, end_range=50500)
+        print(f"Found open ports: {open_ports}")
+    except ConnectionError as e:
+        print(f"Error: {e}")
+    ```
+    """
+    ports = []
+    for port in range(start_range, end_range):
+        try:
+            with closing(socket.socket(socket.AF_INET, socket.SOCK_STREAM)) as sock:
+                sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+                sock.bind(("127.0.0.1", port))
+            ports.append(port)
+        except OSError:
+            pass
+        if len(ports) == n_ports:
+            return ports
+    raise ConnectionError(
+        f"Could not find {n_ports} open ports in range {start_range}-{end_range}."
+        f"Can't open {n_ports} Dymola instances"
+    )
```

### Comparing `ebcpy-0.3.8/ebcpy/simulationapi/fmu.py` & `ebcpy-0.4.1/ebcpy/simulationapi/fmu.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,31 +70,31 @@
     _sim_setup_class: SimulationSetupClass = FMU_Setup
     _type_map = {
         float: np.double,
         bool: np.bool_,
         int: np.int_
     }
 
-    def __init__(self, cd, model_name, **kwargs):
+    def __init__(self, working_directory, model_name, **kwargs):
         """Instantiate class parameters"""
         # Init instance attributes
         self._model_description = None
         self._fmi_type = None
         self._unzip_dir = None
         self._fmu_instance = None
         self.log_fmu = kwargs.get("log_fmu", True)
         self._single_unzip_dir: str = None
 
         if isinstance(model_name, pathlib.Path):
             model_name = str(model_name)
         if not model_name.lower().endswith(".fmu"):
             raise ValueError(f"{model_name} is not a valid fmu file!")
-        if cd is None:
-            cd = os.path.dirname(model_name)
-        super().__init__(cd, model_name, **kwargs)
+        if working_directory is None:
+            working_directory = os.path.dirname(model_name)
+        super().__init__(working_directory, model_name, **kwargs)
         # Register exit option
         atexit.register(self.close)
 
     def _update_model(self):
         # Setup the fmu instance
         self.setup_fmu_instance()
 
@@ -182,16 +182,25 @@
 
         The single argument kwarg is to make this
         function accessible by multiprocessing pool.map.
         """
         # Unpack kwargs:
         parameters = kwargs.pop("parameters", None)
         return_option = kwargs.pop("return_option", "time_series")
-        inputs = kwargs.get("inputs", None)
-        fail_on_error = kwargs.get("fail_on_error", True)
+        inputs = kwargs.pop("inputs", None)
+        fail_on_error = kwargs.pop("fail_on_error", True)
+        result_file_name = kwargs.pop("result_file_name", "resultFile")
+        result_file_suffix = kwargs.pop("result_file_suffix", "csv")
+        parquet_engine = kwargs.pop('parquet_engine', 'pyarrow')
+        savepath = kwargs.pop("savepath", None)
+        if kwargs:
+            self.logger.error(
+                "You passed the following kwargs which "
+                "are not part of the supported kwargs and "
+                "have thus no effect: %s.", " ,".join(list(kwargs.keys())))
 
         if self.use_mp:
             if self._fmu_instance is None:
                 self._setup_single_fmu_instance(use_mp=True)
 
         if inputs is not None:
             if not isinstance(inputs, (TimeSeriesData, pd.DataFrame)):
@@ -251,21 +260,16 @@
 
         # Reshape result:
         df = pd.DataFrame(res).set_index("time")
         df.index = np.round(df.index.astype("float64"),
                             str(self.sim_setup.output_interval)[::-1].find('.'))
 
         if return_option == "savepath":
-            result_file_name = kwargs.get("result_file_name", "resultFile")
-            result_file_suffix = kwargs.get("result_file_suffix", "csv")
-            parquet_engine = kwargs.get('parquet_engine', 'pyarrow')
-            savepath = kwargs.get("savepath", None)
-
             if savepath is None:
-                savepath = self.cd
+                savepath = self.working_directory
 
             os.makedirs(savepath, exist_ok=True)
             filepath = os.path.join(savepath, f"{result_file_name}.{result_file_suffix}")
             TimeSeriesData(df).droplevel(1, axis=1).save(
                 filepath=filepath,
                 key="simulation",
                 engine=parquet_engine
@@ -281,15 +285,15 @@
     def setup_fmu_instance(self):
         """
         Manually set up and extract the data to
         avoid this step in the simulate function.
         """
         self.logger.info("Extracting fmu and reading fmu model description")
         # First load model description and extract variables
-        self._single_unzip_dir = os.path.join(self.cd,
+        self._single_unzip_dir = os.path.join(self.working_directory,
                                               os.path.basename(self.model_name)[:-4] + "_extracted")
         os.makedirs(self._single_unzip_dir, exist_ok=True)
         self._single_unzip_dir = fmpy.extract(self.model_name,
                                               unzipdir=self._single_unzip_dir)
         self._model_description = read_model_description(self._single_unzip_dir,
                                                          validate=True)
```

### Comparing `ebcpy-0.3.8/ebcpy/utils/conversion.py` & `ebcpy-0.4.1/ebcpy/utils/conversion.py`

 * *Files identical despite different names*

### Comparing `ebcpy-0.3.8/ebcpy/utils/reproduction.py` & `ebcpy-0.4.1/ebcpy/utils/reproduction.py`

 * *Files identical despite different names*

### Comparing `ebcpy-0.3.8/ebcpy/utils/statistics_analyzer.py` & `ebcpy-0.4.1/ebcpy/utils/statistics_analyzer.py`

 * *Files identical despite different names*

### Comparing `ebcpy-0.3.8/ebcpy.egg-info/PKG-INFO` & `ebcpy-0.4.1/ebcpy.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,51 @@
 Metadata-Version: 2.1
 Name: ebcpy
-Version: 0.3.8
+Version: 0.4.1
 Summary: Python Library used for different python modules for the analysis and optimization of energy systems, buildings and indoor climate 
 Home-page: https://github.com/RWTH-EBC/ebcpy
+Download-URL: https://github.com/RWTH-EBC/ebcpy/archive/refs/tags/0.4.1.tar.gz
 Author: RWTH Aachen University, E.ON Energy Research Center, Institute of Energy Efficient Buildings and Indoor Climate
 Author-email: fabian.wuellhorst@eonerc.rwth-aachen.de
 License: BSD 3-Clause
-Download-URL: https://github.com/RWTH-EBC/ebcpy/archive/refs/tags/0.3.8.tar.gz
 Keywords: simulation,building,energy,time-series-data,comfort,black-box optimization
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
-Provides-Extra: full
 License-File: LICENSE
+Requires-Dist: numpy>=1.19.5
+Requires-Dist: matplotlib>=3.3.4
+Requires-Dist: scipy>=1.5.4
+Requires-Dist: pandas>=1.1.5
+Requires-Dist: scikit-learn>=0.24.2
+Requires-Dist: fmpy<0.3.17,>=0.2.27
+Requires-Dist: pydantic>=2.0
+Requires-Dist: h5py>=3.1.0
+Requires-Dist: tables>=3.6.1
+Provides-Extra: full
+Requires-Dist: openpyxl>=3.0.5; extra == "full"
+Requires-Dist: xlrd>=2.0.1; extra == "full"
+Requires-Dist: pymoo==0.5.0; extra == "full"
+Requires-Dist: GitPython>=3.1.27; extra == "full"
+Requires-Dist: pyarrow>=11.0.0; extra == "full"
+Requires-Dist: fastparquet>=2023.1.0; extra == "full"
 
 ![E.ON EBC RWTH Aachen University](./docs/EBC_Logo.png)
 
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.03861/status.svg)](https://doi.org/10.21105/joss.03861)
-[![pylint](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/pylint/pylint.svg )](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/pylint/pylint.html)
-[![documentation](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/docs/doc.svg)](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/docs/index.html)
-[![coverage](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/coverage/badge.svg)](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/coverage)
+[![pylint](https://rwth-ebc.github.io/ebcpy/master/pylint/pylint.svg )](https://rwth-ebc.github.io/ebcpy/master/pylint/pylint.html)
+[![documentation](https://rwth-ebc.github.io/ebcpy/master/docs/doc.svg)](https://rwth-ebc.github.io/ebcpy/master/docs/index.html)
+[![coverage](https://rwth-ebc.github.io/ebcpy/master/coverage/badge.svg)](https://rwth-ebc.github.io/ebcpy/master/coverage)
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
-[![build](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/build/build.svg)](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/build/build.svg)
+[![build](https://rwth-ebc.github.io/ebcpy/master/build/build.svg)](https://rwth-ebc.github.io/ebcpy/master/build/build.svg)
 
 
 # ebcpy
 
 This **PY**thon package provides generic functions and classes commonly
 used for the analysis and optimization of **e**nergy systems, **b**uildings and indoor **c**limate (**EBC**).
 
@@ -39,15 +53,15 @@
 
 * `TimeSeriesData`
 * `SimulationAPI`'s
 * Optimization wrapper
 * Pre-/Postprocessing
 * Modelica utilities
 
-It was developed together with `AixCaliBuHA`, a framework for an automated calibration of dynamic building and HVAC models. During this development, we found several interfaces relevant to further reserach. We thus decoupled these interfaces into `ebcpy` and used the framework, for instance in the design optimization of heat pump systems ([link](https://www.sciencedirect.com/science/article/abs/pii/S0196890421010645?via%3Dihub)).
+It was developed together with `AixCaliBuHA`, a framework for an automated calibration of dynamic building and HVAC models. During this development, we found several interfaces relevant to further research. We thus decoupled these interfaces into `ebcpy` and used the framework, for instance in the design optimization of heat pump systems ([link](https://www.sciencedirect.com/science/article/abs/pii/S0196890421010645?via%3Dihub)).
 
 # Installation
 
 To install, simply run
 ```
 pip install ebcpy
 ```
@@ -146,13 +160,11 @@
 # From float to datetime
 tsd.to_datetime_index()
 # To clean your data and create a common frequency:
 tsd.clean_and_space_equally(desired_freq="1s")
 ```
 
 # Documentation
-Visit our official [Documentation](https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/ebcpy/master/docs/index.html).
+Visit our official [Documentation](https://rwth-ebc.github.io/ebcpy/master/docs/index.html).
 
 # Problems?
 Please [raise an issue here](https://github.com/RWTH-EBC/ebcpy/issues/new).
-
-
```

### Comparing `ebcpy-0.3.8/setup.py` & `ebcpy-0.4.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 INSTALL_REQUIRES = [
     'numpy>=1.19.5',
     'matplotlib>=3.3.4',
     'scipy>=1.5.4',
     'pandas>=1.1.5',
     'scikit-learn>=0.24.2',
-    'fmpy>=0.2.27',
+    'fmpy>=0.2.27,<0.3.17',
     'pydantic>=2.0',
     'h5py>=3.1.0',
     'tables>=3.6.1'
 ]
     
 if sys.version_info.minor >= 9 and sys.version_info.major == 3:
     EXTRAS_REQUIRE['full'].append('fastparquet>=2023.1.0')
```

