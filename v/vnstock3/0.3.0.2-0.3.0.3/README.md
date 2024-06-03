# Comparing `tmp/vnstock3-0.3.0.2.tar.gz` & `tmp/vnstock3-0.3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnstock3-0.3.0.2.tar", last modified: Sat May 25 03:09:40 2024, max compression
+gzip compressed data, was "vnstock3-0.3.0.3.tar", last modified: Sun Jun  2 18:17:52 2024, max compression
```

## Comparing `vnstock3-0.3.0.2.tar` & `vnstock3-0.3.0.3.tar`

### file list

```diff
@@ -1,101 +1,105 @@
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.963868 vnstock3-0.3.0.2/
--rw-r--r--   0 mrthinh    (501) staff       (20)     8376 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/LICENSE.md
--rw-r--r--   0 mrthinh    (501) staff       (20)    15714 2024-05-25 03:09:40.963513 vnstock3-0.3.0.2/PKG-INFO
--rw-r--r--   0 mrthinh    (501) staff       (20)     5665 2024-05-24 20:48:14.000000 vnstock3-0.3.0.2/README.md
--rw-r--r--   0 mrthinh    (501) staff       (20)     1019 2024-05-24 17:09:16.000000 vnstock3-0.3.0.2/pyproject.toml
--rw-r--r--   0 mrthinh    (501) staff       (20)       38 2024-05-25 03:09:40.963909 vnstock3-0.3.0.2/setup.cfg
--rw-r--r--   0 mrthinh    (501) staff       (20)     1231 2024-05-24 17:09:06.000000 vnstock3-0.3.0.2/setup.py
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.952639 vnstock3-0.3.0.2/tests/
--rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:36:22.000000 vnstock3-0.3.0.2/tests/__init__.py
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.953069 vnstock3-0.3.0.2/tests/common/
--rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.2/tests/common/__init__.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     7575 2024-05-25 03:08:48.000000 vnstock3-0.3.0.2/tests/common/test_data_explorer.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     1783 2024-05-24 20:39:40.000000 vnstock3-0.3.0.2/tests/config.py
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.953694 vnstock3-0.3.0.2/tests/core/
--rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.2/tests/core/__init__.py
--rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.2/tests/core/test_config.py
--rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.2/tests/core/test_converter.py
--rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.2/tests/core/test_utils.py
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.953794 vnstock3-0.3.0.2/tests/explorer/
--rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.2/tests/explorer/__init__.py
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.954126 vnstock3-0.3.0.2/tests/explorer/misc/
--rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.2/tests/explorer/misc/__init__.py
--rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.2/tests/explorer/misc/test_exchange_rate.py
--rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.2/tests/explorer/misc/test_gold_price.py
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.954320 vnstock3-0.3.0.2/tests/explorer/msn/
--rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.2/tests/explorer/msn/__init__.py
--rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.2/tests/explorer/msn/test_quote.py
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.954769 vnstock3-0.3.0.2/tests/explorer/tcbs/
--rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.2/tests/explorer/tcbs/__init__.py
--rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.2/tests/explorer/tcbs/test_analysis.py
--rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.2/tests/explorer/tcbs/test_company.py
--rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.2/tests/explorer/tcbs/test_quote.py
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.955300 vnstock3-0.3.0.2/tests/explorer/vci/
--rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.2/tests/explorer/vci/__init__.py
--rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.2/tests/explorer/vci/test_analysis.py
--rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.2/tests/explorer/vci/test_company.py
--rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.2/tests/explorer/vci/test_quote.py
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.955428 vnstock3-0.3.0.2/vnstock3/
--rw-r--r--   0 mrthinh    (501) staff       (20)      104 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/__init__.py
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.956291 vnstock3-0.3.0.2/vnstock3/common/
--rw-r--r--   0 mrthinh    (501) staff       (20)      168 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/common/__init__.py
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.956522 vnstock3-0.3.0.2/vnstock3/common/data/
--rw-r--r--   0 mrthinh    (501) staff       (20)       28 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/common/data/__init__.py
--rw-r--r--   0 mrthinh    (501) staff       (20)    17660 2024-05-25 02:32:16.000000 vnstock3-0.3.0.2/vnstock3/common/data/data_explorer.py
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.956996 vnstock3-0.3.0.2/vnstock3/core/
--rw-r--r--   0 mrthinh    (501) staff       (20)      110 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/core/__init__.py
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.957421 vnstock3-0.3.0.2/vnstock3/core/config/
--rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/core/config/__init__.py
--rw-r--r--   0 mrthinh    (501) staff       (20)       16 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/core/config/auth.py
--rw-r--r--   0 mrthinh    (501) staff       (20)      725 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/core/config/const.py
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.957651 vnstock3-0.3.0.2/vnstock3/core/converter/
--rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/core/converter/__init__.py
--rw-r--r--   0 mrthinh    (501) staff       (20)      453 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/core/converter/export.py
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.958694 vnstock3-0.3.0.2/vnstock3/core/utils/
--rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/core/utils/__init__.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     1160 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/core/utils/env.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     1651 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/core/utils/ext.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     1056 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/core/utils/help.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     1487 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/core/utils/launcher.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     3202 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/core/utils/logger.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     5617 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/core/utils/parser.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     1747 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/core/utils/user_agent.py
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.958836 vnstock3-0.3.0.2/vnstock3/explorer/
--rw-r--r--   0 mrthinh    (501) staff       (20)       56 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/__init__.py
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.959198 vnstock3-0.3.0.2/vnstock3/explorer/misc/
--rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/misc/__init__.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     1438 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/misc/exchange_rate.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     2605 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/misc/gold_price.py
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.960010 vnstock3-0.3.0.2/vnstock3/explorer/msn/
--rw-r--r--   0 mrthinh    (501) staff       (20)       43 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/msn/__init__.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     4105 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/msn/const.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     1814 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/msn/helper.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     2832 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/msn/listing.py
--rw-r--r--   0 mrthinh    (501) staff       (20)      276 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/msn/models.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     7301 2024-05-24 18:33:19.000000 vnstock3-0.3.0.2/vnstock3/explorer/msn/quote.py
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.961357 vnstock3-0.3.0.2/vnstock3/explorer/tcbs/
--rw-r--r--   0 mrthinh    (501) staff       (20)      138 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/tcbs/__init__.py
--rw-r--r--   0 mrthinh    (501) staff       (20)       53 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/tcbs/analysis.py
--rw-r--r--   0 mrthinh    (501) staff       (20)    14574 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/tcbs/company.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     3576 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/tcbs/const.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     9466 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/tcbs/financial.py
--rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/tcbs/listing.py
--rw-r--r--   0 mrthinh    (501) staff       (20)      738 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/tcbs/models.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     9684 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/tcbs/quote.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     2267 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/tcbs/trading.py
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.962720 vnstock3-0.3.0.2/vnstock3/explorer/vci/
--rw-r--r--   0 mrthinh    (501) staff       (20)      138 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/vci/__init__.py
--rw-r--r--   0 mrthinh    (501) staff       (20)       23 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/vci/analysis.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     5722 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/vci/company.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     2340 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/vci/const.py
--rw-r--r--   0 mrthinh    (501) staff       (20)    13079 2024-05-25 01:53:24.000000 vnstock3-0.3.0.2/vnstock3/explorer/vci/financial.py
--rw-r--r--   0 mrthinh    (501) staff       (20)    10702 2024-05-24 16:17:17.000000 vnstock3-0.3.0.2/vnstock3/explorer/vci/listing.py
--rw-r--r--   0 mrthinh    (501) staff       (20)      276 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/vci/models.py
--rw-r--r--   0 mrthinh    (501) staff       (20)    11513 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/vci/quote.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     4147 2024-05-24 18:33:49.000000 vnstock3-0.3.0.2/vnstock3/explorer/vci/trading.py
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.962984 vnstock3-0.3.0.2/vnstock3.egg-info/
--rw-r--r--   0 mrthinh    (501) staff       (20)    15714 2024-05-25 03:09:40.000000 vnstock3-0.3.0.2/vnstock3.egg-info/PKG-INFO
--rw-r--r--   0 mrthinh    (501) staff       (20)     2362 2024-05-25 03:09:40.000000 vnstock3-0.3.0.2/vnstock3.egg-info/SOURCES.txt
--rw-r--r--   0 mrthinh    (501) staff       (20)        1 2024-05-25 03:09:40.000000 vnstock3-0.3.0.2/vnstock3.egg-info/dependency_links.txt
--rw-r--r--   0 mrthinh    (501) staff       (20)      146 2024-05-25 03:09:40.000000 vnstock3-0.3.0.2/vnstock3.egg-info/requires.txt
--rw-r--r--   0 mrthinh    (501) staff       (20)       15 2024-05-25 03:09:40.000000 vnstock3-0.3.0.2/vnstock3.egg-info/top_level.txt
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-06-02 18:17:52.335189 vnstock3-0.3.0.3/
+-rw-r--r--   0 mrthinh    (501) staff       (20)     8376 2024-05-16 18:32:12.000000 vnstock3-0.3.0.3/LICENSE.md
+-rw-r--r--   0 mrthinh    (501) staff       (20)    15714 2024-06-02 18:17:52.334886 vnstock3-0.3.0.3/PKG-INFO
+-rw-r--r--   0 mrthinh    (501) staff       (20)     5665 2024-05-24 20:48:14.000000 vnstock3-0.3.0.3/README.md
+-rw-r--r--   0 mrthinh    (501) staff       (20)     1019 2024-06-02 18:17:13.000000 vnstock3-0.3.0.3/pyproject.toml
+-rw-r--r--   0 mrthinh    (501) staff       (20)       38 2024-06-02 18:17:52.335229 vnstock3-0.3.0.3/setup.cfg
+-rw-r--r--   0 mrthinh    (501) staff       (20)     1231 2024-06-02 18:17:06.000000 vnstock3-0.3.0.3/setup.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-06-02 18:17:52.319019 vnstock3-0.3.0.3/tests/
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:36:22.000000 vnstock3-0.3.0.3/tests/__init__.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-06-02 18:17:52.319582 vnstock3-0.3.0.3/tests/common/
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.3/tests/common/__init__.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     7610 2024-06-01 02:16:05.000000 vnstock3-0.3.0.3/tests/common/test_data_explorer.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     1783 2024-05-24 20:39:40.000000 vnstock3-0.3.0.3/tests/config.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-06-02 18:17:52.320379 vnstock3-0.3.0.3/tests/core/
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.3/tests/core/__init__.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.3/tests/core/test_config.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.3/tests/core/test_converter.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.3/tests/core/test_utils.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-06-02 18:17:52.320475 vnstock3-0.3.0.3/tests/explorer/
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.3/tests/explorer/__init__.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-06-02 18:17:52.320765 vnstock3-0.3.0.3/tests/explorer/misc/
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.3/tests/explorer/misc/__init__.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.3/tests/explorer/misc/test_exchange_rate.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.3/tests/explorer/misc/test_gold_price.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-06-02 18:17:52.320970 vnstock3-0.3.0.3/tests/explorer/msn/
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.3/tests/explorer/msn/__init__.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.3/tests/explorer/msn/test_quote.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-06-02 18:17:52.321451 vnstock3-0.3.0.3/tests/explorer/tcbs/
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.3/tests/explorer/tcbs/__init__.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.3/tests/explorer/tcbs/test_analysis.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.3/tests/explorer/tcbs/test_company.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.3/tests/explorer/tcbs/test_quote.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-06-02 18:17:52.321896 vnstock3-0.3.0.3/tests/explorer/vci/
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.3/tests/explorer/vci/__init__.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.3/tests/explorer/vci/test_analysis.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.3/tests/explorer/vci/test_company.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.3/tests/explorer/vci/test_quote.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-06-02 18:17:52.321998 vnstock3-0.3.0.3/vnstock3/
+-rw-r--r--   0 mrthinh    (501) staff       (20)      231 2024-06-01 03:15:50.000000 vnstock3-0.3.0.3/vnstock3/__init__.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-06-02 18:17:52.323400 vnstock3-0.3.0.3/vnstock3/common/
+-rw-r--r--   0 mrthinh    (501) staff       (20)      176 2024-06-01 02:13:36.000000 vnstock3-0.3.0.3/vnstock3/common/__init__.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-06-02 18:17:52.323998 vnstock3-0.3.0.3/vnstock3/common/data/
+-rw-r--r--   0 mrthinh    (501) staff       (20)       28 2024-05-16 18:32:12.000000 vnstock3-0.3.0.3/vnstock3/common/data/__init__.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)    16073 2024-06-01 03:17:53.000000 vnstock3-0.3.0.3/vnstock3/common/data/data_explorer.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-06-02 18:17:52.324605 vnstock3-0.3.0.3/vnstock3/common/plot/
+-rw-r--r--   0 mrthinh    (501) staff       (20)       32 2024-06-01 03:07:46.000000 vnstock3-0.3.0.3/vnstock3/common/plot/__init__.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     8806 2024-06-02 16:30:07.000000 vnstock3-0.3.0.3/vnstock3/common/plot/chart_wrapper.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     1886 2024-06-01 02:08:35.000000 vnstock3-0.3.0.3/vnstock3/common/vnstock.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-06-02 18:17:52.325176 vnstock3-0.3.0.3/vnstock3/core/
+-rw-r--r--   0 mrthinh    (501) staff       (20)      110 2024-05-16 18:32:12.000000 vnstock3-0.3.0.3/vnstock3/core/__init__.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-06-02 18:17:52.325746 vnstock3-0.3.0.3/vnstock3/core/config/
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-16 18:32:12.000000 vnstock3-0.3.0.3/vnstock3/core/config/__init__.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)       16 2024-05-16 18:32:12.000000 vnstock3-0.3.0.3/vnstock3/core/config/auth.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)      725 2024-05-16 18:32:12.000000 vnstock3-0.3.0.3/vnstock3/core/config/const.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-06-02 18:17:52.326372 vnstock3-0.3.0.3/vnstock3/core/converter/
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-16 18:32:12.000000 vnstock3-0.3.0.3/vnstock3/core/converter/__init__.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)      453 2024-05-16 18:32:12.000000 vnstock3-0.3.0.3/vnstock3/core/converter/export.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-06-02 18:17:52.327674 vnstock3-0.3.0.3/vnstock3/core/utils/
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-16 18:32:12.000000 vnstock3-0.3.0.3/vnstock3/core/utils/__init__.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     1160 2024-05-16 18:32:12.000000 vnstock3-0.3.0.3/vnstock3/core/utils/env.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     1651 2024-05-16 18:32:12.000000 vnstock3-0.3.0.3/vnstock3/core/utils/ext.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     1056 2024-05-16 18:32:12.000000 vnstock3-0.3.0.3/vnstock3/core/utils/help.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     1487 2024-05-16 18:32:12.000000 vnstock3-0.3.0.3/vnstock3/core/utils/launcher.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     3202 2024-05-16 18:32:12.000000 vnstock3-0.3.0.3/vnstock3/core/utils/logger.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     5617 2024-05-16 18:32:12.000000 vnstock3-0.3.0.3/vnstock3/core/utils/parser.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     1747 2024-05-16 18:32:12.000000 vnstock3-0.3.0.3/vnstock3/core/utils/user_agent.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-06-02 18:17:52.327814 vnstock3-0.3.0.3/vnstock3/explorer/
+-rw-r--r--   0 mrthinh    (501) staff       (20)       56 2024-05-16 18:32:12.000000 vnstock3-0.3.0.3/vnstock3/explorer/__init__.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-06-02 18:17:52.328224 vnstock3-0.3.0.3/vnstock3/explorer/misc/
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-16 18:32:12.000000 vnstock3-0.3.0.3/vnstock3/explorer/misc/__init__.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     1438 2024-05-16 18:32:12.000000 vnstock3-0.3.0.3/vnstock3/explorer/misc/exchange_rate.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     2605 2024-05-16 18:32:12.000000 vnstock3-0.3.0.3/vnstock3/explorer/misc/gold_price.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-06-02 18:17:52.330072 vnstock3-0.3.0.3/vnstock3/explorer/msn/
+-rw-r--r--   0 mrthinh    (501) staff       (20)       43 2024-05-16 18:32:12.000000 vnstock3-0.3.0.3/vnstock3/explorer/msn/__init__.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     4105 2024-05-16 18:32:12.000000 vnstock3-0.3.0.3/vnstock3/explorer/msn/const.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     2363 2024-05-28 20:48:49.000000 vnstock3-0.3.0.3/vnstock3/explorer/msn/helper.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     2879 2024-06-02 06:11:43.000000 vnstock3-0.3.0.3/vnstock3/explorer/msn/listing.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)      276 2024-05-16 18:32:12.000000 vnstock3-0.3.0.3/vnstock3/explorer/msn/models.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     7329 2024-05-28 21:00:35.000000 vnstock3-0.3.0.3/vnstock3/explorer/msn/quote.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-06-02 18:17:52.332189 vnstock3-0.3.0.3/vnstock3/explorer/tcbs/
+-rw-r--r--   0 mrthinh    (501) staff       (20)      138 2024-05-16 18:32:12.000000 vnstock3-0.3.0.3/vnstock3/explorer/tcbs/__init__.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)       53 2024-05-16 18:32:12.000000 vnstock3-0.3.0.3/vnstock3/explorer/tcbs/analysis.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)    14574 2024-05-16 18:32:12.000000 vnstock3-0.3.0.3/vnstock3/explorer/tcbs/company.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     3576 2024-05-16 18:32:12.000000 vnstock3-0.3.0.3/vnstock3/explorer/tcbs/const.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     9466 2024-05-16 18:32:12.000000 vnstock3-0.3.0.3/vnstock3/explorer/tcbs/financial.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-16 18:32:12.000000 vnstock3-0.3.0.3/vnstock3/explorer/tcbs/listing.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)      738 2024-05-16 18:32:12.000000 vnstock3-0.3.0.3/vnstock3/explorer/tcbs/models.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     9684 2024-05-16 18:32:12.000000 vnstock3-0.3.0.3/vnstock3/explorer/tcbs/quote.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     2267 2024-05-16 18:32:12.000000 vnstock3-0.3.0.3/vnstock3/explorer/tcbs/trading.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-06-02 18:17:52.333983 vnstock3-0.3.0.3/vnstock3/explorer/vci/
+-rw-r--r--   0 mrthinh    (501) staff       (20)      138 2024-05-16 18:32:12.000000 vnstock3-0.3.0.3/vnstock3/explorer/vci/__init__.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)       23 2024-05-16 18:32:12.000000 vnstock3-0.3.0.3/vnstock3/explorer/vci/analysis.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     5722 2024-05-16 18:32:12.000000 vnstock3-0.3.0.3/vnstock3/explorer/vci/company.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     2340 2024-05-16 18:32:12.000000 vnstock3-0.3.0.3/vnstock3/explorer/vci/const.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)    13079 2024-05-25 01:53:24.000000 vnstock3-0.3.0.3/vnstock3/explorer/vci/financial.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)    10702 2024-05-24 16:17:17.000000 vnstock3-0.3.0.3/vnstock3/explorer/vci/listing.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)      276 2024-05-16 18:32:12.000000 vnstock3-0.3.0.3/vnstock3/explorer/vci/models.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)    11513 2024-05-16 18:32:12.000000 vnstock3-0.3.0.3/vnstock3/explorer/vci/quote.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     4147 2024-05-24 18:33:49.000000 vnstock3-0.3.0.3/vnstock3/explorer/vci/trading.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-06-02 18:17:52.334360 vnstock3-0.3.0.3/vnstock3.egg-info/
+-rw-r--r--   0 mrthinh    (501) staff       (20)    15714 2024-06-02 18:17:52.000000 vnstock3-0.3.0.3/vnstock3.egg-info/PKG-INFO
+-rw-r--r--   0 mrthinh    (501) staff       (20)     2460 2024-06-02 18:17:52.000000 vnstock3-0.3.0.3/vnstock3.egg-info/SOURCES.txt
+-rw-r--r--   0 mrthinh    (501) staff       (20)        1 2024-06-02 18:17:52.000000 vnstock3-0.3.0.3/vnstock3.egg-info/dependency_links.txt
+-rw-r--r--   0 mrthinh    (501) staff       (20)      146 2024-06-02 18:17:52.000000 vnstock3-0.3.0.3/vnstock3.egg-info/requires.txt
+-rw-r--r--   0 mrthinh    (501) staff       (20)       15 2024-06-02 18:17:52.000000 vnstock3-0.3.0.3/vnstock3.egg-info/top_level.txt
```

### Comparing `vnstock3-0.3.0.2/LICENSE.md` & `vnstock3-0.3.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.2/PKG-INFO` & `vnstock3-0.3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnstock3
-Version: 0.3.0.2
+Version: 0.3.0.3
 Summary: A comprehensive and transparent solution for Vietnamese stock market analysis.
 Home-page: https://github.com/thinh-vu/vnstock
 Author: Thinh Vu
 Author-email: Thinh Vu <mrthinh@live.com>
 License: **GIẤY PHÉP SỬ DỤNG PHẦN MỀM VNSTOCK3**
         -----------------------------------
```

### Comparing `vnstock3-0.3.0.2/README.md` & `vnstock3-0.3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.2/pyproject.toml` & `vnstock3-0.3.0.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 # Metadata Information
 [project]
 name = "vnstock3"
-version = "0.3.0.2"
+version = "0.3.0.3"
 description = "A comprehensive and transparent solution for Vietnamese stock market analysis."
 authors = [
     { name = "Thinh Vu", email = "mrthinh@live.com" },
     ]
 license = { file = "LICENSE.md" }
 requires-python = ">=3.10"
 readme = { file = "README.md", content-type = "text/markdown" }
```

### Comparing `vnstock3-0.3.0.2/setup.py` & `vnstock3-0.3.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import shutil
 import subprocess
 from setuptools import setup, find_packages, Command
 from setuptools.command.install import install
 
 setup(
     name="vnstock3",
-    version="0.3.0.2",
+    version="0.3.0.3",
     description="A comprehensive and transparent solution for Vietnamese stock market analysis.",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     author="Thinh Vu",
     author_email="mrthinh@live.com",
     url="https://github.com/thinh-vu/vnstock",
     classifiers=[
```

### Comparing `vnstock3-0.3.0.2/tests/common/test_data_explorer.py` & `vnstock3-0.3.0.3/tests/common/test_data_explorer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import unittest
 from unittest.mock import patch, MagicMock
 import pandas as pd
-from vnstock3.common.data.data_explorer import Vnstock, StockComponents, Quote, Listing, Trading, Company, Finance, MSNComponents
+from vnstock3.common.data.data_explorer import StockComponents, Quote, Listing, Trading, Company, Finance, MSNComponents
+from vnstock3.common.vnstock import Vnstock
 from vnstock3.explorer.msn.const import _CURRENCY_ID_MAP, _GLOBAL_INDICES, _CRYPTO_ID_MAP
 msn_symbol_map = {**_CURRENCY_ID_MAP, **_GLOBAL_INDICES, **_CRYPTO_ID_MAP}
 
 class TestVnstock(unittest.TestCase):
 
     def test_vnstock_init_valid_source(self):
         vnstock = Vnstock(source="VCI")
```

### Comparing `vnstock3-0.3.0.2/tests/config.py` & `vnstock3-0.3.0.3/tests/config.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.2/vnstock3/common/data/data_explorer.py` & `vnstock3-0.3.0.3/vnstock3/common/data/data_explorer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,55 +1,15 @@
 import importlib
 from typing import Optional
 from vnstock3.core.utils.logger import get_logger
 from vnstock3.explorer.msn.const import _CURRENCY_ID_MAP, _GLOBAL_INDICES, _CRYPTO_ID_MAP
 from vnstock3.core.utils.parser import get_asset_type
-from functools import wraps
+# from functools import wraps
 
 logger = get_logger(__name__)
-
-class Vnstock:
-    """
-    Class (lớp) chính quản lý các chức năng của thư viện Vnstock.
-    """
-    
-    SUPPORTED_SOURCES = ["VCI", "TCBS", "MSN"]
-    msn_symbol_map = {**_CURRENCY_ID_MAP, **_GLOBAL_INDICES, **_CRYPTO_ID_MAP}
-
-    def __init__(self, source:str="VCI"):
-        self.source = source.upper()
-        if self.source not in self.SUPPORTED_SOURCES:
-            raise ValueError(F"Hiện tại chỉ có nguồn dữ liệu từ {', '.join(self.SUPPORTED_SOURCES)} được hỗ trợ.")
-        self.source = source.upper()
-        # self.utils = Utils(self)
-
-    def stock(self, symbol: Optional[str]=None, source: Optional[str] = "VCI"):
-        if symbol is None:
-            self.symbol = 'VN30F1M'
-            logger.info("Mã chứng khoán không được chỉ định, chương trình mặc định sử dụng VN30F1M")
-        else:
-            self.symbol = symbol
-        return StockComponents(self.symbol, source)
-    
-    def fx(self, symbol: Optional[str]='EURUSD', source: Optional[str] = "MSN"):
-        if symbol:
-            self.symbol = self.msn_symbol_map[symbol]
-        return MSNComponents(self.symbol, source)
-    
-    def crypto(self, symbol: Optional[str]='BTC', source: Optional[str] = "MSN"):
-        if symbol:
-            self.symbol = self.msn_symbol_map[symbol]
-        return MSNComponents(self.symbol, source)
-    
-    def world_index(self, symbol: Optional[str]='DJI', source: Optional[str] = "MSN"):
-        if symbol:
-            self.symbol = self.msn_symbol_map[symbol]
-        return MSNComponents(self.symbol, source)
-
-
 class StockComponents:
     """
     Class (lớp) quản lý các chức năng của thư viện Vnstock liên quan đến cổ phiếu.
     """
     SUPPORTED_SOURCES = ["VCI", "TCBS", "MSN"]
 
     def __init__(self, symbol: str, source: str = "VCI"):
@@ -156,15 +116,15 @@
     
     def price_depth(self, symbol: Optional[str] = None, **kwargs):
         """
         Truy xuất dữ liệu KLGD theo bước giá từ nguồn dữ liệu được chọn.
         """
         self._update_data_source(symbol)
         return self.data_source.price_depth(**kwargs)
-    
+
 class Listing:
     """
     Class (lớp) quản lý các nguồn dữ liệu được tiêu chuẩn hoá cho thông tin niêm yết, dữ liệu trả về tuỳ thuộc vào nguồn dữ liệu sẵn có được chọn.
     """
     
     SUPPORTED_SOURCES = ["VCI", "MSN"]
     def __init__(self, source: str = "VCI"):
@@ -271,14 +231,15 @@
     
     def price_board(self, symbols_list:list, **kwargs):
         """
         Truy xuất dữ liệu giao dịch trong ngày từ nguồn dữ liệu được chọn.
         """
         return self.data_source.price_board(symbols_list, **kwargs)
     
+    
 class Company:
     """
     Class (lớp) quản lý các nguồn dữ liệu được tiêu chuẩn hoá cho thông tin giao dịch.
     """
     def __init__(self, symbol:Optional[str]='ACB', source: str = "TCBS"):
         """
         Initializes the DataExplorer with the specified source and symbol.
@@ -355,14 +316,16 @@
     
     def dividends(self, **kwargs):
         """
         Truy xuất lịch sử chia cổ tức của công ty.
         """
         return self.data_source.dividends(**kwargs)
 
+
+
 class Finance:
     """
     Lớp quản lý các nguồn dữ liệu được tiêu chuẩn hoá cho thông tin tài chính doanh nghiệp.
     """
     SUPPORTED_SOURCES = ["TCBS", "VCI"]
 
     def __init__(self, symbol: str, period: Optional[str] = 'quarter', source: Optional[str] = 'TCBS', get_all: Optional[bool] = True):
@@ -410,14 +373,16 @@
     
     def ratio(self, **kwargs):
         """
         Truy xuất các chỉ số tài chính.
         """
         return self.data_source.ratio(**kwargs)
 
+
+
 class MSNComponents:
     """
     Class (lớp) quản lý các chức năng của thư viện Vnstock liên quan đến thị trường ngoại hối.
     """
     def __init__(self, symbol: Optional[str]='EURUSD', source: str = "MSN"):
         self.symbol = symbol.upper()
         self.source = source.upper()
```

### Comparing `vnstock3-0.3.0.2/vnstock3/core/config/const.py` & `vnstock3-0.3.0.3/vnstock3/core/config/const.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.2/vnstock3/core/utils/env.py` & `vnstock3-0.3.0.3/vnstock3/core/utils/env.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.2/vnstock3/core/utils/ext.py` & `vnstock3-0.3.0.3/vnstock3/core/utils/ext.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.2/vnstock3/core/utils/help.py` & `vnstock3-0.3.0.3/vnstock3/core/utils/help.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.2/vnstock3/core/utils/launcher.py` & `vnstock3-0.3.0.3/vnstock3/core/utils/launcher.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.2/vnstock3/core/utils/logger.py` & `vnstock3-0.3.0.3/vnstock3/core/utils/logger.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.2/vnstock3/core/utils/parser.py` & `vnstock3-0.3.0.3/vnstock3/core/utils/parser.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.2/vnstock3/core/utils/user_agent.py` & `vnstock3-0.3.0.3/vnstock3/core/utils/user_agent.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.2/vnstock3/explorer/misc/exchange_rate.py` & `vnstock3-0.3.0.3/vnstock3/explorer/misc/exchange_rate.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.2/vnstock3/explorer/misc/gold_price.py` & `vnstock3-0.3.0.3/vnstock3/explorer/misc/gold_price.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.2/vnstock3/explorer/msn/const.py` & `vnstock3-0.3.0.3/vnstock3/explorer/msn/const.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.2/vnstock3/explorer/msn/helper.py` & `vnstock3-0.3.0.3/vnstock3/explorer/msn/helper.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,28 +2,35 @@
 from datetime import datetime, timedelta
 from vnstock3.core.utils.user_agent import get_headers
 from vnstock3.explorer.msn.const import _CURRENCY_ID_MAP, _CRYPTO_ID_MAP, _GLOBAL_INDICES
 from vnstock3.core.utils.logger import get_logger
 
 logger = get_logger(__name__)
 
-def msn_apikey (headers, random_agent=False, show_log=False):
+def msn_apikey (headers, version='20240430', show_log=False):
     """
     Lấy apikey của MSN để sử dụng cho các truy vấn dữ liệu
+
+    Tham số:
+        - headers (bắt buộc): Header của request.
+        - version (tùy chọn): Phiên bản của apikey, thường là giá trị ngày tháng của hôm đó, ví dụ 20240527. Mặc định là None. Trong một số trường hợp ngoại lệ, số version hoạt động không theo quy tắc gây lỗi mới cần phải chỉ định mã version.
+        - show_log (tùy chọn): Hiển thị thông tin log giúp debug dễ dàng. Mặc định là False.
     """
     scope = """{"audienceMode":"adult",
                         "browser":{"browserType":"chrome","version":"0","ismobile":"false"},
                         "deviceFormFactor":"desktop","domain":"www.msn.com",
                         "locale":{"content":{"language":"vi","market":"vn"},"display":{"language":"vi","market":"vn"}},
                         "ocid":"hpmsn","os":"macos","platform":"web",
                         "pageType":"financestockdetails"}
                         """
-    today = (datetime.now()-timedelta(hours=7)).strftime("%Y%m%d")
+    if version is None:
+        today = (datetime.now()-timedelta(hours=7)).strftime("%Y%m%d")
+        version = today
     
-    url = f"https://assets.msn.com/resolver/api/resolve/v3/config/?expType=AppConfig&expInstance=default&apptype=finance&v={today}.130&targetScope={scope}"
+    url = f"https://assets.msn.com/resolver/api/resolve/v3/config/?expType=AppConfig&expInstance=default&apptype=finance&v={version}.130&targetScope={scope}"
     if show_log:
         logger.info(f"Requesting apikey from {url}")
     response = requests.request("GET", url, headers=headers)
     data = response.json()
     if show_log:
         logger.info(f"Response: {data}")
     apikey = data['configs']["shared/msn-ns/HoroscopeAnswerCardWC/default"]["properties"]["horoscopeAnswerServiceClientSettings"]["apikey"]
```

### Comparing `vnstock3-0.3.0.2/vnstock3/explorer/msn/listing.py` & `vnstock3-0.3.0.3/vnstock3/explorer/msn/listing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """Listing module."""
 
 from typing import Dict, Optional
 from datetime import datetime
 import pandas as pd
 import requests
 import json
-from vnstock3.core.utils.parser import camel_to_snake
+# from vnstock3.core.utils.parser import camel_to_snake
 from vnstock3.core.utils.logger import get_logger
 from vnstock3.core.utils.user_agent import get_headers
 from vnstock3.explorer.msn.helper import msn_apikey
 from vnstock3.explorer.msn.const import _SYMBOL_INDEX_COLS_MAP
 
 logger = get_logger(__name__)
 
 class Listing:
     """
     Cấu hình truy cập dữ liệu lịch sử giá chứng khoán từ VCI.
     """
-    def __init__(self, random_agent=False):
+    def __init__(self, api_version='20240530', random_agent=False):
         self.data_source = 'MSN'
         self.headers = get_headers(data_source=self.data_source, random_agent=random_agent)
-        self.apikey = msn_apikey(self.headers)
+        self.apikey = msn_apikey(self.headers, version=api_version)
     
     def search_symbol_id (self, query:str, locale:Optional[str]=None, limit:Optional[int]=10, show_log:Optional[bool]=False, to_df: bool =True) -> Dict:
         """
         Truy xuất danh sách toàn. bộ mã và tên các cổ phiếu trên thị trường Việt Nam.
 
         Tham số:
             - query (bắt buộc): Từ khóa tìm kiếm mã cổ phiếu.
```

### Comparing `vnstock3-0.3.0.2/vnstock3/explorer/msn/quote.py` & `vnstock3-0.3.0.3/vnstock3/explorer/msn/quote.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,21 +15,21 @@
 
 logger = get_logger(__name__)
 
 class Quote:
     """
     MSN data source for fetching stock market data, accommodating requests with large date ranges.
     """
-    def __init__(self, symbol_id:str, random_agent:Optional[bool]=False):
+    def __init__(self, symbol_id:str, api_version='20240430', random_agent:Optional[bool]=False):
         self.data_source = 'MSN'
         self.symbol_id = symbol_id.lower()
         self.asset_type = get_asset_type(symbol_id)
         self.base_url = _BASE_URL
         self.headers = get_headers(data_source=self.data_source, random_agent=random_agent)
-        self.apikey = msn_apikey(self.headers)
+        self.apikey = msn_apikey(headers=self.headers, version=api_version)
 
     def _input_validation(self, start: str, end: str, interval: str):
         """
         Validate input data
         """
         # Validate input data
         ticker = TickerModel(symbol=self.symbol_id, start=start, end=end, interval=interval)
@@ -38,15 +38,15 @@
 
     # def history_data(self, start: str, end: Optional[str], interval: Optional[str] = "1D") -> Dict:
     def history(self, start: str, end: Optional[str], interval: Optional[str] = "1D", to_df: bool =True, show_log: bool =False, count_back: Optional[int]=365, asset_type: Optional[str] = None) -> Dict:
         """
         Tham số:
             - start (bắt buộc): thời gian bắt đầu lấy dữ liệu, có thể là ngày dạng string kiểu "YYYY-MM-DD" hoặc "YYYY-MM-DD HH:MM:SS".
             - end (tùy chọn): thời gian kết thúc lấy dữ liệu. Mặc định là None, chương trình tự động lấy thời điểm hiện tại. Có thể nhập ngày dạng string kiểu "YYYY-MM-DD" hoặc "YYYY-MM-DD HH:MM:SS". 
-            - interval (tùy chọn): Khung thời gian trích xuất dữ liệu giá lịch sử. Giá trị nhận: 1m, 5m, 15m, 30m, 1H, 1D, 1W, 1M. Mặc định là "1D".
+            - interval (tùy chọn): Khung thời gian trích xuất dữ liệu giá lịch sử. Giá trị duy nhất được hỗ trợ là "1D".
             - to_df (tùy chọn): Chuyển đổi dữ liệu lịch sử trả về dưới dạng DataFrame. Mặc định là True. Đặt là False để trả về dữ liệu dạng JSON.
             - show_log (tùy chọn): Hiển thị thông tin log giúp debug dễ dàng. Mặc định là False.
             - count_back (tùy chọn): Số lượng dữ liệu trả về từ thời điểm cuối. Mặc định là 365.
         """
 
         # Validate inputs
         ticker = self._input_validation(start, end, interval)
```

### Comparing `vnstock3-0.3.0.2/vnstock3/explorer/tcbs/company.py` & `vnstock3-0.3.0.3/vnstock3/explorer/tcbs/company.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.2/vnstock3/explorer/tcbs/const.py` & `vnstock3-0.3.0.3/vnstock3/explorer/tcbs/const.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.2/vnstock3/explorer/tcbs/financial.py` & `vnstock3-0.3.0.3/vnstock3/explorer/tcbs/financial.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.2/vnstock3/explorer/tcbs/models.py` & `vnstock3-0.3.0.3/vnstock3/explorer/tcbs/models.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.2/vnstock3/explorer/tcbs/quote.py` & `vnstock3-0.3.0.3/vnstock3/explorer/tcbs/quote.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.2/vnstock3/explorer/tcbs/trading.py` & `vnstock3-0.3.0.3/vnstock3/explorer/tcbs/trading.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.2/vnstock3/explorer/vci/company.py` & `vnstock3-0.3.0.3/vnstock3/explorer/vci/company.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.2/vnstock3/explorer/vci/const.py` & `vnstock3-0.3.0.3/vnstock3/explorer/vci/const.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.2/vnstock3/explorer/vci/financial.py` & `vnstock3-0.3.0.3/vnstock3/explorer/vci/financial.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.2/vnstock3/explorer/vci/listing.py` & `vnstock3-0.3.0.3/vnstock3/explorer/vci/listing.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.2/vnstock3/explorer/vci/quote.py` & `vnstock3-0.3.0.3/vnstock3/explorer/vci/quote.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.2/vnstock3/explorer/vci/trading.py` & `vnstock3-0.3.0.3/vnstock3/explorer/vci/trading.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.2/vnstock3.egg-info/PKG-INFO` & `vnstock3-0.3.0.3/vnstock3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnstock3
-Version: 0.3.0.2
+Version: 0.3.0.3
 Summary: A comprehensive and transparent solution for Vietnamese stock market analysis.
 Home-page: https://github.com/thinh-vu/vnstock
 Author: Thinh Vu
 Author-email: Thinh Vu <mrthinh@live.com>
 License: **GIẤY PHÉP SỬ DỤNG PHẦN MỀM VNSTOCK3**
         -----------------------------------
```

### Comparing `vnstock3-0.3.0.2/vnstock3.egg-info/SOURCES.txt` & `vnstock3-0.3.0.3/vnstock3.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -27,16 +27,19 @@
 vnstock3/__init__.py
 vnstock3.egg-info/PKG-INFO
 vnstock3.egg-info/SOURCES.txt
 vnstock3.egg-info/dependency_links.txt
 vnstock3.egg-info/requires.txt
 vnstock3.egg-info/top_level.txt
 vnstock3/common/__init__.py
+vnstock3/common/vnstock.py
 vnstock3/common/data/__init__.py
 vnstock3/common/data/data_explorer.py
+vnstock3/common/plot/__init__.py
+vnstock3/common/plot/chart_wrapper.py
 vnstock3/core/__init__.py
 vnstock3/core/config/__init__.py
 vnstock3/core/config/auth.py
 vnstock3/core/config/const.py
 vnstock3/core/converter/__init__.py
 vnstock3/core/converter/export.py
 vnstock3/core/utils/__init__.py
```

