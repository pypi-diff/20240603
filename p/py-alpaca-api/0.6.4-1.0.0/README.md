# Comparing `tmp/py_alpaca_api-0.6.4.tar.gz` & `tmp/py_alpaca_api-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_alpaca_api-0.6.4.tar", max compression
+gzip compressed data, was "py_alpaca_api-1.0.0.tar", max compression
```

## Comparing `py_alpaca_api-0.6.4.tar` & `py_alpaca_api-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1066 2024-05-19 01:27:26.322892 py_alpaca_api-0.6.4/LICENSE
--rw-r--r--   0        0        0    17780 2024-06-01 03:16:13.087825 py_alpaca_api-0.6.4/README.md
--rw-r--r--   0        0        0        0 2024-05-19 01:27:26.322892 py_alpaca_api-0.6.4/py_alpaca_api/__init__.py
--rw-r--r--   0        0        0     2275 2024-06-01 03:16:13.097825 py_alpaca_api-0.6.4/py_alpaca_api/alpaca.py
--rw-r--r--   0        0        0        0 2024-05-22 22:57:11.657657 py_alpaca_api-0.6.4/py_alpaca_api/src/__init__.py
--rw-r--r--   0        0        0     6313 2024-06-01 00:51:31.644447 py_alpaca_api-0.6.4/py_alpaca_api/src/account.py
--rw-r--r--   0        0        0     2640 2024-06-01 00:51:31.644447 py_alpaca_api-0.6.4/py_alpaca_api/src/asset.py
--rw-r--r--   0        0        0    11730 2024-06-01 03:16:13.097825 py_alpaca_api-0.6.4/py_alpaca_api/src/data_classes.py
--rw-r--r--   0        0        0     7360 2024-06-01 00:51:31.644447 py_alpaca_api-0.6.4/py_alpaca_api/src/history.py
--rw-r--r--   0        0        0     2945 2024-06-01 00:51:31.644447 py_alpaca_api-0.6.4/py_alpaca_api/src/market.py
--rw-r--r--   0        0        0    18520 2024-06-01 00:51:31.644447 py_alpaca_api-0.6.4/py_alpaca_api/src/order.py
--rw-r--r--   0        0        0     8869 2024-06-01 00:51:31.644447 py_alpaca_api-0.6.4/py_alpaca_api/src/position.py
--rw-r--r--   0        0        0     2106 2024-06-01 00:51:31.644447 py_alpaca_api-0.6.4/py_alpaca_api/src/requests.py
--rw-r--r--   0        0        0     9400 2024-06-01 00:51:31.644447 py_alpaca_api-0.6.4/py_alpaca_api/src/screener.py
--rw-r--r--   0        0        0    14784 2024-06-01 00:51:31.644447 py_alpaca_api-0.6.4/py_alpaca_api/src/watchlist.py
--rw-r--r--   0        0        0     1344 2024-06-01 00:51:31.644447 py_alpaca_api-0.6.4/pyproject.toml
--rw-r--r--   0        0        0    18582 1970-01-01 00:00:00.000000 py_alpaca_api-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-19 01:27:26.322892 py_alpaca_api-1.0.0/LICENSE
+-rw-r--r--   0        0        0    17780 2024-06-01 03:16:13.087825 py_alpaca_api-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-19 01:27:26.322892 py_alpaca_api-1.0.0/py_alpaca_api/__init__.py
+-rw-r--r--   0        0        0     2275 2024-06-01 03:16:13.097825 py_alpaca_api-1.0.0/py_alpaca_api/alpaca.py
+-rw-r--r--   0        0        0        0 2024-05-22 22:57:11.657657 py_alpaca_api-1.0.0/py_alpaca_api/src/__init__.py
+-rw-r--r--   0        0        0     6338 2024-06-01 22:41:07.156285 py_alpaca_api-1.0.0/py_alpaca_api/src/account.py
+-rw-r--r--   0        0        0     2640 2024-06-01 00:51:31.644447 py_alpaca_api-1.0.0/py_alpaca_api/src/asset.py
+-rw-r--r--   0        0        0    11730 2024-06-01 03:16:13.097825 py_alpaca_api-1.0.0/py_alpaca_api/src/data_classes.py
+-rw-r--r--   0        0        0     7360 2024-06-01 00:51:31.644447 py_alpaca_api-1.0.0/py_alpaca_api/src/history.py
+-rw-r--r--   0        0        0     2945 2024-06-01 00:51:31.644447 py_alpaca_api-1.0.0/py_alpaca_api/src/market.py
+-rw-r--r--   0        0        0    18520 2024-06-01 00:51:31.644447 py_alpaca_api-1.0.0/py_alpaca_api/src/order.py
+-rw-r--r--   0        0        0     8870 2024-06-01 22:41:07.156285 py_alpaca_api-1.0.0/py_alpaca_api/src/position.py
+-rw-r--r--   0        0        0     4678 2024-06-01 22:41:07.156285 py_alpaca_api-1.0.0/py_alpaca_api/src/requests.py
+-rw-r--r--   0        0        0     9474 2024-06-01 22:41:07.156285 py_alpaca_api-1.0.0/py_alpaca_api/src/screener.py
+-rw-r--r--   0        0        0    14982 2024-06-01 22:41:07.156285 py_alpaca_api-1.0.0/py_alpaca_api/src/watchlist.py
+-rw-r--r--   0        0        0     1299 2024-06-01 22:41:07.156285 py_alpaca_api-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    18582 1970-01-01 00:00:00.000000 py_alpaca_api-1.0.0/PKG-INFO
```

### Comparing `py_alpaca_api-0.6.4/LICENSE` & `py_alpaca_api-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.6.4/README.md` & `py_alpaca_api-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.6.4/py_alpaca_api/alpaca.py` & `py_alpaca_api-1.0.0/py_alpaca_api/alpaca.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.6.4/py_alpaca_api/src/account.py` & `py_alpaca_api-1.0.0/py_alpaca_api/src/account.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,19 +44,14 @@
             raise ValueError("One of the Date and Until Date are required, not both or neither.")
 
         params = {
             "date": date if date else None,
             "until_date": until_date if until_date else None,
         }
 
-        # request = requests.get(url=url, headers=self.headers, params=params)
-
-        # if request.status_code != 200:
-        #     raise Exception(f"Failed to get account activities. Response: {request.text}")
-
         request = Requests().get(url=url, headers=self.headers, params=params)
         response = json.loads(request.text)
 
         activity_df = pd.DataFrame()
         activity_df.assign(
             symbol="NAN",
             activity_type="NAN",
@@ -175,9 +170,17 @@
             ],
         )
 
         timestamp_transformed = (
             pd.to_datetime(portfolio_df["timestamp"], unit="s").dt.tz_localize("America/New_York").dt.tz_convert("UTC").apply(lambda x: x.date())
         )
         portfolio_df["timestamp"] = timestamp_transformed
+        portfolio_df = portfolio_df.astype(
+            {
+                "equity": "float",
+                "profit_loss": "float",
+                "profit_loss_pct": "float",
+                "base_value": "float",
+            }
+        )
         portfolio_df["profit_loss_pct"] = portfolio_df["profit_loss_pct"] * 100
         return portfolio_df
```

### Comparing `py_alpaca_api-0.6.4/py_alpaca_api/src/asset.py` & `py_alpaca_api-1.0.0/py_alpaca_api/src/asset.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.6.4/py_alpaca_api/src/data_classes.py` & `py_alpaca_api-1.0.0/py_alpaca_api/src/data_classes.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.6.4/py_alpaca_api/src/history.py` & `py_alpaca_api-1.0.0/py_alpaca_api/src/history.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.6.4/py_alpaca_api/src/market.py` & `py_alpaca_api-1.0.0/py_alpaca_api/src/market.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.6.4/py_alpaca_api/src/order.py` & `py_alpaca_api-1.0.0/py_alpaca_api/src/order.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.6.4/py_alpaca_api/src/position.py` & `py_alpaca_api-1.0.0/py_alpaca_api/src/position.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     # \\\\\\\\\\\\\\\\\ Get Positions /////////////////////#
     ########################################################
     def get_all(self) -> pd.DataFrame:
         """
         Retrieves all positions from the Alpaca API and returns them as a DataFrame.
 
         Returns:
-            pd.DataFrame: A DataFrame containing the positions data.
+            pd.DataFrame: A DataFrame containing the position's data.
 
         Raises:
             Exception: If the API response is not successful.
         """
 
         url = f"{self.trade_url}/positions"
         request = Requests().get(url=url, headers=self.headers)
```

### Comparing `py_alpaca_api-0.6.4/py_alpaca_api/src/screener.py` & `py_alpaca_api-1.0.0/py_alpaca_api/src/screener.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,16 +93,18 @@
     ) -> pd.DataFrame:
         """
         Returns a filtered DataFrame of stocks that meet the specified conditions for losers.
 
         Args:
             price_greater_than (float): The minimum price threshold for stocks to be considered losers. Default is 5.0.
             change_less_than (float): The maximum change threshold for stocks to be considered losers. Default is -2.0.
-            volume_greater_than (int): The minimum volume threshold for stocks to be considered losers. Default is 20000.
-            trade_count_greater_than (int): The minimum trade count threshold for stocks to be considered losers. Default is 2000.
+            volume_greater_than (int): The minimum volume threshold for stocks to be considered losers. Default is
+            20000.
+            trade_count_greater_than (int): The minimum trade count threshold for stocks to be considered losers.
+             Default is 2000.
             total_losers_returned (int): The maximum number of losers to be returned. Default is 100.
 
         Returns:
             pd.DataFrame: A filtered DataFrame containing stocks that meet the specified conditions for losers.
         """
         return self.filter_stocks(
             price_greater_than,
@@ -122,19 +124,23 @@
         change_greater_than: float = 2.0,
         volume_greater_than: int = 20000,
         trade_count_greater_than: int = 2000,
         total_gainers_returned: int = 100,
     ) -> pd.DataFrame:
         """
         Args:
-            price_greater_than (float): The minimum price threshold for the stocks to be included in the gainers list. Default is 5.0.
-            change_greater_than (float): The minimum change (in percentage) threshold for the stocks to be included in the gainers list.
+            price_greater_than (float): The minimum price threshold for the stocks to be included in the gainers list.
+            Default is 5.0.
+            change_greater_than (float): The minimum change (in percentage) threshold for the stocks to be included in
+            the gainers list.
             Default is 2.0.
-            volume_greater_than (int): The minimum volume threshold for the stocks to be included in the gainers list. Default is 20000.
-            trade_count_greater_than (int): The minimum trade count threshold for the stocks to be included in the gainers list. Default is 2000.
+            volume_greater_than (int): The minimum volume threshold for the stocks to be included in the gainers list.
+             Default is 20000.
+            trade_count_greater_than (int): The minimum trade count threshold for the stocks to be included in the
+            gainers list. Default is 2000.
             total_gainers_returned (int): The maximum number of gainers to be returned. Default is 100.
 
         Returns:
             pd.DataFrame: A Pandas DataFrame containing the stocks that satisfy the criteria for being gainers.
 
         """
         return self.filter_stocks(
```

### Comparing `py_alpaca_api-0.6.4/py_alpaca_api/src/watchlist.py` & `py_alpaca_api-1.0.0/py_alpaca_api/src/watchlist.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,25 +165,29 @@
         name: str = "",
         symbols: Union[list, str] = None,
     ) -> WatchlistClass:
         """
         Update a watchlist with the specified parameters.
 
         Args:
-            watchlist_id (str, optional): The ID of the watchlist to update. Either `watchlist_id` or `watchlist_name` must be provided.
-            watchlist_name (str, optional): The name of the watchlist to update. Either `watchlist_id` or `watchlist_name` must be provided.
+            watchlist_id (str, optional): The ID of the watchlist to update. Either `watchlist_id` or `watchlist_name`
+            must be provided.
+            watchlist_name (str, optional): The name of the watchlist to update. Either `watchlist_id` or
+            `watchlist_name` must be provided.
             name (str, optional): The new name for the watchlist. If not provided, the existing name will be used.
-            symbols (str, optional): A comma-separated string of symbols to update the watchlist with. If not provided, the existing symbols
+            symbols (str, optional): A comma-separated string of symbols to update the watchlist with. If not provided,
+             the existing symbols
             will be used.
 
         Returns:
             WatchlistClass: The updated watchlist.
 
         Raises:
-            ValueError: If both `watchlist_id` and `watchlist_name` are provided, or if neither `watchlist_id` nor `watchlist_name` are provided.
+            ValueError: If both `watchlist_id` and `watchlist_name` are provided, or if neither `watchlist_id` nor
+            `watchlist_name` are provided.
 
         """
 
         if watchlist_id and watchlist_name or (not watchlist_id and not watchlist_name):
             raise ValueError("Watchlist ID or Name is required, not both.")
         # Check if watchlist_id is provided
         if watchlist_id:
@@ -251,23 +255,27 @@
         watchlist_name: str = None,
         symbol: str = "",
     ) -> WatchlistClass:
         """
         Adds an asset to a watchlist.
 
         Args:
-            watchlist_id (str, optional): The ID of the watchlist to add the asset to. If not provided, the watchlist_name
-            parameter must be provided. watchlist_name (str, optional): The name of the watchlist to add the asset to. If not provided,
-            the watchlist_id parameter must be provided. symbol (str): The symbol of the asset to add to the watchlist.
+            watchlist_id (str): The ID of the watchlist to add the asset to. If `watchlist_id` is provided,
+            `watchlist_name` should be None.
+            watchlist_name (str): The name of the watchlist to add the asset to. If `watchlist_name` is provided,
+            `watchlist_id` should be None.
+            symbol (str): The symbol of the asset to add to the watchlist.
 
         Returns:
-            WatchlistClass: The updated watchlist object.
+            WatchlistClass: The updated watchlist after adding the asset.
 
         Raises:
-            ValueError: If both watchlist_id and watchlist_name are provided, or if symbol is not provided.
+            ValueError: If both `watchlist_id` and `watchlist_name` are provided or neither is provided.
+            ValueError: If `symbol` is not provided.
+
         """
         if watchlist_id and watchlist_name or (not watchlist_id and not watchlist_name):
             raise ValueError("Watchlist ID or Name is required, not both.")
 
         if not symbol:
             raise ValueError("Symbol is required")
 
@@ -294,17 +302,19 @@
         watchlist_name: str = None,
         symbol: str = "",
     ) -> WatchlistClass:
         """
         Removes an asset from a watchlist.
 
         Args:
-            watchlist_id (str, optional): The ID of the watchlist. If not provided, the watchlist_name parameter will be used to
+            watchlist_id (str, optional): The ID of the watchlist. If not provided, the watchlist_name parameter
+            will be used to
             retrieve the ID. Defaults to None.
-            watchlist_name (str, optional): The name of the watchlist. If not provided, thewatchlist_id parameter will be used to
+            watchlist_name (str, optional): The name of the watchlist. If not provided, thewatchlist_id parameter
+             will be used to
             retrieve the ID. Defaults to None.
             symbol (str): The symbol of the asset to be removed from the watchlist.
 
         Returns:
             WatchlistClass: The updated watchlist object.
 
         Raises:
@@ -331,24 +341,27 @@
     # /////////// Get Assets from a watchlist /////////////#
     ########################################################
     def get_assets(self, watchlist_id: str = None, watchlist_name: str = None) -> list:
         """
         Retrieves the symbols of assets in a watchlist.
 
         Args:
-            watchlist_id (str, optional): The ID of the watchlist. Either `watchlist_id` or `watchlist_name` should be provided,
+            watchlist_id (str, optional): The ID of the watchlist. Either `watchlist_id` or `watchlist_name`
+             should be provided,
             not both. Defaults to None.
-            watchlist_name (str, optional): The name of the watchlist. Either `watchlist_id` or `watchlist_name` should be
+            watchlist_name (str, optional): The name of the watchlist. Either `watchlist_id` or `watchlist_name`
+             should be
             provided, not both. Defaults to None.
 
         Returns:
             list: A list of symbols of assets in the watchlist.
 
         Raises:
-            ValueError: If both `watchlist_id` and `watchlist_name` are provided, or if neither `watchlist_id` nor `watchlist_name` are provided.
+            ValueError: If both `watchlist_id` and `watchlist_name` are provided, or if neither `watchlist_id` nor
+            `watchlist_name` are provided.
         """
 
         if watchlist_id and watchlist_name:
             raise ValueError("Watchlist ID or Name is required, not both.")
 
         if watchlist_id:
             watchlist = self.get(watchlist_id=watchlist_id)
```

### Comparing `py_alpaca_api-0.6.4/pyproject.toml` & `py_alpaca_api-1.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-alpaca-api"
-version = "0.6.4"
+version = "1.0.0"
 description = "Python package, for communicating with Alpaca Markets REST API."
 authors = ["TexasCoding <jeff10278@me.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/TexasCoding/py-alpaca-api"
 repository = "https://github.com/TexasCoding/py-alpaca-api"
 documentation = "https://py-alpaca-api.readthedocs.io/en/latest/"
@@ -23,16 +23,14 @@
 requests-mock = "^1.12.1"
 black = "^24.4.2"
 isort = "^5.13.2"
 pre-commit = "^3.7.1"
 ipykernel = "^6.29.4"
 pytest-mock = "^3.14.0"
 pytest-mock-server = "^0.3.0"
-python-dotenv = "^1.0.1"
-coverage = "^7.5.1"
 
 
 [tool.poetry.group.test.dependencies]
 flake8 = "^7.0.0"
 
 
 [tool.poetry.group.doc.dependencies]
```

### Comparing `py_alpaca_api-0.6.4/PKG-INFO` & `py_alpaca_api-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-alpaca-api
-Version: 0.6.4
+Version: 1.0.0
 Summary: Python package, for communicating with Alpaca Markets REST API.
 Home-page: https://github.com/TexasCoding/py-alpaca-api
 License: MIT
 Keywords: alpaca,python
 Author: TexasCoding
 Author-email: jeff10278@me.com
 Requires-Python: >=3.12,<4.0
```

