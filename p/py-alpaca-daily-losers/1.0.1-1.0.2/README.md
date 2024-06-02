# Comparing `tmp/py_alpaca_daily_losers-1.0.1.tar.gz` & `tmp/py_alpaca_daily_losers-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_alpaca_daily_losers-1.0.1.tar", max compression
+gzip compressed data, was "py_alpaca_daily_losers-1.0.2.tar", max compression
```

## Comparing `py_alpaca_daily_losers-1.0.1.tar` & `py_alpaca_daily_losers-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     2267 2024-06-01 22:06:14.046692 py_alpaca_daily_losers-1.0.1/README.md
--rw-r--r--   0        0        0     1212 2024-06-01 23:02:16.236042 py_alpaca_daily_losers-1.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.1/src/alpaca_daily_losers/__init__.py
--rw-r--r--   0        0        0      902 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.1/src/alpaca_daily_losers/calc.py
--rw-r--r--   0        0        0    19678 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.1/src/alpaca_daily_losers/daily_losers.py
--rw-r--r--   0        0        0      460 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.1/src/alpaca_daily_losers/global_functions.py
--rw-r--r--   0        0        0     2563 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.1/src/alpaca_daily_losers/openai.py
--rw-r--r--   0        0        0     4550 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.1/src/alpaca_daily_losers/requests.py
--rw-r--r--   0        0        0     1896 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.1/src/alpaca_daily_losers/slack.py
--rw-r--r--   0        0        0     7069 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.1/src/alpaca_daily_losers/yahoo.py
--rw-r--r--   0        0        0     2981 1970-01-01 00:00:00.000000 py_alpaca_daily_losers-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2267 2024-06-01 22:06:14.046692 py_alpaca_daily_losers-1.0.2/README.md
+-rw-r--r--   0        0        0     1212 2024-06-02 22:42:06.706725 py_alpaca_daily_losers-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.2/src/alpaca_daily_losers/__init__.py
+-rw-r--r--   0        0        0      902 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.2/src/alpaca_daily_losers/calc.py
+-rw-r--r--   0        0        0    19743 2024-06-02 22:42:06.706725 py_alpaca_daily_losers-1.0.2/src/alpaca_daily_losers/daily_losers.py
+-rw-r--r--   0        0        0      460 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.2/src/alpaca_daily_losers/global_functions.py
+-rw-r--r--   0        0        0     2563 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.2/src/alpaca_daily_losers/openai.py
+-rw-r--r--   0        0        0     4550 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.2/src/alpaca_daily_losers/requests.py
+-rw-r--r--   0        0        0     1896 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.2/src/alpaca_daily_losers/slack.py
+-rw-r--r--   0        0        0     7069 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.2/src/alpaca_daily_losers/yahoo.py
+-rw-r--r--   0        0        0     2981 1970-01-01 00:00:00.000000 py_alpaca_daily_losers-1.0.2/PKG-INFO
```

### Comparing `py_alpaca_daily_losers-1.0.1/README.md` & `py_alpaca_daily_losers-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-1.0.1/pyproject.toml` & `py_alpaca_daily_losers-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-alpaca-daily-losers"
-version = "1.0.1"
+version = "1.0.2"
 description = "Daily Losers strategy, uses py-alpaca-api for Alpaca Markets integration."
 authors = ["TexasCoding <jeff10278@me.com>"]
 readme = "README.md"
 packages = [{include = "alpaca_daily_losers", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.12"
```

### Comparing `py_alpaca_daily_losers-1.0.1/src/alpaca_daily_losers/calc.py` & `py_alpaca_daily_losers-1.0.2/src/alpaca_daily_losers/calc.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-1.0.1/src/alpaca_daily_losers/daily_losers.py` & `py_alpaca_daily_losers-1.0.2/src/alpaca_daily_losers/daily_losers.py`

 * *Files 1% similar despite different names*

```diff
@@ -354,15 +354,16 @@
         - This function depends on the 'get_ticker_data()', 'buy_criteria()', 'send_message()',
         'get_sentiment()', 'update_or_create_watchlist()', and 'get_assets()'
         methods from other parts of the code.
         - The 'send_message()' function is responsible for sending a message/notification.
         - The 'tqdm' library is used to display a progress bar while processing the symbols.
         """
         yahoo = Yahoo()
-        losers = self.alpaca.screener.losers(total_losers_returned=130)["symbol"].to_list()
+        # losers = self.alpaca.screener.losers(total_losers_returned=130)["symbol"].to_list()
+        losers = self.alpaca.predictor.get_losers_to_gainers()
 
         losers = self.get_ticker_data(losers)
         losers = self.buy_criteria(losers)
 
         if len(losers) == 0:
             send_message("No daily losers found.")
             return []
```

### Comparing `py_alpaca_daily_losers-1.0.1/src/alpaca_daily_losers/openai.py` & `py_alpaca_daily_losers-1.0.2/src/alpaca_daily_losers/openai.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-1.0.1/src/alpaca_daily_losers/requests.py` & `py_alpaca_daily_losers-1.0.2/src/alpaca_daily_losers/requests.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-1.0.1/src/alpaca_daily_losers/slack.py` & `py_alpaca_daily_losers-1.0.2/src/alpaca_daily_losers/slack.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-1.0.1/src/alpaca_daily_losers/yahoo.py` & `py_alpaca_daily_losers-1.0.2/src/alpaca_daily_losers/yahoo.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-1.0.1/PKG-INFO` & `py_alpaca_daily_losers-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-alpaca-daily-losers
-Version: 1.0.1
+Version: 1.0.2
 Summary: Daily Losers strategy, uses py-alpaca-api for Alpaca Markets integration.
 Author: TexasCoding
 Author-email: jeff10278@me.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
```

