# Comparing `tmp/mongodb_orm-0.1.0.tar.gz` & `tmp/mongodb_orm-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongodb_orm-0.1.0.tar", last modified: Fri May 10 11:48:05 2024, max compression
+gzip compressed data, was "mongodb_orm-0.1.0a1.tar", last modified: Mon Jun  3 08:38:52 2024, max compression
```

## Comparing `mongodb_orm-0.1.0.tar` & `mongodb_orm-0.1.0a1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-10 11:48:05.988526 mongodb_orm-0.1.0/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      331 2024-05-10 11:48:05.987779 mongodb_orm-0.1.0/PKG-INFO
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      565 2024-04-23 13:57:27.000000 mongodb_orm-0.1.0/README.md
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-10 11:48:05.967133 mongodb_orm-0.1.0/mongodb_orm/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       91 2024-04-23 14:47:25.000000 mongodb_orm-0.1.0/mongodb_orm/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      475 2024-04-23 14:25:35.000000 mongodb_orm-0.1.0/mongodb_orm/apps.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-10 11:48:05.970866 mongodb_orm-0.1.0/mongodb_orm/custom_urls/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-18 11:23:58.000000 mongodb_orm-0.1.0/mongodb_orm/custom_urls/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1507 2024-05-03 12:46:06.000000 mongodb_orm-0.1.0/mongodb_orm/custom_urls/bread_urls.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-10 11:48:05.972219 mongodb_orm-0.1.0/mongodb_orm/decorators/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.1.0/mongodb_orm/decorators/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      433 2024-05-10 11:46:02.000000 mongodb_orm-0.1.0/mongodb_orm/decorators/chained.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-10 11:48:05.973426 mongodb_orm-0.1.0/mongodb_orm/exceptions/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.1.0/mongodb_orm/exceptions/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      138 2024-04-04 10:34:42.000000 mongodb_orm-0.1.0/mongodb_orm/exceptions/syntax_exceptions.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-10 11:48:05.976092 mongodb_orm-0.1.0/mongodb_orm/interfaces/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:42.000000 mongodb_orm-0.1.0/mongodb_orm/interfaces/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     2619 2024-04-29 14:42:33.000000 mongodb_orm-0.1.0/mongodb_orm/interfaces/base_mongodb_model.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     7653 2024-05-10 11:46:02.000000 mongodb_orm-0.1.0/mongodb_orm/interfaces/mongodb_model.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      801 2024-04-29 09:28:59.000000 mongodb_orm-0.1.0/mongodb_orm/interfaces/mongodb_model_events.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-10 11:48:05.976769 mongodb_orm-0.1.0/mongodb_orm/management/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:43.000000 mongodb_orm-0.1.0/mongodb_orm/management/__init__.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-10 11:48:05.977567 mongodb_orm-0.1.0/mongodb_orm/management/commands/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.1.0/mongodb_orm/management/commands/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     4559 2024-04-23 15:18:03.000000 mongodb_orm-0.1.0/mongodb_orm/management/commands/update_schema.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-10 11:48:05.978271 mongodb_orm-0.1.0/mongodb_orm/models/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:43.000000 mongodb_orm-0.1.0/mongodb_orm/models/__init__.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-10 11:48:05.979203 mongodb_orm-0.1.0/mongodb_orm/singletons/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.1.0/mongodb_orm/singletons/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      380 2024-04-04 10:34:44.000000 mongodb_orm-0.1.0/mongodb_orm/singletons/mongodb_singleton_client.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-10 11:48:05.983370 mongodb_orm-0.1.0/mongodb_orm/types/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      508 2024-04-04 10:34:44.000000 mongodb_orm-0.1.0/mongodb_orm/types/Relation.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.1.0/mongodb_orm/types/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      128 2024-04-04 10:34:44.000000 mongodb_orm-0.1.0/mongodb_orm/types/index.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      406 2024-05-10 11:46:02.000000 mongodb_orm-0.1.0/mongodb_orm/types/logger_object.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      766 2024-05-10 11:46:02.000000 mongodb_orm-0.1.0/mongodb_orm/types/model_schema.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      368 2024-04-23 15:18:03.000000 mongodb_orm-0.1.0/mongodb_orm/types/options.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      189 2024-05-03 12:47:26.000000 mongodb_orm-0.1.0/mongodb_orm/urls.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-10 11:48:05.984472 mongodb_orm-0.1.0/mongodb_orm/utils/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:11:55.000000 mongodb_orm-0.1.0/mongodb_orm/utils/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1855 2024-05-10 11:47:43.000000 mongodb_orm-0.1.0/mongodb_orm/utils/helpers.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-10 11:48:05.985977 mongodb_orm-0.1.0/mongodb_orm/views/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.1.0/mongodb_orm/views/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     4008 2024-05-10 11:47:43.000000 mongodb_orm-0.1.0/mongodb_orm/views/mongodb_api_model_view.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-10 11:48:05.986914 mongodb_orm-0.1.0/mongodb_orm.egg-info/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      331 2024-05-10 11:48:05.000000 mongodb_orm-0.1.0/mongodb_orm.egg-info/PKG-INFO
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1208 2024-05-10 11:48:05.000000 mongodb_orm-0.1.0/mongodb_orm.egg-info/SOURCES.txt
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        1 2024-05-10 11:48:05.000000 mongodb_orm-0.1.0/mongodb_orm.egg-info/dependency_links.txt
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       35 2024-05-10 11:48:05.000000 mongodb_orm-0.1.0/mongodb_orm.egg-info/requires.txt
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       12 2024-05-10 11:48:05.000000 mongodb_orm-0.1.0/mongodb_orm.egg-info/top_level.txt
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       38 2024-05-10 11:48:05.988678 mongodb_orm-0.1.0/setup.cfg
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      592 2024-05-10 11:47:57.000000 mongodb_orm-0.1.0/setup.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 08:38:52.632655 mongodb_orm-0.1.0a1/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      333 2024-06-03 08:38:52.631445 mongodb_orm-0.1.0a1/PKG-INFO
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      565 2024-04-23 13:57:27.000000 mongodb_orm-0.1.0a1/README.md
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 08:38:52.489707 mongodb_orm-0.1.0a1/mongodb_orm/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       91 2024-04-23 14:47:25.000000 mongodb_orm-0.1.0a1/mongodb_orm/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      475 2024-04-23 14:25:35.000000 mongodb_orm-0.1.0a1/mongodb_orm/apps.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 08:38:52.518637 mongodb_orm-0.1.0a1/mongodb_orm/custom_urls/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-18 11:23:58.000000 mongodb_orm-0.1.0a1/mongodb_orm/custom_urls/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1507 2024-05-03 12:46:06.000000 mongodb_orm-0.1.0a1/mongodb_orm/custom_urls/bread_urls.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 08:38:52.520480 mongodb_orm-0.1.0a1/mongodb_orm/decorators/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.1.0a1/mongodb_orm/decorators/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      433 2024-06-03 08:11:09.000000 mongodb_orm-0.1.0a1/mongodb_orm/decorators/chained.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 08:38:52.524355 mongodb_orm-0.1.0a1/mongodb_orm/exceptions/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.1.0a1/mongodb_orm/exceptions/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      138 2024-04-04 10:34:42.000000 mongodb_orm-0.1.0a1/mongodb_orm/exceptions/syntax_exceptions.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 08:38:52.543078 mongodb_orm-0.1.0a1/mongodb_orm/interfaces/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:42.000000 mongodb_orm-0.1.0a1/mongodb_orm/interfaces/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     2619 2024-04-29 14:42:33.000000 mongodb_orm-0.1.0a1/mongodb_orm/interfaces/base_mongodb_model.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     7789 2024-06-03 08:15:07.000000 mongodb_orm-0.1.0a1/mongodb_orm/interfaces/mongodb_model.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      801 2024-04-29 09:28:59.000000 mongodb_orm-0.1.0a1/mongodb_orm/interfaces/mongodb_model_events.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 08:38:52.544520 mongodb_orm-0.1.0a1/mongodb_orm/management/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:43.000000 mongodb_orm-0.1.0a1/mongodb_orm/management/__init__.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 08:38:52.563054 mongodb_orm-0.1.0a1/mongodb_orm/management/commands/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.1.0a1/mongodb_orm/management/commands/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     4559 2024-04-23 15:18:03.000000 mongodb_orm-0.1.0a1/mongodb_orm/management/commands/update_schema.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 08:38:52.564296 mongodb_orm-0.1.0a1/mongodb_orm/models/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:43.000000 mongodb_orm-0.1.0a1/mongodb_orm/models/__init__.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 08:38:52.568356 mongodb_orm-0.1.0a1/mongodb_orm/singletons/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.1.0a1/mongodb_orm/singletons/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      380 2024-04-04 10:34:44.000000 mongodb_orm-0.1.0a1/mongodb_orm/singletons/mongodb_singleton_client.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 08:38:52.590942 mongodb_orm-0.1.0a1/mongodb_orm/types/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      508 2024-04-04 10:34:44.000000 mongodb_orm-0.1.0a1/mongodb_orm/types/Relation.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.1.0a1/mongodb_orm/types/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      128 2024-04-04 10:34:44.000000 mongodb_orm-0.1.0a1/mongodb_orm/types/index.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      406 2024-06-03 08:11:09.000000 mongodb_orm-0.1.0a1/mongodb_orm/types/logger_object.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      766 2024-06-03 08:11:09.000000 mongodb_orm-0.1.0a1/mongodb_orm/types/model_schema.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      368 2024-04-23 15:18:03.000000 mongodb_orm-0.1.0a1/mongodb_orm/types/options.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      189 2024-05-03 12:47:26.000000 mongodb_orm-0.1.0a1/mongodb_orm/urls.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 08:38:52.609676 mongodb_orm-0.1.0a1/mongodb_orm/utils/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:11:55.000000 mongodb_orm-0.1.0a1/mongodb_orm/utils/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1855 2024-06-03 08:11:09.000000 mongodb_orm-0.1.0a1/mongodb_orm/utils/helpers.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 08:38:52.628345 mongodb_orm-0.1.0a1/mongodb_orm/views/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.1.0a1/mongodb_orm/views/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     4008 2024-05-10 11:47:43.000000 mongodb_orm-0.1.0a1/mongodb_orm/views/mongodb_api_model_view.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 08:38:52.629768 mongodb_orm-0.1.0a1/mongodb_orm.egg-info/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      333 2024-06-03 08:38:52.000000 mongodb_orm-0.1.0a1/mongodb_orm.egg-info/PKG-INFO
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1208 2024-06-03 08:38:52.000000 mongodb_orm-0.1.0a1/mongodb_orm.egg-info/SOURCES.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        1 2024-06-03 08:38:52.000000 mongodb_orm-0.1.0a1/mongodb_orm.egg-info/dependency_links.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       35 2024-06-03 08:38:52.000000 mongodb_orm-0.1.0a1/mongodb_orm.egg-info/requires.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       12 2024-06-03 08:38:52.000000 mongodb_orm-0.1.0a1/mongodb_orm.egg-info/top_level.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       38 2024-06-03 08:38:52.632859 mongodb_orm-0.1.0a1/setup.cfg
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      594 2024-06-03 08:38:36.000000 mongodb_orm-0.1.0a1/setup.py
```

### Comparing `mongodb_orm-0.1.0/README.md` & `mongodb_orm-0.1.0a1/README.md`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.1.0/mongodb_orm/custom_urls/bread_urls.py` & `mongodb_orm-0.1.0a1/mongodb_orm/custom_urls/bread_urls.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.1.0/mongodb_orm/interfaces/base_mongodb_model.py` & `mongodb_orm-0.1.0a1/mongodb_orm/interfaces/base_mongodb_model.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.1.0/mongodb_orm/interfaces/mongodb_model.py` & `mongodb_orm-0.1.0a1/mongodb_orm/interfaces/mongodb_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import math
 import pymongo
 from bson import ObjectId
 from datetime import datetime
 from typing import List, Union, Sequence
+
+from pymongo.command_cursor import CommandCursor
 from pymongo.cursor import Cursor
 from pymongo.collection import Collection
 from pymongo.results import InsertOneResult
 
 from mongodb_orm.interfaces.mongodb_model_events import MongoDBModelEvents
 from mongodb_orm.types.index import Index
 from mongodb_orm.utils.helpers import Helper
@@ -88,43 +90,45 @@
         cursor: Cursor = self._collection.find(
             filters, projection=self._projection
         ).sort(sort_criteria).skip(
             (page * per_page) - per_page
         ).limit(per_page)
         # Convert cursor to list of dictionaries
         data = [Helper.standardize_dict(item, underscore=True) for item in list(cursor)]
+        # Get total documents that matches the filters
+        matches = self.count(filters)
         # Get total documents count
         total_documents = self.count()
         # Calculate total pages
         total_pages = math.ceil(total_documents / per_page)
 
         query_result: dict = {
             'data': data,
             'filters': filters,
             'page': page,
             'per_page': per_page,
             'total_pages': total_pages,
             'sort_by': [{sort_tuple[0]: sort_tuple[1]} for sort_tuple in sort_criteria],
-            'matches': len(data),
-            'total_documents': self.count()
+            'matches': matches,
+            'total_documents': total_documents
         }
         return query_result
 
     @chained
     def find_one(self, filters: dict, sort_criteria: List[tuple] = None) -> Union[dict, 'MongoDBModel']:
         return self._collection.find_one(filters, sort=sort_criteria, projection=self._projection)
 
     @chained
     def put(self, pk: str, record: dict) -> Union[dict, 'MongoDBModel']:
         query = self._collection.find_one_and_update({'_id': ObjectId(pk)},
                                                      {'$set': {**record, **({
                                                                                 'updated_at': datetime.utcnow()
                                                                             } if self.timestamp else {})}},
                                                      projection=self._projection)
-        self.on_partial_update(self.get(pk).json(), record)
+        self.on_update(self.get(pk).json(), record)
         return query
 
     @chained
     def patch(self, pk: str, record: dict) -> Union[dict, 'MongoDBModel']:
         query = self._collection.find_one_and_update({'_id': ObjectId(pk)},
                                                      {'$push': record,
                                                       '$set':
```

### Comparing `mongodb_orm-0.1.0/mongodb_orm/interfaces/mongodb_model_events.py` & `mongodb_orm-0.1.0a1/mongodb_orm/interfaces/mongodb_model_events.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.1.0/mongodb_orm/management/commands/update_schema.py` & `mongodb_orm-0.1.0a1/mongodb_orm/management/commands/update_schema.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.1.0/mongodb_orm/types/model_schema.py` & `mongodb_orm-0.1.0a1/mongodb_orm/types/model_schema.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.1.0/mongodb_orm/utils/helpers.py` & `mongodb_orm-0.1.0a1/mongodb_orm/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.1.0/mongodb_orm/views/mongodb_api_model_view.py` & `mongodb_orm-0.1.0a1/mongodb_orm/views/mongodb_api_model_view.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.1.0/mongodb_orm.egg-info/SOURCES.txt` & `mongodb_orm-0.1.0a1/mongodb_orm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.1.0/setup.py` & `mongodb_orm-0.1.0a1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 # Fix and optimise the library installation
 setup(
     name="mongodb_orm",
-    version="0.1.0",
+    version="0.1.0a1",
     author="Khai",
     author_email="sarraj.khaireddine@gmail.com",
     license="MIT",
     packages=find_packages(),
     include_package_data=True,
     description="mongodb ORM for django framework",
     long_description="mongodb ORM for django framework",
```

