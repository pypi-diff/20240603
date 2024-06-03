# Comparing `tmp/waylay_sdk_core-0.2.1.tar.gz` & `tmp/waylay_sdk_core-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waylay_sdk_core-0.2.1.tar", last modified: Tue Apr 23 12:34:40 2024, max compression
+gzip compressed data, was "waylay_sdk_core-0.2.2.tar", last modified: Mon Jun  3 07:54:49 2024, max compression
```

## Comparing `waylay_sdk_core-0.2.1.tar` & `waylay_sdk_core-0.2.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-23 12:34:40.241704 waylay_sdk_core-0.2.1/
--rw-r--r--   0 thomas     (502) staff       (20)      746 2024-03-26 09:30:45.000000 waylay_sdk_core-0.2.1/LICENSE.txt
--rw-r--r--   0 thomas     (502) staff       (20)     3967 2024-04-23 12:34:40.241327 waylay_sdk_core-0.2.1/PKG-INFO
--rw-r--r--   0 thomas     (502) staff       (20)     1710 2024-04-08 12:34:55.000000 waylay_sdk_core-0.2.1/README.md
--rw-r--r--   0 thomas     (502) staff       (20)     1541 2024-04-23 12:31:12.000000 waylay_sdk_core-0.2.1/pyproject.toml
--rw-r--r--   0 thomas     (502) staff       (20)       38 2024-04-23 12:34:40.241761 waylay_sdk_core-0.2.1/setup.cfg
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-23 12:34:40.209468 waylay_sdk_core-0.2.1/src/
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-23 12:34:40.208408 waylay_sdk_core-0.2.1/src/waylay/
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-23 12:34:40.212743 waylay_sdk_core-0.2.1/src/waylay/sdk/
--rw-r--r--   0 thomas     (502) staff       (20)      754 2024-03-27 11:50:39.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/__init__.py
--rw-r--r--   0 thomas     (502) staff       (20)       65 2024-04-23 12:31:08.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/_version.py
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-23 12:34:40.220746 waylay_sdk_core-0.2.1/src/waylay/sdk/api/
--rw-r--r--   0 thomas     (502) staff       (20)      661 2024-03-25 07:17:42.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/api/__init__.py
--rw-r--r--   0 thomas     (502) staff       (20)     6901 2024-04-23 12:29:35.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/api/_models.py
--rw-r--r--   0 thomas     (502) staff       (20)     4423 2024-03-27 11:50:39.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/api/client.py
--rw-r--r--   0 thomas     (502) staff       (20)       40 2024-04-16 11:19:13.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/api/constants.py
--rw-r--r--   0 thomas     (502) staff       (20)     2298 2024-03-15 07:16:26.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/api/exceptions.py
--rw-r--r--   0 thomas     (502) staff       (20)     2299 2024-03-25 07:17:42.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/api/http.py
--rw-r--r--   0 thomas     (502) staff       (20)    14265 2024-04-22 09:24:30.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/api/serialization.py
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-23 12:34:40.223438 waylay_sdk_core-0.2.1/src/waylay/sdk/auth/
--rw-r--r--   0 thomas     (502) staff       (20)      523 2024-03-14 11:07:10.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/auth/__init__.py
--rw-r--r--   0 thomas     (502) staff       (20)      882 2024-03-14 10:54:52.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/auth/exceptions.py
--rw-r--r--   0 thomas     (502) staff       (20)     5972 2024-03-07 17:25:15.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/auth/interactive.py
--rw-r--r--   0 thomas     (502) staff       (20)    11539 2024-03-07 17:25:15.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/auth/model.py
--rw-r--r--   0 thomas     (502) staff       (20)      832 2024-03-07 17:25:15.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/auth/parse.py
--rw-r--r--   0 thomas     (502) staff       (20)     4243 2024-03-07 17:25:15.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/auth/provider.py
--rw-r--r--   0 thomas     (502) staff       (20)     1880 2024-04-08 09:44:30.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/client.py
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-23 12:34:40.228040 waylay_sdk_core-0.2.1/src/waylay/sdk/config/
--rw-r--r--   0 thomas     (502) staff       (20)      341 2024-03-14 11:07:10.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/config/__init__.py
--rw-r--r--   0 thomas     (502) staff       (20)     3106 2024-03-26 17:17:35.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/config/client.py
--rw-r--r--   0 thomas     (502) staff       (20)    13577 2024-04-22 09:24:30.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/config/model.py
--rw-r--r--   0 thomas     (502) staff       (20)     2809 2024-03-15 07:16:26.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/exceptions.py
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-23 12:34:40.230028 waylay_sdk_core-0.2.1/src/waylay/sdk/plugin/
--rw-r--r--   0 thomas     (502) staff       (20)      229 2024-03-14 11:07:10.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/plugin/__init__.py
--rw-r--r--   0 thomas     (502) staff       (20)     4401 2024-03-25 07:17:42.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/plugin/base.py
--rw-r--r--   0 thomas     (502) staff       (20)     2373 2024-03-25 07:17:42.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/plugin/client.py
--rw-r--r--   0 thomas     (502) staff       (20)      206 2024-04-08 09:44:30.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/plugin/loader.py
--rw-r--r--   0 thomas     (502) staff       (20)     2480 2024-04-08 09:44:30.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/plugin/type_stubs.py
--rw-r--r--   0 thomas     (502) staff       (20)       80 2024-02-08 12:59:42.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/py.typed
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-23 12:34:40.233856 waylay_sdk_core-0.2.1/src/waylay/sdk/services/
--rw-r--r--   0 thomas     (502) staff       (20)     4853 2024-04-22 09:24:30.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/services/gateway.py
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-23 12:34:40.240311 waylay_sdk_core-0.2.1/src/waylay_sdk_core.egg-info/
--rw-r--r--   0 thomas     (502) staff       (20)     3967 2024-04-23 12:34:40.000000 waylay_sdk_core-0.2.1/src/waylay_sdk_core.egg-info/PKG-INFO
--rw-r--r--   0 thomas     (502) staff       (20)     1133 2024-04-23 12:34:40.000000 waylay_sdk_core-0.2.1/src/waylay_sdk_core.egg-info/SOURCES.txt
--rw-r--r--   0 thomas     (502) staff       (20)        1 2024-04-23 12:34:40.000000 waylay_sdk_core-0.2.1/src/waylay_sdk_core.egg-info/dependency_links.txt
--rw-r--r--   0 thomas     (502) staff       (20)       64 2024-04-23 12:34:40.000000 waylay_sdk_core-0.2.1/src/waylay_sdk_core.egg-info/entry_points.txt
--rw-r--r--   0 thomas     (502) staff       (20)      365 2024-04-23 12:34:40.000000 waylay_sdk_core-0.2.1/src/waylay_sdk_core.egg-info/requires.txt
--rw-r--r--   0 thomas     (502) staff       (20)        7 2024-04-23 12:34:40.000000 waylay_sdk_core-0.2.1/src/waylay_sdk_core.egg-info/top_level.txt
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-06-03 07:54:49.885872 waylay_sdk_core-0.2.2/
+-rw-r--r--   0 thomas     (502) staff       (20)      746 2024-05-29 07:23:18.000000 waylay_sdk_core-0.2.2/LICENSE.txt
+-rw-r--r--   0 thomas     (502) staff       (20)     3923 2024-06-03 07:54:49.885525 waylay_sdk_core-0.2.2/PKG-INFO
+-rw-r--r--   0 thomas     (502) staff       (20)     1710 2024-04-08 12:34:55.000000 waylay_sdk_core-0.2.2/README.md
+-rw-r--r--   0 thomas     (502) staff       (20)     1854 2024-05-29 07:23:18.000000 waylay_sdk_core-0.2.2/pyproject.toml
+-rw-r--r--   0 thomas     (502) staff       (20)       38 2024-06-03 07:54:49.885920 waylay_sdk_core-0.2.2/setup.cfg
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-06-03 07:54:49.861083 waylay_sdk_core-0.2.2/src/
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-06-03 07:54:49.860213 waylay_sdk_core-0.2.2/src/waylay/
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-06-03 07:54:49.866695 waylay_sdk_core-0.2.2/src/waylay/sdk/
+-rw-r--r--   0 thomas     (502) staff       (20)      754 2024-05-28 09:04:43.000000 waylay_sdk_core-0.2.2/src/waylay/sdk/__init__.py
+-rw-r--r--   0 thomas     (502) staff       (20)      130 2024-05-29 07:23:18.000000 waylay_sdk_core-0.2.2/src/waylay/sdk/_version.py
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-06-03 07:54:49.869699 waylay_sdk_core-0.2.2/src/waylay/sdk/api/
+-rw-r--r--   0 thomas     (502) staff       (20)      661 2024-05-28 09:04:43.000000 waylay_sdk_core-0.2.2/src/waylay/sdk/api/__init__.py
+-rw-r--r--   0 thomas     (502) staff       (20)     6949 2024-05-29 07:23:18.000000 waylay_sdk_core-0.2.2/src/waylay/sdk/api/_models.py
+-rw-r--r--   0 thomas     (502) staff       (20)     4463 2024-06-03 07:53:49.000000 waylay_sdk_core-0.2.2/src/waylay/sdk/api/client.py
+-rw-r--r--   0 thomas     (502) staff       (20)       69 2024-05-28 09:04:43.000000 waylay_sdk_core-0.2.2/src/waylay/sdk/api/constants.py
+-rw-r--r--   0 thomas     (502) staff       (20)     2489 2024-05-28 09:04:43.000000 waylay_sdk_core-0.2.2/src/waylay/sdk/api/exceptions.py
+-rw-r--r--   0 thomas     (502) staff       (20)     2313 2024-05-28 09:04:43.000000 waylay_sdk_core-0.2.2/src/waylay/sdk/api/http.py
+-rw-r--r--   0 thomas     (502) staff       (20)    14530 2024-06-03 07:53:49.000000 waylay_sdk_core-0.2.2/src/waylay/sdk/api/serialization.py
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-06-03 07:54:49.872090 waylay_sdk_core-0.2.2/src/waylay/sdk/auth/
+-rw-r--r--   0 thomas     (502) staff       (20)      522 2024-05-31 08:28:55.000000 waylay_sdk_core-0.2.2/src/waylay/sdk/auth/__init__.py
+-rw-r--r--   0 thomas     (502) staff       (20)      883 2024-05-28 09:04:43.000000 waylay_sdk_core-0.2.2/src/waylay/sdk/auth/exceptions.py
+-rw-r--r--   0 thomas     (502) staff       (20)     5996 2024-05-28 09:04:43.000000 waylay_sdk_core-0.2.2/src/waylay/sdk/auth/interactive.py
+-rw-r--r--   0 thomas     (502) staff       (20)    12079 2024-06-03 07:53:49.000000 waylay_sdk_core-0.2.2/src/waylay/sdk/auth/model.py
+-rw-r--r--   0 thomas     (502) staff       (20)      826 2024-05-28 09:04:43.000000 waylay_sdk_core-0.2.2/src/waylay/sdk/auth/parse.py
+-rw-r--r--   0 thomas     (502) staff       (20)     6349 2024-06-03 07:53:49.000000 waylay_sdk_core-0.2.2/src/waylay/sdk/auth/provider.py
+-rw-r--r--   0 thomas     (502) staff       (20)     1855 2024-05-28 09:04:43.000000 waylay_sdk_core-0.2.2/src/waylay/sdk/client.py
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-06-03 07:54:49.875952 waylay_sdk_core-0.2.2/src/waylay/sdk/config/
+-rw-r--r--   0 thomas     (502) staff       (20)      297 2024-05-28 09:04:43.000000 waylay_sdk_core-0.2.2/src/waylay/sdk/config/__init__.py
+-rw-r--r--   0 thomas     (502) staff       (20)     3053 2024-05-28 09:04:43.000000 waylay_sdk_core-0.2.2/src/waylay/sdk/config/client.py
+-rw-r--r--   0 thomas     (502) staff       (20)    13201 2024-05-29 07:23:18.000000 waylay_sdk_core-0.2.2/src/waylay/sdk/config/model.py
+-rw-r--r--   0 thomas     (502) staff       (20)     2864 2024-05-28 09:04:43.000000 waylay_sdk_core-0.2.2/src/waylay/sdk/exceptions.py
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-06-03 07:54:49.878857 waylay_sdk_core-0.2.2/src/waylay/sdk/plugin/
+-rw-r--r--   0 thomas     (502) staff       (20)      229 2024-05-28 09:04:43.000000 waylay_sdk_core-0.2.2/src/waylay/sdk/plugin/__init__.py
+-rw-r--r--   0 thomas     (502) staff       (20)     4447 2024-06-03 07:53:49.000000 waylay_sdk_core-0.2.2/src/waylay/sdk/plugin/base.py
+-rw-r--r--   0 thomas     (502) staff       (20)     2418 2024-05-28 09:04:43.000000 waylay_sdk_core-0.2.2/src/waylay/sdk/plugin/client.py
+-rw-r--r--   0 thomas     (502) staff       (20)      207 2024-05-28 09:04:43.000000 waylay_sdk_core-0.2.2/src/waylay/sdk/plugin/loader.py
+-rw-r--r--   0 thomas     (502) staff       (20)     2481 2024-05-28 09:04:43.000000 waylay_sdk_core-0.2.2/src/waylay/sdk/plugin/type_stubs.py
+-rw-r--r--   0 thomas     (502) staff       (20)       80 2024-02-08 12:59:42.000000 waylay_sdk_core-0.2.2/src/waylay/sdk/py.typed
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-06-03 07:54:49.879646 waylay_sdk_core-0.2.2/src/waylay/sdk/services/
+-rw-r--r--   0 thomas     (502) staff       (20)     4932 2024-05-28 09:04:43.000000 waylay_sdk_core-0.2.2/src/waylay/sdk/services/gateway.py
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-06-03 07:54:49.884649 waylay_sdk_core-0.2.2/src/waylay_sdk_core.egg-info/
+-rw-r--r--   0 thomas     (502) staff       (20)     3923 2024-06-03 07:54:49.000000 waylay_sdk_core-0.2.2/src/waylay_sdk_core.egg-info/PKG-INFO
+-rw-r--r--   0 thomas     (502) staff       (20)     1133 2024-06-03 07:54:49.000000 waylay_sdk_core-0.2.2/src/waylay_sdk_core.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas     (502) staff       (20)        1 2024-06-03 07:54:49.000000 waylay_sdk_core-0.2.2/src/waylay_sdk_core.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas     (502) staff       (20)       64 2024-06-03 07:54:49.000000 waylay_sdk_core-0.2.2/src/waylay_sdk_core.egg-info/entry_points.txt
+-rw-r--r--   0 thomas     (502) staff       (20)      352 2024-06-03 07:54:49.000000 waylay_sdk_core-0.2.2/src/waylay_sdk_core.egg-info/requires.txt
+-rw-r--r--   0 thomas     (502) staff       (20)        7 2024-06-03 07:54:49.000000 waylay_sdk_core-0.2.2/src/waylay_sdk_core.egg-info/top_level.txt
```

### Comparing `waylay_sdk_core-0.2.1/LICENSE.txt` & `waylay_sdk_core-0.2.2/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ISC License (ISC)
-Copyright 2020, Waylay
+Copyright 2024, Waylay
 
 Permission to use, copy, modify, and/or distribute this software for any purpose 
 with or without fee is hereby granted, provided that the above copyright notice 
 and this permission notice appear in all copies.
 
 THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH 
 REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
```

### Comparing `waylay_sdk_core-0.2.1/PKG-INFO` & `waylay_sdk_core-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-core
-Version: 0.2.1
+Version: 0.2.2
 Summary: Waylay Python SDK.
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
-        Copyright 2020, Waylay
+        Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
         and this permission notice appear in all copies.
         
         THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH 
         REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND 
@@ -43,15 +43,14 @@
 Requires-Dist: starlette; extra == "dev"
 Requires-Dist: syrupy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
 Requires-Dist: types-appdirs; extra == "dev"
 Requires-Dist: types-python-dateutil; extra == "dev"
-Requires-Dist: docformatter; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: sse-starlette; extra == "dev"
 
 # Waylay Python SDK
 
 Python SDK for the Waylay Platform.
```

### Comparing `waylay_sdk_core-0.2.1/README.md` & `waylay_sdk_core-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `waylay_sdk_core-0.2.1/pyproject.toml` & `waylay_sdk_core-0.2.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools"]
+requires = ["setuptools", "setuptools-git-versioning"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "waylay-sdk-core"
-version = "0.2.1"
+dynamic = ["version"]
 description = "Waylay Python SDK."
 requires-python = ">=3.9"
 keywords = ["waylay", "sdk"]
 readme = "README.md"
 authors = [{name = "Waylay", email = "info@waylay.io"}]
 license={file = "LICENSE.txt"}
 dependencies = [
@@ -28,14 +28,16 @@
 Homepage = "https://www.waylay.io/"
 Documentation = "https://docs.waylay.io/#/"
 Repository = "https://github.com/waylayio/waylay-sdk-py.git"
 
 [project.entry-points.dynamic]
 "waylay_sdk_plugins"= "waylay.sdk.plugin.loader:PLUGINS"
 
+[tool.setuptools-git-versioning]
+enabled = true
 
 [tool.setuptools.package-data]
 waylay = ["py.typed"]
 
 [tool.setuptools.packages.find]
 where = ["src/"]
 include = ["waylay*"]
@@ -52,24 +54,32 @@
     "starlette",
     "syrupy",
     "ruff",
     'mypy',
     'types-python-jose',
     'types-appdirs',
     'types-python-dateutil',
-    'docformatter',
     'pre-commit',
     'sse-starlette',
 ]
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 
 [tool.ruff]
 include = ["pyproject.toml", "src/**/*.py", "test/**/*.py"]
 
 [tool.ruff.lint]
+select = ["E", "F", "B", "SIM", "FA", "D", "UP007", "I001", "PIE790"]
+ignore = ["D203", "D213"]
+
+[tool.ruff.lint.isort]
+from-first = false
+known-first-party = ["waylay*"]
+
+[tool.ruff.lint.per-file-ignores]
+"test/**/*.py" = ["D"] # no docstyle required
 
 [tool.coverage.report]
 exclude_also = [
     "if TYPE_CHECKING:"
 ]
```

### Comparing `waylay_sdk_core-0.2.1/src/waylay/sdk/__init__.py` & `waylay_sdk_core-0.2.2/src/waylay/sdk/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """The Waylay Python SDK."""
 
-from .client import WaylayClient
-from .config import WaylayConfig
+from ._version import __version__
+from .api import ApiClient
 from .auth import (
-    WaylayCredentials,
-    ClientCredentials,
     ApplicationCredentials,
-    TokenCredentials,
+    ClientCredentials,
     NoCredentials,
+    TokenCredentials,
+    WaylayCredentials,
     WaylayToken,
 )
-from .plugin import WaylayService, WaylayTool, WaylayPlugin, PluginAccess
-from .api import ApiClient
+from .client import WaylayClient
+from .config import WaylayConfig
 from .exceptions import WaylayError
-from ._version import __version__
+from .plugin import PluginAccess, WaylayPlugin, WaylayService, WaylayTool
 
 __all__ = [
     "WaylayClient",
     "WaylayConfig",
     "WaylayCredentials",
     "ClientCredentials",
     "ApplicationCredentials",
```

### Comparing `waylay_sdk_core-0.2.1/src/waylay/sdk/api/__init__.py` & `waylay_sdk_core-0.2.2/src/waylay/sdk/api/__init__.py`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """Waylay Api Configuration."""
 
 # export api classes
+from ._models import Model, Primitive
 from .client import ApiClient, RESTTimeout
+from .exceptions import ApiError, ApiValueError
 from .http import (
     AsyncClient,
-    HttpClientOptions,
     HeaderTypes,
+    HttpClientOptions,
     QueryParamTypes,
     Request,
-    Response,
-    RequestFiles,
     RequestContent,
     RequestData,
+    RequestFiles,
+    Response,
 )
-from .exceptions import ApiError, ApiValueError
-from ._models import Model, Primitive
 
 __all__ = [
     "ApiClient",
     "RESTTimeout",
     "AsyncClient",
     "HttpClientOptions",
     "HeaderTypes",
```

### Comparing `waylay_sdk_core-0.2.1/src/waylay/sdk/api/_models.py` & `waylay_sdk_core-0.2.2/src/waylay/sdk/api/_models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,38 @@
 from __future__ import annotations
-from abc import ABC
+
 import contextlib
+from abc import ABC
 from copy import deepcopy
 from datetime import date, datetime
 from decimal import Decimal
 from inspect import isclass
-from typing import TYPE_CHECKING, Any, Callable, Dict, List, Union, get_type_hints
+from typing import (
+    TYPE_CHECKING,
+    Annotated,
+    Any,
+    Callable,
+    Dict,
+    List,
+    Union,
+    get_type_hints,
+)
 
 from typing_extensions import (
-    Annotated,  # >=3.9
     Self,  # >=3.12
     TypeAliasType,  # >=3.12
 )
 
 if TYPE_CHECKING:
     from typing_extensions import TypeAlias  # >= Python 3.10
 
 from pydantic import (
     BaseModel as PydanticBaseModel,
+)
+from pydantic import (
     ConfigDict,
     SerializationInfo,
     StrictStr,
     TypeAdapter,
     ValidationError,
     ValidationInfo,
     ValidatorFunctionWrapHandler,
@@ -29,39 +40,45 @@
     model_serializer,
     model_validator,
 )
 from pydantic.functional_validators import ModelWrapValidatorHandler
 
 
 class BaseModel(PydanticBaseModel, ABC):
-    """Waylay base model class that adds some additional methods to Pydantic's `BaseModel`, including a custom validator and serializer."""
+    """Waylay base model class that adds additional methods to Pydantic's `BaseModel`.
+
+    Includes a custom validator and serializer.
+    """
 
     @model_serializer(mode="wrap")
     def _model_serializer(
         self, handler: Callable, info: SerializationInfo
     ) -> Dict[StrictStr, Any]:
-        """The default serializer of the model.
+        """Get the default serializer of the model.
 
         * Excludes `None` fields that were not set at model initialization.
         """
         model_dict = handler(self, info)
         return {
             k: v
             for k, v in model_dict.items()
             if v is not None or k in self.model_fields_set
         }
 
     @model_validator(mode="wrap")  # type: ignore[arg-type]
     def _model_validator(
         cls, value: Any, handler: ModelWrapValidatorHandler, info: ValidationInfo
     ):
-        """The default validator of the model.
+        """Get the default validator of the model.
 
-        When validation is called with a `skip_validation=True` context (e.g. `cls.model_validate(data, context={"skip_validation": True})`), the model is constructed without validation.
-        Any fields with a `Model` type will be constructed from their dict representation recursively.
+        When validation is called with a `skip_validation=True` context
+        (e.g. `cls.model_validate(data, context={"skip_validation": True})`),
+        the model is constructed without validation.
+        Any fields with a `Model` type will be constructed
+        from their dict representation recursively.
         """
         context = info.context or {}
         try:
             return handler(value)
         except ValidationError:
             context = info.context or {}
             if context.get("skip_validation", False):
@@ -81,36 +98,36 @@
                         setattr(model, field_name, None)
 
                 model.__pydantic_fields_set__ = model_fields_set
                 # recursively validate set fields
                 for field_name in model_fields_set:
                     field_value = getattr(model, field_name)
                     strict = (info.config or {}).get("strict")
-                    try:
+                    with contextlib.suppress(BaseException):
                         cls.__pydantic_validator__.validate_assignment(
                             model,
                             field_name,
                             field_value,
                             strict=strict,
                             context=context,
                         )
-                    except BaseException:
-                        pass
                 return model
             else:
                 raise
 
     @field_validator("*", mode="wrap")
     def _field_validator(
         cls, value: Any, handler: ValidatorFunctionWrapHandler, info: ValidationInfo
     ):
-        """The default field validator of the model.
+        """Get the default field validator of the model.
 
-        When validation is called with a `skip_validation=True` context, the field is assigned without validation.
-        If the field is a `Model` type, the model will be constructed from its dict representation recursively.
+        When validation is called with a `skip_validation=True` context,
+        the field is assigned without validation.
+        If the field is a `Model` type, the model will be constructed
+        from its dict representation recursively.
         """
         context = info.context or {}
         try:
             return handler(value)
         except ValidationError:
             context = info.context or {}
             if context.get("skip_validation", False):
@@ -172,14 +189,15 @@
         else:
             return obj
 
 
 Primitive: TypeAlias = Union[
     str, bool, int, float, Decimal, bytes, datetime, date, object, None
 ]
-Model: TypeAlias = TypeAliasType(  # type: ignore[valid-type]  #(https://github.com/python/mypy/issues/16614)
+Model: TypeAlias = TypeAliasType(  # type: ignore[misc]  #(https://github.com/python/mypy/issues/16614)
     "Model",
     Annotated[
-        Union[List["Model"], "_Model", Primitive],  # type: ignore[misc,possible cyclic definition]
-        "A basic model that acts like a `simpleNamespace`, or a collection over such models.",
+        Union[List["Model"], "_Model", Primitive],  # type: ignore[misc]
+        "A basic model that acts like a `simpleNamespace` "
+        "or a collection over such models.",
     ],
 )
```

### Comparing `waylay_sdk_core-0.2.1/src/waylay/sdk/api/client.py` & `waylay_sdk_core-0.2.2/src/waylay/sdk/api/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """API client."""
 
 from __future__ import annotations
-from typing import Mapping, Optional, Tuple, Union
+
+from collections.abc import Mapping
+from typing import Optional, Tuple, Union
 
 from .._version import __version__
 from ..config import WaylayConfig
-
 from .exceptions import SyncCtxMgtNotSupportedError
-from .serialization import WithSerializationSupport
 from .http import AsyncClient, HttpClientOptions, Request, Response
+from .serialization import WithSerializationSupport
 
 RESTTimeout = Union[
     Optional[float],
     Tuple[Optional[float], Optional[float], Optional[float], Optional[float]],
 ]
 
 
@@ -27,20 +28,20 @@
     :param configuration: configuration object for this client
 
     """
 
     config: WaylayConfig
     http_options: HttpClientOptions
     base_url: str
-    _http_client: Optional[AsyncClient]
+    _http_client: AsyncClient | None
 
     def __init__(
         self,
         config: WaylayConfig,
-        http_options: Optional[HttpClientOptions | AsyncClient] = None,
+        http_options: HttpClientOptions | AsyncClient | None = None,
     ) -> None:
         """Create an instance."""
         self.config = config
         self.http_options = {}
         self._http_client = None
         self.base_url = self.config.gateway_url
         if http_options:
@@ -51,15 +52,15 @@
         if not self.is_closed:
             raise AttributeError("Cannot set options on open client.")
         if isinstance(http_options, AsyncClient):
             self._http_client = http_options
         elif isinstance(http_options, Mapping):
             self.http_options = http_options
 
-    def clone(self, http_options: Optional[HttpClientOptions] = None):
+    def clone(self, http_options: HttpClientOptions | None = None):
         """Clone api client without http client."""
         http_options = (
             self.http_options
             if http_options is None
             else {**self.http_options, **http_options}
         )
         return self.__class__(self.config, http_options)
@@ -110,15 +111,15 @@
         auth = opts.get("auth", self.config.auth)
         client.auth = auth  # type: ignore
         client.headers.update({"User-Agent": f"waylay-sdk/python/{__version__}"})
         return client
 
     async def aclose(self):
         """Close the client."""
-        if not self.is_closed:
+        if self._http_client and not self.is_closed:
             await self._http_client.aclose()
             self._http_client = None
 
     async def _request(self, *args, **kwargs) -> Response:
         """Invoke a http request."""
         return await self.http_client.request(*args, **kwargs)
```

### Comparing `waylay_sdk_core-0.2.1/src/waylay/sdk/api/exceptions.py` & `waylay_sdk_core-0.2.2/src/waylay/sdk/api/exceptions.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,60 +1,65 @@
 """Exceptions."""
 
-from typing import Any, Optional
+from __future__ import annotations
 
-from .http import Response
+from typing import Any
 
-from ..exceptions import WaylayError, RequestError, RestResponseError
+from ..exceptions import RequestError, RestResponseError, WaylayError
+from .http import Response
 
 
 class ApiValueError(RequestError, ValueError):
     """Inappropriate argument value (of correct type) in a Waylay API request."""
 
-    def __init__(self, msg, path_to_item=None) -> None:
+    def __init__(self, msg: str, path_to_item=None) -> None:
         """Raise a value error.
 
         Args:
+        ----
             msg (str): the exception message
+            path_to_item (str): path into the request object
 
         Keyword Args:
+        ------------
             path_to_item (list) the path to the exception in the
                 received_data dict. None if unset
 
         """
-
         self.path_to_item = path_to_item
         full_msg = msg
         if path_to_item:
             full_msg = f"{msg} at {render_path(path_to_item)}"
         super(ApiValueError, self).__init__(full_msg)
 
 
 class ApiError(RestResponseError):
     """Exception class wrapping the response data of a REST call."""
 
-    data: Optional[Any]
+    data: Any | None
 
     def __init__(
         self,
+        *args,
         response: Response,
-        data: Optional[Any],
+        data: Any | None,
     ) -> None:
         """Create an instance."""
-        super().__init__(response)
+        super().__init__(*args, response=response)
         self.data = data
 
     @classmethod
     def from_response(
         cls,
+        message: str,
         response: Response,
-        data: Optional[Any],
+        data: Any | None,
     ):
         """Create an instance from a REST exception response."""
-        return cls(response, data)
+        return cls(message, response=response, data=data)
 
     def __str__(self):
         """Get the string representation of the exception."""
         error_message = super().__str__()
         if self.data and self.data != self.response.content:
             error_message += f"\nResponse data: {self.data}"
         return error_message
```

### Comparing `waylay_sdk_core-0.2.1/src/waylay/sdk/api/http.py` & `waylay_sdk_core-0.2.2/src/waylay/sdk/api/http.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Aliases for the http client."""
 
 from __future__ import annotations
+
+from collections.abc import Mapping, Sequence
 from typing import (
-    TypedDict,
-    Mapping,
-    Optional,
-    Callable,
+    IO,
     Any,
-    Union,
-    Sequence,
-    Tuple,
+    Callable,
     List,
-    IO,
+    Optional,
+    Tuple,
+    TypedDict,
+    Union,
 )
-from typing_extensions import Required  # >=3.11
 
-import httpx._client as httpx_types
 import httpx
+import httpx._client as httpx_types
+from typing_extensions import Required  # >=3.11
 
 AsyncClient = httpx.AsyncClient
 Response = httpx.Response
 Request = httpx.Request
 
 HeaderTypes = Union[
     Mapping[str, str],
@@ -60,25 +60,25 @@
     timeout: httpx_types.TimeoutTypes
     extensions: httpx_types.RequestExtensions
 
 
 class HttpClientOptions(TypedDict, total=False):
     """Options passed to the httpx client."""
 
-    auth: Optional[httpx_types.AuthTypes]  # explicit None do disable auth
+    auth: httpx_types.AuthTypes | None  # explicit None do disable auth
     params: httpx_types.QueryParamTypes
     headers: HeaderTypes
     cookies: httpx_types.CookieTypes
     verify: httpx_types.VerifyTypes
     cert: httpx_types.CertTypes
     http1: bool
     http2: bool
     proxy: httpx_types.ProxyTypes
     proxies: httpx_types.ProxiesTypes
-    mounts: Mapping[str, Optional[httpx_types.AsyncBaseTransport]]
+    mounts: Mapping[str, httpx_types.AsyncBaseTransport | None]
     timeout: httpx_types.TimeoutTypes
     follow_redirects: bool
     limits: httpx_types.Limits
     max_redirects: int
     event_hooks: Mapping[str, list[Callable[..., Any]]]
     base_url: str
     transport: httpx_types.AsyncBaseTransport
```

### Comparing `waylay_sdk_core-0.2.1/src/waylay/sdk/api/serialization.py` & `waylay_sdk_core-0.2.2/src/waylay/sdk/api/serialization.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,111 +1,116 @@
 """API client."""
 
 from __future__ import annotations
+
 import contextlib
+import datetime
 import json
 import logging
 import re
-import datetime
-from urllib.parse import quote
-from inspect import isclass
-from typing import (
-    Any,
+from abc import abstractmethod
+from collections.abc import (
     AsyncGenerator,
+    AsyncIterable,
     AsyncIterator,
+    Iterable,
     Mapping,
+)
+from inspect import isclass
+from typing import (
+    Any,
     Optional,
-    AsyncIterable,
+    Protocol,
     Type,
     TypeVar,
     Union,
-    Iterable,
-    Protocol,
     cast,
     runtime_checkable,
 )
-from abc import abstractmethod
+from urllib.parse import quote
 
+import httpx._client as httpxc
+from httpx import USE_CLIENT_DEFAULT, ResponseNotRead
+from jsonpath_ng import parse as jsonpath_parse  # type: ignore[import-untyped]
 from pydantic import BaseModel, ConfigDict, TypeAdapter, ValidationError
 from pydantic_core import to_jsonable_python
-from jsonpath_ng import parse as jsonpath_parse  # type: ignore[import-untyped]
-from httpx import USE_CLIENT_DEFAULT
-import httpx._client as httpxc
+from typing_extensions import (
+    TypeAlias,  # >=3.9
+)
 
+from ._models import Model
+from .exceptions import ApiError, ApiValueError, RestResponseError
 from .http import (
     AsyncClient,
-    Request,
-    Response,
-    QueryParamTypes,
     HeaderTypes,
-    RequestFiles,
+    QueryParamTypes,
+    Request,
     RequestContent,
     RequestData,
+    RequestFiles,
+    Response,
 )
-from .exceptions import ApiValueError, ApiError
-from ._models import Model
 
 _DEFAULT_RESPONSE_TYPE = Model
 _PRIMITIVE_BYTE_TYPES = (bytes, bytearray)
 _CLASS_MAPPING = {
     "date": datetime.date,
     "datetime": datetime.datetime,
     "Any": Any,
 }
 _ALLOWED_METHODS = ["GET", "HEAD", "DELETE", "POST", "PUT", "PATCH", "OPTIONS"]
 
 _MODEL_TYPE_ADAPTER = TypeAdapter(Model)
 
 log = logging.getLogger(__name__)
 
-DEFAULT_SERIALIZATION_ARGS = {"by_alias": True, "exclude_none": True}
-
 TEXT_EVENT_STREAM_CONTENT_TYPE = "text/event-stream"
 NDJSON_EVENT_STREAM_CONTENT_TYPE = "application/x-ndjson"
 EVENT_STREAM_CONTENT_TYPES = [
     TEXT_EVENT_STREAM_CONTENT_TYPE,
     NDJSON_EVENT_STREAM_CONTENT_TYPE,
 ]
+TypeMapping: TypeAlias = Union[
+    Mapping[str, Optional[Type[Any]]], Type[Any], None
+]
 
 
 class WithSerializationSupport:
     """Serialization support for the SDK client."""
 
     base_url: str
-    serialization_args = DEFAULT_SERIALIZATION_ARGS
 
     @property
     @abstractmethod
     def http_client(self) -> AsyncClient:
         """Get (or open) a http client."""
 
     async def request(
         self,
         method: str,
         resource_path: str,
-        path_params: Optional[Mapping[str, str]] = None,
+        path_params: Mapping[str, str] | None = None,
         *,
-        params: Optional[Union[QueryParamTypes, Mapping, BaseModel]] = None,
-        json: Optional[Any] = None,
-        content: Optional[RequestContent] = None,
-        files: Optional[RequestFiles] = None,
-        data: Optional[RequestData] = None,
-        headers: Optional[HeaderTypes] = None,
+        params: QueryParamTypes | Mapping | BaseModel | None = None,
+        json: Any | None = None,
+        content: RequestContent | None = None,
+        files: RequestFiles | None = None,
+        data: RequestData | None = None,
+        headers: HeaderTypes | None = None,
         cookies: httpxc.CookieTypes | None = None,
         timeout: httpxc.TimeoutTypes | None = None,
         extensions: httpxc.RequestExtensions | None = None,
         # Deserialization arguments
         response_type: Mapping[str, Type | None] | Type | None = None,
         select_path: str = "",
         raw_response: bool = False,
         # Additional parameters passed on to the http client
         **kwargs,
     ) -> Response | Any:
         """Perform a request with serialization and deserialization support."""
-
         # set aside send args
         send_args = {}
         for key in ["stream", "follow_redirects", "auth"]:
             if key in kwargs:
                 send_args[key] = kwargs.pop(key)
 
         api_request = self.build_request(
@@ -133,22 +138,22 @@
             stream=send_args.get("stream", False),
         )
 
     def build_request(
         self,
         method: str,
         resource_path: str,
-        path_params: Optional[Mapping[str, str]] = None,
+        path_params: Mapping[str, str] | None = None,
         *,
-        params: Optional[Union[QueryParamTypes, Mapping, BaseModel]] = None,
-        json: Optional[Any] = None,
-        content: Optional[RequestContent] = None,
-        files: Optional[RequestFiles] = None,
-        data: Optional[RequestData] = None,
-        headers: Optional[HeaderTypes] = None,
+        params: QueryParamTypes | Mapping | BaseModel | None = None,
+        json: Any | None = None,
+        content: RequestContent | None = None,
+        files: RequestFiles | None = None,
+        data: RequestData | None = None,
+        headers: HeaderTypes | None = None,
         cookies: httpxc.CookieTypes | None = None,
         timeout: httpxc.TimeoutTypes | None = None,
         extensions: httpxc.RequestExtensions | None = None,
     ) -> Request:
         """Build the HTTP request params needed by the request."""
         method = _validate_method(method)
         url = _interpolate_resource_path(resource_path, path_params)
@@ -164,40 +169,43 @@
             cookies=cookies,
             timeout=USE_CLIENT_DEFAULT if timeout is None else timeout,
             extensions=extensions,
         )
 
     def serialize(self, data):
         """Serialize to a jsonable python data structure."""
-        return to_jsonable_python(data, **self.serialization_args)
+        return to_jsonable_python(data, by_alias=True, exclude_none=True)
 
     def deserialize(
         self,
         response: Response,
         *,
-        response_type: Mapping[str, Type | None] | Type | None = None,
+        response_type: TypeMapping = None,
         select_path: str = "",
         stream: bool = False,
     ) -> Any:
         """Deserialize a http response into a python object.
 
         :param response_data: Response object to be deserialized.
         :param response_type: Response type to use for 2XX status codes,
             or a mapping per status code, including '2XX', '3XX', .. and
             '*' or 'default' wildcard keys.
         :param select_path: json path to be extracted from the json payload.
         :param stream: Whether the response should be in streaming mode.
-            If the response is an event stream, this function will return an async iterator.
-        :return: An instance of the type specified in the mapping, or an async iterator for event stream responses when stream is True.
+            If the response is an event stream, this function
+            will return an async iterator.
+        :return: An instance of the type specified in the mapping, or an async iterator
+            for event stream responses when stream is True.
         """
         status_code = response.status_code
         _response_type = _response_type_for_status_code(status_code, response_type)
 
         if not 200 <= response.status_code <= 299:
             raise ApiError.from_response(
+                "Error response.",
                 response,
                 _deserialize_response(
                     response, response_type=_response_type, select_path=select_path
                 ),
             )
         content_type = response.headers.get("content-type", "")
         is_event_stream = any(
@@ -217,15 +225,15 @@
 
 
 @runtime_checkable
 class Readable(Protocol):
     """Anything with a binary read method."""
 
     def read(self, n: int = -1) -> bytes:
-        """Read a binary chunk"""
+        """Read a binary chunk."""
 
 
 def _convert_content(content: Any):
     """Convert Iterable and Readable to AsyncIterable."""
     # do not handle cases httpx handles
     if isinstance(content, (bytes, str, AsyncIterable)):
         return content
@@ -253,15 +261,15 @@
     if method not in _ALLOWED_METHODS:
         raise ApiValueError(f"Method {method} is not supported.")
     return method
 
 
 def _interpolate_resource_path(
     resource_path: str,
-    path_params: Optional[Mapping[str, str]] = None,
+    path_params: Mapping[str, str] | None = None,
 ):
     if not path_params:
         return resource_path
     for k, v in path_params.items():
         # specified safe chars, encode everything
         resource_path = resource_path.replace("{%s}" % k, quote(str(v)))
     return resource_path
@@ -281,41 +289,44 @@
         return type_adapter.validate_python(data)
     except (TypeError, ValidationError) as exc:
         try:
             _deserialized = type_adapter.validate_python(
                 data, strict=False, context={"skip_validation": True}
             )
             log.warning(
-                "Failed to deserialize response into class %s, using backup non-validating deserializer instead.",
+                "Failed to deserialize response into class %s, "
+                "using backup non-validating deserializer instead.",
                 klass,
                 exc_info=exc,
                 extra={"data": data, "class": klass},
             )
             return _deserialized
         except (TypeError, ValidationError):
             try:
                 _deserialized = _MODEL_TYPE_ADAPTER.validate_python(data)
                 log.warning(
-                    "Failed to deserialize response into class %s, using backup generic model deserializer instead.",
+                    "Failed to deserialize response into class %s, "
+                    "using backup generic model deserializer instead.",
                     klass,
                     exc_info=exc,
                     extra={"data": data, "class": klass},
                 )
                 return _deserialized
             except (TypeError, ValidationError) as exc2:
                 log.warning(
-                    "Failed to deserialize response as a generic Model, returning original data.",
+                    "Failed to deserialize response as a generic Model, "
+                    "returning original data.",
                     exc_info=exc2,
                 )
                 return data
 
 
 def _response_type_for_status_code(
     status_code,
-    response_type: Mapping[str, Type | None] | Type | None,
+    response_type: TypeMapping,
 ):
     status_code_key = str(status_code)
     rt_map = (
         {"2XX": response_type} if not isinstance(response_type, dict) else response_type
     )
     if rt_map is None:
         return _DEFAULT_RESPONSE_TYPE
@@ -369,16 +380,19 @@
                     return_data = _deserialize(_data, response_type)
                 except (TypeError, ValueError):
                     return _data
             else:
                 return_data = response.content  # type: ignore
         elif response_type is None:
             return_data = None
-    finally:
-        return return_data
+    except ResponseNotRead as exc:
+        raise RestResponseError(
+            "Cannot deserialize streaming response as object.", response=response
+        ) from exc
+    return return_data
 
 
 async def _iter_event_stream(
     response: Response,
     response_type: type[T],
     select_path: str = "",
     *,
```

### Comparing `waylay_sdk_core-0.2.1/src/waylay/sdk/auth/__init__.py` & `waylay_sdk_core-0.2.2/src/waylay/sdk/auth/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """Waylay SDK authentication."""
 
+from .exceptions import AuthError
 from .model import (
-    WaylayCredentials,
-    ClientCredentials,
     ApplicationCredentials,
-    TokenCredentials,
+    ClientCredentials,
     NoCredentials,
+    TokenCredentials,
+    WaylayCredentials,
     WaylayToken,
 )
-from .provider import WaylayTokenAuth
 from .parse import parse_credentials
-
-from .exceptions import AuthError
+from .provider import WaylayTokenAuth
 
 __all__ = [
     "WaylayCredentials",
     "ClientCredentials",
     "ApplicationCredentials",
     "TokenCredentials",
     "NoCredentials",
```

### Comparing `waylay_sdk_core-0.2.1/src/waylay/sdk/auth/exceptions.py` & `waylay_sdk_core-0.2.2/src/waylay/sdk/auth/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Auth exception utilities."""
 
 import jose.exceptions as jwt_exc
+
 from ..exceptions import WaylayError
 
 _AUTH_MESSAGE_FOR_EXCEPTON_CLASS = [
     (jwt_exc.JWTClaimsError, "invalid token"),
     (jwt_exc.ExpiredSignatureError, "token expired"),
     (jwt_exc.JWTError, "invalid token"),
     (TypeError, "could not decode token"),
```

### Comparing `waylay_sdk_core-0.2.1/src/waylay/sdk/auth/interactive.py` & `waylay_sdk_core-0.2.2/src/waylay/sdk/auth/interactive.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Interactive authentication callback for client credentials."""
 
-from typing import Optional
+from __future__ import annotations
+
 import logging
 import re
 import urllib.parse
-
 from getpass import getpass
+
 import httpx
 
-from .model import WaylayCredentials, ClientCredentials, AuthError
+from .model import AuthError, ClientCredentials, WaylayCredentials
 
 DEFAULT_GATEWAY_URL = "https://api.waylay.io"
 DEFAULT_ACCOUNTS_URL = "https://accounts-api.waylay.io"
 ACCOUNTS_USERS_ME_PATH = "/accounts/v1/users/me"
 
 _http = httpx
 log = logging.getLogger(__name__)
@@ -29,15 +30,15 @@
 
 
 def ask_secret(prompt: str) -> str:
     """Prompt user for credential information."""
     return getpass(prompt=prompt)
 
 
-def ask_yes_no(prompt: str, default: Optional[bool] = None) -> bool:
+def ask_yes_no(prompt: str, default: bool | None = None) -> bool:
     """Keep prompting the user until response starts with a true or false character."""
     while True:
         resp = ask(prompt)
         if not resp and default is not None:
             return default
         resp_char = resp.lower()[0]
         if resp_char in ("n", "f"):
@@ -57,15 +58,16 @@
             """Examples:
     'enterprise' (or 'api.waylay.io') for the Enterprise platform,
     'https://waylay-api.mycompany.com' as a custom endpoint url
         """
         )
         gateway_url = (
             ask(
-                f"> Press enter to confirm, or specify an alternate gateway [{gateway_url}]: "
+                "> Press enter to confirm, "
+                f"or specify an alternate gateway [{gateway_url}]: "
             )
             or gateway_url
         )
         gateway_url = _gateway_url_for(gateway_url)
         try:
             gateway_status_resp = _http.get(f"{gateway_url}{ACCOUNTS_USERS_ME_PATH}")
         except Exception as err:
```

### Comparing `waylay_sdk_core-0.2.1/src/waylay/sdk/auth/model.py` & `waylay_sdk_core-0.2.2/src/waylay/sdk/auth/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """Utilities to handle waylay authentication."""
 
-from datetime import datetime
-from enum import Enum
-from dataclasses import dataclass
-from typing import Optional, ClassVar, Dict, Any, List
-import json
-import abc
+from __future__ import annotations
 
+import abc
 import base64
 import binascii
-from jose import jwt, JWTError
+import json
+from dataclasses import dataclass
+from datetime import datetime
+from enum import Enum
+from typing import Any, ClassVar, Dict, List
+
+from jose import JWTError, jwt
 
-from .exceptions import TokenParseError, AuthError
+from .exceptions import AuthError, TokenParseError
 
 
 class CredentialsType(str, Enum):
     """Supported Waylay Authentication Methods.
 
     Note that username/password authentication (as used in our IDP at
     https://login.waylay.io)
@@ -35,26 +37,27 @@
 
 TokenString = str
 
 
 class WaylayCredentials(abc.ABC):
     """Base class for the representation of credentials to the waylay platform."""
 
-    gateway_url: Optional[str] = None
+    gateway_url: str | None = None
     credentials_type: ClassVar[CredentialsType] = CredentialsType.CALLBACK
 
     # legacy
-    accounts_url: Optional[str] = None
+    accounts_url: str | None = None
 
     @abc.abstractmethod
     def to_dict(self, obfuscate=True) -> Dict[str, Any]:
         """Convert the credentials to a json-serialisable representation."""
 
-    @abc.abstractproperty
-    def id(self) -> Optional[str]:
+    @property
+    @abc.abstractmethod
+    def id(self) -> str | None:
         """Get the main identifier for this credential."""
         return None
 
     def __repr__(self):
         """Show the implementing class and public information."""
         return f"<{self.__class__.__name__}({str(self)})>"
 
@@ -69,67 +72,67 @@
         This does not assure that they will lead to a succesfull
         authentication.
 
         """
 
 
 @dataclass(repr=False)
-class AccountsUrlMixin:
+class CredentialsBase(WaylayCredentials):
     """Dataclass mixin for the 'gateway_url' (legacy 'accounts_url') property."""
 
-    gateway_url: Optional[str] = None
-    accounts_url: Optional[str] = None
+    gateway_url: str | None = None
+    accounts_url: str | None = None
 
 
 @dataclass(repr=False, init=False)
-class ApiKeySecretMixin(AccountsUrlMixin):
+class KeySecretCredentials(CredentialsBase):
     """Dataclass mixin for the 'api_key' and 'api_secret'."""
 
     api_key: str = ""
     api_secret: str = ""
 
     def __init__(
         self,
         api_key: str,
         api_secret: str,
         *,
-        gateway_url: Optional[str] = None,
-        accounts_url: Optional[str] = None,
+        gateway_url: str | None = None,
+        accounts_url: str | None = None,
     ):
         """Initialise with the api_key and api_secret."""
         super().__init__(gateway_url=gateway_url, accounts_url=accounts_url)
         self.api_key = api_key
         self.api_secret = api_secret
 
     @property
-    def id(self) -> Optional[str]:
+    def id(self) -> str | None:
         """Get the main identifier for this credential."""
         return self.api_key
 
     @classmethod
     def create(
         cls,
         api_key: str,
         api_secret: str,
         *,
-        gateway_url: Optional[str] = None,
-        accounts_url: Optional[str] = None,
+        gateway_url: str | None = None,
+        accounts_url: str | None = None,
     ):
         """Create a client credentials object."""
         return cls(
             api_key=api_key,
             api_secret=api_secret,
             gateway_url=gateway_url,
             accounts_url=accounts_url,
         )
 
     def to_dict(self, obfuscate=True):
         """Convert the credentials to a json-serialisable representation."""
         return dict(
-            type=self.credentials_type.value,
+            type=self.credentials_type.value,  # type: ignore
             api_key=self.api_key,
             api_secret="********" if obfuscate else self.api_secret,
             gateway_url=self.gateway_url,
             accounts_url=self.accounts_url,
         )
 
     def is_well_formed(self) -> bool:
@@ -153,16 +156,16 @@
                 return False
         except binascii.Error:
             return False
         return True
 
 
 @dataclass(repr=False, init=False)
-class NoCredentials(AccountsUrlMixin, WaylayCredentials):
-    """Represents credentials which be asked via (interactive) callback when required."""
+class NoCredentials(CredentialsBase):
+    """Credentials that be resolved via (interactive) callback when required."""
 
     credentials_type: ClassVar[CredentialsType] = CredentialsType.CALLBACK
 
     def to_dict(self, obfuscate=True):  # pylint: disable=unused-argument
         """Convert the credentials to a json-serialisable representation."""
         return dict(
             type=str(self.credentials_type),
@@ -171,54 +174,75 @@
         )
 
     def is_well_formed(self) -> bool:
         """Validate that these credentials are well-formed."""
         return True
 
     @property
-    def id(self) -> Optional[str]:
+    def id(self) -> str | None:
         """Get the main identifier for this credential."""
         return None
 
 
 @dataclass(repr=False, init=False)
-class ClientCredentials(ApiKeySecretMixin, WaylayCredentials):
+class ClientCredentials(KeySecretCredentials):
     """Waylay Credentials: api key and secret of type 'client_credentials'."""
 
     credentials_type: ClassVar[CredentialsType] = CredentialsType.CLIENT
 
 
 @dataclass(repr=False, init=False)
-class ApplicationCredentials(ApiKeySecretMixin, WaylayCredentials):
+class ApplicationCredentials(KeySecretCredentials):
     """Waylay Credentials: api key and secret of type 'application_credentials'."""
 
     credentials_type: ClassVar[CredentialsType] = CredentialsType.APPLICATION
     tenant_id: str = ""
 
+    def __init__(
+        self,
+        api_key: str,
+        api_secret: str,
+        tenant_id: str,
+        *,
+        gateway_url: str | None = None,
+        accounts_url: str | None = None,
+    ):
+        """Initialise with the api_key and api_secret."""
+        super().__init__(
+            api_key, api_secret, gateway_url=gateway_url, accounts_url=accounts_url
+        )
+        self.tenant_id = tenant_id
+
+    def to_dict(self, obfuscate=True):
+        """Get the dict representation."""
+        _dict = super().to_dict(obfuscate)
+        _dict["tenant_id"] = self.tenant_id
+        return _dict
+
 
 @dataclass(repr=False, init=False)
-class TokenCredentials(AccountsUrlMixin, WaylayCredentials):
+class TokenCredentials(CredentialsBase):
     """Waylay JWT Token credentials."""
 
     credentials_type: ClassVar[CredentialsType] = CredentialsType.TOKEN
     token: TokenString = ""
 
     def __init__(
         self,
         token: TokenString,
         *,
-        gateway_url: Optional[str] = None,
-        accounts_url: Optional[str] = None,
+        gateway_url: str | None = None,
+        accounts_url: str | None = None,
     ):
         """Create a TokenCredentials from a token string."""
         super().__init__(gateway_url=gateway_url, accounts_url=accounts_url)
         self.token = token
 
     @property
-    def id(self) -> Optional[str]:
+    def id(self) -> str | None:
         """Get the main identifier for this credential."""
         try:
             token = WaylayToken(self.token)
             return f"[{token.domain}] {token.subject}"
         except AuthError as exc:
             return f"INVALID_TOKEN({exc})"
 
@@ -239,15 +263,15 @@
         except TokenParseError:
             return False
 
 
 class WaylayToken:
     """Holds a Waylay JWT token."""
 
-    def __init__(self, token_string: str, token_data: Optional[Dict] = None):
+    def __init__(self, token_string: str, token_data: Dict | None = None):
         """Create a Waylay Token holder object from given token string or data."""
         self.token_string = token_string
         if token_data is None:
             try:
                 token_data = jwt.decode(
                     token_string, "", options=dict(verify_signature=False)
                 )
@@ -273,25 +297,25 @@
 
         # assert expiry
         if self.is_expired:
             raise AuthError("token expired")
         return self
 
     @property
-    def tenant(self) -> Optional[str]:
+    def tenant(self) -> str | None:
         """Get the tenant id asserted by the token."""
         return self.token_data.get("tenant", None)
 
     @property
-    def domain(self) -> Optional[str]:
+    def domain(self) -> str | None:
         """Get the waylay domain asserted by the token."""
         return self.token_data.get("domain", None)
 
     @property
-    def subject(self) -> Optional[str]:
+    def subject(self) -> str | None:
         """Get the subject asserted by the token."""
         return self.token_data.get("sub", None)
 
     @property
     def licenses(self) -> List[str]:
         """Get the licenses asserted by the token."""
         return self.token_data.get("licenses", [])
@@ -303,21 +327,21 @@
 
     @property
     def permissions(self) -> List[str]:
         """Get the permissions asserted by the token."""
         return self.token_data.get("permissions", [])
 
     @property
-    def expires_at(self) -> Optional[datetime]:
+    def expires_at(self) -> datetime | None:
         """Get the token expiry timestamp."""
         exp = self.token_data.get("exp", None)
         return None if exp is None else datetime.fromtimestamp(exp)
 
     @property
-    def issued_at(self) -> Optional[datetime]:
+    def issued_at(self) -> datetime | None:
         """Get the token issuance timestamp."""
         iat = self.token_data.get("iat", None)
         return None if iat is None else datetime.fromtimestamp(iat)
 
     @property
     def expires_seconds(self) -> int:
         """Get seconds until expiry."""
```

### Comparing `waylay_sdk_core-0.2.1/src/waylay/sdk/auth/parse.py` & `waylay_sdk_core-0.2.2/src/waylay/sdk/auth/parse.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Parse credentials."""
 
-from typing import Dict, Any
+from typing import Any, Dict
 
 from .model import (
-    NoCredentials,
-    ClientCredentials,
-    WaylayCredentials,
     ApplicationCredentials,
+    ClientCredentials,
+    NoCredentials,
     TokenCredentials,
+    WaylayCredentials,
 )
 
 
 def parse_credentials(json_obj: Dict[str, Any]) -> WaylayCredentials:
     """Convert a parsed json representation to a WaylayCredentials object."""
-    cred_type = json_obj.get("type", None)
+    cred_type = json_obj.get("type")
     if cred_type is None:
         raise ValueError("invalid json for credentials: missing type")
 
     for clz in [
         NoCredentials,
         ClientCredentials,
         ApplicationCredentials,
```

### Comparing `waylay_sdk_core-0.2.1/src/waylay/sdk/client.py` & `waylay_sdk_core-0.2.2/src/waylay/sdk/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """REST client for the Waylay Platform."""
 
 from __future__ import annotations
-from typing import TYPE_CHECKING, Optional
+
+from typing import TYPE_CHECKING
 
 from waylay.sdk.services.gateway import GatewayService
 
-from .plugin.client import WithServicesAndTools
-from .config.client import WaylayConfig, WithConfig, HttpClientOptions
 from .api import ApiClient
 from .api.http import AsyncClient
-
+from .config.client import HttpClientOptions, WaylayConfig, WithConfig
+from .plugin.client import WithServicesAndTools
 
 if TYPE_CHECKING:
     from .plugin.type_stubs import (
         AlarmsService,
         DataService,
         RegistryService,
         ResourcesService,
@@ -22,26 +22,26 @@
     )
 
 
 class WaylayClient(WithConfig, WithServicesAndTools):
     """REST client for the Waylay Platform."""
 
     gateway: GatewayService
-    alarms: "AlarmsService"
-    data: "DataService"
-    registry: "RegistryService"
-    resources: "ResourcesService"
-    rules: "RulesService"
-    storage: "StorageService"
+    alarms: AlarmsService
+    data: DataService
+    registry: RegistryService
+    resources: ResourcesService
+    rules: RulesService
+    storage: StorageService
 
     def __init__(
         self,
         config: WaylayConfig | ApiClient,
         /,
-        options: Optional[HttpClientOptions | AsyncClient] = None,
+        options: HttpClientOptions | AsyncClient | None = None,
     ):
         """Create a WaylayConfig instance."""
         client_config: WaylayConfig
         api_client: ApiClient
         if isinstance(config, ApiClient):
             api_client = config
             client_config = api_client.config
```

### Comparing `waylay_sdk_core-0.2.1/src/waylay/sdk/config/client.py` & `waylay_sdk_core-0.2.2/src/waylay/sdk/config/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 """Config mixin for the SDK client."""
 
 from __future__ import annotations
-from typing import Optional
 
+from ..api import AsyncClient, HttpClientOptions
 from ..auth import (
-    WaylayCredentials,
     ClientCredentials,
     TokenCredentials,
+    WaylayCredentials,
 )
-
 from .model import (
-    WaylayConfig,
-    TenantSettings,
     DEFAULT_PROFILE,
-    SERVICE_KEY_GATEWAY,
     SERVICE_KEY_ACCOUNTS,
+    SERVICE_KEY_GATEWAY,
+    TenantSettings,
+    WaylayConfig,
 )
-from ..api import HttpClientOptions, AsyncClient
 
 
 class WithConfig:
     """A configuration Mixin."""
 
     config: WaylayConfig
     http_options: HttpClientOptions
@@ -32,15 +30,15 @@
     @classmethod
     def from_profile(
         cls,
         profile: str = DEFAULT_PROFILE,
         *,
         interactive=True,
         gateway_url=None,
-        options: Optional[HttpClientOptions | AsyncClient] = None,
+        options: HttpClientOptions | AsyncClient | None = None,
     ):
         """Create a WaylayClient named profile.
 
         Uses credentials from environment variables or a locally stored
         configuration.
 
         """
@@ -55,56 +53,56 @@
     def from_client_credentials(
         cls,
         api_key: str,
         api_secret: str,
         *,
         gateway_url=None,
         accounts_url=None,
-        settings: Optional[TenantSettings] = None,
-        options: Optional[HttpClientOptions | AsyncClient] = None,
+        settings: TenantSettings | None = None,
+        options: HttpClientOptions | AsyncClient | None = None,
     ):
         """Create a WaylayClient using the given client credentials."""
         credentials = ClientCredentials(
             api_key, api_secret, **_auth_urls(gateway_url, accounts_url, settings)
         )
         return cls.from_credentials(credentials, settings=settings, options=options)
 
     @classmethod
     def from_token(
         cls,
         token_string: str,
         *,
         gateway_url=None,
         accounts_url=None,
-        settings: Optional[TenantSettings] = None,
-        options: Optional[HttpClientOptions | AsyncClient] = None,
+        settings: TenantSettings | None = None,
+        options: HttpClientOptions | AsyncClient | None = None,
     ):
         """Create a WaylayClient using a waylay token."""
         credentials = TokenCredentials(
             token_string, **_auth_urls(gateway_url, accounts_url, settings)
         )
         return cls.from_credentials(credentials, settings=settings, options=options)
 
     @classmethod
     def from_credentials(
         cls,
         credentials: WaylayCredentials,
-        settings: Optional[TenantSettings] = None,
-        options: Optional[HttpClientOptions | AsyncClient] = None,
+        settings: TenantSettings | None = None,
+        options: HttpClientOptions | AsyncClient | None = None,
     ):
         """Create a WaylayClient using the given client credentials."""
         return cls(
             WaylayConfig(
                 credentials,
                 settings=settings,
             ),
             options=options,
         )
 
 
 def _auth_urls(
-    gateway_url=None, accounts_url=None, settings: Optional[TenantSettings] = None
+    gateway_url=None, accounts_url=None, settings: TenantSettings | None = None
 ):
     if settings:
         gateway_url = gateway_url or settings.get(SERVICE_KEY_GATEWAY)
         accounts_url = accounts_url or settings.get(SERVICE_KEY_ACCOUNTS)
     return {"gateway_url": gateway_url, "accounts_url": accounts_url}
```

### Comparing `waylay_sdk_core-0.2.1/src/waylay/sdk/config/model.py` & `waylay_sdk_core-0.2.2/src/waylay/sdk/config/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 """Client configuration."""
 
-from typing import Optional, Mapping, MutableMapping, Any, Type
+from __future__ import annotations
+
+import json
+import logging
 import os
 import re
+from collections.abc import Mapping, MutableMapping
 from pathlib import Path
-import json
-import logging
+from typing import Any, Type
+
 import httpx
 from appdirs import user_config_dir
+
 from ..auth import (
-    WaylayCredentials,
+    AuthError,
     NoCredentials,
+    WaylayCredentials,
     WaylayToken,
     parse_credentials,
-    AuthError,
-)
-from ..auth.provider import (
-    WaylayTokenAuth,
-    CredentialsCallback,
 )
 from ..auth.interactive import (
     DEFAULT_GATEWAY_URL,
+    _root_url_for,
     ask_gateway,
     request_client_credentials_interactive,
     request_migrate_to_gateway_interactive,
     request_store_config_interactive,
-    _root_url_for,
+)
+from ..auth.provider import (
+    CredentialsCallback,
+    WaylayTokenAuth,
 )
 from ..exceptions import ConfigError
 
 log = logging.getLogger(__name__)
 
 # http client dependencies
 _http = httpx
@@ -40,39 +45,38 @@
 
 
 TenantSettings = Mapping[str, str]
 
 Settings = MutableMapping[str, str]
 
 DEFAULT_PROFILE = "_default_"
-SERVICE_KEY_API = "waylay_api"
 SERVICE_KEY_GATEWAY = "waylay_gateway"
 SERVICE_KEY_ACCOUNTS = "waylay_accounts"
 DEFAULT_DOC_URL: str = "https://docs.waylay.io/#"
 DEFAULT_APIDOC_URL: str = "https://docs.waylay.io/openapi/public/redocly"
 DOC_URL_KEY: str = "doc_url"
 APIDOC_URL_KEY: str = "apidoc_url"
 
 
 class WaylayConfig:
     """Manages the authentication and endpoint configuration for the Waylay Platform."""
 
     profile: str
     _auth: WaylayTokenAuth
     _local_settings: Settings
-    _tenant_settings: Optional[TenantSettings] = None
+    _tenant_settings: TenantSettings | None = None
     _token_auth_provider: Type[WaylayTokenAuth] = WaylayTokenAuth
 
     def __init__(
         self,
-        credentials: Optional[WaylayCredentials] = None,
+        credentials: WaylayCredentials | None = None,
         profile: str = DEFAULT_PROFILE,
-        settings: Optional[TenantSettings] = None,
+        settings: TenantSettings | None = None,
         fetch_tenant_settings=True,
-        credentials_callback: Optional[CredentialsCallback] = None,
+        credentials_callback: CredentialsCallback | None = None,
     ):
         """Create a WaylayConfig."""
         self.profile = profile
         if credentials is None:
             credentials = NoCredentials()
         self._local_settings = {}
         if settings:
@@ -92,63 +96,59 @@
         """
         return self._auth.credentials
 
     def get_root_url(
         self,
         config_key: str,
         *,
-        default_root_url: Optional[str] = None,
-        gateway_root_path: Optional[str] = None,
+        default_root_url: str | None = None,
+        gateway_root_path: str | None = None,
         default_root_path: str = "",
         resolve_settings: bool = True,
-    ) -> Optional[str]:
+    ) -> str | None:
         """Get the root url for a waylay service."""
         config_key = _root_url_key_for(config_key)
         # only resolve remote settings if no gateway available
         use_gateway = gateway_root_path is not None and self.gateway_url is not None
         default_url = (
             f"{self.gateway_url}{gateway_root_path}"
             if use_gateway
             else default_root_url
         )
         settings = self.local_settings
         if not use_gateway:
             resolve_settings = (
                 resolve_settings
                 # do not lookup settings for the bootstrap services
-                and config_key not in (SERVICE_KEY_ACCOUNTS, SERVICE_KEY_API)
+                and config_key not in (SERVICE_KEY_ACCOUNTS)
             )
             settings = self.get_settings(resolve=resolve_settings)
         url_override = settings.get(config_key)
         if url_override is not None:
             url_override = _root_url_for(url_override)
             if url_override.endswith(default_root_path):
                 return url_override
             else:
                 return f"{url_override}{default_root_path}"
         if default_url is not None:
             return _root_url_for(default_url)
-        if config_key == SERVICE_KEY_API:
-            domain = self.get_valid_token().domain
-            if domain:
-                return f"{_root_url_for(domain)}/api"
         return None
 
-    def set_root_url(self, config_key: str, root_url: Optional[str]):
+    def set_root_url(self, config_key: str, root_url: str | None):
         """Override the root url for the given server.
 
         Will persist on `save`.
         Setting a `None` value will remove the override.
 
         """
         config_key = _root_url_key_for(config_key)
         self.set_local_settings(**{config_key: root_url})
 
     @property
-    def accounts_url(self) -> Optional[str]:
+    def accounts_url(self) -> str | None:
         """Get the accounts url."""
         url = self.credentials.accounts_url
         return _root_url_for(url) if url else None
 
     @property
     def gateway_url(self):
         """Get the gateway url."""
@@ -184,15 +184,15 @@
 
         These include the endpoint overrides that are stored with the
         profile.
 
         """
         return self._local_settings
 
-    def set_local_settings(self, **settings: Optional[str]) -> TenantSettings:
+    def set_local_settings(self, **settings: str | None) -> TenantSettings:
         """Set a local endpoint url override for a service."""
         for config_key, value in settings.items():
             if value is None and config_key in self._local_settings:
                 del self._local_settings[config_key]
             if value is not None:
                 self._local_settings[config_key] = value
         return self.local_settings
@@ -211,37 +211,29 @@
 
         """
         return {
             **(self.tenant_settings if resolve else self._tenant_settings or {}),
             **self.local_settings,
         }
 
-    def get_valid_token(self) -> WaylayToken:
+    async def get_valid_token(self) -> WaylayToken:
         """Get the current valid authentication token or fail."""
         if isinstance(self.auth, WaylayTokenAuth):
             try:
-                return self.auth.assure_valid_token()
+                return await self.auth.assure_valid_token_async()
             except AuthError as exc:
                 raise ConfigError(f"Cannot get valid token: {exc}") from exc
         raise ConfigError("not using token authentication")  # pragma: no cover
 
     @property
     def auth(self) -> _http.Auth:
         """Get the current http authentication interceptor."""
         return self._auth
 
     @property
-    def domain(self) -> Optional[str]:
-        """Get the Waylay domain of the current user."""
-        try:
-            return self.get_valid_token().domain
-        except ConfigError:
-            return None
-
-    @property
     def global_settings_url(self) -> str:
         """Get the REST url that fetches global settings."""
         root_url = self.get_root_url(
             "api",
             default_root_url=None,
             gateway_root_path="/configs/v1",
             resolve_settings=False,
@@ -291,21 +283,22 @@
         interactive: bool = True,
         skip_error: bool = False,
         gateway_url: str = DEFAULT_GATEWAY_URL,
     ):
         """Load a stored waylay configuration."""
         profile = DEFAULT_PROFILE if profile is None else profile
         try:
-            with open(
-                cls.config_file_path(profile), mode="r", encoding="utf-8"
-            ) as config_file:
+            with open(cls.config_file_path(profile), encoding="utf-8") as config_file:
                 config_json = json.load(config_file)
             waylay_config = cls.from_dict(config_json)
             if not waylay_config.gateway_url:
-                msg = f"WaylayConfig profile '{profile}' uses a legacy accounts endpoint {waylay_config.accounts_url}."
+                msg = (
+                    f"WaylayConfig profile '{profile}' uses a "
+                    f"legacy accounts endpoint {waylay_config.accounts_url}."
+                )
                 if interactive:
                     if request_migrate_to_gateway_interactive(profile, msg):
                         gateway_url = ask_gateway(waylay_config.accounts_url)
                         waylay_config.credentials.gateway_url = gateway_url
                         waylay_config.save()
                 else:
                     log.warning(msg)
```

### Comparing `waylay_sdk_core-0.2.1/src/waylay/sdk/exceptions.py` & `waylay_sdk_core-0.2.2/src/waylay/sdk/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Base exception class hierarchy for errors in the waylay client."""
 
-from typing import Optional
+from __future__ import annotations
+
 from .api.http import Request, Response
 
 
 class WaylayError(Exception):
     """Root class for all exceptions raised by this module."""
 
 
@@ -17,36 +18,38 @@
 
     Notifies errors in tools and utilities that are not directly related
     to a REST call.
     """
 
 
 class RestConnectionError(RequestError):
-    """Exception class for request errors that are caused by client connection errors."""
+    """Exception class for request errors caused by client connection errors."""
 
 
 class RestError(WaylayError):
     """Exception class for failures to make a REST call."""
 
 
 class RestRequestError(RestError):
     """Exception class for failures to prepare a REST call."""
 
-    request: Optional[Request]
+    request: Request | None
 
     def __init__(
         self,
-        request: Optional[Request],
+        *args,
+        request: Request | None = None,
     ):
         """Create an instance."""
+        super().__init__(*args)
         self.request = request
 
     def __str__(self):
         """Get the string representation of the exception."""
-        error_message = f"{self.__class__.__name__}"
+        error_message = super().__str__()
         if self.request is None:
             return error_message
         req = self.request
         error_message += f"\nRequest: {req.method} {req.url}"
         if req.headers:
             error_message += f"\nRequest headers: {req.headers}"
         if hasattr(req, "_content"):
@@ -59,23 +62,24 @@
 class RestResponseError(RestRequestError):
     """Exception class wrapping the response data of a REST call."""
 
     response: Response
 
     def __init__(
         self,
+        *args,
         response: Response,
     ) -> None:
         """Create an instance."""
-        super().__init__(response._request)
+        super().__init__(*args, request=response._request)
         self.response = response
 
     def __str__(self):
         """Get the string representation of the exception."""
-        error_message = super().__str__()
+        error_message = super().__repr__()
         resp = self.response
         error_message += f"\nStatus: {resp.status_code}"
         error_message += f"\nReason: {resp.reason_phrase}"
         if resp.headers:
             error_message += f"\nResponse headers: {resp.headers}"
         if hasattr(self.response, "_content"):
             error_message += f"\nResponse content: <bytes: len={len(resp._content)}>"
@@ -83,8 +87,8 @@
             error_message += (
                 f"\nResponse content: <streaming: len={resp.num_bytes_downloaded}>"
             )
         return error_message
 
 
 class RestResponseParseError(RestResponseError):
-    """Exception raised when a successfull http request (2XX) could not be parsed succesfully."""
+    """Exception raised when a successfull http request (2XX) could not be parsed."""
```

### Comparing `waylay_sdk_core-0.2.1/src/waylay/sdk/plugin/base.py` & `waylay_sdk_core-0.2.2/src/waylay/sdk/plugin/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """Base classes for Waylay SDK Plugins."""
 
-from typing import Iterator, Optional, Generic, Type, TypeVar, Mapping
+from __future__ import annotations
+
+from collections.abc import Iterator, Mapping
+from typing import Generic, Type, TypeVar
+
 from ..api import ApiClient, HttpClientOptions
 from ..api.exceptions import SyncCtxMgtNotSupportedError
 
-
 P = TypeVar("P", bound="WaylayPlugin")
 PI = TypeVar("PI", bound="WaylayPlugin")
 
 
 class WithApiClient:
     """Base Waylay plugin class."""
 
@@ -20,15 +23,15 @@
 
     async def __aenter__(self):
         """Initialize the api client."""
         self(None)
         self.api_client = await self.api_client.__aenter__()
         return self
 
-    def __call__(self, http_options: Optional[HttpClientOptions] = None):
+    def __call__(self, http_options: HttpClientOptions | None = None):
         """Initialize the http client."""
         if self.api_client.is_closed:
             self.api_client.set_options(http_options)
         else:
             # create a new api client.
             # leave the previous client for other services.
             self.api_client = self.api_client.clone(http_options)
@@ -48,15 +51,15 @@
 
 
 class WaylayPlugin(WithApiClient):
     """Plugin for the Waylay SDK client."""
 
     name: str = "__NO_NAME__"
     title: str = "__NO_TITLE__"
-    description: Optional[str] = None
+    description: str | None = None
 
     def __str__(self):
         """Get a plugin descripton."""
         return f"{self.name}: {self.title}"
 
     def __repr__(self):
         """Get a plugin representation."""
@@ -85,30 +88,30 @@
         """Iterate SDK plugin keys."""
         return self._items.__iter__()
 
     def __len__(self) -> int:
         """Count registred SDK plugin."""
         return self._items.__len__()
 
-    def iter(self, item_class: Type[PI], name: Optional[str] = None) -> Iterator[PI]:
+    def iter(self, item_class: Type[PI], name: str | None = None) -> Iterator[PI]:
         """Iterate over the plugins that satisfy the requirements."""
         if name:
             plug = self._items.get(name, None)
             if isinstance(plug, item_class):
                 yield plug
             return
         for plug in self._items.values():
             if isinstance(plug, item_class):
                 yield plug
 
-    def select(self, item_class: Type[PI], name: Optional[str] = None) -> Optional[PI]:
+    def select(self, item_class: Type[PI], name: str | None = None) -> PI | None:
         """Select the first SDK plugin that satifies the class and name requirements."""
         return next(self.iter(item_class, name), None)
 
-    def require(self, item_class: Type[PI], name: Optional[str] = None) -> PI:
+    def require(self, item_class: Type[PI], name: str | None = None) -> PI:
         """Get the SDK plugin for the given class or raise a ConfigError."""
         item = self.select(item_class, name)
         if item is None:
             info = f"{item_class.__name__} '{name}'" if name else item_class.__name__
             raise AttributeError(f"{info} is not available.")
         return item
 
@@ -126,14 +129,15 @@
 
     _services: PluginAccess[WaylayService]
     _tools: "PluginAccess[WaylayTool]"
 
     def __init__(
         self,
         api_client: ApiClient,
+        *,
         services: PluginAccess[WaylayService],
         tools: "PluginAccess[WaylayTool]",
     ):
         """Create a Waylay Tool."""
         super().__init__(api_client)
         self._services = services
         self._tools = tools
```

### Comparing `waylay_sdk_core-0.2.1/src/waylay/sdk/plugin/client.py` & `waylay_sdk_core-0.2.2/src/waylay/sdk/plugin/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Client mixin for plugins."""
 
+from __future__ import annotations
+
 import sys
-from typing import Type, Dict, Optional
-from importlib.metadata import entry_points
 import warnings
+from importlib.metadata import entry_points
+from typing import Dict, Type
 
-from .base import WaylayService, WaylayTool, WithApiClient, WaylayPlugin, PluginAccess
 from ..api import ApiClient
+from .base import PluginAccess, WaylayPlugin, WaylayService, WaylayTool, WithApiClient
 
 
 class WithServicesAndTools(WithApiClient):
     """Client as loader of service and tool plugins."""
 
     services: PluginAccess[WaylayService]
     tools: PluginAccess[WaylayTool]
@@ -35,29 +37,29 @@
             waylay_entry_points = [
                 ep for ep in entry_points().get(ep_group, []) if ep.name == ep_name
             ]
         for ep in waylay_entry_points:
             for plugin_class in ep.load():
                 self.register(plugin_class)
 
-    def register(self, plugin_class: Type[WaylayPlugin]) -> Optional[WaylayPlugin]:
+    def register(self, plugin_class: Type[WaylayPlugin]) -> WaylayPlugin | None:
         """Register and instantiate plugin class."""
         if issubclass(plugin_class, WaylayService):
             service = plugin_class(self.api_client)
             self._services[service.name] = service
             return service
         if issubclass(plugin_class, WaylayTool):
             tool = plugin_class(
                 self.api_client,
                 services=self.services,
                 tools=self.tools,
             )
             self._tools[tool.name] = tool
             return tool
-        warnings.warn(f"Invalid plug class: {plugin_class}")
+        warnings.warn(message=f"Invalid plug class: {plugin_class}", stacklevel=1)
         return None
 
     def __getattr__(self, name: str):
         """Get plugin by name."""
         if name in self._services:
             return self._services[name]
         if name in self._tools:
```

### Comparing `waylay_sdk_core-0.2.1/src/waylay/sdk/plugin/type_stubs.py` & `waylay_sdk_core-0.2.2/src/waylay/sdk/plugin/type_stubs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Type imports for known services."""
 
 from typing import TYPE_CHECKING
+
 from .base import WaylayService
 
 
 class _WaylayServiceStub(WaylayService):
     """Dummy Waylay service stub."""
 
     def __getattr__(self, name):
```

### Comparing `waylay_sdk_core-0.2.1/src/waylay/sdk/services/gateway.py` & `waylay_sdk_core-0.2.2/src/waylay/sdk/services/gateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """Gateway Service."""
 
 from __future__ import annotations
 
 from typing import Any, Dict, Literal, TypeVar, overload
+
 from pydantic import ConfigDict
 
+from waylay.sdk.api._models import BaseModel as WaylayBaseModel
+from waylay.sdk.api._models import Model
 from waylay.sdk.api.client import ApiClient
 from waylay.sdk.api.http import HeaderTypes, QueryParamTypes, Response
 from waylay.sdk.plugin.base import WaylayService, WithApiClient
-from waylay.sdk.api._models import BaseModel as WaylayBaseModel, Model
 
 T = TypeVar("T")
 
 
 class GatewayService(WaylayService):
     """Gateway Service Class."""
 
@@ -100,34 +102,38 @@
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> GatewayResponse | T | Response | Model:
         """Get the status of the gateway.
 
         :param query: URL Query parameters.
         :type query: QueryParamTypes, optional
-        :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
-        :param select_path: Denotes the json path applied to the response object before returning it.
-                Set it to the empty string `""` to receive the full response object.
-        :param response_type: If specified, the response is parsed into an instance of the specified type.
+        :param raw_response: If true, return the http Response object instead of
+            returning an api model object, or throwing an ApiError.
+        :param select_path: Denotes the json path applied to the response
+            object before returning it.
+            Set it to the empty string `""` to receive the full response object.
+        :param response_type: If specified, the response is parsed into
+            an instance of the specified type.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
             * stream: if true, the response will be in streaming mode
             * cookies
             * extensions
             * auth
             * follow_redirects: bool
 
-        :return: Returns the result object if the http request succeeded with status code '2XX'.
-        :raises APIError: If the http request has a status code different from `2XX`. This
-            object wraps both the http Response and any parsed data.
+        :return: Returns the result object if the http request succeeded
+            with status code '2XX'.
+        :raises APIError: If the http request has a status code different from `2XX`.
+            This object wraps both the http Response and any parsed data.
         """
         response_type_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": GatewayResponse if not select_path else Model,
             }
```

### Comparing `waylay_sdk_core-0.2.1/src/waylay_sdk_core.egg-info/PKG-INFO` & `waylay_sdk_core-0.2.2/src/waylay_sdk_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-core
-Version: 0.2.1
+Version: 0.2.2
 Summary: Waylay Python SDK.
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
-        Copyright 2020, Waylay
+        Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
         and this permission notice appear in all copies.
         
         THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH 
         REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND 
@@ -43,15 +43,14 @@
 Requires-Dist: starlette; extra == "dev"
 Requires-Dist: syrupy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
 Requires-Dist: types-appdirs; extra == "dev"
 Requires-Dist: types-python-dateutil; extra == "dev"
-Requires-Dist: docformatter; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: sse-starlette; extra == "dev"
 
 # Waylay Python SDK
 
 Python SDK for the Waylay Platform.
```

### Comparing `waylay_sdk_core-0.2.1/src/waylay_sdk_core.egg-info/SOURCES.txt` & `waylay_sdk_core-0.2.2/src/waylay_sdk_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

