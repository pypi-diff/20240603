# Comparing `tmp/django_lookup_property-0.1.5.tar.gz` & `tmp/django_lookup_property-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_lookup_property-0.1.5.tar", max compression
+gzip compressed data, was "django_lookup_property-0.1.6.tar", max compression
```

## Comparing `django_lookup_property-0.1.5.tar` & `django_lookup_property-0.1.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1064 2024-05-24 10:22:11.982308 django_lookup_property-0.1.5/LICENSE
--rw-r--r--   0        0        0     2745 2024-05-24 10:22:11.982308 django_lookup_property-0.1.5/README.md
--rw-r--r--   0        0        0      305 2024-05-24 10:22:11.982308 django_lookup_property-0.1.5/lookup_property/__init__.py
--rw-r--r--   0        0        0      689 2024-05-24 10:22:11.982308 django_lookup_property-0.1.5/lookup_property/converters/__init__.py
--rw-r--r--   0        0        0     2383 2024-05-24 10:22:11.982308 django_lookup_property-0.1.5/lookup_property/converters/aggregates.py
--rw-r--r--   0        0        0     4255 2024-05-24 10:22:11.982308 django_lookup_property-0.1.5/lookup_property/converters/cast.py
--rw-r--r--   0        0        0     1915 2024-05-24 10:22:11.982308 django_lookup_property-0.1.5/lookup_property/converters/conditions.py
--rw-r--r--   0        0        0    10299 2024-05-24 10:22:11.982308 django_lookup_property-0.1.5/lookup_property/converters/datetime.py
--rw-r--r--   0        0        0     3382 2024-05-24 10:22:11.982308 django_lookup_property-0.1.5/lookup_property/converters/expressions.py
--rw-r--r--   0        0        0     4311 2024-05-24 10:22:11.982308 django_lookup_property-0.1.5/lookup_property/converters/functions.py
--rw-r--r--   0        0        0    11293 2024-05-24 10:22:11.982308 django_lookup_property-0.1.5/lookup_property/converters/lookups.py
--rw-r--r--   0        0        0     2361 2024-05-24 10:22:11.982308 django_lookup_property-0.1.5/lookup_property/converters/main.py
--rw-r--r--   0        0        0     6043 2024-05-24 10:22:11.986309 django_lookup_property-0.1.5/lookup_property/converters/math.py
--rw-r--r--   0        0        0      433 2024-05-24 10:22:11.986309 django_lookup_property-0.1.5/lookup_property/converters/number.py
--rw-r--r--   0        0        0     9155 2024-05-24 10:22:11.986309 django_lookup_property-0.1.5/lookup_property/converters/string.py
--rw-r--r--   0        0        0     2081 2024-05-24 10:22:11.986309 django_lookup_property-0.1.5/lookup_property/converters/utils.py
--rw-r--r--   0        0        0     4052 2024-05-24 10:22:11.986309 django_lookup_property-0.1.5/lookup_property/decorator.py
--rw-r--r--   0        0        0     1284 2024-05-24 10:22:11.986309 django_lookup_property-0.1.5/lookup_property/dispatch.py
--rw-r--r--   0        0        0    14501 2024-05-24 10:22:11.986309 django_lookup_property-0.1.5/lookup_property/expressions.py
--rw-r--r--   0        0        0     3438 2024-05-24 10:22:11.986309 django_lookup_property-0.1.5/lookup_property/field.py
--rw-r--r--   0        0        0        0 2024-05-24 10:22:11.986309 django_lookup_property-0.1.5/lookup_property/py.typed
--rw-r--r--   0        0        0     2155 2024-05-24 10:22:11.986309 django_lookup_property-0.1.5/lookup_property/typing.py
--rw-r--r--   0        0        0     5480 2024-05-24 10:22:11.986309 django_lookup_property-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3887 1970-01-01 00:00:00.000000 django_lookup_property-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-06-03 07:58:49.062945 django_lookup_property-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2745 2024-06-03 07:58:49.062945 django_lookup_property-0.1.6/README.md
+-rw-r--r--   0        0        0      305 2024-06-03 07:58:49.062945 django_lookup_property-0.1.6/lookup_property/__init__.py
+-rw-r--r--   0        0        0      689 2024-06-03 07:58:49.062945 django_lookup_property-0.1.6/lookup_property/converters/__init__.py
+-rw-r--r--   0        0        0     2434 2024-06-03 07:58:49.062945 django_lookup_property-0.1.6/lookup_property/converters/aggregates.py
+-rw-r--r--   0        0        0     4306 2024-06-03 07:58:49.062945 django_lookup_property-0.1.6/lookup_property/converters/cast.py
+-rw-r--r--   0        0        0     1966 2024-06-03 07:58:49.062945 django_lookup_property-0.1.6/lookup_property/converters/conditions.py
+-rw-r--r--   0        0        0    10350 2024-06-03 07:58:49.062945 django_lookup_property-0.1.6/lookup_property/converters/datetime.py
+-rw-r--r--   0        0        0     3441 2024-06-03 07:58:49.062945 django_lookup_property-0.1.6/lookup_property/converters/expressions.py
+-rw-r--r--   0        0        0     4332 2024-06-03 07:58:49.062945 django_lookup_property-0.1.6/lookup_property/converters/functions.py
+-rw-r--r--   0        0        0    11372 2024-06-03 07:58:49.062945 django_lookup_property-0.1.6/lookup_property/converters/lookups.py
+-rw-r--r--   0        0        0     2304 2024-06-03 07:58:49.062945 django_lookup_property-0.1.6/lookup_property/converters/main.py
+-rw-r--r--   0        0        0     6064 2024-06-03 07:58:49.062945 django_lookup_property-0.1.6/lookup_property/converters/math.py
+-rw-r--r--   0        0        0      448 2024-06-03 07:58:49.062945 django_lookup_property-0.1.6/lookup_property/converters/number.py
+-rw-r--r--   0        0        0     9206 2024-06-03 07:58:49.062945 django_lookup_property-0.1.6/lookup_property/converters/string.py
+-rw-r--r--   0        0        0     2131 2024-06-03 07:58:49.062945 django_lookup_property-0.1.6/lookup_property/converters/utils.py
+-rw-r--r--   0        0        0     4044 2024-06-03 07:58:49.062945 django_lookup_property-0.1.6/lookup_property/decorator.py
+-rw-r--r--   0        0        0     1320 2024-06-03 07:58:49.062945 django_lookup_property-0.1.6/lookup_property/dispatch.py
+-rw-r--r--   0        0        0    14535 2024-06-03 07:58:49.062945 django_lookup_property-0.1.6/lookup_property/expressions.py
+-rw-r--r--   0        0        0     3406 2024-06-03 07:58:49.062945 django_lookup_property-0.1.6/lookup_property/field.py
+-rw-r--r--   0        0        0        0 2024-06-03 07:58:49.062945 django_lookup_property-0.1.6/lookup_property/py.typed
+-rw-r--r--   0        0        0     2152 2024-06-03 07:58:49.062945 django_lookup_property-0.1.6/lookup_property/typing.py
+-rw-r--r--   0        0        0     8593 2024-06-03 07:58:49.062945 django_lookup_property-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3967 1970-01-01 00:00:00.000000 django_lookup_property-0.1.6/PKG-INFO
```

### Comparing `django_lookup_property-0.1.5/LICENSE` & `django_lookup_property-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.5/README.md` & `django_lookup_property-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.5/lookup_property/converters/__init__.py` & `django_lookup_property-0.1.6/lookup_property/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.5/lookup_property/converters/aggregates.py` & `django_lookup_property-0.1.6/lookup_property/converters/aggregates.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+from __future__ import annotations
+
 import ast
 
 from django.db.models import aggregates
 
-from ..typing import State
+from lookup_property.typing import State
+
 from .expressions import expression_to_ast
 from .utils import ast_function, ast_method
 
 
 @expression_to_ast.register
 def _(
     expression: (
```

### Comparing `django_lookup_property-0.1.5/lookup_property/converters/cast.py` & `django_lookup_property-0.1.6/lookup_property/converters/cast.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+from __future__ import annotations
+
 import ast
 from functools import singledispatch
 
 from django.db import models
 from django.db.models import functions
 
-from ..typing import Expr, State
+from lookup_property.typing import Expr, State
+
 from .expressions import expression_to_ast
 
 __all__ = [
     "convert_django_field",
 ]
```

### Comparing `django_lookup_property-0.1.5/lookup_property/converters/conditions.py` & `django_lookup_property-0.1.6/lookup_property/converters/conditions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+from __future__ import annotations
+
 import ast
 
 from django.db import models
 from django.db.models import functions
 
-from ..typing import Expr, State
+from lookup_property.typing import Expr, State
+
 from .expressions import expression_to_ast
 
 
 @expression_to_ast.register
 def _(expression: models.Case, state: State) -> ast.IfExp:
     """
     Case(When(condition=Q(fizz=True), then=Value("foo")), default=Value("bar")))
```

### Comparing `django_lookup_property-0.1.5/lookup_property/converters/datetime.py` & `django_lookup_property-0.1.6/lookup_property/converters/datetime.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+from __future__ import annotations
+
 import ast
 
 from django.db.models import functions
 from django.db.models.functions.datetime import TruncBase
 
-from ..typing import State
+from lookup_property.typing import State
+
 from .expressions import expression_to_ast
 from .utils import ast_attribute, ast_function
 
 _LOOKUP_NAME_TO_TRUNC: dict[str, type[TruncBase]] = {
     "year": functions.TruncYear,
     "quarter": functions.TruncQuarter,
     "month": functions.TruncMonth,
```

### Comparing `django_lookup_property-0.1.5/lookup_property/converters/expressions.py` & `django_lookup_property-0.1.6/lookup_property/converters/expressions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+from __future__ import annotations
+
 import ast
 from functools import singledispatch
 
 from django.db import models
 from django.db.models.constants import LOOKUP_SEP
 from django.db.models.expressions import Combinable, CombinedExpression
 
-from ..typing import State
+from lookup_property.typing import State
+
 from .utils import ast_function, ast_property
 
 __all__ = [
     "expression_to_ast",
 ]
 
 
@@ -27,15 +30,15 @@
         return self.foo == random_string()
     """
     arg = state.extra_kwargs.add(lambda: expression)
     return ast_function(arg)
 
 
 @expression_to_ast.register
-def _(expression: None | str | int | float | bool | bytes, state: State) -> ast.Constant:  # noqa: PYI041
+def _(expression: None | str | int | float | bool | bytes, state: State) -> ast.Constant:  # noqa: PYI041, FBT001
     """Convert builtin values to constants"""
     return ast.Constant(value=expression)
 
 
 @expression_to_ast.register
 def _(expression: list, state: State) -> ast.List:
     """Convert to lists: [..., ..., ...]"""
```

### Comparing `django_lookup_property-0.1.5/lookup_property/converters/functions.py` & `django_lookup_property-0.1.6/lookup_property/converters/functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+from __future__ import annotations
+
 import ast
 
 from django.db.models import functions
-from django.db.models.functions import MD5, SHA1, SHA224, SHA256, SHA384, SHA512  # type: ignore[attr-defined]
+from django.db.models.functions import MD5, SHA1, SHA224, SHA256, SHA384, SHA512
+
+from lookup_property.typing import Expr, State
 
-from ..typing import Expr, State
 from .expressions import expression_to_ast
 
 
 @expression_to_ast.register
 def _(expression: MD5 | SHA1 | SHA224 | SHA256 | SHA384 | SHA512, state: State) -> ast.Call:
     """
     MD5("foo") -> hashlib.md5(self.foo.encode()).hexdigest()
```

### Comparing `django_lookup_property-0.1.5/lookup_property/converters/lookups.py` & `django_lookup_property-0.1.6/lookup_property/converters/lookups.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+from __future__ import annotations
+
 import ast
 from typing import Any
 
 from django.db import models
 from django.db.models import lookups
 from django.db.models.constants import LOOKUP_SEP
 
-from ..dispatch import lookup_singledispatch
-from ..expressions import L
-from ..typing import State
+from lookup_property.dispatch import lookup_singledispatch
+from lookup_property.expressions import L
+from lookup_property.typing import State
+
 from .expressions import expression_to_ast
 from .utils import ast_method, ast_property
 
 __all__ = [
     "lookup_to_ast",
 ]
```

### Comparing `django_lookup_property-0.1.5/lookup_property/converters/main.py` & `django_lookup_property-0.1.6/lookup_property/converters/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 from __future__ import annotations
 
 import ast
 import itertools
 from functools import partial, wraps
-from typing import TYPE_CHECKING
 
 from lookup_property import expression_to_ast
-
-if TYPE_CHECKING:
-    from lookup_property.typing import Expr, ModelMethod, State
-
+from lookup_property.typing import Expr, ModelMethod, State
 
 __all__ = [
     "ast_module_to_function",
     "ast_to_module",
     "query_expression_ast_module",
 ]
```

### Comparing `django_lookup_property-0.1.5/lookup_property/converters/math.py` & `django_lookup_property-0.1.6/lookup_property/converters/math.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+from __future__ import annotations
+
 import ast
 
 from django.db.models import functions
-from django.db.models.functions.math import Random  # type: ignore[attr-defined]
+from django.db.models.functions.math import Random
+
+from lookup_property.typing import Expr, State
 
-from ..typing import Expr, State
 from .expressions import expression_to_ast
 
 
 @expression_to_ast.register
 def _(expression: functions.Abs, state: State) -> ast.Call:
     """Abs("foo") -> abs(self.foo)"""
     return ast.Call(
```

### Comparing `django_lookup_property-0.1.5/lookup_property/converters/string.py` & `django_lookup_property-0.1.6/lookup_property/converters/string.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+from __future__ import annotations
+
 import ast
 
 from django.db.models import functions
 
-from ..typing import Expr, State
+from lookup_property.typing import Expr, State
+
 from .expressions import expression_to_ast
 
 
 @expression_to_ast.register
 def _(expression: functions.Concat, state: State) -> ast.AST:
     """
     Used together with the ConcatPair-converter below to concatenate values in pairs:
```

### Comparing `django_lookup_property-0.1.5/lookup_property/converters/utils.py` & `django_lookup_property-0.1.6/lookup_property/converters/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from __future__ import annotations
+
 import ast
 
-from ..typing import Iterable
+from lookup_property.typing import Iterable
 
 __all__ = [
     "ast_attribute",
     "ast_function",
     "ast_method",
     "ast_property",
 ]
```

### Comparing `django_lookup_property-0.1.5/lookup_property/decorator.py` & `django_lookup_property-0.1.6/lookup_property/decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         self.func = func
         self.module = ast.parse(inspect.cleandoc(inspect.getsource(func)))
 
     def contribute_to_class(
         self,
         cls: type[models.Model],
         name: str,
-        private_only: bool = False,  # noqa: FBT001, FBT002, ARG002
+        private_only: bool = False,  # noqa: FBT001, FBT002
     ) -> None:
         # Called by `django.db.models.base.ModelBase.add_to_class`
         field = LookupPropertyField(cls, target_property=self)
         field.set_attributes_from_name(name)
         field.name = field.attname = f"_{name}"  # Enable using aliases with the same name as the field
         field.concrete = self.state.concrete  # if False -> Don't include field in `SELECT` statements
         cls._meta.add_field(field, private=True)
```

### Comparing `django_lookup_property-0.1.5/lookup_property/dispatch.py` & `django_lookup_property-0.1.6/lookup_property/dispatch.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from functools import wraps
 
 from .typing import Callable, Concatenate, ParamSpec, Protocol, TypeVar, cast
 
 __all__ = [
     "lookup_singledispatch",
 ]
```

### Comparing `django_lookup_property-0.1.5/lookup_property/expressions.py` & `django_lookup_property-0.1.6/lookup_property/expressions.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     from django.db.models.sql.datastructures import Join
     from django.db.models.sql.where import WhereNode
 
     from .field import LookupPropertyField
     from .typing import Any, Callable, ConvertFunc, Expr, ExpressionKind
 
 __all__ = [
-    "LookupPropertyCol",
     "L",
+    "LookupPropertyCol",
 ]
 
 
 class LookupPropertyCol(models.Expression):
     def __init__(self, target_field: LookupPropertyField) -> None:
         self.target = target_field
         super().__init__()
@@ -193,30 +193,31 @@
     def asc(self, **kwargs: Any) -> models.OrderBy:
         return self.order_by(**kwargs)
 
     def desc(self, **kwargs: Any) -> models.OrderBy:
         kwargs["descending"] = True
         return self.order_by(**kwargs)
 
-    def resolve_expression(  # noqa: PLR0913
+    def resolve_expression(
         self,
         query: Query,
         allow_joins: bool,  # noqa: FBT001
         reuse: Any = None,
         summarize: bool = False,  # noqa: FBT001, FBT002
-        for_save: bool = False,  # noqa: ARG002, FBT001, FBT002
+        for_save: bool = False,  # noqa: FBT001, FBT002
     ) -> ExpressionKind:
         """Resolve lookup expression and either return it or build a lookup expression based on it."""
         field, lookup_parts, joined_tables = self.find_lookup_property_field(query)
         lookup_name = field.attname.removeprefix("_")
         expression = field.expression
         for table_name in reversed(joined_tables):
             expression = extend_expression_to_joined_table(expression, table_name)
 
-        query.add_annotation(expression, lookup_name, select=False)
+        if query.annotations.get(lookup_name) is None:
+            query.add_annotation(expression, lookup_name, select=False)
         expression = query.annotations[lookup_name]
 
         # Check whether the query should be grouped by the lookup expression.
         if expression.contains_aggregate:
             query.group_by = True
 
         # For sub-queries, save the resolved expression in place of the OuterRef.
```

### Comparing `django_lookup_property-0.1.5/lookup_property/field.py` & `django_lookup_property-0.1.6/lookup_property/field.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 
     @property
     def expression(self) -> Expr:
         return self.target_property.expression
 
     def get_col(  # type: ignore[override]
         self,
-        alias: str,  # noqa: ARG002
-        output_field: models.Field | None = None,  # noqa: ARG002
+        alias: str,
+        output_field: models.Field | None = None,
     ) -> LookupPropertyCol:
         return self.cached_col
 
     @cached_property
     def cached_col(self) -> LookupPropertyCol:  # type: ignore[override]
         return LookupPropertyCol(target_field=self)
```

### Comparing `django_lookup_property-0.1.5/lookup_property/typing.py` & `django_lookup_property-0.1.6/lookup_property/typing.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 
 if TYPE_CHECKING:
     from django.db.models.sql import Query
 
 __all__ = [
     "Any",
     "Callable",
-    "cast",
     "Collection",
     "Concatenate",
     "ConvertFunc",
     "Expr",
     "FunctionType",
     "Generator",
     "Iterable",
@@ -43,23 +42,24 @@
     "ModelMethod",
     "ParamSpec",
     "Protocol",
     "Self",
     "State",
     "TModel",
     "TypeVar",
+    "cast",
 ]
 
 
 TModel = TypeVar("TModel", bound=models.Model)
 Expr = BaseExpression | Combinable | models.Q
 
 
 class ExpressionKind(Protocol):
-    def resolve_expression(  # noqa: PLR0913
+    def resolve_expression(
         self,
         query: Query,
         allow_joins: bool,  # noqa: FBT001
         reuse: set[str] | None,
         summarize: bool,  # noqa: FBT001
         for_save: bool,  # noqa: FBT001
     ) -> ExpressionKind: ...
@@ -68,15 +68,15 @@
 ModelMethod = Callable[[TModel], Expr] | Callable[[], Expr]
 ConvertFunc = Callable[[Any, BaseExpression, BaseDatabaseWrapper], Any]
 
 Sentinel = object()
 
 
 def random_arg_name() -> str:
-    return "".join(random.choices(string.ascii_lowercase, k=20))
+    return "".join(random.choices(string.ascii_lowercase, k=20))  # noqa: S311
 
 
 class RandomKeyDict(dict[str, Any]):
     """Custom dict for adding items with random keys."""
 
     def add(self, item: Any) -> str:
         """Add an item to the dict with a random key. Return the key."""
```

### Comparing `django_lookup_property-0.1.5/pyproject.toml` & `django_lookup_property-0.1.6/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "django-lookup-property"
-version = "0.1.5"
+version = "0.1.6"
 description = "Django model properties that are also lookup expressions."
 authors = [
     "Matti Lamppu <lamppu.matti.akseli@gmail.com>",
 ]
 packages = [
     { include = "lookup_property" },
 ]
 license = "MIT"
 readme = "README.md"
 homepage = "https://mrthearman.github.io/django-lookup-property"
 repository = "https://github.com/MrThearMan/django-lookup-property"
+documentation = "https://mrthearman.github.io/django-lookup-property"
 keywords = [
     "django",
     "lookup",
     "property",
     "orm",
     "model",
     "extension",
@@ -46,107 +47,211 @@
 
 [tool.poetry.dependencies]
 python = ">=3.11,<4"
 Django = ">=4.2"
 
 [tool.poetry.group.test.dependencies]
 pytest = "8.2.1"
-coverage = "7.5.1"
+coverage = "7.5.3"
 pytest-django = "4.8.0"
-freezegun = "^1.2.2"
+freezegun = "1.5.1"
 pre-commit = "3.7.1"
 tox = "4.15.0"
 tox-gh-actions = "3.2.0"
-factory-boy = "^3.3.0"
-django-shared-property = "^0.8.0"
+factory-boy = "3.3.0"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "1.6.0"
 pymdown-extensions = "10.8.1"
 mkdocs-mermaid2-plugin = "1.1.1"
 
 [tool.poetry.group.lint.dependencies]
 mypy = "1.10.0"
-django-stubs = "5.0.0"
+django-stubs = "5.0.2"
 
 [tool.ruff]
 fix = true
+unsafe-fixes = true
 line-length = 120
 extend-exclude = [
-    "tests/*",
+    "tests*",
 ]
-
-[tool.ruff.lint]
-typing-modules = [
+lint.typing-modules = [
     "lookup_property.typing",
 ]
-select = [
+lint.explicit-preview-rules = true
+lint.preview = true
+lint.select = [
     "A",        # flake8-builtins
     "ANN",      # flake8-annotations
     "ARG",      # flake8-unused-arguments
     "B",        # flake8-bugbear
     "BLE",      # flake8-blind-except
     "C90",      # mccabe
     "C4",       # flake8-comprehensions
     "COM",      # flake8-commas
     "D200",     # pydocstyle: One-line docstring should fit on one line
     "D201",     # pydocstyle: No blank lines allowed before function docstring (found {num_lines})
     "D202",     # pydocstyle: No blank lines allowed after function docstring (found {num_lines})
     "D209",     # pydocstyle: Multi-line docstring closing quotes should be on a separate line
     "D213",     # pydocstyle: Multi-line docstring summary should start at the second line
+    "DJ",       # flake8-django
     "DTZ",      # flake8-datetimez
     "E",        # pycodestyle errors
     "EM",       # flake8-errmsg
     "F",        # pyflakes
+    "FA",       # flake8-future-annotations
     "FBT",      # flake8-boolean-trap
+    "FLY",      # flynt
+    "G",        # flake8-logging-format
     "I",        # isort
+    "ICN",      # flake8-import-conventions
     "INP",      # flake8-no-pep420
+    "INT",      # flake8-gettext
     "ISC",      # flake8-implicit-str-concat
+    "LOG",      # flake8-logging
     "N",        # pep8-naming
     "PERF",     # perflint
     "PGH",      # pygrep-hooks
     "PIE",      # flake8-pie
     "PL",       # pylint
     "PT",       # flake8-pytest-style
     "PTH",      # flake8-use-pathlib
     "PYI",      # flake8-pyi
     "Q",        # flake8-quotes
+    "R",        # Refactor
     "RET",      # flake8-return
     "RSE",      # flake8-raise
     "RUF",      # ruff-specific rules
     "S",        # flake8-bandit
     "SIM",      # flake8-simplify
+    "SLF",      # flake8-self
     "T20",      # flake8-print
     "TCH",      # flake8-type-checking
+    "TID",      # flake8-tidy-imports
     "TRY",      # tryceratops
     "UP",       # pyupgrade
     "W",        # pycodestyle warnings
 ]
-ignore = [
+# Preview rules
+lint.extend-select = [
+    "B909",     # loop-iterator-mutation
+    "FURB110",  # if-exp-instead-of-or-operator
+    "FURB142",  # for-loop-set-mutations
+    "FURB145",  # slice-copy
+    "FURB171",  # single-item-membership-test
+    "FURB187",  # list-reverse-copy
+    "PLE0307",  # invalid-str-return-type
+    "PLR0916",  # too-many-boolean-expressions
+    "PLR1730",  # if-stmt-min-max
+    "PLR1733",  # unnecessary-dict-index-lookup
+    "PLR1736",  # unnecessary-list-index-lookup
+    "PLR6104",  # non-augmented-assignment
+    "PLW0211",  # bad-staticmethod-argument
+    "PLW0642",  # self-or-cls-assignment
+    "RUF021",   # parenthesize-chained-operators
+    "RUF022",   # unsorted-dunder-all
+    "UP042",    # replace-str-enum
+]
+lint.ignore = [
     "ANN101",   # Missing type annotation for `self` in method
-    "ANN401",   # Any is allowed
-    "S311",     # random-module is OK.
+    "ANN102",   # Missing type annotation for `cls` in method
+    "ANN401",   # Any-typing allowed
+    "ARG001",   # Unused function argument
+    "ARG002",   # Unused method argument
+    "ARG003",   # Unused class method argument
+    "G004",     # Logging statement uses f-string
+    "S602",     # Broken: https://github.com/astral-sh/ruff/issues/4045
+    "S603",     # Broken: https://github.com/astral-sh/ruff/issues/4045
+    "TCH001",
+    "TCH002",
     #
     # Conflicting with ruff-format
     #
-    "COM812",   # Trailing comma missing
-    "COM819",   # Trailing comma prohibited
-    "E501",     # Line too long
-    "ISC001",   # Implicitly concatenated string literals on one line
-    "Q000",     # Single quotes found but double quotes preferred
-    "Q001",     # Single quote multiline found but double quotes preferred
-    "Q002",     # Single quote docstring found but double quotes preferred
-    "Q003",     # Change outer quotes to avoid escaping inner quotes
-    "W191",     # Indentation contains tabs
+    "COM812",   # missing-trailing-comma
+    "COM819",   # prohibited-trailing-comma
+    "D206",     # indent-with-spaces
+    "D300",     # triple-single-quotes
+    "E111",     # indentation-with-invalid-multiple
+    "E114",     # indentation-with-invalid-multiple-comment
+    "E117",     # over-indented
+    "ISC001",   # single-line-implicit-string-concatenation
+    "ISC002",   # multi-line-implicit-string-concatenation
+    "Q000",     # bad-quotes-inline-string
+    "Q001",     # bad-quotes-multiline-string
+    "Q002",     # bad-quotes-docstring
+    "Q003",     # avoidable-escaped-quote
+    "W191",     # tab-indentation
 ]
 
 [tool.ruff.lint.extend-per-file-ignores]
-"lookup_property/converters/*.py" = [
-    "ARG001",   # Unused function argument
+"test_*.py" = [
+    "ANN",      # No need to annotate tests
+    "N801",     # Allow whatever class names in tests
+    "N802",     # Allow whatever function names in tests
+    "N815",     # Allow whatever variable names in tests
+    "PLR0915",  # Can have as many statements as needed
+    "PLR2004",  # Magic value comparisons are allowed in tests
+    "S101",     # Assert is fine
+    "S105",     # Hardcoded passwords are fine in tests
+    "S106",     # Hardcoded passwords are fine in tests
+    "S108",     # No need to care about insecure temp file usages in tests
+    "S311",     # Pseudo-random generators are fine here
+    "SLF",      # Allow accessing private members in tests
+    "UP",       # No upgrade rules
+]
+"conftest.py" = [
+    "ARG",      # Fixtures can be unused
+    "ANN",      # No need to annotate tests
+    "UP",       # No upgrade rules
+]
+
+[tool.ruff.lint.isort]
+combine-as-imports = false
+split-on-trailing-comma = false
+known-third-party = [
+    "django",
 ]
+known-first-party = [
+    "query_optimizer",
+]
+
+[tool.ruff.lint.flake8-import-conventions]
+banned-from = [
+    "base64",
+    "csv",
+    "datetime",
+    "hashlib",
+    "hmac",
+    "json",
+    "logging",
+    "math",
+    "os",
+    "pickle",
+    "random",
+    "re",
+    "shutil",
+    "subprocess",
+    "sys",
+    "tempfile",
+    "time",
+    "uuid",
+    "xml",
+    "yaml",
+]
+
+[tool.ruff.lint.flake8-self]
+extend-ignore-names = [
+    "_base_manager",
+    "_default_manager",
+    "_meta",
+]
+
+[tool.ruff.lint.pylint]
+max-args = 7
 
 [tool.mypy]
 python_version = "3.12"
 warn_return_any = "True"
 warn_unused_configs = "True"
 plugins = [
     "mypy_django_plugin.main",
```

### Comparing `django_lookup_property-0.1.5/PKG-INFO` & `django_lookup_property-0.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-lookup-property
-Version: 0.1.5
+Version: 0.1.6
 Summary: Django model properties that are also lookup expressions.
 Home-page: https://mrthearman.github.io/django-lookup-property
 License: MIT
 Keywords: django,lookup,property,orm,model,extension
 Author: Matti Lamppu
 Author-email: lamppu.matti.akseli@gmail.com
 Requires-Python: >=3.11,<4
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: Django (>=4.2)
 Project-URL: Bug Tracker, https://github.com/MrThearMan/django-lookup-property/issues
+Project-URL: Documentation, https://mrthearman.github.io/django-lookup-property
 Project-URL: Repository, https://github.com/MrThearMan/django-lookup-property
 Description-Content-Type: text/markdown
 
 # Django Lookup Property
 
 [![Coverage Status][coverage-badge]][coverage]
 [![GitHub Workflow Status][status-badge]][status]
```

