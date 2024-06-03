# Comparing `tmp/menglingtool-1.0.4.tar.gz` & `tmp/menglingtool-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\menglingtool-1.0.4.tar", last modified: Thu Nov 23 01:05:45 2023, max compression
+gzip compressed data, was "menglingtool-1.1.0.tar", last modified: Mon Jun  3 02:07:19 2024, max compression
```

## Comparing `menglingtool-1.0.4.tar` & `menglingtool-1.1.0.tar`

### file list

```diff
@@ -1,37 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-11-23 01:05:45.622509 menglingtool-1.0.4/
--rw-rw-rw-   0        0        0       32 2023-11-10 00:45:33.000000 menglingtool-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      245 2023-11-23 01:05:45.622509 menglingtool-1.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-11-23 01:05:45.613503 menglingtool-1.0.4/menglingtool/
--rw-rw-rw-   0        0        0       40 2023-11-10 05:04:59.000000 menglingtool-1.0.4/menglingtool/__init__.py
--rw-rw-rw-   0        0        0    11948 2020-12-07 01:38:43.000000 menglingtool-1.0.4/menglingtool/calendar.py
-drwxrwxrwx   0        0        0        0 2023-11-23 01:05:45.621511 menglingtool-1.0.4/menglingtool/decorates/
--rw-rw-rw-   0        0        0      406 2023-02-02 05:36:18.000000 menglingtool-1.0.4/menglingtool/decorates/error.py
--rw-rw-rw-   0        0        0      819 2023-02-15 08:38:47.000000 menglingtool-1.0.4/menglingtool/decorates/retry.py
--rw-rw-rw-   0        0        0      501 2023-02-02 05:28:44.000000 menglingtool-1.0.4/menglingtool/decorates/select.py
--rw-rw-rw-   0        0        0      644 2023-02-02 05:29:00.000000 menglingtool-1.0.4/menglingtool/decorates/timeout.py
--rw-rw-rw-   0        0        0     9646 2023-11-10 00:40:05.000000 menglingtool-1.0.4/menglingtool/file.py
--rw-rw-rw-   0        0        0     5469 2022-10-28 02:52:57.000000 menglingtool-1.0.4/menglingtool/goodlib.py
--rw-rw-rw-   0        0        0      312 2023-01-31 09:07:20.000000 menglingtool-1.0.4/menglingtool/hardware.py
--rw-rw-rw-   0        0        0      268 2023-02-02 05:29:49.000000 menglingtool-1.0.4/menglingtool/model.py
--rw-rw-rw-   0        0        0     1924 2022-05-25 03:17:23.000000 menglingtool-1.0.4/menglingtool/net_tool.py
--rw-rw-rw-   0        0        0     5436 2023-11-23 01:05:20.000000 menglingtool-1.0.4/menglingtool/notice.py
--rw-rw-rw-   0        0        0     1103 2023-09-13 01:59:40.000000 menglingtool-1.0.4/menglingtool/pandas_tool.py
--rw-rw-rw-   0        0        0     4237 2022-07-26 06:22:55.000000 menglingtool-1.0.4/menglingtool/pic.py
--rw-rw-rw-   0        0        0     1055 2023-02-15 07:17:03.000000 menglingtool-1.0.4/menglingtool/process.py
--rw-rw-rw-   0        0        0     3147 2023-11-09 13:49:56.000000 menglingtool-1.0.4/menglingtool/progress.py
--rw-rw-rw-   0        0        0      638 2023-08-29 08:19:15.000000 menglingtool-1.0.4/menglingtool/rely.py
--rw-rw-rw-   0        0        0     6243 2022-05-25 03:11:44.000000 menglingtool-1.0.4/menglingtool/tcp.py
--rw-rw-rw-   0        0        0     4459 2023-03-11 08:57:16.000000 menglingtool-1.0.4/menglingtool/thread.py
--rw-rw-rw-   0        0        0     6512 2023-11-10 00:37:58.000000 menglingtool-1.0.4/menglingtool/time_tool.py
--rw-rw-rw-   0        0        0     2580 2022-05-25 03:12:58.000000 menglingtool-1.0.4/menglingtool/udp.py
--rw-rw-rw-   0        0        0    11956 2023-11-13 02:36:50.000000 menglingtool-1.0.4/menglingtool/visualization.py
--rw-rw-rw-   0        0        0     5091 2023-11-10 00:39:58.000000 menglingtool-1.0.4/menglingtool/window_action.py
--rw-rw-rw-   0        0        0      462 2023-11-10 00:40:17.000000 menglingtool-1.0.4/menglingtool/window_notice.py
--rw-rw-rw-   0        0        0     2067 2023-11-10 00:42:01.000000 menglingtool-1.0.4/menglingtool/word.py
-drwxrwxrwx   0        0        0        0 2023-11-23 01:05:45.617499 menglingtool-1.0.4/menglingtool.egg-info/
--rw-rw-rw-   0        0        0      245 2023-11-23 01:05:45.000000 menglingtool-1.0.4/menglingtool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      803 2023-11-23 01:05:45.000000 menglingtool-1.0.4/menglingtool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-23 01:05:45.000000 menglingtool-1.0.4/menglingtool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-11-23 01:05:45.000000 menglingtool-1.0.4/menglingtool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-23 01:05:45.622509 menglingtool-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      715 2023-11-10 06:01:47.000000 menglingtool-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 02:07:19.763000 menglingtool-1.1.0/
+-rw-rw-rw-   0        0        0       32 2024-05-28 08:25:24.000000 menglingtool-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      195 2024-06-03 02:07:19.762006 menglingtool-1.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-03 02:07:19.741059 menglingtool-1.1.0/menglingtool/
+-rw-rw-rw-   0        0        0       40 2024-05-28 08:25:24.000000 menglingtool-1.1.0/menglingtool/__init__.py
+-rw-rw-rw-   0        0        0    11948 2024-05-28 08:25:24.000000 menglingtool-1.1.0/menglingtool/calendar.py
+drwxrwxrwx   0        0        0        0 2024-06-03 02:07:19.760010 menglingtool-1.1.0/menglingtool/decorates/
+-rw-rw-rw-   0        0        0      680 2024-05-28 08:25:24.000000 menglingtool-1.1.0/menglingtool/decorates/console.py
+-rw-rw-rw-   0        0        0      406 2024-05-28 08:25:24.000000 menglingtool-1.1.0/menglingtool/decorates/error.py
+-rw-rw-rw-   0        0        0      819 2024-05-28 08:25:24.000000 menglingtool-1.1.0/menglingtool/decorates/retry.py
+-rw-rw-rw-   0        0        0      501 2024-05-28 08:25:24.000000 menglingtool-1.1.0/menglingtool/decorates/select.py
+-rw-rw-rw-   0        0        0      644 2024-05-28 08:25:24.000000 menglingtool-1.1.0/menglingtool/decorates/timeout.py
+-rw-rw-rw-   0        0        0     9646 2024-05-28 08:25:24.000000 menglingtool-1.1.0/menglingtool/file.py
+-rw-rw-rw-   0        0        0     5560 2024-06-03 01:26:54.000000 menglingtool-1.1.0/menglingtool/goodlib.py
+-rw-rw-rw-   0        0        0     1309 2024-06-03 01:54:39.000000 menglingtool-1.1.0/menglingtool/goodlib2.py
+-rw-rw-rw-   0        0        0      312 2024-05-28 08:25:24.000000 menglingtool-1.1.0/menglingtool/hardware.py
+-rw-rw-rw-   0        0        0      268 2024-05-28 08:25:24.000000 menglingtool-1.1.0/menglingtool/model.py
+-rw-rw-rw-   0        0        0     1924 2024-05-28 08:25:24.000000 menglingtool-1.1.0/menglingtool/net_tool.py
+-rw-rw-rw-   0        0        0     5436 2024-05-28 08:25:24.000000 menglingtool-1.1.0/menglingtool/notice.py
+-rw-rw-rw-   0        0        0     1103 2024-05-28 08:25:24.000000 menglingtool-1.1.0/menglingtool/pandas_tool.py
+-rw-rw-rw-   0        0        0     4237 2024-05-28 08:25:24.000000 menglingtool-1.1.0/menglingtool/pic.py
+-rw-rw-rw-   0        0        0     1055 2024-05-28 08:25:24.000000 menglingtool-1.1.0/menglingtool/process.py
+-rw-rw-rw-   0        0        0     3147 2024-05-28 08:25:24.000000 menglingtool-1.1.0/menglingtool/progress.py
+-rw-rw-rw-   0        0        0     1430 2024-06-03 01:15:47.000000 menglingtool-1.1.0/menglingtool/queue.py
+-rw-rw-rw-   0        0        0      638 2024-05-28 08:25:24.000000 menglingtool-1.1.0/menglingtool/rely.py
+-rw-rw-rw-   0        0        0     6243 2024-05-28 08:25:24.000000 menglingtool-1.1.0/menglingtool/tcp.py
+-rw-rw-rw-   0        0        0     4459 2024-05-28 08:25:24.000000 menglingtool-1.1.0/menglingtool/thread.py
+-rw-rw-rw-   0        0        0     6512 2024-05-28 08:25:24.000000 menglingtool-1.1.0/menglingtool/time_tool.py
+-rw-rw-rw-   0        0        0     2580 2024-05-28 08:25:24.000000 menglingtool-1.1.0/menglingtool/udp.py
+-rw-rw-rw-   0        0        0      717 2024-05-28 08:25:24.000000 menglingtool-1.1.0/menglingtool/video_tool.py
+-rw-rw-rw-   0        0        0    11613 2024-05-28 08:25:24.000000 menglingtool-1.1.0/menglingtool/visualization.py
+-rw-rw-rw-   0        0        0     5091 2024-05-28 08:25:24.000000 menglingtool-1.1.0/menglingtool/window_action.py
+-rw-rw-rw-   0        0        0      462 2024-05-28 08:25:24.000000 menglingtool-1.1.0/menglingtool/window_notice.py
+-rw-rw-rw-   0        0        0     2067 2024-05-28 08:25:24.000000 menglingtool-1.1.0/menglingtool/word.py
+drwxrwxrwx   0        0        0        0 2024-06-03 02:07:19.751058 menglingtool-1.1.0/menglingtool.egg-info/
+-rw-rw-rw-   0        0        0      195 2024-06-03 02:07:19.000000 menglingtool-1.1.0/menglingtool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      911 2024-06-03 02:07:19.000000 menglingtool-1.1.0/menglingtool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 02:07:19.000000 menglingtool-1.1.0/menglingtool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-06-03 02:07:19.000000 menglingtool-1.1.0/menglingtool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 02:07:19.763000 menglingtool-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      715 2024-05-28 08:25:24.000000 menglingtool-1.1.0/setup.py
```

### Comparing `menglingtool-1.0.4/menglingtool/calendar.py` & `menglingtool-1.1.0/menglingtool/calendar.py`

 * *Files identical despite different names*

### Comparing `menglingtool-1.0.4/menglingtool/decorates/retry.py` & `menglingtool-1.1.0/menglingtool/decorates/retry.py`

 * *Files identical despite different names*

### Comparing `menglingtool-1.0.4/menglingtool/decorates/timeout.py` & `menglingtool-1.1.0/menglingtool/decorates/timeout.py`

 * *Files identical despite different names*

### Comparing `menglingtool-1.0.4/menglingtool/file.py` & `menglingtool-1.1.0/menglingtool/file.py`

 * *Files identical despite different names*

### Comparing `menglingtool-1.0.4/menglingtool/goodlib.py` & `menglingtool-1.1.0/menglingtool/goodlib.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from secrets import randbelow
 from threading import get_ident
+import warnings
 
+warnings.warn("goodlib弃用,之后使用goodlib2!", DeprecationWarning)
 
 class Goods:
     def __init__(self, getgoodfunc_kwarg: list, closegoodfunc=lambda g: g.close()):
         self.__key_good = dict()
         self.getGoodFunc, self.kwarg = getgoodfunc_kwarg
         self.closeGoodFunc = closegoodfunc
```

### Comparing `menglingtool-1.0.4/menglingtool/net_tool.py` & `menglingtool-1.1.0/menglingtool/net_tool.py`

 * *Files identical despite different names*

### Comparing `menglingtool-1.0.4/menglingtool/notice.py` & `menglingtool-1.1.0/menglingtool/notice.py`

 * *Files identical despite different names*

### Comparing `menglingtool-1.0.4/menglingtool/pandas_tool.py` & `menglingtool-1.1.0/menglingtool/pandas_tool.py`

 * *Files identical despite different names*

### Comparing `menglingtool-1.0.4/menglingtool/pic.py` & `menglingtool-1.1.0/menglingtool/pic.py`

 * *Files identical despite different names*

### Comparing `menglingtool-1.0.4/menglingtool/process.py` & `menglingtool-1.1.0/menglingtool/process.py`

 * *Files identical despite different names*

### Comparing `menglingtool-1.0.4/menglingtool/progress.py` & `menglingtool-1.1.0/menglingtool/progress.py`

 * *Files identical despite different names*

### Comparing `menglingtool-1.0.4/menglingtool/rely.py` & `menglingtool-1.1.0/menglingtool/rely.py`

 * *Files identical despite different names*

### Comparing `menglingtool-1.0.4/menglingtool/tcp.py` & `menglingtool-1.1.0/menglingtool/tcp.py`

 * *Files identical despite different names*

### Comparing `menglingtool-1.0.4/menglingtool/thread.py` & `menglingtool-1.1.0/menglingtool/thread.py`

 * *Files identical despite different names*

### Comparing `menglingtool-1.0.4/menglingtool/time_tool.py` & `menglingtool-1.1.0/menglingtool/time_tool.py`

 * *Files identical despite different names*

### Comparing `menglingtool-1.0.4/menglingtool/udp.py` & `menglingtool-1.1.0/menglingtool/udp.py`

 * *Files identical despite different names*

### Comparing `menglingtool-1.0.4/menglingtool/visualization.py` & `menglingtool-1.1.0/menglingtool/visualization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,14 @@
 import json
 from math import inf
 import matplotlib.pyplot as plt
 import numpy as np
 import pyecharts.options as opts
 from pyecharts.charts import Line
 
-
-# 获取回归方程系数
-def _huigui(arr):
-    numerator = 0.0
-    denominator = 0.0
-    arr_mean = np.mean(arr, axis=0)
-    for point in arr:
-        dx = point[0] - arr_mean[0]
-        numerator += dx * (point[1] - arr_mean[1])
-        denominator += np.square(dx)
-    a = numerator / denominator
-    b = arr_mean[1] - a * arr_mean[0]
-    return a, b
-
-
 def _getzh(ifcolor=True):
     if ifcolor:
         datas = ['red', 'blue', 'green', 'gold', 'brown',
                  'peru', 'grey', 'pink', 'slategray']
     else:
         datas = ['-', '--', '-.', ':', 'None', 'solid', 'dashed', 'dashdot', 'dotted']
     i = 0
@@ -77,15 +62,15 @@
     # 绘制线
     if loader.linename:
         ax.plot(loader.arr[:, 0], loader.arr[:, 1], linestyle=loader.linestyle,
                 c=loader.line_color)  # 显示点参数设置 marker='o'
 
     plt.grid(linestyle='-.')
     if loader.ifhuigui:
-        a, b = _huigui(loader.arr)
+        a, b = np.polyfit(loader.arr[:, 0], loader.arr[:, 1], 1)
         ax.plot([loader.arr[0, 0], loader.arr[-1, 0]], [a * loader.arr[0, 0] + b, a * loader.arr[-1, 0] + b],
                 color='black')
     # 根据密度对点进行稀疏处理
     n = int(1 / loader.md)
     xs, ys, texts = [], [], []
     for i in range(0, loader.arr.shape[0], n):
         if loader.texts:
```

### Comparing `menglingtool-1.0.4/menglingtool/window_action.py` & `menglingtool-1.1.0/menglingtool/window_action.py`

 * *Files identical despite different names*

### Comparing `menglingtool-1.0.4/menglingtool/word.py` & `menglingtool-1.1.0/menglingtool/word.py`

 * *Files identical despite different names*

### Comparing `menglingtool-1.0.4/menglingtool.egg-info/SOURCES.txt` & `menglingtool-1.1.0/menglingtool.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 MANIFEST.in
 setup.py
 menglingtool/__init__.py
 menglingtool/calendar.py
 menglingtool/file.py
 menglingtool/goodlib.py
+menglingtool/goodlib2.py
 menglingtool/hardware.py
 menglingtool/model.py
 menglingtool/net_tool.py
 menglingtool/notice.py
 menglingtool/pandas_tool.py
 menglingtool/pic.py
 menglingtool/process.py
 menglingtool/progress.py
+menglingtool/queue.py
 menglingtool/rely.py
 menglingtool/tcp.py
 menglingtool/thread.py
 menglingtool/time_tool.py
 menglingtool/udp.py
+menglingtool/video_tool.py
 menglingtool/visualization.py
 menglingtool/window_action.py
 menglingtool/window_notice.py
 menglingtool/word.py
 menglingtool.egg-info/PKG-INFO
 menglingtool.egg-info/SOURCES.txt
 menglingtool.egg-info/dependency_links.txt
 menglingtool.egg-info/top_level.txt
+menglingtool/decorates/console.py
 menglingtool/decorates/error.py
 menglingtool/decorates/retry.py
 menglingtool/decorates/select.py
 menglingtool/decorates/timeout.py
```

### Comparing `menglingtool-1.0.4/setup.py` & `menglingtool-1.1.0/setup.py`

 * *Files identical despite different names*

