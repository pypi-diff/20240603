# Comparing `tmp/sqlitecloud-0.0.77.tar.gz` & `tmp/sqlitecloud-0.0.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlitecloud-0.0.77.tar", last modified: Fri May 24 18:01:42 2024, max compression
+gzip compressed data, was "sqlitecloud-0.0.78.tar", last modified: Mon Jun  3 08:58:57 2024, max compression
```

## Comparing `sqlitecloud-0.0.77.tar` & `sqlitecloud-0.0.78.tar`

### file list

```diff
@@ -1,31 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:01:42.644730 sqlitecloud-0.0.77/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-24 18:01:36.000000 sqlitecloud-0.0.77/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-24 18:01:42.644730 sqlitecloud-0.0.77/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-24 18:01:39.000000 sqlitecloud-0.0.77/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:01:42.644730 sqlitecloud-0.0.77/SqliteCloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-24 18:01:42.000000 sqlitecloud-0.0.77/SqliteCloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-24 18:01:42.000000 sqlitecloud-0.0.77/SqliteCloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 18:01:42.000000 sqlitecloud-0.0.77/SqliteCloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-24 18:01:42.000000 sqlitecloud-0.0.77/SqliteCloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-24 18:01:42.000000 sqlitecloud-0.0.77/SqliteCloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 18:01:42.644730 sqlitecloud-0.0.77/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-24 18:01:39.000000 sqlitecloud-0.0.77/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:01:42.644730 sqlitecloud-0.0.77/sqlitecloud/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-24 18:01:36.000000 sqlitecloud-0.0.77/sqlitecloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-05-24 18:01:36.000000 sqlitecloud-0.0.77/sqlitecloud/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-24 18:01:36.000000 sqlitecloud-0.0.77/sqlitecloud/download.py
--rw-r--r--   0 runner    (1001) docker     (127)    33631 2024-05-24 18:01:36.000000 sqlitecloud-0.0.77/sqlitecloud/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-24 18:01:36.000000 sqlitecloud-0.0.77/sqlitecloud/pubsub.py
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-05-24 18:01:36.000000 sqlitecloud-0.0.77/sqlitecloud/resultset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-05-24 18:01:36.000000 sqlitecloud-0.0.77/sqlitecloud/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-24 18:01:36.000000 sqlitecloud-0.0.77/sqlitecloud/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:01:42.644730 sqlitecloud-0.0.77/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 18:01:36.000000 sqlitecloud-0.0.77/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-24 18:01:36.000000 sqlitecloud-0.0.77/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:01:42.644730 sqlitecloud-0.0.77/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 18:01:36.000000 sqlitecloud-0.0.77/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23369 2024-05-24 18:01:36.000000 sqlitecloud-0.0.77/tests/integration/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-24 18:01:36.000000 sqlitecloud-0.0.77/tests/integration/test_download.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-24 18:01:36.000000 sqlitecloud-0.0.77/tests/integration/test_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     5373 2024-05-24 18:01:36.000000 sqlitecloud-0.0.77/tests/integration/test_pubsub.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-24 18:01:36.000000 sqlitecloud-0.0.77/tests/integration/test_upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:58:57.464968 sqlitecloud-0.0.78/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-06-03 08:58:52.000000 sqlitecloud-0.0.78/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5770 2024-06-03 08:58:57.464968 sqlitecloud-0.0.78/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4987 2024-06-03 08:58:54.000000 sqlitecloud-0.0.78/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 08:58:57.464968 sqlitecloud-0.0.78/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-06-03 08:58:54.000000 sqlitecloud-0.0.78/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:58:57.464968 sqlitecloud-0.0.78/sqlitecloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-06-03 08:58:52.000000 sqlitecloud-0.0.78/sqlitecloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-06-03 08:58:52.000000 sqlitecloud-0.0.78/sqlitecloud/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14727 2024-06-03 08:58:52.000000 sqlitecloud-0.0.78/sqlitecloud/dbapi2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-06-03 08:58:52.000000 sqlitecloud-0.0.78/sqlitecloud/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36553 2024-06-03 08:58:52.000000 sqlitecloud-0.0.78/sqlitecloud/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-06-03 08:58:52.000000 sqlitecloud-0.0.78/sqlitecloud/pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-06-03 08:58:52.000000 sqlitecloud-0.0.78/sqlitecloud/resultset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7503 2024-06-03 08:58:52.000000 sqlitecloud-0.0.78/sqlitecloud/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-06-03 08:58:52.000000 sqlitecloud-0.0.78/sqlitecloud/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:58:57.464968 sqlitecloud-0.0.78/sqlitecloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5770 2024-06-03 08:58:57.000000 sqlitecloud-0.0.78/sqlitecloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-06-03 08:58:57.000000 sqlitecloud-0.0.78/sqlitecloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 08:58:57.000000 sqlitecloud-0.0.78/sqlitecloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-06-03 08:58:57.000000 sqlitecloud-0.0.78/sqlitecloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-03 08:58:57.000000 sqlitecloud-0.0.78/sqlitecloud.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:58:57.464968 sqlitecloud-0.0.78/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 08:58:52.000000 sqlitecloud-0.0.78/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-06-03 08:58:52.000000 sqlitecloud-0.0.78/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:58:57.464968 sqlitecloud-0.0.78/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 08:58:52.000000 sqlitecloud-0.0.78/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24365 2024-06-03 08:58:52.000000 sqlitecloud-0.0.78/tests/integration/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7828 2024-06-03 08:58:52.000000 sqlitecloud-0.0.78/tests/integration/test_dbapi2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-06-03 08:58:52.000000 sqlitecloud-0.0.78/tests/integration/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-06-03 08:58:52.000000 sqlitecloud-0.0.78/tests/integration/test_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-06-03 08:58:52.000000 sqlitecloud-0.0.78/tests/integration/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-06-03 08:58:52.000000 sqlitecloud-0.0.78/tests/integration/test_pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-06-03 08:58:52.000000 sqlitecloud-0.0.78/tests/integration/test_sqlite3_parity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-06-03 08:58:52.000000 sqlitecloud-0.0.78/tests/integration/test_upload.py
```

### Comparing `sqlitecloud-0.0.77/setup.py` & `sqlitecloud-0.0.78/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 from setuptools import find_packages, setup
 
 # read the contents of your README file
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 setup(
-    name="SqliteCloud",
-    version="0.0.77",
+    name="sqlitecloud",
+    version="0.0.78",
     author="sqlitecloud.io",
     description="A Python package for working with SQLite databases in the cloud.",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/sqlitecloud/python",
+    url="https://github.com/sqlitecloud/sqlitecloud-py",
     packages=find_packages(),
     install_requires=[
         "lz4 >= 3.1.10",
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
```

### Comparing `sqlitecloud-0.0.77/sqlitecloud/client.py` & `sqlitecloud-0.0.78/sqlitecloud/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,157 +1,137 @@
 """ Module to interact with remote SqliteCloud database
 
 """
-from typing import Optional
-from urllib import parse
+from typing import Dict, Optional, Tuple, Union
 
 from sqlitecloud.driver import Driver
-from sqlitecloud.resultset import SqliteCloudResultSet
+from sqlitecloud.resultset import SQLiteCloudResultSet
 from sqlitecloud.types import (
-    SQCLOUD_DEFAULT,
-    SQCloudConfig,
-    SQCloudConnect,
-    SQCloudException,
-    SqliteCloudAccount,
+    SQLiteCloudAccount,
+    SQLiteCloudConfig,
+    SQLiteCloudConnect,
+    SQLiteCloudDataTypes,
+    SQLiteCloudException,
 )
 
 
-class SqliteCloudClient:
+class SQLiteCloudClient:
     """
     Client to interact with Sqlite Cloud
     """
 
     def __init__(
         self,
-        cloud_account: Optional[SqliteCloudAccount] = None,
+        cloud_account: Optional[SQLiteCloudAccount] = None,
         connection_str: Optional[str] = None,
     ) -> None:
         """Initializes a new instance of the class with connection information.
 
         Args:
             cloud_account (SqliteCloudAccount): The account information for the
                 SQlite Cloud database.
             connection_str (str): The connection string for the SQlite Cloud database.
                 Eg: sqlitecloud://user:pass@host.com:port/dbname?timeout=10&apikey=abcd123
 
         """
         self._driver = Driver()
 
-        self.config = SQCloudConfig()
+        self.config = SQLiteCloudConfig()
 
         if connection_str:
-            self.config = self._parse_connection_string(connection_str)
+            self.config = SQLiteCloudConfig(connection_str)
         elif cloud_account:
             self.config.account = cloud_account
-        else:
-            raise SQCloudException("Missing connection parameters")
 
-    def open_connection(self) -> SQCloudConnect:
-        """Opens a connection to the SQCloud server.
+        if self.config.account is None:
+            raise SQLiteCloudException("Missing connection parameters")
+
+    def open_connection(self) -> SQLiteCloudConnect:
+        """Opens a connection to the SQLite Cloud server.
 
         Returns:
-            SQCloudConnect: An instance of the SQCloudConnect class representing
-                the connection to the SQCloud server.
+            SQLiteCloudConnect: An instance of the SQLiteCloudConnect class representing
+                the connection to the SQLite Cloud server.
 
         Raises:
-            SQCloudException: If an error occurs while opening the connection.
+            SQLiteCloudException: If an error occurs while opening the connection.
         """
         connection = self._driver.connect(
             self.config.account.hostname, self.config.account.port, self.config
         )
 
         return connection
 
-    def disconnect(self, conn: SQCloudConnect) -> None:
+    def disconnect(self, conn: SQLiteCloudConnect) -> None:
         """Close the connection to the database."""
         self._driver.disconnect(conn)
 
-    def is_connected(self, conn: SQCloudConnect) -> bool:
+    def is_connected(self, conn: SQLiteCloudConnect) -> bool:
         """Check if the connection is still open.
 
         Args:
-            conn (SQCloudConnect): The connection to the database.
+            conn (SQLiteCloudConnect): The connection to the database.
 
         Returns:
             bool: True if the connection is open, False otherwise.
         """
         return self._driver.is_connected(conn)
 
-    def exec_query(self, query: str, conn: SQCloudConnect) -> SqliteCloudResultSet:
+    def exec_query(self, query: str, conn: SQLiteCloudConnect) -> SQLiteCloudResultSet:
         """Executes a SQL query on the SQLite Cloud database.
 
         Args:
-            query (str): The SQL query to be executed.
+            query (str): The SQL query to execute.
 
         Returns:
             SqliteCloudResultSet: The result set of the executed query.
 
         Raises:
-            SQCloudException: If an error occurs while executing the query.
+            SQLiteCloudException: If an error occurs while executing the query.
         """
         result = self._driver.execute(query, conn)
 
-        return SqliteCloudResultSet(result)
+        return SQLiteCloudResultSet(result)
+
+    def exec_statement(
+        self,
+        query: str,
+        parameters: Union[
+            Tuple[SQLiteCloudDataTypes], Dict[Union[str, int], SQLiteCloudDataTypes]
+        ],
+        conn: SQLiteCloudConnect,
+    ) -> SQLiteCloudResultSet:
+        """
+        Prepare and execute a SQL statement (either a query or command) to the SQLite Cloud database.
+        This function supports two styles of parameter markers:
+
+        1. Question Mark Style: Parameters are passed as a tuple. For example:
+        "SELECT * FROM table WHERE id = ?"
+
+        2. Named Style: Parameters are passed as a dictionary. For example:
+        "SELECT * FROM table WHERE id = :id"
 
-    def sendblob(self, blob: bytes, conn: SQCloudConnect) -> SqliteCloudResultSet:
+        In both cases, the parameters replace the placeholders in the SQL statement.
+
+        Args:
+            query (str): The SQL query to execute.
+            parameters (Union[Tuple[SQLiteCloudDataTypes], Dict[Union[str, int], SQLiteCloudDataTypes]]):
+                The parameters to be used in the query. It can be a tuple or a dictionary.
+            conn (SQLiteCloudConnect): The connection object to use for executing the query.
+
+        Returns:
+            SqliteCloudResultSet: The result set obtained from executing the query.
+        """
+        prepared_statement = self._driver.prepare_statement(query, parameters)
+
+        result = self._driver.execute(prepared_statement, conn)
+
+        return SQLiteCloudResultSet(result)
+
+    def sendblob(self, blob: bytes, conn: SQLiteCloudConnect) -> SQLiteCloudResultSet:
         """Sends a blob to the SQLite database.
 
         Args:
             blob (bytes): The blob to be sent to the database.
-            conn (SQCloudConnect): The connection to the database.
+            conn (SQLiteCloudConnect): The connection to the database.
         """
         return self._driver.send_blob(blob, conn)
-
-    def _parse_connection_string(self, connection_string) -> SQCloudConfig:
-        # URL STRING FORMAT
-        # sqlitecloud://user:pass@host.com:port/dbname?timeout=10&key2=value2&key3=value3
-        # or sqlitecloud://host.sqlite.cloud:8860/dbname?apikey=zIiAARzKm9XBVllbAzkB1wqrgijJ3Gx0X5z1A4m4xBA
-
-        config = SQCloudConfig()
-        config.account = SqliteCloudAccount()
-
-        try:
-            params = parse.urlparse(connection_string)
-
-            options = {}
-            query = params.query
-            options = parse.parse_qs(query)
-            for option, values in options.items():
-                opt = option.lower()
-                value = values.pop()
-
-                if value.lower() in ["true", "false"]:
-                    value = bool(value)
-                elif value.isdigit():
-                    value = int(value)
-                else:
-                    value = value
-
-                if hasattr(config, opt):
-                    setattr(config, opt, value)
-                elif hasattr(config.account, opt):
-                    setattr(config.account, opt, value)
-
-            # apikey or username/password is accepted
-            if not config.account.apikey:
-                config.account.username = (
-                    parse.unquote(params.username) if params.username else ""
-                )
-                config.account.password = (
-                    parse.unquote(params.password) if params.password else ""
-                )
-
-            path = params.path
-            database = path.strip("/")
-            if database:
-                config.account.dbname = database
-
-            config.account.hostname = params.hostname
-            config.account.port = (
-                int(params.port) if params.port else SQCLOUD_DEFAULT.PORT.value
-            )
-
-            return config
-        except Exception as e:
-            raise SQCloudException(
-                f"Invalid connection string {connection_string}"
-            ) from e
```

### Comparing `sqlitecloud-0.0.77/sqlitecloud/download.py` & `sqlitecloud-0.0.78/sqlitecloud/download.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from io import BufferedWriter
 
 from sqlitecloud.driver import Driver
-from sqlitecloud.types import SQCloudConnect
+from sqlitecloud.types import SQLiteCloudConnect
 
 
 def xCallback(
     fd: BufferedWriter, data: bytes, blen: int, ntot: int, nprogress: int
 ) -> None:
     """
     Callback function used for downloading data.
@@ -24,18 +24,18 @@
 
     if blen == 0:
         logging.log(logging.DEBUG, "DOWNLOAD COMPLETE")
     else:
         logging.log(logging.DEBUG, f"{(nprogress + blen) / ntot * 100:.2f}%")
 
 
-def download_db(connection: SQCloudConnect, dbname: str, filename: str) -> None:
+def download_db(connection: SQLiteCloudConnect, dbname: str, filename: str) -> None:
     """
     Download a database from the server.
 
     Raises:
-        SQCloudException: If an error occurs while downloading the database.
+        SQLiteCloudException: If an error occurs while downloading the database.
     """
     driver = Driver()
 
     with open(filename, "wb") as fd:
         driver.download_database(connection, dbname, fd, xCallback, False)
```

### Comparing `sqlitecloud-0.0.77/sqlitecloud/driver.py` & `sqlitecloud-0.0.78/sqlitecloud/driver.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,99 +1,124 @@
+import json
 import logging
 import select
 import socket
 import ssl
 import threading
 from io import BufferedReader, BufferedWriter
-from typing import Callable, Optional, Union
+from typing import Callable, Dict, Optional, Tuple, Union
 
 import lz4.block
 
-from sqlitecloud.resultset import SQCloudResult, SqliteCloudResultSet
+from sqlitecloud.resultset import SQLiteCloudResult, SQLiteCloudResultSet
 from sqlitecloud.types import (
-    SQCLOUD_CMD,
-    SQCLOUD_DEFAULT,
-    SQCLOUD_INTERNAL_ERRCODE,
-    SQCLOUD_RESULT_TYPE,
-    SQCLOUD_ROWSET,
-    SQCloudConfig,
-    SQCloudConnect,
-    SQCloudException,
-    SQCloudNumber,
-    SQCloudRowsetSignature,
-    SQCloudValue,
+    SQLITECLOUD_CMD,
+    SQLITECLOUD_DEFAULT,
+    SQLITECLOUD_INTERNAL_ERRCODE,
+    SQLITECLOUD_RESULT_TYPE,
+    SQLITECLOUD_ROWSET,
+    SQLiteCloudConfig,
+    SQLiteCloudConnect,
+    SQLiteCloudDataTypes,
+    SQLiteCloudException,
+    SQLiteCloudNumber,
+    SQLiteCloudRowsetSignature,
+    SQLiteCloudValue,
 )
 
 
 class Driver:
-    SQCLOUD_DEFAULT_UPLOAD_SIZE = 512 * 1024
+    SQLiteCloud_DEFAULT_UPLOAD_SIZE = 512 * 1024
 
     def __init__(self) -> None:
         # Used while parsing chunked rowset
-        self._rowset: SQCloudResult = None
+        self._rowset: SQLiteCloudResult = None
 
     def connect(
-        self, hostname: str, port: int, config: SQCloudConfig
-    ) -> SQCloudConnect:
+        self, hostname: str, port: int, config: SQLiteCloudConfig
+    ) -> SQLiteCloudConnect:
         """
         Connect to the SQLite Cloud server.
 
         Args:
             hostname (str): The hostname of the server.
             port (int): The port number of the server.
-            config (SQCloudConfig): The configuration for the connection.
+            config (SQLiteCloudConfig): The configuration for the connection.
 
         Returns:
-            SQCloudConnect: The connection object.
+            SQLiteCloudConnect: The connection object.
 
         Raises:
-            SQCloudException: If an error occurs while connecting the socket.
+            SQLiteCloudException: If an error occurs while connecting the socket.
         """
         sock = self._internal_connect(hostname, port, config)
 
-        connection = SQCloudConnect()
+        connection = SQLiteCloudConnect()
         connection.config = config
         connection.socket = sock
 
         self._internal_config_apply(connection, config)
 
         return connection
 
-    def disconnect(self, conn: SQCloudConnect, only_main_socket: bool = False) -> None:
+    def disconnect(
+        self, conn: SQLiteCloudConnect, only_main_socket: bool = False
+    ) -> None:
         """
         Disconnect from the SQLite Cloud server.
         """
         try:
             if conn.socket:
                 conn.socket.close()
             if not only_main_socket and conn.pubsub_socket:
                 conn.pubsub_socket.close()
         finally:
             conn.socket = None
             if not only_main_socket:
                 conn.pubsub_socket = None
 
-    def execute(self, command: str, connection: SQCloudConnect) -> SQCloudResult:
+    def execute(
+        self, command: str, connection: SQLiteCloudConnect
+    ) -> SQLiteCloudResult:
         """
         Execute a query on the SQLite Cloud server.
         """
         return self._internal_run_command(connection, command)
 
-    def send_blob(self, blob: bytes, conn: SQCloudConnect) -> SQCloudResult:
+    def send_blob(self, blob: bytes, conn: SQLiteCloudConnect) -> SQLiteCloudResult:
         """
         Send a blob to the SQLite Cloud server.
         """
         try:
             conn.isblob = True
             return self._internal_run_command(conn, blob)
         finally:
             conn.isblob = False
 
+    def prepare_statement(
+        self,
+        query: str,
+        parameters: Union[
+            Tuple[SQLiteCloudDataTypes], Dict[Union[str, int], SQLiteCloudDataTypes]
+        ],
+    ) -> str:
+        # If parameters is a dictionary, replace the keys in the query with the values
+        if isinstance(parameters, dict):
+            for key, value in parameters.items():
+                query = query.replace(":" + str(key), self.escape_sql_parameter(value))
+
+        # If parameters is a tuple, replace each '?' in the query with a value from the tuple
+        elif isinstance(parameters, tuple):
+            for value in parameters:
+                query = query.replace("?", self.escape_sql_parameter(value), 1)
+
+        return query
+
     def is_connected(
-        self, connection: SQCloudConnect, main_socket: bool = True
+        self, connection: SQLiteCloudConnect, main_socket: bool = True
     ) -> bool:
         """
         Check if the connection is still open.
         """
         sock = connection.socket if main_socket else connection.pubsub_socket
 
         if not sock:
@@ -101,16 +126,43 @@
         try:
             sock.sendall(b"")
         except OSError:
             return False
 
         return True
 
+    def escape_sql_parameter(self, param):
+        if param is None or param is None:
+            return "NULL"
+
+        if isinstance(param, bool):
+            return "1" if param else "0"
+
+        if isinstance(param, str):
+            # replace single quote with two single quotes
+            param = param.replace("'", "''")
+            return f"'{param}'"
+
+        if isinstance(param, (int, float)):
+            return str(param)
+
+        # serialize buffer as X'...' hex encoded string
+        if isinstance(param, bytes):
+            return f"X'{param.hex()}'"
+
+        if isinstance(param, dict) or isinstance(param, list):
+            # serialize json then escape single quotes
+            json_string = json.dumps(param)
+            json_string = json_string.replace("'", "''")
+            return f"'{json_string}'"
+
+        raise SQLiteCloudException(f"Unsupported parameter type: {type(param)}")
+
     def _internal_connect(
-        self, hostname: str, port: int, config: SQCloudConfig
+        self, hostname: str, port: int, config: SQLiteCloudConfig
     ) -> socket:
         """
         Create a socket connection to the SQLite Cloud server.
         """
         sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         sock.settimeout(config.connect_timeout)
         sock.setsockopt(socket.SOL_SOCKET, socket.SO_KEEPALIVE, 1)
@@ -128,31 +180,33 @@
 
             sock = context.wrap_socket(sock, server_hostname=hostname)
 
         try:
             sock.connect((hostname, port))
         except Exception as e:
             errmsg = "An error occurred while initializing the socket."
-            raise SQCloudException(errmsg) from e
+            raise SQLiteCloudException(errmsg) from e
 
         return sock
 
     def _internal_reconnect(self, buffer: bytes) -> bool:
         return True
 
-    def _internal_setup_pubsub(self, connection: SQCloudConnect, buffer: bytes) -> bool:
+    def _internal_setup_pubsub(
+        self, connection: SQLiteCloudConnect, buffer: bytes
+    ) -> bool:
         """
         Prepare the connection for PubSub.
         Opens a new specific socket and starts the thread to listen for incoming messages.
         """
         if self.is_connected(connection, False):
             return True
 
         if connection.pubsub_callback is None:
-            raise SQCloudException(
+            raise SQLiteCloudException(
                 "A callback function must be provided to setup the PubSub connection."
             )
 
         connection.pubsub_socket = self._internal_connect(
             connection.config.account.hostname,
             connection.config.account.port,
             connection.config,
@@ -165,15 +219,15 @@
         # kill the thread when the main one is terminated
         thread.daemon = True
         thread.start()
         connection.pubsub_thread = thread
 
         return True
 
-    def _internal_pubsub_thread(self, connection: SQCloudConnect) -> None:
+    def _internal_pubsub_thread(self, connection: SQLiteCloudConnect) -> None:
         blen = 2048
         buffer: bytes = b""
 
         try:
             while True:
                 tread = 0
 
@@ -195,76 +249,76 @@
 
                     data = connection.pubsub_socket.recv(blen)
                     if not data:
                         logging.info("PubSub connection closed.")
                         break
                 except Exception as e:
                     logging.error(
-                        f"An error occurred while reading data: {SQCLOUD_INTERNAL_ERRCODE.NETWORK.value} ({e})."
+                        f"An error occurred while reading data: {SQLITECLOUD_INTERNAL_ERRCODE.NETWORK.value} ({e})."
                     )
                     break
 
                 nread = len(data)
                 tread += nread
                 blen -= nread
                 buffer += data
 
-                sqcloud_number = self._internal_parse_number(buffer)
-                clen = sqcloud_number.value
+                SQLiteCloud_number = self._internal_parse_number(buffer)
+                clen = SQLiteCloud_number.value
                 if clen == 0:
                     continue
 
                 # check if read is complete
                 # clen is the lenght parsed in the buffer
                 # cstart is the index of the first space
-                cstart = sqcloud_number.cstart
+                cstart = SQLiteCloud_number.cstart
                 if clen + cstart != tread:
                     continue
 
                 result = self._internal_parse_buffer(connection, buffer, tread)
-                if result.tag == SQCLOUD_RESULT_TYPE.RESULT_STRING:
-                    result.tag = SQCLOUD_RESULT_TYPE.RESULT_JSON
+                if result.tag == SQLITECLOUD_RESULT_TYPE.RESULT_STRING:
+                    result.tag = SQLITECLOUD_RESULT_TYPE.RESULT_JSON
 
                 connection.pubsub_callback(
-                    connection, SqliteCloudResultSet(result), connection.pubsub_data
+                    connection, SQLiteCloudResultSet(result), connection.pubsub_data
                 )
         except Exception as e:
             logging.error(f"An error occurred while parsing data: {e}.")
 
         finally:
             connection.pubsub_callback(connection, None, connection.pubsub_data)
 
     def upload_database(
         self,
-        connection: SQCloudConnect,
+        connection: SQLiteCloudConnect,
         dbname: str,
         key: Optional[str],
         is_file_transfer: bool,
         snapshot_id: int,
         is_internal_db: bool,
         fd: BufferedReader,
         dbsize: int,
         xCallback: Callable[[BufferedReader, int, int, int], bytes],
     ) -> None:
         """
         Uploads a database to the server.
 
         Args:
-            connection (SQCloudConnect): The connection object to the SQLite Cloud server.
+            connection (SQLiteCloudConnect): The connection object to the SQLite Cloud server.
             dbname (str): The name of the database to upload.
             key (Optional[str]): The encryption key for the database, if applicable.
             is_file_transfer (bool): Indicates whether the database is being transferred as a file.
             snapshot_id (int): The ID of the snapshot to upload.
             is_internal_db (bool): Indicates whether the database is an internal database.
             fd (BufferedReader): The file descriptor of the database file.
             dbsize (int): The size of the database file.
             xCallback (Callable[[BufferedReader, int, int, int], bytes]): The callback function to read the buffer.
 
         Raises:
-            SQCloudException: If an error occurs during the upload process.
+            SQLiteCloudException: If an error occurs during the upload process.
 
         """
         keyarg = "KEY " if key else ""
         keyvalue = key if key else ""
 
         # prepare command to execute
         command = ""
@@ -273,38 +327,38 @@
             command = f"TRANSFER DATABASE '{dbname}' {keyarg}{keyvalue} SNAPSHOT {snapshot_id} {internalarg}"
         else:
             command = f"UPLOAD DATABASE '{dbname}' {keyarg}{keyvalue}"
 
         # execute command on server side
         result = self._internal_run_command(connection, command)
         if not result.data[0]:
-            raise SQCloudException(
+            raise SQLiteCloudException(
                 "An error occurred while initializing the upload of the database."
             )
 
         buffer: bytes = b""
         blen = 0
         nprogress = 0
         try:
             while True:
                 # execute callback to read buffer
-                blen = SQCLOUD_DEFAULT.UPLOAD_SIZE.value
+                blen = SQLITECLOUD_DEFAULT.UPLOAD_SIZE.value
                 try:
                     buffer = xCallback(fd, blen, dbsize, nprogress)
                     blen = len(buffer)
                 except Exception as e:
-                    raise SQCloudException(
+                    raise SQLiteCloudException(
                         "An error occurred while reading the file."
                     ) from e
 
                 try:
                     # send also the final confirmation blob of zero bytes
                     self.send_blob(buffer, connection)
                 except Exception as e:
-                    raise SQCloudException(
+                    raise SQLiteCloudException(
                         "An error occurred while uploading the file."
                     ) from e
 
                 # update progress
                 nprogress += blen
 
                 if blen == 0:
@@ -312,41 +366,41 @@
                     break
         except Exception as e:
             self._internal_run_command(connection, "UPLOAD ABORT")
             raise e
 
     def download_database(
         self,
-        connection: SQCloudConnect,
+        connection: SQLiteCloudConnect,
         dbname: str,
         fd: BufferedWriter,
         xCallback: Callable[[BufferedWriter, int, int, int], bytes],
         if_exists: bool,
     ) -> None:
         """
         Downloads a database from the SQLite Cloud service.
 
         Args:
-            connection (SQCloudConnect): The connection object used to communicate with the SQLite Cloud service.
+            connection (SQLiteCloudConnect): The connection object used to communicate with the SQLite Cloud service.
             dbname (str): The name of the database to download.
             fd (BufferedWriter): The file descriptor to write the downloaded data to.
             xCallback (Callable[[BufferedWriter, int, int, int], bytes]): A callback function to write downloaded data with the download progress information.
             if_exists (bool): If True, the download won't rise an exception if database is missing.
 
         Raises:
-            SQCloudException: If an error occurs while downloading the database.
+            SQLiteCloudException: If an error occurs while downloading the database.
 
         """
         exists_cmd = " IF EXISTS" if if_exists else ""
         result = self._internal_run_command(
             connection, f"DOWNLOAD DATABASE {dbname}{exists_cmd};"
         )
 
         if result.nrows == 0:
-            raise SQCloudException(
+            raise SQLiteCloudException(
                 "An error occurred while initializing the download of the database."
             )
 
         # result is an ARRAY (database size, number of pages, raft_index)
         download_info = result.data[0]
         db_size = int(download_info[0])
 
@@ -369,21 +423,25 @@
                 if data_len == 0:
                     break
         except Exception as e:
             self._internal_run_command(connection, "DOWNLOAD ABORT")
             raise e
 
     def _internal_config_apply(
-        self, connection: SQCloudConnect, config: SQCloudConfig
+        self, connection: SQLiteCloudConnect, config: SQLiteCloudConfig
     ) -> None:
         if config.timeout > 0:
             connection.socket.settimeout(config.timeout)
 
         buffer = ""
 
+        # it must be executed before authentication command
+        if config.non_linearizable:
+            buffer += "SET CLIENT KEY NONLINEARIZABLE TO 1;"
+
         if config.account.apikey:
             buffer += f"AUTH APIKEY {config.account.apikey};"
 
         if config.account.username and config.account.password:
             command = "HASH" if config.account.password_hashed else "PASSWORD"
             buffer += f"AUTH USER {config.account.username} {command} {config.account.password};"
 
@@ -394,17 +452,14 @@
 
         if config.compression:
             buffer += "SET CLIENT KEY COMPRESSION TO 1;"
 
         if config.zerotext:
             buffer += "SET CLIENT KEY ZEROTEXT TO 1;"
 
-        if config.non_linearizable:
-            buffer += "SET CLIENT KEY NONLINEARIZABLE TO 1;"
-
         if config.noblob:
             buffer += "SET CLIENT KEY NOBLOB TO 1;"
 
         if config.maxdata:
             buffer += f"SET CLIENT KEY MAXDATA TO {config.maxdata};"
 
         if config.maxrows:
@@ -414,24 +469,30 @@
             buffer += f"SET CLIENT KEY MAXROWSET TO {config.maxrowset};"
 
         if len(buffer) > 0:
             self._internal_run_command(connection, buffer)
 
     def _internal_run_command(
         self,
-        connection: SQCloudConnect,
+        connection: SQLiteCloudConnect,
         command: Union[str, bytes],
         main_socket: bool = True,
-    ) -> SQCloudResult:
+    ) -> SQLiteCloudResult:
+        if not self.is_connected(connection, main_socket):
+            raise SQLiteCloudException(
+                "The connection is closed.",
+                SQLITECLOUD_INTERNAL_ERRCODE.NETWORK,
+            )
+
         self._internal_socket_write(connection, command, main_socket)
         return self._internal_socket_read(connection, main_socket)
 
     def _internal_socket_write(
         self,
-        connection: SQCloudConnect,
+        connection: SQLiteCloudConnect,
         command: Union[str, bytes],
         main_socket: bool = True,
     ) -> None:
         # compute header
         delimit = "$" if connection.isblob else "+"
         buffer = command.encode() if isinstance(command, str) else command
         buffer_len = len(buffer)
@@ -439,33 +500,33 @@
 
         sock = connection.socket if main_socket else connection.pubsub_socket
 
         # write header
         try:
             sock.sendall(header.encode())
         except Exception as exc:
-            raise SQCloudException(
+            raise SQLiteCloudException(
                 "An error occurred while writing header data.",
-                SQCLOUD_INTERNAL_ERRCODE.NETWORK,
+                SQLITECLOUD_INTERNAL_ERRCODE.NETWORK,
             ) from exc
 
         # write buffer
         if buffer_len == 0:
             return
         try:
             sock.sendall(buffer)
         except Exception as exc:
-            raise SQCloudException(
+            raise SQLiteCloudException(
                 "An error occurred while writing data.",
-                SQCLOUD_INTERNAL_ERRCODE.NETWORK,
+                SQLITECLOUD_INTERNAL_ERRCODE.NETWORK,
             ) from exc
 
     def _internal_socket_read(
-        self, connection: SQCloudConnect, main_socket: bool = True
-    ) -> SQCloudResult:
+        self, connection: SQLiteCloudConnect, main_socket: bool = True
+    ) -> SQLiteCloudResult:
         """
         Read from the socket and parse the response.
 
         The buffer is stored as a string of bytes without decoding it with UTF-8.
         The dimensions (LEN) specified in the SCSP protocol are in bytes, while
         Python counts decoded strings in characters. This can cause issues when
         slicing the buffer into parts if there are special characters like "ò".
@@ -476,58 +537,60 @@
 
         sock = connection.socket if main_socket else connection.pubsub_socket
 
         while True:
             try:
                 data = sock.recv(buffer_size)
                 if not data:
-                    raise SQCloudException("Incomplete response from server.")
+                    raise SQLiteCloudException("Incomplete response from server.")
             except Exception as exc:
-                raise SQCloudException(
+                raise SQLiteCloudException(
                     "An error occurred while reading data from the socket.",
-                    SQCLOUD_INTERNAL_ERRCODE.NETWORK,
+                    SQLITECLOUD_INTERNAL_ERRCODE.NETWORK,
                 ) from exc
 
             # the expected data length to read
             # matches the string size before decoding it
             nread += len(data)
             # update buffers
             buffer += data
 
             c = chr(buffer[0])
 
             if (
-                c == SQCLOUD_CMD.INT.value
-                or c == SQCLOUD_CMD.FLOAT.value
-                or c == SQCLOUD_CMD.NULL.value
+                c == SQLITECLOUD_CMD.INT.value
+                or c == SQLITECLOUD_CMD.FLOAT.value
+                or c == SQLITECLOUD_CMD.NULL.value
             ):
                 if not buffer.endswith(b" "):
                     continue
-            elif c == SQCLOUD_CMD.ROWSET_CHUNK.value:
-                isEndOfChunk = buffer.endswith(SQCLOUD_ROWSET.CHUNKS_END.value)
+            elif c == SQLITECLOUD_CMD.ROWSET_CHUNK.value:
+                isEndOfChunk = buffer.endswith(SQLITECLOUD_ROWSET.CHUNKS_END.value)
                 if not isEndOfChunk:
                     continue
             else:
-                sqcloud_number = self._internal_parse_number(buffer)
-                n = sqcloud_number.value
-                cstart = sqcloud_number.cstart
+                SQLiteCloud_number = self._internal_parse_number(buffer)
+                n = SQLiteCloud_number.value
+                cstart = SQLiteCloud_number.cstart
 
                 can_be_zerolength = (
-                    c == SQCLOUD_CMD.BLOB.value or c == SQCLOUD_CMD.STRING.value
+                    c == SQLITECLOUD_CMD.BLOB.value or c == SQLITECLOUD_CMD.STRING.value
                 )
                 if n == 0 and not can_be_zerolength:
                     continue
                 if n + cstart != nread:
                     continue
 
             return self._internal_parse_buffer(connection, buffer, len(buffer))
 
-    def _internal_parse_number(self, buffer: bytes, index: int = 1) -> SQCloudNumber:
-        sqcloud_number = SQCloudNumber()
-        sqcloud_number.value = 0
+    def _internal_parse_number(
+        self, buffer: bytes, index: int = 1
+    ) -> SQLiteCloudNumber:
+        SQLiteCloud_number = SQLiteCloudNumber()
+        SQLiteCloud_number.value = 0
         extvalue = 0
         isext = False
         blen = len(buffer)
 
         # from 1 to skip the first command type character
         for i in range(index, blen):
             c = chr(buffer[i])
@@ -535,109 +598,110 @@
             # check for optional extended error code (ERRCODE:EXTERRCODE)
             if c == ":":
                 isext = True
                 continue
 
             # check for end of value
             if c == " ":
-                sqcloud_number.cstart = i + 1
-                sqcloud_number.extcode = extvalue
-                return sqcloud_number
+                SQLiteCloud_number.cstart = i + 1
+                SQLiteCloud_number.extcode = extvalue
+                return SQLiteCloud_number
 
             val = int(c) if c.isdigit() else 0
 
             # compute numeric value
             if isext:
                 extvalue = (extvalue * 10) + val
             else:
-                sqcloud_number.value = (sqcloud_number.value * 10) + val
+                SQLiteCloud_number.value = (SQLiteCloud_number.value * 10) + val
 
-        sqcloud_number.value = 0
-        return sqcloud_number
+        SQLiteCloud_number.value = 0
+        return SQLiteCloud_number
 
     def _internal_parse_buffer(
-        self, connection: SQCloudConnect, buffer: bytes, blen: int
-    ) -> SQCloudResult:
+        self, connection: SQLiteCloudConnect, buffer: bytes, blen: int
+    ) -> SQLiteCloudResult:
         # possible return values:
         # True 	=> OK
         # False 	=> error
         # integer
         # double
         # string
         # list
         # object
         # None
 
         # check OK value
         if buffer == b"+2 OK":
-            return SQCloudResult(SQCLOUD_RESULT_TYPE.RESULT_OK, True)
+            return SQLiteCloudResult(SQLITECLOUD_RESULT_TYPE.RESULT_OK, True)
 
         cmd = chr(buffer[0])
 
         # check for compressed result
-        if cmd == SQCLOUD_CMD.COMPRESSED.value:
+        if cmd == SQLITECLOUD_CMD.COMPRESSED.value:
             buffer = self._internal_uncompress_data(buffer)
             if buffer is None:
-                raise SQCloudException(
+                raise SQLiteCloudException(
                     f"An error occurred while decompressing the input buffer of len {blen}."
                 )
 
             # buffer after decompression
             blen = len(buffer)
             cmd = chr(buffer[0])
 
         # first character contains command type
         if cmd in [
-            SQCLOUD_CMD.ZEROSTRING.value,
-            SQCLOUD_CMD.RECONNECT.value,
-            SQCLOUD_CMD.PUBSUB.value,
-            SQCLOUD_CMD.COMMAND.value,
-            SQCLOUD_CMD.STRING.value,
-            SQCLOUD_CMD.ARRAY.value,
-            SQCLOUD_CMD.BLOB.value,
-            SQCLOUD_CMD.JSON.value,
+            SQLITECLOUD_CMD.ZEROSTRING.value,
+            SQLITECLOUD_CMD.RECONNECT.value,
+            SQLITECLOUD_CMD.PUBSUB.value,
+            SQLITECLOUD_CMD.COMMAND.value,
+            SQLITECLOUD_CMD.STRING.value,
+            SQLITECLOUD_CMD.ARRAY.value,
+            SQLITECLOUD_CMD.BLOB.value,
+            SQLITECLOUD_CMD.JSON.value,
         ]:
             sqlite_number = self._internal_parse_number(buffer)
             len_ = sqlite_number.value
             cstart = sqlite_number.cstart
             if len_ == 0:
-                return SQCloudResult(SQCLOUD_RESULT_TYPE.RESULT_STRING, "")
+                return SQLiteCloudResult(SQLITECLOUD_RESULT_TYPE.RESULT_STRING, "")
 
             tag = (
-                SQCLOUD_RESULT_TYPE.RESULT_JSON
-                if cmd == SQCLOUD_CMD.JSON.value
-                else SQCLOUD_RESULT_TYPE.RESULT_STRING
+                SQLITECLOUD_RESULT_TYPE.RESULT_JSON
+                if cmd == SQLITECLOUD_CMD.JSON.value
+                else SQLITECLOUD_RESULT_TYPE.RESULT_STRING
             )
 
-            if cmd == SQCLOUD_CMD.ZEROSTRING.value:
+            if cmd == SQLITECLOUD_CMD.ZEROSTRING.value:
                 len_ -= 1
             clone = buffer[cstart : cstart + len_]
 
-            if cmd == SQCLOUD_CMD.COMMAND.value:
+            if cmd == SQLITECLOUD_CMD.COMMAND.value:
                 return self._internal_run_command(connection, clone)
-            elif cmd == SQCLOUD_CMD.PUBSUB.value:
-                return SQCloudResult(
-                    SQCLOUD_RESULT_TYPE.RESULT_OK,
+            elif cmd == SQLITECLOUD_CMD.PUBSUB.value:
+                return SQLiteCloudResult(
+                    SQLITECLOUD_RESULT_TYPE.RESULT_OK,
                     self._internal_setup_pubsub(connection, clone),
                 )
-            elif cmd == SQCLOUD_CMD.RECONNECT.value:
-                return SQCloudResult(
-                    SQCLOUD_RESULT_TYPE.RESULT_OK, self._internal_reconnect(clone)
+            elif cmd == SQLITECLOUD_CMD.RECONNECT.value:
+                return SQLiteCloudResult(
+                    SQLITECLOUD_RESULT_TYPE.RESULT_OK, self._internal_reconnect(clone)
                 )
-            elif cmd == SQCLOUD_CMD.ARRAY.value:
-                return SQCloudResult(
-                    SQCLOUD_RESULT_TYPE.RESULT_ARRAY, self._internal_parse_array(clone)
+            elif cmd == SQLITECLOUD_CMD.ARRAY.value:
+                return SQLiteCloudResult(
+                    SQLITECLOUD_RESULT_TYPE.RESULT_ARRAY,
+                    self._internal_parse_array(clone),
                 )
-            elif cmd == SQCLOUD_CMD.BLOB.value:
-                tag = SQCLOUD_RESULT_TYPE.RESULT_BLOB
+            elif cmd == SQLITECLOUD_CMD.BLOB.value:
+                tag = SQLITECLOUD_RESULT_TYPE.RESULT_BLOB
 
-            clone = clone.decode() if cmd != SQCLOUD_CMD.BLOB.value else clone
-            return SQCloudResult(tag, clone)
+            clone = clone.decode() if cmd != SQLITECLOUD_CMD.BLOB.value else clone
+            return SQLiteCloudResult(tag, clone)
 
-        elif cmd == SQCLOUD_CMD.ERROR.value:
+        elif cmd == SQLITECLOUD_CMD.ERROR.value:
             # -LEN ERRCODE:EXTCODE ERRMSG
             sqlite_number = self._internal_parse_number(buffer)
             len_ = sqlite_number.value
             cstart = sqlite_number.cstart
             clone = buffer[cstart:]
 
             sqlite_number = self._internal_parse_number(clone, 0)
@@ -645,25 +709,25 @@
 
             errcode = sqlite_number.value
             xerrcode = sqlite_number.extcode
 
             len_ -= cstart2
             errmsg = clone[cstart2:]
 
-            raise SQCloudException(errmsg.decode(), errcode, xerrcode)
+            raise SQLiteCloudException(errmsg.decode(), errcode, xerrcode)
 
-        elif cmd in [SQCLOUD_CMD.ROWSET.value, SQCLOUD_CMD.ROWSET_CHUNK.value]:
+        elif cmd in [SQLITECLOUD_CMD.ROWSET.value, SQLITECLOUD_CMD.ROWSET_CHUNK.value]:
             # CMD_ROWSET:          *LEN 0:VERSION ROWS COLS DATA
             # - When decompressed, LEN for ROWSET is *0
             #
             # CMD_ROWSET_CHUNK:    /LEN IDX:VERSION ROWS COLS DATA
             #
             rowset_signature = self._internal_parse_rowset_signature(buffer)
             if rowset_signature.start < 0:
-                raise SQCloudException("Cannot parse rowset signature")
+                raise SQLiteCloudException("Cannot parse rowset signature")
 
             # check for end-of-chunk condition
             if rowset_signature.start == 0 and rowset_signature.version == 0:
                 rowset = self._rowset
                 self._rowset = None
                 return rowset
 
@@ -675,43 +739,43 @@
                 rowset_signature.nrows,
                 rowset_signature.ncols,
             )
 
             # continue parsing next chunk in the buffer
             sign_len = rowset_signature.len
             buffer = buffer[sign_len + len(f"/{sign_len} ") :]
-            if cmd == SQCLOUD_CMD.ROWSET_CHUNK.value and buffer:
+            if cmd == SQLITECLOUD_CMD.ROWSET_CHUNK.value and buffer:
                 return self._internal_parse_buffer(connection, buffer, len(buffer))
 
             return rowset
 
-        elif cmd == SQCLOUD_CMD.NULL.value:
-            return SQCloudResult(SQCLOUD_RESULT_TYPE.RESULT_NONE, None)
+        elif cmd == SQLITECLOUD_CMD.NULL.value:
+            return SQLiteCloudResult(SQLITECLOUD_RESULT_TYPE.RESULT_NONE, None)
 
-        elif cmd in [SQCLOUD_CMD.INT.value, SQCLOUD_CMD.FLOAT.value]:
-            sqcloud_value = self._internal_parse_value(buffer)
-            clone = sqcloud_value.value
+        elif cmd in [SQLITECLOUD_CMD.INT.value, SQLITECLOUD_CMD.FLOAT.value]:
+            SQLiteCloud_value = self._internal_parse_value(buffer)
+            clone = SQLiteCloud_value.value
 
             tag = (
-                SQCLOUD_RESULT_TYPE.RESULT_INTEGER
-                if cmd == SQCLOUD_CMD.INT.value
-                else SQCLOUD_RESULT_TYPE.RESULT_FLOAT
+                SQLITECLOUD_RESULT_TYPE.RESULT_INTEGER
+                if cmd == SQLITECLOUD_CMD.INT.value
+                else SQLITECLOUD_RESULT_TYPE.RESULT_FLOAT
             )
 
             if clone is None:
-                return SQCloudResult(tag, 0)
+                return SQLiteCloudResult(tag, 0)
 
-            if cmd == SQCLOUD_CMD.INT.value:
-                return SQCloudResult(tag, int(clone))
-            return SQCloudResult(tag, float(clone))
+            if cmd == SQLITECLOUD_CMD.INT.value:
+                return SQLiteCloudResult(tag, int(clone))
+            return SQLiteCloudResult(tag, float(clone))
 
-        elif cmd == SQCLOUD_CMD.RAWJSON.value:
-            return SQCloudResult(SQCLOUD_RESULT_TYPE.RESULT_NONE, None)
+        elif cmd == SQLITECLOUD_CMD.RAWJSON.value:
+            return SQLiteCloudResult(SQLITECLOUD_RESULT_TYPE.RESULT_NONE, None)
 
-        return SQCloudResult(SQCLOUD_RESULT_TYPE.RESULT_NONE, None)
+        return SQLiteCloudResult(SQLITECLOUD_RESULT_TYPE.RESULT_NONE, None)
 
     def _internal_uncompress_data(self, buffer: bytes) -> Optional[bytes]:
         """
         %LEN COMPRESSED UNCOMPRESSED BUFFER
 
         Args:
             buffer (str): The compressed data buffer.
@@ -753,70 +817,72 @@
         start = 0
         sqlite_number = self._internal_parse_number(buffer, start)
         n = sqlite_number.value
         start = sqlite_number.cstart
 
         r: str = []
         for i in range(n):
-            sqcloud_value = self._internal_parse_value(buffer, start)
-            start += sqcloud_value.cellsize
-            r.append(sqcloud_value.value)
+            SQLiteCloud_value = self._internal_parse_value(buffer, start)
+            start += SQLiteCloud_value.cellsize
+            r.append(SQLiteCloud_value.value)
 
         return r
 
-    def _internal_parse_value(self, buffer: bytes, index: int = 0) -> SQCloudValue:
-        sqcloud_value = SQCloudValue()
+    def _internal_parse_value(self, buffer: bytes, index: int = 0) -> SQLiteCloudValue:
+        SQLiteCloud_value = SQLiteCloudValue()
         len = 0
         cellsize = 0
 
         # handle special NULL value case
         c = chr(buffer[index])
-        if buffer is None or c == SQCLOUD_CMD.NULL.value:
+        if buffer is None or c == SQLITECLOUD_CMD.NULL.value:
             len = 0
             if cellsize is not None:
                 cellsize = 2
 
-            sqcloud_value.len = len
-            sqcloud_value.cellsize = cellsize
+            SQLiteCloud_value.len = len
+            SQLiteCloud_value.cellsize = cellsize
 
-            return sqcloud_value
+            return SQLiteCloud_value
 
-        sqcloud_number = self._internal_parse_number(buffer, index + 1)
-        blen = sqcloud_number.value
-        cstart = sqcloud_number.cstart
+        SQLiteCloud_number = self._internal_parse_number(buffer, index + 1)
+        blen = SQLiteCloud_number.value
+        cstart = SQLiteCloud_number.cstart
 
         # handle decimal/float cases
-        if c == SQCLOUD_CMD.INT.value or c == SQCLOUD_CMD.FLOAT.value:
+        if c == SQLITECLOUD_CMD.INT.value or c == SQLITECLOUD_CMD.FLOAT.value:
             nlen = cstart - index
             len = nlen - 2
             cellsize = nlen
 
-            sqcloud_value.value = (buffer[index + 1 : index + 1 + len]).decode()
-            sqcloud_value.len
-            sqcloud_value.cellsize = cellsize
+            SQLiteCloud_value.value = (buffer[index + 1 : index + 1 + len]).decode()
+            SQLiteCloud_value.len
+            SQLiteCloud_value.cellsize = cellsize
 
-            return sqcloud_value
+            return SQLiteCloud_value
 
-        len = blen - 1 if c == SQCLOUD_CMD.ZEROSTRING.value else blen
+        len = blen - 1 if c == SQLITECLOUD_CMD.ZEROSTRING.value else blen
         cellsize = blen + cstart - index
 
-        sqcloud_value.value = (buffer[cstart : cstart + len]).decode()
-        sqcloud_value.len = len
-        sqcloud_value.cellsize = cellsize
-
-        return sqcloud_value
-
-    def _internal_parse_rowset_signature(self, buffer: bytes) -> SQCloudRowsetSignature:
+        SQLiteCloud_value.value = (buffer[cstart : cstart + len]).decode()
+        SQLiteCloud_value.len = len
+        SQLiteCloud_value.cellsize = cellsize
+
+        return SQLiteCloud_value
+
+    def _internal_parse_rowset_signature(
+        self, buffer: bytes
+    ) -> SQLiteCloudRowsetSignature:
         # ROWSET:          *LEN 0:VERS NROWS NCOLS DATA
         # ROWSET in CHUNK: /LEN IDX:VERS NROWS NCOLS DATA
 
-        signature = SQCloudRowsetSignature()
+        signature = SQLiteCloudRowsetSignature()
 
         # check for end-of-chunk condition
-        if buffer == SQCLOUD_ROWSET.CHUNKS_END.value:
+        if buffer == SQLITECLOUD_ROWSET.CHUNKS_END.value:
             signature.version = 0
             signature.start = 0
             return signature
 
         start = 1
         counter = 0
         n = len(buffer)
@@ -840,132 +906,134 @@
             elif counter == 4:
                 signature.ncols = int(data)
 
                 signature.start = start
 
                 return signature
             else:
-                return SQCloudRowsetSignature()
-        return SQCloudRowsetSignature()
+                return SQLiteCloudRowsetSignature()
+        return SQLiteCloudRowsetSignature()
 
     def _internal_parse_rowset(
         self, buffer: bytes, start: int, idx: int, version: int, nrows: int, ncols: int
-    ) -> SQCloudResult:
+    ) -> SQLiteCloudResult:
         rowset = None
         n = start
-        ischunk = chr(buffer[0]) == SQCLOUD_CMD.ROWSET_CHUNK.value
+        ischunk = chr(buffer[0]) == SQLITECLOUD_CMD.ROWSET_CHUNK.value
 
         # idx == 0 means first (and only) chunk for rowset
         # idx == 1 means first chunk for chunked rowset
         first_chunk = (ischunk and idx == 1) or (not ischunk and idx == 0)
         if first_chunk:
-            rowset = SQCloudResult(SQCLOUD_RESULT_TYPE.RESULT_ROWSET)
+            rowset = SQLiteCloudResult(SQLITECLOUD_RESULT_TYPE.RESULT_ROWSET)
             rowset.nrows = nrows
             rowset.ncols = ncols
             rowset.version = version
             rowset.data = []
             if ischunk:
                 self._rowset = rowset
             n = self._internal_parse_rowset_header(rowset, buffer, start)
             if n <= 0:
-                raise SQCloudException("Cannot parse rowset header")
+                raise SQLiteCloudException("Cannot parse rowset header")
         else:
             rowset = self._rowset
             rowset.nrows += nrows
 
         # parse values
         self._internal_parse_rowset_values(rowset, buffer, n, nrows * ncols)
 
         return rowset
 
     def _internal_parse_rowset_header(
-        self, rowset: SQCloudResult, buffer: bytes, start: int
+        self, rowset: SQLiteCloudResult, buffer: bytes, start: int
     ) -> int:
         ncols = rowset.ncols
 
         # parse column names
         rowset.colname = []
         for i in range(ncols):
-            sqcloud_number = self._internal_parse_number(buffer, start)
-            number_len = sqcloud_number.value
-            cstart = sqcloud_number.cstart
+            SQLiteCloud_number = self._internal_parse_number(buffer, start)
+            number_len = SQLiteCloud_number.value
+            cstart = SQLiteCloud_number.cstart
             value = buffer[cstart : cstart + number_len]
             rowset.colname.append(value.decode())
             start = cstart + number_len
 
         if rowset.version == 1:
             return start
 
         if rowset.version != 2:
-            raise SQCloudException(f"Rowset version {rowset.version} is not supported.")
+            raise SQLiteCloudException(
+                f"Rowset version {rowset.version} is not supported."
+            )
 
         # parse declared types
         rowset.decltype = []
         for i in range(ncols):
-            sqcloud_number = self._internal_parse_number(buffer, start)
-            number_len = sqcloud_number.value
-            cstart = sqcloud_number.cstart
+            SQLiteCloud_number = self._internal_parse_number(buffer, start)
+            number_len = SQLiteCloud_number.value
+            cstart = SQLiteCloud_number.cstart
             value = buffer[cstart : cstart + number_len]
             rowset.decltype.append(value.decode())
             start = cstart + number_len
 
         # parse database names
         rowset.dbname = []
         for i in range(ncols):
-            sqcloud_number = self._internal_parse_number(buffer, start)
-            number_len = sqcloud_number.value
-            cstart = sqcloud_number.cstart
+            SQLiteCloud_number = self._internal_parse_number(buffer, start)
+            number_len = SQLiteCloud_number.value
+            cstart = SQLiteCloud_number.cstart
             value = buffer[cstart : cstart + number_len]
             rowset.dbname.append(value.decode())
             start = cstart + number_len
 
         # parse table names
         rowset.tblname = []
         for i in range(ncols):
-            sqcloud_number = self._internal_parse_number(buffer, start)
-            number_len = sqcloud_number.value
-            cstart = sqcloud_number.cstart
+            SQLiteCloud_number = self._internal_parse_number(buffer, start)
+            number_len = SQLiteCloud_number.value
+            cstart = SQLiteCloud_number.cstart
             value = buffer[cstart : cstart + number_len]
             rowset.tblname.append(value.decode())
             start = cstart + number_len
 
         # parse column original names
         rowset.origname = []
         for i in range(ncols):
-            sqcloud_number = self._internal_parse_number(buffer, start)
-            number_len = sqcloud_number.value
-            cstart = sqcloud_number.cstart
+            SQLiteCloud_number = self._internal_parse_number(buffer, start)
+            number_len = SQLiteCloud_number.value
+            cstart = SQLiteCloud_number.cstart
             value = buffer[cstart : cstart + number_len]
             rowset.origname.append(value.decode())
             start = cstart + number_len
 
         # parse not null flags
         rowset.notnull = []
         for i in range(ncols):
-            sqcloud_number = self._internal_parse_number(buffer, start)
-            rowset.notnull.append(sqcloud_number.value)
-            start = sqcloud_number.cstart
+            SQLiteCloud_number = self._internal_parse_number(buffer, start)
+            rowset.notnull.append(SQLiteCloud_number.value)
+            start = SQLiteCloud_number.cstart
 
         # parse primary key flags
         rowset.prikey = []
         for i in range(ncols):
-            sqcloud_number = self._internal_parse_number(buffer, start)
-            rowset.prikey.append(sqcloud_number.value)
-            start = sqcloud_number.cstart
+            SQLiteCloud_number = self._internal_parse_number(buffer, start)
+            rowset.prikey.append(SQLiteCloud_number.value)
+            start = SQLiteCloud_number.cstart
 
         # parse autoincrement flags
         rowset.autoinc = []
         for i in range(ncols):
-            sqcloud_number = self._internal_parse_number(buffer, start)
-            rowset.autoinc.append(sqcloud_number.value)
-            start = sqcloud_number.cstart
+            SQLiteCloud_number = self._internal_parse_number(buffer, start)
+            rowset.autoinc.append(SQLiteCloud_number.value)
+            start = SQLiteCloud_number.cstart
 
         return start
 
     def _internal_parse_rowset_values(
-        self, rowset: SQCloudResult, buffer: bytes, start: int, bound: int
+        self, rowset: SQLiteCloudResult, buffer: bytes, start: int, bound: int
     ):
         # loop to parse each individual value
         for i in range(bound):
-            sqcloud_value = self._internal_parse_value(buffer, start)
-            start += sqcloud_value.cellsize
-            rowset.data.append(sqcloud_value.value)
+            SQLiteCloud_value = self._internal_parse_value(buffer, start)
+            start += SQLiteCloud_value.cellsize
+            rowset.data.append(SQLiteCloud_value.value)
```

### Comparing `sqlitecloud-0.0.77/sqlitecloud/pubsub.py` & `sqlitecloud-0.0.78/sqlitecloud/pubsub.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,69 +1,71 @@
 from typing import Callable, Optional
 
 from sqlitecloud.driver import Driver
-from sqlitecloud.resultset import SqliteCloudResultSet
-from sqlitecloud.types import SQCLOUD_PUBSUB_SUBJECT, SQCloudConnect
+from sqlitecloud.resultset import SQLiteCloudResultSet
+from sqlitecloud.types import SQLITECLOUD_PUBSUB_SUBJECT, SQLiteCloudConnect
 
 
-class SqliteCloudPubSub:
+class SQLiteCloudPubSub:
     def __init__(self) -> None:
         self._driver = Driver()
 
     def listen(
         self,
-        connection: SQCloudConnect,
-        subject_type: SQCLOUD_PUBSUB_SUBJECT,
+        connection: SQLiteCloudConnect,
+        subject_type: SQLITECLOUD_PUBSUB_SUBJECT,
         subject_name: str,
         callback: Callable[
-            [SQCloudConnect, Optional[SqliteCloudResultSet], Optional[any]], None
+            [SQLiteCloudConnect, Optional[SQLiteCloudResultSet], Optional[any]], None
         ],
         data: Optional[any] = None,
     ) -> None:
         subject = "TABLE " if subject_type.value == "TABLE" else ""
 
         connection.pubsub_callback = callback
         connection.pubsub_data = data
 
         self._driver.execute(f"LISTEN {subject}{subject_name};", connection)
 
     def unlisten(
         self,
-        connection: SQCloudConnect,
-        subject_type: SQCLOUD_PUBSUB_SUBJECT,
+        connection: SQLiteCloudConnect,
+        subject_type: SQLITECLOUD_PUBSUB_SUBJECT,
         subject_name: str,
     ) -> None:
         subject = "TABLE " if subject_type.value == "TABLE" else ""
 
         self._driver.execute(f"UNLISTEN {subject}{subject_name};", connection)
 
         connection.pubsub_callback = None
         connection.pubsub_data = None
 
     def create_channel(
-        self, connection: SQCloudConnect, name: str, if_not_exists: bool = False
+        self, connection: SQLiteCloudConnect, name: str, if_not_exists: bool = False
     ) -> None:
         if if_not_exists:
             self._driver.execute(f"CREATE CHANNEL {name} IF NOT EXISTS;", connection)
         else:
             self._driver.execute(f"CREATE CHANNEL {name};", connection)
 
-    def notify_channel(self, connection: SQCloudConnect, name: str, data: str) -> None:
+    def notify_channel(
+        self, connection: SQLiteCloudConnect, name: str, data: str
+    ) -> None:
         self._driver.execute(f"NOTIFY {name} '{data}';", connection)
 
-    def set_pubsub_only(self, connection: SQCloudConnect) -> None:
+    def set_pubsub_only(self, connection: SQLiteCloudConnect) -> None:
         """
         Close the main socket, leaving only the pub/sub socket opened and ready
         to receive incoming notifications from subscripted channels and tables.
 
         Connection is no longer able to send commands.
         """
         self._driver.execute("PUBSUB ONLY;", connection)
         self._driver.disconnect(connection, only_main_socket=True)
 
-    def is_connected(self, connection: SQCloudConnect) -> bool:
+    def is_connected(self, connection: SQLiteCloudConnect) -> bool:
         return self._driver.is_connected(connection, False)
 
-    def list_connections(self, connection: SQCloudConnect) -> SqliteCloudResultSet:
-        return SqliteCloudResultSet(
+    def list_connections(self, connection: SQLiteCloudConnect) -> SQLiteCloudResultSet:
+        return SQLiteCloudResultSet(
             self._driver.execute("LIST PUBSUB CONNECTIONS;", connection)
         )
```

### Comparing `sqlitecloud-0.0.77/sqlitecloud/resultset.py` & `sqlitecloud-0.0.78/sqlitecloud/resultset.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from typing import Any, Dict, List, Optional
 
-from sqlitecloud.types import SQCLOUD_RESULT_TYPE
+from sqlitecloud.types import SQLITECLOUD_RESULT_TYPE, SQLITECLOUD_VALUE_TYPE
 
 
-class SQCloudResult:
-    def __init__(self, tag: SQCLOUD_RESULT_TYPE, result: Optional[any] = None) -> None:
-        self.tag: SQCLOUD_RESULT_TYPE = tag
+class SQLiteCloudResult:
+    def __init__(
+        self, tag: SQLITECLOUD_RESULT_TYPE, result: Optional[any] = None
+    ) -> None:
+        self.tag: SQLITECLOUD_RESULT_TYPE = tag
         self.nrows: int = 0
         self.ncols: int = 0
         self.version: int = 0
         # table values are stored in 1-dimensional array
         self.data: List[Any] = []
         self.colname: List[str] = []
         self.decltype: List[str] = []
@@ -27,19 +29,56 @@
 
     def init_data(self, result: any) -> None:
         self.nrows = 1
         self.ncols = 1
         self.data = [result]
         self.is_result = True
 
+    def _compute_index(self, row: int, col: int) -> int:
+        if row < 0 or row >= self.nrows:
+            return -1
+        if col < 0 or col >= self.ncols:
+            return -1
+        return row * self.ncols + col
+
+    def get_value(self, row: int, col: int, convert: bool = True) -> Optional[any]:
+        index = self._compute_index(row, col)
+        if index < 0 or not self.data or index >= len(self.data):
+            return None
 
-class SqliteCloudResultSet:
-    def __init__(self, result: SQCloudResult) -> None:
+        value = self.data[index]
+        return self._convert(value, col) if convert else value
+
+    def get_name(self, col: int) -> Optional[str]:
+        if col < 0 or col >= self.ncols:
+            return None
+        return self.colname[col]
+
+    def _convert(self, value: str, col: int) -> any:
+        if col < 0 or col >= len(self.decltype):
+            return value
+
+        decltype = self.decltype[col]
+        if decltype == SQLITECLOUD_VALUE_TYPE.INTEGER.value:
+            return int(value)
+        if decltype == SQLITECLOUD_VALUE_TYPE.FLOAT.value:
+            return float(value)
+        if decltype == SQLITECLOUD_VALUE_TYPE.BLOB.value:
+            # values are received as bytes before being strings
+            return bytes(value)
+        if decltype == SQLITECLOUD_VALUE_TYPE.NULL.value:
+            return None
+
+        return value
+
+
+class SQLiteCloudResultSet:
+    def __init__(self, result: SQLiteCloudResult) -> None:
         self._iter_row: int = 0
-        self._result: SQCloudResult = result
+        self._result: SQLiteCloudResult = result
 
     def __getattr__(self, attr: str) -> Optional[Any]:
         return getattr(self._result, attr)
 
     def __iter__(self):
         return self
 
@@ -55,27 +94,15 @@
                     out[self.get_name(col)] = self.get_value(self._iter_row, col)
                 self._iter_row += 1
 
             return out
 
         raise StopIteration
 
-    def _compute_index(self, row: int, col: int) -> int:
-        if row < 0 or row >= self._result.nrows:
-            return -1
-        if col < 0 or col >= self._result.ncols:
-            return -1
-        return row * self._result.ncols + col
-
     def get_value(self, row: int, col: int) -> Optional[any]:
-        index = self._compute_index(row, col)
-        if index < 0 or not self._result.data or index >= len(self._result.data):
-            return None
-        return self._result.data[index]
+        return self._result.get_value(row, col)
 
     def get_name(self, col: int) -> Optional[str]:
-        if col < 0 or col >= self._result.ncols:
-            return None
-        return self._result.colname[col]
+        return self._result.get_name(col)
 
     def get_result(self) -> Optional[any]:
         return self.get_value(0, 0)
```

### Comparing `sqlitecloud-0.0.77/sqlitecloud/upload.py` & `sqlitecloud-0.0.78/sqlitecloud/upload.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import os
 from io import BufferedReader
 from typing import Optional
 
 from sqlitecloud.driver import Driver
-from sqlitecloud.types import SQCloudConnect
+from sqlitecloud.types import SQLiteCloudConnect
 
 
 def xCallback(fd: BufferedReader, blen: int, ntot: int, nprogress: int) -> bytes:
     """
     Callback function used for uploading data.
 
     Args:
@@ -28,27 +28,27 @@
     else:
         logging.log(logging.DEBUG, f"{(nprogress + nread) / ntot * 100:.2f}%")
 
     return buffer
 
 
 def upload_db(
-    connection: SQCloudConnect, dbname: str, key: Optional[str], filename: str
+    connection: SQLiteCloudConnect, dbname: str, key: Optional[str], filename: str
 ) -> None:
     """
     Uploads a SQLite database to the SQLite Cloud node using the provided connection.
 
     Args:
-        connection (SQCloudConnect): The connection object used to connect to the node.
+        connection (SQLiteCloudConnect): The connection object used to connect to the node.
         dbname (str): The name of the database in SQLite Cloud.
         key (Optional[str]): The encryption key for the database. If None, no encryption is used.
         filename (str): The path to the SQLite database file to be uploaded.
 
     Raises:
-        SQCloudException: If an error occurs while uploading the database.
+        SQLiteCloudException: If an error occurs while uploading the database.
 
     """
 
     # Create a driver object
     driver = Driver()
 
     with open(filename, "rb") as fd:
```

### Comparing `sqlitecloud-0.0.77/tests/conftest.py` & `sqlitecloud-0.0.78/tests/conftest.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,51 @@
 import os
 
 import pytest
 from dotenv import load_dotenv
 
-from sqlitecloud.client import SqliteCloudClient
-from sqlitecloud.types import SQCloudConnect, SqliteCloudAccount
+import sqlitecloud
+from sqlitecloud.client import SQLiteCloudClient
+from sqlitecloud.types import SQLiteCloudAccount, SQLiteCloudConnect
 
 
 @pytest.fixture(autouse=True)
 def load_env_vars():
     load_dotenv(".env")
 
 
 @pytest.fixture()
 def sqlitecloud_connection():
-    account = SqliteCloudAccount()
+    account = SQLiteCloudAccount()
     account.username = os.getenv("SQLITE_USER")
     account.password = os.getenv("SQLITE_PASSWORD")
     account.dbname = os.getenv("SQLITE_DB")
     account.hostname = os.getenv("SQLITE_HOST")
     account.port = int(os.getenv("SQLITE_PORT"))
 
-    client = SqliteCloudClient(cloud_account=account)
+    client = SQLiteCloudClient(cloud_account=account)
 
     connection = client.open_connection()
-    assert isinstance(connection, SQCloudConnect)
+    assert isinstance(connection, SQLiteCloudConnect)
     assert client.is_connected(connection)
 
     yield (connection, client)
 
     client.disconnect(connection)
+
+
+@pytest.fixture()
+def sqlitecloud_dbapi2_connection():
+    account = SQLiteCloudAccount()
+    account.username = os.getenv("SQLITE_USER")
+    account.password = os.getenv("SQLITE_PASSWORD")
+    account.dbname = os.getenv("SQLITE_DB")
+    account.hostname = os.getenv("SQLITE_HOST")
+    account.port = int(os.getenv("SQLITE_PORT"))
+
+    connection = sqlitecloud.connect(account)
+
+    assert isinstance(connection, sqlitecloud.Connection)
+
+    yield connection
+
+    connection.close()
```

### Comparing `sqlitecloud-0.0.77/tests/integration/test_client.py` & `sqlitecloud-0.0.78/tests/integration/test_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,109 +1,109 @@
 import json
 import os
 import time
 
 import pytest
 
-from sqlitecloud.client import SqliteCloudClient
+from sqlitecloud.client import SQLiteCloudClient
 from sqlitecloud.types import (
-    SQCLOUD_ERRCODE,
-    SQCLOUD_INTERNAL_ERRCODE,
-    SQCLOUD_RESULT_TYPE,
-    SQCloudConnect,
-    SQCloudException,
-    SqliteCloudAccount,
+    SQLITECLOUD_ERRCODE,
+    SQLITECLOUD_INTERNAL_ERRCODE,
+    SQLITECLOUD_RESULT_TYPE,
+    SQLiteCloudAccount,
+    SQLiteCloudConnect,
+    SQLiteCloudException,
 )
 
 
 class TestClient:
     # Will warn if a query or other basic operation is slower than this
     WARN_SPEED_MS = 500
 
     # Will except queries to be quicker than this
     EXPECT_SPEED_MS = 6 * 1000
 
     def test_connection_with_credentials(self):
-        account = SqliteCloudAccount()
+        account = SQLiteCloudAccount()
         account.username = os.getenv("SQLITE_USER")
         account.password = os.getenv("SQLITE_PASSWORD")
         account.dbname = os.getenv("SQLITE_DB")
         account.hostname = os.getenv("SQLITE_HOST")
         account.port = int(os.getenv("SQLITE_PORT"))
 
-        client = SqliteCloudClient(cloud_account=account)
+        client = SQLiteCloudClient(cloud_account=account)
         conn = client.open_connection()
-        assert isinstance(conn, SQCloudConnect)
+        assert isinstance(conn, SQLiteCloudConnect)
 
         client.disconnect(conn)
 
     def test_connection_with_apikey(self):
-        account = SqliteCloudAccount()
+        account = SQLiteCloudAccount()
         account.username = os.getenv("SQLITE_API_KEY")
         account.hostname = os.getenv("SQLITE_HOST")
         account.port = int(os.getenv("SQLITE_PORT"))
 
-        client = SqliteCloudClient(cloud_account=account)
+        client = SQLiteCloudClient(cloud_account=account)
         conn = client.open_connection()
-        assert isinstance(conn, SQCloudConnect)
+        assert isinstance(conn, SQLiteCloudConnect)
 
         client.disconnect(conn)
 
     def test_connection_without_credentials_and_apikey(self):
-        account = SqliteCloudAccount()
+        account = SQLiteCloudAccount()
         account.dbname = os.getenv("SQLITE_DB")
         account.hostname = os.getenv("SQLITE_HOST")
         account.port = int(os.getenv("SQLITE_PORT"))
 
-        client = SqliteCloudClient(cloud_account=account)
+        client = SQLiteCloudClient(cloud_account=account)
 
-        with pytest.raises(SQCloudException):
+        with pytest.raises(SQLiteCloudException):
             client.open_connection()
 
     def test_connect_with_string(self):
         connection_string = os.getenv("SQLITE_CONNECTION_STRING")
 
-        client = SqliteCloudClient(connection_str=connection_string)
+        client = SQLiteCloudClient(connection_str=connection_string)
 
         conn = client.open_connection()
-        assert isinstance(conn, SQCloudConnect)
+        assert isinstance(conn, SQLiteCloudConnect)
 
         client.disconnect(conn)
 
     def test_connect_with_string_with_credentials(self):
         connection_string = f"sqlitecloud://{os.getenv('SQLITE_USER')}:{os.getenv('SQLITE_PASSWORD')}@{os.getenv('SQLITE_HOST')}/{os.getenv('SQLITE_DB')}"
 
-        client = SqliteCloudClient(connection_str=connection_string)
+        client = SQLiteCloudClient(connection_str=connection_string)
 
         conn = client.open_connection()
-        assert isinstance(conn, SQCloudConnect)
+        assert isinstance(conn, SQLiteCloudConnect)
 
         client.disconnect(conn)
 
     def test_is_connected(self):
-        account = SqliteCloudAccount()
+        account = SQLiteCloudAccount()
         account.username = os.getenv("SQLITE_API_KEY")
         account.hostname = os.getenv("SQLITE_HOST")
         account.port = int(os.getenv("SQLITE_PORT"))
 
-        client = SqliteCloudClient(cloud_account=account)
+        client = SQLiteCloudClient(cloud_account=account)
 
         conn = client.open_connection()
         assert client.is_connected(conn)
 
         client.disconnect(conn)
         assert not client.is_connected(conn)
 
     def test_disconnect(self):
-        account = SqliteCloudAccount()
+        account = SQLiteCloudAccount()
         account.username = os.getenv("SQLITE_API_KEY")
         account.hostname = os.getenv("SQLITE_HOST")
         account.port = int(os.getenv("SQLITE_PORT"))
 
-        client = SqliteCloudClient(cloud_account=account)
+        client = SQLiteCloudClient(cloud_account=account)
 
         conn = client.open_connection()
         assert client.is_connected(conn)
 
         client.disconnect(conn)
         assert not client.is_connected(conn)
         assert conn.socket is None
@@ -120,36 +120,36 @@
         assert not result.is_result
         assert 1 == result.nrows
         assert 1 == result.ncols
         assert "Hello" == result.get_value(0, 0)
 
     def test_column_not_found(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
-        with pytest.raises(SQCloudException) as e:
+        with pytest.raises(SQLiteCloudException) as e:
             client.exec_query("SELECT not_a_column FROM albums", connection)
 
         assert e.value.errcode == 1
         assert e.value.errmsg == "no such column: not_a_column"
 
     def test_rowset_data(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
         result = client.exec_query("SELECT AlbumId FROM albums LIMIT 2", connection)
 
-        assert SQCLOUD_RESULT_TYPE.RESULT_ROWSET == result.tag
+        assert SQLITECLOUD_RESULT_TYPE.RESULT_ROWSET == result.tag
         assert 2 == result.nrows
         assert 1 == result.ncols
         assert 2 == result.version
 
     def test_get_value(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
         result = client.exec_query("SELECT * FROM albums", connection)
 
-        assert "1" == result.get_value(0, 0)
+        assert 1 == result.get_value(0, 0)
         assert "For Those About To Rock We Salute You" == result.get_value(0, 1)
-        assert "2" == result.get_value(1, 0)
+        assert 2 == result.get_value(1, 0)
 
     def test_select_utf8_value_and_column_name(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
         result = client.exec_query("SELECT 'Minha História'", connection)
 
         assert result.nrows == 1
         assert result.ncols == 1
@@ -190,58 +190,58 @@
         assert "VALUE" == rowset.get_name(0)
         assert value == rowset.get_value(0, 0)
 
     def test_integer(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
         result = client.exec_query("TEST INTEGER", connection)
 
-        assert SQCLOUD_RESULT_TYPE.RESULT_INTEGER == result.tag
+        assert SQLITECLOUD_RESULT_TYPE.RESULT_INTEGER == result.tag
         assert 123456 == result.get_result()
 
     def test_float(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
         result = client.exec_query("TEST FLOAT", connection)
 
-        assert SQCLOUD_RESULT_TYPE.RESULT_FLOAT == result.tag
+        assert SQLITECLOUD_RESULT_TYPE.RESULT_FLOAT == result.tag
         assert 3.1415926 == result.get_result()
 
     def test_string(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
         result = client.exec_query("TEST STRING", connection)
 
-        assert SQCLOUD_RESULT_TYPE.RESULT_STRING == result.tag
+        assert SQLITECLOUD_RESULT_TYPE.RESULT_STRING == result.tag
         assert result.get_result() == "Hello World, this is a test string."
 
     def test_zero_string(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
         result = client.exec_query("TEST ZERO_STRING", connection)
 
-        assert SQCLOUD_RESULT_TYPE.RESULT_STRING == result.tag
+        assert SQLITECLOUD_RESULT_TYPE.RESULT_STRING == result.tag
         assert (
             result.get_result() == "Hello World, this is a zero-terminated test string."
         )
 
     def test_empty_string(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
         result = client.exec_query("TEST STRING0", connection)
 
-        assert SQCLOUD_RESULT_TYPE.RESULT_STRING == result.tag
+        assert SQLITECLOUD_RESULT_TYPE.RESULT_STRING == result.tag
         assert result.get_result() == ""
 
     def test_command(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
         result = client.exec_query("TEST COMMAND", connection)
 
         assert "PONG" == result.get_result()
 
     def test_json(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
         result = client.exec_query("TEST JSON", connection)
 
-        assert SQCLOUD_RESULT_TYPE.RESULT_JSON == result.tag
+        assert SQLITECLOUD_RESULT_TYPE.RESULT_JSON == result.tag
         assert {
             "msg-from": {"class": "soldier", "name": "Wixilav"},
             "msg-to": {"class": "supreme-commander", "name": "[Redacted]"},
             "msg-type": ["0xdeadbeef", "irc log"],
             "msg-log": [
                 "soldier: Boss there is a slight problem with the piece offering to humans",
                 "supreme-commander: Explain yourself soldier!",
@@ -250,37 +250,37 @@
             ],
         } == json.loads(result.get_result())
 
     def test_blob(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
         result = client.exec_query("TEST BLOB", connection)
 
-        assert SQCLOUD_RESULT_TYPE.RESULT_BLOB == result.tag
+        assert SQLITECLOUD_RESULT_TYPE.RESULT_BLOB == result.tag
         assert len(result.get_result()) == 1000
 
     def test_blob0(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
         result = client.exec_query("TEST BLOB0", connection)
 
-        assert SQCLOUD_RESULT_TYPE.RESULT_STRING == result.tag
+        assert SQLITECLOUD_RESULT_TYPE.RESULT_STRING == result.tag
         assert len(result.get_result()) == 0
 
     def test_error(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
 
-        with pytest.raises(SQCloudException) as e:
+        with pytest.raises(SQLiteCloudException) as e:
             client.exec_query("TEST ERROR", connection)
 
         assert e.value.errcode == 66666
         assert e.value.errmsg == "This is a test error message with a devil error code."
 
     def test_ext_error(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
 
-        with pytest.raises(SQCloudException) as e:
+        with pytest.raises(SQLiteCloudException) as e:
             client.exec_query("TEST EXTERROR", connection)
 
         assert e.value.errcode == 66666
         assert e.value.xerrcode == 333
         assert (
             e.value.errmsg
             == "This is a test error message with an extcode and a devil error code."
@@ -288,78 +288,78 @@
 
     def test_array(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
         result = client.exec_query("TEST ARRAY", connection)
 
         result_array = result.get_result()
 
-        assert SQCLOUD_RESULT_TYPE.RESULT_ARRAY == result.tag
+        assert SQLITECLOUD_RESULT_TYPE.RESULT_ARRAY == result.tag
         assert isinstance(result_array, list)
         assert len(result_array) == 5
         assert result_array[0] == "Hello World"
         assert result_array[1] == "123456"
         assert result_array[2] == "3.1415"
         assert result_array[3] is None
 
     def test_rowset(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
         result = client.exec_query("TEST ROWSET", connection)
 
-        assert SQCLOUD_RESULT_TYPE.RESULT_ROWSET == result.tag
+        assert SQLITECLOUD_RESULT_TYPE.RESULT_ROWSET == result.tag
         assert result.nrows >= 30
         assert result.ncols == 2
         assert result.version in [1, 2]
         assert result.get_name(0) == "key"
         assert result.get_name(1) == "value"
 
     def test_max_rows_option(self):
-        account = SqliteCloudAccount()
+        account = SQLiteCloudAccount()
         account.hostname = os.getenv("SQLITE_HOST")
         account.dbname = os.getenv("SQLITE_DB")
         account.apikey = os.getenv("SQLITE_API_KEY")
 
-        client = SqliteCloudClient(cloud_account=account)
+        client = SQLiteCloudClient(cloud_account=account)
         client.config.maxrows = 1
 
         connection = client.open_connection()
 
         rowset = client.exec_query("TEST ROWSET_CHUNK", connection)
 
         client.disconnect(connection)
 
         # maxrows cannot be tested at this level.
         # just expect everything is ok
         assert rowset.nrows > 100
 
     def test_max_rowset_option_to_fail_when_rowset_is_bigger(self):
-        account = SqliteCloudAccount()
+        account = SQLiteCloudAccount()
         account.hostname = os.getenv("SQLITE_HOST")
         account.dbname = os.getenv("SQLITE_DB")
         account.apikey = os.getenv("SQLITE_API_KEY")
 
-        client = SqliteCloudClient(cloud_account=account)
+        client = SQLiteCloudClient(cloud_account=account)
         client.config.maxrowset = 1024
 
         connection = client.open_connection()
 
-        with pytest.raises(SQCloudException) as e:
+        with pytest.raises(SQLiteCloudException) as e:
             client.exec_query("SELECT * FROM albums", connection)
 
         client.disconnect(connection)
 
-        assert SQCLOUD_ERRCODE.INTERNAL.value == e.value.errcode
+        assert SQLITECLOUD_ERRCODE.INTERNAL.value == e.value.errcode
         assert "RowSet too big to be sent (limit set to 1024 bytes)." == e.value.errmsg
 
     def test_max_rowset_option_to_succeed_when_rowset_is_lighter(self):
-        account = SqliteCloudAccount()
+        account = SQLiteCloudAccount()
         account.hostname = os.getenv("SQLITE_HOST")
         account.dbname = os.getenv("SQLITE_DB")
         account.apikey = os.getenv("SQLITE_API_KEY")
 
-        client = SqliteCloudClient(cloud_account=account)
+        client = SQLiteCloudClient(cloud_account=account)
         client.config.maxrowset = 1024
 
         connection = client.open_connection()
 
         rowset = client.exec_query("SELECT 'hello world'", connection)
 
         client.disconnect(connection)
@@ -367,15 +367,15 @@
         assert 1 == rowset.nrows
 
     def test_chunked_rowset(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
 
         rowset = client.exec_query("TEST ROWSET_CHUNK", connection)
 
-        assert SQCLOUD_RESULT_TYPE.RESULT_ROWSET == rowset.tag
+        assert SQLITECLOUD_RESULT_TYPE.RESULT_ROWSET == rowset.tag
         assert 147 == rowset.nrows
         assert 1 == rowset.ncols
         assert 147 == len(rowset.data)
         assert "key" == rowset.get_name(0)
 
     def test_chunked_rowset_twice(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
@@ -409,26 +409,26 @@
             assert 2 == rowset.ncols
             assert "count" == rowset.get_name(0)
             assert "string" == rowset.get_name(1)
             assert str(i) == rowset.get_value(0, 0)
             assert rowset.version in [1, 2]
 
     def test_query_timeout(self):
-        account = SqliteCloudAccount()
+        account = SQLiteCloudAccount()
         account.hostname = os.getenv("SQLITE_HOST")
         account.dbname = os.getenv("SQLITE_DB")
         account.apikey = os.getenv("SQLITE_API_KEY")
 
-        client = SqliteCloudClient(cloud_account=account)
+        client = SQLiteCloudClient(cloud_account=account)
         client.config.timeout = 1  # 1 sec
 
         connection = client.open_connection()
 
         # this operation should take more than 1 sec
-        with pytest.raises(SQCloudException) as e:
+        with pytest.raises(SQLiteCloudException) as e:
             # just a long running query
             client.exec_query(
                 """
                 WITH RECURSIVE r(i) AS (
                     VALUES(0)
                     UNION ALL
                     SELECT i FROM r
@@ -436,15 +436,15 @@
                 )
                 SELECT i FROM r WHERE i = 1;""",
                 connection,
             )
 
         client.disconnect(connection)
 
-        assert e.value.errcode == SQCLOUD_INTERNAL_ERRCODE.NETWORK
+        assert e.value.errcode == SQLITECLOUD_INTERNAL_ERRCODE.NETWORK
         assert e.value.errmsg == "An error occurred while reading data from the socket."
 
     def test_XXL_query(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
 
         xxl_query = 300000
         long_sql = ""
@@ -504,20 +504,20 @@
 
         assert rowset.nrows == 1
         assert rowset.ncols == 1
         assert rowset.get_value(0, 0).startswith("xxxxxxxx")
         assert len(rowset.get_value(0, 0)) == 1000
 
     def test_select_database(self):
-        account = SqliteCloudAccount()
+        account = SQLiteCloudAccount()
         account.hostname = os.getenv("SQLITE_HOST")
         account.dbname = ""
         account.apikey = os.getenv("SQLITE_API_KEY")
 
-        client = SqliteCloudClient(cloud_account=account)
+        client = SQLiteCloudClient(cloud_account=account)
 
         connection = client.open_connection()
 
         rowset = client.exec_query("USE DATABASE chinook.sqlite", connection)
 
         client.disconnect(connection)
 
@@ -600,20 +600,20 @@
                 query_ms = round((time.time() - start_time) * 1000 / num_queries)
                 if query_ms > self.WARN_SPEED_MS:
                     assert (
                         query_ms < self.EXPECT_SPEED_MS
                     ), f"{num_queries}x batched selects, {query_ms}ms per query"
 
     def test_compression_single_column(self):
-        account = SqliteCloudAccount()
+        account = SQLiteCloudAccount()
         account.hostname = os.getenv("SQLITE_HOST")
         account.apikey = os.getenv("SQLITE_API_KEY")
         account.dbname = os.getenv("SQLITE_DB")
 
-        client = SqliteCloudClient(cloud_account=account)
+        client = SQLiteCloudClient(cloud_account=account)
         client.config.compression = True
 
         connection = client.open_connection()
 
         # min compression size for rowset set by default to 20400 bytes
         blob_size = 20 * 1024
         # rowset = client.exec_query("SELECT * from albums inner join albums a2 on albums.AlbumId = a2.AlbumId")
@@ -625,20 +625,20 @@
 
         assert rowset.nrows == 1
         assert rowset.ncols == 1
         assert rowset.get_name(0) == "someColumnName"
         assert len(rowset.get_value(0, 0)) == blob_size * 2
 
     def test_compression_multiple_columns(self):
-        account = SqliteCloudAccount()
+        account = SQLiteCloudAccount()
         account.hostname = os.getenv("SQLITE_HOST")
         account.apikey = os.getenv("SQLITE_API_KEY")
         account.dbname = os.getenv("SQLITE_DB")
 
-        client = SqliteCloudClient(cloud_account=account)
+        client = SQLiteCloudClient(cloud_account=account)
         client.config.compression = True
 
         connection = client.open_connection()
 
         # min compression size for rowset set by default to 20400 bytes
         rowset = client.exec_query(
             "SELECT * from albums inner join albums a2 on albums.AlbumId = a2.AlbumId",
@@ -646,7 +646,34 @@
         )
 
         client.disconnect(connection)
 
         assert rowset.nrows > 0
         assert rowset.ncols > 0
         assert rowset.get_name(0) == "AlbumId"
+
+    def test_exec_statement_with_named_placeholder(self, sqlitecloud_connection):
+        connection, client = sqlitecloud_connection
+
+        result = client.exec_statement(
+            "SELECT * FROM albums WHERE AlbumId = :id and Title = :title",
+            {"id": 1, "title": "For Those About To Rock We Salute You"},
+            connection,
+        )
+
+        assert result.nrows == 1
+        assert result.get_value(0, 0) == 1
+
+    def test_exec_statement_with_qmarks(self, sqlitecloud_connection):
+        connection, client = sqlitecloud_connection
+
+        result = client.exec_statement(
+            "SELECT * FROM albums WHERE AlbumId = ? and Title = ?",
+            (
+                1,
+                "For Those About To Rock We Salute You",
+            ),
+            connection,
+        )
+
+        assert result.nrows == 1
+        assert result.get_value(0, 0) == 1
```

### Comparing `sqlitecloud-0.0.77/tests/integration/test_download.py` & `sqlitecloud-0.0.78/tests/integration/test_download.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sqlite3
 import tempfile
 
 import pytest
 
 from sqlitecloud import download
-from sqlitecloud.types import SQCLOUD_ERRCODE, SQCloudException
+from sqlitecloud.types import SQLITECLOUD_ERRCODE, SQLiteCloudException
 
 
 class TestDownload:
     def test_download_database(self, sqlitecloud_connection):
         connection, _ = sqlitecloud_connection
 
         temp_file = tempfile.mkstemp(prefix="chinook")[1]
@@ -21,12 +21,12 @@
         assert cursor.description[1][0] == "Title"
 
     def test_download_missing_database(self, sqlitecloud_connection):
         connection, _ = sqlitecloud_connection
 
         temp_file = tempfile.mkstemp(prefix="missing")[1]
 
-        with pytest.raises(SQCloudException) as e:
+        with pytest.raises(SQLiteCloudException) as e:
             download.download_db(connection, "missing.sqlite", temp_file)
 
-        assert e.value.errcode == SQCLOUD_ERRCODE.COMMAND.value
+        assert e.value.errcode == SQLITECLOUD_ERRCODE.COMMAND.value
         assert e.value.errmsg == "Database missing.sqlite does not exist."
```

### Comparing `sqlitecloud-0.0.77/tests/integration/test_driver.py` & `sqlitecloud-0.0.78/tests/integration/test_driver.py`

 * *Files identical despite different names*

### Comparing `sqlitecloud-0.0.77/tests/integration/test_pubsub.py` & `sqlitecloud-0.0.78/tests/integration/test_pubsub.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 import threading
 import uuid
 
 import pytest
 
-from sqlitecloud.pubsub import SqliteCloudPubSub
-from sqlitecloud.resultset import SqliteCloudResultSet
+from sqlitecloud.pubsub import SQLiteCloudPubSub
+from sqlitecloud.resultset import SQLiteCloudResultSet
 from sqlitecloud.types import (
-    SQCLOUD_ERRCODE,
-    SQCLOUD_PUBSUB_SUBJECT,
-    SQCLOUD_RESULT_TYPE,
-    SQCloudException,
+    SQLITECLOUD_ERRCODE,
+    SQLITECLOUD_PUBSUB_SUBJECT,
+    SQLITECLOUD_RESULT_TYPE,
+    SQLiteCloudException,
 )
 
 
 class TestPubSub:
     def test_listen_channel_and_notify(self, sqlitecloud_connection):
         connection, _ = sqlitecloud_connection
 
         callback_called = False
         flag = threading.Event()
 
         def assert_callback(conn, result, data):
             nonlocal callback_called
             nonlocal flag
 
-            if isinstance(result, SqliteCloudResultSet):
-                assert result.tag == SQCLOUD_RESULT_TYPE.RESULT_JSON
+            if isinstance(result, SQLiteCloudResultSet):
+                assert result.tag == SQLITECLOUD_RESULT_TYPE.RESULT_JSON
                 assert data == ["somedata"]
                 callback_called = True
                 flag.set()
 
-        pubsub = SqliteCloudPubSub()
-        type = SQCLOUD_PUBSUB_SUBJECT.CHANNEL
+        pubsub = SQLiteCloudPubSub()
+        type = SQLITECLOUD_PUBSUB_SUBJECT.CHANNEL
         channel = "channel" + str(uuid.uuid4())
 
         pubsub.create_channel(connection, channel)
         pubsub.listen(connection, type, channel, assert_callback, ["somedata"])
 
         pubsub.notify_channel(connection, channel, "somedata2")
 
@@ -43,16 +43,16 @@
         flag.wait(30)
 
         assert callback_called
 
     def test_unlisten_channel(self, sqlitecloud_connection):
         connection, _ = sqlitecloud_connection
 
-        pubsub = SqliteCloudPubSub()
-        type = SQCLOUD_PUBSUB_SUBJECT.CHANNEL
+        pubsub = SQLiteCloudPubSub()
+        type = SQLITECLOUD_PUBSUB_SUBJECT.CHANNEL
         channel_name = "channel" + str(uuid.uuid4())
 
         pubsub.create_channel(connection, channel_name)
         pubsub.listen(connection, type, channel_name, lambda conn, result, data: None)
 
         result = pubsub.list_connections(connection)
         assert channel_name in result.data
@@ -64,40 +64,40 @@
         assert channel_name not in result.data
         assert connection.pubsub_callback is None
         assert connection.pubsub_data is None
 
     def test_create_channel_to_fail_if_exists(self, sqlitecloud_connection):
         connection, _ = sqlitecloud_connection
 
-        pubsub = SqliteCloudPubSub()
+        pubsub = SQLiteCloudPubSub()
         channel_name = "channel" + str(uuid.uuid4())
 
         pubsub.create_channel(connection, channel_name, if_not_exists=True)
 
-        with pytest.raises(SQCloudException) as e:
+        with pytest.raises(SQLiteCloudException) as e:
             pubsub.create_channel(connection, channel_name, if_not_exists=False)
 
         assert (
             e.value.errmsg
             == f"Cannot create channel {channel_name} because it already exists."
         )
-        assert e.value.errcode == SQCLOUD_ERRCODE.GENERIC.value
+        assert e.value.errcode == SQLITECLOUD_ERRCODE.GENERIC.value
 
     def test_is_connected(self, sqlitecloud_connection):
         connection, _ = sqlitecloud_connection
 
-        pubsub = SqliteCloudPubSub()
+        pubsub = SQLiteCloudPubSub()
         channel_name = "channel" + str(uuid.uuid4())
 
         assert not pubsub.is_connected(connection)
 
         pubsub.create_channel(connection, channel_name, if_not_exists=True)
         pubsub.listen(
             connection,
-            SQCLOUD_PUBSUB_SUBJECT.CHANNEL,
+            SQLITECLOUD_PUBSUB_SUBJECT.CHANNEL,
             channel_name,
             lambda conn, result, data: None,
         )
 
         assert pubsub.is_connected(connection)
 
     def test_set_pubsub_only(self, sqlitecloud_connection):
@@ -106,33 +106,33 @@
         callback_called = False
         flag = threading.Event()
 
         def assert_callback(conn, result, data):
             nonlocal callback_called
             nonlocal flag
 
-            if isinstance(result, SqliteCloudResultSet):
+            if isinstance(result, SQLiteCloudResultSet):
                 assert result.get_result() is not None
                 callback_called = True
                 flag.set()
 
-        pubsub = SqliteCloudPubSub()
-        type = SQCLOUD_PUBSUB_SUBJECT.CHANNEL
+        pubsub = SQLiteCloudPubSub()
+        type = SQLITECLOUD_PUBSUB_SUBJECT.CHANNEL
         channel = "channel" + str(uuid.uuid4())
 
         pubsub.create_channel(connection, channel, if_not_exists=True)
         pubsub.listen(connection, type, channel, assert_callback)
 
         pubsub.set_pubsub_only(connection)
 
         assert not client.is_connected(connection)
         assert pubsub.is_connected(connection)
 
         connection2 = client.open_connection()
-        pubsub2 = SqliteCloudPubSub()
+        pubsub2 = SQLiteCloudPubSub()
         pubsub2.notify_channel(connection2, channel, "message-in-a-bottle")
 
         client.disconnect(connection2)
 
         # wait for callback to be called
         flag.wait(30)
 
@@ -144,23 +144,23 @@
         callback_called = False
         flag = threading.Event()
 
         def assert_callback(conn, result, data):
             nonlocal callback_called
             nonlocal flag
 
-            if isinstance(result, SqliteCloudResultSet):
-                assert result.tag == SQCLOUD_RESULT_TYPE.RESULT_JSON
+            if isinstance(result, SQLiteCloudResultSet):
+                assert result.tag == SQLITECLOUD_RESULT_TYPE.RESULT_JSON
                 assert new_name in result.get_result()
                 assert data == ["somedata"]
                 callback_called = True
                 flag.set()
 
-        pubsub = SqliteCloudPubSub()
-        type = SQCLOUD_PUBSUB_SUBJECT.TABLE
+        pubsub = SQLiteCloudPubSub()
+        type = SQLITECLOUD_PUBSUB_SUBJECT.TABLE
         new_name = "Rock" + str(uuid.uuid4())
 
         pubsub.listen(connection, type, "genres", assert_callback, ["somedata"])
 
         client.exec_query(
             f"UPDATE genres SET Name = '{new_name}' WHERE GenreId = 1;", connection
         )
```

### Comparing `sqlitecloud-0.0.77/tests/integration/test_upload.py` & `sqlitecloud-0.0.78/tests/integration/test_upload.py`

 * *Files identical despite different names*

