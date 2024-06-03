# Comparing `tmp/etos_environment_provider-4.2.0.tar.gz` & `tmp/etos_environment_provider-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etos_environment_provider-4.2.0.tar", last modified: Thu May  2 11:00:02 2024, max compression
+gzip compressed data, was "etos_environment_provider-4.3.0.tar", last modified: Mon Jun  3 09:22:03 2024, max compression
```

## Comparing `etos_environment_provider-4.2.0.tar` & `etos_environment_provider-4.3.0.tar`

### file list

```diff
@@ -1,137 +1,136 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.783823 etos_environment_provider-4.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.759823 etos_environment_provider-4.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.767823 etos_environment_provider-4.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/.github/workflows/build-push.yml
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)    10850 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-02 11:00:02.783823 etos_environment_provider-4.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.767823 etos_environment_provider-4.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7634 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.767823 etos_environment_provider-4.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.763823 etos_environment_provider-4.2.0/manifests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.767823 etos_environment_provider-4.2.0/manifests/base/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.767823 etos_environment_provider-4.2.0/manifests/base/api/
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/manifests/base/api/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/manifests/base/api/service-account.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/manifests/base/api/service.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/manifests/base/kustomization.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.767823 etos_environment_provider-4.2.0/manifests/base/worker/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/manifests/base/worker/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/manifests/base/worker/service-account.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-02 11:00:02.783823 etos_environment_provider-4.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.763823 etos_environment_provider-4.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.771823 etos_environment_provider-4.2.0/src/environment_provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/environment_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/environment_provider/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    23718 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/environment_provider/environment_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.771823 etos_environment_provider-4.2.0/src/environment_provider/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/environment_provider/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/environment_provider/lib/celery.py
--rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/environment_provider/lib/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/environment_provider/lib/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/environment_provider/lib/encrypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/environment_provider/lib/graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/environment_provider/lib/join.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/environment_provider/lib/json_dumps.py
--rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/environment_provider/lib/log_area.py
--rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/environment_provider/lib/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     7280 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/environment_provider/lib/test_suite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/environment_provider/lib/uuid_generate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.771823 etos_environment_provider-4.2.0/src/environment_provider/splitter/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/environment_provider/splitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/environment_provider/splitter/split.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.783823 etos_environment_provider-4.2.0/src/etos_environment_provider.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-02 11:00:02.000000 etos_environment_provider-4.2.0/src/etos_environment_provider.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-02 11:00:02.000000 etos_environment_provider-4.2.0/src/etos_environment_provider.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 11:00:02.000000 etos_environment_provider-4.2.0/src/etos_environment_provider.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 11:00:02.000000 etos_environment_provider-4.2.0/src/etos_environment_provider.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-02 11:00:02.000000 etos_environment_provider-4.2.0/src/etos_environment_provider.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-02 11:00:02.000000 etos_environment_provider-4.2.0/src/etos_environment_provider.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.775823 etos_environment_provider-4.2.0/src/execution_space_provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/execution_space_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/execution_space_provider/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/execution_space_provider/execution_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/execution_space_provider/execution_space_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.775823 etos_environment_provider-4.2.0/src/execution_space_provider/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/execution_space_provider/schemas/external_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/execution_space_provider/schemas/jsontas_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.775823 etos_environment_provider-4.2.0/src/execution_space_provider/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/execution_space_provider/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/execution_space_provider/utilities/checkin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/execution_space_provider/utilities/checkout.py
--rw-r--r--   0 runner    (1001) docker     (127)    17525 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/execution_space_provider/utilities/external_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/execution_space_provider/utilities/instructions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8247 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/execution_space_provider/utilities/jsontas_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/execution_space_provider/utilities/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.775823 etos_environment_provider-4.2.0/src/iut_provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/iut_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/iut_provider/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/iut_provider/iut.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/iut_provider/iut_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.775823 etos_environment_provider-4.2.0/src/iut_provider/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/iut_provider/schemas/external_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/iut_provider/schemas/jsontas_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.779823 etos_environment_provider-4.2.0/src/iut_provider/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/iut_provider/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/iut_provider/utilities/checkin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/iut_provider/utilities/checkout.py
--rw-r--r--   0 runner    (1001) docker     (127)    13994 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/iut_provider/utilities/external_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     9326 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/iut_provider/utilities/jsontas_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/iut_provider/utilities/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/iut_provider/utilities/prepare.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.779823 etos_environment_provider-4.2.0/src/log_area_provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/log_area_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/log_area_provider/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/log_area_provider/log_area.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/log_area_provider/log_area_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.779823 etos_environment_provider-4.2.0/src/log_area_provider/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/log_area_provider/schemas/external_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/log_area_provider/schemas/jsontas_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.779823 etos_environment_provider-4.2.0/src/log_area_provider/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/log_area_provider/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/log_area_provider/utilities/checkin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/log_area_provider/utilities/checkout.py
--rw-r--r--   0 runner    (1001) docker     (127)    14811 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/log_area_provider/utilities/external_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/log_area_provider/utilities/jsontas_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/log_area_provider/utilities/list.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.779823 etos_environment_provider-4.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.779823 etos_environment_provider-4.2.0/tests/external_execution_space/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/tests/external_execution_space/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25624 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/tests/external_execution_space/test_external_execution_space.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.779823 etos_environment_provider-4.2.0/tests/external_iut/
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/tests/external_iut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24107 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/tests/external_iut/test_external_iut.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.779823 etos_environment_provider-4.2.0/tests/external_log_area/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/tests/external_log_area/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24737 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/tests/external_log_area/test_external_log_area.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.783823 etos_environment_provider-4.2.0/tests/library/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/tests/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/tests/library/fake_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/tests/library/fake_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/tests/library/graphql_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.783823 etos_environment_provider-4.2.0/tests/splitter/
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/tests/splitter/test_splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7967 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/tests/tercc.py
--rw-r--r--   0 runner    (1001) docker     (127)    11667 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/tests/test_environment_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:22:03.427299 etos_environment_provider-4.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:22:03.407299 etos_environment_provider-4.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:22:03.411299 etos_environment_provider-4.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/.github/workflows/build-push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)    10850 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-06-03 09:22:03.427299 etos_environment_provider-4.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:22:03.415299 etos_environment_provider-4.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7634 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:22:03.415299 etos_environment_provider-4.3.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:22:03.407299 etos_environment_provider-4.3.0/manifests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:22:03.415299 etos_environment_provider-4.3.0/manifests/base/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:22:03.415299 etos_environment_provider-4.3.0/manifests/base/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/manifests/base/api/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/manifests/base/api/service-account.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/manifests/base/api/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/manifests/base/kustomization.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:22:03.415299 etos_environment_provider-4.3.0/manifests/base/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/manifests/base/worker/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/manifests/base/worker/service-account.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-06-03 09:22:03.427299 etos_environment_provider-4.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:22:03.407299 etos_environment_provider-4.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:22:03.415299 etos_environment_provider-4.3.0/src/environment_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/environment_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/environment_provider/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22069 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/environment_provider/environment_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:22:03.415299 etos_environment_provider-4.3.0/src/environment_provider/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/environment_provider/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/environment_provider/lib/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/environment_provider/lib/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/environment_provider/lib/encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/environment_provider/lib/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/environment_provider/lib/join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/environment_provider/lib/json_dumps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/environment_provider/lib/log_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/environment_provider/lib/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7280 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/environment_provider/lib/test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/environment_provider/lib/uuid_generate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:22:03.415299 etos_environment_provider-4.3.0/src/environment_provider/splitter/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/environment_provider/splitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/environment_provider/splitter/split.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:22:03.427299 etos_environment_provider-4.3.0/src/etos_environment_provider.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-06-03 09:22:03.000000 etos_environment_provider-4.3.0/src/etos_environment_provider.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-06-03 09:22:03.000000 etos_environment_provider-4.3.0/src/etos_environment_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 09:22:03.000000 etos_environment_provider-4.3.0/src/etos_environment_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 09:22:03.000000 etos_environment_provider-4.3.0/src/etos_environment_provider.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-06-03 09:22:03.000000 etos_environment_provider-4.3.0/src/etos_environment_provider.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-06-03 09:22:03.000000 etos_environment_provider-4.3.0/src/etos_environment_provider.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:22:03.419299 etos_environment_provider-4.3.0/src/execution_space_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/execution_space_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/execution_space_provider/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/execution_space_provider/execution_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/execution_space_provider/execution_space_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:22:03.419299 etos_environment_provider-4.3.0/src/execution_space_provider/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/execution_space_provider/schemas/external_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/execution_space_provider/schemas/jsontas_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:22:03.419299 etos_environment_provider-4.3.0/src/execution_space_provider/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/execution_space_provider/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/execution_space_provider/utilities/checkin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/execution_space_provider/utilities/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17525 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/execution_space_provider/utilities/external_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/execution_space_provider/utilities/instructions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8247 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/execution_space_provider/utilities/jsontas_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/execution_space_provider/utilities/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:22:03.419299 etos_environment_provider-4.3.0/src/iut_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/iut_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/iut_provider/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/iut_provider/iut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/iut_provider/iut_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:22:03.419299 etos_environment_provider-4.3.0/src/iut_provider/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/iut_provider/schemas/external_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/iut_provider/schemas/jsontas_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:22:03.423299 etos_environment_provider-4.3.0/src/iut_provider/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/iut_provider/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/iut_provider/utilities/checkin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/iut_provider/utilities/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13994 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/iut_provider/utilities/external_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9326 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/iut_provider/utilities/jsontas_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/iut_provider/utilities/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/iut_provider/utilities/prepare.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:22:03.423299 etos_environment_provider-4.3.0/src/log_area_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/log_area_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/log_area_provider/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/log_area_provider/log_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/log_area_provider/log_area_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:22:03.423299 etos_environment_provider-4.3.0/src/log_area_provider/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/log_area_provider/schemas/external_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/log_area_provider/schemas/jsontas_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:22:03.423299 etos_environment_provider-4.3.0/src/log_area_provider/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/log_area_provider/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/log_area_provider/utilities/checkin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/log_area_provider/utilities/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14811 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/log_area_provider/utilities/external_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/log_area_provider/utilities/jsontas_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/src/log_area_provider/utilities/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:22:03.423299 etos_environment_provider-4.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:22:03.423299 etos_environment_provider-4.3.0/tests/external_execution_space/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/tests/external_execution_space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25624 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/tests/external_execution_space/test_external_execution_space.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:22:03.427299 etos_environment_provider-4.3.0/tests/external_iut/
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/tests/external_iut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24107 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/tests/external_iut/test_external_iut.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:22:03.427299 etos_environment_provider-4.3.0/tests/external_log_area/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/tests/external_log_area/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24737 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/tests/external_log_area/test_external_log_area.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:22:03.427299 etos_environment_provider-4.3.0/tests/library/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/tests/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/tests/library/fake_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/tests/library/fake_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/tests/library/graphql_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:22:03.427299 etos_environment_provider-4.3.0/tests/splitter/
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/tests/splitter/test_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7967 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/tests/tercc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11935 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/tests/test_environment_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-06-03 09:21:57.000000 etos_environment_provider-4.3.0/tox.ini
```

### Comparing `etos_environment_provider-4.2.0/.coveragerc` & `etos_environment_provider-4.3.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/.github/workflows/build-push.yml` & `etos_environment_provider-4.3.0/.github/workflows/build-push.yml`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/.github/workflows/main.yml` & `etos_environment_provider-4.3.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/.gitignore` & `etos_environment_provider-4.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/LICENSE.txt` & `etos_environment_provider-4.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/PKG-INFO` & `etos_environment_provider-4.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etos_environment_provider
-Version: 4.2.0
+Version: 4.3.0
 Summary: Environment provider for ETOS.
 Home-page: https://github.com/eiffel-community/etos-environment-provider
 Author: Tobias Persson
 Author-email: tobias.persson@axis.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://etos.readthedocs.io/
 Platform: Linux
@@ -12,23 +12,19 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE.txt
 License-File: AUTHORS.rst
-Requires-Dist: eventlet~=0.33
-Requires-Dist: celery~=5.3
 Requires-Dist: cryptography<43.0.0,>=42.0.4
-Requires-Dist: gevent~=23.7
-Requires-Dist: gunicorn~=19.9
 Requires-Dist: jsontas~=1.3
 Requires-Dist: packageurl-python~=0.11
 Requires-Dist: etcd3gw~=2.3
-Requires-Dist: etos_lib==4.2.0
+Requires-Dist: etos_lib==4.3.0
 Requires-Dist: opentelemetry-api~=1.21
 Requires-Dist: opentelemetry-exporter-otlp~=1.21
 Requires-Dist: opentelemetry-sdk~=1.21
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
```

### Comparing `etos_environment_provider-4.2.0/README.rst` & `etos_environment_provider-4.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/docs/Makefile` & `etos_environment_provider-4.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/docs/conf.py` & `etos_environment_provider-4.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/manifests/base/api/deployment.yaml` & `etos_environment_provider-4.3.0/manifests/base/api/deployment.yaml`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/manifests/base/kustomization.yaml` & `etos_environment_provider-4.3.0/manifests/base/kustomization.yaml`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/manifests/base/worker/deployment.yaml` & `etos_environment_provider-4.3.0/manifests/base/worker/deployment.yaml`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/setup.cfg` & `etos_environment_provider-4.3.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -20,23 +20,19 @@
 zip_safe = False
 packages = find:
 include_package_data = True
 package_dir = 
 	=src
 setup_requires = pyscaffold>=3.2a0,<3.3a0
 install_requires = 
-	eventlet~=0.33
-	celery~=5.3
 	cryptography>=42.0.4,<43.0.0
-	gevent~=23.7
-	gunicorn~=19.9
 	jsontas~=1.3
 	packageurl-python~=0.11
 	etcd3gw~=2.3
-	etos_lib==4.2.0
+	etos_lib==4.3.0
 	opentelemetry-api~=1.21
 	opentelemetry-exporter-otlp~=1.21
 	opentelemetry-sdk~=1.21
 python_requires = >=3.8
 
 [options.package_data]
 * = *.json
```

### Comparing `etos_environment_provider-4.2.0/setup.py` & `etos_environment_provider-4.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/environment_provider/__init__.py` & `etos_environment_provider-4.3.0/src/environment_provider/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,26 +14,22 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """ETOS environment provider module."""
 import logging
 import os
 from importlib.metadata import PackageNotFoundError, version
 
-from etos_lib.logging.logger import setup_logging
-
 try:
     VERSION = version("environment_provider")
 except PackageNotFoundError:
     VERSION = "Unknown"
 
 DEV = os.getenv("DEV", "false").lower() == "true"
 ENVIRONMENT = "development" if DEV else "production"
-# Disable extra logging, if the environment provider is imported instead of executed via celery
-if os.getenv("ENVIRONMENT_PROVIDER_DISABLE_LOGGING", "false") == "false":
-    setup_logging("ETOS Environment Provider Worker", VERSION, ENVIRONMENT)
+
 # JSONTas would print all passwords as they are encrypted,
 # which is not safe, so we disable propagation on the loggers.
 # Propagation needs to be set to 0 instead of disabling the
 # logger or setting the loglevel higher because of how the
 # etos library sets up logging.
 logging.getLogger("Dataset").propagate = 0
 logging.getLogger("JSONTas").propagate = 0
```

### Comparing `etos_environment_provider-4.2.0/src/environment_provider/environment.py` & `etos_environment_provider-4.3.0/src/environment_provider/environment.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/environment_provider/environment_provider.py` & `etos_environment_provider-4.3.0/src/environment_provider/environment_provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,41 +9,37 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""ETOS Environment Provider celery task module."""
+"""ETOS Environment Provider module."""
 import json
 import logging
 import os
 import time
 import traceback
 import uuid
-from copy import deepcopy
 from datetime import datetime
 from tempfile import NamedTemporaryFile
-from threading import Lock
 from typing import Any, Union
 
 from etos_lib.etos import ETOS
 from etos_lib.lib.events import EiffelEnvironmentDefinedEvent
 from etos_lib.logging.logger import FORMAT_CONFIG
 from etos_lib.opentelemetry.semconv import Attributes as SemConvAttributes
 from jsontas.jsontas import JsonTas
 import opentelemetry
 from opentelemetry.trace import SpanKind
 
 from execution_space_provider.execution_space import ExecutionSpace
 from log_area_provider.log_area import LogArea
 
-from .lib.celery import APP
 from .lib.config import Config
-from .lib.database import ETCDPath
 from .lib.encrypt import Encrypt
 from .lib.graphql import request_main_suite
 from .lib.join import Join
 from .lib.json_dumps import JsonDumps
 from .lib.log_area import LogArea
 from .lib.registry import ProviderRegistry
 from .lib.test_suite import TestSuite
@@ -58,49 +54,38 @@
 
 
 class EnvironmentProviderNotConfigured(Exception):
     """Environment provider was not configured prior to request."""
 
 
 class EnvironmentProvider:  # pylint:disable=too-many-instance-attributes
-    """Environment provider celery Task."""
+    """Environment provider."""
 
     logger = logging.getLogger("EnvironmentProvider")
     environment_provider_config = None
     iut_provider = None
     log_area_provider = None
     execution_space_provider = None
-    task_track_started = True  # Make celery task report 'STARTED' state
-    lock = Lock()
 
-    def __init__(self, suite_id: str, suite_runner_ids: list[str], copy: bool = True) -> None:
+    def __init__(self, suite_id: str, suite_runner_ids: list[str]) -> None:
         """Initialize ETOS, dataset, provider registry and splitter.
 
         :param suite_id: Suite ID to get an environment for
         :param suite_runner_ids: IDs from the suite runner to correlate sub suites.
-        :param copy: Whether or not to copy the etos config. Set to False if not running celery.
         """
         FORMAT_CONFIG.identifier = suite_id
-        self.logger.info("Initializing EnvironmentProvider task.")
+        self.logger.info("Initializing EnvironmentProvider.")
         self.tracer = opentelemetry.trace.get_tracer(__name__)
 
         self.etos = ETOS("ETOS Environment Provider", os.getenv("HOSTNAME"), "Environment Provider")
 
         self.suite_id = suite_id
         self.suite_runner_ids = suite_runner_ids
 
-        with self.lock:
-            # Since celery workers can share memory between them we need to make the configuration
-            # of ETOS library unique as it uses the memory sharing feature with the internal
-            # configuration dictionary.
-            # The impact of not doing this is that the environment provider would re-use
-            # another workers configuration instead of using its own.
-            if copy:
-                self.etos.config.config = deepcopy(self.etos.config.config)
-            self.reset()
+        self.reset()
         self.splitter = Splitter(self.etos, {})
 
     def reset(self) -> None:
         """Create a new dataset and provider registry."""
         self.jsontas = JsonTas()
         self.dataset = self.jsontas.dataset
         self.dataset.add("json_dumps", JsonDumps)
@@ -303,19 +288,14 @@
         event.meta.event_id = event_id
         self.etos.events.send(
             event,
             {"CONTEXT": self.etos.config.get("environment_provider_context")},
             {"name": sub_suite.get("name"), "uri": url},
         )
 
-        # TODO: These shall be removed when API version v1 is used by the ESR and API.
-        environment = ETCDPath("/environment")
-        environment.join(f"{event_id}/testrun-id").write(self.suite_id)
-        environment.join(f"{event_id}/suite-id").write(sub_suite["test_suite_started_id"])
-
         suite = self.registry.testrun.join(f"suite/{sub_suite['test_suite_started_id']}")
         suite.join(f"/subsuite/{event_id}/suite").write(json.dumps(sub_suite))
 
     def upload_sub_suite(self, sub_suite: dict) -> str:
         """Upload sub suite to log area.
 
         :param sub_suite: Sub suite to upload to log area.
@@ -578,19 +558,7 @@
             traceback.print_exc()
             self.logger.error("Failed creating environment for test. %r", extra={"user_log": True})
             return {"error": str(exception), "details": traceback.format_exc()}
         finally:
             if self.etos.publisher is not None and not self.etos.debug.disable_sending_events:
                 self.etos.publisher.wait_for_unpublished_events()
                 self.etos.publisher.stop()
-
-
-@APP.task(name="EnvironmentProvider")
-def get_environment(suite_id: str, suite_runner_ids: list[str]) -> dict:
-    """Get an environment for ETOS test executions.
-
-    :param suite_id: Suite ID to get an environment for
-    :param suite_runner_ids: Suite runner correlation IDs.
-    :return: Test suite JSON with assigned IUTs, execution spaces and log areas.
-    """
-    environment_provider = EnvironmentProvider(suite_id, suite_runner_ids)
-    return environment_provider.run()
```

### Comparing `etos_environment_provider-4.2.0/src/environment_provider/lib/__init__.py` & `etos_environment_provider-4.3.0/src/environment_provider/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/environment_provider/lib/config.py` & `etos_environment_provider-4.3.0/src/environment_provider/lib/config.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/environment_provider/lib/database.py` & `etos_environment_provider-4.3.0/src/environment_provider/lib/database.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/environment_provider/lib/encrypt.py` & `etos_environment_provider-4.3.0/src/environment_provider/lib/encrypt.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/environment_provider/lib/graphql.py` & `etos_environment_provider-4.3.0/src/environment_provider/lib/graphql.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/environment_provider/lib/join.py` & `etos_environment_provider-4.3.0/src/environment_provider/lib/join.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/environment_provider/lib/json_dumps.py` & `etos_environment_provider-4.3.0/src/environment_provider/lib/json_dumps.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/environment_provider/lib/log_area.py` & `etos_environment_provider-4.3.0/src/environment_provider/lib/log_area.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/environment_provider/lib/registry.py` & `etos_environment_provider-4.3.0/src/environment_provider/lib/registry.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/environment_provider/lib/test_suite.py` & `etos_environment_provider-4.3.0/src/environment_provider/lib/test_suite.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/environment_provider/lib/uuid_generate.py` & `etos_environment_provider-4.3.0/src/environment_provider/lib/uuid_generate.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/environment_provider/splitter/__init__.py` & `etos_environment_provider-4.3.0/src/environment_provider/splitter/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/environment_provider/splitter/split.py` & `etos_environment_provider-4.3.0/src/environment_provider/splitter/split.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/etos_environment_provider.egg-info/PKG-INFO` & `etos_environment_provider-4.3.0/src/etos_environment_provider.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etos_environment_provider
-Version: 4.2.0
+Version: 4.3.0
 Summary: Environment provider for ETOS.
 Home-page: https://github.com/eiffel-community/etos-environment-provider
 Author: Tobias Persson
 Author-email: tobias.persson@axis.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://etos.readthedocs.io/
 Platform: Linux
@@ -12,23 +12,19 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE.txt
 License-File: AUTHORS.rst
-Requires-Dist: eventlet~=0.33
-Requires-Dist: celery~=5.3
 Requires-Dist: cryptography<43.0.0,>=42.0.4
-Requires-Dist: gevent~=23.7
-Requires-Dist: gunicorn~=19.9
 Requires-Dist: jsontas~=1.3
 Requires-Dist: packageurl-python~=0.11
 Requires-Dist: etcd3gw~=2.3
-Requires-Dist: etos_lib==4.2.0
+Requires-Dist: etos_lib==4.3.0
 Requires-Dist: opentelemetry-api~=1.21
 Requires-Dist: opentelemetry-exporter-otlp~=1.21
 Requires-Dist: opentelemetry-sdk~=1.21
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
```

### Comparing `etos_environment_provider-4.2.0/src/etos_environment_provider.egg-info/SOURCES.txt` & `etos_environment_provider-4.3.0/src/etos_environment_provider.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 manifests/base/api/service.yaml
 manifests/base/worker/deployment.yaml
 manifests/base/worker/service-account.yaml
 src/environment_provider/__init__.py
 src/environment_provider/environment.py
 src/environment_provider/environment_provider.py
 src/environment_provider/lib/__init__.py
-src/environment_provider/lib/celery.py
 src/environment_provider/lib/config.py
 src/environment_provider/lib/database.py
 src/environment_provider/lib/encrypt.py
 src/environment_provider/lib/graphql.py
 src/environment_provider/lib/join.py
 src/environment_provider/lib/json_dumps.py
 src/environment_provider/lib/log_area.py
```

### Comparing `etos_environment_provider-4.2.0/src/execution_space_provider/__init__.py` & `etos_environment_provider-4.3.0/src/execution_space_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/execution_space_provider/exceptions.py` & `etos_environment_provider-4.3.0/src/execution_space_provider/exceptions.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/execution_space_provider/execution_space.py` & `etos_environment_provider-4.3.0/src/execution_space_provider/execution_space.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/execution_space_provider/execution_space_provider.py` & `etos_environment_provider-4.3.0/src/execution_space_provider/execution_space_provider.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/execution_space_provider/schemas/external_schema.json` & `etos_environment_provider-4.3.0/src/execution_space_provider/schemas/external_schema.json`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/execution_space_provider/schemas/jsontas_schema.json` & `etos_environment_provider-4.3.0/src/execution_space_provider/schemas/jsontas_schema.json`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/execution_space_provider/utilities/__init__.py` & `etos_environment_provider-4.3.0/src/execution_space_provider/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/execution_space_provider/utilities/checkin.py` & `etos_environment_provider-4.3.0/src/execution_space_provider/utilities/checkin.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/execution_space_provider/utilities/checkout.py` & `etos_environment_provider-4.3.0/src/execution_space_provider/utilities/checkout.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/execution_space_provider/utilities/external_provider.py` & `etos_environment_provider-4.3.0/src/execution_space_provider/utilities/external_provider.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/execution_space_provider/utilities/instructions.py` & `etos_environment_provider-4.3.0/src/execution_space_provider/utilities/instructions.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/execution_space_provider/utilities/jsontas_provider.py` & `etos_environment_provider-4.3.0/src/execution_space_provider/utilities/jsontas_provider.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/execution_space_provider/utilities/list.py` & `etos_environment_provider-4.3.0/src/execution_space_provider/utilities/list.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/iut_provider/__init__.py` & `etos_environment_provider-4.3.0/src/iut_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/iut_provider/exceptions.py` & `etos_environment_provider-4.3.0/src/iut_provider/exceptions.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/iut_provider/iut.py` & `etos_environment_provider-4.3.0/src/iut_provider/iut.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/iut_provider/iut_provider.py` & `etos_environment_provider-4.3.0/src/iut_provider/iut_provider.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/iut_provider/schemas/external_schema.json` & `etos_environment_provider-4.3.0/src/iut_provider/schemas/external_schema.json`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/iut_provider/schemas/jsontas_schema.json` & `etos_environment_provider-4.3.0/src/iut_provider/schemas/jsontas_schema.json`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/iut_provider/utilities/__init__.py` & `etos_environment_provider-4.3.0/src/iut_provider/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/iut_provider/utilities/checkin.py` & `etos_environment_provider-4.3.0/src/iut_provider/utilities/checkin.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/iut_provider/utilities/checkout.py` & `etos_environment_provider-4.3.0/src/iut_provider/utilities/checkout.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/iut_provider/utilities/external_provider.py` & `etos_environment_provider-4.3.0/src/iut_provider/utilities/external_provider.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/iut_provider/utilities/jsontas_provider.py` & `etos_environment_provider-4.3.0/src/iut_provider/utilities/jsontas_provider.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/iut_provider/utilities/list.py` & `etos_environment_provider-4.3.0/src/iut_provider/utilities/list.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/iut_provider/utilities/prepare.py` & `etos_environment_provider-4.3.0/src/iut_provider/utilities/prepare.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/log_area_provider/__init__.py` & `etos_environment_provider-4.3.0/src/log_area_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/log_area_provider/exceptions.py` & `etos_environment_provider-4.3.0/src/log_area_provider/exceptions.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/log_area_provider/log_area.py` & `etos_environment_provider-4.3.0/src/log_area_provider/log_area.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/log_area_provider/log_area_provider.py` & `etos_environment_provider-4.3.0/src/log_area_provider/log_area_provider.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/log_area_provider/schemas/external_schema.json` & `etos_environment_provider-4.3.0/src/log_area_provider/schemas/external_schema.json`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/log_area_provider/schemas/jsontas_schema.json` & `etos_environment_provider-4.3.0/src/log_area_provider/schemas/jsontas_schema.json`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/log_area_provider/utilities/__init__.py` & `etos_environment_provider-4.3.0/src/log_area_provider/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/log_area_provider/utilities/checkin.py` & `etos_environment_provider-4.3.0/src/log_area_provider/utilities/checkin.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/log_area_provider/utilities/checkout.py` & `etos_environment_provider-4.3.0/src/log_area_provider/utilities/checkout.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/log_area_provider/utilities/external_provider.py` & `etos_environment_provider-4.3.0/src/log_area_provider/utilities/external_provider.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/log_area_provider/utilities/jsontas_provider.py` & `etos_environment_provider-4.3.0/src/log_area_provider/utilities/jsontas_provider.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/src/log_area_provider/utilities/list.py` & `etos_environment_provider-4.3.0/src/log_area_provider/utilities/list.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/tests/__init__.py` & `etos_environment_provider-4.3.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/tests/external_execution_space/__init__.py` & `etos_environment_provider-4.3.0/tests/external_execution_space/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/tests/external_execution_space/test_external_execution_space.py` & `etos_environment_provider-4.3.0/tests/external_execution_space/test_external_execution_space.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/tests/external_iut/__init__.py` & `etos_environment_provider-4.3.0/tests/external_iut/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/tests/external_iut/test_external_iut.py` & `etos_environment_provider-4.3.0/tests/external_iut/test_external_iut.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/tests/external_log_area/__init__.py` & `etos_environment_provider-4.3.0/tests/external_log_area/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/tests/external_log_area/test_external_log_area.py` & `etos_environment_provider-4.3.0/tests/external_log_area/test_external_log_area.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/tests/library/__init__.py` & `etos_environment_provider-4.3.0/tests/library/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/tests/library/fake_database.py` & `etos_environment_provider-4.3.0/tests/library/fake_database.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/tests/library/fake_server.py` & `etos_environment_provider-4.3.0/tests/library/fake_server.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/tests/library/graphql_handler.py` & `etos_environment_provider-4.3.0/tests/library/graphql_handler.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/tests/splitter/test_splitter.py` & `etos_environment_provider-4.3.0/tests/splitter/test_splitter.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/tests/tercc.py` & `etos_environment_provider-4.3.0/tests/tercc.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.2.0/tests/test_environment_provider.py` & `etos_environment_provider-4.3.0/tests/test_environment_provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import logging
 import os
 import unittest
 
 from etos_lib.lib.config import Config
 from etos_lib.lib.debug import Debug
 
-from environment_provider.environment_provider import get_environment
+from environment_provider.environment_provider import EnvironmentProvider
 from tests.library.fake_database import FakeDatabase
 from tests.library.fake_server import FakeServer
 from tests.library.graphql_handler import GraphQLHandler
 
 from .tercc import TERCC, TERCC_PERMUTATION, TERCC_SUB_SUITES
 
 IUT_PROVIDER = {
@@ -156,15 +156,16 @@
                 f"/testrun/{suite_id}/provider/dataset",
                 json.dumps({"host": server.host}),
             )
             os.environ["ETOS_GRAPHQL_SERVER"] = server.host
             os.environ["ETOS_API"] = server.host
 
             self.logger.info("STEP: Run the environment provider.")
-            result = get_environment(suite_id, suite_runner_ids)
+            environment_provider = EnvironmentProvider(suite_id, suite_runner_ids)
+            result = environment_provider.run()
             print(result)
         self.assertIsNone(result.get("error"))
 
         self.logger.info("STEP: Verify that two environments were sent.")
         environments = []
         for event in Debug().events_published:
             if event.meta.type == "EiffelEnvironmentDefinedEvent":
@@ -204,15 +205,16 @@
                 f"/testrun/{suite_id}/provider/dataset",
                 json.dumps({"host": server.host}),
             )
             os.environ["ETOS_GRAPHQL_SERVER"] = server.host
             os.environ["ETOS_API"] = server.host
 
             self.logger.info("STEP: Run the environment provider.")
-            result = get_environment(suite_id, suite_runner_ids)
+            environment_provider = EnvironmentProvider(suite_id, suite_runner_ids)
+            result = environment_provider.run()
             print(result)
         self.assertIsNone(result.get("error"))
 
         self.logger.info("STEP: Verify that two environments were sent.")
         environments = []
         for event in Debug().events_published:
             if event.meta.type == "EiffelEnvironmentDefinedEvent":
@@ -255,15 +257,16 @@
                 f"/testrun/{suite_id}/provider/dataset",
                 json.dumps({"host": server.host}),
             )
             os.environ["ETOS_GRAPHQL_SERVER"] = server.host
             os.environ["ETOS_API"] = server.host
 
             self.logger.info("STEP: Run the environment provider.")
-            result = get_environment(suite_id, suite_runner_ids)
+            environment_provider = EnvironmentProvider(suite_id, suite_runner_ids)
+            result = environment_provider.run()
         self.assertIsNone(result.get("error"))
 
         self.logger.info("STEP: Verify that two environments were sent.")
         environments = []
         for event in Debug().events_published:
             if event.meta.type == "EiffelEnvironmentDefinedEvent":
                 environments.append(event)
@@ -304,15 +307,16 @@
                 f"/testrun/{suite_id}/provider/dataset",
                 json.dumps({"host": server.host}),
             )
             os.environ["ETOS_GRAPHQL_SERVER"] = server.host
             os.environ["ETOS_API"] = server.host
 
             self.logger.info("STEP: Run the environment provider.")
-            result = get_environment(suite_id, suite_runner_ids)
+            environment_provider = EnvironmentProvider(suite_id, suite_runner_ids)
+            result = environment_provider.run()
             print(result)
         self.assertIsNone(result.get("error"))
 
         self.logger.info("STEP: Verify that two environments were sent.")
         environments = []
         for event in Debug().events_published:
             if event.meta.type == "EiffelEnvironmentDefinedEvent":
```

### Comparing `etos_environment_provider-4.2.0/tox.ini` & `etos_environment_provider-4.3.0/tox.ini`

 * *Files identical despite different names*

