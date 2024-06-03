# Comparing `tmp/supamodel-0.5.8.tar.gz` & `tmp/supamodel-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supamodel-0.5.8.tar", max compression
+gzip compressed data, was "supamodel-0.5.9.tar", max compression
```

## Comparing `supamodel-0.5.8.tar` & `supamodel-0.5.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     3741 2024-04-15 21:10:14.946524 supamodel-0.5.8/README.md
--rw-r--r--   0        0        0      869 2024-05-01 11:08:33.723095 supamodel-0.5.8/pyproject.toml
--rw-r--r--   0        0        0      336 2024-04-28 01:05:41.483823 supamodel-0.5.8/supamodel/__init__.py
--rw-r--r--   0        0        0     8349 2024-04-15 21:10:14.947482 supamodel-0.5.8/supamodel/_abc.py
--rw-r--r--   0        0        0      291 2024-04-16 02:36:19.549095 supamodel-0.5.8/supamodel/_client.py
--rw-r--r--   0        0        0     8016 2024-04-15 21:10:14.947711 supamodel-0.5.8/supamodel/_core.py
--rw-r--r--   0        0        0      674 2024-04-15 21:10:14.947815 supamodel-0.5.8/supamodel/_logging.py
--rw-r--r--   0        0        0      335 2024-04-15 21:10:14.947906 supamodel-0.5.8/supamodel/_types.py
--rw-r--r--   0        0        0     1488 2024-04-15 21:10:14.948025 supamodel-0.5.8/supamodel/config.py
--rw-r--r--   0        0        0     2284 2024-04-15 21:10:14.948124 supamodel-0.5.8/supamodel/enums.py
--rw-r--r--   0        0        0      321 2024-04-15 21:10:14.948205 supamodel-0.5.8/supamodel/errors.py
--rw-r--r--   0        0        0     1432 2024-04-15 21:10:14.948303 supamodel-0.5.8/supamodel/exceptions.py
--rw-r--r--   0        0        0     8307 2024-04-15 21:10:14.948494 supamodel-0.5.8/supamodel/supa.py
--rw-r--r--   0        0        0     4187 2024-04-15 21:10:14.948633 supamodel-0.5.8/supamodel/supa_builder.py
--rw-r--r--   0        0        0        0 2024-04-15 21:10:14.948743 supamodel-0.5.8/supamodel/trading/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 21:10:14.948807 supamodel-0.5.8/supamodel/trading/assets.py
--rw-r--r--   0        0        0     3690 2024-04-15 21:10:14.949133 supamodel-0.5.8/supamodel/trading/clock.py
--rw-r--r--   0        0        0     3464 2024-04-15 23:57:47.194613 supamodel-0.5.8/supamodel/trading/exchange.py
--rw-r--r--   0        0        0     1336 2024-04-15 21:10:14.949430 supamodel-0.5.8/supamodel/trading/market_data.py
--rw-r--r--   0        0        0     2111 2024-04-27 20:47:39.714063 supamodel-0.5.8/supamodel/trading/order_management.py
--rw-r--r--   0        0        0     1992 2024-04-28 00:56:16.180477 supamodel-0.5.8/supamodel/trading/portfolio.py
--rw-r--r--   0        0        0    11732 2024-04-15 21:10:14.949788 supamodel-0.5.8/supamodel/trading/tokens.py
--rw-r--r--   0        0        0    15200 2024-05-01 11:08:19.531005 supamodel-0.5.8/supamodel/utils.py
--rw-r--r--   0        0        0     4847 1970-01-01 00:00:00.000000 supamodel-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0     3741 2024-05-04 18:44:05.155812 supamodel-0.5.9/README.md
+-rw-r--r--   0        0        0      871 2024-06-03 11:38:49.157604 supamodel-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0      336 2024-04-28 01:05:41.483823 supamodel-0.5.9/supamodel/__init__.py
+-rw-r--r--   0        0        0     8349 2024-04-15 21:10:14.947482 supamodel-0.5.9/supamodel/_abc.py
+-rw-r--r--   0        0        0      291 2024-04-16 02:36:19.549095 supamodel-0.5.9/supamodel/_client.py
+-rw-r--r--   0        0        0     8016 2024-04-15 21:10:14.947711 supamodel-0.5.9/supamodel/_core.py
+-rw-r--r--   0        0        0      196 2024-06-03 11:37:55.231283 supamodel-0.5.9/supamodel/_logging.py
+-rw-r--r--   0        0        0      335 2024-04-15 21:10:14.947906 supamodel-0.5.9/supamodel/_types.py
+-rw-r--r--   0        0        0     1488 2024-04-15 21:10:14.948025 supamodel-0.5.9/supamodel/config.py
+-rw-r--r--   0        0        0     2284 2024-04-15 21:10:14.948124 supamodel-0.5.9/supamodel/enums.py
+-rw-r--r--   0        0        0      321 2024-04-15 21:10:14.948205 supamodel-0.5.9/supamodel/errors.py
+-rw-r--r--   0        0        0     1432 2024-04-15 21:10:14.948303 supamodel-0.5.9/supamodel/exceptions.py
+-rw-r--r--   0        0        0     8307 2024-04-15 21:10:14.948494 supamodel-0.5.9/supamodel/supa.py
+-rw-r--r--   0        0        0     4187 2024-04-15 21:10:14.948633 supamodel-0.5.9/supamodel/supa_builder.py
+-rw-r--r--   0        0        0        0 2024-04-15 21:10:14.948743 supamodel-0.5.9/supamodel/trading/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 21:10:14.948807 supamodel-0.5.9/supamodel/trading/assets.py
+-rw-r--r--   0        0        0     3690 2024-04-15 21:10:14.949133 supamodel-0.5.9/supamodel/trading/clock.py
+-rw-r--r--   0        0        0     3464 2024-04-15 23:57:47.194613 supamodel-0.5.9/supamodel/trading/exchange.py
+-rw-r--r--   0        0        0     1336 2024-04-15 21:10:14.949430 supamodel-0.5.9/supamodel/trading/market_data.py
+-rw-r--r--   0        0        0     2111 2024-04-27 20:47:39.714063 supamodel-0.5.9/supamodel/trading/order_management.py
+-rw-r--r--   0        0        0     1992 2024-04-28 00:56:16.180477 supamodel-0.5.9/supamodel/trading/portfolio.py
+-rw-r--r--   0        0        0    11732 2024-04-15 21:10:14.949788 supamodel-0.5.9/supamodel/trading/tokens.py
+-rw-r--r--   0        0        0    15184 2024-05-03 03:38:23.053959 supamodel-0.5.9/supamodel/utils.py
+-rw-r--r--   0        0        0     4847 1970-01-01 00:00:00.000000 supamodel-0.5.9/PKG-INFO
```

### Comparing `supamodel-0.5.8/README.md` & `supamodel-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.8/pyproject.toml` & `supamodel-0.5.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "supamodel"
-version = "0.5.8"
+version = "0.5.9"
 description = "Pydantic Models for Trading Algos and Supabase"
 authors = ["Kevin Hill <kivo360@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.9,<=3.12"
+python = ">=3.9,<=3.13"
 pendulum = ">=2.0.0,<4.0.0"
 loguru = ">=0.5.0,<1.0.0"
 pydantic = { extras = ["email"], version = "^2.7.0" }
 rich = "^13.7.1"
 pydantic-settings = ">=2.0.0,<=3.0.0"
 numpy = "^1.26.4"
 inflector = "^3.1.1"
@@ -31,11 +31,11 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 # Create ruff configuration
 [tool.ruff]
 fixable = ["ALL"]
-ignore = ["F401"]
+# ignore = ["F401"]
 
 
 # docstring_code_format = false
```

### Comparing `supamodel-0.5.8/supamodel/_abc.py` & `supamodel-0.5.9/supamodel/_abc.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.8/supamodel/_core.py` & `supamodel-0.5.9/supamodel/_core.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.8/supamodel/config.py` & `supamodel-0.5.9/supamodel/config.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.8/supamodel/enums.py` & `supamodel-0.5.9/supamodel/enums.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.8/supamodel/exceptions.py` & `supamodel-0.5.9/supamodel/exceptions.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.8/supamodel/supa.py` & `supamodel-0.5.9/supamodel/supa.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.8/supamodel/supa_builder.py` & `supamodel-0.5.9/supamodel/supa_builder.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.8/supamodel/trading/clock.py` & `supamodel-0.5.9/supamodel/trading/clock.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.8/supamodel/trading/exchange.py` & `supamodel-0.5.9/supamodel/trading/exchange.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.8/supamodel/trading/market_data.py` & `supamodel-0.5.9/supamodel/trading/market_data.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.8/supamodel/trading/order_management.py` & `supamodel-0.5.9/supamodel/trading/order_management.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.8/supamodel/trading/portfolio.py` & `supamodel-0.5.9/supamodel/trading/portfolio.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.8/supamodel/trading/tokens.py` & `supamodel-0.5.9/supamodel/trading/tokens.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.8/supamodel/utils.py` & `supamodel-0.5.9/supamodel/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 import diskcache
 import orjson as json
 import pandas as pd
 import sniffio
 import typer
 from diskcache import UNKNOWN, Cache as LocalCache, memoize_stampede
 from inflector import Inflector
-from pydantic import BaseModel, computed_field
+from pydantic import BaseModel
 from sniffio import current_async_library
 
 # ---------------------------------------------------------
 # Cache utilities
 # ---------------------------------------------------------
```

### Comparing `supamodel-0.5.8/PKG-INFO` & `supamodel-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: supamodel
-Version: 0.5.8
+Version: 0.5.9
 Summary: Pydantic Models for Trading Algos and Supabase
 Author: Kevin Hill
 Author-email: kivo360@gmail.com
-Requires-Python: >=3.9,<=3.12
+Requires-Python: >=3.9,<=3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: diskcache (>=5.6.3,<6.0.0)
 Requires-Dist: inflector (>=3.1.1,<4.0.0)
```

