# Comparing `tmp/myelectricaldatapy-2.2.2.tar.gz` & `tmp/myelectricaldatapy-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myelectricaldatapy-2.2.2.tar", last modified: Tue May 28 07:13:55 2024, max compression
+gzip compressed data, was "myelectricaldatapy-2.2.3.tar", last modified: Mon Jun  3 06:39:48 2024, max compression
```

## Comparing `myelectricaldatapy-2.2.2.tar` & `myelectricaldatapy-2.2.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:13:55.397485 myelectricaldatapy-2.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-28 07:13:43.000000 myelectricaldatapy-2.2.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:13:55.389485 myelectricaldatapy-2.2.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-28 07:13:43.000000 myelectricaldatapy-2.2.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:13:55.389485 myelectricaldatapy-2.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-28 07:13:43.000000 myelectricaldatapy-2.2.2/.github/workflows/auto-approve.yml
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-28 07:13:43.000000 myelectricaldatapy-2.2.2/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-28 07:13:43.000000 myelectricaldatapy-2.2.2/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-28 07:13:43.000000 myelectricaldatapy-2.2.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-28 07:13:43.000000 myelectricaldatapy-2.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-28 07:13:43.000000 myelectricaldatapy-2.2.2/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:13:55.389485 myelectricaldatapy-2.2.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-28 07:13:43.000000 myelectricaldatapy-2.2.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-28 07:13:43.000000 myelectricaldatapy-2.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-28 07:13:43.000000 myelectricaldatapy-2.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-05-28 07:13:55.393485 myelectricaldatapy-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-28 07:13:43.000000 myelectricaldatapy-2.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-28 07:13:43.000000 myelectricaldatapy-2.2.2/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:13:55.393485 myelectricaldatapy-2.2.2/myelectricaldatapy/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-28 07:13:43.000000 myelectricaldatapy-2.2.2/myelectricaldatapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-05-28 07:13:43.000000 myelectricaldatapy-2.2.2/myelectricaldatapy/analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-28 07:13:43.000000 myelectricaldatapy-2.2.2/myelectricaldatapy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-28 07:13:43.000000 myelectricaldatapy-2.2.2/myelectricaldatapy/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-28 07:13:43.000000 myelectricaldatapy-2.2.2/myelectricaldatapy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8468 2024-05-28 07:13:43.000000 myelectricaldatapy-2.2.2/myelectricaldatapy/myelectricaldata.py
--rw-r--r--   0 runner    (1001) docker     (127)    11515 2024-05-28 07:13:43.000000 myelectricaldatapy-2.2.2/myelectricaldatapy/mypdl.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 07:13:43.000000 myelectricaldatapy-2.2.2/myelectricaldatapy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:13:55.393485 myelectricaldatapy-2.2.2/myelectricaldatapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-05-28 07:13:55.000000 myelectricaldatapy-2.2.2/myelectricaldatapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-28 07:13:55.000000 myelectricaldatapy-2.2.2/myelectricaldatapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 07:13:55.000000 myelectricaldatapy-2.2.2/myelectricaldatapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-28 07:13:55.000000 myelectricaldatapy-2.2.2/myelectricaldatapy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-28 07:13:55.000000 myelectricaldatapy-2.2.2/myelectricaldatapy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-28 07:13:43.000000 myelectricaldatapy-2.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-28 07:13:43.000000 myelectricaldatapy-2.2.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-28 07:13:43.000000 myelectricaldatapy-2.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 07:13:55.397485 myelectricaldatapy-2.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:13:55.393485 myelectricaldatapy-2.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-28 07:13:43.000000 myelectricaldatapy-2.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-28 07:13:43.000000 myelectricaldatapy-2.2.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-28 07:13:43.000000 myelectricaldatapy-2.2.2/tests/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:13:55.393485 myelectricaldatapy-2.2.2/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-28 07:13:43.000000 myelectricaldatapy-2.2.2/tests/fixtures/access.json
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-28 07:13:43.000000 myelectricaldatapy-2.2.2/tests/fixtures/address.json
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-28 07:13:43.000000 myelectricaldatapy-2.2.2/tests/fixtures/contract.json
--rw-r--r--   0 runner    (1001) docker     (127)    18546 2024-05-28 07:13:43.000000 myelectricaldatapy-2.2.2/tests/fixtures/daily.json
--rw-r--r--   0 runner    (1001) docker     (127)    21145 2024-05-28 07:13:43.000000 myelectricaldatapy-2.2.2/tests/fixtures/detail.json
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-28 07:13:43.000000 myelectricaldatapy-2.2.2/tests/fixtures/ecowatt.json
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-28 07:13:43.000000 myelectricaldatapy-2.2.2/tests/fixtures/invalid_access.json
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-28 07:13:43.000000 myelectricaldatapy-2.2.2/tests/fixtures/tempo.json
--rw-r--r--   0 runner    (1001) docker     (127)    12707 2024-05-28 07:13:43.000000 myelectricaldatapy-2.2.2/tests/test_analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5557 2024-05-28 07:13:43.000000 myelectricaldatapy-2.2.2/tests/test_load_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:39:48.164916 myelectricaldatapy-2.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-06-03 06:39:38.000000 myelectricaldatapy-2.2.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:39:48.160916 myelectricaldatapy-2.2.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-06-03 06:39:38.000000 myelectricaldatapy-2.2.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:39:48.160916 myelectricaldatapy-2.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-06-03 06:39:38.000000 myelectricaldatapy-2.2.3/.github/workflows/auto-approve.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-06-03 06:39:38.000000 myelectricaldatapy-2.2.3/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-06-03 06:39:38.000000 myelectricaldatapy-2.2.3/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-06-03 06:39:38.000000 myelectricaldatapy-2.2.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-06-03 06:39:38.000000 myelectricaldatapy-2.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-06-03 06:39:38.000000 myelectricaldatapy-2.2.3/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:39:48.160916 myelectricaldatapy-2.2.3/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-06-03 06:39:38.000000 myelectricaldatapy-2.2.3/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-03 06:39:38.000000 myelectricaldatapy-2.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-06-03 06:39:38.000000 myelectricaldatapy-2.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-06-03 06:39:48.164916 myelectricaldatapy-2.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-06-03 06:39:38.000000 myelectricaldatapy-2.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-06-03 06:39:38.000000 myelectricaldatapy-2.2.3/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:39:48.160916 myelectricaldatapy-2.2.3/myelectricaldatapy/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-06-03 06:39:38.000000 myelectricaldatapy-2.2.3/myelectricaldatapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-06-03 06:39:38.000000 myelectricaldatapy-2.2.3/myelectricaldatapy/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-06-03 06:39:38.000000 myelectricaldatapy-2.2.3/myelectricaldatapy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-06-03 06:39:38.000000 myelectricaldatapy-2.2.3/myelectricaldatapy/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-06-03 06:39:38.000000 myelectricaldatapy-2.2.3/myelectricaldatapy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8468 2024-06-03 06:39:38.000000 myelectricaldatapy-2.2.3/myelectricaldatapy/myelectricaldata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11621 2024-06-03 06:39:38.000000 myelectricaldatapy-2.2.3/myelectricaldatapy/mypdl.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 06:39:38.000000 myelectricaldatapy-2.2.3/myelectricaldatapy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:39:48.164916 myelectricaldatapy-2.2.3/myelectricaldatapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-06-03 06:39:48.000000 myelectricaldatapy-2.2.3/myelectricaldatapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-06-03 06:39:48.000000 myelectricaldatapy-2.2.3/myelectricaldatapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 06:39:48.000000 myelectricaldatapy-2.2.3/myelectricaldatapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-06-03 06:39:48.000000 myelectricaldatapy-2.2.3/myelectricaldatapy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-06-03 06:39:48.000000 myelectricaldatapy-2.2.3/myelectricaldatapy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-06-03 06:39:38.000000 myelectricaldatapy-2.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-06-03 06:39:38.000000 myelectricaldatapy-2.2.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-06-03 06:39:38.000000 myelectricaldatapy-2.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 06:39:48.164916 myelectricaldatapy-2.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:39:48.164916 myelectricaldatapy-2.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-06-03 06:39:38.000000 myelectricaldatapy-2.2.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-06-03 06:39:38.000000 myelectricaldatapy-2.2.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-06-03 06:39:38.000000 myelectricaldatapy-2.2.3/tests/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:39:48.164916 myelectricaldatapy-2.2.3/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-06-03 06:39:38.000000 myelectricaldatapy-2.2.3/tests/fixtures/access.json
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-06-03 06:39:38.000000 myelectricaldatapy-2.2.3/tests/fixtures/address.json
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-06-03 06:39:38.000000 myelectricaldatapy-2.2.3/tests/fixtures/contract.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18546 2024-06-03 06:39:38.000000 myelectricaldatapy-2.2.3/tests/fixtures/daily.json
+-rw-r--r--   0 runner    (1001) docker     (127)    21145 2024-06-03 06:39:38.000000 myelectricaldatapy-2.2.3/tests/fixtures/detail.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-06-03 06:39:38.000000 myelectricaldatapy-2.2.3/tests/fixtures/ecowatt.json
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-06-03 06:39:38.000000 myelectricaldatapy-2.2.3/tests/fixtures/invalid_access.json
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-03 06:39:38.000000 myelectricaldatapy-2.2.3/tests/fixtures/tempo.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12707 2024-06-03 06:39:38.000000 myelectricaldatapy-2.2.3/tests/test_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5557 2024-06-03 06:39:38.000000 myelectricaldatapy-2.2.3/tests/test_load_data.py
```

### Comparing `myelectricaldatapy-2.2.2/.github/dependabot.yml` & `myelectricaldatapy-2.2.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.2.2/.github/workflows/auto-approve.yml` & `myelectricaldatapy-2.2.3/.github/workflows/auto-approve.yml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.2.2/.github/workflows/lint.yml` & `myelectricaldatapy-2.2.3/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.2.2/.github/workflows/pythonpublish.yml` & `myelectricaldatapy-2.2.3/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.2.2/.github/workflows/release.yml` & `myelectricaldatapy-2.2.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.2.2/.gitignore` & `myelectricaldatapy-2.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.2.2/.pre-commit-config.yaml` & `myelectricaldatapy-2.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.2.2/LICENSE` & `myelectricaldatapy-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.2.2/PKG-INFO` & `myelectricaldatapy-2.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myelectricaldatapy
-Version: 2.2.2
+Version: 2.2.3
 Summary: Fetch Linky data from myelectricaldata.fr
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: enedis,linky,async,myelectricaldata
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `myelectricaldatapy-2.2.2/README.md` & `myelectricaldatapy-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.2.2/example.py` & `myelectricaldatapy-2.2.3/example.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.2.2/myelectricaldatapy/analytics.py` & `myelectricaldatapy-2.2.3/myelectricaldatapy/analytics.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.2.2/myelectricaldatapy/auth.py` & `myelectricaldatapy-2.2.3/myelectricaldatapy/auth.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,17 +48,18 @@
         except (asyncio.CancelledError, asyncio.TimeoutError) as error:
             raise TimeoutExceededError(
                 "Timeout occurred while connecting to MyElectricalData."
             ) from error
         except ClientResponseError:
             message = contents.decode("utf8")
             if "application/json" in response.headers.get("Content-Type", ""):
+                msg = json.loads(message)
                 if response.status == 409:
-                    raise LimitReached(json.loads(message))
-                raise EnedisException(json.loads(message))
+                    raise LimitReached(msg.get("detail", msg))
+                raise EnedisException(msg.get("detail", msg))
             raise EnedisException({"message": message})
         except (ClientError, socket.gaierror) as error:
             raise HttpRequestError(
                 "Error occurred while communicating with MyElectricalData."
             ) from error
 
         return (
```

### Comparing `myelectricaldatapy-2.2.2/myelectricaldatapy/const.py` & `myelectricaldatapy-2.2.3/myelectricaldatapy/const.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.2.2/myelectricaldatapy/myelectricaldata.py` & `myelectricaldatapy-2.2.3/myelectricaldatapy/myelectricaldata.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.2.2/myelectricaldatapy/mypdl.py` & `myelectricaldatapy-2.2.3/myelectricaldatapy/mypdl.py`

 * *Files 1% similar despite different names*

```diff
@@ -324,14 +324,16 @@
             fn = attr[ATTR_FN]
             try:
                 dataset = await fn(self.pdl, start, end)
             except EnedisException as error:
                 checked = False
                 _LOGGER.error(error)
             else:
+                if dataset is None:
+                    raise EnedisException("Data collection is empty")
                 data = dataset.get("meter_reading", {}).get("interval_reading", [])
                 if len(data) == 0:
                     raise EnedisException("Data collection is empty")
                 checked = checked and len(data) > 0
                 self._params[mode].update({"data": data})
 
             if mode == CONSUMPTION and self._tempo_subs:
```

### Comparing `myelectricaldatapy-2.2.2/myelectricaldatapy.egg-info/PKG-INFO` & `myelectricaldatapy-2.2.3/myelectricaldatapy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myelectricaldatapy
-Version: 2.2.2
+Version: 2.2.3
 Summary: Fetch Linky data from myelectricaldata.fr
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: enedis,linky,async,myelectricaldata
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `myelectricaldatapy-2.2.2/myelectricaldatapy.egg-info/SOURCES.txt` & `myelectricaldatapy-2.2.3/myelectricaldatapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.2.2/pyproject.toml` & `myelectricaldatapy-2.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.2.2/tests/conftest.py` & `myelectricaldatapy-2.2.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.2.2/tests/fixtures/address.json` & `myelectricaldatapy-2.2.3/tests/fixtures/address.json`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.2.2/tests/fixtures/contract.json` & `myelectricaldatapy-2.2.3/tests/fixtures/contract.json`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.2.2/tests/fixtures/daily.json` & `myelectricaldatapy-2.2.3/tests/fixtures/daily.json`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.2.2/tests/fixtures/detail.json` & `myelectricaldatapy-2.2.3/tests/fixtures/detail.json`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.2.2/tests/fixtures/ecowatt.json` & `myelectricaldatapy-2.2.3/tests/fixtures/ecowatt.json`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.2.2/tests/test_analytics.py` & `myelectricaldatapy-2.2.3/tests/test_analytics.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.2.2/tests/test_load_data.py` & `myelectricaldatapy-2.2.3/tests/test_load_data.py`

 * *Files identical despite different names*

