# Comparing `tmp/djangoloco-1.0.tar.gz` & `tmp/djangoloco-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangoloco-1.0.tar", last modified: Sun Jul  9 08:57:41 2023, max compression
+gzip compressed data, was "djangoloco-1.1.0.tar", last modified: Mon Jun  3 09:55:44 2024, max compression
```

## Comparing `djangoloco-1.0.tar` & `djangoloco-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:57:41.380066 djangoloco-1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-09 08:57:29.000000 djangoloco-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-09 08:57:29.000000 djangoloco-1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-09 08:57:41.380066 djangoloco-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-09 08:57:29.000000 djangoloco-1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:57:41.376066 djangoloco-1.0/djangoloco/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 08:57:29.000000 djangoloco-1.0/djangoloco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-09 08:57:29.000000 djangoloco-1.0/djangoloco/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-09 08:57:29.000000 djangoloco-1.0/djangoloco/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:57:41.376066 djangoloco-1.0/djangoloco/management/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:57:41.380066 djangoloco-1.0/djangoloco/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-09 08:57:29.000000 djangoloco-1.0/djangoloco/management/commands/loco.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:57:41.380066 djangoloco-1.0/djangoloco/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 08:57:29.000000 djangoloco-1.0/djangoloco/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-09 08:57:29.000000 djangoloco-1.0/djangoloco/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-09 08:57:29.000000 djangoloco-1.0/djangoloco/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-09 08:57:29.000000 djangoloco-1.0/djangoloco/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:57:41.380066 djangoloco-1.0/djangoloco.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-09 08:57:41.000000 djangoloco-1.0/djangoloco.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-09 08:57:41.000000 djangoloco-1.0/djangoloco.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 08:57:41.000000 djangoloco-1.0/djangoloco.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-09 08:57:41.000000 djangoloco-1.0/djangoloco.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-09 08:57:41.000000 djangoloco-1.0/djangoloco.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-09 08:57:29.000000 djangoloco-1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-09 08:57:41.380066 djangoloco-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 08:57:29.000000 djangoloco-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:55:43.995307 djangoloco-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-06-03 09:55:40.000000 djangoloco-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-06-03 09:55:40.000000 djangoloco-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-06-03 09:55:43.995307 djangoloco-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-06-03 09:55:40.000000 djangoloco-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:55:43.991307 djangoloco-1.1.0/djangoloco/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:55:40.000000 djangoloco-1.1.0/djangoloco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-06-03 09:55:40.000000 djangoloco-1.1.0/djangoloco/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-06-03 09:55:40.000000 djangoloco-1.1.0/djangoloco/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:55:43.991307 djangoloco-1.1.0/djangoloco/management/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:55:43.995307 djangoloco-1.1.0/djangoloco/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-06-03 09:55:40.000000 djangoloco-1.1.0/djangoloco/management/commands/loco.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:55:43.995307 djangoloco-1.1.0/djangoloco/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:55:40.000000 djangoloco-1.1.0/djangoloco/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-06-03 09:55:40.000000 djangoloco-1.1.0/djangoloco/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-06-03 09:55:40.000000 djangoloco-1.1.0/djangoloco/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-06-03 09:55:40.000000 djangoloco-1.1.0/djangoloco/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:55:43.995307 djangoloco-1.1.0/djangoloco.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-06-03 09:55:43.000000 djangoloco-1.1.0/djangoloco.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-06-03 09:55:43.000000 djangoloco-1.1.0/djangoloco.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 09:55:43.000000 djangoloco-1.1.0/djangoloco.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-06-03 09:55:43.000000 djangoloco-1.1.0/djangoloco.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-03 09:55:43.000000 djangoloco-1.1.0/djangoloco.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-06-03 09:55:40.000000 djangoloco-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-06-03 09:55:43.995307 djangoloco-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 09:55:40.000000 djangoloco-1.1.0/setup.py
```

### Comparing `djangoloco-1.0/LICENSE` & `djangoloco-1.1.0/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2023, thisfro
+Copyright (c) 2024, thisfro
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `djangoloco-1.0/PKG-INFO` & `djangoloco-1.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangoloco
-Version: 1.0
+Version: 1.1.0
 Summary: A simple management command to get translations from localise.biz (Loco) for your django app.
 Home-page: https://github.com/thisfro/djangoloco
 Author: Jannis Portmann
 Author-email: jannis@thisfro.ch
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Django>=4.0
 
 # djangoloco
 
 A simple management command to get translations from [localise.biz](https://localise.biz/) (Loco) for your django app. It will automatically download all the configured locales.
 
 ## Install
 ```
@@ -38,17 +39,18 @@
     ...
     "djangoloco",
     ...
 ]
 ```
 
 ## Setup
-In your `settings.py`, set the API key from Loco (get it [here](https://localise.biz/help/developers/api-keys))
+In your `settings.py`, set the API key from Loco (get it [here](https://localise.biz/help/developers/api-keys)) and the app that you want to translate
 ```python
 LOCO_API_KEY = ...
+LOCO_APP = "my_app"
 ```
 
 ## Usage
 To pull the translations, run
 ```
 python manage.py loco
 ```
```

### Comparing `djangoloco-1.0/README.md` & `djangoloco-1.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -12,17 +12,18 @@
     ...
     "djangoloco",
     ...
 ]
 ```
 
 ## Setup
-In your `settings.py`, set the API key from Loco (get it [here](https://localise.biz/help/developers/api-keys))
+In your `settings.py`, set the API key from Loco (get it [here](https://localise.biz/help/developers/api-keys)) and the app that you want to translate
 ```python
 LOCO_API_KEY = ...
+LOCO_APP = "my_app"
 ```
 
 ## Usage
 To pull the translations, run
 ```
 python manage.py loco
 ```
```

### Comparing `djangoloco-1.0/djangoloco/management/commands/loco.py` & `djangoloco-1.1.0/djangoloco/management/commands/loco.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 
 from django.core.management.base import BaseCommand
 from django.utils.translation import trans_real
 from django.apps import apps
 from django.conf import settings
 
 LOCO_API_KEY = getattr(settings, 'LOCO_API_KEY', '')
+LOCO_APP = getattr(settings, 'LOCO_APP', '')
 API_URL = ' https://localise.biz/api/export/locale'
 
 
 class Command(BaseCommand):
     help = 'Fetch translations from Loco (Localise.biz) and write them to message files'
 
     def handle(self, *args, **options):
         errors = 0
 
         if LOCO_API_KEY is None or LOCO_API_KEY == '':
             self.stdout.write(self.style.ERROR('An API key is required'))
             return
 
-        app_config = apps.get_app_config('pflaenzli')
+        app_config = apps.get_app_config(LOCO_APP)
         app_path = app_config.path
 
         for locale in trans_real.get_languages():
             url = f'{API_URL}/{locale}.po'
             self.stdout.write(f'Getting translations for locale {self.style.SUCCESS(locale)}')
             response = requests.get(url, auth=(LOCO_API_KEY, ''))
```

### Comparing `djangoloco-1.0/djangoloco.egg-info/PKG-INFO` & `djangoloco-1.1.0/djangoloco.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangoloco
-Version: 1.0
+Version: 1.1.0
 Summary: A simple management command to get translations from localise.biz (Loco) for your django app.
 Home-page: https://github.com/thisfro/djangoloco
 Author: Jannis Portmann
 Author-email: jannis@thisfro.ch
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Django>=4.0
 
 # djangoloco
 
 A simple management command to get translations from [localise.biz](https://localise.biz/) (Loco) for your django app. It will automatically download all the configured locales.
 
 ## Install
 ```
@@ -38,17 +39,18 @@
     ...
     "djangoloco",
     ...
 ]
 ```
 
 ## Setup
-In your `settings.py`, set the API key from Loco (get it [here](https://localise.biz/help/developers/api-keys))
+In your `settings.py`, set the API key from Loco (get it [here](https://localise.biz/help/developers/api-keys)) and the app that you want to translate
 ```python
 LOCO_API_KEY = ...
+LOCO_APP = "my_app"
 ```
 
 ## Usage
 To pull the translations, run
 ```
 python manage.py loco
 ```
```

### Comparing `djangoloco-1.0/setup.cfg` & `djangoloco-1.1.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = djangoloco
-version = 1.0
+version = 1.1.0
 description = A simple management command to get translations from localise.biz (Loco) for your django app.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/thisfro/djangoloco
 author = Jannis Portmann
 author_email = jannis@thisfro.ch
 license = BSD-3-Clause
```

