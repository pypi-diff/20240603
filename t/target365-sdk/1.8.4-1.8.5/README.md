# Comparing `tmp/target365_sdk-1.8.4.tar.gz` & `tmp/target365_sdk-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "target365_sdk-1.8.4.tar", last modified: Thu Feb 15 13:40:13 2024, max compression
+gzip compressed data, was "target365_sdk-1.8.5.tar", last modified: Mon Jun  3 15:23:14 2024, max compression
```

## Comparing `target365_sdk-1.8.4.tar` & `target365_sdk-1.8.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-02-15 13:40:13.470522 target365_sdk-1.8.4/
--rw-rw-rw-   0        0        0     1101 2020-08-24 14:04:16.000000 target365_sdk-1.8.4/LICENSE
--rw-rw-rw-   0        0        0     1050 2024-02-15 13:40:13.468522 target365_sdk-1.8.4/PKG-INFO
--rw-rw-rw-   0        0        0     4010 2021-11-03 16:18:43.000000 target365_sdk-1.8.4/README.md
--rw-rw-rw-   0        0        0       42 2024-02-15 13:40:13.470522 target365_sdk-1.8.4/setup.cfg
--rw-rw-rw-   0        0        0     1270 2024-02-15 13:37:47.000000 target365_sdk-1.8.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-15 13:40:13.414509 target365_sdk-1.8.4/target365_sdk/
--rw-rw-rw-   0        0        0       61 2020-08-24 14:04:16.000000 target365_sdk-1.8.4/target365_sdk/__init__.py
--rw-rw-rw-   0        0        0    18108 2023-11-01 15:54:08.000000 target365_sdk-1.8.4/target365_sdk/api_client.py
-drwxrwxrwx   0        0        0        0 2024-02-15 13:40:13.428513 target365_sdk-1.8.4/target365_sdk/helpers/
--rw-rw-rw-   0        0        0        0 2020-08-24 14:04:16.000000 target365_sdk-1.8.4/target365_sdk/helpers/__init__.py
--rw-rw-rw-   0        0        0     2972 2023-11-01 21:34:02.000000 target365_sdk-1.8.4/target365_sdk/helpers/http_client.py
-drwxrwxrwx   0        0        0        0 2024-02-15 13:40:13.460521 target365_sdk-1.8.4/target365_sdk/models/
--rw-rw-rw-   0        0        0        0 2020-08-24 14:04:16.000000 target365_sdk-1.8.4/target365_sdk/models/__init__.py
--rw-rw-rw-   0        0        0      631 2024-02-15 13:37:40.000000 target365_sdk-1.8.4/target365_sdk/models/delivery_report.py
--rw-rw-rw-   0        0        0     1189 2021-11-05 14:32:42.000000 target365_sdk-1.8.4/target365_sdk/models/detailed_status_codes.py
--rw-rw-rw-   0        0        0      436 2020-08-24 14:04:16.000000 target365_sdk-1.8.4/target365_sdk/models/in_message.py
--rw-rw-rw-   0        0        0      465 2022-08-04 11:54:49.000000 target365_sdk-1.8.4/target365_sdk/models/keyword.py
--rw-rw-rw-   0        0        0      352 2022-08-04 11:54:49.000000 target365_sdk-1.8.4/target365_sdk/models/keyword_preauth_settings.py
--rw-rw-rw-   0        0        0      557 2020-08-24 14:04:16.000000 target365_sdk-1.8.4/target365_sdk/models/lookup_result.py
--rw-rw-rw-   0        0        0     1106 2020-08-24 14:04:16.000000 target365_sdk-1.8.4/target365_sdk/models/model.py
--rw-rw-rw-   0        0        0      429 2020-08-24 14:04:16.000000 target365_sdk-1.8.4/target365_sdk/models/one_time_password.py
--rw-rw-rw-   0        0        0      728 2021-11-30 13:41:48.000000 target365_sdk-1.8.4/target365_sdk/models/oneclick_config.py
--rw-rw-rw-   0        0        0     1528 2022-08-04 11:54:49.000000 target365_sdk-1.8.4/target365_sdk/models/out_message.py
--rw-rw-rw-   0        0        0      524 2021-11-30 13:43:11.000000 target365_sdk-1.8.4/target365_sdk/models/out_message_strex.py
--rw-rw-rw-   0        0        0      306 2024-02-15 13:35:21.000000 target365_sdk-1.8.4/target365_sdk/models/pincode.py
--rw-rw-rw-   0        0        0      354 2020-08-24 14:04:16.000000 target365_sdk-1.8.4/target365_sdk/models/public_key.py
--rw-rw-rw-   0        0        0      127 2020-08-24 14:04:16.000000 target365_sdk-1.8.4/target365_sdk/models/status_codes.py
--rw-rw-rw-   0        0        0      244 2020-08-24 14:04:16.000000 target365_sdk-1.8.4/target365_sdk/models/strex_merchant.py
--rw-rw-rw-   0        0        0      235 2021-11-03 16:18:43.000000 target365_sdk-1.8.4/target365_sdk/models/strex_registration_sms.py
--rw-rw-rw-   0        0        0      979 2022-08-04 11:54:49.000000 target365_sdk-1.8.4/target365_sdk/models/strex_transaction.py
--rw-rw-rw-   0        0        0      302 2021-11-03 16:18:43.000000 target365_sdk-1.8.4/target365_sdk/models/user_validity.py
-drwxrwxrwx   0        0        0        0 2024-02-15 13:40:13.464523 target365_sdk-1.8.4/target365_sdk/tests/
--rw-rw-rw-   0        0        0        0 2020-08-24 14:04:16.000000 target365_sdk-1.8.4/target365_sdk/tests/__init__.py
--rw-rw-rw-   0        0        0    11204 2024-02-15 13:37:40.000000 target365_sdk-1.8.4/target365_sdk/tests/test_api_client.py
-drwxrwxrwx   0        0        0        0 2024-02-15 13:40:13.466521 target365_sdk-1.8.4/target365_sdk.egg-info/
--rw-rw-rw-   0        0        0     1050 2024-02-15 13:40:13.000000 target365_sdk-1.8.4/target365_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1139 2024-02-15 13:40:13.000000 target365_sdk-1.8.4/target365_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-15 13:40:13.000000 target365_sdk-1.8.4/target365_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-02-15 13:40:13.000000 target365_sdk-1.8.4/target365_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-02-15 13:40:13.000000 target365_sdk-1.8.4/target365_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-03 15:23:14.981885 target365_sdk-1.8.5/
+-rw-rw-rw-   0        0        0     1101 2020-08-24 14:04:16.000000 target365_sdk-1.8.5/LICENSE
+-rw-rw-rw-   0        0        0     1050 2024-06-03 15:23:14.979884 target365_sdk-1.8.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4010 2021-11-03 16:18:43.000000 target365_sdk-1.8.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-03 15:23:14.982885 target365_sdk-1.8.5/setup.cfg
+-rw-rw-rw-   0        0        0     1270 2024-06-03 15:23:01.000000 target365_sdk-1.8.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 15:23:14.851158 target365_sdk-1.8.5/target365_sdk/
+-rw-rw-rw-   0        0        0       61 2020-08-24 14:04:16.000000 target365_sdk-1.8.5/target365_sdk/__init__.py
+-rw-rw-rw-   0        0        0    18108 2023-11-01 15:54:08.000000 target365_sdk-1.8.5/target365_sdk/api_client.py
+drwxrwxrwx   0        0        0        0 2024-06-03 15:23:14.874163 target365_sdk-1.8.5/target365_sdk/helpers/
+-rw-rw-rw-   0        0        0        0 2020-08-24 14:04:16.000000 target365_sdk-1.8.5/target365_sdk/helpers/__init__.py
+-rw-rw-rw-   0        0        0     2972 2024-06-03 15:23:07.000000 target365_sdk-1.8.5/target365_sdk/helpers/http_client.py
+drwxrwxrwx   0        0        0        0 2024-06-03 15:23:14.960881 target365_sdk-1.8.5/target365_sdk/models/
+-rw-rw-rw-   0        0        0        0 2020-08-24 14:04:16.000000 target365_sdk-1.8.5/target365_sdk/models/__init__.py
+-rw-rw-rw-   0        0        0      631 2024-02-15 13:37:40.000000 target365_sdk-1.8.5/target365_sdk/models/delivery_report.py
+-rw-rw-rw-   0        0        0     1189 2021-11-05 14:32:42.000000 target365_sdk-1.8.5/target365_sdk/models/detailed_status_codes.py
+-rw-rw-rw-   0        0        0      436 2020-08-24 14:04:16.000000 target365_sdk-1.8.5/target365_sdk/models/in_message.py
+-rw-rw-rw-   0        0        0      465 2022-08-04 11:54:49.000000 target365_sdk-1.8.5/target365_sdk/models/keyword.py
+-rw-rw-rw-   0        0        0      352 2022-08-04 11:54:49.000000 target365_sdk-1.8.5/target365_sdk/models/keyword_preauth_settings.py
+-rw-rw-rw-   0        0        0      557 2020-08-24 14:04:16.000000 target365_sdk-1.8.5/target365_sdk/models/lookup_result.py
+-rw-rw-rw-   0        0        0     1106 2020-08-24 14:04:16.000000 target365_sdk-1.8.5/target365_sdk/models/model.py
+-rw-rw-rw-   0        0        0      429 2020-08-24 14:04:16.000000 target365_sdk-1.8.5/target365_sdk/models/one_time_password.py
+-rw-rw-rw-   0        0        0      728 2021-11-30 13:41:48.000000 target365_sdk-1.8.5/target365_sdk/models/oneclick_config.py
+-rw-rw-rw-   0        0        0     1528 2022-08-04 11:54:49.000000 target365_sdk-1.8.5/target365_sdk/models/out_message.py
+-rw-rw-rw-   0        0        0      524 2021-11-30 13:43:11.000000 target365_sdk-1.8.5/target365_sdk/models/out_message_strex.py
+-rw-rw-rw-   0        0        0      306 2024-02-15 13:35:21.000000 target365_sdk-1.8.5/target365_sdk/models/pincode.py
+-rw-rw-rw-   0        0        0      354 2020-08-24 14:04:16.000000 target365_sdk-1.8.5/target365_sdk/models/public_key.py
+-rw-rw-rw-   0        0        0      127 2020-08-24 14:04:16.000000 target365_sdk-1.8.5/target365_sdk/models/status_codes.py
+-rw-rw-rw-   0        0        0      244 2020-08-24 14:04:16.000000 target365_sdk-1.8.5/target365_sdk/models/strex_merchant.py
+-rw-rw-rw-   0        0        0      235 2021-11-03 16:18:43.000000 target365_sdk-1.8.5/target365_sdk/models/strex_registration_sms.py
+-rw-rw-rw-   0        0        0     1005 2024-06-03 15:04:14.000000 target365_sdk-1.8.5/target365_sdk/models/strex_transaction.py
+-rw-rw-rw-   0        0        0      302 2021-11-03 16:18:43.000000 target365_sdk-1.8.5/target365_sdk/models/user_validity.py
+drwxrwxrwx   0        0        0        0 2024-06-03 15:23:14.975883 target365_sdk-1.8.5/target365_sdk/tests/
+-rw-rw-rw-   0        0        0        0 2020-08-24 14:04:16.000000 target365_sdk-1.8.5/target365_sdk/tests/__init__.py
+-rw-rw-rw-   0        0        0    11204 2024-02-15 13:37:40.000000 target365_sdk-1.8.5/target365_sdk/tests/test_api_client.py
+drwxrwxrwx   0        0        0        0 2024-06-03 15:23:14.977892 target365_sdk-1.8.5/target365_sdk.egg-info/
+-rw-rw-rw-   0        0        0     1050 2024-06-03 15:23:14.000000 target365_sdk-1.8.5/target365_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1139 2024-06-03 15:23:14.000000 target365_sdk-1.8.5/target365_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 15:23:14.000000 target365_sdk-1.8.5/target365_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-06-03 15:23:14.000000 target365_sdk-1.8.5/target365_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-06-03 15:23:14.000000 target365_sdk-1.8.5/target365_sdk.egg-info/top_level.txt
```

### Comparing `target365_sdk-1.8.4/LICENSE` & `target365_sdk-1.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `target365_sdk-1.8.4/PKG-INFO` & `target365_sdk-1.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: target365_sdk
-Version: 1.8.4
+Version: 1.8.5
 Summary: Target365 SDK
 Home-page: https://github.com/Target365/sdk-for-python
 Author: Target365
 Author-email: support@target365.no
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
```

### Comparing `target365_sdk-1.8.4/README.md` & `target365_sdk-1.8.5/README.md`

 * *Files identical despite different names*

### Comparing `target365_sdk-1.8.4/setup.py` & `target365_sdk-1.8.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="target365_sdk",
-    version="1.8.4",
+    version="1.8.5",
     author="Target365",
     author_email="support@target365.no",
     description="Target365 SDK",
     long_description="Enables integration with Target365 online services.",
     long_description_content_type="text/markdown",
     url="https://github.com/Target365/sdk-for-python",
     packages=setuptools.find_packages(),
```

### Comparing `target365_sdk-1.8.4/target365_sdk/api_client.py` & `target365_sdk-1.8.5/target365_sdk/api_client.py`

 * *Files identical despite different names*

### Comparing `target365_sdk-1.8.4/target365_sdk/helpers/http_client.py` & `target365_sdk-1.8.5/target365_sdk/helpers/http_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         )
 
     def _build_url(self, path):
         return (self.base_uri + path)
 
     def _get_auth_headers(self, method, uri, body=None):
         signature = self._get_signature(method, uri, body)
-        return { "Authorization": "ECDSA " + signature, "X-SDK": "Python", "X-Sdk-Version": "1.8.2" }
+        return { "Authorization": "ECDSA " + signature, "X-SDK": "Python", "X-Sdk-Version": "1.8.5" }
 
     def _get_signature(self, method, uri, body=None):
         timestamp = int(time.time())
         nounce = uuid.uuid4()
 
         content_hash = ""
         if body is not None:
```

### Comparing `target365_sdk-1.8.4/target365_sdk/models/delivery_report.py` & `target365_sdk-1.8.5/target365_sdk/models/delivery_report.py`

 * *Files identical despite different names*

### Comparing `target365_sdk-1.8.4/target365_sdk/models/detailed_status_codes.py` & `target365_sdk-1.8.5/target365_sdk/models/detailed_status_codes.py`

 * *Files identical despite different names*

### Comparing `target365_sdk-1.8.4/target365_sdk/models/lookup_result.py` & `target365_sdk-1.8.5/target365_sdk/models/lookup_result.py`

 * *Files identical despite different names*

### Comparing `target365_sdk-1.8.4/target365_sdk/models/model.py` & `target365_sdk-1.8.5/target365_sdk/models/model.py`

 * *Files identical despite different names*

### Comparing `target365_sdk-1.8.4/target365_sdk/models/oneclick_config.py` & `target365_sdk-1.8.5/target365_sdk/models/oneclick_config.py`

 * *Files identical despite different names*

### Comparing `target365_sdk-1.8.4/target365_sdk/models/out_message.py` & `target365_sdk-1.8.5/target365_sdk/models/out_message.py`

 * *Files identical despite different names*

### Comparing `target365_sdk-1.8.4/target365_sdk/models/out_message_strex.py` & `target365_sdk-1.8.5/target365_sdk/models/out_message_strex.py`

 * *Files identical despite different names*

### Comparing `target365_sdk-1.8.4/target365_sdk/models/strex_transaction.py` & `target365_sdk-1.8.5/target365_sdk/models/strex_transaction.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
     def _accepted_params(self):
         return [
             'transactionId',
             'sessionId',
             'correlationId',
             'shortNumber',
+            'keywordId',
             'recipient',
             'content',
             'oneTimePassword',
             'deliveryMode',
             'statusCode',
             'detailedStatusCode',
             'statusDescription',
```

### Comparing `target365_sdk-1.8.4/target365_sdk/tests/test_api_client.py` & `target365_sdk-1.8.5/target365_sdk/tests/test_api_client.py`

 * *Files identical despite different names*

### Comparing `target365_sdk-1.8.4/target365_sdk.egg-info/PKG-INFO` & `target365_sdk-1.8.5/target365_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: target365_sdk
-Version: 1.8.4
+Version: 1.8.5
 Summary: Target365 SDK
 Home-page: https://github.com/Target365/sdk-for-python
 Author: Target365
 Author-email: support@target365.no
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
```

### Comparing `target365_sdk-1.8.4/target365_sdk.egg-info/SOURCES.txt` & `target365_sdk-1.8.5/target365_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

