# Comparing `tmp/gevent_requests-0.6.1.tar.gz` & `tmp/gevent_requests-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gevent_requests-0.6.1.tar", last modified: Tue Jul 13 14:41:23 2021, max compression
+gzip compressed data, was "gevent_requests-1.0.0.tar", last modified: Mon Jun  3 14:39:38 2024, max compression
```

## Comparing `gevent_requests-0.6.1.tar` & `gevent_requests-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,6 @@
-drwxr-xr-x   0 vic        (501) staff       (20)        0 2021-07-13 14:41:23.000000 gevent_requests-0.6.1/
--rw-r--r--   0 vic        (501) staff       (20)     1198 2021-07-04 10:34:37.000000 gevent_requests-0.6.1/AUTHORS.rst
--rw-r--r--   0 vic        (501) staff       (20)     1283 2021-07-02 12:39:23.000000 gevent_requests-0.6.1/LICENSE
--rw-r--r--   0 vic        (501) staff       (20)       35 2021-07-02 12:39:23.000000 gevent_requests-0.6.1/MANIFEST.in
--rw-r--r--   0 vic        (501) staff       (20)     1627 2021-07-13 14:41:23.000000 gevent_requests-0.6.1/PKG-INFO
--rw-r--r--   0 vic        (501) staff       (20)     2348 2021-07-13 14:24:48.000000 gevent_requests-0.6.1/README.rst
-drwxr-xr-x   0 vic        (501) staff       (20)        0 2021-07-13 14:41:23.000000 gevent_requests-0.6.1/gevent_requests.egg-info/
--rw-r--r--   0 vic        (501) staff       (20)     1627 2021-07-13 14:41:23.000000 gevent_requests-0.6.1/gevent_requests.egg-info/PKG-INFO
--rw-r--r--   0 vic        (501) staff       (20)      312 2021-07-13 14:41:23.000000 gevent_requests-0.6.1/gevent_requests.egg-info/SOURCES.txt
--rw-r--r--   0 vic        (501) staff       (20)        1 2021-07-13 14:41:23.000000 gevent_requests-0.6.1/gevent_requests.egg-info/dependency_links.txt
--rw-r--r--   0 vic        (501) staff       (20)        1 2021-07-13 14:26:30.000000 gevent_requests-0.6.1/gevent_requests.egg-info/not-zip-safe
--rw-r--r--   0 vic        (501) staff       (20)       20 2021-07-13 14:41:23.000000 gevent_requests-0.6.1/gevent_requests.egg-info/requires.txt
--rw-r--r--   0 vic        (501) staff       (20)       16 2021-07-13 14:41:23.000000 gevent_requests-0.6.1/gevent_requests.egg-info/top_level.txt
--rwxr-xr-x   0 vic        (501) staff       (20)     6280 2021-07-10 13:58:51.000000 gevent_requests-0.6.1/gevent_requests.py
--rw-r--r--   0 vic        (501) staff       (20)      164 2021-07-13 14:41:23.000000 gevent_requests-0.6.1/setup.cfg
--rw-r--r--   0 vic        (501) staff       (20)     1884 2021-07-13 14:41:02.000000 gevent_requests-0.6.1/setup.py
+-rw-r--r--   0        0        0     1283 2021-07-14 14:12:33.743683 gevent_requests-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2684 2024-06-03 14:39:08.989678 gevent_requests-1.0.0/README.md
+-rwxr-xr-x   0        0        0    10765 2024-06-03 14:28:40.615053 gevent_requests-1.0.0/gevent_requests.py
+-rw-r--r--   0        0        0      650 2024-06-03 14:39:38.510793 gevent_requests-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     8866 2024-06-03 14:27:30.130545 gevent_requests-1.0.0/tests.py
+-rw-r--r--   0        0        0     2955 1970-01-01 00:00:00.000000 gevent_requests-1.0.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `gevent_requests-0.6.1/LICENSE` & `gevent_requests-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gevent_requests-0.6.1/README.rst` & `gevent_requests-1.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,79 +1,95 @@
-Gevent-Requests: Asynchronous Requests
-===============================
+Metadata-Version: 2.1
+Name: gevent_requests
+Version: 1.0.0
+Summary: Elegant use of requests in gevent
+Author-Email: belingud <im.victor@qq.com>
+License: BSD
+Requires-Python: >=3.8
+Requires-Dist: requests
+Requires-Dist: gevent>0.8
+Description-Content-Type: text/markdown
 
-Gevent-Requests allows you to use Requests with Gevent to make asynchronous HTTP
+gevent-requests: Asynchronous Requests
+
+---
+
+
+[![version](https://img.shields.io/pypi/v/gevent_requests.svg?colorB=blue)](https://pypi.org/project/gevent-requests/) ![pyversions](https://img.shields.io/pypi/pyversions/gevent_requests.svg) ![PyPI - Downloads](https://img.shields.io/pypi/dm/gevent-requests)
+
+
+gevent-requests allows you to use Requests with Gevent to make asynchronous HTTP
 Requests easily.
 
-|version| |pyversions|
+**Note**: You should probably use [requests-threads](https://github.com/requests/requests-threads) or [requests-futures](https://github.com/ross/requests-futures) instead, implemented using threads.
 
+A fork from `grequests <https://github.com/spyoungtech/grequests>`.
 
-**Note**: You should probably use `requests-threads <https://github.com/requests/requests-threads>`_ or `requests-futures <https://github.com/ross/requests-futures>`_ instead.
+It is highly recommended that you patch from the entry and do not include thread, this package does not include patch!
 
+```shell
+pip install gevent-requests
+```
 
-Usage
------
+---
 
 Usage is simple:
 
-.. code-block:: python
+```python
 
-    from gevent import monkey
-    monkey.patch_all(thread=False, select=False)
-    import grequests
-
-    urls = [
-        'http://www.heroku.com',
-        'http://python-tablib.org',
-        'http://httpbin.org',
-        'http://python-requests.org',
-        'http://fakedomain/',
-        'http://kennethreitz.com'
-    ]
+from gevent import monkey
+monkey.patch_all(thread=False, select=False)
+import gevent_requests
+
+urls = [
+    'http://www.heroku.com',
+    'http://python-tablib.org',
+    'http://httpbin.org',
+    'https://shields.io',
+    'http://fakedomain/',
+]
+```
 
 Create a set of unsent Requests:
 
-.. code-block:: python
-
-    >>> rs = (grequests.get(u) for u in urls)
-
+```python
+>>> rs = (gevent_requests.get(u) for u in urls)
+```
 Send them all at the same time:
 
-.. code-block:: python
-
-    >>> grequests.gmap(rs)
-    [<Response [200]>, <Response [200]>, <Response [200]>, <Response [200]>, None, <Response [200]>]
+```python
+>>> print(gevent_requests.gmap(rs))
+[<Response [200]>, <Response [200]>, <Response [200]>, <Response [200]>, <Response [502]>]
+```
 
 Optionally, in the event of a timeout or any other exception during the connection of
 the request, you can add an exception handler that will be called with the request and
 exception inside the main thread:
 
-.. code-block:: python
-
-    >>> def exception_handler(request, exception):
-    ...    print("Request failed")
-
-    >>> reqs = [
-    ...    grequests.get('http://httpbin.org/delay/1', timeout=0.001),
-    ...    grequests.get('http://fakedomain/'),
-    ...    grequests.get('http://httpbin.org/status/500')]
-    >>> grequests.gmap(reqs, exception_handler=exception_handler)
-    Request failed
-    Request failed
-    [None, None, <Response [500]>]
+```python
+>>> def exception_handler(request, exception):
+...    print("Request failed")
+
+>>> reqs = [
+...    gevent_requests.get('http://httpbin.org/delay/1', timeout=0.001),
+...    gevent_requests.get('http://fakedomain/'),
+...    gevent_requests.get('http://httpbin.org/status/500')]
+>>> print(gevent_requests.gmap(reqs, exception_handler=exception_handler))
+Request failed
+[None, <Response [502]>, <Response [500]>]
+```
 
 For some speed/performance gains, you may also want to use `imap` instead of `map`. `imap` returns a generator of responses. Order of these responses does not map to the order of the requests you send out. The API for `imap` is equivalent to the API for `map`.
 
-Installation
-------------
-
-Installation is easy with pip::
-
-    $ pip install gevent-requests
-    ✨🍰✨
-
+Use indexed requests in gevent, use `gimap_enumerate` will yield a indexed requests just like `enumerate` return, an index and a response:
 
-.. |version| image:: https://img.shields.io/pypi/v/gevent-requests.svg?colorB=blue
-    :target: https://pypi.org/project/gevent-requests/
+```python
+>>> rs = (gevent_requests.get(u) for u in urls)
 
-.. |pyversions| image:: https://img.shields.io/pypi/pyversions/gevent-requests.svg?
-    :target: https://pypi.org/project/gevnent-requests/
+>>> for i in gevent_requests.gimap_enumerate(rs, size=len(urls)):
+        print(i)
+(4, <Response [502]>)
+(2, <Response [200]>)
+(0, <Response [200]>)
+(3, <Response [200]>)
+(1, <Response [200]>)
+```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

