# Comparing `tmp/dalpha-0.5.5rc2.tar.gz` & `tmp/dalpha-0.5.5rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dalpha-0.5.5rc2.tar", max compression
+gzip compressed data, was "dalpha-0.5.5rc3.tar", max compression
```

## Comparing `dalpha-0.5.5rc2.tar` & `dalpha-0.5.5rc3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      578 2023-12-18 04:10:26.318635 dalpha-0.5.5rc2/README.md
--rw-r--r--   0        0        0     2159 2024-06-01 20:46:02.704147 dalpha-0.5.5rc2/dalpha/__init__.py
--rw-r--r--   0        0        0     8282 2024-05-16 17:41:28.081119 dalpha-0.5.5rc2/dalpha/agent.py
--rw-r--r--   0        0        0     7889 2024-05-22 02:06:09.763823 dalpha-0.5.5rc2/dalpha/backend_cli.py
--rw-r--r--   0        0        0      555 2024-05-08 06:25:10.211719 dalpha-0.5.5rc2/dalpha/cobra_cls.py
--rw-r--r--   0        0        0      573 2024-02-28 08:10:55.063883 dalpha-0.5.5rc2/dalpha/context.py
--rw-r--r--   0        0        0     2924 2024-06-01 22:17:55.260450 dalpha-0.5.5rc2/dalpha/data_update_cls.py
--rw-r--r--   0        0        0     4688 2024-06-01 20:46:02.704147 dalpha-0.5.5rc2/dalpha/data_update_consumer.py
--rw-r--r--   0        0        0     1798 2024-06-01 12:03:50.256168 dalpha-0.5.5rc2/dalpha/dto.py
--rw-r--r--   0        0        0      616 2024-05-16 07:16:07.980796 dalpha-0.5.5rc2/dalpha/exception.py
--rw-r--r--   0        0        0     6000 2024-05-18 12:36:17.240345 dalpha-0.5.5rc2/dalpha/inference_cls.py
--rw-r--r--   0        0        0      233 2024-03-25 02:37:47.094337 dalpha-0.5.5rc2/dalpha/kafka_cli.py
--rw-r--r--   0        0        0     1861 2024-03-11 02:52:37.986799 dalpha-0.5.5rc2/dalpha/logging/__init__.py
--rw-r--r--   0        0        0      229 2024-02-28 08:10:55.063883 dalpha-0.5.5rc2/dalpha/logging/events.py
--rw-r--r--   0        0        0     1116 2024-02-28 08:10:55.063883 dalpha-0.5.5rc2/dalpha/logging/log_formatter.py
--rw-r--r--   0        0        0     1817 2024-02-28 08:10:55.063883 dalpha-0.5.5rc2/dalpha/logging/utils.py
--rw-r--r--   0        0        0     6689 2024-05-22 02:06:09.767823 dalpha-0.5.5rc2/dalpha/message_consumer.py
--rw-r--r--   0        0        0     1703 2024-05-10 10:54:52.512416 dalpha-0.5.5rc2/dalpha/openai_cls.py
--rw-r--r--   0        0        0     6079 2024-05-02 07:23:00.795089 dalpha-0.5.5rc2/dalpha/redis_cli.py
--rw-r--r--   0        0        0     1886 2024-05-02 07:23:00.795089 dalpha-0.5.5rc2/dalpha/redis_cls.py
--rw-r--r--   0        0        0      776 2024-05-10 10:54:52.512416 dalpha-0.5.5rc2/dalpha/request.py
--rw-r--r--   0        0        0     2673 2024-05-23 10:37:42.216823 dalpha-0.5.5rc2/dalpha/s3.py
--rw-r--r--   0        0        0      497 2024-02-28 08:10:55.063883 dalpha-0.5.5rc2/dalpha/signal_handler.py
--rw-r--r--   0        0        0     4607 2024-06-01 20:46:02.704147 dalpha-0.5.5rc2/dalpha/update_agent.py
--rw-r--r--   0        0        0      952 2024-06-01 22:17:55.260450 dalpha-0.5.5rc2/pyproject.toml
--rw-r--r--   0        0        0     1362 1970-01-01 00:00:00.000000 dalpha-0.5.5rc2/PKG-INFO
+-rw-r--r--   0        0        0      578 2023-12-18 04:10:26.318635 dalpha-0.5.5rc3/README.md
+-rw-r--r--   0        0        0     2159 2024-06-01 20:46:02.704147 dalpha-0.5.5rc3/dalpha/__init__.py
+-rw-r--r--   0        0        0     8282 2024-05-16 17:41:28.081119 dalpha-0.5.5rc3/dalpha/agent.py
+-rw-r--r--   0        0        0     8187 2024-06-03 08:18:07.487077 dalpha-0.5.5rc3/dalpha/backend_cli.py
+-rw-r--r--   0        0        0      555 2024-05-08 06:25:10.211719 dalpha-0.5.5rc3/dalpha/cobra_cls.py
+-rw-r--r--   0        0        0      573 2024-02-28 08:10:55.063883 dalpha-0.5.5rc3/dalpha/context.py
+-rw-r--r--   0        0        0     2924 2024-06-01 22:17:55.260450 dalpha-0.5.5rc3/dalpha/data_update_cls.py
+-rw-r--r--   0        0        0     4688 2024-06-01 20:46:02.704147 dalpha-0.5.5rc3/dalpha/data_update_consumer.py
+-rw-r--r--   0        0        0     1798 2024-06-01 12:03:50.256168 dalpha-0.5.5rc3/dalpha/dto.py
+-rw-r--r--   0        0        0      616 2024-05-16 07:16:07.980796 dalpha-0.5.5rc3/dalpha/exception.py
+-rw-r--r--   0        0        0     6000 2024-05-18 12:36:17.240345 dalpha-0.5.5rc3/dalpha/inference_cls.py
+-rw-r--r--   0        0        0      233 2024-03-25 02:37:47.094337 dalpha-0.5.5rc3/dalpha/kafka_cli.py
+-rw-r--r--   0        0        0     1861 2024-03-11 02:52:37.986799 dalpha-0.5.5rc3/dalpha/logging/__init__.py
+-rw-r--r--   0        0        0      229 2024-02-28 08:10:55.063883 dalpha-0.5.5rc3/dalpha/logging/events.py
+-rw-r--r--   0        0        0     1116 2024-02-28 08:10:55.063883 dalpha-0.5.5rc3/dalpha/logging/log_formatter.py
+-rw-r--r--   0        0        0     1817 2024-02-28 08:10:55.063883 dalpha-0.5.5rc3/dalpha/logging/utils.py
+-rw-r--r--   0        0        0     6689 2024-05-22 02:06:09.767823 dalpha-0.5.5rc3/dalpha/message_consumer.py
+-rw-r--r--   0        0        0     1703 2024-05-10 10:54:52.512416 dalpha-0.5.5rc3/dalpha/openai_cls.py
+-rw-r--r--   0        0        0     6079 2024-05-02 07:23:00.795089 dalpha-0.5.5rc3/dalpha/redis_cli.py
+-rw-r--r--   0        0        0     1886 2024-05-02 07:23:00.795089 dalpha-0.5.5rc3/dalpha/redis_cls.py
+-rw-r--r--   0        0        0      776 2024-05-10 10:54:52.512416 dalpha-0.5.5rc3/dalpha/request.py
+-rw-r--r--   0        0        0     2673 2024-05-23 10:37:42.216823 dalpha-0.5.5rc3/dalpha/s3.py
+-rw-r--r--   0        0        0      497 2024-02-28 08:10:55.063883 dalpha-0.5.5rc3/dalpha/signal_handler.py
+-rw-r--r--   0        0        0     4671 2024-06-03 08:18:07.487077 dalpha-0.5.5rc3/dalpha/update_agent.py
+-rw-r--r--   0        0        0      952 2024-06-03 08:18:07.487077 dalpha-0.5.5rc3/pyproject.toml
+-rw-r--r--   0        0        0     1362 1970-01-01 00:00:00.000000 dalpha-0.5.5rc3/PKG-INFO
```

### Comparing `dalpha-0.5.5rc2/README.md` & `dalpha-0.5.5rc3/README.md`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5rc2/dalpha/__init__.py` & `dalpha-0.5.5rc3/dalpha/__init__.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5rc2/dalpha/agent.py` & `dalpha-0.5.5rc3/dalpha/agent.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5rc2/dalpha/backend_cli.py` & `dalpha-0.5.5rc3/dalpha/backend_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,22 +59,27 @@
                 message = f'error from internal_call(get) / response status_code {response.status_code}: {response.text}'
                 sentry_sdk.capture_message(message)
                 raise Exception(message)
     message = f'internal call result is not returned in timeout({time_out}) seconds.'
     sentry_sdk.capture_message(message)
     raise Exception(message)
 
-def slack_alert(self, channel_name, text):
-    url = os.path.join(self.base_url, f'slack/message')
+def slack_alert(self, channel_name, text, token, dev_server = bool(os.environ.get('DEV_SERVER', 'True') == 'True')):
+    base_url = os.environ.get('DEV_BASE_URL', 'https://api.exp.dalpha.so') if dev_server else os.environ.get('BASE_URL', 'https://api.dalpha.so')
+    url = os.path.join(base_url, f'slack/message')
+    header = {
+        'token': token,
+        'Content-Type': 'application/json'
+    }
     payload = {
         "channelName": channel_name,
         "message": text
     }
     with RetrySession() as s:
-        response = s.post(url, headers=self.header, data=json.dumps(payload))
+        response = s.post(url, headers=header, data=json.dumps(payload))
     if response.status_code == 200:
         return response.json()
     elif response.status_code < 500: # 400대 에러일 때는 확실히 유효하지 않은 메세지로 판단
         logger.warning(f'error from slack_alert / response status_code {response.status_code}: {response.text}')
         return None
     else: # 5회 재시도해도 500대 에러일 때는 유효한지 알 수 없으므로 유효하지 않은 메세지로 판단
         logger.error(f'error from slack_alert / response status_code {response.status_code}: {response.text}')
```

### Comparing `dalpha-0.5.5rc2/dalpha/cobra_cls.py` & `dalpha-0.5.5rc3/dalpha/cobra_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5rc2/dalpha/context.py` & `dalpha-0.5.5rc3/dalpha/context.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5rc2/dalpha/data_update_cls.py` & `dalpha-0.5.5rc3/dalpha/data_update_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5rc2/dalpha/data_update_consumer.py` & `dalpha-0.5.5rc3/dalpha/data_update_consumer.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5rc2/dalpha/dto.py` & `dalpha-0.5.5rc3/dalpha/dto.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5rc2/dalpha/exception.py` & `dalpha-0.5.5rc3/dalpha/exception.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5rc2/dalpha/inference_cls.py` & `dalpha-0.5.5rc3/dalpha/inference_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5rc2/dalpha/logging/__init__.py` & `dalpha-0.5.5rc3/dalpha/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5rc2/dalpha/logging/log_formatter.py` & `dalpha-0.5.5rc3/dalpha/logging/log_formatter.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5rc2/dalpha/logging/utils.py` & `dalpha-0.5.5rc3/dalpha/logging/utils.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5rc2/dalpha/message_consumer.py` & `dalpha-0.5.5rc3/dalpha/message_consumer.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5rc2/dalpha/openai_cls.py` & `dalpha-0.5.5rc3/dalpha/openai_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5rc2/dalpha/redis_cli.py` & `dalpha-0.5.5rc3/dalpha/redis_cli.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5rc2/dalpha/redis_cls.py` & `dalpha-0.5.5rc3/dalpha/redis_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5rc2/dalpha/request.py` & `dalpha-0.5.5rc3/dalpha/request.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5rc2/dalpha/s3.py` & `dalpha-0.5.5rc3/dalpha/s3.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5rc2/dalpha/update_agent.py` & `dalpha-0.5.5rc3/dalpha/update_agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,15 +95,16 @@
             message = f"update completed - {output}",
             event = Event.VALIDATE,
             data = output
         )
         if alert:
             slack_alert(
                 '#data-update-alarm',
-                f"update_complete payload for topic: {self.kafka_topic} - result: {output}"
+                f"update_complete payload for target: {self.target} - result: {output}",
+                token = self.token
             )
         
 
     def validate_error(self, output={}, alert = False):
         '''
         data update 파이프라인에서의 validate_error이라고 보면 된다.
         update 도중 에러가 발생했을 때 이 함수를 통해서 kafka의 offset을 commit한다.
@@ -114,12 +115,13 @@
             message = f"update error - {output}",
             event = Event.VALIDATE_ERROR,
             data = output
         )
         if alert:
             slack_alert(
                 '#data-update-alarm',
-                f"update_error payload for topic: {self.kafka_topic} - result: {output}"
+                f"update_error payload for target: {self.target} - result: {output}",
+                token = self.token
             )
 
     def close(self):
         self.data_update_consumer.close()
```

### Comparing `dalpha-0.5.5rc2/pyproject.toml` & `dalpha-0.5.5rc3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dalpha"
-version = "0.5.5rc2"
+version = "0.5.5rc3"
 description = ""
 authors = ["devops <devops@dalpha.so>"]
 readme = "README.md"
 packages = [{include = "dalpha"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -17,15 +17,15 @@
 pydantic = "^2.7.1"
 
 [tool.poetry.group.dev.dependencies]
 twine = "^4.0.2"
 
 [project]
 name = "dalpha"
-version = "0.5.5rc2"
+version = "0.5.5rc3"
 authors = [
   { name="Beomseok", email="beomseok.kim@dalpha.so" },
   { name="Gideok", email="gideok.kim@dalpha.so" },
 ]
 description = "Dalpha internal sdk"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `dalpha-0.5.5rc2/PKG-INFO` & `dalpha-0.5.5rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalpha
-Version: 0.5.5rc2
+Version: 0.5.5rc3
 Summary: 
 Author: devops
 Author-email: devops@dalpha.so
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

