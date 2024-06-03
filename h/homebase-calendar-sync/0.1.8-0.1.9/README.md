# Comparing `tmp/homebase_calendar_sync-0.1.8.tar.gz` & `tmp/homebase_calendar_sync-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homebase_calendar_sync-0.1.8.tar", last modified: Mon Jun  3 00:42:24 2024, max compression
+gzip compressed data, was "homebase_calendar_sync-0.1.9.tar", last modified: Mon Jun  3 00:50:04 2024, max compression
```

## Comparing `homebase_calendar_sync-0.1.8.tar` & `homebase_calendar_sync-0.1.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-03 00:42:24.755879 homebase_calendar_sync-0.1.8/
--rw-r--r--   0 davidmidlo   (501) staff       (20)     4341 2024-06-03 00:42:24.755671 homebase_calendar_sync-0.1.8/PKG-INFO
--rw-r--r--   0 davidmidlo   (501) staff       (20)     1891 2024-06-03 00:41:59.000000 homebase_calendar_sync-0.1.8/README.md
--rw-r--r--   0 davidmidlo   (501) staff       (20)       38 2024-06-03 00:42:24.755918 homebase_calendar_sync-0.1.8/setup.cfg
--rw-r--r--   0 davidmidlo   (501) staff       (20)     1009 2024-06-03 00:40:17.000000 homebase_calendar_sync-0.1.8/setup.py
-drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-03 00:42:24.750304 homebase_calendar_sync-0.1.8/src/
-drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-03 00:42:24.751715 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync/
--rw-r--r--   0 davidmidlo   (501) staff       (20)      269 2024-06-02 18:56:09.000000 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync/__init__.py
--rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 13:57:40.000000 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync/__main__.py
--rw-r--r--   0 davidmidlo   (501) staff       (20)      937 2024-06-03 00:32:52.000000 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync/config.py
-drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-03 00:42:24.753584 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync/db/
--rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 14:47:10.000000 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync/db/__init__.py
--rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 14:47:19.000000 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync/db/__main__.py
--rw-r--r--   0 davidmidlo   (501) staff       (20)     1084 2024-06-02 19:48:42.000000 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync/db/models.py
-drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-03 00:42:24.754942 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync/google_client/
--rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 14:47:33.000000 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync/google_client/__init__.py
--rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 14:47:49.000000 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync/google_client/__main__.py
--rw-r--r--   0 davidmidlo   (501) staff       (20)    19548 2024-06-02 22:59:26.000000 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync/google_client/auth.py
--rw-r--r--   0 davidmidlo   (501) staff       (20)      106 2024-06-02 04:40:28.000000 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync/google_client/drive_types.py
--rw-r--r--   0 davidmidlo   (501) staff       (20)     9441 2024-06-02 22:37:29.000000 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync/google_client/google_client.py
--rw-r--r--   0 davidmidlo   (501) staff       (20)    16434 2024-06-03 00:35:23.000000 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync/homebase_calendar_sync.py
-drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-03 00:42:24.755268 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync.egg-info/
--rw-r--r--   0 davidmidlo   (501) staff       (20)     4341 2024-06-03 00:42:24.000000 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync.egg-info/PKG-INFO
--rw-r--r--   0 davidmidlo   (501) staff       (20)      881 2024-06-03 00:42:24.000000 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync.egg-info/SOURCES.txt
--rw-r--r--   0 davidmidlo   (501) staff       (20)        1 2024-06-03 00:42:24.000000 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync.egg-info/dependency_links.txt
--rw-r--r--   0 davidmidlo   (501) staff       (20)       94 2024-06-03 00:42:24.000000 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync.egg-info/entry_points.txt
--rw-r--r--   0 davidmidlo   (501) staff       (20)     1080 2024-06-03 00:42:24.000000 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync.egg-info/requires.txt
--rw-r--r--   0 davidmidlo   (501) staff       (20)       23 2024-06-03 00:42:24.000000 homebase_calendar_sync-0.1.8/src/homebase_calendar_sync.egg-info/top_level.txt
+drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-03 00:50:04.541273 homebase_calendar_sync-0.1.9/
+-rw-r--r--   0 davidmidlo   (501) staff       (20)     4515 2024-06-03 00:50:04.541039 homebase_calendar_sync-0.1.9/PKG-INFO
+-rw-r--r--   0 davidmidlo   (501) staff       (20)     1891 2024-06-03 00:41:59.000000 homebase_calendar_sync-0.1.9/README.md
+-rw-r--r--   0 davidmidlo   (501) staff       (20)       38 2024-06-03 00:50:04.541320 homebase_calendar_sync-0.1.9/setup.cfg
+-rw-r--r--   0 davidmidlo   (501) staff       (20)     1009 2024-06-03 00:49:46.000000 homebase_calendar_sync-0.1.9/setup.py
+drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-03 00:50:04.536564 homebase_calendar_sync-0.1.9/src/
+drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-03 00:50:04.537608 homebase_calendar_sync-0.1.9/src/homebase_calendar_sync/
+-rw-r--r--   0 davidmidlo   (501) staff       (20)      269 2024-06-02 18:56:09.000000 homebase_calendar_sync-0.1.9/src/homebase_calendar_sync/__init__.py
+-rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 13:57:40.000000 homebase_calendar_sync-0.1.9/src/homebase_calendar_sync/__main__.py
+-rw-r--r--   0 davidmidlo   (501) staff       (20)      937 2024-06-03 00:32:52.000000 homebase_calendar_sync-0.1.9/src/homebase_calendar_sync/config.py
+drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-03 00:50:04.539179 homebase_calendar_sync-0.1.9/src/homebase_calendar_sync/db/
+-rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 14:47:10.000000 homebase_calendar_sync-0.1.9/src/homebase_calendar_sync/db/__init__.py
+-rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 14:47:19.000000 homebase_calendar_sync-0.1.9/src/homebase_calendar_sync/db/__main__.py
+-rw-r--r--   0 davidmidlo   (501) staff       (20)     1084 2024-06-02 19:48:42.000000 homebase_calendar_sync-0.1.9/src/homebase_calendar_sync/db/models.py
+drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-03 00:50:04.540325 homebase_calendar_sync-0.1.9/src/homebase_calendar_sync/google_client/
+-rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 14:47:33.000000 homebase_calendar_sync-0.1.9/src/homebase_calendar_sync/google_client/__init__.py
+-rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 14:47:49.000000 homebase_calendar_sync-0.1.9/src/homebase_calendar_sync/google_client/__main__.py
+-rw-r--r--   0 davidmidlo   (501) staff       (20)    19548 2024-06-02 22:59:26.000000 homebase_calendar_sync-0.1.9/src/homebase_calendar_sync/google_client/auth.py
+-rw-r--r--   0 davidmidlo   (501) staff       (20)      106 2024-06-02 04:40:28.000000 homebase_calendar_sync-0.1.9/src/homebase_calendar_sync/google_client/drive_types.py
+-rw-r--r--   0 davidmidlo   (501) staff       (20)     9441 2024-06-02 22:37:29.000000 homebase_calendar_sync-0.1.9/src/homebase_calendar_sync/google_client/google_client.py
+-rw-r--r--   0 davidmidlo   (501) staff       (20)    16434 2024-06-03 00:35:23.000000 homebase_calendar_sync-0.1.9/src/homebase_calendar_sync/homebase_calendar_sync.py
+drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-03 00:50:04.540642 homebase_calendar_sync-0.1.9/src/homebase_calendar_sync.egg-info/
+-rw-r--r--   0 davidmidlo   (501) staff       (20)     4515 2024-06-03 00:50:04.000000 homebase_calendar_sync-0.1.9/src/homebase_calendar_sync.egg-info/PKG-INFO
+-rw-r--r--   0 davidmidlo   (501) staff       (20)      881 2024-06-03 00:50:04.000000 homebase_calendar_sync-0.1.9/src/homebase_calendar_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 davidmidlo   (501) staff       (20)        1 2024-06-03 00:50:04.000000 homebase_calendar_sync-0.1.9/src/homebase_calendar_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 davidmidlo   (501) staff       (20)       94 2024-06-03 00:50:04.000000 homebase_calendar_sync-0.1.9/src/homebase_calendar_sync.egg-info/entry_points.txt
+-rw-r--r--   0 davidmidlo   (501) staff       (20)     1179 2024-06-03 00:50:04.000000 homebase_calendar_sync-0.1.9/src/homebase_calendar_sync.egg-info/requires.txt
+-rw-r--r--   0 davidmidlo   (501) staff       (20)       23 2024-06-03 00:50:04.000000 homebase_calendar_sync-0.1.9/src/homebase_calendar_sync.egg-info/top_level.txt
```

### Comparing `homebase_calendar_sync-0.1.8/PKG-INFO` & `homebase_calendar_sync-0.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homebase_calendar_sync
-Version: 0.1.8
+Version: 0.1.9
 Summary: A simple web scraper that reads gethomebase.com's schedule and updates Google Calendar.
 Home-page: https://github.com/dmidlo/homebase_calendar_sync
 Author: David Midlo
 Author-email: dmidlo@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,27 +23,31 @@
 Requires-Dist: google-api-core==2.19.0
 Requires-Dist: google-api-python-client==2.131.0
 Requires-Dist: google-auth==2.29.0
 Requires-Dist: google-auth-httplib2==0.2.0
 Requires-Dist: google-auth-oauthlib==1.2.0
 Requires-Dist: googleapis-common-protos==1.63.0
 Requires-Dist: h11==0.14.0
+Requires-Dist: homebase_calendar_sync==0.1.8
 Requires-Dist: httpcore==1.0.5
 Requires-Dist: httplib2==0.22.0
 Requires-Dist: httpx==0.27.0
 Requires-Dist: idna==3.7
+Requires-Dist: inquirerpy==0.3.4
 Requires-Dist: markdown-it-py==3.0.0
 Requires-Dist: mdurl==0.1.2
 Requires-Dist: mypy-extensions==1.0.0
 Requires-Dist: oauthlib==3.2.2
 Requires-Dist: outcome==1.3.0.post0
 Requires-Dist: packaging==24.0
 Requires-Dist: pathspec==0.12.1
 Requires-Dist: pendulum==3.0.0
+Requires-Dist: pfzy==0.3.4
 Requires-Dist: platformdirs==4.2.2
+Requires-Dist: prompt_toolkit==3.0.45
 Requires-Dist: proto-plus==1.23.0
 Requires-Dist: protobuf==4.25.3
 Requires-Dist: pyasn1==0.6.0
 Requires-Dist: pyasn1_modules==0.4.0
 Requires-Dist: pycparser==2.22
 Requires-Dist: Pygments==2.18.0
 Requires-Dist: pyparsing==3.1.2
@@ -64,14 +68,15 @@
 Requires-Dist: time-machine==2.14.1
 Requires-Dist: trio==0.25.1
 Requires-Dist: trio-websocket==0.11.1
 Requires-Dist: typing_extensions==4.12.0
 Requires-Dist: tzdata==2024.1
 Requires-Dist: uritemplate==4.1.1
 Requires-Dist: urllib3==2.2.1
+Requires-Dist: wcwidth==0.2.13
 Requires-Dist: wsproto==1.2.0
 
 ```
 homebase_calendar_sync --help
 usage: homebase_calendar_sync [-h] [--import-secret [IMPORT_SECRET]] [--reset-remote] [--reset-db] [--reset-events] [--reset-auth] [--reset-local]
                               [--reset-all]
```

### Comparing `homebase_calendar_sync-0.1.8/README.md` & `homebase_calendar_sync-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `homebase_calendar_sync-0.1.8/setup.py` & `homebase_calendar_sync-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 from setuptools import setup, find_packages
 
 setup(
     name='homebase_calendar_sync',
-    version='0.1.8',
+    version='0.1.9',
     author='David Midlo',
     author_email='dmidlo@gmail.com',
     description='A simple web scraper that reads gethomebase.com\'s schedule and updates Google Calendar.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/dmidlo/homebase_calendar_sync',  # Update this to your project's URL
     packages=find_packages(where='src'),
```

### Comparing `homebase_calendar_sync-0.1.8/src/homebase_calendar_sync/config.py` & `homebase_calendar_sync-0.1.9/src/homebase_calendar_sync/config.py`

 * *Files identical despite different names*

### Comparing `homebase_calendar_sync-0.1.8/src/homebase_calendar_sync/db/models.py` & `homebase_calendar_sync-0.1.9/src/homebase_calendar_sync/db/models.py`

 * *Files identical despite different names*

### Comparing `homebase_calendar_sync-0.1.8/src/homebase_calendar_sync/google_client/auth.py` & `homebase_calendar_sync-0.1.9/src/homebase_calendar_sync/google_client/auth.py`

 * *Files identical despite different names*

### Comparing `homebase_calendar_sync-0.1.8/src/homebase_calendar_sync/google_client/google_client.py` & `homebase_calendar_sync-0.1.9/src/homebase_calendar_sync/google_client/google_client.py`

 * *Files identical despite different names*

### Comparing `homebase_calendar_sync-0.1.8/src/homebase_calendar_sync/homebase_calendar_sync.py` & `homebase_calendar_sync-0.1.9/src/homebase_calendar_sync/homebase_calendar_sync.py`

 * *Files identical despite different names*

### Comparing `homebase_calendar_sync-0.1.8/src/homebase_calendar_sync.egg-info/PKG-INFO` & `homebase_calendar_sync-0.1.9/src/homebase_calendar_sync.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homebase_calendar_sync
-Version: 0.1.8
+Version: 0.1.9
 Summary: A simple web scraper that reads gethomebase.com's schedule and updates Google Calendar.
 Home-page: https://github.com/dmidlo/homebase_calendar_sync
 Author: David Midlo
 Author-email: dmidlo@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,27 +23,31 @@
 Requires-Dist: google-api-core==2.19.0
 Requires-Dist: google-api-python-client==2.131.0
 Requires-Dist: google-auth==2.29.0
 Requires-Dist: google-auth-httplib2==0.2.0
 Requires-Dist: google-auth-oauthlib==1.2.0
 Requires-Dist: googleapis-common-protos==1.63.0
 Requires-Dist: h11==0.14.0
+Requires-Dist: homebase_calendar_sync==0.1.8
 Requires-Dist: httpcore==1.0.5
 Requires-Dist: httplib2==0.22.0
 Requires-Dist: httpx==0.27.0
 Requires-Dist: idna==3.7
+Requires-Dist: inquirerpy==0.3.4
 Requires-Dist: markdown-it-py==3.0.0
 Requires-Dist: mdurl==0.1.2
 Requires-Dist: mypy-extensions==1.0.0
 Requires-Dist: oauthlib==3.2.2
 Requires-Dist: outcome==1.3.0.post0
 Requires-Dist: packaging==24.0
 Requires-Dist: pathspec==0.12.1
 Requires-Dist: pendulum==3.0.0
+Requires-Dist: pfzy==0.3.4
 Requires-Dist: platformdirs==4.2.2
+Requires-Dist: prompt_toolkit==3.0.45
 Requires-Dist: proto-plus==1.23.0
 Requires-Dist: protobuf==4.25.3
 Requires-Dist: pyasn1==0.6.0
 Requires-Dist: pyasn1_modules==0.4.0
 Requires-Dist: pycparser==2.22
 Requires-Dist: Pygments==2.18.0
 Requires-Dist: pyparsing==3.1.2
@@ -64,14 +68,15 @@
 Requires-Dist: time-machine==2.14.1
 Requires-Dist: trio==0.25.1
 Requires-Dist: trio-websocket==0.11.1
 Requires-Dist: typing_extensions==4.12.0
 Requires-Dist: tzdata==2024.1
 Requires-Dist: uritemplate==4.1.1
 Requires-Dist: urllib3==2.2.1
+Requires-Dist: wcwidth==0.2.13
 Requires-Dist: wsproto==1.2.0
 
 ```
 homebase_calendar_sync --help
 usage: homebase_calendar_sync [-h] [--import-secret [IMPORT_SECRET]] [--reset-remote] [--reset-db] [--reset-events] [--reset-auth] [--reset-local]
                               [--reset-all]
```

### Comparing `homebase_calendar_sync-0.1.8/src/homebase_calendar_sync.egg-info/SOURCES.txt` & `homebase_calendar_sync-0.1.9/src/homebase_calendar_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `homebase_calendar_sync-0.1.8/src/homebase_calendar_sync.egg-info/requires.txt` & `homebase_calendar_sync-0.1.9/src/homebase_calendar_sync.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -11,27 +11,31 @@
 google-api-core==2.19.0
 google-api-python-client==2.131.0
 google-auth==2.29.0
 google-auth-httplib2==0.2.0
 google-auth-oauthlib==1.2.0
 googleapis-common-protos==1.63.0
 h11==0.14.0
+homebase_calendar_sync==0.1.8
 httpcore==1.0.5
 httplib2==0.22.0
 httpx==0.27.0
 idna==3.7
+inquirerpy==0.3.4
 markdown-it-py==3.0.0
 mdurl==0.1.2
 mypy-extensions==1.0.0
 oauthlib==3.2.2
 outcome==1.3.0.post0
 packaging==24.0
 pathspec==0.12.1
 pendulum==3.0.0
+pfzy==0.3.4
 platformdirs==4.2.2
+prompt_toolkit==3.0.45
 proto-plus==1.23.0
 protobuf==4.25.3
 pyasn1==0.6.0
 pyasn1_modules==0.4.0
 pycparser==2.22
 Pygments==2.18.0
 pyparsing==3.1.2
@@ -52,8 +56,9 @@
 time-machine==2.14.1
 trio==0.25.1
 trio-websocket==0.11.1
 typing_extensions==4.12.0
 tzdata==2024.1
 uritemplate==4.1.1
 urllib3==2.2.1
+wcwidth==0.2.13
 wsproto==1.2.0
```

