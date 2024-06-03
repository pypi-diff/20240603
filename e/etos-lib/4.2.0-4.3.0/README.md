# Comparing `tmp/etos_lib-4.2.0.tar.gz` & `tmp/etos_lib-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etos_lib-4.2.0.tar", last modified: Mon Apr 29 05:41:50 2024, max compression
+gzip compressed data, was "etos_lib-4.3.0.tar", last modified: Mon Jun  3 08:50:45 2024, max compression
```

## Comparing `etos_lib-4.2.0.tar` & `etos_lib-4.3.0.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 05:41:50.337131 etos_lib-4.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-29 05:41:44.000000 etos_lib-4.2.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 05:41:50.325131 etos_lib-4.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 05:41:50.329131 etos_lib-4.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-04-29 05:41:44.000000 etos_lib-4.2.0/.github/workflows/build-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-29 05:41:44.000000 etos_lib-4.2.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-29 05:41:44.000000 etos_lib-4.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-29 05:41:44.000000 etos_lib-4.2.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-29 05:41:44.000000 etos_lib-4.2.0/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)    10850 2024-04-29 05:41:44.000000 etos_lib-4.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-29 05:41:50.337131 etos_lib-4.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-29 05:41:44.000000 etos_lib-4.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 05:41:50.329131 etos_lib-4.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7610 2024-04-29 05:41:44.000000 etos_lib-4.2.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 05:41:50.329131 etos_lib-4.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-29 05:41:44.000000 etos_lib-4.2.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-29 05:41:44.000000 etos_lib-4.2.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-29 05:41:44.000000 etos_lib-4.2.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9169 2024-04-29 05:41:44.000000 etos_lib-4.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-29 05:41:44.000000 etos_lib-4.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-29 05:41:44.000000 etos_lib-4.2.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-29 05:41:44.000000 etos_lib-4.2.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-29 05:41:44.000000 etos_lib-4.2.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-29 05:41:44.000000 etos_lib-4.2.0/pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-29 05:41:44.000000 etos_lib-4.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-29 05:41:50.341131 etos_lib-4.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-29 05:41:44.000000 etos_lib-4.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 05:41:50.325131 etos_lib-4.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 05:41:50.333131 etos_lib-4.2.0/src/etos_lib/
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-29 05:41:44.000000 etos_lib-4.2.0/src/etos_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 05:41:50.333131 etos_lib-4.2.0/src/etos_lib/eiffel/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-29 05:41:44.000000 etos_lib-4.2.0/src/etos_lib/eiffel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-04-29 05:41:44.000000 etos_lib-4.2.0/src/etos_lib/eiffel/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-04-29 05:41:44.000000 etos_lib-4.2.0/src/etos_lib/eiffel/publisher.py
--rw-r--r--   0 runner    (1001) docker     (127)     6754 2024-04-29 05:41:44.000000 etos_lib-4.2.0/src/etos_lib/eiffel/subscriber.py
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-04-29 05:41:44.000000 etos_lib-4.2.0/src/etos_lib/etos.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 05:41:50.333131 etos_lib-4.2.0/src/etos_lib/graphql/
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-29 05:41:44.000000 etos_lib-4.2.0/src/etos_lib/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-29 05:41:44.000000 etos_lib-4.2.0/src/etos_lib/graphql/query_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 05:41:50.333131 etos_lib-4.2.0/src/etos_lib/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-29 05:41:44.000000 etos_lib-4.2.0/src/etos_lib/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-04-29 05:41:44.000000 etos_lib-4.2.0/src/etos_lib/kubernetes/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-29 05:41:44.000000 etos_lib-4.2.0/src/etos_lib/kubernetes/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 05:41:50.337131 etos_lib-4.2.0/src/etos_lib/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-29 05:41:44.000000 etos_lib-4.2.0/src/etos_lib/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-04-29 05:41:44.000000 etos_lib-4.2.0/src/etos_lib/lib/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-29 05:41:44.000000 etos_lib-4.2.0/src/etos_lib/lib/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-04-29 05:41:44.000000 etos_lib-4.2.0/src/etos_lib/lib/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)    15797 2024-04-29 05:41:44.000000 etos_lib-4.2.0/src/etos_lib/lib/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-29 05:41:44.000000 etos_lib-4.2.0/src/etos_lib/lib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-29 05:41:44.000000 etos_lib-4.2.0/src/etos_lib/lib/feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-29 05:41:44.000000 etos_lib-4.2.0/src/etos_lib/lib/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-04-29 05:41:44.000000 etos_lib-4.2.0/src/etos_lib/lib/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10922 2024-04-29 05:41:44.000000 etos_lib-4.2.0/src/etos_lib/lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 05:41:50.337131 etos_lib-4.2.0/src/etos_lib/logging/
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-29 05:41:44.000000 etos_lib-4.2.0/src/etos_lib/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-29 05:41:44.000000 etos_lib-4.2.0/src/etos_lib/logging/default_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-29 05:41:44.000000 etos_lib-4.2.0/src/etos_lib/logging/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-04-29 05:41:44.000000 etos_lib-4.2.0/src/etos_lib/logging/formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-29 05:41:44.000000 etos_lib-4.2.0/src/etos_lib/logging/log_publisher.py
--rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-04-29 05:41:44.000000 etos_lib-4.2.0/src/etos_lib/logging/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-29 05:41:44.000000 etos_lib-4.2.0/src/etos_lib/logging/rabbitmq_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 05:41:50.337131 etos_lib-4.2.0/src/etos_lib/opentelemetry/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-29 05:41:44.000000 etos_lib-4.2.0/src/etos_lib/opentelemetry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-29 05:41:44.000000 etos_lib-4.2.0/src/etos_lib/opentelemetry/semconv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 05:41:50.337131 etos_lib-4.2.0/src/etos_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-29 05:41:50.000000 etos_lib-4.2.0/src/etos_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-29 05:41:50.000000 etos_lib-4.2.0/src/etos_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 05:41:50.000000 etos_lib-4.2.0/src/etos_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 05:41:50.000000 etos_lib-4.2.0/src/etos_lib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-29 05:41:50.000000 etos_lib-4.2.0/src/etos_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-29 05:41:50.000000 etos_lib-4.2.0/src/etos_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-29 05:41:44.000000 etos_lib-4.2.0/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 05:41:50.337131 etos_lib-4.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-29 05:41:44.000000 etos_lib-4.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-29 05:41:44.000000 etos_lib-4.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-29 05:41:44.000000 etos_lib-4.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:50:45.901200 etos_lib-4.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-06-03 08:50:40.000000 etos_lib-4.3.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:50:45.885200 etos_lib-4.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:50:45.889200 etos_lib-4.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-06-03 08:50:40.000000 etos_lib-4.3.0/.github/workflows/build-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-06-03 08:50:40.000000 etos_lib-4.3.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-06-03 08:50:40.000000 etos_lib-4.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-06-03 08:50:40.000000 etos_lib-4.3.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-06-03 08:50:40.000000 etos_lib-4.3.0/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)    10850 2024-06-03 08:50:40.000000 etos_lib-4.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-06-03 08:50:45.901200 etos_lib-4.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-06-03 08:50:40.000000 etos_lib-4.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:50:45.889200 etos_lib-4.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7610 2024-06-03 08:50:40.000000 etos_lib-4.3.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:50:45.889200 etos_lib-4.3.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-03 08:50:40.000000 etos_lib-4.3.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-03 08:50:40.000000 etos_lib-4.3.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-06-03 08:50:40.000000 etos_lib-4.3.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9169 2024-06-03 08:50:40.000000 etos_lib-4.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-06-03 08:50:40.000000 etos_lib-4.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-06-03 08:50:40.000000 etos_lib-4.3.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-06-03 08:50:40.000000 etos_lib-4.3.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-06-03 08:50:40.000000 etos_lib-4.3.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-03 08:50:40.000000 etos_lib-4.3.0/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-06-03 08:50:40.000000 etos_lib-4.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-06-03 08:50:45.901200 etos_lib-4.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-06-03 08:50:40.000000 etos_lib-4.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:50:45.885200 etos_lib-4.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:50:45.893200 etos_lib-4.3.0/src/etos_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-06-03 08:50:40.000000 etos_lib-4.3.0/src/etos_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:50:45.893200 etos_lib-4.3.0/src/etos_lib/eiffel/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-06-03 08:50:40.000000 etos_lib-4.3.0/src/etos_lib/eiffel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-06-03 08:50:40.000000 etos_lib-4.3.0/src/etos_lib/eiffel/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-06-03 08:50:40.000000 etos_lib-4.3.0/src/etos_lib/eiffel/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6754 2024-06-03 08:50:40.000000 etos_lib-4.3.0/src/etos_lib/eiffel/subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-06-03 08:50:40.000000 etos_lib-4.3.0/src/etos_lib/etos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:50:45.893200 etos_lib-4.3.0/src/etos_lib/graphql/
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-06-03 08:50:40.000000 etos_lib-4.3.0/src/etos_lib/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-06-03 08:50:40.000000 etos_lib-4.3.0/src/etos_lib/graphql/query_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:50:45.893200 etos_lib-4.3.0/src/etos_lib/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-06-03 08:50:40.000000 etos_lib-4.3.0/src/etos_lib/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-06-03 08:50:40.000000 etos_lib-4.3.0/src/etos_lib/kubernetes/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-06-03 08:50:40.000000 etos_lib-4.3.0/src/etos_lib/kubernetes/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:50:45.897200 etos_lib-4.3.0/src/etos_lib/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-06-03 08:50:40.000000 etos_lib-4.3.0/src/etos_lib/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-06-03 08:50:40.000000 etos_lib-4.3.0/src/etos_lib/lib/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-06-03 08:50:40.000000 etos_lib-4.3.0/src/etos_lib/lib/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-06-03 08:50:40.000000 etos_lib-4.3.0/src/etos_lib/lib/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15797 2024-06-03 08:50:40.000000 etos_lib-4.3.0/src/etos_lib/lib/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-06-03 08:50:40.000000 etos_lib-4.3.0/src/etos_lib/lib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-06-03 08:50:40.000000 etos_lib-4.3.0/src/etos_lib/lib/feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-06-03 08:50:40.000000 etos_lib-4.3.0/src/etos_lib/lib/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-06-03 08:50:40.000000 etos_lib-4.3.0/src/etos_lib/lib/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10922 2024-06-03 08:50:40.000000 etos_lib-4.3.0/src/etos_lib/lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:50:45.897200 etos_lib-4.3.0/src/etos_lib/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-06-03 08:50:40.000000 etos_lib-4.3.0/src/etos_lib/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-06-03 08:50:40.000000 etos_lib-4.3.0/src/etos_lib/logging/default_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-06-03 08:50:40.000000 etos_lib-4.3.0/src/etos_lib/logging/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-06-03 08:50:40.000000 etos_lib-4.3.0/src/etos_lib/logging/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-06-03 08:50:40.000000 etos_lib-4.3.0/src/etos_lib/logging/log_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-06-03 08:50:40.000000 etos_lib-4.3.0/src/etos_lib/logging/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-06-03 08:50:40.000000 etos_lib-4.3.0/src/etos_lib/logging/rabbitmq_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:50:45.897200 etos_lib-4.3.0/src/etos_lib/opentelemetry/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-06-03 08:50:40.000000 etos_lib-4.3.0/src/etos_lib/opentelemetry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-06-03 08:50:40.000000 etos_lib-4.3.0/src/etos_lib/opentelemetry/semconv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:50:45.897200 etos_lib-4.3.0/src/etos_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-06-03 08:50:45.000000 etos_lib-4.3.0/src/etos_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-06-03 08:50:45.000000 etos_lib-4.3.0/src/etos_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 08:50:45.000000 etos_lib-4.3.0/src/etos_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 08:50:45.000000 etos_lib-4.3.0/src/etos_lib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-06-03 08:50:45.000000 etos_lib-4.3.0/src/etos_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-03 08:50:45.000000 etos_lib-4.3.0/src/etos_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-06-03 08:50:40.000000 etos_lib-4.3.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:50:45.897200 etos_lib-4.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-06-03 08:50:40.000000 etos_lib-4.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-06-03 08:50:40.000000 etos_lib-4.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-06-03 08:50:40.000000 etos_lib-4.3.0/tox.ini
```

### Comparing `etos_lib-4.2.0/.coveragerc` & `etos_lib-4.3.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `etos_lib-4.2.0/.github/workflows/build-publish.yml` & `etos_lib-4.3.0/.github/workflows/build-publish.yml`

 * *Files identical despite different names*

### Comparing `etos_lib-4.2.0/.github/workflows/main.yml` & `etos_lib-4.3.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `etos_lib-4.2.0/.gitignore` & `etos_lib-4.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `etos_lib-4.2.0/LICENSE.txt` & `etos_lib-4.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `etos_lib-4.2.0/PKG-INFO` & `etos_lib-4.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etos_lib
-Version: 4.2.0
+Version: 4.3.0
 Summary: ETOS Library
 Home-page: https://github.com/eiffel-community/etos-library
 Author: Tobias Persson
 Author-email: tobias.persson@axis.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://etos.readthedocs.io/
 Platform: Linux
```

### Comparing `etos_lib-4.2.0/README.rst` & `etos_lib-4.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `etos_lib-4.2.0/docs/Makefile` & `etos_lib-4.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `etos_lib-4.2.0/docs/conf.py` & `etos_lib-4.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.2.0/setup.cfg` & `etos_lib-4.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `etos_lib-4.2.0/setup.py` & `etos_lib-4.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.2.0/src/etos_lib/__init__.py` & `etos_lib-4.3.0/src/etos_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.2.0/src/etos_lib/eiffel/__init__.py` & `etos_lib-4.3.0/src/etos_lib/eiffel/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.2.0/src/etos_lib/eiffel/common.py` & `etos_lib-4.3.0/src/etos_lib/eiffel/common.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.2.0/src/etos_lib/eiffel/publisher.py` & `etos_lib-4.3.0/src/etos_lib/eiffel/publisher.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.2.0/src/etos_lib/eiffel/subscriber.py` & `etos_lib-4.3.0/src/etos_lib/eiffel/subscriber.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.2.0/src/etos_lib/etos.py` & `etos_lib-4.3.0/src/etos_lib/etos.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.2.0/src/etos_lib/graphql/__init__.py` & `etos_lib-4.3.0/src/etos_lib/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.2.0/src/etos_lib/graphql/query_handler.py` & `etos_lib-4.3.0/src/etos_lib/graphql/query_handler.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.2.0/src/etos_lib/kubernetes/__init__.py` & `etos_lib-4.3.0/src/etos_lib/kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.2.0/src/etos_lib/kubernetes/base.py` & `etos_lib-4.3.0/src/etos_lib/kubernetes/base.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.2.0/src/etos_lib/kubernetes/jobs.py` & `etos_lib-4.3.0/src/etos_lib/kubernetes/jobs.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.2.0/src/etos_lib/lib/__init__.py` & `etos_lib-4.3.0/src/etos_lib/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.2.0/src/etos_lib/lib/config.py` & `etos_lib-4.3.0/src/etos_lib/lib/config.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.2.0/src/etos_lib/lib/database.py` & `etos_lib-4.3.0/src/etos_lib/lib/database.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.2.0/src/etos_lib/lib/debug.py` & `etos_lib-4.3.0/src/etos_lib/lib/debug.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.2.0/src/etos_lib/lib/events.py` & `etos_lib-4.3.0/src/etos_lib/lib/events.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.2.0/src/etos_lib/lib/exceptions.py` & `etos_lib-4.3.0/src/etos_lib/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.2.0/src/etos_lib/lib/feature_flags.py` & `etos_lib-4.3.0/src/etos_lib/lib/feature_flags.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.2.0/src/etos_lib/lib/http.py` & `etos_lib-4.3.0/src/etos_lib/lib/http.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.2.0/src/etos_lib/lib/monitor.py` & `etos_lib-4.3.0/src/etos_lib/lib/monitor.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.2.0/src/etos_lib/lib/utils.py` & `etos_lib-4.3.0/src/etos_lib/lib/utils.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.2.0/src/etos_lib/logging/__init__.py` & `etos_lib-4.3.0/src/etos_lib/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.2.0/src/etos_lib/logging/filter.py` & `etos_lib-4.3.0/src/etos_lib/logging/filter.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,28 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """ETOS filter."""
 import logging
 
+from opentelemetry import trace
+
+
+def get_current_otel_trace_id() -> str:
+    """Get current OpenTelemetry trace id.
+
+    The OpenTelemetry trace id is a big integer by default, which is out of range
+    of the type 'long' in Elastic. For this reason the trace id is returned as string.
+
+    If OpenTelemetry is not enabled, this function will return "0".
+    """
+    current_span = trace.get_current_span()
+    return str(current_span.get_span_context().trace_id)
+
 
 class EtosFilter(logging.Filter):  # pylint:disable=too-few-public-methods
     """Filter for adding extra application specific data to log messages."""
 
     def __init__(self, application, version, environment, local):
         """Initialize with a few ETOS application fields.
 
@@ -45,14 +59,15 @@
         :type record: :obj:`logging.LogRecord`
         :return: True
         :rtype: bool
         """
         record.application = self.application
         record.version = self.version
         record.environment = self.environment
+        record.opentelemetry_trace_id = get_current_otel_trace_id()
 
         # Add each thread-local attribute to record.
         for attr in dir(self.local):
             if attr.startswith("__") and attr.endswith("__"):
                 continue
             setattr(record, attr, getattr(self.local, attr))
         if not hasattr(record, "identifier"):
```

### Comparing `etos_lib-4.2.0/src/etos_lib/logging/formatter.py` & `etos_lib-4.3.0/src/etos_lib/logging/formatter.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.2.0/src/etos_lib/logging/log_publisher.py` & `etos_lib-4.3.0/src/etos_lib/logging/log_publisher.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.2.0/src/etos_lib/logging/logger.py` & `etos_lib-4.3.0/src/etos_lib/logging/logger.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.2.0/src/etos_lib/logging/rabbitmq_handler.py` & `etos_lib-4.3.0/src/etos_lib/logging/rabbitmq_handler.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.2.0/src/etos_lib/opentelemetry/__init__.py` & `etos_lib-4.3.0/src/etos_lib/opentelemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.2.0/src/etos_lib/opentelemetry/semconv.py` & `etos_lib-4.3.0/src/etos_lib/opentelemetry/semconv.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.2.0/src/etos_lib.egg-info/PKG-INFO` & `etos_lib-4.3.0/src/etos_lib.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etos_lib
-Version: 4.2.0
+Version: 4.3.0
 Summary: ETOS Library
 Home-page: https://github.com/eiffel-community/etos-library
 Author: Tobias Persson
 Author-email: tobias.persson@axis.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://etos.readthedocs.io/
 Platform: Linux
```

### Comparing `etos_lib-4.2.0/src/etos_lib.egg-info/SOURCES.txt` & `etos_lib-4.3.0/src/etos_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `etos_lib-4.2.0/tests/__init__.py` & `etos_lib-4.3.0/tests/__init__.py`

 * *Files identical despite different names*

