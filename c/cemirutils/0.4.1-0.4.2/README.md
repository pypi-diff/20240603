# Comparing `tmp/cemirutils-0.4.1.tar.gz` & `tmp/cemirutils-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cemirutils-0.4.1.tar", last modified: Mon Jun  3 10:39:12 2024, max compression
+gzip compressed data, was "cemirutils-0.4.2.tar", last modified: Mon Jun  3 10:55:44 2024, max compression
```

## Comparing `cemirutils-0.4.1.tar` & `cemirutils-0.4.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 muslu     (1000) muslu     (1000)        0 2024-06-03 10:39:12.734598 cemirutils-0.4.1/
--rw-rw-r--   0 muslu     (1000) muslu     (1000)        0 2024-06-03 07:24:46.000000 cemirutils-0.4.1/LICENSE
--rw-r--r--   0 muslu     (1000) muslu     (1000)     5294 2024-06-03 10:39:12.734598 cemirutils-0.4.1/PKG-INFO
--rw-rw-r--   0 muslu     (1000) muslu     (1000)     4830 2024-06-03 10:36:07.000000 cemirutils-0.4.1/README.md
-drwxrwxr-x   0 muslu     (1000) muslu     (1000)        0 2024-06-03 10:39:12.734598 cemirutils-0.4.1/cemirutils/
--rw-rw-r--   0 muslu     (1000) muslu     (1000)      140 2024-06-03 07:24:46.000000 cemirutils-0.4.1/cemirutils/__init__.py
--rw-rw-r--   0 muslu     (1000) muslu     (1000)    30488 2024-06-03 10:33:45.000000 cemirutils-0.4.1/cemirutils/utils.py
-drwxrwxr-x   0 muslu     (1000) muslu     (1000)        0 2024-06-03 10:39:12.734598 cemirutils-0.4.1/cemirutils.egg-info/
--rw-r--r--   0 muslu     (1000) muslu     (1000)     5294 2024-06-03 10:39:12.000000 cemirutils-0.4.1/cemirutils.egg-info/PKG-INFO
--rw-rw-r--   0 muslu     (1000) muslu     (1000)      205 2024-06-03 10:39:12.000000 cemirutils-0.4.1/cemirutils.egg-info/SOURCES.txt
--rw-rw-r--   0 muslu     (1000) muslu     (1000)        1 2024-06-03 10:39:12.000000 cemirutils-0.4.1/cemirutils.egg-info/dependency_links.txt
--rw-rw-r--   0 muslu     (1000) muslu     (1000)       11 2024-06-03 10:39:12.000000 cemirutils-0.4.1/cemirutils.egg-info/top_level.txt
--rw-rw-r--   0 muslu     (1000) muslu     (1000)       38 2024-06-03 10:39:12.734598 cemirutils-0.4.1/setup.cfg
--rw-rw-r--   0 muslu     (1000) muslu     (1000)      677 2024-06-03 10:36:54.000000 cemirutils-0.4.1/setup.py
+drwxrwxr-x   0 muslu     (1000) muslu     (1000)        0 2024-06-03 10:55:44.230614 cemirutils-0.4.2/
+-rw-rw-r--   0 muslu     (1000) muslu     (1000)        0 2024-06-03 07:24:46.000000 cemirutils-0.4.2/LICENSE
+-rw-r--r--   0 muslu     (1000) muslu     (1000)     5519 2024-06-03 10:55:44.230614 cemirutils-0.4.2/PKG-INFO
+-rw-rw-r--   0 muslu     (1000) muslu     (1000)     5055 2024-06-03 10:53:24.000000 cemirutils-0.4.2/README.md
+drwxrwxr-x   0 muslu     (1000) muslu     (1000)        0 2024-06-03 10:55:44.230614 cemirutils-0.4.2/cemirutils/
+-rw-rw-r--   0 muslu     (1000) muslu     (1000)      140 2024-06-03 07:24:46.000000 cemirutils-0.4.2/cemirutils/__init__.py
+-rw-rw-r--   0 muslu     (1000) muslu     (1000)    30488 2024-06-03 10:33:45.000000 cemirutils-0.4.2/cemirutils/utils.py
+drwxrwxr-x   0 muslu     (1000) muslu     (1000)        0 2024-06-03 10:55:44.230614 cemirutils-0.4.2/cemirutils.egg-info/
+-rw-r--r--   0 muslu     (1000) muslu     (1000)     5519 2024-06-03 10:55:44.000000 cemirutils-0.4.2/cemirutils.egg-info/PKG-INFO
+-rw-rw-r--   0 muslu     (1000) muslu     (1000)      205 2024-06-03 10:55:44.000000 cemirutils-0.4.2/cemirutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 muslu     (1000) muslu     (1000)        1 2024-06-03 10:55:44.000000 cemirutils-0.4.2/cemirutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 muslu     (1000) muslu     (1000)       11 2024-06-03 10:55:44.000000 cemirutils-0.4.2/cemirutils.egg-info/top_level.txt
+-rw-rw-r--   0 muslu     (1000) muslu     (1000)       38 2024-06-03 10:55:44.230614 cemirutils-0.4.2/setup.cfg
+-rw-rw-r--   0 muslu     (1000) muslu     (1000)      677 2024-06-03 10:55:31.000000 cemirutils-0.4.2/setup.py
```

### Comparing `cemirutils-0.4.1/PKG-INFO` & `cemirutils-0.4.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cemirutils
-Version: 0.4.1
+Version: 0.4.2
 Summary: Basit veri işleme ve SQL yardımcıları
 Home-page: https://github.com/cememir/cemirutils
 Author: Cem Emir / Muslu Yüksektepe
 Author-email: musluyuksektepe@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -29,28 +29,34 @@
 
 ## Kullanım
 
 
 
 
 * PostgreSQL için CRUD işlemleri.
+
 ```python
+from datetime import datetime
 from cemirutils import CemirUtils
 
 # Örnek kullanım
 utils = CemirUtils(data=False, dbname='test_db3', dbuser='postgres', dbpassword='', dbport=5435, dbcreate_db_if_not_exists=True)
 
-print(utils.psql_create_table('test_table_flat', 'id SERIAL PRIMARY KEY, name VARCHAR(100), surname VARCHAR(100)'))
-print(utils.psql_insert('test_table', ('id', 'name', 'data'), (3, "emir", {"age": 40, "city": "İzmir"}), get_id=True))
-print(utils.psql_insert('test_table_flat', ('id', 'name', 'surname'), (3, 'Muslu', 'Yüksektepe'), get_id=True))
-print(utils.psql_read('test_table'))
-print(utils.psql_read('test_table_flat'))
-print(utils.psql_update('test_table', {'name': 'MusluY', 'data': '{"age": 40, "city": "Sivas"}'}, 'id = 2', get_id=True))
-print(utils.psql_delete('test_table', 'id = 2'))
+# print(utils.psql_create_table('test_table_flat', 'id SERIAL PRIMARY KEY, name VARCHAR(100), surname VARCHAR(100)'))
+# print(utils.psql_create_table('test_table_json', 'id SERIAL PRIMARY KEY, dates DATE, content JSONB'))
+
+# print(utils.psql_insert('test_table_flat', ('id', 'name', 'surname'), (3, 'Muslu', 'Yüksektepe'), get_id=True))
+print(utils.psql_insert('test_table_json', ('id', 'dates', 'content'), (2, datetime.now(), {"age": 40, "city": "İzmir"}), get_id=True))
+print(utils.psql_read('test_table_json'))
+
+print(utils.psql_update('test_table_json', {'dates': datetime.now(), 'content': '{"age": 40, "city": "Sivas"}'}, 'id = 1', get_id=True))
+print(utils.psql_read('test_table_json'))
 
+print(utils.psql_delete('test_table_json', 'id = 1'))
+print(utils.psql_read('test_table_json'))
 ```
 
 Kütüphane, farklı veri işleme işlevlerini sağlayan `CemirUtils` sınıfını içerir.
 * Örneğin:
 
 ```python
 from cemirutils import CemirUtils
```

### Comparing `cemirutils-0.4.1/README.md` & `cemirutils-0.4.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -15,28 +15,34 @@
 
 ## Kullanım
 
 
 
 
 * PostgreSQL için CRUD işlemleri.
+
 ```python
+from datetime import datetime
 from cemirutils import CemirUtils
 
 # Örnek kullanım
 utils = CemirUtils(data=False, dbname='test_db3', dbuser='postgres', dbpassword='', dbport=5435, dbcreate_db_if_not_exists=True)
 
-print(utils.psql_create_table('test_table_flat', 'id SERIAL PRIMARY KEY, name VARCHAR(100), surname VARCHAR(100)'))
-print(utils.psql_insert('test_table', ('id', 'name', 'data'), (3, "emir", {"age": 40, "city": "İzmir"}), get_id=True))
-print(utils.psql_insert('test_table_flat', ('id', 'name', 'surname'), (3, 'Muslu', 'Yüksektepe'), get_id=True))
-print(utils.psql_read('test_table'))
-print(utils.psql_read('test_table_flat'))
-print(utils.psql_update('test_table', {'name': 'MusluY', 'data': '{"age": 40, "city": "Sivas"}'}, 'id = 2', get_id=True))
-print(utils.psql_delete('test_table', 'id = 2'))
+# print(utils.psql_create_table('test_table_flat', 'id SERIAL PRIMARY KEY, name VARCHAR(100), surname VARCHAR(100)'))
+# print(utils.psql_create_table('test_table_json', 'id SERIAL PRIMARY KEY, dates DATE, content JSONB'))
+
+# print(utils.psql_insert('test_table_flat', ('id', 'name', 'surname'), (3, 'Muslu', 'Yüksektepe'), get_id=True))
+print(utils.psql_insert('test_table_json', ('id', 'dates', 'content'), (2, datetime.now(), {"age": 40, "city": "İzmir"}), get_id=True))
+print(utils.psql_read('test_table_json'))
+
+print(utils.psql_update('test_table_json', {'dates': datetime.now(), 'content': '{"age": 40, "city": "Sivas"}'}, 'id = 1', get_id=True))
+print(utils.psql_read('test_table_json'))
 
+print(utils.psql_delete('test_table_json', 'id = 1'))
+print(utils.psql_read('test_table_json'))
 ```
 
 Kütüphane, farklı veri işleme işlevlerini sağlayan `CemirUtils` sınıfını içerir.
 * Örneğin:
 
 ```python
 from cemirutils import CemirUtils
```

### Comparing `cemirutils-0.4.1/cemirutils/utils.py` & `cemirutils-0.4.2/cemirutils/utils.py`

 * *Files identical despite different names*

### Comparing `cemirutils-0.4.1/cemirutils.egg-info/PKG-INFO` & `cemirutils-0.4.2/cemirutils.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cemirutils
-Version: 0.4.1
+Version: 0.4.2
 Summary: Basit veri işleme ve SQL yardımcıları
 Home-page: https://github.com/cememir/cemirutils
 Author: Cem Emir / Muslu Yüksektepe
 Author-email: musluyuksektepe@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -29,28 +29,34 @@
 
 ## Kullanım
 
 
 
 
 * PostgreSQL için CRUD işlemleri.
+
 ```python
+from datetime import datetime
 from cemirutils import CemirUtils
 
 # Örnek kullanım
 utils = CemirUtils(data=False, dbname='test_db3', dbuser='postgres', dbpassword='', dbport=5435, dbcreate_db_if_not_exists=True)
 
-print(utils.psql_create_table('test_table_flat', 'id SERIAL PRIMARY KEY, name VARCHAR(100), surname VARCHAR(100)'))
-print(utils.psql_insert('test_table', ('id', 'name', 'data'), (3, "emir", {"age": 40, "city": "İzmir"}), get_id=True))
-print(utils.psql_insert('test_table_flat', ('id', 'name', 'surname'), (3, 'Muslu', 'Yüksektepe'), get_id=True))
-print(utils.psql_read('test_table'))
-print(utils.psql_read('test_table_flat'))
-print(utils.psql_update('test_table', {'name': 'MusluY', 'data': '{"age": 40, "city": "Sivas"}'}, 'id = 2', get_id=True))
-print(utils.psql_delete('test_table', 'id = 2'))
+# print(utils.psql_create_table('test_table_flat', 'id SERIAL PRIMARY KEY, name VARCHAR(100), surname VARCHAR(100)'))
+# print(utils.psql_create_table('test_table_json', 'id SERIAL PRIMARY KEY, dates DATE, content JSONB'))
+
+# print(utils.psql_insert('test_table_flat', ('id', 'name', 'surname'), (3, 'Muslu', 'Yüksektepe'), get_id=True))
+print(utils.psql_insert('test_table_json', ('id', 'dates', 'content'), (2, datetime.now(), {"age": 40, "city": "İzmir"}), get_id=True))
+print(utils.psql_read('test_table_json'))
+
+print(utils.psql_update('test_table_json', {'dates': datetime.now(), 'content': '{"age": 40, "city": "Sivas"}'}, 'id = 1', get_id=True))
+print(utils.psql_read('test_table_json'))
 
+print(utils.psql_delete('test_table_json', 'id = 1'))
+print(utils.psql_read('test_table_json'))
 ```
 
 Kütüphane, farklı veri işleme işlevlerini sağlayan `CemirUtils` sınıfını içerir.
 * Örneğin:
 
 ```python
 from cemirutils import CemirUtils
```

### Comparing `cemirutils-0.4.1/setup.py` & `cemirutils-0.4.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
 setup(
     name='cemirutils',
-    version='0.4.1',
+    version='0.4.2',
     packages=find_packages(),
     install_requires=[],
     author='Cem Emir / Muslu Yüksektepe',
     author_email='musluyuksektepe@gmail.com',
     description='Basit veri işleme ve SQL yardımcıları',
     long_description=open('README.md', encoding="utf-8").read(),
     long_description_content_type='text/markdown',
```

