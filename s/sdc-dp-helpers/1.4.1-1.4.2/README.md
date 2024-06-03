# Comparing `tmp/sdc_dp_helpers-1.4.1.tar.gz` & `tmp/sdc_dp_helpers-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdc_dp_helpers-1.4.1.tar", last modified: Tue May 28 08:05:48 2024, max compression
+gzip compressed data, was "sdc_dp_helpers-1.4.2.tar", last modified: Mon Jun  3 05:14:09 2024, max compression
```

## Comparing `sdc_dp_helpers-1.4.1.tar` & `sdc_dp_helpers-1.4.2.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.380302 sdc_dp_helpers-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-28 08:05:48.380302 sdc_dp_helpers-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.368301 sdc_dp_helpers-1.4.1/sdc_dp_helpers/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.368301 sdc_dp_helpers-1.4.1/sdc_dp_helpers/api_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/api_utilities/__init_.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/api_utilities/data_managers.py
--rw-r--r--   0 runner    (1001) docker     (127)    21226 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/api_utilities/date_managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/api_utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/api_utilities/file_managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/api_utilities/retry_managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/api_utilities/tracking_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.368301 sdc_dp_helpers-1.4.1/sdc_dp_helpers/azure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/azure/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/azure/writers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/base_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/base_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12994 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/base_writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.368301 sdc_dp_helpers-1.4.1/sdc_dp_helpers/facebook/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/facebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/facebook/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/facebook/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.368301 sdc_dp_helpers-1.4.1/sdc_dp_helpers/falcon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/falcon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29672 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/falcon/falcon_sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/falcon/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/falcon/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.372301 sdc_dp_helpers-1.4.1/sdc_dp_helpers/ftp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/ftp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/ftp/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/ftp/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.372301 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_ads/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_ads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_ads/generate_refresh_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_ads/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_ads/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.372301 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_analytics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_analytics/config_managers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17311 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_analytics/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_analytics/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_analytics/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.372301 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_analytics_v4/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_analytics_v4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_analytics_v4/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_analytics_v4/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.372301 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_big_query/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_big_query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_big_query/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_big_query/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.372301 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_knowledge_graph/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_knowledge_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_knowledge_graph/gkg_sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_knowledge_graph/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_knowledge_graph/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.372301 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_knowledge_graph_v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_knowledge_graph_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_knowledge_graph_v1/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_knowledge_graph_v1/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.372301 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_postmaster_tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_postmaster_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_postmaster_tools/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_postmaster_tools/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.376302 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_search_console/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_search_console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8414 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_search_console/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_search_console/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.376302 sdc_dp_helpers-1.4.1/sdc_dp_helpers/onesignal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/onesignal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13915 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/onesignal/onesignal_sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/onesignal/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/onesignal/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.376302 sdc_dp_helpers-1.4.1/sdc_dp_helpers/pyspark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/pyspark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/pyspark/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/pyspark/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.376302 sdc_dp_helpers-1.4.1/sdc_dp_helpers/sailthru/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/sailthru/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/sailthru/config_magagers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6708 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/sailthru/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/sailthru/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/sailthru/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.376302 sdc_dp_helpers-1.4.1/sdc_dp_helpers/sftp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/sftp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/sftp/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/sftp/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.376302 sdc_dp_helpers-1.4.1/sdc_dp_helpers/webvitalize/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/webvitalize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/webvitalize/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/webvitalize/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.376302 sdc_dp_helpers-1.4.1/sdc_dp_helpers/xero/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/xero/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/xero/config_managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/xero/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/xero/writers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12399 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/xero/xero_sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.380302 sdc_dp_helpers-1.4.1/sdc_dp_helpers/xml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/xml/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/xml/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.380302 sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_crm/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_crm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22264 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_crm/bulk_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_crm/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9897 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_crm/records_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     8650 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_crm/users_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_crm/writers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_crm/zoho_crm_sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.380302 sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_recruit/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_recruit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_recruit/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_recruit/writers.py
--rw-r--r--   0 runner    (1001) docker     (127)    28830 2024-05-28 08:05:44.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_recruit/zoho_recruit_sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:48.368301 sdc_dp_helpers-1.4.1/sdc_dp_helpers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-28 08:05:48.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-05-28 08:05:48.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 08:05:48.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-28 08:05:48.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-28 08:05:48.000000 sdc_dp_helpers-1.4.1/sdc_dp_helpers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-28 08:05:48.380302 sdc_dp_helpers-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-28 08:05:46.000000 sdc_dp_helpers-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:09.110511 sdc_dp_helpers-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-06-03 05:14:09.110511 sdc_dp_helpers-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:09.094511 sdc_dp_helpers-1.4.2/sdc_dp_helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:09.098511 sdc_dp_helpers-1.4.2/sdc_dp_helpers/api_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/api_utilities/__init_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/api_utilities/data_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21226 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/api_utilities/date_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/api_utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/api_utilities/file_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/api_utilities/retry_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/api_utilities/tracking_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:09.098511 sdc_dp_helpers-1.4.2/sdc_dp_helpers/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/azure/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/azure/writers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/base_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/base_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12994 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/base_writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:09.098511 sdc_dp_helpers-1.4.2/sdc_dp_helpers/facebook/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/facebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/facebook/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/facebook/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:09.098511 sdc_dp_helpers-1.4.2/sdc_dp_helpers/falcon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/falcon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29672 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/falcon/falcon_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/falcon/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/falcon/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:09.098511 sdc_dp_helpers-1.4.2/sdc_dp_helpers/ftp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/ftp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/ftp/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/ftp/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:09.098511 sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_ads/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_ads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_ads/generate_refresh_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_ads/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_ads/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:09.102511 sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_analytics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_analytics/config_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17311 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_analytics/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_analytics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_analytics/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:09.102511 sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_analytics_v4/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_analytics_v4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_analytics_v4/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_analytics_v4/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:09.102511 sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_big_query/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_big_query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_big_query/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_big_query/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:09.102511 sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_knowledge_graph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_knowledge_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_knowledge_graph/gkg_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_knowledge_graph/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_knowledge_graph/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:09.102511 sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_knowledge_graph_v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_knowledge_graph_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_knowledge_graph_v1/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_knowledge_graph_v1/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:09.102511 sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_postmaster_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_postmaster_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_postmaster_tools/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_postmaster_tools/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:09.102511 sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_search_console/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_search_console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8414 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_search_console/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_search_console/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:09.106511 sdc_dp_helpers-1.4.2/sdc_dp_helpers/onesignal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/onesignal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13915 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/onesignal/onesignal_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/onesignal/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/onesignal/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:09.106511 sdc_dp_helpers-1.4.2/sdc_dp_helpers/pyspark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/pyspark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/pyspark/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/pyspark/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:09.106511 sdc_dp_helpers-1.4.2/sdc_dp_helpers/sailthru/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/sailthru/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/sailthru/config_magagers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6708 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/sailthru/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/sailthru/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/sailthru/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:09.106511 sdc_dp_helpers-1.4.2/sdc_dp_helpers/sftp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/sftp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/sftp/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/sftp/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:09.106511 sdc_dp_helpers-1.4.2/sdc_dp_helpers/webvitalize/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/webvitalize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/webvitalize/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/webvitalize/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:09.106511 sdc_dp_helpers-1.4.2/sdc_dp_helpers/xero/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/xero/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/xero/config_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/xero/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/xero/writers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12694 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/xero/xero_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:09.106511 sdc_dp_helpers-1.4.2/sdc_dp_helpers/xml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/xml/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/xml/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:09.110511 sdc_dp_helpers-1.4.2/sdc_dp_helpers/zoho_crm/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/zoho_crm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22264 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/zoho_crm/bulk_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/zoho_crm/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9897 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/zoho_crm/records_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8650 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/zoho_crm/users_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/zoho_crm/writers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/zoho_crm/zoho_crm_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:09.110511 sdc_dp_helpers-1.4.2/sdc_dp_helpers/zoho_recruit/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/zoho_recruit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/zoho_recruit/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/zoho_recruit/writers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28830 2024-06-03 05:14:05.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers/zoho_recruit/zoho_recruit_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:14:09.098511 sdc_dp_helpers-1.4.2/sdc_dp_helpers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-06-03 05:14:08.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-06-03 05:14:09.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 05:14:08.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-06-03 05:14:08.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-03 05:14:08.000000 sdc_dp_helpers-1.4.2/sdc_dp_helpers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-06-03 05:14:09.110511 sdc_dp_helpers-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-06-03 05:14:07.000000 sdc_dp_helpers-1.4.2/setup.py
```

### Comparing `sdc_dp_helpers-1.4.1/README.md` & `sdc_dp_helpers-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/api_utilities/data_managers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/api_utilities/data_managers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/api_utilities/date_managers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/api_utilities/date_managers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/api_utilities/exceptions.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/api_utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/api_utilities/file_managers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/api_utilities/file_managers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/api_utilities/retry_managers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/api_utilities/retry_managers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/api_utilities/tracking_metadata.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/api_utilities/tracking_metadata.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/azure/readers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/azure/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/azure/writers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/azure/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/base_readers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/base_readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/base_writer.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/base_writer.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/base_writers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/base_writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/facebook/readers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/facebook/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/facebook/writers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/facebook/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/falcon/falcon_sdk.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/falcon/falcon_sdk.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/falcon/readers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/falcon/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/falcon/writers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/falcon/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/ftp/readers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/ftp/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/ftp/writers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/ftp/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_ads/generate_refresh_token.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_ads/generate_refresh_token.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_ads/readers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_ads/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_ads/writers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_ads/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_analytics/config_managers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_analytics/config_managers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_analytics/readers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_analytics/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_analytics/utils.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_analytics/utils.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_analytics/writers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_analytics/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_analytics_v4/readers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_analytics_v4/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_analytics_v4/writers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_analytics_v4/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_big_query/readers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_big_query/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_big_query/writers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_big_query/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_knowledge_graph/gkg_sdk.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_knowledge_graph/gkg_sdk.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_knowledge_graph/readers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_knowledge_graph/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_knowledge_graph/writers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_knowledge_graph/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_knowledge_graph_v1/readers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_knowledge_graph_v1/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_knowledge_graph_v1/writers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_knowledge_graph_v1/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_postmaster_tools/readers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_postmaster_tools/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_postmaster_tools/writers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_postmaster_tools/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_search_console/readers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_search_console/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/google_search_console/writers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/google_search_console/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/onesignal/onesignal_sdk.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/onesignal/onesignal_sdk.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/onesignal/readers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/onesignal/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/onesignal/writers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/onesignal/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/pyspark/utils.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/pyspark/utils.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/pyspark/writers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/pyspark/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/sailthru/readers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/sailthru/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/sailthru/utils.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/sailthru/utils.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/sailthru/writers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/sailthru/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/sftp/readers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/sftp/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/sftp/writers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/sftp/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/webvitalize/readers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/webvitalize/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/webvitalize/writers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/webvitalize/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/xero/readers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/xero/readers.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,73 +18,89 @@
 
     def _get_auth(self):
         """Authenticate."""
         self.service = XeroAPICall(config=self.config, creds_path=self.creds_path)
         return self.service
 
     def _query_handler(
-        self, report: str, start_date:str, end_date:str, tracking_category: str, filterby: str
+        self,
+        tenant_id,
+        report: str,
+        start_date: str,
+        end_date: str,
+        tracking_category: str,
+        filterby: str,
     ):
         """Runs a simple reports."""
         data = self.service.get_reports(
-            report, start_date,end_date, tracking_category, filterby
+            tenant_id, report, start_date, end_date, tracking_category, filterby
         )
         return data
 
     def run_query(self):
         """Controls the Flow of Query"""
         payload = []
         if self.config.get("report"):
-            trackingcategories = GetTrackingCategories(
-                config=self.config, creds_filepath=self.creds_path).make_api_call()
-            for tracking_category in trackingcategories:
-                for filterby in self.config['filters']:
+            for tenants_name, tenant_id in self.config.get("tenants").items():
+                trackingcategories = GetTrackingCategories(
+                    config=self.config, creds_filepath=self.creds_path
+                ).make_api_call(tenant_id)
+                for tracking_category in trackingcategories:
+                    for filterby in self.config["filters"]:
+                        for start_date, end_date in date_range_iterator(
+                            start_date=self.config["start_date"],
+                            end_date=self.config["end_date"],
+                            interval=self.config["interval"],
+                            end_inclusive=True,
+                            time_format="%Y-%m-%d",
+                            ytd=self.config.get("ytd", False),
+                        ):
+                            payload = self._query_handler(
+                                tenant_id,
+                                self.config.get("report"),
+                                start_date,
+                                end_date,
+                                tracking_category,
+                                filterby,
+                            )
+                            yield {
+                                "endpoint": self.config.get("report"),
+                                "tenant_name": tenants_name,
+                                "trackingCategoryId": tracking_category[
+                                    "TrackingCategoryID"
+                                ],
+                                "data": payload,
+                                "date": end_date,
+                                "filterby": filterby,
+                            }
+                            self.is_success()
+                            if not payload:
+                                self.not_success()
+                                print(
+                                    f"""No data for {self.config.get("report")} Report for start_date {start_date} and end_date {end_date}"""
+                                )
+        if self.config.get("modules"):
+            for tenants_name, tenant_id in self.config.get("tenants").items():
+                for module in self.config.get("modules", []):
                     for start_date, end_date in date_range_iterator(
-                        start_date=self.config['start_date'],
-                        end_date=self.config['end_date'],
-                        interval=self.config['interval'],
+                        start_date=self.config["start_date"],
+                        end_date=self.config["end_date"],
+                        interval=self.config["interval"],
                         end_inclusive=True,
                         time_format="%Y-%m-%d",
-                        ytd=self.config.get("ytd", False),
                     ):
-                        payload = self._query_handler(
-                            self.config.get("report"), start_date, end_date, tracking_category, filterby
+                        payload = self.service.get_modules(
+                            tenant_id, module, start_date, end_date
                         )
                         yield {
-                            "endpoint": self.config.get("report"),
-                            "tenant_name": self.config["tenant_name"],
-                            "trackingCategoryId": tracking_category[
-                                "TrackingCategoryID"
-                            ],
+                            "endpoint": module,
+                            "tenant_name": tenants_name,
                             "data": payload,
                             "date": end_date,
-                            "filterby": filterby,
+                            "trackingCategoryId": "",
                         }
                         self.is_success()
                         if not payload:
                             self.not_success()
                             print(
-                                f"""No data for {self.config.get("report")} Report for start_date {start_date} and end_date {end_date}"""
+                                f"""No data for {module} Module for start_date {start_date} and end_date {end_date}"""
                             )
-        if self.config.get("modules"):
-            for module in self.config.get("modules", []):
-                for start_date, end_date in date_range_iterator(
-                    start_date=self.config["start_date"],
-                    end_date=self.config["end_date"],
-                    interval=self.config["interval"],
-                    end_inclusive=True,
-                    time_format="%Y-%m-%d",
-                ):
-                    payload = self.service.get_modules(module, start_date, end_date)
-                    yield {
-                        "endpoint": module,
-                        "tenant_name": self.config["tenant_name"],
-                        "data": payload,
-                        "date": end_date,
-                        "trackingCategoryId": "",
-                    }
-                    self.is_success()
-                    if not payload:
-                        self.not_success()
-                        print(
-                            f"""No data for {module} Module for start_date {start_date} and end_date {end_date}"""
-                        )
```

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/xero/writers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/xero/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/xero/xero_sdk.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/xero/xero_sdk.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,14 +107,15 @@
 
     def __init__(self, creds_path, config):
         self.creds_filepath = creds_path
         self.config = config
 
     def get_reports(
         self,
+        tenant_id,
         report_name: str,
         start_date: str,
         end_date: str,
         tracking_category: str,
         filterby: str,
     ):
         """Get reports data"""
@@ -122,89 +123,95 @@
             "bytrackingoption": ReportsByTrackingOption,
             "notfiltered": ReportsNotFiltered,
         }
         method_ids_caller = get_data_methods[filterby](
             config=self.config, creds_filepath=self.creds_filepath
         )
         data = method_ids_caller.make_api_call(
-            report_name, start_date,end_date, tracking_category
+            tenant_id, report_name, start_date, end_date, tracking_category
         )
         return data
 
-    def get_modules(self, module, start_date, end_date):
+    def get_modules(self, tenant_id, module, start_date, end_date):
         """Get modules data"""
         module_ = Modules(config=self.config, creds_filepath=self.creds_filepath)
-        results = module_.make_api_call(module, start_date, end_date)
+        results = module_.make_api_call(tenant_id, module, start_date, end_date)
         return results
 
-    def get_tracking_categories(self):
+    def get_tracking_categories(self, tenant_id):
         """Get tracking categories data"""
         categories = GetTrackingCategories(
             config=self.config, creds_filepath=self.creds_filepath
         )
-        results = categories.make_api_call()
+        results = categories.make_api_call(tenant_id)
         return results
 
 
 class ReportsNotFiltered(RequestHandler):
     "Class for not Filtered reports"
 
-    def make_api_call(self, report_name, start_date, end_date, tracking_category):
+    def make_api_call(
+        self, tenant_id, report_name, start_date, end_date, tracking_category
+    ):
         request_params = {}
         auth_token = self.authenticator.get_auth_token()
         option_id = None
         request_params.update(
             {"trackingCategoryID": tracking_category["TrackingCategoryID"]}
         )
         report = get_report(
             self.config,
+            tenant_id,
             auth_token,
             start_date,
             end_date,
-            option_id,
             report_name,
             request_params,
         )
+        report = normalize(report, tenant_id, option_id)
         return [report]
 
 
 class GetTrackingCategories(RequestHandler):
     "class to get Reports filtered by Tracking categories"
 
-    def make_api_call(self):
+    def make_api_call(self, tenant_id):
         auth_token = self.authenticator.get_auth_token()
-        auth_token.tenant_id = self.config.get("tenant_id")
+        auth_token.tenant_id = tenant_id
         xero_obj = Xero(auth_token)
         trackingcategories = (
             i for i in xero_obj.trackingcategories.all() if i is not None
         )
         return trackingcategories
 
 
 class ReportsByTrackingOption(RequestHandler):
     "class to get Reports filtered by TrackingOptionID"
 
-    def make_api_call(self, report_name, start_date, end_date, tracking_category):
+    def make_api_call(
+        self, tenant_id, report_name, start_date, end_date, tracking_category
+    ):
         request_params = {}
         auth_token = self.authenticator.get_auth_token()
         option_data = []
         for option_id in tracking_category["Options"]:
             request_params.update(
                 {"trackingCategoryID": tracking_category["TrackingCategoryID"]}
             )
             request_params.update({"TrackingOptionID": option_id["TrackingOptionID"]})
             report = get_report(
                 self.config,
+                tenant_id,
                 auth_token,
                 start_date,
                 end_date,
-                option_id,
                 report_name,
                 request_params,
             )
+            report = normalize(report, tenant_id, option_id)
             option_data.append(report)
         return option_data
 
 
 class Modules(RequestHandler):
     "class to get Modules"
 
@@ -225,20 +232,20 @@
         # XeroRateLimitExceeded
         else:
             return api_call.filter(
                 raw=date_filter_helper(request["from_date"], request["to_date"]),
                 page=request["page"],
             )
 
-    def make_api_call(self, module, start_date, end_date):
+    def make_api_call(self, tenant_id, module, start_date, end_date):
         """
         API call to get module data
         """
         auth_token = self.authenticator.get_auth_token()
-        auth_token.tenant_id = self.config.get("tenant_id")
+        auth_token.tenant_id = tenant_id
         xero = Xero(auth_token)
         data = []
         if module not in ["accounts", "trackingcategories", "currencies"]:
             raise ValueError(module + " is not supported or does not exist.")
         prev_response = None
         page = 1
         while True:
@@ -268,52 +275,61 @@
             page += 1
         return data
 
 
 ############### helper functions
 
 
-@retry_handler(exceptions=XeroQuotaException, total_tries=5, initial_wait=1)
-def get_report(configs,
-    auth_token, start_date, end_date, option_id, report_name, request_params
+@request_handler(
+    wait=float(os.environ.get("API_WAIT_TIME", 5)),
+    backoff_factor=0.01,
+    backoff_method="random",
+)
+@retry_handler(
+    exceptions=XeroQuotaException,
+    total_tries=5,
+    initial_wait=61,
+    backoff_factor=1.2,
+)
+def get_report(
+    configs, tenant_id, auth_token, start_date, end_date, report_name, request_params
 ):
     """Get single report data"""
     if report_name in ["ProfitAndLoss"]:
         request_params.update({"fromDate": start_date})
         request_params.update({"toDate": end_date})
 
     if report_name in ["BalanceSheet"]:
         request_params.update({"date": end_date})
         request_params.update({"timeframe": configs.get("timeframe")})
         request_params.update({"periods": configs.get("periods")})
     headers = {
         "Authorization": "Bearer " + auth_token.token["access_token"],
-        "Xero-Tenant-Id": configs['tenant_id'],
+        "Xero-Tenant-Id": tenant_id,
         "Accept": "application/json",
     }
     try:
         response = requests.get(
             "https://api.xero.com/api.xro/2.0/Reports/" + report_name,
             params=request_params,
             headers=headers,
             timeout=30,
         )
-        report = json.loads(
-            response.text.replace("\r", "").replace("\n", "").strip("'<>() ")
-        )
-        report = normalize(report, configs['tenant_id'], option_id=option_id)
     except Exception as err:
         if err.code == 429:
             raise XeroQuotaException(
                 f"Xero Quota Reached" f"Status code: {err.code}, Reason: {err.reason}. "
             ) from err
-    return report
+    return response
 
 
-def normalize(report, tenant_id, option_id=None):
+def normalize(response, tenant_id, option_id=None):
+    report = json.loads(
+        response.text.replace("\r", "").replace("\n", "").strip("'<>() ")
+    )
     for row in range(len(report["Reports"][0]["Rows"])):
         period = report["Reports"][0]["Rows"][0]["Cells"]
         try:
             for report_ in report["Reports"][0]["Rows"][row]["Rows"]:
                 for idx, cells in enumerate(report_["Cells"]):
                     cells["Attributes"][0].update(
                         {"type": report_["Cells"][0]["Value"]}
```

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/xml/readers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/xml/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/xml/writers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/xml/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_crm/bulk_endpoint.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/zoho_crm/bulk_endpoint.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_crm/readers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/zoho_crm/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_crm/records_endpoint.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/zoho_crm/records_endpoint.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_crm/users_endpoint.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/zoho_crm/users_endpoint.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_crm/writers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/zoho_crm/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_crm/zoho_crm_sdk.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/zoho_crm/zoho_crm_sdk.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_recruit/readers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/zoho_recruit/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_recruit/writers.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/zoho_recruit/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers/zoho_recruit/zoho_recruit_sdk.py` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers/zoho_recruit/zoho_recruit_sdk.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/sdc_dp_helpers.egg-info/SOURCES.txt` & `sdc_dp_helpers-1.4.2/sdc_dp_helpers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.4.1/setup.py` & `sdc_dp_helpers-1.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,19 +71,19 @@
         "paramiko",
         "google-cloud-enterpriseknowledgegraph>=0.3.3",
     ],
     extras_require={"pyspark": ["pyspark"]},
     cmdclass={"sdist_zip": sdistzip},
     description="A module for developing data pipelines from external api's and on ETL like services",
 
-    version="1.4.1",
+    version="1.4.2",
 
     url="http://github.com/RingierIMU/sdc-dataPipeline-helpers",
     author="Ringier South Africa",
     author_email="tools@ringier.co.za",
     keywords=[
         "pip",
         "datapipeline",
         "helpers",
     ],
-    download_url="https://github.com/RingierIMU/sdc-global-dataPipeline-helpers/archive/v1.4.1.zip",
+    download_url="https://github.com/RingierIMU/sdc-global-dataPipeline-helpers/archive/v1.4.2.zip",
 )
```

