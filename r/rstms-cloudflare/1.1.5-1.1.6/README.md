# Comparing `tmp/rstms_cloudflare-1.1.5.tar.gz` & `tmp/rstms_cloudflare-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rstms_cloudflare-1.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "rstms_cloudflare-1.1.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `rstms_cloudflare-1.1.5.tar` & `rstms_cloudflare-1.1.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0      383 2024-05-30 20:17:39.091238 rstms_cloudflare-1.1.5/.bumpversion.cfg
--rw-r--r--   0        0        0     1344 2024-05-21 01:52:37.934629 rstms_cloudflare-1.1.5/.gitignore
--rw-r--r--   0        0        0     1071 2024-04-16 03:08:46.805802 rstms_cloudflare-1.1.5/LICENSE
--rw-r--r--   0        0        0      539 2024-04-16 03:08:46.809802 rstms_cloudflare-1.1.5/Makefile
--rw-r--r--   0        0        0      689 2024-04-16 03:08:46.817802 rstms_cloudflare-1.1.5/README.md
--rw-r--r--   0        0        0        6 2024-05-30 20:17:39.091238 rstms_cloudflare-1.1.5/VERSION
--rw-r--r--   0        0        0      617 2024-04-16 03:08:46.877802 rstms_cloudflare-1.1.5/docs/Makefile
--rw-r--r--   0        0        0       97 2024-04-16 03:08:46.889801 rstms_cloudflare-1.1.5/docs/cli.rst
--rwxr-xr-x   0        0        0     4960 2024-04-16 03:08:46.889801 rstms_cloudflare-1.1.5/docs/conf.py
--rw-r--r--   0        0        0       33 2024-04-16 03:08:46.889801 rstms_cloudflare-1.1.5/docs/contributing.rst
--rw-r--r--   0        0        0      300 2024-04-16 03:08:46.877802 rstms_cloudflare-1.1.5/docs/index.rst
--rw-r--r--   0        0        0     1174 2024-04-16 03:08:46.877802 rstms_cloudflare-1.1.5/docs/installation.rst
--rw-r--r--   0        0        0      778 2024-04-16 03:08:46.877802 rstms_cloudflare-1.1.5/docs/make.bat
--rw-r--r--   0        0        0       27 2024-04-16 03:08:46.873802 rstms_cloudflare-1.1.5/docs/readme.rst
--rw-r--r--   0        0        0      431 2024-04-16 03:08:46.833802 rstms_cloudflare-1.1.5/make/browser.mk
--rw-r--r--   0        0        0      694 2024-04-16 03:08:46.845802 rstms_cloudflare-1.1.5/make/clean.mk
--rw-r--r--   0        0        0     3808 2024-05-30 20:15:10.816745 rstms_cloudflare-1.1.5/make/common.mk
--rw-r--r--   0        0        0      477 2024-04-16 03:08:46.833802 rstms_cloudflare-1.1.5/make/depends.mk
--rw-r--r--   0        0        0      441 2024-04-16 03:08:46.829802 rstms_cloudflare-1.1.5/make/dist.mk
--rw-r--r--   0        0        0      719 2024-04-16 03:08:46.825802 rstms_cloudflare-1.1.5/make/docs.mk
--rw-r--r--   0        0        0      668 2024-05-20 19:47:31.723566 rstms_cloudflare-1.1.5/make/lint.mk
--rw-r--r--   0        0        0     1258 2024-05-30 20:16:32.983910 rstms_cloudflare-1.1.5/make/publish.mk
--rw-r--r--   0        0        0      517 2024-04-16 03:08:46.829802 rstms_cloudflare-1.1.5/make/release.mk
--rw-r--r--   0        0        0      502 2024-04-16 03:08:46.829802 rstms_cloudflare-1.1.5/make/requirements.mk
--rw-r--r--   0        0        0      947 2024-04-16 03:08:46.821802 rstms_cloudflare-1.1.5/make/test.mk
--rw-r--r--   0        0        0     1610 2024-04-16 03:08:46.833802 rstms_cloudflare-1.1.5/make/version.mk
--rw-r--r--   0        0        0     1165 2024-05-30 20:17:39.091238 rstms_cloudflare-1.1.5/pyproject.toml
--rw-r--r--   0        0        0      231 2024-04-16 03:08:46.789803 rstms_cloudflare-1.1.5/pytest.ini
--rw-r--r--   0        0        0       97 2024-05-30 20:17:38.947240 rstms_cloudflare-1.1.5/requirements-dev.txt
--rw-r--r--   0        0        0       47 2024-05-30 20:17:38.999239 rstms_cloudflare-1.1.5/requirements-docs.txt
--rw-r--r--   0        0        0       25 2024-05-30 20:17:38.891240 rstms_cloudflare-1.1.5/requirements.txt
--rw-r--r--   0        0        0      217 2024-04-16 03:18:17.194893 rstms_cloudflare-1.1.5/rstms_cloudflare/__init__.py
--rw-r--r--   0        0        0     6474 2024-05-29 03:01:48.275249 rstms_cloudflare-1.1.5/rstms_cloudflare/cli.py
--rw-r--r--   0        0        0     6182 2024-05-21 01:42:56.024690 rstms_cloudflare-1.1.5/rstms_cloudflare/cloudflare.py
--rw-r--r--   0        0        0     1065 2024-04-16 03:11:31.499807 rstms_cloudflare-1.1.5/rstms_cloudflare/exception_handler.py
--rw-r--r--   0        0        0     1092 2024-04-16 03:11:31.507807 rstms_cloudflare-1.1.5/rstms_cloudflare/shell.py
--rw-r--r--   0        0        0      127 2024-05-30 20:17:39.087238 rstms_cloudflare-1.1.5/rstms_cloudflare/version.py
--rw-r--r--   0        0        0       46 2024-04-16 03:08:46.849802 rstms_cloudflare-1.1.5/tests/__init__.py
--rw-r--r--   0        0        0     2266 2024-04-16 03:11:31.547806 rstms_cloudflare-1.1.5/tests/test_cli.py
--rw-r--r--   0        0        0      432 2024-04-16 03:08:46.789803 rstms_cloudflare-1.1.5/tox.ini
--rw-r--r--   0        0        0     1915 1970-01-01 00:00:00.000000 rstms_cloudflare-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0      383 2024-06-02 23:58:05.301806 rstms_cloudflare-1.1.6/.bumpversion.cfg
+-rw-r--r--   0        0        0     1344 2024-05-21 01:52:37.934629 rstms_cloudflare-1.1.6/.gitignore
+-rw-r--r--   0        0        0     1071 2024-04-16 03:08:46.805802 rstms_cloudflare-1.1.6/LICENSE
+-rw-r--r--   0        0        0      539 2024-04-16 03:08:46.809802 rstms_cloudflare-1.1.6/Makefile
+-rw-r--r--   0        0        0      689 2024-04-16 03:08:46.817802 rstms_cloudflare-1.1.6/README.md
+-rw-r--r--   0        0        0        6 2024-06-02 23:58:05.301806 rstms_cloudflare-1.1.6/VERSION
+-rw-r--r--   0        0        0      617 2024-04-16 03:08:46.877802 rstms_cloudflare-1.1.6/docs/Makefile
+-rw-r--r--   0        0        0       97 2024-04-16 03:08:46.889801 rstms_cloudflare-1.1.6/docs/cli.rst
+-rwxr-xr-x   0        0        0     4960 2024-04-16 03:08:46.889801 rstms_cloudflare-1.1.6/docs/conf.py
+-rw-r--r--   0        0        0       33 2024-04-16 03:08:46.889801 rstms_cloudflare-1.1.6/docs/contributing.rst
+-rw-r--r--   0        0        0      300 2024-04-16 03:08:46.877802 rstms_cloudflare-1.1.6/docs/index.rst
+-rw-r--r--   0        0        0     1174 2024-04-16 03:08:46.877802 rstms_cloudflare-1.1.6/docs/installation.rst
+-rw-r--r--   0        0        0      778 2024-04-16 03:08:46.877802 rstms_cloudflare-1.1.6/docs/make.bat
+-rw-r--r--   0        0        0       27 2024-04-16 03:08:46.873802 rstms_cloudflare-1.1.6/docs/readme.rst
+-rw-r--r--   0        0        0      431 2024-04-16 03:08:46.833802 rstms_cloudflare-1.1.6/make/browser.mk
+-rw-r--r--   0        0        0      694 2024-04-16 03:08:46.845802 rstms_cloudflare-1.1.6/make/clean.mk
+-rw-r--r--   0        0        0     3808 2024-05-30 20:15:10.816745 rstms_cloudflare-1.1.6/make/common.mk
+-rw-r--r--   0        0        0      477 2024-04-16 03:08:46.833802 rstms_cloudflare-1.1.6/make/depends.mk
+-rw-r--r--   0        0        0      441 2024-04-16 03:08:46.829802 rstms_cloudflare-1.1.6/make/dist.mk
+-rw-r--r--   0        0        0      719 2024-04-16 03:08:46.825802 rstms_cloudflare-1.1.6/make/docs.mk
+-rw-r--r--   0        0        0      668 2024-05-30 20:38:28.110546 rstms_cloudflare-1.1.6/make/lint.mk
+-rw-r--r--   0        0        0     1258 2024-05-30 20:16:32.983910 rstms_cloudflare-1.1.6/make/publish.mk
+-rw-r--r--   0        0        0      517 2024-04-16 03:08:46.829802 rstms_cloudflare-1.1.6/make/release.mk
+-rw-r--r--   0        0        0      502 2024-04-16 03:08:46.829802 rstms_cloudflare-1.1.6/make/requirements.mk
+-rw-r--r--   0        0        0      947 2024-04-16 03:08:46.821802 rstms_cloudflare-1.1.6/make/test.mk
+-rw-r--r--   0        0        0     1610 2024-04-16 03:08:46.833802 rstms_cloudflare-1.1.6/make/version.mk
+-rw-r--r--   0        0        0     1165 2024-06-02 23:58:05.301806 rstms_cloudflare-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0      231 2024-04-16 03:08:46.789803 rstms_cloudflare-1.1.6/pytest.ini
+-rw-r--r--   0        0        0       97 2024-06-02 23:58:05.153807 rstms_cloudflare-1.1.6/requirements-dev.txt
+-rw-r--r--   0        0        0       47 2024-06-02 23:58:05.209807 rstms_cloudflare-1.1.6/requirements-docs.txt
+-rw-r--r--   0        0        0       25 2024-06-02 23:58:05.097808 rstms_cloudflare-1.1.6/requirements.txt
+-rw-r--r--   0        0        0      217 2024-04-16 03:18:17.194893 rstms_cloudflare-1.1.6/rstms_cloudflare/__init__.py
+-rw-r--r--   0        0        0     6474 2024-05-30 22:15:44.026028 rstms_cloudflare-1.1.6/rstms_cloudflare/cli.py
+-rw-r--r--   0        0        0     6206 2024-06-02 06:06:02.144209 rstms_cloudflare-1.1.6/rstms_cloudflare/cloudflare.py
+-rw-r--r--   0        0        0     1065 2024-04-16 03:11:31.499807 rstms_cloudflare-1.1.6/rstms_cloudflare/exception_handler.py
+-rw-r--r--   0        0        0     1092 2024-04-16 03:11:31.507807 rstms_cloudflare-1.1.6/rstms_cloudflare/shell.py
+-rw-r--r--   0        0        0      127 2024-06-02 23:58:05.301806 rstms_cloudflare-1.1.6/rstms_cloudflare/version.py
+-rw-r--r--   0        0        0       46 2024-04-16 03:08:46.849802 rstms_cloudflare-1.1.6/tests/__init__.py
+-rw-r--r--   0        0        0     2266 2024-04-16 03:11:31.547806 rstms_cloudflare-1.1.6/tests/test_cli.py
+-rw-r--r--   0        0        0      432 2024-04-16 03:08:46.789803 rstms_cloudflare-1.1.6/tox.ini
+-rw-r--r--   0        0        0     1915 1970-01-01 00:00:00.000000 rstms_cloudflare-1.1.6/PKG-INFO
```

### Comparing `rstms_cloudflare-1.1.5/.gitignore` & `rstms_cloudflare-1.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.5/LICENSE` & `rstms_cloudflare-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.5/Makefile` & `rstms_cloudflare-1.1.6/Makefile`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.5/README.md` & `rstms_cloudflare-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.5/docs/Makefile` & `rstms_cloudflare-1.1.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.5/docs/conf.py` & `rstms_cloudflare-1.1.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.5/docs/installation.rst` & `rstms_cloudflare-1.1.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.5/docs/make.bat` & `rstms_cloudflare-1.1.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.5/make/clean.mk` & `rstms_cloudflare-1.1.6/make/clean.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.5/make/common.mk` & `rstms_cloudflare-1.1.6/make/common.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.5/make/docs.mk` & `rstms_cloudflare-1.1.6/make/docs.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.5/make/lint.mk` & `rstms_cloudflare-1.1.6/make/lint.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.5/make/publish.mk` & `rstms_cloudflare-1.1.6/make/publish.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.5/make/release.mk` & `rstms_cloudflare-1.1.6/make/release.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.5/make/test.mk` & `rstms_cloudflare-1.1.6/make/test.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.5/make/version.mk` & `rstms_cloudflare-1.1.6/make/version.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.5/pyproject.toml` & `rstms_cloudflare-1.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 requires_python = ">=3.10"
 
 
 
 [project]
 name = "rstms-cloudflare"
-version = "1.1.5"
+version = "1.1.6"
 authors = [{name = "Matt Krueger", email = "mkrueger@rstms.net"}]
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
 keywords = ["rstms_cloudflare"]
 classifiers = [
   "Intended Audience :: Developers",
```

### Comparing `rstms_cloudflare-1.1.5/rstms_cloudflare/cli.py` & `rstms_cloudflare-1.1.6/rstms_cloudflare/cli.py`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.5/rstms_cloudflare/cloudflare.py` & `rstms_cloudflare-1.1.6/rstms_cloudflare/cloudflare.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import re
 
 import CloudFlare
 
 
 class API:
 
-    RECORD_TYPES = ["A", "AAAA", "CNAME", "MX", "NS", "SOA", "TXT", "SRV", "LOC"]
+    RECORD_TYPES = ["A", "AAAA", "CNAME", "MX", "NS", "SOA", "TXT", "SRV", "LOC", "SSHFP", "CAA", "TLSA"]
     MAX_ZONES = 128
 
     def __init__(self, token=None, json=False, quiet=False, raw=False, include_id=False, output_function=None):
         token = token or os.environ["CLOUDFLARE_AUTH_TOKEN"]
         self.client = CloudFlare.CloudFlare(token=token)
         self.json = json
         self.raw = raw
```

### Comparing `rstms_cloudflare-1.1.5/rstms_cloudflare/exception_handler.py` & `rstms_cloudflare-1.1.6/rstms_cloudflare/exception_handler.py`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.5/rstms_cloudflare/shell.py` & `rstms_cloudflare-1.1.6/rstms_cloudflare/shell.py`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.5/tests/test_cli.py` & `rstms_cloudflare-1.1.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.5/PKG-INFO` & `rstms_cloudflare-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rstms-cloudflare
-Version: 1.1.5
+Version: 1.1.6
 Summary: Top-level package for rstms-cloudflare.
 Keywords: rstms_cloudflare
 Author-email: Matt Krueger <mkrueger@rstms.net>
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

