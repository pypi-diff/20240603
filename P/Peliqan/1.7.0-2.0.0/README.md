# Comparing `tmp/Peliqan-1.7.0.tar.gz` & `tmp/Peliqan-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Peliqan-1.7.0.tar", last modified: Wed May 29 07:24:54 2024, max compression
+gzip compressed data, was "Peliqan-2.0.0.tar", last modified: Mon Jun  3 11:52:31 2024, max compression
```

## Comparing `Peliqan-1.7.0.tar` & `Peliqan-2.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-05-29 07:24:54.341915 Peliqan-1.7.0/
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      665 2024-05-29 07:24:54.341761 Peliqan-1.7.0/PKG-INFO
-drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-05-29 07:24:54.334356 Peliqan-1.7.0/Peliqan.egg-info/
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      665 2024-05-29 07:24:54.000000 Peliqan-1.7.0/Peliqan.egg-info/PKG-INFO
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      437 2024-05-29 07:24:54.000000 Peliqan-1.7.0/Peliqan.egg-info/SOURCES.txt
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)        1 2024-05-29 07:24:54.000000 Peliqan-1.7.0/Peliqan.egg-info/dependency_links.txt
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       16 2024-05-29 07:24:54.000000 Peliqan-1.7.0/Peliqan.egg-info/requires.txt
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)        8 2024-05-29 07:24:54.000000 Peliqan-1.7.0/Peliqan.egg-info/top_level.txt
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1411 2023-08-02 11:35:09.000000 Peliqan-1.7.0/README.md
-drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-05-29 07:24:54.338492 Peliqan-1.7.0/peliqan/
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      872 2024-05-29 07:07:44.000000 Peliqan-1.7.0/peliqan/__init__.py
-drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-05-29 07:24:54.341338 Peliqan-1.7.0/peliqan/client/
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      421 2024-05-13 13:01:35.000000 Peliqan-1.7.0/peliqan/client/__init__.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    20269 2024-05-28 11:39:58.000000 Peliqan-1.7.0/peliqan/client/backend_service.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1743 2024-05-20 14:08:33.000000 Peliqan-1.7.0/peliqan/client/base.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    11515 2024-05-28 13:06:11.000000 Peliqan-1.7.0/peliqan/client/dbclient.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      928 2024-05-13 13:01:35.000000 Peliqan-1.7.0/peliqan/client/sftpclient.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     4549 2024-05-13 13:01:35.000000 Peliqan-1.7.0/peliqan/client/writeback.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    33371 2024-05-29 06:20:55.000000 Peliqan-1.7.0/peliqan/core.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      393 2024-05-10 06:48:15.000000 Peliqan-1.7.0/peliqan/exceptions.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    20342 2024-03-21 07:17:47.000000 Peliqan-1.7.0/peliqan/local_test.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1118 2024-05-20 14:08:33.000000 Peliqan-1.7.0/peliqan/utils.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       38 2024-05-29 07:24:54.341988 Peliqan-1.7.0/setup.cfg
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1371 2024-05-10 06:48:22.000000 Peliqan-1.7.0/setup.py
+drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-06-03 11:52:31.096014 Peliqan-2.0.0/
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      665 2024-06-03 11:52:31.095856 Peliqan-2.0.0/PKG-INFO
+drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-06-03 11:52:31.090538 Peliqan-2.0.0/Peliqan.egg-info/
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      665 2024-06-03 11:52:30.000000 Peliqan-2.0.0/Peliqan.egg-info/PKG-INFO
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      437 2024-06-03 11:52:30.000000 Peliqan-2.0.0/Peliqan.egg-info/SOURCES.txt
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)        1 2024-06-03 11:52:30.000000 Peliqan-2.0.0/Peliqan.egg-info/dependency_links.txt
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       16 2024-06-03 11:52:30.000000 Peliqan-2.0.0/Peliqan.egg-info/requires.txt
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)        8 2024-06-03 11:52:30.000000 Peliqan-2.0.0/Peliqan.egg-info/top_level.txt
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1411 2023-08-02 11:35:09.000000 Peliqan-2.0.0/README.md
+drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-06-03 11:52:31.092861 Peliqan-2.0.0/peliqan/
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      872 2024-06-03 11:52:24.000000 Peliqan-2.0.0/peliqan/__init__.py
+drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-06-03 11:52:31.095380 Peliqan-2.0.0/peliqan/client/
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      421 2024-05-13 13:01:35.000000 Peliqan-2.0.0/peliqan/client/__init__.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    20284 2024-06-03 11:11:07.000000 Peliqan-2.0.0/peliqan/client/backend_service.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1743 2024-05-20 14:08:33.000000 Peliqan-2.0.0/peliqan/client/base.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    11515 2024-05-31 07:15:43.000000 Peliqan-2.0.0/peliqan/client/dbclient.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      928 2024-05-13 13:01:35.000000 Peliqan-2.0.0/peliqan/client/sftpclient.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     4549 2024-05-13 13:01:35.000000 Peliqan-2.0.0/peliqan/client/writeback.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    35557 2024-06-03 11:50:12.000000 Peliqan-2.0.0/peliqan/core.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      393 2024-05-10 06:48:15.000000 Peliqan-2.0.0/peliqan/exceptions.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    20342 2024-03-21 07:17:47.000000 Peliqan-2.0.0/peliqan/local_test.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1118 2024-05-31 07:15:43.000000 Peliqan-2.0.0/peliqan/utils.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       38 2024-06-03 11:52:31.096094 Peliqan-2.0.0/setup.cfg
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1371 2024-05-10 06:48:22.000000 Peliqan-2.0.0/setup.py
```

### Comparing `Peliqan-1.7.0/PKG-INFO` & `Peliqan-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Peliqan
-Version: 1.7.0
+Version: 2.0.0
 Summary: This package is an sdk that allows any python client to connect with a Peliqan environment.
 Home-page: https://peliqan.io/
 Author: Peliqan.io
 Author-email: dev@peliqan.io
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Peliqan-1.7.0/Peliqan.egg-info/PKG-INFO` & `Peliqan-2.0.0/Peliqan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Peliqan
-Version: 1.7.0
+Version: 2.0.0
 Summary: This package is an sdk that allows any python client to connect with a Peliqan environment.
 Home-page: https://peliqan.io/
 Author: Peliqan.io
 Author-email: dev@peliqan.io
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Peliqan-1.7.0/README.md` & `Peliqan-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `Peliqan-1.7.0/peliqan/__init__.py` & `Peliqan-2.0.0/peliqan/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.7.0"
+__version__ = "2.0.0"
 __author__ = 'Peliqan.io'
 __credits__ = 'Peliqan.io'
 
 __all__ = [
     "Peliqan",
     "BasePeliqanClient"
 ]
```

### Comparing `Peliqan-1.7.0/peliqan/client/backend_service.py` & `Peliqan-2.0.0/peliqan/client/backend_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -368,15 +368,15 @@
     def get_table(self, table_id):
         url = f"{self.BACKEND_URL}/api/database/tables/{table_id}/"
         response_dict = self.call_backend("get", url)
         return response_dict
 
     def create_query(
         self,
-        name,
+        table_name,
         query,
         database_id=None,
         schema_id=None,
         run_on_peliqan_trino=empty,
         materialize=empty
     ):
         url = f"{self.BACKEND_URL}/api/database/tables/create-sql-query/"
@@ -386,37 +386,37 @@
 
         if database_id:
             url = f"{self.BACKEND_URL}/api/database/tables/database/{database_id}/"
 
         data = {
             'table_type': 'query',
             'schema_id': schema_id,
-            'name': name,
+            'name': table_name,
             'query': query
         }
 
         response_dict = self.call_backend("post", url, json=data)
 
-        if run_on_peliqan_trino is True or materialize is True:
+        if run_on_peliqan_trino != empty or materialize != empty:
             response_dict = self.update_table(
                 response_dict['id'],
                 run_on_peliqan_trino=run_on_peliqan_trino,
                 materialize=materialize,
             )
 
         return response_dict
 
     def update_table(
         self,
         table_id,
         name=None,
         query=None,
         settings=None,
+        run_on_peliqan_trino=empty,
         materialize=empty,
-        run_on_peliqan_trino=empty
     ):
         url = f"{self.BACKEND_URL}/api/database/tables/%s/" % table_id
         data = {}
 
         if name:
             data['name'] = name
```

### Comparing `Peliqan-1.7.0/peliqan/client/base.py` & `Peliqan-2.0.0/peliqan/client/base.py`

 * *Files identical despite different names*

### Comparing `Peliqan-1.7.0/peliqan/client/dbclient.py` & `Peliqan-2.0.0/peliqan/client/dbclient.py`

 * *Files identical despite different names*

### Comparing `Peliqan-1.7.0/peliqan/client/sftpclient.py` & `Peliqan-2.0.0/peliqan/client/sftpclient.py`

 * *Files identical despite different names*

### Comparing `Peliqan-1.7.0/peliqan/client/writeback.py` & `Peliqan-2.0.0/peliqan/client/writeback.py`

 * *Files identical despite different names*

### Comparing `Peliqan-1.7.0/peliqan/core.py` & `Peliqan-2.0.0/peliqan/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -506,15 +506,15 @@
         :param materialize: optional, boolean,  whether the query should be materialized as a table into a database.
 
         :return: result of update
         """
 
         update_result_dict = {}
         update_metadata_result_dict = {}
-        if name or query or settings:
+        if name or query or settings or run_on_peliqan_trino != empty or materialize != empty:
             update_result_dict = self.__service_client__.update_table(
                 table_id,
                 name,
                 query,
                 settings,
                 run_on_peliqan_trino,
                 materialize
@@ -618,23 +618,23 @@
             name=name,
             type=script_type,
             run_mode=run_mode
         )
 
     def add_query_table(
         self,
-        name,
+        table_name,
         query,
         database_id=None,
         schema_id=None,
         run_on_peliqan_trino=empty,
         materialize=empty,
     ):
         return self.__service_client__.create_query(
-            name=name,
+            table_name=table_name,
             query=query,
             database_id=database_id,
             schema_id=schema_id,
             run_on_peliqan_trino=run_on_peliqan_trino,
             materialize=materialize
         )
 
@@ -766,54 +766,105 @@
             recipient,
             subject,
             message,
             confirmation_recipient,
             server_type
         )
 
-    def get_or_create_schema(self, database_id, schema_name):
+    def get_or_create_schema(self, schema_name, database_name=None, database_id=None):
+        if not database_id and not database_name:
+            raise PeliqanClientException("'database_name' or 'database_id' must be provided.")
+
+        if not database_id and database_name:
+            response = self.find_resource('database', resource_name=database_name)
+            database_id = response['database_id']
+
         try:
             url = f"{self.BACKEND_URL}/api/database/schemas/database/{database_id}/"
             response = self.__service_client__.call_backend("POST", url, json={'schema_name': schema_name})
         except PeliqanClientException as e:
             if 'ERROR_SCHEMA_ALREADY_EXISTS' not in str(e):
                 raise
+
             response = self.__service_client__.find_schema(database_id=database_id, schema_name=schema_name)
             schema_id = response.get('schema_id')
             if schema_id:
                 response = self.get_schema(schema_id)
 
         return response
 
-    def get_or_create_query_table(
+    def upsert_query_table(
         self,
-        name,
+        table_name,
         query,
-        database_id=None,
         schema_id=None,
+        schema_name=None,
+        database_id=None,
+        database_name=None,
         run_on_peliqan_trino=empty,
         materialize=empty
     ):
+
+        if not database_id and not database_name and not schema_id and not schema_name:
+            schema_name = "My Queries"  # default `My Queries` schema in database
+            # todo: database_id = self.DW_ID
+
         try:
             response = self.__service_client__.find_table_or_field(
                 database_id=database_id,
+                database_name=database_name,
                 schema_id=schema_id,
-                table_name=name
+                schema_name=schema_name,
+                table_name=table_name
             )
 
             table_id = response.get('table_id')
             if table_id:
-                response = self.get_table(table_id)
+                response = self.update_table(
+                    table_id,
+                    name=table_name,
+                    query=query,
+                    run_on_peliqan_trino=run_on_peliqan_trino,
+                    materialize=materialize
+                )
 
         except PeliqanClientException as e:
             if 'ERROR_TABLE_DOES_NOT_EXIST' not in str(e):
                 raise
 
+            if not database_id and database_name:
+                try:
+                    response = self.find_resource('database', resource_name=database_name)
+                    database_id = response['database_id']
+                except PeliqanClientException as e:
+                    if (
+                        'ERROR_APPLICATION_DOES_NOT_EXIST' not in str(e) or
+                        "ERROR_DATABASE_DOES_NOT_EXIST" not in str(e)
+                    ):
+                        raise
+
+            if not schema_id and schema_name:
+                try:
+                    response = self.find_resource(
+                        'schema',
+                        resource_name=schema_name,
+                        database_name=database_name,
+                        database_id=database_id
+                    )
+                    schema_id = response['schema_id']
+
+                except PeliqanClientException as e:
+                    if 'ERROR_SCHEMA_DOES_NOT_EXIST' not in str(e):
+                        raise
+
+                    response = self.get_or_create_schema(schema_name, database_id=database_id)
+                    schema_id = response['id']
+
             response = self.add_query_table(
-                name,
+                table_name,
                 query,
                 database_id=database_id,
                 schema_id=schema_id,
                 run_on_peliqan_trino=run_on_peliqan_trino,
                 materialize=materialize,
             )
```

### Comparing `Peliqan-1.7.0/peliqan/local_test.py` & `Peliqan-2.0.0/peliqan/local_test.py`

 * *Files identical despite different names*

### Comparing `Peliqan-1.7.0/peliqan/utils.py` & `Peliqan-2.0.0/peliqan/utils.py`

 * *Files identical despite different names*

### Comparing `Peliqan-1.7.0/setup.py` & `Peliqan-2.0.0/setup.py`

 * *Files identical despite different names*

