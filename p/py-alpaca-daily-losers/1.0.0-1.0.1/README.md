# Comparing `tmp/py_alpaca_daily_losers-1.0.0.tar.gz` & `tmp/py_alpaca_daily_losers-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_alpaca_daily_losers-1.0.0.tar", max compression
+gzip compressed data, was "py_alpaca_daily_losers-1.0.1.tar", max compression
```

## Comparing `py_alpaca_daily_losers-1.0.0.tar` & `py_alpaca_daily_losers-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     2267 2024-06-01 22:06:14.046692 py_alpaca_daily_losers-1.0.0/README.md
--rw-r--r--   0        0        0     1212 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.0/src/alpaca_daily_losers/__init__.py
--rw-r--r--   0        0        0      902 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.0/src/alpaca_daily_losers/calc.py
--rw-r--r--   0        0        0    19678 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.0/src/alpaca_daily_losers/daily_losers.py
--rw-r--r--   0        0        0      460 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.0/src/alpaca_daily_losers/global_functions.py
--rw-r--r--   0        0        0     2563 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.0/src/alpaca_daily_losers/openai.py
--rw-r--r--   0        0        0     4550 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.0/src/alpaca_daily_losers/requests.py
--rw-r--r--   0        0        0     1896 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.0/src/alpaca_daily_losers/slack.py
--rw-r--r--   0        0        0     7069 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.0/src/alpaca_daily_losers/yahoo.py
--rw-r--r--   0        0        0     2981 1970-01-01 00:00:00.000000 py_alpaca_daily_losers-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2267 2024-06-01 22:06:14.046692 py_alpaca_daily_losers-1.0.1/README.md
+-rw-r--r--   0        0        0     1212 2024-06-01 23:02:16.236042 py_alpaca_daily_losers-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.1/src/alpaca_daily_losers/__init__.py
+-rw-r--r--   0        0        0      902 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.1/src/alpaca_daily_losers/calc.py
+-rw-r--r--   0        0        0    19678 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.1/src/alpaca_daily_losers/daily_losers.py
+-rw-r--r--   0        0        0      460 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.1/src/alpaca_daily_losers/global_functions.py
+-rw-r--r--   0        0        0     2563 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.1/src/alpaca_daily_losers/openai.py
+-rw-r--r--   0        0        0     4550 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.1/src/alpaca_daily_losers/requests.py
+-rw-r--r--   0        0        0     1896 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.1/src/alpaca_daily_losers/slack.py
+-rw-r--r--   0        0        0     7069 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.1/src/alpaca_daily_losers/yahoo.py
+-rw-r--r--   0        0        0     2981 1970-01-01 00:00:00.000000 py_alpaca_daily_losers-1.0.1/PKG-INFO
```

### Comparing `py_alpaca_daily_losers-1.0.0/README.md` & `py_alpaca_daily_losers-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-1.0.0/pyproject.toml` & `py_alpaca_daily_losers-1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "py-alpaca-daily-losers"
-version = "1.0.0"
+version = "1.0.1"
 description = "Daily Losers strategy, uses py-alpaca-api for Alpaca Markets integration."
 authors = ["TexasCoding <jeff10278@me.com>"]
 readme = "README.md"
 packages = [{include = "alpaca_daily_losers", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.12"
-py-alpaca-api = "^0.6.4"
+py-alpaca-api = "^1.0.0"
 requests = "^2.32.3"
 openai = "^1.30.5"
 slack-sdk = "^3.27.2"
 ta = "^0.11.0"
 yfinance = "^0.2.40"
 beautifulsoup4 = "^4.12.3"
 python-dotenv = "^1.0.1"
```

### Comparing `py_alpaca_daily_losers-1.0.0/src/alpaca_daily_losers/calc.py` & `py_alpaca_daily_losers-1.0.1/src/alpaca_daily_losers/calc.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-1.0.0/src/alpaca_daily_losers/daily_losers.py` & `py_alpaca_daily_losers-1.0.1/src/alpaca_daily_losers/daily_losers.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-1.0.0/src/alpaca_daily_losers/openai.py` & `py_alpaca_daily_losers-1.0.1/src/alpaca_daily_losers/openai.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-1.0.0/src/alpaca_daily_losers/requests.py` & `py_alpaca_daily_losers-1.0.1/src/alpaca_daily_losers/requests.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-1.0.0/src/alpaca_daily_losers/slack.py` & `py_alpaca_daily_losers-1.0.1/src/alpaca_daily_losers/slack.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-1.0.0/src/alpaca_daily_losers/yahoo.py` & `py_alpaca_daily_losers-1.0.1/src/alpaca_daily_losers/yahoo.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-1.0.0/PKG-INFO` & `py_alpaca_daily_losers-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: py-alpaca-daily-losers
-Version: 1.0.0
+Version: 1.0.1
 Summary: Daily Losers strategy, uses py-alpaca-api for Alpaca Markets integration.
 Author: TexasCoding
 Author-email: jeff10278@me.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
 Requires-Dist: openai (>=1.30.5,<2.0.0)
-Requires-Dist: py-alpaca-api (>=0.6.4,<0.7.0)
+Requires-Dist: py-alpaca-api (>=1.0.0,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: requests (>=2.32.3,<3.0.0)
 Requires-Dist: slack-sdk (>=3.27.2,<4.0.0)
 Requires-Dist: ta (>=0.11.0,<0.12.0)
 Requires-Dist: yfinance (>=0.2.40,<0.3.0)
 Description-Content-Type: text/markdown
```

