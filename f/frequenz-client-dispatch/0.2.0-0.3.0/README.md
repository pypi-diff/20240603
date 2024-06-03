# Comparing `tmp/frequenz-client-dispatch-0.2.0.tar.gz` & `tmp/frequenz-client-dispatch-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frequenz-client-dispatch-0.2.0.tar", last modified: Wed Apr 24 13:01:53 2024, max compression
+gzip compressed data, was "frequenz-client-dispatch-0.3.0.tar", last modified: Mon Jun  3 12:53:51 2024, max compression
```

## Comparing `frequenz-client-dispatch-0.2.0.tar` & `frequenz-client-dispatch-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:53.958815 frequenz-client-dispatch-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-24 13:01:42.000000 frequenz-client-dispatch-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-24 13:01:42.000000 frequenz-client-dispatch-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-24 13:01:53.958815 frequenz-client-dispatch-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-24 13:01:42.000000 frequenz-client-dispatch-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-24 13:01:42.000000 frequenz-client-dispatch-0.2.0/RELEASE_NOTES.md
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-04-24 13:01:42.000000 frequenz-client-dispatch-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 13:01:53.958815 frequenz-client-dispatch-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:53.954815 frequenz-client-dispatch-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:53.954815 frequenz-client-dispatch-0.2.0/src/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:53.954815 frequenz-client-dispatch-0.2.0/src/frequenz/client/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-24 13:01:42.000000 frequenz-client-dispatch-0.2.0/src/frequenz/client/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:53.954815 frequenz-client-dispatch-0.2.0/src/frequenz/client/dispatch/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-24 13:01:42.000000 frequenz-client-dispatch-0.2.0/src/frequenz/client/dispatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-04-24 13:01:42.000000 frequenz-client-dispatch-0.2.0/src/frequenz/client/dispatch/_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-24 13:01:42.000000 frequenz-client-dispatch-0.2.0/src/frequenz/client/dispatch/_internal_types.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:42.000000 frequenz-client-dispatch-0.2.0/src/frequenz/client/dispatch/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:53.958815 frequenz-client-dispatch-0.2.0/src/frequenz/client/dispatch/test/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-24 13:01:42.000000 frequenz-client-dispatch-0.2.0/src/frequenz/client/dispatch/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-04-24 13:01:42.000000 frequenz-client-dispatch-0.2.0/src/frequenz/client/dispatch/test/_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-24 13:01:42.000000 frequenz-client-dispatch-0.2.0/src/frequenz/client/dispatch/test/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-04-24 13:01:42.000000 frequenz-client-dispatch-0.2.0/src/frequenz/client/dispatch/test/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-04-24 13:01:42.000000 frequenz-client-dispatch-0.2.0/src/frequenz/client/dispatch/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:53.958815 frequenz-client-dispatch-0.2.0/src/frequenz_client_dispatch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-24 13:01:53.000000 frequenz-client-dispatch-0.2.0/src/frequenz_client_dispatch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-24 13:01:53.000000 frequenz-client-dispatch-0.2.0/src/frequenz_client_dispatch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:01:53.000000 frequenz-client-dispatch-0.2.0/src/frequenz_client_dispatch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-24 13:01:53.000000 frequenz-client-dispatch-0.2.0/src/frequenz_client_dispatch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 13:01:53.000000 frequenz-client-dispatch-0.2.0/src/frequenz_client_dispatch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:53:51.753385 frequenz-client-dispatch-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-06-03 12:53:34.000000 frequenz-client-dispatch-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-06-03 12:53:34.000000 frequenz-client-dispatch-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-06-03 12:53:51.753385 frequenz-client-dispatch-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-06-03 12:53:34.000000 frequenz-client-dispatch-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-06-03 12:53:34.000000 frequenz-client-dispatch-0.3.0/RELEASE_NOTES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-06-03 12:53:34.000000 frequenz-client-dispatch-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 12:53:51.753385 frequenz-client-dispatch-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:53:51.749385 frequenz-client-dispatch-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:53:51.749385 frequenz-client-dispatch-0.3.0/src/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:53:51.753385 frequenz-client-dispatch-0.3.0/src/frequenz/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-06-03 12:53:34.000000 frequenz-client-dispatch-0.3.0/src/frequenz/client/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:53:51.753385 frequenz-client-dispatch-0.3.0/src/frequenz/client/dispatch/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-06-03 12:53:34.000000 frequenz-client-dispatch-0.3.0/src/frequenz/client/dispatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12771 2024-06-03 12:53:34.000000 frequenz-client-dispatch-0.3.0/src/frequenz/client/dispatch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6283 2024-06-03 12:53:34.000000 frequenz-client-dispatch-0.3.0/src/frequenz/client/dispatch/_cli_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10447 2024-06-03 12:53:34.000000 frequenz-client-dispatch-0.3.0/src/frequenz/client/dispatch/_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-06-03 12:53:34.000000 frequenz-client-dispatch-0.3.0/src/frequenz/client/dispatch/_internal_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:53:34.000000 frequenz-client-dispatch-0.3.0/src/frequenz/client/dispatch/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:53:51.753385 frequenz-client-dispatch-0.3.0/src/frequenz/client/dispatch/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-06-03 12:53:34.000000 frequenz-client-dispatch-0.3.0/src/frequenz/client/dispatch/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-06-03 12:53:34.000000 frequenz-client-dispatch-0.3.0/src/frequenz/client/dispatch/test/_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-06-03 12:53:34.000000 frequenz-client-dispatch-0.3.0/src/frequenz/client/dispatch/test/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-06-03 12:53:34.000000 frequenz-client-dispatch-0.3.0/src/frequenz/client/dispatch/test/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-06-03 12:53:34.000000 frequenz-client-dispatch-0.3.0/src/frequenz/client/dispatch/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:53:51.753385 frequenz-client-dispatch-0.3.0/src/frequenz_client_dispatch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-06-03 12:53:51.000000 frequenz-client-dispatch-0.3.0/src/frequenz_client_dispatch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-06-03 12:53:51.000000 frequenz-client-dispatch-0.3.0/src/frequenz_client_dispatch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 12:53:51.000000 frequenz-client-dispatch-0.3.0/src/frequenz_client_dispatch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-06-03 12:53:51.000000 frequenz-client-dispatch-0.3.0/src/frequenz_client_dispatch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-06-03 12:53:51.000000 frequenz-client-dispatch-0.3.0/src/frequenz_client_dispatch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-03 12:53:51.000000 frequenz-client-dispatch-0.3.0/src/frequenz_client_dispatch.egg-info/top_level.txt
```

### Comparing `frequenz-client-dispatch-0.2.0/LICENSE` & `frequenz-client-dispatch-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frequenz-client-dispatch-0.2.0/PKG-INFO` & `frequenz-client-dispatch-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-client-dispatch
-Version: 0.2.0
+Version: 0.3.0
 Summary: Dispatch API client for Python
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Documentation, https://frequenz-floss.github.io/frequenz-client-dispatch-python/
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-client-dispatch-python/releases
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-client-dispatch-python/issues
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-client-dispatch-python
@@ -15,14 +15,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
 Requires-Python: <4,>=3.11
 Description-Content-Type: text/markdown
+Provides-Extra: cli
 Provides-Extra: dev-flake8
 Provides-Extra: dev-formatting
 Provides-Extra: dev-mkdocs
 Provides-Extra: dev-mypy
 Provides-Extra: dev-noxfile
 Provides-Extra: dev-pylint
 Provides-Extra: dev-pytest
```

### Comparing `frequenz-client-dispatch-0.2.0/README.md` & `frequenz-client-dispatch-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `frequenz-client-dispatch-0.2.0/pyproject.toml` & `frequenz-client-dispatch-0.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # License: MIT
 # Copyright © 2024 Frequenz Energy-as-a-Service GmbH
 
 [build-system]
 requires = [
   "setuptools == 68.1.0",
   "setuptools_scm[toml] == 7.1.0",
-  "frequenz-repo-config[lib] == 0.9.1",
+  "frequenz-repo-config[lib] == 0.9.2",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "frequenz-client-dispatch"
 description = "Dispatch API client for Python"
 readme = "README.md"
@@ -34,67 +34,72 @@
   "Topic :: Software Development :: Libraries",
   "Typing :: Typed",
 ]
 requires-python = ">= 3.11, < 4"
 dependencies = [
   "typing-extensions >= 4.6.1, < 5",
   "frequenz-api-dispatch >= 0.13.0, < 0.14",
-  "frequenz-client-base >= 0.2.1, < 0.4.0",
-  "frequenz-client-common >= 0.1.0, < 0.2.0",
+  "frequenz-client-base >= 0.2.1, < 0.5.0",
+  "frequenz-client-common >= 0.1.0, < 0.3.0",
   "grpcio >= 1.54.2, < 2",
 ]
 dynamic = ["version"]
 
+[project.scripts]
+dispatch-cli = "frequenz.client.dispatch.__main__:main"
+
 [[project.authors]]
 name = "Frequenz Energy-as-a-Service GmbH"
 email = "floss@frequenz.com"
 
 [project.optional-dependencies]
+cli = ["asyncclick == 8.1.7.2", "prompt-toolkit == 3.0.45", "parsedatetime==2.6", "tzlocal==5.2"]
+
 dev-flake8 = [
   "flake8 == 7.0.0",
   "flake8-docstrings == 1.7.0",
   "flake8-pyproject == 1.2.3",  # For reading the flake8 config from pyproject.toml
   "pydoclint == 0.4.1",
   "pydocstyle == 6.3.0",
 ]
-dev-formatting = ["black == 24.3.0", "isort == 5.13.2"]
+dev-formatting = ["black == 24.4.2", "isort == 5.13.2"]
 dev-mkdocs = [
-  "black == 24.3.0",
+  "black == 24.4.2",
   "Markdown==3.6",
-  "mike == 2.0.0",
+  "mike == 2.1.1",
   "mkdocs-gen-files == 0.5.0",
   "mkdocs-literate-nav == 0.6.1",
   "mkdocs-macros-plugin == 1.0.5",
-  "mkdocs-material == 9.5.17",
-  "mkdocstrings[python] == 0.24.1",
-  "frequenz-repo-config[lib] == 0.9.1",
+  "mkdocs-material == 9.5.25",
+  "mkdocstrings[python] == 0.25.1",
+  "frequenz-repo-config[lib] == 0.9.2",
 ]
 dev-mypy = [
-  "mypy == 1.9.0",
+  "mypy == 1.10.0",
   "types-Markdown == 3.6.0.20240316",
   # For checking the noxfile, docs/ script, and tests
-  "frequenz-client-dispatch[dev-mkdocs,dev-noxfile,dev-pytest]",
+  "frequenz-client-dispatch[cli,dev-mkdocs,dev-noxfile,dev-pytest]",
   "grpc-stubs == 1.53.0.5",
   "types-protobuf == 5.26.0.20240422",
 ]
-dev-noxfile = ["nox == 2024.3.2", "frequenz-repo-config[lib] == 0.9.1"]
+dev-noxfile = ["nox == 2024.4.15", "frequenz-repo-config[lib] == 0.9.2"]
 dev-pylint = [
-  "pylint == 3.1.0",
+  "pylint == 3.2.2",
   # For checking the noxfile, docs/ script, and tests
-  "frequenz-client-dispatch[dev-mkdocs,dev-noxfile,dev-pytest]",
+  "frequenz-client-dispatch[cli,dev-mkdocs,dev-noxfile,dev-pytest]",
   "frequenz-api-dispatch >= 0.13.0, < 0.14",
 ]
 dev-pytest = [
-  "pytest == 8.1.1",
-  "frequenz-repo-config[extra-lint-examples] == 0.9.1",
+  "pytest == 8.2.1",
+  "frequenz-repo-config[extra-lint-examples] == 0.9.2",
   "pytest-mock == 3.14.0",
-  "pytest-asyncio == 0.23.6",
+  "pytest-asyncio == 0.23.7",
   "async-solipsism == 0.6",
-  "hypothesis == 6.100.0",
-  "sybil == 6.0.3",
+  "hypothesis == 6.103.0",
+  "frequenz-client-dispatch[cli]",
 ]
 dev = [
   "frequenz-client-dispatch[dev-mkdocs,dev-flake8,dev-formatting,dev-mkdocs,dev-mypy,dev-noxfile,dev-pylint,dev-pytest]",
 ]
 
 [project.urls]
 Documentation = "https://frequenz-floss.github.io/frequenz-client-dispatch-python/"
```

### Comparing `frequenz-client-dispatch-0.2.0/src/frequenz/client/dispatch/_client.py` & `frequenz-client-dispatch-0.3.0/src/frequenz/client/dispatch/_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,14 +207,16 @@
                     msg.update.start_time.CopyFrom(to_timestamp(val))
                 case "duration":
                     msg.update.duration = int(val.total_seconds())
                 case "selector":
                     msg.update.selector.CopyFrom(component_selector_to_protobuf(val))
                 case "is_active":
                     msg.update.is_active = val
+                case "payload":
+                    msg.update.payload.update(val)
                 case "active":
                     msg.update.is_active = val
                     key = "is_active"
                 case "is_dry_run" | "dry_run":
                     raise ValueError("Updating dry_run is not supported")
                 case "recurrence":
                     match path[1]:
```

### Comparing `frequenz-client-dispatch-0.2.0/src/frequenz/client/dispatch/_internal_types.py` & `frequenz-client-dispatch-0.3.0/src/frequenz/client/dispatch/_internal_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
             The converted protobuf dispatch create request.
         """
         pb_request = PBDispatchCreateRequest()
 
         pb_request.microgrid_id = self.microgrid_id
         pb_request.type = self.type
         pb_request.start_time.CopyFrom(to_timestamp(self.start_time))
-        pb_request.duration = int(self.duration.total_seconds())
+        pb_request.duration = round(self.duration.total_seconds())
         pb_request.selector.CopyFrom(component_selector_to_protobuf(self.selector))
         pb_request.is_active = self.active
         pb_request.is_dry_run = self.dry_run
         pb_request.payload.update(self.payload)
         pb_request.recurrence.CopyFrom(self.recurrence.to_protobuf())
 
         return pb_request
```

### Comparing `frequenz-client-dispatch-0.2.0/src/frequenz/client/dispatch/test/_service.py` & `frequenz-client-dispatch-0.3.0/src/frequenz/client/dispatch/test/_service.py`

 * *Files identical despite different names*

### Comparing `frequenz-client-dispatch-0.2.0/src/frequenz/client/dispatch/test/client.py` & `frequenz-client-dispatch-0.3.0/src/frequenz/client/dispatch/test/client.py`

 * *Files identical despite different names*

### Comparing `frequenz-client-dispatch-0.2.0/src/frequenz/client/dispatch/test/generator.py` & `frequenz-client-dispatch-0.3.0/src/frequenz/client/dispatch/test/generator.py`

 * *Files identical despite different names*

### Comparing `frequenz-client-dispatch-0.2.0/src/frequenz/client/dispatch/types.py` & `frequenz-client-dispatch-0.3.0/src/frequenz/client/dispatch/types.py`

 * *Files identical despite different names*

### Comparing `frequenz-client-dispatch-0.2.0/src/frequenz_client_dispatch.egg-info/PKG-INFO` & `frequenz-client-dispatch-0.3.0/src/frequenz_client_dispatch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-client-dispatch
-Version: 0.2.0
+Version: 0.3.0
 Summary: Dispatch API client for Python
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Documentation, https://frequenz-floss.github.io/frequenz-client-dispatch-python/
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-client-dispatch-python/releases
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-client-dispatch-python/issues
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-client-dispatch-python
@@ -15,14 +15,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
 Requires-Python: <4,>=3.11
 Description-Content-Type: text/markdown
+Provides-Extra: cli
 Provides-Extra: dev-flake8
 Provides-Extra: dev-formatting
 Provides-Extra: dev-mkdocs
 Provides-Extra: dev-mypy
 Provides-Extra: dev-noxfile
 Provides-Extra: dev-pylint
 Provides-Extra: dev-pytest
```

### Comparing `frequenz-client-dispatch-0.2.0/src/frequenz_client_dispatch.egg-info/SOURCES.txt` & `frequenz-client-dispatch-0.3.0/src/frequenz_client_dispatch.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 LICENSE
 MANIFEST.in
 README.md
 RELEASE_NOTES.md
 pyproject.toml
 src/frequenz/client/conftest.py
 src/frequenz/client/dispatch/__init__.py
+src/frequenz/client/dispatch/__main__.py
+src/frequenz/client/dispatch/_cli_types.py
 src/frequenz/client/dispatch/_client.py
 src/frequenz/client/dispatch/_internal_types.py
 src/frequenz/client/dispatch/py.typed
 src/frequenz/client/dispatch/types.py
 src/frequenz/client/dispatch/test/__init__.py
 src/frequenz/client/dispatch/test/_service.py
 src/frequenz/client/dispatch/test/client.py
 src/frequenz/client/dispatch/test/generator.py
 src/frequenz_client_dispatch.egg-info/PKG-INFO
 src/frequenz_client_dispatch.egg-info/SOURCES.txt
 src/frequenz_client_dispatch.egg-info/dependency_links.txt
+src/frequenz_client_dispatch.egg-info/entry_points.txt
 src/frequenz_client_dispatch.egg-info/requires.txt
 src/frequenz_client_dispatch.egg-info/top_level.txt
```

### Comparing `frequenz-client-dispatch-0.2.0/src/frequenz_client_dispatch.egg-info/requires.txt` & `frequenz-client-dispatch-0.3.0/src/frequenz_client_dispatch.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,61 @@
 typing-extensions<5,>=4.6.1
 frequenz-api-dispatch<0.14,>=0.13.0
-frequenz-client-base<0.4.0,>=0.2.1
-frequenz-client-common<0.2.0,>=0.1.0
+frequenz-client-base<0.5.0,>=0.2.1
+frequenz-client-common<0.3.0,>=0.1.0
 grpcio<2,>=1.54.2
 
+[cli]
+asyncclick==8.1.7.2
+prompt-toolkit==3.0.45
+parsedatetime==2.6
+tzlocal==5.2
+
 [dev]
 frequenz-client-dispatch[dev-flake8,dev-formatting,dev-mkdocs,dev-mypy,dev-noxfile,dev-pylint,dev-pytest]
 
 [dev-flake8]
 flake8==7.0.0
 flake8-docstrings==1.7.0
 flake8-pyproject==1.2.3
 pydoclint==0.4.1
 pydocstyle==6.3.0
 
 [dev-formatting]
-black==24.3.0
+black==24.4.2
 isort==5.13.2
 
 [dev-mkdocs]
-black==24.3.0
+black==24.4.2
 Markdown==3.6
-mike==2.0.0
+mike==2.1.1
 mkdocs-gen-files==0.5.0
 mkdocs-literate-nav==0.6.1
 mkdocs-macros-plugin==1.0.5
-mkdocs-material==9.5.17
-mkdocstrings[python]==0.24.1
-frequenz-repo-config[lib]==0.9.1
+mkdocs-material==9.5.25
+mkdocstrings[python]==0.25.1
+frequenz-repo-config[lib]==0.9.2
 
 [dev-mypy]
-mypy==1.9.0
+mypy==1.10.0
 types-Markdown==3.6.0.20240316
-frequenz-client-dispatch[dev-mkdocs,dev-noxfile,dev-pytest]
+frequenz-client-dispatch[cli,dev-mkdocs,dev-noxfile,dev-pytest]
 grpc-stubs==1.53.0.5
 types-protobuf==5.26.0.20240422
 
 [dev-noxfile]
-nox==2024.3.2
-frequenz-repo-config[lib]==0.9.1
+nox==2024.4.15
+frequenz-repo-config[lib]==0.9.2
 
 [dev-pylint]
-pylint==3.1.0
-frequenz-client-dispatch[dev-mkdocs,dev-noxfile,dev-pytest]
+pylint==3.2.2
+frequenz-client-dispatch[cli,dev-mkdocs,dev-noxfile,dev-pytest]
 frequenz-api-dispatch<0.14,>=0.13.0
 
 [dev-pytest]
-pytest==8.1.1
-frequenz-repo-config[extra-lint-examples]==0.9.1
+pytest==8.2.1
+frequenz-repo-config[extra-lint-examples]==0.9.2
 pytest-mock==3.14.0
-pytest-asyncio==0.23.6
+pytest-asyncio==0.23.7
 async-solipsism==0.6
-hypothesis==6.100.0
-sybil==6.0.3
+hypothesis==6.103.0
+frequenz-client-dispatch[cli]
```

