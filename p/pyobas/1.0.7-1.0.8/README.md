# Comparing `tmp/pyobas-1.0.7.tar.gz` & `tmp/pyobas-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobas-1.0.7.tar", last modified: Fri May 31 00:53:39 2024, max compression
+gzip compressed data, was "pyobas-1.0.8.tar", last modified: Mon Jun  3 14:54:36 2024, max compression
```

## Comparing `pyobas-1.0.7.tar` & `pyobas-1.0.8.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-31 00:53:39.676337 pyobas-1.0.7/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-05-31 00:53:27.000000 pyobas-1.0.7/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5167 2024-05-31 00:53:39.676337 pyobas-1.0.7/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3159 2024-05-31 00:53:27.000000 pyobas-1.0.7/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-31 00:53:39.668337 pyobas-1.0.7/pyobas/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      524 2024-05-31 00:53:27.000000 pyobas-1.0.7/pyobas/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      183 2024-05-31 00:53:27.000000 pyobas-1.0.7/pyobas/_version.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-31 00:53:39.672337 pyobas-1.0.7/pyobas/apis/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      593 2024-05-31 00:53:27.000000 pyobas-1.0.7/pyobas/apis/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      643 2024-05-31 00:53:27.000000 pyobas-1.0.7/pyobas/apis/attack_pattern.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      532 2024-05-31 00:53:27.000000 pyobas-1.0.7/pyobas/apis/collector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      516 2024-05-31 00:53:27.000000 pyobas-1.0.7/pyobas/apis/document.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      492 2024-05-31 00:53:27.000000 pyobas-1.0.7/pyobas/apis/endpoint.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      890 2024-05-31 00:53:27.000000 pyobas-1.0.7/pyobas/apis/inject.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2000 2024-05-31 00:53:27.000000 pyobas-1.0.7/pyobas/apis/inject_expectation.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      722 2024-05-31 00:53:27.000000 pyobas-1.0.7/pyobas/apis/injector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2024-05-31 00:53:27.000000 pyobas-1.0.7/pyobas/apis/kill_chain_phase.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      397 2024-05-31 00:53:27.000000 pyobas-1.0.7/pyobas/apis/me.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      263 2024-05-31 00:53:27.000000 pyobas-1.0.7/pyobas/apis/organization.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      788 2024-05-31 00:53:27.000000 pyobas-1.0.7/pyobas/apis/team.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      893 2024-05-31 00:53:27.000000 pyobas-1.0.7/pyobas/apis/user.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-31 00:53:39.672337 pyobas-1.0.7/pyobas/backends/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2024-05-31 00:53:27.000000 pyobas-1.0.7/pyobas/backends/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4328 2024-05-31 00:53:27.000000 pyobas-1.0.7/pyobas/backends/backend.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      842 2024-05-31 00:53:27.000000 pyobas-1.0.7/pyobas/backends/protocol.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10756 2024-05-31 00:53:27.000000 pyobas-1.0.7/pyobas/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16261 2024-05-31 00:53:27.000000 pyobas-1.0.7/pyobas/client.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-31 00:53:39.672337 pyobas-1.0.7/pyobas/contracts/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      103 2024-05-31 00:53:27.000000 pyobas-1.0.7/pyobas/contracts/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2024-05-31 00:53:27.000000 pyobas-1.0.7/pyobas/contracts/contract_builder.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5609 2024-05-31 00:53:27.000000 pyobas-1.0.7/pyobas/contracts/contract_config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      451 2024-05-31 00:53:27.000000 pyobas-1.0.7/pyobas/contracts/contract_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4208 2024-05-31 00:53:27.000000 pyobas-1.0.7/pyobas/contracts/variable_helper.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2525 2024-05-31 00:53:27.000000 pyobas-1.0.7/pyobas/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15494 2024-05-31 00:53:27.000000 pyobas-1.0.7/pyobas/helpers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6777 2024-05-31 00:53:27.000000 pyobas-1.0.7/pyobas/mixins.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5297 2024-05-31 00:53:27.000000 pyobas-1.0.7/pyobas/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-31 00:53:39.672337 pyobas-1.0.7/pyobas.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5167 2024-05-31 00:53:39.000000 pyobas-1.0.7/pyobas.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      914 2024-05-31 00:53:39.000000 pyobas-1.0.7/pyobas.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-31 00:53:39.000000 pyobas-1.0.7/pyobas.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      596 2024-05-31 00:53:39.000000 pyobas-1.0.7/pyobas.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2024-05-31 00:53:39.000000 pyobas-1.0.7/pyobas.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2024-05-31 00:53:27.000000 pyobas-1.0.7/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1604 2024-05-31 00:53:39.676337 pyobas-1.0.7/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-06-03 14:54:36.242806 pyobas-1.0.8/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-06-03 14:54:21.000000 pyobas-1.0.8/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5167 2024-06-03 14:54:36.242806 pyobas-1.0.8/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3159 2024-06-03 14:54:21.000000 pyobas-1.0.8/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-06-03 14:54:36.234805 pyobas-1.0.8/pyobas/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      524 2024-06-03 14:54:21.000000 pyobas-1.0.8/pyobas/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      183 2024-06-03 14:54:21.000000 pyobas-1.0.8/pyobas/_version.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-06-03 14:54:36.238806 pyobas-1.0.8/pyobas/apis/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      593 2024-06-03 14:54:21.000000 pyobas-1.0.8/pyobas/apis/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      643 2024-06-03 14:54:21.000000 pyobas-1.0.8/pyobas/apis/attack_pattern.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      532 2024-06-03 14:54:21.000000 pyobas-1.0.8/pyobas/apis/collector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      516 2024-06-03 14:54:21.000000 pyobas-1.0.8/pyobas/apis/document.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      492 2024-06-03 14:54:21.000000 pyobas-1.0.8/pyobas/apis/endpoint.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      890 2024-06-03 14:54:21.000000 pyobas-1.0.8/pyobas/apis/inject.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2000 2024-06-03 14:54:21.000000 pyobas-1.0.8/pyobas/apis/inject_expectation.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      722 2024-06-03 14:54:21.000000 pyobas-1.0.8/pyobas/apis/injector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2024-06-03 14:54:21.000000 pyobas-1.0.8/pyobas/apis/kill_chain_phase.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      397 2024-06-03 14:54:21.000000 pyobas-1.0.8/pyobas/apis/me.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      263 2024-06-03 14:54:21.000000 pyobas-1.0.8/pyobas/apis/organization.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      788 2024-06-03 14:54:21.000000 pyobas-1.0.8/pyobas/apis/team.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      893 2024-06-03 14:54:21.000000 pyobas-1.0.8/pyobas/apis/user.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-06-03 14:54:36.238806 pyobas-1.0.8/pyobas/backends/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2024-06-03 14:54:21.000000 pyobas-1.0.8/pyobas/backends/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4328 2024-06-03 14:54:21.000000 pyobas-1.0.8/pyobas/backends/backend.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      842 2024-06-03 14:54:21.000000 pyobas-1.0.8/pyobas/backends/protocol.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10756 2024-06-03 14:54:21.000000 pyobas-1.0.8/pyobas/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16261 2024-06-03 14:54:21.000000 pyobas-1.0.8/pyobas/client.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-06-03 14:54:36.238806 pyobas-1.0.8/pyobas/contracts/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      103 2024-06-03 14:54:21.000000 pyobas-1.0.8/pyobas/contracts/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2024-06-03 14:54:21.000000 pyobas-1.0.8/pyobas/contracts/contract_builder.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5609 2024-06-03 14:54:21.000000 pyobas-1.0.8/pyobas/contracts/contract_config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      451 2024-06-03 14:54:21.000000 pyobas-1.0.8/pyobas/contracts/contract_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4208 2024-06-03 14:54:21.000000 pyobas-1.0.8/pyobas/contracts/variable_helper.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2525 2024-06-03 14:54:21.000000 pyobas-1.0.8/pyobas/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15494 2024-06-03 14:54:21.000000 pyobas-1.0.8/pyobas/helpers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6777 2024-06-03 14:54:21.000000 pyobas-1.0.8/pyobas/mixins.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5297 2024-06-03 14:54:21.000000 pyobas-1.0.8/pyobas/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-06-03 14:54:36.242806 pyobas-1.0.8/pyobas.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5167 2024-06-03 14:54:36.000000 pyobas-1.0.8/pyobas.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      914 2024-06-03 14:54:36.000000 pyobas-1.0.8/pyobas.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-06-03 14:54:36.000000 pyobas-1.0.8/pyobas.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      596 2024-06-03 14:54:36.000000 pyobas-1.0.8/pyobas.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2024-06-03 14:54:36.000000 pyobas-1.0.8/pyobas.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2024-06-03 14:54:21.000000 pyobas-1.0.8/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1604 2024-06-03 14:54:36.242806 pyobas-1.0.8/setup.cfg
```

### Comparing `pyobas-1.0.7/LICENSE` & `pyobas-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.7/PKG-INFO` & `pyobas-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobas
-Version: 1.0.7
+Version: 1.0.8
 Summary: Python API client for OpenBAS.
 Home-page: https://github.com/OpenBAS-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyobas-1.0.7/README.md` & `pyobas-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.7/pyobas/__init__.py` & `pyobas-1.0.8/pyobas/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-__version__ = "1.0.7"
+__version__ = "1.0.8"
 
 from pyobas._version import (  # noqa: F401
     __author__,
     __copyright__,
     __email__,
     __license__,
     __title__,
```

### Comparing `pyobas-1.0.7/pyobas/apis/__init__.py` & `pyobas-1.0.8/pyobas/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.7/pyobas/apis/attack_pattern.py` & `pyobas-1.0.8/pyobas/apis/attack_pattern.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.7/pyobas/apis/collector.py` & `pyobas-1.0.8/pyobas/apis/collector.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.7/pyobas/apis/document.py` & `pyobas-1.0.8/pyobas/apis/document.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.7/pyobas/apis/inject.py` & `pyobas-1.0.8/pyobas/apis/inject.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.7/pyobas/apis/inject_expectation.py` & `pyobas-1.0.8/pyobas/apis/inject_expectation.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.7/pyobas/apis/injector.py` & `pyobas-1.0.8/pyobas/apis/injector.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.7/pyobas/apis/kill_chain_phase.py` & `pyobas-1.0.8/pyobas/apis/kill_chain_phase.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.7/pyobas/apis/team.py` & `pyobas-1.0.8/pyobas/apis/team.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.7/pyobas/apis/user.py` & `pyobas-1.0.8/pyobas/apis/user.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.7/pyobas/backends/backend.py` & `pyobas-1.0.8/pyobas/backends/backend.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.7/pyobas/backends/protocol.py` & `pyobas-1.0.8/pyobas/backends/protocol.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.7/pyobas/base.py` & `pyobas-1.0.8/pyobas/base.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.7/pyobas/client.py` & `pyobas-1.0.8/pyobas/client.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.7/pyobas/contracts/contract_builder.py` & `pyobas-1.0.8/pyobas/contracts/contract_builder.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.7/pyobas/contracts/contract_config.py` & `pyobas-1.0.8/pyobas/contracts/contract_config.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.7/pyobas/contracts/variable_helper.py` & `pyobas-1.0.8/pyobas/contracts/variable_helper.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.7/pyobas/exceptions.py` & `pyobas-1.0.8/pyobas/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.7/pyobas/helpers.py` & `pyobas-1.0.8/pyobas/helpers.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.7/pyobas/mixins.py` & `pyobas-1.0.8/pyobas/mixins.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.7/pyobas/utils.py` & `pyobas-1.0.8/pyobas/utils.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.7/pyobas.egg-info/PKG-INFO` & `pyobas-1.0.8/pyobas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobas
-Version: 1.0.7
+Version: 1.0.8
 Summary: Python API client for OpenBAS.
 Home-page: https://github.com/OpenBAS-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyobas-1.0.7/pyobas.egg-info/SOURCES.txt` & `pyobas-1.0.8/pyobas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.7/pyobas.egg-info/requires.txt` & `pyobas-1.0.8/pyobas.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.7/pyproject.toml` & `pyobas-1.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.7/setup.cfg` & `pyobas-1.0.8/setup.cfg`

 * *Files identical despite different names*

