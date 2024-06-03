# Comparing `tmp/audiconnectpy-2.2.9.tar.gz` & `tmp/audiconnectpy-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiconnectpy-2.2.9.tar", last modified: Sun Jun  2 17:52:12 2024, max compression
+gzip compressed data, was "audiconnectpy-2.3.0.tar", last modified: Mon Jun  3 07:11:35 2024, max compression
```

## Comparing `audiconnectpy-2.2.9.tar` & `audiconnectpy-2.3.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:52:12.843371 audiconnectpy-2.2.9/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:52:12.835370 audiconnectpy-2.2.9/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-06-02 17:52:02.000000 audiconnectpy-2.2.9/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:52:12.839370 audiconnectpy-2.2.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-06-02 17:52:02.000000 audiconnectpy-2.2.9/.github/workflows/auto-approve.yml
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-06-02 17:52:02.000000 audiconnectpy-2.2.9/.github/workflows/pythonpackage.yml
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-06-02 17:52:02.000000 audiconnectpy-2.2.9/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-06-02 17:52:02.000000 audiconnectpy-2.2.9/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-06-02 17:52:02.000000 audiconnectpy-2.2.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-06-02 17:52:02.000000 audiconnectpy-2.2.9/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:52:12.839370 audiconnectpy-2.2.9/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-06-02 17:52:02.000000 audiconnectpy-2.2.9/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-02 17:52:02.000000 audiconnectpy-2.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-06-02 17:52:02.000000 audiconnectpy-2.2.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-06-02 17:52:12.843371 audiconnectpy-2.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-06-02 17:52:02.000000 audiconnectpy-2.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:52:12.839370 audiconnectpy-2.2.9/audiconnectpy/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-06-02 17:52:02.000000 audiconnectpy-2.2.9/audiconnectpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-06-02 17:52:02.000000 audiconnectpy-2.2.9/audiconnectpy/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    23465 2024-06-02 17:52:02.000000 audiconnectpy-2.2.9/audiconnectpy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-06-02 17:52:02.000000 audiconnectpy-2.2.9/audiconnectpy/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-06-02 17:52:02.000000 audiconnectpy-2.2.9/audiconnectpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-06-02 17:52:02.000000 audiconnectpy-2.2.9/audiconnectpy/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11853 2024-06-02 17:52:02.000000 audiconnectpy-2.2.9/audiconnectpy/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    26587 2024-06-02 17:52:02.000000 audiconnectpy-2.2.9/audiconnectpy/vehicle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:52:12.843371 audiconnectpy-2.2.9/audiconnectpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-06-02 17:52:12.000000 audiconnectpy-2.2.9/audiconnectpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-06-02 17:52:12.000000 audiconnectpy-2.2.9/audiconnectpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 17:52:12.000000 audiconnectpy-2.2.9/audiconnectpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 17:52:12.000000 audiconnectpy-2.2.9/audiconnectpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-06-02 17:52:12.000000 audiconnectpy-2.2.9/audiconnectpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-02 17:52:12.000000 audiconnectpy-2.2.9/audiconnectpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-06-02 17:52:02.000000 audiconnectpy-2.2.9/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-06-02 17:52:02.000000 audiconnectpy-2.2.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-06-02 17:52:02.000000 audiconnectpy-2.2.9/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-02 17:52:02.000000 audiconnectpy-2.2.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 17:52:12.843371 audiconnectpy-2.2.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:52:12.839370 audiconnectpy-2.2.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-06-02 17:52:02.000000 audiconnectpy-2.2.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-06-02 17:52:02.000000 audiconnectpy-2.2.9/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:52:12.843371 audiconnectpy-2.2.9/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-06-02 17:52:02.000000 audiconnectpy-2.2.9/tests/fixtures/audi0.json
--rw-r--r--   0 runner    (1001) docker     (127)    10852 2024-06-02 17:52:02.000000 audiconnectpy-2.2.9/tests/fixtures/audi1.json
--rw-r--r--   0 runner    (1001) docker     (127)    11886 2024-06-02 17:52:02.000000 audiconnectpy-2.2.9/tests/fixtures/audi2.json
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-06-02 17:52:02.000000 audiconnectpy-2.2.9/tests/fixtures/info_vehicles.json
--rw-r--r--   0 runner    (1001) docker     (127)    62872 2024-06-02 17:52:02.000000 audiconnectpy-2.2.9/tests/fixtures/location.json
--rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-06-02 17:52:02.000000 audiconnectpy-2.2.9/tests/test_home.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:11:35.099592 audiconnectpy-2.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:11:35.095592 audiconnectpy-2.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-06-03 07:11:25.000000 audiconnectpy-2.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:11:35.095592 audiconnectpy-2.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-06-03 07:11:25.000000 audiconnectpy-2.3.0/.github/workflows/auto-approve.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-06-03 07:11:25.000000 audiconnectpy-2.3.0/.github/workflows/pythonpackage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-06-03 07:11:25.000000 audiconnectpy-2.3.0/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-06-03 07:11:25.000000 audiconnectpy-2.3.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-06-03 07:11:25.000000 audiconnectpy-2.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-06-03 07:11:25.000000 audiconnectpy-2.3.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:11:35.095592 audiconnectpy-2.3.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-06-03 07:11:25.000000 audiconnectpy-2.3.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-03 07:11:25.000000 audiconnectpy-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-06-03 07:11:25.000000 audiconnectpy-2.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-06-03 07:11:35.099592 audiconnectpy-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-06-03 07:11:25.000000 audiconnectpy-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:11:35.095592 audiconnectpy-2.3.0/audiconnectpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-06-03 07:11:25.000000 audiconnectpy-2.3.0/audiconnectpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-06-03 07:11:25.000000 audiconnectpy-2.3.0/audiconnectpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23557 2024-06-03 07:11:25.000000 audiconnectpy-2.3.0/audiconnectpy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-06-03 07:11:25.000000 audiconnectpy-2.3.0/audiconnectpy/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-06-03 07:11:25.000000 audiconnectpy-2.3.0/audiconnectpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-06-03 07:11:25.000000 audiconnectpy-2.3.0/audiconnectpy/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11853 2024-06-03 07:11:25.000000 audiconnectpy-2.3.0/audiconnectpy/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26587 2024-06-03 07:11:25.000000 audiconnectpy-2.3.0/audiconnectpy/vehicle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:11:35.099592 audiconnectpy-2.3.0/audiconnectpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-06-03 07:11:35.000000 audiconnectpy-2.3.0/audiconnectpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-06-03 07:11:35.000000 audiconnectpy-2.3.0/audiconnectpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 07:11:35.000000 audiconnectpy-2.3.0/audiconnectpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 07:11:34.000000 audiconnectpy-2.3.0/audiconnectpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-06-03 07:11:35.000000 audiconnectpy-2.3.0/audiconnectpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-03 07:11:35.000000 audiconnectpy-2.3.0/audiconnectpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-06-03 07:11:25.000000 audiconnectpy-2.3.0/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-06-03 07:11:25.000000 audiconnectpy-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-06-03 07:11:25.000000 audiconnectpy-2.3.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-03 07:11:25.000000 audiconnectpy-2.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 07:11:35.099592 audiconnectpy-2.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:11:35.099592 audiconnectpy-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-06-03 07:11:25.000000 audiconnectpy-2.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-06-03 07:11:25.000000 audiconnectpy-2.3.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:11:35.099592 audiconnectpy-2.3.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-06-03 07:11:25.000000 audiconnectpy-2.3.0/tests/fixtures/audi0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10852 2024-06-03 07:11:25.000000 audiconnectpy-2.3.0/tests/fixtures/audi1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11886 2024-06-03 07:11:25.000000 audiconnectpy-2.3.0/tests/fixtures/audi2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-06-03 07:11:25.000000 audiconnectpy-2.3.0/tests/fixtures/info_vehicles.json
+-rw-r--r--   0 runner    (1001) docker     (127)    62872 2024-06-03 07:11:25.000000 audiconnectpy-2.3.0/tests/fixtures/location.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-06-03 07:11:25.000000 audiconnectpy-2.3.0/tests/test_home.py
```

### Comparing `audiconnectpy-2.2.9/.github/dependabot.yml` & `audiconnectpy-2.3.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.9/.github/workflows/auto-approve.yml` & `audiconnectpy-2.3.0/.github/workflows/auto-approve.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.9/.github/workflows/pythonpackage.yml` & `audiconnectpy-2.3.0/.github/workflows/pythonpackage.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.9/.github/workflows/pythonpublish.yml` & `audiconnectpy-2.3.0/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.9/.github/workflows/release.yml` & `audiconnectpy-2.3.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.9/.gitignore` & `audiconnectpy-2.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.9/.pre-commit-config.yaml` & `audiconnectpy-2.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.9/LICENSE` & `audiconnectpy-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.9/PKG-INFO` & `audiconnectpy-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 2.2.9
+Version: 2.3.0
 Summary: Provides asynchronous authentication and access to Audi Connect
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: connect,async,audi
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `audiconnectpy-2.2.9/README.md` & `audiconnectpy-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.9/audiconnectpy/api.py` & `audiconnectpy-2.3.0/audiconnectpy/api.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.9/audiconnectpy/auth.py` & `audiconnectpy-2.3.0/audiconnectpy/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,55 +85,57 @@
     ) -> Any:
         """Request url with method."""
         try:
             async with async_timeout.timeout(TIMEOUT):
                 _LOGGER.debug("Request - Header: %s", kwargs.get("headers"))
                 _LOGGER.debug("Request: %s (%s) - %s", url, method, kwargs.get("data"))
                 response = await self._session.request(method, url, **kwargs)
-                contents = (await response.read()).decode("utf8")
+                contents = await response.read()
                 response.raise_for_status()
         except (asyncio.CancelledError, asyncio.TimeoutError) as error:
             raise TimeoutExceededError(
                 "Timeout occurred while connecting to Audi Connect."
             ) from error
         except ClientResponseError as error:
+            message = contents.decode("utf8")
             if "application/json" in response.headers.get("Content-Type", ""):
+                msg = json.loads(message)
+                if "error" in msg:
+                    msg = msg["error"].get("message")
                 raise ServiceNotFoundError(
-                    response.status, json.loads(contents)
+                    "Service not found: %s (%s)", msg, response.status
                 ) from error
-            raise ServiceNotFoundError(response.status, contents) from error
+            raise ServiceNotFoundError(
+                "Service not found: %s (%s)", msg, response.status
+            ) from error
         except (ClientError, socket.gaierror) as error:
             raise HttpRequestError(
                 "Error occurred while communicating with Audi Connect."
             ) from error
 
         _LOGGER.debug("Response - Headers: %s", response.headers)
         _LOGGER.debug("Response: %s (%s)", contents, response.status)
         _LOGGER.debug("---------------------------------------------------------")
 
         if raw_reply and raw_rsp is False:
             return response
 
         if "application/json" in response.headers.get("Content-Type", ""):
             rsp = await response.json()
-            if "error" in rsp:
-                raise AudiException("Failed to fetch %s (%s)", url, rsp["error"])
         elif (
             (headers := kwargs.get("headers"))
             and "application/json" in headers.get("Accept", "")
             and contents == ""
         ):
             _LOGGER.debug("JSON FIX: Accept is JSON but Response is None")
             rsp = {}
         else:
             rsp = await response.text()
 
-        if raw_reply and raw_rsp:
-            return response, rsp
-        return rsp
+        return response, rsp if raw_reply and raw_rsp else rsp
 
     async def async_connect(self, tries: int = 3) -> None:
         """Connect to API."""
         try:
             await self._async_retrieve_url_service()
         except HttpRequestError as error:
             self.binded = False
```

### Comparing `audiconnectpy-2.2.9/audiconnectpy/const.py` & `audiconnectpy-2.3.0/audiconnectpy/const.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.9/audiconnectpy/helpers.py` & `audiconnectpy-2.3.0/audiconnectpy/helpers.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.9/audiconnectpy/model.py` & `audiconnectpy-2.3.0/audiconnectpy/model.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.9/audiconnectpy/vehicle.py` & `audiconnectpy-2.3.0/audiconnectpy/vehicle.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.9/audiconnectpy.egg-info/PKG-INFO` & `audiconnectpy-2.3.0/audiconnectpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 2.2.9
+Version: 2.3.0
 Summary: Provides asynchronous authentication and access to Audi Connect
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: connect,async,audi
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `audiconnectpy-2.2.9/audiconnectpy.egg-info/SOURCES.txt` & `audiconnectpy-2.3.0/audiconnectpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.9/example.py` & `audiconnectpy-2.3.0/example.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.9/pyproject.toml` & `audiconnectpy-2.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.9/tests/conftest.py` & `audiconnectpy-2.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.9/tests/fixtures/audi0.json` & `audiconnectpy-2.3.0/tests/fixtures/audi0.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.9/tests/fixtures/audi1.json` & `audiconnectpy-2.3.0/tests/fixtures/audi1.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.9/tests/fixtures/audi2.json` & `audiconnectpy-2.3.0/tests/fixtures/audi2.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.9/tests/fixtures/info_vehicles.json` & `audiconnectpy-2.3.0/tests/fixtures/info_vehicles.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.9/tests/fixtures/location.json` & `audiconnectpy-2.3.0/tests/fixtures/location.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.9/tests/test_home.py` & `audiconnectpy-2.3.0/tests/test_home.py`

 * *Files identical despite different names*

