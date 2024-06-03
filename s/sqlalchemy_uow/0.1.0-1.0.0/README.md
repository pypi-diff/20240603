# Comparing `tmp/sqlalchemy_uow-0.1.0.tar.gz` & `tmp/sqlalchemy_uow-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_uow-0.1.0.tar", max compression
+gzip compressed data, was "sqlalchemy_uow-1.0.0.tar", max compression
```

## Comparing `sqlalchemy_uow-0.1.0.tar` & `sqlalchemy_uow-1.0.0.tar`

### file list

```diff
@@ -1,10 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-01-11 14:18:36.794464 sqlalchemy_uow-0.1.0/LICENSE
--rw-r--r--   0        0        0     2713 2023-01-11 14:18:36.811968 sqlalchemy_uow-0.1.0/README.md
--rw-r--r--   0        0        0     1093 2023-01-25 16:15:57.281409 sqlalchemy_uow-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      197 2023-01-11 14:18:36.851230 sqlalchemy_uow-0.1.0/src/sqlalchemy_uow/__init__.py
--rw-r--r--   0        0        0     3294 2023-01-25 16:15:32.875193 sqlalchemy_uow-0.1.0/src/sqlalchemy_uow/repository.py
--rw-r--r--   0        0        0      352 2023-01-12 14:06:58.532848 sqlalchemy_uow-0.1.0/src/sqlalchemy_uow/settings.py
--rw-r--r--   0        0        0     1618 2023-01-14 09:10:25.990016 sqlalchemy_uow-0.1.0/src/sqlalchemy_uow/unit_of_work.py
--rw-r--r--   0        0        0      379 2023-01-12 14:33:22.424253 sqlalchemy_uow-0.1.0/src/sqlalchemy_uow/utils.py
--rw-r--r--   0        0        0     3559 1970-01-01 00:00:00.000000 sqlalchemy_uow-0.1.0/setup.py
--rw-r--r--   0        0        0     3259 1970-01-01 00:00:00.000000 sqlalchemy_uow-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-01-11 14:18:36.794464 sqlalchemy_uow-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2713 2023-01-11 14:18:36.811968 sqlalchemy_uow-1.0.0/README.md
+-rw-r--r--   0        0        0     1093 2024-06-03 04:44:49.363386 sqlalchemy_uow-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-31 08:56:00.048688 sqlalchemy_uow-1.0.0/src/sqlalchemy_uow/__init__.py
+-rw-r--r--   0        0        0     2772 2024-05-31 13:01:10.330458 sqlalchemy_uow-1.0.0/src/sqlalchemy_uow/repository.py
+-rw-r--r--   0        0        0     1206 2024-05-31 13:01:10.348945 sqlalchemy_uow-1.0.0/src/sqlalchemy_uow/unit_of_work.py
+-rw-r--r--   0        0        0      378 2024-05-31 08:56:00.049345 sqlalchemy_uow-1.0.0/src/sqlalchemy_uow/utils.py
+-rw-r--r--   0        0        0     3310 1970-01-01 00:00:00.000000 sqlalchemy_uow-1.0.0/PKG-INFO
```

### Comparing `sqlalchemy_uow-0.1.0/LICENSE` & `sqlalchemy_uow-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_uow-0.1.0/README.md` & `sqlalchemy_uow-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy_uow-0.1.0/pyproject.toml` & `sqlalchemy_uow-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sqlalchemy_uow"
-version = "0.1.0"
+version = "1.0.0"
 description = "Unit of Work for SQLAlchemy project"
 authors = [
     "Barbara Jesacher <barbarajesacher@icloud.com>",
 ]
 readme = "README.md"
 license = "MIT"
```

### Comparing `sqlalchemy_uow-0.1.0/src/sqlalchemy_uow/unit_of_work.py` & `sqlalchemy_uow-1.0.0/src/sqlalchemy_uow/unit_of_work.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,65 +1,50 @@
-# pylint: disable=attribute-defined-outside-init
-"""
-# Unit of Work
-
-Interface to repository.
-
-With help of this module the tool is independent of the database.
-"""
-from __future__ import annotations
-
-from abc import ABC, abstractmethod
-from sqlalchemy.orm.session import Session
-
-from .repository import AbstractRepository, SqlAlchemyRepository, FakeRepository
-
-
-class AbstractUnitOfWork(ABC):
-    items: AbstractRepository
-
-    def __enter__(self) -> AbstractUnitOfWork:
-        return self                             # pragma: no cover
-
-    def __exit__(self, *args):
-        self.rollback()                         # pragma: no cover
-
-    @abstractmethod
-    def commit(self):
-        raise NotImplementedError               # pragma: no cover
-
-    @abstractmethod
-    def rollback(self):
-        raise NotImplementedError               # pragma: no cover
-
-
-class SqlAlchemyUnitOfWork(AbstractUnitOfWork, ABC):
-
-    def __init__(self, session_factory):
-        self.session_factory = session_factory
-
-    def __enter__(self):
-        self.session = self.session_factory()  # type: Session
-        self.items = SqlAlchemyRepository(self.session)
-        return super().__enter__()
-
-    def __exit__(self, *args):
-        super().__exit__(*args)
-        self.session.close()
-
-    def commit(self):
-        self.session.commit()
-
-    def rollback(self):
-        self.session.rollback()
-
-
-class FakeUnitOfWork(AbstractUnitOfWork):
-    def __init__(self):
-        self.items = FakeRepository([])
-        self.committed = False
-
-    def commit(self):
-        self.committed = True
-
-    def rollback(self):
-        pass
+# pylint: disable=attribute-defined-outside-init
+"""
+# Unit of Work
+
+Interface to repository.
+
+With help of this module the tool is independent of the database.
+"""
+from abc import ABC, abstractmethod
+
+from src.sqlalchemy_uow.repository import AbstractRepository, SqlAlchemyRepository
+
+
+class AbstractUnitOfWork(ABC):
+    items: AbstractRepository
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, *args):
+        self.rollback()
+
+    @abstractmethod
+    def commit(self):  # pragma: no cover
+        raise NotImplementedError
+
+    @abstractmethod
+    def rollback(self):  # pragma: no cover
+        raise NotImplementedError
+
+
+class SqlAlchemyUnitOfWork(AbstractUnitOfWork, ABC):
+
+    def __init__(self, session_factory):
+        self.session_factory = session_factory
+
+    def __enter__(self):
+        self.session = self.session_factory()
+        self.items = SqlAlchemyRepository(self.session)
+        return super().__enter__()
+
+    def __exit__(self, *args):
+        super().__exit__(*args)
+        self.session.close()
+
+    def commit(self):
+        self.session.commit()
+
+    def rollback(self):
+        self.session.rollback()
```

### Comparing `sqlalchemy_uow-0.1.0/PKG-INFO` & `sqlalchemy_uow-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
-Name: sqlalchemy-uow
-Version: 0.1.0
+Name: sqlalchemy_uow
+Version: 1.0.0
 Summary: Unit of Work for SQLAlchemy project
 License: MIT
 Author: Barbara Jesacher
 Author-email: barbarajesacher@icloud.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: hydra-core (>=1.1.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # sqlalchemy-uow
 
 Unit of Work for SQLAlchemy project
```

