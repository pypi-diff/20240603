# Comparing `tmp/witchcraft-0.3.0.tar.gz` & `tmp/witchcraft-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "witchcraft-0.3.0.tar", last modified: Thu Feb 29 08:56:20 2024, max compression
+gzip compressed data, was "witchcraft-0.3.1.tar", last modified: Mon Jun  3 09:11:25 2024, max compression
```

## Comparing `witchcraft-0.3.0.tar` & `witchcraft-0.3.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 pfacka    (1000) pfacka    (1000)        0 2024-02-29 08:56:20.198628 witchcraft-0.3.0/
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)     1113 2023-09-08 11:00:49.000000 witchcraft-0.3.0/LICENSE
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)       58 2023-09-08 11:00:49.000000 witchcraft-0.3.0/MANIFEST.in
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)      625 2024-02-29 08:56:20.198628 witchcraft-0.3.0/PKG-INFO
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)      716 2023-09-08 11:00:49.000000 witchcraft-0.3.0/README.md
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)       38 2024-02-29 08:56:20.198628 witchcraft-0.3.0/setup.cfg
--rwxr-xr-x   0 pfacka    (1000) pfacka    (1000)     1008 2024-02-29 08:56:16.000000 witchcraft-0.3.0/setup.py
-drwxr-xr-x   0 pfacka    (1000) pfacka    (1000)        0 2024-02-29 08:56:20.190628 witchcraft-0.3.0/test/
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)     1917 2023-09-08 11:00:52.000000 witchcraft-0.3.0/test/test.py
-drwxr-xr-x   0 pfacka    (1000) pfacka    (1000)        0 2024-02-29 08:56:20.190628 witchcraft-0.3.0/witchcraft/
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)     7276 2023-09-08 11:00:49.000000 witchcraft-0.3.0/witchcraft/__init__.py
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)    14718 2023-09-12 12:44:46.000000 witchcraft-0.3.0/witchcraft/combinators.py
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)     2384 2023-11-30 22:34:31.000000 witchcraft-0.3.0/witchcraft/connection.py
-drwxr-xr-x   0 pfacka    (1000) pfacka    (1000)        0 2024-02-29 08:56:20.194628 witchcraft-0.3.0/witchcraft/dateutil/
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)       46 2023-09-08 11:00:49.000000 witchcraft-0.3.0/witchcraft/dateutil/__init__.py
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)     2611 2023-09-08 11:00:49.000000 witchcraft-0.3.0/witchcraft/dateutil/easter.py
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)    51227 2023-09-08 11:00:49.000000 witchcraft-0.3.0/witchcraft/dateutil/parser.py
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)    21509 2023-09-08 11:00:49.000000 witchcraft-0.3.0/witchcraft/dateutil/relativedelta.py
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)    61599 2023-09-08 11:00:49.000000 witchcraft-0.3.0/witchcraft/dateutil/rrule.py
-drwxr-xr-x   0 pfacka    (1000) pfacka    (1000)        0 2024-02-29 08:56:20.194628 witchcraft-0.3.0/witchcraft/dateutil/tz/
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)      145 2023-09-08 11:00:49.000000 witchcraft-0.3.0/witchcraft/dateutil/tz/__init__.py
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)      461 2023-09-08 11:00:49.000000 witchcraft-0.3.0/witchcraft/dateutil/tz/_common.py
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)    33867 2023-09-08 11:00:49.000000 witchcraft-0.3.0/witchcraft/dateutil/tz/tz.py
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)    11143 2023-09-08 11:00:49.000000 witchcraft-0.3.0/witchcraft/dateutil/tz/win.py
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)       58 2023-09-08 11:00:49.000000 witchcraft-0.3.0/witchcraft/dateutil/tzwin.py
-drwxr-xr-x   0 pfacka    (1000) pfacka    (1000)        0 2024-02-29 08:56:20.198628 witchcraft-0.3.0/witchcraft/queries/
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)       75 2023-09-08 11:00:49.000000 witchcraft-0.3.0/witchcraft/queries/psql_add_column.sql
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)      389 2024-02-29 08:30:07.000000 witchcraft-0.3.0/witchcraft/queries/psql_create_table.sql
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)       38 2023-09-08 11:00:49.000000 witchcraft-0.3.0/witchcraft/queries/psql_delete.sql
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)     1267 2023-09-08 11:00:49.000000 witchcraft-0.3.0/witchcraft/queries/psql_discover_columns.sql
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)        0 2023-09-08 11:00:49.000000 witchcraft-0.3.0/witchcraft/queries/psql_discover_load_table_columns.sql
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)       23 2023-09-08 11:00:49.000000 witchcraft-0.3.0/witchcraft/queries/psql_get_timestamp.sql
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)      335 2023-09-08 11:00:49.000000 witchcraft-0.3.0/witchcraft/queries/psql_insert.sql
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)       62 2023-09-08 11:00:49.000000 witchcraft-0.3.0/witchcraft/queries/psql_load_table_add_column.sql
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)       78 2023-09-08 11:00:49.000000 witchcraft-0.3.0/witchcraft/queries/psql_max_version.sql
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)      215 2023-09-08 11:00:49.000000 witchcraft-0.3.0/witchcraft/queries/psql_prepare_load_table.sql
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)     1171 2023-09-08 11:00:49.000000 witchcraft-0.3.0/witchcraft/queries/psql_upsert.sql
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)      349 2023-09-08 11:00:49.000000 witchcraft-0.3.0/witchcraft/queries/psql_upsert_insert.sql
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)      250 2023-09-08 11:00:49.000000 witchcraft-0.3.0/witchcraft/queries/psql_upsert_load.sql
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)      333 2023-09-08 11:00:49.000000 witchcraft-0.3.0/witchcraft/queries/psql_upsert_update.sql
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)     1713 2023-09-08 11:00:49.000000 witchcraft-0.3.0/witchcraft/reserved_psql.txt
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)      562 2023-09-08 11:00:49.000000 witchcraft-0.3.0/witchcraft/stream.py
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)     8912 2024-01-30 22:46:33.000000 witchcraft-0.3.0/witchcraft/template.py
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)      453 2023-09-08 11:00:49.000000 witchcraft-0.3.0/witchcraft/test.py
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)    19821 2023-09-08 11:00:49.000000 witchcraft-0.3.0/witchcraft/upsert.py
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)    14797 2024-01-20 13:00:13.000000 witchcraft-0.3.0/witchcraft/utils.py
-drwxr-xr-x   0 pfacka    (1000) pfacka    (1000)        0 2024-02-29 08:56:20.194628 witchcraft-0.3.0/witchcraft.egg-info/
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)      625 2024-02-29 08:56:20.000000 witchcraft-0.3.0/witchcraft.egg-info/PKG-INFO
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)     1364 2024-02-29 08:56:20.000000 witchcraft-0.3.0/witchcraft.egg-info/SOURCES.txt
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)        1 2024-02-29 08:56:20.000000 witchcraft-0.3.0/witchcraft.egg-info/dependency_links.txt
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)        1 2023-09-08 11:00:49.000000 witchcraft-0.3.0/witchcraft.egg-info/not-zip-safe
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)       70 2024-02-29 08:56:20.000000 witchcraft-0.3.0/witchcraft.egg-info/requires.txt
--rw-r--r--   0 pfacka    (1000) pfacka    (1000)       11 2024-02-29 08:56:20.000000 witchcraft-0.3.0/witchcraft.egg-info/top_level.txt
+drwxr-xr-x   0 pfacka    (1000) pfacka    (1000)        0 2024-06-03 09:11:25.382962 witchcraft-0.3.1/
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)     1113 2023-09-08 11:00:49.000000 witchcraft-0.3.1/LICENSE
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)       58 2023-09-08 11:00:49.000000 witchcraft-0.3.1/MANIFEST.in
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)      625 2024-06-03 09:11:25.382962 witchcraft-0.3.1/PKG-INFO
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)      716 2023-09-08 11:00:49.000000 witchcraft-0.3.1/README.md
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)       38 2024-06-03 09:11:25.382962 witchcraft-0.3.1/setup.cfg
+-rwxr-xr-x   0 pfacka    (1000) pfacka    (1000)     1008 2024-06-03 09:02:15.000000 witchcraft-0.3.1/setup.py
+drwxr-xr-x   0 pfacka    (1000) pfacka    (1000)        0 2024-06-03 09:11:25.370962 witchcraft-0.3.1/test/
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)     1917 2023-09-08 11:00:52.000000 witchcraft-0.3.1/test/test.py
+drwxr-xr-x   0 pfacka    (1000) pfacka    (1000)        0 2024-06-03 09:11:25.374961 witchcraft-0.3.1/witchcraft/
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)     7276 2023-09-08 11:00:49.000000 witchcraft-0.3.1/witchcraft/__init__.py
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)    14718 2023-09-12 12:44:46.000000 witchcraft-0.3.1/witchcraft/combinators.py
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)     2384 2023-11-30 22:34:31.000000 witchcraft-0.3.1/witchcraft/connection.py
+drwxr-xr-x   0 pfacka    (1000) pfacka    (1000)        0 2024-06-03 09:11:25.374961 witchcraft-0.3.1/witchcraft/dateutil/
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)       46 2023-09-08 11:00:49.000000 witchcraft-0.3.1/witchcraft/dateutil/__init__.py
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)     2611 2023-09-08 11:00:49.000000 witchcraft-0.3.1/witchcraft/dateutil/easter.py
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)    51227 2023-09-08 11:00:49.000000 witchcraft-0.3.1/witchcraft/dateutil/parser.py
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)    21509 2023-09-08 11:00:49.000000 witchcraft-0.3.1/witchcraft/dateutil/relativedelta.py
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)    61599 2023-09-08 11:00:49.000000 witchcraft-0.3.1/witchcraft/dateutil/rrule.py
+drwxr-xr-x   0 pfacka    (1000) pfacka    (1000)        0 2024-06-03 09:11:25.378962 witchcraft-0.3.1/witchcraft/dateutil/tz/
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)      145 2023-09-08 11:00:49.000000 witchcraft-0.3.1/witchcraft/dateutil/tz/__init__.py
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)      461 2023-09-08 11:00:49.000000 witchcraft-0.3.1/witchcraft/dateutil/tz/_common.py
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)    33867 2023-09-08 11:00:49.000000 witchcraft-0.3.1/witchcraft/dateutil/tz/tz.py
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)    11143 2023-09-08 11:00:49.000000 witchcraft-0.3.1/witchcraft/dateutil/tz/win.py
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)       58 2023-09-08 11:00:49.000000 witchcraft-0.3.1/witchcraft/dateutil/tzwin.py
+drwxr-xr-x   0 pfacka    (1000) pfacka    (1000)        0 2024-06-03 09:11:25.382962 witchcraft-0.3.1/witchcraft/queries/
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)       75 2023-09-08 11:00:49.000000 witchcraft-0.3.1/witchcraft/queries/psql_add_column.sql
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)      389 2024-02-29 08:30:07.000000 witchcraft-0.3.1/witchcraft/queries/psql_create_table.sql
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)       38 2023-09-08 11:00:49.000000 witchcraft-0.3.1/witchcraft/queries/psql_delete.sql
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)     1267 2023-09-08 11:00:49.000000 witchcraft-0.3.1/witchcraft/queries/psql_discover_columns.sql
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)        0 2023-09-08 11:00:49.000000 witchcraft-0.3.1/witchcraft/queries/psql_discover_load_table_columns.sql
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)       23 2023-09-08 11:00:49.000000 witchcraft-0.3.1/witchcraft/queries/psql_get_timestamp.sql
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)      335 2023-09-08 11:00:49.000000 witchcraft-0.3.1/witchcraft/queries/psql_insert.sql
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)       62 2023-09-08 11:00:49.000000 witchcraft-0.3.1/witchcraft/queries/psql_load_table_add_column.sql
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)       78 2023-09-08 11:00:49.000000 witchcraft-0.3.1/witchcraft/queries/psql_max_version.sql
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)      215 2023-09-08 11:00:49.000000 witchcraft-0.3.1/witchcraft/queries/psql_prepare_load_table.sql
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)     1171 2023-09-08 11:00:49.000000 witchcraft-0.3.1/witchcraft/queries/psql_upsert.sql
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)      349 2023-09-08 11:00:49.000000 witchcraft-0.3.1/witchcraft/queries/psql_upsert_insert.sql
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)      250 2023-09-08 11:00:49.000000 witchcraft-0.3.1/witchcraft/queries/psql_upsert_load.sql
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)      333 2023-09-08 11:00:49.000000 witchcraft-0.3.1/witchcraft/queries/psql_upsert_update.sql
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)     1713 2023-09-08 11:00:49.000000 witchcraft-0.3.1/witchcraft/reserved_psql.txt
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)      562 2023-09-08 11:00:49.000000 witchcraft-0.3.1/witchcraft/stream.py
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)     8912 2024-01-30 22:46:33.000000 witchcraft-0.3.1/witchcraft/template.py
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)      453 2023-09-08 11:00:49.000000 witchcraft-0.3.1/witchcraft/test.py
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)    19869 2024-05-31 08:12:49.000000 witchcraft-0.3.1/witchcraft/upsert.py
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)    14797 2024-01-20 13:00:13.000000 witchcraft-0.3.1/witchcraft/utils.py
+drwxr-xr-x   0 pfacka    (1000) pfacka    (1000)        0 2024-06-03 09:11:25.374961 witchcraft-0.3.1/witchcraft.egg-info/
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)      625 2024-06-03 09:11:25.000000 witchcraft-0.3.1/witchcraft.egg-info/PKG-INFO
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)     1364 2024-06-03 09:11:25.000000 witchcraft-0.3.1/witchcraft.egg-info/SOURCES.txt
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)        1 2024-06-03 09:11:25.000000 witchcraft-0.3.1/witchcraft.egg-info/dependency_links.txt
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)        1 2023-09-08 11:00:49.000000 witchcraft-0.3.1/witchcraft.egg-info/not-zip-safe
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)       70 2024-06-03 09:11:25.000000 witchcraft-0.3.1/witchcraft.egg-info/requires.txt
+-rw-r--r--   0 pfacka    (1000) pfacka    (1000)       11 2024-06-03 09:11:25.000000 witchcraft-0.3.1/witchcraft.egg-info/top_level.txt
```

### Comparing `witchcraft-0.3.0/LICENSE` & `witchcraft-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `witchcraft-0.3.0/PKG-INFO` & `witchcraft-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: witchcraft
-Version: 0.3.0
+Version: 0.3.1
 Home-page: https://github.com/spookyowl/witchcraft
 Author: Peter Facka
 Author-email: pfacka@spookyowl.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `witchcraft-0.3.0/README.md` & `witchcraft-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `witchcraft-0.3.0/setup.py` & `witchcraft-0.3.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name="witchcraft",
-    version="0.3.0",
+    version="0.3.1",
     description='',
     author='Peter Facka',
     author_email='pfacka@spookyowl.com',
     url='https://github.com/spookyowl/witchcraft',
     packages=[
         'witchcraft',
         'witchcraft.dateutil',
```

### Comparing `witchcraft-0.3.0/test/test.py` & `witchcraft-0.3.1/test/test.py`

 * *Files identical despite different names*

### Comparing `witchcraft-0.3.0/witchcraft/__init__.py` & `witchcraft-0.3.1/witchcraft/__init__.py`

 * *Files identical despite different names*

### Comparing `witchcraft-0.3.0/witchcraft/combinators.py` & `witchcraft-0.3.1/witchcraft/combinators.py`

 * *Files identical despite different names*

### Comparing `witchcraft-0.3.0/witchcraft/connection.py` & `witchcraft-0.3.1/witchcraft/connection.py`

 * *Files identical despite different names*

### Comparing `witchcraft-0.3.0/witchcraft/dateutil/easter.py` & `witchcraft-0.3.1/witchcraft/dateutil/easter.py`

 * *Files identical despite different names*

### Comparing `witchcraft-0.3.0/witchcraft/dateutil/parser.py` & `witchcraft-0.3.1/witchcraft/dateutil/parser.py`

 * *Files identical despite different names*

### Comparing `witchcraft-0.3.0/witchcraft/dateutil/relativedelta.py` & `witchcraft-0.3.1/witchcraft/dateutil/relativedelta.py`

 * *Files identical despite different names*

### Comparing `witchcraft-0.3.0/witchcraft/dateutil/rrule.py` & `witchcraft-0.3.1/witchcraft/dateutil/rrule.py`

 * *Files identical despite different names*

### Comparing `witchcraft-0.3.0/witchcraft/dateutil/tz/tz.py` & `witchcraft-0.3.1/witchcraft/dateutil/tz/tz.py`

 * *Files identical despite different names*

### Comparing `witchcraft-0.3.0/witchcraft/dateutil/tz/win.py` & `witchcraft-0.3.1/witchcraft/dateutil/tz/win.py`

 * *Files identical despite different names*

### Comparing `witchcraft-0.3.0/witchcraft/queries/psql_discover_columns.sql` & `witchcraft-0.3.1/witchcraft/queries/psql_discover_columns.sql`

 * *Files identical despite different names*

### Comparing `witchcraft-0.3.0/witchcraft/queries/psql_upsert.sql` & `witchcraft-0.3.1/witchcraft/queries/psql_upsert.sql`

 * *Files identical despite different names*

### Comparing `witchcraft-0.3.0/witchcraft/reserved_psql.txt` & `witchcraft-0.3.1/witchcraft/reserved_psql.txt`

 * *Files identical despite different names*

### Comparing `witchcraft-0.3.0/witchcraft/stream.py` & `witchcraft-0.3.1/witchcraft/stream.py`

 * *Files identical despite different names*

### Comparing `witchcraft-0.3.0/witchcraft/template.py` & `witchcraft-0.3.1/witchcraft/template.py`

 * *Files identical despite different names*

### Comparing `witchcraft-0.3.0/witchcraft/upsert.py` & `witchcraft-0.3.1/witchcraft/upsert.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,14 +290,17 @@
     #TODO: handle decimal=False/True
     #TODO: regexp \s*[-+]?\s*[€$%]?[0-9,\.]\+
     separators = []   
     groups = ['']
     groups_index = 0
     sign = None
 
+    if number_str is None:
+        return None
+
     for c in number_str:
 
         if c in ['.', ',']:
             separators.append(c)
             groups.append('')
             groups_index += 1
```

### Comparing `witchcraft-0.3.0/witchcraft/utils.py` & `witchcraft-0.3.1/witchcraft/utils.py`

 * *Files identical despite different names*

### Comparing `witchcraft-0.3.0/witchcraft.egg-info/PKG-INFO` & `witchcraft-0.3.1/witchcraft.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: witchcraft
-Version: 0.3.0
+Version: 0.3.1
 Home-page: https://github.com/spookyowl/witchcraft
 Author: Peter Facka
 Author-email: pfacka@spookyowl.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `witchcraft-0.3.0/witchcraft.egg-info/SOURCES.txt` & `witchcraft-0.3.1/witchcraft.egg-info/SOURCES.txt`

 * *Files identical despite different names*

