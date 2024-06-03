# Comparing `tmp/syngen-0.9.1.tar.gz` & `tmp/syngen-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syngen-0.9.1.tar", last modified: Sat Jun  1 12:16:41 2024, max compression
+gzip compressed data, was "syngen-0.9.2.tar", last modified: Mon Jun  3 14:38:23 2024, max compression
```

## Comparing `syngen-0.9.1.tar` & `syngen-0.9.2.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:16:41.166595 syngen-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-06-01 12:15:22.000000 syngen-0.9.1/DESCRIPTION
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-01 12:15:22.000000 syngen-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-06-01 12:15:22.000000 syngen-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    29861 2024-06-01 12:16:41.166595 syngen-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    27936 2024-06-01 12:15:22.000000 syngen-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-06-01 12:15:22.000000 syngen-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-06-01 12:16:41.166595 syngen-0.9.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:16:41.146595 syngen-0.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:16:41.150595 syngen-0.9.1/src/syngen/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/infer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:16:41.154595 syngen-0.9.1/src/syngen/ml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:16:41.154595 syngen-0.9.1/src/syngen/ml/config/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11766 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/config/configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/config/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:16:41.154595 syngen-0.9.1/src/syngen/ml/context/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/context/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:16:41.154595 syngen-0.9.1/src/syngen/ml/convertor/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/convertor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/convertor/convertor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:16:41.154595 syngen-0.9.1/src/syngen/ml/data_loaders/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/data_loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17252 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/data_loaders/data_loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:16:41.154595 syngen-0.9.1/src/syngen/ml/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18510 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/handlers/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:16:41.154595 syngen-0.9.1/src/syngen/ml/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/metrics/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:16:41.154595 syngen-0.9.1/src/syngen/ml/metrics/accuracy_test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/metrics/accuracy_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   723510 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
--rw-r--r--   0 runner    (1001) docker     (127)     9493 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:16:41.158595 syngen-0.9.1/src/syngen/ml/metrics/accuracy_test/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:16:41.158595 syngen-0.9.1/src/syngen/ml/metrics/accuracy_test/src/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)   528976 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:16:41.158595 syngen-0.9.1/src/syngen/ml/metrics/accuracy_test/src/img/
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/metrics/accuracy_test/src/img/linear-gradient.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/metrics/accuracy_test/src/main.css
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/metrics/accuracy_test/src/script.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:16:41.158595 syngen-0.9.1/src/syngen/ml/metrics/metrics_classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/metrics/metrics_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46479 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/metrics/metrics_classes/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:16:41.158595 syngen-0.9.1/src/syngen/ml/metrics/sample_test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/metrics/sample_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   708975 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/metrics/sample_test/sample_report_template.html
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/metrics/sample_test/sample_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:16:41.158595 syngen-0.9.1/src/syngen/ml/mlflow_tracker/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/mlflow_tracker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9520 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/mlflow_tracker/mlflow_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:16:41.158595 syngen-0.9.1/src/syngen/ml/reporters/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9687 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/reporters/reporters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:16:41.158595 syngen-0.9.1/src/syngen/ml/strategies/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8414 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/strategies/strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:16:41.158595 syngen-0.9.1/src/syngen/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12414 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:16:41.158595 syngen-0.9.1/src/syngen/ml/vae/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/vae/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/vae/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:16:41.162595 syngen-0.9.1/src/syngen/ml/vae/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/vae/models/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/vae/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/vae/models/custom_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)    46231 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/vae/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    24260 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/vae/models/features.py
--rw-r--r--   0 runner    (1001) docker     (127)    10457 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/vae/models/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:16:41.162595 syngen-0.9.1/src/syngen/ml/vae/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/vae/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14141 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/vae/wrappers/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:16:41.162595 syngen-0.9.1/src/syngen/ml/validation_schema/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/validation_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/validation_schema/validation_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:16:41.162595 syngen-0.9.1/src/syngen/ml/worker/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19173 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/ml/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:16:41.162595 syngen-0.9.1/src/syngen/streamlit_app/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:16:41.162595 syngen-0.9.1/src/syngen/streamlit_app/.streamlit/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/streamlit_app/.streamlit/config.toml
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/streamlit_app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:16:41.162595 syngen-0.9.1/src/syngen/streamlit_app/css/
--rw-r--r--   0 runner    (1001) docker     (127)   707122 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/streamlit_app/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:16:41.162595 syngen-0.9.1/src/syngen/streamlit_app/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/streamlit_app/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/streamlit_app/handlers/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:16:41.162595 syngen-0.9.1/src/syngen/streamlit_app/img/
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/streamlit_app/img/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/streamlit_app/img/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/streamlit_app/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/streamlit_app/start.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:16:41.162595 syngen-0.9.1/src/syngen/streamlit_app/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/streamlit_app/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/streamlit_app/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-06-01 12:15:22.000000 syngen-0.9.1/src/syngen/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:16:41.166595 syngen-0.9.1/src/syngen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    29861 2024-06-01 12:16:41.000000 syngen-0.9.1/src/syngen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-06-01 12:16:41.000000 syngen-0.9.1/src/syngen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 12:16:41.000000 syngen-0.9.1/src/syngen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-06-01 12:16:41.000000 syngen-0.9.1/src/syngen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-06-01 12:16:41.000000 syngen-0.9.1/src/syngen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-01 12:16:41.000000 syngen-0.9.1/src/syngen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:38:23.497053 syngen-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-06-03 14:37:00.000000 syngen-0.9.2/DESCRIPTION
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-03 14:37:00.000000 syngen-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-06-03 14:37:00.000000 syngen-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    29861 2024-06-03 14:38:23.497053 syngen-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27936 2024-06-03 14:37:00.000000 syngen-0.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-06-03 14:37:00.000000 syngen-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-06-03 14:38:23.497053 syngen-0.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:38:23.481054 syngen-0.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:38:23.485054 syngen-0.9.2/src/syngen/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/infer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:38:23.485054 syngen-0.9.2/src/syngen/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:38:23.485054 syngen-0.9.2/src/syngen/ml/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11766 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/config/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/config/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:38:23.485054 syngen-0.9.2/src/syngen/ml/context/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/context/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:38:23.485054 syngen-0.9.2/src/syngen/ml/convertor/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/convertor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/convertor/convertor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:38:23.485054 syngen-0.9.2/src/syngen/ml/data_loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/data_loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17252 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/data_loaders/data_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:38:23.485054 syngen-0.9.2/src/syngen/ml/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18800 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/handlers/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:38:23.489054 syngen-0.9.2/src/syngen/ml/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/metrics/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:38:23.489054 syngen-0.9.2/src/syngen/ml/metrics/accuracy_test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/metrics/accuracy_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   723510 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9493 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:38:23.489054 syngen-0.9.2/src/syngen/ml/metrics/accuracy_test/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:38:23.489054 syngen-0.9.2/src/syngen/ml/metrics/accuracy_test/src/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   528976 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:38:23.489054 syngen-0.9.2/src/syngen/ml/metrics/accuracy_test/src/img/
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/metrics/accuracy_test/src/img/linear-gradient.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/metrics/accuracy_test/src/main.css
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/metrics/accuracy_test/src/script.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:38:23.489054 syngen-0.9.2/src/syngen/ml/metrics/metrics_classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/metrics/metrics_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46479 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/metrics/metrics_classes/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:38:23.489054 syngen-0.9.2/src/syngen/ml/metrics/sample_test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/metrics/sample_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   708975 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/metrics/sample_test/sample_report_template.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/metrics/sample_test/sample_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:38:23.489054 syngen-0.9.2/src/syngen/ml/mlflow_tracker/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/mlflow_tracker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9520 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/mlflow_tracker/mlflow_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:38:23.489054 syngen-0.9.2/src/syngen/ml/reporters/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9687 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/reporters/reporters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:38:23.493054 syngen-0.9.2/src/syngen/ml/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8414 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/strategies/strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:38:23.493054 syngen-0.9.2/src/syngen/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12175 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:38:23.493054 syngen-0.9.2/src/syngen/ml/vae/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/vae/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/vae/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:38:23.493054 syngen-0.9.2/src/syngen/ml/vae/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/vae/models/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/vae/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/vae/models/custom_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46221 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/vae/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24260 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/vae/models/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10437 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/vae/models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:38:23.493054 syngen-0.9.2/src/syngen/ml/vae/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/vae/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/vae/wrappers/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:38:23.493054 syngen-0.9.2/src/syngen/ml/validation_schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/validation_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/validation_schema/validation_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:38:23.493054 syngen-0.9.2/src/syngen/ml/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19173 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/ml/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:38:23.493054 syngen-0.9.2/src/syngen/streamlit_app/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:38:23.493054 syngen-0.9.2/src/syngen/streamlit_app/.streamlit/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/streamlit_app/.streamlit/config.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/streamlit_app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:38:23.493054 syngen-0.9.2/src/syngen/streamlit_app/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   707122 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/streamlit_app/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:38:23.497053 syngen-0.9.2/src/syngen/streamlit_app/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/streamlit_app/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/streamlit_app/handlers/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:38:23.497053 syngen-0.9.2/src/syngen/streamlit_app/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/streamlit_app/img/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/streamlit_app/img/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/streamlit_app/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/streamlit_app/start.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:38:23.497053 syngen-0.9.2/src/syngen/streamlit_app/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/streamlit_app/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/streamlit_app/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-06-03 14:37:00.000000 syngen-0.9.2/src/syngen/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:38:23.497053 syngen-0.9.2/src/syngen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    29861 2024-06-03 14:38:23.000000 syngen-0.9.2/src/syngen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-06-03 14:38:23.000000 syngen-0.9.2/src/syngen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 14:38:23.000000 syngen-0.9.2/src/syngen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-06-03 14:38:23.000000 syngen-0.9.2/src/syngen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-06-03 14:38:23.000000 syngen-0.9.2/src/syngen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-03 14:38:23.000000 syngen-0.9.2/src/syngen.egg-info/top_level.txt
```

### Comparing `syngen-0.9.1/LICENSE` & `syngen-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `syngen-0.9.1/PKG-INFO` & `syngen-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngen
-Version: 0.9.1
+Version: 0.9.2
 Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen
 Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev
 License: GPLv3 License
 Keywords: data,generation,synthetic,vae,tabular
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `syngen-0.9.1/README.md` & `syngen-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `syngen-0.9.1/setup.cfg` & `syngen-0.9.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `syngen-0.9.1/src/syngen/infer.py` & `syngen-0.9.2/src/syngen/infer.py`

 * *Files identical despite different names*

### Comparing `syngen-0.9.1/src/syngen/ml/config/configurations.py` & `syngen-0.9.2/src/syngen/ml/config/configurations.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 
     def preprocess_data(self):
         data, self.schema = self._extract_data()
         self.columns = list(data.columns)
         data = self._remove_empty_columns(data)
         self._mark_removed_columns(data)
         self._prepare_data(data)
-        self._set_batch_size()
 
     def to_dict(self) -> Dict:
         """
         Return the values of the settings of training process
         """
         return {
             "epochs": self.epochs,
@@ -164,14 +163,15 @@
                 f"please consider any of the steps: 1) provide a bigger table, "
                 f"2) disable drop_null argument"
             )
 
         logger.info(f"The subset of rows was set to {len(data)}")
 
         self.row_subset = len(data)
+        self._set_batch_size()
         return data
 
     def _save_input_data(self, data: pd.DataFrame):
         DataLoader(self.paths["input_data_path"]).save_data(self.paths["input_data_path"], data)
 
     def _prepare_data(self, data: pd.DataFrame):
         """
```

### Comparing `syngen-0.9.1/src/syngen/ml/config/validation.py` & `syngen-0.9.2/src/syngen/ml/config/validation.py`

 * *Files identical despite different names*

### Comparing `syngen-0.9.1/src/syngen/ml/context/context.py` & `syngen-0.9.2/src/syngen/ml/context/context.py`

 * *Files identical despite different names*

### Comparing `syngen-0.9.1/src/syngen/ml/convertor/convertor.py` & `syngen-0.9.2/src/syngen/ml/convertor/convertor.py`

 * *Files identical despite different names*

### Comparing `syngen-0.9.1/src/syngen/ml/data_loaders/data_loaders.py` & `syngen-0.9.2/src/syngen/ml/data_loaders/data_loaders.py`

 * *Files identical despite different names*

### Comparing `syngen-0.9.1/src/syngen/ml/handlers/handlers.py` & `syngen-0.9.2/src/syngen/ml/handlers/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,18 +174,15 @@
 
         logger.debug(
             f"Train model with parameters: epochs={self.epochs}, "
             f"row_subset={self.row_subset}, print_report={self.print_report}, "
             f"drop_null={self.drop_null}, batch_size={self.batch_size}"
         )
 
-        self.model.fit_on_df(
-            data,
-            epochs=self.epochs,
-        )
+        self.model.fit_on_df(epochs=self.epochs)
 
         if not check_if_features_assigned(self.paths["dataset_pickle_path"]):
             return
 
         self.model.save_state(self.paths["state_path"])
         log_message = "Finished VAE training"
         logger.info(log_message)
@@ -220,26 +217,61 @@
     def __post_init__(self):
         if self.random_seed:
             seed(self.random_seed)
         self.random_seeds_list = list()
         self.vae = None
         self.dataset = fetch_dataset(self.paths["dataset_pickle_path"])
         self.has_vae = len(self.dataset.features) > 0
+
+        data, schema = self._get_data()
+
+        if self.has_vae:
+            self.vae = self._get_wrapper(data, schema)
+
         self.has_no_ml = os.path.exists(f'{self.paths["path_to_no_ml"]}')
 
     @staticmethod
     def synth_word(size, indexes, counts):
         return "".join(
             np.random.choice(
                 np.array(list(indexes)),
                 size=size,
                 p=np.array(list(counts.values())) / sum(np.array(list(counts.values()))),
             )
         )
 
+    def _get_data(self) -> Tuple[pd.DataFrame, Dict]:
+        """
+        Load the data from the input data path
+        """
+        input_data_existed = DataLoader(self.paths["input_data_path"]).has_existed_path
+
+        if input_data_existed:
+            data, schema = DataLoader(self.paths["input_data_path"]).load_data()
+        else:
+            data = pd.DataFrame()
+            schema = None
+        return data, schema
+
+    def _get_wrapper(self, data: pd.DataFrame, schema: Dict):
+        """
+        Create and get the wrapper for the VAE model
+        """
+        return self.create_wrapper(
+            self.wrapper_name,
+            data,
+            schema,
+            metadata=self.metadata,
+            table_name=self.table_name,
+            paths=self.paths,
+            batch_size=self.batch_size,
+            main_process=self.type_of_process,
+            process="infer",
+        )
+
     def _prepare_dir(self):
         tmp_store_path = self.paths["tmp_store_path"]
         os.makedirs(tmp_store_path, exist_ok=True)
 
     def _is_pk(self):
         is_pk = self.table_name.endswith("_pk")
         return is_pk
@@ -254,27 +286,15 @@
                 ):
                     cumm_len = 0
                     for i, frame in enumerate(df_slices):
                         frame[column] = frame[column].map(lambda pk_val: pk_val + cumm_len)
                         cumm_len += len(frame)
         return pd.concat(df_slices, ignore_index=True)
 
-    def generate_vae(self, size, data, schema):
-        self.vae = self.create_wrapper(
-            self.wrapper_name,
-            data,
-            schema,
-            metadata=self.metadata,
-            table_name=self.table_name,
-            paths=self.paths,
-            batch_size=self.batch_size,
-            main_process=self.type_of_process,
-            process="infer",
-        )
-        self.vae.load_state(self.paths["state_path"])
+    def generate_vae(self, size):
         synthetic_infer = self.vae.predict_sampled_df(size)
         return synthetic_infer
 
     def generate_long_texts(self, size, synthetic_infer):
         with open(f'{self.paths["path_to_no_ml"]}', "rb") as file:
             features = dill.load(file)
         for col in features.keys():
@@ -296,25 +316,18 @@
 
     def run_separate(self, params: Tuple):
         i, size = params
 
         if self.random_seed:
             seed(self.random_seeds_list[i])
 
-        input_data_existed = DataLoader(self.paths["input_data_path"]).has_existed_path
-
-        if input_data_existed:
-            data, schema = DataLoader(self.paths["input_data_path"]).load_data()
-        else:
-            data = pd.DataFrame()
-            schema = None
-
         synthetic_infer = pd.DataFrame()
+
         if self.has_vae:
-            synthetic_infer = self.generate_vae(size, data, schema)
+            synthetic_infer = self.generate_vae(size)
         if self.has_no_ml:
             synthetic_infer = self.generate_long_texts(size, synthetic_infer)
 
         uuid_columns = self.dataset.uuid_columns
         if uuid_columns:
             synthetic_infer = generate_uuid(size, self.dataset, uuid_columns, synthetic_infer)
```

### Comparing `syngen-0.9.1/src/syngen/ml/metrics/accuracy_test/accuracy_report.html` & `syngen-0.9.2/src/syngen/ml/metrics/accuracy_test/accuracy_report.html`

 * *Files identical despite different names*

### Comparing `syngen-0.9.1/src/syngen/ml/metrics/accuracy_test/accuracy_test.py` & `syngen-0.9.2/src/syngen/ml/metrics/accuracy_test/accuracy_test.py`

 * *Files identical despite different names*

### Comparing `syngen-0.9.1/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf` & `syngen-0.9.2/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf`

 * *Files identical despite different names*

### Comparing `syngen-0.9.1/src/syngen/ml/metrics/accuracy_test/src/img/linear-gradient.svg` & `syngen-0.9.2/src/syngen/ml/metrics/accuracy_test/src/img/linear-gradient.svg`

 * *Files identical despite different names*

### Comparing `syngen-0.9.1/src/syngen/ml/metrics/accuracy_test/src/main.css` & `syngen-0.9.2/src/syngen/ml/metrics/accuracy_test/src/main.css`

 * *Files identical despite different names*

### Comparing `syngen-0.9.1/src/syngen/ml/metrics/metrics_classes/metrics.py` & `syngen-0.9.2/src/syngen/ml/metrics/metrics_classes/metrics.py`

 * *Files identical despite different names*

### Comparing `syngen-0.9.1/src/syngen/ml/metrics/sample_test/sample_report_template.html` & `syngen-0.9.2/src/syngen/ml/metrics/sample_test/sample_report_template.html`

 * *Files identical despite different names*

### Comparing `syngen-0.9.1/src/syngen/ml/metrics/sample_test/sample_test.py` & `syngen-0.9.2/src/syngen/ml/metrics/sample_test/sample_test.py`

 * *Files identical despite different names*

### Comparing `syngen-0.9.1/src/syngen/ml/metrics/utils.py` & `syngen-0.9.2/src/syngen/ml/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `syngen-0.9.1/src/syngen/ml/mlflow_tracker/mlflow_tracker.py` & `syngen-0.9.2/src/syngen/ml/mlflow_tracker/mlflow_tracker.py`

 * *Files identical despite different names*

### Comparing `syngen-0.9.1/src/syngen/ml/reporters/reporters.py` & `syngen-0.9.2/src/syngen/ml/reporters/reporters.py`

 * *Files identical despite different names*

### Comparing `syngen-0.9.1/src/syngen/ml/strategies/strategies.py` & `syngen-0.9.2/src/syngen/ml/strategies/strategies.py`

 * *Files identical despite different names*

### Comparing `syngen-0.9.1/src/syngen/ml/utils/__init__.py` & `syngen-0.9.2/src/syngen/ml/utils/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     fetch_training_config,
     fetch_unique_root,
     generate_uuid,
     generate_uuids,
     setup_logger,
     datetime_to_timestamp,
     timestamp_to_datetime,
-    define_existent_columns,
     set_log_path,
     clean_up_metadata,
     fetch_log_message,
     file_sink,
     ProgressBarHandler,
     check_if_logs_available,
     get_initial_table_name
```

### Comparing `syngen-0.9.1/src/syngen/ml/utils/utils.py` & `syngen-0.9.2/src/syngen/ml/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,23 +240,14 @@
     Deserialize and return the object of class Dataset
     """
     with open(dataset_pickle_path, "rb") as f:
         dataset = pickle.loads(f.read())
     return dataset
 
 
-def define_existent_columns(columns, original_columns):
-    existent_columns = []
-    for column in columns:
-        if column in original_columns:
-            existent_columns.append(column)
-        continue
-    return existent_columns
-
-
 def slugify_attribute(**kwargs):
     """
     Slugify the value of the attribute of the instance
     and set it to the new attribute
     """
 
     def wrapper(function):
```

### Comparing `syngen-0.9.1/src/syngen/ml/vae/models/custom_layers.py` & `syngen-0.9.2/src/syngen/ml/vae/models/custom_layers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.9.1/src/syngen/ml/vae/models/dataset.py` & `syngen-0.9.2/src/syngen/ml/vae/models/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -808,17 +808,17 @@
 
         Args:
             nan_labels (dict): dictionary that matches column name to the label of missing value
                                (e.g. {'Score': 'Not available'})
         """
         self.nan_labels_dict = nan_labels
 
-    def fit(self, data):
+    def fit(self):
         for name, feature in self.features.items():
-            feature.fit(data[self.columns[name]], date_mapping=self.date_mapping)
+            feature.fit(self.df[self.columns[name]], date_mapping=self.date_mapping)
 
         self.all_columns = [col for col in self.columns]
         self.is_fitted = True
 
     def transform(self, data, excluded_features=set()):
         transformed_features = list()
         selected_features = {
@@ -1163,13 +1163,13 @@
             elif column in self.date_columns:
                 self._assign_date_feature(column)
             elif column in self.binary_columns:
                 self._assign_binary_feature(column)
 
         self.set_nan_params(columns_nan_labels)
 
-        self.fit(self.df)
+        self.fit()
 
         # The end of the run related to the preprocessing stage
         MlflowTracker().end_run()
 
         return self.df
```

### Comparing `syngen-0.9.1/src/syngen/ml/vae/models/features.py` & `syngen-0.9.2/src/syngen/ml/vae/models/features.py`

 * *Files identical despite different names*

### Comparing `syngen-0.9.1/src/syngen/ml/vae/models/model.py` & `syngen-0.9.2/src/syngen/ml/vae/models/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,8 +260,7 @@
     def load_state(self, path: str):
         pth = Path(path)
         self.model.load_weights(str(pth / "vae.ckpt"))
         self.generator_model.load_weights(str(pth / "vae_generator.ckpt"))
 
         with open(str(pth / "latent_model.pkl"), "rb") as f:
             self.latent_model = pickle.loads(f.read())
-        return self
```

### Comparing `syngen-0.9.1/src/syngen/ml/vae/wrappers/wrappers.py` & `syngen-0.9.2/src/syngen/ml/vae/wrappers/wrappers.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,159 +19,85 @@
 from syngen.ml.vae.models.model import CVAE
 from syngen.ml.vae.models import Dataset
 from syngen.ml.mlflow_tracker import MlflowTracker
 from syngen.ml.utils import (
     fetch_dataset,
     fetch_training_config,
     check_if_features_assigned,
-    define_existent_columns,
     ProgressBarHandler
 )
 
 warnings.filterwarnings("ignore")
 
 BATCH_SIZE_DEFAULT = 32
 
 
 class BaseWrapper(ABC):
     """
     Abstract class for wrappers
     """
 
-    def __init__(self):
-        self.model = None
-
     @abstractmethod
     def fit_on_df(self, df: pd.DataFrame, epochs: int, columns_subset: List[str] = None):
         pass
 
     @abstractmethod
     def predict_sampled_df(self, n: int) -> pd.DataFrame:
         pass
 
     @abstractmethod
     def save_state(self, path: str):
         pass
 
-    @abstractmethod
-    def load_state(self, path: str):
-        pass
-
 
 @dataclass
 class VAEWrapper(BaseWrapper):
-    """Base class that implements end to end train and generation of structured data.
-
-    Attributes
-    ----------
-    df
-    schema
-    metadata
-    table_name
-    paths
-    process
-    batch_size
-    latent_dim
-    latent_components
-
-    Methods
-    -------
-    _pipeline()
-        data preprocessing
-
-    _train(dataset, row_subset, epochs)
-        train the VAE and save result in model
-
-    display_losses()
-        show train losses curve by each feature
-
-    predict_sampled_df(df, n)
-        generate new data based on df that consist of n rows and return the result as pd.DataFrame
-
-    predict_less_likely_samples(df, n, temp=0.05, variety=3)
-        generate new data based on df that consist of n which has less probability
-        computed as log likelihood and return the result as pd.DataFrame
-    """
     df: pd.DataFrame
     schema: Optional[Dict]
-    metadata: dict
+    metadata: Dict
     table_name: str
-    paths: dict
+    paths: Dict
     process: str
     main_process: str
     batch_size: int
-    latent_dim: int = field(init=False, default=10)
-    latent_components: int = field(init=False, default=30)
+    dataset: Dataset = field(init=False)
+    model: CVAE = field(init=False, default=None)
 
     def __post_init__(self):
         if self.process == "train":
             self.dataset = Dataset(
                 df=self.df,
                 schema=self.schema,
                 metadata=self.metadata,
                 table_name=self.table_name,
                 main_process=self.main_process,
                 paths=self.paths,
             )
             self.dataset.set_metadata()
+            self.df = self.dataset.pipeline()
+            self._save_dataset()
         elif self.process == "infer":
             self.dataset = fetch_dataset(self.paths["dataset_pickle_path"])
             self._update_dataset()
             self._save_dataset()
 
     def _update_dataset(self):
-        # Check if the serialized class has associated dataframe and
-        # drop it as it might contain sensitive data.
-        # Save columns from the dataframe for later use.
-        self.dataset.paths = self.paths
-        self.dataset.main_process = self.main_process
-        self.dataset.metadata = self.metadata
-        existed_columns = fetch_training_config(self.paths["train_config_pickle_path"]).columns
-
-        if hasattr(self.dataset, "df"):
-            self.dataset.order_of_columns = existed_columns
-            delattr(self, "df")
-
-            self.__update_attributes(existed_columns)
-
-    def __update_attributes(self, existed_columns: List[str]):
         """
-        Update attributes of the dataset object
+        Update dataset object related to the current process
         """
-        for attr in vars(self.dataset):
-            if attr in [
-                "primary_keys_mapping",
-                "unique_keys_mapping",
-                "foreign_keys_mapping",
-            ]:
-                attr_value = getattr(self.dataset, attr)
-                updated_attr_value = attr_value.copy()
-                for key, config in attr_value.items():
-                    updated_columns = define_existent_columns(
-                        config.get("columns", []), existed_columns
-                    )
-                    config["columns"] = updated_columns
-                    updated_attr_value[key] = config
-
-                setattr(self.dataset, attr, updated_attr_value)
+        self.dataset.paths = self.paths
+        self.dataset.main_process = self.main_process
 
     def _save_dataset(self):
         """
         Save dataset object on the disk
         """
         with open(self.paths["dataset_pickle_path"], "wb") as f:
             f.write(pickle.dumps(self.dataset))
 
-    def _pipeline(self):
-        """
-        Launch the pipeline in the dataset
-        """
-        self.df = self.dataset.pipeline()
-        self._save_dataset()
-
     def _restore_zero_values(self, df):
         for column in self.dataset.zero_num_column_names:
             if column.endswith("_zero"):
                 # remove _zero to get original column name
                 num_column_name = column[:-5]
                 num_column = df[num_column_name].copy()
                 zero_column_mask = df[column].astype("float") >= 0.5
@@ -209,28 +135,21 @@
             if nan_label is None:
                 nan_label = np.nan
             if column_name in df.select_dtypes(int).columns:
                 df[column_name] = df[column_name].astype("object")
             df[column_name] = df[column_name].fillna(nan_label)
         return df
 
-    @abstractmethod
-    def _init_model(self):
-        pass
-
     def fit_on_df(
         self,
-        df: pd.DataFrame,
         epochs: int,
         columns_subset: List[str] = None,  # TODO columns_subset does not work
     ):
-        self._pipeline()
         if not check_if_features_assigned(self.paths["dataset_pickle_path"]):
             return
-        self._init_model()
 
         if columns_subset is None:
             columns_subset = self.df.columns
         else:
             # if a column is in columns_subset, its null column should also be added if present
             columns_subset += [
                 col
@@ -381,43 +300,58 @@
 
     def save_state(self, path: str):
         self.model.save_state(path)
         logger.info(f"Saved VAE state in {path}")
 
     def load_state(self, path: str):
         try:
-            with open(path + "/model_dataset.pkl", "rb") as f:
-                self.dataset = pickle.loads(f.read())
-
-            self._init_model()
-
-            state = self.model.load_state(path)
+            self.model.load_state(path)
 
-        except (FileNotFoundError, ValueError):
+        except FileNotFoundError:
             raise FileNotFoundError("Missing file with VAE state")
 
         logger.info(f"Loaded VAE state from {path}")
-        return state
 
 
 class VanillaVAEWrapper(VAEWrapper):
     """
     Class that implements end to end train and generation of structured data by CVAE as a model.
 
     Attributes
     ----------
     model : CVAE
         final model that we will use to generate new data
     """
-
-    def _init_model(self):
-        latent_dim = min(self.latent_dim, int(len(self.dataset.columns) / 2))
+    def __init__(
+            self,
+            df: pd.DataFrame,
+            schema: Optional[Dict],
+            metadata: Dict,
+            table_name: str,
+            paths: Dict,
+            process: str,
+            main_process: str,
+            batch_size: int,
+            latent_dim: int = 10,
+            latent_components: int = 30):
+        super().__init__(
+            df,
+            schema,
+            metadata,
+            table_name,
+            paths,
+            process,
+            main_process,
+            batch_size
+        )
+        self.latent_dim = min(latent_dim, int(len(self.dataset.columns) / 2))
 
         self.model = CVAE(
             self.dataset,
             batch_size=self.batch_size,
             latent_dim=latent_dim,
-            latent_components=min(self.latent_components, latent_dim * 2),
+            latent_components=min(latent_components, latent_dim * 2),
             intermediate_dim=128,
         )
-
         self.model.build_model()
+        if self.process == "infer":
+            self.load_state(self.paths["state_path"])
```

### Comparing `syngen-0.9.1/src/syngen/ml/validation_schema/validation_schema.py` & `syngen-0.9.2/src/syngen/ml/validation_schema/validation_schema.py`

 * *Files identical despite different names*

### Comparing `syngen-0.9.1/src/syngen/ml/worker/worker.py` & `syngen-0.9.2/src/syngen/ml/worker/worker.py`

 * *Files identical despite different names*

### Comparing `syngen-0.9.1/src/syngen/streamlit_app/css/style.css` & `syngen-0.9.2/src/syngen/streamlit_app/css/style.css`

 * *Files identical despite different names*

### Comparing `syngen-0.9.1/src/syngen/streamlit_app/handlers/handlers.py` & `syngen-0.9.2/src/syngen/streamlit_app/handlers/handlers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.9.1/src/syngen/streamlit_app/img/favicon.svg` & `syngen-0.9.2/src/syngen/streamlit_app/img/favicon.svg`

 * *Files identical despite different names*

### Comparing `syngen-0.9.1/src/syngen/streamlit_app/img/logo.svg` & `syngen-0.9.2/src/syngen/streamlit_app/img/logo.svg`

 * *Files identical despite different names*

### Comparing `syngen-0.9.1/src/syngen/streamlit_app/run.py` & `syngen-0.9.2/src/syngen/streamlit_app/run.py`

 * *Files identical despite different names*

### Comparing `syngen-0.9.1/src/syngen/streamlit_app/start.py` & `syngen-0.9.2/src/syngen/streamlit_app/start.py`

 * *Files identical despite different names*

### Comparing `syngen-0.9.1/src/syngen/streamlit_app/utils/utils.py` & `syngen-0.9.2/src/syngen/streamlit_app/utils/utils.py`

 * *Files identical despite different names*

### Comparing `syngen-0.9.1/src/syngen/train.py` & `syngen-0.9.2/src/syngen/train.py`

 * *Files identical despite different names*

### Comparing `syngen-0.9.1/src/syngen.egg-info/PKG-INFO` & `syngen-0.9.2/src/syngen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngen
-Version: 0.9.1
+Version: 0.9.2
 Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen
 Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev
 License: GPLv3 License
 Keywords: data,generation,synthetic,vae,tabular
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `syngen-0.9.1/src/syngen.egg-info/SOURCES.txt` & `syngen-0.9.2/src/syngen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `syngen-0.9.1/src/syngen.egg-info/requires.txt` & `syngen-0.9.2/src/syngen.egg-info/requires.txt`

 * *Files identical despite different names*

