# Comparing `tmp/bd_sig_filter-1.0.tar.gz` & `tmp/bd_sig_filter-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bd_sig_filter-1.0.tar", last modified: Sun Jun  2 12:39:57 2024, max compression
+gzip compressed data, was "bd_sig_filter-1.1.tar", last modified: Sun Jun  2 12:44:51 2024, max compression
```

## Comparing `bd_sig_filter-1.0.tar` & `bd_sig_filter-1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:39:57.865299 bd_sig_filter-1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-06-02 12:39:47.000000 bd_sig_filter-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-06-02 12:39:57.865299 bd_sig_filter-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-06-02 12:39:47.000000 bd_sig_filter-1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:39:57.861299 bd_sig_filter-1.0/bd_sig_filter/
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-06-02 12:39:47.000000 bd_sig_filter-1.0/bd_sig_filter/BOMClass.py
--rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-06-02 12:39:47.000000 bd_sig_filter-1.0/bd_sig_filter/ComponentClass.py
--rw-r--r--   0 runner    (1001) docker     (127)     9671 2024-06-02 12:39:47.000000 bd_sig_filter-1.0/bd_sig_filter/ComponentListClass.py
--rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-06-02 12:39:47.000000 bd_sig_filter-1.0/bd_sig_filter/SigEntryClass.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 12:39:47.000000 bd_sig_filter-1.0/bd_sig_filter/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2635 2024-06-02 12:39:47.000000 bd_sig_filter-1.0/bd_sig_filter/bd_data.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1416 2024-06-02 12:39:47.000000 bd_sig_filter-1.0/bd_sig_filter/bd_project.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5395 2024-06-02 12:39:47.000000 bd_sig_filter-1.0/bd_sig_filter/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-06-02 12:39:47.000000 bd_sig_filter-1.0/bd_sig_filter/global_values.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-06-02 12:39:47.000000 bd_sig_filter-1.0/bd_sig_filter/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:39:57.865299 bd_sig_filter-1.0/bd_sig_filter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-06-02 12:39:57.000000 bd_sig_filter-1.0/bd_sig_filter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-06-02 12:39:57.000000 bd_sig_filter-1.0/bd_sig_filter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 12:39:57.000000 bd_sig_filter-1.0/bd_sig_filter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-02 12:39:57.000000 bd_sig_filter-1.0/bd_sig_filter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-02 12:39:57.000000 bd_sig_filter-1.0/bd_sig_filter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-02 12:39:57.000000 bd_sig_filter-1.0/bd_sig_filter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-06-02 12:39:47.000000 bd_sig_filter-1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 12:39:57.865299 bd_sig_filter-1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:44:51.173963 bd_sig_filter-1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-06-02 12:44:41.000000 bd_sig_filter-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-06-02 12:44:51.173963 bd_sig_filter-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-06-02 12:44:41.000000 bd_sig_filter-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:44:51.169963 bd_sig_filter-1.1/bd_sig_filter/
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-06-02 12:44:41.000000 bd_sig_filter-1.1/bd_sig_filter/BOMClass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-06-02 12:44:41.000000 bd_sig_filter-1.1/bd_sig_filter/ComponentClass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9671 2024-06-02 12:44:41.000000 bd_sig_filter-1.1/bd_sig_filter/ComponentListClass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-06-02 12:44:41.000000 bd_sig_filter-1.1/bd_sig_filter/SigEntryClass.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 12:44:41.000000 bd_sig_filter-1.1/bd_sig_filter/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2742 2024-06-02 12:44:41.000000 bd_sig_filter-1.1/bd_sig_filter/bd_data.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1416 2024-06-02 12:44:41.000000 bd_sig_filter-1.1/bd_sig_filter/bd_project.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5395 2024-06-02 12:44:41.000000 bd_sig_filter-1.1/bd_sig_filter/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-06-02 12:44:41.000000 bd_sig_filter-1.1/bd_sig_filter/global_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-06-02 12:44:41.000000 bd_sig_filter-1.1/bd_sig_filter/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:44:51.173963 bd_sig_filter-1.1/bd_sig_filter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-06-02 12:44:51.000000 bd_sig_filter-1.1/bd_sig_filter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-06-02 12:44:51.000000 bd_sig_filter-1.1/bd_sig_filter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 12:44:51.000000 bd_sig_filter-1.1/bd_sig_filter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-02 12:44:51.000000 bd_sig_filter-1.1/bd_sig_filter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-02 12:44:51.000000 bd_sig_filter-1.1/bd_sig_filter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-02 12:44:51.000000 bd_sig_filter-1.1/bd_sig_filter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-06-02 12:44:41.000000 bd_sig_filter-1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 12:44:51.173963 bd_sig_filter-1.1/setup.cfg
```

### Comparing `bd_sig_filter-1.0/LICENSE` & `bd_sig_filter-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bd_sig_filter-1.0/PKG-INFO` & `bd_sig_filter-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bd_sig_filter
-Version: 1.0
+Version: 1.1
 Summary: BD_sig_filter - BD Script to ignore components matched from Signature scan likely to be partial or invalid matches.
 Author-email: Matthew Brady <mbrad@synopsys.com>
 Project-URL: Homepage, https://github.com/matthewb66/bd_sig_filter
 Project-URL: Issues, https://github.com/matthewb66/bd_sig_filter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `bd_sig_filter-1.0/README.md` & `bd_sig_filter-1.1/README.md`

 * *Files identical despite different names*

### Comparing `bd_sig_filter-1.0/bd_sig_filter/BOMClass.py` & `bd_sig_filter-1.1/bd_sig_filter/BOMClass.py`

 * *Files identical despite different names*

### Comparing `bd_sig_filter-1.0/bd_sig_filter/ComponentClass.py` & `bd_sig_filter-1.1/bd_sig_filter/ComponentClass.py`

 * *Files identical despite different names*

### Comparing `bd_sig_filter-1.0/bd_sig_filter/ComponentListClass.py` & `bd_sig_filter-1.1/bd_sig_filter/ComponentListClass.py`

 * *Files identical despite different names*

### Comparing `bd_sig_filter-1.0/bd_sig_filter/SigEntryClass.py` & `bd_sig_filter-1.1/bd_sig_filter/SigEntryClass.py`

 * *Files identical despite different names*

### Comparing `bd_sig_filter-1.0/bd_sig_filter/bd_data.py` & `bd_sig_filter-1.1/bd_sig_filter/bd_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-import aiohttp
-import asyncio
-import platform
+# import aiohttp
+# import asyncio
+# import platform
 # import logging
 
 # import bd_data
 from . import global_values
 
 
-async def async_main(comps, token):
-    async with aiohttp.ClientSession(trust_env=True) as session:
-        data_tasks = []
-        file_tasks = []
-
-        count = 0
-        for url, comp in comps.items():
-            count += 1
-
-            file_task = asyncio.ensure_future(async_get_files(session, comp, token))
-            file_tasks.append(file_task)
-
-        await asyncio.gather(*data_tasks)
-        all_files = dict(await asyncio.gather(*file_tasks))
-
-        await asyncio.sleep(0.250)
-        # print(f'- {count} components ')
-        #
-        # print(all_files)
-
-    return all_files
-
-
-async def async_get_files(session, comp, token):
-    filelist = []
-
-    if not global_values.bd_trustcert:
-        ssl = False
-    else:
-        ssl = None
-
-    # retfile = "NOASSERTION"
-    hrefs = comp['_meta']['links']
-
-    link = next((item for item in hrefs if item["rel"] == "matched-files"), None)
-    # link = next((item for item in hrefs if item["rel"] == "origins"), None)
-    if link:
-        thishref = link['href'] + '?limit=1000'
-        headers = {
-            'Authorization': f'Bearer {token}',
-            'accept': "application/vnd.blackducksoftware.bill-of-materials-6+json",
-            # 'accept': "application/vnd.blackducksoftware.component-detail-5+json",
-        }
-
-        # archive_ignore = False
-        async with session.get(thishref, headers=headers, ssl=ssl) as resp:
-            result_data = await resp.json()
-            for item in result_data['items']:
-                filelist.append(item['filePath']['compositePathContext'])
-
-    return comp['componentVersion'], filelist
-
-
-def get_file_data(compdict):
-    if platform.system() == "Windows":
-        asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
-    file_dict = asyncio.run(async_main(compdict, global_values.bd.session.auth.bearer_token))
-
-    return file_dict
+# async def async_main(comps, token):
+#     async with aiohttp.ClientSession(trust_env=True) as session:
+#         data_tasks = []
+#         file_tasks = []
+#
+#         count = 0
+#         for url, comp in comps.items():
+#             count += 1
+#
+#             file_task = asyncio.ensure_future(async_get_files(session, comp, token))
+#             file_tasks.append(file_task)
+#
+#         await asyncio.gather(*data_tasks)
+#         all_files = dict(await asyncio.gather(*file_tasks))
+#
+#         await asyncio.sleep(0.250)
+#         # print(f'- {count} components ')
+#         #
+#         # print(all_files)
+#
+#     return all_files
+
+
+# async def async_get_files(session, comp, token):
+#     filelist = []
+#
+#     if not global_values.bd_trustcert:
+#         ssl = False
+#     else:
+#         ssl = None
+#
+#     # retfile = "NOASSERTION"
+#     hrefs = comp['_meta']['links']
+#
+#     link = next((item for item in hrefs if item["rel"] == "matched-files"), None)
+#     # link = next((item for item in hrefs if item["rel"] == "origins"), None)
+#     if link:
+#         thishref = link['href'] + '?limit=1000'
+#         headers = {
+#             'Authorization': f'Bearer {token}',
+#             'accept': "application/vnd.blackducksoftware.bill-of-materials-6+json",
+#             # 'accept': "application/vnd.blackducksoftware.component-detail-5+json",
+#         }
+#
+#         # archive_ignore = False
+#         async with session.get(thishref, headers=headers, ssl=ssl) as resp:
+#             result_data = await resp.json()
+#             for item in result_data['items']:
+#                 filelist.append(item['filePath']['compositePathContext'])
+#
+#     return comp['componentVersion'], filelist
+#
+#
+# def get_file_data(compdict):
+#     if platform.system() == "Windows":
+#         asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
+#     file_dict = asyncio.run(async_main(compdict, global_values.bd.session.auth.bearer_token))
+#
+#     return file_dict
 
 
 def get_paginated_data(url, accept_hdr):
     headers = {
         'accept': accept_hdr,
     }
     res = global_values.bd.get_json(url, headers=headers)
```

### Comparing `bd_sig_filter-1.0/bd_sig_filter/bd_project.py` & `bd_sig_filter-1.1/bd_sig_filter/bd_project.py`

 * *Files identical despite different names*

### Comparing `bd_sig_filter-1.0/bd_sig_filter/config.py` & `bd_sig_filter-1.1/bd_sig_filter/config.py`

 * *Files identical despite different names*

### Comparing `bd_sig_filter-1.0/bd_sig_filter.egg-info/PKG-INFO` & `bd_sig_filter-1.1/bd_sig_filter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bd_sig_filter
-Version: 1.0
+Version: 1.1
 Summary: BD_sig_filter - BD Script to ignore components matched from Signature scan likely to be partial or invalid matches.
 Author-email: Matthew Brady <mbrad@synopsys.com>
 Project-URL: Homepage, https://github.com/matthewb66/bd_sig_filter
 Project-URL: Issues, https://github.com/matthewb66/bd_sig_filter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `bd_sig_filter-1.0/bd_sig_filter.egg-info/SOURCES.txt` & `bd_sig_filter-1.1/bd_sig_filter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bd_sig_filter-1.0/pyproject.toml` & `bd_sig_filter-1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bd_sig_filter"
-version = "1.0"
+version = "1.1"
 authors = [
   { name="Matthew Brady", email="mbrad@synopsys.com" },
 ]
 description = "BD_sig_filter - BD Script to ignore components matched from Signature scan likely to be partial or invalid matches."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

