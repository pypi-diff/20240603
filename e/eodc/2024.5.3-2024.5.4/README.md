# Comparing `tmp/eodc-2024.5.3.tar.gz` & `tmp/eodc-2024.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc-2024.5.3.tar", max compression
+gzip compressed data, was "eodc-2024.5.4.tar", max compression
```

## Comparing `eodc-2024.5.3.tar` & `eodc-2024.5.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      733 2024-05-29 12:12:24.051768 eodc-2024.5.3/README.md
--rw-r--r--   0        0        0      195 2024-05-29 12:12:24.051768 eodc-2024.5.3/eodc/__init__.py
--rw-r--r--   0        0        0     1794 2024-05-29 12:12:24.051768 eodc-2024.5.3/eodc/auth.py
--rw-r--r--   0        0        0     1311 2024-05-29 12:12:24.051768 eodc-2024.5.3/eodc/dask.py
--rw-r--r--   0        0        0    13711 2024-05-29 12:12:24.051768 eodc-2024.5.3/eodc/faas.py
--rw-r--r--   0        0        0     1183 2024-05-29 12:12:24.051768 eodc-2024.5.3/eodc/settings.py
--rw-r--r--   0        0        0     2240 2024-05-29 12:12:24.051768 eodc-2024.5.3/eodc/storage.py
--rw-r--r--   0        0        0        0 2024-05-29 12:12:24.051768 eodc-2024.5.3/eodc/visualisation/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 12:12:24.051768 eodc-2024.5.3/eodc/visualisation/vessel_detection/__init__.py
--rwxr-xr-x   0        0        0    15080 2024-05-29 12:12:24.051768 eodc-2024.5.3/eodc/visualisation/vessel_detection/app.py
--rw-r--r--   0        0        0      261 2024-05-29 12:12:24.051768 eodc-2024.5.3/eodc/visualisation/vessel_detection/assets/app.css
--rw-r--r--   0        0        0     2539 2024-05-29 12:12:24.051768 eodc-2024.5.3/eodc/visualisation/vessel_detection/cards.py
--rw-r--r--   0        0        0     8522 2024-05-29 12:12:24.051768 eodc-2024.5.3/eodc/visualisation/vessel_detection/navbar.py
--rw-r--r--   0        0        0     2867 2024-05-29 12:12:24.055768 eodc-2024.5.3/eodc/visualisation/vessel_detection/utils.py
--rw-r--r--   0        0        0    37916 2024-05-29 12:12:24.055768 eodc-2024.5.3/eodc/workspace.py
--rw-r--r--   0        0        0     1890 2024-05-29 12:12:24.055768 eodc-2024.5.3/pyproject.toml
--rw-r--r--   0        0        0     2859 1970-01-01 00:00:00.000000 eodc-2024.5.3/PKG-INFO
+-rw-r--r--   0        0        0      733 2024-06-03 13:20:28.097953 eodc-2024.5.4/README.md
+-rw-r--r--   0        0        0      195 2024-06-03 13:20:28.097953 eodc-2024.5.4/eodc/__init__.py
+-rw-r--r--   0        0        0     1794 2024-06-03 13:20:28.097953 eodc-2024.5.4/eodc/auth.py
+-rw-r--r--   0        0        0     1311 2024-06-03 13:20:28.097953 eodc-2024.5.4/eodc/dask.py
+-rw-r--r--   0        0        0    13711 2024-06-03 13:20:28.097953 eodc-2024.5.4/eodc/faas.py
+-rw-r--r--   0        0        0     1183 2024-06-03 13:20:28.097953 eodc-2024.5.4/eodc/settings.py
+-rw-r--r--   0        0        0     2240 2024-06-03 13:20:28.097953 eodc-2024.5.4/eodc/storage.py
+-rw-r--r--   0        0        0        0 2024-06-03 13:20:28.097953 eodc-2024.5.4/eodc/visualisation/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-03 13:20:28.097953 eodc-2024.5.4/eodc/visualisation/vessel_detection/__init__.py
+-rwxr-xr-x   0        0        0    15080 2024-06-03 13:20:28.097953 eodc-2024.5.4/eodc/visualisation/vessel_detection/app.py
+-rw-r--r--   0        0        0      261 2024-06-03 13:20:28.097953 eodc-2024.5.4/eodc/visualisation/vessel_detection/assets/app.css
+-rw-r--r--   0        0        0     2539 2024-06-03 13:20:28.097953 eodc-2024.5.4/eodc/visualisation/vessel_detection/cards.py
+-rw-r--r--   0        0        0     8522 2024-06-03 13:20:28.097953 eodc-2024.5.4/eodc/visualisation/vessel_detection/navbar.py
+-rw-r--r--   0        0        0     2867 2024-06-03 13:20:28.097953 eodc-2024.5.4/eodc/visualisation/vessel_detection/utils.py
+-rw-r--r--   0        0        0    37799 2024-06-03 13:20:28.097953 eodc-2024.5.4/eodc/workspace.py
+-rw-r--r--   0        0        0     1890 2024-06-03 13:20:28.101953 eodc-2024.5.4/pyproject.toml
+-rw-r--r--   0        0        0     2859 1970-01-01 00:00:00.000000 eodc-2024.5.4/PKG-INFO
```

### Comparing `eodc-2024.5.3/README.md` & `eodc-2024.5.4/README.md`

 * *Files identical despite different names*

### Comparing `eodc-2024.5.3/eodc/auth.py` & `eodc-2024.5.4/eodc/auth.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.5.3/eodc/dask.py` & `eodc-2024.5.4/eodc/dask.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.5.3/eodc/faas.py` & `eodc-2024.5.4/eodc/faas.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.5.3/eodc/settings.py` & `eodc-2024.5.4/eodc/settings.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.5.3/eodc/storage.py` & `eodc-2024.5.4/eodc/storage.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.5.3/eodc/visualisation/vessel_detection/app.py` & `eodc-2024.5.4/eodc/visualisation/vessel_detection/app.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.5.3/eodc/visualisation/vessel_detection/cards.py` & `eodc-2024.5.4/eodc/visualisation/vessel_detection/cards.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.5.3/eodc/visualisation/vessel_detection/navbar.py` & `eodc-2024.5.4/eodc/visualisation/vessel_detection/navbar.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.5.3/eodc/visualisation/vessel_detection/utils.py` & `eodc-2024.5.4/eodc/visualisation/vessel_detection/utils.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.5.3/eodc/workspace.py` & `eodc-2024.5.4/eodc/workspace.py`

 * *Files 1% similar despite different names*

```diff
@@ -638,17 +638,14 @@
     def get_credentials(self):
         return {
             "url": self.url,
             "access_key": self.access_key.get_secret_value(),
             "secret_key": self.secret_key.get_secret_value(),
         }
 
-    def register_user(self, user_name: str) -> dict[str, str]:
-        return {}  # TODO: blocked by philipp API
-
     def list_workspaces(self) -> list[str]:
         return [bucket["Name"] for bucket in self.s3_client.list_buckets()["Buckets"]]
 
     def create_user_workspace(
         self, workspace_name: str, user_name: str = "", tenant_name: str = ""
     ) -> None:
         self.s3_client.create_bucket(Bucket=workspace_name)
@@ -699,18 +696,18 @@
     def get_workspace(self, workspace_name: str):
         return self.s3_client.get_bucket(workspace_name)
 
     def get_fsspec(self, workspace_name: str):
         return fsspec.filesystem(
             "s3",
             anon=False,
-            key=self.get_s3_credentials()["access_key"],
-            secret=self.get_s3_credentials()["secret_key"],
+            key=self.get_credentials()["access_key"],
+            secret=self.get_credentials()["secret_key"],
             client_kwargs={
-                "endpoint_url": self.get_s3_credentials()["url"],
+                "endpoint_url": self.get_credentials()["url"],
             },
             bucket=workspace_name,
         )
 
     def get_signed_url(
         self, bucket_name, object_key, method="GET", expiration_time=3600
     ):
@@ -726,16 +723,16 @@
     # Policies
     def _grant_policy_to_workspace(self, workspace_name: str, policy_string: str):
         self.s3_client.put_bucket_policy(Bucket=workspace_name, Policy=policy_string)
 
     def grant_workspace_to_user(self, user_name: str, workspace_name: str, tenant_name):
         policy_str = (
             S3PolicyBuilder(f"BASIC_{workspace_name.upper()}_{tenant_name}_{user_name}")
-            .add_user_full_privileges(
-                workspace_name, user=user_name, tenant=tenant_name
+            .add_users_full_privileges(
+                workspace_name, tenant_users=[(tenant_name, user_name)]
             )
             .build()
         )
         self._grant_policy_to_workspace(
             workspace_name=workspace_name, policy_string=json.dumps(policy_str)
         )
```

### Comparing `eodc-2024.5.3/pyproject.toml` & `eodc-2024.5.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "eodc"
 
-version = "2024.5.3"
+version = "2024.5.4"
 description = "Python SDK for interacting with EODC services."
 authors = ["Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>", "Gerald Irsiegler <gerald.irsiegler@eodc.eu>", "Christoph Reimer <christoph.reimer@eodc.eu>"]
 maintainers = ["EODC Staff <support@eodc.eu>"]
 readme = "README.md"
 repository = "https://github.com/eodcgmbh/eodc-sdk"
 classifiers = [
     "Development Status :: 1 - Planning",
```

### Comparing `eodc-2024.5.3/PKG-INFO` & `eodc-2024.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodc
-Version: 2024.5.3
+Version: 2024.5.4
 Summary: Python SDK for interacting with EODC services.
 Home-page: https://github.com/eodcgmbh/eodc-sdk
 Author: Lukas Weidenholzer
 Author-email: lukas.weidenholzer@eodc.eu
 Maintainer: EODC Staff
 Maintainer-email: support@eodc.eu
 Requires-Python: >=3.9,<3.12
```

