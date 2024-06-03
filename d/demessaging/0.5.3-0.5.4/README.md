# Comparing `tmp/demessaging-0.5.3.tar.gz` & `tmp/demessaging-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "demessaging-0.5.3.tar", last modified: Mon May  6 13:52:37 2024, max compression
+gzip compressed data, was "demessaging-0.5.4.tar", last modified: Mon Jun  3 11:30:35 2024, max compression
```

## Comparing `demessaging-0.5.3.tar` & `demessaging-0.5.4.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 13:52:37.166015 demessaging-0.5.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 13:52:37.158015 demessaging-0.5.3/LICENSES/
--rw-rw-rw-   0 root         (0) root         (0)    10280 2024-05-06 13:52:06.000000 demessaging-0.5.3/LICENSES/Apache-2.0.txt
--rw-rw-rw-   0 root         (0) root         (0)    17023 2024-05-06 13:52:06.000000 demessaging-0.5.3/LICENSES/CC-BY-4.0.txt
--rw-rw-rw-   0 root         (0) root         (0)     7048 2024-05-06 13:52:06.000000 demessaging-0.5.3/LICENSES/CC0-1.0.txt
--rw-rw-rw-   0 root         (0) root         (0)      399 2024-05-06 13:52:06.000000 demessaging-0.5.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     9634 2024-05-06 13:52:37.166015 demessaging-0.5.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6012 2024-05-06 13:52:06.000000 demessaging-0.5.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 13:52:37.158015 demessaging-0.5.3/demessaging/
--rw-rw-rw-   0 root         (0) root         (0)     3174 2024-05-06 13:52:06.000000 demessaging-0.5.3/demessaging/NetCDFDecoder.py
--rw-rw-rw-   0 root         (0) root         (0)     1002 2024-05-06 13:52:06.000000 demessaging-0.5.3/demessaging/PulsarConnection.py
--rw-rw-rw-   0 root         (0) root         (0)      545 2024-05-06 13:52:06.000000 demessaging-0.5.3/demessaging/PulsarMessageConstants.py
--rw-rw-rw-   0 root         (0) root         (0)      995 2024-05-06 13:52:06.000000 demessaging-0.5.3/demessaging/PulsarMessageConsumer.py
--rw-rw-rw-   0 root         (0) root         (0)      995 2024-05-06 13:52:06.000000 demessaging-0.5.3/demessaging/PulsarMessageProducer.py
--rw-rw-rw-   0 root         (0) root         (0)     1086 2024-05-06 13:52:06.000000 demessaging-0.5.3/demessaging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      481 2024-05-06 13:52:06.000000 demessaging-0.5.3/demessaging/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2024-05-06 13:52:37.166015 demessaging-0.5.3/demessaging/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 13:52:37.158015 demessaging-0.5.3/demessaging/backend/
--rw-rw-rw-   0 root         (0) root         (0)     3243 2024-05-06 13:52:06.000000 demessaging-0.5.3/demessaging/backend/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10346 2024-05-06 13:52:06.000000 demessaging-0.5.3/demessaging/backend/class_.py
--rw-rw-rw-   0 root         (0) root         (0)     8919 2024-05-06 13:52:06.000000 demessaging-0.5.3/demessaging/backend/function.py
--rw-rw-rw-   0 root         (0) root         (0)    16124 2024-05-06 13:52:06.000000 demessaging-0.5.3/demessaging/backend/module.py
--rw-rw-rw-   0 root         (0) root         (0)     7648 2024-05-06 13:52:06.000000 demessaging-0.5.3/demessaging/backend/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    15440 2024-05-06 13:52:06.000000 demessaging-0.5.3/demessaging/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 13:52:37.162015 demessaging-0.5.3/demessaging/config/
--rw-rw-rw-   0 root         (0) root         (0)      686 2024-05-06 13:52:06.000000 demessaging-0.5.3/demessaging/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2812 2024-05-06 13:52:06.000000 demessaging-0.5.3/demessaging/config/api.py
--rw-rw-rw-   0 root         (0) root         (0)    10632 2024-05-06 13:52:06.000000 demessaging-0.5.3/demessaging/config/backend.py
--rw-rw-rw-   0 root         (0) root         (0)     4108 2024-05-06 13:52:06.000000 demessaging-0.5.3/demessaging/config/logging.py
--rw-rw-rw-   0 root         (0) root         (0)      823 2024-05-06 13:52:06.000000 demessaging-0.5.3/demessaging/config/logging.yaml
--rw-rw-rw-   0 root         (0) root         (0)     6238 2024-05-06 13:52:06.000000 demessaging-0.5.3/demessaging/config/messaging.py
--rw-rw-rw-   0 root         (0) root         (0)     2854 2024-05-06 13:52:06.000000 demessaging-0.5.3/demessaging/config/registry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 13:52:37.162015 demessaging-0.5.3/demessaging/messaging/
--rw-rw-rw-   0 root         (0) root         (0)      497 2024-05-06 13:52:06.000000 demessaging-0.5.3/demessaging/messaging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2944 2024-05-06 13:52:06.000000 demessaging-0.5.3/demessaging/messaging/connection.py
--rw-rw-rw-   0 root         (0) root         (0)     2435 2024-05-06 13:52:06.000000 demessaging-0.5.3/demessaging/messaging/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    18285 2024-05-06 13:52:06.000000 demessaging-0.5.3/demessaging/messaging/consumer.py
--rw-rw-rw-   0 root         (0) root         (0)     9907 2024-05-06 13:52:06.000000 demessaging-0.5.3/demessaging/messaging/producer.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 13:52:06.000000 demessaging-0.5.3/demessaging/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 13:52:37.162015 demessaging-0.5.3/demessaging/serializers/
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-06 13:52:06.000000 demessaging-0.5.3/demessaging/serializers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1359 2024-05-06 13:52:06.000000 demessaging-0.5.3/demessaging/serializers/xarray.py
--rw-rw-rw-   0 root         (0) root         (0)     1235 2024-05-06 13:52:06.000000 demessaging-0.5.3/demessaging/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 13:52:37.162015 demessaging-0.5.3/demessaging/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2715 2024-05-06 13:52:06.000000 demessaging-0.5.3/demessaging/templates/class_.py.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1310 2024-05-06 13:52:06.000000 demessaging-0.5.3/demessaging/templates/function.py.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1500 2024-05-06 13:52:06.000000 demessaging-0.5.3/demessaging/templates/module.py.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     2287 2024-05-06 13:52:06.000000 demessaging-0.5.3/demessaging/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 13:52:37.162015 demessaging-0.5.3/demessaging/validators/
--rw-rw-rw-   0 root         (0) root         (0)      158 2024-05-06 13:52:06.000000 demessaging-0.5.3/demessaging/validators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4170 2024-05-06 13:52:06.000000 demessaging-0.5.3/demessaging/validators/xarray.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 13:52:37.162015 demessaging-0.5.3/demessaging.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9634 2024-05-06 13:52:37.000000 demessaging-0.5.3/demessaging.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1616 2024-05-06 13:52:37.000000 demessaging-0.5.3/demessaging.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 13:52:37.000000 demessaging-0.5.3/demessaging.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2024-05-06 13:52:37.000000 demessaging-0.5.3/demessaging.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 13:52:36.000000 demessaging-0.5.3/demessaging.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      661 2024-05-06 13:52:37.000000 demessaging-0.5.3/demessaging.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-05-06 13:52:37.000000 demessaging-0.5.3/demessaging.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     4050 2024-05-06 13:52:06.000000 demessaging-0.5.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-06 13:52:37.166015 demessaging-0.5.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      472 2024-05-06 13:52:06.000000 demessaging-0.5.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 13:52:37.162015 demessaging-0.5.3/tests/
--rw-rw-rw-   0 root         (0) root         (0)     6971 2024-05-06 13:52:06.000000 demessaging-0.5.3/tests/test_backend_class_.py
--rw-rw-rw-   0 root         (0) root         (0)    11385 2024-05-06 13:52:06.000000 demessaging-0.5.3/tests/test_backend_function.py
--rw-rw-rw-   0 root         (0) root         (0)    17479 2024-05-06 13:52:06.000000 demessaging-0.5.3/tests/test_backend_module.py
--rw-rw-rw-   0 root         (0) root         (0)     3533 2024-05-06 13:52:06.000000 demessaging-0.5.3/tests/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)     2233 2024-05-06 13:52:06.000000 demessaging-0.5.3/tests/test_logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:30:35.803021 demessaging-0.5.4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:30:35.791021 demessaging-0.5.4/LICENSES/
+-rw-rw-rw-   0 root         (0) root         (0)    10280 2024-06-03 11:30:07.000000 demessaging-0.5.4/LICENSES/Apache-2.0.txt
+-rw-rw-rw-   0 root         (0) root         (0)    17023 2024-06-03 11:30:07.000000 demessaging-0.5.4/LICENSES/CC-BY-4.0.txt
+-rw-rw-rw-   0 root         (0) root         (0)     7048 2024-06-03 11:30:07.000000 demessaging-0.5.4/LICENSES/CC0-1.0.txt
+-rw-rw-rw-   0 root         (0) root         (0)      399 2024-06-03 11:30:07.000000 demessaging-0.5.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     9634 2024-06-03 11:30:35.803021 demessaging-0.5.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6012 2024-06-03 11:30:07.000000 demessaging-0.5.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:30:35.795021 demessaging-0.5.4/demessaging/
+-rw-rw-rw-   0 root         (0) root         (0)     3174 2024-06-03 11:30:07.000000 demessaging-0.5.4/demessaging/NetCDFDecoder.py
+-rw-rw-rw-   0 root         (0) root         (0)     1002 2024-06-03 11:30:07.000000 demessaging-0.5.4/demessaging/PulsarConnection.py
+-rw-rw-rw-   0 root         (0) root         (0)      545 2024-06-03 11:30:07.000000 demessaging-0.5.4/demessaging/PulsarMessageConstants.py
+-rw-rw-rw-   0 root         (0) root         (0)      995 2024-06-03 11:30:07.000000 demessaging-0.5.4/demessaging/PulsarMessageConsumer.py
+-rw-rw-rw-   0 root         (0) root         (0)      995 2024-06-03 11:30:07.000000 demessaging-0.5.4/demessaging/PulsarMessageProducer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1086 2024-06-03 11:30:07.000000 demessaging-0.5.4/demessaging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      481 2024-06-03 11:30:07.000000 demessaging-0.5.4/demessaging/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-06-03 11:30:35.803021 demessaging-0.5.4/demessaging/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:30:35.795021 demessaging-0.5.4/demessaging/backend/
+-rw-rw-rw-   0 root         (0) root         (0)     3243 2024-06-03 11:30:07.000000 demessaging-0.5.4/demessaging/backend/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10516 2024-06-03 11:30:07.000000 demessaging-0.5.4/demessaging/backend/class_.py
+-rw-rw-rw-   0 root         (0) root         (0)     8919 2024-06-03 11:30:07.000000 demessaging-0.5.4/demessaging/backend/function.py
+-rw-rw-rw-   0 root         (0) root         (0)    16124 2024-06-03 11:30:07.000000 demessaging-0.5.4/demessaging/backend/module.py
+-rw-rw-rw-   0 root         (0) root         (0)     7648 2024-06-03 11:30:07.000000 demessaging-0.5.4/demessaging/backend/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    15440 2024-06-03 11:30:07.000000 demessaging-0.5.4/demessaging/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:30:35.795021 demessaging-0.5.4/demessaging/config/
+-rw-rw-rw-   0 root         (0) root         (0)      686 2024-06-03 11:30:07.000000 demessaging-0.5.4/demessaging/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2812 2024-06-03 11:30:07.000000 demessaging-0.5.4/demessaging/config/api.py
+-rw-rw-rw-   0 root         (0) root         (0)    10632 2024-06-03 11:30:07.000000 demessaging-0.5.4/demessaging/config/backend.py
+-rw-rw-rw-   0 root         (0) root         (0)     4108 2024-06-03 11:30:07.000000 demessaging-0.5.4/demessaging/config/logging.py
+-rw-rw-rw-   0 root         (0) root         (0)      823 2024-06-03 11:30:07.000000 demessaging-0.5.4/demessaging/config/logging.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     6238 2024-06-03 11:30:07.000000 demessaging-0.5.4/demessaging/config/messaging.py
+-rw-rw-rw-   0 root         (0) root         (0)     2854 2024-06-03 11:30:07.000000 demessaging-0.5.4/demessaging/config/registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:30:35.795021 demessaging-0.5.4/demessaging/messaging/
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-06-03 11:30:07.000000 demessaging-0.5.4/demessaging/messaging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2944 2024-06-03 11:30:07.000000 demessaging-0.5.4/demessaging/messaging/connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     2435 2024-06-03 11:30:07.000000 demessaging-0.5.4/demessaging/messaging/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    18285 2024-06-03 11:30:07.000000 demessaging-0.5.4/demessaging/messaging/consumer.py
+-rw-rw-rw-   0 root         (0) root         (0)     9907 2024-06-03 11:30:07.000000 demessaging-0.5.4/demessaging/messaging/producer.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-03 11:30:07.000000 demessaging-0.5.4/demessaging/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:30:35.795021 demessaging-0.5.4/demessaging/serializers/
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-06-03 11:30:07.000000 demessaging-0.5.4/demessaging/serializers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2024-06-03 11:30:07.000000 demessaging-0.5.4/demessaging/serializers/xarray.py
+-rw-rw-rw-   0 root         (0) root         (0)     1235 2024-06-03 11:30:07.000000 demessaging-0.5.4/demessaging/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:30:35.799021 demessaging-0.5.4/demessaging/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2715 2024-06-03 11:30:07.000000 demessaging-0.5.4/demessaging/templates/class_.py.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1310 2024-06-03 11:30:07.000000 demessaging-0.5.4/demessaging/templates/function.py.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1500 2024-06-03 11:30:07.000000 demessaging-0.5.4/demessaging/templates/module.py.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     2287 2024-06-03 11:30:07.000000 demessaging-0.5.4/demessaging/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:30:35.799021 demessaging-0.5.4/demessaging/validators/
+-rw-rw-rw-   0 root         (0) root         (0)      158 2024-06-03 11:30:07.000000 demessaging-0.5.4/demessaging/validators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4170 2024-06-03 11:30:07.000000 demessaging-0.5.4/demessaging/validators/xarray.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:30:35.799021 demessaging-0.5.4/demessaging.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9634 2024-06-03 11:30:35.000000 demessaging-0.5.4/demessaging.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1616 2024-06-03 11:30:35.000000 demessaging-0.5.4/demessaging.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 11:30:35.000000 demessaging-0.5.4/demessaging.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2024-06-03 11:30:35.000000 demessaging-0.5.4/demessaging.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 11:30:35.000000 demessaging-0.5.4/demessaging.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      661 2024-06-03 11:30:35.000000 demessaging-0.5.4/demessaging.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-06-03 11:30:35.000000 demessaging-0.5.4/demessaging.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     4050 2024-06-03 11:30:07.000000 demessaging-0.5.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-06-03 11:30:35.803021 demessaging-0.5.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      472 2024-06-03 11:30:07.000000 demessaging-0.5.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:30:35.799021 demessaging-0.5.4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     6971 2024-06-03 11:30:07.000000 demessaging-0.5.4/tests/test_backend_class_.py
+-rw-rw-rw-   0 root         (0) root         (0)    11385 2024-06-03 11:30:07.000000 demessaging-0.5.4/tests/test_backend_function.py
+-rw-rw-rw-   0 root         (0) root         (0)    17479 2024-06-03 11:30:07.000000 demessaging-0.5.4/tests/test_backend_module.py
+-rw-rw-rw-   0 root         (0) root         (0)     3533 2024-06-03 11:30:07.000000 demessaging-0.5.4/tests/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2233 2024-06-03 11:30:07.000000 demessaging-0.5.4/tests/test_logging.py
```

### Comparing `demessaging-0.5.3/LICENSES/Apache-2.0.txt` & `demessaging-0.5.4/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.3/LICENSES/CC-BY-4.0.txt` & `demessaging-0.5.4/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.3/LICENSES/CC0-1.0.txt` & `demessaging-0.5.4/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.3/PKG-INFO` & `demessaging-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: demessaging
-Version: 0.5.3
+Version: 0.5.4
 Summary: python module wrapper for the data analytics software framework DASF
 Author: Mike Sips, Doris Dransch
 Author-email: Daniel Eggert <daniel.eggert@gfz-potsdam.de>, "Philipp S. Sommer" <philipp.sommer@hereon.de>
 Maintainer-email: "Philipp S. Sommer" <philipp.sommer@hereon.de>
 License: Apache-2.0
 Project-URL: Homepage, https://codebase.helmholtz.cloud/dasf/dasf-messaging-python
 Project-URL: Documentation, https://dasf.readthedocs.io/en/latest/
```

### Comparing `demessaging-0.5.3/README.md` & `demessaging-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.3/demessaging/NetCDFDecoder.py` & `demessaging-0.5.4/demessaging/NetCDFDecoder.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.3/demessaging/PulsarConnection.py` & `demessaging-0.5.4/demessaging/PulsarConnection.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.3/demessaging/PulsarMessageConstants.py` & `demessaging-0.5.4/demessaging/PulsarMessageConstants.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.3/demessaging/PulsarMessageConsumer.py` & `demessaging-0.5.4/demessaging/PulsarMessageConsumer.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.3/demessaging/PulsarMessageProducer.py` & `demessaging-0.5.4/demessaging/PulsarMessageProducer.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.3/demessaging/__init__.py` & `demessaging-0.5.4/demessaging/__init__.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.3/demessaging/backend/__init__.py` & `demessaging-0.5.4/demessaging/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.3/demessaging/backend/class_.py` & `demessaging-0.5.4/demessaging/backend/class_.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,28 +249,33 @@
 
         fields["function"] = (
             function_types,
             Field(description="The method to call."),
         )
         kwargs.update(fields)
 
+        desc = utils.get_desc(docstring_parser.parse(Class.__doc__))
+
         Model: Type[BackendClass] = create_model(  # type: ignore
             class_name,
             __validators__=config.validators,
             __module__=Class.__module__,
             __base__=cls,
             **kwargs,  # type: ignore
         )
 
         Model.backend_config = config
 
         config.Class = Class
         config.update_from_cls()
 
-        Model.__doc__ = config.doc
+        if desc:
+            Model.__doc__ = desc
+        else:
+            Model.__doc__ = ""
 
         return Model
 
     @classmethod
     def _get_constructor_model(cls) -> BaseModel:
         """A convenience method to create a pydantic model for __init__."""
         fields, _ = cls.get_constructor_fields(
@@ -278,14 +283,15 @@
             ClassConfig(
                 **cls.backend_config.model_dump(
                     exclude={"Class", "models", "class_name"}
                 )
             ),
             cls.backend_config.class_name,
         )
+        fields["__doc__"] = cls.__doc__
         return create_model(
             cls.backend_config.class_name,
             __module__=cls.backend_config.Class.__module__,
             **fields,
         )
 
     @classmethod
```

### Comparing `demessaging-0.5.3/demessaging/backend/function.py` & `demessaging-0.5.4/demessaging/backend/function.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.3/demessaging/backend/module.py` & `demessaging-0.5.4/demessaging/backend/module.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.3/demessaging/backend/utils.py` & `demessaging-0.5.4/demessaging/backend/utils.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.3/demessaging/cli.py` & `demessaging-0.5.4/demessaging/cli.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.3/demessaging/config/__init__.py` & `demessaging-0.5.4/demessaging/config/__init__.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.3/demessaging/config/api.py` & `demessaging-0.5.4/demessaging/config/api.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.3/demessaging/config/backend.py` & `demessaging-0.5.4/demessaging/config/backend.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.3/demessaging/config/logging.py` & `demessaging-0.5.4/demessaging/config/logging.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.3/demessaging/config/logging.yaml` & `demessaging-0.5.4/demessaging/config/logging.yaml`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.3/demessaging/config/messaging.py` & `demessaging-0.5.4/demessaging/config/messaging.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.3/demessaging/config/registry.py` & `demessaging-0.5.4/demessaging/config/registry.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.3/demessaging/messaging/connection.py` & `demessaging-0.5.4/demessaging/messaging/connection.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.3/demessaging/messaging/constants.py` & `demessaging-0.5.4/demessaging/messaging/constants.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.3/demessaging/messaging/consumer.py` & `demessaging-0.5.4/demessaging/messaging/consumer.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.3/demessaging/messaging/producer.py` & `demessaging-0.5.4/demessaging/messaging/producer.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.3/demessaging/serializers/xarray.py` & `demessaging-0.5.4/demessaging/serializers/xarray.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.3/demessaging/template.py` & `demessaging-0.5.4/demessaging/template.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.3/demessaging/templates/class_.py.jinja2` & `demessaging-0.5.4/demessaging/templates/class_.py.jinja2`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.3/demessaging/templates/function.py.jinja2` & `demessaging-0.5.4/demessaging/templates/function.py.jinja2`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.3/demessaging/templates/module.py.jinja2` & `demessaging-0.5.4/demessaging/templates/module.py.jinja2`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.3/demessaging/utils.py` & `demessaging-0.5.4/demessaging/utils.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.3/demessaging/validators/xarray.py` & `demessaging-0.5.4/demessaging/validators/xarray.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.3/demessaging.egg-info/PKG-INFO` & `demessaging-0.5.4/demessaging.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: demessaging
-Version: 0.5.3
+Version: 0.5.4
 Summary: python module wrapper for the data analytics software framework DASF
 Author: Mike Sips, Doris Dransch
 Author-email: Daniel Eggert <daniel.eggert@gfz-potsdam.de>, "Philipp S. Sommer" <philipp.sommer@hereon.de>
 Maintainer-email: "Philipp S. Sommer" <philipp.sommer@hereon.de>
 License: Apache-2.0
 Project-URL: Homepage, https://codebase.helmholtz.cloud/dasf/dasf-messaging-python
 Project-URL: Documentation, https://dasf.readthedocs.io/en/latest/
```

### Comparing `demessaging-0.5.3/demessaging.egg-info/SOURCES.txt` & `demessaging-0.5.4/demessaging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.3/demessaging.egg-info/requires.txt` & `demessaging-0.5.4/demessaging.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.3/pyproject.toml` & `demessaging-0.5.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.3/tests/test_backend_class_.py` & `demessaging-0.5.4/tests/test_backend_class_.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.3/tests/test_backend_function.py` & `demessaging-0.5.4/tests/test_backend_function.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.3/tests/test_backend_module.py` & `demessaging-0.5.4/tests/test_backend_module.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.3/tests/test_config.py` & `demessaging-0.5.4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.3/tests/test_logging.py` & `demessaging-0.5.4/tests/test_logging.py`

 * *Files identical despite different names*

