# Comparing `tmp/homebase_calendar_sync-0.1.7.tar.gz` & `tmp/homebase_calendar_sync-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homebase_calendar_sync-0.1.7.tar", last modified: Sun Jun  2 17:18:27 2024, max compression
+gzip compressed data, was "homebase_calendar_sync-0.1.8.tar", last modified: Mon Jun  3 00:42:24 2024, max compression
```

## Comparing `homebase_calendar_sync-0.1.7.tar` & `homebase_calendar_sync-0.1.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-02 17:18:27.828321 homebase_calendar_sync-0.1.7/
--rw-r--r--   0 davidmidlo   (501) staff       (20)     2927 2024-06-02 17:18:27.828121 homebase_calendar_sync-0.1.7/PKG-INFO
--rw-r--r--   0 davidmidlo   (501) staff       (20)      477 2024-06-02 14:42:53.000000 homebase_calendar_sync-0.1.7/README.md
--rw-r--r--   0 davidmidlo   (501) staff       (20)       38 2024-06-02 17:18:27.828371 homebase_calendar_sync-0.1.7/setup.cfg
--rw-r--r--   0 davidmidlo   (501) staff       (20)     1009 2024-06-02 17:18:19.000000 homebase_calendar_sync-0.1.7/setup.py
-drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-02 17:18:27.823861 homebase_calendar_sync-0.1.7/src/
-drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-02 17:18:27.825070 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync/
--rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 13:57:29.000000 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync/__init__.py
--rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 13:57:40.000000 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync/__main__.py
--rw-r--r--   0 davidmidlo   (501) staff       (20)      123 2024-06-02 13:40:44.000000 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync/config.py
-drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-02 17:18:27.826766 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync/db/
--rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 14:47:10.000000 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync/db/__init__.py
--rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 14:47:19.000000 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync/db/__main__.py
--rw-r--r--   0 davidmidlo   (501) staff       (20)      880 2024-06-02 17:16:23.000000 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync/db/models.py
-drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-02 17:18:27.827568 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync/google_client/
--rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 14:47:33.000000 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync/google_client/__init__.py
--rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 14:47:49.000000 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync/google_client/__main__.py
--rw-r--r--   0 davidmidlo   (501) staff       (20)    17978 2024-06-02 17:17:01.000000 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync/google_client/auth.py
--rw-r--r--   0 davidmidlo   (501) staff       (20)      106 2024-06-02 04:40:28.000000 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync/google_client/drive_types.py
--rw-r--r--   0 davidmidlo   (501) staff       (20)     9132 2024-06-02 17:18:10.000000 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync/google_client/google_client.py
--rw-r--r--   0 davidmidlo   (501) staff       (20)    13118 2024-06-02 17:17:19.000000 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync/homebase_calendar_sync.py
-drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-02 17:18:27.827749 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync.egg-info/
--rw-r--r--   0 davidmidlo   (501) staff       (20)     2927 2024-06-02 17:18:27.000000 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync.egg-info/PKG-INFO
--rw-r--r--   0 davidmidlo   (501) staff       (20)      881 2024-06-02 17:18:27.000000 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync.egg-info/SOURCES.txt
--rw-r--r--   0 davidmidlo   (501) staff       (20)        1 2024-06-02 17:18:27.000000 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync.egg-info/dependency_links.txt
--rw-r--r--   0 davidmidlo   (501) staff       (20)       94 2024-06-02 17:18:27.000000 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync.egg-info/entry_points.txt
--rw-r--r--   0 davidmidlo   (501) staff       (20)     1080 2024-06-02 17:18:27.000000 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync.egg-info/requires.txt
--rw-r--r--   0 davidmidlo   (501) staff       (20)       23 2024-06-02 17:18:27.000000 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync.egg-info/top_level.txt
+drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-03 00:42:24.755879 homebase_calendar_sync-0.1.8/
+-rw-r--r--   0 davidmidlo   (501) staff       (20)     4341 2024-06-03 00:42:24.755671 homebase_calendar_sync-0.1.8/PKG-INFO
+-rw-r--r--   0 davidmidlo   (501) staff       (20)     1891 2024-06-03 00:41:59.000000 homebase_calendar_sync-0.1.8/README.md
+-rw-r--r--   0 davidmidlo   (501) staff       (20)       38 2024-06-03 00:42:24.755918 homebase_calendar_sync-0.1.8/setup.cfg
+-rw-r--r--   0 davidmidlo   (501) staff       (20)     1009 2024-06-03 00:40:17.000000 homebase_calendar_sync-0.1.8/setup.py
+drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-03 00:42:24.750304 homebase_calendar_sync-0.1.8/src/
+drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-03 00:42:24.751715 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync/
+-rw-r--r--   0 davidmidlo   (501) staff       (20)      269 2024-06-02 18:56:09.000000 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync/__init__.py
+-rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 13:57:40.000000 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync/__main__.py
+-rw-r--r--   0 davidmidlo   (501) staff       (20)      937 2024-06-03 00:32:52.000000 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync/config.py
+drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-03 00:42:24.753584 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync/db/
+-rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 14:47:10.000000 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync/db/__init__.py
+-rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 14:47:19.000000 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync/db/__main__.py
+-rw-r--r--   0 davidmidlo   (501) staff       (20)     1084 2024-06-02 19:48:42.000000 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync/db/models.py
+drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-03 00:42:24.754942 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync/google_client/
+-rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 14:47:33.000000 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync/google_client/__init__.py
+-rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 14:47:49.000000 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync/google_client/__main__.py
+-rw-r--r--   0 davidmidlo   (501) staff       (20)    19548 2024-06-02 22:59:26.000000 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync/google_client/auth.py
+-rw-r--r--   0 davidmidlo   (501) staff       (20)      106 2024-06-02 04:40:28.000000 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync/google_client/drive_types.py
+-rw-r--r--   0 davidmidlo   (501) staff       (20)     9441 2024-06-02 22:37:29.000000 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync/google_client/google_client.py
+-rw-r--r--   0 davidmidlo   (501) staff       (20)    16434 2024-06-03 00:35:23.000000 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync/homebase_calendar_sync.py
+drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-03 00:42:24.755268 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync.egg-info/
+-rw-r--r--   0 davidmidlo   (501) staff       (20)     4341 2024-06-03 00:42:24.000000 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync.egg-info/PKG-INFO
+-rw-r--r--   0 davidmidlo   (501) staff       (20)      881 2024-06-03 00:42:24.000000 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 davidmidlo   (501) staff       (20)        1 2024-06-03 00:42:24.000000 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 davidmidlo   (501) staff       (20)       94 2024-06-03 00:42:24.000000 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync.egg-info/entry_points.txt
+-rw-r--r--   0 davidmidlo   (501) staff       (20)     1080 2024-06-03 00:42:24.000000 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync.egg-info/requires.txt
+-rw-r--r--   0 davidmidlo   (501) staff       (20)       23 2024-06-03 00:42:24.000000 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync.egg-info/top_level.txt
```

### Comparing `homebase_calendar_sync-0.1.7/setup.py` & `homebase_calendar_sync-0.1.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 from setuptools import setup, find_packages
 
 setup(
     name='homebase_calendar_sync',
-    version='0.1.7',
+    version='0.1.8',
     author='David Midlo',
     author_email='dmidlo@gmail.com',
     description='A simple web scraper that reads gethomebase.com\'s schedule and updates Google Calendar.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/dmidlo/homebase_calendar_sync',  # Update this to your project's URL
     packages=find_packages(where='src'),
```

### Comparing `homebase_calendar_sync-0.1.7/src/homebase_calendar_sync/db/models.py` & `homebase_calendar_sync-0.1.8/src/homebase_calendar_sync/db/models.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import sqlite3
+from pathlib import Path
 from .. import config
 
 
 def connect_database():
-    config.DB = sqlite3.connect("events.db")
+    config.DB = sqlite3.connect(config.DB_NAME)
     config.DB_CURSOR = config.DB.cursor()
 
 
 def setup_database():
-    config.DB = sqlite3.connect("events.db")
+    config.DB = sqlite3.connect(config.DB_NAME)
     config.DB_CURSOR = config.DB.cursor()
     config.DB_CURSOR.execute(
         """
         CREATE TABLE IF NOT EXISTS events (
             id INTEGER PRIMARY KEY AUTOINCREMENT,
             event_id TEXT NOT NULL UNIQUE,
             hash TEXT NOT NULL,
@@ -27,7 +28,14 @@
             id INTEGER PRIMARY KEY AUTOINCREMENT,
             homebase_shift_id TEXT NOT NULL UNIQUE,
             hash TEXT NOT NULL
         )
     """
     )
     config.DB.commit()
+
+def reset_database():
+    db_path = Path.cwd() / config.DB_NAME
+    try:
+        db_path.unlink()
+    except FileNotFoundError:
+        print("no events database to reset")
```

### Comparing `homebase_calendar_sync-0.1.7/src/homebase_calendar_sync/google_client/auth.py` & `homebase_calendar_sync-0.1.8/src/homebase_calendar_sync/google_client/auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,14 +44,17 @@
 from googleapiclient.discovery import Resource
 from googleapiclient.discovery import build
 
 from cryptography.fernet import Fernet
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
 
+from InquirerPy import inquirer
+from InquirerPy.validator import PathValidator
+
 from .. import config
 
 
 class AuthGoogle:
     """
     A class for managing Google authentication credentials and services.
 
@@ -265,18 +268,24 @@
 
         Note:
             The client configuration should be set in `config.META.google_client_secret` before calling this method.
             The client secrets file can be downloaded from the Google Cloud Console at:
             https://console.cloud.google.com/apis/credentials?project=YOUR_PROJECT
         """
         if not config.META.google_client_token:
-            flow: "InstalledAppFlow" = InstalledAppFlow.from_client_config(
-                config.META.google_client_secret, api_scopes
-            )
-            return json.loads(Credentials.to_json(flow.run_local_server(port=0)))
+            try:
+                flow: "InstalledAppFlow" = InstalledAppFlow.from_client_config(
+                    config.META.google_client_secret, api_scopes
+                )
+                return json.loads(Credentials.to_json(flow.run_local_server(port=0)))
+            except ValueError as e:
+                if "client secrets" in str(e).lower():
+                    print("No Google Auth Credentials found. \n download a new client_secrets.json file from: https://console.cloud.google.com/apis/credentials")
+                    raise SystemExit
+
         return config.META.google_client_token
 
     def fetch_credentials(self, api_scopes) -> None:
         """
         Fetches Google OAuth2 credentials and stores them in the `config.META.google_client_token`
         configuration variable. This method first attempts to refresh the existing credentials using
         the `refresh_google_auth_creds` static method. If the credentials are not valid or are not
@@ -338,16 +347,16 @@
         """
         return AuthorizedSession(self.creds)
 
 
 @dataclass
 class Metadata:
     _instance = None
-    app_settings_path = Path.home() / ".homebase_calendar_sync"
-    app_metadata_path = Path.home() / ".homebase_calendar_sync_meta"
+    app_settings_path = Path.home() / config.META_SETTINGS_PATH
+    app_metadata_path = Path.home() / config.META_DATA_PATH
     google_client_secret: dict = field(default_factory=dict)
     google_client_token: Credentials | None = None
 
     def __call__(self, **kwargs):
         for key, value in kwargs.items():
             setattr(self, key, value)
         self.write()
@@ -473,7 +482,39 @@
             secrets_json = next(Path.cwd().glob("client_secret*.json"))
         except StopIteration:
             secrets_json = None
 
         if secrets_json:
             self.import_google_client_secret_json(secrets_json)
             secrets_json.unlink()
+
+def import_client_secret(client_secret: bool | str) -> None:
+    config.META = Metadata.metadata_singleton_factory()
+    
+    if isinstance(client_secret, bool):
+        client_secret_path = inquirer.filepath(
+            message="path to 'client_secret.json:'",
+            default=str(next(Path.cwd().glob("client_secret*.json"))),
+            validate=PathValidator(is_file=True, message="input is not a file"),
+            only_files=True,
+        ).execute()
+    else:
+        client_secret_path = client_secret
+
+    config.META.import_google_client_secret_json(client_secret_path)
+    Path(client_secret_path).unlink()
+    config.META(google_client_token=AuthGoogle.initiate_google_oauth_flow(config.API_SCOPES))
+    
+    print("Imported client_secrets.json file.")
+    print(f"...deleted authentication artifacts: {client_secret_path}")
+    raise SystemExit
+
+def reset_auth_cache() -> None:
+    app_settings_path = Path.home() / config.META_SETTINGS_PATH
+    app_metadata_path = Path.home() / config.META_DATA_PATH
+
+    try:
+        app_metadata_path.unlink()
+        app_settings_path.unlink()
+    except FileNotFoundError:
+        print("no auth cache to reset.")
+
```

### Comparing `homebase_calendar_sync-0.1.7/src/homebase_calendar_sync/google_client/google_client.py` & `homebase_calendar_sync-0.1.8/src/homebase_calendar_sync/google_client/google_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,14 +59,23 @@
     def create_new_event(self, calendar_id: str, event_json: str) -> None:
         event_result = (
             self.auth_google.calendar_service.events()
             .insert(calendarId=calendar_id, body=event_json)
             .execute()
         )
         print(f"Event Created: {event_result.get('htmlLink')}")
+        return event_result
+
+    def remove_event(self, calendar_id: str, event_id: str):
+        event_result = (
+            self.auth_google.calendar_service.events()
+            .delete(calendarId=calendar_id, eventId=event_id)
+            .execute()
+        )
+        print(f"Event Removed: {event_id}")
 
     def get_google_drive_folder(self, folder_id: str) -> dict:
         return (
             self.auth_google.drive_service.files()  # pylint: disable=no-member
             .get(fileId=folder_id, fields="id, name")
             .execute()
         )
```

### Comparing `homebase_calendar_sync-0.1.7/src/homebase_calendar_sync.egg-info/SOURCES.txt` & `homebase_calendar_sync-0.1.8/src/homebase_calendar_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `homebase_calendar_sync-0.1.7/src/homebase_calendar_sync.egg-info/requires.txt` & `homebase_calendar_sync-0.1.8/src/homebase_calendar_sync.egg-info/requires.txt`

 * *Files identical despite different names*

