# Comparing `tmp/alphastats-0.6.6.tar.gz` & `tmp/alphastats-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphastats-0.6.6.tar", last modified: Fri May 24 13:15:46 2024, max compression
+gzip compressed data, was "alphastats-0.6.7.tar", last modified: Mon Jun  3 13:59:28 2024, max compression
```

## Comparing `alphastats-0.6.6.tar` & `alphastats-0.6.7.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:15:46.665721 alphastats-0.6.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-05-24 13:15:20.000000 alphastats-0.6.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-24 13:15:20.000000 alphastats-0.6.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-05-24 13:15:46.665721 alphastats-0.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-05-24 13:15:20.000000 alphastats-0.6.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:15:46.645721 alphastats-0.6.6/alphastats/
--rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/DataSet.py
--rw-r--r--   0 runner    (1001) docker     (127)    19551 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/DataSet_Pathway.py
--rw-r--r--   0 runner    (1001) docker     (127)    13960 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/DataSet_Plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    13426 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/DataSet_Preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/DataSet_Statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:15:46.645721 alphastats-0.6.6/alphastats/data/
--rw-r--r--   0 runner    (1001) docker     (127)    70534 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/data/contaminations.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:15:46.649721 alphastats-0.6.6/alphastats/gui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:15:46.649721 alphastats-0.6.6/alphastats/gui/.streamlit/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/gui/.streamlit/config.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/gui/AlphaPeptStats.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31042 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/gui/alphapeptstats_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    30529 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/gui/alphastats_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    20433 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/gui/alphastats_logo_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/gui/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:15:46.649721 alphastats-0.6.6/alphastats/gui/pages/
--rw-r--r--   0 runner    (1001) docker     (127)    14532 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/gui/pages/02_Import Data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/gui/pages/03_Data Overview.py
--rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/gui/pages/03_Preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/gui/pages/04_Analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/gui/pages/06_Results.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/gui/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:15:46.649721 alphastats-0.6.6/alphastats/gui/sample_data/
--rw-r--r--   0 runner    (1001) docker     (127)    26661 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/gui/sample_data/metadata.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)  9509624 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/gui/sample_data/proteinGroups.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:15:46.661721 alphastats-0.6.6/alphastats/gui/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    10474 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/gui/utils/analysis_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/gui/utils/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/gui/utils/software_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/gui/utils/ui_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/load_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:15:46.661721 alphastats-0.6.6/alphastats/loader/
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/loader/AlphaPeptLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/loader/BaseLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/loader/DIANNLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/loader/FragPipeLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/loader/GenericLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/loader/MaxQuantLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/loader/SpectronautLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/loader/mzTabLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:15:46.661721 alphastats-0.6.6/alphastats/multicova/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/multicova/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29725 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/multicova/multicova.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:15:46.665721 alphastats-0.6.6/alphastats/plots/
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/plots/ClusterMap.py
--rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/plots/DimensionalityReduction.py
--rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/plots/IntensityPlot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/plots/PlotUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/plots/SampleHistogram.py
--rw-r--r--   0 runner    (1001) docker     (127)    13581 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/plots/VolcanoPlot.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/plots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:15:46.665721 alphastats-0.6.6/alphastats/statistics/
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/statistics/Anova.py
--rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/statistics/DifferentialExpressionAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/statistics/MultiCovaAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/statistics/StatisticUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:15:46.665721 alphastats-0.6.6/alphastats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-05-24 13:15:46.000000 alphastats-0.6.6/alphastats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-24 13:15:46.000000 alphastats-0.6.6/alphastats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 13:15:46.000000 alphastats-0.6.6/alphastats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-24 13:15:46.000000 alphastats-0.6.6/alphastats.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-24 13:15:46.000000 alphastats-0.6.6/alphastats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-24 13:15:46.000000 alphastats-0.6.6/alphastats.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 13:15:46.665721 alphastats-0.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-24 13:15:20.000000 alphastats-0.6.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:15:46.665721 alphastats-0.6.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    37650 2024-05-24 13:15:20.000000 alphastats-0.6.6/tests/test_DataSet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-05-24 13:15:20.000000 alphastats-0.6.6/tests/test_DataSet_Pathway.py
--rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-05-24 13:15:20.000000 alphastats-0.6.6/tests/test_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:59:28.630004 alphastats-0.6.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-06-03 13:58:55.000000 alphastats-0.6.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-06-03 13:58:55.000000 alphastats-0.6.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-06-03 13:59:28.630004 alphastats-0.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-06-03 13:58:55.000000 alphastats-0.6.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:59:28.610004 alphastats-0.6.7/alphastats/
+-rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/DataSet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19551 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/DataSet_Pathway.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13960 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/DataSet_Plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13426 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/DataSet_Preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/DataSet_Statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:59:28.610004 alphastats-0.6.7/alphastats/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    70534 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/data/contaminations.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:59:28.610004 alphastats-0.6.7/alphastats/gui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:59:28.610004 alphastats-0.6.7/alphastats/gui/.streamlit/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/gui/.streamlit/config.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/gui/AlphaPeptStats.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31042 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/gui/alphapeptstats_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30529 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/gui/alphastats_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20433 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/gui/alphastats_logo_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/gui/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:59:28.614004 alphastats-0.6.7/alphastats/gui/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)    14608 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/gui/pages/02_Import Data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/gui/pages/03_Data Overview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/gui/pages/03_Preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/gui/pages/04_Analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/gui/pages/06_Results.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/gui/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:59:28.614004 alphastats-0.6.7/alphastats/gui/sample_data/
+-rw-r--r--   0 runner    (1001) docker     (127)    26661 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/gui/sample_data/metadata.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)  9509624 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/gui/sample_data/proteinGroups.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:59:28.626004 alphastats-0.6.7/alphastats/gui/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    10474 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/gui/utils/analysis_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/gui/utils/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/gui/utils/software_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/gui/utils/ui_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/load_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:59:28.626004 alphastats-0.6.7/alphastats/loader/
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/loader/AlphaPeptLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/loader/BaseLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/loader/DIANNLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/loader/FragPipeLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/loader/GenericLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/loader/MaxQuantLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/loader/SpectronautLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/loader/mzTabLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:59:28.626004 alphastats-0.6.7/alphastats/multicova/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/multicova/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29725 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/multicova/multicova.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:59:28.626004 alphastats-0.6.7/alphastats/plots/
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/plots/ClusterMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/plots/DimensionalityReduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/plots/IntensityPlot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/plots/PlotUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/plots/SampleHistogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13581 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/plots/VolcanoPlot.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/plots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:59:28.630004 alphastats-0.6.7/alphastats/statistics/
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/statistics/Anova.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/statistics/DifferentialExpressionAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/statistics/MultiCovaAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/statistics/StatisticUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-06-03 13:58:55.000000 alphastats-0.6.7/alphastats/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:59:28.630004 alphastats-0.6.7/alphastats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-06-03 13:59:28.000000 alphastats-0.6.7/alphastats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-06-03 13:59:28.000000 alphastats-0.6.7/alphastats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 13:59:28.000000 alphastats-0.6.7/alphastats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-06-03 13:59:28.000000 alphastats-0.6.7/alphastats.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-06-03 13:59:28.000000 alphastats-0.6.7/alphastats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-03 13:59:28.000000 alphastats-0.6.7/alphastats.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 13:59:28.630004 alphastats-0.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-06-03 13:58:55.000000 alphastats-0.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:59:28.630004 alphastats-0.6.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    37650 2024-06-03 13:58:55.000000 alphastats-0.6.7/tests/test_DataSet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-06-03 13:58:55.000000 alphastats-0.6.7/tests/test_DataSet_Pathway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-06-03 13:58:55.000000 alphastats-0.6.7/tests/test_loaders.py
```

### Comparing `alphastats-0.6.6/LICENSE.txt` & `alphastats-0.6.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/PKG-INFO` & `alphastats-0.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphastats
-Version: 0.6.6
+Version: 0.6.7
 Summary: An open-source Python package for automated and scalable statistical analysis of mass spectrometry-based proteomics
 Home-page: https://github.com/MannLabs/alphastats
 Author: Mann Labs
 Author-email: elena.krismer@gmail.com
 License: Apache
 Project-URL: Mann Labs at MPIB, https://www.biochem.mpg.de/mann
 Project-URL: GitHub, https://github.com/MannLabs/alphapeptstats
```

### Comparing `alphastats-0.6.6/README.md` & `alphastats-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/alphastats/DataSet.py` & `alphastats-0.6.7/alphastats/DataSet.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/alphastats/DataSet_Pathway.py` & `alphastats-0.6.7/alphastats/DataSet_Pathway.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/alphastats/DataSet_Plot.py` & `alphastats-0.6.7/alphastats/DataSet_Plot.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/alphastats/DataSet_Preprocess.py` & `alphastats-0.6.7/alphastats/DataSet_Preprocess.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/alphastats/DataSet_Statistics.py` & `alphastats-0.6.7/alphastats/DataSet_Statistics.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/alphastats/__init__.py` & `alphastats-0.6.7/alphastats/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __project__ = "alphastats"
-__version__ = "0.6.6"
+__version__ = "0.6.7"
 __license__ = "Apache"
 __description__ = "An open-source Python package for Mass Spectrometry Analysis"
 __author__ = "Mann Labs"
 __author_email__ = "elena.krismer@hotmail.com"
 __github__ = "https://github.com/MannLabs/alphapeptstats"
 __keywords__ = [
     "bioinformatics",
```

### Comparing `alphastats-0.6.6/alphastats/data/contaminations.txt` & `alphastats-0.6.7/alphastats/data/contaminations.txt`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/alphastats/gui/.streamlit/config.toml` & `alphastats-0.6.7/alphastats/gui/.streamlit/config.toml`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/alphastats/gui/AlphaPeptStats.py` & `alphastats-0.6.7/alphastats/gui/AlphaPeptStats.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/alphastats/gui/alphapeptstats_logo.png` & `alphastats-0.6.7/alphastats/gui/alphapeptstats_logo.png`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/alphastats/gui/alphastats_logo.png` & `alphastats-0.6.7/alphastats/gui/alphastats_logo.png`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/alphastats/gui/alphastats_logo_2.png` & `alphastats-0.6.7/alphastats/gui/alphastats_logo_2.png`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/alphastats/gui/gui.py` & `alphastats-0.6.7/alphastats/gui/gui.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/alphastats/gui/pages/02_Import Data.py` & `alphastats-0.6.7/alphastats/gui/pages/02_Import Data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-import io
-import os
-
 import streamlit as st
+import os
+import io
 
 try:
     from alphastats.DataSet import DataSet
     from alphastats.gui.utils.analysis_helper import (
         get_sample_names_from_software_file,
         read_uploaded_file_into_df,
     )
@@ -163,17 +162,15 @@
     )
 
     with st.form("sample_column"):
         st.selectbox("Sample Column", options=valid_sample_columns, key="sample_column")
         submitted = st.form_submit_button("Create DataSet")
 
     if submitted:
-        if len(df[st.session_state.sample_column].to_list()) != len(
-            df[st.session_state.sample_column].unique()
-        ):
+        if len(df[st.session_state.sample_column].to_list()) != len(df[st.session_state.sample_column].unique()):
             st.error("Sample names have to be unique.")
             st.stop()
         return True
 
 
 def upload_softwarefile(software):
     softwarefile = st.file_uploader(
@@ -416,14 +413,16 @@
     Niu L, Geyer PE, Wewer Albrechtsen NJ, Gluud LL, Santos A, Doll S, Treit PV, Holst JJ, Knop FK, Vilsbøll T, Junker A, 
     Sachs S, Stemmer K, Müller TD, Tschöp MH, Hofmann SM, Mann M, Plasma proteome profiling discovers novel proteins 
     associated with non-alcoholic fatty liver disease. Mol Syst Biol, 15(3):e8793(2019)
     """
     )
 
     load_sample_data()
+    if "distribution_plot" not in st.session_state:
+        save_plot_sampledistribution_rawdata()
 
 
 st.markdown("### To start a new session:")
 
 if st.button("New Session: Import new dataset"):
     empty_session_state()
     st.rerun()
```

### Comparing `alphastats-0.6.6/alphastats/gui/pages/03_Data Overview.py` & `alphastats-0.6.7/alphastats/gui/pages/03_Data Overview.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/alphastats/gui/pages/03_Preprocessing.py` & `alphastats-0.6.7/alphastats/gui/pages/03_Preprocessing.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,15 +32,18 @@
             remove_samples = st.multiselect(
                 "Remove samples from analysis", 
                 options=st.session_state.dataset.metadata[st.session_state.dataset.sample].to_list()
             )
 
             data_completeness = st.number_input(
                 f"Data completeness across samples cut-off \n(0.7 -> protein has to be detected in at least 70% of the samples)",
-                value=0, min_value=0, max_value=1
+                value=0.0,
+                min_value=0.0,
+                max_value=1.0,
+                step=0.1,
             )
 
             log2_transform = st.selectbox(
                 "Log2-transform dataset", options=[True, False],
             )
 
             normalization = st.selectbox(
```

### Comparing `alphastats-0.6.6/alphastats/gui/pages/04_Analysis.py` & `alphastats-0.6.7/alphastats/gui/pages/04_Analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,15 @@
 
 if "dataset" in st.session_state:
 
     c1, c2 = st.columns((1, 2))
 
     plot_to_display = False
     df_to_display = False
+    method_plot = None
 
     with c1:
 
         method = select_analysis()
 
         if method in st.session_state.plotting_options.keys():
 
@@ -192,15 +193,15 @@
 
         with col2:
             download_figure(method_plot, format="svg")
 
         with col3:
             download_preprocessing_info(method_plot)
 
-    elif analysis_result is not None and df_to_display:
+    elif analysis_result is not None and df_to_display and method_plot:
         col1, col2, col3 = st.columns([1, 1, 1])
 
         with col1:
             download_figure(method_plot, format="pdf", plotting_library="seaborn")
 
         with col2:
             download_figure(method_plot, format="svg", plotting_library="seaborn")
```

### Comparing `alphastats-0.6.6/alphastats/gui/pages/06_Results.py` & `alphastats-0.6.7/alphastats/gui/pages/06_Results.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,33 +8,33 @@
     from utils.ui_helper import sidebar_info
 
 
 def display_plotly_figure(plot):
     st.plotly_chart(plot)
 
 
-def save_plotly(plot, format):
+def save_plotly(plot, name, format):
     # Create an in-memory buffer
     buffer = io.BytesIO()
     # Save the figure as a pdf to the buffer
-    plot[1].write_image(file=buffer, format=format)
+    plot.write_image(file=buffer, format=format)
     st.download_button(
-        label="Download as " + format, data=buffer, file_name=plot[0] + "." + format
+        label="Download as " + format, data=buffer, file_name=name + "." + format
     )
 
 
 @st.cache_data
 def convert_df(df, user_session_id=st.session_state.user_session_id):
     return df.to_csv().encode("utf-8")
 
 
-def download_preprocessing_info(plot, count):
-    preprocesing_dict = plot[1].preprocessing
+def download_preprocessing_info(plot, name, count):
+    preprocesing_dict = plot.preprocessing
     df = pd.DataFrame(preprocesing_dict.items())
-    filename = "plot" + plot[0] + "preprocessing_info.csv"
+    filename = "plot" + name + "preprocessing_info.csv"
     csv = convert_df(df)
     st.download_button(
         "Download DataSet Info as .csv",
         csv,
         filename,
         "text/csv",
         key="preprocessing" + count,
@@ -46,25 +46,28 @@
 sidebar_info()
 
 if "plot_list" in st.session_state:
     for count, plot in enumerate(st.session_state.plot_list):
         count = str(count)
 
         st.markdown("\n\n")
-        st.write(plot[0])
+        name = plot[0]
+        plot = plot[1]
+        if name == "ttest":
+            plot = plot.plot
+        st.write(name)
 
-        display_plotly_figure(plot[1])
+        display_plotly_figure(plot)
 
         col1, col2, col3 = st.columns([1, 1, 1])
 
         with col1:
-            save_plotly(plot, format="pdf")
+            save_plotly(plot, name + count, format="pdf")
 
         with col2:
-            save_plotly(plot, format="svg")
+            save_plotly(plot, name + count, format="svg")
 
         with col3:
-            download_preprocessing_info(plot, count)
-
+            download_preprocessing_info(plot, name, count)
 
 else:
     st.info("No analysis performed yet.")
```

### Comparing `alphastats-0.6.6/alphastats/gui/sample_data/metadata.xlsx` & `alphastats-0.6.7/alphastats/gui/sample_data/metadata.xlsx`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/alphastats/gui/sample_data/proteinGroups.txt` & `alphastats-0.6.7/alphastats/gui/sample_data/proteinGroups.txt`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/alphastats/gui/utils/analysis_helper.py` & `alphastats-0.6.7/alphastats/gui/utils/analysis_helper.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/alphastats/gui/utils/options.py` & `alphastats-0.6.7/alphastats/gui/utils/options.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/alphastats/gui/utils/software_options.py` & `alphastats-0.6.7/alphastats/gui/utils/software_options.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/alphastats/gui/utils/ui_helper.py` & `alphastats-0.6.7/alphastats/gui/utils/ui_helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         text-align: left;    
         bottom: 14px; 
         width: 100%;
     }  
     </style>
     </head>
     <body>
-        <div class="footer">Mann Group, 2022</div>
+        <div class="footer">Mann Group, 2024</div>
     </body>""",
         unsafe_allow_html=True,
     )
 
 
 def display_sidebar_html_table():
```

### Comparing `alphastats-0.6.6/alphastats/load_data.py` & `alphastats-0.6.7/alphastats/load_data.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/alphastats/loader/AlphaPeptLoader.py` & `alphastats-0.6.7/alphastats/loader/AlphaPeptLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/alphastats/loader/BaseLoader.py` & `alphastats-0.6.7/alphastats/loader/BaseLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/alphastats/loader/DIANNLoader.py` & `alphastats-0.6.7/alphastats/loader/DIANNLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/alphastats/loader/FragPipeLoader.py` & `alphastats-0.6.7/alphastats/loader/FragPipeLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/alphastats/loader/GenericLoader.py` & `alphastats-0.6.7/alphastats/loader/GenericLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/alphastats/loader/MaxQuantLoader.py` & `alphastats-0.6.7/alphastats/loader/MaxQuantLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/alphastats/loader/SpectronautLoader.py` & `alphastats-0.6.7/alphastats/loader/SpectronautLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/alphastats/loader/mzTabLoader.py` & `alphastats-0.6.7/alphastats/loader/mzTabLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/alphastats/multicova/multicova.py` & `alphastats-0.6.7/alphastats/multicova/multicova.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/alphastats/plots/ClusterMap.py` & `alphastats-0.6.7/alphastats/plots/ClusterMap.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/alphastats/plots/DimensionalityReduction.py` & `alphastats-0.6.7/alphastats/plots/DimensionalityReduction.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/alphastats/plots/IntensityPlot.py` & `alphastats-0.6.7/alphastats/plots/IntensityPlot.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/alphastats/plots/PlotUtils.py` & `alphastats-0.6.7/alphastats/plots/PlotUtils.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/alphastats/plots/SampleHistogram.py` & `alphastats-0.6.7/alphastats/plots/SampleHistogram.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/alphastats/plots/VolcanoPlot.py` & `alphastats-0.6.7/alphastats/plots/VolcanoPlot.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/alphastats/statistics/Anova.py` & `alphastats-0.6.7/alphastats/statistics/Anova.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/alphastats/statistics/DifferentialExpressionAnalysis.py` & `alphastats-0.6.7/alphastats/statistics/DifferentialExpressionAnalysis.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/alphastats/statistics/MultiCovaAnalysis.py` & `alphastats-0.6.7/alphastats/statistics/MultiCovaAnalysis.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/alphastats/statistics/StatisticUtils.py` & `alphastats-0.6.7/alphastats/statistics/StatisticUtils.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/alphastats/utils.py` & `alphastats-0.6.7/alphastats/utils.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/alphastats.egg-info/PKG-INFO` & `alphastats-0.6.7/alphastats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphastats
-Version: 0.6.6
+Version: 0.6.7
 Summary: An open-source Python package for automated and scalable statistical analysis of mass spectrometry-based proteomics
 Home-page: https://github.com/MannLabs/alphastats
 Author: Mann Labs
 Author-email: elena.krismer@gmail.com
 License: Apache
 Project-URL: Mann Labs at MPIB, https://www.biochem.mpg.de/mann
 Project-URL: GitHub, https://github.com/MannLabs/alphapeptstats
```

### Comparing `alphastats-0.6.6/alphastats.egg-info/SOURCES.txt` & `alphastats-0.6.7/alphastats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/setup.py` & `alphastats-0.6.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     return required
 
 
 def create_pip_wheel():
     requirements = get_requirements()
     setuptools.setup(
         name="alphastats",
-        version="0.6.6",
+        version="0.6.7",
         license="Apache",
         description="An open-source Python package for automated and scalable statistical analysis of mass spectrometry-based proteomics",
         long_description=get_long_description(),
         long_description_content_type="text/markdown",
         author="Mann Labs",
         author_email="elena.krismer@gmail.com",
         url="https://github.com/MannLabs/alphastats",
```

### Comparing `alphastats-0.6.6/tests/test_DataSet.py` & `alphastats-0.6.7/tests/test_DataSet.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/tests/test_DataSet_Pathway.py` & `alphastats-0.6.7/tests/test_DataSet_Pathway.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.6/tests/test_loaders.py` & `alphastats-0.6.7/tests/test_loaders.py`

 * *Files identical despite different names*

