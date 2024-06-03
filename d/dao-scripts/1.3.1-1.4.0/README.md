# Comparing `tmp/dao_scripts-1.3.1.tar.gz` & `tmp/dao_scripts-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dao_scripts-1.3.1.tar", last modified: Mon May 27 09:00:47 2024, max compression
+gzip compressed data, was "dao_scripts-1.4.0.tar", last modified: Mon Jun  3 09:20:22 2024, max compression
```

## Comparing `dao_scripts-1.3.1.tar` & `dao_scripts-1.4.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:00:47.603149 dao_scripts-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/.envrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:00:47.595149 dao_scripts-1.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:00:47.599149 dao_scripts-1.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/.github/workflows/update-datasets.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-05-27 09:00:47.603149 dao_scripts-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:00:47.603149 dao_scripts-1.3.1/dao_scripts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-05-27 09:00:47.000000 dao_scripts-1.3.1/dao_scripts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-27 09:00:47.000000 dao_scripts-1.3.1/dao_scripts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 09:00:47.000000 dao_scripts-1.3.1/dao_scripts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-27 09:00:47.000000 dao_scripts-1.3.1/dao_scripts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-27 09:00:47.000000 dao_scripts-1.3.1/dao_scripts.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-27 09:00:47.000000 dao_scripts-1.3.1/dao_scripts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-27 09:00:47.000000 dao_scripts-1.3.1/dao_scripts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-27 09:00:47.607149 dao_scripts-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:00:47.599149 dao_scripts-1.3.1/src/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-27 09:00:47.000000 dao_scripts-1.3.1/src/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:00:47.603149 dao_scripts-1.3.1/src/aragon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/aragon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/aragon/dao_names.json
--rw-r--r--   0 runner    (1001) docker     (127)     8163 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/aragon/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/argparser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:00:47.603149 dao_scripts-1.3.1/src/common/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/common/api_requester.py
--rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/common/blockscout.py
--rw-r--r--   0 runner    (1001) docker     (127)    10763 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/common/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/common/cryptocompare.py
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/common/thegraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:00:47.603149 dao_scripts-1.3.1/src/daohaus/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/daohaus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7549 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/daohaus/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:00:47.603149 dao_scripts-1.3.1/src/daostack/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/daostack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10144 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/daostack/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/endpoints.json
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/logging.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5588 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:00:47.603149 dao_scripts-1.3.1/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/src/utils/uploadDataWarehouse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:00:47.603149 dao_scripts-1.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-27 09:00:34.000000 dao_scripts-1.3.1/test/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:20:22.892581 dao_scripts-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/.envrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:20:22.880581 dao_scripts-1.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:20:22.884581 dao_scripts-1.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/.github/workflows/update-datasets.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-06-03 09:20:22.892581 dao_scripts-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:20:22.888581 dao_scripts-1.4.0/dao_scripts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-06-03 09:20:22.000000 dao_scripts-1.4.0/dao_scripts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-06-03 09:20:22.000000 dao_scripts-1.4.0/dao_scripts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 09:20:22.000000 dao_scripts-1.4.0/dao_scripts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-06-03 09:20:22.000000 dao_scripts-1.4.0/dao_scripts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-03 09:20:22.000000 dao_scripts-1.4.0/dao_scripts.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-06-03 09:20:22.000000 dao_scripts-1.4.0/dao_scripts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-03 09:20:22.000000 dao_scripts-1.4.0/dao_scripts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-06-03 09:20:22.892581 dao_scripts-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:20:22.888581 dao_scripts-1.4.0/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-03 09:20:22.000000 dao_scripts-1.4.0/src/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:20:22.888581 dao_scripts-1.4.0/src/aragon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/aragon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/aragon/dao_names.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8163 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/aragon/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/argparser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:20:22.888581 dao_scripts-1.4.0/src/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/common/api_requester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/common/blockscout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10763 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/common/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/common/cryptocompare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/common/thegraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:20:22.888581 dao_scripts-1.4.0/src/daohaus/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/daohaus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7549 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/daohaus/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:20:22.888581 dao_scripts-1.4.0/src/daostack/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/daostack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10144 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/daostack/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/endpoints.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/logging.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5751 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:20:22.888581 dao_scripts-1.4.0/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/utils/uploadDataWarehouse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:20:22.888581 dao_scripts-1.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/test/test_placeholder.py
```

### Comparing `dao_scripts-1.3.1/.github/workflows/ci.yml` & `dao_scripts-1.4.0/.github/workflows/ci.yml`

 * *Files 5% similar despite different names*

```diff
@@ -48,14 +48,18 @@
     needs: [package]
     if: github.ref == 'refs/heads/develop' || startsWith(github.ref, 'refs/tags/' )
     # Specifying a GitHub environment is optional, but strongly encouraged
     permissions:
       # IMPORTANT: this permission is mandatory for trusted publishing
       id-token: write
     steps:
+    - name: Skip Duplicate Actions
+      uses: fkirc/skip-duplicate-actions@v5
+      with:
+        concurrent_skipping: same_content_newer
     - name: Download built package
       uses: actions/download-artifact@v4
       with:
         name: dist
         path: ./dist/
     - name: Publish package
       uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `dao_scripts-1.3.1/.github/workflows/update-datasets.yml` & `dao_scripts-1.4.0/.github/workflows/update-datasets.yml`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.1/.gitignore` & `dao_scripts-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.1/CHANGELOG.md` & `dao_scripts-1.4.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
+## 1.4.0 - 2024-06-03
+- Fixed bug when process was killed
+- Updated endpoint network names
+
 ## 1.3.1 - 2024-05-27
 - Fixed bug with `--delete-force`
 
 ## 1.3.0 - 2024-05-24
 - Improved and standarized logging #10
 - The Graph Hosted Service sunsetting
   - Added DAOA_THE_GRAPH_API_KEY variable (now needed)
```

### Comparing `dao_scripts-1.3.1/LICENSE` & `dao_scripts-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.1/PKG-INFO` & `dao_scripts-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dao-scripts
-Version: 1.3.1
+Version: 1.4.0
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
-Metadata-Version: 2.1 Name: dao-scripts Version: 1.3.1 Summary: "A tool to
+Metadata-Version: 2.1 Name: dao-scripts Version: 1.4.0 Summary: "A tool to
 download data to monitor DAO activity" Home-page: https://github.com/Grasia/
 dao-scripts Author: David DavÃ³ Author-email: ddavo@ucm.es Project-URL: Source,
 https://github.com/Grasia/dao-scripts Project-URL: Bug Tracker, https://
 github.com/Grasia/dao-scripts/issues Project-URL: Changelog, https://
 github.com/Grasia/dao-scripts/blob/main/CHANGELOG.md Classifier: Development
 Status :: 5 - Production/Stable Classifier: Environment :: Console Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
```

### Comparing `dao_scripts-1.3.1/README.md` & `dao_scripts-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.1/dao_scripts.egg-info/PKG-INFO` & `dao_scripts-1.4.0/dao_scripts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dao-scripts
-Version: 1.3.1
+Version: 1.4.0
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
-Metadata-Version: 2.1 Name: dao-scripts Version: 1.3.1 Summary: "A tool to
+Metadata-Version: 2.1 Name: dao-scripts Version: 1.4.0 Summary: "A tool to
 download data to monitor DAO activity" Home-page: https://github.com/Grasia/
 dao-scripts Author: David DavÃ³ Author-email: ddavo@ucm.es Project-URL: Source,
 https://github.com/Grasia/dao-scripts Project-URL: Bug Tracker, https://
 github.com/Grasia/dao-scripts/issues Project-URL: Changelog, https://
 github.com/Grasia/dao-scripts/blob/main/CHANGELOG.md Classifier: Development
 Status :: 5 - Production/Stable Classifier: Environment :: Console Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
```

### Comparing `dao_scripts-1.3.1/dao_scripts.egg-info/SOURCES.txt` & `dao_scripts-1.4.0/dao_scripts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.1/setup.cfg` & `dao_scripts-1.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.1/setup.py` & `dao_scripts-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.1/src/aragon/dao_names.json` & `dao_scripts-1.4.0/src/aragon/dao_names.json`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.1/src/aragon/runner.py` & `dao_scripts-1.4.0/src/aragon/runner.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.1/src/argparser.py` & `dao_scripts-1.4.0/src/argparser.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.1/src/common/api_requester.py` & `dao_scripts-1.4.0/src/common/api_requester.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.1/src/common/blockscout.py` & `dao_scripts-1.4.0/src/common/blockscout.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.1/src/common/common.py` & `dao_scripts-1.4.0/src/common/common.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.1/src/common/cryptocompare.py` & `dao_scripts-1.4.0/src/common/cryptocompare.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.1/src/common/thegraph.py` & `dao_scripts-1.4.0/src/common/thegraph.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.1/src/config.py` & `dao_scripts-1.4.0/src/config.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.1/src/daohaus/runner.py` & `dao_scripts-1.4.0/src/daohaus/runner.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.1/src/daostack/runner.py` & `dao_scripts-1.4.0/src/daostack/runner.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.1/src/endpoints.json` & `dao_scripts-1.4.0/src/endpoints.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.42857142857142855%*

 * *Differences: {"'arbitrum-one'": "OrderedDict([('_blocks', 'AyY1GDtmAyavGWsdoHQ4vNoBCVWSqfDwHa6jPu5KdHgP'), "*

 * *                   "('daohaus', '2c41cggebRCMzFiDqoqDwShZtz4xYucsFKbQnEiXUTzY')])",*

 * * "'matic'": "OrderedDict([('_blocks', '4mJTujCUWKLd4SPBYE1YXbamfNSNRMyphk8tHzczYWf9'), ('daohaus', "*

 * *            "'AkzZk4BsvfNRkRDtzz7Bc8TgktTJN4uv9tgfCehhE6fB')])",*

 * * 'delete': "['polygon', 'arbitrum']"}*

```diff
@@ -1,26 +1,26 @@
 {
     "_theGraph": {
         "index-node": "https://api.thegraph.com/index-node/graphql"
     },
-    "arbitrum": {
+    "arbitrum-one": {
         "_blocks": "AyY1GDtmAyavGWsdoHQ4vNoBCVWSqfDwHa6jPu5KdHgP",
         "daohaus": "2c41cggebRCMzFiDqoqDwShZtz4xYucsFKbQnEiXUTzY"
     },
     "mainnet": {
         "_blocks": "9A6bkprqEG2XsZUYJ5B2XXp6ymz9fNcn4tVPxMWDztYC",
         "aragon": "QmduJYwyy3STKaZCEEHtxCQ9LMRYDPdfqYbgobRob6bDp7",
         "aragon_finance": "7pHfNgz8XYHH2Uu9RdqqP8G29BCqi1VRgo3cdLzz59HZ",
         "aragon_tokens": "EioF9792T18u3oqtt2Hfv5gYgw2Rp2qeqnrURP6deVHg",
         "aragon_voting": "GBsV7wbrW9gTBjJhvBpML5Gcadtaj1fEnapB6NujNaai",
         "blockscout": "https://blockscout.com/eth/mainnet/api",
         "daohaus": "2d3CDkKyxhpLDZRLWHMCvWp9cCYdWp4Y7g5ecaBmeqad",
         "daostack": "43HtV3dXRLPX7GKyV7f8GMLhevPXBmnSvpGBRKyfr53k"
     },
-    "polygon": {
+    "matic": {
         "_blocks": "4mJTujCUWKLd4SPBYE1YXbamfNSNRMyphk8tHzczYWf9",
         "daohaus": "AkzZk4BsvfNRkRDtzz7Bc8TgktTJN4uv9tgfCehhE6fB"
     },
     "xdai": {
         "_blocks": "D58aXwnRLfosFtRaVJAbAjjvKZ11bEsbdiDLkJJRdSC9",
         "blockscout": "https://blockscout.com/xdai/mainnet/api",
         "daohaus": "2GJY9uxsLQUCvgqSfy6QCLAJgM9P9kdxBUpwNcGs7nPR",
```

### Comparing `dao_scripts-1.3.1/src/logging.py` & `dao_scripts-1.4.0/src/logging.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.1/src/main.py` & `dao_scripts-1.4.0/src/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,20 +79,25 @@
     # Exclusive lock for the chache-scripts (no two cache-scripts running)
     cs_lock: Path = datawarehouse / '.cs.lock'
 
     try:
         with pl.Lock(cs_lock, 'w', timeout=1) as lock, \
              tempfile.TemporaryDirectory(prefix="datawarehouse_") as tmp_dw_str:
 
+            running_link = datawarehouse / '.running'
+            if running_link.exists():
+                print("Program was killed, removing aux files")
+                running_link.unlink()
+
             # Writing pid and dir name to lock (debugging)
             tmp_dw = Path(tmp_dw_str)
             print(os.getpid(), file=lock)
             print(tmp_dw, file=lock)
             lock.flush()
-            (datawarehouse / '.running').symlink_to(tmp_dw)
+            running_link.symlink_to(tmp_dw)
 
             # Used to tell the loggers to use errors.log or the main logs
             copied_dw = False
 
             try:
                 ignore = shutil.ignore_patterns('.lock*', 'logs/*')
 
@@ -131,15 +136,15 @@
                 with pl.Lock(p_lock, 'w', timeout=10):
                     shutil.copytree(tmp_dw, datawarehouse, dirs_exist_ok=True, ignore=ignore)
                 
                 copied_dw = True
             finally:
                 # Removing pid from lock
                 lock.truncate(0)
-                (datawarehouse / '.running').unlink()
+                running_link.unlink()
                 finish_logging(errors=not copied_dw)
     except pl.LockException:
         with open(cs_lock, 'r') as f:
             pid = int(f.readline())
 
         print(f"The cache_scripts are already being run with pid {pid}", file=stderr)
         exit(1)
```

### Comparing `dao_scripts-1.3.1/src/metadata.py` & `dao_scripts-1.4.0/src/metadata.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.3.1/src/utils/uploadDataWarehouse.py` & `dao_scripts-1.4.0/src/utils/uploadDataWarehouse.py`

 * *Files identical despite different names*

