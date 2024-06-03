# Comparing `tmp/qctrl_workflow_client-3.1.1.tar.gz` & `tmp/qctrl_workflow_client-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qctrl_workflow_client-3.1.1.tar", max compression
+gzip compressed data, was "qctrl_workflow_client-4.0.0.tar", max compression
```

## Comparing `qctrl_workflow_client-3.1.1.tar` & `qctrl_workflow_client-4.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    36587 2024-05-29 06:32:39.870887 qctrl_workflow_client-3.1.1/LICENSE
--rw-r--r--   0        0        0      223 2024-05-29 06:32:39.870887 qctrl_workflow_client-3.1.1/README.md
--rw-r--r--   0        0        0     2784 2024-05-29 06:33:03.782964 qctrl_workflow_client-3.1.1/pyproject.toml
--rw-r--r--   0        0        0      954 2024-05-29 06:33:03.786964 qctrl_workflow_client-3.1.1/qctrlworkflowclient/__init__.py
--rw-r--r--   0        0        0     3311 2024-05-29 06:32:39.874887 qctrl_workflow_client-3.1.1/qctrlworkflowclient/defaults.py
--rw-r--r--   0        0        0     4944 2024-05-29 06:32:39.874887 qctrl_workflow_client-3.1.1/qctrlworkflowclient/functions.py
--rw-r--r--   0        0        0     1583 2024-05-29 06:32:39.874887 qctrl_workflow_client-3.1.1/qctrlworkflowclient/globals.py
--rw-r--r--   0        0        0      969 2024-05-29 06:32:39.874887 qctrl_workflow_client-3.1.1/qctrlworkflowclient/products.py
--rw-r--r--   0        0        0      638 2024-05-29 06:33:03.790964 qctrl_workflow_client-3.1.1/qctrlworkflowclient/router/__init__.py
--rw-r--r--   0        0        0    24063 2024-05-29 06:32:39.874887 qctrl_workflow_client-3.1.1/qctrlworkflowclient/router/api.py
--rw-r--r--   0        0        0     1206 2024-05-29 06:32:39.874887 qctrl_workflow_client-3.1.1/qctrlworkflowclient/router/base.py
--rw-r--r--   0        0        0     1201 2024-05-29 06:32:39.874887 qctrl_workflow_client-3.1.1/qctrlworkflowclient/router/local.py
--rw-r--r--   0        0        0     3332 2024-05-29 06:32:39.874887 qctrl_workflow_client-3.1.1/qctrlworkflowclient/settings.py
--rw-r--r--   0        0        0     5361 2024-05-29 06:32:39.874887 qctrl_workflow_client-3.1.1/qctrlworkflowclient/utils.py
--rw-r--r--   0        0        0     2489 1970-01-01 00:00:00.000000 qctrl_workflow_client-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0    36587 2024-06-03 01:26:29.111962 qctrl_workflow_client-4.0.0/LICENSE
+-rw-r--r--   0        0        0      223 2024-06-03 01:26:29.111962 qctrl_workflow_client-4.0.0/README.md
+-rw-r--r--   0        0        0     2786 2024-06-03 01:26:52.424125 qctrl_workflow_client-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0      954 2024-06-03 01:26:52.432125 qctrl_workflow_client-4.0.0/qctrlworkflowclient/__init__.py
+-rw-r--r--   0        0        0     3311 2024-06-03 01:26:29.111962 qctrl_workflow_client-4.0.0/qctrlworkflowclient/defaults.py
+-rw-r--r--   0        0        0     4944 2024-06-03 01:26:29.111962 qctrl_workflow_client-4.0.0/qctrlworkflowclient/functions.py
+-rw-r--r--   0        0        0     1583 2024-06-03 01:26:29.111962 qctrl_workflow_client-4.0.0/qctrlworkflowclient/globals.py
+-rw-r--r--   0        0        0      969 2024-06-03 01:26:29.111962 qctrl_workflow_client-4.0.0/qctrlworkflowclient/products.py
+-rw-r--r--   0        0        0      638 2024-06-03 01:26:52.432125 qctrl_workflow_client-4.0.0/qctrlworkflowclient/router/__init__.py
+-rw-r--r--   0        0        0    23750 2024-06-03 01:26:29.111962 qctrl_workflow_client-4.0.0/qctrlworkflowclient/router/api.py
+-rw-r--r--   0        0        0     1206 2024-06-03 01:26:29.111962 qctrl_workflow_client-4.0.0/qctrlworkflowclient/router/base.py
+-rw-r--r--   0        0        0     1201 2024-06-03 01:26:29.111962 qctrl_workflow_client-4.0.0/qctrlworkflowclient/router/local.py
+-rw-r--r--   0        0        0     3332 2024-06-03 01:26:29.111962 qctrl_workflow_client-4.0.0/qctrlworkflowclient/settings.py
+-rw-r--r--   0        0        0     5361 2024-06-03 01:26:29.111962 qctrl_workflow_client-4.0.0/qctrlworkflowclient/utils.py
+-rw-r--r--   0        0        0     2491 1970-01-01 00:00:00.000000 qctrl_workflow_client-4.0.0/PKG-INFO
```

### Comparing `qctrl_workflow_client-3.1.1/LICENSE` & `qctrl_workflow_client-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qctrl_workflow_client-3.1.1/pyproject.toml` & `qctrl_workflow_client-4.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qctrl-workflow-client"
-version = "3.1.1"
+version = "4.0.0"
 description = "Q-CTRL Client"
 license = "https://q-ctrl.com/terms"
 authors = ["Q-CTRL <support@q-ctrl.com>"]
 maintainers = ["Q-CTRL <support@q-ctrl.com>"]
 readme = "README.md"
 homepage = "https://q-ctrl.com"
 documentation = "https://docs.q-ctrl.com"
@@ -41,18 +41,18 @@
   "Development Status :: 5 - Production/Stable",
   "Environment :: Console",
   "Intended Audience :: Developers",
   "Intended Audience :: Education",
   "Intended Audience :: Science/Research",
   "Natural Language :: English",
   "Operating System :: OS Independent",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Topic :: Internet :: WWW/HTTP",
   "Topic :: Scientific/Engineering :: Physics",
   "Topic :: Scientific/Engineering :: Visualization",
   "Topic :: Software Development :: Embedded Systems",
   "Topic :: System :: Distributed Computing",
 ]
 packages = [{ include = "qctrlworkflowclient" }]
@@ -70,34 +70,34 @@
 
 [[tool.poetry.source]]
 name = "Q-CTRL PyPI"
 url = "https://pypi.q-ctrl.com/simple"
 priority = "primary"
 
 [tool.poetry.dependencies]
-python = ">=3.8, <3.12"
+python = ">=3.9, <3.13"
 tomli = "^2.0.1"
 importlib-metadata = "^6.8.0"
 gql = "^3.4.0"
 tenacity = "^8.1.0"
 requests = "^2.32.0"
 packaging = "^23.1.0"
-qctrl-commons = { version = "^22.0.0", source = "PyPI" }
-qctrl-client = { version = "^9.1.0", source = "PyPI" }
+qctrl-commons = { version = "^23.0.0", source = "PyPI" }
+qctrl-client = { version = "^10.0.0", source = "PyPI" }
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.3.0"
 isort = "^5.12.0"
 pre-commit = "^3.3.3"
 pylint = "^3.2.2"
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.10.0"
 pytest-xdist = "^3.2.1"
-qctrl-core-workflow-manager = "^3.2.0"
+qctrl-core-workflow-manager = "^4.0.0"
 
 [tool.isort]
 profile = "black"
 force_grid_wrap = "2"
 
 [tool.pytest.ini_options]
 addopts = "--cov=qctrlworkflowclient --cov-fail-under=80 --cov-report=term-missing:skip-covered"
```

### Comparing `qctrl_workflow_client-3.1.1/qctrlworkflowclient/__init__.py` & `qctrl_workflow_client-4.0.0/qctrlworkflowclient/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 #    https://q-ctrl.com/terms
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS. See the
 # License for the specific language.
 
-__version__ = "3.1.1"
+__version__ = "4.0.0"
 
 from .defaults import (
     get_authenticated_client_for_product,
     get_default_api_url,
     get_default_cli_auth,
     get_default_oidc_url,
 )
```

### Comparing `qctrl_workflow_client-3.1.1/qctrlworkflowclient/defaults.py` & `qctrl_workflow_client-4.0.0/qctrlworkflowclient/defaults.py`

 * *Files identical despite different names*

### Comparing `qctrl_workflow_client-3.1.1/qctrlworkflowclient/functions.py` & `qctrl_workflow_client-4.0.0/qctrlworkflowclient/functions.py`

 * *Files identical despite different names*

### Comparing `qctrl_workflow_client-3.1.1/qctrlworkflowclient/globals.py` & `qctrl_workflow_client-4.0.0/qctrlworkflowclient/globals.py`

 * *Files identical despite different names*

### Comparing `qctrl_workflow_client-3.1.1/qctrlworkflowclient/products.py` & `qctrl_workflow_client-4.0.0/qctrlworkflowclient/products.py`

 * *Files identical despite different names*

### Comparing `qctrl_workflow_client-3.1.1/qctrlworkflowclient/router/__init__.py` & `qctrl_workflow_client-4.0.0/qctrlworkflowclient/router/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl_workflow_client-3.1.1/qctrlworkflowclient/router/api.py` & `qctrl_workflow_client-4.0.0/qctrlworkflowclient/router/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,17 +45,14 @@
 
 from .base import BaseRouter
 
 # every 2s for the first 30s, then every 10s
 _POLL_WAIT_CHAIN = wait_chain(*[wait_fixed(2) for _ in range(15)] + [wait_fixed(10)])
 
 
-_MAX_PARALLEL_QUERY_COUNT = 5
-
-
 class ActionStatus(Enum):
     """
     Valid Action statuses.
     """
 
     SUCCESS = "SUCCESS"  # has completed
     FAILURE = "FAILURE"  # has failed
@@ -748,19 +745,14 @@
     def __exit__(self, exc_type, exc_value, traceback):
         self._router._parallel_task_collector = None
 
         # Do not try to call any functions upon an exception.
         if isinstance(exc_value, Exception):
             return False
 
-        if len(self._async_results) > _MAX_PARALLEL_QUERY_COUNT:
-            raise RuntimeError(
-                f"Number of parallel calculations: {len(self._async_results)}"
-                f" exceeds maximum allowed parallel count of {_MAX_PARALLEL_QUERY_COUNT}."
-            )
         for result in self._async_results:
             action = result.pop("async_result", None)
             assert action is not None
             response = self._router._fetch_action(action)
             if action.action_id != response.action_id:
                 raise RuntimeError(
                     f"Got the wrong result of action {response.action_id}, "
```

### Comparing `qctrl_workflow_client-3.1.1/qctrlworkflowclient/router/base.py` & `qctrl_workflow_client-4.0.0/qctrlworkflowclient/router/base.py`

 * *Files identical despite different names*

### Comparing `qctrl_workflow_client-3.1.1/qctrlworkflowclient/router/local.py` & `qctrl_workflow_client-4.0.0/qctrlworkflowclient/router/local.py`

 * *Files identical despite different names*

### Comparing `qctrl_workflow_client-3.1.1/qctrlworkflowclient/settings.py` & `qctrl_workflow_client-4.0.0/qctrlworkflowclient/settings.py`

 * *Files identical despite different names*

### Comparing `qctrl_workflow_client-3.1.1/qctrlworkflowclient/utils.py` & `qctrl_workflow_client-4.0.0/qctrlworkflowclient/utils.py`

 * *Files identical despite different names*

### Comparing `qctrl_workflow_client-3.1.1/PKG-INFO` & `qctrl_workflow_client-4.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: qctrl-workflow-client
-Version: 3.1.1
+Version: 4.0.0
 Summary: Q-CTRL Client
 Home-page: https://q-ctrl.com
 License: https://q-ctrl.com/terms
 Keywords: black opal,boulder opal,fire opal,nisq,open controls,q control,q ctrl,q-control,q-ctrl,qcontrol,qctrl,quantum,quantum algorithms,quantum circuits,quantum coding,quantum coding software,quantum computing,quantum control,quantum control software,quantum control theory,quantum engineering,quantum error correction,quantum firmware,quantum fundamentals,quantum sensing,qubit,qudit
 Author: Q-CTRL
 Author-email: support@q-ctrl.com
 Maintainer: Q-CTRL
 Maintainer-email: support@q-ctrl.com
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.9,<3.13
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Distributed Computing
 Requires-Dist: gql (>=3.4.0,<4.0.0)
 Requires-Dist: importlib-metadata (>=6.8.0,<7.0.0)
 Requires-Dist: packaging (>=23.1.0,<24.0.0)
-Requires-Dist: qctrl-client (>=9.1.0,<10.0.0)
-Requires-Dist: qctrl-commons (>=22.0.0,<23.0.0)
+Requires-Dist: qctrl-client (>=10.0.0,<11.0.0)
+Requires-Dist: qctrl-commons (>=23.0.0,<24.0.0)
 Requires-Dist: requests (>=2.32.0,<3.0.0)
 Requires-Dist: tenacity (>=8.1.0,<9.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Project-URL: Documentation, https://docs.q-ctrl.com
 Project-URL: Facebook, https://www.facebook.com/qctrl
 Project-URL: GitHub, https://github.com/qctrl
 Project-URL: LinkedIn, https://www.linkedin.com/company/q-ctrl/
```

