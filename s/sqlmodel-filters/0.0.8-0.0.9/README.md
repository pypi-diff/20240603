# Comparing `tmp/sqlmodel_filters-0.0.8.tar.gz` & `tmp/sqlmodel_filters-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlmodel_filters-0.0.8.tar", max compression
+gzip compressed data, was "sqlmodel_filters-0.0.9.tar", max compression
```

## Comparing `sqlmodel_filters-0.0.8.tar` & `sqlmodel_filters-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2024-05-07 10:42:02.201348 sqlmodel_filters-0.0.8/LICENSE
--rw-r--r--   0        0        0     8433 2024-05-07 10:42:02.201348 sqlmodel_filters-0.0.8/README.md
--rw-r--r--   0        0        0     1022 2024-05-07 10:42:15.889348 sqlmodel_filters-0.0.8/pyproject.toml
--rw-r--r--   0        0        0       82 2024-05-07 10:42:02.201348 sqlmodel_filters-0.0.8/sqlmodel_filters/__init__.py
--rw-r--r--   0        0        0     7919 2024-05-07 10:42:02.201348 sqlmodel_filters-0.0.8/sqlmodel_filters/builder.py
--rw-r--r--   0        0        0     7419 2024-05-07 10:42:02.201348 sqlmodel_filters-0.0.8/sqlmodel_filters/components.py
--rw-r--r--   0        0        0      165 2024-05-07 10:42:02.201348 sqlmodel_filters-0.0.8/sqlmodel_filters/exceptions.py
--rw-r--r--   0        0        0      391 2024-05-07 10:42:02.201348 sqlmodel_filters-0.0.8/sqlmodel_filters/utils.py
--rw-r--r--   0        0        0     9018 1970-01-01 00:00:00.000000 sqlmodel_filters-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-06-02 23:45:23.349605 sqlmodel_filters-0.0.9/LICENSE
+-rw-r--r--   0        0        0     8433 2024-06-02 23:45:23.349605 sqlmodel_filters-0.0.9/README.md
+-rw-r--r--   0        0        0     1021 2024-06-02 23:45:38.201546 sqlmodel_filters-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0       82 2024-06-02 23:45:23.349605 sqlmodel_filters-0.0.9/sqlmodel_filters/__init__.py
+-rw-r--r--   0        0        0     7801 2024-06-02 23:45:23.349605 sqlmodel_filters-0.0.9/sqlmodel_filters/builder.py
+-rw-r--r--   0        0        0     7419 2024-06-02 23:45:23.349605 sqlmodel_filters-0.0.9/sqlmodel_filters/components.py
+-rw-r--r--   0        0        0      165 2024-06-02 23:45:23.349605 sqlmodel_filters-0.0.9/sqlmodel_filters/exceptions.py
+-rw-r--r--   0        0        0      391 2024-06-02 23:45:23.349605 sqlmodel_filters-0.0.9/sqlmodel_filters/utils.py
+-rw-r--r--   0        0        0     9017 1970-01-01 00:00:00.000000 sqlmodel_filters-0.0.9/PKG-INFO
```

### Comparing `sqlmodel_filters-0.0.8/LICENSE` & `sqlmodel_filters-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlmodel_filters-0.0.8/README.md` & `sqlmodel_filters-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `sqlmodel_filters-0.0.8/pyproject.toml` & `sqlmodel_filters-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "sqlmodel-filters"
-version = "0.0.8"
-description = "A Lucene query like fliltering for SQLModel"
+version = "0.0.9"
+description = "A Lucene query like filtering for SQLModel"
 authors = ["Manabu Niseki <manabu.niseki@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 luqum = "^0.13"
```

### Comparing `sqlmodel_filters-0.0.8/sqlmodel_filters/builder.py` & `sqlmodel_filters-0.0.9/sqlmodel_filters/builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import contextlib
+import itertools
 from collections.abc import Callable
 from types import MappingProxyType
 from typing import Any, TypeVar
 
 from luqum.thread import parse
 from luqum.tree import (
     AndOperation,
@@ -88,43 +89,34 @@
         yield from super().generic_visit(node, context)
 
     def _handle_group(self, node: Group):
         # NOTE: group can be processed as And operation
         yield from self._handle_and_operation(node)  # type: ignore
 
     def _handle_and_operation(self, node: AndOperation):
-        expressions: list[_ColumnExpressionArgument] = []
-        for child in node.children:
-            expressions.extend(list(self.get_expressions(child)))
-
+        expressions = list(itertools.chain.from_iterable([self.get_expressions(child) for child in node.children]))
         if len(expressions) > 0:
             yield and_(*expressions)
 
     def visit_and_operation(self, node: AndOperation, context: dict):
         self.expressions.extend(list(self.get_expressions(node)))
         yield from super().generic_visit(node, context)
 
     def _handle_or_operation(self, node: OrOperation):
-        expressions: list[_ColumnExpressionArgument] = []
-        for child in node.children:
-            expressions.extend(list(self.get_expressions(child)))
-
+        expressions = list(itertools.chain.from_iterable([self.get_expressions(child) for child in node.children]))
         if len(expressions) > 0:
             first, *others = expressions
             yield or_(first, *others)
 
     def visit_or_operation(self, node: OrOperation, context: dict):
         self.expressions.extend(list(self.get_expressions(node)))
         yield from super().generic_visit(node, context)
 
     def _handle_not(self, node: Not):
-        expressions: list[_ColumnExpressionArgument] = []
-        for child in node.children:
-            expressions.extend(list(self.get_expressions(child)))
-
+        expressions = list(itertools.chain.from_iterable([self.get_expressions(child) for child in node.children]))
         if len(expressions) > 0:
             yield not_(*expressions)
 
     def visit_not(self, node: Not, context: dict):
         self.expressions.extend(list(self.get_expressions(node)))
         yield from super().generic_visit(node, context)
```

### Comparing `sqlmodel_filters-0.0.8/sqlmodel_filters/components.py` & `sqlmodel_filters-0.0.9/sqlmodel_filters/components.py`

 * *Files identical despite different names*

### Comparing `sqlmodel_filters-0.0.8/PKG-INFO` & `sqlmodel_filters-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sqlmodel-filters
-Version: 0.0.8
-Summary: A Lucene query like fliltering for SQLModel
+Version: 0.0.9
+Summary: A Lucene query like filtering for SQLModel
 License: MIT
 Author: Manabu Niseki
 Author-email: manabu.niseki@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

