# Comparing `tmp/locomotivecms-0.0.2.tar.gz` & `tmp/locomotivecms-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/locomotivecms-0.0.2.tar", last modified: Thu Sep 19 14:03:30 2019, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `locomotivecms-0.0.2.tar` & `locomotivecms-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,7 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-19 14:03:30.000000 locomotivecms-0.0.2/
--rw-rw-r--   0 travis    (2000) travis    (2000)       25 2019-09-19 14:03:16.000000 locomotivecms-0.0.2/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2019-09-19 14:03:16.000000 locomotivecms-0.0.2/requirements.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-19 14:03:30.000000 locomotivecms-0.0.2/locomotivecms.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)      522 2019-09-19 14:03:30.000000 locomotivecms-0.0.2/locomotivecms.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-09-19 14:03:30.000000 locomotivecms-0.0.2/locomotivecms.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2019-09-19 14:03:30.000000 locomotivecms-0.0.2/locomotivecms.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-09-19 14:03:30.000000 locomotivecms-0.0.2/locomotivecms.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      316 2019-09-19 14:03:30.000000 locomotivecms-0.0.2/locomotivecms.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2019-09-19 14:03:30.000000 locomotivecms-0.0.2/locomotivecms.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      522 2019-09-19 14:03:30.000000 locomotivecms-0.0.2/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-19 14:03:30.000000 locomotivecms-0.0.2/locomotivecms/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3495 2019-09-19 14:03:16.000000 locomotivecms-0.0.2/locomotivecms/main.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       60 2019-09-19 14:03:16.000000 locomotivecms-0.0.2/locomotivecms/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-09-19 14:03:30.000000 locomotivecms-0.0.2/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      182 2019-09-19 14:03:16.000000 locomotivecms-0.0.2/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1029 2019-09-19 14:03:16.000000 locomotivecms-0.0.2/setup.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 locomotivecms-0.0.3/.github/workflows/release.yml
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 locomotivecms-0.0.3/locomotivecms/__init__.py
+-rw-r--r--   0        0        0     3473 2020-02-02 00:00:00.000000 locomotivecms-0.0.3/locomotivecms/main.py
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 locomotivecms-0.0.3/.gitignore
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 locomotivecms-0.0.3/README.rst
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 locomotivecms-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 locomotivecms-0.0.3/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `locomotivecms-0.0.2/locomotivecms/main.py` & `locomotivecms-0.0.3/locomotivecms/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 # -*- coding: utf-8 -*-
 # Copyright 2017 Akretion (http://www.akretion.com).
 # @author Sébastien BEAU <sebastien.beau@akretion.com>
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl).
 
 import requests
 
-__version__ = '0.0.2'
-
 
 class LocomotiveApiError(Exception):
 
     def __init__(self, response, status_code):
-        message = response.pop('error')
+        message = response.pop('error', str(response))
         super(LocomotiveApiError, self).__init__(message)
         self.status_code = status_code
         self.extra = response
 
 
 class LocomotiveResource(object):
 
@@ -103,15 +101,15 @@
         kwargs = {'headers': self.header()}
         if method == 'get':
             kwargs['params'] = data
         else:
             kwargs['json'] = data
             kwargs['files'] = files
         res = getattr(requests, method)(self.url + url, **kwargs)
-        if res.status_code/100 != 2:
+        if not res.ok:
             raise LocomotiveApiError(res.json(), res.status_code)
         return res.json()
 
     def content(self, content_type):
         return LocomotiveContent(self, content_type)
 
     def asset(self):
```

