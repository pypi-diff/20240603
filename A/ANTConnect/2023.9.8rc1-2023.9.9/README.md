# Comparing `tmp/ANTConnect-2023.9.8rc1.tar.gz` & `tmp/ANTConnect-2023.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ANTConnect-2023.9.8rc1.tar", last modified: Tue Oct 17 08:53:57 2023, max compression
+gzip compressed data, was "dist\ANTConnect-2023.9.9.tar", last modified: Fri Nov 17 11:16:10 2023, max compression
```

## Comparing `ANTConnect-2023.9.8rc1.tar` & `ANTConnect-2023.9.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-10-17 08:53:57.048927 ANTConnect-2023.9.8rc1/
-drwxrwxrwx   0        0        0        0 2023-10-17 08:53:57.024722 ANTConnect-2023.9.8rc1/ANTConnect.egg-info/
--rw-rw-rw-   0        0        0     1020 2023-10-17 08:53:56.000000 ANTConnect-2023.9.8rc1/ANTConnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-10-17 08:53:56.000000 ANTConnect-2023.9.8rc1/ANTConnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-17 08:53:56.000000 ANTConnect-2023.9.8rc1/ANTConnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-10-17 08:53:56.000000 ANTConnect-2023.9.8rc1/ANTConnect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-10-17 08:53:56.000000 ANTConnect-2023.9.8rc1/ANTConnect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1092 2022-12-21 12:12:30.000000 ANTConnect-2023.9.8rc1/LICENSE
--rw-rw-rw-   0        0        0     1020 2023-10-17 08:53:57.049438 ANTConnect-2023.9.8rc1/PKG-INFO
--rw-rw-rw-   0        0        0      586 2022-12-21 12:12:30.000000 ANTConnect-2023.9.8rc1/README.md
-drwxrwxrwx   0        0        0        0 2023-10-17 08:53:57.036518 ANTConnect-2023.9.8rc1/antconnect/
--rw-rw-rw-   0        0        0      149 2023-10-17 08:53:55.000000 ANTConnect-2023.9.8rc1/antconnect/__init__.py
--rw-rw-rw-   0        0        0    53568 2023-10-16 15:20:30.000000 ANTConnect-2023.9.8rc1/antconnect/api.py
--rw-rw-rw-   0        0        0      489 2023-10-17 08:53:57.050969 ANTConnect-2023.9.8rc1/setup.cfg
--rw-rw-rw-   0        0        0      742 2023-10-17 08:53:55.000000 ANTConnect-2023.9.8rc1/setup.py
-drwxrwxrwx   0        0        0        0 2023-10-17 08:53:57.047908 ANTConnect-2023.9.8rc1/tests/
--rw-rw-rw-   0        0        0        0 2022-12-21 12:12:30.000000 ANTConnect-2023.9.8rc1/tests/__init__.py
--rw-rw-rw-   0        0        0      102 2022-12-21 12:12:30.000000 ANTConnect-2023.9.8rc1/tests/test_ant.py
+drwxrwxrwx   0        0        0        0 2023-11-17 11:16:10.213465 ANTConnect-2023.9.9/
+drwxrwxrwx   0        0        0        0 2023-11-17 11:16:10.198462 ANTConnect-2023.9.9/ANTConnect.egg-info/
+-rw-rw-rw-   0        0        0     1017 2023-11-17 11:16:10.000000 ANTConnect-2023.9.9/ANTConnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-11-17 11:16:10.000000 ANTConnect-2023.9.9/ANTConnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-11-17 11:16:10.000000 ANTConnect-2023.9.9/ANTConnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-11-17 11:16:10.000000 ANTConnect-2023.9.9/ANTConnect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-11-17 11:16:10.000000 ANTConnect-2023.9.9/ANTConnect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1092 2022-12-21 12:12:30.000000 ANTConnect-2023.9.9/LICENSE
+-rw-rw-rw-   0        0        0     1017 2023-11-17 11:16:10.214465 ANTConnect-2023.9.9/PKG-INFO
+-rw-rw-rw-   0        0        0      586 2022-12-21 12:12:30.000000 ANTConnect-2023.9.9/README.md
+drwxrwxrwx   0        0        0        0 2023-11-17 11:16:10.201464 ANTConnect-2023.9.9/antconnect/
+-rw-rw-rw-   0        0        0      146 2023-11-17 11:15:57.000000 ANTConnect-2023.9.9/antconnect/__init__.py
+-rw-rw-rw-   0        0        0    53612 2023-11-17 11:15:19.000000 ANTConnect-2023.9.9/antconnect/api.py
+-rw-rw-rw-   0        0        0      486 2023-11-17 11:16:10.216465 ANTConnect-2023.9.9/setup.cfg
+-rw-rw-rw-   0        0        0      739 2023-11-17 11:15:57.000000 ANTConnect-2023.9.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-11-17 11:16:10.212464 ANTConnect-2023.9.9/tests/
+-rw-rw-rw-   0        0        0        0 2022-12-21 12:12:30.000000 ANTConnect-2023.9.9/tests/__init__.py
+-rw-rw-rw-   0        0        0      102 2022-12-21 12:12:30.000000 ANTConnect-2023.9.9/tests/test_ant.py
```

### Comparing `ANTConnect-2023.9.8rc1/ANTConnect.egg-info/PKG-INFO` & `ANTConnect-2023.9.9/ANTConnect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ANTConnect
-Version: 2023.9.8rc1
+Version: 2023.9.9
 Summary: Python SDK for ANT Common Data Engineering
 Home-page: https://antcde.io
 Author: ANT CDE
 Author-email: info@antcde.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ANTConnect-2023.9.8rc1/LICENSE` & `ANTConnect-2023.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ANTConnect-2023.9.8rc1/PKG-INFO` & `ANTConnect-2023.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ANTConnect
-Version: 2023.9.8rc1
+Version: 2023.9.9
 Summary: Python SDK for ANT Common Data Engineering
 Home-page: https://antcde.io
 Author: ANT CDE
 Author-email: info@antcde.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ANTConnect-2023.9.8rc1/README.md` & `ANTConnect-2023.9.9/README.md`

 * *Files identical despite different names*

### Comparing `ANTConnect-2023.9.8rc1/antconnect/api.py` & `ANTConnect-2023.9.9/antconnect/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -301,22 +301,23 @@
         return self._make_api_request(path, 'POST', queryBody)
 
     def tables_query_stream(self, project_id: str, queryBody):
         """ executes query over single table and returns all data"""
         query_path = 'project/{}/tables/query/export'.format(project_id)
 
         query_response = self._make_api_request(query_path, 'POST', queryBody)
-
         unprocessed = True
         while unprocessed:
             batch_path = 'batches/{}/status'.format(query_response['batchId'])
             batch_response = self._make_api_request(batch_path, 'GET')
             unprocessed = batch_response['status'] != 'finished'
-            if batch_response['progress_now'] != 0 and batch_response['progress_max'] != 0:
-                print('Proccesing... {}%'.format((batch_response['progress_now'] / batch_response['progress_max'] * 100 )));
+            # if batch_response['progress_now'] != 0 and batch_response['progress_max'] != 0:
+            #     print(
+            #         'Proccesing... {}%'.format((batch_response['progress_now'] / batch_response['progress_max'] * 100))
+            #     )
             time.sleep(3)
 
         print('Process finished attempt to download...')
         downloads_path = 'downloads'
 
         data = {}
```

### Comparing `ANTConnect-2023.9.8rc1/setup.py` & `ANTConnect-2023.9.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ANTConnect", # Replace with your own username
-    version="2023.9.8rc1",
+    version="2023.9.9",
     author="ANT CDE",
     author_email="info@antcde.io",
     description="Python SDK for ANT Common Data Engineering",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://antcde.io",
     packages=setuptools.find_packages(),
```

