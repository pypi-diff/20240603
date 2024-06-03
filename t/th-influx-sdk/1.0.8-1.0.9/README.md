# Comparing `tmp/th-influx-sdk-1.0.8.tar.gz` & `tmp/th-influx-sdk-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "th-influx-sdk-1.0.8.tar", last modified: Wed May  8 07:22:15 2024, max compression
+gzip compressed data, was "th-influx-sdk-1.0.9.tar", last modified: Mon Jun  3 06:31:15 2024, max compression
```

## Comparing `th-influx-sdk-1.0.8.tar` & `th-influx-sdk-1.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 07:22:15.685640 th-influx-sdk-1.0.8/
--rw-rw-rw-   0        0        0      300 2024-05-08 07:22:15.682648 th-influx-sdk-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       39 2024-04-19 06:33:19.000000 th-influx-sdk-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 07:22:15.666731 th-influx-sdk-1.0.8/ThInfluxSDK/
--rw-rw-rw-   0        0        0       25 2024-04-19 05:50:15.000000 th-influx-sdk-1.0.8/ThInfluxSDK/__init__.py
--rw-rw-rw-   0        0        0    22653 2024-05-08 03:42:11.000000 th-influx-sdk-1.0.8/ThInfluxSDK/influxSDK.py
--rw-rw-rw-   0        0        0       42 2024-05-08 07:22:15.685640 th-influx-sdk-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      553 2024-05-08 07:21:10.000000 th-influx-sdk-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:22:15.679654 th-influx-sdk-1.0.8/th_influx_sdk.egg-info/
--rw-rw-rw-   0        0        0      300 2024-05-08 07:22:15.000000 th-influx-sdk-1.0.8/th_influx_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2024-05-08 07:22:15.000000 th-influx-sdk-1.0.8/th_influx_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 07:22:15.000000 th-influx-sdk-1.0.8/th_influx_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-05-08 07:22:15.000000 th-influx-sdk-1.0.8/th_influx_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-08 07:22:15.000000 th-influx-sdk-1.0.8/th_influx_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-03 06:31:15.727656 th-influx-sdk-1.0.9/
+-rw-rw-rw-   0        0        0      300 2024-06-03 06:31:15.724659 th-influx-sdk-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       39 2024-04-19 06:33:19.000000 th-influx-sdk-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 06:31:15.715667 th-influx-sdk-1.0.9/ThInfluxSDK/
+-rw-rw-rw-   0        0        0       25 2024-04-19 05:50:15.000000 th-influx-sdk-1.0.9/ThInfluxSDK/__init__.py
+-rw-rw-rw-   0        0        0    23891 2024-06-03 06:22:49.000000 th-influx-sdk-1.0.9/ThInfluxSDK/influxSDK.py
+-rw-rw-rw-   0        0        0       42 2024-06-03 06:31:15.727656 th-influx-sdk-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      553 2024-06-03 06:30:16.000000 th-influx-sdk-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 06:31:15.724659 th-influx-sdk-1.0.9/th_influx_sdk.egg-info/
+-rw-rw-rw-   0        0        0      300 2024-06-03 06:31:15.000000 th-influx-sdk-1.0.9/th_influx_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2024-06-03 06:31:15.000000 th-influx-sdk-1.0.9/th_influx_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 06:31:15.000000 th-influx-sdk-1.0.9/th_influx_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-06-03 06:31:15.000000 th-influx-sdk-1.0.9/th_influx_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-06-03 06:31:15.000000 th-influx-sdk-1.0.9/th_influx_sdk.egg-info/top_level.txt
```

### Comparing `th-influx-sdk-1.0.8/ThInfluxSDK/influxSDK.py` & `th-influx-sdk-1.0.9/ThInfluxSDK/influxSDK.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,14 +65,26 @@
     # 使用 dateutil.parser 解析UTC时间字符串
     time = parser.parse(utc_time)
     # 转换为时间戳（毫秒）
     timestamp = int(time.timestamp() * 1000)
     return timestamp
 
 
+def timestamp_to_beijing_time(timestamp):
+    # 将毫秒级时间戳转换为秒级时间戳
+    timestamp_seconds = timestamp / 1000.0
+    # 假设timestamp是自1970年1月1日以来的秒数
+    utc_dt = datetime.utcfromtimestamp(timestamp_seconds)
+    # 将UTC时间转换为北京时间（东八区）
+    beijing_dt = utc_dt + timedelta(hours=8)
+    # 格式化时间字符串
+    formatted_date = beijing_dt.strftime("%Y-%m-%d %H:%M:%S")
+    return formatted_date
+
+
 def utc_time_add_one_day_time(utc_time: str) -> int:
     """
     UTC时间增加一天的时间戳
 
     :param utc_time: 传入的UTC时间, 时间格式：2024-03-13T16:00:00Z
     :return: UTC时间增加一天的时间戳（毫秒）
     """
@@ -167,24 +179,24 @@
         说明：
             本函数可同时满足以下四个场景要求：
             1. 获取一个点的最新值。
             2. 获取一个点在特定时刻的值。
             3. 获取多个点的最新值。
             4. 获取多个点在特定时刻的值。
         """
-    queryTime = convert_beijing_time_to_utc(queryTime)
     # 1. 初始化 resultList
     resultList = []
     # 2. 使用join方法将pointList中的字符串用'|'连接起来
     pointStr = '|'.join(pointList)
     # 3. 构建SQL查询字符串
     SQLForMaxTime = f"SELECT LAST(VALUE), UUID FROM {tableName} WHERE UUID =~ /^{pointStr}$/"
 
     # 4. 如果queryTime不为空，则添加时间条件
     if queryTime is not None and queryTime != "":
+        queryTime = convert_beijing_time_to_utc(queryTime)
         SQLForMaxTime += f" AND time <= '{queryTime}'"
 
     # 5. 执行查询
     queryResult = influxDB.query(SQLForMaxTime, database=database)
 
     # 6. 从查询结果中提取最大的时间戳
     maxTime = ""
@@ -294,16 +306,16 @@
     2、获取一个[点]的[开始，结束]段的[间隔秒]的历史数据;
     3、获取多个[点...] 的[开始，结束] 段的历史数据;
     4、获取多个[点...] 的[开始，结束] 段的[间隔秒] 的历史数据;
 
     Args:
         database (str): 数据库名，必填参数
         tableName (str): 表名，必填参数
-        startTime (str): 开始时间，必填参数，表示使用当前时间。格式应为ISO 8601。
-        endTime (str): 结束时间，必填参数，表示使用当前时间。格式应为ISO 8601。
+        startTime (str): 开始时间，必填参数，表示使用当前时间。
+        endTime (str): 结束时间，必填参数，表示使用当前时间。
         pointList (list of str): 一个或多个点号列表，必填参数，表示查询所有点。
         interval (int, optional): 时间间隔（单位秒），默认为None，表示不使用间隔查询。
         influxDB (InfluxDBClient): InfluxDB连接对象，必填参数，表示使用默认连接。
 
     Returns:
         dict: 包含查询结果的字典，具体结构根据实际应用情况确定。
     """
@@ -327,15 +339,16 @@
     for series in result.raw['series']:
         result_value_map[series['tags']['UUID']] = series['values']
 
     map_record = OrderedDict()
     sb = '['
     index = 0
     for time_stamp in timeList:
-        map_record['time'] = time_stamp  # 添加时间戳
+        dataTimeStr = timestamp_to_beijing_time(time_stamp)
+        map_record['time'] = dataTimeStr  # 添加时间戳
         for point in pointList:
             values_list = result_value_map.get(point)
             if values_list and values_list[index][1]:
                 # 假设 values_list 是一个包含时间戳和值的元组列表
                 map_record[point] = values_list[index][1]
             elif point in map_data:
                 map_record[point] = map_data[point]
@@ -459,26 +472,52 @@
 
     # 构建查询语句
     query = f"SELECT time,VALUE, UUID FROM {tableName} WHERE UUID =~ /{pointStr}/ AND time>='{startTime}' AND time<='{endTime}' "
 
     # 执行查询
     result = influxDB.query(query, database=database)
 
+    od = OrderedDict()
+
+    resultValueMap = OrderedDict()
+
+    map_record = OrderedDict()
+
     # 解析查询结果并提取数据
     result_list = []
     for point in result.get_points():
+        od[point['time']] = point['time']
         obj_list = [point['time'], point['VALUE'], point['UUID']]
         # 获取VALUE和UUID字段的值，假设还有其他字段则继续添加
         result_list.append(obj_list)
+        resultValueMap[point['UUID']+'|'+point['time']] = point['VALUE']
+
+    keys_list = [key for key in od.keys()]
+
+    sb = '['
+    index = 0
+    for time_temp in keys_list:
+        map_record['time'] = convert_utc_to_beijing_time(time_temp)
+        for point in pointList:
+            value = resultValueMap.get(point+'|'+time_temp, '')
+            if value:
+                map_record[point] = value
+            else:
+                map_record[point] = ''
+        if index >= 1:
+            sb += ','
+        sb += json.dumps(map_record)
+        index += 1
 
-    # 将结果转换为JSON字符串
-    json_string = json.dumps(result_list)
+    sb += ']'
+    # # 将结果转换为JSON字符串
+    # json_string = json.dumps(result_list)
 
     # 返回JSON字符串
-    return json_string
+    return sb
 
 
 def write_history_data_to_csv(database: str, tableName: str, startTime: str, endTime: str, pointList: List[str],
                               interval: int,
                               influxDB: InfluxDBClient, filePath: str):
     """
     将历史时间段一个或多个测点数据写入到CSV文件中（进行数据补齐）
```

### Comparing `th-influx-sdk-1.0.8/setup.py` & `th-influx-sdk-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
 
 setup(
     name='th-influx-sdk',
-    version='1.0.8',
+    version='1.0.9',
     description='A SDK for influxDb',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='xiongyi',
     author_email='15679191752@163.com',
     packages=find_packages(),
     install_requires=[
```

