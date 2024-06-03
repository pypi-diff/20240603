# Comparing `tmp/general_operator-0.1.2.tar.gz` & `tmp/general_operator-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "general_operator-0.1.2.tar", last modified: Wed May 15 07:58:18 2024, max compression
+gzip compressed data, was "general_operator-0.1.3.tar", last modified: Mon Jun  3 07:26:40 2024, max compression
```

## Comparing `general_operator-0.1.2.tar` & `general_operator-0.1.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-15 07:58:18.086251 general_operator-0.1.2/
--rw-r--r--   0 wilson08   (501) staff       (20)     3477 2024-05-15 07:58:18.086053 general_operator-0.1.2/PKG-INFO
--rwxr-xr-x   0 wilson08   (501) staff       (20)     2551 2024-05-13 03:26:40.000000 general_operator-0.1.2/README.md
-drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-15 07:58:18.080410 general_operator-0.1.2/general_operator/
--rw-r--r--   0 wilson08   (501) staff       (20)        0 2024-05-13 03:34:24.000000 general_operator-0.1.2/general_operator/__init__.py
-drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-15 07:58:18.083875 general_operator-0.1.2/general_operator/app/
-drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-15 07:58:18.084141 general_operator-0.1.2/general_operator/app/SQL/
--rwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-11 09:53:05.000000 general_operator-0.1.2/general_operator/app/SQL/__init__.py
--rwxr-xr-x   0 wilson08   (501) staff       (20)      884 2024-05-13 03:26:40.000000 general_operator-0.1.2/general_operator/app/SQL/database.py
--rwxr-xr-x   0 wilson08   (501) staff       (20)     4410 2024-05-13 03:26:40.000000 general_operator-0.1.2/general_operator/app/SQL/sql_operate.py
--rw-r--r--   0 wilson08   (501) staff       (20)        0 2024-05-13 03:37:18.000000 general_operator-0.1.2/general_operator/app/__init__.py
-drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-15 07:58:18.084441 general_operator-0.1.2/general_operator/app/influxdb/
--rw-r--r--   0 wilson08   (501) staff       (20)        0 2024-05-11 09:53:05.000000 general_operator-0.1.2/general_operator/app/influxdb/__init__.py
--rw-r--r--   0 wilson08   (501) staff       (20)      664 2024-05-13 03:26:40.000000 general_operator-0.1.2/general_operator/app/influxdb/influxdb.py
--rw-r--r--   0 wilson08   (501) staff       (20)     1382 2024-05-13 03:26:40.000000 general_operator-0.1.2/general_operator/app/influxdb/influxdb_operate.py
-drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-15 07:58:18.084737 general_operator-0.1.2/general_operator/app/redis_db/
--rw-r--r--   0 wilson08   (501) staff       (20)        0 2024-05-11 09:53:05.000000 general_operator-0.1.2/general_operator/app/redis_db/__init__.py
--rw-r--r--   0 wilson08   (501) staff       (20)     1088 2024-05-13 03:26:40.000000 general_operator-0.1.2/general_operator/app/redis_db/redis.py
--rw-r--r--   0 wilson08   (501) staff       (20)     6306 2024-05-13 03:26:40.000000 general_operator-0.1.2/general_operator/app/redis_db/redis_operate.py
-drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-15 07:58:18.085013 general_operator-0.1.2/general_operator/dependencies/
--rw-r--r--   0 wilson08   (501) staff       (20)        0 2024-05-13 03:43:10.000000 general_operator-0.1.2/general_operator/dependencies/__init__.py
--rwxr-xr-x   0 wilson08   (501) staff       (20)      167 2024-05-11 09:53:05.000000 general_operator-0.1.2/general_operator/dependencies/db_dependencies.py
--rwxr-xr-x   0 wilson08   (501) staff       (20)     1178 2024-05-13 06:05:37.000000 general_operator-0.1.2/general_operator/dependencies/get_query_dependencies.py
-drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-15 07:58:18.085494 general_operator-0.1.2/general_operator/function/
--rw-r--r--   0 wilson08   (501) staff       (20)    11029 2024-05-13 03:50:09.000000 general_operator-0.1.2/general_operator/function/General_operate.py
--rw-r--r--   0 wilson08   (501) staff       (20)        0 2024-05-13 03:38:18.000000 general_operator-0.1.2/general_operator/function/__init__.py
--rw-r--r--   0 wilson08   (501) staff       (20)     1147 2024-05-13 03:26:40.000000 general_operator-0.1.2/general_operator/function/create_data_structure.py
--rwxr-xr-x   0 wilson08   (501) staff       (20)      157 2024-05-13 03:26:40.000000 general_operator-0.1.2/general_operator/function/exception.py
--rw-r--r--   0 wilson08   (501) staff       (20)     1878 2024-05-11 09:53:05.000000 general_operator-0.1.2/general_operator/function/search_function.py
-drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-15 07:58:18.085722 general_operator-0.1.2/general_operator/routers/
--rw-r--r--   0 wilson08   (501) staff       (20)     4726 2024-05-13 06:04:34.000000 general_operator-0.1.2/general_operator/routers/General_table_router.py
--rw-r--r--   0 wilson08   (501) staff       (20)        0 2024-05-13 03:45:41.000000 general_operator-0.1.2/general_operator/routers/__init__.py
-drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-15 07:58:18.085840 general_operator-0.1.2/general_operator.egg-info/
--rw-r--r--   0 wilson08   (501) staff       (20)     3477 2024-05-15 07:58:18.000000 general_operator-0.1.2/general_operator.egg-info/PKG-INFO
--rw-r--r--   0 wilson08   (501) staff       (20)     1106 2024-05-15 07:58:18.000000 general_operator-0.1.2/general_operator.egg-info/SOURCES.txt
--rw-r--r--   0 wilson08   (501) staff       (20)        1 2024-05-15 07:58:18.000000 general_operator-0.1.2/general_operator.egg-info/dependency_links.txt
--rw-r--r--   0 wilson08   (501) staff       (20)       72 2024-05-15 07:58:18.000000 general_operator-0.1.2/general_operator.egg-info/requires.txt
--rw-r--r--   0 wilson08   (501) staff       (20)       17 2024-05-15 07:58:18.000000 general_operator-0.1.2/general_operator.egg-info/top_level.txt
--rw-r--r--   0 wilson08   (501) staff       (20)       38 2024-05-15 07:58:18.086285 general_operator-0.1.2/setup.cfg
--rw-r--r--   0 wilson08   (501) staff       (20)     1341 2024-05-15 07:57:19.000000 general_operator-0.1.2/setup.py
+drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-06-03 07:26:40.369599 general_operator-0.1.3/
+-rw-r--r--   0 wilson08   (501) staff       (20)     3477 2024-06-03 07:26:40.369336 general_operator-0.1.3/PKG-INFO
+-rwxr-xr-x   0 wilson08   (501) staff       (20)     2551 2024-05-13 03:26:40.000000 general_operator-0.1.3/README.md
+drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-06-03 07:26:40.365934 general_operator-0.1.3/general_operator/
+-rw-r--r--   0 wilson08   (501) staff       (20)        0 2024-05-13 03:34:24.000000 general_operator-0.1.3/general_operator/__init__.py
+drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-06-03 07:26:40.366754 general_operator-0.1.3/general_operator/app/
+drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-06-03 07:26:40.367019 general_operator-0.1.3/general_operator/app/SQL/
+-rwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-11 09:53:05.000000 general_operator-0.1.3/general_operator/app/SQL/__init__.py
+-rwxr-xr-x   0 wilson08   (501) staff       (20)      884 2024-05-13 03:26:40.000000 general_operator-0.1.3/general_operator/app/SQL/database.py
+-rwxr-xr-x   0 wilson08   (501) staff       (20)     4410 2024-05-13 03:26:40.000000 general_operator-0.1.3/general_operator/app/SQL/sql_operate.py
+-rw-r--r--   0 wilson08   (501) staff       (20)        0 2024-05-13 03:37:18.000000 general_operator-0.1.3/general_operator/app/__init__.py
+drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-06-03 07:26:40.367363 general_operator-0.1.3/general_operator/app/influxdb/
+-rw-r--r--   0 wilson08   (501) staff       (20)        0 2024-05-11 09:53:05.000000 general_operator-0.1.3/general_operator/app/influxdb/__init__.py
+-rw-r--r--   0 wilson08   (501) staff       (20)      664 2024-05-13 03:26:40.000000 general_operator-0.1.3/general_operator/app/influxdb/influxdb.py
+-rw-r--r--   0 wilson08   (501) staff       (20)     1382 2024-05-13 03:26:40.000000 general_operator-0.1.3/general_operator/app/influxdb/influxdb_operate.py
+drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-06-03 07:26:40.367722 general_operator-0.1.3/general_operator/app/redis_db/
+-rw-r--r--   0 wilson08   (501) staff       (20)        0 2024-05-11 09:53:05.000000 general_operator-0.1.3/general_operator/app/redis_db/__init__.py
+-rw-r--r--   0 wilson08   (501) staff       (20)     1303 2024-06-03 07:26:10.000000 general_operator-0.1.3/general_operator/app/redis_db/redis.py
+-rw-r--r--   0 wilson08   (501) staff       (20)     6306 2024-05-13 03:26:40.000000 general_operator-0.1.3/general_operator/app/redis_db/redis_operate.py
+drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-06-03 07:26:40.368022 general_operator-0.1.3/general_operator/dependencies/
+-rw-r--r--   0 wilson08   (501) staff       (20)        0 2024-05-13 03:43:10.000000 general_operator-0.1.3/general_operator/dependencies/__init__.py
+-rwxr-xr-x   0 wilson08   (501) staff       (20)      167 2024-05-11 09:53:05.000000 general_operator-0.1.3/general_operator/dependencies/db_dependencies.py
+-rwxr-xr-x   0 wilson08   (501) staff       (20)     1178 2024-05-13 06:05:37.000000 general_operator-0.1.3/general_operator/dependencies/get_query_dependencies.py
+drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-06-03 07:26:40.368649 general_operator-0.1.3/general_operator/function/
+-rw-r--r--   0 wilson08   (501) staff       (20)    11029 2024-05-13 03:50:09.000000 general_operator-0.1.3/general_operator/function/General_operate.py
+-rw-r--r--   0 wilson08   (501) staff       (20)        0 2024-05-13 03:38:18.000000 general_operator-0.1.3/general_operator/function/__init__.py
+-rw-r--r--   0 wilson08   (501) staff       (20)     1147 2024-05-13 03:26:40.000000 general_operator-0.1.3/general_operator/function/create_data_structure.py
+-rwxr-xr-x   0 wilson08   (501) staff       (20)      157 2024-05-13 03:26:40.000000 general_operator-0.1.3/general_operator/function/exception.py
+-rw-r--r--   0 wilson08   (501) staff       (20)     1878 2024-05-11 09:53:05.000000 general_operator-0.1.3/general_operator/function/search_function.py
+drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-06-03 07:26:40.368926 general_operator-0.1.3/general_operator/routers/
+-rw-r--r--   0 wilson08   (501) staff       (20)     4726 2024-05-13 06:04:34.000000 general_operator-0.1.3/general_operator/routers/General_table_router.py
+-rw-r--r--   0 wilson08   (501) staff       (20)        0 2024-05-13 03:45:41.000000 general_operator-0.1.3/general_operator/routers/__init__.py
+drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-06-03 07:26:40.369037 general_operator-0.1.3/general_operator.egg-info/
+-rw-r--r--   0 wilson08   (501) staff       (20)     3477 2024-06-03 07:26:40.000000 general_operator-0.1.3/general_operator.egg-info/PKG-INFO
+-rw-r--r--   0 wilson08   (501) staff       (20)     1106 2024-06-03 07:26:40.000000 general_operator-0.1.3/general_operator.egg-info/SOURCES.txt
+-rw-r--r--   0 wilson08   (501) staff       (20)        1 2024-06-03 07:26:40.000000 general_operator-0.1.3/general_operator.egg-info/dependency_links.txt
+-rw-r--r--   0 wilson08   (501) staff       (20)       72 2024-06-03 07:26:40.000000 general_operator-0.1.3/general_operator.egg-info/requires.txt
+-rw-r--r--   0 wilson08   (501) staff       (20)       17 2024-06-03 07:26:40.000000 general_operator-0.1.3/general_operator.egg-info/top_level.txt
+-rw-r--r--   0 wilson08   (501) staff       (20)       38 2024-06-03 07:26:40.369659 general_operator-0.1.3/setup.cfg
+-rw-r--r--   0 wilson08   (501) staff       (20)     1341 2024-06-03 07:26:10.000000 general_operator-0.1.3/setup.py
```

### Comparing `general_operator-0.1.2/PKG-INFO` & `general_operator-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: general_operator
-Version: 0.1.2
+Version: 0.1.3
 Summary: general operator for fastapi write sql and redis
 Home-page: https://github.com/littlebluewhite/node_object_module
 Author: wilson
 Author-email: wwilson008@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `general_operator-0.1.2/README.md` & `general_operator-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `general_operator-0.1.2/general_operator/app/SQL/database.py` & `general_operator-0.1.3/general_operator/app/SQL/database.py`

 * *Files identical despite different names*

### Comparing `general_operator-0.1.2/general_operator/app/SQL/sql_operate.py` & `general_operator-0.1.3/general_operator/app/SQL/sql_operate.py`

 * *Files identical despite different names*

### Comparing `general_operator-0.1.2/general_operator/app/influxdb/influxdb.py` & `general_operator-0.1.3/general_operator/app/influxdb/influxdb.py`

 * *Files identical despite different names*

### Comparing `general_operator-0.1.2/general_operator/app/influxdb/influxdb_operate.py` & `general_operator-0.1.3/general_operator/app/influxdb/influxdb_operate.py`

 * *Files identical despite different names*

### Comparing `general_operator-0.1.2/general_operator/app/redis_db/redis_operate.py` & `general_operator-0.1.3/general_operator/app/redis_db/redis_operate.py`

 * *Files identical despite different names*

### Comparing `general_operator-0.1.2/general_operator/dependencies/get_query_dependencies.py` & `general_operator-0.1.3/general_operator/dependencies/get_query_dependencies.py`

 * *Files identical despite different names*

### Comparing `general_operator-0.1.2/general_operator/function/General_operate.py` & `general_operator-0.1.3/general_operator/function/General_operate.py`

 * *Files identical despite different names*

### Comparing `general_operator-0.1.2/general_operator/function/create_data_structure.py` & `general_operator-0.1.3/general_operator/function/create_data_structure.py`

 * *Files identical despite different names*

### Comparing `general_operator-0.1.2/general_operator/function/search_function.py` & `general_operator-0.1.3/general_operator/function/search_function.py`

 * *Files identical despite different names*

### Comparing `general_operator-0.1.2/general_operator/routers/General_table_router.py` & `general_operator-0.1.3/general_operator/routers/General_table_router.py`

 * *Files identical despite different names*

### Comparing `general_operator-0.1.2/general_operator.egg-info/PKG-INFO` & `general_operator-0.1.3/general_operator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: general_operator
-Version: 0.1.2
+Version: 0.1.3
 Summary: general operator for fastapi write sql and redis
 Home-page: https://github.com/littlebluewhite/node_object_module
 Author: wilson
 Author-email: wwilson008@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `general_operator-0.1.2/general_operator.egg-info/SOURCES.txt` & `general_operator-0.1.3/general_operator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `general_operator-0.1.2/setup.py` & `general_operator-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='general_operator',
-    version='0.1.2',
+    version='0.1.3',
     packages=['general_operator', 'general_operator.app', 'general_operator.app.SQL', 'general_operator.app.influxdb',
               'general_operator.app.redis_db', 'general_operator.dependencies', 'general_operator.function', 'general_operator.routers',],
     install_requires=[
         'fastapi>=0.83.0',
         'influxdb-client>=1.22.0',
         'redis>=5.0.1',
         'SQLAlchemy>=2.0.10'
```

