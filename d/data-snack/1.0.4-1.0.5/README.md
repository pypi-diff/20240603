# Comparing `tmp/data_snack-1.0.4.tar.gz` & `tmp/data_snack-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_snack-1.0.4.tar", last modified: Wed May 22 11:20:14 2024, max compression
+gzip compressed data, was "data_snack-1.0.5.tar", last modified: Mon Jun  3 13:21:37 2024, max compression
```

## Comparing `data_snack-1.0.4.tar` & `data_snack-1.0.5.tar`

### file list

```diff
@@ -1,53 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:14.351044 data_snack-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-22 11:20:05.000000 data_snack-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-22 11:20:05.000000 data_snack-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-05-22 11:20:14.351044 data_snack-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-05-22 11:20:05.000000 data_snack-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-22 11:20:05.000000 data_snack-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-22 11:20:05.000000 data_snack-1.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-22 11:20:14.351044 data_snack-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-22 11:20:05.000000 data_snack-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:14.343044 data_snack-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:14.347044 data_snack-1.0.4/src/data_snack/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:14.347044 data_snack-1.0.4/src/data_snack/connections/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/connections/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/connections/memcached.py
--rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/connections/mongo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/connections/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:14.347044 data_snack-1.0.4/src/data_snack/entities/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/entities/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/entities/entity_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/entities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/entities/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/entities/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:14.351044 data_snack-1.0.4/src/data_snack/key_factories/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/key_factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/key_factories/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/key_factories/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/key_factories/hash.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/key_factories/non_cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:14.351044 data_snack-1.0.4/src/data_snack/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/serializers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/serializers/dataclass.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/serializers/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/snack.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:14.351044 data_snack-1.0.4/src/data_snack/wrap/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/wrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/wrap/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/wrap/data_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/wrap/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/wrap/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:14.351044 data_snack-1.0.4/src/data_snack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-05-22 11:20:14.000000 data_snack-1.0.4/src/data_snack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-22 11:20:14.000000 data_snack-1.0.4/src/data_snack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 11:20:14.000000 data_snack-1.0.4/src/data_snack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-22 11:20:14.000000 data_snack-1.0.4/src/data_snack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-22 11:20:14.000000 data_snack-1.0.4/src/data_snack.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:14.351044 data_snack-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-22 11:20:05.000000 data_snack-1.0.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:21:37.715973 data_snack-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-06-03 13:21:24.000000 data_snack-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-03 13:21:24.000000 data_snack-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-06-03 13:21:37.715973 data_snack-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-06-03 13:21:24.000000 data_snack-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-06-03 13:21:24.000000 data_snack-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-06-03 13:21:24.000000 data_snack-1.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-06-03 13:21:37.715973 data_snack-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-06-03 13:21:24.000000 data_snack-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:21:37.707973 data_snack-1.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:21:37.707973 data_snack-1.0.5/src/data_snack/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-06-03 13:21:24.000000 data_snack-1.0.5/src/data_snack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:21:37.711973 data_snack-1.0.5/src/data_snack/connections/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-06-03 13:21:24.000000 data_snack-1.0.5/src/data_snack/connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-06-03 13:21:24.000000 data_snack-1.0.5/src/data_snack/connections/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-06-03 13:21:24.000000 data_snack-1.0.5/src/data_snack/connections/memcached.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-06-03 13:21:24.000000 data_snack-1.0.5/src/data_snack/connections/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-06-03 13:21:24.000000 data_snack-1.0.5/src/data_snack/connections/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:21:37.711973 data_snack-1.0.5/src/data_snack/entities/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-06-03 13:21:24.000000 data_snack-1.0.5/src/data_snack/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-06-03 13:21:24.000000 data_snack-1.0.5/src/data_snack/entities/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-06-03 13:21:24.000000 data_snack-1.0.5/src/data_snack/entities/compound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-06-03 13:21:24.000000 data_snack-1.0.5/src/data_snack/entities/entity_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-06-03 13:21:24.000000 data_snack-1.0.5/src/data_snack/entities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-06-03 13:21:24.000000 data_snack-1.0.5/src/data_snack/entities/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-06-03 13:21:24.000000 data_snack-1.0.5/src/data_snack/entities/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-06-03 13:21:24.000000 data_snack-1.0.5/src/data_snack/entities/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-06-03 13:21:24.000000 data_snack-1.0.5/src/data_snack/entities/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-06-03 13:21:24.000000 data_snack-1.0.5/src/data_snack/entities/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-06-03 13:21:24.000000 data_snack-1.0.5/src/data_snack/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:21:37.711973 data_snack-1.0.5/src/data_snack/key_factories/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-06-03 13:21:24.000000 data_snack-1.0.5/src/data_snack/key_factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-06-03 13:21:24.000000 data_snack-1.0.5/src/data_snack/key_factories/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-06-03 13:21:24.000000 data_snack-1.0.5/src/data_snack/key_factories/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-06-03 13:21:24.000000 data_snack-1.0.5/src/data_snack/key_factories/hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-06-03 13:21:24.000000 data_snack-1.0.5/src/data_snack/key_factories/non_cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:21:37.711973 data_snack-1.0.5/src/data_snack/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-06-03 13:21:24.000000 data_snack-1.0.5/src/data_snack/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-06-03 13:21:24.000000 data_snack-1.0.5/src/data_snack/serializers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-06-03 13:21:24.000000 data_snack-1.0.5/src/data_snack/serializers/dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-06-03 13:21:24.000000 data_snack-1.0.5/src/data_snack/serializers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9594 2024-06-03 13:21:24.000000 data_snack-1.0.5/src/data_snack/snack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-06-03 13:21:24.000000 data_snack-1.0.5/src/data_snack/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:21:37.711973 data_snack-1.0.5/src/data_snack/wrap/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-06-03 13:21:24.000000 data_snack-1.0.5/src/data_snack/wrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-06-03 13:21:24.000000 data_snack-1.0.5/src/data_snack/wrap/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-06-03 13:21:24.000000 data_snack-1.0.5/src/data_snack/wrap/data_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-06-03 13:21:24.000000 data_snack-1.0.5/src/data_snack/wrap/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-06-03 13:21:24.000000 data_snack-1.0.5/src/data_snack/wrap/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:21:37.715973 data_snack-1.0.5/src/data_snack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-06-03 13:21:37.000000 data_snack-1.0.5/src/data_snack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-06-03 13:21:37.000000 data_snack-1.0.5/src/data_snack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 13:21:37.000000 data_snack-1.0.5/src/data_snack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-06-03 13:21:37.000000 data_snack-1.0.5/src/data_snack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-03 13:21:37.000000 data_snack-1.0.5/src/data_snack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:21:37.715973 data_snack-1.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-06-03 13:21:24.000000 data_snack-1.0.5/tests/test_utils.py
```

### Comparing `data_snack-1.0.4/LICENSE` & `data_snack-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.4/PKG-INFO` & `data_snack-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data_snack
-Version: 1.0.4
+Version: 1.0.5
 Home-page: https://github.com/webinterpret-ds/data-snack
 Author: webinterpret-datascience
 Author-email: data-science@webinterpret.com
 Project-URL: Bug Tracker, https://github.com/webinterpret-ds/data-snack/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `data_snack-1.0.4/README.md` & `data_snack-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.4/setup.cfg` & `data_snack-1.0.5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = data-snack
-version = 1.0.4
+version = 1.0.5
 author = webinterpret-datascience
 author_email = data-science@webinterpret.com
 description = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/webinterpret-ds/data-snack
 project_urls =
```

### Comparing `data_snack-1.0.4/setup.py` & `data_snack-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.4/src/data_snack/connections/base.py` & `data_snack-1.0.5/src/data_snack/connections/base.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.4/src/data_snack/connections/memcached.py` & `data_snack-1.0.5/src/data_snack/connections/memcached.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.4/src/data_snack/connections/mongo.py` & `data_snack-1.0.5/src/data_snack/connections/mongo.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.4/src/data_snack/connections/redis.py` & `data_snack-1.0.5/src/data_snack/connections/redis.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.4/src/data_snack/entities/entity.py` & `data_snack-1.0.5/src/data_snack/entities/base.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.4/src/data_snack/entities/schema.py` & `data_snack-1.0.5/src/data_snack/entities/schema.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, Callable, Dict, Type, get_type_hints
 
-from data_snack.entities import Entity
+from data_snack.entities.base import Entity
 
 EntitySchemaGetter = Callable[[Type[Entity], bool], Dict[str, Any]]
 
 
 def get_entity_schema(
     entity_type: Type[Entity], exclude_fields: bool = False
 ) -> Dict[str, Any]:
```

### Comparing `data_snack-1.0.4/src/data_snack/key_factories/base.py` & `data_snack-1.0.5/src/data_snack/key_factories/base.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.4/src/data_snack/serializers/base.py` & `data_snack-1.0.5/src/data_snack/serializers/base.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.4/src/data_snack/serializers/dataclass.py` & `data_snack-1.0.5/src/data_snack/serializers/dataclass.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.4/src/data_snack/serializers/json.py` & `data_snack-1.0.5/src/data_snack/serializers/json.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.4/src/data_snack/snack.py` & `data_snack-1.0.5/src/data_snack/snack.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+from collections import ChainMap
 from dataclasses import dataclass, field
-from typing import Any, List, Optional, Type
+from typing import Any, List, Optional, Type, Union
 
 from data_snack.connections import Connection
 from data_snack.entities import Entity, EntityRegistry
+from data_snack.entities.compound import CompoundEntity
+from data_snack.entities.utils import map_values
 from data_snack.exceptions import EntityAlreadyRegistered
 from data_snack.key_factories import Key, NonClusterKey
 from data_snack.serializers import DataclassSerializer, Serializer
 from data_snack.utils import get_attribute_of_first_element_from_iterable
 from data_snack.wrap import EntityWrap
 
 
@@ -71,54 +74,123 @@
         :return: on success returns key used for the object, None on fail
         """
         key = self._build_record_key(entity)
         record = self._get_serializer(entity.__class__).serialize(entity)
         if self.connection.set(key, record):
             return key.keystring  # Should we return keystring or maybe just a key?
 
-    def get(self, cls: Type[Entity], key_values: List[Any]) -> Optional[Entity]:
+    def _get(self, cls: Type[Entity], key_values: List[Any]) -> Optional[Entity]:
         """
         Gets ane entity of `Entity` type from db based on provided key values.
-        Notice, key is represented as a list of strings, since one Entity can have multiple key fields.
 
         :param cls: `Entity` type
         :param key_values: a list of key values representing the entity
         :return: a retrieved Entity object
         """
         _key = self.key_factory(cls, key_values)
         value = self.connection.get(_key)
         return self._get_serializer(cls).deserialize(value)
 
+    def _get_compound(self, cls: Type[CompoundEntity], key_values: List[Any]) -> Optional[CompoundEntity]:
+        """
+        Gets ane entity of `CompoundEntity` type as collection of source entities based on provided key values.
+
+        :param cls: `CompoundEntity` type
+        :param key_values: a list of key values representing the compound entity
+        :return: a retrieved CompoundEntity object
+        """
+        source_entities = []
+        for source in cls.Meta.sources:
+            mapped_keys = map_values(source.fields_mapping, cls.get_keys())
+            mapped_key_values = [key_values[idx] for idx, key in enumerate(mapped_keys) if key]
+            source_entities.append(self._get(source.entity, mapped_key_values))
+        return cls.create_from_source_entities(source_entities) if all(source_entities) else None
+
+    def get(
+            self, cls: Union[Type[Entity], Type[CompoundEntity]], key_values: List[Any]
+    ) -> Optional[Union[Entity, CompoundEntity]]:
+        """
+        Gets one entity depending on type from db based on provided key values.
+        Notice, key is represented as a list of strings, since one entity can have multiple key fields.
+
+        :param cls: `Entity` or `CompoundEntity` type
+        :param key_values: a list of key values representing the entity
+        :return: a retrieved `Entity` or `CompoundEntity` object
+        """
+        if issubclass(cls, Entity):
+            return self._get(cls, key_values)
+        elif issubclass(cls, CompoundEntity):
+            return self._get_compound(cls, key_values)
+
     def delete(self, cls: Type[Entity], key_values: List[Any]) -> bool:
         """
         Deletes one entity of `Entity` type from db based on provided key values.
         Notice, key is represented as a list of strings, since one Entity can have multiple key fields.
 
         :param cls: `Entity` type
         :param key_values: a list of key values representing the entity
         :return: True if data were deleted
         """
         _key = self.key_factory(cls, key_values)
         return self.connection.delete(_key)
 
-    def get_many(
+    def _get_many(
         self, cls: Type[Entity], keys_values: List[List[Any]]
     ) -> List[Optional[Entity]]:
         """
         Gets list of `Entity` objects from db based on provided list of keys.
 
         :param cls: `Entity` type
         :param keys_values: list of keys, each list defines a set key values for one Entity object
         :return: a list of retrieved Entity objects
         """
         _keys = [self.key_factory(cls, key_values) for key_values in keys_values]
         results_unordered = self.connection.get_many(_keys)
         records_ordered = [results_unordered.get(key.keystring) for key in _keys]
         return self._get_serializer(cls).deserialize(records_ordered, many=True)
 
+    def _get_many_compound(
+        self, cls: Type[CompoundEntity], keys_values: List[List[Any]]
+    ) -> List[Optional[CompoundEntity]]:
+        """
+        Gets list of `CompoundEntity` objects as collections of source entities based on provided key values.
+
+        :param cls: `CompoundEntity` type
+        :param keys_values: list of keys, each list defines a set key values for one CompoundEntity object
+        :return: a list of retrieved CompoundEntity objects
+        """
+        source_entities = []
+        for source in cls.Meta.sources:
+            mapped_keys = map_values(source.fields_mapping, cls.get_keys())
+            mapped_keys_values = [
+                [key_values[index] for index, key in enumerate(mapped_keys) if key]
+                for key_values in keys_values
+            ]
+            source_entities.append(self._get_many(source.entity, mapped_keys_values))
+        return [
+            cls.create_from_source_entities(entities) if all(entities) else None
+            for entities in zip(*source_entities)
+        ]
+
+    def get_many(
+        self, cls: Union[Type[Entity], Type[CompoundEntity]], keys_values: List[List[Any]]
+    ) -> List[Optional[Union[Entity, CompoundEntity]]]:
+        """
+        Gets list of entity objects depending on type from db based on provided key values.
+        Notice, key is represented as a list of strings, since one entity can have multiple key fields.
+
+        :param cls: `Entity` or `CompoundEntity` type
+        :param keys_values: list of keys, each list defines a set key values for one entity object
+        :return: a list of retrieved `Entity` or `CompoundEntity` objects
+        """
+        if issubclass(cls, Entity):
+            return self._get_many(cls, keys_values)
+        elif issubclass(cls, CompoundEntity):
+            return self._get_many_compound(cls, keys_values)
+
     def set_many(self, entities: List[Entity]) -> Any:
         """
         Saves multiple `Entity` objects in db.
 
         :param entities: a list of Entity objects
         :return: a list of keys generated for saved objects
         """
```

### Comparing `data_snack-1.0.4/src/data_snack/wrap/base.py` & `data_snack-1.0.5/src/data_snack/wrap/base.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.4/src/data_snack/wrap/data_frame.py` & `data_snack-1.0.5/src/data_snack/wrap/data_frame.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.4/src/data_snack/wrap/entity.py` & `data_snack-1.0.5/src/data_snack/wrap/entity.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.4/src/data_snack.egg-info/PKG-INFO` & `data_snack-1.0.5/src/data_snack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data_snack
-Version: 1.0.4
+Version: 1.0.5
 Home-page: https://github.com/webinterpret-ds/data-snack
 Author: webinterpret-datascience
 Author-email: data-science@webinterpret.com
 Project-URL: Bug Tracker, https://github.com/webinterpret-ds/data-snack/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `data_snack-1.0.4/src/data_snack.egg-info/SOURCES.txt` & `data_snack-1.0.5/src/data_snack.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -16,19 +16,23 @@
 src/data_snack.egg-info/top_level.txt
 src/data_snack/connections/__init__.py
 src/data_snack/connections/base.py
 src/data_snack/connections/memcached.py
 src/data_snack/connections/mongo.py
 src/data_snack/connections/redis.py
 src/data_snack/entities/__init__.py
-src/data_snack/entities/entity.py
+src/data_snack/entities/base.py
+src/data_snack/entities/compound.py
 src/data_snack/entities/entity_meta.py
 src/data_snack/entities/exceptions.py
+src/data_snack/entities/models.py
 src/data_snack/entities/registry.py
 src/data_snack/entities/schema.py
+src/data_snack/entities/utils.py
+src/data_snack/entities/validation.py
 src/data_snack/key_factories/__init__.py
 src/data_snack/key_factories/base.py
 src/data_snack/key_factories/cluster.py
 src/data_snack/key_factories/hash.py
 src/data_snack/key_factories/non_cluster.py
 src/data_snack/serializers/__init__.py
 src/data_snack/serializers/base.py
```

### Comparing `data_snack-1.0.4/tests/test_utils.py` & `data_snack-1.0.5/tests/test_utils.py`

 * *Files identical despite different names*

