# Comparing `tmp/thoughtspot_rest_api_v1-1.6.1.tar.gz` & `tmp/thoughtspot_rest_api_v1-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thoughtspot_rest_api_v1-1.6.1.tar", last modified: Fri May 31 12:49:17 2024, max compression
+gzip compressed data, was "thoughtspot_rest_api_v1-1.7.0.tar", last modified: Mon Jun  3 14:59:09 2024, max compression
```

## Comparing `thoughtspot_rest_api_v1-1.6.1.tar` & `thoughtspot_rest_api_v1-1.7.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2024-05-31 12:49:17.353702 thoughtspot_rest_api_v1-1.6.1/
--rw-r--r--   0 bryant.howell (535524999) 1339924365    14780 2022-04-06 21:26:49.000000 thoughtspot_rest_api_v1-1.6.1/LICENSE
--rw-r--r--   0 bryant.howell (535524999) 1339924365    29179 2024-05-31 12:49:17.353427 thoughtspot_rest_api_v1-1.6.1/PKG-INFO
--rw-r--r--   0 bryant.howell (535524999) 1339924365    28378 2023-09-19 19:22:42.000000 thoughtspot_rest_api_v1-1.6.1/README.md
--rw-r--r--   0 bryant.howell (535524999) 1339924365       85 2022-04-04 15:39:10.000000 thoughtspot_rest_api_v1-1.6.1/pyproject.toml
--rw-r--r--   0 bryant.howell (535524999) 1339924365      903 2024-05-31 12:49:17.354259 thoughtspot_rest_api_v1-1.6.1/setup.cfg
--rw-r--r--   0 bryant.howell (535524999) 1339924365      236 2022-04-04 15:39:10.000000 thoughtspot_rest_api_v1-1.6.1/setup.py
-drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2024-05-31 12:49:17.333741 thoughtspot_rest_api_v1-1.6.1/src/
-drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2024-05-31 12:49:17.346281 thoughtspot_rest_api_v1-1.6.1/src/thoughtspot_rest_api_v1/
--rw-r--r--   0 bryant.howell (535524999) 1339924365      318 2022-09-09 16:25:24.000000 thoughtspot_rest_api_v1-1.6.1/src/thoughtspot_rest_api_v1/__init__.py
--rw-r--r--   0 bryant.howell (535524999) 1339924365       22 2024-05-31 12:48:22.000000 thoughtspot_rest_api_v1-1.6.1/src/thoughtspot_rest_api_v1/_version.py
--rw-r--r--   0 bryant.howell (535524999) 1339924365     2328 2022-09-09 16:25:24.000000 thoughtspot_rest_api_v1-1.6.1/src/thoughtspot_rest_api_v1/details_objects.py
--rw-r--r--   0 bryant.howell (535524999) 1339924365    76379 2024-05-31 12:15:19.000000 thoughtspot_rest_api_v1-1.6.1/src/thoughtspot_rest_api_v1/tsrestapiv1.py
--rw-r--r--   0 bryant.howell (535524999) 1339924365    28187 2024-05-31 12:48:22.000000 thoughtspot_rest_api_v1-1.6.1/src/thoughtspot_rest_api_v1/tsrestapiv2.py
-drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2024-05-31 12:49:17.352909 thoughtspot_rest_api_v1-1.6.1/src/thoughtspot_rest_api_v1.egg-info/
--rw-r--r--   0 bryant.howell (535524999) 1339924365    29179 2024-05-31 12:49:17.000000 thoughtspot_rest_api_v1-1.6.1/src/thoughtspot_rest_api_v1.egg-info/PKG-INFO
--rw-r--r--   0 bryant.howell (535524999) 1339924365      518 2024-05-31 12:49:17.000000 thoughtspot_rest_api_v1-1.6.1/src/thoughtspot_rest_api_v1.egg-info/SOURCES.txt
--rw-r--r--   0 bryant.howell (535524999) 1339924365        1 2024-05-31 12:49:17.000000 thoughtspot_rest_api_v1-1.6.1/src/thoughtspot_rest_api_v1.egg-info/dependency_links.txt
--rw-r--r--   0 bryant.howell (535524999) 1339924365       40 2024-05-31 12:49:17.000000 thoughtspot_rest_api_v1-1.6.1/src/thoughtspot_rest_api_v1.egg-info/requires.txt
--rw-r--r--   0 bryant.howell (535524999) 1339924365       24 2024-05-31 12:49:17.000000 thoughtspot_rest_api_v1-1.6.1/src/thoughtspot_rest_api_v1.egg-info/top_level.txt
+drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2024-06-03 14:59:09.052463 thoughtspot_rest_api_v1-1.7.0/
+-rw-r--r--   0 bryant.howell (535524999) 1339924365    14780 2022-04-06 21:26:49.000000 thoughtspot_rest_api_v1-1.7.0/LICENSE
+-rw-r--r--   0 bryant.howell (535524999) 1339924365    29179 2024-06-03 14:59:09.052243 thoughtspot_rest_api_v1-1.7.0/PKG-INFO
+-rw-r--r--   0 bryant.howell (535524999) 1339924365    28378 2023-09-19 19:22:42.000000 thoughtspot_rest_api_v1-1.7.0/README.md
+-rw-r--r--   0 bryant.howell (535524999) 1339924365       85 2022-04-04 15:39:10.000000 thoughtspot_rest_api_v1-1.7.0/pyproject.toml
+-rw-r--r--   0 bryant.howell (535524999) 1339924365      903 2024-06-03 14:59:09.053229 thoughtspot_rest_api_v1-1.7.0/setup.cfg
+-rw-r--r--   0 bryant.howell (535524999) 1339924365      236 2022-04-04 15:39:10.000000 thoughtspot_rest_api_v1-1.7.0/setup.py
+drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2024-06-03 14:59:09.029014 thoughtspot_rest_api_v1-1.7.0/src/
+drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2024-06-03 14:59:09.039362 thoughtspot_rest_api_v1-1.7.0/src/thoughtspot_rest_api_v1/
+-rw-r--r--   0 bryant.howell (535524999) 1339924365      318 2022-09-09 16:25:24.000000 thoughtspot_rest_api_v1-1.7.0/src/thoughtspot_rest_api_v1/__init__.py
+-rw-r--r--   0 bryant.howell (535524999) 1339924365       22 2024-06-03 14:46:56.000000 thoughtspot_rest_api_v1-1.7.0/src/thoughtspot_rest_api_v1/_version.py
+-rw-r--r--   0 bryant.howell (535524999) 1339924365     2328 2022-09-09 16:25:24.000000 thoughtspot_rest_api_v1-1.7.0/src/thoughtspot_rest_api_v1/details_objects.py
+-rw-r--r--   0 bryant.howell (535524999) 1339924365    76782 2024-06-03 14:55:47.000000 thoughtspot_rest_api_v1-1.7.0/src/thoughtspot_rest_api_v1/tsrestapiv1.py
+-rw-r--r--   0 bryant.howell (535524999) 1339924365    28187 2024-05-31 12:48:22.000000 thoughtspot_rest_api_v1-1.7.0/src/thoughtspot_rest_api_v1/tsrestapiv2.py
+drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2024-06-03 14:59:09.051266 thoughtspot_rest_api_v1-1.7.0/src/thoughtspot_rest_api_v1.egg-info/
+-rw-r--r--   0 bryant.howell (535524999) 1339924365    29179 2024-06-03 14:59:09.000000 thoughtspot_rest_api_v1-1.7.0/src/thoughtspot_rest_api_v1.egg-info/PKG-INFO
+-rw-r--r--   0 bryant.howell (535524999) 1339924365      518 2024-06-03 14:59:09.000000 thoughtspot_rest_api_v1-1.7.0/src/thoughtspot_rest_api_v1.egg-info/SOURCES.txt
+-rw-r--r--   0 bryant.howell (535524999) 1339924365        1 2024-06-03 14:59:09.000000 thoughtspot_rest_api_v1-1.7.0/src/thoughtspot_rest_api_v1.egg-info/dependency_links.txt
+-rw-r--r--   0 bryant.howell (535524999) 1339924365       40 2024-06-03 14:59:09.000000 thoughtspot_rest_api_v1-1.7.0/src/thoughtspot_rest_api_v1.egg-info/requires.txt
+-rw-r--r--   0 bryant.howell (535524999) 1339924365       24 2024-06-03 14:59:09.000000 thoughtspot_rest_api_v1-1.7.0/src/thoughtspot_rest_api_v1.egg-info/top_level.txt
```

### Comparing `thoughtspot_rest_api_v1-1.6.1/LICENSE` & `thoughtspot_rest_api_v1-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thoughtspot_rest_api_v1-1.6.1/PKG-INFO` & `thoughtspot_rest_api_v1-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thoughtspot_rest_api_v1
-Version: 1.6.1
+Version: 1.7.0
 Summary: Library implementing the ThoughtSpot V1 REST API
 Home-page: https://github.com/thoughtspot/thoughtspot_rest_api_v1_python
 Author: Bryant Howell
 Author-email: bryant.howell@thoughtspot.com
 License: MIT
 Project-URL: Documentation, https://github.com/thoughtspot/thoughtspot_rest_api_v1_python#readme
 Project-URL: Bug Tracker, https://github.com/thoughtspot/thoughtspot_rest_api_v1_python/issues
```

### Comparing `thoughtspot_rest_api_v1-1.6.1/README.md` & `thoughtspot_rest_api_v1-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `thoughtspot_rest_api_v1-1.6.1/setup.cfg` & `thoughtspot_rest_api_v1-1.7.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = thoughtspot_rest_api_v1
-version = 1.6.1
+version = 1.7.0
 description = Library implementing the ThoughtSpot V1 REST API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/thoughtspot/thoughtspot_rest_api_v1_python
 author = Bryant Howell
 author_email = bryant.howell@thoughtspot.com
 license = MIT
```

### Comparing `thoughtspot_rest_api_v1-1.6.1/src/thoughtspot_rest_api_v1/details_objects.py` & `thoughtspot_rest_api_v1-1.7.0/src/thoughtspot_rest_api_v1/details_objects.py`

 * *Files identical despite different names*

### Comparing `thoughtspot_rest_api_v1-1.6.1/src/thoughtspot_rest_api_v1/tsrestapiv1.py` & `thoughtspot_rest_api_v1-1.7.0/src/thoughtspot_rest_api_v1/tsrestapiv1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1069,14 +1069,16 @@
 
         for obj in objs:
             name_guid_map[obj['info']['name']] = obj['info']['id']
 
         return response_str, name_guid_map
 
     # TML import is distinguished by having an {'Accept': 'text/plain'} header on the POST
+    # 'JSON' default actually takes a Python object representing JSON output
+    # Use 'YAML' or 'JSON_STR' as formattype if you have already stringified the input (read from disk etc.)
     def metadata_tml_import(
         self,
         tml: Union[Dict, List[Dict]],
         create_new_on_server: bool = False,
         validate_only: bool = False,
         formattype: str = 'JSON',
         enable_block_tml_metadata_sync: Optional[bool] = None
@@ -1086,30 +1088,36 @@
         formattype = formattype.upper()
 
         # Adjust for single Dict
         if not isinstance(tml, list):
             tml_list = [tml]
         else:
             tml_list = tml
+        encoded_tmls = []
 
+        # Assume JSON is Python object
         if formattype == 'JSON':
-            json_encoded_tml = json.dumps(tml_list)
-        elif formattype == 'YAML':
-            json_encoded_tml = json.dumps(tml_list)
+            for t in tml_list:
+                encoded_tmls.append(json.dumps(t))
+        # YAML or JSON_STR are already string when sent in
+        elif formattype in ['YAML', 'JSON_STR']:
+            for t in tml_list:
+                encoded_tmls.append(t)
         # Assume it's just a Python object which will dump to JSON matching the TML format
         else:
-            json_encoded_tml = json.dumps(tml_list)
+            for t in tml_list:
+                encoded_tmls.append(json.dumps(t))
 
         import_policy = 'ALL_OR_NONE'
 
         if validate_only is True:
             import_policy = 'VALIDATE_ONLY'
 
         post_data = {
-            'import_objects': json_encoded_tml,
+            'import_objects': str(encoded_tmls),
             'import_policy': import_policy,
             'force_create': str(create_new_on_server).lower()
         }
         if enable_block_tml_metadata_sync is not None:
             post_data['enable_block_tml_metadata_sync'] = str(enable_block_tml_metadata_sync).lower()
 
         url = self.base_url + endpoint
```

### Comparing `thoughtspot_rest_api_v1-1.6.1/src/thoughtspot_rest_api_v1/tsrestapiv2.py` & `thoughtspot_rest_api_v1-1.7.0/src/thoughtspot_rest_api_v1/tsrestapiv2.py`

 * *Files identical despite different names*

### Comparing `thoughtspot_rest_api_v1-1.6.1/src/thoughtspot_rest_api_v1.egg-info/PKG-INFO` & `thoughtspot_rest_api_v1-1.7.0/src/thoughtspot_rest_api_v1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thoughtspot_rest_api_v1
-Version: 1.6.1
+Version: 1.7.0
 Summary: Library implementing the ThoughtSpot V1 REST API
 Home-page: https://github.com/thoughtspot/thoughtspot_rest_api_v1_python
 Author: Bryant Howell
 Author-email: bryant.howell@thoughtspot.com
 License: MIT
 Project-URL: Documentation, https://github.com/thoughtspot/thoughtspot_rest_api_v1_python#readme
 Project-URL: Bug Tracker, https://github.com/thoughtspot/thoughtspot_rest_api_v1_python/issues
```

### Comparing `thoughtspot_rest_api_v1-1.6.1/src/thoughtspot_rest_api_v1.egg-info/SOURCES.txt` & `thoughtspot_rest_api_v1-1.7.0/src/thoughtspot_rest_api_v1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

