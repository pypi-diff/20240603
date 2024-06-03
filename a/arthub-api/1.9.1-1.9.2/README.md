# Comparing `tmp/arthub_api-1.9.1.tar.gz` & `tmp/arthub_api-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arthub_api-1.9.1.tar", last modified: Wed May 15 14:23:48 2024, max compression
+gzip compressed data, was "arthub_api-1.9.2.tar", last modified: Mon Jun  3 07:03:58 2024, max compression
```

## Comparing `arthub_api-1.9.1.tar` & `arthub_api-1.9.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 14:23:48.897526 arthub_api-1.9.1/
--rw-rw-rw-   0        0        0     1077 2022-09-05 10:15:53.000000 arthub_api-1.9.1/LICENSE
--rw-rw-rw-   0        0        0      107 2022-09-05 10:15:53.000000 arthub_api-1.9.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1412 2024-05-15 14:23:48.891542 arthub_api-1.9.1/PKG-INFO
--rw-rw-rw-   0        0        0      864 2023-05-19 06:20:15.000000 arthub_api-1.9.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 14:23:48.811207 arthub_api-1.9.1/arthub_api/
--rw-rw-rw-   0        0        0      675 2023-07-25 13:45:45.000000 arthub_api-1.9.1/arthub_api/__init__.py
--rw-rw-rw-   0        0        0     3049 2024-04-26 07:41:26.000000 arthub_api-1.9.1/arthub_api/__main__.py
--rw-rw-rw-   0        0        0      241 2024-05-15 14:23:08.000000 arthub_api-1.9.1/arthub_api/__version__.py
--rw-rw-rw-   0        0        0    13661 2023-05-11 11:13:51.000000 arthub_api-1.9.1/arthub_api/_internal_utils.py
--rw-rw-rw-   0        0        0      128 2024-04-26 07:41:26.000000 arthub_api-1.9.1/arthub_api/arthub_api_config.py
--rw-rw-rw-   0        0        0      501 2023-07-25 13:45:45.000000 arthub_api-1.9.1/arthub_api/asset_matrix.py
--rw-rw-rw-   0        0        0    43536 2023-07-25 13:45:45.000000 arthub_api-1.9.1/arthub_api/blade_api.py
--rw-rw-rw-   0        0        0     2072 2024-04-26 07:41:26.000000 arthub_api-1.9.1/arthub_api/blade_api_instance.py
--rw-rw-rw-   0        0        0    28990 2024-04-26 07:41:26.000000 arthub_api-1.9.1/arthub_api/blade_storage.py
--rw-rw-rw-   0        0        0       22 2023-02-08 16:32:42.000000 arthub_api-1.9.1/arthub_api/cli.py
--rw-rw-rw-   0        0        0     1443 2023-07-25 13:45:45.000000 arthub_api-1.9.1/arthub_api/config.py
--rw-rw-rw-   0        0        0      523 2023-02-08 16:32:42.000000 arthub_api-1.9.1/arthub_api/exception.py
--rw-rw-rw-   0        0        0     1465 2024-04-26 07:41:26.000000 arthub_api-1.9.1/arthub_api/models.py
--rw-rw-rw-   0        0        0    47584 2024-05-15 14:20:21.000000 arthub_api-1.9.1/arthub_api/open_api.py
--rw-rw-rw-   0        0        0    46992 2024-04-26 07:41:26.000000 arthub_api-1.9.1/arthub_api/storage.py
--rw-rw-rw-   0        0        0    10006 2024-04-26 07:41:26.000000 arthub_api-1.9.1/arthub_api/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-15 14:23:48.821181 arthub_api-1.9.1/arthub_api.egg-info/
--rw-rw-rw-   0        0        0     1412 2024-05-15 14:23:47.000000 arthub_api-1.9.1/arthub_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      790 2024-05-15 14:23:48.000000 arthub_api-1.9.1/arthub_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 14:23:47.000000 arthub_api-1.9.1/arthub_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-05-15 14:23:47.000000 arthub_api-1.9.1/arthub_api.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-03-14 07:53:40.000000 arthub_api-1.9.1/arthub_api.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      185 2024-05-15 14:23:47.000000 arthub_api-1.9.1/arthub_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-15 14:23:47.000000 arthub_api-1.9.1/arthub_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       63 2022-09-26 03:28:18.000000 arthub_api-1.9.1/requirements-dev.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 14:23:48.897526 arthub_api-1.9.1/setup.cfg
--rw-rw-rw-   0        0        0     3157 2024-04-26 07:41:26.000000 arthub_api-1.9.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-15 14:23:48.864614 arthub_api-1.9.1/tests/
--rw-rw-rw-   0        0        0      176 2023-07-25 13:45:45.000000 arthub_api-1.9.1/tests/__init__.py
--rw-rw-rw-   0        0        0      108 2023-05-19 06:20:15.000000 arthub_api-1.9.1/tests/_utils.py
--rw-rw-rw-   0        0        0      866 2024-04-26 07:41:26.000000 arthub_api-1.9.1/tests/conftest.py
--rw-rw-rw-   0        0        0     7139 2024-04-26 07:41:26.000000 arthub_api-1.9.1/tests/test_open_api.py
--rw-rw-rw-   0        0        0     3471 2024-04-26 07:41:26.000000 arthub_api-1.9.1/tests/test_storage.py
+drwxrwxrwx   0        0        0        0 2024-06-03 07:03:58.880889 arthub_api-1.9.2/
+-rw-rw-rw-   0        0        0     1077 2022-09-05 10:15:53.000000 arthub_api-1.9.2/LICENSE
+-rw-rw-rw-   0        0        0      107 2022-09-05 10:15:53.000000 arthub_api-1.9.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1412 2024-06-03 07:03:58.880372 arthub_api-1.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0      864 2023-05-19 06:20:15.000000 arthub_api-1.9.2/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 07:03:58.806235 arthub_api-1.9.2/arthub_api/
+-rw-rw-rw-   0        0        0      699 2024-06-03 06:55:08.000000 arthub_api-1.9.2/arthub_api/__init__.py
+-rw-rw-rw-   0        0        0     3049 2024-04-26 07:41:26.000000 arthub_api-1.9.2/arthub_api/__main__.py
+-rw-rw-rw-   0        0        0      241 2024-06-03 07:01:36.000000 arthub_api-1.9.2/arthub_api/__version__.py
+-rw-rw-rw-   0        0        0    13661 2023-05-11 11:13:51.000000 arthub_api-1.9.2/arthub_api/_internal_utils.py
+-rw-rw-rw-   0        0        0      128 2024-04-26 07:41:26.000000 arthub_api-1.9.2/arthub_api/arthub_api_config.py
+-rw-rw-rw-   0        0        0      501 2023-07-25 13:45:45.000000 arthub_api-1.9.2/arthub_api/asset_matrix.py
+-rw-rw-rw-   0        0        0    43536 2023-07-25 13:45:45.000000 arthub_api-1.9.2/arthub_api/blade_api.py
+-rw-rw-rw-   0        0        0     2072 2024-04-26 07:41:26.000000 arthub_api-1.9.2/arthub_api/blade_api_instance.py
+-rw-rw-rw-   0        0        0    28990 2024-04-26 07:41:26.000000 arthub_api-1.9.2/arthub_api/blade_storage.py
+-rw-rw-rw-   0        0        0       22 2023-02-08 16:32:42.000000 arthub_api-1.9.2/arthub_api/cli.py
+-rw-rw-rw-   0        0        0     1786 2024-06-03 06:55:08.000000 arthub_api-1.9.2/arthub_api/config.py
+-rw-rw-rw-   0        0        0      523 2023-02-08 16:32:42.000000 arthub_api-1.9.2/arthub_api/exception.py
+-rw-rw-rw-   0        0        0     1465 2024-04-26 07:41:26.000000 arthub_api-1.9.2/arthub_api/models.py
+-rw-rw-rw-   0        0        0    47672 2024-06-03 06:55:08.000000 arthub_api-1.9.2/arthub_api/open_api.py
+-rw-rw-rw-   0        0        0    46992 2024-04-26 07:41:26.000000 arthub_api-1.9.2/arthub_api/storage.py
+-rw-rw-rw-   0        0        0    10067 2024-06-03 06:55:08.000000 arthub_api-1.9.2/arthub_api/utils.py
+drwxrwxrwx   0        0        0        0 2024-06-03 07:03:58.835155 arthub_api-1.9.2/arthub_api.egg-info/
+-rw-rw-rw-   0        0        0     1412 2024-06-03 07:03:57.000000 arthub_api-1.9.2/arthub_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      790 2024-06-03 07:03:58.000000 arthub_api-1.9.2/arthub_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 07:03:57.000000 arthub_api-1.9.2/arthub_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-06-03 07:03:57.000000 arthub_api-1.9.2/arthub_api.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-06-03 07:03:57.000000 arthub_api-1.9.2/arthub_api.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      185 2024-06-03 07:03:57.000000 arthub_api-1.9.2/arthub_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-06-03 07:03:57.000000 arthub_api-1.9.2/arthub_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       63 2022-09-26 03:28:18.000000 arthub_api-1.9.2/requirements-dev.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 07:03:58.881392 arthub_api-1.9.2/setup.cfg
+-rw-rw-rw-   0        0        0     3157 2024-04-26 07:41:26.000000 arthub_api-1.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 07:03:58.859091 arthub_api-1.9.2/tests/
+-rw-rw-rw-   0        0        0      176 2023-07-25 13:45:45.000000 arthub_api-1.9.2/tests/__init__.py
+-rw-rw-rw-   0        0        0      108 2023-05-19 06:20:15.000000 arthub_api-1.9.2/tests/_utils.py
+-rw-rw-rw-   0        0        0      866 2024-04-26 07:41:26.000000 arthub_api-1.9.2/tests/conftest.py
+-rw-rw-rw-   0        0        0     7139 2024-04-26 07:41:26.000000 arthub_api-1.9.2/tests/test_open_api.py
+-rw-rw-rw-   0        0        0     3471 2024-04-26 07:41:26.000000 arthub_api-1.9.2/tests/test_storage.py
```

### Comparing `arthub_api-1.9.1/LICENSE` & `arthub_api-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `arthub_api-1.9.1/PKG-INFO` & `arthub_api-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arthub_api
-Version: 1.9.1
+Version: 1.9.2
 Summary: ArHhub Python SDK
 Home-page: UNKNOWN
 Author: Joey Ding
 Author-email: joeyding@tencent.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arthub_api-1.9.1/README.md` & `arthub_api-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `arthub_api-1.9.1/arthub_api/__init__.py` & `arthub_api-1.9.2/arthub_api/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,10 +38,11 @@
 from .models import (
     Result
 )
 
 from .config import (
     api_config_oa,
     api_config_qq,
+    api_config_public,
     api_config_oa_test,
     api_config_qq_test,
 )
```

### Comparing `arthub_api-1.9.1/arthub_api/__main__.py` & `arthub_api-1.9.2/arthub_api/__main__.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.9.1/arthub_api/_internal_utils.py` & `arthub_api-1.9.2/arthub_api/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.9.1/arthub_api/blade_api.py` & `arthub_api-1.9.2/arthub_api/blade_api.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.9.1/arthub_api/blade_api_instance.py` & `arthub_api-1.9.2/arthub_api/blade_api_instance.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.9.1/arthub_api/blade_storage.py` & `arthub_api-1.9.2/arthub_api/blade_storage.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.9.1/arthub_api/config.py` & `arthub_api-1.9.2/arthub_api/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 ~~~~~~~~~~~~~~
 
 This module provides configure that are used within API
 """
 # online configuration
 _api_host_oa = "service.arthub.woa.com"
 _api_host_qq = "service.arthub.qq.com"
+_api_host_public = "api.arthubdam.com"
 _client_proxy_host_oa = "client-proxy.arthub.woa.com"
 _client_proxy_host_qq = "client-proxy.arthub.qq.com"
+_client_proxy_host_public = "client-proxy.arthubdam.com"
 
 _api_host_oa_test = "arthub-service-test.woa.com"
 _api_host_qq_test = "arthub-innertest.qq.com"
 _client_proxy_host_oa_test = "arthub-client-proxy-test.woa.com"
 _client_proxy_host_qq_test = "arthub-storage-1.qq.com"
 
 # config for access ArtHub intranet domain
@@ -29,14 +31,23 @@
     "http_scheme": "https:",
     "web_socket_scheme": "wss:",
     "host": _api_host_qq,
     "client_proxy_host": _client_proxy_host_qq,
     "timeout": 10,
 }
 
+# config for access ArtHub public cloud version
+api_config_public = {
+    "http_scheme": "https:",
+    "web_socket_scheme": "wss:",
+    "host": _api_host_public,
+    "client_proxy_host": _client_proxy_host_public,
+    "timeout": 10,
+}
+
 # config for internal test
 api_config_oa_test = {
     "http_scheme": "http:",
     "web_socket_scheme": "ws:",
     "host": _api_host_oa_test,
     "client_proxy_host": _client_proxy_host_oa_test,
     "timeout": 5,
```

### Comparing `arthub_api-1.9.1/arthub_api/exception.py` & `arthub_api-1.9.2/arthub_api/exception.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.9.1/arthub_api/models.py` & `arthub_api-1.9.2/arthub_api/models.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.9.1/arthub_api/open_api.py` & `arthub_api-1.9.2/arthub_api/open_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -441,14 +441,17 @@
 
     def reset_config(self, config):
         self._config = config
 
     def init_from_config(self):
         self.reset_config(utils.get_config_by_name(arthub_api_config.api_config_name, self.config))
 
+    def base_url(self):
+        return "%s//%s" % (self.http_scheme, self.api_host)
+
     def _depot_url(self, asset_hub, api_method):
         return "%s//%s/%s/data/openapi/%s/core/%s" % (
             self.http_scheme, self.api_host, asset_hub, self._api_version_depot, api_method)
 
     def _gateway_url(self, api_method):
         return "%s//%s/gateway/gateway/openapi/%s/core/%s" % (
             self.http_scheme, self.api_host, self._api_version_gateway, api_method)
```

### Comparing `arthub_api-1.9.1/arthub_api/storage.py` & `arthub_api-1.9.2/arthub_api/storage.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.9.1/arthub_api/utils.py` & `arthub_api-1.9.2/arthub_api/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import string
 import requests
 from . import models
 from platformdirs import user_cache_dir
 from .config import (
     api_config_oa,
     api_config_qq,
+    api_config_public,
     api_config_oa_test,
     api_config_qq_test
 )
 from base64 import b64encode, b64decode
 from Crypto.PublicKey import RSA
 from Crypto.Cipher import PKCS1_OAEP
 from Crypto.Hash import SHA256
@@ -301,14 +302,15 @@
 
 def get_config_by_name(env, default_config=None):
     _env_map = {
         "oa": api_config_oa,
         "qq": api_config_qq,
         "oa_test": api_config_oa_test,
         "qq_test": api_config_qq_test,
+        "public": api_config_public
     }
     c = _env_map.get(env)
     if not c:
         if default_config:
             return default_config
         return api_config_oa
     return c
```

### Comparing `arthub_api-1.9.1/arthub_api.egg-info/PKG-INFO` & `arthub_api-1.9.2/arthub_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arthub-api
-Version: 1.9.1
+Version: 1.9.2
 Summary: ArHhub Python SDK
 Home-page: UNKNOWN
 Author: Joey Ding
 Author-email: joeyding@tencent.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arthub_api-1.9.1/arthub_api.egg-info/SOURCES.txt` & `arthub_api-1.9.2/arthub_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arthub_api-1.9.1/setup.py` & `arthub_api-1.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.9.1/tests/conftest.py` & `arthub_api-1.9.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.9.1/tests/test_open_api.py` & `arthub_api-1.9.2/tests/test_open_api.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.9.1/tests/test_storage.py` & `arthub_api-1.9.2/tests/test_storage.py`

 * *Files identical despite different names*

