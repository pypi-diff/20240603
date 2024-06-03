# Comparing `tmp/mongodb_orm-0.1.0a2.tar.gz` & `tmp/mongodb_orm-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongodb_orm-0.1.0a2.tar", last modified: Mon Jun  3 08:50:02 2024, max compression
+gzip compressed data, was "mongodb_orm-0.1.0a3.tar", last modified: Mon Jun  3 09:47:38 2024, max compression
```

## Comparing `mongodb_orm-0.1.0a2.tar` & `mongodb_orm-0.1.0a3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 08:50:02.447567 mongodb_orm-0.1.0a2/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      333 2024-06-03 08:50:02.445181 mongodb_orm-0.1.0a2/PKG-INFO
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      565 2024-04-23 13:57:27.000000 mongodb_orm-0.1.0a2/README.md
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 08:50:02.311206 mongodb_orm-0.1.0a2/mongodb_orm/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       91 2024-04-23 14:47:25.000000 mongodb_orm-0.1.0a2/mongodb_orm/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      475 2024-04-23 14:25:35.000000 mongodb_orm-0.1.0a2/mongodb_orm/apps.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 08:50:02.321257 mongodb_orm-0.1.0a2/mongodb_orm/custom_urls/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-18 11:23:58.000000 mongodb_orm-0.1.0a2/mongodb_orm/custom_urls/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1507 2024-05-03 12:46:06.000000 mongodb_orm-0.1.0a2/mongodb_orm/custom_urls/bread_urls.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 08:50:02.323962 mongodb_orm-0.1.0a2/mongodb_orm/decorators/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.1.0a2/mongodb_orm/decorators/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      433 2024-06-03 08:11:09.000000 mongodb_orm-0.1.0a2/mongodb_orm/decorators/chained.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 08:50:02.327851 mongodb_orm-0.1.0a2/mongodb_orm/exceptions/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.1.0a2/mongodb_orm/exceptions/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      138 2024-04-04 10:34:42.000000 mongodb_orm-0.1.0a2/mongodb_orm/exceptions/syntax_exceptions.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 08:50:02.339343 mongodb_orm-0.1.0a2/mongodb_orm/interfaces/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:42.000000 mongodb_orm-0.1.0a2/mongodb_orm/interfaces/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     2619 2024-04-29 14:42:33.000000 mongodb_orm-0.1.0a2/mongodb_orm/interfaces/base_mongodb_model.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     7789 2024-06-03 08:15:07.000000 mongodb_orm-0.1.0a2/mongodb_orm/interfaces/mongodb_model.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      801 2024-04-29 09:28:59.000000 mongodb_orm-0.1.0a2/mongodb_orm/interfaces/mongodb_model_events.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 08:50:02.359998 mongodb_orm-0.1.0a2/mongodb_orm/management/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:43.000000 mongodb_orm-0.1.0a2/mongodb_orm/management/__init__.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 08:50:02.365150 mongodb_orm-0.1.0a2/mongodb_orm/management/commands/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.1.0a2/mongodb_orm/management/commands/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     4559 2024-04-23 15:18:03.000000 mongodb_orm-0.1.0a2/mongodb_orm/management/commands/update_schema.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 08:50:02.368138 mongodb_orm-0.1.0a2/mongodb_orm/models/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:43.000000 mongodb_orm-0.1.0a2/mongodb_orm/models/__init__.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 08:50:02.371109 mongodb_orm-0.1.0a2/mongodb_orm/singletons/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.1.0a2/mongodb_orm/singletons/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      380 2024-04-04 10:34:44.000000 mongodb_orm-0.1.0a2/mongodb_orm/singletons/mongodb_singleton_client.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 08:50:02.436146 mongodb_orm-0.1.0a2/mongodb_orm/types/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      508 2024-04-04 10:34:44.000000 mongodb_orm-0.1.0a2/mongodb_orm/types/Relation.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.1.0a2/mongodb_orm/types/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      128 2024-04-04 10:34:44.000000 mongodb_orm-0.1.0a2/mongodb_orm/types/index.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      406 2024-06-03 08:11:09.000000 mongodb_orm-0.1.0a2/mongodb_orm/types/logger_object.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      766 2024-06-03 08:11:09.000000 mongodb_orm-0.1.0a2/mongodb_orm/types/model_schema.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      368 2024-04-23 15:18:03.000000 mongodb_orm-0.1.0a2/mongodb_orm/types/options.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      189 2024-05-03 12:47:26.000000 mongodb_orm-0.1.0a2/mongodb_orm/urls.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 08:50:02.440068 mongodb_orm-0.1.0a2/mongodb_orm/utils/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:11:55.000000 mongodb_orm-0.1.0a2/mongodb_orm/utils/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1855 2024-06-03 08:11:09.000000 mongodb_orm-0.1.0a2/mongodb_orm/utils/helpers.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 08:50:02.442180 mongodb_orm-0.1.0a2/mongodb_orm/views/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.1.0a2/mongodb_orm/views/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     4060 2024-06-03 08:49:46.000000 mongodb_orm-0.1.0a2/mongodb_orm/views/mongodb_api_model_view.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 08:50:02.443923 mongodb_orm-0.1.0a2/mongodb_orm.egg-info/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      333 2024-06-03 08:50:02.000000 mongodb_orm-0.1.0a2/mongodb_orm.egg-info/PKG-INFO
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1208 2024-06-03 08:50:02.000000 mongodb_orm-0.1.0a2/mongodb_orm.egg-info/SOURCES.txt
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        1 2024-06-03 08:50:02.000000 mongodb_orm-0.1.0a2/mongodb_orm.egg-info/dependency_links.txt
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       35 2024-06-03 08:50:02.000000 mongodb_orm-0.1.0a2/mongodb_orm.egg-info/requires.txt
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       12 2024-06-03 08:50:02.000000 mongodb_orm-0.1.0a2/mongodb_orm.egg-info/top_level.txt
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       38 2024-06-03 08:50:02.447838 mongodb_orm-0.1.0a2/setup.cfg
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      594 2024-06-03 08:49:52.000000 mongodb_orm-0.1.0a2/setup.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 09:47:38.798621 mongodb_orm-0.1.0a3/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      333 2024-06-03 09:47:38.796923 mongodb_orm-0.1.0a3/PKG-INFO
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      565 2024-04-23 13:57:27.000000 mongodb_orm-0.1.0a3/README.md
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 09:47:38.687806 mongodb_orm-0.1.0a3/mongodb_orm/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       91 2024-04-23 14:47:25.000000 mongodb_orm-0.1.0a3/mongodb_orm/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      475 2024-04-23 14:25:35.000000 mongodb_orm-0.1.0a3/mongodb_orm/apps.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 09:47:38.707054 mongodb_orm-0.1.0a3/mongodb_orm/custom_urls/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-18 11:23:58.000000 mongodb_orm-0.1.0a3/mongodb_orm/custom_urls/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1507 2024-05-03 12:46:06.000000 mongodb_orm-0.1.0a3/mongodb_orm/custom_urls/bread_urls.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 09:47:38.710023 mongodb_orm-0.1.0a3/mongodb_orm/decorators/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.1.0a3/mongodb_orm/decorators/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      433 2024-06-03 08:11:09.000000 mongodb_orm-0.1.0a3/mongodb_orm/decorators/chained.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 09:47:38.712712 mongodb_orm-0.1.0a3/mongodb_orm/exceptions/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.1.0a3/mongodb_orm/exceptions/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      138 2024-04-04 10:34:42.000000 mongodb_orm-0.1.0a3/mongodb_orm/exceptions/syntax_exceptions.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 09:47:38.718035 mongodb_orm-0.1.0a3/mongodb_orm/interfaces/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:42.000000 mongodb_orm-0.1.0a3/mongodb_orm/interfaces/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     2619 2024-04-29 14:42:33.000000 mongodb_orm-0.1.0a3/mongodb_orm/interfaces/base_mongodb_model.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     7846 2024-06-03 09:47:26.000000 mongodb_orm-0.1.0a3/mongodb_orm/interfaces/mongodb_model.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      801 2024-04-29 09:28:59.000000 mongodb_orm-0.1.0a3/mongodb_orm/interfaces/mongodb_model_events.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 09:47:38.719659 mongodb_orm-0.1.0a3/mongodb_orm/management/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:43.000000 mongodb_orm-0.1.0a3/mongodb_orm/management/__init__.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 09:47:38.722456 mongodb_orm-0.1.0a3/mongodb_orm/management/commands/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.1.0a3/mongodb_orm/management/commands/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     4559 2024-04-23 15:18:03.000000 mongodb_orm-0.1.0a3/mongodb_orm/management/commands/update_schema.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 09:47:38.723641 mongodb_orm-0.1.0a3/mongodb_orm/models/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:43.000000 mongodb_orm-0.1.0a3/mongodb_orm/models/__init__.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 09:47:38.725534 mongodb_orm-0.1.0a3/mongodb_orm/singletons/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.1.0a3/mongodb_orm/singletons/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      380 2024-04-04 10:34:44.000000 mongodb_orm-0.1.0a3/mongodb_orm/singletons/mongodb_singleton_client.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 09:47:38.758758 mongodb_orm-0.1.0a3/mongodb_orm/types/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      508 2024-04-04 10:34:44.000000 mongodb_orm-0.1.0a3/mongodb_orm/types/Relation.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.1.0a3/mongodb_orm/types/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      128 2024-04-04 10:34:44.000000 mongodb_orm-0.1.0a3/mongodb_orm/types/index.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      406 2024-06-03 08:11:09.000000 mongodb_orm-0.1.0a3/mongodb_orm/types/logger_object.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      766 2024-06-03 08:11:09.000000 mongodb_orm-0.1.0a3/mongodb_orm/types/model_schema.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      368 2024-04-23 15:18:03.000000 mongodb_orm-0.1.0a3/mongodb_orm/types/options.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      189 2024-05-03 12:47:26.000000 mongodb_orm-0.1.0a3/mongodb_orm/urls.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 09:47:38.766422 mongodb_orm-0.1.0a3/mongodb_orm/utils/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:11:55.000000 mongodb_orm-0.1.0a3/mongodb_orm/utils/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1855 2024-06-03 08:11:09.000000 mongodb_orm-0.1.0a3/mongodb_orm/utils/helpers.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 09:47:38.791580 mongodb_orm-0.1.0a3/mongodb_orm/views/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.1.0a3/mongodb_orm/views/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     4060 2024-06-03 08:49:46.000000 mongodb_orm-0.1.0a3/mongodb_orm/views/mongodb_api_model_view.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 09:47:38.795599 mongodb_orm-0.1.0a3/mongodb_orm.egg-info/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      333 2024-06-03 09:47:38.000000 mongodb_orm-0.1.0a3/mongodb_orm.egg-info/PKG-INFO
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1208 2024-06-03 09:47:38.000000 mongodb_orm-0.1.0a3/mongodb_orm.egg-info/SOURCES.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        1 2024-06-03 09:47:38.000000 mongodb_orm-0.1.0a3/mongodb_orm.egg-info/dependency_links.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       35 2024-06-03 09:47:38.000000 mongodb_orm-0.1.0a3/mongodb_orm.egg-info/requires.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       12 2024-06-03 09:47:38.000000 mongodb_orm-0.1.0a3/mongodb_orm.egg-info/top_level.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       38 2024-06-03 09:47:38.798842 mongodb_orm-0.1.0a3/setup.cfg
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      594 2024-06-03 09:47:30.000000 mongodb_orm-0.1.0a3/setup.py
```

### Comparing `mongodb_orm-0.1.0a2/README.md` & `mongodb_orm-0.1.0a3/README.md`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.1.0a2/mongodb_orm/custom_urls/bread_urls.py` & `mongodb_orm-0.1.0a3/mongodb_orm/custom_urls/bread_urls.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.1.0a2/mongodb_orm/interfaces/base_mongodb_model.py` & `mongodb_orm-0.1.0a3/mongodb_orm/interfaces/base_mongodb_model.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.1.0a2/mongodb_orm/interfaces/mongodb_model.py` & `mongodb_orm-0.1.0a3/mongodb_orm/interfaces/mongodb_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,14 +120,16 @@
     @chained
     def put(self, pk: str, record: dict) -> Union[dict, 'MongoDBModel']:
         query = self._collection.find_one_and_update({'_id': ObjectId(pk)},
                                                      {'$set': {**record, **({
                                                                                 'updated_at': datetime.utcnow()
                                                                             } if self.timestamp else {})}},
                                                      projection=self._projection)
+        print(self.get(pk).json())
+        print(record)
         self.on_update(self.get(pk).json(), record)
         return query
 
     @chained
     def patch(self, pk: str, record: dict) -> Union[dict, 'MongoDBModel']:
         query = self._collection.find_one_and_update({'_id': ObjectId(pk)},
                                                      {'$push': record,
```

### Comparing `mongodb_orm-0.1.0a2/mongodb_orm/interfaces/mongodb_model_events.py` & `mongodb_orm-0.1.0a3/mongodb_orm/interfaces/mongodb_model_events.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.1.0a2/mongodb_orm/management/commands/update_schema.py` & `mongodb_orm-0.1.0a3/mongodb_orm/management/commands/update_schema.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.1.0a2/mongodb_orm/types/model_schema.py` & `mongodb_orm-0.1.0a3/mongodb_orm/types/model_schema.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.1.0a2/mongodb_orm/utils/helpers.py` & `mongodb_orm-0.1.0a3/mongodb_orm/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.1.0a2/mongodb_orm/views/mongodb_api_model_view.py` & `mongodb_orm-0.1.0a3/mongodb_orm/views/mongodb_api_model_view.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.1.0a2/mongodb_orm.egg-info/SOURCES.txt` & `mongodb_orm-0.1.0a3/mongodb_orm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.1.0a2/setup.py` & `mongodb_orm-0.1.0a3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 # Fix and optimise the library installation
 setup(
     name="mongodb_orm",
-    version="0.1.0a2",
+    version="0.1.0a3",
     author="Khai",
     author_email="sarraj.khaireddine@gmail.com",
     license="MIT",
     packages=find_packages(),
     include_package_data=True,
     description="mongodb ORM for django framework",
     long_description="mongodb ORM for django framework",
```

