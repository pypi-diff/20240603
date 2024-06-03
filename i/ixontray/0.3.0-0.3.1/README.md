# Comparing `tmp/ixontray-0.3.0.tar.gz` & `tmp/ixontray-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ixontray-0.3.0.tar", last modified: Tue May 21 06:31:02 2024, max compression
+gzip compressed data, was "ixontray-0.3.1.tar", last modified: Mon Jun  3 11:14:57 2024, max compression
```

## Comparing `ixontray-0.3.0.tar` & `ixontray-0.3.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1273 2024-01-12 19:04:27.438207 ixontray-0.3.0/README.md
--rw-r--r--   0        0        0     2405 2024-05-21 06:31:02.350226 ixontray-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       22 2024-05-21 06:24:02.838938 ixontray-0.3.0/src/ixontray/__init__.py
--rw-r--r--   0        0        0     2881 2023-11-03 06:14:26.000000 ixontray-0.3.0/src/ixontray/base_model_store.py
--rw-r--r--   0        0        0     1024 2023-08-31 08:03:34.000000 ixontray-0.3.0/src/ixontray/commands-windows.yaml
--rw-r--r--   0        0        0     1562 2023-11-06 14:21:03.000000 ixontray-0.3.0/src/ixontray/commands.yaml
--rw-r--r--   0        0        0      579 2023-09-05 07:42:07.000000 ixontray-0.3.0/src/ixontray/config.py
--rw-r--r--   0        0        0    18724 2023-08-31 08:03:34.000000 ixontray-0.3.0/src/ixontray/icon.png
--rw-r--r--   0        0        0     3425 2023-08-31 08:03:34.000000 ixontray-0.3.0/src/ixontray/icon_not_connected.png
--rw-r--r--   0        0        0      227 2023-08-31 08:03:34.000000 ixontray-0.3.0/src/ixontray/install.sh
--rw-r--r--   0        0        0     5299 2023-11-01 19:04:15.000000 ixontray-0.3.0/src/ixontray/ixon_cloud_api.py
--rwxr-xr-x   0        0        0    24495 2024-05-21 06:23:07.359037 ixontray-0.3.0/src/ixontray/ixon_tray.py
--rw-r--r--   0        0        0     3497 2023-09-05 07:42:07.000000 ixontray-0.3.0/src/ixontray/ixon_vpn_client_api.py
--rw-r--r--   0        0        0     7340 2023-11-27 20:22:01.000000 ixontray-0.3.0/src/ixontray/launcher.py
--rw-r--r--   0        0        0    16738 2024-05-21 06:23:07.247038 ixontray-0.3.0/src/ixontray/settings_window.py
--rw-r--r--   0        0        0     5194 2023-11-27 19:49:24.000000 ixontray-0.3.0/src/ixontray/telemetry.py
--rw-r--r--   0        0        0      352 2023-08-31 08:03:34.000000 ixontray-0.3.0/src/ixontray/types/__init__.py
--rw-r--r--   0        0        0     2549 2023-09-05 07:42:07.000000 ixontray-0.3.0/src/ixontray/types/api.py
--rw-r--r--   0        0        0     1216 2023-08-31 19:07:34.000000 ixontray-0.3.0/src/ixontray/types/common.py
--rw-r--r--   0        0        0      863 2023-11-01 20:59:06.000000 ixontray-0.3.0/src/ixontray/update.py
--rw-r--r--   0        0        0      352 2024-01-12 16:09:11.201816 ixontray-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0      562 2024-01-12 16:09:11.201816 ixontray-0.3.0/tests/conftest.py
--rw-r--r--   0        0        0     3467 2024-01-12 16:09:11.201816 ixontray-0.3.0/tests/test_basemodel_store.py
--rw-r--r--   0        0        0     1320 2024-01-12 16:09:11.201816 ixontray-0.3.0/tests/test_ixon_cloud_api_v1.py
--rw-r--r--   0        0        0     1441 2024-01-12 16:09:11.201816 ixontray-0.3.0/tests/test_ixon_cloud_api_v2.py
--rw-r--r--   0        0        0     1623 2024-01-12 16:09:11.201816 ixontray-0.3.0/tests/test_ixon_vpn_api.py
--rw-r--r--   0        0        0     1247 2024-01-12 19:04:27.450207 ixontray-0.3.0/tests/test_telemetry.py
--rw-r--r--   0        0        0     1758 1970-01-01 00:00:00.000000 ixontray-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1273 2024-01-12 19:04:27.438207 ixontray-0.3.1/README.md
+-rw-r--r--   0        0        0     2405 2024-06-03 11:14:57.702142 ixontray-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-06-03 11:14:40.934167 ixontray-0.3.1/src/ixontray/__init__.py
+-rw-r--r--   0        0        0     2881 2023-11-03 06:14:26.000000 ixontray-0.3.1/src/ixontray/base_model_store.py
+-rw-r--r--   0        0        0     1024 2023-08-31 08:03:34.000000 ixontray-0.3.1/src/ixontray/commands-windows.yaml
+-rw-r--r--   0        0        0     1562 2023-11-06 14:21:03.000000 ixontray-0.3.1/src/ixontray/commands.yaml
+-rw-r--r--   0        0        0      579 2023-09-05 07:42:07.000000 ixontray-0.3.1/src/ixontray/config.py
+-rw-r--r--   0        0        0    18724 2023-08-31 08:03:34.000000 ixontray-0.3.1/src/ixontray/icon.png
+-rw-r--r--   0        0        0     3425 2023-08-31 08:03:34.000000 ixontray-0.3.1/src/ixontray/icon_not_connected.png
+-rw-r--r--   0        0        0      227 2023-08-31 08:03:34.000000 ixontray-0.3.1/src/ixontray/install.sh
+-rw-r--r--   0        0        0     5352 2024-06-03 11:14:12.206210 ixontray-0.3.1/src/ixontray/ixon_cloud_api.py
+-rwxr-xr-x   0        0        0    24520 2024-06-03 11:12:15.326382 ixontray-0.3.1/src/ixontray/ixon_tray.py
+-rw-r--r--   0        0        0     3497 2023-09-05 07:42:07.000000 ixontray-0.3.1/src/ixontray/ixon_vpn_client_api.py
+-rw-r--r--   0        0        0     7340 2023-11-27 20:22:01.000000 ixontray-0.3.1/src/ixontray/launcher.py
+-rw-r--r--   0        0        0    16742 2024-06-03 11:11:11.634473 ixontray-0.3.1/src/ixontray/settings_window.py
+-rw-r--r--   0        0        0     5194 2023-11-27 19:49:24.000000 ixontray-0.3.1/src/ixontray/telemetry.py
+-rw-r--r--   0        0        0      352 2023-08-31 08:03:34.000000 ixontray-0.3.1/src/ixontray/types/__init__.py
+-rw-r--r--   0        0        0     2549 2023-09-05 07:42:07.000000 ixontray-0.3.1/src/ixontray/types/api.py
+-rw-r--r--   0        0        0     1216 2023-08-31 19:07:34.000000 ixontray-0.3.1/src/ixontray/types/common.py
+-rw-r--r--   0        0        0      863 2023-11-01 20:59:06.000000 ixontray-0.3.1/src/ixontray/update.py
+-rw-r--r--   0        0        0      352 2024-01-12 16:09:11.201816 ixontray-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0      562 2024-01-12 16:09:11.201816 ixontray-0.3.1/tests/conftest.py
+-rw-r--r--   0        0        0     3467 2024-01-12 16:09:11.201816 ixontray-0.3.1/tests/test_basemodel_store.py
+-rw-r--r--   0        0        0     1320 2024-01-12 16:09:11.201816 ixontray-0.3.1/tests/test_ixon_cloud_api_v1.py
+-rw-r--r--   0        0        0     1441 2024-01-12 16:09:11.201816 ixontray-0.3.1/tests/test_ixon_cloud_api_v2.py
+-rw-r--r--   0        0        0     1623 2024-01-12 16:09:11.201816 ixontray-0.3.1/tests/test_ixon_vpn_api.py
+-rw-r--r--   0        0        0     1247 2024-01-12 19:04:27.450207 ixontray-0.3.1/tests/test_telemetry.py
+-rw-r--r--   0        0        0     1758 1970-01-01 00:00:00.000000 ixontray-0.3.1/PKG-INFO
```

### Comparing `ixontray-0.3.0/README.md` & `ixontray-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ixontray-0.3.0/pyproject.toml` & `ixontray-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -159,14 +159,14 @@
     "packaging>=23.2",
 ]
 requires-python = ">=3.10"
 keywords = [
     "tool",
     "ixon",
 ]
-version = "0.3.0"
+version = "0.3.1"
 
 [project.license]
 text = "BSD"
 
 [project.scripts]
 ixontray = "ixontray.ixon_tray:main"
```

### Comparing `ixontray-0.3.0/src/ixontray/base_model_store.py` & `ixontray-0.3.1/src/ixontray/base_model_store.py`

 * *Files identical despite different names*

### Comparing `ixontray-0.3.0/src/ixontray/commands-windows.yaml` & `ixontray-0.3.1/src/ixontray/commands-windows.yaml`

 * *Files identical despite different names*

### Comparing `ixontray-0.3.0/src/ixontray/commands.yaml` & `ixontray-0.3.1/src/ixontray/commands.yaml`

 * *Files identical despite different names*

### Comparing `ixontray-0.3.0/src/ixontray/config.py` & `ixontray-0.3.1/src/ixontray/config.py`

 * *Files identical despite different names*

### Comparing `ixontray-0.3.0/src/ixontray/icon.png` & `ixontray-0.3.1/src/ixontray/icon.png`

 * *Files identical despite different names*

### Comparing `ixontray-0.3.0/src/ixontray/icon_not_connected.png` & `ixontray-0.3.1/src/ixontray/icon_not_connected.png`

 * *Files identical despite different names*

### Comparing `ixontray-0.3.0/src/ixontray/ixon_cloud_api.py` & `ixontray-0.3.1/src/ixontray/ixon_cloud_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,19 +18,21 @@
     BASE_URL = ""
 
     def __init__(self, application_id: str, token: str | None = None) -> None:
         self._application_id = application_id
         self._bearer = token
 
     @staticmethod
-    def generate_auth(email: str, pwd: str, otp: str = "") -> str:
+    def generate_auth(email: str, pwd: str, otp: str | None = None) -> str:
         """Generates the user specific authentication key for the ixon client.
 
         :return: the base64 typed string of the user credentials
         """
+        if otp is None:
+            otp = ""
         combined = f"{email}:{otp}:{pwd}"
         return base64.urlsafe_b64encode(combined.encode("UTF-8")).decode("ascii")
 
     def generate_access_token(self, auth: str) -> str | None:
         url = "https://api.ayayot.com/access-tokens?fields=secretId"
 
         headers = {
@@ -39,15 +41,14 @@
             "Content-Type": "application/json",
             "Authorization": f"Basic {auth}",
         }
 
         data = {"expiresIn": 3600}
 
         response = requests.request("POST", url, headers=headers, data=json.dumps(data))
-
         if response.status_code == HTTPStatus.CREATED:
             data = json.loads(response.text)["data"]
             self._bearer = data["secretId"]
             return self._bearer
 
         return None
```

### Comparing `ixontray-0.3.0/src/ixontray/ixon_tray.py` & `ixontray-0.3.1/src/ixontray/ixon_tray.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,14 +216,15 @@
         auth_string = self.get_auth_string()
         if auth_string is None:
             logger.info("No auth string")
             return
         self._ixon_api_v1 = IxonCloudAPIv1(application_id=IXapiApplicationID)
         try:
             token = self._ixon_api_v1.generate_access_token(auth=auth_string)
+            print(token)
             if token is not None:
                 self._ixon_vpn_client = IxonVpnClient(token=token)
                 self._ixon_api_v2 = IxonCloudAPIv2(application_id=IXapiApplicationID, token=token)
                 self._no_internet = False
             else:
                 self.show_login_credentials()
         except requests.exceptions.ConnectionError:
```

### Comparing `ixontray-0.3.0/src/ixontray/ixon_vpn_client_api.py` & `ixontray-0.3.1/src/ixontray/ixon_vpn_client_api.py`

 * *Files identical despite different names*

### Comparing `ixontray-0.3.0/src/ixontray/launcher.py` & `ixontray-0.3.1/src/ixontray/launcher.py`

 * *Files identical despite different names*

### Comparing `ixontray-0.3.0/src/ixontray/settings_window.py` & `ixontray-0.3.1/src/ixontray/settings_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         self.le_email = QLineEdit(username)
         self.le_password = QLineEdit(password)
         self.le_password.setEchoMode(QLineEdit.EchoMode.Password)
 
         otp_required = self._settings.value("otp", False)
         self.ch_2fa = QCheckBox()
 
-        self.ch_2fa.setChecked(bool(otp_required))
+        self.ch_2fa.setChecked(otp_required == "true")
 
         self.btn_save = QPushButton("Save")
         self.btn_save.clicked.connect(self.save_auth)
 
         self._layout = QFormLayout()
         self._layout.addRow("Auto start application", self.cb_enable_autostart)
         # self._layout.addRow("Organization ID", self.le_organization_id)
```

### Comparing `ixontray-0.3.0/src/ixontray/telemetry.py` & `ixontray-0.3.1/src/ixontray/telemetry.py`

 * *Files identical despite different names*

### Comparing `ixontray-0.3.0/src/ixontray/types/api.py` & `ixontray-0.3.1/src/ixontray/types/api.py`

 * *Files identical despite different names*

### Comparing `ixontray-0.3.0/src/ixontray/types/common.py` & `ixontray-0.3.1/src/ixontray/types/common.py`

 * *Files identical despite different names*

### Comparing `ixontray-0.3.0/src/ixontray/update.py` & `ixontray-0.3.1/src/ixontray/update.py`

 * *Files identical despite different names*

### Comparing `ixontray-0.3.0/tests/conftest.py` & `ixontray-0.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ixontray-0.3.0/tests/test_basemodel_store.py` & `ixontray-0.3.1/tests/test_basemodel_store.py`

 * *Files identical despite different names*

### Comparing `ixontray-0.3.0/tests/test_ixon_cloud_api_v1.py` & `ixontray-0.3.1/tests/test_ixon_cloud_api_v1.py`

 * *Files identical despite different names*

### Comparing `ixontray-0.3.0/tests/test_ixon_cloud_api_v2.py` & `ixontray-0.3.1/tests/test_ixon_cloud_api_v2.py`

 * *Files identical despite different names*

### Comparing `ixontray-0.3.0/tests/test_ixon_vpn_api.py` & `ixontray-0.3.1/tests/test_ixon_vpn_api.py`

 * *Files identical despite different names*

### Comparing `ixontray-0.3.0/tests/test_telemetry.py` & `ixontray-0.3.1/tests/test_telemetry.py`

 * *Files identical despite different names*

### Comparing `ixontray-0.3.0/PKG-INFO` & `ixontray-0.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ixontray
-Version: 0.3.0
+Version: 0.3.1
 Summary: A tray application and launcher to connect to remote systems using IXON
 Keywords: tool,ixon
 Author-Email: Mart Moerdijk <mart@mmoerdijk.nl>
 License: BSD
 Requires-Python: >=3.10
 Requires-Dist: PyQt6
 Requires-Dist: pydantic
```

