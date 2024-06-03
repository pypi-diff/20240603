# Comparing `tmp/ownlib-0.0.1b6.tar.gz` & `tmp/ownlib-0.0.1b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ownlib-0.0.1b6.tar", max compression
+gzip compressed data, was "ownlib-0.0.1b7.tar", max compression
```

## Comparing `ownlib-0.0.1b6.tar` & `ownlib-0.0.1b7.tar`

### file list

```diff
@@ -1,16 +1,19 @@
--rw-r--r--   0        0        0    35149 2022-10-30 19:22:48.704414 ownlib-0.0.1b6/LICENSE
--rw-r--r--   0        0        0      140 2024-03-03 12:27:11.775267 ownlib-0.0.1b6/README.md
--rw-r--r--   0        0        0      638 2024-05-21 19:17:21.972087 ownlib-0.0.1b6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-03 12:27:11.775267 ownlib-0.0.1b6/src/ownlib/__init__.py
--rw-r--r--   0        0        0     2181 2024-05-21 19:13:41.984078 ownlib-0.0.1b6/src/ownlib/class_person.py
--rw-r--r--   0        0        0     4503 2024-04-12 17:12:32.850420 ownlib-0.0.1b6/src/ownlib/class_whatsapp_message.py
--rw-r--r--   0        0        0    13461 2024-04-12 17:12:32.850420 ownlib-0.0.1b6/src/ownlib/functions_whatsapp_refueling.py
--rw-r--r--   0        0        0     2074 2024-04-12 17:12:32.850420 ownlib-0.0.1b6/src/ownlib/months.py
--rw-r--r--   0        0        0     9806 2024-04-12 17:12:32.850420 ownlib-0.0.1b6/src/ownlib/my_datalib.py
--rw-r--r--   0        0        0      390 2024-04-12 17:12:32.850420 ownlib-0.0.1b6/src/ownlib/my_fileio.py
--rw-r--r--   0        0        0     9496 2024-04-27 20:19:48.292053 ownlib-0.0.1b6/src/ownlib/mytinylib.py
--rw-r--r--   0        0        0     1708 2024-03-03 12:27:11.779267 ownlib-0.0.1b6/src/ownlib/one_s_uat_lib.py
--rw-r--r--   0        0        0      164 2024-03-03 12:27:11.779267 ownlib-0.0.1b6/src/ownlib/platon_settings.py
--rw-r--r--   0        0        0     5512 2024-04-26 05:53:41.129855 ownlib-0.0.1b6/src/ownlib/txt_lib.py
--rw-r--r--   0        0        0     2138 2024-04-12 17:12:32.850420 ownlib-0.0.1b6/src/ownlib/whapp_funcs.py
--rw-r--r--   0        0        0      702 1970-01-01 00:00:00.000000 ownlib-0.0.1b6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-10-30 19:22:48.704414 ownlib-0.0.1b7/LICENSE
+-rw-r--r--   0        0        0      140 2024-03-03 12:27:11.775267 ownlib-0.0.1b7/README.md
+-rw-r--r--   0        0        0      638 2024-06-03 13:11:53.676946 ownlib-0.0.1b7/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-03 12:27:11.775267 ownlib-0.0.1b7/src/ownlib/__init__.py
+-rw-r--r--   0        0        0     2181 2024-05-21 19:13:41.984078 ownlib-0.0.1b7/src/ownlib/class_person.py
+-rw-r--r--   0        0        0     4503 2024-04-12 17:12:32.850420 ownlib-0.0.1b7/src/ownlib/class_whatsapp_message.py
+-rw-r--r--   0        0        0      610 2024-06-03 12:48:38.692828 ownlib-0.0.1b7/src/ownlib/doc/Readme_xml_lib.md
+-rw-r--r--   0        0        0    13461 2024-04-12 17:12:32.850420 ownlib-0.0.1b7/src/ownlib/functions_whatsapp_refueling.py
+-rw-r--r--   0        0        0     2074 2024-04-12 17:12:32.850420 ownlib-0.0.1b7/src/ownlib/months.py
+-rw-r--r--   0        0        0     9806 2024-04-12 17:12:32.850420 ownlib-0.0.1b7/src/ownlib/my_datalib.py
+-rw-r--r--   0        0        0      390 2024-04-12 17:12:32.850420 ownlib-0.0.1b7/src/ownlib/my_fileio.py
+-rw-r--r--   0        0        0     9496 2024-04-27 20:19:48.292053 ownlib-0.0.1b7/src/ownlib/mytinylib.py
+-rw-r--r--   0        0        0     1708 2024-03-03 12:27:11.779267 ownlib-0.0.1b7/src/ownlib/one_s_uat_lib.py
+-rw-r--r--   0        0        0      164 2024-03-03 12:27:11.779267 ownlib-0.0.1b7/src/ownlib/platon_settings.py
+-rw-r--r--   0        0        0     4717 2024-06-03 13:08:36.228566 ownlib-0.0.1b7/src/ownlib/settings/xml_settings.py
+-rw-r--r--   0        0        0     5512 2024-04-26 05:53:41.129855 ownlib-0.0.1b7/src/ownlib/txt_lib.py
+-rw-r--r--   0        0        0     2138 2024-04-12 17:12:32.850420 ownlib-0.0.1b7/src/ownlib/whapp_funcs.py
+-rw-r--r--   0        0        0     3461 2024-06-03 13:08:36.224566 ownlib-0.0.1b7/src/ownlib/xml_lib.py
+-rw-r--r--   0        0        0      702 1970-01-01 00:00:00.000000 ownlib-0.0.1b7/PKG-INFO
```

### Comparing `ownlib-0.0.1b6/LICENSE` & `ownlib-0.0.1b7/LICENSE`

 * *Files identical despite different names*

### Comparing `ownlib-0.0.1b6/pyproject.toml` & `ownlib-0.0.1b7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ownlib"
-version = "0.0.1b6"
+version = "0.0.1b7"
 description = "Sample pypi project"
 authors = ["Андрей Мартынов <real.cloudhunter@gmail.com>"]
 license = "GNU"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `ownlib-0.0.1b6/src/ownlib/class_person.py` & `ownlib-0.0.1b7/src/ownlib/class_person.py`

 * *Files identical despite different names*

### Comparing `ownlib-0.0.1b6/src/ownlib/class_whatsapp_message.py` & `ownlib-0.0.1b7/src/ownlib/class_whatsapp_message.py`

 * *Files identical despite different names*

### Comparing `ownlib-0.0.1b6/src/ownlib/functions_whatsapp_refueling.py` & `ownlib-0.0.1b7/src/ownlib/functions_whatsapp_refueling.py`

 * *Files identical despite different names*

### Comparing `ownlib-0.0.1b6/src/ownlib/months.py` & `ownlib-0.0.1b7/src/ownlib/months.py`

 * *Files identical despite different names*

### Comparing `ownlib-0.0.1b6/src/ownlib/my_datalib.py` & `ownlib-0.0.1b7/src/ownlib/my_datalib.py`

 * *Files identical despite different names*

### Comparing `ownlib-0.0.1b6/src/ownlib/mytinylib.py` & `ownlib-0.0.1b7/src/ownlib/mytinylib.py`

 * *Files identical despite different names*

### Comparing `ownlib-0.0.1b6/src/ownlib/one_s_uat_lib.py` & `ownlib-0.0.1b7/src/ownlib/one_s_uat_lib.py`

 * *Files identical despite different names*

### Comparing `ownlib-0.0.1b6/src/ownlib/txt_lib.py` & `ownlib-0.0.1b7/src/ownlib/txt_lib.py`

 * *Files identical despite different names*

### Comparing `ownlib-0.0.1b6/src/ownlib/whapp_funcs.py` & `ownlib-0.0.1b7/src/ownlib/whapp_funcs.py`

 * *Files identical despite different names*

### Comparing `ownlib-0.0.1b6/PKG-INFO` & `ownlib-0.0.1b7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ownlib
-Version: 0.0.1b6
+Version: 0.0.1b7
 Summary: Sample pypi project
 License: GNU
 Author: Андрей Мартынов
 Author-email: real.cloudhunter@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

