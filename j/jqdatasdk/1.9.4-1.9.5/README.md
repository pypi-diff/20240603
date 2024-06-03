# Comparing `tmp/jqdatasdk-1.9.4.tar.gz` & `tmp/jqdatasdk-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jqdatasdk-1.9.4.tar", last modified: Thu Apr 18 10:01:02 2024, max compression
+gzip compressed data, was "jqdatasdk-1.9.5.tar", last modified: Mon Jun  3 10:46:36 2024, max compression
```

## Comparing `jqdatasdk-1.9.4.tar` & `jqdatasdk-1.9.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 huoty      (501) staff       (20)        0 2024-04-18 10:01:02.852576 jqdatasdk-1.9.4/
--rw-r--r--   0 huoty      (501) staff       (20)     2100 2023-10-09 02:41:53.000000 jqdatasdk-1.9.4/CHANGELOG.md
--rw-r--r--   0 huoty      (501) staff       (20)     1066 2023-10-09 02:41:53.000000 jqdatasdk-1.9.4/LICENSE
--rw-r--r--   0 huoty      (501) staff       (20)       26 2023-10-09 02:41:53.000000 jqdatasdk-1.9.4/MANIFEST.in
--rw-r--r--   0 huoty      (501) staff       (20)     5489 2024-04-18 10:01:02.852452 jqdatasdk-1.9.4/PKG-INFO
--rw-r--r--   0 huoty      (501) staff       (20)     4767 2023-10-09 02:41:53.000000 jqdatasdk-1.9.4/README.md
-drwxr-xr-x   0 huoty      (501) staff       (20)        0 2024-04-18 10:01:02.849860 jqdatasdk-1.9.4/jqdatasdk/
--rw-r--r--   0 huoty      (501) staff       (20)     1893 2024-03-08 07:08:51.000000 jqdatasdk-1.9.4/jqdatasdk/__init__.py
--rw-r--r--   0 huoty      (501) staff       (20)    56654 2023-10-09 02:41:53.000000 jqdatasdk-1.9.4/jqdatasdk/alpha101.py
--rw-r--r--   0 huoty      (501) staff       (20)    88690 2023-10-09 02:41:53.000000 jqdatasdk-1.9.4/jqdatasdk/alpha191.py
--rw-r--r--   0 huoty      (501) staff       (20)    53070 2024-04-18 09:40:52.000000 jqdatasdk-1.9.4/jqdatasdk/api.py
--rw-r--r--   0 huoty      (501) staff       (20)     1680 2023-10-09 02:41:53.000000 jqdatasdk-1.9.4/jqdatasdk/calendar_service.py
--rw-r--r--   0 huoty      (501) staff       (20)    17404 2024-03-13 06:29:19.000000 jqdatasdk-1.9.4/jqdatasdk/client.py
-drwxr-xr-x   0 huoty      (501) staff       (20)        0 2024-04-18 10:01:02.850813 jqdatasdk-1.9.4/jqdatasdk/compat/
--rw-r--r--   0 huoty      (501) staff       (20)        0 2023-10-09 02:41:53.000000 jqdatasdk-1.9.4/jqdatasdk/compat/__init__.py
--rw-r--r--   0 huoty      (501) staff       (20)     8710 2023-10-09 02:41:53.000000 jqdatasdk-1.9.4/jqdatasdk/compat/pickle_compat.py
--rw-r--r--   0 huoty      (501) staff       (20)      166 2023-10-09 02:41:53.000000 jqdatasdk-1.9.4/jqdatasdk/exceptions.py
--rw-r--r--   0 huoty      (501) staff       (20)    10242 2023-10-09 02:41:53.000000 jqdatasdk-1.9.4/jqdatasdk/finance_service.py
--rw-r--r--   0 huoty      (501) staff       (20)    28674 2023-10-09 02:41:53.000000 jqdatasdk-1.9.4/jqdatasdk/finance_tables.py
--rw-r--r--   0 huoty      (501) staff       (20)    33828 2023-10-25 11:44:21.000000 jqdatasdk-1.9.4/jqdatasdk/fundamentals_tables_gen.py
--rw-r--r--   0 huoty      (501) staff       (20)     4235 2024-01-03 07:42:27.000000 jqdatasdk-1.9.4/jqdatasdk/table.py
--rw-r--r--   0 huoty      (501) staff       (20)   106372 2023-10-09 02:41:53.000000 jqdatasdk-1.9.4/jqdatasdk/technical_analysis.py
--rw-r--r--   0 huoty      (501) staff       (20)      836 2023-10-09 02:41:53.000000 jqdatasdk-1.9.4/jqdatasdk/thriftclient.py
--rw-r--r--   0 huoty      (501) staff       (20)    14833 2023-10-09 02:41:53.000000 jqdatasdk-1.9.4/jqdatasdk/utils.py
--rw-r--r--   0 huoty      (501) staff       (20)      422 2024-04-18 09:58:20.000000 jqdatasdk-1.9.4/jqdatasdk/version.py
-drwxr-xr-x   0 huoty      (501) staff       (20)        0 2024-04-18 10:01:02.850626 jqdatasdk-1.9.4/jqdatasdk.egg-info/
--rw-r--r--   0 huoty      (501) staff       (20)     5489 2024-04-18 10:01:02.000000 jqdatasdk-1.9.4/jqdatasdk.egg-info/PKG-INFO
--rw-r--r--   0 huoty      (501) staff       (20)      795 2024-04-18 10:01:02.000000 jqdatasdk-1.9.4/jqdatasdk.egg-info/SOURCES.txt
--rw-r--r--   0 huoty      (501) staff       (20)        1 2024-04-18 10:01:02.000000 jqdatasdk-1.9.4/jqdatasdk.egg-info/dependency_links.txt
--rw-r--r--   0 huoty      (501) staff       (20)        1 2023-11-02 08:41:51.000000 jqdatasdk-1.9.4/jqdatasdk.egg-info/not-zip-safe
--rw-r--r--   0 huoty      (501) staff       (20)      106 2024-04-18 10:01:02.000000 jqdatasdk-1.9.4/jqdatasdk.egg-info/requires.txt
--rw-r--r--   0 huoty      (501) staff       (20)       10 2024-04-18 10:01:02.000000 jqdatasdk-1.9.4/jqdatasdk.egg-info/top_level.txt
--rw-r--r--   0 huoty      (501) staff       (20)      106 2023-10-09 02:41:53.000000 jqdatasdk-1.9.4/requirements-py2.txt
--rw-r--r--   0 huoty      (501) staff       (20)      106 2023-10-09 02:41:53.000000 jqdatasdk-1.9.4/requirements.txt
--rw-r--r--   0 huoty      (501) staff       (20)       38 2024-04-18 10:01:02.852634 jqdatasdk-1.9.4/setup.cfg
--rw-r--r--   0 huoty      (501) staff       (20)     2123 2023-10-09 02:41:53.000000 jqdatasdk-1.9.4/setup.py
-drwxr-xr-x   0 huoty      (501) staff       (20)        0 2024-04-18 10:01:02.852191 jqdatasdk-1.9.4/tests/
--rw-r--r--   0 huoty      (501) staff       (20)    79416 2024-04-18 08:58:43.000000 jqdatasdk-1.9.4/tests/test_api.py
--rw-r--r--   0 huoty      (501) staff       (20)      487 2023-10-09 02:41:53.000000 jqdatasdk-1.9.4/tests/test_client.py
--rw-r--r--   0 huoty      (501) staff       (20)     3670 2024-01-03 07:39:42.000000 jqdatasdk-1.9.4/tests/test_table.py
--rw-r--r--   0 huoty      (501) staff       (20)     2216 2023-10-09 02:41:53.000000 jqdatasdk-1.9.4/tests/test_utils.py
+drwxr-xr-x   0 huoty      (501) staff       (20)        0 2024-06-03 10:46:36.388800 jqdatasdk-1.9.5/
+-rw-r--r--   0 huoty      (501) staff       (20)     2100 2023-10-09 02:41:53.000000 jqdatasdk-1.9.5/CHANGELOG.md
+-rw-r--r--   0 huoty      (501) staff       (20)     1066 2023-10-09 02:41:53.000000 jqdatasdk-1.9.5/LICENSE
+-rw-r--r--   0 huoty      (501) staff       (20)       26 2023-10-09 02:41:53.000000 jqdatasdk-1.9.5/MANIFEST.in
+-rw-r--r--   0 huoty      (501) staff       (20)     5489 2024-06-03 10:46:36.388650 jqdatasdk-1.9.5/PKG-INFO
+-rw-r--r--   0 huoty      (501) staff       (20)     4767 2023-10-09 02:41:53.000000 jqdatasdk-1.9.5/README.md
+drwxr-xr-x   0 huoty      (501) staff       (20)        0 2024-06-03 10:46:36.386015 jqdatasdk-1.9.5/jqdatasdk/
+-rw-r--r--   0 huoty      (501) staff       (20)     1893 2024-03-08 07:08:51.000000 jqdatasdk-1.9.5/jqdatasdk/__init__.py
+-rw-r--r--   0 huoty      (501) staff       (20)    56654 2023-10-09 02:41:53.000000 jqdatasdk-1.9.5/jqdatasdk/alpha101.py
+-rw-r--r--   0 huoty      (501) staff       (20)    88690 2023-10-09 02:41:53.000000 jqdatasdk-1.9.5/jqdatasdk/alpha191.py
+-rw-r--r--   0 huoty      (501) staff       (20)    56489 2024-06-03 10:34:24.000000 jqdatasdk-1.9.5/jqdatasdk/api.py
+-rw-r--r--   0 huoty      (501) staff       (20)     1680 2023-10-09 02:41:53.000000 jqdatasdk-1.9.5/jqdatasdk/calendar_service.py
+-rw-r--r--   0 huoty      (501) staff       (20)    17520 2024-05-22 03:31:33.000000 jqdatasdk-1.9.5/jqdatasdk/client.py
+drwxr-xr-x   0 huoty      (501) staff       (20)        0 2024-06-03 10:46:36.386953 jqdatasdk-1.9.5/jqdatasdk/compat/
+-rw-r--r--   0 huoty      (501) staff       (20)        0 2023-10-09 02:41:53.000000 jqdatasdk-1.9.5/jqdatasdk/compat/__init__.py
+-rw-r--r--   0 huoty      (501) staff       (20)     8710 2023-10-09 02:41:53.000000 jqdatasdk-1.9.5/jqdatasdk/compat/pickle_compat.py
+-rw-r--r--   0 huoty      (501) staff       (20)      166 2023-10-09 02:41:53.000000 jqdatasdk-1.9.5/jqdatasdk/exceptions.py
+-rw-r--r--   0 huoty      (501) staff       (20)    10242 2023-10-09 02:41:53.000000 jqdatasdk-1.9.5/jqdatasdk/finance_service.py
+-rw-r--r--   0 huoty      (501) staff       (20)    31843 2024-05-30 05:53:08.000000 jqdatasdk-1.9.5/jqdatasdk/finance_tables.py
+-rw-r--r--   0 huoty      (501) staff       (20)    37001 2024-05-30 05:53:08.000000 jqdatasdk-1.9.5/jqdatasdk/fundamentals_tables_gen.py
+-rw-r--r--   0 huoty      (501) staff       (20)     4235 2024-01-03 07:42:27.000000 jqdatasdk-1.9.5/jqdatasdk/table.py
+-rw-r--r--   0 huoty      (501) staff       (20)   106372 2023-10-09 02:41:53.000000 jqdatasdk-1.9.5/jqdatasdk/technical_analysis.py
+-rw-r--r--   0 huoty      (501) staff       (20)      836 2023-10-09 02:41:53.000000 jqdatasdk-1.9.5/jqdatasdk/thriftclient.py
+-rw-r--r--   0 huoty      (501) staff       (20)    14833 2023-10-09 02:41:53.000000 jqdatasdk-1.9.5/jqdatasdk/utils.py
+-rw-r--r--   0 huoty      (501) staff       (20)      422 2024-06-03 10:45:28.000000 jqdatasdk-1.9.5/jqdatasdk/version.py
+drwxr-xr-x   0 huoty      (501) staff       (20)        0 2024-06-03 10:46:36.386772 jqdatasdk-1.9.5/jqdatasdk.egg-info/
+-rw-r--r--   0 huoty      (501) staff       (20)     5489 2024-06-03 10:46:36.000000 jqdatasdk-1.9.5/jqdatasdk.egg-info/PKG-INFO
+-rw-r--r--   0 huoty      (501) staff       (20)      795 2024-06-03 10:46:36.000000 jqdatasdk-1.9.5/jqdatasdk.egg-info/SOURCES.txt
+-rw-r--r--   0 huoty      (501) staff       (20)        1 2024-06-03 10:46:36.000000 jqdatasdk-1.9.5/jqdatasdk.egg-info/dependency_links.txt
+-rw-r--r--   0 huoty      (501) staff       (20)        1 2023-11-02 08:41:51.000000 jqdatasdk-1.9.5/jqdatasdk.egg-info/not-zip-safe
+-rw-r--r--   0 huoty      (501) staff       (20)      198 2024-06-03 10:46:36.000000 jqdatasdk-1.9.5/jqdatasdk.egg-info/requires.txt
+-rw-r--r--   0 huoty      (501) staff       (20)       10 2024-06-03 10:46:36.000000 jqdatasdk-1.9.5/jqdatasdk.egg-info/top_level.txt
+-rw-r--r--   0 huoty      (501) staff       (20)      115 2024-05-10 08:03:03.000000 jqdatasdk-1.9.5/requirements-py2.txt
+-rw-r--r--   0 huoty      (501) staff       (20)      192 2024-05-10 08:33:03.000000 jqdatasdk-1.9.5/requirements.txt
+-rw-r--r--   0 huoty      (501) staff       (20)       38 2024-06-03 10:46:36.388844 jqdatasdk-1.9.5/setup.cfg
+-rw-r--r--   0 huoty      (501) staff       (20)     2123 2023-10-09 02:41:53.000000 jqdatasdk-1.9.5/setup.py
+drwxr-xr-x   0 huoty      (501) staff       (20)        0 2024-06-03 10:46:36.388393 jqdatasdk-1.9.5/tests/
+-rw-r--r--   0 huoty      (501) staff       (20)    82711 2024-05-31 02:58:45.000000 jqdatasdk-1.9.5/tests/test_api.py
+-rw-r--r--   0 huoty      (501) staff       (20)      487 2023-10-09 02:41:53.000000 jqdatasdk-1.9.5/tests/test_client.py
+-rw-r--r--   0 huoty      (501) staff       (20)     3670 2024-01-03 07:39:42.000000 jqdatasdk-1.9.5/tests/test_table.py
+-rw-r--r--   0 huoty      (501) staff       (20)     2216 2023-10-09 02:41:53.000000 jqdatasdk-1.9.5/tests/test_utils.py
```

### Comparing `jqdatasdk-1.9.4/CHANGELOG.md` & `jqdatasdk-1.9.5/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `jqdatasdk-1.9.4/LICENSE` & `jqdatasdk-1.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jqdatasdk-1.9.4/PKG-INFO` & `jqdatasdk-1.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jqdatasdk
-Version: 1.9.4
+Version: 1.9.5
 Summary: jqdatasdk<easy utility for getting financial market data of China>
 Home-page: https://www.joinquant.com/data
 Author: JoinQuant
 Author-email: xlx@joinquant.com
 Maintainer: tech_data
 Maintainer-email: tech_data@joinquant.com
 License: Apache License v2
```

### Comparing `jqdatasdk-1.9.4/README.md` & `jqdatasdk-1.9.5/README.md`

 * *Files identical despite different names*

### Comparing `jqdatasdk-1.9.4/jqdatasdk/__init__.py` & `jqdatasdk-1.9.5/jqdatasdk/__init__.py`

 * *Files identical despite different names*

### Comparing `jqdatasdk-1.9.4/jqdatasdk/alpha101.py` & `jqdatasdk-1.9.5/jqdatasdk/alpha101.py`

 * *Files identical despite different names*

### Comparing `jqdatasdk-1.9.4/jqdatasdk/alpha191.py` & `jqdatasdk-1.9.5/jqdatasdk/alpha191.py`

 * *Files identical despite different names*

### Comparing `jqdatasdk-1.9.4/jqdatasdk/api.py` & `jqdatasdk-1.9.5/jqdatasdk/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,36 +143,80 @@
     """ 获取多个标的在指定交易日范围内的市值表数据
     Args:
         security_list: 标的code字符串列表或者单个标的字符串
         end_date: 查询结束时间
         start_date: 查询开始时间，不能与count共用
         count: 表示往前查询每一个标的count个交易日的数据，如果期间标的停牌，则该标的返回的市值数据数量小于count
         fields: 财务数据中市值表的字段，返回结果中总会包含code、day字段，可用字段如下：
-            code	股票代码	带后缀.XSHE/.XSHG
-            day	日期	取数据的日期
-            capitalization	总股本(万股)
-            circulating_cap	流通股本(万股)
-            market_cap	总市值(亿元)
-            circulating_market_cap	流通市值(亿元)
-            turnover_ratio	换手率(%)
-            pe_ratio	市盈率(PE, TTM)
-            pe_ratio_lyr	市盈率(PE)s
-            pb_ratio	市净率(PB)
-            ps_ratio	市销率(PS, TTM)
-            pcf_ratio	市现率(PCF, 现金净流量TTM)
+            code    股票代码        带后缀.XSHE/.XSHG
+            day     日期            取数据的日期
+            pe_ratio	            市盈率(PE, TTM)
+            turnover_ratio	        换手率(%)
+            pb_ratio	            市净率(PB)
+            ps_ratio	            市销率(PS, TTM)
+            pcf_ratio	            市现率(PCF, 现金净流量TTM)
+            capitalization	        总股本(万股)
+            market_cap	            总市值(亿元)
+            circulating_cap	        流通股本(万股)
+            circulating_market_cap  流通市值(亿元)
+            pe_ratio_lyr	        市盈率(PE)s
+            pcf_ratio2              市现率(PCF, 经营活动现金流TTM)
+            dividend_ratio          股息率
+            free_cap                自由流通股本
+            free_market_cap         自由流通市值
+            a_cap                   A 股总股本
+            a_market_cap            A 股总市值
+
     Returns:
         返回一个dataframe，索引默认是pandas的整数索引，返回的结果中总会包含code、day字段。
     """
     start_date = to_date_str(start_date)
     end_date = to_date_str(end_date)
     security_list = convert_security(security_list)
     return JQDataClient.instance().get_valuation(**locals())
 
 
 @assert_auth
+@hashable_lru(maxsize=3)
+def get_index_valuation(security_list, start_date=None, end_date=None, fields=None, count=None):
+    """ 获取多个指数及申万/聚宽一级行业在指定交易日范围内的市值表数据
+    Args:
+        security_list: 标的code字符串列表或者单个标的字符串
+        end_date: 查询结束时间
+        start_date: 查询开始时间，不能与count共用
+        count: 表示往前查询每一个指数count个交易日的数据，如果期间无指数，则该指数返回的市值数据数量小于count
+        fields: 财务数据中市值表的字段，返回结果中总会包含code、day字段，可用字段如下：
+            code    指数和行业代码   指数需带后缀.XSHE/.XSHG/.CSI
+            day     日期            取数据的日期
+            pe_ratio                市盈率(PE, TTM)
+            turnover_ratio          换手率(%)
+            pb_ratio                市净率(PB)
+            ps_ratio                市销率(PS, TTM)
+            pcf_ratio               市现率(PCF, 现金净流量TTM)
+            capitalization          总股本(万股)
+            market_cap              总市值(亿元)
+            circulating_cap         流通股本(万股)
+            circulating_market_cap  流通市值(亿元)
+            pe_ratio_lyr            市盈率(PE)s
+            pcf_ratio2              市现率(PCF, 经营活动现金流TTM)
+            dividend_ratio          股息率
+            free_cap                自由流通股本
+            free_market_cap         自由流通市值
+            a_cap                   A 股总股本
+            a_market_cap            A 股总市值
+    Returns:
+        返回一个dataframe，索引默认是pandas的整数索引，返回的结果中总会包含code、day字段。
+    """
+    start_date = to_date_str(start_date)
+    end_date = to_date_str(end_date)
+    security_list = convert_security(security_list)
+    return JQDataClient.instance().get_index_valuation(**locals())
+
+
+@assert_auth
 def get_history_fundamentals(security, fields, watch_date=None, stat_date=None,
                              count=1, interval='1q', stat_by_year=False):
     """ 获取多个季度/年度的三大财务报表和财务指标数据. 可指定单季度数据, 也可以指定年度数据.
             可以指定观察日期, 也可以指定最后一个报告期的结束日期.
     Args:
         security: 股票代码或者股票代码列表。
         fields: 要查询的财务数据的列, 季度数据和年度数据可选择的列不同. 示例:
@@ -530,15 +574,15 @@
     """
     assert underlying_symbol, "underlying_symbol is required"
     dt = to_date_str(date)
     return JQDataClient.instance().get_future_contracts(underlying_symbol=underlying_symbol, dt=dt)
 
 
 @assert_auth
-def get_dominant_future(underlying_symbol, date=None, end_date=None):
+def get_dominant_future(underlying_symbol=None, date=None, end_date=None):
     """
     获取主力合约对应的标的
 
     :param underlying_symbol 期货合约品种，如 ‘AG’(白银)
     :param date 日期（默认为当前时刻，当指定 end_date 时则表示开始日期）
     :param end_date 结束日期，当指定该参数时表示获取一段时间的主力合约
     :return 主力合约对应的期货合约（指定 end_date 时返回 pandas.Series，否则返回字符串）
@@ -744,14 +788,31 @@
     data.seek(1)  # 跳过第一个字符，从第二个开始取数据
     df = pd.read_csv(data, index_col=0, converters={"datetime": str2time})
     df = df[tick_fields]
     if len(security) <= 1:
         df.index = [0]
     return df
 
+
+@assert_auth
+def get_today_tick_period(security, start_date=None, end_date=None):
+    """获取一个/多个标的当天最新/一段时间内的tick
+    只可以查询当天标的, (期货可含夜盘, start_dt/end_dt必须大于当前交易日的开始时间 20:55)
+    :param security 标的代码,可以为一个标的或者多个标的组成的list
+    :param start_date 默认为 None, 不指定 start_date 时返回截至 end_date 最新的一条 tick, 指定时返回 start_date (含)到 end_date (含)之间的所有 tick
+    :param end_date 默认为None, 即当前时间
+    :return DataFrame
+    """
+    assert security, "security is required"
+    security = convert_security(security)
+    start_date = to_date_str(start_date) if start_date else None
+    end_date = to_date_str(end_date) if end_date else None
+    return JQDataClient.instance().get_today_tick_period(**locals())
+
+
 def request_data(security):
     http_token = JQDataClient.instance().get_http_token()
     codes = ",".join(security)
     headers = {
         'Accept-Encoding': 'gzip, deflate',
         'Content-Type': 'application/json',
         'Connection': 'keep-alive'
@@ -1134,15 +1195,15 @@
 
 @assert_auth
 def get_order_future_bar(symbol,
                          future_type,
                          start_dt,
                          end_dt,
                          unit='1d',
-                         fields=('date', 'open', 'high', 'low', 'close','volume', 'money', 'open_interest'),
+                         fields=('code', 'date', 'open', 'high', 'low', 'close','volume', 'money', 'open_interest'),
                          include_now=True):
     """获取当月/次月/当季/隔季等合约拼接而成的行情数据
     参数
         symbol : 品种代码, 如 'IF'
         future_type : 合约类型, 按当前可交易的合约顺序推算, 0 为当月, 1 为次月, 也可以按季度, '0q' 为当季(最近一个季月), '1q' 为次季 .....
         start_dt : 开始时间
         end_dt : 结束时间
```

### Comparing `jqdatasdk-1.9.4/jqdatasdk/calendar_service.py` & `jqdatasdk-1.9.5/jqdatasdk/calendar_service.py`

 * *Files identical despite different names*

### Comparing `jqdatasdk-1.9.4/jqdatasdk/client.py` & `jqdatasdk-1.9.5/jqdatasdk/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -424,15 +424,19 @@
         for _ in range(count + 5):
             self.ensure_auth()
             try:
                 start_time_local = int(time.time() * 1e9)
                 response = self.client.query(request)
                 end_time = time.time() * 1e9
             except socket_error as ex:
-                if isinstance(ex, socket.timeout) and not self._ping_server():
+                if (
+                    isinstance(ex, socket.timeout) or
+                    "TSocket read 0 bytes" in str(ex) or
+                    not self._ping_server()
+                ):
                     self._reset()
                 continue
             if not response.status:
                 raise self.get_error(response)
             try:
                 start_time = int(response.msg[:50])
             except ValueError:
```

### Comparing `jqdatasdk-1.9.4/jqdatasdk/compat/pickle_compat.py` & `jqdatasdk-1.9.5/jqdatasdk/compat/pickle_compat.py`

 * *Files identical despite different names*

### Comparing `jqdatasdk-1.9.4/jqdatasdk/finance_service.py` & `jqdatasdk-1.9.5/jqdatasdk/finance_service.py`

 * *Files identical despite different names*

### Comparing `jqdatasdk-1.9.4/jqdatasdk/finance_tables.py` & `jqdatasdk-1.9.5/jqdatasdk/finance_tables.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,14 +106,39 @@
     ordinary_risk_reserve_fund = Column(Float(20), doc="一般风险准备(元)")
     retained_profit = Column(Float(20), doc="未分配利润(元)")
     foreign_currency_report_conv_diff = Column(Float(20), doc="外币报表折算差额(元)")
     equities_parent_company_owners = Column(Float(20), doc="归属于母公司股东权益合计(元)")
     minority_interests = Column(Float(20), doc="少数股东权益(元)")
     total_owner_equities = Column(Float(20), doc="股东权益合计(元)")
     total_sheet_owner_equities = Column(Float(20), doc="负债和股东权益合计")
+    other_comprehensive_income = Column(Float(20), doc="其他综合收益(元)")
+    deferred_earning = Column(Float(20), doc="非流动负债-递延收益(元)")
+    loan_and_advance_current_assets = Column(Float(20), doc="流动资产-发放贷款及垫款(元)")
+    derivative_financial_asset = Column(Float(20), doc="衍生金融资产(元)")
+    hold_sale_asset = Column(Float(20), doc="划分为持有待售的资产(元)")
+    loan_and_advance_noncurrent_assets = Column(Float(20), doc="非流动资产-发放贷款及垫款(元)")
+    derivative_financial_liability = Column(Float(20), doc="衍生金融负债(元)")
+    hold_sale_liability = Column(Float(20), doc="划分为持有待售的负债(元)")
+    estimate_liability_current = Column(Float(20), doc="流动负债-预计负债(元)")
+    deferred_earning_current = Column(Float(20), doc="流动负债-递延收益(元)")
+    preferred_shares_noncurrent = Column(Float(20), doc="非流动负债-优先股(元)")
+    pepertual_liability_noncurrent = Column(Float(20), doc="非流动负债-永续债(元)")
+    longterm_salaries_payable = Column(Float(20), doc="长期应付职工薪酬(元)")
+    other_equity_tools = Column(Float(20), doc="其他权益工具(元)")
+    preferred_shares_equity = Column(Float(20), doc="其中：优先股-所有者权益")
+    pepertual_liability_equity = Column(Float(20), doc="所有者权益-永续债(元)")
+    receivable_fin = Column(Float(20), doc="应收款项融资(元)")
+    usufruct_assets = Column(Float(20), doc="使用权资产(元)")
+    contract_assets = Column(Float(20), doc="合同资产")
+    bond_invest = Column(Float(20), doc="债权投资")
+    other_bond_invest = Column(Float(20), doc="其他债权投资")
+    other_equity_tools_invest = Column(Float(20), doc="其他权益工具投资")
+    other_non_current_financial_assets = Column(Float(20), doc="其他非流动金融资产")
+    contract_liability = Column(Float(20), doc="合同负债")
+    lease_liability = Column(Float(20), doc="租赁负债")
 
 
 class CashFlowStatementDay(Base):
     """
     现金流表
     """
 
@@ -226,35 +251,50 @@
     minority_profit = Column(Float(20), doc="少数股东损益(元)")
     basic_eps = Column(Float(20), doc="基本每股收益(元)")
     diluted_eps = Column(Float(20), doc="稀释每股收益(元)")
     other_composite_income = Column(Float(20), doc="其他综合收益(元)")
     total_composite_income = Column(Float(20), doc="综合收益总额(元)")
     ci_parent_company_owners = Column(Float(20), doc="归属于母公司所有者的综合收益总额(元)")
     ci_minority_owners = Column(Float(20), doc="归属于少数股东的综合收益总额(元)")
-
+    rd_expenses = Column(Float(20), doc="研发费用")
+    asset_deal_income = Column(Float(20), doc="资产处置收益")
+    sust_operate_net_profit = Column(Float(20), doc="持续经营净利润")
+    discon_operate_net_profit = Column(Float(20), doc="终止经营净利润")
+    credit_impairment_loss = Column(Float(20), doc="信用减值损失")
+    net_open_hedge_income = Column(Float(20), doc="净敞口套期收益")
+    interest_cost_fin = Column(Float(20), doc="财务费用 - 利息费用")
+    interest_income_fin = Column(Float(20), doc="财务费用 - 利息收入")
+    other_earnings = Column(Float(20), doc="其他收益")
+    other_composite_income_mino_at = Column(Float(20), doc="归属于少数股东的其他综合收益的税后净额")
 
 class StockValuation(Base):
     """
     市值表
     """
     __tablename__ = 'stock_valuation'
 
     id = Column(Integer, primary_key=True)
     code = Column(String(12), nullable=False, doc="股票代码(带后缀: .XSHE/.XSHG)")
+    day = Column(Date, nullable=False, doc="日期")
     pe_ratio = Column(Float(20), doc='市盈率')
     turnover_ratio = Column(Float(20), doc="换手率")
     pb_ratio = Column(Float(20), doc="市净率")
     ps_ratio = Column(Float(20), doc="市销率")
     pcf_ratio = Column(Float(20), doc="市现率")
     capitalization = Column(Float(20), doc="总股本(万股)")
     market_cap = Column(Float(20), doc="总市值(亿元)")
     circulating_cap = Column(Float(20), doc="流通股本(万股)")
     circulating_market_cap = Column(Float(20), doc="总市值(亿元)")
-    day = Column(Date, nullable=False, doc="日期")
     pe_ratio_lyr = Column(Float(20), doc="市盈率LYR")
+    pcf_ratio2 = Column(Float(20), doc="市现率(PCF, 经营活动现金流TTM)")
+    dividend_ratio = Column(Float(20), doc="股息率")
+    free_cap = Column(Float(20), doc="自由流通股本")
+    free_market_cap = Column(Float(20), doc="自由流通市值")
+    a_cap = Column(Float(20), doc="A 股总股本")
+    a_market_cap = Column(Float(20), doc="A 股总市值")
 
 
 class FinancialIndicatorDay(Base):
     """
     财务指标表
     """
 
@@ -410,9 +450,7 @@
     not_expired_duty_reserve = Column(Float(20), doc="未到期责任准备金（产险业务）(元)")
     outstanding_claims_reserve = Column(Float(20), doc="未决赔款准备金（产险业务）(元)")
     comprehensive_cost_ratio = Column(Float(10), doc="综台成本率（产险业务）(%)")
     comprehensive_compensation_rate = Column(Float(10), doc="综台赔付率（产险业务）(%)")
     solvency_adequacy_ratio = Column(Float(10), doc="偿付能力充足率(%)")
     actual_capital = Column(Float(20), doc="实际资本(元)")
     minimum_capital = Column(Float(20), doc="最低资本(元)")
-
-
```

### Comparing `jqdatasdk-1.9.4/jqdatasdk/fundamentals_tables_gen.py` & `jqdatasdk-1.9.5/jqdatasdk/fundamentals_tables_gen.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,14 +117,39 @@
     ordinary_risk_reserve_fund = Column(Float(20), doc="一般风险准备(元)")
     retained_profit = Column(Float(20), doc="未分配利润(元)")
     foreign_currency_report_conv_diff = Column(Float(20), doc="外币报表折算差额(元)")
     equities_parent_company_owners = Column(Float(20), doc="归属于母公司股东权益合计(元)")
     minority_interests = Column(Float(20), doc="少数股东权益(元)")
     total_owner_equities = Column(Float(20), doc="股东权益合计(元)")
     total_sheet_owner_equities = Column(Float(20), doc="负债和股东权益合计")
+    other_comprehensive_income = Column(Float(20), doc="其他综合收益(元)")
+    deferred_earning = Column(Float(20), doc="非流动负债-递延收益(元)")
+    loan_and_advance_current_assets = Column(Float(20), doc="流动资产-发放贷款及垫款(元)")
+    derivative_financial_asset = Column(Float(20), doc="衍生金融资产(元)")
+    hold_sale_asset = Column(Float(20), doc="划分为持有待售的资产(元)")
+    loan_and_advance_noncurrent_assets = Column(Float(20), doc="非流动资产-发放贷款及垫款(元)")
+    derivative_financial_liability = Column(Float(20), doc="衍生金融负债(元)")
+    hold_sale_liability = Column(Float(20), doc="划分为持有待售的负债(元)")
+    estimate_liability_current = Column(Float(20), doc="流动负债-预计负债(元)")
+    deferred_earning_current = Column(Float(20), doc="流动负债-递延收益(元)")
+    preferred_shares_noncurrent = Column(Float(20), doc="非流动负债-优先股(元)")
+    pepertual_liability_noncurrent = Column(Float(20), doc="非流动负债-永续债(元)")
+    longterm_salaries_payable = Column(Float(20), doc="长期应付职工薪酬(元)")
+    other_equity_tools = Column(Float(20), doc="其他权益工具(元)")
+    preferred_shares_equity = Column(Float(20), doc="其中：优先股-所有者权益")
+    pepertual_liability_equity = Column(Float(20), doc="所有者权益-永续债(元)")
+    receivable_fin = Column(Float(20), doc="应收款项融资(元)")
+    usufruct_assets = Column(Float(20), doc="使用权资产(元)")
+    contract_assets = Column(Float(20), doc="合同资产")
+    bond_invest = Column(Float(20), doc="债权投资")
+    other_bond_invest = Column(Float(20), doc="其他债权投资")
+    other_equity_tools_invest = Column(Float(20), doc="其他权益工具投资")
+    other_non_current_financial_assets = Column(Float(20), doc="其他非流动金融资产")
+    contract_liability = Column(Float(20), doc="合同负债")
+    lease_liability = Column(Float(20), doc="租赁负债")
 
 
 class CashFlowStatement(Base):
     """
     现金流表
     """
 
@@ -250,27 +275,39 @@
     basic_eps = Column(Float(20), doc="基本每股收益(元)")
     diluted_eps = Column(Float(20), doc="稀释每股收益(元)")
     other_composite_income = Column(Float(20), doc="其他综合收益(元)")
     total_composite_income = Column(Float(20), doc="综合收益总额(元)")
     ci_parent_company_owners = Column(Float(20), doc="归属于母公司所有者的综合收益总额(元)")
     ci_minority_owners = Column(Float(20), doc="归属于少数股东的综合收益总额(元)")
     # compId = Column(String(16), nullable=False, unique=True, server_default=text("''"))
+    rd_expenses = Column(Float(20), doc="研发费用")
+    asset_deal_income = Column(Float(20), doc="资产处置收益")
+    sust_operate_net_profit = Column(Float(20), doc="持续经营净利润")
+    discon_operate_net_profit = Column(Float(20), doc="终止经营净利润")
+    credit_impairment_loss = Column(Float(20), doc="信用减值损失")
+    net_open_hedge_income = Column(Float(20), doc="净敞口套期收益")
+    interest_cost_fin = Column(Float(20), doc="财务费用 - 利息费用")
+    interest_income_fin = Column(Float(20), doc="财务费用 - 利息收入")
+    other_earnings = Column(Float(20), doc="其他收益")
+    other_composite_income_mino_at = Column(Float(20), doc="归属于少数股东的其他综合收益的税后净额")
+
 
 class StockValuation(Base):
     """
     市值表
     """
     __tablename__ = 'stock_valuation'
     # __table_args__ = (
     #     Index('idx_statDate_code', 'statDate', 'code', unique=True),
     #     Index('idx_day_code', 'day', 'code', unique=True)
     # )
 
     id = Column(Integer, primary_key=True)
     code = Column(String(12), nullable=False, doc="股票代码(带后缀: .XSHE/.XSHG)")
+    day = Column(Date, nullable=False, doc="日期")
     # year = Column(String(4), nullable=False, doc="年份")
     # type = Column(String(64), nullable=False, doc="Q1,S1,Q3,A")
     # pubDate = Column(Date, nullable=False, server_default=text("'0000-00-00'"))
     # statDate = Column(Date, nullable=False, server_default=text("'0000-00-00'"))
     # periodStart = Column(Date, nullable=False, server_default=text("'0000-00-00'"), doc="两次报告之间的日期范围:start date")
     # periodEnd = Column(Date, nullable=False, server_default=text("'0000-00-00'"), doc="两次报告之间的日期范围:end date")
     # reportId = Column(Integer, nullable=False, server_default=text("'0'"))
@@ -279,17 +316,22 @@
     pb_ratio = Column(Float(20), doc="市净率")
     ps_ratio = Column(Float(20), doc="市销率")
     pcf_ratio = Column(Float(20), doc="市现率")
     capitalization = Column(Float(20), doc="总股本(万股)")
     market_cap = Column(Float(20), doc="总市值(亿元)")
     circulating_cap = Column(Float(20), doc="流通股本(万股)")
     circulating_market_cap = Column(Float(20), doc="总市值(亿元)")
-    day = Column(Date, nullable=False, doc="日期")
     # compId = Column(String(16), nullable=False, unique=True, server_default=text("''"))
     pe_ratio_lyr = Column(Float(20), doc="市盈率LYR")
+    pcf_ratio2 = Column(Float(20), doc="市现率(PCF, 经营活动现金流TTM)")
+    dividend_ratio = Column(Float(20), doc="股息率")
+    free_cap = Column(Float(20), doc="自由流通股本")
+    free_market_cap = Column(Float(20), doc="自由流通市值")
+    a_cap = Column(Float(20), doc="A 股总股本")
+    a_market_cap = Column(Float(20), doc="A 股总市值")
 
 
 class FinancialIndicator(Base):
     """
     财务指标表
     """
```

### Comparing `jqdatasdk-1.9.4/jqdatasdk/table.py` & `jqdatasdk-1.9.5/jqdatasdk/table.py`

 * *Files identical despite different names*

### Comparing `jqdatasdk-1.9.4/jqdatasdk/technical_analysis.py` & `jqdatasdk-1.9.5/jqdatasdk/technical_analysis.py`

 * *Files identical despite different names*

### Comparing `jqdatasdk-1.9.4/jqdatasdk/thriftclient.py` & `jqdatasdk-1.9.5/jqdatasdk/thriftclient.py`

 * *Files identical despite different names*

### Comparing `jqdatasdk-1.9.4/jqdatasdk/utils.py` & `jqdatasdk-1.9.5/jqdatasdk/utils.py`

 * *Files identical despite different names*

### Comparing `jqdatasdk-1.9.4/jqdatasdk.egg-info/PKG-INFO` & `jqdatasdk-1.9.5/jqdatasdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jqdatasdk
-Version: 1.9.4
+Version: 1.9.5
 Summary: jqdatasdk<easy utility for getting financial market data of China>
 Home-page: https://www.joinquant.com/data
 Author: JoinQuant
 Author-email: xlx@joinquant.com
 Maintainer: tech_data
 Maintainer-email: tech_data@joinquant.com
 License: Apache License v2
```

### Comparing `jqdatasdk-1.9.4/jqdatasdk.egg-info/SOURCES.txt` & `jqdatasdk-1.9.5/jqdatasdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jqdatasdk-1.9.4/setup.py` & `jqdatasdk-1.9.5/setup.py`

 * *Files identical despite different names*

### Comparing `jqdatasdk-1.9.4/tests/test_api.py` & `jqdatasdk-1.9.5/tests/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from __future__ import print_function
 
 import re
 import time
 import datetime
 import logging
+import six
 
 import pytest
 try:
     from unittest import mock
 except ImportError:
     import mock
 
@@ -547,14 +548,18 @@
     df = get_fundamentals(query(income.day).limit(10), date='2016-07-01')
     assert isinstance(df, pd.DataFrame)
     assert len(df.index) == 10
     df = get_fundamentals(query(income.day).limit(10))
     assert(len(df.index)) == 10
     with pytest.raises(Exception) as e:
         get_fundamentals(query(income.day).limit(10), date='2016-07-01', statDate='2016-07-01')
+    df = get_fundamentals(query(income).limit(10))
+    assert 'rd_expenses' in df.columns
+    df = get_fundamentals(query(balance).limit(10))
+    assert 'lease_liability' in df.columns
 
 
 def test_get_fundamentals2():
     q = query(
         valuation.code,
         indicator.statDate,
         indicator.roe,
@@ -704,14 +709,32 @@
         '2020-05-08': 'AG2006.XSGE', '2020-05-11': 'AG2012.XSGE'
     }).sort_index())
 
     with pytest.raises(Exception):
         get_dominant_future("AG", date="2004-06-30")
     assert len(get_dominant_future("AG", end_date="2004-06-30")) == 0
 
+    res = get_dominant_future(underlying_symbol="ag", date='2020-05-08', end_date="2020-05-08 21:00:00")
+    assert res.equals(pd.Series({'2020-05-08': 'AG2006.XSGE', '2020-05-11': 'AG2012.XSGE'}).sort_index())
+    today_date = str(datetime.date.today())
+    assert set(get_dominant_future().index) == set(get_dominant_future(
+        None, date=today_date, end_date=today_date).columns)
+    res = get_dominant_future('RR')
+    assert isinstance(res, (str, six.string_types))
+    res = get_dominant_future('RR', end_date=today_date)
+    assert isinstance(res, pd.Series)
+    res = get_dominant_future(underlying_symbol=['AG', 'PX', 'SH', 'x'], date='2024-05-06')
+    assert res.equals(pd.Series({'AG': 'AG2406.XSGE', 'PX': 'PX2409.XZCE', 'SH': 'SH2409.XZCE', 'X': ''}))
+    res = get_dominant_future(underlying_symbol=['AG', 'RR'], date='2019-08-16', end_date='2019-08-20')
+    assert set(res.index) == set(['2019-08-16', '2019-08-19', '2019-08-20'])
+    assert set(res.AG) == set(['AG1912.XSGE'])
+    assert set(res.RR) == set(['', 'RR2001.XDCE'])
+    res = get_dominant_future(underlying_symbol=None, date='2019-08-01', end_date='2019-08-10')
+    assert 'RR' not in res.columns
+
 
 def test_get_future_contracts():
     fc = get_future_contracts('IF', datetime.datetime(2016, 9, 12, 10, 0))
     fc_ = get_future_contracts('IF')
     print(fc_)
     assert len(fc) > 0
     cu = get_future_contracts('cu', datetime.datetime(2016, 9, 12, 10, 0))
@@ -1202,14 +1225,52 @@
     assert set(df.index.tolist()) == set(trade_codes)
     assert get_current_tick(["000001.XSHE", "000006.XSHE"]).index.tolist() == ["000001.XSHE", "000006.XSHE"]
     assert get_current_tick("000001.XSHE").index.tolist() == [0]
     with pytest.raises(Exception, match="not support future"):
         get_current_tick(trade_codes + ["AU8888.XSGE"])
 
 
+def test_get_today_tick_period():
+    today_str = str(datetime.date.today())
+    latest_trade_day = str(get_trade_days(end_date=today_str, count=1)[0])
+    codes = get_all_securities('stock', latest_trade_day).index.tolist()[:10]
+    data = get_today_tick_period(codes, end_date=datetime.datetime.now())
+    assert len(data) == 10
+    assert set(data.columns) == set([
+        'datetime', 'current', 'high', 'low', 'volume', 'money',
+        'a1_v', 'a2_v', 'a3_v', 'a4_v', 'a5_v', 'a1_p', 'a2_p', 'a3_p', 'a4_p', 'a5_p',
+        'b1_v', 'b2_v', 'b3_v', 'b4_v', 'b5_v', 'b1_p', 'b2_p', 'b3_p', 'b4_p', 'b5_p'])
+
+    codes = get_all_securities('options', latest_trade_day).index.tolist()[:10]
+    data = get_today_tick_period(codes, end_date=datetime.datetime.now())
+    assert len(data) == 10
+    assert set(data.columns) == set([
+        'datetime', 'current', 'high', 'low', 'volume', 'money', 'position',
+        'a1_v', 'a2_v', 'a3_v', 'a4_v', 'a5_v', 'a1_p', 'a2_p', 'a3_p', 'a4_p', 'a5_p',
+        'b1_v', 'b2_v', 'b3_v', 'b4_v', 'b5_v', 'b1_p', 'b2_p', 'b3_p', 'b4_p', 'b5_p'])
+
+    codes = get_all_securities('futures', latest_trade_day)
+    codes = codes[~codes.index.str.contains(('8888|9999'))].index.tolist()[:10]
+    data = get_today_tick_period(codes, end_date=datetime.datetime.now())
+    assert len(data) == 10
+    assert set(data.columns) == set([
+        'datetime', 'current', 'high', 'low', 'volume', 'money', 'position',
+        'a1_v', 'a1_p', 'b1_v','b1_p'])
+
+    with pytest.raises(Exception):
+        get_today_tick_period(
+            codes,
+            start_date=datetime.datetime.now(),
+            end_date=datetime.datetime.now())
+
+    with pytest.raises(Exception):
+        get_today_tick_period(
+            'AU8888.XSGE',
+            end_date=datetime.datetime.now())
+
 def del_test_get_price_engine():
     df = get_price_engine(["000001.XSHE", "000002.XSHE"], end_date='2018-10-01', count=1, fq=None)
     assert type(df) == pd.core.panel.Panel
     assert df.minor_xs("000001.XSHE").to_json() == ('{"close":{"1538092800000":11.05},"high":{"1538092800000":11.27},'
                                     '"low":{"1538092800000":10.78},"money":{"1538092800000":2331358288.9600000381},'
                                     '"open":{"1538092800000":10.78},"volume":{"1538092800000":211024267.0}}')
     assert get_price_engine(["000001.XSHE", "000002.XSHE"], end_date='2018-10-01', count=1, fq='post',
@@ -1689,15 +1750,15 @@
             'netflow_xl']
     security_list = ['000001.XSHE', '600519.XSHG', '600360.XSHG', '888888.AAA']
     res_1_1 = get_money_flow_pro(security_list,
                                  start_date_1,
                                  end_date_1,
                                  fields=fields)
     print(res_1_1)
-    assert not res_1_1[(start_date_1 < res_1_1.time) & (res_1_1.time < end_date_1)].empty
+    assert not res_1_1[res_1_1.time.between(start_date_1, end_date_1)].empty
     assert '888888.AAA' not in res_1_1.code
 
     res_1_2 = get_money_flow_pro(security_list,
                                  None,
                                  end_date_1,
                                  fields=fields,
                                  count=count_1)
@@ -1709,15 +1770,15 @@
     end_date_2 = datetime.datetime(2023, 9, 10, 16, 0)
     res_2_1 = get_money_flow_pro(security_list,
                                  start_date_2,
                                  end_date_2,
                                  frequency='1m',
                                  fields=fields)
     print(res_2_1)
-    assert not res_2_1[(start_date_2 < res_2_1.time) & (res_2_1.time < end_date_2)].empty
+    assert not res_2_1[res_2_1.time.between(start_date_2, end_date_2)].empty
     assert len(res_2_1) == 3600
     res_2_2 = get_money_flow_pro(security_list,
                                  None,
                                  end_date_2,
                                  frequency='1m',
                                  fields=fields,
                                  count=10)
@@ -1787,12 +1848,17 @@
         'IC2012.CCFX'}
 
     data = get_order_future_bar(symbol='SC',
                                 future_type='4',
                                 start_dt='1999-03-01 09:00:00',
                                 end_dt='2019-02-27 21:30:00',
                                 unit='1m',
-                                fields=['date', 'close', 'volume'])
+                                fields=['code', 'date', 'close', 'volume'])
     assert set(data.columns) == {'date', 'close', 'volume', 'code'}
     assert set(data.code) == {
         'SC1904.XINE', 'SC1903.XINE', 'SC1902.XINE', 'SC1906.XINE',
         'SC1905.XINE', 'SC1901.XINE', 'SC1907.XINE'}
+
+
+def test_get_index_valuation():
+    data = get_index_valuation('932000.CSI', '2024-01-01', '2024-02-01')
+    assert not data.empty
```

### Comparing `jqdatasdk-1.9.4/tests/test_table.py` & `jqdatasdk-1.9.5/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `jqdatasdk-1.9.4/tests/test_utils.py` & `jqdatasdk-1.9.5/tests/test_utils.py`

 * *Files identical despite different names*

