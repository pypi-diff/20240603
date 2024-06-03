# Comparing `tmp/dao_scripts-1.4.1.tar.gz` & `tmp/dao_scripts-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dao_scripts-1.4.1.tar", last modified: Mon Jun  3 09:32:32 2024, max compression
+gzip compressed data, was "dao_scripts-1.4.2.tar", last modified: Mon Jun  3 09:45:45 2024, max compression
```

## Comparing `dao_scripts-1.4.1.tar` & `dao_scripts-1.4.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:32:32.679112 dao_scripts-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/.envrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:32:32.667112 dao_scripts-1.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:32:32.671112 dao_scripts-1.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/.github/workflows/update-datasets.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-06-03 09:32:32.679112 dao_scripts-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:32:32.675112 dao_scripts-1.4.1/dao_scripts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-06-03 09:32:32.000000 dao_scripts-1.4.1/dao_scripts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-06-03 09:32:32.000000 dao_scripts-1.4.1/dao_scripts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 09:32:32.000000 dao_scripts-1.4.1/dao_scripts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-06-03 09:32:32.000000 dao_scripts-1.4.1/dao_scripts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-03 09:32:32.000000 dao_scripts-1.4.1/dao_scripts.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-06-03 09:32:32.000000 dao_scripts-1.4.1/dao_scripts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-03 09:32:32.000000 dao_scripts-1.4.1/dao_scripts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-06-03 09:32:32.679112 dao_scripts-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:32:32.675112 dao_scripts-1.4.1/src/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-03 09:32:32.000000 dao_scripts-1.4.1/src/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:32:32.675112 dao_scripts-1.4.1/src/aragon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/aragon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/aragon/dao_names.json
--rw-r--r--   0 runner    (1001) docker     (127)     8163 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/aragon/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/argparser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:32:32.675112 dao_scripts-1.4.1/src/common/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/common/api_requester.py
--rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/common/blockscout.py
--rw-r--r--   0 runner    (1001) docker     (127)    10763 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/common/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/common/cryptocompare.py
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/common/thegraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:32:32.675112 dao_scripts-1.4.1/src/daohaus/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/daohaus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7549 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/daohaus/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:32:32.675112 dao_scripts-1.4.1/src/daostack/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/daostack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10144 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/daostack/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/endpoints.json
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/logging.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5751 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:32:32.675112 dao_scripts-1.4.1/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/src/utils/uploadDataWarehouse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:32:32.675112 dao_scripts-1.4.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-06-03 09:32:21.000000 dao_scripts-1.4.1/test/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:45:45.785073 dao_scripts-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/.envrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:45:45.777073 dao_scripts-1.4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:45:45.777073 dao_scripts-1.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/.github/workflows/update-datasets.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-06-03 09:45:45.785073 dao_scripts-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:45:45.785073 dao_scripts-1.4.2/dao_scripts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-06-03 09:45:45.000000 dao_scripts-1.4.2/dao_scripts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-06-03 09:45:45.000000 dao_scripts-1.4.2/dao_scripts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 09:45:45.000000 dao_scripts-1.4.2/dao_scripts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-06-03 09:45:45.000000 dao_scripts-1.4.2/dao_scripts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-03 09:45:45.000000 dao_scripts-1.4.2/dao_scripts.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-06-03 09:45:45.000000 dao_scripts-1.4.2/dao_scripts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-03 09:45:45.000000 dao_scripts-1.4.2/dao_scripts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-06-03 09:45:45.785073 dao_scripts-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:45:45.781073 dao_scripts-1.4.2/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-03 09:45:45.000000 dao_scripts-1.4.2/src/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:45:45.781073 dao_scripts-1.4.2/src/aragon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/aragon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/aragon/dao_names.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8163 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/aragon/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/argparser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:45:45.781073 dao_scripts-1.4.2/src/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/common/api_requester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/common/blockscout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10763 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/common/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/common/cryptocompare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/common/thegraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:45:45.781073 dao_scripts-1.4.2/src/daohaus/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/daohaus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7549 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/daohaus/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:45:45.781073 dao_scripts-1.4.2/src/daostack/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/daostack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10144 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/daostack/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/endpoints.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/logging.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5751 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:45:45.781073 dao_scripts-1.4.2/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/src/utils/uploadDataWarehouse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:45:45.785073 dao_scripts-1.4.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-06-03 09:45:39.000000 dao_scripts-1.4.2/test/test_placeholder.py
```

### Comparing `dao_scripts-1.4.1/.github/workflows/ci.yml` & `dao_scripts-1.4.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.1/.github/workflows/update-datasets.yml` & `dao_scripts-1.4.2/.github/workflows/update-datasets.yml`

 * *Files 6% similar despite different names*

```diff
@@ -41,20 +41,24 @@
         name: datawarehouse
         path: ./datawarehouse/
     - uses: actions/setup-python@v5
       with:
         python-version: '3.12'
     - name: Install dao-scripts
       run: pip install 'dao-scripts[upload]>=1.1.14'
+      env:
+        DAOA_THE_GRAPH_API_KEY: ${{ secrets.DAOA_THE_GRAPH_API_KEY }}
+        DAOA_CC_API_KEY: ${{ secrets.DAOA_CC_API_KEY }}
     - name: Patch Zenodo client (provisional)
       run: |
         FILE="$(python -c "from zenodo_client import api; print(api.__file__)")"
         echo "Modyfing file $FILE"
         sed -i 's/_prepare_new_version(new_deposition_data\["metadata"\]\["version"\])/_prepare_new_version(new_deposition_data["metadata"].get("version", ""))/g' "$FILE"
         sed -i 's/json=new_deposition_data/json={"metadata": new_deposition_data\["metadata"\]}/g' "$FILE"
     - name: Upload dataset
-      run: dao-utils-upload-dw --debug ${{matrix.repo}}
+      run: dao-utils-upload-dw ${{matrix.repo}}
       env:
+        DAOA_DEBUG: ${{ runner.debug }}
         KAGGLE_USERNAME: ${{ secrets.KAGGLE_USERNAME }}
         KAGGLE_KEY: ${{ secrets.KAGGLE_KEY }}
         ZENODO_DEPOSITION_ID: ${{ secrets.ZENODO_DEPOSITION_ID }}
         ZENODO_API_TOKEN: ${{ secrets.ZENODO_API_TOKEN }}
```

### Comparing `dao_scripts-1.4.1/.gitignore` & `dao_scripts-1.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.1/CHANGELOG.md` & `dao_scripts-1.4.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.1/LICENSE` & `dao_scripts-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.1/PKG-INFO` & `dao_scripts-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dao-scripts
-Version: 1.4.1
+Version: 1.4.2
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
-Metadata-Version: 2.1 Name: dao-scripts Version: 1.4.1 Summary: "A tool to
+Metadata-Version: 2.1 Name: dao-scripts Version: 1.4.2 Summary: "A tool to
 download data to monitor DAO activity" Home-page: https://github.com/Grasia/
 dao-scripts Author: David DavÃ³ Author-email: ddavo@ucm.es Project-URL: Source,
 https://github.com/Grasia/dao-scripts Project-URL: Bug Tracker, https://
 github.com/Grasia/dao-scripts/issues Project-URL: Changelog, https://
 github.com/Grasia/dao-scripts/blob/main/CHANGELOG.md Classifier: Development
 Status :: 5 - Production/Stable Classifier: Environment :: Console Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
```

### Comparing `dao_scripts-1.4.1/README.md` & `dao_scripts-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.1/dao_scripts.egg-info/PKG-INFO` & `dao_scripts-1.4.2/dao_scripts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dao-scripts
-Version: 1.4.1
+Version: 1.4.2
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
-Metadata-Version: 2.1 Name: dao-scripts Version: 1.4.1 Summary: "A tool to
+Metadata-Version: 2.1 Name: dao-scripts Version: 1.4.2 Summary: "A tool to
 download data to monitor DAO activity" Home-page: https://github.com/Grasia/
 dao-scripts Author: David DavÃ³ Author-email: ddavo@ucm.es Project-URL: Source,
 https://github.com/Grasia/dao-scripts Project-URL: Bug Tracker, https://
 github.com/Grasia/dao-scripts/issues Project-URL: Changelog, https://
 github.com/Grasia/dao-scripts/blob/main/CHANGELOG.md Classifier: Development
 Status :: 5 - Production/Stable Classifier: Environment :: Console Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
```

### Comparing `dao_scripts-1.4.1/dao_scripts.egg-info/SOURCES.txt` & `dao_scripts-1.4.2/dao_scripts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.1/setup.cfg` & `dao_scripts-1.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.1/setup.py` & `dao_scripts-1.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.1/src/aragon/dao_names.json` & `dao_scripts-1.4.2/src/aragon/dao_names.json`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.1/src/aragon/runner.py` & `dao_scripts-1.4.2/src/aragon/runner.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.1/src/argparser.py` & `dao_scripts-1.4.2/src/argparser.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.1/src/common/api_requester.py` & `dao_scripts-1.4.2/src/common/api_requester.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.1/src/common/blockscout.py` & `dao_scripts-1.4.2/src/common/blockscout.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.1/src/common/common.py` & `dao_scripts-1.4.2/src/common/common.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.1/src/common/cryptocompare.py` & `dao_scripts-1.4.2/src/common/cryptocompare.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.1/src/common/thegraph.py` & `dao_scripts-1.4.2/src/common/thegraph.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.1/src/config.py` & `dao_scripts-1.4.2/src/config.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.1/src/daohaus/runner.py` & `dao_scripts-1.4.2/src/daohaus/runner.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.1/src/daostack/runner.py` & `dao_scripts-1.4.2/src/daostack/runner.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.1/src/endpoints.json` & `dao_scripts-1.4.2/src/endpoints.json`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.1/src/logging.py` & `dao_scripts-1.4.2/src/logging.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.1/src/main.py` & `dao_scripts-1.4.2/src/main.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.1/src/metadata.py` & `dao_scripts-1.4.2/src/metadata.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.1/src/utils/uploadDataWarehouse.py` & `dao_scripts-1.4.2/src/utils/uploadDataWarehouse.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,14 +123,15 @@
         default=5,
         help="Zenodo is known to return 504 error, this program will try and upload it again",
     )
     parser.add_argument(
         '-D', '--debug',
         action='store_true',
         help='Enable debug logs',
+        default=os.environ.get('DAOA_DEBUG', False),
     )
 
     args = parser.parse_args() 
     if args.repos == 'all':
         args.repos = available_repos
 
     if args.debug:
```

