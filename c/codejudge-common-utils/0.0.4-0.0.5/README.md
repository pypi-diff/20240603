# Comparing `tmp/codejudge-common-utils-0.0.4.tar.gz` & `tmp/codejudge-common-utils-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codejudge-common-utils-0.0.4.tar", last modified: Sat Jun  1 19:51:28 2024, max compression
+gzip compressed data, was "codejudge-common-utils-0.0.5.tar", last modified: Mon Jun  3 03:28:01 2024, max compression
```

## Comparing `codejudge-common-utils-0.0.4.tar` & `codejudge-common-utils-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxr-xr-x   0 yash       (501) staff       (20)        0 2024-06-01 19:51:28.104319 codejudge-common-utils-0.0.4/
--rw-r--r--   0 yash       (501) staff       (20)     2250 2024-06-01 19:51:28.104090 codejudge-common-utils-0.0.4/PKG-INFO
--rw-r--r--   0 yash       (501) staff       (20)     1496 2024-05-09 12:19:46.000000 codejudge-common-utils-0.0.4/README.md
-drwxr-xr-x   0 yash       (501) staff       (20)        0 2024-06-01 19:51:28.100986 codejudge-common-utils-0.0.4/codejudge_common_utils.egg-info/
--rw-r--r--   0 yash       (501) staff       (20)     2250 2024-06-01 19:51:28.000000 codejudge-common-utils-0.0.4/codejudge_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 yash       (501) staff       (20)      527 2024-06-01 19:51:28.000000 codejudge-common-utils-0.0.4/codejudge_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 yash       (501) staff       (20)        1 2024-06-01 19:51:28.000000 codejudge-common-utils-0.0.4/codejudge_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 yash       (501) staff       (20)        7 2024-06-01 19:51:28.000000 codejudge-common-utils-0.0.4/codejudge_common_utils.egg-info/top_level.txt
-drwxr-xr-x   0 yash       (501) staff       (20)        0 2024-06-01 19:51:28.103713 codejudge-common-utils-0.0.4/common/
--rw-r--r--   0 yash       (501) staff       (20)        0 2024-05-08 13:47:56.000000 codejudge-common-utils-0.0.4/common/__init__.py
--rw-r--r--   0 yash       (501) staff       (20)      179 2024-05-13 20:27:30.000000 codejudge-common-utils-0.0.4/common/common_util.py
--rw-r--r--   0 yash       (501) staff       (20)      102 2024-06-01 19:49:23.000000 codejudge-common-utils-0.0.4/common/constants.py
--rw-r--r--   0 yash       (501) staff       (20)      395 2024-06-01 14:19:58.000000 codejudge-common-utils-0.0.4/common/data_purging_interface.py
--rw-r--r--   0 yash       (501) staff       (20)     6271 2024-06-01 19:49:23.000000 codejudge-common-utils-0.0.4/common/data_purging_util.py
--rw-r--r--   0 yash       (501) staff       (20)     7957 2024-05-09 19:18:11.000000 codejudge-common-utils-0.0.4/common/date_time_util.py
--rw-r--r--   0 yash       (501) staff       (20)     2167 2024-06-01 14:08:40.000000 codejudge-common-utils-0.0.4/common/enum_util.py
--rw-r--r--   0 yash       (501) staff       (20)     4908 2024-06-01 14:09:00.000000 codejudge-common-utils-0.0.4/common/enums.py
--rw-r--r--   0 yash       (501) staff       (20)     2763 2024-05-13 22:11:10.000000 codejudge-common-utils-0.0.4/common/interval_dates_and_archive_table_name.py
--rw-r--r--   0 yash       (501) staff       (20)      429 2024-05-13 08:22:33.000000 codejudge-common-utils-0.0.4/common/interval_type_to_process_function_mapping.py
--rw-r--r--   0 yash       (501) staff       (20)     1144 2024-05-14 09:38:43.000000 codejudge-common-utils-0.0.4/common/model_util.py
--rw-r--r--   0 yash       (501) staff       (20)     4906 2024-06-01 19:22:04.000000 codejudge-common-utils-0.0.4/common/table_util.py
--rw-r--r--   0 yash       (501) staff       (20)       38 2024-06-01 19:51:28.104369 codejudge-common-utils-0.0.4/setup.cfg
--rw-r--r--   0 yash       (501) staff       (20)      986 2024-06-01 19:51:23.000000 codejudge-common-utils-0.0.4/setup.py
+drwxr-xr-x   0 yash       (501) staff       (20)        0 2024-06-03 03:28:01.860745 codejudge-common-utils-0.0.5/
+-rw-r--r--   0 yash       (501) staff       (20)     2290 2024-06-03 03:28:01.860509 codejudge-common-utils-0.0.5/PKG-INFO
+-rw-r--r--   0 yash       (501) staff       (20)     1496 2024-05-09 12:19:46.000000 codejudge-common-utils-0.0.5/README.md
+drwxr-xr-x   0 yash       (501) staff       (20)        0 2024-06-03 03:28:01.849511 codejudge-common-utils-0.0.5/codejudge_common_utils.egg-info/
+-rw-r--r--   0 yash       (501) staff       (20)     2290 2024-06-03 03:28:01.000000 codejudge-common-utils-0.0.5/codejudge_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 yash       (501) staff       (20)      583 2024-06-03 03:28:01.000000 codejudge-common-utils-0.0.5/codejudge_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 yash       (501) staff       (20)        1 2024-06-03 03:28:01.000000 codejudge-common-utils-0.0.5/codejudge_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 yash       (501) staff       (20)        7 2024-06-03 03:28:01.000000 codejudge-common-utils-0.0.5/codejudge_common_utils.egg-info/top_level.txt
+drwxr-xr-x   0 yash       (501) staff       (20)        0 2024-06-03 03:28:01.860017 codejudge-common-utils-0.0.5/common/
+-rw-r--r--   0 yash       (501) staff       (20)       32 2024-06-03 03:25:12.000000 codejudge-common-utils-0.0.5/common/__init__.py
+-rw-r--r--   0 yash       (501) staff       (20)      179 2024-05-13 20:27:30.000000 codejudge-common-utils-0.0.5/common/common_util.py
+-rw-r--r--   0 yash       (501) staff       (20)       99 2024-06-01 22:06:39.000000 codejudge-common-utils-0.0.5/common/constants.py
+-rw-r--r--   0 yash       (501) staff       (20)      395 2024-06-01 14:19:58.000000 codejudge-common-utils-0.0.5/common/data_purging_interface.py
+-rw-r--r--   0 yash       (501) staff       (20)     6245 2024-06-01 22:07:38.000000 codejudge-common-utils-0.0.5/common/data_purging_util.py
+-rw-r--r--   0 yash       (501) staff       (20)     7957 2024-05-09 19:18:11.000000 codejudge-common-utils-0.0.5/common/date_time_util.py
+-rw-r--r--   0 yash       (501) staff       (20)     2167 2024-06-01 14:08:40.000000 codejudge-common-utils-0.0.5/common/enum_util.py
+-rw-r--r--   0 yash       (501) staff       (20)    35138 2024-06-02 10:12:29.000000 codejudge-common-utils-0.0.5/common/enums.py
+-rw-r--r--   0 yash       (501) staff       (20)     4233 2024-06-02 10:12:29.000000 codejudge-common-utils-0.0.5/common/exceptions.py
+-rw-r--r--   0 yash       (501) staff       (20)     2763 2024-05-13 22:11:10.000000 codejudge-common-utils-0.0.5/common/interval_dates_and_archive_table_name.py
+-rw-r--r--   0 yash       (501) staff       (20)      429 2024-05-13 08:22:33.000000 codejudge-common-utils-0.0.5/common/interval_type_to_process_function_mapping.py
+-rw-r--r--   0 yash       (501) staff       (20)     2428 2024-06-03 03:27:49.000000 codejudge-common-utils-0.0.5/common/list_util.py
+-rw-r--r--   0 yash       (501) staff       (20)     1144 2024-05-14 09:38:43.000000 codejudge-common-utils-0.0.5/common/model_util.py
+-rw-r--r--   0 yash       (501) staff       (20)     4906 2024-06-01 19:22:04.000000 codejudge-common-utils-0.0.5/common/table_util.py
+-rw-r--r--   0 yash       (501) staff       (20)     2268 2024-03-20 07:50:29.000000 codejudge-common-utils-0.0.5/common/util.py
+-rw-r--r--   0 yash       (501) staff       (20)       38 2024-06-03 03:28:01.860807 codejudge-common-utils-0.0.5/setup.cfg
+-rw-r--r--   0 yash       (501) staff       (20)      966 2024-06-03 03:25:27.000000 codejudge-common-utils-0.0.5/setup.py
```

### Comparing `codejudge-common-utils-0.0.4/PKG-INFO` & `codejudge-common-utils-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codejudge-common-utils
-Version: 0.0.4
+Version: 0.0.5
 Summary: A codejudge common util library for python to perform certain tasks.
 Author: Yash Mittal
 Author-email: akhil@codejudge.io
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Description-Content-Type: text/markdown
 
 CODEJUDGE COMMON UTIL
 
 
 TESTING
     Whenever any changes are made in this module, follow the steps mentioned below:
```

### Comparing `codejudge-common-utils-0.0.4/README.md` & `codejudge-common-utils-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `codejudge-common-utils-0.0.4/codejudge_common_utils.egg-info/PKG-INFO` & `codejudge-common-utils-0.0.5/codejudge_common_utils.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codejudge-common-utils
-Version: 0.0.4
+Version: 0.0.5
 Summary: A codejudge common util library for python to perform certain tasks.
 Author: Yash Mittal
 Author-email: akhil@codejudge.io
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Description-Content-Type: text/markdown
 
 CODEJUDGE COMMON UTIL
 
 
 TESTING
     Whenever any changes are made in this module, follow the steps mentioned below:
```

### Comparing `codejudge-common-utils-0.0.4/codejudge_common_utils.egg-info/SOURCES.txt` & `codejudge-common-utils-0.0.5/codejudge_common_utils.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -8,11 +8,14 @@
 common/common_util.py
 common/constants.py
 common/data_purging_interface.py
 common/data_purging_util.py
 common/date_time_util.py
 common/enum_util.py
 common/enums.py
+common/exceptions.py
 common/interval_dates_and_archive_table_name.py
 common/interval_type_to_process_function_mapping.py
+common/list_util.py
 common/model_util.py
-common/table_util.py
+common/table_util.py
+common/util.py
```

### Comparing `codejudge-common-utils-0.0.4/common/data_purging_util.py` & `codejudge-common-utils-0.0.5/common/data_purging_util.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 from django.db import transaction, connection
 from rest_framework import status
 
 from common.constants import DATA_PURGING_MAX_RETRY
 from common.table_util import TableUtil
 from restapi.common.list_util import ListUtil
 from restapi.common.file_util import FileUtil
-from restapi.test.worker.data_purging_framework.data_purging_process import get_unique_ids_to_s3_file_paths_map, \
-    upload_json_file_in_s3_and_get_uuid_to_file_urls_map
+from restapi.test.worker.data_purging_framework.data_purging_process import get_ids_to_s3_file_paths_map, \
+    upload_json_file_in_s3_and_get_ids_to_file_urls_map
 from restapi.exception.exception import RecruitException
 
 
 logger = logging.getLogger(__name__)
 
 
 class DataPurgingUtil:
 
     @classmethod
     def archive_and_purge_stale_data(cls, table_name_str, main_table_name, interval_type, db_record_size,
                                      table_name_prefix, all_fields, purge_function_name, filter_table_name, app1,
-                                     is_fb):
+                                     is_fb, project_name):
         workspaces = []
         is_archive_table_present = False
         is_completed = False
         archive_table_name = None
         all_fields_and_values = None
         records_to_delete = None
         try:
@@ -44,19 +44,19 @@
                                                                                                      interval_start_date,
                                                                                                      interval_end_date,
                                                                                                      all_fields,
                                                                                                      table_name_str,
                                                                                                      db_record_size,
                                                                                                      app1)
                     if is_fb:
-                        unique_ids_to_s3_file_paths_map, unique_ids_to_file_names_map, workspaces = get_unique_ids_to_s3_file_paths_map(
-                            records_to_delete)
-                        uuid_to_file_urls_map = upload_json_file_in_s3_and_get_uuid_to_file_urls_map(
-                            unique_ids_to_s3_file_paths_map, unique_ids_to_file_names_map)
-                        all_fields_and_values = [uuid_to_file_urls_map]
+                        ids_to_s3_file_paths_map, ids_to_file_names_map, workspaces = get_ids_to_s3_file_paths_map(
+                            records_to_delete, table_name_str, project_name)
+                        ids_to_file_urls_map = upload_json_file_in_s3_and_get_ids_to_file_urls_map(
+                            ids_to_s3_file_paths_map, ids_to_file_names_map)
+                        all_fields_and_values = [ids_to_file_urls_map]
                     cursor = connection.cursor()
 
                     with transaction.atomic():
                         if is_archive_table_present is False:
                             TableUtil.drop_archive_table_if_exist(archive_table_name, cursor)
                             TableUtil.create_archive_table(archive_table_name, table_name_str, table_name_prefix,
                                                            cursor, is_fb)
@@ -64,22 +64,22 @@
                             is_archive_table_present = True
                         TableUtil.insert_data_to_new_archive_table(archive_table_name, all_fields_and_values, cursor)
                         logger.info("Records are successfully inserted in archive table {}".format(archive_table_name))
                         TableUtil.delete_records(table_name_str, records_to_delete, table_name_prefix, cursor, is_fb,
                                                  app1)
                         logger.info("Records are successfully deleted from the main table {}".format(main_table_name))
                         is_completed = True
-        except Exception as e:
+        finally:
             if is_completed is False:
                 retry_count = DATA_PURGING_MAX_RETRY
                 while retry_count > 0:
                     cursor = connection.cursor()
                     with transaction.atomic():
                         if is_archive_table_present is False:
-                            TableUtil.drop_archive_table_if_exist(archive_table_name)
+                            TableUtil.drop_archive_table_if_exist(archive_table_name, cursor)
                             TableUtil.create_archive_table(archive_table_name, table_name_str, table_name_prefix, cursor, is_fb)
                             TableUtil.make_migrations_to_create_table()
                             is_archive_table_present = True
                         TableUtil.insert_data_to_new_archive_table(archive_table_name, all_fields_and_values, cursor)
                         logger.info("Records are successfully inserted in archive table {}".format(archive_table_name))
                         TableUtil.delete_records(table_name_str, records_to_delete, table_name_prefix, cursor, is_fb,
                                                  app1)
@@ -89,13 +89,11 @@
                         retry_count = retry_count - 1
                         if retry_count == 0:
                             raise RecruitException(
                                 "Couldn't create table or insert rows in the table name {}, Please check the error: {}!".format(
                                     archive_table_name, str(e)), status=status.HTTP_500_INTERNAL_SERVER_ERROR)
                     else:
                         break
-
-        finally:
             if ListUtil.is_valid(workspaces):
                 for workspace in workspaces:
                     if workspace is not None and os.path.exists(workspace):
                         FileUtil.delete_folder(workspace, False)
```

### Comparing `codejudge-common-utils-0.0.4/common/date_time_util.py` & `codejudge-common-utils-0.0.5/common/date_time_util.py`

 * *Files identical despite different names*

### Comparing `codejudge-common-utils-0.0.4/common/enum_util.py` & `codejudge-common-utils-0.0.5/common/enum_util.py`

 * *Files identical despite different names*

### Comparing `codejudge-common-utils-0.0.4/common/interval_dates_and_archive_table_name.py` & `codejudge-common-utils-0.0.5/common/interval_dates_and_archive_table_name.py`

 * *Files identical despite different names*

### Comparing `codejudge-common-utils-0.0.4/common/model_util.py` & `codejudge-common-utils-0.0.5/common/model_util.py`

 * *Files identical despite different names*

### Comparing `codejudge-common-utils-0.0.4/common/table_util.py` & `codejudge-common-utils-0.0.5/common/table_util.py`

 * *Files identical despite different names*

### Comparing `codejudge-common-utils-0.0.4/setup.py` & `codejudge-common-utils-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from setuptools import setup, find_packages
 
-with open('README.md', encoding='utf-8') as f:
-    long_description = f.read()
 
 setup(
     name="codejudge-common-utils",
-    version="0.0.4",
+    version="0.0.5",
     description="A codejudge common util library for python to perform certain tasks.",
-    long_description=long_description,
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
     author="Yash Mittal",
     author_email="akhil@codejudge.io",
     classifiers=
     [
         "Environment :: Web Environment",
         "Framework :: Django",
         "Framework :: Django :: 4.2",
```

