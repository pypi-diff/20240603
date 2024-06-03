# Comparing `tmp/crc_bonfire-5.8.1.tar.gz` & `tmp/crc_bonfire-5.8.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crc_bonfire-5.8.1.tar", last modified: Mon Jun  3 08:55:16 2024, max compression
+gzip compressed data, was "crc_bonfire-5.8.1b0.tar", last modified: Fri May 31 18:34:34 2024, max compression
```

## Comparing `crc_bonfire-5.8.1.tar` & `crc_bonfire-5.8.1b0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:55:16.294653 crc_bonfire-5.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-06-03 08:55:04.000000 crc_bonfire-5.8.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:55:16.282653 crc_bonfire-5.8.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:55:16.286653 crc_bonfire-5.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-06-03 08:55:04.000000 crc_bonfire-5.8.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-06-03 08:55:04.000000 crc_bonfire-5.8.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-06-03 08:55:04.000000 crc_bonfire-5.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-06-03 08:55:04.000000 crc_bonfire-5.8.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-06-03 08:55:04.000000 crc_bonfire-5.8.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-06-03 08:55:04.000000 crc_bonfire-5.8.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    22901 2024-06-03 08:55:16.294653 crc_bonfire-5.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21627 2024-06-03 08:55:04.000000 crc_bonfire-5.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:55:16.290653 crc_bonfire-5.8.1/bonfire/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 08:55:04.000000 crc_bonfire-5.8.1/bonfire/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    48968 2024-06-03 08:55:04.000000 crc_bonfire-5.8.1/bonfire/bonfire.py
--rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-06-03 08:55:04.000000 crc_bonfire-5.8.1/bonfire/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-06-03 08:55:04.000000 crc_bonfire-5.8.1/bonfire/configmaps.py
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-06-03 08:55:04.000000 crc_bonfire-5.8.1/bonfire/elastic_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-06-03 08:55:04.000000 crc_bonfire-5.8.1/bonfire/local.py
--rw-r--r--   0 runner    (1001) docker     (127)    14373 2024-06-03 08:55:04.000000 crc_bonfire-5.8.1/bonfire/namespaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    11706 2024-06-03 08:55:04.000000 crc_bonfire-5.8.1/bonfire/openshift.py
--rw-r--r--   0 runner    (1001) docker     (127)    29373 2024-06-03 08:55:04.000000 crc_bonfire-5.8.1/bonfire/processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    13861 2024-06-03 08:55:04.000000 crc_bonfire-5.8.1/bonfire/qontract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:55:16.290653 crc_bonfire-5.8.1/bonfire/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-06-03 08:55:04.000000 crc_bonfire-5.8.1/bonfire/resources/default-iqe-cji.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-06-03 08:55:04.000000 crc_bonfire-5.8.1/bonfire/resources/default_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-06-03 08:55:04.000000 crc_bonfire-5.8.1/bonfire/resources/ephemeral-cluster-clowdenvironment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-06-03 08:55:04.000000 crc_bonfire-5.8.1/bonfire/resources/local-cluster-clowdenvironment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-06-03 08:55:04.000000 crc_bonfire-5.8.1/bonfire/resources/reservation-template.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-06-03 08:55:04.000000 crc_bonfire-5.8.1/bonfire/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)    23110 2024-06-03 08:55:04.000000 crc_bonfire-5.8.1/bonfire/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      425 2024-06-03 08:55:04.000000 crc_bonfire-5.8.1/build_deploy.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:55:16.290653 crc_bonfire-5.8.1/cicd/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-06-03 08:55:04.000000 crc_bonfire-5.8.1/cicd/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-06-03 08:55:04.000000 crc_bonfire-5.8.1/cicd/bootstrap.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:55:16.294653 crc_bonfire-5.8.1/crc_bonfire.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22901 2024-06-03 08:55:16.000000 crc_bonfire-5.8.1/crc_bonfire.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-06-03 08:55:16.000000 crc_bonfire-5.8.1/crc_bonfire.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 08:55:16.000000 crc_bonfire-5.8.1/crc_bonfire.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-03 08:55:16.000000 crc_bonfire-5.8.1/crc_bonfire.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-06-03 08:55:16.000000 crc_bonfire-5.8.1/crc_bonfire.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-03 08:55:16.000000 crc_bonfire-5.8.1/crc_bonfire.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)  2975380 2024-06-03 08:55:04.000000 crc_bonfire-5.8.1/demo.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      589 2024-06-03 08:55:04.000000 crc_bonfire-5.8.1/entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-06-03 08:55:04.000000 crc_bonfire-5.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 08:55:04.000000 crc_bonfire-5.8.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 08:55:16.294653 crc_bonfire-5.8.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:55:16.294653 crc_bonfire-5.8.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:55:16.294653 crc_bonfire-5.8.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-06-03 08:55:04.000000 crc_bonfire-5.8.1/tests/data/namespace_data.json
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-06-03 08:55:04.000000 crc_bonfire-5.8.1/tests/data/reservation_data.json
--rw-r--r--   0 runner    (1001) docker     (127)    16188 2024-06-03 08:55:04.000000 crc_bonfire-5.8.1/tests/test_app_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14891 2024-06-03 08:55:04.000000 crc_bonfire-5.8.1/tests/test_bonfire.py
--rw-r--r--   0 runner    (1001) docker     (127)    10233 2024-06-03 08:55:04.000000 crc_bonfire-5.8.1/tests/test_get_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    19216 2024-06-03 08:55:04.000000 crc_bonfire-5.8.1/tests/test_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-06-03 08:55:04.000000 crc_bonfire-5.8.1/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:55:16.294653 crc_bonfire-5.8.1/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-06-03 08:55:04.000000 crc_bonfire-5.8.1/utils/search_replace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:34:34.197313 crc_bonfire-5.8.1b0/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:34:34.185313 crc_bonfire-5.8.1b0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:34:34.193313 crc_bonfire-5.8.1b0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    22903 2024-05-31 18:34:34.197313 crc_bonfire-5.8.1b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21627 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:34:34.193313 crc_bonfire-5.8.1b0/bonfire/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/bonfire/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    48968 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/bonfire/bonfire.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/bonfire/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/bonfire/configmaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/bonfire/elastic_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/bonfire/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14373 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/bonfire/namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11706 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/bonfire/openshift.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29373 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/bonfire/processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13861 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/bonfire/qontract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:34:34.193313 crc_bonfire-5.8.1b0/bonfire/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/bonfire/resources/default-iqe-cji.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/bonfire/resources/default_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/bonfire/resources/ephemeral-cluster-clowdenvironment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/bonfire/resources/local-cluster-clowdenvironment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/bonfire/resources/reservation-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/bonfire/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24573 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/bonfire/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      425 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/build_deploy.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:34:34.193313 crc_bonfire-5.8.1b0/cicd/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/cicd/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/cicd/bootstrap.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:34:34.197313 crc_bonfire-5.8.1b0/crc_bonfire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22903 2024-05-31 18:34:34.000000 crc_bonfire-5.8.1b0/crc_bonfire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-31 18:34:34.000000 crc_bonfire-5.8.1b0/crc_bonfire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 18:34:34.000000 crc_bonfire-5.8.1b0/crc_bonfire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-31 18:34:34.000000 crc_bonfire-5.8.1b0/crc_bonfire.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-31 18:34:34.000000 crc_bonfire-5.8.1b0/crc_bonfire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-31 18:34:34.000000 crc_bonfire-5.8.1b0/crc_bonfire.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  2975380 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/demo.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      589 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 18:34:34.197313 crc_bonfire-5.8.1b0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:34:34.197313 crc_bonfire-5.8.1b0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:34:34.197313 crc_bonfire-5.8.1b0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/tests/data/namespace_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/tests/data/reservation_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16188 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/tests/test_app_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14891 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/tests/test_bonfire.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10233 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/tests/test_get_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19216 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/tests/test_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:34:34.197313 crc_bonfire-5.8.1b0/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-31 18:34:20.000000 crc_bonfire-5.8.1b0/utils/search_replace.py
```

### Comparing `crc_bonfire-5.8.1/.github/workflows/release.yml` & `crc_bonfire-5.8.1b0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.1/.github/workflows/tests.yml` & `crc_bonfire-5.8.1b0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.1/.gitignore` & `crc_bonfire-5.8.1b0/.gitignore`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.1/CONTRIBUTING.md` & `crc_bonfire-5.8.1b0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.1/Dockerfile` & `crc_bonfire-5.8.1b0/Dockerfile`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.1/PKG-INFO` & `crc_bonfire-5.8.1b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crc-bonfire
-Version: 5.8.1
+Version: 5.8.1b0
 Summary: A CLI tool used to deploy ephemeral environments for testing cloud.redhat.com applications
 Author-email: Brandon Squizzato <bsquizza@redhat.com>
 License: MIT License
 Project-URL: Homepage, https://www.github.com/RedHatInsights/bonfire
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `crc_bonfire-5.8.1/README.md` & `crc_bonfire-5.8.1b0/README.md`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.1/bonfire/bonfire.py` & `crc_bonfire-5.8.1b0/bonfire/bonfire.py`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.1/bonfire/config.py` & `crc_bonfire-5.8.1b0/bonfire/config.py`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.1/bonfire/configmaps.py` & `crc_bonfire-5.8.1b0/bonfire/configmaps.py`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.1/bonfire/elastic_logging.py` & `crc_bonfire-5.8.1b0/bonfire/elastic_logging.py`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.1/bonfire/local.py` & `crc_bonfire-5.8.1b0/bonfire/local.py`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.1/bonfire/namespaces.py` & `crc_bonfire-5.8.1b0/bonfire/namespaces.py`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.1/bonfire/openshift.py` & `crc_bonfire-5.8.1b0/bonfire/openshift.py`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.1/bonfire/processor.py` & `crc_bonfire-5.8.1b0/bonfire/processor.py`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.1/bonfire/qontract.py` & `crc_bonfire-5.8.1b0/bonfire/qontract.py`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.1/bonfire/resources/default-iqe-cji.yaml` & `crc_bonfire-5.8.1b0/bonfire/resources/default-iqe-cji.yaml`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.1/bonfire/resources/default_config.yaml` & `crc_bonfire-5.8.1b0/bonfire/resources/default_config.yaml`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.1/bonfire/resources/ephemeral-cluster-clowdenvironment.yaml` & `crc_bonfire-5.8.1b0/bonfire/resources/ephemeral-cluster-clowdenvironment.yaml`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.1/bonfire/resources/local-cluster-clowdenvironment.yaml` & `crc_bonfire-5.8.1b0/bonfire/resources/local-cluster-clowdenvironment.yaml`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.1/bonfire/secrets.py` & `crc_bonfire-5.8.1b0/bonfire/secrets.py`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.1/bonfire/utils.py` & `crc_bonfire-5.8.1b0/bonfire/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 import os
 import re
 import shlex
 import socket
 import subprocess
 import tempfile
 import time
-from urllib.request import urlretrieve
-
 from distutils.version import StrictVersion
 from pathlib import Path
 from urllib.parse import urlparse
 
 from typing import List
 
 import sys
@@ -61,15 +59,41 @@
 GL_PROJECTS_URL = "https://gitlab.cee.redhat.com/api/v4/{type}/{group}/projects?search={name}"
 GL_BRANCH_URL = "https://gitlab.cee.redhat.com/api/v4/projects/{id}/repository/branches/{branch}"
 SYNTAX_ERR = "configuration syntax error"
 
 
 GIT_SHA_RE = re.compile(r"[a-f0-9]{40}")
 
-GL_CA_CERT_URL = "https://certs.corp.redhat.com/certs/2022-IT-Root-CA.pem"
+GL_CA_CERT = """
+-----BEGIN CERTIFICATE-----
+MIIENDCCAxygAwIBAgIJANunI0D662cnMA0GCSqGSIb3DQEBCwUAMIGlMQswCQYD
+VQQGEwJVUzEXMBUGA1UECAwOTm9ydGggQ2Fyb2xpbmExEDAOBgNVBAcMB1JhbGVp
+Z2gxFjAUBgNVBAoMDVJlZCBIYXQsIEluYy4xEzARBgNVBAsMClJlZCBIYXQgSVQx
+GzAZBgNVBAMMElJlZCBIYXQgSVQgUm9vdCBDQTEhMB8GCSqGSIb3DQEJARYSaW5m
+b3NlY0ByZWRoYXQuY29tMCAXDTE1MDcwNjE3MzgxMVoYDzIwNTUwNjI2MTczODEx
+WjCBpTELMAkGA1UEBhMCVVMxFzAVBgNVBAgMDk5vcnRoIENhcm9saW5hMRAwDgYD
+VQQHDAdSYWxlaWdoMRYwFAYDVQQKDA1SZWQgSGF0LCBJbmMuMRMwEQYDVQQLDApS
+ZWQgSGF0IElUMRswGQYDVQQDDBJSZWQgSGF0IElUIFJvb3QgQ0ExITAfBgkqhkiG
+9w0BCQEWEmluZm9zZWNAcmVkaGF0LmNvbTCCASIwDQYJKoZIhvcNAQEBBQADggEP
+ADCCAQoCggEBALQt9OJQh6GC5LT1g80qNh0u50BQ4sZ/yZ8aETxt+5lnPVX6MHKz
+bfwI6nO1aMG6j9bSw+6UUyPBHP796+FT/pTS+K0wsDV7c9XvHoxJBJJU38cdLkI2
+c/i7lDqTfTcfLL2nyUBd2fQDk1B0fxrskhGIIZ3ifP1Ps4ltTkv8hRSob3VtNqSo
+GxkKfvD2PKjTPxDPWYyruy9irLZioMffi3i/gCut0ZWtAyO3MVH5qWF/enKwgPES
+X9po+TdCvRB/RUObBaM761EcrLSM1GqHNueSfqnho3AjLQ6dBnPWlo638Zm1VebK
+BELyhkLWMSFkKwDmne0jQ02Y4g075vCKvCsCAwEAAaNjMGEwHQYDVR0OBBYEFH7R
+4yC+UehIIPeuL8Zqw3PzbgcZMB8GA1UdIwQYMBaAFH7R4yC+UehIIPeuL8Zqw3Pz
+bgcZMA8GA1UdEwEB/wQFMAMBAf8wDgYDVR0PAQH/BAQDAgGGMA0GCSqGSIb3DQEB
+CwUAA4IBAQBDNvD2Vm9sA5A9AlOJR8+en5Xz9hXcxJB5phxcZQ8jFoG04Vshvd0e
+LEnUrMcfFgIZ4njMKTQCM4ZFUPAieyLx4f52HuDopp3e5JyIMfW+KFcNIpKwCsak
+oSoKtIUOsUJK7qBVZxcrIyeQV2qcYOeZhtS5wBqIwOAhFwlCET7Ze58QHmS48slj
+S9K0JAcps2xdnGu0fkzhSQxY8GPQNFTlr6rYld5+ID/hHeS76gq0YG3q6RLWRkHf
+4eTkRjivAlExrFzKcljC4axKQlnOvVAzz+Gm32U0xPBF4ByePVxCJUHw1TsyTmel
+RxNEp7yHoXcwn+fXna+t5JWh1gxUZty3
+-----END CERTIFICATE-----
+"""
 
 _RATE_LIMIT_ERR_MSG = (
     "rate limited by GitHub, set GITHUB_TOKEN env var and/or use GITHUB_API_URL "
     "to point to a mirror"
 )
 
 _PARAM_REGEX = re.compile(r"\${(\S+)}")
@@ -203,18 +227,20 @@
         self._session.close()
 
         return result
 
     @cached_property
     def _gl_certfile(self):
         with tempfile.NamedTemporaryFile(delete=False) as fp:
-            urlretrieve(GL_CA_CERT_URL, fp.name)
+            cert_fname = fp.name
+            fp.write(GL_CA_CERT.encode("ascii"))
+
+        atexit.register(os.unlink, cert_fname)
 
-        atexit.register(os.unlink, fp.name)
-        return fp.name
+        return cert_fname
 
     @cached_property
     def _gh_auth_headers(self):
         log_msg = f"using GITHUB_API_URL '{GH_API_URL}' with no authorization"
         headers = None
 
         gh_token = os.getenv("GITHUB_TOKEN")
```

### Comparing `crc_bonfire-5.8.1/cicd/README.md` & `crc_bonfire-5.8.1b0/cicd/README.md`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.1/crc_bonfire.egg-info/PKG-INFO` & `crc_bonfire-5.8.1b0/crc_bonfire.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crc-bonfire
-Version: 5.8.1
+Version: 5.8.1b0
 Summary: A CLI tool used to deploy ephemeral environments for testing cloud.redhat.com applications
 Author-email: Brandon Squizzato <bsquizza@redhat.com>
 License: MIT License
 Project-URL: Homepage, https://www.github.com/RedHatInsights/bonfire
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `crc_bonfire-5.8.1/crc_bonfire.egg-info/SOURCES.txt` & `crc_bonfire-5.8.1b0/crc_bonfire.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.1/demo.gif` & `crc_bonfire-5.8.1b0/demo.gif`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.1/entrypoint.sh` & `crc_bonfire-5.8.1b0/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.1/pyproject.toml` & `crc_bonfire-5.8.1b0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.1/tests/data/namespace_data.json` & `crc_bonfire-5.8.1b0/tests/data/namespace_data.json`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.1/tests/data/reservation_data.json` & `crc_bonfire-5.8.1b0/tests/data/reservation_data.json`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.1/tests/test_app_configs.py` & `crc_bonfire-5.8.1b0/tests/test_app_configs.py`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.1/tests/test_bonfire.py` & `crc_bonfire-5.8.1b0/tests/test_bonfire.py`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.1/tests/test_get_apps.py` & `crc_bonfire-5.8.1b0/tests/test_get_apps.py`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.1/tests/test_processor.py` & `crc_bonfire-5.8.1b0/tests/test_processor.py`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.1/tests/test_utils.py` & `crc_bonfire-5.8.1b0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.8.1/utils/search_replace.py` & `crc_bonfire-5.8.1b0/utils/search_replace.py`

 * *Files identical despite different names*

