# Comparing `tmp/mongodb_orm-0.1.0a8.tar.gz` & `tmp/mongodb_orm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongodb_orm-0.1.0a8.tar", last modified: Mon Jun  3 10:10:10 2024, max compression
+gzip compressed data, was "mongodb_orm-0.1.1.tar", last modified: Mon Jun  3 10:17:38 2024, max compression
```

## Comparing `mongodb_orm-0.1.0a8.tar` & `mongodb_orm-0.1.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 10:10:10.137522 mongodb_orm-0.1.0a8/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      333 2024-06-03 10:10:10.136265 mongodb_orm-0.1.0a8/PKG-INFO
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      565 2024-04-23 13:57:27.000000 mongodb_orm-0.1.0a8/README.md
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 10:10:10.071454 mongodb_orm-0.1.0a8/mongodb_orm/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       91 2024-04-23 14:47:25.000000 mongodb_orm-0.1.0a8/mongodb_orm/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      475 2024-04-23 14:25:35.000000 mongodb_orm-0.1.0a8/mongodb_orm/apps.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 10:10:10.082155 mongodb_orm-0.1.0a8/mongodb_orm/custom_urls/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-18 11:23:58.000000 mongodb_orm-0.1.0a8/mongodb_orm/custom_urls/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1507 2024-05-03 12:46:06.000000 mongodb_orm-0.1.0a8/mongodb_orm/custom_urls/bread_urls.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 10:10:10.085072 mongodb_orm-0.1.0a8/mongodb_orm/decorators/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.1.0a8/mongodb_orm/decorators/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      433 2024-06-03 08:11:09.000000 mongodb_orm-0.1.0a8/mongodb_orm/decorators/chained.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 10:10:10.092101 mongodb_orm-0.1.0a8/mongodb_orm/exceptions/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.1.0a8/mongodb_orm/exceptions/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      138 2024-04-04 10:34:42.000000 mongodb_orm-0.1.0a8/mongodb_orm/exceptions/syntax_exceptions.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 10:10:10.098656 mongodb_orm-0.1.0a8/mongodb_orm/interfaces/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:42.000000 mongodb_orm-0.1.0a8/mongodb_orm/interfaces/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     2619 2024-04-29 14:42:33.000000 mongodb_orm-0.1.0a8/mongodb_orm/interfaces/base_mongodb_model.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     7896 2024-06-03 10:10:00.000000 mongodb_orm-0.1.0a8/mongodb_orm/interfaces/mongodb_model.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      801 2024-04-29 09:28:59.000000 mongodb_orm-0.1.0a8/mongodb_orm/interfaces/mongodb_model_events.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 10:10:10.100359 mongodb_orm-0.1.0a8/mongodb_orm/management/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:43.000000 mongodb_orm-0.1.0a8/mongodb_orm/management/__init__.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 10:10:10.102406 mongodb_orm-0.1.0a8/mongodb_orm/management/commands/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.1.0a8/mongodb_orm/management/commands/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     4559 2024-04-23 15:18:03.000000 mongodb_orm-0.1.0a8/mongodb_orm/management/commands/update_schema.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 10:10:10.103974 mongodb_orm-0.1.0a8/mongodb_orm/models/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:43.000000 mongodb_orm-0.1.0a8/mongodb_orm/models/__init__.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 10:10:10.106423 mongodb_orm-0.1.0a8/mongodb_orm/singletons/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.1.0a8/mongodb_orm/singletons/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      380 2024-04-04 10:34:44.000000 mongodb_orm-0.1.0a8/mongodb_orm/singletons/mongodb_singleton_client.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 10:10:10.117833 mongodb_orm-0.1.0a8/mongodb_orm/types/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      508 2024-04-04 10:34:44.000000 mongodb_orm-0.1.0a8/mongodb_orm/types/Relation.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.1.0a8/mongodb_orm/types/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      128 2024-04-04 10:34:44.000000 mongodb_orm-0.1.0a8/mongodb_orm/types/index.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      406 2024-06-03 08:11:09.000000 mongodb_orm-0.1.0a8/mongodb_orm/types/logger_object.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      766 2024-06-03 08:11:09.000000 mongodb_orm-0.1.0a8/mongodb_orm/types/model_schema.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      368 2024-04-23 15:18:03.000000 mongodb_orm-0.1.0a8/mongodb_orm/types/options.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      189 2024-05-03 12:47:26.000000 mongodb_orm-0.1.0a8/mongodb_orm/urls.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 10:10:10.123396 mongodb_orm-0.1.0a8/mongodb_orm/utils/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:11:55.000000 mongodb_orm-0.1.0a8/mongodb_orm/utils/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1855 2024-06-03 08:11:09.000000 mongodb_orm-0.1.0a8/mongodb_orm/utils/helpers.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 10:10:10.131326 mongodb_orm-0.1.0a8/mongodb_orm/views/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.1.0a8/mongodb_orm/views/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     4009 2024-06-03 10:10:00.000000 mongodb_orm-0.1.0a8/mongodb_orm/views/mongodb_api_model_view.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 10:10:10.134858 mongodb_orm-0.1.0a8/mongodb_orm.egg-info/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      333 2024-06-03 10:10:09.000000 mongodb_orm-0.1.0a8/mongodb_orm.egg-info/PKG-INFO
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1208 2024-06-03 10:10:09.000000 mongodb_orm-0.1.0a8/mongodb_orm.egg-info/SOURCES.txt
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        1 2024-06-03 10:10:09.000000 mongodb_orm-0.1.0a8/mongodb_orm.egg-info/dependency_links.txt
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       35 2024-06-03 10:10:09.000000 mongodb_orm-0.1.0a8/mongodb_orm.egg-info/requires.txt
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       12 2024-06-03 10:10:09.000000 mongodb_orm-0.1.0a8/mongodb_orm.egg-info/top_level.txt
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       38 2024-06-03 10:10:10.137740 mongodb_orm-0.1.0a8/setup.cfg
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      594 2024-06-03 10:10:00.000000 mongodb_orm-0.1.0a8/setup.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 10:17:38.049263 mongodb_orm-0.1.1/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      331 2024-06-03 10:17:38.047062 mongodb_orm-0.1.1/PKG-INFO
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      565 2024-04-23 13:57:27.000000 mongodb_orm-0.1.1/README.md
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 10:17:37.945496 mongodb_orm-0.1.1/mongodb_orm/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       91 2024-04-23 14:47:25.000000 mongodb_orm-0.1.1/mongodb_orm/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      475 2024-04-23 14:25:35.000000 mongodb_orm-0.1.1/mongodb_orm/apps.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 10:17:37.957976 mongodb_orm-0.1.1/mongodb_orm/custom_urls/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-18 11:23:58.000000 mongodb_orm-0.1.1/mongodb_orm/custom_urls/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1507 2024-05-03 12:46:06.000000 mongodb_orm-0.1.1/mongodb_orm/custom_urls/bread_urls.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 10:17:37.961177 mongodb_orm-0.1.1/mongodb_orm/decorators/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.1.1/mongodb_orm/decorators/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      433 2024-06-03 08:11:09.000000 mongodb_orm-0.1.1/mongodb_orm/decorators/chained.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 10:17:37.963590 mongodb_orm-0.1.1/mongodb_orm/exceptions/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.1.1/mongodb_orm/exceptions/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      138 2024-04-04 10:34:42.000000 mongodb_orm-0.1.1/mongodb_orm/exceptions/syntax_exceptions.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 10:17:37.969729 mongodb_orm-0.1.1/mongodb_orm/interfaces/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:42.000000 mongodb_orm-0.1.1/mongodb_orm/interfaces/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     2619 2024-04-29 14:42:33.000000 mongodb_orm-0.1.1/mongodb_orm/interfaces/base_mongodb_model.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     7896 2024-06-03 10:10:00.000000 mongodb_orm-0.1.1/mongodb_orm/interfaces/mongodb_model.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      801 2024-04-29 09:28:59.000000 mongodb_orm-0.1.1/mongodb_orm/interfaces/mongodb_model_events.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 10:17:37.971157 mongodb_orm-0.1.1/mongodb_orm/management/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:43.000000 mongodb_orm-0.1.1/mongodb_orm/management/__init__.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 10:17:37.974453 mongodb_orm-0.1.1/mongodb_orm/management/commands/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.1.1/mongodb_orm/management/commands/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     4559 2024-04-23 15:18:03.000000 mongodb_orm-0.1.1/mongodb_orm/management/commands/update_schema.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 10:17:37.976539 mongodb_orm-0.1.1/mongodb_orm/models/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:43.000000 mongodb_orm-0.1.1/mongodb_orm/models/__init__.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 10:17:37.983066 mongodb_orm-0.1.1/mongodb_orm/singletons/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.1.1/mongodb_orm/singletons/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      380 2024-04-04 10:34:44.000000 mongodb_orm-0.1.1/mongodb_orm/singletons/mongodb_singleton_client.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 10:17:38.001098 mongodb_orm-0.1.1/mongodb_orm/types/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      508 2024-04-04 10:34:44.000000 mongodb_orm-0.1.1/mongodb_orm/types/Relation.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.1.1/mongodb_orm/types/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      128 2024-04-04 10:34:44.000000 mongodb_orm-0.1.1/mongodb_orm/types/index.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      406 2024-06-03 08:11:09.000000 mongodb_orm-0.1.1/mongodb_orm/types/logger_object.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      766 2024-06-03 08:11:09.000000 mongodb_orm-0.1.1/mongodb_orm/types/model_schema.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      368 2024-04-23 15:18:03.000000 mongodb_orm-0.1.1/mongodb_orm/types/options.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      189 2024-05-03 12:47:26.000000 mongodb_orm-0.1.1/mongodb_orm/urls.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 10:17:38.021562 mongodb_orm-0.1.1/mongodb_orm/utils/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:11:55.000000 mongodb_orm-0.1.1/mongodb_orm/utils/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1855 2024-06-03 08:11:09.000000 mongodb_orm-0.1.1/mongodb_orm/utils/helpers.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 10:17:38.034507 mongodb_orm-0.1.1/mongodb_orm/views/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.1.1/mongodb_orm/views/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     4008 2024-06-03 10:17:13.000000 mongodb_orm-0.1.1/mongodb_orm/views/mongodb_api_model_view.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-06-03 10:17:38.039939 mongodb_orm-0.1.1/mongodb_orm.egg-info/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      331 2024-06-03 10:17:37.000000 mongodb_orm-0.1.1/mongodb_orm.egg-info/PKG-INFO
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1208 2024-06-03 10:17:37.000000 mongodb_orm-0.1.1/mongodb_orm.egg-info/SOURCES.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        1 2024-06-03 10:17:37.000000 mongodb_orm-0.1.1/mongodb_orm.egg-info/dependency_links.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       35 2024-06-03 10:17:37.000000 mongodb_orm-0.1.1/mongodb_orm.egg-info/requires.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       12 2024-06-03 10:17:37.000000 mongodb_orm-0.1.1/mongodb_orm.egg-info/top_level.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       38 2024-06-03 10:17:38.049507 mongodb_orm-0.1.1/setup.cfg
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      592 2024-06-03 10:17:29.000000 mongodb_orm-0.1.1/setup.py
```

### Comparing `mongodb_orm-0.1.0a8/README.md` & `mongodb_orm-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.1.0a8/mongodb_orm/custom_urls/bread_urls.py` & `mongodb_orm-0.1.1/mongodb_orm/custom_urls/bread_urls.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.1.0a8/mongodb_orm/interfaces/base_mongodb_model.py` & `mongodb_orm-0.1.1/mongodb_orm/interfaces/base_mongodb_model.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.1.0a8/mongodb_orm/interfaces/mongodb_model.py` & `mongodb_orm-0.1.1/mongodb_orm/interfaces/mongodb_model.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.1.0a8/mongodb_orm/interfaces/mongodb_model_events.py` & `mongodb_orm-0.1.1/mongodb_orm/interfaces/mongodb_model_events.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.1.0a8/mongodb_orm/management/commands/update_schema.py` & `mongodb_orm-0.1.1/mongodb_orm/management/commands/update_schema.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.1.0a8/mongodb_orm/types/model_schema.py` & `mongodb_orm-0.1.1/mongodb_orm/types/model_schema.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.1.0a8/mongodb_orm/utils/helpers.py` & `mongodb_orm-0.1.1/mongodb_orm/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.1.0a8/mongodb_orm/views/mongodb_api_model_view.py` & `mongodb_orm-0.1.1/mongodb_orm/views/mongodb_api_model_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,14 @@
             retrieve_record: dict = MongoDBModel.get(self, pk=str(new_record.inserted_id)).json()
         except Exception as e:
             return Response({'success': False, 'error': str(e)})
         return Response({'success': True, 'record': retrieve_record})
 
     def update(self, request, *args, **kwargs) -> Response:
         MongoDBModel.set_tenant(self, tenant_name=request.headers.get('database', 'public'))
-
         try:
             MongoDBModel.put(self, pk=str(kwargs.get('pk')), record=Helper.standard_record(request.data))
         except Exception as e:
             return Response({'success': False, 'error': str(e)})
         return Response({'success': True})
 
     def partial_update(self, request, *args, **kwargs) -> Response:
```

### Comparing `mongodb_orm-0.1.0a8/mongodb_orm.egg-info/SOURCES.txt` & `mongodb_orm-0.1.1/mongodb_orm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.1.0a8/setup.py` & `mongodb_orm-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 # Fix and optimise the library installation
 setup(
     name="mongodb_orm",
-    version="0.1.0a8",
+    version="0.1.1",
     author="Khai",
     author_email="sarraj.khaireddine@gmail.com",
     license="MIT",
     packages=find_packages(),
     include_package_data=True,
     description="mongodb ORM for django framework",
     long_description="mongodb ORM for django framework",
```

