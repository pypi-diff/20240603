# Comparing `tmp/flask_unleash-2.0.0.tar.gz` & `tmp/flask_unleash-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flask_unleash-2.0.0.tar", last modified: Mon Jan  3 17:17:34 2022, max compression
+gzip compressed data, was "dist/flask_unleash-2.1.0.tar", last modified: Mon Jun  3 09:36:37 2024, max compression
```

## Comparing `flask_unleash-2.0.0.tar` & `flask_unleash-2.1.0.tar`

### file list

```diff
@@ -1,36 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 17:17:34.000000 flask_unleash-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-01-03 17:17:00.000000 flask_unleash-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4453 2022-01-03 17:17:34.000000 flask_unleash-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3351 2022-01-03 17:17:00.000000 flask_unleash-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 17:17:34.000000 flask_unleash-2.0.0/demo_app/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-03 17:17:00.000000 flask_unleash-2.0.0/demo_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      632 2022-01-03 17:17:00.000000 flask_unleash-2.0.0/demo_app/app.py
--rw-r--r--   0 runner    (1001) docker     (121)      393 2022-01-03 17:17:00.000000 flask_unleash-2.0.0/demo_app/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 17:17:34.000000 flask_unleash-2.0.0/demo_app/extensions/
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-01-03 17:17:00.000000 flask_unleash-2.0.0/demo_app/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 17:17:34.000000 flask_unleash-2.0.0/demo_app/extensions/logging/
--rw-r--r--   0 runner    (1001) docker     (121)      787 2022-01-03 17:17:00.000000 flask_unleash-2.0.0/demo_app/extensions/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 17:17:34.000000 flask_unleash-2.0.0/demo_app/extensions/unleash/
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-01-03 17:17:00.000000 flask_unleash-2.0.0/demo_app/extensions/unleash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-01-03 17:17:00.000000 flask_unleash-2.0.0/demo_app/gunicorn.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 17:17:34.000000 flask_unleash-2.0.0/demo_app/modules/
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-01-03 17:17:00.000000 flask_unleash-2.0.0/demo_app/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 17:17:34.000000 flask_unleash-2.0.0/demo_app/modules/check/
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-01-03 17:17:00.000000 flask_unleash-2.0.0/demo_app/modules/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      649 2022-01-03 17:17:00.000000 flask_unleash-2.0.0/demo_app/modules/check/resources.py
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-01-03 17:17:00.000000 flask_unleash-2.0.0/demo_app/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 17:17:34.000000 flask_unleash-2.0.0/flask_unleash/
--rw-r--r--   0 runner    (1001) docker     (121)     1749 2022-01-03 17:17:00.000000 flask_unleash-2.0.0/flask_unleash/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 17:17:34.000000 flask_unleash-2.0.0/flask_unleash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4453 2022-01-03 17:17:34.000000 flask_unleash-2.0.0/flask_unleash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      643 2022-01-03 17:17:34.000000 flask_unleash-2.0.0/flask_unleash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-03 17:17:34.000000 flask_unleash-2.0.0/flask_unleash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-03 17:17:34.000000 flask_unleash-2.0.0/flask_unleash.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-01-03 17:17:34.000000 flask_unleash-2.0.0/flask_unleash.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-01-03 17:17:34.000000 flask_unleash-2.0.0/flask_unleash.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-03 17:17:34.000000 flask_unleash-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      966 2022-01-03 17:17:00.000000 flask_unleash-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 17:17:34.000000 flask_unleash-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-03 17:17:00.000000 flask_unleash-2.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-01-03 17:17:00.000000 flask_unleash-2.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-01-03 17:17:00.000000 flask_unleash-2.0.0/tests/test_helloworld.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:36:37.000000 flask_unleash-2.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:36:37.000000 flask_unleash-2.1.0/.circleci-archive/
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/.circleci-archive/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:36:37.000000 flask_unleash-2.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:36:37.000000 flask_unleash-2.1.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/.github/stale.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:36:37.000000 flask_unleash-2.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/.github/workflows/add-to-project.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/.github/workflows/pull_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/.github/workflows/release-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/.github/workflows/release-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-06-03 09:36:37.000000 flask_unleash-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:36:37.000000 flask_unleash-2.1.0/demo_app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/demo_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/demo_app/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/demo_app/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:36:37.000000 flask_unleash-2.1.0/demo_app/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/demo_app/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:36:37.000000 flask_unleash-2.1.0/demo_app/extensions/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/demo_app/extensions/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:36:37.000000 flask_unleash-2.1.0/demo_app/extensions/unleash/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/demo_app/extensions/unleash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/demo_app/gunicorn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:36:37.000000 flask_unleash-2.1.0/demo_app/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/demo_app/helpers/requestid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:36:37.000000 flask_unleash-2.1.0/demo_app/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/demo_app/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:36:37.000000 flask_unleash-2.1.0/demo_app/modules/check/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/demo_app/modules/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/demo_app/modules/check/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/demo_app/test.http
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/demo_app/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:36:37.000000 flask_unleash-2.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/docs/config.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/docs/development.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:36:37.000000 flask_unleash-2.1.0/flask_unleash/
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/flask_unleash/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:36:37.000000 flask_unleash-2.1.0/flask_unleash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-06-03 09:36:37.000000 flask_unleash-2.1.0/flask_unleash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-06-03 09:36:37.000000 flask_unleash-2.1.0/flask_unleash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 09:36:37.000000 flask_unleash-2.1.0/flask_unleash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 09:36:37.000000 flask_unleash-2.1.0/flask_unleash.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-06-03 09:36:37.000000 flask_unleash-2.1.0/flask_unleash.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-06-03 09:36:37.000000 flask_unleash-2.1.0/flask_unleash.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 09:36:37.000000 flask_unleash-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:36:37.000000 flask_unleash-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/tests/test_helloworld.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-06-03 09:35:44.000000 flask_unleash-2.1.0/tox.ini
```

### Comparing `flask_unleash-2.0.0/PKG-INFO` & `flask_unleash-2.1.0/flask_unleash.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
-Name: flask_unleash
-Version: 2.0.0
+Name: flask-unleash
+Version: 2.1.0
 Summary: Flask extension for unleash-client-python.
 Home-page: https://github.com/Unleash/Flask-Unleash
 Author: Ivan Lee
 Author-email: ivanklee86@gmail.com
 License: MIT
 Description: # Flask-Unleash
         
         ![](https://github.com/unleash/flask-unleash/workflows/CI/badge.svg?branch=main) [![Coverage Status](https://coveralls.io/repos/github/Unleash/Flask-Unleash/badge.svg?branch=main)](https://coveralls.io/github/Unleash/Flask-Unleash?branch=main) [![PyPI version](https://badge.fury.io/py/flask-unleash.svg)](https://badge.fury.io/py/flask-unleash) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/flask_unleash) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
         
         Flask extension to make using Unleash that much easier! 🚦🚦🚦  This plugin makes integrating the [Python Unleash client](https://github.com/unleash/unleash-client-python) into quick and easy.
         
         * [Documentation](https://unleash.github.io/Flask-Unleash/)
-        * [Changelog](https://github.com/Unleash/Flask-Unleash/blob/main/docs/changelog.md)
+        * [Changelog](https://docs.getunleash.io/Flask-Unleash/changelog.html)
         
         ## Pre-requisites
         
         To try out Flask-Unleash, you'll need an instance of the [Unleash](http://github.com/unleash/unleash) server.  You can either use:
         * Spin up a stack in Docker Compose using [unleash-docker](https://github.com/Unleash/unleash-docker)
         * Check out the demo at [Unleash-Hosted](https://www.unleash-hosted.com/)
         
@@ -51,32 +51,19 @@
         flag_value_2 = unleash.client.is_enabled("complex-feature", context)
         ```
         
         Check out the [demo app](https://github.com/Unleash/Flask-Unleash/tree/main/demo_app) for a more real-life sample implementation.
         
         ## Configuring Flask-Unleash
         
-        The following configuration values exist for Flask-Unleash.
-        
-        Config | Description | Required? |  Type |  Default Value|
-        ---------|-------------|-----------|-------|---------------|
-        UNLEASH_URL | Unleash server URL | Y | String | N/A |
-        UNLEASH_APP_NAME | Name of your program | Y | String | N/A |
-        UNLEASH_ENVIRONMENT | Environment of your service | Y | String | N/A |
-        UNLEASH_INSTANCE_ID | Unique ID for your program | N | String | unleash-client-python | 
-        UNLEASH_REFRESH_INTERVAL | How often the unleash client should check for configuration changes. | N | Integer |  15 |
-        UNLEASH_METRIC_INTERVAL | How often the unleash client should send metrics to server. | N | Integer | 60 |
-        UNLEASH_DISABLE_METRICS | Disables sending metrics to Unleash server. | N | Boolean | F |
-        UNLEASH_DISABLE_REGISTRATION | Disables registration with Unleash server. | N | Boolean | F |
-        UNLEASH_CUSTOM_HEADERS | Custom headers to send to Unleash. | N | Dictionary | {}
-        UNLEASH_CUSTOM_OPTIONS | Custom arguments for requests package. | N | Dictionary | {}
-        UNLEASH_CUSTOM_STRATEGIES | Custom strategies you'd like UnleashClient to support. | N | Dictionary | {} |
-        UNLEASH_CACHE_DIRECTORY | Location of the cache directory. When unset, FCache will determine the location | N | Str | Unset |
+        See the [Flask-Unleash documentation](https://docs.getunleash.io/Flask-Unleash/) for information about configuring Unleash.
         
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
```

### Comparing `flask_unleash-2.0.0/demo_app/app.py` & `flask_unleash-2.1.0/demo_app/app.py`

 * *Files identical despite different names*

### Comparing `flask_unleash-2.0.0/demo_app/extensions/logging/__init__.py` & `flask_unleash-2.1.0/demo_app/extensions/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_unleash-2.0.0/demo_app/modules/check/resources.py` & `flask_unleash-2.1.0/demo_app/modules/check/resources.py`

 * *Files identical despite different names*

### Comparing `flask_unleash-2.0.0/flask_unleash/__init__.py` & `flask_unleash-2.1.0/flask_unleash/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+# pylint: disable=too-few-public-methods
 import os
 from UnleashClient import UnleashClient
-from flask import current_app, _app_ctx_stack  # type: ignore
+from flask import current_app  # type: ignore
 
 
 CONFIG_MAPPING = {
     'UNLEASH_INSTANCE_ID': 'instance_id',
     'UNLEASH_REFRESH_INTERVAL': 'refresh_interval',
     'UNLEASH_REFRESH_JITTER': 'refresh_jitter',
     'UNLEASH_METRIC_INTERVAL': 'metrics_interval',
@@ -17,25 +18,36 @@
     'UNLEASH_CACHE_DIRECTORY': 'cache_directory',
     'UNLEASH_PROJECT_NAME': 'project_name',
     'UNLEASH_VERBOSE_LOG_LEVEL': 'verbose_log_level'
 }
 
 
 class Unleash():
+    """
+    Unleash extension for Flask.
+
+    :param app: Flask app instance
+    """
     def __init__(self, app=None):
         # Constants
         self.name = 'unleash_client'
         self.client = None
 
         # Setup
         self.app = app
         if app is not None:
             self.init_app(app)
 
     def init_app(self, app):
+        """
+        Configures Unleash client instance, starts client, and makes it available for use via Flask.
+
+        :param app: Flask app instance
+        """
+
         # Populate required arguments.
         unleash_args = {
             'url': app.config['UNLEASH_URL'],
             'app_name': app.config['UNLEASH_APP_NAME'],
             'environment': app.config['UNLEASH_ENVIRONMENT']
         }
```

### Comparing `flask_unleash-2.0.0/flask_unleash.egg-info/PKG-INFO` & `flask_unleash-2.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
-Name: flask-unleash
-Version: 2.0.0
+Name: flask_unleash
+Version: 2.1.0
 Summary: Flask extension for unleash-client-python.
 Home-page: https://github.com/Unleash/Flask-Unleash
 Author: Ivan Lee
 Author-email: ivanklee86@gmail.com
 License: MIT
 Description: # Flask-Unleash
         
         ![](https://github.com/unleash/flask-unleash/workflows/CI/badge.svg?branch=main) [![Coverage Status](https://coveralls.io/repos/github/Unleash/Flask-Unleash/badge.svg?branch=main)](https://coveralls.io/github/Unleash/Flask-Unleash?branch=main) [![PyPI version](https://badge.fury.io/py/flask-unleash.svg)](https://badge.fury.io/py/flask-unleash) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/flask_unleash) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
         
         Flask extension to make using Unleash that much easier! 🚦🚦🚦  This plugin makes integrating the [Python Unleash client](https://github.com/unleash/unleash-client-python) into quick and easy.
         
         * [Documentation](https://unleash.github.io/Flask-Unleash/)
-        * [Changelog](https://github.com/Unleash/Flask-Unleash/blob/main/docs/changelog.md)
+        * [Changelog](https://docs.getunleash.io/Flask-Unleash/changelog.html)
         
         ## Pre-requisites
         
         To try out Flask-Unleash, you'll need an instance of the [Unleash](http://github.com/unleash/unleash) server.  You can either use:
         * Spin up a stack in Docker Compose using [unleash-docker](https://github.com/Unleash/unleash-docker)
         * Check out the demo at [Unleash-Hosted](https://www.unleash-hosted.com/)
         
@@ -51,32 +51,19 @@
         flag_value_2 = unleash.client.is_enabled("complex-feature", context)
         ```
         
         Check out the [demo app](https://github.com/Unleash/Flask-Unleash/tree/main/demo_app) for a more real-life sample implementation.
         
         ## Configuring Flask-Unleash
         
-        The following configuration values exist for Flask-Unleash.
-        
-        Config | Description | Required? |  Type |  Default Value|
-        ---------|-------------|-----------|-------|---------------|
-        UNLEASH_URL | Unleash server URL | Y | String | N/A |
-        UNLEASH_APP_NAME | Name of your program | Y | String | N/A |
-        UNLEASH_ENVIRONMENT | Environment of your service | Y | String | N/A |
-        UNLEASH_INSTANCE_ID | Unique ID for your program | N | String | unleash-client-python | 
-        UNLEASH_REFRESH_INTERVAL | How often the unleash client should check for configuration changes. | N | Integer |  15 |
-        UNLEASH_METRIC_INTERVAL | How often the unleash client should send metrics to server. | N | Integer | 60 |
-        UNLEASH_DISABLE_METRICS | Disables sending metrics to Unleash server. | N | Boolean | F |
-        UNLEASH_DISABLE_REGISTRATION | Disables registration with Unleash server. | N | Boolean | F |
-        UNLEASH_CUSTOM_HEADERS | Custom headers to send to Unleash. | N | Dictionary | {}
-        UNLEASH_CUSTOM_OPTIONS | Custom arguments for requests package. | N | Dictionary | {}
-        UNLEASH_CUSTOM_STRATEGIES | Custom strategies you'd like UnleashClient to support. | N | Dictionary | {} |
-        UNLEASH_CACHE_DIRECTORY | Location of the cache directory. When unset, FCache will determine the location | N | Str | Unset |
+        See the [Flask-Unleash documentation](https://docs.getunleash.io/Flask-Unleash/) for information about configuring Unleash.
         
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
```

### Comparing `flask_unleash-2.0.0/setup.py` & `flask_unleash-2.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 def readme():
     with open('README.md') as file:
         return file.read()
 
 
 setup(
     name='flask_unleash',
-    version='2.0.0',
     url='https://github.com/Unleash/Flask-Unleash',
     license='MIT',
     author='Ivan Lee',
     author_email='ivanklee86@gmail.com',
     description='Flask extension for unleash-client-python.',
     long_description=readme(),
     long_description_content_type="text/markdown",
@@ -20,17 +19,20 @@
     zip_safe=False,
     include_package_data=True,
     platforms='any',
     install_requires=[
         'UnleashClient',
         'Flask'
     ],
+    setup_requires=['setuptools_scm'],
     python_requres=">=3.6",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8"
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
     ]
 )
```

