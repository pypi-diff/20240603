# Comparing `tmp/chatchat-0.1.3.tar.gz` & `tmp/chatchat-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatchat-0.1.3.tar", last modified: Tue May 28 23:05:00 2024, max compression
+gzip compressed data, was "chatchat-0.1.4.tar", last modified: Mon Jun  3 13:39:14 2024, max compression
```

## Comparing `chatchat-0.1.3.tar` & `chatchat-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:05:00.057630 chatchat-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-28 23:04:54.000000 chatchat-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-28 23:05:00.057630 chatchat-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-28 23:04:54.000000 chatchat-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:05:00.057630 chatchat-0.1.3/chatchat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:04:54.000000 chatchat-0.1.3/chatchat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-28 23:04:54.000000 chatchat-0.1.3/chatchat/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-28 23:04:54.000000 chatchat-0.1.3/chatchat/alibaba.py
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-05-28 23:04:54.000000 chatchat-0.1.3/chatchat/baidu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-28 23:04:54.000000 chatchat-0.1.3/chatchat/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-05-28 23:04:54.000000 chatchat-0.1.3/chatchat/tencent.py
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-28 23:04:54.000000 chatchat-0.1.3/chatchat/xunfei.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:05:00.057630 chatchat-0.1.3/chatchat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-28 23:05:00.000000 chatchat-0.1.3/chatchat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-28 23:05:00.000000 chatchat-0.1.3/chatchat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 23:05:00.000000 chatchat-0.1.3/chatchat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-28 23:05:00.000000 chatchat-0.1.3/chatchat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-28 23:05:00.000000 chatchat-0.1.3/chatchat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-28 23:05:00.000000 chatchat-0.1.3/chatchat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 23:05:00.057630 chatchat-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-28 23:04:54.000000 chatchat-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:39:14.786149 chatchat-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-06-03 13:39:00.000000 chatchat-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-06-03 13:39:14.786149 chatchat-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-06-03 13:39:00.000000 chatchat-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:39:14.782149 chatchat-0.1.4/chatchat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:39:00.000000 chatchat-0.1.4/chatchat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-06-03 13:39:00.000000 chatchat-0.1.4/chatchat/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-06-03 13:39:00.000000 chatchat-0.1.4/chatchat/alibaba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-06-03 13:39:00.000000 chatchat-0.1.4/chatchat/baidu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-06-03 13:39:00.000000 chatchat-0.1.4/chatchat/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-06-03 13:39:00.000000 chatchat-0.1.4/chatchat/tencent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-06-03 13:39:00.000000 chatchat-0.1.4/chatchat/xunfei.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:39:14.786149 chatchat-0.1.4/chatchat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-06-03 13:39:14.000000 chatchat-0.1.4/chatchat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-06-03 13:39:14.000000 chatchat-0.1.4/chatchat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 13:39:14.000000 chatchat-0.1.4/chatchat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-06-03 13:39:14.000000 chatchat-0.1.4/chatchat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-03 13:39:14.000000 chatchat-0.1.4/chatchat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-03 13:39:14.000000 chatchat-0.1.4/chatchat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 13:39:14.786149 chatchat-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-06-03 13:39:00.000000 chatchat-0.1.4/setup.py
```

### Comparing `chatchat-0.1.3/LICENSE` & `chatchat-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chatchat-0.1.3/README.md` & `chatchat-0.1.4/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -6,20 +6,41 @@
 
 ### Install
 ```shell
 pip install chatchat
 ```
 
 ### Usage
+```shell
+# set YOUR secret keys
+# tencent
+chatchat config tencent.secret_id=YOUR_SECRET_ID
+chatchat config tencent.secret_key=YOUR_SECRET_KEY
+# baidu
+chatchat config baidu.api_key=YOUR_API_KEY
+chatchat config baidu.secret_key=YOUR_SECRET_KEY
+# list info of all supported platform
+chatchat config --list
+```
 > Refer to [\[examples\]](./examples)
 
 ### Sponsor
 <table align="center">
     <thead>
         <tr>
+            <th colspan="2">公众号</th>
+        </tr>
+    </thead>
+    <tbody align="center" valign="center">
+        <tr>
+            <td colspan="2"><img src="https://www.chatqkv.com/ghstatic/images/ofa_m.png" style="height: 196px" alt="AliPay.png"></td>
+        </tr>
+    </tbody>
+    <thead>
+        <tr>
             <th>AliPay</th>
             <th>WeChatPay</th>
         </tr>
     </thead>
     <tbody align="center" valign="center">
         <tr>
             <td><img src="https://www.chatqkv.com/AliPay.png" style="width: 196px; height: 196px" alt="AliPay.png"></td>
```

#### html2text {}

```diff
@@ -1,6 +1,13 @@
 ### Large Language Models Python API - â ç¾åº¦æå¿ä¸è¨/ERNIE - â
 é¿ééä¹åé®/QWen - â è®¯é£æç«å¤§æ¨¡å/Spark - â
 è¾è®¯æ··åå¤§æ¨¡å/Hunyuan ### Install ```shell pip install chatchat ``` ###
-Usage > Refer to [\[examples\]](./examples) ### Sponsor
+Usage ```shell # set YOUR secret keys # tencent chatchat config
+tencent.secret_id=YOUR_SECRET_ID chatchat config
+tencent.secret_key=YOUR_SECRET_KEY # baidu chatchat config
+baidu.api_key=YOUR_API_KEY chatchat config baidu.secret_key=YOUR_SECRET_KEY #
+list info of all supported platform chatchat config --list ``` > Refer to [\
+[examples\]](./examples) ### Sponsor
+                         ?å??¬?ä?¼??å??·
+                         [AliPay.png]
                          AAlliiPPaayy       WWeeCChhaattPPaayy
                          [AliPay.png] [WeChatPay.png]
```

### Comparing `chatchat-0.1.3/chatchat/__main__.py` & `chatchat-0.1.4/chatchat/__main__.py`

 * *Files identical despite different names*

### Comparing `chatchat-0.1.3/chatchat/alibaba.py` & `chatchat-0.1.4/chatchat/alibaba.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from chatchat.base import Base
 import httpx
 
 class Completion(Base):
-    def __init__(self, model='qwen-turbo'):
+    def __init__(self, model='qwen-turbo', proxy=None, timeout=None):
         super().__init__()
 
         plat = 'alibaba'
         self.verify_secret_data(plat, ('api_key',))
         self.jdata = self.secret_data[plat]
 
         # https://dashscope.console.aliyun.com/dashboard?apiKey=all&model=qwen-turbo
@@ -17,15 +17,15 @@
         ])
 
         if model not in self.model_type:
             raise RuntimeError(f'supported chat type: {list(self.model_type)}')
         self.model = model
 
         self.api = 'https://dashscope.aliyuncs.com/api/v1/services/aigc/text-generation/generation'
-        self.client = httpx.Client()
+        self.client = httpx.Client(proxy=proxy, timeout=timeout)
         self.headers = {
             'Content-Type': 'application/json',
             'Authorization': f'Bearer {self.jdata["api_key"]}',
         }
 
     def send_message(self, messages: list):
         jmsg = {
```

### Comparing `chatchat-0.1.3/chatchat/baidu.py` & `chatchat-0.1.4/chatchat/baidu.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from chatchat.base import Base
 import httpx, time
 
 class Completion(Base):
-    def __init__(self, model='ERNIE-Speed-8K'):
+    def __init__(self, model='ERNIE-Speed-8K', proxy=None, timeout=None):
         super().__init__()
 
         # https://console.bce.baidu.com/qianfan/ais/console/applicationConsole/application
         #     {
         #         "baidu": {
         #             "api_key": "x",
         #             "secret_key": "y",
@@ -30,15 +30,15 @@
             'ERNIE-Tiny-8K': 'ernie-tiny-8k',
             'Yi-34B-Chat': 'yi_34b_chat',
         }
 
         if model not in self.api_list:
             raise RuntimeError(f'supported chat type: {self.api_list.keys()}')
         self.api = 'https://aip.baidubce.com/rpc/2.0/ai_custom/v1/wenxinworkshop/chat/' + self.api_list[model]
-        self.client = httpx.Client()
+        self.client = httpx.Client(proxy=proxy, timeout=timeout)
         self.headers = {
             'Content-Type': 'application/json',
             'Accept': 'application/json'
         }
 
         self.update_access_token()
```

### Comparing `chatchat-0.1.3/chatchat/base.py` & `chatchat-0.1.4/chatchat/base.py`

 * *Files identical despite different names*

### Comparing `chatchat-0.1.3/chatchat/tencent.py` & `chatchat-0.1.4/chatchat/tencent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from chatchat.base import Base
 import hashlib, hmac, json, time
 from datetime import datetime
 import httpx
 
 class Completion(Base):
-    def __init__(self, model='hunyuan-lite'):
+    def __init__(self, model='hunyuan-lite', proxy=None, timeout=None):
         super().__init__()
 
         plat = 'tencent'
         self.verify_secret_data(plat, ('secret_id', 'secret_key'))
         self.jdata = self.secret_data[plat]
         self.secret_id = self.jdata['secret_id']
         self.secret_key = self.jdata['secret_key']
@@ -21,15 +21,15 @@
         ])
         if model not in self.model_type:
             raise RuntimeError(f'supported chat type: {list(self.model_type)}')
         self.model = model
 
         self.host = 'hunyuan.tencentcloudapi.com'
         self.endpoint = f'https://{self.host}'
-        self.client = httpx.Client()
+        self.client = httpx.Client(proxy=proxy, timeout=timeout)
 
     def encode_message(self, jmsg):
         # step 1
         http_request_method = "POST"
         canonical_uri = "/"
         canonical_querystring = ""
         ct = "application/json; charset=utf-8"
```

### Comparing `chatchat-0.1.3/chatchat/xunfei.py` & `chatchat-0.1.4/chatchat/xunfei.py`

 * *Files identical despite different names*

### Comparing `chatchat-0.1.3/setup.py` & `chatchat-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'chatchat',
     packages = find_packages(exclude=['examples']),
-    version = '0.1.3',
+    version = '0.1.4',
     license = 'GPL-2.0',
     description = 'Large Language Model API',
     author = 'JiauZhang',
     author_email = 'jiauzhang@163.com',
     url = 'https://github.com/JiauZhang/chatchat',
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type = 'text/markdown',
```

