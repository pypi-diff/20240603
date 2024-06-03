# Comparing `tmp/aily_code_sdk_core-0.1.0b5.tar.gz` & `tmp/aily_code_sdk_core-0.1.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aily_code_sdk_core-0.1.0b5.tar", max compression
+gzip compressed data, was "aily_code_sdk_core-0.1.0b6.tar", max compression
```

## Comparing `aily_code_sdk_core-0.1.0b5.tar` & `aily_code_sdk_core-0.1.0b6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    10947 2024-05-29 05:58:44.305920 aily_code_sdk_core-0.1.0b5/LICENSE
--rw-r--r--   0        0        0      446 2024-05-29 05:58:44.306203 aily_code_sdk_core-0.1.0b5/README.md
--rw-r--r--   0        0        0      533 2024-05-30 08:17:33.488769 aily_code_sdk_core-0.1.0b5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-29 05:58:44.306688 aily_code_sdk_core-0.1.0b5/src/aily_code_sdk_core/__init__.py
--rw-r--r--   0        0        0       71 2024-05-29 05:58:44.307011 aily_code_sdk_core-0.1.0b5/src/aily_code_sdk_core/action/__init__.py
--rw-r--r--   0        0        0     1787 2024-05-30 04:08:44.777729 aily_code_sdk_core-0.1.0b5/src/aily_code_sdk_core/action/call_action.py
--rw-r--r--   0        0        0     1390 2024-05-29 06:39:31.368996 aily_code_sdk_core-0.1.0b5/src/aily_code_sdk_core/common/context.py
--rw-r--r--   0        0        0      541 2024-05-29 09:20:25.222586 aily_code_sdk_core-0.1.0b5/src/aily_code_sdk_core/common/util.py
--rw-r--r--   0        0        0       74 2024-05-29 05:58:44.308002 aily_code_sdk_core-0.1.0b5/src/aily_code_sdk_core/credential/__init__.py
--rw-r--r--   0        0        0     1593 2024-05-29 05:58:44.308159 aily_code_sdk_core-0.1.0b5/src/aily_code_sdk_core/credential/credential.py
--rw-r--r--   0        0        0       74 2024-05-29 05:58:44.308382 aily_code_sdk_core-0.1.0b5/src/aily_code_sdk_core/env/__init__.py
--rw-r--r--   0        0        0      437 2024-05-29 06:18:31.530058 aily_code_sdk_core-0.1.0b5/src/aily_code_sdk_core/env/get_env_info.py
--rw-r--r--   0        0        0      752 2024-05-29 05:58:44.308918 aily_code_sdk_core-0.1.0b5/src/aily_code_sdk_core/message/builder.py
--rw-r--r--   0        0        0      682 2024-05-29 05:58:44.309181 aily_code_sdk_core-0.1.0b5/src/aily_code_sdk_core/message/components/__init__.py
--rw-r--r--   0        0        0     1840 2024-05-29 05:58:44.309338 aily_code_sdk_core-0.1.0b5/src/aily_code_sdk_core/message/components/base_component.py
--rw-r--r--   0        0        0     1556 2024-05-29 05:58:44.309521 aily_code_sdk_core-0.1.0b5/src/aily_code_sdk_core/message/components/button.py
--rw-r--r--   0        0        0      288 2024-05-29 05:58:44.309677 aily_code_sdk_core-0.1.0b5/src/aily_code_sdk_core/message/components/chart.py
--rw-r--r--   0        0        0      362 2024-05-29 05:58:44.309822 aily_code_sdk_core-0.1.0b5/src/aily_code_sdk_core/message/components/code.py
--rw-r--r--   0        0        0      266 2024-05-29 05:58:44.309973 aily_code_sdk_core-0.1.0b5/src/aily_code_sdk_core/message/components/col.py
--rw-r--r--   0        0        0      441 2024-05-29 05:58:44.310106 aily_code_sdk_core-0.1.0b5/src/aily_code_sdk_core/message/components/color_text.py
--rw-r--r--   0        0        0      934 2024-05-29 05:58:44.310283 aily_code_sdk_core-0.1.0b5/src/aily_code_sdk_core/message/components/data_record.py
--rw-r--r--   0        0        0      399 2024-05-29 05:58:44.310433 aily_code_sdk_core-0.1.0b5/src/aily_code_sdk_core/message/components/highlight.py
--rw-r--r--   0        0        0      337 2024-05-29 05:58:44.310584 aily_code_sdk_core-0.1.0b5/src/aily_code_sdk_core/message/components/image.py
--rw-r--r--   0        0        0      354 2024-05-29 05:58:44.310776 aily_code_sdk_core-0.1.0b5/src/aily_code_sdk_core/message/components/item_list.py
--rw-r--r--   0        0        0      559 2024-05-29 05:58:44.310921 aily_code_sdk_core-0.1.0b5/src/aily_code_sdk_core/message/components/link.py
--rw-r--r--   0        0        0      365 2024-05-29 05:58:44.311078 aily_code_sdk_core-0.1.0b5/src/aily_code_sdk_core/message/components/mention.py
--rw-r--r--   0        0        0      389 2024-05-29 05:58:44.311215 aily_code_sdk_core-0.1.0b5/src/aily_code_sdk_core/message/components/note.py
--rw-r--r--   0        0        0      491 2024-05-29 05:58:44.311355 aily_code_sdk_core-0.1.0b5/src/aily_code_sdk_core/message/components/ordered_list.py
--rw-r--r--   0        0        0      327 2024-05-29 05:58:44.311541 aily_code_sdk_core-0.1.0b5/src/aily_code_sdk_core/message/components/row.py
--rw-r--r--   0        0        0     1055 2024-05-29 05:58:44.311779 aily_code_sdk_core-0.1.0b5/src/aily_code_sdk_core/message/components/table.py
--rw-r--r--   0        0        0      587 2024-05-29 05:58:44.311902 aily_code_sdk_core-0.1.0b5/src/aily_code_sdk_core/message/components/title.py
--rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 aily_code_sdk_core-0.1.0b5/PKG-INFO
+-rw-r--r--   0        0        0    10947 2024-05-29 05:58:44.305920 aily_code_sdk_core-0.1.0b6/LICENSE
+-rw-r--r--   0        0        0      446 2024-05-29 05:58:44.306203 aily_code_sdk_core-0.1.0b6/README.md
+-rw-r--r--   0        0        0      533 2024-06-03 06:40:26.747676 aily_code_sdk_core-0.1.0b6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-29 05:58:44.306688 aily_code_sdk_core-0.1.0b6/src/aily_code_sdk_core/__init__.py
+-rw-r--r--   0        0        0       71 2024-05-29 05:58:44.307011 aily_code_sdk_core-0.1.0b6/src/aily_code_sdk_core/action/__init__.py
+-rw-r--r--   0        0        0     2122 2024-06-03 06:39:33.318479 aily_code_sdk_core-0.1.0b6/src/aily_code_sdk_core/action/call_action.py
+-rw-r--r--   0        0        0     1394 2024-06-03 06:35:46.556849 aily_code_sdk_core-0.1.0b6/src/aily_code_sdk_core/common/context.py
+-rw-r--r--   0        0        0      597 2024-06-03 06:35:46.572207 aily_code_sdk_core-0.1.0b6/src/aily_code_sdk_core/common/util.py
+-rw-r--r--   0        0        0       74 2024-05-29 05:58:44.308002 aily_code_sdk_core-0.1.0b6/src/aily_code_sdk_core/credential/__init__.py
+-rw-r--r--   0        0        0     1593 2024-05-29 05:58:44.308159 aily_code_sdk_core-0.1.0b6/src/aily_code_sdk_core/credential/credential.py
+-rw-r--r--   0        0        0       74 2024-05-29 05:58:44.308382 aily_code_sdk_core-0.1.0b6/src/aily_code_sdk_core/env/__init__.py
+-rw-r--r--   0        0        0      437 2024-05-29 06:18:31.530058 aily_code_sdk_core-0.1.0b6/src/aily_code_sdk_core/env/get_env_info.py
+-rw-r--r--   0        0        0      752 2024-05-29 05:58:44.308918 aily_code_sdk_core-0.1.0b6/src/aily_code_sdk_core/message/builder.py
+-rw-r--r--   0        0        0      682 2024-05-29 05:58:44.309181 aily_code_sdk_core-0.1.0b6/src/aily_code_sdk_core/message/components/__init__.py
+-rw-r--r--   0        0        0     1840 2024-05-29 05:58:44.309338 aily_code_sdk_core-0.1.0b6/src/aily_code_sdk_core/message/components/base_component.py
+-rw-r--r--   0        0        0     1556 2024-05-29 05:58:44.309521 aily_code_sdk_core-0.1.0b6/src/aily_code_sdk_core/message/components/button.py
+-rw-r--r--   0        0        0      288 2024-05-29 05:58:44.309677 aily_code_sdk_core-0.1.0b6/src/aily_code_sdk_core/message/components/chart.py
+-rw-r--r--   0        0        0      362 2024-05-29 05:58:44.309822 aily_code_sdk_core-0.1.0b6/src/aily_code_sdk_core/message/components/code.py
+-rw-r--r--   0        0        0      266 2024-05-29 05:58:44.309973 aily_code_sdk_core-0.1.0b6/src/aily_code_sdk_core/message/components/col.py
+-rw-r--r--   0        0        0      441 2024-05-29 05:58:44.310106 aily_code_sdk_core-0.1.0b6/src/aily_code_sdk_core/message/components/color_text.py
+-rw-r--r--   0        0        0      934 2024-05-29 05:58:44.310283 aily_code_sdk_core-0.1.0b6/src/aily_code_sdk_core/message/components/data_record.py
+-rw-r--r--   0        0        0      399 2024-05-29 05:58:44.310433 aily_code_sdk_core-0.1.0b6/src/aily_code_sdk_core/message/components/highlight.py
+-rw-r--r--   0        0        0      337 2024-05-29 05:58:44.310584 aily_code_sdk_core-0.1.0b6/src/aily_code_sdk_core/message/components/image.py
+-rw-r--r--   0        0        0      354 2024-05-29 05:58:44.310776 aily_code_sdk_core-0.1.0b6/src/aily_code_sdk_core/message/components/item_list.py
+-rw-r--r--   0        0        0      559 2024-05-29 05:58:44.310921 aily_code_sdk_core-0.1.0b6/src/aily_code_sdk_core/message/components/link.py
+-rw-r--r--   0        0        0      365 2024-05-29 05:58:44.311078 aily_code_sdk_core-0.1.0b6/src/aily_code_sdk_core/message/components/mention.py
+-rw-r--r--   0        0        0      389 2024-05-29 05:58:44.311215 aily_code_sdk_core-0.1.0b6/src/aily_code_sdk_core/message/components/note.py
+-rw-r--r--   0        0        0      491 2024-05-29 05:58:44.311355 aily_code_sdk_core-0.1.0b6/src/aily_code_sdk_core/message/components/ordered_list.py
+-rw-r--r--   0        0        0      327 2024-05-29 05:58:44.311541 aily_code_sdk_core-0.1.0b6/src/aily_code_sdk_core/message/components/row.py
+-rw-r--r--   0        0        0     1055 2024-05-29 05:58:44.311779 aily_code_sdk_core-0.1.0b6/src/aily_code_sdk_core/message/components/table.py
+-rw-r--r--   0        0        0      587 2024-05-29 05:58:44.311902 aily_code_sdk_core-0.1.0b6/src/aily_code_sdk_core/message/components/title.py
+-rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 aily_code_sdk_core-0.1.0b6/PKG-INFO
```

### Comparing `aily_code_sdk_core-0.1.0b5/LICENSE` & `aily_code_sdk_core-0.1.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `aily_code_sdk_core-0.1.0b5/pyproject.toml` & `aily_code_sdk_core-0.1.0b6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "aily-code-sdk-core"
 description = "Aily Code SDK Core"
-version = "0.1.0-beta.5"
+version = "0.1.0-beta.6"
 authors = [
     "lijiuyang.5137 <lijiuyang.5137@bytedance.com>",
     "zhaolizi.milo <zhaolizi.milo@bytedance.com>"
 ]
 readme = "README.md"
 packages = [{ include = "aily_code_sdk_core", from = "src" }]
```

### Comparing `aily_code_sdk_core-0.1.0b5/src/aily_code_sdk_core/action/call_action.py` & `aily_code_sdk_core-0.1.0b6/src/aily_code_sdk_core/action/call_action.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any
 from urllib.parse import urljoin
 import json
 from ..common.context import get_domain, get_by_headers
+
 from ..credential import AppCredential
 from ..common.util import get_http_session
 
 defaultOptions = {
     "timeout": 60 * 1000 * 5,
     "retry_times": 0,
 }
@@ -23,16 +24,20 @@
     token = credential.get_token()
     domain = get_domain()
 
     if not token:
         raise Exception('get token failed')
 
     http = get_http_session(token)
+    current_skill_id = get_by_headers('x-aily-skill-instance-id')
+    if current_skill_id is None and action_api_name == 'action:brn:cn:spring:all:all:connector_action_runtime' \
+                                                       ':/spring_sdk_send_message':
+        raise Exception('发送消息接口暂不支持直接调试, 需要点击技能调试.')
 
-    action_data.update({'skillInstanceID': get_by_headers('x-aily-skill-instance-id')})
+    action_data.update({'skillInstanceID': current_skill_id})
     req = {
         'customerBizId': 'spring',
         'data': {
             'actionApiName': action_api_name,
             'actionData': json.dumps(action_data),
             'options': json.dumps({
                 **defaultOptions,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aily_code_sdk_core-0.1.0b5/src/aily_code_sdk_core/common/context.py` & `aily_code_sdk_core-0.1.0b6/src/aily_code_sdk_core/common/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,8 +61,8 @@
     return get_from_credential("domain")
 
 
 def get_by_headers(key):
     headers = get_ctx_key("sysHeaders")
     if headers is None:
         return ""
-    return headers[key]
+    return headers.get(key)
```

### Comparing `aily_code_sdk_core-0.1.0b5/src/aily_code_sdk_core/common/util.py` & `aily_code_sdk_core-0.1.0b6/src/aily_code_sdk_core/common/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,17 +4,21 @@
 
 
 def get_http_session(token: str = '') -> requests.Session:
     s = requests.Session()
     s.headers.update({
         "Authorization": token,
         "biz_id": "spring",
-        "x-tt-env": get_by_headers("x-tt-env"),
         "Content-Type": "application/json",
         "Rpc-Persist-AUTH-TYPE": "user",
     })
+
+    tt_env = get_by_headers("x-tt-env")
+    if tt_env:
+        s.headers.update({'x-tt-env': tt_env})
+
     user = get_by_headers("x-kunlun-initiator")
     if user:
         user_id = json.loads(user)['_id']
         s.headers.update({'User': str(user_id)})
 
     return s
```

### Comparing `aily_code_sdk_core-0.1.0b5/src/aily_code_sdk_core/credential/credential.py` & `aily_code_sdk_core-0.1.0b6/src/aily_code_sdk_core/credential/credential.py`

 * *Files identical despite different names*

### Comparing `aily_code_sdk_core-0.1.0b5/src/aily_code_sdk_core/message/builder.py` & `aily_code_sdk_core-0.1.0b6/src/aily_code_sdk_core/message/builder.py`

 * *Files identical despite different names*

### Comparing `aily_code_sdk_core-0.1.0b5/src/aily_code_sdk_core/message/components/__init__.py` & `aily_code_sdk_core-0.1.0b6/src/aily_code_sdk_core/message/components/__init__.py`

 * *Files identical despite different names*

### Comparing `aily_code_sdk_core-0.1.0b5/src/aily_code_sdk_core/message/components/base_component.py` & `aily_code_sdk_core-0.1.0b6/src/aily_code_sdk_core/message/components/base_component.py`

 * *Files identical despite different names*

### Comparing `aily_code_sdk_core-0.1.0b5/src/aily_code_sdk_core/message/components/button.py` & `aily_code_sdk_core-0.1.0b6/src/aily_code_sdk_core/message/components/button.py`

 * *Files identical despite different names*

### Comparing `aily_code_sdk_core-0.1.0b5/src/aily_code_sdk_core/message/components/data_record.py` & `aily_code_sdk_core-0.1.0b6/src/aily_code_sdk_core/message/components/data_record.py`

 * *Files identical despite different names*

### Comparing `aily_code_sdk_core-0.1.0b5/src/aily_code_sdk_core/message/components/link.py` & `aily_code_sdk_core-0.1.0b6/src/aily_code_sdk_core/message/components/link.py`

 * *Files identical despite different names*

### Comparing `aily_code_sdk_core-0.1.0b5/src/aily_code_sdk_core/message/components/table.py` & `aily_code_sdk_core-0.1.0b6/src/aily_code_sdk_core/message/components/table.py`

 * *Files identical despite different names*

### Comparing `aily_code_sdk_core-0.1.0b5/src/aily_code_sdk_core/message/components/title.py` & `aily_code_sdk_core-0.1.0b6/src/aily_code_sdk_core/message/components/title.py`

 * *Files identical despite different names*

### Comparing `aily_code_sdk_core-0.1.0b5/PKG-INFO` & `aily_code_sdk_core-0.1.0b6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aily-code-sdk-core
-Version: 0.1.0b5
+Version: 0.1.0b6
 Summary: Aily Code SDK Core
 Author: lijiuyang.5137
 Author-email: lijiuyang.5137@bytedance.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

