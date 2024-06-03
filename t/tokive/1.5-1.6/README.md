# Comparing `tmp/tokive-1.5.tar.gz` & `tmp/tokive-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokive-1.5.tar", last modified: Tue Apr 16 05:16:55 2024, max compression
+gzip compressed data, was "tokive-1.6.tar", last modified: Mon Jun  3 15:13:55 2024, max compression
```

## Comparing `tokive-1.5.tar` & `tokive-1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:16:55.884127 tokive-1.5/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-16 05:16:55.884127 tokive-1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 05:16:48.000000 tokive-1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 05:16:55.884127 tokive-1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-16 05:16:48.000000 tokive-1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:16:55.880127 tokive-1.5/tokhelper/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-16 05:16:48.000000 tokive-1.5/tokhelper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-16 05:16:48.000000 tokive-1.5/tokhelper/captchaCheck_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5820 2024-04-16 05:16:48.000000 tokive-1.5/tokhelper/solve_captcha.py
--rw-r--r--   0 runner    (1001) docker     (127)    58756 2024-04-16 05:16:48.000000 tokive-1.5/tokhelper/tiktok_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-16 05:16:48.000000 tokive-1.5/tokhelper/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-16 05:16:48.000000 tokive-1.5/tokive
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:16:55.880127 tokive-1.5/tokive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-16 05:16:55.000000 tokive-1.5/tokive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-16 05:16:55.000000 tokive-1.5/tokive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 05:16:55.000000 tokive-1.5/tokive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-16 05:16:55.000000 tokive-1.5/tokive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-16 05:16:55.000000 tokive-1.5/tokive.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:13:55.345896 tokive-1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-06-03 15:13:55.345896 tokive-1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-06-03 15:13:47.000000 tokive-1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 15:13:55.345896 tokive-1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-06-03 15:13:47.000000 tokive-1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:13:55.341896 tokive-1.6/tokhelper/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-06-03 15:13:47.000000 tokive-1.6/tokhelper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-06-03 15:13:47.000000 tokive-1.6/tokhelper/captchaCheck_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5820 2024-06-03 15:13:47.000000 tokive-1.6/tokhelper/solve_captcha.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58760 2024-06-03 15:13:47.000000 tokive-1.6/tokhelper/tiktok_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-06-03 15:13:47.000000 tokive-1.6/tokhelper/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-06-03 15:13:47.000000 tokive-1.6/tokive
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:13:55.345896 tokive-1.6/tokive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-06-03 15:13:55.000000 tokive-1.6/tokive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-06-03 15:13:55.000000 tokive-1.6/tokive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 15:13:55.000000 tokive-1.6/tokive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-06-03 15:13:55.000000 tokive-1.6/tokive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-03 15:13:55.000000 tokive-1.6/tokive.egg-info/top_level.txt
```

### Comparing `tokive-1.5/setup.py` & `tokive-1.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='tokive',
-    version='1.5',
+    version='1.6',
     author="Thanh Hoa",
     author_email="thanhhoakhmt1@gmail.com",
     description="A Des of tokive",
     long_description="Des",
     long_description_content_type="text/markdown",
     url="https://github.com/AutoWinTeam/tokive",
     packages=setuptools.find_packages(),
```

### Comparing `tokive-1.5/tokhelper/captchaCheck_pb2.py` & `tokive-1.6/tokhelper/captchaCheck_pb2.py`

 * *Files identical despite different names*

### Comparing `tokive-1.5/tokhelper/solve_captcha.py` & `tokive-1.6/tokhelper/solve_captcha.py`

 * *Files identical despite different names*

### Comparing `tokive-1.5/tokhelper/tiktok_main.py` & `tokive-1.6/tokhelper/tiktok_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 import json, sys
 from tokhelper import captchaCheck_pb2
 from tokhelper.solve_captcha import TikTokCaptchaSolver
 from urllib.parse import urlencode
 import traceback
 URL_SESSION="https://autolive.vip/api/tiktok/commit"
 
-P_VERSION_CODE="0.54.0"
-P_WEBCAST_VERSION="540"
-P_BROWSER_VERSION="5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) TikTokLIVEStudio/0.54.0 Chrome/104.0.5112.102 Electron/20.1.0-tt.8.release.main.35 TTElectron/20.1.0-tt.8.release.main.35 Safari/537.36"
-H_USER_AGENT="Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) TikTokLIVEStudio/0.54.0 Chrome/104.0.5112.102 Electron/20.1.0-tt.8.release.main.35 TTElectron/20.1.0-tt.8.release.main.35 Safari/537.36"
+P_VERSION_CODE="0.57.0"
+P_WEBCAST_VERSION="570"
+P_BROWSER_VERSION="5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) TikTokLIVEStudio/0.57.0 Chrome/108.0.5359.215 Electron/22.3.18-tt.8.release.main.26 TTElectron/22.3.18-tt.8.release.main.26 Safari/537.36"
+H_USER_AGENT="Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) TikTokLIVEStudio/0.57.0 Chrome/108.0.5359.215 Electron/22.3.18-tt.8.release.main.26 TTElectron/22.3.18-tt.8.release.main.26 Safari/537.36"
 
 def load_tiktok_acc(id):
     url = f"https://autolive.vip/api/tiktok/load?id={id}"
     data = None
     try:
         headers={"platform":"Autolive"}
         res = requests.get(url, headers=headers).json()
```

### Comparing `tokive-1.5/tokhelper/utils.py` & `tokive-1.6/tokhelper/utils.py`

 * *Files identical despite different names*

### Comparing `tokive-1.5/tokive` & `tokive-1.6/tokive`

 * *Files identical despite different names*

