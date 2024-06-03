# Comparing `tmp/opal_client-0.7.6.tar.gz` & `tmp/opal-client-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opal_client-0.7.6.tar", last modified: Tue Apr 30 17:18:48 2024, max compression
+gzip compressed data, was "opal-client-0.7.7.tar", last modified: Mon Jun  3 13:38:16 2024, max compression
```

## Comparing `opal_client-0.7.6.tar` & `opal-client-0.7.7.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.888325 opal_client-0.7.6/
--rw-r--r--   0 roekatz    (501) staff       (20)    10001 2024-04-30 17:18:48.887806 opal_client-0.7.6/PKG-INFO
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.880180 opal_client-0.7.6/opal_client/
--rw-r--r--   0 roekatz    (501) staff       (20)       31 2022-12-08 13:40:17.000000 opal_client-0.7.6/opal_client/__init__.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.881709 opal_client-0.7.6/opal_client/callbacks/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_client-0.7.6/opal_client/callbacks/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3034 2022-12-08 13:40:17.000000 opal_client-0.7.6/opal_client/callbacks/api.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4385 2024-03-19 14:53:02.000000 opal_client-0.7.6/opal_client/callbacks/register.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3729 2024-03-19 14:53:02.000000 opal_client-0.7.6/opal_client/callbacks/reporter.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2213 2023-05-29 10:10:14.000000 opal_client-0.7.6/opal_client/cli.py
--rw-r--r--   0 roekatz    (501) staff       (20)    20271 2024-04-30 13:01:51.000000 opal_client-0.7.6/opal_client/client.py
--rw-r--r--   0 roekatz    (501) staff       (20)    12812 2024-04-30 16:48:47.000000 opal_client-0.7.6/opal_client/config.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.882507 opal_client-0.7.6/opal_client/data/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_client-0.7.6/opal_client/data/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)      863 2022-12-08 13:40:17.000000 opal_client-0.7.6/opal_client/data/api.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4489 2024-04-30 12:59:10.000000 opal_client-0.7.6/opal_client/data/fetcher.py
--rw-r--r--   0 roekatz    (501) staff       (20)      842 2022-12-08 13:40:17.000000 opal_client-0.7.6/opal_client/data/rpc.py
--rw-r--r--   0 roekatz    (501) staff       (20)    23358 2024-04-30 13:01:51.000000 opal_client-0.7.6/opal_client/data/updater.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.883537 opal_client-0.7.6/opal_client/engine/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2023-05-29 10:10:14.000000 opal_client-0.7.6/opal_client/engine/__init__.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.883850 opal_client-0.7.6/opal_client/engine/healthcheck/
--rw-r--r--   0 roekatz    (501) staff       (20)     1123 2023-05-29 10:10:14.000000 opal_client-0.7.6/opal_client/engine/healthcheck/opal.rego
--rw-r--r--   0 roekatz    (501) staff       (20)     3032 2024-03-19 14:53:02.000000 opal_client-0.7.6/opal_client/engine/logger.py
--rw-r--r--   0 roekatz    (501) staff       (20)     5702 2023-05-29 10:10:14.000000 opal_client-0.7.6/opal_client/engine/options.py
--rw-r--r--   0 roekatz    (501) staff       (20)    12557 2024-03-19 14:53:02.000000 opal_client-0.7.6/opal_client/engine/runner.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2220 2022-12-08 13:40:17.000000 opal_client-0.7.6/opal_client/limiter.py
--rw-r--r--   0 roekatz    (501) staff       (20)       33 2022-12-08 13:40:17.000000 opal_client-0.7.6/opal_client/logger.py
--rw-r--r--   0 roekatz    (501) staff       (20)       96 2022-12-08 13:40:17.000000 opal_client-0.7.6/opal_client/main.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.885051 opal_client-0.7.6/opal_client/policy/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_client-0.7.6/opal_client/policy/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)      509 2024-03-19 14:53:02.000000 opal_client-0.7.6/opal_client/policy/api.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4678 2024-04-30 12:59:10.000000 opal_client-0.7.6/opal_client/policy/fetcher.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1791 2024-02-28 15:15:55.000000 opal_client-0.7.6/opal_client/policy/options.py
--rw-r--r--   0 roekatz    (501) staff       (20)      596 2022-12-08 13:40:17.000000 opal_client-0.7.6/opal_client/policy/topics.py
--rw-r--r--   0 roekatz    (501) staff       (20)    15053 2024-03-19 14:53:02.000000 opal_client-0.7.6/opal_client/policy/updater.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.886421 opal_client-0.7.6/opal_client/policy_store/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_client-0.7.6/opal_client/policy_store/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1650 2023-05-29 10:10:14.000000 opal_client-0.7.6/opal_client/policy_store/api.py
--rw-r--r--   0 roekatz    (501) staff       (20)     8442 2024-03-13 14:12:07.000000 opal_client-0.7.6/opal_client/policy_store/base_policy_store_client.py
--rw-r--r--   0 roekatz    (501) staff       (20)    12318 2023-05-29 10:10:14.000000 opal_client-0.7.6/opal_client/policy_store/cedar_client.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3040 2024-03-19 14:53:02.000000 opal_client-0.7.6/opal_client/policy_store/mock_policy_store_client.py
--rw-r--r--   0 roekatz    (501) staff       (20)    36976 2024-03-19 14:53:02.000000 opal_client-0.7.6/opal_client/policy_store/opa_client.py
--rw-r--r--   0 roekatz    (501) staff       (20)     6605 2024-03-13 14:12:07.000000 opal_client-0.7.6/opal_client/policy_store/policy_store_client_factory.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1831 2023-06-20 17:01:29.000000 opal_client-0.7.6/opal_client/policy_store/schemas.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.887034 opal_client-0.7.6/opal_client/tests/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_client-0.7.6/opal_client/tests/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)    10553 2024-03-19 14:53:02.000000 opal_client-0.7.6/opal_client/tests/data_updater_test.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3973 2024-03-19 14:53:02.000000 opal_client-0.7.6/opal_client/tests/opa_client_test.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4542 2024-03-19 14:53:02.000000 opal_client-0.7.6/opal_client/tests/server_to_client_intergation_test.py
--rw-r--r--   0 roekatz    (501) staff       (20)      613 2023-07-17 14:14:01.000000 opal_client-0.7.6/opal_client/utils.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.887306 opal_client-0.7.6/opal_client.egg-info/
--rw-r--r--   0 roekatz    (501) staff       (20)    10001 2024-04-30 17:18:48.000000 opal_client-0.7.6/opal_client.egg-info/PKG-INFO
--rw-r--r--   0 roekatz    (501) staff       (20)     1501 2024-04-30 17:18:48.000000 opal_client-0.7.6/opal_client.egg-info/SOURCES.txt
--rw-r--r--   0 roekatz    (501) staff       (20)        1 2024-04-30 17:18:48.000000 opal_client-0.7.6/opal_client.egg-info/dependency_links.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       52 2024-04-30 17:18:48.000000 opal_client-0.7.6/opal_client.egg-info/entry_points.txt
--rw-r--r--   0 roekatz    (501) staff       (20)      426 2024-04-30 17:18:48.000000 opal_client-0.7.6/opal_client.egg-info/requires.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       12 2024-04-30 17:18:48.000000 opal_client-0.7.6/opal_client.egg-info/top_level.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       38 2024-04-30 17:18:48.888400 opal_client-0.7.6/setup.cfg
--rw-r--r--   0 roekatz    (501) staff       (20)     2886 2024-04-30 13:01:51.000000 opal_client-0.7.6/setup.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:16.930505 opal-client-0.7.7/
+-rw-r--r--   0 asafc      (501) staff       (20)     9293 2024-06-03 13:38:16.930295 opal-client-0.7.7/PKG-INFO
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:16.924580 opal-client-0.7.7/opal_client/
+-rw-r--r--   0 asafc      (501) staff       (20)       31 2022-10-01 21:13:25.000000 opal-client-0.7.7/opal_client/__init__.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:16.925815 opal-client-0.7.7/opal_client/callbacks/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-client-0.7.7/opal_client/callbacks/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3034 2022-10-01 21:13:25.000000 opal-client-0.7.7/opal_client/callbacks/api.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4385 2024-03-17 08:56:30.000000 opal-client-0.7.7/opal_client/callbacks/register.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3729 2024-03-17 08:56:30.000000 opal-client-0.7.7/opal_client/callbacks/reporter.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2213 2023-05-10 17:44:36.000000 opal-client-0.7.7/opal_client/cli.py
+-rw-r--r--   0 asafc      (501) staff       (20)    20271 2024-05-29 13:03:42.000000 opal-client-0.7.7/opal_client/client.py
+-rw-r--r--   0 asafc      (501) staff       (20)    12812 2024-05-29 13:03:42.000000 opal-client-0.7.7/opal_client/config.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:16.926420 opal-client-0.7.7/opal_client/data/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-client-0.7.7/opal_client/data/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)      863 2022-10-01 21:13:25.000000 opal-client-0.7.7/opal_client/data/api.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4489 2024-05-29 13:03:42.000000 opal-client-0.7.7/opal_client/data/fetcher.py
+-rw-r--r--   0 asafc      (501) staff       (20)      842 2022-10-01 21:13:25.000000 opal-client-0.7.7/opal_client/data/rpc.py
+-rw-r--r--   0 asafc      (501) staff       (20)    23358 2024-05-29 13:03:42.000000 opal-client-0.7.7/opal_client/data/updater.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:16.926914 opal-client-0.7.7/opal_client/engine/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-10 17:44:40.000000 opal-client-0.7.7/opal_client/engine/__init__.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:16.927059 opal-client-0.7.7/opal_client/engine/healthcheck/
+-rw-r--r--   0 asafc      (501) staff       (20)     1123 2023-05-10 17:44:40.000000 opal-client-0.7.7/opal_client/engine/healthcheck/opal.rego
+-rw-r--r--   0 asafc      (501) staff       (20)     3032 2024-03-17 08:56:30.000000 opal-client-0.7.7/opal_client/engine/logger.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5702 2023-05-10 17:44:40.000000 opal-client-0.7.7/opal_client/engine/options.py
+-rw-r--r--   0 asafc      (501) staff       (20)    12557 2024-03-17 08:56:30.000000 opal-client-0.7.7/opal_client/engine/runner.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2220 2022-10-01 21:13:25.000000 opal-client-0.7.7/opal_client/limiter.py
+-rw-r--r--   0 asafc      (501) staff       (20)       33 2022-10-01 21:13:25.000000 opal-client-0.7.7/opal_client/logger.py
+-rw-r--r--   0 asafc      (501) staff       (20)       96 2022-10-01 21:13:25.000000 opal-client-0.7.7/opal_client/main.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:16.928257 opal-client-0.7.7/opal_client/policy/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-client-0.7.7/opal_client/policy/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)      509 2024-03-17 08:56:30.000000 opal-client-0.7.7/opal_client/policy/api.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4678 2024-05-29 13:03:42.000000 opal-client-0.7.7/opal_client/policy/fetcher.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1791 2024-01-16 10:53:37.000000 opal-client-0.7.7/opal_client/policy/options.py
+-rw-r--r--   0 asafc      (501) staff       (20)      596 2022-10-01 21:13:25.000000 opal-client-0.7.7/opal_client/policy/topics.py
+-rw-r--r--   0 asafc      (501) staff       (20)    15053 2024-03-17 08:56:30.000000 opal-client-0.7.7/opal_client/policy/updater.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:16.929541 opal-client-0.7.7/opal_client/policy_store/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-client-0.7.7/opal_client/policy_store/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1650 2023-05-10 06:45:11.000000 opal-client-0.7.7/opal_client/policy_store/api.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8442 2023-05-10 17:44:40.000000 opal-client-0.7.7/opal_client/policy_store/base_policy_store_client.py
+-rw-r--r--   0 asafc      (501) staff       (20)    12318 2023-05-10 17:44:40.000000 opal-client-0.7.7/opal_client/policy_store/cedar_client.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3040 2024-03-17 08:56:30.000000 opal-client-0.7.7/opal_client/policy_store/mock_policy_store_client.py
+-rw-r--r--   0 asafc      (501) staff       (20)    36976 2024-03-17 08:56:30.000000 opal-client-0.7.7/opal_client/policy_store/opa_client.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6605 2023-09-11 17:35:10.000000 opal-client-0.7.7/opal_client/policy_store/policy_store_client_factory.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1831 2023-09-11 17:35:10.000000 opal-client-0.7.7/opal_client/policy_store/schemas.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:16.930060 opal-client-0.7.7/opal_client/tests/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-client-0.7.7/opal_client/tests/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)    10553 2024-03-17 08:56:30.000000 opal-client-0.7.7/opal_client/tests/data_updater_test.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3973 2024-03-17 08:56:30.000000 opal-client-0.7.7/opal_client/tests/opa_client_test.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4542 2024-03-17 08:56:30.000000 opal-client-0.7.7/opal_client/tests/server_to_client_intergation_test.py
+-rw-r--r--   0 asafc      (501) staff       (20)      613 2023-09-11 17:35:10.000000 opal-client-0.7.7/opal_client/utils.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:16.925335 opal-client-0.7.7/opal_client.egg-info/
+-rw-r--r--   0 asafc      (501) staff       (20)     9293 2024-06-03 13:38:16.000000 opal-client-0.7.7/opal_client.egg-info/PKG-INFO
+-rw-r--r--   0 asafc      (501) staff       (20)     1501 2024-06-03 13:38:16.000000 opal-client-0.7.7/opal_client.egg-info/SOURCES.txt
+-rw-r--r--   0 asafc      (501) staff       (20)        1 2024-06-03 13:38:16.000000 opal-client-0.7.7/opal_client.egg-info/dependency_links.txt
+-rw-r--r--   0 asafc      (501) staff       (20)       52 2024-06-03 13:38:16.000000 opal-client-0.7.7/opal_client.egg-info/entry_points.txt
+-rw-r--r--   0 asafc      (501) staff       (20)      426 2024-06-03 13:38:16.000000 opal-client-0.7.7/opal_client.egg-info/requires.txt
+-rw-r--r--   0 asafc      (501) staff       (20)       12 2024-06-03 13:38:16.000000 opal-client-0.7.7/opal_client.egg-info/top_level.txt
+-rw-r--r--   0 asafc      (501) staff       (20)       38 2024-06-03 13:38:16.930548 opal-client-0.7.7/setup.cfg
+-rw-r--r--   0 asafc      (501) staff       (20)     2886 2024-05-29 13:03:42.000000 opal-client-0.7.7/setup.py
```

### Comparing `opal_client-0.7.6/PKG-INFO` & `opal-client-0.7.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opal-client
-Version: 0.7.6
+Version: 0.7.7
 Summary: OPAL is an administration layer for Open Policy Agent (OPA), detecting changes to both policy and data and pushing live updates to your agents. The opal-client is deployed alongside a policy-store (e.g: OPA), keeping it up-to-date, by connecting to an opal-server and subscribing to pub/sub updates for policy and policy data changes.
 Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen
 Author-email: or@permit.io
 License: Apache 2.0
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
@@ -14,33 +14,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: aiofiles<1,>=0.8.0
-Requires-Dist: aiohttp<4,>=3.9.2
-Requires-Dist: psutil<6,>=5.9.1
-Requires-Dist: tenacity<9,>=8.0.1
-Requires-Dist: websockets<11,>=10.3
-Requires-Dist: dpath<3,>=2.1.5
-Requires-Dist: jsonpatch<2,>=1.33
-Requires-Dist: opal-common==0.7.6
-Requires-Dist: idna<4,>=3.3
-Requires-Dist: typer<1,>=0.4.1
-Requires-Dist: fastapi<1,>=0.109.1
-Requires-Dist: fastapi_websocket_pubsub==0.3.7
-Requires-Dist: fastapi_websocket_rpc<1,>=0.1.21
-Requires-Dist: gunicorn<23,>=22.0.0
-Requires-Dist: pydantic[email]<2,>=1.9.1
-Requires-Dist: typing-extensions; python_version < "3.8"
-Requires-Dist: uvicorn[standard]<1,>=0.17.6
-Requires-Dist: fastapi-utils<1,>=0.2.1
-Requires-Dist: setuptools>=65.5.1
 
 <p  align="center">
  <img src="https://github.com/permitio/opal/assets/4082578/4e21f85f-30ab-43e2-92de-b82f78888c71" height=170 alt="opal" border="0" />
 </p>
 <h1 align="center">
 ⚡OPAL⚡
 </h1>
```

#### html2text {}

```diff
@@ -1,32 +1,22 @@
-Metadata-Version: 2.1 Name: opal-client Version: 0.7.6 Summary: OPAL is an
+Metadata-Version: 2.1 Name: opal-client Version: 0.7.7 Summary: OPAL is an
 administration layer for Open Policy Agent (OPA), detecting changes to both
 policy and data and pushing live updates to your agents. The opal-client is
 deployed alongside a policy-store (e.g: OPA), keeping it up-to-date, by
 connecting to an opal-server and subscribing to pub/sub updates for policy and
 policy data changes. Home-page: https://github.com/permitio/opal Author: Or
 Weis, Asaf Cohen Author-email: or@permit.io License: Apache 2.0 Classifier:
 Operating System :: OS Independent Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI Requires-Python: >=3.9
-Description-Content-Type: text/markdown Requires-Dist: aiofiles<1,>=0.8.0
-Requires-Dist: aiohttp<4,>=3.9.2 Requires-Dist: psutil<6,>=5.9.1 Requires-Dist:
-tenacity<9,>=8.0.1 Requires-Dist: websockets<11,>=10.3 Requires-Dist:
-dpath<3,>=2.1.5 Requires-Dist: jsonpatch<2,>=1.33 Requires-Dist: opal-
-common==0.7.6 Requires-Dist: idna<4,>=3.3 Requires-Dist: typer<1,>=0.4.1
-Requires-Dist: fastapi<1,>=0.109.1 Requires-Dist:
-fastapi_websocket_pubsub==0.3.7 Requires-Dist: fastapi_websocket_rpc<1,>=0.1.21
-Requires-Dist: gunicorn<23,>=22.0.0 Requires-Dist: pydantic[email]<2,>=1.9.1
-Requires-Dist: typing-extensions; python_version < "3.8" Requires-Dist: uvicorn
-[standard]<1,>=0.17.6 Requires-Dist: fastapi-utils<1,>=0.2.1 Requires-Dist:
-setuptools>=65.5.1
+Description-Content-Type: text/markdown
                                     [opal]
                            ************ ?â??¡OOPPAALL?â??¡ ************
                  ********** OOppeenn PPoolliiccyy AAddmmiinniissttrraattiioonn LLaayyeerr **********
 _[_T_e_s_t_s_]_[_P_a_c_k_a_g_e_]_[_P_a_c_k_a_g_e_]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_c_k_e_r_ _p_u_l_l_s_]_[_J_o_i_n_ _o_u_r_ _S_l_a_c_k_!_]_[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_t_w_i_t_t_e_r_/_f_o_l_l_o_w_/
 _p_e_r_m_i_t___i_o_?_l_a_b_e_l_=_F_o_l_l_o_w_%_2_0_%_4_0_p_e_r_m_i_t___i_o_&_s_t_y_l_e_=_s_o_c_i_a_l_]## What is OPAL? OPAL is an
 administration layer for Policy Engines such as _O_p_e_n_ _P_o_l_i_c_y_ _A_g_e_n_t_ _(_O_P_A_), and
```

### Comparing `opal_client-0.7.6/opal_client/callbacks/api.py` & `opal-client-0.7.7/opal_client/callbacks/api.py`

 * *Files identical despite different names*

### Comparing `opal_client-0.7.6/opal_client/callbacks/register.py` & `opal-client-0.7.7/opal_client/callbacks/register.py`

 * *Files identical despite different names*

### Comparing `opal_client-0.7.6/opal_client/callbacks/reporter.py` & `opal-client-0.7.7/opal_client/callbacks/reporter.py`

 * *Files identical despite different names*

### Comparing `opal_client-0.7.6/opal_client/cli.py` & `opal-client-0.7.7/opal_client/cli.py`

 * *Files identical despite different names*

### Comparing `opal_client-0.7.6/opal_client/client.py` & `opal-client-0.7.7/opal_client/client.py`

 * *Files identical despite different names*

### Comparing `opal_client-0.7.6/opal_client/config.py` & `opal-client-0.7.7/opal_client/config.py`

 * *Files identical despite different names*

### Comparing `opal_client-0.7.6/opal_client/data/api.py` & `opal-client-0.7.7/opal_client/data/api.py`

 * *Files identical despite different names*

### Comparing `opal_client-0.7.6/opal_client/data/fetcher.py` & `opal-client-0.7.7/opal_client/data/fetcher.py`

 * *Files identical despite different names*

### Comparing `opal_client-0.7.6/opal_client/data/rpc.py` & `opal-client-0.7.7/opal_client/data/rpc.py`

 * *Files identical despite different names*

### Comparing `opal_client-0.7.6/opal_client/data/updater.py` & `opal-client-0.7.7/opal_client/data/updater.py`

 * *Files identical despite different names*

### Comparing `opal_client-0.7.6/opal_client/engine/healthcheck/opal.rego` & `opal-client-0.7.7/opal_client/engine/healthcheck/opal.rego`

 * *Files identical despite different names*

### Comparing `opal_client-0.7.6/opal_client/engine/logger.py` & `opal-client-0.7.7/opal_client/engine/logger.py`

 * *Files identical despite different names*

### Comparing `opal_client-0.7.6/opal_client/engine/options.py` & `opal-client-0.7.7/opal_client/engine/options.py`

 * *Files identical despite different names*

### Comparing `opal_client-0.7.6/opal_client/engine/runner.py` & `opal-client-0.7.7/opal_client/engine/runner.py`

 * *Files identical despite different names*

### Comparing `opal_client-0.7.6/opal_client/limiter.py` & `opal-client-0.7.7/opal_client/limiter.py`

 * *Files identical despite different names*

### Comparing `opal_client-0.7.6/opal_client/policy/fetcher.py` & `opal-client-0.7.7/opal_client/policy/fetcher.py`

 * *Files identical despite different names*

### Comparing `opal_client-0.7.6/opal_client/policy/options.py` & `opal-client-0.7.7/opal_client/policy/options.py`

 * *Files identical despite different names*

### Comparing `opal_client-0.7.6/opal_client/policy/topics.py` & `opal-client-0.7.7/opal_client/policy/topics.py`

 * *Files identical despite different names*

### Comparing `opal_client-0.7.6/opal_client/policy/updater.py` & `opal-client-0.7.7/opal_client/policy/updater.py`

 * *Files identical despite different names*

### Comparing `opal_client-0.7.6/opal_client/policy_store/api.py` & `opal-client-0.7.7/opal_client/policy_store/api.py`

 * *Files identical despite different names*

### Comparing `opal_client-0.7.6/opal_client/policy_store/base_policy_store_client.py` & `opal-client-0.7.7/opal_client/policy_store/base_policy_store_client.py`

 * *Files identical despite different names*

### Comparing `opal_client-0.7.6/opal_client/policy_store/cedar_client.py` & `opal-client-0.7.7/opal_client/policy_store/cedar_client.py`

 * *Files identical despite different names*

### Comparing `opal_client-0.7.6/opal_client/policy_store/mock_policy_store_client.py` & `opal-client-0.7.7/opal_client/policy_store/mock_policy_store_client.py`

 * *Files identical despite different names*

### Comparing `opal_client-0.7.6/opal_client/policy_store/opa_client.py` & `opal-client-0.7.7/opal_client/policy_store/opa_client.py`

 * *Files identical despite different names*

### Comparing `opal_client-0.7.6/opal_client/policy_store/policy_store_client_factory.py` & `opal-client-0.7.7/opal_client/policy_store/policy_store_client_factory.py`

 * *Files identical despite different names*

### Comparing `opal_client-0.7.6/opal_client/policy_store/schemas.py` & `opal-client-0.7.7/opal_client/policy_store/schemas.py`

 * *Files identical despite different names*

### Comparing `opal_client-0.7.6/opal_client/tests/data_updater_test.py` & `opal-client-0.7.7/opal_client/tests/data_updater_test.py`

 * *Files identical despite different names*

### Comparing `opal_client-0.7.6/opal_client/tests/opa_client_test.py` & `opal-client-0.7.7/opal_client/tests/opa_client_test.py`

 * *Files identical despite different names*

### Comparing `opal_client-0.7.6/opal_client/tests/server_to_client_intergation_test.py` & `opal-client-0.7.7/opal_client/tests/server_to_client_intergation_test.py`

 * *Files identical despite different names*

### Comparing `opal_client-0.7.6/opal_client/utils.py` & `opal-client-0.7.7/opal_client/utils.py`

 * *Files identical despite different names*

### Comparing `opal_client-0.7.6/opal_client.egg-info/PKG-INFO` & `opal-client-0.7.7/opal_client.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opal-client
-Version: 0.7.6
+Version: 0.7.7
 Summary: OPAL is an administration layer for Open Policy Agent (OPA), detecting changes to both policy and data and pushing live updates to your agents. The opal-client is deployed alongside a policy-store (e.g: OPA), keeping it up-to-date, by connecting to an opal-server and subscribing to pub/sub updates for policy and policy data changes.
 Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen
 Author-email: or@permit.io
 License: Apache 2.0
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
@@ -14,33 +14,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: aiofiles<1,>=0.8.0
-Requires-Dist: aiohttp<4,>=3.9.2
-Requires-Dist: psutil<6,>=5.9.1
-Requires-Dist: tenacity<9,>=8.0.1
-Requires-Dist: websockets<11,>=10.3
-Requires-Dist: dpath<3,>=2.1.5
-Requires-Dist: jsonpatch<2,>=1.33
-Requires-Dist: opal-common==0.7.6
-Requires-Dist: idna<4,>=3.3
-Requires-Dist: typer<1,>=0.4.1
-Requires-Dist: fastapi<1,>=0.109.1
-Requires-Dist: fastapi_websocket_pubsub==0.3.7
-Requires-Dist: fastapi_websocket_rpc<1,>=0.1.21
-Requires-Dist: gunicorn<23,>=22.0.0
-Requires-Dist: pydantic[email]<2,>=1.9.1
-Requires-Dist: typing-extensions; python_version < "3.8"
-Requires-Dist: uvicorn[standard]<1,>=0.17.6
-Requires-Dist: fastapi-utils<1,>=0.2.1
-Requires-Dist: setuptools>=65.5.1
 
 <p  align="center">
  <img src="https://github.com/permitio/opal/assets/4082578/4e21f85f-30ab-43e2-92de-b82f78888c71" height=170 alt="opal" border="0" />
 </p>
 <h1 align="center">
 ⚡OPAL⚡
 </h1>
```

#### html2text {}

```diff
@@ -1,32 +1,22 @@
-Metadata-Version: 2.1 Name: opal-client Version: 0.7.6 Summary: OPAL is an
+Metadata-Version: 2.1 Name: opal-client Version: 0.7.7 Summary: OPAL is an
 administration layer for Open Policy Agent (OPA), detecting changes to both
 policy and data and pushing live updates to your agents. The opal-client is
 deployed alongside a policy-store (e.g: OPA), keeping it up-to-date, by
 connecting to an opal-server and subscribing to pub/sub updates for policy and
 policy data changes. Home-page: https://github.com/permitio/opal Author: Or
 Weis, Asaf Cohen Author-email: or@permit.io License: Apache 2.0 Classifier:
 Operating System :: OS Independent Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI Requires-Python: >=3.9
-Description-Content-Type: text/markdown Requires-Dist: aiofiles<1,>=0.8.0
-Requires-Dist: aiohttp<4,>=3.9.2 Requires-Dist: psutil<6,>=5.9.1 Requires-Dist:
-tenacity<9,>=8.0.1 Requires-Dist: websockets<11,>=10.3 Requires-Dist:
-dpath<3,>=2.1.5 Requires-Dist: jsonpatch<2,>=1.33 Requires-Dist: opal-
-common==0.7.6 Requires-Dist: idna<4,>=3.3 Requires-Dist: typer<1,>=0.4.1
-Requires-Dist: fastapi<1,>=0.109.1 Requires-Dist:
-fastapi_websocket_pubsub==0.3.7 Requires-Dist: fastapi_websocket_rpc<1,>=0.1.21
-Requires-Dist: gunicorn<23,>=22.0.0 Requires-Dist: pydantic[email]<2,>=1.9.1
-Requires-Dist: typing-extensions; python_version < "3.8" Requires-Dist: uvicorn
-[standard]<1,>=0.17.6 Requires-Dist: fastapi-utils<1,>=0.2.1 Requires-Dist:
-setuptools>=65.5.1
+Description-Content-Type: text/markdown
                                     [opal]
                            ************ ?â??¡OOPPAALL?â??¡ ************
                  ********** OOppeenn PPoolliiccyy AAddmmiinniissttrraattiioonn LLaayyeerr **********
 _[_T_e_s_t_s_]_[_P_a_c_k_a_g_e_]_[_P_a_c_k_a_g_e_]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_c_k_e_r_ _p_u_l_l_s_]_[_J_o_i_n_ _o_u_r_ _S_l_a_c_k_!_]_[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_t_w_i_t_t_e_r_/_f_o_l_l_o_w_/
 _p_e_r_m_i_t___i_o_?_l_a_b_e_l_=_F_o_l_l_o_w_%_2_0_%_4_0_p_e_r_m_i_t___i_o_&_s_t_y_l_e_=_s_o_c_i_a_l_]## What is OPAL? OPAL is an
 administration layer for Policy Engines such as _O_p_e_n_ _P_o_l_i_c_y_ _A_g_e_n_t_ _(_O_P_A_), and
```

### Comparing `opal_client-0.7.6/opal_client.egg-info/SOURCES.txt` & `opal-client-0.7.7/opal_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opal_client-0.7.6/setup.py` & `opal-client-0.7.7/setup.py`

 * *Files identical despite different names*

