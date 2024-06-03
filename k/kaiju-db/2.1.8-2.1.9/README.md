# Comparing `tmp/kaiju_db-2.1.8-py3-none-any.whl.zip` & `tmp/kaiju_db-2.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 20882 bytes, number of entries: 12
--rw-r--r--  2.0 unx      184 b- defN 23-Jul-27 19:34 kaiju_db/__init__.py
--rw-r--r--  2.0 unx     3740 b- defN 23-Jul-27 19:34 kaiju_db/functions.py
--rw-r--r--  2.0 unx    61457 b- defN 23-Jul-27 19:34 kaiju_db/services.py
--rw-r--r--  2.0 unx      453 b- defN 23-Jul-27 19:34 kaiju_db/types.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-27 19:34 kaiju_db/tests/__init__.py
--rw-r--r--  2.0 unx     3292 b- defN 23-Jul-27 19:34 kaiju_db/tests/fixtures.py
--rw-r--r--  2.0 unx     4846 b- defN 23-Jul-27 19:34 kaiju_db/tests/test_db.py
--rw-rw-rw-  2.0 unx      610 b- defN 23-Jul-27 19:34 kaiju_db-2.1.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     3259 b- defN 23-Jul-27 19:34 kaiju_db-2.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-27 19:34 kaiju_db-2.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-27 19:34 kaiju_db-2.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      939 b- defN 23-Jul-27 19:34 kaiju_db-2.1.8.dist-info/RECORD
-12 files, 78881 bytes uncompressed, 19310 bytes compressed:  75.5%
+Zip file size: 22533 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      184 b- defN 23-Dec-14 15:13 kaiju_db/__init__.py
+-rw-r--r--  2.0 unx     3795 b- defN 23-Dec-14 15:13 kaiju_db/functions.py
+-rw-r--r--  2.0 unx    68609 b- defN 23-Dec-14 15:13 kaiju_db/services.py
+-rw-r--r--  2.0 unx     1176 b- defN 23-Dec-14 15:13 kaiju_db/types.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Dec-14 15:13 kaiju_db/tests/__init__.py
+-rw-r--r--  2.0 unx     3292 b- defN 23-Dec-14 15:13 kaiju_db/tests/fixtures.py
+-rw-r--r--  2.0 unx     4830 b- defN 23-Dec-14 15:13 kaiju_db/tests/test_db.py
+-rw-rw-rw-  2.0 unx      610 b- defN 23-Dec-14 15:13 kaiju_db-2.1.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3026 b- defN 23-Dec-14 15:13 kaiju_db-2.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Dec-14 15:13 kaiju_db-2.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Dec-14 15:13 kaiju_db-2.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      940 b- defN 23-Dec-14 15:13 kaiju_db-2.1.9.dist-info/RECORD
+12 files, 86563 bytes uncompressed, 20961 bytes compressed:  75.8%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: kaiju_db/tests/fixtures.py
 Comment: 
 
 Filename: kaiju_db/tests/test_db.py
 Comment: 
 
-Filename: kaiju_db-2.1.8.dist-info/LICENSE
+Filename: kaiju_db-2.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: kaiju_db-2.1.8.dist-info/METADATA
+Filename: kaiju_db-2.1.9.dist-info/METADATA
 Comment: 
 
-Filename: kaiju_db-2.1.8.dist-info/WHEEL
+Filename: kaiju_db-2.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: kaiju_db-2.1.8.dist-info/top_level.txt
+Filename: kaiju_db-2.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: kaiju_db-2.1.8.dist-info/RECORD
+Filename: kaiju_db-2.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kaiju_db/__init__.py

```diff
@@ -1,8 +1,8 @@
 from .types import *
 from .functions import *
 from .services import *
 
-__version__ = '2.1.8'
+__version__ = '2.1.9'
 __python_version__ = '3.11'
 __author__ = 'antonnidhoggr@me.com'
 __service_package__ = True
```

## kaiju_db/functions.py

```diff
@@ -1,15 +1,16 @@
+"""SQL functions related classes."""
+
 from typing import Tuple, Type
 
+from kaiju_tools.registry import ClassRegistry
 from sqlalchemy import DDL
 from sqlalchemy.event import listen
 from sqlalchemy.sql.functions import GenericFunction
 
-from kaiju_tools.registry import ClassRegistry
-
 
 __all__ = ['DDL', 'UserFunction', 'SQLFunctionsRegistry', 'SQL_FUNCTIONS']
 
 
 def DDL(target, identifier, body):  # noqa
     """
     Specifies literal SQL DDL to be executed by the database.  DDL objects
@@ -115,19 +116,19 @@
             body = f'FUNCTION {body}'
         if not body.endswith(';'):
             body += ';'
         return body
 
 
 class SQLFunctionsRegistry(ClassRegistry):
-    """A simple registry for SQL functions."""
+    """Registry for SQL functions."""
 
     @classmethod
-    def get_base_classes(cls) -> Tuple[Type, ...]:
+    def get_base_classes(cls) -> tuple[type, ...]:
         return (UserFunction,)
 
     @classmethod
     def get_key(cls, obj) -> str:
         return obj.name
 
 
-SQL_FUNCTIONS = SQLFunctionsRegistry(raise_if_exists=False)
+SQL_FUNCTIONS = SQLFunctionsRegistry(raise_if_exists=False)  #: sql functions registry
```

## kaiju_db/services.py

```diff
@@ -1,38 +1,37 @@
 """Database services."""
 
 import abc
 from collections.abc import AsyncGenerator, Collection, Hashable
 from enum import Enum
 from functools import cached_property
 from pathlib import Path
-from typing import Generic, List, Literal, Optional, TypedDict, TypeVar, Union, cast, final
+from typing import Any, Generic, List, Literal, Optional, TypedDict, TypeVar, Union, cast, final
 
 import sqlalchemy as sa
 import sqlalchemy.dialects.postgresql as sa_pg
 from kaiju_tools.app import SERVICE_CLASS_REGISTRY, ContextableService, Service
 from kaiju_tools.encoding import dumps, load, loads
 from kaiju_tools.exceptions import Conflict, InternalError, MethodNotAllowed, NotFound, ValidationError
 from kaiju_tools.interfaces import DataStore, Locks, PublicInterface
 from sqlalchemy import MetaData, Table, text
+from sqlalchemy.engine import Result
 from sqlalchemy.exc import IntegrityError
 from sqlalchemy.ext.asyncio import create_async_engine
-from sqlalchemy.sql.expression import nullslast  # noqa: package
+from sqlalchemy.sql.expression import nullslast  # noqa pycharm
 
 from kaiju_db.functions import SQL_FUNCTIONS, UserFunction
+from kaiju_db.types import MigrationState
 
 
 __all__ = ['DatabaseService', 'SQLService', 'PermHook', 'FixtureService', 'DatabaseMigrationService']
 
 
-async def setup_asyncpg_jsonb_codec(conn):
-    """Set up JSONB codec for asyncpg.
-
-    Overriden for binary json serializer.
-    """
+async def _setup_asyncpg_jsonb_codec(conn):
+    """Set up JSONB codec for asyncpg overriden for binary json serializer."""
 
     def _jsonb_encoder(str_value):
         # \x01 is the prefix for jsonb used by Postgres.
         # asyncpg requires it when format='binary'
         return b'\x01' + str_value
 
     def _jsonb_decoder(bin_value):
@@ -72,21 +71,22 @@
         root_password: str = '',
         root_database: str = 'postgres',
         metadata: MetaData = None,
         init_db: bool = True,
         init_tables: bool = True,
         pool_size: int = 10,
         idle_connection_lifetime: int = 3600,
-        extensions: list[str] = None,
+        extensions: List[str] = None,
         functions=SQL_FUNCTIONS,
+        echo: bool = False,
         logger=None,
     ):
         """Initialize.
 
-        :param app:
+        :param app: web app
         :param host: db url or address
         :param port: db port
         :param database: db name
         :param user: db user (non-root)
         :param password: db user password (non-root)
         :param root_user: root user is required only for database and extensions initialization
         :param root_password: root user is required only for database and extensions initialization
@@ -94,18 +94,19 @@
         :param metadata: optional SA metadata object
         :param init_db: perform database and pg extensions initialization upon start (requires root credentials)
         :param init_tables: initialize tables upon start (in not present)
         :param pool_size: connection pool size
         :param idle_connection_lifetime: connection idle lifetime before recycling
         :param extensions: list of pg extensions to init (init_db flag should be enabled)
         :param functions: optional function registry for pre-defined functions
-        :param logger:
+        :param echo: echo SQL requests in console
+        :param logger: optional logger
         """
-        super().__init__(app, logger)
-        self.metadata = metadata if metadata else self.app.db_meta  # noqa
+        super().__init__(app=app, logger=logger)
+        self.metadata = metadata if metadata else self.app.db_meta
         self._host = host
         self._port = port
         self._db = database
         self._user = user
         self._password = password
         self._root_user = root_user if root_user else user
         self._root_password = root_password if root_password else password
@@ -113,132 +114,172 @@
         self._init_db = init_db
         self._init_tables = any((init_tables, init_db))
         self._pool_size = pool_size
         self._idle_connection_lifetime = idle_connection_lifetime
         self._extensions = extensions
         self._functions_registry = functions
         self._engine = None
+        self._echo = echo
 
     @property
     def engine(self):
-        """Alias to the SA async engine."""
+        """Get sqlalchemy async engine.
+
+        See `sqlalchemy.AsyncEngine <https://docs.sqlalchemy.org/en/20/orm/extensions/\
+            asyncio.html#sqlalchemy.ext.asyncio.AsyncEngine>`_
+        """
         return self._engine
 
     def begin(self, *args, **kws):
-        """Alias to the SA engine transaction begin.
+        """Start an sqlalchemy transaction with auto-commit.
+
+        See `sqlalchemy.AsyncEngine.begin <https://docs.sqlalchemy.org/en/20/orm/extensions/\
+            asyncio.html#sqlalchemy.ext.asyncio.AsyncEngine.begin>`_
 
         .. code-block:: python
 
             async with db.begin() as conn:
                 ...  # transaction block
-                await conn.commit()
 
         """
         return self.engine.begin(*args, **kws)
 
     def connect(self, *args, **kws):
-        """Alias to the SA engine connection.
+        """Start an sqlalchemy transaction with no auto-commit.
+
+        See `sqlalchemy.AsyncEngine.connect <https://docs.sqlalchemy.org/en/20/orm/extensions/\
+            asyncio.html#sqlalchemy.ext.asyncio.AsyncEngine.connect>`_
 
         .. code-block:: python
 
             async with db.connect() as conn:
-                ...
+                ...  # transaction block
                 await conn.commit()
 
         """
         return self.engine.connect(*args, **kws)
 
-    async def execute(self, __obj, *args, _commit=True, _conn=None, **kws):
-        """Execute an SQL command."""
+    async def execute(self, __obj, *args, _commit=True, _conn=None, **kws) -> Result:
+        """Execute a single SQL command.
+
+        A wrapper around `sqlalchemy.AsyncConnection.execute <https://docs.sqlalchemy.org/en/20/orm/extensions/\
+            asyncio.html#sqlalchemy.ext.asyncio.AsyncConnection.execute>`_
+
+        This method will return a `sqlalchemy.Result object <https://docs.sqlalchemy.org/en/20/core/\
+            connections.html#sqlalchemy.engine.Result>`_ so you can use `result.all()` or `result.first()` etc.
+            to retrieve results (these methods are synchronous) depending on what you need. These methods return
+            *namedtuple rows*. To convert a namedtuple to a old-style dictionary use `row._asdict()` method.
+        """
         if type(__obj) is str:
             __obj = text(__obj)
         if _conn:
             result = await _conn.execute(__obj, *args, **kws)
         else:
             async with self._engine.connect() as conn:
                 result = await conn.execute(__obj, *args, **kws)
                 if _commit:
                     await conn.commit()
         return result
 
-    async def fetchrow(self, __obj, *args, _commit=True, _conn=None, **kws):
-        """Execute an SQL command and fetch the first result."""
+    async def fetchrow(self, __obj, *args, _commit=True, _conn=None, **kws) -> dict | None:
+        """Execute an SQL command and fetch the first row.
+
+        A wrapper around `sqlalchemy.AsyncConnection.executoe <https://docs.sqlalchemy.org/en/20/orm/extensions/\
+            asyncio.html#sqlalchemy.ext.asyncio.AsyncConnection.execute>`_
+
+        Returns the first row as dict or None.
+        """
         result = await self.execute(__obj, *args, _commit=_commit, _conn=_conn, **kws)
         result = result.first()
         return result._asdict() if result else None  # noqa
 
-    async def fetch(self, __obj, *args, _commit=True, _conn=None, **kws):
-        """Execute an SQL command and fetch all results."""
+    async def fetch(self, __obj, *args, _commit=True, _conn=None, **kws) -> List[dict]:
+        """Execute an SQL command and fetch all the results.
+
+        A wrapper around `sqlalchemy.AsyncConnection.executoe <https://docs.sqlalchemy.org/en/20/orm/extensions/\
+            asyncio.html#sqlalchemy.ext.asyncio.AsyncConnection.execute>`_
+
+        Returns a list of rows as dicts.
+        """
         result = await self.execute(__obj, *args, _commit=_commit, _conn=_conn, **kws)
         return [r._asdict() for r in result.all()]  # noqa
 
-    async def fetchval(self, __obj, *args, _commit=True, _conn=None, **kws):
-        """Execute an SQL command and fetch a first column in the first result."""
+    async def fetchval(self, __obj, *args, _commit=True, _conn=None, **kws) -> Any:
+        """Execute an SQL command and fetch the first column of the first row.
+
+        A wrapper around `sqlalchemy.AsyncConnection.executoe <https://docs.sqlalchemy.org/en/20/orm/extensions/\
+            asyncio.html#sqlalchemy.ext.asyncio.AsyncConnection.execute>`_
+        """
         result = await self.execute(__obj, *args, _commit=_commit, _conn=_conn, **kws)
         return result.scalar()
 
     async def init(self):
         if self._init_db:
             await self._init_database()
         # self._root_user = None
         # self._root_password = None
         self._engine = self._create_engine(self._user, self._password, self._db)
-        self._engine.dialect.setup_asyncpg_jsonb_codec = setup_asyncpg_jsonb_codec
+        self._engine.dialect.setup_asyncpg_jsonb_codec = _setup_asyncpg_jsonb_codec
         if self._init_tables:
             async with self._engine.connect() as conn:
                 await conn.execution_options(**{'isolation_level': 'AUTOCOMMIT'})
                 await self._create_functions(conn)
                 await conn.run_sync(self.metadata.create_all, checkfirst=True)
 
     async def close(self):
         if self._engine:
             await self._engine.dispose()
             self._engine = None
 
     def add_table(self, table: Table) -> Table:
-        """Register a table in SA metadata.
+        """Register a table in the database service metadata.
 
         This method must be called before async init if you want to automatically create this table at start time.
+        SQL services do this automatically for their tables.
         """
         if table.name in self.metadata:
             return self.metadata.tables[table.name]
         else:
             self.metadata._add_table(table.name, None, table)  # noqa
             table.metadata = self.metadata
             return table
 
-    async def _init_database(self):
+    async def _init_database(self) -> None:
+        """Initialize the database (root credentials are required)."""
         # root pool for root db
         engine = self._create_engine(self._root_user, self._root_password, self._root_database)
-        engine.dialect.setup_asyncpg_jsonb_codec = setup_asyncpg_jsonb_codec
+        engine.dialect.setup_asyncpg_jsonb_codec = _setup_asyncpg_jsonb_codec
         async with engine.connect() as conn:
             await conn.execution_options(**{'isolation_level': 'AUTOCOMMIT'})
             if not await self._db_exists(conn):
                 await self._create_db(conn)
             if not await self._user_exists(conn):
                 await self._create_user(conn)
         await engine.dispose()
         if self._extensions:
             # postgres can create extension only if superuser :-(
             engine = self._create_engine(self._root_user, self._root_password, self._db)
-            engine.dialect.setup_asyncpg_jsonb_codec = setup_asyncpg_jsonb_codec
+            engine.dialect.setup_asyncpg_jsonb_codec = _setup_asyncpg_jsonb_codec
             async with engine.connect() as conn:
                 await conn.execution_options(**{'isolation_level': 'AUTOCOMMIT'})
                 for ext in self._extensions:
                     await self._create_extension(conn, ext)
             await engine.dispose()
 
     def _create_engine(self, user: str, password: str, db: str):
+        """Create a fresh asyncpg engine."""
         self.logger.debug('Initializing a pool for user "%s" in database "%s".', user, db)
         engine = create_async_engine(
             f'postgresql+asyncpg://{user}:{password}@{self._host}:{self._port}/{db}',
             json_serializer=dumps,
             json_deserializer=loads,
             pool_size=self._pool_size,
             pool_recycle=self._idle_connection_lifetime,
+            pool_pre_ping=True,
+            echo=self._echo,
         )
         return engine
 
     async def _db_exists(self, conn) -> bool:
         self.logger.debug('Checking database "%s".', self._db)
         result = await conn.execute(text(f"SELECT 1 FROM pg_database WHERE datname = '{self._db}';"))  # noqa
         return bool(result.first())
@@ -283,27 +324,27 @@
     desc: str
 
 
 _Id = TypeVar('_Id', bound=Hashable)
 _Row = TypeVar('_Row', bound=dict)
 _Columns = Union[Collection[str], Literal['*'], None]
 _SortField = Union[_SortDesc, _SortAsc, str]
-_Sort = Optional[list[_SortField]]
-_Condition = Union[dict, list[dict], None]
+_Sort = Optional[List[_SortField]]
+_Condition = Union[dict, List[dict], None]
 
 
 class _List(TypedDict):
     """Type hinting for a list query."""
 
     count: int | None  #: total rows matching the query, None if count hasn't been requested
     offset: int  #: row offset for this selection
     page: int | None  #: current page number, None if count hasn't been requested
     pages: int | None  #: total pages, None if count hasn't been requested
     on_page: int  #: number of rows on this page
-    data: list[_Row] | None  #: returned rows, None if limit was set to 0
+    data: List[_Row] | None  #: returned rows, None if limit was set to 0
 
 
 class SQLService(Service, DataStore, Generic[_Id, _Row], abc.ABC):
     """Base SQL service interface with common commands and errors.
 
     Optimized for a single primary key only with a name "id"
 
@@ -353,31 +394,35 @@
         FIELD_DOES_NOT_EXISTS = 'query.field_does_not_exists'
         INVALID_CONDITION = 'query.invalid_condition_command'
         INVALID_ORDERING = 'query.invalid_ordering_command'
         INVALID_PAGINATION_OFFSET = 'query.invalid_pagination_offset'
         INVALID_PAGINATION_LIMIT = 'query.invalid_pagination_limit'
         INVALID_COLUMN = 'query.invalid_insert_column'
 
-    DEFAULT_ROW_LIMIT = 24  #: defaults of LIMIT on queries
-    MAX_ROW_LIMIT = 1000  #: max size of queries
-    MAX_GET_QUERY_SIZE = 65535
+    DEFAULT_ROW_LIMIT = 24  #: defaults row limit on list / iter queries
+    MAX_ROW_LIMIT = 1000  #: max page size in list / iter queries
 
     select_columns = None  #: you can specify a whitelist of output columns here
     select_columns_blacklist = None
     update_columns = None  #: you may specify columns for update here
     update_columns_blacklist = None
     insert_columns = None  #: you may specify insert columns here
     insert_columns_blacklist = None
     table = None  #: here should be your table
 
     virtual_columns = None  # virtual SQL columns (i.e. functions) names and definitions
     # virtual columns can be selected but never updated / inserted
 
-    def __init__(self, app, database_service: DatabaseService | str = None, logger=None):
-        """Initialize."""
+    def __init__(self, app, database_service: DatabaseService = None, logger=None):
+        """Initialize.
+
+        :param app: web app
+        :param database_service: database transport service
+        :param logger: optional logger instance
+        """
 
         def _prepare_whitelist(whitelist, blacklist):
             if blacklist:
                 whitelist = {col.name for col in self.table.columns} if whitelist is None else set(whitelist)
                 return frozenset(whitelist.difference(set(blacklist)))
             elif whitelist:
                 return frozenset(whitelist)
@@ -419,30 +464,52 @@
             'm_update': self.m_update,
             'm_delete': self.m_delete,
             'list': self.list,
         }
 
     @staticmethod
     def get_condition_hook(sql):
-        """Set up specific get conditions."""
+        """Set up specific get conditions.
+
+        You can use this hook to impose permission check based on current user session, add some conditions
+        to filter out data for public (rpc) output etc.
+
+        Example:
+
+        .. code-block:: python
+
+            def get_condition_hook(self, sql):
+                sql = sql.where(self.table.c.enabled.is_(True))
+                return sql
+
+        """
         return sql
 
     @staticmethod
     def insert_condition_hook(sql):
-        """Set up specific insert conditions."""
+        """Set up specific insert conditions.
+
+        Similar to :py:meth:`~kaiju_db.services.SQLService.get_condition_hook`.
+        """
         return sql
 
     @staticmethod
     def update_condition_hook(sql):
-        """Set up specific update conditions."""
+        """Set up specific update conditions.
+
+        Similar to :py:meth:`~kaiju_db.services.SQLService.get_condition_hook`.
+        """
         return sql
 
     @staticmethod
     def delete_condition_hook(sql):
-        """Set up specific delete conditions."""
+        """Set up specific delete conditions.
+
+        Similar to :py:meth:`~kaiju_db.services.SQLService.get_condition_hook`.
+        """
         return sql
 
     def _create_primary_key_condition_for_single_key(self, sql, _id: _Id):
         return sql.where(self._primary_key == _id)
 
     def _create_list_primary_key_condition_for_single_key(self, sql, _id: _Id | Collection[_Id]):
         if not isinstance(_id, (list, tuple, set)):
@@ -531,20 +598,21 @@
         sql = self.get_condition_hook(sql)
         sql = sql.limit(1)
         return sql
 
     async def exists(self, id: _Id, _connection=None) -> bool:
         """Return True if object exists. False otherwise.
 
-        If you have composite primary keys you should pass dictionary objects
-        in id field, like this:
+        :param id: object id
+
+        If you have composite primary keys you should pass them as tuples:
 
         .. code-block:: python
 
-            await service.exists({'id': 1, 'key': 'abc'})
+            await service.exists((1, 'abc'), ...)
 
         """
         sql = self._create_exists_query(id)
         result = await self._wrap_get(_connection, sql)
         return bool(result.first())
 
     def _create_m_exists_query(self, _id: Collection[_Id], table=None):
@@ -554,20 +622,26 @@
         sql = self._list_primary_key_condition(sql, _id)
         sql = self.get_condition_hook(sql)
         return sql
 
     async def m_exists(self, id: Collection[_Id], _connection=None) -> frozenset[_Id]:
         """Return a set of existing IDs for a list of IDs.
 
-        If you have composite primary keys you should pass dictionary objects
-        in id field, like this:
+        :param id: list of object ids
+        :returns: a set of existing ids
+
+        .. note::
+
+            Be aware that there is database limit on max number of ids per query (65535 in postgres).
+
+        If you have composite primary keys you should pass them as tuples:
 
         .. code-block:: python
 
-            await service.m_exists([{'id': 1, 'key': 'abc'}, ...])
+            await service.m_exists([(1, 'abc'), ...])
 
         """
         sql = self._create_m_exists_query(id)
         result = await self._wrap_get(_connection, sql)
         rows = result.all()
         if rows:
             if self._composite_primary_key:
@@ -642,15 +716,15 @@
                     columns = [self._sql_get_column(table, key) for key in columns if key in self.select_columns]
                 else:
                     columns = [self._sql_get_column(table, key) for key in columns]
 
         return columns
 
     @staticmethod
-    def _filter_columns(columns: list[sa.Column], whitelist: frozenset | None):
+    def _filter_columns(columns: List[sa.Column], whitelist: frozenset | None):
         if whitelist is None:
             return columns
         else:
             return [col for col in columns if col.name in whitelist]
 
     def _create_get_query(self, _id: _Id, columns, table=None):
         if table is None:
@@ -661,22 +735,24 @@
         sql = self.get_condition_hook(sql)
         sql = sql.limit(1)
         return sql
 
     async def get(self, id: _Id, columns: _Columns = '*', _connection=None) -> _Row:
         """Return information about an object.
 
-        If you have composite primary keys you should pass dictionary objects
-        in id field, like this:
+        :param id: object id
+        :param columns: list of columns to return, `None` for no return, `*` for all
+        :raises NotFound:
+
+        If you have composite primary keys you should pass them as tuples:
 
         .. code-block:: python
 
-            await service.get({'id': 1, 'key': 'abc'}, ...)
+            await service.get((1, 'abc'), ...)
 
-        :raises NotFound:
         """
         if columns is None:
             raise ValidationError('Null "columns" param is not allowed in a get query.')
 
         sql = self._create_get_query(id, columns)
         result = await self._wrap_get(_connection, sql)
         result = result.first()
@@ -696,32 +772,39 @@
         columns = self._sql_get_columns(columns, table=table)
         sql = table.select().with_only_columns(*columns)
         if _id:
             sql = self._list_primary_key_condition(sql, _id)
         if conditions:
             sql = self._create_conditions(sql, conditions, table)
         sql = self.get_condition_hook(sql)
-        sql = sql.limit(self.MAX_GET_QUERY_SIZE)
         return sql
 
     async def m_get(
         self, id: Collection[_Id] = None, conditions: _Condition = None, columns: _Columns = '*', _connection=None
-    ) -> list[_Row]:
+    ) -> List[_Row]:
         """Return multiple objects.
 
+        :param id: object id
+        :param conditions: filtering conditions.
+        :param columns: list of columns to return, `None` for no return, `*` for all
+        :returns: a list of objects found
+
+        .. note::
+
+            Be aware that there is a database limit on max number of ids per query (65535 in postgres).
+
         Objects that don't exist will be skipped.
         Returns all data at once without pagination. Use `SQLService.list` if
         you want pagination or sorting.
 
-        If you have composite primary keys you should pass dictionary objects
-        in id field, like this:
+        If you have composite primary keys you should pass them as tuples
 
         .. code-block:: python
 
-            await service.m_get([{'id': 1, 'key': 'abc'}, ...], ...)
+            await service.m_get([(1, 'abc'), ...], ...)
 
         """
         sql = self._create_m_get_query(id, conditions, columns)
         result = await self._wrap_get(_connection, sql)
         return [row._asdict() for row in result.all()]
 
     def _create_delete_query(self, _id: _Id, columns, table=None):
@@ -733,25 +816,28 @@
         sql = self.delete_condition_hook(sql)
         if columns:
             sql = sql.returning(*columns)
         else:
             sql = sql.returning(sa.literal_column('1'))
         return sql
 
-    async def delete(self, id: _Id, columns: _Columns = None, _connection=None) -> _Row:
+    async def delete(self, id: _Id, columns: _Columns = None, _connection=None) -> Optional[_Row]:
         """Remove a single object from a table.
 
-        If you have composite primary keys you should pass dictionary objects
-        in id field, like this:
+        :param id: object id
+        :param columns: list of columns to return, `None` for no return, `*` for all
+        :returns: a deleted object columns if requested
+        :raises NotFound: if object doesn't exist or already was deleted
+
+        If you have composite primary keys you should pass them as tuples:
 
         .. code-block:: python
 
-            await service.delete({'id': 1, 'key': 'abc'}, ...)
+            await service.delete((1, 'abc'), ...)
 
-        :raises NotFound: if object doesn't exist or already was deleted
         """
         sql = self._create_delete_query(id, columns)
         result = await self._wrap_delete(_connection, sql)
         result = result.first()
         if result is None:
             raise NotFound(
                 'Object does not exist thus it cannot be removed.',
@@ -773,34 +859,47 @@
             sql = self._create_conditions(sql, conditions, table)
         sql = self.delete_condition_hook(sql)
         sql = sql.returning(*columns)
         return sql
 
     async def m_delete(
         self, id: Collection[_Id] = None, conditions: _Condition = None, columns: _Columns = None, _connection=None
-    ) -> list[_Row]:
+    ) -> List[_Row] | None:
         """Remove multiple objects from a table. Non-existing objects will be skipped.
 
-        If you have composite primary keys you should pass dictionary objects
-        in id field, like this:
+        :param id: object ids
+        :param conditions: filtering conditions.
+        :param columns: list of columns to return, `None` for no return, `*` for all
+        :returns: a list of deleted objects if requested
+
+        If you have composite primary keys you should pass them as tuples:
 
         .. code-block:: python
 
-            await service.m_delete([{'id': 1, 'key': 'abc'}, ...], ...)
+            await service.m_delete([(1, 'abc'), ...])
+
+        You can also use conditions without primary keys if you provide an empty key list:
+
+        .. code-block:: python
+
+            await service.m_delete([], conditions={'enabled': False})
 
         """
         sql = self._create_m_delete_query(id, conditions, columns)
         result = await self._wrap_delete(_connection, sql)
         if columns:
             result = result.all()
             return [row._asdict() for row in result]
 
     @staticmethod
-    def prepare_insert_data(data: dict):
-        """Define your custom row init logic here."""
+    def prepare_insert_data(data: dict) -> _Row:
+        """Prepare data before insert.
+
+        :param data: raw data
+        """
         return data
 
     def _validate_row(self, data: dict, whitelist: frozenset):
         """Validate and prepare insert row data."""
         if not data:
             raise ValidationError(
                 'There are no columns for insert.',
@@ -845,24 +944,27 @@
         self,
         data: dict,
         columns: _Columns = '*',
         _connection=None,
         on_conflict=None,
         on_conflict_keys=None,
         on_conflict_values=None,
-    ) -> _Row:
+    ) -> Optional[_Row]:
         """Create a single object.
 
         :param data: objects data
-        :param columns: columns to return, None for no return
+        :param columns: columns to return, `None` for no return, `*` for all
         :param on_conflict: on conflict clause if required ('do_nothing', 'do_update')
         :param on_conflict_keys: list of on conflict constraints
         :param on_conflict_values: an object with on conflict values, used only by `do_update` clause
         :param _connection: optional connection object (when using inside a transactional block)
-        :returns: inserted object
+        :returns: inserted object if requested
+
+        Customize :py:meth:`~kaiju_db.services.SQLService.prepare_insert_data` to normalize and prepare data
+        before insert if you want more control over inserted data.
         """
         sql = self._create_insert_query(
             data,
             columns,
             on_conflict=on_conflict,
             on_conflict_keys=on_conflict_keys,
             on_conflict_values=on_conflict_values,
@@ -889,62 +991,77 @@
         self,
         data: Collection[dict],
         columns: _Columns = '*',
         _connection=None,
         on_conflict: str = None,
         on_conflict_keys: list = None,
         on_conflict_values: dict = None,
-    ) -> list[_Row]:
+    ) -> List[_Row] | None:
         """Create multiple objects.
 
         :param data: list of objects data
-        :param columns: columns to return, None for no return
+        :param columns: columns to return, `None` for no return, `*` for all
         :param on_conflict: on conflict clause if required ('do_nothing', 'do_update')
         :param on_conflict_keys: list of on conflict constraints
         :param on_conflict_values: an object with on conflict values, used only by `do_update` clause
         :param _connection: optional connection object (when using inside a transactional block)
-        :returns: inserted objects
+        :returns: inserted objects if requested
+
+        Customize :py:meth:`~kaiju_db.services.SQLService.prepare_insert_data` to normalize and prepare data
+        before insert if you want more control over inserted data.
         """
         sql = self._create_m_insert_query(
             data,
             columns,
             on_conflict=on_conflict,
             on_conflict_keys=on_conflict_keys,
             on_conflict_values=on_conflict_values,
         )
         result = await self._wrap_insert(_connection, sql)
         if columns:
             return [row._asdict() for row in result.all()]
 
     @staticmethod
     def prepare_update_data(data: dict):
-        """You may define your custom row update logic here."""
+        """Prepare data before update.
+
+        :param data: raw data
+        """
         return data
 
     def _create_update_query(self, _id: _Id, data: dict, columns, table=None):
         if table is None:
             table = self.table
         columns = self._sql_get_columns(columns, table=table)
         self._validate_row(data, whitelist=self.update_columns)
         data = self.prepare_update_data(data)
         sql = table.update().values(data)
         sql = self._primary_key_condition(sql, _id)
         sql = self.update_condition_hook(sql)
         sql = sql.returning(*columns) if columns else sql.returning(sa.literal_column('1'))
         return sql
 
-    async def update(self, id: _Id, data: dict, columns: _Columns = '*', _connection=None) -> _Row:
+    async def update(self, id: _Id, data: dict, columns: _Columns = '*', _connection=None) -> Optional[_Row]:
         """Update a single object. Raises error if object doesn't exist.
 
-        If you have composite primary keys you should pass dictionary objects
-        in id field, like this:
+        :param id: object id
+        :param data: data to update
+        :param columns: columns to return, `None` for no return, `*` for all
+        :param _connection: optional connection object (when using inside a transactional block)
+        :returns: inserted object if requested
+        :raises NotFound:
+
+        Customize :py:meth:`~kaiju_db.services.SQLService.prepare_update_data`
+        to normalize and prepare data before update if you want more control over updated data.
+
+        Use tuples for composite keys:
 
         .. code-block:: python
 
-            await service.update({'id': 1, 'key': 'abc'}, ...)
+            await service.update((1, 'abc'), ...)
 
         """
         sql = self._create_update_query(id, data, columns)
         result = await self._wrap_update(_connection, sql)
         result = result.first()
         if not result:
             raise NotFound(
@@ -969,23 +1086,38 @@
             sql = self._create_conditions(sql, conditions, table)
         sql = self.update_condition_hook(sql)
         sql = sql.returning(*columns)
         return sql
 
     async def m_update(
         self, id: Collection[_Id], data: dict, conditions: _Condition = None, columns: _Columns = '*', _connection=None
-    ) -> list[_Row]:
+    ) -> List[_Row] | None:
         """Update multiple objects with the same data. Non-existing objects will be skipped.
 
-        If you have composite primary keys you should pass dictionary objects
-        in id field, like this:
+        :param id: list of ids
+        :param data: update data
+        :param columns: columns to return, `None` for no return, `*` for all
+        :param conditions: update conditions
+        :param _connection: optional connection object (when using inside a transactional block)
+        :returns: inserted objects if requested
+
+        Customize :py:meth:`~kaiju_db.services.SQLService.prepare_update_data`
+        to normalize and prepare data before update if you want more control over updated data.
+
+        Use tuples for composite keys:
 
         .. code-block:: python
 
-            await service.m_update([{'id': 1, 'key': 'abc'}, ...], ...)
+            await service.m_update([(1, 'abc'), ...], ...)
+
+        You can also use conditions without primary keys if you provide an empty key list:
+
+        .. code-block:: python
+
+            await service.m_update([], data={'value': 42}, conditions={'enabled': True})
 
         """
         sql = self._create_m_update_query(id, data, conditions, columns)
         result = await self._wrap_update(_connection, sql)
         if columns:
             return [row._asdict() for row in result.all()]
 
@@ -1196,15 +1328,15 @@
         """List rows with pagination and conditions.
 
         :param conditions: optional query conditions
         :param sort: optional row ordering
         :param offset: optional row offset
         :param limit: optional row limit
         :param count: calculate page count
-        :param columns: columns to return
+        :param columns: columns to return, `None` for nothing (count only), `*` for all columns
         :param _connection: optional connection object (when using inside a transactional block)
         :returns: This method may return different data depending on the provided params
 
         Condition example:
 
         .. code-block:: python
 
@@ -1307,20 +1439,36 @@
         sort: _Sort = None,
         offset: int = 0,
         limit: int = DEFAULT_ROW_LIMIT,
         columns: _Columns = '*',
     ) -> AsyncGenerator[List[_Row], None]:
         """Iterate over listed data.
 
-        Almost the same as `SQLService.list` but returns a generator which iterates
-        over the query content. It's not intended to be used by a client
-        but inside the app or the service itself.
+        :param conditions: optional query conditions
+        :param sort: optional row ordering
+        :param offset: optional row offset
+        :param limit: optional row limit
+        :param columns: columns to return, `*` for all columns
+        :returns: This method may return different data depending on the provided params
+
+        Same as :py:meth:`~kaiju_db.services.SQLService.list` except it provides an async generator over all selected
+        data. At each iteration a batch with max size of `limit` is returned. You can use this method to
+        asynchronously iterate over selected table data in chunks.
+
+        .. code-block:: python
+
+            async for batch in sql_service.iter(conditions={'enabled': True}, sort=['created'], limit=100):
+                for row in batch:
+                    ... # batches of max 100 rows will be returned
+            # the generator will exit after when last batch of data has been returned
 
-        See `SQLService.list` for info about params.
         """
+        if not columns:
+            return
+
         if not sort:
             sort = self._primary_key_list
 
         result = await self.list(
             conditions=conditions, sort=sort, offset=offset, limit=limit, columns=columns, count=True
         )
 
@@ -1338,14 +1486,26 @@
             page += 1
 
 
 class FixtureService(ContextableService):
     """Fixture service.
 
     It can load data from json files using SQLService interface.
+
+    How to set up automatic fixtures:
+
+    1. Add FixtureService to your app configuration.
+    2. Create your sql service.
+    3. Create a .json file inside `FixtureService.root_dir` location with the name matching your sql service
+        public name, i.e. `your_service.service_name`.
+    4. Write an array of json objects into the file with object attributes same as your service expects
+        in `m_create` method.
+
+    Upon the app start the fixture service will automatically create data from fixture files *if there is no data
+    currently in respective tables*.
     """
 
     def __init__(
         self,
         app,
         root_dir: str = './fixtures/sql',
         fixtures: Collection[str] = None,
@@ -1356,39 +1516,39 @@
         """Initialize.
 
         :param app: web app
         :param root_dir: fixtures base dir
         :param fixtures: list of fixtures (service names) to load, None - load all
         :param empty_tables_only: load only when the service table is empty
         :param load_on_init: load all fixtures on service init (when starting the app)
-        :param logger: parent logger instance
+        :param logger: optional logger instance
         """
         super().__init__(app=app, logger=logger)
         self.root_dir = Path(root_dir).resolve()
         self.fixtures = fixtures
         self.empty_tables_only = empty_tables_only
         self.load_on_init = load_on_init
 
     async def init(self):
         if not self.root_dir.exists():
             self.logger.warning('Fixture path does not exist', root_dir=str(self.root_dir))
         if self.load_on_init:
             await self.load_all()
 
     async def load_all(self) -> None:
-        """Load all fixtures in the root dir."""
+        """Load all fixtures from the root dir."""
         for path in self.root_dir.rglob('*.json'):
             if self.fixtures and path.stem not in self.fixtures:
                 continue
             await self.load_fixture(path)
 
     async def load_fixture(self, path: Path) -> None:
-        """Load a single service fixture.
+        """Load a particular fixture.
 
-        A file must be a JSON list with rows of data.
+        :param path: fixture path, must contain a json array of objects
         """
         service_name = path.stem
 
         if service_name not in self.app.services:
             self.logger.debug('Cannot load fixture: no such service', fixture=service_name)
             return
 
@@ -1416,22 +1576,31 @@
     async def _table_not_empty(self, service_name: str) -> bool:
         service = cast(SQLService, self.app.services[service_name])
         data = await service.list(limit=1, count=False)
         return bool(data['data'])
 
 
 class DatabaseMigrationService(ContextableService):
-    """Simple migration tool."""
+    """Simple migration tool.
 
-    class State(TypedDict, total=False):
-        """Migration state as in the migrations json file."""
+    This service does not resolve migration issues leaving them for the developer. You should create an appropriate
+    SQL queries yourself before migration. The only thing what this service does is maintains the database state
+    and performs listed migration instructions from a pre-configured list of migrations.
+    The service uses `db_info` table to store its current state.
+
+    How to set up migrations:
+
+    1. Add `DatabaseMigrationService` to your configuration file.
+    2. Create `DatabaseMigrationService.migrations_file` which must be a json array of migration state objects.
+    3. When a migration is required you should write a new migration state into a json array,
+       see :py:class:`~kaiju_db.types.MigrationState` for example. Note that `id` must be an incremental integer
+       starting from 0.
 
-        id: int  #: identifier
-        comments: str  #: commit SHA
-        commands: list[str]  #: command or a set of commands to perform
+    Once the app has started, the migration service will automatically perform all the migrations.
+    """
 
     table = sa.Table('db_info', sa.MetaData(), sa.Column('key', sa.TEXT), sa.Column('value', sa_pg.JSONB))
     _state_key = 'state'
     _null_state = -1
 
     def __init__(
         self,
@@ -1464,39 +1633,23 @@
         self._locks = self.discover_service(self._locks, cls=Locks)
         if self._migrate_on_start:
             await self.migrate()
 
     async def migrate(self, from_: int = None, to_: int = None, migrations_file: str = None) -> int:
         """Migrate DB from one state to another.
 
-        Migration file is expected to be a json file with a number of sorted states containing state id and a list of
-        sequential SQL commands. State ids must start from 0.
-
-        .. code-block:: json
-
-            [
-                {
-                    "id": 0,
-                    "comments": "dev comments",
-                    "commands": [
-                        "ALTER TABLE my_table ADD COLUMN new_col DEFAULT NULL;",
-                        "ALTER TABLE my_table DROP COLUMN old_col;",
-                    ]
-                }
-            ]
-
         :param from_: state to migrate from (by default the current state is used)
         :param to_: state to migrate to (by default the last state is used)
         :param migrations_file: optional migrations file path
         :return: current state id
         """
         if migrations_file is None:
             migrations_file = self._migrations_file
         with open(migrations_file) as f:
-            migrations: list[DatabaseMigrationService.State] = load(f)
+            migrations: List[MigrationState] = load(f)
         if not migrations:
             return self._null_state
         identifier = await self._locks.acquire(self._lock_key)  # TODO: lock context
         try:
             state_id = await self.get_state()
             self.logger.debug('Current state: #%d.', state_id)
             if from_ is None:
@@ -1536,15 +1689,15 @@
             state_id = self._null_state
         else:
             state_id = state['value']
         return state_id
 
 
 class PermHook(PublicInterface, abc.ABC):
-    """Sql service with a user permissions hook.
+    """Sql service with a pre-configured user permissions hook.
 
     it uses 'user_id' column by default to check if objects can be edited or viewed by users.
     You should modify `_set_user_condition()` if you intend to use different columns.
     """
 
     service_name: str
     table: sa.Table
@@ -1571,26 +1724,26 @@
         """Get a view permission key."""
         return f'{self.service_name}.{self.Permission.VIEW_OTHERS.value}'
 
     def _set_user_condition(self, sql, permission: str):
         """Place user condition."""
         if not self.has_permission(permission):
             user_id = self.get_user_id()
-            sql = sql.where(self.table.c.user_id == user_id)
+            sql = sql.where(sa.and_(self.table.c.user_id == user_id, self.table.c.user_id.is_not(None)))
         return sql
 
-    def _update_condition_hook(self, sql):
+    def update_condition_hook(self, sql):
         """Place user condition on update operations."""
         return self._set_user_condition(sql, self.permission_modify)
 
-    def _delete_condition_hook(self, sql):
+    def delete_condition_hook(self, sql):
         """Place user condition on delete operations."""
-        return self._update_condition_hook(sql)
+        return self.update_condition_hook(sql)
 
-    def _get_condition_hook(self, sql):
+    def get_condition_hook(self, sql):
         """Place user condition on get and list operations."""
         return self._set_user_condition(sql, self.permission_view)
 
 
 SERVICE_CLASS_REGISTRY.register(DatabaseService)
 SERVICE_CLASS_REGISTRY.register(DatabaseMigrationService)
 SERVICE_CLASS_REGISTRY.register(FixtureService)
```

## kaiju_db/types.py

```diff
@@ -1,12 +1,40 @@
-import sqlalchemy.types as types
+"""Postgres data types."""
+
+from typing import TypedDict
+
 import sqlalchemy.dialects.postgresql as sa_pg
+import sqlalchemy.types as types
 from sqlalchemy_utils import Ltree as PGLtree
 
-__all__ = ['CITEXT', 'Ltree']
+
+__all__ = ['CITEXT', 'Ltree', 'MigrationState']
+
+
+class MigrationState(TypedDict):
+    """Migration service migration.
+
+    This data format is used by migration services to perform migrations. See an example below.
+
+    .. code-block:: python
+
+        {
+            "id": 0,
+            "comments": "dev comments",
+            "commands": [
+                "ALTER TABLE my_table ADD COLUMN new_col DEFAULT NULL;",
+                "ALTER TABLE my_table DROP COLUMN old_col;",
+            ]
+        }
+
+    """
+
+    id: int  #: state id, sequential integer >= 0
+    comments: str  #: human readable comments
+    commands: list[str]  #: a list of sql commands performed inside a transaction block
 
 
 class CITEXT(types.UserDefinedType, sa_pg.TEXT):
     """Postgres case-insensitive text data type."""
 
     def get_col_spec(self):  # noqa: required
         return 'CITEXT'
```

## kaiju_db/tests/test_db.py

```diff
@@ -4,15 +4,16 @@
 import pytest_asyncio
 import sqlalchemy as sa
 import sqlalchemy.dialects.postgresql as sa_pg
 
 from kaiju_tools.encoding import dumps
 from kaiju_tools.tests.test_data_store import TestDataStore
 
-from kaiju_db.services import SQLService, DatabaseMigrationService
+from kaiju_db.services import SQLService
+from kaiju_db.types import MigrationState
 
 __all__ = ['TestDatabaseService', 'TestMigrationService', 'TestSQLService', 'TestSQLServiceCompKey']
 
 
 @pytest.mark.asyncio
 @pytest.mark.docker
 class TestDatabaseService:
@@ -51,22 +52,22 @@
     """Test migrations."""
 
     @pytest.fixture
     def _migrations_file(self, migrations_file, test_table):
         migrations_file.write_text(
             dumps(
                 [
-                    DatabaseMigrationService.State(
+                    MigrationState(
                         id=0,
                         commands=[
                             'CREATE SEQUENCE test;',
                             f'ALTER TABLE {test_table.name} ADD COLUMN new_column INT DEFAULT 42;',
                         ],
                     ),
-                    DatabaseMigrationService.State(
+                    MigrationState(
                         id=1, commands=[f'ALTER TABLE {test_table.name} ADD COLUMN new_column_2 BOOLEAN DEFAULT TRUE;']
                     ),
                 ]
             ).decode('utf-8')
         )
         return migrations_file
```

## Comparing `kaiju_db-2.1.8.dist-info/LICENSE` & `kaiju_db-2.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kaiju_db-2.1.8.dist-info/METADATA` & `kaiju_db-2.1.9.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,83 +1,77 @@
 Metadata-Version: 2.1
 Name: kaiju-db
-Version: 2.1.8
+Version: 2.1.9
 Summary: Postgresql db services and tools
 Home-page: https://gitlab.com/kaiju-python/kaiju-db
 Author: antonnidhoggr@me.com
 Author-email: antonnidhoggr@me.com
 License: Apache Software License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: asyncpg (>=0.28)
-Requires-Dist: greenlet (>=2.0.2)
-Requires-Dist: sqlalchemy[asyncio] (>=2.0.19)
-Requires-Dist: sqlalchemy-utils (>=0.41)
-Requires-Dist: kaiju-tools (<3,>=2)
+Requires-Dist: asyncpg >=0.29
+Requires-Dist: greenlet >=3.0.1
+Requires-Dist: sqlalchemy[asyncio] >=2.0.23
+Requires-Dist: sqlalchemy-utils >=0.41
+Requires-Dist: kaiju-tools <3,>=2
 Provides-Extra: dev
-Requires-Dist: bump2version (>=1.0) ; extra == 'dev'
-Requires-Dist: pyroma (>=4.1) ; extra == 'dev'
-Requires-Dist: bandit (>=1.7) ; extra == 'dev'
-Requires-Dist: black (>=22.12) ; extra == 'dev'
-Requires-Dist: flake8 (>=6.0) ; extra == 'dev'
-Requires-Dist: flake8-walrus (>=1.2.0) ; extra == 'dev'
-Requires-Dist: pyproject-flake8 ; extra == 'dev'
-Requires-Dist: pre-commit (>=3.1) ; extra == 'dev'
-Requires-Dist: pydocstyle (>=6.3) ; extra == 'dev'
-Requires-Dist: setup-cfg-fmt (>=2.2) ; extra == 'dev'
-Requires-Dist: restructuredtext-lint (>=1.4) ; extra == 'dev'
-Requires-Dist: tox (>=3.28) ; extra == 'dev'
-Requires-Dist: tox-pyenv (>=1.1) ; extra == 'dev'
-Requires-Dist: pip-tools (>=6.13) ; extra == 'dev'
-Requires-Dist: pyupgrade (>=3.4) ; extra == 'dev'
-Requires-Dist: towncrier (>=23.6) ; extra == 'dev'
-Requires-Dist: isort (>=5.12.0) ; extra == 'dev'
-Requires-Dist: xenon (>=0.9.0) ; extra == 'dev'
+Requires-Dist: bump2version >=1.0 ; extra == 'dev'
+Requires-Dist: pyroma >=4.1 ; extra == 'dev'
+Requires-Dist: bandit >=1.7 ; extra == 'dev'
+Requires-Dist: black >=23.11 ; extra == 'dev'
+Requires-Dist: flake8 >=6.1 ; extra == 'dev'
+Requires-Dist: flake8-walrus >=1.2 ; extra == 'dev'
+Requires-Dist: pyproject-flake8 >=6.1 ; extra == 'dev'
+Requires-Dist: pre-commit >=3.5 ; extra == 'dev'
+Requires-Dist: pydocstyle >=6.3 ; extra == 'dev'
+Requires-Dist: setup-cfg-fmt >=2.5 ; extra == 'dev'
+Requires-Dist: restructuredtext-lint >=1.4 ; extra == 'dev'
+Requires-Dist: tox >=4.11 ; extra == 'dev'
+Requires-Dist: virtualenv-pyenv >=0.4 ; extra == 'dev'
+Requires-Dist: pip-tools >=7.3 ; extra == 'dev'
+Requires-Dist: pyupgrade >=3.15 ; extra == 'dev'
+Requires-Dist: towncrier >=23.11 ; extra == 'dev'
+Requires-Dist: isort >=5.12.0 ; extra == 'dev'
+Requires-Dist: xenon >=0.9.1 ; extra == 'dev'
+Provides-Extra: docker
+Requires-Dist: docker >=6.1.3 ; extra == 'docker'
 Provides-Extra: docs
 Requires-Dist: sphinx ; extra == 'docs'
 Requires-Dist: python-docs-theme ; extra == 'docs'
 Provides-Extra: test
-Requires-Dist: pytest (>=7.4) ; extra == 'test'
-Requires-Dist: pytest-asyncio (>=0.21) ; extra == 'test'
-Requires-Dist: docker (>=6.1.3) ; extra == 'test'
-Requires-Dist: pytest-timeout (>=2.1) ; extra == 'test'
-Requires-Dist: pytest-aiohttp (>=1.0.4) ; extra == 'test'
-Requires-Dist: pytest-cov (>=4.1.0) ; extra == 'test'
+Requires-Dist: pytest >=7.4 ; extra == 'test'
+Requires-Dist: pytest-asyncio >=0.21 ; extra == 'test'
+Requires-Dist: docker >=6.1.3 ; extra == 'test'
+Requires-Dist: pytest-timeout >=2.1 ; extra == 'test'
+Requires-Dist: pytest-aiohttp >=1.0.5 ; extra == 'test'
+Requires-Dist: pytest-cov >=4.1.0 ; extra == 'test'
 
 
 .. image:: https://badge.fury.io/py/kaiju-db.svg
     :target: https://pypi.org/project/kaiju-db
     :alt: Latest package version
 
-.. image:: https://readthedocs.org/projects/kaiju-db/badge/?version=latest
-    :target: https://kaiju-db.readthedocs.io/en/latest/?badge=latest
-    :alt: Documentation Status
-
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style - Black
 
-Summary
--------
-
-**Python** >=3.11
-**Postgresql** >= 14
+`Python <https://www.python.org>`_ >=3.11 `Postgres <https://www.postgresql.org>`_ >=14
 
-`Project documentation <https://kaiju-db.readthedocs.io/en/latest/>`_
+Database connector services, database initialization, fixtures initialization, migrations.
+Interfaces for remote interaction with tables via RPC.
+See `documentation <https://kaiju-db.readthedocs.io/>`_ for more info.
 
-System and user tasks management classes.
-They are used to schedule and execute sets of RPC commands across applications.
+Installation
+------------
 
-Use `pip install kaiju-db` to install the package.
+.. code-block:: console
 
-For development run the init script `tools/init.sh`.
-It will setup git hooks and install the dev version of the project.
+  pip install kaiju-db
 
-See `developer guide <https://kaiju-db.readthedocs.io/en/latest/#developer-guide>`_ for details.
+You need a `kaiju application <https://gitlab.com/kaiju-python/kaiju-base-app>`_ to run these services.
```

