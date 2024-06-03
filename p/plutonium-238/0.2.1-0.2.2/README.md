# Comparing `tmp/plutonium-238-0.2.1.tar.gz` & `tmp/plutonium-238-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plutonium-238-0.2.1.tar", last modified: Fri May 31 02:08:16 2024, max compression
+gzip compressed data, was "plutonium-238-0.2.2.tar", last modified: Mon Jun  3 10:57:41 2024, max compression
```

## Comparing `plutonium-238-0.2.1.tar` & `plutonium-238-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 john       (501) staff       (20)        0 2024-05-31 02:08:16.147294 plutonium-238-0.2.1/
--rw-r--r--   0 john       (501) staff       (20)      868 2024-05-31 02:08:16.146921 plutonium-238-0.2.1/PKG-INFO
--rw-r--r--   0 john       (501) staff       (20)       34 2023-03-02 03:59:40.000000 plutonium-238-0.2.1/README.md
-drwxr-xr-x   0 john       (501) staff       (20)        0 2024-05-31 02:08:16.142185 plutonium-238-0.2.1/plutonium/
--rw-r--r--   0 john       (501) staff       (20)        0 2023-01-17 14:47:08.000000 plutonium-238-0.2.1/plutonium/__init__.py
--rw-r--r--   0 john       (501) staff       (20)     6753 2024-05-31 02:00:51.000000 plutonium-238-0.2.1/plutonium/cli.py
--rw-r--r--   0 john       (501) staff       (20)     3190 2024-05-31 01:52:11.000000 plutonium-238-0.2.1/plutonium/config.py
--rw-r--r--   0 john       (501) staff       (20)     7802 2024-05-31 01:52:11.000000 plutonium-238-0.2.1/plutonium/utils.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2024-05-31 02:08:16.145886 plutonium-238-0.2.1/plutonium_238.egg-info/
--rw-r--r--   0 john       (501) staff       (20)      868 2024-05-31 02:08:16.000000 plutonium-238-0.2.1/plutonium_238.egg-info/PKG-INFO
--rw-r--r--   0 john       (501) staff       (20)      320 2024-05-31 02:08:16.000000 plutonium-238-0.2.1/plutonium_238.egg-info/SOURCES.txt
--rw-r--r--   0 john       (501) staff       (20)        1 2024-05-31 02:08:16.000000 plutonium-238-0.2.1/plutonium_238.egg-info/dependency_links.txt
--rw-r--r--   0 john       (501) staff       (20)       50 2024-05-31 02:08:16.000000 plutonium-238-0.2.1/plutonium_238.egg-info/entry_points.txt
--rw-r--r--   0 john       (501) staff       (20)        9 2024-05-31 02:08:16.000000 plutonium-238-0.2.1/plutonium_238.egg-info/requires.txt
--rw-r--r--   0 john       (501) staff       (20)       10 2024-05-31 02:08:16.000000 plutonium-238-0.2.1/plutonium_238.egg-info/top_level.txt
--rw-r--r--   0 john       (501) staff       (20)       38 2024-05-31 02:08:16.147378 plutonium-238-0.2.1/setup.cfg
--rw-r--r--   0 john       (501) staff       (20)     1205 2024-05-31 02:01:45.000000 plutonium-238-0.2.1/setup.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2024-06-03 10:57:41.570187 plutonium-238-0.2.2/
+-rw-r--r--   0 john       (501) staff       (20)      868 2024-06-03 10:57:41.569690 plutonium-238-0.2.2/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)       34 2023-03-02 03:59:40.000000 plutonium-238-0.2.2/README.md
+drwxr-xr-x   0 john       (501) staff       (20)        0 2024-06-03 10:57:41.560480 plutonium-238-0.2.2/plutonium/
+-rw-r--r--   0 john       (501) staff       (20)        0 2023-01-17 14:47:08.000000 plutonium-238-0.2.2/plutonium/__init__.py
+-rw-r--r--   0 john       (501) staff       (20)     6753 2024-05-31 02:00:51.000000 plutonium-238-0.2.2/plutonium/cli.py
+-rw-r--r--   0 john       (501) staff       (20)     3190 2024-06-03 10:57:10.000000 plutonium-238-0.2.2/plutonium/config.py
+-rw-r--r--   0 john       (501) staff       (20)    10947 2024-06-03 10:54:32.000000 plutonium-238-0.2.2/plutonium/utils.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2024-06-03 10:57:41.568792 plutonium-238-0.2.2/plutonium_238.egg-info/
+-rw-r--r--   0 john       (501) staff       (20)      868 2024-06-03 10:57:41.000000 plutonium-238-0.2.2/plutonium_238.egg-info/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)      320 2024-06-03 10:57:41.000000 plutonium-238-0.2.2/plutonium_238.egg-info/SOURCES.txt
+-rw-r--r--   0 john       (501) staff       (20)        1 2024-06-03 10:57:41.000000 plutonium-238-0.2.2/plutonium_238.egg-info/dependency_links.txt
+-rw-r--r--   0 john       (501) staff       (20)       50 2024-06-03 10:57:41.000000 plutonium-238-0.2.2/plutonium_238.egg-info/entry_points.txt
+-rw-r--r--   0 john       (501) staff       (20)        9 2024-06-03 10:57:41.000000 plutonium-238-0.2.2/plutonium_238.egg-info/requires.txt
+-rw-r--r--   0 john       (501) staff       (20)       10 2024-06-03 10:57:41.000000 plutonium-238-0.2.2/plutonium_238.egg-info/top_level.txt
+-rw-r--r--   0 john       (501) staff       (20)       38 2024-06-03 10:57:41.570435 plutonium-238-0.2.2/setup.cfg
+-rw-r--r--   0 john       (501) staff       (20)     1205 2024-06-03 10:57:20.000000 plutonium-238-0.2.2/setup.py
```

### Comparing `plutonium-238-0.2.1/PKG-INFO` & `plutonium-238-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plutonium-238
-Version: 0.2.1
+Version: 0.2.2
 Summary: SCA Agent, Copyright@Plutonium
 Home-page: https://www.google.com
 Author: tom
 Author-email: tom@google.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `plutonium-238-0.2.1/plutonium/cli.py` & `plutonium-238-0.2.2/plutonium/cli.py`

 * *Files identical despite different names*

### Comparing `plutonium-238-0.2.1/plutonium/config.py` & `plutonium-238-0.2.2/plutonium/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
    |       ____  _       _              _                   ____  _____  ___       |
    |      |  _ \| |_   _| |_ ___  _ __ (_)_   _ _ __ ___   |___ \|___ / ( _ )      |
    |      | |_) | | | | | __/ _ \| '_ \| | | | | '_ ` _ \    __) | |_ \ / _ \      |
    |      |  __/| | |_| | || (_) | | | | | |_| | | | | | |  / __/ ___) | (_) |     |
    |      |_|   |_|\__,_|\__\___/|_| |_|_|\__,_|_| |_| |_| |_____|____/ \___/      |
    |                                                                               |
    |                                                                               |
-   |                                                             version 0.2.1     |
+   |                                                             version 0.2.2     |
    |                                                                               |
    |                 This is a SCA Agent, Copyright@Plutonium Team                 |
    |                                                                               |
    |                                                                               |
    `-------------------------------------------------------------------------------'
 """
 # 结果轮询最大时间
```

### Comparing `plutonium-238-0.2.1/plutonium/utils.py` & `plutonium-238-0.2.2/plutonium/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import subprocess
 import logging
 import os
+import json
 import sys
 import zipfile
 import shutil
 import requests
 import plutonium.config as config
 from uuid import uuid4
 logger = logging.getLogger(__name__)
@@ -103,14 +104,67 @@
     logger.info(sca_args)
     exec_status = exec_tool(sca_args, config.LOG_FILENAME, timeout )
     result['status'] = exec_status['status']
     result['message'] = exec_status['message']
     result['data']['cmd'] = ' '.join(sca_args)
     return result
 
+def sca_by_opensca(bom_file, src_dir=".", log_file="",  timeout=config.CMD_TIME_OUT):
+    # 获取配置文件，配置maven等信息
+
+    result = {
+        'status': False,
+        'data': {
+            'cmd': '',
+            'result_file': bom_file
+        },
+        'message': '',
+    }
+    sca_args = ["opensca-cli", "-path", src_dir, "-config", config.TEMP_DIR+'/opensca_config.json', "-out", "{}".format(bom_file)]
+    exec_status = exec_tool(sca_args, config.LOG_FILENAME, timeout)
+    result['status'] = exec_status['status']
+    result['message'] = exec_status['message']
+    result['data']['cmd'] = ' '.join(sca_args)
+    return result
+def sca_by_jd_sbom_tool(bom_file, src_dir=".", log_file="",  timeout=config.CMD_TIME_OUT):
+    # 获取配置文件，配置maven等信息
+    result = {
+        'status': False,
+        'data': {
+            'cmd': '',
+            'result_file': bom_file
+        },
+        'message': '',
+    }
+    sca_args = ["sbom-tool", "-out ", bom_file, "-path", src_dir, "-log", log_file]
+    logger.info(sca_args)
+    exec_status = exec_tool(sca_args, config.LOG_FILENAME, timeout)
+    result['status'] = exec_status['status']
+    result['message'] = exec_status['message']
+    result['data']['cmd'] = ' '.join(sca_args)
+    return result
+
+def sca_by_fosseye(bom_file, src_dir=".", log_file="",  timeout=config.CMD_TIME_OUT):
+    # 获取配置文件，配置maven等信息
+
+    result = {
+        'status': False,
+        'data': {
+            'cmd': '',
+            'result_file': bom_file
+        },
+        'message': '',
+    }
+    sca_args = ["opensca-cli", "-out ", bom_file, "-path", src_dir, "-log", log_file]
+    logger.info(sca_args)
+    exec_status = exec_tool(sca_args, config.LOG_FILENAME, timeout)
+    result['status'] = exec_status['status']
+    result['message'] = exec_status['message']
+    result['data']['cmd'] = ' '.join(sca_args)
+    return result
 
 # 服务端检测
 class VoyagerDetect():
     def __init__(self, token=None, url=None, username=None, password=None, api=None):
         self.api_url = url
         self.api_token = token
         self.api_username = username
@@ -178,20 +232,48 @@
             else:
                 login_status['message'] = '无法生成访问token，账号密码可能错误'
         else:
             login_status['message'] = '请提供API账号以及密码信息'
         logger.info(login_status['message'])
         return login_status
 
+    def init_opensca(self):
+        login_status = self.login()
+        data = {
+            'type': 'get_opensca_config',
+        }
+        if login_status['status']:
+            response = self.req.post(self.api_url + config.VOYAGER_BASE_API, data=data,
+                                         files=[('files', ('', None,)), ])
+            try:
+                print(response.json())
+                if response.json().get('success'):
+                    config_data = response.json().get('data')
+                    print(config.TEMP_DIR+'opensca_config.json')
+                    with open(config.TEMP_DIR+'/opensca_config.json', 'w') as f:
+                        f.write(json.dumps(config_data))
+            except Exception as e:
+                logger.error(e)
+        else:
+            return login_status['message']
+
     # sca分析
     def sca_analysis(self, src_dir=".", tool='cdxgen'):
         if tool == 'cdxgen':
             result_file = config.DATA_DIR+'/{}_{}.json'.format(tool, uuid4().hex)
             return sca_by_cdxgen(result_file, src_dir)
-
+        elif tool == 'opensca':
+            self.init_opensca()
+            result_file = config.DATA_DIR+'/{}_{}.json'.format(tool, uuid4().hex)
+            log_file = config.DATA_DIR+'/{}_log_{}.log'.format(tool, uuid4().hex)
+            return sca_by_opensca(result_file, src_dir, log_file)
+        elif tool == 'jd-sbom-tool':
+            pass
+        elif tool == 'fosseye':
+            pass
         return None
 
     # upload
     def upload(self, data, files):
         login_status = self.login()
         if login_status['status']:
             if files:
```

### Comparing `plutonium-238-0.2.1/plutonium_238.egg-info/PKG-INFO` & `plutonium-238-0.2.2/plutonium_238.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plutonium-238
-Version: 0.2.1
+Version: 0.2.2
 Summary: SCA Agent, Copyright@Plutonium
 Home-page: https://www.google.com
 Author: tom
 Author-email: tom@google.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `plutonium-238-0.2.1/setup.py` & `plutonium-238-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="plutonium-238",
-    version="0.2.1",
+    version="0.2.2",
     author="tom",
     author_email="tom@google.com",
     description="SCA Agent, Copyright@Plutonium",
     entry_points={
         "console_scripts": ["plutonium=plutonium.cli:main",]
     },
     license="MIT",
```

