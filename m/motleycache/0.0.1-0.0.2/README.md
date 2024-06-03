# Comparing `tmp/motleycache-0.0.1.tar.gz` & `tmp/motleycache-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motleycache-0.0.1.tar", max compression
+gzip compressed data, was "motleycache-0.0.2.tar", max compression
```

## Comparing `motleycache-0.0.1.tar` & `motleycache-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      251 2024-05-24 12:32:45.695099 motleycache-0.0.1/README.md
--rw-r--r--   0        0        0      221 2024-05-24 12:32:45.695294 motleycache-0.0.1/motleycache/__init__.py
--rw-r--r--   0        0        0     1592 2024-05-24 12:32:45.695417 motleycache-0.0.1/motleycache/caching.py
--rw-r--r--   0        0        0    14424 2024-05-24 12:32:45.695663 motleycache-0.0.1/motleycache/http_cache.py
--rw-r--r--   0        0        0     1987 2024-05-24 12:32:45.695800 motleycache-0.0.1/motleycache/utils.py
--rw-r--r--   0        0        0      541 2024-05-24 12:33:15.665354 motleycache-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1053 1970-01-01 00:00:00.000000 motleycache-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-06-03 13:08:04.583883 motleycache-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3297 2024-06-03 13:08:04.584465 motleycache-0.0.2/README.md
+-rw-r--r--   0        0        0      221 2024-05-24 12:32:45.695294 motleycache-0.0.2/motleycache/__init__.py
+-rw-r--r--   0        0        0     1592 2024-05-24 12:32:45.695417 motleycache-0.0.2/motleycache/caching.py
+-rw-r--r--   0        0        0    14637 2024-06-03 13:08:04.585173 motleycache-0.0.2/motleycache/http_cache.py
+-rw-r--r--   0        0        0     1987 2024-05-24 12:32:45.695800 motleycache-0.0.2/motleycache/utils.py
+-rw-r--r--   0        0        0      541 2024-06-03 13:08:36.966963 motleycache-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4099 1970-01-01 00:00:00.000000 motleycache-0.0.2/PKG-INFO
```

### Comparing `motleycache-0.0.1/motleycache/caching.py` & `motleycache-0.0.2/motleycache/caching.py`

 * *Files identical despite different names*

### Comparing `motleycache-0.0.1/motleycache/http_cache.py` & `motleycache-0.0.2/motleycache/http_cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,20 +19,22 @@
 )
 from curl_cffi.requests import AsyncSession as CurlCFFI__AsyncSession
 from curl_cffi.requests import Headers as CurlCFFI__Headers
 
 
 try:
     from lunary import track_event, run_ctx, event_queue_ctx
+    from lunary import queue as lunary_main_queue
 
     do_update_lunary_event = True
 except ImportError:
     track_event = None
     run_ctx = None
     event_queue_ctx = None
+    lunary_main_queue = None
     do_update_lunary_event = False
 
 
 from .utils import recursive_hash, shorten_filename, FakeRLock
 
 
 logger = logging.getLogger(__name__)
@@ -238,21 +240,27 @@
         run_id: str, app_id: str, run_type: str = "llm", is_cache: bool = True
     ) -> None:
         """Updating lunary event"""
 
         if not do_update_lunary_event:
             return
 
+        try:
+            callback_queue = event_queue_ctx.get()
+        except LookupError:
+            callback_queue = lunary_main_queue
+
         event_params = {
             "run_type": run_type,
             "event_name": "update",
             "run_id": run_id,
-            "callback_queue": event_queue_ctx.get(),
+            "callback_queue": callback_queue,
             "app_id": app_id,
         }
+
         if is_cache:
             event_params["metadata"] = {"cache": True}
 
         try:
             track_event(**event_params)
         except Exception as exc:
             msg = "[Lunary] An error occurred while updating lunary event {}: {}\n{}".format(
```

### Comparing `motleycache-0.0.1/motleycache/utils.py` & `motleycache-0.0.2/motleycache/utils.py`

 * *Files identical despite different names*

### Comparing `motleycache-0.0.1/pyproject.toml` & `motleycache-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motleycache"
-version = "0.0.1"
+version = "0.0.2"
 description = "Package for caching http requests"
 authors = ["MotleyCrew <github@motleycrew.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pytest = "^8.0.2"
```

