# Comparing `tmp/fastapi_resources-0.5.0.tar.gz` & `tmp/fastapi_resources-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_resources-0.5.0.tar", max compression
+gzip compressed data, was "fastapi_resources-0.5.1.tar", max compression
```

## Comparing `fastapi_resources-0.5.0.tar` & `fastapi_resources-0.5.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0        0 2022-10-05 19:53:19.150339 fastapi_resources-0.5.0/fastapi_resources/__init__.py
--rw-r--r--   0        0        0       26 2023-11-09 18:16:44.991887 fastapi_resources-0.5.0/fastapi_resources/resources/__init__.py
--rw-r--r--   0        0        0     4979 2023-11-12 01:59:25.551967 fastapi_resources-0.5.0/fastapi_resources/resources/base_resource.py
--rw-r--r--   0        0        0       25 2023-11-09 18:16:44.992339 fastapi_resources-0.5.0/fastapi_resources/resources/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     8203 2023-11-12 01:23:46.162326 fastapi_resources-0.5.0/fastapi_resources/resources/sqlalchemy/base.py
--rw-r--r--   0        0        0       36 2023-11-09 18:16:44.992745 fastapi_resources-0.5.0/fastapi_resources/resources/sqlalchemy/exceptions.py
--rw-r--r--   0        0        0     7440 2024-02-29 19:45:06.485617 fastapi_resources-0.5.0/fastapi_resources/resources/sqlalchemy/mixins.py
--rw-r--r--   0        0        0      553 2023-11-09 18:16:44.993163 fastapi_resources-0.5.0/fastapi_resources/resources/sqlalchemy/paginators.py
--rw-r--r--   0        0        0      777 2023-11-09 18:16:44.993327 fastapi_resources-0.5.0/fastapi_resources/resources/sqlalchemy/resources.py
--rw-r--r--   0        0        0     2405 2023-11-09 18:16:44.993495 fastapi_resources-0.5.0/fastapi_resources/resources/sqlalchemy/types.py
--rw-r--r--   0        0        0     1881 2023-11-29 17:08:00.200960 fastapi_resources-0.5.0/fastapi_resources/resources/types.py
--rw-r--r--   0        0        0       91 2022-10-05 19:53:19.151384 fastapi_resources-0.5.0/fastapi_resources/routers/__init__.py
--rw-r--r--   0        0        0    13551 2024-05-19 23:19:50.957345 fastapi_resources-0.5.0/fastapi_resources/routers/base_router.py
--rw-r--r--   0        0        0      897 2024-05-19 23:15:26.291112 fastapi_resources-0.5.0/fastapi_resources/routers/decorators.py
--rw-r--r--   0        0        0       51 2022-10-12 22:33:19.044947 fastapi_resources-0.5.0/fastapi_resources/routers/json_api_router/__init__.py
--rw-r--r--   0        0        0    17118 2023-12-10 21:30:56.451631 fastapi_resources-0.5.0/fastapi_resources/routers/json_api_router/json_api_router.py
--rw-r--r--   0        0        0     2341 2023-11-23 17:39:00.279502 fastapi_resources-0.5.0/fastapi_resources/routers/json_api_router/types.py
--rw-r--r--   0        0        0        0 2022-10-05 19:53:19.152483 fastapi_resources-0.5.0/fastapi_resources/types.py
--rw-r--r--   0        0        0      630 2024-05-19 23:20:37.765483 fastapi_resources-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      378 1970-01-01 00:00:00.000000 fastapi_resources-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-10-05 19:53:19.150339 fastapi_resources-0.5.1/fastapi_resources/__init__.py
+-rw-r--r--   0        0        0       26 2023-11-09 18:16:44.991887 fastapi_resources-0.5.1/fastapi_resources/resources/__init__.py
+-rw-r--r--   0        0        0     5049 2024-06-03 03:40:20.778685 fastapi_resources-0.5.1/fastapi_resources/resources/base_resource.py
+-rw-r--r--   0        0        0       25 2023-11-09 18:16:44.992339 fastapi_resources-0.5.1/fastapi_resources/resources/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0    11809 2024-06-03 03:38:27.902203 fastapi_resources-0.5.1/fastapi_resources/resources/sqlalchemy/base.py
+-rw-r--r--   0        0        0       36 2023-11-09 18:16:44.992745 fastapi_resources-0.5.1/fastapi_resources/resources/sqlalchemy/exceptions.py
+-rw-r--r--   0        0        0     7428 2024-06-03 03:41:41.829718 fastapi_resources-0.5.1/fastapi_resources/resources/sqlalchemy/mixins.py
+-rw-r--r--   0        0        0      553 2023-11-09 18:16:44.993163 fastapi_resources-0.5.1/fastapi_resources/resources/sqlalchemy/paginators.py
+-rw-r--r--   0        0        0      777 2023-11-09 18:16:44.993327 fastapi_resources-0.5.1/fastapi_resources/resources/sqlalchemy/resources.py
+-rw-r--r--   0        0        0     2441 2024-06-03 03:10:17.529961 fastapi_resources-0.5.1/fastapi_resources/resources/sqlalchemy/types.py
+-rw-r--r--   0        0        0     1949 2024-06-03 03:40:02.642115 fastapi_resources-0.5.1/fastapi_resources/resources/types.py
+-rw-r--r--   0        0        0       91 2022-10-05 19:53:19.151384 fastapi_resources-0.5.1/fastapi_resources/routers/__init__.py
+-rw-r--r--   0        0        0    13545 2024-06-03 03:39:16.592745 fastapi_resources-0.5.1/fastapi_resources/routers/base_router.py
+-rw-r--r--   0        0        0      897 2024-05-19 23:15:26.291112 fastapi_resources-0.5.1/fastapi_resources/routers/decorators.py
+-rw-r--r--   0        0        0       51 2022-10-12 22:33:19.044947 fastapi_resources-0.5.1/fastapi_resources/routers/json_api_router/__init__.py
+-rw-r--r--   0        0        0    17112 2024-06-03 03:40:50.490941 fastapi_resources-0.5.1/fastapi_resources/routers/json_api_router/json_api_router.py
+-rw-r--r--   0        0        0     2341 2023-11-23 17:39:00.279502 fastapi_resources-0.5.1/fastapi_resources/routers/json_api_router/types.py
+-rw-r--r--   0        0        0        0 2022-10-05 19:53:19.152483 fastapi_resources-0.5.1/fastapi_resources/types.py
+-rw-r--r--   0        0        0      630 2024-06-03 03:42:54.842555 fastapi_resources-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      378 1970-01-01 00:00:00.000000 fastapi_resources-0.5.1/PKG-INFO
```

### Comparing `fastapi_resources-0.5.0/fastapi_resources/resources/base_resource.py` & `fastapi_resources-0.5.1/fastapi_resources/resources/base_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,20 +34,21 @@
         inclusions: Optional[Inclusions] = None,
         context: Optional[dict] = None,
         page: Optional[str] = None,
         limit: Optional[int] = None,
         *args,
         **kwargs,
     ):
-        if inclusions:
-            self.validate_inclusions(inclusions=inclusions)
-
         self.inclusions = inclusions or []
         self.context = context or {}
         self.tasks = []
+        self.relationships = self.get_relationships()
+
+        if inclusions:
+            self.validate_inclusions(inclusions=inclusions)
 
     def close(self):
         pass
 
     def _zipped_inclusions_with_resource(
         self, _relationships: Relationships, _inclusion: list[str]
     ) -> list[InclusionWithResource]:
@@ -63,17 +64,16 @@
         if relationship_info.schema_with_relationships.schema not in self.registry:
             raise Exception(
                 f"Resource not found for relationship {relationship_info.field}"
             )
 
         resource = self.registry[relationship_info.schema_with_relationships.schema]
 
-        zipped_inclusions = [
-            InclusionWithResource(field=current_inclusion, resource=resource)
-        ]
+        field = relationship_info.loaded_field or current_inclusion
+        zipped_inclusions = [InclusionWithResource(field=field, resource=resource)]
 
         if (
             next_relationships := relationship_info.schema_with_relationships.relationships
         ):
             zipped_inclusions = [
                 *zipped_inclusions,
                 *self._zipped_inclusions_with_resource(
@@ -82,26 +82,26 @@
                 ),
             ]
 
         return zipped_inclusions
 
     def validate_inclusions(self, inclusions: Inclusions):
         """Validate the inclusions by walking the relationships."""
-        relationships = self.get_relationships()
+        relationships = self.relationships
 
         for inclusion in inclusions:
             self._zipped_inclusions_with_resource(
                 _relationships=relationships, _inclusion=inclusion
             )
 
     def zipped_inclusions_with_resource(
         self, inclusion: list[str]
     ) -> list[InclusionWithResource]:
         return self._zipped_inclusions_with_resource(
-            _relationships=self.get_relationships(),
+            _relationships=self.relationships,
             _inclusion=inclusion,
         )
 
     @classmethod
     def get_relationships(cls) -> Relationships:
         return {}
 
@@ -150,9 +150,9 @@
                         )
                     ],
                 ]
 
             return selected_objs
 
         return select_objs(
-            _obj=obj, _inclusion=inclusion, _relationships=self.get_relationships()
+            _obj=obj, _inclusion=inclusion, _relationships=self.relationships
         )
```

### Comparing `fastapi_resources-0.5.0/fastapi_resources/resources/sqlalchemy/base.py` & `fastapi_resources-0.5.1/fastapi_resources/resources/sqlalchemy/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,80 +1,175 @@
 import copy
+from dataclasses import dataclass
 from typing import Any, ClassVar, Generic, Optional, Type
 
 from sqlalchemy import exc as sa_exceptions
 from sqlalchemy import func, inspect, select
-from sqlalchemy.orm import MANYTOONE, DeclarativeBase, Session, joinedload
+from sqlalchemy.ext.associationproxy import (
+    AssociationProxy,
+    AssociationProxyExtensionType,
+)
+from sqlalchemy.orm import (
+    MANYTOONE,
+    DeclarativeBase,
+    Mapper,
+    RelationshipDirection,
+    Session,
+    joinedload,
+)
 
 from fastapi_resources.resources import base_resource
 from fastapi_resources.resources.sqlalchemy.exceptions import NotFound
 
 from . import types
 
 
+@dataclass
+class SAInstrumentedRelationship:
+    direction: RelationshipDirection
+    update_field: str
+    many: bool
+    related_schema: Type[DeclarativeBase]
+    loaded_field: str | None = None
+
+
+def get_instrumented_relationships_from_schema(inspected: Mapper[DeclarativeBase]):
+    return {
+        field: SAInstrumentedRelationship(
+            related_schema=relationship.mapper.class_,
+            many=relationship.uselist or False,
+            direction=relationship.direction,
+            update_field=list(
+                relationship.local_columns
+                if relationship.direction == MANYTOONE
+                else relationship.remote_side
+            )[0].name,
+        )
+        for field, relationship in inspected.relationships.items()
+    }
+
+
+def get_instrumented_relationships_from_schema_association_proxies(
+    inspected: Mapper[DeclarativeBase],
+):
+    proxies: list[tuple[str, AssociationProxy]] = [
+        (field, desc)
+        for field, desc in inspected.all_orm_descriptors.items()
+        if desc.extension_type is AssociationProxyExtensionType.ASSOCIATION_PROXY
+    ]  # type: ignore
+
+    sa_relationships: dict[str, SAInstrumentedRelationship] = {}
+
+    for field, proxy in proxies:
+        # This is the field on the model that the proxy proxies to
+        target_collection = proxy.target_collection
+        # This is the attribute on the target collection that gets pulled
+        value_attr = proxy.value_attr
+
+        # It can be any field type, but we only care about proxies to relationships
+        target_collection_relationship = inspected.relationships.get(target_collection)
+        if not target_collection_relationship:
+            continue
+
+        # The schema of the association table
+        association_schema: type[
+            DeclarativeBase
+        ] = target_collection_relationship.mapper.class_
+        association_inspected = inspect(association_schema)
+        # The relationship on the association that we're extracting
+        target_relationship = association_inspected.relationships[value_attr]
+
+        sa_relationships[field] = SAInstrumentedRelationship(
+            related_schema=target_relationship.mapper.class_,
+            # We want to use the `many` based on the field we're proxing to
+            many=target_collection_relationship.uselist or False,
+            # Same with the direction
+            direction=target_collection_relationship.direction,
+            # The update_field isn't supported for associations, at least right now
+            update_field="",
+            # We can't load from the association proxy, instead we load from the
+            # field the proxy uses
+            loaded_field=target_collection,
+        )
+
+    return sa_relationships
+
+
 def get_relationships_from_schema(
     schema: Type[DeclarativeBase],
     schema_cache: Optional[
         dict[
             tuple[Optional[str], Type[DeclarativeBase]],
             types.SchemaWithRelationships,
         ]
     ] = None,
     immediate_parent_backpopulated_field: Optional[str] = None,
     parent_key: Optional[str] = None,
 ):
     schema_cache = schema_cache or {}
-
     relationships = {}
-
     parent_schema_with_relationships = types.SchemaWithRelationships(
         schema=schema,
         relationships=relationships,
     )
+    inspected = inspect(schema)
 
     # Just a sanity check. This function should never be called for a relationship
     # that already exists.
     assert (parent_key, schema) not in schema_cache
-
     schema_cache[(parent_key, schema)] = parent_schema_with_relationships
 
-    for field, sqlalchemy_relationship in inspect(schema).relationships.items():
-        related_schema = sqlalchemy_relationship.mapper.class_
-        many = sqlalchemy_relationship.uselist
+    # Get relationships from actual relationships()
+    sa_relationships = get_instrumented_relationships_from_schema(inspected=inspected)
+    # Get relationships via AssociationProxies
+    sa_relationships.update(
+        get_instrumented_relationships_from_schema_association_proxies(
+            inspected=inspected
+        )
+    )
+
+    # Build SQLAlchemyRelationshipInfo objects from the instrumented relationships
+    for field, sqlalchemy_relationship in sa_relationships.items():
+        related_schema = sqlalchemy_relationship.related_schema
+        many = sqlalchemy_relationship.many
 
         # Used to uniquely identify the related schema relative to a parent
         new_parent_key = f"{schema}.{field}"
 
         # TODO: Handle MANYTOMANY
         direction = sqlalchemy_relationship.direction
-        update_field = list(
-            sqlalchemy_relationship.local_columns
-            if direction == MANYTOONE
-            else sqlalchemy_relationship.remote_side
-        )[0].name
+        update_field = sqlalchemy_relationship.update_field
 
         # If this branch already contains the schema with the same parent,
         # we can reuse the relationship to avoid a cycle.
         if relationship_info := schema_cache.get((new_parent_key, related_schema)):
             relationships[field] = types.SQLAlchemyRelationshipInfo(
                 schema_with_relationships=relationship_info,
                 many=many,
                 field=field,
                 direction=direction,
                 update_field=update_field,
+                loaded_field=sqlalchemy_relationship.loaded_field,
             )
             continue
 
         # For any relationship, the child will have a backpopulated reference
         # to the parent; we want to exclude that from available relationships
         if field == immediate_parent_backpopulated_field:
             continue
 
         # TODO: Can we cache the relationships when added to the registry?
-        backpopulated_field = inspect(schema).relationships[field].back_populates
+        # NOTE: If there's no relationship on the schema, that means this is a
+        # simulated relationship via an AssociationProxy. Those don't have
+        # backpopulated fields, so we can safely set this to "".
+        backpopulated_field = (
+            inspected.relationships[field].back_populates
+            if field in inspected.relationships
+            else ""
+        )
 
         get_relationships_from_schema(
             schema=related_schema,
             schema_cache=schema_cache,
             immediate_parent_backpopulated_field=backpopulated_field,
             parent_key=new_parent_key,
         )
@@ -89,14 +184,15 @@
 
         relationships[field] = types.SQLAlchemyRelationshipInfo(
             schema_with_relationships=schema_with_relationship,
             many=many,
             field=field,
             direction=direction,
             update_field=update_field,
+            loaded_field=sqlalchemy_relationship.loaded_field,
         )
 
     return relationships
 
 
 class BaseSQLAlchemyResource(
     base_resource.Resource[types.TDb],
@@ -127,16 +223,14 @@
     ):
         if session:
             self.session = session
         else:
             assert self.engine, "A session or an engine must be given."
             self.session = Session(self.engine)
 
-        # TODO: Save the relationships on the instance at instantiation for caching
-
         if Paginator := getattr(self, "Paginator", None):
             self.paginator = Paginator(cursor=cursor, limit=limit)
 
         super().__init__(inclusions=inclusions, *args, **kwargs)
 
     def close(self):
         self.session.close()
```

### Comparing `fastapi_resources-0.5.0/fastapi_resources/resources/sqlalchemy/mixins.py` & `fastapi_resources-0.5.1/fastapi_resources/resources/sqlalchemy/mixins.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         self: types.SQLAlchemyResourceProtocol[types.TDb],
         attributes: dict,
         relationships: Optional[dict[str, str | int | list[str | int]]] = None,
         **kwargs,
     ):
         create_kwargs = attributes | kwargs
         relationships = relationships or {}
-        model_relationships = self.get_relationships()
+        model_relationships = self.relationships
         did_set_relationship = False
 
         for field, related_ids in relationships.items():
             relationship = model_relationships[field]
             direction = relationship.direction
 
             RelatedResource = self.registry[
@@ -101,15 +101,15 @@
         **kwargs,
     ):
         row = self.get_object(id=id)
 
         for key, value in list(attributes.items()) + list(kwargs.items()):
             setattr(row, key, value)
 
-        model_relationships = self.get_relationships()
+        model_relationships = self.relationships
 
         if relationships:
             for field, related_ids in relationships.items():
                 relationship = model_relationships[field]
                 direction = relationship.direction
 
                 RelatedResource = self.registry[
```

### Comparing `fastapi_resources-0.5.0/fastapi_resources/resources/sqlalchemy/paginators.py` & `fastapi_resources-0.5.1/fastapi_resources/resources/sqlalchemy/paginators.py`

 * *Files identical despite different names*

### Comparing `fastapi_resources-0.5.0/fastapi_resources/resources/sqlalchemy/resources.py` & `fastapi_resources-0.5.1/fastapi_resources/resources/sqlalchemy/resources.py`

 * *Files identical despite different names*

### Comparing `fastapi_resources-0.5.0/fastapi_resources/resources/sqlalchemy/types.py` & `fastapi_resources-0.5.1/fastapi_resources/resources/sqlalchemy/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 @dataclass
 class SQLAlchemyRelationshipInfo:
     schema_with_relationships: SchemaWithRelationships
     many: bool
     field: str
     direction: RelationshipDirection
     update_field: str
+    loaded_field: str | None = None
 
 
 Relationships = dict[str, SQLAlchemyRelationshipInfo]
 
 
 TDb = TypeVar("TDb", bound=DeclarativeBase)
```

### Comparing `fastapi_resources-0.5.0/fastapi_resources/resources/types.py` & `fastapi_resources-0.5.1/fastapi_resources/resources/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from dataclasses import dataclass
 from typing import (
     Callable,
     ClassVar,
     Generic,
     List,
+    Mapping,
     Optional,
     Protocol,
     Set,
     Type,
     TypeVar,
 )
 
@@ -27,14 +28,15 @@
 
 
 @dataclass
 class RelationshipInfo:
     schema_with_relationships: SchemaWithRelationships
     many: bool
     field: str
+    loaded_field: str | None = None
 
 
 Relationships = dict[str, RelationshipInfo]
 
 
 @dataclass
 class SelectedObj:
@@ -58,22 +60,23 @@
     delete: ClassVar[Optional[Callable]] = None
     delete_all: ClassVar[Optional[Callable]] = None
     retrieve: ClassVar[Optional[Callable]] = None
 
     inclusions: Inclusions
     context: dict = {}
     tasks: List = []
+    relationships: Relationships
 
     def __init__(*args, **kwargs):
         pass
 
     @classmethod
     def get_relationships(
         cls,
-    ) -> dict[str, RelationshipInfo]:
+    ) -> Relationships:
         ...
 
     @classmethod
     def get_attributes(cls) -> Set[str]:
         """Get the non-relationships attributes for the resource.
 
         The attributes that end up in the response depend on those specified in
```

### Comparing `fastapi_resources-0.5.0/fastapi_resources/routers/base_router.py` & `fastapi_resources-0.5.1/fastapi_resources/routers/base_router.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,15 +238,15 @@
         return rows
 
     def parse_update(
         self,
         resource: TResource,
         update: dict,
     ):
-        resource_relationships = resource.get_relationships()
+        resource_relationships = resource.relationships
 
         relationships = {}
 
         for field in list(update.keys()):
             value = update[field]
             if field in resource_relationships:
                 relationships[field] = value
```

### Comparing `fastapi_resources-0.5.0/fastapi_resources/routers/decorators.py` & `fastapi_resources-0.5.1/fastapi_resources/routers/decorators.py`

 * *Files identical despite different names*

### Comparing `fastapi_resources-0.5.0/fastapi_resources/routers/json_api_router/json_api_router.py` & `fastapi_resources-0.5.1/fastapi_resources/routers/json_api_router/json_api_router.py`

 * *Files 0% similar despite different names*

```diff
@@ -337,15 +337,15 @@
         self, obj: types.Object, resource: TResource
     ):
         relationships = {}
 
         for (
             relationship_name,
             relationship_info,
-        ) in resource.get_relationships().items():
+        ) in resource.relationships.items():
             # The relationships will have been properly selected, so this should not send
             # another query.
             data = [
                 self.build_resource_identifier_object(
                     related_obj=related_obj.obj,
                     resource=resource,
                     relationship_info=relationship_info,
```

### Comparing `fastapi_resources-0.5.0/fastapi_resources/routers/json_api_router/types.py` & `fastapi_resources-0.5.1/fastapi_resources/routers/json_api_router/types.py`

 * *Files identical despite different names*

### Comparing `fastapi_resources-0.5.0/pyproject.toml` & `fastapi_resources-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-resources"
-version = "0.5.0"
+version = "0.5.1"
 description = ""
 authors = ["Ben Davis <ben@bencdavis.com>"]
 packages = [
     { include = "fastapi_resources" }
 ]
 
 [tool.poetry.dependencies]
```

