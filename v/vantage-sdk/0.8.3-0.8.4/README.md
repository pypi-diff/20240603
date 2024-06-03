# Comparing `tmp/vantage_sdk-0.8.3.tar.gz` & `tmp/vantage_sdk-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage_sdk-0.8.3.tar", max compression
+gzip compressed data, was "vantage_sdk-0.8.4.tar", max compression
```

## Comparing `vantage_sdk-0.8.3.tar` & `vantage_sdk-0.8.4.tar`

### file list

```diff
@@ -1,84 +1,84 @@
--rw-r--r--   0        0        0    11357 2024-01-11 12:38:41.319331 vantage_sdk-0.8.3/LICENSE
--rw-r--r--   0        0        0     3971 2024-05-31 14:01:17.976145 vantage_sdk-0.8.3/README.md
--rw-r--r--   0        0        0     2976 2024-05-31 14:01:17.979479 vantage_sdk-0.8.3/docs/api.md
--rw-r--r--   0        0        0    31784 2024-05-31 14:01:17.979479 vantage_sdk-0.8.3/docs/assets/vantage_logo.png
--rw-r--r--   0        0        0    17557 2024-05-31 14:01:17.979479 vantage_sdk-0.8.3/docs/assets/vantage_logo_small.png
--rw-r--r--   0        0        0       19 2024-05-31 14:01:17.979479 vantage_sdk-0.8.3/docs/index.md
--rw-r--r--   0        0        0      169 2024-05-31 14:01:17.979479 vantage_sdk-0.8.3/docs/stylesheets/extra.css
--rw-r--r--   0        0        0     3084 2024-05-31 14:01:17.979479 vantage_sdk-0.8.3/pyproject.toml
--rw-r--r--   0        0        0       41 2024-01-15 14:39:17.295617 vantage_sdk-0.8.3/tests/__init__.py
--rw-r--r--   0        0        0    70399 2024-03-07 14:45:28.746459 vantage_sdk-0.8.3/tests/data/documents.jsonl
--rw-r--r--   0        0        0     2971 2024-01-31 13:54:14.501245 vantage_sdk-0.8.3/tests/data/hello_world.parquet
--rw-r--r--   0        0        0      777 2024-04-12 11:53:13.437182 vantage_sdk-0.8.3/tests/integration_tests/.env-example
--rw-r--r--   0        0        0        0 2024-03-12 12:22:06.326740 vantage_sdk-0.8.3/tests/integration_tests/__init__.py
--rw-r--r--   0        0        0    10571 2024-05-14 13:03:23.582862 vantage_sdk-0.8.3/tests/integration_tests/conftest.py
--rw-r--r--   0        0        0     3027 2024-05-21 10:41:28.285018 vantage_sdk-0.8.3/tests/integration_tests/test_account.py
--rw-r--r--   0        0        0    10935 2024-05-31 14:01:17.979479 vantage_sdk-0.8.3/tests/integration_tests/test_api_keys.py
--rw-r--r--   0        0        0    12709 2024-05-14 13:03:23.582862 vantage_sdk-0.8.3/tests/integration_tests/test_collection.py
--rw-r--r--   0        0        0     4219 2024-05-31 14:01:17.982812 vantage_sdk-0.8.3/tests/integration_tests/test_documents.py
--rw-r--r--   0        0        0     9132 2024-04-11 13:25:19.388795 vantage_sdk-0.8.3/tests/integration_tests/test_search.py
--rw-r--r--   0        0        0      665 2024-05-31 14:01:17.982812 vantage_sdk-0.8.3/vantage_sdk/__init__.py
--rw-r--r--   0        0        0    66901 2024-05-31 14:01:17.982812 vantage_sdk-0.8.3/vantage_sdk/client.py
--rw-r--r--   0        0        0      239 2024-05-14 13:03:23.582862 vantage_sdk-0.8.3/vantage_sdk/config.py
--rw-r--r--   0        0        0       43 2024-04-11 13:15:31.438553 vantage_sdk-0.8.3/vantage_sdk/core/__init__.py
--rw-r--r--   0        0        0     6471 2024-04-11 13:15:31.438553 vantage_sdk-0.8.3/vantage_sdk/core/base.py
--rw-r--r--   0        0        0     2172 2024-05-31 14:01:17.982812 vantage_sdk-0.8.3/vantage_sdk/core/exceptions.py
--rw-r--r--   0        0        0     4108 2024-05-31 14:01:17.982812 vantage_sdk-0.8.3/vantage_sdk/core/http/__init__.py
--rw-r--r--   0        0        0      508 2024-05-31 14:01:17.982812 vantage_sdk-0.8.3/vantage_sdk/core/http/api/__init__.py
--rw-r--r--   0        0        0    22934 2024-04-11 13:15:31.438553 vantage_sdk-0.8.3/vantage_sdk/core/http/api/account_management_api.py
--rw-r--r--   0        0        0    75134 2024-05-14 13:03:23.586196 vantage_sdk-0.8.3/vantage_sdk/core/http/api/collection_management_api.py
--rw-r--r--   0        0        0    15180 2024-04-11 13:15:31.438553 vantage_sdk-0.8.3/vantage_sdk/core/http/api/documents_api.py
--rw-r--r--   0        0        0    57239 2024-05-31 14:01:17.982812 vantage_sdk-0.8.3/vantage_sdk/core/http/api/external_keys_api.py
--rw-r--r--   0        0        0    54428 2024-04-11 13:15:31.438553 vantage_sdk-0.8.3/vantage_sdk/core/http/api/search_api.py
--rw-r--r--   0        0        0    22624 2024-05-14 13:03:23.589529 vantage_sdk-0.8.3/vantage_sdk/core/http/api/vantage_api_keys_api.py
--rw-r--r--   0        0        0    24948 2024-04-11 13:15:31.439553 vantage_sdk-0.8.3/vantage_sdk/core/http/api_client.py
--rw-r--r--   0        0        0      678 2024-04-11 13:15:31.439553 vantage_sdk-0.8.3/vantage_sdk/core/http/api_response.py
--rw-r--r--   0        0        0    15524 2024-04-12 10:31:03.021028 vantage_sdk-0.8.3/vantage_sdk/core/http/configuration.py
--rw-r--r--   0        0        0     6369 2024-04-11 13:15:31.439553 vantage_sdk-0.8.3/vantage_sdk/core/http/exceptions.py
--rw-r--r--   0        0        0     3231 2024-05-31 14:01:17.982812 vantage_sdk-0.8.3/vantage_sdk/core/http/models/__init__.py
--rw-r--r--   0        0        0     2951 2024-04-11 13:15:31.439553 vantage_sdk-0.8.3/vantage_sdk/core/http/models/account.py
--rw-r--r--   0        0        0     2735 2024-04-11 13:15:31.439553 vantage_sdk-0.8.3/vantage_sdk/core/http/models/account_modifiable.py
--rw-r--r--   0        0        0     2812 2024-04-11 13:15:31.439553 vantage_sdk-0.8.3/vantage_sdk/core/http/models/account_read_only.py
--rw-r--r--   0        0        0     7511 2024-05-31 14:01:17.982812 vantage_sdk-0.8.3/vantage_sdk/core/http/models/collection.py
--rw-r--r--   0        0        0     4615 2024-04-11 13:15:31.441553 vantage_sdk-0.8.3/vantage_sdk/core/http/models/collection_immutable.py
--rw-r--r--   0        0        0     4010 2024-05-31 14:01:17.982812 vantage_sdk-0.8.3/vantage_sdk/core/http/models/collection_modifiable.py
--rw-r--r--   0        0        0     4316 2024-04-11 13:15:31.441553 vantage_sdk-0.8.3/vantage_sdk/core/http/models/collection_read_only.py
--rw-r--r--   0        0        0     3698 2024-04-11 13:15:31.441553 vantage_sdk-0.8.3/vantage_sdk/core/http/models/collection_upload_url.py
--rw-r--r--   0        0        0     5862 2024-05-31 14:01:17.982812 vantage_sdk-0.8.3/vantage_sdk/core/http/models/create_collection_request.py
--rw-r--r--   0        0        0     2962 2024-04-11 13:15:31.442553 vantage_sdk-0.8.3/vantage_sdk/core/http/models/document_batch.py
--rw-r--r--   0        0        0     5725 2024-05-31 14:01:17.982812 vantage_sdk-0.8.3/vantage_sdk/core/http/models/embedding_search_query.py
--rw-r--r--   0        0        0     4338 2024-05-31 14:01:17.982812 vantage_sdk-0.8.3/vantage_sdk/core/http/models/external_key.py
--rw-r--r--   0        0        0     3371 2024-05-31 14:01:17.982812 vantage_sdk-0.8.3/vantage_sdk/core/http/models/external_key_modifiable.py
--rw-r--r--   0        0        0     3661 2024-05-31 14:01:17.982812 vantage_sdk-0.8.3/vantage_sdk/core/http/models/external_key_read_only.py
--rw-r--r--   0        0        0     3282 2024-04-12 10:31:03.021028 vantage_sdk-0.8.3/vantage_sdk/core/http/models/ml_these.py
--rw-r--r--   0        0        0     3326 2024-04-11 13:15:31.444553 vantage_sdk-0.8.3/vantage_sdk/core/http/models/ml_these_these_inner.py
--rw-r--r--   0        0        0     6228 2024-05-31 14:01:17.982812 vantage_sdk-0.8.3/vantage_sdk/core/http/models/more_like_these_query.py
--rw-r--r--   0        0        0     5686 2024-05-31 14:01:17.982812 vantage_sdk-0.8.3/vantage_sdk/core/http/models/more_like_this_query.py
--rw-r--r--   0        0        0     5537 2024-05-31 14:01:17.982812 vantage_sdk-0.8.3/vantage_sdk/core/http/models/search_options.py
--rw-r--r--   0        0        0     2816 2024-05-31 14:01:17.982812 vantage_sdk-0.8.3/vantage_sdk/core/http/models/search_options_collection.py
--rw-r--r--   0        0        0     4560 2024-05-31 14:01:17.982812 vantage_sdk-0.8.3/vantage_sdk/core/http/models/search_options_field_value_weighting.py
--rw-r--r--   0        0        0     2773 2024-05-31 14:01:17.982812 vantage_sdk-0.8.3/vantage_sdk/core/http/models/search_options_filter.py
--rw-r--r--   0        0        0     2976 2024-05-31 14:01:17.982812 vantage_sdk-0.8.3/vantage_sdk/core/http/models/search_options_pagination.py
--rw-r--r--   0        0        0     3621 2024-05-31 14:01:17.982812 vantage_sdk-0.8.3/vantage_sdk/core/http/models/search_options_sort.py
--rw-r--r--   0        0        0     3721 2024-04-12 10:31:03.021028 vantage_sdk-0.8.3/vantage_sdk/core/http/models/search_result.py
--rw-r--r--   0        0        0     2870 2024-04-11 13:15:31.444553 vantage_sdk-0.8.3/vantage_sdk/core/http/models/search_result_results_inner.py
--rw-r--r--   0        0        0     3441 2024-05-31 14:01:17.986146 vantage_sdk-0.8.3/vantage_sdk/core/http/models/secondary_external_account.py
--rw-r--r--   0        0        0     5666 2024-05-31 14:01:17.986146 vantage_sdk-0.8.3/vantage_sdk/core/http/models/semantic_search_query.py
--rw-r--r--   0        0        0     4093 2024-04-11 13:15:31.444553 vantage_sdk-0.8.3/vantage_sdk/core/http/models/vantage_api_key.py
--rw-r--r--   0        0        0     3003 2024-04-11 13:15:31.444553 vantage_sdk-0.8.3/vantage_sdk/core/http/models/weighted_field_values.py
--rw-r--r--   0        0        0        0 2024-04-11 13:15:31.444553 vantage_sdk-0.8.3/vantage_sdk/core/http/py.typed
--rw-r--r--   0        0        0    10169 2024-04-11 13:15:31.445553 vantage_sdk-0.8.3/vantage_sdk/core/http/rest.py
--rw-r--r--   0        0        0       95 2024-04-11 13:15:31.445553 vantage_sdk-0.8.3/vantage_sdk/core/management/__init__.py
--rw-r--r--   0        0        0     3249 2024-05-31 14:01:17.986146 vantage_sdk-0.8.3/vantage_sdk/core/management/management.py
--rw-r--r--   0        0        0       79 2024-04-11 13:15:31.445553 vantage_sdk-0.8.3/vantage_sdk/core/search/__init__.py
--rw-r--r--   0        0        0      645 2024-05-31 14:01:17.986146 vantage_sdk-0.8.3/vantage_sdk/core/search/search.py
--rw-r--r--   0        0        0    13313 2024-05-31 14:01:17.986146 vantage_sdk-0.8.3/vantage_sdk/core/validation.py
--rw-r--r--   0        0        0      559 2024-04-11 13:15:31.445553 vantage_sdk-0.8.3/vantage_sdk/exceptions.py
--rw-r--r--   0        0        0       37 2024-05-31 14:01:17.986146 vantage_sdk-0.8.3/vantage_sdk/model/__init__.py
--rw-r--r--   0        0        0      437 2024-05-31 14:01:17.986146 vantage_sdk-0.8.3/vantage_sdk/model/account.py
--rw-r--r--   0        0        0     5145 2024-05-31 14:01:17.986146 vantage_sdk-0.8.3/vantage_sdk/model/collection.py
--rw-r--r--   0        0        0     2362 2024-05-31 14:01:17.986146 vantage_sdk-0.8.3/vantage_sdk/model/document.py
--rw-r--r--   0        0        0     2349 2024-05-31 14:01:17.986146 vantage_sdk-0.8.3/vantage_sdk/model/keys.py
--rw-r--r--   0        0        0     5241 2024-05-31 14:01:17.986146 vantage_sdk-0.8.3/vantage_sdk/model/search.py
--rw-r--r--   0        0        0     1198 2024-05-31 14:01:17.986146 vantage_sdk-0.8.3/vantage_sdk/model/validation.py
--rw-r--r--   0        0        0     6215 1970-01-01 00:00:00.000000 vantage_sdk-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-06-03 12:33:26.276459 vantage_sdk-0.8.4/LICENSE
+-rw-r--r--   0        0        0     3971 2024-06-03 12:33:26.279792 vantage_sdk-0.8.4/README.md
+-rw-r--r--   0        0        0     2976 2024-06-03 12:33:26.279792 vantage_sdk-0.8.4/docs/api.md
+-rw-r--r--   0        0        0    31784 2024-06-03 12:33:26.279792 vantage_sdk-0.8.4/docs/assets/vantage_logo.png
+-rw-r--r--   0        0        0    17557 2024-06-03 12:33:26.279792 vantage_sdk-0.8.4/docs/assets/vantage_logo_small.png
+-rw-r--r--   0        0        0       19 2024-06-03 12:33:26.279792 vantage_sdk-0.8.4/docs/index.md
+-rw-r--r--   0        0        0      169 2024-06-03 12:33:26.279792 vantage_sdk-0.8.4/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0     3102 2024-06-03 13:50:31.792071 vantage_sdk-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0       41 2024-06-03 12:33:26.283126 vantage_sdk-0.8.4/tests/__init__.py
+-rw-r--r--   0        0        0    70399 2024-06-03 12:33:26.283126 vantage_sdk-0.8.4/tests/data/documents.jsonl
+-rw-r--r--   0        0        0     2971 2024-06-03 12:33:26.283126 vantage_sdk-0.8.4/tests/data/hello_world.parquet
+-rw-r--r--   0        0        0      777 2024-06-03 12:33:26.283126 vantage_sdk-0.8.4/tests/integration_tests/.env-example
+-rw-r--r--   0        0        0        0 2024-06-03 12:33:26.283126 vantage_sdk-0.8.4/tests/integration_tests/__init__.py
+-rw-r--r--   0        0        0    10571 2024-06-03 12:33:26.286459 vantage_sdk-0.8.4/tests/integration_tests/conftest.py
+-rw-r--r--   0        0        0     3027 2024-06-03 12:33:26.286459 vantage_sdk-0.8.4/tests/integration_tests/test_account.py
+-rw-r--r--   0        0        0    10935 2024-06-03 12:33:26.286459 vantage_sdk-0.8.4/tests/integration_tests/test_api_keys.py
+-rw-r--r--   0        0        0    12709 2024-06-03 12:33:26.289793 vantage_sdk-0.8.4/tests/integration_tests/test_collection.py
+-rw-r--r--   0        0        0     4219 2024-06-03 12:33:26.289793 vantage_sdk-0.8.4/tests/integration_tests/test_documents.py
+-rw-r--r--   0        0        0     9132 2024-06-03 12:33:26.289793 vantage_sdk-0.8.4/tests/integration_tests/test_search.py
+-rw-r--r--   0        0        0      665 2024-06-03 13:50:31.792071 vantage_sdk-0.8.4/vantage_sdk/__init__.py
+-rw-r--r--   0        0        0    66901 2024-06-03 12:33:26.289793 vantage_sdk-0.8.4/vantage_sdk/client.py
+-rw-r--r--   0        0        0      239 2024-06-03 12:33:26.293126 vantage_sdk-0.8.4/vantage_sdk/config.py
+-rw-r--r--   0        0        0       43 2024-06-03 12:33:26.293126 vantage_sdk-0.8.4/vantage_sdk/core/__init__.py
+-rw-r--r--   0        0        0     6471 2024-06-03 12:33:26.293126 vantage_sdk-0.8.4/vantage_sdk/core/base.py
+-rw-r--r--   0        0        0     2172 2024-06-03 12:33:26.293126 vantage_sdk-0.8.4/vantage_sdk/core/exceptions.py
+-rw-r--r--   0        0        0     4108 2024-06-03 12:33:26.293126 vantage_sdk-0.8.4/vantage_sdk/core/http/__init__.py
+-rw-r--r--   0        0        0      508 2024-06-03 12:33:26.296460 vantage_sdk-0.8.4/vantage_sdk/core/http/api/__init__.py
+-rw-r--r--   0        0        0    22934 2024-06-03 12:33:26.296460 vantage_sdk-0.8.4/vantage_sdk/core/http/api/account_management_api.py
+-rw-r--r--   0        0        0    75134 2024-06-03 12:33:26.296460 vantage_sdk-0.8.4/vantage_sdk/core/http/api/collection_management_api.py
+-rw-r--r--   0        0        0    15180 2024-06-03 12:33:26.299793 vantage_sdk-0.8.4/vantage_sdk/core/http/api/documents_api.py
+-rw-r--r--   0        0        0    57239 2024-06-03 12:33:26.299793 vantage_sdk-0.8.4/vantage_sdk/core/http/api/external_keys_api.py
+-rw-r--r--   0        0        0    54428 2024-06-03 12:33:26.299793 vantage_sdk-0.8.4/vantage_sdk/core/http/api/search_api.py
+-rw-r--r--   0        0        0    22624 2024-06-03 12:33:26.299793 vantage_sdk-0.8.4/vantage_sdk/core/http/api/vantage_api_keys_api.py
+-rw-r--r--   0        0        0    24948 2024-06-03 12:33:26.303127 vantage_sdk-0.8.4/vantage_sdk/core/http/api_client.py
+-rw-r--r--   0        0        0      678 2024-06-03 12:33:26.303127 vantage_sdk-0.8.4/vantage_sdk/core/http/api_response.py
+-rw-r--r--   0        0        0    15524 2024-06-03 12:33:26.303127 vantage_sdk-0.8.4/vantage_sdk/core/http/configuration.py
+-rw-r--r--   0        0        0     6369 2024-06-03 12:33:26.303127 vantage_sdk-0.8.4/vantage_sdk/core/http/exceptions.py
+-rw-r--r--   0        0        0     3231 2024-06-03 12:33:26.303127 vantage_sdk-0.8.4/vantage_sdk/core/http/models/__init__.py
+-rw-r--r--   0        0        0     2951 2024-06-03 12:33:26.303127 vantage_sdk-0.8.4/vantage_sdk/core/http/models/account.py
+-rw-r--r--   0        0        0     2735 2024-06-03 12:33:26.303127 vantage_sdk-0.8.4/vantage_sdk/core/http/models/account_modifiable.py
+-rw-r--r--   0        0        0     2812 2024-06-03 12:33:26.303127 vantage_sdk-0.8.4/vantage_sdk/core/http/models/account_read_only.py
+-rw-r--r--   0        0        0     7511 2024-06-03 12:33:26.303127 vantage_sdk-0.8.4/vantage_sdk/core/http/models/collection.py
+-rw-r--r--   0        0        0     4615 2024-06-03 12:33:26.303127 vantage_sdk-0.8.4/vantage_sdk/core/http/models/collection_immutable.py
+-rw-r--r--   0        0        0     4010 2024-06-03 12:33:26.329794 vantage_sdk-0.8.4/vantage_sdk/core/http/models/collection_modifiable.py
+-rw-r--r--   0        0        0     4316 2024-06-03 12:33:26.329794 vantage_sdk-0.8.4/vantage_sdk/core/http/models/collection_read_only.py
+-rw-r--r--   0        0        0     3698 2024-06-03 12:33:26.329794 vantage_sdk-0.8.4/vantage_sdk/core/http/models/collection_upload_url.py
+-rw-r--r--   0        0        0     5862 2024-06-03 12:33:26.336461 vantage_sdk-0.8.4/vantage_sdk/core/http/models/create_collection_request.py
+-rw-r--r--   0        0        0     2962 2024-06-03 12:33:26.336461 vantage_sdk-0.8.4/vantage_sdk/core/http/models/document_batch.py
+-rw-r--r--   0        0        0     5725 2024-06-03 12:33:26.339795 vantage_sdk-0.8.4/vantage_sdk/core/http/models/embedding_search_query.py
+-rw-r--r--   0        0        0     4338 2024-06-03 12:33:26.339795 vantage_sdk-0.8.4/vantage_sdk/core/http/models/external_key.py
+-rw-r--r--   0        0        0     3371 2024-06-03 12:33:26.339795 vantage_sdk-0.8.4/vantage_sdk/core/http/models/external_key_modifiable.py
+-rw-r--r--   0        0        0     3661 2024-06-03 12:33:26.339795 vantage_sdk-0.8.4/vantage_sdk/core/http/models/external_key_read_only.py
+-rw-r--r--   0        0        0     3282 2024-06-03 12:33:26.343128 vantage_sdk-0.8.4/vantage_sdk/core/http/models/ml_these.py
+-rw-r--r--   0        0        0     3326 2024-06-03 12:33:26.343128 vantage_sdk-0.8.4/vantage_sdk/core/http/models/ml_these_these_inner.py
+-rw-r--r--   0        0        0     6228 2024-06-03 12:33:26.343128 vantage_sdk-0.8.4/vantage_sdk/core/http/models/more_like_these_query.py
+-rw-r--r--   0        0        0     5686 2024-06-03 12:33:26.343128 vantage_sdk-0.8.4/vantage_sdk/core/http/models/more_like_this_query.py
+-rw-r--r--   0        0        0     5537 2024-06-03 12:33:26.343128 vantage_sdk-0.8.4/vantage_sdk/core/http/models/search_options.py
+-rw-r--r--   0        0        0     2816 2024-06-03 12:33:26.343128 vantage_sdk-0.8.4/vantage_sdk/core/http/models/search_options_collection.py
+-rw-r--r--   0        0        0     4560 2024-06-03 12:33:26.343128 vantage_sdk-0.8.4/vantage_sdk/core/http/models/search_options_field_value_weighting.py
+-rw-r--r--   0        0        0     2773 2024-06-03 12:33:26.343128 vantage_sdk-0.8.4/vantage_sdk/core/http/models/search_options_filter.py
+-rw-r--r--   0        0        0     2976 2024-06-03 12:33:26.343128 vantage_sdk-0.8.4/vantage_sdk/core/http/models/search_options_pagination.py
+-rw-r--r--   0        0        0     3621 2024-06-03 12:33:26.343128 vantage_sdk-0.8.4/vantage_sdk/core/http/models/search_options_sort.py
+-rw-r--r--   0        0        0     3721 2024-06-03 12:33:26.346462 vantage_sdk-0.8.4/vantage_sdk/core/http/models/search_result.py
+-rw-r--r--   0        0        0     2870 2024-06-03 12:33:26.346462 vantage_sdk-0.8.4/vantage_sdk/core/http/models/search_result_results_inner.py
+-rw-r--r--   0        0        0     3441 2024-06-03 12:33:26.346462 vantage_sdk-0.8.4/vantage_sdk/core/http/models/secondary_external_account.py
+-rw-r--r--   0        0        0     5666 2024-06-03 12:33:26.349795 vantage_sdk-0.8.4/vantage_sdk/core/http/models/semantic_search_query.py
+-rw-r--r--   0        0        0     4093 2024-06-03 12:33:26.349795 vantage_sdk-0.8.4/vantage_sdk/core/http/models/vantage_api_key.py
+-rw-r--r--   0        0        0     3003 2024-06-03 12:33:26.353129 vantage_sdk-0.8.4/vantage_sdk/core/http/models/weighted_field_values.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:33:26.353129 vantage_sdk-0.8.4/vantage_sdk/core/http/py.typed
+-rw-r--r--   0        0        0    10169 2024-06-03 12:33:26.353129 vantage_sdk-0.8.4/vantage_sdk/core/http/rest.py
+-rw-r--r--   0        0        0       95 2024-06-03 12:33:26.353129 vantage_sdk-0.8.4/vantage_sdk/core/management/__init__.py
+-rw-r--r--   0        0        0     3249 2024-06-03 12:33:26.353129 vantage_sdk-0.8.4/vantage_sdk/core/management/management.py
+-rw-r--r--   0        0        0       79 2024-06-03 12:33:26.353129 vantage_sdk-0.8.4/vantage_sdk/core/search/__init__.py
+-rw-r--r--   0        0        0      645 2024-06-03 12:33:26.353129 vantage_sdk-0.8.4/vantage_sdk/core/search/search.py
+-rw-r--r--   0        0        0    13313 2024-06-03 12:33:26.353129 vantage_sdk-0.8.4/vantage_sdk/core/validation.py
+-rw-r--r--   0        0        0      559 2024-06-03 12:33:26.353129 vantage_sdk-0.8.4/vantage_sdk/exceptions.py
+-rw-r--r--   0        0        0       37 2024-06-03 12:33:26.353129 vantage_sdk-0.8.4/vantage_sdk/model/__init__.py
+-rw-r--r--   0        0        0      437 2024-06-03 12:33:26.353129 vantage_sdk-0.8.4/vantage_sdk/model/account.py
+-rw-r--r--   0        0        0     5145 2024-06-03 12:33:26.353129 vantage_sdk-0.8.4/vantage_sdk/model/collection.py
+-rw-r--r--   0        0        0     2362 2024-06-03 12:33:26.353129 vantage_sdk-0.8.4/vantage_sdk/model/document.py
+-rw-r--r--   0        0        0     2349 2024-06-03 12:33:26.353129 vantage_sdk-0.8.4/vantage_sdk/model/keys.py
+-rw-r--r--   0        0        0     5241 2024-06-03 12:33:26.353129 vantage_sdk-0.8.4/vantage_sdk/model/search.py
+-rw-r--r--   0        0        0     1198 2024-06-03 12:33:26.353129 vantage_sdk-0.8.4/vantage_sdk/model/validation.py
+-rw-r--r--   0        0        0     6254 1970-01-01 00:00:00.000000 vantage_sdk-0.8.4/PKG-INFO
```

### Comparing `vantage_sdk-0.8.3/LICENSE` & `vantage_sdk-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/README.md` & `vantage_sdk-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/docs/api.md` & `vantage_sdk-0.8.4/docs/api.md`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/docs/assets/vantage_logo.png` & `vantage_sdk-0.8.4/docs/assets/vantage_logo.png`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/docs/assets/vantage_logo_small.png` & `vantage_sdk-0.8.4/docs/assets/vantage_logo_small.png`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/pyproject.toml` & `vantage_sdk-0.8.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "vantage-sdk"
-version = "0.8.3"
+version = "0.8.4"
 description = "Vantage Python SDK."
 authors = ["Vantage <none@vantage.com>"]
 readme = "README.md"
 repository = "https://github.com/VantageDiscovery/vantage-sdk-python"
 documentation = "https://docs.vantagediscovery.com/docs/concepts"
 classifiers=[
     'Programming Language :: Python :: 3.10',
@@ -48,14 +48,15 @@
 python-dotenv = ">=1.0.1"
 bumpver = {version = ">=2023.1129"}
 pip-tools = {version = ">=7.3.0"}
 mkdocstrings = {version = ">=0.25.1", extras = ["python"]}
 griffe-fieldz = {version = ">= 0.1.2"}
 tiktoken = {version = ">=0.7.0"}
 pyarrow = {version = ">=16.1.0"}
+pandas = "^2.2.2"
 
 [tool.poetry.extras]
 test = [
     "pytest",
     "black",
     "isort",
     "mypy",
@@ -118,15 +119,15 @@
     "D107"
 ]
 
 [tool.mypy]
 exclude = "vantage_sdk/core/http"
 
 [bumpver]
-current_version = "0.8.3"
+current_version = "0.8.4"
 version_pattern = "MAJOR.MINOR.PATCH"
 
 [bumpver.file_patterns]
 "pyproject.toml" = [
     'version = "{version}"',
 ]
 "vantage_sdk/__init__.py" = [
```

### Comparing `vantage_sdk-0.8.3/tests/data/documents.jsonl` & `vantage_sdk-0.8.4/tests/data/documents.jsonl`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/tests/data/hello_world.parquet` & `vantage_sdk-0.8.4/tests/data/hello_world.parquet`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/tests/integration_tests/.env-example` & `vantage_sdk-0.8.4/tests/integration_tests/.env-example`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/tests/integration_tests/conftest.py` & `vantage_sdk-0.8.4/tests/integration_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/tests/integration_tests/test_account.py` & `vantage_sdk-0.8.4/tests/integration_tests/test_account.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/tests/integration_tests/test_api_keys.py` & `vantage_sdk-0.8.4/tests/integration_tests/test_api_keys.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/tests/integration_tests/test_collection.py` & `vantage_sdk-0.8.4/tests/integration_tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/tests/integration_tests/test_documents.py` & `vantage_sdk-0.8.4/tests/integration_tests/test_documents.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/tests/integration_tests/test_search.py` & `vantage_sdk-0.8.4/tests/integration_tests/test_search.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/__init__.py` & `vantage_sdk-0.8.4/vantage_sdk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     SearchResult,
     SearchResultItem,
 )
 
 
 __author__ = """Vantage"""
 __email__ = 'none@vantage.com'
-__version__ = '0.8.3'
+__version__ = '0.8.4'
 __all__ = [
     "VantageClient",
     "Collection",
     "CollectionUploadURL",
     "Account",
     "VantageAPIKey",
     "ExternalKey",
```

### Comparing `vantage_sdk-0.8.3/vantage_sdk/client.py` & `vantage_sdk-0.8.4/vantage_sdk/client.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/base.py` & `vantage_sdk-0.8.4/vantage_sdk/core/base.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/exceptions.py` & `vantage_sdk-0.8.4/vantage_sdk/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/__init__.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/api/account_management_api.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/api/account_management_api.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/api/collection_management_api.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/api/collection_management_api.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/api/documents_api.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/api/documents_api.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/api/external_keys_api.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/api/external_keys_api.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/api/search_api.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/api/search_api.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/api/vantage_api_keys_api.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/api/vantage_api_keys_api.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/api_client.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/api_client.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/api_response.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/api_response.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/configuration.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/configuration.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/exceptions.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/exceptions.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/models/__init__.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/models/account.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/models/account.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/models/account_modifiable.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/models/account_modifiable.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/models/account_read_only.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/models/account_read_only.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/models/collection.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/models/collection.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/models/collection_immutable.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/models/collection_immutable.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/models/collection_modifiable.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/models/collection_modifiable.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/models/collection_read_only.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/models/collection_read_only.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/models/collection_upload_url.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/models/collection_upload_url.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/models/create_collection_request.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/models/create_collection_request.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/models/document_batch.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/models/document_batch.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/models/embedding_search_query.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/models/embedding_search_query.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/models/external_key.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/models/external_key.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/models/external_key_modifiable.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/models/external_key_modifiable.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/models/external_key_read_only.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/models/external_key_read_only.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/models/ml_these.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/models/ml_these.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/models/ml_these_these_inner.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/models/ml_these_these_inner.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/models/more_like_these_query.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/models/more_like_these_query.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/models/more_like_this_query.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/models/more_like_this_query.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/models/search_options.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/models/search_options.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/models/search_options_collection.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/models/search_options_collection.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/models/search_options_field_value_weighting.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/models/search_options_field_value_weighting.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/models/search_options_filter.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/models/search_options_filter.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/models/search_options_pagination.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/models/search_options_pagination.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/models/search_options_sort.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/models/search_options_sort.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/models/search_result.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/models/search_result.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/models/search_result_results_inner.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/models/search_result_results_inner.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/models/secondary_external_account.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/models/secondary_external_account.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/models/semantic_search_query.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/models/semantic_search_query.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/models/vantage_api_key.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/models/vantage_api_key.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/models/weighted_field_values.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/models/weighted_field_values.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/http/rest.py` & `vantage_sdk-0.8.4/vantage_sdk/core/http/rest.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/management/management.py` & `vantage_sdk-0.8.4/vantage_sdk/core/management/management.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/search/search.py` & `vantage_sdk-0.8.4/vantage_sdk/core/search/search.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/core/validation.py` & `vantage_sdk-0.8.4/vantage_sdk/core/validation.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/exceptions.py` & `vantage_sdk-0.8.4/vantage_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/model/collection.py` & `vantage_sdk-0.8.4/vantage_sdk/model/collection.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/model/document.py` & `vantage_sdk-0.8.4/vantage_sdk/model/document.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/model/keys.py` & `vantage_sdk-0.8.4/vantage_sdk/model/keys.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/model/search.py` & `vantage_sdk-0.8.4/vantage_sdk/model/search.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/vantage_sdk/model/validation.py` & `vantage_sdk-0.8.4/vantage_sdk/model/validation.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.3/PKG-INFO` & `vantage_sdk-0.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage-sdk
-Version: 0.8.3
+Version: 0.8.4
 Summary: Vantage Python SDK.
 Home-page: https://github.com/VantageDiscovery/vantage-sdk-python
 Author: Vantage
 Author-email: none@vantage.com
 Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -22,14 +22,15 @@
 Requires-Dist: griffe-fieldz (>=0.1.2)
 Requires-Dist: isort (>=5.8.0,<6.0.0) ; extra == "test"
 Requires-Dist: mkdocs (>=1.6.0,<2.0.0) ; extra == "doc"
 Requires-Dist: mkdocs-include-markdown-plugin (>=6.0.6,<7.0.0) ; extra == "doc"
 Requires-Dist: mkdocs-material (>=9.5.23,<10.0.0) ; extra == "doc"
 Requires-Dist: mkdocstrings[python] (>=0.25.1)
 Requires-Dist: mypy (>=1.5,<2.0) ; extra == "test"
+Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: pip ; extra == "dev"
 Requires-Dist: pip-tools (>=7.3.0) ; extra == "dev"
 Requires-Dist: pre-commit (>=3.3.0,<4.0.0) ; extra == "dev"
 Requires-Dist: pyarrow (>=16.1.0)
 Requires-Dist: pydantic (>=2)
 Requires-Dist: pytest (>=7.2.0,<8.0.0) ; extra == "test"
 Requires-Dist: pytest-cov (>=4.0.0,<5.0.0) ; extra == "test"
```

