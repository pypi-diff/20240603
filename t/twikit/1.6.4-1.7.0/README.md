# Comparing `tmp/twikit-1.6.4.tar.gz` & `tmp/twikit-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twikit-1.6.4.tar", last modified: Sun May 26 04:01:17 2024, max compression
+gzip compressed data, was "twikit-1.7.0.tar", last modified: Sun Jun  2 15:43:20 2024, max compression
```

## Comparing `twikit-1.6.4.tar` & `twikit-1.7.0.tar`

### file list

```diff
@@ -1,47 +1,53 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 04:01:17.501724 twikit-1.6.4/
--rw-rw-rw-   0        0        0     1079 2024-05-26 04:00:24.000000 twikit-1.6.4/LICENSE
--rw-rw-rw-   0        0        0     3635 2024-05-26 04:01:17.499729 twikit-1.6.4/PKG-INFO
--rw-rw-rw-   0        0        0     3364 2024-05-26 04:00:24.000000 twikit-1.6.4/README.md
--rw-rw-rw-   0        0        0       42 2024-05-26 04:01:17.501724 twikit-1.6.4/setup.cfg
--rw-rw-rw-   0        0        0      694 2024-05-26 04:00:24.000000 twikit-1.6.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 04:01:17.421943 twikit-1.6.4/twikit/
--rw-rw-rw-   0        0        0      713 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/__init__.py
--rw-rw-rw-   0        0        0     1686 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/bookmark.py
--rw-rw-rw-   0        0        0   154823 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/client.py
--rw-rw-rw-   0        0        0     8639 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/community.py
--rw-rw-rw-   0        0        0     2666 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/errors.py
--rw-rw-rw-   0        0        0     2708 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/geo.py
--rw-rw-rw-   0        0        0     7305 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/group.py
--rw-rw-rw-   0        0        0     2218 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/http.py
--rw-rw-rw-   0        0        0     7617 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/list.py
--rw-rw-rw-   0        0        0     3908 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/message.py
--rw-rw-rw-   0        0        0     1439 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/notification.py
--rw-rw-rw-   0        0        0        0 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/py.typed
--rw-rw-rw-   0        0        0     8193 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/streaming.py
--rw-rw-rw-   0        0        0     2825 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/trend.py
--rw-rw-rw-   0        0        0    23780 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/tweet.py
-drwxrwxrwx   0        0        0        0 2024-05-26 04:01:17.495740 twikit-1.6.4/twikit/twikit_async/
--rw-rw-rw-   0        0        0      634 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/twikit_async/__init__.py
--rw-rw-rw-   0        0        0     1758 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/twikit_async/bookmark.py
--rw-rw-rw-   0        0        0   157383 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/twikit_async/client.py
--rw-rw-rw-   0        0        0     8767 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/twikit_async/community.py
--rw-rw-rw-   0        0        0      875 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/twikit_async/errors.py
--rw-rw-rw-   0        0        0     2720 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/twikit_async/geo.py
--rw-rw-rw-   0        0        0     7509 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/twikit_async/group.py
--rw-rw-rw-   0        0        0     2260 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/twikit_async/http.py
--rw-rw-rw-   0        0        0     7780 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/twikit_async/list.py
--rw-rw-rw-   0        0        0     3974 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/twikit_async/message.py
--rw-rw-rw-   0        0        0     1439 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/twikit_async/notification.py
--rw-rw-rw-   0        0        0     8320 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/twikit_async/streaming.py
--rw-rw-rw-   0        0        0     2844 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/twikit_async/trend.py
--rw-rw-rw-   0        0        0    23661 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/twikit_async/tweet.py
--rw-rw-rw-   0        0        0    14740 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/twikit_async/user.py
--rw-rw-rw-   0        0        0     3390 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/twikit_async/utils.py
--rw-rw-rw-   0        0        0    14517 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/user.py
--rw-rw-rw-   0        0        0    31186 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-26 04:01:17.438900 twikit-1.6.4/twikit.egg-info/
--rw-rw-rw-   0        0        0     3635 2024-05-26 04:01:17.000000 twikit-1.6.4/twikit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      951 2024-05-26 04:01:17.000000 twikit-1.6.4/twikit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 04:01:17.000000 twikit-1.6.4/twikit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-26 04:01:17.000000 twikit-1.6.4/twikit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-26 04:01:17.000000 twikit-1.6.4/twikit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 15:43:20.749594 twikit-1.7.0/
+-rw-rw-rw-   0        0        0     1079 2024-05-01 18:21:05.000000 twikit-1.7.0/LICENSE
+-rw-rw-rw-   0        0        0     3635 2024-06-02 15:43:20.747598 twikit-1.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3364 2024-06-02 03:40:33.000000 twikit-1.7.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-02 15:43:20.750589 twikit-1.7.0/setup.cfg
+-rw-rw-rw-   0        0        0      694 2024-05-31 14:57:05.000000 twikit-1.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 15:43:20.647864 twikit-1.7.0/twikit/
+-rw-rw-rw-   0        0        0      746 2024-05-27 06:02:59.000000 twikit-1.7.0/twikit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 15:43:20.675789 twikit-1.7.0/twikit/_captcha/
+-rw-rw-rw-   0        0        0       67 2024-05-26 14:16:02.000000 twikit-1.7.0/twikit/_captcha/__init__.py
+-rw-rw-rw-   0        0        0     3537 2024-05-31 13:32:03.000000 twikit-1.7.0/twikit/_captcha/base.py
+-rw-rw-rw-   0        0        0     2975 2024-06-02 15:18:52.000000 twikit-1.7.0/twikit/_captcha/capsolver.py
+-rw-rw-rw-   0        0        0     1686 2024-05-01 18:21:05.000000 twikit-1.7.0/twikit/bookmark.py
+-rw-rw-rw-   0        0        0   160326 2024-06-02 15:20:18.000000 twikit-1.7.0/twikit/client.py
+-rw-rw-rw-   0        0        0     8639 2024-05-01 18:21:05.000000 twikit-1.7.0/twikit/community.py
+-rw-rw-rw-   0        0        0     2782 2024-06-02 03:52:14.000000 twikit-1.7.0/twikit/errors.py
+-rw-rw-rw-   0        0        0     2708 2024-05-18 16:51:35.000000 twikit-1.7.0/twikit/geo.py
+-rw-rw-rw-   0        0        0     7305 2024-05-01 18:21:05.000000 twikit-1.7.0/twikit/group.py
+-rw-rw-rw-   0        0        0     7617 2024-05-01 18:21:05.000000 twikit-1.7.0/twikit/list.py
+-rw-rw-rw-   0        0        0     3908 2024-05-01 18:21:05.000000 twikit-1.7.0/twikit/message.py
+-rw-rw-rw-   0        0        0     1439 2024-05-01 18:21:05.000000 twikit-1.7.0/twikit/notification.py
+-rw-rw-rw-   0        0        0        0 2024-05-01 18:21:05.000000 twikit-1.7.0/twikit/py.typed
+-rw-rw-rw-   0        0        0     8193 2024-05-04 04:14:29.000000 twikit-1.7.0/twikit/streaming.py
+-rw-rw-rw-   0        0        0     2825 2024-05-04 04:17:28.000000 twikit-1.7.0/twikit/trend.py
+-rw-rw-rw-   0        0        0    23801 2024-06-02 03:40:33.000000 twikit-1.7.0/twikit/tweet.py
+drwxrwxrwx   0        0        0        0 2024-06-02 15:43:20.732638 twikit-1.7.0/twikit/twikit_async/
+-rw-rw-rw-   0        0        0      667 2024-05-31 14:47:23.000000 twikit-1.7.0/twikit/twikit_async/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 15:43:20.743610 twikit-1.7.0/twikit/twikit_async/_captcha/
+-rw-rw-rw-   0        0        0       67 2024-05-26 14:16:02.000000 twikit-1.7.0/twikit/twikit_async/_captcha/__init__.py
+-rw-rw-rw-   0        0        0     3579 2024-05-31 14:15:56.000000 twikit-1.7.0/twikit/twikit_async/_captcha/base.py
+-rw-rw-rw-   0        0        0     2975 2024-06-02 15:17:29.000000 twikit-1.7.0/twikit/twikit_async/_captcha/capsolver.py
+-rw-rw-rw-   0        0        0     1758 2024-05-01 18:21:05.000000 twikit-1.7.0/twikit/twikit_async/bookmark.py
+-rw-rw-rw-   0        0        0   163187 2024-06-02 15:20:24.000000 twikit-1.7.0/twikit/twikit_async/client.py
+-rw-rw-rw-   0        0        0     8767 2024-05-01 18:21:05.000000 twikit-1.7.0/twikit/twikit_async/community.py
+-rw-rw-rw-   0        0        0      875 2024-05-01 18:21:05.000000 twikit-1.7.0/twikit/twikit_async/errors.py
+-rw-rw-rw-   0        0        0     2720 2024-05-18 16:51:29.000000 twikit-1.7.0/twikit/twikit_async/geo.py
+-rw-rw-rw-   0        0        0     7509 2024-05-01 18:21:05.000000 twikit-1.7.0/twikit/twikit_async/group.py
+-rw-rw-rw-   0        0        0     7780 2024-05-01 18:21:05.000000 twikit-1.7.0/twikit/twikit_async/list.py
+-rw-rw-rw-   0        0        0     3974 2024-05-01 18:21:05.000000 twikit-1.7.0/twikit/twikit_async/message.py
+-rw-rw-rw-   0        0        0     1439 2024-05-01 18:21:05.000000 twikit-1.7.0/twikit/twikit_async/notification.py
+-rw-rw-rw-   0        0        0     8320 2024-05-04 04:19:04.000000 twikit-1.7.0/twikit/twikit_async/streaming.py
+-rw-rw-rw-   0        0        0     2844 2024-05-04 04:17:45.000000 twikit-1.7.0/twikit/twikit_async/trend.py
+-rw-rw-rw-   0        0        0    23682 2024-06-02 03:42:22.000000 twikit-1.7.0/twikit/twikit_async/tweet.py
+-rw-rw-rw-   0        0        0    15430 2024-06-02 14:54:05.000000 twikit-1.7.0/twikit/twikit_async/user.py
+-rw-rw-rw-   0        0        0     3379 2024-06-01 04:55:55.000000 twikit-1.7.0/twikit/twikit_async/utils.py
+-rw-rw-rw-   0        0        0    15183 2024-06-02 14:53:37.000000 twikit-1.7.0/twikit/user.py
+-rw-rw-rw-   0        0        0    31177 2024-06-01 04:56:26.000000 twikit-1.7.0/twikit/utils.py
+drwxrwxrwx   0        0        0        0 2024-06-02 15:43:20.665816 twikit-1.7.0/twikit.egg-info/
+-rw-rw-rw-   0        0        0     3635 2024-06-02 15:43:20.000000 twikit-1.7.0/twikit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1109 2024-06-02 15:43:20.000000 twikit-1.7.0/twikit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 15:43:20.000000 twikit-1.7.0/twikit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-06-02 15:43:20.000000 twikit-1.7.0/twikit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-06-02 15:43:20.000000 twikit-1.7.0/twikit.egg-info/top_level.txt
```

### Comparing `twikit-1.6.4/LICENSE` & `twikit-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `twikit-1.6.4/PKG-INFO` & `twikit-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twikit
-Version: 1.6.4
+Version: 1.7.0
 Summary: Twitter API wrapper for python with **no API key required**.
 Home-page: https://github.com/d60/twikit
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `twikit-1.6.4/README.md` & `twikit-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `twikit-1.6.4/setup.py` & `twikit-1.7.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,16 +9,16 @@
     version = re.findall(r"__version__ = '(.+)'", f.read())[0]
 
 setup(
     name='twikit',
     version=version,
     install_requires=[
         'httpx',
-        'fake_useragent',
-        'filetype'
+        'filetype',
+        'beautifulsoup4'
     ],
     python_requires='>=3.10',
     description='Twitter API wrapper for python with **no API key required**.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
     url='https://github.com/d60/twikit',
```

### Comparing `twikit-1.6.4/twikit/__init__.py` & `twikit-1.7.0/twikit/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 Twikit Twitter API Wrapper
 ==========================
 
 https://github.com/d60/twikit
 A Python library for interacting with the Twitter API.
 """
 
-__version__ = '1.6.4'
+__version__ = '1.7.0'
 
+from ._captcha import Capsolver
 from .bookmark import BookmarkFolder
 from .client import Client
 from .community import (Community, CommunityCreator, CommunityMember,
                         CommunityRule)
 from .errors import *
 from .geo import Place
 from .group import Group, GroupMessage
```

### Comparing `twikit-1.6.4/twikit/bookmark.py` & `twikit-1.7.0/twikit/bookmark.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.4/twikit/client.py` & `twikit-1.7.0/twikit/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 from __future__ import annotations
 
 import io
 import json
 import time
 import warnings
 from functools import partial
-from typing import Generator, Literal
+from typing import Any, Generator, Literal
 
 import filetype
-from fake_useragent import UserAgent
+import httpx
 from httpx import Response
 
 from .bookmark import BookmarkFolder
+from ._captcha import Capsolver
 from .community import Community, CommunityMember
 from .errors import (
+    AccountSuspended,
+    BadRequest,
     CouldNotTweet,
+    Forbidden,
     InvalidMedia,
+    NotFound,
+    RequestTimeout,
+    ServerError,
     TweetNotAvailable,
     TwitterException,
+    TooManyRequests,
+    Unauthorized,
     UserNotFound,
     UserUnavailable,
     raise_exceptions_from_response
 )
 from .geo import Place, _places_from_response
 from .group import Group, GroupMessage
-from .http import HTTPClient
 from .list import List
 from .message import Message
 from .notification import Notification
 from .trend import PlaceTrend, PlaceTrends, Location, Trend
 from .streaming import Payload, StreamingSession, _payload_from_data
 from .tweet import CommunityNote, Poll, ScheduledTweet, Tweet, tweet_from_data
 from .user import User
@@ -51,49 +59,161 @@
     find_dict,
     flatten_params,
     get_query_id,
     urlencode
 )
 
 
-class Client:
+class BaseClient:
+    """:meta private:"""
+
+    def __init__(
+        self,
+        language: str | None = None,
+        proxy: str | None = None,
+        captcha_solver: Capsolver | None = None,
+        **kwargs
+    ) -> None:
+        if 'proxies' in kwargs:
+            message = (
+                "The 'proxies' argument is now deprecated. Use 'proxy' "
+                "instead. https://github.com/encode/httpx/pull/2879"
+            )
+            warnings.warn(message)
+
+        self.http = httpx.Client(proxy=proxy, **kwargs)
+        self.language = language
+        self.proxy = proxy
+        self.captcha_solver = captcha_solver
+        if captcha_solver is not None:
+            captcha_solver.client = self
+
+        self._token = TOKEN
+        self._user_id = None
+        self._user_agent = ('Mozilla/5.0 (Windows NT 10.0; Win64; x64) '
+                            'AppleWebKit/537.36 (KHTML, like Gecko) '
+                            'Chrome/122.0.0.0 Safari/537.36')
+        self._act_as = None
+
+    def request(
+        self,
+        method: str,
+        url: str,
+        auto_unlock: bool = True,
+        raise_exception: bool = True,
+        **kwargs
+    ) -> tuple[dict | Any, httpx.Response]:
+        cookies_backup = self.get_cookies().copy()
+        response = self.http.request(method, url, **kwargs)
+        self._remove_duplicate_ct0_cookie()
+
+        try:
+            response_data = response.json()
+        except json.decoder.JSONDecodeError:
+            response_data = response.text
+
+        if isinstance(response_data, dict) and 'errors' in response_data:
+            error_code = response_data['errors'][0]['code']
+            error_message = response_data['errors'][0].get('message')
+            if error_code == 37:
+                # Account suspended
+                raise AccountSuspended(error_message)
+
+            if error_code == 326:
+                # Account unlocking
+                if self.captcha_solver is None:
+                    raise TwitterException(
+                        'Your account is locked. Visit '
+                        'https://twitter.com/account/access to unlock it.'
+                    )
+                if auto_unlock:
+                    self.unlock()
+                    self.set_cookies(cookies_backup, clear_cookies=True)
+                    response = self.http.request(method, url, **kwargs)
+                    self._remove_duplicate_ct0_cookie()
+                    try:
+                        response_data = response.json()
+                    except json.decoder.JSONDecodeError:
+                        response_data = response.text
+
+        status_code = response.status_code
+
+        if status_code >= 400 and raise_exception:
+            message = f'status: {status_code}, message: "{response.text}"'
+            if status_code == 400:
+                raise BadRequest(message, headers=response.headers)
+            elif status_code == 401:
+                raise Unauthorized(message, headers=response.headers)
+            elif status_code == 403:
+                raise Forbidden(message, headers=response.headers)
+            elif status_code == 404:
+                raise NotFound(message, headers=response.headers)
+            elif status_code == 408:
+                raise RequestTimeout(message, headers=response.headers)
+            elif status_code == 429:
+                raise TooManyRequests(message, headers=response.headers)
+            elif 500 <= status_code < 600:
+                raise ServerError(message, headers=response.headers)
+            else:
+                raise TwitterException(message, headers=response.headers)
+
+        return response_data, response
+
+    def get(self, url, **kwargs) -> tuple[dict | Any, httpx.Response]:
+        return self.request('GET', url, **kwargs)
+
+    def post(self, url, **kwargs) -> tuple[dict | Any, httpx.Response]:
+        return self.request('POST', url, **kwargs)
+
+    def stream(self, *args, **kwargs):
+        response = self.http.stream(*args, **kwargs)
+        return response
+
+    def _remove_duplicate_ct0_cookie(self) -> None:
+        cookies = {}
+        for cookie in self.http.cookies.jar:
+            if 'ct0' in cookies and cookie.name == 'ct0':
+                continue
+            cookies[cookie.name] = cookie.value
+        self.http.cookies = list(cookies.items())
+
+
+class Client(BaseClient):
     """
     A client for interacting with the Twitter API.
 
+    Parameters
+    ----------
+    language : :class:`str` | None, default=None
+        The language code to use in API requests.
+    proxy : :class:`str` | None, default=None
+        The proxy server URL to use for request
+        (e.g., 'http://0.0.0.0:0000').
+    captcha_solver : :class:`.Capsolver` | None, default=None
+        See :class:`.Capsolver`.
+
     Examples
     --------
     >>> client = Client(language='en-US')
 
     >>> client.login(
     ...     auth_info_1='example_user',
     ...     auth_info_2='email@example.com',
     ...     password='00000000'
     ... )
     """
-
-    def __init__(
-        self, language: str | None = None,
-        proxies: dict | None = None, **kwargs
-    ) -> None:
-        self._token = TOKEN
-        self.language = language
-        self.http = HTTPClient(proxies=proxies, **kwargs)
-        self._user_id = None
-        self._user_agent = UserAgent().random.strip()
-        self._act_as = None
-
     def _get_guest_token(self) -> str:
         headers = self._base_headers
         headers.pop('X-Twitter-Active-User')
         headers.pop('X-Twitter-Auth-Type')
-        response = self.http.post(
+        response, _ = self.post(
             Endpoint.GUEST_TOKEN,
             headers=headers,
             data={}
-        ).json()
+        )
         guest_token = response['guest_token']
         return guest_token
 
     @property
     def _base_headers(self) -> dict[str, str]:
         """
         Base headers for Twitter API requests.
@@ -107,33 +227,75 @@
             'User-Agent': self._user_agent,
         }
 
         if self.language is not None:
             headers['Accept-Language'] = self.language
             headers['X-Twitter-Client-Language'] = self.language
 
-        csrf_token = self._get_csrf_token()
+        csrf_token = self.http.cookies.get('ct0')
         if csrf_token is not None:
             headers['X-Csrf-Token'] = csrf_token
         if self._act_as is not None:
             headers['X-Act-As-User-Id'] = self._act_as
             headers['X-Contributor-Version'] = '1'
         return headers
 
-    def _get_csrf_token(self) -> str:
-        """
-        Retrieves the Cross-Site Request Forgery (CSRF) token from the
-        current session's cookies.
+    def unlock(self) -> None:
+        if self.captcha_solver is None:
+            raise ValueError('Captcha solver is not provided.')
+
+        response, html = self.captcha_solver.get_unlock_html()
+
+        if html.delete_button:
+            response, html = self.captcha_solver.confirm_unlock(
+                html.authenticity_token,
+                html.assignment_token,
+                ui_metrics=True
+            )
 
-        Returns
-        -------
-        str
-            The CSRF token as a string.
-        """
-        return self.http.client.cookies.get('ct0')
+        if html.start_button or html.finish_button:
+            response, html = self.captcha_solver.confirm_unlock(
+                html.authenticity_token,
+                html.assignment_token,
+                ui_metrics=True
+            )
+
+        cookies_backup = self.get_cookies().copy()
+        max_unlock_attempts = self.captcha_solver.max_attempts
+        attempt = 0
+        while attempt < max_unlock_attempts:
+            attempt += 1
+
+            if html.authenticity_token is None:
+                response, html = self.captcha_solver.get_unlock_html()
+
+            result = self.captcha_solver.solve_funcaptcha(html.blob)
+            if result['errorId'] == 1:
+                continue
+
+            self.set_cookies(cookies_backup, clear_cookies=True)
+            response, html = self.captcha_solver.confirm_unlock(
+                html.authenticity_token,
+                html.assignment_token,
+                result['solution']['token'],
+            )
+
+            if html.finish_button:
+                response, html = self.captcha_solver.confirm_unlock(
+                    html.authenticity_token,
+                    html.assignment_token,
+                    ui_metrics=True
+                )
+            finished = (
+                response.next_request is not None and
+                response.next_request.url.path == '/'
+            )
+            if finished:
+                return
+        raise Exception('could not unlock the account.')
 
     def login(
         self,
         *,
         auth_info_1: str,
         auth_info_2: str | None = None,
         password: str
@@ -162,15 +324,15 @@
         --------
         >>> client.login(
         ...     auth_info_1='example_user',
         ...     auth_info_2='email@example.com',
         ...     password='00000000'
         ... )
         """
-        self.http.client.cookies.clear()
+        self.http.cookies.clear()
         guest_token = self._get_guest_token()
         headers = self._base_headers | {
             'x-guest-token': guest_token
         }
         headers.pop('X-Twitter-Active-User')
         headers.pop('X-Twitter-Auth-Type')
 
@@ -246,30 +408,30 @@
 
         return flow.response
 
     def logout(self) -> Response:
         """
         Logs out of the currently logged-in account.
         """
-        response = self.http.post(
+        _, response = self.http.post(
             Endpoint.LOGOUT,
             headers=self._base_headers
         )
         return response
 
     def user_id(self) -> str:
         """
         Retrieves the user ID associated with the authenticated account.
         """
         if self._user_id is not None:
             return self._user_id
-        response = self.http.get(
+        response, _ = self.get(
             Endpoint.SETTINGS,
             headers=self._base_headers
-        ).json()
+        )
         screen_name = response['screen_name']
         self._user_id = self.get_user_by_screen_name(screen_name).id
         return self._user_id
 
     def user(self) -> User:
         """
         Retrieve detailed information about the authenticated user.
@@ -288,15 +450,15 @@
 
         See Also
         --------
         .set_cookies
         .load_cookies
         .save_cookies
         """
-        return dict(self.http.client.cookies)
+        return dict(self.http.cookies)
 
     def save_cookies(self, path: str) -> None:
         """
         Save cookies to file in json format.
         You can skip the login procedure by loading the saved cookies
         using the :func:`load_cookies` method.
 
@@ -336,16 +498,16 @@
         See Also
         --------
         .get_cookies
         .load_cookies
         .save_cookies
         """
         if clear_cookies:
-            self.http.client.cookies.clear()
-        self.http.client.cookies.update(cookies)
+            self.http.cookies.clear()
+        self.http.cookies.update(cookies)
 
     def load_cookies(self, path: str) -> None:
         """
         Loads cookies from a file.
         You can skip the login procedure by loading a saved cookies.
 
         Parameters
@@ -396,19 +558,19 @@
         }
         if cursor is not None:
             variables['cursor'] = cursor
         params = flatten_params({
             'variables': variables,
             'features': FEATURES
         })
-        response = self.http.get(
+        response, _ = self.get(
             Endpoint.SEARCH_TIMELINE,
             params=params,
             headers=self._base_headers
-        ).json()
+        )
 
         return response
 
     def search_tweet(
         self,
         query: str,
         product: Literal['Top', 'Latest', 'Media'],
@@ -587,19 +749,19 @@
             A list of Tweet objects representing tweets
             similar to the specified tweet.
         """
         params = flatten_params({
             'variables': {'tweet_id': tweet_id},
             'features': SIMILAR_POSTS_FEATURES
         })
-        response = self.http.get(
+        response, _ = self.get(
             Endpoint.SIMILAR_POSTS,
             params=params,
             headers=self._base_headers
-        ).json()
+        )
         items_ = find_dict(response, 'entries')
         results = []
         if not items_:
             return results
 
         for item in items_[0]:
             if not item['entryId'].startswith('tweet'):
@@ -706,19 +868,19 @@
         params = {
             'command': 'INIT',
             'total_bytes': total_bytes,
             'media_type': media_type
         }
         if media_category is not None:
             params['media_category'] = media_category
-        response = self.http.post(
+        response, _ = self.post(
             endpoint,
             params=params,
             headers=self._base_headers
-        ).json()
+        )
         media_id = response['media_id']
         # =========== APPEND ============
         segment_index = 0
         bytes_sent = 0
         MAX_SEGMENT_SIZE = 8 * 1024 * 1024  # The maximum segment size is 8 MB
 
         while bytes_sent < total_bytes:
@@ -734,15 +896,15 @@
             files = {
                 'media': (
                     'blob',
                     chunk_stream,
                     'application/octet-stream',
                 )
             }
-            self.http.post(
+            self.post(
                 endpoint,
                 params=params,
                 headers=headers,
                 files=files
             )
 
             chunk_stream.close()
@@ -750,15 +912,15 @@
             bytes_sent += len(chunk)
 
         # ========== FINALIZE ===========
         params = {
             'command': 'FINALIZE',
             'media_id': media_id,
         }
-        self.http.post(
+        self.post(
             endpoint,
             params=params,
             headers=self._base_headers,
         )
 
         if wait_for_completion:
             while True:
@@ -793,19 +955,19 @@
             'command': 'STATUS',
             'media_id': media_id
         }
         if is_long_video:
             endpoint = Endpoint.UPLOAD_MEDIA_2
         else:
             endpoint = Endpoint.UPLOAD_MEDIA
-        response = self.http.get(
+        response, _ = self.get(
             endpoint,
             params=params,
             headers=self._base_headers
-        ).json()
+        )
         return response
 
     def create_media_metadata(
         self,
         media_id: str,
         alt_text: str | None = None,
         sensitive_warning: list[
@@ -839,29 +1001,20 @@
         >>> client.create_tweet(media_ids=[media_id])
         """
         data = {'media_id': media_id}
         if alt_text is not None:
             data['alt_text'] = {'text': alt_text}
         if sensitive_warning is not None:
             data['sensitive_media_warning'] = sensitive_warning
-        return self.http.post(
+        _, response = self.post(
             Endpoint.CREATE_MEDIA_METADATA,
             json=data,
             headers=self._base_headers
         )
-
-    def get_media(self, url: str) -> bytes:
-        """Retrieves media bytes.
-
-        Parameters
-        ----------
-        url : str
-            Media URL
-        """
-        return self.http.get(url, headers=self._base_headers).content
+        return response
 
     def create_poll(
         self,
         choices: list[str],
         duration_minutes: int
     ) -> str:
         """
@@ -900,19 +1053,19 @@
 
         data = urlencode(
             {'card_data': card_data}
         )
         headers = self._base_headers | {
             'content-type': 'application/x-www-form-urlencoded'
         }
-        response = self.http.post(
+        response, _ = self.post(
             Endpoint.CREATE_CARD,
             data=data,
             headers=headers,
-        ).json()
+        )
 
         return response['card_uri']
 
     def vote(
         self,
         selected_choice: str,
         card_uri: str,
@@ -944,19 +1097,19 @@
             'twitter:string:response_card_name': card_name,
             'twitter:string:cards_platform': 'Web-12',
             'twitter:string:selected_choice': selected_choice
         })
         headers = self._base_headers | {
             'content-type': 'application/x-www-form-urlencoded'
         }
-        response = self.http.post(
+        response, _ = self.post(
             Endpoint.VOTE,
             data=data,
             headers=headers
-        ).json()
+        )
 
         card_data = {
             'rest_id': response['card']['url'],
             'legacy': response['card']
         }
         return Poll(self, card_data, None)
 
@@ -1108,19 +1261,19 @@
             endpoint = Endpoint.CREATE_TWEET
             features = FEATURES
         data = {
             'variables': variables,
             'queryId': get_query_id(Endpoint.CREATE_TWEET),
             'features': features,
         }
-        response = self.http.post(
+        response, _ = self.post(
             endpoint,
             json=data,
             headers=self._base_headers,
-        ).json()
+        )
 
         _result = find_dict(response, 'result')
         if not _result:
             raise_exceptions_from_response(response['errors'])
             raise CouldNotTweet(
                 response['errors'][0]
                 if response['errors']
@@ -1179,19 +1332,19 @@
             },
             'execute_at': scheduled_at
         }
         data = {
             'variables': variables,
             'queryId': get_query_id(Endpoint.CREATE_SCHEDULED_TWEET),
         }
-        response = self.http.post(
+        response, _ = self.post(
             Endpoint.CREATE_SCHEDULED_TWEET,
             json=data,
             headers=self._base_headers,
-        ).json()
+        )
         return response['data']['tweet']['rest_id']
 
     def delete_tweet(self, tweet_id: str) -> Response:
         """Deletes a tweet.
 
         Parameters
         ----------
@@ -1211,15 +1364,15 @@
         data = {
             'variables': {
                 'tweet_id': tweet_id,
                 'dark_request': False
             },
             'queryId': get_query_id(Endpoint.DELETE_TWEET)
         }
-        response = self.http.post(
+        _, response = self.post(
             Endpoint.DELETE_TWEET,
             json=data,
             headers=self._base_headers
         )
         return response
 
     def get_user_by_screen_name(self, screen_name: str) -> User:
@@ -1249,19 +1402,19 @@
             'withSafetyModeUserFields': False
         }
         params = flatten_params({
             'variables': variables,
             'features': USER_FEATURES,
             'fieldToggles': {'withAuxiliaryUserLabels': False}
         })
-        response = self.http.get(
+        response, _ = self.get(
             Endpoint.USER_BY_SCREEN_NAME,
             params=params,
             headers=self._base_headers
-        ).json()
+        )
 
         if 'user' not in response['data']:
             raise UserNotFound('The user does not exist.')
         user_data = response['data']['user']['result']
         if user_data.get('__typename') == 'UserUnavailable':
             raise UserUnavailable(user_data.get('message'))
 
@@ -1293,19 +1446,19 @@
             'userId': user_id,
             'withSafetyModeUserFields': True
         }
         params = flatten_params({
             'variables': variables,
             'features': USER_FEATURES
         })
-        response = self.http.get(
+        response, _ = self.get(
             Endpoint.USER_BY_REST_ID,
             params=params,
             headers=self._base_headers
-        ).json()
+        )
         if 'result' not in response['data']['user']:
             raise TwitterException(f'Invalid user id: {user_id}')
         user_data = response['data']['user']['result']
         if user_data.get('__typename') == 'UserUnavailable':
             raise UserUnavailable(user_data.get('message'))
         return User(self, user_data)
 
@@ -1341,19 +1494,19 @@
             'granularity': granularity,
             'max_results': max_results
         }
         for k, v in tuple(params.items()):
             if v is None:
                 params.pop(k)
 
-        response = self.http.get(
+        response, _ = self.get(
             Endpoint.REVERSE_GEOCODE,
             params=params,
             headers=self._base_headers
-        ).json()
+        )
         return _places_from_response(self, response)
 
     def search_geo(
         self, lat: float | None = None, long: float | None = None,
         query: str | None = None, ip: str | None = None,
         granularity: str | None = None, max_results: int | None = None
     ) -> list[Place]:
@@ -1392,36 +1545,36 @@
             'granularity': granularity,
             'max_results': max_results
         }
         for k, v in tuple(params.items()):
             if v is None:
                 params.pop(k)
 
-        response = self.http.get(
+        response, _ = self.get(
             Endpoint.SEARCH_GEO,
             params=params,
             headers=self._base_headers
-        ).json()
+        )
         return _places_from_response(self, response)
 
     def get_place(self, id: str) -> Place:
         """
         Parameters
         ----------
         id : :class:`str`
             The ID of the place.
 
         Returns
         -------
         :class:`.Place`
         """
-        response = self.http.get(
+        response, _ = self.get(
             Endpoint.PLACE_BY_ID.format(id),
             headers=self._base_headers
-        ).json()
+        )
         return Place(self, response)
 
     def _get_tweet_detail(self, tweet_id: str, cursor: str | None):
         variables = {
             'focalTweetId': tweet_id,
             'with_rux_injections': False,
             'includePromotedContent': True,
@@ -1434,19 +1587,19 @@
         if cursor is not None:
             variables['cursor'] = cursor
         params = flatten_params({
             'variables': variables,
             'features': FEATURES,
             'fieldToggles': {'withAuxiliaryUserLabels': False}
         })
-        response = self.http.get(
+        response, _ = self.get(
             Endpoint.TWEET_DETAIL,
             params=params,
             headers=self._base_headers
-        ).json()
+        )
         return response
 
     def _get_more_replies(self, tweet_id: str, cursor: str) -> Result[Tweet]:
         response = self._get_tweet_detail(tweet_id, cursor)
         entries = find_dict(response, 'entries')[0]
 
         results = []
@@ -1591,19 +1744,19 @@
         -------
         list[:class:`ScheduledTweet`]
             List of ScheduledTweet objects representing the scheduled tweets.
         """
         params = flatten_params({
             'variables': {'ascending': True}
         })
-        response = self.http.get(
+        response, _ = self.get(
             Endpoint.FETCH_SCHEDULED_TWEETS,
             params=params,
             headers=self._base_headers
-        ).json()
+        )
         tweets = find_dict(response, 'scheduled_tweet_list')[0]
         return [ScheduledTweet(self, tweet) for tweet in tweets]
 
     def delete_scheduled_tweet(self, tweet_id: str) -> Response:
         """
         Delete a scheduled tweet.
 
@@ -1619,15 +1772,15 @@
         """
         data = {
             'variables': {
                 'scheduled_tweet_id': tweet_id
             },
             'queryId': get_query_id(Endpoint.DELETE_SCHEDULED_TWEET)
         }
-        response = self.http.post(
+        _, response = self.post(
             Endpoint.DELETE_SCHEDULED_TWEET,
             json=data,
             headers=self._base_headers
         )
         return response
 
     def _get_tweet_engagements(
@@ -1643,19 +1796,19 @@
         }
         if cursor is not None:
             variables['cursor'] = cursor
         params = flatten_params({
             'variables': variables,
             'features': FEATURES
         })
-        response = self.http.get(
+        response, _ = self.get(
             endpoint,
             params=params,
             headers=self._base_headers
-        ).json()
+        )
         items_ = find_dict(response, 'entries')
         if not items_:
             return Result([])
         items = items_[0]
         next_cursor = items[-1]['content']['value']
         previous_cursor = items[-2]['content']['value']
 
@@ -1775,19 +1928,19 @@
         >>> print(note)
         <CommunityNote id="...">
         """
         params = flatten_params({
             'variables': {'note_id': note_id},
             'features': COMMUNITY_NOTE_FEATURES
         })
-        response = self.http.get(
+        response, _ = self.get(
             Endpoint.FETCH_COMMUNITY_NOTE,
             params=params,
             headers=self._base_headers
-        ).json()
+        )
         note_data = response['data']['birdwatch_note_by_rest_id']
         if 'data_v1' not in note_data:
             raise TwitterException(f'Invalid note id: {note_id}')
         return CommunityNote(
             self, note_data
         )
 
@@ -1870,19 +2023,19 @@
         endpoint = {
             'Tweets': Endpoint.USER_TWEETS,
             'Replies': Endpoint.USER_TWEETS_AND_REPLIES,
             'Media': Endpoint.USER_MEDIA,
             'Likes': Endpoint.USER_LIKES,
         }[tweet_type]
 
-        response = self.http.get(
+        response, _ = self.get(
             endpoint,
             params=params,
             headers=self._base_headers
-        ).json()
+        )
 
         instructions_ = find_dict(response, 'instructions')
         if not instructions_:
             return Result([])
         instructions = instructions_[0]
 
         items = instructions[-1]['entries']
@@ -1985,19 +2138,19 @@
             variables['cursor'] = cursor
 
         data = {
             'variables': variables,
             'queryId': get_query_id(Endpoint.HOME_TIMELINE),
             'features': FEATURES,
         }
-        response = self.http.post(
+        response, _ = self.post(
             Endpoint.HOME_TIMELINE,
             json=data,
             headers=self._base_headers
-        ).json()
+        )
 
         items = find_dict(response, 'entries')[0]
         next_cursor = items[-1]['content']['value']
         results = []
 
         for item in items:
             if 'itemContent' not in item['content']:
@@ -2066,19 +2219,19 @@
             variables['cursor'] = cursor
 
         data = {
             'variables': variables,
             'queryId': get_query_id(Endpoint.HOME_LATEST_TIMELINE),
             'features': FEATURES,
         }
-        response = self.http.post(
+        response, _ = self.post(
             Endpoint.HOME_LATEST_TIMELINE,
             json=data,
             headers=self._base_headers
-        ).json()
+        )
 
         items = find_dict(response, 'entries')[0]
         next_cursor = items[-1]['content']['value']
         results = []
 
         for item in items:
             if 'itemContent' not in item['content']:
@@ -2118,15 +2271,15 @@
         --------
         .unfavorite_tweet
         """
         data = {
             'variables': {'tweet_id': tweet_id},
             'queryId': get_query_id(Endpoint.FAVORITE_TWEET)
         }
-        response = self.http.post(
+        _, response = self.post(
             Endpoint.FAVORITE_TWEET,
             json=data,
             headers=self._base_headers
         )
         return response
 
     def unfavorite_tweet(self, tweet_id: str) -> Response:
@@ -2152,15 +2305,15 @@
         --------
         .favorite_tweet
         """
         data = {
             'variables': {'tweet_id': tweet_id},
             'queryId': get_query_id(Endpoint.UNFAVORITE_TWEET)
         }
-        response = self.http.post(
+        _, response = self.post(
             Endpoint.UNFAVORITE_TWEET,
             json=data,
             headers=self._base_headers
         )
         return response
 
     def retweet(self, tweet_id: str) -> Response:
@@ -2186,15 +2339,15 @@
         --------
         .delete_retweet
         """
         data = {
             'variables': {'tweet_id': tweet_id, 'dark_request': False},
             'queryId': get_query_id(Endpoint.CREATE_RETWEET)
         }
-        response = self.http.post(
+        _, response = self.post(
             Endpoint.CREATE_RETWEET,
             json=data,
             headers=self._base_headers
         )
         return response
 
     def delete_retweet(self, tweet_id: str) -> Response:
@@ -2220,15 +2373,15 @@
         --------
         .retweet
         """
         data = {
             'variables': {'source_tweet_id': tweet_id,'dark_request': False},
             'queryId': get_query_id(Endpoint.DELETE_RETWEET)
         }
-        response = self.http.post(
+        _, response = self.post(
             Endpoint.DELETE_RETWEET,
             json=data,
             headers=self._base_headers
         )
         return response
 
     def bookmark_tweet(
@@ -2261,15 +2414,15 @@
             endpoint = Endpoint.BOOKMARK_TO_FOLDER
             variables['bookmark_collection_id'] = folder_id
 
         data = {
             'variables': variables,
             'queryId': get_query_id(Endpoint.CREATE_BOOKMARK)
         }
-        response = self.http.post(
+        _, response = self.post(
             endpoint,
             json=data,
             headers=self._base_headers
         )
         return response
 
     def delete_bookmark(self, tweet_id: str) -> Response:
@@ -2295,15 +2448,15 @@
         --------
         .bookmark_tweet
         """
         data = {
             'variables': {'tweet_id': tweet_id},
             'queryId': get_query_id(Endpoint.DELETE_BOOKMARK)
         }
-        response = self.http.post(
+        _, response = self.post(
             Endpoint.DELETE_BOOKMARK,
             json=data,
             headers=self._base_headers
         )
         return response
 
     def get_bookmarks(
@@ -2356,19 +2509,19 @@
 
         if cursor is not None:
             variables['cursor'] = cursor
         params = flatten_params({
             'variables': variables,
             'features': features
         })
-        response = self.http.get(
+        response, _ = self.get(
             endpoint,
             params=params,
             headers=self._base_headers
-        ).json()
+        )
 
         items_ = find_dict(response, 'entries')
         if not items_:
             return Result([])
         items = items_[0]
         next_cursor = items[-1]['content']['value']
         if folder_id is None:
@@ -2409,15 +2562,15 @@
         --------
         >>> client.delete_all_bookmarks()
         """
         data = {
             'variables': {},
             'queryId': get_query_id(Endpoint.BOOKMARKS_ALL_DELETE)
         }
-        response = self.http.post(
+        _, response = self.post(
             Endpoint.BOOKMARKS_ALL_DELETE,
             json=data,
             headers=self._base_headers
         )
         return response
 
     def get_bookmark_folders(
@@ -2438,19 +2591,19 @@
         [<BookmarkFolder id="...">, ..., <BookmarkFolder id="...">]
         >>> more_folders = folders.next()  # Retrieve more folders
         """
         variables = {}
         if cursor is not None:
             variables['cursor'] = cursor
         params = flatten_params({'variables': variables})
-        response = self.http.get(
+        response, _ = self.get(
             Endpoint.BOOKMARK_FOLDERS,
             params=params,
             headers=self._base_headers
-        ).json()
+        )
 
         slice = find_dict(response, 'bookmark_collections_slice')[0]
         results = []
         for item in slice['items']:
             results.append(BookmarkFolder(self, item))
 
         if 'next_cursor' in slice['slice_info']:
@@ -2492,19 +2645,19 @@
             'bookmark_collection_id': folder_id,
             'name': name
         }
         data = {
             'variables': variables,
             'queryId': get_query_id(Endpoint.EDIT_BOOKMARK_FOLDER)
         }
-        response = self.http.post(
+        response, _ = self.post(
             Endpoint.EDIT_BOOKMARK_FOLDER,
             json=data,
             headers=self._base_headers
-        ).json()
+        )
         return BookmarkFolder(
             self, response['data']['bookmark_collection_update']
         )
 
     def delete_bookmark_folder(self, folder_id: str) -> Response:
         """
         Deletes a bookmark folder.
@@ -2522,15 +2675,15 @@
         variables = {
             'bookmark_collection_id': folder_id
         }
         data = {
             'variables': variables,
             'queryId': get_query_id(Endpoint.DELETE_BOOKMARK_FOLDER)
         }
-        response = self.http.post(
+        _, response = self.post(
             Endpoint.DELETE_BOOKMARK_FOLDER,
             json=data,
             headers=self._base_headers
         )
         return response
 
     def create_bookmark_folder(self, name: str) -> BookmarkFolder:
@@ -2549,19 +2702,19 @@
         variables = {
             'name': name
         }
         data = {
             'variables': variables,
             'queryId': get_query_id(Endpoint.CREATE_BOOKMARK_FOLDER)
         }
-        response = self.http.post(
+        response, _ = self.post(
             Endpoint.CREATE_BOOKMARK_FOLDER,
             json=data,
             headers=self._base_headers
-        ).json()
+        )
         return BookmarkFolder(
             self, response['data']['bookmark_collection_create']
         )
 
     def follow_user(self, user_id: str) -> Response:
         """
         Follows a user.
@@ -2599,15 +2752,15 @@
             'include_ext_profile_image_shape': 1,
             'skip_status': 1,
             'user_id': user_id
         })
         headers = self._base_headers | {
             'content-type': 'application/x-www-form-urlencoded'
         }
-        response = self.http.post(
+        _, response = self.post(
             Endpoint.CREATE_FRIENDSHIPS,
             data=data,
             headers=headers
         )
         return response
 
     def unfollow_user(self, user_id: str) -> Response:
@@ -2647,15 +2800,15 @@
             'include_ext_profile_image_shape': 1,
             'skip_status': 1,
             'user_id': user_id
         })
         headers = self._base_headers | {
             'content-type': 'application/x-www-form-urlencoded'
         }
-        response = self.http.post(
+        _, response = self.post(
             Endpoint.DESTROY_FRIENDSHIPS,
             data=data,
             headers=headers
         )
         return response
 
     def block_user(self, user_id: str) -> Response:
@@ -2675,15 +2828,15 @@
         See Also
         --------
         .unblock_user
         """
         data = urlencode({'user_id': user_id})
         headers = self._base_headers
         headers['content-type'] = 'application/x-www-form-urlencoded'
-        response = self.http.post(
+        _, response = self.post(
             Endpoint.BLOCK_USER,
             data=data,
             headers=headers
         )
         return response
 
     def unblock_user(self, user_id: str) -> Response:
@@ -2703,15 +2856,15 @@
         See Also
         --------
         .block_user
         """
         data = urlencode({'user_id': user_id})
         headers = self._base_headers
         headers['content-type'] = 'application/x-www-form-urlencoded'
-        response = self.http.post(
+        _, response = self.post(
             Endpoint.UNBLOCK_USER,
             data=data,
             headers=headers
         )
         return response
 
     def mute_user(self, user_id: str) -> Response:
@@ -2731,15 +2884,15 @@
         See Also
         --------
         .unmute_user
         """
         data = urlencode({'user_id': user_id})
         headers = self._base_headers
         headers['content-type'] = 'application/x-www-form-urlencoded'
-        response = self.http.post(
+        _, response = self.post(
             Endpoint.MUTE_USER,
             data=data,
             headers=headers
         )
         return response
 
     def unmute_user(self, user_id: str) -> Response:
@@ -2759,15 +2912,15 @@
         See Also
         --------
         .mute_user
         """
         data = urlencode({'user_id': user_id})
         headers = self._base_headers
         headers['content-type'] = 'application/x-www-form-urlencoded'
-        response = self.http.post(
+        _, response = self.post(
             Endpoint.UNMUTE_USER,
             data=data,
             headers=headers
         )
         return response
 
     def get_trends(
@@ -2821,19 +2974,19 @@
         params = {
             'count': count,
             'include_page_configuration': True,
             'initial_tab_id': category
         }
         if additional_request_params is not None:
             params |= additional_request_params
-        response = self.http.get(
+        response, _ = self.get(
             Endpoint.TREND,
             params=params,
             headers=self._base_headers
-        ).json()
+        )
 
         entry_id_prefix = 'trends' if category == 'trending' else 'Guide'
         entries = [
             i for i in find_dict(response, 'entries')[0]
             if i['entryId'].startswith(entry_id_prefix)
         ]
 
@@ -2859,31 +3012,31 @@
         """
         Retrieves locations where trends can be retrieved.
 
         Returns
         -------
         list[:class:`.Location`]
         """
-        response = self.http.get(
+        response, _ = self.get(
             Endpoint.AVAILABLE_LOCATIONS,
             headers=self._base_headers
-        ).json()
+        )
         return [Location(self, data) for data in response]
 
     def get_place_trends(self, woeid: int) -> PlaceTrends:
         """
         Retrieves the top 50 trending topics for a specific id.
         You can get available woeid using
         :attr:`.Client.get_available_locations`.
         """
-        response = self.http.get(
+        response, _ = self.get(
             Endpoint.PLACE_TRENDS,
             params={'id': woeid},
             headers=self._base_headers
-        ).json()
+        )
         trend_data = response[0]
         trends = [PlaceTrend(self, data) for data in trend_data['trends']]
         trend_data['trends'] = trends
         return trend_data
 
     def _get_user_friendship(
         self,
@@ -2902,19 +3055,19 @@
         }
         if cursor is not None:
             variables['cursor'] = cursor
         params = flatten_params({
             'variables': variables,
             'features': FEATURES
         })
-        response = self.http.get(
+        response, _ = self.get(
             endpoint,
             params=params,
             headers=self._base_headers
-        ).json()
+        )
 
         items = find_dict(response, 'entries')[0]
         results = []
         for item in items:
             entry_id = item['entryId']
             if entry_id.startswith('user'):
                 user_info = find_dict(item, 'result')
@@ -2947,19 +3100,19 @@
             params['user_id'] = user_id
         elif user_id is not None:
             params['screen_name'] = screen_name
 
         if cursor is not None:
             params['cursor'] = cursor
 
-        response = self.http.get(
+        response, _ = self.get(
             endpoint,
             params=params,
             headers=self._base_headers
-        ).json()
+        )
 
         users = response['users']
         results = []
         for user in users:
             results.append(User(self, build_user_data(user)))
 
         previous_cursor = response['previous_cursor']
@@ -3146,19 +3299,19 @@
             params['user_id'] = user_id
         elif user_id is not None:
             params['screen_name'] = screen_name
 
         if cursor is not None:
             params['cursor'] = cursor
 
-        response = self.http.get(
+        response, _ = self.get(
             endpoint,
             params=params,
             headers=self._base_headers
-        ).json()
+        )
         previous_cursor = response['previous_cursor']
         next_cursor = response['next_cursor']
 
         return Result(
             response['ids'],
             partial(self._get_friendship_ids, user_id,
                      screen_name, count, endpoint, next_cursor),
@@ -3252,19 +3405,20 @@
             'text': text
         }
         if media_id is not None:
             data['media_id'] = media_id
         if reply_to is not None:
             data['reply_to_dm_id'] = reply_to
 
-        return self.http.post(
+        response, _ = self.post(
             Endpoint.SEND_DM,
             json=data,
             headers=self._base_headers
-        ).json()
+        )
+        return response
 
     def _get_dm_history(
         self,
         conversation_id: str,
         max_id: str | None = None
     ) -> dict:
         """
@@ -3272,19 +3426,20 @@
         """
         params = {
             'context': 'FETCH_DM_CONVERSATION_HISTORY'
         }
         if max_id is not None:
             params['max_id'] = max_id
 
-        return self.http.get(
+        response, _ = self.get(
             Endpoint.CONVERSATION.format(conversation_id),
             params=params,
             headers=self._base_headers
-        ).json()
+        )
+        return response
 
     def send_dm(
         self,
         user_id: str,
         text: str,
         media_id: str | None = None,
         reply_to: str | None = None
@@ -3372,15 +3527,15 @@
             'reactionTypes': ['Emoji'],
             'emojiReactions': [emoji]
         }
         data = {
             'variables': variables,
             'queryId': get_query_id(Endpoint.MESSAGE_ADD_REACTION)
         }
-        response = self.http.post(
+        _, response = self.post(
             Endpoint.MESSAGE_ADD_REACTION,
             json=data,
             headers=self._base_headers
         )
         return response
 
     def remove_reaction_from_message(
@@ -3418,15 +3573,15 @@
             'reactionTypes': ['Emoji'],
             'emojiReactions': [emoji]
         }
         data = {
             'variables': variables,
             'queryId': get_query_id(Endpoint.MESSAGE_REMOVE_REACTION)
         }
-        response = self.http.post(
+        _, response = self.post(
             Endpoint.MESSAGE_REMOVE_REACTION,
             json=data,
             headers=self._base_headers
         )
         return response
 
     def delete_dm(self, message_id: str) -> Response:
@@ -3450,15 +3605,15 @@
 
         data = {
             'variables': {
                 'messageId': message_id
             },
             'queryId': get_query_id(Endpoint.DELETE_DM)
         }
-        response = self.http.post(
+        _, response = self.post(
             Endpoint.DELETE_DM,
             json=data,
             headers=self._base_headers
         )
         return response
 
     def get_dm_history(
@@ -3649,19 +3804,19 @@
         :class:`Group`
             An object representing the retrieved group.
         """
         params = {
             'context': 'FETCH_DM_CONVERSATION_HISTORY',
             'include_conversation_info': True,
         }
-        response = self.http.get(
+        response, _ = self.get(
             Endpoint.CONVERSATION.format(group_id),
             params=params,
             headers=self._base_headers
-        ).json()
+        )
         return Group(self, group_id, response)
 
     def add_members_to_group(
         self, group_id: str, user_ids: list[str]
     ) -> Response:
         """Adds members to a group.
 
@@ -3686,15 +3841,15 @@
         data = {
             'variables': {
                 'addedParticipants': user_ids,
                 'conversationId': group_id
             },
             'queryId': get_query_id(Endpoint.ADD_MEMBER_TO_GROUP)
         }
-        response = self.http.post(
+        _, response = self.post(
             Endpoint.ADD_MEMBER_TO_GROUP,
             json=data,
             headers=self._base_headers
         )
         return response
 
     def change_group_name(self, group_id: str, name: str) -> Response:
@@ -3713,15 +3868,15 @@
             Response returned from twitter api.
         """
         data = urlencode({
             'name': name
         })
         headers = self._base_headers
         headers['content-type'] = 'application/x-www-form-urlencoded'
-        response = self.http.post(
+        _, response = self.post(
             Endpoint.CHANGE_GROUP_NAME.format(group_id),
             data=data,
             headers=headers
         )
         return response
 
     def create_list(
@@ -3760,19 +3915,19 @@
             'description': description
         }
         data = {
             'variables': variables,
             'features': LIST_FEATURES,
             'queryId': get_query_id(Endpoint.CREATE_LIST)
         }
-        response = self.http.post(
+        response, _ = self.post(
             Endpoint.CREATE_LIST,
             json=data,
             headers=self._base_headers
-        ).json()
+        )
         list_info = find_dict(response, 'list')[0]
         return List(self, list_info)
 
     def edit_list_banner(self, list_id: str, media_id: str) -> Response:
         """
         Edit the banner image of a list.
 
@@ -3799,15 +3954,15 @@
             'mediaId': media_id
         }
         data = {
             'variables': variables,
             'features': LIST_FEATURES,
             'queryId': get_query_id(Endpoint.EDIT_LIST_BANNER)
         }
-        response = self.http.post(
+        _, response = self.post(
             Endpoint.EDIT_LIST_BANNER,
             json=data,
             headers=self._base_headers
         )
         return response
 
     def delete_list_banner(self, list_id: str) -> Response:
@@ -3826,15 +3981,15 @@
         data = {
             'variables': {
                 'listId': list_id
             },
             'features': LIST_FEATURES,
             'queryId': get_query_id(Endpoint.DELETE_LIST_BANNER)
         }
-        response = self.http.post(
+        _, response = self.post(
             Endpoint.DELETE_LIST_BANNER,
             json=data,
             headers=self._base_headers
         )
         return response
 
     def edit_list(
@@ -3880,19 +4035,19 @@
         if is_private is not None:
             variables['isPrivate'] = is_private
         data = {
             'variables': variables,
             'features': LIST_FEATURES,
             'queryId': get_query_id(Endpoint.UPDATE_LIST)
         }
-        response = self.http.post(
+        response, _ = self.post(
             Endpoint.UPDATE_LIST,
             json=data,
             headers=self._base_headers
-        ).json()
+        )
         list_info = find_dict(response, 'list')[0]
         return List(self, list_info)
 
     def add_list_member(self, list_id: str, user_id: str) -> Response:
         """
         Adds a user to a list.
 
@@ -3917,15 +4072,15 @@
             'userId': user_id
         }
         data = {
             'variables': variables,
             'features': LIST_FEATURES,
             'queryId': get_query_id(Endpoint.LIST_ADD_MEMBER)
         }
-        response = self.http.post(
+        _, response = self.post(
             Endpoint.LIST_ADD_MEMBER,
             json=data,
             headers=self._base_headers
         )
         return response
 
     def remove_list_member(self, list_id: str, user_id: str) -> Response:
@@ -3953,15 +4108,15 @@
             'userId': user_id
         }
         data = {
             'variables': variables,
             'features': LIST_FEATURES,
             'queryId': get_query_id(Endpoint.LIST_REMOVE_MEMBER)
         }
-        response = self.http.post(
+        _, response = self.post(
             Endpoint.LIST_REMOVE_MEMBER,
             json=data,
             headers=self._base_headers
         )
         return response
 
     def get_lists(
@@ -3996,19 +4151,19 @@
         }
         if cursor is not None:
             variables['cursor'] = cursor
         params = flatten_params({
             'variables': variables,
             'features': FEATURES
         })
-        response = self.http.get(
+        response, _ = self.get(
             Endpoint.LIST_MANAGEMENT,
             params=params,
             headers=self._base_headers
-        ).json()
+        )
 
         entries = find_dict(response, 'entries')[0]
         items = find_dict(entries, 'items')
 
         if len(items) < 2:
             return Result([])
 
@@ -4040,19 +4195,19 @@
         :class:`List`
             List object.
         """
         params = flatten_params({
             'variables': {'listId': list_id},
             'features': LIST_FEATURES
         })
-        response = self.http.get(
+        response, _ = self.get(
             Endpoint.LIST_BY_REST_ID,
             params=params,
             headers=self._base_headers
-        ).json()
+        )
         list_info = find_dict(response, 'list')[0]
         return List(self, list_info)
 
     def get_list_tweets(
         self, list_id: str, count: int = 20, cursor: str | None = None
     ) -> Result[Tweet]:
         """
@@ -4096,19 +4251,19 @@
         }
         if cursor is not None:
             variables['cursor'] = cursor
         params = flatten_params({
             'variables': variables,
             'features': FEATURES
         })
-        response = self.http.get(
+        response, _ = self.get(
             Endpoint.LIST_LATEST_TWEETS,
             params=params,
             headers=self._base_headers
-        ).json()
+        )
 
         items = find_dict(response, 'entries')[0]
         next_cursor = items[-1]['content']['value']
 
         results = []
         for item in items:
             if not item['entryId'].startswith('tweet'):
@@ -4136,19 +4291,19 @@
         }
         if cursor is not None:
             variables['cursor'] = cursor
         params = flatten_params({
             'variables': variables,
             'features': FEATURES
         })
-        response = self.http.get(
+        response, _ = self.get(
             endpoint,
             params=params,
             headers=self._base_headers
-        ).json()
+        )
 
         items = find_dict(response, 'entries')[0]
         results = []
         for item in items:
             entry_id = item['entryId']
             if entry_id.startswith('user'):
                 user_info = find_dict(item, 'result')[0]
@@ -4330,19 +4485,19 @@
 
         params = {
             'count': count
         }
         if cursor is not None:
             params['cursor'] = cursor
 
-        response = self.http.get(
+        response, _ = self.get(
             endpoint,
             params=params,
             headers=self._base_headers
-        ).json()
+        )
 
         global_objects = response['globalObjects']
         users = {
             id: User(self, build_user_data(data))
             for id, data in global_objects.get('users', {}).items()
         }
         tweets = {}
@@ -4420,19 +4575,19 @@
             'query': query,
         }
         if cursor is not None:
             variables['cursor'] = cursor
         params = flatten_params({
             'variables': variables
         })
-        response = self.http.get(
+        response, _ = self.get(
             Endpoint.SEARCH_COMMUNITY,
             params=params,
             headers=self._base_headers
-        ).json()
+        )
 
         items = find_dict(response, 'items_results')[0]
         communities = []
         for item in items:
             communities.append(Community(self, item['result']))
         next_cursor_ = find_dict(response, 'next_cursor')
         next_cursor = next_cursor_[0] if next_cursor_ else None
@@ -4464,19 +4619,19 @@
         params = flatten_params({
             'variables': {'communityId': community_id},
             'features': {
                 'c9s_list_members_action_api_enabled':False,
                 'c9s_superc9s_indication_enabled':False
             }
         })
-        response = self.http.get(
+        response, _ = self.get(
             Endpoint.GET_COMMUNITY,
             params=params,
             headers=self._base_headers
-        ).json()
+        )
         community_data = find_dict(response, 'result')[0]
         return Community(self, community_data)
 
     def get_community_tweets(
         self,
         community_id: str,
         tweet_type: Literal['Top', 'Latest', 'Media'],
@@ -4531,19 +4686,19 @@
         if cursor is not None:
             variables['cursor'] = cursor
 
         params = flatten_params({
             'variables': variables,
             'features': COMMUNITY_TWEETS_FEATURES
         })
-        response = self.http.get(
+        response, _ = self.get(
             endpoint,
             params=params,
             headers=self._base_headers
-        ).json()
+        )
 
         entries = find_dict(response, 'entries')[0]
         if tweet_type == 'Media':
             if cursor is None:
                 items = entries[0]['content']['items']
                 next_cursor = entries[-1]['content']['value']
                 previous_cursor = entries[-2]['content']['value']
@@ -4607,19 +4762,19 @@
         }
         if cursor is not None:
             variables['cursor'] = cursor
         params = flatten_params({
             'variables': variables,
             'features': COMMUNITY_TWEETS_FEATURES
         })
-        response = self.http.get(
+        response, _ = self.get(
             Endpoint.COMMUNITIES_TIMELINE,
             params=params,
             headers=self._base_headers
-        ).json()
+        )
         items = find_dict(response, 'entries')[0]
         tweets = []
         for item in items:
             if not item['entryId'].startswith('tweet'):
                 continue
             tweet = tweet_from_data(self, item)
             tweet_data = find_dict(item, 'result')[0]
@@ -4663,19 +4818,19 @@
         data = {
             'variables': {
                 'communityId': community_id
             },
             'features': JOIN_COMMUNITY_FEATURES,
             'queryId': get_query_id(Endpoint.JOIN_COMMUNITY)
         }
-        response = self.http.post(
+        response, _ = self.post(
             Endpoint.JOIN_COMMUNITY,
             json=data,
             headers=self._base_headers
-        ).json()
+        )
         community_data = response['data']['community_join']
         community_data['rest_id'] = community_data['id_str']
         return Community(self, community_data)
 
     def leave_community(self, community_id: str) -> Community:
         """
         Leave a community.
@@ -4693,19 +4848,19 @@
         data = {
             'variables': {
                 'communityId': community_id
             },
             'features': JOIN_COMMUNITY_FEATURES,
             'queryId': get_query_id(Endpoint.LEAVE_COMMUNITY)
         }
-        response = self.http.post(
+        response, _ = self.post(
             Endpoint.LEAVE_COMMUNITY,
             json=data,
             headers=self._base_headers
-        ).json()
+        )
         community_data = response['data']['community_leave']
         community_data['rest_id'] = community_data['id_str']
         return Community(self, community_data)
 
     def request_to_join_community(
         self, community_id: str, answer: str | None = None
     ) -> Community:
@@ -4728,19 +4883,19 @@
             'variables': {
                 'communityId': community_id,
                 'answer': '' if answer is None else answer
             },
             'features': JOIN_COMMUNITY_FEATURES,
             'queryId': get_query_id(Endpoint.REQUEST_TO_JOIN_COMMUNITY)
         }
-        response = self.http.post(
+        response, _ = self.post(
             Endpoint.REQUEST_TO_JOIN_COMMUNITY,
             json=data,
             headers=self._base_headers
-        ).json()
+        )
         community_data = find_dict(response, 'result')[0]
         community_data['rest_id'] = community_data['id_str']
         return Community(self, community_data)
 
     def _get_community_users(
         self, endpoint: str, community_id: str, count: int, cursor: str | None
     ):
@@ -4755,19 +4910,19 @@
             variables['cursor'] = cursor
         params = flatten_params({
             'variables': variables,
             'features': {
                 'responsive_web_graphql_timeline_navigation_enabled': True
             }
         })
-        response =  self.http.get(
+        response, _ = self.get(
             endpoint,
             params=params,
             headers=self._base_headers
-        ).json()
+        )
 
         items = find_dict(response, 'items_results')[0]
         users = []
         for item in items:
             if not 'result' in item:
                 continue
             if item['result'].get('__typename') != 'User':
@@ -4874,19 +5029,19 @@
         }
         if cursor is not None:
             variables['cursor'] = cursor
         params = flatten_params({
             'variables': variables,
             'features': COMMUNITY_TWEETS_FEATURES
         })
-        response = self.http.get(
+        response, _ = self.get(
             Endpoint.SEARCH_COMMUNITY_TWEET,
             params=params,
             headers=self._base_headers
-        ).json()
+        )
 
         items = find_dict(response, 'entries')[0]
         tweets = []
         for item in items:
             if not item['entryId'].startswith('tweet'):
                 continue
 
@@ -4908,18 +5063,18 @@
         )
 
     def _stream(self, topics: set[str]) -> Generator[tuple[str, Payload]]:
         headers = self._base_headers
         headers.pop('content-type')
         params = {'topics': ','.join(topics)}
 
-        with self.http.stream(
+        with self.stream(
             'GET', Endpoint.EVENTS, params=params, timeout=None
         ) as response:
-            self.http._remove_duplicate_ct0_cookie()
+            self._remove_duplicate_ct0_cookie()
             for line in response.iter_lines():
                 try:
                     data = json.loads(line)
                 except json.JSONDecodeError:
                     continue
                 payload = _payload_from_data(data['payload'])
                 yield data.get('topic'), payload
@@ -5013,14 +5168,14 @@
         data = urlencode({
             'sub_topics': ','.join(subscribe),
             'unsub_topics': ','.join(unsubscribe)
         })
         headers = self._base_headers
         headers['content-type'] = 'application/x-www-form-urlencoded'
         headers['LivePipeline-Session'] = session.id
-        response = self.http.post(
+        response, _ = self.post(
             Endpoint.UPDATE_SUBSCRIPTIONS, data=data, headers=headers
-        ).json()
+        )
         session.topics |= subscribe
         session.topics -= unsubscribe
 
         return _payload_from_data(response)
```

### Comparing `twikit-1.6.4/twikit/community.py` & `twikit-1.7.0/twikit/community.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.4/twikit/errors.py` & `twikit-1.7.0/twikit/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,19 @@
     """
 
 class UserUnavailable(TwitterException):
     """
     Exception raised when a user is unavailable.
     """
 
+class AccountSuspended(TwitterException):
+    """
+    Exception raised when the account is suspended.
+    """
+
 ERROR_CODE_TO_EXCEPTION: dict[int, TwitterException] = {
     187: DuplicateTweet,
     324: InvalidMedia
 }
 
 
 def raise_exceptions_from_response(errors: list[dict]):
```

### Comparing `twikit-1.6.4/twikit/geo.py` & `twikit-1.7.0/twikit/geo.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.4/twikit/group.py` & `twikit-1.7.0/twikit/group.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.4/twikit/list.py` & `twikit-1.7.0/twikit/list.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.4/twikit/message.py` & `twikit-1.7.0/twikit/message.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.4/twikit/notification.py` & `twikit-1.7.0/twikit/notification.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.4/twikit/streaming.py` & `twikit-1.7.0/twikit/streaming.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.4/twikit/trend.py` & `twikit-1.7.0/twikit/trend.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.4/twikit/tweet.py` & `twikit-1.7.0/twikit/tweet.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,18 +31,18 @@
         The full text of the tweet.
     lang : :class:`str`
         The language of the tweet.
     in_reply_to : :class:`str`
         The tweet ID this tweet is in reply to, if any
     is_quote_status : :class:`bool`
         Indicates if the tweet is a quote status.
-    quote : :class:`Tweet`
+    quote : :class:`Tweet` | None
         The Tweet being quoted (if any)
-    retweeted_tweet : :class:`bool`
-        Whether the tweet is a retweet
+    retweeted_tweet : :class:`Tweet` | None
+        The Tweet being retweeted (if any)
     possibly_sensitive : :class:`bool`
         Indicates if the tweet content may be sensitive.
     possibly_sensitive_editable : :class:`bool`
         Indicates if the tweet's sensitivity can be edited.
     quote_count : :class:`int`
         The count of quotes for the tweet.
     media : :class:`list`
@@ -700,8 +700,8 @@
     def __repr__(self) -> str:
         return f'<CommunityNote id="{self.id}">'
 
     def __eq__(self, __value: object) -> bool:
         return isinstance(__value, CommunityNote) and self.id == __value.id
 
     def __ne__(self, __value: object) -> bool:
-        return not self == __value
+        return not self == __value
```

### Comparing `twikit-1.6.4/twikit/twikit_async/__init__.py` & `twikit-1.7.0/twikit/twikit_async/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import asyncio
 import os
 
 if os.name == 'nt':
     asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
 
+from ._captcha import Capsolver
 from .bookmark import BookmarkFolder
 from ..errors import *
 from ..utils import build_query
 from .client import Client
 from .community import (Community, CommunityCreator, CommunityMember,
                         CommunityRule)
 from .geo import Place
```

### Comparing `twikit-1.6.4/twikit/twikit_async/bookmark.py` & `twikit-1.7.0/twikit/twikit_async/bookmark.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.4/twikit/twikit_async/client.py` & `twikit-1.7.0/twikit/twikit_async/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 from __future__ import annotations
 
 import asyncio
 import io
 import json
 import warnings
 from functools import partial
-from typing import AsyncGenerator, Literal
+from typing import Any, AsyncGenerator, Literal
 
 import filetype
-from fake_useragent import UserAgent
+import httpx
 from httpx import Response
 
 from ..errors import (
+    AccountSuspended,
+    BadRequest,
     CouldNotTweet,
+    Forbidden,
     InvalidMedia,
-    TwitterException,
+    NotFound,
+    RequestTimeout,
+    ServerError,
     TweetNotAvailable,
+    TwitterException,
+    TooManyRequests,
+    Unauthorized,
     UserNotFound,
     UserUnavailable,
     raise_exceptions_from_response
 )
 from ..utils import (
     BOOKMARK_FOLDER_TIMELINE_FEATURES,
     COMMUNITY_TWEETS_FEATURES,
@@ -36,68 +44,180 @@
     build_user_data,
     find_dict,
     flatten_params,
     get_query_id,
     urlencode
 )
 from .bookmark import BookmarkFolder
+from ._captcha import Capsolver
 from .community import (
     Community,
     CommunityMember
 )
 from .geo import Place, _places_from_response
 from .group import Group, GroupMessage
-from .http import HTTPClient
 from .list import List
 from .message import Message
 from .notification import Notification
 from .trend import Location, PlaceTrend, PlaceTrends, Trend
 from .streaming import Payload, StreamingSession, _payload_from_data
 from .tweet import CommunityNote, Poll, ScheduledTweet, Tweet, tweet_from_data
 from .user import User
 from .utils import Flow, Result
 
 
-class Client:
+class BaseClient:
+    """:meta private:"""
+
+    def __init__(
+        self,
+        language: str | None = None,
+        proxy: str | None = None,
+        captcha_solver: Capsolver | None = None,
+        **kwargs
+    ) -> None:
+        if 'proxies' in kwargs:
+            message = (
+                "The 'proxies' argument is now deprecated. Use 'proxy' "
+                "instead. https://github.com/encode/httpx/pull/2879"
+            )
+            warnings.warn(message)
+
+        self.http = httpx.AsyncClient(proxy=proxy, **kwargs)
+        self.language = language
+        self.proxy = proxy
+        self.captcha_solver = captcha_solver
+        if captcha_solver is not None:
+            captcha_solver.client = self
+
+        self._token = TOKEN
+        self._user_id = None
+        self._user_agent = ('Mozilla/5.0 (Windows NT 10.0; Win64; x64) '
+                            'AppleWebKit/537.36 (KHTML, like Gecko) '
+                            'Chrome/122.0.0.0 Safari/537.36')
+        self._act_as = None
+
+    async def request(
+        self,
+        method: str,
+        url: str,
+        auto_unlock: bool = True,
+        raise_exception: bool = True,
+        **kwargs
+    ) -> tuple[dict | Any, httpx.Response]:
+        cookies_backup = self.get_cookies().copy()
+        response = await self.http.request(method, url, **kwargs)
+        self._remove_duplicate_ct0_cookie()
+
+        try:
+            response_data = response.json()
+        except json.decoder.JSONDecodeError:
+            response_data = response.text
+
+        if isinstance(response_data, dict) and 'errors' in response_data:
+            error_code = response_data['errors'][0]['code']
+            error_message = response_data['errors'][0].get('message')
+            if error_code == 37:
+                # Account suspended
+                raise AccountSuspended(error_message)
+
+            if error_code == 326:
+                # Account unlocking
+                if self.captcha_solver is None:
+                    raise TwitterException(
+                        'Your account is locked. Visit '
+                        'https://twitter.com/account/access to unlock it.'
+                    )
+                if auto_unlock:
+                    await self.unlock()
+                    self.set_cookies(cookies_backup, clear_cookies=True)
+                    response = await self.http.request(method, url, **kwargs)
+                    self._remove_duplicate_ct0_cookie()
+                    try:
+                        response_data = response.json()
+                    except json.decoder.JSONDecodeError:
+                        response_data = response.text
+
+        status_code = response.status_code
+
+        if status_code >= 400 and raise_exception:
+            message = f'status: {status_code}, message: "{response.text}"'
+            if status_code == 400:
+                raise BadRequest(message, headers=response.headers)
+            elif status_code == 401:
+                raise Unauthorized(message, headers=response.headers)
+            elif status_code == 403:
+                raise Forbidden(message, headers=response.headers)
+            elif status_code == 404:
+                raise NotFound(message, headers=response.headers)
+            elif status_code == 408:
+                raise RequestTimeout(message, headers=response.headers)
+            elif status_code == 429:
+                raise TooManyRequests(message, headers=response.headers)
+            elif 500 <= status_code < 600:
+                raise ServerError(message, headers=response.headers)
+            else:
+                raise TwitterException(message, headers=response.headers)
+
+        return response_data, response
+
+    async def get(self, url, **kwargs) -> tuple[dict | Any, httpx.Response]:
+        return await self.request('GET', url, **kwargs)
+
+    async def post(self, url, **kwargs) -> tuple[dict | Any, httpx.Response]:
+        return await self.request('POST', url, **kwargs)
+
+    async def stream(self, *args, **kwargs) -> Response:
+        response = await self.http.stream(*args, **kwargs)
+        return response
+
+    def _remove_duplicate_ct0_cookie(self) -> None:
+        cookies = {}
+        for cookie in self.http.cookies.jar:
+            if 'ct0' in cookies and cookie.name == 'ct0':
+                continue
+            cookies[cookie.name] = cookie.value
+        self.http.cookies = list(cookies.items())
+
+
+class Client(BaseClient):
     """
     A client for interacting with the Twitter API.
     Since this class is for asynchronous use,
     methods must be executed using await.
 
+    Parameters
+    ----------
+    language : :class:`str` | None, default=None
+        The language code to use in API requests.
+    proxy : :class:`str` | None, default=None
+        The proxy server URL to use for request
+        (e.g., 'http://0.0.0.0:0000').
+    captcha_solver : :class:`.Capsolver` | None, default=None
+        See :class:`.Capsolver`.
+
     Examples
     --------
     >>> client = Client(language='en-US')
 
     >>> await client.login(
     ...     auth_info_1='example_user',
     ...     auth_info_2='email@example.com',
     ...     password='00000000'
     ... )
     """
-
-    def __init__(
-        self, language: str | None = None,
-        proxies: dict | None = None, **kwargs
-    ) -> None:
-        self._token = TOKEN
-        self.language = language
-        self.http = HTTPClient(proxies=proxies, **kwargs)
-        self._user_id = None
-        self._user_agent = UserAgent().random.strip()
-        self._act_as = None
-
     async def _get_guest_token(self) -> str:
         headers = self._base_headers
         headers.pop('X-Twitter-Active-User')
         headers.pop('X-Twitter-Auth-Type')
-        response = (await self.http.post(
+        response, _ = await self.post(
             Endpoint.GUEST_TOKEN,
             headers=headers,
             data={}
-        )).json()
+        )
         guest_token = response['guest_token']
         return guest_token
 
     @property
     def _base_headers(self) -> dict[str, str]:
         """
         Base headers for Twitter API requests.
@@ -128,15 +248,69 @@
         current session's cookies.
 
         Returns
         -------
         :class:`str`
             The CSRF token as a string.
         """
-        return self.http.client.cookies.get('ct0')
+        return self.http.cookies.get('ct0')
+
+    async def unlock(self) -> None:
+        if self.captcha_solver is None:
+            raise ValueError('Captcha solver is not provided.')
+
+        response, html = await self.captcha_solver.get_unlock_html()
+
+        if html.delete_button:
+            response, html = await self.captcha_solver.confirm_unlock(
+                html.authenticity_token,
+                html.assignment_token,
+                ui_metrics=True
+            )
+
+        if html.start_button or html.finish_button:
+            response, html = await self.captcha_solver.confirm_unlock(
+                html.authenticity_token,
+                html.assignment_token,
+                ui_metrics=True
+            )
+
+        cookies_backup = self.get_cookies().copy()
+        max_unlock_attempts = self.captcha_solver.max_attempts
+        attempt = 0
+        while attempt < max_unlock_attempts:
+            attempt += 1
+
+            if html.authenticity_token is None:
+                response, html = await self.captcha_solver.get_unlock_html()
+
+            result = self.captcha_solver.solve_funcaptcha(html.blob)
+            if result['errorId'] == 1:
+                continue
+
+            self.set_cookies(cookies_backup, clear_cookies=True)
+            response, html = await self.captcha_solver.confirm_unlock(
+                html.authenticity_token,
+                html.assignment_token,
+                result['solution']['token'],
+            )
+
+            if html.finish_button:
+                response, html = await self.captcha_solver.confirm_unlock(
+                    html.authenticity_token,
+                    html.assignment_token,
+                    ui_metrics=True
+                )
+            finished = (
+                response.next_request is not None and
+                response.next_request.url.path == '/'
+            )
+            if finished:
+                return
+        raise Exception('could not unlock the account.')
 
     async def login(
         self,
         *,
         auth_info_1: str,
         auth_info_2: str | None = None,
         password: str,
@@ -165,15 +339,15 @@
         --------
         >>> await client.login(
         ...     auth_info_1='example_user',
         ...     auth_info_2='email@example.com',
         ...     password='00000000'
         ... )
         """
-        self.http.client.cookies.clear()
+        self.http.cookies.clear()
         guest_token = await self._get_guest_token()
         headers = self._base_headers | {
             'x-guest-token': guest_token
         }
         headers.pop('X-Twitter-Active-User')
         headers.pop('X-Twitter-Auth-Type')
 
@@ -249,30 +423,30 @@
 
         return flow.response
 
     async def logout(self) -> Response:
         """
         Logs out of the currently logged-in account.
         """
-        response = await self.http.post(
+        response, _ = await self.post(
             Endpoint.LOGOUT,
             headers=self._base_headers
         )
         return response
 
     async def user_id(self) -> str:
         """
         Retrieves the user ID associated with the authenticated account.
         """
         if self._user_id is not None:
             return self._user_id
-        response = (await self.http.get(
+        response, _ = await self.get(
             Endpoint.SETTINGS,
             headers=self._base_headers
-        )).json()
+        )
         screen_name = response['screen_name']
         self._user_id = (await self.get_user_by_screen_name(screen_name)).id
         return self._user_id
 
     async def user(self) -> User:
         """
         Retrieve detailed information about the authenticated user.
@@ -291,15 +465,15 @@
 
         See Also
         --------
         .set_cookies
         .load_cookies
         .save_cookies
         """
-        return dict(self.http.client.cookies)
+        return dict(self.http.cookies)
 
     def save_cookies(self, path: str) -> None:
         """
         Save cookies to file in json format.
         You can skip the login procedure by loading the saved cookies
         using the :func:`load_cookies` method.
 
@@ -339,16 +513,16 @@
         See Also
         --------
         .get_cookies
         .load_cookies
         .save_cookies
         """
         if clear_cookies:
-            self.http.client.cookies.clear()
-        self.http.client.cookies.update(cookies)
+            self.http.cookies.clear()
+        self.http.cookies.update(cookies)
 
     def load_cookies(self, path: str) -> None:
         """
         Loads cookies from a file.
         You can skip the login procedure by loading a saved cookies.
 
         Parameters
@@ -399,19 +573,19 @@
         }
         if cursor is not None:
             variables['cursor'] = cursor
         params = flatten_params({
             'variables': variables,
             'features': FEATURES
         })
-        response = (await self.http.get(
+        response, _ = await self.get(
             Endpoint.SEARCH_TIMELINE,
             params=params,
             headers=self._base_headers
-        )).json()
+        )
 
         return response
 
     async def search_tweet(
         self,
         query: str,
         product: Literal['Top', 'Latest', 'Media'],
@@ -592,19 +766,19 @@
             A list of Tweet objects representing tweets
             similar to the specified tweet.
         """
         params = flatten_params({
             'variables': {'tweet_id': tweet_id},
             'features': SIMILAR_POSTS_FEATURES
         })
-        response = (await self.http.get(
+        response, _ = await self.get(
             Endpoint.SIMILAR_POSTS,
             params=params,
             headers=self._base_headers
-        )).json()
+        )
         items_ = find_dict(response, 'entries')
         results = []
         if not items_:
             return results
 
         for item in items_[0]:
             if not item['entryId'].startswith('tweet'):
@@ -711,19 +885,19 @@
         params = {
             'command': 'INIT',
             'total_bytes': total_bytes,
             'media_type': media_type
         }
         if media_category is not None:
             params['media_category'] = media_category
-        response = (await self.http.post(
+        response, _ = await self.post(
             endpoint,
             params=params,
             headers=self._base_headers
-        )).json()
+        )
         media_id = response['media_id']
         # =========== APPEND ============
         segment_index = 0
         bytes_sent = 0
         MAX_SEGMENT_SIZE = 8 * 1024 * 1024  # The maximum segment size is 8 MB
         tasks = []
         chunk_streams: list[io.BytesIO] = []
@@ -742,15 +916,15 @@
                 'media': (
                     'blob',
                     chunk_stream,
                     'application/octet-stream',
                 )
             }
 
-            coro = self.http.post(
+            coro = self.post(
                 endpoint,
                 params=params,
                 headers=headers,
                 files=files
             )
             tasks.append(asyncio.create_task(coro))
             chunk_streams.append(chunk_stream)
@@ -766,15 +940,15 @@
             chunk_stream.close()
 
         # ========== FINALIZE ===========
         params = {
             'command': 'FINALIZE',
             'media_id': media_id,
         }
-        await self.http.post(
+        await self.post(
             endpoint,
             params=params,
             headers=self._base_headers,
         )
 
         if wait_for_completion:
             while True:
@@ -809,19 +983,19 @@
             'command': 'STATUS',
             'media_id': media_id
         }
         if is_long_video:
             endpoint = Endpoint.UPLOAD_MEDIA_2
         else:
             endpoint = Endpoint.UPLOAD_MEDIA
-        response = (await self.http.get(
+        response, _ = await self.get(
             endpoint,
             params=params,
             headers=self._base_headers
-        )).json()
+        )
         return response
 
     async def create_media_metadata(
         self,
         media_id: str,
         alt_text: str | None = None,
         sensitive_warning: list[
@@ -855,29 +1029,20 @@
         >>> await client.create_tweet(media_ids=[media_id])
         """
         data = {'media_id': media_id}
         if alt_text is not None:
             data['alt_text'] = {'text': alt_text}
         if sensitive_warning is not None:
             data['sensitive_media_warning'] = sensitive_warning
-        return await self.http.post(
+        _, response = await self.post(
             Endpoint.CREATE_MEDIA_METADATA,
             json=data,
             headers=self._base_headers
         )
-
-    async def get_media(self, url: str) -> bytes:
-        """Retrieves media bytes.
-
-        Parameters
-        ----------
-        url : str
-            Media URL
-        """
-        return (await self.http.get(url, headers=self._base_headers)).content
+        return response
 
     async def create_poll(
         self,
         choices: list[str],
         duration_minutes: int
     ) -> str:
         """
@@ -916,19 +1081,19 @@
 
         data = urlencode(
             {'card_data': card_data}
         )
         headers = self._base_headers | {
             'content-type': 'application/x-www-form-urlencoded'
         }
-        response = (await self.http.post(
+        response, _ = await self.post(
             Endpoint.CREATE_CARD,
             data=data,
             headers=headers,
-        )).json()
+        )
 
         return response['card_uri']
 
     async def vote(
         self,
         selected_choice: str,
         card_uri: str,
@@ -958,19 +1123,19 @@
             'twitter:string:response_card_name': card_name,
             'twitter:string:cards_platform': 'Web-12',
             'twitter:string:selected_choice': selected_choice
         })
         headers = self._base_headers | {
             'content-type': 'application/x-www-form-urlencoded'
         }
-        response = (await self.http.post(
+        response, _ = await self.post(
             Endpoint.VOTE,
             data=data,
             headers=headers
-        )).json()
+        )
 
         card_data = {
             'rest_id': response['card']['url'],
             'legacy': response['card']
         }
         return Poll(self, card_data, None)
 
@@ -1121,19 +1286,19 @@
             endpoint = Endpoint.CREATE_TWEET
             features = FEATURES
         data = {
             'variables': variables,
             'queryId': get_query_id(Endpoint.CREATE_TWEET),
             'features': features,
         }
-        response = (await self.http.post(
+        response, _ = await self.post(
             endpoint,
             json=data,
             headers=self._base_headers,
-        )).json()
+        )
 
         _result = find_dict(response, 'result')
         if not _result:
             raise_exceptions_from_response(response['errors'])
             raise CouldNotTweet(
                 response['errors'][0]
                 if response['errors']
@@ -1192,19 +1357,19 @@
             },
             'execute_at': scheduled_at
         }
         data = {
             'variables': variables,
             'queryId': get_query_id(Endpoint.CREATE_SCHEDULED_TWEET),
         }
-        response = (await self.http.post(
+        response, _ = await self.post(
             Endpoint.CREATE_SCHEDULED_TWEET,
             json=data,
             headers=self._base_headers,
-        )).json()
+        )
         return response['data']['tweet']['rest_id']
 
     async def delete_tweet(self, tweet_id: str) -> Response:
         """Deletes a tweet.
 
         Parameters
         ----------
@@ -1224,15 +1389,15 @@
         data = {
             'variables': {
                 'tweet_id': tweet_id,
                 'dark_request': False
             },
             'queryId': get_query_id(Endpoint.DELETE_TWEET)
         }
-        response = await self.http.post(
+        _, response = await self.post(
             Endpoint.DELETE_TWEET,
             json=data,
             headers=self._base_headers
         )
         return response
 
     async def get_user_by_screen_name(self, screen_name: str) -> User:
@@ -1262,19 +1427,19 @@
             'withSafetyModeUserFields': False
         }
         params = flatten_params({
             'variables': variables,
             'features': USER_FEATURES,
             'fieldToggles': {'withAuxiliaryUserLabels': False}
         })
-        response = (await self.http.get(
+        response, _ = await self.get(
             Endpoint.USER_BY_SCREEN_NAME,
             params=params,
             headers=self._base_headers
-        )).json()
+        )
 
         if 'user' not in response['data']:
             raise UserNotFound('The user does not exist.')
         user_data = response['data']['user']['result']
         if user_data.get('__typename') == 'UserUnavailable':
             raise UserUnavailable(user_data.get('message'))
 
@@ -1306,19 +1471,19 @@
             'userId': user_id,
             'withSafetyModeUserFields': True
         }
         params = flatten_params({
             'variables': variables,
             'features': USER_FEATURES
         })
-        response = (await self.http.get(
+        response, _ = await self.get(
             Endpoint.USER_BY_REST_ID,
             params=params,
             headers=self._base_headers
-        )).json()
+        )
         if 'result' not in response['data']['user']:
             raise TwitterException(f'Invalid user id: {user_id}')
         user_data = response['data']['user']['result']
         if user_data.get('__typename') == 'UserUnavailable':
             raise UserUnavailable(user_data.get('message'))
         return User(self, user_data)
 
@@ -1354,19 +1519,19 @@
             'granularity': granularity,
             'max_results': max_results
         }
         for k, v in tuple(params.items()):
             if v is None:
                 params.pop(k)
 
-        response = (await self.http.get(
+        response, _ = await self.get(
             Endpoint.REVERSE_GEOCODE,
             params=params,
             headers=self._base_headers
-        )).json()
+        )
         return _places_from_response(self, response)
 
     async def search_geo(
         self, lat: float | None = None, long: float | None = None,
         query: str | None = None, ip: str | None = None,
         granularity: str | None = None, max_results: int | None = None
     ) -> list[Place]:
@@ -1405,36 +1570,36 @@
             'granularity': granularity,
             'max_results': max_results
         }
         for k, v in tuple(params.items()):
             if v is None:
                 params.pop(k)
 
-        response = (await self.http.get(
+        response, _ = await self.get(
             Endpoint.SEARCH_GEO,
             params=params,
             headers=self._base_headers
-        )).json()
+        )
         return _places_from_response(self, response)
 
     async def get_place(self, id: str) -> Place:
         """
         Parameters
         ----------
         id : :class:`str`
             The ID of the place.
 
         Returns
         -------
         :class:`.Place`
         """
-        response = (await self.http.get(
+        response, _ = await self.get(
             Endpoint.PLACE_BY_ID.format(id),
             headers=self._base_headers
-        )).json()
+        )
         return Place(self, response)
 
     async def _get_tweet_detail(self, tweet_id: str, cursor: str | None):
         variables = {
             'focalTweetId': tweet_id,
             'with_rux_injections': False,
             'includePromotedContent': True,
@@ -1447,19 +1612,19 @@
         if cursor is not None:
             variables['cursor'] = cursor
         params = flatten_params({
             'variables': variables,
             'features': FEATURES,
             'fieldToggles': {'withAuxiliaryUserLabels': False}
         })
-        response = (await self.http.get(
+        response, _ = await self.get(
             Endpoint.TWEET_DETAIL,
             params=params,
             headers=self._base_headers
-        )).json()
+        )
         return response
 
     async def _get_more_replies(
         self, tweet_id: str, cursor: str
     ) -> Result[Tweet]:
         response = await self._get_tweet_detail(tweet_id, cursor)
         entries = find_dict(response, 'entries')[0]
@@ -1609,19 +1774,19 @@
         list[:class:`ScheduledTweet`]
             List of ScheduledTweet objects representing the scheduled tweets.
         """
 
         params = flatten_params({
             'variables': {'ascending': True}
         })
-        response = (await self.http.get(
+        response, _ = await self.get(
             Endpoint.FETCH_SCHEDULED_TWEETS,
             params=params,
             headers=self._base_headers
-        )).json()
+        )
         tweets = find_dict(response, 'scheduled_tweet_list')[0]
         return [ScheduledTweet(self, tweet) for tweet in tweets]
 
     async def delete_scheduled_tweet(self, tweet_id: str) -> Response:
         """
         Delete a scheduled tweet.
 
@@ -1637,15 +1802,15 @@
         """
         data = {
             'variables': {
                 'scheduled_tweet_id': tweet_id
             },
             'queryId': get_query_id(Endpoint.DELETE_SCHEDULED_TWEET)
         }
-        response = await self.http.post(
+        _, response = await self.post(
             Endpoint.DELETE_SCHEDULED_TWEET,
             json=data,
             headers=self._base_headers
         )
         return response
 
     async def _get_tweet_engagements(
@@ -1661,19 +1826,19 @@
         }
         if cursor is not None:
             variables['cursor'] = cursor
         params = flatten_params({
             'variables': variables,
             'features': FEATURES
         })
-        response = (await self.http.get(
+        response, _ = await self.get(
             endpoint,
             params=params,
             headers=self._base_headers
-        )).json()
+        )
         items_ = find_dict(response, 'entries')
         if not items_:
             return Result([])
         items = items_[0]
         next_cursor = items[-1]['content']['value']
         previous_cursor = items[-2]['content']['value']
 
@@ -1795,19 +1960,19 @@
         >>> print(note)
         <CommunityNote id="...">
         """
         params = flatten_params({
             'variables': {'note_id': note_id},
             'features': COMMUNITY_NOTE_FEATURES
         })
-        response = (await self.http.get(
+        response, _ = await self.get(
             Endpoint.FETCH_COMMUNITY_NOTE,
             params=params,
             headers=self._base_headers
-        )).json()
+        )
         note_data = response['data']['birdwatch_note_by_rest_id']
         if 'data_v1' not in note_data:
             raise TwitterException(f'Invalid user id: {note_id}')
         return CommunityNote(
             self, note_data
         )
 
@@ -1891,19 +2056,19 @@
         endpoint = {
             'Tweets': Endpoint.USER_TWEETS,
             'Replies': Endpoint.USER_TWEETS_AND_REPLIES,
             'Media': Endpoint.USER_MEDIA,
             'Likes': Endpoint.USER_LIKES,
         }[tweet_type]
 
-        response = (await self.http.get(
+        response, _ = await self.get(
             endpoint,
             params=params,
             headers=self._base_headers
-        )).json()
+        )
 
         instructions_ = find_dict(response, 'instructions')
         if not instructions_:
             return Result([])
         instructions = instructions_[0]
 
         items = instructions[-1]['entries']
@@ -2006,19 +2171,19 @@
             variables['cursor'] = cursor
 
         data = {
             'variables': variables,
             'queryId': get_query_id(Endpoint.HOME_TIMELINE),
             'features': FEATURES,
         }
-        response = (await self.http.post(
+        response, _ = await self.post(
             Endpoint.HOME_TIMELINE,
             json=data,
             headers=self._base_headers
-        )).json()
+        )
 
         items = find_dict(response, 'entries')[0]
         next_cursor = items[-1]['content']['value']
         results = []
 
         for item in items:
             if 'itemContent' not in item['content']:
@@ -2087,19 +2252,19 @@
             variables['cursor'] = cursor
 
         data = {
             'variables': variables,
             'queryId': get_query_id(Endpoint.HOME_LATEST_TIMELINE),
             'features': FEATURES,
         }
-        response = (await self.http.post(
+        response, _ = await self.post(
             Endpoint.HOME_LATEST_TIMELINE,
             json=data,
             headers=self._base_headers
-        )).json()
+        )
 
         items = find_dict(response, 'entries')[0]
         next_cursor = items[-1]['content']['value']
         results = []
 
         for item in items:
             if 'itemContent' not in item['content']:
@@ -2139,15 +2304,15 @@
         --------
         .unfavorite_tweet
         """
         data = {
             'variables': {'tweet_id': tweet_id},
             'queryId': get_query_id(Endpoint.FAVORITE_TWEET)
         }
-        response = await self.http.post(
+        _, response = await self.post(
             Endpoint.FAVORITE_TWEET,
             json=data,
             headers=self._base_headers
         )
         return response
 
     async def unfavorite_tweet(self, tweet_id: str) -> Response:
@@ -2173,15 +2338,15 @@
         --------
         .favorite_tweet
         """
         data = {
             'variables': {'tweet_id': tweet_id},
             'queryId': get_query_id(Endpoint.UNFAVORITE_TWEET)
         }
-        response = await self.http.post(
+        _, response = await self.post(
             Endpoint.UNFAVORITE_TWEET,
             json=data,
             headers=self._base_headers
         )
         return response
 
     async def retweet(self, tweet_id: str) -> Response:
@@ -2207,15 +2372,15 @@
         --------
         .delete_retweet
         """
         data = {
             'variables': {'tweet_id': tweet_id, 'dark_request': False},
             'queryId': get_query_id(Endpoint.CREATE_RETWEET)
         }
-        response = await self.http.post(
+        _, response = await self.post(
             Endpoint.CREATE_RETWEET,
             json=data,
             headers=self._base_headers
         )
         return response
 
     async def delete_retweet(self, tweet_id: str) -> Response:
@@ -2241,15 +2406,15 @@
         --------
         .retweet
         """
         data = {
             'variables': {'source_tweet_id': tweet_id,'dark_request': False},
             'queryId': get_query_id(Endpoint.DELETE_RETWEET)
         }
-        response = await self.http.post(
+        _, response = await self.post(
             Endpoint.DELETE_RETWEET,
             json=data,
             headers=self._base_headers
         )
         return response
 
     async def bookmark_tweet(
@@ -2282,15 +2447,15 @@
             endpoint = Endpoint.BOOKMARK_TO_FOLDER
             variables['bookmark_collection_id'] = folder_id
 
         data = {
             'variables': variables,
             'queryId': get_query_id(Endpoint.CREATE_BOOKMARK)
         }
-        response = await self.http.post(
+        _, response = await self.post(
             endpoint,
             json=data,
             headers=self._base_headers
         )
         return response
 
     async def delete_bookmark(self, tweet_id: str) -> Response:
@@ -2316,15 +2481,15 @@
         --------
         .bookmark_tweet
         """
         data = {
             'variables': {'tweet_id': tweet_id},
             'queryId': get_query_id(Endpoint.DELETE_BOOKMARK)
         }
-        response = await self.http.post(
+        _, response = await self.post(
             Endpoint.DELETE_BOOKMARK,
             json=data,
             headers=self._base_headers
         )
         return response
 
     async def get_bookmarks(
@@ -2378,19 +2543,19 @@
 
         if cursor is not None:
             variables['cursor'] = cursor
         params = flatten_params({
             'variables': variables,
             'features': features
         })
-        response = (await self.http.get(
+        response, _ = await self.get(
             endpoint,
             params=params,
             headers=self._base_headers
-        )).json()
+        )
 
         items_ = find_dict(response, 'entries')
         if not items_:
             return Result([])
         items = items_[0]
         next_cursor = items[-1]['content']['value']
         if folder_id is None:
@@ -2429,15 +2594,15 @@
         --------
         >>> await client.delete_all_bookmarks()
         """
         data = {
             'variables': {},
             'queryId': get_query_id(Endpoint.BOOKMARKS_ALL_DELETE)
         }
-        response = await self.http.post(
+        _, response = await self.post(
             Endpoint.BOOKMARKS_ALL_DELETE,
             json=data,
             headers=self._base_headers
         )
         return response
 
     async def get_bookmark_folders(
@@ -2458,19 +2623,19 @@
         [<BookmarkFolder id="...">, ..., <BookmarkFolder id="...">]
         >>> more_folders = await folders.next()  # Retrieve more folders
         """
         variables = {}
         if cursor is not None:
             variables['cursor'] = cursor
         params = flatten_params({'variables': variables})
-        response = (await self.http.get(
+        response, _ = await self.get(
             Endpoint.BOOKMARK_FOLDERS,
             params=params,
             headers=self._base_headers
-        )).json()
+        )
 
         slice = find_dict(response, 'bookmark_collections_slice')[0]
         results = []
         for item in slice['items']:
             results.append(BookmarkFolder(self, item))
 
         if 'next_cursor' in slice['slice_info']:
@@ -2512,19 +2677,19 @@
             'bookmark_collection_id': folder_id,
             'name': name
         }
         data = {
             'variables': variables,
             'queryId': get_query_id(Endpoint.EDIT_BOOKMARK_FOLDER)
         }
-        response = (await self.http.post(
+        response, _ = await self.post(
             Endpoint.EDIT_BOOKMARK_FOLDER,
             json=data,
             headers=self._base_headers
-        )).json()
+        )
         return BookmarkFolder(
             self, response['data']['bookmark_collection_update']
         )
 
     async def delete_bookmark_folder(self, folder_id: str) -> Response:
         """
         Deletes a bookmark folder.
@@ -2542,15 +2707,15 @@
         variables = {
             'bookmark_collection_id': folder_id
         }
         data = {
             'variables': variables,
             'queryId': get_query_id(Endpoint.DELETE_BOOKMARK_FOLDER)
         }
-        response = await self.http.post(
+        _, response = await self.post(
             Endpoint.DELETE_BOOKMARK_FOLDER,
             json=data,
             headers=self._base_headers
         )
         return response
 
     async def create_bookmark_folder(self, name: str) -> BookmarkFolder:
@@ -2569,19 +2734,19 @@
         variables = {
             'name': name
         }
         data = {
             'variables': variables,
             'queryId': get_query_id(Endpoint.CREATE_BOOKMARK_FOLDER)
         }
-        response = (await self.http.post(
+        response, _ = await self.post(
             Endpoint.CREATE_BOOKMARK_FOLDER,
             json=data,
             headers=self._base_headers
-        )).json()
+        )
         return BookmarkFolder(
             self, response['data']['bookmark_collection_create']
         )
 
     async def follow_user(self, user_id: str) -> Response:
         """
         Follows a user.
@@ -2619,15 +2784,15 @@
             'include_ext_profile_image_shape': 1,
             'skip_status': 1,
             'user_id': user_id
         })
         headers = self._base_headers | {
             'content-type': 'application/x-www-form-urlencoded'
         }
-        response = await self.http.post(
+        _, response = await self.post(
             Endpoint.CREATE_FRIENDSHIPS,
             data=data,
             headers=headers
         )
         return response
 
     async def unfollow_user(self, user_id: str) -> Response:
@@ -2667,15 +2832,15 @@
             'include_ext_profile_image_shape': 1,
             'skip_status': 1,
             'user_id': user_id
         })
         headers = self._base_headers | {
             'content-type': 'application/x-www-form-urlencoded'
         }
-        response = await self.http.post(
+        _, response = await self.post(
             Endpoint.DESTROY_FRIENDSHIPS,
             data=data,
             headers=headers
         )
         return response
 
     async def block_user(self, user_id: str) -> Response:
@@ -2695,15 +2860,15 @@
         See Also
         --------
         .unblock_user
         """
         data = urlencode({'user_id': user_id})
         headers = self._base_headers
         headers['content-type'] = 'application/x-www-form-urlencoded'
-        response = await self.http.post(
+        _, response = await self.post(
             Endpoint.BLOCK_USER,
             data=data,
             headers=headers
         )
         return response
 
     async def unblock_user(self, user_id: str) -> Response:
@@ -2723,15 +2888,15 @@
         See Also
         --------
         .block_user
         """
         data = urlencode({'user_id': user_id})
         headers = self._base_headers
         headers['content-type'] = 'application/x-www-form-urlencoded'
-        response = await self.http.post(
+        _, response = await self.post(
             Endpoint.UNBLOCK_USER,
             data=data,
             headers=headers
         )
         return response
 
     async def mute_user(self, user_id: str) -> Response:
@@ -2751,15 +2916,15 @@
         See Also
         --------
         .unmute_user
         """
         data = urlencode({'user_id': user_id})
         headers = self._base_headers
         headers['content-type'] = 'application/x-www-form-urlencoded'
-        response = await self.http.post(
+        _, response = await self.post(
             Endpoint.MUTE_USER,
             data=data,
             headers=headers
         )
         return response
 
     async def unmute_user(self, user_id: str) -> Response:
@@ -2779,15 +2944,15 @@
         See Also
         --------
         .mute_user
         """
         data = urlencode({'user_id': user_id})
         headers = self._base_headers
         headers['content-type'] = 'application/x-www-form-urlencoded'
-        response = await self.http.post(
+        _, response = await self.post(
             Endpoint.UNMUTE_USER,
             data=data,
             headers=headers
         )
         return response
 
     async def get_trends(
@@ -2841,19 +3006,19 @@
         params = {
             'count': count,
             'include_page_configuration': True,
             'initial_tab_id': category
         }
         if additional_request_params is not None:
             params |= additional_request_params
-        response = (await self.http.get(
+        response, _ = await self.get(
             Endpoint.TREND,
             params=params,
             headers=self._base_headers
-        )).json()
+        )
 
         entry_id_prefix = 'trends' if category == 'trending' else 'Guide'
         entries = [
             i for i in find_dict(response, 'entries')[0]
             if i['entryId'].startswith(entry_id_prefix)
         ]
 
@@ -2879,31 +3044,31 @@
         """
         Retrieves locations where trends can be retrieved.
 
         Returns
         -------
         list[:class:`.Location`]
         """
-        response = (await self.http.get(
+        response, _ = await self.get(
             Endpoint.AVAILABLE_LOCATIONS,
             headers=self._base_headers
-        )).json()
+        )
         return [Location(self, data) for data in response]
 
     async def get_place_trends(self, woeid: int) -> PlaceTrends:
         """
         Retrieves the top 50 trending topics for a specific id.
         You can get available woeid using
         :attr:`.Client.get_available_locations`.
         """
-        response = (await self.http.get(
+        response, _ = await self.get(
             Endpoint.PLACE_TRENDS,
             params={'id': woeid},
             headers=self._base_headers
-        )).json()
+        )
         trend_data = response[0]
         trends = [PlaceTrend(self, data) for data in trend_data['trends']]
         trend_data['trends'] = trends
         return trend_data
 
     async def _get_user_friendship(
         self,
@@ -2922,19 +3087,19 @@
         }
         if cursor is not None:
             variables['cursor'] = cursor
         params = flatten_params({
             'variables': variables,
             'features': FEATURES
         })
-        response = (await self.http.get(
+        response, _ = await self.get(
             endpoint,
             params=params,
             headers=self._base_headers
-        )).json()
+        )
 
         items = find_dict(response, 'entries')[0]
         results = []
         for item in items:
             entry_id = item['entryId']
             if entry_id.startswith('user'):
                 user_info = find_dict(item, 'result')
@@ -2967,19 +3132,19 @@
             params['user_id'] = user_id
         elif user_id is not None:
             params['screen_name'] = screen_name
 
         if cursor is not None:
             params['cursor'] = cursor
 
-        response = (await self.http.get(
+        response, _ = await self.get(
             endpoint,
             params=params,
             headers=self._base_headers
-        )).json()
+        )
 
         users = response['users']
         results = []
         for user in users:
             results.append(User(self, build_user_data(user)))
 
         previous_cursor = response['previous_cursor']
@@ -3165,19 +3330,19 @@
             params['user_id'] = user_id
         elif user_id is not None:
             params['screen_name'] = screen_name
 
         if cursor is not None:
             params['cursor'] = cursor
 
-        response = (await self.http.get(
+        response, _ = await self.get(
             endpoint,
             params=params,
             headers=self._base_headers
-        )).json()
+        )
         previous_cursor = response['previous_cursor']
         next_cursor = response['next_cursor']
 
         return Result(
             response['ids'],
             partial(self._get_friendship_ids, user_id,
                      screen_name, count, endpoint, next_cursor),
@@ -3271,19 +3436,20 @@
             'text': text
         }
         if media_id is not None:
             data['media_id'] = media_id
         if reply_to is not None:
             data['reply_to_dm_id'] = reply_to
 
-        return (await self.http.post(
+        response, _ = await self.post(
             Endpoint.SEND_DM,
             json=data,
             headers=self._base_headers
-        )).json()
+        )
+        return response
 
     async def _get_dm_history(
         self,
         conversation_id: str,
         max_id: str | None = None
     ) -> dict:
         """
@@ -3291,19 +3457,20 @@
         """
         params = {
             'context': 'FETCH_DM_CONVERSATION_HISTORY'
         }
         if max_id is not None:
             params['max_id'] = max_id
 
-        return (await self.http.get(
+        response, _ = await self.get(
             Endpoint.CONVERSATION.format(conversation_id),
             params=params,
             headers=self._base_headers
-        )).json()
+        )
+        return response
 
     async def send_dm(
         self,
         user_id: str,
         text: str,
         media_id: str | None = None,
         reply_to: str | None = None
@@ -3391,15 +3558,15 @@
             'reactionTypes': ['Emoji'],
             'emojiReactions': [emoji]
         }
         data = {
             'variables': variables,
             'queryId': get_query_id(Endpoint.MESSAGE_ADD_REACTION)
         }
-        response = await self.http.post(
+        _, response = await self.post(
             Endpoint.MESSAGE_ADD_REACTION,
             json=data,
             headers=self._base_headers
         )
         return response
 
     async def remove_reaction_from_message(
@@ -3437,15 +3604,15 @@
             'reactionTypes': ['Emoji'],
             'emojiReactions': [emoji]
         }
         data = {
             'variables': variables,
             'queryId': get_query_id(Endpoint.MESSAGE_REMOVE_REACTION)
         }
-        response = await self.http.post(
+        _, response = await self.post(
             Endpoint.MESSAGE_REMOVE_REACTION,
             json=data,
             headers=self._base_headers
         )
         return response
 
     async def delete_dm(self, message_id: str) -> Response:
@@ -3469,15 +3636,15 @@
 
         data = {
             'variables': {
                 'messageId': message_id
             },
             'queryId': get_query_id(Endpoint.DELETE_DM)
         }
-        response = await self.http.post(
+        _, response = await self.post(
             Endpoint.DELETE_DM,
             json=data,
             headers=self._base_headers
         )
         return response
 
     async def get_dm_history(
@@ -3672,19 +3839,19 @@
         :class:`Group`
             An object representing the retrieved group.
         """
         params = {
             'context': 'FETCH_DM_CONVERSATION_HISTORY',
             'include_conversation_info': True,
         }
-        response = (await self.http.get(
+        response, _ = await self.get(
             Endpoint.CONVERSATION.format(group_id),
             params=params,
             headers=self._base_headers
-        )).json()
+        )
         return Group(self, group_id, response)
 
     async def add_members_to_group(
         self, group_id: str, user_ids: list[str]
     ) -> Response:
         """Adds members to a group.
 
@@ -3709,15 +3876,15 @@
         data = {
             'variables': {
                 'addedParticipants': user_ids,
                 'conversationId': group_id
             },
             'queryId': get_query_id(Endpoint.ADD_MEMBER_TO_GROUP)
         }
-        response = await self.http.post(
+        _, response = await self.post(
             Endpoint.ADD_MEMBER_TO_GROUP,
             json=data,
             headers=self._base_headers
         )
         return response
 
     async def change_group_name(self, group_id: str, name: str) -> Response:
@@ -3736,15 +3903,15 @@
             Response returned from twitter api.
         """
         data = urlencode({
             'name': name
         })
         headers = self._base_headers
         headers['content-type'] = 'application/x-www-form-urlencoded'
-        response = await self.http.post(
+        _, response = await self.post(
             Endpoint.CHANGE_GROUP_NAME.format(group_id),
             data=data,
             headers=headers
         )
         return response
 
     async def create_list(
@@ -3783,19 +3950,19 @@
             'description': description
         }
         data = {
             'variables': variables,
             'features': LIST_FEATURES,
             'queryId': get_query_id(Endpoint.CREATE_LIST)
         }
-        response = (await self.http.post(
+        response, _ = await self.post(
             Endpoint.CREATE_LIST,
             json=data,
             headers=self._base_headers
-        )).json()
+        )
         list_info = find_dict(response, 'list')[0]
         return List(self, list_info)
 
     async def edit_list_banner(self, list_id: str, media_id: str) -> Response:
         """
         Edit the banner image of a list.
 
@@ -3822,15 +3989,15 @@
             'mediaId': media_id
         }
         data = {
             'variables': variables,
             'features': LIST_FEATURES,
             'queryId': get_query_id(Endpoint.EDIT_LIST_BANNER)
         }
-        response = await self.http.post(
+        _, response = await self.post(
             Endpoint.EDIT_LIST_BANNER,
             json=data,
             headers=self._base_headers
         )
         return response
 
     async def delete_list_banner(self, list_id: str) -> Response:
@@ -3849,15 +4016,15 @@
         data = {
             'variables': {
                 'listId': list_id
             },
             'features': LIST_FEATURES,
             'queryId': get_query_id(Endpoint.DELETE_LIST_BANNER)
         }
-        response = await self.http.post(
+        _, response = await self.post(
             Endpoint.DELETE_LIST_BANNER,
             json=data,
             headers=self._base_headers
         )
         return response
 
     async def edit_list(
@@ -3903,19 +4070,19 @@
         if is_private is not None:
             variables['isPrivate'] = is_private
         data = {
             'variables': variables,
             'features': LIST_FEATURES,
             'queryId': get_query_id(Endpoint.UPDATE_LIST)
         }
-        response = (await self.http.post(
+        response, _ = await self.post(
             Endpoint.UPDATE_LIST,
             json=data,
             headers=self._base_headers
-        )).json()
+        )
         list_info = find_dict(response, 'list')[0]
         return List(self, list_info)
 
     async def add_list_member(self, list_id: str, user_id: str) -> Response:
         """
         Adds a user to a list.
 
@@ -3940,15 +4107,15 @@
             'userId': user_id
         }
         data = {
             'variables': variables,
             'features': LIST_FEATURES,
             'queryId': get_query_id(Endpoint.LIST_ADD_MEMBER)
         }
-        response = await self.http.post(
+        _, response = await self.post(
             Endpoint.LIST_ADD_MEMBER,
             json=data,
             headers=self._base_headers
         )
         return response
 
     async def remove_list_member(self, list_id: str, user_id: str) -> Response:
@@ -3976,15 +4143,15 @@
             'userId': user_id
         }
         data = {
             'variables': variables,
             'features': LIST_FEATURES,
             'queryId': get_query_id(Endpoint.LIST_REMOVE_MEMBER)
         }
-        response = await self.http.post(
+        _, response = await self.post(
             Endpoint.LIST_REMOVE_MEMBER,
             json=data,
             headers=self._base_headers
         )
         return response
 
     async def get_lists(
@@ -4019,19 +4186,19 @@
         }
         if cursor is not None:
             variables['cursor'] = cursor
         params = flatten_params({
             'variables': variables,
             'features': FEATURES
         })
-        response = (await self.http.get(
+        response, _ = await self.get(
             Endpoint.LIST_MANAGEMENT,
             params=params,
             headers=self._base_headers
-        )).json()
+        )
 
         entries = find_dict(response, 'entries')[0]
         items = find_dict(entries, 'items')
 
         if len(items) < 2:
             return Result([])
 
@@ -4063,19 +4230,19 @@
         :class:`List`
             List object.
         """
         params = flatten_params({
             'variables': {'listId': list_id},
             'features': LIST_FEATURES
         })
-        response = (await self.http.get(
+        response, _ = await self.get(
             Endpoint.LIST_BY_REST_ID,
             params=params,
             headers=self._base_headers
-        )).json()
+        )
         list_info = find_dict(response, 'list')[0]
         return List(self, list_info)
 
     async def get_list_tweets(
         self, list_id: str, count: int = 20, cursor: str | None = None
     ) -> Result[Tweet]:
         """
@@ -4119,19 +4286,19 @@
         }
         if cursor is not None:
             variables['cursor'] = cursor
         params = flatten_params({
             'variables': variables,
             'features': FEATURES
         })
-        response = (await self.http.get(
+        response, _ = await self.get(
             Endpoint.LIST_LATEST_TWEETS,
             params=params,
             headers=self._base_headers
-        )).json()
+        )
 
         items = find_dict(response, 'entries')[0]
         next_cursor = items[-1]['content']['value']
 
         results = []
         for item in items:
             if not item['entryId'].startswith('tweet'):
@@ -4159,19 +4326,19 @@
         }
         if cursor is not None:
             variables['cursor'] = cursor
         params = flatten_params({
             'variables': variables,
             'features': FEATURES
         })
-        response = (await self.http.get(
+        response, _ = await self.get(
             endpoint,
             params=params,
             headers=self._base_headers
-        )).json()
+        )
 
         items = find_dict(response, 'entries')[0]
         results = []
         for item in items:
             entry_id = item['entryId']
             if entry_id.startswith('user'):
                 user_info = find_dict(item, 'result')[0]
@@ -4357,19 +4524,19 @@
 
         params = {
             'count': count
         }
         if cursor is not None:
             params['cursor'] = cursor
 
-        response = (await self.http.get(
+        response, _ = await self.get(
             endpoint,
             params=params,
             headers=self._base_headers
-        )).json()
+        )
 
         global_objects = response['globalObjects']
         users = {
             id: User(self, build_user_data(data))
             for id, data in global_objects.get('users', {}).items()
         }
         tweets = {}
@@ -4448,19 +4615,19 @@
             'query': query,
         }
         if cursor is not None:
             variables['cursor'] = cursor
         params = flatten_params({
             'variables': variables
         })
-        response = (await self.http.get(
+        response, _ = await self.get(
             Endpoint.SEARCH_COMMUNITY,
             params=params,
             headers=self._base_headers
-        )).json()
+        )
 
         items = find_dict(response, 'items_results')[0]
         communities = []
         for item in items:
             communities.append(Community(self, item['result']))
         next_cursor_ = find_dict(response, 'next_cursor')
         next_cursor = next_cursor_[0] if next_cursor_ else None
@@ -4492,19 +4659,19 @@
         params = flatten_params({
             'variables': {'communityId': community_id},
             'features': {
                 'c9s_list_members_action_api_enabled':False,
                 'c9s_superc9s_indication_enabled':False
             }
         })
-        response = (await self.http.get(
+        response, _ = await self.get(
             Endpoint.GET_COMMUNITY,
             params=params,
             headers=self._base_headers
-        )).json()
+        )
         community_data = find_dict(response, 'result')[0]
         return Community(self, community_data)
 
     async def get_community_tweets(
         self,
         community_id: str,
         tweet_type: Literal['Top', 'Latest', 'Media'],
@@ -4559,19 +4726,19 @@
         if cursor is not None:
             variables['cursor'] = cursor
 
         params = flatten_params({
             'variables': variables,
             'features': COMMUNITY_TWEETS_FEATURES
         })
-        response = (await self.http.get(
+        response, _ = await self.get(
             endpoint,
             params=params,
             headers=self._base_headers
-        )).json()
+        )
 
         entries = find_dict(response, 'entries')[0]
         if tweet_type == 'Media':
             if cursor is None:
                 items = entries[0]['content']['items']
                 next_cursor = entries[-1]['content']['value']
                 previous_cursor = entries[-2]['content']['value']
@@ -4635,19 +4802,19 @@
         }
         if cursor is not None:
             variables['cursor'] = cursor
         params = flatten_params({
             'variables': variables,
             'features': COMMUNITY_TWEETS_FEATURES
         })
-        response = (await self.http.get(
+        response, _ = await self.get(
             Endpoint.COMMUNITIES_TIMELINE,
             params=params,
             headers=self._base_headers
-        )).json()
+        )
         items = find_dict(response, 'entries')[0]
         tweets = []
         for item in items:
             if not item['entryId'].startswith('tweet'):
                 continue
             tweet_data = find_dict(item, 'result')[0]
             if 'tweet' in tweet_data:
@@ -4690,19 +4857,19 @@
         data = {
             'variables': {
                 'communityId': community_id
             },
             'features': JOIN_COMMUNITY_FEATURES,
             'queryId': get_query_id(Endpoint.JOIN_COMMUNITY)
         }
-        response = (await self.http.post(
+        response, _ = await self.post(
             Endpoint.JOIN_COMMUNITY,
             json=data,
             headers=self._base_headers
-        )).json()
+        )
         community_data = response['data']['community_join']
         community_data['rest_id'] = community_data['id_str']
         return Community(self, community_data)
 
     async def leave_community(self, community_id: str) -> Community:
         """
         Leave a community.
@@ -4720,19 +4887,19 @@
         data = {
             'variables': {
                 'communityId': community_id
             },
             'features': JOIN_COMMUNITY_FEATURES,
             'queryId': get_query_id(Endpoint.LEAVE_COMMUNITY)
         }
-        response = (await self.http.post(
+        response, _ = await self.post(
             Endpoint.LEAVE_COMMUNITY,
             json=data,
             headers=self._base_headers
-        )).json()
+        )
         community_data = response['data']['community_leave']
         community_data['rest_id'] = community_data['id_str']
         return Community(self, community_data)
 
     async def request_to_join_community(
         self, community_id: str, answer: str | None = None
     ) -> Community:
@@ -4755,19 +4922,19 @@
             'variables': {
                 'communityId': community_id,
                 'answer': '' if answer is None else answer
             },
             'features': JOIN_COMMUNITY_FEATURES,
             'queryId': get_query_id(Endpoint.REQUEST_TO_JOIN_COMMUNITY)
         }
-        response = (await self.http.post(
+        response, _ = await self.post(
             Endpoint.REQUEST_TO_JOIN_COMMUNITY,
             json=data,
             headers=self._base_headers
-        )).json()
+        )
         community_data = find_dict(response, 'result')[0]
         community_data['rest_id'] = community_data['id_str']
         return Community(self, community_data)
 
     async def _get_community_users(
         self, endpoint: str, community_id: str, count: int, cursor: str | None
     ):
@@ -4782,19 +4949,19 @@
             variables['cursor'] = cursor
         params = flatten_params({
             'variables': variables,
             'features': {
                 'responsive_web_graphql_timeline_navigation_enabled': True
             }
         })
-        response = (await self.http.get(
+        response, _ = await self.get(
             endpoint,
             params=params,
             headers=self._base_headers
-        )).json()
+        )
 
         items = find_dict(response, 'items_results')[0]
         users = []
         for item in items:
             if not 'result' in item:
                 continue
             if item['result'].get('__typename') != 'User':
@@ -4901,19 +5068,19 @@
         }
         if cursor is not None:
             variables['cursor'] = cursor
         params = flatten_params({
             'variables': variables,
             'features': COMMUNITY_TWEETS_FEATURES
         })
-        response = (await self.http.get(
+        response, _ = await self.get(
             Endpoint.SEARCH_COMMUNITY_TWEET,
             params=params,
             headers=self._base_headers
-        )).json()
+        )
 
         items = find_dict(response, 'entries')[0]
         tweets = []
         for item in items:
             if not item['entryId'].startswith('tweet'):
                 continue
 
@@ -4937,18 +5104,18 @@
     async def _stream(
         self, topics: set[str]
     ) -> AsyncGenerator[tuple[str, Payload]]:
         headers = self._base_headers
         headers.pop('content-type')
         params = {'topics': ','.join(topics)}
 
-        async with self.http.stream(
+        async with self.stream(
             'GET', Endpoint.EVENTS, params=params, timeout=None
         ) as response:
-            self.http._remove_duplicate_ct0_cookie()
+            self._remove_duplicate_ct0_cookie()
             async for line in response.aiter_lines():
                 try:
                     data = json.loads(line)
                 except json.JSONDecodeError:
                     continue
                 payload = _payload_from_data(data['payload'])
                 yield data.get('topic'), payload
@@ -5044,14 +5211,14 @@
         data = urlencode({
             'sub_topics': ','.join(subscribe),
             'unsub_topics': ','.join(unsubscribe)
         })
         headers = self._base_headers
         headers['content-type'] = 'application/x-www-form-urlencoded'
         headers['LivePipeline-Session'] = session.id
-        response = (await self.http.post(
+        response, _ = await self.post(
             Endpoint.UPDATE_SUBSCRIPTIONS, data=data, headers=headers
-        )).json()
+        )
         session.topics |= subscribe
         session.topics -= unsubscribe
 
         return _payload_from_data(response)
```

### Comparing `twikit-1.6.4/twikit/twikit_async/community.py` & `twikit-1.7.0/twikit/twikit_async/community.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.4/twikit/twikit_async/errors.py` & `twikit-1.7.0/twikit/twikit_async/errors.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.4/twikit/twikit_async/geo.py` & `twikit-1.7.0/twikit/twikit_async/geo.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.4/twikit/twikit_async/group.py` & `twikit-1.7.0/twikit/twikit_async/group.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.4/twikit/twikit_async/list.py` & `twikit-1.7.0/twikit/twikit_async/list.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.4/twikit/twikit_async/message.py` & `twikit-1.7.0/twikit/twikit_async/message.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.4/twikit/twikit_async/notification.py` & `twikit-1.7.0/twikit/twikit_async/notification.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.4/twikit/twikit_async/streaming.py` & `twikit-1.7.0/twikit/twikit_async/streaming.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.4/twikit/twikit_async/trend.py` & `twikit-1.7.0/twikit/twikit_async/trend.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.4/twikit/twikit_async/tweet.py` & `twikit-1.7.0/twikit/twikit_async/tweet.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,18 +30,18 @@
         The full text of the tweet.
     lang : :class:`str`
         The language of the tweet.
     in_reply_to : :class:`str`
         The tweet ID this tweet is in reply to, if any
     is_quote_status : :class:`bool`
         Indicates if the tweet is a quote status.
-    quote : :class:`Tweet`
+    quote : :class:`Tweet` | None
         The Tweet being quoted (if any)
-    retweeted_tweet : :class:`bool`
-        Whether the tweet is a retweet
+    retweeted_tweet : :class:`Tweet` | None
+        The Tweet being retweeted (if any)
     possibly_sensitive : :class:`bool`
         Indicates if the tweet content may be sensitive.
     possibly_sensitive_editable : :class:`bool`
         Indicates if the tweet's sensitivity can be edited.
     quote_count : :class:`int`
         The count of quotes for the tweet.
     media : :class:`list`
@@ -688,8 +688,8 @@
     def __repr__(self) -> str:
         return f'<CommunityNote id="{self.id}">'
 
     def __eq__(self, __value: object) -> bool:
         return isinstance(__value, CommunityNote) and self.id == __value.id
 
     def __ne__(self, __value: object) -> bool:
-        return not self == __value
+        return not self == __value
```

### Comparing `twikit-1.6.4/twikit/twikit_async/user.py` & `twikit-1.7.0/twikit/twikit_async/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -375,14 +375,36 @@
 
         See Also
         --------
         Client.get_user_subscriptions
         """
         return await self._client.get_user_subscriptions(self.id, count)
 
+    async def get_latest_followers(
+        self, count: int | None = None, cursor: str | None = None
+    ) -> Result[User]:
+        """
+        Retrieves the latest followers.
+        Max count : 200
+        """
+        return await self._client.get_latest_followers(
+            self.id, count=count, cursor=cursor
+        )
+
+    async def get_latest_friends(
+        self, count: int | None = None, cursor: str | None = None
+    ) -> Result[User]:
+        """
+        Retrieves the latest friends (following users).
+        Max count : 200
+        """
+        return await self._client.get_latest_friends(
+            self.id, count=count, cursor=cursor
+        )
+
     async def send_dm(
         self, text: str, media_id: str = None, reply_to = None
     ) -> Message:
         """
         Send a direct message to the user.
 
         Parameters
```

### Comparing `twikit-1.6.4/twikit/twikit_async/utils.py` & `twikit-1.7.0/twikit/twikit_async/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,20 +94,20 @@
         data = {}
 
         if self.token is not None:
             data['flow_token'] = self.token
         if subtask_inputs is not None:
             data['subtask_inputs'] = list(subtask_inputs)
 
-        response = (await self._client.http.post(
+        response, _ = await self._client.post(
             self.endpoint,
             data=json.dumps(data),
             headers=self.headers,
             **kwargs
-        )).json()
+        )
         self.response = response
 
     @property
     def token(self) -> str | None:
         if self.response is None:
             return None
         return self.response.get('flow_token')
```

### Comparing `twikit-1.6.4/twikit/user.py` & `twikit-1.7.0/twikit/user.py`

 * *Files 6% similar despite different names*

```diff
@@ -375,14 +375,36 @@
 
         See Also
         --------
         Client.get_user_subscriptions
         """
         return self._client.get_user_subscriptions(self.id, count)
 
+    def get_latest_followers(
+        self, count: int | None = None, cursor: str | None = None
+    ) -> Result[User]:
+        """
+        Retrieves the latest followers.
+        Max count : 200
+        """
+        return self._client.get_latest_followers(
+            self.id, count=count, cursor=cursor
+        )
+
+    def get_latest_friends(
+        self, count: int | None = None, cursor: str | None = None
+    ) -> Result[User]:
+        """
+        Retrieves the latest friends (following users).
+        Max count : 200
+        """
+        return self._client.get_latest_friends(
+            self.id, count=count, cursor=cursor
+        )
+
     def send_dm(
         self, text: str, media_id: str = None, reply_to = None
     ) -> Message:
         """
         Send a direct message to the user.
 
         Parameters
```

### Comparing `twikit-1.6.4/twikit/utils.py` & `twikit-1.7.0/twikit/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -389,20 +389,20 @@
         data = {}
 
         if self.token is not None:
             data['flow_token'] = self.token
         if subtask_inputs is not None:
             data['subtask_inputs'] = list(subtask_inputs)
 
-        response = self._client.http.post(
+        response, _ = self._client.post(
             self.endpoint,
             data=json.dumps(data),
             headers=self.headers,
             **kwargs
-        ).json()
+        )
         self.response = response
 
     @property
     def token(self) -> str | None:
         if self.response is None:
             return None
         return self.response.get('flow_token')
```

### Comparing `twikit-1.6.4/twikit.egg-info/PKG-INFO` & `twikit-1.7.0/twikit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twikit
-Version: 1.6.4
+Version: 1.7.0
 Summary: Twitter API wrapper for python with **no API key required**.
 Home-page: https://github.com/d60/twikit
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `twikit-1.6.4/twikit.egg-info/SOURCES.txt` & `twikit-1.7.0/twikit.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -4,38 +4,42 @@
 twikit/__init__.py
 twikit/bookmark.py
 twikit/client.py
 twikit/community.py
 twikit/errors.py
 twikit/geo.py
 twikit/group.py
-twikit/http.py
 twikit/list.py
 twikit/message.py
 twikit/notification.py
 twikit/py.typed
 twikit/streaming.py
 twikit/trend.py
 twikit/tweet.py
 twikit/user.py
 twikit/utils.py
 twikit.egg-info/PKG-INFO
 twikit.egg-info/SOURCES.txt
 twikit.egg-info/dependency_links.txt
 twikit.egg-info/requires.txt
 twikit.egg-info/top_level.txt
+twikit/_captcha/__init__.py
+twikit/_captcha/base.py
+twikit/_captcha/capsolver.py
 twikit/twikit_async/__init__.py
 twikit/twikit_async/bookmark.py
 twikit/twikit_async/client.py
 twikit/twikit_async/community.py
 twikit/twikit_async/errors.py
 twikit/twikit_async/geo.py
 twikit/twikit_async/group.py
-twikit/twikit_async/http.py
 twikit/twikit_async/list.py
 twikit/twikit_async/message.py
 twikit/twikit_async/notification.py
 twikit/twikit_async/streaming.py
 twikit/twikit_async/trend.py
 twikit/twikit_async/tweet.py
 twikit/twikit_async/user.py
-twikit/twikit_async/utils.py
+twikit/twikit_async/utils.py
+twikit/twikit_async/_captcha/__init__.py
+twikit/twikit_async/_captcha/base.py
+twikit/twikit_async/_captcha/capsolver.py
```

