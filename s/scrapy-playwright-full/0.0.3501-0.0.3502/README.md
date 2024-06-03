# Comparing `tmp/scrapy_playwright_full-0.0.3501.tar.gz` & `tmp/scrapy_playwright_full-0.0.3502.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapy_playwright_full-0.0.3501.tar", last modified: Sun Jun  2 17:52:19 2024, max compression
+gzip compressed data, was "scrapy_playwright_full-0.0.3502.tar", last modified: Mon Jun  3 04:05:32 2024, max compression
```

## Comparing `scrapy_playwright_full-0.0.3501.tar` & `scrapy_playwright_full-0.0.3502.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:52:19.827414 scrapy_playwright_full-0.0.3501/
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-06-02 17:52:12.000000 scrapy_playwright_full-0.0.3501/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    35611 2024-06-02 17:52:19.827414 scrapy_playwright_full-0.0.3501/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    34512 2024-06-02 17:52:12.000000 scrapy_playwright_full-0.0.3501/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-06-02 17:52:12.000000 scrapy_playwright_full-0.0.3501/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:52:19.827414 scrapy_playwright_full-0.0.3501/scrapy_playwright/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-02 17:52:12.000000 scrapy_playwright_full-0.0.3501/scrapy_playwright/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-06-02 17:52:12.000000 scrapy_playwright_full-0.0.3501/scrapy_playwright/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    33020 2024-06-02 17:52:12.000000 scrapy_playwright_full-0.0.3501/scrapy_playwright/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-06-02 17:52:12.000000 scrapy_playwright_full-0.0.3501/scrapy_playwright/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-06-02 17:52:12.000000 scrapy_playwright_full-0.0.3501/scrapy_playwright/memusage.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-06-02 17:52:12.000000 scrapy_playwright_full-0.0.3501/scrapy_playwright/page.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:52:19.827414 scrapy_playwright_full-0.0.3501/scrapy_playwright_full.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    35611 2024-06-02 17:52:19.000000 scrapy_playwright_full-0.0.3501/scrapy_playwright_full.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-06-02 17:52:19.000000 scrapy_playwright_full-0.0.3501/scrapy_playwright_full.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 17:52:19.000000 scrapy_playwright_full-0.0.3501/scrapy_playwright_full.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-06-02 17:52:19.000000 scrapy_playwright_full-0.0.3501/scrapy_playwright_full.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-02 17:52:19.000000 scrapy_playwright_full-0.0.3501/scrapy_playwright_full.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-02 17:52:19.827414 scrapy_playwright_full-0.0.3501/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-06-02 17:52:12.000000 scrapy_playwright_full-0.0.3501/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:05:32.890565 scrapy_playwright_full-0.0.3502/
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-06-03 04:05:24.000000 scrapy_playwright_full-0.0.3502/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    35611 2024-06-03 04:05:32.890565 scrapy_playwright_full-0.0.3502/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    34512 2024-06-03 04:05:24.000000 scrapy_playwright_full-0.0.3502/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-06-03 04:05:24.000000 scrapy_playwright_full-0.0.3502/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:05:32.890565 scrapy_playwright_full-0.0.3502/scrapy_playwright/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-03 04:05:24.000000 scrapy_playwright_full-0.0.3502/scrapy_playwright/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-06-03 04:05:24.000000 scrapy_playwright_full-0.0.3502/scrapy_playwright/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33157 2024-06-03 04:05:24.000000 scrapy_playwright_full-0.0.3502/scrapy_playwright/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-06-03 04:05:24.000000 scrapy_playwright_full-0.0.3502/scrapy_playwright/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-06-03 04:05:24.000000 scrapy_playwright_full-0.0.3502/scrapy_playwright/memusage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-06-03 04:05:24.000000 scrapy_playwright_full-0.0.3502/scrapy_playwright/page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:05:32.890565 scrapy_playwright_full-0.0.3502/scrapy_playwright_full.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    35611 2024-06-03 04:05:32.000000 scrapy_playwright_full-0.0.3502/scrapy_playwright_full.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-06-03 04:05:32.000000 scrapy_playwright_full-0.0.3502/scrapy_playwright_full.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 04:05:32.000000 scrapy_playwright_full-0.0.3502/scrapy_playwright_full.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-06-03 04:05:32.000000 scrapy_playwright_full-0.0.3502/scrapy_playwright_full.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-03 04:05:32.000000 scrapy_playwright_full-0.0.3502/scrapy_playwright_full.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-03 04:05:32.890565 scrapy_playwright_full-0.0.3502/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-06-03 04:05:24.000000 scrapy_playwright_full-0.0.3502/setup.py
```

### Comparing `scrapy_playwright_full-0.0.3501/LICENSE` & `scrapy_playwright_full-0.0.3502/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapy_playwright_full-0.0.3501/PKG-INFO` & `scrapy_playwright_full-0.0.3502/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-playwright-full
-Version: 0.0.3501
+Version: 0.0.3502
 Summary: Playwright integration for Scrapy
 Home-page: https://github.com/scrapy-plugins/scrapy-playwright
 Author: Eugenio Lacuesta
 Author-email: eugenio.lacuesta@gmail.com
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `scrapy_playwright_full-0.0.3501/README.md` & `scrapy_playwright_full-0.0.3502/README.md`

 * *Files identical despite different names*

### Comparing `scrapy_playwright_full-0.0.3501/scrapy_playwright/_utils.py` & `scrapy_playwright_full-0.0.3502/scrapy_playwright/_utils.py`

 * *Files identical despite different names*

### Comparing `scrapy_playwright_full-0.0.3501/scrapy_playwright/handler.py` & `scrapy_playwright_full-0.0.3502/scrapy_playwright/handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -284,15 +284,15 @@
         )
         self._set_max_concurrent_page_count()
         if self.config.navigation_timeout is not None:
             page.set_default_navigation_timeout(self.config.navigation_timeout)
 
         page.on("close", self._make_close_page_callback(context_name))
         page.on("crash", self._make_close_page_callback(context_name))
-        page.on("request", _make_request_logger(context_name, spider))
+        page.on("request", _make_request_logger(context_name, spider, getattr(request, 'playwright_id', None)))
         page.on("response", _make_response_logger(context_name, spider))
         page.on("request", self._increment_request_stats)
         page.on("response", self._increment_response_stats)
 
         return page
 
     def _get_total_page_count(self):
@@ -751,23 +751,24 @@
                     "scrapy_request_url": request.url,
                     "scrapy_request_method": request.method,
                 }
             )
             raise
 
 
-def _make_request_logger(context_name: str, spider: Spider) -> Callable:
+def _make_request_logger(context_name: str, spider: Spider, playwright_id: str) -> Callable:
     async def _log_request(request: PlaywrightRequest) -> None:
-        log_args = [context_name, request.method.upper(), request.url, request.resource_type]
+        uid = "" if playwright_id is None else f" {playwright_id}"
+        log_args = [context_name, request.method.upper(), request.url, uid, request.resource_type]
         referrer = await _get_header_value(request, "referer")
         if referrer:
             log_args.append(referrer)
-            log_msg = "[Context=%s] Request: <%s %s> (resource type: %s, referrer: %s)"
+            log_msg = "[Context=%s] Request: <%s %s%s> (resource type: %s, referrer: %s)"
         else:
-            log_msg = "[Context=%s] Request: <%s %s> (resource type: %s)"
+            log_msg = "[Context=%s] Request: <%s %s%s> (resource type: %s)"
         logger.debug(
             log_msg,
             *log_args,
             extra={
                 "spider": spider,
                 "context_name": context_name,
                 "playwright_request_url": request.url,
```

### Comparing `scrapy_playwright_full-0.0.3501/scrapy_playwright/headers.py` & `scrapy_playwright_full-0.0.3502/scrapy_playwright/headers.py`

 * *Files identical despite different names*

### Comparing `scrapy_playwright_full-0.0.3501/scrapy_playwright/memusage.py` & `scrapy_playwright_full-0.0.3502/scrapy_playwright/memusage.py`

 * *Files identical despite different names*

### Comparing `scrapy_playwright_full-0.0.3501/scrapy_playwright/page.py` & `scrapy_playwright_full-0.0.3502/scrapy_playwright/page.py`

 * *Files identical despite different names*

### Comparing `scrapy_playwright_full-0.0.3501/scrapy_playwright_full.egg-info/PKG-INFO` & `scrapy_playwright_full-0.0.3502/scrapy_playwright_full.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-playwright-full
-Version: 0.0.3501
+Version: 0.0.3502
 Summary: Playwright integration for Scrapy
 Home-page: https://github.com/scrapy-plugins/scrapy-playwright
 Author: Eugenio Lacuesta
 Author-email: eugenio.lacuesta@gmail.com
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `scrapy_playwright_full-0.0.3501/setup.py` & `scrapy_playwright_full-0.0.3502/setup.py`

 * *Files identical despite different names*

