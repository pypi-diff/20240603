# Comparing `tmp/feeluown-bilibili-0.3.3.tar.gz` & `tmp/feeluown-bilibili-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feeluown-bilibili-0.3.3.tar", last modified: Fri Jan 26 16:54:48 2024, max compression
+gzip compressed data, was "feeluown-bilibili-0.4.0.tar", last modified: Mon Jun  3 13:31:52 2024, max compression
```

## Comparing `feeluown-bilibili-0.3.3.tar` & `feeluown-bilibili-0.4.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 16:54:48.857013 feeluown-bilibili-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-01-26 16:54:46.000000 feeluown-bilibili-0.3.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-01-26 16:54:48.857013 feeluown-bilibili-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-01-26 16:54:46.000000 feeluown-bilibili-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 16:54:48.853013 feeluown-bilibili-0.3.3/feeluown_bilibili.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-01-26 16:54:48.000000 feeluown-bilibili-0.3.3/feeluown_bilibili.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-01-26 16:54:48.000000 feeluown-bilibili-0.3.3/feeluown_bilibili.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 16:54:48.000000 feeluown-bilibili-0.3.3/feeluown_bilibili.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-26 16:54:48.000000 feeluown-bilibili-0.3.3/feeluown_bilibili.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-01-26 16:54:48.000000 feeluown-bilibili-0.3.3/feeluown_bilibili.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-26 16:54:48.000000 feeluown-bilibili-0.3.3/feeluown_bilibili.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 16:54:48.853013 feeluown-bilibili-0.3.3/fuo_bilibili/
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-01-26 16:54:46.000000 feeluown-bilibili-0.3.3/fuo_bilibili/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 16:54:48.857013 feeluown-bilibili-0.3.3/fuo_bilibili/api/
--rw-r--r--   0 runner    (1001) docker     (127)     6485 2024-01-26 16:54:46.000000 feeluown-bilibili-0.3.3/fuo_bilibili/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-01-26 16:54:46.000000 feeluown-bilibili-0.3.3/fuo_bilibili/api/audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-01-26 16:54:46.000000 feeluown-bilibili-0.3.3/fuo_bilibili/api/base.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-26 16:54:46.000000 feeluown-bilibili-0.3.3/fuo_bilibili/api/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-01-26 16:54:46.000000 feeluown-bilibili-0.3.3/fuo_bilibili/api/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-01-26 16:54:46.000000 feeluown-bilibili-0.3.3/fuo_bilibili/api/live.py
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-01-26 16:54:46.000000 feeluown-bilibili-0.3.3/fuo_bilibili/api/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-01-26 16:54:46.000000 feeluown-bilibili-0.3.3/fuo_bilibili/api/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-01-26 16:54:46.000000 feeluown-bilibili-0.3.3/fuo_bilibili/api/playlist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 16:54:48.857013 feeluown-bilibili-0.3.3/fuo_bilibili/api/schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 16:54:46.000000 feeluown-bilibili-0.3.3/fuo_bilibili/api/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-01-26 16:54:46.000000 feeluown-bilibili-0.3.3/fuo_bilibili/api/schema/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-01-26 16:54:46.000000 feeluown-bilibili-0.3.3/fuo_bilibili/api/schema/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)    26468 2024-01-26 16:54:46.000000 feeluown-bilibili-0.3.3/fuo_bilibili/api/schema/responses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-01-26 16:54:46.000000 feeluown-bilibili-0.3.3/fuo_bilibili/api/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-01-26 16:54:46.000000 feeluown-bilibili-0.3.3/fuo_bilibili/api/video.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-01-26 16:54:46.000000 feeluown-bilibili-0.3.3/fuo_bilibili/api/wbi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 16:54:48.857013 feeluown-bilibili-0.3.3/fuo_bilibili/assets/
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-01-26 16:54:46.000000 feeluown-bilibili-0.3.3/fuo_bilibili/assets/icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-01-26 16:54:46.000000 feeluown-bilibili-0.3.3/fuo_bilibili/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    40663 2024-01-26 16:54:46.000000 feeluown-bilibili-0.3.3/fuo_bilibili/danmaku2ass.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 16:54:48.857013 feeluown-bilibili-0.3.3/fuo_bilibili/geetest/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 16:54:46.000000 feeluown-bilibili-0.3.3/fuo_bilibili/geetest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7737 2024-01-26 16:54:46.000000 feeluown-bilibili-0.3.3/fuo_bilibili/geetest/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-01-26 16:54:46.000000 feeluown-bilibili-0.3.3/fuo_bilibili/geetest/server.py
--rw-r--r--   0 runner    (1001) docker     (127)    17123 2024-01-26 16:54:46.000000 feeluown-bilibili-0.3.3/fuo_bilibili/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-01-26 16:54:46.000000 feeluown-bilibili-0.3.3/fuo_bilibili/page_home.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-01-26 16:54:46.000000 feeluown-bilibili-0.3.3/fuo_bilibili/page_ranking.py
--rw-r--r--   0 runner    (1001) docker     (127)    28402 2024-01-26 16:54:46.000000 feeluown-bilibili-0.3.3/fuo_bilibili/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    15655 2024-01-26 16:54:46.000000 feeluown-bilibili-0.3.3/fuo_bilibili/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-01-26 16:54:46.000000 feeluown-bilibili-0.3.3/fuo_bilibili/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-01-26 16:54:46.000000 feeluown-bilibili-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-26 16:54:48.857013 feeluown-bilibili-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-01-26 16:54:46.000000 feeluown-bilibili-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:31:52.081682 feeluown-bilibili-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-03 13:31:44.000000 feeluown-bilibili-0.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-06-03 13:31:52.081682 feeluown-bilibili-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-06-03 13:31:44.000000 feeluown-bilibili-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:31:52.077682 feeluown-bilibili-0.4.0/feeluown_bilibili.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-06-03 13:31:51.000000 feeluown-bilibili-0.4.0/feeluown_bilibili.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-06-03 13:31:51.000000 feeluown-bilibili-0.4.0/feeluown_bilibili.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 13:31:51.000000 feeluown-bilibili-0.4.0/feeluown_bilibili.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-06-03 13:31:51.000000 feeluown-bilibili-0.4.0/feeluown_bilibili.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-06-03 13:31:51.000000 feeluown-bilibili-0.4.0/feeluown_bilibili.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-03 13:31:51.000000 feeluown-bilibili-0.4.0/feeluown_bilibili.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:31:52.081682 feeluown-bilibili-0.4.0/fuo_bilibili/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-06-03 13:31:44.000000 feeluown-bilibili-0.4.0/fuo_bilibili/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:31:52.081682 feeluown-bilibili-0.4.0/fuo_bilibili/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     5955 2024-06-03 13:31:44.000000 feeluown-bilibili-0.4.0/fuo_bilibili/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-06-03 13:31:44.000000 feeluown-bilibili-0.4.0/fuo_bilibili/api/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-06-03 13:31:44.000000 feeluown-bilibili-0.4.0/fuo_bilibili/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-06-03 13:31:44.000000 feeluown-bilibili-0.4.0/fuo_bilibili/api/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-06-03 13:31:44.000000 feeluown-bilibili-0.4.0/fuo_bilibili/api/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-06-03 13:31:44.000000 feeluown-bilibili-0.4.0/fuo_bilibili/api/live.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-06-03 13:31:44.000000 feeluown-bilibili-0.4.0/fuo_bilibili/api/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-06-03 13:31:44.000000 feeluown-bilibili-0.4.0/fuo_bilibili/api/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-06-03 13:31:44.000000 feeluown-bilibili-0.4.0/fuo_bilibili/api/playlist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:31:52.081682 feeluown-bilibili-0.4.0/fuo_bilibili/api/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:31:44.000000 feeluown-bilibili-0.4.0/fuo_bilibili/api/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-06-03 13:31:44.000000 feeluown-bilibili-0.4.0/fuo_bilibili/api/schema/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-06-03 13:31:44.000000 feeluown-bilibili-0.4.0/fuo_bilibili/api/schema/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26468 2024-06-03 13:31:44.000000 feeluown-bilibili-0.4.0/fuo_bilibili/api/schema/responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-06-03 13:31:44.000000 feeluown-bilibili-0.4.0/fuo_bilibili/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-06-03 13:31:44.000000 feeluown-bilibili-0.4.0/fuo_bilibili/api/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-06-03 13:31:44.000000 feeluown-bilibili-0.4.0/fuo_bilibili/api/wbi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:31:52.081682 feeluown-bilibili-0.4.0/fuo_bilibili/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-06-03 13:31:44.000000 feeluown-bilibili-0.4.0/fuo_bilibili/assets/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-06-03 13:31:44.000000 feeluown-bilibili-0.4.0/fuo_bilibili/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40663 2024-06-03 13:31:44.000000 feeluown-bilibili-0.4.0/fuo_bilibili/danmaku2ass.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:31:52.081682 feeluown-bilibili-0.4.0/fuo_bilibili/geetest/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:31:44.000000 feeluown-bilibili-0.4.0/fuo_bilibili/geetest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7737 2024-06-03 13:31:44.000000 feeluown-bilibili-0.4.0/fuo_bilibili/geetest/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-06-03 13:31:44.000000 feeluown-bilibili-0.4.0/fuo_bilibili/geetest/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18016 2024-06-03 13:31:44.000000 feeluown-bilibili-0.4.0/fuo_bilibili/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-06-03 13:31:44.000000 feeluown-bilibili-0.4.0/fuo_bilibili/page_home.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-06-03 13:31:44.000000 feeluown-bilibili-0.4.0/fuo_bilibili/page_ranking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28335 2024-06-03 13:31:44.000000 feeluown-bilibili-0.4.0/fuo_bilibili/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15886 2024-06-03 13:31:44.000000 feeluown-bilibili-0.4.0/fuo_bilibili/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-06-03 13:31:44.000000 feeluown-bilibili-0.4.0/fuo_bilibili/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-06-03 13:31:44.000000 feeluown-bilibili-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 13:31:52.081682 feeluown-bilibili-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-06-03 13:31:44.000000 feeluown-bilibili-0.4.0/setup.py
```

### Comparing `feeluown-bilibili-0.3.3/LICENSE.txt` & `feeluown-bilibili-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `feeluown-bilibili-0.3.3/README.md` & `feeluown-bilibili-0.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ![Libraries.io dependency status for GitHub repo](https://img.shields.io/librariesio/github/brucezhang1993/feeluown-bilibili?style=for-the-badge)
 
 ## Prerequisite
 
 You must have [FeelUOwn](https://github.com/feeluown/FeelUOwn) first
 
 - Python >= 3.10
-- FeelUOwn >= 3.8.14
+- FeelUOwn >= 4.1.5
 
 ## Installation
 
 ### PyPI
 
 https://pypi.org/project/feeluown-bilibili/
```

### Comparing `feeluown-bilibili-0.3.3/feeluown_bilibili.egg-info/SOURCES.txt` & `feeluown-bilibili-0.4.0/feeluown_bilibili.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feeluown-bilibili-0.3.3/fuo_bilibili/__init__.py` & `feeluown-bilibili-0.4.0/fuo_bilibili/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,17 +13,25 @@
 from fuo_bilibili.provider import BilibiliProvider
 from fuo_bilibili.ui import BUiManager
 
 provider = BilibiliProvider()
 ui_mgr: Optional[BUiManager] = None
 
 
+def init_config(config):
+    config.deffield('ENABLE_LIVE_ROOM_AS_VIDEO',
+                    type_=bool,
+                    default=True,
+                    desc='treat live room as video')
+
+
 # noinspection PyProtectedMember
 def enable(app: Union[App, GuiApp]):
     global ui_mgr
+    provider.enable_live_room_as_video = app.config.bilibili.ENABLE_LIVE_ROOM_AS_VIDEO
     app.library.register(provider)
     if app.mode & App.GuiMode:
         ui_mgr = BUiManager(app, provider)
 
 
 def disable(app: App):
     app.library.deregister(provider)
```

### Comparing `feeluown-bilibili-0.3.3/fuo_bilibili/api/__init__.py` & `feeluown-bilibili-0.4.0/fuo_bilibili/api/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,49 +31,29 @@
     def __init__(self):
         self._headers = {
             'Referer': 'https://www.bilibili.com/',
             'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_9_2)'
                           ' AppleWebKit/537.36 (KHTML, like Gecko)'
                           ' Chrome/33.0.1750.152 Safari/537.36'
         }
-        self._cookie = MozillaCookieJar(PLUGIN_API_COOKIEJAR_FILE)
         self._session = requests.Session()
         # UPDATE(2024-01-11): To make self.nav_info work, the header needs to be added
         # UPDATE(2023-xx-xx): The header cause some API failing: self.nav_info
         self._session.headers.update(self._headers)
-        self._session.cookies = self._cookie
         self._wbi: Optional[NavInfoResponse.NavInfoResponseData.Wbi] = None
 
-    @staticmethod
-    def cookie_check():
-        if not PLUGIN_API_COOKIEJAR_FILE.exists():
-            return False
-        return True
-
     def get_session(self):
         return self._session
 
-    def get_cookies(self):
+    def get_cookiejar(self):
         return self._session.cookies
 
-    @staticmethod
-    def remove_cookie():
-        PLUGIN_API_COOKIEJAR_FILE.unlink(missing_ok=True)
-
-    def from_cookiejar(self, jar: CookieJar):
-        for cookie in jar:
-            if 'bilibili.com' in cookie.domain:
-                self._cookie.set_cookie(cookie)
-        self._dump_cookie_to_file()
-
-    def load_cookies(self):
-        self._cookie.load()
-
-    def _dump_cookie_to_file(self):
-        self._cookie.save()
+    def from_cookiedict(self, cookies):
+        cookiejar = requests.cookies.cookiejar_from_dict(cookies)
+        self._session.cookies = cookiejar
 
     def set_wbi(self, wbi: NavInfoResponse.NavInfoResponseData.Wbi):
         self._wbi = wbi
 
     @staticmethod
     def clear_cache_by_url(urls: List[str]):
         for key in CACHE.keys():
```

### Comparing `feeluown-bilibili-0.3.3/fuo_bilibili/api/audio.py` & `feeluown-bilibili-0.4.0/fuo_bilibili/api/audio.py`

 * *Files identical despite different names*

### Comparing `feeluown-bilibili-0.3.3/fuo_bilibili/api/base.py` & `feeluown-bilibili-0.4.0/fuo_bilibili/api/base.py`

 * *Files identical despite different names*

### Comparing `feeluown-bilibili-0.3.3/fuo_bilibili/api/history.py` & `feeluown-bilibili-0.4.0/fuo_bilibili/api/history.py`

 * *Files identical despite different names*

### Comparing `feeluown-bilibili-0.3.3/fuo_bilibili/api/live.py` & `feeluown-bilibili-0.4.0/fuo_bilibili/api/live.py`

 * *Files identical despite different names*

### Comparing `feeluown-bilibili-0.3.3/fuo_bilibili/api/login.py` & `feeluown-bilibili-0.4.0/fuo_bilibili/api/login.py`

 * *Files identical despite different names*

### Comparing `feeluown-bilibili-0.3.3/fuo_bilibili/api/media.py` & `feeluown-bilibili-0.4.0/fuo_bilibili/api/media.py`

 * *Files identical despite different names*

### Comparing `feeluown-bilibili-0.3.3/fuo_bilibili/api/playlist.py` & `feeluown-bilibili-0.4.0/fuo_bilibili/api/playlist.py`

 * *Files identical despite different names*

### Comparing `feeluown-bilibili-0.3.3/fuo_bilibili/api/schema/enums.py` & `feeluown-bilibili-0.4.0/fuo_bilibili/api/schema/enums.py`

 * *Files identical despite different names*

### Comparing `feeluown-bilibili-0.3.3/fuo_bilibili/api/schema/requests.py` & `feeluown-bilibili-0.4.0/fuo_bilibili/api/schema/requests.py`

 * *Files identical despite different names*

### Comparing `feeluown-bilibili-0.3.3/fuo_bilibili/api/schema/responses.py` & `feeluown-bilibili-0.4.0/fuo_bilibili/api/schema/responses.py`

 * *Files identical despite different names*

### Comparing `feeluown-bilibili-0.3.3/fuo_bilibili/api/user.py` & `feeluown-bilibili-0.4.0/fuo_bilibili/api/user.py`

 * *Files identical despite different names*

### Comparing `feeluown-bilibili-0.3.3/fuo_bilibili/api/video.py` & `feeluown-bilibili-0.4.0/fuo_bilibili/api/video.py`

 * *Files identical despite different names*

### Comparing `feeluown-bilibili-0.3.3/fuo_bilibili/api/wbi.py` & `feeluown-bilibili-0.4.0/fuo_bilibili/api/wbi.py`

 * *Files identical despite different names*

### Comparing `feeluown-bilibili-0.3.3/fuo_bilibili/assets/icon.svg` & `feeluown-bilibili-0.4.0/fuo_bilibili/assets/icon.svg`

 * *Files identical despite different names*

### Comparing `feeluown-bilibili-0.3.3/fuo_bilibili/const.py` & `feeluown-bilibili-0.4.0/fuo_bilibili/const.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 FEELUOWN_DIRECTORY = Path.home() / '.FeelUOwn'
 PLUGIN_DATA_DIRECTORY = FEELUOWN_DIRECTORY / 'fuo_bilibili'
 DANMAKU_DIRECTORY = PLUGIN_DATA_DIRECTORY / 'subtitles'
 
 # Cookiejar file
 PLUGIN_API_COOKIEJAR_FILE = PLUGIN_DATA_DIRECTORY / 'bilibili_api.cookie'
+PLUGIN_API_COOKIEDICT_FILE = PLUGIN_DATA_DIRECTORY / 'bilibili_api_cookie.json'
 
 # Ensure directories
 PLUGIN_DATA_DIRECTORY.mkdir(parents=True, exist_ok=True)
 DANMAKU_DIRECTORY.mkdir(parents=True, exist_ok=True)
 
 # Clear old files
 for f in DANMAKU_DIRECTORY.glob('*.ass'):
```

### Comparing `feeluown-bilibili-0.3.3/fuo_bilibili/danmaku2ass.py` & `feeluown-bilibili-0.4.0/fuo_bilibili/danmaku2ass.py`

 * *Files identical despite different names*

### Comparing `feeluown-bilibili-0.3.3/fuo_bilibili/geetest/index.html` & `feeluown-bilibili-0.4.0/fuo_bilibili/geetest/index.html`

 * *Files identical despite different names*

### Comparing `feeluown-bilibili-0.3.3/fuo_bilibili/geetest/server.py` & `feeluown-bilibili-0.4.0/fuo_bilibili/geetest/server.py`

 * *Files identical despite different names*

### Comparing `feeluown-bilibili-0.3.3/fuo_bilibili/model.py` & `feeluown-bilibili-0.4.0/fuo_bilibili/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,24 @@
     AudioPlaylistSong, VideoHotCommentsResponse, SearchResultUser, LiveFeedListResponse, SearchResultLiveRoom, \
     SearchResultMedia, MediaGetListResponse, VideoWeeklyListResponse
 from fuo_bilibili.util import format_timedelta_to_hms
 
 PROVIDER_ID = __identifier__
 
 
+def get_text_from_html(html):
+    return BeautifulSoup(html, features="html.parser").get_text()
+
+
+def wrap_pic(pic):
+    if pic.startswith('//'):
+        return f'http:{pic}'
+    return pic
+
+
 class BBriefAlbumModel(BriefAlbumModel):
     cover: str = ''
 
 
 class BSongModel(SongModel):
     source: str = PROVIDER_ID
 
@@ -104,15 +114,15 @@
             song = cls(
                 source=__identifier__,
                 identifier=f'paged_{result.bvid}__{page.page}',
                 album=None,
                 title=page.part,
                 artists=[],
                 duration=page.duration.total_seconds() * 1000,
-                pic_url=result.pic,
+                pic_url=wrap_pic(result.pic),
             )
             children.append(song)
 
         return cls(
             source=__identifier__,
             identifier=result.bvid,
             album=BBriefAlbumModel(
@@ -126,15 +136,15 @@
             artists=[BriefArtistModel(
                 source=PROVIDER_ID,
                 identifier=result.owner.mid,
                 name=result.owner.name,
             )],
             duration=result.duration.total_seconds() * 1000,
             lyric=lrc or '',
-            pic_url=result.pic,
+            pic_url=wrap_pic(result.pic),
             children=children,
         )
 
     @classmethod
     def create_history_brief_model(cls, media):
         return BriefSongModel(
             source=__identifier__,
@@ -237,14 +247,15 @@
                 results += r.data.result
         else:
             results = response.data.result or []
         # fixme: implements multiple search types
         for result in results:
             if isinstance(result, SearchResultVideo):
                 songs.append(BSongModel.create_model(result))
+                videos.append(BVideoModel.create_video_model(result))
             elif isinstance(result, SearchResultUser):
                 artists.append(cls.search_user_model(result))
             elif isinstance(result, SearchResultLiveRoom):
                 videos.append(cls.search_live_model(result))
             elif isinstance(result, SearchResultMedia):
                 albums.append(cls.search_media_model(result))
         return SimpleSearchResult(
@@ -473,7 +484,25 @@
                     identifier=live.uid,
                     name=live.uname
                 )
             ],
             duration=0,
             cover=live.cover,
         )
+
+    @classmethod
+    def create_video_model(cls, result: SearchResultVideo) -> 'VideoModel':
+        return VideoModel(
+            source=__identifier__,
+            identifier=result.bvid,
+            title=get_text_from_html(result.title),
+            artists=[BriefArtistModel(
+                source=__identifier__,
+                name=result.author,
+                identifier=result.mid
+            )],
+            duration=result.duration.total_seconds(),
+            cover=wrap_pic(result.pic),
+            play_count=result.play,
+            released=result.pubdate.strftime('%Y-%m-%d'),
+        )
+
```

### Comparing `feeluown-bilibili-0.3.3/fuo_bilibili/page_home.py` & `feeluown-bilibili-0.4.0/fuo_bilibili/page_home.py`

 * *Files identical despite different names*

### Comparing `feeluown-bilibili-0.3.3/fuo_bilibili/page_ranking.py` & `feeluown-bilibili-0.4.0/fuo_bilibili/page_ranking.py`

 * *Files identical despite different names*

### Comparing `feeluown-bilibili-0.3.3/fuo_bilibili/provider.py` & `feeluown-bilibili-0.4.0/fuo_bilibili/provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,16 @@
 from fuo_bilibili.const import DANMAKU_DIRECTORY
 from fuo_bilibili.danmaku2ass import Danmaku2ASS
 from fuo_bilibili.model import BSearchModel, BSongModel, BPlaylistModel, BArtistModel, BCommentModel, BVideoModel, \
     BAlbumModel
 from fuo_bilibili.util import json_to_lrc_text
 
 SEARCH_TYPE_MAP = {
-    FuoSearchType.vi: BilibiliSearchType.LIVE_ROOM,  # 对应直播间
+    # 对应直播间
+    FuoSearchType.vi: BilibiliSearchType.LIVE_ROOM,
     FuoSearchType.ar: BilibiliSearchType.BILI_USER,  # 对应B站用户
     FuoSearchType.so: BilibiliSearchType.VIDEO,  # 对应投稿视频
     FuoSearchType.al: (BilibiliSearchType.MEDIA, BilibiliSearchType.BANGUMI),  # 对应番剧电影
 }
 
 
 def is_child_model(model):
@@ -96,49 +97,45 @@
             ModelType.song: (Pf.model_v2 | Pf.get | Pf.multi_quality | Pf.lyric | Pf.mv | Pf.similar | Pf.hot_comments),
             ModelType.video: (Pf.model_v2 | Pf.multi_quality | Pf.get),
             ModelType.playlist: (Pf.model_v2 | Pf.get | Pf.songs_rd | Pf.add_song | Pf.remove_song),
             ModelType.artist: (Pf.model_v2 | Pf.get | Pf.songs_rd),
             ModelType.album: (Pf.model_v2 | Pf.get),
         }
 
-    def __init__(self):
+    def __init__(self, enable_live_room_as_video=True):
         super(BilibiliProvider, self).__init__()
         self._api = BilibiliApi()
         self._user = None
         self._video_quality_codes = dict()
         self._video_cids = dict()
         self._video_avids = dict()
 
+        self.enable_live_room_as_video = enable_live_room_as_video
+
     def _format_search_request(self, keyword, type_) -> Union[SearchRequest, Tuple[SearchRequest]]:
-        btype = SEARCH_TYPE_MAP.get(type_)
+        if self.enable_live_room_as_video is False and type_ == FuoSearchType.vi:
+            btype = BilibiliSearchType.VIDEO
+        else:
+            btype = SEARCH_TYPE_MAP.get(type_)
         if btype is None:
             raise NotImplementedError
         if isinstance(btype, Tuple):
             return tuple([SearchRequest(search_type=t, keyword=keyword) for t in btype])
         return SearchRequest(search_type=btype, keyword=keyword)
 
     def request_captcha(self) -> RequestCaptchaResponse.RequestCaptchaResponseData:
         res = self._api.request_captcha()
         assert hasattr(res.data, 'geetest') and res.data.geetest is not None
         return res.data
 
     def request_key(self) -> RequestLoginKeyResponse:
         return self._api.request_login_key()
 
-    def cookie_check(self):
-        return self._api.cookie_check()
-
-    def auth(self, _):
-        self._api.load_cookies()
-        try:
-            self._user = self.user_info()
-        except RuntimeError as re:
-            self._api.remove_cookie()
-            print(str(re) + ' 请重新登录')
-        return self._user
+    def auth(self, user):
+        self._user = user
 
     def has_current_user(self) -> bool:
         return self._user is not None
 
     def get_current_user(self):
         if self._user is None:
             raise NoUserLoggedIn
@@ -341,15 +338,14 @@
             fnval=VideoFnval.DASH
         ))
         # select audio
         audios = sorted(response.data.dash.audio, key=lambda a: a.bandwidth, reverse=True)
         if audios is None or len(audios) == 0:
             return None
         # select video
-        print(response.data.dash.video)
         max_quality_code = VideoQualityNum.get_max_from_quality(quality)
         select_quality = max(filter(lambda c: c.value <= max_quality_code, self._video_quality_codes[video.identifier]),
                              key=lambda c: c.value)
         videos = sorted(filter(lambda a: a.id <= select_quality.value, response.data.dash.video), key=lambda a: a.id,
                         reverse=True)
         if videos is None or len(videos) == 0:
             return None
```

### Comparing `feeluown-bilibili-0.3.3/fuo_bilibili/ui.py` & `feeluown-bilibili-0.4.0/fuo_bilibili/ui.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,66 @@
 import asyncio
 import logging
+import json
 from pathlib import Path
 from typing import Optional
 
 from PyQt5.QtCore import Qt, pyqtSignal
 from PyQt5.QtGui import QCloseEvent
 from PyQt5.QtWidgets import QDialog, QLineEdit, QVBoxLayout, QPushButton, QLabel, QFrame, QTabWidget, QMessageBox, \
     QAction, QInputDialog, QWidget
 from feeluown.app.gui_app import GuiApp
 from feeluown.gui import ProviderUiManager
+from feeluown.gui.widgets.login import CookiesLoginDialog, InvalidCookies
 from feeluown.library import UserModel
+from feeluown.utils.aio import run_fn
 
 from fuo_bilibili import __identifier__, __alias__, BilibiliProvider
 from fuo_bilibili.api.schema.requests import PasswordLoginRequest, SendSmsCodeRequest, SmsCodeLoginRequest
 from fuo_bilibili.api.schema.responses import RequestLoginKeyResponse
 from fuo_bilibili.geetest.server import GeetestAuthServer
 from fuo_bilibili.util import rsa_encrypt, get_random_available_port
+from fuo_bilibili.const import PLUGIN_API_COOKIEDICT_FILE
 
 logger = logging.getLogger(__name__)
 
 
-class KeyringLoginWidget(QWidget):
-    finished = pyqtSignal()
+class LoginDialog(CookiesLoginDialog):
 
     def __init__(self, provider: BilibiliProvider, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self._provider = provider
-        self._chrome_btn = QPushButton('从 Chrome 中读取 Cookie')
+        self.provider = provider
 
-        self._layout = QVBoxLayout(self)
-        self._layout.addWidget(self._chrome_btn)
-        self._chrome_btn.clicked.connect(self._get_cookies_from_chrome)
+    def setup_user(self, user):
+        self.provider.auth(user)
 
-    def _get_cookies_from_chrome(self):
-        from feeluown.utils.yt_dlp_cookies import load_cookies
-        jar = load_cookies(None, ['chrome'], None)
-        self._provider.cookiejar_login(jar)
-        self.finished.emit()
+    async def user_from_cookies(self, cookies):
+        if not cookies:  # is None or empty
+            raise InvalidCookies('empty cookies')
 
-    @classmethod
-    def is_supported(cls):
+        self.provider._api.from_cookiedict(cookies)
         try:
-            from feeluown.utils.yt_dlp_cookies import load_cookies  # noqa
-        except ImportError:
-            return False
-        return True
+            user = await run_fn(self.provider.user_info)
+        except RuntimeError as e:
+            raise InvalidCookies(f'get user with cookies failed: {e}')
+        return user
+
+    def load_user_cookies(self):
+        if PLUGIN_API_COOKIEDICT_FILE.exists():
+            with PLUGIN_API_COOKIEDICT_FILE.open('r', encoding='utf-8') as f:
+                try:
+                    cookie_dict = json.load(f)
+                except Exception:
+                    logger.warning('parse cookies(json) failed')
+                    return None
+            return cookie_dict
+
+    def dump_user_cookies(self, _, cookies):
+        with PLUGIN_API_COOKIEDICT_FILE.open('w', encoding='utf-8') as f:
+            json.dump(cookies, f, indent=2)
 
 
 class BAuthDialog(QDialog):
     """
     人机验证
     """
     # signal: validate, seccode, challenge, token, type
@@ -193,24 +205,14 @@
         self.ok_btn.clicked.connect(self._start_auth)
 
         # NOTE(cosven, 2023-08-01): 这两个登录方法已经不可用了
         self._sms_tab.hide()
         self._pw_tab.hide()
         # self._tab.addTab(self._sms_tab, '验证码登录')
         # self._tab.addTab(self._pw_tab, '密码登录')
-        if KeyringLoginWidget.is_supported():
-            # keyring 登录
-            self._keyring_tab = KeyringLoginWidget(self._provider, parent=self._tab)
-            self._tab.addTab(self._keyring_tab, 'Keyring 登录')
-            self._keyring_tab.finished.connect(self._finish_keyring_login)
-        else:
-            self._tab.addTab(
-                QLabel('登录功能从 2023-08-01 开始，已经无法使用', self),
-                '提示',
-            )
 
         # auth back signal
         # noinspection PyUnresolvedReferences
         self._auth_dialog.auth_success.connect(self._auth_back)
 
     def _finish_keyring_login(self):
         self.close()
@@ -299,28 +301,28 @@
         self._pvd_item = self._pvd_uimgr.create_item(
             name=__identifier__,
             text=__alias__,
             symbol='📺',
             desc='点击登录',
             colorful_svg=(Path(__file__).parent / 'assets' / 'icon.svg').as_posix()
         )
-        self._pvd_item.clicked.connect(self._login_or_get_user)
+        self._pvd_item.clicked.connect(self.login_or_go_home)
         self._pvd_uimgr.add_item(self._pvd_item)
-        self.login_dialog = BLoginDialog(None, self._provider)
+
+        self.login_dialog = None
+
         # 新建收藏夹
         pl_header = self._app.ui.left_panel.playlists_header
         pl_header.setContextMenuPolicy(Qt.ActionsContextMenu)
         new_pl_action = QAction('新建收藏夹', pl_header)
         pl_header.addAction(new_pl_action)
         # noinspection PyUnresolvedReferences
         new_pl_action.triggered.connect(self.new_playlist)
         self._initial_pages()
 
-        self.login_dialog.login_succeed.connect(self._login_or_get_user)
-
     def new_playlist(self):
         name, o1 = QInputDialog.getText(self._app.ui.left_panel.playlists_header, '新建收藏夹', '收藏夹标题')
         if not o1:
             return
         desc, o2 = QInputDialog.getText(self._app.ui.left_panel.playlists_header, '新建收藏夹', '收藏夹简介')
         if not o2:
             return
@@ -366,18 +368,24 @@
         self._app.pl_uimgr.add(fav_playlists, is_fav=True)
         # 音频区
         audio_fav_list = self._provider.audio_favorite_playlists()
         audio_coll_list = self._provider.audio_collected_playlists()
         self._app.pl_uimgr.add(audio_fav_list)
         self._app.pl_uimgr.add(audio_coll_list, is_fav=True)
 
-    def _login(self):
-        self._user = self._provider.auth(None)
-        if self._user is not None:
-            self._pvd_item.text = f'{__alias__}已登录：{self._user.name} UID:{self._user.identifier}'
+    def after_login_succeed(self):
+        user = self._provider.get_current_user()
+        assert user is not None
+        self._user = user
+        self._pvd_item.text = f'{__alias__}已登录：{self._user.name} UID:{self._user.identifier}'
         asyncio.ensure_future(self.load_user_content())
 
-    def _login_or_get_user(self):
-        if self._provider.cookie_check():
-            self._login()
-            return
-        self.login_dialog.show()
+    def login_or_go_home(self):
+        if self._provider._user is None:
+            # keyring 登录
+            self.login_dialog = LoginDialog(
+                self._provider, 'https://bilibili.com', ['SESSDATA'])
+            self.login_dialog.login_succeed.connect(self.after_login_succeed)
+            self.login_dialog.autologin()
+            self.login_dialog.show()
+        else:
+            self.after_login_succeed()
```

### Comparing `feeluown-bilibili-0.3.3/fuo_bilibili/util.py` & `feeluown-bilibili-0.4.0/fuo_bilibili/util.py`

 * *Files identical despite different names*

### Comparing `feeluown-bilibili-0.3.3/pyproject.toml` & `feeluown-bilibili-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `feeluown-bilibili-0.3.3/setup.py` & `feeluown-bilibili-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,22 +7,22 @@
  'fuo_bilibili.api.schema',
  'fuo_bilibili.geetest']
 
 package_data = \
 {'': ['*'], 'fuo_bilibili': ['assets/*']}
 
 install_requires = \
-['beautifulsoup4', 'cachetools', 'feeluown>=3.8.14', 'pycryptodome']
+['beautifulsoup4', 'cachetools', 'feeluown>=4.1.5', 'pycryptodome']
 
 entry_points = \
 {'fuo.plugins_v1': ['bilibili = fuo_bilibili']}
 
 setup_kwargs = {
     'name': 'feeluown-bilibili',
-    'version': '0.3.3',
+    'version': '0.4.0',
     'description': 'Bilibili provider for FeelUOwn player.',
     'author': 'Bruce Zhang',
     'url': 'https://github.com/feeluown/feeluown-bilibili',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
```

