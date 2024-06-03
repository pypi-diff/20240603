# Comparing `tmp/dao_scripts-1.4.3.tar.gz` & `tmp/dao_scripts-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dao_scripts-1.4.3.tar", last modified: Mon Jun  3 09:59:31 2024, max compression
+gzip compressed data, was "dao_scripts-1.4.4.tar", last modified: Mon Jun  3 11:17:32 2024, max compression
```

## Comparing `dao_scripts-1.4.3.tar` & `dao_scripts-1.4.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:59:31.866890 dao_scripts-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/.envrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:59:31.854889 dao_scripts-1.4.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:59:31.858890 dao_scripts-1.4.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/.github/workflows/update-datasets.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-06-03 09:59:31.866890 dao_scripts-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:59:31.862890 dao_scripts-1.4.3/dao_scripts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-06-03 09:59:31.000000 dao_scripts-1.4.3/dao_scripts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-06-03 09:59:31.000000 dao_scripts-1.4.3/dao_scripts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 09:59:31.000000 dao_scripts-1.4.3/dao_scripts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-06-03 09:59:31.000000 dao_scripts-1.4.3/dao_scripts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-03 09:59:31.000000 dao_scripts-1.4.3/dao_scripts.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-06-03 09:59:31.000000 dao_scripts-1.4.3/dao_scripts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-03 09:59:31.000000 dao_scripts-1.4.3/dao_scripts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-06-03 09:59:31.866890 dao_scripts-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:59:31.862890 dao_scripts-1.4.3/src/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-03 09:59:31.000000 dao_scripts-1.4.3/src/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:59:31.862890 dao_scripts-1.4.3/src/aragon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/aragon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/aragon/dao_names.json
--rw-r--r--   0 runner    (1001) docker     (127)     8163 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/aragon/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/argparser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:59:31.862890 dao_scripts-1.4.3/src/common/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/common/api_requester.py
--rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/common/blockscout.py
--rw-r--r--   0 runner    (1001) docker     (127)    10874 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/common/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/common/cryptocompare.py
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/common/thegraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:59:31.862890 dao_scripts-1.4.3/src/daohaus/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/daohaus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7549 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/daohaus/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:59:31.862890 dao_scripts-1.4.3/src/daostack/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/daostack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10144 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/daostack/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/endpoints.json
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/logging.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5751 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:59:31.862890 dao_scripts-1.4.3/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/src/utils/uploadDataWarehouse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:59:31.862890 dao_scripts-1.4.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-06-03 09:59:26.000000 dao_scripts-1.4.3/test/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:32.975557 dao_scripts-1.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/.envrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:32.963557 dao_scripts-1.4.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:32.967557 dao_scripts-1.4.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/.github/workflows/update-datasets.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-06-03 11:17:32.975557 dao_scripts-1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:32.975557 dao_scripts-1.4.4/dao_scripts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-06-03 11:17:32.000000 dao_scripts-1.4.4/dao_scripts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-06-03 11:17:32.000000 dao_scripts-1.4.4/dao_scripts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 11:17:32.000000 dao_scripts-1.4.4/dao_scripts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-06-03 11:17:32.000000 dao_scripts-1.4.4/dao_scripts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-03 11:17:32.000000 dao_scripts-1.4.4/dao_scripts.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-06-03 11:17:32.000000 dao_scripts-1.4.4/dao_scripts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-03 11:17:32.000000 dao_scripts-1.4.4/dao_scripts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-06-03 11:17:32.975557 dao_scripts-1.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:32.971557 dao_scripts-1.4.4/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-03 11:17:32.000000 dao_scripts-1.4.4/src/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:32.971557 dao_scripts-1.4.4/src/aragon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/aragon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/aragon/dao_names.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8163 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/aragon/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/argparser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:32.971557 dao_scripts-1.4.4/src/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/common/api_requester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/common/blockscout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10874 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/common/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/common/cryptocompare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/common/thegraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:32.971557 dao_scripts-1.4.4/src/daohaus/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/daohaus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7549 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/daohaus/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:32.971557 dao_scripts-1.4.4/src/daostack/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/daostack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10144 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/daostack/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/endpoints.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/logging.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5989 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:32.975557 dao_scripts-1.4.4/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/src/utils/uploadDataWarehouse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:32.975557 dao_scripts-1.4.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-06-03 11:17:22.000000 dao_scripts-1.4.4/test/test_placeholder.py
```

### Comparing `dao_scripts-1.4.3/.github/workflows/ci.yml` & `dao_scripts-1.4.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.3/.github/workflows/update-datasets.yml` & `dao_scripts-1.4.4/.github/workflows/update-datasets.yml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,17 @@
       with:
         workflow: update-datasets.yml
         name: datawarehouse
         path: ./datawarehouse/
         if_no_artifact_found: warn
     - name: Obtain datawarehouse
       run: dao-scripts --skip-token-balances
+      env:
+        DAOA_THE_GRAPH_API_KEY: ${{ secrets.DAOA_THE_GRAPH_API_KEY }}
+        DAOA_CC_API_KEY: ${{ secrets.DAOA_CC_API_KEY }}
     - name: Upload artifact
       uses: actions/upload-artifact@v4
       with:
         name: datawarehouse
         path: ./datawarehouse/
   upload_dw:
     runs-on: ubuntu-latest
@@ -41,17 +44,14 @@
         name: datawarehouse
         path: ./datawarehouse/
     - uses: actions/setup-python@v5
       with:
         python-version: '3.12'
     - name: Install dao-scripts
       run: pip install 'dao-scripts[upload]>=1.1.14'
-      env:
-        DAOA_THE_GRAPH_API_KEY: ${{ secrets.DAOA_THE_GRAPH_API_KEY }}
-        DAOA_CC_API_KEY: ${{ secrets.DAOA_CC_API_KEY }}
     - name: Patch Zenodo client (provisional)
       run: |
         FILE="$(python -c "from zenodo_client import api; print(api.__file__)")"
         echo "Modyfing file $FILE"
         sed -i 's/_prepare_new_version(new_deposition_data\["metadata"\]\["version"\])/_prepare_new_version(new_deposition_data["metadata"].get("version", ""))/g' "$FILE"
         sed -i 's/json=new_deposition_data/json={"metadata": new_deposition_data\["metadata"\]}/g' "$FILE"
     - name: Upload dataset
```

### Comparing `dao_scripts-1.4.3/.gitignore` & `dao_scripts-1.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.3/CHANGELOG.md` & `dao_scripts-1.4.4/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.3/LICENSE` & `dao_scripts-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.3/PKG-INFO` & `dao_scripts-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dao-scripts
-Version: 1.4.3
+Version: 1.4.4
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
-Metadata-Version: 2.1 Name: dao-scripts Version: 1.4.3 Summary: "A tool to
+Metadata-Version: 2.1 Name: dao-scripts Version: 1.4.4 Summary: "A tool to
 download data to monitor DAO activity" Home-page: https://github.com/Grasia/
 dao-scripts Author: David DavÃ³ Author-email: ddavo@ucm.es Project-URL: Source,
 https://github.com/Grasia/dao-scripts Project-URL: Bug Tracker, https://
 github.com/Grasia/dao-scripts/issues Project-URL: Changelog, https://
 github.com/Grasia/dao-scripts/blob/main/CHANGELOG.md Classifier: Development
 Status :: 5 - Production/Stable Classifier: Environment :: Console Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
```

### Comparing `dao_scripts-1.4.3/README.md` & `dao_scripts-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.3/dao_scripts.egg-info/PKG-INFO` & `dao_scripts-1.4.4/dao_scripts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dao-scripts
-Version: 1.4.3
+Version: 1.4.4
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
-Metadata-Version: 2.1 Name: dao-scripts Version: 1.4.3 Summary: "A tool to
+Metadata-Version: 2.1 Name: dao-scripts Version: 1.4.4 Summary: "A tool to
 download data to monitor DAO activity" Home-page: https://github.com/Grasia/
 dao-scripts Author: David DavÃ³ Author-email: ddavo@ucm.es Project-URL: Source,
 https://github.com/Grasia/dao-scripts Project-URL: Bug Tracker, https://
 github.com/Grasia/dao-scripts/issues Project-URL: Changelog, https://
 github.com/Grasia/dao-scripts/blob/main/CHANGELOG.md Classifier: Development
 Status :: 5 - Production/Stable Classifier: Environment :: Console Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
```

### Comparing `dao_scripts-1.4.3/dao_scripts.egg-info/SOURCES.txt` & `dao_scripts-1.4.4/dao_scripts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.3/setup.cfg` & `dao_scripts-1.4.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.3/setup.py` & `dao_scripts-1.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.3/src/aragon/dao_names.json` & `dao_scripts-1.4.4/src/aragon/dao_names.json`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.3/src/aragon/runner.py` & `dao_scripts-1.4.4/src/aragon/runner.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.3/src/argparser.py` & `dao_scripts-1.4.4/src/argparser.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.3/src/common/api_requester.py` & `dao_scripts-1.4.4/src/common/api_requester.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.3/src/common/blockscout.py` & `dao_scripts-1.4.4/src/common/blockscout.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.3/src/common/common.py` & `dao_scripts-1.4.4/src/common/common.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.3/src/common/cryptocompare.py` & `dao_scripts-1.4.4/src/common/cryptocompare.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.3/src/common/thegraph.py` & `dao_scripts-1.4.4/src/common/thegraph.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.3/src/config.py` & `dao_scripts-1.4.4/src/config.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.3/src/daohaus/runner.py` & `dao_scripts-1.4.4/src/daohaus/runner.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.3/src/daostack/runner.py` & `dao_scripts-1.4.4/src/daostack/runner.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.3/src/endpoints.json` & `dao_scripts-1.4.4/src/endpoints.json`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.3/src/logging.py` & `dao_scripts-1.4.4/src/logging.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.3/src/main.py` & `dao_scripts-1.4.4/src/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
             lock.flush()
             running_link.symlink_to(tmp_dw)
 
             # Used to tell the loggers to use errors.log or the main logs
             copied_dw = False
 
             try:
-                ignore = shutil.ignore_patterns('.lock*', 'logs/*')
+                ignore = shutil.ignore_patterns('*.lock', 'logs', '.running')
 
                 # We want to copy the dw, so we open it as readers
                 p_lock.touch(exist_ok=True)
                 with pl.Lock(p_lock, 'r', timeout=1, flags=pl.LOCK_SH | pl.LOCK_NB):
                     shutil.copytree(datawarehouse, tmp_dw, dirs_exist_ok=True, ignore=ignore)
 
                 if args.delete_force or not _is_good_version(tmp_dw):
@@ -130,15 +130,19 @@
                     block_datetime=args.block_datetime,
                     force=args.force,
                 )
 
                 # Copying back the dw
                 logger.info(f"<<< Copying back the datawarehouse from {tmp_dw} to {datawarehouse}")
                 with pl.Lock(p_lock, 'w', timeout=10):
-                    shutil.copytree(tmp_dw, datawarehouse, dirs_exist_ok=True, ignore=ignore)
+                    def verbose_copy(src, dst):
+                        logger.debug(f'Copying {src} to {Path(dst).absolute()}')
+                        return shutil.copy2(src, dst)
+                
+                    shutil.copytree(tmp_dw, datawarehouse, dirs_exist_ok=True, ignore=ignore, copy_function=verbose_copy)
                 
                 copied_dw = True
             finally:
                 # Removing pid from lock
                 lock.truncate(0)
                 running_link.unlink()
                 finish_logging(errors=not copied_dw)
```

### Comparing `dao_scripts-1.4.3/src/metadata.py` & `dao_scripts-1.4.4/src/metadata.py`

 * *Files identical despite different names*

### Comparing `dao_scripts-1.4.3/src/utils/uploadDataWarehouse.py` & `dao_scripts-1.4.4/src/utils/uploadDataWarehouse.py`

 * *Files identical despite different names*

