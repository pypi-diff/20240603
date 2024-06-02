# Comparing `tmp/sportswrangler-0.1.8.tar.gz` & `tmp/sportswrangler-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sportswrangler-0.1.8.tar", max compression
+gzip compressed data, was "sportswrangler-0.1.9.tar", max compression
```

## Comparing `sportswrangler-0.1.8.tar` & `sportswrangler-0.1.9.tar`

### file list

```diff
@@ -1,34 +1,37 @@
--rw-r--r--   0        0        0      454 2024-05-19 06:40:56.168608 sportswrangler-0.1.8/README.md
--rw-r--r--   0        0        0      422 2024-05-19 06:40:56.168608 sportswrangler-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      218 2024-05-19 06:40:56.168608 sportswrangler-0.1.8/sportswrangler/__init__.py
--rw-r--r--   0        0        0        0 2024-05-19 06:40:56.168608 sportswrangler-0.1.8/sportswrangler/generic/__init__.py
--rw-r--r--   0        0        0     2070 2024-05-19 06:40:56.168608 sportswrangler-0.1.8/sportswrangler/generic/wrangler.py
--rw-r--r--   0        0        0      129 2024-05-19 06:40:56.168608 sportswrangler-0.1.8/sportswrangler/global_configs.py
--rw-r--r--   0        0        0       28 2024-05-19 06:40:56.168608 sportswrangler-0.1.8/sportswrangler/odds/__init__.py
--rw-r--r--   0        0        0      206 2024-05-19 06:40:56.168608 sportswrangler-0.1.8/sportswrangler/odds/the_odds_api/__init__.py
--rw-r--r--   0        0        0        0 2024-05-19 06:40:56.168608 sportswrangler-0.1.8/sportswrangler/odds/the_odds_api/utils/__init__.py
--rw-r--r--   0        0        0     3747 2024-05-19 06:40:56.168608 sportswrangler-0.1.8/sportswrangler/odds/the_odds_api/utils/classes.py
--rw-r--r--   0        0        0      238 2024-05-19 06:40:56.168608 sportswrangler-0.1.8/sportswrangler/odds/the_odds_api/utils/constants.py
--rw-r--r--   0        0        0     4739 2024-05-19 06:40:56.168608 sportswrangler-0.1.8/sportswrangler/odds/the_odds_api/utils/enums.py
--rw-r--r--   0        0        0      252 2024-05-19 06:40:56.168608 sportswrangler-0.1.8/sportswrangler/odds/the_odds_api/wranglers/__init__.py
--rw-r--r--   0        0        0    20320 2024-05-19 06:40:56.168608 sportswrangler-0.1.8/sportswrangler/odds/the_odds_api/wranglers/base.py
--rw-r--r--   0        0        0     2059 2024-05-19 06:40:56.172608 sportswrangler-0.1.8/sportswrangler/odds/the_odds_api/wranglers/epl.py
--rw-r--r--   0        0        0     2127 2024-05-19 06:40:56.172608 sportswrangler-0.1.8/sportswrangler/odds/the_odds_api/wranglers/mlb.py
--rw-r--r--   0        0        0     1979 2024-05-19 06:40:56.172608 sportswrangler-0.1.8/sportswrangler/odds/the_odds_api/wranglers/nba.py
--rw-r--r--   0        0        0     2324 2024-05-19 06:40:56.172608 sportswrangler-0.1.8/sportswrangler/odds/the_odds_api/wranglers/nfl.py
--rw-r--r--   0        0        0     1400 2024-05-19 06:40:56.172608 sportswrangler-0.1.8/sportswrangler/odds/the_odds_api/wranglers/nhl.py
--rw-r--r--   0        0        0       51 2024-05-19 06:40:56.172608 sportswrangler-0.1.8/sportswrangler/sports/__init__.py
--rw-r--r--   0        0        0       40 2024-05-19 06:40:56.172608 sportswrangler-0.1.8/sportswrangler/sports/data_feeds/__init__.py
--rw-r--r--   0        0        0   531535 2024-05-19 06:40:56.172608 sportswrangler-0.1.8/sportswrangler/sports/data_feeds/assets/MLB/players.csv
--rw-r--r--   0        0        0     5204 2024-05-19 06:40:56.172608 sportswrangler-0.1.8/sportswrangler/sports/data_feeds/assets/MLB/teams.csv
--rw-r--r--   0        0        0   144790 2024-05-19 06:40:56.176608 sportswrangler-0.1.8/sportswrangler/sports/data_feeds/assets/NBA/players.csv
--rw-r--r--   0        0        0     3101 2024-05-19 06:40:56.176608 sportswrangler-0.1.8/sportswrangler/sports/data_feeds/assets/NBA/teams.csv
--rw-r--r--   0        0        0   774056 2024-05-19 06:40:56.176608 sportswrangler-0.1.8/sportswrangler/sports/data_feeds/assets/NFL/players.csv
--rw-r--r--   0        0        0     8878 2024-05-19 06:40:56.180608 sportswrangler-0.1.8/sportswrangler/sports/data_feeds/assets/NFL/teams.csv
--rw-r--r--   0        0        0   293594 2024-05-19 06:40:56.180608 sportswrangler-0.1.8/sportswrangler/sports/data_feeds/assets/NHL/players.csv
--rw-r--r--   0        0        0     3313 2024-05-19 06:40:56.180608 sportswrangler-0.1.8/sportswrangler/sports/data_feeds/assets/NHL/teams.csv
--rw-r--r--   0        0        0    12392 2024-05-19 06:40:56.180608 sportswrangler-0.1.8/sportswrangler/sports/data_feeds/wrangler.py
--rw-r--r--   0        0        0        0 2024-05-19 06:40:56.180608 sportswrangler-0.1.8/sportswrangler/utils/__init__.py
--rw-r--r--   0        0        0      250 2024-05-19 06:40:56.180608 sportswrangler-0.1.8/sportswrangler/utils/enums.py
--rw-r--r--   0        0        0      142 2024-05-19 06:40:56.180608 sportswrangler-0.1.8/sportswrangler/utils/helpers.py
--rw-r--r--   0        0        0     1104 1970-01-01 00:00:00.000000 sportswrangler-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      454 2024-06-02 22:29:32.726347 sportswrangler-0.1.9/README.md
+-rw-r--r--   0        0        0      437 2024-06-02 22:29:32.726347 sportswrangler-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      241 2024-06-02 22:29:32.730347 sportswrangler-0.1.9/sportswrangler/__init__.py
+-rw-r--r--   0        0        0       46 2024-06-02 22:29:32.730347 sportswrangler-0.1.9/sportswrangler/fantasy/__init__.py
+-rw-r--r--   0        0        0       42 2024-06-02 22:29:32.730347 sportswrangler-0.1.9/sportswrangler/fantasy/ktc/__init__.py
+-rw-r--r--   0        0        0     2810 2024-06-02 22:29:32.730347 sportswrangler-0.1.9/sportswrangler/fantasy/ktc/wrangler.py
+-rw-r--r--   0        0        0        0 2024-06-02 22:29:32.730347 sportswrangler-0.1.9/sportswrangler/generic/__init__.py
+-rw-r--r--   0        0        0     2070 2024-06-02 22:29:32.730347 sportswrangler-0.1.9/sportswrangler/generic/wrangler.py
+-rw-r--r--   0        0        0      129 2024-06-02 22:29:32.730347 sportswrangler-0.1.9/sportswrangler/global_configs.py
+-rw-r--r--   0        0        0       28 2024-06-02 22:29:32.730347 sportswrangler-0.1.9/sportswrangler/odds/__init__.py
+-rw-r--r--   0        0        0      206 2024-06-02 22:29:32.730347 sportswrangler-0.1.9/sportswrangler/odds/the_odds_api/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-02 22:29:32.730347 sportswrangler-0.1.9/sportswrangler/odds/the_odds_api/utils/__init__.py
+-rw-r--r--   0        0        0     3747 2024-06-02 22:29:32.730347 sportswrangler-0.1.9/sportswrangler/odds/the_odds_api/utils/classes.py
+-rw-r--r--   0        0        0      238 2024-06-02 22:29:32.730347 sportswrangler-0.1.9/sportswrangler/odds/the_odds_api/utils/constants.py
+-rw-r--r--   0        0        0     4739 2024-06-02 22:29:32.730347 sportswrangler-0.1.9/sportswrangler/odds/the_odds_api/utils/enums.py
+-rw-r--r--   0        0        0      252 2024-06-02 22:29:32.730347 sportswrangler-0.1.9/sportswrangler/odds/the_odds_api/wranglers/__init__.py
+-rw-r--r--   0        0        0    20320 2024-06-02 22:29:32.730347 sportswrangler-0.1.9/sportswrangler/odds/the_odds_api/wranglers/base.py
+-rw-r--r--   0        0        0     2059 2024-06-02 22:29:32.730347 sportswrangler-0.1.9/sportswrangler/odds/the_odds_api/wranglers/epl.py
+-rw-r--r--   0        0        0     2127 2024-06-02 22:29:32.730347 sportswrangler-0.1.9/sportswrangler/odds/the_odds_api/wranglers/mlb.py
+-rw-r--r--   0        0        0     1979 2024-06-02 22:29:32.730347 sportswrangler-0.1.9/sportswrangler/odds/the_odds_api/wranglers/nba.py
+-rw-r--r--   0        0        0     2324 2024-06-02 22:29:32.730347 sportswrangler-0.1.9/sportswrangler/odds/the_odds_api/wranglers/nfl.py
+-rw-r--r--   0        0        0     1400 2024-06-02 22:29:32.730347 sportswrangler-0.1.9/sportswrangler/odds/the_odds_api/wranglers/nhl.py
+-rw-r--r--   0        0        0       51 2024-06-02 22:29:32.730347 sportswrangler-0.1.9/sportswrangler/sports/__init__.py
+-rw-r--r--   0        0        0       40 2024-06-02 22:29:32.730347 sportswrangler-0.1.9/sportswrangler/sports/data_feeds/__init__.py
+-rw-r--r--   0        0        0   531535 2024-06-02 22:29:32.734347 sportswrangler-0.1.9/sportswrangler/sports/data_feeds/assets/MLB/players.csv
+-rw-r--r--   0        0        0     5204 2024-06-02 22:29:32.734347 sportswrangler-0.1.9/sportswrangler/sports/data_feeds/assets/MLB/teams.csv
+-rw-r--r--   0        0        0   144790 2024-06-02 22:29:32.734347 sportswrangler-0.1.9/sportswrangler/sports/data_feeds/assets/NBA/players.csv
+-rw-r--r--   0        0        0     3101 2024-06-02 22:29:32.734347 sportswrangler-0.1.9/sportswrangler/sports/data_feeds/assets/NBA/teams.csv
+-rw-r--r--   0        0        0   774056 2024-06-02 22:29:32.738347 sportswrangler-0.1.9/sportswrangler/sports/data_feeds/assets/NFL/players.csv
+-rw-r--r--   0        0        0     8878 2024-06-02 22:29:32.738347 sportswrangler-0.1.9/sportswrangler/sports/data_feeds/assets/NFL/teams.csv
+-rw-r--r--   0        0        0   293594 2024-06-02 22:29:32.742347 sportswrangler-0.1.9/sportswrangler/sports/data_feeds/assets/NHL/players.csv
+-rw-r--r--   0        0        0     3313 2024-06-02 22:29:32.742347 sportswrangler-0.1.9/sportswrangler/sports/data_feeds/assets/NHL/teams.csv
+-rw-r--r--   0        0        0    12342 2024-06-02 22:29:32.742347 sportswrangler-0.1.9/sportswrangler/sports/data_feeds/wrangler.py
+-rw-r--r--   0        0        0        0 2024-06-02 22:29:32.742347 sportswrangler-0.1.9/sportswrangler/utils/__init__.py
+-rw-r--r--   0        0        0      250 2024-06-02 22:29:32.742347 sportswrangler-0.1.9/sportswrangler/utils/enums.py
+-rw-r--r--   0        0        0      142 2024-06-02 22:29:32.742347 sportswrangler-0.1.9/sportswrangler/utils/helpers.py
+-rw-r--r--   0        0        0     1140 1970-01-01 00:00:00.000000 sportswrangler-0.1.9/PKG-INFO
```

### Comparing `sportswrangler-0.1.8/sportswrangler/generic/wrangler.py` & `sportswrangler-0.1.9/sportswrangler/generic/wrangler.py`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.8/sportswrangler/odds/the_odds_api/utils/classes.py` & `sportswrangler-0.1.9/sportswrangler/odds/the_odds_api/utils/classes.py`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.8/sportswrangler/odds/the_odds_api/utils/enums.py` & `sportswrangler-0.1.9/sportswrangler/odds/the_odds_api/utils/enums.py`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.8/sportswrangler/odds/the_odds_api/wranglers/base.py` & `sportswrangler-0.1.9/sportswrangler/odds/the_odds_api/wranglers/base.py`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.8/sportswrangler/odds/the_odds_api/wranglers/epl.py` & `sportswrangler-0.1.9/sportswrangler/odds/the_odds_api/wranglers/epl.py`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.8/sportswrangler/odds/the_odds_api/wranglers/mlb.py` & `sportswrangler-0.1.9/sportswrangler/odds/the_odds_api/wranglers/mlb.py`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.8/sportswrangler/odds/the_odds_api/wranglers/nba.py` & `sportswrangler-0.1.9/sportswrangler/odds/the_odds_api/wranglers/nba.py`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.8/sportswrangler/odds/the_odds_api/wranglers/nfl.py` & `sportswrangler-0.1.9/sportswrangler/odds/the_odds_api/wranglers/nfl.py`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.8/sportswrangler/odds/the_odds_api/wranglers/nhl.py` & `sportswrangler-0.1.9/sportswrangler/odds/the_odds_api/wranglers/nhl.py`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.8/sportswrangler/sports/data_feeds/assets/MLB/players.csv` & `sportswrangler-0.1.9/sportswrangler/sports/data_feeds/assets/MLB/players.csv`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.8/sportswrangler/sports/data_feeds/assets/MLB/teams.csv` & `sportswrangler-0.1.9/sportswrangler/sports/data_feeds/assets/MLB/teams.csv`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.8/sportswrangler/sports/data_feeds/assets/NBA/players.csv` & `sportswrangler-0.1.9/sportswrangler/sports/data_feeds/assets/NBA/players.csv`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.8/sportswrangler/sports/data_feeds/assets/NBA/teams.csv` & `sportswrangler-0.1.9/sportswrangler/sports/data_feeds/assets/NBA/teams.csv`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.8/sportswrangler/sports/data_feeds/assets/NFL/players.csv` & `sportswrangler-0.1.9/sportswrangler/sports/data_feeds/assets/NFL/players.csv`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.8/sportswrangler/sports/data_feeds/assets/NFL/teams.csv` & `sportswrangler-0.1.9/sportswrangler/sports/data_feeds/assets/NFL/teams.csv`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.8/sportswrangler/sports/data_feeds/assets/NHL/players.csv` & `sportswrangler-0.1.9/sportswrangler/sports/data_feeds/assets/NHL/players.csv`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.8/sportswrangler/sports/data_feeds/assets/NHL/teams.csv` & `sportswrangler-0.1.9/sportswrangler/sports/data_feeds/assets/NHL/teams.csv`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.8/sportswrangler/sports/data_feeds/wrangler.py` & `sportswrangler-0.1.9/sportswrangler/sports/data_feeds/wrangler.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from sportswrangler.utils.enums import Sport
 
 logger = logging.getLogger(__name__)
 __location__ = os.path.realpath(os.path.join(os.getcwd(), os.path.dirname(__file__)))
 
 
 class DataFeedsWrangler(Wrangler):
-    _endpoint = "http://rest.datafeeds.rolling-insights.com"
+    _endpoint = "http://rest.datafeeds.rolling-insights.com/api/v1"
     sport: Sport = None
     rsc_token: str = os.environ.get("DATA_FEEDS_RSC_TOKEN")
     """
     Token assigned to your account to make calls to DataFeeds
     """
 
     def request(self, url: str, additional_params=None) -> Response:
@@ -49,17 +49,16 @@
         self, api_path: str, additional_params=None, sports: list[Sport] = None
     ) -> dict[str, list] | dict[str, pd.DataFrame] | dict[str, pl.LazyFrame]:
         """
         :param sports: list of sports to parse into preferred dataframe
         :param api_path: path that will be appended to http://rest.datafeeds.rolling-insights.com/api/v1
         :param additional_params: dict of parameters to combine with RSC_token parameter
         """
-        path = "http://rest.datafeeds.rolling-insights.com/api/v1"
         response = self.request(
-            url=path + api_path,
+            url=self._endpoint + api_path,
             additional_params=additional_params or {},
         )
         data = response.json()["data"]
         if sports and self.preferred_dataframe:
             for sport in sports:
                 data[sport] = (
                     pd.DataFrame(data[sport])
```

### Comparing `sportswrangler-0.1.8/PKG-INFO` & `sportswrangler-0.1.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: sportswrangler
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python package for wranglin' sports and sports odds data
 Author: Dejon
 Author-email: dejon.wright@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: bs4 (>=0.0.2,<0.0.3)
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: polars (>=0.20.21,<0.21.0)
 Requires-Dist: pydantic (>=2.7.0,<3.0.0)
 Requires-Dist: pytest (>=8.1.1,<9.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
```

