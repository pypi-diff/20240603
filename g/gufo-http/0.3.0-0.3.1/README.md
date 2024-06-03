# Comparing `tmp/gufo_http-0.3.0.tar.gz` & `tmp/gufo_http-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gufo_http-0.3.0.tar", last modified: Sun Mar 24 10:30:33 2024, max compression
+gzip compressed data, was "gufo_http-0.3.1.tar", last modified: Mon Jun  3 07:43:14 2024, max compression
```

## Comparing `gufo_http-0.3.0.tar` & `gufo_http-0.3.1.tar`

### file list

```diff
@@ -1,30 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 10:30:33.865465 gufo_http-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-03-24 10:30:25.000000 gufo_http-0.3.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-03-24 10:30:33.861465 gufo_http-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-03-24 10:30:25.000000 gufo_http-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-03-24 10:30:25.000000 gufo_http-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 10:30:33.865465 gufo_http-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 10:30:33.857465 gufo_http-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 10:30:33.857465 gufo_http-0.3.0/src/gufo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 10:30:33.861465 gufo_http-0.3.0/src/gufo/http/
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-03-24 10:30:25.000000 gufo_http-0.3.0/src/gufo/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-03-24 10:30:25.000000 gufo_http-0.3.0/src/gufo/http/_fast.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-03-24 10:30:25.000000 gufo_http-0.3.0/src/gufo/http/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12881 2024-03-24 10:30:25.000000 gufo_http-0.3.0/src/gufo/http/httpd.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      169 2024-03-24 10:30:25.000000 gufo_http-0.3.0/src/gufo/http/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9079 2024-03-24 10:30:25.000000 gufo_http-0.3.0/src/gufo/http/sync_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-03-24 10:30:25.000000 gufo_http-0.3.0/src/gufo/http/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 10:30:33.861465 gufo_http-0.3.0/src/gufo_http.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-03-24 10:30:33.000000 gufo_http-0.3.0/src/gufo_http.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-03-24 10:30:33.000000 gufo_http-0.3.0/src/gufo_http.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 10:30:33.000000 gufo_http-0.3.0/src/gufo_http.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 10:30:33.000000 gufo_http-0.3.0/src/gufo_http.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-24 10:30:33.000000 gufo_http-0.3.0/src/gufo_http.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 10:30:33.861465 gufo_http-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    16919 2024-03-24 10:30:25.000000 gufo_http-0.3.0/tests/test_async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-03-24 10:30:25.000000 gufo_http-0.3.0/tests/test_ci.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-03-24 10:30:25.000000 gufo_http-0.3.0/tests/test_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-03-24 10:30:25.000000 gufo_http-0.3.0/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (127)    13012 2024-03-24 10:30:25.000000 gufo_http-0.3.0/tests/test_sync_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-03-24 10:30:25.000000 gufo_http-0.3.0/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-03-24 10:30:25.000000 gufo_http-0.3.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:43:14.019708 gufo_http-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-06-03 07:43:00.000000 gufo_http-0.3.1/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-06-03 07:43:00.000000 gufo_http-0.3.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-06-03 07:43:00.000000 gufo_http-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-06-03 07:43:14.019708 gufo_http-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-06-03 07:43:00.000000 gufo_http-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-06-03 07:43:00.000000 gufo_http-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 07:43:14.019708 gufo_http-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:43:14.015708 gufo_http-0.3.1/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-06-03 07:43:00.000000 gufo_http-0.3.1/src/async_client.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-06-03 07:43:00.000000 gufo_http-0.3.1/src/auth.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-06-03 07:43:00.000000 gufo_http-0.3.1/src/error.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:43:14.015708 gufo_http-0.3.1/src/gufo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:43:14.019708 gufo_http-0.3.1/src/gufo/http/
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-06-03 07:43:00.000000 gufo_http-0.3.1/src/gufo/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-06-03 07:43:00.000000 gufo_http-0.3.1/src/gufo/http/_fast.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-06-03 07:43:00.000000 gufo_http-0.3.1/src/gufo/http/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12881 2024-06-03 07:43:00.000000 gufo_http-0.3.1/src/gufo/http/httpd.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      169 2024-06-03 07:43:00.000000 gufo_http-0.3.1/src/gufo/http/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-06-03 07:43:00.000000 gufo_http-0.3.1/src/gufo/http/sync_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-06-03 07:43:00.000000 gufo_http-0.3.1/src/gufo/http/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:43:14.019708 gufo_http-0.3.1/src/gufo_http.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-06-03 07:43:14.000000 gufo_http-0.3.1/src/gufo_http.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-06-03 07:43:14.000000 gufo_http-0.3.1/src/gufo_http.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 07:43:14.000000 gufo_http-0.3.1/src/gufo_http.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 07:43:13.000000 gufo_http-0.3.1/src/gufo_http.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-06-03 07:43:14.000000 gufo_http-0.3.1/src/gufo_http.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-06-03 07:43:00.000000 gufo_http-0.3.1/src/headers.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-06-03 07:43:00.000000 gufo_http-0.3.1/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-06-03 07:43:00.000000 gufo_http-0.3.1/src/method.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-06-03 07:43:00.000000 gufo_http-0.3.1/src/proxy.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-06-03 07:43:00.000000 gufo_http-0.3.1/src/response.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-06-03 07:43:00.000000 gufo_http-0.3.1/src/sync_client.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:43:14.019708 gufo_http-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    16919 2024-06-03 07:43:00.000000 gufo_http-0.3.1/tests/test_async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-06-03 07:43:00.000000 gufo_http-0.3.1/tests/test_ci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-06-03 07:43:00.000000 gufo_http-0.3.1/tests/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-06-03 07:43:00.000000 gufo_http-0.3.1/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13012 2024-06-03 07:43:00.000000 gufo_http-0.3.1/tests/test_sync_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-06-03 07:43:00.000000 gufo_http-0.3.1/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-06-03 07:43:00.000000 gufo_http-0.3.1/tests/test_util.py
```

### Comparing `gufo_http-0.3.0/LICENSE.md` & `gufo_http-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gufo_http-0.3.0/PKG-INFO` & `gufo_http-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gufo_http
-Version: 0.3.0
+Version: 0.3.1
 Author: Gufo Labs
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/gufolabs/gufo_http/issues
 Project-URL: Changelog, https://github.com/gufolabs/gufo_http/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://docs.gufolabs.com/gufo_http/
 Project-URL: Homepage, https://github.com/gufolabs/gufo_http/
 Project-URL: Source Code, https://github.com/gufolabs/gufo_http/
```

### Comparing `gufo_http-0.3.0/README.md` & `gufo_http-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `gufo_http-0.3.0/pyproject.toml` & `gufo_http-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gufo_http-0.3.0/src/gufo/http/__init__.py` & `gufo_http-0.3.1/src/gufo/http/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     Proxy,
     RedirectError,
     RequestError,
     RequestMethod,
     Response,
 )
 
-__version__: str = "0.3.0"
+__version__: str = "0.3.1"
 __all__ = [
     "__version__",
     "HttpError",
     "RedirectError",
     "RequestError",
     "Headers",
     "DEFLATE",
```

### Comparing `gufo_http-0.3.0/src/gufo/http/_fast.pyi` & `gufo_http-0.3.1/src/gufo/http/_fast.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     @staticmethod
     def get(name: str) -> Optional["RequestMethod"]: ...
 
 # Constants for compression methods
 DEFLATE: int
 GZIP: int
 BROTLI: int
+ZSTD: int
 
 class Headers(object):
     def __contains__(self: "Headers", k: str) -> bool: ...
     def __getitem__(self: "Headers", k: str) -> bytes: ...
     def get(
         self: "Headers", k: str, default: Optional[bytes]
     ) -> Optional[bytes]: ...
```

### Comparing `gufo_http-0.3.0/src/gufo/http/async_client.py` & `gufo_http-0.3.1/src/gufo/http/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             * **None**: Disable automatic redirect processing.
             * **0**: Deny redirects. Will raise `RedirectError`
                 on 3xx response.
             * **>0**: Follow redirects automatically. Will raise
                 `RedirectError` when redirects limit exceeded.
 
         compression: Acceptable compression methods,
-            must be a combination of `DEFLATE`, `GZIP`, `BROTLI`.
+            must be a combination of `DEFLATE`, `GZIP`, `BROTLI`, and `ZSTD`.
             Set to `None` to disable compression support.
         validate_cert: Set to `False` to disable TLS certificate
             validation. Otherwise, raise `ConnectionError`
             on invalid certificates.
         connect_timeout: Timeout to establish connection, in seconds.
         timeout: Request timeout, in seconds.
         auth: Authentication settings.
```

### Comparing `gufo_http-0.3.0/src/gufo/http/httpd.py` & `gufo_http-0.3.1/src/gufo/http/httpd.py`

 * *Files identical despite different names*

### Comparing `gufo_http-0.3.0/src/gufo/http/sync_client.py` & `gufo_http-0.3.1/src/gufo/http/sync_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             * **None**: Disable automatic redirect processing.
             * **0**: Deny redirects. Will raise `RedirectError`
                 on 3xx response.
             * **>0**: Follow redirects automatically. Will raise
                 `RedirectError` when redirects limit exceeded.
 
         compression: Acceptable compression methods,
-            must be a combination of `DEFLATE`, `GZIP`, `BROTLI`.
+            must be a combination of `DEFLATE`, `GZIP`, `BROTLI`, and `ZSTD`.
             Set to `None` to disable compression support.
         validate_cert: Set to `False` to disable TLS certificate
             validation. Otherwise, raise `ConnectionError`
             on invalid certificates.
         connect_timeout: Timeout to establish connection, in seconds.
         timeout: Request timeout, in seconds.
         auth: Authentication settings.
```

### Comparing `gufo_http-0.3.0/src/gufo/http/util.py` & `gufo_http-0.3.1/src/gufo/http/util.py`

 * *Files identical despite different names*

### Comparing `gufo_http-0.3.0/src/gufo_http.egg-info/PKG-INFO` & `gufo_http-0.3.1/src/gufo_http.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gufo_http
-Version: 0.3.0
+Version: 0.3.1
 Author: Gufo Labs
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/gufolabs/gufo_http/issues
 Project-URL: Changelog, https://github.com/gufolabs/gufo_http/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://docs.gufolabs.com/gufo_http/
 Project-URL: Homepage, https://github.com/gufolabs/gufo_http/
 Project-URL: Source Code, https://github.com/gufolabs/gufo_http/
```

### Comparing `gufo_http-0.3.0/tests/test_async_client.py` & `gufo_http-0.3.1/tests/test_async_client.py`

 * *Files identical despite different names*

### Comparing `gufo_http-0.3.0/tests/test_ci.py` & `gufo_http-0.3.1/tests/test_ci.py`

 * *Files identical despite different names*

### Comparing `gufo_http-0.3.0/tests/test_docs.py` & `gufo_http-0.3.1/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `gufo_http-0.3.0/tests/test_project.py` & `gufo_http-0.3.1/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `gufo_http-0.3.0/tests/test_sync_client.py` & `gufo_http-0.3.1/tests/test_sync_client.py`

 * *Files identical despite different names*

### Comparing `gufo_http-0.3.0/tests/test_types.py` & `gufo_http-0.3.1/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `gufo_http-0.3.0/tests/test_util.py` & `gufo_http-0.3.1/tests/test_util.py`

 * *Files identical despite different names*

