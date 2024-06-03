# Comparing `tmp/opal_common-0.7.6.tar.gz` & `tmp/opal-common-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opal_common-0.7.6.tar", last modified: Tue Apr 30 17:18:48 2024, max compression
+gzip compressed data, was "opal-common-0.7.7.tar", last modified: Mon Jun  3 13:38:16 2024, max compression
```

## Comparing `opal_common-0.7.6.tar` & `opal-common-0.7.7.tar`

### file list

```diff
@@ -1,123 +1,122 @@
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.529060 opal_common-0.7.6/
--rw-r--r--   0 roekatz    (501) staff       (20)    10034 2024-04-30 17:18:48.528689 opal_common-0.7.6/PKG-INFO
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.515323 opal_common-0.7.6/opal_common/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3574 2024-04-30 13:01:51.000000 opal_common-0.7.6/opal_common/async_utils.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.517116 opal_common-0.7.6/opal_common/authentication/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/authentication/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1477 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/authentication/authz.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3329 2024-04-30 13:01:51.000000 opal_common-0.7.6/opal_common/authentication/casting.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4990 2023-10-04 11:07:26.000000 opal_common-0.7.6/opal_common/authentication/deps.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4669 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/authentication/signer.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.517557 opal_common-0.7.6/opal_common/authentication/tests/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/authentication/tests/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)    17336 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/authentication/tests/jwt_signer_test.py
--rw-r--r--   0 roekatz    (501) staff       (20)      950 2024-04-30 16:48:47.000000 opal_common-0.7.6/opal_common/authentication/types.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4225 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/authentication/verifier.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.518771 opal_common-0.7.6/opal_common/cli/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/cli/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     6657 2023-05-29 10:10:14.000000 opal_common-0.7.6/opal_common/cli/commands.py
--rw-r--r--   0 roekatz    (501) staff       (20)      702 2024-03-19 14:53:02.000000 opal_common-0.7.6/opal_common/cli/docs.py
--rw-r--r--   0 roekatz    (501) staff       (20)      167 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/cli/typer_app.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.519354 opal_common-0.7.6/opal_common/confi/
--rw-r--r--   0 roekatz    (501) staff       (20)       21 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/confi/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2278 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/confi/cli.py
--rw-r--r--   0 roekatz    (501) staff       (20)    14044 2024-03-19 14:53:02.000000 opal_common-0.7.6/opal_common/confi/confi.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2836 2024-03-19 14:53:02.000000 opal_common-0.7.6/opal_common/confi/types.py
--rw-r--r--   0 roekatz    (501) staff       (20)     7139 2024-03-19 14:53:02.000000 opal_common-0.7.6/opal_common/config.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1492 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/corn_utils.py
--rw-r--r--   0 roekatz    (501) staff       (20)     6045 2024-03-19 14:53:02.000000 opal_common-0.7.6/opal_common/emport.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.519868 opal_common-0.7.6/opal_common/engine/
--rw-r--r--   0 roekatz    (501) staff       (20)       90 2023-05-29 10:10:14.000000 opal_common-0.7.6/opal_common/engine/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)      576 2023-05-29 10:10:14.000000 opal_common-0.7.6/opal_common/engine/parsing.py
--rw-r--r--   0 roekatz    (501) staff       (20)      593 2023-05-29 10:10:14.000000 opal_common-0.7.6/opal_common/engine/paths.py
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2023-05-29 10:10:14.000000 opal_common-0.7.6/opal_common/engine/py.typed
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.520471 opal_common-0.7.6/opal_common/fetcher/
--rw-r--r--   0 roekatz    (501) staff       (20)      143 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/fetcher/__init__.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.521104 opal_common-0.7.6/opal_common/fetcher/engine/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/fetcher/engine/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2653 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/fetcher/engine/base_fetching_engine.py
--rw-r--r--   0 roekatz    (501) staff       (20)      296 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/fetcher/engine/core_callbacks.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1536 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/fetcher/engine/fetch_worker.py
--rw-r--r--   0 roekatz    (501) staff       (20)     8602 2024-03-19 14:53:02.000000 opal_common-0.7.6/opal_common/fetcher/engine/fetching_engine.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1191 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/fetcher/events.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2548 2024-03-26 18:21:06.000000 opal_common-0.7.6/opal_common/fetcher/fetch_provider.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3030 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/fetcher/fetcher_register.py
--rw-r--r--   0 roekatz    (501) staff       (20)      116 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/fetcher/logger.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.521522 opal_common-0.7.6/opal_common/fetcher/providers/
--rw-r--r--   0 roekatz    (501) staff       (20)       67 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/fetcher/providers/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1710 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/fetcher/providers/fastapi_rpc_fetch_provider.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3570 2024-02-28 15:15:55.000000 opal_common-0.7.6/opal_common/fetcher/providers/http_fetch_provider.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.522064 opal_common-0.7.6/opal_common/fetcher/tests/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/fetcher/tests/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1918 2024-03-19 14:53:02.000000 opal_common-0.7.6/opal_common/fetcher/tests/failure_handler_test.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4289 2024-03-19 14:53:02.000000 opal_common-0.7.6/opal_common/fetcher/tests/http_fetch_test.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2141 2024-03-19 14:53:02.000000 opal_common-0.7.6/opal_common/fetcher/tests/rpc_fetch_test.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.523494 opal_common-0.7.6/opal_common/git/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/git/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     5461 2023-05-29 10:10:14.000000 opal_common-0.7.6/opal_common/git/branch_tracker.py
--rw-r--r--   0 roekatz    (501) staff       (20)    15724 2024-03-19 14:53:02.000000 opal_common-0.7.6/opal_common/git/bundle_maker.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1887 2023-05-29 10:10:14.000000 opal_common-0.7.6/opal_common/git/bundle_utils.py
--rw-r--r--   0 roekatz    (501) staff       (20)     8684 2023-05-29 10:10:14.000000 opal_common-0.7.6/opal_common/git/commit_viewer.py
--rw-r--r--   0 roekatz    (501) staff       (20)     7948 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/git/diff_viewer.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1580 2023-05-29 10:10:14.000000 opal_common-0.7.6/opal_common/git/env.py
--rw-r--r--   0 roekatz    (501) staff       (20)      299 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/git/exceptions.py
--rw-r--r--   0 roekatz    (501) staff       (20)     8535 2023-05-29 10:10:14.000000 opal_common-0.7.6/opal_common/git/repo_cloner.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4237 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/git/tar_file_to_local_git_extractor.py
--rw-r--r--   0 roekatz    (501) staff       (20)      182 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/http.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1908 2024-03-19 14:53:02.000000 opal_common-0.7.6/opal_common/logger.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.524285 opal_common-0.7.6/opal_common/logging/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/logging/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)      412 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/logging/decorators.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1166 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/logging/filter.py
--rw-r--r--   0 roekatz    (501) staff       (20)      616 2024-03-19 14:53:02.000000 opal_common-0.7.6/opal_common/logging/formatter.py
--rw-r--r--   0 roekatz    (501) staff       (20)      700 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/logging/intercept.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1355 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/logging/thirdparty.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3520 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/middleware.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.524642 opal_common-0.7.6/opal_common/monitoring/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2024-03-19 14:53:02.000000 opal_common-0.7.6/opal_common/monitoring/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1546 2024-03-19 14:53:02.000000 opal_common-0.7.6/opal_common/monitoring/apm.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1446 2024-03-19 14:53:02.000000 opal_common-0.7.6/opal_common/monitoring/metrics.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4067 2023-05-29 10:10:14.000000 opal_common-0.7.6/opal_common/paths.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.525734 opal_common-0.7.6/opal_common/schemas/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/schemas/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     7140 2024-03-19 14:53:02.000000 opal_common-0.7.6/opal_common/schemas/data.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1387 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/schemas/policy.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1767 2023-05-29 10:10:14.000000 opal_common-0.7.6/opal_common/schemas/policy_source.py
--rw-r--r--   0 roekatz    (501) staff       (20)      508 2023-04-04 11:14:44.000000 opal_common-0.7.6/opal_common/schemas/scopes.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1573 2023-05-23 16:26:33.000000 opal_common-0.7.6/opal_common/schemas/security.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2398 2023-07-17 14:14:01.000000 opal_common-0.7.6/opal_common/schemas/store.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1438 2023-05-29 10:10:14.000000 opal_common-0.7.6/opal_common/schemas/webhook.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.526099 opal_common-0.7.6/opal_common/security/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/security/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)      799 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/security/sslcontext.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3294 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/security/tarsafe.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.526622 opal_common-0.7.6/opal_common/sources/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/sources/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)    11747 2024-04-30 12:59:10.000000 opal_common-0.7.6/opal_common/sources/api_policy_source.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4283 2023-05-29 10:10:14.000000 opal_common-0.7.6/opal_common/sources/base_policy_source.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4238 2023-05-29 10:10:14.000000 opal_common-0.7.6/opal_common/sources/git_policy_source.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.527045 opal_common-0.7.6/opal_common/synchronization/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/synchronization/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1307 2023-10-04 11:07:26.000000 opal_common-0.7.6/opal_common/synchronization/expiring_redis_lock.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2990 2023-05-29 10:10:14.000000 opal_common-0.7.6/opal_common/synchronization/named_lock.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.527590 opal_common-0.7.6/opal_common/tests/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/tests/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     9622 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/tests/path_utils_test.py
--rw-r--r--   0 roekatz    (501) staff       (20)      539 2024-03-19 14:53:02.000000 opal_common-0.7.6/opal_common/tests/test_utils.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1223 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/tests/url_utils_test.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.528117 opal_common-0.7.6/opal_common/topics/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/topics/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2371 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/topics/listener.py
--rw-r--r--   0 roekatz    (501) staff       (20)     7127 2024-03-19 14:53:02.000000 opal_common-0.7.6/opal_common/topics/publisher.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1054 2023-05-29 10:10:14.000000 opal_common-0.7.6/opal_common/topics/utils.py
--rw-r--r--   0 roekatz    (501) staff       (20)      988 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/urls.py
--rw-r--r--   0 roekatz    (501) staff       (20)     8578 2024-04-30 12:59:10.000000 opal_common-0.7.6/opal_common/utils.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.528311 opal_common-0.7.6/opal_common.egg-info/
--rw-r--r--   0 roekatz    (501) staff       (20)    10034 2024-04-30 17:18:48.000000 opal_common-0.7.6/opal_common.egg-info/PKG-INFO
--rw-r--r--   0 roekatz    (501) staff       (20)     3366 2024-04-30 17:18:48.000000 opal_common-0.7.6/opal_common.egg-info/SOURCES.txt
--rw-r--r--   0 roekatz    (501) staff       (20)        1 2024-04-30 17:18:48.000000 opal_common-0.7.6/opal_common.egg-info/dependency_links.txt
--rw-r--r--   0 roekatz    (501) staff       (20)      515 2024-04-30 17:18:48.000000 opal_common-0.7.6/opal_common.egg-info/requires.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       12 2024-04-30 17:18:48.000000 opal_common-0.7.6/opal_common.egg-info/top_level.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       38 2024-04-30 17:18:48.529104 opal_common-0.7.6/setup.cfg
--rw-r--r--   0 roekatz    (501) staff       (20)     2653 2024-04-30 13:01:51.000000 opal_common-0.7.6/setup.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:16.612259 opal-common-0.7.7/
+-rw-r--r--   0 asafc      (501) staff       (20)     9177 2024-06-03 13:38:16.611899 opal-common-0.7.7/PKG-INFO
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:16.599629 opal-common-0.7.7/opal_common/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3574 2024-05-29 13:03:42.000000 opal-common-0.7.7/opal_common/async_utils.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:16.601335 opal-common-0.7.7/opal_common/authentication/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/authentication/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1477 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/authentication/authz.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3329 2024-05-29 13:03:42.000000 opal-common-0.7.7/opal_common/authentication/casting.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4990 2023-10-24 07:43:19.000000 opal-common-0.7.7/opal_common/authentication/deps.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4669 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/authentication/signer.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:16.601630 opal-common-0.7.7/opal_common/authentication/tests/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/authentication/tests/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)    17336 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/authentication/tests/jwt_signer_test.py
+-rw-r--r--   0 asafc      (501) staff       (20)      950 2024-05-29 13:03:42.000000 opal-common-0.7.7/opal_common/authentication/types.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4225 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/authentication/verifier.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:16.602220 opal-common-0.7.7/opal_common/cli/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/cli/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6657 2023-05-10 06:45:11.000000 opal-common-0.7.7/opal_common/cli/commands.py
+-rw-r--r--   0 asafc      (501) staff       (20)      702 2024-03-17 08:56:30.000000 opal-common-0.7.7/opal_common/cli/docs.py
+-rw-r--r--   0 asafc      (501) staff       (20)      167 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/cli/typer_app.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:16.602811 opal-common-0.7.7/opal_common/confi/
+-rw-r--r--   0 asafc      (501) staff       (20)       21 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/confi/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2278 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/confi/cli.py
+-rw-r--r--   0 asafc      (501) staff       (20)    14044 2024-03-17 08:56:30.000000 opal-common-0.7.7/opal_common/confi/confi.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2836 2024-03-17 08:56:30.000000 opal-common-0.7.7/opal_common/confi/types.py
+-rw-r--r--   0 asafc      (501) staff       (20)     7403 2024-06-03 13:34:45.000000 opal-common-0.7.7/opal_common/config.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1492 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/corn_utils.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6045 2024-03-17 08:56:30.000000 opal-common-0.7.7/opal_common/emport.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:16.603241 opal-common-0.7.7/opal_common/engine/
+-rw-r--r--   0 asafc      (501) staff       (20)       90 2023-05-10 17:44:40.000000 opal-common-0.7.7/opal_common/engine/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)      576 2023-05-10 17:44:40.000000 opal-common-0.7.7/opal_common/engine/parsing.py
+-rw-r--r--   0 asafc      (501) staff       (20)      593 2023-05-10 17:44:40.000000 opal-common-0.7.7/opal_common/engine/paths.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:16.603862 opal-common-0.7.7/opal_common/fetcher/
+-rw-r--r--   0 asafc      (501) staff       (20)      143 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/fetcher/__init__.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:16.604449 opal-common-0.7.7/opal_common/fetcher/engine/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/fetcher/engine/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2653 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/fetcher/engine/base_fetching_engine.py
+-rw-r--r--   0 asafc      (501) staff       (20)      296 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/fetcher/engine/core_callbacks.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1536 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/fetcher/engine/fetch_worker.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8602 2024-03-17 08:56:30.000000 opal-common-0.7.7/opal_common/fetcher/engine/fetching_engine.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1191 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/fetcher/events.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2548 2023-05-10 06:45:11.000000 opal-common-0.7.7/opal_common/fetcher/fetch_provider.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3030 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/fetcher/fetcher_register.py
+-rw-r--r--   0 asafc      (501) staff       (20)      116 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/fetcher/logger.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:16.604869 opal-common-0.7.7/opal_common/fetcher/providers/
+-rw-r--r--   0 asafc      (501) staff       (20)       67 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/fetcher/providers/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1710 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/fetcher/providers/fastapi_rpc_fetch_provider.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4201 2024-06-03 13:34:45.000000 opal-common-0.7.7/opal_common/fetcher/providers/http_fetch_provider.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:16.605385 opal-common-0.7.7/opal_common/fetcher/tests/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/fetcher/tests/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1918 2024-03-17 08:56:30.000000 opal-common-0.7.7/opal_common/fetcher/tests/failure_handler_test.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4289 2024-03-17 08:56:30.000000 opal-common-0.7.7/opal_common/fetcher/tests/http_fetch_test.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2141 2024-03-17 08:56:30.000000 opal-common-0.7.7/opal_common/fetcher/tests/rpc_fetch_test.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:16.606844 opal-common-0.7.7/opal_common/git/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/git/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5461 2023-02-01 11:46:28.000000 opal-common-0.7.7/opal_common/git/branch_tracker.py
+-rw-r--r--   0 asafc      (501) staff       (20)    15724 2024-03-17 08:56:30.000000 opal-common-0.7.7/opal_common/git/bundle_maker.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1887 2023-05-10 06:45:11.000000 opal-common-0.7.7/opal_common/git/bundle_utils.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8684 2023-05-10 06:45:11.000000 opal-common-0.7.7/opal_common/git/commit_viewer.py
+-rw-r--r--   0 asafc      (501) staff       (20)     7948 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/git/diff_viewer.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1580 2023-02-01 11:46:28.000000 opal-common-0.7.7/opal_common/git/env.py
+-rw-r--r--   0 asafc      (501) staff       (20)      299 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/git/exceptions.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8535 2023-05-10 06:45:11.000000 opal-common-0.7.7/opal_common/git/repo_cloner.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4237 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/git/tar_file_to_local_git_extractor.py
+-rw-r--r--   0 asafc      (501) staff       (20)      382 2024-06-03 13:34:45.000000 opal-common-0.7.7/opal_common/http.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1908 2024-03-17 08:56:30.000000 opal-common-0.7.7/opal_common/logger.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:16.607664 opal-common-0.7.7/opal_common/logging/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/logging/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)      412 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/logging/decorators.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1166 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/logging/filter.py
+-rw-r--r--   0 asafc      (501) staff       (20)      616 2024-03-17 08:56:30.000000 opal-common-0.7.7/opal_common/logging/formatter.py
+-rw-r--r--   0 asafc      (501) staff       (20)      700 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/logging/intercept.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1355 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/logging/thirdparty.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3520 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/middleware.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:16.608003 opal-common-0.7.7/opal_common/monitoring/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2024-03-17 08:56:30.000000 opal-common-0.7.7/opal_common/monitoring/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1546 2024-03-17 08:56:30.000000 opal-common-0.7.7/opal_common/monitoring/apm.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1446 2024-03-17 08:56:30.000000 opal-common-0.7.7/opal_common/monitoring/metrics.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4067 2023-05-10 06:45:11.000000 opal-common-0.7.7/opal_common/paths.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:16.608974 opal-common-0.7.7/opal_common/schemas/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/schemas/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     7140 2024-03-17 08:56:30.000000 opal-common-0.7.7/opal_common/schemas/data.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1387 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/schemas/policy.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1767 2023-02-24 20:59:56.000000 opal-common-0.7.7/opal_common/schemas/policy_source.py
+-rw-r--r--   0 asafc      (501) staff       (20)      508 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/schemas/scopes.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1573 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/schemas/security.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2398 2023-09-11 17:35:10.000000 opal-common-0.7.7/opal_common/schemas/store.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1438 2023-05-10 06:45:11.000000 opal-common-0.7.7/opal_common/schemas/webhook.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:16.609379 opal-common-0.7.7/opal_common/security/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/security/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)      799 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/security/sslcontext.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3294 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/security/tarsafe.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:16.609988 opal-common-0.7.7/opal_common/sources/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/sources/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)    11747 2024-05-29 13:03:42.000000 opal-common-0.7.7/opal_common/sources/api_policy_source.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4283 2023-05-10 06:45:11.000000 opal-common-0.7.7/opal_common/sources/base_policy_source.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4238 2023-05-10 06:45:11.000000 opal-common-0.7.7/opal_common/sources/git_policy_source.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:16.610367 opal-common-0.7.7/opal_common/synchronization/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/synchronization/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1307 2023-10-24 07:43:19.000000 opal-common-0.7.7/opal_common/synchronization/expiring_redis_lock.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2990 2023-05-10 06:45:11.000000 opal-common-0.7.7/opal_common/synchronization/named_lock.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:16.611095 opal-common-0.7.7/opal_common/tests/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/tests/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     9622 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/tests/path_utils_test.py
+-rw-r--r--   0 asafc      (501) staff       (20)      539 2024-03-17 08:56:30.000000 opal-common-0.7.7/opal_common/tests/test_utils.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1223 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/tests/url_utils_test.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:16.611695 opal-common-0.7.7/opal_common/topics/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/topics/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2371 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/topics/listener.py
+-rw-r--r--   0 asafc      (501) staff       (20)     7127 2024-03-17 08:56:30.000000 opal-common-0.7.7/opal_common/topics/publisher.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1054 2023-05-10 06:45:11.000000 opal-common-0.7.7/opal_common/topics/utils.py
+-rw-r--r--   0 asafc      (501) staff       (20)      988 2022-10-01 21:13:25.000000 opal-common-0.7.7/opal_common/urls.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8578 2024-05-29 13:03:42.000000 opal-common-0.7.7/opal_common/utils.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:16.600326 opal-common-0.7.7/opal_common.egg-info/
+-rw-r--r--   0 asafc      (501) staff       (20)     9177 2024-06-03 13:38:16.000000 opal-common-0.7.7/opal_common.egg-info/PKG-INFO
+-rw-r--r--   0 asafc      (501) staff       (20)     3338 2024-06-03 13:38:16.000000 opal-common-0.7.7/opal_common.egg-info/SOURCES.txt
+-rw-r--r--   0 asafc      (501) staff       (20)        1 2024-06-03 13:38:16.000000 opal-common-0.7.7/opal_common.egg-info/dependency_links.txt
+-rw-r--r--   0 asafc      (501) staff       (20)      529 2024-06-03 13:38:16.000000 opal-common-0.7.7/opal_common.egg-info/requires.txt
+-rw-r--r--   0 asafc      (501) staff       (20)       12 2024-06-03 13:38:16.000000 opal-common-0.7.7/opal_common.egg-info/top_level.txt
+-rw-r--r--   0 asafc      (501) staff       (20)       38 2024-06-03 13:38:16.612328 opal-common-0.7.7/setup.cfg
+-rw-r--r--   0 asafc      (501) staff       (20)     2653 2024-05-29 13:03:42.000000 opal-common-0.7.7/setup.py
```

### Comparing `opal_common-0.7.6/PKG-INFO` & `opal-common-0.7.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opal-common
-Version: 0.7.6
+Version: 0.7.7
 Summary: OPAL is an administration layer for Open Policy Agent (OPA), detecting changes to both policy and data and pushing live updates to your agents. opal-common contains common code used by both opal-client and opal-server.
 Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen
 Author-email: or@permit.io
 License: Apache 2.0
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
@@ -14,37 +14,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: aiohttp<4,>=3.9.2
-Requires-Dist: click<9,>=8.1.3
-Requires-Dist: cryptography<43,>=42.0.4
-Requires-Dist: gitpython<4,>=3.1.32
-Requires-Dist: loguru<1,>=0.6.0
-Requires-Dist: pyjwt[crypto]<3,>=2.4.0
-Requires-Dist: python-decouple<4,>=3.6
-Requires-Dist: tenacity<9,>=8.0.1
-Requires-Dist: datadog<1,>=0.44.0
-Requires-Dist: ddtrace<3,>=2.8.1
-Requires-Dist: certifi>=2023.7.22
-Requires-Dist: requests>=2.31.0
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
@@ -1,32 +1,20 @@
-Metadata-Version: 2.1 Name: opal-common Version: 0.7.6 Summary: OPAL is an
+Metadata-Version: 2.1 Name: opal-common Version: 0.7.7 Summary: OPAL is an
 administration layer for Open Policy Agent (OPA), detecting changes to both
 policy and data and pushing live updates to your agents. opal-common contains
 common code used by both opal-client and opal-server. Home-page: https://
 github.com/permitio/opal Author: Or Weis, Asaf Cohen Author-email: or@permit.io
 License: Apache 2.0 Classifier: Operating System :: OS Independent Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: Topic :: Internet :: WWW/
 HTTP :: HTTP Servers Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
-Requires-Python: >=3.9 Description-Content-Type: text/markdown Requires-Dist:
-aiohttp<4,>=3.9.2 Requires-Dist: click<9,>=8.1.3 Requires-Dist:
-cryptography<43,>=42.0.4 Requires-Dist: gitpython<4,>=3.1.32 Requires-Dist:
-loguru<1,>=0.6.0 Requires-Dist: pyjwt[crypto]<3,>=2.4.0 Requires-Dist: python-
-decouple<4,>=3.6 Requires-Dist: tenacity<9,>=8.0.1 Requires-Dist:
-datadog<1,>=0.44.0 Requires-Dist: ddtrace<3,>=2.8.1 Requires-Dist:
-certifi>=2023.7.22 Requires-Dist: requests>=2.31.0 Requires-Dist: idna<4,>=3.3
-Requires-Dist: typer<1,>=0.4.1 Requires-Dist: fastapi<1,>=0.109.1 Requires-
-Dist: fastapi_websocket_pubsub==0.3.7 Requires-Dist:
-fastapi_websocket_rpc<1,>=0.1.21 Requires-Dist: gunicorn<23,>=22.0.0 Requires-
-Dist: pydantic[email]<2,>=1.9.1 Requires-Dist: typing-extensions;
-python_version < "3.8" Requires-Dist: uvicorn[standard]<1,>=0.17.6 Requires-
-Dist: fastapi-utils<1,>=0.2.1 Requires-Dist: setuptools>=65.5.1
+Requires-Python: >=3.9 Description-Content-Type: text/markdown
                                     [opal]
                            ************ ?â??¡OOPPAALL?â??¡ ************
                  ********** OOppeenn PPoolliiccyy AAddmmiinniissttrraattiioonn LLaayyeerr **********
 _[_T_e_s_t_s_]_[_P_a_c_k_a_g_e_]_[_P_a_c_k_a_g_e_]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_c_k_e_r_ _p_u_l_l_s_]_[_J_o_i_n_ _o_u_r_ _S_l_a_c_k_!_]_[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_t_w_i_t_t_e_r_/_f_o_l_l_o_w_/
 _p_e_r_m_i_t___i_o_?_l_a_b_e_l_=_F_o_l_l_o_w_%_2_0_%_4_0_p_e_r_m_i_t___i_o_&_s_t_y_l_e_=_s_o_c_i_a_l_]## What is OPAL? OPAL is an
 administration layer for Policy Engines such as _O_p_e_n_ _P_o_l_i_c_y_ _A_g_e_n_t_ _(_O_P_A_), and
```

### Comparing `opal_common-0.7.6/opal_common/async_utils.py` & `opal-common-0.7.7/opal_common/async_utils.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/authentication/authz.py` & `opal-common-0.7.7/opal_common/authentication/authz.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/authentication/casting.py` & `opal-common-0.7.7/opal_common/authentication/casting.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/authentication/deps.py` & `opal-common-0.7.7/opal_common/authentication/deps.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/authentication/signer.py` & `opal-common-0.7.7/opal_common/authentication/signer.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/authentication/tests/jwt_signer_test.py` & `opal-common-0.7.7/opal_common/authentication/tests/jwt_signer_test.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/authentication/types.py` & `opal-common-0.7.7/opal_common/authentication/types.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/authentication/verifier.py` & `opal-common-0.7.7/opal_common/authentication/verifier.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/cli/commands.py` & `opal-common-0.7.7/opal_common/cli/commands.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/cli/docs.py` & `opal-common-0.7.7/opal_common/cli/docs.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/confi/cli.py` & `opal-common-0.7.7/opal_common/confi/cli.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/confi/confi.py` & `opal-common-0.7.7/opal_common/confi/confi.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/confi/types.py` & `opal-common-0.7.7/opal_common/confi/types.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/config.py` & `opal-common-0.7.7/opal_common/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -165,10 +165,16 @@
 
     # optional APM tracing with datadog
     ENABLE_DATADOG_APM = confi.bool(
         "ENABLE_DATADOG_APM",
         False,
         description="Set if OPAL server should enable tracing with datadog APM",
     )
+    HTTP_FETCHER_PROVIDER_CLIENT = confi.str(
+        "HTTP_FETCHER_PROVIDER_CLIENT",
+        "aiohttp",
+        description="The client to use for fetching data, can be either aiohttp or httpx."
+        "if provided different value, aiohttp will be used.",
+    )
 
 
 opal_common_config = OpalCommonConfig(prefix="OPAL_")
```

### Comparing `opal_common-0.7.6/opal_common/corn_utils.py` & `opal-common-0.7.7/opal_common/corn_utils.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/emport.py` & `opal-common-0.7.7/opal_common/emport.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/engine/parsing.py` & `opal-common-0.7.7/opal_common/engine/parsing.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/engine/paths.py` & `opal-common-0.7.7/opal_common/engine/paths.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/fetcher/engine/base_fetching_engine.py` & `opal-common-0.7.7/opal_common/fetcher/engine/base_fetching_engine.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/fetcher/engine/fetch_worker.py` & `opal-common-0.7.7/opal_common/fetcher/engine/fetch_worker.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/fetcher/engine/fetching_engine.py` & `opal-common-0.7.7/opal_common/fetcher/engine/fetching_engine.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/fetcher/events.py` & `opal-common-0.7.7/opal_common/fetcher/events.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/fetcher/fetch_provider.py` & `opal-common-0.7.7/opal_common/fetcher/fetch_provider.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/fetcher/fetcher_register.py` & `opal-common-0.7.7/opal_common/fetcher/fetcher_register.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/fetcher/providers/fastapi_rpc_fetch_provider.py` & `opal-common-0.7.7/opal_common/fetcher/providers/fastapi_rpc_fetch_provider.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/fetcher/providers/http_fetch_provider.py` & `opal-common-0.7.7/opal_common/fetcher/providers/http_fetch_provider.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Simple HTTP get data fetcher using requests supports."""
 
 from enum import Enum
-from typing import Any
+from typing import Any, Union, cast
 
+import httpx
 from aiohttp import ClientResponse, ClientSession
+from opal_common.config import opal_common_config
 from pydantic import validator
 
 from ...http import is_http_error_response
 from ...security.sslcontext import get_custom_ssl_context
 from ..events import FetcherConfig, FetchEvent
 from ..fetch_provider import BaseFetchProvider
 from ..logger import get_logger
@@ -67,48 +69,59 @@
     def parse_event(self, event: FetchEvent) -> HttpFetchEvent:
         return HttpFetchEvent(**event.dict(exclude={"config"}), config=event.config)
 
     async def __aenter__(self):
         headers = {}
         if self._event.config.headers is not None:
             headers = self._event.config.headers
-        self._session = await ClientSession(
-            headers=headers, raise_for_status=True
-        ).__aenter__()
+        if opal_common_config.HTTP_FETCHER_PROVIDER_CLIENT == "httpx":
+            self._session = httpx.AsyncClient(headers=headers)
+        else:
+            self._session = ClientSession(headers=headers, raise_for_status=True)
+        self._session = await self._session.__aenter__()
         return self
 
     async def __aexit__(self, exc_type=None, exc_val=None, tb=None):
-        await self._session.__aexit__(exc_type=exc_type, exc_val=exc_val, exc_tb=tb)
+        await self._session.__aexit__(exc_type, exc_val, tb)
 
     async def _fetch_(self):
         logger.debug(f"{self.__class__.__name__} fetching from {self._url}")
         http_method = self.match_http_method_from_type(
             self._session, self._event.config.method
         )
         if self._event.config.data is not None:
-            result = await http_method(
+            result: Union[ClientResponse, httpx.Response] = await http_method(
                 self._url, data=self._event.config.data, **self._ssl_context_kwargs
             )
         else:
             result = await http_method(self._url, **self._ssl_context_kwargs)
+        result.raise_for_status()
         return result
 
     @staticmethod
-    def match_http_method_from_type(session: ClientSession, method_type: HttpMethods):
+    def match_http_method_from_type(
+        session: Union[ClientSession, httpx.AsyncClient], method_type: HttpMethods
+    ):
         return getattr(session, method_type.value)
 
-    async def _process_(self, res: ClientResponse):
+    @staticmethod
+    async def _response_to_data(
+        res: Union[ClientResponse, httpx.Response], *, is_json: bool
+    ) -> Any:
+        if isinstance(res, httpx.Response):
+            return res.json() if is_json else res.text
+        else:
+            res = cast(ClientResponse, res)
+            return await (res.json() if is_json else res.text())
+
+    async def _process_(self, res: Union[ClientResponse, httpx.Response]):
         # do not process data when the http response is an error
         if is_http_error_response(res):
             return res
 
         # if we are asked to process the data before we return it
         if self._event.config.process_data:
-            # if data is JSON
-            if self._event.config.is_json:
-                data = await res.json()
-            else:
-                data = await res.text()
+            data = await self._response_to_data(res, is_json=self._event.config.is_json)
             return data
         # return raw result
         else:
             return res
```

### Comparing `opal_common-0.7.6/opal_common/fetcher/tests/failure_handler_test.py` & `opal-common-0.7.7/opal_common/fetcher/tests/failure_handler_test.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/fetcher/tests/http_fetch_test.py` & `opal-common-0.7.7/opal_common/fetcher/tests/http_fetch_test.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/fetcher/tests/rpc_fetch_test.py` & `opal-common-0.7.7/opal_common/fetcher/tests/rpc_fetch_test.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/git/branch_tracker.py` & `opal-common-0.7.7/opal_common/git/branch_tracker.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/git/bundle_maker.py` & `opal-common-0.7.7/opal_common/git/bundle_maker.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/git/bundle_utils.py` & `opal-common-0.7.7/opal_common/git/bundle_utils.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/git/commit_viewer.py` & `opal-common-0.7.7/opal_common/git/commit_viewer.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/git/diff_viewer.py` & `opal-common-0.7.7/opal_common/git/diff_viewer.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/git/env.py` & `opal-common-0.7.7/opal_common/git/env.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/git/repo_cloner.py` & `opal-common-0.7.7/opal_common/git/repo_cloner.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/git/tar_file_to_local_git_extractor.py` & `opal-common-0.7.7/opal_common/git/tar_file_to_local_git_extractor.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/logger.py` & `opal-common-0.7.7/opal_common/logger.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/logging/filter.py` & `opal-common-0.7.7/opal_common/logging/filter.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/logging/formatter.py` & `opal-common-0.7.7/opal_common/logging/formatter.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/logging/intercept.py` & `opal-common-0.7.7/opal_common/logging/intercept.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/logging/thirdparty.py` & `opal-common-0.7.7/opal_common/logging/thirdparty.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/middleware.py` & `opal-common-0.7.7/opal_common/middleware.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/monitoring/apm.py` & `opal-common-0.7.7/opal_common/monitoring/apm.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/monitoring/metrics.py` & `opal-common-0.7.7/opal_common/monitoring/metrics.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/paths.py` & `opal-common-0.7.7/opal_common/paths.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/schemas/data.py` & `opal-common-0.7.7/opal_common/schemas/data.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/schemas/policy.py` & `opal-common-0.7.7/opal_common/schemas/policy.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/schemas/policy_source.py` & `opal-common-0.7.7/opal_common/schemas/policy_source.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/schemas/security.py` & `opal-common-0.7.7/opal_common/schemas/security.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/schemas/store.py` & `opal-common-0.7.7/opal_common/schemas/store.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/schemas/webhook.py` & `opal-common-0.7.7/opal_common/schemas/webhook.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/security/sslcontext.py` & `opal-common-0.7.7/opal_common/security/sslcontext.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/security/tarsafe.py` & `opal-common-0.7.7/opal_common/security/tarsafe.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/sources/api_policy_source.py` & `opal-common-0.7.7/opal_common/sources/api_policy_source.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/sources/base_policy_source.py` & `opal-common-0.7.7/opal_common/sources/base_policy_source.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/sources/git_policy_source.py` & `opal-common-0.7.7/opal_common/sources/git_policy_source.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/synchronization/expiring_redis_lock.py` & `opal-common-0.7.7/opal_common/synchronization/expiring_redis_lock.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/synchronization/named_lock.py` & `opal-common-0.7.7/opal_common/synchronization/named_lock.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/tests/path_utils_test.py` & `opal-common-0.7.7/opal_common/tests/path_utils_test.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/tests/test_utils.py` & `opal-common-0.7.7/opal_common/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/tests/url_utils_test.py` & `opal-common-0.7.7/opal_common/tests/url_utils_test.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/topics/listener.py` & `opal-common-0.7.7/opal_common/topics/listener.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/topics/publisher.py` & `opal-common-0.7.7/opal_common/topics/publisher.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/topics/utils.py` & `opal-common-0.7.7/opal_common/topics/utils.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/urls.py` & `opal-common-0.7.7/opal_common/urls.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common/utils.py` & `opal-common-0.7.7/opal_common/utils.py`

 * *Files identical despite different names*

### Comparing `opal_common-0.7.6/opal_common.egg-info/PKG-INFO` & `opal-common-0.7.7/opal_common.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opal-common
-Version: 0.7.6
+Version: 0.7.7
 Summary: OPAL is an administration layer for Open Policy Agent (OPA), detecting changes to both policy and data and pushing live updates to your agents. opal-common contains common code used by both opal-client and opal-server.
 Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen
 Author-email: or@permit.io
 License: Apache 2.0
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
@@ -14,37 +14,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: aiohttp<4,>=3.9.2
-Requires-Dist: click<9,>=8.1.3
-Requires-Dist: cryptography<43,>=42.0.4
-Requires-Dist: gitpython<4,>=3.1.32
-Requires-Dist: loguru<1,>=0.6.0
-Requires-Dist: pyjwt[crypto]<3,>=2.4.0
-Requires-Dist: python-decouple<4,>=3.6
-Requires-Dist: tenacity<9,>=8.0.1
-Requires-Dist: datadog<1,>=0.44.0
-Requires-Dist: ddtrace<3,>=2.8.1
-Requires-Dist: certifi>=2023.7.22
-Requires-Dist: requests>=2.31.0
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
@@ -1,32 +1,20 @@
-Metadata-Version: 2.1 Name: opal-common Version: 0.7.6 Summary: OPAL is an
+Metadata-Version: 2.1 Name: opal-common Version: 0.7.7 Summary: OPAL is an
 administration layer for Open Policy Agent (OPA), detecting changes to both
 policy and data and pushing live updates to your agents. opal-common contains
 common code used by both opal-client and opal-server. Home-page: https://
 github.com/permitio/opal Author: Or Weis, Asaf Cohen Author-email: or@permit.io
 License: Apache 2.0 Classifier: Operating System :: OS Independent Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: Topic :: Internet :: WWW/
 HTTP :: HTTP Servers Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
-Requires-Python: >=3.9 Description-Content-Type: text/markdown Requires-Dist:
-aiohttp<4,>=3.9.2 Requires-Dist: click<9,>=8.1.3 Requires-Dist:
-cryptography<43,>=42.0.4 Requires-Dist: gitpython<4,>=3.1.32 Requires-Dist:
-loguru<1,>=0.6.0 Requires-Dist: pyjwt[crypto]<3,>=2.4.0 Requires-Dist: python-
-decouple<4,>=3.6 Requires-Dist: tenacity<9,>=8.0.1 Requires-Dist:
-datadog<1,>=0.44.0 Requires-Dist: ddtrace<3,>=2.8.1 Requires-Dist:
-certifi>=2023.7.22 Requires-Dist: requests>=2.31.0 Requires-Dist: idna<4,>=3.3
-Requires-Dist: typer<1,>=0.4.1 Requires-Dist: fastapi<1,>=0.109.1 Requires-
-Dist: fastapi_websocket_pubsub==0.3.7 Requires-Dist:
-fastapi_websocket_rpc<1,>=0.1.21 Requires-Dist: gunicorn<23,>=22.0.0 Requires-
-Dist: pydantic[email]<2,>=1.9.1 Requires-Dist: typing-extensions;
-python_version < "3.8" Requires-Dist: uvicorn[standard]<1,>=0.17.6 Requires-
-Dist: fastapi-utils<1,>=0.2.1 Requires-Dist: setuptools>=65.5.1
+Requires-Python: >=3.9 Description-Content-Type: text/markdown
                                     [opal]
                            ************ ?â??¡OOPPAALL?â??¡ ************
                  ********** OOppeenn PPoolliiccyy AAddmmiinniissttrraattiioonn LLaayyeerr **********
 _[_T_e_s_t_s_]_[_P_a_c_k_a_g_e_]_[_P_a_c_k_a_g_e_]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_c_k_e_r_ _p_u_l_l_s_]_[_J_o_i_n_ _o_u_r_ _S_l_a_c_k_!_]_[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_t_w_i_t_t_e_r_/_f_o_l_l_o_w_/
 _p_e_r_m_i_t___i_o_?_l_a_b_e_l_=_F_o_l_l_o_w_%_2_0_%_4_0_p_e_r_m_i_t___i_o_&_s_t_y_l_e_=_s_o_c_i_a_l_]## What is OPAL? OPAL is an
 administration layer for Policy Engines such as _O_p_e_n_ _P_o_l_i_c_y_ _A_g_e_n_t_ _(_O_P_A_), and
```

### Comparing `opal_common-0.7.6/opal_common.egg-info/SOURCES.txt` & `opal-common-0.7.7/opal_common.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 opal_common/confi/__init__.py
 opal_common/confi/cli.py
 opal_common/confi/confi.py
 opal_common/confi/types.py
 opal_common/engine/__init__.py
 opal_common/engine/parsing.py
 opal_common/engine/paths.py
-opal_common/engine/py.typed
 opal_common/fetcher/__init__.py
 opal_common/fetcher/events.py
 opal_common/fetcher/fetch_provider.py
 opal_common/fetcher/fetcher_register.py
 opal_common/fetcher/logger.py
 opal_common/fetcher/engine/__init__.py
 opal_common/fetcher/engine/base_fetching_engine.py
```

### Comparing `opal_common-0.7.6/opal_common.egg-info/requires.txt` & `opal-common-0.7.7/opal_common.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 pyjwt[crypto]<3,>=2.4.0
 python-decouple<4,>=3.6
 tenacity<9,>=8.0.1
 datadog<1,>=0.44.0
 ddtrace<3,>=2.8.1
 certifi>=2023.7.22
 requests>=2.31.0
+httpx==0.27.0
 idna<4,>=3.3
 typer<1,>=0.4.1
 fastapi<1,>=0.109.1
 fastapi_websocket_pubsub==0.3.7
 fastapi_websocket_rpc<1,>=0.1.21
 gunicorn<23,>=22.0.0
 pydantic[email]<2,>=1.9.1
```

### Comparing `opal_common-0.7.6/setup.py` & `opal-common-0.7.7/setup.py`

 * *Files identical despite different names*

