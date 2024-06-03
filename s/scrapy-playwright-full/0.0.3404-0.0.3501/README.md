# Comparing `tmp/scrapy_playwright_full-0.0.3404.tar.gz` & `tmp/scrapy_playwright_full-0.0.3501.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapy_playwright_full-0.0.3404.tar", last modified: Wed May  8 11:23:23 2024, max compression
+gzip compressed data, was "scrapy_playwright_full-0.0.3501.tar", last modified: Sun Jun  2 17:52:19 2024, max compression
```

## Comparing `scrapy_playwright_full-0.0.3404.tar` & `scrapy_playwright_full-0.0.3501.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:23:23.482540 scrapy_playwright_full-0.0.3404/
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-08 11:23:12.000000 scrapy_playwright_full-0.0.3404/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    35611 2024-05-08 11:23:23.482540 scrapy_playwright_full-0.0.3404/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    34512 2024-05-08 11:23:12.000000 scrapy_playwright_full-0.0.3404/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-08 11:23:12.000000 scrapy_playwright_full-0.0.3404/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:23:23.482540 scrapy_playwright_full-0.0.3404/scrapy_playwright/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-08 11:23:12.000000 scrapy_playwright_full-0.0.3404/scrapy_playwright/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-08 11:23:12.000000 scrapy_playwright_full-0.0.3404/scrapy_playwright/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    33276 2024-05-08 11:23:12.000000 scrapy_playwright_full-0.0.3404/scrapy_playwright/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-08 11:23:12.000000 scrapy_playwright_full-0.0.3404/scrapy_playwright/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-08 11:23:12.000000 scrapy_playwright_full-0.0.3404/scrapy_playwright/memusage.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-08 11:23:12.000000 scrapy_playwright_full-0.0.3404/scrapy_playwright/page.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:23:23.482540 scrapy_playwright_full-0.0.3404/scrapy_playwright_full.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    35611 2024-05-08 11:23:23.000000 scrapy_playwright_full-0.0.3404/scrapy_playwright_full.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-08 11:23:23.000000 scrapy_playwright_full-0.0.3404/scrapy_playwright_full.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 11:23:23.000000 scrapy_playwright_full-0.0.3404/scrapy_playwright_full.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-08 11:23:23.000000 scrapy_playwright_full-0.0.3404/scrapy_playwright_full.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-08 11:23:23.000000 scrapy_playwright_full-0.0.3404/scrapy_playwright_full.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-08 11:23:23.486540 scrapy_playwright_full-0.0.3404/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-08 11:23:12.000000 scrapy_playwright_full-0.0.3404/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:52:19.827414 scrapy_playwright_full-0.0.3501/
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-06-02 17:52:12.000000 scrapy_playwright_full-0.0.3501/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    35611 2024-06-02 17:52:19.827414 scrapy_playwright_full-0.0.3501/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    34512 2024-06-02 17:52:12.000000 scrapy_playwright_full-0.0.3501/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-06-02 17:52:12.000000 scrapy_playwright_full-0.0.3501/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:52:19.827414 scrapy_playwright_full-0.0.3501/scrapy_playwright/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-02 17:52:12.000000 scrapy_playwright_full-0.0.3501/scrapy_playwright/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-06-02 17:52:12.000000 scrapy_playwright_full-0.0.3501/scrapy_playwright/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33020 2024-06-02 17:52:12.000000 scrapy_playwright_full-0.0.3501/scrapy_playwright/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-06-02 17:52:12.000000 scrapy_playwright_full-0.0.3501/scrapy_playwright/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-06-02 17:52:12.000000 scrapy_playwright_full-0.0.3501/scrapy_playwright/memusage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-06-02 17:52:12.000000 scrapy_playwright_full-0.0.3501/scrapy_playwright/page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:52:19.827414 scrapy_playwright_full-0.0.3501/scrapy_playwright_full.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    35611 2024-06-02 17:52:19.000000 scrapy_playwright_full-0.0.3501/scrapy_playwright_full.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-06-02 17:52:19.000000 scrapy_playwright_full-0.0.3501/scrapy_playwright_full.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 17:52:19.000000 scrapy_playwright_full-0.0.3501/scrapy_playwright_full.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-06-02 17:52:19.000000 scrapy_playwright_full-0.0.3501/scrapy_playwright_full.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-02 17:52:19.000000 scrapy_playwright_full-0.0.3501/scrapy_playwright_full.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-02 17:52:19.827414 scrapy_playwright_full-0.0.3501/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-06-02 17:52:12.000000 scrapy_playwright_full-0.0.3501/setup.py
```

### Comparing `scrapy_playwright_full-0.0.3404/LICENSE` & `scrapy_playwright_full-0.0.3501/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapy_playwright_full-0.0.3404/PKG-INFO` & `scrapy_playwright_full-0.0.3501/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-playwright-full
-Version: 0.0.3404
+Version: 0.0.3501
 Summary: Playwright integration for Scrapy
 Home-page: https://github.com/scrapy-plugins/scrapy-playwright
 Author: Eugenio Lacuesta
 Author-email: eugenio.lacuesta@gmail.com
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `scrapy_playwright_full-0.0.3404/README.md` & `scrapy_playwright_full-0.0.3501/README.md`

 * *Files identical despite different names*

### Comparing `scrapy_playwright_full-0.0.3404/scrapy_playwright/_utils.py` & `scrapy_playwright_full-0.0.3501/scrapy_playwright/_utils.py`

 * *Files identical despite different names*

### Comparing `scrapy_playwright_full-0.0.3404/scrapy_playwright/handler.py` & `scrapy_playwright_full-0.0.3501/scrapy_playwright/handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -502,27 +502,26 @@
         page_methods = request.meta.get("playwright_page_methods") or ()
         if isinstance(page_methods, dict):
             page_methods = page_methods.values()
         for pm in page_methods:
             if isinstance(pm, PageMethod):
                 try:
                     method = getattr(page, pm.method)
-                except AttributeError as ex:
+                except AttributeError:
                     logger.warning(
                         "Ignoring %r: could not find method",
                         pm,
                         extra={
                             "spider": spider,
                             "context_name": context_name,
                             "scrapy_request_url": request.url,
                             "scrapy_request_method": request.method,
-                            "exception": ex,
-                        },
-                        exc_info=True,
+                        }
                     )
+                    raise
                 else:
                     pm.result = await _maybe_await(method(*pm.args, **pm.kwargs))
                     await page.wait_for_load_state(timeout=self.config.navigation_timeout)
             else:
                 logger.warning(
                     "Ignoring %r: expected PageMethod, got %r",
                     pm,
@@ -670,17 +669,15 @@
                         extra={
                             "spider": spider,
                             "context_name": context_name,
                             "scrapy_request_url": url,
                             "scrapy_request_method": method,
                             "playwright_request_url": playwright_request.url,
                             "playwright_request_method": playwright_request.method,
-                            "exception": ex,
-                        },
-                        exc_info=True,
+                        }
                     )
                 else:
                     raise
 
         return _request_handler
 
 
@@ -702,18 +699,17 @@
                     handler,
                     event,
                     extra={
                         "spider": spider,
                         "context_name": context_name,
                         "scrapy_request_url": request.url,
                         "scrapy_request_method": request.method,
-                        "exception": ex,
-                    },
-                    exc_info=True,
+                    }
                 )
+                raise
 
 
 async def _set_redirect_meta(request: Request, response: PlaywrightResponse) -> None:
     """Update a Scrapy request with metadata about redirects."""
     redirect_times: int = 0
     redirect_urls: list = []
     redirect_reasons: list = []
@@ -750,18 +746,17 @@
                 type(ex),
                 str(ex),
                 extra={
                     "spider": spider,
                     "context_name": context_name,
                     "scrapy_request_url": request.url,
                     "scrapy_request_method": request.method,
-                    "exception": ex,
-                },
-                exc_info=True,
+                }
             )
+            raise
 
 
 def _make_request_logger(context_name: str, spider: Spider) -> Callable:
     async def _log_request(request: PlaywrightRequest) -> None:
         log_args = [context_name, request.method.upper(), request.url, request.resource_type]
         referrer = await _get_header_value(request, "referer")
         if referrer:
```

### Comparing `scrapy_playwright_full-0.0.3404/scrapy_playwright/headers.py` & `scrapy_playwright_full-0.0.3501/scrapy_playwright/headers.py`

 * *Files identical despite different names*

### Comparing `scrapy_playwright_full-0.0.3404/scrapy_playwright/memusage.py` & `scrapy_playwright_full-0.0.3501/scrapy_playwright/memusage.py`

 * *Files identical despite different names*

### Comparing `scrapy_playwright_full-0.0.3404/scrapy_playwright/page.py` & `scrapy_playwright_full-0.0.3501/scrapy_playwright/page.py`

 * *Files identical despite different names*

### Comparing `scrapy_playwright_full-0.0.3404/scrapy_playwright_full.egg-info/PKG-INFO` & `scrapy_playwright_full-0.0.3501/scrapy_playwright_full.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-playwright-full
-Version: 0.0.3404
+Version: 0.0.3501
 Summary: Playwright integration for Scrapy
 Home-page: https://github.com/scrapy-plugins/scrapy-playwright
 Author: Eugenio Lacuesta
 Author-email: eugenio.lacuesta@gmail.com
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `scrapy_playwright_full-0.0.3404/setup.py` & `scrapy_playwright_full-0.0.3501/setup.py`

 * *Files identical despite different names*

