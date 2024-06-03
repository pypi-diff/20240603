# Comparing `tmp/dao_scripts-1.4.4.tar.gz` & `tmp/dao_scripts-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dao_scripts-1.4.4.tar", last modified: Mon Jun  3 11:17:32 2024, max compression
+gzip compressed data, was "dao_scripts-1.4.5.tar", last modified: Mon Jun  3 14:30:12 2024, max compression
```

## Comparing `dao_scripts-1.4.4.tar` & `dao_scripts-1.4.5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:32.975557 dao_scripts-1.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/.envrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:32.963557 dao_scripts-1.4.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:32.967557 dao_scripts-1.4.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/.github/workflows/update-datasets.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-06-03 11:17:32.975557 dao_scripts-1.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:32.975557 dao_scripts-1.4.4/dao_scripts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-06-03 11:17:32.000000 dao_scripts-1.4.4/dao_scripts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-06-03 11:17:32.000000 dao_scripts-1.4.4/dao_scripts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 11:17:32.000000 dao_scripts-1.4.4/dao_scripts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-06-03 11:17:32.000000 dao_scripts-1.4.4/dao_scripts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-03 11:17:32.000000 dao_scripts-1.4.4/dao_scripts.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-06-03 11:17:32.000000 dao_scripts-1.4.4/dao_scripts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-03 11:17:32.000000 dao_scripts-1.4.4/dao_scripts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-06-03 11:17:32.975557 dao_scripts-1.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:32.971557 dao_scripts-1.4.4/src/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-03 11:17:32.000000 dao_scripts-1.4.4/src/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:32.971557 dao_scripts-1.4.4/src/aragon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/aragon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/aragon/dao_names.json
--rw-r--r--   0 runner    (1001) docker     (127)     8163 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/aragon/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/argparser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:32.971557 dao_scripts-1.4.4/src/common/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/common/api_requester.py
--rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/common/blockscout.py
--rw-r--r--   0 runner    (1001) docker     (127)    10874 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/common/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/common/cryptocompare.py
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/common/thegraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:32.971557 dao_scripts-1.4.4/src/daohaus/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/daohaus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7549 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/daohaus/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:32.971557 dao_scripts-1.4.4/src/daostack/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/daostack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10144 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/daostack/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/endpoints.json
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/logging.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5989 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:32.975557 dao_scripts-1.4.4/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/utils/uploadDataWarehouse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:32.975557 dao_scripts-1.4.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/test/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:30:12.291145 dao_scripts-1.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-06-03 14:29:57.000000 dao_scripts-1.4.5/.envrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:30:12.283145 dao_scripts-1.4.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:30:12.283145 dao_scripts-1.4.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-06-03 14:29:57.000000 dao_scripts-1.4.5/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-06-03 14:29:57.000000 dao_scripts-1.4.5/.github/workflows/update-datasets.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-06-03 14:29:57.000000 dao_scripts-1.4.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-06-03 14:29:57.000000 dao_scripts-1.4.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-03 14:29:57.000000 dao_scripts-1.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-06-03 14:30:12.291145 dao_scripts-1.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-06-03 14:29:57.000000 dao_scripts-1.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:30:12.291145 dao_scripts-1.4.5/dao_scripts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-06-03 14:30:12.000000 dao_scripts-1.4.5/dao_scripts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-06-03 14:30:12.000000 dao_scripts-1.4.5/dao_scripts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 14:30:12.000000 dao_scripts-1.4.5/dao_scripts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-06-03 14:30:12.000000 dao_scripts-1.4.5/dao_scripts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-03 14:30:12.000000 dao_scripts-1.4.5/dao_scripts.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-06-03 14:30:12.000000 dao_scripts-1.4.5/dao_scripts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-03 14:30:12.000000 dao_scripts-1.4.5/dao_scripts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-06-03 14:29:57.000000 dao_scripts-1.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-06-03 14:30:12.295145 dao_scripts-1.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-06-03 14:29:57.000000 dao_scripts-1.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:30:12.287145 dao_scripts-1.4.5/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-06-03 14:29:57.000000 dao_scripts-1.4.5/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-06-03 14:29:57.000000 dao_scripts-1.4.5/src/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-03 14:30:12.000000 dao_scripts-1.4.5/src/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:30:12.287145 dao_scripts-1.4.5/src/aragon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:29:57.000000 dao_scripts-1.4.5/src/aragon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-06-03 14:29:57.000000 dao_scripts-1.4.5/src/aragon/dao_names.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8163 2024-06-03 14:29:57.000000 dao_scripts-1.4.5/src/aragon/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-06-03 14:29:57.000000 dao_scripts-1.4.5/src/argparser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:30:12.291145 dao_scripts-1.4.5/src/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-06-03 14:29:57.000000 dao_scripts-1.4.5/src/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-06-03 14:29:57.000000 dao_scripts-1.4.5/src/common/api_requester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-06-03 14:29:57.000000 dao_scripts-1.4.5/src/common/blockscout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10910 2024-06-03 14:29:57.000000 dao_scripts-1.4.5/src/common/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-06-03 14:29:57.000000 dao_scripts-1.4.5/src/common/cryptocompare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-06-03 14:29:57.000000 dao_scripts-1.4.5/src/common/thegraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-06-03 14:29:57.000000 dao_scripts-1.4.5/src/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:30:12.291145 dao_scripts-1.4.5/src/daohaus/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:29:57.000000 dao_scripts-1.4.5/src/daohaus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7549 2024-06-03 14:29:57.000000 dao_scripts-1.4.5/src/daohaus/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:30:12.291145 dao_scripts-1.4.5/src/daostack/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:29:57.000000 dao_scripts-1.4.5/src/daostack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10144 2024-06-03 14:29:57.000000 dao_scripts-1.4.5/src/daostack/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-06-03 14:29:57.000000 dao_scripts-1.4.5/src/endpoints.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-06-03 14:29:57.000000 dao_scripts-1.4.5/src/logging.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5989 2024-06-03 14:29:57.000000 dao_scripts-1.4.5/src/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-06-03 14:29:57.000000 dao_scripts-1.4.5/src/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:30:12.291145 dao_scripts-1.4.5/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:29:57.000000 dao_scripts-1.4.5/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-06-03 14:29:57.000000 dao_scripts-1.4.5/src/utils/uploadDataWarehouse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:30:12.291145 dao_scripts-1.4.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-06-03 14:29:57.000000 dao_scripts-1.4.5/test/test_placeholder.py
```

### Comparing `dao_scripts-1.4.4/.github/workflows/ci.yml` & `dao_scripts-1.4.5/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.4/.github/workflows/update-datasets.yml` & `dao_scripts-1.4.5/.github/workflows/update-datasets.yml`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.4/.gitignore` & `dao_scripts-1.4.5/.gitignore`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.4/CHANGELOG.md` & `dao_scripts-1.4.5/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.4/LICENSE` & `dao_scripts-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.4/PKG-INFO` & `dao_scripts-1.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dao-scripts
-Version: 1.4.4
+Version: 1.4.5
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
-Metadata-Version: 2.1 Name: dao-scripts Version: 1.4.4 Summary: "A tool to
+Metadata-Version: 2.1 Name: dao-scripts Version: 1.4.5 Summary: "A tool to
 download data to monitor DAO activity" Home-page: https://github.com/Grasia/
 dao-scripts Author: David DavÃ³ Author-email: ddavo@ucm.es Project-URL: Source,
 https://github.com/Grasia/dao-scripts Project-URL: Bug Tracker, https://
 github.com/Grasia/dao-scripts/issues Project-URL: Changelog, https://
 github.com/Grasia/dao-scripts/blob/main/CHANGELOG.md Classifier: Development
 Status :: 5 - Production/Stable Classifier: Environment :: Console Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
```

### Comparing `dao_scripts-1.4.4/README.md` & `dao_scripts-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.4/dao_scripts.egg-info/PKG-INFO` & `dao_scripts-1.4.5/dao_scripts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dao-scripts
-Version: 1.4.4
+Version: 1.4.5
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
-Metadata-Version: 2.1 Name: dao-scripts Version: 1.4.4 Summary: "A tool to
+Metadata-Version: 2.1 Name: dao-scripts Version: 1.4.5 Summary: "A tool to
 download data to monitor DAO activity" Home-page: https://github.com/Grasia/
 dao-scripts Author: David DavÃ³ Author-email: ddavo@ucm.es Project-URL: Source,
 https://github.com/Grasia/dao-scripts Project-URL: Bug Tracker, https://
 github.com/Grasia/dao-scripts/issues Project-URL: Changelog, https://
 github.com/Grasia/dao-scripts/blob/main/CHANGELOG.md Classifier: Development
 Status :: 5 - Production/Stable Classifier: Environment :: Console Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
```

### Comparing `dao_scripts-1.4.4/dao_scripts.egg-info/SOURCES.txt` & `dao_scripts-1.4.5/dao_scripts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.4/setup.cfg` & `dao_scripts-1.4.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.4/setup.py` & `dao_scripts-1.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.4/src/aragon/dao_names.json` & `dao_scripts-1.4.5/src/aragon/dao_names.json`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.4/src/aragon/runner.py` & `dao_scripts-1.4.5/src/aragon/runner.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.4/src/argparser.py` & `dao_scripts-1.4.5/src/argparser.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.4/src/common/api_requester.py` & `dao_scripts-1.4.5/src/common/api_requester.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.4/src/common/blockscout.py` & `dao_scripts-1.4.5/src/common/blockscout.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.4/src/common/common.py` & `dao_scripts-1.4.5/src/common/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -262,15 +262,15 @@
                             # Getting a block more recent than the one in the metadata (just to narrow down the search)
                             print("Requesting a block number...", end='\r')
                             blocks[c.network] = self.validated_block(
                                 network=c.network, 
                                 prev_block=None if force else metadata[c.collectorid].block,
                                 until_date=until_date,
                             )
-                            print(f"Using block {blocks[c.network].id} for {c.network} (ts: {blocks[c.network].timestamp.isoformat()})")
+                            print(f"Using block number {blocks[c.network].number} ({blocks[c.network].id}) for {c.network} (ts: {blocks[c.network].timestamp.isoformat()})")
 
                         print(f"Running collector {c.long_name} ({c.network})")
                         olderBlock = blocks[c.network] < metadata[c.collectorid].block
                         if not force and olderBlock:
                             print("Warning: Forcing because requesting an older block")
                             self.logger.warning("Forcing because using an older block")
```

### Comparing `dao_scripts-1.4.4/src/common/cryptocompare.py` & `dao_scripts-1.4.5/src/common/cryptocompare.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.4/src/common/thegraph.py` & `dao_scripts-1.4.5/src/common/thegraph.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,15 +185,15 @@
             return partial_query(self.query, {'_change_block': {'number_gte': prev_block.number}})
         else:
             return self.query
 
     def run(self, force=False, block: Optional[Block] = None, prev_block: Optional[Block] = None):
         self.logger.info(f"Running The Graph collector with block: {block}, prev_block: {prev_block}")
         if block and self._indexer_block:
-            assert self._indexer_block >= block, "Block number is not indexed yet"
+            assert self._indexer_block >= block, f"Block number {block} is not indexed yet ({self._indexer_block})"
         
         if block is None:
             block = Block()
         if prev_block is None or force:
             prev_block = Block()
 
         data = self._requester.n_requests(query=self.query_cb(prev_block), block_hash=block.id)
```

### Comparing `dao_scripts-1.4.4/src/config.py` & `dao_scripts-1.4.5/src/config.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.4/src/daohaus/runner.py` & `dao_scripts-1.4.5/src/daohaus/runner.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.4/src/daostack/runner.py` & `dao_scripts-1.4.5/src/daostack/runner.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.4/src/endpoints.json` & `dao_scripts-1.4.5/src/endpoints.json`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.4/src/logging.py` & `dao_scripts-1.4.5/src/logging.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.4/src/main.py` & `dao_scripts-1.4.5/src/main.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.4/src/metadata.py` & `dao_scripts-1.4.5/src/metadata.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.4/src/utils/uploadDataWarehouse.py` & `dao_scripts-1.4.5/src/utils/uploadDataWarehouse.py`

 * *Files identical despite different names*

