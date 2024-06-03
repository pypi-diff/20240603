# Comparing `tmp/homebase_calendar_sync-0.1.6.tar.gz` & `tmp/homebase_calendar_sync-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homebase_calendar_sync-0.1.6.tar", last modified: Sun Jun  2 17:12:39 2024, max compression
+gzip compressed data, was "homebase_calendar_sync-0.1.7.tar", last modified: Sun Jun  2 17:18:27 2024, max compression
```

## Comparing `homebase_calendar_sync-0.1.6.tar` & `homebase_calendar_sync-0.1.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-02 17:12:39.365757 homebase_calendar_sync-0.1.6/
--rw-r--r--   0 davidmidlo   (501) staff       (20)     2927 2024-06-02 17:12:39.365549 homebase_calendar_sync-0.1.6/PKG-INFO
--rw-r--r--   0 davidmidlo   (501) staff       (20)      477 2024-06-02 14:42:53.000000 homebase_calendar_sync-0.1.6/README.md
--rw-r--r--   0 davidmidlo   (501) staff       (20)       38 2024-06-02 17:12:39.365799 homebase_calendar_sync-0.1.6/setup.cfg
--rw-r--r--   0 davidmidlo   (501) staff       (20)     1009 2024-06-02 17:12:24.000000 homebase_calendar_sync-0.1.6/setup.py
-drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-02 17:12:39.361645 homebase_calendar_sync-0.1.6/src/
-drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-02 17:12:39.362657 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync/
--rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 13:57:29.000000 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync/__init__.py
--rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 13:57:40.000000 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync/__main__.py
--rw-r--r--   0 davidmidlo   (501) staff       (20)      123 2024-06-02 13:40:44.000000 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync/config.py
-drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-02 17:12:39.363832 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync/db/
--rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 14:47:10.000000 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync/db/__init__.py
--rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 14:47:19.000000 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync/db/__main__.py
--rw-r--r--   0 davidmidlo   (501) staff       (20)      872 2024-06-02 15:58:26.000000 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync/db/models.py
-drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-02 17:12:39.364917 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync/google_client/
--rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 14:47:33.000000 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync/google_client/__init__.py
--rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 14:47:49.000000 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync/google_client/__main__.py
--rw-r--r--   0 davidmidlo   (501) staff       (20)    17970 2024-06-02 15:59:07.000000 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync/google_client/auth.py
--rw-r--r--   0 davidmidlo   (501) staff       (20)      106 2024-06-02 04:40:28.000000 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync/google_client/drive_types.py
--rw-r--r--   0 davidmidlo   (501) staff       (20)     9124 2024-06-02 15:59:34.000000 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync/google_client/google_client.py
--rw-r--r--   0 davidmidlo   (501) staff       (20)    13108 2024-06-02 17:11:16.000000 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync/homebase_calendar_sync.py
-drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-02 17:12:39.365211 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync.egg-info/
--rw-r--r--   0 davidmidlo   (501) staff       (20)     2927 2024-06-02 17:12:39.000000 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync.egg-info/PKG-INFO
--rw-r--r--   0 davidmidlo   (501) staff       (20)      881 2024-06-02 17:12:39.000000 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync.egg-info/SOURCES.txt
--rw-r--r--   0 davidmidlo   (501) staff       (20)        1 2024-06-02 17:12:39.000000 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync.egg-info/dependency_links.txt
--rw-r--r--   0 davidmidlo   (501) staff       (20)       94 2024-06-02 17:12:39.000000 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync.egg-info/entry_points.txt
--rw-r--r--   0 davidmidlo   (501) staff       (20)     1080 2024-06-02 17:12:39.000000 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync.egg-info/requires.txt
--rw-r--r--   0 davidmidlo   (501) staff       (20)       23 2024-06-02 17:12:39.000000 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync.egg-info/top_level.txt
+drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-02 17:18:27.828321 homebase_calendar_sync-0.1.7/
+-rw-r--r--   0 davidmidlo   (501) staff       (20)     2927 2024-06-02 17:18:27.828121 homebase_calendar_sync-0.1.7/PKG-INFO
+-rw-r--r--   0 davidmidlo   (501) staff       (20)      477 2024-06-02 14:42:53.000000 homebase_calendar_sync-0.1.7/README.md
+-rw-r--r--   0 davidmidlo   (501) staff       (20)       38 2024-06-02 17:18:27.828371 homebase_calendar_sync-0.1.7/setup.cfg
+-rw-r--r--   0 davidmidlo   (501) staff       (20)     1009 2024-06-02 17:18:19.000000 homebase_calendar_sync-0.1.7/setup.py
+drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-02 17:18:27.823861 homebase_calendar_sync-0.1.7/src/
+drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-02 17:18:27.825070 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync/
+-rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 13:57:29.000000 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync/__init__.py
+-rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 13:57:40.000000 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync/__main__.py
+-rw-r--r--   0 davidmidlo   (501) staff       (20)      123 2024-06-02 13:40:44.000000 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync/config.py
+drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-02 17:18:27.826766 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync/db/
+-rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 14:47:10.000000 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync/db/__init__.py
+-rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 14:47:19.000000 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync/db/__main__.py
+-rw-r--r--   0 davidmidlo   (501) staff       (20)      880 2024-06-02 17:16:23.000000 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync/db/models.py
+drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-02 17:18:27.827568 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync/google_client/
+-rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 14:47:33.000000 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync/google_client/__init__.py
+-rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 14:47:49.000000 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync/google_client/__main__.py
+-rw-r--r--   0 davidmidlo   (501) staff       (20)    17978 2024-06-02 17:17:01.000000 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync/google_client/auth.py
+-rw-r--r--   0 davidmidlo   (501) staff       (20)      106 2024-06-02 04:40:28.000000 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync/google_client/drive_types.py
+-rw-r--r--   0 davidmidlo   (501) staff       (20)     9132 2024-06-02 17:18:10.000000 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync/google_client/google_client.py
+-rw-r--r--   0 davidmidlo   (501) staff       (20)    13118 2024-06-02 17:17:19.000000 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync/homebase_calendar_sync.py
+drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-02 17:18:27.827749 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync.egg-info/
+-rw-r--r--   0 davidmidlo   (501) staff       (20)     2927 2024-06-02 17:18:27.000000 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync.egg-info/PKG-INFO
+-rw-r--r--   0 davidmidlo   (501) staff       (20)      881 2024-06-02 17:18:27.000000 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 davidmidlo   (501) staff       (20)        1 2024-06-02 17:18:27.000000 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 davidmidlo   (501) staff       (20)       94 2024-06-02 17:18:27.000000 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync.egg-info/entry_points.txt
+-rw-r--r--   0 davidmidlo   (501) staff       (20)     1080 2024-06-02 17:18:27.000000 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync.egg-info/requires.txt
+-rw-r--r--   0 davidmidlo   (501) staff       (20)       23 2024-06-02 17:18:27.000000 homebase_calendar_sync-0.1.7/src/homebase_calendar_sync.egg-info/top_level.txt
```

### Comparing `homebase_calendar_sync-0.1.6/PKG-INFO` & `homebase_calendar_sync-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homebase_calendar_sync
-Version: 0.1.6
+Version: 0.1.7
 Summary: A simple web scraper that reads gethomebase.com's schedule and updates Google Calendar.
 Home-page: https://github.com/dmidlo/homebase_calendar_sync
 Author: David Midlo
 Author-email: dmidlo@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `homebase_calendar_sync-0.1.6/setup.py` & `homebase_calendar_sync-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 from setuptools import setup, find_packages
 
 setup(
     name='homebase_calendar_sync',
-    version='0.1.6',
+    version='0.1.7',
     author='David Midlo',
     author_email='dmidlo@gmail.com',
     description='A simple web scraper that reads gethomebase.com\'s schedule and updates Google Calendar.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/dmidlo/homebase_calendar_sync',  # Update this to your project's URL
     packages=find_packages(where='src'),
```

### Comparing `homebase_calendar_sync-0.1.6/src/homebase_calendar_sync/db/models.py` & `homebase_calendar_sync-0.1.7/src/homebase_calendar_sync/db/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import sqlite3
-import config
+from .. import config
 
 
 def connect_database():
     config.DB = sqlite3.connect("events.db")
     config.DB_CURSOR = config.DB.cursor()
```

### Comparing `homebase_calendar_sync-0.1.6/src/homebase_calendar_sync/google_client/auth.py` & `homebase_calendar_sync-0.1.7/src/homebase_calendar_sync/google_client/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 from googleapiclient.discovery import Resource
 from googleapiclient.discovery import build
 
 from cryptography.fernet import Fernet
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
 
-import config
+from .. import config
 
 
 class AuthGoogle:
     """
     A class for managing Google authentication credentials and services.
 
     Args:
```

### Comparing `homebase_calendar_sync-0.1.6/src/homebase_calendar_sync/google_client/google_client.py` & `homebase_calendar_sync-0.1.7/src/homebase_calendar_sync/google_client/google_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 from googleapiclient.errors import HttpError
 
 from .auth import AuthGoogle
 from .drive_types import DriveTypes
 
-import config
+from .. import config
 
 
 # TODO: Should make this a singleton as well.
 #  making this a singleton will allow the None checks for config.GOOGLE to be removed.
 #  presently AuthGoogle is only used here in the client and therefore would be encapsulated
 #  in this singleton and would not need be one itself.
 class GoogleClient:
```

### Comparing `homebase_calendar_sync-0.1.6/src/homebase_calendar_sync/homebase_calendar_sync.py` & `homebase_calendar_sync-0.1.7/src/homebase_calendar_sync/homebase_calendar_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from bs4 import BeautifulSoup
 import pendulum
 from pathlib import Path
 from dotenv import load_dotenv
 from rich import print
 import hashlib
 
-import config
-from db.models import setup_database, connect_database
-from google_client.auth import Metadata
-from google_client.google_client import GoogleClient
+from . import config
+from .db.models import setup_database, connect_database
+from .google_client.auth import Metadata
+from .google_client.google_client import GoogleClient
 
 DOTENV_BASE_DIR = Path.cwd()
 load_dotenv(Path(DOTENV_BASE_DIR, ".env"))
 
 HOMEBASE_USERNAME = os.environ["CC_HOMEBASE_USERNAME"]
 HOMEBASE_PASSWORD = os.environ["CC_HOMEBASE_PASSWORD"]
 EMPLOYEE_FIRSTNAME = os.environ["CC_HOMEBASE_EMPLOYEE_FIRSTNAME"]
```

### Comparing `homebase_calendar_sync-0.1.6/src/homebase_calendar_sync.egg-info/PKG-INFO` & `homebase_calendar_sync-0.1.7/src/homebase_calendar_sync.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homebase_calendar_sync
-Version: 0.1.6
+Version: 0.1.7
 Summary: A simple web scraper that reads gethomebase.com's schedule and updates Google Calendar.
 Home-page: https://github.com/dmidlo/homebase_calendar_sync
 Author: David Midlo
 Author-email: dmidlo@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `homebase_calendar_sync-0.1.6/src/homebase_calendar_sync.egg-info/SOURCES.txt` & `homebase_calendar_sync-0.1.7/src/homebase_calendar_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `homebase_calendar_sync-0.1.6/src/homebase_calendar_sync.egg-info/requires.txt` & `homebase_calendar_sync-0.1.7/src/homebase_calendar_sync.egg-info/requires.txt`

 * *Files identical despite different names*

