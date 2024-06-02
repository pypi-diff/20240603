# Comparing `tmp/graphene_cruddals-0.2.0.tar.gz` & `tmp/graphene_cruddals-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphene_cruddals-0.2.0.tar", last modified: Sun Jun  2 23:50:27 2024, max compression
+gzip compressed data, was "graphene_cruddals-0.2.6.tar", last modified: Sun Jun  2 23:50:53 2024, max compression
```

## Comparing `graphene_cruddals-0.2.0.tar` & `graphene_cruddals-0.2.6.tar`

### file list

```diff
@@ -1,34 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 23:50:27.450590 graphene_cruddals-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    10254 2024-06-02 23:50:20.000000 graphene_cruddals-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-06-02 23:50:20.000000 graphene_cruddals-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-06-02 23:50:27.450590 graphene_cruddals-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-06-02 23:50:20.000000 graphene_cruddals-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 23:50:27.446590 graphene_cruddals-0.2.0/graphene_cruddals/
--rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-06-02 23:50:20.000000 graphene_cruddals-0.2.0/graphene_cruddals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46029 2024-06-02 23:50:20.000000 graphene_cruddals-0.2.0/graphene_cruddals/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 23:50:27.446590 graphene_cruddals-0.2.0/graphene_cruddals/operation_fields/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 23:50:20.000000 graphene_cruddals-0.2.0/graphene_cruddals/operation_fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13952 2024-06-02 23:50:20.000000 graphene_cruddals-0.2.0/graphene_cruddals/operation_fields/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 23:50:27.446590 graphene_cruddals-0.2.0/graphene_cruddals/registry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 23:50:20.000000 graphene_cruddals-0.2.0/graphene_cruddals/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-06-02 23:50:20.000000 graphene_cruddals-0.2.0/graphene_cruddals/registry/registry_global.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 23:50:27.450590 graphene_cruddals-0.2.0/graphene_cruddals/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 23:50:20.000000 graphene_cruddals-0.2.0/graphene_cruddals/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-06-02 23:50:20.000000 graphene_cruddals-0.2.0/graphene_cruddals/types/error_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    12178 2024-06-02 23:50:20.000000 graphene_cruddals-0.2.0/graphene_cruddals/types/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    15174 2024-06-02 23:50:20.000000 graphene_cruddals-0.2.0/graphene_cruddals/types/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 23:50:27.450590 graphene_cruddals-0.2.0/graphene_cruddals/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 23:50:20.000000 graphene_cruddals-0.2.0/graphene_cruddals/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17808 2024-06-02 23:50:20.000000 graphene_cruddals-0.2.0/graphene_cruddals/utils/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 23:50:27.450590 graphene_cruddals-0.2.0/graphene_cruddals/utils/typing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 23:50:20.000000 graphene_cruddals-0.2.0/graphene_cruddals/utils/typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-06-02 23:50:20.000000 graphene_cruddals-0.2.0/graphene_cruddals/utils/typing/custom_typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 23:50:27.446590 graphene_cruddals-0.2.0/graphene_cruddals.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-06-02 23:50:27.000000 graphene_cruddals-0.2.0/graphene_cruddals.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-06-02 23:50:27.000000 graphene_cruddals-0.2.0/graphene_cruddals.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 23:50:27.000000 graphene_cruddals-0.2.0/graphene_cruddals.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 23:50:27.000000 graphene_cruddals-0.2.0/graphene_cruddals.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-06-02 23:50:27.000000 graphene_cruddals-0.2.0/graphene_cruddals.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-02 23:50:27.000000 graphene_cruddals-0.2.0/graphene_cruddals.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-06-02 23:50:27.450590 graphene_cruddals-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-06-02 23:50:20.000000 graphene_cruddals-0.2.0/setup.py
+drwxrwxr-x   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-06-02 23:50:53.844702 graphene_cruddals-0.2.6/
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)    10254 2024-05-29 11:55:19.000000 graphene_cruddals-0.2.6/LICENSE
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)       26 2024-04-28 03:54:55.000000 graphene_cruddals-0.2.6/MANIFEST.in
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     3874 2024-06-02 23:50:53.844702 graphene_cruddals-0.2.6/PKG-INFO
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     2888 2024-05-29 17:03:24.000000 graphene_cruddals-0.2.6/README.md
+drwxrwxr-x   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-06-02 23:50:53.824702 graphene_cruddals-0.2.6/graphene_cruddals/
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     4593 2024-06-02 23:50:20.000000 graphene_cruddals-0.2.6/graphene_cruddals/__init__.py
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)    46029 2024-06-02 17:30:25.000000 graphene_cruddals-0.2.6/graphene_cruddals/main.py
+drwxrwxr-x   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-06-02 23:50:53.832702 graphene_cruddals-0.2.6/graphene_cruddals/operation_fields/
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-04-24 02:45:24.000000 graphene_cruddals-0.2.6/graphene_cruddals/operation_fields/__init__.py
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)    13952 2024-06-01 12:52:43.000000 graphene_cruddals-0.2.6/graphene_cruddals/operation_fields/main.py
+drwxrwxr-x   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-06-02 23:50:53.836702 graphene_cruddals-0.2.6/graphene_cruddals/registry/
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-04-26 16:57:02.000000 graphene_cruddals-0.2.6/graphene_cruddals/registry/__init__.py
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     4691 2024-05-30 21:18:53.000000 graphene_cruddals-0.2.6/graphene_cruddals/registry/registry_global.py
+drwxrwxr-x   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-06-02 23:50:53.840702 graphene_cruddals-0.2.6/graphene_cruddals/types/
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-04-28 18:50:06.000000 graphene_cruddals-0.2.6/graphene_cruddals/types/__init__.py
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     1971 2024-05-25 04:06:09.000000 graphene_cruddals-0.2.6/graphene_cruddals/types/error_types.py
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)    12178 2024-06-02 22:31:44.000000 graphene_cruddals-0.2.6/graphene_cruddals/types/main.py
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)    15174 2024-06-02 17:30:25.000000 graphene_cruddals-0.2.6/graphene_cruddals/types/utils.py
+drwxrwxr-x   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-06-02 23:50:53.840702 graphene_cruddals-0.2.6/graphene_cruddals/utils/
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-04-24 02:48:51.000000 graphene_cruddals-0.2.6/graphene_cruddals/utils/__init__.py
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)    17808 2024-05-30 21:11:33.000000 graphene_cruddals-0.2.6/graphene_cruddals/utils/main.py
+drwxrwxr-x   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-06-02 23:50:53.844702 graphene_cruddals-0.2.6/graphene_cruddals/utils/typing/
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-04-24 03:01:40.000000 graphene_cruddals-0.2.6/graphene_cruddals/utils/typing/__init__.py
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     6367 2024-04-28 15:59:30.000000 graphene_cruddals-0.2.6/graphene_cruddals/utils/typing/custom_typing.py
+drwxrwxr-x   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-06-02 23:50:53.832702 graphene_cruddals-0.2.6/graphene_cruddals.egg-info/
+-rw-r--r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     3874 2024-06-02 23:50:53.000000 graphene_cruddals-0.2.6/graphene_cruddals.egg-info/PKG-INFO
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     1032 2024-06-02 23:50:53.000000 graphene_cruddals-0.2.6/graphene_cruddals.egg-info/SOURCES.txt
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)        1 2024-06-02 23:50:53.000000 graphene_cruddals-0.2.6/graphene_cruddals.egg-info/dependency_links.txt
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)        1 2024-05-24 21:10:55.000000 graphene_cruddals-0.2.6/graphene_cruddals.egg-info/not-zip-safe
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)      184 2024-06-02 23:50:53.000000 graphene_cruddals-0.2.6/graphene_cruddals.egg-info/requires.txt
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)       18 2024-06-02 23:50:53.000000 graphene_cruddals-0.2.6/graphene_cruddals.egg-info/top_level.txt
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)      165 2024-06-02 23:50:53.844702 graphene_cruddals-0.2.6/setup.cfg
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     1832 2024-05-25 01:52:32.000000 graphene_cruddals-0.2.6/setup.py
+drwxrwxr-x   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-06-02 23:50:53.844702 graphene_cruddals-0.2.6/tests/
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)    28445 2024-06-02 17:30:25.000000 graphene_cruddals-0.2.6/tests/test_main.py
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)    34512 2024-06-01 22:02:38.000000 graphene_cruddals-0.2.6/tests/test_operation_fields_main.py
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     2189 2024-05-30 09:35:18.000000 graphene_cruddals-0.2.6/tests/test_registry_registry_global.py
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)    23264 2024-06-01 15:10:11.000000 graphene_cruddals-0.2.6/tests/test_type_main.py
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)    15536 2024-06-01 15:11:36.000000 graphene_cruddals-0.2.6/tests/test_types_utils.py
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     7146 2024-05-29 16:53:40.000000 graphene_cruddals-0.2.6/tests/test_utils_main.py
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-04-28 15:54:18.000000 graphene_cruddals-0.2.6/tests/test_utils_typing_custom_typing.py
```

### Comparing `graphene_cruddals-0.2.0/LICENSE` & `graphene_cruddals-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `graphene_cruddals-0.2.0/PKG-INFO` & `graphene_cruddals-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphene_cruddals
-Version: 0.2.0
+Version: 0.2.6
 Summary: Library base for create others libraries with the objective of create a CRUD+DALS with GraphQL
 Home-page: https://github.com/juanjcardona13/graphene_cruddals
 Author: Juan J Cardona
 Author-email: juanjcardona13@gmail.com
 License: Apache 2.0
 Keywords: api graphql crud graphene cruddals
 Platform: any
@@ -15,16 +15,16 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Description-Content-Type: text/markdown
-Provides-Extra: test
 Provides-Extra: dev
+Provides-Extra: test
 License-File: LICENSE
 
 
 
 <h1 align="center">Graphene-CRUDDALS</h1>
 <div align="center">
 
@@ -86,7 +86,9 @@
 - [LinkedIn](https://www.linkedin.com/in/juanjcardona/)
 - [GitHub](https://github.com/juanjcardona13)
 
 ## <a name="acknowledgements">🙏 Acknowledgements</a>
 
 - [Python](https://www.python.org/)
 - [Graphene ](https://docs.graphene-python.org/projects/django/en/latest/)
+
+
```

### Comparing `graphene_cruddals-0.2.0/README.md` & `graphene_cruddals-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `graphene_cruddals-0.2.0/graphene_cruddals/__init__.py` & `graphene_cruddals-0.2.6/graphene_cruddals/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     TypeRegistryForFieldEnum,
     TypeRegistryForModel,
     TypeRegistryForModelEnum,
     TypesMutation,
     TypesMutationEnum,
 )
 
-__version__ = "0.2.0"
+__version__ = "0.2.6"
 
 __all__ = [
     "__version__",
     "CruddalsBuilderConfig",
     "BaseCruddals",
     "BuilderCruddalsModel",
     "CruddalsModel",
```

### Comparing `graphene_cruddals-0.2.0/graphene_cruddals/main.py` & `graphene_cruddals-0.2.6/graphene_cruddals/main.py`

 * *Files identical despite different names*

### Comparing `graphene_cruddals-0.2.0/graphene_cruddals/operation_fields/main.py` & `graphene_cruddals-0.2.6/graphene_cruddals/operation_fields/main.py`

 * *Files identical despite different names*

### Comparing `graphene_cruddals-0.2.0/graphene_cruddals/registry/registry_global.py` & `graphene_cruddals-0.2.6/graphene_cruddals/registry/registry_global.py`

 * *Files identical despite different names*

### Comparing `graphene_cruddals-0.2.0/graphene_cruddals/types/error_types.py` & `graphene_cruddals-0.2.6/graphene_cruddals/types/error_types.py`

 * *Files identical despite different names*

### Comparing `graphene_cruddals-0.2.0/graphene_cruddals/types/main.py` & `graphene_cruddals-0.2.6/graphene_cruddals/types/main.py`

 * *Files identical despite different names*

### Comparing `graphene_cruddals-0.2.0/graphene_cruddals/types/utils.py` & `graphene_cruddals-0.2.6/graphene_cruddals/types/utils.py`

 * *Files identical despite different names*

### Comparing `graphene_cruddals-0.2.0/graphene_cruddals/utils/main.py` & `graphene_cruddals-0.2.6/graphene_cruddals/utils/main.py`

 * *Files identical despite different names*

### Comparing `graphene_cruddals-0.2.0/graphene_cruddals/utils/typing/custom_typing.py` & `graphene_cruddals-0.2.6/graphene_cruddals/utils/typing/custom_typing.py`

 * *Files identical despite different names*

### Comparing `graphene_cruddals-0.2.0/graphene_cruddals.egg-info/PKG-INFO` & `graphene_cruddals-0.2.6/graphene_cruddals.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphene-cruddals
-Version: 0.2.0
+Version: 0.2.6
 Summary: Library base for create others libraries with the objective of create a CRUD+DALS with GraphQL
 Home-page: https://github.com/juanjcardona13/graphene_cruddals
 Author: Juan J Cardona
 Author-email: juanjcardona13@gmail.com
 License: Apache 2.0
 Keywords: api graphql crud graphene cruddals
 Platform: any
@@ -15,16 +15,16 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Description-Content-Type: text/markdown
-Provides-Extra: test
 Provides-Extra: dev
+Provides-Extra: test
 License-File: LICENSE
 
 
 
 <h1 align="center">Graphene-CRUDDALS</h1>
 <div align="center">
 
@@ -86,7 +86,9 @@
 - [LinkedIn](https://www.linkedin.com/in/juanjcardona/)
 - [GitHub](https://github.com/juanjcardona13)
 
 ## <a name="acknowledgements">🙏 Acknowledgements</a>
 
 - [Python](https://www.python.org/)
 - [Graphene ](https://docs.graphene-python.org/projects/django/en/latest/)
+
+
```

### Comparing `graphene_cruddals-0.2.0/setup.py` & `graphene_cruddals-0.2.6/setup.py`

 * *Files identical despite different names*

