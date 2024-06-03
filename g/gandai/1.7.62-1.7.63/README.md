# Comparing `tmp/gandai-1.7.62.tar.gz` & `tmp/gandai-1.7.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gandai-1.7.62.tar", last modified: Wed May 29 19:39:42 2024, max compression
+gzip compressed data, was "gandai-1.7.63.tar", last modified: Mon Jun  3 15:10:23 2024, max compression
```

## Comparing `gandai-1.7.62.tar` & `gandai-1.7.63.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 19:39:42.273670 gandai-1.7.62/
--rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.7.62/MANIFEST.in
--rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-29 19:39:42.273434 gandai-1.7.62/PKG-INFO
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 19:39:42.266437 gandai-1.7.62/gandai/
--rw-r--r--   0 parker     (501) staff       (20)      429 2023-11-27 12:36:32.000000 gandai-1.7.62/gandai/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 19:39:42.270351 gandai-1.7.62/gandai/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      750 2023-11-27 12:36:32.000000 gandai-1.7.62/gandai/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.7.62/gandai/__pycache__/adapters.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     8783 2024-03-29 15:43:44.000000 gandai-1.7.62/gandai/__pycache__/analytics.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-27 20:57:55.000000 gandai-1.7.62/gandai/__pycache__/auth.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2623 2024-05-29 02:35:57.000000 gandai-1.7.62/gandai/__pycache__/constants.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.7.62/gandai/__pycache__/datastore.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2014 2024-03-29 15:42:35.000000 gandai-1.7.62/gandai/__pycache__/db.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2168 2023-11-20 15:35:11.000000 gandai-1.7.62/gandai/__pycache__/google.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    17445 2024-05-29 12:27:02.000000 gandai-1.7.62/gandai/__pycache__/gpt.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1673 2024-05-29 02:22:28.000000 gandai-1.7.62/gandai/__pycache__/grata.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2703 2024-05-29 00:06:01.000000 gandai-1.7.62/gandai/__pycache__/helpers.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    16266 2024-05-29 19:34:01.000000 gandai-1.7.62/gandai/__pycache__/main.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    10401 2024-05-29 00:06:00.000000 gandai-1.7.62/gandai/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    46276 2024-05-29 19:33:57.000000 gandai-1.7.62/gandai/__pycache__/query.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2237 2023-11-20 15:35:11.000000 gandai-1.7.62/gandai/__pycache__/secrets.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.7.62/gandai/__pycache__/services.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    13620 2023-11-15 17:26:28.000000 gandai-1.7.62/gandai/__pycache__/sources.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1697 2024-05-29 19:36:04.000000 gandai-1.7.62/gandai/__pycache__/tasks.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5714 2024-03-29 15:34:07.000000 gandai-1.7.62/gandai/analytics.py
--rw-r--r--   0 parker     (501) staff       (20)     1700 2024-05-29 02:35:57.000000 gandai-1.7.62/gandai/constants.py
--rw-r--r--   0 parker     (501) staff       (20)     1202 2024-03-29 15:34:07.000000 gandai-1.7.62/gandai/db.py
--rw-r--r--   0 parker     (501) staff       (20)     1036 2023-11-17 19:29:48.000000 gandai-1.7.62/gandai/google.py
--rw-r--r--   0 parker     (501) staff       (20)    16796 2024-05-29 12:26:59.000000 gandai-1.7.62/gandai/gpt.py
--rw-r--r--   0 parker     (501) staff       (20)     4127 2024-05-29 02:22:25.000000 gandai-1.7.62/gandai/grata.py
--rw-r--r--   0 parker     (501) staff       (20)     1283 2024-05-29 00:05:27.000000 gandai-1.7.62/gandai/helpers.py
--rw-r--r--   0 parker     (501) staff       (20)    13093 2024-05-29 19:33:57.000000 gandai-1.7.62/gandai/main.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 19:39:42.271077 gandai-1.7.62/gandai/migrations/
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.7.62/gandai/migrations/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 19:39:42.271591 gandai-1.7.62/gandai/migrations/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.7.62/gandai/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.7.62/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.7.62/gandai/migrations/db_create.py
--rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.7.62/gandai/migrations/db_seed.py
--rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.7.62/gandai/migrations/dealcloud.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 19:39:42.272896 gandai-1.7.62/gandai/migrations/sql/
--rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.7.62/gandai/migrations/sql/2305023-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)     1720 2023-09-05 16:26:02.000000 gandai-1.7.62/gandai/migrations/sql/230818-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)      136 2024-05-24 15:09:36.000000 gandai-1.7.62/gandai/migrations/sql/240523-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)     3021 2024-05-28 15:04:19.000000 gandai-1.7.62/gandai/migrations/sql/schema.sql
--rw-r--r--   0 parker     (501) staff       (20)     4501 2024-05-29 00:05:27.000000 gandai-1.7.62/gandai/models.py
--rw-r--r--   0 parker     (501) staff       (20)    31724 2024-05-29 19:33:54.000000 gandai-1.7.62/gandai/query.py
--rw-r--r--   0 parker     (501) staff       (20)     1129 2023-11-17 19:29:48.000000 gandai-1.7.62/gandai/secrets.py
--rw-r--r--   0 parker     (501) staff       (20)     1081 2024-05-29 19:36:01.000000 gandai-1.7.62/gandai/tasks.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-29 19:39:42.273185 gandai-1.7.62/gandai.egg-info/
--rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-29 19:39:42.000000 gandai-1.7.62/gandai.egg-info/PKG-INFO
--rw-r--r--   0 parker     (501) staff       (20)     1517 2024-05-29 19:39:42.000000 gandai-1.7.62/gandai.egg-info/SOURCES.txt
--rw-r--r--   0 parker     (501) staff       (20)        1 2024-05-29 19:39:42.000000 gandai-1.7.62/gandai.egg-info/dependency_links.txt
--rw-r--r--   0 parker     (501) staff       (20)        7 2024-05-29 19:39:42.000000 gandai-1.7.62/gandai.egg-info/top_level.txt
--rw-r--r--   0 parker     (501) staff       (20)      384 2024-05-29 19:39:33.000000 gandai-1.7.62/pyproject.toml
--rw-r--r--   0 parker     (501) staff       (20)       38 2024-05-29 19:39:42.273711 gandai-1.7.62/setup.cfg
--rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.7.62/setup.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-06-03 15:10:23.725256 gandai-1.7.63/
+-rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.7.63/MANIFEST.in
+-rw-r--r--   0 parker     (501) staff       (20)      215 2024-06-03 15:10:23.725070 gandai-1.7.63/PKG-INFO
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-06-03 15:10:23.713676 gandai-1.7.63/gandai/
+-rw-r--r--   0 parker     (501) staff       (20)      429 2023-11-27 12:36:32.000000 gandai-1.7.63/gandai/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-06-03 15:10:23.720892 gandai-1.7.63/gandai/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      750 2023-11-27 12:36:32.000000 gandai-1.7.63/gandai/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.7.63/gandai/__pycache__/adapters.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     8783 2024-03-29 15:43:44.000000 gandai-1.7.63/gandai/__pycache__/analytics.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-27 20:57:55.000000 gandai-1.7.63/gandai/__pycache__/auth.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2623 2024-05-29 02:35:57.000000 gandai-1.7.63/gandai/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.7.63/gandai/__pycache__/datastore.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2014 2024-03-29 15:42:35.000000 gandai-1.7.63/gandai/__pycache__/db.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2168 2023-11-20 15:35:11.000000 gandai-1.7.63/gandai/__pycache__/google.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    17445 2024-05-30 18:05:53.000000 gandai-1.7.63/gandai/__pycache__/gpt.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5730 2024-06-03 15:01:06.000000 gandai-1.7.63/gandai/__pycache__/grata.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2703 2024-05-29 00:06:01.000000 gandai-1.7.63/gandai/__pycache__/helpers.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    17329 2024-06-03 15:08:46.000000 gandai-1.7.63/gandai/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    10484 2024-06-03 14:59:18.000000 gandai-1.7.63/gandai/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    47406 2024-06-03 15:07:15.000000 gandai-1.7.63/gandai/__pycache__/query.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2237 2023-11-20 15:35:11.000000 gandai-1.7.63/gandai/__pycache__/secrets.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.7.63/gandai/__pycache__/services.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    13620 2023-11-15 17:26:28.000000 gandai-1.7.63/gandai/__pycache__/sources.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1697 2024-05-29 19:36:04.000000 gandai-1.7.63/gandai/__pycache__/tasks.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5714 2024-03-29 15:34:07.000000 gandai-1.7.63/gandai/analytics.py
+-rw-r--r--   0 parker     (501) staff       (20)     1700 2024-05-29 02:35:57.000000 gandai-1.7.63/gandai/constants.py
+-rw-r--r--   0 parker     (501) staff       (20)     1202 2024-03-29 15:34:07.000000 gandai-1.7.63/gandai/db.py
+-rw-r--r--   0 parker     (501) staff       (20)     1036 2023-11-17 19:29:48.000000 gandai-1.7.63/gandai/google.py
+-rw-r--r--   0 parker     (501) staff       (20)    16796 2024-05-30 18:05:53.000000 gandai-1.7.63/gandai/gpt.py
+-rw-r--r--   0 parker     (501) staff       (20)     3968 2024-06-03 15:01:03.000000 gandai-1.7.63/gandai/grata.py
+-rw-r--r--   0 parker     (501) staff       (20)     1283 2024-05-29 00:05:27.000000 gandai-1.7.63/gandai/helpers.py
+-rw-r--r--   0 parker     (501) staff       (20)    11952 2024-06-03 15:08:44.000000 gandai-1.7.63/gandai/main.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-06-03 15:10:23.721921 gandai-1.7.63/gandai/migrations/
+-rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.7.63/gandai/migrations/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-06-03 15:10:23.722611 gandai-1.7.63/gandai/migrations/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.7.63/gandai/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.7.63/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.7.63/gandai/migrations/db_create.py
+-rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.7.63/gandai/migrations/db_seed.py
+-rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.7.63/gandai/migrations/dealcloud.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-06-03 15:10:23.724331 gandai-1.7.63/gandai/migrations/sql/
+-rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.7.63/gandai/migrations/sql/2305023-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)     1720 2023-09-05 16:26:02.000000 gandai-1.7.63/gandai/migrations/sql/230818-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)      136 2024-05-24 15:09:36.000000 gandai-1.7.63/gandai/migrations/sql/240523-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)     3021 2024-05-28 15:04:19.000000 gandai-1.7.63/gandai/migrations/sql/schema.sql
+-rw-r--r--   0 parker     (501) staff       (20)     4499 2024-06-03 14:59:16.000000 gandai-1.7.63/gandai/models.py
+-rw-r--r--   0 parker     (501) staff       (20)    32396 2024-06-03 15:07:12.000000 gandai-1.7.63/gandai/query.py
+-rw-r--r--   0 parker     (501) staff       (20)     1129 2023-11-17 19:29:48.000000 gandai-1.7.63/gandai/secrets.py
+-rw-r--r--   0 parker     (501) staff       (20)     1081 2024-05-29 19:36:01.000000 gandai-1.7.63/gandai/tasks.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-06-03 15:10:23.724886 gandai-1.7.63/gandai.egg-info/
+-rw-r--r--   0 parker     (501) staff       (20)      215 2024-06-03 15:10:23.000000 gandai-1.7.63/gandai.egg-info/PKG-INFO
+-rw-r--r--   0 parker     (501) staff       (20)     1517 2024-06-03 15:10:23.000000 gandai-1.7.63/gandai.egg-info/SOURCES.txt
+-rw-r--r--   0 parker     (501) staff       (20)        1 2024-06-03 15:10:23.000000 gandai-1.7.63/gandai.egg-info/dependency_links.txt
+-rw-r--r--   0 parker     (501) staff       (20)        7 2024-06-03 15:10:23.000000 gandai-1.7.63/gandai.egg-info/top_level.txt
+-rw-r--r--   0 parker     (501) staff       (20)      384 2024-06-03 15:10:03.000000 gandai-1.7.63/pyproject.toml
+-rw-r--r--   0 parker     (501) staff       (20)       38 2024-06-03 15:10:23.725299 gandai-1.7.63/setup.cfg
+-rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.7.63/setup.py
```

### Comparing `gandai-1.7.62/gandai/__pycache__/__init__.cpython-311.pyc` & `gandai-1.7.63/gandai/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.62/gandai/__pycache__/adapters.cpython-311.pyc` & `gandai-1.7.63/gandai/__pycache__/adapters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.62/gandai/__pycache__/analytics.cpython-311.pyc` & `gandai-1.7.63/gandai/__pycache__/analytics.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.62/gandai/__pycache__/auth.cpython-311.pyc` & `gandai-1.7.63/gandai/__pycache__/auth.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.62/gandai/__pycache__/constants.cpython-311.pyc` & `gandai-1.7.63/gandai/__pycache__/constants.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.62/gandai/__pycache__/datastore.cpython-311.pyc` & `gandai-1.7.63/gandai/__pycache__/datastore.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.62/gandai/__pycache__/db.cpython-311.pyc` & `gandai-1.7.63/gandai/__pycache__/db.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.62/gandai/__pycache__/google.cpython-311.pyc` & `gandai-1.7.63/gandai/__pycache__/google.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.62/gandai/__pycache__/gpt.cpython-311.pyc` & `gandai-1.7.63/gandai/__pycache__/gpt.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x131f5766 (Wed May 29 12:26:59 2024 UTC)
+moddate:  0x01c05866 (Thu May 30 18:05:53 2024 UTC)
 files sz: 16796
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `gandai-1.7.62/gandai/__pycache__/helpers.cpython-311.pyc` & `gandai-1.7.63/gandai/__pycache__/helpers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.62/gandai/__pycache__/main.cpython-311.pyc` & `gandai-1.7.63/gandai/__pycache__/main.cpython-311.pyc`

 * *Files 3% similar despite different names*

#### Python bytecode

```diff
@@ -1,29 +1,31 @@
 magic:    0xa70d0d0a
-moddate:  0x25835766 (Wed May 29 19:33:57 2024 UTC)
-files sz: 13093
+moddate:  0x7cdc5d66 (Mon Jun  3 15:08:44 2024 UTC)
+files sz: 11952
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d025a020100640064
       036c035a04640064036c055a05640064046c066d075a070100640064056c
       036d085a080100640665096602640784045a0a640865046a0b0000000000
       0000006a0c000000000000000064066509640964036606640a84045a0d64
       0865046a0b00000000000000006a0c0000000000000000640b65046a0b00
       000000000000006a0e0000000000000000640964036606640c84045a0f64
       0865046a0b00000000000000006a0c0000000000000000640b65046a0b00
       000000000000006a0e0000000000000000640964036606640d84045a1064
+      0865046a0b00000000000000006a0c0000000000000000640b65046a0b00
+      000000000000006a0e0000000000000000640964036606640e84045a1164
       0b65046a0b00000000000000006a0e000000000000000064096403660464
-      0e84045a11640f65046a0b00000000000000006a12000000000000000064
-      0964036604641084045a13640b65046a0b00000000000000006a0e000000
-      0000000000640964036604641184045a1464126515640964036604641384
-      045a1664035300
+      0f84045a12641065046a0b00000000000000006a13000000000000000064
+      0964036604641184045a14640b65046a0b00000000000000006a0e000000
+      0000000000640964036604641284045a1564136516640964036604641484
+      045a1764035300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('asdict',))
                  6 IMPORT_NAME              0 (dataclasses)
                  8 IMPORT_FROM              1 (asdict)
                 10 STORE_NAME               1 (asdict)
@@ -76,87 +78,102 @@
                106 LOAD_CONST               9 ('return')
                108 LOAD_CONST               3 (None)
                110 BUILD_TUPLE              6
                112 LOAD_CONST              10 (<code object run_similarity_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 48>)
                114 MAKE_FUNCTION            4 (annotations)
                116 STORE_NAME              13 (run_similarity_search)
    
-    73         118 LOAD_CONST               8 ('search')
+    61         118 LOAD_CONST               8 ('search')
                120 LOAD_NAME                4 (ts)
                122 LOAD_ATTR               11 (models)
                132 LOAD_ATTR               12 (Search)
                142 LOAD_CONST              11 ('event')
                144 LOAD_NAME                4 (ts)
                146 LOAD_ATTR               11 (models)
                156 LOAD_ATTR               14 (Event)
                166 LOAD_CONST               9 ('return')
                168 LOAD_CONST               3 (None)
                170 BUILD_TUPLE              6
-               172 LOAD_CONST              12 (<code object run_maps_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 73>)
+               172 LOAD_CONST              12 (<code object run_criteria_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 61>)
                174 MAKE_FUNCTION            4 (annotations)
-               176 STORE_NAME              15 (run_maps_search)
+               176 STORE_NAME              15 (run_criteria_search)
    
-   118         178 LOAD_CONST               8 ('search')
+    75         178 LOAD_CONST               8 ('search')
                180 LOAD_NAME                4 (ts)
                182 LOAD_ATTR               11 (models)
                192 LOAD_ATTR               12 (Search)
                202 LOAD_CONST              11 ('event')
                204 LOAD_NAME                4 (ts)
                206 LOAD_ATTR               11 (models)
                216 LOAD_ATTR               14 (Event)
                226 LOAD_CONST               9 ('return')
                228 LOAD_CONST               3 (None)
                230 BUILD_TUPLE              6
-               232 LOAD_CONST              13 (<code object run_google_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 118>)
+               232 LOAD_CONST              13 (<code object run_maps_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 75>)
                234 MAKE_FUNCTION            4 (annotations)
-               236 STORE_NAME              16 (run_google_search)
+               236 STORE_NAME              16 (run_maps_search)
    
-   173         238 LOAD_CONST              11 ('event')
+   120         238 LOAD_CONST               8 ('search')
                240 LOAD_NAME                4 (ts)
                242 LOAD_ATTR               11 (models)
-               252 LOAD_ATTR               14 (Event)
-               262 LOAD_CONST               9 ('return')
-               264 LOAD_CONST               3 (None)
-               266 BUILD_TUPLE              4
-               268 LOAD_CONST              14 (<code object handle_prompt, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 173>)
-               270 MAKE_FUNCTION            4 (annotations)
-               272 STORE_NAME              17 (handle_prompt)
+               252 LOAD_ATTR               12 (Search)
+               262 LOAD_CONST              11 ('event')
+               264 LOAD_NAME                4 (ts)
+               266 LOAD_ATTR               11 (models)
+               276 LOAD_ATTR               14 (Event)
+               286 LOAD_CONST               9 ('return')
+               288 LOAD_CONST               3 (None)
+               290 BUILD_TUPLE              6
+               292 LOAD_CONST              14 (<code object run_google_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 120>)
+               294 MAKE_FUNCTION            4 (annotations)
+               296 STORE_NAME              17 (run_google_search)
+   
+   137         298 LOAD_CONST              11 ('event')
+               300 LOAD_NAME                4 (ts)
+               302 LOAD_ATTR               11 (models)
+               312 LOAD_ATTR               14 (Event)
+               322 LOAD_CONST               9 ('return')
+               324 LOAD_CONST               3 (None)
+               326 BUILD_TUPLE              4
+               328 LOAD_CONST              15 (<code object handle_prompt, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 137>)
+               330 MAKE_FUNCTION            4 (annotations)
+               332 STORE_NAME              18 (handle_prompt)
    
-   219         274 LOAD_CONST              15 ('company')
-               276 LOAD_NAME                4 (ts)
-               278 LOAD_ATTR               11 (models)
-               288 LOAD_ATTR               18 (Company)
-               298 LOAD_CONST               9 ('return')
-               300 LOAD_CONST               3 (None)
-               302 BUILD_TUPLE              4
-               304 LOAD_CONST              16 (<code object enrich_with_gpt, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 219>)
-               306 MAKE_FUNCTION            4 (annotations)
-               308 STORE_NAME              19 (enrich_with_gpt)
+   183         334 LOAD_CONST              16 ('company')
+               336 LOAD_NAME                4 (ts)
+               338 LOAD_ATTR               11 (models)
+               348 LOAD_ATTR               19 (Company)
+               358 LOAD_CONST               9 ('return')
+               360 LOAD_CONST               3 (None)
+               362 BUILD_TUPLE              4
+               364 LOAD_CONST              17 (<code object enrich_with_gpt, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 183>)
+               366 MAKE_FUNCTION            4 (annotations)
+               368 STORE_NAME              20 (enrich_with_gpt)
    
-   258         310 LOAD_CONST              11 ('event')
-               312 LOAD_NAME                4 (ts)
-               314 LOAD_ATTR               11 (models)
-               324 LOAD_ATTR               14 (Event)
-               334 LOAD_CONST               9 ('return')
-               336 LOAD_CONST               3 (None)
-               338 BUILD_TUPLE              4
-               340 LOAD_CONST              17 (<code object run_enrichment, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 258>)
-               342 MAKE_FUNCTION            4 (annotations)
-               344 STORE_NAME              20 (run_enrichment)
+   222         370 LOAD_CONST              11 ('event')
+               372 LOAD_NAME                4 (ts)
+               374 LOAD_ATTR               11 (models)
+               384 LOAD_ATTR               14 (Event)
+               394 LOAD_CONST               9 ('return')
+               396 LOAD_CONST               3 (None)
+               398 BUILD_TUPLE              4
+               400 LOAD_CONST              18 (<code object run_enrichment, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 222>)
+               402 MAKE_FUNCTION            4 (annotations)
+               404 STORE_NAME              21 (run_enrichment)
    
-   277         346 LOAD_CONST              18 ('event_id')
-               348 LOAD_NAME               21 (int)
-               350 LOAD_CONST               9 ('return')
-               352 LOAD_CONST               3 (None)
-               354 BUILD_TUPLE              4
-               356 LOAD_CONST              19 (<code object process_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 277>)
-               358 MAKE_FUNCTION            4 (annotations)
-               360 STORE_NAME              22 (process_event)
-               362 LOAD_CONST               3 (None)
-               364 RETURN_VALUE
+   241         406 LOAD_CONST              19 ('event_id')
+               408 LOAD_NAME               22 (int)
+               410 LOAD_CONST               9 ('return')
+               412 LOAD_CONST               3 (None)
+               414 BUILD_TUPLE              4
+               416 LOAD_CONST              20 (<code object process_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 241>)
+               418 MAKE_FUNCTION            4 (annotations)
+               420 STORE_NAME              23 (process_event)
+               422 LOAD_CONST               3 (None)
+               424 RETURN_VALUE
    consts
       0
       ('asdict',)
       ('time',)
       None
       ('from_dict',)
       ('secrets',)
@@ -328,73 +345,157 @@
       code
          argcount  : 2
          nlocals   : 3
          stacksize : 7
          flags     : 3
          code
             0x97007400000000000000000000006a010000000000000000a002000000
-            00000000000000000000000000000000007c017c00ac01a6020000ab0200
-            000000000000007d027400000000000000000000006a0300000000000000
-            00a00400000000000000000000000000000000000000007c027c006a0500
-            00000000000000640264037c019b009d026404ac05a6050000ab05000000
-            0000000000010064005300
+            00000000000000000000000000000000007c006a030000000000000000ac
+            01a6010000ab0100000000000000007c005f040000000000000000740000
+            0000000000000000006a050000000000000000a006000000000000000000
+            00000000000000000000007c017c00ac02a6020000ab0200000000000000
+            007d027400000000000000000000006a010000000000000000a007000000
+            00000000000000000000000000000000007c027c006a0300000000000000
+            00640364047c019b009d026405ac06a6050000ab05000000000000000001
+            0064005300
           48           0 RESUME                   0
          
           49           2 LOAD_GLOBAL              0 (ts)
-                      14 LOAD_ATTR                1 (grata)
-                      24 LOAD_METHOD              2 (find_similar)
-                      46 LOAD_FAST                1 (domain)
-                      48 LOAD_FAST                0 (search)
-                      50 KW_NAMES                 1
-                      52 PRECALL                  2
-                      56 CALL                     2
-                      66 STORE_FAST               2 (grata_companies)
-         
-          50          68 LOAD_GLOBAL              0 (ts)
-                      80 LOAD_ATTR                3 (query)
-                      90 LOAD_METHOD              4 (insert_companies_as_targets)
-         
-          51         112 LOAD_FAST                2 (grata_companies)
-         
-          52         114 LOAD_FAST                0 (search)
-                     116 LOAD_ATTR                5 (uid)
-         
-          53         126 LOAD_CONST               2 ('grata')
-         
-          55         128 LOAD_CONST               3 ('grata/')
+                      14 LOAD_ATTR                1 (query)
+                      24 LOAD_METHOD              2 (find_search_criteria)
+                      46 LOAD_FAST                0 (search)
+                      48 LOAD_ATTR                3 (uid)
+                      58 KW_NAMES                 1
+                      60 PRECALL                  1
+                      64 CALL                     1
+                      74 LOAD_FAST                0 (search)
+                      76 STORE_ATTR               4 (criteria)
+         
+          50          86 LOAD_GLOBAL              0 (ts)
+                      98 LOAD_ATTR                5 (grata)
+                     108 LOAD_METHOD              6 (find_similar)
                      130 LOAD_FAST                1 (domain)
-                     132 FORMAT_VALUE             0
-                     134 BUILD_STRING             2
-         
-          56         136 LOAD_CONST               4 ('similar')
-         
-          50         138 KW_NAMES                 5
-                     140 PRECALL                  5
-                     144 CALL                     5
-                     154 POP_TOP
-                     156 LOAD_CONST               0 (None)
-                     158 RETURN_VALUE
+                     132 LOAD_FAST                0 (search)
+                     134 KW_NAMES                 2
+                     136 PRECALL                  2
+                     140 CALL                     2
+                     150 STORE_FAST               2 (grata_companies)
+         
+          51         152 LOAD_GLOBAL              0 (ts)
+                     164 LOAD_ATTR                1 (query)
+                     174 LOAD_METHOD              7 (insert_companies_as_targets)
+         
+          52         196 LOAD_FAST                2 (grata_companies)
+         
+          53         198 LOAD_FAST                0 (search)
+                     200 LOAD_ATTR                3 (uid)
+         
+          54         210 LOAD_CONST               3 ('grata')
+         
+          56         212 LOAD_CONST               4 ('grata/')
+                     214 LOAD_FAST                1 (domain)
+                     216 FORMAT_VALUE             0
+                     218 BUILD_STRING             2
+         
+          57         220 LOAD_CONST               5 ('similar')
+         
+          51         222 KW_NAMES                 6
+                     224 PRECALL                  5
+                     228 CALL                     5
+                     238 POP_TOP
+                     240 LOAD_CONST               0 (None)
+                     242 RETURN_VALUE
          consts
             None
+            ('search_uid',)
             ('domain', 'search')
             'grata'
             'grata/'
             'similar'
             ('companies', 'search_uid', 'actor_key', 'source', 'stage')
-         names      ('ts', 'grata', 'find_similar', 'query', 'insert_companies_as_targets', 'uid')
+         names      ('ts', 'query', 'find_search_criteria', 'uid', 'criteria', 'grata', 'find_similar', 'insert_companies_as_targets')
          varnames   ('search', 'domain', 'grata_companies')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
          name       'run_similarity_search'
          firstlineno 48
-         lnotab 0x020142012c0102010c010202080102fa
+         lnotab 0x0201540142012c0102010c010202080102fa
       'event'
       code
          argcount  : 2
+         nlocals   : 3
+         stacksize : 7
+         flags     : 3
+         code
+            0x97007401000000000000000000007402000000000000000000006a0200
+            000000000000006a0300000000000000007c016a040000000000000000a6
+            020000ab0200000000000000007c005f0500000000000000007402000000
+            000000000000006a060000000000000000a0070000000000000000000000
+            0000000000000000007c00a6010000ab0100000000000000007d02740200
+            0000000000000000006a080000000000000000a009000000000000000000
+            00000000000000000000007c027c006a0a00000000000000006401640264
+            01ac03a6050000ab050000000000000000010064005300
+          61           0 RESUME                   0
+         
+          64           2 LOAD_GLOBAL              1 (NULL + from_dict)
+                      14 LOAD_GLOBAL              2 (ts)
+                      26 LOAD_ATTR                2 (models)
+                      36 LOAD_ATTR                3 (Criteria)
+                      46 LOAD_FAST                1 (event)
+                      48 LOAD_ATTR                4 (data)
+                      58 PRECALL                  2
+                      62 CALL                     2
+                      72 LOAD_FAST                0 (search)
+                      74 STORE_ATTR               5 (criteria)
+         
+          65          84 LOAD_GLOBAL              2 (ts)
+                      96 LOAD_ATTR                6 (grata)
+                     106 LOAD_METHOD              7 (find_by_criteria)
+                     128 LOAD_FAST                0 (search)
+                     130 PRECALL                  1
+                     134 CALL                     1
+                     144 STORE_FAST               2 (grata_companies)
+         
+          66         146 LOAD_GLOBAL              2 (ts)
+                     158 LOAD_ATTR                8 (query)
+                     168 LOAD_METHOD              9 (insert_companies_as_targets)
+         
+          67         190 LOAD_FAST                2 (grata_companies)
+         
+          68         192 LOAD_FAST                0 (search)
+                     194 LOAD_ATTR               10 (uid)
+         
+          69         204 LOAD_CONST               1 ('grata')
+         
+          70         206 LOAD_CONST               2 (True)
+         
+          71         208 LOAD_CONST               1 ('grata')
+         
+          66         210 KW_NAMES                 3
+                     212 PRECALL                  5
+                     216 CALL                     5
+                     226 POP_TOP
+                     228 LOAD_CONST               0 (None)
+                     230 RETURN_VALUE
+         consts
+            None
+            'grata'
+            True
+            ('companies', 'search_uid', 'actor_key', 'force', 'source')
+         names      ('from_dict', 'ts', 'models', 'Criteria', 'data', 'criteria', 'grata', 'find_by_criteria', 'query', 'insert_companies_as_targets', 'uid')
+         varnames   ('search', 'event', 'grata_companies')
+         freevars   ()
+         cellvars   ()
+         filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
+         name       'run_criteria_search'
+         firstlineno 61
+         lnotab 0x020352013e012c0102010c010201020102fb
+      code
+         argcount  : 2
          nlocals   : 6
          stacksize : 6
          flags     : 3
          code
             0x870697007400000000000000000000006a010000000000000000a00200
             000000000000000000000000000000000000007c006a0300000000000000
             00ac01a6010000ab010000000000000000640219000000000000000000a0
@@ -407,92 +508,92 @@
             0100000000000000007d047417000000000000000000007c04a6010000ab
             01000000000000000001007c04640319000000000000000000a00c000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             0044005d0f7d0502007c027c057c00ac09a6020000ab0200000000000000
             0001008c1064005300
                        0 MAKE_CELL                6 (existing_search_domains)
          
-          73           2 RESUME                   0
+          75           2 RESUME                   0
          
-          74           4 LOAD_GLOBAL              0 (ts)
+          76           4 LOAD_GLOBAL              0 (ts)
                       16 LOAD_ATTR                1 (query)
                       26 LOAD_METHOD              2 (search_targets)
                       48 LOAD_FAST                0 (search)
                       50 LOAD_ATTR                3 (uid)
                       60 KW_NAMES                 1
                       62 PRECALL                  1
                       66 CALL                     1
          
-          75          76 LOAD_CONST               2 ('domain')
+          77          76 LOAD_CONST               2 ('domain')
          
-          74          78 BINARY_SUBSCR
+          76          78 BINARY_SUBSCR
          
-          76          88 LOAD_METHOD              4 (to_list)
+          78          88 LOAD_METHOD              4 (to_list)
                      110 PRECALL                  0
                      114 CALL                     0
          
-          74         124 STORE_DEREF              6 (existing_search_domains)
+          76         124 STORE_DEREF              6 (existing_search_domains)
          
-          78         126 LOAD_CONST               3 ('place_id')
+          80         126 LOAD_CONST               3 ('place_id')
                      128 LOAD_GLOBAL             10 (str)
                      140 LOAD_CONST               4 ('search')
                      142 LOAD_GLOBAL              0 (ts)
                      154 LOAD_ATTR                6 (models)
                      164 LOAD_ATTR                7 (Search)
                      174 LOAD_CONST               5 ('return')
                      176 LOAD_CONST               0 (None)
                      178 BUILD_TUPLE              6
                      180 LOAD_CLOSURE             6 (existing_search_domains)
                      182 BUILD_TUPLE              1
-                     184 LOAD_CONST               6 (<code object build_place, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 78>)
+                     184 LOAD_CONST               6 (<code object build_place, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 80>)
                      186 MAKE_FUNCTION           12 (annotations, closure)
                      188 STORE_FAST               2 (build_place)
          
-         109         190 LOAD_FAST                1 (event)
+         111         190 LOAD_FAST                1 (event)
                      192 LOAD_ATTR                8 (data)
                      202 LOAD_CONST               7 ('query')
                      204 BINARY_SUBSCR
                      214 STORE_FAST               3 (q)
          
-         110         216 LOAD_GLOBAL              0 (ts)
+         112         216 LOAD_GLOBAL              0 (ts)
                      228 LOAD_ATTR                9 (google)
                      238 LOAD_METHOD             10 (get_google_places)
                      260 LOAD_FAST                3 (q)
                      262 KW_NAMES                 8
                      264 PRECALL                  1
                      268 CALL                     1
                      278 STORE_FAST               4 (results)
          
-         111         280 LOAD_GLOBAL             23 (NULL + print)
+         113         280 LOAD_GLOBAL             23 (NULL + print)
                      292 LOAD_FAST                4 (results)
                      294 PRECALL                  1
                      298 CALL                     1
                      308 POP_TOP
          
-         114         310 LOAD_FAST                4 (results)
+         116         310 LOAD_FAST                4 (results)
                      312 LOAD_CONST               3 ('place_id')
                      314 BINARY_SUBSCR
                      324 LOAD_METHOD             12 (tolist)
                      346 PRECALL                  0
                      350 CALL                     0
                      360 GET_ITER
                  >>  362 FOR_ITER                15 (to 394)
                      364 STORE_FAST               5 (place)
          
-         115         366 PUSH_NULL
+         117         366 PUSH_NULL
                      368 LOAD_FAST                2 (build_place)
                      370 LOAD_FAST                5 (place)
                      372 LOAD_FAST                0 (search)
                      374 KW_NAMES                 9
                      376 PRECALL                  2
                      380 CALL                     2
                      390 POP_TOP
                      392 JUMP_BACKWARD           16 (to 362)
          
-         114     >>  394 LOAD_CONST               0 (None)
+         116     >>  394 LOAD_CONST               0 (None)
                      396 RETURN_VALUE
          consts
             None
             ('search_uid',)
             'domain'
             'place_id'
             'search'
@@ -523,131 +624,131 @@
                   000000000000007c016a0f0000000000000000640a7c066a0d0000000000
                   000000640b640c7c036901ac0da6050000ab0500000000000000007d0774
                   00000000000000000000006a0a0000000000000000a01000000000000000
                   000000000000000000000000007c07a6010000ab01000000000000000001
                   0064005300
                              0 COPY_FREE_VARS           1
                
-                78           2 RESUME                   0
+                80           2 RESUME                   0
                
-                79           4 LOAD_GLOBAL              0 (ts)
+                81           4 LOAD_GLOBAL              0 (ts)
                             16 LOAD_ATTR                1 (google)
                             26 LOAD_ATTR                2 (gmaps)
                             36 LOAD_METHOD              3 (place)
                
-                80          58 LOAD_FAST                0 (place_id)
+                82          58 LOAD_FAST                0 (place_id)
                             60 BUILD_LIST               0
                             62 LOAD_CONST               1 (('name', 'website', 'reviews'))
                             64 LIST_EXTEND              1
                
-                79          66 KW_NAMES                 2
+                81          66 KW_NAMES                 2
                             68 PRECALL                  2
                             72 CALL                     2
                             82 STORE_FAST               2 (resp)
                
-                82          84 LOAD_FAST                2 (resp)
+                84          84 LOAD_FAST                2 (resp)
                             86 LOAD_CONST               3 ('result')
                             88 BINARY_SUBSCR
                             98 STORE_FAST               3 (place)
                
-                83         100 LOAD_GLOBAL              0 (ts)
+                85         100 LOAD_GLOBAL              0 (ts)
                            112 LOAD_ATTR                4 (helpers)
                            122 LOAD_METHOD              5 (clean_domain)
                            144 LOAD_FAST                3 (place)
                            146 LOAD_METHOD              6 (get)
                            168 LOAD_CONST               4 ('website')
                            170 PRECALL                  1
                            174 CALL                     1
                            184 PRECALL                  1
                            188 CALL                     1
                            198 STORE_FAST               4 (domain)
                
-                84         200 LOAD_FAST                4 (domain)
+                86         200 LOAD_FAST                4 (domain)
                            202 POP_JUMP_FORWARD_IF_NOT_NONE     2 (to 208)
                
-                85         204 LOAD_CONST               0 (None)
+                87         204 LOAD_CONST               0 (None)
                            206 RETURN_VALUE
                
-                86     >>  208 LOAD_FAST                4 (domain)
+                88     >>  208 LOAD_FAST                4 (domain)
                            210 LOAD_DEREF               8 (existing_search_domains)
                            212 CONTAINS_OP              0
                            214 POP_JUMP_FORWARD_IF_FALSE    21 (to 258)
                
-                87         216 LOAD_GLOBAL             15 (NULL + print)
+                89         216 LOAD_GLOBAL             15 (NULL + print)
                            228 LOAD_CONST               5 ('domain ')
                            230 LOAD_FAST                4 (domain)
                            232 FORMAT_VALUE             0
                            234 LOAD_CONST               6 (' already in search. skipping...')
                            236 BUILD_STRING             3
                            238 PRECALL                  1
                            242 CALL                     1
                            252 POP_TOP
                
-                88         254 LOAD_CONST               0 (None)
+                90         254 LOAD_CONST               0 (None)
                            256 RETURN_VALUE
                
-                89     >>  258 LOAD_GLOBAL              0 (ts)
+                91     >>  258 LOAD_GLOBAL              0 (ts)
                            270 LOAD_ATTR                8 (models)
                            280 LOAD_METHOD              9 (Company)
                
-                90         302 LOAD_FAST                3 (place)
+                92         302 LOAD_FAST                3 (place)
                            304 LOAD_CONST               7 ('name')
                            306 BINARY_SUBSCR
                
-                91         316 LOAD_FAST                4 (domain)
+                93         316 LOAD_FAST                4 (domain)
                
-                92         318 LOAD_CONST               8 ('Map API')
+                94         318 LOAD_CONST               8 ('Map API')
                
-                89         320 KW_NAMES                 9
+                91         320 KW_NAMES                 9
                            322 PRECALL                  3
                            326 CALL                     3
                            336 STORE_FAST               5 (new_company)
                
-                94         338 LOAD_GLOBAL              0 (ts)
+                96         338 LOAD_GLOBAL              0 (ts)
                            350 LOAD_ATTR               10 (query)
                            360 LOAD_METHOD             11 (insert_company)
                            382 LOAD_FAST                5 (new_company)
                            384 PRECALL                  1
                            388 CALL                     1
                            398 POP_TOP
                
-                95         400 LOAD_GLOBAL              0 (ts)
+                97         400 LOAD_GLOBAL              0 (ts)
                            412 LOAD_ATTR               10 (query)
                            422 LOAD_METHOD             12 (find_company_by_domain)
                            444 LOAD_FAST                5 (new_company)
                            446 LOAD_ATTR               13 (domain)
                            456 PRECALL                  1
                            460 CALL                     1
                            470 STORE_FAST               6 (company)
                
-                97         472 LOAD_GLOBAL              0 (ts)
+                99         472 LOAD_GLOBAL              0 (ts)
                            484 LOAD_ATTR                8 (models)
                            494 LOAD_METHOD             14 (Event)
                
-                98         516 LOAD_FAST                1 (search)
+               100         516 LOAD_FAST                1 (search)
                            518 LOAD_ATTR               15 (uid)
                
-                99         528 LOAD_CONST              10 ('create')
+               101         528 LOAD_CONST              10 ('create')
                
-               100         530 LOAD_FAST                6 (company)
+               102         530 LOAD_FAST                6 (company)
                            532 LOAD_ATTR               13 (domain)
                
-               101         542 LOAD_CONST              11 ('google')
+               103         542 LOAD_CONST              11 ('google')
                
-               103         544 LOAD_CONST              12 ('place')
+               105         544 LOAD_CONST              12 ('place')
                            546 LOAD_FAST                3 (place)
                
-               102         548 BUILD_MAP                1
+               104         548 BUILD_MAP                1
                
-                97         550 KW_NAMES                13
+                99         550 KW_NAMES                13
                            552 PRECALL                  5
                            556 CALL                     5
                            566 STORE_FAST               7 (event)
                
-               107         568 LOAD_GLOBAL              0 (ts)
+               109         568 LOAD_GLOBAL              0 (ts)
                            580 LOAD_ATTR               10 (query)
                            590 LOAD_METHOD             16 (insert_event)
                            612 LOAD_FAST                7 (event)
                            614 PRECALL                  1
                            618 CALL                     1
                            628 POP_TOP
                            630 LOAD_CONST               0 (None)
@@ -669,28 +770,28 @@
                   ('search_uid', 'type', 'domain', 'actor_key', 'data')
                names      ('ts', 'google', 'gmaps', 'place', 'helpers', 'clean_domain', 'get', 'print', 'models', 'Company', 'query', 'insert_company', 'find_company_by_domain', 'domain', 'Event', 'uid', 'insert_event')
                varnames   ('place_id', 'search', 'resp', 'place', 'domain', 'new_company', 'company', 'event')
                freevars   ('existing_search_domains',)
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
                name       'build_place'
-               firstlineno 78
+               firstlineno 80
                lnotab
                   0x0401360108ff120310016401040104010801260104012c010e01020102
                   fd12053e0148022c010c0102010c01020204ff02fb120a
             'query'
             ('q',)
             ('place_id', 'search')
          names      ('ts', 'query', 'search_targets', 'uid', 'to_list', 'str', 'models', 'Search', 'data', 'google', 'get_google_places', 'print', 'tolist')
          varnames   ('search', 'event', 'build_place', 'q', 'results', 'place')
          freevars   ()
          cellvars   ('existing_search_domains',)
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
          name       'run_maps_search'
-         firstlineno 73
+         firstlineno 75
          lnotab 0x0401480102ff0a0224fe0204401f1a0140011e0338011cff
       code
          argcount  : 2
          nlocals   : 4
          stacksize : 7
          flags     : 3
          code
@@ -707,36 +808,36 @@
             00ab0100000000000000007d037411000000000000000000007c03a60100
             00ab01000000000000000001007404000000000000000000006a09000000
             0000000000a00a00000000000000000000000000000000000000007c0364
             09640b670219000000000000000000a00b00000000000000000000000000
             00000000000000640dac0ea6010000ab0100000000000000007c016a0c00
             000000000000007c016a0d0000000000000000640fac10a6040000ab0400
             00000000000000010064005300
-         118           0 RESUME                   0
+         120           0 RESUME                   0
          
-         119           2 LOAD_FAST                1 (event)
+         121           2 LOAD_FAST                1 (event)
                        4 LOAD_ATTR                0 (data)
                       14 LOAD_CONST               1 ('q')
                       16 BINARY_SUBSCR
                       26 STORE_FAST               2 (q)
          
-         120          28 LOAD_GLOBAL              3 (NULL + len)
+         122          28 LOAD_GLOBAL              3 (NULL + len)
                       40 LOAD_FAST                2 (q)
                       42 PRECALL                  1
                       46 CALL                     1
                       56 LOAD_CONST               2 (0)
                       58 COMPARE_OP               4 (>)
                       64 POP_JUMP_FORWARD_IF_TRUE    10 (to 86)
                       66 LOAD_ASSERTION_ERROR
                       68 LOAD_CONST               3 ('q must be a non-empty string')
                       70 PRECALL                  0
                       74 CALL                     0
                       84 RAISE_VARARGS            1
          
-         121     >>   86 LOAD_GLOBAL              4 (ts)
+         123     >>   86 LOAD_GLOBAL              4 (ts)
                       98 LOAD_ATTR                3 (google)
                      108 LOAD_METHOD              4 (search)
                      130 LOAD_FAST                2 (q)
                      132 LOAD_FAST                1 (event)
                      134 LOAD_ATTR                0 (data)
                      144 LOAD_METHOD              5 (get)
                      166 LOAD_CONST               4 ('count')
@@ -744,66 +845,66 @@
                      170 PRECALL                  2
                      174 CALL                     2
                      184 KW_NAMES                 6
                      186 PRECALL                  2
                      190 CALL                     2
                      200 STORE_FAST               3 (results)
          
-         122         202 LOAD_FAST                3 (results)
+         124         202 LOAD_FAST                3 (results)
                      204 LOAD_CONST               7 ('link')
                      206 BINARY_SUBSCR
                      216 LOAD_METHOD              6 (apply)
-                     238 LOAD_CONST               8 (<code object <lambda>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 122>)
+                     238 LOAD_CONST               8 (<code object <lambda>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 124>)
                      240 MAKE_FUNCTION            0
                      242 PRECALL                  1
                      246 CALL                     1
                      256 LOAD_FAST                3 (results)
                      258 LOAD_CONST               9 ('domain')
                      260 STORE_SUBSCR
          
-         123         264 LOAD_FAST                3 (results)
+         125         264 LOAD_FAST                3 (results)
                      266 LOAD_METHOD              7 (rename)
                      288 LOAD_CONST              10 ('snippet')
                      290 LOAD_CONST              11 ('description')
                      292 BUILD_MAP                1
                      294 KW_NAMES                12
                      296 PRECALL                  1
                      300 CALL                     1
                      310 STORE_FAST               3 (results)
          
-         124         312 LOAD_GLOBAL             17 (NULL + print)
+         126         312 LOAD_GLOBAL             17 (NULL + print)
                      324 LOAD_FAST                3 (results)
                      326 PRECALL                  1
                      330 CALL                     1
                      340 POP_TOP
          
-         125         342 LOAD_GLOBAL              4 (ts)
+         127         342 LOAD_GLOBAL              4 (ts)
                      354 LOAD_ATTR                9 (query)
                      364 LOAD_METHOD             10 (insert_companies_as_targets)
          
-         126         386 LOAD_FAST                3 (results)
+         128         386 LOAD_FAST                3 (results)
                      388 LOAD_CONST               9 ('domain')
                      390 LOAD_CONST              11 ('description')
                      392 BUILD_LIST               2
                      394 BINARY_SUBSCR
                      404 LOAD_METHOD             11 (to_dict)
                      426 LOAD_CONST              13 ('records')
                      428 KW_NAMES                14
                      430 PRECALL                  1
                      434 CALL                     1
          
-         127         444 LOAD_FAST                1 (event)
+         129         444 LOAD_FAST                1 (event)
                      446 LOAD_ATTR               12 (search_uid)
          
-         128         456 LOAD_FAST                1 (event)
+         130         456 LOAD_FAST                1 (event)
                      458 LOAD_ATTR               13 (actor_key)
          
-         129         468 LOAD_CONST              15 ('Google')
+         131         468 LOAD_CONST              15 ('Google')
          
-         125         470 KW_NAMES                16
+         127         470 KW_NAMES                16
                      472 PRECALL                  4
                      476 CALL                     4
                      486 POP_TOP
                      488 LOAD_CONST               0 (None)
                      490 RETURN_VALUE
          consts
             None
@@ -819,15 +920,15 @@
                nlocals   : 1
                stacksize : 3
                flags     : 19
                code
                   0x97007400000000000000000000006a010000000000000000a002000000
                   00000000000000000000000000000000007c00a6010000ab010000000000
                   0000005300
-               122           0 RESUME                   0
+               124           0 RESUME                   0
                              2 LOAD_GLOBAL              0 (ts)
                             14 LOAD_ATTR                1 (helpers)
                             24 LOAD_METHOD              2 (clean_domain)
                             46 LOAD_FAST                0 (x)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 RETURN_VALUE
@@ -835,15 +936,15 @@
                   None
                names      ('ts', 'helpers', 'clean_domain')
                varnames   ('x',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
                name       '<lambda>'
-               firstlineno 122
+               firstlineno 124
                lnotab 0x
             'domain'
             'snippet'
             'description'
             ('columns',)
             'records'
             ('orient',)
@@ -851,15 +952,15 @@
             ('companies', 'search_uid', 'actor_key', 'source')
          names      ('data', 'len', 'ts', 'google', 'search', 'get', 'apply', 'rename', 'print', 'query', 'insert_companies_as_targets', 'to_dict', 'search_uid', 'actor_key')
          varnames   ('search', 'event', 'q', 'results')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
          name       'run_google_search'
-         firstlineno 118
+         firstlineno 120
          lnotab 0x02011a013a0174013e0130011e012c013a010c010c0102fc
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 10
          flags     : 3
          code
@@ -882,169 +983,169 @@
             0000007402000000000000000000006a0d00000000000000006a0e000000
             00000000007c03a6020000ab0200000000000000007d0474010000000000
             00000000007c04a6010000ab01000000000000000001007c006a0a000000
             00000000006407190000000000000000007c046a0a000000000000000064
             073c0000007402000000000000000000006a0f0000000000000000a01000
             000000000000000000000000000000000000007c04a6010000ab01000000
             000000000001008c7f64005300
-         173           0 RESUME                   0
+         137           0 RESUME                   0
          
-         174           2 LOAD_GLOBAL              1 (NULL + print)
+         138           2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_CONST               1 ('prompt event:')
                       16 LOAD_FAST                0 (event)
                       18 PRECALL                  2
                       22 CALL                     2
                       32 POP_TOP
          
-         177          34 LOAD_CONST               2 ('system')
+         141          34 LOAD_CONST               2 ('system')
          
-         178          36 LOAD_GLOBAL              2 (ts)
+         142          36 LOAD_GLOBAL              2 (ts)
                       48 LOAD_ATTR                2 (gpt)
                       58 LOAD_ATTR                3 (HOW_TO_RESPOND)
          
-         176          68 LOAD_CONST               3 (('role', 'content'))
+         140          68 LOAD_CONST               3 (('role', 'content'))
                       70 BUILD_CONST_KEY_MAP      2
          
-         181          72 LOAD_CONST               2 ('system')
+         145          72 LOAD_CONST               2 ('system')
          
-         182          74 LOAD_GLOBAL              2 (ts)
+         146          74 LOAD_GLOBAL              2 (ts)
                       86 LOAD_ATTR                2 (gpt)
                       96 LOAD_ATTR                4 (HOW_TO_IMPORT)
          
-         180         106 LOAD_CONST               3 (('role', 'content'))
+         144         106 LOAD_CONST               3 (('role', 'content'))
                      108 BUILD_CONST_KEY_MAP      2
          
-         185         110 LOAD_CONST               2 ('system')
+         149         110 LOAD_CONST               2 ('system')
          
-         186         112 LOAD_GLOBAL              2 (ts)
+         150         112 LOAD_GLOBAL              2 (ts)
                      124 LOAD_ATTR                2 (gpt)
                      134 LOAD_ATTR                5 (HOW_TO_TRANSITION)
          
-         184         144 LOAD_CONST               3 (('role', 'content'))
+         148         144 LOAD_CONST               3 (('role', 'content'))
                      146 BUILD_CONST_KEY_MAP      2
          
-         189         148 LOAD_CONST               2 ('system')
+         153         148 LOAD_CONST               2 ('system')
          
-         190         150 LOAD_GLOBAL              2 (ts)
+         154         150 LOAD_GLOBAL              2 (ts)
                      162 LOAD_ATTR                2 (gpt)
                      172 LOAD_ATTR                6 (HOW_TO_GOOGLE)
          
-         188         182 LOAD_CONST               3 (('role', 'content'))
+         152         182 LOAD_CONST               3 (('role', 'content'))
                      184 BUILD_CONST_KEY_MAP      2
          
-         193         186 LOAD_CONST               2 ('system')
+         157         186 LOAD_CONST               2 ('system')
          
-         194         188 LOAD_GLOBAL              2 (ts)
+         158         188 LOAD_GLOBAL              2 (ts)
                      200 LOAD_ATTR                2 (gpt)
                      210 LOAD_ATTR                7 (HOW_TO_GOOGLE_MAPS)
          
-         192         220 LOAD_CONST               3 (('role', 'content'))
+         156         220 LOAD_CONST               3 (('role', 'content'))
                      222 BUILD_CONST_KEY_MAP      2
          
-         197         224 LOAD_CONST               2 ('system')
+         161         224 LOAD_CONST               2 ('system')
          
-         198         226 LOAD_CONST               4 ('the search_uid is ')
+         162         226 LOAD_CONST               4 ('the search_uid is ')
                      228 LOAD_FAST                0 (event)
                      230 LOAD_ATTR                8 (search_uid)
                      240 FORMAT_VALUE             0
                      242 BUILD_STRING             2
          
-         196         244 LOAD_CONST               3 (('role', 'content'))
+         160         244 LOAD_CONST               3 (('role', 'content'))
                      246 BUILD_CONST_KEY_MAP      2
          
-         201         248 LOAD_CONST               2 ('system')
+         165         248 LOAD_CONST               2 ('system')
          
-         202         250 LOAD_CONST               5 ('the actor_key is ')
+         166         250 LOAD_CONST               5 ('the actor_key is ')
                      252 LOAD_FAST                0 (event)
                      254 LOAD_ATTR                9 (actor_key)
                      264 FORMAT_VALUE             0
                      266 BUILD_STRING             2
          
-         200         268 LOAD_CONST               3 (('role', 'content'))
+         164         268 LOAD_CONST               3 (('role', 'content'))
                      270 BUILD_CONST_KEY_MAP      2
          
-         204         272 LOAD_CONST               6 ('user')
+         168         272 LOAD_CONST               6 ('user')
                      274 LOAD_FAST                0 (event)
                      276 LOAD_ATTR               10 (data)
                      286 LOAD_CONST               7 ('prompt')
                      288 BINARY_SUBSCR
                      298 LOAD_CONST               3 (('role', 'content'))
                      300 BUILD_CONST_KEY_MAP      2
          
-         175         302 BUILD_LIST               8
+         139         302 BUILD_LIST               8
                      304 STORE_FAST               1 (messages)
          
-         206         306 LOAD_GLOBAL              2 (ts)
+         170         306 LOAD_GLOBAL              2 (ts)
                      318 LOAD_ATTR                2 (gpt)
                      328 LOAD_METHOD             11 (ask_gpt4)
                      350 LOAD_FAST                1 (messages)
                      352 PRECALL                  1
                      356 CALL                     1
                      366 STORE_FAST               2 (resp)
          
-         208         368 LOAD_GLOBAL              1 (NULL + print)
+         172         368 LOAD_GLOBAL              1 (NULL + print)
                      380 LOAD_FAST                2 (resp)
                      382 PRECALL                  1
                      386 CALL                     1
                      396 POP_TOP
          
-         209         398 LOAD_FAST                2 (resp)
+         173         398 LOAD_FAST                2 (resp)
                      400 LOAD_CONST               8 ('events')
                      402 BINARY_SUBSCR
                      412 GET_ITER
                  >>  414 FOR_ITER               126 (to 668)
                      416 STORE_FAST               3 (new_event)
          
-         210         418 LOAD_GLOBAL              1 (NULL + print)
+         174         418 LOAD_GLOBAL              1 (NULL + print)
                      430 LOAD_CONST               9 ('new event:')
                      432 LOAD_FAST                3 (new_event)
                      434 PRECALL                  2
                      438 CALL                     2
                      448 POP_TOP
          
-         211         450 LOAD_FAST                0 (event)
+         175         450 LOAD_FAST                0 (event)
                      452 LOAD_ATTR                8 (search_uid)
                      462 LOAD_FAST                3 (new_event)
                      464 LOAD_CONST              10 ('search_uid')
                      466 STORE_SUBSCR
          
-         212         470 LOAD_GLOBAL             25 (NULL + from_dict)
+         176         470 LOAD_GLOBAL             25 (NULL + from_dict)
                      482 LOAD_GLOBAL              2 (ts)
                      494 LOAD_ATTR               13 (models)
                      504 LOAD_ATTR               14 (Event)
                      514 LOAD_FAST                3 (new_event)
                      516 PRECALL                  2
                      520 CALL                     2
                      530 STORE_FAST               4 (e)
          
-         213         532 LOAD_GLOBAL              1 (NULL + print)
+         177         532 LOAD_GLOBAL              1 (NULL + print)
                      544 LOAD_FAST                4 (e)
                      546 PRECALL                  1
                      550 CALL                     1
                      560 POP_TOP
          
-         215         562 LOAD_FAST                0 (event)
+         179         562 LOAD_FAST                0 (event)
                      564 LOAD_ATTR               10 (data)
                      574 LOAD_CONST               7 ('prompt')
                      576 BINARY_SUBSCR
                      586 LOAD_FAST                4 (e)
                      588 LOAD_ATTR               10 (data)
                      598 LOAD_CONST               7 ('prompt')
                      600 STORE_SUBSCR
          
-         216         604 LOAD_GLOBAL              2 (ts)
+         180         604 LOAD_GLOBAL              2 (ts)
                      616 LOAD_ATTR               15 (query)
                      626 LOAD_METHOD             16 (insert_event)
                      648 LOAD_FAST                4 (e)
                      650 PRECALL                  1
                      654 CALL                     1
                      664 POP_TOP
                      666 JUMP_BACKWARD          127 (to 414)
          
-         209     >>  668 LOAD_CONST               0 (None)
+         173     >>  668 LOAD_CONST               0 (None)
                      670 RETURN_VALUE
          consts
             None
             'prompt event:'
             'system'
             ('role', 'content')
             'the search_uid is '
@@ -1056,15 +1157,15 @@
             'search_uid'
          names      ('print', 'ts', 'gpt', 'HOW_TO_RESPOND', 'HOW_TO_IMPORT', 'HOW_TO_TRANSITION', 'HOW_TO_GOOGLE', 'HOW_TO_GOOGLE_MAPS', 'search_uid', 'actor_key', 'data', 'ask_gpt4', 'from_dict', 'models', 'Event', 'query', 'insert_event')
          varnames   ('event', 'messages', 'resp', 'new_event', 'e')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
          name       'handle_prompt'
-         firstlineno 173
+         firstlineno 137
          lnotab
             0x02012003020120fe0405020120fe0405020120fe0405020120fe040502
             0120fe0405020112fe0405020112fe04041ee3041f3e021e011401200114
             013e011e022a0140f9
       'company'
       code
          argcount  : 1
@@ -1090,165 +1191,165 @@
             00000000007c055f040000000000000000741d0000000000000000000074
             1f00000000000000000000a6000000ab000000000000000000a6010000ab
             0100000000000000007c056a100000000000000000640b3c000000740100
             0000000000000000007c05a6010000ab0100000000000000000100740200
             0000000000000000006a110000000000000000a012000000000000000000
             00000000000000000000007c05a6010000ab01000000000000000001007c
             045300
-         219           0 RESUME                   0
+         183           0 RESUME                   0
          
-         220           2 LOAD_GLOBAL              1 (NULL + print)
+         184           2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_CONST               1 ('enriching with gpt...')
                       16 PRECALL                  1
                       20 CALL                     1
                       30 POP_TOP
          
-         221          32 NOP
+         185          32 NOP
          
-         222          34 LOAD_GLOBAL              2 (ts)
+         186          34 LOAD_GLOBAL              2 (ts)
                       46 LOAD_ATTR                2 (helpers)
                       56 LOAD_METHOD              3 (get_homepage_text)
                       78 LOAD_FAST                0 (company)
                       80 LOAD_ATTR                4 (domain)
                       90 PRECALL                  1
                       94 CALL                     1
                      104 STORE_FAST               1 (homepage_text)
                      106 JUMP_FORWARD            40 (to 188)
                  >>  108 PUSH_EXC_INFO
          
-         223         110 LOAD_GLOBAL             10 (Exception)
+         187         110 LOAD_GLOBAL             10 (Exception)
                      122 CHECK_EXC_MATCH
                      124 POP_JUMP_FORWARD_IF_FALSE    27 (to 180)
                      126 STORE_FAST               2 (e)
          
-         224         128 LOAD_GLOBAL              1 (NULL + print)
+         188         128 LOAD_GLOBAL              1 (NULL + print)
                      140 LOAD_FAST                2 (e)
                      142 PRECALL                  1
                      146 CALL                     1
                      156 POP_TOP
          
-         225         158 LOAD_CONST               2 ('<could not fetch homepage>')
+         189         158 LOAD_CONST               2 ('<could not fetch homepage>')
                      160 STORE_FAST               1 (homepage_text)
                      162 POP_EXCEPT
                      164 LOAD_CONST               0 (None)
                      166 STORE_FAST               2 (e)
                      168 DELETE_FAST              2 (e)
                      170 JUMP_FORWARD             8 (to 188)
                  >>  172 LOAD_CONST               0 (None)
                      174 STORE_FAST               2 (e)
                      176 DELETE_FAST              2 (e)
                      178 RERAISE                  1
          
-         223     >>  180 RERAISE                  0
+         187     >>  180 RERAISE                  0
                  >>  182 COPY                     3
                      184 POP_EXCEPT
                      186 RERAISE                  1
          
-         228     >>  188 LOAD_CONST               3 ('system')
+         192     >>  188 LOAD_CONST               3 ('system')
          
-         229         190 LOAD_CONST               4 ('You will help us evaluate ')
+         193         190 LOAD_CONST               4 ('You will help us evaluate ')
                      192 LOAD_FAST                0 (company)
                      194 LOAD_ATTR                6 (name)
                      204 FORMAT_VALUE             0
                      206 LOAD_CONST               5 (' for acquisition.')
                      208 BUILD_STRING             3
          
-         227         210 LOAD_CONST               6 (('role', 'content'))
+         191         210 LOAD_CONST               6 (('role', 'content'))
                      212 BUILD_CONST_KEY_MAP      2
          
-         232         214 LOAD_CONST               3 ('system')
+         196         214 LOAD_CONST               3 ('system')
          
-         233         216 LOAD_CONST               7 ('You will consider this existing information: ')
+         197         216 LOAD_CONST               7 ('You will consider this existing information: ')
                      218 LOAD_GLOBAL             15 (NULL + asdict)
                      230 LOAD_FAST                0 (company)
                      232 PRECALL                  1
                      236 CALL                     1
                      246 FORMAT_VALUE             0
                      248 BUILD_STRING             2
          
-         231         250 LOAD_CONST               6 (('role', 'content'))
+         195         250 LOAD_CONST               6 (('role', 'content'))
                      252 BUILD_CONST_KEY_MAP      2
          
-         236         254 LOAD_CONST               3 ('system')
+         200         254 LOAD_CONST               3 ('system')
          
-         237         256 LOAD_CONST               8 ('You will consider this copy from the company homepage as the most up to date. homepage_text: ')
+         201         256 LOAD_CONST               8 ('You will consider this copy from the company homepage as the most up to date. homepage_text: ')
                      258 LOAD_FAST                1 (homepage_text)
                      260 FORMAT_VALUE             0
                      262 BUILD_STRING             2
          
-         235         264 LOAD_CONST               6 (('role', 'content'))
+         199         264 LOAD_CONST               6 (('role', 'content'))
                      266 BUILD_CONST_KEY_MAP      2
          
-         240         268 LOAD_CONST               3 ('system')
+         204         268 LOAD_CONST               3 ('system')
          
-         241         270 LOAD_CONST               9 ('You will respond with only the JSON object.')
+         205         270 LOAD_CONST               9 ('You will respond with only the JSON object.')
          
-         239         272 LOAD_CONST               6 (('role', 'content'))
+         203         272 LOAD_CONST               6 (('role', 'content'))
                      274 BUILD_CONST_KEY_MAP      2
          
-         244         276 LOAD_CONST              10 ('user')
+         208         276 LOAD_CONST              10 ('user')
          
-         245         278 LOAD_GLOBAL              2 (ts)
+         209         278 LOAD_GLOBAL              2 (ts)
                      290 LOAD_ATTR                8 (gpt)
                      300 LOAD_ATTR                9 (HOW_TO_ENRICH)
          
-         243         310 LOAD_CONST               6 (('role', 'content'))
+         207         310 LOAD_CONST               6 (('role', 'content'))
                      312 BUILD_CONST_KEY_MAP      2
          
-         226         314 BUILD_LIST               5
+         190         314 BUILD_LIST               5
                      316 STORE_FAST               3 (messages)
          
-         249         318 LOAD_GLOBAL              2 (ts)
+         213         318 LOAD_GLOBAL              2 (ts)
                      330 LOAD_ATTR                8 (gpt)
                      340 LOAD_METHOD             10 (ask_gpt4)
                      362 LOAD_FAST                3 (messages)
                      364 PRECALL                  1
                      368 CALL                     1
                      378 STORE_FAST               4 (resp)
          
-         250         380 LOAD_GLOBAL             23 (NULL + from_dict)
+         214         380 LOAD_GLOBAL             23 (NULL + from_dict)
                      392 LOAD_GLOBAL              2 (ts)
                      404 LOAD_ATTR               12 (models)
                      414 LOAD_ATTR               13 (Event)
                      424 LOAD_FAST                4 (resp)
                      426 PRECALL                  2
                      430 CALL                     2
                      440 STORE_FAST               5 (update_event)
          
-         251         442 LOAD_FAST                0 (company)
+         215         442 LOAD_FAST                0 (company)
                      444 LOAD_ATTR                4 (domain)
                      454 LOAD_FAST                5 (update_event)
                      456 STORE_ATTR               4 (domain)
          
-         252         466 LOAD_GLOBAL             29 (NULL + int)
+         216         466 LOAD_GLOBAL             29 (NULL + int)
                      478 LOAD_GLOBAL             31 (NULL + time)
                      490 PRECALL                  0
                      494 CALL                     0
                      504 PRECALL                  1
                      508 CALL                     1
                      518 LOAD_FAST                5 (update_event)
                      520 LOAD_ATTR               16 (data)
                      530 LOAD_CONST              11 ('gpt')
                      532 STORE_SUBSCR
          
-         253         536 LOAD_GLOBAL              1 (NULL + print)
+         217         536 LOAD_GLOBAL              1 (NULL + print)
                      548 LOAD_FAST                5 (update_event)
                      550 PRECALL                  1
                      554 CALL                     1
                      564 POP_TOP
          
-         254         566 LOAD_GLOBAL              2 (ts)
+         218         566 LOAD_GLOBAL              2 (ts)
                      578 LOAD_ATTR               17 (query)
                      588 LOAD_METHOD             18 (insert_event)
                      610 LOAD_FAST                5 (update_event)
                      612 PRECALL                  1
                      616 CALL                     1
                      626 POP_TOP
          
-         255         628 LOAD_FAST                4 (resp)
+         219         628 LOAD_FAST                4 (resp)
                      630 RETURN_VALUE
          ExceptionTable:
            34 to 104 -> 108 [0]
            108 to 126 -> 182 [1] lasti
            128 to 160 -> 172 [1] lasti
            172 to 180 -> 182 [1] lasti
          consts
@@ -1266,15 +1367,15 @@
             'gpt'
          names      ('print', 'ts', 'helpers', 'get_homepage_text', 'domain', 'Exception', 'name', 'asdict', 'gpt', 'HOW_TO_ENRICH', 'ask_gpt4', 'from_dict', 'models', 'Event', 'int', 'time', 'data', 'query', 'insert_event')
          varnames   ('company', 'homepage_text', 'e', 'messages', 'resp', 'update_event')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
          name       'enrich_with_gpt'
-         firstlineno 219
+         firstlineno 183
          lnotab
             0x02011e0102014c0112011e0116fe0805020114fe0405020122fe040502
             0108fe0405020102fe0405020120fe04ef04173e013e01180146011e013e
             01
       code
          argcount  : 1
          nlocals   : 4
@@ -1296,105 +1397,105 @@
             00000000000000a5017c03a5017c025f0400000000000000007402000000
             000000000000006a020000000000000000a00b0000000000000000000000
             0000000000000000007c02a6010000ab01000000000000000001007c026a
             040000000000000000a00500000000000000000000000000000000000000
             006405a6010000ab0100000000000000007211740d000000000000000000
             006406a6010000ab01000000000000000001006400530074190000000000
             00000000007c02ac07a6010000ab010000000000000000010064005300
-         258           0 RESUME                   0
+         222           0 RESUME                   0
          
-         259           2 LOAD_FAST                0 (event)
+         223           2 LOAD_FAST                0 (event)
                        4 LOAD_ATTR                0 (domain)
                       14 STORE_FAST               1 (domain)
          
-         261          16 LOAD_GLOBAL              2 (ts)
+         225          16 LOAD_GLOBAL              2 (ts)
                       28 LOAD_ATTR                2 (query)
                       38 LOAD_METHOD              3 (find_company_by_domain)
                       60 LOAD_FAST                1 (domain)
                       62 PRECALL                  1
                       66 CALL                     1
                       76 STORE_FAST               2 (company)
          
-         262          78 LOAD_FAST                2 (company)
+         226          78 LOAD_FAST                2 (company)
                       80 LOAD_ATTR                4 (meta)
                       90 LOAD_METHOD              5 (get)
                      112 LOAD_CONST               1 ('company_uid')
                      114 PRECALL                  1
                      118 CALL                     1
                      128 POP_JUMP_FORWARD_IF_FALSE    16 (to 162)
          
-         263         130 LOAD_GLOBAL             13 (NULL + print)
+         227         130 LOAD_GLOBAL             13 (NULL + print)
                      142 LOAD_CONST               2 ('company already exists. skipping enrichment...')
                      144 PRECALL                  1
                      148 CALL                     1
                      158 POP_TOP
                      160 JUMP_FORWARD           142 (to 446)
          
-         265     >>  162 LOAD_GLOBAL              2 (ts)
+         229     >>  162 LOAD_GLOBAL              2 (ts)
                      174 LOAD_ATTR                7 (grata)
                      184 LOAD_METHOD              8 (enrich)
                      206 LOAD_FAST                2 (company)
                      208 LOAD_ATTR                0 (domain)
                      218 PRECALL                  1
                      222 CALL                     1
                      232 STORE_FAST               3 (resp)
          
-         266         234 LOAD_FAST                2 (company)
+         230         234 LOAD_FAST                2 (company)
                      236 LOAD_ATTR                9 (name)
                      246 JUMP_IF_TRUE_OR_POP     20 (to 288)
                      248 LOAD_FAST                3 (resp)
                      250 LOAD_METHOD              5 (get)
                      272 LOAD_CONST               3 ('name')
                      274 PRECALL                  1
                      278 CALL                     1
                  >>  288 LOAD_FAST                2 (company)
                      290 STORE_ATTR               9 (name)
          
-         267         300 LOAD_FAST                3 (resp)
+         231         300 LOAD_FAST                3 (resp)
                      302 LOAD_METHOD              5 (get)
                      324 LOAD_CONST               4 ('description')
                      326 PRECALL                  1
                      330 CALL                     1
                      340 LOAD_FAST                2 (company)
                      342 STORE_ATTR              10 (description)
          
-         268         352 BUILD_MAP                0
+         232         352 BUILD_MAP                0
                      354 LOAD_FAST                2 (company)
                      356 LOAD_ATTR                4 (meta)
                      366 DICT_UPDATE              1
                      368 LOAD_FAST                3 (resp)
                      370 DICT_UPDATE              1
                      372 LOAD_FAST                2 (company)
                      374 STORE_ATTR               4 (meta)
          
-         269         384 LOAD_GLOBAL              2 (ts)
+         233         384 LOAD_GLOBAL              2 (ts)
                      396 LOAD_ATTR                2 (query)
                      406 LOAD_METHOD             11 (update_company)
                      428 LOAD_FAST                2 (company)
                      430 PRECALL                  1
                      434 CALL                     1
                      444 POP_TOP
          
-         271     >>  446 LOAD_FAST                2 (company)
+         235     >>  446 LOAD_FAST                2 (company)
                      448 LOAD_ATTR                4 (meta)
                      458 LOAD_METHOD              5 (get)
                      480 LOAD_CONST               5 ('gpt_description')
                      482 PRECALL                  1
                      486 CALL                     1
                      496 POP_JUMP_FORWARD_IF_FALSE    17 (to 532)
          
-         272         498 LOAD_GLOBAL             13 (NULL + print)
+         236         498 LOAD_GLOBAL             13 (NULL + print)
                      510 LOAD_CONST               6 ('company already enriched with gpt. skipping...')
                      512 PRECALL                  1
                      516 CALL                     1
                      526 POP_TOP
                      528 LOAD_CONST               0 (None)
                      530 RETURN_VALUE
          
-         274     >>  532 LOAD_GLOBAL             25 (NULL + enrich_with_gpt)
+         238     >>  532 LOAD_GLOBAL             25 (NULL + enrich_with_gpt)
                      544 LOAD_FAST                2 (company)
                      546 KW_NAMES                 7
                      548 PRECALL                  1
                      552 CALL                     1
                      562 POP_TOP
                      564 LOAD_CONST               0 (None)
                      566 RETURN_VALUE
@@ -1409,15 +1510,15 @@
             ('company',)
          names      ('domain', 'ts', 'query', 'find_company_by_domain', 'meta', 'get', 'print', 'grata', 'enrich', 'name', 'description', 'update_company', 'enrich_with_gpt')
          varnames   ('event', 'domain', 'company', 'resp')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
          name       'run_enrichment'
-         firstlineno 258
+         firstlineno 222
          lnotab 0x02010e023e013401200248014201340120013e0234012202
       'event_id'
       code
          argcount  : 1
          nlocals   : 9
          stacksize : 9
          flags     : 3
@@ -1452,706 +1553,742 @@
             04a6010000ab01000000000000000001007415000000000000000000007c
             027c03ac0aa6020000ab0200000000000000000100640053007c016a0700
             0000000000000064106b02000000007202640053007c016a070000000000
             00000064116b020000000072127411000000000000000000007c01ac04a6
             010000ab0100000000000000000100640053007c016a0700000000000000
             0064126b020000000072127417000000000000000000007c01ac04a60100
             00ab0100000000000000000100640053007c016a07000000000000000064
-            136b020000000072137419000000000000000000007c027c01ac14a60200
-            00ab0200000000000000000100640053007c016a07000000000000000064
-            156b02000000007213741b000000000000000000007c027c01ac14a60200
-            00ab0200000000000000000100640053007c016a07000000000000000064
-            166b02000000007213741b000000000000000000007c027c01ac14a60200
-            00ab0200000000000000000100640053007c016a07000000000000000064
-            176b020000000072227402000000000000000000006a0200000000000000
-            00a00e00000000000000000000000000000000000000007c01ac04a60100
-            00ab0100000000000000000100640053007c016a07000000000000000064
-            186b020000000072597c016a0f0000000000000000641919000000000000
-            00000044005d497d047402000000000000000000006a0200000000000000
-            00a01000000000000000000000000000000000000000007c04ac1aa60100
-            00ab0100000000000000007d057402000000000000000000006a02000000
-            0000000000a01100000000000000000000000000000000000000007c057c
-            027c016a120000000000000000ac1ba6030000ab03000000000000000001
-            008c4a640053007c016a070000000000000000641c6b0200000000723674
-            0100000000000000000000641da6010000ab010000000000000000010074
+            136b020000000072397419000000000000000000007c016a0d0000000000
+            000000641419000000000000000000641519000000000000000000a60100
+            00ab01000000000000000064166b04000000007213741d00000000000000
+            0000007c027c01ac17a6020000ab02000000000000000001006400530064
+            0053007c016a07000000000000000064186b02000000007213741f000000
+            000000000000007c027c01ac17a6020000ab020000000000000000010064
+            0053007c016a07000000000000000064196b020000000072137421000000
+            000000000000007c027c01ac17a6020000ab020000000000000000010064
+            0053007c016a070000000000000000641a6b020000000072137421000000
+            000000000000007c027c01ac17a6020000ab020000000000000000010064
+            0053007c016a070000000000000000641b6b020000000072227402000000
+            000000000000006a020000000000000000a0110000000000000000000000
+            0000000000000000007c01ac04a6010000ab010000000000000000010064
+            0053007c016a070000000000000000641c6b020000000072597c016a0d00
+            00000000000000641d1900000000000000000044005d497d047402000000
+            000000000000006a020000000000000000a0120000000000000000000000
+            0000000000000000007c04ac1ea6010000ab0100000000000000007d0574
             02000000000000000000006a020000000000000000a01300000000000000
-            000000000000000000000000007c026a140000000000000000ac1ea60100
-            00ab0100000000000000000100640053007c016a07000000000000000064
-            1f6b02000000009001721f7401000000000000000000007c01a6010000ab
-            01000000000000000001007c016a0f0000000000000000641f1900000000
-            00000000007d067c016a0f00000000000000006420190000000000000000
-            007d077c0664216b0200000000724c7402000000000000000000006a0200
-            00000000000000a015000000000000000000000000000000000000000074
-            02000000000000000000006a160000000000000000a01700000000000000
-            000000000000000000000000007c026a140000000000000000640d7c037c
-            016a120000000000000000ac22a6040000ab040000000000000000a60100
-            00ab0100000000000000000100640053007c0664236b0200000000724c74
-            02000000000000000000006a020000000000000000a01500000000000000
-            000000000000000000000000007402000000000000000000006a16000000
-            0000000000a01700000000000000000000000000000000000000007c026a
-            14000000000000000064247c037c016a120000000000000000ac22a60400
-            00ab040000000000000000a6010000ab0100000000000000000100640053
-            007c0764257600724c7402000000000000000000006a0200000000000000
-            00a015000000000000000000000000000000000000000074020000000000
-            00000000006a160000000000000000a01700000000000000000000000000
-            000000000000007c026a14000000000000000064087c037c016a12000000
-            0000000000ac22a6040000ab040000000000000000a6010000ab01000000
-            0000000000010064005300640053007c016a07000000000000000064266b
-            020000000072b97c0372817402000000000000000000006a020000000000
-            000000a01800000000000000000000000000000000000000007c03a60100
-            00ab0100000000000000007d087c016a0f0000000000000000a019000000
-            00000000000000000000000000000000006427a6010000ab010000000000
-            00000072127c016a0f00000000000000006427190000000000000000007c
-            085f1a000000000000000069007c086a1b0000000000000000a5017c016a
-            0f0000000000000000a5017c085f1b000000000000000074020000000000
-            00000000006a020000000000000000a01c00000000000000000000000000
-            000000000000007c08a6010000ab01000000000000000001006400530069
-            007c026a1b0000000000000000a5017c016a0f0000000000000000a5017c
-            025f1b00000000000000007402000000000000000000006a020000000000
-            000000a01d00000000000000000000000000000000000000007c02a60100
-            00ab0100000000000000000100640053007c016a07000000000000000064
-            286b020000000072757c016a0f0000000000000000642919000000000000
-            00000044005d697d03740100000000000000000000642a7c03a6020000ab
-            02000000000000000001007402000000000000000000006a020000000000
-            000000a01500000000000000000000000000000000000000007402000000
-            000000000000006a160000000000000000a0170000000000000000000000
-            0000000000000000007c026a1400000000000000007c037c016a0f000000
-            0000000000642b190000000000000000007c016a120000000000000000ac
-            2ca6040000ab040000000000000000a6010000ab01000000000000000001
-            008c686400530064005300
-         277           0 RESUME                   0
+            000000000000000000000000007c057c027c016a140000000000000000ac
+            1fa6030000ab03000000000000000001008c4a640053007c016a07000000
+            000000000064206b020000000072367401000000000000000000006421a6
+            010000ab01000000000000000001007402000000000000000000006a0200
+            00000000000000a01500000000000000000000000000000000000000007c
+            026a160000000000000000ac22a6010000ab010000000000000000010064
+            0053007c016a07000000000000000064236b02000000009001721f740100
+            0000000000000000007c01a6010000ab01000000000000000001007c016a
+            0d00000000000000006423190000000000000000007d067c016a0d000000
+            00000000006424190000000000000000007d077c0664256b020000000072
+            4c7402000000000000000000006a020000000000000000a0170000000000
+            0000000000000000000000000000007402000000000000000000006a1800
+            00000000000000a01900000000000000000000000000000000000000007c
+            026a160000000000000000640d7c037c016a140000000000000000ac26a6
+            040000ab040000000000000000a6010000ab010000000000000000010064
+            0053007c0664276b0200000000724c7402000000000000000000006a0200
+            00000000000000a017000000000000000000000000000000000000000074
+            02000000000000000000006a180000000000000000a01900000000000000
+            000000000000000000000000007c026a16000000000000000064287c037c
+            016a140000000000000000ac26a6040000ab040000000000000000a60100
+            00ab0100000000000000000100640053007c0764297600724c7402000000
+            000000000000006a020000000000000000a0170000000000000000000000
+            0000000000000000007402000000000000000000006a1800000000000000
+            00a01900000000000000000000000000000000000000007c026a16000000
+            000000000064087c037c016a140000000000000000ac26a6040000ab0400
+            00000000000000a6010000ab010000000000000000010064005300640053
+            007c016a070000000000000000642a6b020000000072b97c037281740200
+            0000000000000000006a020000000000000000a01a000000000000000000
+            00000000000000000000007c03a6010000ab0100000000000000007d087c
+            016a0d0000000000000000a01b0000000000000000000000000000000000
+            000000642ba6010000ab01000000000000000072127c016a0d0000000000
+            000000642b190000000000000000007c085f1c000000000000000069007c
+            086a1d0000000000000000a5017c016a0d0000000000000000a5017c085f
+            1d00000000000000007402000000000000000000006a0200000000000000
+            00a01e00000000000000000000000000000000000000007c08a6010000ab
+            01000000000000000001006400530069007c026a1d0000000000000000a5
+            017c016a0d0000000000000000a5017c025f1d0000000000000000740200
+            0000000000000000006a020000000000000000a01f000000000000000000
+            00000000000000000000007c02a6010000ab010000000000000000010064
+            0053007c016a070000000000000000642c6b020000000072757c016a0d00
+            00000000000000642d1900000000000000000044005d697d037401000000
+            00000000000000642e7c03a6020000ab0200000000000000000100740200
+            0000000000000000006a020000000000000000a017000000000000000000
+            00000000000000000000007402000000000000000000006a180000000000
+            000000a01900000000000000000000000000000000000000007c026a1600
+            000000000000007c037c016a0d0000000000000000642f19000000000000
+            0000007c016a140000000000000000ac30a6040000ab0400000000000000
+            00a6010000ab01000000000000000001008c686400530064005300
+         241           0 RESUME                   0
          
-         278           2 LOAD_GLOBAL              1 (NULL + print)
+         242           2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_CONST               1 ('processing event_id: ')
                       16 LOAD_FAST                0 (event_id)
                       18 PRECALL                  2
                       22 CALL                     2
                       32 POP_TOP
          
-         279          34 LOAD_GLOBAL              2 (ts)
+         243          34 LOAD_GLOBAL              2 (ts)
                       46 LOAD_ATTR                2 (query)
                       56 LOAD_METHOD              3 (find_event_by_id)
                       78 LOAD_FAST                0 (event_id)
                       80 PRECALL                  1
                       84 CALL                     1
                       94 STORE_FAST               1 (event)
          
-         280          96 LOAD_GLOBAL              1 (NULL + print)
+         244          96 LOAD_GLOBAL              1 (NULL + print)
                      108 LOAD_FAST                1 (event)
                      110 PRECALL                  1
                      114 CALL                     1
                      124 POP_TOP
          
-         281         126 LOAD_GLOBAL              2 (ts)
+         245         126 LOAD_GLOBAL              2 (ts)
                      138 LOAD_ATTR                2 (query)
                      148 LOAD_METHOD              4 (find_search)
                      170 LOAD_FAST                1 (event)
                      172 LOAD_ATTR                5 (search_uid)
                      182 KW_NAMES                 2
                      184 PRECALL                  1
                      188 CALL                     1
                      198 STORE_FAST               2 (search)
          
-         282         200 LOAD_FAST                1 (event)
+         246         200 LOAD_FAST                1 (event)
                      202 LOAD_ATTR                6 (domain)
                      212 STORE_FAST               3 (domain)
          
-         283         214 LOAD_FAST                1 (event)
+         247         214 LOAD_FAST                1 (event)
                      216 LOAD_ATTR                7 (type)
                      226 LOAD_CONST               3 ('land')
                      228 COMPARE_OP               2 (==)
                      234 POP_JUMP_FORWARD_IF_FALSE    18 (to 272)
          
-         284         236 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         248         236 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      248 LOAD_FAST                1 (event)
                      250 KW_NAMES                 4
                      252 PRECALL                  1
                      256 CALL                     1
                      266 POP_TOP
                      268 LOAD_CONST               0 (None)
                      270 RETURN_VALUE
          
-         285     >>  272 LOAD_FAST                1 (event)
+         249     >>  272 LOAD_FAST                1 (event)
                      274 LOAD_ATTR                7 (type)
                      284 LOAD_CONST               5 ('create')
                      286 COMPARE_OP               2 (==)
                      292 POP_JUMP_FORWARD_IF_FALSE    18 (to 330)
          
-         286         294 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         250         294 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      306 LOAD_FAST                1 (event)
                      308 KW_NAMES                 4
                      310 PRECALL                  1
                      314 CALL                     1
                      324 POP_TOP
                      326 LOAD_CONST               0 (None)
                      328 RETURN_VALUE
          
-         287     >>  330 LOAD_FAST                1 (event)
+         251     >>  330 LOAD_FAST                1 (event)
                      332 LOAD_ATTR                7 (type)
                      342 LOAD_CONST               6 ('similar')
                      344 COMPARE_OP               2 (==)
                      350 POP_JUMP_FORWARD_IF_FALSE    18 (to 388)
          
-         288         352 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         252         352 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      364 LOAD_FAST                1 (event)
                      366 KW_NAMES                 4
                      368 PRECALL                  1
                      372 CALL                     1
                      382 POP_TOP
                      384 LOAD_CONST               0 (None)
                      386 RETURN_VALUE
          
-         289     >>  388 LOAD_FAST                1 (event)
+         253     >>  388 LOAD_FAST                1 (event)
                      390 LOAD_ATTR                7 (type)
                      400 LOAD_CONST               7 ('advance')
                      402 COMPARE_OP               2 (==)
                      408 POP_JUMP_FORWARD_IF_FALSE    18 (to 446)
          
-         290         410 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         254         410 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      422 LOAD_FAST                1 (event)
                      424 KW_NAMES                 4
                      426 PRECALL                  1
                      430 CALL                     1
                      440 POP_TOP
                      442 LOAD_CONST               0 (None)
                      444 RETURN_VALUE
          
-         291     >>  446 LOAD_FAST                1 (event)
+         255     >>  446 LOAD_FAST                1 (event)
                      448 LOAD_ATTR                7 (type)
                      458 LOAD_CONST               8 ('validate')
                      460 COMPARE_OP               2 (==)
                      466 POP_JUMP_FORWARD_IF_FALSE    51 (to 570)
          
-         292         468 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         256         468 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      480 LOAD_FAST                1 (event)
                      482 KW_NAMES                 4
                      484 PRECALL                  1
                      488 CALL                     1
                      498 POP_TOP
          
-         293         500 LOAD_GLOBAL             19 (NULL + run_acquired_check)
+         257         500 LOAD_GLOBAL             19 (NULL + run_acquired_check)
                      512 LOAD_FAST                3 (domain)
                      514 KW_NAMES                 9
                      516 PRECALL                  1
                      520 CALL                     1
                      530 POP_TOP
          
-         294         532 LOAD_GLOBAL             21 (NULL + run_similarity_search)
+         258         532 LOAD_GLOBAL             21 (NULL + run_similarity_search)
                      544 LOAD_FAST                2 (search)
                      546 LOAD_FAST                3 (domain)
                      548 KW_NAMES                10
                      550 PRECALL                  2
                      554 CALL                     2
                      564 POP_TOP
                      566 LOAD_CONST               0 (None)
                      568 RETURN_VALUE
          
-         295     >>  570 LOAD_FAST                1 (event)
+         259     >>  570 LOAD_FAST                1 (event)
                      572 LOAD_ATTR                7 (type)
                      582 LOAD_CONST              11 ('send')
                      584 COMPARE_OP               2 (==)
                      590 POP_JUMP_FORWARD_IF_FALSE    18 (to 628)
          
-         296         592 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         260         592 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      604 LOAD_FAST                1 (event)
                      606 KW_NAMES                 4
                      608 PRECALL                  1
                      612 CALL                     1
                      622 POP_TOP
                      624 LOAD_CONST               0 (None)
                      626 RETURN_VALUE
          
-         297     >>  628 LOAD_FAST                1 (event)
+         261     >>  628 LOAD_FAST                1 (event)
                      630 LOAD_ATTR                7 (type)
                      640 LOAD_CONST              12 ('client_approve')
                      642 COMPARE_OP               2 (==)
                      648 POP_JUMP_FORWARD_IF_FALSE    35 (to 720)
          
-         298         650 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         262         650 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      662 LOAD_FAST                1 (event)
                      664 KW_NAMES                 4
                      666 PRECALL                  1
                      670 CALL                     1
                      680 POP_TOP
          
-         299         682 LOAD_GLOBAL             21 (NULL + run_similarity_search)
+         263         682 LOAD_GLOBAL             21 (NULL + run_similarity_search)
                      694 LOAD_FAST                2 (search)
                      696 LOAD_FAST                3 (domain)
                      698 KW_NAMES                10
                      700 PRECALL                  2
                      704 CALL                     2
                      714 POP_TOP
                      716 LOAD_CONST               0 (None)
                      718 RETURN_VALUE
          
-         300     >>  720 LOAD_FAST                1 (event)
+         264     >>  720 LOAD_FAST                1 (event)
                      722 LOAD_ATTR                7 (type)
                      732 LOAD_CONST              13 ('reject')
                      734 COMPARE_OP               2 (==)
                      740 POP_JUMP_FORWARD_IF_FALSE     2 (to 746)
          
-         301         742 LOAD_CONST               0 (None)
+         265         742 LOAD_CONST               0 (None)
                      744 RETURN_VALUE
          
-         302     >>  746 LOAD_FAST                1 (event)
+         266     >>  746 LOAD_FAST                1 (event)
                      748 LOAD_ATTR                7 (type)
                      758 LOAD_CONST              14 ('client_reject')
                      760 COMPARE_OP               2 (==)
                      766 POP_JUMP_FORWARD_IF_FALSE     2 (to 772)
          
-         303         768 LOAD_CONST               0 (None)
+         267         768 LOAD_CONST               0 (None)
                      770 RETURN_VALUE
          
-         304     >>  772 LOAD_FAST                1 (event)
+         268     >>  772 LOAD_FAST                1 (event)
                      774 LOAD_ATTR                7 (type)
                      784 LOAD_CONST              15 ('conflict')
                      786 COMPARE_OP               2 (==)
                      792 POP_JUMP_FORWARD_IF_FALSE    35 (to 864)
          
-         305         794 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         269         794 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      806 LOAD_FAST                1 (event)
                      808 KW_NAMES                 4
                      810 PRECALL                  1
                      814 CALL                     1
                      824 POP_TOP
          
-         306         826 LOAD_GLOBAL             21 (NULL + run_similarity_search)
+         270         826 LOAD_GLOBAL             21 (NULL + run_similarity_search)
                      838 LOAD_FAST                2 (search)
                      840 LOAD_FAST                3 (domain)
                      842 KW_NAMES                10
                      844 PRECALL                  2
                      848 CALL                     2
                      858 POP_TOP
                      860 LOAD_CONST               0 (None)
                      862 RETURN_VALUE
          
-         307     >>  864 LOAD_FAST                1 (event)
+         271     >>  864 LOAD_FAST                1 (event)
                      866 LOAD_ATTR                7 (type)
                      876 LOAD_CONST              16 ('client_conflict')
                      878 COMPARE_OP               2 (==)
                      884 POP_JUMP_FORWARD_IF_FALSE     2 (to 890)
          
-         308         886 LOAD_CONST               0 (None)
+         272         886 LOAD_CONST               0 (None)
                      888 RETURN_VALUE
          
-         310     >>  890 LOAD_FAST                1 (event)
+         274     >>  890 LOAD_FAST                1 (event)
                      892 LOAD_ATTR                7 (type)
                      902 LOAD_CONST              17 ('enrich')
                      904 COMPARE_OP               2 (==)
                      910 POP_JUMP_FORWARD_IF_FALSE    18 (to 948)
          
-         311         912 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         275         912 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      924 LOAD_FAST                1 (event)
                      926 KW_NAMES                 4
                      928 PRECALL                  1
                      932 CALL                     1
                      942 POP_TOP
                      944 LOAD_CONST               0 (None)
                      946 RETURN_VALUE
          
-         313     >>  948 LOAD_FAST                1 (event)
+         277     >>  948 LOAD_FAST                1 (event)
                      950 LOAD_ATTR                7 (type)
                      960 LOAD_CONST              18 ('prompt')
                      962 COMPARE_OP               2 (==)
                      968 POP_JUMP_FORWARD_IF_FALSE    18 (to 1006)
          
-         314         970 LOAD_GLOBAL             23 (NULL + handle_prompt)
+         278         970 LOAD_GLOBAL             23 (NULL + handle_prompt)
                      982 LOAD_FAST                1 (event)
                      984 KW_NAMES                 4
                      986 PRECALL                  1
                      990 CALL                     1
                     1000 POP_TOP
                     1002 LOAD_CONST               0 (None)
                     1004 RETURN_VALUE
          
-         318     >> 1006 LOAD_FAST                1 (event)
+         279     >> 1006 LOAD_FAST                1 (event)
                     1008 LOAD_ATTR                7 (type)
-                    1018 LOAD_CONST              19 ('maps')
+                    1018 LOAD_CONST              19 ('criteria')
                     1020 COMPARE_OP               2 (==)
-                    1026 POP_JUMP_FORWARD_IF_FALSE    19 (to 1066)
+                    1026 POP_JUMP_FORWARD_IF_FALSE    57 (to 1142)
          
-         319        1028 LOAD_GLOBAL             25 (NULL + run_maps_search)
-                    1040 LOAD_FAST                2 (search)
-                    1042 LOAD_FAST                1 (event)
-                    1044 KW_NAMES                20
-                    1046 PRECALL                  2
-                    1050 CALL                     2
-                    1060 POP_TOP
-                    1062 LOAD_CONST               0 (None)
-                    1064 RETURN_VALUE
-         
-         320     >> 1066 LOAD_FAST                1 (event)
-                    1068 LOAD_ATTR                7 (type)
-                    1078 LOAD_CONST              21 ('google')
-                    1080 COMPARE_OP               2 (==)
-                    1086 POP_JUMP_FORWARD_IF_FALSE    19 (to 1126)
-         
-         321        1088 LOAD_GLOBAL             27 (NULL + run_google_search)
-                    1100 LOAD_FAST                2 (search)
-                    1102 LOAD_FAST                1 (event)
-                    1104 KW_NAMES                20
-                    1106 PRECALL                  2
-                    1110 CALL                     2
-                    1120 POP_TOP
-                    1122 LOAD_CONST               0 (None)
-                    1124 RETURN_VALUE
-         
-         323     >> 1126 LOAD_FAST                1 (event)
-                    1128 LOAD_ATTR                7 (type)
-                    1138 LOAD_CONST              22 ('grata_search')
-                    1140 COMPARE_OP               2 (==)
-                    1146 POP_JUMP_FORWARD_IF_FALSE    19 (to 1186)
-         
-         324        1148 LOAD_GLOBAL             27 (NULL + run_google_search)
-                    1160 LOAD_FAST                2 (search)
-                    1162 LOAD_FAST                1 (event)
-                    1164 KW_NAMES                20
-                    1166 PRECALL                  2
-                    1170 CALL                     2
-                    1180 POP_TOP
-                    1182 LOAD_CONST               0 (None)
-                    1184 RETURN_VALUE
-         
-         326     >> 1186 LOAD_FAST                1 (event)
-                    1188 LOAD_ATTR                7 (type)
-                    1198 LOAD_CONST              23 ('import')
-                    1200 COMPARE_OP               2 (==)
-                    1206 POP_JUMP_FORWARD_IF_FALSE    34 (to 1276)
-         
-         327        1208 LOAD_GLOBAL              2 (ts)
-                    1220 LOAD_ATTR                2 (query)
-                    1230 LOAD_METHOD             14 (important_targets_from_event)
-                    1252 LOAD_FAST                1 (event)
-                    1254 KW_NAMES                 4
-                    1256 PRECALL                  1
-                    1260 CALL                     1
-                    1270 POP_TOP
-                    1272 LOAD_CONST               0 (None)
-                    1274 RETURN_VALUE
-         
-         329     >> 1276 LOAD_FAST                1 (event)
-                    1278 LOAD_ATTR                7 (type)
-                    1288 LOAD_CONST              24 ('import_searches')
-                    1290 COMPARE_OP               2 (==)
-                    1296 POP_JUMP_FORWARD_IF_FALSE    89 (to 1476)
-         
-         330        1298 LOAD_FAST                1 (event)
-                    1300 LOAD_ATTR               15 (data)
-                    1310 LOAD_CONST              25 ('searches')
-                    1312 BINARY_SUBSCR
-                    1322 GET_ITER
-                 >> 1324 FOR_ITER                73 (to 1472)
-                    1326 STORE_FAST               4 (label)
-         
-         331        1328 LOAD_GLOBAL              2 (ts)
-                    1340 LOAD_ATTR                2 (query)
-                    1350 LOAD_METHOD             16 (find_search_by_label)
-                    1372 LOAD_FAST                4 (label)
-                    1374 KW_NAMES                26
-                    1376 PRECALL                  1
-                    1380 CALL                     1
-                    1390 STORE_FAST               5 (from_search)
-         
-         332        1392 LOAD_GLOBAL              2 (ts)
-                    1404 LOAD_ATTR                2 (query)
-                    1414 LOAD_METHOD             17 (important_targets_from_search)
-         
-         333        1436 LOAD_FAST                5 (from_search)
-                    1438 LOAD_FAST                2 (search)
-                    1440 LOAD_FAST                1 (event)
-                    1442 LOAD_ATTR               18 (actor_key)
-         
-         332        1452 KW_NAMES                27
-                    1454 PRECALL                  3
-                    1458 CALL                     3
-                    1468 POP_TOP
-                    1470 JUMP_BACKWARD           74 (to 1324)
-         
-         330     >> 1472 LOAD_CONST               0 (None)
-                    1474 RETURN_VALUE
-         
-         336     >> 1476 LOAD_FAST                1 (event)
-                    1478 LOAD_ATTR                7 (type)
-                    1488 LOAD_CONST              28 ('reset')
-                    1490 COMPARE_OP               2 (==)
-                    1496 POP_JUMP_FORWARD_IF_FALSE    54 (to 1606)
-         
-         337        1498 LOAD_GLOBAL              1 (NULL + print)
-                    1510 LOAD_CONST              29 ('💣 Resetting Inbox...')
+         280        1028 LOAD_GLOBAL             25 (NULL + len)
+                    1040 LOAD_FAST                1 (event)
+                    1042 LOAD_ATTR               13 (data)
+                    1052 LOAD_CONST              20 ('inclusion')
+                    1054 BINARY_SUBSCR
+                    1064 LOAD_CONST              21 ('keywords')
+                    1066 BINARY_SUBSCR
+                    1076 PRECALL                  1
+                    1080 CALL                     1
+                    1090 LOAD_CONST              22 (0)
+                    1092 COMPARE_OP               4 (>)
+                    1098 POP_JUMP_FORWARD_IF_FALSE    19 (to 1138)
+         
+         281        1100 LOAD_GLOBAL             29 (NULL + run_criteria_search)
+                    1112 LOAD_FAST                2 (search)
+                    1114 LOAD_FAST                1 (event)
+                    1116 KW_NAMES                23
+                    1118 PRECALL                  2
+                    1122 CALL                     2
+                    1132 POP_TOP
+                    1134 LOAD_CONST               0 (None)
+                    1136 RETURN_VALUE
+         
+         280     >> 1138 LOAD_CONST               0 (None)
+                    1140 RETURN_VALUE
+         
+         282     >> 1142 LOAD_FAST                1 (event)
+                    1144 LOAD_ATTR                7 (type)
+                    1154 LOAD_CONST              24 ('maps')
+                    1156 COMPARE_OP               2 (==)
+                    1162 POP_JUMP_FORWARD_IF_FALSE    19 (to 1202)
+         
+         283        1164 LOAD_GLOBAL             31 (NULL + run_maps_search)
+                    1176 LOAD_FAST                2 (search)
+                    1178 LOAD_FAST                1 (event)
+                    1180 KW_NAMES                23
+                    1182 PRECALL                  2
+                    1186 CALL                     2
+                    1196 POP_TOP
+                    1198 LOAD_CONST               0 (None)
+                    1200 RETURN_VALUE
+         
+         284     >> 1202 LOAD_FAST                1 (event)
+                    1204 LOAD_ATTR                7 (type)
+                    1214 LOAD_CONST              25 ('google')
+                    1216 COMPARE_OP               2 (==)
+                    1222 POP_JUMP_FORWARD_IF_FALSE    19 (to 1262)
+         
+         285        1224 LOAD_GLOBAL             33 (NULL + run_google_search)
+                    1236 LOAD_FAST                2 (search)
+                    1238 LOAD_FAST                1 (event)
+                    1240 KW_NAMES                23
+                    1242 PRECALL                  2
+                    1246 CALL                     2
+                    1256 POP_TOP
+                    1258 LOAD_CONST               0 (None)
+                    1260 RETURN_VALUE
+         
+         287     >> 1262 LOAD_FAST                1 (event)
+                    1264 LOAD_ATTR                7 (type)
+                    1274 LOAD_CONST              26 ('grata_search')
+                    1276 COMPARE_OP               2 (==)
+                    1282 POP_JUMP_FORWARD_IF_FALSE    19 (to 1322)
+         
+         288        1284 LOAD_GLOBAL             33 (NULL + run_google_search)
+                    1296 LOAD_FAST                2 (search)
+                    1298 LOAD_FAST                1 (event)
+                    1300 KW_NAMES                23
+                    1302 PRECALL                  2
+                    1306 CALL                     2
+                    1316 POP_TOP
+                    1318 LOAD_CONST               0 (None)
+                    1320 RETURN_VALUE
+         
+         290     >> 1322 LOAD_FAST                1 (event)
+                    1324 LOAD_ATTR                7 (type)
+                    1334 LOAD_CONST              27 ('import')
+                    1336 COMPARE_OP               2 (==)
+                    1342 POP_JUMP_FORWARD_IF_FALSE    34 (to 1412)
+         
+         291        1344 LOAD_GLOBAL              2 (ts)
+                    1356 LOAD_ATTR                2 (query)
+                    1366 LOAD_METHOD             17 (important_targets_from_event)
+                    1388 LOAD_FAST                1 (event)
+                    1390 KW_NAMES                 4
+                    1392 PRECALL                  1
+                    1396 CALL                     1
+                    1406 POP_TOP
+                    1408 LOAD_CONST               0 (None)
+                    1410 RETURN_VALUE
+         
+         293     >> 1412 LOAD_FAST                1 (event)
+                    1414 LOAD_ATTR                7 (type)
+                    1424 LOAD_CONST              28 ('import_searches')
+                    1426 COMPARE_OP               2 (==)
+                    1432 POP_JUMP_FORWARD_IF_FALSE    89 (to 1612)
+         
+         294        1434 LOAD_FAST                1 (event)
+                    1436 LOAD_ATTR               13 (data)
+                    1446 LOAD_CONST              29 ('searches')
+                    1448 BINARY_SUBSCR
+                    1458 GET_ITER
+                 >> 1460 FOR_ITER                73 (to 1608)
+                    1462 STORE_FAST               4 (label)
+         
+         295        1464 LOAD_GLOBAL              2 (ts)
+                    1476 LOAD_ATTR                2 (query)
+                    1486 LOAD_METHOD             18 (find_search_by_label)
+                    1508 LOAD_FAST                4 (label)
+                    1510 KW_NAMES                30
                     1512 PRECALL                  1
                     1516 CALL                     1
-                    1526 POP_TOP
+                    1526 STORE_FAST               5 (from_search)
          
-         338        1528 LOAD_GLOBAL              2 (ts)
+         296        1528 LOAD_GLOBAL              2 (ts)
                     1540 LOAD_ATTR                2 (query)
-                    1550 LOAD_METHOD             19 (reset_inbox)
-                    1572 LOAD_FAST                2 (search)
-                    1574 LOAD_ATTR               20 (uid)
-                    1584 KW_NAMES                30
-                    1586 PRECALL                  1
-                    1590 CALL                     1
-                    1600 POP_TOP
-                    1602 LOAD_CONST               0 (None)
-                    1604 RETURN_VALUE
-         
-         340     >> 1606 LOAD_FAST                1 (event)
-                    1608 LOAD_ATTR                7 (type)
-                    1618 LOAD_CONST              31 ('rating')
-                    1620 COMPARE_OP               2 (==)
-                    1626 EXTENDED_ARG             1
-                    1628 POP_JUMP_FORWARD_IF_FALSE   287 (to 2204)
-         
-         342        1630 LOAD_GLOBAL              1 (NULL + print)
-                    1642 LOAD_FAST                1 (event)
-                    1644 PRECALL                  1
-                    1648 CALL                     1
-                    1658 POP_TOP
-         
-         343        1660 LOAD_FAST                1 (event)
-                    1662 LOAD_ATTR               15 (data)
-                    1672 LOAD_CONST              31 ('rating')
-                    1674 BINARY_SUBSCR
-                    1684 STORE_FAST               6 (rating)
-         
-         344        1686 LOAD_FAST                1 (event)
-                    1688 LOAD_ATTR               15 (data)
-                    1698 LOAD_CONST              32 ('currentView')
-                    1700 BINARY_SUBSCR
-                    1710 STORE_FAST               7 (from_stage)
-         
-         345        1712 LOAD_FAST                6 (rating)
-                    1714 LOAD_CONST              33 (1)
-                    1716 COMPARE_OP               2 (==)
-                    1722 POP_JUMP_FORWARD_IF_FALSE    76 (to 1876)
-         
-         346        1724 LOAD_GLOBAL              2 (ts)
-                    1736 LOAD_ATTR                2 (query)
-                    1746 LOAD_METHOD             21 (insert_event)
-         
-         347        1768 LOAD_GLOBAL              2 (ts)
-                    1780 LOAD_ATTR               22 (models)
-                    1790 LOAD_METHOD             23 (Event)
-         
-         348        1812 LOAD_FAST                2 (search)
-                    1814 LOAD_ATTR               20 (uid)
-         
-         349        1824 LOAD_CONST              13 ('reject')
-         
-         350        1826 LOAD_FAST                3 (domain)
-         
-         351        1828 LOAD_FAST                1 (event)
-                    1830 LOAD_ATTR               18 (actor_key)
-         
-         347        1840 KW_NAMES                34
-                    1842 PRECALL                  4
-                    1846 CALL                     4
-         
-         346        1856 PRECALL                  1
-                    1860 CALL                     1
-                    1870 POP_TOP
-                    1872 LOAD_CONST               0 (None)
-                    1874 RETURN_VALUE
-         
-         354     >> 1876 LOAD_FAST                6 (rating)
-                    1878 LOAD_CONST              35 (2)
-                    1880 COMPARE_OP               2 (==)
-                    1886 POP_JUMP_FORWARD_IF_FALSE    76 (to 2040)
-         
-         355        1888 LOAD_GLOBAL              2 (ts)
-                    1900 LOAD_ATTR                2 (query)
-                    1910 LOAD_METHOD             21 (insert_event)
-         
-         356        1932 LOAD_GLOBAL              2 (ts)
-                    1944 LOAD_ATTR               22 (models)
-                    1954 LOAD_METHOD             23 (Event)
-         
-         357        1976 LOAD_FAST                2 (search)
-                    1978 LOAD_ATTR               20 (uid)
-         
-         358        1988 LOAD_CONST              36 ('hold')
-         
-         359        1990 LOAD_FAST                3 (domain)
-         
-         360        1992 LOAD_FAST                1 (event)
-                    1994 LOAD_ATTR               18 (actor_key)
-         
-         356        2004 KW_NAMES                34
-                    2006 PRECALL                  4
-                    2010 CALL                     4
-         
-         355        2020 PRECALL                  1
-                    2024 CALL                     1
-                    2034 POP_TOP
-                    2036 LOAD_CONST               0 (None)
-                    2038 RETURN_VALUE
-         
-         363     >> 2040 LOAD_FAST                7 (from_stage)
-                    2042 LOAD_CONST              37 (('land', 'create', 'advance', 'hold', 'similar'))
-                    2044 CONTAINS_OP              0
-                    2046 POP_JUMP_FORWARD_IF_FALSE    76 (to 2200)
-         
-         364        2048 LOAD_GLOBAL              2 (ts)
-                    2060 LOAD_ATTR                2 (query)
-                    2070 LOAD_METHOD             21 (insert_event)
-         
-         365        2092 LOAD_GLOBAL              2 (ts)
-                    2104 LOAD_ATTR               22 (models)
-                    2114 LOAD_METHOD             23 (Event)
-         
-         366        2136 LOAD_FAST                2 (search)
-                    2138 LOAD_ATTR               20 (uid)
-         
-         367        2148 LOAD_CONST               8 ('validate')
-         
-         368        2150 LOAD_FAST                3 (domain)
-         
-         369        2152 LOAD_FAST                1 (event)
-                    2154 LOAD_ATTR               18 (actor_key)
-         
-         365        2164 KW_NAMES                34
-                    2166 PRECALL                  4
-                    2170 CALL                     4
-         
-         364        2180 PRECALL                  1
-                    2184 CALL                     1
-                    2194 POP_TOP
-                    2196 LOAD_CONST               0 (None)
-                    2198 RETURN_VALUE
-         
-         363     >> 2200 LOAD_CONST               0 (None)
-                    2202 RETURN_VALUE
-         
-         373     >> 2204 LOAD_FAST                1 (event)
-                    2206 LOAD_ATTR                7 (type)
-                    2216 LOAD_CONST              38 ('update')
-                    2218 COMPARE_OP               2 (==)
-                    2224 POP_JUMP_FORWARD_IF_FALSE   185 (to 2596)
-         
-         374        2226 LOAD_FAST                3 (domain)
-                    2228 POP_JUMP_FORWARD_IF_FALSE   129 (to 2488)
-         
-         375        2230 LOAD_GLOBAL              2 (ts)
-                    2242 LOAD_ATTR                2 (query)
-                    2252 LOAD_METHOD             24 (find_company_by_domain)
-                    2274 LOAD_FAST                3 (domain)
-                    2276 PRECALL                  1
-                    2280 CALL                     1
-                    2290 STORE_FAST               8 (company)
-         
-         376        2292 LOAD_FAST                1 (event)
-                    2294 LOAD_ATTR               15 (data)
-                    2304 LOAD_METHOD             25 (get)
-                    2326 LOAD_CONST              39 ('name')
-                    2328 PRECALL                  1
-                    2332 CALL                     1
-                    2342 POP_JUMP_FORWARD_IF_FALSE    18 (to 2380)
-         
-         377        2344 LOAD_FAST                1 (event)
-                    2346 LOAD_ATTR               15 (data)
-                    2356 LOAD_CONST              39 ('name')
-                    2358 BINARY_SUBSCR
-                    2368 LOAD_FAST                8 (company)
-                    2370 STORE_ATTR              26 (name)
-         
-         378     >> 2380 BUILD_MAP                0
-                    2382 LOAD_FAST                8 (company)
-                    2384 LOAD_ATTR               27 (meta)
-                    2394 DICT_UPDATE              1
-                    2396 LOAD_FAST                1 (event)
-                    2398 LOAD_ATTR               15 (data)
-                    2408 DICT_UPDATE              1
-                    2410 LOAD_FAST                8 (company)
-                    2412 STORE_ATTR              27 (meta)
-         
-         379        2422 LOAD_GLOBAL              2 (ts)
-                    2434 LOAD_ATTR                2 (query)
-                    2444 LOAD_METHOD             28 (update_company)
-                    2466 LOAD_FAST                8 (company)
-                    2468 PRECALL                  1
-                    2472 CALL                     1
-                    2482 POP_TOP
-                    2484 LOAD_CONST               0 (None)
-                    2486 RETURN_VALUE
-         
-         381     >> 2488 BUILD_MAP                0
-                    2490 LOAD_FAST                2 (search)
-                    2492 LOAD_ATTR               27 (meta)
-                    2502 DICT_UPDATE              1
-                    2504 LOAD_FAST                1 (event)
-                    2506 LOAD_ATTR               15 (data)
-                    2516 DICT_UPDATE              1
-                    2518 LOAD_FAST                2 (search)
-                    2520 STORE_ATTR              27 (meta)
-         
-         382        2530 LOAD_GLOBAL              2 (ts)
-                    2542 LOAD_ATTR                2 (query)
-                    2552 LOAD_METHOD             29 (update_search)
-                    2574 LOAD_FAST                2 (search)
-                    2576 PRECALL                  1
-                    2580 CALL                     1
-                    2590 POP_TOP
-                    2592 LOAD_CONST               0 (None)
-                    2594 RETURN_VALUE
-         
-         384     >> 2596 LOAD_FAST                1 (event)
-                    2598 LOAD_ATTR                7 (type)
-                    2608 LOAD_CONST              40 ('move')
-                    2610 COMPARE_OP               2 (==)
-                    2616 POP_JUMP_FORWARD_IF_FALSE   117 (to 2852)
-         
-         386        2618 LOAD_FAST                1 (event)
-                    2620 LOAD_ATTR               15 (data)
-                    2630 LOAD_CONST              41 ('domains')
-                    2632 BINARY_SUBSCR
-                    2642 GET_ITER
-                 >> 2644 FOR_ITER               105 (to 2856)
-                    2646 STORE_FAST               3 (domain)
-         
-         387        2648 LOAD_GLOBAL              1 (NULL + print)
-                    2660 LOAD_CONST              42 ('moving domain:')
-                    2662 LOAD_FAST                3 (domain)
-                    2664 PRECALL                  2
-                    2668 CALL                     2
-                    2678 POP_TOP
-         
-         388        2680 LOAD_GLOBAL              2 (ts)
-                    2692 LOAD_ATTR                2 (query)
-                    2702 LOAD_METHOD             21 (insert_event)
-         
-         389        2724 LOAD_GLOBAL              2 (ts)
-                    2736 LOAD_ATTR               22 (models)
-                    2746 LOAD_METHOD             23 (Event)
-         
-         390        2768 LOAD_FAST                2 (search)
-                    2770 LOAD_ATTR               20 (uid)
-         
-         391        2780 LOAD_FAST                3 (domain)
-         
-         392        2782 LOAD_FAST                1 (event)
-                    2784 LOAD_ATTR               15 (data)
-                    2794 LOAD_CONST              43 ('stage')
-                    2796 BINARY_SUBSCR
-         
-         393        2806 LOAD_FAST                1 (event)
-                    2808 LOAD_ATTR               18 (actor_key)
-         
-         389        2818 KW_NAMES                44
-                    2820 PRECALL                  4
-                    2824 CALL                     4
-         
-         388        2834 PRECALL                  1
-                    2838 CALL                     1
-                    2848 POP_TOP
-                    2850 JUMP_BACKWARD          104 (to 2644)
+                    1550 LOAD_METHOD             19 (important_targets_from_search)
+         
+         297        1572 LOAD_FAST                5 (from_search)
+                    1574 LOAD_FAST                2 (search)
+                    1576 LOAD_FAST                1 (event)
+                    1578 LOAD_ATTR               20 (actor_key)
+         
+         296        1588 KW_NAMES                31
+                    1590 PRECALL                  3
+                    1594 CALL                     3
+                    1604 POP_TOP
+                    1606 JUMP_BACKWARD           74 (to 1460)
+         
+         294     >> 1608 LOAD_CONST               0 (None)
+                    1610 RETURN_VALUE
+         
+         300     >> 1612 LOAD_FAST                1 (event)
+                    1614 LOAD_ATTR                7 (type)
+                    1624 LOAD_CONST              32 ('reset')
+                    1626 COMPARE_OP               2 (==)
+                    1632 POP_JUMP_FORWARD_IF_FALSE    54 (to 1742)
+         
+         301        1634 LOAD_GLOBAL              1 (NULL + print)
+                    1646 LOAD_CONST              33 ('💣 Resetting Inbox...')
+                    1648 PRECALL                  1
+                    1652 CALL                     1
+                    1662 POP_TOP
+         
+         302        1664 LOAD_GLOBAL              2 (ts)
+                    1676 LOAD_ATTR                2 (query)
+                    1686 LOAD_METHOD             21 (reset_inbox)
+                    1708 LOAD_FAST                2 (search)
+                    1710 LOAD_ATTR               22 (uid)
+                    1720 KW_NAMES                34
+                    1722 PRECALL                  1
+                    1726 CALL                     1
+                    1736 POP_TOP
+                    1738 LOAD_CONST               0 (None)
+                    1740 RETURN_VALUE
+         
+         304     >> 1742 LOAD_FAST                1 (event)
+                    1744 LOAD_ATTR                7 (type)
+                    1754 LOAD_CONST              35 ('rating')
+                    1756 COMPARE_OP               2 (==)
+                    1762 EXTENDED_ARG             1
+                    1764 POP_JUMP_FORWARD_IF_FALSE   287 (to 2340)
+         
+         306        1766 LOAD_GLOBAL              1 (NULL + print)
+                    1778 LOAD_FAST                1 (event)
+                    1780 PRECALL                  1
+                    1784 CALL                     1
+                    1794 POP_TOP
+         
+         307        1796 LOAD_FAST                1 (event)
+                    1798 LOAD_ATTR               13 (data)
+                    1808 LOAD_CONST              35 ('rating')
+                    1810 BINARY_SUBSCR
+                    1820 STORE_FAST               6 (rating)
+         
+         308        1822 LOAD_FAST                1 (event)
+                    1824 LOAD_ATTR               13 (data)
+                    1834 LOAD_CONST              36 ('currentView')
+                    1836 BINARY_SUBSCR
+                    1846 STORE_FAST               7 (from_stage)
+         
+         309        1848 LOAD_FAST                6 (rating)
+                    1850 LOAD_CONST              37 (1)
+                    1852 COMPARE_OP               2 (==)
+                    1858 POP_JUMP_FORWARD_IF_FALSE    76 (to 2012)
+         
+         310        1860 LOAD_GLOBAL              2 (ts)
+                    1872 LOAD_ATTR                2 (query)
+                    1882 LOAD_METHOD             23 (insert_event)
+         
+         311        1904 LOAD_GLOBAL              2 (ts)
+                    1916 LOAD_ATTR               24 (models)
+                    1926 LOAD_METHOD             25 (Event)
+         
+         312        1948 LOAD_FAST                2 (search)
+                    1950 LOAD_ATTR               22 (uid)
+         
+         313        1960 LOAD_CONST              13 ('reject')
+         
+         314        1962 LOAD_FAST                3 (domain)
+         
+         315        1964 LOAD_FAST                1 (event)
+                    1966 LOAD_ATTR               20 (actor_key)
+         
+         311        1976 KW_NAMES                38
+                    1978 PRECALL                  4
+                    1982 CALL                     4
+         
+         310        1992 PRECALL                  1
+                    1996 CALL                     1
+                    2006 POP_TOP
+                    2008 LOAD_CONST               0 (None)
+                    2010 RETURN_VALUE
+         
+         318     >> 2012 LOAD_FAST                6 (rating)
+                    2014 LOAD_CONST              39 (2)
+                    2016 COMPARE_OP               2 (==)
+                    2022 POP_JUMP_FORWARD_IF_FALSE    76 (to 2176)
+         
+         319        2024 LOAD_GLOBAL              2 (ts)
+                    2036 LOAD_ATTR                2 (query)
+                    2046 LOAD_METHOD             23 (insert_event)
+         
+         320        2068 LOAD_GLOBAL              2 (ts)
+                    2080 LOAD_ATTR               24 (models)
+                    2090 LOAD_METHOD             25 (Event)
+         
+         321        2112 LOAD_FAST                2 (search)
+                    2114 LOAD_ATTR               22 (uid)
+         
+         322        2124 LOAD_CONST              40 ('hold')
+         
+         323        2126 LOAD_FAST                3 (domain)
+         
+         324        2128 LOAD_FAST                1 (event)
+                    2130 LOAD_ATTR               20 (actor_key)
+         
+         320        2140 KW_NAMES                38
+                    2142 PRECALL                  4
+                    2146 CALL                     4
+         
+         319        2156 PRECALL                  1
+                    2160 CALL                     1
+                    2170 POP_TOP
+                    2172 LOAD_CONST               0 (None)
+                    2174 RETURN_VALUE
+         
+         327     >> 2176 LOAD_FAST                7 (from_stage)
+                    2178 LOAD_CONST              41 (('land', 'create', 'advance', 'hold', 'similar'))
+                    2180 CONTAINS_OP              0
+                    2182 POP_JUMP_FORWARD_IF_FALSE    76 (to 2336)
+         
+         328        2184 LOAD_GLOBAL              2 (ts)
+                    2196 LOAD_ATTR                2 (query)
+                    2206 LOAD_METHOD             23 (insert_event)
+         
+         329        2228 LOAD_GLOBAL              2 (ts)
+                    2240 LOAD_ATTR               24 (models)
+                    2250 LOAD_METHOD             25 (Event)
+         
+         330        2272 LOAD_FAST                2 (search)
+                    2274 LOAD_ATTR               22 (uid)
+         
+         331        2284 LOAD_CONST               8 ('validate')
+         
+         332        2286 LOAD_FAST                3 (domain)
+         
+         333        2288 LOAD_FAST                1 (event)
+                    2290 LOAD_ATTR               20 (actor_key)
+         
+         329        2300 KW_NAMES                38
+                    2302 PRECALL                  4
+                    2306 CALL                     4
+         
+         328        2316 PRECALL                  1
+                    2320 CALL                     1
+                    2330 POP_TOP
+                    2332 LOAD_CONST               0 (None)
+                    2334 RETURN_VALUE
+         
+         327     >> 2336 LOAD_CONST               0 (None)
+                    2338 RETURN_VALUE
+         
+         337     >> 2340 LOAD_FAST                1 (event)
+                    2342 LOAD_ATTR                7 (type)
+                    2352 LOAD_CONST              42 ('update')
+                    2354 COMPARE_OP               2 (==)
+                    2360 POP_JUMP_FORWARD_IF_FALSE   185 (to 2732)
+         
+         338        2362 LOAD_FAST                3 (domain)
+                    2364 POP_JUMP_FORWARD_IF_FALSE   129 (to 2624)
+         
+         339        2366 LOAD_GLOBAL              2 (ts)
+                    2378 LOAD_ATTR                2 (query)
+                    2388 LOAD_METHOD             26 (find_company_by_domain)
+                    2410 LOAD_FAST                3 (domain)
+                    2412 PRECALL                  1
+                    2416 CALL                     1
+                    2426 STORE_FAST               8 (company)
+         
+         340        2428 LOAD_FAST                1 (event)
+                    2430 LOAD_ATTR               13 (data)
+                    2440 LOAD_METHOD             27 (get)
+                    2462 LOAD_CONST              43 ('name')
+                    2464 PRECALL                  1
+                    2468 CALL                     1
+                    2478 POP_JUMP_FORWARD_IF_FALSE    18 (to 2516)
+         
+         341        2480 LOAD_FAST                1 (event)
+                    2482 LOAD_ATTR               13 (data)
+                    2492 LOAD_CONST              43 ('name')
+                    2494 BINARY_SUBSCR
+                    2504 LOAD_FAST                8 (company)
+                    2506 STORE_ATTR              28 (name)
+         
+         342     >> 2516 BUILD_MAP                0
+                    2518 LOAD_FAST                8 (company)
+                    2520 LOAD_ATTR               29 (meta)
+                    2530 DICT_UPDATE              1
+                    2532 LOAD_FAST                1 (event)
+                    2534 LOAD_ATTR               13 (data)
+                    2544 DICT_UPDATE              1
+                    2546 LOAD_FAST                8 (company)
+                    2548 STORE_ATTR              29 (meta)
+         
+         343        2558 LOAD_GLOBAL              2 (ts)
+                    2570 LOAD_ATTR                2 (query)
+                    2580 LOAD_METHOD             30 (update_company)
+                    2602 LOAD_FAST                8 (company)
+                    2604 PRECALL                  1
+                    2608 CALL                     1
+                    2618 POP_TOP
+                    2620 LOAD_CONST               0 (None)
+                    2622 RETURN_VALUE
+         
+         345     >> 2624 BUILD_MAP                0
+                    2626 LOAD_FAST                2 (search)
+                    2628 LOAD_ATTR               29 (meta)
+                    2638 DICT_UPDATE              1
+                    2640 LOAD_FAST                1 (event)
+                    2642 LOAD_ATTR               13 (data)
+                    2652 DICT_UPDATE              1
+                    2654 LOAD_FAST                2 (search)
+                    2656 STORE_ATTR              29 (meta)
+         
+         346        2666 LOAD_GLOBAL              2 (ts)
+                    2678 LOAD_ATTR                2 (query)
+                    2688 LOAD_METHOD             31 (update_search)
+                    2710 LOAD_FAST                2 (search)
+                    2712 PRECALL                  1
+                    2716 CALL                     1
+                    2726 POP_TOP
+                    2728 LOAD_CONST               0 (None)
+                    2730 RETURN_VALUE
+         
+         348     >> 2732 LOAD_FAST                1 (event)
+                    2734 LOAD_ATTR                7 (type)
+                    2744 LOAD_CONST              44 ('move')
+                    2746 COMPARE_OP               2 (==)
+                    2752 POP_JUMP_FORWARD_IF_FALSE   117 (to 2988)
+         
+         350        2754 LOAD_FAST                1 (event)
+                    2756 LOAD_ATTR               13 (data)
+                    2766 LOAD_CONST              45 ('domains')
+                    2768 BINARY_SUBSCR
+                    2778 GET_ITER
+                 >> 2780 FOR_ITER               105 (to 2992)
+                    2782 STORE_FAST               3 (domain)
+         
+         351        2784 LOAD_GLOBAL              1 (NULL + print)
+                    2796 LOAD_CONST              46 ('moving domain:')
+                    2798 LOAD_FAST                3 (domain)
+                    2800 PRECALL                  2
+                    2804 CALL                     2
+                    2814 POP_TOP
+         
+         352        2816 LOAD_GLOBAL              2 (ts)
+                    2828 LOAD_ATTR                2 (query)
+                    2838 LOAD_METHOD             23 (insert_event)
+         
+         353        2860 LOAD_GLOBAL              2 (ts)
+                    2872 LOAD_ATTR               24 (models)
+                    2882 LOAD_METHOD             25 (Event)
+         
+         354        2904 LOAD_FAST                2 (search)
+                    2906 LOAD_ATTR               22 (uid)
+         
+         355        2916 LOAD_FAST                3 (domain)
+         
+         356        2918 LOAD_FAST                1 (event)
+                    2920 LOAD_ATTR               13 (data)
+                    2930 LOAD_CONST              47 ('stage')
+                    2932 BINARY_SUBSCR
+         
+         357        2942 LOAD_FAST                1 (event)
+                    2944 LOAD_ATTR               20 (actor_key)
+         
+         353        2954 KW_NAMES                48
+                    2956 PRECALL                  4
+                    2960 CALL                     4
+         
+         352        2970 PRECALL                  1
+                    2974 CALL                     1
+                    2984 POP_TOP
+                    2986 JUMP_BACKWARD          104 (to 2780)
          
-         384     >> 2852 LOAD_CONST               0 (None)
-                    2854 RETURN_VALUE
+         348     >> 2988 LOAD_CONST               0 (None)
+                    2990 RETURN_VALUE
          
-         386     >> 2856 LOAD_CONST               0 (None)
-                    2858 RETURN_VALUE
+         350     >> 2992 LOAD_CONST               0 (None)
+                    2994 RETURN_VALUE
          consts
             None
             'processing event_id: '
             ('uid',)
             'land'
             ('event',)
             'create'
@@ -2164,16 +2301,20 @@
             'client_approve'
             'reject'
             'client_reject'
             'conflict'
             'client_conflict'
             'enrich'
             'prompt'
-            'maps'
+            'criteria'
+            'inclusion'
+            'keywords'
+            0
             ('search', 'event')
+            'maps'
             'google'
             'grata_search'
             'import'
             'import_searches'
             'searches'
             ('label',)
             ('from_search', 'to_search', 'actor_key')
@@ -2190,33 +2331,33 @@
             'update'
             'name'
             'move'
             'domains'
             'moving domain:'
             'stage'
             ('search_uid', 'domain', 'type', 'actor_key')
-         names      ('print', 'ts', 'query', 'find_event_by_id', 'find_search', 'search_uid', 'domain', 'type', 'run_enrichment', 'run_acquired_check', 'run_similarity_search', 'handle_prompt', 'run_maps_search', 'run_google_search', 'important_targets_from_event', 'data', 'find_search_by_label', 'important_targets_from_search', 'actor_key', 'reset_inbox', 'uid', 'insert_event', 'models', 'Event', 'find_company_by_domain', 'get', 'name', 'meta', 'update_company', 'update_search')
+         names      ('print', 'ts', 'query', 'find_event_by_id', 'find_search', 'search_uid', 'domain', 'type', 'run_enrichment', 'run_acquired_check', 'run_similarity_search', 'handle_prompt', 'len', 'data', 'run_criteria_search', 'run_maps_search', 'run_google_search', 'important_targets_from_event', 'find_search_by_label', 'important_targets_from_search', 'actor_key', 'reset_inbox', 'uid', 'insert_event', 'models', 'Event', 'find_company_by_domain', 'get', 'name', 'meta', 'update_company', 'update_search')
          varnames   ('event_id', 'event', 'search', 'domain', 'label', 'from_search', 'rating', 'from_stage', 'company')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
          name       'process_event'
-         firstlineno 277
+         firstlineno 241
          lnotab
             0x020120013e011e014a010e011601240116012401160124011601240116
             012001200126011601240116012001260116010401160104011601200126
-            011601040216012402160124041601260116012602160126021601440216
-            011e0140012c0110ff14fe040616011e014e0218021e011a011a010c012c
-            012c010c01020102010cfc10ff14080c012c012c010c01020102010cfc10
-            ff140808012c012c010c01020102010cfc10ff14ff040a160104013e0134
-            0124012a0142022a01420216021e0120012c012c010c01020118010cfc10
-            ff12fc0402
-   names      ('dataclasses', 'asdict', 'time', 'gandai', 'ts', 'requests', 'dacite', 'from_dict', 'secrets', 'str', 'run_acquired_check', 'models', 'Search', 'run_similarity_search', 'Event', 'run_maps_search', 'run_google_search', 'handle_prompt', 'Company', 'enrich_with_gpt', 'run_enrichment', 'int', 'process_event')
+            011601040216012402160124011601480126ff0402160126011601260216
+            0126021601440216011e0140012c0110ff14fe040616011e014e0218021e
+            011a011a010c012c012c010c01020102010cfc10ff14080c012c012c010c
+            01020102010cfc10ff140808012c012c010c01020102010cfc10ff14ff04
+            0a160104013e01340124012a0142022a01420216021e0120012c012c010c
+            01020118010cfc10ff12fc0402
+   names      ('dataclasses', 'asdict', 'time', 'gandai', 'ts', 'requests', 'dacite', 'from_dict', 'secrets', 'str', 'run_acquired_check', 'models', 'Search', 'run_similarity_search', 'Event', 'run_criteria_search', 'run_maps_search', 'run_google_search', 'handle_prompt', 'Company', 'enrich_with_gpt', 'run_enrichment', 'int', 'process_event')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010c010c02080108010c010c030c2628193c2d3c37242e242724
-      13
+      0x00ff02010c010c02080108010c010c030c26280d3c0e3c2d3c11242e24
+      272413
```

### Comparing `gandai-1.7.62/gandai/__pycache__/models.cpython-311.pyc` & `gandai-1.7.63/gandai/__pycache__/models.cpython-311.pyc`

 * *Files 3% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x47715666 (Wed May 29 00:05:27 2024 UTC)
-files sz: 4501
+moddate:  0x44da5d66 (Mon Jun  3 14:59:16 2024 UTC)
+files sz: 4499
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a026d035a036d045a0401
@@ -1416,21 +1416,23 @@
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x970065005a0164005a0255006503650464013c0000006505650464023c
             000000020065066507ac03a6010000ab0100000000000000005a08650765
-            0464043c000000650964056505660264068404a6000000ab000000000000
-            0000005a0a650964056505660264078404a6000000ab0000000000000000
-            005a0b650964056505660264088404a6000000ab0000000000000000005a
-            0c650964056505660264098404a6000000ab0000000000000000005a0d65
-            09640565056602640a8404a6000000ab0000000000000000005a0e650964
-            0565056602640b8404a6000000ab0000000000000000005a0f6509640565
-            056602640c8404a6000000ab0000000000000000005a10640d5300
+            0464043c000000020065066509ac03a6010000ab0100000000000000005a
+            0a6509650464053c000000650b64066505660264078404a6000000ab0000
+            000000000000005a0c650b64066505660264088404a6000000ab00000000
+            00000000005a0d650b64066505660264098404a6000000ab000000000000
+            0000005a0e650b640665056602640a8404a6000000ab0000000000000000
+            005a0f650b640665056602640b8404a6000000ab0000000000000000005a
+            10650b640665056602640c8404a6000000ab0000000000000000005a1165
+            0b640665056602640d8404a6000000ab0000000000000000005a12640e53
+            00
          138           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Search')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
@@ -1452,112 +1454,125 @@
                       44 CALL                     1
                       54 STORE_NAME               8 (meta)
                       56 LOAD_NAME                7 (dict)
                       58 LOAD_NAME                4 (__annotations__)
                       60 LOAD_CONST               4 ('meta')
                       62 STORE_SUBSCR
          
-         147          66 LOAD_NAME                9 (property)
+         143          66 PUSH_NULL
+                      68 LOAD_NAME                6 (field)
+                      70 LOAD_NAME                9 (Criteria)
+                      72 KW_NAMES                 3
+                      74 PRECALL                  1
+                      78 CALL                     1
+                      88 STORE_NAME              10 (criteria)
+                      90 LOAD_NAME                9 (Criteria)
+                      92 LOAD_NAME                4 (__annotations__)
+                      94 LOAD_CONST               5 ('criteria')
+                      96 STORE_SUBSCR
          
-         148          68 LOAD_CONST               5 ('return')
-                      70 LOAD_NAME                5 (str)
-                      72 BUILD_TUPLE              2
-                      74 LOAD_CONST               6 (<code object notes, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 147>)
-                      76 MAKE_FUNCTION            4 (annotations)
+         147         100 LOAD_NAME               11 (property)
          
-         147          78 PRECALL                  0
-                      82 CALL                     0
+         148         102 LOAD_CONST               6 ('return')
+                     104 LOAD_NAME                5 (str)
+                     106 BUILD_TUPLE              2
+                     108 LOAD_CONST               7 (<code object notes, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 147>)
+                     110 MAKE_FUNCTION            4 (annotations)
          
-         148          92 STORE_NAME              10 (notes)
+         147         112 PRECALL                  0
+                     116 CALL                     0
          
-         151          94 LOAD_NAME                9 (property)
+         148         126 STORE_NAME              12 (notes)
          
-         152          96 LOAD_CONST               5 ('return')
-                      98 LOAD_NAME                5 (str)
-                     100 BUILD_TUPLE              2
-                     102 LOAD_CONST               7 (<code object type, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 151>)
-                     104 MAKE_FUNCTION            4 (annotations)
+         151         128 LOAD_NAME               11 (property)
          
-         151         106 PRECALL                  0
-                     110 CALL                     0
+         152         130 LOAD_CONST               6 ('return')
+                     132 LOAD_NAME                5 (str)
+                     134 BUILD_TUPLE              2
+                     136 LOAD_CONST               8 (<code object type, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 151>)
+                     138 MAKE_FUNCTION            4 (annotations)
          
-         152         120 STORE_NAME              11 (type)
+         151         140 PRECALL                  0
+                     144 CALL                     0
          
-         155         122 LOAD_NAME                9 (property)
+         152         154 STORE_NAME              13 (type)
          
-         156         124 LOAD_CONST               5 ('return')
-                     126 LOAD_NAME                5 (str)
-                     128 BUILD_TUPLE              2
-                     130 LOAD_CONST               8 (<code object prompt, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 155>)
-                     132 MAKE_FUNCTION            4 (annotations)
+         155         156 LOAD_NAME               11 (property)
          
-         155         134 PRECALL                  0
-                     138 CALL                     0
+         156         158 LOAD_CONST               6 ('return')
+                     160 LOAD_NAME                5 (str)
+                     162 BUILD_TUPLE              2
+                     164 LOAD_CONST               9 (<code object prompt, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 155>)
+                     166 MAKE_FUNCTION            4 (annotations)
+         
+         155         168 PRECALL                  0
+                     172 CALL                     0
          
-         156         148 STORE_NAME              12 (prompt)
+         156         182 STORE_NAME              14 (prompt)
          
-         159         150 LOAD_NAME                9 (property)
+         159         184 LOAD_NAME               11 (property)
          
-         160         152 LOAD_CONST               5 ('return')
-                     154 LOAD_NAME                5 (str)
-                     156 BUILD_TUPLE              2
-                     158 LOAD_CONST               9 (<code object products, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 159>)
-                     160 MAKE_FUNCTION            4 (annotations)
+         160         186 LOAD_CONST               6 ('return')
+                     188 LOAD_NAME                5 (str)
+                     190 BUILD_TUPLE              2
+                     192 LOAD_CONST              10 (<code object products, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 159>)
+                     194 MAKE_FUNCTION            4 (annotations)
          
-         159         162 PRECALL                  0
-                     166 CALL                     0
+         159         196 PRECALL                  0
+                     200 CALL                     0
          
-         160         176 STORE_NAME              13 (products)
+         160         210 STORE_NAME              15 (products)
          
-         164         178 LOAD_NAME                9 (property)
+         164         212 LOAD_NAME               11 (property)
          
-         165         180 LOAD_CONST               5 ('return')
-                     182 LOAD_NAME                5 (str)
-                     184 BUILD_TUPLE              2
-                     186 LOAD_CONST              10 (<code object services, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 164>)
-                     188 MAKE_FUNCTION            4 (annotations)
+         165         214 LOAD_CONST               6 ('return')
+                     216 LOAD_NAME                5 (str)
+                     218 BUILD_TUPLE              2
+                     220 LOAD_CONST              11 (<code object services, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 164>)
+                     222 MAKE_FUNCTION            4 (annotations)
          
-         164         190 PRECALL                  0
-                     194 CALL                     0
+         164         224 PRECALL                  0
+                     228 CALL                     0
          
-         165         204 STORE_NAME              14 (services)
+         165         238 STORE_NAME              16 (services)
          
-         169         206 LOAD_NAME                9 (property)
+         169         240 LOAD_NAME               11 (property)
          
-         170         208 LOAD_CONST               5 ('return')
-                     210 LOAD_NAME                5 (str)
-                     212 BUILD_TUPLE              2
-                     214 LOAD_CONST              11 (<code object customers, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 169>)
-                     216 MAKE_FUNCTION            4 (annotations)
+         170         242 LOAD_CONST               6 ('return')
+                     244 LOAD_NAME                5 (str)
+                     246 BUILD_TUPLE              2
+                     248 LOAD_CONST              12 (<code object customers, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 169>)
+                     250 MAKE_FUNCTION            4 (annotations)
          
-         169         218 PRECALL                  0
-                     222 CALL                     0
+         169         252 PRECALL                  0
+                     256 CALL                     0
          
-         170         232 STORE_NAME              15 (customers)
+         170         266 STORE_NAME              17 (customers)
          
-         174         234 LOAD_NAME                9 (property)
+         174         268 LOAD_NAME               11 (property)
          
-         175         236 LOAD_CONST               5 ('return')
-                     238 LOAD_NAME                5 (str)
-                     240 BUILD_TUPLE              2
-                     242 LOAD_CONST              12 (<code object token, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 174>)
-                     244 MAKE_FUNCTION            4 (annotations)
+         175         270 LOAD_CONST               6 ('return')
+                     272 LOAD_NAME                5 (str)
+                     274 BUILD_TUPLE              2
+                     276 LOAD_CONST              13 (<code object token, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 174>)
+                     278 MAKE_FUNCTION            4 (annotations)
          
-         174         246 PRECALL                  0
-                     250 CALL                     0
+         174         280 PRECALL                  0
+                     284 CALL                     0
          
-         175         260 STORE_NAME              16 (token)
-                     262 LOAD_CONST              13 (None)
-                     264 RETURN_VALUE
+         175         294 STORE_NAME              18 (token)
+                     296 LOAD_CONST              14 (None)
+                     298 RETURN_VALUE
          consts
             'Search'
             'uid'
             'label'
             ('default_factory',)
             'meta'
+            'criteria'
             'return'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
@@ -1768,25 +1783,25 @@
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
                name       'token'
                firstlineno 174
                lnotab 0x0203
             None
-         names      ('__name__', '__module__', '__qualname__', 'int', '__annotations__', 'str', 'field', 'dict', 'meta', 'property', 'notes', 'type', 'prompt', 'products', 'services', 'customers', 'token')
+         names      ('__name__', '__module__', '__qualname__', 'int', '__annotations__', 'str', 'field', 'dict', 'meta', 'Criteria', 'criteria', 'property', 'notes', 'type', 'prompt', 'products', 'services', 'customers', 'token')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
          name       'Search'
          firstlineno 138
          lnotab
-            0x0c020a010a01220502010aff0e01020302010aff0e01020302010aff0e
-            01020302010aff0e01020402010aff0e01020402010aff0e01020402010a
-            ff0e01
+            0x0c020a010a012201220402010aff0e01020302010aff0e01020302010a
+            ff0e01020302010aff0e01020402010aff0e01020402010aff0e01020402
+            010aff0e01
       'Search'
    names      ('hashlib', 'dataclasses', 'asdict', 'dataclass', 'field', 'enum', 'Enum', 'auto', 'typing', 'Any', 'List', 'Optional', 'Actor', 'Company', 'str', 'EventType', 'Event', 'Comment', 'Rating', 'Inclusion', 'Exclusion', 'Criteria', 'Maps', 'Search')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
    name       '<module>'
```

### Comparing `gandai-1.7.62/gandai/__pycache__/query.cpython-311.pyc` & `gandai-1.7.63/gandai/__pycache__/query.cpython-311.pyc`

 * *Files 3% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x22835766 (Wed May 29 19:33:54 2024 UTC)
-files sz: 31724
+moddate:  0x20dc5d66 (Mon Jun  3 15:07:12 2024 UTC)
+files sz: 32396
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 15
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064026c026d035a0301
@@ -16,461 +16,470 @@
       006513a6000000ab0000000000000000005a1a640a6517640b6517660464
       0c84045a1b640d6516640b65106a1c00000000000000006a160000000000
       0000006604640e84045a1d640f6515640b65156604641084045a1e641165
       19640b65196604641284045a1f641365106a1c00000000000000006a1900
       00000000000000641465106a1c00000000000000006a1900000000000000
       0064156520640b64016608641684045a21640a65106a1c00000000000000
       006a170000000000000000640b64016604641784045a2209000900090064
-      3e641a6507650619000000000000000000641b652364156520641c652464
+      3f641a6507650619000000000000000000641b652364156520641c652464
       1d6520641e6520640b6401660e641f84055a25640b65096a260000000000
       0000006602642084045a27642184005a28640b65096a2600000000000000
       006602642284045a29642384005a2a642484005a2b640b65096a26000000
       00000000006602642584045a2c640b65096a260000000000000000660264
       2684045a2d641b65236602642784045a2e641b6523640b65096a26000000
       00000000006604642884045a2f641b6523640b65096a2600000000000000
       006604642984045a30641b6523640b65096a260000000000000000660464
       2a84045a31641b6523640b65096a2600000000000000006604642b84045a
       32642c6523640b65106a1c00000000000000006a19000000000000000066
       04642d84045a33642e6520640b65106a1c00000000000000006a19000000
       00000000006604642f84045a3464306520640b65106a1c00000000000000
       006a1900000000000000006604643184045a3564326520640b6516660464
       3384045a3664346520640b65166604643584045a3764366523640b651766
-      04643784045a38640d6516640b64016604643884045a3964116519640b64
-      016604643984045a3a64366523640b64016604643a84045a3b643b652364
-      0b64016604643c84045a3c641b6523640b64016604643d84045a3d640153
-      00
-     0           0 RESUME                   0
-   
-     1           2 LOAD_CONST               0 (0)
-                 4 LOAD_CONST               1 (None)
-                 6 IMPORT_NAME              0 (hashlib)
-                 8 STORE_NAME               0 (hashlib)
-   
-     2          10 LOAD_CONST               0 (0)
-                12 LOAD_CONST               1 (None)
-                14 IMPORT_NAME              1 (json)
-                16 STORE_NAME               1 (json)
-   
-     3          18 LOAD_CONST               0 (0)
-                20 LOAD_CONST               2 (('asdict',))
-                22 IMPORT_NAME              2 (dataclasses)
-                24 IMPORT_FROM              3 (asdict)
-                26 STORE_NAME               3 (asdict)
-                28 POP_TOP
-   
-     4          30 LOAD_CONST               0 (0)
-                32 LOAD_CONST               3 (('time',))
-                34 IMPORT_NAME              4 (time)
-                36 IMPORT_FROM              4 (time)
-                38 STORE_NAME               4 (time)
-                40 POP_TOP
-   
-     5          42 LOAD_CONST               0 (0)
-                44 LOAD_CONST               4 (('Any', 'List'))
-                46 IMPORT_NAME              5 (typing)
-                48 IMPORT_FROM              6 (Any)
-                50 STORE_NAME               6 (Any)
-                52 IMPORT_FROM              7 (List)
-                54 STORE_NAME               7 (List)
-                56 POP_TOP
-   
-     7          58 LOAD_CONST               0 (0)
-                60 LOAD_CONST               1 (None)
-                62 IMPORT_NAME              8 (pandas)
-                64 STORE_NAME               9 (pd)
-   
-     8          66 LOAD_CONST               0 (0)
-                68 LOAD_CONST               1 (None)
-                70 IMPORT_NAME             10 (sqlalchemy)
-                72 STORE_NAME              10 (sqlalchemy)
-   
-     9          74 LOAD_CONST               0 (0)
-                76 LOAD_CONST               5 (('from_dict',))
-                78 IMPORT_NAME             11 (dacite)
-                80 IMPORT_FROM             12 (from_dict)
-                82 STORE_NAME              12 (from_dict)
-                84 POP_TOP
-   
-    10          86 LOAD_CONST               0 (0)
-                88 LOAD_CONST               6 (('load_dotenv',))
-                90 IMPORT_NAME             13 (dotenv)
-                92 IMPORT_FROM             14 (load_dotenv)
-                94 STORE_NAME              14 (load_dotenv)
-                96 POP_TOP
-   
-    12          98 PUSH_NULL
-               100 LOAD_NAME               14 (load_dotenv)
-               102 PRECALL                  0
-               106 CALL                     0
-               116 POP_TOP
-   
-    14         118 LOAD_CONST               0 (0)
-               120 LOAD_CONST               1 (None)
-               122 IMPORT_NAME             15 (gandai)
-               124 STORE_NAME              16 (ts)
-   
-    15         126 LOAD_CONST               0 (0)
-               128 LOAD_CONST               7 (('helpers',))
-               130 IMPORT_NAME             15 (gandai)
-               132 IMPORT_FROM             17 (helpers)
-               134 STORE_NAME              17 (helpers)
-               136 POP_TOP
-   
-    16         138 LOAD_CONST               0 (0)
-               140 LOAD_CONST               8 (('connect_with_connector',))
-               142 IMPORT_NAME             18 (gandai.db)
-               144 IMPORT_FROM             19 (connect_with_connector)
-               146 STORE_NAME              19 (connect_with_connector)
-               148 POP_TOP
-   
-    17         150 LOAD_CONST               0 (0)
-               152 LOAD_CONST               9 (('Actor', 'Company', 'Event', 'EventType', 'Search'))
-               154 IMPORT_NAME             20 (gandai.models)
-               156 IMPORT_FROM             21 (Actor)
-               158 STORE_NAME              21 (Actor)
-               160 IMPORT_FROM             22 (Company)
-               162 STORE_NAME              22 (Company)
-               164 IMPORT_FROM             23 (Event)
-               166 STORE_NAME              23 (Event)
-               168 IMPORT_FROM             24 (EventType)
-               170 STORE_NAME              24 (EventType)
-               172 IMPORT_FROM             25 (Search)
-               174 STORE_NAME              25 (Search)
-               176 POP_TOP
-   
-    19         178 PUSH_NULL
-               180 LOAD_NAME               19 (connect_with_connector)
-               182 PRECALL                  0
-               186 CALL                     0
-               196 STORE_NAME              26 (db)
-   
-    25         198 LOAD_CONST              10 ('event')
-               200 LOAD_NAME               23 (Event)
-               202 LOAD_CONST              11 ('return')
-               204 LOAD_NAME               23 (Event)
-               206 BUILD_TUPLE              4
-               208 LOAD_CONST              12 (<code object insert_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 25>)
-               210 MAKE_FUNCTION            4 (annotations)
-               212 STORE_NAME              27 (insert_event)
-   
-    55         214 LOAD_CONST              13 ('company')
-               216 LOAD_NAME               22 (Company)
-               218 LOAD_CONST              11 ('return')
-               220 LOAD_NAME               16 (ts)
-               222 LOAD_ATTR               28 (models)
-               232 LOAD_ATTR               22 (Company)
-               242 BUILD_TUPLE              4
-               244 LOAD_CONST              14 (<code object insert_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 55>)
-               246 MAKE_FUNCTION            4 (annotations)
-               248 STORE_NAME              29 (insert_company)
-   
-    69         250 LOAD_CONST              15 ('actor')
-               252 LOAD_NAME               21 (Actor)
-               254 LOAD_CONST              11 ('return')
-               256 LOAD_NAME               21 (Actor)
-               258 BUILD_TUPLE              4
-               260 LOAD_CONST              16 (<code object insert_actor, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 69>)
-               262 MAKE_FUNCTION            4 (annotations)
-               264 STORE_NAME              30 (insert_actor)
-   
-    84         266 LOAD_CONST              17 ('search')
-               268 LOAD_NAME               25 (Search)
-               270 LOAD_CONST              11 ('return')
-               272 LOAD_NAME               25 (Search)
-               274 BUILD_TUPLE              4
-               276 LOAD_CONST              18 (<code object insert_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 84>)
-               278 MAKE_FUNCTION            4 (annotations)
-               280 STORE_NAME              31 (insert_search)
-   
-   100         282 LOAD_CONST              19 ('from_search')
-   
-   101         284 LOAD_NAME               16 (ts)
-               286 LOAD_ATTR               28 (models)
-               296 LOAD_ATTR               25 (Search)
-   
-   100         306 LOAD_CONST              20 ('to_search')
-   
-   101         308 LOAD_NAME               16 (ts)
-               310 LOAD_ATTR               28 (models)
-               320 LOAD_ATTR               25 (Search)
-   
-   100         330 LOAD_CONST              21 ('actor_key')
-   
-   101         332 LOAD_NAME               32 (str)
-   
-   100         334 LOAD_CONST              11 ('return')
-   
-   102         336 LOAD_CONST               1 (None)
-   
-   100         338 BUILD_TUPLE              8
-               340 LOAD_CONST              22 (<code object important_targets_from_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 100>)
-               342 MAKE_FUNCTION            4 (annotations)
-               344 STORE_NAME              33 (important_targets_from_search)
-   
-   161         346 LOAD_CONST              10 ('event')
-               348 LOAD_NAME               16 (ts)
-               350 LOAD_ATTR               28 (models)
-               360 LOAD_ATTR               23 (Event)
-               370 LOAD_CONST              11 ('return')
-               372 LOAD_CONST               1 (None)
-               374 BUILD_TUPLE              4
-               376 LOAD_CONST              23 (<code object important_targets_from_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 161>)
-               378 MAKE_FUNCTION            4 (annotations)
-               380 STORE_NAME              34 (important_targets_from_event)
-   
-   239         382 NOP
-   
-   240         384 NOP
-   
-   241         386 NOP
-   
-   235         388 LOAD_CONST              62 ((True, None, 'create'))
-               390 LOAD_CONST              26 ('companies')
-   
-   236         392 LOAD_NAME                7 (List)
-               394 LOAD_NAME                6 (Any)
-               396 BINARY_SUBSCR
-   
-   235         406 LOAD_CONST              27 ('search_uid')
-   
-   237         408 LOAD_NAME               35 (int)
-   
-   235         410 LOAD_CONST              21 ('actor_key')
-   
-   238         412 LOAD_NAME               32 (str)
-   
-   235         414 LOAD_CONST              28 ('force')
-   
-   239         416 LOAD_NAME               36 (bool)
-   
-   235         418 LOAD_CONST              29 ('source')
-   
-   240         420 LOAD_NAME               32 (str)
-   
-   235         422 LOAD_CONST              30 ('stage')
-   
-   241         424 LOAD_NAME               32 (str)
-   
-   235         426 LOAD_CONST              11 ('return')
-   
-   242         428 LOAD_CONST               1 (None)
-   
-   235         430 BUILD_TUPLE             14
-               432 LOAD_CONST              31 (<code object insert_companies_as_targets, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 235>)
-               434 MAKE_FUNCTION            5 (defaults, annotations)
-               436 STORE_NAME              37 (insert_companies_as_targets)
-   
-   332         438 LOAD_CONST              11 ('return')
-               440 LOAD_NAME                9 (pd)
-               442 LOAD_ATTR               38 (DataFrame)
-               452 BUILD_TUPLE              2
-               454 LOAD_CONST              32 (<code object searches_query, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 332>)
-               456 MAKE_FUNCTION            4 (annotations)
-               458 STORE_NAME              39 (searches_query)
-   
-   364         460 LOAD_CONST              33 (<code object average_rating_per_search_query, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 364>)
-               462 MAKE_FUNCTION            0
-               464 STORE_NAME              40 (average_rating_per_search_query)
-   
-   376         466 LOAD_CONST              11 ('return')
-               468 LOAD_NAME                9 (pd)
-               470 LOAD_ATTR               38 (DataFrame)
-               480 BUILD_TUPLE              2
-               482 LOAD_CONST              34 (<code object validation_history, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 376>)
-               484 MAKE_FUNCTION            4 (annotations)
-               486 STORE_NAME              41 (validation_history)
-   
-   419         488 LOAD_CONST              35 (<code object searches_comment_counts, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 419>)
-               490 MAKE_FUNCTION            0
-               492 STORE_NAME              42 (searches_comment_counts)
-   
-   439         494 LOAD_CONST              36 (<code object enriched_searches_query, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 439>)
-               496 MAKE_FUNCTION            0
-               498 STORE_NAME              43 (enriched_searches_query)
-   
-   459         500 LOAD_CONST              11 ('return')
-               502 LOAD_NAME                9 (pd)
-               504 LOAD_ATTR               38 (DataFrame)
-               514 BUILD_TUPLE              2
-               516 LOAD_CONST              37 (<code object actor, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 459>)
-               518 MAKE_FUNCTION            4 (annotations)
-               520 STORE_NAME              44 (actor)
-   
-   473         522 LOAD_CONST              11 ('return')
-               524 LOAD_NAME                9 (pd)
-               526 LOAD_ATTR               38 (DataFrame)
-               536 BUILD_TUPLE              2
-               538 LOAD_CONST              38 (<code object buyer, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 473>)
-               540 MAKE_FUNCTION            4 (annotations)
-               542 STORE_NAME              45 (buyer)
-   
-   570         544 LOAD_CONST              27 ('search_uid')
-               546 LOAD_NAME               35 (int)
-               548 BUILD_TUPLE              2
-               550 LOAD_CONST              39 (<code object search_targets, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 570>)
-               552 MAKE_FUNCTION            4 (annotations)
-               554 STORE_NAME              46 (search_targets)
-   
-   704         556 LOAD_CONST              27 ('search_uid')
-               558 LOAD_NAME               35 (int)
-               560 LOAD_CONST              11 ('return')
-               562 LOAD_NAME                9 (pd)
-               564 LOAD_ATTR               38 (DataFrame)
-               574 BUILD_TUPLE              4
-               576 LOAD_CONST              40 (<code object search_comments, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 704>)
-               578 MAKE_FUNCTION            4 (annotations)
-               580 STORE_NAME              47 (search_comments)
-   
-   726         582 LOAD_CONST              27 ('search_uid')
-               584 LOAD_NAME               35 (int)
-               586 LOAD_CONST              11 ('return')
-               588 LOAD_NAME                9 (pd)
-               590 LOAD_ATTR               38 (DataFrame)
-               600 BUILD_TUPLE              4
-               602 LOAD_CONST              41 (<code object event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 726>)
-               604 MAKE_FUNCTION            4 (annotations)
-               606 STORE_NAME              48 (event)
-   
-   738         608 LOAD_CONST              27 ('search_uid')
-               610 LOAD_NAME               35 (int)
-               612 LOAD_CONST              11 ('return')
-               614 LOAD_NAME                9 (pd)
-               616 LOAD_ATTR               38 (DataFrame)
-               626 BUILD_TUPLE              4
-               628 LOAD_CONST              42 (<code object event_history, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 738>)
-               630 MAKE_FUNCTION            4 (annotations)
-               632 STORE_NAME              49 (event_history)
-   
-   768         634 LOAD_CONST              27 ('search_uid')
-               636 LOAD_NAME               35 (int)
-               638 LOAD_CONST              11 ('return')
-               640 LOAD_NAME                9 (pd)
-               642 LOAD_ATTR               38 (DataFrame)
-               652 BUILD_TUPLE              4
-               654 LOAD_CONST              43 (<code object search_criteria_history, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 768>)
-               656 MAKE_FUNCTION            4 (annotations)
-               658 STORE_NAME              50 (search_criteria_history)
-   
-   797         660 LOAD_CONST              44 ('uid')
-               662 LOAD_NAME               35 (int)
-               664 LOAD_CONST              11 ('return')
-               666 LOAD_NAME               16 (ts)
-               668 LOAD_ATTR               28 (models)
-               678 LOAD_ATTR               25 (Search)
-               688 BUILD_TUPLE              4
-               690 LOAD_CONST              45 (<code object find_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 797>)
-               692 MAKE_FUNCTION            4 (annotations)
-               694 STORE_NAME              51 (find_search)
-   
-   821         696 LOAD_CONST              46 ('label')
-               698 LOAD_NAME               32 (str)
-               700 LOAD_CONST              11 ('return')
-               702 LOAD_NAME               16 (ts)
-               704 LOAD_ATTR               28 (models)
-               714 LOAD_ATTR               25 (Search)
-               724 BUILD_TUPLE              4
-               726 LOAD_CONST              47 (<code object find_search_by_label, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 821>)
-               728 MAKE_FUNCTION            4 (annotations)
-               730 STORE_NAME              52 (find_search_by_label)
-   
-   845         732 LOAD_CONST              48 ('searchToken')
-               734 LOAD_NAME               32 (str)
-               736 LOAD_CONST              11 ('return')
-               738 LOAD_NAME               16 (ts)
-               740 LOAD_ATTR               28 (models)
-               750 LOAD_ATTR               25 (Search)
-               760 BUILD_TUPLE              4
-               762 LOAD_CONST              49 (<code object find_search_by_token, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 845>)
-               764 MAKE_FUNCTION            4 (annotations)
-               766 STORE_NAME              53 (find_search_by_token)
-   
-   854         768 LOAD_CONST              50 ('domain')
-               770 LOAD_NAME               32 (str)
-               772 LOAD_CONST              11 ('return')
-               774 LOAD_NAME               22 (Company)
-               776 BUILD_TUPLE              4
-               778 LOAD_CONST              51 (<code object find_company_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 854>)
-               780 MAKE_FUNCTION            4 (annotations)
-               782 STORE_NAME              54 (find_company_by_domain)
-   
-   870         784 LOAD_CONST              52 ('email')
-               786 LOAD_NAME               32 (str)
-               788 LOAD_CONST              11 ('return')
-               790 LOAD_NAME               22 (Company)
-               792 BUILD_TUPLE              4
-               794 LOAD_CONST              53 (<code object find_actor_by_email, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 870>)
-               796 MAKE_FUNCTION            4 (annotations)
-               798 STORE_NAME              55 (find_actor_by_email)
-   
-   886         800 LOAD_CONST              54 ('event_id')
-               802 LOAD_NAME               35 (int)
-               804 LOAD_CONST              11 ('return')
-               806 LOAD_NAME               23 (Event)
-               808 BUILD_TUPLE              4
-               810 LOAD_CONST              55 (<code object find_event_by_id, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 886>)
-               812 MAKE_FUNCTION            4 (annotations)
-               814 STORE_NAME              56 (find_event_by_id)
-   
-   905         816 LOAD_CONST              13 ('company')
-               818 LOAD_NAME               22 (Company)
-               820 LOAD_CONST              11 ('return')
-               822 LOAD_CONST               1 (None)
-               824 BUILD_TUPLE              4
-               826 LOAD_CONST              56 (<code object update_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 905>)
-               828 MAKE_FUNCTION            4 (annotations)
-               830 STORE_NAME              57 (update_company)
-   
-   934         832 LOAD_CONST              17 ('search')
-               834 LOAD_NAME               25 (Search)
-               836 LOAD_CONST              11 ('return')
-               838 LOAD_CONST               1 (None)
-               840 BUILD_TUPLE              4
-               842 LOAD_CONST              57 (<code object update_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 934>)
-               844 MAKE_FUNCTION            4 (annotations)
-               846 STORE_NAME              58 (update_search)
-   
-   957         848 LOAD_CONST              54 ('event_id')
-               850 LOAD_NAME               35 (int)
-               852 LOAD_CONST              11 ('return')
-               854 LOAD_CONST               1 (None)
-               856 BUILD_TUPLE              4
-               858 LOAD_CONST              58 (<code object mute_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 957>)
-               860 MAKE_FUNCTION            4 (annotations)
-               862 STORE_NAME              59 (mute_event)
-   
-   980         864 LOAD_CONST              59 ('comment_id')
-               866 LOAD_NAME               35 (int)
-               868 LOAD_CONST              11 ('return')
-               870 LOAD_CONST               1 (None)
-               872 BUILD_TUPLE              4
-               874 LOAD_CONST              60 (<code object delete_comment, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 980>)
-               876 MAKE_FUNCTION            4 (annotations)
-               878 STORE_NAME              60 (delete_comment)
-   
-   991         880 LOAD_CONST              27 ('search_uid')
-               882 LOAD_NAME               35 (int)
-               884 LOAD_CONST              11 ('return')
-               886 LOAD_CONST               1 (None)
-               888 BUILD_TUPLE              4
-               890 LOAD_CONST              61 (<code object reset_inbox, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 991>)
-               892 MAKE_FUNCTION            4 (annotations)
-               894 STORE_NAME              61 (reset_inbox)
-               896 LOAD_CONST               1 (None)
-               898 RETURN_VALUE
+      04643784045a38641b6523640b65186604643884045a39640d6516640b64
+      016604643984045a3a64116519640b64016604643a84045a3b6436652364
+      0b64016604643b84045a3c643c6523640b64016604643d84045a3d641b65
+      23640b64016604643e84045a3e64015300
+      0           0 RESUME                   0
+   
+      1           2 LOAD_CONST               0 (0)
+                  4 LOAD_CONST               1 (None)
+                  6 IMPORT_NAME              0 (hashlib)
+                  8 STORE_NAME               0 (hashlib)
+   
+      2          10 LOAD_CONST               0 (0)
+                 12 LOAD_CONST               1 (None)
+                 14 IMPORT_NAME              1 (json)
+                 16 STORE_NAME               1 (json)
+   
+      3          18 LOAD_CONST               0 (0)
+                 20 LOAD_CONST               2 (('asdict',))
+                 22 IMPORT_NAME              2 (dataclasses)
+                 24 IMPORT_FROM              3 (asdict)
+                 26 STORE_NAME               3 (asdict)
+                 28 POP_TOP
+   
+      4          30 LOAD_CONST               0 (0)
+                 32 LOAD_CONST               3 (('time',))
+                 34 IMPORT_NAME              4 (time)
+                 36 IMPORT_FROM              4 (time)
+                 38 STORE_NAME               4 (time)
+                 40 POP_TOP
+   
+      5          42 LOAD_CONST               0 (0)
+                 44 LOAD_CONST               4 (('Any', 'List'))
+                 46 IMPORT_NAME              5 (typing)
+                 48 IMPORT_FROM              6 (Any)
+                 50 STORE_NAME               6 (Any)
+                 52 IMPORT_FROM              7 (List)
+                 54 STORE_NAME               7 (List)
+                 56 POP_TOP
+   
+      7          58 LOAD_CONST               0 (0)
+                 60 LOAD_CONST               1 (None)
+                 62 IMPORT_NAME              8 (pandas)
+                 64 STORE_NAME               9 (pd)
+   
+      8          66 LOAD_CONST               0 (0)
+                 68 LOAD_CONST               1 (None)
+                 70 IMPORT_NAME             10 (sqlalchemy)
+                 72 STORE_NAME              10 (sqlalchemy)
+   
+      9          74 LOAD_CONST               0 (0)
+                 76 LOAD_CONST               5 (('from_dict',))
+                 78 IMPORT_NAME             11 (dacite)
+                 80 IMPORT_FROM             12 (from_dict)
+                 82 STORE_NAME              12 (from_dict)
+                 84 POP_TOP
+   
+     10          86 LOAD_CONST               0 (0)
+                 88 LOAD_CONST               6 (('load_dotenv',))
+                 90 IMPORT_NAME             13 (dotenv)
+                 92 IMPORT_FROM             14 (load_dotenv)
+                 94 STORE_NAME              14 (load_dotenv)
+                 96 POP_TOP
+   
+     12          98 PUSH_NULL
+                100 LOAD_NAME               14 (load_dotenv)
+                102 PRECALL                  0
+                106 CALL                     0
+                116 POP_TOP
+   
+     14         118 LOAD_CONST               0 (0)
+                120 LOAD_CONST               1 (None)
+                122 IMPORT_NAME             15 (gandai)
+                124 STORE_NAME              16 (ts)
+   
+     15         126 LOAD_CONST               0 (0)
+                128 LOAD_CONST               7 (('helpers',))
+                130 IMPORT_NAME             15 (gandai)
+                132 IMPORT_FROM             17 (helpers)
+                134 STORE_NAME              17 (helpers)
+                136 POP_TOP
+   
+     16         138 LOAD_CONST               0 (0)
+                140 LOAD_CONST               8 (('connect_with_connector',))
+                142 IMPORT_NAME             18 (gandai.db)
+                144 IMPORT_FROM             19 (connect_with_connector)
+                146 STORE_NAME              19 (connect_with_connector)
+                148 POP_TOP
+   
+     17         150 LOAD_CONST               0 (0)
+                152 LOAD_CONST               9 (('Actor', 'Company', 'Event', 'Criteria', 'Search'))
+                154 IMPORT_NAME             20 (gandai.models)
+                156 IMPORT_FROM             21 (Actor)
+                158 STORE_NAME              21 (Actor)
+                160 IMPORT_FROM             22 (Company)
+                162 STORE_NAME              22 (Company)
+                164 IMPORT_FROM             23 (Event)
+                166 STORE_NAME              23 (Event)
+                168 IMPORT_FROM             24 (Criteria)
+                170 STORE_NAME              24 (Criteria)
+                172 IMPORT_FROM             25 (Search)
+                174 STORE_NAME              25 (Search)
+                176 POP_TOP
+   
+     19         178 PUSH_NULL
+                180 LOAD_NAME               19 (connect_with_connector)
+                182 PRECALL                  0
+                186 CALL                     0
+                196 STORE_NAME              26 (db)
+   
+     25         198 LOAD_CONST              10 ('event')
+                200 LOAD_NAME               23 (Event)
+                202 LOAD_CONST              11 ('return')
+                204 LOAD_NAME               23 (Event)
+                206 BUILD_TUPLE              4
+                208 LOAD_CONST              12 (<code object insert_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 25>)
+                210 MAKE_FUNCTION            4 (annotations)
+                212 STORE_NAME              27 (insert_event)
+   
+     55         214 LOAD_CONST              13 ('company')
+                216 LOAD_NAME               22 (Company)
+                218 LOAD_CONST              11 ('return')
+                220 LOAD_NAME               16 (ts)
+                222 LOAD_ATTR               28 (models)
+                232 LOAD_ATTR               22 (Company)
+                242 BUILD_TUPLE              4
+                244 LOAD_CONST              14 (<code object insert_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 55>)
+                246 MAKE_FUNCTION            4 (annotations)
+                248 STORE_NAME              29 (insert_company)
+   
+     69         250 LOAD_CONST              15 ('actor')
+                252 LOAD_NAME               21 (Actor)
+                254 LOAD_CONST              11 ('return')
+                256 LOAD_NAME               21 (Actor)
+                258 BUILD_TUPLE              4
+                260 LOAD_CONST              16 (<code object insert_actor, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 69>)
+                262 MAKE_FUNCTION            4 (annotations)
+                264 STORE_NAME              30 (insert_actor)
+   
+     84         266 LOAD_CONST              17 ('search')
+                268 LOAD_NAME               25 (Search)
+                270 LOAD_CONST              11 ('return')
+                272 LOAD_NAME               25 (Search)
+                274 BUILD_TUPLE              4
+                276 LOAD_CONST              18 (<code object insert_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 84>)
+                278 MAKE_FUNCTION            4 (annotations)
+                280 STORE_NAME              31 (insert_search)
+   
+    100         282 LOAD_CONST              19 ('from_search')
+   
+    101         284 LOAD_NAME               16 (ts)
+                286 LOAD_ATTR               28 (models)
+                296 LOAD_ATTR               25 (Search)
+   
+    100         306 LOAD_CONST              20 ('to_search')
+   
+    101         308 LOAD_NAME               16 (ts)
+                310 LOAD_ATTR               28 (models)
+                320 LOAD_ATTR               25 (Search)
+   
+    100         330 LOAD_CONST              21 ('actor_key')
+   
+    101         332 LOAD_NAME               32 (str)
+   
+    100         334 LOAD_CONST              11 ('return')
+   
+    102         336 LOAD_CONST               1 (None)
+   
+    100         338 BUILD_TUPLE              8
+                340 LOAD_CONST              22 (<code object important_targets_from_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 100>)
+                342 MAKE_FUNCTION            4 (annotations)
+                344 STORE_NAME              33 (important_targets_from_search)
+   
+    161         346 LOAD_CONST              10 ('event')
+                348 LOAD_NAME               16 (ts)
+                350 LOAD_ATTR               28 (models)
+                360 LOAD_ATTR               23 (Event)
+                370 LOAD_CONST              11 ('return')
+                372 LOAD_CONST               1 (None)
+                374 BUILD_TUPLE              4
+                376 LOAD_CONST              23 (<code object important_targets_from_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 161>)
+                378 MAKE_FUNCTION            4 (annotations)
+                380 STORE_NAME              34 (important_targets_from_event)
+   
+    239         382 NOP
+   
+    240         384 NOP
+   
+    241         386 NOP
+   
+    235         388 LOAD_CONST              63 ((True, None, 'create'))
+                390 LOAD_CONST              26 ('companies')
+   
+    236         392 LOAD_NAME                7 (List)
+                394 LOAD_NAME                6 (Any)
+                396 BINARY_SUBSCR
+   
+    235         406 LOAD_CONST              27 ('search_uid')
+   
+    237         408 LOAD_NAME               35 (int)
+   
+    235         410 LOAD_CONST              21 ('actor_key')
+   
+    238         412 LOAD_NAME               32 (str)
+   
+    235         414 LOAD_CONST              28 ('force')
+   
+    239         416 LOAD_NAME               36 (bool)
+   
+    235         418 LOAD_CONST              29 ('source')
+   
+    240         420 LOAD_NAME               32 (str)
+   
+    235         422 LOAD_CONST              30 ('stage')
+   
+    241         424 LOAD_NAME               32 (str)
+   
+    235         426 LOAD_CONST              11 ('return')
+   
+    242         428 LOAD_CONST               1 (None)
+   
+    235         430 BUILD_TUPLE             14
+                432 LOAD_CONST              31 (<code object insert_companies_as_targets, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 235>)
+                434 MAKE_FUNCTION            5 (defaults, annotations)
+                436 STORE_NAME              37 (insert_companies_as_targets)
+   
+    332         438 LOAD_CONST              11 ('return')
+                440 LOAD_NAME                9 (pd)
+                442 LOAD_ATTR               38 (DataFrame)
+                452 BUILD_TUPLE              2
+                454 LOAD_CONST              32 (<code object searches_query, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 332>)
+                456 MAKE_FUNCTION            4 (annotations)
+                458 STORE_NAME              39 (searches_query)
+   
+    364         460 LOAD_CONST              33 (<code object average_rating_per_search_query, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 364>)
+                462 MAKE_FUNCTION            0
+                464 STORE_NAME              40 (average_rating_per_search_query)
+   
+    376         466 LOAD_CONST              11 ('return')
+                468 LOAD_NAME                9 (pd)
+                470 LOAD_ATTR               38 (DataFrame)
+                480 BUILD_TUPLE              2
+                482 LOAD_CONST              34 (<code object validation_history, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 376>)
+                484 MAKE_FUNCTION            4 (annotations)
+                486 STORE_NAME              41 (validation_history)
+   
+    419         488 LOAD_CONST              35 (<code object searches_comment_counts, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 419>)
+                490 MAKE_FUNCTION            0
+                492 STORE_NAME              42 (searches_comment_counts)
+   
+    439         494 LOAD_CONST              36 (<code object enriched_searches_query, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 439>)
+                496 MAKE_FUNCTION            0
+                498 STORE_NAME              43 (enriched_searches_query)
+   
+    459         500 LOAD_CONST              11 ('return')
+                502 LOAD_NAME                9 (pd)
+                504 LOAD_ATTR               38 (DataFrame)
+                514 BUILD_TUPLE              2
+                516 LOAD_CONST              37 (<code object actor, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 459>)
+                518 MAKE_FUNCTION            4 (annotations)
+                520 STORE_NAME              44 (actor)
+   
+    473         522 LOAD_CONST              11 ('return')
+                524 LOAD_NAME                9 (pd)
+                526 LOAD_ATTR               38 (DataFrame)
+                536 BUILD_TUPLE              2
+                538 LOAD_CONST              38 (<code object buyer, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 473>)
+                540 MAKE_FUNCTION            4 (annotations)
+                542 STORE_NAME              45 (buyer)
+   
+    570         544 LOAD_CONST              27 ('search_uid')
+                546 LOAD_NAME               35 (int)
+                548 BUILD_TUPLE              2
+                550 LOAD_CONST              39 (<code object search_targets, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 570>)
+                552 MAKE_FUNCTION            4 (annotations)
+                554 STORE_NAME              46 (search_targets)
+   
+    704         556 LOAD_CONST              27 ('search_uid')
+                558 LOAD_NAME               35 (int)
+                560 LOAD_CONST              11 ('return')
+                562 LOAD_NAME                9 (pd)
+                564 LOAD_ATTR               38 (DataFrame)
+                574 BUILD_TUPLE              4
+                576 LOAD_CONST              40 (<code object search_comments, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 704>)
+                578 MAKE_FUNCTION            4 (annotations)
+                580 STORE_NAME              47 (search_comments)
+   
+    726         582 LOAD_CONST              27 ('search_uid')
+                584 LOAD_NAME               35 (int)
+                586 LOAD_CONST              11 ('return')
+                588 LOAD_NAME                9 (pd)
+                590 LOAD_ATTR               38 (DataFrame)
+                600 BUILD_TUPLE              4
+                602 LOAD_CONST              41 (<code object event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 726>)
+                604 MAKE_FUNCTION            4 (annotations)
+                606 STORE_NAME              48 (event)
+   
+    738         608 LOAD_CONST              27 ('search_uid')
+                610 LOAD_NAME               35 (int)
+                612 LOAD_CONST              11 ('return')
+                614 LOAD_NAME                9 (pd)
+                616 LOAD_ATTR               38 (DataFrame)
+                626 BUILD_TUPLE              4
+                628 LOAD_CONST              42 (<code object event_history, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 738>)
+                630 MAKE_FUNCTION            4 (annotations)
+                632 STORE_NAME              49 (event_history)
+   
+    768         634 LOAD_CONST              27 ('search_uid')
+                636 LOAD_NAME               35 (int)
+                638 LOAD_CONST              11 ('return')
+                640 LOAD_NAME                9 (pd)
+                642 LOAD_ATTR               38 (DataFrame)
+                652 BUILD_TUPLE              4
+                654 LOAD_CONST              43 (<code object search_criteria_history, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 768>)
+                656 MAKE_FUNCTION            4 (annotations)
+                658 STORE_NAME              50 (search_criteria_history)
+   
+    797         660 LOAD_CONST              44 ('uid')
+                662 LOAD_NAME               35 (int)
+                664 LOAD_CONST              11 ('return')
+                666 LOAD_NAME               16 (ts)
+                668 LOAD_ATTR               28 (models)
+                678 LOAD_ATTR               25 (Search)
+                688 BUILD_TUPLE              4
+                690 LOAD_CONST              45 (<code object find_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 797>)
+                692 MAKE_FUNCTION            4 (annotations)
+                694 STORE_NAME              51 (find_search)
+   
+    821         696 LOAD_CONST              46 ('label')
+                698 LOAD_NAME               32 (str)
+                700 LOAD_CONST              11 ('return')
+                702 LOAD_NAME               16 (ts)
+                704 LOAD_ATTR               28 (models)
+                714 LOAD_ATTR               25 (Search)
+                724 BUILD_TUPLE              4
+                726 LOAD_CONST              47 (<code object find_search_by_label, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 821>)
+                728 MAKE_FUNCTION            4 (annotations)
+                730 STORE_NAME              52 (find_search_by_label)
+   
+    845         732 LOAD_CONST              48 ('searchToken')
+                734 LOAD_NAME               32 (str)
+                736 LOAD_CONST              11 ('return')
+                738 LOAD_NAME               16 (ts)
+                740 LOAD_ATTR               28 (models)
+                750 LOAD_ATTR               25 (Search)
+                760 BUILD_TUPLE              4
+                762 LOAD_CONST              49 (<code object find_search_by_token, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 845>)
+                764 MAKE_FUNCTION            4 (annotations)
+                766 STORE_NAME              53 (find_search_by_token)
+   
+    854         768 LOAD_CONST              50 ('domain')
+                770 LOAD_NAME               32 (str)
+                772 LOAD_CONST              11 ('return')
+                774 LOAD_NAME               22 (Company)
+                776 BUILD_TUPLE              4
+                778 LOAD_CONST              51 (<code object find_company_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 854>)
+                780 MAKE_FUNCTION            4 (annotations)
+                782 STORE_NAME              54 (find_company_by_domain)
+   
+    870         784 LOAD_CONST              52 ('email')
+                786 LOAD_NAME               32 (str)
+                788 LOAD_CONST              11 ('return')
+                790 LOAD_NAME               22 (Company)
+                792 BUILD_TUPLE              4
+                794 LOAD_CONST              53 (<code object find_actor_by_email, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 870>)
+                796 MAKE_FUNCTION            4 (annotations)
+                798 STORE_NAME              55 (find_actor_by_email)
+   
+    886         800 LOAD_CONST              54 ('event_id')
+                802 LOAD_NAME               35 (int)
+                804 LOAD_CONST              11 ('return')
+                806 LOAD_NAME               23 (Event)
+                808 BUILD_TUPLE              4
+                810 LOAD_CONST              55 (<code object find_event_by_id, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 886>)
+                812 MAKE_FUNCTION            4 (annotations)
+                814 STORE_NAME              56 (find_event_by_id)
+   
+    901         816 LOAD_CONST              27 ('search_uid')
+                818 LOAD_NAME               35 (int)
+                820 LOAD_CONST              11 ('return')
+                822 LOAD_NAME               24 (Criteria)
+                824 BUILD_TUPLE              4
+                826 LOAD_CONST              56 (<code object find_search_criteria, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 901>)
+                828 MAKE_FUNCTION            4 (annotations)
+                830 STORE_NAME              57 (find_search_criteria)
+   
+    923         832 LOAD_CONST              13 ('company')
+                834 LOAD_NAME               22 (Company)
+                836 LOAD_CONST              11 ('return')
+                838 LOAD_CONST               1 (None)
+                840 BUILD_TUPLE              4
+                842 LOAD_CONST              57 (<code object update_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 923>)
+                844 MAKE_FUNCTION            4 (annotations)
+                846 STORE_NAME              58 (update_company)
+   
+    952         848 LOAD_CONST              17 ('search')
+                850 LOAD_NAME               25 (Search)
+                852 LOAD_CONST              11 ('return')
+                854 LOAD_CONST               1 (None)
+                856 BUILD_TUPLE              4
+                858 LOAD_CONST              58 (<code object update_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 952>)
+                860 MAKE_FUNCTION            4 (annotations)
+                862 STORE_NAME              59 (update_search)
+   
+    975         864 LOAD_CONST              54 ('event_id')
+                866 LOAD_NAME               35 (int)
+                868 LOAD_CONST              11 ('return')
+                870 LOAD_CONST               1 (None)
+                872 BUILD_TUPLE              4
+                874 LOAD_CONST              59 (<code object mute_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 975>)
+                876 MAKE_FUNCTION            4 (annotations)
+                878 STORE_NAME              60 (mute_event)
+   
+    998         880 LOAD_CONST              60 ('comment_id')
+                882 LOAD_NAME               35 (int)
+                884 LOAD_CONST              11 ('return')
+                886 LOAD_CONST               1 (None)
+                888 BUILD_TUPLE              4
+                890 LOAD_CONST              61 (<code object delete_comment, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 998>)
+                892 MAKE_FUNCTION            4 (annotations)
+                894 STORE_NAME              61 (delete_comment)
+   
+   1009         896 LOAD_CONST              27 ('search_uid')
+                898 LOAD_NAME               35 (int)
+                900 LOAD_CONST              11 ('return')
+                902 LOAD_CONST               1 (None)
+                904 BUILD_TUPLE              4
+                906 LOAD_CONST              62 (<code object reset_inbox, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 1009>)
+                908 MAKE_FUNCTION            4 (annotations)
+                910 STORE_NAME              62 (reset_inbox)
+                912 LOAD_CONST               1 (None)
+                914 RETURN_VALUE
    consts
       0
       None
       ('asdict',)
       ('time',)
       ('Any', 'List')
       ('from_dict',)
       ('load_dotenv',)
       ('helpers',)
       ('connect_with_connector',)
-      ('Actor', 'Company', 'Event', 'EventType', 'Search')
+      ('Actor', 'Company', 'Event', 'Criteria', 'Search')
       'event'
       'return'
       code
          argcount  : 1
          nlocals   : 6
          stacksize : 6
          flags     : 3
@@ -4574,14 +4583,133 @@
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_event_by_id'
          firstlineno 886
          lnotab 0x02013401040554fa2e08160104028201
       code
          argcount  : 1
+         nlocals   : 5
+         stacksize : 7
+         flags     : 3
+         code
+            0x9700740000000000000000000000a00100000000000000000000000000
+            00000000000000a6000000ab00000000000000000035007d0164017d027c
+            01a002000000000000000000000000000000000000000074070000000000
+            00000000006a0400000000000000007c02a6010000ab0100000000000000
+            0064027c006901a6020000ab0200000000000000007d03640064006400a6
+            020000ab02000000000000000001006e0b23003100730477027803590077
+            0101005900010001007c036a05000000000000000064036b020000000072
+            0264005300740d00000000000000000000740f000000000000000000007c
+            03a0080000000000000000000000000000000000000000a6000000ab0000
+            000000000000007c03a00900000000000000000000000000000000000000
+            00a6000000ab000000000000000000a6020000ab020000000000000000a6
+            010000ab0100000000000000007d04741500000000000000000000741600
+            0000000000000000007c04a00c0000000000000000000000000000000000
+            0000006404a6010000ab010000000000000000a6020000ab020000000000
+            0000005300
+         901           0 RESUME                   0
+         
+         903           2 LOAD_GLOBAL              0 (db)
+                      14 LOAD_METHOD              1 (connect)
+                      36 PRECALL                  0
+                      40 CALL                     0
+                      50 BEFORE_WITH
+                      52 STORE_FAST               1 (conn)
+         
+         904          54 LOAD_CONST               1 ("\n                SELECT *\n                FROM event\n                WHERE search_uid = :search_uid\n                AND type = 'criteria'\n                ORDER BY created DESC\n                LIMIT 1\n            ")
+                      56 STORE_FAST               2 (statement)
+         
+         912          58 LOAD_FAST                1 (conn)
+                      60 LOAD_METHOD              2 (execute)
+                      82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+                      94 LOAD_ATTR                4 (text)
+                     104 LOAD_FAST                2 (statement)
+                     106 PRECALL                  1
+                     110 CALL                     1
+                     120 LOAD_CONST               2 ('search_uid')
+                     122 LOAD_FAST                0 (search_uid)
+                     124 BUILD_MAP                1
+                     126 PRECALL                  2
+                     130 CALL                     2
+                     140 STORE_FAST               3 (result)
+         
+         903         142 LOAD_CONST               0 (None)
+                     144 LOAD_CONST               0 (None)
+                     146 LOAD_CONST               0 (None)
+                     148 PRECALL                  2
+                     152 CALL                     2
+                     162 POP_TOP
+                     164 JUMP_FORWARD            11 (to 188)
+                 >>  166 PUSH_EXC_INFO
+                     168 WITH_EXCEPT_START
+                     170 POP_JUMP_FORWARD_IF_TRUE     4 (to 180)
+                     172 RERAISE                  2
+                 >>  174 COPY                     3
+                     176 POP_EXCEPT
+                     178 RERAISE                  1
+                 >>  180 POP_TOP
+                     182 POP_EXCEPT
+                     184 POP_TOP
+                     186 POP_TOP
+         
+         914     >>  188 LOAD_FAST                3 (result)
+                     190 LOAD_ATTR                5 (rowcount)
+                     200 LOAD_CONST               3 (0)
+                     202 COMPARE_OP               2 (==)
+                     208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
+         
+         915         210 LOAD_CONST               0 (None)
+                     212 RETURN_VALUE
+         
+         917     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+                     226 LOAD_GLOBAL             15 (NULL + zip)
+                     238 LOAD_FAST                3 (result)
+                     240 LOAD_METHOD              8 (keys)
+                     262 PRECALL                  0
+                     266 CALL                     0
+                     276 LOAD_FAST                3 (result)
+                     278 LOAD_METHOD              9 (fetchone)
+                     300 PRECALL                  0
+                     304 CALL                     0
+                     314 PRECALL                  2
+                     318 CALL                     2
+                     328 PRECALL                  1
+                     332 CALL                     1
+                     342 STORE_FAST               4 (obj)
+         
+         918         344 LOAD_GLOBAL             21 (NULL + from_dict)
+                     356 LOAD_GLOBAL             22 (Criteria)
+                     368 LOAD_FAST                4 (obj)
+                     370 LOAD_METHOD             12 (get)
+                     392 LOAD_CONST               4 ('data')
+                     394 PRECALL                  1
+                     398 CALL                     1
+                     408 PRECALL                  2
+                     412 CALL                     2
+                     422 RETURN_VALUE
+         ExceptionTable:
+           52 to 140 -> 166 [1] lasti
+           166 to 172 -> 174 [3] lasti
+           180 to 180 -> 174 [3] lasti
+         consts
+            None
+            "\n                SELECT *\n                FROM event\n                WHERE search_uid = :search_uid\n                AND type = 'criteria'\n                ORDER BY created DESC\n                LIMIT 1\n            "
+            'search_uid'
+            0
+            'data'
+         names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'Criteria', 'get')
+         varnames   ('search_uid', 'conn', 'statement', 'result', 'obj')
+         freevars   ()
+         cellvars   ()
+         filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
+         name       'find_search_criteria'
+         firstlineno 901
+         lnotab 0x02023401040854f72e0b160104028201
+      code
+         argcount  : 1
          nlocals   : 3
          stacksize : 12
          flags     : 3
          code
             0x9700740000000000000000000000a00100000000000000000000000000
             00000000000000a6000000ab00000000000000000035007d0164017d027c
             01a002000000000000000000000000000000000000000074070000000000
@@ -4590,71 +4718,71 @@
             000000000000007c006a0800000000000000007c006a0900000000000000
             007415000000000000000000006a0b00000000000000007c006a0c000000
             0000000000a6010000ab01000000000000000064029c06a6020000ab0200
             0000000000000001007c01a00d0000000000000000000000000000000000
             000000a6000000ab0000000000000000000100640064006400a6020000ab
             020000000000000000010064005300230031007304770278035900770101
             0059000100010064005300
-         905           0 RESUME                   0
+         923           0 RESUME                   0
          
-         906           2 LOAD_GLOBAL              0 (db)
+         924           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         907          54 LOAD_CONST               1 ('\n            UPDATE company\n            SET\n                uid = :uid,\n                name = :name,\n                description = :description,\n                source = :source,\n                meta = :meta,\n                updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n            WHERE domain = :domain\n            ')
+         925          54 LOAD_CONST               1 ('\n            UPDATE company\n            SET\n                uid = :uid,\n                name = :name,\n                description = :description,\n                source = :source,\n                meta = :meta,\n                updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n            WHERE domain = :domain\n            ')
                       56 STORE_FAST               2 (statement)
          
-         919          58 LOAD_FAST                1 (conn)
+         937          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         920          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         938          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
          
-         922         120 LOAD_FAST                0 (company)
+         940         120 LOAD_FAST                0 (company)
                      122 LOAD_ATTR                5 (uid)
          
-         923         132 LOAD_FAST                0 (company)
+         941         132 LOAD_FAST                0 (company)
                      134 LOAD_ATTR                6 (name)
          
-         924         144 LOAD_FAST                0 (company)
+         942         144 LOAD_FAST                0 (company)
                      146 LOAD_ATTR                7 (description)
          
-         925         156 LOAD_FAST                0 (company)
+         943         156 LOAD_FAST                0 (company)
                      158 LOAD_ATTR                8 (domain)
          
-         926         168 LOAD_FAST                0 (company)
+         944         168 LOAD_FAST                0 (company)
                      170 LOAD_ATTR                9 (source)
          
-         927         180 LOAD_GLOBAL             21 (NULL + json)
+         945         180 LOAD_GLOBAL             21 (NULL + json)
                      192 LOAD_ATTR               11 (dumps)
                      202 LOAD_FAST                0 (company)
                      204 LOAD_ATTR               12 (meta)
                      214 PRECALL                  1
                      218 CALL                     1
          
-         921         228 LOAD_CONST               2 (('uid', 'name', 'description', 'domain', 'source', 'meta'))
+         939         228 LOAD_CONST               2 (('uid', 'name', 'description', 'domain', 'source', 'meta'))
                      230 BUILD_CONST_KEY_MAP      6
          
-         919         232 PRECALL                  2
+         937         232 PRECALL                  2
                      236 CALL                     2
                      246 POP_TOP
          
-         931         248 LOAD_FAST                1 (conn)
+         949         248 LOAD_FAST                1 (conn)
                      250 LOAD_METHOD             13 (commit)
                      272 PRECALL                  0
                      276 CALL                     0
                      286 POP_TOP
          
-         906         288 LOAD_CONST               0 (None)
+         924         288 LOAD_CONST               0 (None)
                      290 LOAD_CONST               0 (None)
                      292 LOAD_CONST               0 (None)
                      294 PRECALL                  2
                      298 CALL                     2
                      308 POP_TOP
                      310 LOAD_CONST               0 (None)
                      312 RETURN_VALUE
@@ -4681,15 +4809,15 @@
             ('uid', 'name', 'description', 'domain', 'source', 'meta')
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'uid', 'name', 'description', 'domain', 'source', 'json', 'dumps', 'meta', 'commit')
          varnames   ('company', 'conn', 'statement')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'update_company'
-         firstlineno 905
+         firstlineno 923
          lnotab 0x02013401040c180126020c010c010c010c010c0130fa04fe100c28e7
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 7
          flags     : 3
          code
@@ -4699,58 +4827,58 @@
             006a0400000000000000006401a6010000ab010000000000000000740b00
             0000000000000000006a0600000000000000007c006a0700000000000000
             00a6010000ab0100000000000000007c006a08000000000000000064029c
             02a6020000ab02000000000000000001007c01a009000000000000000000
             0000000000000000000000a6000000ab0000000000000000000100640064
             006400a6020000ab02000000000000000001006400530023003100730477
             02780359007701010059000100010064005300
-         934           0 RESUME                   0
+         952           0 RESUME                   0
          
-         935           2 LOAD_GLOBAL              0 (db)
+         953           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         936          54 LOAD_FAST                1 (conn)
+         954          54 LOAD_FAST                1 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         937          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         955          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         938         100 LOAD_CONST               1 ('\n                UPDATE search\n                SET\n                    meta = :meta,\n                    updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n                WHERE uid = :uid\n                ')
+         956         100 LOAD_CONST               1 ('\n                UPDATE search\n                SET\n                    meta = :meta,\n                    updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n                WHERE uid = :uid\n                ')
          
-         937         102 PRECALL                  1
+         955         102 PRECALL                  1
                      106 CALL                     1
          
-         947         116 LOAD_GLOBAL             11 (NULL + json)
+         965         116 LOAD_GLOBAL             11 (NULL + json)
                      128 LOAD_ATTR                6 (dumps)
                      138 LOAD_FAST                0 (search)
                      140 LOAD_ATTR                7 (meta)
                      150 PRECALL                  1
                      154 CALL                     1
          
-         948         164 LOAD_FAST                0 (search)
+         966         164 LOAD_FAST                0 (search)
                      166 LOAD_ATTR                8 (uid)
          
-         946         176 LOAD_CONST               2 (('meta', 'uid'))
+         964         176 LOAD_CONST               2 (('meta', 'uid'))
                      178 BUILD_CONST_KEY_MAP      2
          
-         936         180 PRECALL                  2
+         954         180 PRECALL                  2
                      184 CALL                     2
                      194 POP_TOP
          
-         951         196 LOAD_FAST                1 (conn)
+         969         196 LOAD_FAST                1 (conn)
                      198 LOAD_METHOD              9 (commit)
                      220 PRECALL                  0
                      224 CALL                     0
                      234 POP_TOP
          
-         935         236 LOAD_CONST               0 (None)
+         953         236 LOAD_CONST               0 (None)
                      238 LOAD_CONST               0 (None)
                      240 LOAD_CONST               0 (None)
                      242 PRECALL                  2
                      246 CALL                     2
                      256 POP_TOP
                      258 LOAD_CONST               0 (None)
                      260 RETURN_VALUE
@@ -4777,15 +4905,15 @@
             ('meta', 'uid')
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'json', 'dumps', 'meta', 'uid', 'commit')
          varnames   ('search', 'conn')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'update_search'
-         firstlineno 934
+         firstlineno 952
          lnotab 0x020134011801160102ff0e0a30010cfe04f6100f28f0
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 6
          flags     : 3
          code
@@ -4796,61 +4924,61 @@
             006901a6020000ab02000000000000000001007c01a00200000000000000
             000000000000000000000000007407000000000000000000006a04000000
             00000000006403a6010000ab010000000000000000a6010000ab01000000
             000000000001007c01a00500000000000000000000000000000000000000
             00a6000000ab0000000000000000000100640064006400a6020000ab0200
             000000000000000100640053002300310073047702780359007701010059
             000100010064005300
-         957           0 RESUME                   0
+         975           0 RESUME                   0
          
-         959           2 LOAD_GLOBAL              0 (db)
+         977           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         960          54 LOAD_FAST                1 (conn)
+         978          54 LOAD_FAST                1 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         961          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         979          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         962         100 LOAD_CONST               1 ("\n                UPDATE event\n                SET\n                    type = 'mute'\n                WHERE id = :event_id\n                ")
+         980         100 LOAD_CONST               1 ("\n                UPDATE event\n                SET\n                    type = 'mute'\n                WHERE id = :event_id\n                ")
          
-         961         102 PRECALL                  1
+         979         102 PRECALL                  1
                      106 CALL                     1
          
-         970         116 LOAD_CONST               2 ('event_id')
+         988         116 LOAD_CONST               2 ('event_id')
                      118 LOAD_FAST                0 (event_id)
          
-         969         120 BUILD_MAP                1
+         987         120 BUILD_MAP                1
          
-         960         122 PRECALL                  2
+         978         122 PRECALL                  2
                      126 CALL                     2
                      136 POP_TOP
          
-         973         138 LOAD_FAST                1 (conn)
+         991         138 LOAD_FAST                1 (conn)
                      140 LOAD_METHOD              2 (execute)
                      162 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                      174 LOAD_ATTR                4 (text)
                      184 LOAD_CONST               3 ('REFRESH MATERIALIZED VIEW comment')
                      186 PRECALL                  1
                      190 CALL                     1
                      200 PRECALL                  1
                      204 CALL                     1
                      214 POP_TOP
          
-         974         216 LOAD_FAST                1 (conn)
+         992         216 LOAD_FAST                1 (conn)
                      218 LOAD_METHOD              5 (commit)
                      240 PRECALL                  0
                      244 CALL                     0
                      254 POP_TOP
          
-         959         256 LOAD_CONST               0 (None)
+         977         256 LOAD_CONST               0 (None)
                      258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 PRECALL                  2
                      266 CALL                     2
                      276 POP_TOP
                      278 LOAD_CONST               0 (None)
                      280 RETURN_VALUE
@@ -4878,15 +5006,15 @@
             'REFRESH MATERIALIZED VIEW comment'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'commit')
          varnames   ('event_id', 'conn')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'mute_event'
-         firstlineno 957
+         firstlineno 975
          lnotab 0x020234011801160102ff0e0904ff02f7100d4e0128f1
       'comment_id'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 6
          flags     : 3
@@ -4898,78 +5026,78 @@
             0064027c006901a6020000ab02000000000000000001007c01a002000000
             00000000000000000000000000000000007407000000000000000000006a
             0400000000000000006403a6010000ab010000000000000000a6010000ab
             01000000000000000001007c01a005000000000000000000000000000000
             0000000000a6000000ab0000000000000000000100640064006400a60200
             00ab02000000000000000001006400530023003100730477027803590077
             01010059000100010064005300
-         980           0 RESUME                   0
+          998           0 RESUME                   0
          
-         981           2 LOAD_GLOBAL              0 (db)
-                      14 LOAD_METHOD              1 (connect)
-                      36 PRECALL                  0
-                      40 CALL                     0
-                      50 BEFORE_WITH
-                      52 STORE_FAST               1 (conn)
-         
-         982          54 LOAD_CONST               1 ('\n                DELETE FROM event\n                WHERE id = :comment_id\n            ')
-                      56 STORE_FAST               2 (statement)
-         
-         986          58 LOAD_FAST                1 (conn)
-                      60 LOAD_METHOD              2 (execute)
-                      82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
-                      94 LOAD_ATTR                4 (text)
-                     104 LOAD_FAST                2 (statement)
-                     106 PRECALL                  1
-                     110 CALL                     1
-                     120 LOAD_CONST               2 ('comment_id')
-                     122 LOAD_FAST                0 (comment_id)
-                     124 BUILD_MAP                1
-                     126 PRECALL                  2
-                     130 CALL                     2
-                     140 POP_TOP
+          999           2 LOAD_GLOBAL              0 (db)
+                       14 LOAD_METHOD              1 (connect)
+                       36 PRECALL                  0
+                       40 CALL                     0
+                       50 BEFORE_WITH
+                       52 STORE_FAST               1 (conn)
          
-         987         142 LOAD_FAST                1 (conn)
-                     144 LOAD_METHOD              2 (execute)
-                     166 LOAD_GLOBAL              7 (NULL + sqlalchemy)
-                     178 LOAD_ATTR                4 (text)
-                     188 LOAD_CONST               3 ('REFRESH MATERIALIZED VIEW comment')
-                     190 PRECALL                  1
-                     194 CALL                     1
-                     204 PRECALL                  1
-                     208 CALL                     1
-                     218 POP_TOP
-         
-         988         220 LOAD_FAST                1 (conn)
-                     222 LOAD_METHOD              5 (commit)
-                     244 PRECALL                  0
-                     248 CALL                     0
-                     258 POP_TOP
+         1000          54 LOAD_CONST               1 ('\n                DELETE FROM event\n                WHERE id = :comment_id\n            ')
+                       56 STORE_FAST               2 (statement)
          
-         981         260 LOAD_CONST               0 (None)
-                     262 LOAD_CONST               0 (None)
-                     264 LOAD_CONST               0 (None)
-                     266 PRECALL                  2
-                     270 CALL                     2
-                     280 POP_TOP
-                     282 LOAD_CONST               0 (None)
-                     284 RETURN_VALUE
-                 >>  286 PUSH_EXC_INFO
-                     288 WITH_EXCEPT_START
-                     290 POP_JUMP_FORWARD_IF_TRUE     4 (to 300)
-                     292 RERAISE                  2
-                 >>  294 COPY                     3
-                     296 POP_EXCEPT
-                     298 RERAISE                  1
-                 >>  300 POP_TOP
-                     302 POP_EXCEPT
-                     304 POP_TOP
-                     306 POP_TOP
-                     308 LOAD_CONST               0 (None)
-                     310 RETURN_VALUE
+         1004          58 LOAD_FAST                1 (conn)
+                       60 LOAD_METHOD              2 (execute)
+                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+                       94 LOAD_ATTR                4 (text)
+                      104 LOAD_FAST                2 (statement)
+                      106 PRECALL                  1
+                      110 CALL                     1
+                      120 LOAD_CONST               2 ('comment_id')
+                      122 LOAD_FAST                0 (comment_id)
+                      124 BUILD_MAP                1
+                      126 PRECALL                  2
+                      130 CALL                     2
+                      140 POP_TOP
+         
+         1005         142 LOAD_FAST                1 (conn)
+                      144 LOAD_METHOD              2 (execute)
+                      166 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+                      178 LOAD_ATTR                4 (text)
+                      188 LOAD_CONST               3 ('REFRESH MATERIALIZED VIEW comment')
+                      190 PRECALL                  1
+                      194 CALL                     1
+                      204 PRECALL                  1
+                      208 CALL                     1
+                      218 POP_TOP
+         
+         1006         220 LOAD_FAST                1 (conn)
+                      222 LOAD_METHOD              5 (commit)
+                      244 PRECALL                  0
+                      248 CALL                     0
+                      258 POP_TOP
+         
+          999         260 LOAD_CONST               0 (None)
+                      262 LOAD_CONST               0 (None)
+                      264 LOAD_CONST               0 (None)
+                      266 PRECALL                  2
+                      270 CALL                     2
+                      280 POP_TOP
+                      282 LOAD_CONST               0 (None)
+                      284 RETURN_VALUE
+                  >>  286 PUSH_EXC_INFO
+                      288 WITH_EXCEPT_START
+                      290 POP_JUMP_FORWARD_IF_TRUE     4 (to 300)
+                      292 RERAISE                  2
+                  >>  294 COPY                     3
+                      296 POP_EXCEPT
+                      298 RERAISE                  1
+                  >>  300 POP_TOP
+                      302 POP_EXCEPT
+                      304 POP_TOP
+                      306 POP_TOP
+                      308 LOAD_CONST               0 (None)
+                      310 RETURN_VALUE
          ExceptionTable:
            52 to 258 -> 286 [1] lasti
            286 to 292 -> 294 [3] lasti
            300 to 300 -> 294 [3] lasti
          consts
             None
             '\n                DELETE FROM event\n                WHERE id = :comment_id\n            '
@@ -4977,15 +5105,15 @@
             'REFRESH MATERIALIZED VIEW comment'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'commit')
          varnames   ('comment_id', 'conn', 'statement')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'delete_comment'
-         firstlineno 980
+         firstlineno 998
          lnotab 0x02013401040454014e0128f9
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 6
          flags     : 3
          code
@@ -4998,71 +5126,71 @@
             00000000006403a6010000ab010000000000000000a6010000ab01000000
             000000000001007c01a00200000000000000000000000000000000000000
             007407000000000000000000006a0400000000000000006404a6010000ab
             010000000000000000a6010000ab01000000000000000001007c01a00500
             00000000000000000000000000000000000000a6000000ab000000000000
             0000000100640064006400a6020000ab0200000000000000000100640053
             002300310073047702780359007701010059000100010064005300
-          991           0 RESUME                   0
+         1009           0 RESUME                   0
          
-          995           2 LOAD_GLOBAL              0 (db)
+         1013           2 LOAD_GLOBAL              0 (db)
                        14 LOAD_METHOD              1 (connect)
                        36 PRECALL                  0
                        40 CALL                     0
                        50 BEFORE_WITH
                        52 STORE_FAST               1 (conn)
          
-          996          54 LOAD_FAST                1 (conn)
+         1014          54 LOAD_FAST                1 (conn)
                        56 LOAD_METHOD              2 (execute)
          
-          997          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         1015          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                        90 LOAD_ATTR                4 (text)
          
-          998         100 LOAD_CONST               1 ("\n                DELETE FROM event\n                WHERE search_uid = :search_uid\n                and type = 'create'\n                ")
+         1016         100 LOAD_CONST               1 ("\n                DELETE FROM event\n                WHERE search_uid = :search_uid\n                and type = 'create'\n                ")
          
-          997         102 PRECALL                  1
+         1015         102 PRECALL                  1
                       106 CALL                     1
          
-         1004         116 LOAD_CONST               2 ('search_uid')
+         1022         116 LOAD_CONST               2 ('search_uid')
                       118 LOAD_FAST                0 (search_uid)
                       120 BUILD_MAP                1
          
-          996         122 PRECALL                  2
+         1014         122 PRECALL                  2
                       126 CALL                     2
                       136 POP_TOP
          
-         1006         138 LOAD_FAST                1 (conn)
+         1024         138 LOAD_FAST                1 (conn)
                       140 LOAD_METHOD              2 (execute)
                       162 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       174 LOAD_ATTR                4 (text)
                       184 LOAD_CONST               3 ('REFRESH MATERIALIZED VIEW comment')
                       186 PRECALL                  1
                       190 CALL                     1
                       200 PRECALL                  1
                       204 CALL                     1
                       214 POP_TOP
          
-         1007         216 LOAD_FAST                1 (conn)
+         1025         216 LOAD_FAST                1 (conn)
                       218 LOAD_METHOD              2 (execute)
                       240 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       252 LOAD_ATTR                4 (text)
                       262 LOAD_CONST               4 ('REFRESH MATERIALIZED VIEW rating')
                       264 PRECALL                  1
                       268 CALL                     1
                       278 PRECALL                  1
                       282 CALL                     1
                       292 POP_TOP
          
-         1010         294 LOAD_FAST                1 (conn)
+         1028         294 LOAD_FAST                1 (conn)
                       296 LOAD_METHOD              5 (commit)
                       318 PRECALL                  0
                       322 CALL                     0
                       332 POP_TOP
          
-          995         334 LOAD_CONST               0 (None)
+         1013         334 LOAD_CONST               0 (None)
                       336 LOAD_CONST               0 (None)
                       338 LOAD_CONST               0 (None)
                       340 PRECALL                  2
                       344 CALL                     2
                       354 POP_TOP
                       356 LOAD_CONST               0 (None)
                       358 RETURN_VALUE
@@ -5091,23 +5219,23 @@
             'REFRESH MATERIALIZED VIEW rating'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'commit')
          varnames   ('search_uid', 'conn')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'reset_inbox'
-         firstlineno 991
+         firstlineno 1009
          lnotab 0x020434011801160102ff0e0706f8100a4e014e0328f1
       (True, None, 'create')
-   names      ('hashlib', 'json', 'dataclasses', 'asdict', 'time', 'typing', 'Any', 'List', 'pandas', 'pd', 'sqlalchemy', 'dacite', 'from_dict', 'dotenv', 'load_dotenv', 'gandai', 'ts', 'helpers', 'gandai.db', 'connect_with_connector', 'gandai.models', 'Actor', 'Company', 'Event', 'EventType', 'Search', 'db', 'insert_event', 'models', 'insert_company', 'insert_actor', 'insert_search', 'str', 'important_targets_from_search', 'important_targets_from_event', 'int', 'bool', 'insert_companies_as_targets', 'DataFrame', 'searches_query', 'average_rating_per_search_query', 'validation_history', 'searches_comment_counts', 'enriched_searches_query', 'actor', 'buyer', 'search_targets', 'search_comments', 'event', 'event_history', 'search_criteria_history', 'find_search', 'find_search_by_label', 'find_search_by_token', 'find_company_by_domain', 'find_actor_by_email', 'find_event_by_id', 'update_company', 'update_search', 'mute_event', 'delete_comment', 'reset_inbox')
+   names      ('hashlib', 'json', 'dataclasses', 'asdict', 'time', 'typing', 'Any', 'List', 'pandas', 'pd', 'sqlalchemy', 'dacite', 'from_dict', 'dotenv', 'load_dotenv', 'gandai', 'ts', 'helpers', 'gandai.db', 'connect_with_connector', 'gandai.models', 'Actor', 'Company', 'Event', 'Criteria', 'Search', 'db', 'insert_event', 'models', 'insert_company', 'insert_actor', 'insert_search', 'str', 'important_targets_from_search', 'important_targets_from_event', 'int', 'bool', 'insert_companies_as_targets', 'DataFrame', 'searches_query', 'average_rating_per_search_query', 'validation_history', 'searches_comment_counts', 'enriched_searches_query', 'actor', 'buyer', 'search_targets', 'search_comments', 'event', 'event_history', 'search_criteria_history', 'find_search', 'find_search_by_label', 'find_search_by_token', 'find_company_by_domain', 'find_actor_by_email', 'find_event_by_id', 'find_search_criteria', 'update_company', 'update_search', 'mute_event', 'delete_comment', 'reset_inbox')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff0201080108010c010c011002080108010c010c02140208010c010c
       011c021406101e240e100f1010020116ff020116ff020102ff020202fe08
       3d244e0201020102fa04010eff020202fe020302fd020402fc020502fb02
       0602fa020702f908611620060c162b06140614160e16610c7f00071a161a
-      0c1a1e1a1d241824182409101010101013101d10171017100b
+      0c1a1e1a1d24182418240910101010100f1016101d10171017100b
```

### Comparing `gandai-1.7.62/gandai/__pycache__/secrets.cpython-311.pyc` & `gandai-1.7.63/gandai/__pycache__/secrets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.62/gandai/__pycache__/services.cpython-311.pyc` & `gandai-1.7.63/gandai/__pycache__/services.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.62/gandai/__pycache__/sources.cpython-311.pyc` & `gandai-1.7.63/gandai/__pycache__/sources.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.62/gandai/__pycache__/tasks.cpython-311.pyc` & `gandai-1.7.63/gandai/__pycache__/tasks.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.62/gandai/analytics.py` & `gandai-1.7.63/gandai/analytics.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.62/gandai/constants.py` & `gandai-1.7.63/gandai/constants.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.62/gandai/db.py` & `gandai-1.7.63/gandai/db.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.62/gandai/google.py` & `gandai-1.7.63/gandai/google.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.62/gandai/gpt.py` & `gandai-1.7.63/gandai/gpt.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.62/gandai/grata.py` & `gandai-1.7.63/gandai/grata.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,122 +5,120 @@
 HEADERS = {
     "Authorization": secrets.access_secret_version("GRATA_API_TOKEN"),
     "Content-Type": "application/json",
 }
 
 
 def find_similar(domain: str, search: models.Search) -> list:
-    api_filters = {
+    api_filters = _get_api_filter(search)
+    similiar_filters = {
         "domain": domain,
+        "grata_employees_estimates_range": api_filters[
+            "grata_employees_estimates_range"
+        ],
+        "headquarters": api_filters["headquarters"],
+        "ownership": api_filters["ownership"],
+        "exclude": api_filters["exclude"],
     }
-    # similiar_filters = {
-    #     "domain": domain,
-    #     "grata_employees_estimates_range": api_filters[
-    #         "grata_employees_estimates_range"
-    #     ],
-    #     "headquarters": api_filters["headquarters"],
-    #     "ownership": api_filters["ownership"],
-    #     "exclude": api_filters["exclude"],
-    # }
     # print(similiar_filters)
     response = requests.post(
         "https://search.grata.com/api/v1.3/search-similar/",
         headers=HEADERS,
-        json=api_filters,
+        json=similiar_filters,
     )
     data = response.json()
     # print("find_similar:", data)
     data["companies"] = data.get("results", [])  # asking grata about this
 
     return data["companies"]
 
 
-# def find_by_criteria(search: models.Search) -> list:
-#     # rethink this
-#     # consider handling "25 skipped", etc
-
-#     pages = search.criteria.result_count / 25
-#     companies = []
-#     api_filters = _get_api_filter(search)
-
-#     def _find_by_criteria(api_filters: dict, page_token=None) -> dict:
-#         if page_token:
-#             api_filters["page_token"] = page_token
-#         response = requests.post(
-#             "https://search.grata.com/api/v1.3/search/",
-#             headers=HEADERS,
-#             json=api_filters,
-#         )
-#         data = response.json()
-#         return data
-
-#     print(api_filters)
-#     resp = _find_by_criteria(api_filters)
-#     page_token = resp.get("page_token")
-#     companies.extend(resp.get("companies", []))
-#     if pages > 1:
-#         for _ in range(1, int(pages)):
-#             resp = _find_by_criteria(api_filters, page_token)
-#             companies.extend(resp.get("companies", []))
-#             page_token = resp.get("page_token")
-#             if not page_token:
-#                 break
+def find_by_criteria(search: models.Search) -> list:
+    # rethink this
+    # consider handling "25 skipped", etc
+
+    pages = search.criteria.result_count / 25
+    companies = []
+    api_filters = _get_api_filter(search)
+
+    def _find_by_criteria(api_filters: dict, page_token=None) -> dict:
+        if page_token:
+            api_filters["page_token"] = page_token
+        response = requests.post(
+            "https://search.grata.com/api/v1.3/search/",
+            headers=HEADERS,
+            json=api_filters,
+        )
+        data = response.json()
+        return data
+
+    print(api_filters)
+    resp = _find_by_criteria(api_filters)
+    page_token = resp.get("page_token")
+    companies.extend(resp.get("companies", []))
+    if pages > 1:
+        for _ in range(1, int(pages)):
+            resp = _find_by_criteria(api_filters, page_token)
+            companies.extend(resp.get("companies", []))
+            page_token = resp.get("page_token")
+            if not page_token:
+                break
 
-#     # should I return last page token?
-#     return companies
+    # should I return last page token?
+    return companies
 
 
 def enrich(domain: str) -> dict:
     response = requests.post(
         "https://search.grata.com/api/v1.3/enrich/",
         headers=HEADERS,
         json={"domain": domain},
     )
     data = response.json()
     data["linkedin"] = data.get("social_linkedin")
     data["ownership"] = data.get("ownership_status")
     return data
 
 
-# def _get_api_filter(search: models.Search) -> dict:
-#     def _hq_include() -> list:
-#         hq_include = []
-#         cities = search.criteria.inclusion.city
-#         states = search.criteria.inclusion.state
-#         countries = search.criteria.inclusion.country
-
-#         if len(cities) > 0:
-#             # front-end validates only one state when city selected
-#             state = ts.constants.STATES[states[0]]
-#             for city in cities:
-#                 hq_include.append(
-#                     {"city": city, "state": state, "country": "United States"}
-#                 )
-#             return hq_include
-
-#         if len(states) > 0:
-#             for state in states:
-#                 hq_include.append({"state": ts.constants.STATES[state]})
-#         elif len(countries) > 0:
-#             for country in countries:
-#                 hq_include.append({"country": ts.constants.COUNTRIES[country]})
-#         return hq_include
-
-#     def _hq_exclude() -> list:
-#         hq_exclude = []
-#         for state in search.criteria.exclusion.state:
-#             hq_exclude.append({"state": ts.constants.STATES[state]})
-#         return hq_exclude
-
-#     api_filters = {
-#         "op": search.criteria.operator,
-#         "include": search.criteria.inclusion.keywords,
-#         "exclude": search.criteria.exclusion.keywords,
-#         "grata_employees_estimates_range": search.criteria.inclusion.employees_range,
-#         "ownership": search.criteria.inclusion.ownership,
-#         "headquarters": {
-#             "include": _hq_include(),
-#             "exclude": _hq_exclude(),
-#         },
-#     }
-#     # print(api_filters)
-#     return api_filters
+def _get_api_filter(search: models.Search) -> dict:
+    def _hq_include() -> list:
+        hq_include = []
+        cities = search.criteria.inclusion.city
+        states = search.criteria.inclusion.state
+        countries = search.criteria.inclusion.country
+
+        if len(cities) > 0:
+            # front-end validates only one state when city selected
+            state = ts.constants.STATES[states[0]]
+            for city in cities:
+                hq_include.append(
+                    {"city": city, "state": state, "country": "United States"}
+                )
+            return hq_include
+
+        if len(states) > 0:
+            for state in states:
+                hq_include.append({"state": ts.constants.STATES[state]})
+        elif len(countries) > 0:
+            for country in countries:
+                hq_include.append({"country": ts.constants.COUNTRIES[country]})
+        return hq_include
+
+    def _hq_exclude() -> list:
+        hq_exclude = []
+        for state in search.criteria.exclusion.state:
+            hq_exclude.append({"state": ts.constants.STATES[state]})
+        return hq_exclude
+
+    api_filters = {
+        "op": search.criteria.operator,
+        "include": search.criteria.inclusion.keywords,
+        "exclude": search.criteria.exclusion.keywords,
+        "grata_employees_estimates_range": search.criteria.inclusion.employees_range,
+        "ownership": search.criteria.inclusion.ownership,
+        "headquarters": {
+            "include": _hq_include(),
+            "exclude": _hq_exclude(),
+        },
+    }
+    # print(api_filters)
+    return api_filters
```

### Comparing `gandai-1.7.62/gandai/helpers.py` & `gandai-1.7.63/gandai/helpers.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.62/gandai/main.py` & `gandai-1.7.63/gandai/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,36 +42,38 @@
     print(updates)
     company.meta = {**company.meta, **updates}
     # this is where I could also make a comment
     ts.query.update_company(company)
 
 
 def run_similarity_search(search: ts.models.Search, domain: str) -> None:
+    search.criteria = ts.query.find_search_criteria(search_uid=search.uid)
     grata_companies = ts.grata.find_similar(domain=domain, search=search)
     ts.query.insert_companies_as_targets(
         companies=grata_companies,
         search_uid=search.uid,
         actor_key="grata",
         # force=True # ok
         source=f"grata/{domain}",
         stage="similar",
     )
 
 
-# def run_criteria_search(search: ts.models.Search) -> None:
-#     # don't have to pass the event because the criteria
-#     # is the event that we're responding to
-#     grata_companies = ts.grata.find_by_criteria(search)
-#     ts.query.insert_companies_as_targets(
-#         companies=grata_companies,
-#         search_uid=search.uid,
-#         actor_key="grata",
-#         force=True,
-#         source="grata",
-#     )
+def run_criteria_search(search: ts.models.Search, event: ts.models.Event) -> None:
+    # don't have to pass the event because the criteria
+    # is the event that we're responding to
+    search.criteria = from_dict(ts.models.Criteria, event.data)
+    grata_companies = ts.grata.find_by_criteria(search)
+    ts.query.insert_companies_as_targets(
+        companies=grata_companies,
+        search_uid=search.uid,
+        actor_key="grata",
+        force=True,
+        source="grata",
+    )
 
 
 def run_maps_search(search: ts.models.Search, event: ts.models.Event) -> None:
     existing_search_domains = ts.query.search_targets(search_uid=search.uid)[
         "domain"
     ].to_list()
 
@@ -126,52 +128,14 @@
         companies=results[["domain", "description"]].to_dict(orient="records"),
         search_uid=event.search_uid,
         actor_key=event.actor_key,
         source="Google",
     )
 
 
-# def run_gpt_grata_search(search: ts.models.Search, event: ts.models.Event) -> None:
-#     HEADERS = {
-#         "Authorization": secrets.access_secret_version("GRATA_API_TOKEN"),
-#         "Content-Type": "application/json",
-#     }
-
-#     messages = [
-#         {"role": "system", "content": ts.gpt.HOW_TO_SEARCH_GRATA_API},
-#         {
-#             "role": "user",
-#             "content": event.data["prompt"],
-#         },
-#     ]
-
-#     api_filters: dict = ts.gpt.ask_gpt4(messages, temperature=0.5)
-
-#     response = requests.post(
-#         "https://search.grata.com/api/v1.3/search/",
-#         headers=HEADERS,
-#         json={
-#             "include": api_filters["include"],
-#             "exclude": api_filters["exclude"],
-#             "grata_employees_estimates_range": api_filters[
-#                 "grata_employees_estimates_range"
-#             ],
-#             "headquarters": {
-#                 "include": api_filters["headquarters"]["include"],
-#                 "exclude": api_filters["headquarters"]["exclude"],
-#             },
-#         },
-#     )
-#     data = response.json()
-#     ts.query.insert_companies_as_targets(
-#         companies=data["companies"],
-#         search_uid=search.uid,
-#         actor_key="grata",
-#         source="gpt_grata",
-#     )
 
 
 def handle_prompt(event: ts.models.Event) -> None:
     print("prompt event:", event)
     messages = [
         {
             "role": "system",
@@ -308,17 +272,17 @@
         pass
 
     elif event.type == "enrich":
         run_enrichment(event=event)
     ## actions
     elif event.type == "prompt":
         handle_prompt(event=event)
-    # elif event.type == "criteria":
-    #     if len(event.data["inclusion"]["keywords"]) > 0:
-    #         run_criteria_search(search=search)
+    elif event.type == "criteria":
+        if len(event.data["inclusion"]["keywords"]) > 0:
+            run_criteria_search(search=search, event=event)
     elif event.type == "maps":
         run_maps_search(search=search, event=event)
     elif event.type == "google":
         run_google_search(search=search, event=event)
 
     elif event.type == "grata_search":
         run_google_search(search=search, event=event)
```

### Comparing `gandai-1.7.62/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc` & `gandai-1.7.63/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.62/gandai/migrations/db_seed.py` & `gandai-1.7.63/gandai/migrations/db_seed.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.62/gandai/migrations/dealcloud.py` & `gandai-1.7.63/gandai/migrations/dealcloud.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.62/gandai/migrations/sql/230818-alter.sql` & `gandai-1.7.63/gandai/migrations/sql/230818-alter.sql`

 * *Files identical despite different names*

### Comparing `gandai-1.7.62/gandai/migrations/sql/schema.sql` & `gandai-1.7.63/gandai/migrations/sql/schema.sql`

 * *Files identical despite different names*

### Comparing `gandai-1.7.62/gandai/models.py` & `gandai-1.7.63/gandai/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
 
 
 @dataclass
 class Search:
     uid: int  # foreign key, dealcloud id
     label: str  # maps to dealcloud engagement name
     meta: dict = field(default_factory=dict)
-    # criteria: Criteria = field(default_factory=Criteria)
+    criteria: Criteria = field(default_factory=Criteria)
     # maps: Maps = field(default_factory=Maps)
 
     # uh what are these for?
     @property
     def notes(self) -> str:
         return self.meta.get("notes", None)
```

### Comparing `gandai-1.7.62/gandai/query.py` & `gandai-1.7.63/gandai/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from dotenv import load_dotenv
 
 load_dotenv()
 
 import gandai as ts
 from gandai import helpers
 from gandai.db import connect_with_connector
-from gandai.models import Actor, Company, Event, EventType, Search
+from gandai.models import Actor, Company, Event, Criteria, Search
 
 db = connect_with_connector()
 
 
 ### WRITES ###
 
 
@@ -894,14 +894,32 @@
         # obj = dict(zip(result.keys(), result.fetchone()))
     if result.rowcount == 0:
         return None
     else:
         obj = dict(zip(result.keys(), result.fetchone()))
         return from_dict(Event, obj)
 
+def find_search_criteria(search_uid: int) -> Criteria:
+    ## finds last criteria event
+    with db.connect() as conn:
+        statement = """
+                SELECT *
+                FROM event
+                WHERE search_uid = :search_uid
+                AND type = 'criteria'
+                ORDER BY created DESC
+                LIMIT 1
+            """
+        result = conn.execute(sqlalchemy.text(statement), {"search_uid": search_uid})
+        # obj = dict(zip(result.keys(), result.fetchone()))
+    if result.rowcount == 0:
+        return None
+    else:
+        obj = dict(zip(result.keys(), result.fetchone()))
+        return from_dict(Criteria, obj.get("data"))
 
 ### UPDATE ###
 
 
 def update_company(company: Company) -> None:
     with db.connect() as conn:
         statement = """
```

### Comparing `gandai-1.7.62/gandai/secrets.py` & `gandai-1.7.63/gandai/secrets.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.62/gandai/tasks.py` & `gandai-1.7.63/gandai/tasks.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.62/gandai.egg-info/SOURCES.txt` & `gandai-1.7.63/gandai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

