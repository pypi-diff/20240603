# Comparing `tmp/dao_scripts-1.4.2.tar.gz` & `tmp/dao_scripts-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dao_scripts-1.4.2.tar", last modified: Mon Jun  3 09:45:45 2024, max compression
+gzip compressed data, was "dao_scripts-1.4.3.tar", last modified: Mon Jun  3 09:59:31 2024, max compression
```

## Comparing `dao_scripts-1.4.2.tar` & `dao_scripts-1.4.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:45:45.785073 dao_scripts-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/.envrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:45:45.777073 dao_scripts-1.4.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:45:45.777073 dao_scripts-1.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/.github/workflows/update-datasets.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-06-03 09:45:45.785073 dao_scripts-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:45:45.785073 dao_scripts-1.4.2/dao_scripts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-06-03 09:45:45.000000 dao_scripts-1.4.2/dao_scripts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-06-03 09:45:45.000000 dao_scripts-1.4.2/dao_scripts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 09:45:45.000000 dao_scripts-1.4.2/dao_scripts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-06-03 09:45:45.000000 dao_scripts-1.4.2/dao_scripts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-03 09:45:45.000000 dao_scripts-1.4.2/dao_scripts.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-06-03 09:45:45.000000 dao_scripts-1.4.2/dao_scripts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-03 09:45:45.000000 dao_scripts-1.4.2/dao_scripts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-06-03 09:45:45.785073 dao_scripts-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:45:45.781073 dao_scripts-1.4.2/src/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-03 09:45:45.000000 dao_scripts-1.4.2/src/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:45:45.781073 dao_scripts-1.4.2/src/aragon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/aragon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/aragon/dao_names.json
--rw-r--r--   0 runner    (1001) docker     (127)     8163 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/aragon/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/argparser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:45:45.781073 dao_scripts-1.4.2/src/common/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/common/api_requester.py
--rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/common/blockscout.py
--rw-r--r--   0 runner    (1001) docker     (127)    10763 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/common/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/common/cryptocompare.py
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/common/thegraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:45:45.781073 dao_scripts-1.4.2/src/daohaus/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/daohaus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7549 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/daohaus/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:45:45.781073 dao_scripts-1.4.2/src/daostack/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/daostack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10144 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/daostack/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/endpoints.json
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/logging.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5751 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:45:45.781073 dao_scripts-1.4.2/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/utils/uploadDataWarehouse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:45:45.785073 dao_scripts-1.4.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/test/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:59:31.866890 dao_scripts-1.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/.envrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:59:31.854889 dao_scripts-1.4.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:59:31.858890 dao_scripts-1.4.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/.github/workflows/update-datasets.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-06-03 09:59:31.866890 dao_scripts-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:59:31.862890 dao_scripts-1.4.3/dao_scripts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-06-03 09:59:31.000000 dao_scripts-1.4.3/dao_scripts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-06-03 09:59:31.000000 dao_scripts-1.4.3/dao_scripts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 09:59:31.000000 dao_scripts-1.4.3/dao_scripts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-06-03 09:59:31.000000 dao_scripts-1.4.3/dao_scripts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-03 09:59:31.000000 dao_scripts-1.4.3/dao_scripts.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-06-03 09:59:31.000000 dao_scripts-1.4.3/dao_scripts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-03 09:59:31.000000 dao_scripts-1.4.3/dao_scripts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-06-03 09:59:31.866890 dao_scripts-1.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:59:31.862890 dao_scripts-1.4.3/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-03 09:59:31.000000 dao_scripts-1.4.3/src/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:59:31.862890 dao_scripts-1.4.3/src/aragon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/aragon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/aragon/dao_names.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8163 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/aragon/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/argparser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:59:31.862890 dao_scripts-1.4.3/src/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/common/api_requester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/common/blockscout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10874 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/common/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/common/cryptocompare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/common/thegraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:59:31.862890 dao_scripts-1.4.3/src/daohaus/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/daohaus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7549 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/daohaus/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:59:31.862890 dao_scripts-1.4.3/src/daostack/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/daostack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10144 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/daostack/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/endpoints.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/logging.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5751 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:59:31.862890 dao_scripts-1.4.3/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/utils/uploadDataWarehouse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:59:31.862890 dao_scripts-1.4.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/test/test_placeholder.py
```

### Comparing `dao_scripts-1.4.2/.github/workflows/ci.yml` & `dao_scripts-1.4.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.2/.github/workflows/update-datasets.yml` & `dao_scripts-1.4.3/.github/workflows/update-datasets.yml`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.2/.gitignore` & `dao_scripts-1.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.2/CHANGELOG.md` & `dao_scripts-1.4.3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.2/LICENSE` & `dao_scripts-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.2/PKG-INFO` & `dao_scripts-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dao-scripts
-Version: 1.4.2
+Version: 1.4.3
 Summary: "A tool to download data to monitor DAO activity"
 Home-page: https://github.com/Grasia/dao-scripts
 Author: David Davó
 Author-email: ddavo@ucm.es
 Project-URL: Source, https://github.com/Grasia/dao-scripts
 Project-URL: Bug Tracker, https://github.com/Grasia/dao-scripts/issues
 Project-URL: Changelog, https://github.com/Grasia/dao-scripts/blob/main/CHANGELOG.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dao-scripts Version: 1.4.2 Summary: "A tool to
+Metadata-Version: 2.1 Name: dao-scripts Version: 1.4.3 Summary: "A tool to
 download data to monitor DAO activity" Home-page: https://github.com/Grasia/
 dao-scripts Author: David DavÃ³ Author-email: ddavo@ucm.es Project-URL: Source,
 https://github.com/Grasia/dao-scripts Project-URL: Bug Tracker, https://
 github.com/Grasia/dao-scripts/issues Project-URL: Changelog, https://
 github.com/Grasia/dao-scripts/blob/main/CHANGELOG.md Classifier: Development
 Status :: 5 - Production/Stable Classifier: Environment :: Console Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
```

### Comparing `dao_scripts-1.4.2/README.md` & `dao_scripts-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.2/dao_scripts.egg-info/PKG-INFO` & `dao_scripts-1.4.3/dao_scripts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dao-scripts
-Version: 1.4.2
+Version: 1.4.3
 Summary: "A tool to download data to monitor DAO activity"
 Home-page: https://github.com/Grasia/dao-scripts
 Author: David Davó
 Author-email: ddavo@ucm.es
 Project-URL: Source, https://github.com/Grasia/dao-scripts
 Project-URL: Bug Tracker, https://github.com/Grasia/dao-scripts/issues
 Project-URL: Changelog, https://github.com/Grasia/dao-scripts/blob/main/CHANGELOG.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dao-scripts Version: 1.4.2 Summary: "A tool to
+Metadata-Version: 2.1 Name: dao-scripts Version: 1.4.3 Summary: "A tool to
 download data to monitor DAO activity" Home-page: https://github.com/Grasia/
 dao-scripts Author: David DavÃ³ Author-email: ddavo@ucm.es Project-URL: Source,
 https://github.com/Grasia/dao-scripts Project-URL: Bug Tracker, https://
 github.com/Grasia/dao-scripts/issues Project-URL: Changelog, https://
 github.com/Grasia/dao-scripts/blob/main/CHANGELOG.md Classifier: Development
 Status :: 5 - Production/Stable Classifier: Environment :: Console Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
```

### Comparing `dao_scripts-1.4.2/dao_scripts.egg-info/SOURCES.txt` & `dao_scripts-1.4.3/dao_scripts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.2/setup.cfg` & `dao_scripts-1.4.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.2/setup.py` & `dao_scripts-1.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.2/src/aragon/dao_names.json` & `dao_scripts-1.4.3/src/aragon/dao_names.json`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.2/src/aragon/runner.py` & `dao_scripts-1.4.3/src/aragon/runner.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.2/src/argparser.py` & `dao_scripts-1.4.3/src/argparser.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.2/src/common/api_requester.py` & `dao_scripts-1.4.3/src/common/api_requester.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.2/src/common/blockscout.py` & `dao_scripts-1.4.3/src/common/blockscout.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.2/src/common/common.py` & `dao_scripts-1.4.3/src/common/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,15 +246,15 @@
         print("Verifying collectors")
         verified = self._verifyCollectors(self.filterCollectors(
             networks=networks,
             long_names=collectors
         ))
         if not verified:
             # Nothing to do
-            return
+            raise ValueError(f"No collectors for runner {self.name} were valid. Please don't use this runner or fix the errors.")
 
         with RunnerMetadata(self) as metadata:
             print(f'--- Updating {self.name} datawarehouse ---')            
             blocks: dict[str, Block] = {}
             for c in verified:
                 try:
                     if isinstance(c, NetworkCollector):
```

### Comparing `dao_scripts-1.4.2/src/common/cryptocompare.py` & `dao_scripts-1.4.3/src/common/cryptocompare.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.2/src/common/thegraph.py` & `dao_scripts-1.4.3/src/common/thegraph.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.2/src/config.py` & `dao_scripts-1.4.3/src/config.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.2/src/daohaus/runner.py` & `dao_scripts-1.4.3/src/daohaus/runner.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.2/src/daostack/runner.py` & `dao_scripts-1.4.3/src/daostack/runner.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.2/src/endpoints.json` & `dao_scripts-1.4.3/src/endpoints.json`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.2/src/logging.py` & `dao_scripts-1.4.3/src/logging.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.2/src/main.py` & `dao_scripts-1.4.3/src/main.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.2/src/metadata.py` & `dao_scripts-1.4.3/src/metadata.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.2/src/utils/uploadDataWarehouse.py` & `dao_scripts-1.4.3/src/utils/uploadDataWarehouse.py`

 * *Files identical despite different names*

