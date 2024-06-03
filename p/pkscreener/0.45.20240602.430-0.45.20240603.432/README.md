# Comparing `tmp/pkscreener-0.45.20240602.430.tar.gz` & `tmp/pkscreener-0.45.20240603.432.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.45.20240602.430.tar", last modified: Sun Jun  2 23:45:09 2024, max compression
+gzip compressed data, was "pkscreener-0.45.20240603.432.tar", last modified: Mon Jun  3 10:21:28 2024, max compression
```

## Comparing `pkscreener-0.45.20240602.430.tar` & `pkscreener-0.45.20240603.432.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 23:45:09.933004 pkscreener-0.45.20240602.430/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/LICENSE-Others
--rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-06-02 23:45:09.933004 pkscreener-0.45.20240602.430/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    26594 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 23:45:09.929004 pkscreener-0.45.20240602.430/pkscreener/
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 23:45:09.933004 pkscreener-0.45.20240602.430/pkscreener/classes/
--rw-r--r--   0 runner    (1001) docker     (127)    13194 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/ArtTexts.py
--rw-r--r--   0 runner    (1001) docker     (127)     9908 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/Backtest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/Barometer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16986 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/CandlePatterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/Changelog.py
--rw-r--r--   0 runner    (1001) docker     (127)    36121 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/ConfigManager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10122 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/Fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    14227 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/MarketMonitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/MarketStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)    47566 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/MenuOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12039 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/OtaUpdater.py
--rw-r--r--   0 runner    (1001) docker     (127)    24198 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-r--r--   0 runner    (1001) docker     (127)    22357 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/PKScanRunner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/PKScheduledTaskProgress.py
--rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/PKScheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/PKSpreadsheets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/PKTask.py
--rw-r--r--   0 runner    (1001) docker     (127)    19048 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/Pktalib.py
--rw-r--r--   0 runner    (1001) docker     (127)    13876 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/Portfolio.py
--rw-r--r--   0 runner    (1001) docker     (127)    47779 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/PortfolioXRay.py
--rw-r--r--   0 runner    (1001) docker     (127)   165167 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/ScreeningStatistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    56535 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/StockScreener.py
--rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/UserMenuChoicesHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    85786 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/Utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/WorkflowManager.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-06-02 23:45:03.000000 pkscreener-0.45.20240602.430/pkscreener/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/keys.py
--rw-r--r--   0 runner    (1001) docker     (127)   791436 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/courbd.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   153034 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/pkscreener.ini
--rw-r--r--   0 runner    (1001) docker     (127)    61567 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/pkscreenerbot.py
--rw-r--r--   0 runner    (1001) docker     (127)    37014 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/pkscreenercli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 23:45:09.929004 pkscreener-0.45.20240602.430/pkscreener.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-06-02 23:45:09.000000 pkscreener-0.45.20240602.430/pkscreener.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-06-02 23:45:09.000000 pkscreener-0.45.20240602.430/pkscreener.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 23:45:09.000000 pkscreener-0.45.20240602.430/pkscreener.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-06-02 23:45:09.000000 pkscreener-0.45.20240602.430/pkscreener.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 23:45:09.000000 pkscreener-0.45.20240602.430/pkscreener.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-06-02 23:45:09.000000 pkscreener-0.45.20240602.430/pkscreener.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-02 23:45:09.000000 pkscreener-0.45.20240602.430/pkscreener.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-06-02 23:45:09.933004 pkscreener-0.45.20240602.430/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5567 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:21:28.357165 pkscreener-0.45.20240603.432/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-06-03 10:19:24.000000 pkscreener-0.45.20240603.432/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-06-03 10:19:24.000000 pkscreener-0.45.20240603.432/LICENSE-Others
+-rw-r--r--   0 runner    (1001) docker     (127)    27466 2024-06-03 10:21:28.357165 pkscreener-0.45.20240603.432/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    26549 2024-06-03 10:19:24.000000 pkscreener-0.45.20240603.432/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:21:28.353165 pkscreener-0.45.20240603.432/pkscreener/
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-06-03 10:19:24.000000 pkscreener-0.45.20240603.432/pkscreener/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:21:28.357165 pkscreener-0.45.20240603.432/pkscreener/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)    13194 2024-06-03 10:19:24.000000 pkscreener-0.45.20240603.432/pkscreener/classes/ArtTexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9908 2024-06-03 10:19:24.000000 pkscreener-0.45.20240603.432/pkscreener/classes/Backtest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-06-03 10:19:24.000000 pkscreener-0.45.20240603.432/pkscreener/classes/Barometer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16986 2024-06-03 10:19:24.000000 pkscreener-0.45.20240603.432/pkscreener/classes/CandlePatterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-06-03 10:19:24.000000 pkscreener-0.45.20240603.432/pkscreener/classes/Changelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36121 2024-06-03 10:19:24.000000 pkscreener-0.45.20240603.432/pkscreener/classes/ConfigManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10122 2024-06-03 10:19:24.000000 pkscreener-0.45.20240603.432/pkscreener/classes/Fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14227 2024-06-03 10:19:24.000000 pkscreener-0.45.20240603.432/pkscreener/classes/MarketMonitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-06-03 10:19:24.000000 pkscreener-0.45.20240603.432/pkscreener/classes/MarketStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48000 2024-06-03 10:19:24.000000 pkscreener-0.45.20240603.432/pkscreener/classes/MenuOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12039 2024-06-03 10:19:24.000000 pkscreener-0.45.20240603.432/pkscreener/classes/OtaUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24198 2024-06-03 10:19:24.000000 pkscreener-0.45.20240603.432/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22357 2024-06-03 10:19:24.000000 pkscreener-0.45.20240603.432/pkscreener/classes/PKScanRunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-06-03 10:19:24.000000 pkscreener-0.45.20240603.432/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-06-03 10:19:24.000000 pkscreener-0.45.20240603.432/pkscreener/classes/PKScheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-06-03 10:19:24.000000 pkscreener-0.45.20240603.432/pkscreener/classes/PKSpreadsheets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-06-03 10:19:24.000000 pkscreener-0.45.20240603.432/pkscreener/classes/PKTask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19048 2024-06-03 10:19:24.000000 pkscreener-0.45.20240603.432/pkscreener/classes/Pktalib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13876 2024-06-03 10:19:24.000000 pkscreener-0.45.20240603.432/pkscreener/classes/Portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47779 2024-06-03 10:19:24.000000 pkscreener-0.45.20240603.432/pkscreener/classes/PortfolioXRay.py
+-rw-r--r--   0 runner    (1001) docker     (127)   165260 2024-06-03 10:19:24.000000 pkscreener-0.45.20240603.432/pkscreener/classes/ScreeningStatistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56535 2024-06-03 10:19:24.000000 pkscreener-0.45.20240603.432/pkscreener/classes/StockScreener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-06-03 10:19:24.000000 pkscreener-0.45.20240603.432/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85786 2024-06-03 10:19:24.000000 pkscreener-0.45.20240603.432/pkscreener/classes/Utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-06-03 10:19:24.000000 pkscreener-0.45.20240603.432/pkscreener/classes/WorkflowManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-06-03 10:21:21.000000 pkscreener-0.45.20240603.432/pkscreener/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-06-03 10:19:24.000000 pkscreener-0.45.20240603.432/pkscreener/classes/keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)   791436 2024-06-03 10:19:24.000000 pkscreener-0.45.20240603.432/pkscreener/courbd.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   153115 2024-06-03 10:19:24.000000 pkscreener-0.45.20240603.432/pkscreener/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-06-03 10:19:25.000000 pkscreener-0.45.20240603.432/pkscreener/pkscreener.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    61567 2024-06-03 10:19:25.000000 pkscreener-0.45.20240603.432/pkscreener/pkscreenerbot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37014 2024-06-03 10:19:25.000000 pkscreener-0.45.20240603.432/pkscreener/pkscreenercli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:21:28.353165 pkscreener-0.45.20240603.432/pkscreener.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27466 2024-06-03 10:21:28.000000 pkscreener-0.45.20240603.432/pkscreener.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-06-03 10:21:28.000000 pkscreener-0.45.20240603.432/pkscreener.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 10:21:28.000000 pkscreener-0.45.20240603.432/pkscreener.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-06-03 10:21:28.000000 pkscreener-0.45.20240603.432/pkscreener.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 10:21:28.000000 pkscreener-0.45.20240603.432/pkscreener.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-06-03 10:21:28.000000 pkscreener-0.45.20240603.432/pkscreener.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-03 10:21:28.000000 pkscreener-0.45.20240603.432/pkscreener.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-06-03 10:21:28.357165 pkscreener-0.45.20240603.432/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5567 2024-06-03 10:19:25.000000 pkscreener-0.45.20240603.432/setup.py
```

### Comparing `pkscreener-0.45.20240602.430/LICENSE` & `pkscreener-0.45.20240603.432/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.430/LICENSE-Others` & `pkscreener-0.45.20240603.432/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.430/PKG-INFO` & `pkscreener-0.45.20240603.432/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.45.20240602.430
+Version: 0.45.20240603.432
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240602.430.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240603.432.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,24 +269,24 @@
 * Please feel free to Suggest improvements bugs by creating an issue.
 * Please follow the [Guidelines for Contributing](https://github.com/pkjmesra/PKScreener/blob/main/CONTRIBUTING.md) while making a Pull Request.
 
 ## Disclaimer:
 * DO NOT use the results provided by the software 'solely' to make your trading decisions.
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
-* This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
+* This screener began as a [fork] but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.429/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.430/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.429/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.430/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.429/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.430/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240602.430/README.md` & `pkscreener-0.45.20240603.432/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,24 +247,24 @@
 * Please feel free to Suggest improvements bugs by creating an issue.
 * Please follow the [Guidelines for Contributing](https://github.com/pkjmesra/PKScreener/blob/main/CONTRIBUTING.md) while making a Pull Request.
 
 ## Disclaimer:
 * DO NOT use the results provided by the software 'solely' to make your trading decisions.
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
-* This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
+* This screener began as a [fork] but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.429/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.430/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.429/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.430/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.429/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.430/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240602.430/pkscreener/__init__.py` & `pkscreener-0.45.20240603.432/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.430/pkscreener/classes/ArtTexts.py` & `pkscreener-0.45.20240603.432/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.430/pkscreener/classes/Backtest.py` & `pkscreener-0.45.20240603.432/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.430/pkscreener/classes/Barometer.py` & `pkscreener-0.45.20240603.432/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.430/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.45.20240603.432/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.430/pkscreener/classes/Changelog.py` & `pkscreener-0.45.20240603.432/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.430/pkscreener/classes/ConfigManager.py` & `pkscreener-0.45.20240603.432/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.430/pkscreener/classes/Fetcher.py` & `pkscreener-0.45.20240603.432/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.430/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.45.20240603.432/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.430/pkscreener/classes/MarketStatus.py` & `pkscreener-0.45.20240603.432/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.430/pkscreener/classes/MenuOptions.py` & `pkscreener-0.45.20240603.432/pkscreener/classes/MenuOptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,54 +57,60 @@
 }
 level1_P_MenuDict = {
     "1": "Predefined Piped Scanners",
     "2": "Define my custom Piped Scanner",
     "3": "Run Piped Scans Saved So Far",
     "M": "Back to the Top/Main menu",
 }
-PREDEFINED_SCAN_MENU_KEYS = ["1","2","3","4","5","6","7","8","9","10","11","12","13","14","15","16"]
+PREDEFINED_SCAN_MENU_KEYS = ["1","2","3","4","5","6","7","8","9","10","11","12","13","14","15","16","17","18","19"]
 PREDEFINED_SCAN_MENU_TEXTS = [
     "Volume Scanners | High Momentum | Breaking Out Now | ATR Cross     ",
     "Volume Scanners | High Momentum | ATR Cross",
     "Volume Scanners | High Momentum                                    ",
     "Volume Scanners | ATR Cross",
     "Volume Scanners | High Bid/Ask Build Up                            ",
+    "Volume Scanners | ATR Cross | ATR Trailing Stops",
+    "Volume Scanners | ATR Trailing Stops                               ",
     "High Momentum | ATR Cross",
     "High Momentum | ATR Trailing Stop                                  ",
     "ATR Cross | ATR Trailing Stop",
     "TTM Sqeeze Buy | Intraday RSI b/w 0 to 54                          ",
     "Volume Scanners | High Momentum | Breaking Out Now | ATR Cross | Intraday RSI b/w 0 to 54",
     "Volume Scanners | ATR Cross | Intraday RSI b/w 0 to 54             ",
     "VCP (Mark Minervini) | Chart Patterns | MA Support",
     "VCP | Chart Patterns | MA Support                                  ",
     "Already Breaking out | VCP (Minervini) | Chart Patterns | MA Support",
     "ATR Trailing Stops | VCP (Minervini)                               ",
     "VCP | ATR Trailing Stops",
+    "Nifty 50,Nifty Bank | VCP | ATR Trailing Stops                     ",
 ]
 level2_P_MenuDict = {}
 for key in PREDEFINED_SCAN_MENU_KEYS:
     level2_P_MenuDict[key] = PREDEFINED_SCAN_MENU_TEXTS[int(key)-1]
 level2_P_MenuDict["M"] = "Back to the Top/Main menu"
 PREDEFINED_SCAN_MENU_VALUES =[
     "--systemlaunched -a y -e -o 'X:12:9:2.5:>|X:0:31:>|X:0:23:>|X:0:27:'",
     "--systemlaunched -a y -e -o 'X:12:9:2.5:>|X:0:31:>|X:0:27:'",
     "--systemlaunched -a y -e -o 'X:12:9:2.5:>|X:0:31:'",
     "--systemlaunched -a y -e -o 'X:12:9:2.5:>|X:0:27:'",
     "--systemlaunched -a y -e -o 'X:12:9:2.5:>|X:0:29:'",
+    "--systemlaunched -a y -e -o 'X:12:9:2.5:>|X:0:27:>|X:12:30:1:'",
+    "--systemlaunched -a y -e -o 'X:12:9:2.5:>|X:12:30:1:'",
     "--systemlaunched -a y -e -o 'X:12:31:>|X:0:27:'",
     "--systemlaunched -a y -e -o 'X:12:31:>|X:0:30:1:'",
     "--systemlaunched -a y -e -o 'X:12:27:>|X:0:30:1:'",
     "--systemlaunched -a y -e -o 'X:12:7:6:1:>|X:0:5:0:54:i 1m'",
     "--systemlaunched -a y -e -o 'X:12:9:2.5:>|X:0:31:>|X:0:23:>|X:0:27:>|X:0:5:0:54:i 1m'",
     "--systemlaunched -a y -e -o 'X:12:9:2.5:>|X:0:27:>|X:0:5:0:54:i 1m'",
     "--systemlaunched -a y -e -o 'X:12:7:8:>|X:12:7:9:1:1:'",
     "--systemlaunched -a y -e -o 'X:12:7:4:>|X:12:7:9:1:1:'",
     "--systemlaunched -a y -e -o 'X:12:2:>|X:12:7:8:>|X:12:7:9:1:1:'",
     "--systemlaunched -a y -e -o 'X:12:30:1:>|X:12:7:8:'",
     "--systemlaunched -a y -e -o 'X:12:7:4:>|X:12:30:1:'",
+    "--systemlaunched -a y -e -o 'X:0:0:^NSEI,^NSEBANK:>|X:12:7:4:>|X:12:30:1:'",
 ]
 PIPED_SCANNERS = {}
 for key in PREDEFINED_SCAN_MENU_KEYS:
     PIPED_SCANNERS[key] = PREDEFINED_SCAN_MENU_VALUES[int(key)-1]
 
 level1_T_MenuDict = {
     "L": "Long Term",
```

### Comparing `pkscreener-0.45.20240602.430/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.45.20240603.432/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.430/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.45.20240603.432/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.430/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.45.20240603.432/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.430/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.45.20240603.432/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.430/pkscreener/classes/PKScheduler.py` & `pkscreener-0.45.20240603.432/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.430/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.45.20240603.432/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.430/pkscreener/classes/PKTask.py` & `pkscreener-0.45.20240603.432/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.430/pkscreener/classes/Pktalib.py` & `pkscreener-0.45.20240603.432/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.430/pkscreener/classes/Portfolio.py` & `pkscreener-0.45.20240603.432/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.430/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.45.20240603.432/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.430/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.45.20240603.432/pkscreener/classes/ScreeningStatistics.py`

 * *Files 0% similar despite different names*

```diff
@@ -6679,3645 +6679,3651 @@
 0001a160: 616c 3a0a 2020 2020 2020 2020 2020 2020  al:.            
 0001a170: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
 0001a180: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
 0001a190: 6469 7469 6f6e 203d 206c 6173 745f 7369  dition = last_si
 0001a1a0: 676e 616c 5b64 6174 615f 6c69 7374 5b63  gnal[data_list[c
 0001a1b0: 6e74 5d5d 5b30 5d5b 2253 4c22 5d5b 305d  nt]][0]["SL"][0]
 0001a1c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a1d0: 2065 7863 6570 7420 4b65 7945 7272 6f72   except KeyError
-0001a1e0: 2061 7320 653a 2023 2070 7261 676d 613a   as e: # pragma:
-0001a1f0: 206e 6f20 636f 7665 720a 2020 2020 2020   no cover.      
-0001a200: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0001a210: 6c66 2e64 6566 6175 6c74 5f6c 6f67 6765  lf.default_logge
-0001a220: 722e 6465 6275 6728 652c 2065 7863 5f69  r.debug(e, exc_i
-0001a230: 6e66 6f3d 5472 7565 290a 2020 2020 2020  nfo=True).      
-0001a240: 2020 2020 2020 2020 2020 2020 2020 636f                co
-0001a250: 6e64 6974 696f 6e20 3d20 6c61 7374 5f73  ndition = last_s
-0001a260: 6967 6e61 6c5b 6461 7461 5f6c 6973 745b  ignal[data_list[
-0001a270: 636e 745d 5d5b 2253 4c22 5d5b 305d 0a20  cnt]]["SL"][0]. 
-0001a280: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0001a290: 2069 6620 6c61 7374 5f73 6967 6e61 6c5b   if last_signal[
-0001a2a0: 6461 7461 5f6c 6973 745b 636e 745d 5d20  data_list[cnt]] 
-0001a2b0: 6973 206e 6f74 2066 696e 616c 3a20 2020  is not final:   
-0001a2c0: 2020 2020 2020 2023 2044 6562 7567 202d         # Debug -
-0001a2d0: 2053 686f 7773 2061 6c6c 2063 6f6e 6469   Shows all condi
-0001a2e0: 7469 6f6e 730a 2020 2020 2020 2020 2020  tions.          
-0001a2f0: 2020 2020 2020 6966 206c 656e 2866 696e        if len(fin
-0001a300: 616c 5b22 534c 225d 2920 3e20 3020 616e  al["SL"]) > 0 an
-0001a310: 6420 636f 6e64 6974 696f 6e20 213d 2066  d condition != f
-0001a320: 696e 616c 5b22 534c 225d 2e69 6c6f 635b  inal["SL"].iloc[
-0001a330: 305d 3a0a 2020 2020 2020 2020 2020 2020  0]:.            
-0001a340: 2020 2020 2020 2020 2320 446f 2073 6f6d          # Do som
-0001a350: 6574 6869 6e67 2077 6974 6820 7265 7375  ething with resu
-0001a360: 6c74 730a 2020 2020 2020 2020 2020 2020  lts.            
-0001a370: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-0001a380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a390: 2020 2020 2072 6573 756c 745f 6466 203d       result_df =
-0001a3a0: 2070 642e 636f 6e63 6174 280a 2020 2020   pd.concat(.    
-0001a3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a3c0: 2020 2020 2020 2020 5b0a 2020 2020 2020          [.      
-0001a3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a3e0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0001a3f0: 5f64 662c 0a20 2020 2020 2020 2020 2020  _df,.           
-0001a400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a410: 2020 2020 2070 642e 4461 7461 4672 616d       pd.DataFram
-0001a420: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
+0001a1d0: 2065 7863 6570 7420 284b 6579 4572 726f   except (KeyErro
+0001a1e0: 722c 496e 6465 7845 7272 6f72 2920 6173  r,IndexError) as
+0001a1f0: 2065 3a20 2320 7072 6167 6d61 3a20 6e6f   e: # pragma: no
+0001a200: 2063 6f76 6572 0a20 2020 2020 2020 2020   cover.         
+0001a210: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
+0001a220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a230: 2020 2020 2020 2020 636f 6e64 6974 696f          conditio
+0001a240: 6e20 3d20 6c61 7374 5f73 6967 6e61 6c5b  n = last_signal[
+0001a250: 6461 7461 5f6c 6973 745b 636e 745d 5d5b  data_list[cnt]][
+0001a260: 2253 4c22 5d5b 305d 0a20 2020 2020 2020  "SL"][0].       
+0001a270: 2020 2020 2020 2020 2020 2020 2065 7863               exc
+0001a280: 6570 7420 284b 6579 4572 726f 722c 496e  ept (KeyError,In
+0001a290: 6465 7845 7272 6f72 2920 6173 2065 3a20  dexError) as e: 
+0001a2a0: 2320 7072 6167 6d61 3a20 6e6f 2063 6f76  # pragma: no cov
+0001a2b0: 6572 0a20 2020 2020 2020 2020 2020 2020  er.             
+0001a2c0: 2020 2020 2020 2020 2020 2063 6f6e 6469             condi
+0001a2d0: 7469 6f6e 203d 204e 6f6e 650a 2020 2020  tion = None.    
+0001a2e0: 2020 2020 2020 2020 2020 2020 2320 6966              # if
+0001a2f0: 206c 6173 745f 7369 676e 616c 5b64 6174   last_signal[dat
+0001a300: 615f 6c69 7374 5b63 6e74 5d5d 2069 7320  a_list[cnt]] is 
+0001a310: 6e6f 7420 6669 6e61 6c3a 2020 2020 2020  not final:      
+0001a320: 2020 2020 2320 4465 6275 6720 2d20 5368      # Debug - Sh
+0001a330: 6f77 7320 616c 6c20 636f 6e64 6974 696f  ows all conditio
+0001a340: 6e73 0a20 2020 2020 2020 2020 2020 2020  ns.             
+0001a350: 2020 2069 6620 6c65 6e28 6669 6e61 6c5b     if len(final[
+0001a360: 2253 4c22 5d29 203e 2030 2061 6e64 2063  "SL"]) > 0 and c
+0001a370: 6f6e 6469 7469 6f6e 2021 3d20 6669 6e61  ondition != fina
+0001a380: 6c5b 2253 4c22 5d2e 696c 6f63 5b30 5d3a  l["SL"].iloc[0]:
+0001a390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a3a0: 2020 2020 2023 2044 6f20 736f 6d65 7468       # Do someth
+0001a3b0: 696e 6720 7769 7468 2072 6573 756c 7473  ing with results
+0001a3c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a3d0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+0001a3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a3f0: 2020 7265 7375 6c74 5f64 6620 3d20 7064    result_df = pd
+0001a400: 2e63 6f6e 6361 7428 0a20 2020 2020 2020  .concat(.       
+0001a410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a420: 2020 2020 205b 0a20 2020 2020 2020 2020       [.         
 0001a430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a440: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
-0001a450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a440: 2020 2020 2020 2072 6573 756c 745f 6466         result_df
+0001a450: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
 0001a460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a470: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+0001a470: 2020 7064 2e44 6174 6146 7261 6d65 280a    pd.DataFrame(.
 0001a480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a490: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0001a4a0: 6f6c 6f72 5465 7874 2e42 4c55 450a 2020  olorText.BLUE.  
+0001a490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a4a0: 2020 2020 5b0a 2020 2020 2020 2020 2020      [.          
 0001a4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a4d0: 2020 2020 2020 2020 2020 2b20 7374 7228            + str(
-0001a4e0: 6669 6e61 6c2e 696e 6465 785b 305d 290a  final.index[0]).
-0001a4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a510: 2020 2020 2020 2020 2020 2020 2b20 636f              + co
-0001a520: 6c6f 7254 6578 742e 454e 442c 0a20 2020  lorText.END,.   
-0001a530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a550: 2020 2020 2020 2020 2063 6f6c 6f72 5465           colorTe
-0001a560: 7874 2e42 4f4c 440a 2020 2020 2020 2020  xt.BOLD.        
-0001a570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a590: 2020 2020 2b20 636f 6c6f 7254 6578 742e      + colorText.
-0001a5a0: 5741 524e 0a20 2020 2020 2020 2020 2020  WARN.           
-0001a5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a5d0: 202b 2064 6174 615f 6c69 7374 5b63 6e74   + data_list[cnt
-0001a5e0: 5d2e 7370 6c69 7428 225f 2229 5b30 5d2e  ].split("_")[0].
-0001a5f0: 7570 7065 7228 290a 2020 2020 2020 2020  upper().        
-0001a600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a4c0: 2020 2020 2020 2020 2020 2020 2020 5b0a                [.
+0001a4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a4f0: 2020 2020 2020 2020 2020 2020 636f 6c6f              colo
+0001a500: 7254 6578 742e 424c 5545 0a20 2020 2020  rText.BLUE.     
+0001a510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a530: 2020 2020 2020 202b 2073 7472 2866 696e         + str(fin
+0001a540: 616c 2e69 6e64 6578 5b30 5d29 0a20 2020  al.index[0]).   
+0001a550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a570: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
+0001a580: 5465 7874 2e45 4e44 2c0a 2020 2020 2020  Text.END,.      
+0001a590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a5b0: 2020 2020 2020 636f 6c6f 7254 6578 742e        colorText.
+0001a5c0: 424f 4c44 0a20 2020 2020 2020 2020 2020  BOLD.           
+0001a5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a5f0: 202b 2063 6f6c 6f72 5465 7874 2e57 4152   + colorText.WAR
+0001a600: 4e0a 2020 2020 2020 2020 2020 2020 2020  N.              
 0001a610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a620: 2020 2020 2b20 636f 6c6f 7254 6578 742e      + colorText.
-0001a630: 454e 442c 0a20 2020 2020 2020 2020 2020  END,.           
-0001a640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a660: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+0001a620: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+0001a630: 6461 7461 5f6c 6973 745b 636e 745d 2e73  data_list[cnt].s
+0001a640: 706c 6974 2822 5f22 295b 305d 2e75 7070  plit("_")[0].upp
+0001a650: 6572 2829 0a20 2020 2020 2020 2020 2020  er().           
+0001a660: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001a670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a690: 2020 2063 6f6c 6f72 5465 7874 2e42 4f4c     colorText.BOL
-0001a6a0: 440a 2020 2020 2020 2020 2020 2020 2020  D.              
-0001a6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a680: 202b 2063 6f6c 6f72 5465 7874 2e45 4e44   + colorText.END
+0001a690: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001a6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a6b0: 2020 2020 2020 2020 2020 2020 2020 280a                (.
 0001a6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a6d0: 2020 2b20 636f 6c6f 7254 6578 742e 4641    + colorText.FA
-0001a6e0: 494c 0a20 2020 2020 2020 2020 2020 2020  IL.             
-0001a6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a6f0: 636f 6c6f 7254 6578 742e 424f 4c44 0a20  colorText.BOLD. 
 0001a700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a710: 2020 202b 2064 6174 615f 6c69 7374 5b63     + data_list[c
-0001a720: 6e74 5d2e 7370 6c69 7428 225f 2229 5b31  nt].split("_")[1
-0001a730: 5d2e 7570 7065 7228 290a 2020 2020 2020  ].upper().      
+0001a710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a720: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+0001a730: 2063 6f6c 6f72 5465 7874 2e46 4149 4c0a   colorText.FAIL.
 0001a740: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001a750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a760: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
-0001a770: 7254 6578 742e 454e 440a 2020 2020 2020  rText.END.      
-0001a780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a7a0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0001a760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a770: 2b20 6461 7461 5f6c 6973 745b 636e 745d  + data_list[cnt]
+0001a780: 2e73 706c 6974 2822 5f22 295b 315d 2e75  .split("_")[1].u
+0001a790: 7070 6572 2829 0a20 2020 2020 2020 2020  pper().         
+0001a7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001a7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a7d0: 2020 2020 6966 2022 7365 6c6c 2220 696e      if "sell" in
-0001a7e0: 2064 6174 615f 6c69 7374 5b63 6e74 5d0a   data_list[cnt].
+0001a7c0: 2020 2020 2020 202b 2063 6f6c 6f72 5465         + colorTe
+0001a7d0: 7874 2e45 4e44 0a20 2020 2020 2020 2020  xt.END.         
+0001a7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001a7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a810: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0001a820: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
-0001a830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a850: 2020 2063 6f6c 6f72 5465 7874 2e42 4f4c     colorText.BOL
-0001a860: 440a 2020 2020 2020 2020 2020 2020 2020  D.              
-0001a870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a800: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+0001a810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a830: 2069 6620 2273 656c 6c22 2069 6e20 6461   if "sell" in da
+0001a840: 7461 5f6c 6973 745b 636e 745d 0a20 2020  ta_list[cnt].   
+0001a850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a870: 2020 2020 2020 2020 2065 6c73 6520 280a           else (.
 0001a880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a890: 2020 2b20 636f 6c6f 7254 6578 742e 4752    + colorText.GR
-0001a8a0: 4545 4e0a 2020 2020 2020 2020 2020 2020  EEN.            
-0001a8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a8b0: 636f 6c6f 7254 6578 742e 424f 4c44 0a20  colorText.BOLD. 
 0001a8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a8d0: 2020 2020 2b20 6461 7461 5f6c 6973 745b      + data_list[
-0001a8e0: 636e 745d 2e73 706c 6974 2822 5f22 295b  cnt].split("_")[
-0001a8f0: 315d 2e75 7070 6572 2829 0a20 2020 2020  1].upper().     
-0001a900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a8e0: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+0001a8f0: 2063 6f6c 6f72 5465 7874 2e47 5245 454e   colorText.GREEN
+0001a900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0001a910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a920: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
-0001a930: 6f72 5465 7874 2e45 4e44 0a20 2020 2020  orText.END.     
-0001a940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a960: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
+0001a920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a930: 202b 2064 6174 615f 6c69 7374 5b63 6e74   + data_list[cnt
+0001a940: 5d2e 7370 6c69 7428 225f 2229 5b31 5d2e  ].split("_")[1].
+0001a950: 7570 7065 7228 290a 2020 2020 2020 2020  upper().        
+0001a960: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001a970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a990: 2020 2020 2020 636f 6c6f 7254 6578 742e        colorText.
-0001a9a0: 4641 494c 0a20 2020 2020 2020 2020 2020  FAIL.           
+0001a980: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
+0001a990: 6578 742e 454e 440a 2020 2020 2020 2020  ext.END.        
+0001a9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001a9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a9d0: 202b 2073 7472 2866 696e 616c 2e53 4c5b   + str(final.SL[
-0001a9e0: 305d 290a 2020 2020 2020 2020 2020 2020  0]).            
-0001a9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aa00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aa10: 2b20 636f 6c6f 7254 6578 742e 454e 442c  + colorText.END,
-0001aa20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001aa30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aa40: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
-0001aa50: 6f72 5465 7874 2e47 5245 454e 0a20 2020  orText.GREEN.   
-0001aa60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aa70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aa80: 2020 2020 2020 2020 202b 2073 7472 2866           + str(f
-0001aa90: 696e 616c 2e54 6172 6765 745b 305d 290a  inal.Target[0]).
-0001aaa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aac0: 2020 2020 2020 2020 2020 2020 2b20 636f              + co
-0001aad0: 6c6f 7254 6578 742e 454e 442c 0a20 2020  lorText.END,.   
-0001aae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aaf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ab00: 2020 2020 2020 2020 2066 2231 3a7b 7269           f"1:{ri
-0001ab10: 736b 5f72 6577 6172 647d 222c 0a20 2020  sk_reward}",.   
-0001ab20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ab30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ab40: 2020 2020 205d 0a20 2020 2020 2020 2020       ].         
+0001a9c0: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
+0001a9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a9f0: 2020 2063 6f6c 6f72 5465 7874 2e46 4149     colorText.FAI
+0001aa00: 4c0a 2020 2020 2020 2020 2020 2020 2020  L.              
+0001aa10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aa20: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+0001aa30: 7374 7228 6669 6e61 6c2e 534c 5b30 5d29  str(final.SL[0])
+0001aa40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001aa50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aa60: 2020 2020 2020 2020 2020 2020 202b 2063               + c
+0001aa70: 6f6c 6f72 5465 7874 2e45 4e44 2c0a 2020  olorText.END,.  
+0001aa80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aa90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aaa0: 2020 2020 2020 2020 2020 636f 6c6f 7254            colorT
+0001aab0: 6578 742e 4752 4545 4e0a 2020 2020 2020  ext.GREEN.      
+0001aac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aae0: 2020 2020 2020 2b20 7374 7228 6669 6e61        + str(fina
+0001aaf0: 6c2e 5461 7267 6574 5b30 5d29 0a20 2020  l.Target[0]).   
+0001ab00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ab10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ab20: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
+0001ab30: 5465 7874 2e45 4e44 2c0a 2020 2020 2020  Text.END,.      
+0001ab40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001ab50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ab60: 2020 2020 2020 2020 2020 205d 2c0a 2020             ],.  
-0001ab70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ab60: 2020 2020 2020 6622 313a 7b72 6973 6b5f        f"1:{risk_
+0001ab70: 7265 7761 7264 7d22 2c0a 2020 2020 2020  reward}",.      
 0001ab80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ab90: 2020 636f 6c75 6d6e 733d 7265 7375 6c74    columns=result
-0001aba0: 5f64 662e 636f 6c75 6d6e 732c 0a20 2020  _df.columns,.   
+0001ab90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aba0: 2020 5d0a 2020 2020 2020 2020 2020 2020    ].            
 0001abb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001abc0: 2020 2020 2020 2020 2020 2020 2029 2c0a               ),.
+0001abc0: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
 0001abd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001abe0: 2020 2020 2020 2020 2020 2020 5d2c 0a20              ],. 
-0001abf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ac00: 2020 2020 2020 2020 2020 2061 7869 733d             axis=
-0001ac10: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
-0001ac20: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0001abe0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0001abf0: 6f6c 756d 6e73 3d72 6573 756c 745f 6466  olumns=result_df
+0001ac00: 2e63 6f6c 756d 6e73 2c0a 2020 2020 2020  .columns,.      
+0001ac10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ac20: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
 0001ac30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ac40: 2020 2020 2072 6573 756c 745f 6466 2e72       result_df.r
-0001ac50: 6573 6574 5f69 6e64 6578 2864 726f 703d  eset_index(drop=
-0001ac60: 5472 7565 2c20 696e 706c 6163 653d 5472  True, inplace=Tr
-0001ac70: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
-0001ac80: 2020 2020 2020 2020 6578 6365 7074 2045          except E
-0001ac90: 7863 6570 7469 6f6e 2061 7320 653a 2020  xception as e:  
-0001aca0: 2320 7072 6167 6d61 3a20 6e6f 2063 6f76  # pragma: no cov
-0001acb0: 6572 0a20 2020 2020 2020 2020 2020 2020  er.             
-0001acc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001acd0: 6465 6661 756c 745f 6c6f 6767 6572 2e64  default_logger.d
-0001ace0: 6562 7567 2865 2c20 6578 635f 696e 666f  ebug(e, exc_info
-0001acf0: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
-0001ad00: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0001ad10: 6173 730a 2020 2020 2020 2020 2020 2020  ass.            
-0001ad20: 2020 2020 2020 2020 2320 5468 656e 2075          # Then u
-0001ad30: 7064 6174 650a 2020 2020 2020 2020 2020  pdate.          
-0001ad40: 2020 2020 2020 2020 2020 6c61 7374 5f73            last_s
-0001ad50: 6967 6e61 6c5b 6461 7461 5f6c 6973 745b  ignal[data_list[
-0001ad60: 636e 745d 5d20 3d20 5b66 696e 616c 5d0a  cnt]] = [final].
-0001ad70: 2020 2020 2020 2020 6966 2072 6573 756c          if resul
-0001ad80: 745f 6466 2069 7320 6e6f 7420 4e6f 6e65  t_df is not None
-0001ad90: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0001ada0: 7375 6c74 5f64 662e 6472 6f70 5f64 7570  sult_df.drop_dup
-0001adb0: 6c69 6361 7465 7328 6b65 6570 3d22 6c61  licates(keep="la
-0001adc0: 7374 222c 2069 6e70 6c61 6365 3d54 7275  st", inplace=Tru
-0001add0: 6529 0a20 2020 2020 2020 2020 2020 2072  e).            r
-0001ade0: 6573 756c 745f 6466 2e73 6f72 745f 7661  esult_df.sort_va
-0001adf0: 6c75 6573 2862 793d 2254 696d 6522 2c20  lues(by="Time", 
-0001ae00: 696e 706c 6163 653d 5472 7565 290a 2020  inplace=True).  
-0001ae10: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-0001ae20: 756c 745f 6466 5b3a 3a2d 315d 0a0a 2020  ult_df[::-1]..  
-0001ae30: 2020 2320 5072 6570 726f 6365 7373 2074    # Preprocess t
-0001ae40: 6865 2061 6371 7569 7265 6420 6461 7461  he acquired data
-0001ae50: 0a20 2020 2064 6566 2070 7265 7072 6f63  .    def preproc
-0001ae60: 6573 7344 6174 6128 7365 6c66 2c20 6466  essData(self, df
-0001ae70: 2c20 6461 7973 546f 4c6f 6f6b 6261 636b  , daysToLookback
-0001ae80: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
-0001ae90: 6173 7365 7274 2069 7369 6e73 7461 6e63  assert isinstanc
-0001aea0: 6528 6466 2c20 7064 2e44 6174 6146 7261  e(df, pd.DataFra
-0001aeb0: 6d65 290a 2020 2020 2020 2020 6461 7461  me).        data
-0001aec0: 203d 2064 662e 636f 7079 2829 0a20 2020   = df.copy().   
-0001aed0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-0001aee0: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
-0001aef0: 612e 7265 706c 6163 6528 6e70 2e69 6e66  a.replace(np.inf
-0001af00: 2c20 6e70 2e6e 616e 292e 7265 706c 6163  , np.nan).replac
-0001af10: 6528 2d6e 702e 696e 662c 206e 702e 6e61  e(-np.inf, np.na
-0001af20: 6e29 2e64 726f 706e 6128 686f 773d 2261  n).dropna(how="a
-0001af30: 6c6c 2229 0a20 2020 2020 2020 2020 2020  ll").           
-0001af40: 2023 2073 656c 662e 6465 6661 756c 745f   # self.default_
-0001af50: 6c6f 6767 6572 2e69 6e66 6f28 6622 5072  logger.info(f"Pr
-0001af60: 6570 726f 6365 7373 696e 6720 6461 7461  eprocessing data
-0001af70: 3a5c 6e7b 6461 7461 2e68 6561 6428 3129  :\n{data.head(1)
-0001af80: 7d5c 6e22 290a 2020 2020 2020 2020 2020  }\n").          
-0001af90: 2020 6966 2064 6179 7354 6f4c 6f6f 6b62    if daysToLookb
-0001afa0: 6163 6b20 6973 204e 6f6e 653a 0a20 2020  ack is None:.   
-0001afb0: 2020 2020 2020 2020 2020 2020 2064 6179               day
-0001afc0: 7354 6f4c 6f6f 6b62 6163 6b20 3d20 7365  sToLookback = se
-0001afd0: 6c66 2e63 6f6e 6669 674d 616e 6167 6572  lf.configManager
-0001afe0: 2e64 6179 7354 6f4c 6f6f 6b62 6163 6b0a  .daysToLookback.
-0001aff0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0001b000: 656c 662e 636f 6e66 6967 4d61 6e61 6765  elf.configManage
-0001b010: 722e 7573 6545 4d41 3a0a 2020 2020 2020  r.useEMA:.      
-0001b020: 2020 2020 2020 2020 2020 736d 6120 3d20            sma = 
-0001b030: 706b 7461 6c69 622e 454d 4128 6461 7461  pktalib.EMA(data
-0001b040: 5b22 436c 6f73 6522 5d2c 2074 696d 6570  ["Close"], timep
-0001b050: 6572 696f 643d 3530 290a 2020 2020 2020  eriod=50).      
-0001b060: 2020 2020 2020 2020 2020 6c6d 6120 3d20            lma = 
-0001b070: 706b 7461 6c69 622e 454d 4128 6461 7461  pktalib.EMA(data
-0001b080: 5b22 436c 6f73 6522 5d2c 2074 696d 6570  ["Close"], timep
-0001b090: 6572 696f 643d 3230 3029 0a20 2020 2020  eriod=200).     
-0001b0a0: 2020 2020 2020 2020 2020 2073 736d 6120             ssma 
-0001b0b0: 3d20 706b 7461 6c69 622e 454d 4128 6461  = pktalib.EMA(da
-0001b0c0: 7461 5b22 436c 6f73 6522 5d2c 2074 696d  ta["Close"], tim
-0001b0d0: 6570 6572 696f 643d 3929 0a20 2020 2020  eperiod=9).     
-0001b0e0: 2020 2020 2020 2020 2020 2073 736d 6132             ssma2
-0001b0f0: 3020 3d20 706b 7461 6c69 622e 454d 4128  0 = pktalib.EMA(
-0001b100: 6461 7461 5b22 436c 6f73 6522 5d2c 2074  data["Close"], t
-0001b110: 696d 6570 6572 696f 643d 3230 290a 2020  imeperiod=20).  
-0001b120: 2020 2020 2020 2020 2020 2020 2020 6461                da
-0001b130: 7461 2e69 6e73 6572 7428 6c65 6e28 6461  ta.insert(len(da
-0001b140: 7461 2e63 6f6c 756d 6e73 292c 2022 534d  ta.columns), "SM
-0001b150: 4122 2c20 736d 6129 0a20 2020 2020 2020  A", sma).       
-0001b160: 2020 2020 2020 2020 2064 6174 612e 696e           data.in
-0001b170: 7365 7274 286c 656e 2864 6174 612e 636f  sert(len(data.co
-0001b180: 6c75 6d6e 7329 2c20 224c 4d41 222c 206c  lumns), "LMA", l
-0001b190: 6d61 290a 2020 2020 2020 2020 2020 2020  ma).            
-0001b1a0: 2020 2020 6461 7461 2e69 6e73 6572 7428      data.insert(
-0001b1b0: 6c65 6e28 6461 7461 2e63 6f6c 756d 6e73  len(data.columns
-0001b1c0: 292c 2022 5353 4d41 222c 2073 736d 6129  ), "SSMA", ssma)
-0001b1d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b1e0: 2064 6174 612e 696e 7365 7274 286c 656e   data.insert(len
-0001b1f0: 2864 6174 612e 636f 6c75 6d6e 7329 2c20  (data.columns), 
-0001b200: 2253 534d 4132 3022 2c20 7373 6d61 3230  "SSMA20", ssma20
-0001b210: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-0001b220: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0001b230: 2020 2020 736d 6120 3d20 706b 7461 6c69      sma = pktali
-0001b240: 622e 534d 4128 6461 7461 5b22 436c 6f73  b.SMA(data["Clos
-0001b250: 6522 5d2c 2074 696d 6570 6572 696f 643d  e"], timeperiod=
-0001b260: 3530 290a 2020 2020 2020 2020 2020 2020  50).            
-0001b270: 2020 2020 6c6d 6120 3d20 706b 7461 6c69      lma = pktali
-0001b280: 622e 534d 4128 6461 7461 5b22 436c 6f73  b.SMA(data["Clos
-0001b290: 6522 5d2c 2074 696d 6570 6572 696f 643d  e"], timeperiod=
-0001b2a0: 3230 3029 0a20 2020 2020 2020 2020 2020  200).           
-0001b2b0: 2020 2020 2073 736d 6120 3d20 706b 7461       ssma = pkta
-0001b2c0: 6c69 622e 534d 4128 6461 7461 5b22 436c  lib.SMA(data["Cl
-0001b2d0: 6f73 6522 5d2c 2074 696d 6570 6572 696f  ose"], timeperio
-0001b2e0: 643d 3929 0a20 2020 2020 2020 2020 2020  d=9).           
-0001b2f0: 2020 2020 2073 736d 6132 3020 3d20 706b       ssma20 = pk
-0001b300: 7461 6c69 622e 534d 4128 6461 7461 5b22  talib.SMA(data["
-0001b310: 436c 6f73 6522 5d2c 2074 696d 6570 6572  Close"], timeper
-0001b320: 696f 643d 3230 290a 2020 2020 2020 2020  iod=20).        
-0001b330: 2020 2020 2020 2020 6461 7461 2e69 6e73          data.ins
-0001b340: 6572 7428 6c65 6e28 6461 7461 2e63 6f6c  ert(len(data.col
-0001b350: 756d 6e73 292c 2022 534d 4122 2c20 736d  umns), "SMA", sm
-0001b360: 6129 0a20 2020 2020 2020 2020 2020 2020  a).             
-0001b370: 2020 2064 6174 612e 696e 7365 7274 286c     data.insert(l
-0001b380: 656e 2864 6174 612e 636f 6c75 6d6e 7329  en(data.columns)
-0001b390: 2c20 224c 4d41 222c 206c 6d61 290a 2020  , "LMA", lma).  
-0001b3a0: 2020 2020 2020 2020 2020 2020 2020 6461                da
-0001b3b0: 7461 2e69 6e73 6572 7428 6c65 6e28 6461  ta.insert(len(da
-0001b3c0: 7461 2e63 6f6c 756d 6e73 292c 2022 5353  ta.columns), "SS
-0001b3d0: 4d41 222c 2073 736d 6129 0a20 2020 2020  MA", ssma).     
-0001b3e0: 2020 2020 2020 2020 2020 2064 6174 612e             data.
-0001b3f0: 696e 7365 7274 286c 656e 2864 6174 612e  insert(len(data.
-0001b400: 636f 6c75 6d6e 7329 2c20 2253 534d 4132  columns), "SSMA2
-0001b410: 3022 2c20 7373 6d61 3230 290a 2020 2020  0", ssma20).    
-0001b420: 2020 2020 2020 2020 766f 6c20 3d20 706b          vol = pk
-0001b430: 7461 6c69 622e 534d 4128 6461 7461 5b22  talib.SMA(data["
-0001b440: 566f 6c75 6d65 225d 2c20 7469 6d65 7065  Volume"], timepe
-0001b450: 7269 6f64 3d32 3029 0a20 2020 2020 2020  riod=20).       
-0001b460: 2020 2020 2072 7369 203d 2070 6b74 616c       rsi = pktal
-0001b470: 6962 2e52 5349 2864 6174 615b 2243 6c6f  ib.RSI(data["Clo
-0001b480: 7365 225d 2c20 7469 6d65 7065 7269 6f64  se"], timeperiod
-0001b490: 3d31 3429 0a20 2020 2020 2020 2020 2020  =14).           
-0001b4a0: 2064 6174 612e 696e 7365 7274 286c 656e   data.insert(len
-0001b4b0: 2864 6174 612e 636f 6c75 6d6e 7329 2c20  (data.columns), 
-0001b4c0: 2256 6f6c 4d41 222c 2076 6f6c 290a 2020  "VolMA", vol).  
-0001b4d0: 2020 2020 2020 2020 2020 6461 7461 2e69            data.i
-0001b4e0: 6e73 6572 7428 6c65 6e28 6461 7461 2e63  nsert(len(data.c
-0001b4f0: 6f6c 756d 6e73 292c 2022 5253 4922 2c20  olumns), "RSI", 
-0001b500: 7273 6929 0a20 2020 2020 2020 2020 2020  rsi).           
-0001b510: 2063 6369 203d 2070 6b74 616c 6962 2e43   cci = pktalib.C
-0001b520: 4349 2864 6174 615b 2248 6967 6822 5d2c  CI(data["High"],
-0001b530: 2064 6174 615b 224c 6f77 225d 2c20 6461   data["Low"], da
-0001b540: 7461 5b22 436c 6f73 6522 5d2c 2074 696d  ta["Close"], tim
-0001b550: 6570 6572 696f 643d 3134 290a 2020 2020  eperiod=14).    
-0001b560: 2020 2020 2020 2020 6461 7461 2e69 6e73          data.ins
-0001b570: 6572 7428 6c65 6e28 6461 7461 2e63 6f6c  ert(len(data.col
-0001b580: 756d 6e73 292c 2022 4343 4922 2c20 6363  umns), "CCI", cc
-0001b590: 6929 0a20 2020 2020 2020 2020 2020 2074  i).            t
-0001b5a0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-0001b5b0: 2020 2020 6661 7374 6b2c 2066 6173 7464      fastk, fastd
-0001b5c0: 203d 2070 6b74 616c 6962 2e53 544f 4348   = pktalib.STOCH
-0001b5d0: 5253 4928 0a20 2020 2020 2020 2020 2020  RSI(.           
-0001b5e0: 2020 2020 2020 2020 2064 6174 615b 2243           data["C
-0001b5f0: 6c6f 7365 225d 2c20 7469 6d65 7065 7269  lose"], timeperi
-0001b600: 6f64 3d31 342c 2066 6173 746b 5f70 6572  od=14, fastk_per
-0001b610: 696f 643d 352c 2066 6173 7464 5f70 6572  iod=5, fastd_per
-0001b620: 696f 643d 332c 2066 6173 7464 5f6d 6174  iod=3, fastd_mat
-0001b630: 7970 653d 300a 2020 2020 2020 2020 2020  ype=0.          
-0001b640: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0001b650: 2020 2020 2020 2020 6461 7461 2e69 6e73          data.ins
-0001b660: 6572 7428 6c65 6e28 6461 7461 2e63 6f6c  ert(len(data.col
-0001b670: 756d 6e73 292c 2022 4641 5354 4b22 2c20  umns), "FASTK", 
-0001b680: 6661 7374 6b29 0a20 2020 2020 2020 2020  fastk).         
-0001b690: 2020 2020 2020 2064 6174 612e 696e 7365         data.inse
-0001b6a0: 7274 286c 656e 2864 6174 612e 636f 6c75  rt(len(data.colu
-0001b6b0: 6d6e 7329 2c20 2246 4153 5444 222c 2066  mns), "FASTD", f
-0001b6c0: 6173 7464 290a 2020 2020 2020 2020 2020  astd).          
-0001b6d0: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
-0001b6e0: 6f6e 2061 7320 653a 0a20 2020 2020 2020  on as e:.       
-0001b6f0: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
-0001b700: 6661 756c 745f 6c6f 6767 6572 2e64 6562  fault_logger.deb
-0001b710: 7567 2865 2c20 6578 635f 696e 666f 3d54  ug(e, exc_info=T
-0001b720: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
-0001b730: 2020 2020 2070 6173 730a 2020 2020 2020       pass.      
-0001b740: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
-0001b750: 6f6e 2061 7320 653a 0a20 2020 2020 2020  on as e:.       
-0001b760: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
-0001b770: 6661 756c 745f 6c6f 6767 6572 2e64 6562  fault_logger.deb
-0001b780: 7567 2865 2c20 6578 635f 696e 666f 3d54  ug(e, exc_info=T
-0001b790: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
-0001b7a0: 2020 2020 2070 6173 730a 2020 2020 2020       pass.      
-0001b7b0: 2020 6461 7461 203d 2064 6174 615b 3a3a    data = data[::
-0001b7c0: 2d31 5d20 2023 2052 6576 6572 7365 2074  -1]  # Reverse t
-0001b7d0: 6865 2064 6174 6166 7261 6d65 0a20 2020  he dataframe.   
-0001b7e0: 2020 2020 2023 2064 6174 6120 3d20 6461       # data = da
-0001b7f0: 7461 2e66 696c 6c6e 6128 3029 0a20 2020  ta.fillna(0).   
-0001b800: 2020 2020 2023 2064 6174 6120 3d20 6461       # data = da
-0001b810: 7461 2e72 6570 6c61 6365 285b 6e70 2e69  ta.replace([np.i
-0001b820: 6e66 2c20 2d6e 702e 696e 665d 2c20 3029  nf, -np.inf], 0)
-0001b830: 0a20 2020 2020 2020 2066 756c 6c44 6174  .        fullDat
-0001b840: 6120 3d20 6461 7461 0a20 2020 2020 2020  a = data.       
-0001b850: 2074 7269 6d6d 6564 4461 7461 203d 2064   trimmedData = d
-0001b860: 6174 612e 6865 6164 2864 6179 7354 6f4c  ata.head(daysToL
-0001b870: 6f6f 6b62 6163 6b29 0a20 2020 2020 2020  ookback).       
-0001b880: 2072 6574 7572 6e20 2866 756c 6c44 6174   return (fullDat
-0001b890: 612c 2074 7269 6d6d 6564 4461 7461 290a  a, trimmedData).
-0001b8a0: 0a20 2020 2023 2056 616c 6964 6174 6520  .    # Validate 
-0001b8b0: 6966 2074 6865 2073 746f 636b 2069 7320  if the stock is 
-0001b8c0: 6275 6c6c 6973 6820 696e 2074 6865 2073  bullish in the s
-0001b8d0: 686f 7274 2074 6572 6d0a 2020 2020 6465  hort term.    de
-0001b8e0: 6620 7661 6c69 6461 7465 3135 4d69 6e75  f validate15Minu
-0001b8f0: 7465 5072 6963 6556 6f6c 756d 6542 7265  tePriceVolumeBre
-0001b900: 616b 6f75 7428 7365 6c66 2c20 6466 293a  akout(self, df):
-0001b910: 0a20 2020 2020 2020 2069 6620 6466 2069  .        if df i
-0001b920: 7320 4e6f 6e65 206f 7220 6c65 6e28 6466  s None or len(df
-0001b930: 2920 3d3d 2030 3a0a 2020 2020 2020 2020  ) == 0:.        
-0001b940: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-0001b950: 0a20 2020 2020 2020 2023 2068 7474 7073  .        # https
-0001b960: 3a2f 2f63 6861 7274 696e 6b2e 636f 6d2f  ://chartink.com/
-0001b970: 7363 7265 656e 6572 2f31 352d 6d69 6e2d  screener/15-min-
-0001b980: 7072 6963 652d 766f 6c75 6d65 2d62 7265  price-volume-bre
-0001b990: 616b 6f75 740a 2020 2020 2020 2020 6461  akout.        da
-0001b9a0: 7461 203d 2064 662e 636f 7079 2829 0a20  ta = df.copy(). 
-0001b9b0: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
-0001b9c0: 7461 2e66 696c 6c6e 6128 3029 0a20 2020  ta.fillna(0).   
-0001b9d0: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
-0001b9e0: 2e72 6570 6c61 6365 285b 6e70 2e69 6e66  .replace([np.inf
-0001b9f0: 2c20 2d6e 702e 696e 665d 2c20 3029 0a20  , -np.inf], 0). 
-0001ba00: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
-0001ba10: 7461 5b3a 3a2d 315d 2020 2320 5265 7665  ta[::-1]  # Reve
-0001ba20: 7273 6520 7468 6520 6461 7461 6672 616d  rse the datafram
-0001ba30: 6520 736f 2074 6861 7420 6974 7320 7468  e so that its th
-0001ba40: 6520 6f6c 6465 7374 2064 6174 6520 6669  e oldest date fi
-0001ba50: 7273 740a 2020 2020 2020 2020 6461 7461  rst.        data
-0001ba60: 5b22 534d 4132 3022 5d20 3d20 706b 7461  ["SMA20"] = pkta
-0001ba70: 6c69 622e 534d 4128 6461 7461 5b22 436c  lib.SMA(data["Cl
-0001ba80: 6f73 6522 5d2c 2032 3029 0a20 2020 2020  ose"], 20).     
-0001ba90: 2020 2064 6174 615b 2253 4d41 3230 5622     data["SMA20V"
-0001baa0: 5d20 3d20 706b 7461 6c69 622e 534d 4128  ] = pktalib.SMA(
-0001bab0: 6461 7461 5b22 566f 6c75 6d65 225d 2c20  data["Volume"], 
-0001bac0: 3230 290a 2020 2020 2020 2020 6461 7461  20).        data
-0001bad0: 203d 2064 6174 615b 0a20 2020 2020 2020   = data[.       
-0001bae0: 2020 2020 203a 3a2d 310a 2020 2020 2020       ::-1.      
-0001baf0: 2020 5d20 2023 2052 6576 6572 7365 2074    ]  # Reverse t
-0001bb00: 6865 2064 6174 6166 7261 6d65 2073 6f20  he dataframe so 
-0001bb10: 7468 6174 2069 7427 7320 7468 6520 6d6f  that it's the mo
-0001bb20: 7374 2072 6563 656e 7420 6461 7465 2066  st recent date f
-0001bb30: 6972 7374 0a20 2020 2020 2020 2072 6563  irst.        rec
-0001bb40: 656e 7420 3d20 6461 7461 2e68 6561 6428  ent = data.head(
-0001bb50: 3329 0a20 2020 2020 2020 2069 6620 6c65  3).        if le
-0001bb60: 6e28 7265 6365 6e74 2920 3c20 333a 0a20  n(recent) < 3:. 
-0001bb70: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0001bb80: 6e20 4661 6c73 650a 2020 2020 2020 2020  n False.        
-0001bb90: 636f 6e64 3120 3d20 7265 6365 6e74 5b22  cond1 = recent["
-0001bba0: 436c 6f73 6522 5d2e 696c 6f63 5b30 5d20  Close"].iloc[0] 
-0001bbb0: 3e20 7265 6365 6e74 5b22 436c 6f73 6522  > recent["Close"
-0001bbc0: 5d2e 696c 6f63 5b31 5d0a 2020 2020 2020  ].iloc[1].      
-0001bbd0: 2020 636f 6e64 3220 3d20 636f 6e64 3120    cond2 = cond1 
-0001bbe0: 616e 6420 2872 6563 656e 745b 2243 6c6f  and (recent["Clo
-0001bbf0: 7365 225d 2e69 6c6f 635b 305d 203e 2072  se"].iloc[0] > r
-0001bc00: 6563 656e 745b 2253 4d41 3230 225d 2e69  ecent["SMA20"].i
-0001bc10: 6c6f 635b 305d 290a 2020 2020 2020 2020  loc[0]).        
-0001bc20: 636f 6e64 3320 3d20 636f 6e64 3220 616e  cond3 = cond2 an
-0001bc30: 6420 2872 6563 656e 745b 2243 6c6f 7365  d (recent["Close
-0001bc40: 225d 2e69 6c6f 635b 315d 203e 2072 6563  "].iloc[1] > rec
-0001bc50: 656e 745b 2248 6967 6822 5d2e 696c 6f63  ent["High"].iloc
-0001bc60: 5b32 5d29 0a20 2020 2020 2020 2063 6f6e  [2]).        con
-0001bc70: 6434 203d 2063 6f6e 6433 2061 6e64 2028  d4 = cond3 and (
-0001bc80: 7265 6365 6e74 5b22 566f 6c75 6d65 225d  recent["Volume"]
-0001bc90: 2e69 6c6f 635b 305d 203e 2072 6563 656e  .iloc[0] > recen
-0001bca0: 745b 2253 4d41 3230 5622 5d2e 696c 6f63  t["SMA20V"].iloc
-0001bcb0: 5b30 5d29 0a20 2020 2020 2020 2063 6f6e  [0]).        con
-0001bcc0: 6435 203d 2063 6f6e 6434 2061 6e64 2028  d5 = cond4 and (
-0001bcd0: 7265 6365 6e74 5b22 566f 6c75 6d65 225d  recent["Volume"]
-0001bce0: 2e69 6c6f 635b 315d 203e 2072 6563 656e  .iloc[1] > recen
-0001bcf0: 745b 2253 4d41 3230 5622 5d2e 696c 6f63  t["SMA20V"].iloc
-0001bd00: 5b30 5d29 0a20 2020 2020 2020 2072 6574  [0]).        ret
-0001bd10: 7572 6e20 636f 6e64 350a 0a20 2020 2064  urn cond5..    d
-0001bd20: 6566 2076 616c 6964 6174 6542 756c 6c69  ef validateBulli
-0001bd30: 7368 466f 7254 6f6d 6f72 726f 7728 7365  shForTomorrow(se
-0001bd40: 6c66 2c20 6466 293a 0a20 2020 2020 2020  lf, df):.       
-0001bd50: 2069 6620 6466 2069 7320 4e6f 6e65 206f   if df is None o
-0001bd60: 7220 6c65 6e28 6466 2920 3d3d 2030 3a0a  r len(df) == 0:.
-0001bd70: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0001bd80: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
-0001bd90: 2064 6174 6120 3d20 6466 2e63 6f70 7928   data = df.copy(
-0001bda0: 290a 2020 2020 2020 2020 2320 6874 7470  ).        # http
-0001bdb0: 733a 2f2f 6368 6172 7469 6e6b 2e63 6f6d  s://chartink.com
-0001bdc0: 2f73 6372 6565 6e65 722f 6275 6c6c 6973  /screener/bullis
-0001bdd0: 682d 666f 722d 746f 6d6f 7272 6f77 0a20  h-for-tomorrow. 
-0001bde0: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
-0001bdf0: 7461 2e66 696c 6c6e 6128 3029 0a20 2020  ta.fillna(0).   
-0001be00: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
-0001be10: 2e72 6570 6c61 6365 285b 6e70 2e69 6e66  .replace([np.inf
-0001be20: 2c20 2d6e 702e 696e 665d 2c20 3029 0a20  , -np.inf], 0). 
-0001be30: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
-0001be40: 7461 5b3a 3a2d 315d 2020 2320 5265 7665  ta[::-1]  # Reve
-0001be50: 7273 6520 7468 6520 6461 7461 6672 616d  rse the datafram
-0001be60: 6520 736f 2074 6861 7420 6974 7320 7468  e so that its th
-0001be70: 6520 6f6c 6465 7374 2064 6174 6520 6669  e oldest date fi
-0001be80: 7273 740a 2020 2020 2020 2020 6d61 6364  rst.        macd
-0001be90: 4c69 6e65 203d 2070 6b74 616c 6962 2e4d  Line = pktalib.M
-0001bea0: 4143 4428 6461 7461 5b22 436c 6f73 6522  ACD(data["Close"
-0001beb0: 5d2c 2031 322c 2032 362c 2039 295b 305d  ], 12, 26, 9)[0]
-0001bec0: 2e74 6169 6c28 3329 0a20 2020 2020 2020  .tail(3).       
-0001bed0: 206d 6163 6453 6967 6e61 6c20 3d20 706b   macdSignal = pk
-0001bee0: 7461 6c69 622e 4d41 4344 2864 6174 615b  talib.MACD(data[
-0001bef0: 2243 6c6f 7365 225d 2c20 3132 2c20 3236  "Close"], 12, 26
-0001bf00: 2c20 3929 5b31 5d2e 7461 696c 2833 290a  , 9)[1].tail(3).
-0001bf10: 2020 2020 2020 2020 6d61 6364 4869 7374          macdHist
-0001bf20: 203d 2070 6b74 616c 6962 2e4d 4143 4428   = pktalib.MACD(
-0001bf30: 6461 7461 5b22 436c 6f73 6522 5d2c 2031  data["Close"], 1
-0001bf40: 322c 2032 362c 2039 295b 325d 2e74 6169  2, 26, 9)[2].tai
-0001bf50: 6c28 3329 0a0a 2020 2020 2020 2020 7265  l(3)..        re
-0001bf60: 7475 726e 2028 0a20 2020 2020 2020 2020  turn (.         
-0001bf70: 2020 2028 6d61 6364 4869 7374 2e69 6c6f     (macdHist.ilo
-0001bf80: 635b 3a31 5d2e 696c 6f63 5b30 5d20 3c20  c[:1].iloc[0] < 
-0001bf90: 6d61 6364 4869 7374 2e69 6c6f 635b 3a32  macdHist.iloc[:2
-0001bfa0: 5d2e 696c 6f63 5b31 5d29 0a20 2020 2020  ].iloc[1]).     
-0001bfb0: 2020 2020 2020 2061 6e64 2028 6d61 6364         and (macd
-0001bfc0: 4869 7374 2e69 6c6f 635b 3a33 5d2e 696c  Hist.iloc[:3].il
-0001bfd0: 6f63 5b32 5d20 3e20 6d61 6364 4869 7374  oc[2] > macdHist
-0001bfe0: 2e69 6c6f 635b 3a32 5d2e 696c 6f63 5b31  .iloc[:2].iloc[1
-0001bff0: 5d29 0a20 2020 2020 2020 2020 2020 2061  ]).            a
-0001c000: 6e64 2028 0a20 2020 2020 2020 2020 2020  nd (.           
-0001c010: 2020 2020 2028 6d61 6364 4c69 6e65 2e69       (macdLine.i
-0001c020: 6c6f 635b 3a33 5d2e 696c 6f63 5b32 5d20  loc[:3].iloc[2] 
-0001c030: 2d20 6d61 6364 5369 676e 616c 2e69 6c6f  - macdSignal.ilo
-0001c040: 635b 3a33 5d2e 696c 6f63 5b32 5d29 0a20  c[:3].iloc[2]). 
-0001c050: 2020 2020 2020 2020 2020 2020 2020 202d                 -
-0001c060: 2028 6d61 6364 4c69 6e65 2e69 6c6f 635b   (macdLine.iloc[
-0001c070: 3a32 5d2e 696c 6f63 5b31 5d20 2d20 6d61  :2].iloc[1] - ma
-0001c080: 6364 5369 676e 616c 2e69 6c6f 635b 3a32  cdSignal.iloc[:2
-0001c090: 5d2e 696c 6f63 5b31 5d29 0a20 2020 2020  ].iloc[1]).     
-0001c0a0: 2020 2020 2020 2020 2020 203e 3d20 302e             >= 0.
-0001c0b0: 340a 2020 2020 2020 2020 2020 2020 290a  4.            ).
-0001c0c0: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-0001c0d0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0001c0e0: 2020 286d 6163 644c 696e 652e 696c 6f63    (macdLine.iloc
-0001c0f0: 5b3a 325d 2e69 6c6f 635b 315d 202d 206d  [:2].iloc[1] - m
-0001c100: 6163 6453 6967 6e61 6c2e 696c 6f63 5b3a  acdSignal.iloc[:
-0001c110: 325d 2e69 6c6f 635b 315d 290a 2020 2020  2].iloc[1]).    
-0001c120: 2020 2020 2020 2020 2020 2020 2d20 286d              - (m
-0001c130: 6163 644c 696e 652e 696c 6f63 5b3a 315d  acdLine.iloc[:1]
-0001c140: 2e69 6c6f 635b 305d 202d 206d 6163 6453  .iloc[0] - macdS
-0001c150: 6967 6e61 6c2e 696c 6f63 5b3a 315d 2e69  ignal.iloc[:1].i
-0001c160: 6c6f 635b 305d 290a 2020 2020 2020 2020  loc[0]).        
-0001c170: 2020 2020 2020 2020 3c3d 2030 2e32 0a20          <= 0.2. 
-0001c180: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0001c190: 2020 2020 2020 2020 2061 6e64 2028 6d61           and (ma
-0001c1a0: 6364 4c69 6e65 2e69 6c6f 635b 3a33 5d2e  cdLine.iloc[:3].
-0001c1b0: 696c 6f63 5b32 5d20 3e20 6d61 6364 5369  iloc[2] > macdSi
-0001c1c0: 676e 616c 2e69 6c6f 635b 3a33 5d2e 696c  gnal.iloc[:3].il
-0001c1d0: 6f63 5b32 5d29 0a20 2020 2020 2020 2020  oc[2]).         
-0001c1e0: 2020 2061 6e64 2028 0a20 2020 2020 2020     and (.       
-0001c1f0: 2020 2020 2020 2020 2028 6d61 6364 4c69           (macdLi
-0001c200: 6e65 2e69 6c6f 635b 3a33 5d2e 696c 6f63  ne.iloc[:3].iloc
-0001c210: 5b32 5d20 2d20 6d61 6364 5369 676e 616c  [2] - macdSignal
-0001c220: 2e69 6c6f 635b 3a33 5d2e 696c 6f63 5b32  .iloc[:3].iloc[2
-0001c230: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-0001c240: 2020 202d 2028 6d61 6364 4c69 6e65 2e69     - (macdLine.i
-0001c250: 6c6f 635b 3a32 5d2e 696c 6f63 5b31 5d20  loc[:2].iloc[1] 
-0001c260: 2d20 6d61 6364 5369 676e 616c 2e69 6c6f  - macdSignal.ilo
-0001c270: 635b 3a32 5d2e 696c 6f63 5b31 5d29 0a20  c[:2].iloc[1]). 
-0001c280: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0001c290: 2031 0a20 2020 2020 2020 2020 2020 2029   1.            )
-0001c2a0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-0001c2b0: 2340 6d65 6173 7572 655f 7469 6d65 0a20  #@measure_time. 
-0001c2c0: 2020 2023 2076 616c 6964 6174 6520 6966     # validate if
-0001c2d0: 2043 4349 2069 7320 7769 7468 696e 2067   CCI is within g
-0001c2e0: 6976 656e 2072 616e 6765 0a20 2020 2064  iven range.    d
-0001c2f0: 6566 2076 616c 6964 6174 6543 4349 2873  ef validateCCI(s
-0001c300: 656c 662c 2064 662c 2073 6372 6565 6e44  elf, df, screenD
-0001c310: 6963 742c 2073 6176 6544 6963 742c 206d  ict, saveDict, m
-0001c320: 696e 4343 492c 206d 6178 4343 4929 3a0a  inCCI, maxCCI):.
-0001c330: 2020 2020 2020 2020 6966 2064 6620 6973          if df is
-0001c340: 204e 6f6e 6520 6f72 206c 656e 2864 6629   None or len(df)
-0001c350: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
-0001c360: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-0001c370: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
-0001c380: 662e 636f 7079 2829 0a20 2020 2020 2020  f.copy().       
-0001c390: 2064 6174 6120 3d20 6461 7461 2e66 696c   data = data.fil
-0001c3a0: 6c6e 6128 3029 0a20 2020 2020 2020 2064  lna(0).        d
-0001c3b0: 6174 6120 3d20 6461 7461 2e72 6570 6c61  ata = data.repla
-0001c3c0: 6365 285b 6e70 2e69 6e66 2c20 2d6e 702e  ce([np.inf, -np.
-0001c3d0: 696e 665d 2c20 3029 0a20 2020 2020 2020  inf], 0).       
-0001c3e0: 2063 6369 203d 2069 6e74 2864 6174 612e   cci = int(data.
-0001c3f0: 6865 6164 2831 295b 2243 4349 225d 2e69  head(1)["CCI"].i
-0001c400: 6c6f 635b 305d 290a 2020 2020 2020 2020  loc[0]).        
-0001c410: 7361 7665 4469 6374 5b22 4343 4922 5d20  saveDict["CCI"] 
-0001c420: 3d20 6363 690a 2020 2020 2020 2020 6966  = cci.        if
-0001c430: 2028 6363 6920 3e3d 206d 696e 4343 4920   (cci >= minCCI 
-0001c440: 616e 6420 6363 6920 3c3d 206d 6178 4343  and cci <= maxCC
-0001c450: 4929 3a0a 2020 2020 2020 2020 2020 2020  I):.            
-0001c460: 6966 2028 2255 7022 2069 6e20 7361 7665  if ("Up" in save
-0001c470: 4469 6374 5b22 5472 656e 6422 5d29 3a0a  Dict["Trend"]):.
-0001c480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c490: 7363 7265 656e 4469 6374 5b22 4343 4922  screenDict["CCI"
-0001c4a0: 5d20 3d20 280a 2020 2020 2020 2020 2020  ] = (.          
-0001c4b0: 2020 2020 2020 2020 2020 2863 6f6c 6f72            (color
-0001c4c0: 5465 7874 2e42 4f4c 4420 6966 2028 2253  Text.BOLD if ("S
-0001c4d0: 7472 6f6e 6722 2069 6e20 7361 7665 4469  trong" in saveDi
-0001c4e0: 6374 5b22 5472 656e 6422 5d29 2065 6c73  ct["Trend"]) els
-0001c4f0: 6520 2222 2920 2b20 636f 6c6f 7254 6578  e "") + colorTex
-0001c500: 742e 4752 4545 4e20 2b20 7374 7228 6363  t.GREEN + str(cc
-0001c510: 6929 202b 2063 6f6c 6f72 5465 7874 2e45  i) + colorText.E
-0001c520: 4e44 0a20 2020 2020 2020 2020 2020 2020  ND.             
-0001c530: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0001c540: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0001c550: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
-0001c560: 745b 2243 4349 225d 203d 2028 0a20 2020  t["CCI"] = (.   
-0001c570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c580: 2028 636f 6c6f 7254 6578 742e 424f 4c44   (colorText.BOLD
-0001c590: 2069 6620 2822 5374 726f 6e67 2220 696e   if ("Strong" in
-0001c5a0: 2073 6176 6544 6963 745b 2254 7265 6e64   saveDict["Trend
-0001c5b0: 225d 2920 656c 7365 2022 2229 202b 2063  "]) else "") + c
-0001c5c0: 6f6c 6f72 5465 7874 2e46 4149 4c20 2b20  olorText.FAIL + 
-0001c5d0: 7374 7228 6363 6929 202b 2063 6f6c 6f72  str(cci) + color
-0001c5e0: 5465 7874 2e45 4e44 0a20 2020 2020 2020  Text.END.       
-0001c5f0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0001c600: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-0001c610: 7565 0a20 2020 2020 2020 2073 6372 6565  ue.        scree
-0001c620: 6e44 6963 745b 2243 4349 225d 203d 2063  nDict["CCI"] = c
-0001c630: 6f6c 6f72 5465 7874 2e42 4f4c 4420 2b20  olorText.BOLD + 
-0001c640: 636f 6c6f 7254 6578 742e 4641 494c 202b  colorText.FAIL +
-0001c650: 2073 7472 2863 6369 2920 2b20 636f 6c6f   str(cci) + colo
-0001c660: 7254 6578 742e 454e 440a 2020 2020 2020  rText.END.      
-0001c670: 2020 7265 7475 726e 2046 616c 7365 0a0a    return False..
-0001c680: 2020 2020 2320 4669 6e64 2043 6f6e 666c      # Find Confl
-0001c690: 7563 656e 6365 0a20 2020 2064 6566 2076  ucence.    def v
-0001c6a0: 616c 6964 6174 6543 6f6e 666c 7565 6e63  alidateConfluenc
-0001c6b0: 6528 7365 6c66 2c20 7374 6f63 6b2c 2064  e(self, stock, d
-0001c6c0: 662c 2073 6372 6565 6e44 6963 742c 2073  f, screenDict, s
-0001c6d0: 6176 6544 6963 742c 2070 6572 6365 6e74  aveDict, percent
-0001c6e0: 6167 653d 302e 312c 636f 6e66 4669 6c74  age=0.1,confFilt
-0001c6f0: 6572 3d33 293a 0a20 2020 2020 2020 2069  er=3):.        i
-0001c700: 6620 6466 2069 7320 4e6f 6e65 206f 7220  f df is None or 
-0001c710: 6c65 6e28 6466 2920 3d3d 2030 3a0a 2020  len(df) == 0:.  
-0001c720: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0001c730: 2046 616c 7365 0a20 2020 2020 2020 2064   False.        d
-0001c740: 6174 6120 3d20 6466 2e63 6f70 7928 290a  ata = df.copy().
-0001c750: 2020 2020 2020 2020 7265 6365 6e74 203d          recent =
-0001c760: 2064 6174 612e 6865 6164 2832 290a 2020   data.head(2).  
-0001c770: 2020 2020 2020 6966 206c 656e 2872 6563        if len(rec
-0001c780: 656e 7429 203c 2032 3a0a 2020 2020 2020  ent) < 2:.      
-0001c790: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-0001c7a0: 7365 0a20 2020 2020 2020 206b 6579 3120  se.        key1 
-0001c7b0: 3d20 2253 4d41 220a 2020 2020 2020 2020  = "SMA".        
-0001c7c0: 6b65 7932 203d 2022 4c4d 4122 0a20 2020  key2 = "LMA".   
-0001c7d0: 2020 2020 206b 6579 3320 3d20 2235 3044       key3 = "50D
-0001c7e0: 4d41 220a 2020 2020 2020 2020 6b65 7934  MA".        key4
-0001c7f0: 203d 2022 3230 3044 4d41 220a 2020 2020   = "200DMA".    
-0001c800: 2020 2020 6973 3230 444d 4143 726f 7373      is20DMACross
-0001c810: 6f76 6572 3530 444d 4120 3d20 2872 6563  over50DMA = (rec
-0001c820: 656e 745b 2253 534d 4132 3022 5d2e 696c  ent["SSMA20"].il
-0001c830: 6f63 5b30 5d20 3e3d 2072 6563 656e 745b  oc[0] >= recent[
-0001c840: 2253 4d41 225d 2e69 6c6f 635b 305d 2920  "SMA"].iloc[0]) 
-0001c850: 616e 6420 5c0a 2020 2020 2020 2020 2020  and \.          
-0001c860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c870: 2020 2872 6563 656e 745b 2253 534d 4132    (recent["SSMA2
-0001c880: 3022 5d2e 696c 6f63 5b31 5d20 3c3d 2072  0"].iloc[1] <= r
-0001c890: 6563 656e 745b 2253 4d41 225d 2e69 6c6f  ecent["SMA"].ilo
-0001c8a0: 635b 315d 290a 2020 2020 2020 2020 6973  c[1]).        is
-0001c8b0: 3530 444d 4143 726f 7373 6f76 6572 3230  50DMACrossover20
-0001c8c0: 3044 4d41 203d 2028 7265 6365 6e74 5b22  0DMA = (recent["
-0001c8d0: 534d 4122 5d2e 696c 6f63 5b30 5d20 3e3d  SMA"].iloc[0] >=
-0001c8e0: 2072 6563 656e 745b 224c 4d41 225d 2e69   recent["LMA"].i
-0001c8f0: 6c6f 635b 305d 2920 616e 6420 5c0a 2020  loc[0]) and \.  
-0001c900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c910: 2020 2020 2020 2020 2020 2872 6563 656e            (recen
-0001c920: 745b 2253 4d41 225d 2e69 6c6f 635b 315d  t["SMA"].iloc[1]
-0001c930: 203c 3d20 7265 6365 6e74 5b22 4c4d 4122   <= recent["LMA"
-0001c940: 5d2e 696c 6f63 5b31 5d29 0a20 2020 2020  ].iloc[1]).     
-0001c950: 2020 2069 7347 6f6c 6465 6e43 726f 7373     isGoldenCross
-0001c960: 4f76 6572 203d 2069 7332 3044 4d41 4372  Over = is20DMACr
-0001c970: 6f73 736f 7665 7235 3044 4d41 206f 7220  ossover50DMA or 
-0001c980: 6973 3530 444d 4143 726f 7373 6f76 6572  is50DMACrossover
-0001c990: 3230 3044 4d41 0a20 2020 2020 2020 2069  200DMA.        i
-0001c9a0: 7335 3044 4d41 4372 6f73 736f 7665 7232  s50DMACrossover2
-0001c9b0: 3030 444d 4144 6f77 6e20 3d20 2872 6563  00DMADown = (rec
-0001c9c0: 656e 745b 2253 4d41 225d 2e69 6c6f 635b  ent["SMA"].iloc[
-0001c9d0: 305d 203c 3d20 7265 6365 6e74 5b22 4c4d  0] <= recent["LM
-0001c9e0: 4122 5d2e 696c 6f63 5b30 5d29 2061 6e64  A"].iloc[0]) and
-0001c9f0: 205c 0a20 2020 2020 2020 2020 2020 2020   \.             
-0001ca00: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-0001ca10: 7265 6365 6e74 5b22 534d 4122 5d2e 696c  recent["SMA"].il
-0001ca20: 6f63 5b31 5d20 3e3d 2072 6563 656e 745b  oc[1] >= recent[
-0001ca30: 224c 4d41 225d 2e69 6c6f 635b 315d 290a  "LMA"].iloc[1]).
-0001ca40: 2020 2020 2020 2020 6973 3230 444d 4143          is20DMAC
-0001ca50: 726f 7373 6f76 6572 3530 444d 4144 6f77  rossover50DMADow
-0001ca60: 6e20 3d20 2872 6563 656e 745b 2253 534d  n = (recent["SSM
-0001ca70: 4132 3022 5d2e 696c 6f63 5b30 5d20 3c3d  A20"].iloc[0] <=
-0001ca80: 2072 6563 656e 745b 2253 4d41 225d 2e69   recent["SMA"].i
-0001ca90: 6c6f 635b 305d 2920 616e 6420 5c0a 2020  loc[0]) and \.  
-0001caa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cab0: 2020 2020 2020 2020 2020 2872 6563 656e            (recen
-0001cac0: 745b 2253 534d 4132 3022 5d2e 696c 6f63  t["SSMA20"].iloc
-0001cad0: 5b31 5d20 3e3d 2072 6563 656e 745b 2253  [1] >= recent["S
-0001cae0: 4d41 225d 2e69 6c6f 635b 315d 290a 2020  MA"].iloc[1]).  
-0001caf0: 2020 2020 2020 6973 4465 6164 4372 6f73        isDeadCros
-0001cb00: 734f 7665 7220 3d20 6973 3230 444d 4143  sOver = is20DMAC
-0001cb10: 726f 7373 6f76 6572 3530 444d 4144 6f77  rossover50DMADow
-0001cb20: 6e20 6f72 2069 7335 3044 4d41 4372 6f73  n or is50DMACros
-0001cb30: 736f 7665 7232 3030 444d 4144 6f77 6e0a  sover200DMADown.
-0001cb40: 2020 2020 2020 2020 6465 6164 784f 7665          deadxOve
-0001cb50: 7254 6578 7420 3d20 6627 4465 6164 4372  rText = f'DeadCr
-0001cb60: 6f73 736f 7665 727b 2228 3230 2922 2069  ossover{"(20)" i
-0001cb70: 6620 6973 3230 444d 4143 726f 7373 6f76  f is20DMACrossov
-0001cb80: 6572 3530 444d 4144 6f77 6e20 656c 7365  er50DMADown else
-0001cb90: 2028 2228 3530 2922 2069 6620 6973 3530   ("(50)" if is50
-0001cba0: 444d 4143 726f 7373 6f76 6572 3230 3044  DMACrossover200D
-0001cbb0: 4d41 446f 776e 2065 6c73 6520 2222 297d  MADown else "")}
-0001cbc0: 270a 2020 2020 2020 2020 676f 6c64 656e  '.        golden
-0001cbd0: 784f 7665 7254 6578 7420 3d20 6627 476f  xOverText = f'Go
-0001cbe0: 6c64 656e 4372 6f73 736f 7665 727b 2228  ldenCrossover{"(
-0001cbf0: 3230 2922 2069 6620 6973 3230 444d 4143  20)" if is20DMAC
-0001cc00: 726f 7373 6f76 6572 3530 444d 4120 656c  rossover50DMA el
-0001cc10: 7365 2028 2228 3530 2922 2069 6620 6973  se ("(50)" if is
-0001cc20: 3530 444d 4143 726f 7373 6f76 6572 3230  50DMACrossover20
-0001cc30: 3044 4d41 2065 6c73 6520 2222 297d 270a  0DMA else "")}'.
-0001cc40: 2020 2020 2020 2020 6966 2069 7332 3044          if is20D
-0001cc50: 4d41 4372 6f73 736f 7665 7235 3044 4d41  MACrossover50DMA
-0001cc60: 206f 7220 6973 3230 444d 4143 726f 7373   or is20DMACross
-0001cc70: 6f76 6572 3530 444d 4144 6f77 6e3a 0a20  over50DMADown:. 
-0001cc80: 2020 2020 2020 2020 2020 206b 6579 3120             key1 
-0001cc90: 3d20 2253 534d 4132 3022 0a20 2020 2020  = "SSMA20".     
-0001cca0: 2020 2020 2020 206b 6579 3220 3d20 2253         key2 = "S
-0001ccb0: 4d41 220a 2020 2020 2020 2020 2020 2020  MA".            
-0001ccc0: 6b65 7933 203d 2022 3230 444d 4122 0a20  key3 = "20DMA". 
-0001ccd0: 2020 2020 2020 2020 2020 206b 6579 3420             key4 
-0001cce0: 3d20 2235 3044 4d41 220a 2020 2020 2020  = "50DMA".      
-0001ccf0: 2020 6973 3530 444d 4155 7054 7265 6e64    is50DMAUpTrend
-0001cd00: 203d 2028 7265 6365 6e74 5b6b 6579 315d   = (recent[key1]
-0001cd10: 2e69 6c6f 635b 305d 203e 2072 6563 656e  .iloc[0] > recen
-0001cd20: 745b 6b65 7932 5d2e 696c 6f63 5b31 5d29  t[key2].iloc[1])
-0001cd30: 0a20 2020 2020 2020 2069 7335 3044 4d41  .        is50DMA
-0001cd40: 446f 776e 5472 656e 6420 3d20 2872 6563  DownTrend = (rec
-0001cd50: 656e 745b 6b65 7931 5d2e 696c 6f63 5b30  ent[key1].iloc[0
-0001cd60: 5d20 3c20 7265 6365 6e74 5b6b 6579 315d  ] < recent[key1]
-0001cd70: 2e69 6c6f 635b 315d 290a 2020 2020 2020  .iloc[1]).      
-0001cd80: 2020 6973 3530 444d 4120 3d20 2872 6563    is50DMA = (rec
-0001cd90: 656e 745b 6b65 7931 5d2e 696c 6f63 5b30  ent[key1].iloc[0
-0001cda0: 5d20 3c3d 2072 6563 656e 745b 2243 6c6f  ] <= recent["Clo
-0001cdb0: 7365 225d 2e69 6c6f 635b 305d 290a 2020  se"].iloc[0]).  
-0001cdc0: 2020 2020 2020 6973 3230 3044 4d41 203d        is200DMA =
-0001cdd0: 2028 7265 6365 6e74 5b6b 6579 325d 2e69   (recent[key2].i
-0001cde0: 6c6f 635b 305d 203c 3d20 7265 6365 6e74  loc[0] <= recent
-0001cdf0: 5b22 436c 6f73 6522 5d2e 696c 6f63 5b30  ["Close"].iloc[0
-0001ce00: 5d29 0a20 2020 2020 2020 2064 6966 6665  ]).        diffe
-0001ce10: 7265 6e63 6520 3d20 726f 756e 6428 2872  rence = round((r
-0001ce20: 6563 656e 745b 6b65 7931 5d2e 696c 6f63  ecent[key1].iloc
-0001ce30: 5b30 5d20 2d20 7265 6365 6e74 5b6b 6579  [0] - recent[key
-0001ce40: 325d 2e69 6c6f 635b 305d 290a 2020 2020  2].iloc[0]).    
-0001ce50: 2020 2020 2020 2020 2020 2020 2f20 7265              / re
-0001ce60: 6365 6e74 5b22 436c 6f73 6522 5d2e 696c  cent["Close"].il
-0001ce70: 6f63 5b30 5d0a 2020 2020 2020 2020 2020  oc[0].          
-0001ce80: 2020 2020 2020 2a20 3130 302c 0a20 2020        * 100,.   
-0001ce90: 2020 2020 2020 2020 2020 2020 2032 2c0a               2,.
-0001cea0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0001ceb0: 2020 2020 2020 7361 7665 4469 6374 5b22        saveDict["
-0001cec0: 436f 6e66 444d 4144 6966 6665 7265 6e63  ConfDMADifferenc
-0001ced0: 6522 5d20 3d20 6469 6666 6572 656e 6365  e"] = difference
-0001cee0: 0a20 2020 2020 2020 2073 6372 6565 6e44  .        screenD
-0001cef0: 6963 745b 2243 6f6e 6644 4d41 4469 6666  ict["ConfDMADiff
-0001cf00: 6572 656e 6365 225d 203d 2064 6966 6665  erence"] = diffe
-0001cf10: 7265 6e63 650a 2020 2020 2020 2020 7361  rence.        sa
-0001cf20: 7665 6420 3d20 7365 6c66 2e66 696e 6443  ved = self.findC
-0001cf30: 7572 7265 6e74 5361 7665 6456 616c 7565  urrentSavedValue
-0001cf40: 2873 6372 6565 6e44 6963 742c 7361 7665  (screenDict,save
-0001cf50: 4469 6374 2c22 4d41 2d53 6967 6e61 6c22  Dict,"MA-Signal"
-0001cf60: 290a 2020 2020 2020 2020 2320 6469 6666  ).        # diff
-0001cf70: 6572 656e 6365 203d 2061 6273 2864 6966  erence = abs(dif
-0001cf80: 6665 7265 6e63 6529 0a20 2020 2020 2020  ference).       
-0001cf90: 2063 6f6e 6654 6578 7420 3d20 6622 7b67   confText = f"{g
-0001cfa0: 6f6c 6465 6e78 4f76 6572 5465 7874 2069  oldenxOverText i
-0001cfb0: 6620 6973 476f 6c64 656e 4372 6f73 734f  f isGoldenCrossO
-0001cfc0: 7665 7220 656c 7365 2028 6465 6164 784f  ver else (deadxO
-0001cfd0: 7665 7254 6578 7420 6966 2069 7344 6561  verText if isDea
-0001cfe0: 6443 726f 7373 4f76 6572 2065 6c73 6520  dCrossOver else 
-0001cff0: 2827 436f 6e66 2e55 7027 2069 6620 6973  ('Conf.Up' if is
-0001d000: 3530 444d 4155 7054 7265 6e64 2065 6c73  50DMAUpTrend els
-0001d010: 6520 2827 436f 6e66 2e44 6f77 6e27 2069  e ('Conf.Down' i
-0001d020: 6620 6973 3530 444d 4144 6f77 6e54 7265  f is50DMADownTre
-0001d030: 6e64 2065 6c73 6520 286b 6579 3320 6966  nd else (key3 if
-0001d040: 2069 7335 3044 4d41 2065 6c73 6520 286b   is50DMA else (k
-0001d050: 6579 3420 6966 2069 7332 3030 444d 4120  ey4 if is200DMA 
-0001d060: 656c 7365 2027 556e 6b6e 6f77 6e27 2929  else 'Unknown'))
-0001d070: 2929 297d 220a 2020 2020 2020 2020 6966  )))}".        if
-0001d080: 2061 6273 2872 6563 656e 745b 6b65 7931   abs(recent[key1
-0001d090: 5d2e 696c 6f63 5b30 5d20 2d20 7265 6365  ].iloc[0] - rece
-0001d0a0: 6e74 5b6b 6579 325d 2e69 6c6f 635b 305d  nt[key2].iloc[0]
-0001d0b0: 2920 3c3d 2028 0a20 2020 2020 2020 2020  ) <= (.         
-0001d0c0: 2020 2072 6563 656e 745b 6b65 7931 5d2e     recent[key1].
-0001d0d0: 696c 6f63 5b30 5d20 2a20 7065 7263 656e  iloc[0] * percen
-0001d0e0: 7461 6765 0a20 2020 2020 2020 2029 3a0a  tage.        ):.
-0001d0f0: 2020 2020 2020 2020 2020 2020 6966 2072              if r
-0001d100: 6563 656e 745b 6b65 7931 5d2e 696c 6f63  ecent[key1].iloc
-0001d110: 5b30 5d20 3e3d 2072 6563 656e 745b 6b65  [0] >= recent[ke
-0001d120: 7932 5d2e 696c 6f63 5b30 5d3a 0a20 2020  y2].iloc[0]:.   
-0001d130: 2020 2020 2020 2020 2020 2020 2073 6372               scr
-0001d140: 6565 6e44 6963 745b 224d 412d 5369 676e  eenDict["MA-Sign
-0001d150: 616c 225d 203d 2028 0a20 2020 2020 2020  al"] = (.       
-0001d160: 2020 2020 2020 2020 2020 2020 2073 6176               sav
-0001d170: 6564 5b30 5d20 0a20 2020 2020 2020 2020  ed[0] .         
-0001d180: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
-0001d190: 6f72 5465 7874 2e42 4f4c 440a 2020 2020  orText.BOLD.    
-0001d1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d1b0: 2b20 2863 6f6c 6f72 5465 7874 2e47 5245  + (colorText.GRE
-0001d1c0: 454e 2069 6620 6973 3530 444d 4155 7054  EN if is50DMAUpT
-0001d1d0: 7265 6e64 2065 6c73 6520 2863 6f6c 6f72  rend else (color
-0001d1e0: 5465 7874 2e46 4149 4c20 6966 2069 7335  Text.FAIL if is5
-0001d1f0: 3044 4d41 446f 776e 5472 656e 6420 656c  0DMADownTrend el
-0001d200: 7365 2063 6f6c 6f72 5465 7874 2e57 4152  se colorText.WAR
-0001d210: 4e29 290a 2020 2020 2020 2020 2020 2020  N)).            
-0001d220: 2020 2020 2020 2020 2b20 6622 7b63 6f6e          + f"{con
-0001d230: 6654 6578 747d 2028 7b64 6966 6665 7265  fText} ({differe
-0001d240: 6e63 657d 2529 220a 2020 2020 2020 2020  nce}%)".        
-0001d250: 2020 2020 2020 2020 2020 2020 2b20 636f              + co
-0001d260: 6c6f 7254 6578 742e 454e 440a 2020 2020  lorText.END.    
-0001d270: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0001d280: 2020 2020 2020 2020 2020 2020 2020 7361                sa
-0001d290: 7665 4469 6374 5b22 4d41 2d53 6967 6e61  veDict["MA-Signa
-0001d2a0: 6c22 5d20 3d20 7361 7665 645b 315d 202b  l"] = saved[1] +
-0001d2b0: 2066 227b 636f 6e66 5465 7874 7d20 287b   f"{confText} ({
-0001d2c0: 6469 6666 6572 656e 6365 7d25 2922 0a20  difference}%)". 
-0001d2d0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0001d2e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001d2f0: 2073 6372 6565 6e44 6963 745b 224d 412d   screenDict["MA-
-0001d300: 5369 676e 616c 225d 203d 2028 0a20 2020  Signal"] = (.   
-0001d310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d320: 2073 6176 6564 5b30 5d20 0a20 2020 2020   saved[0] .     
-0001d330: 2020 2020 2020 2020 2020 2020 2020 202b                 +
-0001d340: 2063 6f6c 6f72 5465 7874 2e42 4f4c 440a   colorText.BOLD.
-0001d350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d360: 2020 2020 2b20 2863 6f6c 6f72 5465 7874      + (colorText
-0001d370: 2e47 5245 454e 2069 6620 6973 3530 444d  .GREEN if is50DM
-0001d380: 4155 7054 7265 6e64 2065 6c73 6520 2863  AUpTrend else (c
-0001d390: 6f6c 6f72 5465 7874 2e46 4149 4c20 6966  olorText.FAIL if
-0001d3a0: 2069 7335 3044 4d41 446f 776e 5472 656e   is50DMADownTren
-0001d3b0: 6420 656c 7365 2063 6f6c 6f72 5465 7874  d else colorText
-0001d3c0: 2e57 4152 4e29 290a 2020 2020 2020 2020  .WARN)).        
-0001d3d0: 2020 2020 2020 2020 2020 2020 2b20 6622              + f"
-0001d3e0: 7b63 6f6e 6654 6578 747d 2028 7b64 6966  {confText} ({dif
-0001d3f0: 6665 7265 6e63 657d 2529 220a 2020 2020  ference}%)".    
-0001d400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d410: 2b20 636f 6c6f 7254 6578 742e 454e 440a  + colorText.END.
-0001d420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d430: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001d440: 2020 7361 7665 4469 6374 5b22 4d41 2d53    saveDict["MA-S
-0001d450: 6967 6e61 6c22 5d20 3d20 7361 7665 645b  ignal"] = saved[
-0001d460: 315d 202b 2066 227b 636f 6e66 5465 7874  1] + f"{confText
-0001d470: 7d20 287b 6469 6666 6572 656e 6365 7d25  } ({difference}%
-0001d480: 2922 0a20 2020 2020 2020 2020 2020 2072  )".            r
-0001d490: 6574 7572 6e20 636f 6e66 4669 6c74 6572  eturn confFilter
-0001d4a0: 203d 3d20 3320 6f72 205c 0a20 2020 2020   == 3 or \.     
-0001d4b0: 2020 2020 2020 2020 2020 2028 636f 6e66             (conf
-0001d4c0: 4669 6c74 6572 203d 3d20 3120 616e 6420  Filter == 1 and 
-0001d4d0: 6e6f 7420 6973 4465 6164 4372 6f73 734f  not isDeadCrossO
-0001d4e0: 7665 7220 616e 6420 2869 7335 3044 4d41  ver and (is50DMA
-0001d4f0: 5570 5472 656e 6420 6f72 2028 6973 476f  UpTrend or (isGo
-0001d500: 6c64 656e 4372 6f73 734f 7665 7220 6f72  ldenCrossOver or
-0001d510: 2027 5570 2720 696e 2063 6f6e 6654 6578   'Up' in confTex
-0001d520: 7429 2929 206f 7220 5c0a 2020 2020 2020  t))) or \.      
-0001d530: 2020 2020 2020 2020 2020 2863 6f6e 6646            (confF
-0001d540: 696c 7465 7220 3d3d 2032 2061 6e64 206e  ilter == 2 and n
-0001d550: 6f74 2069 7347 6f6c 6465 6e43 726f 7373  ot isGoldenCross
-0001d560: 4f76 6572 2061 6e64 2028 6973 3530 444d  Over and (is50DM
-0001d570: 4144 6f77 6e54 7265 6e64 206f 7220 6973  ADownTrend or is
-0001d580: 4465 6164 4372 6f73 734f 7665 7220 6f72  DeadCrossOver or
-0001d590: 2027 446f 776e 2720 696e 2063 6f6e 6654   'Down' in confT
-0001d5a0: 6578 7429 290a 2020 2020 2020 2020 2320  ext)).        # 
-0001d5b0: 4d61 7962 6520 7468 6520 6469 6666 6572  Maybe the differ
-0001d5c0: 656e 6365 2069 7320 6e6f 7420 7769 7468  ence is not with
-0001d5d0: 696e 2074 6865 2072 616e 6765 2c20 6275  in the range, bu
-0001d5e0: 7420 7765 2764 2073 7469 6c6c 206c 696b  t we'd still lik
-0001d5f0: 6520 746f 206b 6565 7020 7468 6520 7374  e to keep the st
-0001d600: 6f63 6b20 696e 0a20 2020 2020 2020 2023  ock in.        #
-0001d610: 2074 6865 206c 6973 7420 6966 2069 7427   the list if it'
-0001d620: 7320 6120 676f 6c64 656e 2063 726f 7373  s a golden cross
-0001d630: 6f76 6572 206f 7220 6465 6164 2063 726f  over or dead cro
-0001d640: 7373 6f76 6572 0a20 2020 2020 2020 2069  ssover.        i
-0001d650: 6620 6973 476f 6c64 656e 4372 6f73 734f  f isGoldenCrossO
-0001d660: 7665 7220 6f72 2069 7344 6561 6443 726f  ver or isDeadCro
-0001d670: 7373 4f76 6572 3a0a 2020 2020 2020 2020  ssOver:.        
-0001d680: 2020 2020 7363 7265 656e 4469 6374 5b22      screenDict["
-0001d690: 4d41 2d53 6967 6e61 6c22 5d20 3d20 280a  MA-Signal"] = (.
-0001d6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d6b0: 2020 2020 7361 7665 645b 305d 200a 2020      saved[0] .  
-0001d6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d6d0: 2020 2b20 636f 6c6f 7254 6578 742e 424f    + colorText.BO
-0001d6e0: 4c44 0a20 2020 2020 2020 2020 2020 2020  LD.             
-0001d6f0: 2020 2020 2020 202b 2028 636f 6c6f 7254         + (colorT
-0001d700: 6578 742e 4752 4545 4e20 6966 2069 7335  ext.GREEN if is5
-0001d710: 3044 4d41 5570 5472 656e 6420 656c 7365  0DMAUpTrend else
-0001d720: 2028 636f 6c6f 7254 6578 742e 4641 494c   (colorText.FAIL
-0001d730: 2069 6620 6973 3530 444d 4144 6f77 6e54   if is50DMADownT
-0001d740: 7265 6e64 2065 6c73 6520 636f 6c6f 7254  rend else colorT
-0001d750: 6578 742e 5741 524e 2929 0a20 2020 2020  ext.WARN)).     
-0001d760: 2020 2020 2020 2020 2020 2020 2020 202b                 +
-0001d770: 2066 227b 636f 6e66 5465 7874 7d20 287b   f"{confText} ({
-0001d780: 6469 6666 6572 656e 6365 7d25 2922 0a20  difference}%)". 
-0001d790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d7a0: 2020 202b 2063 6f6c 6f72 5465 7874 2e45     + colorText.E
-0001d7b0: 4e44 0a20 2020 2020 2020 2020 2020 2020  ND.             
-0001d7c0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0001d7d0: 2073 6176 6544 6963 745b 224d 412d 5369   saveDict["MA-Si
-0001d7e0: 676e 616c 225d 203d 2073 6176 6564 5b31  gnal"] = saved[1
-0001d7f0: 5d20 2b20 6622 7b63 6f6e 6654 6578 747d  ] + f"{confText}
-0001d800: 2028 7b64 6966 6665 7265 6e63 657d 2529   ({difference}%)
-0001d810: 220a 2020 2020 2020 2020 2020 2020 7265  ".            re
-0001d820: 7475 726e 2063 6f6e 6646 696c 7465 7220  turn confFilter 
-0001d830: 3d3d 2033 206f 7220 5c0a 2020 2020 2020  == 3 or \.      
-0001d840: 2020 2020 2020 2020 2020 2863 6f6e 6646            (confF
-0001d850: 696c 7465 7220 3d3d 2031 2061 6e64 2069  ilter == 1 and i
-0001d860: 7347 6f6c 6465 6e43 726f 7373 4f76 6572  sGoldenCrossOver
-0001d870: 2920 6f72 205c 0a20 2020 2020 2020 2020  ) or \.         
-0001d880: 2020 2020 2020 2028 636f 6e66 4669 6c74         (confFilt
-0001d890: 6572 203d 3d20 3220 616e 6420 6973 4465  er == 2 and isDe
-0001d8a0: 6164 4372 6f73 734f 7665 7229 0a20 2020  adCrossOver).   
-0001d8b0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-0001d8c0: 650a 0a20 2020 2023 406d 6561 7375 7265  e..    #@measure
-0001d8d0: 5f74 696d 650a 2020 2020 2320 5661 6c69  _time.    # Vali
-0001d8e0: 6461 7465 2069 6620 7368 6172 6520 7072  date if share pr
-0001d8f0: 6963 6573 2061 7265 2063 6f6e 736f 6c69  ices are consoli
-0001d900: 6461 7469 6e67 0a20 2020 2064 6566 2076  dating.    def v
-0001d910: 616c 6964 6174 6543 6f6e 736f 6c69 6461  alidateConsolida
-0001d920: 7469 6f6e 2873 656c 662c 2064 662c 2073  tion(self, df, s
-0001d930: 6372 6565 6e44 6963 742c 2073 6176 6544  creenDict, saveD
-0001d940: 6963 742c 2070 6572 6365 6e74 6167 653d  ict, percentage=
-0001d950: 3130 293a 0a20 2020 2020 2020 2069 6620  10):.        if 
-0001d960: 6466 2069 7320 4e6f 6e65 206f 7220 6c65  df is None or le
-0001d970: 6e28 6466 2920 3d3d 2030 3a0a 2020 2020  n(df) == 0:.    
-0001d980: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-0001d990: 616c 7365 0a20 2020 2020 2020 2064 6174  alse.        dat
-0001d9a0: 6120 3d20 6466 2e63 6f70 7928 290a 2020  a = df.copy().  
-0001d9b0: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
-0001d9c0: 612e 6669 6c6c 6e61 2830 290a 2020 2020  a.fillna(0).    
-0001d9d0: 2020 2020 6461 7461 203d 2064 6174 612e      data = data.
-0001d9e0: 7265 706c 6163 6528 5b6e 702e 696e 662c  replace([np.inf,
-0001d9f0: 202d 6e70 2e69 6e66 5d2c 2030 290a 2020   -np.inf], 0).  
-0001da00: 2020 2020 2020 6863 203d 2064 6174 612e        hc = data.
-0001da10: 6465 7363 7269 6265 2829 5b22 436c 6f73  describe()["Clos
-0001da20: 6522 5d5b 226d 6178 225d 0a20 2020 2020  e"]["max"].     
-0001da30: 2020 206c 6320 3d20 6461 7461 2e64 6573     lc = data.des
-0001da40: 6372 6962 6528 295b 2243 6c6f 7365 225d  cribe()["Close"]
-0001da50: 5b22 6d69 6e22 5d0a 2020 2020 2020 2020  ["min"].        
-0001da60: 6966 2028 6863 202d 206c 6329 203c 3d20  if (hc - lc) <= 
-0001da70: 2868 6320 2a20 7065 7263 656e 7461 6765  (hc * percentage
-0001da80: 202f 2031 3030 2920 616e 6420 2868 6320   / 100) and (hc 
-0001da90: 2d20 6c63 2021 3d20 3029 3a0a 2020 2020  - lc != 0):.    
-0001daa0: 2020 2020 2020 2020 7363 7265 656e 4469          screenDi
-0001dab0: 6374 5b22 436f 6e73 6f6c 2e22 5d20 3d20  ct["Consol."] = 
-0001dac0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0001dad0: 2020 636f 6c6f 7254 6578 742e 424f 4c44    colorText.BOLD
-0001dae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001daf0: 202b 2063 6f6c 6f72 5465 7874 2e47 5245   + colorText.GRE
-0001db00: 454e 0a20 2020 2020 2020 2020 2020 2020  EN.             
-0001db10: 2020 202b 2022 5261 6e67 653a 220a 2020     + "Range:".  
-0001db20: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-0001db30: 7374 7228 726f 756e 6428 2861 6273 2828  str(round((abs((
-0001db40: 6863 202d 206c 6329 202f 2068 6329 202a  hc - lc) / hc) *
-0001db50: 2031 3030 292c 2031 2929 0a20 2020 2020   100), 1)).     
-0001db60: 2020 2020 2020 2020 2020 202b 2022 2522             + "%"
-0001db70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001db80: 202b 2063 6f6c 6f72 5465 7874 2e45 4e44   + colorText.END
-0001db90: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-0001dba0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0001dbb0: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
-0001dbc0: 6963 745b 2243 6f6e 736f 6c2e 225d 203d  ict["Consol."] =
-0001dbd0: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
-0001dbe0: 2020 2063 6f6c 6f72 5465 7874 2e42 4f4c     colorText.BOL
-0001dbf0: 440a 2020 2020 2020 2020 2020 2020 2020  D.              
-0001dc00: 2020 2b20 636f 6c6f 7254 6578 742e 4641    + colorText.FA
-0001dc10: 494c 0a20 2020 2020 2020 2020 2020 2020  IL.             
-0001dc20: 2020 202b 2022 5261 6e67 653a 220a 2020     + "Range:".  
-0001dc30: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-0001dc40: 7374 7228 726f 756e 6428 2861 6273 2828  str(round((abs((
-0001dc50: 6863 202d 206c 6329 202f 2068 6329 202a  hc - lc) / hc) *
-0001dc60: 2031 3030 292c 2031 2929 0a20 2020 2020   100), 1)).     
-0001dc70: 2020 2020 2020 2020 2020 202b 2022 2522             + "%"
-0001dc80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001dc90: 202b 2063 6f6c 6f72 5465 7874 2e45 4e44   + colorText.END
-0001dca0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-0001dcb0: 2020 2020 2020 2073 6176 6544 6963 745b         saveDict[
-0001dcc0: 2243 6f6e 736f 6c2e 225d 203d 2066 2752  "Consol."] = f'R
-0001dcd0: 616e 6765 3a7b 7374 7228 726f 756e 6428  ange:{str(round(
-0001dce0: 2861 6273 2828 6863 2d6c 6329 2f68 6329  (abs((hc-lc)/hc)
-0001dcf0: 2a31 3030 292c 3129 292b 2225 227d 270a  *100),1))+"%"}'.
-0001dd00: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-0001dd10: 6f75 6e64 2828 6162 7328 2868 6320 2d20  ound((abs((hc - 
-0001dd20: 6c63 2920 2f20 6863 2920 2a20 3130 3029  lc) / hc) * 100)
-0001dd30: 2c20 3129 0a0a 2020 2020 2320 7661 6c69  , 1)..    # vali
-0001dd40: 6461 7465 2069 6620 7468 6520 7374 6f63  date if the stoc
-0001dd50: 6b20 6861 7320 6265 656e 2068 6176 696e  k has been havin
-0001dd60: 6720 6869 6768 6572 2068 6967 6873 2c20  g higher highs, 
-0001dd70: 6869 6768 6572 206c 6f77 730a 2020 2020  higher lows.    
-0001dd80: 2320 616e 6420 6869 6768 6572 2063 6c6f  # and higher clo
-0001dd90: 7365 2077 6974 6820 6c61 7465 7374 2063  se with latest c
-0001dda0: 6c6f 7365 203e 2073 7570 6572 7472 656e  lose > supertren
-0001ddb0: 6420 616e 6420 382d 454d 412e 0a20 2020  d and 8-EMA..   
-0001ddc0: 2064 6566 2076 616c 6964 6174 6548 6967   def validateHig
-0001ddd0: 6865 7248 6967 6873 4869 6768 6572 4c6f  herHighsHigherLo
-0001dde0: 7773 4869 6768 6572 436c 6f73 6528 7365  wsHigherClose(se
-0001ddf0: 6c66 2c20 6466 293a 0a20 2020 2020 2020  lf, df):.       
-0001de00: 2069 6620 6466 2069 7320 4e6f 6e65 206f   if df is None o
-0001de10: 7220 6c65 6e28 6466 2920 3d3d 2030 3a0a  r len(df) == 0:.
-0001de20: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0001de30: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
-0001de40: 2064 6174 6120 3d20 6466 2e63 6f70 7928   data = df.copy(
-0001de50: 290a 2020 2020 2020 2020 6461 7930 203d  ).        day0 =
-0001de60: 2064 6174 610a 2020 2020 2020 2020 6461   data.        da
-0001de70: 7931 203d 2064 6174 615b 313a 5d0a 2020  y1 = data[1:].  
-0001de80: 2020 2020 2020 6461 7932 203d 2064 6174        day2 = dat
-0001de90: 615b 323a 5d0a 2020 2020 2020 2020 6461  a[2:].        da
-0001dea0: 7933 203d 2064 6174 615b 333a 5d0a 2020  y3 = data[3:].  
-0001deb0: 2020 2020 2020 6966 206c 656e 2864 6179        if len(day
-0001dec0: 3129 203c 2031 206f 7220 6c65 6e28 6461  1) < 1 or len(da
-0001ded0: 7932 2920 3c20 3120 6f72 206c 656e 2864  y2) < 1 or len(d
-0001dee0: 6179 3329 203c 2031 3a0a 2020 2020 2020  ay3) < 1:.      
-0001def0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-0001df00: 7365 0a20 2020 2020 2020 2068 6967 6865  se.        highe
-0001df10: 7248 6967 6873 203d 2028 0a20 2020 2020  rHighs = (.     
-0001df20: 2020 2020 2020 2028 6461 7930 5b22 4869         (day0["Hi
-0001df30: 6768 225d 2e69 6c6f 635b 305d 203e 2064  gh"].iloc[0] > d
-0001df40: 6179 315b 2248 6967 6822 5d2e 696c 6f63  ay1["High"].iloc
-0001df50: 5b30 5d29 0a20 2020 2020 2020 2020 2020  [0]).           
-0001df60: 2061 6e64 2028 6461 7931 5b22 4869 6768   and (day1["High
-0001df70: 225d 2e69 6c6f 635b 305d 203e 2064 6179  "].iloc[0] > day
-0001df80: 325b 2248 6967 6822 5d2e 696c 6f63 5b30  2["High"].iloc[0
-0001df90: 5d29 0a20 2020 2020 2020 2020 2020 2061  ]).            a
-0001dfa0: 6e64 2028 6461 7932 5b22 4869 6768 225d  nd (day2["High"]
-0001dfb0: 2e69 6c6f 635b 305d 203e 2064 6179 335b  .iloc[0] > day3[
-0001dfc0: 2248 6967 6822 5d2e 696c 6f63 5b30 5d29  "High"].iloc[0])
-0001dfd0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-0001dfe0: 2020 2068 6967 6865 724c 6f77 7320 3d20     higherLows = 
-0001dff0: 280a 2020 2020 2020 2020 2020 2020 2864  (.            (d
-0001e000: 6179 305b 224c 6f77 225d 2e69 6c6f 635b  ay0["Low"].iloc[
-0001e010: 305d 203e 2064 6179 315b 224c 6f77 225d  0] > day1["Low"]
-0001e020: 2e69 6c6f 635b 305d 290a 2020 2020 2020  .iloc[0]).      
-0001e030: 2020 2020 2020 616e 6420 2864 6179 315b        and (day1[
-0001e040: 224c 6f77 225d 2e69 6c6f 635b 305d 203e  "Low"].iloc[0] >
-0001e050: 2064 6179 325b 224c 6f77 225d 2e69 6c6f   day2["Low"].ilo
-0001e060: 635b 305d 290a 2020 2020 2020 2020 2020  c[0]).          
-0001e070: 2020 616e 6420 2864 6179 325b 224c 6f77    and (day2["Low
-0001e080: 225d 2e69 6c6f 635b 305d 203e 2064 6179  "].iloc[0] > day
-0001e090: 335b 224c 6f77 225d 2e69 6c6f 635b 305d  3["Low"].iloc[0]
-0001e0a0: 290a 2020 2020 2020 2020 290a 2020 2020  ).        ).    
-0001e0b0: 2020 2020 6869 6768 6572 436c 6f73 6520      higherClose 
-0001e0c0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-0001e0d0: 2864 6179 305b 2243 6c6f 7365 225d 2e69  (day0["Close"].i
-0001e0e0: 6c6f 635b 305d 203e 2064 6179 315b 2243  loc[0] > day1["C
-0001e0f0: 6c6f 7365 225d 2e69 6c6f 635b 305d 290a  lose"].iloc[0]).
-0001e100: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-0001e110: 2864 6179 315b 2243 6c6f 7365 225d 2e69  (day1["Close"].i
-0001e120: 6c6f 635b 305d 203e 2064 6179 325b 2243  loc[0] > day2["C
-0001e130: 6c6f 7365 225d 2e69 6c6f 635b 305d 290a  lose"].iloc[0]).
-0001e140: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-0001e150: 2864 6179 325b 2243 6c6f 7365 225d 2e69  (day2["Close"].i
-0001e160: 6c6f 635b 305d 203e 2064 6179 335b 2243  loc[0] > day3["C
-0001e170: 6c6f 7365 225d 2e69 6c6f 635b 305d 290a  lose"].iloc[0]).
-0001e180: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0001e190: 2020 2320 6869 6768 6572 5253 4920 3d20    # higherRSI = 
-0001e1a0: 2864 6179 305b 2252 5349 225d 2e69 6c6f  (day0["RSI"].ilo
-0001e1b0: 635b 305d 203e 2064 6179 315b 2252 5349  c[0] > day1["RSI
-0001e1c0: 225d 2e69 6c6f 635b 305d 2920 616e 6420  "].iloc[0]) and 
-0001e1d0: 5c0a 2020 2020 2020 2020 2320 2020 2020  \.        #     
-0001e1e0: 2020 2020 2020 2020 2020 2020 2864 6179              (day
-0001e1f0: 315b 2252 5349 225d 2e69 6c6f 635b 305d  1["RSI"].iloc[0]
-0001e200: 203e 2064 6179 325b 2252 5349 225d 2e69   > day2["RSI"].i
-0001e210: 6c6f 635b 305d 2920 616e 6420 5c0a 2020  loc[0]) and \.  
-0001e220: 2020 2020 2020 2320 2020 2020 2020 2020        #         
-0001e230: 2020 2020 2020 2020 2864 6179 325b 2252          (day2["R
-0001e240: 5349 225d 2e69 6c6f 635b 305d 203e 2064  SI"].iloc[0] > d
-0001e250: 6179 335b 2252 5349 225d 2e69 6c6f 635b  ay3["RSI"].iloc[
-0001e260: 305d 2920 616e 6420 5c0a 2020 2020 2020  0]) and \.      
-0001e270: 2020 2320 2020 2020 2020 2020 2020 2020    #             
-0001e280: 2020 2020 6461 7933 5b22 5253 4922 5d2e      day3["RSI"].
-0001e290: 696c 6f63 5b30 5d20 3e3d 2035 3020 616e  iloc[0] >= 50 an
-0001e2a0: 6420 6461 7930 5b22 5253 4922 5d2e 696c  d day0["RSI"].il
-0001e2b0: 6f63 5b30 5d20 3e3d 2036 350a 2020 2020  oc[0] >= 65.    
-0001e2c0: 2020 2020 7265 7665 7273 6564 4461 7461      reversedData
-0001e2d0: 203d 2064 6174 615b 3a3a 2d31 5d2e 636f   = data[::-1].co
-0001e2e0: 7079 2829 0a20 2020 2020 2020 2072 6576  py().        rev
-0001e2f0: 6572 7365 6444 6174 615b 2253 5550 4552  ersedData["SUPER
-0001e300: 5422 5d20 3d20 706b 7461 6c69 622e 7375  T"] = pktalib.su
-0001e310: 7065 7274 7265 6e64 2872 6576 6572 7365  pertrend(reverse
-0001e320: 6444 6174 612c 2037 2c20 3329 5b22 5355  dData, 7, 3)["SU
-0001e330: 5045 5254 5f37 5f33 2e30 225d 0a20 2020  PERT_7_3.0"].   
-0001e340: 2020 2020 2072 6576 6572 7365 6444 6174       reversedDat
-0001e350: 615b 2245 4d41 3822 5d20 3d20 706b 7461  a["EMA8"] = pkta
-0001e360: 6c69 622e 454d 4128 7265 7665 7273 6564  lib.EMA(reversed
-0001e370: 4461 7461 5b22 436c 6f73 6522 5d2c 2074  Data["Close"], t
-0001e380: 696d 6570 6572 696f 643d 3929 0a20 2020  imeperiod=9).   
-0001e390: 2020 2020 2068 6967 6865 7243 6c6f 7365       higherClose
-0001e3a0: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
-0001e3b0: 2068 6967 6865 7243 6c6f 7365 0a20 2020   higherClose.   
-0001e3c0: 2020 2020 2020 2020 2061 6e64 2064 6179           and day
-0001e3d0: 305b 2243 6c6f 7365 225d 2e69 6c6f 635b  0["Close"].iloc[
-0001e3e0: 305d 203e 2072 6576 6572 7365 6444 6174  0] > reversedDat
-0001e3f0: 612e 7461 696c 2831 295b 2253 5550 4552  a.tail(1)["SUPER
-0001e400: 5422 5d2e 696c 6f63 5b30 5d0a 2020 2020  T"].iloc[0].    
-0001e410: 2020 2020 2020 2020 616e 6420 6461 7930          and day0
-0001e420: 5b22 436c 6f73 6522 5d2e 696c 6f63 5b30  ["Close"].iloc[0
-0001e430: 5d20 3e20 7265 7665 7273 6564 4461 7461  ] > reversedData
-0001e440: 2e74 6169 6c28 3129 5b22 454d 4138 225d  .tail(1)["EMA8"]
-0001e450: 2e69 6c6f 635b 305d 0a20 2020 2020 2020  .iloc[0].       
-0001e460: 2029 0a20 2020 2020 2020 2072 6574 7572   ).        retur
-0001e470: 6e20 6869 6768 6572 4869 6768 7320 616e  n higherHighs an
-0001e480: 6420 6869 6768 6572 4c6f 7773 2061 6e64  d higherLows and
-0001e490: 2068 6967 6865 7243 6c6f 7365 0a0a 2020   higherClose..  
-0001e4a0: 2020 2340 6d65 6173 7572 655f 7469 6d65    #@measure_time
-0001e4b0: 0a20 2020 2023 2056 616c 6964 6174 6520  .    # Validate 
-0001e4c0: 2749 6e73 6964 6520 4261 7227 2073 7472  'Inside Bar' str
-0001e4d0: 7563 7475 7265 2066 6f72 2072 6563 656e  ucture for recen
-0001e4e0: 7420 6461 7973 0a20 2020 2064 6566 2076  t days.    def v
-0001e4f0: 616c 6964 6174 6549 6e73 6964 6542 6172  alidateInsideBar
-0001e500: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
-0001e510: 6466 2c20 7363 7265 656e 4469 6374 2c20  df, screenDict, 
-0001e520: 7361 7665 4469 6374 2c20 6368 6172 7450  saveDict, chartP
-0001e530: 6174 7465 726e 3d31 2c20 6461 7973 546f  attern=1, daysTo
-0001e540: 4c6f 6f6b 6261 636b 3d35 0a20 2020 2029  Lookback=5.    )
-0001e550: 3a0a 2020 2020 2020 2020 6966 2064 6620  :.        if df 
-0001e560: 6973 204e 6f6e 6520 6f72 206c 656e 2864  is None or len(d
-0001e570: 6629 203d 3d20 303a 0a20 2020 2020 2020  f) == 0:.       
-0001e580: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-0001e590: 650a 2020 2020 2020 2020 6461 7461 203d  e.        data =
-0001e5a0: 2064 662e 636f 7079 2829 0a20 2020 2020   df.copy().     
-0001e5b0: 2020 206f 7267 4461 7461 203d 2064 6174     orgData = dat
-0001e5c0: 610a 2020 2020 2020 2020 7361 7665 6420  a.        saved 
-0001e5d0: 3d20 7365 6c66 2e66 696e 6443 7572 7265  = self.findCurre
-0001e5e0: 6e74 5361 7665 6456 616c 7565 2873 6372  ntSavedValue(scr
-0001e5f0: 6565 6e44 6963 742c 2073 6176 6544 6963  eenDict, saveDic
-0001e600: 742c 2022 5061 7474 6572 6e22 290a 2020  t, "Pattern").  
-0001e610: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
-0001e620: 616e 6765 2869 6e74 2864 6179 7354 6f4c  ange(int(daysToL
-0001e630: 6f6f 6b62 6163 6b29 2c20 696e 7428 726f  ookback), int(ro
-0001e640: 756e 6428 6461 7973 546f 4c6f 6f6b 6261  und(daysToLookba
-0001e650: 636b 202a 2030 2e35 2929 202d 2031 2c20  ck * 0.5)) - 1, 
-0001e660: 2d31 293a 0a20 2020 2020 2020 2020 2020  -1):.           
-0001e670: 2069 6620 6920 3d3d 2032 3a0a 2020 2020   if i == 2:.    
-0001e680: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0001e690: 726e 2030 2020 2320 4578 6974 2069 6620  rn 0  # Exit if 
-0001e6a0: 6f6e 6c79 206c 6173 7420 3220 6361 6e64  only last 2 cand
-0001e6b0: 6c65 7320 6172 6520 6c65 6674 0a20 2020  les are left.   
-0001e6c0: 2020 2020 2020 2020 2069 6620 6368 6172           if char
-0001e6d0: 7450 6174 7465 726e 203d 3d20 313a 0a20  tPattern == 1:. 
-0001e6e0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0001e6f0: 6620 2255 7022 2069 6e20 7361 7665 4469  f "Up" in saveDi
-0001e700: 6374 5b22 5472 656e 6422 5d20 616e 6420  ct["Trend"] and 
-0001e710: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0001e720: 2020 2020 2020 2242 756c 6c22 2069 6e20        "Bull" in 
-0001e730: 7361 7665 4469 6374 5b22 4d41 2d53 6967  saveDict["MA-Sig
-0001e740: 6e61 6c22 5d0a 2020 2020 2020 2020 2020  nal"].          
-0001e750: 2020 2020 2020 2020 2020 6f72 2022 5375            or "Su
-0001e760: 7070 6f72 7422 2069 6e20 7361 7665 4469  pport" in saveDi
-0001e770: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d0a  ct["MA-Signal"].
-0001e780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e790: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0001e7a0: 2020 2020 2020 2064 6174 6120 3d20 6f72         data = or
-0001e7b0: 6744 6174 612e 6865 6164 2869 290a 2020  gData.head(i).  
-0001e7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e7d0: 2020 7265 6643 616e 646c 6520 3d20 6461    refCandle = da
-0001e7e0: 7461 2e74 6169 6c28 3129 0a20 2020 2020  ta.tail(1).     
-0001e7f0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0001e800: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
-0001e810: 2020 2020 2020 2020 2020 2020 286c 656e              (len
-0001e820: 2864 6174 612e 4869 6768 5b64 6174 612e  (data.High[data.
-0001e830: 4869 6768 203e 2072 6566 4361 6e64 6c65  High > refCandle
-0001e840: 2e48 6967 682e 6974 656d 2829 5d29 203d  .High.item()]) =
-0001e850: 3d20 3029 0a20 2020 2020 2020 2020 2020  = 0).           
-0001e860: 2020 2020 2020 2020 2020 2020 2061 6e64               and
-0001e870: 2028 6c65 6e28 6461 7461 2e4c 6f77 5b64   (len(data.Low[d
-0001e880: 6174 612e 4c6f 7720 3c20 7265 6643 616e  ata.Low < refCan
-0001e890: 646c 652e 4c6f 772e 6974 656d 2829 5d29  dle.Low.item()])
-0001e8a0: 203d 3d20 3029 0a20 2020 2020 2020 2020   == 0).         
-0001e8b0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0001e8c0: 6e64 2028 6c65 6e28 6461 7461 2e4f 7065  nd (len(data.Ope
-0001e8d0: 6e5b 6461 7461 2e4f 7065 6e20 3e20 7265  n[data.Open > re
-0001e8e0: 6643 616e 646c 652e 4869 6768 2e69 7465  fCandle.High.ite
-0001e8f0: 6d28 295d 2920 3d3d 2030 290a 2020 2020  m()]) == 0).    
-0001e900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e910: 2020 2020 616e 6420 286c 656e 2864 6174      and (len(dat
-0001e920: 612e 436c 6f73 655b 6461 7461 2e43 6c6f  a.Close[data.Clo
-0001e930: 7365 203c 2072 6566 4361 6e64 6c65 2e4c  se < refCandle.L
-0001e940: 6f77 2e69 7465 6d28 295d 2920 3d3d 2030  ow.item()]) == 0
-0001e950: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001e960: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
-0001e970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e980: 2073 6372 6565 6e44 6963 745b 2250 6174   screenDict["Pat
-0001e990: 7465 726e 225d 203d 2028 0a20 2020 2020  tern"] = (.     
-0001e9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e9b0: 2020 2020 2020 2073 6176 6564 5b30 5d0a         saved[0].
-0001e9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e9d0: 2020 2020 2020 2020 2020 2020 2b20 636f              + co
-0001e9e0: 6c6f 7254 6578 742e 424f 4c44 0a20 2020  lorText.BOLD.   
-0001e9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ea00: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
-0001ea10: 5465 7874 2e57 4152 4e0a 2020 2020 2020  Text.WARN.      
+0001ac40: 2020 2020 2020 2020 205d 2c0a 2020 2020           ],.    
+0001ac50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ac60: 2020 2020 2020 2020 6178 6973 3d30 2c0a          axis=0,.
+0001ac70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ac80: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0001ac90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aca0: 2020 7265 7375 6c74 5f64 662e 7265 7365    result_df.rese
+0001acb0: 745f 696e 6465 7828 6472 6f70 3d54 7275  t_index(drop=Tru
+0001acc0: 652c 2069 6e70 6c61 6365 3d54 7275 6529  e, inplace=True)
+0001acd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001ace0: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
+0001acf0: 7074 696f 6e20 6173 2065 3a20 2023 2070  ption as e:  # p
+0001ad00: 7261 676d 613a 206e 6f20 636f 7665 720a  ragma: no cover.
+0001ad10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ad20: 2020 2020 2020 2020 7365 6c66 2e64 6566          self.def
+0001ad30: 6175 6c74 5f6c 6f67 6765 722e 6465 6275  ault_logger.debu
+0001ad40: 6728 652c 2065 7863 5f69 6e66 6f3d 5472  g(e, exc_info=Tr
+0001ad50: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
+0001ad60: 2020 2020 2020 2020 2020 2020 7061 7373              pass
+0001ad70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001ad80: 2020 2020 2023 2054 6865 6e20 7570 6461       # Then upda
+0001ad90: 7465 0a20 2020 2020 2020 2020 2020 2020  te.             
+0001ada0: 2020 2020 2020 206c 6173 745f 7369 676e         last_sign
+0001adb0: 616c 5b64 6174 615f 6c69 7374 5b63 6e74  al[data_list[cnt
+0001adc0: 5d5d 203d 205b 6669 6e61 6c5d 0a20 2020  ]] = [final].   
+0001add0: 2020 2020 2069 6620 7265 7375 6c74 5f64       if result_d
+0001ade0: 6620 6973 206e 6f74 204e 6f6e 653a 0a20  f is not None:. 
+0001adf0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0001ae00: 745f 6466 2e64 726f 705f 6475 706c 6963  t_df.drop_duplic
+0001ae10: 6174 6573 286b 6565 703d 226c 6173 7422  ates(keep="last"
+0001ae20: 2c20 696e 706c 6163 653d 5472 7565 290a  , inplace=True).
+0001ae30: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0001ae40: 6c74 5f64 662e 736f 7274 5f76 616c 7565  lt_df.sort_value
+0001ae50: 7328 6279 3d22 5469 6d65 222c 2069 6e70  s(by="Time", inp
+0001ae60: 6c61 6365 3d54 7275 6529 0a20 2020 2020  lace=True).     
+0001ae70: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+0001ae80: 5f64 665b 3a3a 2d31 5d0a 0a20 2020 2023  _df[::-1]..    #
+0001ae90: 2050 7265 7072 6f63 6573 7320 7468 6520   Preprocess the 
+0001aea0: 6163 7175 6972 6564 2064 6174 610a 2020  acquired data.  
+0001aeb0: 2020 6465 6620 7072 6570 726f 6365 7373    def preprocess
+0001aec0: 4461 7461 2873 656c 662c 2064 662c 2064  Data(self, df, d
+0001aed0: 6179 7354 6f4c 6f6f 6b62 6163 6b3d 4e6f  aysToLookback=No
+0001aee0: 6e65 293a 0a20 2020 2020 2020 2061 7373  ne):.        ass
+0001aef0: 6572 7420 6973 696e 7374 616e 6365 2864  ert isinstance(d
+0001af00: 662c 2070 642e 4461 7461 4672 616d 6529  f, pd.DataFrame)
+0001af10: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
+0001af20: 6466 2e63 6f70 7928 290a 2020 2020 2020  df.copy().      
+0001af30: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+0001af40: 2020 2064 6174 6120 3d20 6461 7461 2e72     data = data.r
+0001af50: 6570 6c61 6365 286e 702e 696e 662c 206e  eplace(np.inf, n
+0001af60: 702e 6e61 6e29 2e72 6570 6c61 6365 282d  p.nan).replace(-
+0001af70: 6e70 2e69 6e66 2c20 6e70 2e6e 616e 292e  np.inf, np.nan).
+0001af80: 6472 6f70 6e61 2868 6f77 3d22 616c 6c22  dropna(how="all"
+0001af90: 290a 2020 2020 2020 2020 2020 2020 2320  ).            # 
+0001afa0: 7365 6c66 2e64 6566 6175 6c74 5f6c 6f67  self.default_log
+0001afb0: 6765 722e 696e 666f 2866 2250 7265 7072  ger.info(f"Prepr
+0001afc0: 6f63 6573 7369 6e67 2064 6174 613a 5c6e  ocessing data:\n
+0001afd0: 7b64 6174 612e 6865 6164 2831 297d 5c6e  {data.head(1)}\n
+0001afe0: 2229 0a20 2020 2020 2020 2020 2020 2069  ").            i
+0001aff0: 6620 6461 7973 546f 4c6f 6f6b 6261 636b  f daysToLookback
+0001b000: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+0001b010: 2020 2020 2020 2020 2020 6461 7973 546f            daysTo
+0001b020: 4c6f 6f6b 6261 636b 203d 2073 656c 662e  Lookback = self.
+0001b030: 636f 6e66 6967 4d61 6e61 6765 722e 6461  configManager.da
+0001b040: 7973 546f 4c6f 6f6b 6261 636b 0a20 2020  ysToLookback.   
+0001b050: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+0001b060: 2e63 6f6e 6669 674d 616e 6167 6572 2e75  .configManager.u
+0001b070: 7365 454d 413a 0a20 2020 2020 2020 2020  seEMA:.         
+0001b080: 2020 2020 2020 2073 6d61 203d 2070 6b74         sma = pkt
+0001b090: 616c 6962 2e45 4d41 2864 6174 615b 2243  alib.EMA(data["C
+0001b0a0: 6c6f 7365 225d 2c20 7469 6d65 7065 7269  lose"], timeperi
+0001b0b0: 6f64 3d35 3029 0a20 2020 2020 2020 2020  od=50).         
+0001b0c0: 2020 2020 2020 206c 6d61 203d 2070 6b74         lma = pkt
+0001b0d0: 616c 6962 2e45 4d41 2864 6174 615b 2243  alib.EMA(data["C
+0001b0e0: 6c6f 7365 225d 2c20 7469 6d65 7065 7269  lose"], timeperi
+0001b0f0: 6f64 3d32 3030 290a 2020 2020 2020 2020  od=200).        
+0001b100: 2020 2020 2020 2020 7373 6d61 203d 2070          ssma = p
+0001b110: 6b74 616c 6962 2e45 4d41 2864 6174 615b  ktalib.EMA(data[
+0001b120: 2243 6c6f 7365 225d 2c20 7469 6d65 7065  "Close"], timepe
+0001b130: 7269 6f64 3d39 290a 2020 2020 2020 2020  riod=9).        
+0001b140: 2020 2020 2020 2020 7373 6d61 3230 203d          ssma20 =
+0001b150: 2070 6b74 616c 6962 2e45 4d41 2864 6174   pktalib.EMA(dat
+0001b160: 615b 2243 6c6f 7365 225d 2c20 7469 6d65  a["Close"], time
+0001b170: 7065 7269 6f64 3d32 3029 0a20 2020 2020  period=20).     
+0001b180: 2020 2020 2020 2020 2020 2064 6174 612e             data.
+0001b190: 696e 7365 7274 286c 656e 2864 6174 612e  insert(len(data.
+0001b1a0: 636f 6c75 6d6e 7329 2c20 2253 4d41 222c  columns), "SMA",
+0001b1b0: 2073 6d61 290a 2020 2020 2020 2020 2020   sma).          
+0001b1c0: 2020 2020 2020 6461 7461 2e69 6e73 6572        data.inser
+0001b1d0: 7428 6c65 6e28 6461 7461 2e63 6f6c 756d  t(len(data.colum
+0001b1e0: 6e73 292c 2022 4c4d 4122 2c20 6c6d 6129  ns), "LMA", lma)
+0001b1f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b200: 2064 6174 612e 696e 7365 7274 286c 656e   data.insert(len
+0001b210: 2864 6174 612e 636f 6c75 6d6e 7329 2c20  (data.columns), 
+0001b220: 2253 534d 4122 2c20 7373 6d61 290a 2020  "SSMA", ssma).  
+0001b230: 2020 2020 2020 2020 2020 2020 2020 6461                da
+0001b240: 7461 2e69 6e73 6572 7428 6c65 6e28 6461  ta.insert(len(da
+0001b250: 7461 2e63 6f6c 756d 6e73 292c 2022 5353  ta.columns), "SS
+0001b260: 4d41 3230 222c 2073 736d 6132 3029 0a20  MA20", ssma20). 
+0001b270: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0001b280: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b290: 2073 6d61 203d 2070 6b74 616c 6962 2e53   sma = pktalib.S
+0001b2a0: 4d41 2864 6174 615b 2243 6c6f 7365 225d  MA(data["Close"]
+0001b2b0: 2c20 7469 6d65 7065 7269 6f64 3d35 3029  , timeperiod=50)
+0001b2c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b2d0: 206c 6d61 203d 2070 6b74 616c 6962 2e53   lma = pktalib.S
+0001b2e0: 4d41 2864 6174 615b 2243 6c6f 7365 225d  MA(data["Close"]
+0001b2f0: 2c20 7469 6d65 7065 7269 6f64 3d32 3030  , timeperiod=200
+0001b300: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001b310: 2020 7373 6d61 203d 2070 6b74 616c 6962    ssma = pktalib
+0001b320: 2e53 4d41 2864 6174 615b 2243 6c6f 7365  .SMA(data["Close
+0001b330: 225d 2c20 7469 6d65 7065 7269 6f64 3d39  "], timeperiod=9
+0001b340: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001b350: 2020 7373 6d61 3230 203d 2070 6b74 616c    ssma20 = pktal
+0001b360: 6962 2e53 4d41 2864 6174 615b 2243 6c6f  ib.SMA(data["Clo
+0001b370: 7365 225d 2c20 7469 6d65 7065 7269 6f64  se"], timeperiod
+0001b380: 3d32 3029 0a20 2020 2020 2020 2020 2020  =20).           
+0001b390: 2020 2020 2064 6174 612e 696e 7365 7274       data.insert
+0001b3a0: 286c 656e 2864 6174 612e 636f 6c75 6d6e  (len(data.column
+0001b3b0: 7329 2c20 2253 4d41 222c 2073 6d61 290a  s), "SMA", sma).
+0001b3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b3d0: 6461 7461 2e69 6e73 6572 7428 6c65 6e28  data.insert(len(
+0001b3e0: 6461 7461 2e63 6f6c 756d 6e73 292c 2022  data.columns), "
+0001b3f0: 4c4d 4122 2c20 6c6d 6129 0a20 2020 2020  LMA", lma).     
+0001b400: 2020 2020 2020 2020 2020 2064 6174 612e             data.
+0001b410: 696e 7365 7274 286c 656e 2864 6174 612e  insert(len(data.
+0001b420: 636f 6c75 6d6e 7329 2c20 2253 534d 4122  columns), "SSMA"
+0001b430: 2c20 7373 6d61 290a 2020 2020 2020 2020  , ssma).        
+0001b440: 2020 2020 2020 2020 6461 7461 2e69 6e73          data.ins
+0001b450: 6572 7428 6c65 6e28 6461 7461 2e63 6f6c  ert(len(data.col
+0001b460: 756d 6e73 292c 2022 5353 4d41 3230 222c  umns), "SSMA20",
+0001b470: 2073 736d 6132 3029 0a20 2020 2020 2020   ssma20).       
+0001b480: 2020 2020 2076 6f6c 203d 2070 6b74 616c       vol = pktal
+0001b490: 6962 2e53 4d41 2864 6174 615b 2256 6f6c  ib.SMA(data["Vol
+0001b4a0: 756d 6522 5d2c 2074 696d 6570 6572 696f  ume"], timeperio
+0001b4b0: 643d 3230 290a 2020 2020 2020 2020 2020  d=20).          
+0001b4c0: 2020 7273 6920 3d20 706b 7461 6c69 622e    rsi = pktalib.
+0001b4d0: 5253 4928 6461 7461 5b22 436c 6f73 6522  RSI(data["Close"
+0001b4e0: 5d2c 2074 696d 6570 6572 696f 643d 3134  ], timeperiod=14
+0001b4f0: 290a 2020 2020 2020 2020 2020 2020 6461  ).            da
+0001b500: 7461 2e69 6e73 6572 7428 6c65 6e28 6461  ta.insert(len(da
+0001b510: 7461 2e63 6f6c 756d 6e73 292c 2022 566f  ta.columns), "Vo
+0001b520: 6c4d 4122 2c20 766f 6c29 0a20 2020 2020  lMA", vol).     
+0001b530: 2020 2020 2020 2064 6174 612e 696e 7365         data.inse
+0001b540: 7274 286c 656e 2864 6174 612e 636f 6c75  rt(len(data.colu
+0001b550: 6d6e 7329 2c20 2252 5349 222c 2072 7369  mns), "RSI", rsi
+0001b560: 290a 2020 2020 2020 2020 2020 2020 6363  ).            cc
+0001b570: 6920 3d20 706b 7461 6c69 622e 4343 4928  i = pktalib.CCI(
+0001b580: 6461 7461 5b22 4869 6768 225d 2c20 6461  data["High"], da
+0001b590: 7461 5b22 4c6f 7722 5d2c 2064 6174 615b  ta["Low"], data[
+0001b5a0: 2243 6c6f 7365 225d 2c20 7469 6d65 7065  "Close"], timepe
+0001b5b0: 7269 6f64 3d31 3429 0a20 2020 2020 2020  riod=14).       
+0001b5c0: 2020 2020 2064 6174 612e 696e 7365 7274       data.insert
+0001b5d0: 286c 656e 2864 6174 612e 636f 6c75 6d6e  (len(data.column
+0001b5e0: 7329 2c20 2243 4349 222c 2063 6369 290a  s), "CCI", cci).
+0001b5f0: 2020 2020 2020 2020 2020 2020 7472 793a              try:
+0001b600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b610: 2066 6173 746b 2c20 6661 7374 6420 3d20   fastk, fastd = 
+0001b620: 706b 7461 6c69 622e 5354 4f43 4852 5349  pktalib.STOCHRSI
+0001b630: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0001b640: 2020 2020 2020 6461 7461 5b22 436c 6f73        data["Clos
+0001b650: 6522 5d2c 2074 696d 6570 6572 696f 643d  e"], timeperiod=
+0001b660: 3134 2c20 6661 7374 6b5f 7065 7269 6f64  14, fastk_period
+0001b670: 3d35 2c20 6661 7374 645f 7065 7269 6f64  =5, fastd_period
+0001b680: 3d33 2c20 6661 7374 645f 6d61 7479 7065  =3, fastd_matype
+0001b690: 3d30 0a20 2020 2020 2020 2020 2020 2020  =0.             
+0001b6a0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+0001b6b0: 2020 2020 2064 6174 612e 696e 7365 7274       data.insert
+0001b6c0: 286c 656e 2864 6174 612e 636f 6c75 6d6e  (len(data.column
+0001b6d0: 7329 2c20 2246 4153 544b 222c 2066 6173  s), "FASTK", fas
+0001b6e0: 746b 290a 2020 2020 2020 2020 2020 2020  tk).            
+0001b6f0: 2020 2020 6461 7461 2e69 6e73 6572 7428      data.insert(
+0001b700: 6c65 6e28 6461 7461 2e63 6f6c 756d 6e73  len(data.columns
+0001b710: 292c 2022 4641 5354 4422 2c20 6661 7374  ), "FASTD", fast
+0001b720: 6429 0a20 2020 2020 2020 2020 2020 2065  d).            e
+0001b730: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
+0001b740: 6173 2065 3a0a 2020 2020 2020 2020 2020  as e:.          
+0001b750: 2020 2020 2020 7365 6c66 2e64 6566 6175        self.defau
+0001b760: 6c74 5f6c 6f67 6765 722e 6465 6275 6728  lt_logger.debug(
+0001b770: 652c 2065 7863 5f69 6e66 6f3d 5472 7565  e, exc_info=True
+0001b780: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001b790: 2020 7061 7373 0a20 2020 2020 2020 2065    pass.        e
+0001b7a0: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
+0001b7b0: 6173 2065 3a0a 2020 2020 2020 2020 2020  as e:.          
+0001b7c0: 2020 2020 2020 7365 6c66 2e64 6566 6175        self.defau
+0001b7d0: 6c74 5f6c 6f67 6765 722e 6465 6275 6728  lt_logger.debug(
+0001b7e0: 652c 2065 7863 5f69 6e66 6f3d 5472 7565  e, exc_info=True
+0001b7f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001b800: 2020 7061 7373 0a20 2020 2020 2020 2064    pass.        d
+0001b810: 6174 6120 3d20 6461 7461 5b3a 3a2d 315d  ata = data[::-1]
+0001b820: 2020 2320 5265 7665 7273 6520 7468 6520    # Reverse the 
+0001b830: 6461 7461 6672 616d 650a 2020 2020 2020  dataframe.      
+0001b840: 2020 2320 6461 7461 203d 2064 6174 612e    # data = data.
+0001b850: 6669 6c6c 6e61 2830 290a 2020 2020 2020  fillna(0).      
+0001b860: 2020 2320 6461 7461 203d 2064 6174 612e    # data = data.
+0001b870: 7265 706c 6163 6528 5b6e 702e 696e 662c  replace([np.inf,
+0001b880: 202d 6e70 2e69 6e66 5d2c 2030 290a 2020   -np.inf], 0).  
+0001b890: 2020 2020 2020 6675 6c6c 4461 7461 203d        fullData =
+0001b8a0: 2064 6174 610a 2020 2020 2020 2020 7472   data.        tr
+0001b8b0: 696d 6d65 6444 6174 6120 3d20 6461 7461  immedData = data
+0001b8c0: 2e68 6561 6428 6461 7973 546f 4c6f 6f6b  .head(daysToLook
+0001b8d0: 6261 636b 290a 2020 2020 2020 2020 7265  back).        re
+0001b8e0: 7475 726e 2028 6675 6c6c 4461 7461 2c20  turn (fullData, 
+0001b8f0: 7472 696d 6d65 6444 6174 6129 0a0a 2020  trimmedData)..  
+0001b900: 2020 2320 5661 6c69 6461 7465 2069 6620    # Validate if 
+0001b910: 7468 6520 7374 6f63 6b20 6973 2062 756c  the stock is bul
+0001b920: 6c69 7368 2069 6e20 7468 6520 7368 6f72  lish in the shor
+0001b930: 7420 7465 726d 0a20 2020 2064 6566 2076  t term.    def v
+0001b940: 616c 6964 6174 6531 354d 696e 7574 6550  alidate15MinuteP
+0001b950: 7269 6365 566f 6c75 6d65 4272 6561 6b6f  riceVolumeBreako
+0001b960: 7574 2873 656c 662c 2064 6629 3a0a 2020  ut(self, df):.  
+0001b970: 2020 2020 2020 6966 2064 6620 6973 204e        if df is N
+0001b980: 6f6e 6520 6f72 206c 656e 2864 6629 203d  one or len(df) =
+0001b990: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
+0001b9a0: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
+0001b9b0: 2020 2020 2020 2320 6874 7470 733a 2f2f        # https://
+0001b9c0: 6368 6172 7469 6e6b 2e63 6f6d 2f73 6372  chartink.com/scr
+0001b9d0: 6565 6e65 722f 3135 2d6d 696e 2d70 7269  eener/15-min-pri
+0001b9e0: 6365 2d76 6f6c 756d 652d 6272 6561 6b6f  ce-volume-breako
+0001b9f0: 7574 0a20 2020 2020 2020 2064 6174 6120  ut.        data 
+0001ba00: 3d20 6466 2e63 6f70 7928 290a 2020 2020  = df.copy().    
+0001ba10: 2020 2020 6461 7461 203d 2064 6174 612e      data = data.
+0001ba20: 6669 6c6c 6e61 2830 290a 2020 2020 2020  fillna(0).      
+0001ba30: 2020 6461 7461 203d 2064 6174 612e 7265    data = data.re
+0001ba40: 706c 6163 6528 5b6e 702e 696e 662c 202d  place([np.inf, -
+0001ba50: 6e70 2e69 6e66 5d2c 2030 290a 2020 2020  np.inf], 0).    
+0001ba60: 2020 2020 6461 7461 203d 2064 6174 615b      data = data[
+0001ba70: 3a3a 2d31 5d20 2023 2052 6576 6572 7365  ::-1]  # Reverse
+0001ba80: 2074 6865 2064 6174 6166 7261 6d65 2073   the dataframe s
+0001ba90: 6f20 7468 6174 2069 7473 2074 6865 206f  o that its the o
+0001baa0: 6c64 6573 7420 6461 7465 2066 6972 7374  ldest date first
+0001bab0: 0a20 2020 2020 2020 2064 6174 615b 2253  .        data["S
+0001bac0: 4d41 3230 225d 203d 2070 6b74 616c 6962  MA20"] = pktalib
+0001bad0: 2e53 4d41 2864 6174 615b 2243 6c6f 7365  .SMA(data["Close
+0001bae0: 225d 2c20 3230 290a 2020 2020 2020 2020  "], 20).        
+0001baf0: 6461 7461 5b22 534d 4132 3056 225d 203d  data["SMA20V"] =
+0001bb00: 2070 6b74 616c 6962 2e53 4d41 2864 6174   pktalib.SMA(dat
+0001bb10: 615b 2256 6f6c 756d 6522 5d2c 2032 3029  a["Volume"], 20)
+0001bb20: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
+0001bb30: 6461 7461 5b0a 2020 2020 2020 2020 2020  data[.          
+0001bb40: 2020 3a3a 2d31 0a20 2020 2020 2020 205d    ::-1.        ]
+0001bb50: 2020 2320 5265 7665 7273 6520 7468 6520    # Reverse the 
+0001bb60: 6461 7461 6672 616d 6520 736f 2074 6861  dataframe so tha
+0001bb70: 7420 6974 2773 2074 6865 206d 6f73 7420  t it's the most 
+0001bb80: 7265 6365 6e74 2064 6174 6520 6669 7273  recent date firs
+0001bb90: 740a 2020 2020 2020 2020 7265 6365 6e74  t.        recent
+0001bba0: 203d 2064 6174 612e 6865 6164 2833 290a   = data.head(3).
+0001bbb0: 2020 2020 2020 2020 6966 206c 656e 2872          if len(r
+0001bbc0: 6563 656e 7429 203c 2033 3a0a 2020 2020  ecent) < 3:.    
+0001bbd0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+0001bbe0: 616c 7365 0a20 2020 2020 2020 2063 6f6e  alse.        con
+0001bbf0: 6431 203d 2072 6563 656e 745b 2243 6c6f  d1 = recent["Clo
+0001bc00: 7365 225d 2e69 6c6f 635b 305d 203e 2072  se"].iloc[0] > r
+0001bc10: 6563 656e 745b 2243 6c6f 7365 225d 2e69  ecent["Close"].i
+0001bc20: 6c6f 635b 315d 0a20 2020 2020 2020 2063  loc[1].        c
+0001bc30: 6f6e 6432 203d 2063 6f6e 6431 2061 6e64  ond2 = cond1 and
+0001bc40: 2028 7265 6365 6e74 5b22 436c 6f73 6522   (recent["Close"
+0001bc50: 5d2e 696c 6f63 5b30 5d20 3e20 7265 6365  ].iloc[0] > rece
+0001bc60: 6e74 5b22 534d 4132 3022 5d2e 696c 6f63  nt["SMA20"].iloc
+0001bc70: 5b30 5d29 0a20 2020 2020 2020 2063 6f6e  [0]).        con
+0001bc80: 6433 203d 2063 6f6e 6432 2061 6e64 2028  d3 = cond2 and (
+0001bc90: 7265 6365 6e74 5b22 436c 6f73 6522 5d2e  recent["Close"].
+0001bca0: 696c 6f63 5b31 5d20 3e20 7265 6365 6e74  iloc[1] > recent
+0001bcb0: 5b22 4869 6768 225d 2e69 6c6f 635b 325d  ["High"].iloc[2]
+0001bcc0: 290a 2020 2020 2020 2020 636f 6e64 3420  ).        cond4 
+0001bcd0: 3d20 636f 6e64 3320 616e 6420 2872 6563  = cond3 and (rec
+0001bce0: 656e 745b 2256 6f6c 756d 6522 5d2e 696c  ent["Volume"].il
+0001bcf0: 6f63 5b30 5d20 3e20 7265 6365 6e74 5b22  oc[0] > recent["
+0001bd00: 534d 4132 3056 225d 2e69 6c6f 635b 305d  SMA20V"].iloc[0]
+0001bd10: 290a 2020 2020 2020 2020 636f 6e64 3520  ).        cond5 
+0001bd20: 3d20 636f 6e64 3420 616e 6420 2872 6563  = cond4 and (rec
+0001bd30: 656e 745b 2256 6f6c 756d 6522 5d2e 696c  ent["Volume"].il
+0001bd40: 6f63 5b31 5d20 3e20 7265 6365 6e74 5b22  oc[1] > recent["
+0001bd50: 534d 4132 3056 225d 2e69 6c6f 635b 305d  SMA20V"].iloc[0]
+0001bd60: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0001bd70: 2063 6f6e 6435 0a0a 2020 2020 6465 6620   cond5..    def 
+0001bd80: 7661 6c69 6461 7465 4275 6c6c 6973 6846  validateBullishF
+0001bd90: 6f72 546f 6d6f 7272 6f77 2873 656c 662c  orTomorrow(self,
+0001bda0: 2064 6629 3a0a 2020 2020 2020 2020 6966   df):.        if
+0001bdb0: 2064 6620 6973 204e 6f6e 6520 6f72 206c   df is None or l
+0001bdc0: 656e 2864 6629 203d 3d20 303a 0a20 2020  en(df) == 0:.   
+0001bdd0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0001bde0: 4661 6c73 650a 2020 2020 2020 2020 6461  False.        da
+0001bdf0: 7461 203d 2064 662e 636f 7079 2829 0a20  ta = df.copy(). 
+0001be00: 2020 2020 2020 2023 2068 7474 7073 3a2f         # https:/
+0001be10: 2f63 6861 7274 696e 6b2e 636f 6d2f 7363  /chartink.com/sc
+0001be20: 7265 656e 6572 2f62 756c 6c69 7368 2d66  reener/bullish-f
+0001be30: 6f72 2d74 6f6d 6f72 726f 770a 2020 2020  or-tomorrow.    
+0001be40: 2020 2020 6461 7461 203d 2064 6174 612e      data = data.
+0001be50: 6669 6c6c 6e61 2830 290a 2020 2020 2020  fillna(0).      
+0001be60: 2020 6461 7461 203d 2064 6174 612e 7265    data = data.re
+0001be70: 706c 6163 6528 5b6e 702e 696e 662c 202d  place([np.inf, -
+0001be80: 6e70 2e69 6e66 5d2c 2030 290a 2020 2020  np.inf], 0).    
+0001be90: 2020 2020 6461 7461 203d 2064 6174 615b      data = data[
+0001bea0: 3a3a 2d31 5d20 2023 2052 6576 6572 7365  ::-1]  # Reverse
+0001beb0: 2074 6865 2064 6174 6166 7261 6d65 2073   the dataframe s
+0001bec0: 6f20 7468 6174 2069 7473 2074 6865 206f  o that its the o
+0001bed0: 6c64 6573 7420 6461 7465 2066 6972 7374  ldest date first
+0001bee0: 0a20 2020 2020 2020 206d 6163 644c 696e  .        macdLin
+0001bef0: 6520 3d20 706b 7461 6c69 622e 4d41 4344  e = pktalib.MACD
+0001bf00: 2864 6174 615b 2243 6c6f 7365 225d 2c20  (data["Close"], 
+0001bf10: 3132 2c20 3236 2c20 3929 5b30 5d2e 7461  12, 26, 9)[0].ta
+0001bf20: 696c 2833 290a 2020 2020 2020 2020 6d61  il(3).        ma
+0001bf30: 6364 5369 676e 616c 203d 2070 6b74 616c  cdSignal = pktal
+0001bf40: 6962 2e4d 4143 4428 6461 7461 5b22 436c  ib.MACD(data["Cl
+0001bf50: 6f73 6522 5d2c 2031 322c 2032 362c 2039  ose"], 12, 26, 9
+0001bf60: 295b 315d 2e74 6169 6c28 3329 0a20 2020  )[1].tail(3).   
+0001bf70: 2020 2020 206d 6163 6448 6973 7420 3d20       macdHist = 
+0001bf80: 706b 7461 6c69 622e 4d41 4344 2864 6174  pktalib.MACD(dat
+0001bf90: 615b 2243 6c6f 7365 225d 2c20 3132 2c20  a["Close"], 12, 
+0001bfa0: 3236 2c20 3929 5b32 5d2e 7461 696c 2833  26, 9)[2].tail(3
+0001bfb0: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+0001bfc0: 6e20 280a 2020 2020 2020 2020 2020 2020  n (.            
+0001bfd0: 286d 6163 6448 6973 742e 696c 6f63 5b3a  (macdHist.iloc[:
+0001bfe0: 315d 2e69 6c6f 635b 305d 203c 206d 6163  1].iloc[0] < mac
+0001bff0: 6448 6973 742e 696c 6f63 5b3a 325d 2e69  dHist.iloc[:2].i
+0001c000: 6c6f 635b 315d 290a 2020 2020 2020 2020  loc[1]).        
+0001c010: 2020 2020 616e 6420 286d 6163 6448 6973      and (macdHis
+0001c020: 742e 696c 6f63 5b3a 335d 2e69 6c6f 635b  t.iloc[:3].iloc[
+0001c030: 325d 203e 206d 6163 6448 6973 742e 696c  2] > macdHist.il
+0001c040: 6f63 5b3a 325d 2e69 6c6f 635b 315d 290a  oc[:2].iloc[1]).
+0001c050: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+0001c060: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0001c070: 2020 286d 6163 644c 696e 652e 696c 6f63    (macdLine.iloc
+0001c080: 5b3a 335d 2e69 6c6f 635b 325d 202d 206d  [:3].iloc[2] - m
+0001c090: 6163 6453 6967 6e61 6c2e 696c 6f63 5b3a  acdSignal.iloc[:
+0001c0a0: 335d 2e69 6c6f 635b 325d 290a 2020 2020  3].iloc[2]).    
+0001c0b0: 2020 2020 2020 2020 2020 2020 2d20 286d              - (m
+0001c0c0: 6163 644c 696e 652e 696c 6f63 5b3a 325d  acdLine.iloc[:2]
+0001c0d0: 2e69 6c6f 635b 315d 202d 206d 6163 6453  .iloc[1] - macdS
+0001c0e0: 6967 6e61 6c2e 696c 6f63 5b3a 325d 2e69  ignal.iloc[:2].i
+0001c0f0: 6c6f 635b 315d 290a 2020 2020 2020 2020  loc[1]).        
+0001c100: 2020 2020 2020 2020 3e3d 2030 2e34 0a20          >= 0.4. 
+0001c110: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0001c120: 2020 2020 2020 2020 2061 6e64 2028 0a20           and (. 
+0001c130: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+0001c140: 6d61 6364 4c69 6e65 2e69 6c6f 635b 3a32  macdLine.iloc[:2
+0001c150: 5d2e 696c 6f63 5b31 5d20 2d20 6d61 6364  ].iloc[1] - macd
+0001c160: 5369 676e 616c 2e69 6c6f 635b 3a32 5d2e  Signal.iloc[:2].
+0001c170: 696c 6f63 5b31 5d29 0a20 2020 2020 2020  iloc[1]).       
+0001c180: 2020 2020 2020 2020 202d 2028 6d61 6364           - (macd
+0001c190: 4c69 6e65 2e69 6c6f 635b 3a31 5d2e 696c  Line.iloc[:1].il
+0001c1a0: 6f63 5b30 5d20 2d20 6d61 6364 5369 676e  oc[0] - macdSign
+0001c1b0: 616c 2e69 6c6f 635b 3a31 5d2e 696c 6f63  al.iloc[:1].iloc
+0001c1c0: 5b30 5d29 0a20 2020 2020 2020 2020 2020  [0]).           
+0001c1d0: 2020 2020 203c 3d20 302e 320a 2020 2020       <= 0.2.    
+0001c1e0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0001c1f0: 2020 2020 2020 616e 6420 286d 6163 644c        and (macdL
+0001c200: 696e 652e 696c 6f63 5b3a 335d 2e69 6c6f  ine.iloc[:3].ilo
+0001c210: 635b 325d 203e 206d 6163 6453 6967 6e61  c[2] > macdSigna
+0001c220: 6c2e 696c 6f63 5b3a 335d 2e69 6c6f 635b  l.iloc[:3].iloc[
+0001c230: 325d 290a 2020 2020 2020 2020 2020 2020  2]).            
+0001c240: 616e 6420 280a 2020 2020 2020 2020 2020  and (.          
+0001c250: 2020 2020 2020 286d 6163 644c 696e 652e        (macdLine.
+0001c260: 696c 6f63 5b3a 335d 2e69 6c6f 635b 325d  iloc[:3].iloc[2]
+0001c270: 202d 206d 6163 6453 6967 6e61 6c2e 696c   - macdSignal.il
+0001c280: 6f63 5b3a 335d 2e69 6c6f 635b 325d 290a  oc[:3].iloc[2]).
+0001c290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c2a0: 2d20 286d 6163 644c 696e 652e 696c 6f63  - (macdLine.iloc
+0001c2b0: 5b3a 325d 2e69 6c6f 635b 315d 202d 206d  [:2].iloc[1] - m
+0001c2c0: 6163 6453 6967 6e61 6c2e 696c 6f63 5b3a  acdSignal.iloc[:
+0001c2d0: 325d 2e69 6c6f 635b 315d 290a 2020 2020  2].iloc[1]).    
+0001c2e0: 2020 2020 2020 2020 2020 2020 3c20 310a              < 1.
+0001c2f0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0001c300: 2020 2020 2020 290a 0a20 2020 2023 406d        )..    #@m
+0001c310: 6561 7375 7265 5f74 696d 650a 2020 2020  easure_time.    
+0001c320: 2320 7661 6c69 6461 7465 2069 6620 4343  # validate if CC
+0001c330: 4920 6973 2077 6974 6869 6e20 6769 7665  I is within give
+0001c340: 6e20 7261 6e67 650a 2020 2020 6465 6620  n range.    def 
+0001c350: 7661 6c69 6461 7465 4343 4928 7365 6c66  validateCCI(self
+0001c360: 2c20 6466 2c20 7363 7265 656e 4469 6374  , df, screenDict
+0001c370: 2c20 7361 7665 4469 6374 2c20 6d69 6e43  , saveDict, minC
+0001c380: 4349 2c20 6d61 7843 4349 293a 0a20 2020  CI, maxCCI):.   
+0001c390: 2020 2020 2069 6620 6466 2069 7320 4e6f       if df is No
+0001c3a0: 6e65 206f 7220 6c65 6e28 6466 2920 3d3d  ne or len(df) ==
+0001c3b0: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+0001c3c0: 7265 7475 726e 2046 616c 7365 0a20 2020  return False.   
+0001c3d0: 2020 2020 2064 6174 6120 3d20 6466 2e63       data = df.c
+0001c3e0: 6f70 7928 290a 2020 2020 2020 2020 6461  opy().        da
+0001c3f0: 7461 203d 2064 6174 612e 6669 6c6c 6e61  ta = data.fillna
+0001c400: 2830 290a 2020 2020 2020 2020 6461 7461  (0).        data
+0001c410: 203d 2064 6174 612e 7265 706c 6163 6528   = data.replace(
+0001c420: 5b6e 702e 696e 662c 202d 6e70 2e69 6e66  [np.inf, -np.inf
+0001c430: 5d2c 2030 290a 2020 2020 2020 2020 6363  ], 0).        cc
+0001c440: 6920 3d20 696e 7428 6461 7461 2e68 6561  i = int(data.hea
+0001c450: 6428 3129 5b22 4343 4922 5d2e 696c 6f63  d(1)["CCI"].iloc
+0001c460: 5b30 5d29 0a20 2020 2020 2020 2073 6176  [0]).        sav
+0001c470: 6544 6963 745b 2243 4349 225d 203d 2063  eDict["CCI"] = c
+0001c480: 6369 0a20 2020 2020 2020 2069 6620 2863  ci.        if (c
+0001c490: 6369 203e 3d20 6d69 6e43 4349 2061 6e64  ci >= minCCI and
+0001c4a0: 2063 6369 203c 3d20 6d61 7843 4349 293a   cci <= maxCCI):
+0001c4b0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0001c4c0: 2822 5570 2220 696e 2073 6176 6544 6963  ("Up" in saveDic
+0001c4d0: 745b 2254 7265 6e64 225d 293a 0a20 2020  t["Trend"]):.   
+0001c4e0: 2020 2020 2020 2020 2020 2020 2073 6372               scr
+0001c4f0: 6565 6e44 6963 745b 2243 4349 225d 203d  eenDict["CCI"] =
+0001c500: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+0001c510: 2020 2020 2020 2028 636f 6c6f 7254 6578         (colorTex
+0001c520: 742e 424f 4c44 2069 6620 2822 5374 726f  t.BOLD if ("Stro
+0001c530: 6e67 2220 696e 2073 6176 6544 6963 745b  ng" in saveDict[
+0001c540: 2254 7265 6e64 225d 2920 656c 7365 2022  "Trend"]) else "
+0001c550: 2229 202b 2063 6f6c 6f72 5465 7874 2e47  ") + colorText.G
+0001c560: 5245 454e 202b 2073 7472 2863 6369 2920  REEN + str(cci) 
+0001c570: 2b20 636f 6c6f 7254 6578 742e 454e 440a  + colorText.END.
+0001c580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c590: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+0001c5a0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0001c5b0: 2020 2020 7363 7265 656e 4469 6374 5b22      screenDict["
+0001c5c0: 4343 4922 5d20 3d20 280a 2020 2020 2020  CCI"] = (.      
+0001c5d0: 2020 2020 2020 2020 2020 2020 2020 2863                (c
+0001c5e0: 6f6c 6f72 5465 7874 2e42 4f4c 4420 6966  olorText.BOLD if
+0001c5f0: 2028 2253 7472 6f6e 6722 2069 6e20 7361   ("Strong" in sa
+0001c600: 7665 4469 6374 5b22 5472 656e 6422 5d29  veDict["Trend"])
+0001c610: 2065 6c73 6520 2222 2920 2b20 636f 6c6f   else "") + colo
+0001c620: 7254 6578 742e 4641 494c 202b 2073 7472  rText.FAIL + str
+0001c630: 2863 6369 2920 2b20 636f 6c6f 7254 6578  (cci) + colorTex
+0001c640: 742e 454e 440a 2020 2020 2020 2020 2020  t.END.          
+0001c650: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0001c660: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+0001c670: 2020 2020 2020 2020 7363 7265 656e 4469          screenDi
+0001c680: 6374 5b22 4343 4922 5d20 3d20 636f 6c6f  ct["CCI"] = colo
+0001c690: 7254 6578 742e 424f 4c44 202b 2063 6f6c  rText.BOLD + col
+0001c6a0: 6f72 5465 7874 2e46 4149 4c20 2b20 7374  orText.FAIL + st
+0001c6b0: 7228 6363 6929 202b 2063 6f6c 6f72 5465  r(cci) + colorTe
+0001c6c0: 7874 2e45 4e44 0a20 2020 2020 2020 2072  xt.END.        r
+0001c6d0: 6574 7572 6e20 4661 6c73 650a 0a20 2020  eturn False..   
+0001c6e0: 2023 2046 696e 6420 436f 6e66 6c75 6365   # Find Confluce
+0001c6f0: 6e63 650a 2020 2020 6465 6620 7661 6c69  nce.    def vali
+0001c700: 6461 7465 436f 6e66 6c75 656e 6365 2873  dateConfluence(s
+0001c710: 656c 662c 2073 746f 636b 2c20 6466 2c20  elf, stock, df, 
+0001c720: 7363 7265 656e 4469 6374 2c20 7361 7665  screenDict, save
+0001c730: 4469 6374 2c20 7065 7263 656e 7461 6765  Dict, percentage
+0001c740: 3d30 2e31 2c63 6f6e 6646 696c 7465 723d  =0.1,confFilter=
+0001c750: 3329 3a0a 2020 2020 2020 2020 6966 2064  3):.        if d
+0001c760: 6620 6973 204e 6f6e 6520 6f72 206c 656e  f is None or len
+0001c770: 2864 6629 203d 3d20 303a 0a20 2020 2020  (df) == 0:.     
+0001c780: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+0001c790: 6c73 650a 2020 2020 2020 2020 6461 7461  lse.        data
+0001c7a0: 203d 2064 662e 636f 7079 2829 0a20 2020   = df.copy().   
+0001c7b0: 2020 2020 2072 6563 656e 7420 3d20 6461       recent = da
+0001c7c0: 7461 2e68 6561 6428 3229 0a20 2020 2020  ta.head(2).     
+0001c7d0: 2020 2069 6620 6c65 6e28 7265 6365 6e74     if len(recent
+0001c7e0: 2920 3c20 323a 0a20 2020 2020 2020 2020  ) < 2:.         
+0001c7f0: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+0001c800: 2020 2020 2020 2020 6b65 7931 203d 2022          key1 = "
+0001c810: 534d 4122 0a20 2020 2020 2020 206b 6579  SMA".        key
+0001c820: 3220 3d20 224c 4d41 220a 2020 2020 2020  2 = "LMA".      
+0001c830: 2020 6b65 7933 203d 2022 3530 444d 4122    key3 = "50DMA"
+0001c840: 0a20 2020 2020 2020 206b 6579 3420 3d20  .        key4 = 
+0001c850: 2232 3030 444d 4122 0a20 2020 2020 2020  "200DMA".       
+0001c860: 2069 7332 3044 4d41 4372 6f73 736f 7665   is20DMACrossove
+0001c870: 7235 3044 4d41 203d 2028 7265 6365 6e74  r50DMA = (recent
+0001c880: 5b22 5353 4d41 3230 225d 2e69 6c6f 635b  ["SSMA20"].iloc[
+0001c890: 305d 203e 3d20 7265 6365 6e74 5b22 534d  0] >= recent["SM
+0001c8a0: 4122 5d2e 696c 6f63 5b30 5d29 2061 6e64  A"].iloc[0]) and
+0001c8b0: 205c 0a20 2020 2020 2020 2020 2020 2020   \.             
+0001c8c0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+0001c8d0: 7265 6365 6e74 5b22 5353 4d41 3230 225d  recent["SSMA20"]
+0001c8e0: 2e69 6c6f 635b 315d 203c 3d20 7265 6365  .iloc[1] <= rece
+0001c8f0: 6e74 5b22 534d 4122 5d2e 696c 6f63 5b31  nt["SMA"].iloc[1
+0001c900: 5d29 0a20 2020 2020 2020 2069 7335 3044  ]).        is50D
+0001c910: 4d41 4372 6f73 736f 7665 7232 3030 444d  MACrossover200DM
+0001c920: 4120 3d20 2872 6563 656e 745b 2253 4d41  A = (recent["SMA
+0001c930: 225d 2e69 6c6f 635b 305d 203e 3d20 7265  "].iloc[0] >= re
+0001c940: 6365 6e74 5b22 4c4d 4122 5d2e 696c 6f63  cent["LMA"].iloc
+0001c950: 5b30 5d29 2061 6e64 205c 0a20 2020 2020  [0]) and \.     
+0001c960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c970: 2020 2020 2020 2028 7265 6365 6e74 5b22         (recent["
+0001c980: 534d 4122 5d2e 696c 6f63 5b31 5d20 3c3d  SMA"].iloc[1] <=
+0001c990: 2072 6563 656e 745b 224c 4d41 225d 2e69   recent["LMA"].i
+0001c9a0: 6c6f 635b 315d 290a 2020 2020 2020 2020  loc[1]).        
+0001c9b0: 6973 476f 6c64 656e 4372 6f73 734f 7665  isGoldenCrossOve
+0001c9c0: 7220 3d20 6973 3230 444d 4143 726f 7373  r = is20DMACross
+0001c9d0: 6f76 6572 3530 444d 4120 6f72 2069 7335  over50DMA or is5
+0001c9e0: 3044 4d41 4372 6f73 736f 7665 7232 3030  0DMACrossover200
+0001c9f0: 444d 410a 2020 2020 2020 2020 6973 3530  DMA.        is50
+0001ca00: 444d 4143 726f 7373 6f76 6572 3230 3044  DMACrossover200D
+0001ca10: 4d41 446f 776e 203d 2028 7265 6365 6e74  MADown = (recent
+0001ca20: 5b22 534d 4122 5d2e 696c 6f63 5b30 5d20  ["SMA"].iloc[0] 
+0001ca30: 3c3d 2072 6563 656e 745b 224c 4d41 225d  <= recent["LMA"]
+0001ca40: 2e69 6c6f 635b 305d 2920 616e 6420 5c0a  .iloc[0]) and \.
+0001ca50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ca60: 2020 2020 2020 2020 2020 2020 2872 6563              (rec
+0001ca70: 656e 745b 2253 4d41 225d 2e69 6c6f 635b  ent["SMA"].iloc[
+0001ca80: 315d 203e 3d20 7265 6365 6e74 5b22 4c4d  1] >= recent["LM
+0001ca90: 4122 5d2e 696c 6f63 5b31 5d29 0a20 2020  A"].iloc[1]).   
+0001caa0: 2020 2020 2069 7332 3044 4d41 4372 6f73       is20DMACros
+0001cab0: 736f 7665 7235 3044 4d41 446f 776e 203d  sover50DMADown =
+0001cac0: 2028 7265 6365 6e74 5b22 5353 4d41 3230   (recent["SSMA20
+0001cad0: 225d 2e69 6c6f 635b 305d 203c 3d20 7265  "].iloc[0] <= re
+0001cae0: 6365 6e74 5b22 534d 4122 5d2e 696c 6f63  cent["SMA"].iloc
+0001caf0: 5b30 5d29 2061 6e64 205c 0a20 2020 2020  [0]) and \.     
+0001cb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cb10: 2020 2020 2020 2028 7265 6365 6e74 5b22         (recent["
+0001cb20: 5353 4d41 3230 225d 2e69 6c6f 635b 315d  SSMA20"].iloc[1]
+0001cb30: 203e 3d20 7265 6365 6e74 5b22 534d 4122   >= recent["SMA"
+0001cb40: 5d2e 696c 6f63 5b31 5d29 0a20 2020 2020  ].iloc[1]).     
+0001cb50: 2020 2069 7344 6561 6443 726f 7373 4f76     isDeadCrossOv
+0001cb60: 6572 203d 2069 7332 3044 4d41 4372 6f73  er = is20DMACros
+0001cb70: 736f 7665 7235 3044 4d41 446f 776e 206f  sover50DMADown o
+0001cb80: 7220 6973 3530 444d 4143 726f 7373 6f76  r is50DMACrossov
+0001cb90: 6572 3230 3044 4d41 446f 776e 0a20 2020  er200DMADown.   
+0001cba0: 2020 2020 2064 6561 6478 4f76 6572 5465       deadxOverTe
+0001cbb0: 7874 203d 2066 2744 6561 6443 726f 7373  xt = f'DeadCross
+0001cbc0: 6f76 6572 7b22 2832 3029 2220 6966 2069  over{"(20)" if i
+0001cbd0: 7332 3044 4d41 4372 6f73 736f 7665 7235  s20DMACrossover5
+0001cbe0: 3044 4d41 446f 776e 2065 6c73 6520 2822  0DMADown else ("
+0001cbf0: 2835 3029 2220 6966 2069 7335 3044 4d41  (50)" if is50DMA
+0001cc00: 4372 6f73 736f 7665 7232 3030 444d 4144  Crossover200DMAD
+0001cc10: 6f77 6e20 656c 7365 2022 2229 7d27 0a20  own else "")}'. 
+0001cc20: 2020 2020 2020 2067 6f6c 6465 6e78 4f76         goldenxOv
+0001cc30: 6572 5465 7874 203d 2066 2747 6f6c 6465  erText = f'Golde
+0001cc40: 6e43 726f 7373 6f76 6572 7b22 2832 3029  nCrossover{"(20)
+0001cc50: 2220 6966 2069 7332 3044 4d41 4372 6f73  " if is20DMACros
+0001cc60: 736f 7665 7235 3044 4d41 2065 6c73 6520  sover50DMA else 
+0001cc70: 2822 2835 3029 2220 6966 2069 7335 3044  ("(50)" if is50D
+0001cc80: 4d41 4372 6f73 736f 7665 7232 3030 444d  MACrossover200DM
+0001cc90: 4120 656c 7365 2022 2229 7d27 0a20 2020  A else "")}'.   
+0001cca0: 2020 2020 2069 6620 6973 3230 444d 4143       if is20DMAC
+0001ccb0: 726f 7373 6f76 6572 3530 444d 4120 6f72  rossover50DMA or
+0001ccc0: 2069 7332 3044 4d41 4372 6f73 736f 7665   is20DMACrossove
+0001ccd0: 7235 3044 4d41 446f 776e 3a0a 2020 2020  r50DMADown:.    
+0001cce0: 2020 2020 2020 2020 6b65 7931 203d 2022          key1 = "
+0001ccf0: 5353 4d41 3230 220a 2020 2020 2020 2020  SSMA20".        
+0001cd00: 2020 2020 6b65 7932 203d 2022 534d 4122      key2 = "SMA"
+0001cd10: 0a20 2020 2020 2020 2020 2020 206b 6579  .            key
+0001cd20: 3320 3d20 2232 3044 4d41 220a 2020 2020  3 = "20DMA".    
+0001cd30: 2020 2020 2020 2020 6b65 7934 203d 2022          key4 = "
+0001cd40: 3530 444d 4122 0a20 2020 2020 2020 2069  50DMA".        i
+0001cd50: 7335 3044 4d41 5570 5472 656e 6420 3d20  s50DMAUpTrend = 
+0001cd60: 2872 6563 656e 745b 6b65 7931 5d2e 696c  (recent[key1].il
+0001cd70: 6f63 5b30 5d20 3e20 7265 6365 6e74 5b6b  oc[0] > recent[k
+0001cd80: 6579 325d 2e69 6c6f 635b 315d 290a 2020  ey2].iloc[1]).  
+0001cd90: 2020 2020 2020 6973 3530 444d 4144 6f77        is50DMADow
+0001cda0: 6e54 7265 6e64 203d 2028 7265 6365 6e74  nTrend = (recent
+0001cdb0: 5b6b 6579 315d 2e69 6c6f 635b 305d 203c  [key1].iloc[0] <
+0001cdc0: 2072 6563 656e 745b 6b65 7931 5d2e 696c   recent[key1].il
+0001cdd0: 6f63 5b31 5d29 0a20 2020 2020 2020 2069  oc[1]).        i
+0001cde0: 7335 3044 4d41 203d 2028 7265 6365 6e74  s50DMA = (recent
+0001cdf0: 5b6b 6579 315d 2e69 6c6f 635b 305d 203c  [key1].iloc[0] <
+0001ce00: 3d20 7265 6365 6e74 5b22 436c 6f73 6522  = recent["Close"
+0001ce10: 5d2e 696c 6f63 5b30 5d29 0a20 2020 2020  ].iloc[0]).     
+0001ce20: 2020 2069 7332 3030 444d 4120 3d20 2872     is200DMA = (r
+0001ce30: 6563 656e 745b 6b65 7932 5d2e 696c 6f63  ecent[key2].iloc
+0001ce40: 5b30 5d20 3c3d 2072 6563 656e 745b 2243  [0] <= recent["C
+0001ce50: 6c6f 7365 225d 2e69 6c6f 635b 305d 290a  lose"].iloc[0]).
+0001ce60: 2020 2020 2020 2020 6469 6666 6572 656e          differen
+0001ce70: 6365 203d 2072 6f75 6e64 2828 7265 6365  ce = round((rece
+0001ce80: 6e74 5b6b 6579 315d 2e69 6c6f 635b 305d  nt[key1].iloc[0]
+0001ce90: 202d 2072 6563 656e 745b 6b65 7932 5d2e   - recent[key2].
+0001cea0: 696c 6f63 5b30 5d29 0a20 2020 2020 2020  iloc[0]).       
+0001ceb0: 2020 2020 2020 2020 202f 2072 6563 656e           / recen
+0001cec0: 745b 2243 6c6f 7365 225d 2e69 6c6f 635b  t["Close"].iloc[
+0001ced0: 305d 0a20 2020 2020 2020 2020 2020 2020  0].             
+0001cee0: 2020 202a 2031 3030 2c0a 2020 2020 2020     * 100,.      
+0001cef0: 2020 2020 2020 2020 2020 322c 0a20 2020            2,.   
+0001cf00: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0001cf10: 2020 2073 6176 6544 6963 745b 2243 6f6e     saveDict["Con
+0001cf20: 6644 4d41 4469 6666 6572 656e 6365 225d  fDMADifference"]
+0001cf30: 203d 2064 6966 6665 7265 6e63 650a 2020   = difference.  
+0001cf40: 2020 2020 2020 7363 7265 656e 4469 6374        screenDict
+0001cf50: 5b22 436f 6e66 444d 4144 6966 6665 7265  ["ConfDMADiffere
+0001cf60: 6e63 6522 5d20 3d20 6469 6666 6572 656e  nce"] = differen
+0001cf70: 6365 0a20 2020 2020 2020 2073 6176 6564  ce.        saved
+0001cf80: 203d 2073 656c 662e 6669 6e64 4375 7272   = self.findCurr
+0001cf90: 656e 7453 6176 6564 5661 6c75 6528 7363  entSavedValue(sc
+0001cfa0: 7265 656e 4469 6374 2c73 6176 6544 6963  reenDict,saveDic
+0001cfb0: 742c 224d 412d 5369 676e 616c 2229 0a20  t,"MA-Signal"). 
+0001cfc0: 2020 2020 2020 2023 2064 6966 6665 7265         # differe
+0001cfd0: 6e63 6520 3d20 6162 7328 6469 6666 6572  nce = abs(differ
+0001cfe0: 656e 6365 290a 2020 2020 2020 2020 636f  ence).        co
+0001cff0: 6e66 5465 7874 203d 2066 227b 676f 6c64  nfText = f"{gold
+0001d000: 656e 784f 7665 7254 6578 7420 6966 2069  enxOverText if i
+0001d010: 7347 6f6c 6465 6e43 726f 7373 4f76 6572  sGoldenCrossOver
+0001d020: 2065 6c73 6520 2864 6561 6478 4f76 6572   else (deadxOver
+0001d030: 5465 7874 2069 6620 6973 4465 6164 4372  Text if isDeadCr
+0001d040: 6f73 734f 7665 7220 656c 7365 2028 2743  ossOver else ('C
+0001d050: 6f6e 662e 5570 2720 6966 2069 7335 3044  onf.Up' if is50D
+0001d060: 4d41 5570 5472 656e 6420 656c 7365 2028  MAUpTrend else (
+0001d070: 2743 6f6e 662e 446f 776e 2720 6966 2069  'Conf.Down' if i
+0001d080: 7335 3044 4d41 446f 776e 5472 656e 6420  s50DMADownTrend 
+0001d090: 656c 7365 2028 6b65 7933 2069 6620 6973  else (key3 if is
+0001d0a0: 3530 444d 4120 656c 7365 2028 6b65 7934  50DMA else (key4
+0001d0b0: 2069 6620 6973 3230 3044 4d41 2065 6c73   if is200DMA els
+0001d0c0: 6520 2755 6e6b 6e6f 776e 2729 2929 2929  e 'Unknown')))))
+0001d0d0: 7d22 0a20 2020 2020 2020 2069 6620 6162  }".        if ab
+0001d0e0: 7328 7265 6365 6e74 5b6b 6579 315d 2e69  s(recent[key1].i
+0001d0f0: 6c6f 635b 305d 202d 2072 6563 656e 745b  loc[0] - recent[
+0001d100: 6b65 7932 5d2e 696c 6f63 5b30 5d29 203c  key2].iloc[0]) <
+0001d110: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+0001d120: 7265 6365 6e74 5b6b 6579 315d 2e69 6c6f  recent[key1].ilo
+0001d130: 635b 305d 202a 2070 6572 6365 6e74 6167  c[0] * percentag
+0001d140: 650a 2020 2020 2020 2020 293a 0a20 2020  e.        ):.   
+0001d150: 2020 2020 2020 2020 2069 6620 7265 6365           if rece
+0001d160: 6e74 5b6b 6579 315d 2e69 6c6f 635b 305d  nt[key1].iloc[0]
+0001d170: 203e 3d20 7265 6365 6e74 5b6b 6579 325d   >= recent[key2]
+0001d180: 2e69 6c6f 635b 305d 3a0a 2020 2020 2020  .iloc[0]:.      
+0001d190: 2020 2020 2020 2020 2020 7363 7265 656e            screen
+0001d1a0: 4469 6374 5b22 4d41 2d53 6967 6e61 6c22  Dict["MA-Signal"
+0001d1b0: 5d20 3d20 280a 2020 2020 2020 2020 2020  ] = (.          
+0001d1c0: 2020 2020 2020 2020 2020 7361 7665 645b            saved[
+0001d1d0: 305d 200a 2020 2020 2020 2020 2020 2020  0] .            
+0001d1e0: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
+0001d1f0: 6578 742e 424f 4c44 0a20 2020 2020 2020  ext.BOLD.       
+0001d200: 2020 2020 2020 2020 2020 2020 202b 2028               + (
+0001d210: 636f 6c6f 7254 6578 742e 4752 4545 4e20  colorText.GREEN 
+0001d220: 6966 2069 7335 3044 4d41 5570 5472 656e  if is50DMAUpTren
+0001d230: 6420 656c 7365 2028 636f 6c6f 7254 6578  d else (colorTex
+0001d240: 742e 4641 494c 2069 6620 6973 3530 444d  t.FAIL if is50DM
+0001d250: 4144 6f77 6e54 7265 6e64 2065 6c73 6520  ADownTrend else 
+0001d260: 636f 6c6f 7254 6578 742e 5741 524e 2929  colorText.WARN))
+0001d270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001d280: 2020 2020 202b 2066 227b 636f 6e66 5465       + f"{confTe
+0001d290: 7874 7d20 287b 6469 6666 6572 656e 6365  xt} ({difference
+0001d2a0: 7d25 2922 0a20 2020 2020 2020 2020 2020  }%)".           
+0001d2b0: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
+0001d2c0: 5465 7874 2e45 4e44 0a20 2020 2020 2020  Text.END.       
+0001d2d0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0001d2e0: 2020 2020 2020 2020 2020 2073 6176 6544             saveD
+0001d2f0: 6963 745b 224d 412d 5369 676e 616c 225d  ict["MA-Signal"]
+0001d300: 203d 2073 6176 6564 5b31 5d20 2b20 6622   = saved[1] + f"
+0001d310: 7b63 6f6e 6654 6578 747d 2028 7b64 6966  {confText} ({dif
+0001d320: 6665 7265 6e63 657d 2529 220a 2020 2020  ference}%)".    
+0001d330: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0001d340: 2020 2020 2020 2020 2020 2020 2020 7363                sc
+0001d350: 7265 656e 4469 6374 5b22 4d41 2d53 6967  reenDict["MA-Sig
+0001d360: 6e61 6c22 5d20 3d20 280a 2020 2020 2020  nal"] = (.      
+0001d370: 2020 2020 2020 2020 2020 2020 2020 7361                sa
+0001d380: 7665 645b 305d 200a 2020 2020 2020 2020  ved[0] .        
+0001d390: 2020 2020 2020 2020 2020 2020 2b20 636f              + co
+0001d3a0: 6c6f 7254 6578 742e 424f 4c44 0a20 2020  lorText.BOLD.   
+0001d3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d3c0: 202b 2028 636f 6c6f 7254 6578 742e 4752   + (colorText.GR
+0001d3d0: 4545 4e20 6966 2069 7335 3044 4d41 5570  EEN if is50DMAUp
+0001d3e0: 5472 656e 6420 656c 7365 2028 636f 6c6f  Trend else (colo
+0001d3f0: 7254 6578 742e 4641 494c 2069 6620 6973  rText.FAIL if is
+0001d400: 3530 444d 4144 6f77 6e54 7265 6e64 2065  50DMADownTrend e
+0001d410: 6c73 6520 636f 6c6f 7254 6578 742e 5741  lse colorText.WA
+0001d420: 524e 2929 0a20 2020 2020 2020 2020 2020  RN)).           
+0001d430: 2020 2020 2020 2020 202b 2066 227b 636f           + f"{co
+0001d440: 6e66 5465 7874 7d20 287b 6469 6666 6572  nfText} ({differ
+0001d450: 656e 6365 7d25 2922 0a20 2020 2020 2020  ence}%)".       
+0001d460: 2020 2020 2020 2020 2020 2020 202b 2063               + c
+0001d470: 6f6c 6f72 5465 7874 2e45 4e44 0a20 2020  olorText.END.   
+0001d480: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+0001d490: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001d4a0: 6176 6544 6963 745b 224d 412d 5369 676e  aveDict["MA-Sign
+0001d4b0: 616c 225d 203d 2073 6176 6564 5b31 5d20  al"] = saved[1] 
+0001d4c0: 2b20 6622 7b63 6f6e 6654 6578 747d 2028  + f"{confText} (
+0001d4d0: 7b64 6966 6665 7265 6e63 657d 2529 220a  {difference}%)".
+0001d4e0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0001d4f0: 726e 2063 6f6e 6646 696c 7465 7220 3d3d  rn confFilter ==
+0001d500: 2033 206f 7220 5c0a 2020 2020 2020 2020   3 or \.        
+0001d510: 2020 2020 2020 2020 2863 6f6e 6646 696c          (confFil
+0001d520: 7465 7220 3d3d 2031 2061 6e64 206e 6f74  ter == 1 and not
+0001d530: 2069 7344 6561 6443 726f 7373 4f76 6572   isDeadCrossOver
+0001d540: 2061 6e64 2028 6973 3530 444d 4155 7054   and (is50DMAUpT
+0001d550: 7265 6e64 206f 7220 2869 7347 6f6c 6465  rend or (isGolde
+0001d560: 6e43 726f 7373 4f76 6572 206f 7220 2755  nCrossOver or 'U
+0001d570: 7027 2069 6e20 636f 6e66 5465 7874 2929  p' in confText))
+0001d580: 2920 6f72 205c 0a20 2020 2020 2020 2020  ) or \.         
+0001d590: 2020 2020 2020 2028 636f 6e66 4669 6c74         (confFilt
+0001d5a0: 6572 203d 3d20 3220 616e 6420 6e6f 7420  er == 2 and not 
+0001d5b0: 6973 476f 6c64 656e 4372 6f73 734f 7665  isGoldenCrossOve
+0001d5c0: 7220 616e 6420 2869 7335 3044 4d41 446f  r and (is50DMADo
+0001d5d0: 776e 5472 656e 6420 6f72 2069 7344 6561  wnTrend or isDea
+0001d5e0: 6443 726f 7373 4f76 6572 206f 7220 2744  dCrossOver or 'D
+0001d5f0: 6f77 6e27 2069 6e20 636f 6e66 5465 7874  own' in confText
+0001d600: 2929 0a20 2020 2020 2020 2023 204d 6179  )).        # May
+0001d610: 6265 2074 6865 2064 6966 6665 7265 6e63  be the differenc
+0001d620: 6520 6973 206e 6f74 2077 6974 6869 6e20  e is not within 
+0001d630: 7468 6520 7261 6e67 652c 2062 7574 2077  the range, but w
+0001d640: 6527 6420 7374 696c 6c20 6c69 6b65 2074  e'd still like t
+0001d650: 6f20 6b65 6570 2074 6865 2073 746f 636b  o keep the stock
+0001d660: 2069 6e0a 2020 2020 2020 2020 2320 7468   in.        # th
+0001d670: 6520 6c69 7374 2069 6620 6974 2773 2061  e list if it's a
+0001d680: 2067 6f6c 6465 6e20 6372 6f73 736f 7665   golden crossove
+0001d690: 7220 6f72 2064 6561 6420 6372 6f73 736f  r or dead crosso
+0001d6a0: 7665 720a 2020 2020 2020 2020 6966 2069  ver.        if i
+0001d6b0: 7347 6f6c 6465 6e43 726f 7373 4f76 6572  sGoldenCrossOver
+0001d6c0: 206f 7220 6973 4465 6164 4372 6f73 734f   or isDeadCrossO
+0001d6d0: 7665 723a 0a20 2020 2020 2020 2020 2020  ver:.           
+0001d6e0: 2073 6372 6565 6e44 6963 745b 224d 412d   screenDict["MA-
+0001d6f0: 5369 676e 616c 225d 203d 2028 0a20 2020  Signal"] = (.   
+0001d700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d710: 2073 6176 6564 5b30 5d20 0a20 2020 2020   saved[0] .     
+0001d720: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+0001d730: 2063 6f6c 6f72 5465 7874 2e42 4f4c 440a   colorText.BOLD.
+0001d740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d750: 2020 2020 2b20 2863 6f6c 6f72 5465 7874      + (colorText
+0001d760: 2e47 5245 454e 2069 6620 6973 3530 444d  .GREEN if is50DM
+0001d770: 4155 7054 7265 6e64 2065 6c73 6520 2863  AUpTrend else (c
+0001d780: 6f6c 6f72 5465 7874 2e46 4149 4c20 6966  olorText.FAIL if
+0001d790: 2069 7335 3044 4d41 446f 776e 5472 656e   is50DMADownTren
+0001d7a0: 6420 656c 7365 2063 6f6c 6f72 5465 7874  d else colorText
+0001d7b0: 2e57 4152 4e29 290a 2020 2020 2020 2020  .WARN)).        
+0001d7c0: 2020 2020 2020 2020 2020 2020 2b20 6622              + f"
+0001d7d0: 7b63 6f6e 6654 6578 747d 2028 7b64 6966  {confText} ({dif
+0001d7e0: 6665 7265 6e63 657d 2529 220a 2020 2020  ference}%)".    
+0001d7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d800: 2b20 636f 6c6f 7254 6578 742e 454e 440a  + colorText.END.
+0001d810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d820: 290a 2020 2020 2020 2020 2020 2020 7361  ).            sa
+0001d830: 7665 4469 6374 5b22 4d41 2d53 6967 6e61  veDict["MA-Signa
+0001d840: 6c22 5d20 3d20 7361 7665 645b 315d 202b  l"] = saved[1] +
+0001d850: 2066 227b 636f 6e66 5465 7874 7d20 287b   f"{confText} ({
+0001d860: 6469 6666 6572 656e 6365 7d25 2922 0a20  difference}%)". 
+0001d870: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0001d880: 6e20 636f 6e66 4669 6c74 6572 203d 3d20  n confFilter == 
+0001d890: 3320 6f72 205c 0a20 2020 2020 2020 2020  3 or \.         
+0001d8a0: 2020 2020 2020 2028 636f 6e66 4669 6c74         (confFilt
+0001d8b0: 6572 203d 3d20 3120 616e 6420 6973 476f  er == 1 and isGo
+0001d8c0: 6c64 656e 4372 6f73 734f 7665 7229 206f  ldenCrossOver) o
+0001d8d0: 7220 5c0a 2020 2020 2020 2020 2020 2020  r \.            
+0001d8e0: 2020 2020 2863 6f6e 6646 696c 7465 7220      (confFilter 
+0001d8f0: 3d3d 2032 2061 6e64 2069 7344 6561 6443  == 2 and isDeadC
+0001d900: 726f 7373 4f76 6572 290a 2020 2020 2020  rossOver).      
+0001d910: 2020 7265 7475 726e 2046 616c 7365 0a0a    return False..
+0001d920: 2020 2020 2340 6d65 6173 7572 655f 7469      #@measure_ti
+0001d930: 6d65 0a20 2020 2023 2056 616c 6964 6174  me.    # Validat
+0001d940: 6520 6966 2073 6861 7265 2070 7269 6365  e if share price
+0001d950: 7320 6172 6520 636f 6e73 6f6c 6964 6174  s are consolidat
+0001d960: 696e 670a 2020 2020 6465 6620 7661 6c69  ing.    def vali
+0001d970: 6461 7465 436f 6e73 6f6c 6964 6174 696f  dateConsolidatio
+0001d980: 6e28 7365 6c66 2c20 6466 2c20 7363 7265  n(self, df, scre
+0001d990: 656e 4469 6374 2c20 7361 7665 4469 6374  enDict, saveDict
+0001d9a0: 2c20 7065 7263 656e 7461 6765 3d31 3029  , percentage=10)
+0001d9b0: 3a0a 2020 2020 2020 2020 6966 2064 6620  :.        if df 
+0001d9c0: 6973 204e 6f6e 6520 6f72 206c 656e 2864  is None or len(d
+0001d9d0: 6629 203d 3d20 303a 0a20 2020 2020 2020  f) == 0:.       
+0001d9e0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+0001d9f0: 650a 2020 2020 2020 2020 6461 7461 203d  e.        data =
+0001da00: 2064 662e 636f 7079 2829 0a20 2020 2020   df.copy().     
+0001da10: 2020 2064 6174 6120 3d20 6461 7461 2e66     data = data.f
+0001da20: 696c 6c6e 6128 3029 0a20 2020 2020 2020  illna(0).       
+0001da30: 2064 6174 6120 3d20 6461 7461 2e72 6570   data = data.rep
+0001da40: 6c61 6365 285b 6e70 2e69 6e66 2c20 2d6e  lace([np.inf, -n
+0001da50: 702e 696e 665d 2c20 3029 0a20 2020 2020  p.inf], 0).     
+0001da60: 2020 2068 6320 3d20 6461 7461 2e64 6573     hc = data.des
+0001da70: 6372 6962 6528 295b 2243 6c6f 7365 225d  cribe()["Close"]
+0001da80: 5b22 6d61 7822 5d0a 2020 2020 2020 2020  ["max"].        
+0001da90: 6c63 203d 2064 6174 612e 6465 7363 7269  lc = data.descri
+0001daa0: 6265 2829 5b22 436c 6f73 6522 5d5b 226d  be()["Close"]["m
+0001dab0: 696e 225d 0a20 2020 2020 2020 2069 6620  in"].        if 
+0001dac0: 2868 6320 2d20 6c63 2920 3c3d 2028 6863  (hc - lc) <= (hc
+0001dad0: 202a 2070 6572 6365 6e74 6167 6520 2f20   * percentage / 
+0001dae0: 3130 3029 2061 6e64 2028 6863 202d 206c  100) and (hc - l
+0001daf0: 6320 213d 2030 293a 0a20 2020 2020 2020  c != 0):.       
+0001db00: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
+0001db10: 2243 6f6e 736f 6c2e 225d 203d 2028 0a20  "Consol."] = (. 
+0001db20: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0001db30: 6f6c 6f72 5465 7874 2e42 4f4c 440a 2020  olorText.BOLD.  
+0001db40: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+0001db50: 636f 6c6f 7254 6578 742e 4752 4545 4e0a  colorText.GREEN.
+0001db60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001db70: 2b20 2252 616e 6765 3a22 0a20 2020 2020  + "Range:".     
+0001db80: 2020 2020 2020 2020 2020 202b 2073 7472             + str
+0001db90: 2872 6f75 6e64 2828 6162 7328 2868 6320  (round((abs((hc 
+0001dba0: 2d20 6c63 2920 2f20 6863 2920 2a20 3130  - lc) / hc) * 10
+0001dbb0: 3029 2c20 3129 290a 2020 2020 2020 2020  0), 1)).        
+0001dbc0: 2020 2020 2020 2020 2b20 2225 220a 2020          + "%".  
+0001dbd0: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+0001dbe0: 636f 6c6f 7254 6578 742e 454e 440a 2020  colorText.END.  
+0001dbf0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0001dc00: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0001dc10: 2020 2020 2020 7363 7265 656e 4469 6374        screenDict
+0001dc20: 5b22 436f 6e73 6f6c 2e22 5d20 3d20 280a  ["Consol."] = (.
+0001dc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dc40: 636f 6c6f 7254 6578 742e 424f 4c44 0a20  colorText.BOLD. 
+0001dc50: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+0001dc60: 2063 6f6c 6f72 5465 7874 2e46 4149 4c0a   colorText.FAIL.
+0001dc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dc80: 2b20 2252 616e 6765 3a22 0a20 2020 2020  + "Range:".     
+0001dc90: 2020 2020 2020 2020 2020 202b 2073 7472             + str
+0001dca0: 2872 6f75 6e64 2828 6162 7328 2868 6320  (round((abs((hc 
+0001dcb0: 2d20 6c63 2920 2f20 6863 2920 2a20 3130  - lc) / hc) * 10
+0001dcc0: 3029 2c20 3129 290a 2020 2020 2020 2020  0), 1)).        
+0001dcd0: 2020 2020 2020 2020 2b20 2225 220a 2020          + "%".  
+0001dce0: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+0001dcf0: 636f 6c6f 7254 6578 742e 454e 440a 2020  colorText.END.  
+0001dd00: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0001dd10: 2020 2020 7361 7665 4469 6374 5b22 436f      saveDict["Co
+0001dd20: 6e73 6f6c 2e22 5d20 3d20 6627 5261 6e67  nsol."] = f'Rang
+0001dd30: 653a 7b73 7472 2872 6f75 6e64 2828 6162  e:{str(round((ab
+0001dd40: 7328 2868 632d 6c63 292f 6863 292a 3130  s((hc-lc)/hc)*10
+0001dd50: 3029 2c31 2929 2b22 2522 7d27 0a20 2020  0),1))+"%"}'.   
+0001dd60: 2020 2020 2072 6574 7572 6e20 726f 756e       return roun
+0001dd70: 6428 2861 6273 2828 6863 202d 206c 6329  d((abs((hc - lc)
+0001dd80: 202f 2068 6329 202a 2031 3030 292c 2031   / hc) * 100), 1
+0001dd90: 290a 0a20 2020 2023 2076 616c 6964 6174  )..    # validat
+0001dda0: 6520 6966 2074 6865 2073 746f 636b 2068  e if the stock h
+0001ddb0: 6173 2062 6565 6e20 6861 7669 6e67 2068  as been having h
+0001ddc0: 6967 6865 7220 6869 6768 732c 2068 6967  igher highs, hig
+0001ddd0: 6865 7220 6c6f 7773 0a20 2020 2023 2061  her lows.    # a
+0001dde0: 6e64 2068 6967 6865 7220 636c 6f73 6520  nd higher close 
+0001ddf0: 7769 7468 206c 6174 6573 7420 636c 6f73  with latest clos
+0001de00: 6520 3e20 7375 7065 7274 7265 6e64 2061  e > supertrend a
+0001de10: 6e64 2038 2d45 4d41 2e0a 2020 2020 6465  nd 8-EMA..    de
+0001de20: 6620 7661 6c69 6461 7465 4869 6768 6572  f validateHigher
+0001de30: 4869 6768 7348 6967 6865 724c 6f77 7348  HighsHigherLowsH
+0001de40: 6967 6865 7243 6c6f 7365 2873 656c 662c  igherClose(self,
+0001de50: 2064 6629 3a0a 2020 2020 2020 2020 6966   df):.        if
+0001de60: 2064 6620 6973 204e 6f6e 6520 6f72 206c   df is None or l
+0001de70: 656e 2864 6629 203d 3d20 303a 0a20 2020  en(df) == 0:.   
+0001de80: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0001de90: 4661 6c73 650a 2020 2020 2020 2020 6461  False.        da
+0001dea0: 7461 203d 2064 662e 636f 7079 2829 0a20  ta = df.copy(). 
+0001deb0: 2020 2020 2020 2064 6179 3020 3d20 6461         day0 = da
+0001dec0: 7461 0a20 2020 2020 2020 2064 6179 3120  ta.        day1 
+0001ded0: 3d20 6461 7461 5b31 3a5d 0a20 2020 2020  = data[1:].     
+0001dee0: 2020 2064 6179 3220 3d20 6461 7461 5b32     day2 = data[2
+0001def0: 3a5d 0a20 2020 2020 2020 2064 6179 3320  :].        day3 
+0001df00: 3d20 6461 7461 5b33 3a5d 0a20 2020 2020  = data[3:].     
+0001df10: 2020 2069 6620 6c65 6e28 6461 7931 2920     if len(day1) 
+0001df20: 3c20 3120 6f72 206c 656e 2864 6179 3229  < 1 or len(day2)
+0001df30: 203c 2031 206f 7220 6c65 6e28 6461 7933   < 1 or len(day3
+0001df40: 2920 3c20 313a 0a20 2020 2020 2020 2020  ) < 1:.         
+0001df50: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+0001df60: 2020 2020 2020 2020 6869 6768 6572 4869          higherHi
+0001df70: 6768 7320 3d20 280a 2020 2020 2020 2020  ghs = (.        
+0001df80: 2020 2020 2864 6179 305b 2248 6967 6822      (day0["High"
+0001df90: 5d2e 696c 6f63 5b30 5d20 3e20 6461 7931  ].iloc[0] > day1
+0001dfa0: 5b22 4869 6768 225d 2e69 6c6f 635b 305d  ["High"].iloc[0]
+0001dfb0: 290a 2020 2020 2020 2020 2020 2020 616e  ).            an
+0001dfc0: 6420 2864 6179 315b 2248 6967 6822 5d2e  d (day1["High"].
+0001dfd0: 696c 6f63 5b30 5d20 3e20 6461 7932 5b22  iloc[0] > day2["
+0001dfe0: 4869 6768 225d 2e69 6c6f 635b 305d 290a  High"].iloc[0]).
+0001dff0: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+0001e000: 2864 6179 325b 2248 6967 6822 5d2e 696c  (day2["High"].il
+0001e010: 6f63 5b30 5d20 3e20 6461 7933 5b22 4869  oc[0] > day3["Hi
+0001e020: 6768 225d 2e69 6c6f 635b 305d 290a 2020  gh"].iloc[0]).  
+0001e030: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0001e040: 6869 6768 6572 4c6f 7773 203d 2028 0a20  higherLows = (. 
+0001e050: 2020 2020 2020 2020 2020 2028 6461 7930             (day0
+0001e060: 5b22 4c6f 7722 5d2e 696c 6f63 5b30 5d20  ["Low"].iloc[0] 
+0001e070: 3e20 6461 7931 5b22 4c6f 7722 5d2e 696c  > day1["Low"].il
+0001e080: 6f63 5b30 5d29 0a20 2020 2020 2020 2020  oc[0]).         
+0001e090: 2020 2061 6e64 2028 6461 7931 5b22 4c6f     and (day1["Lo
+0001e0a0: 7722 5d2e 696c 6f63 5b30 5d20 3e20 6461  w"].iloc[0] > da
+0001e0b0: 7932 5b22 4c6f 7722 5d2e 696c 6f63 5b30  y2["Low"].iloc[0
+0001e0c0: 5d29 0a20 2020 2020 2020 2020 2020 2061  ]).            a
+0001e0d0: 6e64 2028 6461 7932 5b22 4c6f 7722 5d2e  nd (day2["Low"].
+0001e0e0: 696c 6f63 5b30 5d20 3e20 6461 7933 5b22  iloc[0] > day3["
+0001e0f0: 4c6f 7722 5d2e 696c 6f63 5b30 5d29 0a20  Low"].iloc[0]). 
+0001e100: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0001e110: 2068 6967 6865 7243 6c6f 7365 203d 2028   higherClose = (
+0001e120: 0a20 2020 2020 2020 2020 2020 2028 6461  .            (da
+0001e130: 7930 5b22 436c 6f73 6522 5d2e 696c 6f63  y0["Close"].iloc
+0001e140: 5b30 5d20 3e20 6461 7931 5b22 436c 6f73  [0] > day1["Clos
+0001e150: 6522 5d2e 696c 6f63 5b30 5d29 0a20 2020  e"].iloc[0]).   
+0001e160: 2020 2020 2020 2020 2061 6e64 2028 6461           and (da
+0001e170: 7931 5b22 436c 6f73 6522 5d2e 696c 6f63  y1["Close"].iloc
+0001e180: 5b30 5d20 3e20 6461 7932 5b22 436c 6f73  [0] > day2["Clos
+0001e190: 6522 5d2e 696c 6f63 5b30 5d29 0a20 2020  e"].iloc[0]).   
+0001e1a0: 2020 2020 2020 2020 2061 6e64 2028 6461           and (da
+0001e1b0: 7932 5b22 436c 6f73 6522 5d2e 696c 6f63  y2["Close"].iloc
+0001e1c0: 5b30 5d20 3e20 6461 7933 5b22 436c 6f73  [0] > day3["Clos
+0001e1d0: 6522 5d2e 696c 6f63 5b30 5d29 0a20 2020  e"].iloc[0]).   
+0001e1e0: 2020 2020 2029 0a20 2020 2020 2020 2023       ).        #
+0001e1f0: 2068 6967 6865 7252 5349 203d 2028 6461   higherRSI = (da
+0001e200: 7930 5b22 5253 4922 5d2e 696c 6f63 5b30  y0["RSI"].iloc[0
+0001e210: 5d20 3e20 6461 7931 5b22 5253 4922 5d2e  ] > day1["RSI"].
+0001e220: 696c 6f63 5b30 5d29 2061 6e64 205c 0a20  iloc[0]) and \. 
+0001e230: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+0001e240: 2020 2020 2020 2020 2028 6461 7931 5b22           (day1["
+0001e250: 5253 4922 5d2e 696c 6f63 5b30 5d20 3e20  RSI"].iloc[0] > 
+0001e260: 6461 7932 5b22 5253 4922 5d2e 696c 6f63  day2["RSI"].iloc
+0001e270: 5b30 5d29 2061 6e64 205c 0a20 2020 2020  [0]) and \.     
+0001e280: 2020 2023 2020 2020 2020 2020 2020 2020     #            
+0001e290: 2020 2020 2028 6461 7932 5b22 5253 4922       (day2["RSI"
+0001e2a0: 5d2e 696c 6f63 5b30 5d20 3e20 6461 7933  ].iloc[0] > day3
+0001e2b0: 5b22 5253 4922 5d2e 696c 6f63 5b30 5d29  ["RSI"].iloc[0])
+0001e2c0: 2061 6e64 205c 0a20 2020 2020 2020 2023   and \.        #
+0001e2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e2e0: 2064 6179 335b 2252 5349 225d 2e69 6c6f   day3["RSI"].ilo
+0001e2f0: 635b 305d 203e 3d20 3530 2061 6e64 2064  c[0] >= 50 and d
+0001e300: 6179 305b 2252 5349 225d 2e69 6c6f 635b  ay0["RSI"].iloc[
+0001e310: 305d 203e 3d20 3635 0a20 2020 2020 2020  0] >= 65.       
+0001e320: 2072 6576 6572 7365 6444 6174 6120 3d20   reversedData = 
+0001e330: 6461 7461 5b3a 3a2d 315d 2e63 6f70 7928  data[::-1].copy(
+0001e340: 290a 2020 2020 2020 2020 7265 7665 7273  ).        revers
+0001e350: 6564 4461 7461 5b22 5355 5045 5254 225d  edData["SUPERT"]
+0001e360: 203d 2070 6b74 616c 6962 2e73 7570 6572   = pktalib.super
+0001e370: 7472 656e 6428 7265 7665 7273 6564 4461  trend(reversedDa
+0001e380: 7461 2c20 372c 2033 295b 2253 5550 4552  ta, 7, 3)["SUPER
+0001e390: 545f 375f 332e 3022 5d0a 2020 2020 2020  T_7_3.0"].      
+0001e3a0: 2020 7265 7665 7273 6564 4461 7461 5b22    reversedData["
+0001e3b0: 454d 4138 225d 203d 2070 6b74 616c 6962  EMA8"] = pktalib
+0001e3c0: 2e45 4d41 2872 6576 6572 7365 6444 6174  .EMA(reversedDat
+0001e3d0: 615b 2243 6c6f 7365 225d 2c20 7469 6d65  a["Close"], time
+0001e3e0: 7065 7269 6f64 3d39 290a 2020 2020 2020  period=9).      
+0001e3f0: 2020 6869 6768 6572 436c 6f73 6520 3d20    higherClose = 
+0001e400: 280a 2020 2020 2020 2020 2020 2020 6869  (.            hi
+0001e410: 6768 6572 436c 6f73 650a 2020 2020 2020  gherClose.      
+0001e420: 2020 2020 2020 616e 6420 6461 7930 5b22        and day0["
+0001e430: 436c 6f73 6522 5d2e 696c 6f63 5b30 5d20  Close"].iloc[0] 
+0001e440: 3e20 7265 7665 7273 6564 4461 7461 2e74  > reversedData.t
+0001e450: 6169 6c28 3129 5b22 5355 5045 5254 225d  ail(1)["SUPERT"]
+0001e460: 2e69 6c6f 635b 305d 0a20 2020 2020 2020  .iloc[0].       
+0001e470: 2020 2020 2061 6e64 2064 6179 305b 2243       and day0["C
+0001e480: 6c6f 7365 225d 2e69 6c6f 635b 305d 203e  lose"].iloc[0] >
+0001e490: 2072 6576 6572 7365 6444 6174 612e 7461   reversedData.ta
+0001e4a0: 696c 2831 295b 2245 4d41 3822 5d2e 696c  il(1)["EMA8"].il
+0001e4b0: 6f63 5b30 5d0a 2020 2020 2020 2020 290a  oc[0].        ).
+0001e4c0: 2020 2020 2020 2020 7265 7475 726e 2068          return h
+0001e4d0: 6967 6865 7248 6967 6873 2061 6e64 2068  igherHighs and h
+0001e4e0: 6967 6865 724c 6f77 7320 616e 6420 6869  igherLows and hi
+0001e4f0: 6768 6572 436c 6f73 650a 0a20 2020 2023  gherClose..    #
+0001e500: 406d 6561 7375 7265 5f74 696d 650a 2020  @measure_time.  
+0001e510: 2020 2320 5661 6c69 6461 7465 2027 496e    # Validate 'In
+0001e520: 7369 6465 2042 6172 2720 7374 7275 6374  side Bar' struct
+0001e530: 7572 6520 666f 7220 7265 6365 6e74 2064  ure for recent d
+0001e540: 6179 730a 2020 2020 6465 6620 7661 6c69  ays.    def vali
+0001e550: 6461 7465 496e 7369 6465 4261 7228 0a20  dateInsideBar(. 
+0001e560: 2020 2020 2020 2073 656c 662c 2064 662c         self, df,
+0001e570: 2073 6372 6565 6e44 6963 742c 2073 6176   screenDict, sav
+0001e580: 6544 6963 742c 2063 6861 7274 5061 7474  eDict, chartPatt
+0001e590: 6572 6e3d 312c 2064 6179 7354 6f4c 6f6f  ern=1, daysToLoo
+0001e5a0: 6b62 6163 6b3d 350a 2020 2020 293a 0a20  kback=5.    ):. 
+0001e5b0: 2020 2020 2020 2069 6620 6466 2069 7320         if df is 
+0001e5c0: 4e6f 6e65 206f 7220 6c65 6e28 6466 2920  None or len(df) 
+0001e5d0: 3d3d 2030 3a0a 2020 2020 2020 2020 2020  == 0:.          
+0001e5e0: 2020 7265 7475 726e 2046 616c 7365 0a20    return False. 
+0001e5f0: 2020 2020 2020 2064 6174 6120 3d20 6466         data = df
+0001e600: 2e63 6f70 7928 290a 2020 2020 2020 2020  .copy().        
+0001e610: 6f72 6744 6174 6120 3d20 6461 7461 0a20  orgData = data. 
+0001e620: 2020 2020 2020 2073 6176 6564 203d 2073         saved = s
+0001e630: 656c 662e 6669 6e64 4375 7272 656e 7453  elf.findCurrentS
+0001e640: 6176 6564 5661 6c75 6528 7363 7265 656e  avedValue(screen
+0001e650: 4469 6374 2c20 7361 7665 4469 6374 2c20  Dict, saveDict, 
+0001e660: 2250 6174 7465 726e 2229 0a20 2020 2020  "Pattern").     
+0001e670: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
+0001e680: 6528 696e 7428 6461 7973 546f 4c6f 6f6b  e(int(daysToLook
+0001e690: 6261 636b 292c 2069 6e74 2872 6f75 6e64  back), int(round
+0001e6a0: 2864 6179 7354 6f4c 6f6f 6b62 6163 6b20  (daysToLookback 
+0001e6b0: 2a20 302e 3529 2920 2d20 312c 202d 3129  * 0.5)) - 1, -1)
+0001e6c0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+0001e6d0: 2069 203d 3d20 323a 0a20 2020 2020 2020   i == 2:.       
+0001e6e0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0001e6f0: 3020 2023 2045 7869 7420 6966 206f 6e6c  0  # Exit if onl
+0001e700: 7920 6c61 7374 2032 2063 616e 646c 6573  y last 2 candles
+0001e710: 2061 7265 206c 6566 740a 2020 2020 2020   are left.      
+0001e720: 2020 2020 2020 6966 2063 6861 7274 5061        if chartPa
+0001e730: 7474 6572 6e20 3d3d 2031 3a0a 2020 2020  ttern == 1:.    
+0001e740: 2020 2020 2020 2020 2020 2020 6966 2022              if "
+0001e750: 5570 2220 696e 2073 6176 6544 6963 745b  Up" in saveDict[
+0001e760: 2254 7265 6e64 225d 2061 6e64 2028 0a20  "Trend"] and (. 
+0001e770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e780: 2020 2022 4275 6c6c 2220 696e 2073 6176     "Bull" in sav
+0001e790: 6544 6963 745b 224d 412d 5369 676e 616c  eDict["MA-Signal
+0001e7a0: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
+0001e7b0: 2020 2020 2020 206f 7220 2253 7570 706f         or "Suppo
+0001e7c0: 7274 2220 696e 2073 6176 6544 6963 745b  rt" in saveDict[
+0001e7d0: 224d 412d 5369 676e 616c 225d 0a20 2020  "MA-Signal"].   
+0001e7e0: 2020 2020 2020 2020 2020 2020 2029 3a0a               ):.
+0001e7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e800: 2020 2020 6461 7461 203d 206f 7267 4461      data = orgDa
+0001e810: 7461 2e68 6561 6428 6929 0a20 2020 2020  ta.head(i).     
+0001e820: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0001e830: 6566 4361 6e64 6c65 203d 2064 6174 612e  efCandle = data.
+0001e840: 7461 696c 2831 290a 2020 2020 2020 2020  tail(1).        
+0001e850: 2020 2020 2020 2020 2020 2020 6966 2028              if (
+0001e860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001e870: 2020 2020 2020 2020 2028 6c65 6e28 6461           (len(da
+0001e880: 7461 2e48 6967 685b 6461 7461 2e48 6967  ta.High[data.Hig
+0001e890: 6820 3e20 7265 6643 616e 646c 652e 4869  h > refCandle.Hi
+0001e8a0: 6768 2e69 7465 6d28 295d 2920 3d3d 2030  gh.item()]) == 0
+0001e8b0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001e8c0: 2020 2020 2020 2020 2020 616e 6420 286c            and (l
+0001e8d0: 656e 2864 6174 612e 4c6f 775b 6461 7461  en(data.Low[data
+0001e8e0: 2e4c 6f77 203c 2072 6566 4361 6e64 6c65  .Low < refCandle
+0001e8f0: 2e4c 6f77 2e69 7465 6d28 295d 2920 3d3d  .Low.item()]) ==
+0001e900: 2030 290a 2020 2020 2020 2020 2020 2020   0).            
+0001e910: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+0001e920: 286c 656e 2864 6174 612e 4f70 656e 5b64  (len(data.Open[d
+0001e930: 6174 612e 4f70 656e 203e 2072 6566 4361  ata.Open > refCa
+0001e940: 6e64 6c65 2e48 6967 682e 6974 656d 2829  ndle.High.item()
+0001e950: 5d29 203d 3d20 3029 0a20 2020 2020 2020  ]) == 0).       
+0001e960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e970: 2061 6e64 2028 6c65 6e28 6461 7461 2e43   and (len(data.C
+0001e980: 6c6f 7365 5b64 6174 612e 436c 6f73 6520  lose[data.Close 
+0001e990: 3c20 7265 6643 616e 646c 652e 4c6f 772e  < refCandle.Low.
+0001e9a0: 6974 656d 2829 5d29 203d 3d20 3029 0a20  item()]) == 0). 
+0001e9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e9c0: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
+0001e9d0: 2020 2020 2020 2020 2020 2020 2020 7363                sc
+0001e9e0: 7265 656e 4469 6374 5b22 5061 7474 6572  reenDict["Patter
+0001e9f0: 6e22 5d20 3d20 280a 2020 2020 2020 2020  n"] = (.        
+0001ea00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ea10: 2020 2020 7361 7665 645b 305d 0a20 2020      saved[0].   
 0001ea20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ea30: 2020 2020 2020 2b20 2822 496e 7369 6465        + ("Inside
-0001ea40: 2042 6172 2028 2564 2922 2025 2069 290a   Bar (%d)" % i).
+0001ea30: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
+0001ea40: 5465 7874 2e42 4f4c 440a 2020 2020 2020  Text.BOLD.      
 0001ea50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ea60: 2020 2020 2020 2020 2020 2020 2b20 636f              + co
-0001ea70: 6c6f 7254 6578 742e 454e 440a 2020 2020  lorText.END.    
+0001ea60: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
+0001ea70: 742e 5741 524e 0a20 2020 2020 2020 2020  t.WARN.         
 0001ea80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ea90: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-0001eaa0: 2020 2020 2020 2020 2020 2020 2020 7361                sa
-0001eab0: 7665 4469 6374 5b22 5061 7474 6572 6e22  veDict["Pattern"
-0001eac0: 5d20 3d20 7361 7665 645b 315d 202b 2022  ] = saved[1] + "
-0001ead0: 496e 7369 6465 2042 6172 2028 2564 2922  Inside Bar (%d)"
-0001eae0: 2025 2069 0a20 2020 2020 2020 2020 2020   % i.           
-0001eaf0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-0001eb00: 7572 6e20 690a 2020 2020 2020 2020 2020  urn i.          
-0001eb10: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0001eb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001eb30: 7265 7475 726e 2030 0a20 2020 2020 2020  return 0.       
-0001eb40: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0001eb50: 2020 2020 2020 2020 2020 2069 6620 2244             if "D
-0001eb60: 6f77 6e22 2069 6e20 7361 7665 4469 6374  own" in saveDict
-0001eb70: 5b22 5472 656e 6422 5d20 616e 6420 280a  ["Trend"] and (.
-0001eb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001eb90: 2020 2020 2242 6561 7222 2069 6e20 7361      "Bear" in sa
-0001eba0: 7665 4469 6374 5b22 4d41 2d53 6967 6e61  veDict["MA-Signa
-0001ebb0: 6c22 5d20 6f72 2022 5265 7369 7374 2220  l"] or "Resist" 
-0001ebc0: 696e 2073 6176 6544 6963 745b 224d 412d  in saveDict["MA-
-0001ebd0: 5369 676e 616c 225d 0a20 2020 2020 2020  Signal"].       
-0001ebe0: 2020 2020 2020 2020 2029 3a0a 2020 2020           ):.    
-0001ebf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ec00: 6461 7461 203d 206f 7267 4461 7461 2e68  data = orgData.h
-0001ec10: 6561 6428 6929 0a20 2020 2020 2020 2020  ead(i).         
-0001ec20: 2020 2020 2020 2020 2020 2072 6566 4361             refCa
-0001ec30: 6e64 6c65 203d 2064 6174 612e 7461 696c  ndle = data.tail
-0001ec40: 2831 290a 2020 2020 2020 2020 2020 2020  (1).            
-0001ec50: 2020 2020 2020 2020 6966 2028 0a20 2020          if (.   
-0001ec60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ec70: 2020 2020 2028 6c65 6e28 6461 7461 2e48       (len(data.H
-0001ec80: 6967 685b 6461 7461 2e48 6967 6820 3e20  igh[data.High > 
-0001ec90: 7265 6643 616e 646c 652e 4869 6768 2e69  refCandle.High.i
-0001eca0: 7465 6d28 295d 2920 3d3d 2030 290a 2020  tem()]) == 0).  
-0001ecb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ecc0: 2020 2020 2020 616e 6420 286c 656e 2864        and (len(d
-0001ecd0: 6174 612e 4c6f 775b 6461 7461 2e4c 6f77  ata.Low[data.Low
-0001ece0: 203c 2072 6566 4361 6e64 6c65 2e4c 6f77   < refCandle.Low
-0001ecf0: 2e69 7465 6d28 295d 2920 3d3d 2030 290a  .item()]) == 0).
-0001ed00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ed10: 2020 2020 2020 2020 616e 6420 286c 656e          and (len
-0001ed20: 2864 6174 612e 4f70 656e 5b64 6174 612e  (data.Open[data.
-0001ed30: 4f70 656e 203e 2072 6566 4361 6e64 6c65  Open > refCandle
-0001ed40: 2e48 6967 682e 6974 656d 2829 5d29 203d  .High.item()]) =
-0001ed50: 3d20 3029 0a20 2020 2020 2020 2020 2020  = 0).           
-0001ed60: 2020 2020 2020 2020 2020 2020 2061 6e64               and
-0001ed70: 2028 6c65 6e28 6461 7461 2e43 6c6f 7365   (len(data.Close
-0001ed80: 5b64 6174 612e 436c 6f73 6520 3c20 7265  [data.Close < re
-0001ed90: 6643 616e 646c 652e 4c6f 772e 6974 656d  fCandle.Low.item
-0001eda0: 2829 5d29 203d 3d20 3029 0a20 2020 2020  ()]) == 0).     
-0001edb0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0001edc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001edd0: 2020 2020 2020 2020 2020 7363 7265 656e            screen
-0001ede0: 4469 6374 5b22 5061 7474 6572 6e22 5d20  Dict["Pattern"] 
-0001edf0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-0001ee00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ee10: 7361 7665 645b 305d 0a20 2020 2020 2020  saved[0].       
+0001ea90: 2020 202b 2028 2249 6e73 6964 6520 4261     + ("Inside Ba
+0001eaa0: 7220 2825 6429 2220 2520 6929 0a20 2020  r (%d)" % i).   
+0001eab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001eac0: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
+0001ead0: 5465 7874 2e45 4e44 0a20 2020 2020 2020  Text.END.       
+0001eae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001eaf0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+0001eb00: 2020 2020 2020 2020 2020 2073 6176 6544             saveD
+0001eb10: 6963 745b 2250 6174 7465 726e 225d 203d  ict["Pattern"] =
+0001eb20: 2073 6176 6564 5b31 5d20 2b20 2249 6e73   saved[1] + "Ins
+0001eb30: 6964 6520 4261 7220 2825 6429 2220 2520  ide Bar (%d)" % 
+0001eb40: 690a 2020 2020 2020 2020 2020 2020 2020  i.              
+0001eb50: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0001eb60: 2069 0a20 2020 2020 2020 2020 2020 2020   i.             
+0001eb70: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0001eb80: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+0001eb90: 7572 6e20 300a 2020 2020 2020 2020 2020  urn 0.          
+0001eba0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0001ebb0: 2020 2020 2020 2020 6966 2022 446f 776e          if "Down
+0001ebc0: 2220 696e 2073 6176 6544 6963 745b 2254  " in saveDict["T
+0001ebd0: 7265 6e64 225d 2061 6e64 2028 0a20 2020  rend"] and (.   
+0001ebe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ebf0: 2022 4265 6172 2220 696e 2073 6176 6544   "Bear" in saveD
+0001ec00: 6963 745b 224d 412d 5369 676e 616c 225d  ict["MA-Signal"]
+0001ec10: 206f 7220 2252 6573 6973 7422 2069 6e20   or "Resist" in 
+0001ec20: 7361 7665 4469 6374 5b22 4d41 2d53 6967  saveDict["MA-Sig
+0001ec30: 6e61 6c22 5d0a 2020 2020 2020 2020 2020  nal"].          
+0001ec40: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
+0001ec50: 2020 2020 2020 2020 2020 2020 2064 6174               dat
+0001ec60: 6120 3d20 6f72 6744 6174 612e 6865 6164  a = orgData.head
+0001ec70: 2869 290a 2020 2020 2020 2020 2020 2020  (i).            
+0001ec80: 2020 2020 2020 2020 7265 6643 616e 646c          refCandl
+0001ec90: 6520 3d20 6461 7461 2e74 6169 6c28 3129  e = data.tail(1)
+0001eca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001ecb0: 2020 2020 2069 6620 280a 2020 2020 2020       if (.      
+0001ecc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ecd0: 2020 286c 656e 2864 6174 612e 4869 6768    (len(data.High
+0001ece0: 5b64 6174 612e 4869 6768 203e 2072 6566  [data.High > ref
+0001ecf0: 4361 6e64 6c65 2e48 6967 682e 6974 656d  Candle.High.item
+0001ed00: 2829 5d29 203d 3d20 3029 0a20 2020 2020  ()]) == 0).     
+0001ed10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ed20: 2020 2061 6e64 2028 6c65 6e28 6461 7461     and (len(data
+0001ed30: 2e4c 6f77 5b64 6174 612e 4c6f 7720 3c20  .Low[data.Low < 
+0001ed40: 7265 6643 616e 646c 652e 4c6f 772e 6974  refCandle.Low.it
+0001ed50: 656d 2829 5d29 203d 3d20 3029 0a20 2020  em()]) == 0).   
+0001ed60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ed70: 2020 2020 2061 6e64 2028 6c65 6e28 6461       and (len(da
+0001ed80: 7461 2e4f 7065 6e5b 6461 7461 2e4f 7065  ta.Open[data.Ope
+0001ed90: 6e20 3e20 7265 6643 616e 646c 652e 4869  n > refCandle.Hi
+0001eda0: 6768 2e69 7465 6d28 295d 2920 3d3d 2030  gh.item()]) == 0
+0001edb0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001edc0: 2020 2020 2020 2020 2020 616e 6420 286c            and (l
+0001edd0: 656e 2864 6174 612e 436c 6f73 655b 6461  en(data.Close[da
+0001ede0: 7461 2e43 6c6f 7365 203c 2072 6566 4361  ta.Close < refCa
+0001edf0: 6e64 6c65 2e4c 6f77 2e69 7465 6d28 295d  ndle.Low.item()]
+0001ee00: 2920 3d3d 2030 290a 2020 2020 2020 2020  ) == 0).        
+0001ee10: 2020 2020 2020 2020 2020 2020 293a 0a20              ):. 
 0001ee20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ee30: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
-0001ee40: 2e42 4f4c 440a 2020 2020 2020 2020 2020  .BOLD.          
-0001ee50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ee60: 2020 2b20 636f 6c6f 7254 6578 742e 5741    + colorText.WA
-0001ee70: 524e 0a20 2020 2020 2020 2020 2020 2020  RN.             
-0001ee80: 2020 2020 2020 2020 2020 2020 2020 202b                 +
-0001ee90: 2028 2249 6e73 6964 6520 4261 7220 2825   ("Inside Bar (%
-0001eea0: 6429 2220 2520 6929 0a20 2020 2020 2020  d)" % i).       
-0001eeb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001eec0: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
-0001eed0: 2e45 4e44 0a20 2020 2020 2020 2020 2020  .END.           
-0001eee0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-0001eef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ef00: 2020 2020 2020 2073 6176 6544 6963 745b         saveDict[
-0001ef10: 2250 6174 7465 726e 225d 203d 2073 6176  "Pattern"] = sav
-0001ef20: 6564 5b31 5d20 2b20 2249 6e73 6964 6520  ed[1] + "Inside 
-0001ef30: 4261 7220 2825 6429 2220 2520 690a 2020  Bar (%d)" % i.  
-0001ef40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ef50: 2020 2020 2020 7265 7475 726e 2069 0a20        return i. 
-0001ef60: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0001ef70: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0001ef80: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0001ef90: 300a 2020 2020 2020 2020 7265 7475 726e  0.        return
-0001efa0: 2030 0a0a 2020 2020 2320 4669 6e64 2049   0..    # Find I
-0001efb0: 504f 2062 6173 650a 2020 2020 6465 6620  PO base.    def 
-0001efc0: 7661 6c69 6461 7465 4970 6f42 6173 6528  validateIpoBase(
-0001efd0: 7365 6c66 2c20 7374 6f63 6b2c 2064 662c  self, stock, df,
-0001efe0: 2073 6372 6565 6e44 6963 742c 2073 6176   screenDict, sav
-0001eff0: 6544 6963 742c 2070 6572 6365 6e74 6167  eDict, percentag
-0001f000: 653d 302e 3329 3a0a 2020 2020 2020 2020  e=0.3):.        
-0001f010: 6966 2064 6620 6973 204e 6f6e 6520 6f72  if df is None or
-0001f020: 206c 656e 2864 6629 203d 3d20 303a 0a20   len(df) == 0:. 
-0001f030: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0001f040: 6e20 4661 6c73 650a 2020 2020 2020 2020  n False.        
-0001f050: 6461 7461 203d 2064 662e 636f 7079 2829  data = df.copy()
-0001f060: 0a20 2020 2020 2020 206c 6973 7469 6e67  .        listing
-0001f070: 5072 6963 6520 3d20 6461 7461 5b3a 3a2d  Price = data[::-
-0001f080: 315d 2e68 6561 6428 3129 5b22 4f70 656e  1].head(1)["Open
-0001f090: 225d 2e69 6c6f 635b 305d 0a20 2020 2020  "].iloc[0].     
-0001f0a0: 2020 2063 7572 7265 6e74 5072 6963 6520     currentPrice 
-0001f0b0: 3d20 6461 7461 2e68 6561 6428 3129 5b22  = data.head(1)["
-0001f0c0: 436c 6f73 6522 5d2e 696c 6f63 5b30 5d0a  Close"].iloc[0].
-0001f0d0: 2020 2020 2020 2020 4154 4820 3d20 6461          ATH = da
-0001f0e0: 7461 2e64 6573 6372 6962 6528 295b 2248  ta.describe()["H
-0001f0f0: 6967 6822 5d5b 226d 6178 225d 0a20 2020  igh"]["max"].   
-0001f100: 2020 2020 2069 6620 4154 4820 3e20 286c       if ATH > (l
-0001f110: 6973 7469 6e67 5072 6963 6520 2b20 286c  istingPrice + (l
-0001f120: 6973 7469 6e67 5072 6963 6520 2a20 7065  istingPrice * pe
-0001f130: 7263 656e 7461 6765 2929 3a0a 2020 2020  rcentage)):.    
-0001f140: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-0001f150: 616c 7365 0a20 2020 2020 2020 2061 7761  alse.        awa
-0001f160: 7920 3d20 726f 756e 6428 2828 6375 7272  y = round(((curr
-0001f170: 656e 7450 7269 6365 202d 206c 6973 7469  entPrice - listi
-0001f180: 6e67 5072 6963 6529 202f 206c 6973 7469  ngPrice) / listi
-0001f190: 6e67 5072 6963 6529 202a 2031 3030 2c20  ngPrice) * 100, 
-0001f1a0: 3129 0a20 2020 2020 2020 2069 6620 280a  1).        if (.
-0001f1b0: 2020 2020 2020 2020 2020 2020 286c 6973              (lis
-0001f1c0: 7469 6e67 5072 6963 6520 2d20 286c 6973  tingPrice - (lis
-0001f1d0: 7469 6e67 5072 6963 6520 2a20 7065 7263  tingPrice * perc
-0001f1e0: 656e 7461 6765 2929 0a20 2020 2020 2020  entage)).       
-0001f1f0: 2020 2020 203c 3d20 6375 7272 656e 7450       <= currentP
-0001f200: 7269 6365 0a20 2020 2020 2020 2020 2020  rice.           
-0001f210: 203c 3d20 286c 6973 7469 6e67 5072 6963   <= (listingPric
-0001f220: 6520 2b20 286c 6973 7469 6e67 5072 6963  e + (listingPric
-0001f230: 6520 2a20 7065 7263 656e 7461 6765 2929  e * percentage))
-0001f240: 0a20 2020 2020 2020 2029 3a0a 2020 2020  .        ):.    
-0001f250: 2020 2020 2020 2020 7361 7665 6420 3d20          saved = 
-0001f260: 7365 6c66 2e66 696e 6443 7572 7265 6e74  self.findCurrent
-0001f270: 5361 7665 6456 616c 7565 2873 6372 6565  SavedValue(scree
-0001f280: 6e44 6963 742c 2073 6176 6544 6963 742c  nDict, saveDict,
-0001f290: 2022 5061 7474 6572 6e22 290a 2020 2020   "Pattern").    
-0001f2a0: 2020 2020 2020 2020 6966 2061 7761 7920          if away 
-0001f2b0: 3e20 303a 0a20 2020 2020 2020 2020 2020  > 0:.           
-0001f2c0: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
-0001f2d0: 2250 6174 7465 726e 225d 203d 2028 0a20  "Pattern"] = (. 
-0001f2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f2f0: 2020 2073 6176 6564 5b30 5d20 0a20 2020     saved[0] .   
-0001f300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f310: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
-0001f320: 440a 2020 2020 2020 2020 2020 2020 2020  D.              
-0001f330: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
-0001f340: 742e 4752 4545 4e0a 2020 2020 2020 2020  t.GREEN.        
-0001f350: 2020 2020 2020 2020 2020 2020 2b20 6622              + f"
-0001f360: 4950 4f20 4261 7365 2028 7b61 7761 797d  IPO Base ({away}
-0001f370: 2025 2922 0a20 2020 2020 2020 2020 2020   %)".           
-0001f380: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
-0001f390: 5465 7874 2e45 4e44 0a20 2020 2020 2020  Text.END.       
-0001f3a0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0001f3b0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0001f3c0: 2020 2020 2020 2020 2020 2020 2073 6372               scr
-0001f3d0: 6565 6e44 6963 745b 2250 6174 7465 726e  eenDict["Pattern
-0001f3e0: 225d 203d 2028 0a20 2020 2020 2020 2020  "] = (.         
-0001f3f0: 2020 2020 2020 2020 2020 2073 6176 6564             saved
-0001f400: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
-0001f410: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
-0001f420: 6578 742e 424f 4c44 0a20 2020 2020 2020  ext.BOLD.       
-0001f430: 2020 2020 2020 2020 2020 2020 202b 2063               + c
-0001f440: 6f6c 6f72 5465 7874 2e47 5245 454e 0a20  olorText.GREEN. 
-0001f450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f460: 2020 202b 2022 4950 4f20 4261 7365 2022     + "IPO Base "
-0001f470: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001f480: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
-0001f490: 2e46 4149 4c0a 2020 2020 2020 2020 2020  .FAIL.          
-0001f4a0: 2020 2020 2020 2020 2020 2b20 6622 287b            + f"({
-0001f4b0: 6177 6179 7d20 2529 220a 2020 2020 2020  away} %)".      
-0001f4c0: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-0001f4d0: 636f 6c6f 7254 6578 742e 454e 440a 2020  colorText.END.  
-0001f4e0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-0001f4f0: 2020 2020 2020 2020 2020 2020 7361 7665              save
-0001f500: 4469 6374 5b22 5061 7474 6572 6e22 5d20  Dict["Pattern"] 
-0001f510: 3d20 7361 7665 645b 315d 202b 2066 2249  = saved[1] + f"I
-0001f520: 504f 2042 6173 6520 287b 6177 6179 7d20  PO Base ({away} 
-0001f530: 2529 220a 2020 2020 2020 2020 2020 2020  %)".            
-0001f540: 7265 7475 726e 2054 7275 650a 2020 2020  return True.    
-0001f550: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-0001f560: 0a0a 2020 2020 2340 6d65 6173 7572 655f  ..    #@measure_
-0001f570: 7469 6d65 0a20 2020 2023 2056 616c 6964  time.    # Valid
-0001f580: 6174 6520 4c6f 7265 6e74 7a69 616e 2043  ate Lorentzian C
-0001f590: 6c61 7373 6966 6963 6174 696f 6e20 7369  lassification si
-0001f5a0: 676e 616c 0a20 2020 2064 6566 2076 616c  gnal.    def val
-0001f5b0: 6964 6174 654c 6f72 656e 747a 6961 6e28  idateLorentzian(
-0001f5c0: 7365 6c66 2c20 6466 2c20 7363 7265 656e  self, df, screen
-0001f5d0: 4469 6374 2c20 7361 7665 4469 6374 2c20  Dict, saveDict, 
-0001f5e0: 6c6f 6f6b 466f 723d 3329 3a0a 2020 2020  lookFor=3):.    
-0001f5f0: 2020 2020 6966 2064 6620 6973 204e 6f6e      if df is Non
-0001f600: 6520 6f72 206c 656e 2864 6629 203d 3d20  e or len(df) == 
-0001f610: 303a 0a20 2020 2020 2020 2020 2020 2072  0:.            r
-0001f620: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
-0001f630: 2020 2020 6461 7461 203d 2064 662e 636f      data = df.co
-0001f640: 7079 2829 0a20 2020 2020 2020 2023 206c  py().        # l
-0001f650: 6f6f 6b46 6f72 3a20 312d 4275 792c 2032  ookFor: 1-Buy, 2
-0001f660: 2d53 656c 6c2c 2033 2d41 6e79 0a20 2020  -Sell, 3-Any.   
-0001f670: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
-0001f680: 5b3a 3a2d 315d 2020 2320 5265 7665 7273  [::-1]  # Revers
-0001f690: 6520 7468 6520 6461 7461 6672 616d 650a  e the dataframe.
-0001f6a0: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
-0001f6b0: 6174 612e 7265 6e61 6d65 280a 2020 2020  ata.rename(.    
-0001f6c0: 2020 2020 2020 2020 636f 6c75 6d6e 733d          columns=
-0001f6d0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-0001f6e0: 2020 224f 7065 6e22 3a20 226f 7065 6e22    "Open": "open"
-0001f6f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0001f700: 2020 2243 6c6f 7365 223a 2022 636c 6f73    "Close": "clos
-0001f710: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
-0001f720: 2020 2020 2248 6967 6822 3a20 2268 6967      "High": "hig
-0001f730: 6822 2c0a 2020 2020 2020 2020 2020 2020  h",.            
-0001f740: 2020 2020 224c 6f77 223a 2022 6c6f 7722      "Low": "low"
-0001f750: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0001f760: 2020 2256 6f6c 756d 6522 3a20 2276 6f6c    "Volume": "vol
-0001f770: 756d 6522 2c0a 2020 2020 2020 2020 2020  ume",.          
-0001f780: 2020 7d0a 2020 2020 2020 2020 290a 2020    }.        ).  
-0001f790: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-0001f7a0: 2020 2020 2020 2077 6974 6820 5375 7070         with Supp
-0001f7b0: 7265 7373 4f75 7470 7574 2873 7570 7072  ressOutput(suppr
-0001f7c0: 6573 735f 7374 646f 7574 3d54 7275 652c  ess_stdout=True,
-0001f7d0: 2073 7570 7072 6573 735f 7374 6465 7272   suppress_stderr
-0001f7e0: 3d54 7275 6529 3a0a 2020 2020 2020 2020  =True):.        
-0001f7f0: 2020 2020 2020 2020 6c63 203d 2061 7461          lc = ata
-0001f800: 2e4c 6f72 656e 747a 6961 6e43 6c61 7373  .LorentzianClass
-0001f810: 6966 6963 6174 696f 6e28 6461 7461 3d64  ification(data=d
-0001f820: 6174 6129 0a20 2020 2020 2020 2020 2020  ata).           
-0001f830: 2073 6176 6564 203d 2073 656c 662e 6669   saved = self.fi
-0001f840: 6e64 4375 7272 656e 7453 6176 6564 5661  ndCurrentSavedVa
-0001f850: 6c75 6528 7363 7265 656e 4469 6374 2c20  lue(screenDict, 
-0001f860: 7361 7665 4469 6374 2c20 2250 6174 7465  saveDict, "Patte
-0001f870: 726e 2229 0a20 2020 2020 2020 2020 2020  rn").           
-0001f880: 2069 6620 6c63 2e64 662e 696c 6f63 5b2d   if lc.df.iloc[-
-0001f890: 315d 5b22 6973 4e65 7742 7579 5369 676e  1]["isNewBuySign
-0001f8a0: 616c 225d 3a0a 2020 2020 2020 2020 2020  al"]:.          
-0001f8b0: 2020 2020 2020 7363 7265 656e 4469 6374        screenDict
-0001f8c0: 5b22 5061 7474 6572 6e22 5d20 3d20 280a  ["Pattern"] = (.
-0001f8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f8e0: 2020 2020 7361 7665 645b 305d 202b 2063      saved[0] + c
-0001f8f0: 6f6c 6f72 5465 7874 2e42 4f4c 4420 2b20  olorText.BOLD + 
-0001f900: 636f 6c6f 7254 6578 742e 4752 4545 4e20  colorText.GREEN 
-0001f910: 2b20 224c 6f72 656e 747a 6961 6e2d 4275  + "Lorentzian-Bu
-0001f920: 7922 202b 2063 6f6c 6f72 5465 7874 2e45  y" + colorText.E
-0001f930: 4e44 0a20 2020 2020 2020 2020 2020 2020  ND.             
-0001f940: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0001f950: 2020 2020 2073 6176 6544 6963 745b 2250       saveDict["P
-0001f960: 6174 7465 726e 225d 203d 2073 6176 6564  attern"] = saved
-0001f970: 5b31 5d20 2b20 224c 6f72 656e 747a 6961  [1] + "Lorentzia
-0001f980: 6e2d 4275 7922 0a20 2020 2020 2020 2020  n-Buy".         
-0001f990: 2020 2020 2020 2069 6620 6c6f 6f6b 466f         if lookFo
-0001f9a0: 7220 213d 2032 3a20 2320 4e6f 7420 5365  r != 2: # Not Se
-0001f9b0: 6c6c 0a20 2020 2020 2020 2020 2020 2020  ll.             
-0001f9c0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-0001f9d0: 7565 0a20 2020 2020 2020 2020 2020 2065  ue.            e
-0001f9e0: 6c69 6620 6c63 2e64 662e 696c 6f63 5b2d  lif lc.df.iloc[-
-0001f9f0: 315d 5b22 6973 4e65 7753 656c 6c53 6967  1]["isNewSellSig
-0001fa00: 6e61 6c22 5d3a 0a20 2020 2020 2020 2020  nal"]:.         
-0001fa10: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
-0001fa20: 745b 2250 6174 7465 726e 225d 203d 2028  t["Pattern"] = (
-0001fa30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001fa40: 2020 2020 2073 6176 6564 5b30 5d20 2b20       saved[0] + 
-0001fa50: 636f 6c6f 7254 6578 742e 424f 4c44 202b  colorText.BOLD +
-0001fa60: 2063 6f6c 6f72 5465 7874 2e46 4149 4c20   colorText.FAIL 
-0001fa70: 2b20 224c 6f72 656e 747a 6961 6e2d 5365  + "Lorentzian-Se
-0001fa80: 6c6c 2220 2b20 636f 6c6f 7254 6578 742e  ll" + colorText.
-0001fa90: 454e 440a 2020 2020 2020 2020 2020 2020  END.            
-0001faa0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-0001fab0: 2020 2020 2020 7361 7665 4469 6374 5b22        saveDict["
-0001fac0: 5061 7474 6572 6e22 5d20 3d20 7361 7665  Pattern"] = save
-0001fad0: 645b 315d 202b 2022 4c6f 7265 6e74 7a69  d[1] + "Lorentzi
-0001fae0: 616e 2d53 656c 6c22 0a20 2020 2020 2020  an-Sell".       
-0001faf0: 2020 2020 2020 2020 2069 6620 6c6f 6f6b           if look
-0001fb00: 466f 7220 213d 2031 3a20 2320 4e6f 7420  For != 1: # Not 
-0001fb10: 4275 790a 2020 2020 2020 2020 2020 2020  Buy.            
-0001fb20: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-0001fb30: 7275 650a 2020 2020 2020 2020 6578 6365  rue.        exce
-0001fb40: 7074 2045 7863 6570 7469 6f6e 3a20 2023  pt Exception:  #
-0001fb50: 2070 7261 676d 613a 206e 6f20 636f 7665   pragma: no cove
-0001fb60: 720a 2020 2020 2020 2020 2020 2020 2320  r.            # 
-0001fb70: 5661 6c75 6545 7272 6f72 3a20 6f70 6572  ValueError: oper
-0001fb80: 616e 6473 2063 6f75 6c64 206e 6f74 2062  ands could not b
-0001fb90: 6520 6272 6f61 6463 6173 7420 746f 6765  e broadcast toge
-0001fba0: 7468 6572 2077 6974 6820 7368 6170 6573  ther with shapes
-0001fbb0: 2028 3230 2c29 2028 3236 2c29 0a20 2020   (20,) (26,).   
-0001fbc0: 2020 2020 2020 2020 2023 2046 696c 6520           # File 
-0001fbd0: 222f 6f70 742f 686f 6d65 6272 6577 2f6c  "/opt/homebrew/l
-0001fbe0: 6962 2f70 7974 686f 6e33 2e31 312f 7369  ib/python3.11/si
-0001fbf0: 7465 2d70 6163 6b61 6765 732f 6164 7661  te-packages/adva
-0001fc00: 6e63 6564 5f74 612f 4c6f 7265 6e74 7a69  nced_ta/Lorentzi
-0001fc10: 616e 436c 6173 7369 6669 6361 7469 6f6e  anClassification
-0001fc20: 2f43 6c61 7373 6966 6965 722e 7079 222c  /Classifier.py",
-0001fc30: 206c 696e 6520 3138 362c 2069 6e20 5f5f   line 186, in __
-0001fc40: 696e 6974 5f5f 0a20 2020 2020 2020 2020  init__.         
-0001fc50: 2020 2023 2046 696c 6520 222f 6f70 742f     # File "/opt/
-0001fc60: 686f 6d65 6272 6577 2f6c 6962 2f70 7974  homebrew/lib/pyt
-0001fc70: 686f 6e33 2e31 312f 7369 7465 2d70 6163  hon3.11/site-pac
-0001fc80: 6b61 6765 732f 6164 7661 6e63 6564 5f74  kages/advanced_t
-0001fc90: 612f 4c6f 7265 6e74 7a69 616e 436c 6173  a/LorentzianClas
-0001fca0: 7369 6669 6361 7469 6f6e 2f43 6c61 7373  sification/Class
-0001fcb0: 6966 6965 722e 7079 222c 206c 696e 6520  ifier.py", line 
-0001fcc0: 3339 352c 2069 6e20 5f5f 636c 6173 7369  395, in __classi
-0001fcd0: 6679 0a20 2020 2020 2020 2020 2020 2023  fy.            #
-0001fce0: 2046 696c 6520 222f 6f70 742f 686f 6d65   File "/opt/home
-0001fcf0: 6272 6577 2f6c 6962 2f70 7974 686f 6e33  brew/lib/python3
-0001fd00: 2e31 312f 7369 7465 2d70 6163 6b61 6765  .11/site-package
-0001fd10: 732f 7061 6e64 6173 2f63 6f72 652f 6f70  s/pandas/core/op
-0001fd20: 732f 636f 6d6d 6f6e 2e70 7922 2c20 6c69  s/common.py", li
-0001fd30: 6e65 2037 362c 2069 6e20 6e65 775f 6d65  ne 76, in new_me
-0001fd40: 7468 6f64 0a20 2020 2020 2020 2020 2020  thod.           
-0001fd50: 2023 2046 696c 6520 222f 6f70 742f 686f   # File "/opt/ho
-0001fd60: 6d65 6272 6577 2f6c 6962 2f70 7974 686f  mebrew/lib/pytho
-0001fd70: 6e33 2e31 312f 7369 7465 2d70 6163 6b61  n3.11/site-packa
-0001fd80: 6765 732f 7061 6e64 6173 2f63 6f72 652f  ges/pandas/core/
-0001fd90: 6172 7261 796c 696b 652e 7079 222c 206c  arraylike.py", l
-0001fda0: 696e 6520 3730 2c20 696e 205f 5f61 6e64  ine 70, in __and
-0001fdb0: 5f5f 0a20 2020 2020 2020 2020 2020 2023  __.            #
-0001fdc0: 2046 696c 6520 222f 6f70 742f 686f 6d65   File "/opt/home
-0001fdd0: 6272 6577 2f6c 6962 2f70 7974 686f 6e33  brew/lib/python3
-0001fde0: 2e31 312f 7369 7465 2d70 6163 6b61 6765  .11/site-package
-0001fdf0: 732f 7061 6e64 6173 2f63 6f72 652f 7365  s/pandas/core/se
-0001fe00: 7269 6573 2e70 7922 2c20 6c69 6e65 2035  ries.py", line 5
-0001fe10: 3831 302c 2069 6e20 5f6c 6f67 6963 616c  810, in _logical
-0001fe20: 5f6d 6574 686f 640a 2020 2020 2020 2020  _method.        
-0001fe30: 2020 2020 2320 4669 6c65 2022 2f6f 7074      # File "/opt
-0001fe40: 2f68 6f6d 6562 7265 772f 6c69 622f 7079  /homebrew/lib/py
-0001fe50: 7468 6f6e 332e 3131 2f73 6974 652d 7061  thon3.11/site-pa
-0001fe60: 636b 6167 6573 2f70 616e 6461 732f 636f  ckages/pandas/co
-0001fe70: 7265 2f6f 7073 2f61 7272 6179 5f6f 7073  re/ops/array_ops
-0001fe80: 2e70 7922 2c20 6c69 6e65 2034 3536 2c20  .py", line 456, 
-0001fe90: 696e 206c 6f67 6963 616c 5f6f 700a 2020  in logical_op.  
-0001fea0: 2020 2020 2020 2020 2020 2320 4669 6c65            # File
-0001feb0: 2022 2f6f 7074 2f68 6f6d 6562 7265 772f   "/opt/homebrew/
-0001fec0: 6c69 622f 7079 7468 6f6e 332e 3131 2f73  lib/python3.11/s
-0001fed0: 6974 652d 7061 636b 6167 6573 2f70 616e  ite-packages/pan
-0001fee0: 6461 732f 636f 7265 2f6f 7073 2f61 7272  das/core/ops/arr
-0001fef0: 6179 5f6f 7073 2e70 7922 2c20 6c69 6e65  ay_ops.py", line
-0001ff00: 2033 3634 2c20 696e 206e 615f 6c6f 6769   364, in na_logi
-0001ff10: 6361 6c5f 6f70 0a20 2020 2020 2020 2020  cal_op.         
-0001ff20: 2020 2023 2073 656c 662e 6465 6661 756c     # self.defaul
-0001ff30: 745f 6c6f 6767 6572 2e64 6562 7567 2865  t_logger.debug(e
-0001ff40: 2c20 6578 635f 696e 666f 3d54 7275 6529  , exc_info=True)
-0001ff50: 0a20 2020 2020 2020 2020 2020 2070 6173  .            pas
-0001ff60: 730a 2020 2020 2020 2020 7265 7475 726e  s.        return
-0001ff70: 2046 616c 7365 0a0a 2020 2020 2320 7661   False..    # va
-0001ff80: 6c69 6461 7465 2069 6620 7468 6520 7374  lidate if the st
-0001ff90: 6f63 6b20 6861 7320 6265 656e 2068 6176  ock has been hav
-0001ffa0: 696e 6720 6c6f 7765 7220 6c6f 7773 2c20  ing lower lows, 
-0001ffb0: 6c6f 7765 7220 6869 6768 730a 2020 2020  lower highs.    
-0001ffc0: 6465 6620 7661 6c69 6461 7465 4c6f 7765  def validateLowe
-0001ffd0: 7248 6967 6873 4c6f 7765 724c 6f77 7328  rHighsLowerLows(
-0001ffe0: 7365 6c66 2c20 6466 293a 0a20 2020 2020  self, df):.     
-0001fff0: 2020 2069 6620 6466 2069 7320 4e6f 6e65     if df is None
-00020000: 206f 7220 6c65 6e28 6466 2920 3d3d 2030   or len(df) == 0
-00020010: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00020020: 7475 726e 2046 616c 7365 0a20 2020 2020  turn False.     
-00020030: 2020 2064 6174 6120 3d20 6466 2e63 6f70     data = df.cop
-00020040: 7928 290a 2020 2020 2020 2020 6461 7930  y().        day0
-00020050: 203d 2064 6174 610a 2020 2020 2020 2020   = data.        
-00020060: 6461 7931 203d 2064 6174 615b 313a 5d0a  day1 = data[1:].
-00020070: 2020 2020 2020 2020 6461 7932 203d 2064          day2 = d
-00020080: 6174 615b 323a 5d0a 2020 2020 2020 2020  ata[2:].        
-00020090: 6461 7933 203d 2064 6174 615b 333a 5d0a  day3 = data[3:].
-000200a0: 2020 2020 2020 2020 6c6f 7765 7248 6967          lowerHig
-000200b0: 6873 203d 2028 0a20 2020 2020 2020 2020  hs = (.         
-000200c0: 2020 2028 6461 7930 5b22 4869 6768 225d     (day0["High"]
-000200d0: 2e69 6c6f 635b 305d 203c 2064 6179 315b  .iloc[0] < day1[
-000200e0: 2248 6967 6822 5d2e 696c 6f63 5b30 5d29  "High"].iloc[0])
-000200f0: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
-00020100: 2028 6461 7931 5b22 4869 6768 225d 2e69   (day1["High"].i
-00020110: 6c6f 635b 305d 203c 2064 6179 325b 2248  loc[0] < day2["H
-00020120: 6967 6822 5d2e 696c 6f63 5b30 5d29 0a20  igh"].iloc[0]). 
-00020130: 2020 2020 2020 2020 2020 2061 6e64 2028             and (
-00020140: 6461 7932 5b22 4869 6768 225d 2e69 6c6f  day2["High"].ilo
-00020150: 635b 305d 203c 2064 6179 335b 2248 6967  c[0] < day3["Hig
-00020160: 6822 5d2e 696c 6f63 5b30 5d29 0a20 2020  h"].iloc[0]).   
-00020170: 2020 2020 2029 0a20 2020 2020 2020 206c       ).        l
-00020180: 6f77 6572 4c6f 7773 203d 2028 0a20 2020  owerLows = (.   
-00020190: 2020 2020 2020 2020 2028 6461 7930 5b22           (day0["
-000201a0: 4c6f 7722 5d2e 696c 6f63 5b30 5d20 3c20  Low"].iloc[0] < 
-000201b0: 6461 7931 5b22 4c6f 7722 5d2e 696c 6f63  day1["Low"].iloc
-000201c0: 5b30 5d29 0a20 2020 2020 2020 2020 2020  [0]).           
-000201d0: 2061 6e64 2028 6461 7931 5b22 4c6f 7722   and (day1["Low"
-000201e0: 5d2e 696c 6f63 5b30 5d20 3c20 6461 7932  ].iloc[0] < day2
-000201f0: 5b22 4c6f 7722 5d2e 696c 6f63 5b30 5d29  ["Low"].iloc[0])
-00020200: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
-00020210: 2028 6461 7932 5b22 4c6f 7722 5d2e 696c   (day2["Low"].il
-00020220: 6f63 5b30 5d20 3c20 6461 7933 5b22 4c6f  oc[0] < day3["Lo
-00020230: 7722 5d2e 696c 6f63 5b30 5d29 0a20 2020  w"].iloc[0]).   
-00020240: 2020 2020 2029 0a20 2020 2020 2020 2068       ).        h
-00020250: 6967 6865 7252 5349 203d 2028 0a20 2020  igherRSI = (.   
-00020260: 2020 2020 2020 2020 2028 6461 7930 5b22           (day0["
-00020270: 5253 4922 5d2e 696c 6f63 5b30 5d20 3c20  RSI"].iloc[0] < 
-00020280: 6461 7931 5b22 5253 4922 5d2e 696c 6f63  day1["RSI"].iloc
-00020290: 5b30 5d29 0a20 2020 2020 2020 2020 2020  [0]).           
-000202a0: 2061 6e64 2028 6461 7931 5b22 5253 4922   and (day1["RSI"
-000202b0: 5d2e 696c 6f63 5b30 5d20 3c20 6461 7932  ].iloc[0] < day2
-000202c0: 5b22 5253 4922 5d2e 696c 6f63 5b30 5d29  ["RSI"].iloc[0])
-000202d0: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
-000202e0: 2028 6461 7932 5b22 5253 4922 5d2e 696c   (day2["RSI"].il
-000202f0: 6f63 5b30 5d20 3c20 6461 7933 5b22 5253  oc[0] < day3["RS
-00020300: 4922 5d2e 696c 6f63 5b30 5d29 0a20 2020  I"].iloc[0]).   
-00020310: 2020 2020 2020 2020 2061 6e64 2064 6179           and day
-00020320: 305b 2252 5349 225d 2e69 6c6f 635b 305d  0["RSI"].iloc[0]
-00020330: 203e 3d20 3530 0a20 2020 2020 2020 2029   >= 50.        )
-00020340: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00020350: 6c6f 7765 7248 6967 6873 2061 6e64 206c  lowerHighs and l
-00020360: 6f77 6572 4c6f 7773 2061 6e64 2068 6967  owerLows and hig
-00020370: 6865 7252 5349 0a0a 2020 2020 2320 5661  herRSI..    # Va
-00020380: 6c69 6461 7465 2069 6620 7265 6365 6e74  lidate if recent
-00020390: 2076 6f6c 756d 6520 6973 206c 6f77 6573   volume is lowes
-000203a0: 7420 6f66 206c 6173 7420 274e 2720 4461  t of last 'N' Da
-000203b0: 7973 0a20 2020 2064 6566 2076 616c 6964  ys.    def valid
-000203c0: 6174 654c 6f77 6573 7456 6f6c 756d 6528  ateLowestVolume(
-000203d0: 7365 6c66 2c20 6466 2c20 6461 7973 466f  self, df, daysFo
-000203e0: 724c 6f77 6573 7456 6f6c 756d 6529 3a0a  rLowestVolume):.
-000203f0: 2020 2020 2020 2020 6966 2064 6620 6973          if df is
-00020400: 204e 6f6e 6520 6f72 206c 656e 2864 6629   None or len(df)
-00020410: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
-00020420: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-00020430: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
-00020440: 662e 636f 7079 2829 0a20 2020 2020 2020  f.copy().       
-00020450: 2064 6174 6120 3d20 6461 7461 2e66 696c   data = data.fil
-00020460: 6c6e 6128 3029 0a20 2020 2020 2020 2064  lna(0).        d
-00020470: 6174 6120 3d20 6461 7461 2e72 6570 6c61  ata = data.repla
-00020480: 6365 285b 6e70 2e69 6e66 2c20 2d6e 702e  ce([np.inf, -np.
-00020490: 696e 665d 2c20 3029 0a20 2020 2020 2020  inf], 0).       
-000204a0: 2069 6620 6461 7973 466f 724c 6f77 6573   if daysForLowes
-000204b0: 7456 6f6c 756d 6520 6973 204e 6f6e 653a  tVolume is None:
-000204c0: 0a20 2020 2020 2020 2020 2020 2064 6179  .            day
-000204d0: 7346 6f72 4c6f 7765 7374 566f 6c75 6d65  sForLowestVolume
-000204e0: 203d 2033 300a 2020 2020 2020 2020 6966   = 30.        if
-000204f0: 206c 656e 2864 6174 6129 203c 2064 6179   len(data) < day
-00020500: 7346 6f72 4c6f 7765 7374 566f 6c75 6d65  sForLowestVolume
-00020510: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00020520: 7475 726e 2046 616c 7365 0a20 2020 2020  turn False.     
-00020530: 2020 2064 6174 6120 3d20 6461 7461 2e68     data = data.h
-00020540: 6561 6428 6461 7973 466f 724c 6f77 6573  ead(daysForLowes
-00020550: 7456 6f6c 756d 6529 0a20 2020 2020 2020  tVolume).       
-00020560: 2072 6563 656e 7420 3d20 6461 7461 2e68   recent = data.h
-00020570: 6561 6428 3129 0a20 2020 2020 2020 2069  ead(1).        i
-00020580: 6620 6c65 6e28 7265 6365 6e74 2920 3c20  f len(recent) < 
-00020590: 313a 0a20 2020 2020 2020 2020 2020 2072  1:.            r
-000205a0: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
-000205b0: 2020 2020 6966 2028 7265 6365 6e74 5b22      if (recent["
-000205c0: 566f 6c75 6d65 225d 2e69 6c6f 635b 305d  Volume"].iloc[0]
-000205d0: 203c 3d20 6461 7461 2e64 6573 6372 6962   <= data.describ
-000205e0: 6528 295b 2256 6f6c 756d 6522 5d5b 226d  e()["Volume"]["m
-000205f0: 696e 225d 2920 616e 6420 7265 6365 6e74  in"]) and recent
-00020600: 5b0a 2020 2020 2020 2020 2020 2020 2256  [.            "V
-00020610: 6f6c 756d 6522 0a20 2020 2020 2020 205d  olume".        ]
-00020620: 5b30 5d20 213d 206e 702e 6e61 6e3a 0a20  [0] != np.nan:. 
-00020630: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00020640: 6e20 5472 7565 0a20 2020 2020 2020 2072  n True.        r
-00020650: 6574 7572 6e20 4661 6c73 650a 0a20 2020  eturn False..   
-00020660: 2023 2056 616c 6964 6174 6520 4c54 5020   # Validate LTP 
-00020670: 7769 7468 696e 206c 696d 6974 730a 2020  within limits.  
-00020680: 2020 6465 6620 7661 6c69 6461 7465 4c54    def validateLT
-00020690: 5028 7365 6c66 2c20 6466 2c20 7363 7265  P(self, df, scre
-000206a0: 656e 4469 6374 2c20 7361 7665 4469 6374  enDict, saveDict
-000206b0: 2c20 6d69 6e4c 5450 3d4e 6f6e 652c 206d  , minLTP=None, m
-000206c0: 6178 4c54 503d 4e6f 6e65 2c6d 696e 4368  axLTP=None,minCh
-000206d0: 616e 6765 3d30 293a 0a20 2020 2020 2020  ange=0):.       
-000206e0: 2064 6174 6120 3d20 6466 2e63 6f70 7928   data = df.copy(
-000206f0: 290a 2020 2020 2020 2020 6c74 7056 616c  ).        ltpVal
-00020700: 6964 203d 2046 616c 7365 0a20 2020 2020  id = False.     
-00020710: 2020 2069 6620 6d69 6e4c 5450 2069 7320     if minLTP is 
-00020720: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00020730: 2020 6d69 6e4c 5450 203d 2073 656c 662e    minLTP = self.
-00020740: 636f 6e66 6967 4d61 6e61 6765 722e 6d69  configManager.mi
-00020750: 6e4c 5450 0a20 2020 2020 2020 2069 6620  nLTP.        if 
-00020760: 6d61 784c 5450 2069 7320 4e6f 6e65 3a0a  maxLTP is None:.
-00020770: 2020 2020 2020 2020 2020 2020 6d61 784c              maxL
-00020780: 5450 203d 2073 656c 662e 636f 6e66 6967  TP = self.config
-00020790: 4d61 6e61 6765 722e 6d61 784c 5450 0a20  Manager.maxLTP. 
-000207a0: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
-000207b0: 7461 2e66 696c 6c6e 6128 3029 0a20 2020  ta.fillna(0).   
-000207c0: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
-000207d0: 2e72 6570 6c61 6365 285b 6e70 2e69 6e66  .replace([np.inf
-000207e0: 2c20 2d6e 702e 696e 665d 2c20 3029 0a20  , -np.inf], 0). 
-000207f0: 2020 2020 2020 2072 6563 656e 7420 3d20         recent = 
-00020800: 6461 7461 2e68 6561 6428 3129 0a0a 2020  data.head(1)..  
-00020810: 2020 2020 2020 7063 745f 6368 616e 6765        pct_change
-00020820: 203d 2028 6461 7461 5b3a 3a2d 315d 5b22   = (data[::-1]["
-00020830: 436c 6f73 6522 5d2e 7063 745f 6368 616e  Close"].pct_chan
-00020840: 6765 2829 202a 2031 3030 292e 696c 6f63  ge() * 100).iloc
-00020850: 5b2d 315d 0a20 2020 2020 2020 2069 6620  [-1].        if 
-00020860: 7063 745f 6368 616e 6765 203d 3d20 6e70  pct_change == np
-00020870: 2e69 6e66 206f 7220 7063 745f 6368 616e  .inf or pct_chan
-00020880: 6765 203d 3d20 2d6e 702e 696e 663a 0a20  ge == -np.inf:. 
-00020890: 2020 2020 2020 2020 2020 2070 6374 5f63             pct_c
-000208a0: 6861 6e67 6520 3d20 300a 2020 2020 2020  hange = 0.      
-000208b0: 2020 7063 745f 7361 7665 203d 2022 252e    pct_save = "%.
-000208c0: 3166 2525 2220 2520 7063 745f 6368 616e  1f%%" % pct_chan
-000208d0: 6765 0a20 2020 2020 2020 2069 6620 7063  ge.        if pc
-000208e0: 745f 6368 616e 6765 203e 2030 2e32 3a0a  t_change > 0.2:.
-000208f0: 2020 2020 2020 2020 2020 2020 7063 745f              pct_
-00020900: 6368 616e 6765 203d 2063 6f6c 6f72 5465  change = colorTe
-00020910: 7874 2e47 5245 454e 202b 2028 2225 2e31  xt.GREEN + ("%.1
-00020920: 6625 2522 2025 2070 6374 5f63 6861 6e67  f%%" % pct_chang
-00020930: 6529 202b 2063 6f6c 6f72 5465 7874 2e45  e) + colorText.E
-00020940: 4e44 0a20 2020 2020 2020 2065 6c69 6620  ND.        elif 
-00020950: 7063 745f 6368 616e 6765 203c 202d 302e  pct_change < -0.
-00020960: 323a 0a20 2020 2020 2020 2020 2020 2070  2:.            p
-00020970: 6374 5f63 6861 6e67 6520 3d20 636f 6c6f  ct_change = colo
-00020980: 7254 6578 742e 4641 494c 202b 2028 2225  rText.FAIL + ("%
-00020990: 2e31 6625 2522 2025 2070 6374 5f63 6861  .1f%%" % pct_cha
-000209a0: 6e67 6529 202b 2063 6f6c 6f72 5465 7874  nge) + colorText
-000209b0: 2e45 4e44 0a20 2020 2020 2020 2065 6c73  .END.        els
-000209c0: 653a 0a20 2020 2020 2020 2020 2020 2070  e:.            p
-000209d0: 6374 5f63 6861 6e67 6520 3d20 636f 6c6f  ct_change = colo
-000209e0: 7254 6578 742e 5741 524e 202b 2028 2225  rText.WARN + ("%
-000209f0: 2e31 6625 2522 2025 2070 6374 5f63 6861  .1f%%" % pct_cha
-00020a00: 6e67 6529 202b 2063 6f6c 6f72 5465 7874  nge) + colorText
-00020a10: 2e45 4e44 0a20 2020 2020 2020 2073 6176  .END.        sav
-00020a20: 6544 6963 745b 2225 4368 6e67 225d 203d  eDict["%Chng"] =
-00020a30: 2070 6374 5f73 6176 650a 2020 2020 2020   pct_save.      
-00020a40: 2020 7363 7265 656e 4469 6374 5b22 2543    screenDict["%C
-00020a50: 686e 6722 5d20 3d20 7063 745f 6368 616e  hng"] = pct_chan
-00020a60: 6765 0a20 2020 2020 2020 206c 7470 203d  ge.        ltp =
-00020a70: 2072 6f75 6e64 2872 6563 656e 745b 2243   round(recent["C
-00020a80: 6c6f 7365 225d 2e69 6c6f 635b 305d 2c20  lose"].iloc[0], 
-00020a90: 3229 0a20 2020 2020 2020 2076 6572 6966  2).        verif
-00020aa0: 7953 7461 6765 5477 6f20 3d20 5472 7565  yStageTwo = True
-00020ab0: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-00020ac0: 6461 7461 2920 3e20 3235 303a 0a20 2020  data) > 250:.   
-00020ad0: 2020 2020 2020 2020 2079 6561 726c 794c           yearlyL
-00020ae0: 6f77 203d 2064 6174 612e 6865 6164 2832  ow = data.head(2
-00020af0: 3530 295b 2243 6c6f 7365 225d 2e6d 696e  50)["Close"].min
-00020b00: 2829 0a20 2020 2020 2020 2020 2020 2079  ().            y
-00020b10: 6561 726c 7948 6967 6820 3d20 6461 7461  earlyHigh = data
-00020b20: 2e68 6561 6428 3235 3029 5b22 436c 6f73  .head(250)["Clos
-00020b30: 6522 5d2e 6d61 7828 290a 2020 2020 2020  e"].max().      
-00020b40: 2020 2020 2020 6966 206c 7470 203c 2028        if ltp < (
-00020b50: 3220 2a20 7965 6172 6c79 4c6f 7729 2061  2 * yearlyLow) a
-00020b60: 6e64 206c 7470 203c 2028 302e 3735 202a  nd ltp < (0.75 *
-00020b70: 2079 6561 726c 7948 6967 6829 3a0a 2020   yearlyHigh):.  
-00020b80: 2020 2020 2020 2020 2020 2020 2020 7665                ve
-00020b90: 7269 6679 5374 6167 6554 776f 203d 2046  rifyStageTwo = F
-00020ba0: 616c 7365 0a20 2020 2020 2020 2020 2020  alse.           
-00020bb0: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
-00020bc0: 2253 746f 636b 225d 203d 2063 6f6c 6f72  "Stock"] = color
-00020bd0: 5465 7874 2e46 4149 4c20 2b20 7361 7665  Text.FAIL + save
-00020be0: 4469 6374 5b22 5374 6f63 6b22 5d20 2b20  Dict["Stock"] + 
-00020bf0: 636f 6c6f 7254 6578 742e 454e 440a 2020  colorText.END.  
-00020c00: 2020 2020 2020 6966 206c 7470 203e 3d20        if ltp >= 
-00020c10: 6d69 6e4c 5450 2061 6e64 206c 7470 203c  minLTP and ltp <
-00020c20: 3d20 6d61 784c 5450 3a0a 2020 2020 2020  = maxLTP:.      
-00020c30: 2020 2020 2020 6c74 7056 616c 6964 203d        ltpValid =
-00020c40: 2054 7275 650a 2020 2020 2020 2020 2020   True.          
-00020c50: 2020 6966 206d 696e 4368 616e 6765 2021    if minChange !
-00020c60: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
-00020c70: 2020 2020 2023 2055 7365 7220 6861 7320       # User has 
-00020c80: 7375 7070 6c69 6564 2073 6f6d 6520 6669  supplied some fi
-00020c90: 6c74 6572 2066 6f72 2070 6572 6365 6e74  lter for percent
-00020ca0: 6167 6520 6368 616e 6765 0a20 2020 2020  age change.     
-00020cb0: 2020 2020 2020 2020 2020 206c 7470 5661             ltpVa
-00020cc0: 6c69 6420 3d20 666c 6f61 7428 7374 7228  lid = float(str(
-00020cd0: 7063 745f 7361 7665 292e 7265 706c 6163  pct_save).replac
-00020ce0: 6528 2225 222c 2222 2929 203e 3d20 6d69  e("%","")) >= mi
-00020cf0: 6e43 6861 6e67 650a 2020 2020 2020 2020  nChange.        
-00020d00: 2020 2020 7361 7665 4469 6374 5b22 4c54      saveDict["LT
-00020d10: 5022 5d20 3d20 726f 756e 6428 6c74 702c  P"] = round(ltp,
-00020d20: 2032 290a 2020 2020 2020 2020 2020 2020   2).            
-00020d30: 7363 7265 656e 4469 6374 5b22 4c54 5022  screenDict["LTP"
-00020d40: 5d20 3d20 2863 6f6c 6f72 5465 7874 2e47  ] = (colorText.G
-00020d50: 5245 454e 2069 6620 6c74 7056 616c 6964  REEN if ltpValid
-00020d60: 2065 6c73 6520 636f 6c6f 7254 6578 742e   else colorText.
-00020d70: 4641 494c 2920 2b20 2822 252e 3266 2220  FAIL) + ("%.2f" 
-00020d80: 2520 6c74 7029 202b 2063 6f6c 6f72 5465  % ltp) + colorTe
-00020d90: 7874 2e45 4e44 0a20 2020 2020 2020 2020  xt.END.         
-00020da0: 2020 2072 6574 7572 6e20 6c74 7056 616c     return ltpVal
-00020db0: 6964 2c20 7665 7269 6679 5374 6167 6554  id, verifyStageT
-00020dc0: 776f 0a20 2020 2020 2020 2073 6372 6565  wo.        scree
-00020dd0: 6e44 6963 745b 224c 5450 225d 203d 2063  nDict["LTP"] = c
-00020de0: 6f6c 6f72 5465 7874 2e46 4149 4c20 2b20  olorText.FAIL + 
-00020df0: 2822 252e 3266 2220 2520 6c74 7029 202b  ("%.2f" % ltp) +
-00020e00: 2063 6f6c 6f72 5465 7874 2e45 4e44 0a20   colorText.END. 
-00020e10: 2020 2020 2020 2073 6176 6544 6963 745b         saveDict[
-00020e20: 224c 5450 225d 203d 2072 6f75 6e64 286c  "LTP"] = round(l
-00020e30: 7470 2c20 3229 0a20 2020 2020 2020 2072  tp, 2).        r
-00020e40: 6574 7572 6e20 6c74 7056 616c 6964 2c20  eturn ltpValid, 
-00020e50: 7665 7269 6679 5374 6167 6554 776f 0a0a  verifyStageTwo..
-00020e60: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-00020e70: 4c54 5046 6f72 506f 7274 666f 6c69 6f43  LTPForPortfolioC
-00020e80: 616c 6328 7365 6c66 2c20 6466 2c20 7363  alc(self, df, sc
-00020e90: 7265 656e 4469 6374 2c20 7361 7665 4469  reenDict, saveDi
-00020ea0: 6374 2c72 6571 7565 7374 6564 5065 7269  ct,requestedPeri
-00020eb0: 6f64 3d30 293a 0a20 2020 2020 2020 2064  od=0):.        d
-00020ec0: 6174 6120 3d20 6466 2e63 6f70 7928 290a  ata = df.copy().
-00020ed0: 2020 2020 2020 2020 7065 7269 6f64 7320          periods 
-00020ee0: 3d20 7365 6c66 2e63 6f6e 6669 674d 616e  = self.configMan
-00020ef0: 6167 6572 2e70 6572 696f 6473 5261 6e67  ager.periodsRang
-00020f00: 650a 2020 2020 2020 2020 6966 2072 6571  e.        if req
-00020f10: 7565 7374 6564 5065 7269 6f64 203e 2030  uestedPeriod > 0
-00020f20: 2061 6e64 2072 6571 7565 7374 6564 5065   and requestedPe
-00020f30: 7269 6f64 206e 6f74 2069 6e20 7065 7269  riod not in peri
-00020f40: 6f64 733a 0a20 2020 2020 2020 2020 2020  ods:.           
-00020f50: 2070 6572 696f 6473 2e61 7070 656e 6428   periods.append(
-00020f60: 7265 7175 6573 7465 6450 6572 696f 6429  requestedPeriod)
-00020f70: 0a20 2020 2020 2020 2070 7265 7669 6f75  .        previou
-00020f80: 735f 7265 6365 6e74 203d 2064 6174 612e  s_recent = data.
-00020f90: 6865 6164 2831 290a 2020 2020 2020 2020  head(1).        
-00020fa0: 7072 6576 696f 7573 5f72 6563 656e 742e  previous_recent.
-00020fb0: 7265 7365 745f 696e 6465 7828 696e 706c  reset_index(inpl
-00020fc0: 6163 653d 5472 7565 290a 2020 2020 2020  ace=True).      
-00020fd0: 2020 6361 6c63 5f64 6174 6520 3d20 7374    calc_date = st
-00020fe0: 7228 7072 6576 696f 7573 5f72 6563 656e  r(previous_recen
-00020ff0: 742e 696c 6f63 5b3a 2c20 305d 5b30 5d29  t.iloc[:, 0][0])
-00021000: 2e73 706c 6974 2822 2022 295b 305d 0a20  .split(" ")[0]. 
-00021010: 2020 2020 2020 2066 6f72 2070 7264 2069         for prd i
-00021020: 6e20 7065 7269 6f64 733a 0a20 2020 2020  n periods:.     
-00021030: 2020 2020 2020 2069 6620 6c65 6e28 6461         if len(da
-00021040: 7461 2920 3e3d 2070 7264 202b 2031 3a0a  ta) >= prd + 1:.
-00021050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021060: 7072 6576 4c74 7020 3d20 6461 7461 5b22  prevLtp = data["
-00021070: 436c 6f73 6522 5d2e 696c 6f63 5b30 5d0a  Close"].iloc[0].
-00021080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021090: 6c74 7054 6479 203d 2064 6174 615b 2243  ltpTdy = data["C
-000210a0: 6c6f 7365 225d 2e69 6c6f 635b 7072 645d  lose"].iloc[prd]
-000210b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000210c0: 2069 6620 6973 696e 7374 616e 6365 2870   if isinstance(p
-000210d0: 7265 764c 7470 2c70 642e 5365 7269 6573  revLtp,pd.Series
-000210e0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000210f0: 2020 2020 2020 2070 7265 764c 7470 203d         prevLtp =
-00021100: 2070 7265 764c 7470 5b30 5d0a 2020 2020   prevLtp[0].    
-00021110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021120: 6c74 7054 6479 203d 206c 7470 5464 795b  ltpTdy = ltpTdy[
-00021130: 305d 0a20 2020 2020 2020 2020 2020 2020  0].             
-00021140: 2020 2073 6372 6565 6e44 6963 745b 6622     screenDict[f"
-00021150: 4c54 507b 7072 647d 225d 203d 2028 0a20  LTP{prd}"] = (. 
-00021160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021170: 2020 2028 636f 6c6f 7254 6578 742e 4752     (colorText.GR
-00021180: 4545 4e20 6966 2028 6c74 7054 6479 203e  EEN if (ltpTdy >
-00021190: 3d20 7072 6576 4c74 7029 2065 6c73 6520  = prevLtp) else 
-000211a0: 2863 6f6c 6f72 5465 7874 2e46 4149 4c29  (colorText.FAIL)
-000211b0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000211c0: 2020 2020 2020 2b20 7374 7228 227b 3a2e        + str("{:.
-000211d0: 3266 7d22 2e66 6f72 6d61 7428 6c74 7054  2f}".format(ltpT
-000211e0: 6479 2929 0a20 2020 2020 2020 2020 2020  dy)).           
-000211f0: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
-00021200: 5465 7874 2e45 4e44 0a20 2020 2020 2020  Text.END.       
-00021210: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00021220: 2020 2020 2020 2020 2020 2073 6372 6565             scree
-00021230: 6e44 6963 745b 6622 4772 6f77 7468 7b70  nDict[f"Growth{p
-00021240: 7264 7d22 5d20 3d20 280a 2020 2020 2020  rd}"] = (.      
-00021250: 2020 2020 2020 2020 2020 2020 2020 2863                (c
-00021260: 6f6c 6f72 5465 7874 2e47 5245 454e 2069  olorText.GREEN i
-00021270: 6620 286c 7470 5464 7920 3e3d 2070 7265  f (ltpTdy >= pre
-00021280: 764c 7470 2920 656c 7365 2028 636f 6c6f  vLtp) else (colo
-00021290: 7254 6578 742e 4641 494c 2929 0a20 2020  rText.FAIL)).   
-000212a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000212b0: 202b 2073 7472 2822 7b3a 2e32 667d 222e   + str("{:.2f}".
-000212c0: 666f 726d 6174 286c 7470 5464 7920 2d20  format(ltpTdy - 
-000212d0: 7072 6576 4c74 7029 290a 2020 2020 2020  prevLtp)).      
-000212e0: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-000212f0: 636f 6c6f 7254 6578 742e 454e 440a 2020  colorText.END.  
-00021300: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00021310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021320: 7361 7665 4469 6374 5b66 224c 5450 7b70  saveDict[f"LTP{p
-00021330: 7264 7d22 5d20 3d20 726f 756e 6428 6c74  rd}"] = round(lt
-00021340: 7054 6479 2c20 3229 0a20 2020 2020 2020  pTdy, 2).       
-00021350: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
-00021360: 745b 6622 4772 6f77 7468 7b70 7264 7d22  t[f"Growth{prd}"
-00021370: 5d20 3d20 726f 756e 6428 6c74 7054 6479  ] = round(ltpTdy
-00021380: 202d 2070 7265 764c 7470 2c20 3229 0a20   - prevLtp, 2). 
-00021390: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000213a0: 6620 7072 6420 3d3d 2032 3220 6f72 2028  f prd == 22 or (
-000213b0: 7072 6420 3d3d 2072 6571 7565 7374 6564  prd == requested
-000213c0: 5065 7269 6f64 293a 0a20 2020 2020 2020  Period):.       
-000213d0: 2020 2020 2020 2020 2020 2020 2063 6861               cha
-000213e0: 6e67 6550 6572 6365 6e74 203d 2072 6f75  ngePercent = rou
-000213f0: 6e64 2828 2870 7265 764c 7470 2d6c 7470  nd(((prevLtp-ltp
-00021400: 5464 7929 2069 6620 7265 7175 6573 7465  Tdy) if requeste
-00021410: 6450 6572 696f 6420 3d3d 3020 656c 7365  dPeriod ==0 else
-00021420: 2028 6c74 7054 6479 202d 2070 7265 764c   (ltpTdy - prevL
-00021430: 7470 2929 2a31 3030 2f6c 7470 5464 792c  tp))*100/ltpTdy,
-00021440: 2032 290a 2020 2020 2020 2020 2020 2020   2).            
-00021450: 2020 2020 2020 2020 7361 7665 4469 6374          saveDict
-00021460: 5b66 227b 7072 647d 2d50 6422 5d20 3d20  [f"{prd}-Pd"] = 
-00021470: 6622 7b63 6861 6e67 6550 6572 6365 6e74  f"{changePercent
-00021480: 7d25 2220 6966 206e 6f74 2070 642e 6973  }%" if not pd.is
-00021490: 6e61 2863 6861 6e67 6550 6572 6365 6e74  na(changePercent
-000214a0: 2920 656c 7365 2027 2d27 0a20 2020 2020  ) else '-'.     
-000214b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000214c0: 6372 6565 6e44 6963 745b 6622 7b70 7264  creenDict[f"{prd
-000214d0: 7d2d 5064 225d 203d 2028 2863 6f6c 6f72  }-Pd"] = ((color
-000214e0: 5465 7874 2e47 5245 454e 2069 6620 6368  Text.GREEN if ch
-000214f0: 616e 6765 5065 7263 656e 7420 3e3d 3020  angePercent >=0 
-00021500: 656c 7365 2063 6f6c 6f72 5465 7874 2e46  else colorText.F
-00021510: 4149 4c29 202b 2066 227b 6368 616e 6765  AIL) + f"{change
-00021520: 5065 7263 656e 747d 2522 202b 2063 6f6c  Percent}%" + col
-00021530: 6f72 5465 7874 2e45 4e44 2920 6966 206e  orText.END) if n
-00021540: 6f74 2070 642e 6973 6e61 2863 6861 6e67  ot pd.isna(chang
-00021550: 6550 6572 6365 6e74 2920 656c 7365 2027  ePercent) else '
-00021560: 2d27 0a20 2020 2020 2020 2020 2020 2020  -'.             
-00021570: 2020 2020 2020 2069 6620 2870 7264 203d         if (prd =
-00021580: 3d20 7265 7175 6573 7465 6450 6572 696f  = requestedPerio
-00021590: 6429 3a0a 2020 2020 2020 2020 2020 2020  d):.            
-000215a0: 2020 2020 2020 2020 2020 2020 6d61 784c              maxL
-000215b0: 5450 506f 7465 6e74 6961 6c20 3d20 6d61  TPPotential = ma
-000215c0: 7828 6461 7461 5b22 4869 6768 225d 2e68  x(data["High"].h
-000215d0: 6561 6428 7072 6429 290a 2020 2020 2020  ead(prd)).      
-000215e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000215f0: 2020 7363 7265 656e 4469 6374 5b66 224d    screenDict[f"M
-00021600: 6178 4c54 5022 5d20 3d20 280a 2020 2020  axLTP"] = (.    
-00021610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021620: 2020 2020 2020 2020 2863 6f6c 6f72 5465          (colorTe
-00021630: 7874 2e47 5245 454e 2069 6620 286d 6178  xt.GREEN if (max
-00021640: 4c54 5050 6f74 656e 7469 616c 203e 3d20  LTPPotential >= 
-00021650: 7072 6576 4c74 7029 2065 6c73 6520 2863  prevLtp) else (c
-00021660: 6f6c 6f72 5465 7874 2e46 4149 4c29 290a  olorText.FAIL)).
+0001ee30: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
+0001ee40: 745b 2250 6174 7465 726e 225d 203d 2028  t["Pattern"] = (
+0001ee50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001ee60: 2020 2020 2020 2020 2020 2020 2073 6176               sav
+0001ee70: 6564 5b30 5d0a 2020 2020 2020 2020 2020  ed[0].          
+0001ee80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ee90: 2020 2b20 636f 6c6f 7254 6578 742e 424f    + colorText.BO
+0001eea0: 4c44 0a20 2020 2020 2020 2020 2020 2020  LD.             
+0001eeb0: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+0001eec0: 2063 6f6c 6f72 5465 7874 2e57 4152 4e0a   colorText.WARN.
+0001eed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001eee0: 2020 2020 2020 2020 2020 2020 2b20 2822              + ("
+0001eef0: 496e 7369 6465 2042 6172 2028 2564 2922  Inside Bar (%d)"
+0001ef00: 2025 2069 290a 2020 2020 2020 2020 2020   % i).          
+0001ef10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ef20: 2020 2b20 636f 6c6f 7254 6578 742e 454e    + colorText.EN
+0001ef30: 440a 2020 2020 2020 2020 2020 2020 2020  D.              
+0001ef40: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0001ef50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ef60: 2020 2020 7361 7665 4469 6374 5b22 5061      saveDict["Pa
+0001ef70: 7474 6572 6e22 5d20 3d20 7361 7665 645b  ttern"] = saved[
+0001ef80: 315d 202b 2022 496e 7369 6465 2042 6172  1] + "Inside Bar
+0001ef90: 2028 2564 2922 2025 2069 0a20 2020 2020   (%d)" % i.     
+0001efa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001efb0: 2020 2072 6574 7572 6e20 690a 2020 2020     return i.    
+0001efc0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0001efd0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001efe0: 2020 2020 2020 7265 7475 726e 2030 0a20        return 0. 
+0001eff0: 2020 2020 2020 2072 6574 7572 6e20 300a         return 0.
+0001f000: 0a20 2020 2023 2046 696e 6420 4950 4f20  .    # Find IPO 
+0001f010: 6261 7365 0a20 2020 2064 6566 2076 616c  base.    def val
+0001f020: 6964 6174 6549 706f 4261 7365 2873 656c  idateIpoBase(sel
+0001f030: 662c 2073 746f 636b 2c20 6466 2c20 7363  f, stock, df, sc
+0001f040: 7265 656e 4469 6374 2c20 7361 7665 4469  reenDict, saveDi
+0001f050: 6374 2c20 7065 7263 656e 7461 6765 3d30  ct, percentage=0
+0001f060: 2e33 293a 0a20 2020 2020 2020 2069 6620  .3):.        if 
+0001f070: 6466 2069 7320 4e6f 6e65 206f 7220 6c65  df is None or le
+0001f080: 6e28 6466 2920 3d3d 2030 3a0a 2020 2020  n(df) == 0:.    
+0001f090: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+0001f0a0: 616c 7365 0a20 2020 2020 2020 2064 6174  alse.        dat
+0001f0b0: 6120 3d20 6466 2e63 6f70 7928 290a 2020  a = df.copy().  
+0001f0c0: 2020 2020 2020 6c69 7374 696e 6750 7269        listingPri
+0001f0d0: 6365 203d 2064 6174 615b 3a3a 2d31 5d2e  ce = data[::-1].
+0001f0e0: 6865 6164 2831 295b 224f 7065 6e22 5d2e  head(1)["Open"].
+0001f0f0: 696c 6f63 5b30 5d0a 2020 2020 2020 2020  iloc[0].        
+0001f100: 6375 7272 656e 7450 7269 6365 203d 2064  currentPrice = d
+0001f110: 6174 612e 6865 6164 2831 295b 2243 6c6f  ata.head(1)["Clo
+0001f120: 7365 225d 2e69 6c6f 635b 305d 0a20 2020  se"].iloc[0].   
+0001f130: 2020 2020 2041 5448 203d 2064 6174 612e       ATH = data.
+0001f140: 6465 7363 7269 6265 2829 5b22 4869 6768  describe()["High
+0001f150: 225d 5b22 6d61 7822 5d0a 2020 2020 2020  "]["max"].      
+0001f160: 2020 6966 2041 5448 203e 2028 6c69 7374    if ATH > (list
+0001f170: 696e 6750 7269 6365 202b 2028 6c69 7374  ingPrice + (list
+0001f180: 696e 6750 7269 6365 202a 2070 6572 6365  ingPrice * perce
+0001f190: 6e74 6167 6529 293a 0a20 2020 2020 2020  ntage)):.       
+0001f1a0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+0001f1b0: 650a 2020 2020 2020 2020 6177 6179 203d  e.        away =
+0001f1c0: 2072 6f75 6e64 2828 2863 7572 7265 6e74   round(((current
+0001f1d0: 5072 6963 6520 2d20 6c69 7374 696e 6750  Price - listingP
+0001f1e0: 7269 6365 2920 2f20 6c69 7374 696e 6750  rice) / listingP
+0001f1f0: 7269 6365 2920 2a20 3130 302c 2031 290a  rice) * 100, 1).
+0001f200: 2020 2020 2020 2020 6966 2028 0a20 2020          if (.   
+0001f210: 2020 2020 2020 2020 2028 6c69 7374 696e           (listin
+0001f220: 6750 7269 6365 202d 2028 6c69 7374 696e  gPrice - (listin
+0001f230: 6750 7269 6365 202a 2070 6572 6365 6e74  gPrice * percent
+0001f240: 6167 6529 290a 2020 2020 2020 2020 2020  age)).          
+0001f250: 2020 3c3d 2063 7572 7265 6e74 5072 6963    <= currentPric
+0001f260: 650a 2020 2020 2020 2020 2020 2020 3c3d  e.            <=
+0001f270: 2028 6c69 7374 696e 6750 7269 6365 202b   (listingPrice +
+0001f280: 2028 6c69 7374 696e 6750 7269 6365 202a   (listingPrice *
+0001f290: 2070 6572 6365 6e74 6167 6529 290a 2020   percentage)).  
+0001f2a0: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
+0001f2b0: 2020 2020 2073 6176 6564 203d 2073 656c       saved = sel
+0001f2c0: 662e 6669 6e64 4375 7272 656e 7453 6176  f.findCurrentSav
+0001f2d0: 6564 5661 6c75 6528 7363 7265 656e 4469  edValue(screenDi
+0001f2e0: 6374 2c20 7361 7665 4469 6374 2c20 2250  ct, saveDict, "P
+0001f2f0: 6174 7465 726e 2229 0a20 2020 2020 2020  attern").       
+0001f300: 2020 2020 2069 6620 6177 6179 203e 2030       if away > 0
+0001f310: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001f320: 2020 7363 7265 656e 4469 6374 5b22 5061    screenDict["Pa
+0001f330: 7474 6572 6e22 5d20 3d20 280a 2020 2020  ttern"] = (.    
+0001f340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f350: 7361 7665 645b 305d 200a 2020 2020 2020  saved[0] .      
+0001f360: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+0001f370: 636f 6c6f 7254 6578 742e 424f 4c44 0a20  colorText.BOLD. 
+0001f380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f390: 2020 202b 2063 6f6c 6f72 5465 7874 2e47     + colorText.G
+0001f3a0: 5245 454e 0a20 2020 2020 2020 2020 2020  REEN.           
+0001f3b0: 2020 2020 2020 2020 202b 2066 2249 504f           + f"IPO
+0001f3c0: 2042 6173 6520 287b 6177 6179 7d20 2529   Base ({away} %)
+0001f3d0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0001f3e0: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
+0001f3f0: 742e 454e 440a 2020 2020 2020 2020 2020  t.END.          
+0001f400: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0001f410: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0001f420: 2020 2020 2020 2020 2020 7363 7265 656e            screen
+0001f430: 4469 6374 5b22 5061 7474 6572 6e22 5d20  Dict["Pattern"] 
+0001f440: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+0001f450: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
+0001f460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001f470: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
+0001f480: 2e42 4f4c 440a 2020 2020 2020 2020 2020  .BOLD.          
+0001f490: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
+0001f4a0: 7254 6578 742e 4752 4545 4e0a 2020 2020  rText.GREEN.    
+0001f4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f4c0: 2b20 2249 504f 2042 6173 6520 220a 2020  + "IPO Base ".  
+0001f4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f4e0: 2020 2b20 636f 6c6f 7254 6578 742e 4641    + colorText.FA
+0001f4f0: 494c 0a20 2020 2020 2020 2020 2020 2020  IL.             
+0001f500: 2020 2020 2020 202b 2066 2228 7b61 7761         + f"({awa
+0001f510: 797d 2025 2922 0a20 2020 2020 2020 2020  y} %)".         
+0001f520: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
+0001f530: 6f72 5465 7874 2e45 4e44 0a20 2020 2020  orText.END.     
+0001f540: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0001f550: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
+0001f560: 745b 2250 6174 7465 726e 225d 203d 2073  t["Pattern"] = s
+0001f570: 6176 6564 5b31 5d20 2b20 6622 4950 4f20  aved[1] + f"IPO 
+0001f580: 4261 7365 2028 7b61 7761 797d 2025 2922  Base ({away} %)"
+0001f590: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0001f5a0: 7572 6e20 5472 7565 0a20 2020 2020 2020  urn True.       
+0001f5b0: 2072 6574 7572 6e20 4661 6c73 650a 0a20   return False.. 
+0001f5c0: 2020 2023 406d 6561 7375 7265 5f74 696d     #@measure_tim
+0001f5d0: 650a 2020 2020 2320 5661 6c69 6461 7465  e.    # Validate
+0001f5e0: 204c 6f72 656e 747a 6961 6e20 436c 6173   Lorentzian Clas
+0001f5f0: 7369 6669 6361 7469 6f6e 2073 6967 6e61  sification signa
+0001f600: 6c0a 2020 2020 6465 6620 7661 6c69 6461  l.    def valida
+0001f610: 7465 4c6f 7265 6e74 7a69 616e 2873 656c  teLorentzian(sel
+0001f620: 662c 2064 662c 2073 6372 6565 6e44 6963  f, df, screenDic
+0001f630: 742c 2073 6176 6544 6963 742c 206c 6f6f  t, saveDict, loo
+0001f640: 6b46 6f72 3d33 293a 0a20 2020 2020 2020  kFor=3):.       
+0001f650: 2069 6620 6466 2069 7320 4e6f 6e65 206f   if df is None o
+0001f660: 7220 6c65 6e28 6466 2920 3d3d 2030 3a0a  r len(df) == 0:.
+0001f670: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0001f680: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
+0001f690: 2064 6174 6120 3d20 6466 2e63 6f70 7928   data = df.copy(
+0001f6a0: 290a 2020 2020 2020 2020 2320 6c6f 6f6b  ).        # look
+0001f6b0: 466f 723a 2031 2d42 7579 2c20 322d 5365  For: 1-Buy, 2-Se
+0001f6c0: 6c6c 2c20 332d 416e 790a 2020 2020 2020  ll, 3-Any.      
+0001f6d0: 2020 6461 7461 203d 2064 6174 615b 3a3a    data = data[::
+0001f6e0: 2d31 5d20 2023 2052 6576 6572 7365 2074  -1]  # Reverse t
+0001f6f0: 6865 2064 6174 6166 7261 6d65 0a20 2020  he dataframe.   
+0001f700: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
+0001f710: 2e72 656e 616d 6528 0a20 2020 2020 2020  .rename(.       
+0001f720: 2020 2020 2063 6f6c 756d 6e73 3d7b 0a20       columns={. 
+0001f730: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0001f740: 4f70 656e 223a 2022 6f70 656e 222c 0a20  Open": "open",. 
+0001f750: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0001f760: 436c 6f73 6522 3a20 2263 6c6f 7365 222c  Close": "close",
+0001f770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001f780: 2022 4869 6768 223a 2022 6869 6768 222c   "High": "high",
+0001f790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001f7a0: 2022 4c6f 7722 3a20 226c 6f77 222c 0a20   "Low": "low",. 
+0001f7b0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0001f7c0: 566f 6c75 6d65 223a 2022 766f 6c75 6d65  Volume": "volume
+0001f7d0: 222c 0a20 2020 2020 2020 2020 2020 207d  ",.            }
+0001f7e0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+0001f7f0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+0001f800: 2020 2020 7769 7468 2053 7570 7072 6573      with Suppres
+0001f810: 734f 7574 7075 7428 7375 7070 7265 7373  sOutput(suppress
+0001f820: 5f73 7464 6f75 743d 5472 7565 2c20 7375  _stdout=True, su
+0001f830: 7070 7265 7373 5f73 7464 6572 723d 5472  ppress_stderr=Tr
+0001f840: 7565 293a 0a20 2020 2020 2020 2020 2020  ue):.           
+0001f850: 2020 2020 206c 6320 3d20 6174 612e 4c6f       lc = ata.Lo
+0001f860: 7265 6e74 7a69 616e 436c 6173 7369 6669  rentzianClassifi
+0001f870: 6361 7469 6f6e 2864 6174 613d 6461 7461  cation(data=data
+0001f880: 290a 2020 2020 2020 2020 2020 2020 7361  ).            sa
+0001f890: 7665 6420 3d20 7365 6c66 2e66 696e 6443  ved = self.findC
+0001f8a0: 7572 7265 6e74 5361 7665 6456 616c 7565  urrentSavedValue
+0001f8b0: 2873 6372 6565 6e44 6963 742c 2073 6176  (screenDict, sav
+0001f8c0: 6544 6963 742c 2022 5061 7474 6572 6e22  eDict, "Pattern"
+0001f8d0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+0001f8e0: 206c 632e 6466 2e69 6c6f 635b 2d31 5d5b   lc.df.iloc[-1][
+0001f8f0: 2269 734e 6577 4275 7953 6967 6e61 6c22  "isNewBuySignal"
+0001f900: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
+0001f910: 2020 2073 6372 6565 6e44 6963 745b 2250     screenDict["P
+0001f920: 6174 7465 726e 225d 203d 2028 0a20 2020  attern"] = (.   
+0001f930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f940: 2073 6176 6564 5b30 5d20 2b20 636f 6c6f   saved[0] + colo
+0001f950: 7254 6578 742e 424f 4c44 202b 2063 6f6c  rText.BOLD + col
+0001f960: 6f72 5465 7874 2e47 5245 454e 202b 2022  orText.GREEN + "
+0001f970: 4c6f 7265 6e74 7a69 616e 2d42 7579 2220  Lorentzian-Buy" 
+0001f980: 2b20 636f 6c6f 7254 6578 742e 454e 440a  + colorText.END.
+0001f990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f9a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001f9b0: 2020 7361 7665 4469 6374 5b22 5061 7474    saveDict["Patt
+0001f9c0: 6572 6e22 5d20 3d20 7361 7665 645b 315d  ern"] = saved[1]
+0001f9d0: 202b 2022 4c6f 7265 6e74 7a69 616e 2d42   + "Lorentzian-B
+0001f9e0: 7579 220a 2020 2020 2020 2020 2020 2020  uy".            
+0001f9f0: 2020 2020 6966 206c 6f6f 6b46 6f72 2021      if lookFor !
+0001fa00: 3d20 323a 2023 204e 6f74 2053 656c 6c0a  = 2: # Not Sell.
+0001fa10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001fa20: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+0001fa30: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+0001fa40: 206c 632e 6466 2e69 6c6f 635b 2d31 5d5b   lc.df.iloc[-1][
+0001fa50: 2269 734e 6577 5365 6c6c 5369 676e 616c  "isNewSellSignal
+0001fa60: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
+0001fa70: 2020 2020 7363 7265 656e 4469 6374 5b22      screenDict["
+0001fa80: 5061 7474 6572 6e22 5d20 3d20 280a 2020  Pattern"] = (.  
+0001fa90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001faa0: 2020 7361 7665 645b 305d 202b 2063 6f6c    saved[0] + col
+0001fab0: 6f72 5465 7874 2e42 4f4c 4420 2b20 636f  orText.BOLD + co
+0001fac0: 6c6f 7254 6578 742e 4641 494c 202b 2022  lorText.FAIL + "
+0001fad0: 4c6f 7265 6e74 7a69 616e 2d53 656c 6c22  Lorentzian-Sell"
+0001fae0: 202b 2063 6f6c 6f72 5465 7874 2e45 4e44   + colorText.END
+0001faf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001fb00: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+0001fb10: 2020 2073 6176 6544 6963 745b 2250 6174     saveDict["Pat
+0001fb20: 7465 726e 225d 203d 2073 6176 6564 5b31  tern"] = saved[1
+0001fb30: 5d20 2b20 224c 6f72 656e 747a 6961 6e2d  ] + "Lorentzian-
+0001fb40: 5365 6c6c 220a 2020 2020 2020 2020 2020  Sell".          
+0001fb50: 2020 2020 2020 6966 206c 6f6f 6b46 6f72        if lookFor
+0001fb60: 2021 3d20 313a 2023 204e 6f74 2042 7579   != 1: # Not Buy
+0001fb70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001fb80: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+0001fb90: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+0001fba0: 4578 6365 7074 696f 6e3a 2020 2320 7072  Exception:  # pr
+0001fbb0: 6167 6d61 3a20 6e6f 2063 6f76 6572 0a20  agma: no cover. 
+0001fbc0: 2020 2020 2020 2020 2020 2023 2056 616c             # Val
+0001fbd0: 7565 4572 726f 723a 206f 7065 7261 6e64  ueError: operand
+0001fbe0: 7320 636f 756c 6420 6e6f 7420 6265 2062  s could not be b
+0001fbf0: 726f 6164 6361 7374 2074 6f67 6574 6865  roadcast togethe
+0001fc00: 7220 7769 7468 2073 6861 7065 7320 2832  r with shapes (2
+0001fc10: 302c 2920 2832 362c 290a 2020 2020 2020  0,) (26,).      
+0001fc20: 2020 2020 2020 2320 4669 6c65 2022 2f6f        # File "/o
+0001fc30: 7074 2f68 6f6d 6562 7265 772f 6c69 622f  pt/homebrew/lib/
+0001fc40: 7079 7468 6f6e 332e 3131 2f73 6974 652d  python3.11/site-
+0001fc50: 7061 636b 6167 6573 2f61 6476 616e 6365  packages/advance
+0001fc60: 645f 7461 2f4c 6f72 656e 747a 6961 6e43  d_ta/LorentzianC
+0001fc70: 6c61 7373 6966 6963 6174 696f 6e2f 436c  lassification/Cl
+0001fc80: 6173 7369 6669 6572 2e70 7922 2c20 6c69  assifier.py", li
+0001fc90: 6e65 2031 3836 2c20 696e 205f 5f69 6e69  ne 186, in __ini
+0001fca0: 745f 5f0a 2020 2020 2020 2020 2020 2020  t__.            
+0001fcb0: 2320 4669 6c65 2022 2f6f 7074 2f68 6f6d  # File "/opt/hom
+0001fcc0: 6562 7265 772f 6c69 622f 7079 7468 6f6e  ebrew/lib/python
+0001fcd0: 332e 3131 2f73 6974 652d 7061 636b 6167  3.11/site-packag
+0001fce0: 6573 2f61 6476 616e 6365 645f 7461 2f4c  es/advanced_ta/L
+0001fcf0: 6f72 656e 747a 6961 6e43 6c61 7373 6966  orentzianClassif
+0001fd00: 6963 6174 696f 6e2f 436c 6173 7369 6669  ication/Classifi
+0001fd10: 6572 2e70 7922 2c20 6c69 6e65 2033 3935  er.py", line 395
+0001fd20: 2c20 696e 205f 5f63 6c61 7373 6966 790a  , in __classify.
+0001fd30: 2020 2020 2020 2020 2020 2020 2320 4669              # Fi
+0001fd40: 6c65 2022 2f6f 7074 2f68 6f6d 6562 7265  le "/opt/homebre
+0001fd50: 772f 6c69 622f 7079 7468 6f6e 332e 3131  w/lib/python3.11
+0001fd60: 2f73 6974 652d 7061 636b 6167 6573 2f70  /site-packages/p
+0001fd70: 616e 6461 732f 636f 7265 2f6f 7073 2f63  andas/core/ops/c
+0001fd80: 6f6d 6d6f 6e2e 7079 222c 206c 696e 6520  ommon.py", line 
+0001fd90: 3736 2c20 696e 206e 6577 5f6d 6574 686f  76, in new_metho
+0001fda0: 640a 2020 2020 2020 2020 2020 2020 2320  d.            # 
+0001fdb0: 4669 6c65 2022 2f6f 7074 2f68 6f6d 6562  File "/opt/homeb
+0001fdc0: 7265 772f 6c69 622f 7079 7468 6f6e 332e  rew/lib/python3.
+0001fdd0: 3131 2f73 6974 652d 7061 636b 6167 6573  11/site-packages
+0001fde0: 2f70 616e 6461 732f 636f 7265 2f61 7272  /pandas/core/arr
+0001fdf0: 6179 6c69 6b65 2e70 7922 2c20 6c69 6e65  aylike.py", line
+0001fe00: 2037 302c 2069 6e20 5f5f 616e 645f 5f0a   70, in __and__.
+0001fe10: 2020 2020 2020 2020 2020 2020 2320 4669              # Fi
+0001fe20: 6c65 2022 2f6f 7074 2f68 6f6d 6562 7265  le "/opt/homebre
+0001fe30: 772f 6c69 622f 7079 7468 6f6e 332e 3131  w/lib/python3.11
+0001fe40: 2f73 6974 652d 7061 636b 6167 6573 2f70  /site-packages/p
+0001fe50: 616e 6461 732f 636f 7265 2f73 6572 6965  andas/core/serie
+0001fe60: 732e 7079 222c 206c 696e 6520 3538 3130  s.py", line 5810
+0001fe70: 2c20 696e 205f 6c6f 6769 6361 6c5f 6d65  , in _logical_me
+0001fe80: 7468 6f64 0a20 2020 2020 2020 2020 2020  thod.           
+0001fe90: 2023 2046 696c 6520 222f 6f70 742f 686f   # File "/opt/ho
+0001fea0: 6d65 6272 6577 2f6c 6962 2f70 7974 686f  mebrew/lib/pytho
+0001feb0: 6e33 2e31 312f 7369 7465 2d70 6163 6b61  n3.11/site-packa
+0001fec0: 6765 732f 7061 6e64 6173 2f63 6f72 652f  ges/pandas/core/
+0001fed0: 6f70 732f 6172 7261 795f 6f70 732e 7079  ops/array_ops.py
+0001fee0: 222c 206c 696e 6520 3435 362c 2069 6e20  ", line 456, in 
+0001fef0: 6c6f 6769 6361 6c5f 6f70 0a20 2020 2020  logical_op.     
+0001ff00: 2020 2020 2020 2023 2046 696c 6520 222f         # File "/
+0001ff10: 6f70 742f 686f 6d65 6272 6577 2f6c 6962  opt/homebrew/lib
+0001ff20: 2f70 7974 686f 6e33 2e31 312f 7369 7465  /python3.11/site
+0001ff30: 2d70 6163 6b61 6765 732f 7061 6e64 6173  -packages/pandas
+0001ff40: 2f63 6f72 652f 6f70 732f 6172 7261 795f  /core/ops/array_
+0001ff50: 6f70 732e 7079 222c 206c 696e 6520 3336  ops.py", line 36
+0001ff60: 342c 2069 6e20 6e61 5f6c 6f67 6963 616c  4, in na_logical
+0001ff70: 5f6f 700a 2020 2020 2020 2020 2020 2020  _op.            
+0001ff80: 2320 7365 6c66 2e64 6566 6175 6c74 5f6c  # self.default_l
+0001ff90: 6f67 6765 722e 6465 6275 6728 652c 2065  ogger.debug(e, e
+0001ffa0: 7863 5f69 6e66 6f3d 5472 7565 290a 2020  xc_info=True).  
+0001ffb0: 2020 2020 2020 2020 2020 7061 7373 0a20            pass. 
+0001ffc0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+0001ffd0: 6c73 650a 0a20 2020 2023 2076 616c 6964  lse..    # valid
+0001ffe0: 6174 6520 6966 2074 6865 2073 746f 636b  ate if the stock
+0001fff0: 2068 6173 2062 6565 6e20 6861 7669 6e67   has been having
+00020000: 206c 6f77 6572 206c 6f77 732c 206c 6f77   lower lows, low
+00020010: 6572 2068 6967 6873 0a20 2020 2064 6566  er highs.    def
+00020020: 2076 616c 6964 6174 654c 6f77 6572 4869   validateLowerHi
+00020030: 6768 734c 6f77 6572 4c6f 7773 2873 656c  ghsLowerLows(sel
+00020040: 662c 2064 6629 3a0a 2020 2020 2020 2020  f, df):.        
+00020050: 6966 2064 6620 6973 204e 6f6e 6520 6f72  if df is None or
+00020060: 206c 656e 2864 6629 203d 3d20 303a 0a20   len(df) == 0:. 
+00020070: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00020080: 6e20 4661 6c73 650a 2020 2020 2020 2020  n False.        
+00020090: 6461 7461 203d 2064 662e 636f 7079 2829  data = df.copy()
+000200a0: 0a20 2020 2020 2020 2064 6179 3020 3d20  .        day0 = 
+000200b0: 6461 7461 0a20 2020 2020 2020 2064 6179  data.        day
+000200c0: 3120 3d20 6461 7461 5b31 3a5d 0a20 2020  1 = data[1:].   
+000200d0: 2020 2020 2064 6179 3220 3d20 6461 7461       day2 = data
+000200e0: 5b32 3a5d 0a20 2020 2020 2020 2064 6179  [2:].        day
+000200f0: 3320 3d20 6461 7461 5b33 3a5d 0a20 2020  3 = data[3:].   
+00020100: 2020 2020 206c 6f77 6572 4869 6768 7320       lowerHighs 
+00020110: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+00020120: 2864 6179 305b 2248 6967 6822 5d2e 696c  (day0["High"].il
+00020130: 6f63 5b30 5d20 3c20 6461 7931 5b22 4869  oc[0] < day1["Hi
+00020140: 6768 225d 2e69 6c6f 635b 305d 290a 2020  gh"].iloc[0]).  
+00020150: 2020 2020 2020 2020 2020 616e 6420 2864            and (d
+00020160: 6179 315b 2248 6967 6822 5d2e 696c 6f63  ay1["High"].iloc
+00020170: 5b30 5d20 3c20 6461 7932 5b22 4869 6768  [0] < day2["High
+00020180: 225d 2e69 6c6f 635b 305d 290a 2020 2020  "].iloc[0]).    
+00020190: 2020 2020 2020 2020 616e 6420 2864 6179          and (day
+000201a0: 325b 2248 6967 6822 5d2e 696c 6f63 5b30  2["High"].iloc[0
+000201b0: 5d20 3c20 6461 7933 5b22 4869 6768 225d  ] < day3["High"]
+000201c0: 2e69 6c6f 635b 305d 290a 2020 2020 2020  .iloc[0]).      
+000201d0: 2020 290a 2020 2020 2020 2020 6c6f 7765    ).        lowe
+000201e0: 724c 6f77 7320 3d20 280a 2020 2020 2020  rLows = (.      
+000201f0: 2020 2020 2020 2864 6179 305b 224c 6f77        (day0["Low
+00020200: 225d 2e69 6c6f 635b 305d 203c 2064 6179  "].iloc[0] < day
+00020210: 315b 224c 6f77 225d 2e69 6c6f 635b 305d  1["Low"].iloc[0]
+00020220: 290a 2020 2020 2020 2020 2020 2020 616e  ).            an
+00020230: 6420 2864 6179 315b 224c 6f77 225d 2e69  d (day1["Low"].i
+00020240: 6c6f 635b 305d 203c 2064 6179 325b 224c  loc[0] < day2["L
+00020250: 6f77 225d 2e69 6c6f 635b 305d 290a 2020  ow"].iloc[0]).  
+00020260: 2020 2020 2020 2020 2020 616e 6420 2864            and (d
+00020270: 6179 325b 224c 6f77 225d 2e69 6c6f 635b  ay2["Low"].iloc[
+00020280: 305d 203c 2064 6179 335b 224c 6f77 225d  0] < day3["Low"]
+00020290: 2e69 6c6f 635b 305d 290a 2020 2020 2020  .iloc[0]).      
+000202a0: 2020 290a 2020 2020 2020 2020 6869 6768    ).        high
+000202b0: 6572 5253 4920 3d20 280a 2020 2020 2020  erRSI = (.      
+000202c0: 2020 2020 2020 2864 6179 305b 2252 5349        (day0["RSI
+000202d0: 225d 2e69 6c6f 635b 305d 203c 2064 6179  "].iloc[0] < day
+000202e0: 315b 2252 5349 225d 2e69 6c6f 635b 305d  1["RSI"].iloc[0]
+000202f0: 290a 2020 2020 2020 2020 2020 2020 616e  ).            an
+00020300: 6420 2864 6179 315b 2252 5349 225d 2e69  d (day1["RSI"].i
+00020310: 6c6f 635b 305d 203c 2064 6179 325b 2252  loc[0] < day2["R
+00020320: 5349 225d 2e69 6c6f 635b 305d 290a 2020  SI"].iloc[0]).  
+00020330: 2020 2020 2020 2020 2020 616e 6420 2864            and (d
+00020340: 6179 325b 2252 5349 225d 2e69 6c6f 635b  ay2["RSI"].iloc[
+00020350: 305d 203c 2064 6179 335b 2252 5349 225d  0] < day3["RSI"]
+00020360: 2e69 6c6f 635b 305d 290a 2020 2020 2020  .iloc[0]).      
+00020370: 2020 2020 2020 616e 6420 6461 7930 5b22        and day0["
+00020380: 5253 4922 5d2e 696c 6f63 5b30 5d20 3e3d  RSI"].iloc[0] >=
+00020390: 2035 300a 2020 2020 2020 2020 290a 2020   50.        ).  
+000203a0: 2020 2020 2020 7265 7475 726e 206c 6f77        return low
+000203b0: 6572 4869 6768 7320 616e 6420 6c6f 7765  erHighs and lowe
+000203c0: 724c 6f77 7320 616e 6420 6869 6768 6572  rLows and higher
+000203d0: 5253 490a 0a20 2020 2023 2056 616c 6964  RSI..    # Valid
+000203e0: 6174 6520 6966 2072 6563 656e 7420 766f  ate if recent vo
+000203f0: 6c75 6d65 2069 7320 6c6f 7765 7374 206f  lume is lowest o
+00020400: 6620 6c61 7374 2027 4e27 2044 6179 730a  f last 'N' Days.
+00020410: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+00020420: 4c6f 7765 7374 566f 6c75 6d65 2873 656c  LowestVolume(sel
+00020430: 662c 2064 662c 2064 6179 7346 6f72 4c6f  f, df, daysForLo
+00020440: 7765 7374 566f 6c75 6d65 293a 0a20 2020  westVolume):.   
+00020450: 2020 2020 2069 6620 6466 2069 7320 4e6f       if df is No
+00020460: 6e65 206f 7220 6c65 6e28 6466 2920 3d3d  ne or len(df) ==
+00020470: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+00020480: 7265 7475 726e 2046 616c 7365 0a20 2020  return False.   
+00020490: 2020 2020 2064 6174 6120 3d20 6466 2e63       data = df.c
+000204a0: 6f70 7928 290a 2020 2020 2020 2020 6461  opy().        da
+000204b0: 7461 203d 2064 6174 612e 6669 6c6c 6e61  ta = data.fillna
+000204c0: 2830 290a 2020 2020 2020 2020 6461 7461  (0).        data
+000204d0: 203d 2064 6174 612e 7265 706c 6163 6528   = data.replace(
+000204e0: 5b6e 702e 696e 662c 202d 6e70 2e69 6e66  [np.inf, -np.inf
+000204f0: 5d2c 2030 290a 2020 2020 2020 2020 6966  ], 0).        if
+00020500: 2064 6179 7346 6f72 4c6f 7765 7374 566f   daysForLowestVo
+00020510: 6c75 6d65 2069 7320 4e6f 6e65 3a0a 2020  lume is None:.  
+00020520: 2020 2020 2020 2020 2020 6461 7973 466f            daysFo
+00020530: 724c 6f77 6573 7456 6f6c 756d 6520 3d20  rLowestVolume = 
+00020540: 3330 0a20 2020 2020 2020 2069 6620 6c65  30.        if le
+00020550: 6e28 6461 7461 2920 3c20 6461 7973 466f  n(data) < daysFo
+00020560: 724c 6f77 6573 7456 6f6c 756d 653a 0a20  rLowestVolume:. 
+00020570: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00020580: 6e20 4661 6c73 650a 2020 2020 2020 2020  n False.        
+00020590: 6461 7461 203d 2064 6174 612e 6865 6164  data = data.head
+000205a0: 2864 6179 7346 6f72 4c6f 7765 7374 566f  (daysForLowestVo
+000205b0: 6c75 6d65 290a 2020 2020 2020 2020 7265  lume).        re
+000205c0: 6365 6e74 203d 2064 6174 612e 6865 6164  cent = data.head
+000205d0: 2831 290a 2020 2020 2020 2020 6966 206c  (1).        if l
+000205e0: 656e 2872 6563 656e 7429 203c 2031 3a0a  en(recent) < 1:.
+000205f0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00020600: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
+00020610: 2069 6620 2872 6563 656e 745b 2256 6f6c   if (recent["Vol
+00020620: 756d 6522 5d2e 696c 6f63 5b30 5d20 3c3d  ume"].iloc[0] <=
+00020630: 2064 6174 612e 6465 7363 7269 6265 2829   data.describe()
+00020640: 5b22 566f 6c75 6d65 225d 5b22 6d69 6e22  ["Volume"]["min"
+00020650: 5d29 2061 6e64 2072 6563 656e 745b 0a20  ]) and recent[. 
+00020660: 2020 2020 2020 2020 2020 2022 566f 6c75             "Volu
+00020670: 6d65 220a 2020 2020 2020 2020 5d5b 305d  me".        ][0]
+00020680: 2021 3d20 6e70 2e6e 616e 3a0a 2020 2020   != np.nan:.    
+00020690: 2020 2020 2020 2020 7265 7475 726e 2054          return T
+000206a0: 7275 650a 2020 2020 2020 2020 7265 7475  rue.        retu
+000206b0: 726e 2046 616c 7365 0a0a 2020 2020 2320  rn False..    # 
+000206c0: 5661 6c69 6461 7465 204c 5450 2077 6974  Validate LTP wit
+000206d0: 6869 6e20 6c69 6d69 7473 0a20 2020 2064  hin limits.    d
+000206e0: 6566 2076 616c 6964 6174 654c 5450 2873  ef validateLTP(s
+000206f0: 656c 662c 2064 662c 2073 6372 6565 6e44  elf, df, screenD
+00020700: 6963 742c 2073 6176 6544 6963 742c 206d  ict, saveDict, m
+00020710: 696e 4c54 503d 4e6f 6e65 2c20 6d61 784c  inLTP=None, maxL
+00020720: 5450 3d4e 6f6e 652c 6d69 6e43 6861 6e67  TP=None,minChang
+00020730: 653d 3029 3a0a 2020 2020 2020 2020 6461  e=0):.        da
+00020740: 7461 203d 2064 662e 636f 7079 2829 0a20  ta = df.copy(). 
+00020750: 2020 2020 2020 206c 7470 5661 6c69 6420         ltpValid 
+00020760: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
+00020770: 6966 206d 696e 4c54 5020 6973 204e 6f6e  if minLTP is Non
+00020780: 653a 0a20 2020 2020 2020 2020 2020 206d  e:.            m
+00020790: 696e 4c54 5020 3d20 7365 6c66 2e63 6f6e  inLTP = self.con
+000207a0: 6669 674d 616e 6167 6572 2e6d 696e 4c54  figManager.minLT
+000207b0: 500a 2020 2020 2020 2020 6966 206d 6178  P.        if max
+000207c0: 4c54 5020 6973 204e 6f6e 653a 0a20 2020  LTP is None:.   
+000207d0: 2020 2020 2020 2020 206d 6178 4c54 5020           maxLTP 
+000207e0: 3d20 7365 6c66 2e63 6f6e 6669 674d 616e  = self.configMan
+000207f0: 6167 6572 2e6d 6178 4c54 500a 2020 2020  ager.maxLTP.    
+00020800: 2020 2020 6461 7461 203d 2064 6174 612e      data = data.
+00020810: 6669 6c6c 6e61 2830 290a 2020 2020 2020  fillna(0).      
+00020820: 2020 6461 7461 203d 2064 6174 612e 7265    data = data.re
+00020830: 706c 6163 6528 5b6e 702e 696e 662c 202d  place([np.inf, -
+00020840: 6e70 2e69 6e66 5d2c 2030 290a 2020 2020  np.inf], 0).    
+00020850: 2020 2020 7265 6365 6e74 203d 2064 6174      recent = dat
+00020860: 612e 6865 6164 2831 290a 0a20 2020 2020  a.head(1)..     
+00020870: 2020 2070 6374 5f63 6861 6e67 6520 3d20     pct_change = 
+00020880: 2864 6174 615b 3a3a 2d31 5d5b 2243 6c6f  (data[::-1]["Clo
+00020890: 7365 225d 2e70 6374 5f63 6861 6e67 6528  se"].pct_change(
+000208a0: 2920 2a20 3130 3029 2e69 6c6f 635b 2d31  ) * 100).iloc[-1
+000208b0: 5d0a 2020 2020 2020 2020 6966 2070 6374  ].        if pct
+000208c0: 5f63 6861 6e67 6520 3d3d 206e 702e 696e  _change == np.in
+000208d0: 6620 6f72 2070 6374 5f63 6861 6e67 6520  f or pct_change 
+000208e0: 3d3d 202d 6e70 2e69 6e66 3a0a 2020 2020  == -np.inf:.    
+000208f0: 2020 2020 2020 2020 7063 745f 6368 616e          pct_chan
+00020900: 6765 203d 2030 0a20 2020 2020 2020 2070  ge = 0.        p
+00020910: 6374 5f73 6176 6520 3d20 2225 2e31 6625  ct_save = "%.1f%
+00020920: 2522 2025 2070 6374 5f63 6861 6e67 650a  %" % pct_change.
+00020930: 2020 2020 2020 2020 6966 2070 6374 5f63          if pct_c
+00020940: 6861 6e67 6520 3e20 302e 323a 0a20 2020  hange > 0.2:.   
+00020950: 2020 2020 2020 2020 2070 6374 5f63 6861           pct_cha
+00020960: 6e67 6520 3d20 636f 6c6f 7254 6578 742e  nge = colorText.
+00020970: 4752 4545 4e20 2b20 2822 252e 3166 2525  GREEN + ("%.1f%%
+00020980: 2220 2520 7063 745f 6368 616e 6765 2920  " % pct_change) 
+00020990: 2b20 636f 6c6f 7254 6578 742e 454e 440a  + colorText.END.
+000209a0: 2020 2020 2020 2020 656c 6966 2070 6374          elif pct
+000209b0: 5f63 6861 6e67 6520 3c20 2d30 2e32 3a0a  _change < -0.2:.
+000209c0: 2020 2020 2020 2020 2020 2020 7063 745f              pct_
+000209d0: 6368 616e 6765 203d 2063 6f6c 6f72 5465  change = colorTe
+000209e0: 7874 2e46 4149 4c20 2b20 2822 252e 3166  xt.FAIL + ("%.1f
+000209f0: 2525 2220 2520 7063 745f 6368 616e 6765  %%" % pct_change
+00020a00: 2920 2b20 636f 6c6f 7254 6578 742e 454e  ) + colorText.EN
+00020a10: 440a 2020 2020 2020 2020 656c 7365 3a0a  D.        else:.
+00020a20: 2020 2020 2020 2020 2020 2020 7063 745f              pct_
+00020a30: 6368 616e 6765 203d 2063 6f6c 6f72 5465  change = colorTe
+00020a40: 7874 2e57 4152 4e20 2b20 2822 252e 3166  xt.WARN + ("%.1f
+00020a50: 2525 2220 2520 7063 745f 6368 616e 6765  %%" % pct_change
+00020a60: 2920 2b20 636f 6c6f 7254 6578 742e 454e  ) + colorText.EN
+00020a70: 440a 2020 2020 2020 2020 7361 7665 4469  D.        saveDi
+00020a80: 6374 5b22 2543 686e 6722 5d20 3d20 7063  ct["%Chng"] = pc
+00020a90: 745f 7361 7665 0a20 2020 2020 2020 2073  t_save.        s
+00020aa0: 6372 6565 6e44 6963 745b 2225 4368 6e67  creenDict["%Chng
+00020ab0: 225d 203d 2070 6374 5f63 6861 6e67 650a  "] = pct_change.
+00020ac0: 2020 2020 2020 2020 6c74 7020 3d20 726f          ltp = ro
+00020ad0: 756e 6428 7265 6365 6e74 5b22 436c 6f73  und(recent["Clos
+00020ae0: 6522 5d2e 696c 6f63 5b30 5d2c 2032 290a  e"].iloc[0], 2).
+00020af0: 2020 2020 2020 2020 7665 7269 6679 5374          verifySt
+00020b00: 6167 6554 776f 203d 2054 7275 650a 2020  ageTwo = True.  
+00020b10: 2020 2020 2020 6966 206c 656e 2864 6174        if len(dat
+00020b20: 6129 203e 2032 3530 3a0a 2020 2020 2020  a) > 250:.      
+00020b30: 2020 2020 2020 7965 6172 6c79 4c6f 7720        yearlyLow 
+00020b40: 3d20 6461 7461 2e68 6561 6428 3235 3029  = data.head(250)
+00020b50: 5b22 436c 6f73 6522 5d2e 6d69 6e28 290a  ["Close"].min().
+00020b60: 2020 2020 2020 2020 2020 2020 7965 6172              year
+00020b70: 6c79 4869 6768 203d 2064 6174 612e 6865  lyHigh = data.he
+00020b80: 6164 2832 3530 295b 2243 6c6f 7365 225d  ad(250)["Close"]
+00020b90: 2e6d 6178 2829 0a20 2020 2020 2020 2020  .max().         
+00020ba0: 2020 2069 6620 6c74 7020 3c20 2832 202a     if ltp < (2 *
+00020bb0: 2079 6561 726c 794c 6f77 2920 616e 6420   yearlyLow) and 
+00020bc0: 6c74 7020 3c20 2830 2e37 3520 2a20 7965  ltp < (0.75 * ye
+00020bd0: 6172 6c79 4869 6768 293a 0a20 2020 2020  arlyHigh):.     
+00020be0: 2020 2020 2020 2020 2020 2076 6572 6966             verif
+00020bf0: 7953 7461 6765 5477 6f20 3d20 4661 6c73  yStageTwo = Fals
+00020c00: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00020c10: 2020 7363 7265 656e 4469 6374 5b22 5374    screenDict["St
+00020c20: 6f63 6b22 5d20 3d20 636f 6c6f 7254 6578  ock"] = colorTex
+00020c30: 742e 4641 494c 202b 2073 6176 6544 6963  t.FAIL + saveDic
+00020c40: 745b 2253 746f 636b 225d 202b 2063 6f6c  t["Stock"] + col
+00020c50: 6f72 5465 7874 2e45 4e44 0a20 2020 2020  orText.END.     
+00020c60: 2020 2069 6620 6c74 7020 3e3d 206d 696e     if ltp >= min
+00020c70: 4c54 5020 616e 6420 6c74 7020 3c3d 206d  LTP and ltp <= m
+00020c80: 6178 4c54 503a 0a20 2020 2020 2020 2020  axLTP:.         
+00020c90: 2020 206c 7470 5661 6c69 6420 3d20 5472     ltpValid = Tr
+00020ca0: 7565 0a20 2020 2020 2020 2020 2020 2069  ue.            i
+00020cb0: 6620 6d69 6e43 6861 6e67 6520 213d 2030  f minChange != 0
+00020cc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00020cd0: 2020 2320 5573 6572 2068 6173 2073 7570    # User has sup
+00020ce0: 706c 6965 6420 736f 6d65 2066 696c 7465  plied some filte
+00020cf0: 7220 666f 7220 7065 7263 656e 7461 6765  r for percentage
+00020d00: 2063 6861 6e67 650a 2020 2020 2020 2020   change.        
+00020d10: 2020 2020 2020 2020 6c74 7056 616c 6964          ltpValid
+00020d20: 203d 2066 6c6f 6174 2873 7472 2870 6374   = float(str(pct
+00020d30: 5f73 6176 6529 2e72 6570 6c61 6365 2822  _save).replace("
+00020d40: 2522 2c22 2229 2920 3e3d 206d 696e 4368  %","")) >= minCh
+00020d50: 616e 6765 0a20 2020 2020 2020 2020 2020  ange.           
+00020d60: 2073 6176 6544 6963 745b 224c 5450 225d   saveDict["LTP"]
+00020d70: 203d 2072 6f75 6e64 286c 7470 2c20 3229   = round(ltp, 2)
+00020d80: 0a20 2020 2020 2020 2020 2020 2073 6372  .            scr
+00020d90: 6565 6e44 6963 745b 224c 5450 225d 203d  eenDict["LTP"] =
+00020da0: 2028 636f 6c6f 7254 6578 742e 4752 4545   (colorText.GREE
+00020db0: 4e20 6966 206c 7470 5661 6c69 6420 656c  N if ltpValid el
+00020dc0: 7365 2063 6f6c 6f72 5465 7874 2e46 4149  se colorText.FAI
+00020dd0: 4c29 202b 2028 2225 2e32 6622 2025 206c  L) + ("%.2f" % l
+00020de0: 7470 2920 2b20 636f 6c6f 7254 6578 742e  tp) + colorText.
+00020df0: 454e 440a 2020 2020 2020 2020 2020 2020  END.            
+00020e00: 7265 7475 726e 206c 7470 5661 6c69 642c  return ltpValid,
+00020e10: 2076 6572 6966 7953 7461 6765 5477 6f0a   verifyStageTwo.
+00020e20: 2020 2020 2020 2020 7363 7265 656e 4469          screenDi
+00020e30: 6374 5b22 4c54 5022 5d20 3d20 636f 6c6f  ct["LTP"] = colo
+00020e40: 7254 6578 742e 4641 494c 202b 2028 2225  rText.FAIL + ("%
+00020e50: 2e32 6622 2025 206c 7470 2920 2b20 636f  .2f" % ltp) + co
+00020e60: 6c6f 7254 6578 742e 454e 440a 2020 2020  lorText.END.    
+00020e70: 2020 2020 7361 7665 4469 6374 5b22 4c54      saveDict["LT
+00020e80: 5022 5d20 3d20 726f 756e 6428 6c74 702c  P"] = round(ltp,
+00020e90: 2032 290a 2020 2020 2020 2020 7265 7475   2).        retu
+00020ea0: 726e 206c 7470 5661 6c69 642c 2076 6572  rn ltpValid, ver
+00020eb0: 6966 7953 7461 6765 5477 6f0a 0a20 2020  ifyStageTwo..   
+00020ec0: 2064 6566 2076 616c 6964 6174 654c 5450   def validateLTP
+00020ed0: 466f 7250 6f72 7466 6f6c 696f 4361 6c63  ForPortfolioCalc
+00020ee0: 2873 656c 662c 2064 662c 2073 6372 6565  (self, df, scree
+00020ef0: 6e44 6963 742c 2073 6176 6544 6963 742c  nDict, saveDict,
+00020f00: 7265 7175 6573 7465 6450 6572 696f 643d  requestedPeriod=
+00020f10: 3029 3a0a 2020 2020 2020 2020 6461 7461  0):.        data
+00020f20: 203d 2064 662e 636f 7079 2829 0a20 2020   = df.copy().   
+00020f30: 2020 2020 2070 6572 696f 6473 203d 2073       periods = s
+00020f40: 656c 662e 636f 6e66 6967 4d61 6e61 6765  elf.configManage
+00020f50: 722e 7065 7269 6f64 7352 616e 6765 0a20  r.periodsRange. 
+00020f60: 2020 2020 2020 2069 6620 7265 7175 6573         if reques
+00020f70: 7465 6450 6572 696f 6420 3e20 3020 616e  tedPeriod > 0 an
+00020f80: 6420 7265 7175 6573 7465 6450 6572 696f  d requestedPerio
+00020f90: 6420 6e6f 7420 696e 2070 6572 696f 6473  d not in periods
+00020fa0: 3a0a 2020 2020 2020 2020 2020 2020 7065  :.            pe
+00020fb0: 7269 6f64 732e 6170 7065 6e64 2872 6571  riods.append(req
+00020fc0: 7565 7374 6564 5065 7269 6f64 290a 2020  uestedPeriod).  
+00020fd0: 2020 2020 2020 7072 6576 696f 7573 5f72        previous_r
+00020fe0: 6563 656e 7420 3d20 6461 7461 2e68 6561  ecent = data.hea
+00020ff0: 6428 3129 0a20 2020 2020 2020 2070 7265  d(1).        pre
+00021000: 7669 6f75 735f 7265 6365 6e74 2e72 6573  vious_recent.res
+00021010: 6574 5f69 6e64 6578 2869 6e70 6c61 6365  et_index(inplace
+00021020: 3d54 7275 6529 0a20 2020 2020 2020 2063  =True).        c
+00021030: 616c 635f 6461 7465 203d 2073 7472 2870  alc_date = str(p
+00021040: 7265 7669 6f75 735f 7265 6365 6e74 2e69  revious_recent.i
+00021050: 6c6f 635b 3a2c 2030 5d5b 305d 292e 7370  loc[:, 0][0]).sp
+00021060: 6c69 7428 2220 2229 5b30 5d0a 2020 2020  lit(" ")[0].    
+00021070: 2020 2020 666f 7220 7072 6420 696e 2070      for prd in p
+00021080: 6572 696f 6473 3a0a 2020 2020 2020 2020  eriods:.        
+00021090: 2020 2020 6966 206c 656e 2864 6174 6129      if len(data)
+000210a0: 203e 3d20 7072 6420 2b20 313a 0a20 2020   >= prd + 1:.   
+000210b0: 2020 2020 2020 2020 2020 2020 2070 7265               pre
+000210c0: 764c 7470 203d 2064 6174 615b 2243 6c6f  vLtp = data["Clo
+000210d0: 7365 225d 2e69 6c6f 635b 305d 0a20 2020  se"].iloc[0].   
+000210e0: 2020 2020 2020 2020 2020 2020 206c 7470               ltp
+000210f0: 5464 7920 3d20 6461 7461 5b22 436c 6f73  Tdy = data["Clos
+00021100: 6522 5d2e 696c 6f63 5b70 7264 5d0a 2020  e"].iloc[prd].  
+00021110: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00021120: 2069 7369 6e73 7461 6e63 6528 7072 6576   isinstance(prev
+00021130: 4c74 702c 7064 2e53 6572 6965 7329 3a0a  Ltp,pd.Series):.
+00021140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021150: 2020 2020 7072 6576 4c74 7020 3d20 7072      prevLtp = pr
+00021160: 6576 4c74 705b 305d 0a20 2020 2020 2020  evLtp[0].       
+00021170: 2020 2020 2020 2020 2020 2020 206c 7470               ltp
+00021180: 5464 7920 3d20 6c74 7054 6479 5b30 5d0a  Tdy = ltpTdy[0].
+00021190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000211a0: 7363 7265 656e 4469 6374 5b66 224c 5450  screenDict[f"LTP
+000211b0: 7b70 7264 7d22 5d20 3d20 280a 2020 2020  {prd}"] = (.    
+000211c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000211d0: 2863 6f6c 6f72 5465 7874 2e47 5245 454e  (colorText.GREEN
+000211e0: 2069 6620 286c 7470 5464 7920 3e3d 2070   if (ltpTdy >= p
+000211f0: 7265 764c 7470 2920 656c 7365 2028 636f  revLtp) else (co
+00021200: 6c6f 7254 6578 742e 4641 494c 2929 0a20  lorText.FAIL)). 
+00021210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021220: 2020 202b 2073 7472 2822 7b3a 2e32 667d     + str("{:.2f}
+00021230: 222e 666f 726d 6174 286c 7470 5464 7929  ".format(ltpTdy)
+00021240: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00021250: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
+00021260: 742e 454e 440a 2020 2020 2020 2020 2020  t.END.          
+00021270: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00021280: 2020 2020 2020 2020 7363 7265 656e 4469          screenDi
+00021290: 6374 5b66 2247 726f 7774 687b 7072 647d  ct[f"Growth{prd}
+000212a0: 225d 203d 2028 0a20 2020 2020 2020 2020  "] = (.         
+000212b0: 2020 2020 2020 2020 2020 2028 636f 6c6f             (colo
+000212c0: 7254 6578 742e 4752 4545 4e20 6966 2028  rText.GREEN if (
+000212d0: 6c74 7054 6479 203e 3d20 7072 6576 4c74  ltpTdy >= prevLt
+000212e0: 7029 2065 6c73 6520 2863 6f6c 6f72 5465  p) else (colorTe
+000212f0: 7874 2e46 4149 4c29 290a 2020 2020 2020  xt.FAIL)).      
+00021300: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+00021310: 7374 7228 227b 3a2e 3266 7d22 2e66 6f72  str("{:.2f}".for
+00021320: 6d61 7428 6c74 7054 6479 202d 2070 7265  mat(ltpTdy - pre
+00021330: 764c 7470 2929 0a20 2020 2020 2020 2020  vLtp)).         
+00021340: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
+00021350: 6f72 5465 7874 2e45 4e44 0a20 2020 2020  orText.END.     
+00021360: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00021370: 2020 2020 2020 2020 2020 2020 2073 6176               sav
+00021380: 6544 6963 745b 6622 4c54 507b 7072 647d  eDict[f"LTP{prd}
+00021390: 225d 203d 2072 6f75 6e64 286c 7470 5464  "] = round(ltpTd
+000213a0: 792c 2032 290a 2020 2020 2020 2020 2020  y, 2).          
+000213b0: 2020 2020 2020 7361 7665 4469 6374 5b66        saveDict[f
+000213c0: 2247 726f 7774 687b 7072 647d 225d 203d  "Growth{prd}"] =
+000213d0: 2072 6f75 6e64 286c 7470 5464 7920 2d20   round(ltpTdy - 
+000213e0: 7072 6576 4c74 702c 2032 290a 2020 2020  prevLtp, 2).    
+000213f0: 2020 2020 2020 2020 2020 2020 6966 2070              if p
+00021400: 7264 203d 3d20 3232 206f 7220 2870 7264  rd == 22 or (prd
+00021410: 203d 3d20 7265 7175 6573 7465 6450 6572   == requestedPer
+00021420: 696f 6429 3a0a 2020 2020 2020 2020 2020  iod):.          
+00021430: 2020 2020 2020 2020 2020 6368 616e 6765            change
+00021440: 5065 7263 656e 7420 3d20 726f 756e 6428  Percent = round(
+00021450: 2828 7072 6576 4c74 702d 6c74 7054 6479  ((prevLtp-ltpTdy
+00021460: 2920 6966 2072 6571 7565 7374 6564 5065  ) if requestedPe
+00021470: 7269 6f64 203d 3d30 2065 6c73 6520 286c  riod ==0 else (l
+00021480: 7470 5464 7920 2d20 7072 6576 4c74 7029  tpTdy - prevLtp)
+00021490: 292a 3130 302f 6c74 7054 6479 2c20 3229  )*100/ltpTdy, 2)
+000214a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000214b0: 2020 2020 2073 6176 6544 6963 745b 6622       saveDict[f"
+000214c0: 7b70 7264 7d2d 5064 225d 203d 2066 227b  {prd}-Pd"] = f"{
+000214d0: 6368 616e 6765 5065 7263 656e 747d 2522  changePercent}%"
+000214e0: 2069 6620 6e6f 7420 7064 2e69 736e 6128   if not pd.isna(
+000214f0: 6368 616e 6765 5065 7263 656e 7429 2065  changePercent) e
+00021500: 6c73 6520 272d 270a 2020 2020 2020 2020  lse '-'.        
+00021510: 2020 2020 2020 2020 2020 2020 7363 7265              scre
+00021520: 656e 4469 6374 5b66 227b 7072 647d 2d50  enDict[f"{prd}-P
+00021530: 6422 5d20 3d20 2828 636f 6c6f 7254 6578  d"] = ((colorTex
+00021540: 742e 4752 4545 4e20 6966 2063 6861 6e67  t.GREEN if chang
+00021550: 6550 6572 6365 6e74 203e 3d30 2065 6c73  ePercent >=0 els
+00021560: 6520 636f 6c6f 7254 6578 742e 4641 494c  e colorText.FAIL
+00021570: 2920 2b20 6622 7b63 6861 6e67 6550 6572  ) + f"{changePer
+00021580: 6365 6e74 7d25 2220 2b20 636f 6c6f 7254  cent}%" + colorT
+00021590: 6578 742e 454e 4429 2069 6620 6e6f 7420  ext.END) if not 
+000215a0: 7064 2e69 736e 6128 6368 616e 6765 5065  pd.isna(changePe
+000215b0: 7263 656e 7429 2065 6c73 6520 272d 270a  rcent) else '-'.
+000215c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000215d0: 2020 2020 6966 2028 7072 6420 3d3d 2072      if (prd == r
+000215e0: 6571 7565 7374 6564 5065 7269 6f64 293a  equestedPeriod):
+000215f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00021600: 2020 2020 2020 2020 206d 6178 4c54 5050           maxLTPP
+00021610: 6f74 656e 7469 616c 203d 206d 6178 2864  otential = max(d
+00021620: 6174 615b 2248 6967 6822 5d2e 6865 6164  ata["High"].head
+00021630: 2870 7264 2929 0a20 2020 2020 2020 2020  (prd)).         
+00021640: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00021650: 6372 6565 6e44 6963 745b 6622 4d61 784c  creenDict[f"MaxL
+00021660: 5450 225d 203d 2028 0a20 2020 2020 2020  TP"] = (.       
 00021670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021680: 2020 2020 2020 2020 2020 2020 2b20 7374              + st
-00021690: 7228 227b 3a2e 3266 7d22 2e66 6f72 6d61  r("{:.2f}".forma
-000216a0: 7428 6d61 784c 5450 506f 7465 6e74 6961  t(maxLTPPotentia
-000216b0: 6c29 290a 2020 2020 2020 2020 2020 2020  l)).            
-000216c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000216d0: 2b20 636f 6c6f 7254 6578 742e 454e 440a  + colorText.END.
-000216e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000216f0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00021700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021710: 2020 7363 7265 656e 4469 6374 5b66 2250    screenDict[f"P
-00021720: 6f74 2e47 7277 225d 203d 2028 0a20 2020  ot.Grw"] = (.   
-00021730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021740: 2020 2020 2020 2020 2028 636f 6c6f 7254           (colorT
-00021750: 6578 742e 4752 4545 4e20 6966 2028 6d61  ext.GREEN if (ma
-00021760: 784c 5450 506f 7465 6e74 6961 6c20 3e3d  xLTPPotential >=
-00021770: 2070 7265 764c 7470 2920 656c 7365 2028   prevLtp) else (
-00021780: 636f 6c6f 7254 6578 742e 4641 494c 2929  colorText.FAIL))
-00021790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000217a0: 2020 2020 2020 2020 2020 2020 202b 2073               + s
-000217b0: 7472 2822 7b3a 2e32 667d 2522 2e66 6f72  tr("{:.2f}%".for
-000217c0: 6d61 7428 286d 6178 4c54 5050 6f74 656e  mat((maxLTPPoten
-000217d0: 7469 616c 202d 2070 7265 764c 7470 292a  tial - prevLtp)*
-000217e0: 3130 302f 7072 6576 4c74 7029 290a 2020  100/prevLtp)).  
+00021680: 2020 2020 2028 636f 6c6f 7254 6578 742e       (colorText.
+00021690: 4752 4545 4e20 6966 2028 6d61 784c 5450  GREEN if (maxLTP
+000216a0: 506f 7465 6e74 6961 6c20 3e3d 2070 7265  Potential >= pre
+000216b0: 764c 7470 2920 656c 7365 2028 636f 6c6f  vLtp) else (colo
+000216c0: 7254 6578 742e 4641 494c 2929 0a20 2020  rText.FAIL)).   
+000216d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000216e0: 2020 2020 2020 2020 202b 2073 7472 2822           + str("
+000216f0: 7b3a 2e32 667d 222e 666f 726d 6174 286d  {:.2f}".format(m
+00021700: 6178 4c54 5050 6f74 656e 7469 616c 2929  axLTPPotential))
+00021710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00021720: 2020 2020 2020 2020 2020 2020 202b 2063               + c
+00021730: 6f6c 6f72 5465 7874 2e45 4e44 0a20 2020  olorText.END.   
+00021740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021750: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00021760: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00021770: 6372 6565 6e44 6963 745b 6622 506f 742e  creenDict[f"Pot.
+00021780: 4772 7722 5d20 3d20 280a 2020 2020 2020  Grw"] = (.      
+00021790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000217a0: 2020 2020 2020 2863 6f6c 6f72 5465 7874        (colorText
+000217b0: 2e47 5245 454e 2069 6620 286d 6178 4c54  .GREEN if (maxLT
+000217c0: 5050 6f74 656e 7469 616c 203e 3d20 7072  PPotential >= pr
+000217d0: 6576 4c74 7029 2065 6c73 6520 2863 6f6c  evLtp) else (col
+000217e0: 6f72 5465 7874 2e46 4149 4c29 290a 2020  orText.FAIL)).  
 000217f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021800: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
-00021810: 7254 6578 742e 454e 440a 2020 2020 2020  rText.END.      
-00021820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021830: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00021840: 2020 2020 2020 2020 2020 2020 7361 7665              save
-00021850: 4469 6374 5b66 224d 6178 4c54 5022 5d20  Dict[f"MaxLTP"] 
-00021860: 3d20 726f 756e 6428 6d61 784c 5450 506f  = round(maxLTPPo
-00021870: 7465 6e74 6961 6c2c 2032 290a 2020 2020  tential, 2).    
-00021880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021890: 2020 2020 7361 7665 4469 6374 5b66 2250      saveDict[f"P
-000218a0: 6f74 2e47 7277 225d 203d 2066 227b 726f  ot.Grw"] = f"{ro
-000218b0: 756e 6428 286d 6178 4c54 5050 6f74 656e  und((maxLTPPoten
-000218c0: 7469 616c 202d 2070 7265 764c 7470 292a  tial - prevLtp)*
-000218d0: 3130 302f 7072 6576 4c74 702c 2032 297d  100/prevLtp, 2)}
-000218e0: 2522 0a20 2020 2020 2020 2020 2020 2020  %".             
-000218f0: 2020 2073 6372 6565 6e44 6963 745b 2244     screenDict["D
-00021900: 6174 6522 5d20 3d20 6361 6c63 5f64 6174  ate"] = calc_dat
-00021910: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00021920: 2020 7361 7665 4469 6374 5b22 4461 7465    saveDict["Date
-00021930: 225d 203d 2063 616c 635f 6461 7465 0a20  "] = calc_date. 
-00021940: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00021950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00021960: 2073 6176 6544 6963 745b 6622 4c54 507b   saveDict[f"LTP{
-00021970: 7072 647d 225d 203d 206e 702e 6e61 6e0a  prd}"] = np.nan.
-00021980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021990: 7361 7665 4469 6374 5b66 2247 726f 7774  saveDict[f"Growt
-000219a0: 687b 7072 647d 225d 203d 206e 702e 6e61  h{prd}"] = np.na
-000219b0: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
-000219c0: 2020 7363 7265 656e 4469 6374 5b22 4461    screenDict["Da
-000219d0: 7465 225d 203d 2063 616c 635f 6461 7465  te"] = calc_date
-000219e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000219f0: 2073 6176 6544 6963 745b 2244 6174 6522   saveDict["Date"
-00021a00: 5d20 3d20 6361 6c63 5f64 6174 650a 0a20  ] = calc_date.. 
-00021a10: 2020 2023 2046 696e 6420 7374 6f63 6b73     # Find stocks
-00021a20: 2074 6861 7420 6172 6520 6265 6172 6973   that are bearis
-00021a30: 6820 696e 7472 6164 6179 3a20 4d61 6364  h intraday: Macd
-00021a40: 2048 6973 746f 6772 616d 206e 6567 6174   Histogram negat
-00021a50: 6976 650a 2020 2020 6465 6620 7661 6c69  ive.    def vali
-00021a60: 6461 7465 4d41 4344 4869 7374 6f67 7261  dateMACDHistogra
-00021a70: 6d42 656c 6f77 3028 7365 6c66 2c20 6466  mBelow0(self, df
-00021a80: 293a 0a20 2020 2020 2020 2069 6620 6466  ):.        if df
-00021a90: 2069 7320 4e6f 6e65 206f 7220 6c65 6e28   is None or len(
-00021aa0: 6466 2920 3d3d 2030 3a0a 2020 2020 2020  df) == 0:.      
-00021ab0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-00021ac0: 7365 0a20 2020 2020 2020 2064 6174 6120  se.        data 
-00021ad0: 3d20 6466 2e63 6f70 7928 290a 2020 2020  = df.copy().    
-00021ae0: 2020 2020 6461 7461 203d 2064 6174 612e      data = data.
-00021af0: 6669 6c6c 6e61 2830 290a 2020 2020 2020  fillna(0).      
-00021b00: 2020 6461 7461 203d 2064 6174 612e 7265    data = data.re
-00021b10: 706c 6163 6528 5b6e 702e 696e 662c 202d  place([np.inf, -
-00021b20: 6e70 2e69 6e66 5d2c 2030 290a 2020 2020  np.inf], 0).    
-00021b30: 2020 2020 6461 7461 203d 2064 6174 615b      data = data[
-00021b40: 3a3a 2d31 5d20 2023 2052 6576 6572 7365  ::-1]  # Reverse
-00021b50: 2074 6865 2064 6174 6166 7261 6d65 2073   the dataframe s
-00021b60: 6f20 7468 6174 2069 7473 2074 6865 206f  o that its the o
-00021b70: 6c64 6573 7420 6461 7465 2066 6972 7374  ldest date first
-00021b80: 0a20 2020 2020 2020 206d 6163 6420 3d20  .        macd = 
-00021b90: 706b 7461 6c69 622e 4d41 4344 2864 6174  pktalib.MACD(dat
-00021ba0: 615b 2243 6c6f 7365 225d 2c20 3132 2c20  a["Close"], 12, 
-00021bb0: 3236 2c20 3929 5b32 5d2e 7461 696c 2831  26, 9)[2].tail(1
-00021bc0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00021bd0: 206d 6163 642e 696c 6f63 5b3a 315d 5b30   macd.iloc[:1][0
-00021be0: 5d20 3c20 300a 0a20 2020 2023 406d 6561  ] < 0..    #@mea
-00021bf0: 7375 7265 5f74 696d 650a 2020 2020 2320  sure_time.    # 
-00021c00: 4669 6e64 2069 6620 7374 6f63 6b20 6761  Find if stock ga
-00021c10: 696e 696e 6720 6275 6c6c 6973 6820 6d6f  ining bullish mo
-00021c20: 6d65 6e74 756d 0a20 2020 2064 6566 2076  mentum.    def v
-00021c30: 616c 6964 6174 654d 6f6d 656e 7475 6d28  alidateMomentum(
-00021c40: 7365 6c66 2c20 6466 2c20 7363 7265 656e  self, df, screen
-00021c50: 4469 6374 2c20 7361 7665 4469 6374 293a  Dict, saveDict):
-00021c60: 0a20 2020 2020 2020 2069 6620 6466 2069  .        if df i
-00021c70: 7320 4e6f 6e65 206f 7220 6c65 6e28 6466  s None or len(df
-00021c80: 2920 3d3d 2030 3a0a 2020 2020 2020 2020  ) == 0:.        
-00021c90: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-00021ca0: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
-00021cb0: 6466 2e63 6f70 7928 290a 2020 2020 2020  df.copy().      
-00021cc0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-00021cd0: 2020 2064 6174 6120 3d20 6461 7461 2e68     data = data.h
-00021ce0: 6561 6428 3329 0a20 2020 2020 2020 2020  ead(3).         
-00021cf0: 2020 2069 6620 6c65 6e28 6461 7461 2920     if len(data) 
-00021d00: 3c20 333a 0a20 2020 2020 2020 2020 2020  < 3:.           
-00021d10: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-00021d20: 650a 2020 2020 2020 2020 2020 2020 666f  e.            fo
-00021d30: 7220 726f 7720 696e 2064 6174 612e 6974  r row in data.it
-00021d40: 6572 726f 7773 2829 3a0a 2020 2020 2020  errows():.      
-00021d50: 2020 2020 2020 2020 2020 2320 416c 6c20            # All 
-00021d60: 3320 6361 6e64 6c65 7320 7368 6f75 6c64  3 candles should
-00021d70: 2062 6520 4772 6565 6e20 616e 6420 4e4f   be Green and NO
-00021d80: 5420 4369 7263 7569 7473 0a20 2020 2020  T Circuits.     
-00021d90: 2020 2020 2020 2020 2020 2079 6320 3d20             yc = 
-00021da0: 726f 775b 315d 5b22 436c 6f73 6522 5d0a  row[1]["Close"].
-00021db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021dc0: 796f 203d 2072 6f77 5b31 5d5b 224f 7065  yo = row[1]["Ope
-00021dd0: 6e22 5d0a 2020 2020 2020 2020 2020 2020  n"].            
-00021de0: 2020 2020 6966 2079 6320 3c3d 2079 6f3a      if yc <= yo:
-00021df0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00021e00: 2020 2020 2023 2073 656c 662e 6465 6661       # self.defa
-00021e10: 756c 745f 6c6f 6767 6572 2e69 6e66 6f28  ult_logger.info(
-00021e20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00021e30: 2020 2020 2023 2020 2020 2066 2753 746f       #     f'Sto
-00021e40: 636b 3a7b 7361 7665 4469 6374 5b22 5374  ck:{saveDict["St
-00021e50: 6f63 6b22 5d7d 2c20 6973 206e 6f74 2061  ock"]}, is not a
-00021e60: 206d 6f6d 656e 7475 6d2d 6761 696e 6572   momentum-gainer
-00021e70: 2062 6563 6175 7365 2079 6573 7465 7264   because yesterd
-00021e80: 6179 2d63 6c6f 7365 2028 7b79 637d 2920  ay-close ({yc}) 
-00021e90: 3c3d 2079 6573 7465 7264 6179 2d6f 7065  <= yesterday-ope
-00021ea0: 6e20 287b 796f 7d29 270a 2020 2020 2020  n ({yo})'.      
-00021eb0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00021ec0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00021ed0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-00021ee0: 7365 0a20 2020 2020 2020 2020 2020 206f  se.            o
-00021ef0: 7065 6e44 6573 6320 3d20 6461 7461 2e73  penDesc = data.s
-00021f00: 6f72 745f 7661 6c75 6573 2862 793d 5b22  ort_values(by=["
-00021f10: 4f70 656e 225d 2c20 6173 6365 6e64 696e  Open"], ascendin
-00021f20: 673d 4661 6c73 6529 0a20 2020 2020 2020  g=False).       
-00021f30: 2020 2020 2063 6c6f 7365 4465 7363 203d       closeDesc =
-00021f40: 2064 6174 612e 736f 7274 5f76 616c 7565   data.sort_value
-00021f50: 7328 6279 3d5b 2243 6c6f 7365 225d 2c20  s(by=["Close"], 
-00021f60: 6173 6365 6e64 696e 673d 4661 6c73 6529  ascending=False)
-00021f70: 0a20 2020 2020 2020 2020 2020 2076 6f6c  .            vol
-00021f80: 4465 7363 203d 2064 6174 612e 736f 7274  Desc = data.sort
-00021f90: 5f76 616c 7565 7328 6279 3d5b 2256 6f6c  _values(by=["Vol
-00021fa0: 756d 6522 5d2c 2061 7363 656e 6469 6e67  ume"], ascending
-00021fb0: 3d46 616c 7365 290a 2020 2020 2020 2020  =False).        
-00021fc0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00021fd0: 2020 2020 2020 2020 2069 6620 280a 2020           if (.  
-00021fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021ff0: 2020 6461 7461 2e65 7175 616c 7328 6f70    data.equals(op
-00022000: 656e 4465 7363 290a 2020 2020 2020 2020  enDesc).        
-00022010: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-00022020: 6461 7461 2e65 7175 616c 7328 636c 6f73  data.equals(clos
-00022030: 6544 6573 6329 0a20 2020 2020 2020 2020  eDesc).         
-00022040: 2020 2020 2020 2020 2020 2061 6e64 2064             and d
-00022050: 6174 612e 6571 7561 6c73 2876 6f6c 4465  ata.equals(volDe
-00022060: 7363 290a 2020 2020 2020 2020 2020 2020  sc).            
-00022070: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
-00022080: 2020 2020 2020 2020 2020 2023 2073 656c             # sel
-00022090: 662e 6465 6661 756c 745f 6c6f 6767 6572  f.default_logger
-000220a0: 2e69 6e66 6f28 0a20 2020 2020 2020 2020  .info(.         
-000220b0: 2020 2020 2020 2020 2020 2023 2020 2020             #    
-000220c0: 2066 2753 746f 636b 3a7b 7361 7665 4469   f'Stock:{saveDi
-000220d0: 6374 5b22 5374 6f63 6b22 5d7d 2c20 6f70  ct["Stock"]}, op
-000220e0: 656e 2c63 6c6f 7365 2061 6e64 2076 6f6c  en,close and vol
-000220f0: 756d 6520 6571 7561 6c20 6672 6f6d 2064  ume equal from d
-00022100: 6179 2062 6566 6f72 6520 7965 7374 6572  ay before yester
-00022110: 6461 792e 2041 2070 6f74 656e 7469 616c  day. A potential
-00022120: 206d 6f6d 656e 7475 6d2d 6761 696e 6572   momentum-gainer
-00022130: 2127 0a20 2020 2020 2020 2020 2020 2020  !'.             
-00022140: 2020 2020 2020 2023 2029 0a20 2020 2020         # ).     
-00022150: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00022160: 6f20 3d20 6461 7461 5b22 4f70 656e 225d  o = data["Open"]
-00022170: 2e69 6c6f 635b 305d 0a20 2020 2020 2020  .iloc[0].       
-00022180: 2020 2020 2020 2020 2020 2020 2079 6320               yc 
-00022190: 3d20 6461 7461 5b22 436c 6f73 6522 5d2e  = data["Close"].
-000221a0: 696c 6f63 5b31 5d0a 2020 2020 2020 2020  iloc[1].        
-000221b0: 2020 2020 2020 2020 2020 2020 796f 203d              yo =
+00021800: 2020 2020 2020 2020 2020 2b20 7374 7228            + str(
+00021810: 227b 3a2e 3266 7d25 222e 666f 726d 6174  "{:.2f}%".format
+00021820: 2828 6d61 784c 5450 506f 7465 6e74 6961  ((maxLTPPotentia
+00021830: 6c20 2d20 7072 6576 4c74 7029 2a31 3030  l - prevLtp)*100
+00021840: 2f70 7265 764c 7470 2929 0a20 2020 2020  /prevLtp)).     
+00021850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021860: 2020 2020 2020 202b 2063 6f6c 6f72 5465         + colorTe
+00021870: 7874 2e45 4e44 0a20 2020 2020 2020 2020  xt.END.         
+00021880: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00021890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000218a0: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
+000218b0: 745b 6622 4d61 784c 5450 225d 203d 2072  t[f"MaxLTP"] = r
+000218c0: 6f75 6e64 286d 6178 4c54 5050 6f74 656e  ound(maxLTPPoten
+000218d0: 7469 616c 2c20 3229 0a20 2020 2020 2020  tial, 2).       
+000218e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000218f0: 2073 6176 6544 6963 745b 6622 506f 742e   saveDict[f"Pot.
+00021900: 4772 7722 5d20 3d20 6622 7b72 6f75 6e64  Grw"] = f"{round
+00021910: 2828 6d61 784c 5450 506f 7465 6e74 6961  ((maxLTPPotentia
+00021920: 6c20 2d20 7072 6576 4c74 7029 2a31 3030  l - prevLtp)*100
+00021930: 2f70 7265 764c 7470 2c20 3229 7d25 220a  /prevLtp, 2)}%".
+00021940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021950: 7363 7265 656e 4469 6374 5b22 4461 7465  screenDict["Date
+00021960: 225d 203d 2063 616c 635f 6461 7465 0a20  "] = calc_date. 
+00021970: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00021980: 6176 6544 6963 745b 2244 6174 6522 5d20  aveDict["Date"] 
+00021990: 3d20 6361 6c63 5f64 6174 650a 2020 2020  = calc_date.    
+000219a0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+000219b0: 2020 2020 2020 2020 2020 2020 2020 7361                sa
+000219c0: 7665 4469 6374 5b66 224c 5450 7b70 7264  veDict[f"LTP{prd
+000219d0: 7d22 5d20 3d20 6e70 2e6e 616e 0a20 2020  }"] = np.nan.   
+000219e0: 2020 2020 2020 2020 2020 2020 2073 6176               sav
+000219f0: 6544 6963 745b 6622 4772 6f77 7468 7b70  eDict[f"Growth{p
+00021a00: 7264 7d22 5d20 3d20 6e70 2e6e 616e 0a20  rd}"] = np.nan. 
+00021a10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00021a20: 6372 6565 6e44 6963 745b 2244 6174 6522  creenDict["Date"
+00021a30: 5d20 3d20 6361 6c63 5f64 6174 650a 2020  ] = calc_date.  
+00021a40: 2020 2020 2020 2020 2020 2020 2020 7361                sa
+00021a50: 7665 4469 6374 5b22 4461 7465 225d 203d  veDict["Date"] =
+00021a60: 2063 616c 635f 6461 7465 0a0a 2020 2020   calc_date..    
+00021a70: 2320 4669 6e64 2073 746f 636b 7320 7468  # Find stocks th
+00021a80: 6174 2061 7265 2062 6561 7269 7368 2069  at are bearish i
+00021a90: 6e74 7261 6461 793a 204d 6163 6420 4869  ntraday: Macd Hi
+00021aa0: 7374 6f67 7261 6d20 6e65 6761 7469 7665  stogram negative
+00021ab0: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+00021ac0: 654d 4143 4448 6973 746f 6772 616d 4265  eMACDHistogramBe
+00021ad0: 6c6f 7730 2873 656c 662c 2064 6629 3a0a  low0(self, df):.
+00021ae0: 2020 2020 2020 2020 6966 2064 6620 6973          if df is
+00021af0: 204e 6f6e 6520 6f72 206c 656e 2864 6629   None or len(df)
+00021b00: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
+00021b10: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+00021b20: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
+00021b30: 662e 636f 7079 2829 0a20 2020 2020 2020  f.copy().       
+00021b40: 2064 6174 6120 3d20 6461 7461 2e66 696c   data = data.fil
+00021b50: 6c6e 6128 3029 0a20 2020 2020 2020 2064  lna(0).        d
+00021b60: 6174 6120 3d20 6461 7461 2e72 6570 6c61  ata = data.repla
+00021b70: 6365 285b 6e70 2e69 6e66 2c20 2d6e 702e  ce([np.inf, -np.
+00021b80: 696e 665d 2c20 3029 0a20 2020 2020 2020  inf], 0).       
+00021b90: 2064 6174 6120 3d20 6461 7461 5b3a 3a2d   data = data[::-
+00021ba0: 315d 2020 2320 5265 7665 7273 6520 7468  1]  # Reverse th
+00021bb0: 6520 6461 7461 6672 616d 6520 736f 2074  e dataframe so t
+00021bc0: 6861 7420 6974 7320 7468 6520 6f6c 6465  hat its the olde
+00021bd0: 7374 2064 6174 6520 6669 7273 740a 2020  st date first.  
+00021be0: 2020 2020 2020 6d61 6364 203d 2070 6b74        macd = pkt
+00021bf0: 616c 6962 2e4d 4143 4428 6461 7461 5b22  alib.MACD(data["
+00021c00: 436c 6f73 6522 5d2c 2031 322c 2032 362c  Close"], 12, 26,
+00021c10: 2039 295b 325d 2e74 6169 6c28 3129 0a20   9)[2].tail(1). 
+00021c20: 2020 2020 2020 2072 6574 7572 6e20 6d61         return ma
+00021c30: 6364 2e69 6c6f 635b 3a31 5d5b 305d 203c  cd.iloc[:1][0] <
+00021c40: 2030 0a0a 2020 2020 2340 6d65 6173 7572   0..    #@measur
+00021c50: 655f 7469 6d65 0a20 2020 2023 2046 696e  e_time.    # Fin
+00021c60: 6420 6966 2073 746f 636b 2067 6169 6e69  d if stock gaini
+00021c70: 6e67 2062 756c 6c69 7368 206d 6f6d 656e  ng bullish momen
+00021c80: 7475 6d0a 2020 2020 6465 6620 7661 6c69  tum.    def vali
+00021c90: 6461 7465 4d6f 6d65 6e74 756d 2873 656c  dateMomentum(sel
+00021ca0: 662c 2064 662c 2073 6372 6565 6e44 6963  f, df, screenDic
+00021cb0: 742c 2073 6176 6544 6963 7429 3a0a 2020  t, saveDict):.  
+00021cc0: 2020 2020 2020 6966 2064 6620 6973 204e        if df is N
+00021cd0: 6f6e 6520 6f72 206c 656e 2864 6629 203d  one or len(df) =
+00021ce0: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
+00021cf0: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
+00021d00: 2020 2020 2020 6461 7461 203d 2064 662e        data = df.
+00021d10: 636f 7079 2829 0a20 2020 2020 2020 2074  copy().        t
+00021d20: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00021d30: 6461 7461 203d 2064 6174 612e 6865 6164  data = data.head
+00021d40: 2833 290a 2020 2020 2020 2020 2020 2020  (3).            
+00021d50: 6966 206c 656e 2864 6174 6129 203c 2033  if len(data) < 3
+00021d60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00021d70: 2020 7265 7475 726e 2046 616c 7365 0a20    return False. 
+00021d80: 2020 2020 2020 2020 2020 2066 6f72 2072             for r
+00021d90: 6f77 2069 6e20 6461 7461 2e69 7465 7272  ow in data.iterr
+00021da0: 6f77 7328 293a 0a20 2020 2020 2020 2020  ows():.         
+00021db0: 2020 2020 2020 2023 2041 6c6c 2033 2063         # All 3 c
+00021dc0: 616e 646c 6573 2073 686f 756c 6420 6265  andles should be
+00021dd0: 2047 7265 656e 2061 6e64 204e 4f54 2043   Green and NOT C
+00021de0: 6972 6375 6974 730a 2020 2020 2020 2020  ircuits.        
+00021df0: 2020 2020 2020 2020 7963 203d 2072 6f77          yc = row
+00021e00: 5b31 5d5b 2243 6c6f 7365 225d 0a20 2020  [1]["Close"].   
+00021e10: 2020 2020 2020 2020 2020 2020 2079 6f20               yo 
+00021e20: 3d20 726f 775b 315d 5b22 4f70 656e 225d  = row[1]["Open"]
+00021e30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00021e40: 2069 6620 7963 203c 3d20 796f 3a0a 2020   if yc <= yo:.  
+00021e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021e60: 2020 2320 7365 6c66 2e64 6566 6175 6c74    # self.default
+00021e70: 5f6c 6f67 6765 722e 696e 666f 280a 2020  _logger.info(.  
+00021e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021e90: 2020 2320 2020 2020 6627 5374 6f63 6b3a    #     f'Stock:
+00021ea0: 7b73 6176 6544 6963 745b 2253 746f 636b  {saveDict["Stock
+00021eb0: 225d 7d2c 2069 7320 6e6f 7420 6120 6d6f  "]}, is not a mo
+00021ec0: 6d65 6e74 756d 2d67 6169 6e65 7220 6265  mentum-gainer be
+00021ed0: 6361 7573 6520 7965 7374 6572 6461 792d  cause yesterday-
+00021ee0: 636c 6f73 6520 287b 7963 7d29 203c 3d20  close ({yc}) <= 
+00021ef0: 7965 7374 6572 6461 792d 6f70 656e 2028  yesterday-open (
+00021f00: 7b79 6f7d 2927 0a20 2020 2020 2020 2020  {yo})'.         
+00021f10: 2020 2020 2020 2020 2020 2023 2029 0a20             # ). 
+00021f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021f30: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+00021f40: 2020 2020 2020 2020 2020 2020 6f70 656e              open
+00021f50: 4465 7363 203d 2064 6174 612e 736f 7274  Desc = data.sort
+00021f60: 5f76 616c 7565 7328 6279 3d5b 224f 7065  _values(by=["Ope
+00021f70: 6e22 5d2c 2061 7363 656e 6469 6e67 3d46  n"], ascending=F
+00021f80: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
+00021f90: 2020 636c 6f73 6544 6573 6320 3d20 6461    closeDesc = da
+00021fa0: 7461 2e73 6f72 745f 7661 6c75 6573 2862  ta.sort_values(b
+00021fb0: 793d 5b22 436c 6f73 6522 5d2c 2061 7363  y=["Close"], asc
+00021fc0: 656e 6469 6e67 3d46 616c 7365 290a 2020  ending=False).  
+00021fd0: 2020 2020 2020 2020 2020 766f 6c44 6573            volDes
+00021fe0: 6320 3d20 6461 7461 2e73 6f72 745f 7661  c = data.sort_va
+00021ff0: 6c75 6573 2862 793d 5b22 566f 6c75 6d65  lues(by=["Volume
+00022000: 225d 2c20 6173 6365 6e64 696e 673d 4661  "], ascending=Fa
+00022010: 6c73 6529 0a20 2020 2020 2020 2020 2020  lse).           
+00022020: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00022030: 2020 2020 2020 6966 2028 0a20 2020 2020        if (.     
+00022040: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00022050: 6174 612e 6571 7561 6c73 286f 7065 6e44  ata.equals(openD
+00022060: 6573 6329 0a20 2020 2020 2020 2020 2020  esc).           
+00022070: 2020 2020 2020 2020 2061 6e64 2064 6174           and dat
+00022080: 612e 6571 7561 6c73 2863 6c6f 7365 4465  a.equals(closeDe
+00022090: 7363 290a 2020 2020 2020 2020 2020 2020  sc).            
+000220a0: 2020 2020 2020 2020 616e 6420 6461 7461          and data
+000220b0: 2e65 7175 616c 7328 766f 6c44 6573 6329  .equals(volDesc)
+000220c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000220d0: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
+000220e0: 2020 2020 2020 2020 2320 7365 6c66 2e64          # self.d
+000220f0: 6566 6175 6c74 5f6c 6f67 6765 722e 696e  efault_logger.in
+00022100: 666f 280a 2020 2020 2020 2020 2020 2020  fo(.            
+00022110: 2020 2020 2020 2020 2320 2020 2020 6627          #     f'
+00022120: 5374 6f63 6b3a 7b73 6176 6544 6963 745b  Stock:{saveDict[
+00022130: 2253 746f 636b 225d 7d2c 206f 7065 6e2c  "Stock"]}, open,
+00022140: 636c 6f73 6520 616e 6420 766f 6c75 6d65  close and volume
+00022150: 2065 7175 616c 2066 726f 6d20 6461 7920   equal from day 
+00022160: 6265 666f 7265 2079 6573 7465 7264 6179  before yesterday
+00022170: 2e20 4120 706f 7465 6e74 6961 6c20 6d6f  . A potential mo
+00022180: 6d65 6e74 756d 2d67 6169 6e65 7221 270a  mentum-gainer!'.
+00022190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000221a0: 2020 2020 2320 290a 2020 2020 2020 2020      # ).        
+000221b0: 2020 2020 2020 2020 2020 2020 746f 203d              to =
 000221c0: 2064 6174 615b 224f 7065 6e22 5d2e 696c   data["Open"].il
-000221d0: 6f63 5b31 5d0a 2020 2020 2020 2020 2020  oc[1].          
-000221e0: 2020 2020 2020 2020 2020 6479 6320 3d20            dyc = 
-000221f0: 6461 7461 5b22 436c 6f73 6522 5d2e 696c  data["Close"].il
-00022200: 6f63 5b32 5d0a 2020 2020 2020 2020 2020  oc[2].          
-00022210: 2020 2020 2020 2020 2020 6966 2028 746f            if (to
-00022220: 203e 3d20 7963 2920 616e 6420 2879 6f20   >= yc) and (yo 
-00022230: 3e3d 2064 7963 293a 0a20 2020 2020 2020  >= dyc):.       
-00022240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022250: 2023 2073 656c 662e 6465 6661 756c 745f   # self.default_
-00022260: 6c6f 6767 6572 2e69 6e66 6f28 0a20 2020  logger.info(.   
-00022270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022280: 2020 2020 2023 2020 2020 2066 2753 746f       #     f'Sto
-00022290: 636b 3a7b 7361 7665 4469 6374 5b22 5374  ck:{saveDict["St
-000222a0: 6f63 6b22 5d7d 2c20 6973 2061 206d 6f6d  ock"]}, is a mom
-000222b0: 656e 7475 6d2d 6761 696e 6572 2062 6563  entum-gainer bec
-000222c0: 6175 7365 2074 6f64 6179 2d6f 7065 6e20  ause today-open 
-000222d0: 287b 746f 7d29 203e 3d20 7965 7374 6572  ({to}) >= yester
-000222e0: 6461 792d 636c 6f73 6520 287b 7963 7d29  day-close ({yc})
-000222f0: 2061 6e64 2079 6573 7465 7264 6179 2d6f   and yesterday-o
-00022300: 7065 6e28 7b79 6f7d 2920 3e3d 2064 6179  pen({yo}) >= day
-00022310: 2d62 6566 6f72 652d 636c 6f73 6528 7b64  -before-close({d
-00022320: 7963 7d29 270a 2020 2020 2020 2020 2020  yc})'.          
-00022330: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00022340: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00022350: 2020 2020 2020 2020 2020 7361 7665 6420            saved 
-00022360: 3d20 7365 6c66 2e66 696e 6443 7572 7265  = self.findCurre
-00022370: 6e74 5361 7665 6456 616c 7565 2873 6372  ntSavedValue(scr
-00022380: 6565 6e44 6963 742c 2073 6176 6544 6963  eenDict, saveDic
-00022390: 742c 2022 5061 7474 6572 6e22 290a 2020  t, "Pattern").  
+000221d0: 6f63 5b30 5d0a 2020 2020 2020 2020 2020  oc[0].          
+000221e0: 2020 2020 2020 2020 2020 7963 203d 2064            yc = d
+000221f0: 6174 615b 2243 6c6f 7365 225d 2e69 6c6f  ata["Close"].ilo
+00022200: 635b 315d 0a20 2020 2020 2020 2020 2020  c[1].           
+00022210: 2020 2020 2020 2020 2079 6f20 3d20 6461           yo = da
+00022220: 7461 5b22 4f70 656e 225d 2e69 6c6f 635b  ta["Open"].iloc[
+00022230: 315d 0a20 2020 2020 2020 2020 2020 2020  1].             
+00022240: 2020 2020 2020 2064 7963 203d 2064 6174         dyc = dat
+00022250: 615b 2243 6c6f 7365 225d 2e69 6c6f 635b  a["Close"].iloc[
+00022260: 325d 0a20 2020 2020 2020 2020 2020 2020  2].             
+00022270: 2020 2020 2020 2069 6620 2874 6f20 3e3d         if (to >=
+00022280: 2079 6329 2061 6e64 2028 796f 203e 3d20   yc) and (yo >= 
+00022290: 6479 6329 3a0a 2020 2020 2020 2020 2020  dyc):.          
+000222a0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+000222b0: 7365 6c66 2e64 6566 6175 6c74 5f6c 6f67  self.default_log
+000222c0: 6765 722e 696e 666f 280a 2020 2020 2020  ger.info(.      
+000222d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000222e0: 2020 2320 2020 2020 6627 5374 6f63 6b3a    #     f'Stock:
+000222f0: 7b73 6176 6544 6963 745b 2253 746f 636b  {saveDict["Stock
+00022300: 225d 7d2c 2069 7320 6120 6d6f 6d65 6e74  "]}, is a moment
+00022310: 756d 2d67 6169 6e65 7220 6265 6361 7573  um-gainer becaus
+00022320: 6520 746f 6461 792d 6f70 656e 2028 7b74  e today-open ({t
+00022330: 6f7d 2920 3e3d 2079 6573 7465 7264 6179  o}) >= yesterday
+00022340: 2d63 6c6f 7365 2028 7b79 637d 2920 616e  -close ({yc}) an
+00022350: 6420 7965 7374 6572 6461 792d 6f70 656e  d yesterday-open
+00022360: 287b 796f 7d29 203e 3d20 6461 792d 6265  ({yo}) >= day-be
+00022370: 666f 7265 2d63 6c6f 7365 287b 6479 637d  fore-close({dyc}
+00022380: 2927 0a20 2020 2020 2020 2020 2020 2020  )'.             
+00022390: 2020 2020 2020 2020 2020 2023 2029 0a20             # ). 
 000223a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000223b0: 2020 2020 2020 7363 7265 656e 4469 6374        screenDict
-000223c0: 5b22 5061 7474 6572 6e22 5d20 3d20 280a  ["Pattern"] = (.
-000223d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000223e0: 2020 2020 2020 2020 2020 2020 7361 7665              save
-000223f0: 645b 305d 0a20 2020 2020 2020 2020 2020  d[0].           
+000223b0: 2020 2020 2020 2073 6176 6564 203d 2073         saved = s
+000223c0: 656c 662e 6669 6e64 4375 7272 656e 7453  elf.findCurrentS
+000223d0: 6176 6564 5661 6c75 6528 7363 7265 656e  avedValue(screen
+000223e0: 4469 6374 2c20 7361 7665 4469 6374 2c20  Dict, saveDict, 
+000223f0: 2250 6174 7465 726e 2229 0a20 2020 2020  "Pattern").     
 00022400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022410: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
-00022420: 440a 2020 2020 2020 2020 2020 2020 2020  D.              
-00022430: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-00022440: 636f 6c6f 7254 6578 742e 4752 4545 4e0a  colorText.GREEN.
-00022450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022460: 2020 2020 2020 2020 2020 2020 2b20 224d              + "M
-00022470: 6f6d 656e 7475 6d20 4761 696e 6572 220a  omentum Gainer".
+00022410: 2020 2073 6372 6565 6e44 6963 745b 2250     screenDict["P
+00022420: 6174 7465 726e 225d 203d 2028 0a20 2020  attern"] = (.   
+00022430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022440: 2020 2020 2020 2020 2073 6176 6564 5b30           saved[0
+00022450: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00022460: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+00022470: 636f 6c6f 7254 6578 742e 424f 4c44 0a20  colorText.BOLD. 
 00022480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022490: 2020 2020 2020 2020 2020 2020 2b20 636f              + co
-000224a0: 6c6f 7254 6578 742e 454e 440a 2020 2020  lorText.END.    
+00022490: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
+000224a0: 6f72 5465 7874 2e47 5245 454e 0a20 2020  orText.GREEN.   
 000224b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000224c0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-000224d0: 2020 2020 2020 2020 2020 2020 2020 7361                sa
-000224e0: 7665 4469 6374 5b22 5061 7474 6572 6e22  veDict["Pattern"
-000224f0: 5d20 3d20 7361 7665 645b 315d 202b 2022  ] = saved[1] + "
-00022500: 4d6f 6d65 6e74 756d 2047 6169 6e65 7222  Momentum Gainer"
-00022510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00022520: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00022530: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
-00022540: 2020 2020 2020 2020 2023 2073 656c 662e           # self.
-00022550: 6465 6661 756c 745f 6c6f 6767 6572 2e69  default_logger.i
-00022560: 6e66 6f28 0a20 2020 2020 2020 2020 2020  nfo(.           
-00022570: 2020 2020 2020 2020 2023 2020 2020 2066           #     f
-00022580: 2753 746f 636b 3a7b 7361 7665 4469 6374  'Stock:{saveDict
-00022590: 5b22 5374 6f63 6b22 5d7d 2c20 6973 206e  ["Stock"]}, is n
-000225a0: 6f74 2061 206d 6f6d 656e 7475 6d2d 6761  ot a momentum-ga
-000225b0: 696e 6572 2062 6563 6175 7365 2065 6974  iner because eit
-000225c0: 6865 7220 746f 6461 792d 6f70 656e 2028  her today-open (
-000225d0: 7b74 6f7d 2920 3c20 7965 7374 6572 6461  {to}) < yesterda
-000225e0: 792d 636c 6f73 6520 287b 7963 7d29 206f  y-close ({yc}) o
-000225f0: 7220 7965 7374 6572 6461 792d 6f70 656e  r yesterday-open
-00022600: 287b 796f 7d29 203c 2064 6179 2d62 6566  ({yo}) < day-bef
-00022610: 6f72 652d 636c 6f73 6528 7b64 7963 7d29  ore-close({dyc})
-00022620: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-00022630: 2020 2020 2020 2320 290a 2020 2020 2020        # ).      
-00022640: 2020 2020 2020 6578 6365 7074 2049 6e64        except Ind
-00022650: 6578 4572 726f 7220 6173 2065 3a20 2320  exError as e: # 
-00022660: 7072 6167 6d61 3a20 6e6f 2063 6f76 6572  pragma: no cover
-00022670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00022680: 2073 656c 662e 6465 6661 756c 745f 6c6f   self.default_lo
-00022690: 6767 6572 2e64 6562 7567 2865 2c20 6578  gger.debug(e, ex
-000226a0: 635f 696e 666f 3d54 7275 6529 0a20 2020  c_info=True).   
-000226b0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000226c0: 662e 6465 6661 756c 745f 6c6f 6767 6572  f.default_logger
-000226d0: 2e64 6562 7567 2864 6174 6129 0a20 2020  .debug(data).   
-000226e0: 2020 2020 2020 2020 2020 2020 2070 6173               pas
-000226f0: 730a 2020 2020 2020 2020 2020 2020 7265  s.            re
-00022700: 7475 726e 2046 616c 7365 0a20 2020 2020  turn False.     
-00022710: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-00022720: 696f 6e20 6173 2065 3a20 2023 2070 7261  ion as e:  # pra
-00022730: 676d 613a 206e 6f20 636f 7665 720a 2020  gma: no cover.  
-00022740: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-00022750: 6566 6175 6c74 5f6c 6f67 6765 722e 6465  efault_logger.de
-00022760: 6275 6728 652c 2065 7863 5f69 6e66 6f3d  bug(e, exc_info=
-00022770: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
-00022780: 2020 7265 7475 726e 2046 616c 7365 0a0a    return False..
-00022790: 2020 2020 2340 6d65 6173 7572 655f 7469      #@measure_ti
-000227a0: 6d65 0a20 2020 2023 2056 616c 6964 6174  me.    # Validat
-000227b0: 6520 4d6f 7669 6e67 2061 7665 7261 6765  e Moving average
-000227c0: 7320 616e 6420 6c6f 6f6b 2066 6f72 2062  s and look for b
-000227d0: 7579 2f73 656c 6c20 7369 676e 616c 730a  uy/sell signals.
-000227e0: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-000227f0: 4d6f 7669 6e67 4176 6572 6167 6573 2873  MovingAverages(s
-00022800: 656c 662c 2064 662c 2073 6372 6565 6e44  elf, df, screenD
-00022810: 6963 742c 2073 6176 6544 6963 742c 206d  ict, saveDict, m
-00022820: 6152 616e 6765 3d32 2e35 2c6d 614c 656e  aRange=2.5,maLen
-00022830: 6774 683d 3029 3a0a 2020 2020 2020 2020  gth=0):.        
-00022840: 6461 7461 203d 2064 662e 636f 7079 2829  data = df.copy()
-00022850: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
-00022860: 6461 7461 2e66 696c 6c6e 6128 3029 0a20  data.fillna(0). 
-00022870: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
-00022880: 7461 2e72 6570 6c61 6365 285b 6e70 2e69  ta.replace([np.i
-00022890: 6e66 2c20 2d6e 702e 696e 665d 2c20 3029  nf, -np.inf], 0)
-000228a0: 0a20 2020 2020 2020 2072 6563 656e 7420  .        recent 
-000228b0: 3d20 6461 7461 2e68 6561 6428 3129 0a20  = data.head(1). 
-000228c0: 2020 2020 2020 206d 6153 6967 6e61 6c73         maSignals
-000228d0: 203d 205b 5d0a 2020 2020 2020 2020 6966   = [].        if
-000228e0: 2073 7472 286d 614c 656e 6774 6829 2069   str(maLength) i
-000228f0: 6e20 5b22 3022 2c22 3222 2c22 3322 5d3a  n ["0","2","3"]:
-00022900: 0a20 2020 2020 2020 2020 2020 2073 6176  .            sav
-00022910: 6564 203d 2073 656c 662e 6669 6e64 4375  ed = self.findCu
-00022920: 7272 656e 7453 6176 6564 5661 6c75 6528  rrentSavedValue(
-00022930: 7363 7265 656e 4469 6374 2c73 6176 6544  screenDict,saveD
-00022940: 6963 742c 224d 412d 5369 676e 616c 2229  ict,"MA-Signal")
-00022950: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00022960: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00022970: 2020 7265 6365 6e74 5b22 534d 4122 5d2e    recent["SMA"].
-00022980: 696c 6f63 5b30 5d20 3e20 7265 6365 6e74  iloc[0] > recent
-00022990: 5b22 4c4d 4122 5d2e 696c 6f63 5b30 5d0a  ["LMA"].iloc[0].
-000229a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000229b0: 616e 6420 7265 6365 6e74 5b22 436c 6f73  and recent["Clos
-000229c0: 6522 5d2e 696c 6f63 5b30 5d20 3e20 7265  e"].iloc[0] > re
-000229d0: 6365 6e74 5b22 534d 4122 5d2e 696c 6f63  cent["SMA"].iloc
-000229e0: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
-000229f0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00022a00: 2020 2073 6372 6565 6e44 6963 745b 224d     screenDict["M
-00022a10: 412d 5369 676e 616c 225d 203d 2028 0a20  A-Signal"] = (. 
-00022a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022a30: 2020 2073 6176 6564 5b30 5d20 2b20 636f     saved[0] + co
-00022a40: 6c6f 7254 6578 742e 424f 4c44 202b 2063  lorText.BOLD + c
-00022a50: 6f6c 6f72 5465 7874 2e47 5245 454e 202b  olorText.GREEN +
-00022a60: 2022 4275 6c6c 6973 6822 202b 2063 6f6c   "Bullish" + col
-00022a70: 6f72 5465 7874 2e45 4e44 0a20 2020 2020  orText.END.     
-00022a80: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00022a90: 2020 2020 2020 2020 2020 2020 2073 6176               sav
-00022aa0: 6544 6963 745b 224d 412d 5369 676e 616c  eDict["MA-Signal
-00022ab0: 225d 203d 2073 6176 6564 5b31 5d20 2b20  "] = saved[1] + 
-00022ac0: 2242 756c 6c69 7368 220a 2020 2020 2020  "Bullish".      
-00022ad0: 2020 2020 2020 2020 2020 6d61 5369 676e            maSign
-00022ae0: 616c 732e 6170 7065 6e64 2822 3322 290a  als.append("3").
-00022af0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-00022b00: 2072 6563 656e 745b 2253 4d41 225d 2e69   recent["SMA"].i
-00022b10: 6c6f 635b 305d 203c 2072 6563 656e 745b  loc[0] < recent[
-00022b20: 224c 4d41 225d 2e69 6c6f 635b 305d 3a0a  "LMA"].iloc[0]:.
-00022b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022b40: 7363 7265 656e 4469 6374 5b22 4d41 2d53  screenDict["MA-S
-00022b50: 6967 6e61 6c22 5d20 3d20 280a 2020 2020  ignal"] = (.    
-00022b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022b70: 7361 7665 645b 305d 202b 2063 6f6c 6f72  saved[0] + color
-00022b80: 5465 7874 2e42 4f4c 4420 2b20 636f 6c6f  Text.BOLD + colo
-00022b90: 7254 6578 742e 4641 494c 202b 2022 4265  rText.FAIL + "Be
-00022ba0: 6172 6973 6822 202b 2063 6f6c 6f72 5465  arish" + colorTe
-00022bb0: 7874 2e45 4e44 0a20 2020 2020 2020 2020  xt.END.         
-00022bc0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00022bd0: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
-00022be0: 745b 224d 412d 5369 676e 616c 225d 203d  t["MA-Signal"] =
-00022bf0: 2073 6176 6564 5b31 5d20 2b20 2242 6561   saved[1] + "Bea
-00022c00: 7269 7368 220a 2020 2020 2020 2020 2020  rish".          
-00022c10: 2020 2020 2020 6d61 5369 676e 616c 732e        maSignals.
-00022c20: 6170 7065 6e64 2822 3222 290a 2020 2020  append("2").    
-00022c30: 2020 2020 2020 2020 656c 6966 2072 6563          elif rec
-00022c40: 656e 745b 2253 4d41 225d 2e69 6c6f 635b  ent["SMA"].iloc[
-00022c50: 305d 203d 3d20 303a 0a20 2020 2020 2020  0] == 0:.       
-00022c60: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
-00022c70: 6963 745b 224d 412d 5369 676e 616c 225d  ict["MA-Signal"]
-00022c80: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
-00022c90: 2020 2020 2020 2020 2073 6176 6564 5b30           saved[0
-00022ca0: 5d20 2b20 636f 6c6f 7254 6578 742e 424f  ] + colorText.BO
-00022cb0: 4c44 202b 2063 6f6c 6f72 5465 7874 2e57  LD + colorText.W
-00022cc0: 4152 4e20 2b20 2255 6e6b 6e6f 776e 2220  ARN + "Unknown" 
-00022cd0: 2b20 636f 6c6f 7254 6578 742e 454e 440a  + colorText.END.
-00022ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022cf0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00022d00: 2020 7361 7665 4469 6374 5b22 4d41 2d53    saveDict["MA-S
-00022d10: 6967 6e61 6c22 5d20 3d20 7361 7665 645b  ignal"] = saved[
-00022d20: 315d 202b 2022 556e 6b6e 6f77 6e22 0a20  1] + "Unknown". 
-00022d30: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00022d40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00022d50: 2073 6372 6565 6e44 6963 745b 224d 412d   screenDict["MA-
-00022d60: 5369 676e 616c 225d 203d 2028 0a20 2020  Signal"] = (.   
-00022d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022d80: 2073 6176 6564 5b30 5d20 2b20 636f 6c6f   saved[0] + colo
-00022d90: 7254 6578 742e 424f 4c44 202b 2063 6f6c  rText.BOLD + col
-00022da0: 6f72 5465 7874 2e57 4152 4e20 2b20 224e  orText.WARN + "N
-00022db0: 6575 7472 616c 2220 2b20 636f 6c6f 7254  eutral" + colorT
-00022dc0: 6578 742e 454e 440a 2020 2020 2020 2020  ext.END.        
-00022dd0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00022de0: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
-00022df0: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d20  ct["MA-Signal"] 
-00022e00: 3d20 7361 7665 645b 315d 202b 2022 4e65  = saved[1] + "Ne
-00022e10: 7574 7261 6c22 0a20 2020 2020 2020 2072  utral".        r
-00022e20: 6576 6572 7365 6444 6174 6120 3d20 6461  eversedData = da
-00022e30: 7461 5b3a 3a2d 315d 2020 2320 5265 7665  ta[::-1]  # Reve
-00022e40: 7273 6520 7468 6520 6461 7461 6672 616d  rse the datafram
-00022e50: 650a 2020 2020 2020 2020 656d 615f 3230  e.        ema_20
-00022e60: 203d 2070 6b74 616c 6962 2e45 4d41 2872   = pktalib.EMA(r
-00022e70: 6576 6572 7365 6444 6174 615b 2243 6c6f  eversedData["Clo
-00022e80: 7365 225d 2c32 3029 2e74 6169 6c28 3129  se"],20).tail(1)
-00022e90: 2e69 6c6f 635b 305d 0a20 2020 2020 2020  .iloc[0].       
-00022ea0: 2076 7761 7020 3d20 706b 7461 6c69 622e   vwap = pktalib.
-00022eb0: 5657 4150 2872 6576 6572 7365 6444 6174  VWAP(reversedDat
-00022ec0: 615b 2248 6967 6822 5d2c 7265 7665 7273  a["High"],revers
-00022ed0: 6564 4461 7461 5b22 4c6f 7722 5d2c 7265  edData["Low"],re
-00022ee0: 7665 7273 6564 4461 7461 5b22 436c 6f73  versedData["Clos
-00022ef0: 6522 5d2c 7265 7665 7273 6564 4461 7461  e"],reversedData
-00022f00: 5b22 566f 6c75 6d65 225d 292e 7461 696c  ["Volume"]).tail
-00022f10: 2831 292e 696c 6f63 5b30 5d0a 2020 2020  (1).iloc[0].    
-00022f20: 2020 2020 736d 6144 6576 203d 2064 6174      smaDev = dat
-00022f30: 615b 2253 4d41 225d 2e69 6c6f 635b 305d  a["SMA"].iloc[0]
-00022f40: 202a 206d 6152 616e 6765 202f 2031 3030   * maRange / 100
-00022f50: 0a20 2020 2020 2020 206c 6d61 4465 7620  .        lmaDev 
-00022f60: 3d20 6461 7461 5b22 4c4d 4122 5d2e 696c  = data["LMA"].il
-00022f70: 6f63 5b30 5d20 2a20 6d61 5261 6e67 6520  oc[0] * maRange 
-00022f80: 2f20 3130 300a 2020 2020 2020 2020 656d  / 100.        em
-00022f90: 6144 6576 203d 2065 6d61 5f32 3020 2a20  aDev = ema_20 * 
+000224c0: 2020 2020 2020 2020 202b 2022 4d6f 6d65           + "Mome
+000224d0: 6e74 756d 2047 6169 6e65 7222 0a20 2020  ntum Gainer".   
+000224e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000224f0: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
+00022500: 5465 7874 2e45 4e44 0a20 2020 2020 2020  Text.END.       
+00022510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022520: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+00022530: 2020 2020 2020 2020 2020 2073 6176 6544             saveD
+00022540: 6963 745b 2250 6174 7465 726e 225d 203d  ict["Pattern"] =
+00022550: 2073 6176 6564 5b31 5d20 2b20 224d 6f6d   saved[1] + "Mom
+00022560: 656e 7475 6d20 4761 696e 6572 220a 2020  entum Gainer".  
+00022570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022580: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
+00022590: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+000225a0: 2020 2020 2020 2320 7365 6c66 2e64 6566        # self.def
+000225b0: 6175 6c74 5f6c 6f67 6765 722e 696e 666f  ault_logger.info
+000225c0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000225d0: 2020 2020 2020 2320 2020 2020 6627 5374        #     f'St
+000225e0: 6f63 6b3a 7b73 6176 6544 6963 745b 2253  ock:{saveDict["S
+000225f0: 746f 636b 225d 7d2c 2069 7320 6e6f 7420  tock"]}, is not 
+00022600: 6120 6d6f 6d65 6e74 756d 2d67 6169 6e65  a momentum-gaine
+00022610: 7220 6265 6361 7573 6520 6569 7468 6572  r because either
+00022620: 2074 6f64 6179 2d6f 7065 6e20 287b 746f   today-open ({to
+00022630: 7d29 203c 2079 6573 7465 7264 6179 2d63  }) < yesterday-c
+00022640: 6c6f 7365 2028 7b79 637d 2920 6f72 2079  lose ({yc}) or y
+00022650: 6573 7465 7264 6179 2d6f 7065 6e28 7b79  esterday-open({y
+00022660: 6f7d 2920 3c20 6461 792d 6265 666f 7265  o}) < day-before
+00022670: 2d63 6c6f 7365 287b 6479 637d 2927 0a20  -close({dyc})'. 
+00022680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022690: 2020 2023 2029 0a20 2020 2020 2020 2020     # ).         
+000226a0: 2020 2065 7863 6570 7420 496e 6465 7845     except IndexE
+000226b0: 7272 6f72 2061 7320 653a 2023 2070 7261  rror as e: # pra
+000226c0: 676d 613a 206e 6f20 636f 7665 720a 2020  gma: no cover.  
+000226d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000226e0: 6c66 2e64 6566 6175 6c74 5f6c 6f67 6765  lf.default_logge
+000226f0: 722e 6465 6275 6728 652c 2065 7863 5f69  r.debug(e, exc_i
+00022700: 6e66 6f3d 5472 7565 290a 2020 2020 2020  nfo=True).      
+00022710: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+00022720: 6566 6175 6c74 5f6c 6f67 6765 722e 6465  efault_logger.de
+00022730: 6275 6728 6461 7461 290a 2020 2020 2020  bug(data).      
+00022740: 2020 2020 2020 2020 2020 7061 7373 0a20            pass. 
+00022750: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00022760: 6e20 4661 6c73 650a 2020 2020 2020 2020  n False.        
+00022770: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
+00022780: 2061 7320 653a 2020 2320 7072 6167 6d61   as e:  # pragma
+00022790: 3a20 6e6f 2063 6f76 6572 0a20 2020 2020  : no cover.     
+000227a0: 2020 2020 2020 2073 656c 662e 6465 6661         self.defa
+000227b0: 756c 745f 6c6f 6767 6572 2e64 6562 7567  ult_logger.debug
+000227c0: 2865 2c20 6578 635f 696e 666f 3d54 7275  (e, exc_info=Tru
+000227d0: 6529 0a20 2020 2020 2020 2020 2020 2072  e).            r
+000227e0: 6574 7572 6e20 4661 6c73 650a 0a20 2020  eturn False..   
+000227f0: 2023 406d 6561 7375 7265 5f74 696d 650a   #@measure_time.
+00022800: 2020 2020 2320 5661 6c69 6461 7465 204d      # Validate M
+00022810: 6f76 696e 6720 6176 6572 6167 6573 2061  oving averages a
+00022820: 6e64 206c 6f6f 6b20 666f 7220 6275 792f  nd look for buy/
+00022830: 7365 6c6c 2073 6967 6e61 6c73 0a20 2020  sell signals.   
+00022840: 2064 6566 2076 616c 6964 6174 654d 6f76   def validateMov
+00022850: 696e 6741 7665 7261 6765 7328 7365 6c66  ingAverages(self
+00022860: 2c20 6466 2c20 7363 7265 656e 4469 6374  , df, screenDict
+00022870: 2c20 7361 7665 4469 6374 2c20 6d61 5261  , saveDict, maRa
+00022880: 6e67 653d 322e 352c 6d61 4c65 6e67 7468  nge=2.5,maLength
+00022890: 3d30 293a 0a20 2020 2020 2020 2064 6174  =0):.        dat
+000228a0: 6120 3d20 6466 2e63 6f70 7928 290a 2020  a = df.copy().  
+000228b0: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
+000228c0: 612e 6669 6c6c 6e61 2830 290a 2020 2020  a.fillna(0).    
+000228d0: 2020 2020 6461 7461 203d 2064 6174 612e      data = data.
+000228e0: 7265 706c 6163 6528 5b6e 702e 696e 662c  replace([np.inf,
+000228f0: 202d 6e70 2e69 6e66 5d2c 2030 290a 2020   -np.inf], 0).  
+00022900: 2020 2020 2020 7265 6365 6e74 203d 2064        recent = d
+00022910: 6174 612e 6865 6164 2831 290a 2020 2020  ata.head(1).    
+00022920: 2020 2020 6d61 5369 676e 616c 7320 3d20      maSignals = 
+00022930: 5b5d 0a20 2020 2020 2020 2069 6620 7374  [].        if st
+00022940: 7228 6d61 4c65 6e67 7468 2920 696e 205b  r(maLength) in [
+00022950: 2230 222c 2232 222c 2233 225d 3a0a 2020  "0","2","3"]:.  
+00022960: 2020 2020 2020 2020 2020 7361 7665 6420            saved 
+00022970: 3d20 7365 6c66 2e66 696e 6443 7572 7265  = self.findCurre
+00022980: 6e74 5361 7665 6456 616c 7565 2873 6372  ntSavedValue(scr
+00022990: 6565 6e44 6963 742c 7361 7665 4469 6374  eenDict,saveDict
+000229a0: 2c22 4d41 2d53 6967 6e61 6c22 290a 2020  ,"MA-Signal").  
+000229b0: 2020 2020 2020 2020 2020 6966 2028 0a20            if (. 
+000229c0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000229d0: 6563 656e 745b 2253 4d41 225d 2e69 6c6f  ecent["SMA"].ilo
+000229e0: 635b 305d 203e 2072 6563 656e 745b 224c  c[0] > recent["L
+000229f0: 4d41 225d 2e69 6c6f 635b 305d 0a20 2020  MA"].iloc[0].   
+00022a00: 2020 2020 2020 2020 2020 2020 2061 6e64               and
+00022a10: 2072 6563 656e 745b 2243 6c6f 7365 225d   recent["Close"]
+00022a20: 2e69 6c6f 635b 305d 203e 2072 6563 656e  .iloc[0] > recen
+00022a30: 745b 2253 4d41 225d 2e69 6c6f 635b 305d  t["SMA"].iloc[0]
+00022a40: 0a20 2020 2020 2020 2020 2020 2029 3a0a  .            ):.
+00022a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022a60: 7363 7265 656e 4469 6374 5b22 4d41 2d53  screenDict["MA-S
+00022a70: 6967 6e61 6c22 5d20 3d20 280a 2020 2020  ignal"] = (.    
+00022a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022a90: 7361 7665 645b 305d 202b 2063 6f6c 6f72  saved[0] + color
+00022aa0: 5465 7874 2e42 4f4c 4420 2b20 636f 6c6f  Text.BOLD + colo
+00022ab0: 7254 6578 742e 4752 4545 4e20 2b20 2242  rText.GREEN + "B
+00022ac0: 756c 6c69 7368 2220 2b20 636f 6c6f 7254  ullish" + colorT
+00022ad0: 6578 742e 454e 440a 2020 2020 2020 2020  ext.END.        
+00022ae0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00022af0: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
+00022b00: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d20  ct["MA-Signal"] 
+00022b10: 3d20 7361 7665 645b 315d 202b 2022 4275  = saved[1] + "Bu
+00022b20: 6c6c 6973 6822 0a20 2020 2020 2020 2020  llish".         
+00022b30: 2020 2020 2020 206d 6153 6967 6e61 6c73         maSignals
+00022b40: 2e61 7070 656e 6428 2233 2229 0a20 2020  .append("3").   
+00022b50: 2020 2020 2020 2020 2065 6c69 6620 7265           elif re
+00022b60: 6365 6e74 5b22 534d 4122 5d2e 696c 6f63  cent["SMA"].iloc
+00022b70: 5b30 5d20 3c20 7265 6365 6e74 5b22 4c4d  [0] < recent["LM
+00022b80: 4122 5d2e 696c 6f63 5b30 5d3a 0a20 2020  A"].iloc[0]:.   
+00022b90: 2020 2020 2020 2020 2020 2020 2073 6372               scr
+00022ba0: 6565 6e44 6963 745b 224d 412d 5369 676e  eenDict["MA-Sign
+00022bb0: 616c 225d 203d 2028 0a20 2020 2020 2020  al"] = (.       
+00022bc0: 2020 2020 2020 2020 2020 2020 2073 6176               sav
+00022bd0: 6564 5b30 5d20 2b20 636f 6c6f 7254 6578  ed[0] + colorTex
+00022be0: 742e 424f 4c44 202b 2063 6f6c 6f72 5465  t.BOLD + colorTe
+00022bf0: 7874 2e46 4149 4c20 2b20 2242 6561 7269  xt.FAIL + "Beari
+00022c00: 7368 2220 2b20 636f 6c6f 7254 6578 742e  sh" + colorText.
+00022c10: 454e 440a 2020 2020 2020 2020 2020 2020  END.            
+00022c20: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00022c30: 2020 2020 2020 7361 7665 4469 6374 5b22        saveDict["
+00022c40: 4d41 2d53 6967 6e61 6c22 5d20 3d20 7361  MA-Signal"] = sa
+00022c50: 7665 645b 315d 202b 2022 4265 6172 6973  ved[1] + "Bearis
+00022c60: 6822 0a20 2020 2020 2020 2020 2020 2020  h".             
+00022c70: 2020 206d 6153 6967 6e61 6c73 2e61 7070     maSignals.app
+00022c80: 656e 6428 2232 2229 0a20 2020 2020 2020  end("2").       
+00022c90: 2020 2020 2065 6c69 6620 7265 6365 6e74       elif recent
+00022ca0: 5b22 534d 4122 5d2e 696c 6f63 5b30 5d20  ["SMA"].iloc[0] 
+00022cb0: 3d3d 2030 3a0a 2020 2020 2020 2020 2020  == 0:.          
+00022cc0: 2020 2020 2020 7363 7265 656e 4469 6374        screenDict
+00022cd0: 5b22 4d41 2d53 6967 6e61 6c22 5d20 3d20  ["MA-Signal"] = 
+00022ce0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00022cf0: 2020 2020 2020 7361 7665 645b 305d 202b        saved[0] +
+00022d00: 2063 6f6c 6f72 5465 7874 2e42 4f4c 4420   colorText.BOLD 
+00022d10: 2b20 636f 6c6f 7254 6578 742e 5741 524e  + colorText.WARN
+00022d20: 202b 2022 556e 6b6e 6f77 6e22 202b 2063   + "Unknown" + c
+00022d30: 6f6c 6f72 5465 7874 2e45 4e44 0a20 2020  olorText.END.   
+00022d40: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+00022d50: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00022d60: 6176 6544 6963 745b 224d 412d 5369 676e  aveDict["MA-Sign
+00022d70: 616c 225d 203d 2073 6176 6564 5b31 5d20  al"] = saved[1] 
+00022d80: 2b20 2255 6e6b 6e6f 776e 220a 2020 2020  + "Unknown".    
+00022d90: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00022da0: 2020 2020 2020 2020 2020 2020 2020 7363                sc
+00022db0: 7265 656e 4469 6374 5b22 4d41 2d53 6967  reenDict["MA-Sig
+00022dc0: 6e61 6c22 5d20 3d20 280a 2020 2020 2020  nal"] = (.      
+00022dd0: 2020 2020 2020 2020 2020 2020 2020 7361                sa
+00022de0: 7665 645b 305d 202b 2063 6f6c 6f72 5465  ved[0] + colorTe
+00022df0: 7874 2e42 4f4c 4420 2b20 636f 6c6f 7254  xt.BOLD + colorT
+00022e00: 6578 742e 5741 524e 202b 2022 4e65 7574  ext.WARN + "Neut
+00022e10: 7261 6c22 202b 2063 6f6c 6f72 5465 7874  ral" + colorText
+00022e20: 2e45 4e44 0a20 2020 2020 2020 2020 2020  .END.           
+00022e30: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00022e40: 2020 2020 2020 2073 6176 6544 6963 745b         saveDict[
+00022e50: 224d 412d 5369 676e 616c 225d 203d 2073  "MA-Signal"] = s
+00022e60: 6176 6564 5b31 5d20 2b20 224e 6575 7472  aved[1] + "Neutr
+00022e70: 616c 220a 2020 2020 2020 2020 7265 7665  al".        reve
+00022e80: 7273 6564 4461 7461 203d 2064 6174 615b  rsedData = data[
+00022e90: 3a3a 2d31 5d20 2023 2052 6576 6572 7365  ::-1]  # Reverse
+00022ea0: 2074 6865 2064 6174 6166 7261 6d65 0a20   the dataframe. 
+00022eb0: 2020 2020 2020 2065 6d61 5f32 3020 3d20         ema_20 = 
+00022ec0: 706b 7461 6c69 622e 454d 4128 7265 7665  pktalib.EMA(reve
+00022ed0: 7273 6564 4461 7461 5b22 436c 6f73 6522  rsedData["Close"
+00022ee0: 5d2c 3230 292e 7461 696c 2831 292e 696c  ],20).tail(1).il
+00022ef0: 6f63 5b30 5d0a 2020 2020 2020 2020 7677  oc[0].        vw
+00022f00: 6170 203d 2070 6b74 616c 6962 2e56 5741  ap = pktalib.VWA
+00022f10: 5028 7265 7665 7273 6564 4461 7461 5b22  P(reversedData["
+00022f20: 4869 6768 225d 2c72 6576 6572 7365 6444  High"],reversedD
+00022f30: 6174 615b 224c 6f77 225d 2c72 6576 6572  ata["Low"],rever
+00022f40: 7365 6444 6174 615b 2243 6c6f 7365 225d  sedData["Close"]
+00022f50: 2c72 6576 6572 7365 6444 6174 615b 2256  ,reversedData["V
+00022f60: 6f6c 756d 6522 5d29 2e74 6169 6c28 3129  olume"]).tail(1)
+00022f70: 2e69 6c6f 635b 305d 0a20 2020 2020 2020  .iloc[0].       
+00022f80: 2073 6d61 4465 7620 3d20 6461 7461 5b22   smaDev = data["
+00022f90: 534d 4122 5d2e 696c 6f63 5b30 5d20 2a20  SMA"].iloc[0] * 
 00022fa0: 6d61 5261 6e67 6520 2f20 3130 300a 2020  maRange / 100.  
-00022fb0: 2020 2020 2020 7677 6170 4465 7620 3d20        vwapDev = 
-00022fc0: 7677 6170 202a 206d 6152 616e 6765 202f  vwap * maRange /
-00022fd0: 2031 3030 0a20 2020 2020 2020 206f 7065   100.        ope
-00022fe0: 6e2c 2068 6967 682c 206c 6f77 2c20 636c  n, high, low, cl
-00022ff0: 6f73 652c 2073 6d61 2c20 6c6d 6120 3d20  ose, sma, lma = 
-00023000: 280a 2020 2020 2020 2020 2020 2020 6461  (.            da
-00023010: 7461 5b22 4f70 656e 225d 2e69 6c6f 635b  ta["Open"].iloc[
-00023020: 305d 2c0a 2020 2020 2020 2020 2020 2020  0],.            
-00023030: 6461 7461 5b22 4869 6768 225d 2e69 6c6f  data["High"].ilo
-00023040: 635b 305d 2c0a 2020 2020 2020 2020 2020  c[0],.          
-00023050: 2020 6461 7461 5b22 4c6f 7722 5d2e 696c    data["Low"].il
-00023060: 6f63 5b30 5d2c 0a20 2020 2020 2020 2020  oc[0],.         
-00023070: 2020 2064 6174 615b 2243 6c6f 7365 225d     data["Close"]
-00023080: 2e69 6c6f 635b 305d 2c0a 2020 2020 2020  .iloc[0],.      
-00023090: 2020 2020 2020 6461 7461 5b22 534d 4122        data["SMA"
-000230a0: 5d2e 696c 6f63 5b30 5d2c 0a20 2020 2020  ].iloc[0],.     
-000230b0: 2020 2020 2020 2064 6174 615b 224c 4d41         data["LMA
-000230c0: 225d 2e69 6c6f 635b 305d 2c0a 2020 2020  "].iloc[0],.    
-000230d0: 2020 2020 290a 2020 2020 2020 2020 6d61      ).        ma
-000230e0: 7320 3d20 5b73 6d61 2c6c 6d61 2c65 6d61  s = [sma,lma,ema
-000230f0: 5f32 302c 7677 6170 5d20 6966 206d 614c  _20,vwap] if maL
-00023100: 656e 6774 683d 3d30 2065 6c73 6520 5b73  ength==0 else [s
-00023110: 6d61 2c6c 6d61 2c65 6d61 5f32 305d 0a20  ma,lma,ema_20]. 
-00023120: 2020 2020 2020 206d 6144 6576 7320 3d20         maDevs = 
-00023130: 5b73 6d61 4465 762c 206c 6d61 4465 762c  [smaDev, lmaDev,
-00023140: 2065 6d61 4465 762c 2076 7761 7044 6576   emaDev, vwapDev
-00023150: 5d20 6966 206d 614c 656e 6774 683d 3d30  ] if maLength==0
-00023160: 2065 6c73 6520 5b73 6d61 4465 762c 206c   else [smaDev, l
-00023170: 6d61 4465 762c 2065 6d61 4465 765d 0a20  maDev, emaDev]. 
-00023180: 2020 2020 2020 206d 6154 6578 7473 203d         maTexts =
-00023190: 205b 2235 304d 4122 2c22 3230 304d 4122   ["50MA","200MA"
-000231a0: 2c22 3230 454d 4122 2c22 5657 4150 225d  ,"20EMA","VWAP"]
-000231b0: 2069 6620 6d61 4c65 6e67 7468 3d3d 3020   if maLength==0 
-000231c0: 656c 7365 205b 2235 304d 4122 2c22 3230  else ["50MA","20
-000231d0: 304d 4122 2c22 3230 454d 4122 5d0a 2020  0MA","20EMA"].  
-000231e0: 2020 2020 2020 6d61 5265 7665 7273 616c        maReversal
-000231f0: 203d 2030 0a20 2020 2020 2020 2069 6e64   = 0.        ind
-00023200: 6578 203d 2030 0a20 2020 2020 2020 2062  ex = 0.        b
-00023210: 756c 6c69 7368 4361 6e64 6c65 203d 2073  ullishCandle = s
-00023220: 656c 662e 6765 7443 616e 646c 6554 7970  elf.getCandleTyp
-00023230: 6528 6461 7461 290a 2020 2020 2020 2020  e(data).        
-00023240: 6966 2073 7472 286d 614c 656e 6774 6829  if str(maLength)
-00023250: 206e 6f74 2069 6e20 5b22 3222 2c22 3322   not in ["2","3"
-00023260: 5d3a 0a20 2020 2020 2020 2020 2020 2066  ]:.            f
-00023270: 6f72 206d 6120 696e 206d 6173 3a0a 2020  or ma in mas:.  
-00023280: 2020 2020 2020 2020 2020 2020 2020 7361                sa
-00023290: 7665 6420 3d20 7365 6c66 2e66 696e 6443  ved = self.findC
-000232a0: 7572 7265 6e74 5361 7665 6456 616c 7565  urrentSavedValue
-000232b0: 2873 6372 6565 6e44 6963 742c 7361 7665  (screenDict,save
-000232c0: 4469 6374 2c22 4d41 2d53 6967 6e61 6c22  Dict,"MA-Signal"
-000232d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000232e0: 2020 2320 5461 6b69 6e67 2053 7570 706f    # Taking Suppo
-000232f0: 7274 0a20 2020 2020 2020 2020 2020 2020  rt.             
-00023300: 2020 2069 6620 636c 6f73 6520 3e20 6d61     if close > ma
-00023310: 2061 6e64 206c 6f77 203c 3d20 286d 6120   and low <= (ma 
-00023320: 2b20 6d61 4465 7673 5b69 6e64 6578 5d29  + maDevs[index])
-00023330: 2061 6e64 2073 7472 286d 614c 656e 6774   and str(maLengt
-00023340: 6829 2069 6e20 5b22 3022 2c22 3122 5d3a  h) in ["0","1"]:
-00023350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00023360: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
-00023370: 224d 412d 5369 676e 616c 225d 203d 2028  "MA-Signal"] = (
-00023380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00023390: 2020 2020 2020 2020 2073 6176 6564 5b30           saved[0
-000233a0: 5d20 2b20 636f 6c6f 7254 6578 742e 424f  ] + colorText.BO
-000233b0: 4c44 202b 2063 6f6c 6f72 5465 7874 2e47  LD + colorText.G
-000233c0: 5245 454e 202b 2066 227b 6d61 5465 7874  REEN + f"{maText
-000233d0: 735b 696e 6465 785d 7d2d 5375 7070 6f72  s[index]}-Suppor
-000233e0: 7422 202b 2063 6f6c 6f72 5465 7874 2e45  t" + colorText.E
-000233f0: 4e44 0a20 2020 2020 2020 2020 2020 2020  ND.             
-00023400: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00023410: 2020 2020 2020 2020 2020 2020 2073 6176               sav
-00023420: 6544 6963 745b 224d 412d 5369 676e 616c  eDict["MA-Signal
-00023430: 225d 203d 2073 6176 6564 5b31 5d20 2b20  "] = saved[1] + 
-00023440: 6622 7b6d 6154 6578 7473 5b69 6e64 6578  f"{maTexts[index
-00023450: 5d7d 2d53 7570 706f 7274 220a 2020 2020  ]}-Support".    
-00023460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023470: 6d61 5265 7665 7273 616c 203d 2031 0a20  maReversal = 1. 
-00023480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023490: 2020 206d 6153 6967 6e61 6c73 2e61 7070     maSignals.app
-000234a0: 656e 6428 2231 2229 0a20 2020 2020 2020  end("1").       
-000234b0: 2020 2020 2020 2020 2023 2056 616c 6964           # Valid
-000234c0: 6174 696e 6720 5265 7369 7374 616e 6365  ating Resistance
-000234d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000234e0: 2065 6c69 6620 636c 6f73 6520 3c20 6d61   elif close < ma
-000234f0: 2061 6e64 2068 6967 6820 3e3d 2028 6d61   and high >= (ma
-00023500: 202d 206d 6144 6576 735b 696e 6465 785d   - maDevs[index]
-00023510: 2920 616e 6420 7374 7228 6d61 4c65 6e67  ) and str(maLeng
-00023520: 7468 2920 696e 205b 2230 222c 2236 225d  th) in ["0","6"]
-00023530: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00023540: 2020 2020 2020 7363 7265 656e 4469 6374        screenDict
-00023550: 5b22 4d41 2d53 6967 6e61 6c22 5d20 3d20  ["MA-Signal"] = 
-00023560: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00023570: 2020 2020 2020 2020 2020 7361 7665 645b            saved[
-00023580: 305d 202b 2063 6f6c 6f72 5465 7874 2e42  0] + colorText.B
-00023590: 4f4c 4420 2b20 636f 6c6f 7254 6578 742e  OLD + colorText.
-000235a0: 4641 494c 202b 2066 227b 6d61 5465 7874  FAIL + f"{maText
-000235b0: 735b 696e 6465 785d 7d2d 5265 7369 7374  s[index]}-Resist
-000235c0: 2220 2b20 636f 6c6f 7254 6578 742e 454e  " + colorText.EN
-000235d0: 440a 2020 2020 2020 2020 2020 2020 2020  D.              
-000235e0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000235f0: 2020 2020 2020 2020 2020 2020 7361 7665              save
-00023600: 4469 6374 5b22 4d41 2d53 6967 6e61 6c22  Dict["MA-Signal"
-00023610: 5d20 3d20 7361 7665 645b 315d 202b 2066  ] = saved[1] + f
-00023620: 227b 6d61 5465 7874 735b 696e 6465 785d  "{maTexts[index]
-00023630: 7d2d 5265 7369 7374 220a 2020 2020 2020  }-Resist".      
-00023640: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-00023650: 5265 7665 7273 616c 203d 202d 310a 2020  Reversal = -1.  
-00023660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023670: 2020 6d61 5369 676e 616c 732e 6170 7065    maSignals.appe
-00023680: 6e64 2822 3622 290a 2020 2020 2020 2020  nd("6").        
-00023690: 2020 2020 2020 2020 2320 466f 7220 6120          # For a 
-000236a0: 4275 6c6c 6973 6820 4361 6e64 6c65 0a20  Bullish Candle. 
-000236b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000236c0: 6620 6275 6c6c 6973 6843 616e 646c 653a  f bullishCandle:
-000236d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000236e0: 2020 2020 2023 2043 726f 7373 696e 6720       # Crossing 
-000236f0: 7570 0a20 2020 2020 2020 2020 2020 2020  up.             
-00023700: 2020 2020 2020 2069 6620 6f70 656e 203c         if open <
-00023710: 206d 6120 616e 6420 636c 6f73 6520 3e20   ma and close > 
-00023720: 6d61 2061 6e64 2073 7472 286d 614c 656e  ma and str(maLen
-00023730: 6774 6829 2069 6e20 5b22 3022 2c22 3522  gth) in ["0","5"
-00023740: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
-00023750: 2020 2020 2020 2020 2020 2073 6372 6565             scree
-00023760: 6e44 6963 745b 224d 412d 5369 676e 616c  nDict["MA-Signal
-00023770: 225d 203d 2028 0a20 2020 2020 2020 2020  "] = (.         
-00023780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023790: 2020 2073 6176 6564 5b30 5d20 2b20 636f     saved[0] + co
-000237a0: 6c6f 7254 6578 742e 424f 4c44 202b 2063  lorText.BOLD + c
-000237b0: 6f6c 6f72 5465 7874 2e47 5245 454e 202b  olorText.GREEN +
-000237c0: 2066 2242 756c 6c43 726f 7373 2d7b 6d61   f"BullCross-{ma
-000237d0: 5465 7874 735b 696e 6465 785d 7d22 202b  Texts[index]}" +
-000237e0: 2063 6f6c 6f72 5465 7874 2e45 4e44 0a20   colorText.END. 
-000237f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023800: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00023810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023820: 2073 6176 6544 6963 745b 224d 412d 5369   saveDict["MA-Si
-00023830: 676e 616c 225d 203d 2073 6176 6564 5b31  gnal"] = saved[1
-00023840: 5d20 2b20 6622 4275 6c6c 4372 6f73 732d  ] + f"BullCross-
-00023850: 7b6d 6154 6578 7473 5b69 6e64 6578 5d7d  {maTexts[index]}
-00023860: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00023870: 2020 2020 2020 2020 2020 6d61 5265 7665            maReve
-00023880: 7273 616c 203d 2031 0a20 2020 2020 2020  rsal = 1.       
-00023890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000238a0: 206d 6153 6967 6e61 6c73 2e61 7070 656e   maSignals.appen
-000238b0: 6428 2235 2229 0a20 2020 2020 2020 2020  d("5").         
-000238c0: 2020 2020 2020 2023 2046 6f72 2061 2042         # For a B
-000238d0: 6561 7269 7368 2043 616e 646c 650a 2020  earish Candle.  
-000238e0: 2020 2020 2020 2020 2020 2020 2020 656c                el
-000238f0: 6966 206e 6f74 2062 756c 6c69 7368 4361  if not bullishCa
-00023900: 6e64 6c65 3a0a 2020 2020 2020 2020 2020  ndle:.          
-00023910: 2020 2020 2020 2020 2020 2320 4372 6f73            # Cros
-00023920: 7369 6e67 2064 6f77 6e0a 2020 2020 2020  sing down.      
-00023930: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00023940: 206f 7065 6e20 3e20 736d 6120 616e 6420   open > sma and 
-00023950: 636c 6f73 6520 3c20 736d 6120 616e 6420  close < sma and 
-00023960: 7374 7228 6d61 4c65 6e67 7468 2920 696e  str(maLength) in
-00023970: 205b 2230 222c 2234 225d 3a0a 2020 2020   ["0","4"]:.    
-00023980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023990: 2020 2020 7363 7265 656e 4469 6374 5b22      screenDict["
-000239a0: 4d41 2d53 6967 6e61 6c22 5d20 3d20 280a  MA-Signal"] = (.
-000239b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000239c0: 2020 2020 2020 2020 2020 2020 7361 7665              save
-000239d0: 645b 305d 202b 2063 6f6c 6f72 5465 7874  d[0] + colorText
-000239e0: 2e42 4f4c 4420 2b20 636f 6c6f 7254 6578  .BOLD + colorTex
-000239f0: 742e 4641 494c 202b 2066 2242 6561 7243  t.FAIL + f"BearC
-00023a00: 726f 7373 2d7b 6d61 5465 7874 735b 696e  ross-{maTexts[in
-00023a10: 6465 785d 7d22 202b 2063 6f6c 6f72 5465  dex]}" + colorTe
-00023a20: 7874 2e45 4e44 0a20 2020 2020 2020 2020  xt.END.         
-00023a30: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00023a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00023a50: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
-00023a60: 745b 224d 412d 5369 676e 616c 225d 203d  t["MA-Signal"] =
-00023a70: 2073 6176 6564 5b31 5d20 2b20 6622 4265   saved[1] + f"Be
-00023a80: 6172 4372 6f73 732d 7b6d 6154 6578 7473  arCross-{maTexts
-00023a90: 5b69 6e64 6578 5d7d 220a 2020 2020 2020  [index]}".      
+00022fb0: 2020 2020 2020 6c6d 6144 6576 203d 2064        lmaDev = d
+00022fc0: 6174 615b 224c 4d41 225d 2e69 6c6f 635b  ata["LMA"].iloc[
+00022fd0: 305d 202a 206d 6152 616e 6765 202f 2031  0] * maRange / 1
+00022fe0: 3030 0a20 2020 2020 2020 2065 6d61 4465  00.        emaDe
+00022ff0: 7620 3d20 656d 615f 3230 202a 206d 6152  v = ema_20 * maR
+00023000: 616e 6765 202f 2031 3030 0a20 2020 2020  ange / 100.     
+00023010: 2020 2076 7761 7044 6576 203d 2076 7761     vwapDev = vwa
+00023020: 7020 2a20 6d61 5261 6e67 6520 2f20 3130  p * maRange / 10
+00023030: 300a 2020 2020 2020 2020 6f70 656e 2c20  0.        open, 
+00023040: 6869 6768 2c20 6c6f 772c 2063 6c6f 7365  high, low, close
+00023050: 2c20 736d 612c 206c 6d61 203d 2028 0a20  , sma, lma = (. 
+00023060: 2020 2020 2020 2020 2020 2064 6174 615b             data[
+00023070: 224f 7065 6e22 5d2e 696c 6f63 5b30 5d2c  "Open"].iloc[0],
+00023080: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+00023090: 615b 2248 6967 6822 5d2e 696c 6f63 5b30  a["High"].iloc[0
+000230a0: 5d2c 0a20 2020 2020 2020 2020 2020 2064  ],.            d
+000230b0: 6174 615b 224c 6f77 225d 2e69 6c6f 635b  ata["Low"].iloc[
+000230c0: 305d 2c0a 2020 2020 2020 2020 2020 2020  0],.            
+000230d0: 6461 7461 5b22 436c 6f73 6522 5d2e 696c  data["Close"].il
+000230e0: 6f63 5b30 5d2c 0a20 2020 2020 2020 2020  oc[0],.         
+000230f0: 2020 2064 6174 615b 2253 4d41 225d 2e69     data["SMA"].i
+00023100: 6c6f 635b 305d 2c0a 2020 2020 2020 2020  loc[0],.        
+00023110: 2020 2020 6461 7461 5b22 4c4d 4122 5d2e      data["LMA"].
+00023120: 696c 6f63 5b30 5d2c 0a20 2020 2020 2020  iloc[0],.       
+00023130: 2029 0a20 2020 2020 2020 206d 6173 203d   ).        mas =
+00023140: 205b 736d 612c 6c6d 612c 656d 615f 3230   [sma,lma,ema_20
+00023150: 2c76 7761 705d 2069 6620 6d61 4c65 6e67  ,vwap] if maLeng
+00023160: 7468 3d3d 3020 656c 7365 205b 736d 612c  th==0 else [sma,
+00023170: 6c6d 612c 656d 615f 3230 5d0a 2020 2020  lma,ema_20].    
+00023180: 2020 2020 6d61 4465 7673 203d 205b 736d      maDevs = [sm
+00023190: 6144 6576 2c20 6c6d 6144 6576 2c20 656d  aDev, lmaDev, em
+000231a0: 6144 6576 2c20 7677 6170 4465 765d 2069  aDev, vwapDev] i
+000231b0: 6620 6d61 4c65 6e67 7468 3d3d 3020 656c  f maLength==0 el
+000231c0: 7365 205b 736d 6144 6576 2c20 6c6d 6144  se [smaDev, lmaD
+000231d0: 6576 2c20 656d 6144 6576 5d0a 2020 2020  ev, emaDev].    
+000231e0: 2020 2020 6d61 5465 7874 7320 3d20 5b22      maTexts = ["
+000231f0: 3530 4d41 222c 2232 3030 4d41 222c 2232  50MA","200MA","2
+00023200: 3045 4d41 222c 2256 5741 5022 5d20 6966  0EMA","VWAP"] if
+00023210: 206d 614c 656e 6774 683d 3d30 2065 6c73   maLength==0 els
+00023220: 6520 5b22 3530 4d41 222c 2232 3030 4d41  e ["50MA","200MA
+00023230: 222c 2232 3045 4d41 225d 0a20 2020 2020  ","20EMA"].     
+00023240: 2020 206d 6152 6576 6572 7361 6c20 3d20     maReversal = 
+00023250: 300a 2020 2020 2020 2020 696e 6465 7820  0.        index 
+00023260: 3d20 300a 2020 2020 2020 2020 6275 6c6c  = 0.        bull
+00023270: 6973 6843 616e 646c 6520 3d20 7365 6c66  ishCandle = self
+00023280: 2e67 6574 4361 6e64 6c65 5479 7065 2864  .getCandleType(d
+00023290: 6174 6129 0a20 2020 2020 2020 2069 6620  ata).        if 
+000232a0: 7374 7228 6d61 4c65 6e67 7468 2920 6e6f  str(maLength) no
+000232b0: 7420 696e 205b 2232 222c 2233 225d 3a0a  t in ["2","3"]:.
+000232c0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000232d0: 6d61 2069 6e20 6d61 733a 0a20 2020 2020  ma in mas:.     
+000232e0: 2020 2020 2020 2020 2020 2073 6176 6564             saved
+000232f0: 203d 2073 656c 662e 6669 6e64 4375 7272   = self.findCurr
+00023300: 656e 7453 6176 6564 5661 6c75 6528 7363  entSavedValue(sc
+00023310: 7265 656e 4469 6374 2c73 6176 6544 6963  reenDict,saveDic
+00023320: 742c 224d 412d 5369 676e 616c 2229 0a20  t,"MA-Signal"). 
+00023330: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00023340: 2054 616b 696e 6720 5375 7070 6f72 740a   Taking Support.
+00023350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023360: 6966 2063 6c6f 7365 203e 206d 6120 616e  if close > ma an
+00023370: 6420 6c6f 7720 3c3d 2028 6d61 202b 206d  d low <= (ma + m
+00023380: 6144 6576 735b 696e 6465 785d 2920 616e  aDevs[index]) an
+00023390: 6420 7374 7228 6d61 4c65 6e67 7468 2920  d str(maLength) 
+000233a0: 696e 205b 2230 222c 2231 225d 3a0a 2020  in ["0","1"]:.  
+000233b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000233c0: 2020 7363 7265 656e 4469 6374 5b22 4d41    screenDict["MA
+000233d0: 2d53 6967 6e61 6c22 5d20 3d20 280a 2020  -Signal"] = (.  
+000233e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000233f0: 2020 2020 2020 7361 7665 645b 305d 202b        saved[0] +
+00023400: 2063 6f6c 6f72 5465 7874 2e42 4f4c 4420   colorText.BOLD 
+00023410: 2b20 636f 6c6f 7254 6578 742e 4752 4545  + colorText.GREE
+00023420: 4e20 2b20 6622 7b6d 6154 6578 7473 5b69  N + f"{maTexts[i
+00023430: 6e64 6578 5d7d 2d53 7570 706f 7274 2220  ndex]}-Support" 
+00023440: 2b20 636f 6c6f 7254 6578 742e 454e 440a  + colorText.END.
+00023450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023460: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00023470: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
+00023480: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d20  ct["MA-Signal"] 
+00023490: 3d20 7361 7665 645b 315d 202b 2066 227b  = saved[1] + f"{
+000234a0: 6d61 5465 7874 735b 696e 6465 785d 7d2d  maTexts[index]}-
+000234b0: 5375 7070 6f72 7422 0a20 2020 2020 2020  Support".       
+000234c0: 2020 2020 2020 2020 2020 2020 206d 6152               maR
+000234d0: 6576 6572 7361 6c20 3d20 310a 2020 2020  eversal = 1.    
+000234e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000234f0: 6d61 5369 676e 616c 732e 6170 7065 6e64  maSignals.append
+00023500: 2822 3122 290a 2020 2020 2020 2020 2020  ("1").          
+00023510: 2020 2020 2020 2320 5661 6c69 6461 7469        # Validati
+00023520: 6e67 2052 6573 6973 7461 6e63 650a 2020  ng Resistance.  
+00023530: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00023540: 6966 2063 6c6f 7365 203c 206d 6120 616e  if close < ma an
+00023550: 6420 6869 6768 203e 3d20 286d 6120 2d20  d high >= (ma - 
+00023560: 6d61 4465 7673 5b69 6e64 6578 5d29 2061  maDevs[index]) a
+00023570: 6e64 2073 7472 286d 614c 656e 6774 6829  nd str(maLength)
+00023580: 2069 6e20 5b22 3022 2c22 3622 5d3a 0a20   in ["0","6"]:. 
+00023590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000235a0: 2020 2073 6372 6565 6e44 6963 745b 224d     screenDict["M
+000235b0: 412d 5369 676e 616c 225d 203d 2028 0a20  A-Signal"] = (. 
+000235c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000235d0: 2020 2020 2020 2073 6176 6564 5b30 5d20         saved[0] 
+000235e0: 2b20 636f 6c6f 7254 6578 742e 424f 4c44  + colorText.BOLD
+000235f0: 202b 2063 6f6c 6f72 5465 7874 2e46 4149   + colorText.FAI
+00023600: 4c20 2b20 6622 7b6d 6154 6578 7473 5b69  L + f"{maTexts[i
+00023610: 6e64 6578 5d7d 2d52 6573 6973 7422 202b  ndex]}-Resist" +
+00023620: 2063 6f6c 6f72 5465 7874 2e45 4e44 0a20   colorText.END. 
+00023630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023640: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00023650: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
+00023660: 745b 224d 412d 5369 676e 616c 225d 203d  t["MA-Signal"] =
+00023670: 2073 6176 6564 5b31 5d20 2b20 6622 7b6d   saved[1] + f"{m
+00023680: 6154 6578 7473 5b69 6e64 6578 5d7d 2d52  aTexts[index]}-R
+00023690: 6573 6973 7422 0a20 2020 2020 2020 2020  esist".         
+000236a0: 2020 2020 2020 2020 2020 206d 6152 6576             maRev
+000236b0: 6572 7361 6c20 3d20 2d31 0a20 2020 2020  ersal = -1.     
+000236c0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+000236d0: 6153 6967 6e61 6c73 2e61 7070 656e 6428  aSignals.append(
+000236e0: 2236 2229 0a20 2020 2020 2020 2020 2020  "6").           
+000236f0: 2020 2020 2023 2046 6f72 2061 2042 756c       # For a Bul
+00023700: 6c69 7368 2043 616e 646c 650a 2020 2020  lish Candle.    
+00023710: 2020 2020 2020 2020 2020 2020 6966 2062              if b
+00023720: 756c 6c69 7368 4361 6e64 6c65 3a0a 2020  ullishCandle:.  
+00023730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023740: 2020 2320 4372 6f73 7369 6e67 2075 700a    # Crossing up.
+00023750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023760: 2020 2020 6966 206f 7065 6e20 3c20 6d61      if open < ma
+00023770: 2061 6e64 2063 6c6f 7365 203e 206d 6120   and close > ma 
+00023780: 616e 6420 7374 7228 6d61 4c65 6e67 7468  and str(maLength
+00023790: 2920 696e 205b 2230 222c 2235 225d 3a0a  ) in ["0","5"]:.
+000237a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000237b0: 2020 2020 2020 2020 7363 7265 656e 4469          screenDi
+000237c0: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d20  ct["MA-Signal"] 
+000237d0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+000237e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000237f0: 7361 7665 645b 305d 202b 2063 6f6c 6f72  saved[0] + color
+00023800: 5465 7874 2e42 4f4c 4420 2b20 636f 6c6f  Text.BOLD + colo
+00023810: 7254 6578 742e 4752 4545 4e20 2b20 6622  rText.GREEN + f"
+00023820: 4275 6c6c 4372 6f73 732d 7b6d 6154 6578  BullCross-{maTex
+00023830: 7473 5b69 6e64 6578 5d7d 2220 2b20 636f  ts[index]}" + co
+00023840: 6c6f 7254 6578 742e 454e 440a 2020 2020  lorText.END.    
+00023850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023860: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00023870: 2020 2020 2020 2020 2020 2020 2020 7361                sa
+00023880: 7665 4469 6374 5b22 4d41 2d53 6967 6e61  veDict["MA-Signa
+00023890: 6c22 5d20 3d20 7361 7665 645b 315d 202b  l"] = saved[1] +
+000238a0: 2066 2242 756c 6c43 726f 7373 2d7b 6d61   f"BullCross-{ma
+000238b0: 5465 7874 735b 696e 6465 785d 7d22 0a20  Texts[index]}". 
+000238c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000238d0: 2020 2020 2020 206d 6152 6576 6572 7361         maReversa
+000238e0: 6c20 3d20 310a 2020 2020 2020 2020 2020  l = 1.          
+000238f0: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
+00023900: 5369 676e 616c 732e 6170 7065 6e64 2822  Signals.append("
+00023910: 3522 290a 2020 2020 2020 2020 2020 2020  5").            
+00023920: 2020 2020 2320 466f 7220 6120 4265 6172      # For a Bear
+00023930: 6973 6820 4361 6e64 6c65 0a20 2020 2020  ish Candle.     
+00023940: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00023950: 6e6f 7420 6275 6c6c 6973 6843 616e 646c  not bullishCandl
+00023960: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00023970: 2020 2020 2020 2023 2043 726f 7373 696e         # Crossin
+00023980: 6720 646f 776e 0a20 2020 2020 2020 2020  g down.         
+00023990: 2020 2020 2020 2020 2020 2069 6620 6f70             if op
+000239a0: 656e 203e 2073 6d61 2061 6e64 2063 6c6f  en > sma and clo
+000239b0: 7365 203c 2073 6d61 2061 6e64 2073 7472  se < sma and str
+000239c0: 286d 614c 656e 6774 6829 2069 6e20 5b22  (maLength) in ["
+000239d0: 3022 2c22 3422 5d3a 0a20 2020 2020 2020  0","4"]:.       
+000239e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000239f0: 2073 6372 6565 6e44 6963 745b 224d 412d   screenDict["MA-
+00023a00: 5369 676e 616c 225d 203d 2028 0a20 2020  Signal"] = (.   
+00023a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023a20: 2020 2020 2020 2020 2073 6176 6564 5b30           saved[0
+00023a30: 5d20 2b20 636f 6c6f 7254 6578 742e 424f  ] + colorText.BO
+00023a40: 4c44 202b 2063 6f6c 6f72 5465 7874 2e46  LD + colorText.F
+00023a50: 4149 4c20 2b20 6622 4265 6172 4372 6f73  AIL + f"BearCros
+00023a60: 732d 7b6d 6154 6578 7473 5b69 6e64 6578  s-{maTexts[index
+00023a70: 5d7d 2220 2b20 636f 6c6f 7254 6578 742e  ]}" + colorText.
+00023a80: 454e 440a 2020 2020 2020 2020 2020 2020  END.            
+00023a90: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
 00023aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023ab0: 2020 6d61 5265 7665 7273 616c 203d 202d    maReversal = -
-00023ac0: 310a 2020 2020 2020 2020 2020 2020 2020  1.              
-00023ad0: 2020 2020 2020 2020 2020 6d61 5369 676e            maSign
-00023ae0: 616c 732e 6170 7065 6e64 2822 3422 290a  als.append("4").
-00023af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023b00: 696e 6465 7820 2b3d 2031 0a20 2020 2020  index += 1.     
-00023b10: 2020 2072 6574 7572 6e56 616c 7565 203d     returnValue =
-00023b20: 206d 6152 6576 6572 7361 6c0a 2020 2020   maReversal.    
-00023b30: 2020 2020 6966 206d 614c 656e 6774 6820      if maLength 
-00023b40: 213d 2030 3a0a 2020 2020 2020 2020 2020  != 0:.          
-00023b50: 2020 7265 7475 726e 5661 6c75 6520 3d20    returnValue = 
-00023b60: 7374 7228 6d61 4c65 6e67 7468 2920 696e  str(maLength) in
-00023b70: 206d 6153 6967 6e61 6c73 0a20 2020 2020   maSignals.     
-00023b80: 2020 2072 6574 7572 6e20 7265 7475 726e     return return
-00023b90: 5661 6c75 650a 0a20 2020 2023 2046 696e  Value..    # Fin
-00023ba0: 6420 4e52 7820 7261 6e67 6520 666f 7220  d NRx range for 
-00023bb0: 5265 7665 7273 616c 0a20 2020 2064 6566  Reversal.    def
-00023bc0: 2076 616c 6964 6174 654e 6172 726f 7752   validateNarrowR
-00023bd0: 616e 6765 2873 656c 662c 2064 662c 2073  ange(self, df, s
-00023be0: 6372 6565 6e44 6963 742c 2073 6176 6544  creenDict, saveD
-00023bf0: 6963 742c 206e 723d 3429 3a0a 2020 2020  ict, nr=4):.    
-00023c00: 2020 2020 6966 2064 6620 6973 204e 6f6e      if df is Non
-00023c10: 6520 6f72 206c 656e 2864 6629 203d 3d20  e or len(df) == 
-00023c20: 303a 0a20 2020 2020 2020 2020 2020 2072  0:.            r
-00023c30: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
-00023c40: 2020 2020 6461 7461 203d 2064 662e 636f      data = df.co
-00023c50: 7079 2829 0a20 2020 2020 2020 2073 6176  py().        sav
-00023c60: 6564 203d 2073 656c 662e 6669 6e64 4375  ed = self.findCu
-00023c70: 7272 656e 7453 6176 6564 5661 6c75 6528  rrentSavedValue(
-00023c80: 7363 7265 656e 4469 6374 2c20 7361 7665  screenDict, save
-00023c90: 4469 6374 2c20 2250 6174 7465 726e 2229  Dict, "Pattern")
-00023ca0: 0a20 2020 2020 2020 2069 6620 504b 4461  .        if PKDa
-00023cb0: 7465 5574 696c 6974 6965 732e 6973 5472  teUtilities.isTr
-00023cc0: 6164 696e 6754 696d 6528 293a 0a20 2020  adingTime():.   
-00023cd0: 2020 2020 2020 2020 2072 616e 6765 4461           rangeDa
-00023ce0: 7461 203d 2064 6174 612e 6865 6164 286e  ta = data.head(n
-00023cf0: 7220 2b20 3129 5b31 3a5d 0a20 2020 2020  r + 1)[1:].     
-00023d00: 2020 2020 2020 206e 6f77 5f63 616e 646c         now_candl
-00023d10: 6520 3d20 6461 7461 2e68 6561 6428 3129  e = data.head(1)
-00023d20: 0a20 2020 2020 2020 2020 2020 2072 616e  .            ran
-00023d30: 6765 4461 7461 5b22 5261 6e67 6522 5d20  geData["Range"] 
-00023d40: 3d20 6162 7328 7261 6e67 6544 6174 615b  = abs(rangeData[
-00023d50: 2243 6c6f 7365 225d 202d 2072 616e 6765  "Close"] - range
-00023d60: 4461 7461 5b22 4f70 656e 225d 290a 2020  Data["Open"]).  
-00023d70: 2020 2020 2020 2020 2020 7265 6365 6e74            recent
-00023d80: 203d 2072 616e 6765 4461 7461 2e68 6561   = rangeData.hea
-00023d90: 6428 3129 0a20 2020 2020 2020 2020 2020  d(1).           
-00023da0: 2069 6620 280a 2020 2020 2020 2020 2020   if (.          
-00023db0: 2020 2020 2020 6c65 6e28 7265 6365 6e74        len(recent
-00023dc0: 2920 3d3d 2031 0a20 2020 2020 2020 2020  ) == 1.         
-00023dd0: 2020 2020 2020 2061 6e64 2072 6563 656e         and recen
-00023de0: 745b 2252 616e 6765 225d 2e69 6c6f 635b  t["Range"].iloc[
-00023df0: 305d 203d 3d20 7261 6e67 6544 6174 612e  0] == rangeData.
-00023e00: 6465 7363 7269 6265 2829 5b22 5261 6e67  describe()["Rang
-00023e10: 6522 5d5b 226d 696e 225d 0a20 2020 2020  e"]["min"].     
-00023e20: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
-00023e30: 2020 2020 2020 2020 2020 6966 2028 0a20            if (. 
-00023e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023e50: 2020 2073 656c 662e 6765 7443 616e 646c     self.getCandl
-00023e60: 6554 7970 6528 7265 6365 6e74 290a 2020  eType(recent).  
-00023e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023e80: 2020 616e 6420 6e6f 775f 6361 6e64 6c65    and now_candle
-00023e90: 5b22 436c 6f73 6522 5d2e 696c 6f63 5b30  ["Close"].iloc[0
-00023ea0: 5d20 3e3d 2072 6563 656e 745b 2243 6c6f  ] >= recent["Clo
-00023eb0: 7365 225d 2e69 6c6f 635b 305d 0a20 2020  se"].iloc[0].   
-00023ec0: 2020 2020 2020 2020 2020 2020 2029 3a0a               ):.
-00023ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023ee0: 2020 2020 7363 7265 656e 4469 6374 5b22      screenDict["
-00023ef0: 5061 7474 6572 6e22 5d20 3d20 280a 2020  Pattern"] = (.  
-00023f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023f10: 2020 2020 2020 7361 7665 645b 305d 202b        saved[0] +
-00023f20: 2063 6f6c 6f72 5465 7874 2e42 4f4c 4420   colorText.BOLD 
-00023f30: 2b20 636f 6c6f 7254 6578 742e 4752 4545  + colorText.GREE
-00023f40: 4e20 2b20 6622 4275 792d 4e52 7b6e 727d  N + f"Buy-NR{nr}
-00023f50: 2220 2b20 636f 6c6f 7254 6578 742e 454e  " + colorText.EN
-00023f60: 440a 2020 2020 2020 2020 2020 2020 2020  D.              
-00023f70: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00023f80: 2020 2020 2020 2020 2020 2020 7361 7665              save
-00023f90: 4469 6374 5b22 5061 7474 6572 6e22 5d20  Dict["Pattern"] 
-00023fa0: 3d20 7361 7665 645b 315d 202b 2066 2242  = saved[1] + f"B
-00023fb0: 7579 2d4e 527b 6e72 7d22 0a20 2020 2020  uy-NR{nr}".     
-00023fc0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00023fd0: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
-00023fe0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00023ff0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00024000: 2020 2020 2020 6e6f 7420 7365 6c66 2e67        not self.g
-00024010: 6574 4361 6e64 6c65 5479 7065 2872 6563  etCandleType(rec
-00024020: 656e 7429 0a20 2020 2020 2020 2020 2020  ent).           
-00024030: 2020 2020 2020 2020 2061 6e64 206e 6f77           and now
-00024040: 5f63 616e 646c 655b 2243 6c6f 7365 225d  _candle["Close"]
-00024050: 2e69 6c6f 635b 305d 203c 3d20 7265 6365  .iloc[0] <= rece
-00024060: 6e74 5b22 436c 6f73 6522 5d2e 696c 6f63  nt["Close"].iloc
-00024070: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
-00024080: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
-00024090: 2020 2020 2020 2020 2020 2073 6372 6565             scree
-000240a0: 6e44 6963 745b 2250 6174 7465 726e 225d  nDict["Pattern"]
-000240b0: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
-000240c0: 2020 2020 2020 2020 2020 2020 2073 6176               sav
-000240d0: 6564 5b30 5d20 2b20 636f 6c6f 7254 6578  ed[0] + colorTex
-000240e0: 742e 424f 4c44 202b 2063 6f6c 6f72 5465  t.BOLD + colorTe
-000240f0: 7874 2e46 4149 4c20 2b20 6622 5365 6c6c  xt.FAIL + f"Sell
-00024100: 2d4e 527b 6e72 7d22 202b 2063 6f6c 6f72  -NR{nr}" + color
-00024110: 5465 7874 2e45 4e44 0a20 2020 2020 2020  Text.END.       
-00024120: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00024130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024140: 2020 2073 6176 6544 6963 745b 2250 6174     saveDict["Pat
-00024150: 7465 726e 225d 203d 2073 6176 6564 5b31  tern"] = saved[1
-00024160: 5d20 2b20 6622 5365 6c6c 2d4e 527b 6e72  ] + f"Sell-NR{nr
-00024170: 7d22 0a20 2020 2020 2020 2020 2020 2020  }".             
-00024180: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-00024190: 7565 0a20 2020 2020 2020 2020 2020 2072  ue.            r
-000241a0: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
-000241b0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-000241c0: 2020 2020 2020 7261 6e67 6544 6174 6120        rangeData 
-000241d0: 3d20 6461 7461 2e68 6561 6428 6e72 290a  = data.head(nr).
-000241e0: 2020 2020 2020 2020 2020 2020 7261 6e67              rang
-000241f0: 6544 6174 612e 6c6f 635b 3a2c 2752 616e  eData.loc[:,'Ran
-00024200: 6765 275d 203d 2061 6273 2872 616e 6765  ge'] = abs(range
-00024210: 4461 7461 5b22 436c 6f73 6522 5d20 2d20  Data["Close"] - 
-00024220: 7261 6e67 6544 6174 615b 224f 7065 6e22  rangeData["Open"
-00024230: 5d29 0a20 2020 2020 2020 2020 2020 2072  ]).            r
-00024240: 6563 656e 7420 3d20 7261 6e67 6544 6174  ecent = rangeDat
-00024250: 612e 6865 6164 2831 290a 2020 2020 2020  a.head(1).      
-00024260: 2020 2020 2020 6966 2072 6563 656e 745b        if recent[
-00024270: 2252 616e 6765 225d 2e69 6c6f 635b 305d  "Range"].iloc[0]
-00024280: 203d 3d20 7261 6e67 6544 6174 612e 6465   == rangeData.de
-00024290: 7363 7269 6265 2829 5b22 5261 6e67 6522  scribe()["Range"
-000242a0: 5d5b 226d 696e 225d 3a0a 2020 2020 2020  ]["min"]:.      
-000242b0: 2020 2020 2020 2020 2020 7363 7265 656e            screen
-000242c0: 4469 6374 5b22 5061 7474 6572 6e22 5d20  Dict["Pattern"] 
-000242d0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-000242e0: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
-000242f0: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
-00024300: 4420 2b20 636f 6c6f 7254 6578 742e 4752  D + colorText.GR
-00024310: 4545 4e20 2b20 6622 4e52 7b6e 727d 2220  EEN + f"NR{nr}" 
-00024320: 2b20 636f 6c6f 7254 6578 742e 454e 440a  + colorText.END.
-00024330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024340: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00024350: 2020 7361 7665 4469 6374 5b22 5061 7474    saveDict["Patt
-00024360: 6572 6e22 5d20 3d20 7361 7665 645b 315d  ern"] = saved[1]
-00024370: 202b 2066 224e 527b 6e72 7d22 0a20 2020   + f"NR{nr}".   
-00024380: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00024390: 7572 6e20 5472 7565 0a20 2020 2020 2020  urn True.       
-000243a0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-000243b0: 650a 0a20 2020 2023 2046 696e 6420 6966  e..    # Find if
-000243c0: 2073 746f 636b 2069 7320 6e65 776c 7920   stock is newly 
-000243d0: 6c69 7374 6564 0a20 2020 2064 6566 2076  listed.    def v
-000243e0: 616c 6964 6174 654e 6577 6c79 4c69 7374  alidateNewlyList
-000243f0: 6564 2873 656c 662c 2064 662c 2064 6179  ed(self, df, day
-00024400: 7354 6f4c 6f6f 6b62 6163 6b29 3a0a 2020  sToLookback):.  
-00024410: 2020 2020 2020 6966 2064 6620 6973 204e        if df is N
-00024420: 6f6e 6520 6f72 206c 656e 2864 6629 203d  one or len(df) =
-00024430: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
-00024440: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
-00024450: 2020 2020 2020 6461 7461 203d 2064 662e        data = df.
-00024460: 636f 7079 2829 0a20 2020 2020 2020 2064  copy().        d
-00024470: 6179 7354 6f4c 6f6f 6b62 6163 6b20 3d20  aysToLookback = 
-00024480: 696e 7428 6461 7973 546f 4c6f 6f6b 6261  int(daysToLookba
-00024490: 636b 5b3a 2d31 5d29 0a20 2020 2020 2020  ck[:-1]).       
-000244a0: 2072 6563 656e 7420 3d20 6461 7461 2e68   recent = data.h
-000244b0: 6561 6428 3129 0a20 2020 2020 2020 2069  ead(1).        i
-000244c0: 6620 6c65 6e28 7265 6365 6e74 2920 3c20  f len(recent) < 
-000244d0: 313a 0a20 2020 2020 2020 2020 2020 2072  1:.            r
-000244e0: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
-000244f0: 2020 2020 6966 206c 656e 2864 6174 6129      if len(data)
-00024500: 203c 2064 6179 7354 6f4c 6f6f 6b62 6163   < daysToLookbac
-00024510: 6b20 616e 6420 280a 2020 2020 2020 2020  k and (.        
-00024520: 2020 2020 7265 6365 6e74 5b22 436c 6f73      recent["Clos
-00024530: 6522 5d2e 696c 6f63 5b30 5d20 213d 206e  e"].iloc[0] != n
-00024540: 702e 6e61 6e20 616e 6420 7265 6365 6e74  p.nan and recent
-00024550: 5b22 436c 6f73 6522 5d2e 696c 6f63 5b30  ["Close"].iloc[0
-00024560: 5d20 3e20 300a 2020 2020 2020 2020 293a  ] > 0.        ):
-00024570: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00024580: 7572 6e20 5472 7565 0a20 2020 2020 2020  urn True.       
-00024590: 2072 6574 7572 6e20 4661 6c73 650a 0a20   return False.. 
-000245a0: 2020 2023 2056 616c 6964 6174 6520 6966     # Validate if
-000245b0: 2074 6865 2073 746f 636b 2070 7269 6365   the stock price
-000245c0: 7320 6172 6520 6174 206c 6561 7374 2072  s are at least r
-000245d0: 6973 696e 6720 6279 2032 2520 666f 7220  ising by 2% for 
-000245e0: 7468 6520 6c61 7374 2033 2073 6573 7369  the last 3 sessi
-000245f0: 6f6e 730a 2020 2020 6465 6620 7661 6c69  ons.    def vali
-00024600: 6461 7465 5072 6963 6552 6973 696e 6742  datePriceRisingB
-00024610: 7941 744c 6561 7374 3250 6572 6365 6e74  yAtLeast2Percent
-00024620: 2873 656c 662c 2064 662c 2073 6372 6565  (self, df, scree
-00024630: 6e44 6963 742c 2073 6176 6544 6963 7429  nDict, saveDict)
-00024640: 3a0a 2020 2020 2020 2020 6966 2064 6620  :.        if df 
-00024650: 6973 204e 6f6e 6520 6f72 206c 656e 2864  is None or len(d
-00024660: 6629 203d 3d20 303a 0a20 2020 2020 2020  f) == 0:.       
-00024670: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-00024680: 650a 2020 2020 2020 2020 6461 7461 203d  e.        data =
-00024690: 2064 662e 636f 7079 2829 0a20 2020 2020   df.copy().     
-000246a0: 2020 2064 6174 6120 3d20 6461 7461 2e66     data = data.f
-000246b0: 696c 6c6e 6128 3029 0a20 2020 2020 2020  illna(0).       
-000246c0: 2064 6174 6120 3d20 6461 7461 2e72 6570   data = data.rep
-000246d0: 6c61 6365 285b 6e70 2e69 6e66 2c20 2d6e  lace([np.inf, -n
-000246e0: 702e 696e 665d 2c20 3029 0a20 2020 2020  p.inf], 0).     
-000246f0: 2020 2064 6174 6120 3d20 6461 7461 2e68     data = data.h
-00024700: 6561 6428 3429 0a20 2020 2020 2020 2069  ead(4).        i
-00024710: 6620 6c65 6e28 6461 7461 2920 3c20 343a  f len(data) < 4:
-00024720: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00024730: 7572 6e20 4661 6c73 650a 2020 2020 2020  urn False.      
-00024740: 2020 6461 7930 203d 2064 6174 612e 696c    day0 = data.il
-00024750: 6f63 5b30 5d5b 2243 6c6f 7365 225d 2e69  oc[0]["Close"].i
-00024760: 7465 6d28 290a 2020 2020 2020 2020 6461  tem().        da
-00024770: 794d 696e 7573 3120 3d20 6461 7461 2e69  yMinus1 = data.i
-00024780: 6c6f 635b 315d 5b22 436c 6f73 6522 5d2e  loc[1]["Close"].
-00024790: 6974 656d 2829 0a20 2020 2020 2020 2064  item().        d
-000247a0: 6179 4d69 6e75 7332 203d 2064 6174 612e  ayMinus2 = data.
-000247b0: 696c 6f63 5b32 5d5b 2243 6c6f 7365 225d  iloc[2]["Close"]
-000247c0: 2e69 7465 6d28 290a 2020 2020 2020 2020  .item().        
-000247d0: 6461 794d 696e 7573 3320 3d20 6461 7461  dayMinus3 = data
-000247e0: 2e69 6c6f 635b 335d 5b22 436c 6f73 6522  .iloc[3]["Close"
-000247f0: 5d2e 6974 656d 2829 0a20 2020 2020 2020  ].item().       
-00024800: 2070 6572 6365 6e74 3320 3d20 726f 756e   percent3 = roun
-00024810: 6428 2864 6179 4d69 6e75 7332 202d 2064  d((dayMinus2 - d
-00024820: 6179 4d69 6e75 7333 2920 2a20 3130 3020  ayMinus3) * 100 
-00024830: 2f20 6461 794d 696e 7573 332c 2032 290a  / dayMinus3, 2).
-00024840: 2020 2020 2020 2020 7065 7263 656e 7432          percent2
-00024850: 203d 2072 6f75 6e64 2828 6461 794d 696e   = round((dayMin
-00024860: 7573 3120 2d20 6461 794d 696e 7573 3229  us1 - dayMinus2)
-00024870: 202a 2031 3030 202f 2064 6179 4d69 6e75   * 100 / dayMinu
-00024880: 7332 2c20 3229 0a20 2020 2020 2020 2070  s2, 2).        p
-00024890: 6572 6365 6e74 3120 3d20 726f 756e 6428  ercent1 = round(
-000248a0: 2864 6179 3020 2d20 6461 794d 696e 7573  (day0 - dayMinus
-000248b0: 3129 202a 2031 3030 202f 2064 6179 4d69  1) * 100 / dayMi
-000248c0: 6e75 7331 2c20 3229 0a0a 2020 2020 2020  nus1, 2)..      
-000248d0: 2020 6966 2070 6572 6365 6e74 3120 3e3d    if percent1 >=
-000248e0: 2032 2061 6e64 2070 6572 6365 6e74 3220   2 and percent2 
-000248f0: 3e3d 2032 2061 6e64 2070 6572 6365 6e74  >= 2 and percent
-00024900: 3320 3e3d 2032 3a0a 2020 2020 2020 2020  3 >= 2:.        
-00024910: 2020 2020 7063 745f 6368 616e 6765 5f74      pct_change_t
-00024920: 6578 7420 3d20 280a 2020 2020 2020 2020  ext = (.        
-00024930: 2020 2020 2020 2020 2822 252e 3166 2525          ("%.1f%%
-00024940: 2220 2520 7065 7263 656e 7431 290a 2020  " % percent1).  
-00024950: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-00024960: 2822 2028 252e 3166 2525 2c22 2025 2070  (" (%.1f%%," % p
-00024970: 6572 6365 6e74 3229 0a20 2020 2020 2020  ercent2).       
-00024980: 2020 2020 2020 2020 202b 2028 2220 252e           + (" %.
-00024990: 3166 2525 2922 2025 2070 6572 6365 6e74  1f%%)" % percent
-000249a0: 3329 0a20 2020 2020 2020 2020 2020 2029  3).            )
-000249b0: 0a20 2020 2020 2020 2020 2020 2073 6176  .            sav
-000249c0: 6544 6963 745b 2225 4368 6e67 225d 203d  eDict["%Chng"] =
-000249d0: 2070 6374 5f63 6861 6e67 655f 7465 7874   pct_change_text
-000249e0: 0a20 2020 2020 2020 2020 2020 2073 6372  .            scr
-000249f0: 6565 6e44 6963 745b 2225 4368 6e67 225d  eenDict["%Chng"]
-00024a00: 203d 2063 6f6c 6f72 5465 7874 2e47 5245   = colorText.GRE
-00024a10: 454e 202b 2070 6374 5f63 6861 6e67 655f  EN + pct_change_
-00024a20: 7465 7874 202b 2063 6f6c 6f72 5465 7874  text + colorText
-00024a30: 2e45 4e44 0a20 2020 2020 2020 2020 2020  .END.           
-00024a40: 2072 6574 7572 6e20 5472 7565 2061 6e64   return True and
-00024a50: 2073 656c 662e 6765 7443 616e 646c 6554   self.getCandleT
-00024a60: 7970 6528 6461 7461 2e68 6561 6428 3129  ype(data.head(1)
-00024a70: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00024a80: 2046 616c 7365 0a0a 2020 2020 2340 6d65   False..    #@me
-00024a90: 6173 7572 655f 7469 6d65 0a20 2020 2023  asure_time.    #
-00024aa0: 2076 616c 6964 6174 6520 6966 2052 5349   validate if RSI
-00024ab0: 2069 7320 7769 7468 696e 2067 6976 656e   is within given
-00024ac0: 2072 616e 6765 0a20 2020 2064 6566 2076   range.    def v
-00024ad0: 616c 6964 6174 6552 5349 2873 656c 662c  alidateRSI(self,
-00024ae0: 2064 662c 2073 6372 6565 6e44 6963 742c   df, screenDict,
-00024af0: 2073 6176 6544 6963 742c 206d 696e 5253   saveDict, minRS
-00024b00: 492c 206d 6178 5253 492c 7273 694b 6579  I, maxRSI,rsiKey
-00024b10: 3d22 5253 4922 293a 0a20 2020 2020 2020  ="RSI"):.       
-00024b20: 2069 6620 6466 2069 7320 4e6f 6e65 206f   if df is None o
-00024b30: 7220 6c65 6e28 6466 2920 3d3d 2030 3a0a  r len(df) == 0:.
-00024b40: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00024b50: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
-00024b60: 2069 6620 7273 694b 6579 206e 6f74 2069   if rsiKey not i
-00024b70: 6e20 6466 2e63 6f6c 756d 6e73 3a0a 2020  n df.columns:.  
-00024b80: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00024b90: 2046 616c 7365 0a20 2020 2020 2020 2064   False.        d
-00024ba0: 6174 6120 3d20 6466 2e63 6f70 7928 290a  ata = df.copy().
-00024bb0: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
-00024bc0: 6174 612e 6669 6c6c 6e61 2830 290a 2020  ata.fillna(0).  
-00024bd0: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
-00024be0: 612e 7265 706c 6163 6528 5b6e 702e 696e  a.replace([np.in
-00024bf0: 662c 202d 6e70 2e69 6e66 5d2c 2030 290a  f, -np.inf], 0).
-00024c00: 2020 2020 2020 2020 7273 6920 3d20 696e          rsi = in
-00024c10: 7428 6461 7461 2e68 6561 6428 3129 5b72  t(data.head(1)[r
-00024c20: 7369 4b65 795d 2e69 6c6f 635b 305d 290a  siKey].iloc[0]).
-00024c30: 2020 2020 2020 2020 7361 7665 4469 6374          saveDict
-00024c40: 5b72 7369 4b65 795d 203d 2072 7369 0a20  [rsiKey] = rsi. 
-00024c50: 2020 2020 2020 2023 2068 7474 7073 3a2f         # https:/
-00024c60: 2f63 6861 7274 696e 6b2e 636f 6d2f 7363  /chartink.com/sc
-00024c70: 7265 656e 6572 2f72 7369 2d73 6372 6565  reener/rsi-scree
-00024c80: 6e69 6e67 0a20 2020 2020 2020 2069 6620  ning.        if 
-00024c90: 7273 693e 2030 2061 6e64 2072 7369 203e  rsi> 0 and rsi >
-00024ca0: 3d20 6d69 6e52 5349 2061 6e64 2072 7369  = minRSI and rsi
-00024cb0: 203c 3d20 6d61 7852 5349 3a20 2023 206f   <= maxRSI:  # o
-00024cc0: 7220 2872 7369 203c 3d20 3731 2061 6e64  r (rsi <= 71 and
-00024cd0: 2072 7369 203e 3d20 3637 293a 0a20 2020   rsi >= 67):.   
-00024ce0: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
-00024cf0: 6963 745b 7273 694b 6579 5d20 3d20 280a  ict[rsiKey] = (.
-00024d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024d10: 636f 6c6f 7254 6578 742e 424f 4c44 202b  colorText.BOLD +
-00024d20: 2063 6f6c 6f72 5465 7874 2e47 5245 454e   colorText.GREEN
-00024d30: 202b 2073 7472 2872 7369 2920 2b20 636f   + str(rsi) + co
-00024d40: 6c6f 7254 6578 742e 454e 440a 2020 2020  lorText.END.    
-00024d50: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00024d60: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
-00024d70: 6520 6966 2028 7273 694b 6579 203d 3d20  e if (rsiKey == 
-00024d80: 2252 5349 6922 2920 656c 7365 2028 7365  "RSIi") else (se
-00024d90: 6c66 2e76 616c 6964 6174 6552 5349 2864  lf.validateRSI(d
-00024da0: 662c 2073 6372 6565 6e44 6963 742c 2073  f, screenDict, s
-00024db0: 6176 6544 6963 742c 206d 696e 5253 492c  aveDict, minRSI,
-00024dc0: 206d 6178 5253 492c 7273 694b 6579 3d22   maxRSI,rsiKey="
-00024dd0: 5253 4969 2229 206f 7220 5472 7565 290a  RSIi") or True).
-00024de0: 2020 2020 2020 2020 7363 7265 656e 4469          screenDi
-00024df0: 6374 5b72 7369 4b65 795d 203d 2063 6f6c  ct[rsiKey] = col
-00024e00: 6f72 5465 7874 2e42 4f4c 4420 2b20 636f  orText.BOLD + co
-00024e10: 6c6f 7254 6578 742e 4641 494c 202b 2073  lorText.FAIL + s
-00024e20: 7472 2872 7369 2920 2b20 636f 6c6f 7254  tr(rsi) + colorT
-00024e30: 6578 742e 454e 440a 2020 2020 2020 2020  ext.END.        
-00024e40: 2320 4966 2065 6974 6865 7220 6461 696c  # If either dail
-00024e50: 7920 6f72 2069 6e74 7261 6461 7920 5253  y or intraday RS
-00024e60: 4920 636f 6d65 7320 7769 7468 696e 2072  I comes within r
-00024e70: 616e 6765 3f0a 2020 2020 2020 2020 7265  ange?.        re
-00024e80: 7475 726e 2046 616c 7365 2069 6620 2872  turn False if (r
-00024e90: 7369 4b65 7920 3d3d 2022 5253 4969 2229  siKey == "RSIi")
-00024ea0: 2065 6c73 6520 2873 656c 662e 7661 6c69   else (self.vali
-00024eb0: 6461 7465 5253 4928 6466 2c20 7363 7265  dateRSI(df, scre
-00024ec0: 656e 4469 6374 2c20 7361 7665 4469 6374  enDict, saveDict
-00024ed0: 2c20 6d69 6e52 5349 2c20 6d61 7852 5349  , minRSI, maxRSI
-00024ee0: 2c72 7369 4b65 793d 2252 5349 6922 2929  ,rsiKey="RSIi"))
-00024ef0: 0a0a 2020 2020 2320 5661 6c69 6461 7465  ..    # Validate
-00024f00: 2069 6620 7468 6520 7374 6f63 6b20 6973   if the stock is
-00024f10: 2062 756c 6c69 7368 2069 6e20 7468 6520   bullish in the 
-00024f20: 7368 6f72 7420 7465 726d 0a20 2020 2064  short term.    d
-00024f30: 6566 2076 616c 6964 6174 6553 686f 7274  ef validateShort
-00024f40: 5465 726d 4275 6c6c 6973 6828 7365 6c66  TermBullish(self
-00024f50: 2c20 6466 2c20 7363 7265 656e 4469 6374  , df, screenDict
-00024f60: 2c20 7361 7665 4469 6374 293a 0a20 2020  , saveDict):.   
-00024f70: 2020 2020 2069 6620 6466 2069 7320 4e6f       if df is No
-00024f80: 6e65 206f 7220 6c65 6e28 6466 2920 3d3d  ne or len(df) ==
-00024f90: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
-00024fa0: 7265 7475 726e 2046 616c 7365 0a20 2020  return False.   
-00024fb0: 2020 2020 2064 6174 6120 3d20 6466 2e63       data = df.c
-00024fc0: 6f70 7928 290a 2020 2020 2020 2020 2320  opy().        # 
-00024fd0: 6874 7470 733a 2f2f 6368 6172 7469 6e6b  https://chartink
-00024fe0: 2e63 6f6d 2f73 6372 6565 6e65 722f 7368  .com/screener/sh
-00024ff0: 6f72 742d 7465 726d 2d62 756c 6c69 7368  ort-term-bullish
-00025000: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
-00025010: 6461 7461 2e66 696c 6c6e 6128 3029 0a20  data.fillna(0). 
-00025020: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
-00025030: 7461 2e72 6570 6c61 6365 285b 6e70 2e69  ta.replace([np.i
-00025040: 6e66 2c20 2d6e 702e 696e 665d 2c20 3029  nf, -np.inf], 0)
-00025050: 0a20 2020 2020 2020 2072 6563 656e 7420  .        recent 
-00025060: 3d20 6461 7461 2e68 6561 6428 3129 0a20  = data.head(1). 
-00025070: 2020 2020 2020 2066 6b20 3d20 3020 6966         fk = 0 if
-00025080: 206c 656e 2864 6174 6129 203c 2033 2065   len(data) < 3 e
-00025090: 6c73 6520 6e70 2e72 6f75 6e64 2864 6174  lse np.round(dat
-000250a0: 615b 2246 4153 544b 225d 2e69 6c6f 635b  a["FASTK"].iloc[
-000250b0: 325d 2c20 3529 0a20 2020 2020 2020 2023  2], 5).        #
-000250c0: 2052 6576 6572 7365 2074 6865 2064 6174   Reverse the dat
-000250d0: 6166 7261 6d65 2066 6f72 2069 6368 696d  aframe for ichim
-000250e0: 6f6b 7520 6361 6c63 756c 6174 696f 6e73  oku calculations
-000250f0: 2077 6974 6820 6461 7465 2069 6e20 6173   with date in as
-00025100: 6365 6e64 696e 6720 6f72 6465 720a 2020  cending order.  
-00025110: 2020 2020 2020 6466 5f6e 6577 203d 2064        df_new = d
-00025120: 6174 615b 3a3a 2d31 5d0a 2020 2020 2020  ata[::-1].      
-00025130: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-00025140: 2020 2064 665f 6963 6869 203d 2064 665f     df_ichi = df_
-00025150: 6e65 772e 7265 6e61 6d65 280a 2020 2020  new.rename(.    
-00025160: 2020 2020 2020 2020 2020 2020 636f 6c75              colu
-00025170: 6d6e 733d 7b0a 2020 2020 2020 2020 2020  mns={.          
-00025180: 2020 2020 2020 2020 2020 224f 7065 6e22            "Open"
-00025190: 3a20 226f 7065 6e22 2c0a 2020 2020 2020  : "open",.      
-000251a0: 2020 2020 2020 2020 2020 2020 2020 2248                "H
-000251b0: 6967 6822 3a20 2268 6967 6822 2c0a 2020  igh": "high",.  
-000251c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000251d0: 2020 224c 6f77 223a 2022 6c6f 7722 2c0a    "Low": "low",.
-000251e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000251f0: 2020 2020 2243 6c6f 7365 223a 2022 636c      "Close": "cl
-00025200: 6f73 6522 2c0a 2020 2020 2020 2020 2020  ose",.          
-00025210: 2020 2020 2020 2020 2020 2256 6f6c 756d            "Volum
-00025220: 6522 3a20 2276 6f6c 756d 6522 2c0a 2020  e": "volume",.  
-00025230: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
-00025240: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00025250: 2020 2020 2020 2020 2020 6963 6869 203d            ichi =
-00025260: 2070 6b74 616c 6962 2e69 6368 696d 6f6b   pktalib.ichimok
-00025270: 7528 6466 5f69 6368 692c 2039 2c20 3236  u(df_ichi, 9, 26
-00025280: 2c20 3532 2c20 3236 290a 2020 2020 2020  , 52, 26).      
-00025290: 2020 2020 2020 6966 2069 6368 6920 6973        if ichi is
-000252a0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000252b0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-000252c0: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
-000252d0: 6466 5f6e 6577 203d 2070 642e 636f 6e63  df_new = pd.conc
-000252e0: 6174 285b 6466 5f6e 6577 2c20 6963 6869  at([df_new, ichi
-000252f0: 5d2c 2061 7869 733d 3129 0a20 2020 2020  ], axis=1).     
-00025300: 2020 2020 2020 2023 2052 6576 6572 7365         # Reverse
-00025310: 2061 6761 696e 2074 6f20 6765 7420 7468   again to get th
-00025320: 6520 6d6f 7374 2072 6563 656e 7420 6461  e most recent da
-00025330: 7465 206f 6e20 746f 700a 2020 2020 2020  te on top.      
-00025340: 2020 2020 2020 6466 5f6e 6577 203d 2064        df_new = d
-00025350: 665f 6e65 775b 3a3a 2d31 5d0a 2020 2020  f_new[::-1].    
-00025360: 2020 2020 2020 2020 6466 5f6e 6577 203d          df_new =
-00025370: 2064 665f 6e65 772e 6865 6164 2831 290a   df_new.head(1).
-00025380: 2020 2020 2020 2020 2020 2020 6466 5f6e              df_n
-00025390: 6577 5b22 636c 6f75 645f 6772 6565 6e22  ew["cloud_green"
-000253a0: 5d20 3d20 6466 5f6e 6577 5b22 4953 415f  ] = df_new["ISA_
-000253b0: 3922 5d2e 696c 6f63 5b30 5d20 3e20 6466  9"].iloc[0] > df
-000253c0: 5f6e 6577 5b22 4953 425f 3236 225d 2e69  _new["ISB_26"].i
-000253d0: 6c6f 635b 305d 0a20 2020 2020 2020 2020  loc[0].         
-000253e0: 2020 2064 665f 6e65 775b 2263 6c6f 7564     df_new["cloud
-000253f0: 5f72 6564 225d 203d 2064 665f 6e65 775b  _red"] = df_new[
-00025400: 2249 5342 5f32 3622 5d2e 696c 6f63 5b30  "ISB_26"].iloc[0
-00025410: 5d20 3e20 6466 5f6e 6577 5b22 4953 415f  ] > df_new["ISA_
-00025420: 3922 5d2e 696c 6f63 5b30 5d0a 2020 2020  9"].iloc[0].    
-00025430: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
-00025440: 7469 6f6e 2061 7320 653a 2020 2320 7072  tion as e:  # pr
-00025450: 6167 6d61 3a20 6e6f 2063 6f76 6572 0a20  agma: no cover. 
-00025460: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00025470: 6465 6661 756c 745f 6c6f 6767 6572 2e64  default_logger.d
-00025480: 6562 7567 2865 2c20 6578 635f 696e 666f  ebug(e, exc_info
-00025490: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
-000254a0: 2020 2070 6173 730a 2020 2020 2020 2020     pass.        
-000254b0: 6162 6f76 6543 6c6f 7564 546f 7020 3d20  aboveCloudTop = 
-000254c0: 4661 6c73 650a 2020 2020 2020 2020 2320  False.        # 
-000254d0: 6261 7365 6c69 6e65 203e 2063 6c6f 7564  baseline > cloud
-000254e0: 2074 6f70 2028 636c 6f75 6420 6973 2062   top (cloud is b
-000254f0: 6f75 6e64 2062 7920 7370 616e 2061 2061  ound by span a a
-00025500: 6e64 2073 7061 6e20 6229 2061 6e64 2063  nd span b) and c
-00025510: 6c6f 7365 2069 7320 3e20 636c 6f75 6420  lose is > cloud 
-00025520: 746f 700a 2020 2020 2020 2020 6966 2064  top.        if d
-00025530: 665f 6e65 775b 2263 6c6f 7564 5f67 7265  f_new["cloud_gre
-00025540: 656e 225d 2e69 6c6f 635b 305d 3a0a 2020  en"].iloc[0]:.  
-00025550: 2020 2020 2020 2020 2020 6162 6f76 6543            aboveC
-00025560: 6c6f 7564 546f 7020 3d20 280a 2020 2020  loudTop = (.    
-00025570: 2020 2020 2020 2020 2020 2020 6466 5f6e              df_n
-00025580: 6577 5b22 494b 535f 3236 225d 2e69 6c6f  ew["IKS_26"].ilo
-00025590: 635b 305d 203e 2064 665f 6e65 775b 2249  c[0] > df_new["I
-000255a0: 5341 5f39 225d 2e69 6c6f 635b 305d 0a20  SA_9"].iloc[0]. 
-000255b0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-000255c0: 6e64 2072 6563 656e 745b 2243 6c6f 7365  nd recent["Close
-000255d0: 225d 2e69 6c6f 635b 305d 203e 2064 665f  "].iloc[0] > df_
-000255e0: 6e65 775b 2249 5341 5f39 225d 2e69 6c6f  new["ISA_9"].ilo
-000255f0: 635b 305d 0a20 2020 2020 2020 2020 2020  c[0].           
-00025600: 2029 0a20 2020 2020 2020 2065 6c69 6620   ).        elif 
-00025610: 6466 5f6e 6577 5b22 636c 6f75 645f 7265  df_new["cloud_re
-00025620: 6422 5d2e 696c 6f63 5b30 5d3a 0a20 2020  d"].iloc[0]:.   
-00025630: 2020 2020 2020 2020 2061 626f 7665 436c           aboveCl
-00025640: 6f75 6454 6f70 203d 2028 0a20 2020 2020  oudTop = (.     
-00025650: 2020 2020 2020 2020 2020 2064 665f 6e65             df_ne
-00025660: 775b 2249 4b53 5f32 3622 5d2e 696c 6f63  w["IKS_26"].iloc
-00025670: 5b30 5d20 3e20 6466 5f6e 6577 5b22 4953  [0] > df_new["IS
-00025680: 425f 3236 225d 2e69 6c6f 635b 305d 0a20  B_26"].iloc[0]. 
-00025690: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-000256a0: 6e64 2072 6563 656e 745b 2243 6c6f 7365  nd recent["Close
-000256b0: 225d 2e69 6c6f 635b 305d 203e 2064 665f  "].iloc[0] > df_
-000256c0: 6e65 775b 2249 5342 5f32 3622 5d2e 696c  new["ISB_26"].il
-000256d0: 6f63 5b30 5d0a 2020 2020 2020 2020 2020  oc[0].          
-000256e0: 2020 290a 0a20 2020 2020 2020 2023 204c    )..        # L
-000256f0: 6174 6573 7420 4963 6869 6d6f 6b75 2062  atest Ichimoku b
-00025700: 6173 656c 696e 6520 6973 203c 206c 6174  aseline is < lat
-00025710: 6573 7420 4963 6869 6d6f 6b75 2063 6f6e  est Ichimoku con
-00025720: 7665 7273 696f 6e20 6c69 6e65 0a20 2020  version line.   
-00025730: 2020 2020 2069 6620 6162 6f76 6543 6c6f       if aboveClo
-00025740: 7564 546f 7020 616e 6420 6466 5f6e 6577  udTop and df_new
-00025750: 5b22 494b 535f 3236 225d 2e69 6c6f 635b  ["IKS_26"].iloc[
-00025760: 305d 203c 2064 665f 6e65 775b 2249 5453  0] < df_new["ITS
-00025770: 5f39 225d 2e69 6c6f 635b 305d 3a0a 2020  _9"].iloc[0]:.  
-00025780: 2020 2020 2020 2020 2020 2320 5374 6f63            # Stoc
-00025790: 6852 5349 2063 726f 7373 6564 2032 3020  hRSI crossed 20 
-000257a0: 616e 6420 5253 4920 3e20 3530 0a20 2020  and RSI > 50.   
-000257b0: 2020 2020 2020 2020 2069 6620 666b 203e           if fk >
-000257c0: 2032 3020 616e 6420 7265 6365 6e74 5b22   20 and recent["
-000257d0: 5253 4922 5d2e 696c 6f63 5b30 5d20 3e20  RSI"].iloc[0] > 
-000257e0: 3530 3a0a 2020 2020 2020 2020 2020 2020  50:.            
-000257f0: 2020 2020 2320 636f 6e64 6974 696f 6e20      # condition 
-00025800: 6f66 2063 726f 7373 696e 6720 7468 6520  of crossing the 
-00025810: 5374 6f63 6852 5349 206d 6169 6e20 7369  StochRSI main si
-00025820: 676e 616c 206c 696e 6520 6672 6f6d 2062  gnal line from b
-00025830: 6f74 746f 6d20 746f 2074 6f70 0a20 2020  ottom to top.   
-00025840: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00025850: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00025860: 2020 2020 2020 6461 7461 5b22 4641 5354        data["FAST
-00025870: 4422 5d2e 696c 6f63 5b31 3030 5d20 3c20  D"].iloc[100] < 
-00025880: 6461 7461 5b22 4641 5354 4b22 5d2e 696c  data["FASTK"].il
-00025890: 6f63 5b31 3030 5d0a 2020 2020 2020 2020  oc[100].        
-000258a0: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-000258b0: 6461 7461 5b22 4641 5354 4422 5d2e 696c  data["FASTD"].il
-000258c0: 6f63 5b31 3031 5d20 3e20 6461 7461 5b22  oc[101] > data["
-000258d0: 4641 5354 4b22 5d2e 696c 6f63 5b31 3031  FASTK"].iloc[101
-000258e0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-000258f0: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
-00025900: 2020 2020 2020 2020 2023 2063 6c6f 7365           # close
-00025910: 203e 2035 3020 7065 7269 6f64 2053 4d41   > 50 period SMA
-00025920: 2f45 4d41 2061 6e64 2032 3030 2070 6572  /EMA and 200 per
-00025930: 696f 6420 534d 412f 454d 410a 2020 2020  iod SMA/EMA.    
-00025940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025950: 6966 2028 0a20 2020 2020 2020 2020 2020  if (.           
-00025960: 2020 2020 2020 2020 2020 2020 2072 6563               rec
-00025970: 656e 745b 2253 534d 4122 5d2e 696c 6f63  ent["SSMA"].iloc
-00025980: 5b30 5d20 3e20 7265 6365 6e74 5b22 534d  [0] > recent["SM
-00025990: 4122 5d2e 696c 6f63 5b30 5d0a 2020 2020  A"].iloc[0].    
-000259a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000259b0: 2020 2020 616e 6420 7265 6365 6e74 5b22      and recent["
-000259c0: 436c 6f73 6522 5d2e 696c 6f63 5b30 5d20  Close"].iloc[0] 
-000259d0: 3e20 7265 6365 6e74 5b22 5353 4d41 225d  > recent["SSMA"]
-000259e0: 2e69 6c6f 635b 305d 0a20 2020 2020 2020  .iloc[0].       
-000259f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025a00: 2061 6e64 2072 6563 656e 745b 2243 6c6f   and recent["Clo
-00025a10: 7365 225d 2e69 6c6f 635b 305d 203e 2072  se"].iloc[0] > r
-00025a20: 6563 656e 745b 224c 4d41 225d 2e69 6c6f  ecent["LMA"].ilo
-00025a30: 635b 305d 0a20 2020 2020 2020 2020 2020  c[0].           
-00025a40: 2020 2020 2020 2020 2029 3a0a 2020 2020           ):.    
-00025a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025a60: 2020 2020 7361 7665 6420 3d20 7365 6c66      saved = self
-00025a70: 2e66 696e 6443 7572 7265 6e74 5361 7665  .findCurrentSave
-00025a80: 6456 616c 7565 2873 6372 6565 6e44 6963  dValue(screenDic
-00025a90: 742c 7361 7665 4469 6374 2c22 4d41 2d53  t,saveDict,"MA-S
-00025aa0: 6967 6e61 6c22 290a 2020 2020 2020 2020  ignal").        
+00023ab0: 2020 2020 2020 7361 7665 4469 6374 5b22        saveDict["
+00023ac0: 4d41 2d53 6967 6e61 6c22 5d20 3d20 7361  MA-Signal"] = sa
+00023ad0: 7665 645b 315d 202b 2066 2242 6561 7243  ved[1] + f"BearC
+00023ae0: 726f 7373 2d7b 6d61 5465 7874 735b 696e  ross-{maTexts[in
+00023af0: 6465 785d 7d22 0a20 2020 2020 2020 2020  dex]}".         
+00023b00: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00023b10: 6152 6576 6572 7361 6c20 3d20 2d31 0a20  aReversal = -1. 
+00023b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023b30: 2020 2020 2020 206d 6153 6967 6e61 6c73         maSignals
+00023b40: 2e61 7070 656e 6428 2234 2229 0a20 2020  .append("4").   
+00023b50: 2020 2020 2020 2020 2020 2020 2069 6e64               ind
+00023b60: 6578 202b 3d20 310a 2020 2020 2020 2020  ex += 1.        
+00023b70: 7265 7475 726e 5661 6c75 6520 3d20 6d61  returnValue = ma
+00023b80: 5265 7665 7273 616c 0a20 2020 2020 2020  Reversal.       
+00023b90: 2069 6620 6d61 4c65 6e67 7468 2021 3d20   if maLength != 
+00023ba0: 303a 0a20 2020 2020 2020 2020 2020 2072  0:.            r
+00023bb0: 6574 7572 6e56 616c 7565 203d 2073 7472  eturnValue = str
+00023bc0: 286d 614c 656e 6774 6829 2069 6e20 6d61  (maLength) in ma
+00023bd0: 5369 676e 616c 730a 2020 2020 2020 2020  Signals.        
+00023be0: 7265 7475 726e 2072 6574 7572 6e56 616c  return returnVal
+00023bf0: 7565 0a0a 2020 2020 2320 4669 6e64 204e  ue..    # Find N
+00023c00: 5278 2072 616e 6765 2066 6f72 2052 6576  Rx range for Rev
+00023c10: 6572 7361 6c0a 2020 2020 6465 6620 7661  ersal.    def va
+00023c20: 6c69 6461 7465 4e61 7272 6f77 5261 6e67  lidateNarrowRang
+00023c30: 6528 7365 6c66 2c20 6466 2c20 7363 7265  e(self, df, scre
+00023c40: 656e 4469 6374 2c20 7361 7665 4469 6374  enDict, saveDict
+00023c50: 2c20 6e72 3d34 293a 0a20 2020 2020 2020  , nr=4):.       
+00023c60: 2069 6620 6466 2069 7320 4e6f 6e65 206f   if df is None o
+00023c70: 7220 6c65 6e28 6466 2920 3d3d 2030 3a0a  r len(df) == 0:.
+00023c80: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00023c90: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
+00023ca0: 2064 6174 6120 3d20 6466 2e63 6f70 7928   data = df.copy(
+00023cb0: 290a 2020 2020 2020 2020 7361 7665 6420  ).        saved 
+00023cc0: 3d20 7365 6c66 2e66 696e 6443 7572 7265  = self.findCurre
+00023cd0: 6e74 5361 7665 6456 616c 7565 2873 6372  ntSavedValue(scr
+00023ce0: 6565 6e44 6963 742c 2073 6176 6544 6963  eenDict, saveDic
+00023cf0: 742c 2022 5061 7474 6572 6e22 290a 2020  t, "Pattern").  
+00023d00: 2020 2020 2020 6966 2050 4b44 6174 6555        if PKDateU
+00023d10: 7469 6c69 7469 6573 2e69 7354 7261 6469  tilities.isTradi
+00023d20: 6e67 5469 6d65 2829 3a0a 2020 2020 2020  ngTime():.      
+00023d30: 2020 2020 2020 7261 6e67 6544 6174 6120        rangeData 
+00023d40: 3d20 6461 7461 2e68 6561 6428 6e72 202b  = data.head(nr +
+00023d50: 2031 295b 313a 5d0a 2020 2020 2020 2020   1)[1:].        
+00023d60: 2020 2020 6e6f 775f 6361 6e64 6c65 203d      now_candle =
+00023d70: 2064 6174 612e 6865 6164 2831 290a 2020   data.head(1).  
+00023d80: 2020 2020 2020 2020 2020 7261 6e67 6544            rangeD
+00023d90: 6174 615b 2252 616e 6765 225d 203d 2061  ata["Range"] = a
+00023da0: 6273 2872 616e 6765 4461 7461 5b22 436c  bs(rangeData["Cl
+00023db0: 6f73 6522 5d20 2d20 7261 6e67 6544 6174  ose"] - rangeDat
+00023dc0: 615b 224f 7065 6e22 5d29 0a20 2020 2020  a["Open"]).     
+00023dd0: 2020 2020 2020 2072 6563 656e 7420 3d20         recent = 
+00023de0: 7261 6e67 6544 6174 612e 6865 6164 2831  rangeData.head(1
+00023df0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00023e00: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+00023e10: 2020 206c 656e 2872 6563 656e 7429 203d     len(recent) =
+00023e20: 3d20 310a 2020 2020 2020 2020 2020 2020  = 1.            
+00023e30: 2020 2020 616e 6420 7265 6365 6e74 5b22      and recent["
+00023e40: 5261 6e67 6522 5d2e 696c 6f63 5b30 5d20  Range"].iloc[0] 
+00023e50: 3d3d 2072 616e 6765 4461 7461 2e64 6573  == rangeData.des
+00023e60: 6372 6962 6528 295b 2252 616e 6765 225d  cribe()["Range"]
+00023e70: 5b22 6d69 6e22 5d0a 2020 2020 2020 2020  ["min"].        
+00023e80: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
+00023e90: 2020 2020 2020 2069 6620 280a 2020 2020         if (.    
+00023ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023eb0: 7365 6c66 2e67 6574 4361 6e64 6c65 5479  self.getCandleTy
+00023ec0: 7065 2872 6563 656e 7429 0a20 2020 2020  pe(recent).     
+00023ed0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00023ee0: 6e64 206e 6f77 5f63 616e 646c 655b 2243  nd now_candle["C
+00023ef0: 6c6f 7365 225d 2e69 6c6f 635b 305d 203e  lose"].iloc[0] >
+00023f00: 3d20 7265 6365 6e74 5b22 436c 6f73 6522  = recent["Close"
+00023f10: 5d2e 696c 6f63 5b30 5d0a 2020 2020 2020  ].iloc[0].      
+00023f20: 2020 2020 2020 2020 2020 293a 0a20 2020            ):.   
+00023f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023f40: 2073 6372 6565 6e44 6963 745b 2250 6174   screenDict["Pat
+00023f50: 7465 726e 225d 203d 2028 0a20 2020 2020  tern"] = (.     
+00023f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023f70: 2020 2073 6176 6564 5b30 5d20 2b20 636f     saved[0] + co
+00023f80: 6c6f 7254 6578 742e 424f 4c44 202b 2063  lorText.BOLD + c
+00023f90: 6f6c 6f72 5465 7874 2e47 5245 454e 202b  olorText.GREEN +
+00023fa0: 2066 2242 7579 2d4e 527b 6e72 7d22 202b   f"Buy-NR{nr}" +
+00023fb0: 2063 6f6c 6f72 5465 7874 2e45 4e44 0a20   colorText.END. 
+00023fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023fd0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00023fe0: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
+00023ff0: 745b 2250 6174 7465 726e 225d 203d 2073  t["Pattern"] = s
+00024000: 6176 6564 5b31 5d20 2b20 6622 4275 792d  aved[1] + f"Buy-
+00024010: 4e52 7b6e 727d 220a 2020 2020 2020 2020  NR{nr}".        
+00024020: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00024030: 726e 2054 7275 650a 2020 2020 2020 2020  rn True.        
+00024040: 2020 2020 2020 2020 656c 6966 2028 0a20          elif (. 
+00024050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024060: 2020 206e 6f74 2073 656c 662e 6765 7443     not self.getC
+00024070: 616e 646c 6554 7970 6528 7265 6365 6e74  andleType(recent
+00024080: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00024090: 2020 2020 2020 616e 6420 6e6f 775f 6361        and now_ca
+000240a0: 6e64 6c65 5b22 436c 6f73 6522 5d2e 696c  ndle["Close"].il
+000240b0: 6f63 5b30 5d20 3c3d 2072 6563 656e 745b  oc[0] <= recent[
+000240c0: 2243 6c6f 7365 225d 2e69 6c6f 635b 305d  "Close"].iloc[0]
+000240d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000240e0: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
+000240f0: 2020 2020 2020 2020 7363 7265 656e 4469          screenDi
+00024100: 6374 5b22 5061 7474 6572 6e22 5d20 3d20  ct["Pattern"] = 
+00024110: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00024120: 2020 2020 2020 2020 2020 7361 7665 645b            saved[
+00024130: 305d 202b 2063 6f6c 6f72 5465 7874 2e42  0] + colorText.B
+00024140: 4f4c 4420 2b20 636f 6c6f 7254 6578 742e  OLD + colorText.
+00024150: 4641 494c 202b 2066 2253 656c 6c2d 4e52  FAIL + f"Sell-NR
+00024160: 7b6e 727d 2220 2b20 636f 6c6f 7254 6578  {nr}" + colorTex
+00024170: 742e 454e 440a 2020 2020 2020 2020 2020  t.END.          
+00024180: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00024190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000241a0: 7361 7665 4469 6374 5b22 5061 7474 6572  saveDict["Patter
+000241b0: 6e22 5d20 3d20 7361 7665 645b 315d 202b  n"] = saved[1] +
+000241c0: 2066 2253 656c 6c2d 4e52 7b6e 727d 220a   f"Sell-NR{nr}".
+000241d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000241e0: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+000241f0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00024200: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
+00024210: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00024220: 2020 2072 616e 6765 4461 7461 203d 2064     rangeData = d
+00024230: 6174 612e 6865 6164 286e 7229 0a20 2020  ata.head(nr).   
+00024240: 2020 2020 2020 2020 2072 616e 6765 4461           rangeDa
+00024250: 7461 2e6c 6f63 5b3a 2c27 5261 6e67 6527  ta.loc[:,'Range'
+00024260: 5d20 3d20 6162 7328 7261 6e67 6544 6174  ] = abs(rangeDat
+00024270: 615b 2243 6c6f 7365 225d 202d 2072 616e  a["Close"] - ran
+00024280: 6765 4461 7461 5b22 4f70 656e 225d 290a  geData["Open"]).
+00024290: 2020 2020 2020 2020 2020 2020 7265 6365              rece
+000242a0: 6e74 203d 2072 616e 6765 4461 7461 2e68  nt = rangeData.h
+000242b0: 6561 6428 3129 0a20 2020 2020 2020 2020  ead(1).         
+000242c0: 2020 2069 6620 7265 6365 6e74 5b22 5261     if recent["Ra
+000242d0: 6e67 6522 5d2e 696c 6f63 5b30 5d20 3d3d  nge"].iloc[0] ==
+000242e0: 2072 616e 6765 4461 7461 2e64 6573 6372   rangeData.descr
+000242f0: 6962 6528 295b 2252 616e 6765 225d 5b22  ibe()["Range"]["
+00024300: 6d69 6e22 5d3a 0a20 2020 2020 2020 2020  min"]:.         
+00024310: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
+00024320: 745b 2250 6174 7465 726e 225d 203d 2028  t["Pattern"] = (
+00024330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00024340: 2020 2020 2073 6176 6564 5b30 5d20 2b20       saved[0] + 
+00024350: 636f 6c6f 7254 6578 742e 424f 4c44 202b  colorText.BOLD +
+00024360: 2063 6f6c 6f72 5465 7874 2e47 5245 454e   colorText.GREEN
+00024370: 202b 2066 224e 527b 6e72 7d22 202b 2063   + f"NR{nr}" + c
+00024380: 6f6c 6f72 5465 7874 2e45 4e44 0a20 2020  olorText.END.   
+00024390: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+000243a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000243b0: 6176 6544 6963 745b 2250 6174 7465 726e  aveDict["Pattern
+000243c0: 225d 203d 2073 6176 6564 5b31 5d20 2b20  "] = saved[1] + 
+000243d0: 6622 4e52 7b6e 727d 220a 2020 2020 2020  f"NR{nr}".      
+000243e0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000243f0: 2054 7275 650a 2020 2020 2020 2020 2020   True.          
+00024400: 2020 7265 7475 726e 2046 616c 7365 0a0a    return False..
+00024410: 2020 2020 2320 4669 6e64 2069 6620 7374      # Find if st
+00024420: 6f63 6b20 6973 206e 6577 6c79 206c 6973  ock is newly lis
+00024430: 7465 640a 2020 2020 6465 6620 7661 6c69  ted.    def vali
+00024440: 6461 7465 4e65 776c 794c 6973 7465 6428  dateNewlyListed(
+00024450: 7365 6c66 2c20 6466 2c20 6461 7973 546f  self, df, daysTo
+00024460: 4c6f 6f6b 6261 636b 293a 0a20 2020 2020  Lookback):.     
+00024470: 2020 2069 6620 6466 2069 7320 4e6f 6e65     if df is None
+00024480: 206f 7220 6c65 6e28 6466 2920 3d3d 2030   or len(df) == 0
+00024490: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000244a0: 7475 726e 2046 616c 7365 0a20 2020 2020  turn False.     
+000244b0: 2020 2064 6174 6120 3d20 6466 2e63 6f70     data = df.cop
+000244c0: 7928 290a 2020 2020 2020 2020 6461 7973  y().        days
+000244d0: 546f 4c6f 6f6b 6261 636b 203d 2069 6e74  ToLookback = int
+000244e0: 2864 6179 7354 6f4c 6f6f 6b62 6163 6b5b  (daysToLookback[
+000244f0: 3a2d 315d 290a 2020 2020 2020 2020 7265  :-1]).        re
+00024500: 6365 6e74 203d 2064 6174 612e 6865 6164  cent = data.head
+00024510: 2831 290a 2020 2020 2020 2020 6966 206c  (1).        if l
+00024520: 656e 2872 6563 656e 7429 203c 2031 3a0a  en(recent) < 1:.
+00024530: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00024540: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
+00024550: 2069 6620 6c65 6e28 6461 7461 2920 3c20   if len(data) < 
+00024560: 6461 7973 546f 4c6f 6f6b 6261 636b 2061  daysToLookback a
+00024570: 6e64 2028 0a20 2020 2020 2020 2020 2020  nd (.           
+00024580: 2072 6563 656e 745b 2243 6c6f 7365 225d   recent["Close"]
+00024590: 2e69 6c6f 635b 305d 2021 3d20 6e70 2e6e  .iloc[0] != np.n
+000245a0: 616e 2061 6e64 2072 6563 656e 745b 2243  an and recent["C
+000245b0: 6c6f 7365 225d 2e69 6c6f 635b 305d 203e  lose"].iloc[0] >
+000245c0: 2030 0a20 2020 2020 2020 2029 3a0a 2020   0.        ):.  
+000245d0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000245e0: 2054 7275 650a 2020 2020 2020 2020 7265   True.        re
+000245f0: 7475 726e 2046 616c 7365 0a0a 2020 2020  turn False..    
+00024600: 2320 5661 6c69 6461 7465 2069 6620 7468  # Validate if th
+00024610: 6520 7374 6f63 6b20 7072 6963 6573 2061  e stock prices a
+00024620: 7265 2061 7420 6c65 6173 7420 7269 7369  re at least risi
+00024630: 6e67 2062 7920 3225 2066 6f72 2074 6865  ng by 2% for the
+00024640: 206c 6173 7420 3320 7365 7373 696f 6e73   last 3 sessions
+00024650: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+00024660: 6550 7269 6365 5269 7369 6e67 4279 4174  ePriceRisingByAt
+00024670: 4c65 6173 7432 5065 7263 656e 7428 7365  Least2Percent(se
+00024680: 6c66 2c20 6466 2c20 7363 7265 656e 4469  lf, df, screenDi
+00024690: 6374 2c20 7361 7665 4469 6374 293a 0a20  ct, saveDict):. 
+000246a0: 2020 2020 2020 2069 6620 6466 2069 7320         if df is 
+000246b0: 4e6f 6e65 206f 7220 6c65 6e28 6466 2920  None or len(df) 
+000246c0: 3d3d 2030 3a0a 2020 2020 2020 2020 2020  == 0:.          
+000246d0: 2020 7265 7475 726e 2046 616c 7365 0a20    return False. 
+000246e0: 2020 2020 2020 2064 6174 6120 3d20 6466         data = df
+000246f0: 2e63 6f70 7928 290a 2020 2020 2020 2020  .copy().        
+00024700: 6461 7461 203d 2064 6174 612e 6669 6c6c  data = data.fill
+00024710: 6e61 2830 290a 2020 2020 2020 2020 6461  na(0).        da
+00024720: 7461 203d 2064 6174 612e 7265 706c 6163  ta = data.replac
+00024730: 6528 5b6e 702e 696e 662c 202d 6e70 2e69  e([np.inf, -np.i
+00024740: 6e66 5d2c 2030 290a 2020 2020 2020 2020  nf], 0).        
+00024750: 6461 7461 203d 2064 6174 612e 6865 6164  data = data.head
+00024760: 2834 290a 2020 2020 2020 2020 6966 206c  (4).        if l
+00024770: 656e 2864 6174 6129 203c 2034 3a0a 2020  en(data) < 4:.  
+00024780: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00024790: 2046 616c 7365 0a20 2020 2020 2020 2064   False.        d
+000247a0: 6179 3020 3d20 6461 7461 2e69 6c6f 635b  ay0 = data.iloc[
+000247b0: 305d 5b22 436c 6f73 6522 5d2e 6974 656d  0]["Close"].item
+000247c0: 2829 0a20 2020 2020 2020 2064 6179 4d69  ().        dayMi
+000247d0: 6e75 7331 203d 2064 6174 612e 696c 6f63  nus1 = data.iloc
+000247e0: 5b31 5d5b 2243 6c6f 7365 225d 2e69 7465  [1]["Close"].ite
+000247f0: 6d28 290a 2020 2020 2020 2020 6461 794d  m().        dayM
+00024800: 696e 7573 3220 3d20 6461 7461 2e69 6c6f  inus2 = data.ilo
+00024810: 635b 325d 5b22 436c 6f73 6522 5d2e 6974  c[2]["Close"].it
+00024820: 656d 2829 0a20 2020 2020 2020 2064 6179  em().        day
+00024830: 4d69 6e75 7333 203d 2064 6174 612e 696c  Minus3 = data.il
+00024840: 6f63 5b33 5d5b 2243 6c6f 7365 225d 2e69  oc[3]["Close"].i
+00024850: 7465 6d28 290a 2020 2020 2020 2020 7065  tem().        pe
+00024860: 7263 656e 7433 203d 2072 6f75 6e64 2828  rcent3 = round((
+00024870: 6461 794d 696e 7573 3220 2d20 6461 794d  dayMinus2 - dayM
+00024880: 696e 7573 3329 202a 2031 3030 202f 2064  inus3) * 100 / d
+00024890: 6179 4d69 6e75 7333 2c20 3229 0a20 2020  ayMinus3, 2).   
+000248a0: 2020 2020 2070 6572 6365 6e74 3220 3d20       percent2 = 
+000248b0: 726f 756e 6428 2864 6179 4d69 6e75 7331  round((dayMinus1
+000248c0: 202d 2064 6179 4d69 6e75 7332 2920 2a20   - dayMinus2) * 
+000248d0: 3130 3020 2f20 6461 794d 696e 7573 322c  100 / dayMinus2,
+000248e0: 2032 290a 2020 2020 2020 2020 7065 7263   2).        perc
+000248f0: 656e 7431 203d 2072 6f75 6e64 2828 6461  ent1 = round((da
+00024900: 7930 202d 2064 6179 4d69 6e75 7331 2920  y0 - dayMinus1) 
+00024910: 2a20 3130 3020 2f20 6461 794d 696e 7573  * 100 / dayMinus
+00024920: 312c 2032 290a 0a20 2020 2020 2020 2069  1, 2)..        i
+00024930: 6620 7065 7263 656e 7431 203e 3d20 3220  f percent1 >= 2 
+00024940: 616e 6420 7065 7263 656e 7432 203e 3d20  and percent2 >= 
+00024950: 3220 616e 6420 7065 7263 656e 7433 203e  2 and percent3 >
+00024960: 3d20 323a 0a20 2020 2020 2020 2020 2020  = 2:.           
+00024970: 2070 6374 5f63 6861 6e67 655f 7465 7874   pct_change_text
+00024980: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
+00024990: 2020 2020 2028 2225 2e31 6625 2522 2025       ("%.1f%%" %
+000249a0: 2070 6572 6365 6e74 3129 0a20 2020 2020   percent1).     
+000249b0: 2020 2020 2020 2020 2020 202b 2028 2220             + (" 
+000249c0: 2825 2e31 6625 252c 2220 2520 7065 7263  (%.1f%%," % perc
+000249d0: 656e 7432 290a 2020 2020 2020 2020 2020  ent2).          
+000249e0: 2020 2020 2020 2b20 2822 2025 2e31 6625        + (" %.1f%
+000249f0: 2529 2220 2520 7065 7263 656e 7433 290a  %)" % percent3).
+00024a00: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00024a10: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
+00024a20: 6374 5b22 2543 686e 6722 5d20 3d20 7063  ct["%Chng"] = pc
+00024a30: 745f 6368 616e 6765 5f74 6578 740a 2020  t_change_text.  
+00024a40: 2020 2020 2020 2020 2020 7363 7265 656e            screen
+00024a50: 4469 6374 5b22 2543 686e 6722 5d20 3d20  Dict["%Chng"] = 
+00024a60: 636f 6c6f 7254 6578 742e 4752 4545 4e20  colorText.GREEN 
+00024a70: 2b20 7063 745f 6368 616e 6765 5f74 6578  + pct_change_tex
+00024a80: 7420 2b20 636f 6c6f 7254 6578 742e 454e  t + colorText.EN
+00024a90: 440a 2020 2020 2020 2020 2020 2020 7265  D.            re
+00024aa0: 7475 726e 2054 7275 6520 616e 6420 7365  turn True and se
+00024ab0: 6c66 2e67 6574 4361 6e64 6c65 5479 7065  lf.getCandleType
+00024ac0: 2864 6174 612e 6865 6164 2831 2929 0a20  (data.head(1)). 
+00024ad0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+00024ae0: 6c73 650a 0a20 2020 2023 406d 6561 7375  lse..    #@measu
+00024af0: 7265 5f74 696d 650a 2020 2020 2320 7661  re_time.    # va
+00024b00: 6c69 6461 7465 2069 6620 5253 4920 6973  lidate if RSI is
+00024b10: 2077 6974 6869 6e20 6769 7665 6e20 7261   within given ra
+00024b20: 6e67 650a 2020 2020 6465 6620 7661 6c69  nge.    def vali
+00024b30: 6461 7465 5253 4928 7365 6c66 2c20 6466  dateRSI(self, df
+00024b40: 2c20 7363 7265 656e 4469 6374 2c20 7361  , screenDict, sa
+00024b50: 7665 4469 6374 2c20 6d69 6e52 5349 2c20  veDict, minRSI, 
+00024b60: 6d61 7852 5349 2c72 7369 4b65 793d 2252  maxRSI,rsiKey="R
+00024b70: 5349 2229 3a0a 2020 2020 2020 2020 6966  SI"):.        if
+00024b80: 2064 6620 6973 204e 6f6e 6520 6f72 206c   df is None or l
+00024b90: 656e 2864 6629 203d 3d20 303a 0a20 2020  en(df) == 0:.   
+00024ba0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00024bb0: 4661 6c73 650a 2020 2020 2020 2020 6966  False.        if
+00024bc0: 2072 7369 4b65 7920 6e6f 7420 696e 2064   rsiKey not in d
+00024bd0: 662e 636f 6c75 6d6e 733a 0a20 2020 2020  f.columns:.     
+00024be0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+00024bf0: 6c73 650a 2020 2020 2020 2020 6461 7461  lse.        data
+00024c00: 203d 2064 662e 636f 7079 2829 0a20 2020   = df.copy().   
+00024c10: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
+00024c20: 2e66 696c 6c6e 6128 3029 0a20 2020 2020  .fillna(0).     
+00024c30: 2020 2064 6174 6120 3d20 6461 7461 2e72     data = data.r
+00024c40: 6570 6c61 6365 285b 6e70 2e69 6e66 2c20  eplace([np.inf, 
+00024c50: 2d6e 702e 696e 665d 2c20 3029 0a20 2020  -np.inf], 0).   
+00024c60: 2020 2020 2072 7369 203d 2069 6e74 2864       rsi = int(d
+00024c70: 6174 612e 6865 6164 2831 295b 7273 694b  ata.head(1)[rsiK
+00024c80: 6579 5d2e 696c 6f63 5b30 5d29 0a20 2020  ey].iloc[0]).   
+00024c90: 2020 2020 2073 6176 6544 6963 745b 7273       saveDict[rs
+00024ca0: 694b 6579 5d20 3d20 7273 690a 2020 2020  iKey] = rsi.    
+00024cb0: 2020 2020 2320 6874 7470 733a 2f2f 6368      # https://ch
+00024cc0: 6172 7469 6e6b 2e63 6f6d 2f73 6372 6565  artink.com/scree
+00024cd0: 6e65 722f 7273 692d 7363 7265 656e 696e  ner/rsi-screenin
+00024ce0: 670a 2020 2020 2020 2020 6966 2072 7369  g.        if rsi
+00024cf0: 3e20 3020 616e 6420 7273 6920 3e3d 206d  > 0 and rsi >= m
+00024d00: 696e 5253 4920 616e 6420 7273 6920 3c3d  inRSI and rsi <=
+00024d10: 206d 6178 5253 493a 2020 2320 6f72 2028   maxRSI:  # or (
+00024d20: 7273 6920 3c3d 2037 3120 616e 6420 7273  rsi <= 71 and rs
+00024d30: 6920 3e3d 2036 3729 3a0a 2020 2020 2020  i >= 67):.      
+00024d40: 2020 2020 2020 7363 7265 656e 4469 6374        screenDict
+00024d50: 5b72 7369 4b65 795d 203d 2028 0a20 2020  [rsiKey] = (.   
+00024d60: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
+00024d70: 6f72 5465 7874 2e42 4f4c 4420 2b20 636f  orText.BOLD + co
+00024d80: 6c6f 7254 6578 742e 4752 4545 4e20 2b20  lorText.GREEN + 
+00024d90: 7374 7228 7273 6929 202b 2063 6f6c 6f72  str(rsi) + color
+00024da0: 5465 7874 2e45 4e44 0a20 2020 2020 2020  Text.END.       
+00024db0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00024dc0: 2020 2072 6574 7572 6e20 5472 7565 2069     return True i
+00024dd0: 6620 2872 7369 4b65 7920 3d3d 2022 5253  f (rsiKey == "RS
+00024de0: 4969 2229 2065 6c73 6520 2873 656c 662e  Ii") else (self.
+00024df0: 7661 6c69 6461 7465 5253 4928 6466 2c20  validateRSI(df, 
+00024e00: 7363 7265 656e 4469 6374 2c20 7361 7665  screenDict, save
+00024e10: 4469 6374 2c20 6d69 6e52 5349 2c20 6d61  Dict, minRSI, ma
+00024e20: 7852 5349 2c72 7369 4b65 793d 2252 5349  xRSI,rsiKey="RSI
+00024e30: 6922 2920 6f72 2054 7275 6529 0a20 2020  i") or True).   
+00024e40: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
+00024e50: 7273 694b 6579 5d20 3d20 636f 6c6f 7254  rsiKey] = colorT
+00024e60: 6578 742e 424f 4c44 202b 2063 6f6c 6f72  ext.BOLD + color
+00024e70: 5465 7874 2e46 4149 4c20 2b20 7374 7228  Text.FAIL + str(
+00024e80: 7273 6929 202b 2063 6f6c 6f72 5465 7874  rsi) + colorText
+00024e90: 2e45 4e44 0a20 2020 2020 2020 2023 2049  .END.        # I
+00024ea0: 6620 6569 7468 6572 2064 6169 6c79 206f  f either daily o
+00024eb0: 7220 696e 7472 6164 6179 2052 5349 2063  r intraday RSI c
+00024ec0: 6f6d 6573 2077 6974 6869 6e20 7261 6e67  omes within rang
+00024ed0: 653f 0a20 2020 2020 2020 2072 6574 7572  e?.        retur
+00024ee0: 6e20 4661 6c73 6520 6966 2028 7273 694b  n False if (rsiK
+00024ef0: 6579 203d 3d20 2252 5349 6922 2920 656c  ey == "RSIi") el
+00024f00: 7365 2028 7365 6c66 2e76 616c 6964 6174  se (self.validat
+00024f10: 6552 5349 2864 662c 2073 6372 6565 6e44  eRSI(df, screenD
+00024f20: 6963 742c 2073 6176 6544 6963 742c 206d  ict, saveDict, m
+00024f30: 696e 5253 492c 206d 6178 5253 492c 7273  inRSI, maxRSI,rs
+00024f40: 694b 6579 3d22 5253 4969 2229 290a 0a20  iKey="RSIi")).. 
+00024f50: 2020 2023 2056 616c 6964 6174 6520 6966     # Validate if
+00024f60: 2074 6865 2073 746f 636b 2069 7320 6275   the stock is bu
+00024f70: 6c6c 6973 6820 696e 2074 6865 2073 686f  llish in the sho
+00024f80: 7274 2074 6572 6d0a 2020 2020 6465 6620  rt term.    def 
+00024f90: 7661 6c69 6461 7465 5368 6f72 7454 6572  validateShortTer
+00024fa0: 6d42 756c 6c69 7368 2873 656c 662c 2064  mBullish(self, d
+00024fb0: 662c 2073 6372 6565 6e44 6963 742c 2073  f, screenDict, s
+00024fc0: 6176 6544 6963 7429 3a0a 2020 2020 2020  aveDict):.      
+00024fd0: 2020 6966 2064 6620 6973 204e 6f6e 6520    if df is None 
+00024fe0: 6f72 206c 656e 2864 6629 203d 3d20 303a  or len(df) == 0:
+00024ff0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00025000: 7572 6e20 4661 6c73 650a 2020 2020 2020  urn False.      
+00025010: 2020 6461 7461 203d 2064 662e 636f 7079    data = df.copy
+00025020: 2829 0a20 2020 2020 2020 2023 2068 7474  ().        # htt
+00025030: 7073 3a2f 2f63 6861 7274 696e 6b2e 636f  ps://chartink.co
+00025040: 6d2f 7363 7265 656e 6572 2f73 686f 7274  m/screener/short
+00025050: 2d74 6572 6d2d 6275 6c6c 6973 680a 2020  -term-bullish.  
+00025060: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
+00025070: 612e 6669 6c6c 6e61 2830 290a 2020 2020  a.fillna(0).    
+00025080: 2020 2020 6461 7461 203d 2064 6174 612e      data = data.
+00025090: 7265 706c 6163 6528 5b6e 702e 696e 662c  replace([np.inf,
+000250a0: 202d 6e70 2e69 6e66 5d2c 2030 290a 2020   -np.inf], 0).  
+000250b0: 2020 2020 2020 7265 6365 6e74 203d 2064        recent = d
+000250c0: 6174 612e 6865 6164 2831 290a 2020 2020  ata.head(1).    
+000250d0: 2020 2020 666b 203d 2030 2069 6620 6c65      fk = 0 if le
+000250e0: 6e28 6461 7461 2920 3c20 3320 656c 7365  n(data) < 3 else
+000250f0: 206e 702e 726f 756e 6428 6461 7461 5b22   np.round(data["
+00025100: 4641 5354 4b22 5d2e 696c 6f63 5b32 5d2c  FASTK"].iloc[2],
+00025110: 2035 290a 2020 2020 2020 2020 2320 5265   5).        # Re
+00025120: 7665 7273 6520 7468 6520 6461 7461 6672  verse the datafr
+00025130: 616d 6520 666f 7220 6963 6869 6d6f 6b75  ame for ichimoku
+00025140: 2063 616c 6375 6c61 7469 6f6e 7320 7769   calculations wi
+00025150: 7468 2064 6174 6520 696e 2061 7363 656e  th date in ascen
+00025160: 6469 6e67 206f 7264 6572 0a20 2020 2020  ding order.     
+00025170: 2020 2064 665f 6e65 7720 3d20 6461 7461     df_new = data
+00025180: 5b3a 3a2d 315d 0a20 2020 2020 2020 2074  [::-1].        t
+00025190: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+000251a0: 6466 5f69 6368 6920 3d20 6466 5f6e 6577  df_ichi = df_new
+000251b0: 2e72 656e 616d 6528 0a20 2020 2020 2020  .rename(.       
+000251c0: 2020 2020 2020 2020 2063 6f6c 756d 6e73           columns
+000251d0: 3d7b 0a20 2020 2020 2020 2020 2020 2020  ={.             
+000251e0: 2020 2020 2020 2022 4f70 656e 223a 2022         "Open": "
+000251f0: 6f70 656e 222c 0a20 2020 2020 2020 2020  open",.         
+00025200: 2020 2020 2020 2020 2020 2022 4869 6768             "High
+00025210: 223a 2022 6869 6768 222c 0a20 2020 2020  ": "high",.     
+00025220: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00025230: 4c6f 7722 3a20 226c 6f77 222c 0a20 2020  Low": "low",.   
+00025240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025250: 2022 436c 6f73 6522 3a20 2263 6c6f 7365   "Close": "close
+00025260: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00025270: 2020 2020 2020 2022 566f 6c75 6d65 223a         "Volume":
+00025280: 2022 766f 6c75 6d65 222c 0a20 2020 2020   "volume",.     
+00025290: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+000252a0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+000252b0: 2020 2020 2020 2069 6368 6920 3d20 706b         ichi = pk
+000252c0: 7461 6c69 622e 6963 6869 6d6f 6b75 2864  talib.ichimoku(d
+000252d0: 665f 6963 6869 2c20 392c 2032 362c 2035  f_ichi, 9, 26, 5
+000252e0: 322c 2032 3629 0a20 2020 2020 2020 2020  2, 26).         
+000252f0: 2020 2069 6620 6963 6869 2069 7320 4e6f     if ichi is No
+00025300: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00025310: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+00025320: 0a20 2020 2020 2020 2020 2020 2064 665f  .            df_
+00025330: 6e65 7720 3d20 7064 2e63 6f6e 6361 7428  new = pd.concat(
+00025340: 5b64 665f 6e65 772c 2069 6368 695d 2c20  [df_new, ichi], 
+00025350: 6178 6973 3d31 290a 2020 2020 2020 2020  axis=1).        
+00025360: 2020 2020 2320 5265 7665 7273 6520 6167      # Reverse ag
+00025370: 6169 6e20 746f 2067 6574 2074 6865 206d  ain to get the m
+00025380: 6f73 7420 7265 6365 6e74 2064 6174 6520  ost recent date 
+00025390: 6f6e 2074 6f70 0a20 2020 2020 2020 2020  on top.         
+000253a0: 2020 2064 665f 6e65 7720 3d20 6466 5f6e     df_new = df_n
+000253b0: 6577 5b3a 3a2d 315d 0a20 2020 2020 2020  ew[::-1].       
+000253c0: 2020 2020 2064 665f 6e65 7720 3d20 6466       df_new = df
+000253d0: 5f6e 6577 2e68 6561 6428 3129 0a20 2020  _new.head(1).   
+000253e0: 2020 2020 2020 2020 2064 665f 6e65 775b           df_new[
+000253f0: 2263 6c6f 7564 5f67 7265 656e 225d 203d  "cloud_green"] =
+00025400: 2064 665f 6e65 775b 2249 5341 5f39 225d   df_new["ISA_9"]
+00025410: 2e69 6c6f 635b 305d 203e 2064 665f 6e65  .iloc[0] > df_ne
+00025420: 775b 2249 5342 5f32 3622 5d2e 696c 6f63  w["ISB_26"].iloc
+00025430: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
+00025440: 6466 5f6e 6577 5b22 636c 6f75 645f 7265  df_new["cloud_re
+00025450: 6422 5d20 3d20 6466 5f6e 6577 5b22 4953  d"] = df_new["IS
+00025460: 425f 3236 225d 2e69 6c6f 635b 305d 203e  B_26"].iloc[0] >
+00025470: 2064 665f 6e65 775b 2249 5341 5f39 225d   df_new["ISA_9"]
+00025480: 2e69 6c6f 635b 305d 0a20 2020 2020 2020  .iloc[0].       
+00025490: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+000254a0: 6e20 6173 2065 3a20 2023 2070 7261 676d  n as e:  # pragm
+000254b0: 613a 206e 6f20 636f 7665 720a 2020 2020  a: no cover.    
+000254c0: 2020 2020 2020 2020 7365 6c66 2e64 6566          self.def
+000254d0: 6175 6c74 5f6c 6f67 6765 722e 6465 6275  ault_logger.debu
+000254e0: 6728 652c 2065 7863 5f69 6e66 6f3d 5472  g(e, exc_info=Tr
+000254f0: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
+00025500: 7061 7373 0a20 2020 2020 2020 2061 626f  pass.        abo
+00025510: 7665 436c 6f75 6454 6f70 203d 2046 616c  veCloudTop = Fal
+00025520: 7365 0a20 2020 2020 2020 2023 2062 6173  se.        # bas
+00025530: 656c 696e 6520 3e20 636c 6f75 6420 746f  eline > cloud to
+00025540: 7020 2863 6c6f 7564 2069 7320 626f 756e  p (cloud is boun
+00025550: 6420 6279 2073 7061 6e20 6120 616e 6420  d by span a and 
+00025560: 7370 616e 2062 2920 616e 6420 636c 6f73  span b) and clos
+00025570: 6520 6973 203e 2063 6c6f 7564 2074 6f70  e is > cloud top
+00025580: 0a20 2020 2020 2020 2069 6620 6466 5f6e  .        if df_n
+00025590: 6577 5b22 636c 6f75 645f 6772 6565 6e22  ew["cloud_green"
+000255a0: 5d2e 696c 6f63 5b30 5d3a 0a20 2020 2020  ].iloc[0]:.     
+000255b0: 2020 2020 2020 2061 626f 7665 436c 6f75         aboveClou
+000255c0: 6454 6f70 203d 2028 0a20 2020 2020 2020  dTop = (.       
+000255d0: 2020 2020 2020 2020 2064 665f 6e65 775b           df_new[
+000255e0: 2249 4b53 5f32 3622 5d2e 696c 6f63 5b30  "IKS_26"].iloc[0
+000255f0: 5d20 3e20 6466 5f6e 6577 5b22 4953 415f  ] > df_new["ISA_
+00025600: 3922 5d2e 696c 6f63 5b30 5d0a 2020 2020  9"].iloc[0].    
+00025610: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+00025620: 7265 6365 6e74 5b22 436c 6f73 6522 5d2e  recent["Close"].
+00025630: 696c 6f63 5b30 5d20 3e20 6466 5f6e 6577  iloc[0] > df_new
+00025640: 5b22 4953 415f 3922 5d2e 696c 6f63 5b30  ["ISA_9"].iloc[0
+00025650: 5d0a 2020 2020 2020 2020 2020 2020 290a  ].            ).
+00025660: 2020 2020 2020 2020 656c 6966 2064 665f          elif df_
+00025670: 6e65 775b 2263 6c6f 7564 5f72 6564 225d  new["cloud_red"]
+00025680: 2e69 6c6f 635b 305d 3a0a 2020 2020 2020  .iloc[0]:.      
+00025690: 2020 2020 2020 6162 6f76 6543 6c6f 7564        aboveCloud
+000256a0: 546f 7020 3d20 280a 2020 2020 2020 2020  Top = (.        
+000256b0: 2020 2020 2020 2020 6466 5f6e 6577 5b22          df_new["
+000256c0: 494b 535f 3236 225d 2e69 6c6f 635b 305d  IKS_26"].iloc[0]
+000256d0: 203e 2064 665f 6e65 775b 2249 5342 5f32   > df_new["ISB_2
+000256e0: 3622 5d2e 696c 6f63 5b30 5d0a 2020 2020  6"].iloc[0].    
+000256f0: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+00025700: 7265 6365 6e74 5b22 436c 6f73 6522 5d2e  recent["Close"].
+00025710: 696c 6f63 5b30 5d20 3e20 6466 5f6e 6577  iloc[0] > df_new
+00025720: 5b22 4953 425f 3236 225d 2e69 6c6f 635b  ["ISB_26"].iloc[
+00025730: 305d 0a20 2020 2020 2020 2020 2020 2029  0].            )
+00025740: 0a0a 2020 2020 2020 2020 2320 4c61 7465  ..        # Late
+00025750: 7374 2049 6368 696d 6f6b 7520 6261 7365  st Ichimoku base
+00025760: 6c69 6e65 2069 7320 3c20 6c61 7465 7374  line is < latest
+00025770: 2049 6368 696d 6f6b 7520 636f 6e76 6572   Ichimoku conver
+00025780: 7369 6f6e 206c 696e 650a 2020 2020 2020  sion line.      
+00025790: 2020 6966 2061 626f 7665 436c 6f75 6454    if aboveCloudT
+000257a0: 6f70 2061 6e64 2064 665f 6e65 775b 2249  op and df_new["I
+000257b0: 4b53 5f32 3622 5d2e 696c 6f63 5b30 5d20  KS_26"].iloc[0] 
+000257c0: 3c20 6466 5f6e 6577 5b22 4954 535f 3922  < df_new["ITS_9"
+000257d0: 5d2e 696c 6f63 5b30 5d3a 0a20 2020 2020  ].iloc[0]:.     
+000257e0: 2020 2020 2020 2023 2053 746f 6368 5253         # StochRS
+000257f0: 4920 6372 6f73 7365 6420 3230 2061 6e64  I crossed 20 and
+00025800: 2052 5349 203e 2035 300a 2020 2020 2020   RSI > 50.      
+00025810: 2020 2020 2020 6966 2066 6b20 3e20 3230        if fk > 20
+00025820: 2061 6e64 2072 6563 656e 745b 2252 5349   and recent["RSI
+00025830: 225d 2e69 6c6f 635b 305d 203e 2035 303a  "].iloc[0] > 50:
+00025840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00025850: 2023 2063 6f6e 6469 7469 6f6e 206f 6620   # condition of 
+00025860: 6372 6f73 7369 6e67 2074 6865 2053 746f  crossing the Sto
+00025870: 6368 5253 4920 6d61 696e 2073 6967 6e61  chRSI main signa
+00025880: 6c20 6c69 6e65 2066 726f 6d20 626f 7474  l line from bott
+00025890: 6f6d 2074 6f20 746f 700a 2020 2020 2020  om to top.      
+000258a0: 2020 2020 2020 2020 2020 6966 2028 0a20            if (. 
+000258b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000258c0: 2020 2064 6174 615b 2246 4153 5444 225d     data["FASTD"]
+000258d0: 2e69 6c6f 635b 3130 305d 203c 2064 6174  .iloc[100] < dat
+000258e0: 615b 2246 4153 544b 225d 2e69 6c6f 635b  a["FASTK"].iloc[
+000258f0: 3130 305d 0a20 2020 2020 2020 2020 2020  100].           
+00025900: 2020 2020 2020 2020 2061 6e64 2064 6174           and dat
+00025910: 615b 2246 4153 5444 225d 2e69 6c6f 635b  a["FASTD"].iloc[
+00025920: 3130 315d 203e 2064 6174 615b 2246 4153  101] > data["FAS
+00025930: 544b 225d 2e69 6c6f 635b 3130 315d 0a20  TK"].iloc[101]. 
+00025940: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00025950: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00025960: 2020 2020 2020 2320 636c 6f73 6520 3e20        # close > 
+00025970: 3530 2070 6572 696f 6420 534d 412f 454d  50 period SMA/EM
+00025980: 4120 616e 6420 3230 3020 7065 7269 6f64  A and 200 period
+00025990: 2053 4d41 2f45 4d41 0a20 2020 2020 2020   SMA/EMA.       
+000259a0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000259b0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000259c0: 2020 2020 2020 2020 2020 7265 6365 6e74            recent
+000259d0: 5b22 5353 4d41 225d 2e69 6c6f 635b 305d  ["SSMA"].iloc[0]
+000259e0: 203e 2072 6563 656e 745b 2253 4d41 225d   > recent["SMA"]
+000259f0: 2e69 6c6f 635b 305d 0a20 2020 2020 2020  .iloc[0].       
+00025a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025a10: 2061 6e64 2072 6563 656e 745b 2243 6c6f   and recent["Clo
+00025a20: 7365 225d 2e69 6c6f 635b 305d 203e 2072  se"].iloc[0] > r
+00025a30: 6563 656e 745b 2253 534d 4122 5d2e 696c  ecent["SSMA"].il
+00025a40: 6f63 5b30 5d0a 2020 2020 2020 2020 2020  oc[0].          
+00025a50: 2020 2020 2020 2020 2020 2020 2020 616e                an
+00025a60: 6420 7265 6365 6e74 5b22 436c 6f73 6522  d recent["Close"
+00025a70: 5d2e 696c 6f63 5b30 5d20 3e20 7265 6365  ].iloc[0] > rece
+00025a80: 6e74 5b22 4c4d 4122 5d2e 696c 6f63 5b30  nt["LMA"].iloc[0
+00025a90: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00025aa0: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
 00025ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025ac0: 7363 7265 656e 4469 6374 5b22 4d41 2d53  screenDict["MA-S
-00025ad0: 6967 6e61 6c22 5d20 3d20 280a 2020 2020  ignal"] = (.    
-00025ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025af0: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
-00025b00: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
-00025b10: 4420 2b20 636f 6c6f 7254 6578 742e 4752  D + colorText.GR
-00025b20: 4545 4e20 2b20 2242 756c 6c69 7368 2220  EEN + "Bullish" 
-00025b30: 2b20 636f 6c6f 7254 6578 742e 454e 440a  + colorText.END.
+00025ac0: 2073 6176 6564 203d 2073 656c 662e 6669   saved = self.fi
+00025ad0: 6e64 4375 7272 656e 7453 6176 6564 5661  ndCurrentSavedVa
+00025ae0: 6c75 6528 7363 7265 656e 4469 6374 2c73  lue(screenDict,s
+00025af0: 6176 6544 6963 742c 224d 412d 5369 676e  aveDict,"MA-Sign
+00025b00: 616c 2229 0a20 2020 2020 2020 2020 2020  al").           
+00025b10: 2020 2020 2020 2020 2020 2020 2073 6372               scr
+00025b20: 6565 6e44 6963 745b 224d 412d 5369 676e  eenDict["MA-Sign
+00025b30: 616c 225d 203d 2028 0a20 2020 2020 2020  al"] = (.       
 00025b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025b50: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00025b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025b70: 2020 7361 7665 4469 6374 5b22 4d41 2d53    saveDict["MA-S
-00025b80: 6967 6e61 6c22 5d20 3d20 7361 7665 645b  ignal"] = saved[
-00025b90: 315d 202b 2022 4275 6c6c 6973 6822 0a20  1] + "Bullish". 
+00025b50: 2020 2020 2073 6176 6564 5b30 5d20 2b20       saved[0] + 
+00025b60: 636f 6c6f 7254 6578 742e 424f 4c44 202b  colorText.BOLD +
+00025b70: 2063 6f6c 6f72 5465 7874 2e47 5245 454e   colorText.GREEN
+00025b80: 202b 2022 4275 6c6c 6973 6822 202b 2063   + "Bullish" + c
+00025b90: 6f6c 6f72 5465 7874 2e45 4e44 0a20 2020  olorText.END.   
 00025ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025bb0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-00025bc0: 7565 0a20 2020 2020 2020 2072 6574 7572  ue.        retur
-00025bd0: 6e20 4661 6c73 650a 2020 2020 0a20 2020  n False.    .   
-00025be0: 2023 2056 616c 6964 6174 6520 5643 5020   # Validate VCP 
-00025bf0: 6173 2070 6572 204d 6172 6b20 4d69 6e65  as per Mark Mine
-00025c00: 7276 696e 690a 2020 2020 2320 6874 7470  rvini.    # http
-00025c10: 733a 2f2f 6368 6172 7469 6e6b 2e63 6f6d  s://chartink.com
-00025c20: 2f73 6372 6565 6e65 722f 766f 6c61 7469  /screener/volati
-00025c30: 6c69 7479 2d63 6f6d 7072 6573 7369 6f6e  lity-compression
-00025c40: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-00025c50: 6556 4350 4d61 726b 4d69 6e65 7276 696e  eVCPMarkMinervin
-00025c60: 6928 7365 6c66 2c20 6466 3a70 642e 4461  i(self, df:pd.Da
-00025c70: 7461 4672 616d 652c 2073 6372 6565 6e44  taFrame, screenD
-00025c80: 6963 742c 2073 6176 6544 6963 7429 3a0a  ict, saveDict):.
-00025c90: 2020 2020 2020 2020 6966 2064 6620 6973          if df is
-00025ca0: 204e 6f6e 6520 6f72 206c 656e 2864 6629   None or len(df)
-00025cb0: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
-00025cc0: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-00025cd0: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
-00025ce0: 662e 636f 7079 2829 0a20 2020 2020 2020  f.copy().       
-00025cf0: 206f 686c 635f 6469 6374 203d 207b 0a20   ohlc_dict = {. 
-00025d00: 2020 2020 2020 2020 2020 2027 4f70 656e             'Open
-00025d10: 273a 2766 6972 7374 272c 0a20 2020 2020  ':'first',.     
-00025d20: 2020 2020 2020 2027 4869 6768 273a 276d         'High':'m
-00025d30: 6178 272c 0a20 2020 2020 2020 2020 2020  ax',.           
-00025d40: 2027 4c6f 7727 3a27 6d69 6e27 2c0a 2020   'Low':'min',.  
-00025d50: 2020 2020 2020 2020 2020 2743 6c6f 7365            'Close
-00025d60: 273a 276c 6173 7427 2c0a 2020 2020 2020  ':'last',.      
-00025d70: 2020 2020 2020 2756 6f6c 756d 6527 3a27        'Volume':'
-00025d80: 7375 6d27 0a20 2020 2020 2020 207d 0a20  sum'.        }. 
-00025d90: 2020 2020 2020 2023 2066 696e 616c 5f64         # final_d
-00025da0: 6620 3d20 6466 2e72 6573 616d 706c 6528  f = df.resample(
-00025db0: 2757 2d46 5249 272c 2063 6c6f 7365 643d  'W-FRI', closed=
-00025dc0: 276c 6566 7427 292e 6167 6728 6f68 6c63  'left').agg(ohlc
-00025dd0: 5f64 6963 7429 2e73 6869 6674 2827 3164  _dict).shift('1d
-00025de0: 2729 0a20 2020 2020 2020 2077 6565 6b6c  ').        weekl
-00025df0: 7944 6174 6120 3d20 6461 7461 2e72 6573  yData = data.res
-00025e00: 616d 706c 6528 2757 2729 2e61 6767 286f  ample('W').agg(o
-00025e10: 686c 635f 6469 6374 290a 2020 2020 2020  hlc_dict).      
-00025e20: 2020 7265 7665 7273 6564 4461 7461 203d    reversedData =
-00025e30: 2064 6174 615b 3a3a 2d31 5d20 2023 2052   data[::-1]  # R
-00025e40: 6576 6572 7365 2074 6865 2064 6174 6166  everse the dataf
-00025e50: 7261 6d65 0a20 2020 2020 2020 2072 6563  rame.        rec
-00025e60: 656e 745f 636c 6f73 6520 3d20 6461 7461  ent_close = data
-00025e70: 5b22 436c 6f73 6522 5d2e 6865 6164 2831  ["Close"].head(1
-00025e80: 292e 696c 6f63 5b30 5d0a 2020 2020 2020  ).iloc[0].      
-00025e90: 2020 775f 656d 615f 3133 203d 2070 6b74    w_ema_13 = pkt
-00025ea0: 616c 6962 2e45 4d41 2877 6565 6b6c 7944  alib.EMA(weeklyD
-00025eb0: 6174 615b 2243 6c6f 7365 225d 2c74 696d  ata["Close"],tim
-00025ec0: 6570 6572 696f 643d 3133 292e 7461 696c  eperiod=13).tail
-00025ed0: 2831 292e 696c 6f63 5b30 5d0a 2020 2020  (1).iloc[0].    
-00025ee0: 2020 2020 775f 656d 615f 3236 203d 2070      w_ema_26 = p
-00025ef0: 6b74 616c 6962 2e45 4d41 2877 6565 6b6c  ktalib.EMA(weekl
-00025f00: 7944 6174 615b 2243 6c6f 7365 225d 2c74  yData["Close"],t
-00025f10: 696d 6570 6572 696f 643d 3236 292e 7461  imeperiod=26).ta
-00025f20: 696c 2831 292e 696c 6f63 5b30 5d0a 2020  il(1).iloc[0].  
-00025f30: 2020 2020 2020 775f 736d 615f 3530 203d        w_sma_50 =
-00025f40: 2070 6b74 616c 6962 2e53 4d41 2877 6565   pktalib.SMA(wee
-00025f50: 6b6c 7944 6174 615b 2243 6c6f 7365 225d  klyData["Close"]
-00025f60: 2c74 696d 6570 6572 696f 643d 3530 292e  ,timeperiod=50).
-00025f70: 7461 696c 2831 292e 696c 6f63 5b30 5d0a  tail(1).iloc[0].
-00025f80: 2020 2020 2020 2020 775f 736d 615f 3430          w_sma_40
-00025f90: 203d 2070 6b74 616c 6962 2e53 4d41 2877   = pktalib.SMA(w
-00025fa0: 6565 6b6c 7944 6174 615b 2243 6c6f 7365  eeklyData["Close
-00025fb0: 225d 2c74 696d 6570 6572 696f 643d 3430  "],timeperiod=40
-00025fc0: 292e 7461 696c 2831 292e 696c 6f63 5b30  ).tail(1).iloc[0
-00025fd0: 5d0a 2020 2020 2020 2020 775f 736d 615f  ].        w_sma_
-00025fe0: 3430 5f35 775f 6167 6f20 3d20 706b 7461  40_5w_ago = pkta
-00025ff0: 6c69 622e 534d 4128 7765 656b 6c79 4461  lib.SMA(weeklyDa
-00026000: 7461 2e68 6561 6428 6c65 6e28 7765 656b  ta.head(len(week
-00026010: 6c79 4461 7461 292d 3529 5b22 436c 6f73  lyData)-5)["Clos
-00026020: 6522 5d2c 7469 6d65 7065 7269 6f64 3d34  e"],timeperiod=4
-00026030: 3029 2e74 6169 6c28 3129 2e69 6c6f 635b  0).tail(1).iloc[
-00026040: 305d 0a20 2020 2020 2020 2077 5f6d 696e  0].        w_min
-00026050: 5f35 3020 3d20 6d69 6e28 312e 332a 7765  _50 = min(1.3*we
-00026060: 656b 6c79 4461 7461 2e74 6169 6c28 3530  eklyData.tail(50
-00026070: 295b 224c 6f77 225d 290a 2020 2020 2020  )["Low"]).      
-00026080: 2020 775f 6d61 785f 3530 203d 206d 6178    w_max_50 = max
-00026090: 2830 2e37 352a 7765 656b 6c79 4461 7461  (0.75*weeklyData
-000260a0: 2e74 6169 6c28 3530 295b 2248 6967 6822  .tail(50)["High"
-000260b0: 5d29 0a20 2020 2020 2020 2077 5f65 6d61  ]).        w_ema
-000260c0: 5f32 365f 3230 775f 6167 6f20 3d20 706b  _26_20w_ago = pk
-000260d0: 7461 6c69 622e 454d 4128 7765 656b 6c79  talib.EMA(weekly
-000260e0: 4461 7461 2e68 6561 6428 6c65 6e28 7765  Data.head(len(we
-000260f0: 656b 6c79 4461 7461 292d 3230 295b 2243  eklyData)-20)["C
-00026100: 6c6f 7365 225d 2c74 696d 6570 6572 696f  lose"],timeperio
-00026110: 643d 3236 292e 7461 696c 2831 292e 696c  d=26).tail(1).il
-00026120: 6f63 5b30 5d0a 2020 2020 2020 2020 7265  oc[0].        re
-00026130: 6365 6e74 5f65 6d61 5f31 335f 3230 645f  cent_ema_13_20d_
-00026140: 6167 6f20 3d20 706b 7461 6c69 622e 454d  ago = pktalib.EM
-00026150: 4128 7265 7665 7273 6564 4461 7461 2e68  A(reversedData.h
-00026160: 6561 6428 6c65 6e28 7265 7665 7273 6564  ead(len(reversed
-00026170: 4461 7461 292d 3230 295b 2243 6c6f 7365  Data)-20)["Close
-00026180: 225d 2c74 696d 6570 6572 696f 643d 3133  "],timeperiod=13
-00026190: 292e 7461 696c 2831 292e 696c 6f63 5b30  ).tail(1).iloc[0
-000261a0: 5d0a 2020 2020 2020 2020 775f 736d 615f  ].        w_sma_
-000261b0: 3430 5f35 775f 6167 6f20 3d20 706b 7461  40_5w_ago = pkta
-000261c0: 6c69 622e 534d 4128 7765 656b 6c79 4461  lib.SMA(weeklyDa
-000261d0: 7461 2e68 6561 6428 6c65 6e28 7765 656b  ta.head(len(week
-000261e0: 6c79 4461 7461 292d 3529 5b22 436c 6f73  lyData)-5)["Clos
-000261f0: 6522 5d2c 7469 6d65 7065 7269 6f64 3d34  e"],timeperiod=4
-00026200: 3029 2e74 6169 6c28 3129 2e69 6c6f 635b  0).tail(1).iloc[
-00026210: 305d 0a20 2020 2020 2020 2077 5f73 6d61  0].        w_sma
-00026220: 5f34 305f 3130 775f 6167 6f20 3d20 706b  _40_10w_ago = pk
-00026230: 7461 6c69 622e 534d 4128 7765 656b 6c79  talib.SMA(weekly
-00026240: 4461 7461 2e68 6561 6428 6c65 6e28 7765  Data.head(len(we
-00026250: 656b 6c79 4461 7461 292d 3130 295b 2243  eklyData)-10)["C
-00026260: 6c6f 7365 225d 2c74 696d 6570 6572 696f  lose"],timeperio
-00026270: 643d 3430 292e 7461 696c 2831 292e 696c  d=40).tail(1).il
-00026280: 6f63 5b30 5d0a 2020 2020 2020 2020 7265  oc[0].        re
-00026290: 6365 6e74 5f73 6d61 5f35 3020 3d20 706b  cent_sma_50 = pk
-000262a0: 7461 6c69 622e 534d 4128 7265 7665 7273  talib.SMA(revers
-000262b0: 6564 4461 7461 5b22 436c 6f73 6522 5d2c  edData["Close"],
-000262c0: 7469 6d65 7065 7269 6f64 3d35 3029 2e74  timeperiod=50).t
-000262d0: 6169 6c28 3129 2e69 6c6f 635b 305d 0a20  ail(1).iloc[0]. 
-000262e0: 2020 2020 2020 2077 5f77 6d61 5f38 203d         w_wma_8 =
-000262f0: 2070 6b74 616c 6962 2e57 4d41 2877 6565   pktalib.WMA(wee
-00026300: 6b6c 7944 6174 615b 2243 6c6f 7365 225d  klyData["Close"]
-00026310: 2c74 696d 6570 6572 696f 643d 3829 2e74  ,timeperiod=8).t
-00026320: 6169 6c28 3129 2e69 6c6f 635b 305d 0a20  ail(1).iloc[0]. 
-00026330: 2020 2020 2020 2077 5f73 6d61 5f38 203d         w_sma_8 =
-00026340: 2070 6b74 616c 6962 2e53 4d41 2877 6565   pktalib.SMA(wee
-00026350: 6b6c 7944 6174 615b 2243 6c6f 7365 225d  klyData["Close"]
-00026360: 2c74 696d 6570 6572 696f 643d 3829 2e74  ,timeperiod=8).t
-00026370: 6169 6c28 3129 2e69 6c6f 635b 305d 0a20  ail(1).iloc[0]. 
-00026380: 2020 2020 2020 206e 756d 5072 6576 696f         numPrevio
-00026390: 7573 4361 6e64 6c65 7320 3d20 3230 0a20  usCandles = 20. 
-000263a0: 2020 2020 2020 2070 756c 6c62 6163 6b44         pullbackD
-000263b0: 6174 6120 3d20 6461 7461 2e68 6561 6428  ata = data.head(
-000263c0: 6e75 6d50 7265 7669 6f75 7343 616e 646c  numPreviousCandl
-000263d0: 6573 290a 2020 2020 2020 2020 7075 6c6c  es).        pull
-000263e0: 6261 636b 4461 7461 2e6c 6f63 5b3a 2c27  backData.loc[:,'
-000263f0: 5075 6c6c 4261 636b 275d 203d 2070 756c  PullBack'] = pul
-00026400: 6c62 6163 6b44 6174 615b 2243 6c6f 7365  lbackData["Close
-00026410: 225d 2e6c 7428 7075 6c6c 6261 636b 4461  "].lt(pullbackDa
-00026420: 7461 5b22 4f70 656e 225d 2920 232e 7368  ta["Open"]) #.sh
-00026430: 6966 7428 7065 7269 6f64 733d 3129 2920  ift(periods=1)) 
-00026440: 2326 2064 6174 615b 224c 6f77 225d 2e6c  #& data["Low"].l
-00026450: 7428 6461 7461 5b22 4c6f 7722 5d2e 7368  t(data["Low"].sh
-00026460: 6966 7428 7065 7269 6f64 733d 3129 290a  ift(periods=1)).
-00026470: 2020 2020 2020 2020 7368 7269 6e6b 6564          shrinked
-00026480: 566f 6c44 6174 6120 3d20 7075 6c6c 6261  VolData = pullba
-00026490: 636b 4461 7461 5b70 756c 6c62 6163 6b44  ckData[pullbackD
-000264a0: 6174 615b 2250 756c 6c42 6163 6b22 5d20  ata["PullBack"] 
-000264b0: 3d3d 2054 7275 655d 2e68 6561 6428 6e75  == True].head(nu
-000264c0: 6d50 7265 7669 6f75 7343 616e 646c 6573  mPreviousCandles
-000264d0: 290a 2020 2020 2020 2020 7265 6365 6e74  ).        recent
-000264e0: 4c61 7267 6573 7456 6f6c 756d 6520 3d20  LargestVolume = 
-000264f0: 6d61 7828 7075 6c6c 6261 636b 4461 7461  max(pullbackData
-00026500: 5b70 756c 6c62 6163 6b44 6174 615b 2250  [pullbackData["P
-00026510: 756c 6c42 6163 6b22 5d20 3d3d 2046 616c  ullBack"] == Fal
-00026520: 7365 5d2e 6865 6164 2833 295b 2256 6f6c  se].head(3)["Vol
-00026530: 756d 6522 5d29 0a20 2020 2020 2020 2023  ume"]).        #
-00026540: 2070 756c 6c62 6163 6b44 6174 612e 6c6f   pullbackData.lo
-00026550: 635b 3a2c 2750 4256 6f6c 5261 7469 6f27  c[:,'PBVolRatio'
-00026560: 5d20 3d20 7075 6c6c 6261 636b 4461 7461  ] = pullbackData
-00026570: 5b22 566f 6c75 6d65 225d 2f72 6563 656e  ["Volume"]/recen
-00026580: 744c 6172 6765 7374 566f 6c75 6d65 0a20  tLargestVolume. 
-00026590: 2020 2020 2020 2076 6f6c 496e 5072 6576         volInPrev
-000265a0: 696f 7573 5075 6c6c 6261 636b 7353 6872  iousPullbacksShr
-000265b0: 696e 6b65 6420 3d20 4661 6c73 650a 2020  inked = False.  
-000265c0: 2020 2020 2020 6966 206e 6f74 2073 6872        if not shr
-000265d0: 696e 6b65 6456 6f6c 4461 7461 2e65 6d70  inkedVolData.emp
-000265e0: 7479 3a0a 2020 2020 2020 2020 2020 2020  ty:.            
-000265f0: 696e 6465 7820 3d20 300a 2020 2020 2020  index = 0.      
-00026600: 2020 2020 2020 7768 696c 6520 696e 6465        while inde
-00026610: 7820 3c20 6c65 6e28 7368 7269 6e6b 6564  x < len(shrinked
-00026620: 566f 6c44 6174 6129 3a0a 2020 2020 2020  VolData):.      
-00026630: 2020 2020 2020 2020 2020 766f 6c49 6e50            volInP
-00026640: 7265 7669 6f75 7350 756c 6c62 6163 6b73  reviousPullbacks
-00026650: 5368 7269 6e6b 6564 203d 2073 6872 696e  Shrinked = shrin
-00026660: 6b65 6456 6f6c 4461 7461 5b22 566f 6c75  kedVolData["Volu
-00026670: 6d65 225d 2e69 6c6f 635b 696e 6465 785d  me"].iloc[index]
-00026680: 203c 2073 656c 662e 636f 6e66 6967 4d61   < self.configMa
-00026690: 6e61 6765 722e 7663 7056 6f6c 756d 6543  nager.vcpVolumeC
-000266a0: 6f6e 7472 6163 7469 6f6e 5261 7469 6f20  ontractionRatio 
-000266b0: 2a20 7265 6365 6e74 4c61 7267 6573 7456  * recentLargestV
-000266c0: 6f6c 756d 650a 2020 2020 2020 2020 2020  olume.          
-000266d0: 2020 2020 2020 6966 206e 6f74 2076 6f6c        if not vol
-000266e0: 496e 5072 6576 696f 7573 5075 6c6c 6261  InPreviousPullba
-000266f0: 636b 7353 6872 696e 6b65 643a 0a20 2020  cksShrinked:.   
-00026700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026710: 2062 7265 616b 0a20 2020 2020 2020 2020   break.         
-00026720: 2020 2020 2020 2069 6e64 6578 202b 3d20         index += 
-00026730: 310a 2020 2020 2020 2020 7265 6365 6e74  1.        recent
-00026740: 566f 6c75 6d65 4861 7341 626f 7665 4176  VolumeHasAboveAv
-00026750: 6756 6f6c 203d 2072 6563 656e 744c 6172  gVol = recentLar
-00026760: 6765 7374 566f 6c75 6d65 203e 3d20 7365  gestVolume >= se
-00026770: 6c66 2e63 6f6e 6669 674d 616e 6167 6572  lf.configManager
-00026780: 2e76 6f6c 756d 6552 6174 696f 202a 2064  .volumeRatio * d
-00026790: 6174 615b 2256 6f6c 4d41 225d 2e69 6c6f  ata["VolMA"].ilo
-000267a0: 635b 305d 0a20 2020 2020 2020 2069 7356  c[0].        isV
-000267b0: 4350 203d 2077 5f65 6d61 5f31 3320 3e20  CP = w_ema_13 > 
-000267c0: 775f 656d 615f 3236 2061 6e64 205c 0a20  w_ema_26 and \. 
-000267d0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-000267e0: 5f65 6d61 5f32 3620 3e20 775f 736d 615f  _ema_26 > w_sma_
-000267f0: 3530 2061 6e64 205c 0a20 2020 2020 2020  50 and \.       
-00026800: 2020 2020 2020 2020 2077 5f73 6d61 5f34           w_sma_4
-00026810: 3020 3e20 775f 736d 615f 3430 5f35 775f  0 > w_sma_40_5w_
-00026820: 6167 6f20 616e 6420 5c0a 2020 2020 2020  ago and \.      
-00026830: 2020 2020 2020 2020 2020 7265 6365 6e74            recent
-00026840: 5f63 6c6f 7365 203e 3d20 775f 6d69 6e5f  _close >= w_min_
-00026850: 3530 2061 6e64 205c 0a20 2020 2020 2020  50 and \.       
-00026860: 2020 2020 2020 2020 2072 6563 656e 745f           recent_
-00026870: 636c 6f73 6520 3e3d 2077 5f6d 6178 5f35  close >= w_max_5
-00026880: 3020 616e 6420 5c0a 2020 2020 2020 2020  0 and \.        
-00026890: 2020 2020 2020 2020 7265 6365 6e74 5f65          recent_e
-000268a0: 6d61 5f31 335f 3230 645f 6167 6f20 3e20  ma_13_20d_ago > 
-000268b0: 775f 656d 615f 3236 5f32 3077 5f61 676f  w_ema_26_20w_ago
-000268c0: 2061 6e64 205c 0a20 2020 2020 2020 2020   and \.         
-000268d0: 2020 2020 2020 2077 5f73 6d61 5f34 305f         w_sma_40_
-000268e0: 3577 5f61 676f 203e 2077 5f73 6d61 5f34  5w_ago > w_sma_4
-000268f0: 305f 3130 775f 6167 6f20 616e 6420 5c0a  0_10w_ago and \.
-00026900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026910: 7265 6365 6e74 5f63 6c6f 7365 203e 2072  recent_close > r
-00026920: 6563 656e 745f 736d 615f 3530 2061 6e64  ecent_sma_50 and
-00026930: 205c 0a20 2020 2020 2020 2020 2020 2020   \.             
-00026940: 2020 2028 775f 776d 615f 3820 2d20 775f     (w_wma_8 - w_
-00026950: 736d 615f 3829 2a36 2f32 3920 3c20 302e  sma_8)*6/29 < 0.
-00026960: 3520 616e 6420 5c0a 2020 2020 2020 2020  5 and \.        
-00026970: 2020 2020 2020 2020 766f 6c49 6e50 7265          volInPre
-00026980: 7669 6f75 7350 756c 6c62 6163 6b73 5368  viousPullbacksSh
-00026990: 7269 6e6b 6564 2061 6e64 205c 0a20 2020  rinked and \.   
-000269a0: 2020 2020 2020 2020 2020 2020 2072 6563               rec
-000269b0: 656e 7456 6f6c 756d 6548 6173 4162 6f76  entVolumeHasAbov
-000269c0: 6541 7667 566f 6c20 616e 6420 5c0a 2020  eAvgVol and \.  
-000269d0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000269e0: 6365 6e74 5f63 6c6f 7365 203e 2031 300a  cent_close > 10.
-000269f0: 2020 2020 2020 2020 6966 2069 7356 4350          if isVCP
-00026a00: 3a0a 2020 2020 2020 2020 2020 2020 7361  :.            sa
-00026a10: 7665 6420 3d20 7365 6c66 2e66 696e 6443  ved = self.findC
-00026a20: 7572 7265 6e74 5361 7665 6456 616c 7565  urrentSavedValue
-00026a30: 2873 6372 6565 6e44 6963 742c 2073 6176  (screenDict, sav
-00026a40: 6544 6963 742c 2022 5061 7474 6572 6e22  eDict, "Pattern"
-00026a50: 290a 2020 2020 2020 2020 2020 2020 7363  ).            sc
-00026a60: 7265 656e 4469 6374 5b22 5061 7474 6572  reenDict["Patter
-00026a70: 6e22 5d20 3d20 280a 2020 2020 2020 2020  n"] = (.        
-00026a80: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
-00026a90: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-00026aa0: 2020 2b20 636f 6c6f 7254 6578 742e 424f    + colorText.BO
-00026ab0: 4c44 0a20 2020 2020 2020 2020 2020 2020  LD.             
-00026ac0: 2020 202b 2063 6f6c 6f72 5465 7874 2e47     + colorText.G
-00026ad0: 5245 454e 0a20 2020 2020 2020 2020 2020  REEN.           
-00026ae0: 2020 2020 202b 2066 2256 4350 284d 696e       + f"VCP(Min
-00026af0: 6572 7669 6e69 2922 0a20 2020 2020 2020  ervini)".       
-00026b00: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
-00026b10: 5465 7874 2e45 4e44 0a20 2020 2020 2020  Text.END.       
-00026b20: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00026b30: 2020 2073 6176 6544 6963 745b 2250 6174     saveDict["Pat
-00026b40: 7465 726e 225d 203d 2073 6176 6564 5b31  tern"] = saved[1
-00026b50: 5d20 2b20 6622 5643 5028 4d69 6e65 7276  ] + f"VCP(Minerv
-00026b60: 696e 6929 220a 2020 2020 2020 2020 7265  ini)".        re
-00026b70: 7475 726e 2069 7356 4350 0a20 2020 200a  turn isVCP.    .
-00026b80: 2020 2020 2320 5661 6c69 6461 7465 2056      # Validate V
-00026b90: 4350 0a20 2020 2064 6566 2076 616c 6964  CP.    def valid
-00026ba0: 6174 6556 4350 280a 2020 2020 2020 2020  ateVCP(.        
-00026bb0: 7365 6c66 2c20 6466 2c20 7363 7265 656e  self, df, screen
-00026bc0: 4469 6374 2c20 7361 7665 4469 6374 2c20  Dict, saveDict, 
-00026bd0: 7374 6f63 6b4e 616d 653d 4e6f 6e65 2c20  stockName=None, 
-00026be0: 7769 6e64 6f77 3d33 2c20 7065 7263 656e  window=3, percen
-00026bf0: 7461 6765 4672 6f6d 546f 703d 330a 2020  tageFromTop=3.  
-00026c00: 2020 293a 0a20 2020 2020 2020 2069 6620    ):.        if 
-00026c10: 6466 2069 7320 4e6f 6e65 206f 7220 6c65  df is None or le
-00026c20: 6e28 6466 2920 3d3d 2030 3a0a 2020 2020  n(df) == 0:.    
-00026c30: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-00026c40: 616c 7365 0a20 2020 2020 2020 2064 6174  alse.        dat
-00026c50: 6120 3d20 6466 2e63 6f70 7928 290a 2020  a = df.copy().  
-00026c60: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-00026c70: 2020 2020 2020 2070 6572 6365 6e74 6167         percentag
-00026c80: 6546 726f 6d54 6f70 202f 3d20 3130 300a  eFromTop /= 100.
-00026c90: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00026ca0: 2e72 6573 6574 5f69 6e64 6578 2869 6e70  .reset_index(inp
-00026cb0: 6c61 6365 3d54 7275 6529 0a20 2020 2020  lace=True).     
-00026cc0: 2020 2020 2020 2064 6174 612e 7265 6e61         data.rena
-00026cd0: 6d65 2863 6f6c 756d 6e73 3d7b 2269 6e64  me(columns={"ind
-00026ce0: 6578 223a 2022 4461 7465 227d 2c20 696e  ex": "Date"}, in
-00026cf0: 706c 6163 653d 5472 7565 290a 2020 2020  place=True).    
-00026d00: 2020 2020 2020 2020 6461 7461 5b22 746f          data["to
-00026d10: 7073 225d 203d 2028 6461 7461 5b22 4869  ps"] = (data["Hi
-00026d20: 6768 225d 2e69 6c6f 635b 6c69 7374 2870  gh"].iloc[list(p
-00026d30: 6b74 616c 6962 2e61 7267 7265 6c65 7874  ktalib.argrelext
-00026d40: 7265 6d61 286e 702e 6172 7261 7928 6461  rema(np.array(da
-00026d50: 7461 5b22 4869 6768 225d 292c 206e 702e  ta["High"]), np.
-00026d60: 6772 6561 7465 725f 6571 7561 6c2c 206f  greater_equal, o
-00026d70: 7264 6572 3d77 696e 646f 7729 5b30 5d29  rder=window)[0])
-00026d80: 5d2e 6865 6164 2834 2929 0a20 2020 2020  ].head(4)).     
-00026d90: 2020 2020 2020 2064 6174 615b 2262 6f74         data["bot
-00026da0: 7322 5d20 3d20 2864 6174 615b 224c 6f77  s"] = (data["Low
-00026db0: 225d 2e69 6c6f 635b 6c69 7374 2870 6b74  "].iloc[list(pkt
-00026dc0: 616c 6962 2e61 7267 7265 6c65 7874 7265  alib.argrelextre
-00026dd0: 6d61 286e 702e 6172 7261 7928 6461 7461  ma(np.array(data
-00026de0: 5b22 4c6f 7722 5d29 2c20 6e70 2e6c 6573  ["Low"]), np.les
-00026df0: 735f 6571 7561 6c2c 206f 7264 6572 3d77  s_equal, order=w
-00026e00: 696e 646f 7729 5b30 5d29 5d2e 6865 6164  indow)[0])].head
-00026e10: 2834 2929 0a20 2020 2020 2020 2020 2020  (4)).           
-00026e20: 2064 6174 6120 3d20 6461 7461 2e66 696c   data = data.fil
-00026e30: 6c6e 6128 3029 0a20 2020 2020 2020 2020  lna(0).         
-00026e40: 2020 2064 6174 6120 3d20 6461 7461 2e72     data = data.r
-00026e50: 6570 6c61 6365 285b 6e70 2e69 6e66 2c20  eplace([np.inf, 
-00026e60: 2d6e 702e 696e 665d 2c20 3029 0a20 2020  -np.inf], 0).   
-00026e70: 2020 2020 2020 2020 2074 6f70 7320 3d20           tops = 
-00026e80: 6461 7461 5b64 6174 612e 746f 7073 203e  data[data.tops >
-00026e90: 2030 5d0a 2020 2020 2020 2020 2020 2020   0].            
-00026ea0: 2320 626f 7473 203d 2064 6174 615b 6461  # bots = data[da
-00026eb0: 7461 2e62 6f74 7320 3e20 305d 0a20 2020  ta.bots > 0].   
-00026ec0: 2020 2020 2020 2020 2068 6967 6865 7374           highest
-00026ed0: 546f 7020 3d20 726f 756e 6428 746f 7073  Top = round(tops
-00026ee0: 2e64 6573 6372 6962 6528 295b 2248 6967  .describe()["Hig
-00026ef0: 6822 5d5b 226d 6178 225d 2c20 3129 0a20  h"]["max"], 1). 
-00026f00: 2020 2020 2020 2020 2020 2066 696c 7465             filte
-00026f10: 7265 6454 6f70 7320 3d20 746f 7073 5b0a  redTops = tops[.
-00026f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026f30: 746f 7073 2e74 6f70 7320 3e20 2868 6967  tops.tops > (hig
-00026f40: 6865 7374 546f 7020 2d20 2868 6967 6865  hestTop - (highe
-00026f50: 7374 546f 7020 2a20 7065 7263 656e 7461  stTop * percenta
-00026f60: 6765 4672 6f6d 546f 7029 290a 2020 2020  geFromTop)).    
-00026f70: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
-00026f80: 2020 2020 2020 6966 2066 696c 7465 7265        if filtere
-00026f90: 6454 6f70 732e 6571 7561 6c73 2874 6f70  dTops.equals(top
-00026fa0: 7329 3a20 2023 2054 6f70 7320 6172 6520  s):  # Tops are 
-00026fb0: 696e 2074 6865 2072 616e 6765 0a20 2020  in the range.   
-00026fc0: 2020 2020 2020 2020 2020 2020 206c 6f77               low
-00026fd0: 506f 696e 7473 203d 205b 5d0a 2020 2020  Points = [].    
-00026fe0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00026ff0: 6920 696e 2072 616e 6765 286c 656e 2874  i in range(len(t
-00027000: 6f70 7329 202d 2031 293a 0a20 2020 2020  ops) - 1):.     
-00027010: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00027020: 6e64 4461 7465 203d 2074 6f70 732e 696c  ndDate = tops.il
-00027030: 6f63 5b69 5d5b 2244 6174 6522 5d0a 2020  oc[i]["Date"].  
-00027040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027050: 2020 7374 6172 7444 6174 6520 3d20 746f    startDate = to
-00027060: 7073 2e69 6c6f 635b 6920 2b20 315d 5b22  ps.iloc[i + 1]["
-00027070: 4461 7465 225d 0a20 2020 2020 2020 2020  Date"].         
-00027080: 2020 2020 2020 2020 2020 206c 6f77 506f             lowPo
-00027090: 696e 7473 2e61 7070 656e 6428 0a20 2020  ints.append(.   
-000270a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000270b0: 2020 2020 2064 6174 615b 0a20 2020 2020       data[.     
-000270c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000270d0: 2020 2020 2020 2028 6461 7461 2e44 6174         (data.Dat
-000270e0: 6520 3e3d 2073 7461 7274 4461 7465 2920  e >= startDate) 
-000270f0: 2620 2864 6174 612e 4461 7465 203c 3d20  & (data.Date <= 
-00027100: 656e 6444 6174 6529 0a20 2020 2020 2020  endDate).       
-00027110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027120: 205d 2e64 6573 6372 6962 6528 295b 224c   ].describe()["L
-00027130: 6f77 225d 5b22 6d69 6e22 5d0a 2020 2020  ow"]["min"].    
-00027140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027150: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00027160: 2020 6c6f 7750 6f69 6e74 734f 7267 203d    lowPointsOrg =
-00027170: 206c 6f77 506f 696e 7473 0a20 2020 2020   lowPoints.     
-00027180: 2020 2020 2020 2020 2020 206c 6f77 506f             lowPo
-00027190: 696e 7473 2e73 6f72 7428 7265 7665 7273  ints.sort(revers
-000271a0: 653d 5472 7565 290a 2020 2020 2020 2020  e=True).        
-000271b0: 2020 2020 2020 2020 6c6f 7750 6f69 6e74          lowPoint
-000271c0: 7353 6f72 7465 6420 3d20 6c6f 7750 6f69  sSorted = lowPoi
-000271d0: 6e74 730a 2020 2020 2020 2020 2020 2020  nts.            
-000271e0: 2020 2020 6966 2064 6174 612e 656d 7074      if data.empt
-000271f0: 7920 6f72 206c 656e 286c 6f77 506f 696e  y or len(lowPoin
-00027200: 7473 2920 3c20 313a 0a20 2020 2020 2020  ts) < 1:.       
-00027210: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00027220: 7572 6e20 4661 6c73 650a 2020 2020 2020  urn False.      
-00027230: 2020 2020 2020 2020 2020 6c74 7020 3d20            ltp = 
-00027240: 6461 7461 2e68 6561 6428 3129 5b22 436c  data.head(1)["Cl
-00027250: 6f73 6522 5d2e 696c 6f63 5b30 5d0a 2020  ose"].iloc[0].  
-00027260: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00027270: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
-00027280: 2020 2020 2020 206c 6f77 506f 696e 7473         lowPoints
-00027290: 4f72 6720 3d3d 206c 6f77 506f 696e 7473  Org == lowPoints
-000272a0: 536f 7274 6564 0a20 2020 2020 2020 2020  Sorted.         
-000272b0: 2020 2020 2020 2020 2020 2061 6e64 206c             and l
-000272c0: 7470 203c 2068 6967 6865 7374 546f 700a  tp < highestTop.
+00025bb0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00025bc0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00025bd0: 6176 6544 6963 745b 224d 412d 5369 676e  aveDict["MA-Sign
+00025be0: 616c 225d 203d 2073 6176 6564 5b31 5d20  al"] = saved[1] 
+00025bf0: 2b20 2242 756c 6c69 7368 220a 2020 2020  + "Bullish".    
+00025c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025c10: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+00025c20: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+00025c30: 616c 7365 0a20 2020 200a 2020 2020 2320  alse.    .    # 
+00025c40: 5661 6c69 6461 7465 2056 4350 2061 7320  Validate VCP as 
+00025c50: 7065 7220 4d61 726b 204d 696e 6572 7669  per Mark Minervi
+00025c60: 6e69 0a20 2020 2023 2068 7474 7073 3a2f  ni.    # https:/
+00025c70: 2f63 6861 7274 696e 6b2e 636f 6d2f 7363  /chartink.com/sc
+00025c80: 7265 656e 6572 2f76 6f6c 6174 696c 6974  reener/volatilit
+00025c90: 792d 636f 6d70 7265 7373 696f 6e0a 2020  y-compression.  
+00025ca0: 2020 6465 6620 7661 6c69 6461 7465 5643    def validateVC
+00025cb0: 504d 6172 6b4d 696e 6572 7669 6e69 2873  PMarkMinervini(s
+00025cc0: 656c 662c 2064 663a 7064 2e44 6174 6146  elf, df:pd.DataF
+00025cd0: 7261 6d65 2c20 7363 7265 656e 4469 6374  rame, screenDict
+00025ce0: 2c20 7361 7665 4469 6374 293a 0a20 2020  , saveDict):.   
+00025cf0: 2020 2020 2069 6620 6466 2069 7320 4e6f       if df is No
+00025d00: 6e65 206f 7220 6c65 6e28 6466 2920 3d3d  ne or len(df) ==
+00025d10: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+00025d20: 7265 7475 726e 2046 616c 7365 0a20 2020  return False.   
+00025d30: 2020 2020 2064 6174 6120 3d20 6466 2e63       data = df.c
+00025d40: 6f70 7928 290a 2020 2020 2020 2020 6f68  opy().        oh
+00025d50: 6c63 5f64 6963 7420 3d20 7b0a 2020 2020  lc_dict = {.    
+00025d60: 2020 2020 2020 2020 274f 7065 6e27 3a27          'Open':'
+00025d70: 6669 7273 7427 2c0a 2020 2020 2020 2020  first',.        
+00025d80: 2020 2020 2748 6967 6827 3a27 6d61 7827      'High':'max'
+00025d90: 2c0a 2020 2020 2020 2020 2020 2020 274c  ,.            'L
+00025da0: 6f77 273a 276d 696e 272c 0a20 2020 2020  ow':'min',.     
+00025db0: 2020 2020 2020 2027 436c 6f73 6527 3a27         'Close':'
+00025dc0: 6c61 7374 272c 0a20 2020 2020 2020 2020  last',.         
+00025dd0: 2020 2027 566f 6c75 6d65 273a 2773 756d     'Volume':'sum
+00025de0: 270a 2020 2020 2020 2020 7d0a 2020 2020  '.        }.    
+00025df0: 2020 2020 2320 6669 6e61 6c5f 6466 203d      # final_df =
+00025e00: 2064 662e 7265 7361 6d70 6c65 2827 572d   df.resample('W-
+00025e10: 4652 4927 2c20 636c 6f73 6564 3d27 6c65  FRI', closed='le
+00025e20: 6674 2729 2e61 6767 286f 686c 635f 6469  ft').agg(ohlc_di
+00025e30: 6374 292e 7368 6966 7428 2731 6427 290a  ct).shift('1d').
+00025e40: 2020 2020 2020 2020 7765 656b 6c79 4461          weeklyDa
+00025e50: 7461 203d 2064 6174 612e 7265 7361 6d70  ta = data.resamp
+00025e60: 6c65 2827 5727 292e 6167 6728 6f68 6c63  le('W').agg(ohlc
+00025e70: 5f64 6963 7429 0a20 2020 2020 2020 2072  _dict).        r
+00025e80: 6576 6572 7365 6444 6174 6120 3d20 6461  eversedData = da
+00025e90: 7461 5b3a 3a2d 315d 2020 2320 5265 7665  ta[::-1]  # Reve
+00025ea0: 7273 6520 7468 6520 6461 7461 6672 616d  rse the datafram
+00025eb0: 650a 2020 2020 2020 2020 7265 6365 6e74  e.        recent
+00025ec0: 5f63 6c6f 7365 203d 2064 6174 615b 2243  _close = data["C
+00025ed0: 6c6f 7365 225d 2e68 6561 6428 3129 2e69  lose"].head(1).i
+00025ee0: 6c6f 635b 305d 0a20 2020 2020 2020 2077  loc[0].        w
+00025ef0: 5f65 6d61 5f31 3320 3d20 706b 7461 6c69  _ema_13 = pktali
+00025f00: 622e 454d 4128 7765 656b 6c79 4461 7461  b.EMA(weeklyData
+00025f10: 5b22 436c 6f73 6522 5d2c 7469 6d65 7065  ["Close"],timepe
+00025f20: 7269 6f64 3d31 3329 2e74 6169 6c28 3129  riod=13).tail(1)
+00025f30: 2e69 6c6f 635b 305d 0a20 2020 2020 2020  .iloc[0].       
+00025f40: 2077 5f65 6d61 5f32 3620 3d20 706b 7461   w_ema_26 = pkta
+00025f50: 6c69 622e 454d 4128 7765 656b 6c79 4461  lib.EMA(weeklyDa
+00025f60: 7461 5b22 436c 6f73 6522 5d2c 7469 6d65  ta["Close"],time
+00025f70: 7065 7269 6f64 3d32 3629 2e74 6169 6c28  period=26).tail(
+00025f80: 3129 2e69 6c6f 635b 305d 0a20 2020 2020  1).iloc[0].     
+00025f90: 2020 2077 5f73 6d61 5f35 3020 3d20 706b     w_sma_50 = pk
+00025fa0: 7461 6c69 622e 534d 4128 7765 656b 6c79  talib.SMA(weekly
+00025fb0: 4461 7461 5b22 436c 6f73 6522 5d2c 7469  Data["Close"],ti
+00025fc0: 6d65 7065 7269 6f64 3d35 3029 2e74 6169  meperiod=50).tai
+00025fd0: 6c28 3129 2e69 6c6f 635b 305d 0a20 2020  l(1).iloc[0].   
+00025fe0: 2020 2020 2077 5f73 6d61 5f34 3020 3d20       w_sma_40 = 
+00025ff0: 706b 7461 6c69 622e 534d 4128 7765 656b  pktalib.SMA(week
+00026000: 6c79 4461 7461 5b22 436c 6f73 6522 5d2c  lyData["Close"],
+00026010: 7469 6d65 7065 7269 6f64 3d34 3029 2e74  timeperiod=40).t
+00026020: 6169 6c28 3129 2e69 6c6f 635b 305d 0a20  ail(1).iloc[0]. 
+00026030: 2020 2020 2020 2077 5f73 6d61 5f34 305f         w_sma_40_
+00026040: 3577 5f61 676f 203d 2070 6b74 616c 6962  5w_ago = pktalib
+00026050: 2e53 4d41 2877 6565 6b6c 7944 6174 612e  .SMA(weeklyData.
+00026060: 6865 6164 286c 656e 2877 6565 6b6c 7944  head(len(weeklyD
+00026070: 6174 6129 2d35 295b 2243 6c6f 7365 225d  ata)-5)["Close"]
+00026080: 2c74 696d 6570 6572 696f 643d 3430 292e  ,timeperiod=40).
+00026090: 7461 696c 2831 292e 696c 6f63 5b30 5d0a  tail(1).iloc[0].
+000260a0: 2020 2020 2020 2020 775f 6d69 6e5f 3530          w_min_50
+000260b0: 203d 206d 696e 2831 2e33 2a77 6565 6b6c   = min(1.3*weekl
+000260c0: 7944 6174 612e 7461 696c 2835 3029 5b22  yData.tail(50)["
+000260d0: 4c6f 7722 5d29 0a20 2020 2020 2020 2077  Low"]).        w
+000260e0: 5f6d 6178 5f35 3020 3d20 6d61 7828 302e  _max_50 = max(0.
+000260f0: 3735 2a77 6565 6b6c 7944 6174 612e 7461  75*weeklyData.ta
+00026100: 696c 2835 3029 5b22 4869 6768 225d 290a  il(50)["High"]).
+00026110: 2020 2020 2020 2020 775f 656d 615f 3236          w_ema_26
+00026120: 5f32 3077 5f61 676f 203d 2070 6b74 616c  _20w_ago = pktal
+00026130: 6962 2e45 4d41 2877 6565 6b6c 7944 6174  ib.EMA(weeklyDat
+00026140: 612e 6865 6164 286c 656e 2877 6565 6b6c  a.head(len(weekl
+00026150: 7944 6174 6129 2d32 3029 5b22 436c 6f73  yData)-20)["Clos
+00026160: 6522 5d2c 7469 6d65 7065 7269 6f64 3d32  e"],timeperiod=2
+00026170: 3629 2e74 6169 6c28 3129 2e69 6c6f 635b  6).tail(1).iloc[
+00026180: 305d 0a20 2020 2020 2020 2072 6563 656e  0].        recen
+00026190: 745f 656d 615f 3133 5f32 3064 5f61 676f  t_ema_13_20d_ago
+000261a0: 203d 2070 6b74 616c 6962 2e45 4d41 2872   = pktalib.EMA(r
+000261b0: 6576 6572 7365 6444 6174 612e 6865 6164  eversedData.head
+000261c0: 286c 656e 2872 6576 6572 7365 6444 6174  (len(reversedDat
+000261d0: 6129 2d32 3029 5b22 436c 6f73 6522 5d2c  a)-20)["Close"],
+000261e0: 7469 6d65 7065 7269 6f64 3d31 3329 2e74  timeperiod=13).t
+000261f0: 6169 6c28 3129 2e69 6c6f 635b 305d 0a20  ail(1).iloc[0]. 
+00026200: 2020 2020 2020 2077 5f73 6d61 5f34 305f         w_sma_40_
+00026210: 3577 5f61 676f 203d 2070 6b74 616c 6962  5w_ago = pktalib
+00026220: 2e53 4d41 2877 6565 6b6c 7944 6174 612e  .SMA(weeklyData.
+00026230: 6865 6164 286c 656e 2877 6565 6b6c 7944  head(len(weeklyD
+00026240: 6174 6129 2d35 295b 2243 6c6f 7365 225d  ata)-5)["Close"]
+00026250: 2c74 696d 6570 6572 696f 643d 3430 292e  ,timeperiod=40).
+00026260: 7461 696c 2831 292e 696c 6f63 5b30 5d0a  tail(1).iloc[0].
+00026270: 2020 2020 2020 2020 775f 736d 615f 3430          w_sma_40
+00026280: 5f31 3077 5f61 676f 203d 2070 6b74 616c  _10w_ago = pktal
+00026290: 6962 2e53 4d41 2877 6565 6b6c 7944 6174  ib.SMA(weeklyDat
+000262a0: 612e 6865 6164 286c 656e 2877 6565 6b6c  a.head(len(weekl
+000262b0: 7944 6174 6129 2d31 3029 5b22 436c 6f73  yData)-10)["Clos
+000262c0: 6522 5d2c 7469 6d65 7065 7269 6f64 3d34  e"],timeperiod=4
+000262d0: 3029 2e74 6169 6c28 3129 2e69 6c6f 635b  0).tail(1).iloc[
+000262e0: 305d 0a20 2020 2020 2020 2072 6563 656e  0].        recen
+000262f0: 745f 736d 615f 3530 203d 2070 6b74 616c  t_sma_50 = pktal
+00026300: 6962 2e53 4d41 2872 6576 6572 7365 6444  ib.SMA(reversedD
+00026310: 6174 615b 2243 6c6f 7365 225d 2c74 696d  ata["Close"],tim
+00026320: 6570 6572 696f 643d 3530 292e 7461 696c  eperiod=50).tail
+00026330: 2831 292e 696c 6f63 5b30 5d0a 2020 2020  (1).iloc[0].    
+00026340: 2020 2020 775f 776d 615f 3820 3d20 706b      w_wma_8 = pk
+00026350: 7461 6c69 622e 574d 4128 7765 656b 6c79  talib.WMA(weekly
+00026360: 4461 7461 5b22 436c 6f73 6522 5d2c 7469  Data["Close"],ti
+00026370: 6d65 7065 7269 6f64 3d38 292e 7461 696c  meperiod=8).tail
+00026380: 2831 292e 696c 6f63 5b30 5d0a 2020 2020  (1).iloc[0].    
+00026390: 2020 2020 775f 736d 615f 3820 3d20 706b      w_sma_8 = pk
+000263a0: 7461 6c69 622e 534d 4128 7765 656b 6c79  talib.SMA(weekly
+000263b0: 4461 7461 5b22 436c 6f73 6522 5d2c 7469  Data["Close"],ti
+000263c0: 6d65 7065 7269 6f64 3d38 292e 7461 696c  meperiod=8).tail
+000263d0: 2831 292e 696c 6f63 5b30 5d0a 2020 2020  (1).iloc[0].    
+000263e0: 2020 2020 6e75 6d50 7265 7669 6f75 7343      numPreviousC
+000263f0: 616e 646c 6573 203d 2032 300a 2020 2020  andles = 20.    
+00026400: 2020 2020 7075 6c6c 6261 636b 4461 7461      pullbackData
+00026410: 203d 2064 6174 612e 6865 6164 286e 756d   = data.head(num
+00026420: 5072 6576 696f 7573 4361 6e64 6c65 7329  PreviousCandles)
+00026430: 0a20 2020 2020 2020 2070 756c 6c62 6163  .        pullbac
+00026440: 6b44 6174 612e 6c6f 635b 3a2c 2750 756c  kData.loc[:,'Pul
+00026450: 6c42 6163 6b27 5d20 3d20 7075 6c6c 6261  lBack'] = pullba
+00026460: 636b 4461 7461 5b22 436c 6f73 6522 5d2e  ckData["Close"].
+00026470: 6c74 2870 756c 6c62 6163 6b44 6174 615b  lt(pullbackData[
+00026480: 224f 7065 6e22 5d29 2023 2e73 6869 6674  "Open"]) #.shift
+00026490: 2870 6572 696f 6473 3d31 2929 2023 2620  (periods=1)) #& 
+000264a0: 6461 7461 5b22 4c6f 7722 5d2e 6c74 2864  data["Low"].lt(d
+000264b0: 6174 615b 224c 6f77 225d 2e73 6869 6674  ata["Low"].shift
+000264c0: 2870 6572 696f 6473 3d31 2929 0a20 2020  (periods=1)).   
+000264d0: 2020 2020 2073 6872 696e 6b65 6456 6f6c       shrinkedVol
+000264e0: 4461 7461 203d 2070 756c 6c62 6163 6b44  Data = pullbackD
+000264f0: 6174 615b 7075 6c6c 6261 636b 4461 7461  ata[pullbackData
+00026500: 5b22 5075 6c6c 4261 636b 225d 203d 3d20  ["PullBack"] == 
+00026510: 5472 7565 5d2e 6865 6164 286e 756d 5072  True].head(numPr
+00026520: 6576 696f 7573 4361 6e64 6c65 7329 0a20  eviousCandles). 
+00026530: 2020 2020 2020 2072 6563 656e 744c 6172         recentLar
+00026540: 6765 7374 566f 6c75 6d65 203d 206d 6178  gestVolume = max
+00026550: 2870 756c 6c62 6163 6b44 6174 615b 7075  (pullbackData[pu
+00026560: 6c6c 6261 636b 4461 7461 5b22 5075 6c6c  llbackData["Pull
+00026570: 4261 636b 225d 203d 3d20 4661 6c73 655d  Back"] == False]
+00026580: 2e68 6561 6428 3329 5b22 566f 6c75 6d65  .head(3)["Volume
+00026590: 225d 290a 2020 2020 2020 2020 2320 7075  "]).        # pu
+000265a0: 6c6c 6261 636b 4461 7461 2e6c 6f63 5b3a  llbackData.loc[:
+000265b0: 2c27 5042 566f 6c52 6174 696f 275d 203d  ,'PBVolRatio'] =
+000265c0: 2070 756c 6c62 6163 6b44 6174 615b 2256   pullbackData["V
+000265d0: 6f6c 756d 6522 5d2f 7265 6365 6e74 4c61  olume"]/recentLa
+000265e0: 7267 6573 7456 6f6c 756d 650a 2020 2020  rgestVolume.    
+000265f0: 2020 2020 766f 6c49 6e50 7265 7669 6f75      volInPreviou
+00026600: 7350 756c 6c62 6163 6b73 5368 7269 6e6b  sPullbacksShrink
+00026610: 6564 203d 2046 616c 7365 0a20 2020 2020  ed = False.     
+00026620: 2020 2069 6620 6e6f 7420 7368 7269 6e6b     if not shrink
+00026630: 6564 566f 6c44 6174 612e 656d 7074 793a  edVolData.empty:
+00026640: 0a20 2020 2020 2020 2020 2020 2069 6e64  .            ind
+00026650: 6578 203d 2030 0a20 2020 2020 2020 2020  ex = 0.         
+00026660: 2020 2077 6869 6c65 2069 6e64 6578 203c     while index <
+00026670: 206c 656e 2873 6872 696e 6b65 6456 6f6c   len(shrinkedVol
+00026680: 4461 7461 293a 0a20 2020 2020 2020 2020  Data):.         
+00026690: 2020 2020 2020 2076 6f6c 496e 5072 6576         volInPrev
+000266a0: 696f 7573 5075 6c6c 6261 636b 7353 6872  iousPullbacksShr
+000266b0: 696e 6b65 6420 3d20 7368 7269 6e6b 6564  inked = shrinked
+000266c0: 566f 6c44 6174 615b 2256 6f6c 756d 6522  VolData["Volume"
+000266d0: 5d2e 696c 6f63 5b69 6e64 6578 5d20 3c20  ].iloc[index] < 
+000266e0: 7365 6c66 2e63 6f6e 6669 674d 616e 6167  self.configManag
+000266f0: 6572 2e76 6370 566f 6c75 6d65 436f 6e74  er.vcpVolumeCont
+00026700: 7261 6374 696f 6e52 6174 696f 202a 2072  ractionRatio * r
+00026710: 6563 656e 744c 6172 6765 7374 566f 6c75  ecentLargestVolu
+00026720: 6d65 0a20 2020 2020 2020 2020 2020 2020  me.             
+00026730: 2020 2069 6620 6e6f 7420 766f 6c49 6e50     if not volInP
+00026740: 7265 7669 6f75 7350 756c 6c62 6163 6b73  reviousPullbacks
+00026750: 5368 7269 6e6b 6564 3a0a 2020 2020 2020  Shrinked:.      
+00026760: 2020 2020 2020 2020 2020 2020 2020 6272                br
+00026770: 6561 6b0a 2020 2020 2020 2020 2020 2020  eak.            
+00026780: 2020 2020 696e 6465 7820 2b3d 2031 0a20      index += 1. 
+00026790: 2020 2020 2020 2072 6563 656e 7456 6f6c         recentVol
+000267a0: 756d 6548 6173 4162 6f76 6541 7667 566f  umeHasAboveAvgVo
+000267b0: 6c20 3d20 7265 6365 6e74 4c61 7267 6573  l = recentLarges
+000267c0: 7456 6f6c 756d 6520 3e3d 2073 656c 662e  tVolume >= self.
+000267d0: 636f 6e66 6967 4d61 6e61 6765 722e 766f  configManager.vo
+000267e0: 6c75 6d65 5261 7469 6f20 2a20 6461 7461  lumeRatio * data
+000267f0: 5b22 566f 6c4d 4122 5d2e 696c 6f63 5b30  ["VolMA"].iloc[0
+00026800: 5d0a 2020 2020 2020 2020 6973 5643 5020  ].        isVCP 
+00026810: 3d20 775f 656d 615f 3133 203e 2077 5f65  = w_ema_13 > w_e
+00026820: 6d61 5f32 3620 616e 6420 5c0a 2020 2020  ma_26 and \.    
+00026830: 2020 2020 2020 2020 2020 2020 775f 656d              w_em
+00026840: 615f 3236 203e 2077 5f73 6d61 5f35 3020  a_26 > w_sma_50 
+00026850: 616e 6420 5c0a 2020 2020 2020 2020 2020  and \.          
+00026860: 2020 2020 2020 775f 736d 615f 3430 203e        w_sma_40 >
+00026870: 2077 5f73 6d61 5f34 305f 3577 5f61 676f   w_sma_40_5w_ago
+00026880: 2061 6e64 205c 0a20 2020 2020 2020 2020   and \.         
+00026890: 2020 2020 2020 2072 6563 656e 745f 636c         recent_cl
+000268a0: 6f73 6520 3e3d 2077 5f6d 696e 5f35 3020  ose >= w_min_50 
+000268b0: 616e 6420 5c0a 2020 2020 2020 2020 2020  and \.          
+000268c0: 2020 2020 2020 7265 6365 6e74 5f63 6c6f        recent_clo
+000268d0: 7365 203e 3d20 775f 6d61 785f 3530 2061  se >= w_max_50 a
+000268e0: 6e64 205c 0a20 2020 2020 2020 2020 2020  nd \.           
+000268f0: 2020 2020 2072 6563 656e 745f 656d 615f       recent_ema_
+00026900: 3133 5f32 3064 5f61 676f 203e 2077 5f65  13_20d_ago > w_e
+00026910: 6d61 5f32 365f 3230 775f 6167 6f20 616e  ma_26_20w_ago an
+00026920: 6420 5c0a 2020 2020 2020 2020 2020 2020  d \.            
+00026930: 2020 2020 775f 736d 615f 3430 5f35 775f      w_sma_40_5w_
+00026940: 6167 6f20 3e20 775f 736d 615f 3430 5f31  ago > w_sma_40_1
+00026950: 3077 5f61 676f 2061 6e64 205c 0a20 2020  0w_ago and \.   
+00026960: 2020 2020 2020 2020 2020 2020 2072 6563               rec
+00026970: 656e 745f 636c 6f73 6520 3e20 7265 6365  ent_close > rece
+00026980: 6e74 5f73 6d61 5f35 3020 616e 6420 5c0a  nt_sma_50 and \.
+00026990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000269a0: 2877 5f77 6d61 5f38 202d 2077 5f73 6d61  (w_wma_8 - w_sma
+000269b0: 5f38 292a 362f 3239 203c 2030 2e35 2061  _8)*6/29 < 0.5 a
+000269c0: 6e64 205c 0a20 2020 2020 2020 2020 2020  nd \.           
+000269d0: 2020 2020 2076 6f6c 496e 5072 6576 696f       volInPrevio
+000269e0: 7573 5075 6c6c 6261 636b 7353 6872 696e  usPullbacksShrin
+000269f0: 6b65 6420 616e 6420 5c0a 2020 2020 2020  ked and \.      
+00026a00: 2020 2020 2020 2020 2020 7265 6365 6e74            recent
+00026a10: 566f 6c75 6d65 4861 7341 626f 7665 4176  VolumeHasAboveAv
+00026a20: 6756 6f6c 2061 6e64 205c 0a20 2020 2020  gVol and \.     
+00026a30: 2020 2020 2020 2020 2020 2072 6563 656e             recen
+00026a40: 745f 636c 6f73 6520 3e20 3130 0a20 2020  t_close > 10.   
+00026a50: 2020 2020 2069 6620 6973 5643 503a 0a20       if isVCP:. 
+00026a60: 2020 2020 2020 2020 2020 2073 6176 6564             saved
+00026a70: 203d 2073 656c 662e 6669 6e64 4375 7272   = self.findCurr
+00026a80: 656e 7453 6176 6564 5661 6c75 6528 7363  entSavedValue(sc
+00026a90: 7265 656e 4469 6374 2c20 7361 7665 4469  reenDict, saveDi
+00026aa0: 6374 2c20 2250 6174 7465 726e 2229 0a20  ct, "Pattern"). 
+00026ab0: 2020 2020 2020 2020 2020 2073 6372 6565             scree
+00026ac0: 6e44 6963 745b 2250 6174 7465 726e 225d  nDict["Pattern"]
+00026ad0: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
+00026ae0: 2020 2020 2073 6176 6564 5b30 5d20 0a20       saved[0] . 
+00026af0: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+00026b00: 2063 6f6c 6f72 5465 7874 2e42 4f4c 440a   colorText.BOLD.
+00026b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026b20: 2b20 636f 6c6f 7254 6578 742e 4752 4545  + colorText.GREE
+00026b30: 4e0a 2020 2020 2020 2020 2020 2020 2020  N.              
+00026b40: 2020 2b20 6622 5643 5028 4d69 6e65 7276    + f"VCP(Minerv
+00026b50: 696e 6929 220a 2020 2020 2020 2020 2020  ini)".          
+00026b60: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
+00026b70: 742e 454e 440a 2020 2020 2020 2020 2020  t.END.          
+00026b80: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00026b90: 7361 7665 4469 6374 5b22 5061 7474 6572  saveDict["Patter
+00026ba0: 6e22 5d20 3d20 7361 7665 645b 315d 202b  n"] = saved[1] +
+00026bb0: 2066 2256 4350 284d 696e 6572 7669 6e69   f"VCP(Minervini
+00026bc0: 2922 0a20 2020 2020 2020 2072 6574 7572  )".        retur
+00026bd0: 6e20 6973 5643 500a 2020 2020 0a20 2020  n isVCP.    .   
+00026be0: 2023 2056 616c 6964 6174 6520 5643 500a   # Validate VCP.
+00026bf0: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+00026c00: 5643 5028 0a20 2020 2020 2020 2073 656c  VCP(.        sel
+00026c10: 662c 2064 662c 2073 6372 6565 6e44 6963  f, df, screenDic
+00026c20: 742c 2073 6176 6544 6963 742c 2073 746f  t, saveDict, sto
+00026c30: 636b 4e61 6d65 3d4e 6f6e 652c 2077 696e  ckName=None, win
+00026c40: 646f 773d 332c 2070 6572 6365 6e74 6167  dow=3, percentag
+00026c50: 6546 726f 6d54 6f70 3d33 0a20 2020 2029  eFromTop=3.    )
+00026c60: 3a0a 2020 2020 2020 2020 6966 2064 6620  :.        if df 
+00026c70: 6973 204e 6f6e 6520 6f72 206c 656e 2864  is None or len(d
+00026c80: 6629 203d 3d20 303a 0a20 2020 2020 2020  f) == 0:.       
+00026c90: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00026ca0: 650a 2020 2020 2020 2020 6461 7461 203d  e.        data =
+00026cb0: 2064 662e 636f 7079 2829 0a20 2020 2020   df.copy().     
+00026cc0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+00026cd0: 2020 2020 7065 7263 656e 7461 6765 4672      percentageFr
+00026ce0: 6f6d 546f 7020 2f3d 2031 3030 0a20 2020  omTop /= 100.   
+00026cf0: 2020 2020 2020 2020 2064 6174 612e 7265           data.re
+00026d00: 7365 745f 696e 6465 7828 696e 706c 6163  set_index(inplac
+00026d10: 653d 5472 7565 290a 2020 2020 2020 2020  e=True).        
+00026d20: 2020 2020 6461 7461 2e72 656e 616d 6528      data.rename(
+00026d30: 636f 6c75 6d6e 733d 7b22 696e 6465 7822  columns={"index"
+00026d40: 3a20 2244 6174 6522 7d2c 2069 6e70 6c61  : "Date"}, inpla
+00026d50: 6365 3d54 7275 6529 0a20 2020 2020 2020  ce=True).       
+00026d60: 2020 2020 2064 6174 615b 2274 6f70 7322       data["tops"
+00026d70: 5d20 3d20 2864 6174 615b 2248 6967 6822  ] = (data["High"
+00026d80: 5d2e 696c 6f63 5b6c 6973 7428 706b 7461  ].iloc[list(pkta
+00026d90: 6c69 622e 6172 6772 656c 6578 7472 656d  lib.argrelextrem
+00026da0: 6128 6e70 2e61 7272 6179 2864 6174 615b  a(np.array(data[
+00026db0: 2248 6967 6822 5d29 2c20 6e70 2e67 7265  "High"]), np.gre
+00026dc0: 6174 6572 5f65 7175 616c 2c20 6f72 6465  ater_equal, orde
+00026dd0: 723d 7769 6e64 6f77 295b 305d 295d 2e68  r=window)[0])].h
+00026de0: 6561 6428 3429 290a 2020 2020 2020 2020  ead(4)).        
+00026df0: 2020 2020 6461 7461 5b22 626f 7473 225d      data["bots"]
+00026e00: 203d 2028 6461 7461 5b22 4c6f 7722 5d2e   = (data["Low"].
+00026e10: 696c 6f63 5b6c 6973 7428 706b 7461 6c69  iloc[list(pktali
+00026e20: 622e 6172 6772 656c 6578 7472 656d 6128  b.argrelextrema(
+00026e30: 6e70 2e61 7272 6179 2864 6174 615b 224c  np.array(data["L
+00026e40: 6f77 225d 292c 206e 702e 6c65 7373 5f65  ow"]), np.less_e
+00026e50: 7175 616c 2c20 6f72 6465 723d 7769 6e64  qual, order=wind
+00026e60: 6f77 295b 305d 295d 2e68 6561 6428 3429  ow)[0])].head(4)
+00026e70: 290a 2020 2020 2020 2020 2020 2020 6461  ).            da
+00026e80: 7461 203d 2064 6174 612e 6669 6c6c 6e61  ta = data.fillna
+00026e90: 2830 290a 2020 2020 2020 2020 2020 2020  (0).            
+00026ea0: 6461 7461 203d 2064 6174 612e 7265 706c  data = data.repl
+00026eb0: 6163 6528 5b6e 702e 696e 662c 202d 6e70  ace([np.inf, -np
+00026ec0: 2e69 6e66 5d2c 2030 290a 2020 2020 2020  .inf], 0).      
+00026ed0: 2020 2020 2020 746f 7073 203d 2064 6174        tops = dat
+00026ee0: 615b 6461 7461 2e74 6f70 7320 3e20 305d  a[data.tops > 0]
+00026ef0: 0a20 2020 2020 2020 2020 2020 2023 2062  .            # b
+00026f00: 6f74 7320 3d20 6461 7461 5b64 6174 612e  ots = data[data.
+00026f10: 626f 7473 203e 2030 5d0a 2020 2020 2020  bots > 0].      
+00026f20: 2020 2020 2020 6869 6768 6573 7454 6f70        highestTop
+00026f30: 203d 2072 6f75 6e64 2874 6f70 732e 6465   = round(tops.de
+00026f40: 7363 7269 6265 2829 5b22 4869 6768 225d  scribe()["High"]
+00026f50: 5b22 6d61 7822 5d2c 2031 290a 2020 2020  ["max"], 1).    
+00026f60: 2020 2020 2020 2020 6669 6c74 6572 6564          filtered
+00026f70: 546f 7073 203d 2074 6f70 735b 0a20 2020  Tops = tops[.   
+00026f80: 2020 2020 2020 2020 2020 2020 2074 6f70               top
+00026f90: 732e 746f 7073 203e 2028 6869 6768 6573  s.tops > (highes
+00026fa0: 7454 6f70 202d 2028 6869 6768 6573 7454  tTop - (highestT
+00026fb0: 6f70 202a 2070 6572 6365 6e74 6167 6546  op * percentageF
+00026fc0: 726f 6d54 6f70 2929 0a20 2020 2020 2020  romTop)).       
+00026fd0: 2020 2020 205d 0a20 2020 2020 2020 2020       ].         
+00026fe0: 2020 2069 6620 6669 6c74 6572 6564 546f     if filteredTo
+00026ff0: 7073 2e65 7175 616c 7328 746f 7073 293a  ps.equals(tops):
+00027000: 2020 2320 546f 7073 2061 7265 2069 6e20    # Tops are in 
+00027010: 7468 6520 7261 6e67 650a 2020 2020 2020  the range.      
+00027020: 2020 2020 2020 2020 2020 6c6f 7750 6f69            lowPoi
+00027030: 6e74 7320 3d20 5b5d 0a20 2020 2020 2020  nts = [].       
+00027040: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+00027050: 6e20 7261 6e67 6528 6c65 6e28 746f 7073  n range(len(tops
+00027060: 2920 2d20 3129 3a0a 2020 2020 2020 2020  ) - 1):.        
+00027070: 2020 2020 2020 2020 2020 2020 656e 6444              endD
+00027080: 6174 6520 3d20 746f 7073 2e69 6c6f 635b  ate = tops.iloc[
+00027090: 695d 5b22 4461 7465 225d 0a20 2020 2020  i]["Date"].     
+000270a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000270b0: 7461 7274 4461 7465 203d 2074 6f70 732e  tartDate = tops.
+000270c0: 696c 6f63 5b69 202b 2031 5d5b 2244 6174  iloc[i + 1]["Dat
+000270d0: 6522 5d0a 2020 2020 2020 2020 2020 2020  e"].            
+000270e0: 2020 2020 2020 2020 6c6f 7750 6f69 6e74          lowPoint
+000270f0: 732e 6170 7065 6e64 280a 2020 2020 2020  s.append(.      
+00027100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027110: 2020 6461 7461 5b0a 2020 2020 2020 2020    data[.        
+00027120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027130: 2020 2020 2864 6174 612e 4461 7465 203e      (data.Date >
+00027140: 3d20 7374 6172 7444 6174 6529 2026 2028  = startDate) & (
+00027150: 6461 7461 2e44 6174 6520 3c3d 2065 6e64  data.Date <= end
+00027160: 4461 7465 290a 2020 2020 2020 2020 2020  Date).          
+00027170: 2020 2020 2020 2020 2020 2020 2020 5d2e                ].
+00027180: 6465 7363 7269 6265 2829 5b22 4c6f 7722  describe()["Low"
+00027190: 5d5b 226d 696e 225d 0a20 2020 2020 2020  ]["min"].       
+000271a0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+000271b0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+000271c0: 6f77 506f 696e 7473 4f72 6720 3d20 6c6f  owPointsOrg = lo
+000271d0: 7750 6f69 6e74 730a 2020 2020 2020 2020  wPoints.        
+000271e0: 2020 2020 2020 2020 6c6f 7750 6f69 6e74          lowPoint
+000271f0: 732e 736f 7274 2872 6576 6572 7365 3d54  s.sort(reverse=T
+00027200: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
+00027210: 2020 2020 206c 6f77 506f 696e 7473 536f       lowPointsSo
+00027220: 7274 6564 203d 206c 6f77 506f 696e 7473  rted = lowPoints
+00027230: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00027240: 2069 6620 6461 7461 2e65 6d70 7479 206f   if data.empty o
+00027250: 7220 6c65 6e28 6c6f 7750 6f69 6e74 7329  r len(lowPoints)
+00027260: 203c 2031 3a0a 2020 2020 2020 2020 2020   < 1:.          
+00027270: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00027280: 2046 616c 7365 0a20 2020 2020 2020 2020   False.         
+00027290: 2020 2020 2020 206c 7470 203d 2064 6174         ltp = dat
+000272a0: 612e 6865 6164 2831 295b 2243 6c6f 7365  a.head(1)["Close
+000272b0: 225d 2e69 6c6f 635b 305d 0a20 2020 2020  "].iloc[0].     
+000272c0: 2020 2020 2020 2020 2020 2069 6620 280a             if (.
 000272d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000272e0: 2020 2020 616e 6420 6c74 7020 3e20 6c6f      and ltp > lo
-000272f0: 7750 6f69 6e74 735b 305d 0a20 2020 2020  wPoints[0].     
-00027300: 2020 2020 2020 2020 2020 2029 3a0a 2020             ):.  
-00027310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027320: 2020 7361 7665 6420 3d20 7365 6c66 2e66    saved = self.f
-00027330: 696e 6443 7572 7265 6e74 5361 7665 6456  indCurrentSavedV
-00027340: 616c 7565 2873 6372 6565 6e44 6963 742c  alue(screenDict,
-00027350: 2073 6176 6544 6963 742c 2022 5061 7474   saveDict, "Patt
-00027360: 6572 6e22 290a 2020 2020 2020 2020 2020  ern").          
-00027370: 2020 2020 2020 2020 2020 7363 7265 656e            screen
-00027380: 4469 6374 5b22 5061 7474 6572 6e22 5d20  Dict["Pattern"] 
-00027390: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-000273a0: 2020 2020 2020 2020 2020 2020 7361 7665              save
-000273b0: 645b 305d 200a 2020 2020 2020 2020 2020  d[0] .          
-000273c0: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-000273d0: 636f 6c6f 7254 6578 742e 424f 4c44 0a20  colorText.BOLD. 
-000273e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000273f0: 2020 2020 2020 202b 2063 6f6c 6f72 5465         + colorTe
-00027400: 7874 2e47 5245 454e 0a20 2020 2020 2020  xt.GREEN.       
-00027410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027420: 202b 2066 2256 4350 2028 424f 3a20 7b68   + f"VCP (BO: {h
-00027430: 6967 6865 7374 546f 707d 2922 0a20 2020  ighestTop})".   
+000272e0: 2020 2020 6c6f 7750 6f69 6e74 734f 7267      lowPointsOrg
+000272f0: 203d 3d20 6c6f 7750 6f69 6e74 7353 6f72   == lowPointsSor
+00027300: 7465 640a 2020 2020 2020 2020 2020 2020  ted.            
+00027310: 2020 2020 2020 2020 616e 6420 6c74 7020          and ltp 
+00027320: 3c20 6869 6768 6573 7454 6f70 0a20 2020  < highestTop.   
+00027330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027340: 2061 6e64 206c 7470 203e 206c 6f77 506f   and ltp > lowPo
+00027350: 696e 7473 5b30 5d0a 2020 2020 2020 2020  ints[0].        
+00027360: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
+00027370: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00027380: 6176 6564 203d 2073 656c 662e 6669 6e64  aved = self.find
+00027390: 4375 7272 656e 7453 6176 6564 5661 6c75  CurrentSavedValu
+000273a0: 6528 7363 7265 656e 4469 6374 2c20 7361  e(screenDict, sa
+000273b0: 7665 4469 6374 2c20 2250 6174 7465 726e  veDict, "Pattern
+000273c0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+000273d0: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
+000273e0: 745b 2250 6174 7465 726e 225d 203d 2028  t["Pattern"] = (
+000273f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00027400: 2020 2020 2020 2020 2073 6176 6564 5b30           saved[0
+00027410: 5d20 0a20 2020 2020 2020 2020 2020 2020  ] .             
+00027420: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
+00027430: 6f72 5465 7874 2e42 4f4c 440a 2020 2020  orText.BOLD.    
 00027440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027450: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
-00027460: 2e45 4e44 0a20 2020 2020 2020 2020 2020  .END.           
-00027470: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00027480: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00027490: 6176 6544 6963 745b 2250 6174 7465 726e  aveDict["Pattern
-000274a0: 225d 203d 2073 6176 6564 5b31 5d20 2b20  "] = saved[1] + 
-000274b0: 6622 5643 5020 2842 4f3a 207b 6869 6768  f"VCP (BO: {high
-000274c0: 6573 7454 6f70 7d29 220a 2020 2020 2020  estTop})".      
-000274d0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000274e0: 7475 726e 2054 7275 650a 2020 2020 2020  turn True.      
-000274f0: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
-00027500: 6f6e 2061 7320 653a 2020 2320 7072 6167  on as e:  # prag
-00027510: 6d61 3a20 6e6f 2063 6f76 6572 0a20 2020  ma: no cover.   
-00027520: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
-00027530: 6661 756c 745f 6c6f 6767 6572 2e64 6562  fault_logger.deb
-00027540: 7567 2865 2c20 6578 635f 696e 666f 3d54  ug(e, exc_info=T
-00027550: 7275 6529 0a20 2020 2020 2020 2072 6574  rue).        ret
-00027560: 7572 6e20 4661 6c73 650a 0a20 2020 2023  urn False..    #
-00027570: 2056 616c 6964 6174 6520 6966 2076 6f6c   Validate if vol
-00027580: 756d 6520 6f66 206c 6173 7420 6461 7920  ume of last day 
-00027590: 6973 2068 6967 6865 7220 7468 616e 2061  is higher than a
-000275a0: 7667 0a20 2020 2064 6566 2076 616c 6964  vg.    def valid
-000275b0: 6174 6556 6f6c 756d 6528 0a20 2020 2020  ateVolume(.     
-000275c0: 2020 2073 656c 662c 2064 662c 2073 6372     self, df, scr
-000275d0: 6565 6e44 6963 742c 2073 6176 6544 6963  eenDict, saveDic
-000275e0: 742c 2076 6f6c 756d 6552 6174 696f 3d32  t, volumeRatio=2
-000275f0: 2e35 2c20 6d69 6e56 6f6c 756d 653d 3130  .5, minVolume=10
-00027600: 300a 2020 2020 293a 0a20 2020 2020 2020  0.    ):.       
-00027610: 2069 6620 6466 2069 7320 4e6f 6e65 206f   if df is None o
-00027620: 7220 6c65 6e28 6466 2920 3d3d 2030 3a0a  r len(df) == 0:.
-00027630: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00027640: 726e 2046 616c 7365 2c20 4661 6c73 650a  rn False, False.
-00027650: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
-00027660: 662e 636f 7079 2829 0a20 2020 2020 2020  f.copy().       
-00027670: 2064 6174 6120 3d20 6461 7461 2e66 696c   data = data.fil
-00027680: 6c6e 6128 3029 0a20 2020 2020 2020 2064  lna(0).        d
-00027690: 6174 6120 3d20 6461 7461 2e72 6570 6c61  ata = data.repla
-000276a0: 6365 285b 6e70 2e69 6e66 2c20 2d6e 702e  ce([np.inf, -np.
-000276b0: 696e 665d 2c20 3029 0a20 2020 2020 2020  inf], 0).       
-000276c0: 2072 6563 656e 7420 3d20 6461 7461 2e68   recent = data.h
-000276d0: 6561 6428 3129 0a20 2020 2020 2020 2023  ead(1).        #
-000276e0: 2045 6974 6865 7220 7468 6520 726f 6c6c   Either the roll
-000276f0: 696e 6720 766f 6c75 6d65 206f 6620 7061  ing volume of pa
-00027700: 7374 2032 3020 7365 7373 696f 6e73 206f  st 20 sessions o
-00027710: 7220 746f 6461 7927 7320 766f 6c75 6d65  r today's volume
-00027720: 2073 686f 756c 6420 6265 203e 206d 696e   should be > min
-00027730: 2076 6f6c 756d 650a 2020 2020 2020 2020   volume.        
-00027740: 6861 734d 696e 696d 756d 566f 6c75 6d65  hasMinimumVolume
-00027750: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
-00027760: 2072 6563 656e 745b 2256 6f6c 4d41 225d   recent["VolMA"]
-00027770: 2e69 6c6f 635b 305d 203e 3d20 6d69 6e56  .iloc[0] >= minV
-00027780: 6f6c 756d 650a 2020 2020 2020 2020 2020  olume.          
-00027790: 2020 6f72 2072 6563 656e 745b 2256 6f6c    or recent["Vol
-000277a0: 756d 6522 5d2e 696c 6f63 5b30 5d20 3e3d  ume"].iloc[0] >=
-000277b0: 206d 696e 566f 6c75 6d65 0a20 2020 2020   minVolume.     
-000277c0: 2020 2029 0a20 2020 2020 2020 2069 6620     ).        if 
-000277d0: 7265 6365 6e74 5b22 566f 6c4d 4122 5d2e  recent["VolMA"].
-000277e0: 696c 6f63 5b30 5d20 3d3d 2030 3a20 2023  iloc[0] == 0:  #
-000277f0: 2048 616e 646c 6573 2044 6976 6964 6520   Handles Divide 
-00027800: 6279 2030 2077 6172 6e69 6e67 0a20 2020  by 0 warning.   
-00027810: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
-00027820: 745b 2256 6f6c 756d 6522 5d20 3d20 3020  t["Volume"] = 0 
-00027830: 2023 2022 556e 6b6e 6f77 6e22 0a20 2020   # "Unknown".   
-00027840: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
-00027850: 6963 745b 2256 6f6c 756d 6522 5d20 3d20  ict["Volume"] = 
-00027860: 300a 2020 2020 2020 2020 2020 2020 7265  0.            re
-00027870: 7475 726e 2046 616c 7365 2c20 6861 734d  turn False, hasM
-00027880: 696e 696d 756d 566f 6c75 6d65 0a20 2020  inimumVolume.   
-00027890: 2020 2020 2072 6174 696f 203d 2072 6f75       ratio = rou
-000278a0: 6e64 2872 6563 656e 745b 2256 6f6c 756d  nd(recent["Volum
-000278b0: 6522 5d2e 696c 6f63 5b30 5d20 2f20 7265  e"].iloc[0] / re
-000278c0: 6365 6e74 5b22 566f 6c4d 4122 5d2e 696c  cent["VolMA"].il
-000278d0: 6f63 5b30 5d2c 2032 290a 2020 2020 2020  oc[0], 2).      
-000278e0: 2020 7361 7665 4469 6374 5b22 566f 6c75    saveDict["Volu
-000278f0: 6d65 225d 203d 2072 6174 696f 0a20 2020  me"] = ratio.   
-00027900: 2020 2020 2069 6620 7261 7469 6f20 3e3d       if ratio >=
-00027910: 2076 6f6c 756d 6552 6174 696f 2061 6e64   volumeRatio and
-00027920: 2072 6174 696f 2021 3d20 6e70 2e6e 616e   ratio != np.nan
-00027930: 2061 6e64 2028 6e6f 7420 6d61 7468 2e69   and (not math.i
-00027940: 7369 6e66 2872 6174 696f 2929 3a0a 2020  sinf(ratio)):.  
-00027950: 2020 2020 2020 2020 2020 7363 7265 656e            screen
-00027960: 4469 6374 5b22 566f 6c75 6d65 225d 203d  Dict["Volume"] =
-00027970: 2072 6174 696f 0a20 2020 2020 2020 2020   ratio.         
-00027980: 2020 2072 6574 7572 6e20 5472 7565 2c20     return True, 
-00027990: 6861 734d 696e 696d 756d 566f 6c75 6d65  hasMinimumVolume
-000279a0: 0a20 2020 2020 2020 2073 6372 6565 6e44  .        screenD
-000279b0: 6963 745b 2256 6f6c 756d 6522 5d20 3d20  ict["Volume"] = 
-000279c0: 7261 7469 6f0a 2020 2020 2020 2020 7265  ratio.        re
-000279d0: 7475 726e 2046 616c 7365 2c20 6861 734d  turn False, hasM
-000279e0: 696e 696d 756d 566f 6c75 6d65 0a0a 2020  inimumVolume..  
-000279f0: 2020 2320 4669 6e64 2069 6620 7374 6f63    # Find if stoc
-00027a00: 6b20 6973 2076 616c 6964 6174 696e 6720  k is validating 
-00027a10: 766f 6c75 6d65 2073 7072 6561 6420 616e  volume spread an
-00027a20: 616c 7973 6973 0a20 2020 2064 6566 2076  alysis.    def v
-00027a30: 616c 6964 6174 6556 6f6c 756d 6553 7072  alidateVolumeSpr
-00027a40: 6561 6441 6e61 6c79 7369 7328 7365 6c66  eadAnalysis(self
-00027a50: 2c20 6466 2c20 7363 7265 656e 4469 6374  , df, screenDict
-00027a60: 2c20 7361 7665 4469 6374 293a 0a20 2020  , saveDict):.   
-00027a70: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-00027a80: 2020 2020 2020 6966 2064 6620 6973 204e        if df is N
-00027a90: 6f6e 6520 6f72 206c 656e 2864 6629 203d  one or len(df) =
-00027aa0: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
-00027ab0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-00027ac0: 650a 2020 2020 2020 2020 2020 2020 6461  e.            da
-00027ad0: 7461 203d 2064 662e 636f 7079 2829 0a20  ta = df.copy(). 
-00027ae0: 2020 2020 2020 2020 2020 2064 6174 6120             data 
-00027af0: 3d20 6461 7461 2e68 6561 6428 3229 0a20  = data.head(2). 
-00027b00: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
-00027b10: 6e28 6461 7461 2920 3c20 323a 0a20 2020  n(data) < 2:.   
-00027b20: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00027b30: 7572 6e20 4661 6c73 650a 2020 2020 2020  urn False.      
-00027b40: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-00027b50: 2020 2020 2020 2020 2020 2023 2043 6865             # Che
-00027b60: 636b 2066 6f72 2070 7265 7669 6f75 7320  ck for previous 
-00027b70: 5245 4420 6361 6e64 6c65 730a 2020 2020  RED candles.    
-00027b80: 2020 2020 2020 2020 2020 2020 2320 4375              # Cu
-00027b90: 7272 656e 7420 6361 6e64 6c65 203d 2030  rrent candle = 0
-00027ba0: 7468 2c20 5072 6576 696f 7573 2043 616e  th, Previous Can
-00027bb0: 646c 6520 3d20 3173 7420 666f 7220 666f  dle = 1st for fo
-00027bc0: 6c6c 6f77 696e 6720 6c6f 6769 630a 2020  llowing logic.  
-00027bd0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00027be0: 2064 6174 612e 696c 6f63 5b31 5d5b 224f   data.iloc[1]["O
-00027bf0: 7065 6e22 5d20 3e3d 2064 6174 612e 696c  pen"] >= data.il
-00027c00: 6f63 5b31 5d5b 2243 6c6f 7365 225d 3a0a  oc[1]["Close"]:.
-00027c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027c20: 2020 2020 7370 7265 6164 3120 3d20 6162      spread1 = ab
-00027c30: 7328 6461 7461 2e69 6c6f 635b 315d 5b22  s(data.iloc[1]["
-00027c40: 4f70 656e 225d 202d 2064 6174 612e 696c  Open"] - data.il
-00027c50: 6f63 5b31 5d5b 2243 6c6f 7365 225d 290a  oc[1]["Close"]).
-00027c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027c70: 2020 2020 7370 7265 6164 3020 3d20 6162      spread0 = ab
-00027c80: 7328 6461 7461 2e69 6c6f 635b 305d 5b22  s(data.iloc[0]["
-00027c90: 4f70 656e 225d 202d 2064 6174 612e 696c  Open"] - data.il
-00027ca0: 6f63 5b30 5d5b 2243 6c6f 7365 225d 290a  oc[0]["Close"]).
-00027cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027cc0: 2020 2020 6c6f 7765 725f 7769 636b 5f73      lower_wick_s
-00027cd0: 7072 6561 6430 203d 2028 0a20 2020 2020  pread0 = (.     
-00027ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027cf0: 2020 206d 6178 2864 6174 612e 696c 6f63     max(data.iloc
-00027d00: 5b30 5d5b 224f 7065 6e22 5d2c 2064 6174  [0]["Open"], dat
-00027d10: 612e 696c 6f63 5b30 5d5b 2243 6c6f 7365  a.iloc[0]["Close
-00027d20: 225d 290a 2020 2020 2020 2020 2020 2020  "]).            
-00027d30: 2020 2020 2020 2020 2020 2020 2d20 6461              - da
-00027d40: 7461 2e69 6c6f 635b 305d 5b22 4c6f 7722  ta.iloc[0]["Low"
-00027d50: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-00027d60: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00027d70: 2020 2020 2020 2020 2020 2020 766f 6c31              vol1
-00027d80: 203d 2064 6174 612e 696c 6f63 5b31 5d5b   = data.iloc[1][
-00027d90: 2256 6f6c 756d 6522 5d0a 2020 2020 2020  "Volume"].      
-00027da0: 2020 2020 2020 2020 2020 2020 2020 766f                vo
-00027db0: 6c30 203d 2064 6174 612e 696c 6f63 5b30  l0 = data.iloc[0
-00027dc0: 5d5b 2256 6f6c 756d 6522 5d0a 2020 2020  ]["Volume"].    
-00027dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027de0: 7361 7665 6420 3d20 7365 6c66 2e66 696e  saved = self.fin
-00027df0: 6443 7572 7265 6e74 5361 7665 6456 616c  dCurrentSavedVal
-00027e00: 7565 2873 6372 6565 6e44 6963 742c 2073  ue(screenDict, s
-00027e10: 6176 6544 6963 742c 2022 5061 7474 6572  aveDict, "Patter
-00027e20: 6e22 290a 2020 2020 2020 2020 2020 2020  n").            
-00027e30: 2020 2020 2020 2020 6966 2028 0a20 2020          if (.   
-00027e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027e50: 2020 2020 2073 7072 6561 6430 203e 2073       spread0 > s
-00027e60: 7072 6561 6431 0a20 2020 2020 2020 2020  pread1.         
-00027e70: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00027e80: 6e64 2076 6f6c 3020 3c20 766f 6c31 0a20  nd vol0 < vol1. 
-00027e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027ea0: 2020 2020 2020 2061 6e64 2064 6174 612e         and data.
-00027eb0: 696c 6f63 5b30 5d5b 2256 6f6c 756d 6522  iloc[0]["Volume"
-00027ec0: 5d20 3c20 6461 7461 2e69 6c6f 635b 305d  ] < data.iloc[0]
-00027ed0: 5b22 566f 6c4d 4122 5d0a 2020 2020 2020  ["VolMA"].      
-00027ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027ef0: 2020 616e 6420 6461 7461 2e69 6c6f 635b    and data.iloc[
-00027f00: 305d 5b22 436c 6f73 6522 5d20 3c3d 2064  0]["Close"] <= d
-00027f10: 6174 612e 696c 6f63 5b31 5d5b 224f 7065  ata.iloc[1]["Ope
-00027f20: 6e22 5d0a 2020 2020 2020 2020 2020 2020  n"].            
-00027f30: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-00027f40: 7370 7265 6164 3020 3c20 6c6f 7765 725f  spread0 < lower_
-00027f50: 7769 636b 5f73 7072 6561 6430 0a20 2020  wick_spread0.   
-00027f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027f70: 2020 2020 2061 6e64 2064 6174 612e 696c       and data.il
-00027f80: 6f63 5b30 5d5b 2256 6f6c 756d 6522 5d20  oc[0]["Volume"] 
-00027f90: 3c3d 2069 6e74 2864 6174 612e 696c 6f63  <= int(data.iloc
-00027fa0: 5b31 5d5b 2256 6f6c 756d 6522 5d20 2a20  [1]["Volume"] * 
-00027fb0: 302e 3735 290a 2020 2020 2020 2020 2020  0.75).          
-00027fc0: 2020 2020 2020 2020 2020 293a 0a20 2020            ):.   
-00027fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027fe0: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
-00027ff0: 2250 6174 7465 726e 225d 203d 2028 0a20  "Pattern"] = (. 
-00028000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028010: 2020 2020 2020 2020 2020 2073 6176 6564             saved
-00028020: 5b30 5d20 0a20 2020 2020 2020 2020 2020  [0] .           
+00027450: 2020 2020 2b20 636f 6c6f 7254 6578 742e      + colorText.
+00027460: 4752 4545 4e0a 2020 2020 2020 2020 2020  GREEN.          
+00027470: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+00027480: 6622 5643 5020 2842 4f3a 207b 6869 6768  f"VCP (BO: {high
+00027490: 6573 7454 6f70 7d29 220a 2020 2020 2020  estTop})".      
+000274a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000274b0: 2020 2b20 636f 6c6f 7254 6578 742e 454e    + colorText.EN
+000274c0: 440a 2020 2020 2020 2020 2020 2020 2020  D.              
+000274d0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+000274e0: 2020 2020 2020 2020 2020 2020 7361 7665              save
+000274f0: 4469 6374 5b22 5061 7474 6572 6e22 5d20  Dict["Pattern"] 
+00027500: 3d20 7361 7665 645b 315d 202b 2066 2256  = saved[1] + f"V
+00027510: 4350 2028 424f 3a20 7b68 6967 6865 7374  CP (BO: {highest
+00027520: 546f 707d 2922 0a20 2020 2020 2020 2020  Top})".         
+00027530: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00027540: 6e20 5472 7565 0a20 2020 2020 2020 2065  n True.        e
+00027550: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
+00027560: 6173 2065 3a20 2023 2070 7261 676d 613a  as e:  # pragma:
+00027570: 206e 6f20 636f 7665 720a 2020 2020 2020   no cover.      
+00027580: 2020 2020 2020 7365 6c66 2e64 6566 6175        self.defau
+00027590: 6c74 5f6c 6f67 6765 722e 6465 6275 6728  lt_logger.debug(
+000275a0: 652c 2065 7863 5f69 6e66 6f3d 5472 7565  e, exc_info=True
+000275b0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+000275c0: 2046 616c 7365 0a0a 2020 2020 2320 5661   False..    # Va
+000275d0: 6c69 6461 7465 2069 6620 766f 6c75 6d65  lidate if volume
+000275e0: 206f 6620 6c61 7374 2064 6179 2069 7320   of last day is 
+000275f0: 6869 6768 6572 2074 6861 6e20 6176 670a  higher than avg.
+00027600: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+00027610: 566f 6c75 6d65 280a 2020 2020 2020 2020  Volume(.        
+00027620: 7365 6c66 2c20 6466 2c20 7363 7265 656e  self, df, screen
+00027630: 4469 6374 2c20 7361 7665 4469 6374 2c20  Dict, saveDict, 
+00027640: 766f 6c75 6d65 5261 7469 6f3d 322e 352c  volumeRatio=2.5,
+00027650: 206d 696e 566f 6c75 6d65 3d31 3030 0a20   minVolume=100. 
+00027660: 2020 2029 3a0a 2020 2020 2020 2020 6966     ):.        if
+00027670: 2064 6620 6973 204e 6f6e 6520 6f72 206c   df is None or l
+00027680: 656e 2864 6629 203d 3d20 303a 0a20 2020  en(df) == 0:.   
+00027690: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000276a0: 4661 6c73 652c 2046 616c 7365 0a20 2020  False, False.   
+000276b0: 2020 2020 2064 6174 6120 3d20 6466 2e63       data = df.c
+000276c0: 6f70 7928 290a 2020 2020 2020 2020 6461  opy().        da
+000276d0: 7461 203d 2064 6174 612e 6669 6c6c 6e61  ta = data.fillna
+000276e0: 2830 290a 2020 2020 2020 2020 6461 7461  (0).        data
+000276f0: 203d 2064 6174 612e 7265 706c 6163 6528   = data.replace(
+00027700: 5b6e 702e 696e 662c 202d 6e70 2e69 6e66  [np.inf, -np.inf
+00027710: 5d2c 2030 290a 2020 2020 2020 2020 7265  ], 0).        re
+00027720: 6365 6e74 203d 2064 6174 612e 6865 6164  cent = data.head
+00027730: 2831 290a 2020 2020 2020 2020 2320 4569  (1).        # Ei
+00027740: 7468 6572 2074 6865 2072 6f6c 6c69 6e67  ther the rolling
+00027750: 2076 6f6c 756d 6520 6f66 2070 6173 7420   volume of past 
+00027760: 3230 2073 6573 7369 6f6e 7320 6f72 2074  20 sessions or t
+00027770: 6f64 6179 2773 2076 6f6c 756d 6520 7368  oday's volume sh
+00027780: 6f75 6c64 2062 6520 3e20 6d69 6e20 766f  ould be > min vo
+00027790: 6c75 6d65 0a20 2020 2020 2020 2068 6173  lume.        has
+000277a0: 4d69 6e69 6d75 6d56 6f6c 756d 6520 3d20  MinimumVolume = 
+000277b0: 280a 2020 2020 2020 2020 2020 2020 7265  (.            re
+000277c0: 6365 6e74 5b22 566f 6c4d 4122 5d2e 696c  cent["VolMA"].il
+000277d0: 6f63 5b30 5d20 3e3d 206d 696e 566f 6c75  oc[0] >= minVolu
+000277e0: 6d65 0a20 2020 2020 2020 2020 2020 206f  me.            o
+000277f0: 7220 7265 6365 6e74 5b22 566f 6c75 6d65  r recent["Volume
+00027800: 225d 2e69 6c6f 635b 305d 203e 3d20 6d69  "].iloc[0] >= mi
+00027810: 6e56 6f6c 756d 650a 2020 2020 2020 2020  nVolume.        
+00027820: 290a 2020 2020 2020 2020 6966 2072 6563  ).        if rec
+00027830: 656e 745b 2256 6f6c 4d41 225d 2e69 6c6f  ent["VolMA"].ilo
+00027840: 635b 305d 203d 3d20 303a 2020 2320 4861  c[0] == 0:  # Ha
+00027850: 6e64 6c65 7320 4469 7669 6465 2062 7920  ndles Divide by 
+00027860: 3020 7761 726e 696e 670a 2020 2020 2020  0 warning.      
+00027870: 2020 2020 2020 7361 7665 4469 6374 5b22        saveDict["
+00027880: 566f 6c75 6d65 225d 203d 2030 2020 2320  Volume"] = 0  # 
+00027890: 2255 6e6b 6e6f 776e 220a 2020 2020 2020  "Unknown".      
+000278a0: 2020 2020 2020 7363 7265 656e 4469 6374        screenDict
+000278b0: 5b22 566f 6c75 6d65 225d 203d 2030 0a20  ["Volume"] = 0. 
+000278c0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000278d0: 6e20 4661 6c73 652c 2068 6173 4d69 6e69  n False, hasMini
+000278e0: 6d75 6d56 6f6c 756d 650a 2020 2020 2020  mumVolume.      
+000278f0: 2020 7261 7469 6f20 3d20 726f 756e 6428    ratio = round(
+00027900: 7265 6365 6e74 5b22 566f 6c75 6d65 225d  recent["Volume"]
+00027910: 2e69 6c6f 635b 305d 202f 2072 6563 656e  .iloc[0] / recen
+00027920: 745b 2256 6f6c 4d41 225d 2e69 6c6f 635b  t["VolMA"].iloc[
+00027930: 305d 2c20 3229 0a20 2020 2020 2020 2073  0], 2).        s
+00027940: 6176 6544 6963 745b 2256 6f6c 756d 6522  aveDict["Volume"
+00027950: 5d20 3d20 7261 7469 6f0a 2020 2020 2020  ] = ratio.      
+00027960: 2020 6966 2072 6174 696f 203e 3d20 766f    if ratio >= vo
+00027970: 6c75 6d65 5261 7469 6f20 616e 6420 7261  lumeRatio and ra
+00027980: 7469 6f20 213d 206e 702e 6e61 6e20 616e  tio != np.nan an
+00027990: 6420 286e 6f74 206d 6174 682e 6973 696e  d (not math.isin
+000279a0: 6628 7261 7469 6f29 293a 0a20 2020 2020  f(ratio)):.     
+000279b0: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
+000279c0: 745b 2256 6f6c 756d 6522 5d20 3d20 7261  t["Volume"] = ra
+000279d0: 7469 6f0a 2020 2020 2020 2020 2020 2020  tio.            
+000279e0: 7265 7475 726e 2054 7275 652c 2068 6173  return True, has
+000279f0: 4d69 6e69 6d75 6d56 6f6c 756d 650a 2020  MinimumVolume.  
+00027a00: 2020 2020 2020 7363 7265 656e 4469 6374        screenDict
+00027a10: 5b22 566f 6c75 6d65 225d 203d 2072 6174  ["Volume"] = rat
+00027a20: 696f 0a20 2020 2020 2020 2072 6574 7572  io.        retur
+00027a30: 6e20 4661 6c73 652c 2068 6173 4d69 6e69  n False, hasMini
+00027a40: 6d75 6d56 6f6c 756d 650a 0a20 2020 2023  mumVolume..    #
+00027a50: 2046 696e 6420 6966 2073 746f 636b 2069   Find if stock i
+00027a60: 7320 7661 6c69 6461 7469 6e67 2076 6f6c  s validating vol
+00027a70: 756d 6520 7370 7265 6164 2061 6e61 6c79  ume spread analy
+00027a80: 7369 730a 2020 2020 6465 6620 7661 6c69  sis.    def vali
+00027a90: 6461 7465 566f 6c75 6d65 5370 7265 6164  dateVolumeSpread
+00027aa0: 416e 616c 7973 6973 2873 656c 662c 2064  Analysis(self, d
+00027ab0: 662c 2073 6372 6565 6e44 6963 742c 2073  f, screenDict, s
+00027ac0: 6176 6544 6963 7429 3a0a 2020 2020 2020  aveDict):.      
+00027ad0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+00027ae0: 2020 2069 6620 6466 2069 7320 4e6f 6e65     if df is None
+00027af0: 206f 7220 6c65 6e28 6466 2920 3d3d 2030   or len(df) == 0
+00027b00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00027b10: 2020 7265 7475 726e 2046 616c 7365 0a20    return False. 
+00027b20: 2020 2020 2020 2020 2020 2064 6174 6120             data 
+00027b30: 3d20 6466 2e63 6f70 7928 290a 2020 2020  = df.copy().    
+00027b40: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
+00027b50: 6174 612e 6865 6164 2832 290a 2020 2020  ata.head(2).    
+00027b60: 2020 2020 2020 2020 6966 206c 656e 2864          if len(d
+00027b70: 6174 6129 203c 2032 3a0a 2020 2020 2020  ata) < 2:.      
+00027b80: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00027b90: 2046 616c 7365 0a20 2020 2020 2020 2020   False.         
+00027ba0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+00027bb0: 2020 2020 2020 2020 2320 4368 6563 6b20          # Check 
+00027bc0: 666f 7220 7072 6576 696f 7573 2052 4544  for previous RED
+00027bd0: 2063 616e 646c 6573 0a20 2020 2020 2020   candles.       
+00027be0: 2020 2020 2020 2020 2023 2043 7572 7265           # Curre
+00027bf0: 6e74 2063 616e 646c 6520 3d20 3074 682c  nt candle = 0th,
+00027c00: 2050 7265 7669 6f75 7320 4361 6e64 6c65   Previous Candle
+00027c10: 203d 2031 7374 2066 6f72 2066 6f6c 6c6f   = 1st for follo
+00027c20: 7769 6e67 206c 6f67 6963 0a20 2020 2020  wing logic.     
+00027c30: 2020 2020 2020 2020 2020 2069 6620 6461             if da
+00027c40: 7461 2e69 6c6f 635b 315d 5b22 4f70 656e  ta.iloc[1]["Open
+00027c50: 225d 203e 3d20 6461 7461 2e69 6c6f 635b  "] >= data.iloc[
+00027c60: 315d 5b22 436c 6f73 6522 5d3a 0a20 2020  1]["Close"]:.   
+00027c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027c80: 2073 7072 6561 6431 203d 2061 6273 2864   spread1 = abs(d
+00027c90: 6174 612e 696c 6f63 5b31 5d5b 224f 7065  ata.iloc[1]["Ope
+00027ca0: 6e22 5d20 2d20 6461 7461 2e69 6c6f 635b  n"] - data.iloc[
+00027cb0: 315d 5b22 436c 6f73 6522 5d29 0a20 2020  1]["Close"]).   
+00027cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027cd0: 2073 7072 6561 6430 203d 2061 6273 2864   spread0 = abs(d
+00027ce0: 6174 612e 696c 6f63 5b30 5d5b 224f 7065  ata.iloc[0]["Ope
+00027cf0: 6e22 5d20 2d20 6461 7461 2e69 6c6f 635b  n"] - data.iloc[
+00027d00: 305d 5b22 436c 6f73 6522 5d29 0a20 2020  0]["Close"]).   
+00027d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027d20: 206c 6f77 6572 5f77 6963 6b5f 7370 7265   lower_wick_spre
+00027d30: 6164 3020 3d20 280a 2020 2020 2020 2020  ad0 = (.        
+00027d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027d50: 6d61 7828 6461 7461 2e69 6c6f 635b 305d  max(data.iloc[0]
+00027d60: 5b22 4f70 656e 225d 2c20 6461 7461 2e69  ["Open"], data.i
+00027d70: 6c6f 635b 305d 5b22 436c 6f73 6522 5d29  loc[0]["Close"])
+00027d80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00027d90: 2020 2020 2020 2020 202d 2064 6174 612e           - data.
+00027da0: 696c 6f63 5b30 5d5b 224c 6f77 225d 0a20  iloc[0]["Low"]. 
+00027db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027dc0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00027dd0: 2020 2020 2020 2020 2076 6f6c 3120 3d20           vol1 = 
+00027de0: 6461 7461 2e69 6c6f 635b 315d 5b22 566f  data.iloc[1]["Vo
+00027df0: 6c75 6d65 225d 0a20 2020 2020 2020 2020  lume"].         
+00027e00: 2020 2020 2020 2020 2020 2076 6f6c 3020             vol0 
+00027e10: 3d20 6461 7461 2e69 6c6f 635b 305d 5b22  = data.iloc[0]["
+00027e20: 566f 6c75 6d65 225d 0a20 2020 2020 2020  Volume"].       
+00027e30: 2020 2020 2020 2020 2020 2020 2073 6176               sav
+00027e40: 6564 203d 2073 656c 662e 6669 6e64 4375  ed = self.findCu
+00027e50: 7272 656e 7453 6176 6564 5661 6c75 6528  rrentSavedValue(
+00027e60: 7363 7265 656e 4469 6374 2c20 7361 7665  screenDict, save
+00027e70: 4469 6374 2c20 2250 6174 7465 726e 2229  Dict, "Pattern")
+00027e80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00027e90: 2020 2020 2069 6620 280a 2020 2020 2020       if (.      
+00027ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027eb0: 2020 7370 7265 6164 3020 3e20 7370 7265    spread0 > spre
+00027ec0: 6164 310a 2020 2020 2020 2020 2020 2020  ad1.            
+00027ed0: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+00027ee0: 766f 6c30 203c 2076 6f6c 310a 2020 2020  vol0 < vol1.    
+00027ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027f00: 2020 2020 616e 6420 6461 7461 2e69 6c6f      and data.ilo
+00027f10: 635b 305d 5b22 566f 6c75 6d65 225d 203c  c[0]["Volume"] <
+00027f20: 2064 6174 612e 696c 6f63 5b30 5d5b 2256   data.iloc[0]["V
+00027f30: 6f6c 4d41 225d 0a20 2020 2020 2020 2020  olMA"].         
+00027f40: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00027f50: 6e64 2064 6174 612e 696c 6f63 5b30 5d5b  nd data.iloc[0][
+00027f60: 2243 6c6f 7365 225d 203c 3d20 6461 7461  "Close"] <= data
+00027f70: 2e69 6c6f 635b 315d 5b22 4f70 656e 225d  .iloc[1]["Open"]
+00027f80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00027f90: 2020 2020 2020 2020 2061 6e64 2073 7072           and spr
+00027fa0: 6561 6430 203c 206c 6f77 6572 5f77 6963  ead0 < lower_wic
+00027fb0: 6b5f 7370 7265 6164 300a 2020 2020 2020  k_spread0.      
+00027fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027fd0: 2020 616e 6420 6461 7461 2e69 6c6f 635b    and data.iloc[
+00027fe0: 305d 5b22 566f 6c75 6d65 225d 203c 3d20  0]["Volume"] <= 
+00027ff0: 696e 7428 6461 7461 2e69 6c6f 635b 315d  int(data.iloc[1]
+00028000: 5b22 566f 6c75 6d65 225d 202a 2030 2e37  ["Volume"] * 0.7
+00028010: 3529 0a20 2020 2020 2020 2020 2020 2020  5).             
+00028020: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
 00028030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028040: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
-00028050: 440a 2020 2020 2020 2020 2020 2020 2020  D.              
-00028060: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-00028070: 636f 6c6f 7254 6578 742e 4752 4545 4e0a  colorText.GREEN.
-00028080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028090: 2020 2020 2020 2020 2020 2020 2b20 2253              + "S
-000280a0: 7570 706c 7920 4472 6f75 6768 7422 0a20  upply Drought". 
+00028040: 2020 7363 7265 656e 4469 6374 5b22 5061    screenDict["Pa
+00028050: 7474 6572 6e22 5d20 3d20 280a 2020 2020  ttern"] = (.    
+00028060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028070: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
+00028080: 200a 2020 2020 2020 2020 2020 2020 2020   .              
+00028090: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+000280a0: 636f 6c6f 7254 6578 742e 424f 4c44 0a20  colorText.BOLD. 
 000280b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000280c0: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
-000280d0: 6f72 5465 7874 2e45 4e44 0a20 2020 2020  orText.END.     
+000280d0: 6f72 5465 7874 2e47 5245 454e 0a20 2020  orText.GREEN.   
 000280e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000280f0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00028100: 2020 2020 2020 2020 2020 2020 2073 6176               sav
-00028110: 6544 6963 745b 2250 6174 7465 726e 225d  eDict["Pattern"]
-00028120: 203d 2073 6176 6564 5b31 5d20 2b20 2253   = saved[1] + "S
-00028130: 7570 706c 7920 4472 6f75 6768 7422 0a20  upply Drought". 
+000280f0: 2020 2020 2020 2020 202b 2022 5375 7070           + "Supp
+00028100: 6c79 2044 726f 7567 6874 220a 2020 2020  ly Drought".    
+00028110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028120: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
+00028130: 6578 742e 454e 440a 2020 2020 2020 2020  ext.END.        
 00028140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028150: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-00028160: 7565 0a20 2020 2020 2020 2020 2020 2020  ue.             
-00028170: 2020 2020 2020 2069 6620 280a 2020 2020         if (.    
-00028180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028190: 2020 2020 7370 7265 6164 3020 3c20 7370      spread0 < sp
-000281a0: 7265 6164 310a 2020 2020 2020 2020 2020  read1.          
-000281b0: 2020 2020 2020 2020 2020 2020 2020 616e                an
-000281c0: 6420 766f 6c30 203e 2076 6f6c 310a 2020  d vol0 > vol1.  
-000281d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000281e0: 2020 2020 2020 616e 6420 6461 7461 2e69        and data.i
-000281f0: 6c6f 635b 305d 5b22 566f 6c75 6d65 225d  loc[0]["Volume"]
-00028200: 203e 2064 6174 612e 696c 6f63 5b30 5d5b   > data.iloc[0][
-00028210: 2256 6f6c 4d41 225d 0a20 2020 2020 2020  "VolMA"].       
-00028220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028230: 2061 6e64 2064 6174 612e 696c 6f63 5b30   and data.iloc[0
-00028240: 5d5b 2243 6c6f 7365 225d 203c 3d20 6461  ]["Close"] <= da
-00028250: 7461 2e69 6c6f 635b 315d 5b22 4f70 656e  ta.iloc[1]["Open
-00028260: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
-00028270: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
-00028280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028290: 2020 7363 7265 656e 4469 6374 5b22 5061    screenDict["Pa
-000282a0: 7474 6572 6e22 5d20 3d20 280a 2020 2020  ttern"] = (.    
-000282b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000282c0: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
-000282d0: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-000282e0: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-000282f0: 636f 6c6f 7254 6578 742e 424f 4c44 0a20  colorText.BOLD. 
-00028300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028310: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
-00028320: 6f72 5465 7874 2e47 5245 454e 0a20 2020  orText.GREEN.   
+00028150: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00028160: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
+00028170: 6374 5b22 5061 7474 6572 6e22 5d20 3d20  ct["Pattern"] = 
+00028180: 7361 7665 645b 315d 202b 2022 5375 7070  saved[1] + "Supp
+00028190: 6c79 2044 726f 7567 6874 220a 2020 2020  ly Drought".    
+000281a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000281b0: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+000281c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000281d0: 2020 2020 6966 2028 0a20 2020 2020 2020      if (.       
+000281e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000281f0: 2073 7072 6561 6430 203c 2073 7072 6561   spread0 < sprea
+00028200: 6431 0a20 2020 2020 2020 2020 2020 2020  d1.             
+00028210: 2020 2020 2020 2020 2020 2061 6e64 2076             and v
+00028220: 6f6c 3020 3e20 766f 6c31 0a20 2020 2020  ol0 > vol1.     
+00028230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028240: 2020 2061 6e64 2064 6174 612e 696c 6f63     and data.iloc
+00028250: 5b30 5d5b 2256 6f6c 756d 6522 5d20 3e20  [0]["Volume"] > 
+00028260: 6461 7461 2e69 6c6f 635b 305d 5b22 566f  data.iloc[0]["Vo
+00028270: 6c4d 4122 5d0a 2020 2020 2020 2020 2020  lMA"].          
+00028280: 2020 2020 2020 2020 2020 2020 2020 616e                an
+00028290: 6420 6461 7461 2e69 6c6f 635b 305d 5b22  d data.iloc[0]["
+000282a0: 436c 6f73 6522 5d20 3c3d 2064 6174 612e  Close"] <= data.
+000282b0: 696c 6f63 5b31 5d5b 224f 7065 6e22 5d0a  iloc[1]["Open"].
+000282c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000282d0: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
+000282e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000282f0: 6372 6565 6e44 6963 745b 2250 6174 7465  creenDict["Patte
+00028300: 726e 225d 203d 2028 0a20 2020 2020 2020  rn"] = (.       
+00028310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028320: 2020 2020 2073 6176 6564 5b30 5d20 0a20       saved[0] . 
 00028330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028340: 2020 2020 2020 2020 202b 2022 4465 6d61           + "Dema
-00028350: 6e64 2052 6973 6522 0a20 2020 2020 2020  nd Rise".       
+00028340: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
+00028350: 6f72 5465 7874 2e42 4f4c 440a 2020 2020  orText.BOLD.    
 00028360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028370: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
-00028380: 2e45 4e44 0a20 2020 2020 2020 2020 2020  .END.           
-00028390: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-000283a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000283b0: 2020 2020 2020 2073 6176 6544 6963 745b         saveDict[
-000283c0: 2250 6174 7465 726e 225d 203d 2073 6176  "Pattern"] = sav
-000283d0: 6564 5b31 5d20 2b20 2244 656d 616e 6420  ed[1] + "Demand 
-000283e0: 5269 7365 220a 2020 2020 2020 2020 2020  Rise".          
-000283f0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00028400: 7475 726e 2054 7275 650a 2020 2020 2020  turn True.      
-00028410: 2020 2020 2020 6578 6365 7074 2049 6e64        except Ind
-00028420: 6578 4572 726f 7220 6173 2065 3a20 2320  exError as e: # 
-00028430: 7072 6167 6d61 3a20 6e6f 2063 6f76 6572  pragma: no cover
-00028440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00028450: 2073 656c 662e 6465 6661 756c 745f 6c6f   self.default_lo
-00028460: 6767 6572 2e64 6562 7567 2865 2c20 6578  gger.debug(e, ex
-00028470: 635f 696e 666f 3d54 7275 6529 0a20 2020  c_info=True).   
-00028480: 2020 2020 2020 2020 2020 2020 2070 6173               pas
-00028490: 730a 2020 2020 2020 2020 2020 2020 7265  s.            re
-000284a0: 7475 726e 2046 616c 7365 0a20 2020 2020  turn False.     
-000284b0: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-000284c0: 696f 6e20 6173 2065 3a20 2023 2070 7261  ion as e:  # pra
-000284d0: 676d 613a 206e 6f20 636f 7665 720a 2020  gma: no cover.  
-000284e0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-000284f0: 6566 6175 6c74 5f6c 6f67 6765 722e 6465  efault_logger.de
-00028500: 6275 6728 652c 2065 7863 5f69 6e66 6f3d  bug(e, exc_info=
-00028510: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
-00028520: 2020 7265 7475 726e 2046 616c 7365 0a      return False.
+00028370: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
+00028380: 6578 742e 4752 4545 4e0a 2020 2020 2020  ext.GREEN.      
+00028390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000283a0: 2020 2020 2020 2b20 2244 656d 616e 6420        + "Demand 
+000283b0: 5269 7365 220a 2020 2020 2020 2020 2020  Rise".          
+000283c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000283d0: 2020 2b20 636f 6c6f 7254 6578 742e 454e    + colorText.EN
+000283e0: 440a 2020 2020 2020 2020 2020 2020 2020  D.              
+000283f0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00028400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028410: 2020 2020 7361 7665 4469 6374 5b22 5061      saveDict["Pa
+00028420: 7474 6572 6e22 5d20 3d20 7361 7665 645b  ttern"] = saved[
+00028430: 315d 202b 2022 4465 6d61 6e64 2052 6973  1] + "Demand Ris
+00028440: 6522 0a20 2020 2020 2020 2020 2020 2020  e".             
+00028450: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00028460: 6e20 5472 7565 0a20 2020 2020 2020 2020  n True.         
+00028470: 2020 2065 7863 6570 7420 496e 6465 7845     except IndexE
+00028480: 7272 6f72 2061 7320 653a 2023 2070 7261  rror as e: # pra
+00028490: 676d 613a 206e 6f20 636f 7665 720a 2020  gma: no cover.  
+000284a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000284b0: 6c66 2e64 6566 6175 6c74 5f6c 6f67 6765  lf.default_logge
+000284c0: 722e 6465 6275 6728 652c 2065 7863 5f69  r.debug(e, exc_i
+000284d0: 6e66 6f3d 5472 7565 290a 2020 2020 2020  nfo=True).      
+000284e0: 2020 2020 2020 2020 2020 7061 7373 0a20            pass. 
+000284f0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00028500: 6e20 4661 6c73 650a 2020 2020 2020 2020  n False.        
+00028510: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
+00028520: 2061 7320 653a 2020 2320 7072 6167 6d61   as e:  # pragma
+00028530: 3a20 6e6f 2063 6f76 6572 0a20 2020 2020  : no cover.     
+00028540: 2020 2020 2020 2073 656c 662e 6465 6661         self.defa
+00028550: 756c 745f 6c6f 6767 6572 2e64 6562 7567  ult_logger.debug
+00028560: 2865 2c20 6578 635f 696e 666f 3d54 7275  (e, exc_info=Tru
+00028570: 6529 0a20 2020 2020 2020 2020 2020 2072  e).            r
+00028580: 6574 7572 6e20 4661 6c73 650a            eturn False.
```

### Comparing `pkscreener-0.45.20240602.430/pkscreener/classes/StockScreener.py` & `pkscreener-0.45.20240603.432/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.430/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.45.20240603.432/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.430/pkscreener/classes/Utility.py` & `pkscreener-0.45.20240603.432/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.430/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.45.20240603.432/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.430/pkscreener/classes/keys.py` & `pkscreener-0.45.20240603.432/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.430/pkscreener/courbd.ttf` & `pkscreener-0.45.20240603.432/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.430/pkscreener/globals.py` & `pkscreener-0.45.20240603.432/pkscreener/globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -2770,15 +2770,15 @@
         # if filename is not None:
         #     sendMessageToTelegramChannel(
         #         document_filePath=filename, caption=caption, user=user
         #     )
         OutputControls().printOutput(
             colorText.BOLD
             + colorText.WARN
-            + "[+] Notes:1.Trend calculation is based on 'daysToLookBack'. See configuration. 2.Reduce the console font size to fit all columns on screen."
+            + "[+] Notes:1.Trend calculation is based on 'daysToLookBack'. See configuration.\n[+] 2.Reduce the console font size to fit all columns on screen.\n[+] Many columns may have been hidden. Please check pkscreener.ini config."
             + colorText.END
         )
         # try:
         #     if filename is not None:
         #         os.remove(filename)
         # except Exception as e:  # pragma: no cover
         #     default_logger().debug(e, exc_info=True)
```

### Comparing `pkscreener-0.45.20240602.430/pkscreener/pkscreener.ini` & `pkscreener-0.45.20240603.432/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.430/pkscreener/pkscreenerbot.py` & `pkscreener-0.45.20240603.432/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.430/pkscreener/pkscreenercli.py` & `pkscreener-0.45.20240603.432/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.430/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.45.20240603.432/pkscreener.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.45.20240602.430
+Version: 0.45.20240603.432
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240602.430.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240603.432.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,24 +269,24 @@
 * Please feel free to Suggest improvements bugs by creating an issue.
 * Please follow the [Guidelines for Contributing](https://github.com/pkjmesra/PKScreener/blob/main/CONTRIBUTING.md) while making a Pull Request.
 
 ## Disclaimer:
 * DO NOT use the results provided by the software 'solely' to make your trading decisions.
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
-* This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
+* This screener began as a [fork] but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.429/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.430/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.429/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.430/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.429/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.430/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240602.430/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.45.20240603.432/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.430/setup.py` & `pkscreener-0.45.20240603.432/setup.py`

 * *Files identical despite different names*

