# Comparing `tmp/data_snack_dynamic_entity-0.2.0.tar.gz` & `tmp/data_snack_dynamic_entity-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_snack_dynamic_entity-0.2.0.tar", last modified: Tue May 21 08:59:43 2024, max compression
+gzip compressed data, was "data_snack_dynamic_entity-0.3.0.tar", last modified: Mon Jun  3 14:10:05 2024, max compression
```

## Comparing `data_snack_dynamic_entity-0.2.0.tar` & `data_snack_dynamic_entity-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:59:43.179689 data_snack_dynamic_entity-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-21 08:59:38.000000 data_snack_dynamic_entity-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-21 08:59:38.000000 data_snack_dynamic_entity-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-21 08:59:43.179689 data_snack_dynamic_entity-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-21 08:59:38.000000 data_snack_dynamic_entity-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-21 08:59:38.000000 data_snack_dynamic_entity-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 08:59:38.000000 data_snack_dynamic_entity-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-21 08:59:43.179689 data_snack_dynamic_entity-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-21 08:59:38.000000 data_snack_dynamic_entity-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:59:43.175689 data_snack_dynamic_entity-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:59:43.175689 data_snack_dynamic_entity-0.2.0/src/data_snack_dynamic_entity/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-21 08:59:38.000000 data_snack_dynamic_entity-0.2.0/src/data_snack_dynamic_entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-21 08:59:38.000000 data_snack_dynamic_entity-0.2.0/src/data_snack_dynamic_entity/entityTemplates.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-05-21 08:59:38.000000 data_snack_dynamic_entity-0.2.0/src/data_snack_dynamic_entity/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-21 08:59:38.000000 data_snack_dynamic_entity-0.2.0/src/data_snack_dynamic_entity/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-21 08:59:38.000000 data_snack_dynamic_entity-0.2.0/src/data_snack_dynamic_entity/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:59:43.179689 data_snack_dynamic_entity-0.2.0/src/data_snack_dynamic_entity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-21 08:59:43.000000 data_snack_dynamic_entity-0.2.0/src/data_snack_dynamic_entity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-21 08:59:43.000000 data_snack_dynamic_entity-0.2.0/src/data_snack_dynamic_entity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 08:59:43.000000 data_snack_dynamic_entity-0.2.0/src/data_snack_dynamic_entity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-21 08:59:43.000000 data_snack_dynamic_entity-0.2.0/src/data_snack_dynamic_entity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-21 08:59:43.000000 data_snack_dynamic_entity-0.2.0/src/data_snack_dynamic_entity.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:10:05.473272 data_snack_dynamic_entity-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-06-03 14:09:55.000000 data_snack_dynamic_entity-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-06-03 14:09:55.000000 data_snack_dynamic_entity-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-06-03 14:10:05.473272 data_snack_dynamic_entity-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-06-03 14:09:55.000000 data_snack_dynamic_entity-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-06-03 14:09:55.000000 data_snack_dynamic_entity-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 14:09:55.000000 data_snack_dynamic_entity-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-06-03 14:10:05.473272 data_snack_dynamic_entity-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-06-03 14:09:55.000000 data_snack_dynamic_entity-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:10:05.465273 data_snack_dynamic_entity-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:10:05.469272 data_snack_dynamic_entity-0.3.0/src/data_snack_dynamic_entity/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:09:55.000000 data_snack_dynamic_entity-0.3.0/src/data_snack_dynamic_entity/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:10:05.473272 data_snack_dynamic_entity-0.3.0/src/data_snack_dynamic_entity/compound_entity/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:09:55.000000 data_snack_dynamic_entity-0.3.0/src/data_snack_dynamic_entity/compound_entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-06-03 14:09:55.000000 data_snack_dynamic_entity-0.3.0/src/data_snack_dynamic_entity/compound_entity/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-06-03 14:09:55.000000 data_snack_dynamic_entity-0.3.0/src/data_snack_dynamic_entity/compound_entity/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-06-03 14:09:55.000000 data_snack_dynamic_entity-0.3.0/src/data_snack_dynamic_entity/compound_entity/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-06-03 14:09:55.000000 data_snack_dynamic_entity-0.3.0/src/data_snack_dynamic_entity/entityTemplates.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-06-03 14:09:55.000000 data_snack_dynamic_entity-0.3.0/src/data_snack_dynamic_entity/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:10:05.473272 data_snack_dynamic_entity-0.3.0/src/data_snack_dynamic_entity/simple_entity/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:09:55.000000 data_snack_dynamic_entity-0.3.0/src/data_snack_dynamic_entity/simple_entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-06-03 14:09:55.000000 data_snack_dynamic_entity-0.3.0/src/data_snack_dynamic_entity/simple_entity/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-06-03 14:09:55.000000 data_snack_dynamic_entity-0.3.0/src/data_snack_dynamic_entity/simple_entity/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-06-03 14:09:55.000000 data_snack_dynamic_entity-0.3.0/src/data_snack_dynamic_entity/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-06-03 14:09:55.000000 data_snack_dynamic_entity-0.3.0/src/data_snack_dynamic_entity/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:10:05.473272 data_snack_dynamic_entity-0.3.0/src/data_snack_dynamic_entity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-06-03 14:10:05.000000 data_snack_dynamic_entity-0.3.0/src/data_snack_dynamic_entity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-06-03 14:10:05.000000 data_snack_dynamic_entity-0.3.0/src/data_snack_dynamic_entity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 14:10:05.000000 data_snack_dynamic_entity-0.3.0/src/data_snack_dynamic_entity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-06-03 14:10:05.000000 data_snack_dynamic_entity-0.3.0/src/data_snack_dynamic_entity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-06-03 14:10:05.000000 data_snack_dynamic_entity-0.3.0/src/data_snack_dynamic_entity.egg-info/top_level.txt
```

### Comparing `data_snack_dynamic_entity-0.2.0/LICENSE` & `data_snack_dynamic_entity-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `data_snack_dynamic_entity-0.2.0/PKG-INFO` & `data_snack_dynamic_entity-0.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: data_snack_dynamic_entity
-Version: 0.2.0
+Version: 0.3.0
 Home-page: https://github.com/webinterpret-ds/data-snack-dynamic-entity
 Author: webinterpret-datascience
 Author-email: data-science@webinterpret.com
 Project-URL: Bug Tracker, https://github.com/webinterpret-ds/data-snack-dynamic-entity/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: data-snack>=1.0.3
+Requires-Dist: data-snack>=1.0.5
 Requires-Dist: jsonschema>=4.17.3
 
 # Data Snack - Dynamic entity 
 
 # About
 Used to dynamically load `data-snack` `Entity` objects from json schema.
 Especially useful for complex dataset with many fields.
```

### Comparing `data_snack_dynamic_entity-0.2.0/README.md` & `data_snack_dynamic_entity-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `data_snack_dynamic_entity-0.2.0/setup.cfg` & `data_snack_dynamic_entity-0.3.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = data-snack-dynamic-entity
-version = 0.2.0
+version = 0.3.0
 author = webinterpret-datascience
 author_email = data-science@webinterpret.com
 description = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/webinterpret-ds/data-snack-dynamic-entity
 project_urls =
```

### Comparing `data_snack_dynamic_entity-0.2.0/setup.py` & `data_snack_dynamic_entity-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `data_snack_dynamic_entity-0.2.0/src/data_snack_dynamic_entity/factory.py` & `data_snack_dynamic_entity-0.3.0/src/data_snack_dynamic_entity/simple_entity/factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 import builtins
+
 from data_snack.entities import Entity
 from dataclasses import dataclass, field, make_dataclass
 from typing import Dict, Type, Any, List, Optional
 
-from data_snack_dynamic_entity.types import EntitySchema, FieldSchema, EntityTemplates
+from data_snack_dynamic_entity.simple_entity.types import SimpleEntitySchema, SimpleEntityTemplates
 from data_snack_dynamic_entity.validate import validate_entity_templates
 
 
 @dataclass
-class EntityFactory:
+class SimpleEntityFactory:
     types_mapping: Dict[str, Any] = field(
         default_factory=dict
     )  # this will store custom mappings
 
-    def load_entities(self, templates: EntityTemplates) -> Dict[str, Type]:
+    def load_entities(self, templates: SimpleEntityTemplates) -> Dict[str, Type]:
         """
         Creates new Entity types based on provided config.
         Config should contain a valid template that is created according to the schema (see README).
 
         :param templates: input config containing templates
         :returns: a dictionary with all created Entity types
         """
 
         validate_entity_templates(templates)
         return {
-            entity_name: self._create_entity(entity_name, entity_schema)
+            entity_name: self._create_simple_entity(entity_name, entity_schema)
             for entity_name, entity_schema in templates.items()
         }
 
-    def _create_entity(self, entity_name: str, entity_schema: EntitySchema) -> Type:
+    def _create_simple_entity(self, entity_name: str, entity_schema: SimpleEntitySchema) -> Type:
         """
         Creates entity of given name according to given schema.
         :param entity_name: new entity name
         :param entity_schema: new entity schema
         :return: new entity type
         """
         fields = []
@@ -51,15 +52,15 @@
             if "default" in field_schema:
                 fields_with_defaults.append(
                     (field_name, field_type, field(default=field_schema["default"]))
                 )
             else:
                 fields.append((field_name, field_type))
 
-        entity_template = self._create_entity_template(
+        entity_template = self._create_simple_entity_template(
             entity_name=entity_name, keys=keys, excluded_fields=excluded_fields, version=entity_schema["version"]
         )
         return make_dataclass(
             entity_name,
             fields + fields_with_defaults,
             bases=(entity_template,),
             namespace={"__module__": __name__},
@@ -73,29 +74,21 @@
             return t
         except AttributeError as e:
             if t := self.types_mapping.get(name):
                 return t
             raise ValueError(name) from e
 
     @staticmethod
-    def _create_entity_template(
+    def _create_simple_entity_template(
         entity_name: str, keys: List[str], excluded_fields: List[str], version: int
     ) -> Type:
         return type(
             f"{entity_name}Template",
             (Entity,),
             {
                 "Meta": type(
                     "Meta",
                     (object,),
                     {"keys": keys, "excluded_fields": excluded_fields, "version": version},
                 )
             },
         )
-
-
-def load_entities(
-    templates: EntityTemplates, types_mapping: Dict[str, Any] = None
-) -> Dict[str, Type]:
-    if not types_mapping:
-        types_mapping = {}
-    return EntityFactory(types_mapping).load_entities(templates)
```

### Comparing `data_snack_dynamic_entity-0.2.0/src/data_snack_dynamic_entity/validate.py` & `data_snack_dynamic_entity-0.3.0/src/data_snack_dynamic_entity/validate.py`

 * *Files identical despite different names*

### Comparing `data_snack_dynamic_entity-0.2.0/src/data_snack_dynamic_entity.egg-info/PKG-INFO` & `data_snack_dynamic_entity-0.3.0/src/data_snack_dynamic_entity.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: data_snack_dynamic_entity
-Version: 0.2.0
+Version: 0.3.0
 Home-page: https://github.com/webinterpret-ds/data-snack-dynamic-entity
 Author: webinterpret-datascience
 Author-email: data-science@webinterpret.com
 Project-URL: Bug Tracker, https://github.com/webinterpret-ds/data-snack-dynamic-entity/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: data-snack>=1.0.3
+Requires-Dist: data-snack>=1.0.5
 Requires-Dist: jsonschema>=4.17.3
 
 # Data Snack - Dynamic entity 
 
 # About
 Used to dynamically load `data-snack` `Entity` objects from json schema.
 Especially useful for complex dataset with many fields.
```

