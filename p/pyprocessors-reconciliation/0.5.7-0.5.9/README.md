# Comparing `tmp/pyprocessors_reconciliation-0.5.7.tar.gz` & `tmp/pyprocessors_reconciliation-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprocessors_reconciliation-0.5.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyprocessors_reconciliation-0.5.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyprocessors_reconciliation-0.5.7.tar` & `pyprocessors_reconciliation-0.5.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rwxr-xr-x   0        0        0     1774 2024-05-30 17:31:20.484068 pyprocessors_reconciliation-0.5.7/.gitignore
--rwxr-xr-x   0        0        0      123 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.7/AUTHORS.md
--rwxr-xr-x   0        0        0      268 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.7/CHANGELOG.md
--rwxr-xr-x   0        0        0      476 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.7/Dockerfile
--rw-r--r--   0        0        0    13995 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.7/Jenkinsfile
--rwxr-xr-x   0        0        0     1082 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.7/LICENSE
--rwxr-xr-x   0        0        0     1660 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.7/README.md
--rwxr-xr-x   0        0        0      953 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.7/RELEASE.md
--rwxr-xr-x   0        0        0     1559 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.7/bumpversion.py
--rwxr-xr-x   0        0        0       62 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.7/docs/.gitignore
--rwxr-xr-x   0        0        0      268 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.7/docs/CHANGELOG.md
--rwxr-xr-x   0        0        0     1082 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.7/docs/LICENSE
--rwxr-xr-x   0        0        0        0 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.7/docs/_static/.gitkeep
--rwxr-xr-x   0        0        0        0 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.7/docs/_templates/.gitkeep
--rwxr-xr-x   0        0        0     2909 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.7/docs/conf.py
--rwxr-xr-x   0        0        0      148 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.7/docs/index.rst
--rwxr-xr-x   0        0        0       98 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.7/mypy.ini
--rwxr-xr-x   0        0        0     2314 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.7/pyproject.toml
--rwxr-xr-x   0        0        0     1921 2024-05-30 19:34:44.701643 pyprocessors_reconciliation-0.5.7/results.xml
--rwxr-xr-x   0        0        0       60 2024-05-30 19:36:20.120712 pyprocessors_reconciliation-0.5.7/src/pyprocessors_reconciliation/__init__.py
--rwxr-xr-x   0        0        0    12237 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.7/src/pyprocessors_reconciliation/reconciliation.py
--rwxr-xr-x   0        0        0        0 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.7/tests/__init__.py
--rwxr-xr-x   0        0        0     6824 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.7/tests/data/afp_ner_fr-document-test-whitelist2.json
--rw-r--r--   0        0        0    20748 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.7/tests/data/x_cago_ner_en-document-test.json
--rw-r--r--   0        0        0    17283 2024-05-30 19:36:17.332622 pyprocessors_reconciliation-0.5.7/tests/data/x_cago_ner_en-document_conso.json
--rwxr-xr-x   0        0        0     2243 2024-05-30 17:41:23.214952 pyprocessors_reconciliation-0.5.7/tests/test_reconciliation.py
--rwxr-xr-x   0        0        0      893 2024-05-30 17:41:23.214952 pyprocessors_reconciliation-0.5.7/tox.ini
--rw-r--r--   0        0        0     1432 1970-01-01 00:00:00.000000 pyprocessors_reconciliation-0.5.7/setup.py
--rw-r--r--   0        0        0     3522 1970-01-01 00:00:00.000000 pyprocessors_reconciliation-0.5.7/PKG-INFO
+-rwxr-xr-x   0        0        0     1774 2024-05-30 17:31:20.484068 pyprocessors_reconciliation-0.5.9/.gitignore
+-rwxr-xr-x   0        0        0      123 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.9/AUTHORS.md
+-rwxr-xr-x   0        0        0      268 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.9/CHANGELOG.md
+-rwxr-xr-x   0        0        0      476 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.9/Dockerfile
+-rw-r--r--   0        0        0    13995 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.9/Jenkinsfile
+-rwxr-xr-x   0        0        0     1082 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.9/LICENSE
+-rwxr-xr-x   0        0        0     1660 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.9/README.md
+-rwxr-xr-x   0        0        0      953 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.9/RELEASE.md
+-rwxr-xr-x   0        0        0     1559 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.9/bumpversion.py
+-rwxr-xr-x   0        0        0       62 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.9/docs/.gitignore
+-rwxr-xr-x   0        0        0      268 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.9/docs/CHANGELOG.md
+-rwxr-xr-x   0        0        0     1082 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.9/docs/LICENSE
+-rwxr-xr-x   0        0        0        0 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.9/docs/_static/.gitkeep
+-rwxr-xr-x   0        0        0        0 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.9/docs/_templates/.gitkeep
+-rwxr-xr-x   0        0        0     2909 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.9/docs/conf.py
+-rwxr-xr-x   0        0        0      148 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.9/docs/index.rst
+-rwxr-xr-x   0        0        0       98 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.9/mypy.ini
+-rwxr-xr-x   0        0        0     2314 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.9/pyproject.toml
+-rwxr-xr-x   0        0        0     1921 2024-05-30 19:36:30.777054 pyprocessors_reconciliation-0.5.9/results.xml
+-rwxr-xr-x   0        0        0       60 2024-05-30 19:37:58.563877 pyprocessors_reconciliation-0.5.9/src/pyprocessors_reconciliation/__init__.py
+-rwxr-xr-x   0        0        0    12237 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.9/src/pyprocessors_reconciliation/reconciliation.py
+-rwxr-xr-x   0        0        0        0 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.9/tests/__init__.py
+-rwxr-xr-x   0        0        0     6824 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.9/tests/data/afp_ner_fr-document-test-whitelist2.json
+-rw-r--r--   0        0        0    20748 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.9/tests/data/x_cago_ner_en-document-test.json
+-rw-r--r--   0        0        0    17283 2024-05-30 19:37:55.867791 pyprocessors_reconciliation-0.5.9/tests/data/x_cago_ner_en-document_conso.json
+-rwxr-xr-x   0        0        0     2243 2024-05-30 17:41:23.214952 pyprocessors_reconciliation-0.5.9/tests/test_reconciliation.py
+-rwxr-xr-x   0        0        0      893 2024-05-30 17:41:23.214952 pyprocessors_reconciliation-0.5.9/tox.ini
+-rw-r--r--   0        0        0     1432 1970-01-01 00:00:00.000000 pyprocessors_reconciliation-0.5.9/setup.py
+-rw-r--r--   0        0        0     3522 1970-01-01 00:00:00.000000 pyprocessors_reconciliation-0.5.9/PKG-INFO
```

### Comparing `pyprocessors_reconciliation-0.5.7/.gitignore` & `pyprocessors_reconciliation-0.5.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pyprocessors_reconciliation-0.5.7/Jenkinsfile` & `pyprocessors_reconciliation-0.5.9/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `pyprocessors_reconciliation-0.5.7/LICENSE` & `pyprocessors_reconciliation-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprocessors_reconciliation-0.5.7/README.md` & `pyprocessors_reconciliation-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `pyprocessors_reconciliation-0.5.7/RELEASE.md` & `pyprocessors_reconciliation-0.5.9/RELEASE.md`

 * *Files identical despite different names*

### Comparing `pyprocessors_reconciliation-0.5.7/bumpversion.py` & `pyprocessors_reconciliation-0.5.9/bumpversion.py`

 * *Files identical despite different names*

### Comparing `pyprocessors_reconciliation-0.5.7/docs/LICENSE` & `pyprocessors_reconciliation-0.5.9/docs/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprocessors_reconciliation-0.5.7/docs/conf.py` & `pyprocessors_reconciliation-0.5.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyprocessors_reconciliation-0.5.7/pyproject.toml` & `pyprocessors_reconciliation-0.5.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyprocessors_reconciliation-0.5.7/results.xml` & `pyprocessors_reconciliation-0.5.9/results.xml`

 * *Files identical despite different names*

### Comparing `pyprocessors_reconciliation-0.5.7/src/pyprocessors_reconciliation/reconciliation.py` & `pyprocessors_reconciliation-0.5.9/src/pyprocessors_reconciliation/reconciliation.py`

 * *Files identical despite different names*

### Comparing `pyprocessors_reconciliation-0.5.7/tests/data/afp_ner_fr-document-test-whitelist2.json` & `pyprocessors_reconciliation-0.5.9/tests/data/afp_ner_fr-document-test-whitelist2.json`

 * *Files identical despite different names*

### Comparing `pyprocessors_reconciliation-0.5.7/tests/data/x_cago_ner_en-document-test.json` & `pyprocessors_reconciliation-0.5.9/tests/data/x_cago_ner_en-document-test.json`

 * *Files identical despite different names*

### Comparing `pyprocessors_reconciliation-0.5.7/tests/data/x_cago_ner_en-document_conso.json` & `pyprocessors_reconciliation-0.5.9/tests/data/x_cago_ner_en-document_conso.json`

 * *Files identical despite different names*

### Comparing `pyprocessors_reconciliation-0.5.7/tests/test_reconciliation.py` & `pyprocessors_reconciliation-0.5.9/tests/test_reconciliation.py`

 * *Files identical despite different names*

### Comparing `pyprocessors_reconciliation-0.5.7/tox.ini` & `pyprocessors_reconciliation-0.5.9/tox.ini`

 * *Files identical despite different names*

### Comparing `pyprocessors_reconciliation-0.5.7/setup.py` & `pyprocessors_reconciliation-0.5.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
           'dirty-equals']}
 
 entry_points = \
 {'pyprocessors.plugins': ['reconciliation = '
                           'pyprocessors_reconciliation.reconciliation:ReconciliationProcessor']}
 
 setup(name='pyprocessors-reconciliation',
-      version='0.5.7',
+      version='0.5.9',
       description='Sherpa reconciliation processor',
       author='Olivier Terrier',
       author_email='olivier.terrier@kairntech.com',
       url='https://github.com/oterrier/pyprocessors_reconciliation/',
       packages=packages,
       package_data=package_data,
       package_dir=package_dir,
```

### Comparing `pyprocessors_reconciliation-0.5.7/PKG-INFO` & `pyprocessors_reconciliation-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprocessors-reconciliation
-Version: 0.5.7
+Version: 0.5.9
 Summary: Sherpa reconciliation processor
 Home-page: https://github.com/oterrier/pyprocessors_reconciliation/
 Keywords: 
 Author: Olivier Terrier
 Author-email: olivier.terrier@kairntech.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

