# Comparing `tmp/django-expanded-test-cases-0.7.0.tar.gz` & `tmp/django_expanded_test_cases-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-expanded-test-cases-0.7.0.tar", last modified: Wed Feb 21 23:28:15 2024, max compression
+gzip compressed data, was "django_expanded_test_cases-0.7.1.tar", last modified: Mon Jun  3 10:36:16 2024, max compression
```

## Comparing `django-expanded-test-cases-0.7.0.tar` & `django_expanded_test_cases-0.7.1.tar`

### file list

```diff
@@ -1,48 +1,51 @@
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2024-02-21 23:28:15.398198 django-expanded-test-cases-0.7.0/
--rw-r--r--   0 brodriguez  (1000) brodriguez  (1000)     1074 2023-05-23 04:12:24.000000 django-expanded-test-cases-0.7.0/LICENSE
--rw-r--r--   0 brodriguez  (1000) brodriguez  (1000)       91 2023-05-23 04:25:19.000000 django-expanded-test-cases-0.7.0/MANIFEST.in
--rw-r--r--   0 brodriguez  (1000) brodriguez  (1000)     5529 2024-02-21 23:28:15.398198 django-expanded-test-cases-0.7.0/PKG-INFO
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2024-02-21 23:28:15.394199 django-expanded-test-cases-0.7.0/django_expanded_test_cases/
--rw-r--r--   0 brodriguez  (1000) brodriguez  (1000)      181 2023-05-23 04:12:47.000000 django-expanded-test-cases-0.7.0/django_expanded_test_cases/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    14281 2024-02-21 21:11:48.000000 django-expanded-test-cases-0.7.0/django_expanded_test_cases/constants.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      901 2023-11-22 05:15:45.000000 django-expanded-test-cases-0.7.0/django_expanded_test_cases/exceptions.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2024-02-21 23:28:15.394199 django-expanded-test-cases-0.7.0/django_expanded_test_cases/mixins/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1612 2023-11-24 17:48:59.000000 django-expanded-test-cases-0.7.0/django_expanded_test_cases/mixins/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    46871 2024-02-21 21:11:48.000000 django-expanded-test-cases-0.7.0/django_expanded_test_cases/mixins/core_mixin.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    31741 2024-02-21 21:11:48.000000 django-expanded-test-cases-0.7.0/django_expanded_test_cases/mixins/live_server_mixin.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    38389 2024-02-21 21:11:48.000000 django-expanded-test-cases-0.7.0/django_expanded_test_cases/mixins/response_mixin.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2024-02-21 23:28:15.394199 django-expanded-test-cases-0.7.0/django_expanded_test_cases/templates/
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2024-02-21 23:28:15.398198 django-expanded-test-cases-0.7.0/django_expanded_test_cases/templates/django_expanded_test_cases/
--rw-r--r--   0 brodriguez  (1000) brodriguez  (1000)      528 2023-05-23 04:25:19.000000 django-expanded-test-cases-0.7.0/django_expanded_test_cases/templates/django_expanded_test_cases/index.html
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2024-02-21 23:28:15.398198 django-expanded-test-cases-0.7.0/django_expanded_test_cases/test_cases/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2493 2023-11-22 05:51:55.000000 django-expanded-test-cases-0.7.0/django_expanded_test_cases/test_cases/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    18648 2023-11-24 17:48:59.000000 django-expanded-test-cases-0.7.0/django_expanded_test_cases/test_cases/base_test_case.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3298 2023-11-22 05:15:45.000000 django-expanded-test-cases-0.7.0/django_expanded_test_cases/test_cases/channels_live_server_test_case.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    69859 2024-02-21 21:11:48.000000 django-expanded-test-cases-0.7.0/django_expanded_test_cases/test_cases/integration_test_case.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3246 2023-11-22 05:15:45.000000 django-expanded-test-cases-0.7.0/django_expanded_test_cases/test_cases/live_server_test_case.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1591 2024-02-21 21:22:58.000000 django-expanded-test-cases-0.7.0/django_expanded_test_cases/test_urls.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2024-02-21 23:28:15.398198 django-expanded-test-cases-0.7.0/django_expanded_test_cases.egg-info/
--rw-r--r--   0 brodriguez  (1000) brodriguez  (1000)     5529 2024-02-21 23:28:15.000000 django-expanded-test-cases-0.7.0/django_expanded_test_cases.egg-info/PKG-INFO
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1462 2024-02-21 23:28:15.000000 django-expanded-test-cases-0.7.0/django_expanded_test_cases.egg-info/SOURCES.txt
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        1 2024-02-21 23:28:15.000000 django-expanded-test-cases-0.7.0/django_expanded_test_cases.egg-info/dependency_links.txt
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      112 2024-02-21 23:28:15.000000 django-expanded-test-cases-0.7.0/django_expanded_test_cases.egg-info/requires.txt
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)       37 2024-02-21 23:28:15.000000 django-expanded-test-cases-0.7.0/django_expanded_test_cases.egg-info/top_level.txt
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2024-02-21 23:28:15.398198 django-expanded-test-cases-0.7.0/etc_tests/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        0 2024-02-21 21:22:58.000000 django-expanded-test-cases-0.7.0/etc_tests/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      202 2024-02-21 21:22:58.000000 django-expanded-test-cases-0.7.0/etc_tests/apps.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      570 2024-02-21 21:22:58.000000 django-expanded-test-cases-0.7.0/etc_tests/asgi.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2024-02-21 23:28:15.398198 django-expanded-test-cases-0.7.0/etc_tests/mock_pages/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        0 2024-02-21 21:12:32.000000 django-expanded-test-cases-0.7.0/etc_tests/mock_pages/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3544 2024-02-21 21:22:58.000000 django-expanded-test-cases-0.7.0/etc_tests/settings.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2024-02-21 23:28:15.398198 django-expanded-test-cases-0.7.0/etc_tests/test_cases/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        0 2024-02-21 21:22:58.000000 django-expanded-test-cases-0.7.0/etc_tests/test_cases/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)   128046 2024-02-21 23:18:53.000000 django-expanded-test-cases-0.7.0/etc_tests/test_cases/test_base_case.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3453 2024-02-21 21:22:58.000000 django-expanded-test-cases-0.7.0/etc_tests/test_cases/test_channels_live_server_case.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)   374159 2024-02-21 21:22:58.000000 django-expanded-test-cases-0.7.0/etc_tests/test_cases/test_integration_case.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3197 2024-02-21 21:22:58.000000 django-expanded-test-cases-0.7.0/etc_tests/test_cases/test_live_server_case.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)   152207 2024-02-21 21:22:58.000000 django-expanded-test-cases-0.7.0/etc_tests/test_cases/universal_live_test_mixin.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      316 2024-02-21 21:22:58.000000 django-expanded-test-cases-0.7.0/etc_tests/urls.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     6141 2024-02-21 21:22:58.000000 django-expanded-test-cases-0.7.0/etc_tests/views.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1849 2024-02-21 23:08:19.000000 django-expanded-test-cases-0.7.0/pyproject.toml
--rw-r--r--   0 brodriguez  (1000) brodriguez  (1000)     2335 2023-05-23 04:25:19.000000 django-expanded-test-cases-0.7.0/readme.md
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1192 2024-02-21 23:28:15.398198 django-expanded-test-cases-0.7.0/setup.cfg
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2024-06-03 10:36:16.433782 django_expanded_test_cases-0.7.1/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1074 2024-06-02 23:06:01.000000 django_expanded_test_cases-0.7.1/LICENSE
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)       91 2024-06-02 23:06:01.000000 django_expanded_test_cases-0.7.1/MANIFEST.in
+-rw-r--r--   0 brodriguez  (1000) brodriguez  (1000)     5529 2024-06-03 10:36:16.433782 django_expanded_test_cases-0.7.1/PKG-INFO
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2024-06-03 10:36:16.429782 django_expanded_test_cases-0.7.1/django_expanded_test_cases/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      181 2024-06-02 23:06:01.000000 django_expanded_test_cases-0.7.1/django_expanded_test_cases/__init__.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2024-06-03 10:36:16.429782 django_expanded_test_cases-0.7.1/django_expanded_test_cases/constants/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2411 2024-06-03 10:22:50.000000 django_expanded_test_cases-0.7.1/django_expanded_test_cases/constants/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     5156 2024-06-03 10:22:50.000000 django_expanded_test_cases-0.7.1/django_expanded_test_cases/constants/auth_constants.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     7407 2024-06-03 10:22:50.000000 django_expanded_test_cases-0.7.1/django_expanded_test_cases/constants/debug_output_constants.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3404 2024-06-03 10:22:50.000000 django_expanded_test_cases-0.7.1/django_expanded_test_cases/constants/general_handling_constants.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3482 2024-06-03 10:22:50.000000 django_expanded_test_cases-0.7.1/django_expanded_test_cases/constants/selenium_constants.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      902 2024-06-03 10:22:50.000000 django_expanded_test_cases-0.7.1/django_expanded_test_cases/exceptions.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2024-06-03 10:36:16.429782 django_expanded_test_cases-0.7.1/django_expanded_test_cases/mixins/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1611 2024-06-03 10:22:50.000000 django_expanded_test_cases-0.7.1/django_expanded_test_cases/mixins/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    47510 2024-06-03 10:22:50.000000 django_expanded_test_cases-0.7.1/django_expanded_test_cases/mixins/core_mixin.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    31851 2024-06-03 10:22:50.000000 django_expanded_test_cases-0.7.1/django_expanded_test_cases/mixins/live_server_mixin.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    41652 2024-06-03 10:22:50.000000 django_expanded_test_cases-0.7.1/django_expanded_test_cases/mixins/response_mixin.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2024-06-03 10:36:16.425782 django_expanded_test_cases-0.7.1/django_expanded_test_cases/templates/
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2024-06-03 10:36:16.429782 django_expanded_test_cases-0.7.1/django_expanded_test_cases/templates/django_expanded_test_cases/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      528 2024-06-02 23:06:01.000000 django_expanded_test_cases-0.7.1/django_expanded_test_cases/templates/django_expanded_test_cases/index.html
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2024-06-03 10:36:16.429782 django_expanded_test_cases-0.7.1/django_expanded_test_cases/test_cases/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2495 2024-06-03 10:22:50.000000 django_expanded_test_cases-0.7.1/django_expanded_test_cases/test_cases/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    19365 2024-06-03 10:22:50.000000 django_expanded_test_cases-0.7.1/django_expanded_test_cases/test_cases/base_test_case.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3298 2024-06-02 23:06:01.000000 django_expanded_test_cases-0.7.1/django_expanded_test_cases/test_cases/channels_live_server_test_case.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    76362 2024-06-03 10:22:50.000000 django_expanded_test_cases-0.7.1/django_expanded_test_cases/test_cases/integration_test_case.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3246 2024-06-02 23:06:01.000000 django_expanded_test_cases-0.7.1/django_expanded_test_cases/test_cases/live_server_test_case.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1649 2024-06-03 10:22:50.000000 django_expanded_test_cases-0.7.1/django_expanded_test_cases/test_urls.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2024-06-03 10:36:16.433782 django_expanded_test_cases-0.7.1/django_expanded_test_cases.egg-info/
+-rw-r--r--   0 brodriguez  (1000) brodriguez  (1000)     5529 2024-06-03 10:36:16.000000 django_expanded_test_cases-0.7.1/django_expanded_test_cases.egg-info/PKG-INFO
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1682 2024-06-03 10:36:16.000000 django_expanded_test_cases-0.7.1/django_expanded_test_cases.egg-info/SOURCES.txt
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        1 2024-06-03 10:36:16.000000 django_expanded_test_cases-0.7.1/django_expanded_test_cases.egg-info/dependency_links.txt
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      112 2024-06-03 10:36:16.000000 django_expanded_test_cases-0.7.1/django_expanded_test_cases.egg-info/requires.txt
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)       37 2024-06-03 10:36:16.000000 django_expanded_test_cases-0.7.1/django_expanded_test_cases.egg-info/top_level.txt
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2024-06-03 10:36:16.429782 django_expanded_test_cases-0.7.1/etc_tests/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        0 2024-06-02 23:06:01.000000 django_expanded_test_cases-0.7.1/etc_tests/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      202 2024-06-02 23:06:01.000000 django_expanded_test_cases-0.7.1/etc_tests/apps.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      592 2024-06-03 10:22:50.000000 django_expanded_test_cases-0.7.1/etc_tests/asgi.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3543 2024-06-03 10:22:50.000000 django_expanded_test_cases-0.7.1/etc_tests/settings.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2024-06-03 10:36:16.429782 django_expanded_test_cases-0.7.1/etc_tests/test_cases/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        0 2024-06-02 23:06:01.000000 django_expanded_test_cases-0.7.1/etc_tests/test_cases/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)   137917 2024-06-03 10:22:50.000000 django_expanded_test_cases-0.7.1/etc_tests/test_cases/test_base_case.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3453 2024-06-02 23:06:01.000000 django_expanded_test_cases-0.7.1/etc_tests/test_cases/test_channels_live_server_case.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)   446822 2024-06-03 10:22:50.000000 django_expanded_test_cases-0.7.1/etc_tests/test_cases/test_integration_case.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3197 2024-06-02 23:06:01.000000 django_expanded_test_cases-0.7.1/etc_tests/test_cases/test_live_server_case.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)   152209 2024-06-03 10:22:50.000000 django_expanded_test_cases-0.7.1/etc_tests/test_cases/universal_live_test_mixin.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      316 2024-06-02 23:06:01.000000 django_expanded_test_cases-0.7.1/etc_tests/urls.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     6591 2024-06-03 10:22:50.000000 django_expanded_test_cases-0.7.1/etc_tests/views.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1912 2024-06-03 10:30:29.000000 django_expanded_test_cases-0.7.1/pyproject.toml
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2335 2024-06-02 23:06:01.000000 django_expanded_test_cases-0.7.1/readme.md
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1192 2024-06-03 10:36:16.433782 django_expanded_test_cases-0.7.1/setup.cfg
```

### Comparing `django-expanded-test-cases-0.7.0/LICENSE` & `django_expanded_test_cases-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.7.0/PKG-INFO` & `django_expanded_test_cases-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-expanded-test-cases
-Version: 0.7.0
+Version: 0.7.1
 Summary: Expands the existing Django TestCase class with extra functionality.
 Home-page: https://github.com/brodriguez8774/django-expanded-test-cases
 Author: Brandon Rodriguez
 Author-email: Brandon Rodriguez <brodriguez8774@gmail.com>
 Maintainer-email: Brandon Rodriguez <brodriguez8774@gmail.com>
 License: MIT License
```

### Comparing `django-expanded-test-cases-0.7.0/django_expanded_test_cases/exceptions.py` & `django_expanded_test_cases-0.7.1/django_expanded_test_cases/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 
 class ExpandedTestCasesBaseException(ABC, Exception):
     """General customized exception for ETC project.
 
     Holds boilerplate logic and should NOT be directly called.
     """
+
     def __init__(self, value):
         # Ensure expected type for exception message.
         if value is None:
             value = ''
         self.value = str(value).strip()
 
         # Populate to default value if not provided.
```

### Comparing `django-expanded-test-cases-0.7.0/django_expanded_test_cases/mixins/__init__.py` & `django_expanded_test_cases-0.7.1/django_expanded_test_cases/mixins/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,25 +19,26 @@
 try:
     from .live_server_mixin import LiveServerMixin
 except ModuleNotFoundError:
     # Project likely does not have selenium package installed.
     # This is okay, as we don't want this logic as a hard requirement to use this library.
 
     # However, we do want to define a dummy class to give feedback errors.
-    class LiveServerTestCase():
+    class LiveServerTestCase:
         err_msg = """
         Cannot use LiveServer TestCases class without "selenium" package installed.
         To use these TestCases, add the following packages to your project:
             * selenium              # Required
             * channels              # Optional, used in ChannelsLiveServerTestCase only.
             * daphne                # Optional, used in ChannelsLiveServerTestCase only.
 
         For more information, see:
         https://www.selenium.dev/documentation/webdriver/getting_started/
         """
+
         @classmethod
         def setUpClass(cls):
             raise Exception(cls.err_msg)
 
         def setUp(self):
             raise Exception(self.err_msg)
```

### Comparing `django-expanded-test-cases-0.7.0/django_expanded_test_cases/mixins/core_mixin.py` & `django_expanded_test_cases-0.7.1/django_expanded_test_cases/mixins/core_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,40 +30,45 @@
     ETC_OUTPUT_EXPECTED_MATCH_COLOR,
     ETC_OUTPUT_RESET_COLOR,
 )
 
 
 # region Debug Print Wrapper Logic
 
+
 def wrapper(method):
     """Wrapper logic to intercept all functions on AssertionError and print error at bottom of output."""
+
     @wraps(method)
     def wrapped(*args, **kwargs):
         try:
             return method(*args, **kwargs)
         except AssertionError as err:
             if ETC_DEBUG_PRINT:
                 print('\n')
                 print('{0}{1}{2}'.format(ETC_OUTPUT_ERROR_COLOR, err, ETC_OUTPUT_RESET_COLOR))
                 print('')
             raise err
+
     return wrapped
 
 
 class DebugPrintMetaClass(type):
     """Courtesy of https://stackoverflow.com/a/11350487"""
+
     def __new__(meta, classname, bases, classDict):
         newClassDict = {}
         for attributeName, attribute in classDict.items():
             if isinstance(attribute, FunctionType):
                 # Replace function with a DebugPrint-wrapped version.
                 attribute = wrapper(attribute)
             newClassDict[attributeName] = attribute
         return type.__new__(meta, classname, bases, newClassDict)
 
+
 # endregion Debug Print Wrapper Logic
 
 
 class BaseMixin:
     """Base mixin that all other project classes should inherit from in some way.
 
     Basically only exists to guarantee certain expected functions exist during inheritance chain, unconditionally.
@@ -174,16 +179,15 @@
                     'The extra_usergen_kwargs value must be a dictionary of additional args used in the '
                     'get_user_model().objects.create_user() function.'
                 )
 
             cls._auto_generate_test_users(extra_usergen_kwargs=extra_usergen_kwargs)
 
     def subTest(self, *args, **kwargs):
-        """Test logic setup run every time we enter a subtest.
-        """
+        """Test logic setup run every time we enter a subtest."""
 
         # Call parent logic.
         super().subTest(*args, **kwargs)
 
         # Reset display error, in case multiple subtests run and fail in a given test.
         self._error_displayed = False
 
@@ -408,30 +412,38 @@
                         total_actual_index = total_actual_count_thus_far
                     else:
                         # Is negative, so endsWith(). Count from end of text.
                         total_actual_index = actual_text_total_len - total_actual_count_thus_far
 
                 if curr_expected_line == curr_actual_line:
                     # Line is full match and correct.
-                    curr_expected_line = '{0}{1}{2}\n'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, curr_expected_line, ETC_OUTPUT_RESET_COLOR)
-                    curr_actual_line = '{0}{1}{2}\n'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, curr_actual_line, ETC_OUTPUT_RESET_COLOR)
+                    curr_expected_line = '{output_color}{line_output}{reset_color}\n'.format(
+                        output_color=ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                        line_output=curr_expected_line,
+                        reset_color=ETC_OUTPUT_RESET_COLOR,
+                    )
+                    curr_actual_line = '{output_color}{line_output}{reset_color}\n'.format(
+                        output_color=ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                        line_output=curr_actual_line,
+                        reset_color=ETC_OUTPUT_RESET_COLOR,
+                    )
                 elif curr_expected_line is None:
                     # "Actual" output is longer than "expected" output. Impossible to match current line.
                     curr_expected_line = ''
-                    curr_actual_line = '{0}{1}{2}\n'.format(
-                        ETC_OUTPUT_ACTUALS_ERROR_COLOR,
-                        curr_actual_line,
-                        ETC_OUTPUT_RESET_COLOR,
+                    curr_actual_line = '{output_color}{line_output}{reset_color}\n'.format(
+                        output_color=ETC_OUTPUT_ACTUALS_ERROR_COLOR,
+                        line_output=curr_actual_line,
+                        reset_color=ETC_OUTPUT_RESET_COLOR,
                     )
                 elif curr_actual_line is None:
                     # "Expected" output is longer than "actual" output. Impossible to match current line.
-                    curr_expected_line = '{0}{1}{2}\n'.format(
-                        ETC_OUTPUT_EXPECTED_ERROR_COLOR,
-                        curr_expected_line,
-                        ETC_OUTPUT_RESET_COLOR,
+                    curr_expected_line = '{output_color}{line_output}{reset_color}\n'.format(
+                        output_color=ETC_OUTPUT_EXPECTED_ERROR_COLOR,
+                        line_output=curr_expected_line,
+                        reset_color=ETC_OUTPUT_RESET_COLOR,
                     )
                     curr_actual_line = ''
                 else:
                     # Both lines are populated but do not match.
                     # Determine which one is longer.
                     if len(curr_actual_line) > len(curr_expected_line):
                         max_chars = len(curr_actual_line)
@@ -456,15 +468,15 @@
                                 if total_actual_index > compare_index:
                                     do_char_compare = False
                             else:
                                 # Is negative, so endsWith().
                                 total_actual_index -= 1
 
                                 # Skip comparison if actual_index is before compare_index.
-                                if total_actual_index > - compare_index:
+                                if total_actual_index > -compare_index:
                                     do_char_compare = False
 
                         # Grab current character.
                         try:
                             expected_char = curr_expected_line[char_index]
                         except IndexError:
                             expected_char = ''
@@ -765,17 +777,17 @@
         # If kwargs were provided, trim final slash if url ends with such.
         # Makes sure handling is consistent, even if ordering of ? and / are weird.
         while url.endswith('/'):
             url = url[:-1]
 
         # Finally, generate actual url and return.
         get_params = urlencode(kwargs)
-        get_url = '{0}/{1}'.format(
-            url,
-            ('' if get_params == '' else '?' + get_params)
+        get_url = '{url}/{params}'.format(
+            url=url,
+            params=('' if get_params == '' else '?' + get_params),
         )
 
         self._debug_print('URL: {0}'.format(get_url))
         return get_url
 
     def standardize_characters(self, value):
         """Standardizes various characters in provided str.
@@ -1014,21 +1026,26 @@
 
     # region Properties
 
     @property
     def site_root_url(self):
         """"""
         if (
+            # No url defined.
             self._site_root_url is None
+            # Url is empty.
             or self._site_root_url == ''
         ):
             # No site root populated. Check for "live_server_url", which is auto-populated for Selenium tests.
             if (
+                # Has attribute.
                 hasattr(self, 'live_server_url')
+                # Attribute populated.
                 and self.live_server_url is not None
+                # And non-empty.
                 and self.live_server_url != ''
             ):
                 return self.live_server_url
 
             # Failed to get auto-populated Selenium url.
             # Return default (will apply in most cases).
             return '127.0.0.1'
```

### Comparing `django-expanded-test-cases-0.7.0/django_expanded_test_cases/mixins/live_server_mixin.py` & `django_expanded_test_cases-0.7.1/django_expanded_test_cases/mixins/live_server_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,19 +12,20 @@
 # Third-Party Imports.
 from selenium import webdriver
 from selenium.webdriver.chrome.service import Service as ChromeService
 from selenium.webdriver.firefox.service import Service as FireFoxService
 
 # Internal Imports.
 from django_expanded_test_cases.constants import (
+    # Output settings.
     ETC_INCLUDE_RESPONSE_DEBUG_URL,
     ETC_INCLUDE_RESPONSE_DEBUG_CONTENT,
     ETC_RESPONSE_DEBUG_CONTENT_COLOR,
     ETC_OUTPUT_EMPHASIS_COLOR,
-
+    # Selenium handling settings.
     ETC_SELENIUM_BROWSER,
     ETC_SELENIUM_HEADLESS,
     ETC_SELENIUM_DISABLE_CACHE,
     ETC_SELENIUM_DEBUG_PORT_START_VALUE,
     ETC_SELENIUM_WINDOW_POSITIONS,
     ETC_SELENIUM_EXTRA_BROWSER_OPTIONS,
     ETC_SELENIUM_PAGE_TIMEOUT_DEFAULT,
@@ -40,14 +41,15 @@
 # Using the same port seems to cause issues with allowing proper switching between drivers.
 # Each generated driver increments this value by one, to guarantee all tests among all files should have unique ports.
 SELENIUM_DEBUG_PORT = ETC_SELENIUM_DEBUG_PORT_START_VALUE
 
 
 class LiveServerMixin(ResponseTestCaseMixin):
     """Universal logic for all selenium LiveServer test cases."""
+
     @classmethod
     def setUpClass(cls, *args, initial_driver_count=1, debug_print=None, **kwargs):
         """Test logic setup run at the start of class creation.
 
         :param initial_driver_count: Number of drivers to generate at the start of test class creation.
                                      Defaults to 1. Set to 0 to skip creating drivers at class level.
         :param debug_print: Optional bool that indicates if debug output should print to console.
@@ -375,18 +377,18 @@
         :param window_index: Index of window to switch to.
         :return: New focus window.
         """
         # Attempt to get window at specified driver index.
         try:
             focus_window = driver.window_handles[window_index]
         except IndexError:
-            err_msg = 'Attempted to switch to window of index "{0}", but driver only has {1} windows open.'.format(
-                window_index,
-                len(driver.window_handles)
-            )
+            err_msg = (
+                'Attempted to switch to window of index "{window_index}", '
+                'but driver only has {window_count} windows open.'
+            ).format(window_index=window_index, window_count=len(driver.window_handles))
             raise IndexError(err_msg)
 
         # Switch window to be focused.
         driver.switch_to.window(focus_window)
 
         # Return newly switched window.
         return focus_window
```

### Comparing `django-expanded-test-cases-0.7.0/django_expanded_test_cases/mixins/response_mixin.py` & `django_expanded_test_cases-0.7.1/django_expanded_test_cases/mixins/response_mixin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,46 @@
 """
 Core testing logic that pertains to handling Response objects.
 """
 
 # System Imports.
+import warnings
 import logging, re
 from urllib.parse import parse_qs
 
 # Third-Party Imports.
 from bs4 import BeautifulSoup
 from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.http.response import HttpResponseBase
 
 # Internal Imports.
 from . import CoreTestCaseMixin
 from django.urls import reverse
 from django.urls.exceptions import NoReverseMatch
 from django_expanded_test_cases.constants import (
+    ETC_DEBUG_PRINT__RESPONSE_SEPARATOR,
+    ETC_DEBUG_PRINT__SKIP_DISPLAY,
+    ETC_INCLUDE_RESPONSE_DEBUG_CONTENT,
+    ETC_INCLUDE_RESPONSE_DEBUG_CONTEXT,
+    ETC_INCLUDE_RESPONSE_DEBUG_FORMS,
+    ETC_INCLUDE_RESPONSE_DEBUG_HEADER,
+    ETC_INCLUDE_RESPONSE_DEBUG_MESSAGES,
+    ETC_INCLUDE_RESPONSE_DEBUG_SESSION,
+    ETC_INCLUDE_RESPONSE_DEBUG_USER_INFO,
+    ETC_OUTPUT_EMPHASIS_COLOR,
     ETC_OUTPUT_ERROR_COLOR,
     ETC_RESPONSE_DEBUG_CONTENT_COLOR,
-    ETC_RESPONSE_DEBUG_HEADER_COLOR,
     ETC_RESPONSE_DEBUG_CONTEXT_COLOR,
+    ETC_RESPONSE_DEBUG_FORM_COLOR,
+    ETC_RESPONSE_DEBUG_HEADER_COLOR,
+    ETC_RESPONSE_DEBUG_USER_INFO_COLOR,
     ETC_RESPONSE_DEBUG_MESSAGE_COLOR,
     ETC_RESPONSE_DEBUG_SESSION_COLOR,
     ETC_RESPONSE_DEBUG_URL_COLOR,
-    ETC_RESPONSE_DEBUG_FORM_COLOR,
-    ETC_RESPONSE_DEBUG_USER_INFO_COLOR,
-    ETC_OUTPUT_EMPHASIS_COLOR,
-    ETC_AUTO_GENERATE_USERS,
-    ETC_DEBUG_PRINT__SKIP_DISPLAY
 )
 
 
 # Initialize logging.
 logger = logging.getLogger(__name__)
 
 
@@ -47,25 +55,59 @@
                             Param overrides setting value if both param and setting are set.
         """
         # Run parent setup logic.
         super().setUpClass(*args, debug_print=debug_print, **kwargs)
 
     # region Debug Output Functions
 
+    def full_debug_print(self, response):
+        """Attempts to display debug output for all of response data."""
+
+        if ETC_INCLUDE_RESPONSE_DEBUG_CONTENT:
+            self.show_debug_content(response)
+        if ETC_INCLUDE_RESPONSE_DEBUG_HEADER:
+            self.show_debug_headers(response)
+        if ETC_INCLUDE_RESPONSE_DEBUG_CONTEXT:
+            self.show_debug_context(response)
+        if ETC_INCLUDE_RESPONSE_DEBUG_SESSION:
+            self.show_debug_session_data(response)
+        if ETC_INCLUDE_RESPONSE_DEBUG_MESSAGES:
+            self.show_debug_messages(response)
+        if ETC_INCLUDE_RESPONSE_DEBUG_FORMS:
+            self.show_debug_form_data(response)
+        if ETC_INCLUDE_RESPONSE_DEBUG_USER_INFO:
+            self.show_debug_user_info(response)
+
+        # Optionally display custom debug-output separators for additional end-of-assertion clarity.
+        if len(ETC_DEBUG_PRINT__RESPONSE_SEPARATOR) > 0:
+            self._debug_print(ETC_DEBUG_PRINT__RESPONSE_SEPARATOR)
+
     def show_debug_url(self, url):
         """Prints debug url output."""
 
         # Ensure url is in consistent format.
         url = self.standardize_url(url, append_root=True)
         message = 'Attempting to access url "{0}"'.format(url)
 
         self._debug_print('\n\n')
-        self._debug_print('{0}'.format('-' * len(message)), fore=ETC_RESPONSE_DEBUG_URL_COLOR, style=ETC_OUTPUT_EMPHASIS_COLOR)
-        self._debug_print(message, fore=ETC_RESPONSE_DEBUG_URL_COLOR, style=ETC_OUTPUT_EMPHASIS_COLOR)
-        self._debug_print('{0}'.format('-' * len(message)), fore=ETC_RESPONSE_DEBUG_URL_COLOR, style=ETC_OUTPUT_EMPHASIS_COLOR)
+        self._debug_print(
+            '{0}'.format('-' * len(message)),
+            fore=ETC_RESPONSE_DEBUG_URL_COLOR,
+            style=ETC_OUTPUT_EMPHASIS_COLOR,
+        )
+        self._debug_print(
+            message,
+            fore=ETC_RESPONSE_DEBUG_URL_COLOR,
+            style=ETC_OUTPUT_EMPHASIS_COLOR,
+        )
+        self._debug_print(
+            '{0}'.format('-' * len(message)),
+            fore=ETC_RESPONSE_DEBUG_URL_COLOR,
+            style=ETC_OUTPUT_EMPHASIS_COLOR,
+        )
 
     def show_debug_content(self, response_content):
         """Prints debug response page output."""
 
         # Handle for potential param types.
         if isinstance(response_content, HttpResponseBase):
             response_content = response_content.content.decode('utf-8')
@@ -120,25 +162,31 @@
             fore=ETC_RESPONSE_DEBUG_HEADER_COLOR,
             style=ETC_OUTPUT_EMPHASIS_COLOR,
         )
 
         # Print out data, if present.
         if response_headers is not None and len(response_headers) > 0:
             for key, value in response_headers.items():
-                self._debug_print('    * "{0}": "{1}"'.format(key, value), fore=ETC_RESPONSE_DEBUG_HEADER_COLOR)
+                self._debug_print(
+                    '    * "{0}": "{1}"'.format(key, value),
+                    fore=ETC_RESPONSE_DEBUG_HEADER_COLOR,
+                )
         else:
             self._debug_print('    No response headers found.')
         self._debug_print()
 
     def show_debug_context(self, response_context):
         """Prints debug response context data."""
 
         # Handle for potential param types.
         if isinstance(response_context, HttpResponseBase):
-            response_context = response_context.context or {}
+            if hasattr(response_context, 'context'):
+                response_context = response_context.context or {}
+            else:
+                response_context = {}
 
         if response_context is not None:
             # Attempt to access key object. If fails, attempt to generate dict of values.
             try:
                 response_context.keys()
 
             except AttributeError:
@@ -155,14 +203,15 @@
             except Exception as err:
                 # Error occurred.
                 # Check if error is due to ContextDict/ContextList object being passed.
                 # Unsure why this happens, but seems to occur in tests that access Django 4.2.7 admin views?
                 # Needs further research. For now, this seems like enough to bypass it
                 # and have no immediately noticeable side effects.
                 from django.test.utils import ContextList
+
                 if isinstance(response_context, ContextList):
                     # Skip output.
                     return
 
                 else:
                     # Raise original error.
                     raise err
@@ -173,31 +222,43 @@
             fore=ETC_RESPONSE_DEBUG_CONTEXT_COLOR,
             style=ETC_OUTPUT_EMPHASIS_COLOR,
         )
 
         # NOTE: Response context object is strange, in that it's basically a dictionary,
         # and it allows .keys() but not .values(). Thus, iterate on keys only and pull respective value.
         if response_context is not None and len(response_context.keys()) > 0:
-            # pass
-            for key in response_context.keys():
-                context_value = str(response_context.get(key))
-                # Truncate display if very long.
-                if len(context_value) > 80:
-                    context_value = '"{0}"..."{1}"'.format(context_value[:40], context_value[-40:])
-                self._debug_print('    * {0}: {1}'.format(key, context_value), fore=ETC_RESPONSE_DEBUG_CONTEXT_COLOR)
+
+            # Fix for
+            # RemovedInDjango50Warning: The "default.html" templates for forms and formsets will be removed.
+            # Warning, prior to Django 5.0. Seems to trigger due to ETC accessing context in an "unexpected" way.
+            with warnings.catch_warnings(action="ignore"):
+
+                # Iterate through context values.
+                for key in response_context.keys():
+                    context_value = str(response_context.get(key))
+                    # Truncate display if very long.
+                    if len(context_value) > 80:
+                        context_value = '"{0}"..."{1}"'.format(context_value[:40], context_value[-40:])
+                    self._debug_print(
+                        '    * {0}: {1}'.format(key, context_value),
+                        fore=ETC_RESPONSE_DEBUG_CONTEXT_COLOR,
+                    )
         else:
             self._debug_print('    No context data found.', fore=ETC_RESPONSE_DEBUG_CONTEXT_COLOR)
         self._debug_print()
 
     def show_debug_session_data(self, client):
         """Prints debug response session data."""
 
         # Handle for potential param types.
         if isinstance(client, HttpResponseBase):
-            client = client.client
+            if hasattr(client, 'client'):
+                client = client.client
+            else:
+                client = None
 
         self._debug_print()
         self._debug_print(
             '{0} {1} {0}'.format('=' * 10, 'client.session'),
             fore=ETC_RESPONSE_DEBUG_SESSION_COLOR,
             style=ETC_OUTPUT_EMPHASIS_COLOR,
         )
@@ -210,15 +271,18 @@
         self._debug_print()
 
     def show_debug_messages(self, response_context):
         """Prints debug response message data."""
 
         # Handle for potential param types.
         if isinstance(response_context, HttpResponseBase):
-            response_context = response_context.context
+            if hasattr(response_context, 'context'):
+                response_context = response_context.context or {}
+            else:
+                response_context = {}
 
         self._debug_print()
         self._debug_print(
             '{0} {1} {0}'.format('=' * 10, 'response.context["messages"]'),
             fore=ETC_RESPONSE_DEBUG_MESSAGE_COLOR,
             style=ETC_OUTPUT_EMPHASIS_COLOR,
         )
@@ -236,15 +300,18 @@
         self._debug_print()
 
     def show_debug_form_data(self, response_context):
         """Prints debug response form data."""
 
         # Handle for potential param types.
         if isinstance(response_context, HttpResponseBase):
-            response_context = response_context.context
+            if hasattr(response_context, 'context'):
+                response_context = response_context.context or {}
+            else:
+                response_context = {}
 
         self._debug_print()
         self._debug_print(
             '{0} {1} {0}'.format('=' * 10, 'Form Data'),
             fore=ETC_RESPONSE_DEBUG_FORM_COLOR,
             style=ETC_OUTPUT_EMPHASIS_COLOR,
         )
@@ -259,33 +326,44 @@
                 form_present = True
                 form = response_context['form']
 
                 # Print general form data.
                 self._debug_print('    Provided Form Fields:', fore=ETC_RESPONSE_DEBUG_FORM_COLOR)
                 fields_submitted = False
                 for key, value in form.data.items():
-                    self._debug_print('        {0}: {1}'.format(key, value), fore=ETC_RESPONSE_DEBUG_FORM_COLOR)
+                    self._debug_print(
+                        '        {0}: {1}'.format(key, value),
+                        fore=ETC_RESPONSE_DEBUG_FORM_COLOR,
+                    )
                     fields_submitted = True
                 if not fields_submitted:
                     self._debug_print('        No form field data submitted.', fore=ETC_RESPONSE_DEBUG_FORM_COLOR)
 
                 # Print form data errors if present.
                 if not form.is_valid():
                     self._debug_print()
                     if len(form.errors) > 0 or len(form.non_field_errors()) > 0:
-                        self._debug_print('    Form Invalid:'.format(not form.is_valid()), fore=ETC_RESPONSE_DEBUG_FORM_COLOR)
+                        self._debug_print(
+                            '    Form Invalid:'.format(not form.is_valid()), fore=ETC_RESPONSE_DEBUG_FORM_COLOR
+                        )
                         if len(form.non_field_errors()) > 0:
                             self._debug_print('        Non-field Frrors:', fore=ETC_RESPONSE_DEBUG_FORM_COLOR)
                             for error in form.non_field_errors():
-                                self._debug_print('            {0}'.format(error), fore=ETC_RESPONSE_DEBUG_FORM_COLOR)
+                                self._debug_print(
+                                    '            {0}'.format(error),
+                                    fore=ETC_RESPONSE_DEBUG_FORM_COLOR,
+                                )
 
                         if len(form.errors) > 0:
                             self._debug_print('        Field Errors:', fore=ETC_RESPONSE_DEBUG_FORM_COLOR)
                             for error in form.errors:
-                                self._debug_print('            {0}'.format(error), fore=ETC_RESPONSE_DEBUG_FORM_COLOR)
+                                self._debug_print(
+                                    '            {0}'.format(error),
+                                    fore=ETC_RESPONSE_DEBUG_FORM_COLOR,
+                                )
 
                 else:
                     self._debug_print('    Form found and valid.', fore=ETC_RESPONSE_DEBUG_FORM_COLOR)
 
             # Attempt to get formset data.
             if 'formset' in response_context:
                 if form_present:
@@ -306,56 +384,76 @@
 
     def show_debug_user_info(self, user):
         """Prints debug user data."""
 
         # Imported here to prevent potential "Apps aren't loaded yet" error.
         from django.contrib.auth.models import AnonymousUser
 
+        # Handle for potential param types.
+        if isinstance(user, HttpResponseBase):
+            if hasattr(user, 'user'):
+                user = user.user
+            else:
+                user = None
+
         self._debug_print()
         self._debug_print(
             '{0} {1} {0}'.format('=' * 10, 'User Info'),
             fore=ETC_RESPONSE_DEBUG_USER_INFO_COLOR,
             style=ETC_OUTPUT_EMPHASIS_COLOR,
         )
 
         # Only proceed if we got a proper user model.
         if isinstance(user, get_user_model()):
 
             # General user information.
             self._debug_print('    * pk: "{0}"'.format(user.pk), fore=ETC_RESPONSE_DEBUG_USER_INFO_COLOR)
-            self._debug_print('    * Username: "{0}"'.format(user.username), fore=ETC_RESPONSE_DEBUG_USER_INFO_COLOR)
-            self._debug_print('    * First: "{0}"'.format(user.first_name), fore=ETC_RESPONSE_DEBUG_USER_INFO_COLOR)
+            self._debug_print(
+                '    * Username: "{0}"'.format(user.username),
+                fore=ETC_RESPONSE_DEBUG_USER_INFO_COLOR,
+            )
+            self._debug_print(
+                '    * First: "{0}"'.format(user.first_name),
+                fore=ETC_RESPONSE_DEBUG_USER_INFO_COLOR,
+            )
             self._debug_print('    * Last: "{0}"'.format(user.last_name), fore=ETC_RESPONSE_DEBUG_USER_INFO_COLOR)
             self._debug_print('    * Email: "{0}"'.format(user.email), fore=ETC_RESPONSE_DEBUG_USER_INFO_COLOR)
 
             # User auth data.
             self._debug_print(
                 '    * is_authenticated: {0}'.format(user.is_authenticated),
                 fore=ETC_RESPONSE_DEBUG_USER_INFO_COLOR,
             )
 
             # User groups.
-            self._debug_print('    * User Groups: {0}'.format(user.groups.all()), fore=ETC_RESPONSE_DEBUG_USER_INFO_COLOR)
+            self._debug_print(
+                '    * User Groups: {0}'.format(user.groups.all()), fore=ETC_RESPONSE_DEBUG_USER_INFO_COLOR
+            )
 
             # User permissions.
             self._debug_print(
                 '    * User Permissions: {0}'.format(user.user_permissions.all()),
                 fore=ETC_RESPONSE_DEBUG_USER_INFO_COLOR,
             )
 
         elif isinstance(user, AnonymousUser):
-
             self._debug_print('    Anonymous user. No user is logged in.', fore=ETC_RESPONSE_DEBUG_USER_INFO_COLOR)
 
+        elif user is None:
+            self._debug_print('    User not defined. Was None type.', fore=ETC_RESPONSE_DEBUG_USER_INFO_COLOR)
+
         else:
-            self._debug_print('    * Invalid user "{0}" of type "{1}". Expected "{2}".'.format(
-                user,
-                type(user),
-                type(get_user_model()),
-            ), fore=ETC_OUTPUT_ERROR_COLOR)
+            self._debug_print(
+                '    * Invalid user "{0}" of type "{1}". Expected "{2}".'.format(
+                    user,
+                    type(user),
+                    type(get_user_model()),
+                ),
+                fore=ETC_OUTPUT_ERROR_COLOR,
+            )
         self._debug_print()
         self._debug_print()
 
     # endregion Debug Output Functions.
 
     def standardize_url(self, url, url_args=None, url_kwargs=None, url_query_params=None, append_root=True):
         """Attempts to standardize URL value, such as in event url is in format for reverse() function.
@@ -564,15 +662,15 @@
         element_list = self.find_elements_by_tag(content, element)
 
         # Verify only one value was found.
         if len(element_list) > 1:
             self.fail(
                 f'Found multiple instances of "<{element}>" element. Expected only one instance. '
                 f'Content was:\n{content}'
-             )
+            )
 
         # Return found item.
         return element_list[0]
 
     def find_elements_by_id(self, content, element_id):
         """Finds all HTML elements that match the provided id.
```

### Comparing `django-expanded-test-cases-0.7.0/django_expanded_test_cases/templates/django_expanded_test_cases/index.html` & `django_expanded_test_cases-0.7.1/django_expanded_test_cases/templates/django_expanded_test_cases/index.html`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.7.0/django_expanded_test_cases/test_cases/__init__.py` & `django_expanded_test_cases-0.7.1/django_expanded_test_cases/test_cases/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         Cannot use LiveServerTestCase class without "selenium" package installed.
         To use this TestCase, add the following packages to your project:
             * selenium              # Required
 
         For more information, see:
         https://www.selenium.dev/documentation/webdriver/getting_started/
         """
+
         @classmethod
         def setUpClass(cls):
             raise Exception(cls.err_msg)
 
         def setUp(self):
             raise Exception(self.err_msg)
 
@@ -54,14 +55,15 @@
             * channels              # Required
             * daphne                # Required
             * selenium              # Required
 
         For more information, see:
         https://www.selenium.dev/documentation/webdriver/getting_started/
         """
+
         @classmethod
         def setUpClass(cls):
             raise Exception(cls.err_msg)
 
         def setUp(self):
             raise Exception(self.err_msg)
```

### Comparing `django-expanded-test-cases-0.7.0/django_expanded_test_cases/test_cases/base_test_case.py` & `django_expanded_test_cases-0.7.1/django_expanded_test_cases/test_cases/base_test_case.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,20 @@
 Testing class for generalized logic.
 """
 
 # Third-Party Imports.
 from django.test import TestCase
 
 # Internal Imports.
-from django_expanded_test_cases.constants import ETC_OUTPUT_EMPHASIS_COLOR, ETC_OUTPUT_ERROR_COLOR
+from django_expanded_test_cases.constants import (
+    ETC_DEBUG_PRINT__LOGGING_SEPARATOR,
+    ETC_DEBUG_PRINT__STD_OUT_SEPARATOR,
+    ETC_OUTPUT_EMPHASIS_COLOR,
+    ETC_OUTPUT_ERROR_COLOR,
+)
 from django_expanded_test_cases.mixins import CoreTestCaseMixin
 
 
 class BaseTestCase(TestCase, CoreTestCaseMixin):
     """Generalized testing functionality. Builds upon Django's default TestCase class."""
 
     @classmethod
@@ -91,15 +96,15 @@
         Mostly for ensuring consistent output on assertion failure.
         """
         # Only handle error if an earlier function call has not yet done so.
         # This helps prevent calling this logic multiple times on error (and thus spamming console output),
         # regardless of order of testing functions.
         # We also skip output such as when the logger is disabled.
         # This is likely due to temporary checks failing, and not a legitimate error/failure.
-        if not self._error_displayed:
+        if not hasattr(self, '_error_displayed') or not self._error_displayed:
             # Print error to both logging and standard console output.
             self._debug_print(
                 '{0} {1} UnitTesting {2} {0}'.format(
                     ('=' * 10),
                     self.__class__.__name__,
                     type(err).__name__,
                 ),
@@ -107,14 +112,24 @@
                 style=ETC_OUTPUT_EMPHASIS_COLOR,
             )
             self._debug_print('{0}\n\n'.format(str(err)))
 
             # Save that we have output error.
             self._error_displayed = True
 
+            # Optionally display custom debug-output separators for additional end-of-test clarity.
+            if len(ETC_DEBUG_PRINT__STD_OUT_SEPARATOR) > 0:
+                # Local std_out separator is defined. Print to console.
+                self._debug_print(ETC_DEBUG_PRINT__STD_OUT_SEPARATOR)
+            if len(ETC_DEBUG_PRINT__LOGGING_SEPARATOR) > 0:
+                # Local std_out separator is defined. Log with logger.
+                import logging
+                logger = logging.getLogger(__name__)
+                logger.error(ETC_DEBUG_PRINT__LOGGING_SEPARATOR)
+
     # region Default Test Function Overrides
 
     def fail(self, *args, **kwargs):
         try:
             return super().fail(*args, **kwargs)
         except Exception as err:
             # If any error occurs, this makes sure it displays to console as the most recent output.
```

### Comparing `django-expanded-test-cases-0.7.0/django_expanded_test_cases/test_cases/channels_live_server_test_case.py` & `django_expanded_test_cases-0.7.1/django_expanded_test_cases/test_cases/channels_live_server_test_case.py`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.7.0/django_expanded_test_cases/test_cases/integration_test_case.py` & `django_expanded_test_cases-0.7.1/django_expanded_test_cases/test_cases/integration_test_case.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 """
 Testing logic for views and other multi-part components.
 """
 
 # System Imports.
+import logging
 import re, textwrap
 
 # Third-Party Imports.
 from django.conf import settings
 from django.core.exceptions import ValidationError
 from django.http.response import HttpResponseBase
 from django.urls import reverse
 from django.urls.exceptions import NoReverseMatch
 
 # Internal Imports.
 from .base_test_case import BaseTestCase
 from django_expanded_test_cases.constants import (
+    ETC_ASSERT_CONTENT__SURROUNDING_CHECK_OUTPUT_LENGTH,
     ETC_INCLUDE_RESPONSE_DEBUG_URL,
-    ETC_INCLUDE_RESPONSE_DEBUG_CONTENT,
-    ETC_INCLUDE_RESPONSE_DEBUG_CONTEXT,
-    ETC_INCLUDE_RESPONSE_DEBUG_FORMS,
-    ETC_INCLUDE_RESPONSE_DEBUG_HEADER,
-    ETC_INCLUDE_RESPONSE_DEBUG_MESSAGES,
-    ETC_INCLUDE_RESPONSE_DEBUG_SESSION,
-    ETC_INCLUDE_RESPONSE_DEBUG_USER_INFO,
+    ETC_RESPONSE_DEBUG_LOGGING_LEVEL,
     ETC_ALLOW_TITLE_PARTIALS,
     ETC_ALLOW_MESSAGE_PARTIALS,
-    ETC_AUTO_GENERATE_USERS,
     ETC_REQUEST_USER_STRICTNESS,
     ETC_DEFAULT_STANDARD_USER_IDENTIFIER,
     ETC_OUTPUT_ERROR_COLOR,
     ETC_OUTPUT_RESET_COLOR,
     ETC_OUTPUT_ACTUALS_MATCH_COLOR,
     ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+    ETC_VIEWS_SHOULD_REDIRECT,
     VOID_ELEMENT_LIST,
 )
 from django_expanded_test_cases.mixins import ResponseTestCaseMixin
 
 
 class IntegrationTestCase(BaseTestCase, ResponseTestCaseMixin):
     """Testing functionality for views and other multi-part components."""
@@ -112,24 +108,43 @@
         # ETC setup/teardown functions never contain a return value.
         return return_val
 
     # region Custom Assertions
 
     def assertResponse(
         self,
-        url, *args,
-        get=True, data=None, secure=True,
+        url,
+        *args,
+        get=True,
+        data=None,
+        secure=True,
         expected_status=200,
+        expected_url=None,
         expected_redirect_url=None,
-        url_args=None, url_kwargs=None, url_query_params=None,
-        redirect_args=None, redirect_kwargs=None, redirect_query_params=None,
-        expected_title=None, expected_header=None, expected_messages=None,
-        expected_content=None, expected_not_content=None,
-        auto_login=True, user=None, user_permissions=None, user_groups=None, extra_usergen_kwargs=None,
-        ignore_content_ordering=False, content_starts_after=None, content_ends_before=None,
+        view_should_redirect=None,
+        url_args=None,
+        url_kwargs=None,
+        url_query_params=None,
+        redirect_args=None,
+        redirect_kwargs=None,
+        redirect_query_params=None,
+        expected_title=None,
+        expected_header=None,
+        expected_messages=None,
+        expected_content=None,
+        expected_not_content=None,
+        auto_login=True,
+        user=None,
+        user_permissions=None,
+        user_groups=None,
+        extra_usergen_kwargs=None,
+        ignore_content_ordering=False,
+        content_starts_after=None,
+        content_ends_before=None,
+        debug_logging_level=None,
         **kwargs,
     ):
         """Verifies the view response object at given URL matches provided parameters.
 
         At minimum, gets a response object from parsing provided url, then asserts the status code matches.
         Optionally also allows testing:
             * Title - The expected title, aka what displays in the browser tab text at the top of the browser.
@@ -137,15 +152,17 @@
             * Messages - One or more messages, generated from the Django messages framework.
             * Content - One or more values that should physically appear within html rendering.
 
         :param url: Url to get response object from.
         :param get: Bool indicating if response is GET or POST. Defaults to GET.
         :param data: Optional dict of items to pass into response generation.
         :param secure: Bool indicating if request should be retrieved as HTTP or HTTPS.
+        :param expected_url: Expected url, before any redirections.
         :param expected_redirect_url: Expected url, after any redirections.
+        :param view_should_redirect: True to make sure view has redirected. False to make sure it didn't. None to skip.
         :param url_args: Values to provide for URL population, in "arg" format.
         :param url_kwargs: Values to provide for URL population, in "kwarg" format.
         :param url_query_params: Query parameter values to provide for URL population.
         :param redirect_args: Values to provide for redirect URL population, in "arg" format.
         :param redirect_kwargs: Values to provide for redirect URL population, in "kwarg" format.
         :param redirect_query_params: Query parameter values to provide for redirect URL population.
         :param expected_status: Expected status code, after any redirections. Default code of 200.
@@ -160,16 +177,30 @@
         :param user_groups: Optional groups to provide to login user.
         :param extra_usergen_kwargs: Optional dictionary of values to pass to _get_login_user__extra_user_auth_setup().
         :param ignore_content_ordering: Bool indicating if ordering should be verified. Defaults to checking ordering.
         :param content_starts_after: The HTML that expected_content should occur after. This HTML and everything
                                      preceding is stripped out of the "search space" for the expected_content value.
         :param content_ends_before: The HTML that expected_content should occur before. This HTML and everything
                                     following is stripped out of the "search space" for the expected_content value.
+        :param debug_logging_level: Optionally set a logging level. Any logging of this level or lower is disabled.
         """
 
+        # Configure logging for this specific assertion run.
+        # Can be used to disable logging output for views with many logging statements.
+        orig_logging_level = None
+        if debug_logging_level or ETC_RESPONSE_DEBUG_LOGGING_LEVEL:
+            # Try to use the value passed method, use settings value as fallback.
+            logging_level = debug_logging_level or ETC_RESPONSE_DEBUG_LOGGING_LEVEL
+            orig_logging_level = logging.getLevelName(logging.root.level)
+
+            # Set logging level, which configures logging to only show messages of set level or higher.
+            # If CRITICAL is provided, then all logging is effectively disabled.
+            # If NOTSET is provided, then all logging is effectively enabled.
+            logging.disable(getattr(logging, logging_level))
+
         # Handle mutable data defaults.
         data = data or {}
         url_args = (*args, *kwargs.pop('args', []), *(url_args or []))
         url_query_params = url_query_params or {}
         redirect_args = (*args, *(redirect_args or []))
         redirect_kwargs = {**kwargs, **(redirect_kwargs or {})}
         redirect_query_params = redirect_query_params or {}
@@ -196,60 +227,92 @@
             user_permissions=user_permissions,
             user_groups=user_groups,
             extra_usergen_kwargs=extra_usergen_kwargs,
         )
 
         # Optionally output all debug info for found response.
         if self._debug_print_bool:
-            if ETC_INCLUDE_RESPONSE_DEBUG_CONTENT:
-                self.show_debug_content(response)
-            if ETC_INCLUDE_RESPONSE_DEBUG_HEADER:
-                self.show_debug_headers(response)
-            if ETC_INCLUDE_RESPONSE_DEBUG_CONTEXT:
-                self.show_debug_context(response)
-            if ETC_INCLUDE_RESPONSE_DEBUG_SESSION:
-                self.show_debug_session_data(response)
-            if ETC_INCLUDE_RESPONSE_DEBUG_MESSAGES:
-                self.show_debug_messages(response)
-            if ETC_INCLUDE_RESPONSE_DEBUG_FORMS:
-                self.show_debug_form_data(response)
-            if ETC_INCLUDE_RESPONSE_DEBUG_USER_INFO:
-                self.show_debug_user_info(response.user)
+            self.full_debug_print(response)
 
         # Optional hook for running custom pre-builtin-test logic.
         self._assertResponse__pre_builtin_tests(
-            response.url, *args,
+            response.url,
+            *args,
             response=response,
-            get=get, data=data, secure=secure,
+            get=get,
+            data=data,
+            secure=secure,
             expected_status=expected_status,
+            expected_url=expected_url,
             expected_redirect_url=expected_redirect_url,
-            url_args=url_args, url_kwargs=url_kwargs, url_query_params=url_query_params,
-            redirect_args=redirect_args, redirect_kwargs=redirect_kwargs, redirect_query_params=redirect_query_params,
-            expected_title=expected_title, expected_header=expected_header, expected_messages=expected_messages,
-            expected_content=expected_content, expected_not_content=expected_not_content,
-            auto_login=auto_login, user=user, user_permissions=user_permissions, user_groups=user_groups,
+            view_should_redirect=view_should_redirect,
+            url_args=url_args,
+            url_kwargs=url_kwargs,
+            url_query_params=url_query_params,
+            redirect_args=redirect_args,
+            redirect_kwargs=redirect_kwargs,
+            redirect_query_params=redirect_query_params,
+            expected_title=expected_title,
+            expected_header=expected_header,
+            expected_messages=expected_messages,
+            expected_content=expected_content,
+            expected_not_content=expected_not_content,
+            auto_login=auto_login,
+            user=user,
+            user_permissions=user_permissions,
+            user_groups=user_groups,
             extra_usergen_kwargs=extra_usergen_kwargs,
-            ignore_content_ordering=ignore_content_ordering, content_starts_after=content_starts_after,
+            ignore_content_ordering=ignore_content_ordering,
+            content_starts_after=content_starts_after,
             content_ends_before=content_ends_before,
+            debug_logging_level=None,
             **kwargs,
         )
 
         # Verify page status code.
         self.assertStatusCode(response, expected_status)
 
+        # Verify base url.
+        if expected_url is not None and response.url != expected_url:
+            self.fail(
+                (
+                    'Expected Url and actual Url do not match. \n'
+                    'Expected Url: \n'
+                    '"{0}" \n'
+                    'Actual Url: \n'
+                    '"{1}" \n'
+                ).format(
+                    expected_url,
+                    response.url,
+                )
+            )
+
         # Verify page redirect.
         if expected_redirect_url is not None:
             self.assertRedirects(
                 response,
                 expected_redirect_url,
                 redirect_args=redirect_args,
                 redirect_kwargs=redirect_kwargs,
                 redirect_query_params=redirect_query_params,
             )
 
+        # Verify if redirecting or not.
+        # Set to True to make sure view redirected (accomplishes similar to above expected_redirect_url) logic.
+        # Set to False to make sure view did NOT redirect.
+        # Leave None to skip this assertion.
+        if view_should_redirect is None:
+            # No value provided for this assertion. Fall back to settings value.
+            view_should_redirect = ETC_VIEWS_SHOULD_REDIRECT
+        if view_should_redirect is not None and not (bool(response.redirect_url) == view_should_redirect):
+            if view_should_redirect:
+                self.fail('Expected a page redirect, but response did not redirect.')
+            else:
+                self.fail('Expected no page redirects, but response processed one or more redirects.')
+
         # Verify page title.
         if expected_title is not None:
             self.assertPageTitle(response, expected_title)
 
         # Verify page header.
         if expected_header is not None:
             self.assertPageHeader(response, expected_header)
@@ -275,45 +338,84 @@
                 expected_not_content,
                 debug_output=True,
                 # debug_output=False,
             )
 
         # Optional hook for running custom post-builtin-test logic.
         self._assertResponse__post_builtin_tests(
-            response.url, *args,
+            response.url,
+            *args,
             response=response,
-            get=get, data=data, secure=secure,
+            get=get,
+            data=data,
+            secure=secure,
             expected_status=expected_status,
+            expected_url=expected_url,
             expected_redirect_url=expected_redirect_url,
-            url_args=url_args, url_kwargs=url_kwargs, url_query_params=url_query_params,
-            redirect_args=redirect_args, redirect_kwargs=redirect_kwargs, redirect_query_params=redirect_query_params,
-            expected_title=expected_title, expected_header=expected_header, expected_messages=expected_messages,
-            expected_content=expected_content, expected_not_content=expected_not_content,
-            auto_login=auto_login, user=user, user_permissions=user_permissions, user_groups=user_groups,
+            view_should_redirect=view_should_redirect,
+            url_args=url_args,
+            url_kwargs=url_kwargs,
+            url_query_params=url_query_params,
+            redirect_args=redirect_args,
+            redirect_kwargs=redirect_kwargs,
+            redirect_query_params=redirect_query_params,
+            expected_title=expected_title,
+            expected_header=expected_header,
+            expected_messages=expected_messages,
+            expected_content=expected_content,
+            expected_not_content=expected_not_content,
+            auto_login=auto_login,
+            user=user,
+            user_permissions=user_permissions,
+            user_groups=user_groups,
             extra_usergen_kwargs=extra_usergen_kwargs,
-            ignore_content_ordering=ignore_content_ordering, content_starts_after=content_starts_after,
+            ignore_content_ordering=ignore_content_ordering,
+            content_starts_after=content_starts_after,
             content_ends_before=content_ends_before,
+            debug_logging_level=None,
             **kwargs,
         )
 
+        # Reset logging level for post-assertion, if it was set earlier.
+        if orig_logging_level:
+            logging.disable(getattr(logging, orig_logging_level))
+
         # All assertions passed so far. Return response in case user wants to do further checks.
         return response
 
     def assertGetResponse(
         self,
-        url, *args,
-        data=None, secure=True,
+        url,
+        *args,
+        data=None,
+        secure=True,
         expected_status=200,
+        expected_url=None,
         expected_redirect_url=None,
-        url_args=None, url_kwargs=None, url_query_params=None,
-        redirect_args=None, redirect_kwargs=None, redirect_query_params=None,
-        expected_title=None, expected_header=None, expected_messages=None,
-        expected_content=None, expected_not_content=None,
-        auto_login=True, user=None, user_permissions=None, user_groups=None, extra_usergen_kwargs=None,
-        ignore_content_ordering=False, content_starts_after=None, content_ends_before=None,
+        view_should_redirect=None,
+        url_args=None,
+        url_kwargs=None,
+        url_query_params=None,
+        redirect_args=None,
+        redirect_kwargs=None,
+        redirect_query_params=None,
+        expected_title=None,
+        expected_header=None,
+        expected_messages=None,
+        expected_content=None,
+        expected_not_content=None,
+        auto_login=True,
+        user=None,
+        user_permissions=None,
+        user_groups=None,
+        extra_usergen_kwargs=None,
+        ignore_content_ordering=False,
+        content_starts_after=None,
+        content_ends_before=None,
+        debug_logging_level=None,
         **kwargs,
     ):
         """Verifies a GET response was found at given URL, and matches provided parameters."""
 
         # Handle mutable data defaults.
         data = data or {}
         url_args = url_args or []
@@ -328,15 +430,17 @@
         return self.assertResponse(
             url,
             *args,
             get=True,
             data=data,
             secure=secure,
             expected_status=expected_status,
+            expected_url=expected_url,
             expected_redirect_url=expected_redirect_url,
+            view_should_redirect=view_should_redirect,
             url_args=url_args,
             url_kwargs=url_kwargs,
             url_query_params=url_query_params,
             redirect_args=redirect_args,
             redirect_kwargs=redirect_kwargs,
             redirect_query_params=redirect_query_params,
             expected_title=expected_title,
@@ -348,29 +452,48 @@
             user=user,
             user_permissions=user_permissions,
             user_groups=user_groups,
             extra_usergen_kwargs=extra_usergen_kwargs,
             ignore_content_ordering=ignore_content_ordering,
             content_starts_after=content_starts_after,
             content_ends_before=content_ends_before,
+            debug_logging_level=debug_logging_level,
             **kwargs,
         )
 
     def assertPostResponse(
         self,
-        url, *args,
-        data=None, secure=True,
+        url,
+        *args,
+        data=None,
+        secure=True,
         expected_status=200,
+        expected_url=None,
         expected_redirect_url=None,
-        url_args=None, url_kwargs=None, url_query_params=None,
-        redirect_args=None, redirect_kwargs=None, redirect_query_params=None,
-        expected_title=None, expected_header=None, expected_messages=None,
-        expected_content=None, expected_not_content=None,
-        auto_login=True, user=None, user_permissions=None, user_groups=None, extra_usergen_kwargs=None,
-        ignore_content_ordering=False, content_starts_after=None, content_ends_before=None,
+        view_should_redirect=None,
+        url_args=None,
+        url_kwargs=None,
+        url_query_params=None,
+        redirect_args=None,
+        redirect_kwargs=None,
+        redirect_query_params=None,
+        expected_title=None,
+        expected_header=None,
+        expected_messages=None,
+        expected_content=None,
+        expected_not_content=None,
+        auto_login=True,
+        user=None,
+        user_permissions=None,
+        user_groups=None,
+        extra_usergen_kwargs=None,
+        ignore_content_ordering=False,
+        content_starts_after=None,
+        content_ends_before=None,
+        debug_logging_level=None,
         **kwargs,
     ):
         """Verifies a GET response was found at given URL, and matches provided parameters."""
 
         # Handle mutable data defaults.
         data = data or {}
         url_args = url_args or []
@@ -391,15 +514,17 @@
         return self.assertResponse(
             url,
             *args,
             get=False,
             data=data,
             secure=secure,
             expected_status=expected_status,
+            expected_url=expected_url,
             expected_redirect_url=expected_redirect_url,
+            view_should_redirect=view_should_redirect,
             url_args=url_args,
             url_kwargs=url_kwargs,
             url_query_params=url_query_params,
             redirect_args=redirect_args,
             redirect_kwargs=redirect_kwargs,
             redirect_query_params=redirect_query_params,
             expected_title=expected_title,
@@ -411,21 +536,27 @@
             user=user,
             user_permissions=user_permissions,
             user_groups=user_groups,
             extra_usergen_kwargs=extra_usergen_kwargs,
             ignore_content_ordering=ignore_content_ordering,
             content_starts_after=content_starts_after,
             content_ends_before=content_ends_before,
+            debug_logging_level=debug_logging_level,
             **kwargs,
         )
 
     def assertRedirects(
         self,
-        response, expected_redirect_url, *args,
-        redirect_args=None, redirect_kwargs=None, redirect_query_params=None, **kwargs,
+        response,
+        expected_redirect_url,
+        *args,
+        redirect_args=None,
+        redirect_kwargs=None,
+        redirect_query_params=None,
+        **kwargs,
     ):
         """Assert that a response redirected to a specific URL and that the redirect URL can be loaded.
 
         Most functionality is in the default Django assertRedirects() function.
         However, this acts as a wrapper to also:
             * Check that provided response param is a valid Response object. Attempts to generate one if not.
             * Attempt url as reverse, before trying assertion.
@@ -452,17 +583,19 @@
             append_root=False,
         )
 
         # Run assertion on provided value.
         try:
             return super().assertRedirects(response, expected_redirect_url, *args, **kwargs)
         except AssertionError:
-            self.fail('Response didn\'t redirect as expected. Response code was {0} (expected 302).'.format(
-                response.status_code
-            ))
+            self.fail(
+                'Response didn\'t redirect as expected. Response code was {0} (expected 302).'.format(
+                    response.status_code
+                )
+            )
 
     def assertStatusCode(self, response, expected_status):
         """Verifies the page status code value.
 
         :param response: Response object to check against.
         :param expected_status: Expected status code, after any redirections.
         """
@@ -517,27 +650,31 @@
         expected_title = expected_title.strip()
 
         # Check element.
         err_msg = 'Expected title HTML contents of "{0}" ({1}). Actual value was "{2}".'
         if not allow_partials:
             # Check using exact match.
             if expected_title != actual_title:
-                self.fail(err_msg.format(
-                    expected_title,
-                    'using exact matching',
-                    actual_title,
-                ))
+                self.fail(
+                    err_msg.format(
+                        expected_title,
+                        'using exact matching',
+                        actual_title,
+                    )
+                )
         else:
             # Check using partial match.
             if expected_title not in actual_title:
-                self.fail(err_msg.format(
-                    expected_title,
-                    'using partial matching',
-                    actual_title,
-                ))
+                self.fail(
+                    err_msg.format(
+                        expected_title,
+                        'using partial matching',
+                        actual_title,
+                    )
+                )
 
         # Return title in case user wants to run additional logic on it.
         return actual_title
 
     def assertPageHeader(self, response, expected_header):
         """Verifies the page H1 header HTML element.
 
@@ -554,18 +691,20 @@
             expected_header = expected_header[4:]
         if expected_header.endswith('</h1>'):
             expected_header = expected_header[:-5]
         expected_header = expected_header.strip()
 
         # Check element.
         if expected_header != actual_header:
-            self.fail('Expected H1 header HTML contents of "{0}". Actual value was "{1}".'.format(
-                expected_header,
-                actual_header,
-            ))
+            self.fail(
+                'Expected H1 header HTML contents of "{0}". Actual value was "{1}".'.format(
+                    expected_header,
+                    actual_header,
+                )
+            )
 
         # Return header in case user wants to run additional logic on it.
         return actual_header
 
     def assertContextMessages(self, response, expected_messages, allow_partials=None, debug_output=True):
         """Verifies the context messages.
 
@@ -634,23 +773,28 @@
 
                     # Loop through all context messages until found, or all are checked.
                     if expected_message in actual_messages:
                         message_found = True
 
                 # Raise assertion error if not found.
                 if not message_found:
-                    self.fail('Failed to find message "{0}" in context (using {1} matching).'.format(
-                        expected_message,
-                        'partial' if allow_partials else 'exact'
-                    ))
+                    self.fail(
+                        'Failed to find message "{0}" in context (using {1} matching).'.format(
+                            expected_message, 'partial' if allow_partials else 'exact'
+                        )
+                    )
 
     def assertPageContent(
         self,
-        response, expected_content,
-        ignore_ordering=False, content_starts_after=None, content_ends_before=None, debug_output=True,
+        response,
+        expected_content,
+        ignore_ordering=False,
+        content_starts_after=None,
+        content_ends_before=None,
+        debug_output=True,
     ):
         """Verifies the page content html, similar to the built-in assertContains() function.
         The main difference is that Django templating may create large amounts of whitespace in response html,
         often in places where we wouldn't intuitively expect it, when running tests.
         Technically, the built-in assertHTMLEqual() and assertInHTML() functions exist, and probably could accomplish
         the same assertions. But we still need to parse and format full response object, to display for test failure
         debugging. So I'm not sure if it's helpful at that point to use those or use separate assertions like here.
@@ -667,26 +811,26 @@
         :return: Parsed out and formatted content string.
         """
         if debug_output:
             # Print out actual response content, for debug output.
             self.show_debug_content(response)
 
         main_err_msg = (
+            # To prevent Black single-lining this.
             'Could not find expected content value in response. Provided value was:\n'
             '{0}\n'
         )
         checked_content_str_addon = (
+            # To prevent Black single-lining this.
             '\n'
             '\n'
             'Surrounding Checks:\n'
             '{0}'
             '{1}'
             '{2}'
-            '{3}'
-            '{4}'
         )
         ordering_err_msg = 'Expected content value was found, but ordering of values do not match. Problem value:\n{0}'
         casing_err_msg = (
             'Expected content value was found, but letter capitalization did not match. Expected was:\n'
             '{0}\n'
             '\n'
             'Found was:\n'
@@ -709,41 +853,84 @@
             # The expected_content param is an array of items. Verify they all exist on page.
             trimmed_content = trimmed_original_content
             for index in range(len(expected_content)):
                 expected = expected_content[index]
 
                 if len(expected_content) > 1:
                     # Update str in event of error.
-                    updated_checked_content_str_addon = checked_content_str_addon.format(
-                        '{1}    * {0}{2}\n'.format(
-                            expected_content[index - 2],
+                    before_debug_output = ''
+                    before_debug_output_statements = ''
+                    after_debug_output = ''
+                    after_debug_output_statements = ''
+
+                    # Handle "before" output.
+                    if ETC_ASSERT_CONTENT__SURROUNDING_CHECK_OUTPUT_LENGTH > 0:
+                        before_debug_output = '{0}Content Checks Before:{1}\n'.format(
                             ETC_OUTPUT_EXPECTED_MATCH_COLOR,
                             ETC_OUTPUT_RESET_COLOR,
-                        ) if index >= 2 else '',
-                        '{1}    * {0}{2}\n'.format(
-                            expected_content[index - 1],
-                            ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                        )
+
+                        for surrounding_check_index in reversed(range(ETC_ASSERT_CONTENT__SURROUNDING_CHECK_OUTPUT_LENGTH + 1)):
+                            if surrounding_check_index == 0:
+                                continue
+
+                            before_debug_output_statements += (
+                                '{1}    * {0}{2}\n'.format(
+                                    expected_content[index - surrounding_check_index],
+                                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                                    ETC_OUTPUT_RESET_COLOR,
+                                )
+                                if 0 < ((index + 1) - surrounding_check_index) < len(expected_content)
+                                else ''
+                            )
+
+                        if before_debug_output_statements != '':
+                            before_debug_output += before_debug_output_statements
+                        else:
+                            before_debug_output = ''
+
+                    # Handle "after" output.
+                    if ETC_ASSERT_CONTENT__SURROUNDING_CHECK_OUTPUT_LENGTH > 0:
+                        after_debug_output = '{0}Content Checks After:{1}\n'.format(
+                            ETC_OUTPUT_ACTUALS_MATCH_COLOR,
                             ETC_OUTPUT_RESET_COLOR,
-                        ) if index >= 1 else '',
-                        '{1}  > * {0}{2}\n'.format(
+                        )
+
+                        for surrounding_check_index in range(ETC_ASSERT_CONTENT__SURROUNDING_CHECK_OUTPUT_LENGTH + 1):
+                            if surrounding_check_index == 0:
+                                continue
+
+                            after_debug_output_statements += (
+                                '{1}    * {0}{2}\n'.format(
+                                    expected_content[index + surrounding_check_index],
+                                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                                    ETC_OUTPUT_RESET_COLOR,
+                                )
+                                if (len(expected_content) - index) > surrounding_check_index
+                                else ''
+                            )
+
+                        if after_debug_output_statements != '':
+                            after_debug_output += after_debug_output_statements
+                        else:
+                            after_debug_output = ''
+
+                    updated_checked_content_str_addon = checked_content_str_addon.format(
+                        before_debug_output,
+                        (
+                            '{1}Failed Check:{2}\n'
+                            '{1}  > * {0}{2}\n'
+                        ).format(
                             expected_content[index],
                             ETC_OUTPUT_ERROR_COLOR,
                             ETC_OUTPUT_RESET_COLOR,
                         ),
-                        '{1}    * {0}{2}\n'.format(
-                            expected_content[index + 1],
-                            ETC_OUTPUT_ACTUALS_MATCH_COLOR,
-                            ETC_OUTPUT_RESET_COLOR,
-                        ) if (len(expected_content) - index) > 1 else '',
-                        '{1}    * {0}{2}\n'.format(
-                            expected_content[index + 2],
-                            ETC_OUTPUT_ACTUALS_MATCH_COLOR,
-                            ETC_OUTPUT_RESET_COLOR,
-                        ) if (len(expected_content) - index) > 2 else '',
+                        after_debug_output,
                     )
+
                 else:
                     updated_checked_content_str_addon = ''
 
                 # Handle if expected is a list or tuple.
                 additional_error_info = ''
                 if (isinstance(expected, list) or isinstance(expected, tuple)) and len(expected) == 2:
                     # Nested array or tuple.
@@ -873,17 +1060,21 @@
                     )
 
         # Return page content in case user wants to run additional logic on it.
         return trimmed_original_content
 
     def _assertPageContent(
         self,
-        actual_content, minimized_expected, display_expected,
-        strip_actual_start, strip_actual_end,
-        err_msg, checked_content_str_addon,
+        actual_content,
+        minimized_expected,
+        display_expected,
+        strip_actual_start,
+        strip_actual_end,
+        err_msg,
+        checked_content_str_addon,
         additional_error_info='',
     ):
         """Internal sub-assertion for assertPageContent() function."""
         strip_err_msg = 'Expected content value was found, but occurred in "{0}" section. Expected was:\n{1}'
 
         # Check if error was due to content_starts_after/content_ends_before variables.
         found_expected = False
@@ -902,23 +1093,25 @@
             # Content value was in stripped section. Raise corresponding strip message.
             if checked_content_str_addon:
                 strip_err_msg += checked_content_str_addon
             self.fail(strip_err_msg.format(found_expected, display_expected))
 
         else:
             # Content value was physically not present at all. Raise "main" message.
+            updated_err_msg = err_msg.format(display_expected)
             if checked_content_str_addon:
-                err_msg += checked_content_str_addon
+                updated_err_msg += checked_content_str_addon
             if additional_error_info:
-                err_msg += '\n{0}'.format(additional_error_info)
-            self.fail(err_msg.format(display_expected))
+                updated_err_msg += '\n{0}'.format(additional_error_info)
+            self.fail(updated_err_msg)
 
     def assertNotPageContent(
         self,
-        response, expected_not_content,
+        response,
+        expected_not_content,
         debug_output=True,
     ):
         """Verifies the non-existance of page content html.
         Django templating may create large amounts of whitespace in response html, often in places where we wouldn't
         intuitively expect it, when running tests. This converts output to a more normalized/predictable format,
         and then verifies the normalized content is not present. Results in more consistent and predictable testing.
 
@@ -970,16 +1163,20 @@
                 self.fail(
                     'Found content in response. Expected content to not be present. Content was:\n'
                     '{0}'.format(expected_not_content)
                 )
 
     def assertRepeatingElement(
         self,
-        response, expected_repeating_element, repeat_count,
-        content_starts_after=None, content_ends_before=None, debug_output=True,
+        response,
+        expected_repeating_element,
+        repeat_count,
+        content_starts_after=None,
+        content_ends_before=None,
+        debug_output=True,
     ):
         """Verifies that a given HTMl element repeats, within a given section of content.
 
         Note: This expects a full HTML element, including both opening and closing tags.
 
         :param response: Response object to check against.
         :param expected_repeating_element: The expected repeating HTML element. Ex: <li>, <p>, etc.
@@ -1097,17 +1294,25 @@
         # Return calculated user.
         return user
 
     def _get_page_response(
         self,
         url,
         *args,
-        get=True, data=None, secure=True,
-        url_args=None, url_kwargs=None, query_params=None,
-        auto_login=True, user=None, user_permissions=None, user_groups=None, extra_usergen_kwargs=None,
+        get=True,
+        data=None,
+        secure=True,
+        url_args=None,
+        url_kwargs=None,
+        query_params=None,
+        auto_login=True,
+        user=None,
+        user_permissions=None,
+        user_groups=None,
+        extra_usergen_kwargs=None,
         **kwargs,
     ):
         """Helper function for assertResponse().
 
         Fully parses provided user url, and returns corresponding response object.
 
         :param url: Url to get response object from.
@@ -1161,14 +1366,19 @@
             response = self.client.get(url, data=data, secure=secure, follow=True)
         else:
             response = self.client.post(url, data=data, secure=secure, follow=True)
 
         # Update response object with additional useful values for further testing/analysis.
         response.url = url
         response.full_url = full_url
+        response.redirect_url = None
+        if hasattr(response, 'redirect_chain') and len(response.redirect_chain) > 0:
+            redirect_data = response.redirect_chain[-1]
+            if redirect_data[1] == 302 or redirect_data[0] != response.url:
+                response.redirect_url = redirect_data[0]
         response.user = user
 
         # Return generated response.
         return response
 
     def _get_login_user(self, user, *args, auto_login=True, user_permissions=None, user_groups=None, **kwargs):
         """Handles simulating user login with corresponding permissions/groups/etc.
@@ -1276,22 +1486,26 @@
 
         elif response_title is not None:
             # Tag was found.
 
             # Check how many title tags were found.
             if len(response_title) > 1:
                 # Multiple headers were found. Raise error and direct user to helper h1 documentation.
-                raise AssertionError(textwrap.dedent(
-                    """
+                raise AssertionError(
+                    textwrap.dedent(
+                        """
                     Found multiple titles ({0} total). There should only be one <title> tag per page.
                     For further reference on <title> tags, consider consulting:
                         * https://www.w3schools.com/tags/tag_title.asp
                         * https://developer.mozilla.org/en-US/docs/Web/HTML/Element/title
-                    """.format(len(response_title))
-                ).strip())
+                    """.format(
+                            len(response_title)
+                        )
+                    ).strip()
+                )
 
             elif len(response_title) == 0:
                 # No title text was found. Return empty string.
                 response_title = ''
 
             elif len(response_title) == 1:
 
@@ -1334,22 +1548,26 @@
 
         elif response_header is not None:
             # Tag was found.
 
             # Check how many header tags were found.
             if len(response_header) > 1:
                 # Multiple headers were found. Raise error and direct user to helper h1 documentation.
-                raise AssertionError(textwrap.dedent(
-                    """
+                raise AssertionError(
+                    textwrap.dedent(
+                        """
                     Found multiple headers ({0} total). There should only be one <h1> tag per page.
                     For further reference on <h1> tags, consider consulting:
                         * https://www.w3schools.com/tags/tag_hn.asp
                         * https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Heading_Elements
-                    """.format(len(response_header))
-                ).strip())
+                    """.format(
+                            len(response_header)
+                        )
+                    ).strip()
+                )
 
             elif len(response_header) == 0:
                 # No headers text was found. Return empty string.
                 response_header = ''
 
             elif len(response_header) == 1:
 
@@ -1443,43 +1661,69 @@
 
     # endregion Helper Functions
 
     # region Hook Functions
 
     def _assertResponse__pre_builtin_tests(
         self,
-        url, *args,
-        get=True, data=None,
+        url,
+        *args,
+        get=True,
+        data=None,
         expected_status=200,
         expected_redirect_url=None,
-        url_args=None, url_kwargs=None, redirect_args=None, redirect_kwargs=None,
-        expected_title=None, expected_header=None, expected_messages=None, expected_content=None,
-        auto_login=True, user=None, user_permissions=None, user_groups=None,
-        ignore_content_ordering=False, content_starts_after=None, content_ends_before=None,
+        url_args=None,
+        url_kwargs=None,
+        redirect_args=None,
+        redirect_kwargs=None,
+        expected_title=None,
+        expected_header=None,
+        expected_messages=None,
+        expected_content=None,
+        auto_login=True,
+        user=None,
+        user_permissions=None,
+        user_groups=None,
+        ignore_content_ordering=False,
+        content_starts_after=None,
+        content_ends_before=None,
         **kwargs,
     ):
         """Hook function to allow injecting code prior to running any of the built-in assertResponse() tests.
 
         For maximum usability, this function receives all args/kwargs provided to the default assertResponse()
         function.
 
         This hook does nothing by default, and is exclusively provided for custom extension logic.
         """
         pass
 
     def _assertResponse__post_builtin_tests(
         self,
-        url, *args,
-        get=True, data=None,
+        url,
+        *args,
+        get=True,
+        data=None,
         expected_status=200,
         expected_redirect_url=None,
-        url_args=None, url_kwargs=None, redirect_args=None, redirect_kwargs=None,
-        expected_title=None, expected_header=None, expected_messages=None, expected_content=None,
-        auto_login=True, user=None, user_permissions=None, user_groups=None,
-        ignore_content_ordering=False, content_starts_after=None, content_ends_before=None,
+        url_args=None,
+        url_kwargs=None,
+        redirect_args=None,
+        redirect_kwargs=None,
+        expected_title=None,
+        expected_header=None,
+        expected_messages=None,
+        expected_content=None,
+        auto_login=True,
+        user=None,
+        user_permissions=None,
+        user_groups=None,
+        ignore_content_ordering=False,
+        content_starts_after=None,
+        content_ends_before=None,
         **kwargs,
     ):
         """Hook function to allow injecting code after running all of the built-in assertResponse() tests.
 
         For maximum usability, this function receives all args/kwargs provided to the default assertResponse()
         function.
 
@@ -1488,15 +1732,16 @@
         pass
 
     def _get_login_user__extra_user_auth_setup(
         self,
         user,
         *args,
         auto_login=True,
-        user_permissions=None, user_groups=None,
+        user_permissions=None,
+        user_groups=None,
         **kwargs,
     ):
         """Hook function, to allow running extra authentication setup logic on User object.
 
         Useful such as for running things like 2-Factor setup logic for User.
 
         For maximum usability, this function receives all args/kwargs provided to the default _get_login_user()
```

### Comparing `django-expanded-test-cases-0.7.0/django_expanded_test_cases/test_cases/live_server_test_case.py` & `django_expanded_test_cases-0.7.1/django_expanded_test_cases/test_cases/live_server_test_case.py`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.7.0/django_expanded_test_cases/test_urls.py` & `django_expanded_test_cases-0.7.1/django_expanded_test_cases/test_urls.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,23 +16,27 @@
     # Simple test views.
     path('login/', views.login, name='login'),
     path('views/one-message/', views.view_with_one_message, name='response-with-one-message'),
     path('views/two-messages/', views.view_with_two_messages, name='response-with-two-messages'),
     path('views/three-messages/', views.view_with_three_messages, name='response-with-three-messages'),
     path('views/repeating-elements/', views.view_with_repeating_elements, name='response-with-repeating-elements'),
     path('views/<int:id>/<str:name>/', views.view_with_args, name='response-with-args'),
-
     # Template response views.
     path('template-response/index/', views.template_response_index, name='template-response-index'),
-    path('template-response/messages/', views.template_response_with_three_messages, name='template-response-messages'),
-    path('template-response/<int:id>/<str:name>/', views.template_response_with_args, name='template-response-with-args'),
-
+    path(
+        'template-response/messages/',
+        views.template_response_with_three_messages,
+        name='template-response-messages',
+    ),
+    path(
+        'template-response/<int:id>/<str:name>/',
+        views.template_response_with_args,
+        name='template-response-with-args',
+    ),
     # Model test views.
     path('user/detail/<int:pk>/', views.user_detail, name='user-detail'),
-
     # Redirect views.
     path('redirect/index/', views.redirect_to_index, name='redirect-to-index'),
     path('redirect/with_args/<int:id>/<str:name>/', views.redirect_with_args, name='redirect-with-args'),
-
     # Index view.
     path('', views.index, name='index'),
 ]
```

### Comparing `django-expanded-test-cases-0.7.0/django_expanded_test_cases.egg-info/PKG-INFO` & `django_expanded_test_cases-0.7.1/django_expanded_test_cases.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-expanded-test-cases
-Version: 0.7.0
+Version: 0.7.1
 Summary: Expands the existing Django TestCase class with extra functionality.
 Home-page: https://github.com/brodriguez8774/django-expanded-test-cases
 Author: Brandon Rodriguez
 Author-email: Brandon Rodriguez <brodriguez8774@gmail.com>
 Maintainer-email: Brandon Rodriguez <brodriguez8774@gmail.com>
 License: MIT License
```

### Comparing `django-expanded-test-cases-0.7.0/django_expanded_test_cases.egg-info/SOURCES.txt` & `django_expanded_test_cases-0.7.1/django_expanded_test_cases.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 LICENSE
 MANIFEST.in
 pyproject.toml
 readme.md
 setup.cfg
 django_expanded_test_cases/__init__.py
-django_expanded_test_cases/constants.py
 django_expanded_test_cases/exceptions.py
 django_expanded_test_cases/test_urls.py
 django_expanded_test_cases.egg-info/PKG-INFO
 django_expanded_test_cases.egg-info/SOURCES.txt
 django_expanded_test_cases.egg-info/dependency_links.txt
 django_expanded_test_cases.egg-info/requires.txt
 django_expanded_test_cases.egg-info/top_level.txt
+django_expanded_test_cases/constants/__init__.py
+django_expanded_test_cases/constants/auth_constants.py
+django_expanded_test_cases/constants/debug_output_constants.py
+django_expanded_test_cases/constants/general_handling_constants.py
+django_expanded_test_cases/constants/selenium_constants.py
 django_expanded_test_cases/mixins/__init__.py
 django_expanded_test_cases/mixins/core_mixin.py
 django_expanded_test_cases/mixins/live_server_mixin.py
 django_expanded_test_cases/mixins/response_mixin.py
 django_expanded_test_cases/templates/django_expanded_test_cases/index.html
 django_expanded_test_cases/test_cases/__init__.py
 django_expanded_test_cases/test_cases/base_test_case.py
@@ -24,14 +28,13 @@
 django_expanded_test_cases/test_cases/live_server_test_case.py
 etc_tests/__init__.py
 etc_tests/apps.py
 etc_tests/asgi.py
 etc_tests/settings.py
 etc_tests/urls.py
 etc_tests/views.py
-etc_tests/mock_pages/__init__.py
 etc_tests/test_cases/__init__.py
 etc_tests/test_cases/test_base_case.py
 etc_tests/test_cases/test_channels_live_server_case.py
 etc_tests/test_cases/test_integration_case.py
 etc_tests/test_cases/test_live_server_case.py
 etc_tests/test_cases/universal_live_test_mixin.py
```

### Comparing `django-expanded-test-cases-0.7.0/etc_tests/asgi.py` & `django_expanded_test_cases-0.7.1/etc_tests/asgi.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-
 # System Imports.
 import os
 
 # Third-Party Imports.
 import django
 from channels.routing import ProtocolTypeRouter
 
 # Import handling for post-Django V2.
 try:
     from django.core.asgi import get_asgi_application as AsgiHandler
+
     # Success. Is Django3 or higher.
 except ImportError:
     # Failure. Likely Django 2.
     from channels.http import AsgiHandler
 
 
 os.environ.setdefault('DJANGO_SETTINGS_MODULE', 'etc_tests.settings')
 django.setup()
 
 
-application = ProtocolTypeRouter({
-  "http": AsgiHandler(),
-  # Just HTTP for now. (We can add other protocols later.)
-})
+application = ProtocolTypeRouter(
+    {
+        "http": AsgiHandler(),
+        # Just HTTP for now. (We can add other protocols later.)
+    }
+)
```

### Comparing `django-expanded-test-cases-0.7.0/etc_tests/settings.py` & `django_expanded_test_cases-0.7.1/etc_tests/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 except ModuleNotFoundError:
     # Failed to import channels. Assume not installed.
     CHANNELS_PACKAGE_INSTALLED = False
 
 
 INSTALLED_APPS = (
     'django_expanded_test_cases',
-
     'django.contrib.admin',
     'django.contrib.auth',
     'django.contrib.contenttypes',
     'django.contrib.sessions',
     'django.contrib.messages',
     'django.contrib.staticfiles',
 )
```

### Comparing `django-expanded-test-cases-0.7.0/etc_tests/test_cases/test_base_case.py` & `django_expanded_test_cases-0.7.1/etc_tests/test_cases/test_base_case.py`

 * *Files 12% similar despite different names*

```diff
@@ -112,16 +112,16 @@
 
         with self.subTest('Large string'):
             # Full lorem.
             self.assertText(lorem_str, lorem_str)
 
             # Substring match.
             lorem_len = len(lorem_str)
-            self.assertText(lorem_str[:int(lorem_len / 2)], lorem_str[:int(lorem_len / 2)])
-            self.assertText(lorem_str[int(lorem_len / 2):], lorem_str[int(lorem_len / 2):])
+            self.assertText(lorem_str[: int(lorem_len / 2)], lorem_str[: int(lorem_len / 2)])
+            self.assertText(lorem_str[int(lorem_len / 2) :], lorem_str[int(lorem_len / 2) :])
 
     def test__assertText__fail(self):
         """
         Tests assertText() function, in cases when it should fail.
         """
         exception_msg = '\'{0}\' != \'{1}\'\n- {0}\n{2}+ {1}\n{3}'
 
@@ -137,19 +137,35 @@
             with self.assertRaises(AssertionError) as err:
                 self.assertText('a', 1)
             self.assertEqual(exception_msg.format('a', '1', '', ''), str(err.exception))
 
         with self.subTest('Whitespace mismatch'):
             with self.assertRaises(AssertionError) as err:
                 self.assertText('a b c', 'abc')
-            self.assertEqual(exception_msg.format('a b c', 'abc', '?  - -\n', ''), str(err.exception))
+            self.assertEqual(
+                exception_msg.format(
+                    'a b c',
+                    'abc',
+                    '?  - -\n',
+                    '',
+                ),
+                str(err.exception),
+            )
 
             with self.assertRaises(AssertionError) as err:
                 self.assertText('abc', 'a b c')
-            self.assertEqual(exception_msg.format('abc', 'a b c', '', '?  + +\n'), str(err.exception))
+            self.assertEqual(
+                exception_msg.format(
+                    'abc',
+                    'a b c',
+                    '',
+                    '?  + +\n',
+                ),
+                str(err.exception),
+            )
 
         with self.subTest('Inner value mismatch'):
             with self.assertRaises(AssertionError) as err:
                 self.assertText('This is a test sentence.', 'This is a test')
             self.assertEqual(
                 exception_msg.format(
                     'This is a test sentence.',
@@ -159,50 +175,65 @@
                 ),
                 str(err.exception),
             )
 
             with self.assertRaises(AssertionError) as err:
                 self.assertText('This is a test sentence.', 'This is test sentence.')
             self.assertEqual(
-                exception_msg.format('This is a test sentence.', 'This is test sentence.', '?        --\n', ''),
+                exception_msg.format(
+                    'This is a test sentence.',
+                    'This is test sentence.',
+                    '?        --\n',
+                    '',
+                ),
                 str(err.exception),
             )
 
             with self.assertRaises(AssertionError) as err:
                 self.assertText('This is a test sentence.', 'test sentence.')
             self.assertEqual(
-                exception_msg.format('This is a test sentence.', 'test sentence.', '? ----------\n', ''),
+                exception_msg.format(
+                    'This is a test sentence.',
+                    'test sentence.',
+                    '? ----------\n',
+                    '',
+                ),
                 str(err.exception),
             )
 
             with self.assertRaises(AssertionError) as err:
                 self.assertText('This is a test sentence.', 'This is a test.')
             self.assertEqual(
-                exception_msg.format('This is a test sentence.', 'This is a test.', '?               ---------\n', ''),
+                exception_msg.format(
+                    'This is a test sentence.',
+                    'This is a test.',
+                    '?               ---------\n',
+                    '',
+                ),
                 str(err.exception),
             )
 
         with self.subTest('Large string'):
             half_lorem_len = int(len(lorem_str) / 2)
 
             # With character replaced.
             with self.assertRaises(AssertionError) as err:
-                modified_str = lorem_str[:(half_lorem_len - 1)] + 'z' + lorem_str[(half_lorem_len + 1):]
+                modified_str = lorem_str[: (half_lorem_len - 1)] + 'z' + lorem_str[(half_lorem_len + 1) :]
                 self.assertText(lorem_str, modified_str)
             # self.assertEqual(str(err.exception), exception_msg)
 
             # With character added.
             with self.assertRaises(AssertionError) as err:
-                modified_str = lorem_str[:(half_lorem_len)] + 'z' + lorem_str[(half_lorem_len + 1):]
+                modified_str = lorem_str[:(half_lorem_len)] + 'z' + lorem_str[(half_lorem_len + 1) :]
                 self.assertText(lorem_str, modified_str)
             # self.assertEqual(str(err.exception), exception_msg)
 
             # With character removed.
             with self.assertRaises(AssertionError) as err:
-                modified_str = lorem_str[:(half_lorem_len - 1)] + lorem_str[(half_lorem_len + 1):]
+                modified_str = lorem_str[: (half_lorem_len - 1)] + lorem_str[(half_lorem_len + 1) :]
                 self.assertText(lorem_str, modified_str)
             # self.assertEqual(str(err.exception), exception_msg)
 
     @skipIf(not settings.DJANGO_EXPANDED_TESTCASES_DEBUG_PRINT, 'Test only works as expected with DEBUG PRINT.')
     def test__assertText_coloring__missing_lines(self):
         """Tests assertText() function color output, when assertion fails due to incorrect line counts.
 
@@ -216,22 +247,37 @@
             std_out_lines = std_out.getvalue().split('\n')[3:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
             self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[4],
+                '{0}EXPECTED:{1}'.format(
+                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(std_out_lines[5], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[8],
+                '{0}ACTUAL:{1}'.format(
+                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(
                 std_out_lines[9],
-                '{0}Actuals has values here. Expected does not.{1}'.format(ETC_OUTPUT_ACTUALS_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
+                '{0}Actuals has values here. Expected does not.{1}'.format(
+                    ETC_OUTPUT_ACTUALS_ERROR_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
             )
             self.assertEqual(std_out_lines[10], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[11], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[12], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[13], '')
 
         with self.subTest('With actuals as empty'):
@@ -242,23 +288,38 @@
             std_out_lines = std_out.getvalue().split('\n')[5:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
             self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[4],
+                '{0}EXPECTED:{1}'.format(
+                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(
                 std_out_lines[5],
-                '{0}Expected has values here. Actuals does not.{1}'.format(ETC_OUTPUT_EXPECTED_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
+                '{0}Expected has values here. Actuals does not.{1}'.format(
+                    ETC_OUTPUT_EXPECTED_ERROR_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
             )
             self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[8], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[9], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[9],
+                '{0}ACTUAL:{1}'.format(
+                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(std_out_lines[10], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[11], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[12], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[13], '')
 
         with self.subTest('With expected as empty and actuals as multi-line'):
             std_out = StringIO()
@@ -268,24 +329,45 @@
             std_out_lines = std_out.getvalue().split('\n')[4:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
             self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[4],
+                '{0}EXPECTED:{1}'.format(
+                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(std_out_lines[5], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[8],
+                '{0}ACTUAL:{1}'.format(
+                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(
                 std_out_lines[9],
-                '{0}Actuals has values here.{1}'.format(ETC_OUTPUT_ACTUALS_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
+                '{0}Actuals has values here.{1}'.format(
+                    ETC_OUTPUT_ACTUALS_ERROR_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
+            self.assertEqual(
+                std_out_lines[10],
+                '{0}Expected does not.{1}'.format(
+                    ETC_OUTPUT_ACTUALS_ERROR_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
             )
-            self.assertEqual(std_out_lines[10], '{0}Expected does not.{1}'.format(ETC_OUTPUT_ACTUALS_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR))
             self.assertEqual(std_out_lines[11], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[12], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[13], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[14], '')
 
         with self.subTest('With actuals as empty and expected as multi-line'):
             std_out = StringIO()
@@ -295,24 +377,45 @@
             std_out_lines = std_out.getvalue().split('\n')[4:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
             self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[4],
+                '{0}EXPECTED:{1}'.format(
+                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(
                 std_out_lines[5],
-                '{0}Expected has values here.{1}'.format(ETC_OUTPUT_EXPECTED_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
+                '{0}Expected has values here.{1}'.format(
+                    ETC_OUTPUT_EXPECTED_ERROR_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
+            self.assertEqual(
+                std_out_lines[6],
+                '{0}Actuals does not.{1}'.format(
+                    ETC_OUTPUT_EXPECTED_ERROR_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
             )
-            self.assertEqual(std_out_lines[6], '{0}Actuals does not.{1}'.format(ETC_OUTPUT_EXPECTED_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR))
             self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[8], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[9], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[10], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[10],
+                '{0}ACTUAL:{1}'.format(
+                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(std_out_lines[11], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[12], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[13], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[14], '')
 
         with self.subTest('With expected as one line less - At end'):
             std_out = StringIO()
@@ -324,22 +427,52 @@
             std_out_lines = std_out.getvalue().split('\n')[6:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
             self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
-            self.assertEqual(std_out_lines[5], '{0}One line.{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[4],
+                '{0}EXPECTED:{1}'.format(
+                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
+            self.assertEqual(
+                std_out_lines[5],
+                '{0}One line.{1}'.format(
+                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[8], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[9], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
-            self.assertEqual(std_out_lines[10], '{0}One line.{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
-            self.assertEqual(std_out_lines[11], '{0}Two line.{1}'.format(ETC_OUTPUT_ACTUALS_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[9],
+                '{0}ACTUAL:{1}'.format(
+                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
+            self.assertEqual(
+                std_out_lines[10],
+                '{0}One line.{1}'.format(
+                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
+            self.assertEqual(
+                std_out_lines[11],
+                '{0}Two line.{1}'.format(
+                    ETC_OUTPUT_ACTUALS_ERROR_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(std_out_lines[12], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[13], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[14], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[15], '')
 
         with self.subTest('With actuals as one line less - At end'):
             std_out = StringIO()
@@ -349,22 +482,52 @@
             std_out_lines = std_out.getvalue().split('\n')[5:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
             self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
-            self.assertEqual(std_out_lines[5], '{0}One line.{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
-            self.assertEqual(std_out_lines[6], '{0}Two line.{1}'.format(ETC_OUTPUT_EXPECTED_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[4],
+                '{0}EXPECTED:{1}'.format(
+                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
+            self.assertEqual(
+                std_out_lines[5],
+                '{0}One line.{1}'.format(
+                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
+            self.assertEqual(
+                std_out_lines[6],
+                '{0}Two line.{1}'.format(
+                    ETC_OUTPUT_EXPECTED_ERROR_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[8], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[9], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[10], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
-            self.assertEqual(std_out_lines[11], '{0}One line.{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[10],
+                '{0}ACTUAL:{1}'.format(
+                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
+            self.assertEqual(
+                std_out_lines[11],
+                '{0}One line.{1}'.format(
+                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(std_out_lines[12], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[13], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[14], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[15], '')
 
     @skipIf(not settings.DJANGO_EXPANDED_TESTCASES_DEBUG_PRINT, 'Test only works as expected with DEBUG PRINT.')
     def test__assertText_coloring__missing_characters(self):
@@ -381,25 +544,43 @@
             std_out_lines = std_out.getvalue().split('\n')[6:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
             self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[4],
+                '{0}EXPECTED:{1}'.format(
+                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(
                 std_out_lines[5],
-                '{0}esting.{1}'.format(ETC_OUTPUT_EXPECTED_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
+                '{0}esting.{1}'.format(
+                    ETC_OUTPUT_EXPECTED_ERROR_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
             )
             self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[8],
+                '{0}ACTUAL:{1}'.format(
+                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(
                 std_out_lines[9],
-                '{0}Testing.{1}'.format(ETC_OUTPUT_ACTUALS_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
+                '{0}Testing.{1}'.format(
+                    ETC_OUTPUT_ACTUALS_ERROR_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
             )
             self.assertEqual(std_out_lines[10], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[11], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[12], '')
 
         with self.subTest('With actuals as one char missing - At start'):
             std_out = StringIO()
@@ -409,25 +590,43 @@
             std_out_lines = std_out.getvalue().split('\n')[6:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
             self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[4],
+                '{0}EXPECTED:{1}'.format(
+                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(
                 std_out_lines[5],
-                '{0}Testing.{1}'.format(ETC_OUTPUT_EXPECTED_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
+                '{0}Testing.{1}'.format(
+                    ETC_OUTPUT_EXPECTED_ERROR_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
             )
             self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[8],
+                '{0}ACTUAL:{1}'.format(
+                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(
                 std_out_lines[9],
-                '{0}esting.{1}'.format(ETC_OUTPUT_ACTUALS_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
+                '{0}esting.{1}'.format(
+                    ETC_OUTPUT_ACTUALS_ERROR_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
             )
             self.assertEqual(std_out_lines[10], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[11], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[12], '')
 
         with self.subTest('With expected as multiple characters missing - At start'):
             std_out = StringIO()
@@ -437,25 +636,43 @@
             std_out_lines = std_out.getvalue().split('\n')[6:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
             self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[4],
+                '{0}EXPECTED:{1}'.format(
+                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(
                 std_out_lines[5],
-                '{0}sting.{1}'.format(ETC_OUTPUT_EXPECTED_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
+                '{0}sting.{1}'.format(
+                    ETC_OUTPUT_EXPECTED_ERROR_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
             )
             self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[8],
+                '{0}ACTUAL:{1}'.format(
+                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(
                 std_out_lines[9],
-                '{0}Testing.{1}'.format(ETC_OUTPUT_ACTUALS_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
+                '{0}Testing.{1}'.format(
+                    ETC_OUTPUT_ACTUALS_ERROR_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
             )
             self.assertEqual(std_out_lines[10], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[11], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[12], '')
 
         with self.subTest('With actuals as multiple characters missing - At start'):
             std_out = StringIO()
@@ -465,25 +682,43 @@
             std_out_lines = std_out.getvalue().split('\n')[6:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
             self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[4],
+                '{0}EXPECTED:{1}'.format(
+                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(
                 std_out_lines[5],
-                '{0}Testing.{1}'.format(ETC_OUTPUT_EXPECTED_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
+                '{0}Testing.{1}'.format(
+                    ETC_OUTPUT_EXPECTED_ERROR_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
             )
             self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[8],
+                '{0}ACTUAL:{1}'.format(
+                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(
                 std_out_lines[9],
-                '{0}sting.{1}'.format(ETC_OUTPUT_ACTUALS_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
+                '{0}sting.{1}'.format(
+                    ETC_OUTPUT_ACTUALS_ERROR_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
             )
             self.assertEqual(std_out_lines[10], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[11], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[12], '')
 
         with self.subTest('With expected as one char missing - At middle'):
             std_out = StringIO()
@@ -493,25 +728,45 @@
             std_out_lines = std_out.getvalue().split('\n')[6:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
             self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[4],
+                '{0}EXPECTED:{1}'.format(
+                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(
                 std_out_lines[5],
-                '{0}Tes{1}ing.{2}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_EXPECTED_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
+                '{0}Tes{1}ing.{2}'.format(
+                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                    ETC_OUTPUT_EXPECTED_ERROR_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
             )
             self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[8],
+                '{0}ACTUAL:{1}'.format(
+                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(
                 std_out_lines[9],
-                '{0}Tes{1}ting.{2}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_ACTUALS_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
+                '{0}Tes{1}ting.{2}'.format(
+                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                    ETC_OUTPUT_ACTUALS_ERROR_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
             )
             self.assertEqual(std_out_lines[10], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[11], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[12], '')
 
         with self.subTest('With actuals as one char missing - At middle'):
             std_out = StringIO()
@@ -521,25 +776,45 @@
             std_out_lines = std_out.getvalue().split('\n')[6:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
             self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[4],
+                '{0}EXPECTED:{1}'.format(
+                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(
                 std_out_lines[5],
-                '{0}Tes{1}ting.{2}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_EXPECTED_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
+                '{0}Tes{1}ting.{2}'.format(
+                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                    ETC_OUTPUT_EXPECTED_ERROR_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
             )
             self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[8],
+                '{0}ACTUAL:{1}'.format(
+                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(
                 std_out_lines[9],
-                '{0}Tes{1}ing.{2}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_ACTUALS_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
+                '{0}Tes{1}ing.{2}'.format(
+                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                    ETC_OUTPUT_ACTUALS_ERROR_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
             )
             self.assertEqual(std_out_lines[10], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[11], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[12], '')
 
         with self.subTest('With expected as multiple characters missing - At middle'):
             std_out = StringIO()
@@ -549,25 +824,45 @@
             std_out_lines = std_out.getvalue().split('\n')[6:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
             self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[4],
+                '{0}EXPECTED:{1}'.format(
+                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(
                 std_out_lines[5],
-                '{0}Te{1}ng.{2}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_EXPECTED_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
+                '{0}Te{1}ng.{2}'.format(
+                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                    ETC_OUTPUT_EXPECTED_ERROR_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
             )
             self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[8],
+                '{0}ACTUAL:{1}'.format(
+                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(
                 std_out_lines[9],
-                '{0}Te{1}sting.{2}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_ACTUALS_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
+                '{0}Te{1}sting.{2}'.format(
+                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                    ETC_OUTPUT_ACTUALS_ERROR_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
             )
             self.assertEqual(std_out_lines[10], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[11], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[12], '')
 
         with self.subTest('With actuals as multiple characters missing - At middle'):
             std_out = StringIO()
@@ -577,25 +872,45 @@
             std_out_lines = std_out.getvalue().split('\n')[6:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
             self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[4],
+                '{0}EXPECTED:{1}'.format(
+                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(
                 std_out_lines[5],
-                '{0}Te{1}sting.{2}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_EXPECTED_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
+                '{0}Te{1}sting.{2}'.format(
+                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                    ETC_OUTPUT_EXPECTED_ERROR_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
             )
             self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[8],
+                '{0}ACTUAL:{1}'.format(
+                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(
                 std_out_lines[9],
-                '{0}Te{1}ng.{2}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_ACTUALS_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
+                '{0}Te{1}ng.{2}'.format(
+                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                    ETC_OUTPUT_ACTUALS_ERROR_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
             )
             self.assertEqual(std_out_lines[10], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[11], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[12], '')
 
         with self.subTest('With expected as one char missing - At end'):
             std_out = StringIO()
@@ -605,25 +920,45 @@
             std_out_lines = std_out.getvalue().split('\n')[6:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
             self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[4],
+                '{0}EXPECTED:{1}'.format(
+                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(
                 std_out_lines[5],
-                '{0}Testing{1}{2}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_EXPECTED_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
+                '{0}Testing{1}{2}'.format(
+                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                    ETC_OUTPUT_EXPECTED_ERROR_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
             )
             self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[8],
+                '{0}ACTUAL:{1}'.format(
+                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(
                 std_out_lines[9],
-                '{0}Testing{1}.{2}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_ACTUALS_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
+                '{0}Testing{1}.{2}'.format(
+                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                    ETC_OUTPUT_ACTUALS_ERROR_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
             )
             self.assertEqual(std_out_lines[10], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[11], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[12], '')
 
         with self.subTest('With actuals as one char missing - At end'):
             std_out = StringIO()
@@ -633,25 +968,45 @@
             std_out_lines = std_out.getvalue().split('\n')[6:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
             self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[4],
+                '{0}EXPECTED:{1}'.format(
+                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(
                 std_out_lines[5],
-                '{0}Testing{1}.{2}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_EXPECTED_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
+                '{0}Testing{1}.{2}'.format(
+                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                    ETC_OUTPUT_EXPECTED_ERROR_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
             )
             self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[8],
+                '{0}ACTUAL:{1}'.format(
+                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(
                 std_out_lines[9],
-                '{0}Testing{1}{2}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_ACTUALS_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
+                '{0}Testing{1}{2}'.format(
+                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                    ETC_OUTPUT_ACTUALS_ERROR_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
             )
             self.assertEqual(std_out_lines[10], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[11], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[12], '')
 
         with self.subTest('With expected as multiple characters missing - At end'):
             std_out = StringIO()
@@ -661,25 +1016,45 @@
             std_out_lines = std_out.getvalue().split('\n')[5:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
             self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[4],
+                '{0}EXPECTED:{1}'.format(
+                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(
                 std_out_lines[5],
-                '{0}Test{1}{2}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_EXPECTED_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
+                '{0}Test{1}{2}'.format(
+                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                    ETC_OUTPUT_EXPECTED_ERROR_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
             )
             self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[8],
+                '{0}ACTUAL:{1}'.format(
+                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(
                 std_out_lines[9],
-                '{0}Test{1}ing.{2}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_ACTUALS_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
+                '{0}Test{1}ing.{2}'.format(
+                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                    ETC_OUTPUT_ACTUALS_ERROR_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
             )
             self.assertEqual(std_out_lines[10], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[11], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[12], '')
 
         with self.subTest('With actuals as multiple characters missing - At end'):
             std_out = StringIO()
@@ -689,25 +1064,45 @@
             std_out_lines = std_out.getvalue().split('\n')[5:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
             self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[4],
+                '{0}EXPECTED:{1}'.format(
+                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(
                 std_out_lines[5],
-                '{0}Test{1}ing.{2}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_EXPECTED_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
+                '{0}Test{1}ing.{2}'.format(
+                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                    ETC_OUTPUT_EXPECTED_ERROR_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
             )
             self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[8],
+                '{0}ACTUAL:{1}'.format(
+                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(
                 std_out_lines[9],
-                '{0}Test{1}{2}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_ACTUALS_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
+                '{0}Test{1}{2}'.format(
+                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                    ETC_OUTPUT_ACTUALS_ERROR_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
             )
             self.assertEqual(std_out_lines[10], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[11], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[12], '')
 
     @skipIf(not settings.DJANGO_EXPANDED_TESTCASES_DEBUG_PRINT, 'Test only works as expected with DEBUG PRINT.')
     def test__assertText_coloring__wrong_characters(self):
@@ -723,26 +1118,38 @@
             std_out_lines = std_out.getvalue().split('\n')[7:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
             self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[4],
+                '{0}EXPECTED:{1}'.format(
+                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(
                 std_out_lines[5],
                 '{0}a{1}BC{2}'.format(
                     ETC_OUTPUT_EXPECTED_ERROR_COLOR,
                     ETC_OUTPUT_EXPECTED_MATCH_COLOR,
                     ETC_OUTPUT_RESET_COLOR,
                 ),
             )
             self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[8],
+                '{0}ACTUAL:{1}'.format(
+                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(
                 std_out_lines[9],
                 '{0}A{1}BC{2}'.format(
                     ETC_OUTPUT_ACTUALS_ERROR_COLOR,
                     ETC_OUTPUT_ACTUALS_MATCH_COLOR,
                     ETC_OUTPUT_RESET_COLOR,
                 ),
@@ -759,26 +1166,38 @@
             std_out_lines = std_out.getvalue().split('\n')[7:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
             self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[4],
+                '{0}EXPECTED:{1}'.format(
+                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(
                 std_out_lines[5],
                 '{0}tHIS{1} is a test value.{2}'.format(
                     ETC_OUTPUT_EXPECTED_ERROR_COLOR,
                     ETC_OUTPUT_EXPECTED_MATCH_COLOR,
                     ETC_OUTPUT_RESET_COLOR,
                 ),
             )
             self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[8],
+                '{0}ACTUAL:{1}'.format(
+                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(
                 std_out_lines[9],
                 '{0}This{1} is a test value.{2}'.format(
                     ETC_OUTPUT_ACTUALS_ERROR_COLOR,
                     ETC_OUTPUT_ACTUALS_MATCH_COLOR,
                     ETC_OUTPUT_RESET_COLOR,
                 ),
@@ -795,26 +1214,38 @@
             std_out_lines = std_out.getvalue().split('\n')[7:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
             self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[4],
+                '{0}EXPECTED:{1}'.format(
+                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(
                 std_out_lines[5],
                 '{0}A{1}b{0}C{2}'.format(
                     ETC_OUTPUT_EXPECTED_MATCH_COLOR,
                     ETC_OUTPUT_EXPECTED_ERROR_COLOR,
                     ETC_OUTPUT_RESET_COLOR,
                 ),
             )
             self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[8],
+                '{0}ACTUAL:{1}'.format(
+                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(
                 std_out_lines[9],
                 '{0}A{1}B{0}C{2}'.format(
                     ETC_OUTPUT_ACTUALS_MATCH_COLOR,
                     ETC_OUTPUT_ACTUALS_ERROR_COLOR,
                     ETC_OUTPUT_RESET_COLOR,
                 ),
@@ -831,26 +1262,38 @@
             std_out_lines = std_out.getvalue().split('\n')[5:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
             self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[4],
+                '{0}EXPECTED:{1}'.format(
+                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(
                 std_out_lines[5],
                 '{0}This {1}IS{0} {1}A{0} {1}TEST{0} value.{2}'.format(
                     ETC_OUTPUT_EXPECTED_MATCH_COLOR,
                     ETC_OUTPUT_EXPECTED_ERROR_COLOR,
                     ETC_OUTPUT_RESET_COLOR,
                 ),
             )
             self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[8],
+                '{0}ACTUAL:{1}'.format(
+                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(
                 std_out_lines[9],
                 '{0}This {1}is{0} {1}a{0} {1}test{0} value.{2}'.format(
                     ETC_OUTPUT_ACTUALS_MATCH_COLOR,
                     ETC_OUTPUT_ACTUALS_ERROR_COLOR,
                     ETC_OUTPUT_RESET_COLOR,
                 ),
@@ -867,26 +1310,38 @@
             std_out_lines = std_out.getvalue().split('\n')[7:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
             self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[4],
+                '{0}EXPECTED:{1}'.format(
+                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(
                 std_out_lines[5],
                 '{0}AB{1}c{2}'.format(
                     ETC_OUTPUT_EXPECTED_MATCH_COLOR,
                     ETC_OUTPUT_EXPECTED_ERROR_COLOR,
                     ETC_OUTPUT_RESET_COLOR,
                 ),
             )
             self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[8],
+                '{0}ACTUAL:{1}'.format(
+                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(
                 std_out_lines[9],
                 '{0}AB{1}C{2}'.format(
                     ETC_OUTPUT_ACTUALS_MATCH_COLOR,
                     ETC_OUTPUT_ACTUALS_ERROR_COLOR,
                     ETC_OUTPUT_RESET_COLOR,
                 ),
@@ -903,26 +1358,38 @@
             std_out_lines = std_out.getvalue().split('\n')[5:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
             self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[4],
+                '{0}EXPECTED:{1}'.format(
+                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(
                 std_out_lines[5],
                 '{0}This is a test {1}VALUE!{2}'.format(
                     ETC_OUTPUT_EXPECTED_MATCH_COLOR,
                     ETC_OUTPUT_EXPECTED_ERROR_COLOR,
                     ETC_OUTPUT_RESET_COLOR,
                 ),
             )
             self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
-            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[8],
+                '{0}ACTUAL:{1}'.format(
+                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
+                ),
+            )
             self.assertEqual(
                 std_out_lines[9],
                 '{0}This is a test {1}value.{2}'.format(
                     ETC_OUTPUT_ACTUALS_MATCH_COLOR,
                     ETC_OUTPUT_ACTUALS_ERROR_COLOR,
                     ETC_OUTPUT_RESET_COLOR,
                 ),
@@ -985,23 +1452,23 @@
 
         with self.subTest('Large string'):
             # Full lorem.
             self.assertTextStartsWith(lorem_str, lorem_str)
 
             # Substring match.
             lorem_len = len(lorem_str)
-            self.assertTextStartsWith(lorem_str[:int(lorem_len - 1)], lorem_str)
-            self.assertTextStartsWith(lorem_str[:int(lorem_len - 2)], lorem_str)
-            self.assertTextStartsWith(lorem_str[:int(lorem_len - 3)], lorem_str)
-            self.assertTextStartsWith(lorem_str[:int(lorem_len - 4)], lorem_str)
-            self.assertTextStartsWith(lorem_str[:int(lorem_len - 5)], lorem_str)
-            self.assertTextStartsWith(lorem_str[:int(lorem_len / 2)], lorem_str)
-            self.assertTextStartsWith(lorem_str[:int(lorem_len / 3)], lorem_str)
-            self.assertTextStartsWith(lorem_str[:int(lorem_len / 4)], lorem_str)
-            self.assertTextStartsWith(lorem_str[:int(lorem_len / 5)], lorem_str)
+            self.assertTextStartsWith(lorem_str[: int(lorem_len - 1)], lorem_str)
+            self.assertTextStartsWith(lorem_str[: int(lorem_len - 2)], lorem_str)
+            self.assertTextStartsWith(lorem_str[: int(lorem_len - 3)], lorem_str)
+            self.assertTextStartsWith(lorem_str[: int(lorem_len - 4)], lorem_str)
+            self.assertTextStartsWith(lorem_str[: int(lorem_len - 5)], lorem_str)
+            self.assertTextStartsWith(lorem_str[: int(lorem_len / 2)], lorem_str)
+            self.assertTextStartsWith(lorem_str[: int(lorem_len / 3)], lorem_str)
+            self.assertTextStartsWith(lorem_str[: int(lorem_len / 4)], lorem_str)
+            self.assertTextStartsWith(lorem_str[: int(lorem_len / 5)], lorem_str)
 
     def test__assertTextStartsWith__fail(self):
         """
         Tests assertTextStartsWith() function, in cases when it should fail.
         """
         exception_msg = '\'{0}\' != \'{1}\'\n- {0}\n{2}+ {1}\n{3}'
 
@@ -1012,71 +1479,110 @@
 
             with self.assertRaises(AssertionError) as err:
                 self.assertTextStartsWith('a', 'A')
             self.assertEqual(exception_msg.format('a', 'A', '', ''), str(err.exception))
 
             with self.assertRaises(AssertionError) as err:
                 self.assertTextStartsWith('a', 1)
-            self.assertEqual( exception_msg.format('a', '1', '', ''), str(err.exception))
+            self.assertEqual(exception_msg.format('a', '1', '', ''), str(err.exception))
 
         with self.subTest('Whitespace mismatch'):
             with self.assertRaises(AssertionError) as err:
                 self.assertTextStartsWith('a b c', 'abc')
-            self.assertEqual(exception_msg.format('a b c', 'abc', '?  - -\n', ''), str(err.exception))
+            self.assertEqual(
+                exception_msg.format(
+                    'a b c',
+                    'abc',
+                    '?  - -\n',
+                    '',
+                ),
+                str(err.exception),
+            )
             with self.assertRaises(AssertionError) as err:
                 self.assertTextStartsWith('a b', 'abc')
-            self.assertEqual(exception_msg.format('a b', 'abc', '?  -\n', '?   +\n'), str(err.exception))
+            self.assertEqual(
+                exception_msg.format(
+                    'a b',
+                    'abc',
+                    '?  -\n',
+                    '?   +\n',
+                ),
+                str(err.exception),
+            )
 
             with self.assertRaises(AssertionError) as err:
                 self.assertTextStartsWith('abc', 'a b c')
-            self.assertEqual(exception_msg.format('abc', 'a b c', '', '?  + +\n'), str(err.exception))
+            self.assertEqual(
+                exception_msg.format(
+                    'abc',
+                    'a b c',
+                    '',
+                    '?  + +\n',
+                ),
+                str(err.exception),
+            )
             with self.assertRaises(AssertionError) as err:
                 self.assertTextStartsWith('ab', 'a b c')
             self.assertEqual(exception_msg.format('ab', 'a b c', '', ''), str(err.exception))
 
         with self.subTest('Inner value mismatch'):
             with self.assertRaises(AssertionError) as err:
                 self.assertTextStartsWith('This is a test sentence.', 'This is test sentence.')
             self.assertEqual(
-                exception_msg.format('This is a test sentence.', 'This is test sentence.', '?        --\n', ''),
+                exception_msg.format(
+                    'This is a test sentence.',
+                    'This is test sentence.',
+                    '?        --\n',
+                    '',
+                ),
                 str(err.exception),
             )
 
             with self.assertRaises(AssertionError) as err:
                 self.assertTextStartsWith('This is a test sentence.', 'test sentence.')
             self.assertEqual(
-                exception_msg.format('This is a test sentence.', 'test sentence.', '? ----------\n', ''),
+                exception_msg.format(
+                    'This is a test sentence.',
+                    'test sentence.',
+                    '? ----------\n',
+                    '',
+                ),
                 str(err.exception),
             )
 
             with self.assertRaises(AssertionError) as err:
                 self.assertTextStartsWith('This is a test sentence.', 'This is a test.')
             self.assertEqual(
-                exception_msg.format('This is a test sentence.', 'This is a test.', '?               ---------\n', ''),
+                exception_msg.format(
+                    'This is a test sentence.',
+                    'This is a test.',
+                    '?               ---------\n',
+                    '',
+                ),
                 str(err.exception),
             )
 
         with self.subTest('Large string'):
             half_lorem_len = int(len(lorem_str) / 2)
 
             # With character replaced.
             with self.assertRaises(AssertionError) as err:
-                modified_str = lorem_str[:(half_lorem_len - 1)] + 'z' + lorem_str[(half_lorem_len + 1):]
+                modified_str = lorem_str[: (half_lorem_len - 1)] + 'z' + lorem_str[(half_lorem_len + 1) :]
                 self.assertTextStartsWith(lorem_str, modified_str)
             # self.assertEqual(str(err.exception), exception_msg)
 
             # With character added.
             with self.assertRaises(AssertionError) as err:
-                modified_str = lorem_str[:(half_lorem_len)] + 'z' + lorem_str[(half_lorem_len + 1):]
+                modified_str = lorem_str[:(half_lorem_len)] + 'z' + lorem_str[(half_lorem_len + 1) :]
                 self.assertTextStartsWith(lorem_str, modified_str)
             # self.assertEqual(str(err.exception), exception_msg)
 
             # With character removed.
             with self.assertRaises(AssertionError) as err:
-                modified_str = lorem_str[:(half_lorem_len - 1)] + lorem_str[(half_lorem_len + 1):]
+                modified_str = lorem_str[: (half_lorem_len - 1)] + lorem_str[(half_lorem_len + 1) :]
                 self.assertTextStartsWith(lorem_str, modified_str)
             # self.assertEqual(str(err.exception), exception_msg)
 
     def test__assertTextEndsWith__success(self):
         """
         Tests assertTextEndsWith() function, in cases when it should succeed.
         """
@@ -1130,23 +1636,23 @@
 
         with self.subTest('Large string'):
             # Full lorem.
             self.assertTextEndsWith(lorem_str, lorem_str)
 
             # Substring match.
             lorem_len = len(lorem_str)
-            self.assertTextEndsWith(lorem_str[int(lorem_len - 1):], lorem_str)
-            self.assertTextEndsWith(lorem_str[int(lorem_len - 2):], lorem_str)
-            self.assertTextEndsWith(lorem_str[int(lorem_len - 3):], lorem_str)
-            self.assertTextEndsWith(lorem_str[int(lorem_len - 4):], lorem_str)
-            self.assertTextEndsWith(lorem_str[int(lorem_len - 5):], lorem_str)
-            self.assertTextEndsWith(lorem_str[int(lorem_len / 2):], lorem_str)
-            self.assertTextEndsWith(lorem_str[int(lorem_len / 3):], lorem_str)
-            self.assertTextEndsWith(lorem_str[int(lorem_len / 4):], lorem_str)
-            self.assertTextEndsWith(lorem_str[int(lorem_len / 5):], lorem_str)
+            self.assertTextEndsWith(lorem_str[int(lorem_len - 1) :], lorem_str)
+            self.assertTextEndsWith(lorem_str[int(lorem_len - 2) :], lorem_str)
+            self.assertTextEndsWith(lorem_str[int(lorem_len - 3) :], lorem_str)
+            self.assertTextEndsWith(lorem_str[int(lorem_len - 4) :], lorem_str)
+            self.assertTextEndsWith(lorem_str[int(lorem_len - 5) :], lorem_str)
+            self.assertTextEndsWith(lorem_str[int(lorem_len / 2) :], lorem_str)
+            self.assertTextEndsWith(lorem_str[int(lorem_len / 3) :], lorem_str)
+            self.assertTextEndsWith(lorem_str[int(lorem_len / 4) :], lorem_str)
+            self.assertTextEndsWith(lorem_str[int(lorem_len / 5) :], lorem_str)
 
     def test__assertTextEndsWith__fail(self):
         """
         Tests assertTextEndsWith() function, in cases when it should fail.
         """
         exception_msg = '\'{0}\' != \'{1}\'\n- {0}\n{2}+ {1}\n{3}'
 
@@ -1162,19 +1668,35 @@
             with self.assertRaises(AssertionError) as err:
                 self.assertTextEndsWith('a', 1)
             self.assertEqual(exception_msg.format('a', '1', '', ''), str(err.exception))
 
         with self.subTest('Whitespace mismatch'):
             with self.assertRaises(AssertionError) as err:
                 self.assertTextEndsWith('a b c', 'abc')
-            self.assertEqual(exception_msg.format('a b c', 'abc', '?  - -\n', ''), str(err.exception))
+            self.assertEqual(
+                exception_msg.format(
+                    'a b c',
+                    'abc',
+                    '?  - -\n',
+                    '',
+                ),
+                str(err.exception),
+            )
 
             with self.assertRaises(AssertionError) as err:
                 self.assertTextEndsWith('abc', 'a b c')
-            self.assertEqual(exception_msg.format('abc', 'a b c', '', '?  + +\n'), str(err.exception))
+            self.assertEqual(
+                exception_msg.format(
+                    'abc',
+                    'a b c',
+                    '',
+                    '?  + +\n',
+                ),
+                str(err.exception),
+            )
 
         with self.subTest('Inner value mismatch'):
             with self.assertRaises(AssertionError) as err:
                 self.assertTextEndsWith('This is a test sentence.', 'This is a test')
             self.assertEqual(
                 exception_msg.format(
                     'This is a test sentence.',
@@ -1184,50 +1706,65 @@
                 ),
                 str(err.exception),
             )
 
             with self.assertRaises(AssertionError) as err:
                 self.assertTextEndsWith('This is a test sentence.', 'This is test sentence.')
             self.assertEqual(
-                exception_msg.format('This is a test sentence.', 'This is test sentence.', '?        --\n', ''),
+                exception_msg.format(
+                    'This is a test sentence.',
+                    'This is test sentence.',
+                    '?        --\n',
+                    '',
+                ),
                 str(err.exception),
             )
 
             with self.assertRaises(AssertionError) as err:
                 self.assertTextEndsWith('This is a test sentence.', 'test sentence.')
             self.assertEqual(
-                exception_msg.format('This is a test sentence.', 'test sentence.', '? ----------\n', ''),
+                exception_msg.format(
+                    'This is a test sentence.',
+                    'test sentence.',
+                    '? ----------\n',
+                    '',
+                ),
                 str(err.exception),
             )
 
             with self.assertRaises(AssertionError) as err:
                 self.assertTextEndsWith('This is a test sentence.', 'This is a test.')
             self.assertEqual(
-                exception_msg.format('This is a test sentence.', 'This is a test.', '?               ---------\n', ''),
+                exception_msg.format(
+                    'This is a test sentence.',
+                    'This is a test.',
+                    '?               ---------\n',
+                    '',
+                ),
                 str(err.exception),
             )
 
         with self.subTest('Large string'):
             half_lorem_len = int(len(lorem_str) / 2)
 
             # With character replaced.
             with self.assertRaises(AssertionError) as err:
-                modified_str = lorem_str[:(half_lorem_len - 1)] + 'z' + lorem_str[(half_lorem_len + 1):]
+                modified_str = lorem_str[: (half_lorem_len - 1)] + 'z' + lorem_str[(half_lorem_len + 1) :]
                 self.assertTextEndsWith(lorem_str, modified_str)
             # self.assertEqual(str(err.exception), exception_msg)
 
             # With character added.
             with self.assertRaises(AssertionError) as err:
-                modified_str = lorem_str[:(half_lorem_len)] + 'z' + lorem_str[(half_lorem_len + 1):]
+                modified_str = lorem_str[:(half_lorem_len)] + 'z' + lorem_str[(half_lorem_len + 1) :]
                 self.assertTextEndsWith(lorem_str, modified_str)
             # self.assertEqual(str(err.exception), exception_msg)
 
             # With character removed.
             with self.assertRaises(AssertionError) as err:
-                modified_str = lorem_str[:(half_lorem_len - 1)] + lorem_str[(half_lorem_len + 1):]
+                modified_str = lorem_str[: (half_lorem_len - 1)] + lorem_str[(half_lorem_len + 1) :]
                 self.assertTextEndsWith(lorem_str, modified_str)
             # self.assertEqual(str(err.exception), exception_msg)
 
     # endregion Assertion Tests
 
     # region User Management Function Tests
 
@@ -1942,15 +2479,16 @@
                 '&#92; &#x5C; &#x5c; &bsol; \\',
                 '\\ \\ \\ \\ \\',
             )
 
         with self.subTest('Test closing square bracket'):
             self.assert_symbol_standardization(
                 '&#93; &#x5D; &#x5d; &rbrack; ]',
-                '] ] ] ] ]',)
+                '] ] ] ] ]',
+            )
 
         with self.subTest('Test up arrow'):
             self.assert_symbol_standardization(
                 '&#94; &#x5E; &#x5e; &Hat; ^',
                 '^ ^ ^ ^ ^',
             )
 
@@ -2657,14 +3195,15 @@
 
 
 class BaseClassTest_WithRealNames(BaseTestCase):
     """Tests for BaseTestCase class, when using settings to generate users with real names.
 
     Required as a separate class, since user generation is handled on class initialization.
     """
+
     @classmethod
     @patch('django_expanded_test_cases.mixins.core_mixin.ETC_GENERATE_USERS_WITH_REAL_NAMES', True)
     def setUpTestData(cls):
         # Call parent logic.
         super().setUpTestData()
 
     def test__get_user__with_real_names(self):
```

### Comparing `django-expanded-test-cases-0.7.0/etc_tests/test_cases/test_channels_live_server_case.py` & `django_expanded_test_cases-0.7.1/etc_tests/test_cases/test_channels_live_server_case.py`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.7.0/etc_tests/test_cases/test_integration_case.py` & `django_expanded_test_cases-0.7.1/etc_tests/test_cases/test_integration_case.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,27 +13,35 @@
 from django.core.exceptions import ValidationError
 from django.http import HttpResponse
 from django.test import override_settings
 from django.urls import reverse
 
 # Internal Imports.
 from django_expanded_test_cases import IntegrationTestCase
+from django_expanded_test_cases.constants import (
+    COLORAMA_PRESENT,
+    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+    ETC_OUTPUT_ERROR_COLOR,
+    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+    ETC_OUTPUT_RESET_COLOR,
+)
 
 
 class IntegrationClassTest__Base(IntegrationTestCase):
     """Tests for IntegrationTestCase class."""
 
     # region Assertion Tests
 
     # region Response Assertion Tests
 
     def test__assertResponse__url(self):
         """
         Tests URL value returned response object in assertResponse() function.
         """
+
         with self.subTest('With no site_root_url value defined - Via literal value'):
             # Test 404 page url.
             response = self.assertResponse('bad_url', expected_status=404)
             self.assertText('/bad_url/', response.url)
             self.assertText('127.0.0.1/bad_url/', response.full_url)
             response = self.assertResponse('bad_url/', expected_status=404)
             self.assertText('/bad_url/', response.url)
@@ -192,24 +200,30 @@
             self.assertText('/user/detail/2/', response.url)
             self.assertText('127.0.0.1/user/detail/2/', response.full_url)
 
             # Test "user detail" page url via args plus query params.
             response = self.assertResponse(
                 'django_expanded_test_cases:user-detail',
                 args=(1,),
-                url_query_params={'test_1': 'aaa', 'test_2': 'bbb'},
+                url_query_params={
+                    'test_1': 'aaa',
+                    'test_2': 'bbb',
+                },
             )
             self.assertText('/user/detail/1/?test_1=aaa&test_2=bbb', response.url)
             self.assertText('127.0.0.1/user/detail/1/?test_1=aaa&test_2=bbb', response.full_url)
 
             # Test "user detail" page url via kwargs plus query params.
             response = self.assertResponse(
                 'django_expanded_test_cases:user-detail',
                 kwargs={'pk': 2},
-                url_query_params={'test_1': 'aaa', 'test_2': 'bbb'},
+                url_query_params={
+                    'test_1': 'aaa',
+                    'test_2': 'bbb',
+                },
             )
             self.assertText('/user/detail/2/?test_1=aaa&test_2=bbb', response.url)
             self.assertText('127.0.0.1/user/detail/2/?test_1=aaa&test_2=bbb', response.full_url)
 
         with self.subTest('With no site_root_url value defined - Via url_args/url_kwargs'):
 
             # Test "user detail" page url via args.
@@ -222,24 +236,30 @@
             self.assertText('/user/detail/2/', response.url)
             self.assertText('127.0.0.1/user/detail/2/', response.full_url)
 
             # Test "user detail" page url via args plus query params.
             response = self.assertResponse(
                 'django_expanded_test_cases:user-detail',
                 url_args=(1,),
-                url_query_params={'test_1': 'aaa', 'test_2': 'bbb'},
+                url_query_params={
+                    'test_1': 'aaa',
+                    'test_2': 'bbb',
+                },
             )
             self.assertText('/user/detail/1/?test_1=aaa&test_2=bbb', response.url)
             self.assertText('127.0.0.1/user/detail/1/?test_1=aaa&test_2=bbb', response.full_url)
 
             # Test "user detail" page url via kwargs plus query params.
             response = self.assertResponse(
                 'django_expanded_test_cases:user-detail',
                 url_kwargs={'pk': 2},
-                url_query_params={'test_1': 'aaa', 'test_2': 'bbb'},
+                url_query_params={
+                    'test_1': 'aaa',
+                    'test_2': 'bbb',
+                },
             )
             self.assertText('/user/detail/2/?test_1=aaa&test_2=bbb', response.url)
             self.assertText('127.0.0.1/user/detail/2/?test_1=aaa&test_2=bbb', response.full_url)
 
         with self.subTest('With no site_root_url value defined - Via reverse()'):
 
             # Test "user detail" page url via args.
@@ -271,24 +291,30 @@
         with self.subTest('With custom site_root_url value defined'):
             self.site_root_url = 'https://my_really_cool_site.com/'
 
             # Test "user detail" page url via args.
             response = self.assertResponse(
                 'django_expanded_test_cases:user-detail',
                 args=(1,),
-                url_query_params={'test_1': 'aaa', 'test_2': 'bbb'},
+                url_query_params={
+                    'test_1': 'aaa',
+                    'test_2': 'bbb',
+                },
             )
             self.assertText('/user/detail/1/?test_1=aaa&test_2=bbb', response.url)
             self.assertText('https://my_really_cool_site.com/user/detail/1/?test_1=aaa&test_2=bbb', response.full_url)
 
             # Test "user detail" page url via kwargs.
             response = self.assertResponse(
                 'django_expanded_test_cases:user-detail',
                 kwargs={'pk': 2},
-                url_query_params={'test_1': 'aaa', 'test_2': 'bbb'},
+                url_query_params={
+                    'test_1': 'aaa',
+                    'test_2': 'bbb',
+                },
             )
             self.assertText('/user/detail/2/?test_1=aaa&test_2=bbb', response.url)
             self.assertText('https://my_really_cool_site.com/user/detail/2/?test_1=aaa&test_2=bbb', response.full_url)
 
     def test__assertResponse__url__with_query_params(self):
         """
         Tests URL value returned response object in assertResponse() function.
@@ -379,165 +405,170 @@
                 expected_redirect_url='django_expanded_test_cases:index',
             )
 
         with self.subTest('With view that does not redirect'):
             # Using direct url.
             self.assertResponse('')
             with self.assertRaises(AssertionError) as err:
-                self.assertResponse('', expected_redirect_url='/')
+                self.assertResponse(
+                    '',
+                    expected_redirect_url='/',
+                )
             self.assertText(exception_msg, str(err.exception))
             with self.assertRaises(AssertionError) as err:
-                self.assertResponse('', expected_redirect_url='django_expanded_test_cases:index')
+                self.assertResponse(
+                    '',
+                    expected_redirect_url='django_expanded_test_cases:index',
+                )
             self.assertText(exception_msg, str(err.exception))
             with self.assertRaises(AssertionError) as err:
-                self.assertResponse('login/', expected_redirect_url='django_expanded_test_cases:index')
+                self.assertResponse(
+                    'login/',
+                    expected_redirect_url='django_expanded_test_cases:index',
+                )
             self.assertText(exception_msg, str(err.exception))
 
             # Using reverse.
             self.assertResponse('django_expanded_test_cases:index')
             with self.assertRaises(AssertionError) as err:
-                self.assertResponse('django_expanded_test_cases:index', expected_redirect_url='/')
+                self.assertResponse(
+                    'django_expanded_test_cases:index',
+                    expected_redirect_url='/',
+                )
             self.assertText(exception_msg, str(err.exception))
             with self.assertRaises(AssertionError) as err:
-                self.assertResponse('django_expanded_test_cases:index', expected_redirect_url='django_expanded_test_cases:index')
+                self.assertResponse(
+                    'django_expanded_test_cases:index',
+                    expected_redirect_url='django_expanded_test_cases:index',
+                )
             self.assertText(exception_msg, str(err.exception))
             with self.assertRaises(AssertionError) as err:
-                self.assertResponse('django_expanded_test_cases:login', expected_redirect_url='django_expanded_test_cases:index')
+                self.assertResponse(
+                    'django_expanded_test_cases:login',
+                    expected_redirect_url='django_expanded_test_cases:index',
+                )
             self.assertText(exception_msg, str(err.exception))
 
     def test__assertResponse__url_redirect__with_args(self):
         """
         Tests "url_redirect" functionality of assertResponse() function,
         when accessing a view via url args.
         """
 
         with self.subTest('Provide via standard reverse'):
 
             # Reverse, as args.
             self.assertResponse(
-
                 # Standard url reverse, as the passed url.
                 reverse(
                     'django_expanded_test_cases:redirect-with-args',
                     args=(1, 'As standard url reverse() args'),
                 ),
-
                 # Url we expect to end up at.
                 expected_redirect_url=reverse(
                     'django_expanded_test_cases:template-response-with-args',
                     args=(1, 'As standard url reverse() args'),
                 ),
-
                 # Expected content on final page.
                 expected_content=[
                     'id: "1"',
                     'name: "As standard url reverse() args"',
                 ],
             )
 
             # Reverse, as kwargs.
             self.assertResponse(
-
                 # Standard url reverse, as the passed url.
                 reverse(
                     'django_expanded_test_cases:redirect-with-args',
-                    kwargs={'id': 2, 'name': 'As standard url reverse() kwargs'},
+                    kwargs={
+                        'id': 2,
+                        'name': 'As standard url reverse() kwargs',
+                    },
                 ),
-
                 # Url we expect to end up at.
                 expected_redirect_url=reverse(
                     'django_expanded_test_cases:template-response-with-args',
-                    kwargs={'id': 2, 'name': 'As standard url reverse() kwargs'},
+                    kwargs={
+                        'id': 2,
+                        'name': 'As standard url reverse() kwargs',
+                    },
                 ),
-
                 # Expected content on final page.
                 expected_content=[
                     'id: "2"',
                     'name: "As standard url reverse() kwargs"',
                 ],
             )
 
         with self.subTest('Provide via individually passed values'):
 
             # As args.
             self.assertResponse(
-
                 # Desired url, as standard reverse string.
                 'django_expanded_test_cases:redirect-with-args',
-
                 # Individual args to use for url.
                 3,
                 'As passed args',
-
                 # Url we expect to end up at.
                 expected_redirect_url=reverse(
                     'django_expanded_test_cases:template-response-with-args',
                     args=(3, 'As passed args'),
                 ),
-
                 # Expected content on final page.
                 expected_content=[
                     'id: "3"',
                     'name: "As passed args"',
                 ],
             )
 
             # As kwargs.
             self.assertResponse(
                 # Desired url, as standard reverse string.
                 'django_expanded_test_cases:redirect-with-args',
-
                 # Url we expect to end up at.
                 expected_redirect_url=reverse(
                     'django_expanded_test_cases:template-response-with-args',
                     args=(6, 'As individually passed kwargs'),
                 ),
-
                 # Individual args to use for url.
                 id=6,
                 name='As individually passed kwargs',
-
                 # Expected content on final page.
                 expected_content=[
                     'id: "6"',
                     'name: "As individually passed kwargs"',
                 ],
             )
 
         with self.subTest('Provide via args keyword'):
             self.assertResponse(
                 # Desired url, as standard reverse string.
                 'django_expanded_test_cases:redirect-with-args',
-
                 # Url we expect to end up at.
                 expected_redirect_url='django_expanded_test_cases:template-response-with-args',
-
                 # Args for url.
                 url_args=[4, 'As url_args'],
                 redirect_args=(4, 'As url_args'),
-
                 # Expected content on final page.
                 expected_content=[
                     'id: "4"',
                     'name: "As url_args"',
                 ],
             )
 
         with self.subTest('Provide via kwargs keyword'):
             self.assertResponse(
                 # Desired url, as standard reverse string.
                 'django_expanded_test_cases:redirect-with-args',
-
                 # Url we expect to end up at.
                 expected_redirect_url='django_expanded_test_cases:template-response-with-args',
-
                 # Args for url.
                 url_kwargs={'id': 5, 'name': 'As redirect_args'},
                 redirect_kwargs={'id': 5, 'name': 'As redirect_args'},
-
                 # Expected content on final page.
                 expected_content=[
                     'id: "5"',
                     'name: "As redirect_args"',
                 ],
             )
 
@@ -581,26 +612,563 @@
 
         with self.subTest('With status_code=404'):
             # Test 404 in direct url.
             response = self.assertResponse('bad_url', expected_status=404)
             self.assertEqual(response.status_code, 404)
 
             # Test 404 in reverse() url, via args.
-            response = self.assertResponse('django_expanded_test_cases:user-detail', args=(234,), expected_status=404)
+            response = self.assertResponse(
+                'django_expanded_test_cases:user-detail',
+                args=(234,),
+                expected_status=404,
+            )
             self.assertEqual(response.status_code, 404)
 
             # Test 404 in reverse() url, via kwargs.
-            response = self.assertResponse('django_expanded_test_cases:user-detail', kwargs={'pk': 345}, expected_status=404)
+            response = self.assertResponse(
+                'django_expanded_test_cases:user-detail',
+                kwargs={'pk': 345},
+                expected_status=404,
+            )
             self.assertEqual(response.status_code, 404)
 
             # With non-404 code provided.
             with self.assertRaises(AssertionError) as err:
                 self.assertResponse('bad_url', expected_status=200)
             self.assertText(exception_msg.format(404, 200), str(err.exception))
 
+    def test__assertResponse__expected_url(self):
+        """
+        Tests "expected_url" functionality of assertResponse() function.
+        """
+
+        with self.subTest('With no site_root_url value defined - Via literal value'):
+            # Test 404 page url.
+            response = self.assertResponse('bad_url', expected_url='/bad_url/', expected_status=404)
+            self.assertText('/bad_url/', response.url)
+            self.assertText('127.0.0.1/bad_url/', response.full_url)
+            response = self.assertResponse('bad_url/', expected_url='/bad_url/', expected_status=404)
+            self.assertText('/bad_url/', response.url)
+            self.assertText('127.0.0.1/bad_url/', response.full_url)
+            response = self.assertResponse('127.0.0.1/bad_url/', expected_url='/bad_url/', expected_status=404)
+            self.assertText('/bad_url/', response.url)
+            self.assertText('127.0.0.1/bad_url/', response.full_url)
+            response = self.assertResponse('///bad_url///', expected_url='/bad_url/', expected_status=404)
+            self.assertText('/bad_url/', response.url)
+            self.assertText('127.0.0.1/bad_url/', response.full_url)
+
+            # Test "index" page url.
+            response = self.assertResponse('', expected_url='/')
+            self.assertText('/', response.url)
+            self.assertText('127.0.0.1/', response.full_url)
+            response = self.assertResponse('/', expected_url='/')
+            self.assertText('/', response.url)
+            self.assertText('127.0.0.1/', response.full_url)
+            response = self.assertResponse('127.0.0.1/', expected_url='/')
+            self.assertText('/', response.url)
+            self.assertText('127.0.0.1/', response.full_url)
+
+            # Test "login" page url.
+            response = self.assertResponse('login/', expected_url='/login/')
+            self.assertText('/login/', response.url)
+            self.assertText('127.0.0.1/login/', response.full_url)
+            response = self.assertResponse('/login/', expected_url='/login/')
+            self.assertText('/login/', response.url)
+            self.assertText('127.0.0.1/login/', response.full_url)
+            response = self.assertResponse('127.0.0.1/login/', expected_url='/login/')
+            self.assertText('/login/', response.url)
+            self.assertText('127.0.0.1/login/', response.full_url)
+
+            # Test "one message" page url.
+            response = self.assertResponse('views/one-message/', expected_url='/views/one-message/')
+            self.assertText('/views/one-message/', response.url)
+            self.assertText('127.0.0.1/views/one-message/', response.full_url)
+            response = self.assertResponse('/views/one-message/', expected_url='/views/one-message/')
+            self.assertText('/views/one-message/', response.url)
+            self.assertText('127.0.0.1/views/one-message/', response.full_url)
+            response = self.assertResponse('127.0.0.1/views/one-message/', expected_url='/views/one-message/')
+            self.assertText('/views/one-message/', response.url)
+            self.assertText('127.0.0.1/views/one-message/', response.full_url)
+
+            # Test "two messages" page url.
+            response = self.assertResponse('views/two-messages/', expected_url='/views/two-messages/')
+            self.assertText('/views/two-messages/', response.url)
+            self.assertText('127.0.0.1/views/two-messages/', response.full_url)
+            response = self.assertResponse('/views/two-messages/', expected_url='/views/two-messages/')
+            self.assertText('/views/two-messages/', response.url)
+            self.assertText('127.0.0.1/views/two-messages/', response.full_url)
+            response = self.assertResponse('127.0.0.1/views/two-messages/', expected_url='/views/two-messages/')
+            self.assertText('/views/two-messages/', response.url)
+            self.assertText('127.0.0.1/views/two-messages/', response.full_url)
+
+            # Test "three messages" page url.
+            response = self.assertResponse('views/three-messages/', expected_url='/views/three-messages/')
+            self.assertText('/views/three-messages/', response.url)
+            self.assertText('127.0.0.1/views/three-messages/', response.full_url)
+            response = self.assertResponse('/views/three-messages/', expected_url='/views/three-messages/')
+            self.assertText('/views/three-messages/', response.url)
+            self.assertText('127.0.0.1/views/three-messages/', response.full_url)
+            response = self.assertResponse('127.0.0.1/views/three-messages/', expected_url='/views/three-messages/')
+            self.assertText('/views/three-messages/', response.url)
+            self.assertText('127.0.0.1/views/three-messages/', response.full_url)
+
+            # Test "user detail" page url via args.
+            response = self.assertResponse('user/detail/1/', expected_url='/user/detail/1/')
+            self.assertText('/user/detail/1/', response.url)
+            self.assertText('127.0.0.1/user/detail/1/', response.full_url)
+            response = self.assertResponse('/user/detail/1/', expected_url='/user/detail/1/')
+            self.assertText('/user/detail/1/', response.url)
+            self.assertText('127.0.0.1/user/detail/1/', response.full_url)
+            response = self.assertResponse('127.0.0.1/user/detail/1/', expected_url='/user/detail/1/')
+            self.assertText('/user/detail/1/', response.url)
+            self.assertText('127.0.0.1/user/detail/1/', response.full_url)
+
+            # Test "user detail" page url via kwargs.
+            response = self.assertResponse('user/detail/2/', expected_url='/user/detail/2/')
+            self.assertText('/user/detail/2/', response.url)
+            self.assertText('127.0.0.1/user/detail/2/', response.full_url)
+            response = self.assertResponse('/user/detail/2/', expected_url='/user/detail/2/')
+            self.assertText('/user/detail/2/', response.url)
+            self.assertText('127.0.0.1/user/detail/2/', response.full_url)
+            response = self.assertResponse('127.0.0.1/user/detail/2/', expected_url='/user/detail/2/')
+            self.assertText('/user/detail/2/', response.url)
+            self.assertText('127.0.0.1/user/detail/2/', response.full_url)
+
+        with self.subTest('With no site_root_url value defined - Via reverse()'):
+            # Test "index" page url.
+            response = self.assertResponse('django_expanded_test_cases:index', expected_url='/')
+            self.assertText('/', response.url)
+            self.assertText('127.0.0.1/', response.full_url)
+
+            # Test "login" page url.
+            response = self.assertResponse('django_expanded_test_cases:login', expected_url='/login/')
+            self.assertText('/login/', response.url)
+            self.assertText('127.0.0.1/login/', response.full_url)
+
+            # Test "one message" page url.
+            response = self.assertResponse(
+                'django_expanded_test_cases:response-with-one-message',
+                expected_url='/views/one-message/',
+            )
+            self.assertText('/views/one-message/', response.url)
+            self.assertText('127.0.0.1/views/one-message/', response.full_url)
+
+            # Test "two messages" page url.
+            response = self.assertResponse(
+                'django_expanded_test_cases:response-with-two-messages',
+                expected_url='/views/two-messages/',
+            )
+            self.assertText('/views/two-messages/', response.url)
+            self.assertText('127.0.0.1/views/two-messages/', response.full_url)
+
+            # Test "three messages" page url.
+            response = self.assertResponse(
+                'django_expanded_test_cases:response-with-three-messages',
+                expected_url='/views/three-messages/',
+            )
+            self.assertText('/views/three-messages/', response.url)
+            self.assertText('127.0.0.1/views/three-messages/', response.full_url)
+
+        with self.subTest('With custom site_root_url value defined'):
+            self.site_root_url = 'https://my_really_cool_site.com/'
+
+            # Test "index" page url.
+            response = self.assertResponse('django_expanded_test_cases:index', expected_url='/')
+            self.assertText('/', response.url)
+            self.assertText('https://my_really_cool_site.com/', response.full_url)
+
+            # Test "login" page url.
+            response = self.assertResponse('django_expanded_test_cases:login', expected_url='/login/')
+            self.assertText('/login/', response.url)
+            self.assertText('https://my_really_cool_site.com/login/', response.full_url)
+
+            # Test "one message" page url.
+            response = self.assertResponse(
+                'django_expanded_test_cases:response-with-one-message',
+                expected_url='/views/one-message/',
+            )
+            self.assertText('/views/one-message/', response.url)
+            self.assertText('https://my_really_cool_site.com/views/one-message/', response.full_url)
+
+            # Test "two messages" page url.
+            response = self.assertResponse(
+                'django_expanded_test_cases:response-with-two-messages',
+                expected_url='/views/two-messages/',
+            )
+            self.assertText('/views/two-messages/', response.url)
+            self.assertText('https://my_really_cool_site.com/views/two-messages/', response.full_url)
+
+            # Test "three messages" page url.
+            response = self.assertResponse(
+                'django_expanded_test_cases:response-with-three-messages',
+                expected_url='/views/three-messages/',
+            )
+            self.assertText('/views/three-messages/', response.url)
+            self.assertText('https://my_really_cool_site.com/views/three-messages/', response.full_url)
+
+        with self.subTest('With view that redirects'):
+            # Using direct url.
+            self.assertResponse('redirect/index/', expected_url='/redirect/index/')
+            self.assertResponse('redirect/index/', expected_url='/redirect/index/', expected_redirect_url='/')
+            self.assertResponse(
+                'redirect/index/',
+                expected_url='/redirect/index/',
+                expected_redirect_url='django_expanded_test_cases:index',
+            )
+
+            # Using reverse.
+            self.assertResponse('django_expanded_test_cases:redirect-to-index', expected_url='/redirect/index/')
+            self.assertResponse(
+                'django_expanded_test_cases:redirect-to-index',
+                expected_url='/redirect/index/',
+                expected_redirect_url='/',
+            )
+            self.assertResponse(
+                'django_expanded_test_cases:redirect-to-index',
+                expected_url='/redirect/index/',
+                expected_redirect_url='django_expanded_test_cases:index',
+            )
+
+        with self.subTest('Verify error on urls that don\'t match'):
+            expected_err_msg = (
+                # To prevent Black single-lining this.
+                'Expected Url and actual Url do not match. \n'
+                'Expected Url: \n'
+                '"{0}" \n'
+                'Actual Url: \n'
+                '"{1}" \n'
+            )
+            wrong_url = '/wrong_url/'
+
+            # Test 404 page url.
+            with self.assertRaises(AssertionError) as err:
+                self.assertResponse('bad_url', expected_url=wrong_url, expected_status=404)
+            self.assertEqual(expected_err_msg.format(wrong_url, '/bad_url/'), str(err.exception))
+
+            # Test "index" page url.
+            with self.assertRaises(AssertionError) as err:
+                self.assertResponse('', expected_url=wrong_url)
+            self.assertEqual(expected_err_msg.format(wrong_url, '/'), str(err.exception))
+
+            # Test "login" page url.
+            with self.assertRaises(AssertionError) as err:
+                self.assertResponse('login/', expected_url=wrong_url)
+            self.assertEqual(expected_err_msg.format(wrong_url, '/login/'), str(err.exception))
+
+            # Test "one message" page url.
+            with self.assertRaises(AssertionError) as err:
+                self.assertResponse('views/one-message/', expected_url=wrong_url)
+            self.assertEqual(expected_err_msg.format(wrong_url, '/views/one-message/'), str(err.exception))
+
+            # Test "two messages" page url.
+            with self.assertRaises(AssertionError) as err:
+                self.assertResponse('views/two-messages/', expected_url=wrong_url)
+            self.assertEqual(expected_err_msg.format(wrong_url, '/views/two-messages/'), str(err.exception))
+
+            # Test "three messages" page url.
+            with self.assertRaises(AssertionError) as err:
+                self.assertResponse('views/three-messages/', expected_url=wrong_url)
+            self.assertEqual(expected_err_msg.format(wrong_url, '/views/three-messages/'), str(err.exception))
+
+            # Test "user detail" page url via args.
+            with self.assertRaises(AssertionError) as err:
+                self.assertResponse('user/detail/1/', expected_url=wrong_url)
+            self.assertEqual(expected_err_msg.format(wrong_url, '/user/detail/1/'), str(err.exception))
+
+            # Test "user detail" page url via kwargs.
+            with self.assertRaises(AssertionError) as err:
+                self.assertResponse('user/detail/2/', expected_url=wrong_url)
+            self.assertEqual(expected_err_msg.format(wrong_url, '/user/detail/2/'), str(err.exception))
+
+    def test__assertResponse__view_should_redirect__success(self):
+        """
+        Tests "expected_url" functionality of assertResponse() function, with assertions that should succeed.
+        """
+
+        with self.subTest('With view that doesn\'t redirect'):
+            # Test 404 page url.
+            response = self.assertResponse(
+                'bad_url',
+                expected_url='/bad_url/',
+                expected_status=404,
+                view_should_redirect=False,
+            )
+            self.assertText('/bad_url/', response.url)
+            self.assertText('127.0.0.1/bad_url/', response.full_url)
+            response = self.assertResponse(
+                'bad_url/',
+                expected_url='/bad_url/',
+                expected_status=404,
+                view_should_redirect=False,
+            )
+            self.assertText('/bad_url/', response.url)
+            self.assertText('127.0.0.1/bad_url/', response.full_url)
+            response = self.assertResponse(
+                '127.0.0.1/bad_url/',
+                expected_url='/bad_url/',
+                expected_status=404,
+                view_should_redirect=False,
+            )
+            self.assertText('/bad_url/', response.url)
+            self.assertText('127.0.0.1/bad_url/', response.full_url)
+            response = self.assertResponse(
+                '///bad_url///',
+                expected_url='/bad_url/',
+                expected_status=404,
+                view_should_redirect=False,
+            )
+            self.assertText('/bad_url/', response.url)
+            self.assertText('127.0.0.1/bad_url/', response.full_url)
+
+            # Test "index" page url.
+            response = self.assertResponse('', expected_url='/', view_should_redirect=False)
+            self.assertText('/', response.url)
+            self.assertText('127.0.0.1/', response.full_url)
+            response = self.assertResponse('/', expected_url='/', view_should_redirect=False)
+            self.assertText('/', response.url)
+            self.assertText('127.0.0.1/', response.full_url)
+            response = self.assertResponse('127.0.0.1/', expected_url='/', view_should_redirect=False)
+            self.assertText('/', response.url)
+            self.assertText('127.0.0.1/', response.full_url)
+
+            # Test "login" page url.
+            response = self.assertResponse('login/', expected_url='/login/', view_should_redirect=False)
+            self.assertText('/login/', response.url)
+            self.assertText('127.0.0.1/login/', response.full_url)
+            response = self.assertResponse('/login/', expected_url='/login/', view_should_redirect=False)
+            self.assertText('/login/', response.url)
+            self.assertText('127.0.0.1/login/', response.full_url)
+            response = self.assertResponse('127.0.0.1/login/', expected_url='/login/', view_should_redirect=False)
+            self.assertText('/login/', response.url)
+            self.assertText('127.0.0.1/login/', response.full_url)
+
+            # Test "one message" page url.
+            response = self.assertResponse(
+                'views/one-message/',
+                expected_url='/views/one-message/',
+                view_should_redirect=False,
+            )
+            self.assertText('/views/one-message/', response.url)
+            self.assertText('127.0.0.1/views/one-message/', response.full_url)
+            response = self.assertResponse(
+                '/views/one-message/',
+                expected_url='/views/one-message/',
+                view_should_redirect=False,
+            )
+            self.assertText('/views/one-message/', response.url)
+            self.assertText('127.0.0.1/views/one-message/', response.full_url)
+            response = self.assertResponse(
+                '127.0.0.1/views/one-message/',
+                expected_url='/views/one-message/',
+                view_should_redirect=False,
+            )
+            self.assertText('/views/one-message/', response.url)
+            self.assertText('127.0.0.1/views/one-message/', response.full_url)
+
+            # Test "two messages" page url.
+            response = self.assertResponse(
+                'views/two-messages/',
+                expected_url='/views/two-messages/',
+                view_should_redirect=False,
+            )
+            self.assertText('/views/two-messages/', response.url)
+            self.assertText('127.0.0.1/views/two-messages/', response.full_url)
+            response = self.assertResponse(
+                '/views/two-messages/',
+                expected_url='/views/two-messages/',
+                view_should_redirect=False,
+            )
+            self.assertText('/views/two-messages/', response.url)
+            self.assertText('127.0.0.1/views/two-messages/', response.full_url)
+            response = self.assertResponse(
+                '127.0.0.1/views/two-messages/',
+                expected_url='/views/two-messages/',
+                view_should_redirect=False,
+            )
+            self.assertText('/views/two-messages/', response.url)
+            self.assertText('127.0.0.1/views/two-messages/', response.full_url)
+
+            # Test "three messages" page url.
+            response = self.assertResponse(
+                'views/three-messages/',
+                expected_url='/views/three-messages/',
+                view_should_redirect=False,
+            )
+            self.assertText('/views/three-messages/', response.url)
+            self.assertText('127.0.0.1/views/three-messages/', response.full_url)
+            response = self.assertResponse(
+                '/views/three-messages/',
+                expected_url='/views/three-messages/',
+                view_should_redirect=False,
+            )
+            self.assertText('/views/three-messages/', response.url)
+            self.assertText('127.0.0.1/views/three-messages/', response.full_url)
+            response = self.assertResponse(
+                '127.0.0.1/views/three-messages/',
+                expected_url='/views/three-messages/',
+                view_should_redirect=False,
+            )
+            self.assertText('/views/three-messages/', response.url)
+            self.assertText('127.0.0.1/views/three-messages/', response.full_url)
+
+            # Test "user detail" page url via args.
+            response = self.assertResponse(
+                'user/detail/1/',
+                expected_url='/user/detail/1/',
+                view_should_redirect=False,
+            )
+            self.assertText('/user/detail/1/', response.url)
+            self.assertText('127.0.0.1/user/detail/1/', response.full_url)
+            response = self.assertResponse(
+                '/user/detail/1/',
+                expected_url='/user/detail/1/',
+                view_should_redirect=False,
+            )
+            self.assertText('/user/detail/1/', response.url)
+            self.assertText('127.0.0.1/user/detail/1/', response.full_url)
+            response = self.assertResponse(
+                '127.0.0.1/user/detail/1/',
+                expected_url='/user/detail/1/',
+                view_should_redirect=False,
+            )
+            self.assertText('/user/detail/1/', response.url)
+            self.assertText('127.0.0.1/user/detail/1/', response.full_url)
+
+            # Test "user detail" page url via kwargs.
+            response = self.assertResponse(
+                'user/detail/2/',
+                expected_url='/user/detail/2/',
+                view_should_redirect=False,
+            )
+            self.assertText('/user/detail/2/', response.url)
+            self.assertText('127.0.0.1/user/detail/2/', response.full_url)
+            response = self.assertResponse(
+                '/user/detail/2/',
+                expected_url='/user/detail/2/',
+                view_should_redirect=False,
+            )
+            self.assertText('/user/detail/2/', response.url)
+            self.assertText('127.0.0.1/user/detail/2/', response.full_url)
+            response = self.assertResponse(
+                '127.0.0.1/user/detail/2/',
+                expected_url='/user/detail/2/',
+                view_should_redirect=False,
+            )
+            self.assertText('/user/detail/2/', response.url)
+            self.assertText('127.0.0.1/user/detail/2/', response.full_url)
+
+        with self.subTest('With view that redirects'):
+            # Using direct url.
+            self.assertResponse(
+                'redirect/index/',
+                expected_url='/redirect/index/',
+                expected_redirect_url='/',
+                view_should_redirect=True,
+            )
+            self.assertResponse(
+                'redirect/index/',
+                expected_url='/redirect/index/',
+                expected_redirect_url='django_expanded_test_cases:index',
+                view_should_redirect=True,
+            )
+
+            # Using reverse.
+            self.assertResponse(
+                'django_expanded_test_cases:redirect-to-index',
+                expected_url='/redirect/index/',
+                expected_redirect_url='/',
+                view_should_redirect=True,
+            )
+            self.assertResponse(
+                'django_expanded_test_cases:redirect-to-index',
+                expected_url='/redirect/index/',
+                expected_redirect_url='django_expanded_test_cases:index',
+                view_should_redirect=True,
+            )
+
+    def test__assertResponse__view_should_redirect__failure(self):
+        """
+        Tests "expected_url" functionality of assertResponse() function, with assertions that should fail.
+        """
+
+        with self.subTest('With view that doesn\'t redirect'):
+            # Test 404 page url.
+            with self.assertRaises(AssertionError) as err:
+                self.assertResponse(
+                    'bad_url',
+                    expected_url='/bad_url/',
+                    expected_status=404,
+                    view_should_redirect=True,
+                )
+            self.assertEqual(str(err.exception), 'Expected a page redirect, but response did not redirect.')
+
+            # Test "index" page url.
+            with self.assertRaises(AssertionError) as err:
+                self.assertResponse('', expected_url='/', view_should_redirect=True)
+            self.assertEqual(str(err.exception), 'Expected a page redirect, but response did not redirect.')
+
+            # Test "login" page url.
+            with self.assertRaises(AssertionError) as err:
+                self.assertResponse('login/', expected_url='/login/', view_should_redirect=True)
+            self.assertEqual(str(err.exception), 'Expected a page redirect, but response did not redirect.')
+
+            # Test "one message" page url.
+            with self.assertRaises(AssertionError) as err:
+                self.assertResponse(
+                    'views/one-message/',
+                    expected_url='/views/one-message/',
+                    view_should_redirect=True,
+                )
+            self.assertEqual(str(err.exception), 'Expected a page redirect, but response did not redirect.')
+
+            # Test "three messages" page url.
+            with self.assertRaises(AssertionError) as err:
+                self.assertResponse(
+                    'views/three-messages/',
+                    expected_url='/views/three-messages/',
+                    view_should_redirect=True,
+                )
+            self.assertEqual(str(err.exception), 'Expected a page redirect, but response did not redirect.')
+
+            # Test "user detail" page url via kwargs.
+            with self.assertRaises(AssertionError) as err:
+                self.assertResponse(
+                    'user/detail/2/',
+                    expected_url='/user/detail/2/',
+                    view_should_redirect=True,
+                )
+            self.assertEqual(str(err.exception), 'Expected a page redirect, but response did not redirect.')
+
+        with self.subTest('With view that redirects'):
+            # Using direct url.
+            with self.assertRaises(AssertionError) as err:
+                self.assertResponse(
+                    'redirect/index/',
+                    expected_url='/redirect/index/',
+                    expected_redirect_url='/',
+                    view_should_redirect=False,
+                )
+            self.assertEqual(
+                str(err.exception),
+                'Expected no page redirects, but response processed one or more redirects.',
+            )
+
+            # Using reverse.
+            with self.assertRaises(AssertionError) as err:
+                self.assertResponse(
+                    'django_expanded_test_cases:redirect-to-index',
+                    expected_url='/redirect/index/',
+                    expected_redirect_url='/',
+                    view_should_redirect=False,
+                )
+            self.assertEqual(
+                str(err.exception),
+                'Expected no page redirects, but response processed one or more redirects.',
+            )
+
     def test__assertResponse__expected_title(self):
         """
         Tests "expected_title" functionality of assertResponse() function.
         """
         exception_msg = (
             'Expected title HTML contents of "Wrong Title" (using exact matching). '
             'Actual value was "Home Page | Test Views".'
@@ -643,33 +1211,52 @@
                 self.assertResponse('django_expanded_test_cases:index', expected_messages='Wrong message.')
             self.assertText(exception_msg.format('Wrong message.', 'exact'), str(err.exception))
             with self.assertRaises(AssertionError) as err:
                 self.assertResponse('django_expanded_test_cases:index', expected_messages=['Wrong message.'])
             self.assertText(exception_msg.format('Wrong message.', 'exact'), str(err.exception))
 
         with self.subTest('Multiple messages on page - match'):
-            self.assertResponse('django_expanded_test_cases:response-with-three-messages', expected_messages='Test info message.')
-            self.assertResponse('django_expanded_test_cases:response-with-three-messages', expected_messages=['Test warning message.'])
             self.assertResponse(
                 'django_expanded_test_cases:response-with-three-messages',
-                expected_messages=['Test info message.', 'Test warning message.'],
+                expected_messages='Test info message.',
+            )
+            self.assertResponse(
+                'django_expanded_test_cases:response-with-three-messages',
+                expected_messages=['Test warning message.'],
+            )
+            self.assertResponse(
+                'django_expanded_test_cases:response-with-three-messages',
+                expected_messages=[
+                    'Test info message.',
+                    'Test warning message.',
+                ],
             )
             self.assertResponse(
                 'django_expanded_test_cases:response-with-three-messages',
-                expected_messages=['Test info message.', 'Test warning message.', 'Test error message.'],
+                expected_messages=[
+                    'Test info message.',
+                    'Test warning message.',
+                    'Test error message.',
+                ],
             )
 
         with self.subTest('Multiple messages on page - mismatch'):
             with self.assertRaises(AssertionError) as err:
-                self.assertResponse('django_expanded_test_cases:response-with-three-messages', expected_messages='Wrong message.')
+                self.assertResponse(
+                    'django_expanded_test_cases:response-with-three-messages',
+                    expected_messages='Wrong message.',
+                )
             self.assertText(exception_msg.format('Wrong message.', 'exact'), str(err.exception))
             with self.assertRaises(AssertionError) as err:
                 self.assertResponse(
                     'django_expanded_test_cases:response-with-three-messages',
-                    expected_messages=['Test info message.', 'Wrong message.'],
+                    expected_messages=[
+                        'Test info message.',
+                        'Wrong message.',
+                    ],
                 )
             self.assertText(exception_msg.format('Wrong message.', 'exact'), str(err.exception))
 
     def test__assertResponse__expected_content(self):
         """
         Tests "expected_content" functionality of assertResponse() function.
         """
@@ -832,30 +1419,30 @@
                     """,
                 ],
                 content_starts_after='<meta charset="utf-8">',
                 content_ends_before='<p>Pretend this is the project landing page.</p>',
             )
 
     def test__assertPageContent__expected_content__repeating_elements(self):
-        with (self.subTest('Sanity check, making sure each individual content section is found from full response')):
+        with self.subTest('Sanity check, making sure each individual content section is found from full response'):
             self.assertResponse(
                 'django_expanded_test_cases:response-with-repeating-elements',
                 expected_content=['<p>Test First Unique Line</p>'],
                 content_starts_after='<p>Repeating Line</p>',
             )
             self.assertResponse(
                 'django_expanded_test_cases:response-with-repeating-elements',
                 expected_content=['<p>Test Second Unique Line</p>'],
                 content_starts_after='<p>Repeating Line</p>',
             )
             self.assertResponse(
                 'django_expanded_test_cases:response-with-repeating-elements',
                 expected_content=['<p>Test Third Unique Line</p>'],
                 content_starts_after='<p>Repeating Line</p>',
-              )
+            )
             self.assertResponse(
                 'django_expanded_test_cases:response-with-repeating-elements',
                 expected_content=['<p>Repeating Line</p>'],
             )
 
         with self.subTest('Check all values together'):
             self.assertResponse(
@@ -892,15 +1479,14 @@
                 'django_expanded_test_cases:index',
                 expected_not_content=[
                     '<title>Home Page | Test Views</title>',
                     '<h1>Home Page Header</h1>',
                     '<p>Pretend this is',
                     'the project landing page.</p>',
                 ],
-
             )
         self.assertText(exception_msg.format('<title>Home Page | Test Views</title>'), str(err.exception))
 
     def test__assertGetResponse(self):
         """
         Tests assertGetResponse() function.
         Note: Most logic in here passes into the assertResponse() function.
@@ -1068,55 +1654,82 @@
 
     def test__assertResponseRedirects__success(self):
         """
         Tests assertResponseRedirects() function, in cases when it should succeed.
         """
         with self.subTest('With view that redirects'):
             # Using direct url.
-            self.assertRedirects('redirect/index/', expected_redirect_url='/')
-            self.assertRedirects('redirect/index/', expected_redirect_url='django_expanded_test_cases:index')
+            self.assertRedirects(
+                'redirect/index/',
+                expected_redirect_url='/',
+            )
+            self.assertRedirects(
+                'redirect/index/',
+                expected_redirect_url='django_expanded_test_cases:index',
+            )
 
             # Using reverse.
-            self.assertRedirects('django_expanded_test_cases:redirect-to-index', expected_redirect_url='/')
+            self.assertRedirects(
+                'django_expanded_test_cases:redirect-to-index',
+                expected_redirect_url='/',
+            )
             self.assertRedirects(
                 'django_expanded_test_cases:redirect-to-index',
                 expected_redirect_url='django_expanded_test_cases:index',
             )
 
     def test__assertResponseRedirects__failure(self):
         """
         Tests assertResponseRedirects() function, in cases when it should fail.
         """
         exception_msg = 'Response didn\'t redirect as expected. Response code was {0} (expected 302).'
 
         with self.subTest('With view that does not redirect - Invalid page'):
             request = self._get_page_response('bad_page/')
             with self.assertRaises(AssertionError) as err:
-                self.assertRedirects(request, expected_redirect_url='/')
+                self.assertRedirects(
+                    request,
+                    expected_redirect_url='/',
+                )
             self.assertText(exception_msg.format(request.status_code), str(err.exception))
             with self.assertRaises(AssertionError) as err:
-                self.assertRedirects(request, expected_redirect_url='django_expanded_test_cases:invalid')
+                self.assertRedirects(
+                    request,
+                    expected_redirect_url='django_expanded_test_cases:invalid',
+                )
             self.assertText(exception_msg.format(request.status_code), str(err.exception))
 
         with self.subTest('With view that does not redirect - Index page'):
             request = self._get_page_response('')
             with self.assertRaises(AssertionError) as err:
-                self.assertRedirects(request, expected_redirect_url='/')
+                self.assertRedirects(
+                    request,
+                    expected_redirect_url='/',
+                )
             self.assertText(exception_msg.format(request.status_code), str(err.exception))
             with self.assertRaises(AssertionError) as err:
-                self.assertRedirects(request, expected_redirect_url='django_expanded_test_cases:index')
+                self.assertRedirects(
+                    request,
+                    expected_redirect_url='django_expanded_test_cases:index',
+                )
             self.assertText(exception_msg.format(request.status_code), str(err.exception))
 
         with self.subTest('With view that does not redirect - Non-index page'):
             request = self._get_page_response('login/')
             with self.assertRaises(AssertionError) as err:
-                self.assertRedirects(request, expected_redirect_url='/')
+                self.assertRedirects(
+                    request,
+                    expected_redirect_url='/',
+                )
             self.assertText(exception_msg.format(request.status_code), str(err.exception))
             with self.assertRaises(AssertionError) as err:
-                self.assertRedirects(request, expected_redirect_url='django_expanded_test_cases:login')
+                self.assertRedirects(
+                    request,
+                    expected_redirect_url='django_expanded_test_cases:login',
+                )
             self.assertText(exception_msg.format(request.status_code), str(err.exception))
 
     def test__assertStatusCode__success(self):
         """
         Tests assertStatusCode() function, in cases when it should succeed.
         """
         with self.subTest('Status 200'):
@@ -1192,15 +1805,18 @@
         """
         with self.subTest('Including title tag in expected'):
             response = HttpResponse('<title>Test Title</title>')
             self.assertPageTitle(response, '<title>Test Title</title>')
 
         with self.subTest('Including title tag in expected, with extra whitespace around tag'):
             response = HttpResponse('<title>Test Title</title>')
-            self.assertPageTitle(response, '   <title>    Test Title    </title>   ')
+            self.assertPageTitle(
+                response,
+                '   <title>    Test Title    </title>   ',
+            )
 
         with self.subTest('No title element in response (simulates things like file downloads)'):
             response = HttpResponse('')
             self.assertPageTitle(response, '')
 
         with self.subTest('Title exists, but is empty'):
             response = HttpResponse('<title></title>')
@@ -1216,35 +1832,67 @@
 
         with self.subTest('Basic title, with extra whitespace (to simulate Django templating)'):
             response = HttpResponse('<title>   Test    Title   </title>')
             self.assertPageTitle(response, 'Test Title')
 
         with self.subTest('Complex title - Exact Match'):
             response = HttpResponse('<title>Test Title | My Custom App | My Really Cool Site</title>')
-            self.assertPageTitle(response, 'Test Title | My Custom App | My Really Cool Site', allow_partials=False)
+            self.assertPageTitle(
+                response,
+                'Test Title | My Custom App | My Really Cool Site',
+                allow_partials=False,
+            )
 
         with self.subTest('Complex title, with extra whitespace (to simulate Django templating) - Exact Match'):
             response = HttpResponse(
                 '<title>   Test   Title    \n|\n   My Custom App   \n|\n   My Really Cool Site   </title>'
             )
-            self.assertPageTitle(response, 'Test Title | My Custom App | My Really Cool Site', allow_partials=False)
+            self.assertPageTitle(
+                response,
+                'Test Title | My Custom App | My Really Cool Site',
+                allow_partials=False,
+            )
 
         with self.subTest('Complex title - Loose Match'):
             response = HttpResponse('<title>Test Title | My Custom App | My Really Cool Site</title>')
-            self.assertPageTitle(response, 'Test Title', allow_partials=True)
-            self.assertPageTitle(response, 'My Custom App', allow_partials=True)
-            self.assertPageTitle(response, 'My Really Cool Site', allow_partials=True)
+            self.assertPageTitle(
+                response,
+                'Test Title',
+                allow_partials=True,
+            )
+            self.assertPageTitle(
+                response,
+                'My Custom App',
+                allow_partials=True,
+            )
+            self.assertPageTitle(
+                response,
+                'My Really Cool Site',
+                allow_partials=True,
+            )
 
         with self.subTest('Complex title, with extra whitespace (to simulate Django templating) - Loose Match'):
             response = HttpResponse(
                 '<title>   Test   Title    \n|\n   My Custom App   \n|\n   My Really Cool Site   </title>'
             )
-            self.assertPageTitle(response, 'Test Title', allow_partials=True)
-            self.assertPageTitle(response, 'My Custom App', allow_partials=True)
-            self.assertPageTitle(response, 'My Really Cool Site', allow_partials=True)
+            self.assertPageTitle(
+                response,
+                'Test Title',
+                allow_partials=True,
+            )
+            self.assertPageTitle(
+                response,
+                'My Custom App',
+                allow_partials=True,
+            )
+            self.assertPageTitle(
+                response,
+                'My Really Cool Site',
+                allow_partials=True,
+            )
 
         with self.subTest('Title has non-standard values in base page'):
             # Test with "standard" values.
             response = HttpResponse('<title>This Title has Two Arrows => =></title>')
             self.assertPageTitle(response, 'This Title has Two Arrows => =>')
 
             # Test with "mixed" values.
@@ -1261,31 +1909,43 @@
         """
         exception_msg = 'Expected title HTML contents of "{0}" (using {2} matching). Actual value was "{1}".'
 
         with self.subTest('Checking for title when none exists'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('')
                 self.assertPageTitle(response, 'Test Title')
-            self.assertText(exception_msg.format('Test Title', '', 'exact'), str(err.exception))
+            self.assertText(
+                exception_msg.format('Test Title', '', 'exact'),
+                str(err.exception),
+            )
 
         with self.subTest('Expected value is on page, but not in title tag'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('Test Title')
                 self.assertPageTitle(response, 'Test Title')
-            self.assertText(exception_msg.format('Test Title', '', 'exact'), str(err.exception))
+            self.assertText(
+                exception_msg.format('Test Title', '', 'exact'),
+                str(err.exception),
+            )
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<h1>Test Title</h1><p>Test Title</p>')
                 self.assertPageTitle(response, 'Test Title')
-            self.assertText(exception_msg.format('Test Title', '', 'exact'), str(err.exception))
+            self.assertText(
+                exception_msg.format('Test Title', '', 'exact'),
+                str(err.exception),
+            )
 
         with self.subTest('Assuming extra whitespace is still present'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<title>   Test    Title   </title>')
                 self.assertPageTitle(response, '   Test    Title   ')
-            self.assertText(exception_msg.format('Test    Title', 'Test Title', 'exact'), str(err.exception))
+            self.assertText(
+                exception_msg.format('Test    Title', 'Test Title', 'exact'),
+                str(err.exception),
+            )
 
         with self.subTest('Set to exact match, but only passing in title subsection'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<title>Test Title | My Custom App | My Really Cool Site</title>')
                 self.assertPageTitle(response, 'Test Title')
             self.assertText(
                 exception_msg.format(
@@ -1319,29 +1979,41 @@
             )
 
         with self.subTest('Set to partial match, but value is not in title'):
             # Full mismatch.
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('Test Title')
                 self.assertPageTitle(response, 'Wrong Value', allow_partials=True)
-            self.assertText(exception_msg.format('Wrong Value', '', 'partial'), str(err.exception))
+            self.assertText(
+                exception_msg.format('Wrong Value', '', 'partial'),
+                str(err.exception),
+            )
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<title>Test Title</title>')
                 self.assertPageTitle(response, 'Wrong Value', allow_partials=True)
-            self.assertText(exception_msg.format('Wrong Value', 'Test Title', 'partial'), str(err.exception))
+            self.assertText(
+                exception_msg.format('Wrong Value', 'Test Title', 'partial'),
+                str(err.exception),
+            )
 
             # Partial match, but also has extra.
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('Test Title')
                 self.assertPageTitle(response, 'Test Title and More', allow_partials=True)
-            self.assertText(exception_msg.format('Test Title and More', '', 'partial'), str(err.exception))
+            self.assertText(
+                exception_msg.format('Test Title and More', '', 'partial'),
+                str(err.exception),
+            )
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<title>Test Title</title>')
                 self.assertPageTitle(response, 'Test Title and More', allow_partials=True)
-            self.assertText(exception_msg.format('Test Title and More', 'Test Title', 'partial'), str(err.exception))
+            self.assertText(
+                exception_msg.format('Test Title and More', 'Test Title', 'partial'),
+                str(err.exception),
+            )
 
         with self.subTest('Multiple Titles - Two and no spaces'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<title>Title 1</title><title>Title 2</title>')
                 self.assertPageTitle(response, '')
             self.assertText(
                 (
@@ -1456,37 +2128,52 @@
         """
         exception_msg = 'Expected H1 header HTML contents of "{0}". Actual value was "{1}".'
 
         with self.subTest('Checking for header when none exists'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('')
                 self.assertPageHeader(response, 'Test Header')
-            self.assertText(exception_msg.format('Test Header', ''), str(err.exception))
+            self.assertText(
+                exception_msg.format('Test Header', ''),
+                str(err.exception),
+            )
 
         with self.subTest('Expected value is on page, but not in header tag'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('Test Header')
                 self.assertPageHeader(response, 'Test Header')
-            self.assertText(exception_msg.format('Test Header', ''), str(err.exception))
+            self.assertText(
+                exception_msg.format('Test Header', ''),
+                str(err.exception),
+            )
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<h2>Test Header</h2><p>Test Header</p>')
                 self.assertPageHeader(response, 'Test Header')
-            self.assertText(exception_msg.format('Test Header', ''), str(err.exception))
+            self.assertText(
+                exception_msg.format('Test Header', ''),
+                str(err.exception),
+            )
 
         with self.subTest('Assuming extra whitespace is still present'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<h1>   Test    Header   </h1>')
                 self.assertPageHeader(response, '   Test    Header   ')
-            self.assertText(exception_msg.format('Test    Header', 'Test Header'), str(err.exception))
+            self.assertText(
+                exception_msg.format('Test    Header', 'Test Header'),
+                str(err.exception),
+            )
 
         with self.subTest('Expected value is present, plus extra'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<h1>Test Header</h1>')
                 self.assertPageHeader(response, 'Test Header plus Extra')
-            self.assertText(exception_msg.format('Test Header plus Extra', 'Test Header'), str(err.exception))
+            self.assertText(
+                exception_msg.format('Test Header plus Extra', 'Test Header'),
+                str(err.exception),
+            )
 
         with self.subTest('Multiple Headers - Two and no spaces'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<h1>Header 1</h1><h1>Header 2</h1>')
                 self.assertPageHeader(response, '')
             self.assertText(
                 (
@@ -1505,15 +2192,15 @@
             self.assertText(
                 (
                     'Found multiple headers (2 total). There should only be one <h1> tag per page.\n'
                     'For further reference on <h1> tags, consider consulting:\n'
                     '    * https://www.w3schools.com/tags/tag_hn.asp\n'
                     '    * https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Heading_Elements'
                 ),
-                str(err.exception)
+                str(err.exception),
             )
 
         with self.subTest('Multiple Headers - Two with line breaks'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<h1>Header 1</h1>\n<br>\n<h1>Header 2</h1>')
                 self.assertPageHeader(response, '')
             self.assertText(
@@ -1623,96 +2310,197 @@
         Tests assertContextMessages() function, in cases when it should fail.
         """
         exception_msg = 'Failed to find message "{0}" in context (using {1} matching).'
 
         with self.subTest('Checking for single message, none exist'):
             with self.assertRaises(AssertionError) as err:
                 response = self._get_page_response('django_expanded_test_cases:index')
-                self.assertContextMessages(response, 'This is a test message.')
-            self.assertText(exception_msg.format('This is a test message.', 'exact'), str(err.exception))
+                self.assertContextMessages(
+                    response,
+                    'This is a test message.',
+                )
+            self.assertText(
+                exception_msg.format('This is a test message.', 'exact'),
+                str(err.exception),
+            )
 
         with self.subTest('Checking for single message, one exists but doesn\'t match'):
             with self.assertRaises(AssertionError) as err:
                 response = self._get_page_response('django_expanded_test_cases:response-with-one-message')
                 self.assertContextMessages(response, 'Testing!')
-            self.assertText(exception_msg.format('Testing!', 'exact'), str(err.exception))
+            self.assertText(
+                exception_msg.format('Testing!', 'exact'),
+                str(err.exception),
+            )
 
         with self.subTest('Checking for single message, but it\'s only a partial match'):
             response = self._get_page_response('django_expanded_test_cases:response-with-one-message')
             with self.assertRaises(AssertionError) as err:
-                self.assertContextMessages(response, 'This is a test message')
-            self.assertText(exception_msg.format('This is a test message', 'exact'), str(err.exception))
+                self.assertContextMessages(
+                    response,
+                    'This is a test message',
+                )
+            self.assertText(
+                exception_msg.format('This is a test message', 'exact'),
+                str(err.exception),
+            )
             with self.assertRaises(AssertionError) as err:
                 self.assertContextMessages(response, 'test message.')
-            self.assertText(exception_msg.format('test message.', 'exact'), str(err.exception))
+            self.assertText(
+                exception_msg.format('test message.', 'exact'),
+                str(err.exception),
+            )
             with self.assertRaises(AssertionError) as err:
-                self.assertContextMessages(response, 'test')
-            self.assertText(exception_msg.format('test', 'exact'), str(err.exception))
+                self.assertContextMessages(
+                    response,
+                    'test',
+                )
+            self.assertText(
+                exception_msg.format('test', 'exact'),
+                str(err.exception),
+            )
 
         with self.subTest('Checking for single message, multiple exist but don\'t match'):
             with self.assertRaises(AssertionError) as err:
-                response = self._get_page_response('django_expanded_test_cases:response-with-three-messages')
+                response = self._get_page_response(
+                    'django_expanded_test_cases:response-with-three-messages',
+                )
                 self.assertContextMessages(response, 'Testing!')
-            self.assertText(exception_msg.format('Testing!', 'exact'), str(err.exception))
+            self.assertText(
+                exception_msg.format('Testing!', 'exact'),
+                str(err.exception),
+            )
 
         with self.subTest('Checking for two messages, none exist'):
             with self.assertRaises(AssertionError) as err:
                 response = self._get_page_response('django_expanded_test_cases:index')
-                self.assertContextMessages(response, ['This is a test message.', 'Another message.'])
-            self.assertText(exception_msg.format('This is a test message.', 'exact'), str(err.exception))
+                self.assertContextMessages(
+                    response,
+                    ['This is a test message.', 'Another message.'],
+                )
+            self.assertText(
+                exception_msg.format('This is a test message.', 'exact'),
+                str(err.exception),
+            )
 
         with self.subTest('Checking for two messages, but only one exists'):
             with self.assertRaises(AssertionError) as err:
                 response = self._get_page_response('django_expanded_test_cases:response-with-one-message')
-                self.assertContextMessages(response, ['This is a test message.', 'Another message.'])
-            self.assertText(exception_msg.format('Another message.', 'exact'), str(err.exception))
+                self.assertContextMessages(
+                    response,
+                    ['This is a test message.', 'Another message.'],
+                )
+            self.assertText(
+                exception_msg.format('Another message.', 'exact'),
+                str(err.exception),
+            )
 
         with self.subTest('Checking for two messages, multiple exist but one doesn\'t match'):
             response = self._get_page_response('django_expanded_test_cases:response-with-three-messages')
             with self.assertRaises(AssertionError) as err:
-                self.assertContextMessages(response, ['Test info message.', 'Another message.'])
-            self.assertText(exception_msg.format('Another message.', 'exact'), str(err.exception))
+                self.assertContextMessages(
+                    response,
+                    ['Test info message.', 'Another message.'],
+                )
+            self.assertText(
+                exception_msg.format('Another message.', 'exact'),
+                str(err.exception),
+            )
             with self.assertRaises(AssertionError) as err:
-                self.assertContextMessages(response, ['Bad message', 'Test info message.'])
-            self.assertText(exception_msg.format('Bad message', 'exact'), str(err.exception))
+                self.assertContextMessages(
+                    response,
+                    ['Bad message', 'Test info message.'],
+                )
+            self.assertText(
+                exception_msg.format('Bad message', 'exact'),
+                str(err.exception),
+            )
 
         with self.subTest('Checking for two messages, multiple exist but none match'):
             with self.assertRaises(AssertionError) as err:
                 response = self._get_page_response('django_expanded_test_cases:response-with-three-messages')
-                self.assertContextMessages(response, ['Testing!', 'Testing again!'])
-            self.assertText(exception_msg.format('Testing!', 'exact'), str(err.exception))
+                self.assertContextMessages(
+                    response,
+                    ['Testing!', 'Testing again!'],
+                )
+            self.assertText(
+                exception_msg.format('Testing!', 'exact'),
+                str(err.exception),
+            )
 
         with self.subTest('Set to partial match, but value is not in title'):
             # Full mismatch.
             with self.assertRaises(AssertionError) as err:
                 response = self._get_page_response('django_expanded_test_cases:response-with-one-message')
-                self.assertContextMessages(response, 'Wrong Value', allow_partials=True)
-            self.assertText(exception_msg.format('Wrong Value', 'partial'), str(err.exception))
+                self.assertContextMessages(
+                    response,
+                    'Wrong Value',
+                    allow_partials=True,
+                )
+            self.assertText(
+                exception_msg.format('Wrong Value', 'partial'),
+                str(err.exception),
+            )
             with self.assertRaises(AssertionError) as err:
                 response = self._get_page_response('django_expanded_test_cases:response-with-two-messages')
-                self.assertContextMessages(response, 'Wrong Value', allow_partials=True)
-            self.assertText(exception_msg.format('Wrong Value', 'partial'), str(err.exception))
+                self.assertContextMessages(
+                    response,
+                    'Wrong Value',
+                    allow_partials=True,
+                )
+            self.assertText(
+                exception_msg.format('Wrong Value', 'partial'),
+                str(err.exception),
+            )
             with self.assertRaises(AssertionError) as err:
                 response = self._get_page_response('django_expanded_test_cases:response-with-three-messages')
-                self.assertContextMessages(response, 'Wrong Value', allow_partials=True)
-            self.assertText(exception_msg.format('Wrong Value', 'partial'), str(err.exception))
+                self.assertContextMessages(
+                    response,
+                    'Wrong Value',
+                    allow_partials=True,
+                )
+            self.assertText(
+                exception_msg.format('Wrong Value', 'partial'),
+                str(err.exception),
+            )
 
             # Partial match, but also has extra.
             with self.assertRaises(AssertionError) as err:
                 response = self._get_page_response('django_expanded_test_cases:response-with-one-message')
-                self.assertContextMessages(response, 'This is a test message, testing', allow_partials=True)
-            self.assertText(exception_msg.format('This is a test message, testing', 'partial'), str(err.exception))
+                self.assertContextMessages(
+                    response,
+                    'This is a test message, testing',
+                    allow_partials=True,
+                )
+            self.assertText(
+                exception_msg.format('This is a test message, testing', 'partial'),
+                str(err.exception),
+            )
             with self.assertRaises(AssertionError) as err:
                 response = self._get_page_response('django_expanded_test_cases:response-with-two-messages')
-                self.assertContextMessages(response, 'This is and more', allow_partials=True)
-            self.assertText(exception_msg.format('This is and more','partial'), str(err.exception))
+                self.assertContextMessages(
+                    response,
+                    'This is and more',
+                    allow_partials=True,
+                )
+            self.assertText(
+                exception_msg.format('This is and more', 'partial'),
+                str(err.exception),
+            )
             with self.assertRaises(AssertionError) as err:
                 response = self._get_page_response('django_expanded_test_cases:response-with-three-messages')
-                self.assertContextMessages(response, 'info message and more', allow_partials=True)
-            self.assertText(exception_msg.format('info message and more','partial'), str(err.exception))
+                self.assertContextMessages(
+                    response,
+                    'info message and more',
+                    allow_partials=True,
+                )
+            self.assertText(
+                exception_msg.format('info message and more', 'partial'),
+                str(err.exception),
+            )
 
     def test__assertPageContent__success(self):
         """
         Tests assertPageContent() function, in cases when it should succeed.
         """
         with self.subTest('Empty response, no value passed.'):
             response = HttpResponse('')
@@ -1744,28 +2532,37 @@
 
         with self.subTest('Standard Response, no value passed'):
             response = self._get_page_response('django_expanded_test_cases:login')
             self.assertPageContent(response, '')
 
         with self.subTest('Standard Response - Login Page'):
             response = self._get_page_response('django_expanded_test_cases:login')
-            self.assertPageContent(response, '<h1>Login Page Header</h1><p>Pretend this is a login page.</p>')
+            self.assertPageContent(
+                response,
+                '<h1>Login Page Header</h1><p>Pretend this is a login page.</p>',
+            )
 
         with self.subTest('Standard Response, missing part of value'):
             response = self._get_page_response('django_expanded_test_cases:login')
             self.assertPageContent(response, '<h1>Login Page Header</h1>')
             self.assertPageContent(response, '<p>Pretend this is a login page.</p>')
 
         with self.subTest('Standard Response - Render() Home Page'):
             response = self._get_page_response('django_expanded_test_cases:index')
-            self.assertPageContent(response, '<h1>Home Page Header</h1><p>Pretend this is the project landing page.</p>')
+            self.assertPageContent(
+                response,
+                '<h1>Home Page Header</h1><p>Pretend this is the project landing page.</p>',
+            )
 
         with self.subTest('Standard Response - TemplateResponse Home Page'):
             response = self._get_page_response('django_expanded_test_cases:template-response-index')
-            self.assertPageContent(response, '<h1>Home Page Header</h1><p>Pretend this is the project landing page.</p>')
+            self.assertPageContent(
+                response,
+                '<h1>Home Page Header</h1><p>Pretend this is the project landing page.</p>',
+            )
 
         with self.subTest('Standard Response - One Message Page'):
             response = self._get_page_response('django_expanded_test_cases:response-with-one-message')
             self.assertPageContent(
                 response,
                 (
                     '<ul><li><p>This is a test message.</p></li></ul>'
@@ -1796,15 +2593,19 @@
                     'Pretend this',
                     'project landing',
                 ),
                 ignore_ordering=True,  # Ignore because we recheck the same values.
             )
 
         with self.subTest('Standard Response - Set of items on user page - As list'):
-            response = self._get_page_response('django_expanded_test_cases:user-detail', args=(1,), user=self.test_user)
+            response = self._get_page_response(
+                'django_expanded_test_cases:user-detail',
+                args=(1,),
+                user=self.test_user,
+            )
 
             # Standard, ordered page match.
             self.assertPageContent(
                 response,
                 [
                     '<h1>User Detail Page Header</h1>',
                     'Username: "test_superuser"',
@@ -1844,15 +2645,19 @@
                     'Last Name: "SuperUserLast"',
                     '<h1>User Detail Page Header</h1>',
                 ],
                 ignore_ordering=True,  # Ignore because unordered.
             )
 
         with self.subTest('Standard Response - Set of items on user page - As Tuple'):
-            response = self._get_page_response('django_expanded_test_cases:user-detail', args=(1,), user=self.test_user)
+            response = self._get_page_response(
+                'django_expanded_test_cases:user-detail',
+                args=(1,),
+                user=self.test_user,
+            )
 
             # Standard, ordered page match.
             self.assertPageContent(
                 response,
                 (
                     '<h1>User Detail Page Header</h1>',
                     'Username: "test_superuser"',
@@ -2062,33 +2867,42 @@
             'Expected content value was found, but ordering of values do not match. Problem value:\n{0}'
         )
 
         with self.subTest('Empty response, but value passed.'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('')
                 self.assertPageContent(response, '<h1>Test Title</h1>')
-            self.assertText(exception_msg_not_found.format('<h1>Test Title</h1>'), str(err.exception))
+            self.assertText(
+                exception_msg_not_found.format('<h1>Test Title</h1>'),
+                str(err.exception),
+            )
 
         with self.subTest('Minimal Response - Wrong value passed'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<h1>Test Title</h1>')
                 self.assertPageContent(response, '<h1>Testing</h1>')
-            self.assertText(exception_msg_not_found.format('<h1>Testing</h1>'), str(err.exception))
+            self.assertText(
+                exception_msg_not_found.format('<h1>Testing</h1>'),
+                str(err.exception),
+            )
 
         with self.subTest('Minimal Response - With additional error info provided.'):
             # First verify as standard not-found in array.
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<h1>Test Title</h1>')
                 self.assertPageContent(
                     response,
                     [
                         '<h1>Testing</h1>',
                     ],
                 )
-            self.assertText(exception_msg_not_found.format('<h1>Testing</h1>'), str(err.exception))
+            self.assertText(
+                exception_msg_not_found.format('<h1>Testing</h1>'),
+                str(err.exception),
+            )
 
             # Now actually verify same thing, but with extra error info (as list).
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<h1>Test Title</h1>')
                 self.assertPageContent(
                     response,
                     [
@@ -2121,15 +2935,18 @@
                 self.assertPageContent(
                     response,
                     [
                         '<h1>Testing</h1>',
                     ],
                     ignore_ordering=True,
                 )
-            self.assertText(exception_msg_not_found.format('<h1>Testing</h1>'), str(err.exception))
+            self.assertText(
+                exception_msg_not_found.format('<h1>Testing</h1>'),
+                str(err.exception),
+            )
 
             # Now actually verify same thing, but with extra error info (as list).
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<h1>Test Title</h1>')
                 self.assertPageContent(
                     response,
                     [
@@ -2167,53 +2984,128 @@
             )
 
         with self.subTest('Standard Response - Set of items with wrong values'):
             response = self._get_page_response('django_expanded_test_cases:index')
 
             # Test as list.
             with self.assertRaises(AssertionError) as err:
-                self.assertPageContent(response, ['<h1>Test Page Header</h1>'])
-            self.assertTextStartsWith(exception_msg_not_found.format('<h1>Test Page Header</h1>'), str(err.exception))
+                self.assertPageContent(
+                    response,
+                    ['<h1>Test Page Header</h1>'],
+                )
+            self.assertTextStartsWith(
+                exception_msg_not_found.format('<h1>Test Page Header</h1>'),
+                str(err.exception),
+            )
             with self.assertRaises(AssertionError) as err:
-                self.assertPageContent(response, ['Wrong Content'])
-            self.assertTextStartsWith(exception_msg_not_found.format('Wrong Content'), str(err.exception))
+                self.assertPageContent(
+                    response,
+                    ['Wrong Content'],
+                )
+            self.assertTextStartsWith(
+                exception_msg_not_found.format('Wrong Content'),
+                str(err.exception),
+            )
             with self.assertRaises(AssertionError) as err:
-                self.assertPageContent(response, ['<h1>Home Page Wrong'])
-            self.assertTextStartsWith(exception_msg_not_found.format('<h1>Home Page Wrong'), str(err.exception))
+                self.assertPageContent(
+                    response,
+                    ['<h1>Home Page Wrong'],
+                )
+            self.assertTextStartsWith(
+                exception_msg_not_found.format('<h1>Home Page Wrong'),
+                str(err.exception),
+            )
             with self.assertRaises(AssertionError) as err:
-                self.assertPageContent(response, ['Wrong Page Header</h1>'])
-            self.assertTextStartsWith(exception_msg_not_found.format('Wrong Page Header</h1>'), str(err.exception))
+                self.assertPageContent(
+                    response,
+                    ['Wrong Page Header</h1>'],
+                )
+            self.assertTextStartsWith(
+                exception_msg_not_found.format('Wrong Page Header</h1>'),
+                str(err.exception),
+            )
             with self.assertRaises(AssertionError) as err:
-                self.assertPageContent(response, ['<h1>Home Page Header</h1>', 'Wrong text'])
-            self.assertTextStartsWith(exception_msg_not_found.format('Wrong text'), str(err.exception))
+                self.assertPageContent(
+                    response,
+                    ['<h1>Home Page Header</h1>', 'Wrong text'],
+                )
+            self.assertTextStartsWith(
+                exception_msg_not_found.format('Wrong text'),
+                str(err.exception),
+            )
             with self.assertRaises(AssertionError) as err:
-                self.assertPageContent(response, ['<h1>Wrong Header</h1>', 'project landing page'])
-            self.assertTextStartsWith(exception_msg_not_found.format('<h1>Wrong Header</h1>'), str(err.exception))
+                self.assertPageContent(
+                    response,
+                    ['<h1>Wrong Header</h1>', 'project landing page'],
+                )
+            self.assertTextStartsWith(
+                exception_msg_not_found.format('<h1>Wrong Header</h1>'),
+                str(err.exception),
+            )
             # Test as tuple.
             with self.assertRaises(AssertionError) as err:
-                self.assertPageContent(response, ('<h1>Test Page Header</h1>',))
-            self.assertTextStartsWith(exception_msg_not_found.format('<h1>Test Page Header</h1>'), str(err.exception))
+                self.assertPageContent(
+                    response,
+                    ('<h1>Test Page Header</h1>',),
+                )
+            self.assertTextStartsWith(
+                exception_msg_not_found.format('<h1>Test Page Header</h1>'),
+                str(err.exception),
+            )
             with self.assertRaises(AssertionError) as err:
-                self.assertPageContent(response, ('Wrong Content',))
-            self.assertTextStartsWith(exception_msg_not_found.format('Wrong Content'), str(err.exception))
+                self.assertPageContent(
+                    response,
+                    ('Wrong Content',),
+                )
+            self.assertTextStartsWith(
+                exception_msg_not_found.format('Wrong Content'),
+                str(err.exception),
+            )
             with self.assertRaises(AssertionError) as err:
-                self.assertPageContent(response, ('<h1>Home Page Wrong',))
-            self.assertTextStartsWith(exception_msg_not_found.format('<h1>Home Page Wrong'), str(err.exception))
+                self.assertPageContent(
+                    response,
+                    ('<h1>Home Page Wrong',),
+                )
+            self.assertTextStartsWith(
+                exception_msg_not_found.format('<h1>Home Page Wrong'),
+                str(err.exception),
+            )
             with self.assertRaises(AssertionError) as err:
-                self.assertPageContent(response, ('Wrong Page Header</h1>',))
-            self.assertTextStartsWith(exception_msg_not_found.format('Wrong Page Header</h1>'), str(err.exception))
+                self.assertPageContent(
+                    response,
+                    ('Wrong Page Header</h1>',),
+                )
+            self.assertTextStartsWith(
+                exception_msg_not_found.format('Wrong Page Header</h1>'),
+                str(err.exception),
+            )
             with self.assertRaises(AssertionError) as err:
-                self.assertPageContent(response, ('<h1>Home Page Header</h1>', 'Wrong text'))
-            self.assertTextStartsWith(exception_msg_not_found.format('Wrong text'), str(err.exception))
+                self.assertPageContent(
+                    response,
+                    ('<h1>Home Page Header</h1>', 'Wrong text'),
+                )
+            self.assertTextStartsWith(
+                exception_msg_not_found.format('Wrong text'),
+                str(err.exception),
+            )
             with self.assertRaises(AssertionError) as err:
-                self.assertPageContent(response, ('<h1>Wrong Header</h1>', 'project landing page'))
-            self.assertTextStartsWith(exception_msg_not_found.format('<h1>Wrong Header</h1>'), str(err.exception))
+                self.assertPageContent(
+                    response,
+                    ('<h1>Wrong Header</h1>', 'project landing page'),
+                )
+            self.assertTextStartsWith(
+                exception_msg_not_found.format('<h1>Wrong Header</h1>'),
+                str(err.exception),
+            )
 
         with self.subTest('Standard Response - Wrong ordering'):
-            response = self._get_page_response('django_expanded_test_cases:user-detail', args=(1,))
+            response = self._get_page_response(
+                'django_expanded_test_cases:user-detail',
+                args=(1,),
+            )
 
             with self.assertRaises(AssertionError) as err:
                 # Test "first name" string at top.
                 self.assertPageContent(
                     response,
                     [
                         'First Name: "SuperUserFirst"',
@@ -2221,15 +3113,18 @@
                         'Username: "test_superuser"',
                         'Last Name: "SuperUserLast"',
                         'Is Active: "True"',
                         'Is SuperUser: "True"',
                         'Is Staff: "False"',
                     ],
                 )
-            self.assertTextStartsWith(exception_msg_bad_order.format('<h1>User Detail Page Header</h1>'), str(err.exception))
+            self.assertTextStartsWith(
+                exception_msg_bad_order.format('<h1>User Detail Page Header</h1>'),
+                str(err.exception),
+            )
 
             with self.assertRaises(AssertionError) as err:
                 # Test "first name" string after header.
                 self.assertPageContent(
                     response,
                     [
                         '<h1>User Detail Page Header</h1>',
@@ -2237,15 +3132,18 @@
                         'Username: "test_superuser"',
                         'Last Name: "SuperUserLast"',
                         'Is Active: "True"',
                         'Is SuperUser: "True"',
                         'Is Staff: "False"',
                     ],
                 )
-            self.assertTextStartsWith(exception_msg_bad_order.format('Username: "test_superuser"'), str(err.exception))
+            self.assertTextStartsWith(
+                exception_msg_bad_order.format('Username: "test_superuser"'),
+                str(err.exception),
+            )
 
             with self.assertRaises(AssertionError) as err:
                 # Test "first name" string after last name.
                 self.assertPageContent(
                     response,
                     [
                         '<h1>User Detail Page Header</h1>',
@@ -2253,15 +3151,18 @@
                         'Last Name: "SuperUserLast"',
                         'First Name: "SuperUserFirst"',
                         'Is Active: "True"',
                         'Is SuperUser: "True"',
                         'Is Staff: "False"',
                     ],
                 )
-            self.assertTextStartsWith(exception_msg_bad_order.format('First Name: "SuperUserFirst"'), str(err.exception))
+            self.assertTextStartsWith(
+                exception_msg_bad_order.format('First Name: "SuperUserFirst"'),
+                str(err.exception),
+            )
 
             with self.assertRaises(AssertionError) as err:
                 # Test "first name" string after active.
                 self.assertPageContent(
                     response,
                     [
                         '<h1>User Detail Page Header</h1>',
@@ -2269,15 +3170,18 @@
                         'Last Name: "SuperUserLast"',
                         'Is Active: "True"',
                         'First Name: "SuperUserFirst"',
                         'Is SuperUser: "True"',
                         'Is Staff: "False"',
                     ],
                 )
-            self.assertTextStartsWith(exception_msg_bad_order.format('First Name: "SuperUserFirst"'), str(err.exception))
+            self.assertTextStartsWith(
+                exception_msg_bad_order.format('First Name: "SuperUserFirst"'),
+                str(err.exception),
+            )
 
             with self.assertRaises(AssertionError) as err:
                 # Test "first name" string after superuser.
                 self.assertPageContent(
                     response,
                     [
                         '<h1>User Detail Page Header</h1>',
@@ -2285,15 +3189,18 @@
                         'Last Name: "SuperUserLast"',
                         'Is Active: "True"',
                         'Is SuperUser: "True"',
                         'First Name: "SuperUserFirst"',
                         'Is Staff: "False"',
                     ],
                 )
-            self.assertTextStartsWith(exception_msg_bad_order.format('First Name: "SuperUserFirst"'), str(err.exception))
+            self.assertTextStartsWith(
+                exception_msg_bad_order.format('First Name: "SuperUserFirst"'),
+                str(err.exception),
+            )
 
             with self.assertRaises(AssertionError) as err:
                 # Test "first name" string after staff.
                 self.assertPageContent(
                     response,
                     [
                         '<h1>User Detail Page Header</h1>',
@@ -2301,37 +3208,46 @@
                         'Last Name: "SuperUserLast"',
                         'Is Active: "True"',
                         'Is SuperUser: "True"',
                         'Is Staff: "False"',
                         'First Name: "SuperUserFirst"',
                     ],
                 )
-            self.assertTextStartsWith(exception_msg_bad_order.format('First Name: "SuperUserFirst"'), str(err.exception))
+            self.assertTextStartsWith(
+                exception_msg_bad_order.format('First Name: "SuperUserFirst"'),
+                str(err.exception),
+            )
 
     def test__assertPageContent__failure__with_bad_search_space(self):
         exception_msg = 'Could not find "{0}" value in content response. Provided value was:\n{1}'
         response = self._get_page_response('django_expanded_test_cases:index')
 
         # Bad content_starts_after values.
         with self.subTest('With content_starts_after not found'):
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content='<h1>Home Page Header</h1>',
                     content_starts_after='Wrong value.',
                 )
-            self.assertText(exception_msg.format('content_starts_after', 'Wrong value.'), str(err.exception))
+            self.assertText(
+                exception_msg.format('content_starts_after', 'Wrong value.'),
+                str(err.exception),
+            )
         with self.subTest('With content_starts_after not found'):
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content='Wrong content value.',
                     content_starts_after='Wrong value.',
                 )
-            self.assertText(exception_msg.format('content_starts_after', 'Wrong value.'), str(err.exception))
+            self.assertText(
+                exception_msg.format('content_starts_after', 'Wrong value.'),
+                str(err.exception),
+            )
         with self.subTest('With content_starts_after found with extra'):
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content='<h1>Home Page Header</h1>',
                     content_starts_after='Home Page Header plus Extra',
                 )
@@ -2344,23 +3260,29 @@
         with self.subTest('With content_ends_before not found'):
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content='<h1>Home Page Header</h1>',
                     content_ends_before='Wrong value.',
                 )
-            self.assertText(exception_msg.format('content_ends_before', 'Wrong value.'), str(err.exception))
+            self.assertText(
+                exception_msg.format('content_ends_before', 'Wrong value.'),
+                str(err.exception),
+            )
         with self.subTest('With content_ends_before and expected_content not found'):
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content='Wrong content value.',
                     content_ends_before='Wrong value.',
                 )
-            self.assertText(exception_msg.format('content_ends_before', 'Wrong value.'), str(err.exception))
+            self.assertText(
+                exception_msg.format('content_ends_before', 'Wrong value.'),
+                str(err.exception),
+            )
         with self.subTest('With content_ends_before found with extra'):
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content='<h1>Home Page Header</h1>',
                     content_ends_before='Home Page Header plus Extra',
                 )
@@ -2377,56 +3299,74 @@
             # Expected as single value.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content='<head>',
                     content_starts_after='<h1>Home Page Header</h1>',
                 )
-            self.assertText(exception_msg.format('content_starts_after', '<head>'), str(err.exception))
+            self.assertText(
+                exception_msg.format('content_starts_after', '<head>'),
+                str(err.exception),
+            )
             # Expected as single value.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content='<meta charset="utf-8">',
                     content_starts_after='<h1>Home Page Header</h1>',
                 )
-            self.assertText(exception_msg.format('content_starts_after', '<meta charset="utf-8">'), str(err.exception))
+            self.assertText(
+                exception_msg.format('content_starts_after', '<meta charset="utf-8">'),
+                str(err.exception),
+            )
             # Expected as single value.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content='</head>',
                     content_starts_after='<h1>Home Page Header</h1>',
                     ignore_ordering=True,
                 )
-            self.assertText(exception_msg.format('content_starts_after', '</head>'), str(err.exception))
+            self.assertText(
+                exception_msg.format('content_starts_after', '</head>'),
+                str(err.exception),
+            )
             # Expected as single value.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content='<body>',
                     content_starts_after='<h1>Home Page Header</h1>',
                 )
-            self.assertText(exception_msg.format('content_starts_after', '<body>'), str(err.exception))
+            self.assertText(
+                exception_msg.format('content_starts_after', '<body>'),
+                str(err.exception),
+            )
             # Expected as single value - With exact match.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content='<h1>Home Page Header</h1>',
                     content_starts_after='<h1>Home Page Header</h1>',
                 )
-            self.assertText(exception_msg.format('content_starts_after', '<h1>Home Page Header</h1>'), str(err.exception))
+            self.assertText(
+                exception_msg.format('content_starts_after', '<h1>Home Page Header</h1>'),
+                str(err.exception),
+            )
             # Expected as single value - With partial of exact match.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content='h1>',
                     content_starts_after='<h1>Home Page Header</h1>',
                 )
-            self.assertText(exception_msg.format('content_starts_after', 'h1>'), str(err.exception))
+            self.assertText(
+                exception_msg.format('content_starts_after', 'h1>'),
+                str(err.exception),
+            )
 
             # Expected as array.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content=[
                         '<meta charset="utf-8">',
@@ -2475,23 +3415,29 @@
             # Expected as single value - Exact match.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content='<h1>Home Page Header</h1>',
                     content_ends_before='<h1>Home Page Header</h1>',
                 )
-            self.assertText(exception_msg.format('content_ends_before', '<h1>Home Page Header</h1>'), str(err.exception))
+            self.assertText(
+                exception_msg.format('content_ends_before', '<h1>Home Page Header</h1>'),
+                str(err.exception),
+            )
             # Expected as single value - Partial of exact match.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content='h1>',
                     content_ends_before='<h1>Home Page Header</h1>',
                 )
-            self.assertText(exception_msg.format('content_ends_before', 'h1>'), str(err.exception))
+            self.assertText(
+                exception_msg.format('content_ends_before', 'h1>'),
+                str(err.exception),
+            )
             # Expected as single value.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content='<p>Pretend this is the project landing page.</p>',
                     content_ends_before='<h1>Home Page Header</h1>',
                 )
@@ -2514,15 +3460,18 @@
             # Expected as single value.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content='</body>',
                     content_ends_before='<h1>Home Page Header</h1>',
                 )
-            self.assertText(exception_msg.format('content_ends_before', '</body>'), str(err.exception))
+            self.assertText(
+                exception_msg.format('content_ends_before', '</body>'),
+                str(err.exception),
+            )
 
             # Expected as array.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content=[
                         '<p>Pretend this is the project landing page.</p>',
@@ -2556,15 +3505,18 @@
                     expected_content=[
                         '</body>',
                         '<p>Pretend this is the project landing page.</p>',
                     ],
                     ignore_ordering=True,
                     content_ends_before='<h1>Home Page Header</h1>',
                 )
-            self.assertTextStartsWith(exception_msg.format('content_ends_before', '</body>'), str(err.exception))
+            self.assertTextStartsWith(
+                exception_msg.format('content_ends_before', '</body>'),
+                str(err.exception),
+            )
 
         with self.subTest('Standard Response - With both content containers defined'):
             response = self._get_page_response('django_expanded_test_cases:index')
 
             # Expected as single value - above search area.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
@@ -2593,15 +3545,18 @@
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content='</body>',
                     content_starts_after='<title>Home Page | Test Views</title>',
                     content_ends_before='<p>Pretend this is the project landing page.</p>',
                 )
-            self.assertText(exception_msg.format('content_ends_before', '</body>'), str(err.exception))
+            self.assertText(
+                exception_msg.format('content_ends_before', '</body>'),
+                str(err.exception),
+            )
             # Expected as single value - below search area, exact match.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content='<p>Pretend this is the project landing page.</p>',
                     content_starts_after='<title>Home Page | Test Views</title>',
                     content_ends_before='<p>Pretend this is the project landing page.</p>',
@@ -2631,28 +3586,34 @@
                     expected_content=[
                         '<head>',
                         '<meta charset="utf-8">',
                     ],
                     content_starts_after='<title>Home Page | Test Views</title>',
                     content_ends_before='<p>Pretend this is the project landing page.</p>',
                 )
-            self.assertTextStartsWith(exception_msg.format('content_starts_after', '<head>'), str(err.exception))
+            self.assertTextStartsWith(
+                exception_msg.format('content_starts_after', '<head>'),
+                str(err.exception),
+            )
             # Expected as array - Above search area, with ignore_ordering.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content=[
                         '<head>',
                         '<meta charset="utf-8">',
                     ],
                     ignore_ordering=True,
                     content_starts_after='<title>Home Page | Test Views</title>',
                     content_ends_before='<p>Pretend this is the project landing page.</p>',
                 )
-            self.assertTextStartsWith(exception_msg.format('content_starts_after', '<head>'), str(err.exception))
+            self.assertTextStartsWith(
+                exception_msg.format('content_starts_after', '<head>'),
+                str(err.exception),
+            )
             # Expected as array - Above search area, with ignore_ordering and content mis-ordered.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content=[
                         '<meta charset="utf-8">',
                         '<head>',
@@ -2704,15 +3665,18 @@
                         '</body>',
                         'the project landing page.</p>',
                     ],
                     ignore_ordering=True,
                     content_starts_after='<title>Home Page | Test Views</title>',
                     content_ends_before='<p>Pretend this is',
                 )
-            self.assertTextStartsWith(exception_msg.format('content_ends_before', '</body>'), str(err.exception))
+            self.assertTextStartsWith(
+                exception_msg.format('content_ends_before', '</body>'),
+                str(err.exception),
+            )
 
     def test__assertPageContent__fail__with_content_casing_mismatch__exact_match(self):
         exception_msg = (
             'Expected content value was found, but letter capitalization did not match. Expected was:\n'
             '{0}\n'
             '\n'
             'Found was:\n'
@@ -3127,43 +4091,1058 @@
         with self.subTest('Standard Response - With response mixed and check upper'):
             with self.assertRaises(AssertionError) as err:
                 response = self._get_page_response('django_expanded_test_cases:index')
                 self.assertPageContent(response, '<H1>HOME PAGE HEADER</H1>')
             self.assertText(
                 exception_msg.format(
                     '<H1>HOME PAGE HEADER</H1>',
-                    '... /title></head><body><h1>Home Page Header</h1><p>Pretend this is t ...'
+                    '... /title></head><body><h1>Home Page Header</h1><p>Pretend this is t ...',
                 ),
                 str(err.exception),
             )
 
         with self.subTest('Standard Response - With response mixed and check lower'):
             with self.assertRaises(AssertionError) as err:
                 response = self._get_page_response('django_expanded_test_cases:index')
                 self.assertPageContent(response, '<h1>home page header</h1>')
             self.assertText(
                 exception_msg.format(
                     '<h1>home page header</h1>',
-                    '... /title></head><body><h1>Home Page Header</h1><p>Pretend this is t ...'
+                    '... /title></head><body><h1>Home Page Header</h1><p>Pretend this is t ...',
                 ),
                 str(err.exception),
             )
 
         with self.subTest('Standard Response - With response mixed and check mixed'):
             with self.assertRaises(AssertionError) as err:
                 response = self._get_page_response('django_expanded_test_cases:index')
                 self.assertPageContent(response, '<h1>home Page header</h1>')
             self.assertText(
                 exception_msg.format(
                     '<h1>home Page header</h1>',
-                    '... /title></head><body><h1>Home Page Header</h1><p>Pretend this is t ...'
+                    '... /title></head><body><h1>Home Page Header</h1><p>Pretend this is t ...',
+                ),
+                str(err.exception),
+            )
+
+    def test__assertPageContent__edge_case__user_content_has_str_format_syntax__single_assertion(self):
+        """Testing with assertPageContent when user content has string formatting syntax.
+        Such as { or } characters, without the matching equivalent other side.
+
+        When dealing with only a single statement to check for in content.
+        """
+
+        with self.subTest('Success Check - Has { character.'):
+
+            response = HttpResponse('<title>My title has { in it, oops!</title>')
+            self.assertPageContent(response, '<title>My title has { in it, oops!</title>')
+
+        with self.subTest('Success Check - Has } character.'):
+
+            response = HttpResponse('<title>My title has } in it, oops!</title>')
+            self.assertPageContent(response, '<title>My title has } in it, oops!</title>')
+
+        with self.subTest('Success Check - Has { and } characters (standard order).'):
+
+            response = HttpResponse('<title>My title has { and } in it, oops!</title>')
+            self.assertPageContent(response, '<title>My title has { and } in it, oops!</title>')
+
+        with self.subTest('Success Check - Has { and } characters (reverse order).'):
+
+            response = HttpResponse('<title>My title has } and { in it, oops!</title>')
+            self.assertPageContent(response, '<title>My title has } and { in it, oops!</title>')
+
+        with self.subTest('Failure Check - Expected { character.'):
+
+            response = HttpResponse('<title>Test Title</title>')
+
+            # Expecting single character.
+            with self.assertRaises(AssertionError) as err:
+                self.assertPageContent(response, '{')
+            self.assertEqual(
+                (
+                    # So black does not one-line this.
+                    'Could not find expected content value in response. Provided value was:\n'
+                    '{\n'
+                ),
+                str(err.exception),
+            )
+
+            # Expecting single character in tag.
+            with self.assertRaises(AssertionError) as err:
+                self.assertPageContent(response, '<title>{</title>')
+            self.assertEqual(
+                (
+                    # So black does not one-line this.
+                    'Could not find expected content value in response. Provided value was:\n'
+                    '<title>{</title>\n'
+                ),
+                str(err.exception),
+            )
+
+            # Full value.
+            with self.assertRaises(AssertionError) as err:
+                self.assertPageContent(response, '<title>My title has { in it, oops!</title>')
+            self.assertEqual(
+                (
+                    # So black does not one-line this.
+                    'Could not find expected content value in response. Provided value was:\n'
+                    '<title>My title has{in it, oops!</title>\n'
+                ),
+                str(err.exception),
+            )
+
+        with self.subTest('Failure Check - Expected } character.'):
+
+            response = HttpResponse('<title>Test Title</title>')
+
+            # Expecting single character.
+            with self.assertRaises(AssertionError) as err:
+                self.assertPageContent(response, '}')
+            self.assertEqual(
+                (
+                    # So black does not one-line this.
+                    'Could not find expected content value in response. Provided value was:\n'
+                    '}\n'
+                ),
+                str(err.exception),
+            )
+
+            # Expecting single character in tag.
+            with self.assertRaises(AssertionError) as err:
+                self.assertPageContent(response, '<title>}</title>')
+            self.assertEqual(
+                (
+                    # So black does not one-line this.
+                    'Could not find expected content value in response. Provided value was:\n'
+                    '<title>}</title>\n'
+                ),
+                str(err.exception),
+            )
+
+            # Full value.
+            with self.assertRaises(AssertionError) as err:
+                self.assertPageContent(response, '<title>My title has } in it, oops!</title>')
+            self.assertEqual(
+                (
+                    # So black does not one-line this.
+                    'Could not find expected content value in response. Provided value was:\n'
+                    '<title>My title has}in it, oops!</title>\n'
+                ),
+                str(err.exception),
+            )
+
+        with self.subTest('Failure Check - Expected { and } characters (standard order).'):
+
+            response = HttpResponse('<title>Test Title</title>')
+
+            # Expecting single character.
+            with self.assertRaises(AssertionError) as err:
+                self.assertPageContent(response, '{ }')
+            self.assertEqual(
+                (
+                    # So black does not one-line this.
+                    'Could not find expected content value in response. Provided value was:\n'
+                    '{}\n'
+                ),
+                str(err.exception),
+            )
+
+            # Expecting single character in tag.
+            with self.assertRaises(AssertionError) as err:
+                self.assertPageContent(response, '<title>{ }</title>')
+            self.assertEqual(
+                (
+                    # So black does not one-line this.
+                    'Could not find expected content value in response. Provided value was:\n'
+                    '<title>{}</title>\n'
+                ),
+                str(err.exception),
+            )
+
+            # Full value.
+            with self.assertRaises(AssertionError) as err:
+                self.assertPageContent(response, '<title>My title has { and } in it, oops!</title>')
+            self.assertEqual(
+                (
+                    # So black does not one-line this.
+                    'Could not find expected content value in response. Provided value was:\n'
+                    '<title>My title has{and}in it, oops!</title>\n'
+                ),
+                str(err.exception),
+            )
+
+        with self.subTest('Failure Check - Expected { and } characters (reverse order).'):
+
+            response = HttpResponse('<title>Test Title</title>')
+
+            # Expecting single character.
+            with self.assertRaises(AssertionError) as err:
+                self.assertPageContent(response, '} {')
+            self.assertEqual(
+                (
+                    # So black does not one-line this.
+                    'Could not find expected content value in response. Provided value was:\n'
+                    '}{\n'
+                ),
+                str(err.exception),
+            )
+
+            # Expecting single character in tag.
+            with self.assertRaises(AssertionError) as err:
+                self.assertPageContent(response, '<title>} {</title>')
+            self.assertEqual(
+                (
+                    # So black does not one-line this.
+                    'Could not find expected content value in response. Provided value was:\n'
+                    '<title>}{</title>\n'
+                ),
+                str(err.exception),
+            )
+
+            # Full value.
+            with self.assertRaises(AssertionError) as err:
+                self.assertPageContent(response, '<title>My title has } and { in it, oops!</title>')
+            self.assertEqual(
+                (
+                    # So black does not one-line this.
+                    'Could not find expected content value in response. Provided value was:\n'
+                    '<title>My title has}and{in it, oops!</title>\n'
                 ),
                 str(err.exception),
             )
 
+        with self.subTest('Failure Check - Didn\'t expect { character.'):
+
+            response = HttpResponse('<title>My title has { in it, oops!</title>')
+
+            with self.assertRaises(AssertionError) as err:
+                self.assertPageContent(response, '<title>My title has  in it, oops!</title>')
+            self.assertEqual(
+                (
+                    'Could not find expected content value in response. Provided value was:\n'
+                    '<title>My title has in it, oops!</title>\n'
+                ),
+                str(err.exception),
+            )
+
+        with self.subTest('Failure Check - Didn\'t expect } character.'):
+
+            response = HttpResponse('<title>My title has } in it, oops!</title>')
+
+            with self.assertRaises(AssertionError) as err:
+                self.assertPageContent(response, '<title>My title has  in it, oops!</title>')
+            self.assertEqual(
+                (
+                    'Could not find expected content value in response. Provided value was:\n'
+                    '<title>My title has in it, oops!</title>\n'
+                ),
+                str(err.exception),
+            )
+
+        with self.subTest('Failure Check - Didn\'t expect { and } characters (standard order).'):
+
+            response = HttpResponse('<title>My title has { and } in it, oops!</title>')
+
+            with self.assertRaises(AssertionError) as err:
+                self.assertPageContent(response, '<title>My title has  in it, oops!</title>')
+            self.assertEqual(
+                (
+                    'Could not find expected content value in response. Provided value was:\n'
+                    '<title>My title has in it, oops!</title>\n'
+                ),
+                str(err.exception),
+            )
+
+        with self.subTest('Failure Check - Didn\'t expect { and } characters (reverse order).'):
+
+            response = HttpResponse('<title>My title has } and { in it, oops!</title>')
+
+            with self.assertRaises(AssertionError) as err:
+                self.assertPageContent(response, '<title>My title has  in it, oops!</title>')
+            self.assertEqual(
+                (
+                    'Could not find expected content value in response. Provided value was:\n'
+                    '<title>My title has in it, oops!</title>\n'
+                ),
+                str(err.exception),
+            )
+
+    def test__assertPageContent__edge_case__user_content_has_str_format_syntax__multi_assertion(self):
+        """Testing with assertPageContent when user content has string formatting syntax.
+        Such as { or } characters, without the matching equivalent other side.
+
+        When dealing with multiple statements to check for in content.
+        """
+
+        with self.subTest('Success Check - Has { character.'):
+
+            # Generate response.
+            response = HttpResponse('<title>My title has { in it, oops!</title>')
+
+            self.assertPageContent(
+                response,
+                [
+                    '<title>',
+                    'My',
+                    'title',
+                    'has',
+                    '{',
+                    'in it,',
+                    'oops!',
+                    '</title>',
+                ],
+            )
+
+        with self.subTest('Success Check - Has } character.'):
+
+            # Generate response.
+            response = HttpResponse('<title>My title has } in it, oops!</title>')
+
+            self.assertPageContent(
+                response,
+                [
+                    '<title>',
+                    'My',
+                    'title',
+                    'has',
+                    '}',
+                    'in it,',
+                    'oops!',
+                    '</title>',
+                ],
+            )
+
+        with self.subTest('Success Check - Has { and } characters (standard order).'):
+
+            # Generate response.
+            response = HttpResponse('<title>My title has { and } in it, oops!</title>')
+
+            self.assertPageContent(
+                response,
+                [
+                    '<title>',
+                    'My',
+                    'title',
+                    'has',
+                    '{ and }',
+                    'in it,',
+                    'oops!',
+                    '</title>',
+                ],
+            )
+
+        with self.subTest('Success Check - Has { and } characters (reverse order).'):
+
+            # Generate response.
+            response = HttpResponse('<title>My title has } and { in it, oops!</title>')
+
+            self.assertPageContent(
+                response,
+                [
+                    '<title>',
+                    'My',
+                    'title',
+                    'has',
+                    '} and {',
+                    'in it,',
+                    'oops!',
+                    '</title>',
+                ],
+            )
+
+        with self.subTest('Failure Check - Expected { character.'):
+
+            # Generate response.
+            response = HttpResponse('<title>My title has blah in it, oops!</title>')
+
+            with self.assertRaises(AssertionError) as err:
+                self.assertPageContent(
+                    response,
+                    [
+                        '<title>',
+                        'My',
+                        'title',
+                        'has',
+                        '{',
+                        'in it,',
+                        'oops!',
+                        '</title>',
+                    ],
+                )
+            self.assertTextStartsWith(
+                'Could not find expected content value in response. Provided value was:\n',
+                str(err.exception),
+            )
+
+        with self.subTest('Failure Check - Expected } character.'):
+            # Generate response.
+            response = HttpResponse('<title>My title has blah in it, oops!</title>')
+
+            # Expecting single character.
+            with self.assertRaises(AssertionError) as err:
+                self.assertPageContent(
+                    response,
+                    [
+                        '<title>',
+                        'My',
+                        'title',
+                        'has',
+                        '}',
+                        'in it,',
+                        'oops!',
+                        '</title>',
+                    ],
+                )
+            self.assertTextStartsWith(
+                'Could not find expected content value in response. Provided value was:\n',
+                str(err.exception),
+            )
+
+        with self.subTest('Failure Check - Expected { and } characters (standard order).'):
+            # Generate response.
+            response = HttpResponse('<title>My title has blah in it, oops!</title>')
+
+            # Expecting single character.
+            with self.assertRaises(AssertionError) as err:
+                self.assertPageContent(
+                    response,
+                    [
+                        '<title>',
+                        'My',
+                        'title',
+                        'has',
+                        '{ and }',
+                        'in it,',
+                        'oops!',
+                        '</title>',
+                    ],
+                )
+            self.assertTextStartsWith(
+                'Could not find expected content value in response. Provided value was:\n',
+                str(err.exception),
+            )
+
+        with self.subTest('Failure Check - Expected { and } characters (reverse order).'):
+            # Generate response.
+            response = HttpResponse('<title>My title has blah in it, oops!</title>')
+
+            # Expecting single character.
+            with self.assertRaises(AssertionError) as err:
+                self.assertPageContent(
+                    response,
+                    [
+                        '<title>',
+                        'My',
+                        'title',
+                        'has',
+                        '} and {',
+                        'in it,',
+                        'oops!',
+                        '</title>',
+                    ],
+                )
+            self.assertTextStartsWith(
+                'Could not find expected content value in response. Provided value was:\n',
+                str(err.exception),
+            )
+
+        with self.subTest('Failure Check - Didn\'t expect { character.'):
+
+            response = HttpResponse('<title>My title has { in it, oops!</title>')
+
+            with self.assertRaises(AssertionError) as err:
+                self.assertPageContent(
+                    response,
+                    [
+                        '<title>',
+                        'My',
+                        'title',
+                        'has in it,',
+                        'oops!',
+                        '</title>',
+                    ],
+                )
+            self.assertTextStartsWith(
+                'Could not find expected content value in response. Provided value was:\n',
+                str(err.exception),
+            )
+
+        with self.subTest('Failure Check - Didn\'t expect } character.'):
+
+            response = HttpResponse('<title>My title has } in it, oops!</title>')
+
+            with self.assertRaises(AssertionError) as err:
+                self.assertPageContent(
+                    response,
+                    [
+                        '<title>',
+                        'My',
+                        'title',
+                        'has in it,',
+                        'oops!',
+                        '</title>',
+                    ],
+                )
+            self.assertTextStartsWith(
+                'Could not find expected content value in response. Provided value was:\n',
+                str(err.exception),
+            )
+
+        with self.subTest('Failure Check - Didn\'t expect { and } characters (standard order).'):
+
+            response = HttpResponse('<title>My title has { and } in it, oops!</title>')
+
+            with self.assertRaises(AssertionError) as err:
+                self.assertPageContent(
+                    response,
+                    [
+                        '<title>',
+                        'My',
+                        'title',
+                        'has in it,',
+                        'oops!',
+                        '</title>',
+                    ],
+                )
+            self.assertTextStartsWith(
+                'Could not find expected content value in response. Provided value was:\n',
+                str(err.exception),
+            )
+
+        with self.subTest('Failure Check - Didn\'t expect { and } characters (reverse order).'):
+
+            response = HttpResponse('<title>My title has } and { in it, oops!</title>')
+
+            with self.assertRaises(AssertionError) as err:
+                self.assertPageContent(
+                    response,
+                    [
+                        '<title>',
+                        'My',
+                        'title',
+                        'has in it,',
+                        'oops!',
+                        '</title>',
+                    ],
+                )
+            self.assertTextStartsWith(
+                'Could not find expected content value in response. Provided value was:\n',
+                str(err.exception),
+            )
+
+    def test__assertPageContent__verifying_contextual_output__default(self):
+        """Verifies contextual output for assertContent, when multiple values are provided in a single statement.
+        This tests the default setting value.
+        """
+        response = HttpResponse('<span>This is my test span.</span>')
+
+        if COLORAMA_PRESENT:
+            output_color_before = ETC_OUTPUT_EXPECTED_MATCH_COLOR
+            output_color_after = ETC_OUTPUT_ACTUALS_MATCH_COLOR
+            output_color_error = ETC_OUTPUT_ERROR_COLOR
+            output_color_reset = ETC_OUTPUT_RESET_COLOR
+        else:
+            output_color_before = ''
+            output_color_after = ''
+            output_color_error = ''
+            output_color_reset = ''
+
+        # Test with full values.
+        with self.assertRaises(AssertionError) as err:
+            self.assertPageContent(
+                response,
+                [
+                    '<span>',
+                    'This',
+                    'is',
+                    'my',
+                    'testing',
+                    'span',
+                    '.',
+                    '</span>',
+                ]
+            )
+        self.assertText(
+            (
+                'Could not find expected content value in response. Provided value was:\n'
+                'testing\n'
+                '\n'
+                '\n'
+                'Surrounding Checks:\n'
+                '{1}Content Checks Before:{0}\n'
+                '{1}    * is{0}\n'
+                '{1}    * my{0}\n'
+                '{2}Failed Check:{0}\n'
+                '{2}  > * testing{0}\n'
+                '{3}Content Checks After:{0}\n'
+                '{3}    * span{0}\n'
+                '{3}    * .{0}\n'
+            ).format(
+                output_color_reset,
+                output_color_before,
+                output_color_error,
+                output_color_after,
+            ),
+            str(err.exception),
+        )
+
+        # Test missing before.
+        with self.assertRaises(AssertionError) as err:
+            self.assertPageContent(
+                response,
+                [
+                    'testing',
+                    'span',
+                    '.',
+                    '</span>',
+                ]
+            )
+        self.assertText(
+            (
+                'Could not find expected content value in response. Provided value was:\n'
+                'testing\n'
+                '\n'
+                '\n'
+                'Surrounding Checks:\n'
+                '{2}Failed Check:{0}\n'
+                '{2}  > * testing{0}\n'
+                '{3}Content Checks After:{0}\n'
+                '{3}    * span{0}\n'
+                '{3}    * .{0}\n'
+            ).format(
+                output_color_reset,
+                output_color_before,
+                output_color_error,
+                output_color_after,
+            ),
+            str(err.exception),
+        )
+
+        # Test missing after.
+        with self.assertRaises(AssertionError) as err:
+            self.assertPageContent(
+                response,
+                [
+                    '<span>',
+                    'This',
+                    'is',
+                    'my',
+                    'testing',
+                ]
+            )
+        self.assertText(
+            (
+                'Could not find expected content value in response. Provided value was:\n'
+                'testing\n'
+                '\n'
+                '\n'
+                'Surrounding Checks:\n'
+                '{1}Content Checks Before:{0}\n'
+                '{1}    * is{0}\n'
+                '{1}    * my{0}\n'
+                '{2}Failed Check:{0}\n'
+                '{2}  > * testing{0}\n'
+            ).format(
+                output_color_reset,
+                output_color_before,
+                output_color_error,
+                output_color_after,
+            ),
+            str(err.exception),
+        )
+
+        # Test only one per side.
+        with self.assertRaises(AssertionError) as err:
+            self.assertPageContent(
+                response,
+                [
+                    'my',
+                    'testing',
+                    'span',
+                ]
+            )
+        self.assertText(
+            (
+                'Could not find expected content value in response. Provided value was:\n'
+                'testing\n'
+                '\n'
+                '\n'
+                'Surrounding Checks:\n'
+                '{1}Content Checks Before:{0}\n'
+                '{1}    * my{0}\n'
+                '{2}Failed Check:{0}\n'
+                '{2}  > * testing{0}\n'
+                '{3}Content Checks After:{0}\n'
+                '{3}    * span{0}\n'
+            ).format(
+                output_color_reset,
+                output_color_before,
+                output_color_error,
+                output_color_after,
+            ),
+            str(err.exception),
+        )
+
+        # Test missing all.
+        with self.assertRaises(AssertionError) as err:
+            self.assertPageContent(
+                response,
+                [
+                    'testing',
+                ]
+            )
+        self.assertText(
+            (
+                'Could not find expected content value in response. Provided value was:\n'
+                'testing\n'
+            ),
+            str(err.exception),
+        )
+
+    @patch("django_expanded_test_cases.test_cases.integration_test_case.ETC_ASSERT_CONTENT__SURROUNDING_CHECK_OUTPUT_LENGTH", 1)
+    def test__assertPageContent__verifying_contextual_output__one(self):
+        """Verifies contextual output for assertContent, when multiple values are provided in a single statement.
+        This tests settings value of 1 contextual item output.
+        """
+        response = HttpResponse('<span>This is my test span.</span>')
+
+        if COLORAMA_PRESENT:
+            output_color_before = ETC_OUTPUT_EXPECTED_MATCH_COLOR
+            output_color_after = ETC_OUTPUT_ACTUALS_MATCH_COLOR
+            output_color_error = ETC_OUTPUT_ERROR_COLOR
+            output_color_reset = ETC_OUTPUT_RESET_COLOR
+        else:
+            output_color_before = ''
+            output_color_after = ''
+            output_color_error = ''
+            output_color_reset = ''
+
+        # Test with full values.
+        with self.assertRaises(AssertionError) as err:
+            self.assertPageContent(
+                response,
+                [
+                    '<span>',
+                    'This',
+                    'is',
+                    'my',
+                    'testing',
+                    'span',
+                    '.',
+                    '</span>',
+                ]
+            )
+        self.assertText(
+            (
+                'Could not find expected content value in response. Provided value was:\n'
+                'testing\n'
+                '\n'
+                '\n'
+                'Surrounding Checks:\n'
+                '{1}Content Checks Before:{0}\n'
+                '{1}    * my{0}\n'
+                '{2}Failed Check:{0}\n'
+                '{2}  > * testing{0}\n'
+                '{3}Content Checks After:{0}\n'
+                '{3}    * span{0}\n'
+            ).format(
+                output_color_reset,
+                output_color_before,
+                output_color_error,
+                output_color_after,
+            ),
+            str(err.exception),
+        )
+
+        # Test missing before.
+        with self.assertRaises(AssertionError) as err:
+            self.assertPageContent(
+                response,
+                [
+                    'testing',
+                    'span',
+                    '.',
+                    '</span>',
+                ]
+            )
+        self.assertText(
+            (
+                'Could not find expected content value in response. Provided value was:\n'
+                'testing\n'
+                '\n'
+                '\n'
+                'Surrounding Checks:\n'
+                '{2}Failed Check:{0}\n'
+                '{2}  > * testing{0}\n'
+                '{3}Content Checks After:{0}\n'
+                '{3}    * span{0}\n'
+            ).format(
+                output_color_reset,
+                output_color_before,
+                output_color_error,
+                output_color_after,
+            ),
+            str(err.exception),
+        )
+
+        # Test missing after.
+        with self.assertRaises(AssertionError) as err:
+            self.assertPageContent(
+                response,
+                [
+                    '<span>',
+                    'This',
+                    'is',
+                    'my',
+                    'testing',
+                ]
+            )
+        self.assertText(
+            (
+                'Could not find expected content value in response. Provided value was:\n'
+                'testing\n'
+                '\n'
+                '\n'
+                'Surrounding Checks:\n'
+                '{1}Content Checks Before:{0}\n'
+                '{1}    * my{0}\n'
+                '{2}Failed Check:{0}\n'
+                '{2}  > * testing{0}\n'
+            ).format(
+                output_color_reset,
+                output_color_before,
+                output_color_error,
+                output_color_after,
+            ),
+            str(err.exception),
+        )
+
+        # Test only one per side.
+        with self.assertRaises(AssertionError) as err:
+            self.assertPageContent(
+                response,
+                [
+                    'my',
+                    'testing',
+                    'span',
+                ]
+            )
+        self.assertText(
+            (
+                'Could not find expected content value in response. Provided value was:\n'
+                'testing\n'
+                '\n'
+                '\n'
+                'Surrounding Checks:\n'
+                '{1}Content Checks Before:{0}\n'
+                '{1}    * my{0}\n'
+                '{2}Failed Check:{0}\n'
+                '{2}  > * testing{0}\n'
+                '{3}Content Checks After:{0}\n'
+                '{3}    * span{0}\n'
+            ).format(
+                output_color_reset,
+                output_color_before,
+                output_color_error,
+                output_color_after,
+            ),
+            str(err.exception),
+        )
+
+        # Test missing all.
+        with self.assertRaises(AssertionError) as err:
+            self.assertPageContent(
+                response,
+                [
+                    'testing',
+                ]
+            )
+        self.assertText(
+            (
+                'Could not find expected content value in response. Provided value was:\n'
+                'testing\n'
+            ),
+            str(err.exception),
+        )
+
+    @patch("django_expanded_test_cases.test_cases.integration_test_case.ETC_ASSERT_CONTENT__SURROUNDING_CHECK_OUTPUT_LENGTH", 3)
+    def test__assertPageContent__verifying_contextual_output__three(self):
+        """Verifies contextual output for assertContent, when multiple values are provided in a single statement.
+        This tests settings value of 3 contextual item outputs.
+        """
+        response = HttpResponse('<span>This is my test span.</span>')
+
+        if COLORAMA_PRESENT:
+            output_color_before = ETC_OUTPUT_EXPECTED_MATCH_COLOR
+            output_color_after = ETC_OUTPUT_ACTUALS_MATCH_COLOR
+            output_color_error = ETC_OUTPUT_ERROR_COLOR
+            output_color_reset = ETC_OUTPUT_RESET_COLOR
+        else:
+            output_color_before = ''
+            output_color_after = ''
+            output_color_error = ''
+            output_color_reset = ''
+
+        # Test with full values.
+        with self.assertRaises(AssertionError) as err:
+            self.assertPageContent(
+                response,
+                [
+                    '<span>',
+                    'This',
+                    'is',
+                    'my',
+                    'testing',
+                    'span',
+                    '.',
+                    '</span>',
+                ]
+            )
+        self.assertText(
+            (
+                'Could not find expected content value in response. Provided value was:\n'
+                'testing\n'
+                '\n'
+                '\n'
+                'Surrounding Checks:\n'
+                '{1}Content Checks Before:{0}\n'
+                '{1}    * This{0}\n'
+                '{1}    * is{0}\n'
+                '{1}    * my{0}\n'
+                '{2}Failed Check:{0}\n'
+                '{2}  > * testing{0}\n'
+                '{3}Content Checks After:{0}\n'
+                '{3}    * span{0}\n'
+                '{3}    * .{0}\n'
+                '{3}    * </span>{0}\n'
+            ).format(
+                output_color_reset,
+                output_color_before,
+                output_color_error,
+                output_color_after,
+            ),
+            str(err.exception),
+        )
+
+        # Test missing before.
+        with self.assertRaises(AssertionError) as err:
+            self.assertPageContent(
+                response,
+                [
+                    'testing',
+                    'span',
+                    '.',
+                    '</span>',
+                ]
+            )
+        self.assertText(
+            (
+                'Could not find expected content value in response. Provided value was:\n'
+                'testing\n'
+                '\n'
+                '\n'
+                'Surrounding Checks:\n'
+                '{2}Failed Check:{0}\n'
+                '{2}  > * testing{0}\n'
+                '{3}Content Checks After:{0}\n'
+                '{3}    * span{0}\n'
+                '{3}    * .{0}\n'
+                '{3}    * </span>{0}\n'
+            ).format(
+                output_color_reset,
+                output_color_before,
+                output_color_error,
+                output_color_after,
+            ),
+            str(err.exception),
+        )
+
+        # Test missing after.
+        with self.assertRaises(AssertionError) as err:
+            self.assertPageContent(
+                response,
+                [
+                    '<span>',
+                    'This',
+                    'is',
+                    'my',
+                    'testing',
+                ]
+            )
+        self.assertText(
+            (
+                'Could not find expected content value in response. Provided value was:\n'
+                'testing\n'
+                '\n'
+                '\n'
+                'Surrounding Checks:\n'
+                '{1}Content Checks Before:{0}\n'
+                '{1}    * This{0}\n'
+                '{1}    * is{0}\n'
+                '{1}    * my{0}\n'
+                '{2}Failed Check:{0}\n'
+                '{2}  > * testing{0}\n'
+            ).format(
+                output_color_reset,
+                output_color_before,
+                output_color_error,
+                output_color_after,
+            ),
+            str(err.exception),
+        )
+
+        # Test only one per side.
+        with self.assertRaises(AssertionError) as err:
+            self.assertPageContent(
+                response,
+                [
+                    'my',
+                    'testing',
+                    'span',
+                ]
+            )
+        self.assertText(
+            (
+                'Could not find expected content value in response. Provided value was:\n'
+                'testing\n'
+                '\n'
+                '\n'
+                'Surrounding Checks:\n'
+                '{1}Content Checks Before:{0}\n'
+                '{1}    * my{0}\n'
+                '{2}Failed Check:{0}\n'
+                '{2}  > * testing{0}\n'
+                '{3}Content Checks After:{0}\n'
+                '{3}    * span{0}\n'
+            ).format(
+                output_color_reset,
+                output_color_before,
+                output_color_error,
+                output_color_after,
+            ),
+            str(err.exception),
+        )
+
+        # Test missing all.
+        with self.assertRaises(AssertionError) as err:
+            self.assertPageContent(
+                response,
+                [
+                    'testing',
+                ]
+            )
+        self.assertText(
+            (
+                'Could not find expected content value in response. Provided value was:\n'
+                'testing\n'
+            ),
+            str(err.exception),
+        )
+
     def test__assertNotPageContent__success(self):
         """
         Tests assertNotPageContent() function, in cases when it should succeed.
         """
 
         with self.subTest('Empty response, no value passed.'):
             # Technically this one "matches".
@@ -3190,15 +5169,18 @@
         with self.subTest('Standard Response, no value passed'):
             # Same as above, or any other case with empty-strings.
             response = self._get_page_response('django_expanded_test_cases:login')
             self.assertNotPageContent(response, '')
 
         with self.subTest('Standard Response - Wrong value passed'):
             response = self._get_page_response('django_expanded_test_cases:login')
-            self.assertNotPageContent(response, '<h1>Testing Header</h1><p>Pretend this is a page.</p>')
+            self.assertNotPageContent(
+                response,
+                '<h1>Testing Header</h1><p>Pretend this is a page.</p>',
+            )
 
         with self.subTest('Standard Response - Set of items with wrong values'):
             response = self._get_page_response('django_expanded_test_cases:index')
 
             # Test as list.
             # First verify value we know SHOULD be there.
             self.assertPageContent(response, ['<h1>Home Page Header</h1>'])
@@ -3219,35 +5201,41 @@
             # Ensure other content is consistently NOT found.
             self.assertNotPageContent(response, ['Wrong Content'])
             self.assertNotPageContent(response, ['<h1>Home Page Wrong'])
             self.assertNotPageContent(response, ['Wrong Page Header</h1>'])
 
             # Ensure multiple values are also all not found.
             # Above values, but all in a single list. All should fail to be found.
-            self.assertNotPageContent(response, [
-                '<h1>HomePage Header</h1>',
-                '<h1>Home PageHeader</h1>',
-                '<h1>HomePageHeader</h1>',
-                '<h1>Home Pge Header</h1>',
-                'HomePage Header',
-                'Home PageHeader',
-                'HomePageHeader',
-                'Home Pge Header',
-                'Home PageHeader</h1>',
-                '<h1>HomePage Header',
-                '<h2>Home Page Header</h2>',
-            ])
+            self.assertNotPageContent(
+                response,
+                [
+                    '<h1>HomePage Header</h1>',
+                    '<h1>Home PageHeader</h1>',
+                    '<h1>HomePageHeader</h1>',
+                    '<h1>Home Pge Header</h1>',
+                    'HomePage Header',
+                    'Home PageHeader',
+                    'HomePageHeader',
+                    'Home Pge Header',
+                    'Home PageHeader</h1>',
+                    '<h1>HomePage Header',
+                    '<h2>Home Page Header</h2>',
+                ],
+            )
             # Multiple values that should not be present.
-            self.assertNotPageContent(response, [
-                'Wrong Content',
-                'Wrong text',
-                '<h1>Home Page Wrong',
-                '<h1>Wrong Header</h1>',
-                'Wrong Page Header</h1>',
-            ])
+            self.assertNotPageContent(
+                response,
+                [
+                    'Wrong Content',
+                    'Wrong text',
+                    '<h1>Home Page Wrong',
+                    '<h1>Wrong Header</h1>',
+                    'Wrong Page Header</h1>',
+                ],
+            )
 
             # Test as tuple.
             # First verify value we know SHOULD be there.
             self.assertPageContent(response, ('<h1>Home Page Header</h1>',))
 
             # Now ensure we FAIL to find variations of it.
             self.assertNotPageContent(response, ('<h1>HomePage Header</h1>',))
@@ -3265,35 +5253,41 @@
             # Ensure other content is consistently NOT found.
             self.assertNotPageContent(response, ('Wrong Content',))
             self.assertNotPageContent(response, ('<h1>Home Page Wrong',))
             self.assertNotPageContent(response, ('Wrong Page Header</h1>',))
 
             # Ensure multiple values are also all not found.
             # Above values, but all in a single list. All should fail to be found.
-            self.assertNotPageContent(response, (
-                '<h1>HomePage Header</h1>',
-                '<h1>Home PageHeader</h1>',
-                '<h1>HomePageHeader</h1>',
-                '<h1>Home Pge Header</h1>',
-                'HomePage Header',
-                'Home PageHeader',
-                'HomePageHeader',
-                'Home Pge Header',
-                'Home PageHeader</h1>',
-                '<h1>HomePage Header',
-                '<h2>Home Page Header</h2>',
-            ))
+            self.assertNotPageContent(
+                response,
+                (
+                    '<h1>HomePage Header</h1>',
+                    '<h1>Home PageHeader</h1>',
+                    '<h1>HomePageHeader</h1>',
+                    '<h1>Home Pge Header</h1>',
+                    'HomePage Header',
+                    'Home PageHeader',
+                    'HomePageHeader',
+                    'Home Pge Header',
+                    'Home PageHeader</h1>',
+                    '<h1>HomePage Header',
+                    '<h2>Home Page Header</h2>',
+                ),
+            )
             # Multiple values that should not be present.
-            self.assertNotPageContent(response, (
-                'Wrong Content',
-                'Wrong text',
-                '<h1>Home Page Wrong',
-                '<h1>Wrong Header</h1>',
-                'Wrong Page Header</h1>',
-            ))
+            self.assertNotPageContent(
+                response,
+                (
+                    'Wrong Content',
+                    'Wrong text',
+                    '<h1>Home Page Wrong',
+                    '<h1>Wrong Header</h1>',
+                    'Wrong Page Header</h1>',
+                ),
+            )
 
     def test__assertNotPageContent__failure(self):
         """
         Tests assertNotPageContent() function, in cases when it should fail.
         """
         err_msg = 'Found content in response. Expected content to not be present. Content was:\n{0}'
 
@@ -3399,76 +5393,94 @@
         )
 
         with self.subTest('Standard Response - Set of items where one or more items is found (none should be found)'):
             response = self._get_page_response('django_expanded_test_cases:index')
 
             # First item is found.
             with self.assertRaises(AssertionError) as err:
-                self.assertNotPageContent(response, (
-                    '<h1>Home Page Header</h1>',
-                    'Wrong Content',
-                    'Wrong text',
-                    '<h1>Home Page Wrong',
-                    '<h1>Wrong Header</h1>',
-                    'Wrong Page Header</h1>',
-                ))
+                self.assertNotPageContent(
+                    response,
+                    (
+                        '<h1>Home Page Header</h1>',
+                        'Wrong Content',
+                        'Wrong text',
+                        '<h1>Home Page Wrong',
+                        '<h1>Wrong Header</h1>',
+                        'Wrong Page Header</h1>',
+                    ),
+                )
             self.assertText(err_msg.format('<h1>Home Page Header</h1>'), str(err.exception))
             with self.assertRaises(AssertionError) as err:
-                self.assertNotPageContent(response, (
-                    'Home Page Header',
-                    'Wrong Content',
-                    'Wrong text',
-                    '<h1>Home Page Wrong',
-                    '<h1>Wrong Header</h1>',
-                    'Wrong Page Header</h1>',
-                ))
+                self.assertNotPageContent(
+                    response,
+                    (
+                        'Home Page Header',
+                        'Wrong Content',
+                        'Wrong text',
+                        '<h1>Home Page Wrong',
+                        '<h1>Wrong Header</h1>',
+                        'Wrong Page Header</h1>',
+                    ),
+                )
             self.assertText(err_msg.format('Home Page Header'), str(err.exception))
 
             # Middle item is found.
             with self.assertRaises(AssertionError) as err:
-                self.assertNotPageContent(response, (
-                    'Wrong Content',
-                    'Wrong text',
-                    '<h1>Home Page Header</h1>',
-                    '<h1>Home Page Wrong',
-                    '<h1>Wrong Header</h1>',
-                    'Wrong Page Header</h1>',
-                ))
+                self.assertNotPageContent(
+                    response,
+                    (
+                        'Wrong Content',
+                        'Wrong text',
+                        '<h1>Home Page Header</h1>',
+                        '<h1>Home Page Wrong',
+                        '<h1>Wrong Header</h1>',
+                        'Wrong Page Header</h1>',
+                    ),
+                )
             self.assertText(err_msg.format('<h1>Home Page Header</h1>'), str(err.exception))
             with self.assertRaises(AssertionError) as err:
-                self.assertNotPageContent(response, (
-                    'Wrong Content',
-                    'Wrong text',
-                    'Home Page Header',
-                    '<h1>Home Page Wrong',
-                    '<h1>Wrong Header</h1>',
-                    'Wrong Page Header</h1>',
-                ))
+                self.assertNotPageContent(
+                    response,
+                    (
+                        'Wrong Content',
+                        'Wrong text',
+                        'Home Page Header',
+                        '<h1>Home Page Wrong',
+                        '<h1>Wrong Header</h1>',
+                        'Wrong Page Header</h1>',
+                    ),
+                )
             self.assertText(err_msg.format('Home Page Header'), str(err.exception))
 
             # Last item is found.
             with self.assertRaises(AssertionError) as err:
-                self.assertNotPageContent(response, (
-                    'Wrong Content',
-                    'Wrong text',
-                    '<h1>Home Page Wrong',
-                    '<h1>Wrong Header</h1>',
-                    'Wrong Page Header</h1>',
-                    '<h1>Home Page Header</h1>',
-                ))
+                self.assertNotPageContent(
+                    response,
+                    (
+                        'Wrong Content',
+                        'Wrong text',
+                        '<h1>Home Page Wrong',
+                        '<h1>Wrong Header</h1>',
+                        'Wrong Page Header</h1>',
+                        '<h1>Home Page Header</h1>',
+                    ),
+                )
             self.assertText(err_msg.format('<h1>Home Page Header</h1>'), str(err.exception))
             with self.assertRaises(AssertionError) as err:
-                self.assertNotPageContent(response, (
-                    'Wrong Content',
-                    'Wrong text',
-                    '<h1>Home Page Wrong',
-                    '<h1>Wrong Header</h1>',
-                    'Wrong Page Header</h1>',
-                    'Home Page Header',
-                ))
+                self.assertNotPageContent(
+                    response,
+                    (
+                        'Wrong Content',
+                        'Wrong text',
+                        '<h1>Home Page Wrong',
+                        '<h1>Wrong Header</h1>',
+                        'Wrong Page Header</h1>',
+                        'Home Page Header',
+                    ),
+                )
             self.assertText(err_msg.format('Home Page Header'), str(err.exception))
 
     def test__assertRepeatingElement__success__standard_elements__basic(self):
         """
         Tests assertPageContent() function, in cases when it should succeed on "standard" (non-void) elements.
         """
         with self.subTest('Response with one item, when one item is expected'):
@@ -4135,27 +6147,39 @@
             response = HttpResponse('<title>   Test    Title   </title>')
             self.assertText('Test Title', self.get_page_title(response))
             self.assertText('Test Title', self.get_page_title(response.content))
             self.assertText('Test Title', self.get_page_title(response.content.decode('utf-8')))
 
         with self.subTest('Complex title'):
             response = HttpResponse('<title>Test Title | My Custom App | My Really Cool Site</title>')
-            self.assertText('Test Title | My Custom App | My Really Cool Site', self.get_page_title(response))
-            self.assertText('Test Title | My Custom App | My Really Cool Site', self.get_page_title(response.content))
+            self.assertText(
+                'Test Title | My Custom App | My Really Cool Site',
+                self.get_page_title(response),
+            )
+            self.assertText(
+                'Test Title | My Custom App | My Really Cool Site',
+                self.get_page_title(response.content),
+            )
             self.assertText(
                 'Test Title | My Custom App | My Really Cool Site',
                 self.get_page_title(response.content.decode('utf-8')),
             )
 
         with self.subTest('Complex title, with extra whitespace (to simulate Django templating)'):
             response = HttpResponse(
                 '<title>   Test   Title    \n|\n   My Custom App   \n|\n   My Really Cool Site   </title>'
             )
-            self.assertText('Test Title | My Custom App | My Really Cool Site', self.get_page_title(response))
-            self.assertText('Test Title | My Custom App | My Really Cool Site', self.get_page_title(response.content))
+            self.assertText(
+                'Test Title | My Custom App | My Really Cool Site',
+                self.get_page_title(response),
+            )
+            self.assertText(
+                'Test Title | My Custom App | My Really Cool Site',
+                self.get_page_title(response.content),
+            )
             self.assertText(
                 'Test Title | My Custom App | My Really Cool Site',
                 self.get_page_title(response.content.decode('utf-8')),
             )
 
     def test__get_page_header__empty_header(self):
         """
@@ -4397,91 +6421,145 @@
     def test__standardize_url__success(self):
         """
         Tests standardize_url() function, in situations when it should succeed.
         """
 
         with self.subTest('Emtpy url'):
             # Base url.
-            url = self.standardize_url('', append_root=False)
+            url = self.standardize_url(
+                '',
+                append_root=False,
+            )
             self.assertText('/', url)
 
             # With site root.
-            url = self.standardize_url('', append_root=True)
+            url = self.standardize_url(
+                '',
+                append_root=True,
+            )
             self.assertText('127.0.0.1/', url)
 
         with self.subTest('Basic url - No outer slashes'):
             # Base url.
-            url = self.standardize_url('login', append_root=False)
+            url = self.standardize_url(
+                'login',
+                append_root=False,
+            )
             self.assertText('/login/', url)
 
             # With site root.
-            url = self.standardize_url('login', append_root=True)
+            url = self.standardize_url(
+                'login',
+                append_root=True,
+            )
             self.assertText('127.0.0.1/login/', url)
 
         with self.subTest('Basic url - With outer slashes'):
             # Base url.
-            url = self.standardize_url('/login/', append_root=False)
+            url = self.standardize_url(
+                '/login/',
+                append_root=False,
+            )
             self.assertText('/login/', url)
 
             # With site root.
-            url = self.standardize_url('/login/', append_root=True)
+            url = self.standardize_url(
+                '/login/',
+                append_root=True,
+            )
             self.assertText('127.0.0.1/login/', url)
 
         with self.subTest('Longer url - No outer slashes'):
             # Base url.
-            url = self.standardize_url('this/is/a/test/url', append_root=False)
+            url = self.standardize_url(
+                'this/is/a/test/url',
+                append_root=False,
+            )
             self.assertText('/this/is/a/test/url/', url)
 
             # With site root.
-            url = self.standardize_url('/this/is/a/test/url/', append_root=True)
+            url = self.standardize_url(
+                '/this/is/a/test/url/',
+                append_root=True,
+            )
             self.assertText('127.0.0.1/this/is/a/test/url/', url)
 
         with self.subTest('With GET args - Provided in url'):
             # Base url.
-            url = self.standardize_url('/my/url/?arg1=testing&arg2=aaa', append_root=False)
+            url = self.standardize_url(
+                '/my/url/?arg1=testing&arg2=aaa',
+                append_root=False,
+            )
             self.assertText('/my/url/?arg1=testing&arg2=aaa', url)
 
             # With site root.
-            url = self.standardize_url('/my/url/?arg1=testing&arg2=aaa', append_root=True)
+            url = self.standardize_url(
+                '/my/url/?arg1=testing&arg2=aaa',
+                append_root=True,
+            )
             self.assertText('127.0.0.1/my/url/?arg1=testing&arg2=aaa', url)
 
         with self.subTest('With GET args - Provided via generate_get_url()'):
             # Base url.
-            url = self.standardize_url(self.generate_get_url('/my/url/', arg1='testing', arg2='aaa'), append_root=False)
+            url = self.standardize_url(
+                self.generate_get_url('/my/url/', arg1='testing', arg2='aaa'),
+                append_root=False,
+            )
             self.assertText('/my/url/?arg1=testing&arg2=aaa', url)
 
             # With site root.
-            url = self.standardize_url(self.generate_get_url('/my/url/', arg1='testing', arg2='aaa'), append_root=True)
+            url = self.standardize_url(
+                self.generate_get_url('/my/url/', arg1='testing', arg2='aaa'),
+                append_root=True,
+            )
             self.assertText('127.0.0.1/my/url/?arg1=testing&arg2=aaa', url)
 
         with self.subTest('With GET args - Provided in url with mixed characters'):
             # Base url.
-            url = self.standardize_url('/my/url/?arg1=testing stuff?<blah>weird_values-aaa', append_root=False)
+            url = self.standardize_url(
+                '/my/url/?arg1=testing stuff?<blah>weird_values-aaa',
+                append_root=False,
+            )
             self.assertText('/my/url/?arg1=testing+stuff%3F%3Cblah%3Eweird_values-aaa', url)
 
             # With site root.
-            url = self.standardize_url('/my/url/?arg1=testing stuff?<blah>weird_values-aaa', append_root=True)
+            url = self.standardize_url(
+                '/my/url/?arg1=testing stuff?<blah>weird_values-aaa',
+                append_root=True,
+            )
             self.assertText('127.0.0.1/my/url/?arg1=testing+stuff%3F%3Cblah%3Eweird_values-aaa', url)
 
         with self.subTest('With GET args - Provided in generate_get_url() with mixed characters'):
             # Base url.
-            url = self.standardize_url(self.generate_get_url('/my/url/?', test='testing stuff?<blah>weird_values-aaa'), append_root=False)
+            url = self.standardize_url(
+                self.generate_get_url('/my/url/?', test='testing stuff?<blah>weird_values-aaa'),
+                append_root=False,
+            )
             self.assertText('/my/url/?test=testing+stuff%3F%3Cblah%3Eweird_values-aaa', url)
 
             # With site root.
-            url = self.standardize_url(self.generate_get_url('/my/url/?', test='testing stuff?<blah>weird_values-aaa'), append_root=True)
+            url = self.standardize_url(
+                self.generate_get_url('/my/url/?', test='testing stuff?<blah>weird_values-aaa'),
+                append_root=True,
+            )
             self.assertText('127.0.0.1/my/url/?test=testing+stuff%3F%3Cblah%3Eweird_values-aaa', url)
 
         with self.subTest('Basic resolve url'):
             # Base url.
-            url = self.standardize_url('django_expanded_test_cases:login', append_root=False)
+            url = self.standardize_url(
+                'django_expanded_test_cases:login',
+                append_root=False,
+            )
             self.assertText('/login/', url)
 
             # With site root.
-            url = self.standardize_url('django_expanded_test_cases:login', append_root=True)
+            url = self.standardize_url(
+                'django_expanded_test_cases:login',
+                append_root=True,
+            )
             self.assertText('127.0.0.1/login/', url)
 
         with self.subTest('Resolve url with params as args'):
             # Base url.
             url = self.standardize_url(
                 'django_expanded_test_cases:response-with-args',
                 url_args=(11, 'args_test_1'),
@@ -5472,18 +7550,15 @@
 
             with self.assertRaises(AssertionError) as err:
                 self.find_elements_by_css_selector(response, 'li .test_class > a')
             self.assertText(err_msg, str(err.exception))
 
             # Missing two parts.
             response = HttpResponse('<li></li>')
-            err_msg = (
-                'Unable to find css selector "li .test_class > a" in content. '
-                'Provided content was:\n<li></li>'
-            )
+            err_msg = 'Unable to find css selector "li .test_class > a" in content. Provided content was:\n<li></li>'
 
             with self.assertRaises(AssertionError) as err:
                 self.find_elements_by_css_selector(response, 'li .test_class > a')
             self.assertText(err_msg, str(err.exception))
 
             # Missing one part.
             response = HttpResponse('<li><p class="test_class"></p></li>')
@@ -6557,28 +8632,30 @@
             # Verify full results when not limiting by element type.
             results = self.find_elements_by_text(response, 'test_element_text')
             self.assertEqual(len(results), 4)
 
             # Verify non-results when limiting by each non-present type.
             # Type h3.
             err_msg = (
-                'Unable to find element text "test_element_text" in content under element type of "h3". Provided content was:\n'
+                'Unable to find element text "test_element_text" in content under element type of "h3". '
+                'Provided content was:\n'
                 '<div>\n'
                 '<h1>test_element_text</h1>\n'
                 '<h2>test_element_text</h2>\n'
                 '<p>test_element_text</p>\n'
                 '<li>test_element_text</li>\n'
                 '</div>\n'
             )
             with self.assertRaises(AssertionError) as err:
                 self.find_elements_by_text(response, 'test_element_text', element_type='h3')
             self.assertText(err_msg, str(err.exception))
             # Type span.
             err_msg = (
-                'Unable to find element text "test_element_text" in content under element type of "span". Provided content was:\n'
+                'Unable to find element text "test_element_text" in content under element type of "span". '
+                'Provided content was:\n'
                 '<div>\n'
                 '<h1>test_element_text</h1>\n'
                 '<h2>test_element_text</h2>\n'
                 '<p>test_element_text</p>\n'
                 '<li>test_element_text</li>\n'
                 '</div>\n'
             )
@@ -6660,15 +8737,16 @@
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_text(response, 'test_element_text')
             self.assertText(err_msg, str(err.exception))
 
         with self.subTest('When expected element_text is present multiple times'):
             response = HttpResponse('<a href="">test_element_text</a><a href="">test_element_text</a>')
             err_msg = (
-                'Found multiple instances of "test_element_text" element text. Expected only one instance. Content was:\n'
+                'Found multiple instances of "test_element_text" element text. Expected only one instance. '
+                'Content was:\n'
                 '<a href="">test_element_text</a><a href="">test_element_text</a>'
             )
 
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_text(response, 'test_element_text')
             self.assertText(err_msg, str(err.exception))
 
@@ -6852,64 +8930,84 @@
             # Various checks, of different ways to ensure expected user is logged in.
             self.assertEqual(new_user.pk, int(self.client.session['_auth_user_id']))
             self.assertEqual(new_user, response.wsgi_request.user)
             self.assertEqual(new_user, response.context['user'])
             self.assertEqual(new_user, response.user)
 
         with self.subTest(
-            'Check login using super user - Provided with conflicting values (function value should win)'):
+            'Check login using super user - Provided with conflicting values (function value should win)'
+        ):
             self.user = self.get_user('new_user')
-            response = self.assertGetResponse('django_expanded_test_cases:index', user='test_superuser')
+            response = self.assertGetResponse(
+                'django_expanded_test_cases:index',
+                user='test_superuser',
+            )
 
             # Various checks, of different ways to ensure expected user is logged in.
             self.assertEqual(self.test_superuser.pk, int(self.client.session['_auth_user_id']))
             self.assertEqual(self.test_superuser, response.wsgi_request.user)
             self.assertEqual(self.test_superuser, response.context['user'])
             self.assertEqual(self.test_superuser, response.user)
 
         with self.subTest(
-            'Check login using admin user - Provided with conflicting values (function value should win)'):
+            'Check login using admin user - Provided with conflicting values (function value should win)'
+        ):
             self.user = self.get_user('test_superuser')
-            response = self.assertGetResponse('django_expanded_test_cases:index', user='test_admin')
+            response = self.assertGetResponse(
+                'django_expanded_test_cases:index',
+                user='test_admin',
+            )
 
             # Various checks, of different ways to ensure expected user is logged in.
             self.assertEqual(self.test_admin.pk, int(self.client.session['_auth_user_id']))
             self.assertEqual(self.test_admin, response.wsgi_request.user)
             self.assertEqual(self.test_admin, response.context['user'])
             self.assertEqual(self.test_admin, response.user)
 
         with self.subTest(
-            'Check login using inactive user - Provided with conflicting values (function value should win)'):
+            'Check login using inactive user - Provided with conflicting values (function value should win)'
+        ):
             self.user = self.get_user('test_admin')
-            response = self.assertGetResponse('django_expanded_test_cases:index', user='test_inactive')
+            response = self.assertGetResponse(
+                'django_expanded_test_cases:index',
+                user='test_inactive',
+            )
 
             # Various checks, of different ways to ensure expected user is logged in.
             with self.assertRaises(KeyError):
                 self.client.session['_auth_user_id']
             self.assertTrue(isinstance(response.wsgi_request.user, AnonymousUser))
             self.assertFalse(isinstance(response.wsgi_request.user, get_user_model()))
             self.assertNotEqual(self.test_inactive_user, response.wsgi_request.user)
             self.assertTrue(isinstance(response.user, AnonymousUser))
             self.assertFalse(isinstance(response.user, get_user_model()))
 
         with self.subTest(
-            'Check login using standard user - Provided with conflicting values (function value should win)'):
+            'Check login using standard user - Provided with conflicting values (function value should win)'
+        ):
             self.user = self.get_user('test_inactive')
-            response = self.assertGetResponse('django_expanded_test_cases:index', user='test_user')
+            response = self.assertGetResponse(
+                'django_expanded_test_cases:index',
+                user='test_user',
+            )
 
             # Various checks, of different ways to ensure expected user is logged in.
             self.assertEqual(self.test_user.pk, int(self.client.session['_auth_user_id']))
             self.assertEqual(self.test_user, response.wsgi_request.user)
             self.assertEqual(self.test_user, response.context['user'])
             self.assertEqual(self.test_user, response.user)
 
         with self.subTest(
-            'Check login using custom new user - Provided with conflicting values (function value should win)'):
+            'Check login using custom new user - Provided with conflicting values (function value should win)'
+        ):
             self.user = self.get_user('test_user')
-            response = self.assertGetResponse('django_expanded_test_cases:index', user='new_user')
+            response = self.assertGetResponse(
+                'django_expanded_test_cases:index',
+                user='new_user',
+            )
 
             # Various checks, of different ways to ensure expected user is logged in.
             self.assertEqual(new_user.pk, int(self.client.session['_auth_user_id']))
             self.assertEqual(new_user, response.wsgi_request.user)
             self.assertEqual(new_user, response.context['user'])
             self.assertEqual(new_user, response.user)
 
@@ -7107,58 +9205,68 @@
 
             # Various checks, of different ways to ensure expected user is logged in.
             self.assertEqual(new_user.pk, int(self.client.session['_auth_user_id']))
             self.assertEqual(new_user, response.wsgi_request.user)
             self.assertEqual(new_user, response.context['user'])
             self.assertEqual(new_user, response.user)
 
-        with self.subTest('Check login using super user - Provided with conflicting values (function value should win)'):
+        with self.subTest(
+            'Check login using super user - Provided with conflicting values (function value should win)'
+        ):
             self.user = self.get_user('new_user')
             response = self.assertGetResponse('django_expanded_test_cases:index', user='test_superuser')
 
             # Various checks, of different ways to ensure expected user is logged in.
             self.assertEqual(self.test_superuser.pk, int(self.client.session['_auth_user_id']))
             self.assertEqual(self.test_superuser, response.wsgi_request.user)
             self.assertEqual(self.test_superuser, response.context['user'])
             self.assertEqual(self.test_superuser, response.user)
 
-        with self.subTest('Check login using admin user - Provided with conflicting values (function value should win)'):
+        with self.subTest(
+            'Check login using admin user - Provided with conflicting values (function value should win)'
+        ):
             self.user = self.get_user('test_superuser')
             response = self.assertGetResponse('django_expanded_test_cases:index', user='test_admin')
 
             # Various checks, of different ways to ensure expected user is logged in.
             self.assertEqual(self.test_admin.pk, int(self.client.session['_auth_user_id']))
             self.assertEqual(self.test_admin, response.wsgi_request.user)
             self.assertEqual(self.test_admin, response.context['user'])
             self.assertEqual(self.test_admin, response.user)
 
-        with self.subTest('Check login using inactive user - Provided with conflicting values (function value should win)'):
+        with self.subTest(
+            'Check login using inactive user - Provided with conflicting values (function value should win)'
+        ):
             self.user = self.get_user('test_admin')
             response = self.assertGetResponse('django_expanded_test_cases:index', user='test_inactive')
 
             # Various checks, of different ways to ensure expected user is logged in.
             with self.assertRaises(KeyError):
                 self.client.session['_auth_user_id']
             self.assertTrue(isinstance(response.wsgi_request.user, AnonymousUser))
             self.assertFalse(isinstance(response.wsgi_request.user, get_user_model()))
             self.assertNotEqual(self.test_inactive_user, response.wsgi_request.user)
             self.assertTrue(isinstance(response.user, AnonymousUser))
             self.assertFalse(isinstance(response.user, get_user_model()))
 
-        with self.subTest('Check login using standard user - Provided with conflicting values (function value should win)'):
+        with self.subTest(
+            'Check login using standard user - Provided with conflicting values (function value should win)'
+        ):
             self.user = self.get_user('test_inactive')
             response = self.assertGetResponse('django_expanded_test_cases:index', user='test_user')
 
             # Various checks, of different ways to ensure expected user is logged in.
             self.assertEqual(self.test_user.pk, int(self.client.session['_auth_user_id']))
             self.assertEqual(self.test_user, response.wsgi_request.user)
             self.assertEqual(self.test_user, response.context['user'])
             self.assertEqual(self.test_user, response.user)
 
-        with self.subTest('Check login using custom new user - Provided with conflicting values (function value should win)'):
+        with self.subTest(
+            'Check login using custom new user - Provided with conflicting values (function value should win)'
+        ):
             self.user = self.get_user('test_user')
             response = self.assertGetResponse('django_expanded_test_cases:index', user='new_user')
 
             # Various checks, of different ways to ensure expected user is logged in.
             self.assertEqual(new_user.pk, int(self.client.session['_auth_user_id']))
             self.assertEqual(new_user, response.wsgi_request.user)
             self.assertEqual(new_user, response.context['user'])
@@ -7347,58 +9455,68 @@
 
             # Various checks, of different ways to ensure expected user is logged in.
             self.assertEqual(new_user.pk, int(self.client.session['_auth_user_id']))
             self.assertEqual(new_user, response.wsgi_request.user)
             self.assertEqual(new_user, response.context['user'])
             self.assertEqual(new_user, response.user)
 
-        with self.subTest('Check login using super user - Provided with conflicting values (function value should win)'):
+        with self.subTest(
+            'Check login using super user - Provided with conflicting values (function value should win)'
+        ):
             self.user = self.get_user('new_user')
             response = self.assertGetResponse('django_expanded_test_cases:index', user='test_superuser')
 
             # Various checks, of different ways to ensure expected user is logged in.
             self.assertEqual(self.test_superuser.pk, int(self.client.session['_auth_user_id']))
             self.assertEqual(self.test_superuser, response.wsgi_request.user)
             self.assertEqual(self.test_superuser, response.context['user'])
             self.assertEqual(self.test_superuser, response.user)
 
-        with self.subTest('Check login using admin user - Provided with conflicting values (function value should win)'):
+        with self.subTest(
+            'Check login using admin user - Provided with conflicting values (function value should win)'
+        ):
             self.user = self.get_user('test_superuser')
             response = self.assertGetResponse('django_expanded_test_cases:index', user='test_admin')
 
             # Various checks, of different ways to ensure expected user is logged in.
             self.assertEqual(self.test_admin.pk, int(self.client.session['_auth_user_id']))
             self.assertEqual(self.test_admin, response.wsgi_request.user)
             self.assertEqual(self.test_admin, response.context['user'])
             self.assertEqual(self.test_admin, response.user)
 
-        with self.subTest('Check login using inactive user - Provided with conflicting values (function value should win)'):
+        with self.subTest(
+            'Check login using inactive user - Provided with conflicting values (function value should win)'
+        ):
             self.user = self.get_user('test_admin')
             response = self.assertGetResponse('django_expanded_test_cases:index', user='test_inactive')
 
             # Various checks, of different ways to ensure expected user is logged in.
             with self.assertRaises(KeyError):
                 self.client.session['_auth_user_id']
             self.assertTrue(isinstance(response.wsgi_request.user, AnonymousUser))
             self.assertFalse(isinstance(response.wsgi_request.user, get_user_model()))
             self.assertNotEqual(self.test_inactive_user, response.wsgi_request.user)
             self.assertTrue(isinstance(response.user, AnonymousUser))
             self.assertFalse(isinstance(response.user, get_user_model()))
 
-        with self.subTest('Check login using standard user - Provided with conflicting values (function value should win)'):
+        with self.subTest(
+            'Check login using standard user - Provided with conflicting values (function value should win)'
+        ):
             self.user = self.get_user('test_inactive')
             response = self.assertGetResponse('django_expanded_test_cases:index', user='test_user')
 
             # Various checks, of different ways to ensure expected user is logged in.
             self.assertEqual(self.test_user.pk, int(self.client.session['_auth_user_id']))
             self.assertEqual(self.test_user, response.wsgi_request.user)
             self.assertEqual(self.test_user, response.context['user'])
             self.assertEqual(self.test_user, response.user)
 
-        with self.subTest('Check login using custom new user - Provided with conflicting values (function value should win)'):
+        with self.subTest(
+            'Check login using custom new user - Provided with conflicting values (function value should win)'
+        ):
             self.user = self.get_user('test_user')
             response = self.assertGetResponse('django_expanded_test_cases:index', user='new_user')
 
             # Various checks, of different ways to ensure expected user is logged in.
             self.assertEqual(new_user.pk, int(self.client.session['_auth_user_id']))
             self.assertEqual(new_user, response.wsgi_request.user)
             self.assertEqual(new_user, response.context['user'])
```

### Comparing `django-expanded-test-cases-0.7.0/etc_tests/test_cases/test_live_server_case.py` & `django_expanded_test_cases-0.7.1/etc_tests/test_cases/test_live_server_case.py`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.7.0/etc_tests/test_cases/universal_live_test_mixin.py` & `django_expanded_test_cases-0.7.1/etc_tests/test_cases/universal_live_test_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1014,15 +1014,15 @@
                 '</div>\n'
                 '</body></html>'
             )
 
             # Open file and write expected page contents.
             with open(file_name, 'w') as file:
                 file.write(
-                """
+                    """
                 <div>
                     <h1>Page Header</h1>
                     <p id="some_value">Some text.</p>
                     <p id="another_id">Some more text.</p>
                     <p>Some text with the str "id" in it.</p>
                 </div>
                 """
@@ -1958,15 +1958,14 @@
                     """
                 )
 
             # Get driver object to open generated file.
             driver = self.get_driver()
             driver.get('file://{0}'.format(file_name))
 
-
             results = self.find_elements_by_data_attribute(driver, 'my_attr', 'my_val')
             self.assertEqual(len(results), 3)
             self.assertIn('<li my_attr="my_val">\n<p>\n One\n</p>\n</li>', results)
             self.assertIn('<li my_attr="my_val">\n<p>\n Two\n</p>\n</li>', results)
             self.assertIn('<li my_attr="my_val" test_attr="test_val">\n<p>\n Four\n</p>\n</li>', results)
 
             # As <p> tag.
@@ -1989,15 +1988,14 @@
                     """
                 )
 
             # Get driver object to open generated file.
             driver = self.get_driver()
             driver.get('file://{0}'.format(file_name))
 
-
             results = self.find_elements_by_data_attribute(driver, 'my_attr', 'my_val')
             self.assertEqual(len(results), 3)
             self.assertIn('<p my_attr="my_val">\n One\n</p>', results)
             self.assertIn('<p my_attr="my_val">\n Two\n</p>', results)
             self.assertIn('<p my_attr="my_val" test_attr="test_val">\n Four\n</p>', results)
 
     def test__find_elements_by_data_attribute__failure(self):
```

### Comparing `django-expanded-test-cases-0.7.0/etc_tests/views.py` & `django_expanded_test_cases-0.7.1/etc_tests/views.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,187 +10,219 @@
 from django.template.response import TemplateResponse
 
 
 def index(request):
     """Page that simulates a site index/home."""
 
     # Render response.
-    return render(request, 'django_expanded_test_cases/index.html', {
-        'header': 'Home Page',
-        'text': 'Pretend this is the project landing page.',
-    })
+    return render(
+        request,
+        'django_expanded_test_cases/index.html',
+        {
+            'header': 'Home Page',
+            'text': 'Pretend this is the project landing page.',
+        },
+    )
 
 
 def template_response_index(request):
     """Page that simulates a site index/home. Specifically served as TemplateResponse."""
 
     # Render response.
-    return TemplateResponse(request, 'django_expanded_test_cases/index.html', {
-        'header': 'Home Page',
-        'text': 'Pretend this is the project landing page.',
-    })
+    return TemplateResponse(
+        request,
+        'django_expanded_test_cases/index.html',
+        {
+            'header': 'Home Page',
+            'text': 'Pretend this is the project landing page.',
+        },
+    )
 
 
 def login(request):
     """Page that simulates a login page."""
 
     # Render response.
-    return render(request, 'django_expanded_test_cases/index.html', {
-        'header': 'Login Page',
-        'text': 'Pretend this is a login page.',
-    })
+    return render(
+        request,
+        'django_expanded_test_cases/index.html',
+        {
+            'header': 'Login Page',
+            'text': 'Pretend this is a login page.',
+        },
+    )
 
 
 def view_with_one_message(request):
     """Page that simulates a view with a single message."""
 
     # Generate response messages.
     messages.info(request, 'This is a test message.')
 
     # Render response.
-    return render(request, 'django_expanded_test_cases/index.html', {
-        'header': 'View with One Message',
-        'text': (
-            'Pretend useful stuff is displayed here, for one-message render() view.'
-        )
-    })
+    return render(
+        request,
+        'django_expanded_test_cases/index.html',
+        {
+            'header': 'View with One Message',
+            'text': ('Pretend useful stuff is displayed here, for one-message render() view.'),
+        },
+    )
 
 
 def view_with_two_messages(request):
     """Page that simulates a view with two messages."""
 
     # Generate response messages.
     messages.info(request, 'Test message #1.')
     messages.warning(request, 'Test message #2.')
 
     # Render response.
-    return render(request, 'django_expanded_test_cases/index.html', {
-        'header': 'View with Two Messages',
-        'text': (
-            'Pretend useful stuff is displayed here, for two-message render() view.'
-        )
-    })
+    return render(
+        request,
+        'django_expanded_test_cases/index.html',
+        {
+            'header': 'View with Two Messages',
+            'text': ('Pretend useful stuff is displayed here, for two-message render() view.'),
+        },
+    )
 
 
 def view_with_three_messages(request):
     """Page that simulates a view with three messages."""
 
     # Generate response messages.
     messages.info(request, 'Test info message.')
     messages.warning(request, 'Test warning message.')
     messages.error(request, 'Test error message.')
 
     # Render response.
-    return render(request, 'django_expanded_test_cases/index.html', {
-        'header': 'View with Three Messages',
-        'text': (
-            'Pretend useful stuff is displayed here, for three-message render() view.'
-        )
-    })
+    return render(
+        request,
+        'django_expanded_test_cases/index.html',
+        {
+            'header': 'View with Three Messages',
+            'text': ('Pretend useful stuff is displayed here, for three-message render() view.'),
+        },
+    )
 
 
 def view_with_repeating_elements(request):
     """Page that simulates a view with multiple repeating elements."""
 
     # Render response.
-    return render(request, 'django_expanded_test_cases/index.html', {
-        'header': 'View with Repeating Elements',
-        'text': (
-            'Pretend useful stuff is displayed here, for render() view with url args.'
-        ),
-        'li_set': (
-            '<p>Repeating Line</p>',
-            '<p>Test First Unique Line</p>',
-            '<p>Repeating Line</p>',
-            '<p>Test Second Unique Line</p>',
-            '<p>Repeating Line</p>',
-            '<p>Test Third Unique Line</p>',
-            '<p>Repeating Line</p>',
-        ),
-    })
+    return render(
+        request,
+        'django_expanded_test_cases/index.html',
+        {
+            'header': 'View with Repeating Elements',
+            'text': ('Pretend useful stuff is displayed here, for render() view with url args.'),
+            'li_set': (
+                '<p>Repeating Line</p>',
+                '<p>Test First Unique Line</p>',
+                '<p>Repeating Line</p>',
+                '<p>Test Second Unique Line</p>',
+                '<p>Repeating Line</p>',
+                '<p>Test Third Unique Line</p>',
+                '<p>Repeating Line</p>',
+            ),
+        },
+    )
 
 
 def view_with_args(request, id, name):
     """Page that simulates a view with passed args."""
 
     # Render response.
-    return render(request, 'django_expanded_test_cases/index.html', {
-        'header': 'View with Args',
-        'text': (
-            'Pretend useful stuff is displayed here, for render() view with url args.'
-        ),
-        'li_set': (
-            'id: "{0}"'.format(id),
-            'name: "{0}"'.format(name),
-        ),
-    })
+    return render(
+        request,
+        'django_expanded_test_cases/index.html',
+        {
+            'header': 'View with Args',
+            'text': ('Pretend useful stuff is displayed here, for render() view with url args.'),
+            'li_set': (
+                'id: "{0}"'.format(id),
+                'name: "{0}"'.format(name),
+            ),
+        },
+    )
 
 
 def template_response_with_three_messages(request):
     """Page that simulates a view with three messages. Specifically served as TemplateResponse."""
 
     # Generate response messages.
     messages.info(request, 'Test info message.')
     messages.warning(request, 'Test warning message.')
     messages.error(request, 'Test error message.')
 
     # Render response.
-    return TemplateResponse(request, 'django_expanded_test_cases/index.html', {
-        'header': 'TemplateResponse View with Three Messages',
-        'text': (
-            'Pretend useful stuff is displayed here, for three-message TemplateResponse view.'
-        )
-    })
+    return TemplateResponse(
+        request,
+        'django_expanded_test_cases/index.html',
+        {
+            'header': 'TemplateResponse View with Three Messages',
+            'text': ('Pretend useful stuff is displayed here, for three-message TemplateResponse view.'),
+        },
+    )
 
 
 def template_response_with_args(request, id, name):
     """Page that simulates a view with passed args. Specifically served as a TemplateResponse."""
 
     # Render response.
-    return TemplateResponse(request, 'django_expanded_test_cases/index.html', {
-        'header': 'TemplateResponse View with Args',
-        'text': (
-            'Pretend useful stuff is displayed here, for TemplateResponse view with url args.'
-        ),
-        'li_set': (
-            'id: "{0}"'.format(id),
-            'name: "{0}"'.format(name),
-        ),
-    })
+    return TemplateResponse(
+        request,
+        'django_expanded_test_cases/index.html',
+        {
+            'header': 'TemplateResponse View with Args',
+            'text': ('Pretend useful stuff is displayed here, for TemplateResponse view with url args.'),
+            'li_set': (
+                'id: "{0}"'.format(id),
+                'name: "{0}"'.format(name),
+            ),
+        },
+    )
 
 
 def user_detail(request, pk):
     """Page that simulates a model detail page."""
 
     # Pull database info.
     user = get_object_or_404(get_user_model(), pk=pk)
 
     # Render response.
-    return render(request, 'django_expanded_test_cases/index.html', {
-        'header': 'User Detail Page',
-        'text': '{0}'.format(user),
-        'li_set': (
-            'Username: "{0}"'.format(user.username),
-            'First Name: "{0}"'.format(user.first_name),
-            'Last Name: "{0}"'.format(user.last_name),
-            'Is Active: "{0}"'.format(user.is_active),
-            'Is SuperUser: "{0}"'.format(user.is_superuser),
-            'Is Staff: "{0}"'.format(user.is_staff),
-        )
-    })
+    return render(
+        request,
+        'django_expanded_test_cases/index.html',
+        {
+            'header': 'User Detail Page',
+            'text': '{0}'.format(user),
+            'li_set': (
+                'Username: "{0}"'.format(user.username),
+                'First Name: "{0}"'.format(user.first_name),
+                'Last Name: "{0}"'.format(user.last_name),
+                'Is Active: "{0}"'.format(user.is_active),
+                'Is SuperUser: "{0}"'.format(user.is_superuser),
+                'Is Staff: "{0}"'.format(user.is_staff),
+            ),
+        },
+    )
 
 
 def redirect_to_index(request):
     """Page that simulates a redirect."""
 
     # Redirect to intended view.
     return redirect('django_expanded_test_cases:index')
 
 
 def redirect_with_args(request, id, name):
     """Page that simulates a redirect, with included url args."""
 
     # Redirect to intended view.
-    return redirect(reverse(
-        'django_expanded_test_cases:template-response-with-args',
-        args=(id, name),
-    ))
+    return redirect(
+        reverse(
+            'django_expanded_test_cases:template-response-with-args',
+            args=(id, name),
+        )
+    )
```

### Comparing `django-expanded-test-cases-0.7.0/pyproject.toml` & `django_expanded_test_cases-0.7.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=40.8.0', 'wheel']
 build-backend = 'setuptools.build_meta:__legacy__'
 
 [project]
 name = "django-expanded-test-cases"
-version = "0.7.0"
+version = "0.7.1"
 description = "Expands the existing Django TestCase class with extra functionality."
 readme = "readme.md"
 authors = [
     { name = "Brandon Rodriguez", email = "brodriguez8774@gmail.com" },
 ]
 maintainers = [
     { name = "Brandon Rodriguez", email = "brodriguez8774@gmail.com" },
@@ -61,7 +61,12 @@
     "sphinx",
     "sphinx-autobuild",
     "sphinx-rtd-theme",
 ]
 
 [project.urls]
 Homepage = "https://github.com/brodriguez8774/django-expanded-test-cases"
+
+
+[tool.black]
+line-length = 120
+skip-string-normalization = 1
```

### Comparing `django-expanded-test-cases-0.7.0/readme.md` & `django_expanded_test_cases-0.7.1/readme.md`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.7.0/setup.cfg` & `django_expanded_test_cases-0.7.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-expanded-test-cases
-version = 0.7.0
+version = 0.7.1
 description = Expands the existing Django TestCase class with extra functionality.
 long_description = file: readme.md
 url = https://github.com/brodriguez8774/django-expanded-test-cases
 author = Brandon Rodriguez
 author_email = brodriguez8774@gmail.com
 license = MIT License
 classifiers =
```

