# Comparing `tmp/pkscreener-0.45.20240602.429.tar.gz` & `tmp/pkscreener-0.45.20240602.430.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.45.20240602.429.tar", last modified: Sun Jun  2 19:34:25 2024, max compression
+gzip compressed data, was "pkscreener-0.45.20240602.430.tar", last modified: Sun Jun  2 23:45:09 2024, max compression
```

## Comparing `pkscreener-0.45.20240602.429.tar` & `pkscreener-0.45.20240602.430.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:34:25.261185 pkscreener-0.45.20240602.429/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-06-02 19:32:15.000000 pkscreener-0.45.20240602.429/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-06-02 19:32:15.000000 pkscreener-0.45.20240602.429/LICENSE-Others
--rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-06-02 19:34:25.261185 pkscreener-0.45.20240602.429/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    26594 2024-06-02 19:32:15.000000 pkscreener-0.45.20240602.429/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:34:25.253185 pkscreener-0.45.20240602.429/pkscreener/
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-06-02 19:32:15.000000 pkscreener-0.45.20240602.429/pkscreener/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:34:25.261185 pkscreener-0.45.20240602.429/pkscreener/classes/
--rw-r--r--   0 runner    (1001) docker     (127)    13194 2024-06-02 19:32:15.000000 pkscreener-0.45.20240602.429/pkscreener/classes/ArtTexts.py
--rw-r--r--   0 runner    (1001) docker     (127)     9908 2024-06-02 19:32:15.000000 pkscreener-0.45.20240602.429/pkscreener/classes/Backtest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-06-02 19:32:15.000000 pkscreener-0.45.20240602.429/pkscreener/classes/Barometer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16986 2024-06-02 19:32:15.000000 pkscreener-0.45.20240602.429/pkscreener/classes/CandlePatterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-06-02 19:32:15.000000 pkscreener-0.45.20240602.429/pkscreener/classes/Changelog.py
--rw-r--r--   0 runner    (1001) docker     (127)    36121 2024-06-02 19:32:15.000000 pkscreener-0.45.20240602.429/pkscreener/classes/ConfigManager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10122 2024-06-02 19:32:15.000000 pkscreener-0.45.20240602.429/pkscreener/classes/Fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    13402 2024-06-02 19:32:15.000000 pkscreener-0.45.20240602.429/pkscreener/classes/MarketMonitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-06-02 19:32:15.000000 pkscreener-0.45.20240602.429/pkscreener/classes/MarketStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)    47411 2024-06-02 19:32:15.000000 pkscreener-0.45.20240602.429/pkscreener/classes/MenuOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12039 2024-06-02 19:32:15.000000 pkscreener-0.45.20240602.429/pkscreener/classes/OtaUpdater.py
--rw-r--r--   0 runner    (1001) docker     (127)    24198 2024-06-02 19:32:15.000000 pkscreener-0.45.20240602.429/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-r--r--   0 runner    (1001) docker     (127)    22357 2024-06-02 19:32:15.000000 pkscreener-0.45.20240602.429/pkscreener/classes/PKScanRunner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-06-02 19:32:15.000000 pkscreener-0.45.20240602.429/pkscreener/classes/PKScheduledTaskProgress.py
--rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-06-02 19:32:15.000000 pkscreener-0.45.20240602.429/pkscreener/classes/PKScheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-06-02 19:32:15.000000 pkscreener-0.45.20240602.429/pkscreener/classes/PKSpreadsheets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-06-02 19:32:15.000000 pkscreener-0.45.20240602.429/pkscreener/classes/PKTask.py
--rw-r--r--   0 runner    (1001) docker     (127)    19048 2024-06-02 19:32:15.000000 pkscreener-0.45.20240602.429/pkscreener/classes/Pktalib.py
--rw-r--r--   0 runner    (1001) docker     (127)    13876 2024-06-02 19:32:15.000000 pkscreener-0.45.20240602.429/pkscreener/classes/Portfolio.py
--rw-r--r--   0 runner    (1001) docker     (127)    47779 2024-06-02 19:32:15.000000 pkscreener-0.45.20240602.429/pkscreener/classes/PortfolioXRay.py
--rw-r--r--   0 runner    (1001) docker     (127)   164271 2024-06-02 19:32:15.000000 pkscreener-0.45.20240602.429/pkscreener/classes/ScreeningStatistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    56535 2024-06-02 19:32:15.000000 pkscreener-0.45.20240602.429/pkscreener/classes/StockScreener.py
--rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-06-02 19:32:15.000000 pkscreener-0.45.20240602.429/pkscreener/classes/UserMenuChoicesHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    85660 2024-06-02 19:32:15.000000 pkscreener-0.45.20240602.429/pkscreener/classes/Utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-06-02 19:32:15.000000 pkscreener-0.45.20240602.429/pkscreener/classes/WorkflowManager.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-06-02 19:34:18.000000 pkscreener-0.45.20240602.429/pkscreener/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-06-02 19:32:15.000000 pkscreener-0.45.20240602.429/pkscreener/classes/keys.py
--rw-r--r--   0 runner    (1001) docker     (127)   791436 2024-06-02 19:32:15.000000 pkscreener-0.45.20240602.429/pkscreener/courbd.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   148321 2024-06-02 19:32:15.000000 pkscreener-0.45.20240602.429/pkscreener/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-06-02 19:32:15.000000 pkscreener-0.45.20240602.429/pkscreener/pkscreener.ini
--rw-r--r--   0 runner    (1001) docker     (127)    61567 2024-06-02 19:32:15.000000 pkscreener-0.45.20240602.429/pkscreener/pkscreenerbot.py
--rw-r--r--   0 runner    (1001) docker     (127)    36859 2024-06-02 19:32:15.000000 pkscreener-0.45.20240602.429/pkscreener/pkscreenercli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:34:25.257185 pkscreener-0.45.20240602.429/pkscreener.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-06-02 19:34:25.000000 pkscreener-0.45.20240602.429/pkscreener.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-06-02 19:34:25.000000 pkscreener-0.45.20240602.429/pkscreener.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 19:34:25.000000 pkscreener-0.45.20240602.429/pkscreener.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-06-02 19:34:25.000000 pkscreener-0.45.20240602.429/pkscreener.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 19:34:25.000000 pkscreener-0.45.20240602.429/pkscreener.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-06-02 19:34:25.000000 pkscreener-0.45.20240602.429/pkscreener.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-02 19:34:25.000000 pkscreener-0.45.20240602.429/pkscreener.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-06-02 19:34:25.261185 pkscreener-0.45.20240602.429/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5567 2024-06-02 19:32:15.000000 pkscreener-0.45.20240602.429/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 23:45:09.933004 pkscreener-0.45.20240602.430/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/LICENSE-Others
+-rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-06-02 23:45:09.933004 pkscreener-0.45.20240602.430/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    26594 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 23:45:09.929004 pkscreener-0.45.20240602.430/pkscreener/
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 23:45:09.933004 pkscreener-0.45.20240602.430/pkscreener/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)    13194 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/ArtTexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9908 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/Backtest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/Barometer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16986 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/CandlePatterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/Changelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36121 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/ConfigManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10122 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/Fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14227 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/MarketMonitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/MarketStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47566 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/MenuOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12039 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/OtaUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24198 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22357 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/PKScanRunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/PKScheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/PKSpreadsheets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/PKTask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19048 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/Pktalib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13876 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/Portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47779 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/PortfolioXRay.py
+-rw-r--r--   0 runner    (1001) docker     (127)   165167 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/ScreeningStatistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56535 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/StockScreener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85786 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/Utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/WorkflowManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-06-02 23:45:03.000000 pkscreener-0.45.20240602.430/pkscreener/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/classes/keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)   791436 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/courbd.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   153034 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/pkscreener.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    61567 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/pkscreenerbot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37014 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/pkscreener/pkscreenercli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 23:45:09.929004 pkscreener-0.45.20240602.430/pkscreener.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-06-02 23:45:09.000000 pkscreener-0.45.20240602.430/pkscreener.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-06-02 23:45:09.000000 pkscreener-0.45.20240602.430/pkscreener.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 23:45:09.000000 pkscreener-0.45.20240602.430/pkscreener.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-06-02 23:45:09.000000 pkscreener-0.45.20240602.430/pkscreener.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 23:45:09.000000 pkscreener-0.45.20240602.430/pkscreener.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-06-02 23:45:09.000000 pkscreener-0.45.20240602.430/pkscreener.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-02 23:45:09.000000 pkscreener-0.45.20240602.430/pkscreener.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-06-02 23:45:09.933004 pkscreener-0.45.20240602.430/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5567 2024-06-02 23:43:15.000000 pkscreener-0.45.20240602.430/setup.py
```

### Comparing `pkscreener-0.45.20240602.429/LICENSE` & `pkscreener-0.45.20240602.430/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.429/LICENSE-Others` & `pkscreener-0.45.20240602.430/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.429/PKG-INFO` & `pkscreener-0.45.20240602.430/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.45.20240602.429
+Version: 0.45.20240602.430
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240602.429.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240602.430.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -274,19 +274,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.428/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.429/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.428/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.429/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.428/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.429/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240602.429/README.md` & `pkscreener-0.45.20240602.430/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -252,19 +252,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.428/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.429/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.428/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.429/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.428/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.429/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240602.429/pkscreener/__init__.py` & `pkscreener-0.45.20240602.430/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.429/pkscreener/classes/ArtTexts.py` & `pkscreener-0.45.20240602.430/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.429/pkscreener/classes/Backtest.py` & `pkscreener-0.45.20240602.430/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.429/pkscreener/classes/Barometer.py` & `pkscreener-0.45.20240602.430/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.429/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.45.20240602.430/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.429/pkscreener/classes/Changelog.py` & `pkscreener-0.45.20240602.430/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.429/pkscreener/classes/ConfigManager.py` & `pkscreener-0.45.20240602.430/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.429/pkscreener/classes/Fetcher.py` & `pkscreener-0.45.20240602.430/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.429/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.45.20240602.430/pkscreener/classes/MarketMonitor.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         super(MarketMonitor, self).__init__()
         if monitors is not None and len(monitors) > 0:
             
             self.monitors = monitors[:maxNumResultRowsInMonitor*maxNumResultsPerRow]
             self.monitorIndex = 0
             self.monitorPositions = {}
             self.monitorResultStocks = {}
+            self.hiddenColumns = ""
             # self.monitorNames = {}
             # We are going to present the dataframes in a 3x3 matrix with limited set of columns
             rowIndex = 0
             colIndex = 0
             self.maxNumResultRowsInMonitor = maxNumResultRowsInMonitor
             self.maxNumRowsInEachResult = maxNumRowsInEachResult
             self.maxNumColsInEachResult = maxNumColsInEachResult
@@ -177,17 +178,31 @@
             headers="keys" if self.isPinnedSingleMonitorMode else (),
             highlightCharacter=colorText.HEAD+"="+colorText.END,
             showindex=self.isPinnedSingleMonitorMode,
             highlightedRows=highlightRows,
             highlightedColumns=highlightCols,
             maxcolwidths=Utility.tools.getMaxColumnWidths(self.monitor_df)
         )
+        console_results = ""
+        if self.isPinnedSingleMonitorMode:
+            copyScreenResults = self.monitor_df.copy()
+            hiddenColumns = self.hiddenColumns.split(",")
+            for col in copyScreenResults.columns:
+                if col in hiddenColumns:
+                    copyScreenResults.drop(col, axis=1, inplace=True, errors="ignore")
+            try:
+                console_results = colorText.miniTabulator().tabulate(
+                        copyScreenResults, headers="keys", tablefmt=colorText.No_Pad_GridFormat,
+                        maxcolwidths=Utility.tools.getMaxColumnWidths(copyScreenResults)
+                    )
+            except:
+                console_results = tabulated_results
         numRecords = len(tabulated_results.splitlines())
         self.lines = numRecords + 1 # 1 for the progress bar at the bottom and 1 for the chosenMenu option
-        OutputControls().printOutput(tabulated_results, enableMultipleLineOutput=True)
+        OutputControls().printOutput(tabulated_results if not self.isPinnedSingleMonitorMode else console_results, enableMultipleLineOutput=True)
         
         if not self.isPinnedSingleMonitorMode:
             if telegram:
                 self.updateIfRunningInTelegramBotMode(screenOptions, chosenMenu, dbTimestamp, telegram, telegram_df)
             elif screenOptions.split(":")[2] == "5" and numRecords > 1: # RSI conditions met? Sound alert!
                 Utility.tools.alertSound(beeps=5)
         else:
```

### Comparing `pkscreener-0.45.20240602.429/pkscreener/classes/MarketStatus.py` & `pkscreener-0.45.20240602.430/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.429/pkscreener/classes/MenuOptions.py` & `pkscreener-0.45.20240602.430/pkscreener/classes/MenuOptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 }
 level1_P_MenuDict = {
     "1": "Predefined Piped Scanners",
     "2": "Define my custom Piped Scanner",
     "3": "Run Piped Scans Saved So Far",
     "M": "Back to the Top/Main menu",
 }
-PREDEFINED_SCAN_MENU_KEYS = ["1","2","3","4","5","6","7","8","9","10","11","12","13","14","15"]
+PREDEFINED_SCAN_MENU_KEYS = ["1","2","3","4","5","6","7","8","9","10","11","12","13","14","15","16"]
 PREDEFINED_SCAN_MENU_TEXTS = [
     "Volume Scanners | High Momentum | Breaking Out Now | ATR Cross     ",
     "Volume Scanners | High Momentum | ATR Cross",
     "Volume Scanners | High Momentum                                    ",
     "Volume Scanners | ATR Cross",
     "Volume Scanners | High Bid/Ask Build Up                            ",
     "High Momentum | ATR Cross",
@@ -74,14 +74,15 @@
     "TTM Sqeeze Buy | Intraday RSI b/w 0 to 54                          ",
     "Volume Scanners | High Momentum | Breaking Out Now | ATR Cross | Intraday RSI b/w 0 to 54",
     "Volume Scanners | ATR Cross | Intraday RSI b/w 0 to 54             ",
     "VCP (Mark Minervini) | Chart Patterns | MA Support",
     "VCP | Chart Patterns | MA Support                                  ",
     "Already Breaking out | VCP (Minervini) | Chart Patterns | MA Support",
     "ATR Trailing Stops | VCP (Minervini)                               ",
+    "VCP | ATR Trailing Stops",
 ]
 level2_P_MenuDict = {}
 for key in PREDEFINED_SCAN_MENU_KEYS:
     level2_P_MenuDict[key] = PREDEFINED_SCAN_MENU_TEXTS[int(key)-1]
 level2_P_MenuDict["M"] = "Back to the Top/Main menu"
 PREDEFINED_SCAN_MENU_VALUES =[
     "--systemlaunched -a y -e -o 'X:12:9:2.5:>|X:0:31:>|X:0:23:>|X:0:27:'",
@@ -94,23 +95,25 @@
     "--systemlaunched -a y -e -o 'X:12:27:>|X:0:30:1:'",
     "--systemlaunched -a y -e -o 'X:12:7:6:1:>|X:0:5:0:54:i 1m'",
     "--systemlaunched -a y -e -o 'X:12:9:2.5:>|X:0:31:>|X:0:23:>|X:0:27:>|X:0:5:0:54:i 1m'",
     "--systemlaunched -a y -e -o 'X:12:9:2.5:>|X:0:27:>|X:0:5:0:54:i 1m'",
     "--systemlaunched -a y -e -o 'X:12:7:8:>|X:12:7:9:1:1:'",
     "--systemlaunched -a y -e -o 'X:12:7:4:>|X:12:7:9:1:1:'",
     "--systemlaunched -a y -e -o 'X:12:2:>|X:12:7:8:>|X:12:7:9:1:1:'",
-    "--systemlaunched -a y -e -o 'X:12:30:1:>|X:12:7:8:'"
+    "--systemlaunched -a y -e -o 'X:12:30:1:>|X:12:7:8:'",
+    "--systemlaunched -a y -e -o 'X:12:7:4:>|X:12:30:1:'",
 ]
 PIPED_SCANNERS = {}
 for key in PREDEFINED_SCAN_MENU_KEYS:
     PIPED_SCANNERS[key] = PREDEFINED_SCAN_MENU_VALUES[int(key)-1]
 
 level1_T_MenuDict = {
     "L": "Long Term",
     "S": "Short Term (Intraday)",
+    "B": "Quick Backtest for N-days/candles ago",
     "M": "Back to the Top/Main menu",
 }
 # Valid periods: 1d,5d,1mo,3mo,6mo,1y,2y,5y,10y,ytd,max
 # Valid intervals: 1m,2m,5m,15m,30m,60m,90m,1h,1d,5d,1wk,1mo,3mo
 level2_T_MenuDict_L = {
     "1": "Daily (1y, 1d)",
     "2": "Weekly (1y, 1wk)",
@@ -736,21 +739,21 @@
         
     def renderLevel1_T_Menus(
         self, skip=[], asList=False, renderStyle=None, parent=None
     ):
         defaultKey = 'L' if configManager.period == '1y' else 'S'
         menuText = self.fromDictionary(
             level1_T_MenuDict,
-            renderExceptionKeys=["M"],
+            renderExceptionKeys=["M","B"],
             renderStyle=renderStyle
             if renderStyle is not None
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
-        ).render(asList=asList,coloredValues=[defaultKey] if not asList else [])
+        ).render(asList=asList,coloredValues=[defaultKey,"B"] if not asList else [])
         if asList:
             return menuText
         else:
             if OutputControls().enableMultipleLineOutput:
                 OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.WARN
```

### Comparing `pkscreener-0.45.20240602.429/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.45.20240602.430/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.429/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.45.20240602.430/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.429/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.45.20240602.430/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.429/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.45.20240602.430/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.429/pkscreener/classes/PKScheduler.py` & `pkscreener-0.45.20240602.430/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.429/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.45.20240602.430/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.429/pkscreener/classes/PKTask.py` & `pkscreener-0.45.20240602.430/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.429/pkscreener/classes/Pktalib.py` & `pkscreener-0.45.20240602.430/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.429/pkscreener/classes/Portfolio.py` & `pkscreener-0.45.20240602.430/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.429/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.45.20240602.430/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.429/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.45.20240602.430/pkscreener/classes/ScreeningStatistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -8529,1739 +8529,1795 @@
 00021500: 656c 7365 2063 6f6c 6f72 5465 7874 2e46  else colorText.F
 00021510: 4149 4c29 202b 2066 227b 6368 616e 6765  AIL) + f"{change
 00021520: 5065 7263 656e 747d 2522 202b 2063 6f6c  Percent}%" + col
 00021530: 6f72 5465 7874 2e45 4e44 2920 6966 206e  orText.END) if n
 00021540: 6f74 2070 642e 6973 6e61 2863 6861 6e67  ot pd.isna(chang
 00021550: 6550 6572 6365 6e74 2920 656c 7365 2027  ePercent) else '
 00021560: 2d27 0a20 2020 2020 2020 2020 2020 2020  -'.             
-00021570: 2020 2073 6372 6565 6e44 6963 745b 2244     screenDict["D
-00021580: 6174 6522 5d20 3d20 6361 6c63 5f64 6174  ate"] = calc_dat
-00021590: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-000215a0: 2020 7361 7665 4469 6374 5b22 4461 7465    saveDict["Date
-000215b0: 225d 203d 2063 616c 635f 6461 7465 0a20  "] = calc_date. 
-000215c0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-000215d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000215e0: 2073 6176 6544 6963 745b 6622 4c54 507b   saveDict[f"LTP{
-000215f0: 7072 647d 225d 203d 206e 702e 6e61 6e0a  prd}"] = np.nan.
-00021600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021610: 7361 7665 4469 6374 5b66 2247 726f 7774  saveDict[f"Growt
-00021620: 687b 7072 647d 225d 203d 206e 702e 6e61  h{prd}"] = np.na
-00021630: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
-00021640: 2020 7363 7265 656e 4469 6374 5b22 4461    screenDict["Da
-00021650: 7465 225d 203d 2063 616c 635f 6461 7465  te"] = calc_date
-00021660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00021670: 2073 6176 6544 6963 745b 2244 6174 6522   saveDict["Date"
-00021680: 5d20 3d20 6361 6c63 5f64 6174 650a 0a20  ] = calc_date.. 
-00021690: 2020 2023 2046 696e 6420 7374 6f63 6b73     # Find stocks
-000216a0: 2074 6861 7420 6172 6520 6265 6172 6973   that are bearis
-000216b0: 6820 696e 7472 6164 6179 3a20 4d61 6364  h intraday: Macd
-000216c0: 2048 6973 746f 6772 616d 206e 6567 6174   Histogram negat
-000216d0: 6976 650a 2020 2020 6465 6620 7661 6c69  ive.    def vali
-000216e0: 6461 7465 4d41 4344 4869 7374 6f67 7261  dateMACDHistogra
-000216f0: 6d42 656c 6f77 3028 7365 6c66 2c20 6466  mBelow0(self, df
-00021700: 293a 0a20 2020 2020 2020 2069 6620 6466  ):.        if df
-00021710: 2069 7320 4e6f 6e65 206f 7220 6c65 6e28   is None or len(
-00021720: 6466 2920 3d3d 2030 3a0a 2020 2020 2020  df) == 0:.      
-00021730: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-00021740: 7365 0a20 2020 2020 2020 2064 6174 6120  se.        data 
-00021750: 3d20 6466 2e63 6f70 7928 290a 2020 2020  = df.copy().    
-00021760: 2020 2020 6461 7461 203d 2064 6174 612e      data = data.
-00021770: 6669 6c6c 6e61 2830 290a 2020 2020 2020  fillna(0).      
-00021780: 2020 6461 7461 203d 2064 6174 612e 7265    data = data.re
-00021790: 706c 6163 6528 5b6e 702e 696e 662c 202d  place([np.inf, -
-000217a0: 6e70 2e69 6e66 5d2c 2030 290a 2020 2020  np.inf], 0).    
-000217b0: 2020 2020 6461 7461 203d 2064 6174 615b      data = data[
-000217c0: 3a3a 2d31 5d20 2023 2052 6576 6572 7365  ::-1]  # Reverse
-000217d0: 2074 6865 2064 6174 6166 7261 6d65 2073   the dataframe s
-000217e0: 6f20 7468 6174 2069 7473 2074 6865 206f  o that its the o
-000217f0: 6c64 6573 7420 6461 7465 2066 6972 7374  ldest date first
-00021800: 0a20 2020 2020 2020 206d 6163 6420 3d20  .        macd = 
-00021810: 706b 7461 6c69 622e 4d41 4344 2864 6174  pktalib.MACD(dat
-00021820: 615b 2243 6c6f 7365 225d 2c20 3132 2c20  a["Close"], 12, 
-00021830: 3236 2c20 3929 5b32 5d2e 7461 696c 2831  26, 9)[2].tail(1
-00021840: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00021850: 206d 6163 642e 696c 6f63 5b3a 315d 5b30   macd.iloc[:1][0
-00021860: 5d20 3c20 300a 0a20 2020 2023 406d 6561  ] < 0..    #@mea
-00021870: 7375 7265 5f74 696d 650a 2020 2020 2320  sure_time.    # 
-00021880: 4669 6e64 2069 6620 7374 6f63 6b20 6761  Find if stock ga
-00021890: 696e 696e 6720 6275 6c6c 6973 6820 6d6f  ining bullish mo
-000218a0: 6d65 6e74 756d 0a20 2020 2064 6566 2076  mentum.    def v
-000218b0: 616c 6964 6174 654d 6f6d 656e 7475 6d28  alidateMomentum(
-000218c0: 7365 6c66 2c20 6466 2c20 7363 7265 656e  self, df, screen
-000218d0: 4469 6374 2c20 7361 7665 4469 6374 293a  Dict, saveDict):
-000218e0: 0a20 2020 2020 2020 2069 6620 6466 2069  .        if df i
-000218f0: 7320 4e6f 6e65 206f 7220 6c65 6e28 6466  s None or len(df
-00021900: 2920 3d3d 2030 3a0a 2020 2020 2020 2020  ) == 0:.        
-00021910: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-00021920: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
-00021930: 6466 2e63 6f70 7928 290a 2020 2020 2020  df.copy().      
-00021940: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-00021950: 2020 2064 6174 6120 3d20 6461 7461 2e68     data = data.h
-00021960: 6561 6428 3329 0a20 2020 2020 2020 2020  ead(3).         
-00021970: 2020 2069 6620 6c65 6e28 6461 7461 2920     if len(data) 
-00021980: 3c20 333a 0a20 2020 2020 2020 2020 2020  < 3:.           
-00021990: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-000219a0: 650a 2020 2020 2020 2020 2020 2020 666f  e.            fo
-000219b0: 7220 726f 7720 696e 2064 6174 612e 6974  r row in data.it
-000219c0: 6572 726f 7773 2829 3a0a 2020 2020 2020  errows():.      
-000219d0: 2020 2020 2020 2020 2020 2320 416c 6c20            # All 
-000219e0: 3320 6361 6e64 6c65 7320 7368 6f75 6c64  3 candles should
-000219f0: 2062 6520 4772 6565 6e20 616e 6420 4e4f   be Green and NO
-00021a00: 5420 4369 7263 7569 7473 0a20 2020 2020  T Circuits.     
-00021a10: 2020 2020 2020 2020 2020 2079 6320 3d20             yc = 
-00021a20: 726f 775b 315d 5b22 436c 6f73 6522 5d0a  row[1]["Close"].
-00021a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021a40: 796f 203d 2072 6f77 5b31 5d5b 224f 7065  yo = row[1]["Ope
-00021a50: 6e22 5d0a 2020 2020 2020 2020 2020 2020  n"].            
-00021a60: 2020 2020 6966 2079 6320 3c3d 2079 6f3a      if yc <= yo:
-00021a70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00021a80: 2020 2020 2023 2073 656c 662e 6465 6661       # self.defa
-00021a90: 756c 745f 6c6f 6767 6572 2e69 6e66 6f28  ult_logger.info(
-00021aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00021ab0: 2020 2020 2023 2020 2020 2066 2753 746f       #     f'Sto
-00021ac0: 636b 3a7b 7361 7665 4469 6374 5b22 5374  ck:{saveDict["St
-00021ad0: 6f63 6b22 5d7d 2c20 6973 206e 6f74 2061  ock"]}, is not a
-00021ae0: 206d 6f6d 656e 7475 6d2d 6761 696e 6572   momentum-gainer
-00021af0: 2062 6563 6175 7365 2079 6573 7465 7264   because yesterd
-00021b00: 6179 2d63 6c6f 7365 2028 7b79 637d 2920  ay-close ({yc}) 
-00021b10: 3c3d 2079 6573 7465 7264 6179 2d6f 7065  <= yesterday-ope
-00021b20: 6e20 287b 796f 7d29 270a 2020 2020 2020  n ({yo})'.      
-00021b30: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00021b40: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00021b50: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-00021b60: 7365 0a20 2020 2020 2020 2020 2020 206f  se.            o
-00021b70: 7065 6e44 6573 6320 3d20 6461 7461 2e73  penDesc = data.s
-00021b80: 6f72 745f 7661 6c75 6573 2862 793d 5b22  ort_values(by=["
-00021b90: 4f70 656e 225d 2c20 6173 6365 6e64 696e  Open"], ascendin
-00021ba0: 673d 4661 6c73 6529 0a20 2020 2020 2020  g=False).       
-00021bb0: 2020 2020 2063 6c6f 7365 4465 7363 203d       closeDesc =
-00021bc0: 2064 6174 612e 736f 7274 5f76 616c 7565   data.sort_value
-00021bd0: 7328 6279 3d5b 2243 6c6f 7365 225d 2c20  s(by=["Close"], 
-00021be0: 6173 6365 6e64 696e 673d 4661 6c73 6529  ascending=False)
-00021bf0: 0a20 2020 2020 2020 2020 2020 2076 6f6c  .            vol
-00021c00: 4465 7363 203d 2064 6174 612e 736f 7274  Desc = data.sort
-00021c10: 5f76 616c 7565 7328 6279 3d5b 2256 6f6c  _values(by=["Vol
-00021c20: 756d 6522 5d2c 2061 7363 656e 6469 6e67  ume"], ascending
-00021c30: 3d46 616c 7365 290a 2020 2020 2020 2020  =False).        
-00021c40: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00021c50: 2020 2020 2020 2020 2069 6620 280a 2020           if (.  
-00021c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021c70: 2020 6461 7461 2e65 7175 616c 7328 6f70    data.equals(op
-00021c80: 656e 4465 7363 290a 2020 2020 2020 2020  enDesc).        
-00021c90: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-00021ca0: 6461 7461 2e65 7175 616c 7328 636c 6f73  data.equals(clos
-00021cb0: 6544 6573 6329 0a20 2020 2020 2020 2020  eDesc).         
-00021cc0: 2020 2020 2020 2020 2020 2061 6e64 2064             and d
-00021cd0: 6174 612e 6571 7561 6c73 2876 6f6c 4465  ata.equals(volDe
-00021ce0: 7363 290a 2020 2020 2020 2020 2020 2020  sc).            
-00021cf0: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
-00021d00: 2020 2020 2020 2020 2020 2023 2073 656c             # sel
-00021d10: 662e 6465 6661 756c 745f 6c6f 6767 6572  f.default_logger
-00021d20: 2e69 6e66 6f28 0a20 2020 2020 2020 2020  .info(.         
-00021d30: 2020 2020 2020 2020 2020 2023 2020 2020             #    
-00021d40: 2066 2753 746f 636b 3a7b 7361 7665 4469   f'Stock:{saveDi
-00021d50: 6374 5b22 5374 6f63 6b22 5d7d 2c20 6f70  ct["Stock"]}, op
-00021d60: 656e 2c63 6c6f 7365 2061 6e64 2076 6f6c  en,close and vol
-00021d70: 756d 6520 6571 7561 6c20 6672 6f6d 2064  ume equal from d
-00021d80: 6179 2062 6566 6f72 6520 7965 7374 6572  ay before yester
-00021d90: 6461 792e 2041 2070 6f74 656e 7469 616c  day. A potential
-00021da0: 206d 6f6d 656e 7475 6d2d 6761 696e 6572   momentum-gainer
-00021db0: 2127 0a20 2020 2020 2020 2020 2020 2020  !'.             
-00021dc0: 2020 2020 2020 2023 2029 0a20 2020 2020         # ).     
-00021dd0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00021de0: 6f20 3d20 6461 7461 5b22 4f70 656e 225d  o = data["Open"]
-00021df0: 2e69 6c6f 635b 305d 0a20 2020 2020 2020  .iloc[0].       
-00021e00: 2020 2020 2020 2020 2020 2020 2079 6320               yc 
-00021e10: 3d20 6461 7461 5b22 436c 6f73 6522 5d2e  = data["Close"].
-00021e20: 696c 6f63 5b31 5d0a 2020 2020 2020 2020  iloc[1].        
-00021e30: 2020 2020 2020 2020 2020 2020 796f 203d              yo =
-00021e40: 2064 6174 615b 224f 7065 6e22 5d2e 696c   data["Open"].il
-00021e50: 6f63 5b31 5d0a 2020 2020 2020 2020 2020  oc[1].          
-00021e60: 2020 2020 2020 2020 2020 6479 6320 3d20            dyc = 
-00021e70: 6461 7461 5b22 436c 6f73 6522 5d2e 696c  data["Close"].il
-00021e80: 6f63 5b32 5d0a 2020 2020 2020 2020 2020  oc[2].          
-00021e90: 2020 2020 2020 2020 2020 6966 2028 746f            if (to
-00021ea0: 203e 3d20 7963 2920 616e 6420 2879 6f20   >= yc) and (yo 
-00021eb0: 3e3d 2064 7963 293a 0a20 2020 2020 2020  >= dyc):.       
-00021ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021ed0: 2023 2073 656c 662e 6465 6661 756c 745f   # self.default_
-00021ee0: 6c6f 6767 6572 2e69 6e66 6f28 0a20 2020  logger.info(.   
-00021ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021f00: 2020 2020 2023 2020 2020 2066 2753 746f       #     f'Sto
-00021f10: 636b 3a7b 7361 7665 4469 6374 5b22 5374  ck:{saveDict["St
-00021f20: 6f63 6b22 5d7d 2c20 6973 2061 206d 6f6d  ock"]}, is a mom
-00021f30: 656e 7475 6d2d 6761 696e 6572 2062 6563  entum-gainer bec
-00021f40: 6175 7365 2074 6f64 6179 2d6f 7065 6e20  ause today-open 
-00021f50: 287b 746f 7d29 203e 3d20 7965 7374 6572  ({to}) >= yester
-00021f60: 6461 792d 636c 6f73 6520 287b 7963 7d29  day-close ({yc})
-00021f70: 2061 6e64 2079 6573 7465 7264 6179 2d6f   and yesterday-o
-00021f80: 7065 6e28 7b79 6f7d 2920 3e3d 2064 6179  pen({yo}) >= day
-00021f90: 2d62 6566 6f72 652d 636c 6f73 6528 7b64  -before-close({d
-00021fa0: 7963 7d29 270a 2020 2020 2020 2020 2020  yc})'.          
-00021fb0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00021fc0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00021fd0: 2020 2020 2020 2020 2020 7361 7665 6420            saved 
-00021fe0: 3d20 7365 6c66 2e66 696e 6443 7572 7265  = self.findCurre
-00021ff0: 6e74 5361 7665 6456 616c 7565 2873 6372  ntSavedValue(scr
-00022000: 6565 6e44 6963 742c 2073 6176 6544 6963  eenDict, saveDic
-00022010: 742c 2022 5061 7474 6572 6e22 290a 2020  t, "Pattern").  
-00022020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022030: 2020 2020 2020 7363 7265 656e 4469 6374        screenDict
-00022040: 5b22 5061 7474 6572 6e22 5d20 3d20 280a  ["Pattern"] = (.
-00022050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022060: 2020 2020 2020 2020 2020 2020 7361 7665              save
-00022070: 645b 305d 0a20 2020 2020 2020 2020 2020  d[0].           
-00022080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022090: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
-000220a0: 440a 2020 2020 2020 2020 2020 2020 2020  D.              
-000220b0: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-000220c0: 636f 6c6f 7254 6578 742e 4752 4545 4e0a  colorText.GREEN.
-000220d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000220e0: 2020 2020 2020 2020 2020 2020 2b20 224d              + "M
-000220f0: 6f6d 656e 7475 6d20 4761 696e 6572 220a  omentum Gainer".
-00022100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022110: 2020 2020 2020 2020 2020 2020 2b20 636f              + co
-00022120: 6c6f 7254 6578 742e 454e 440a 2020 2020  lorText.END.    
-00022130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022140: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00022150: 2020 2020 2020 2020 2020 2020 2020 7361                sa
-00022160: 7665 4469 6374 5b22 5061 7474 6572 6e22  veDict["Pattern"
-00022170: 5d20 3d20 7361 7665 645b 315d 202b 2022  ] = saved[1] + "
-00022180: 4d6f 6d65 6e74 756d 2047 6169 6e65 7222  Momentum Gainer"
-00022190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000221a0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000221b0: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
-000221c0: 2020 2020 2020 2020 2023 2073 656c 662e           # self.
-000221d0: 6465 6661 756c 745f 6c6f 6767 6572 2e69  default_logger.i
-000221e0: 6e66 6f28 0a20 2020 2020 2020 2020 2020  nfo(.           
-000221f0: 2020 2020 2020 2020 2023 2020 2020 2066           #     f
-00022200: 2753 746f 636b 3a7b 7361 7665 4469 6374  'Stock:{saveDict
-00022210: 5b22 5374 6f63 6b22 5d7d 2c20 6973 206e  ["Stock"]}, is n
-00022220: 6f74 2061 206d 6f6d 656e 7475 6d2d 6761  ot a momentum-ga
-00022230: 696e 6572 2062 6563 6175 7365 2065 6974  iner because eit
-00022240: 6865 7220 746f 6461 792d 6f70 656e 2028  her today-open (
-00022250: 7b74 6f7d 2920 3c20 7965 7374 6572 6461  {to}) < yesterda
-00022260: 792d 636c 6f73 6520 287b 7963 7d29 206f  y-close ({yc}) o
-00022270: 7220 7965 7374 6572 6461 792d 6f70 656e  r yesterday-open
-00022280: 287b 796f 7d29 203c 2064 6179 2d62 6566  ({yo}) < day-bef
-00022290: 6f72 652d 636c 6f73 6528 7b64 7963 7d29  ore-close({dyc})
-000222a0: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-000222b0: 2020 2020 2020 2320 290a 2020 2020 2020        # ).      
-000222c0: 2020 2020 2020 6578 6365 7074 2049 6e64        except Ind
-000222d0: 6578 4572 726f 7220 6173 2065 3a20 2320  exError as e: # 
-000222e0: 7072 6167 6d61 3a20 6e6f 2063 6f76 6572  pragma: no cover
-000222f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00022300: 2073 656c 662e 6465 6661 756c 745f 6c6f   self.default_lo
-00022310: 6767 6572 2e64 6562 7567 2865 2c20 6578  gger.debug(e, ex
-00022320: 635f 696e 666f 3d54 7275 6529 0a20 2020  c_info=True).   
-00022330: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00022340: 662e 6465 6661 756c 745f 6c6f 6767 6572  f.default_logger
-00022350: 2e64 6562 7567 2864 6174 6129 0a20 2020  .debug(data).   
-00022360: 2020 2020 2020 2020 2020 2020 2070 6173               pas
-00022370: 730a 2020 2020 2020 2020 2020 2020 7265  s.            re
-00022380: 7475 726e 2046 616c 7365 0a20 2020 2020  turn False.     
-00022390: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-000223a0: 696f 6e20 6173 2065 3a20 2023 2070 7261  ion as e:  # pra
-000223b0: 676d 613a 206e 6f20 636f 7665 720a 2020  gma: no cover.  
-000223c0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-000223d0: 6566 6175 6c74 5f6c 6f67 6765 722e 6465  efault_logger.de
-000223e0: 6275 6728 652c 2065 7863 5f69 6e66 6f3d  bug(e, exc_info=
-000223f0: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
-00022400: 2020 7265 7475 726e 2046 616c 7365 0a0a    return False..
-00022410: 2020 2020 2340 6d65 6173 7572 655f 7469      #@measure_ti
-00022420: 6d65 0a20 2020 2023 2056 616c 6964 6174  me.    # Validat
-00022430: 6520 4d6f 7669 6e67 2061 7665 7261 6765  e Moving average
-00022440: 7320 616e 6420 6c6f 6f6b 2066 6f72 2062  s and look for b
-00022450: 7579 2f73 656c 6c20 7369 676e 616c 730a  uy/sell signals.
-00022460: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-00022470: 4d6f 7669 6e67 4176 6572 6167 6573 2873  MovingAverages(s
-00022480: 656c 662c 2064 662c 2073 6372 6565 6e44  elf, df, screenD
-00022490: 6963 742c 2073 6176 6544 6963 742c 206d  ict, saveDict, m
-000224a0: 6152 616e 6765 3d32 2e35 2c6d 614c 656e  aRange=2.5,maLen
-000224b0: 6774 683d 3029 3a0a 2020 2020 2020 2020  gth=0):.        
-000224c0: 6461 7461 203d 2064 662e 636f 7079 2829  data = df.copy()
-000224d0: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
-000224e0: 6461 7461 2e66 696c 6c6e 6128 3029 0a20  data.fillna(0). 
-000224f0: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
-00022500: 7461 2e72 6570 6c61 6365 285b 6e70 2e69  ta.replace([np.i
-00022510: 6e66 2c20 2d6e 702e 696e 665d 2c20 3029  nf, -np.inf], 0)
-00022520: 0a20 2020 2020 2020 2072 6563 656e 7420  .        recent 
-00022530: 3d20 6461 7461 2e68 6561 6428 3129 0a20  = data.head(1). 
-00022540: 2020 2020 2020 206d 6153 6967 6e61 6c73         maSignals
-00022550: 203d 205b 5d0a 2020 2020 2020 2020 6966   = [].        if
-00022560: 2073 7472 286d 614c 656e 6774 6829 2069   str(maLength) i
-00022570: 6e20 5b22 3022 2c22 3222 2c22 3322 5d3a  n ["0","2","3"]:
-00022580: 0a20 2020 2020 2020 2020 2020 2073 6176  .            sav
-00022590: 6564 203d 2073 656c 662e 6669 6e64 4375  ed = self.findCu
-000225a0: 7272 656e 7453 6176 6564 5661 6c75 6528  rrentSavedValue(
-000225b0: 7363 7265 656e 4469 6374 2c73 6176 6544  screenDict,saveD
-000225c0: 6963 742c 224d 412d 5369 676e 616c 2229  ict,"MA-Signal")
-000225d0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000225e0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000225f0: 2020 7265 6365 6e74 5b22 534d 4122 5d2e    recent["SMA"].
-00022600: 696c 6f63 5b30 5d20 3e20 7265 6365 6e74  iloc[0] > recent
-00022610: 5b22 4c4d 4122 5d2e 696c 6f63 5b30 5d0a  ["LMA"].iloc[0].
-00022620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022630: 616e 6420 7265 6365 6e74 5b22 436c 6f73  and recent["Clos
-00022640: 6522 5d2e 696c 6f63 5b30 5d20 3e20 7265  e"].iloc[0] > re
-00022650: 6365 6e74 5b22 534d 4122 5d2e 696c 6f63  cent["SMA"].iloc
-00022660: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
-00022670: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00022680: 2020 2073 6372 6565 6e44 6963 745b 224d     screenDict["M
-00022690: 412d 5369 676e 616c 225d 203d 2028 0a20  A-Signal"] = (. 
-000226a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000226b0: 2020 2073 6176 6564 5b30 5d20 2b20 636f     saved[0] + co
-000226c0: 6c6f 7254 6578 742e 424f 4c44 202b 2063  lorText.BOLD + c
-000226d0: 6f6c 6f72 5465 7874 2e47 5245 454e 202b  olorText.GREEN +
-000226e0: 2022 4275 6c6c 6973 6822 202b 2063 6f6c   "Bullish" + col
-000226f0: 6f72 5465 7874 2e45 4e44 0a20 2020 2020  orText.END.     
-00022700: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00022710: 2020 2020 2020 2020 2020 2020 2073 6176               sav
-00022720: 6544 6963 745b 224d 412d 5369 676e 616c  eDict["MA-Signal
-00022730: 225d 203d 2073 6176 6564 5b31 5d20 2b20  "] = saved[1] + 
-00022740: 2242 756c 6c69 7368 220a 2020 2020 2020  "Bullish".      
-00022750: 2020 2020 2020 2020 2020 6d61 5369 676e            maSign
-00022760: 616c 732e 6170 7065 6e64 2822 3322 290a  als.append("3").
-00022770: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-00022780: 2072 6563 656e 745b 2253 4d41 225d 2e69   recent["SMA"].i
-00022790: 6c6f 635b 305d 203c 2072 6563 656e 745b  loc[0] < recent[
-000227a0: 224c 4d41 225d 2e69 6c6f 635b 305d 3a0a  "LMA"].iloc[0]:.
-000227b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000227c0: 7363 7265 656e 4469 6374 5b22 4d41 2d53  screenDict["MA-S
-000227d0: 6967 6e61 6c22 5d20 3d20 280a 2020 2020  ignal"] = (.    
-000227e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000227f0: 7361 7665 645b 305d 202b 2063 6f6c 6f72  saved[0] + color
-00022800: 5465 7874 2e42 4f4c 4420 2b20 636f 6c6f  Text.BOLD + colo
-00022810: 7254 6578 742e 4641 494c 202b 2022 4265  rText.FAIL + "Be
-00022820: 6172 6973 6822 202b 2063 6f6c 6f72 5465  arish" + colorTe
-00022830: 7874 2e45 4e44 0a20 2020 2020 2020 2020  xt.END.         
-00022840: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00022850: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
-00022860: 745b 224d 412d 5369 676e 616c 225d 203d  t["MA-Signal"] =
-00022870: 2073 6176 6564 5b31 5d20 2b20 2242 6561   saved[1] + "Bea
-00022880: 7269 7368 220a 2020 2020 2020 2020 2020  rish".          
-00022890: 2020 2020 2020 6d61 5369 676e 616c 732e        maSignals.
-000228a0: 6170 7065 6e64 2822 3222 290a 2020 2020  append("2").    
-000228b0: 2020 2020 2020 2020 656c 6966 2072 6563          elif rec
-000228c0: 656e 745b 2253 4d41 225d 2e69 6c6f 635b  ent["SMA"].iloc[
-000228d0: 305d 203d 3d20 303a 0a20 2020 2020 2020  0] == 0:.       
-000228e0: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
-000228f0: 6963 745b 224d 412d 5369 676e 616c 225d  ict["MA-Signal"]
-00022900: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
-00022910: 2020 2020 2020 2020 2073 6176 6564 5b30           saved[0
-00022920: 5d20 2b20 636f 6c6f 7254 6578 742e 424f  ] + colorText.BO
-00022930: 4c44 202b 2063 6f6c 6f72 5465 7874 2e57  LD + colorText.W
-00022940: 4152 4e20 2b20 2255 6e6b 6e6f 776e 2220  ARN + "Unknown" 
-00022950: 2b20 636f 6c6f 7254 6578 742e 454e 440a  + colorText.END.
-00022960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022970: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00022980: 2020 7361 7665 4469 6374 5b22 4d41 2d53    saveDict["MA-S
-00022990: 6967 6e61 6c22 5d20 3d20 7361 7665 645b  ignal"] = saved[
-000229a0: 315d 202b 2022 556e 6b6e 6f77 6e22 0a20  1] + "Unknown". 
-000229b0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-000229c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000229d0: 2073 6372 6565 6e44 6963 745b 224d 412d   screenDict["MA-
-000229e0: 5369 676e 616c 225d 203d 2028 0a20 2020  Signal"] = (.   
-000229f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022a00: 2073 6176 6564 5b30 5d20 2b20 636f 6c6f   saved[0] + colo
-00022a10: 7254 6578 742e 424f 4c44 202b 2063 6f6c  rText.BOLD + col
-00022a20: 6f72 5465 7874 2e57 4152 4e20 2b20 224e  orText.WARN + "N
-00022a30: 6575 7472 616c 2220 2b20 636f 6c6f 7254  eutral" + colorT
-00022a40: 6578 742e 454e 440a 2020 2020 2020 2020  ext.END.        
-00022a50: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00022a60: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
-00022a70: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d20  ct["MA-Signal"] 
-00022a80: 3d20 7361 7665 645b 315d 202b 2022 4e65  = saved[1] + "Ne
-00022a90: 7574 7261 6c22 0a20 2020 2020 2020 2072  utral".        r
-00022aa0: 6576 6572 7365 6444 6174 6120 3d20 6461  eversedData = da
-00022ab0: 7461 5b3a 3a2d 315d 2020 2320 5265 7665  ta[::-1]  # Reve
-00022ac0: 7273 6520 7468 6520 6461 7461 6672 616d  rse the datafram
-00022ad0: 650a 2020 2020 2020 2020 656d 615f 3230  e.        ema_20
-00022ae0: 203d 2070 6b74 616c 6962 2e45 4d41 2872   = pktalib.EMA(r
-00022af0: 6576 6572 7365 6444 6174 615b 2243 6c6f  eversedData["Clo
-00022b00: 7365 225d 2c32 3029 2e74 6169 6c28 3129  se"],20).tail(1)
-00022b10: 2e69 6c6f 635b 305d 0a20 2020 2020 2020  .iloc[0].       
-00022b20: 2076 7761 7020 3d20 706b 7461 6c69 622e   vwap = pktalib.
-00022b30: 5657 4150 2872 6576 6572 7365 6444 6174  VWAP(reversedDat
-00022b40: 615b 2248 6967 6822 5d2c 7265 7665 7273  a["High"],revers
-00022b50: 6564 4461 7461 5b22 4c6f 7722 5d2c 7265  edData["Low"],re
-00022b60: 7665 7273 6564 4461 7461 5b22 436c 6f73  versedData["Clos
-00022b70: 6522 5d2c 7265 7665 7273 6564 4461 7461  e"],reversedData
-00022b80: 5b22 566f 6c75 6d65 225d 292e 7461 696c  ["Volume"]).tail
-00022b90: 2831 292e 696c 6f63 5b30 5d0a 2020 2020  (1).iloc[0].    
-00022ba0: 2020 2020 736d 6144 6576 203d 2064 6174      smaDev = dat
-00022bb0: 615b 2253 4d41 225d 2e69 6c6f 635b 305d  a["SMA"].iloc[0]
-00022bc0: 202a 206d 6152 616e 6765 202f 2031 3030   * maRange / 100
-00022bd0: 0a20 2020 2020 2020 206c 6d61 4465 7620  .        lmaDev 
-00022be0: 3d20 6461 7461 5b22 4c4d 4122 5d2e 696c  = data["LMA"].il
-00022bf0: 6f63 5b30 5d20 2a20 6d61 5261 6e67 6520  oc[0] * maRange 
-00022c00: 2f20 3130 300a 2020 2020 2020 2020 656d  / 100.        em
-00022c10: 6144 6576 203d 2065 6d61 5f32 3020 2a20  aDev = ema_20 * 
-00022c20: 6d61 5261 6e67 6520 2f20 3130 300a 2020  maRange / 100.  
-00022c30: 2020 2020 2020 7677 6170 4465 7620 3d20        vwapDev = 
-00022c40: 7677 6170 202a 206d 6152 616e 6765 202f  vwap * maRange /
-00022c50: 2031 3030 0a20 2020 2020 2020 206f 7065   100.        ope
-00022c60: 6e2c 2068 6967 682c 206c 6f77 2c20 636c  n, high, low, cl
-00022c70: 6f73 652c 2073 6d61 2c20 6c6d 6120 3d20  ose, sma, lma = 
-00022c80: 280a 2020 2020 2020 2020 2020 2020 6461  (.            da
-00022c90: 7461 5b22 4f70 656e 225d 2e69 6c6f 635b  ta["Open"].iloc[
-00022ca0: 305d 2c0a 2020 2020 2020 2020 2020 2020  0],.            
-00022cb0: 6461 7461 5b22 4869 6768 225d 2e69 6c6f  data["High"].ilo
-00022cc0: 635b 305d 2c0a 2020 2020 2020 2020 2020  c[0],.          
-00022cd0: 2020 6461 7461 5b22 4c6f 7722 5d2e 696c    data["Low"].il
-00022ce0: 6f63 5b30 5d2c 0a20 2020 2020 2020 2020  oc[0],.         
-00022cf0: 2020 2064 6174 615b 2243 6c6f 7365 225d     data["Close"]
-00022d00: 2e69 6c6f 635b 305d 2c0a 2020 2020 2020  .iloc[0],.      
-00022d10: 2020 2020 2020 6461 7461 5b22 534d 4122        data["SMA"
-00022d20: 5d2e 696c 6f63 5b30 5d2c 0a20 2020 2020  ].iloc[0],.     
-00022d30: 2020 2020 2020 2064 6174 615b 224c 4d41         data["LMA
-00022d40: 225d 2e69 6c6f 635b 305d 2c0a 2020 2020  "].iloc[0],.    
-00022d50: 2020 2020 290a 2020 2020 2020 2020 6d61      ).        ma
-00022d60: 7320 3d20 5b73 6d61 2c6c 6d61 2c65 6d61  s = [sma,lma,ema
-00022d70: 5f32 302c 7677 6170 5d20 6966 206d 614c  _20,vwap] if maL
-00022d80: 656e 6774 683d 3d30 2065 6c73 6520 5b73  ength==0 else [s
-00022d90: 6d61 2c6c 6d61 2c65 6d61 5f32 305d 0a20  ma,lma,ema_20]. 
-00022da0: 2020 2020 2020 206d 6144 6576 7320 3d20         maDevs = 
-00022db0: 5b73 6d61 4465 762c 206c 6d61 4465 762c  [smaDev, lmaDev,
-00022dc0: 2065 6d61 4465 762c 2076 7761 7044 6576   emaDev, vwapDev
-00022dd0: 5d20 6966 206d 614c 656e 6774 683d 3d30  ] if maLength==0
-00022de0: 2065 6c73 6520 5b73 6d61 4465 762c 206c   else [smaDev, l
-00022df0: 6d61 4465 762c 2065 6d61 4465 765d 0a20  maDev, emaDev]. 
-00022e00: 2020 2020 2020 206d 6154 6578 7473 203d         maTexts =
-00022e10: 205b 2235 304d 4122 2c22 3230 304d 4122   ["50MA","200MA"
-00022e20: 2c22 3230 454d 4122 2c22 5657 4150 225d  ,"20EMA","VWAP"]
-00022e30: 2069 6620 6d61 4c65 6e67 7468 3d3d 3020   if maLength==0 
-00022e40: 656c 7365 205b 2235 304d 4122 2c22 3230  else ["50MA","20
-00022e50: 304d 4122 2c22 3230 454d 4122 5d0a 2020  0MA","20EMA"].  
-00022e60: 2020 2020 2020 6d61 5265 7665 7273 616c        maReversal
-00022e70: 203d 2030 0a20 2020 2020 2020 2069 6e64   = 0.        ind
-00022e80: 6578 203d 2030 0a20 2020 2020 2020 2062  ex = 0.        b
-00022e90: 756c 6c69 7368 4361 6e64 6c65 203d 2073  ullishCandle = s
-00022ea0: 656c 662e 6765 7443 616e 646c 6554 7970  elf.getCandleTyp
-00022eb0: 6528 6461 7461 290a 2020 2020 2020 2020  e(data).        
-00022ec0: 6966 2073 7472 286d 614c 656e 6774 6829  if str(maLength)
-00022ed0: 206e 6f74 2069 6e20 5b22 3222 2c22 3322   not in ["2","3"
-00022ee0: 5d3a 0a20 2020 2020 2020 2020 2020 2066  ]:.            f
-00022ef0: 6f72 206d 6120 696e 206d 6173 3a0a 2020  or ma in mas:.  
-00022f00: 2020 2020 2020 2020 2020 2020 2020 7361                sa
-00022f10: 7665 6420 3d20 7365 6c66 2e66 696e 6443  ved = self.findC
-00022f20: 7572 7265 6e74 5361 7665 6456 616c 7565  urrentSavedValue
-00022f30: 2873 6372 6565 6e44 6963 742c 7361 7665  (screenDict,save
-00022f40: 4469 6374 2c22 4d41 2d53 6967 6e61 6c22  Dict,"MA-Signal"
-00022f50: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00022f60: 2020 2320 5461 6b69 6e67 2053 7570 706f    # Taking Suppo
-00022f70: 7274 0a20 2020 2020 2020 2020 2020 2020  rt.             
-00022f80: 2020 2069 6620 636c 6f73 6520 3e20 6d61     if close > ma
-00022f90: 2061 6e64 206c 6f77 203c 3d20 286d 6120   and low <= (ma 
-00022fa0: 2b20 6d61 4465 7673 5b69 6e64 6578 5d29  + maDevs[index])
-00022fb0: 2061 6e64 2073 7472 286d 614c 656e 6774   and str(maLengt
-00022fc0: 6829 2069 6e20 5b22 3022 2c22 3122 5d3a  h) in ["0","1"]:
-00022fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00022fe0: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
-00022ff0: 224d 412d 5369 676e 616c 225d 203d 2028  "MA-Signal"] = (
-00023000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00023010: 2020 2020 2020 2020 2073 6176 6564 5b30           saved[0
-00023020: 5d20 2b20 636f 6c6f 7254 6578 742e 424f  ] + colorText.BO
-00023030: 4c44 202b 2063 6f6c 6f72 5465 7874 2e47  LD + colorText.G
-00023040: 5245 454e 202b 2066 227b 6d61 5465 7874  REEN + f"{maText
-00023050: 735b 696e 6465 785d 7d2d 5375 7070 6f72  s[index]}-Suppor
-00023060: 7422 202b 2063 6f6c 6f72 5465 7874 2e45  t" + colorText.E
-00023070: 4e44 0a20 2020 2020 2020 2020 2020 2020  ND.             
-00023080: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00023090: 2020 2020 2020 2020 2020 2020 2073 6176               sav
-000230a0: 6544 6963 745b 224d 412d 5369 676e 616c  eDict["MA-Signal
-000230b0: 225d 203d 2073 6176 6564 5b31 5d20 2b20  "] = saved[1] + 
-000230c0: 6622 7b6d 6154 6578 7473 5b69 6e64 6578  f"{maTexts[index
-000230d0: 5d7d 2d53 7570 706f 7274 220a 2020 2020  ]}-Support".    
-000230e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000230f0: 6d61 5265 7665 7273 616c 203d 2031 0a20  maReversal = 1. 
-00023100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023110: 2020 206d 6153 6967 6e61 6c73 2e61 7070     maSignals.app
-00023120: 656e 6428 2231 2229 0a20 2020 2020 2020  end("1").       
-00023130: 2020 2020 2020 2020 2023 2056 616c 6964           # Valid
-00023140: 6174 696e 6720 5265 7369 7374 616e 6365  ating Resistance
-00023150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00023160: 2065 6c69 6620 636c 6f73 6520 3c20 6d61   elif close < ma
-00023170: 2061 6e64 2068 6967 6820 3e3d 2028 6d61   and high >= (ma
-00023180: 202d 206d 6144 6576 735b 696e 6465 785d   - maDevs[index]
-00023190: 2920 616e 6420 7374 7228 6d61 4c65 6e67  ) and str(maLeng
-000231a0: 7468 2920 696e 205b 2230 222c 2236 225d  th) in ["0","6"]
-000231b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000231c0: 2020 2020 2020 7363 7265 656e 4469 6374        screenDict
-000231d0: 5b22 4d41 2d53 6967 6e61 6c22 5d20 3d20  ["MA-Signal"] = 
-000231e0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000231f0: 2020 2020 2020 2020 2020 7361 7665 645b            saved[
-00023200: 305d 202b 2063 6f6c 6f72 5465 7874 2e42  0] + colorText.B
-00023210: 4f4c 4420 2b20 636f 6c6f 7254 6578 742e  OLD + colorText.
-00023220: 4641 494c 202b 2066 227b 6d61 5465 7874  FAIL + f"{maText
-00023230: 735b 696e 6465 785d 7d2d 5265 7369 7374  s[index]}-Resist
-00023240: 2220 2b20 636f 6c6f 7254 6578 742e 454e  " + colorText.EN
-00023250: 440a 2020 2020 2020 2020 2020 2020 2020  D.              
-00023260: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00023270: 2020 2020 2020 2020 2020 2020 7361 7665              save
-00023280: 4469 6374 5b22 4d41 2d53 6967 6e61 6c22  Dict["MA-Signal"
-00023290: 5d20 3d20 7361 7665 645b 315d 202b 2066  ] = saved[1] + f
-000232a0: 227b 6d61 5465 7874 735b 696e 6465 785d  "{maTexts[index]
-000232b0: 7d2d 5265 7369 7374 220a 2020 2020 2020  }-Resist".      
-000232c0: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-000232d0: 5265 7665 7273 616c 203d 202d 310a 2020  Reversal = -1.  
-000232e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000232f0: 2020 6d61 5369 676e 616c 732e 6170 7065    maSignals.appe
-00023300: 6e64 2822 3622 290a 2020 2020 2020 2020  nd("6").        
-00023310: 2020 2020 2020 2020 2320 466f 7220 6120          # For a 
-00023320: 4275 6c6c 6973 6820 4361 6e64 6c65 0a20  Bullish Candle. 
-00023330: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00023340: 6620 6275 6c6c 6973 6843 616e 646c 653a  f bullishCandle:
+00021570: 2020 2020 2020 2069 6620 2870 7264 203d         if (prd =
+00021580: 3d20 7265 7175 6573 7465 6450 6572 696f  = requestedPerio
+00021590: 6429 3a0a 2020 2020 2020 2020 2020 2020  d):.            
+000215a0: 2020 2020 2020 2020 2020 2020 6d61 784c              maxL
+000215b0: 5450 506f 7465 6e74 6961 6c20 3d20 6d61  TPPotential = ma
+000215c0: 7828 6461 7461 5b22 4869 6768 225d 2e68  x(data["High"].h
+000215d0: 6561 6428 7072 6429 290a 2020 2020 2020  ead(prd)).      
+000215e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000215f0: 2020 7363 7265 656e 4469 6374 5b66 224d    screenDict[f"M
+00021600: 6178 4c54 5022 5d20 3d20 280a 2020 2020  axLTP"] = (.    
+00021610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021620: 2020 2020 2020 2020 2863 6f6c 6f72 5465          (colorTe
+00021630: 7874 2e47 5245 454e 2069 6620 286d 6178  xt.GREEN if (max
+00021640: 4c54 5050 6f74 656e 7469 616c 203e 3d20  LTPPotential >= 
+00021650: 7072 6576 4c74 7029 2065 6c73 6520 2863  prevLtp) else (c
+00021660: 6f6c 6f72 5465 7874 2e46 4149 4c29 290a  olorText.FAIL)).
+00021670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021680: 2020 2020 2020 2020 2020 2020 2b20 7374              + st
+00021690: 7228 227b 3a2e 3266 7d22 2e66 6f72 6d61  r("{:.2f}".forma
+000216a0: 7428 6d61 784c 5450 506f 7465 6e74 6961  t(maxLTPPotentia
+000216b0: 6c29 290a 2020 2020 2020 2020 2020 2020  l)).            
+000216c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000216d0: 2b20 636f 6c6f 7254 6578 742e 454e 440a  + colorText.END.
+000216e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000216f0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00021700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021710: 2020 7363 7265 656e 4469 6374 5b66 2250    screenDict[f"P
+00021720: 6f74 2e47 7277 225d 203d 2028 0a20 2020  ot.Grw"] = (.   
+00021730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021740: 2020 2020 2020 2020 2028 636f 6c6f 7254           (colorT
+00021750: 6578 742e 4752 4545 4e20 6966 2028 6d61  ext.GREEN if (ma
+00021760: 784c 5450 506f 7465 6e74 6961 6c20 3e3d  xLTPPotential >=
+00021770: 2070 7265 764c 7470 2920 656c 7365 2028   prevLtp) else (
+00021780: 636f 6c6f 7254 6578 742e 4641 494c 2929  colorText.FAIL))
+00021790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000217a0: 2020 2020 2020 2020 2020 2020 202b 2073               + s
+000217b0: 7472 2822 7b3a 2e32 667d 2522 2e66 6f72  tr("{:.2f}%".for
+000217c0: 6d61 7428 286d 6178 4c54 5050 6f74 656e  mat((maxLTPPoten
+000217d0: 7469 616c 202d 2070 7265 764c 7470 292a  tial - prevLtp)*
+000217e0: 3130 302f 7072 6576 4c74 7029 290a 2020  100/prevLtp)).  
+000217f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021800: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
+00021810: 7254 6578 742e 454e 440a 2020 2020 2020  rText.END.      
+00021820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021830: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00021840: 2020 2020 2020 2020 2020 2020 7361 7665              save
+00021850: 4469 6374 5b66 224d 6178 4c54 5022 5d20  Dict[f"MaxLTP"] 
+00021860: 3d20 726f 756e 6428 6d61 784c 5450 506f  = round(maxLTPPo
+00021870: 7465 6e74 6961 6c2c 2032 290a 2020 2020  tential, 2).    
+00021880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021890: 2020 2020 7361 7665 4469 6374 5b66 2250      saveDict[f"P
+000218a0: 6f74 2e47 7277 225d 203d 2066 227b 726f  ot.Grw"] = f"{ro
+000218b0: 756e 6428 286d 6178 4c54 5050 6f74 656e  und((maxLTPPoten
+000218c0: 7469 616c 202d 2070 7265 764c 7470 292a  tial - prevLtp)*
+000218d0: 3130 302f 7072 6576 4c74 702c 2032 297d  100/prevLtp, 2)}
+000218e0: 2522 0a20 2020 2020 2020 2020 2020 2020  %".             
+000218f0: 2020 2073 6372 6565 6e44 6963 745b 2244     screenDict["D
+00021900: 6174 6522 5d20 3d20 6361 6c63 5f64 6174  ate"] = calc_dat
+00021910: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00021920: 2020 7361 7665 4469 6374 5b22 4461 7465    saveDict["Date
+00021930: 225d 203d 2063 616c 635f 6461 7465 0a20  "] = calc_date. 
+00021940: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00021950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00021960: 2073 6176 6544 6963 745b 6622 4c54 507b   saveDict[f"LTP{
+00021970: 7072 647d 225d 203d 206e 702e 6e61 6e0a  prd}"] = np.nan.
+00021980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021990: 7361 7665 4469 6374 5b66 2247 726f 7774  saveDict[f"Growt
+000219a0: 687b 7072 647d 225d 203d 206e 702e 6e61  h{prd}"] = np.na
+000219b0: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
+000219c0: 2020 7363 7265 656e 4469 6374 5b22 4461    screenDict["Da
+000219d0: 7465 225d 203d 2063 616c 635f 6461 7465  te"] = calc_date
+000219e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000219f0: 2073 6176 6544 6963 745b 2244 6174 6522   saveDict["Date"
+00021a00: 5d20 3d20 6361 6c63 5f64 6174 650a 0a20  ] = calc_date.. 
+00021a10: 2020 2023 2046 696e 6420 7374 6f63 6b73     # Find stocks
+00021a20: 2074 6861 7420 6172 6520 6265 6172 6973   that are bearis
+00021a30: 6820 696e 7472 6164 6179 3a20 4d61 6364  h intraday: Macd
+00021a40: 2048 6973 746f 6772 616d 206e 6567 6174   Histogram negat
+00021a50: 6976 650a 2020 2020 6465 6620 7661 6c69  ive.    def vali
+00021a60: 6461 7465 4d41 4344 4869 7374 6f67 7261  dateMACDHistogra
+00021a70: 6d42 656c 6f77 3028 7365 6c66 2c20 6466  mBelow0(self, df
+00021a80: 293a 0a20 2020 2020 2020 2069 6620 6466  ):.        if df
+00021a90: 2069 7320 4e6f 6e65 206f 7220 6c65 6e28   is None or len(
+00021aa0: 6466 2920 3d3d 2030 3a0a 2020 2020 2020  df) == 0:.      
+00021ab0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+00021ac0: 7365 0a20 2020 2020 2020 2064 6174 6120  se.        data 
+00021ad0: 3d20 6466 2e63 6f70 7928 290a 2020 2020  = df.copy().    
+00021ae0: 2020 2020 6461 7461 203d 2064 6174 612e      data = data.
+00021af0: 6669 6c6c 6e61 2830 290a 2020 2020 2020  fillna(0).      
+00021b00: 2020 6461 7461 203d 2064 6174 612e 7265    data = data.re
+00021b10: 706c 6163 6528 5b6e 702e 696e 662c 202d  place([np.inf, -
+00021b20: 6e70 2e69 6e66 5d2c 2030 290a 2020 2020  np.inf], 0).    
+00021b30: 2020 2020 6461 7461 203d 2064 6174 615b      data = data[
+00021b40: 3a3a 2d31 5d20 2023 2052 6576 6572 7365  ::-1]  # Reverse
+00021b50: 2074 6865 2064 6174 6166 7261 6d65 2073   the dataframe s
+00021b60: 6f20 7468 6174 2069 7473 2074 6865 206f  o that its the o
+00021b70: 6c64 6573 7420 6461 7465 2066 6972 7374  ldest date first
+00021b80: 0a20 2020 2020 2020 206d 6163 6420 3d20  .        macd = 
+00021b90: 706b 7461 6c69 622e 4d41 4344 2864 6174  pktalib.MACD(dat
+00021ba0: 615b 2243 6c6f 7365 225d 2c20 3132 2c20  a["Close"], 12, 
+00021bb0: 3236 2c20 3929 5b32 5d2e 7461 696c 2831  26, 9)[2].tail(1
+00021bc0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00021bd0: 206d 6163 642e 696c 6f63 5b3a 315d 5b30   macd.iloc[:1][0
+00021be0: 5d20 3c20 300a 0a20 2020 2023 406d 6561  ] < 0..    #@mea
+00021bf0: 7375 7265 5f74 696d 650a 2020 2020 2320  sure_time.    # 
+00021c00: 4669 6e64 2069 6620 7374 6f63 6b20 6761  Find if stock ga
+00021c10: 696e 696e 6720 6275 6c6c 6973 6820 6d6f  ining bullish mo
+00021c20: 6d65 6e74 756d 0a20 2020 2064 6566 2076  mentum.    def v
+00021c30: 616c 6964 6174 654d 6f6d 656e 7475 6d28  alidateMomentum(
+00021c40: 7365 6c66 2c20 6466 2c20 7363 7265 656e  self, df, screen
+00021c50: 4469 6374 2c20 7361 7665 4469 6374 293a  Dict, saveDict):
+00021c60: 0a20 2020 2020 2020 2069 6620 6466 2069  .        if df i
+00021c70: 7320 4e6f 6e65 206f 7220 6c65 6e28 6466  s None or len(df
+00021c80: 2920 3d3d 2030 3a0a 2020 2020 2020 2020  ) == 0:.        
+00021c90: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+00021ca0: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
+00021cb0: 6466 2e63 6f70 7928 290a 2020 2020 2020  df.copy().      
+00021cc0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+00021cd0: 2020 2064 6174 6120 3d20 6461 7461 2e68     data = data.h
+00021ce0: 6561 6428 3329 0a20 2020 2020 2020 2020  ead(3).         
+00021cf0: 2020 2069 6620 6c65 6e28 6461 7461 2920     if len(data) 
+00021d00: 3c20 333a 0a20 2020 2020 2020 2020 2020  < 3:.           
+00021d10: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00021d20: 650a 2020 2020 2020 2020 2020 2020 666f  e.            fo
+00021d30: 7220 726f 7720 696e 2064 6174 612e 6974  r row in data.it
+00021d40: 6572 726f 7773 2829 3a0a 2020 2020 2020  errows():.      
+00021d50: 2020 2020 2020 2020 2020 2320 416c 6c20            # All 
+00021d60: 3320 6361 6e64 6c65 7320 7368 6f75 6c64  3 candles should
+00021d70: 2062 6520 4772 6565 6e20 616e 6420 4e4f   be Green and NO
+00021d80: 5420 4369 7263 7569 7473 0a20 2020 2020  T Circuits.     
+00021d90: 2020 2020 2020 2020 2020 2079 6320 3d20             yc = 
+00021da0: 726f 775b 315d 5b22 436c 6f73 6522 5d0a  row[1]["Close"].
+00021db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021dc0: 796f 203d 2072 6f77 5b31 5d5b 224f 7065  yo = row[1]["Ope
+00021dd0: 6e22 5d0a 2020 2020 2020 2020 2020 2020  n"].            
+00021de0: 2020 2020 6966 2079 6320 3c3d 2079 6f3a      if yc <= yo:
+00021df0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00021e00: 2020 2020 2023 2073 656c 662e 6465 6661       # self.defa
+00021e10: 756c 745f 6c6f 6767 6572 2e69 6e66 6f28  ult_logger.info(
+00021e20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00021e30: 2020 2020 2023 2020 2020 2066 2753 746f       #     f'Sto
+00021e40: 636b 3a7b 7361 7665 4469 6374 5b22 5374  ck:{saveDict["St
+00021e50: 6f63 6b22 5d7d 2c20 6973 206e 6f74 2061  ock"]}, is not a
+00021e60: 206d 6f6d 656e 7475 6d2d 6761 696e 6572   momentum-gainer
+00021e70: 2062 6563 6175 7365 2079 6573 7465 7264   because yesterd
+00021e80: 6179 2d63 6c6f 7365 2028 7b79 637d 2920  ay-close ({yc}) 
+00021e90: 3c3d 2079 6573 7465 7264 6179 2d6f 7065  <= yesterday-ope
+00021ea0: 6e20 287b 796f 7d29 270a 2020 2020 2020  n ({yo})'.      
+00021eb0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00021ec0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00021ed0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+00021ee0: 7365 0a20 2020 2020 2020 2020 2020 206f  se.            o
+00021ef0: 7065 6e44 6573 6320 3d20 6461 7461 2e73  penDesc = data.s
+00021f00: 6f72 745f 7661 6c75 6573 2862 793d 5b22  ort_values(by=["
+00021f10: 4f70 656e 225d 2c20 6173 6365 6e64 696e  Open"], ascendin
+00021f20: 673d 4661 6c73 6529 0a20 2020 2020 2020  g=False).       
+00021f30: 2020 2020 2063 6c6f 7365 4465 7363 203d       closeDesc =
+00021f40: 2064 6174 612e 736f 7274 5f76 616c 7565   data.sort_value
+00021f50: 7328 6279 3d5b 2243 6c6f 7365 225d 2c20  s(by=["Close"], 
+00021f60: 6173 6365 6e64 696e 673d 4661 6c73 6529  ascending=False)
+00021f70: 0a20 2020 2020 2020 2020 2020 2076 6f6c  .            vol
+00021f80: 4465 7363 203d 2064 6174 612e 736f 7274  Desc = data.sort
+00021f90: 5f76 616c 7565 7328 6279 3d5b 2256 6f6c  _values(by=["Vol
+00021fa0: 756d 6522 5d2c 2061 7363 656e 6469 6e67  ume"], ascending
+00021fb0: 3d46 616c 7365 290a 2020 2020 2020 2020  =False).        
+00021fc0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+00021fd0: 2020 2020 2020 2020 2069 6620 280a 2020           if (.  
+00021fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021ff0: 2020 6461 7461 2e65 7175 616c 7328 6f70    data.equals(op
+00022000: 656e 4465 7363 290a 2020 2020 2020 2020  enDesc).        
+00022010: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+00022020: 6461 7461 2e65 7175 616c 7328 636c 6f73  data.equals(clos
+00022030: 6544 6573 6329 0a20 2020 2020 2020 2020  eDesc).         
+00022040: 2020 2020 2020 2020 2020 2061 6e64 2064             and d
+00022050: 6174 612e 6571 7561 6c73 2876 6f6c 4465  ata.equals(volDe
+00022060: 7363 290a 2020 2020 2020 2020 2020 2020  sc).            
+00022070: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
+00022080: 2020 2020 2020 2020 2020 2023 2073 656c             # sel
+00022090: 662e 6465 6661 756c 745f 6c6f 6767 6572  f.default_logger
+000220a0: 2e69 6e66 6f28 0a20 2020 2020 2020 2020  .info(.         
+000220b0: 2020 2020 2020 2020 2020 2023 2020 2020             #    
+000220c0: 2066 2753 746f 636b 3a7b 7361 7665 4469   f'Stock:{saveDi
+000220d0: 6374 5b22 5374 6f63 6b22 5d7d 2c20 6f70  ct["Stock"]}, op
+000220e0: 656e 2c63 6c6f 7365 2061 6e64 2076 6f6c  en,close and vol
+000220f0: 756d 6520 6571 7561 6c20 6672 6f6d 2064  ume equal from d
+00022100: 6179 2062 6566 6f72 6520 7965 7374 6572  ay before yester
+00022110: 6461 792e 2041 2070 6f74 656e 7469 616c  day. A potential
+00022120: 206d 6f6d 656e 7475 6d2d 6761 696e 6572   momentum-gainer
+00022130: 2127 0a20 2020 2020 2020 2020 2020 2020  !'.             
+00022140: 2020 2020 2020 2023 2029 0a20 2020 2020         # ).     
+00022150: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00022160: 6f20 3d20 6461 7461 5b22 4f70 656e 225d  o = data["Open"]
+00022170: 2e69 6c6f 635b 305d 0a20 2020 2020 2020  .iloc[0].       
+00022180: 2020 2020 2020 2020 2020 2020 2079 6320               yc 
+00022190: 3d20 6461 7461 5b22 436c 6f73 6522 5d2e  = data["Close"].
+000221a0: 696c 6f63 5b31 5d0a 2020 2020 2020 2020  iloc[1].        
+000221b0: 2020 2020 2020 2020 2020 2020 796f 203d              yo =
+000221c0: 2064 6174 615b 224f 7065 6e22 5d2e 696c   data["Open"].il
+000221d0: 6f63 5b31 5d0a 2020 2020 2020 2020 2020  oc[1].          
+000221e0: 2020 2020 2020 2020 2020 6479 6320 3d20            dyc = 
+000221f0: 6461 7461 5b22 436c 6f73 6522 5d2e 696c  data["Close"].il
+00022200: 6f63 5b32 5d0a 2020 2020 2020 2020 2020  oc[2].          
+00022210: 2020 2020 2020 2020 2020 6966 2028 746f            if (to
+00022220: 203e 3d20 7963 2920 616e 6420 2879 6f20   >= yc) and (yo 
+00022230: 3e3d 2064 7963 293a 0a20 2020 2020 2020  >= dyc):.       
+00022240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022250: 2023 2073 656c 662e 6465 6661 756c 745f   # self.default_
+00022260: 6c6f 6767 6572 2e69 6e66 6f28 0a20 2020  logger.info(.   
+00022270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022280: 2020 2020 2023 2020 2020 2066 2753 746f       #     f'Sto
+00022290: 636b 3a7b 7361 7665 4469 6374 5b22 5374  ck:{saveDict["St
+000222a0: 6f63 6b22 5d7d 2c20 6973 2061 206d 6f6d  ock"]}, is a mom
+000222b0: 656e 7475 6d2d 6761 696e 6572 2062 6563  entum-gainer bec
+000222c0: 6175 7365 2074 6f64 6179 2d6f 7065 6e20  ause today-open 
+000222d0: 287b 746f 7d29 203e 3d20 7965 7374 6572  ({to}) >= yester
+000222e0: 6461 792d 636c 6f73 6520 287b 7963 7d29  day-close ({yc})
+000222f0: 2061 6e64 2079 6573 7465 7264 6179 2d6f   and yesterday-o
+00022300: 7065 6e28 7b79 6f7d 2920 3e3d 2064 6179  pen({yo}) >= day
+00022310: 2d62 6566 6f72 652d 636c 6f73 6528 7b64  -before-close({d
+00022320: 7963 7d29 270a 2020 2020 2020 2020 2020  yc})'.          
+00022330: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00022340: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00022350: 2020 2020 2020 2020 2020 7361 7665 6420            saved 
+00022360: 3d20 7365 6c66 2e66 696e 6443 7572 7265  = self.findCurre
+00022370: 6e74 5361 7665 6456 616c 7565 2873 6372  ntSavedValue(scr
+00022380: 6565 6e44 6963 742c 2073 6176 6544 6963  eenDict, saveDic
+00022390: 742c 2022 5061 7474 6572 6e22 290a 2020  t, "Pattern").  
+000223a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000223b0: 2020 2020 2020 7363 7265 656e 4469 6374        screenDict
+000223c0: 5b22 5061 7474 6572 6e22 5d20 3d20 280a  ["Pattern"] = (.
+000223d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000223e0: 2020 2020 2020 2020 2020 2020 7361 7665              save
+000223f0: 645b 305d 0a20 2020 2020 2020 2020 2020  d[0].           
+00022400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022410: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
+00022420: 440a 2020 2020 2020 2020 2020 2020 2020  D.              
+00022430: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+00022440: 636f 6c6f 7254 6578 742e 4752 4545 4e0a  colorText.GREEN.
+00022450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022460: 2020 2020 2020 2020 2020 2020 2b20 224d              + "M
+00022470: 6f6d 656e 7475 6d20 4761 696e 6572 220a  omentum Gainer".
+00022480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022490: 2020 2020 2020 2020 2020 2020 2b20 636f              + co
+000224a0: 6c6f 7254 6578 742e 454e 440a 2020 2020  lorText.END.    
+000224b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000224c0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+000224d0: 2020 2020 2020 2020 2020 2020 2020 7361                sa
+000224e0: 7665 4469 6374 5b22 5061 7474 6572 6e22  veDict["Pattern"
+000224f0: 5d20 3d20 7361 7665 645b 315d 202b 2022  ] = saved[1] + "
+00022500: 4d6f 6d65 6e74 756d 2047 6169 6e65 7222  Momentum Gainer"
+00022510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00022520: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00022530: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
+00022540: 2020 2020 2020 2020 2023 2073 656c 662e           # self.
+00022550: 6465 6661 756c 745f 6c6f 6767 6572 2e69  default_logger.i
+00022560: 6e66 6f28 0a20 2020 2020 2020 2020 2020  nfo(.           
+00022570: 2020 2020 2020 2020 2023 2020 2020 2066           #     f
+00022580: 2753 746f 636b 3a7b 7361 7665 4469 6374  'Stock:{saveDict
+00022590: 5b22 5374 6f63 6b22 5d7d 2c20 6973 206e  ["Stock"]}, is n
+000225a0: 6f74 2061 206d 6f6d 656e 7475 6d2d 6761  ot a momentum-ga
+000225b0: 696e 6572 2062 6563 6175 7365 2065 6974  iner because eit
+000225c0: 6865 7220 746f 6461 792d 6f70 656e 2028  her today-open (
+000225d0: 7b74 6f7d 2920 3c20 7965 7374 6572 6461  {to}) < yesterda
+000225e0: 792d 636c 6f73 6520 287b 7963 7d29 206f  y-close ({yc}) o
+000225f0: 7220 7965 7374 6572 6461 792d 6f70 656e  r yesterday-open
+00022600: 287b 796f 7d29 203c 2064 6179 2d62 6566  ({yo}) < day-bef
+00022610: 6f72 652d 636c 6f73 6528 7b64 7963 7d29  ore-close({dyc})
+00022620: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+00022630: 2020 2020 2020 2320 290a 2020 2020 2020        # ).      
+00022640: 2020 2020 2020 6578 6365 7074 2049 6e64        except Ind
+00022650: 6578 4572 726f 7220 6173 2065 3a20 2320  exError as e: # 
+00022660: 7072 6167 6d61 3a20 6e6f 2063 6f76 6572  pragma: no cover
+00022670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00022680: 2073 656c 662e 6465 6661 756c 745f 6c6f   self.default_lo
+00022690: 6767 6572 2e64 6562 7567 2865 2c20 6578  gger.debug(e, ex
+000226a0: 635f 696e 666f 3d54 7275 6529 0a20 2020  c_info=True).   
+000226b0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000226c0: 662e 6465 6661 756c 745f 6c6f 6767 6572  f.default_logger
+000226d0: 2e64 6562 7567 2864 6174 6129 0a20 2020  .debug(data).   
+000226e0: 2020 2020 2020 2020 2020 2020 2070 6173               pas
+000226f0: 730a 2020 2020 2020 2020 2020 2020 7265  s.            re
+00022700: 7475 726e 2046 616c 7365 0a20 2020 2020  turn False.     
+00022710: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
+00022720: 696f 6e20 6173 2065 3a20 2023 2070 7261  ion as e:  # pra
+00022730: 676d 613a 206e 6f20 636f 7665 720a 2020  gma: no cover.  
+00022740: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+00022750: 6566 6175 6c74 5f6c 6f67 6765 722e 6465  efault_logger.de
+00022760: 6275 6728 652c 2065 7863 5f69 6e66 6f3d  bug(e, exc_info=
+00022770: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
+00022780: 2020 7265 7475 726e 2046 616c 7365 0a0a    return False..
+00022790: 2020 2020 2340 6d65 6173 7572 655f 7469      #@measure_ti
+000227a0: 6d65 0a20 2020 2023 2056 616c 6964 6174  me.    # Validat
+000227b0: 6520 4d6f 7669 6e67 2061 7665 7261 6765  e Moving average
+000227c0: 7320 616e 6420 6c6f 6f6b 2066 6f72 2062  s and look for b
+000227d0: 7579 2f73 656c 6c20 7369 676e 616c 730a  uy/sell signals.
+000227e0: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+000227f0: 4d6f 7669 6e67 4176 6572 6167 6573 2873  MovingAverages(s
+00022800: 656c 662c 2064 662c 2073 6372 6565 6e44  elf, df, screenD
+00022810: 6963 742c 2073 6176 6544 6963 742c 206d  ict, saveDict, m
+00022820: 6152 616e 6765 3d32 2e35 2c6d 614c 656e  aRange=2.5,maLen
+00022830: 6774 683d 3029 3a0a 2020 2020 2020 2020  gth=0):.        
+00022840: 6461 7461 203d 2064 662e 636f 7079 2829  data = df.copy()
+00022850: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
+00022860: 6461 7461 2e66 696c 6c6e 6128 3029 0a20  data.fillna(0). 
+00022870: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
+00022880: 7461 2e72 6570 6c61 6365 285b 6e70 2e69  ta.replace([np.i
+00022890: 6e66 2c20 2d6e 702e 696e 665d 2c20 3029  nf, -np.inf], 0)
+000228a0: 0a20 2020 2020 2020 2072 6563 656e 7420  .        recent 
+000228b0: 3d20 6461 7461 2e68 6561 6428 3129 0a20  = data.head(1). 
+000228c0: 2020 2020 2020 206d 6153 6967 6e61 6c73         maSignals
+000228d0: 203d 205b 5d0a 2020 2020 2020 2020 6966   = [].        if
+000228e0: 2073 7472 286d 614c 656e 6774 6829 2069   str(maLength) i
+000228f0: 6e20 5b22 3022 2c22 3222 2c22 3322 5d3a  n ["0","2","3"]:
+00022900: 0a20 2020 2020 2020 2020 2020 2073 6176  .            sav
+00022910: 6564 203d 2073 656c 662e 6669 6e64 4375  ed = self.findCu
+00022920: 7272 656e 7453 6176 6564 5661 6c75 6528  rrentSavedValue(
+00022930: 7363 7265 656e 4469 6374 2c73 6176 6544  screenDict,saveD
+00022940: 6963 742c 224d 412d 5369 676e 616c 2229  ict,"MA-Signal")
+00022950: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00022960: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00022970: 2020 7265 6365 6e74 5b22 534d 4122 5d2e    recent["SMA"].
+00022980: 696c 6f63 5b30 5d20 3e20 7265 6365 6e74  iloc[0] > recent
+00022990: 5b22 4c4d 4122 5d2e 696c 6f63 5b30 5d0a  ["LMA"].iloc[0].
+000229a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000229b0: 616e 6420 7265 6365 6e74 5b22 436c 6f73  and recent["Clos
+000229c0: 6522 5d2e 696c 6f63 5b30 5d20 3e20 7265  e"].iloc[0] > re
+000229d0: 6365 6e74 5b22 534d 4122 5d2e 696c 6f63  cent["SMA"].iloc
+000229e0: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
+000229f0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00022a00: 2020 2073 6372 6565 6e44 6963 745b 224d     screenDict["M
+00022a10: 412d 5369 676e 616c 225d 203d 2028 0a20  A-Signal"] = (. 
+00022a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022a30: 2020 2073 6176 6564 5b30 5d20 2b20 636f     saved[0] + co
+00022a40: 6c6f 7254 6578 742e 424f 4c44 202b 2063  lorText.BOLD + c
+00022a50: 6f6c 6f72 5465 7874 2e47 5245 454e 202b  olorText.GREEN +
+00022a60: 2022 4275 6c6c 6973 6822 202b 2063 6f6c   "Bullish" + col
+00022a70: 6f72 5465 7874 2e45 4e44 0a20 2020 2020  orText.END.     
+00022a80: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00022a90: 2020 2020 2020 2020 2020 2020 2073 6176               sav
+00022aa0: 6544 6963 745b 224d 412d 5369 676e 616c  eDict["MA-Signal
+00022ab0: 225d 203d 2073 6176 6564 5b31 5d20 2b20  "] = saved[1] + 
+00022ac0: 2242 756c 6c69 7368 220a 2020 2020 2020  "Bullish".      
+00022ad0: 2020 2020 2020 2020 2020 6d61 5369 676e            maSign
+00022ae0: 616c 732e 6170 7065 6e64 2822 3322 290a  als.append("3").
+00022af0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00022b00: 2072 6563 656e 745b 2253 4d41 225d 2e69   recent["SMA"].i
+00022b10: 6c6f 635b 305d 203c 2072 6563 656e 745b  loc[0] < recent[
+00022b20: 224c 4d41 225d 2e69 6c6f 635b 305d 3a0a  "LMA"].iloc[0]:.
+00022b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022b40: 7363 7265 656e 4469 6374 5b22 4d41 2d53  screenDict["MA-S
+00022b50: 6967 6e61 6c22 5d20 3d20 280a 2020 2020  ignal"] = (.    
+00022b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022b70: 7361 7665 645b 305d 202b 2063 6f6c 6f72  saved[0] + color
+00022b80: 5465 7874 2e42 4f4c 4420 2b20 636f 6c6f  Text.BOLD + colo
+00022b90: 7254 6578 742e 4641 494c 202b 2022 4265  rText.FAIL + "Be
+00022ba0: 6172 6973 6822 202b 2063 6f6c 6f72 5465  arish" + colorTe
+00022bb0: 7874 2e45 4e44 0a20 2020 2020 2020 2020  xt.END.         
+00022bc0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00022bd0: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
+00022be0: 745b 224d 412d 5369 676e 616c 225d 203d  t["MA-Signal"] =
+00022bf0: 2073 6176 6564 5b31 5d20 2b20 2242 6561   saved[1] + "Bea
+00022c00: 7269 7368 220a 2020 2020 2020 2020 2020  rish".          
+00022c10: 2020 2020 2020 6d61 5369 676e 616c 732e        maSignals.
+00022c20: 6170 7065 6e64 2822 3222 290a 2020 2020  append("2").    
+00022c30: 2020 2020 2020 2020 656c 6966 2072 6563          elif rec
+00022c40: 656e 745b 2253 4d41 225d 2e69 6c6f 635b  ent["SMA"].iloc[
+00022c50: 305d 203d 3d20 303a 0a20 2020 2020 2020  0] == 0:.       
+00022c60: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
+00022c70: 6963 745b 224d 412d 5369 676e 616c 225d  ict["MA-Signal"]
+00022c80: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
+00022c90: 2020 2020 2020 2020 2073 6176 6564 5b30           saved[0
+00022ca0: 5d20 2b20 636f 6c6f 7254 6578 742e 424f  ] + colorText.BO
+00022cb0: 4c44 202b 2063 6f6c 6f72 5465 7874 2e57  LD + colorText.W
+00022cc0: 4152 4e20 2b20 2255 6e6b 6e6f 776e 2220  ARN + "Unknown" 
+00022cd0: 2b20 636f 6c6f 7254 6578 742e 454e 440a  + colorText.END.
+00022ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022cf0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00022d00: 2020 7361 7665 4469 6374 5b22 4d41 2d53    saveDict["MA-S
+00022d10: 6967 6e61 6c22 5d20 3d20 7361 7665 645b  ignal"] = saved[
+00022d20: 315d 202b 2022 556e 6b6e 6f77 6e22 0a20  1] + "Unknown". 
+00022d30: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00022d40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00022d50: 2073 6372 6565 6e44 6963 745b 224d 412d   screenDict["MA-
+00022d60: 5369 676e 616c 225d 203d 2028 0a20 2020  Signal"] = (.   
+00022d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022d80: 2073 6176 6564 5b30 5d20 2b20 636f 6c6f   saved[0] + colo
+00022d90: 7254 6578 742e 424f 4c44 202b 2063 6f6c  rText.BOLD + col
+00022da0: 6f72 5465 7874 2e57 4152 4e20 2b20 224e  orText.WARN + "N
+00022db0: 6575 7472 616c 2220 2b20 636f 6c6f 7254  eutral" + colorT
+00022dc0: 6578 742e 454e 440a 2020 2020 2020 2020  ext.END.        
+00022dd0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00022de0: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
+00022df0: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d20  ct["MA-Signal"] 
+00022e00: 3d20 7361 7665 645b 315d 202b 2022 4e65  = saved[1] + "Ne
+00022e10: 7574 7261 6c22 0a20 2020 2020 2020 2072  utral".        r
+00022e20: 6576 6572 7365 6444 6174 6120 3d20 6461  eversedData = da
+00022e30: 7461 5b3a 3a2d 315d 2020 2320 5265 7665  ta[::-1]  # Reve
+00022e40: 7273 6520 7468 6520 6461 7461 6672 616d  rse the datafram
+00022e50: 650a 2020 2020 2020 2020 656d 615f 3230  e.        ema_20
+00022e60: 203d 2070 6b74 616c 6962 2e45 4d41 2872   = pktalib.EMA(r
+00022e70: 6576 6572 7365 6444 6174 615b 2243 6c6f  eversedData["Clo
+00022e80: 7365 225d 2c32 3029 2e74 6169 6c28 3129  se"],20).tail(1)
+00022e90: 2e69 6c6f 635b 305d 0a20 2020 2020 2020  .iloc[0].       
+00022ea0: 2076 7761 7020 3d20 706b 7461 6c69 622e   vwap = pktalib.
+00022eb0: 5657 4150 2872 6576 6572 7365 6444 6174  VWAP(reversedDat
+00022ec0: 615b 2248 6967 6822 5d2c 7265 7665 7273  a["High"],revers
+00022ed0: 6564 4461 7461 5b22 4c6f 7722 5d2c 7265  edData["Low"],re
+00022ee0: 7665 7273 6564 4461 7461 5b22 436c 6f73  versedData["Clos
+00022ef0: 6522 5d2c 7265 7665 7273 6564 4461 7461  e"],reversedData
+00022f00: 5b22 566f 6c75 6d65 225d 292e 7461 696c  ["Volume"]).tail
+00022f10: 2831 292e 696c 6f63 5b30 5d0a 2020 2020  (1).iloc[0].    
+00022f20: 2020 2020 736d 6144 6576 203d 2064 6174      smaDev = dat
+00022f30: 615b 2253 4d41 225d 2e69 6c6f 635b 305d  a["SMA"].iloc[0]
+00022f40: 202a 206d 6152 616e 6765 202f 2031 3030   * maRange / 100
+00022f50: 0a20 2020 2020 2020 206c 6d61 4465 7620  .        lmaDev 
+00022f60: 3d20 6461 7461 5b22 4c4d 4122 5d2e 696c  = data["LMA"].il
+00022f70: 6f63 5b30 5d20 2a20 6d61 5261 6e67 6520  oc[0] * maRange 
+00022f80: 2f20 3130 300a 2020 2020 2020 2020 656d  / 100.        em
+00022f90: 6144 6576 203d 2065 6d61 5f32 3020 2a20  aDev = ema_20 * 
+00022fa0: 6d61 5261 6e67 6520 2f20 3130 300a 2020  maRange / 100.  
+00022fb0: 2020 2020 2020 7677 6170 4465 7620 3d20        vwapDev = 
+00022fc0: 7677 6170 202a 206d 6152 616e 6765 202f  vwap * maRange /
+00022fd0: 2031 3030 0a20 2020 2020 2020 206f 7065   100.        ope
+00022fe0: 6e2c 2068 6967 682c 206c 6f77 2c20 636c  n, high, low, cl
+00022ff0: 6f73 652c 2073 6d61 2c20 6c6d 6120 3d20  ose, sma, lma = 
+00023000: 280a 2020 2020 2020 2020 2020 2020 6461  (.            da
+00023010: 7461 5b22 4f70 656e 225d 2e69 6c6f 635b  ta["Open"].iloc[
+00023020: 305d 2c0a 2020 2020 2020 2020 2020 2020  0],.            
+00023030: 6461 7461 5b22 4869 6768 225d 2e69 6c6f  data["High"].ilo
+00023040: 635b 305d 2c0a 2020 2020 2020 2020 2020  c[0],.          
+00023050: 2020 6461 7461 5b22 4c6f 7722 5d2e 696c    data["Low"].il
+00023060: 6f63 5b30 5d2c 0a20 2020 2020 2020 2020  oc[0],.         
+00023070: 2020 2064 6174 615b 2243 6c6f 7365 225d     data["Close"]
+00023080: 2e69 6c6f 635b 305d 2c0a 2020 2020 2020  .iloc[0],.      
+00023090: 2020 2020 2020 6461 7461 5b22 534d 4122        data["SMA"
+000230a0: 5d2e 696c 6f63 5b30 5d2c 0a20 2020 2020  ].iloc[0],.     
+000230b0: 2020 2020 2020 2064 6174 615b 224c 4d41         data["LMA
+000230c0: 225d 2e69 6c6f 635b 305d 2c0a 2020 2020  "].iloc[0],.    
+000230d0: 2020 2020 290a 2020 2020 2020 2020 6d61      ).        ma
+000230e0: 7320 3d20 5b73 6d61 2c6c 6d61 2c65 6d61  s = [sma,lma,ema
+000230f0: 5f32 302c 7677 6170 5d20 6966 206d 614c  _20,vwap] if maL
+00023100: 656e 6774 683d 3d30 2065 6c73 6520 5b73  ength==0 else [s
+00023110: 6d61 2c6c 6d61 2c65 6d61 5f32 305d 0a20  ma,lma,ema_20]. 
+00023120: 2020 2020 2020 206d 6144 6576 7320 3d20         maDevs = 
+00023130: 5b73 6d61 4465 762c 206c 6d61 4465 762c  [smaDev, lmaDev,
+00023140: 2065 6d61 4465 762c 2076 7761 7044 6576   emaDev, vwapDev
+00023150: 5d20 6966 206d 614c 656e 6774 683d 3d30  ] if maLength==0
+00023160: 2065 6c73 6520 5b73 6d61 4465 762c 206c   else [smaDev, l
+00023170: 6d61 4465 762c 2065 6d61 4465 765d 0a20  maDev, emaDev]. 
+00023180: 2020 2020 2020 206d 6154 6578 7473 203d         maTexts =
+00023190: 205b 2235 304d 4122 2c22 3230 304d 4122   ["50MA","200MA"
+000231a0: 2c22 3230 454d 4122 2c22 5657 4150 225d  ,"20EMA","VWAP"]
+000231b0: 2069 6620 6d61 4c65 6e67 7468 3d3d 3020   if maLength==0 
+000231c0: 656c 7365 205b 2235 304d 4122 2c22 3230  else ["50MA","20
+000231d0: 304d 4122 2c22 3230 454d 4122 5d0a 2020  0MA","20EMA"].  
+000231e0: 2020 2020 2020 6d61 5265 7665 7273 616c        maReversal
+000231f0: 203d 2030 0a20 2020 2020 2020 2069 6e64   = 0.        ind
+00023200: 6578 203d 2030 0a20 2020 2020 2020 2062  ex = 0.        b
+00023210: 756c 6c69 7368 4361 6e64 6c65 203d 2073  ullishCandle = s
+00023220: 656c 662e 6765 7443 616e 646c 6554 7970  elf.getCandleTyp
+00023230: 6528 6461 7461 290a 2020 2020 2020 2020  e(data).        
+00023240: 6966 2073 7472 286d 614c 656e 6774 6829  if str(maLength)
+00023250: 206e 6f74 2069 6e20 5b22 3222 2c22 3322   not in ["2","3"
+00023260: 5d3a 0a20 2020 2020 2020 2020 2020 2066  ]:.            f
+00023270: 6f72 206d 6120 696e 206d 6173 3a0a 2020  or ma in mas:.  
+00023280: 2020 2020 2020 2020 2020 2020 2020 7361                sa
+00023290: 7665 6420 3d20 7365 6c66 2e66 696e 6443  ved = self.findC
+000232a0: 7572 7265 6e74 5361 7665 6456 616c 7565  urrentSavedValue
+000232b0: 2873 6372 6565 6e44 6963 742c 7361 7665  (screenDict,save
+000232c0: 4469 6374 2c22 4d41 2d53 6967 6e61 6c22  Dict,"MA-Signal"
+000232d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000232e0: 2020 2320 5461 6b69 6e67 2053 7570 706f    # Taking Suppo
+000232f0: 7274 0a20 2020 2020 2020 2020 2020 2020  rt.             
+00023300: 2020 2069 6620 636c 6f73 6520 3e20 6d61     if close > ma
+00023310: 2061 6e64 206c 6f77 203c 3d20 286d 6120   and low <= (ma 
+00023320: 2b20 6d61 4465 7673 5b69 6e64 6578 5d29  + maDevs[index])
+00023330: 2061 6e64 2073 7472 286d 614c 656e 6774   and str(maLengt
+00023340: 6829 2069 6e20 5b22 3022 2c22 3122 5d3a  h) in ["0","1"]:
 00023350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00023360: 2020 2020 2023 2043 726f 7373 696e 6720       # Crossing 
-00023370: 7570 0a20 2020 2020 2020 2020 2020 2020  up.             
-00023380: 2020 2020 2020 2069 6620 6f70 656e 203c         if open <
-00023390: 206d 6120 616e 6420 636c 6f73 6520 3e20   ma and close > 
-000233a0: 6d61 2061 6e64 2073 7472 286d 614c 656e  ma and str(maLen
-000233b0: 6774 6829 2069 6e20 5b22 3022 2c22 3522  gth) in ["0","5"
-000233c0: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
-000233d0: 2020 2020 2020 2020 2020 2073 6372 6565             scree
-000233e0: 6e44 6963 745b 224d 412d 5369 676e 616c  nDict["MA-Signal
-000233f0: 225d 203d 2028 0a20 2020 2020 2020 2020  "] = (.         
-00023400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023410: 2020 2073 6176 6564 5b30 5d20 2b20 636f     saved[0] + co
-00023420: 6c6f 7254 6578 742e 424f 4c44 202b 2063  lorText.BOLD + c
-00023430: 6f6c 6f72 5465 7874 2e47 5245 454e 202b  olorText.GREEN +
-00023440: 2066 2242 756c 6c43 726f 7373 2d7b 6d61   f"BullCross-{ma
-00023450: 5465 7874 735b 696e 6465 785d 7d22 202b  Texts[index]}" +
-00023460: 2063 6f6c 6f72 5465 7874 2e45 4e44 0a20   colorText.END. 
-00023470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023480: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00023490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000234a0: 2073 6176 6544 6963 745b 224d 412d 5369   saveDict["MA-Si
-000234b0: 676e 616c 225d 203d 2073 6176 6564 5b31  gnal"] = saved[1
-000234c0: 5d20 2b20 6622 4275 6c6c 4372 6f73 732d  ] + f"BullCross-
-000234d0: 7b6d 6154 6578 7473 5b69 6e64 6578 5d7d  {maTexts[index]}
-000234e0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-000234f0: 2020 2020 2020 2020 2020 6d61 5265 7665            maReve
-00023500: 7273 616c 203d 2031 0a20 2020 2020 2020  rsal = 1.       
-00023510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023520: 206d 6153 6967 6e61 6c73 2e61 7070 656e   maSignals.appen
-00023530: 6428 2235 2229 0a20 2020 2020 2020 2020  d("5").         
-00023540: 2020 2020 2020 2023 2046 6f72 2061 2042         # For a B
-00023550: 6561 7269 7368 2043 616e 646c 650a 2020  earish Candle.  
-00023560: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00023570: 6966 206e 6f74 2062 756c 6c69 7368 4361  if not bullishCa
-00023580: 6e64 6c65 3a0a 2020 2020 2020 2020 2020  ndle:.          
-00023590: 2020 2020 2020 2020 2020 2320 4372 6f73            # Cros
-000235a0: 7369 6e67 2064 6f77 6e0a 2020 2020 2020  sing down.      
-000235b0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000235c0: 206f 7065 6e20 3e20 736d 6120 616e 6420   open > sma and 
-000235d0: 636c 6f73 6520 3c20 736d 6120 616e 6420  close < sma and 
-000235e0: 7374 7228 6d61 4c65 6e67 7468 2920 696e  str(maLength) in
-000235f0: 205b 2230 222c 2234 225d 3a0a 2020 2020   ["0","4"]:.    
-00023600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023610: 2020 2020 7363 7265 656e 4469 6374 5b22      screenDict["
-00023620: 4d41 2d53 6967 6e61 6c22 5d20 3d20 280a  MA-Signal"] = (.
-00023630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023640: 2020 2020 2020 2020 2020 2020 7361 7665              save
-00023650: 645b 305d 202b 2063 6f6c 6f72 5465 7874  d[0] + colorText
-00023660: 2e42 4f4c 4420 2b20 636f 6c6f 7254 6578  .BOLD + colorTex
-00023670: 742e 4641 494c 202b 2066 2242 6561 7243  t.FAIL + f"BearC
-00023680: 726f 7373 2d7b 6d61 5465 7874 735b 696e  ross-{maTexts[in
-00023690: 6465 785d 7d22 202b 2063 6f6c 6f72 5465  dex]}" + colorTe
-000236a0: 7874 2e45 4e44 0a20 2020 2020 2020 2020  xt.END.         
-000236b0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-000236c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000236d0: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
-000236e0: 745b 224d 412d 5369 676e 616c 225d 203d  t["MA-Signal"] =
-000236f0: 2073 6176 6564 5b31 5d20 2b20 6622 4265   saved[1] + f"Be
-00023700: 6172 4372 6f73 732d 7b6d 6154 6578 7473  arCross-{maTexts
-00023710: 5b69 6e64 6578 5d7d 220a 2020 2020 2020  [index]}".      
-00023720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023730: 2020 6d61 5265 7665 7273 616c 203d 202d    maReversal = -
-00023740: 310a 2020 2020 2020 2020 2020 2020 2020  1.              
-00023750: 2020 2020 2020 2020 2020 6d61 5369 676e            maSign
-00023760: 616c 732e 6170 7065 6e64 2822 3422 290a  als.append("4").
-00023770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023780: 696e 6465 7820 2b3d 2031 0a20 2020 2020  index += 1.     
-00023790: 2020 2072 6574 7572 6e56 616c 7565 203d     returnValue =
-000237a0: 206d 6152 6576 6572 7361 6c0a 2020 2020   maReversal.    
-000237b0: 2020 2020 6966 206d 614c 656e 6774 6820      if maLength 
-000237c0: 213d 2030 3a0a 2020 2020 2020 2020 2020  != 0:.          
-000237d0: 2020 7265 7475 726e 5661 6c75 6520 3d20    returnValue = 
-000237e0: 7374 7228 6d61 4c65 6e67 7468 2920 696e  str(maLength) in
-000237f0: 206d 6153 6967 6e61 6c73 0a20 2020 2020   maSignals.     
-00023800: 2020 2072 6574 7572 6e20 7265 7475 726e     return return
-00023810: 5661 6c75 650a 0a20 2020 2023 2046 696e  Value..    # Fin
-00023820: 6420 4e52 7820 7261 6e67 6520 666f 7220  d NRx range for 
-00023830: 5265 7665 7273 616c 0a20 2020 2064 6566  Reversal.    def
-00023840: 2076 616c 6964 6174 654e 6172 726f 7752   validateNarrowR
-00023850: 616e 6765 2873 656c 662c 2064 662c 2073  ange(self, df, s
-00023860: 6372 6565 6e44 6963 742c 2073 6176 6544  creenDict, saveD
-00023870: 6963 742c 206e 723d 3429 3a0a 2020 2020  ict, nr=4):.    
-00023880: 2020 2020 6966 2064 6620 6973 204e 6f6e      if df is Non
-00023890: 6520 6f72 206c 656e 2864 6629 203d 3d20  e or len(df) == 
-000238a0: 303a 0a20 2020 2020 2020 2020 2020 2072  0:.            r
-000238b0: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
-000238c0: 2020 2020 6461 7461 203d 2064 662e 636f      data = df.co
-000238d0: 7079 2829 0a20 2020 2020 2020 2073 6176  py().        sav
-000238e0: 6564 203d 2073 656c 662e 6669 6e64 4375  ed = self.findCu
-000238f0: 7272 656e 7453 6176 6564 5661 6c75 6528  rrentSavedValue(
-00023900: 7363 7265 656e 4469 6374 2c20 7361 7665  screenDict, save
-00023910: 4469 6374 2c20 2250 6174 7465 726e 2229  Dict, "Pattern")
-00023920: 0a20 2020 2020 2020 2069 6620 504b 4461  .        if PKDa
-00023930: 7465 5574 696c 6974 6965 732e 6973 5472  teUtilities.isTr
-00023940: 6164 696e 6754 696d 6528 293a 0a20 2020  adingTime():.   
-00023950: 2020 2020 2020 2020 2072 616e 6765 4461           rangeDa
-00023960: 7461 203d 2064 6174 612e 6865 6164 286e  ta = data.head(n
-00023970: 7220 2b20 3129 5b31 3a5d 0a20 2020 2020  r + 1)[1:].     
-00023980: 2020 2020 2020 206e 6f77 5f63 616e 646c         now_candl
-00023990: 6520 3d20 6461 7461 2e68 6561 6428 3129  e = data.head(1)
-000239a0: 0a20 2020 2020 2020 2020 2020 2072 616e  .            ran
-000239b0: 6765 4461 7461 5b22 5261 6e67 6522 5d20  geData["Range"] 
-000239c0: 3d20 6162 7328 7261 6e67 6544 6174 615b  = abs(rangeData[
-000239d0: 2243 6c6f 7365 225d 202d 2072 616e 6765  "Close"] - range
-000239e0: 4461 7461 5b22 4f70 656e 225d 290a 2020  Data["Open"]).  
-000239f0: 2020 2020 2020 2020 2020 7265 6365 6e74            recent
-00023a00: 203d 2072 616e 6765 4461 7461 2e68 6561   = rangeData.hea
-00023a10: 6428 3129 0a20 2020 2020 2020 2020 2020  d(1).           
-00023a20: 2069 6620 280a 2020 2020 2020 2020 2020   if (.          
-00023a30: 2020 2020 2020 6c65 6e28 7265 6365 6e74        len(recent
-00023a40: 2920 3d3d 2031 0a20 2020 2020 2020 2020  ) == 1.         
-00023a50: 2020 2020 2020 2061 6e64 2072 6563 656e         and recen
-00023a60: 745b 2252 616e 6765 225d 2e69 6c6f 635b  t["Range"].iloc[
-00023a70: 305d 203d 3d20 7261 6e67 6544 6174 612e  0] == rangeData.
-00023a80: 6465 7363 7269 6265 2829 5b22 5261 6e67  describe()["Rang
-00023a90: 6522 5d5b 226d 696e 225d 0a20 2020 2020  e"]["min"].     
-00023aa0: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
-00023ab0: 2020 2020 2020 2020 2020 6966 2028 0a20            if (. 
-00023ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023ad0: 2020 2073 656c 662e 6765 7443 616e 646c     self.getCandl
-00023ae0: 6554 7970 6528 7265 6365 6e74 290a 2020  eType(recent).  
+00023360: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
+00023370: 224d 412d 5369 676e 616c 225d 203d 2028  "MA-Signal"] = (
+00023380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00023390: 2020 2020 2020 2020 2073 6176 6564 5b30           saved[0
+000233a0: 5d20 2b20 636f 6c6f 7254 6578 742e 424f  ] + colorText.BO
+000233b0: 4c44 202b 2063 6f6c 6f72 5465 7874 2e47  LD + colorText.G
+000233c0: 5245 454e 202b 2066 227b 6d61 5465 7874  REEN + f"{maText
+000233d0: 735b 696e 6465 785d 7d2d 5375 7070 6f72  s[index]}-Suppor
+000233e0: 7422 202b 2063 6f6c 6f72 5465 7874 2e45  t" + colorText.E
+000233f0: 4e44 0a20 2020 2020 2020 2020 2020 2020  ND.             
+00023400: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00023410: 2020 2020 2020 2020 2020 2020 2073 6176               sav
+00023420: 6544 6963 745b 224d 412d 5369 676e 616c  eDict["MA-Signal
+00023430: 225d 203d 2073 6176 6564 5b31 5d20 2b20  "] = saved[1] + 
+00023440: 6622 7b6d 6154 6578 7473 5b69 6e64 6578  f"{maTexts[index
+00023450: 5d7d 2d53 7570 706f 7274 220a 2020 2020  ]}-Support".    
+00023460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023470: 6d61 5265 7665 7273 616c 203d 2031 0a20  maReversal = 1. 
+00023480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023490: 2020 206d 6153 6967 6e61 6c73 2e61 7070     maSignals.app
+000234a0: 656e 6428 2231 2229 0a20 2020 2020 2020  end("1").       
+000234b0: 2020 2020 2020 2020 2023 2056 616c 6964           # Valid
+000234c0: 6174 696e 6720 5265 7369 7374 616e 6365  ating Resistance
+000234d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000234e0: 2065 6c69 6620 636c 6f73 6520 3c20 6d61   elif close < ma
+000234f0: 2061 6e64 2068 6967 6820 3e3d 2028 6d61   and high >= (ma
+00023500: 202d 206d 6144 6576 735b 696e 6465 785d   - maDevs[index]
+00023510: 2920 616e 6420 7374 7228 6d61 4c65 6e67  ) and str(maLeng
+00023520: 7468 2920 696e 205b 2230 222c 2236 225d  th) in ["0","6"]
+00023530: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00023540: 2020 2020 2020 7363 7265 656e 4469 6374        screenDict
+00023550: 5b22 4d41 2d53 6967 6e61 6c22 5d20 3d20  ["MA-Signal"] = 
+00023560: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00023570: 2020 2020 2020 2020 2020 7361 7665 645b            saved[
+00023580: 305d 202b 2063 6f6c 6f72 5465 7874 2e42  0] + colorText.B
+00023590: 4f4c 4420 2b20 636f 6c6f 7254 6578 742e  OLD + colorText.
+000235a0: 4641 494c 202b 2066 227b 6d61 5465 7874  FAIL + f"{maText
+000235b0: 735b 696e 6465 785d 7d2d 5265 7369 7374  s[index]}-Resist
+000235c0: 2220 2b20 636f 6c6f 7254 6578 742e 454e  " + colorText.EN
+000235d0: 440a 2020 2020 2020 2020 2020 2020 2020  D.              
+000235e0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+000235f0: 2020 2020 2020 2020 2020 2020 7361 7665              save
+00023600: 4469 6374 5b22 4d41 2d53 6967 6e61 6c22  Dict["MA-Signal"
+00023610: 5d20 3d20 7361 7665 645b 315d 202b 2066  ] = saved[1] + f
+00023620: 227b 6d61 5465 7874 735b 696e 6465 785d  "{maTexts[index]
+00023630: 7d2d 5265 7369 7374 220a 2020 2020 2020  }-Resist".      
+00023640: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
+00023650: 5265 7665 7273 616c 203d 202d 310a 2020  Reversal = -1.  
+00023660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023670: 2020 6d61 5369 676e 616c 732e 6170 7065    maSignals.appe
+00023680: 6e64 2822 3622 290a 2020 2020 2020 2020  nd("6").        
+00023690: 2020 2020 2020 2020 2320 466f 7220 6120          # For a 
+000236a0: 4275 6c6c 6973 6820 4361 6e64 6c65 0a20  Bullish Candle. 
+000236b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000236c0: 6620 6275 6c6c 6973 6843 616e 646c 653a  f bullishCandle:
+000236d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000236e0: 2020 2020 2023 2043 726f 7373 696e 6720       # Crossing 
+000236f0: 7570 0a20 2020 2020 2020 2020 2020 2020  up.             
+00023700: 2020 2020 2020 2069 6620 6f70 656e 203c         if open <
+00023710: 206d 6120 616e 6420 636c 6f73 6520 3e20   ma and close > 
+00023720: 6d61 2061 6e64 2073 7472 286d 614c 656e  ma and str(maLen
+00023730: 6774 6829 2069 6e20 5b22 3022 2c22 3522  gth) in ["0","5"
+00023740: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
+00023750: 2020 2020 2020 2020 2020 2073 6372 6565             scree
+00023760: 6e44 6963 745b 224d 412d 5369 676e 616c  nDict["MA-Signal
+00023770: 225d 203d 2028 0a20 2020 2020 2020 2020  "] = (.         
+00023780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023790: 2020 2073 6176 6564 5b30 5d20 2b20 636f     saved[0] + co
+000237a0: 6c6f 7254 6578 742e 424f 4c44 202b 2063  lorText.BOLD + c
+000237b0: 6f6c 6f72 5465 7874 2e47 5245 454e 202b  olorText.GREEN +
+000237c0: 2066 2242 756c 6c43 726f 7373 2d7b 6d61   f"BullCross-{ma
+000237d0: 5465 7874 735b 696e 6465 785d 7d22 202b  Texts[index]}" +
+000237e0: 2063 6f6c 6f72 5465 7874 2e45 4e44 0a20   colorText.END. 
+000237f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023800: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00023810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023820: 2073 6176 6544 6963 745b 224d 412d 5369   saveDict["MA-Si
+00023830: 676e 616c 225d 203d 2073 6176 6564 5b31  gnal"] = saved[1
+00023840: 5d20 2b20 6622 4275 6c6c 4372 6f73 732d  ] + f"BullCross-
+00023850: 7b6d 6154 6578 7473 5b69 6e64 6578 5d7d  {maTexts[index]}
+00023860: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00023870: 2020 2020 2020 2020 2020 6d61 5265 7665            maReve
+00023880: 7273 616c 203d 2031 0a20 2020 2020 2020  rsal = 1.       
+00023890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000238a0: 206d 6153 6967 6e61 6c73 2e61 7070 656e   maSignals.appen
+000238b0: 6428 2235 2229 0a20 2020 2020 2020 2020  d("5").         
+000238c0: 2020 2020 2020 2023 2046 6f72 2061 2042         # For a B
+000238d0: 6561 7269 7368 2043 616e 646c 650a 2020  earish Candle.  
+000238e0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+000238f0: 6966 206e 6f74 2062 756c 6c69 7368 4361  if not bullishCa
+00023900: 6e64 6c65 3a0a 2020 2020 2020 2020 2020  ndle:.          
+00023910: 2020 2020 2020 2020 2020 2320 4372 6f73            # Cros
+00023920: 7369 6e67 2064 6f77 6e0a 2020 2020 2020  sing down.      
+00023930: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00023940: 206f 7065 6e20 3e20 736d 6120 616e 6420   open > sma and 
+00023950: 636c 6f73 6520 3c20 736d 6120 616e 6420  close < sma and 
+00023960: 7374 7228 6d61 4c65 6e67 7468 2920 696e  str(maLength) in
+00023970: 205b 2230 222c 2234 225d 3a0a 2020 2020   ["0","4"]:.    
+00023980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023990: 2020 2020 7363 7265 656e 4469 6374 5b22      screenDict["
+000239a0: 4d41 2d53 6967 6e61 6c22 5d20 3d20 280a  MA-Signal"] = (.
+000239b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000239c0: 2020 2020 2020 2020 2020 2020 7361 7665              save
+000239d0: 645b 305d 202b 2063 6f6c 6f72 5465 7874  d[0] + colorText
+000239e0: 2e42 4f4c 4420 2b20 636f 6c6f 7254 6578  .BOLD + colorTex
+000239f0: 742e 4641 494c 202b 2066 2242 6561 7243  t.FAIL + f"BearC
+00023a00: 726f 7373 2d7b 6d61 5465 7874 735b 696e  ross-{maTexts[in
+00023a10: 6465 785d 7d22 202b 2063 6f6c 6f72 5465  dex]}" + colorTe
+00023a20: 7874 2e45 4e44 0a20 2020 2020 2020 2020  xt.END.         
+00023a30: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00023a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00023a50: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
+00023a60: 745b 224d 412d 5369 676e 616c 225d 203d  t["MA-Signal"] =
+00023a70: 2073 6176 6564 5b31 5d20 2b20 6622 4265   saved[1] + f"Be
+00023a80: 6172 4372 6f73 732d 7b6d 6154 6578 7473  arCross-{maTexts
+00023a90: 5b69 6e64 6578 5d7d 220a 2020 2020 2020  [index]}".      
+00023aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023ab0: 2020 6d61 5265 7665 7273 616c 203d 202d    maReversal = -
+00023ac0: 310a 2020 2020 2020 2020 2020 2020 2020  1.              
+00023ad0: 2020 2020 2020 2020 2020 6d61 5369 676e            maSign
+00023ae0: 616c 732e 6170 7065 6e64 2822 3422 290a  als.append("4").
 00023af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023b00: 2020 616e 6420 6e6f 775f 6361 6e64 6c65    and now_candle
-00023b10: 5b22 436c 6f73 6522 5d2e 696c 6f63 5b30  ["Close"].iloc[0
-00023b20: 5d20 3e3d 2072 6563 656e 745b 2243 6c6f  ] >= recent["Clo
-00023b30: 7365 225d 2e69 6c6f 635b 305d 0a20 2020  se"].iloc[0].   
-00023b40: 2020 2020 2020 2020 2020 2020 2029 3a0a               ):.
-00023b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023b60: 2020 2020 7363 7265 656e 4469 6374 5b22      screenDict["
-00023b70: 5061 7474 6572 6e22 5d20 3d20 280a 2020  Pattern"] = (.  
-00023b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023b90: 2020 2020 2020 7361 7665 645b 305d 202b        saved[0] +
-00023ba0: 2063 6f6c 6f72 5465 7874 2e42 4f4c 4420   colorText.BOLD 
-00023bb0: 2b20 636f 6c6f 7254 6578 742e 4752 4545  + colorText.GREE
-00023bc0: 4e20 2b20 6622 4275 792d 4e52 7b6e 727d  N + f"Buy-NR{nr}
-00023bd0: 2220 2b20 636f 6c6f 7254 6578 742e 454e  " + colorText.EN
-00023be0: 440a 2020 2020 2020 2020 2020 2020 2020  D.              
-00023bf0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00023c00: 2020 2020 2020 2020 2020 2020 7361 7665              save
-00023c10: 4469 6374 5b22 5061 7474 6572 6e22 5d20  Dict["Pattern"] 
-00023c20: 3d20 7361 7665 645b 315d 202b 2066 2242  = saved[1] + f"B
-00023c30: 7579 2d4e 527b 6e72 7d22 0a20 2020 2020  uy-NR{nr}".     
-00023c40: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00023c50: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
-00023c60: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00023c70: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00023c80: 2020 2020 2020 6e6f 7420 7365 6c66 2e67        not self.g
-00023c90: 6574 4361 6e64 6c65 5479 7065 2872 6563  etCandleType(rec
-00023ca0: 656e 7429 0a20 2020 2020 2020 2020 2020  ent).           
-00023cb0: 2020 2020 2020 2020 2061 6e64 206e 6f77           and now
-00023cc0: 5f63 616e 646c 655b 2243 6c6f 7365 225d  _candle["Close"]
-00023cd0: 2e69 6c6f 635b 305d 203c 3d20 7265 6365  .iloc[0] <= rece
-00023ce0: 6e74 5b22 436c 6f73 6522 5d2e 696c 6f63  nt["Close"].iloc
-00023cf0: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
-00023d00: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
-00023d10: 2020 2020 2020 2020 2020 2073 6372 6565             scree
-00023d20: 6e44 6963 745b 2250 6174 7465 726e 225d  nDict["Pattern"]
-00023d30: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
-00023d40: 2020 2020 2020 2020 2020 2020 2073 6176               sav
-00023d50: 6564 5b30 5d20 2b20 636f 6c6f 7254 6578  ed[0] + colorTex
-00023d60: 742e 424f 4c44 202b 2063 6f6c 6f72 5465  t.BOLD + colorTe
-00023d70: 7874 2e46 4149 4c20 2b20 6622 5365 6c6c  xt.FAIL + f"Sell
-00023d80: 2d4e 527b 6e72 7d22 202b 2063 6f6c 6f72  -NR{nr}" + color
-00023d90: 5465 7874 2e45 4e44 0a20 2020 2020 2020  Text.END.       
-00023da0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00023db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023dc0: 2020 2073 6176 6544 6963 745b 2250 6174     saveDict["Pat
-00023dd0: 7465 726e 225d 203d 2073 6176 6564 5b31  tern"] = saved[1
-00023de0: 5d20 2b20 6622 5365 6c6c 2d4e 527b 6e72  ] + f"Sell-NR{nr
-00023df0: 7d22 0a20 2020 2020 2020 2020 2020 2020  }".             
-00023e00: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-00023e10: 7565 0a20 2020 2020 2020 2020 2020 2072  ue.            r
-00023e20: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
-00023e30: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00023e40: 2020 2020 2020 7261 6e67 6544 6174 6120        rangeData 
-00023e50: 3d20 6461 7461 2e68 6561 6428 6e72 290a  = data.head(nr).
-00023e60: 2020 2020 2020 2020 2020 2020 7261 6e67              rang
-00023e70: 6544 6174 612e 6c6f 635b 3a2c 2752 616e  eData.loc[:,'Ran
-00023e80: 6765 275d 203d 2061 6273 2872 616e 6765  ge'] = abs(range
-00023e90: 4461 7461 5b22 436c 6f73 6522 5d20 2d20  Data["Close"] - 
-00023ea0: 7261 6e67 6544 6174 615b 224f 7065 6e22  rangeData["Open"
-00023eb0: 5d29 0a20 2020 2020 2020 2020 2020 2072  ]).            r
-00023ec0: 6563 656e 7420 3d20 7261 6e67 6544 6174  ecent = rangeDat
-00023ed0: 612e 6865 6164 2831 290a 2020 2020 2020  a.head(1).      
-00023ee0: 2020 2020 2020 6966 2072 6563 656e 745b        if recent[
-00023ef0: 2252 616e 6765 225d 2e69 6c6f 635b 305d  "Range"].iloc[0]
-00023f00: 203d 3d20 7261 6e67 6544 6174 612e 6465   == rangeData.de
-00023f10: 7363 7269 6265 2829 5b22 5261 6e67 6522  scribe()["Range"
-00023f20: 5d5b 226d 696e 225d 3a0a 2020 2020 2020  ]["min"]:.      
-00023f30: 2020 2020 2020 2020 2020 7363 7265 656e            screen
-00023f40: 4469 6374 5b22 5061 7474 6572 6e22 5d20  Dict["Pattern"] 
-00023f50: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-00023f60: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
-00023f70: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
-00023f80: 4420 2b20 636f 6c6f 7254 6578 742e 4752  D + colorText.GR
-00023f90: 4545 4e20 2b20 6622 4e52 7b6e 727d 2220  EEN + f"NR{nr}" 
-00023fa0: 2b20 636f 6c6f 7254 6578 742e 454e 440a  + colorText.END.
-00023fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023fc0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00023fd0: 2020 7361 7665 4469 6374 5b22 5061 7474    saveDict["Patt
-00023fe0: 6572 6e22 5d20 3d20 7361 7665 645b 315d  ern"] = saved[1]
-00023ff0: 202b 2066 224e 527b 6e72 7d22 0a20 2020   + f"NR{nr}".   
-00024000: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00024010: 7572 6e20 5472 7565 0a20 2020 2020 2020  urn True.       
-00024020: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-00024030: 650a 0a20 2020 2023 2046 696e 6420 6966  e..    # Find if
-00024040: 2073 746f 636b 2069 7320 6e65 776c 7920   stock is newly 
-00024050: 6c69 7374 6564 0a20 2020 2064 6566 2076  listed.    def v
-00024060: 616c 6964 6174 654e 6577 6c79 4c69 7374  alidateNewlyList
-00024070: 6564 2873 656c 662c 2064 662c 2064 6179  ed(self, df, day
-00024080: 7354 6f4c 6f6f 6b62 6163 6b29 3a0a 2020  sToLookback):.  
-00024090: 2020 2020 2020 6966 2064 6620 6973 204e        if df is N
-000240a0: 6f6e 6520 6f72 206c 656e 2864 6629 203d  one or len(df) =
-000240b0: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
-000240c0: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
-000240d0: 2020 2020 2020 6461 7461 203d 2064 662e        data = df.
-000240e0: 636f 7079 2829 0a20 2020 2020 2020 2064  copy().        d
-000240f0: 6179 7354 6f4c 6f6f 6b62 6163 6b20 3d20  aysToLookback = 
-00024100: 696e 7428 6461 7973 546f 4c6f 6f6b 6261  int(daysToLookba
-00024110: 636b 5b3a 2d31 5d29 0a20 2020 2020 2020  ck[:-1]).       
-00024120: 2072 6563 656e 7420 3d20 6461 7461 2e68   recent = data.h
-00024130: 6561 6428 3129 0a20 2020 2020 2020 2069  ead(1).        i
-00024140: 6620 6c65 6e28 7265 6365 6e74 2920 3c20  f len(recent) < 
-00024150: 313a 0a20 2020 2020 2020 2020 2020 2072  1:.            r
-00024160: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
-00024170: 2020 2020 6966 206c 656e 2864 6174 6129      if len(data)
-00024180: 203c 2064 6179 7354 6f4c 6f6f 6b62 6163   < daysToLookbac
-00024190: 6b20 616e 6420 280a 2020 2020 2020 2020  k and (.        
-000241a0: 2020 2020 7265 6365 6e74 5b22 436c 6f73      recent["Clos
-000241b0: 6522 5d2e 696c 6f63 5b30 5d20 213d 206e  e"].iloc[0] != n
-000241c0: 702e 6e61 6e20 616e 6420 7265 6365 6e74  p.nan and recent
-000241d0: 5b22 436c 6f73 6522 5d2e 696c 6f63 5b30  ["Close"].iloc[0
-000241e0: 5d20 3e20 300a 2020 2020 2020 2020 293a  ] > 0.        ):
-000241f0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00024200: 7572 6e20 5472 7565 0a20 2020 2020 2020  urn True.       
-00024210: 2072 6574 7572 6e20 4661 6c73 650a 0a20   return False.. 
-00024220: 2020 2023 2056 616c 6964 6174 6520 6966     # Validate if
-00024230: 2074 6865 2073 746f 636b 2070 7269 6365   the stock price
-00024240: 7320 6172 6520 6174 206c 6561 7374 2072  s are at least r
-00024250: 6973 696e 6720 6279 2032 2520 666f 7220  ising by 2% for 
-00024260: 7468 6520 6c61 7374 2033 2073 6573 7369  the last 3 sessi
-00024270: 6f6e 730a 2020 2020 6465 6620 7661 6c69  ons.    def vali
-00024280: 6461 7465 5072 6963 6552 6973 696e 6742  datePriceRisingB
-00024290: 7941 744c 6561 7374 3250 6572 6365 6e74  yAtLeast2Percent
-000242a0: 2873 656c 662c 2064 662c 2073 6372 6565  (self, df, scree
-000242b0: 6e44 6963 742c 2073 6176 6544 6963 7429  nDict, saveDict)
-000242c0: 3a0a 2020 2020 2020 2020 6966 2064 6620  :.        if df 
-000242d0: 6973 204e 6f6e 6520 6f72 206c 656e 2864  is None or len(d
-000242e0: 6629 203d 3d20 303a 0a20 2020 2020 2020  f) == 0:.       
-000242f0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-00024300: 650a 2020 2020 2020 2020 6461 7461 203d  e.        data =
-00024310: 2064 662e 636f 7079 2829 0a20 2020 2020   df.copy().     
-00024320: 2020 2064 6174 6120 3d20 6461 7461 2e66     data = data.f
-00024330: 696c 6c6e 6128 3029 0a20 2020 2020 2020  illna(0).       
-00024340: 2064 6174 6120 3d20 6461 7461 2e72 6570   data = data.rep
-00024350: 6c61 6365 285b 6e70 2e69 6e66 2c20 2d6e  lace([np.inf, -n
-00024360: 702e 696e 665d 2c20 3029 0a20 2020 2020  p.inf], 0).     
-00024370: 2020 2064 6174 6120 3d20 6461 7461 2e68     data = data.h
-00024380: 6561 6428 3429 0a20 2020 2020 2020 2069  ead(4).        i
-00024390: 6620 6c65 6e28 6461 7461 2920 3c20 343a  f len(data) < 4:
-000243a0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000243b0: 7572 6e20 4661 6c73 650a 2020 2020 2020  urn False.      
-000243c0: 2020 6461 7930 203d 2064 6174 612e 696c    day0 = data.il
-000243d0: 6f63 5b30 5d5b 2243 6c6f 7365 225d 2e69  oc[0]["Close"].i
-000243e0: 7465 6d28 290a 2020 2020 2020 2020 6461  tem().        da
-000243f0: 794d 696e 7573 3120 3d20 6461 7461 2e69  yMinus1 = data.i
-00024400: 6c6f 635b 315d 5b22 436c 6f73 6522 5d2e  loc[1]["Close"].
-00024410: 6974 656d 2829 0a20 2020 2020 2020 2064  item().        d
-00024420: 6179 4d69 6e75 7332 203d 2064 6174 612e  ayMinus2 = data.
-00024430: 696c 6f63 5b32 5d5b 2243 6c6f 7365 225d  iloc[2]["Close"]
-00024440: 2e69 7465 6d28 290a 2020 2020 2020 2020  .item().        
-00024450: 6461 794d 696e 7573 3320 3d20 6461 7461  dayMinus3 = data
-00024460: 2e69 6c6f 635b 335d 5b22 436c 6f73 6522  .iloc[3]["Close"
-00024470: 5d2e 6974 656d 2829 0a20 2020 2020 2020  ].item().       
-00024480: 2070 6572 6365 6e74 3320 3d20 726f 756e   percent3 = roun
-00024490: 6428 2864 6179 4d69 6e75 7332 202d 2064  d((dayMinus2 - d
-000244a0: 6179 4d69 6e75 7333 2920 2a20 3130 3020  ayMinus3) * 100 
-000244b0: 2f20 6461 794d 696e 7573 332c 2032 290a  / dayMinus3, 2).
-000244c0: 2020 2020 2020 2020 7065 7263 656e 7432          percent2
-000244d0: 203d 2072 6f75 6e64 2828 6461 794d 696e   = round((dayMin
-000244e0: 7573 3120 2d20 6461 794d 696e 7573 3229  us1 - dayMinus2)
-000244f0: 202a 2031 3030 202f 2064 6179 4d69 6e75   * 100 / dayMinu
-00024500: 7332 2c20 3229 0a20 2020 2020 2020 2070  s2, 2).        p
-00024510: 6572 6365 6e74 3120 3d20 726f 756e 6428  ercent1 = round(
-00024520: 2864 6179 3020 2d20 6461 794d 696e 7573  (day0 - dayMinus
-00024530: 3129 202a 2031 3030 202f 2064 6179 4d69  1) * 100 / dayMi
-00024540: 6e75 7331 2c20 3229 0a0a 2020 2020 2020  nus1, 2)..      
-00024550: 2020 6966 2070 6572 6365 6e74 3120 3e3d    if percent1 >=
-00024560: 2032 2061 6e64 2070 6572 6365 6e74 3220   2 and percent2 
-00024570: 3e3d 2032 2061 6e64 2070 6572 6365 6e74  >= 2 and percent
-00024580: 3320 3e3d 2032 3a0a 2020 2020 2020 2020  3 >= 2:.        
-00024590: 2020 2020 7063 745f 6368 616e 6765 5f74      pct_change_t
-000245a0: 6578 7420 3d20 280a 2020 2020 2020 2020  ext = (.        
-000245b0: 2020 2020 2020 2020 2822 252e 3166 2525          ("%.1f%%
-000245c0: 2220 2520 7065 7263 656e 7431 290a 2020  " % percent1).  
-000245d0: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-000245e0: 2822 2028 252e 3166 2525 2c22 2025 2070  (" (%.1f%%," % p
-000245f0: 6572 6365 6e74 3229 0a20 2020 2020 2020  ercent2).       
-00024600: 2020 2020 2020 2020 202b 2028 2220 252e           + (" %.
-00024610: 3166 2525 2922 2025 2070 6572 6365 6e74  1f%%)" % percent
-00024620: 3329 0a20 2020 2020 2020 2020 2020 2029  3).            )
-00024630: 0a20 2020 2020 2020 2020 2020 2073 6176  .            sav
-00024640: 6544 6963 745b 2225 4368 6e67 225d 203d  eDict["%Chng"] =
-00024650: 2070 6374 5f63 6861 6e67 655f 7465 7874   pct_change_text
-00024660: 0a20 2020 2020 2020 2020 2020 2073 6372  .            scr
-00024670: 6565 6e44 6963 745b 2225 4368 6e67 225d  eenDict["%Chng"]
-00024680: 203d 2063 6f6c 6f72 5465 7874 2e47 5245   = colorText.GRE
-00024690: 454e 202b 2070 6374 5f63 6861 6e67 655f  EN + pct_change_
-000246a0: 7465 7874 202b 2063 6f6c 6f72 5465 7874  text + colorText
-000246b0: 2e45 4e44 0a20 2020 2020 2020 2020 2020  .END.           
-000246c0: 2072 6574 7572 6e20 5472 7565 2061 6e64   return True and
-000246d0: 2073 656c 662e 6765 7443 616e 646c 6554   self.getCandleT
-000246e0: 7970 6528 6461 7461 2e68 6561 6428 3129  ype(data.head(1)
-000246f0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00024700: 2046 616c 7365 0a0a 2020 2020 2340 6d65   False..    #@me
-00024710: 6173 7572 655f 7469 6d65 0a20 2020 2023  asure_time.    #
-00024720: 2076 616c 6964 6174 6520 6966 2052 5349   validate if RSI
-00024730: 2069 7320 7769 7468 696e 2067 6976 656e   is within given
-00024740: 2072 616e 6765 0a20 2020 2064 6566 2076   range.    def v
-00024750: 616c 6964 6174 6552 5349 2873 656c 662c  alidateRSI(self,
-00024760: 2064 662c 2073 6372 6565 6e44 6963 742c   df, screenDict,
-00024770: 2073 6176 6544 6963 742c 206d 696e 5253   saveDict, minRS
-00024780: 492c 206d 6178 5253 492c 7273 694b 6579  I, maxRSI,rsiKey
-00024790: 3d22 5253 4922 293a 0a20 2020 2020 2020  ="RSI"):.       
-000247a0: 2069 6620 6466 2069 7320 4e6f 6e65 206f   if df is None o
-000247b0: 7220 6c65 6e28 6466 2920 3d3d 2030 3a0a  r len(df) == 0:.
-000247c0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000247d0: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
-000247e0: 2069 6620 7273 694b 6579 206e 6f74 2069   if rsiKey not i
-000247f0: 6e20 6466 2e63 6f6c 756d 6e73 3a0a 2020  n df.columns:.  
-00024800: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00024810: 2046 616c 7365 0a20 2020 2020 2020 2064   False.        d
-00024820: 6174 6120 3d20 6466 2e63 6f70 7928 290a  ata = df.copy().
-00024830: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
-00024840: 6174 612e 6669 6c6c 6e61 2830 290a 2020  ata.fillna(0).  
-00024850: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
-00024860: 612e 7265 706c 6163 6528 5b6e 702e 696e  a.replace([np.in
-00024870: 662c 202d 6e70 2e69 6e66 5d2c 2030 290a  f, -np.inf], 0).
-00024880: 2020 2020 2020 2020 7273 6920 3d20 696e          rsi = in
-00024890: 7428 6461 7461 2e68 6561 6428 3129 5b72  t(data.head(1)[r
-000248a0: 7369 4b65 795d 2e69 6c6f 635b 305d 290a  siKey].iloc[0]).
-000248b0: 2020 2020 2020 2020 7361 7665 4469 6374          saveDict
-000248c0: 5b72 7369 4b65 795d 203d 2072 7369 0a20  [rsiKey] = rsi. 
-000248d0: 2020 2020 2020 2023 2068 7474 7073 3a2f         # https:/
-000248e0: 2f63 6861 7274 696e 6b2e 636f 6d2f 7363  /chartink.com/sc
-000248f0: 7265 656e 6572 2f72 7369 2d73 6372 6565  reener/rsi-scree
-00024900: 6e69 6e67 0a20 2020 2020 2020 2069 6620  ning.        if 
-00024910: 7273 693e 2030 2061 6e64 2072 7369 203e  rsi> 0 and rsi >
-00024920: 3d20 6d69 6e52 5349 2061 6e64 2072 7369  = minRSI and rsi
-00024930: 203c 3d20 6d61 7852 5349 3a20 2023 206f   <= maxRSI:  # o
-00024940: 7220 2872 7369 203c 3d20 3731 2061 6e64  r (rsi <= 71 and
-00024950: 2072 7369 203e 3d20 3637 293a 0a20 2020   rsi >= 67):.   
-00024960: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
-00024970: 6963 745b 7273 694b 6579 5d20 3d20 280a  ict[rsiKey] = (.
-00024980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024990: 636f 6c6f 7254 6578 742e 424f 4c44 202b  colorText.BOLD +
-000249a0: 2063 6f6c 6f72 5465 7874 2e47 5245 454e   colorText.GREEN
-000249b0: 202b 2073 7472 2872 7369 2920 2b20 636f   + str(rsi) + co
-000249c0: 6c6f 7254 6578 742e 454e 440a 2020 2020  lorText.END.    
-000249d0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-000249e0: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
-000249f0: 6520 6966 2028 7273 694b 6579 203d 3d20  e if (rsiKey == 
-00024a00: 2252 5349 6922 2920 656c 7365 2028 7365  "RSIi") else (se
-00024a10: 6c66 2e76 616c 6964 6174 6552 5349 2864  lf.validateRSI(d
-00024a20: 662c 2073 6372 6565 6e44 6963 742c 2073  f, screenDict, s
-00024a30: 6176 6544 6963 742c 206d 696e 5253 492c  aveDict, minRSI,
-00024a40: 206d 6178 5253 492c 7273 694b 6579 3d22   maxRSI,rsiKey="
-00024a50: 5253 4969 2229 206f 7220 5472 7565 290a  RSIi") or True).
-00024a60: 2020 2020 2020 2020 7363 7265 656e 4469          screenDi
-00024a70: 6374 5b72 7369 4b65 795d 203d 2063 6f6c  ct[rsiKey] = col
-00024a80: 6f72 5465 7874 2e42 4f4c 4420 2b20 636f  orText.BOLD + co
-00024a90: 6c6f 7254 6578 742e 4641 494c 202b 2073  lorText.FAIL + s
-00024aa0: 7472 2872 7369 2920 2b20 636f 6c6f 7254  tr(rsi) + colorT
-00024ab0: 6578 742e 454e 440a 2020 2020 2020 2020  ext.END.        
-00024ac0: 2320 4966 2065 6974 6865 7220 6461 696c  # If either dail
-00024ad0: 7920 6f72 2069 6e74 7261 6461 7920 5253  y or intraday RS
-00024ae0: 4920 636f 6d65 7320 7769 7468 696e 2072  I comes within r
-00024af0: 616e 6765 3f0a 2020 2020 2020 2020 7265  ange?.        re
-00024b00: 7475 726e 2046 616c 7365 2069 6620 2872  turn False if (r
-00024b10: 7369 4b65 7920 3d3d 2022 5253 4969 2229  siKey == "RSIi")
-00024b20: 2065 6c73 6520 2873 656c 662e 7661 6c69   else (self.vali
-00024b30: 6461 7465 5253 4928 6466 2c20 7363 7265  dateRSI(df, scre
-00024b40: 656e 4469 6374 2c20 7361 7665 4469 6374  enDict, saveDict
-00024b50: 2c20 6d69 6e52 5349 2c20 6d61 7852 5349  , minRSI, maxRSI
-00024b60: 2c72 7369 4b65 793d 2252 5349 6922 2929  ,rsiKey="RSIi"))
-00024b70: 0a0a 2020 2020 2320 5661 6c69 6461 7465  ..    # Validate
-00024b80: 2069 6620 7468 6520 7374 6f63 6b20 6973   if the stock is
-00024b90: 2062 756c 6c69 7368 2069 6e20 7468 6520   bullish in the 
-00024ba0: 7368 6f72 7420 7465 726d 0a20 2020 2064  short term.    d
-00024bb0: 6566 2076 616c 6964 6174 6553 686f 7274  ef validateShort
-00024bc0: 5465 726d 4275 6c6c 6973 6828 7365 6c66  TermBullish(self
-00024bd0: 2c20 6466 2c20 7363 7265 656e 4469 6374  , df, screenDict
-00024be0: 2c20 7361 7665 4469 6374 293a 0a20 2020  , saveDict):.   
-00024bf0: 2020 2020 2069 6620 6466 2069 7320 4e6f       if df is No
-00024c00: 6e65 206f 7220 6c65 6e28 6466 2920 3d3d  ne or len(df) ==
-00024c10: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
-00024c20: 7265 7475 726e 2046 616c 7365 0a20 2020  return False.   
-00024c30: 2020 2020 2064 6174 6120 3d20 6466 2e63       data = df.c
-00024c40: 6f70 7928 290a 2020 2020 2020 2020 2320  opy().        # 
-00024c50: 6874 7470 733a 2f2f 6368 6172 7469 6e6b  https://chartink
-00024c60: 2e63 6f6d 2f73 6372 6565 6e65 722f 7368  .com/screener/sh
-00024c70: 6f72 742d 7465 726d 2d62 756c 6c69 7368  ort-term-bullish
-00024c80: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
-00024c90: 6461 7461 2e66 696c 6c6e 6128 3029 0a20  data.fillna(0). 
-00024ca0: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
-00024cb0: 7461 2e72 6570 6c61 6365 285b 6e70 2e69  ta.replace([np.i
-00024cc0: 6e66 2c20 2d6e 702e 696e 665d 2c20 3029  nf, -np.inf], 0)
-00024cd0: 0a20 2020 2020 2020 2072 6563 656e 7420  .        recent 
-00024ce0: 3d20 6461 7461 2e68 6561 6428 3129 0a20  = data.head(1). 
-00024cf0: 2020 2020 2020 2066 6b20 3d20 3020 6966         fk = 0 if
-00024d00: 206c 656e 2864 6174 6129 203c 2033 2065   len(data) < 3 e
-00024d10: 6c73 6520 6e70 2e72 6f75 6e64 2864 6174  lse np.round(dat
-00024d20: 615b 2246 4153 544b 225d 2e69 6c6f 635b  a["FASTK"].iloc[
-00024d30: 325d 2c20 3529 0a20 2020 2020 2020 2023  2], 5).        #
-00024d40: 2052 6576 6572 7365 2074 6865 2064 6174   Reverse the dat
-00024d50: 6166 7261 6d65 2066 6f72 2069 6368 696d  aframe for ichim
-00024d60: 6f6b 7520 6361 6c63 756c 6174 696f 6e73  oku calculations
-00024d70: 2077 6974 6820 6461 7465 2069 6e20 6173   with date in as
-00024d80: 6365 6e64 696e 6720 6f72 6465 720a 2020  cending order.  
-00024d90: 2020 2020 2020 6466 5f6e 6577 203d 2064        df_new = d
-00024da0: 6174 615b 3a3a 2d31 5d0a 2020 2020 2020  ata[::-1].      
-00024db0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-00024dc0: 2020 2064 665f 6963 6869 203d 2064 665f     df_ichi = df_
-00024dd0: 6e65 772e 7265 6e61 6d65 280a 2020 2020  new.rename(.    
-00024de0: 2020 2020 2020 2020 2020 2020 636f 6c75              colu
-00024df0: 6d6e 733d 7b0a 2020 2020 2020 2020 2020  mns={.          
-00024e00: 2020 2020 2020 2020 2020 224f 7065 6e22            "Open"
-00024e10: 3a20 226f 7065 6e22 2c0a 2020 2020 2020  : "open",.      
-00024e20: 2020 2020 2020 2020 2020 2020 2020 2248                "H
-00024e30: 6967 6822 3a20 2268 6967 6822 2c0a 2020  igh": "high",.  
-00024e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024e50: 2020 224c 6f77 223a 2022 6c6f 7722 2c0a    "Low": "low",.
-00024e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024e70: 2020 2020 2243 6c6f 7365 223a 2022 636c      "Close": "cl
-00024e80: 6f73 6522 2c0a 2020 2020 2020 2020 2020  ose",.          
-00024e90: 2020 2020 2020 2020 2020 2256 6f6c 756d            "Volum
-00024ea0: 6522 3a20 2276 6f6c 756d 6522 2c0a 2020  e": "volume",.  
-00024eb0: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
-00024ec0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00024ed0: 2020 2020 2020 2020 2020 6963 6869 203d            ichi =
-00024ee0: 2070 6b74 616c 6962 2e69 6368 696d 6f6b   pktalib.ichimok
-00024ef0: 7528 6466 5f69 6368 692c 2039 2c20 3236  u(df_ichi, 9, 26
-00024f00: 2c20 3532 2c20 3236 290a 2020 2020 2020  , 52, 26).      
-00024f10: 2020 2020 2020 6966 2069 6368 6920 6973        if ichi is
-00024f20: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00024f30: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-00024f40: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
-00024f50: 6466 5f6e 6577 203d 2070 642e 636f 6e63  df_new = pd.conc
-00024f60: 6174 285b 6466 5f6e 6577 2c20 6963 6869  at([df_new, ichi
-00024f70: 5d2c 2061 7869 733d 3129 0a20 2020 2020  ], axis=1).     
-00024f80: 2020 2020 2020 2023 2052 6576 6572 7365         # Reverse
-00024f90: 2061 6761 696e 2074 6f20 6765 7420 7468   again to get th
-00024fa0: 6520 6d6f 7374 2072 6563 656e 7420 6461  e most recent da
-00024fb0: 7465 206f 6e20 746f 700a 2020 2020 2020  te on top.      
-00024fc0: 2020 2020 2020 6466 5f6e 6577 203d 2064        df_new = d
-00024fd0: 665f 6e65 775b 3a3a 2d31 5d0a 2020 2020  f_new[::-1].    
-00024fe0: 2020 2020 2020 2020 6466 5f6e 6577 203d          df_new =
-00024ff0: 2064 665f 6e65 772e 6865 6164 2831 290a   df_new.head(1).
-00025000: 2020 2020 2020 2020 2020 2020 6466 5f6e              df_n
-00025010: 6577 5b22 636c 6f75 645f 6772 6565 6e22  ew["cloud_green"
-00025020: 5d20 3d20 6466 5f6e 6577 5b22 4953 415f  ] = df_new["ISA_
-00025030: 3922 5d2e 696c 6f63 5b30 5d20 3e20 6466  9"].iloc[0] > df
-00025040: 5f6e 6577 5b22 4953 425f 3236 225d 2e69  _new["ISB_26"].i
-00025050: 6c6f 635b 305d 0a20 2020 2020 2020 2020  loc[0].         
-00025060: 2020 2064 665f 6e65 775b 2263 6c6f 7564     df_new["cloud
-00025070: 5f72 6564 225d 203d 2064 665f 6e65 775b  _red"] = df_new[
-00025080: 2249 5342 5f32 3622 5d2e 696c 6f63 5b30  "ISB_26"].iloc[0
-00025090: 5d20 3e20 6466 5f6e 6577 5b22 4953 415f  ] > df_new["ISA_
-000250a0: 3922 5d2e 696c 6f63 5b30 5d0a 2020 2020  9"].iloc[0].    
-000250b0: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
-000250c0: 7469 6f6e 2061 7320 653a 2020 2320 7072  tion as e:  # pr
-000250d0: 6167 6d61 3a20 6e6f 2063 6f76 6572 0a20  agma: no cover. 
-000250e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000250f0: 6465 6661 756c 745f 6c6f 6767 6572 2e64  default_logger.d
-00025100: 6562 7567 2865 2c20 6578 635f 696e 666f  ebug(e, exc_info
-00025110: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
-00025120: 2020 2070 6173 730a 2020 2020 2020 2020     pass.        
-00025130: 6162 6f76 6543 6c6f 7564 546f 7020 3d20  aboveCloudTop = 
-00025140: 4661 6c73 650a 2020 2020 2020 2020 2320  False.        # 
-00025150: 6261 7365 6c69 6e65 203e 2063 6c6f 7564  baseline > cloud
-00025160: 2074 6f70 2028 636c 6f75 6420 6973 2062   top (cloud is b
-00025170: 6f75 6e64 2062 7920 7370 616e 2061 2061  ound by span a a
-00025180: 6e64 2073 7061 6e20 6229 2061 6e64 2063  nd span b) and c
-00025190: 6c6f 7365 2069 7320 3e20 636c 6f75 6420  lose is > cloud 
-000251a0: 746f 700a 2020 2020 2020 2020 6966 2064  top.        if d
-000251b0: 665f 6e65 775b 2263 6c6f 7564 5f67 7265  f_new["cloud_gre
-000251c0: 656e 225d 2e69 6c6f 635b 305d 3a0a 2020  en"].iloc[0]:.  
-000251d0: 2020 2020 2020 2020 2020 6162 6f76 6543            aboveC
-000251e0: 6c6f 7564 546f 7020 3d20 280a 2020 2020  loudTop = (.    
-000251f0: 2020 2020 2020 2020 2020 2020 6466 5f6e              df_n
-00025200: 6577 5b22 494b 535f 3236 225d 2e69 6c6f  ew["IKS_26"].ilo
-00025210: 635b 305d 203e 2064 665f 6e65 775b 2249  c[0] > df_new["I
-00025220: 5341 5f39 225d 2e69 6c6f 635b 305d 0a20  SA_9"].iloc[0]. 
-00025230: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00025240: 6e64 2072 6563 656e 745b 2243 6c6f 7365  nd recent["Close
-00025250: 225d 2e69 6c6f 635b 305d 203e 2064 665f  "].iloc[0] > df_
-00025260: 6e65 775b 2249 5341 5f39 225d 2e69 6c6f  new["ISA_9"].ilo
-00025270: 635b 305d 0a20 2020 2020 2020 2020 2020  c[0].           
-00025280: 2029 0a20 2020 2020 2020 2065 6c69 6620   ).        elif 
-00025290: 6466 5f6e 6577 5b22 636c 6f75 645f 7265  df_new["cloud_re
-000252a0: 6422 5d2e 696c 6f63 5b30 5d3a 0a20 2020  d"].iloc[0]:.   
-000252b0: 2020 2020 2020 2020 2061 626f 7665 436c           aboveCl
-000252c0: 6f75 6454 6f70 203d 2028 0a20 2020 2020  oudTop = (.     
-000252d0: 2020 2020 2020 2020 2020 2064 665f 6e65             df_ne
-000252e0: 775b 2249 4b53 5f32 3622 5d2e 696c 6f63  w["IKS_26"].iloc
-000252f0: 5b30 5d20 3e20 6466 5f6e 6577 5b22 4953  [0] > df_new["IS
-00025300: 425f 3236 225d 2e69 6c6f 635b 305d 0a20  B_26"].iloc[0]. 
-00025310: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00025320: 6e64 2072 6563 656e 745b 2243 6c6f 7365  nd recent["Close
-00025330: 225d 2e69 6c6f 635b 305d 203e 2064 665f  "].iloc[0] > df_
-00025340: 6e65 775b 2249 5342 5f32 3622 5d2e 696c  new["ISB_26"].il
-00025350: 6f63 5b30 5d0a 2020 2020 2020 2020 2020  oc[0].          
-00025360: 2020 290a 0a20 2020 2020 2020 2023 204c    )..        # L
-00025370: 6174 6573 7420 4963 6869 6d6f 6b75 2062  atest Ichimoku b
-00025380: 6173 656c 696e 6520 6973 203c 206c 6174  aseline is < lat
-00025390: 6573 7420 4963 6869 6d6f 6b75 2063 6f6e  est Ichimoku con
-000253a0: 7665 7273 696f 6e20 6c69 6e65 0a20 2020  version line.   
-000253b0: 2020 2020 2069 6620 6162 6f76 6543 6c6f       if aboveClo
-000253c0: 7564 546f 7020 616e 6420 6466 5f6e 6577  udTop and df_new
-000253d0: 5b22 494b 535f 3236 225d 2e69 6c6f 635b  ["IKS_26"].iloc[
-000253e0: 305d 203c 2064 665f 6e65 775b 2249 5453  0] < df_new["ITS
-000253f0: 5f39 225d 2e69 6c6f 635b 305d 3a0a 2020  _9"].iloc[0]:.  
-00025400: 2020 2020 2020 2020 2020 2320 5374 6f63            # Stoc
-00025410: 6852 5349 2063 726f 7373 6564 2032 3020  hRSI crossed 20 
-00025420: 616e 6420 5253 4920 3e20 3530 0a20 2020  and RSI > 50.   
-00025430: 2020 2020 2020 2020 2069 6620 666b 203e           if fk >
-00025440: 2032 3020 616e 6420 7265 6365 6e74 5b22   20 and recent["
-00025450: 5253 4922 5d2e 696c 6f63 5b30 5d20 3e20  RSI"].iloc[0] > 
-00025460: 3530 3a0a 2020 2020 2020 2020 2020 2020  50:.            
-00025470: 2020 2020 2320 636f 6e64 6974 696f 6e20      # condition 
-00025480: 6f66 2063 726f 7373 696e 6720 7468 6520  of crossing the 
-00025490: 5374 6f63 6852 5349 206d 6169 6e20 7369  StochRSI main si
-000254a0: 676e 616c 206c 696e 6520 6672 6f6d 2062  gnal line from b
-000254b0: 6f74 746f 6d20 746f 2074 6f70 0a20 2020  ottom to top.   
-000254c0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000254d0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000254e0: 2020 2020 2020 6461 7461 5b22 4641 5354        data["FAST
-000254f0: 4422 5d2e 696c 6f63 5b31 3030 5d20 3c20  D"].iloc[100] < 
-00025500: 6461 7461 5b22 4641 5354 4b22 5d2e 696c  data["FASTK"].il
-00025510: 6f63 5b31 3030 5d0a 2020 2020 2020 2020  oc[100].        
-00025520: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-00025530: 6461 7461 5b22 4641 5354 4422 5d2e 696c  data["FASTD"].il
-00025540: 6f63 5b31 3031 5d20 3e20 6461 7461 5b22  oc[101] > data["
-00025550: 4641 5354 4b22 5d2e 696c 6f63 5b31 3031  FASTK"].iloc[101
-00025560: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-00025570: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
-00025580: 2020 2020 2020 2020 2023 2063 6c6f 7365           # close
-00025590: 203e 2035 3020 7065 7269 6f64 2053 4d41   > 50 period SMA
-000255a0: 2f45 4d41 2061 6e64 2032 3030 2070 6572  /EMA and 200 per
-000255b0: 696f 6420 534d 412f 454d 410a 2020 2020  iod SMA/EMA.    
-000255c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000255d0: 6966 2028 0a20 2020 2020 2020 2020 2020  if (.           
-000255e0: 2020 2020 2020 2020 2020 2020 2072 6563               rec
-000255f0: 656e 745b 2253 534d 4122 5d2e 696c 6f63  ent["SSMA"].iloc
-00025600: 5b30 5d20 3e20 7265 6365 6e74 5b22 534d  [0] > recent["SM
-00025610: 4122 5d2e 696c 6f63 5b30 5d0a 2020 2020  A"].iloc[0].    
-00025620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025630: 2020 2020 616e 6420 7265 6365 6e74 5b22      and recent["
-00025640: 436c 6f73 6522 5d2e 696c 6f63 5b30 5d20  Close"].iloc[0] 
-00025650: 3e20 7265 6365 6e74 5b22 5353 4d41 225d  > recent["SSMA"]
-00025660: 2e69 6c6f 635b 305d 0a20 2020 2020 2020  .iloc[0].       
-00025670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025680: 2061 6e64 2072 6563 656e 745b 2243 6c6f   and recent["Clo
-00025690: 7365 225d 2e69 6c6f 635b 305d 203e 2072  se"].iloc[0] > r
-000256a0: 6563 656e 745b 224c 4d41 225d 2e69 6c6f  ecent["LMA"].ilo
-000256b0: 635b 305d 0a20 2020 2020 2020 2020 2020  c[0].           
-000256c0: 2020 2020 2020 2020 2029 3a0a 2020 2020           ):.    
-000256d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000256e0: 2020 2020 7361 7665 6420 3d20 7365 6c66      saved = self
-000256f0: 2e66 696e 6443 7572 7265 6e74 5361 7665  .findCurrentSave
-00025700: 6456 616c 7565 2873 6372 6565 6e44 6963  dValue(screenDic
-00025710: 742c 7361 7665 4469 6374 2c22 4d41 2d53  t,saveDict,"MA-S
-00025720: 6967 6e61 6c22 290a 2020 2020 2020 2020  ignal").        
-00025730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025740: 7363 7265 656e 4469 6374 5b22 4d41 2d53  screenDict["MA-S
-00025750: 6967 6e61 6c22 5d20 3d20 280a 2020 2020  ignal"] = (.    
-00025760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025770: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
-00025780: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
-00025790: 4420 2b20 636f 6c6f 7254 6578 742e 4752  D + colorText.GR
-000257a0: 4545 4e20 2b20 2242 756c 6c69 7368 2220  EEN + "Bullish" 
-000257b0: 2b20 636f 6c6f 7254 6578 742e 454e 440a  + colorText.END.
-000257c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000257d0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-000257e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000257f0: 2020 7361 7665 4469 6374 5b22 4d41 2d53    saveDict["MA-S
-00025800: 6967 6e61 6c22 5d20 3d20 7361 7665 645b  ignal"] = saved[
-00025810: 315d 202b 2022 4275 6c6c 6973 6822 0a20  1] + "Bullish". 
-00025820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025830: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-00025840: 7565 0a20 2020 2020 2020 2072 6574 7572  ue.        retur
-00025850: 6e20 4661 6c73 650a 2020 2020 0a20 2020  n False.    .   
-00025860: 2023 2056 616c 6964 6174 6520 5643 5020   # Validate VCP 
-00025870: 6173 2070 6572 204d 6172 6b20 4d69 6e65  as per Mark Mine
-00025880: 7276 696e 690a 2020 2020 2320 6874 7470  rvini.    # http
-00025890: 733a 2f2f 6368 6172 7469 6e6b 2e63 6f6d  s://chartink.com
-000258a0: 2f73 6372 6565 6e65 722f 766f 6c61 7469  /screener/volati
-000258b0: 6c69 7479 2d63 6f6d 7072 6573 7369 6f6e  lity-compression
-000258c0: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-000258d0: 6556 4350 4d61 726b 4d69 6e65 7276 696e  eVCPMarkMinervin
-000258e0: 6928 7365 6c66 2c20 6466 3a70 642e 4461  i(self, df:pd.Da
-000258f0: 7461 4672 616d 652c 2073 6372 6565 6e44  taFrame, screenD
-00025900: 6963 742c 2073 6176 6544 6963 7429 3a0a  ict, saveDict):.
-00025910: 2020 2020 2020 2020 6966 2064 6620 6973          if df is
-00025920: 204e 6f6e 6520 6f72 206c 656e 2864 6629   None or len(df)
-00025930: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
-00025940: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-00025950: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
-00025960: 662e 636f 7079 2829 0a20 2020 2020 2020  f.copy().       
-00025970: 206f 686c 635f 6469 6374 203d 207b 0a20   ohlc_dict = {. 
-00025980: 2020 2020 2020 2020 2020 2027 4f70 656e             'Open
-00025990: 273a 2766 6972 7374 272c 0a20 2020 2020  ':'first',.     
-000259a0: 2020 2020 2020 2027 4869 6768 273a 276d         'High':'m
-000259b0: 6178 272c 0a20 2020 2020 2020 2020 2020  ax',.           
-000259c0: 2027 4c6f 7727 3a27 6d69 6e27 2c0a 2020   'Low':'min',.  
-000259d0: 2020 2020 2020 2020 2020 2743 6c6f 7365            'Close
-000259e0: 273a 276c 6173 7427 2c0a 2020 2020 2020  ':'last',.      
-000259f0: 2020 2020 2020 2756 6f6c 756d 6527 3a27        'Volume':'
-00025a00: 7375 6d27 0a20 2020 2020 2020 207d 0a20  sum'.        }. 
-00025a10: 2020 2020 2020 2023 2066 696e 616c 5f64         # final_d
-00025a20: 6620 3d20 6466 2e72 6573 616d 706c 6528  f = df.resample(
-00025a30: 2757 2d46 5249 272c 2063 6c6f 7365 643d  'W-FRI', closed=
-00025a40: 276c 6566 7427 292e 6167 6728 6f68 6c63  'left').agg(ohlc
-00025a50: 5f64 6963 7429 2e73 6869 6674 2827 3164  _dict).shift('1d
-00025a60: 2729 0a20 2020 2020 2020 2077 6565 6b6c  ').        weekl
-00025a70: 7944 6174 6120 3d20 6461 7461 2e72 6573  yData = data.res
-00025a80: 616d 706c 6528 2757 2729 2e61 6767 286f  ample('W').agg(o
-00025a90: 686c 635f 6469 6374 290a 2020 2020 2020  hlc_dict).      
-00025aa0: 2020 7265 7665 7273 6564 4461 7461 203d    reversedData =
-00025ab0: 2064 6174 615b 3a3a 2d31 5d20 2023 2052   data[::-1]  # R
-00025ac0: 6576 6572 7365 2074 6865 2064 6174 6166  everse the dataf
-00025ad0: 7261 6d65 0a20 2020 2020 2020 2072 6563  rame.        rec
-00025ae0: 656e 745f 636c 6f73 6520 3d20 6461 7461  ent_close = data
-00025af0: 5b22 436c 6f73 6522 5d2e 6865 6164 2831  ["Close"].head(1
-00025b00: 292e 696c 6f63 5b30 5d0a 2020 2020 2020  ).iloc[0].      
-00025b10: 2020 775f 656d 615f 3133 203d 2070 6b74    w_ema_13 = pkt
-00025b20: 616c 6962 2e45 4d41 2877 6565 6b6c 7944  alib.EMA(weeklyD
-00025b30: 6174 615b 2243 6c6f 7365 225d 2c74 696d  ata["Close"],tim
-00025b40: 6570 6572 696f 643d 3133 292e 7461 696c  eperiod=13).tail
-00025b50: 2831 292e 696c 6f63 5b30 5d0a 2020 2020  (1).iloc[0].    
-00025b60: 2020 2020 775f 656d 615f 3236 203d 2070      w_ema_26 = p
-00025b70: 6b74 616c 6962 2e45 4d41 2877 6565 6b6c  ktalib.EMA(weekl
-00025b80: 7944 6174 615b 2243 6c6f 7365 225d 2c74  yData["Close"],t
-00025b90: 696d 6570 6572 696f 643d 3236 292e 7461  imeperiod=26).ta
-00025ba0: 696c 2831 292e 696c 6f63 5b30 5d0a 2020  il(1).iloc[0].  
-00025bb0: 2020 2020 2020 775f 736d 615f 3530 203d        w_sma_50 =
-00025bc0: 2070 6b74 616c 6962 2e53 4d41 2877 6565   pktalib.SMA(wee
-00025bd0: 6b6c 7944 6174 615b 2243 6c6f 7365 225d  klyData["Close"]
-00025be0: 2c74 696d 6570 6572 696f 643d 3530 292e  ,timeperiod=50).
-00025bf0: 7461 696c 2831 292e 696c 6f63 5b30 5d0a  tail(1).iloc[0].
-00025c00: 2020 2020 2020 2020 775f 736d 615f 3430          w_sma_40
-00025c10: 203d 2070 6b74 616c 6962 2e53 4d41 2877   = pktalib.SMA(w
-00025c20: 6565 6b6c 7944 6174 615b 2243 6c6f 7365  eeklyData["Close
-00025c30: 225d 2c74 696d 6570 6572 696f 643d 3430  "],timeperiod=40
-00025c40: 292e 7461 696c 2831 292e 696c 6f63 5b30  ).tail(1).iloc[0
-00025c50: 5d0a 2020 2020 2020 2020 775f 736d 615f  ].        w_sma_
-00025c60: 3430 5f35 775f 6167 6f20 3d20 706b 7461  40_5w_ago = pkta
-00025c70: 6c69 622e 534d 4128 7765 656b 6c79 4461  lib.SMA(weeklyDa
-00025c80: 7461 2e68 6561 6428 6c65 6e28 7765 656b  ta.head(len(week
-00025c90: 6c79 4461 7461 292d 3529 5b22 436c 6f73  lyData)-5)["Clos
-00025ca0: 6522 5d2c 7469 6d65 7065 7269 6f64 3d34  e"],timeperiod=4
-00025cb0: 3029 2e74 6169 6c28 3129 2e69 6c6f 635b  0).tail(1).iloc[
-00025cc0: 305d 0a20 2020 2020 2020 2077 5f6d 696e  0].        w_min
-00025cd0: 5f35 3020 3d20 6d69 6e28 312e 332a 7765  _50 = min(1.3*we
-00025ce0: 656b 6c79 4461 7461 2e74 6169 6c28 3530  eklyData.tail(50
-00025cf0: 295b 224c 6f77 225d 290a 2020 2020 2020  )["Low"]).      
-00025d00: 2020 775f 6d61 785f 3530 203d 206d 6178    w_max_50 = max
-00025d10: 2830 2e37 352a 7765 656b 6c79 4461 7461  (0.75*weeklyData
-00025d20: 2e74 6169 6c28 3530 295b 2248 6967 6822  .tail(50)["High"
-00025d30: 5d29 0a20 2020 2020 2020 2077 5f65 6d61  ]).        w_ema
-00025d40: 5f32 365f 3230 775f 6167 6f20 3d20 706b  _26_20w_ago = pk
-00025d50: 7461 6c69 622e 454d 4128 7765 656b 6c79  talib.EMA(weekly
-00025d60: 4461 7461 2e68 6561 6428 6c65 6e28 7765  Data.head(len(we
-00025d70: 656b 6c79 4461 7461 292d 3230 295b 2243  eklyData)-20)["C
-00025d80: 6c6f 7365 225d 2c74 696d 6570 6572 696f  lose"],timeperio
-00025d90: 643d 3236 292e 7461 696c 2831 292e 696c  d=26).tail(1).il
-00025da0: 6f63 5b30 5d0a 2020 2020 2020 2020 7265  oc[0].        re
-00025db0: 6365 6e74 5f65 6d61 5f31 335f 3230 645f  cent_ema_13_20d_
-00025dc0: 6167 6f20 3d20 706b 7461 6c69 622e 454d  ago = pktalib.EM
-00025dd0: 4128 7265 7665 7273 6564 4461 7461 2e68  A(reversedData.h
-00025de0: 6561 6428 6c65 6e28 7265 7665 7273 6564  ead(len(reversed
-00025df0: 4461 7461 292d 3230 295b 2243 6c6f 7365  Data)-20)["Close
-00025e00: 225d 2c74 696d 6570 6572 696f 643d 3133  "],timeperiod=13
-00025e10: 292e 7461 696c 2831 292e 696c 6f63 5b30  ).tail(1).iloc[0
-00025e20: 5d0a 2020 2020 2020 2020 775f 736d 615f  ].        w_sma_
-00025e30: 3430 5f35 775f 6167 6f20 3d20 706b 7461  40_5w_ago = pkta
-00025e40: 6c69 622e 534d 4128 7765 656b 6c79 4461  lib.SMA(weeklyDa
-00025e50: 7461 2e68 6561 6428 6c65 6e28 7765 656b  ta.head(len(week
-00025e60: 6c79 4461 7461 292d 3529 5b22 436c 6f73  lyData)-5)["Clos
-00025e70: 6522 5d2c 7469 6d65 7065 7269 6f64 3d34  e"],timeperiod=4
-00025e80: 3029 2e74 6169 6c28 3129 2e69 6c6f 635b  0).tail(1).iloc[
-00025e90: 305d 0a20 2020 2020 2020 2077 5f73 6d61  0].        w_sma
-00025ea0: 5f34 305f 3130 775f 6167 6f20 3d20 706b  _40_10w_ago = pk
-00025eb0: 7461 6c69 622e 534d 4128 7765 656b 6c79  talib.SMA(weekly
-00025ec0: 4461 7461 2e68 6561 6428 6c65 6e28 7765  Data.head(len(we
-00025ed0: 656b 6c79 4461 7461 292d 3130 295b 2243  eklyData)-10)["C
-00025ee0: 6c6f 7365 225d 2c74 696d 6570 6572 696f  lose"],timeperio
-00025ef0: 643d 3430 292e 7461 696c 2831 292e 696c  d=40).tail(1).il
-00025f00: 6f63 5b30 5d0a 2020 2020 2020 2020 7265  oc[0].        re
-00025f10: 6365 6e74 5f73 6d61 5f35 3020 3d20 706b  cent_sma_50 = pk
-00025f20: 7461 6c69 622e 534d 4128 7265 7665 7273  talib.SMA(revers
-00025f30: 6564 4461 7461 5b22 436c 6f73 6522 5d2c  edData["Close"],
-00025f40: 7469 6d65 7065 7269 6f64 3d35 3029 2e74  timeperiod=50).t
-00025f50: 6169 6c28 3129 2e69 6c6f 635b 305d 0a20  ail(1).iloc[0]. 
-00025f60: 2020 2020 2020 2077 5f77 6d61 5f38 203d         w_wma_8 =
-00025f70: 2070 6b74 616c 6962 2e57 4d41 2877 6565   pktalib.WMA(wee
-00025f80: 6b6c 7944 6174 615b 2243 6c6f 7365 225d  klyData["Close"]
-00025f90: 2c74 696d 6570 6572 696f 643d 3829 2e74  ,timeperiod=8).t
-00025fa0: 6169 6c28 3129 2e69 6c6f 635b 305d 0a20  ail(1).iloc[0]. 
-00025fb0: 2020 2020 2020 2077 5f73 6d61 5f38 203d         w_sma_8 =
-00025fc0: 2070 6b74 616c 6962 2e53 4d41 2877 6565   pktalib.SMA(wee
-00025fd0: 6b6c 7944 6174 615b 2243 6c6f 7365 225d  klyData["Close"]
-00025fe0: 2c74 696d 6570 6572 696f 643d 3829 2e74  ,timeperiod=8).t
-00025ff0: 6169 6c28 3129 2e69 6c6f 635b 305d 0a20  ail(1).iloc[0]. 
-00026000: 2020 2020 2020 206e 756d 5072 6576 696f         numPrevio
-00026010: 7573 4361 6e64 6c65 7320 3d20 3230 0a20  usCandles = 20. 
-00026020: 2020 2020 2020 2070 756c 6c62 6163 6b44         pullbackD
-00026030: 6174 6120 3d20 6461 7461 2e68 6561 6428  ata = data.head(
-00026040: 6e75 6d50 7265 7669 6f75 7343 616e 646c  numPreviousCandl
-00026050: 6573 290a 2020 2020 2020 2020 7075 6c6c  es).        pull
-00026060: 6261 636b 4461 7461 2e6c 6f63 5b3a 2c27  backData.loc[:,'
-00026070: 5075 6c6c 4261 636b 275d 203d 2070 756c  PullBack'] = pul
-00026080: 6c62 6163 6b44 6174 615b 2243 6c6f 7365  lbackData["Close
-00026090: 225d 2e6c 7428 7075 6c6c 6261 636b 4461  "].lt(pullbackDa
-000260a0: 7461 5b22 4f70 656e 225d 2920 232e 7368  ta["Open"]) #.sh
-000260b0: 6966 7428 7065 7269 6f64 733d 3129 2920  ift(periods=1)) 
-000260c0: 2326 2064 6174 615b 224c 6f77 225d 2e6c  #& data["Low"].l
-000260d0: 7428 6461 7461 5b22 4c6f 7722 5d2e 7368  t(data["Low"].sh
-000260e0: 6966 7428 7065 7269 6f64 733d 3129 290a  ift(periods=1)).
-000260f0: 2020 2020 2020 2020 7368 7269 6e6b 6564          shrinked
-00026100: 566f 6c44 6174 6120 3d20 7075 6c6c 6261  VolData = pullba
-00026110: 636b 4461 7461 5b70 756c 6c62 6163 6b44  ckData[pullbackD
-00026120: 6174 615b 2250 756c 6c42 6163 6b22 5d20  ata["PullBack"] 
-00026130: 3d3d 2054 7275 655d 2e68 6561 6428 6e75  == True].head(nu
-00026140: 6d50 7265 7669 6f75 7343 616e 646c 6573  mPreviousCandles
-00026150: 290a 2020 2020 2020 2020 7265 6365 6e74  ).        recent
-00026160: 4c61 7267 6573 7456 6f6c 756d 6520 3d20  LargestVolume = 
-00026170: 6d61 7828 7075 6c6c 6261 636b 4461 7461  max(pullbackData
-00026180: 5b70 756c 6c62 6163 6b44 6174 615b 2250  [pullbackData["P
-00026190: 756c 6c42 6163 6b22 5d20 3d3d 2046 616c  ullBack"] == Fal
-000261a0: 7365 5d2e 6865 6164 2833 295b 2256 6f6c  se].head(3)["Vol
-000261b0: 756d 6522 5d29 0a20 2020 2020 2020 2023  ume"]).        #
-000261c0: 2070 756c 6c62 6163 6b44 6174 612e 6c6f   pullbackData.lo
-000261d0: 635b 3a2c 2750 4256 6f6c 5261 7469 6f27  c[:,'PBVolRatio'
-000261e0: 5d20 3d20 7075 6c6c 6261 636b 4461 7461  ] = pullbackData
-000261f0: 5b22 566f 6c75 6d65 225d 2f72 6563 656e  ["Volume"]/recen
-00026200: 744c 6172 6765 7374 566f 6c75 6d65 0a20  tLargestVolume. 
-00026210: 2020 2020 2020 2076 6f6c 496e 5072 6576         volInPrev
-00026220: 696f 7573 5075 6c6c 6261 636b 7353 6872  iousPullbacksShr
-00026230: 696e 6b65 6420 3d20 4661 6c73 650a 2020  inked = False.  
-00026240: 2020 2020 2020 6966 206e 6f74 2073 6872        if not shr
-00026250: 696e 6b65 6456 6f6c 4461 7461 2e65 6d70  inkedVolData.emp
-00026260: 7479 3a0a 2020 2020 2020 2020 2020 2020  ty:.            
-00026270: 696e 6465 7820 3d20 300a 2020 2020 2020  index = 0.      
-00026280: 2020 2020 2020 7768 696c 6520 696e 6465        while inde
-00026290: 7820 3c20 6c65 6e28 7368 7269 6e6b 6564  x < len(shrinked
-000262a0: 566f 6c44 6174 6129 3a0a 2020 2020 2020  VolData):.      
-000262b0: 2020 2020 2020 2020 2020 766f 6c49 6e50            volInP
-000262c0: 7265 7669 6f75 7350 756c 6c62 6163 6b73  reviousPullbacks
-000262d0: 5368 7269 6e6b 6564 203d 2073 6872 696e  Shrinked = shrin
-000262e0: 6b65 6456 6f6c 4461 7461 5b22 566f 6c75  kedVolData["Volu
-000262f0: 6d65 225d 2e69 6c6f 635b 696e 6465 785d  me"].iloc[index]
-00026300: 203c 2073 656c 662e 636f 6e66 6967 4d61   < self.configMa
-00026310: 6e61 6765 722e 7663 7056 6f6c 756d 6543  nager.vcpVolumeC
-00026320: 6f6e 7472 6163 7469 6f6e 5261 7469 6f20  ontractionRatio 
-00026330: 2a20 7265 6365 6e74 4c61 7267 6573 7456  * recentLargestV
-00026340: 6f6c 756d 650a 2020 2020 2020 2020 2020  olume.          
-00026350: 2020 2020 2020 6966 206e 6f74 2076 6f6c        if not vol
-00026360: 496e 5072 6576 696f 7573 5075 6c6c 6261  InPreviousPullba
-00026370: 636b 7353 6872 696e 6b65 643a 0a20 2020  cksShrinked:.   
-00026380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026390: 2062 7265 616b 0a20 2020 2020 2020 2020   break.         
-000263a0: 2020 2020 2020 2069 6e64 6578 202b 3d20         index += 
-000263b0: 310a 2020 2020 2020 2020 7265 6365 6e74  1.        recent
-000263c0: 566f 6c75 6d65 4861 7341 626f 7665 4176  VolumeHasAboveAv
-000263d0: 6756 6f6c 203d 2072 6563 656e 744c 6172  gVol = recentLar
-000263e0: 6765 7374 566f 6c75 6d65 203e 3d20 7365  gestVolume >= se
-000263f0: 6c66 2e63 6f6e 6669 674d 616e 6167 6572  lf.configManager
-00026400: 2e76 6f6c 756d 6552 6174 696f 202a 2064  .volumeRatio * d
-00026410: 6174 615b 2256 6f6c 4d41 225d 2e69 6c6f  ata["VolMA"].ilo
-00026420: 635b 305d 0a20 2020 2020 2020 2069 7356  c[0].        isV
-00026430: 4350 203d 2077 5f65 6d61 5f31 3320 3e20  CP = w_ema_13 > 
-00026440: 775f 656d 615f 3236 2061 6e64 205c 0a20  w_ema_26 and \. 
-00026450: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-00026460: 5f65 6d61 5f32 3620 3e20 775f 736d 615f  _ema_26 > w_sma_
-00026470: 3530 2061 6e64 205c 0a20 2020 2020 2020  50 and \.       
-00026480: 2020 2020 2020 2020 2077 5f73 6d61 5f34           w_sma_4
-00026490: 3020 3e20 775f 736d 615f 3430 5f35 775f  0 > w_sma_40_5w_
-000264a0: 6167 6f20 616e 6420 5c0a 2020 2020 2020  ago and \.      
-000264b0: 2020 2020 2020 2020 2020 7265 6365 6e74            recent
-000264c0: 5f63 6c6f 7365 203e 3d20 775f 6d69 6e5f  _close >= w_min_
-000264d0: 3530 2061 6e64 205c 0a20 2020 2020 2020  50 and \.       
-000264e0: 2020 2020 2020 2020 2072 6563 656e 745f           recent_
-000264f0: 636c 6f73 6520 3e3d 2077 5f6d 6178 5f35  close >= w_max_5
-00026500: 3020 616e 6420 5c0a 2020 2020 2020 2020  0 and \.        
-00026510: 2020 2020 2020 2020 7265 6365 6e74 5f65          recent_e
-00026520: 6d61 5f31 335f 3230 645f 6167 6f20 3e20  ma_13_20d_ago > 
-00026530: 775f 656d 615f 3236 5f32 3077 5f61 676f  w_ema_26_20w_ago
-00026540: 2061 6e64 205c 0a20 2020 2020 2020 2020   and \.         
-00026550: 2020 2020 2020 2077 5f73 6d61 5f34 305f         w_sma_40_
-00026560: 3577 5f61 676f 203e 2077 5f73 6d61 5f34  5w_ago > w_sma_4
-00026570: 305f 3130 775f 6167 6f20 616e 6420 5c0a  0_10w_ago and \.
-00026580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026590: 7265 6365 6e74 5f63 6c6f 7365 203e 2072  recent_close > r
-000265a0: 6563 656e 745f 736d 615f 3530 2061 6e64  ecent_sma_50 and
-000265b0: 205c 0a20 2020 2020 2020 2020 2020 2020   \.             
-000265c0: 2020 2028 775f 776d 615f 3820 2d20 775f     (w_wma_8 - w_
-000265d0: 736d 615f 3829 2a36 2f32 3920 3c20 302e  sma_8)*6/29 < 0.
-000265e0: 3520 616e 6420 5c0a 2020 2020 2020 2020  5 and \.        
-000265f0: 2020 2020 2020 2020 766f 6c49 6e50 7265          volInPre
-00026600: 7669 6f75 7350 756c 6c62 6163 6b73 5368  viousPullbacksSh
-00026610: 7269 6e6b 6564 2061 6e64 205c 0a20 2020  rinked and \.   
-00026620: 2020 2020 2020 2020 2020 2020 2072 6563               rec
-00026630: 656e 7456 6f6c 756d 6548 6173 4162 6f76  entVolumeHasAbov
-00026640: 6541 7667 566f 6c20 616e 6420 5c0a 2020  eAvgVol and \.  
-00026650: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00026660: 6365 6e74 5f63 6c6f 7365 203e 2031 300a  cent_close > 10.
-00026670: 2020 2020 2020 2020 6966 2069 7356 4350          if isVCP
-00026680: 3a0a 2020 2020 2020 2020 2020 2020 7361  :.            sa
-00026690: 7665 6420 3d20 7365 6c66 2e66 696e 6443  ved = self.findC
-000266a0: 7572 7265 6e74 5361 7665 6456 616c 7565  urrentSavedValue
-000266b0: 2873 6372 6565 6e44 6963 742c 2073 6176  (screenDict, sav
-000266c0: 6544 6963 742c 2022 5061 7474 6572 6e22  eDict, "Pattern"
-000266d0: 290a 2020 2020 2020 2020 2020 2020 7363  ).            sc
-000266e0: 7265 656e 4469 6374 5b22 5061 7474 6572  reenDict["Patter
-000266f0: 6e22 5d20 3d20 280a 2020 2020 2020 2020  n"] = (.        
-00026700: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
-00026710: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-00026720: 2020 2b20 636f 6c6f 7254 6578 742e 424f    + colorText.BO
-00026730: 4c44 0a20 2020 2020 2020 2020 2020 2020  LD.             
-00026740: 2020 202b 2063 6f6c 6f72 5465 7874 2e47     + colorText.G
-00026750: 5245 454e 0a20 2020 2020 2020 2020 2020  REEN.           
-00026760: 2020 2020 202b 2066 2256 4350 284d 696e       + f"VCP(Min
-00026770: 6572 7669 6e69 2922 0a20 2020 2020 2020  ervini)".       
-00026780: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
-00026790: 5465 7874 2e45 4e44 0a20 2020 2020 2020  Text.END.       
-000267a0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-000267b0: 2020 2073 6176 6544 6963 745b 2250 6174     saveDict["Pat
-000267c0: 7465 726e 225d 203d 2073 6176 6564 5b31  tern"] = saved[1
-000267d0: 5d20 2b20 6622 5643 5028 4d69 6e65 7276  ] + f"VCP(Minerv
-000267e0: 696e 6929 220a 2020 2020 2020 2020 7265  ini)".        re
-000267f0: 7475 726e 2069 7356 4350 0a20 2020 200a  turn isVCP.    .
-00026800: 2020 2020 2320 5661 6c69 6461 7465 2056      # Validate V
-00026810: 4350 0a20 2020 2064 6566 2076 616c 6964  CP.    def valid
-00026820: 6174 6556 4350 280a 2020 2020 2020 2020  ateVCP(.        
-00026830: 7365 6c66 2c20 6466 2c20 7363 7265 656e  self, df, screen
-00026840: 4469 6374 2c20 7361 7665 4469 6374 2c20  Dict, saveDict, 
-00026850: 7374 6f63 6b4e 616d 653d 4e6f 6e65 2c20  stockName=None, 
-00026860: 7769 6e64 6f77 3d33 2c20 7065 7263 656e  window=3, percen
-00026870: 7461 6765 4672 6f6d 546f 703d 330a 2020  tageFromTop=3.  
-00026880: 2020 293a 0a20 2020 2020 2020 2069 6620    ):.        if 
-00026890: 6466 2069 7320 4e6f 6e65 206f 7220 6c65  df is None or le
-000268a0: 6e28 6466 2920 3d3d 2030 3a0a 2020 2020  n(df) == 0:.    
-000268b0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-000268c0: 616c 7365 0a20 2020 2020 2020 2064 6174  alse.        dat
-000268d0: 6120 3d20 6466 2e63 6f70 7928 290a 2020  a = df.copy().  
-000268e0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-000268f0: 2020 2020 2020 2070 6572 6365 6e74 6167         percentag
-00026900: 6546 726f 6d54 6f70 202f 3d20 3130 300a  eFromTop /= 100.
-00026910: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00026920: 2e72 6573 6574 5f69 6e64 6578 2869 6e70  .reset_index(inp
-00026930: 6c61 6365 3d54 7275 6529 0a20 2020 2020  lace=True).     
-00026940: 2020 2020 2020 2064 6174 612e 7265 6e61         data.rena
-00026950: 6d65 2863 6f6c 756d 6e73 3d7b 2269 6e64  me(columns={"ind
-00026960: 6578 223a 2022 4461 7465 227d 2c20 696e  ex": "Date"}, in
-00026970: 706c 6163 653d 5472 7565 290a 2020 2020  place=True).    
-00026980: 2020 2020 2020 2020 6461 7461 5b22 746f          data["to
-00026990: 7073 225d 203d 2028 6461 7461 5b22 4869  ps"] = (data["Hi
-000269a0: 6768 225d 2e69 6c6f 635b 6c69 7374 2870  gh"].iloc[list(p
-000269b0: 6b74 616c 6962 2e61 7267 7265 6c65 7874  ktalib.argrelext
-000269c0: 7265 6d61 286e 702e 6172 7261 7928 6461  rema(np.array(da
-000269d0: 7461 5b22 4869 6768 225d 292c 206e 702e  ta["High"]), np.
-000269e0: 6772 6561 7465 725f 6571 7561 6c2c 206f  greater_equal, o
-000269f0: 7264 6572 3d77 696e 646f 7729 5b30 5d29  rder=window)[0])
-00026a00: 5d2e 6865 6164 2834 2929 0a20 2020 2020  ].head(4)).     
-00026a10: 2020 2020 2020 2064 6174 615b 2262 6f74         data["bot
-00026a20: 7322 5d20 3d20 2864 6174 615b 224c 6f77  s"] = (data["Low
-00026a30: 225d 2e69 6c6f 635b 6c69 7374 2870 6b74  "].iloc[list(pkt
-00026a40: 616c 6962 2e61 7267 7265 6c65 7874 7265  alib.argrelextre
-00026a50: 6d61 286e 702e 6172 7261 7928 6461 7461  ma(np.array(data
-00026a60: 5b22 4c6f 7722 5d29 2c20 6e70 2e6c 6573  ["Low"]), np.les
-00026a70: 735f 6571 7561 6c2c 206f 7264 6572 3d77  s_equal, order=w
-00026a80: 696e 646f 7729 5b30 5d29 5d2e 6865 6164  indow)[0])].head
-00026a90: 2834 2929 0a20 2020 2020 2020 2020 2020  (4)).           
-00026aa0: 2064 6174 6120 3d20 6461 7461 2e66 696c   data = data.fil
-00026ab0: 6c6e 6128 3029 0a20 2020 2020 2020 2020  lna(0).         
-00026ac0: 2020 2064 6174 6120 3d20 6461 7461 2e72     data = data.r
-00026ad0: 6570 6c61 6365 285b 6e70 2e69 6e66 2c20  eplace([np.inf, 
-00026ae0: 2d6e 702e 696e 665d 2c20 3029 0a20 2020  -np.inf], 0).   
-00026af0: 2020 2020 2020 2020 2074 6f70 7320 3d20           tops = 
-00026b00: 6461 7461 5b64 6174 612e 746f 7073 203e  data[data.tops >
-00026b10: 2030 5d0a 2020 2020 2020 2020 2020 2020   0].            
-00026b20: 2320 626f 7473 203d 2064 6174 615b 6461  # bots = data[da
-00026b30: 7461 2e62 6f74 7320 3e20 305d 0a20 2020  ta.bots > 0].   
-00026b40: 2020 2020 2020 2020 2068 6967 6865 7374           highest
-00026b50: 546f 7020 3d20 726f 756e 6428 746f 7073  Top = round(tops
-00026b60: 2e64 6573 6372 6962 6528 295b 2248 6967  .describe()["Hig
-00026b70: 6822 5d5b 226d 6178 225d 2c20 3129 0a20  h"]["max"], 1). 
-00026b80: 2020 2020 2020 2020 2020 2066 696c 7465             filte
-00026b90: 7265 6454 6f70 7320 3d20 746f 7073 5b0a  redTops = tops[.
-00026ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026bb0: 746f 7073 2e74 6f70 7320 3e20 2868 6967  tops.tops > (hig
-00026bc0: 6865 7374 546f 7020 2d20 2868 6967 6865  hestTop - (highe
-00026bd0: 7374 546f 7020 2a20 7065 7263 656e 7461  stTop * percenta
-00026be0: 6765 4672 6f6d 546f 7029 290a 2020 2020  geFromTop)).    
-00026bf0: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
-00026c00: 2020 2020 2020 6966 2066 696c 7465 7265        if filtere
-00026c10: 6454 6f70 732e 6571 7561 6c73 2874 6f70  dTops.equals(top
-00026c20: 7329 3a20 2023 2054 6f70 7320 6172 6520  s):  # Tops are 
-00026c30: 696e 2074 6865 2072 616e 6765 0a20 2020  in the range.   
-00026c40: 2020 2020 2020 2020 2020 2020 206c 6f77               low
-00026c50: 506f 696e 7473 203d 205b 5d0a 2020 2020  Points = [].    
-00026c60: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00026c70: 6920 696e 2072 616e 6765 286c 656e 2874  i in range(len(t
-00026c80: 6f70 7329 202d 2031 293a 0a20 2020 2020  ops) - 1):.     
-00026c90: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00026ca0: 6e64 4461 7465 203d 2074 6f70 732e 696c  ndDate = tops.il
-00026cb0: 6f63 5b69 5d5b 2244 6174 6522 5d0a 2020  oc[i]["Date"].  
-00026cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026cd0: 2020 7374 6172 7444 6174 6520 3d20 746f    startDate = to
-00026ce0: 7073 2e69 6c6f 635b 6920 2b20 315d 5b22  ps.iloc[i + 1]["
-00026cf0: 4461 7465 225d 0a20 2020 2020 2020 2020  Date"].         
-00026d00: 2020 2020 2020 2020 2020 206c 6f77 506f             lowPo
-00026d10: 696e 7473 2e61 7070 656e 6428 0a20 2020  ints.append(.   
-00026d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026d30: 2020 2020 2064 6174 615b 0a20 2020 2020       data[.     
-00026d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026d50: 2020 2020 2020 2028 6461 7461 2e44 6174         (data.Dat
-00026d60: 6520 3e3d 2073 7461 7274 4461 7465 2920  e >= startDate) 
-00026d70: 2620 2864 6174 612e 4461 7465 203c 3d20  & (data.Date <= 
-00026d80: 656e 6444 6174 6529 0a20 2020 2020 2020  endDate).       
-00026d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026da0: 205d 2e64 6573 6372 6962 6528 295b 224c   ].describe()["L
-00026db0: 6f77 225d 5b22 6d69 6e22 5d0a 2020 2020  ow"]["min"].    
-00026dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026dd0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00026de0: 2020 6c6f 7750 6f69 6e74 734f 7267 203d    lowPointsOrg =
-00026df0: 206c 6f77 506f 696e 7473 0a20 2020 2020   lowPoints.     
-00026e00: 2020 2020 2020 2020 2020 206c 6f77 506f             lowPo
-00026e10: 696e 7473 2e73 6f72 7428 7265 7665 7273  ints.sort(revers
-00026e20: 653d 5472 7565 290a 2020 2020 2020 2020  e=True).        
-00026e30: 2020 2020 2020 2020 6c6f 7750 6f69 6e74          lowPoint
-00026e40: 7353 6f72 7465 6420 3d20 6c6f 7750 6f69  sSorted = lowPoi
-00026e50: 6e74 730a 2020 2020 2020 2020 2020 2020  nts.            
-00026e60: 2020 2020 6966 2064 6174 612e 656d 7074      if data.empt
-00026e70: 7920 6f72 206c 656e 286c 6f77 506f 696e  y or len(lowPoin
-00026e80: 7473 2920 3c20 313a 0a20 2020 2020 2020  ts) < 1:.       
-00026e90: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00026ea0: 7572 6e20 4661 6c73 650a 2020 2020 2020  urn False.      
-00026eb0: 2020 2020 2020 2020 2020 6c74 7020 3d20            ltp = 
-00026ec0: 6461 7461 2e68 6561 6428 3129 5b22 436c  data.head(1)["Cl
-00026ed0: 6f73 6522 5d2e 696c 6f63 5b30 5d0a 2020  ose"].iloc[0].  
-00026ee0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00026ef0: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
-00026f00: 2020 2020 2020 206c 6f77 506f 696e 7473         lowPoints
-00026f10: 4f72 6720 3d3d 206c 6f77 506f 696e 7473  Org == lowPoints
-00026f20: 536f 7274 6564 0a20 2020 2020 2020 2020  Sorted.         
-00026f30: 2020 2020 2020 2020 2020 2061 6e64 206c             and l
-00026f40: 7470 203c 2068 6967 6865 7374 546f 700a  tp < highestTop.
-00026f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026f60: 2020 2020 616e 6420 6c74 7020 3e20 6c6f      and ltp > lo
-00026f70: 7750 6f69 6e74 735b 305d 0a20 2020 2020  wPoints[0].     
-00026f80: 2020 2020 2020 2020 2020 2029 3a0a 2020             ):.  
-00026f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026fa0: 2020 7361 7665 6420 3d20 7365 6c66 2e66    saved = self.f
-00026fb0: 696e 6443 7572 7265 6e74 5361 7665 6456  indCurrentSavedV
-00026fc0: 616c 7565 2873 6372 6565 6e44 6963 742c  alue(screenDict,
-00026fd0: 2073 6176 6544 6963 742c 2022 5061 7474   saveDict, "Patt
-00026fe0: 6572 6e22 290a 2020 2020 2020 2020 2020  ern").          
-00026ff0: 2020 2020 2020 2020 2020 7363 7265 656e            screen
-00027000: 4469 6374 5b22 5061 7474 6572 6e22 5d20  Dict["Pattern"] 
-00027010: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-00027020: 2020 2020 2020 2020 2020 2020 7361 7665              save
-00027030: 645b 305d 200a 2020 2020 2020 2020 2020  d[0] .          
-00027040: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-00027050: 636f 6c6f 7254 6578 742e 424f 4c44 0a20  colorText.BOLD. 
-00027060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027070: 2020 2020 2020 202b 2063 6f6c 6f72 5465         + colorTe
-00027080: 7874 2e47 5245 454e 0a20 2020 2020 2020  xt.GREEN.       
-00027090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000270a0: 202b 2066 2256 4350 2028 424f 3a20 7b68   + f"VCP (BO: {h
-000270b0: 6967 6865 7374 546f 707d 2922 0a20 2020  ighestTop})".   
+00023b00: 696e 6465 7820 2b3d 2031 0a20 2020 2020  index += 1.     
+00023b10: 2020 2072 6574 7572 6e56 616c 7565 203d     returnValue =
+00023b20: 206d 6152 6576 6572 7361 6c0a 2020 2020   maReversal.    
+00023b30: 2020 2020 6966 206d 614c 656e 6774 6820      if maLength 
+00023b40: 213d 2030 3a0a 2020 2020 2020 2020 2020  != 0:.          
+00023b50: 2020 7265 7475 726e 5661 6c75 6520 3d20    returnValue = 
+00023b60: 7374 7228 6d61 4c65 6e67 7468 2920 696e  str(maLength) in
+00023b70: 206d 6153 6967 6e61 6c73 0a20 2020 2020   maSignals.     
+00023b80: 2020 2072 6574 7572 6e20 7265 7475 726e     return return
+00023b90: 5661 6c75 650a 0a20 2020 2023 2046 696e  Value..    # Fin
+00023ba0: 6420 4e52 7820 7261 6e67 6520 666f 7220  d NRx range for 
+00023bb0: 5265 7665 7273 616c 0a20 2020 2064 6566  Reversal.    def
+00023bc0: 2076 616c 6964 6174 654e 6172 726f 7752   validateNarrowR
+00023bd0: 616e 6765 2873 656c 662c 2064 662c 2073  ange(self, df, s
+00023be0: 6372 6565 6e44 6963 742c 2073 6176 6544  creenDict, saveD
+00023bf0: 6963 742c 206e 723d 3429 3a0a 2020 2020  ict, nr=4):.    
+00023c00: 2020 2020 6966 2064 6620 6973 204e 6f6e      if df is Non
+00023c10: 6520 6f72 206c 656e 2864 6629 203d 3d20  e or len(df) == 
+00023c20: 303a 0a20 2020 2020 2020 2020 2020 2072  0:.            r
+00023c30: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
+00023c40: 2020 2020 6461 7461 203d 2064 662e 636f      data = df.co
+00023c50: 7079 2829 0a20 2020 2020 2020 2073 6176  py().        sav
+00023c60: 6564 203d 2073 656c 662e 6669 6e64 4375  ed = self.findCu
+00023c70: 7272 656e 7453 6176 6564 5661 6c75 6528  rrentSavedValue(
+00023c80: 7363 7265 656e 4469 6374 2c20 7361 7665  screenDict, save
+00023c90: 4469 6374 2c20 2250 6174 7465 726e 2229  Dict, "Pattern")
+00023ca0: 0a20 2020 2020 2020 2069 6620 504b 4461  .        if PKDa
+00023cb0: 7465 5574 696c 6974 6965 732e 6973 5472  teUtilities.isTr
+00023cc0: 6164 696e 6754 696d 6528 293a 0a20 2020  adingTime():.   
+00023cd0: 2020 2020 2020 2020 2072 616e 6765 4461           rangeDa
+00023ce0: 7461 203d 2064 6174 612e 6865 6164 286e  ta = data.head(n
+00023cf0: 7220 2b20 3129 5b31 3a5d 0a20 2020 2020  r + 1)[1:].     
+00023d00: 2020 2020 2020 206e 6f77 5f63 616e 646c         now_candl
+00023d10: 6520 3d20 6461 7461 2e68 6561 6428 3129  e = data.head(1)
+00023d20: 0a20 2020 2020 2020 2020 2020 2072 616e  .            ran
+00023d30: 6765 4461 7461 5b22 5261 6e67 6522 5d20  geData["Range"] 
+00023d40: 3d20 6162 7328 7261 6e67 6544 6174 615b  = abs(rangeData[
+00023d50: 2243 6c6f 7365 225d 202d 2072 616e 6765  "Close"] - range
+00023d60: 4461 7461 5b22 4f70 656e 225d 290a 2020  Data["Open"]).  
+00023d70: 2020 2020 2020 2020 2020 7265 6365 6e74            recent
+00023d80: 203d 2072 616e 6765 4461 7461 2e68 6561   = rangeData.hea
+00023d90: 6428 3129 0a20 2020 2020 2020 2020 2020  d(1).           
+00023da0: 2069 6620 280a 2020 2020 2020 2020 2020   if (.          
+00023db0: 2020 2020 2020 6c65 6e28 7265 6365 6e74        len(recent
+00023dc0: 2920 3d3d 2031 0a20 2020 2020 2020 2020  ) == 1.         
+00023dd0: 2020 2020 2020 2061 6e64 2072 6563 656e         and recen
+00023de0: 745b 2252 616e 6765 225d 2e69 6c6f 635b  t["Range"].iloc[
+00023df0: 305d 203d 3d20 7261 6e67 6544 6174 612e  0] == rangeData.
+00023e00: 6465 7363 7269 6265 2829 5b22 5261 6e67  describe()["Rang
+00023e10: 6522 5d5b 226d 696e 225d 0a20 2020 2020  e"]["min"].     
+00023e20: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
+00023e30: 2020 2020 2020 2020 2020 6966 2028 0a20            if (. 
+00023e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023e50: 2020 2073 656c 662e 6765 7443 616e 646c     self.getCandl
+00023e60: 6554 7970 6528 7265 6365 6e74 290a 2020  eType(recent).  
+00023e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023e80: 2020 616e 6420 6e6f 775f 6361 6e64 6c65    and now_candle
+00023e90: 5b22 436c 6f73 6522 5d2e 696c 6f63 5b30  ["Close"].iloc[0
+00023ea0: 5d20 3e3d 2072 6563 656e 745b 2243 6c6f  ] >= recent["Clo
+00023eb0: 7365 225d 2e69 6c6f 635b 305d 0a20 2020  se"].iloc[0].   
+00023ec0: 2020 2020 2020 2020 2020 2020 2029 3a0a               ):.
+00023ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023ee0: 2020 2020 7363 7265 656e 4469 6374 5b22      screenDict["
+00023ef0: 5061 7474 6572 6e22 5d20 3d20 280a 2020  Pattern"] = (.  
+00023f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023f10: 2020 2020 2020 7361 7665 645b 305d 202b        saved[0] +
+00023f20: 2063 6f6c 6f72 5465 7874 2e42 4f4c 4420   colorText.BOLD 
+00023f30: 2b20 636f 6c6f 7254 6578 742e 4752 4545  + colorText.GREE
+00023f40: 4e20 2b20 6622 4275 792d 4e52 7b6e 727d  N + f"Buy-NR{nr}
+00023f50: 2220 2b20 636f 6c6f 7254 6578 742e 454e  " + colorText.EN
+00023f60: 440a 2020 2020 2020 2020 2020 2020 2020  D.              
+00023f70: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00023f80: 2020 2020 2020 2020 2020 2020 7361 7665              save
+00023f90: 4469 6374 5b22 5061 7474 6572 6e22 5d20  Dict["Pattern"] 
+00023fa0: 3d20 7361 7665 645b 315d 202b 2066 2242  = saved[1] + f"B
+00023fb0: 7579 2d4e 527b 6e72 7d22 0a20 2020 2020  uy-NR{nr}".     
+00023fc0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00023fd0: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
+00023fe0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00023ff0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00024000: 2020 2020 2020 6e6f 7420 7365 6c66 2e67        not self.g
+00024010: 6574 4361 6e64 6c65 5479 7065 2872 6563  etCandleType(rec
+00024020: 656e 7429 0a20 2020 2020 2020 2020 2020  ent).           
+00024030: 2020 2020 2020 2020 2061 6e64 206e 6f77           and now
+00024040: 5f63 616e 646c 655b 2243 6c6f 7365 225d  _candle["Close"]
+00024050: 2e69 6c6f 635b 305d 203c 3d20 7265 6365  .iloc[0] <= rece
+00024060: 6e74 5b22 436c 6f73 6522 5d2e 696c 6f63  nt["Close"].iloc
+00024070: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
+00024080: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
+00024090: 2020 2020 2020 2020 2020 2073 6372 6565             scree
+000240a0: 6e44 6963 745b 2250 6174 7465 726e 225d  nDict["Pattern"]
+000240b0: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
+000240c0: 2020 2020 2020 2020 2020 2020 2073 6176               sav
+000240d0: 6564 5b30 5d20 2b20 636f 6c6f 7254 6578  ed[0] + colorTex
+000240e0: 742e 424f 4c44 202b 2063 6f6c 6f72 5465  t.BOLD + colorTe
+000240f0: 7874 2e46 4149 4c20 2b20 6622 5365 6c6c  xt.FAIL + f"Sell
+00024100: 2d4e 527b 6e72 7d22 202b 2063 6f6c 6f72  -NR{nr}" + color
+00024110: 5465 7874 2e45 4e44 0a20 2020 2020 2020  Text.END.       
+00024120: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+00024130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024140: 2020 2073 6176 6544 6963 745b 2250 6174     saveDict["Pat
+00024150: 7465 726e 225d 203d 2073 6176 6564 5b31  tern"] = saved[1
+00024160: 5d20 2b20 6622 5365 6c6c 2d4e 527b 6e72  ] + f"Sell-NR{nr
+00024170: 7d22 0a20 2020 2020 2020 2020 2020 2020  }".             
+00024180: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
+00024190: 7565 0a20 2020 2020 2020 2020 2020 2072  ue.            r
+000241a0: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
+000241b0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+000241c0: 2020 2020 2020 7261 6e67 6544 6174 6120        rangeData 
+000241d0: 3d20 6461 7461 2e68 6561 6428 6e72 290a  = data.head(nr).
+000241e0: 2020 2020 2020 2020 2020 2020 7261 6e67              rang
+000241f0: 6544 6174 612e 6c6f 635b 3a2c 2752 616e  eData.loc[:,'Ran
+00024200: 6765 275d 203d 2061 6273 2872 616e 6765  ge'] = abs(range
+00024210: 4461 7461 5b22 436c 6f73 6522 5d20 2d20  Data["Close"] - 
+00024220: 7261 6e67 6544 6174 615b 224f 7065 6e22  rangeData["Open"
+00024230: 5d29 0a20 2020 2020 2020 2020 2020 2072  ]).            r
+00024240: 6563 656e 7420 3d20 7261 6e67 6544 6174  ecent = rangeDat
+00024250: 612e 6865 6164 2831 290a 2020 2020 2020  a.head(1).      
+00024260: 2020 2020 2020 6966 2072 6563 656e 745b        if recent[
+00024270: 2252 616e 6765 225d 2e69 6c6f 635b 305d  "Range"].iloc[0]
+00024280: 203d 3d20 7261 6e67 6544 6174 612e 6465   == rangeData.de
+00024290: 7363 7269 6265 2829 5b22 5261 6e67 6522  scribe()["Range"
+000242a0: 5d5b 226d 696e 225d 3a0a 2020 2020 2020  ]["min"]:.      
+000242b0: 2020 2020 2020 2020 2020 7363 7265 656e            screen
+000242c0: 4469 6374 5b22 5061 7474 6572 6e22 5d20  Dict["Pattern"] 
+000242d0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+000242e0: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
+000242f0: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
+00024300: 4420 2b20 636f 6c6f 7254 6578 742e 4752  D + colorText.GR
+00024310: 4545 4e20 2b20 6622 4e52 7b6e 727d 2220  EEN + f"NR{nr}" 
+00024320: 2b20 636f 6c6f 7254 6578 742e 454e 440a  + colorText.END.
+00024330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024340: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00024350: 2020 7361 7665 4469 6374 5b22 5061 7474    saveDict["Patt
+00024360: 6572 6e22 5d20 3d20 7361 7665 645b 315d  ern"] = saved[1]
+00024370: 202b 2066 224e 527b 6e72 7d22 0a20 2020   + f"NR{nr}".   
+00024380: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00024390: 7572 6e20 5472 7565 0a20 2020 2020 2020  urn True.       
+000243a0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+000243b0: 650a 0a20 2020 2023 2046 696e 6420 6966  e..    # Find if
+000243c0: 2073 746f 636b 2069 7320 6e65 776c 7920   stock is newly 
+000243d0: 6c69 7374 6564 0a20 2020 2064 6566 2076  listed.    def v
+000243e0: 616c 6964 6174 654e 6577 6c79 4c69 7374  alidateNewlyList
+000243f0: 6564 2873 656c 662c 2064 662c 2064 6179  ed(self, df, day
+00024400: 7354 6f4c 6f6f 6b62 6163 6b29 3a0a 2020  sToLookback):.  
+00024410: 2020 2020 2020 6966 2064 6620 6973 204e        if df is N
+00024420: 6f6e 6520 6f72 206c 656e 2864 6629 203d  one or len(df) =
+00024430: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
+00024440: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
+00024450: 2020 2020 2020 6461 7461 203d 2064 662e        data = df.
+00024460: 636f 7079 2829 0a20 2020 2020 2020 2064  copy().        d
+00024470: 6179 7354 6f4c 6f6f 6b62 6163 6b20 3d20  aysToLookback = 
+00024480: 696e 7428 6461 7973 546f 4c6f 6f6b 6261  int(daysToLookba
+00024490: 636b 5b3a 2d31 5d29 0a20 2020 2020 2020  ck[:-1]).       
+000244a0: 2072 6563 656e 7420 3d20 6461 7461 2e68   recent = data.h
+000244b0: 6561 6428 3129 0a20 2020 2020 2020 2069  ead(1).        i
+000244c0: 6620 6c65 6e28 7265 6365 6e74 2920 3c20  f len(recent) < 
+000244d0: 313a 0a20 2020 2020 2020 2020 2020 2072  1:.            r
+000244e0: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
+000244f0: 2020 2020 6966 206c 656e 2864 6174 6129      if len(data)
+00024500: 203c 2064 6179 7354 6f4c 6f6f 6b62 6163   < daysToLookbac
+00024510: 6b20 616e 6420 280a 2020 2020 2020 2020  k and (.        
+00024520: 2020 2020 7265 6365 6e74 5b22 436c 6f73      recent["Clos
+00024530: 6522 5d2e 696c 6f63 5b30 5d20 213d 206e  e"].iloc[0] != n
+00024540: 702e 6e61 6e20 616e 6420 7265 6365 6e74  p.nan and recent
+00024550: 5b22 436c 6f73 6522 5d2e 696c 6f63 5b30  ["Close"].iloc[0
+00024560: 5d20 3e20 300a 2020 2020 2020 2020 293a  ] > 0.        ):
+00024570: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00024580: 7572 6e20 5472 7565 0a20 2020 2020 2020  urn True.       
+00024590: 2072 6574 7572 6e20 4661 6c73 650a 0a20   return False.. 
+000245a0: 2020 2023 2056 616c 6964 6174 6520 6966     # Validate if
+000245b0: 2074 6865 2073 746f 636b 2070 7269 6365   the stock price
+000245c0: 7320 6172 6520 6174 206c 6561 7374 2072  s are at least r
+000245d0: 6973 696e 6720 6279 2032 2520 666f 7220  ising by 2% for 
+000245e0: 7468 6520 6c61 7374 2033 2073 6573 7369  the last 3 sessi
+000245f0: 6f6e 730a 2020 2020 6465 6620 7661 6c69  ons.    def vali
+00024600: 6461 7465 5072 6963 6552 6973 696e 6742  datePriceRisingB
+00024610: 7941 744c 6561 7374 3250 6572 6365 6e74  yAtLeast2Percent
+00024620: 2873 656c 662c 2064 662c 2073 6372 6565  (self, df, scree
+00024630: 6e44 6963 742c 2073 6176 6544 6963 7429  nDict, saveDict)
+00024640: 3a0a 2020 2020 2020 2020 6966 2064 6620  :.        if df 
+00024650: 6973 204e 6f6e 6520 6f72 206c 656e 2864  is None or len(d
+00024660: 6629 203d 3d20 303a 0a20 2020 2020 2020  f) == 0:.       
+00024670: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00024680: 650a 2020 2020 2020 2020 6461 7461 203d  e.        data =
+00024690: 2064 662e 636f 7079 2829 0a20 2020 2020   df.copy().     
+000246a0: 2020 2064 6174 6120 3d20 6461 7461 2e66     data = data.f
+000246b0: 696c 6c6e 6128 3029 0a20 2020 2020 2020  illna(0).       
+000246c0: 2064 6174 6120 3d20 6461 7461 2e72 6570   data = data.rep
+000246d0: 6c61 6365 285b 6e70 2e69 6e66 2c20 2d6e  lace([np.inf, -n
+000246e0: 702e 696e 665d 2c20 3029 0a20 2020 2020  p.inf], 0).     
+000246f0: 2020 2064 6174 6120 3d20 6461 7461 2e68     data = data.h
+00024700: 6561 6428 3429 0a20 2020 2020 2020 2069  ead(4).        i
+00024710: 6620 6c65 6e28 6461 7461 2920 3c20 343a  f len(data) < 4:
+00024720: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00024730: 7572 6e20 4661 6c73 650a 2020 2020 2020  urn False.      
+00024740: 2020 6461 7930 203d 2064 6174 612e 696c    day0 = data.il
+00024750: 6f63 5b30 5d5b 2243 6c6f 7365 225d 2e69  oc[0]["Close"].i
+00024760: 7465 6d28 290a 2020 2020 2020 2020 6461  tem().        da
+00024770: 794d 696e 7573 3120 3d20 6461 7461 2e69  yMinus1 = data.i
+00024780: 6c6f 635b 315d 5b22 436c 6f73 6522 5d2e  loc[1]["Close"].
+00024790: 6974 656d 2829 0a20 2020 2020 2020 2064  item().        d
+000247a0: 6179 4d69 6e75 7332 203d 2064 6174 612e  ayMinus2 = data.
+000247b0: 696c 6f63 5b32 5d5b 2243 6c6f 7365 225d  iloc[2]["Close"]
+000247c0: 2e69 7465 6d28 290a 2020 2020 2020 2020  .item().        
+000247d0: 6461 794d 696e 7573 3320 3d20 6461 7461  dayMinus3 = data
+000247e0: 2e69 6c6f 635b 335d 5b22 436c 6f73 6522  .iloc[3]["Close"
+000247f0: 5d2e 6974 656d 2829 0a20 2020 2020 2020  ].item().       
+00024800: 2070 6572 6365 6e74 3320 3d20 726f 756e   percent3 = roun
+00024810: 6428 2864 6179 4d69 6e75 7332 202d 2064  d((dayMinus2 - d
+00024820: 6179 4d69 6e75 7333 2920 2a20 3130 3020  ayMinus3) * 100 
+00024830: 2f20 6461 794d 696e 7573 332c 2032 290a  / dayMinus3, 2).
+00024840: 2020 2020 2020 2020 7065 7263 656e 7432          percent2
+00024850: 203d 2072 6f75 6e64 2828 6461 794d 696e   = round((dayMin
+00024860: 7573 3120 2d20 6461 794d 696e 7573 3229  us1 - dayMinus2)
+00024870: 202a 2031 3030 202f 2064 6179 4d69 6e75   * 100 / dayMinu
+00024880: 7332 2c20 3229 0a20 2020 2020 2020 2070  s2, 2).        p
+00024890: 6572 6365 6e74 3120 3d20 726f 756e 6428  ercent1 = round(
+000248a0: 2864 6179 3020 2d20 6461 794d 696e 7573  (day0 - dayMinus
+000248b0: 3129 202a 2031 3030 202f 2064 6179 4d69  1) * 100 / dayMi
+000248c0: 6e75 7331 2c20 3229 0a0a 2020 2020 2020  nus1, 2)..      
+000248d0: 2020 6966 2070 6572 6365 6e74 3120 3e3d    if percent1 >=
+000248e0: 2032 2061 6e64 2070 6572 6365 6e74 3220   2 and percent2 
+000248f0: 3e3d 2032 2061 6e64 2070 6572 6365 6e74  >= 2 and percent
+00024900: 3320 3e3d 2032 3a0a 2020 2020 2020 2020  3 >= 2:.        
+00024910: 2020 2020 7063 745f 6368 616e 6765 5f74      pct_change_t
+00024920: 6578 7420 3d20 280a 2020 2020 2020 2020  ext = (.        
+00024930: 2020 2020 2020 2020 2822 252e 3166 2525          ("%.1f%%
+00024940: 2220 2520 7065 7263 656e 7431 290a 2020  " % percent1).  
+00024950: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+00024960: 2822 2028 252e 3166 2525 2c22 2025 2070  (" (%.1f%%," % p
+00024970: 6572 6365 6e74 3229 0a20 2020 2020 2020  ercent2).       
+00024980: 2020 2020 2020 2020 202b 2028 2220 252e           + (" %.
+00024990: 3166 2525 2922 2025 2070 6572 6365 6e74  1f%%)" % percent
+000249a0: 3329 0a20 2020 2020 2020 2020 2020 2029  3).            )
+000249b0: 0a20 2020 2020 2020 2020 2020 2073 6176  .            sav
+000249c0: 6544 6963 745b 2225 4368 6e67 225d 203d  eDict["%Chng"] =
+000249d0: 2070 6374 5f63 6861 6e67 655f 7465 7874   pct_change_text
+000249e0: 0a20 2020 2020 2020 2020 2020 2073 6372  .            scr
+000249f0: 6565 6e44 6963 745b 2225 4368 6e67 225d  eenDict["%Chng"]
+00024a00: 203d 2063 6f6c 6f72 5465 7874 2e47 5245   = colorText.GRE
+00024a10: 454e 202b 2070 6374 5f63 6861 6e67 655f  EN + pct_change_
+00024a20: 7465 7874 202b 2063 6f6c 6f72 5465 7874  text + colorText
+00024a30: 2e45 4e44 0a20 2020 2020 2020 2020 2020  .END.           
+00024a40: 2072 6574 7572 6e20 5472 7565 2061 6e64   return True and
+00024a50: 2073 656c 662e 6765 7443 616e 646c 6554   self.getCandleT
+00024a60: 7970 6528 6461 7461 2e68 6561 6428 3129  ype(data.head(1)
+00024a70: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00024a80: 2046 616c 7365 0a0a 2020 2020 2340 6d65   False..    #@me
+00024a90: 6173 7572 655f 7469 6d65 0a20 2020 2023  asure_time.    #
+00024aa0: 2076 616c 6964 6174 6520 6966 2052 5349   validate if RSI
+00024ab0: 2069 7320 7769 7468 696e 2067 6976 656e   is within given
+00024ac0: 2072 616e 6765 0a20 2020 2064 6566 2076   range.    def v
+00024ad0: 616c 6964 6174 6552 5349 2873 656c 662c  alidateRSI(self,
+00024ae0: 2064 662c 2073 6372 6565 6e44 6963 742c   df, screenDict,
+00024af0: 2073 6176 6544 6963 742c 206d 696e 5253   saveDict, minRS
+00024b00: 492c 206d 6178 5253 492c 7273 694b 6579  I, maxRSI,rsiKey
+00024b10: 3d22 5253 4922 293a 0a20 2020 2020 2020  ="RSI"):.       
+00024b20: 2069 6620 6466 2069 7320 4e6f 6e65 206f   if df is None o
+00024b30: 7220 6c65 6e28 6466 2920 3d3d 2030 3a0a  r len(df) == 0:.
+00024b40: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00024b50: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
+00024b60: 2069 6620 7273 694b 6579 206e 6f74 2069   if rsiKey not i
+00024b70: 6e20 6466 2e63 6f6c 756d 6e73 3a0a 2020  n df.columns:.  
+00024b80: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00024b90: 2046 616c 7365 0a20 2020 2020 2020 2064   False.        d
+00024ba0: 6174 6120 3d20 6466 2e63 6f70 7928 290a  ata = df.copy().
+00024bb0: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
+00024bc0: 6174 612e 6669 6c6c 6e61 2830 290a 2020  ata.fillna(0).  
+00024bd0: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
+00024be0: 612e 7265 706c 6163 6528 5b6e 702e 696e  a.replace([np.in
+00024bf0: 662c 202d 6e70 2e69 6e66 5d2c 2030 290a  f, -np.inf], 0).
+00024c00: 2020 2020 2020 2020 7273 6920 3d20 696e          rsi = in
+00024c10: 7428 6461 7461 2e68 6561 6428 3129 5b72  t(data.head(1)[r
+00024c20: 7369 4b65 795d 2e69 6c6f 635b 305d 290a  siKey].iloc[0]).
+00024c30: 2020 2020 2020 2020 7361 7665 4469 6374          saveDict
+00024c40: 5b72 7369 4b65 795d 203d 2072 7369 0a20  [rsiKey] = rsi. 
+00024c50: 2020 2020 2020 2023 2068 7474 7073 3a2f         # https:/
+00024c60: 2f63 6861 7274 696e 6b2e 636f 6d2f 7363  /chartink.com/sc
+00024c70: 7265 656e 6572 2f72 7369 2d73 6372 6565  reener/rsi-scree
+00024c80: 6e69 6e67 0a20 2020 2020 2020 2069 6620  ning.        if 
+00024c90: 7273 693e 2030 2061 6e64 2072 7369 203e  rsi> 0 and rsi >
+00024ca0: 3d20 6d69 6e52 5349 2061 6e64 2072 7369  = minRSI and rsi
+00024cb0: 203c 3d20 6d61 7852 5349 3a20 2023 206f   <= maxRSI:  # o
+00024cc0: 7220 2872 7369 203c 3d20 3731 2061 6e64  r (rsi <= 71 and
+00024cd0: 2072 7369 203e 3d20 3637 293a 0a20 2020   rsi >= 67):.   
+00024ce0: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
+00024cf0: 6963 745b 7273 694b 6579 5d20 3d20 280a  ict[rsiKey] = (.
+00024d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024d10: 636f 6c6f 7254 6578 742e 424f 4c44 202b  colorText.BOLD +
+00024d20: 2063 6f6c 6f72 5465 7874 2e47 5245 454e   colorText.GREEN
+00024d30: 202b 2073 7472 2872 7369 2920 2b20 636f   + str(rsi) + co
+00024d40: 6c6f 7254 6578 742e 454e 440a 2020 2020  lorText.END.    
+00024d50: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00024d60: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
+00024d70: 6520 6966 2028 7273 694b 6579 203d 3d20  e if (rsiKey == 
+00024d80: 2252 5349 6922 2920 656c 7365 2028 7365  "RSIi") else (se
+00024d90: 6c66 2e76 616c 6964 6174 6552 5349 2864  lf.validateRSI(d
+00024da0: 662c 2073 6372 6565 6e44 6963 742c 2073  f, screenDict, s
+00024db0: 6176 6544 6963 742c 206d 696e 5253 492c  aveDict, minRSI,
+00024dc0: 206d 6178 5253 492c 7273 694b 6579 3d22   maxRSI,rsiKey="
+00024dd0: 5253 4969 2229 206f 7220 5472 7565 290a  RSIi") or True).
+00024de0: 2020 2020 2020 2020 7363 7265 656e 4469          screenDi
+00024df0: 6374 5b72 7369 4b65 795d 203d 2063 6f6c  ct[rsiKey] = col
+00024e00: 6f72 5465 7874 2e42 4f4c 4420 2b20 636f  orText.BOLD + co
+00024e10: 6c6f 7254 6578 742e 4641 494c 202b 2073  lorText.FAIL + s
+00024e20: 7472 2872 7369 2920 2b20 636f 6c6f 7254  tr(rsi) + colorT
+00024e30: 6578 742e 454e 440a 2020 2020 2020 2020  ext.END.        
+00024e40: 2320 4966 2065 6974 6865 7220 6461 696c  # If either dail
+00024e50: 7920 6f72 2069 6e74 7261 6461 7920 5253  y or intraday RS
+00024e60: 4920 636f 6d65 7320 7769 7468 696e 2072  I comes within r
+00024e70: 616e 6765 3f0a 2020 2020 2020 2020 7265  ange?.        re
+00024e80: 7475 726e 2046 616c 7365 2069 6620 2872  turn False if (r
+00024e90: 7369 4b65 7920 3d3d 2022 5253 4969 2229  siKey == "RSIi")
+00024ea0: 2065 6c73 6520 2873 656c 662e 7661 6c69   else (self.vali
+00024eb0: 6461 7465 5253 4928 6466 2c20 7363 7265  dateRSI(df, scre
+00024ec0: 656e 4469 6374 2c20 7361 7665 4469 6374  enDict, saveDict
+00024ed0: 2c20 6d69 6e52 5349 2c20 6d61 7852 5349  , minRSI, maxRSI
+00024ee0: 2c72 7369 4b65 793d 2252 5349 6922 2929  ,rsiKey="RSIi"))
+00024ef0: 0a0a 2020 2020 2320 5661 6c69 6461 7465  ..    # Validate
+00024f00: 2069 6620 7468 6520 7374 6f63 6b20 6973   if the stock is
+00024f10: 2062 756c 6c69 7368 2069 6e20 7468 6520   bullish in the 
+00024f20: 7368 6f72 7420 7465 726d 0a20 2020 2064  short term.    d
+00024f30: 6566 2076 616c 6964 6174 6553 686f 7274  ef validateShort
+00024f40: 5465 726d 4275 6c6c 6973 6828 7365 6c66  TermBullish(self
+00024f50: 2c20 6466 2c20 7363 7265 656e 4469 6374  , df, screenDict
+00024f60: 2c20 7361 7665 4469 6374 293a 0a20 2020  , saveDict):.   
+00024f70: 2020 2020 2069 6620 6466 2069 7320 4e6f       if df is No
+00024f80: 6e65 206f 7220 6c65 6e28 6466 2920 3d3d  ne or len(df) ==
+00024f90: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+00024fa0: 7265 7475 726e 2046 616c 7365 0a20 2020  return False.   
+00024fb0: 2020 2020 2064 6174 6120 3d20 6466 2e63       data = df.c
+00024fc0: 6f70 7928 290a 2020 2020 2020 2020 2320  opy().        # 
+00024fd0: 6874 7470 733a 2f2f 6368 6172 7469 6e6b  https://chartink
+00024fe0: 2e63 6f6d 2f73 6372 6565 6e65 722f 7368  .com/screener/sh
+00024ff0: 6f72 742d 7465 726d 2d62 756c 6c69 7368  ort-term-bullish
+00025000: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
+00025010: 6461 7461 2e66 696c 6c6e 6128 3029 0a20  data.fillna(0). 
+00025020: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
+00025030: 7461 2e72 6570 6c61 6365 285b 6e70 2e69  ta.replace([np.i
+00025040: 6e66 2c20 2d6e 702e 696e 665d 2c20 3029  nf, -np.inf], 0)
+00025050: 0a20 2020 2020 2020 2072 6563 656e 7420  .        recent 
+00025060: 3d20 6461 7461 2e68 6561 6428 3129 0a20  = data.head(1). 
+00025070: 2020 2020 2020 2066 6b20 3d20 3020 6966         fk = 0 if
+00025080: 206c 656e 2864 6174 6129 203c 2033 2065   len(data) < 3 e
+00025090: 6c73 6520 6e70 2e72 6f75 6e64 2864 6174  lse np.round(dat
+000250a0: 615b 2246 4153 544b 225d 2e69 6c6f 635b  a["FASTK"].iloc[
+000250b0: 325d 2c20 3529 0a20 2020 2020 2020 2023  2], 5).        #
+000250c0: 2052 6576 6572 7365 2074 6865 2064 6174   Reverse the dat
+000250d0: 6166 7261 6d65 2066 6f72 2069 6368 696d  aframe for ichim
+000250e0: 6f6b 7520 6361 6c63 756c 6174 696f 6e73  oku calculations
+000250f0: 2077 6974 6820 6461 7465 2069 6e20 6173   with date in as
+00025100: 6365 6e64 696e 6720 6f72 6465 720a 2020  cending order.  
+00025110: 2020 2020 2020 6466 5f6e 6577 203d 2064        df_new = d
+00025120: 6174 615b 3a3a 2d31 5d0a 2020 2020 2020  ata[::-1].      
+00025130: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+00025140: 2020 2064 665f 6963 6869 203d 2064 665f     df_ichi = df_
+00025150: 6e65 772e 7265 6e61 6d65 280a 2020 2020  new.rename(.    
+00025160: 2020 2020 2020 2020 2020 2020 636f 6c75              colu
+00025170: 6d6e 733d 7b0a 2020 2020 2020 2020 2020  mns={.          
+00025180: 2020 2020 2020 2020 2020 224f 7065 6e22            "Open"
+00025190: 3a20 226f 7065 6e22 2c0a 2020 2020 2020  : "open",.      
+000251a0: 2020 2020 2020 2020 2020 2020 2020 2248                "H
+000251b0: 6967 6822 3a20 2268 6967 6822 2c0a 2020  igh": "high",.  
+000251c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000251d0: 2020 224c 6f77 223a 2022 6c6f 7722 2c0a    "Low": "low",.
+000251e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000251f0: 2020 2020 2243 6c6f 7365 223a 2022 636c      "Close": "cl
+00025200: 6f73 6522 2c0a 2020 2020 2020 2020 2020  ose",.          
+00025210: 2020 2020 2020 2020 2020 2256 6f6c 756d            "Volum
+00025220: 6522 3a20 2276 6f6c 756d 6522 2c0a 2020  e": "volume",.  
+00025230: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
+00025240: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00025250: 2020 2020 2020 2020 2020 6963 6869 203d            ichi =
+00025260: 2070 6b74 616c 6962 2e69 6368 696d 6f6b   pktalib.ichimok
+00025270: 7528 6466 5f69 6368 692c 2039 2c20 3236  u(df_ichi, 9, 26
+00025280: 2c20 3532 2c20 3236 290a 2020 2020 2020  , 52, 26).      
+00025290: 2020 2020 2020 6966 2069 6368 6920 6973        if ichi is
+000252a0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000252b0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+000252c0: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
+000252d0: 6466 5f6e 6577 203d 2070 642e 636f 6e63  df_new = pd.conc
+000252e0: 6174 285b 6466 5f6e 6577 2c20 6963 6869  at([df_new, ichi
+000252f0: 5d2c 2061 7869 733d 3129 0a20 2020 2020  ], axis=1).     
+00025300: 2020 2020 2020 2023 2052 6576 6572 7365         # Reverse
+00025310: 2061 6761 696e 2074 6f20 6765 7420 7468   again to get th
+00025320: 6520 6d6f 7374 2072 6563 656e 7420 6461  e most recent da
+00025330: 7465 206f 6e20 746f 700a 2020 2020 2020  te on top.      
+00025340: 2020 2020 2020 6466 5f6e 6577 203d 2064        df_new = d
+00025350: 665f 6e65 775b 3a3a 2d31 5d0a 2020 2020  f_new[::-1].    
+00025360: 2020 2020 2020 2020 6466 5f6e 6577 203d          df_new =
+00025370: 2064 665f 6e65 772e 6865 6164 2831 290a   df_new.head(1).
+00025380: 2020 2020 2020 2020 2020 2020 6466 5f6e              df_n
+00025390: 6577 5b22 636c 6f75 645f 6772 6565 6e22  ew["cloud_green"
+000253a0: 5d20 3d20 6466 5f6e 6577 5b22 4953 415f  ] = df_new["ISA_
+000253b0: 3922 5d2e 696c 6f63 5b30 5d20 3e20 6466  9"].iloc[0] > df
+000253c0: 5f6e 6577 5b22 4953 425f 3236 225d 2e69  _new["ISB_26"].i
+000253d0: 6c6f 635b 305d 0a20 2020 2020 2020 2020  loc[0].         
+000253e0: 2020 2064 665f 6e65 775b 2263 6c6f 7564     df_new["cloud
+000253f0: 5f72 6564 225d 203d 2064 665f 6e65 775b  _red"] = df_new[
+00025400: 2249 5342 5f32 3622 5d2e 696c 6f63 5b30  "ISB_26"].iloc[0
+00025410: 5d20 3e20 6466 5f6e 6577 5b22 4953 415f  ] > df_new["ISA_
+00025420: 3922 5d2e 696c 6f63 5b30 5d0a 2020 2020  9"].iloc[0].    
+00025430: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
+00025440: 7469 6f6e 2061 7320 653a 2020 2320 7072  tion as e:  # pr
+00025450: 6167 6d61 3a20 6e6f 2063 6f76 6572 0a20  agma: no cover. 
+00025460: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00025470: 6465 6661 756c 745f 6c6f 6767 6572 2e64  default_logger.d
+00025480: 6562 7567 2865 2c20 6578 635f 696e 666f  ebug(e, exc_info
+00025490: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
+000254a0: 2020 2070 6173 730a 2020 2020 2020 2020     pass.        
+000254b0: 6162 6f76 6543 6c6f 7564 546f 7020 3d20  aboveCloudTop = 
+000254c0: 4661 6c73 650a 2020 2020 2020 2020 2320  False.        # 
+000254d0: 6261 7365 6c69 6e65 203e 2063 6c6f 7564  baseline > cloud
+000254e0: 2074 6f70 2028 636c 6f75 6420 6973 2062   top (cloud is b
+000254f0: 6f75 6e64 2062 7920 7370 616e 2061 2061  ound by span a a
+00025500: 6e64 2073 7061 6e20 6229 2061 6e64 2063  nd span b) and c
+00025510: 6c6f 7365 2069 7320 3e20 636c 6f75 6420  lose is > cloud 
+00025520: 746f 700a 2020 2020 2020 2020 6966 2064  top.        if d
+00025530: 665f 6e65 775b 2263 6c6f 7564 5f67 7265  f_new["cloud_gre
+00025540: 656e 225d 2e69 6c6f 635b 305d 3a0a 2020  en"].iloc[0]:.  
+00025550: 2020 2020 2020 2020 2020 6162 6f76 6543            aboveC
+00025560: 6c6f 7564 546f 7020 3d20 280a 2020 2020  loudTop = (.    
+00025570: 2020 2020 2020 2020 2020 2020 6466 5f6e              df_n
+00025580: 6577 5b22 494b 535f 3236 225d 2e69 6c6f  ew["IKS_26"].ilo
+00025590: 635b 305d 203e 2064 665f 6e65 775b 2249  c[0] > df_new["I
+000255a0: 5341 5f39 225d 2e69 6c6f 635b 305d 0a20  SA_9"].iloc[0]. 
+000255b0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+000255c0: 6e64 2072 6563 656e 745b 2243 6c6f 7365  nd recent["Close
+000255d0: 225d 2e69 6c6f 635b 305d 203e 2064 665f  "].iloc[0] > df_
+000255e0: 6e65 775b 2249 5341 5f39 225d 2e69 6c6f  new["ISA_9"].ilo
+000255f0: 635b 305d 0a20 2020 2020 2020 2020 2020  c[0].           
+00025600: 2029 0a20 2020 2020 2020 2065 6c69 6620   ).        elif 
+00025610: 6466 5f6e 6577 5b22 636c 6f75 645f 7265  df_new["cloud_re
+00025620: 6422 5d2e 696c 6f63 5b30 5d3a 0a20 2020  d"].iloc[0]:.   
+00025630: 2020 2020 2020 2020 2061 626f 7665 436c           aboveCl
+00025640: 6f75 6454 6f70 203d 2028 0a20 2020 2020  oudTop = (.     
+00025650: 2020 2020 2020 2020 2020 2064 665f 6e65             df_ne
+00025660: 775b 2249 4b53 5f32 3622 5d2e 696c 6f63  w["IKS_26"].iloc
+00025670: 5b30 5d20 3e20 6466 5f6e 6577 5b22 4953  [0] > df_new["IS
+00025680: 425f 3236 225d 2e69 6c6f 635b 305d 0a20  B_26"].iloc[0]. 
+00025690: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+000256a0: 6e64 2072 6563 656e 745b 2243 6c6f 7365  nd recent["Close
+000256b0: 225d 2e69 6c6f 635b 305d 203e 2064 665f  "].iloc[0] > df_
+000256c0: 6e65 775b 2249 5342 5f32 3622 5d2e 696c  new["ISB_26"].il
+000256d0: 6f63 5b30 5d0a 2020 2020 2020 2020 2020  oc[0].          
+000256e0: 2020 290a 0a20 2020 2020 2020 2023 204c    )..        # L
+000256f0: 6174 6573 7420 4963 6869 6d6f 6b75 2062  atest Ichimoku b
+00025700: 6173 656c 696e 6520 6973 203c 206c 6174  aseline is < lat
+00025710: 6573 7420 4963 6869 6d6f 6b75 2063 6f6e  est Ichimoku con
+00025720: 7665 7273 696f 6e20 6c69 6e65 0a20 2020  version line.   
+00025730: 2020 2020 2069 6620 6162 6f76 6543 6c6f       if aboveClo
+00025740: 7564 546f 7020 616e 6420 6466 5f6e 6577  udTop and df_new
+00025750: 5b22 494b 535f 3236 225d 2e69 6c6f 635b  ["IKS_26"].iloc[
+00025760: 305d 203c 2064 665f 6e65 775b 2249 5453  0] < df_new["ITS
+00025770: 5f39 225d 2e69 6c6f 635b 305d 3a0a 2020  _9"].iloc[0]:.  
+00025780: 2020 2020 2020 2020 2020 2320 5374 6f63            # Stoc
+00025790: 6852 5349 2063 726f 7373 6564 2032 3020  hRSI crossed 20 
+000257a0: 616e 6420 5253 4920 3e20 3530 0a20 2020  and RSI > 50.   
+000257b0: 2020 2020 2020 2020 2069 6620 666b 203e           if fk >
+000257c0: 2032 3020 616e 6420 7265 6365 6e74 5b22   20 and recent["
+000257d0: 5253 4922 5d2e 696c 6f63 5b30 5d20 3e20  RSI"].iloc[0] > 
+000257e0: 3530 3a0a 2020 2020 2020 2020 2020 2020  50:.            
+000257f0: 2020 2020 2320 636f 6e64 6974 696f 6e20      # condition 
+00025800: 6f66 2063 726f 7373 696e 6720 7468 6520  of crossing the 
+00025810: 5374 6f63 6852 5349 206d 6169 6e20 7369  StochRSI main si
+00025820: 676e 616c 206c 696e 6520 6672 6f6d 2062  gnal line from b
+00025830: 6f74 746f 6d20 746f 2074 6f70 0a20 2020  ottom to top.   
+00025840: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00025850: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00025860: 2020 2020 2020 6461 7461 5b22 4641 5354        data["FAST
+00025870: 4422 5d2e 696c 6f63 5b31 3030 5d20 3c20  D"].iloc[100] < 
+00025880: 6461 7461 5b22 4641 5354 4b22 5d2e 696c  data["FASTK"].il
+00025890: 6f63 5b31 3030 5d0a 2020 2020 2020 2020  oc[100].        
+000258a0: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+000258b0: 6461 7461 5b22 4641 5354 4422 5d2e 696c  data["FASTD"].il
+000258c0: 6f63 5b31 3031 5d20 3e20 6461 7461 5b22  oc[101] > data["
+000258d0: 4641 5354 4b22 5d2e 696c 6f63 5b31 3031  FASTK"].iloc[101
+000258e0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+000258f0: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
+00025900: 2020 2020 2020 2020 2023 2063 6c6f 7365           # close
+00025910: 203e 2035 3020 7065 7269 6f64 2053 4d41   > 50 period SMA
+00025920: 2f45 4d41 2061 6e64 2032 3030 2070 6572  /EMA and 200 per
+00025930: 696f 6420 534d 412f 454d 410a 2020 2020  iod SMA/EMA.    
+00025940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025950: 6966 2028 0a20 2020 2020 2020 2020 2020  if (.           
+00025960: 2020 2020 2020 2020 2020 2020 2072 6563               rec
+00025970: 656e 745b 2253 534d 4122 5d2e 696c 6f63  ent["SSMA"].iloc
+00025980: 5b30 5d20 3e20 7265 6365 6e74 5b22 534d  [0] > recent["SM
+00025990: 4122 5d2e 696c 6f63 5b30 5d0a 2020 2020  A"].iloc[0].    
+000259a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000259b0: 2020 2020 616e 6420 7265 6365 6e74 5b22      and recent["
+000259c0: 436c 6f73 6522 5d2e 696c 6f63 5b30 5d20  Close"].iloc[0] 
+000259d0: 3e20 7265 6365 6e74 5b22 5353 4d41 225d  > recent["SSMA"]
+000259e0: 2e69 6c6f 635b 305d 0a20 2020 2020 2020  .iloc[0].       
+000259f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025a00: 2061 6e64 2072 6563 656e 745b 2243 6c6f   and recent["Clo
+00025a10: 7365 225d 2e69 6c6f 635b 305d 203e 2072  se"].iloc[0] > r
+00025a20: 6563 656e 745b 224c 4d41 225d 2e69 6c6f  ecent["LMA"].ilo
+00025a30: 635b 305d 0a20 2020 2020 2020 2020 2020  c[0].           
+00025a40: 2020 2020 2020 2020 2029 3a0a 2020 2020           ):.    
+00025a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025a60: 2020 2020 7361 7665 6420 3d20 7365 6c66      saved = self
+00025a70: 2e66 696e 6443 7572 7265 6e74 5361 7665  .findCurrentSave
+00025a80: 6456 616c 7565 2873 6372 6565 6e44 6963  dValue(screenDic
+00025a90: 742c 7361 7665 4469 6374 2c22 4d41 2d53  t,saveDict,"MA-S
+00025aa0: 6967 6e61 6c22 290a 2020 2020 2020 2020  ignal").        
+00025ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025ac0: 7363 7265 656e 4469 6374 5b22 4d41 2d53  screenDict["MA-S
+00025ad0: 6967 6e61 6c22 5d20 3d20 280a 2020 2020  ignal"] = (.    
+00025ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025af0: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
+00025b00: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
+00025b10: 4420 2b20 636f 6c6f 7254 6578 742e 4752  D + colorText.GR
+00025b20: 4545 4e20 2b20 2242 756c 6c69 7368 2220  EEN + "Bullish" 
+00025b30: 2b20 636f 6c6f 7254 6578 742e 454e 440a  + colorText.END.
+00025b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025b50: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00025b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025b70: 2020 7361 7665 4469 6374 5b22 4d41 2d53    saveDict["MA-S
+00025b80: 6967 6e61 6c22 5d20 3d20 7361 7665 645b  ignal"] = saved[
+00025b90: 315d 202b 2022 4275 6c6c 6973 6822 0a20  1] + "Bullish". 
+00025ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025bb0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
+00025bc0: 7565 0a20 2020 2020 2020 2072 6574 7572  ue.        retur
+00025bd0: 6e20 4661 6c73 650a 2020 2020 0a20 2020  n False.    .   
+00025be0: 2023 2056 616c 6964 6174 6520 5643 5020   # Validate VCP 
+00025bf0: 6173 2070 6572 204d 6172 6b20 4d69 6e65  as per Mark Mine
+00025c00: 7276 696e 690a 2020 2020 2320 6874 7470  rvini.    # http
+00025c10: 733a 2f2f 6368 6172 7469 6e6b 2e63 6f6d  s://chartink.com
+00025c20: 2f73 6372 6565 6e65 722f 766f 6c61 7469  /screener/volati
+00025c30: 6c69 7479 2d63 6f6d 7072 6573 7369 6f6e  lity-compression
+00025c40: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+00025c50: 6556 4350 4d61 726b 4d69 6e65 7276 696e  eVCPMarkMinervin
+00025c60: 6928 7365 6c66 2c20 6466 3a70 642e 4461  i(self, df:pd.Da
+00025c70: 7461 4672 616d 652c 2073 6372 6565 6e44  taFrame, screenD
+00025c80: 6963 742c 2073 6176 6544 6963 7429 3a0a  ict, saveDict):.
+00025c90: 2020 2020 2020 2020 6966 2064 6620 6973          if df is
+00025ca0: 204e 6f6e 6520 6f72 206c 656e 2864 6629   None or len(df)
+00025cb0: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
+00025cc0: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+00025cd0: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
+00025ce0: 662e 636f 7079 2829 0a20 2020 2020 2020  f.copy().       
+00025cf0: 206f 686c 635f 6469 6374 203d 207b 0a20   ohlc_dict = {. 
+00025d00: 2020 2020 2020 2020 2020 2027 4f70 656e             'Open
+00025d10: 273a 2766 6972 7374 272c 0a20 2020 2020  ':'first',.     
+00025d20: 2020 2020 2020 2027 4869 6768 273a 276d         'High':'m
+00025d30: 6178 272c 0a20 2020 2020 2020 2020 2020  ax',.           
+00025d40: 2027 4c6f 7727 3a27 6d69 6e27 2c0a 2020   'Low':'min',.  
+00025d50: 2020 2020 2020 2020 2020 2743 6c6f 7365            'Close
+00025d60: 273a 276c 6173 7427 2c0a 2020 2020 2020  ':'last',.      
+00025d70: 2020 2020 2020 2756 6f6c 756d 6527 3a27        'Volume':'
+00025d80: 7375 6d27 0a20 2020 2020 2020 207d 0a20  sum'.        }. 
+00025d90: 2020 2020 2020 2023 2066 696e 616c 5f64         # final_d
+00025da0: 6620 3d20 6466 2e72 6573 616d 706c 6528  f = df.resample(
+00025db0: 2757 2d46 5249 272c 2063 6c6f 7365 643d  'W-FRI', closed=
+00025dc0: 276c 6566 7427 292e 6167 6728 6f68 6c63  'left').agg(ohlc
+00025dd0: 5f64 6963 7429 2e73 6869 6674 2827 3164  _dict).shift('1d
+00025de0: 2729 0a20 2020 2020 2020 2077 6565 6b6c  ').        weekl
+00025df0: 7944 6174 6120 3d20 6461 7461 2e72 6573  yData = data.res
+00025e00: 616d 706c 6528 2757 2729 2e61 6767 286f  ample('W').agg(o
+00025e10: 686c 635f 6469 6374 290a 2020 2020 2020  hlc_dict).      
+00025e20: 2020 7265 7665 7273 6564 4461 7461 203d    reversedData =
+00025e30: 2064 6174 615b 3a3a 2d31 5d20 2023 2052   data[::-1]  # R
+00025e40: 6576 6572 7365 2074 6865 2064 6174 6166  everse the dataf
+00025e50: 7261 6d65 0a20 2020 2020 2020 2072 6563  rame.        rec
+00025e60: 656e 745f 636c 6f73 6520 3d20 6461 7461  ent_close = data
+00025e70: 5b22 436c 6f73 6522 5d2e 6865 6164 2831  ["Close"].head(1
+00025e80: 292e 696c 6f63 5b30 5d0a 2020 2020 2020  ).iloc[0].      
+00025e90: 2020 775f 656d 615f 3133 203d 2070 6b74    w_ema_13 = pkt
+00025ea0: 616c 6962 2e45 4d41 2877 6565 6b6c 7944  alib.EMA(weeklyD
+00025eb0: 6174 615b 2243 6c6f 7365 225d 2c74 696d  ata["Close"],tim
+00025ec0: 6570 6572 696f 643d 3133 292e 7461 696c  eperiod=13).tail
+00025ed0: 2831 292e 696c 6f63 5b30 5d0a 2020 2020  (1).iloc[0].    
+00025ee0: 2020 2020 775f 656d 615f 3236 203d 2070      w_ema_26 = p
+00025ef0: 6b74 616c 6962 2e45 4d41 2877 6565 6b6c  ktalib.EMA(weekl
+00025f00: 7944 6174 615b 2243 6c6f 7365 225d 2c74  yData["Close"],t
+00025f10: 696d 6570 6572 696f 643d 3236 292e 7461  imeperiod=26).ta
+00025f20: 696c 2831 292e 696c 6f63 5b30 5d0a 2020  il(1).iloc[0].  
+00025f30: 2020 2020 2020 775f 736d 615f 3530 203d        w_sma_50 =
+00025f40: 2070 6b74 616c 6962 2e53 4d41 2877 6565   pktalib.SMA(wee
+00025f50: 6b6c 7944 6174 615b 2243 6c6f 7365 225d  klyData["Close"]
+00025f60: 2c74 696d 6570 6572 696f 643d 3530 292e  ,timeperiod=50).
+00025f70: 7461 696c 2831 292e 696c 6f63 5b30 5d0a  tail(1).iloc[0].
+00025f80: 2020 2020 2020 2020 775f 736d 615f 3430          w_sma_40
+00025f90: 203d 2070 6b74 616c 6962 2e53 4d41 2877   = pktalib.SMA(w
+00025fa0: 6565 6b6c 7944 6174 615b 2243 6c6f 7365  eeklyData["Close
+00025fb0: 225d 2c74 696d 6570 6572 696f 643d 3430  "],timeperiod=40
+00025fc0: 292e 7461 696c 2831 292e 696c 6f63 5b30  ).tail(1).iloc[0
+00025fd0: 5d0a 2020 2020 2020 2020 775f 736d 615f  ].        w_sma_
+00025fe0: 3430 5f35 775f 6167 6f20 3d20 706b 7461  40_5w_ago = pkta
+00025ff0: 6c69 622e 534d 4128 7765 656b 6c79 4461  lib.SMA(weeklyDa
+00026000: 7461 2e68 6561 6428 6c65 6e28 7765 656b  ta.head(len(week
+00026010: 6c79 4461 7461 292d 3529 5b22 436c 6f73  lyData)-5)["Clos
+00026020: 6522 5d2c 7469 6d65 7065 7269 6f64 3d34  e"],timeperiod=4
+00026030: 3029 2e74 6169 6c28 3129 2e69 6c6f 635b  0).tail(1).iloc[
+00026040: 305d 0a20 2020 2020 2020 2077 5f6d 696e  0].        w_min
+00026050: 5f35 3020 3d20 6d69 6e28 312e 332a 7765  _50 = min(1.3*we
+00026060: 656b 6c79 4461 7461 2e74 6169 6c28 3530  eklyData.tail(50
+00026070: 295b 224c 6f77 225d 290a 2020 2020 2020  )["Low"]).      
+00026080: 2020 775f 6d61 785f 3530 203d 206d 6178    w_max_50 = max
+00026090: 2830 2e37 352a 7765 656b 6c79 4461 7461  (0.75*weeklyData
+000260a0: 2e74 6169 6c28 3530 295b 2248 6967 6822  .tail(50)["High"
+000260b0: 5d29 0a20 2020 2020 2020 2077 5f65 6d61  ]).        w_ema
+000260c0: 5f32 365f 3230 775f 6167 6f20 3d20 706b  _26_20w_ago = pk
+000260d0: 7461 6c69 622e 454d 4128 7765 656b 6c79  talib.EMA(weekly
+000260e0: 4461 7461 2e68 6561 6428 6c65 6e28 7765  Data.head(len(we
+000260f0: 656b 6c79 4461 7461 292d 3230 295b 2243  eklyData)-20)["C
+00026100: 6c6f 7365 225d 2c74 696d 6570 6572 696f  lose"],timeperio
+00026110: 643d 3236 292e 7461 696c 2831 292e 696c  d=26).tail(1).il
+00026120: 6f63 5b30 5d0a 2020 2020 2020 2020 7265  oc[0].        re
+00026130: 6365 6e74 5f65 6d61 5f31 335f 3230 645f  cent_ema_13_20d_
+00026140: 6167 6f20 3d20 706b 7461 6c69 622e 454d  ago = pktalib.EM
+00026150: 4128 7265 7665 7273 6564 4461 7461 2e68  A(reversedData.h
+00026160: 6561 6428 6c65 6e28 7265 7665 7273 6564  ead(len(reversed
+00026170: 4461 7461 292d 3230 295b 2243 6c6f 7365  Data)-20)["Close
+00026180: 225d 2c74 696d 6570 6572 696f 643d 3133  "],timeperiod=13
+00026190: 292e 7461 696c 2831 292e 696c 6f63 5b30  ).tail(1).iloc[0
+000261a0: 5d0a 2020 2020 2020 2020 775f 736d 615f  ].        w_sma_
+000261b0: 3430 5f35 775f 6167 6f20 3d20 706b 7461  40_5w_ago = pkta
+000261c0: 6c69 622e 534d 4128 7765 656b 6c79 4461  lib.SMA(weeklyDa
+000261d0: 7461 2e68 6561 6428 6c65 6e28 7765 656b  ta.head(len(week
+000261e0: 6c79 4461 7461 292d 3529 5b22 436c 6f73  lyData)-5)["Clos
+000261f0: 6522 5d2c 7469 6d65 7065 7269 6f64 3d34  e"],timeperiod=4
+00026200: 3029 2e74 6169 6c28 3129 2e69 6c6f 635b  0).tail(1).iloc[
+00026210: 305d 0a20 2020 2020 2020 2077 5f73 6d61  0].        w_sma
+00026220: 5f34 305f 3130 775f 6167 6f20 3d20 706b  _40_10w_ago = pk
+00026230: 7461 6c69 622e 534d 4128 7765 656b 6c79  talib.SMA(weekly
+00026240: 4461 7461 2e68 6561 6428 6c65 6e28 7765  Data.head(len(we
+00026250: 656b 6c79 4461 7461 292d 3130 295b 2243  eklyData)-10)["C
+00026260: 6c6f 7365 225d 2c74 696d 6570 6572 696f  lose"],timeperio
+00026270: 643d 3430 292e 7461 696c 2831 292e 696c  d=40).tail(1).il
+00026280: 6f63 5b30 5d0a 2020 2020 2020 2020 7265  oc[0].        re
+00026290: 6365 6e74 5f73 6d61 5f35 3020 3d20 706b  cent_sma_50 = pk
+000262a0: 7461 6c69 622e 534d 4128 7265 7665 7273  talib.SMA(revers
+000262b0: 6564 4461 7461 5b22 436c 6f73 6522 5d2c  edData["Close"],
+000262c0: 7469 6d65 7065 7269 6f64 3d35 3029 2e74  timeperiod=50).t
+000262d0: 6169 6c28 3129 2e69 6c6f 635b 305d 0a20  ail(1).iloc[0]. 
+000262e0: 2020 2020 2020 2077 5f77 6d61 5f38 203d         w_wma_8 =
+000262f0: 2070 6b74 616c 6962 2e57 4d41 2877 6565   pktalib.WMA(wee
+00026300: 6b6c 7944 6174 615b 2243 6c6f 7365 225d  klyData["Close"]
+00026310: 2c74 696d 6570 6572 696f 643d 3829 2e74  ,timeperiod=8).t
+00026320: 6169 6c28 3129 2e69 6c6f 635b 305d 0a20  ail(1).iloc[0]. 
+00026330: 2020 2020 2020 2077 5f73 6d61 5f38 203d         w_sma_8 =
+00026340: 2070 6b74 616c 6962 2e53 4d41 2877 6565   pktalib.SMA(wee
+00026350: 6b6c 7944 6174 615b 2243 6c6f 7365 225d  klyData["Close"]
+00026360: 2c74 696d 6570 6572 696f 643d 3829 2e74  ,timeperiod=8).t
+00026370: 6169 6c28 3129 2e69 6c6f 635b 305d 0a20  ail(1).iloc[0]. 
+00026380: 2020 2020 2020 206e 756d 5072 6576 696f         numPrevio
+00026390: 7573 4361 6e64 6c65 7320 3d20 3230 0a20  usCandles = 20. 
+000263a0: 2020 2020 2020 2070 756c 6c62 6163 6b44         pullbackD
+000263b0: 6174 6120 3d20 6461 7461 2e68 6561 6428  ata = data.head(
+000263c0: 6e75 6d50 7265 7669 6f75 7343 616e 646c  numPreviousCandl
+000263d0: 6573 290a 2020 2020 2020 2020 7075 6c6c  es).        pull
+000263e0: 6261 636b 4461 7461 2e6c 6f63 5b3a 2c27  backData.loc[:,'
+000263f0: 5075 6c6c 4261 636b 275d 203d 2070 756c  PullBack'] = pul
+00026400: 6c62 6163 6b44 6174 615b 2243 6c6f 7365  lbackData["Close
+00026410: 225d 2e6c 7428 7075 6c6c 6261 636b 4461  "].lt(pullbackDa
+00026420: 7461 5b22 4f70 656e 225d 2920 232e 7368  ta["Open"]) #.sh
+00026430: 6966 7428 7065 7269 6f64 733d 3129 2920  ift(periods=1)) 
+00026440: 2326 2064 6174 615b 224c 6f77 225d 2e6c  #& data["Low"].l
+00026450: 7428 6461 7461 5b22 4c6f 7722 5d2e 7368  t(data["Low"].sh
+00026460: 6966 7428 7065 7269 6f64 733d 3129 290a  ift(periods=1)).
+00026470: 2020 2020 2020 2020 7368 7269 6e6b 6564          shrinked
+00026480: 566f 6c44 6174 6120 3d20 7075 6c6c 6261  VolData = pullba
+00026490: 636b 4461 7461 5b70 756c 6c62 6163 6b44  ckData[pullbackD
+000264a0: 6174 615b 2250 756c 6c42 6163 6b22 5d20  ata["PullBack"] 
+000264b0: 3d3d 2054 7275 655d 2e68 6561 6428 6e75  == True].head(nu
+000264c0: 6d50 7265 7669 6f75 7343 616e 646c 6573  mPreviousCandles
+000264d0: 290a 2020 2020 2020 2020 7265 6365 6e74  ).        recent
+000264e0: 4c61 7267 6573 7456 6f6c 756d 6520 3d20  LargestVolume = 
+000264f0: 6d61 7828 7075 6c6c 6261 636b 4461 7461  max(pullbackData
+00026500: 5b70 756c 6c62 6163 6b44 6174 615b 2250  [pullbackData["P
+00026510: 756c 6c42 6163 6b22 5d20 3d3d 2046 616c  ullBack"] == Fal
+00026520: 7365 5d2e 6865 6164 2833 295b 2256 6f6c  se].head(3)["Vol
+00026530: 756d 6522 5d29 0a20 2020 2020 2020 2023  ume"]).        #
+00026540: 2070 756c 6c62 6163 6b44 6174 612e 6c6f   pullbackData.lo
+00026550: 635b 3a2c 2750 4256 6f6c 5261 7469 6f27  c[:,'PBVolRatio'
+00026560: 5d20 3d20 7075 6c6c 6261 636b 4461 7461  ] = pullbackData
+00026570: 5b22 566f 6c75 6d65 225d 2f72 6563 656e  ["Volume"]/recen
+00026580: 744c 6172 6765 7374 566f 6c75 6d65 0a20  tLargestVolume. 
+00026590: 2020 2020 2020 2076 6f6c 496e 5072 6576         volInPrev
+000265a0: 696f 7573 5075 6c6c 6261 636b 7353 6872  iousPullbacksShr
+000265b0: 696e 6b65 6420 3d20 4661 6c73 650a 2020  inked = False.  
+000265c0: 2020 2020 2020 6966 206e 6f74 2073 6872        if not shr
+000265d0: 696e 6b65 6456 6f6c 4461 7461 2e65 6d70  inkedVolData.emp
+000265e0: 7479 3a0a 2020 2020 2020 2020 2020 2020  ty:.            
+000265f0: 696e 6465 7820 3d20 300a 2020 2020 2020  index = 0.      
+00026600: 2020 2020 2020 7768 696c 6520 696e 6465        while inde
+00026610: 7820 3c20 6c65 6e28 7368 7269 6e6b 6564  x < len(shrinked
+00026620: 566f 6c44 6174 6129 3a0a 2020 2020 2020  VolData):.      
+00026630: 2020 2020 2020 2020 2020 766f 6c49 6e50            volInP
+00026640: 7265 7669 6f75 7350 756c 6c62 6163 6b73  reviousPullbacks
+00026650: 5368 7269 6e6b 6564 203d 2073 6872 696e  Shrinked = shrin
+00026660: 6b65 6456 6f6c 4461 7461 5b22 566f 6c75  kedVolData["Volu
+00026670: 6d65 225d 2e69 6c6f 635b 696e 6465 785d  me"].iloc[index]
+00026680: 203c 2073 656c 662e 636f 6e66 6967 4d61   < self.configMa
+00026690: 6e61 6765 722e 7663 7056 6f6c 756d 6543  nager.vcpVolumeC
+000266a0: 6f6e 7472 6163 7469 6f6e 5261 7469 6f20  ontractionRatio 
+000266b0: 2a20 7265 6365 6e74 4c61 7267 6573 7456  * recentLargestV
+000266c0: 6f6c 756d 650a 2020 2020 2020 2020 2020  olume.          
+000266d0: 2020 2020 2020 6966 206e 6f74 2076 6f6c        if not vol
+000266e0: 496e 5072 6576 696f 7573 5075 6c6c 6261  InPreviousPullba
+000266f0: 636b 7353 6872 696e 6b65 643a 0a20 2020  cksShrinked:.   
+00026700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026710: 2062 7265 616b 0a20 2020 2020 2020 2020   break.         
+00026720: 2020 2020 2020 2069 6e64 6578 202b 3d20         index += 
+00026730: 310a 2020 2020 2020 2020 7265 6365 6e74  1.        recent
+00026740: 566f 6c75 6d65 4861 7341 626f 7665 4176  VolumeHasAboveAv
+00026750: 6756 6f6c 203d 2072 6563 656e 744c 6172  gVol = recentLar
+00026760: 6765 7374 566f 6c75 6d65 203e 3d20 7365  gestVolume >= se
+00026770: 6c66 2e63 6f6e 6669 674d 616e 6167 6572  lf.configManager
+00026780: 2e76 6f6c 756d 6552 6174 696f 202a 2064  .volumeRatio * d
+00026790: 6174 615b 2256 6f6c 4d41 225d 2e69 6c6f  ata["VolMA"].ilo
+000267a0: 635b 305d 0a20 2020 2020 2020 2069 7356  c[0].        isV
+000267b0: 4350 203d 2077 5f65 6d61 5f31 3320 3e20  CP = w_ema_13 > 
+000267c0: 775f 656d 615f 3236 2061 6e64 205c 0a20  w_ema_26 and \. 
+000267d0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+000267e0: 5f65 6d61 5f32 3620 3e20 775f 736d 615f  _ema_26 > w_sma_
+000267f0: 3530 2061 6e64 205c 0a20 2020 2020 2020  50 and \.       
+00026800: 2020 2020 2020 2020 2077 5f73 6d61 5f34           w_sma_4
+00026810: 3020 3e20 775f 736d 615f 3430 5f35 775f  0 > w_sma_40_5w_
+00026820: 6167 6f20 616e 6420 5c0a 2020 2020 2020  ago and \.      
+00026830: 2020 2020 2020 2020 2020 7265 6365 6e74            recent
+00026840: 5f63 6c6f 7365 203e 3d20 775f 6d69 6e5f  _close >= w_min_
+00026850: 3530 2061 6e64 205c 0a20 2020 2020 2020  50 and \.       
+00026860: 2020 2020 2020 2020 2072 6563 656e 745f           recent_
+00026870: 636c 6f73 6520 3e3d 2077 5f6d 6178 5f35  close >= w_max_5
+00026880: 3020 616e 6420 5c0a 2020 2020 2020 2020  0 and \.        
+00026890: 2020 2020 2020 2020 7265 6365 6e74 5f65          recent_e
+000268a0: 6d61 5f31 335f 3230 645f 6167 6f20 3e20  ma_13_20d_ago > 
+000268b0: 775f 656d 615f 3236 5f32 3077 5f61 676f  w_ema_26_20w_ago
+000268c0: 2061 6e64 205c 0a20 2020 2020 2020 2020   and \.         
+000268d0: 2020 2020 2020 2077 5f73 6d61 5f34 305f         w_sma_40_
+000268e0: 3577 5f61 676f 203e 2077 5f73 6d61 5f34  5w_ago > w_sma_4
+000268f0: 305f 3130 775f 6167 6f20 616e 6420 5c0a  0_10w_ago and \.
+00026900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026910: 7265 6365 6e74 5f63 6c6f 7365 203e 2072  recent_close > r
+00026920: 6563 656e 745f 736d 615f 3530 2061 6e64  ecent_sma_50 and
+00026930: 205c 0a20 2020 2020 2020 2020 2020 2020   \.             
+00026940: 2020 2028 775f 776d 615f 3820 2d20 775f     (w_wma_8 - w_
+00026950: 736d 615f 3829 2a36 2f32 3920 3c20 302e  sma_8)*6/29 < 0.
+00026960: 3520 616e 6420 5c0a 2020 2020 2020 2020  5 and \.        
+00026970: 2020 2020 2020 2020 766f 6c49 6e50 7265          volInPre
+00026980: 7669 6f75 7350 756c 6c62 6163 6b73 5368  viousPullbacksSh
+00026990: 7269 6e6b 6564 2061 6e64 205c 0a20 2020  rinked and \.   
+000269a0: 2020 2020 2020 2020 2020 2020 2072 6563               rec
+000269b0: 656e 7456 6f6c 756d 6548 6173 4162 6f76  entVolumeHasAbov
+000269c0: 6541 7667 566f 6c20 616e 6420 5c0a 2020  eAvgVol and \.  
+000269d0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+000269e0: 6365 6e74 5f63 6c6f 7365 203e 2031 300a  cent_close > 10.
+000269f0: 2020 2020 2020 2020 6966 2069 7356 4350          if isVCP
+00026a00: 3a0a 2020 2020 2020 2020 2020 2020 7361  :.            sa
+00026a10: 7665 6420 3d20 7365 6c66 2e66 696e 6443  ved = self.findC
+00026a20: 7572 7265 6e74 5361 7665 6456 616c 7565  urrentSavedValue
+00026a30: 2873 6372 6565 6e44 6963 742c 2073 6176  (screenDict, sav
+00026a40: 6544 6963 742c 2022 5061 7474 6572 6e22  eDict, "Pattern"
+00026a50: 290a 2020 2020 2020 2020 2020 2020 7363  ).            sc
+00026a60: 7265 656e 4469 6374 5b22 5061 7474 6572  reenDict["Patter
+00026a70: 6e22 5d20 3d20 280a 2020 2020 2020 2020  n"] = (.        
+00026a80: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
+00026a90: 200a 2020 2020 2020 2020 2020 2020 2020   .              
+00026aa0: 2020 2b20 636f 6c6f 7254 6578 742e 424f    + colorText.BO
+00026ab0: 4c44 0a20 2020 2020 2020 2020 2020 2020  LD.             
+00026ac0: 2020 202b 2063 6f6c 6f72 5465 7874 2e47     + colorText.G
+00026ad0: 5245 454e 0a20 2020 2020 2020 2020 2020  REEN.           
+00026ae0: 2020 2020 202b 2066 2256 4350 284d 696e       + f"VCP(Min
+00026af0: 6572 7669 6e69 2922 0a20 2020 2020 2020  ervini)".       
+00026b00: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
+00026b10: 5465 7874 2e45 4e44 0a20 2020 2020 2020  Text.END.       
+00026b20: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00026b30: 2020 2073 6176 6544 6963 745b 2250 6174     saveDict["Pat
+00026b40: 7465 726e 225d 203d 2073 6176 6564 5b31  tern"] = saved[1
+00026b50: 5d20 2b20 6622 5643 5028 4d69 6e65 7276  ] + f"VCP(Minerv
+00026b60: 696e 6929 220a 2020 2020 2020 2020 7265  ini)".        re
+00026b70: 7475 726e 2069 7356 4350 0a20 2020 200a  turn isVCP.    .
+00026b80: 2020 2020 2320 5661 6c69 6461 7465 2056      # Validate V
+00026b90: 4350 0a20 2020 2064 6566 2076 616c 6964  CP.    def valid
+00026ba0: 6174 6556 4350 280a 2020 2020 2020 2020  ateVCP(.        
+00026bb0: 7365 6c66 2c20 6466 2c20 7363 7265 656e  self, df, screen
+00026bc0: 4469 6374 2c20 7361 7665 4469 6374 2c20  Dict, saveDict, 
+00026bd0: 7374 6f63 6b4e 616d 653d 4e6f 6e65 2c20  stockName=None, 
+00026be0: 7769 6e64 6f77 3d33 2c20 7065 7263 656e  window=3, percen
+00026bf0: 7461 6765 4672 6f6d 546f 703d 330a 2020  tageFromTop=3.  
+00026c00: 2020 293a 0a20 2020 2020 2020 2069 6620    ):.        if 
+00026c10: 6466 2069 7320 4e6f 6e65 206f 7220 6c65  df is None or le
+00026c20: 6e28 6466 2920 3d3d 2030 3a0a 2020 2020  n(df) == 0:.    
+00026c30: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+00026c40: 616c 7365 0a20 2020 2020 2020 2064 6174  alse.        dat
+00026c50: 6120 3d20 6466 2e63 6f70 7928 290a 2020  a = df.copy().  
+00026c60: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+00026c70: 2020 2020 2020 2070 6572 6365 6e74 6167         percentag
+00026c80: 6546 726f 6d54 6f70 202f 3d20 3130 300a  eFromTop /= 100.
+00026c90: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00026ca0: 2e72 6573 6574 5f69 6e64 6578 2869 6e70  .reset_index(inp
+00026cb0: 6c61 6365 3d54 7275 6529 0a20 2020 2020  lace=True).     
+00026cc0: 2020 2020 2020 2064 6174 612e 7265 6e61         data.rena
+00026cd0: 6d65 2863 6f6c 756d 6e73 3d7b 2269 6e64  me(columns={"ind
+00026ce0: 6578 223a 2022 4461 7465 227d 2c20 696e  ex": "Date"}, in
+00026cf0: 706c 6163 653d 5472 7565 290a 2020 2020  place=True).    
+00026d00: 2020 2020 2020 2020 6461 7461 5b22 746f          data["to
+00026d10: 7073 225d 203d 2028 6461 7461 5b22 4869  ps"] = (data["Hi
+00026d20: 6768 225d 2e69 6c6f 635b 6c69 7374 2870  gh"].iloc[list(p
+00026d30: 6b74 616c 6962 2e61 7267 7265 6c65 7874  ktalib.argrelext
+00026d40: 7265 6d61 286e 702e 6172 7261 7928 6461  rema(np.array(da
+00026d50: 7461 5b22 4869 6768 225d 292c 206e 702e  ta["High"]), np.
+00026d60: 6772 6561 7465 725f 6571 7561 6c2c 206f  greater_equal, o
+00026d70: 7264 6572 3d77 696e 646f 7729 5b30 5d29  rder=window)[0])
+00026d80: 5d2e 6865 6164 2834 2929 0a20 2020 2020  ].head(4)).     
+00026d90: 2020 2020 2020 2064 6174 615b 2262 6f74         data["bot
+00026da0: 7322 5d20 3d20 2864 6174 615b 224c 6f77  s"] = (data["Low
+00026db0: 225d 2e69 6c6f 635b 6c69 7374 2870 6b74  "].iloc[list(pkt
+00026dc0: 616c 6962 2e61 7267 7265 6c65 7874 7265  alib.argrelextre
+00026dd0: 6d61 286e 702e 6172 7261 7928 6461 7461  ma(np.array(data
+00026de0: 5b22 4c6f 7722 5d29 2c20 6e70 2e6c 6573  ["Low"]), np.les
+00026df0: 735f 6571 7561 6c2c 206f 7264 6572 3d77  s_equal, order=w
+00026e00: 696e 646f 7729 5b30 5d29 5d2e 6865 6164  indow)[0])].head
+00026e10: 2834 2929 0a20 2020 2020 2020 2020 2020  (4)).           
+00026e20: 2064 6174 6120 3d20 6461 7461 2e66 696c   data = data.fil
+00026e30: 6c6e 6128 3029 0a20 2020 2020 2020 2020  lna(0).         
+00026e40: 2020 2064 6174 6120 3d20 6461 7461 2e72     data = data.r
+00026e50: 6570 6c61 6365 285b 6e70 2e69 6e66 2c20  eplace([np.inf, 
+00026e60: 2d6e 702e 696e 665d 2c20 3029 0a20 2020  -np.inf], 0).   
+00026e70: 2020 2020 2020 2020 2074 6f70 7320 3d20           tops = 
+00026e80: 6461 7461 5b64 6174 612e 746f 7073 203e  data[data.tops >
+00026e90: 2030 5d0a 2020 2020 2020 2020 2020 2020   0].            
+00026ea0: 2320 626f 7473 203d 2064 6174 615b 6461  # bots = data[da
+00026eb0: 7461 2e62 6f74 7320 3e20 305d 0a20 2020  ta.bots > 0].   
+00026ec0: 2020 2020 2020 2020 2068 6967 6865 7374           highest
+00026ed0: 546f 7020 3d20 726f 756e 6428 746f 7073  Top = round(tops
+00026ee0: 2e64 6573 6372 6962 6528 295b 2248 6967  .describe()["Hig
+00026ef0: 6822 5d5b 226d 6178 225d 2c20 3129 0a20  h"]["max"], 1). 
+00026f00: 2020 2020 2020 2020 2020 2066 696c 7465             filte
+00026f10: 7265 6454 6f70 7320 3d20 746f 7073 5b0a  redTops = tops[.
+00026f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026f30: 746f 7073 2e74 6f70 7320 3e20 2868 6967  tops.tops > (hig
+00026f40: 6865 7374 546f 7020 2d20 2868 6967 6865  hestTop - (highe
+00026f50: 7374 546f 7020 2a20 7065 7263 656e 7461  stTop * percenta
+00026f60: 6765 4672 6f6d 546f 7029 290a 2020 2020  geFromTop)).    
+00026f70: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
+00026f80: 2020 2020 2020 6966 2066 696c 7465 7265        if filtere
+00026f90: 6454 6f70 732e 6571 7561 6c73 2874 6f70  dTops.equals(top
+00026fa0: 7329 3a20 2023 2054 6f70 7320 6172 6520  s):  # Tops are 
+00026fb0: 696e 2074 6865 2072 616e 6765 0a20 2020  in the range.   
+00026fc0: 2020 2020 2020 2020 2020 2020 206c 6f77               low
+00026fd0: 506f 696e 7473 203d 205b 5d0a 2020 2020  Points = [].    
+00026fe0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00026ff0: 6920 696e 2072 616e 6765 286c 656e 2874  i in range(len(t
+00027000: 6f70 7329 202d 2031 293a 0a20 2020 2020  ops) - 1):.     
+00027010: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00027020: 6e64 4461 7465 203d 2074 6f70 732e 696c  ndDate = tops.il
+00027030: 6f63 5b69 5d5b 2244 6174 6522 5d0a 2020  oc[i]["Date"].  
+00027040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027050: 2020 7374 6172 7444 6174 6520 3d20 746f    startDate = to
+00027060: 7073 2e69 6c6f 635b 6920 2b20 315d 5b22  ps.iloc[i + 1]["
+00027070: 4461 7465 225d 0a20 2020 2020 2020 2020  Date"].         
+00027080: 2020 2020 2020 2020 2020 206c 6f77 506f             lowPo
+00027090: 696e 7473 2e61 7070 656e 6428 0a20 2020  ints.append(.   
+000270a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000270b0: 2020 2020 2064 6174 615b 0a20 2020 2020       data[.     
 000270c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000270d0: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
-000270e0: 2e45 4e44 0a20 2020 2020 2020 2020 2020  .END.           
-000270f0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00027100: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00027110: 6176 6544 6963 745b 2250 6174 7465 726e  aveDict["Pattern
-00027120: 225d 203d 2073 6176 6564 5b31 5d20 2b20  "] = saved[1] + 
-00027130: 6622 5643 5020 2842 4f3a 207b 6869 6768  f"VCP (BO: {high
-00027140: 6573 7454 6f70 7d29 220a 2020 2020 2020  estTop})".      
-00027150: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00027160: 7475 726e 2054 7275 650a 2020 2020 2020  turn True.      
-00027170: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
-00027180: 6f6e 2061 7320 653a 2020 2320 7072 6167  on as e:  # prag
-00027190: 6d61 3a20 6e6f 2063 6f76 6572 0a20 2020  ma: no cover.   
-000271a0: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
-000271b0: 6661 756c 745f 6c6f 6767 6572 2e64 6562  fault_logger.deb
-000271c0: 7567 2865 2c20 6578 635f 696e 666f 3d54  ug(e, exc_info=T
-000271d0: 7275 6529 0a20 2020 2020 2020 2072 6574  rue).        ret
-000271e0: 7572 6e20 4661 6c73 650a 0a20 2020 2023  urn False..    #
-000271f0: 2056 616c 6964 6174 6520 6966 2076 6f6c   Validate if vol
-00027200: 756d 6520 6f66 206c 6173 7420 6461 7920  ume of last day 
-00027210: 6973 2068 6967 6865 7220 7468 616e 2061  is higher than a
-00027220: 7667 0a20 2020 2064 6566 2076 616c 6964  vg.    def valid
-00027230: 6174 6556 6f6c 756d 6528 0a20 2020 2020  ateVolume(.     
-00027240: 2020 2073 656c 662c 2064 662c 2073 6372     self, df, scr
-00027250: 6565 6e44 6963 742c 2073 6176 6544 6963  eenDict, saveDic
-00027260: 742c 2076 6f6c 756d 6552 6174 696f 3d32  t, volumeRatio=2
-00027270: 2e35 2c20 6d69 6e56 6f6c 756d 653d 3130  .5, minVolume=10
-00027280: 300a 2020 2020 293a 0a20 2020 2020 2020  0.    ):.       
-00027290: 2069 6620 6466 2069 7320 4e6f 6e65 206f   if df is None o
-000272a0: 7220 6c65 6e28 6466 2920 3d3d 2030 3a0a  r len(df) == 0:.
-000272b0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000272c0: 726e 2046 616c 7365 2c20 4661 6c73 650a  rn False, False.
-000272d0: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
-000272e0: 662e 636f 7079 2829 0a20 2020 2020 2020  f.copy().       
-000272f0: 2064 6174 6120 3d20 6461 7461 2e66 696c   data = data.fil
-00027300: 6c6e 6128 3029 0a20 2020 2020 2020 2064  lna(0).        d
-00027310: 6174 6120 3d20 6461 7461 2e72 6570 6c61  ata = data.repla
-00027320: 6365 285b 6e70 2e69 6e66 2c20 2d6e 702e  ce([np.inf, -np.
-00027330: 696e 665d 2c20 3029 0a20 2020 2020 2020  inf], 0).       
-00027340: 2072 6563 656e 7420 3d20 6461 7461 2e68   recent = data.h
-00027350: 6561 6428 3129 0a20 2020 2020 2020 2023  ead(1).        #
-00027360: 2045 6974 6865 7220 7468 6520 726f 6c6c   Either the roll
-00027370: 696e 6720 766f 6c75 6d65 206f 6620 7061  ing volume of pa
-00027380: 7374 2032 3020 7365 7373 696f 6e73 206f  st 20 sessions o
-00027390: 7220 746f 6461 7927 7320 766f 6c75 6d65  r today's volume
-000273a0: 2073 686f 756c 6420 6265 203e 206d 696e   should be > min
-000273b0: 2076 6f6c 756d 650a 2020 2020 2020 2020   volume.        
-000273c0: 6861 734d 696e 696d 756d 566f 6c75 6d65  hasMinimumVolume
-000273d0: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
-000273e0: 2072 6563 656e 745b 2256 6f6c 4d41 225d   recent["VolMA"]
-000273f0: 2e69 6c6f 635b 305d 203e 3d20 6d69 6e56  .iloc[0] >= minV
-00027400: 6f6c 756d 650a 2020 2020 2020 2020 2020  olume.          
-00027410: 2020 6f72 2072 6563 656e 745b 2256 6f6c    or recent["Vol
-00027420: 756d 6522 5d2e 696c 6f63 5b30 5d20 3e3d  ume"].iloc[0] >=
-00027430: 206d 696e 566f 6c75 6d65 0a20 2020 2020   minVolume.     
-00027440: 2020 2029 0a20 2020 2020 2020 2069 6620     ).        if 
-00027450: 7265 6365 6e74 5b22 566f 6c4d 4122 5d2e  recent["VolMA"].
-00027460: 696c 6f63 5b30 5d20 3d3d 2030 3a20 2023  iloc[0] == 0:  #
-00027470: 2048 616e 646c 6573 2044 6976 6964 6520   Handles Divide 
-00027480: 6279 2030 2077 6172 6e69 6e67 0a20 2020  by 0 warning.   
-00027490: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
-000274a0: 745b 2256 6f6c 756d 6522 5d20 3d20 3020  t["Volume"] = 0 
-000274b0: 2023 2022 556e 6b6e 6f77 6e22 0a20 2020   # "Unknown".   
-000274c0: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
-000274d0: 6963 745b 2256 6f6c 756d 6522 5d20 3d20  ict["Volume"] = 
-000274e0: 300a 2020 2020 2020 2020 2020 2020 7265  0.            re
-000274f0: 7475 726e 2046 616c 7365 2c20 6861 734d  turn False, hasM
-00027500: 696e 696d 756d 566f 6c75 6d65 0a20 2020  inimumVolume.   
-00027510: 2020 2020 2072 6174 696f 203d 2072 6f75       ratio = rou
-00027520: 6e64 2872 6563 656e 745b 2256 6f6c 756d  nd(recent["Volum
-00027530: 6522 5d2e 696c 6f63 5b30 5d20 2f20 7265  e"].iloc[0] / re
-00027540: 6365 6e74 5b22 566f 6c4d 4122 5d2e 696c  cent["VolMA"].il
-00027550: 6f63 5b30 5d2c 2032 290a 2020 2020 2020  oc[0], 2).      
-00027560: 2020 7361 7665 4469 6374 5b22 566f 6c75    saveDict["Volu
-00027570: 6d65 225d 203d 2072 6174 696f 0a20 2020  me"] = ratio.   
-00027580: 2020 2020 2069 6620 7261 7469 6f20 3e3d       if ratio >=
-00027590: 2076 6f6c 756d 6552 6174 696f 2061 6e64   volumeRatio and
-000275a0: 2072 6174 696f 2021 3d20 6e70 2e6e 616e   ratio != np.nan
-000275b0: 2061 6e64 2028 6e6f 7420 6d61 7468 2e69   and (not math.i
-000275c0: 7369 6e66 2872 6174 696f 2929 3a0a 2020  sinf(ratio)):.  
-000275d0: 2020 2020 2020 2020 2020 7363 7265 656e            screen
-000275e0: 4469 6374 5b22 566f 6c75 6d65 225d 203d  Dict["Volume"] =
-000275f0: 2072 6174 696f 0a20 2020 2020 2020 2020   ratio.         
-00027600: 2020 2072 6574 7572 6e20 5472 7565 2c20     return True, 
-00027610: 6861 734d 696e 696d 756d 566f 6c75 6d65  hasMinimumVolume
-00027620: 0a20 2020 2020 2020 2073 6372 6565 6e44  .        screenD
-00027630: 6963 745b 2256 6f6c 756d 6522 5d20 3d20  ict["Volume"] = 
-00027640: 7261 7469 6f0a 2020 2020 2020 2020 7265  ratio.        re
-00027650: 7475 726e 2046 616c 7365 2c20 6861 734d  turn False, hasM
-00027660: 696e 696d 756d 566f 6c75 6d65 0a0a 2020  inimumVolume..  
-00027670: 2020 2320 4669 6e64 2069 6620 7374 6f63    # Find if stoc
-00027680: 6b20 6973 2076 616c 6964 6174 696e 6720  k is validating 
-00027690: 766f 6c75 6d65 2073 7072 6561 6420 616e  volume spread an
-000276a0: 616c 7973 6973 0a20 2020 2064 6566 2076  alysis.    def v
-000276b0: 616c 6964 6174 6556 6f6c 756d 6553 7072  alidateVolumeSpr
-000276c0: 6561 6441 6e61 6c79 7369 7328 7365 6c66  eadAnalysis(self
-000276d0: 2c20 6466 2c20 7363 7265 656e 4469 6374  , df, screenDict
-000276e0: 2c20 7361 7665 4469 6374 293a 0a20 2020  , saveDict):.   
-000276f0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-00027700: 2020 2020 2020 6966 2064 6620 6973 204e        if df is N
-00027710: 6f6e 6520 6f72 206c 656e 2864 6629 203d  one or len(df) =
-00027720: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
-00027730: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-00027740: 650a 2020 2020 2020 2020 2020 2020 6461  e.            da
-00027750: 7461 203d 2064 662e 636f 7079 2829 0a20  ta = df.copy(). 
-00027760: 2020 2020 2020 2020 2020 2064 6174 6120             data 
-00027770: 3d20 6461 7461 2e68 6561 6428 3229 0a20  = data.head(2). 
-00027780: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
-00027790: 6e28 6461 7461 2920 3c20 323a 0a20 2020  n(data) < 2:.   
-000277a0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-000277b0: 7572 6e20 4661 6c73 650a 2020 2020 2020  urn False.      
-000277c0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-000277d0: 2020 2020 2020 2020 2020 2023 2043 6865             # Che
-000277e0: 636b 2066 6f72 2070 7265 7669 6f75 7320  ck for previous 
-000277f0: 5245 4420 6361 6e64 6c65 730a 2020 2020  RED candles.    
-00027800: 2020 2020 2020 2020 2020 2020 2320 4375              # Cu
-00027810: 7272 656e 7420 6361 6e64 6c65 203d 2030  rrent candle = 0
-00027820: 7468 2c20 5072 6576 696f 7573 2043 616e  th, Previous Can
-00027830: 646c 6520 3d20 3173 7420 666f 7220 666f  dle = 1st for fo
-00027840: 6c6c 6f77 696e 6720 6c6f 6769 630a 2020  llowing logic.  
-00027850: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00027860: 2064 6174 612e 696c 6f63 5b31 5d5b 224f   data.iloc[1]["O
-00027870: 7065 6e22 5d20 3e3d 2064 6174 612e 696c  pen"] >= data.il
-00027880: 6f63 5b31 5d5b 2243 6c6f 7365 225d 3a0a  oc[1]["Close"]:.
-00027890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000278a0: 2020 2020 7370 7265 6164 3120 3d20 6162      spread1 = ab
-000278b0: 7328 6461 7461 2e69 6c6f 635b 315d 5b22  s(data.iloc[1]["
-000278c0: 4f70 656e 225d 202d 2064 6174 612e 696c  Open"] - data.il
-000278d0: 6f63 5b31 5d5b 2243 6c6f 7365 225d 290a  oc[1]["Close"]).
-000278e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000278f0: 2020 2020 7370 7265 6164 3020 3d20 6162      spread0 = ab
-00027900: 7328 6461 7461 2e69 6c6f 635b 305d 5b22  s(data.iloc[0]["
-00027910: 4f70 656e 225d 202d 2064 6174 612e 696c  Open"] - data.il
-00027920: 6f63 5b30 5d5b 2243 6c6f 7365 225d 290a  oc[0]["Close"]).
-00027930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027940: 2020 2020 6c6f 7765 725f 7769 636b 5f73      lower_wick_s
-00027950: 7072 6561 6430 203d 2028 0a20 2020 2020  pread0 = (.     
-00027960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027970: 2020 206d 6178 2864 6174 612e 696c 6f63     max(data.iloc
-00027980: 5b30 5d5b 224f 7065 6e22 5d2c 2064 6174  [0]["Open"], dat
-00027990: 612e 696c 6f63 5b30 5d5b 2243 6c6f 7365  a.iloc[0]["Close
-000279a0: 225d 290a 2020 2020 2020 2020 2020 2020  "]).            
-000279b0: 2020 2020 2020 2020 2020 2020 2d20 6461              - da
-000279c0: 7461 2e69 6c6f 635b 305d 5b22 4c6f 7722  ta.iloc[0]["Low"
-000279d0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-000279e0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000279f0: 2020 2020 2020 2020 2020 2020 766f 6c31              vol1
-00027a00: 203d 2064 6174 612e 696c 6f63 5b31 5d5b   = data.iloc[1][
-00027a10: 2256 6f6c 756d 6522 5d0a 2020 2020 2020  "Volume"].      
-00027a20: 2020 2020 2020 2020 2020 2020 2020 766f                vo
-00027a30: 6c30 203d 2064 6174 612e 696c 6f63 5b30  l0 = data.iloc[0
-00027a40: 5d5b 2256 6f6c 756d 6522 5d0a 2020 2020  ]["Volume"].    
-00027a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027a60: 7361 7665 6420 3d20 7365 6c66 2e66 696e  saved = self.fin
-00027a70: 6443 7572 7265 6e74 5361 7665 6456 616c  dCurrentSavedVal
-00027a80: 7565 2873 6372 6565 6e44 6963 742c 2073  ue(screenDict, s
-00027a90: 6176 6544 6963 742c 2022 5061 7474 6572  aveDict, "Patter
-00027aa0: 6e22 290a 2020 2020 2020 2020 2020 2020  n").            
-00027ab0: 2020 2020 2020 2020 6966 2028 0a20 2020          if (.   
-00027ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027ad0: 2020 2020 2073 7072 6561 6430 203e 2073       spread0 > s
-00027ae0: 7072 6561 6431 0a20 2020 2020 2020 2020  pread1.         
-00027af0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00027b00: 6e64 2076 6f6c 3020 3c20 766f 6c31 0a20  nd vol0 < vol1. 
-00027b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027b20: 2020 2020 2020 2061 6e64 2064 6174 612e         and data.
-00027b30: 696c 6f63 5b30 5d5b 2256 6f6c 756d 6522  iloc[0]["Volume"
-00027b40: 5d20 3c20 6461 7461 2e69 6c6f 635b 305d  ] < data.iloc[0]
-00027b50: 5b22 566f 6c4d 4122 5d0a 2020 2020 2020  ["VolMA"].      
-00027b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027b70: 2020 616e 6420 6461 7461 2e69 6c6f 635b    and data.iloc[
-00027b80: 305d 5b22 436c 6f73 6522 5d20 3c3d 2064  0]["Close"] <= d
-00027b90: 6174 612e 696c 6f63 5b31 5d5b 224f 7065  ata.iloc[1]["Ope
-00027ba0: 6e22 5d0a 2020 2020 2020 2020 2020 2020  n"].            
-00027bb0: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-00027bc0: 7370 7265 6164 3020 3c20 6c6f 7765 725f  spread0 < lower_
-00027bd0: 7769 636b 5f73 7072 6561 6430 0a20 2020  wick_spread0.   
-00027be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027bf0: 2020 2020 2061 6e64 2064 6174 612e 696c       and data.il
-00027c00: 6f63 5b30 5d5b 2256 6f6c 756d 6522 5d20  oc[0]["Volume"] 
-00027c10: 3c3d 2069 6e74 2864 6174 612e 696c 6f63  <= int(data.iloc
-00027c20: 5b31 5d5b 2256 6f6c 756d 6522 5d20 2a20  [1]["Volume"] * 
-00027c30: 302e 3735 290a 2020 2020 2020 2020 2020  0.75).          
-00027c40: 2020 2020 2020 2020 2020 293a 0a20 2020            ):.   
-00027c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027c60: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
-00027c70: 2250 6174 7465 726e 225d 203d 2028 0a20  "Pattern"] = (. 
-00027c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027c90: 2020 2020 2020 2020 2020 2073 6176 6564             saved
-00027ca0: 5b30 5d20 0a20 2020 2020 2020 2020 2020  [0] .           
+000270d0: 2020 2020 2020 2028 6461 7461 2e44 6174         (data.Dat
+000270e0: 6520 3e3d 2073 7461 7274 4461 7465 2920  e >= startDate) 
+000270f0: 2620 2864 6174 612e 4461 7465 203c 3d20  & (data.Date <= 
+00027100: 656e 6444 6174 6529 0a20 2020 2020 2020  endDate).       
+00027110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027120: 205d 2e64 6573 6372 6962 6528 295b 224c   ].describe()["L
+00027130: 6f77 225d 5b22 6d69 6e22 5d0a 2020 2020  ow"]["min"].    
+00027140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027150: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00027160: 2020 6c6f 7750 6f69 6e74 734f 7267 203d    lowPointsOrg =
+00027170: 206c 6f77 506f 696e 7473 0a20 2020 2020   lowPoints.     
+00027180: 2020 2020 2020 2020 2020 206c 6f77 506f             lowPo
+00027190: 696e 7473 2e73 6f72 7428 7265 7665 7273  ints.sort(revers
+000271a0: 653d 5472 7565 290a 2020 2020 2020 2020  e=True).        
+000271b0: 2020 2020 2020 2020 6c6f 7750 6f69 6e74          lowPoint
+000271c0: 7353 6f72 7465 6420 3d20 6c6f 7750 6f69  sSorted = lowPoi
+000271d0: 6e74 730a 2020 2020 2020 2020 2020 2020  nts.            
+000271e0: 2020 2020 6966 2064 6174 612e 656d 7074      if data.empt
+000271f0: 7920 6f72 206c 656e 286c 6f77 506f 696e  y or len(lowPoin
+00027200: 7473 2920 3c20 313a 0a20 2020 2020 2020  ts) < 1:.       
+00027210: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00027220: 7572 6e20 4661 6c73 650a 2020 2020 2020  urn False.      
+00027230: 2020 2020 2020 2020 2020 6c74 7020 3d20            ltp = 
+00027240: 6461 7461 2e68 6561 6428 3129 5b22 436c  data.head(1)["Cl
+00027250: 6f73 6522 5d2e 696c 6f63 5b30 5d0a 2020  ose"].iloc[0].  
+00027260: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00027270: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+00027280: 2020 2020 2020 206c 6f77 506f 696e 7473         lowPoints
+00027290: 4f72 6720 3d3d 206c 6f77 506f 696e 7473  Org == lowPoints
+000272a0: 536f 7274 6564 0a20 2020 2020 2020 2020  Sorted.         
+000272b0: 2020 2020 2020 2020 2020 2061 6e64 206c             and l
+000272c0: 7470 203c 2068 6967 6865 7374 546f 700a  tp < highestTop.
+000272d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000272e0: 2020 2020 616e 6420 6c74 7020 3e20 6c6f      and ltp > lo
+000272f0: 7750 6f69 6e74 735b 305d 0a20 2020 2020  wPoints[0].     
+00027300: 2020 2020 2020 2020 2020 2029 3a0a 2020             ):.  
+00027310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027320: 2020 7361 7665 6420 3d20 7365 6c66 2e66    saved = self.f
+00027330: 696e 6443 7572 7265 6e74 5361 7665 6456  indCurrentSavedV
+00027340: 616c 7565 2873 6372 6565 6e44 6963 742c  alue(screenDict,
+00027350: 2073 6176 6544 6963 742c 2022 5061 7474   saveDict, "Patt
+00027360: 6572 6e22 290a 2020 2020 2020 2020 2020  ern").          
+00027370: 2020 2020 2020 2020 2020 7363 7265 656e            screen
+00027380: 4469 6374 5b22 5061 7474 6572 6e22 5d20  Dict["Pattern"] 
+00027390: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+000273a0: 2020 2020 2020 2020 2020 2020 7361 7665              save
+000273b0: 645b 305d 200a 2020 2020 2020 2020 2020  d[0] .          
+000273c0: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+000273d0: 636f 6c6f 7254 6578 742e 424f 4c44 0a20  colorText.BOLD. 
+000273e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000273f0: 2020 2020 2020 202b 2063 6f6c 6f72 5465         + colorTe
+00027400: 7874 2e47 5245 454e 0a20 2020 2020 2020  xt.GREEN.       
+00027410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027420: 202b 2066 2256 4350 2028 424f 3a20 7b68   + f"VCP (BO: {h
+00027430: 6967 6865 7374 546f 707d 2922 0a20 2020  ighestTop})".   
+00027440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027450: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
+00027460: 2e45 4e44 0a20 2020 2020 2020 2020 2020  .END.           
+00027470: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00027480: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00027490: 6176 6544 6963 745b 2250 6174 7465 726e  aveDict["Pattern
+000274a0: 225d 203d 2073 6176 6564 5b31 5d20 2b20  "] = saved[1] + 
+000274b0: 6622 5643 5020 2842 4f3a 207b 6869 6768  f"VCP (BO: {high
+000274c0: 6573 7454 6f70 7d29 220a 2020 2020 2020  estTop})".      
+000274d0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+000274e0: 7475 726e 2054 7275 650a 2020 2020 2020  turn True.      
+000274f0: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
+00027500: 6f6e 2061 7320 653a 2020 2320 7072 6167  on as e:  # prag
+00027510: 6d61 3a20 6e6f 2063 6f76 6572 0a20 2020  ma: no cover.   
+00027520: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
+00027530: 6661 756c 745f 6c6f 6767 6572 2e64 6562  fault_logger.deb
+00027540: 7567 2865 2c20 6578 635f 696e 666f 3d54  ug(e, exc_info=T
+00027550: 7275 6529 0a20 2020 2020 2020 2072 6574  rue).        ret
+00027560: 7572 6e20 4661 6c73 650a 0a20 2020 2023  urn False..    #
+00027570: 2056 616c 6964 6174 6520 6966 2076 6f6c   Validate if vol
+00027580: 756d 6520 6f66 206c 6173 7420 6461 7920  ume of last day 
+00027590: 6973 2068 6967 6865 7220 7468 616e 2061  is higher than a
+000275a0: 7667 0a20 2020 2064 6566 2076 616c 6964  vg.    def valid
+000275b0: 6174 6556 6f6c 756d 6528 0a20 2020 2020  ateVolume(.     
+000275c0: 2020 2073 656c 662c 2064 662c 2073 6372     self, df, scr
+000275d0: 6565 6e44 6963 742c 2073 6176 6544 6963  eenDict, saveDic
+000275e0: 742c 2076 6f6c 756d 6552 6174 696f 3d32  t, volumeRatio=2
+000275f0: 2e35 2c20 6d69 6e56 6f6c 756d 653d 3130  .5, minVolume=10
+00027600: 300a 2020 2020 293a 0a20 2020 2020 2020  0.    ):.       
+00027610: 2069 6620 6466 2069 7320 4e6f 6e65 206f   if df is None o
+00027620: 7220 6c65 6e28 6466 2920 3d3d 2030 3a0a  r len(df) == 0:.
+00027630: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00027640: 726e 2046 616c 7365 2c20 4661 6c73 650a  rn False, False.
+00027650: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
+00027660: 662e 636f 7079 2829 0a20 2020 2020 2020  f.copy().       
+00027670: 2064 6174 6120 3d20 6461 7461 2e66 696c   data = data.fil
+00027680: 6c6e 6128 3029 0a20 2020 2020 2020 2064  lna(0).        d
+00027690: 6174 6120 3d20 6461 7461 2e72 6570 6c61  ata = data.repla
+000276a0: 6365 285b 6e70 2e69 6e66 2c20 2d6e 702e  ce([np.inf, -np.
+000276b0: 696e 665d 2c20 3029 0a20 2020 2020 2020  inf], 0).       
+000276c0: 2072 6563 656e 7420 3d20 6461 7461 2e68   recent = data.h
+000276d0: 6561 6428 3129 0a20 2020 2020 2020 2023  ead(1).        #
+000276e0: 2045 6974 6865 7220 7468 6520 726f 6c6c   Either the roll
+000276f0: 696e 6720 766f 6c75 6d65 206f 6620 7061  ing volume of pa
+00027700: 7374 2032 3020 7365 7373 696f 6e73 206f  st 20 sessions o
+00027710: 7220 746f 6461 7927 7320 766f 6c75 6d65  r today's volume
+00027720: 2073 686f 756c 6420 6265 203e 206d 696e   should be > min
+00027730: 2076 6f6c 756d 650a 2020 2020 2020 2020   volume.        
+00027740: 6861 734d 696e 696d 756d 566f 6c75 6d65  hasMinimumVolume
+00027750: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
+00027760: 2072 6563 656e 745b 2256 6f6c 4d41 225d   recent["VolMA"]
+00027770: 2e69 6c6f 635b 305d 203e 3d20 6d69 6e56  .iloc[0] >= minV
+00027780: 6f6c 756d 650a 2020 2020 2020 2020 2020  olume.          
+00027790: 2020 6f72 2072 6563 656e 745b 2256 6f6c    or recent["Vol
+000277a0: 756d 6522 5d2e 696c 6f63 5b30 5d20 3e3d  ume"].iloc[0] >=
+000277b0: 206d 696e 566f 6c75 6d65 0a20 2020 2020   minVolume.     
+000277c0: 2020 2029 0a20 2020 2020 2020 2069 6620     ).        if 
+000277d0: 7265 6365 6e74 5b22 566f 6c4d 4122 5d2e  recent["VolMA"].
+000277e0: 696c 6f63 5b30 5d20 3d3d 2030 3a20 2023  iloc[0] == 0:  #
+000277f0: 2048 616e 646c 6573 2044 6976 6964 6520   Handles Divide 
+00027800: 6279 2030 2077 6172 6e69 6e67 0a20 2020  by 0 warning.   
+00027810: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
+00027820: 745b 2256 6f6c 756d 6522 5d20 3d20 3020  t["Volume"] = 0 
+00027830: 2023 2022 556e 6b6e 6f77 6e22 0a20 2020   # "Unknown".   
+00027840: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
+00027850: 6963 745b 2256 6f6c 756d 6522 5d20 3d20  ict["Volume"] = 
+00027860: 300a 2020 2020 2020 2020 2020 2020 7265  0.            re
+00027870: 7475 726e 2046 616c 7365 2c20 6861 734d  turn False, hasM
+00027880: 696e 696d 756d 566f 6c75 6d65 0a20 2020  inimumVolume.   
+00027890: 2020 2020 2072 6174 696f 203d 2072 6f75       ratio = rou
+000278a0: 6e64 2872 6563 656e 745b 2256 6f6c 756d  nd(recent["Volum
+000278b0: 6522 5d2e 696c 6f63 5b30 5d20 2f20 7265  e"].iloc[0] / re
+000278c0: 6365 6e74 5b22 566f 6c4d 4122 5d2e 696c  cent["VolMA"].il
+000278d0: 6f63 5b30 5d2c 2032 290a 2020 2020 2020  oc[0], 2).      
+000278e0: 2020 7361 7665 4469 6374 5b22 566f 6c75    saveDict["Volu
+000278f0: 6d65 225d 203d 2072 6174 696f 0a20 2020  me"] = ratio.   
+00027900: 2020 2020 2069 6620 7261 7469 6f20 3e3d       if ratio >=
+00027910: 2076 6f6c 756d 6552 6174 696f 2061 6e64   volumeRatio and
+00027920: 2072 6174 696f 2021 3d20 6e70 2e6e 616e   ratio != np.nan
+00027930: 2061 6e64 2028 6e6f 7420 6d61 7468 2e69   and (not math.i
+00027940: 7369 6e66 2872 6174 696f 2929 3a0a 2020  sinf(ratio)):.  
+00027950: 2020 2020 2020 2020 2020 7363 7265 656e            screen
+00027960: 4469 6374 5b22 566f 6c75 6d65 225d 203d  Dict["Volume"] =
+00027970: 2072 6174 696f 0a20 2020 2020 2020 2020   ratio.         
+00027980: 2020 2072 6574 7572 6e20 5472 7565 2c20     return True, 
+00027990: 6861 734d 696e 696d 756d 566f 6c75 6d65  hasMinimumVolume
+000279a0: 0a20 2020 2020 2020 2073 6372 6565 6e44  .        screenD
+000279b0: 6963 745b 2256 6f6c 756d 6522 5d20 3d20  ict["Volume"] = 
+000279c0: 7261 7469 6f0a 2020 2020 2020 2020 7265  ratio.        re
+000279d0: 7475 726e 2046 616c 7365 2c20 6861 734d  turn False, hasM
+000279e0: 696e 696d 756d 566f 6c75 6d65 0a0a 2020  inimumVolume..  
+000279f0: 2020 2320 4669 6e64 2069 6620 7374 6f63    # Find if stoc
+00027a00: 6b20 6973 2076 616c 6964 6174 696e 6720  k is validating 
+00027a10: 766f 6c75 6d65 2073 7072 6561 6420 616e  volume spread an
+00027a20: 616c 7973 6973 0a20 2020 2064 6566 2076  alysis.    def v
+00027a30: 616c 6964 6174 6556 6f6c 756d 6553 7072  alidateVolumeSpr
+00027a40: 6561 6441 6e61 6c79 7369 7328 7365 6c66  eadAnalysis(self
+00027a50: 2c20 6466 2c20 7363 7265 656e 4469 6374  , df, screenDict
+00027a60: 2c20 7361 7665 4469 6374 293a 0a20 2020  , saveDict):.   
+00027a70: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+00027a80: 2020 2020 2020 6966 2064 6620 6973 204e        if df is N
+00027a90: 6f6e 6520 6f72 206c 656e 2864 6629 203d  one or len(df) =
+00027aa0: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
+00027ab0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00027ac0: 650a 2020 2020 2020 2020 2020 2020 6461  e.            da
+00027ad0: 7461 203d 2064 662e 636f 7079 2829 0a20  ta = df.copy(). 
+00027ae0: 2020 2020 2020 2020 2020 2064 6174 6120             data 
+00027af0: 3d20 6461 7461 2e68 6561 6428 3229 0a20  = data.head(2). 
+00027b00: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
+00027b10: 6e28 6461 7461 2920 3c20 323a 0a20 2020  n(data) < 2:.   
+00027b20: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00027b30: 7572 6e20 4661 6c73 650a 2020 2020 2020  urn False.      
+00027b40: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+00027b50: 2020 2020 2020 2020 2020 2023 2043 6865             # Che
+00027b60: 636b 2066 6f72 2070 7265 7669 6f75 7320  ck for previous 
+00027b70: 5245 4420 6361 6e64 6c65 730a 2020 2020  RED candles.    
+00027b80: 2020 2020 2020 2020 2020 2020 2320 4375              # Cu
+00027b90: 7272 656e 7420 6361 6e64 6c65 203d 2030  rrent candle = 0
+00027ba0: 7468 2c20 5072 6576 696f 7573 2043 616e  th, Previous Can
+00027bb0: 646c 6520 3d20 3173 7420 666f 7220 666f  dle = 1st for fo
+00027bc0: 6c6c 6f77 696e 6720 6c6f 6769 630a 2020  llowing logic.  
+00027bd0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00027be0: 2064 6174 612e 696c 6f63 5b31 5d5b 224f   data.iloc[1]["O
+00027bf0: 7065 6e22 5d20 3e3d 2064 6174 612e 696c  pen"] >= data.il
+00027c00: 6f63 5b31 5d5b 2243 6c6f 7365 225d 3a0a  oc[1]["Close"]:.
+00027c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027c20: 2020 2020 7370 7265 6164 3120 3d20 6162      spread1 = ab
+00027c30: 7328 6461 7461 2e69 6c6f 635b 315d 5b22  s(data.iloc[1]["
+00027c40: 4f70 656e 225d 202d 2064 6174 612e 696c  Open"] - data.il
+00027c50: 6f63 5b31 5d5b 2243 6c6f 7365 225d 290a  oc[1]["Close"]).
+00027c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027c70: 2020 2020 7370 7265 6164 3020 3d20 6162      spread0 = ab
+00027c80: 7328 6461 7461 2e69 6c6f 635b 305d 5b22  s(data.iloc[0]["
+00027c90: 4f70 656e 225d 202d 2064 6174 612e 696c  Open"] - data.il
+00027ca0: 6f63 5b30 5d5b 2243 6c6f 7365 225d 290a  oc[0]["Close"]).
 00027cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027cc0: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
-00027cd0: 440a 2020 2020 2020 2020 2020 2020 2020  D.              
-00027ce0: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-00027cf0: 636f 6c6f 7254 6578 742e 4752 4545 4e0a  colorText.GREEN.
-00027d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027d10: 2020 2020 2020 2020 2020 2020 2b20 2253              + "S
-00027d20: 7570 706c 7920 4472 6f75 6768 7422 0a20  upply Drought". 
-00027d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027d40: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
-00027d50: 6f72 5465 7874 2e45 4e44 0a20 2020 2020  orText.END.     
-00027d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027d70: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00027d80: 2020 2020 2020 2020 2020 2020 2073 6176               sav
-00027d90: 6544 6963 745b 2250 6174 7465 726e 225d  eDict["Pattern"]
-00027da0: 203d 2073 6176 6564 5b31 5d20 2b20 2253   = saved[1] + "S
-00027db0: 7570 706c 7920 4472 6f75 6768 7422 0a20  upply Drought". 
-00027dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027dd0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-00027de0: 7565 0a20 2020 2020 2020 2020 2020 2020  ue.             
-00027df0: 2020 2020 2020 2069 6620 280a 2020 2020         if (.    
-00027e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027e10: 2020 2020 7370 7265 6164 3020 3c20 7370      spread0 < sp
-00027e20: 7265 6164 310a 2020 2020 2020 2020 2020  read1.          
-00027e30: 2020 2020 2020 2020 2020 2020 2020 616e                an
-00027e40: 6420 766f 6c30 203e 2076 6f6c 310a 2020  d vol0 > vol1.  
-00027e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027e60: 2020 2020 2020 616e 6420 6461 7461 2e69        and data.i
-00027e70: 6c6f 635b 305d 5b22 566f 6c75 6d65 225d  loc[0]["Volume"]
-00027e80: 203e 2064 6174 612e 696c 6f63 5b30 5d5b   > data.iloc[0][
-00027e90: 2256 6f6c 4d41 225d 0a20 2020 2020 2020  "VolMA"].       
-00027ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027eb0: 2061 6e64 2064 6174 612e 696c 6f63 5b30   and data.iloc[0
-00027ec0: 5d5b 2243 6c6f 7365 225d 203c 3d20 6461  ]["Close"] <= da
-00027ed0: 7461 2e69 6c6f 635b 315d 5b22 4f70 656e  ta.iloc[1]["Open
-00027ee0: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
-00027ef0: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
-00027f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027f10: 2020 7363 7265 656e 4469 6374 5b22 5061    screenDict["Pa
-00027f20: 7474 6572 6e22 5d20 3d20 280a 2020 2020  ttern"] = (.    
-00027f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027f40: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
-00027f50: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-00027f60: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-00027f70: 636f 6c6f 7254 6578 742e 424f 4c44 0a20  colorText.BOLD. 
-00027f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027f90: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
-00027fa0: 6f72 5465 7874 2e47 5245 454e 0a20 2020  orText.GREEN.   
-00027fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027fc0: 2020 2020 2020 2020 202b 2022 4465 6d61           + "Dema
-00027fd0: 6e64 2052 6973 6522 0a20 2020 2020 2020  nd Rise".       
-00027fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027ff0: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
-00028000: 2e45 4e44 0a20 2020 2020 2020 2020 2020  .END.           
-00028010: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00028020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028030: 2020 2020 2020 2073 6176 6544 6963 745b         saveDict[
-00028040: 2250 6174 7465 726e 225d 203d 2073 6176  "Pattern"] = sav
-00028050: 6564 5b31 5d20 2b20 2244 656d 616e 6420  ed[1] + "Demand 
-00028060: 5269 7365 220a 2020 2020 2020 2020 2020  Rise".          
-00028070: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00028080: 7475 726e 2054 7275 650a 2020 2020 2020  turn True.      
-00028090: 2020 2020 2020 6578 6365 7074 2049 6e64        except Ind
-000280a0: 6578 4572 726f 7220 6173 2065 3a20 2320  exError as e: # 
-000280b0: 7072 6167 6d61 3a20 6e6f 2063 6f76 6572  pragma: no cover
-000280c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000280d0: 2073 656c 662e 6465 6661 756c 745f 6c6f   self.default_lo
-000280e0: 6767 6572 2e64 6562 7567 2865 2c20 6578  gger.debug(e, ex
-000280f0: 635f 696e 666f 3d54 7275 6529 0a20 2020  c_info=True).   
-00028100: 2020 2020 2020 2020 2020 2020 2070 6173               pas
-00028110: 730a 2020 2020 2020 2020 2020 2020 7265  s.            re
-00028120: 7475 726e 2046 616c 7365 0a20 2020 2020  turn False.     
-00028130: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-00028140: 696f 6e20 6173 2065 3a20 2023 2070 7261  ion as e:  # pra
-00028150: 676d 613a 206e 6f20 636f 7665 720a 2020  gma: no cover.  
-00028160: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-00028170: 6566 6175 6c74 5f6c 6f67 6765 722e 6465  efault_logger.de
-00028180: 6275 6728 652c 2065 7863 5f69 6e66 6f3d  bug(e, exc_info=
-00028190: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
-000281a0: 2020 7265 7475 726e 2046 616c 7365 0a      return False.
+00027cc0: 2020 2020 6c6f 7765 725f 7769 636b 5f73      lower_wick_s
+00027cd0: 7072 6561 6430 203d 2028 0a20 2020 2020  pread0 = (.     
+00027ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027cf0: 2020 206d 6178 2864 6174 612e 696c 6f63     max(data.iloc
+00027d00: 5b30 5d5b 224f 7065 6e22 5d2c 2064 6174  [0]["Open"], dat
+00027d10: 612e 696c 6f63 5b30 5d5b 2243 6c6f 7365  a.iloc[0]["Close
+00027d20: 225d 290a 2020 2020 2020 2020 2020 2020  "]).            
+00027d30: 2020 2020 2020 2020 2020 2020 2d20 6461              - da
+00027d40: 7461 2e69 6c6f 635b 305d 5b22 4c6f 7722  ta.iloc[0]["Low"
+00027d50: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00027d60: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00027d70: 2020 2020 2020 2020 2020 2020 766f 6c31              vol1
+00027d80: 203d 2064 6174 612e 696c 6f63 5b31 5d5b   = data.iloc[1][
+00027d90: 2256 6f6c 756d 6522 5d0a 2020 2020 2020  "Volume"].      
+00027da0: 2020 2020 2020 2020 2020 2020 2020 766f                vo
+00027db0: 6c30 203d 2064 6174 612e 696c 6f63 5b30  l0 = data.iloc[0
+00027dc0: 5d5b 2256 6f6c 756d 6522 5d0a 2020 2020  ]["Volume"].    
+00027dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027de0: 7361 7665 6420 3d20 7365 6c66 2e66 696e  saved = self.fin
+00027df0: 6443 7572 7265 6e74 5361 7665 6456 616c  dCurrentSavedVal
+00027e00: 7565 2873 6372 6565 6e44 6963 742c 2073  ue(screenDict, s
+00027e10: 6176 6544 6963 742c 2022 5061 7474 6572  aveDict, "Patter
+00027e20: 6e22 290a 2020 2020 2020 2020 2020 2020  n").            
+00027e30: 2020 2020 2020 2020 6966 2028 0a20 2020          if (.   
+00027e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027e50: 2020 2020 2073 7072 6561 6430 203e 2073       spread0 > s
+00027e60: 7072 6561 6431 0a20 2020 2020 2020 2020  pread1.         
+00027e70: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00027e80: 6e64 2076 6f6c 3020 3c20 766f 6c31 0a20  nd vol0 < vol1. 
+00027e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027ea0: 2020 2020 2020 2061 6e64 2064 6174 612e         and data.
+00027eb0: 696c 6f63 5b30 5d5b 2256 6f6c 756d 6522  iloc[0]["Volume"
+00027ec0: 5d20 3c20 6461 7461 2e69 6c6f 635b 305d  ] < data.iloc[0]
+00027ed0: 5b22 566f 6c4d 4122 5d0a 2020 2020 2020  ["VolMA"].      
+00027ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027ef0: 2020 616e 6420 6461 7461 2e69 6c6f 635b    and data.iloc[
+00027f00: 305d 5b22 436c 6f73 6522 5d20 3c3d 2064  0]["Close"] <= d
+00027f10: 6174 612e 696c 6f63 5b31 5d5b 224f 7065  ata.iloc[1]["Ope
+00027f20: 6e22 5d0a 2020 2020 2020 2020 2020 2020  n"].            
+00027f30: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+00027f40: 7370 7265 6164 3020 3c20 6c6f 7765 725f  spread0 < lower_
+00027f50: 7769 636b 5f73 7072 6561 6430 0a20 2020  wick_spread0.   
+00027f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027f70: 2020 2020 2061 6e64 2064 6174 612e 696c       and data.il
+00027f80: 6f63 5b30 5d5b 2256 6f6c 756d 6522 5d20  oc[0]["Volume"] 
+00027f90: 3c3d 2069 6e74 2864 6174 612e 696c 6f63  <= int(data.iloc
+00027fa0: 5b31 5d5b 2256 6f6c 756d 6522 5d20 2a20  [1]["Volume"] * 
+00027fb0: 302e 3735 290a 2020 2020 2020 2020 2020  0.75).          
+00027fc0: 2020 2020 2020 2020 2020 293a 0a20 2020            ):.   
+00027fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027fe0: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
+00027ff0: 2250 6174 7465 726e 225d 203d 2028 0a20  "Pattern"] = (. 
+00028000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028010: 2020 2020 2020 2020 2020 2073 6176 6564             saved
+00028020: 5b30 5d20 0a20 2020 2020 2020 2020 2020  [0] .           
+00028030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028040: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
+00028050: 440a 2020 2020 2020 2020 2020 2020 2020  D.              
+00028060: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+00028070: 636f 6c6f 7254 6578 742e 4752 4545 4e0a  colorText.GREEN.
+00028080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028090: 2020 2020 2020 2020 2020 2020 2b20 2253              + "S
+000280a0: 7570 706c 7920 4472 6f75 6768 7422 0a20  upply Drought". 
+000280b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000280c0: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
+000280d0: 6f72 5465 7874 2e45 4e44 0a20 2020 2020  orText.END.     
+000280e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000280f0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00028100: 2020 2020 2020 2020 2020 2020 2073 6176               sav
+00028110: 6544 6963 745b 2250 6174 7465 726e 225d  eDict["Pattern"]
+00028120: 203d 2073 6176 6564 5b31 5d20 2b20 2253   = saved[1] + "S
+00028130: 7570 706c 7920 4472 6f75 6768 7422 0a20  upply Drought". 
+00028140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028150: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
+00028160: 7565 0a20 2020 2020 2020 2020 2020 2020  ue.             
+00028170: 2020 2020 2020 2069 6620 280a 2020 2020         if (.    
+00028180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028190: 2020 2020 7370 7265 6164 3020 3c20 7370      spread0 < sp
+000281a0: 7265 6164 310a 2020 2020 2020 2020 2020  read1.          
+000281b0: 2020 2020 2020 2020 2020 2020 2020 616e                an
+000281c0: 6420 766f 6c30 203e 2076 6f6c 310a 2020  d vol0 > vol1.  
+000281d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000281e0: 2020 2020 2020 616e 6420 6461 7461 2e69        and data.i
+000281f0: 6c6f 635b 305d 5b22 566f 6c75 6d65 225d  loc[0]["Volume"]
+00028200: 203e 2064 6174 612e 696c 6f63 5b30 5d5b   > data.iloc[0][
+00028210: 2256 6f6c 4d41 225d 0a20 2020 2020 2020  "VolMA"].       
+00028220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028230: 2061 6e64 2064 6174 612e 696c 6f63 5b30   and data.iloc[0
+00028240: 5d5b 2243 6c6f 7365 225d 203c 3d20 6461  ]["Close"] <= da
+00028250: 7461 2e69 6c6f 635b 315d 5b22 4f70 656e  ta.iloc[1]["Open
+00028260: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
+00028270: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
+00028280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028290: 2020 7363 7265 656e 4469 6374 5b22 5061    screenDict["Pa
+000282a0: 7474 6572 6e22 5d20 3d20 280a 2020 2020  ttern"] = (.    
+000282b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000282c0: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
+000282d0: 200a 2020 2020 2020 2020 2020 2020 2020   .              
+000282e0: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+000282f0: 636f 6c6f 7254 6578 742e 424f 4c44 0a20  colorText.BOLD. 
+00028300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028310: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
+00028320: 6f72 5465 7874 2e47 5245 454e 0a20 2020  orText.GREEN.   
+00028330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028340: 2020 2020 2020 2020 202b 2022 4465 6d61           + "Dema
+00028350: 6e64 2052 6973 6522 0a20 2020 2020 2020  nd Rise".       
+00028360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028370: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
+00028380: 2e45 4e44 0a20 2020 2020 2020 2020 2020  .END.           
+00028390: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+000283a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000283b0: 2020 2020 2020 2073 6176 6544 6963 745b         saveDict[
+000283c0: 2250 6174 7465 726e 225d 203d 2073 6176  "Pattern"] = sav
+000283d0: 6564 5b31 5d20 2b20 2244 656d 616e 6420  ed[1] + "Demand 
+000283e0: 5269 7365 220a 2020 2020 2020 2020 2020  Rise".          
+000283f0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00028400: 7475 726e 2054 7275 650a 2020 2020 2020  turn True.      
+00028410: 2020 2020 2020 6578 6365 7074 2049 6e64        except Ind
+00028420: 6578 4572 726f 7220 6173 2065 3a20 2320  exError as e: # 
+00028430: 7072 6167 6d61 3a20 6e6f 2063 6f76 6572  pragma: no cover
+00028440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00028450: 2073 656c 662e 6465 6661 756c 745f 6c6f   self.default_lo
+00028460: 6767 6572 2e64 6562 7567 2865 2c20 6578  gger.debug(e, ex
+00028470: 635f 696e 666f 3d54 7275 6529 0a20 2020  c_info=True).   
+00028480: 2020 2020 2020 2020 2020 2020 2070 6173               pas
+00028490: 730a 2020 2020 2020 2020 2020 2020 7265  s.            re
+000284a0: 7475 726e 2046 616c 7365 0a20 2020 2020  turn False.     
+000284b0: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
+000284c0: 696f 6e20 6173 2065 3a20 2023 2070 7261  ion as e:  # pra
+000284d0: 676d 613a 206e 6f20 636f 7665 720a 2020  gma: no cover.  
+000284e0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+000284f0: 6566 6175 6c74 5f6c 6f67 6765 722e 6465  efault_logger.de
+00028500: 6275 6728 652c 2065 7863 5f69 6e66 6f3d  bug(e, exc_info=
+00028510: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
+00028520: 2020 7265 7475 726e 2046 616c 7365 0a      return False.
```

### Comparing `pkscreener-0.45.20240602.429/pkscreener/classes/StockScreener.py` & `pkscreener-0.45.20240602.430/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.429/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.45.20240602.430/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.429/pkscreener/classes/Utility.py` & `pkscreener-0.45.20240602.430/pkscreener/classes/Utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -1153,15 +1153,15 @@
                         isIntraday = isIntraday,
                         forceRedownload=forceRedownload
                     )
                 
         return stockDict,stockDataLoaded
 
     # Save screened results to excel
-    def promptSaveResults(sheetName,df, defaultAnswer=None):
+    def promptSaveResults(sheetName,df, defaultAnswer=None,pastDate=None):
         """
         Tries to save the dataframe output into an excel file.
 
         It will first try to save to the current-working-directory/results/
 
         If it fails to save, it will then try to save to Desktop and then eventually into
         a temporary directory.
@@ -1178,16 +1178,18 @@
                 ).upper()
             else:
                 response = defaultAnswer
         except ValueError as e:  # pragma: no cover
             default_logger().debug(e, exc_info=True)
             response = "Y"
         if response is not None and response.upper() != "N":
+            pastDateString = f"{pastDate}_to_" if pastDate is not None else ""
             filename = (
                 "PKScreener-result_"
+                + pastDateString
                 + PKDateUtilities.currentDateTime().strftime("%d-%m-%y_%H.%M.%S")
                 + ".xlsx"
             )
             desktop = os.path.expanduser("~/Desktop")
             # # the above is valid on Windows (after 7) but if you want it in os normalized form:
             desktop = os.path.normpath(os.path.expanduser("~/Desktop"))
             filePath = ""
```

### Comparing `pkscreener-0.45.20240602.429/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.45.20240602.430/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.429/pkscreener/classes/keys.py` & `pkscreener-0.45.20240602.430/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.429/pkscreener/courbd.ttf` & `pkscreener-0.45.20240602.430/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.429/pkscreener/globals.py` & `pkscreener-0.45.20240602.430/pkscreener/globals.py`

 * *Files 2% similar despite different names*

```diff
@@ -400,15 +400,15 @@
         if userPassedArgs is None or userPassedArgs.options is None:
             selectedMenu = m0.find(menuOption)
             m1.renderForMenu(selectedMenu=selectedMenu)
             periodOption = input(
                     colorText.BOLD + colorText.FAIL + "[+] Select option: "
                 ) or ('L' if configManager.period == '1y' else 'S')
             OutputControls().printOutput(colorText.END, end="")
-            if periodOption is None or periodOption.upper() not in ["L","S"]:
+            if periodOption is None or periodOption.upper() not in ["L","S","B"]:
                 return
             Utility.tools.clearScreen(forceTop=True)
             if periodOption.upper() in ["L","S"]:
                 selectedMenu = m1.find(periodOption)
                 m2.renderForMenu(selectedMenu=selectedMenu)
                 durationOption = input(
                         colorText.BOLD + colorText.FAIL + "[+] Select option: "
@@ -422,14 +422,27 @@
                     periodDurations = selectedMenu.menuText.split("(")[1].split(")")[0].split(", ")
                     configManager.period = periodDurations[0]
                     configManager.duration = periodDurations[1]
                     configManager.setConfig(ConfigManager.parser, default=True, showFileCreatedText=False)
                 elif durationOption.upper() in ["5"]:
                     configManager.setConfig(ConfigManager.parser, default=False, showFileCreatedText=True)
                 return
+            elif periodOption.upper() in ["B"]:
+                backtestDaysAgo = input(
+                    colorText.BOLD + colorText.FAIL + "[+] Enter no. of days/candles in the past as starting candle for which you'd like to run the scans (e.g. 10 for 10 candles ago or 0 for today):"
+                ) or ('22' if configManager.period == '1y' else '15')
+                OutputControls().printOutput(colorText.END, end="")
+                launcher = f'"{sys.argv[0]}"' if " " in sys.argv[0] else sys.argv[0]
+                requestingUser = f" -u {userPassedArgs.user}" if userPassedArgs.user is not None else ""
+                enableLog = f" -l" if userPassedArgs.log else ""
+                launcher = f"python3.11 {launcher}" if (launcher.endswith(".py\"") or launcher.endswith(".py")) else launcher
+                OutputControls().printOutput(f"{colorText.GREEN}Launching PKScreener in quick backtest mode. If it does not launch, please try with the following:{colorText.END}\n{colorText.FAIL}{launcher} --backtestdaysago {int(backtestDaysAgo)}{requestingUser}{enableLog}{colorText.END}\n{colorText.WARN}Press Ctrl + C to exit quick backtest mode.{colorText.END}")
+                sleep(2)
+                os.system(f"{launcher} --systemlaunched -a Y -e --backtestdaysago {int(backtestDaysAgo)}{requestingUser}{enableLog}")
+                sys.exit(0)
         elif userPassedArgs is not None and userPassedArgs.options is not None:
             options = userPassedArgs.options.split(":")
             selectedMenu = m0.find(options[0])
             m1.renderForMenu(selectedMenu=selectedMenu, asList=True)
             selectedMenu = m1.find(options[1])
             m2.renderForMenu(selectedMenu=selectedMenu)
             if options[2] in ["1","2","3","4"]:
@@ -467,22 +480,24 @@
         + colorText.FAIL
         + "[+] You chose: "
         + f" (Piped Scan Mode) [{userPassedArgs.pipedmenus}]"
         + colorText.END
     )
     m0.renderForMenu(selectedMenu=None)
     try:
+        needsCalc = userPassedArgs is not None and userPassedArgs.backtestdaysago is not None
+        pastDate = f"[+] [ Running in Quick Backtest Mode for {colorText.WARN}{PKDateUtilities.nthPastTradingDateStringFromFutureDate(int(userPassedArgs.backtestdaysago) if needsCalc else 0)}{colorText.END} ]\n" if needsCalc else ""
         if menuOption is None:
             if "PKDevTools_Default_Log_Level" in os.environ.keys():
                 from PKDevTools.classes import Archiver
                 log_file_path = os.path.join(Archiver.get_user_outputs_dir(), "pkscreener-logs.txt")
                 OutputControls().printOutput(colorText.FAIL + "\n    [+] Logs will be written to:"+colorText.END)
                 OutputControls().printOutput(colorText.GREEN + f"    [+] {log_file_path}"+colorText.END)
                 OutputControls().printOutput(colorText.FAIL + "    [+] If you need to share,run through the menus that are causing problems. At the end, open this folder, zip the log file to share at https://github.com/pkjmesra/PKScreener/issues .\n" + colorText.END)
-            menuOption = input(colorText.BOLD + colorText.FAIL + "[+] Select option: ")
+            menuOption = input(colorText.BOLD + colorText.FAIL + f"{pastDate}[+] Select option: ")
             OutputControls().printOutput(colorText.END, end="")
         if menuOption == "" or menuOption is None:
             menuOption = "X"
         menuOption = menuOption.upper()
         selectedMenu = m0.find(menuOption)
         if selectedMenu is not None:
             if selectedMenu.menuKey == "Z":
@@ -526,17 +541,19 @@
         + (f" (Piped Scan Mode) [{userPassedArgs.pipedmenus}]" if (userPassedArgs is not None and userPassedArgs.pipedmenus is not None) else "")
         + colorText.END
     )
     if indexOption is None:
         selectedMenu = m0.find(menuOption)
         m1.renderForMenu(selectedMenu=selectedMenu, skip=skip)
     try:
+        needsCalc = userPassedArgs is not None and userPassedArgs.backtestdaysago is not None
+        pastDate = f"[+] [ Running in Quick Backtest Mode for {colorText.WARN}{PKDateUtilities.nthPastTradingDateStringFromFutureDate(int(userPassedArgs.backtestdaysago) if needsCalc else 0)}{colorText.END} ]\n" if needsCalc else ""
         if indexOption is None:
             indexOption = input(
-                colorText.BOLD + colorText.FAIL + "[+] Select option: "
+                colorText.BOLD + colorText.FAIL + f"{pastDate}[+] Select option: "
             )
             OutputControls().printOutput(colorText.END, end="")
         if indexOption == "" or indexOption is None:
             indexOption = int(configManager.defaultIndex)
         # elif indexOption == 'W' or indexOption == 'w' or indexOption == 'N' or indexOption == 'n' or indexOption == 'E' or indexOption == 'e':
         elif not str(indexOption).isnumeric():
             indexOption = indexOption.upper()
@@ -584,18 +601,20 @@
                 + level1_X_MenuDict[selectedChoice["1"]].strip()
                 + (f" (Piped Scan Mode) [{userPassedArgs.pipedmenus}]" if (userPassedArgs is not None and userPassedArgs.pipedmenus is not None) else "")
                 + colorText.END
             )
             selectedMenu = m1.find(indexOption)
             m2.renderForMenu(selectedMenu=selectedMenu, skip=skip)
     try:
+        needsCalc = userPassedArgs is not None and userPassedArgs.backtestdaysago is not None
+        pastDate = f"[+] [ Running in Quick Backtest Mode for {colorText.WARN}{PKDateUtilities.nthPastTradingDateStringFromFutureDate(int(userPassedArgs.backtestdaysago) if needsCalc else 0)}{colorText.END} ]\n" if needsCalc else ""
         if indexOption is not None and indexOption != "W":
             if executeOption is None:
                 executeOption = input(
-                    colorText.BOLD + colorText.FAIL + "[+] Select option: "
+                    colorText.BOLD + colorText.FAIL + f"{pastDate}[+] Select option: "
                 ) or "9"
                 OutputControls().printOutput(colorText.END, end="")
             if executeOption == "":
                 executeOption = 1
             if not str(executeOption).isnumeric():
                 executeOption = executeOption.upper()
             else:
@@ -806,40 +825,44 @@
         selPredefinedOption = None
         if len(options) >= 3:
             predefinedOption = str(options[1])
             selPredefinedOption = str(options[2])
         updateMenuChoiceHierarchy()
         selectedMenu = m0.find(menuOption)
         m1.renderForMenu(selectedMenu)
+        needsCalc = userPassedArgs is not None and userPassedArgs.backtestdaysago is not None
+        pastDate = f"[+] [ Running in Quick Backtest Mode for {colorText.WARN}{PKDateUtilities.nthPastTradingDateStringFromFutureDate(int(userPassedArgs.backtestdaysago) if needsCalc else 0)}{colorText.END} ]\n" if needsCalc else ""
         if predefinedOption is None:
-            predefinedOption = input(colorText.BOLD + colorText.FAIL + "[+] Select option: ") or "1"
+            predefinedOption = input(colorText.BOLD + colorText.FAIL + f"{pastDate}[+] Select option: ") or "1"
         OutputControls().printOutput(colorText.END, end="")
         if predefinedOption not in ["1","2","3"]:
             return None, None
         if predefinedOption == "1":
             updateMenuChoiceHierarchy()
             selectedMenu = m1.find(predefinedOption)
             m2.renderForMenu(selectedMenu=selectedMenu)
             if selPredefinedOption is None:
-                selPredefinedOption = input(colorText.BOLD + colorText.FAIL + "[+] Select option: ") or "1"
+                selPredefinedOption = input(colorText.BOLD + colorText.FAIL + f"{pastDate}[+] Select option: ") or "1"
             OutputControls().printOutput(colorText.END, end="")
             if selPredefinedOption in PREDEFINED_SCAN_MENU_KEYS:
                 scannerOption = PIPED_SCANNERS[selPredefinedOption]
                 updateMenuChoiceHierarchy()
                 if userPassedArgs.pipedmenus is not None:
                     chosenOptions = scannerOption.split("-o ")[1]
                     userPassedArgs.options = chosenOptions.replace("'","")
                     return addOrRunPipedMenus()
                 launcher = f'"{sys.argv[0]}"' if " " in sys.argv[0] else sys.argv[0]
                 launcher = f"python3.11 {launcher}" if (launcher.endswith(".py\"") or launcher.endswith(".py")) else launcher
                 scannerOptionQuoted = scannerOption.replace("'",'"')
                 requestingUser = f" -u {userPassedArgs.user}" if userPassedArgs.user is not None else ""
-                OutputControls().printOutput(f"{colorText.GREEN}Launching PKScreener with piped scanners. If it does not launch, please try with the following:{colorText.END}\n{colorText.FAIL}{launcher} {scannerOptionQuoted}{requestingUser}{colorText.END}")
+                enableLog = f" -l" if userPassedArgs.log else ""
+                backtestParam = f" --backtestdaysago {userPassedArgs.backtestdaysago}" if userPassedArgs.backtestdaysago else ""
+                OutputControls().printOutput(f"{colorText.GREEN}Launching PKScreener with piped scanners. If it does not launch, please try with the following:{colorText.END}\n{colorText.FAIL}{launcher} {scannerOptionQuoted}{requestingUser}{enableLog}{backtestParam}{colorText.END}")
                 sleep(2)
-                os.system(f"{launcher} {scannerOptionQuoted}{requestingUser}")
+                os.system(f"{launcher} {scannerOptionQuoted}{requestingUser}{enableLog}{backtestParam}")
                 OutputControls().printOutput(
                         colorText.GREEN
                         + f"[+] Finished running all piped scanners!"
                         + colorText.END
                     )
                 if defaultAnswer is None:
                     input("Press <Enter> to exit...")
@@ -1587,16 +1610,17 @@
                 df["LastTradeDate"], df["LastTradeTime"] = getLatestTradeDateTime(stockDictPrimary)
                 gClient.df_to_sheet(df=df,sheetName=runOption)
                 OutputControls().printOutput(f"{colorText.GREEN} => Done in {round(time.time()-begin,2)}s{colorText.END}")
     except:
         pass
     if "RUNNER" not in os.environ.keys() and not testing and (userPassedArgs is None or (userPassedArgs is not None and userPassedArgs.user is None and (userPassedArgs.answerdefault is None or userPassedArgs.systemlaunched))):
         prevOutput_results = saveResults.index if (saveResults is not None and not saveResults.empty) else []
-        hasFoundStocks = len(prevOutput_results) > 0 and (("|" not in userPassedArgs.options) if (userPassedArgs is not None and userPassedArgs.options is not None) else True)
-        if hasFoundStocks or configManager.showPinnedMenuEvenForNoResult:
+        isNotPiped = (("|" not in userPassedArgs.options) if (userPassedArgs is not None and userPassedArgs.options is not None) else True)
+        hasFoundStocks = len(prevOutput_results) > 0 and isNotPiped
+        if hasFoundStocks or (configManager.showPinnedMenuEvenForNoResult and isNotPiped):
             monitorOption = userPassedArgs.systemlaunched if (userPassedArgs is not None and isinstance(userPassedArgs.systemlaunched,str) and userPassedArgs.systemlaunched is not None) else (userPassedArgs.options if (userPassedArgs is not None and userPassedArgs.options is not None) else "")
             if len(monitorOption) == 0:
                 for choice in selectedChoice.keys():
                     monitorOption = (f"{monitorOption}:" if len(monitorOption) > 0  else '') + f"{selectedChoice[choice]}"
             m0.renderPinnedMenu(substitutes=[monitorOption,len(prevOutput_results)])
             pinOption = input(
                     colorText.BOLD + colorText.FAIL + "[+] Select option: "
@@ -1740,17 +1764,19 @@
         shouldAddMoreIntoPipe = input(colorText.FAIL + "[+] Select [Y/N] (Default:N): " + colorText.END) or 'n'
     if shouldAddMoreIntoPipe.lower() != 'y':
         launcher = f'"{sys.argv[0]}"' if " " in sys.argv[0] else sys.argv[0]
         launcher = f"python3.11 {launcher}" if (launcher.endswith(".py\"") or launcher.endswith(".py")) else launcher
         monitorOption = f'"{userPassedArgs.pipedmenus}"'
         scannerOptionQuoted = monitorOption.replace("'",'"').replace(":>",":D:D:D:>").replace("::",":")
         requestingUser = f" -u {userPassedArgs.user}" if userPassedArgs.user is not None else ""
-        OutputControls().printOutput(f"{colorText.GREEN}Launching PKScreener with piped scanners. If it does not launch, please try with the following:{colorText.END}\n{colorText.FAIL}{launcher} -a Y -e -o {scannerOptionQuoted}{requestingUser}{colorText.END}")
+        enableLog = f" -l" if userPassedArgs.log else ""
+        backtestParam = f" --backtestdaysago {userPassedArgs.backtestdaysago}" if userPassedArgs.backtestdaysago else ""
+        OutputControls().printOutput(f"{colorText.GREEN}Launching PKScreener with piped scanners. If it does not launch, please try with the following:{colorText.END}\n{colorText.FAIL}{launcher} -a Y -e -o {scannerOptionQuoted}{requestingUser}{enableLog}{backtestParam}{colorText.END}")
         sleep(2)
-        os.system(f"{launcher} --systemlaunched -a Y -e -o {scannerOptionQuoted}{requestingUser}")
+        os.system(f"{launcher} --systemlaunched -a Y -e -o {scannerOptionQuoted}{requestingUser}{enableLog}{backtestParam}")
         userPassedArgs.pipedmenus = None
         OutputControls().printOutput(
                 colorText.GREEN
                 + f"[+] Finished running all piped scanners!"
                 + colorText.END
             )
         if defaultAnswer is None:
@@ -2027,27 +2053,29 @@
                 + f'>{level4_X_ChartPattern_MASignalMenuDict[selectedChoice["4"]].strip()}'
             )
         elif selectedChoice["2"] == "21":
             menuChoiceHierarchy = (
                 menuChoiceHierarchy
                 + f'>{level3_X_PopularStocks_MenuDict[selectedChoice["3"]].strip()}'
             )
-        intraday = "(Intraday)" if (userPassedArgs is not None and userPassedArgs.intraday) or configManager.isIntradayConfig() else ""
+        intraday = "(Intraday)" if ("Intraday" not in menuChoiceHierarchy and (userPassedArgs is not None and userPassedArgs.intraday) or configManager.isIntradayConfig()) else ""
         menuChoiceHierarchy = f"{menuChoiceHierarchy}{intraday}"
         global nValueForMenu
         menuChoiceHierarchy = menuChoiceHierarchy.replace("N-",f"{nValueForMenu}-")
     except:
         pass
     Utility.tools.clearScreen(forceTop=True)
+    needsCalc = userPassedArgs is not None and userPassedArgs.backtestdaysago is not None
+    pastDate = f"[ {PKDateUtilities.nthPastTradingDateStringFromFutureDate(int(userPassedArgs.backtestdaysago) if needsCalc else 0)} ]" if needsCalc else ""
     OutputControls().printOutput(
         colorText.BOLD
         + colorText.FAIL
         + "[+] You chose: "
         + menuChoiceHierarchy
-        + (f" (Piped Scan Mode) [{userPassedArgs.pipedmenus}]" if (userPassedArgs is not None and userPassedArgs.pipedmenus is not None) else "")
+        + (f" (Piped Scan Mode) [{userPassedArgs.pipedmenus}] {pastDate}" if (userPassedArgs is not None and userPassedArgs.pipedmenus is not None) else "")
         + colorText.END
     )
     default_logger().info(menuChoiceHierarchy)
     return menuChoiceHierarchy
 
 def printNotifySaveScreenedResults(
     screenResults, saveResults, selectedChoice, menuChoiceHierarchy, testing, user=None
@@ -2165,34 +2193,39 @@
                 if saveResultsTrimmed is not None and len(saveResultsTrimmed) > 0:
                     markdown_results = colorText.miniTabulator().tabulate(
                         saveResultsTrimmed,
                         headers="keys",
                         tablefmt=colorText.No_Pad_GridFormat,
                         maxcolwidths=Utility.tools.getMaxColumnWidths(saveResultsTrimmed)
                     ).encode("utf-8").decode(STD_ENCODING)
-                    caption_df = saveResultsTrimmed[['LTP','%Chng','Volume']].head(5)
-                    caption_df.loc[:, "LTP"] = caption_df.loc[:, "LTP"].apply(
-                        lambda x: str(int(round(float(x),0)))
-                    )
-                    caption_df.loc[:, "%Chng"] = caption_df.loc[:, "%Chng"].apply(
-                        lambda x: f'{int(round(float(x.replace("%","")),0))}%'
-                    )
-                    caption_df.loc[:, "Volume"] = caption_df.loc[:, "Volume"].apply(
-                        lambda x: f'{int(round(float(x.replace("x","")),0))}x' if (len(x.replace("x","").strip()) > 0 and not pd.isna(float(x.replace("x","")))) else ''
-                    )
-                    caption_df.rename(columns={"%Chng": "Ch%","Volume":"Vol"}, inplace=True)
+                    try:
+                        caption_df = saveResultsTrimmed[['LTP','%Chng','Volume']].head(5)
+                        caption_df.loc[:, "LTP"] = caption_df.loc[:, "LTP"].apply(
+                            lambda x: str(int(round(float(x),0)))
+                        )
+                        caption_df.loc[:, "%Chng"] = caption_df.loc[:, "%Chng"].apply(
+                            lambda x: f'{int(round(float(x.replace("%","")),0))}%'
+                        )
+                        caption_df.loc[:, "Volume"] = caption_df.loc[:, "Volume"].apply(
+                            lambda x: f'{int(round(float(x.replace("x","")),0))}x' if (len(x.replace("x","").strip()) > 0 and not pd.isna(float(x.replace("x","")))) else ''
+                        )
+                        caption_df.rename(columns={"%Chng": "Ch%","Volume":"Vol"}, inplace=True)
+                    except:
+                        cols = [list(saveResultsTrimmed.columns)[0]]
+                        cols.extend(list(saveResultsTrimmed.columns[5:]))
+                        caption_df = saveResultsTrimmed[cols].head(2)
                     for col in caption_df.columns:
                         caption_df[col] = caption_df[col].astype(str)
                     caption_results = colorText.miniTabulator().tabulate(
                         caption_df,
                         headers="keys",
                         tablefmt=colorText.No_Pad_GridFormat,
                         maxcolwidths=[None,None,4,3]
                     ).encode("utf-8").decode(STD_ENCODING).replace("-K-----S-----C-----R","-K-----S----C---R").replace("%  ","% ").replace("=K=====S=====C=====R","=K=====S====C===R").replace("Vol  |","Vol|").replace("x  ","x")
-                    caption_results = caption_results.replace("-E-----N-----E-----R","-E-----N----E---R").replace("=E=====N=====E=====R","=E=====N====E===R")
+                    caption_results = Utility.tools.removeAllColorStyles(caption_results.replace("-E-----N-----E-----R","-E-----N----E---R").replace("=E=====N=====E=====R","=E=====N====E===R"))
                     caption = f"{caption}.Open attached image for more. Samples:<pre>{caption_results}</pre>{elapsed_text}{pipedTitle}" #<i>Author is <u><b>NOT</b> a SEBI registered financial advisor</u> and MUST NOT be deemed as one.</i>"
                 if not testing: # and not userPassedArgs.runintradayanalysis:
                     sendQuickScanResult(
                         f"{reportTitle}{menuChoiceHierarchy}",
                         user,
                         tabulated_results,
                         markdown_results,
@@ -2237,18 +2270,20 @@
                             # traceback.print_exc()
                     else:
                         tabulateBacktestResults(saveResults)
             else:
                 tabulateBacktestResults(saveResults)
         else:
             tabulateBacktestResults(saveResults)
+            needsCalc = userPassedArgs is not None and userPassedArgs.backtestdaysago is not None
+            pastDate = PKDateUtilities.nthPastTradingDateStringFromFutureDate(int(userPassedArgs.backtestdaysago) if needsCalc else 0)
             OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.GREEN
-                + f"[+] Found {len(screenResults) if screenResults is not None else 0} Stocks in {str('{:.2f}'.format(elapsed_time))} sec. Showing only stocks that met the filter criteria in the filters section of user configuration{(' with portfolio returns:' + summaryReturns) if (len(summaryReturns) > 0) else ''}"
+                + f"[+] Found {len(screenResults) if screenResults is not None else 0} Stocks in {str('{:.2f}'.format(elapsed_time))} sec for {pastDate}. Showing only stocks that met the filter criteria in the filters section of user configuration{(' with portfolio returns:' + summaryReturns) if (len(summaryReturns) > 0) else ''}"
                 + colorText.END
             )
     elif user is not None:
         sendMessageToTelegramChannel(
             message=f"No scan results found for {menuChoiceHierarchy}", user=user
         )
     if not testing:
@@ -2724,17 +2759,18 @@
 ):
     global userPassedArgs, elapsed_time, selectedChoice
     if user is None and userPassedArgs.user is not None:
         user = userPassedArgs.user
     caption = f'<b>{menuChoiceHierarchy.split(">")[-1]}</b>'
     if screenResults is not None and len(screenResults) >= 1:
         choices = PKScanRunner.getFormattedChoices(userPassedArgs,selectedChoice)
+        needsCalc = userPassedArgs is not None and userPassedArgs.backtestdaysago is not None
+        pastDate = PKDateUtilities.nthPastTradingDateStringFromFutureDate(int(userPassedArgs.backtestdaysago) if needsCalc else 0) if needsCalc else None
         filename = Utility.tools.promptSaveResults(choices,
-            saveResults, defaultAnswer=defaultAnswer
-        )
+            saveResults, defaultAnswer=defaultAnswer,pastDate=pastDate)
         # if filename is not None:
         #     sendMessageToTelegramChannel(
         #         document_filePath=filename, caption=caption, user=user
         #     )
         OutputControls().printOutput(
             colorText.BOLD
             + colorText.WARN
@@ -2743,18 +2779,20 @@
         )
         # try:
         #     if filename is not None:
         #         os.remove(filename)
         # except Exception as e:  # pragma: no cover
         #     default_logger().debug(e, exc_info=True)
     if userPassedArgs.monitor is None:
+        needsCalc = userPassedArgs is not None and userPassedArgs.backtestdaysago is not None
+        pastDate = PKDateUtilities.nthPastTradingDateStringFromFutureDate(int(userPassedArgs.backtestdaysago) if needsCalc else 0)
         OutputControls().printOutput(
             colorText.BOLD
             + colorText.GREEN
-            + f"[+] Screening Completed. Found {len(screenResults) if screenResults is not None else 0} results in {round(elapsed_time,2)} sec.! Press Enter to Continue.."
+            + f"[+] Screening Completed. Found {len(screenResults) if screenResults is not None else 0} results in {round(elapsed_time,2)} sec. for {pastDate}! Press Enter to Continue.."
             + colorText.END
             , enableMultipleLineOutput=True
         )
         if defaultAnswer is None:
             input("Press <Enter> to continue...")
 
 def sendGlobalMarketBarometer(userArgs=None):
@@ -2793,24 +2831,24 @@
             default_logger().debug(e, exc_info=True)
     else:
         message = ""
     if photo_filePath is not None:
         try:
             if caption is not None:
                 caption = f"{caption.replace('&','n')}"
-            send_photo(photo_filePath, caption, userID=user)
+            send_photo(photo_filePath, (caption if len(caption) <=1024 else ""), userID=user)
             # Breather for the telegram API to be able to send the heavy photo
             sleep(2)
         except Exception as e:  # pragma: no cover
             default_logger().debug(e, exc_info=True)
     if document_filePath is not None:
         try:
             if caption is not None:
                 caption = f"{caption.replace('&','n')}"
-            send_document(document_filePath, caption, userID=user)
+            send_document(document_filePath, (caption if len(caption) <=1024 else ""), userID=user)
             # Breather for the telegram API to be able to send the document
             sleep(2)
         except Exception as e:  # pragma: no cover
             default_logger().debug(e, exc_info=True)
     if user is not None:
         channel_userID="-1001785195297"
         if user != channel_userID:
```

### Comparing `pkscreener-0.45.20240602.429/pkscreener/pkscreener.ini` & `pkscreener-0.45.20240602.430/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.429/pkscreener/pkscreenerbot.py` & `pkscreener-0.45.20240602.430/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.429/pkscreener/pkscreenercli.py` & `pkscreener-0.45.20240602.430/pkscreener/pkscreenercli.py`

 * *Files 0% similar despite different names*

```diff
@@ -451,14 +451,15 @@
         else:
             global results, resultStocks, plainResults, dbTimestamp, elapsed_time, start_time
             monitorOption_org = ""
             # args.monitor = configManager.defaultMonitorOptions
             if args.monitor:
                 configManager.getConfig(ConfigManager.parser)
                 args.answerdefault = args.answerdefault or 'Y'
+                MarketMonitor().hiddenColumns = configManager.alwaysHiddenDisplayColumns
                 if MarketMonitor().monitorIndex == 0:
                     dbTimestamp = PKDateUtilities.currentDateTime().strftime("%H:%M:%S")
                     elapsed_time = 0
                     if start_time is None:
                         start_time = time.time()
                     else:
                         elapsed_time = round(time.time() - start_time,2)
@@ -564,14 +565,16 @@
                     # We need to switch to daily scan
         args.intraday = None
         configManager.toggleConfig(candleDuration='1d', clearCache=False)
     return monitorOption
 
 
 def pipeResults(prevOutput,args):
+    if args is None or args.options is None:
+        return False
     nextOnes = args.options.split(">")
     hasFoundStocks = False
     if len(nextOnes) > 1:
         monitorOption = nextOnes[1]
         if len(monitorOption) == 0:
             return False
         lastComponent = monitorOption.split(":")[-1]
```

### Comparing `pkscreener-0.45.20240602.429/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.45.20240602.430/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.45.20240602.429
+Version: 0.45.20240602.430
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240602.429.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240602.430.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -274,19 +274,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.428/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.429/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.428/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.429/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.428/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.429/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240602.429/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.45.20240602.430/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.429/setup.py` & `pkscreener-0.45.20240602.430/setup.py`

 * *Files identical despite different names*

