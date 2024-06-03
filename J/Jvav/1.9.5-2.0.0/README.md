# Comparing `tmp/Jvav-1.9.5.tar.gz` & `tmp/Jvav-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/zh/Codes/jvav/dist/.tmp-qjz87kh5/Jvav-1.9.5.tar", last modified: Sat Jun  1 04:30:55 2024, max compression
+gzip compressed data, was "/Users/zh/Codes/jvav/dist/.tmp-fezxj5tn/Jvav-2.0.0.tar", last modified: Mon Jun  3 05:35:48 2024, max compression
```

## Comparing `Jvav-1.9.5.tar` & `Jvav-2.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-06-01 04:30:55.000000 Jvav-1.9.5/
-drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-06-01 04:30:55.000000 Jvav-1.9.5/Jvav.egg-info/
--rw-r--r--   0 zh         (501) staff       (20)     4311 2024-06-01 04:30:55.000000 Jvav-1.9.5/Jvav.egg-info/PKG-INFO
--rw-r--r--   0 zh         (501) staff       (20)      295 2024-06-01 04:30:55.000000 Jvav-1.9.5/Jvav.egg-info/SOURCES.txt
--rw-r--r--   0 zh         (501) staff       (20)        1 2024-06-01 04:30:55.000000 Jvav-1.9.5/Jvav.egg-info/dependency_links.txt
--rw-r--r--   0 zh         (501) staff       (20)       39 2024-06-01 04:30:55.000000 Jvav-1.9.5/Jvav.egg-info/entry_points.txt
--rw-r--r--   0 zh         (501) staff       (20)        1 2023-07-18 10:13:18.000000 Jvav-1.9.5/Jvav.egg-info/not-zip-safe
--rw-r--r--   0 zh         (501) staff       (20)      579 2024-06-01 04:30:55.000000 Jvav-1.9.5/Jvav.egg-info/requires.txt
--rw-r--r--   0 zh         (501) staff       (20)       11 2024-06-01 04:30:55.000000 Jvav-1.9.5/Jvav.egg-info/top_level.txt
--rw-r--r--   0 zh         (501) staff       (20)    35149 2023-07-16 04:15:06.000000 Jvav-1.9.5/LICENSE
--rw-r--r--   0 zh         (501) staff       (20)      108 2023-07-16 04:15:06.000000 Jvav-1.9.5/MANIFEST.in
--rw-r--r--   0 zh         (501) staff       (20)     4311 2024-06-01 04:30:55.000000 Jvav-1.9.5/PKG-INFO
--rw-r--r--   0 zh         (501) staff       (20)     3581 2024-04-21 15:00:39.000000 Jvav-1.9.5/README.md
-drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-06-01 04:30:55.000000 Jvav-1.9.5/jvav/
--rw-r--r--   0 zh         (501) staff       (20)      481 2024-06-01 04:30:31.000000 Jvav-1.9.5/jvav/__init__.py
--rw-r--r--   0 zh         (501) staff       (20)     7578 2024-02-16 02:42:42.000000 Jvav-1.9.5/jvav/cmd.py
--rw-r--r--   0 zh         (501) staff       (20)    76575 2024-06-01 04:29:47.000000 Jvav-1.9.5/jvav/utils.py
--rw-r--r--   0 zh         (501) staff       (20)      579 2024-05-31 16:49:11.000000 Jvav-1.9.5/requirements.txt
--rw-r--r--   0 zh         (501) staff       (20)       38 2024-06-01 04:30:55.000000 Jvav-1.9.5/setup.cfg
--rw-r--r--   0 zh         (501) staff       (20)     1345 2024-06-01 04:30:31.000000 Jvav-1.9.5/setup.py
+drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-06-03 05:35:48.000000 Jvav-2.0.0/
+drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-06-03 05:35:48.000000 Jvav-2.0.0/Jvav.egg-info/
+-rw-r--r--   0 zh         (501) staff       (20)     4311 2024-06-03 05:35:48.000000 Jvav-2.0.0/Jvav.egg-info/PKG-INFO
+-rw-r--r--   0 zh         (501) staff       (20)      295 2024-06-03 05:35:48.000000 Jvav-2.0.0/Jvav.egg-info/SOURCES.txt
+-rw-r--r--   0 zh         (501) staff       (20)        1 2024-06-03 05:35:48.000000 Jvav-2.0.0/Jvav.egg-info/dependency_links.txt
+-rw-r--r--   0 zh         (501) staff       (20)       39 2024-06-03 05:35:48.000000 Jvav-2.0.0/Jvav.egg-info/entry_points.txt
+-rw-r--r--   0 zh         (501) staff       (20)        1 2023-07-18 10:13:18.000000 Jvav-2.0.0/Jvav.egg-info/not-zip-safe
+-rw-r--r--   0 zh         (501) staff       (20)      579 2024-06-03 05:35:48.000000 Jvav-2.0.0/Jvav.egg-info/requires.txt
+-rw-r--r--   0 zh         (501) staff       (20)       11 2024-06-03 05:35:48.000000 Jvav-2.0.0/Jvav.egg-info/top_level.txt
+-rw-r--r--   0 zh         (501) staff       (20)    35149 2023-07-16 04:15:06.000000 Jvav-2.0.0/LICENSE
+-rw-r--r--   0 zh         (501) staff       (20)      108 2023-07-16 04:15:06.000000 Jvav-2.0.0/MANIFEST.in
+-rw-r--r--   0 zh         (501) staff       (20)     4311 2024-06-03 05:35:48.000000 Jvav-2.0.0/PKG-INFO
+-rw-r--r--   0 zh         (501) staff       (20)     3581 2024-04-21 15:00:39.000000 Jvav-2.0.0/README.md
+drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-06-03 05:35:48.000000 Jvav-2.0.0/jvav/
+-rw-r--r--   0 zh         (501) staff       (20)      455 2024-06-03 05:35:04.000000 Jvav-2.0.0/jvav/__init__.py
+-rw-r--r--   0 zh         (501) staff       (20)     7578 2024-02-16 02:42:42.000000 Jvav-2.0.0/jvav/cmd.py
+-rw-r--r--   0 zh         (501) staff       (20)    77436 2024-06-03 05:34:21.000000 Jvav-2.0.0/jvav/utils.py
+-rw-r--r--   0 zh         (501) staff       (20)      579 2024-05-31 16:49:11.000000 Jvav-2.0.0/requirements.txt
+-rw-r--r--   0 zh         (501) staff       (20)       38 2024-06-03 05:35:48.000000 Jvav-2.0.0/setup.cfg
+-rw-r--r--   0 zh         (501) staff       (20)     1345 2024-06-03 05:35:04.000000 Jvav-2.0.0/setup.py
```

### Comparing `Jvav-1.9.5/Jvav.egg-info/PKG-INFO` & `Jvav-2.0.0/Jvav.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jvav
-Version: 1.9.5
+Version: 2.0.0
 Summary: Useful tools for Jav.
 Home-page: https://github.com/akynazh/jvav
 Download-URL: https://github.com/akynazh/jvav/releases/latest
 Author: akynazh
 Author-email: akynazh@gmail.com
 License: GPLv3
 Project-URL: Tracker, https://github.com/akynazh/jvav/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Jvav Version: 1.9.5 Summary: Useful tools for Jav.
+Metadata-Version: 2.1 Name: Jvav Version: 2.0.0 Summary: Useful tools for Jav.
 Home-page: https://github.com/akynazh/jvav Download-URL: https://github.com/
 akynazh/jvav/releases/latest Author: akynazh Author-email: akynazh@gmail.com
 License: GPLv3 Project-URL: Tracker, https://github.com/akynazh/jvav/issues
 Project-URL: Source, https://github.com/akynazh/jvav Keywords: jav japan av api
 library python spider Classifier: License :: OSI Approved :: GNU General Public
 License v3 (GPLv3) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Topic :: Internet :: WWW/HTTP
```

### Comparing `Jvav-1.9.5/Jvav.egg-info/requires.txt` & `Jvav-2.0.0/Jvav.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Jvav-1.9.5/LICENSE` & `Jvav-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Jvav-1.9.5/PKG-INFO` & `Jvav-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jvav
-Version: 1.9.5
+Version: 2.0.0
 Summary: Useful tools for Jav.
 Home-page: https://github.com/akynazh/jvav
 Download-URL: https://github.com/akynazh/jvav/releases/latest
 Author: akynazh
 Author-email: akynazh@gmail.com
 License: GPLv3
 Project-URL: Tracker, https://github.com/akynazh/jvav/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Jvav Version: 1.9.5 Summary: Useful tools for Jav.
+Metadata-Version: 2.1 Name: Jvav Version: 2.0.0 Summary: Useful tools for Jav.
 Home-page: https://github.com/akynazh/jvav Download-URL: https://github.com/
 akynazh/jvav/releases/latest Author: akynazh Author-email: akynazh@gmail.com
 License: GPLv3 Project-URL: Tracker, https://github.com/akynazh/jvav/issues
 Project-URL: Source, https://github.com/akynazh/jvav Keywords: jav japan av api
 library python spider Classifier: License :: OSI Approved :: GNU General Public
 License v3 (GPLv3) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Topic :: Internet :: WWW/HTTP
```

### Comparing `Jvav-1.9.5/README.md` & `Jvav-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `Jvav-1.9.5/jvav/cmd.py` & `Jvav-2.0.0/jvav/cmd.py`

 * *Files identical despite different names*

### Comparing `Jvav-1.9.5/jvav/utils.py` & `Jvav-2.0.0/jvav/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: UTF-8 -*-
 import concurrent.futures
 import logging
 import random
 import re
-import typing
+from typing import Tuple, Union, List, Any, Dict
 
 import requests
 import requests_cache
 import unicodedata
 import wikipediaapi
 from anti_useragent import UserAgent
 from bs4 import BeautifulSoup
@@ -53,15 +53,15 @@
 
         :return str: UserAgent
         """
         return UserAgent().random
 
     def _inner_send_req(
             self, url: str, session, headers={}, proxies={}, m=0, **args
-    ) -> typing.Tuple[int, requests.Response]:
+    ) -> Union[Tuple[int, None], Tuple[int, Any]]:
         if headers == {}:
             headers = {"user-agent": self.ua()}
         if proxies == {}:
             proxies = self.proxy_json
         try:
             if m == 0:
                 resp = session.get(url, proxies=proxies, headers=headers, **args)
@@ -76,15 +76,15 @@
             return 200, resp
         except Exception as e:
             self.log.error(f"BaseUtil: 访问 {url}: {e}")
             return 502, None
 
     def send_req(
             self, url: str, headers={}, proxies={}, m=0, **args
-    ) -> typing.Tuple[int, requests.Response]:
+    ) -> Tuple[int, requests.Response]:
         """发送请求
 
         :param str url: 地址
         :param dict headers: 请求头, 默认使用随机请求头
         :param dict proxies: 代理字典, 默认使用类初始化时指定的代理进行配置
         :param int m: 请求方法, 默认为 get(0), 其他为 post(1), delete(2), put(3)
         :param dict args: 其他 requests 参数
@@ -116,67 +116,70 @@
             f.write(resp.text)
 
 
 class RankUtil(BaseUtil):
     BASE_URL_AV_RANK = "https://gist.githubusercontent.com/jinjier/7a405fad753f996d85ed43073e3bf009/raw/29bf7a4635c1283a1415aad9fb335f92ece2972b/250.csv"
     BASE_URL_STAR_RANK = ""  # DmmUtil supports
 
-    def random_get_av_from_rank(self) -> typing.Tuple[int, str]:
+    def random_get_av_from_rank(self) -> Tuple[int, str]:
         """从排行榜随机获取一个番号
 
         :return tuple[int, str]: 状态码和番号
         """
         code, resp = self.send_req(self.BASE_URL_AV_RANK)
         if code != 200:
             return code, None
         lines = str(resp.text).splitlines()
         id = lines[random.randint(0, len(lines) - 1)].split(",")[1]
         return 200, id
 
-    def get_av_250_rank(self) -> typing.Tuple[int, list]:
+    def get_av_250_rank(self) -> Tuple[int, list]:
         """获取 av 排行榜
 
         :return tuple[int, list]: 状态码和番号列表
         """
         code, resp = self.send_req(self.BASE_URL_AV_RANK)
         if code != 200:
             return code, None
         lines = str(resp.text).splitlines()
         return 200, [line.split(",")[1] for line in lines]
 
 
 class JavDbUtil(BaseUtil):
     BASE_URL = "https://javdb.com"
-    BASE_URL_NEW_AV = BASE_URL + "/?vft=1&vst=1"
-    BASE_URL_SEARCH = BASE_URL + "/search?q="
-    BASE_URL_VIDEO = BASE_URL + "/v/"
-    BASE_URL_ACTOR = BASE_URL + "/actors/"
-    BASE_URL_SEARCH_STAR = BASE_URL + "/search?f=actor&q="
     BASE_PARAM_NICE_AVS_OF_STAR = "?sort_type=1"
     PAT_SCORE = re.compile(r"(\d+\.?\d+)分")
 
     def __init__(
             self,
             proxy_addr="",
             use_cache=True,
             max_home_page_count=100,
             max_new_avs_count=8,
+            base_url=BASE_URL,
     ):
         """初始化
 
         :param str proxy_addr: 代理服务器地址, 默认为 ''
         :param bool use_cache: 是否使用缓存, 默认为 True
         :param int max_home_page_count: 主页最大爬取页数, 默认为 100 页
         :param int max_new_avs_count: 获取最新 AV 数量, 默认为 8 部
+        :param str base_url: 基础地址, 默认为 BASE_URL
         """
         super().__init__(proxy_addr, use_cache)
+        self.base_url = base_url
+        self.base_url_new_av = self.base_url + "/?vft=1&vst=1"
+        self.base_url_search = self.base_url + "/search?q="
+        self.base_url_video = self.base_url + "/v/"
+        self.base_url_actor = self.base_url + "/actors/"
+        self.base_url_search_star = self.base_url + "/search?f=actor&q="
         self.max_home_page_count = max_home_page_count
         self.max_new_avs_count = max_new_avs_count
 
-    def get_max_page(self, url: str) -> typing.Tuple[int, int]:
+    def get_max_page(self, url: str) -> Union[Tuple[int, None], Tuple[int, int]]:
         """获取最大页数
 
         :param str url: 页面地址
         :return tuple[int, int]: 状态码和最大页数
         """
         code, resp = self.send_req(url)
         if code != 200:
@@ -189,26 +192,26 @@
             if not last_page:
                 return 404, None
             return 200, last_page
         except Exception as e:
             self.log.error(f"JavDbUtil: 从 {url} 获取最大页数: {e}")
             return 404, None
 
-    def get_new_ids(self) -> typing.Tuple[int, list]:
+    def get_new_ids(self) -> Tuple[int, any]:
         """获取最新的番号列表
 
-        :return typing.Tuple[int, list]: 状态码和番号列表
+        :return Tuple[int, list]: 状态码和番号列表
         """
-        return self.get_ids_from_page(self.BASE_URL_NEW_AV)
+        return self.get_ids_from_page(self.base_url_new_av)
 
-    def get_ids_from_page(self, url: str) -> typing.Tuple[int, list]:
+    def get_ids_from_page(self, url: str) -> Union[Tuple[int, None], Tuple[int, List[Any]]]:
         """从页面 url 获取番号列表
 
         :param str url: 首页/搜索页
-        :return typing.Tuple[int, list]: 状态码和番号列表
+        :return Tuple[int, list]: 状态码和番号列表
         """
         code, resp = self.send_req(url=url)
         if code != 200:
             return code, None
         try:
             soup = self.get_soup(resp)
             items = soup.find_all(class_="item")
@@ -218,35 +221,35 @@
             if not ids:
                 return 404, None
             return 200, ids
         except Exception as e:
             self.log.error(f"JavDbUtil: 从页面获取番号列表: {e}")
             return 404, None
 
-    def get_star_page_by_star_name(self, star_name):
-        code, resp = self.send_req(url=JavDbUtil.BASE_URL_SEARCH_STAR + star_name)
+    def get_star_page_by_star_name(self, star_name) -> Union[Tuple[int, None], Tuple[int, str]]:
+        code, resp = self.send_req(url=self.base_url_search_star + star_name)
         if code != 200:
             return code, None
         try:
             soup = self.get_soup(resp)
             url = soup.find(class_="actor-box").find("a").attrs["href"]
             if not url:
                 return 404, None
-            return 200, f"{self.BASE_URL}{url}"
+            return 200, f"{self.base_url}{url}"
         except Exception as e:
             self.log.error(f"JavDbUtil: 获取预览图片: {e}")
             return 404, None
 
-    def fuzzy_search_stars(self, text) -> typing.Tuple[int, any]:
+    def fuzzy_search_stars(self, text) -> Union[Tuple[int, None], Tuple[int, List[Any]]]:
         """模糊搜索演员
 
         :param str text: 演员名称
-        :return typing.Tuple[int, list]: 状态码和演员列表
+        :return Tuple[int, list]: 状态码和演员列表
         """
-        code, resp = self.send_req(url=JavDbUtil.BASE_URL_SEARCH_STAR + text)
+        code, resp = self.send_req(url=self.base_url_search_star + text)
         if code != 200:
             return code, None
         try:
             soup = self.get_soup(resp)
             actor_boxs = soup.find_all(class_="actor-box")
             names = [box.find("a")["title"] for box in actor_boxs]
             if not names:
@@ -254,27 +257,28 @@
             names = [name.split(',')[0] for name in names]
             names = list(set(names))
             return 200, names
         except Exception as e:
             self.log.error(f"JavDbUtil: 模糊搜索演员: {e}")
             return 404, None
 
-    def get_id_by_star_name(self, star_name: str, page=-1) -> typing.Tuple[int, str]:
+    def get_id_by_star_name(self, star_name: str, page=-1) -> Union[Tuple[int, None], Tuple[int, Any]]:
         """根据演员名称获取一个番号
 
         :param str star_name: 演员名称
         :param int page: 用于指定爬取哪一页的数据, 默认值为 -1, 表示随机获取某一页
         :return tuple[int, str]: 状态码和番号
         """
         code, ids = self.get_ids_by_star_name(star_name, page)
         if code != 200:
             return code, None
         return 200, random.choice(ids)
 
-    def get_ids_by_star_name(self, star_name: str, page=-1) -> typing.Tuple[int, list]:
+    def get_ids_by_star_name(self, star_name: str, page=-1) -> Union[
+        Tuple[Any, None], Tuple[int, Any], Tuple[int, None]]:
         """根据演员名称获取一批番号
 
         :param str star_name: 演员名称
         :param int page: 用于指定爬取哪一页的数据, 默认值为 -1, 表示随机获取某一页
         :return tuple[int, list]: 状态码和番号
         """
         code, base_page_url = self.get_star_page_by_star_name(star_name)
@@ -292,19 +296,19 @@
             if code != 200:
                 return code, None
             return 200, ids
         except Exception as e:
             self.log.error(f"JavDbUtil: 根据演员名称获取一个番号: {e}")
             return 404, None
 
-    def get_new_ids_by_star_name(self, star_name: str) -> typing.Tuple[int, list]:
+    def get_new_ids_by_star_name(self, star_name: str) -> Union[Tuple[Any, None], Tuple[int, Any], Tuple[int, None]]:
         """根据演员名字获取最新番号列表
 
         :param str star_name: 演员名称
-        :return typing.Tuple[int, list]: 状态码和番号列表
+        :return Tuple[int, list]: 状态码和番号列表
         """
         code, url = self.get_star_page_by_star_name(star_name)
         if code != 200:
             return code, None
         try:
             code, ids = self.get_ids_from_page(url)
             if code != 200:
@@ -312,20 +316,20 @@
             return 200, ids[: self.max_new_avs_count]
         except Exception as e:
             self.log.error(f"JavDbUtil: 根据演员名字获取最新番号列表: {e}")
             return 404, None
 
     def get_nice_avs_by_star_name(
             self, star_name: str, cookie: str
-    ) -> typing.Tuple[int, list]:
+    ) -> Union[Tuple[Any, None], Tuple[int, None], Tuple[int, List[Dict[str, Union[str, Any]]]]]:
         """根据演员名字获取高分番号列表(需要登录)
 
         :param str star_name: 演员名字
         :param str cookie: 该方法需要登录，cookie 中的 _jdb_session 为必须值
-        :return typing.Tuple[int, list]: 状态码和番号列表
+        :return Tuple[int, list]: 状态码和番号列表
         番号列表单个对象结构:
         {
             'rate': rate, # 评分
             'id': id # 番号
         }
         """
         code, base_page_url = self.get_star_page_by_star_name(star_name)
@@ -356,39 +360,39 @@
             if not res:
                 return 404, None
             return 200, res
         except Exception as e:
             self.log.error(f"JavDbUtil: 从页面获取番号列表: {e}")
             return 404, None
 
-    def get_javdb_id_by_id(self, id: str) -> typing.Tuple[int, str]:
+    def get_javdb_id_by_id(self, id: str) -> Union[Tuple[int, None], Tuple[int, Any]]:
         """通过番号获取 JavDB 内部 ID
 
         :param id: 番号
-        :return: tuple[int, None] 状态码和 JavDB 内部 ID
+        :return: tuple[int, str] 状态码和 JavDB 内部 ID
         """
-        code, resp = self.send_req(url=JavDbUtil.BASE_URL_SEARCH + id)
+        code, resp = self.send_req(url=self.base_url_search + id)
         if code != 200:
             return code, None
         try:
             soup = self.get_soup(resp)
             items = soup.find_all(class_="item")
             for item in items:
                 if item.find(class_="video-title").strong.text.strip() == id.upper():
                     return 200, item.find("a")["href"].split("/")[-1]
             return 404, None  # if there is no correct result, return 404
         except Exception as e:
             self.log.error(f"JavDbUtil: 通过番号获取JavDB内部ID: {e}")
             return 404, None
 
-    def get_javdb_ids_from_page(self, url: str) -> typing.Tuple[int, list]:
+    def get_javdb_ids_from_page(self, url: str) -> Union[Tuple[int, None], Tuple[int, List[Any]]]:
         """从页面 url 获取 JavDB 的 ID 列表
 
         :param url: 首页/搜索页
-        :return: typing.Tuple[int, list]: 状态码和 JavDB 的 ID 列表
+        :return: Tuple[int, list]: 状态码和 JavDB 的 ID 列表
         """
         code, resp = self.send_req(url=url)
         if code != 200:
             return code, None
         try:
             soup = self.get_soup(resp)
             items = soup.find_all(class_="item")
@@ -396,140 +400,140 @@
             if not ids:
                 return 404, None
             return 200, ids
         except Exception as e:
             self.log.error(f"JavDbUtil: 从页面获取 JavDB 内部 ID 列表: {e}")
             return 404, None
 
-    def get_id_from_home(self) -> typing.Tuple[int, str]:
+    def get_id_from_home(self) -> Union[Tuple[Any, None], Tuple[int, Any]]:
         """从主页获取一个番号(随机选取) 从首页获取 ID 或 JavDB ID
 
-        :return typing.Tuple[int, str]: 状态码和番号
+        :return Tuple[int, str]: 状态码和番号
         """
-        code, resp = self.get_ids_from_page(url=JavDbUtil.BASE_URL)
+        code, resp = self.get_ids_from_page(url=self.base_url)
         if code != 200:
             return code, None
         else:
             return 200, random.choice(resp)
 
-    def get_javdb_id_from_home(self) -> typing.Tuple[int, str]:
+    def get_javdb_id_from_home(self) -> Union[Tuple[Any, None], Tuple[int, Any]]:
         """从主页获取一个 JavDB 内部 ID (随机选取)
 
-        :return typing.Tuple[int, str]: 状态码和 JavDB 内部 ID
+        :return Tuple[int, str]: 状态码和 JavDB 内部 ID
         """
-        code, resp = self.get_javdb_ids_from_page(url=JavDbUtil.BASE_URL)
+        code, resp = self.get_javdb_ids_from_page(url=self.base_url)
         if code != 200:
             return code, None
         else:
             return 200, random.choice(resp)
 
-    def get_ids_from_home(self) -> typing.Tuple[int, list]:
+    def get_ids_from_home(self) -> Union[Tuple[Any, None], Tuple[int, Any]]:
         """从主页获取全部番号
 
-        :return typing.Tuple[int, list]: 状态码和番号列表
+        :return Tuple[int, list]: 状态码和番号列表
         """
-        code, resp = self.get_ids_from_page(url=JavDbUtil.BASE_URL)
+        code, resp = self.get_ids_from_page(url=self.base_url)
         if code != 200:
             return code, None
         else:
             return 200, resp
 
-    def get_javdb_ids_from_home(self) -> typing.Tuple[int, list]:
+    def get_javdb_ids_from_home(self) -> Union[Tuple[Any, None], Tuple[int, Any]]:
         """从主页获取全部 JavDB 内部 ID
 
-        :return typing.Tuple[int, list]: 状态码和 JavDB 内部 ID 列表
+        :return Tuple[int, list]: 状态码和 JavDB 内部 ID 列表
         """
-        code, resp = self.get_javdb_ids_from_page(url=JavDbUtil.BASE_URL)
+        code, resp = self.get_javdb_ids_from_page(url=self.base_url)
         if code != 200:
             return code, None
         else:
             return 200, resp
 
-    def get_ids_by_tag(self, tag: str) -> typing.Tuple[int, list]:
+    def get_ids_by_tag(self, tag: str) -> Tuple[int, list]:
         """根据标签获取番号列表
 
         :param str tag: 标签
-        :return typing.Tuple[int, list]: 状态码和番号列表
+        :return Tuple[int, list]: 状态码和番号列表
         """
-        url = f"{JavDbUtil.BASE_URL_SEARCH}{tag}"
+        url = f"{self.base_url_search}{tag}"
         return self.get_ids_from_page(url)
 
-    def get_javdb_ids_by_tag(self, tag: str) -> typing.Tuple[int, list]:
+    def get_javdb_ids_by_tag(self, tag: str) -> Tuple[int, list]:
         """根据标签获取 JavDB 列表
 
         :param str tag: 标签
-        :return typing.Tuple[int, list]: 状态码和番号列表
+        :return Tuple[int, list]: 状态码和番号列表
         """
-        url = f"{JavDbUtil.BASE_URL_SEARCH}{tag}"
+        url = f"{self.base_url_search}{tag}"
         return self.get_javdb_ids_from_page(url)
 
-    def get_cover_by_id(self, id: str) -> typing.Tuple[int, str]:
+    def get_cover_by_id(self, id: str) -> Union[Tuple[int, None], Tuple[int, Any]]:
         """根据番号获取封面
 
         :param str id: 番号
-        :return typing.Tuple[int, str]: 状态码和封面
+        :return Tuple[int, str]: 状态码和封面
         """
-        code, resp = self.send_req(url=JavDbUtil.BASE_URL_SEARCH + id)
+        code, resp = self.send_req(url=self.base_url_search + id)
         if code != 200:
             return code, None
         try:
             soup = self.get_soup(resp)
             items = soup.find_all(class_="item")
             for item in items:
                 if item.find(class_="video-title").strong.text.strip() == id.upper():
                     return 200, item.find("img")["src"]
             else:
                 return 404, None
         except Exception as e:
             self.log.error(f"JavDbUtil: 通过番号获取封面: {e}")
             return 404, None
 
-    def get_cover_by_javdb_id(self, javdb_id: str) -> typing.Tuple[int, str]:
+    def get_cover_by_javdb_id(self, javdb_id: str) -> Union[Tuple[int, None], Tuple[int, Union[str, Any]]]:
         """通过 JavDB ID 获取封面
 
         :param str javdb_id: JavDB 内部 ID
-        :return typing.Tuple[int, str]: 状态码和封面
+        :return Tuple[int, str]: 状态码和封面
         """
-        code, resp = self.send_req(url=JavDbUtil.BASE_URL_VIDEO + javdb_id)
+        code, resp = self.send_req(url=self.base_url_video + javdb_id)
         if code != 200:
             return code, None
         try:
             soup = self.get_soup(resp)
             cover = soup.find(class_="column column-video-cover")
             if not cover:
                 return 404, None
             return 200, cover.find("img")["src"]
         except Exception as e:
             self.log.error(f"JavDbUtil: 通过JavDB ID获取封面: {e}")
             return 404, None
 
-    def get_pv_by_id(self, id: str):
+    def get_pv_by_id(self, id: str) -> Union[Tuple[Any, None], Tuple[int, None], Tuple[int, Union[str, Any]]]:
         code, j_id = self.get_javdb_id_by_id(id)
         if code != 200:
             return code, None
-        code, resp = self.send_req(url=JavDbUtil.BASE_URL_VIDEO + j_id)
+        code, resp = self.send_req(url=self.base_url_video + j_id)
         if code != 200:
             return code, None
         try:
             soup = self.get_soup(resp)
             url = soup.find(id="preview-video").find("source").attrs["src"]
             if not url:
                 return 404, None
             if "http" not in url:
                 url = f"https:{url}"
             return 200, url
         except Exception as e:
             self.log.error(f"JavDbUtil: 获取预览视频: {e}")
             return 404, None
 
-    def get_samples_by_id(self, id: str):
+    def get_samples_by_id(self, id: str) -> Union[Tuple[Any, None], Tuple[int, None], Tuple[int, List[Any]]]:
         code, j_id = self.get_javdb_id_by_id(id)
         if code != 200:
             return code, None
-        code, resp = self.send_req(url=JavDbUtil.BASE_URL_VIDEO + j_id)
+        code, resp = self.send_req(url=self.base_url_video + j_id)
         if code != 200:
             return code, None
         try:
             soup = self.get_soup(resp)
             img_tags = soup.find_all(class_="tile-item")
             if not img_tags:
                 return 404, None
@@ -541,23 +545,23 @@
     def get_av_by_javdb_id(
             self,
             javdb_id: str,
             is_nice: bool,
             is_uncensored: bool,
             sex_limit: bool = False,
             magnet_max_count=10,
-    ) -> typing.Tuple[int, dict]:
+    ) -> Tuple[int, any]:
         """通过 JavDB ID 获取 av
 
         :param javdb_id: JavDB 内部 ID
         :param bool is_nice: 是否过滤出高清，有字幕磁链
         :param bool is_uncensored: 是否过滤出无码磁链
         :param bool sex_limit: 是否只获取女优信息
         :param int magnet_max_count: 过滤后磁链的最大数目, 默认为 10
-        :return typing.Tuple[int, dict]: 状态码和 av
+        :return Tuple[int, any]: 状态码和 av
         av格式:
         {
             'id': '',       # 番号
             'date': '',     # 发行日期
             'title': '',    # 标题
             'title_cn': '', # 中文标题
             'img': '',      # 封面地址
@@ -583,15 +587,15 @@
         演员格式:
         {
             'name': '', # 演员名称
             'id': ''    # 演员编号
             'sex': ''   # 演员性别
         }
         """
-        code, resp = self.send_req(url=JavDbUtil.BASE_URL_VIDEO + javdb_id)
+        code, resp = self.send_req(url=self.base_url_video + javdb_id)
         if code != 200:
             return code, None
         try:
             av = {
                 "id": "",
                 "date": "",
                 "img": "",
@@ -601,15 +605,15 @@
                 "producer": "",
                 "publisher": "",
                 "series": "",
                 "score": "",
                 "tags": [],
                 "stars": [],
                 "magnets": [],
-                "url": JavDbUtil.BASE_URL_VIDEO + javdb_id,
+                "url": self.base_url_video + javdb_id,
             }
             soup = self.get_soup(resp)
             # 获取元信息
             title_cn = soup.find("strong", {"class": "current-title"})
             title = soup.find("span", {"class": "origin-title"})
             if not title:
                 title, title_cn = title_cn, ""
@@ -722,22 +726,22 @@
     def get_av_by_id(
             self,
             id: str,
             is_nice: bool,
             is_uncensored: bool,
             sex_limit: bool = False,
             magnet_max_count=10,
-    ) -> typing.Tuple[int, dict]:
+    ) -> Tuple[int, any]:
         """通过 javdb 获取番号对应 av
 
         :param str id: 番号
         :param bool is_nice: 是否过滤出高清，有字幕磁链
         :param bool is_uncensored: 是否过滤出无码磁链
         :param int magnet_max_count: 过滤后磁链的最大数目, 默认为 10
-        :return typing.Tuple[int, dict]: 状态码和 av
+        :return Tuple[int, dict]: 状态码和 av
         av格式:
         {
             'id': '',       # 番号
             'date': '',     # 发行日期
             'title': '',    # 标题
             'title_cn': '', # 中文标题
             'img': '',      # 封面地址
@@ -775,115 +779,132 @@
             if code == 200
             else (code, None)
         )
 
 
 class JavLibUtil(BaseUtil):
     BASE_URL = "https://www.javlibrary.com"
-    # nice
-    BASE_URL_BEST_RATED_LAST_MONTH = BASE_URL + "/cn/vl_bestrated.php?mode=1&page="
-    BASE_URL_BEST_RATED_ALL = BASE_URL + "/cn/vl_bestrated.php?mode=2&page="
-    BASE_URL_MOST_WANTED_LAST_MONTH = BASE_URL + "/cn/vl_mostwanted.php?&mode=1&page="
-    BASE_URL_MOST_WANTED_ALL = BASE_URL + "/cn/vl_mostwanted.php?&mode=2&page="
-    # new
-    BASE_URL_NEW_RELEASE_HAVE_COMMENT = BASE_URL + "/cn/vl_newrelease.php?&mode=1&page="
-    BASE_URL_NEW_RELEASE_ALL = BASE_URL + "/cn/vl_newrelease.php?&mode=2&page="
-    BASE_URL_NEW_ENTRIES = BASE_URL + "/cn/vl_newentries.php?page="
-    URLS_NICE = [
-        BASE_URL_BEST_RATED_LAST_MONTH,
-        BASE_URL_BEST_RATED_ALL,
-        BASE_URL_MOST_WANTED_LAST_MONTH,
-        BASE_URL_MOST_WANTED_ALL,
-    ]
-    URLS_NEW = [
-        BASE_URL_NEW_RELEASE_HAVE_COMMENT,
-        BASE_URL_NEW_RELEASE_ALL,
-        BASE_URL_NEW_ENTRIES,
-    ]
-    # search
-    BASE_URL_SEARCH_AV = BASE_URL + "/cn/vl_searchbyid.php?keyword="
-    # comment
-    BASE_URL_COMMENT = BASE_URL + "/cn/videocomments.php?v="
-    # review 最佳评论
-    BASE_URL_REVIEW = BASE_URL + "/cn/videoreviews.php?v="
     # 排行榜最大页数
     MAX_RANK_PAGE = 25
 
+    def __init__(
+            self,
+            proxy_addr="",
+            use_cache=True,
+            base_url=BASE_URL,
+    ):
+        """初始化
+
+        :param str proxy_addr: 代理服务器地址, 默认为 ''
+        :param bool use_cache: 是否使用缓存, 默认为 True
+        :param str base_url: 基础地址, 默认为 BASE_URL
+        """
+        super().__init__(proxy_addr, use_cache)
+        self.base_url = base_url
+        # nice
+        self.base_url_best_rated_last_month = self.base_url + "/cn/vl_bestrated.php?mode=1&page="
+        self.base_url_best_rated_all = self.base_url + "/cn/vl_bestrated.php?mode=2&page="
+        self.base_url_most_wanted_last_month = self.base_url + "/cn/vl_mostwanted.php?&mode=1&page="
+        self.base_url_most_wanted_all = self.base_url + "/cn/vl_mostwanted.php?&mode=2&page="
+        # new
+        self.base_url_new_release_have_comment = self.base_url + "/cn/vl_newrelease.php?&mode=1&page="
+        self.base_url_new_release_all = self.base_url + "/cn/vl_newrelease.php?&mode=2&page="
+        self.base_url_new_entries = self.base_url + "/cn/vl_newentries.php?page="
+        self.urls_nice = [
+            self.base_url_best_rated_last_month,
+            self.base_url_best_rated_all,
+            self.base_url_most_wanted_last_month,
+            self.base_url_most_wanted_all,
+        ]
+        self.urls_new = [
+            self.base_url_new_release_have_comment,
+            self.base_url_new_release_all,
+            self.base_url_new_entries,
+        ]
+        # search
+        self.base_url_search_av = self.base_url + "/cn/vl_searchbyid.php?keyword="
+        # comment
+        self.base_url_comment = self.base_url + "/cn/videocomments.php?v="
+        # review 最佳评论
+        self.base_url_review = self.base_url + "/cn/videoreviews.php?v="
+
+    def get_headers(self):
+        return {
+            "cookie": "over18=18;",
+            "user-agent": self.ua_desktop(),
+        }
+
     def get_random_ids_from_rank_by_page(
             self, page: int, list_type: int
-    ) -> typing.Tuple[int, str]:
+    ) -> Union[Tuple[int, None], Tuple[int, List[Any]]]:
         """从排行榜某页中获取该页番号列表
 
         :param int page: 第几页
         :param int list_type: 排行榜类型 0 nice | 1 new
-        :return typing.Tuple[int, list]: 状态码和番号列表
+        :return Tuple[int, list]: 状态码和番号列表
         """
+        url = None
         if list_type == 0:
-            url = random.choice(JavLibUtil.URLS_NICE)
+            url = random.choice(self.urls_nice)
         elif list_type == 1:
-            url = random.choice(JavLibUtil.URLS_NEW)
-        headers = {
-            "cookie": "over18=18;",
-            "user-agent": self.ua_desktop(),
-        }
-        code, resp = self.send_req(url=url + str(page), headers=headers)
+            url = random.choice(self.urls_new)
+        code, resp = self.send_req(url=url + str(page), headers=self.get_headers())
         if code != 200:
             return code, None
         try:
             soup = self.get_soup(resp)
             tag_ids = soup.find_all(class_="id")
             ids = [tag.text for tag in tag_ids]
             if len(ids) > 0:
                 return 200, ids
             else:
                 return 404, None
         except Exception as e:
             self.log.error(f"JavLibUtil: 从排行榜某页中获取该页番号列表: {e}")
             return 404, None
 
-    def get_random_id_from_rank(self, list_type: int) -> typing.Tuple[int, str]:
+    def get_random_id_from_rank(self, list_type: int) -> Union[Tuple[Any, None], Tuple[int, Any]]:
         """从排行榜中随机获取番号
 
         :param int list_type: 排行榜类型 0 nice | 1 new
-        :return typing.Tuple[int, str]: 状态码和番号
+        :return Tuple[int, str]: 状态码和番号
         """
         page = random.randint(1, self.MAX_RANK_PAGE)
         code, ids = self.get_random_ids_from_rank_by_page(
             page=page, list_type=list_type
         )
         if code != 200:
             return code, None
         else:
             return 200, random.choice(ids)
 
-    def get_comments_by_id(self, id: str) -> typing.Tuple[int, list]:
+    def get_comments_by_id(self, id: str) -> Union[Tuple[int, None], Tuple[int, List[Any]]]:
         """根据番号获取评论 (最佳评论, 最多 5 条)
 
         :param str id: 番号
-        :return typing.Tuple[int, list]: 状态码和评论列表
+        :return Tuple[int, list]: 状态码和评论列表
         """
-        url = JavLibUtil.BASE_URL_SEARCH_AV + id
-        code, resp = self.send_req(url=url)
+        url = self.base_url_search_av + id
+        code, resp = self.send_req(url=url, headers=self.get_headers())
         if code != 200:
             return code, None
-        javlib_av_id = ""
         if resp.url == url:
             try:
                 soup = self.get_soup(resp)
                 videos = soup.find_all(class_="video")
                 video_href = videos[0].a["href"]
                 javlib_av_id = video_href[video_href.find("v=") + 2:]
             except Exception as e:
                 self.log.error(f"JavLibUtil: 根据番号 {id} 获取评论失败: {e}")
                 return 404, None
         else:
             r_url = resp.url
             javlib_av_id = r_url[r_url.find("v=") + 2:]
-        comment_url = JavLibUtil.BASE_URL_REVIEW + javlib_av_id
-        code, resp = self.send_req(url=comment_url)
+        comment_url = self.base_url_review + javlib_av_id
+        code, resp = self.send_req(url=comment_url, headers=self.get_headers())
         if code != 200:
             return code, None
         try:
             soup = self.get_soup(resp)
             comment_tags = soup.find_all(class_="t")
             comments = []
             for c in comment_tags:
@@ -894,34 +915,49 @@
         except Exception as e:
             self.log.error(f"JavLibUtil: 根据番号 {id} 获取评论失败: {e}")
             return 404, None
 
 
 class DmmUtil(BaseUtil):
     BASE_URL = "https://www.dmm.co.jp"
-    BASE_URL_SEARCH_AV = BASE_URL + "/mono/-/search/=/searchstr="
-    BASE_URL_SEARCH_AV_MONTHLY = (
-            BASE_URL + "/monthly/dream/-/list/search/=/sort=ranking/?searchstr="
-    )
-    BASE_URL_SEARCH_STAR = (
-            BASE_URL + "/digital/videoa/-/list/search/=/device=tv/sort=ranking/?searchstr="
-    )
-    BASE_URL_TOP_STARS = BASE_URL + "/digital/videoa/-/ranking/=/type=actress"
     PAT_CID = re.compile(r"/cid=.+/")
     PAT_CID_REAL = re.compile(r"[A-Za-z]+0+[0-9]+")
     PAT_AV = re.compile(r"[a-z]+\d+")
 
-    def get_pv_by_id(self, id: str) -> typing.Tuple[int, str]:
+    def __init__(
+            self,
+            proxy_addr="",
+            use_cache=True,
+            base_url=BASE_URL,
+    ):
+        """初始化
+
+        :param str proxy_addr: 代理服务器地址, 默认为 ''
+        :param bool use_cache: 是否使用缓存, 默认为 True
+        :param str base_url: 基础地址, 默认为 BASE_URL
+        """
+        super().__init__(proxy_addr, use_cache)
+        self.base_url = base_url
+        self.base_url_search_av = self.base_url + "/mono/-/search/=/searchstr="
+        self.base_url_search_av_monthly = (
+                self.base_url + "/monthly/dream/-/list/search/=/sort=ranking/?searchstr="
+        )
+        self.base_url_search_star = (
+                self.base_url + "/digital/videoa/-/list/search/=/device=tv/sort=ranking/?searchstr="
+        )
+        self.base_url_top_stars = self.base_url + "/digital/videoa/-/ranking/=/type=actress"
+
+    def get_pv_by_id(self, id: str) -> Union[Tuple[int, None], Tuple[int, Any]]:
         """根据番号从 DMM 获取预览视频地址
 
         :param str id: 番号
         :return tuple[int, str]: 状态码和预览视频地址
         """
         # 搜索番号
-        url = DmmUtil.BASE_URL_SEARCH_AV + id
+        url = self.base_url_search_av + id
         code, resp = self.send_req(url=url, headers={
             "user-agent": self.ua_mobile(),
         }, cookies={
             "age_check_done": "1",
         })
         if code != 200:
             return code, None
@@ -929,24 +965,24 @@
             soup = self.get_soup(resp)
             res = soup.find(class_="box-sampleplay")
             return 200, res.a["href"]
         except Exception as e:
             self.log.error(f"DmmUtil: 根据番号 {id} 从 DMM 获取预览视频地址: {e}")
             return 404, None
 
-    def get_cid_from_link(self, lk: str) -> str:
+    def get_cid_from_link(self, lk: str) -> Union[None, str]:
         try:
             match = self.PAT_CID.findall(lk)
             cid = match[0].replace("/cid=", "").replace("/", "")
             # cid = self.CID_PAT_REAL.findall(cid)[0]
             return cid
         except Exception:
             return None
 
-    def get_cids(self, url: str) -> typing.Tuple[int, list]:
+    def get_cids(self, url: str) -> Union[Tuple[int, None], Tuple[int, List[str]]]:
         code, resp = self.send_req(url=url, headers={
             "user-agent": self.ua_desktop(),  # 桌面端页面更方便爬取
         }, cookies={
             "age_check_done": "1",
         })
         if code != 200:
             return code, None
@@ -963,15 +999,15 @@
                 except Exception:
                     pass
             return 200, cids
         except Exception as e:
             self.log.error(f"DmmUtil: 根据 {url} 从 DMM 获取 cid 列表: {e}")
             return 404, None
 
-    def get_cids_monthly(self, url: str) -> typing.Tuple[int, list]:
+    def get_cids_monthly(self, url: str) -> Union[Tuple[int, None], Tuple[int, List[str]]]:
         code, resp = self.send_req(url=url, headers={
             "user-agent": self.ua_desktop(),  # 桌面端页面更方便爬取
         }, cookies={
             "age_check_done": "1",
         })
         if code != 200:
             return code, None
@@ -988,39 +1024,39 @@
                 except Exception:
                     pass
             return 200, cids
         except Exception as e:
             self.log.error(f"DmmUtil: 根据 {url} 从 DMM 获取 cid 列表: {e}")
             return 404, None
 
-    def get_cids_by_tag(self, tag: str) -> typing.Tuple[int, list]:
-        return self.get_cids(self.BASE_URL_SEARCH_AV + tag)
+    def get_cids_by_tag(self, tag: str) -> Tuple[int, list]:
+        return self.get_cids(self.base_url_search_av + tag)
 
-    def get_cids_by_tag_monthly(self, tag: str) -> typing.Tuple[int, list]:
-        return self.get_cids_monthly(self.BASE_URL_SEARCH_AV_MONTHLY + tag)
+    def get_cids_by_tag_monthly(self, tag: str) -> Tuple[int, list]:
+        return self.get_cids_monthly(self.base_url_search_av_monthly + tag)
 
-    def get_cids_by_link(self, lk: str) -> typing.Tuple[int, list]:
+    def get_cids_by_link(self, lk: str) -> Tuple[int, list]:
         return self.get_cids(lk)
 
-    def get_cids_by_link_monthly(self, lk: str) -> typing.Tuple[int, list]:
+    def get_cids_by_link_monthly(self, lk: str) -> Tuple[int, list]:
         return self.get_cids_monthly(lk)
 
-    def get_nice_avs_by_star_name(self, star_name: str) -> typing.Tuple[int, list]:
+    def get_nice_avs_by_star_name(self, star_name: str) -> Tuple[int, any]:
         """根据演员名字获取高分番号列表
 
         :param str star_name: 演员名字
-        :return typing.Tuple[int, list]: 状态码和番号列表
+        :return Tuple[int, list]: 状态码和番号列表
         番号列表单个对象结构:
         {
             'rate': rate, # 评分
             'id': id # 番号
         }
         """
         # 搜索演员
-        url = DmmUtil.BASE_URL_SEARCH_STAR + star_name
+        url = self.base_url_search_star + star_name
         code, resp = self.send_req(url=url, headers={
             "user-agent": self.ua_desktop(),  # 桌面端页面更方便爬取
         }, cookies={
             "age_check_done": "1",
         })
         if code != 200:
             return code, resp
@@ -1047,22 +1083,22 @@
             if len(avs) == 0:
                 return 404, None
             return 200, avs
         except Exception as e:
             self.log.error(f"DmmUtil: 根据演员名字 {star_name} 获取高分番号列表: {e}")
             return 404, None
 
-    def get_score_by_id(self, id: str) -> typing.Tuple[int, str]:
+    def get_score_by_id(self, id: str) -> Tuple[int, any]:
         """根据番号返回评分
 
         :param str id: 番号
         :return tuple[int, str]: 状态码和评分
         """
         # 搜索番号
-        url = DmmUtil.BASE_URL_SEARCH_AV + id
+        url = self.base_url_search_av + id
         code, resp = self.send_req(url=url, headers={
             "user-agent": self.ua_desktop(),  # 桌面端页面更方便爬取
         }, cookies={
             "age_check_done": "1",
         })
         if code != 200:
             return code, resp
@@ -1078,21 +1114,21 @@
         """根据普通 src 获取更清晰的 src
 
         :param str src
         :return str: nice src
         """
         return src.replace("_sm_", "_dmb_")
 
-    def get_top_stars(self, page=1) -> typing.Tuple[int, list]:
+    def get_top_stars(self, page=1) -> Union[Tuple[int, None], Tuple[int, List[Any]]]:
         """根据页数获取明星排行榜某页中的明星列表
 
         :param int page: 页数, 共 5 页, 每页 20 位, 共 100 位,  defaults to 1
         :return tuple[int, list]: 状态码和明星列表
         """
-        url = DmmUtil.BASE_URL_TOP_STARS + f"/page={page}/"
+        url = self.base_url_top_stars + f"/page={page}/"
         code, resp = self.send_req(url=url, headers={
             "user-agent": self.ua_desktop(),  # 桌面端页面更方便爬取
         }, cookies={
             "age_check_done": "1",
         })
         if code != 200:
             return code, None
@@ -1102,15 +1138,15 @@
             if not res or len(res) == 0:
                 return 404, None
             return 200, [obj.p.a.text for obj in res]
         except Exception as e:
             self.log.error(f"DmmUtil: 获取明星排行榜第 {page} 页中的明星列表: {e}")
             return 404, None
 
-    def get_all_top_stars(self) -> typing.Tuple[int, list]:
+    def get_all_top_stars(self) -> Union[Tuple[int, None], Tuple[int, List[Any]]]:
         """获取 DMM 排行榜前 100 名女优
 
         :return tuple[int, list]: 状态码和女优名称列表
         """
         with concurrent.futures.ThreadPoolExecutor(max_workers=6) as executor:
             # 爬取第一到第五页数据
             futures = {
@@ -1130,19 +1166,14 @@
             if stars == []:
                 return 404, None
             return 200, stars
 
 
 class JavBusUtil(BaseUtil):
     BASE_URL = "https://www.javbus.com"
-    BASE_URL_SEARCH_BY_STAR_NAME = f"{BASE_URL}/search"
-    BASE_URL_SEARCH_BY_STAR_ID = f"{BASE_URL}/star"
-    BASE_URL_SEARCH_STAR = f"{BASE_URL}/searchstar"
-    BASE_URL_MAGNET = f"{BASE_URL}/ajax/uncledatoolsbyajax.php?lang=zh"
-    BASE_URL_GENRE = f"{BASE_URL}/genre"
 
     def get_headers(self):
         # return {
         #     "authority": "www.javbus.com",
         #     "accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
         #     "accept-language": "zh-CN,zh;q=0.9,en;q=0.8,en-US;q=0.7,fr-FR;q=0.6,fr;q=0.5",
         #     "cookie": f"bus_auth={self.bus_auth};",
@@ -1165,35 +1196,43 @@
     def __init__(
             self,
             bus_auth: str,
             proxy_addr="",
             use_cache=True,
             max_home_page_count=100,
             max_new_avs_count=8,
+            base_url=BASE_URL
     ):
         """初始化
 
         :param str proxy_addr: 代理服务器地址, 默认为 ''
         :param bool use_cache: 是否使用缓存
         :param int max_home_page_count: 主页最大爬取页数, 默认为 100 页
         :param int max_new_avs_count: 获取最新 AV 数量, 默认为 8 部
         :param str bus_auth: cookie 需要用到的值
+        :param str base_url: 基础地址, 默认为 BASE_URL
         """
         super().__init__(proxy_addr, use_cache)
         self.max_home_page_count = max_home_page_count
         self.max_new_avs_count = max_new_avs_count
         self.bus_auth = bus_auth
+        self.base_url = base_url
+        self.base_url_search_by_star_name = f"{self.base_url}/search"
+        self.base_url_search_by_star_id = f"{self.base_url}/star"
+        self.base_url_search_star = f"{self.base_url}/searchstar"
+        self.base_url_magnet = f"{self.base_url}/ajax/uncledatoolsbyajax.php?lang=zh"
+        self.base_url_genre = f"{self.base_url}/genre"
 
-    def get_all_genres(self) -> typing.Tuple[int, list]:
+    def get_all_genres(self) -> Union[Tuple[int, None], Tuple[int, List[Dict[Any, Any]]]]:
         """获取所有类别
 
-        :return typing.Tuple[int, list]: 状态码和类别列表
+        :return Tuple[int, list]: 状态码和类别列表
         """
         code, resp = self.send_req(
-            url=JavBusUtil.BASE_URL_GENRE, headers=self.get_headers()
+            url=self.base_url_genre, headers=self.get_headers()
         )
         if code != 200:
             return code, None
         try:
             soup = self.get_soup(resp)
             boxes = soup.find_all(class_="row genre-box")
             genres = []
@@ -1204,35 +1243,35 @@
             if genres == []:
                 return 404, None
             return 200, genres
         except Exception as e:
             self.log.error(f"JavBusUtil: 获取所有标签失败: {e}")
             return 404, None
 
-    def get_id_by_genre_id(self, genre: str) -> typing.Tuple[int, str]:
+    def get_id_by_genre_id(self, genre: str) -> Tuple[int, str]:
         """通过类别编号获取一个番号
 
         :param str genre: 类别编号
-        :return typing.Tuple[int, str]: 状态码和番号
+        :return Tuple[int, str]: 状态码和番号
         """
         return self.get_id_from_page(
-            base_page_url=f"{JavBusUtil.BASE_URL_GENRE}/{genre}"
+            base_page_url=f"{self.base_url_genre}/{genre}"
         )
 
-    def get_id_by_genre_name(self, genre: str) -> typing.Tuple[int, str]:
+    def get_id_by_genre_name(self, genre: str) -> Tuple[int, str]:
         """通过类别编号获取一个番号
 
         :param str genre: 类别名称
-        :return typing.Tuple[int, str]: 状态码和番号
+        :return Tuple[int, str]: 状态码和番号
         """
         return self.get_id_from_page(
-            base_page_url=f"{JavBusUtil.BASE_URL_GENRE}/{genre}"
+            base_page_url=f"{self.base_url_genre}/{genre}"
         )
 
-    def get_max_page(self, url: str) -> typing.Tuple[int, int]:
+    def get_max_page(self, url: str) -> Union[Tuple[int, None], Tuple[int, int]]:
         """获取最大页数(只适用于不超过 10 页的页面)
 
         :param str url: 页面地址
         :return tuple[int, int]: 状态码和最大页数
         """
         code, resp = self.send_req(url, headers=self.get_headers())
         if code != 200:
@@ -1245,15 +1284,15 @@
                 return 200, 1
             tags_li = tag_pagination.find_all("li")
             return 200, int(tags_li[len(tags_li) - 2].a.text)
         except Exception as e:
             self.log.error(f"JavBusUtil: 从 {url} 获取最大页数: {e}")
             return 404, None
 
-    def get_ids_from_page(self, base_page_url: str, page=1) -> typing.Tuple[int, list]:
+    def get_ids_from_page(self, base_page_url: str, page=1) -> Union[Tuple[int, None], Tuple[int, List[Any]]]:
         """从 av 列表页面获取该页面全部番号
 
         :param str base_page: 基础页地址, 也是第一页地址
         :param int page: 用于指定爬取哪一页的数据, 默认值为 1, 表示获取第一页
         :return tuple[int, str]: 状态码和番号列表
         """
         if page != -1:
@@ -1279,140 +1318,140 @@
             return 200, ids
         except Exception as e:
             self.log.error(
                 f"JavBusUtil: 从 av 列表页面 {base_page_url} 获取该页面全部番号: {e}"
             )
             return 404, None
 
-    def get_id_from_page(self, base_page_url: str, page=-1) -> typing.Tuple[int, str]:
+    def get_id_from_page(self, base_page_url: str, page=-1) -> Union[Tuple[int, None], Tuple[int, Any]]:
         """从 av 列表页面获取一个番号
 
         :param str base_page: 基础页地址, 也是第一页地址
         :param int page: 用于指定爬取哪一页的数据, 默认值为 -1, 表示随机获取某一页
         :return tuple[int, str]: 状态码和番号
         """
         code, ids = self.get_ids_from_page(base_page_url, page)
         if code != 200:
             return code, None
         return 200, random.choice(ids)
 
-    def get_id_from_home(self, page=-1) -> typing.Tuple[int, str]:
+    def get_id_from_home(self, page=-1) -> Tuple[int, str]:
         """从 javbus 主页获取一个番号
 
         :param int page: 用于指定爬取哪一页的数据, 默认值为 -1, 表示随机获取某一页
         :return tuple[int, str]: 状态码和番号
         """
         if page == -1:
             page = random.randint(1, self.max_home_page_count)
         return self.get_id_from_page(
-            base_page_url=JavBusUtil.BASE_URL + "/page", page=page
+            base_page_url=self.base_url + "/page", page=page
         )
 
-    def get_id_by_star_name(self, star_name: str, page=-1) -> typing.Tuple[int, str]:
+    def get_id_by_star_name(self, star_name: str, page=-1) -> Tuple[int, str]:
         """根据演员名称获取一个番号
 
         :param str star_name: 演员名称
         :param int page: 用于指定爬取哪一页的数据, 默认值为 -1, 表示随机获取某一页
         :return tuple[int, str]: 状态码和番号
         """
         return self.get_id_from_page(
-            base_page_url=f"{JavBusUtil.BASE_URL_SEARCH_BY_STAR_NAME}/{star_name}",
+            base_page_url=f"{self.base_url_search_by_star_name}/{star_name}",
             page=page,
         )
 
-    def get_ids_by_star_name(self, star_name: str, page=-1) -> typing.Tuple[int, list]:
+    def get_ids_by_star_name(self, star_name: str, page=-1) -> Tuple[int, list]:
         """根据演员名称获取一批番号
 
         :param str star_name: 演员名称
         :param int page: 用于指定爬取哪一页的数据, 默认值为 -1, 表示随机获取某一页
         :return tuple[int, list]: 状态码和番号
         """
         return self.get_ids_from_page(
-            base_page_url=f"{JavBusUtil.BASE_URL_SEARCH_BY_STAR_NAME}/{star_name}",
+            base_page_url=f"{self.base_url_search_by_star_name}/{star_name}",
             page=page,
         )
 
-    def get_new_ids_by_star_name(self, star_name: str) -> typing.Tuple[int, list]:
+    def get_new_ids_by_star_name(self, star_name: str) -> Union[Tuple[int, None], Tuple[int, Any]]:
         """根据演员名字获取最新番号列表
 
         :param str star_name: 演员名称
-        :return typing.Tuple[int, list]: 状态码和番号列表
+        :return Tuple[int, list]: 状态码和番号列表
         """
         code, ids = self.get_ids_from_page(
-            base_page_url=f"{JavBusUtil.BASE_URL_SEARCH_BY_STAR_NAME}/{star_name}",
+            base_page_url=f"{self.base_url_search_by_star_name}/{star_name}",
             page=1,
         )
         if code != 200:
             return code, None
         return 200, ids[: self.max_new_avs_count]
 
-    def get_id_by_star_id(self, star_id: str, page=-1) -> typing.Tuple[int, str]:
+    def get_id_by_star_id(self, star_id: str, page=-1) -> Tuple[int, str]:
         """根据演员编号获取一个番号
 
         :param str star_id: 演员编号
         :param int page: 用于指定爬取哪一页的数据, 默认值为 -1, 表示随机获取某一页
         :return tuple[int, str]: 状态码和番号
         """
         return self.get_id_from_page(
-            base_page_url=f"{JavBusUtil.BASE_URL_SEARCH_BY_STAR_ID}/{star_id}",
+            base_page_url=f"{self.base_url_search_by_star_id}/{star_id}",
             page=page,
         )
 
-    def get_new_ids_by_star_id(self, star_id: str) -> typing.Tuple[int, list]:
+    def get_new_ids_by_star_id(self, star_id: str) -> Union[Tuple[int, None], Tuple[int, list]]:
         """根据演员编号获取最新番号
 
         :param str star_id: 演员编号
         :return tuple[int, list]: 状态码和番号列表
         """
         code, ids = self.get_ids_from_page(
-            base_page_url=f"{JavBusUtil.BASE_URL_SEARCH_BY_STAR_ID}/{star_id}", page=1
+            base_page_url=f"{self.base_url_search_by_star_id}/{star_id}", page=1
         )
         if code != 200:
             return code, None
         return 200, ids[: self.max_new_avs_count]
 
-    def get_samples_by_id(self, id: str) -> typing.Tuple[int, list]:
+    def get_samples_by_id(self, id: str) -> Union[Tuple[int, None], Tuple[int, List[Union[str, Any]]]]:
         """根据番号获取截图
 
         :param str id: 番号
         :return tuple[int, list]: 状态码和截图列表
         """
         samples = []
-        url = f"{JavBusUtil.BASE_URL}/{id}"
+        url = f"{self.base_url}/{id}"
         code, resp = self.send_req(url=url, headers=self.get_headers())
         if code != 200:
             return code, None
         try:
             soup = self.get_soup(resp)
             sample_tags = soup.find_all(class_="sample-box")
             for tag in sample_tags:
                 sample_link = tag["href"]
                 if sample_link.find("https") == -1:
-                    sample_link = JavBusUtil.BASE_URL + sample_link
+                    sample_link = self.base_url + sample_link
                 samples.append(sample_link)
             if samples == []:
                 return 404, None
             return 200, samples
         except Exception as e:
             self.log.error(f"JavBusUtil: 根据番号 {id} 获取截图: {e}")
             return 404, None
 
-    def check_star_exists(self, star_name: str) -> typing.Tuple[int, dict]:
+    def check_star_exists(self, star_name: str) -> Union[Tuple[int, None], Tuple[int, Dict[str, Union[str, Any]]]]:
         """根据演员名称确认该演员在 javbus 是否存在, 如果存在则返回演员 id 和演员名称
 
         :param str star_name: 演员名称
         :return tuple[int, dict]: 状态码, 演员 id 和演员名称
         dict 格式:
         {
             "star_id": star_id,
             "star_name": star_name
         }
         """
         code, resp = self.send_req(
-            url=f"{JavBusUtil.BASE_URL_SEARCH_STAR}/{star_name}",
+            url=f"{self.base_url_search_star}/{star_name}",
             headers=self.get_headers(),
         )
         if code != 200:
             return code, None
         try:
             soup = self.get_soup(resp)
             star = soup.find(class_="avatar-box text-center")
@@ -1421,21 +1460,21 @@
             return 200, {"star_id": star_id, "star_name": res_star_name}
         except Exception as e:
             self.log.error(
                 f"JavBusUtil: 根据演员名称 {star_name} 确认该演员在 javbus 是否存在: {e}"
             )
             return 404, None
 
-    def fuzzy_search_stars(self, text) -> typing.Tuple[int, list]:
+    def fuzzy_search_stars(self, text) -> Union[Tuple[int, None], Tuple[int, List[Any]]]:
         """模糊搜索演员
 
         :param str text: 演员名称
-        :return typing.Tuple[int, list]: 状态码和演员列表
+        :return Tuple[int, list]: 状态码和演员列表
         """
-        code, resp = self.send_req(url=f"{JavBusUtil.BASE_URL_SEARCH_STAR}/{text}", headers=self.get_headers())
+        code, resp = self.send_req(url=f"{self.base_url_search_star}/{text}", headers=self.get_headers())
         if code != 200:
             return code, None
         try:
             soup = self.get_soup(resp)
             actor_boxs = soup.find_all(class_="avatar-box text-center")
             names = [box.find("img")["title"] for box in actor_boxs]
             if not names:
@@ -1448,15 +1487,15 @@
 
     def get_av_by_id(
             self,
             id: str,
             is_nice: bool,
             is_uncensored: bool,
             magnet_max_count=10,
-    ) -> typing.Tuple[int, dict]:
+    ) -> Tuple[int, any]:
         """通过 javbus 获取番号对应 av
 
         :param str id: 番号
         :param bool is_nice: 是否过滤出高清, 有字幕磁链
         :param bool is_uncensored: 是否过滤出无码磁链
         :param int magnet_max_count: 过滤后磁链的最大数目, 默认为 10
         :return tuple[int, dict]: 状态码和 av
@@ -1493,29 +1532,29 @@
             "img": "",
             "date": "",
             "tags": "",
             "stars": [],
             "magnets": [],
             "url": "",
         }
-        url = f"{JavBusUtil.BASE_URL}/{id}"
+        url = f"{self.base_url}/{id}"
         av["url"] = url
         code, resp = self.send_req(url=url, headers=self.get_headers())
         if code != 200:
             return code, None
         soup = self.get_soup(resp)
         html = soup.prettify()
         try:
             # 获取封面和标题
             big_image = soup.find(class_="bigImage")
             img = None
             if big_image:
                 img = big_image["href"]
                 if img.find("http") == -1:
-                    av["img"] = JavBusUtil.BASE_URL + img
+                    av["img"] = self.base_url + img
                     av["title"] = big_image.img["title"]
             paras = soup.find(class_="col-md-3 info").find_all("p")
             for i, p in enumerate(paras):
                 # 获取識別碼
                 if p.text.find("識別碼:") != -1:
                     av["id"] = "".join(
                         p.text.replace("識別碼:", "").replace('"', "").split()
@@ -1551,18 +1590,18 @@
         gid = None
         if match:
             gid = match[0].replace("var gid = ", "").replace(";", "")
         # 如果不存在磁链则直接返回
         if not uc and not gid:
             return 200, av
         # 得到磁链的ajax请求地址
-        url = f"{JavBusUtil.BASE_URL_MAGNET}&gid={gid}&uc={uc}"
+        url = f"{self.base_url_magnet}&gid={gid}&uc={uc}"
         headers = {
             "user-agent": self.ua(),
-            "referer": f"{JavBusUtil.BASE_URL}/{id}",
+            "referer": f"{self.base_url}/{id}",
         }
         # 发送请求获取含磁链页
         code, resp = self.send_req(url=url, headers=headers)
         # 如果不存在磁链或请求失败则直接返回
         if code != 200:
             return 200, av
         # 解析页面获取磁链
@@ -1613,27 +1652,42 @@
             self.log.error(f"JavBusUtil: 通过 javbus 获取番号 {id} 对应 av: {e}")
         return 200, av
 
 
 class AvgleUtil(BaseUtil):
     BASE_URL = "https://api.avgle.com"
 
-    def get_video_by_id(self, id: str) -> typing.Tuple[int, dict]:
+    def __init__(
+            self,
+            proxy_addr="",
+            use_cache=True,
+            base_url=BASE_URL,
+    ):
+        """初始化
+
+        :param str proxy_addr: 代理服务器地址, 默认为 ''
+        :param bool use_cache: 是否使用缓存, 默认为 True
+        :param str base_url: 基础地址, 默认为 BASE_URL
+        """
+        super().__init__(proxy_addr, use_cache)
+        self.base_url = base_url
+
+    def get_video_by_id(self, id: str) -> Tuple[int, any]:
         """根据番号从 avgle 获取视频
         :param str id: 番号
         :return tuple[int, dict]: 状态码, 视频链接
         视频链接：
         {
             'fv': '', # 完整视频链接
             'pv': ''  # 预览视频链接
         }
         """
         page = 0
         limit = 3
-        url = f"{AvgleUtil.BASE_URL}/v1/jav/{id}/{page}?limit={limit}"
+        url = f"{self.base_url}/v1/jav/{id}/{page}?limit={limit}"
         res = {"fv": "", "pv": ""}
         code, resp = self.send_req(url=url)
         if code != 200:
             return code, None
         if resp.json()["success"]:
             videos = resp.json()["response"]["videos"]
             if videos != []:
@@ -1644,28 +1698,28 @@
                         res["fv"] = fv_url
                     if res["pv"] == "" and pv_url != "":
                         res["pv"] = pv_url
             return code, res
         else:
             return 404, None
 
-    def get_pv_by_id(self, id: str) -> typing.Tuple[int, str]:
+    def get_pv_by_id(self, id: str) -> Union[Tuple[int, None], Tuple[int, str]]:
         """根据番号从 avgle 获取预览视频
         :param str id: 番号
         :return tuple[int, str]: 状态码, 预览视频链接
         """
         code, res = self.get_video_by_id(id)
         if code != 200:
             return code, None
         if res["pv"] != "":
             return 200, res["pv"]
         else:
             return 404, None
 
-    def get_fv_by_id(self, id: str) -> typing.Tuple[int, str]:
+    def get_fv_by_id(self, id: str) -> Union[Tuple[int, None], Tuple[int, str]]:
         """根据番号从 avgle 获取完整视频
         :param str id: 番号
         :return tuple[int, str]: 状态码, 完整视频链接
         """
         code, res = self.get_video_by_id(id)
         if code != 200:
             return code, None
@@ -1721,21 +1775,36 @@
         magnets = sorted(magnets, key=lambda m: m["size_no_unit"], reverse=True)
         return magnets
 
 
 class SukebeiUtil(BaseUtil):
     BASE_URL = "https://sukebei.nyaa.si"
 
+    def __init__(
+            self,
+            proxy_addr="",
+            use_cache=True,
+            base_url=BASE_URL,
+    ):
+        """初始化
+
+        :param str proxy_addr: 代理服务器地址, 默认为 ''
+        :param bool use_cache: 是否使用缓存, 默认为 True
+        :param str base_url: 基础地址, 默认为 BASE_URL
+        """
+        super().__init__(proxy_addr, use_cache)
+        self.base_url = base_url
+
     def get_av_by_id(
             self,
             id: str,
             is_nice: bool,
             is_uncensored: bool,
             magnet_max_count=10,
-    ) -> typing.Tuple[int, dict]:
+    ) -> Tuple[int, any]:
         """通过 sukebei 获取番号对应 av
 
         :param str id: 番号
         :param bool is_nice: 是否过滤出高清, 有字幕磁链
         :param bool is_uncensored: 是否过滤出无码磁链
         :param int magnet_max_count: 过滤后磁链的最大数目, 默认为 10
         :return tuple[int, dict]: 状态码和 av
@@ -1775,15 +1844,15 @@
             "magnets": [],
             "url": "",
         }
         qid = id.lower()
         if qid.find("fc2") != -1:
             qid = qid.replace("-", " ")
         # 查找av
-        url = f"{SukebeiUtil.BASE_URL}?q={qid}"
+        url = f"{self.base_url}?q={qid}"
         code, resp = self.send_req(url=url)
         if code != 200:
             return code, None
         try:
             av["url"] = url
             soup = self.get_soup(resp)
             torrent_list = soup.find(class_="torrent-list")
@@ -1826,26 +1895,26 @@
                 av["magnets"] = magnets
 
         except Exception as e:
             self.log.error(f"SukebeiUtil: 通过 sukebei 获取番号 {id} 对应 av: {e}")
             return 404, None
         return 200, av
 
-    def search_av_by_tag(self, tag: str) -> typing.Tuple[int, list]:
+    def search_av_by_tag(self, tag: str) -> Tuple[int, any]:
         """根据关键字搜索影片
 
         :param str tag: 关键字
-        :return typing.Tuple[int, list]: 状态码和影片列表
+        :return Tuple[int, list]: 状态码和影片列表
         影片列表单位结构:
         {
             "title": "",
             "loc": "", # /view/{num}
         }
         """
-        url = f"{SukebeiUtil.BASE_URL}?q={tag}"
+        url = f"{self.base_url}?q={tag}"
         code, resp = self.send_req(url=url)
         if code != 200:
             return code, None
         try:
             soup = self.get_soup(resp)
             torrent_list = soup.find(class_="torrent-list")
             trs = torrent_list.tbody.find_all("tr")
@@ -1862,19 +1931,19 @@
             if avs == []:
                 return 404, None
             return 200, avs
         except Exception as e:
             self.log.error(f"SukebeiUtil: 根据关键字{tag}搜索影片: {e}")
             return 404, None
 
-    def get_av_by_url(self, url: str) -> typing.Tuple[int, dict]:
+    def get_av_by_url(self, url: str) -> Tuple[int, any]:
         """根据地址获取 av
 
         :param str url: 地址
-        :return typing.Tuple[int, dict]: 状态码和资源
+        :return Tuple[int, dict]: 状态码和资源
         资源结构:
         {
             "url": "",
             "title": "",
             "img": [],
             "magnet": "",
         }
@@ -1902,15 +1971,15 @@
 
 
 class WikiUtil(BaseUtil):
     logging.getLogger("wikipediaapi").setLevel(logging.ERROR)
     BASE_URL_JAPAN_WIKI = "https://ja.wikipedia.org/wiki"
     BASE_URL_CHINA_WIKI = "https://zh.wikipedia.org/wiki"
 
-    def get_wiki_page_by_lang(self, topic: str, from_lang: str, to_lang: str) -> dict:
+    def get_wiki_page_by_lang(self, topic: str, from_lang: str, to_lang: str) -> Union[dict, None]:
         """根据搜索词和原来语言码返回指定语言维基页, 如果搜索不到结果则返回空, 如果搜索到结果但找不到指定语言维基页则返回原页
 
         :param str topic: 搜索词
         :param str from_lang: 原来语言码
         :param str to_lang: 目标语言码
         :return dict: 结果集
         {
@@ -1936,15 +2005,15 @@
                             "lang": langlinks[k].language,
                         }
                 return {"title": page.title, "url": page.fullurl, "lang": from_lang}
         except Exception as e:
             self.log.error(
                 f"WikiUtil: 根据搜索词 {topic} 和原来语言码 {from_lang} 返回指定语言 {to_lang} 维基页: {e}"
             )
-            return
+            return None
 
 
 class TransUtil(BaseUtil):
     def trans(self, text: str, from_lang="auto", to_lang="zh-CN") -> str:
         """翻译
 
         :param str text: 要翻译的文本
@@ -1954,67 +2023,7 @@
         """
         try:
             return GoogleTranslator(
                 source=from_lang, target=to_lang, proxies=self.proxy_json
             ).translate(text)
         except Exception as e:
             self.log.error(f"TransUtil: 翻译: {e}")
-
-
-class SgpUtil(BaseUtil):
-    BASE_URL = "http://www.fpie2.com"
-    BASE_URL_SEARCH = "https://api.cbbee0.com/v1_2/articleSearch"
-    BASE_URL_DETAIL = f"{BASE_URL}/play-details/1/"
-
-    def get_video_by_av_id(self, av_id: str) -> typing.Tuple[int, str]:
-        headers = {
-            "authority": "api.cbbee0.com",
-            "accept": "application/json, text/plain, */*",
-            "accept-language": "zh-CN,zh;q=0.9,en;q=0.8,en-GB;q=0.7,en-US;q=0.6,zh-TW;q=0.5",
-            "content-type": "application/json;charset=UTF-8",
-            "origin": SgpUtil.BASE_URL,
-            "referer": SgpUtil.BASE_URL + "/",
-            "sec-ch-ua": '"Not.A/Brand";v="8", "Chromium";v="114", "Microsoft Edge";v="114"',
-            "sec-ch-ua-mobile": "?0",
-            "sec-ch-ua-platform": '"macOS"',
-            "sec-fetch-dest": "empty",
-            "sec-fetch-mode": "cors",
-            "sec-fetch-site": "cross-site",
-            "user-agent": self.ua(),
-        }
-        data = (
-                '{"conditions": "'
-                + av_id
-                + '", "field": 0, "target": 1, "sort": 1, "userToken": "", "hm": "008-api", "device_id": ""}'
-        )
-
-        code, resp = self.send_req(
-            url=SgpUtil.BASE_URL_SEARCH, headers=headers, m=1, data=data
-        )
-        if code != 200:
-            return code, None
-        res = resp.json()
-        code, resp = self.send_req(
-            url=SgpUtil.BASE_URL_DETAIL,
-            headers=headers,
-            json={
-                "encrypt_key": res["encrypt_key"],
-                "encrypt_data": res["encrypt_data"],
-            },
-        )
-        if code != 200:
-            return code, None
-        soup = self.get_soup(resp)
-        try:
-            suffix = soup.find("iframe")["src"]
-            video_addr = f"{SgpUtil.BASE_URL}{suffix}"
-            video_content = soup.find("div", {"class": "content"})
-            res = f"""解说视频地址: {video_addr}
-            
-            解说内容:
-            
-            {video_content}
-            
-            解说视频地址: {video_addr}"""
-            return 200, res
-        except Exception:
-            return 404, None
```

### Comparing `Jvav-1.9.5/requirements.txt` & `Jvav-2.0.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `Jvav-1.9.5/setup.py` & `Jvav-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     requires = [i.strip() for i in r]
 
 with open("README.md", encoding="utf-8") as f:
     readme = f.read()
 
 setup(
     name="Jvav",
-    version="1.9.5",
+    version="2.0.0",
     description="Useful tools for Jav.",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/akynazh/jvav",
     download_url="https://github.com/akynazh/jvav/releases/latest",
     author="akynazh",
     author_email="akynazh@gmail.com",
```

