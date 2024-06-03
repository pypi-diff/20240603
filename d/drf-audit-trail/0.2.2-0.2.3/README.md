# Comparing `tmp/drf_audit_trail-0.2.2.tar.gz` & `tmp/drf_audit_trail-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_audit_trail-0.2.2.tar", max compression
+gzip compressed data, was "drf_audit_trail-0.2.3.tar", max compression
```

## Comparing `drf_audit_trail-0.2.2.tar` & `drf_audit_trail-0.2.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1087 2024-05-22 13:39:48.438874 drf_audit_trail-0.2.2/README.md
--rw-r--r--   0        0        0        0 2024-05-08 01:49:41.058976 drf_audit_trail-0.2.2/drf_audit_trail/__init__.py
--rw-r--r--   0        0        0     1169 2024-05-28 13:08:30.611976 drf_audit_trail-0.2.2/drf_audit_trail/admin.py
--rw-r--r--   0        0        0      255 2024-05-10 20:28:23.293537 drf_audit_trail-0.2.2/drf_audit_trail/apps.py
--rw-r--r--   0        0        0        0 2024-05-08 23:42:25.366271 drf_audit_trail-0.2.2/drf_audit_trail/integrations/__init__.py
--rw-r--r--   0        0        0     1132 2024-05-30 23:45:36.060657 drf_audit_trail-0.2.2/drf_audit_trail/integrations/rest_framework_simplejwt.py
--rw-r--r--   0        0        0      106 2024-05-09 18:15:40.126054 drf_audit_trail-0.2.2/drf_audit_trail/managers/__init__.py
--rw-r--r--   0        0        0     1301 2024-05-09 18:19:21.825227 drf_audit_trail-0.2.2/drf_audit_trail/managers/request_audit_event_manager.py
--rw-r--r--   0        0        0      120 2024-05-09 01:34:50.633399 drf_audit_trail-0.2.2/drf_audit_trail/middleware/__init__.py
--rw-r--r--   0        0        0     6149 2024-05-30 23:45:14.280862 drf_audit_trail-0.2.2/drf_audit_trail/middleware/request_login_audit_event.py
--rw-r--r--   0        0        0     5511 2024-05-28 13:08:30.611976 drf_audit_trail-0.2.2/drf_audit_trail/migrations/0001_initial.py
--rw-r--r--   0        0        0      547 2024-05-28 13:08:30.611976 drf_audit_trail-0.2.2/drf_audit_trail/migrations/0002_alter_loginauditevent_request.py
--rw-r--r--   0        0        0        0 2024-05-08 01:49:41.058976 drf_audit_trail-0.2.2/drf_audit_trail/migrations/__init__.py
--rw-r--r--   0        0        0      433 2024-05-21 21:33:32.240334 drf_audit_trail-0.2.2/drf_audit_trail/mixins.py
--rw-r--r--   0        0        0      150 2024-05-09 17:52:36.716410 drf_audit_trail-0.2.2/drf_audit_trail/models/__init__.py
--rw-r--r--   0        0        0      792 2024-05-22 01:12:11.888359 drf_audit_trail-0.2.2/drf_audit_trail/models/login_audit_event.py
--rw-r--r--   0        0        0     1932 2024-05-28 13:08:30.611976 drf_audit_trail-0.2.2/drf_audit_trail/models/request_audit_event.py
--rw-r--r--   0        0        0      700 2024-05-10 00:12:08.881038 drf_audit_trail-0.2.2/drf_audit_trail/settings.py
--rw-r--r--   0        0        0       60 2024-05-08 01:49:41.058976 drf_audit_trail-0.2.2/drf_audit_trail/tests.py
--rw-r--r--   0        0        0      715 2024-05-28 13:34:00.035597 drf_audit_trail-0.2.2/drf_audit_trail/utils.py
--rw-r--r--   0        0        0      575 2024-05-30 23:58:34.885774 drf_audit_trail-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1837 1970-01-01 00:00:00.000000 drf_audit_trail-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1087 2024-05-22 13:39:48.438874 drf_audit_trail-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-08 01:49:41.058976 drf_audit_trail-0.2.3/drf_audit_trail/__init__.py
+-rw-r--r--   0        0        0     1169 2024-05-28 13:08:30.611976 drf_audit_trail-0.2.3/drf_audit_trail/admin.py
+-rw-r--r--   0        0        0      255 2024-05-10 20:28:23.293537 drf_audit_trail-0.2.3/drf_audit_trail/apps.py
+-rw-r--r--   0        0        0        0 2024-05-08 23:42:25.366271 drf_audit_trail-0.2.3/drf_audit_trail/integrations/__init__.py
+-rw-r--r--   0        0        0     1132 2024-05-30 23:45:36.060657 drf_audit_trail-0.2.3/drf_audit_trail/integrations/rest_framework_simplejwt.py
+-rw-r--r--   0        0        0      106 2024-05-09 18:15:40.126054 drf_audit_trail-0.2.3/drf_audit_trail/managers/__init__.py
+-rw-r--r--   0        0        0     1301 2024-05-09 18:19:21.825227 drf_audit_trail-0.2.3/drf_audit_trail/managers/request_audit_event_manager.py
+-rw-r--r--   0        0        0      120 2024-05-09 01:34:50.633399 drf_audit_trail-0.2.3/drf_audit_trail/middleware/__init__.py
+-rw-r--r--   0        0        0     5989 2024-06-03 13:34:26.472862 drf_audit_trail-0.2.3/drf_audit_trail/middleware/request_login_audit_event.py
+-rw-r--r--   0        0        0     5511 2024-05-28 13:08:30.611976 drf_audit_trail-0.2.3/drf_audit_trail/migrations/0001_initial.py
+-rw-r--r--   0        0        0      547 2024-05-28 13:08:30.611976 drf_audit_trail-0.2.3/drf_audit_trail/migrations/0002_alter_loginauditevent_request.py
+-rw-r--r--   0        0        0        0 2024-05-08 01:49:41.058976 drf_audit_trail-0.2.3/drf_audit_trail/migrations/__init__.py
+-rw-r--r--   0        0        0      433 2024-05-21 21:33:32.240334 drf_audit_trail-0.2.3/drf_audit_trail/mixins.py
+-rw-r--r--   0        0        0      150 2024-05-09 17:52:36.716410 drf_audit_trail-0.2.3/drf_audit_trail/models/__init__.py
+-rw-r--r--   0        0        0      792 2024-05-22 01:12:11.888359 drf_audit_trail-0.2.3/drf_audit_trail/models/login_audit_event.py
+-rw-r--r--   0        0        0     1932 2024-05-28 13:08:30.611976 drf_audit_trail-0.2.3/drf_audit_trail/models/request_audit_event.py
+-rw-r--r--   0        0        0      700 2024-05-10 00:12:08.881038 drf_audit_trail-0.2.3/drf_audit_trail/settings.py
+-rw-r--r--   0        0        0       60 2024-05-08 01:49:41.058976 drf_audit_trail-0.2.3/drf_audit_trail/tests.py
+-rw-r--r--   0        0        0      715 2024-05-28 13:34:00.035597 drf_audit_trail-0.2.3/drf_audit_trail/utils.py
+-rw-r--r--   0        0        0      575 2024-06-03 13:35:00.994877 drf_audit_trail-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1837 1970-01-01 00:00:00.000000 drf_audit_trail-0.2.3/PKG-INFO
```

### Comparing `drf_audit_trail-0.2.2/README.md` & `drf_audit_trail-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `drf_audit_trail-0.2.2/drf_audit_trail/admin.py` & `drf_audit_trail-0.2.3/drf_audit_trail/admin.py`

 * *Files identical despite different names*

### Comparing `drf_audit_trail-0.2.2/drf_audit_trail/integrations/rest_framework_simplejwt.py` & `drf_audit_trail-0.2.3/drf_audit_trail/integrations/rest_framework_simplejwt.py`

 * *Files identical despite different names*

### Comparing `drf_audit_trail-0.2.2/drf_audit_trail/managers/request_audit_event_manager.py` & `drf_audit_trail-0.2.3/drf_audit_trail/managers/request_audit_event_manager.py`

 * *Files identical despite different names*

### Comparing `drf_audit_trail-0.2.2/drf_audit_trail/middleware/request_login_audit_event.py` & `drf_audit_trail-0.2.3/drf_audit_trail/middleware/request_login_audit_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,16 @@
             "http"
         ):
             _thread_locals.url = request.path
             _thread_locals.method = request.method
             _thread_locals.META = request.META
             _thread_locals.query_params = _thread_locals.META.get("QUERY_STRING")
             _thread_locals.ip_addresses = get_ip_addresses(request)
+            _thread_locals.META["drf_request_audit_event"] = {}
+            _thread_locals.META["drf_login_audit_event"] = {}
 
             _thread_locals.request_audit_event_enabled = False
             for i in DRF_AUDIT_TRAIL_REQUEST_AUDIT_URLS:
                 if bool(re.match(i, _thread_locals.url)):
                     _thread_locals.request_audit_event_enabled = True
                     break
 
@@ -47,19 +49,14 @@
                 _thread_locals.request_audit_event_enabled = True
 
             _thread_locals.start_time = time()
             _thread_locals.META["drf_audit_event_start_time"] = (
                 _thread_locals.start_time
             )
 
-    def process_view(self, request: HttpRequest, view_func, view_args, view_kwargs):
-        if getattr(_thread_locals, "request_audit_event_enabled", False):
-            _thread_locals.META["drf_request_audit_event"] = {}
-            _thread_locals.META["drf_login_audit_event"] = {}
-
     def process_response(self, request, response):
         if getattr(_thread_locals, "request_audit_event_enabled", False):
             authenticated_user = self.__get_authenticated_user(request)
             extra_informations = self._get_extra_informations(
                 _thread_locals.META["drf_request_audit_event"]
             )
```

### Comparing `drf_audit_trail-0.2.2/drf_audit_trail/migrations/0001_initial.py` & `drf_audit_trail-0.2.3/drf_audit_trail/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `drf_audit_trail-0.2.2/drf_audit_trail/migrations/0002_alter_loginauditevent_request.py` & `drf_audit_trail-0.2.3/drf_audit_trail/migrations/0002_alter_loginauditevent_request.py`

 * *Files identical despite different names*

### Comparing `drf_audit_trail-0.2.2/drf_audit_trail/models/login_audit_event.py` & `drf_audit_trail-0.2.3/drf_audit_trail/models/login_audit_event.py`

 * *Files identical despite different names*

### Comparing `drf_audit_trail-0.2.2/drf_audit_trail/models/request_audit_event.py` & `drf_audit_trail-0.2.3/drf_audit_trail/models/request_audit_event.py`

 * *Files identical despite different names*

### Comparing `drf_audit_trail-0.2.2/drf_audit_trail/settings.py` & `drf_audit_trail-0.2.3/drf_audit_trail/settings.py`

 * *Files identical despite different names*

### Comparing `drf_audit_trail-0.2.2/drf_audit_trail/utils.py` & `drf_audit_trail-0.2.3/drf_audit_trail/utils.py`

 * *Files identical despite different names*

### Comparing `drf_audit_trail-0.2.2/pyproject.toml` & `drf_audit_trail-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drf-audit-trail"
-version = "0.2.2"
+version = "0.2.3"
 description = "A reusable django [DRF] application that handles auditing of requests and logins"
 authors = ["Talismar Fernandes Costa <talismar788.una@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/Talismar/drf-audit-trail"
 
 
 [tool.poetry.dependencies]
```

### Comparing `drf_audit_trail-0.2.2/PKG-INFO` & `drf_audit_trail-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-audit-trail
-Version: 0.2.2
+Version: 0.2.3
 Summary: A reusable django [DRF] application that handles auditing of requests and logins
 Home-page: https://github.com/Talismar/drf-audit-trail
 Author: Talismar Fernandes Costa
 Author-email: talismar788.una@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

