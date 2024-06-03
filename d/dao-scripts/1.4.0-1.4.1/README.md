# Comparing `tmp/dao_scripts-1.4.0.tar.gz` & `tmp/dao_scripts-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dao_scripts-1.4.0.tar", last modified: Mon Jun  3 09:20:22 2024, max compression
+gzip compressed data, was "dao_scripts-1.4.1.tar", last modified: Mon Jun  3 09:32:32 2024, max compression
```

## Comparing `dao_scripts-1.4.0.tar` & `dao_scripts-1.4.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:20:22.892581 dao_scripts-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/.envrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:20:22.880581 dao_scripts-1.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:20:22.884581 dao_scripts-1.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/.github/workflows/update-datasets.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-06-03 09:20:22.892581 dao_scripts-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:20:22.888581 dao_scripts-1.4.0/dao_scripts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-06-03 09:20:22.000000 dao_scripts-1.4.0/dao_scripts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-06-03 09:20:22.000000 dao_scripts-1.4.0/dao_scripts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 09:20:22.000000 dao_scripts-1.4.0/dao_scripts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-06-03 09:20:22.000000 dao_scripts-1.4.0/dao_scripts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-03 09:20:22.000000 dao_scripts-1.4.0/dao_scripts.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-06-03 09:20:22.000000 dao_scripts-1.4.0/dao_scripts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-03 09:20:22.000000 dao_scripts-1.4.0/dao_scripts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-06-03 09:20:22.892581 dao_scripts-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:20:22.888581 dao_scripts-1.4.0/src/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-03 09:20:22.000000 dao_scripts-1.4.0/src/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:20:22.888581 dao_scripts-1.4.0/src/aragon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/aragon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/aragon/dao_names.json
--rw-r--r--   0 runner    (1001) docker     (127)     8163 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/aragon/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/argparser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:20:22.888581 dao_scripts-1.4.0/src/common/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/common/api_requester.py
--rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/common/blockscout.py
--rw-r--r--   0 runner    (1001) docker     (127)    10763 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/common/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/common/cryptocompare.py
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/common/thegraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:20:22.888581 dao_scripts-1.4.0/src/daohaus/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/daohaus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7549 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/daohaus/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:20:22.888581 dao_scripts-1.4.0/src/daostack/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/daostack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10144 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/daostack/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/endpoints.json
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/logging.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5751 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:20:22.888581 dao_scripts-1.4.0/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/src/utils/uploadDataWarehouse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:20:22.888581 dao_scripts-1.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-06-03 09:20:15.000000 dao_scripts-1.4.0/test/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:32:32.679112 dao_scripts-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/.envrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:32:32.667112 dao_scripts-1.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:32:32.671112 dao_scripts-1.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/.github/workflows/update-datasets.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-06-03 09:32:32.679112 dao_scripts-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:32:32.675112 dao_scripts-1.4.1/dao_scripts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-06-03 09:32:32.000000 dao_scripts-1.4.1/dao_scripts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-06-03 09:32:32.000000 dao_scripts-1.4.1/dao_scripts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 09:32:32.000000 dao_scripts-1.4.1/dao_scripts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-06-03 09:32:32.000000 dao_scripts-1.4.1/dao_scripts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-03 09:32:32.000000 dao_scripts-1.4.1/dao_scripts.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-06-03 09:32:32.000000 dao_scripts-1.4.1/dao_scripts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-03 09:32:32.000000 dao_scripts-1.4.1/dao_scripts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-06-03 09:32:32.679112 dao_scripts-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:32:32.675112 dao_scripts-1.4.1/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-03 09:32:32.000000 dao_scripts-1.4.1/src/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:32:32.675112 dao_scripts-1.4.1/src/aragon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/aragon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/aragon/dao_names.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8163 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/aragon/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/argparser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:32:32.675112 dao_scripts-1.4.1/src/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/common/api_requester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/common/blockscout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10763 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/common/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/common/cryptocompare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/common/thegraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:32:32.675112 dao_scripts-1.4.1/src/daohaus/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/daohaus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7549 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/daohaus/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:32:32.675112 dao_scripts-1.4.1/src/daostack/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/daostack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10144 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/daostack/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/endpoints.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/logging.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5751 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:32:32.675112 dao_scripts-1.4.1/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/utils/uploadDataWarehouse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:32:32.675112 dao_scripts-1.4.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/test/test_placeholder.py
```

### Comparing `dao_scripts-1.4.0/.github/workflows/ci.yml` & `dao_scripts-1.4.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.0/.github/workflows/update-datasets.yml` & `dao_scripts-1.4.1/.github/workflows/update-datasets.yml`

 * *Files 1% similar despite different names*

```diff
@@ -48,13 +48,13 @@
     - name: Patch Zenodo client (provisional)
       run: |
         FILE="$(python -c "from zenodo_client import api; print(api.__file__)")"
         echo "Modyfing file $FILE"
         sed -i 's/_prepare_new_version(new_deposition_data\["metadata"\]\["version"\])/_prepare_new_version(new_deposition_data["metadata"].get("version", ""))/g' "$FILE"
         sed -i 's/json=new_deposition_data/json={"metadata": new_deposition_data\["metadata"\]}/g' "$FILE"
     - name: Upload dataset
-      run: dao-utils-upload-dw ${{matrix.repo}}
+      run: dao-utils-upload-dw --debug ${{matrix.repo}}
       env:
         KAGGLE_USERNAME: ${{ secrets.KAGGLE_USERNAME }}
         KAGGLE_KEY: ${{ secrets.KAGGLE_KEY }}
         ZENODO_DEPOSITION_ID: ${{ secrets.ZENODO_DEPOSITION_ID }}
         ZENODO_API_TOKEN: ${{ secrets.ZENODO_API_TOKEN }}
```

### Comparing `dao_scripts-1.4.0/.gitignore` & `dao_scripts-1.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.0/CHANGELOG.md` & `dao_scripts-1.4.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
+## 1.4.1 - 2024-06-03
+- Added debug logging to `dao-utils-upload-dw`
+
 ## 1.4.0 - 2024-06-03
 - Fixed bug when process was killed
 - Updated endpoint network names
 
 ## 1.3.1 - 2024-05-27
 - Fixed bug with `--delete-force`
```

### Comparing `dao_scripts-1.4.0/LICENSE` & `dao_scripts-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.0/PKG-INFO` & `dao_scripts-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dao-scripts
-Version: 1.4.0
+Version: 1.4.1
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
-Metadata-Version: 2.1 Name: dao-scripts Version: 1.4.0 Summary: "A tool to
+Metadata-Version: 2.1 Name: dao-scripts Version: 1.4.1 Summary: "A tool to
 download data to monitor DAO activity" Home-page: https://github.com/Grasia/
 dao-scripts Author: David DavÃ³ Author-email: ddavo@ucm.es Project-URL: Source,
 https://github.com/Grasia/dao-scripts Project-URL: Bug Tracker, https://
 github.com/Grasia/dao-scripts/issues Project-URL: Changelog, https://
 github.com/Grasia/dao-scripts/blob/main/CHANGELOG.md Classifier: Development
 Status :: 5 - Production/Stable Classifier: Environment :: Console Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
```

### Comparing `dao_scripts-1.4.0/README.md` & `dao_scripts-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.0/dao_scripts.egg-info/PKG-INFO` & `dao_scripts-1.4.1/dao_scripts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dao-scripts
-Version: 1.4.0
+Version: 1.4.1
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
-Metadata-Version: 2.1 Name: dao-scripts Version: 1.4.0 Summary: "A tool to
+Metadata-Version: 2.1 Name: dao-scripts Version: 1.4.1 Summary: "A tool to
 download data to monitor DAO activity" Home-page: https://github.com/Grasia/
 dao-scripts Author: David DavÃ³ Author-email: ddavo@ucm.es Project-URL: Source,
 https://github.com/Grasia/dao-scripts Project-URL: Bug Tracker, https://
 github.com/Grasia/dao-scripts/issues Project-URL: Changelog, https://
 github.com/Grasia/dao-scripts/blob/main/CHANGELOG.md Classifier: Development
 Status :: 5 - Production/Stable Classifier: Environment :: Console Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
```

### Comparing `dao_scripts-1.4.0/dao_scripts.egg-info/SOURCES.txt` & `dao_scripts-1.4.1/dao_scripts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.0/setup.cfg` & `dao_scripts-1.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.0/setup.py` & `dao_scripts-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.0/src/aragon/dao_names.json` & `dao_scripts-1.4.1/src/aragon/dao_names.json`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.0/src/aragon/runner.py` & `dao_scripts-1.4.1/src/aragon/runner.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.0/src/argparser.py` & `dao_scripts-1.4.1/src/argparser.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.0/src/common/api_requester.py` & `dao_scripts-1.4.1/src/common/api_requester.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.0/src/common/blockscout.py` & `dao_scripts-1.4.1/src/common/blockscout.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.0/src/common/common.py` & `dao_scripts-1.4.1/src/common/common.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.0/src/common/cryptocompare.py` & `dao_scripts-1.4.1/src/common/cryptocompare.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.0/src/common/thegraph.py` & `dao_scripts-1.4.1/src/common/thegraph.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.0/src/config.py` & `dao_scripts-1.4.1/src/config.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.0/src/daohaus/runner.py` & `dao_scripts-1.4.1/src/daohaus/runner.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.0/src/daostack/runner.py` & `dao_scripts-1.4.1/src/daostack/runner.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.0/src/endpoints.json` & `dao_scripts-1.4.1/src/endpoints.json`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.0/src/logging.py` & `dao_scripts-1.4.1/src/logging.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.0/src/main.py` & `dao_scripts-1.4.1/src/main.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.0/src/metadata.py` & `dao_scripts-1.4.1/src/metadata.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.0/src/utils/uploadDataWarehouse.py` & `dao_scripts-1.4.1/src/utils/uploadDataWarehouse.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import sys
 import tempfile
 from pathlib import Path
 import shutil
 import json
 import requests
 from time import sleep
+import logging
 
 from tqdm import tqdm
 
 DEFAULT_DATAWAREHOUSE = Path(os.getenv('DAOA_DW_PATH', 'datawarehouse'))
 
 def getDwPaths():
     """ Returns dw paths """
@@ -118,19 +119,35 @@
     parser.add_argument(
         '-z',
         '--zenodo-max-retries',
         type=int,
         default=5,
         help="Zenodo is known to return 504 error, this program will try and upload it again",
     )
+    parser.add_argument(
+        '-D', '--debug',
+        action='store_true',
+        help='Enable debug logs',
+    )
 
     args = parser.parse_args() 
     if args.repos == 'all':
         args.repos = available_repos
 
+    if args.debug:
+        from http.client import HTTPConnection
+        
+        # https://requests.readthedocs.io/en/latest/api/#api-changes
+        HTTPConnection.debuglevel = 1
+        logging.basicConfig()
+        logging.getLogger().setLevel(logging.DEBUG)
+        requests_log = logging.getLogger('urllib3')
+        requests_log.setLevel(logging.DEBUG)
+        requests_log.propagate = True
+
     with tempfile.TemporaryDirectory() as tmpdir:
         tmpdir = Path(tmpdir)
 
         print("Archiving datawarehouse")
         archivedw(DEFAULT_DATAWAREHOUSE, tmpdir)
         if 'zenodo' in args.repos:
             print("Uploading to zenodo")
```

