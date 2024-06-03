# Comparing `tmp/market_generic-0.2.0.tar.gz` & `tmp/market_generic-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "market_generic-0.2.0.tar", last modified: Sun Jun  2 06:17:43 2024, max compression
+gzip compressed data, was "market_generic-0.2.1.tar", last modified: Sun Jun  2 18:02:28 2024, max compression
```

## Comparing `market_generic-0.2.0.tar` & `market_generic-0.2.1.tar`

### file list

```diff
@@ -1,51 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:17:43.030336 market_generic-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-06-02 06:17:43.030336 market_generic-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-06-02 06:17:28.000000 market_generic-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:17:43.030336 market_generic-0.2.0/market_generic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-06-02 06:17:42.000000 market_generic-0.2.0/market_generic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-06-02 06:17:42.000000 market_generic-0.2.0/market_generic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 06:17:42.000000 market_generic-0.2.0/market_generic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-06-02 06:17:42.000000 market_generic-0.2.0/market_generic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-02 06:17:42.000000 market_generic-0.2.0/market_generic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-06-02 06:17:28.000000 market_generic-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 06:17:43.030336 market_generic-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-06-02 06:17:28.000000 market_generic-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:17:43.026336 market_generic-0.2.0/trade/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:17:43.026336 market_generic-0.2.0/trade/calendar/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/calendar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11288 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/calendar/calendar_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/calendar/calendar_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:17:43.026336 market_generic-0.2.0/trade/exchange/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/exchange/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/exchange/api_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/exchange/market.py
--rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/exchange/yf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:17:43.030336 market_generic-0.2.0/trade/nse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/nse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/nse/data_generics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:17:43.030336 market_generic-0.2.0/trade/nse/indices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/nse/indices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/nse/indices/nse_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/nse/indices/nse_indices_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7810 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/nse/nse_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/nse/nse_fno.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:17:43.030336 market_generic-0.2.0/trade/nse/stocks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/nse/stocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/nse/stocks/nse_all_stocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/nse/stocks/nse_stock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:17:43.030336 market_generic-0.2.0/trade/option_chain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/option_chain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10672 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/option_chain/generic_option_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/option_chain/index_option_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/option_chain/stock_option_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:17:43.030336 market_generic-0.2.0/trade/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/utils/df_market_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/utils/gsheet_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/utils/html_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/utils/log_configurator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/utils/network_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/utils/op_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/utils/telegram_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/utils/utility_enabler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:02:28.864233 market_generic-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-06-02 18:02:28.864233 market_generic-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-06-02 18:02:16.000000 market_generic-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:02:28.864233 market_generic-0.2.1/market_generic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-06-02 18:02:28.000000 market_generic-0.2.1/market_generic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-06-02 18:02:28.000000 market_generic-0.2.1/market_generic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 18:02:28.000000 market_generic-0.2.1/market_generic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-06-02 18:02:28.000000 market_generic-0.2.1/market_generic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-02 18:02:28.000000 market_generic-0.2.1/market_generic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-06-02 18:02:16.000000 market_generic-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 18:02:28.864233 market_generic-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-06-02 18:02:16.000000 market_generic-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:02:28.856233 market_generic-0.2.1/trade/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 18:02:16.000000 market_generic-0.2.1/trade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:02:28.856233 market_generic-0.2.1/trade/calendar/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-06-02 18:02:16.000000 market_generic-0.2.1/trade/calendar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11288 2024-06-02 18:02:16.000000 market_generic-0.2.1/trade/calendar/calendar_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-06-02 18:02:16.000000 market_generic-0.2.1/trade/calendar/calendar_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:02:28.856233 market_generic-0.2.1/trade/exchange/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-06-02 18:02:16.000000 market_generic-0.2.1/trade/exchange/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-06-02 18:02:16.000000 market_generic-0.2.1/trade/exchange/api_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-06-02 18:02:16.000000 market_generic-0.2.1/trade/exchange/market.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-06-02 18:02:16.000000 market_generic-0.2.1/trade/exchange/yf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:02:28.860233 market_generic-0.2.1/trade/nse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 18:02:16.000000 market_generic-0.2.1/trade/nse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-06-02 18:02:16.000000 market_generic-0.2.1/trade/nse/data_generics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:02:28.860233 market_generic-0.2.1/trade/nse/indices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 18:02:16.000000 market_generic-0.2.1/trade/nse/indices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-06-02 18:02:16.000000 market_generic-0.2.1/trade/nse/indices/nse_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-06-02 18:02:16.000000 market_generic-0.2.1/trade/nse/indices/nse_indices_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7810 2024-06-02 18:02:16.000000 market_generic-0.2.1/trade/nse/nse_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-06-02 18:02:16.000000 market_generic-0.2.1/trade/nse/nse_fno.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:02:28.860233 market_generic-0.2.1/trade/nse/stocks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 18:02:16.000000 market_generic-0.2.1/trade/nse/stocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-06-02 18:02:16.000000 market_generic-0.2.1/trade/nse/stocks/nse_all_stocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-06-02 18:02:16.000000 market_generic-0.2.1/trade/nse/stocks/nse_stock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:02:28.860233 market_generic-0.2.1/trade/technicals/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-06-02 18:02:16.000000 market_generic-0.2.1/trade/technicals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:02:28.860233 market_generic-0.2.1/trade/technicals/indicators/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-06-02 18:02:16.000000 market_generic-0.2.1/trade/technicals/indicators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-06-02 18:02:16.000000 market_generic-0.2.1/trade/technicals/indicators/generic_indicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-06-02 18:02:16.000000 market_generic-0.2.1/trade/technicals/indicators/moving_averges.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:02:28.860233 market_generic-0.2.1/trade/technicals/indicators/pivot_points/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-06-02 18:02:16.000000 market_generic-0.2.1/trade/technicals/indicators/pivot_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-06-02 18:02:16.000000 market_generic-0.2.1/trade/technicals/indicators/pivot_points/pivot_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-06-02 18:02:16.000000 market_generic-0.2.1/trade/technicals/indicators/pivot_points/standard_pivot_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 18:02:16.000000 market_generic-0.2.1/trade/technicals/indicators/rsi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:02:28.860233 market_generic-0.2.1/trade/technicals/option_chain/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-06-02 18:02:16.000000 market_generic-0.2.1/trade/technicals/option_chain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10672 2024-06-02 18:02:16.000000 market_generic-0.2.1/trade/technicals/option_chain/generic_option_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-06-02 18:02:16.000000 market_generic-0.2.1/trade/technicals/option_chain/index_option_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-06-02 18:02:16.000000 market_generic-0.2.1/trade/technicals/option_chain/stock_option_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:02:28.860233 market_generic-0.2.1/trade/technicals/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 18:02:16.000000 market_generic-0.2.1/trade/technicals/strategies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:02:28.864233 market_generic-0.2.1/trade/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-06-02 18:02:16.000000 market_generic-0.2.1/trade/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-06-02 18:02:16.000000 market_generic-0.2.1/trade/utils/df_market_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-06-02 18:02:16.000000 market_generic-0.2.1/trade/utils/gsheet_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-06-02 18:02:16.000000 market_generic-0.2.1/trade/utils/html_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-06-02 18:02:16.000000 market_generic-0.2.1/trade/utils/log_configurator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-06-02 18:02:16.000000 market_generic-0.2.1/trade/utils/network_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-06-02 18:02:16.000000 market_generic-0.2.1/trade/utils/op_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-06-02 18:02:16.000000 market_generic-0.2.1/trade/utils/telegram_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-06-02 18:02:16.000000 market_generic-0.2.1/trade/utils/utility_enabler.py
```

### Comparing `market_generic-0.2.0/PKG-INFO` & `market_generic-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: market-generic
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Generic Python Package for Stock Market Analysis and Trading
 Home-page: https://github.com/sharmasourab93/market-generic
 Author: Sourab S Sharma
 Author-email: sharmasourab93@gmail.com
 Keywords: Market,Trade,Analysis
 Description-Content-Type: text/markdown
 Requires-Dist: black==24.4.2
@@ -16,14 +16,15 @@
 Requires-Dist: python-telegram-bot==21.1.1
 Requires-Dist: yfinance==0.2.38
 Requires-Dist: requests~=2.31.0
 Requires-Dist: pytz~=2024.1
 Requires-Dist: setuptools~=69.5.1
 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: openpyxl==3.1.2
+Requires-Dist: pandas-ta==0.3.14b0
 
 # market-generic - A Generic Python Package for Stock Market Analysis and Trading
 
 ### Overview
 
 `market-generic` is a powerful and flexible Python library designed to simplify the process of working with stock market data. It provides a comprehensive set of tools and utilities to handle, analyze, and visualize stock data, enabling developers and analysts to build dynamic stock scanners, trading strategies, and other financial applications with ease.
```

### Comparing `market_generic-0.2.0/README.md` & `market_generic-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `market_generic-0.2.0/market_generic.egg-info/PKG-INFO` & `market_generic-0.2.1/market_generic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: market-generic
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Generic Python Package for Stock Market Analysis and Trading
 Home-page: https://github.com/sharmasourab93/market-generic
 Author: Sourab S Sharma
 Author-email: sharmasourab93@gmail.com
 Keywords: Market,Trade,Analysis
 Description-Content-Type: text/markdown
 Requires-Dist: black==24.4.2
@@ -16,14 +16,15 @@
 Requires-Dist: python-telegram-bot==21.1.1
 Requires-Dist: yfinance==0.2.38
 Requires-Dist: requests~=2.31.0
 Requires-Dist: pytz~=2024.1
 Requires-Dist: setuptools~=69.5.1
 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: openpyxl==3.1.2
+Requires-Dist: pandas-ta==0.3.14b0
 
 # market-generic - A Generic Python Package for Stock Market Analysis and Trading
 
 ### Overview
 
 `market-generic` is a powerful and flexible Python library designed to simplify the process of working with stock market data. It provides a comprehensive set of tools and utilities to handle, analyze, and visualize stock data, enabling developers and analysts to build dynamic stock scanners, trading strategies, and other financial applications with ease.
```

### Comparing `market_generic-0.2.0/setup.py` & `market_generic-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages, setup
 
 NAME = "market-generic"
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 DESCRITPION = "A Generic Python Package for Stock Market Analysis and Trading"
 URL = "https://github.com/sharmasourab93/market-generic"
 AUTHOR = "Sourab S Sharma"
 EMAIL = "sharmasourab93@gmail.com"
 
 with open("README.md", "r") as f:
     LONG_DESCRIPTION = f.read()
```

### Comparing `market_generic-0.2.0/trade/calendar/calendar_data.py` & `market_generic-0.2.1/trade/calendar/calendar_data.py`

 * *Files identical despite different names*

### Comparing `market_generic-0.2.0/trade/calendar/calendar_tool.py` & `market_generic-0.2.1/trade/calendar/calendar_tool.py`

 * *Files identical despite different names*

### Comparing `market_generic-0.2.0/trade/exchange/api_config.py` & `market_generic-0.2.1/trade/exchange/api_config.py`

 * *Files identical despite different names*

### Comparing `market_generic-0.2.0/trade/exchange/market.py` & `market_generic-0.2.1/trade/exchange/market.py`

 * *Files identical despite different names*

### Comparing `market_generic-0.2.0/trade/exchange/yf.py` & `market_generic-0.2.1/trade/exchange/yf.py`

 * *Files identical despite different names*

### Comparing `market_generic-0.2.0/trade/nse/indices/nse_index.py` & `market_generic-0.2.1/trade/nse/indices/nse_index.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,35 +22,40 @@
         self._config = NSEIndexConfig(self.dated)
         quotes = self._config.get_quote_index(self.symbol)
 
         for key, value in quotes.items():
             if key not in ("symbol", "dated"):
                 setattr(self, key, value)
 
+        self.indicators = self.apply_indicators()
+
     def get_ohlc(self) -> OHLC_TYPE:
 
         return {self.symbol: self.ohlc}
 
 
 @dataclass
 class SpotIndices:
 
     dated: str
 
     def __post_init__(self):
 
         self._config = NSEIndexConfig(self.dated)
-        self.symbols = [NSEIndex(i, self.dated) for i in INDICES]
+        self.symbols = {i: NSEIndex(i, self.dated) for i in INDICES}
         self.vix = self._config.get_vix()
         self.metrics = self._config.get_index_metrics()
 
+    def __getitem__(self, item: str) -> NSEIndex | None:
+        return self.symbols.get(item, None)
+
     def get_ohlc(self) -> OHLC_TYPE:
 
         resulting_dict = dict()
-        for sym in self.symbols:
+        for sym in self.symbols.values():
             resulting_dict.update(sym.get_ohlc())
 
         return resulting_dict
 
 
 if __name__ == "__main__":
     obj = SpotIndices("31-May-2024")
```

### Comparing `market_generic-0.2.0/trade/nse/indices/nse_indices_config.py` & `market_generic-0.2.1/trade/nse/indices/nse_indices_config.py`

 * *Files identical despite different names*

### Comparing `market_generic-0.2.0/trade/nse/nse_config.py` & `market_generic-0.2.1/trade/nse/nse_config.py`

 * *Files identical despite different names*

### Comparing `market_generic-0.2.0/trade/nse/nse_fno.py` & `market_generic-0.2.1/trade/nse/nse_fno.py`

 * *Files identical despite different names*

### Comparing `market_generic-0.2.0/trade/nse/stocks/nse_all_stocks.py` & `market_generic-0.2.1/trade/nse/stocks/nse_all_stocks.py`

 * *Files identical despite different names*

### Comparing `market_generic-0.2.0/trade/nse/stocks/nse_stock.py` & `market_generic-0.2.1/trade/nse/stocks/nse_stock.py`

 * *Files identical despite different names*

### Comparing `market_generic-0.2.0/trade/option_chain/generic_option_chain.py` & `market_generic-0.2.1/trade/technicals/option_chain/generic_option_chain.py`

 * *Files identical despite different names*

### Comparing `market_generic-0.2.0/trade/option_chain/index_option_chain.py` & `market_generic-0.2.1/trade/technicals/option_chain/index_option_chain.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from trade.nse.indices.nse_indices_config import INDICES, NSEIndexConfig
-from trade.option_chain.generic_option_chain import GenericOptionChain
+from trade.technicals.option_chain.generic_option_chain import GenericOptionChain
 
 WEEKLY_EXPIRY = (3, 2, 1, 9999, 0)
 INDICES_WEEKLY_EXPIRY = {index: expiry for index, expiry in zip(INDICES, WEEKLY_EXPIRY)}
 INDICES_FREQUENCY = {
     i: ("Weekly" if INDICES != "NIFTY NEXT 50" else "Monthly", INDICES_WEEKLY_EXPIRY[i])
     for i in INDICES
 }
```

### Comparing `market_generic-0.2.0/trade/option_chain/stock_option_chain.py` & `market_generic-0.2.1/trade/technicals/option_chain/stock_option_chain.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from trade.nse.nse_config import NSEConfig
-from trade.option_chain.generic_option_chain import GenericOptionChain
+from trade.technicals.option_chain.generic_option_chain import GenericOptionChain
 
 
-class StockOptionChain(GenericOptionChain):
+class StockOptionChainAnalysis(GenericOptionChain):
     def __init__(
         self,
         symbol: str,
         oc_data: dict,
         dated: str,
         strike_multiples: dict,
         Config: type = NSEConfig,
```

### Comparing `market_generic-0.2.0/trade/utils/gsheet_util.py` & `market_generic-0.2.1/trade/utils/gsheet_util.py`

 * *Files identical despite different names*

### Comparing `market_generic-0.2.0/trade/utils/html_parsing.py` & `market_generic-0.2.1/trade/utils/html_parsing.py`

 * *Files identical despite different names*

### Comparing `market_generic-0.2.0/trade/utils/log_configurator.py` & `market_generic-0.2.1/trade/utils/log_configurator.py`

 * *Files identical despite different names*

### Comparing `market_generic-0.2.0/trade/utils/network_tools.py` & `market_generic-0.2.1/trade/utils/network_tools.py`

 * *Files identical despite different names*

### Comparing `market_generic-0.2.0/trade/utils/op_utils.py` & `market_generic-0.2.1/trade/utils/op_utils.py`

 * *Files identical despite different names*

### Comparing `market_generic-0.2.0/trade/utils/telegram_api.py` & `market_generic-0.2.1/trade/utils/telegram_api.py`

 * *Files identical despite different names*

### Comparing `market_generic-0.2.0/trade/utils/utility_enabler.py` & `market_generic-0.2.1/trade/utils/utility_enabler.py`

 * *Files identical despite different names*

