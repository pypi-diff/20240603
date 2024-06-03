# Comparing `tmp/intellipandora-1.0.8-py3-none-any.whl.zip` & `tmp/intellipandora-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,32 +1,33 @@
-Zip file size: 97082 bytes, number of entries: 123
--rwxr-xr-x  2.0 unx      173 b- defN 24-May-04 14:02 intellipandora-1.0.8.data/scripts/runner.py
--rw-r--r--  2.0 unx      953 b- defN 24-Jun-01 14:28 ipandora/CHANGELOG
+Zip file size: 98705 bytes, number of entries: 125
+-rwxr-xr-x  2.0 unx      173 b- defN 24-May-04 14:02 intellipandora-1.0.9.data/scripts/runner.py
+-rw-r--r--  2.0 unx     1119 b- defN 24-Jun-02 11:17 ipandora/CHANGELOG
 -rw-r--r--  2.0 unx       93 b- defN 24-Apr-17 02:43 ipandora/__init__.py
 -rw-r--r--  2.0 unx      643 b- defN 24-Apr-20 11:39 ipandora/version.py
 -rw-r--r--  2.0 unx       93 b- defN 24-Apr-17 02:43 ipandora/common/__init__.py
 -rw-r--r--  2.0 unx      826 b- defN 24-May-22 06:33 ipandora/common/dictutils.py
 -rw-r--r--  2.0 unx     3008 b- defN 24-Jun-01 13:16 ipandora/common/mysqlaction.py
 -rw-r--r--  2.0 unx     3605 b- defN 24-May-22 07:02 ipandora/common/stringaction.py
 -rw-r--r--  2.0 unx     3304 b- defN 24-Jun-01 13:16 ipandora/common/systeminfo.py
 -rw-r--r--  2.0 unx     4218 b- defN 24-May-21 01:15 ipandora/common/timeutils.py
+-rw-r--r--  2.0 unx     1546 b- defN 24-Jun-02 11:15 ipandora/common/uuidutils.py
 -rw-r--r--  2.0 unx       93 b- defN 24-Apr-17 02:43 ipandora/conf/__init__.py
 -rw-r--r--  2.0 unx      396 b- defN 24-Jun-01 13:13 ipandora/core/__init__.py
 -rw-r--r--  2.0 unx       93 b- defN 24-Apr-17 10:33 ipandora/core/base/__init__.py
 -rw-r--r--  2.0 unx       93 b- defN 24-Apr-17 10:35 ipandora/core/base/classwrap/__init__.py
 -rw-r--r--  2.0 unx     1061 b- defN 24-May-24 23:26 ipandora/core/base/classwrap/attrvaluesplit.py
 -rw-r--r--  2.0 unx     1487 b- defN 24-Apr-20 11:52 ipandora/core/base/classwrap/classproperty.py
 -rw-r--r--  2.0 unx     2787 b- defN 24-May-04 14:02 ipandora/core/base/classwrap/multihandle.py
 -rw-r--r--  2.0 unx      608 b- defN 24-Apr-20 11:49 ipandora/core/base/classwrap/singleton.py
 -rw-r--r--  2.0 unx       95 b- defN 24-Apr-20 11:52 ipandora/core/base/data/__init__.py
 -rw-r--r--  2.0 unx     1155 b- defN 24-Apr-19 04:30 ipandora/core/base/data/markdata.py
 -rw-r--r--  2.0 unx       93 b- defN 24-Apr-17 10:39 ipandora/core/base/loglib/__init__.py
 -rw-r--r--  2.0 unx      995 b- defN 24-May-05 01:23 ipandora/core/base/loglib/log.py
 -rw-r--r--  2.0 unx       95 b- defN 24-May-23 02:07 ipandora/core/base/repository/__init__.py
--rw-r--r--  2.0 unx     4691 b- defN 24-Jun-01 13:46 ipandora/core/base/repository/baserepository.py
+-rw-r--r--  2.0 unx     6912 b- defN 24-Jun-02 11:01 ipandora/core/base/repository/baserepository.py
 -rw-r--r--  2.0 unx       95 b- defN 24-Apr-20 11:53 ipandora/core/engine/__init__.py
 -rw-r--r--  2.0 unx       95 b- defN 24-May-21 16:13 ipandora/core/engine/crypto/__init__.py
 -rw-r--r--  2.0 unx     3997 b- defN 24-Jun-01 13:19 ipandora/core/engine/crypto/aescryptographer.py
 -rw-r--r--  2.0 unx     2229 b- defN 24-Jun-01 13:19 ipandora/core/engine/crypto/crypto.py
 -rw-r--r--  2.0 unx      285 b- defN 24-May-22 07:18 ipandora/core/engine/crypto/cryptoabc.py
 -rw-r--r--  2.0 unx     2804 b- defN 24-Jun-01 13:19 ipandora/core/engine/crypto/fercryptographer.py
 -rw-r--r--  2.0 unx     3898 b- defN 24-Jun-01 13:19 ipandora/core/engine/crypto/rsacryptographer.py
@@ -34,34 +35,35 @@
 -rw-r--r--  2.0 unx      497 b- defN 24-Jun-01 13:24 ipandora/core/engine/generator/model/__init__.py
 -rw-r--r--  2.0 unx       94 b- defN 24-Apr-29 08:25 ipandora/core/engine/generator/model/data/__init__.py
 -rw-r--r--  2.0 unx       94 b- defN 24-May-24 16:46 ipandora/core/engine/generator/model/data/moduledata.py
 -rw-r--r--  2.0 unx     1969 b- defN 24-May-03 01:38 ipandora/core/engine/generator/model/data/robotcase.py
 -rw-r--r--  2.0 unx     3078 b- defN 24-May-24 00:47 ipandora/core/engine/generator/model/data/robotcaselegacy.py
 -rw-r--r--  2.0 unx      798 b- defN 24-May-25 05:33 ipandora/core/engine/generator/model/data/robotsuite.py
 -rw-r--r--  2.0 unx     8941 b- defN 24-Jun-01 13:20 ipandora/core/engine/generator/model/data/robotsuitelegacy.py
--rw-r--r--  2.0 unx     4105 b- defN 24-Jun-01 01:07 ipandora/core/engine/generator/model/data/testcase.py
+-rw-r--r--  2.0 unx     4450 b- defN 24-Jun-02 10:58 ipandora/core/engine/generator/model/data/testcase.py
 -rw-r--r--  2.0 unx       95 b- defN 24-Apr-28 09:00 ipandora/core/engine/generator/model/handler/__init__.py
 -rw-r--r--  2.0 unx     3412 b- defN 24-Jun-01 13:21 ipandora/core/engine/generator/model/handler/robotrenderer.py
 -rw-r--r--  2.0 unx     1932 b- defN 24-Jun-01 13:21 ipandora/core/engine/generator/model/handler/robotrendererlegacy.py
 -rw-r--r--  2.0 unx       95 b- defN 24-Apr-28 09:00 ipandora/core/engine/generator/provider/__init__.py
 -rw-r--r--  2.0 unx      825 b- defN 24-May-02 12:33 ipandora/core/engine/generator/provider/caseprovider.py
 -rw-r--r--  2.0 unx      838 b- defN 24-May-23 02:02 ipandora/core/engine/generator/provider/robotbaseprovider.py
 -rw-r--r--  2.0 unx     2854 b- defN 24-Jun-01 13:24 ipandora/core/engine/generator/provider/robotprovider.py
 -rw-r--r--  2.0 unx       95 b- defN 24-May-22 09:30 ipandora/core/engine/generator/repository/__init__.py
--rw-r--r--  2.0 unx     1418 b- defN 24-Jun-01 13:24 ipandora/core/engine/generator/repository/modulerepository.py
--rw-r--r--  2.0 unx     1496 b- defN 24-Jun-01 13:24 ipandora/core/engine/generator/repository/projectrepository.py
--rw-r--r--  2.0 unx     1708 b- defN 24-Jun-01 13:24 ipandora/core/engine/generator/repository/submodulerepository.py
--rw-r--r--  2.0 unx     2450 b- defN 24-Jun-01 13:24 ipandora/core/engine/generator/repository/tagcategoryrepository.py
--rw-r--r--  2.0 unx     3131 b- defN 24-Jun-01 13:24 ipandora/core/engine/generator/repository/tagrepository.py
--rw-r--r--  2.0 unx    12370 b- defN 24-Jun-01 13:24 ipandora/core/engine/generator/repository/testcaserepository.py
--rw-r--r--  2.0 unx     2788 b- defN 24-Jun-01 13:24 ipandora/core/engine/generator/repository/testcasetagsrepository.py
--rw-r--r--  2.0 unx     2568 b- defN 24-Jun-01 13:24 ipandora/core/engine/generator/repository/teststeprepository.py
+-rw-r--r--  2.0 unx     1084 b- defN 24-Jun-02 11:02 ipandora/core/engine/generator/repository/modulerepository.py
+-rw-r--r--  2.0 unx     1122 b- defN 24-Jun-02 11:02 ipandora/core/engine/generator/repository/projectrepository.py
+-rw-r--r--  2.0 unx     1329 b- defN 24-Jun-02 11:07 ipandora/core/engine/generator/repository/submodulerepository.py
+-rw-r--r--  2.0 unx     2120 b- defN 24-Jun-02 11:07 ipandora/core/engine/generator/repository/tagcategoryrepository.py
+-rw-r--r--  2.0 unx     2584 b- defN 24-Jun-02 11:07 ipandora/core/engine/generator/repository/tagrepository.py
+-rw-r--r--  2.0 unx     1934 b- defN 24-Jun-02 11:07 ipandora/core/engine/generator/repository/testcaseattachment.py
+-rw-r--r--  2.0 unx    11804 b- defN 24-Jun-02 11:07 ipandora/core/engine/generator/repository/testcaserepository.py
+-rw-r--r--  2.0 unx     2663 b- defN 24-Jun-02 11:07 ipandora/core/engine/generator/repository/testcasetagsrepository.py
+-rw-r--r--  2.0 unx     2314 b- defN 24-Jun-02 11:07 ipandora/core/engine/generator/repository/teststeprepository.py
 -rw-r--r--  2.0 unx       95 b- defN 24-May-24 01:36 ipandora/core/engine/generator/service/__init__.py
 -rw-r--r--  2.0 unx     2813 b- defN 24-Jun-01 13:24 ipandora/core/engine/generator/service/robotcaseservice.py
--rw-r--r--  2.0 unx     9692 b- defN 24-Jun-01 13:24 ipandora/core/engine/generator/service/testcaseserivce.py
+-rw-r--r--  2.0 unx    11131 b- defN 24-Jun-02 11:00 ipandora/core/engine/generator/service/testcaseserivce.py
 -rw-r--r--  2.0 unx      314 b- defN 24-May-04 14:02 ipandora/core/plugin/__init__.py
 -rw-r--r--  2.0 unx     1038 b- defN 24-May-04 14:26 ipandora/core/plugin/innerplugin.py
 -rw-r--r--  2.0 unx     1169 b- defN 24-May-04 14:02 ipandora/core/plugin/pluginmanager.py
 -rw-r--r--  2.0 unx     3045 b- defN 24-May-04 14:02 ipandora/core/plugin/specificationsbuilder.py
 -rw-r--r--  2.0 unx      411 b- defN 24-May-04 14:02 ipandora/core/plugin/interface/__init__.py
 -rw-r--r--  2.0 unx      231 b- defN 24-May-04 14:02 ipandora/core/plugin/interface/endpointsinterface.py
 -rw-r--r--  2.0 unx      235 b- defN 24-May-04 14:02 ipandora/core/plugin/interface/httpregisterinterface.py
@@ -111,15 +113,15 @@
 -rw-r--r--  2.0 unx     1805 b- defN 24-May-04 14:02 ipandora/utils/importpath.py
 -rw-r--r--  2.0 unx     3269 b- defN 24-Jun-01 13:12 ipandora/utils/log.py
 -rw-r--r--  2.0 unx     2408 b- defN 24-Apr-17 03:25 ipandora/utils/match.py
 -rw-r--r--  2.0 unx      521 b- defN 24-Apr-17 05:38 ipandora/utils/niceline.py
 -rw-r--r--  2.0 unx     3650 b- defN 24-Jun-01 13:16 ipandora/utils/pathutils.py
 -rw-r--r--  2.0 unx     4769 b- defN 24-Jun-01 13:16 ipandora/utils/robotlogparser.py
 -rw-r--r--  2.0 unx     2183 b- defN 24-Apr-19 14:34 ipandora/utils/variable.py
--rw-r--r--  2.0 unx      479 b- defN 24-Jun-01 14:29 intellipandora-1.0.8.dist-info/AUTHORS.rst
--rw-r--r--  2.0 unx    11342 b- defN 24-Jun-01 14:29 intellipandora-1.0.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     3471 b- defN 24-Jun-01 14:29 intellipandora-1.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jun-01 14:29 intellipandora-1.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       55 b- defN 24-Jun-01 14:29 intellipandora-1.0.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 24-Jun-01 14:29 intellipandora-1.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    12147 b- defN 24-Jun-01 14:29 intellipandora-1.0.8.dist-info/RECORD
-123 files, 241746 bytes uncompressed, 77162 bytes compressed:  68.1%
+-rw-r--r--  2.0 unx      479 b- defN 24-Jun-02 11:18 intellipandora-1.0.9.dist-info/AUTHORS.rst
+-rw-r--r--  2.0 unx    11342 b- defN 24-Jun-02 11:18 intellipandora-1.0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3680 b- defN 24-Jun-02 11:18 intellipandora-1.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Jun-02 11:18 intellipandora-1.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       55 b- defN 24-Jun-02 11:18 intellipandora-1.0.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-Jun-02 11:18 intellipandora-1.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    12354 b- defN 24-Jun-02 11:18 intellipandora-1.0.9.dist-info/RECORD
+125 files, 246904 bytes uncompressed, 78451 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -1,8 +1,8 @@
-Filename: intellipandora-1.0.8.data/scripts/runner.py
+Filename: intellipandora-1.0.9.data/scripts/runner.py
 Comment: 
 
 Filename: ipandora/CHANGELOG
 Comment: 
 
 Filename: ipandora/__init__.py
 Comment: 
@@ -24,14 +24,17 @@
 
 Filename: ipandora/common/systeminfo.py
 Comment: 
 
 Filename: ipandora/common/timeutils.py
 Comment: 
 
+Filename: ipandora/common/uuidutils.py
+Comment: 
+
 Filename: ipandora/conf/__init__.py
 Comment: 
 
 Filename: ipandora/core/__init__.py
 Comment: 
 
 Filename: ipandora/core/base/__init__.py
@@ -153,14 +156,17 @@
 
 Filename: ipandora/core/engine/generator/repository/tagcategoryrepository.py
 Comment: 
 
 Filename: ipandora/core/engine/generator/repository/tagrepository.py
 Comment: 
 
+Filename: ipandora/core/engine/generator/repository/testcaseattachment.py
+Comment: 
+
 Filename: ipandora/core/engine/generator/repository/testcaserepository.py
 Comment: 
 
 Filename: ipandora/core/engine/generator/repository/testcasetagsrepository.py
 Comment: 
 
 Filename: ipandora/core/engine/generator/repository/teststeprepository.py
@@ -342,29 +348,29 @@
 
 Filename: ipandora/utils/robotlogparser.py
 Comment: 
 
 Filename: ipandora/utils/variable.py
 Comment: 
 
-Filename: intellipandora-1.0.8.dist-info/AUTHORS.rst
+Filename: intellipandora-1.0.9.dist-info/AUTHORS.rst
 Comment: 
 
-Filename: intellipandora-1.0.8.dist-info/LICENSE
+Filename: intellipandora-1.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: intellipandora-1.0.8.dist-info/METADATA
+Filename: intellipandora-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: intellipandora-1.0.8.dist-info/WHEEL
+Filename: intellipandora-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: intellipandora-1.0.8.dist-info/entry_points.txt
+Filename: intellipandora-1.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: intellipandora-1.0.8.dist-info/top_level.txt
+Filename: intellipandora-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: intellipandora-1.0.8.dist-info/RECORD
+Filename: intellipandora-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ipandora/CHANGELOG

```diff
@@ -1,7 +1,13 @@
+v1.0.9
+==============
+* update BaseRepository, generate_insert_query and generate_update_query
+* refactory BaseRepository.execute_with_transaction
+* add UUIDFactory
+
 v1.0.8
 ==============
 * add architecture for the framework
 
 v1.0.7
 ==============
 * add common libraries -- timeutils, fileutils, stringutils
```

## ipandora/core/base/repository/baserepository.py

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 @Author: Shao Feng
 @File  : baserepository.py
 @Time  : 2024-05-23
 """
-from typing import Any, Optional
+from typing import Any, Optional, Tuple
 from pymysql.connections import Connection
 from pymysql.err import MySQLError
 from ipandora.common.mysqlaction import MysqlAction
 from ipandora.common.timeutils import TimeUtils
 from ipandora.core.schedule.runtime import Runtime
 from ipandora.utils.log import logger
 
@@ -48,26 +48,25 @@
     def execute_update(self, query: str, params: tuple = ()) -> int:
         try:
             with MysqlAction(**self.db_config) as mysql:
                 cursor = mysql.connection.cursor()
                 current_time = TimeUtils.get_current_datatime()
                 params_with_modified_by_and_time = params[:-1] + (current_time, self.modified_by,
                                                                   params[-1])
-                print(params_with_modified_by_and_time)
                 cursor.execute(query, params_with_modified_by_and_time)
                 mysql.connection.commit()
                 return cursor.rowcount
         except MySQLError as e:
             logger.error(f"Error executing update: {e}")
             return -1
 
     def start_transaction(self) -> Connection:
         try:
-            mysql = MysqlAction(**self.db_config)
-            mysql.connection.start_transaction()
+            mysql = MysqlAction(**self.db_config).connect()
+            mysql.start_transaction()
             return mysql.connection
         except MySQLError as e:
             logger.error(f"Error starting transaction: {e}")
             raise
 
     @staticmethod
     def commit_transaction(connection: Connection):
@@ -89,42 +88,90 @@
             raise
 
     @staticmethod
     def close_connection(connection: Connection):
         try:
             connection.close()
         except MySQLError as e:
-            logger.error(f"Error closing connection: {e}")
-            raise
+            logger.warning(f"Error closing connection: {e}")
 
     def execute_with_transaction(self, query: str, params: tuple = (),
-                                 connection: Optional[Connection] = None,):
+                                 connection: Optional[Connection] = None
+                                 ) -> Tuple[Optional[Connection], int]:
         """
         Execute SQL query with transaction and handle possible exceptions.
-        :param query:
-        :param params:
-        :param connection:
-        :return:
+        :param query: SQL query string
+        :param params: Parameters to be used in the query
+        :param connection: Optional existing connection of database
+        :return: Connection and result
         """
         is_new_connection = False
         if connection is None:
             connection = self.start_transaction()
+            is_new_connection = True
         try:
             cursor = connection.cursor()
-            cursor.execute(query, params)
-            result = cursor.lastrowid if (
-                query.strip().lower().startswith('insert')) else cursor.rowcount
-            # return connection and result if new connection is created
+
+            # Modify params based on query type
+            if query.strip().lower().startswith('insert'):
+                params_with_modified_by = params + (self.modified_by,)
+                cursor.execute(query, params_with_modified_by)
+                result = cursor.lastrowid
+            elif query.strip().lower().startswith('update'):
+                current_time = TimeUtils.get_current_datatime()
+                params_with_modified_by_and_time = params[:-1] + (current_time, self.modified_by,
+                                                                  params[-1])
+                cursor.execute(query, params_with_modified_by_and_time)
+                result = cursor.rowcount
+            else:
+                cursor.execute(query, params)
+                result = cursor.rowcount
+
+            # Commit if new connection was created
             if is_new_connection:
                 return connection, result
-            else:
-                return None, result
+            return None, result
         except MySQLError as e:
             if is_new_connection:
                 connection.rollback()
                 connection.close()
             logger.error(f"Error in execute_with_transaction: {e}")
             raise
 
+    @staticmethod
+    def _get_fields_and_values(obj, operation= 'insert', exclude_fields=None):
+        exclude_fields = exclude_fields or []
+        fields = []
+        values = []
+        for attr, value in obj.__dict__.items():
+            # Add any other necessary checks or transformations
+            if value is not None and attr not in exclude_fields:
+                if operation == 'update':
+                    fields.append(f"{attr} = %s")
+                elif operation == 'insert':
+                    fields.append(attr)
+                values.append(value)
+        return fields, values
+
+    def generate_insert_query(self, obj, table_name):
+        fields, values = self._get_fields_and_values(obj, 'insert')
+        query = f"""
+            INSERT INTO {table_name} ({', '.join(fields)}, ModifiedBy)
+            VALUES ({', '.join(['%s'] * len(values))}, %s)
+        """
+        return query, values
+
+    def generate_update_query(self, obj, table_name, primary_key_field):
+        fields, values = self._get_fields_and_values(obj, 'update',
+                                                     exclude_fields=[primary_key_field])
+        query = f"""
+            UPDATE {table_name}
+            SET {', '.join(fields)}, UpdatedTime = %s, ModifiedBy = %s
+            WHERE {primary_key_field} = %s
+        """
+        # Add the primary key value to the values list
+        values.extend([obj.__dict__[primary_key_field]])
+        return query, values
+
```

## ipandora/core/engine/generator/model/data/testcase.py

```diff
@@ -173,12 +173,25 @@
     ModuleName: Optional[str]
     SubmoduleID: Optional[int]
     SubmoduleName: Optional[str]
     Description: Optional[str]
     Precondition: Optional[str]
     IsAutomated: bool
     Tags: List[str] = field(default_factory=list)
+    Steps: List[TestStep] = field(default_factory=list)
+    ModifiedBy: Optional[str] = None
+    CreatedTime: Optional[datetime] = None
+    UpdatedTime: Optional[datetime] = None
+
+
+@dataclass
+class TestCaseAttachment:
+    AttachmentID: Optional[int]
+    TestCaseID: int
+    OriginalFileName: str
+    FilePath: str
+    Description: Optional[str]
     ModifiedBy: Optional[str] = None
     CreatedTime: Optional[datetime] = None
     UpdatedTime: Optional[datetime] = None
```

## ipandora/core/engine/generator/repository/modulerepository.py

```diff
@@ -1,39 +1,29 @@
 # -*- coding: utf-8 -*-
 """
 @Author: Shao Feng
 @File  : modulerepository.py
 @Time  : 2024-05-23
 """
 from typing import List
-from ipandora.core.base.classwrap.attrvaluesplit import AttrValueSplit
-from ipandora.core.engine.generator.model.data.testcase import Module, Submodule, SubmoduleUpdate, \
-    ModuleUpdate
+from ipandora.core.engine.generator.model.data.testcase import (Module, Submodule, SubmoduleUpdate,
+                                                                ModuleUpdate)
 from ipandora.core.base.repository.baserepository import BaseRepository
 from ipandora.utils.log import logger
 
 
 class ModuleRepository(BaseRepository):
 
     def get_modules(self) -> List[Module]:
         query = "SELECT * FROM Modules"
         rows = self.execute_query(query)
         return [Module(**row) for row in rows] if rows else []
 
     def insert_module(self, module: Module) -> int:
-        fields, values = AttrValueSplit(module).get_fields_and_values()
-        query = f"""
-            INSERT INTO Module ({', '.join(fields)}, ModifiedBy)
-            VALUES ({', '.join(['%s'] * len(values))}, %s)
-        """
+        query, values = self.generate_insert_query(module, "Module")
         return self.execute_insert(query, tuple(values))
 
     def update_module(self, module_update: ModuleUpdate) -> int:
-        fields, values = AttrValueSplit(module_update, "ModuleID").get_fields_and_values()
-        query = f"""
-            UPDATE Module
-            SET {', '.join(fields)}, UpdatedTime = %s, ModifiedBy = %s
-            WHERE SubmoduleID = %s
-        """
-        values.append(module_update.ModuleID)
+        query, values = self.generate_update_query(module_update, "Module",
+                                                   "ModuleID")
         return self.execute_update(query, tuple(values))
```

## ipandora/core/engine/generator/repository/projectrepository.py

```diff
@@ -16,28 +16,18 @@
 
     def get_projects(self) -> List[Project]:
         query = "SELECT * FROM Projects"
         rows = self.execute_query(query)
         return [Project(**row) for row in rows] if rows else []
 
     def insert_project(self, project: Project) -> int:
-        fields, values = AttrValueSplit(project).get_fields_and_values()
-        query = f"""
-            INSERT INTO Projects ({', '.join(fields)}, ModifiedBy)
-            VALUES ({', '.join(['%s'] * len(values))}, %s)
-        """
+        query, values = self.generate_insert_query(project, "Projects")
         return self.execute_insert(query, tuple(values))
 
     def update_project(self, project_update: ProjectUpdate) -> int:
-        fields, values = AttrValueSplit(project_update, "ProjectID").get_fields_and_values()
-        query = f"""
-            UPDATE Projects
-            SET {', '.join(fields)}, UpdatedTime = %s, ModifiedBy = %s
-            WHERE ProjectID = %s
-        """
-        values.append(project_update.ProjectID)
+        query, values = self.generate_update_query(project_update, "Projects", "ProjectID")
         return self.execute_update(query, tuple(values))
 
 
 if __name__ == '__main__':
     resp = ProjectRepository().get_projects()
     print(resp)
```

## ipandora/core/engine/generator/repository/submodulerepository.py

```diff
@@ -20,23 +20,13 @@
 
     def get_submodules_by_module_id(self, module_id: int) -> List[Submodule]:
         query = "SELECT * FROM Submodules WHERE ModuleID = %s"
         rows = self.execute_query(query % module_id)
         return [Submodule(**row) for row in rows] if rows else []
 
     def insert_submodule(self, submodule: Submodule) -> int:
-        fields, values = AttrValueSplit(submodule).get_fields_and_values()
-        query = f"""
-            INSERT INTO Submodules ({', '.join(fields)}, ModifiedBy)
-            VALUES ({', '.join(['%s'] * len(values))}, %s)
-        """
+        query, values = self.generate_insert_query(submodule, "Submodules")
         return self.execute_insert(query, tuple(values))
 
     def update_submodule(self, submodule_update: SubmoduleUpdate) -> int:
-        fields, values = AttrValueSplit(submodule_update, "SubmoduleID").get_fields_and_values()
-        query = f"""
-            UPDATE Submodules
-            SET {', '.join(fields)}, UpdatedTime = %s, ModifiedBy = %s
-            WHERE SubmoduleID = %s
-        """
-        values.append(submodule_update.SubmoduleID)
-        return self.execute_update(query, tuple(values))
+        query, values = self.generate_update_query(submodule_update, "Submodules", "SubmoduleID")
+        return self.execute_update(query, tuple(values))
```

## ipandora/core/engine/generator/repository/tagcategoryrepository.py

```diff
@@ -31,28 +31,19 @@
 
     def get_tag_categories_by_description(self, description: str) -> List[TagCategory]:
         query = "SELECT * FROM TagCategories WHERE Description LIKE %s"
         rows = self.execute_query(query, (f"%{description}%",))
         return [TagCategory(**row) for row in rows] if rows else []
 
     def insert_tag_category(self, tag_category: TagCategory) -> int:
-        fields, values = AttrValueSplit(tag_category).get_fields_and_values()
-        query = f"""
-            INSERT INTO TagCategories ({', '.join(fields)}, ModifiedBy)
-            VALUES ({', '.join(['%s'] * len(values))}, %s)
-        """
+        query, values = self.generate_insert_query(tag_category, "TagCategories")
         return self.execute_insert(query, tuple(values))
 
     def update_tag_category(self, tag_category_update: TagCategoryUpdate) -> int:
-        fields, values = AttrValueSplit(tag_category_update, "CategoryId").get_fields_and_values()
-        query = f"""
-            UPDATE TagCategories
-            SET {', '.join(fields)}, UpdatedTime = %s, ModifiedBy = %s
-            WHERE CategoryId = %s
-        """
-        values.append(tag_category_update.CategoryId)
+        query, values = self.generate_update_query(tag_category_update, "TagCategories",
+                                                   "CategoryId")
         return self.execute_update(query, tuple(values))
 
 
 if __name__ == '__main__':
     _result = TagCategoryRepository().get_tag_categories()
     print(_result)
```

## ipandora/core/engine/generator/repository/tagrepository.py

```diff
@@ -23,15 +23,14 @@
     def get_tags_by_category_id(self, category_id: int) -> List[Tag]:
         query = "SELECT * FROM Tags WHERE CategoryId = %s"
         rows = self.execute_query(query % category_id)
         return [Tag(**row) for row in rows] if rows else []
 
     def get_tags_by_name(self, tag_name: str) -> List[Tag]:
         query = "SELECT * FROM Tags WHERE TagName = '%s'"
-        print(query % tag_name)
         rows = self.execute_query(query % tag_name)
         return [Tag(**row) for row in rows] if rows else []
 
     def get_tags_by_description(self, description: str) -> List[Tag]:
         query = "SELECT * FROM Tags WHERE Description LIKE %s"
         rows = self.execute_query(query % f"%{description}%")
         return [Tag(**row) for row in rows] if rows else []
@@ -43,37 +42,23 @@
 
     def get_tag_id_by_name(self, tag_name: str) -> Optional[int]:
         query = "SELECT TagID FROM Tags WHERE TagName = %s"
         rows = self.execute_query(query, (tag_name,))
         return rows[0]['TagID'] if rows else None
 
     def insert_tag(self, tag: Tag) -> int:
-        fields, values = AttrValueSplit(tag).get_fields_and_values()
-        query = f"""
-            INSERT INTO Tags ({', '.join(fields)}, ModifiedBy)
-            VALUES ({', '.join(['%s'] * len(values))}, %s)
-        """
+        query, values = self.generate_insert_query(tag, "Tags")
         return self.execute_insert(query, tuple(values))
 
     def update_tag(self, tag: TagUpdate) -> int:
-        fields, values = AttrValueSplit(tag, "TagID").get_fields_and_values()
-        query = f"""
-            UPDATE Tags
-            SET {', '.join(fields)}, UpdatedTime = %s, ModifiedBy = %s
-            WHERE TagID = %s
-        """
-        values.append(tag.TagID)
+        query, values = self.generate_update_query(tag, "Tags", "TagID")
         return self.execute_update(query, tuple(values))
 
     def insert_tag_as_transaction(self, tag: Tag, last_trans: bool = False):
-        fields, values = AttrValueSplit(tag).get_fields_and_values()
-        query = f"""
-            INSERT INTO Tags ({', '.join(fields)}, ModifiedBy)
-            VALUES ({', '.join(['%s'] * len(values))}, %s)
-        """
+        query, values = self.generate_insert_query(tag, "Tags")
         _conn, result = self.execute_with_transaction(query, tuple(values))
         if last_trans:
             self.commit_transaction(_conn)
         return _conn, result
 
 
 if __name__ == '__main__':
```

## ipandora/core/engine/generator/repository/testcaserepository.py

```diff
@@ -96,17 +96,14 @@
                     SELECT COUNT(DISTINCT TagID)
                     FROM TestCaseTags AS innerTCT
                     WHERE innerTCT.TestCaseID = TestCaseTags.TestCaseID
                 )
             ) tct ON tc.TestCaseID = tct.TestCaseID
         """
         rows = self.execute_query(query, tuple(tag_ids + [tag_count]))
-        print(query)
-        print(tuple(tag_ids + [tag_count]))
-        print(rows)
         return [TestCase(**row) for row in rows] if rows else []
 
     def get_test_cases_by_contain_tag_ids(self, tag_ids: List[int]) -> List[TestCase]:
         """
         Get test cases by tag ids, return test cases that contain all the tag ids
         :param tag_ids:
         :return:
@@ -243,46 +240,33 @@
             row = rows[0]
             tags_str = row.pop('Tags', None)
             tags = tags_str.split(', ') if tags_str else []
             return TestCaseFull(**row, Tags=tags)
         return None
 
     def insert_test_case(self, test_case: TestCase) -> int:
-        fields, values = AttrValueSplit(test_case).get_fields_and_values()
-        query = f"""
-            INSERT INTO TestCases ({', '.join(fields)}, ModifiedBy)
-            VALUES ({', '.join(['%s'] * len(values))}, %s)
-        """
+        query, values = self.generate_insert_query(test_case, "TestCases")
         return self.execute_insert(query, tuple(values))
 
     def update_test_case(self, case_update: TestCaseUpdate) -> int:
-        fields, values = AttrValueSplit(case_update, "TestCaseID").get_fields_and_values()
-        query = f"""
-            UPDATE TestCases
-            SET {', '.join(fields)}, UpdatedTime = %s, ModifiedBy = %s
-            WHERE TestCaseID = %s
-        """
-        values.append(case_update.TestCaseID)
+        query, values = self.generate_update_query(case_update, "TestCases",
+                                                   "TestCaseID")
         return self.execute_update(query, tuple(values))
 
     def insert_test_case_as_transaction(self, test_case: TestCase,
                                         connection: Optional[Connection] = None,
                                         last_trans: bool = False):
         """
         Insert test case as transaction.
         :param test_case:
         :param connection:
         :param last_trans:
         :return:
         """
-        fields, values = AttrValueSplit(test_case).get_fields_and_values()
-        query = f"""
-            INSERT INTO TestCases ({', '.join(fields)}, ModifiedBy)
-            VALUES ({', '.join(['%s'] * len(values))}, %s)
-        """
+        query, values = self.generate_insert_query(test_case, "TestCases")
         _conn, result = self.execute_with_transaction(query, tuple(values), connection)
         if last_trans:
             self.commit_transaction(_conn)
         return _conn, result
 
 
 if __name__ == '__main__':
@@ -297,7 +281,8 @@
     # resp3 = TestCaseRepository().get_automated_cases_by_tag_ids([44, 118],
     #                                                             is_automated=False)
     # print(resp3)
     # print(len(resp3))
     resp4 = TestCaseRepository().get_full_cases()
     print(resp4)
     print(len(resp4))
+
```

## ipandora/core/engine/generator/repository/testcasetagsrepository.py

```diff
@@ -26,37 +26,32 @@
 
     def get_test_case_ids_by_tag_id(self, tag_id: int) -> List[int]:
         query = "SELECT TestCaseID FROM TestCaseTags WHERE TagID = %s"
         rows = self.execute_query(query, (tag_id,))
         return [row['TestCaseID'] for row in rows] if rows else []
 
     def insert_test_case_tag(self, test_case_tag: TestCaseTag) -> int:
-        fields, values = AttrValueSplit(test_case_tag).get_fields_and_values()
-        query = f"""
-            INSERT INTO TestCaseTags ({', '.join(fields)}, ModifiedBy)
-            VALUES ({', '.join(['%s'] * len(values))}, %s)
-        """
+        query, values = self.generate_insert_query(test_case_tag, "TestCaseTags")
         return self.execute_insert(query, tuple(values))
 
     def update_test_case_tag(self, test_case_tag: TestCaseTagUpdate) -> int:
-        fields, values = AttrValueSplit(test_case_tag, "TestCaseID").get_fields_and_values()
+        fields, values = self._get_fields_and_values(test_case_tag, "TestCaseID")
         query = f"""
             UPDATE TestCaseTags
             SET {', '.join(fields)}, UpdatedTime = %s, ModifiedBy = %s
             WHERE TestCaseTagID = %s
         """
         values.append(test_case_tag.TestCaseID)
+        query, values = self.generate_update_query(test_case_tag, "TestCaseTags",
+                                                   "TestCaseID")
         return self.execute_update(query, tuple(values))
 
     def insert_test_case_tag_as_transaction(self, test_case_tag: TestCaseTag,
                                             connection: Optional[Connection] = None,
                                             last_trans: bool = False):
-        fields, values = AttrValueSplit(test_case_tag).get_fields_and_values()
-        query = f"""
-            INSERT INTO TestCaseTags ({', '.join(fields)}, ModifiedBy)
-            VALUES ({', '.join(['%s'] * len(values))}, %s)
-        """
+        query, values = self.generate_insert_query(test_case_tag, "TestCaseTags")
         _conn, result = self.execute_with_transaction(query, tuple(values), connection)
         if last_trans:
+            _conn = connection if _conn is None else _conn
             self.commit_transaction(_conn)
         return _conn, result
```

## ipandora/core/engine/generator/repository/teststeprepository.py

```diff
@@ -15,45 +15,37 @@
 class TestStepRepository(BaseRepository):
 
     def get_test_steps(self, test_case_id: int) -> List[TestStep]:
         query = "SELECT * FROM TestSteps WHERE TestCaseID = %s"
         rows = self.execute_query(query % test_case_id)
         return [TestStep(**row) for row in rows] if rows else []
 
+    def get_test_steps_by_case_id(self, test_case_id: int) -> List[TestStep]:
+        query = "SELECT * FROM TestSteps WHERE TestCaseID = %s"
+        rows = self.execute_query(query, (test_case_id,))
+        return [TestStep(**row) for row in rows] if rows else []
+
     def get_latest_step(self, test_case_id: int) -> Optional[TestStep]:
         query = "SELECT * FROM TestSteps WHERE TestCaseID = %s ORDER BY StepNumber DESC LIMIT 1"
         rows = self.execute_query(query, (test_case_id,))
         return TestStep(**rows[0]) if rows else None
 
     def insert_test_step(self, test_step: TestStep) -> int:
-        fields, values = AttrValueSplit(test_step).get_fields_and_values()
-        query = f"""
-                    INSERT INTO TestSteps ({', '.join(fields)}, ModifiedBy)
-                    VALUES ({', '.join(['%s'] * len(values))}, %s)
-                """
+        query, values = self.generate_insert_query(test_step, "TestSteps")
         return self.execute_insert(query, tuple(values))
 
     def update_test_step(self, test_step: TestStepUpdate) -> int:
-        fields, values = AttrValueSplit(test_step, "StepID").get_fields_and_values()
-        query = f"""
-            UPDATE TestSteps
-            SET {', '.join(fields)}, UpdatedTime = %s, ModifiedBy = %s
-            WHERE StepID = %s
-        """
-        values.append(test_step.StepID)
+        query, values = self.generate_update_query(test_step, "TestSteps",
+                                                   "StepID")
         return self.execute_update(query, tuple(values))
 
     def insert_test_step_as_transaction(self, test_step: TestStep,
                                         connection: Optional[Connection] = None,
                                         last_trans: bool = False):
-        fields, values = AttrValueSplit(test_step).get_fields_and_values()
-        query = f"""
-                    INSERT INTO TestSteps ({', '.join(fields)}, ModifiedBy)
-                    VALUES ({', '.join(['%s'] * len(values))}, %s)
-                """
+        query, values = self.generate_insert_query(test_step, "TestSteps")
         _conn, result = self.execute_with_transaction(query, tuple(values), connection)
         if last_trans:
             self.commit_transaction(_conn)
         return _conn, result
 
 
 if __name__ == '__main__':
```

## ipandora/core/engine/generator/service/testcaseserivce.py

```diff
@@ -2,23 +2,24 @@
 """
 @Author: Shao Feng
 @File  : testcaseserivce.py
 @Time  : 2024-05-24
 """
 from typing import List, Optional
 from pymysql.connections import Connection
+from ipandora.common.timeutils import TimeUtils
 from ipandora.core.engine.generator.repository.testcaserepository import TestCaseRepository
 from ipandora.core.engine.generator.repository.teststeprepository import TestStepRepository
 from ipandora.core.engine.generator.repository.tagrepository import TagRepository
 from ipandora.core.engine.generator.repository.testcasetagsrepository import TestCaseTagsRepository
 from ipandora.core.engine.generator.model.data.testcase import (TestCase, TestStep, Tag,
-                                                                 TestCaseTag, TestCaseUpdate,
-                                                                 TestCaseFull)
+                                                                TestCaseTag, TestCaseUpdate,
+                                                                TestCaseFull)
 from ipandora.core.engine.generator.model.data.robotsuite import (RobotSuite, RobotCase,
-                                                                   RobotSettings)
+                                                                  RobotSettings)
 from ipandora.utils.log import logger
 
 
 class TestCaseService:
 
     def __init__(self):
         self.test_case_repo = TestCaseRepository()
@@ -29,53 +30,72 @@
     def get_test_case_by_id(self, test_case_id: int) -> TestCase:
         return self.test_case_repo.get_test_case_by_id(test_case_id)
 
     def get_tags_by_case_id(self, test_case_id: int) -> List[Tag]:
         test_case_tags = self.test_case_tags_repo.get_test_case_tags_by_test_case_id(test_case_id)
         return [self.tag_repo.get_tag_by_id(tag.TagID) for tag in test_case_tags]
 
+    def get_steps_by_case_id(self, test_case_id: int) -> List[TestStep]:
+        return self.test_step_repo.get_test_steps_by_case_id(test_case_id)
+
     def get_test_cases_by_tags(self, tag_names: List[str]) -> List[TestCase]:
+        """
+        Get test cases by tag names. Return test cases that tags exactly the same as the tag ids.
+        :param tag_names:
+        :return:
+        """
         tags = [self.tag_repo.get_tags_by_name(tag_name) for tag_name in tag_names]
         tag_ids = [tag[0].TagID for tag in tags if tag]
         if not tag_ids:
             return []
-        return self.test_case_repo.get_test_cases_by_contain_tag_ids(tag_ids)
+        return self.test_case_repo.get_test_cases_by_exact_tag_ids(tag_ids)
 
-    def get_automated_test_cases_by_tags(self, tag_names: List[str]) -> List[TestCase]:
+    def get_test_cases_contain_tags(self, tag_names: List[str]) -> List[TestCase]:
+        """
+        Get test cases by tag names. Return test cases that tags contain the tag ids.
+        :param tag_names:
+        :return:
+        """
         tags = [self.tag_repo.get_tags_by_name(tag_name) for tag_name in tag_names]
         tag_ids = [tag[0].TagID for tag in tags if tag]
         if not tag_ids:
             return []
-        return self.test_case_repo.get_automated_cases_by_tag_ids(tag_ids, True)
+        return self.test_case_repo.get_test_cases_by_contain_tag_ids(tag_ids)
 
-    def get_test_cases_by_contain_tags(self, tag_names: List[str]) -> List[TestCase]:
+    def get_automated_test_cases_by_tags(self, tag_names: List[str]) -> List[TestCase]:
         tags = [self.tag_repo.get_tags_by_name(tag_name) for tag_name in tag_names]
         tag_ids = [tag[0].TagID for tag in tags if tag]
         if not tag_ids:
             return []
-        return self.test_case_repo.get_test_cases_by_contain_tag_ids(tag_ids)
+        return self.test_case_repo.get_automated_cases_by_tag_ids(tag_ids, True)
+
+    def get_full_case_by_id(self, test_case_id: int) -> TestCaseFull:
+        _steps_obj = self.get_steps_by_case_id(test_case_id)
+        _full_case_obj = self.test_case_repo.get_full_case_by_id(test_case_id)
+        _full_case_obj.Steps = _steps_obj
+        return _full_case_obj
 
     def get_full_cases_by_tag(self, tag_name: str) -> List[TestCaseFull]:
         _tag_id = self.tag_repo.get_tag_id_by_name(tag_name)
         if not _tag_id:
             return []
         _case_id_list = self.test_case_tags_repo.get_test_case_ids_by_tag_id(_tag_id)
         if not _case_id_list:
             return []
-        return [self.test_case_repo.get_full_case_by_id(_case_id)
+        return [self.get_full_case_by_id(_case_id)
                 for _case_id in _case_id_list]
 
     def get_automated_full_cases_by_tag(self, tag_name: str) -> List[TestCaseFull]:
         _tag_id = self.tag_repo.get_tag_id_by_name(tag_name)
         if not _tag_id:
             return []
         _case_id_list = self.test_case_repo.get_automated_case_id_by_tag_id(_tag_id)
         if not _case_id_list:
             return []
-        return [self.test_case_repo.get_full_case_by_id(_case_id)
+        return [self.get_full_case_by_id(_case_id)
                 for _case_id in _case_id_list]
 
     def add_testcase(self, test_case: TestCase) -> int:
         test_case_id = self.test_case_repo.insert_test_case(test_case)
         logger.info(f"Test case inserted with ID: {test_case_id}")
         return test_case_id
 
@@ -112,105 +132,103 @@
                 return latest_step.StepNumber
             return 0
         except Exception as e:
             logger.error(f"Error getting latest step number for case {test_case_id}: {e}")
             raise e
 
     def create_test_case(self, test_case: TestCase, steps: List[TestStep],
-                         tags: List[TestCaseTag]) -> bool:
+                         tags: List[str]) -> bool:
         _connection: Optional[Connection] = None
+        _test_case_id = -1
         try:
             # add case with transaction.
+            logger.info("Start to create test case.")
             _connection, _test_case_id = self.test_case_repo.insert_test_case_as_transaction(
                 test_case)
             if _test_case_id == -1:
+                logger.warning("Failed to insert test case. Rollback transaction.")
                 self.test_case_repo.close_connection(_connection)
                 raise Exception("Failed to insert test case")
 
             # add test steps.
+            logger.info("Start to add test steps.")
             for step in steps:
                 step.TestCaseID = _test_case_id
-                _, _step_ids = self.test_step_repo.insert_test_step_as_transaction(step, _connection)
+                _, _step_ids = self.test_step_repo.insert_test_step_as_transaction(step,
+                                                                                   _connection)
                 if _step_ids == -1:
-                    # self.test_step_repo.close_connection(connection)
+                    logger.warning("Failed to insert test step. Rollback transaction.")
                     raise Exception("Failed to insert test step")
-            # add tags and the last one will commit.
-            for i, tag in enumerate(tags):
-                tag.TestCaseID = _test_case_id
+            # generated TagCase object and add tags; the last one will commit.
+            logger.info("Start to add tags.")
+            for i, tag_name in enumerate(tags):
+                _tag_id = self.tag_repo.get_tag_id_by_name(tag_name)
+                if not _tag_id:
+                    logger.warning(f"No tags found with the provided names: <{tag_name}>.")
+                    if i == len(tags) - 1:
+                        self.test_case_repo.commit_transaction(_connection)
+                    continue
+                tag_case_obj = TestCaseTag(TestCaseID=_test_case_id, TagID=_tag_id)
                 if i == len(tags) - 1:
+                    logger.info("This is the last sql statement, commit transaction.")
                     _, _tag_case_id = self.test_case_tags_repo.insert_test_case_tag_as_transaction(
-                        tag, _connection, True)
+                        tag_case_obj, _connection, True)
                     if _tag_case_id == -1:
-                        # self.test_case_tags_repo.close_connection(connection)
+                        logger.warning("Failed to insert test case tag(last). Rollback transaction.")
                         raise Exception("Failed to insert test case tag")
                 else:
                     _, _tag_case_id = self.test_case_tags_repo.insert_test_case_tag_as_transaction(
-                        tag, _connection)
+                        tag_case_obj, _connection)
                     if _tag_case_id == -1:
+                        logger.warning("Failed to insert test case tag. Rollback transaction.")
                         # self.test_case_tags_repo.close_connection(connection)
                         raise Exception("Failed to insert test case tag")
-            return True
         except Exception as e:
             if _connection:
                 # rollback transaction
+                logger.warning("Start to Rollback transaction.")
                 self.test_case_repo.rollback_transaction(_connection)
             logger.error(f"Error creating test case: {e}")
             return False
         finally:
             if _connection:
-                _connection.close()
+                self.test_case_repo.close_connection(_connection)
+            return _test_case_id
 
 
 if __name__ == '__main__':
     from ipandora.core.engine.generator.model.data.testcase import TestCase
-    # 创建服务实例
+    # # create service
     test_case_service = TestCaseService()
-    result = test_case_service.get_full_cases_by_tag('G40')
-    print(result)
-    result = test_case_service.get_automated_full_cases_by_tag('G40')
-    print(result)
-
-    # # 创建一个测试用例对象
-    # new_test_case = TestCase(
-    #     TestCaseID=None,
-    #     SubmoduleID=11,
-    #     Title="Test Case Title Shaft 006",
-    #     Description="Test Case Description Shaft 006",
-    #     Precondition="Precondition Shaft 006",
-    #     IsAutomated=True,
-    # )
-    # print(new_test_case)
-    # _case_id = test_case_service.add_testcase(new_test_case)
-    # print(f"New test case ID: {_case_id}")
-    #
-    # modify_test = TestCaseUpdate(
-    #     TestCaseID=_case_id,
-    #     SubmoduleID=None,
-    #     Title="Test Case Title Shaft 006, Modified222",
-    #     Description=None,
-    #     Precondition=None,
-    #     IsAutomated=True,
-    # )
-    # print(modify_test)
-    # test_case_service.modify_test_case(modify_test)
-
-    # # add test steps and tags
-    # test_case_service.add_tags_to_case(_case_id, ['smoke', 'G00', 'generator'])
-
-    # _test_step1 = TestStep(
-    #     StepID=None,
-    #     TestCaseID=None,
-    #     StepDescription="Test Step Description Shaft 005 - 001",
-    #     StepNumber=1,
-    #     ExpectedResult="Expected Result Shaft 005 - 001",
-    # )
-    # test_case_service.add_test_step_to_case(_case_id, _test_step1)
-    #
-    # _test_step2 = TestStep(
-    #     StepID=None,
-    #     TestCaseID=None,
-    #     StepDescription="Test Step Description Shaft 005 - 002",
-    #     StepNumber=1,
-    #     ExpectedResult="Expected Result Shaft 005 - 002",
-    # )
-    #
-    # test_case_service.add_test_step_to_case(7, _test_step1)
+    # result = test_case_service.get_full_cases_by_tag('G40')
+    # print(result)
+    # result = test_case_service.get_automated_full_cases_by_tag('G40')
+    # print(result)
+
+    # 创建一个测试用例对象
+    new_test_case = TestCase(
+        TestCaseID=None,
+        SubmoduleID=11,
+        Title="Test Case Title Shaft 006",
+        Description="Test Case Description Shaft 006",
+        Precondition="Precondition Shaft 006",
+        IsAutomated=True,
+    )
+    print(new_test_case)
+    # create steps
+    _steps = []
+    for _i in range(1, 6):
+        _timestamp = TimeUtils.get_current_timestamp_ms()
+        _test_step = TestStep(
+            StepID=None,
+            TestCaseID=None,
+            StepDescription=f"Test Step Description Shaft create 00{_i} - {_timestamp}",
+            StepNumber=_i,
+            ExpectedResult=f"Expected Result Shaft create- 00{_i}",
+        )
+        _steps.append(_test_step)
+    # test_case_service.add_test_step_to_case(_case_id, _test_step3)
+    _new_case_id = test_case_service.create_test_case(new_test_case, _steps,
+                                                      ['smoke', 'G00', 'document'])
+    print(_new_case_id)
+    _full_case = test_case_service.get_full_case_by_id(_new_case_id)
+    print(_full_case)
```

## Comparing `intellipandora-1.0.8.dist-info/LICENSE` & `intellipandora-1.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `intellipandora-1.0.8.dist-info/METADATA` & `intellipandora-1.0.9.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intellipandora
-Version: 1.0.8
+Version: 1.0.9
 Summary: Generic automation framework for system testing and model evaluation
 Home-page: https://github.com/Conan-Shao/IntelliPandora
 Author: Shao Feng
 Author-email: just.shao.007@gmail.com
 License: Apache License 2.0
 Keywords: intellipandora
 Classifier: Development Status :: 4 - Beta
@@ -82,24 +82,32 @@
 ### 使用手册(待添加)
 > 包含了框架使用，例如http如何调用，用于接口自动化测试
 * [IntelliPandora使用手册](docs/usr/user_guider.md)
 
 
 ## 三、开发
 * [IntelliPandora开发说明](docs/dev/IntelliPandora_Dev.md)
-* 
+
 ### **3.1 框架结构介绍**
 > 代码都在***src/intellipandora***
 * **core**: 提供自动化核心能力接口。
   * **base**: 基础类(基类)，如SingletonClass、BaseRepository等
   * **protocol**: 提供协议能力，支持与被测对象交互/通信。如http、grpc、websocket等
   * **engine**: 提供执行引擎，提供框架核心功能，如自动生成、加密、分布式执行处理等
 * **common**: 基础方法封装，支持自动化测试断言、数据准备、数据处理等
 * **run**: 框架的命令行模块
 * **utils**: 框架基础功能，如log、error...
 * **conf**: 配置文件
 
+### **3.2 框架设计**
+
+* **架构图**
+  ![IntelliPandora架构图](./docs/dev/static/framework_architecture.jpg)
+
+* **业务流程图**
+![IntelliPandora业务流程图](./docs/dev/static/business_flow.png)
+
 
 ## GitHub Feature
 
 1. You can use Readme\_XXX.md to support different languages, such as Readme\_en.md, Readme\_zh.md
 2. Explore open source project [IntelliPandora](https://github.com/Conan-Shao/IntelliPandora)
```

## Comparing `intellipandora-1.0.8.dist-info/RECORD` & `intellipandora-1.0.9.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,32 @@
-intellipandora-1.0.8.data/scripts/runner.py,sha256=PY1i5YDyMo6NpEajxWwGfO3NlvP47NcAVP-lgI2cigY,173
-ipandora/CHANGELOG,sha256=WFWLR3q6wpVT1VVFx_6q75M1CJTGsOBrKm1sdaAuthk,953
+intellipandora-1.0.9.data/scripts/runner.py,sha256=PY1i5YDyMo6NpEajxWwGfO3NlvP47NcAVP-lgI2cigY,173
+ipandora/CHANGELOG,sha256=pPT9hyeJqNRg4Qg5XkyeV0g5oHjLPxoqQrI4hqFLZ90,1119
 ipandora/__init__.py,sha256=E5O_DsKDHoEyLVSq0z28FbuviMrBGUxHYLcZwAa_mrQ,93
 ipandora/version.py,sha256=sH31l0BYCiRZ137xEQIoFhJbEhocRHJoTPq9uNNlwt0,643
 ipandora/common/__init__.py,sha256=Y5poEhdll69EYWO4FC-FkPA_0bRJhWCojeOiEOuTugw,93
 ipandora/common/dictutils.py,sha256=A-aIFawYvwCI52tA9Xd3ddesJdereKm44OS0_WVaAes,826
 ipandora/common/mysqlaction.py,sha256=VCCs09TusSRGUfDO5bVMfInJKzcqhgWUAw4ihCvy94Q,3008
 ipandora/common/stringaction.py,sha256=Nc33hzabwO7fHHlYjh2RiE_TWSdr0iFVk0Je2RwUkRI,3605
 ipandora/common/systeminfo.py,sha256=0-fYqK_pkiK2MWcksuB0GLGxmdsD80RPsICjj1eyAY4,3304
 ipandora/common/timeutils.py,sha256=EW4h7KQRkEBvmbjOBtLybMPjoSdUEMrMF0oYnmI7_pc,4218
+ipandora/common/uuidutils.py,sha256=4uDkUDzNN5drDsyT1QMCZNOV3xXABDbF2ceaCpuWH6E,1546
 ipandora/conf/__init__.py,sha256=Y5poEhdll69EYWO4FC-FkPA_0bRJhWCojeOiEOuTugw,93
 ipandora/core/__init__.py,sha256=vZgX0fLc3ju1z_Whmg8qz3-dwuziz_wbCkRGfufTgKQ,396
 ipandora/core/base/__init__.py,sha256=Y5poEhdll69EYWO4FC-FkPA_0bRJhWCojeOiEOuTugw,93
 ipandora/core/base/classwrap/__init__.py,sha256=Y5poEhdll69EYWO4FC-FkPA_0bRJhWCojeOiEOuTugw,93
 ipandora/core/base/classwrap/attrvaluesplit.py,sha256=Vsjh-x65LUZEd9ogQjjr6DxR1XkNHNAwSIQlTz00xnY,1061
 ipandora/core/base/classwrap/classproperty.py,sha256=24A6bnry6nC8bcpKG2X2so6bOUSB7oYNHvYrRrIO5qA,1487
 ipandora/core/base/classwrap/multihandle.py,sha256=WHoVK8TjspPjJ6tdWfrdwOL6ON-wounfdYQcjBPDLEY,2787
 ipandora/core/base/classwrap/singleton.py,sha256=r_1SWj0cFzUiUrXRfX3h-2-rTulE1ube3lW8I2637bs,608
 ipandora/core/base/data/__init__.py,sha256=kN56eO5g7PvMHmcdhzuKA2UuzaQBf2ZbCBzmp0WYPI4,95
 ipandora/core/base/data/markdata.py,sha256=NPJCf5KkH5is6TwLCS8fZu1Osx2xA1IZOZY_k-9z-ts,1155
 ipandora/core/base/loglib/__init__.py,sha256=Y5poEhdll69EYWO4FC-FkPA_0bRJhWCojeOiEOuTugw,93
 ipandora/core/base/loglib/log.py,sha256=8FxKjE4skqXPudjLM8v6-WkZPJC1dXdDUV4c_E90MsA,995
 ipandora/core/base/repository/__init__.py,sha256=pB_MW2OvHVyHaGalZCbpk1xJVi_E04t9bFeXp2-pRCk,95
-ipandora/core/base/repository/baserepository.py,sha256=o8c_I0iMI4MHpFDKthS_5LiLOAvVBDl6eRNiqULO940,4691
+ipandora/core/base/repository/baserepository.py,sha256=ZWCgovZ2REZa0emnQBIPzcGetxW0_u-enhGmQSgJMPc,6912
 ipandora/core/engine/__init__.py,sha256=wNPK4pG-Zhm5GaohCQcLVHbCfzzFaaqc0AnZNvi0eYQ,95
 ipandora/core/engine/crypto/__init__.py,sha256=blbxfw0bVwgaNND_ck7NednAuFmPJ29r8_kGc2_d94w,95
 ipandora/core/engine/crypto/aescryptographer.py,sha256=rFA46PAqbKjx45wilLjO3kUrRrn7oI7Lkksaaugv70E,3997
 ipandora/core/engine/crypto/crypto.py,sha256=5LN57O3XbSr2DN-Q659XusMbMI3clA2xJVQGEyv5UAA,2229
 ipandora/core/engine/crypto/cryptoabc.py,sha256=KHRoWs1Ic2n3kixJrxkLEhKdLll_Pz27GB15G7PWBNA,285
 ipandora/core/engine/crypto/fercryptographer.py,sha256=N3uOoTgx6buf9hMJwB7gFyvX1Eu5w9w7uF85Xbfg1Sk,2804
 ipandora/core/engine/crypto/rsacryptographer.py,sha256=Kb75XlrGztQdqufaSQl0CCTyAbE28s5gezFE3odUzrQ,3898
@@ -33,34 +34,35 @@
 ipandora/core/engine/generator/model/__init__.py,sha256=TTddEo3r12HZYiUTYZzWWd_sIyWBe9fWMSk07shH7A8,497
 ipandora/core/engine/generator/model/data/__init__.py,sha256=w0FTd9iMJpAQoYC1z8tLi8_5WUdv2BT-kqq163bAglU,94
 ipandora/core/engine/generator/model/data/moduledata.py,sha256=9w35IZ0amhJsWgG5gGBiiBHTQ0ja7qlT9Zvay2R07c0,94
 ipandora/core/engine/generator/model/data/robotcase.py,sha256=8Gc1NJW4NucJLKjdjekKvjqodhhl_gAmg_O6mdSH2To,1969
 ipandora/core/engine/generator/model/data/robotcaselegacy.py,sha256=c2aT7vjDFHpZFo983zjo7tFPi61h5l0vNinbnh-VS1c,3078
 ipandora/core/engine/generator/model/data/robotsuite.py,sha256=h1lsowZZ58NXwQO88h0vhcOIioYBouxgGpQX1jjpsLY,798
 ipandora/core/engine/generator/model/data/robotsuitelegacy.py,sha256=mjyMYlTHD1DCpE7iaWabsG8SHDMMQiOyuUOc9gpra-w,8941
-ipandora/core/engine/generator/model/data/testcase.py,sha256=jk9Qzfj1M-oT_9jTGdfrMiw7hlaZjEdtjjQdzuMMQxI,4105
+ipandora/core/engine/generator/model/data/testcase.py,sha256=QYIfS3gX6Cg2YsU9p2rHAnEwwiu1YBYXWRTMSrtMz2M,4450
 ipandora/core/engine/generator/model/handler/__init__.py,sha256=DvEZBI8XxHtdB6HDWo_cw8KdMoQtyRx0G9PgWdTJkUI,95
 ipandora/core/engine/generator/model/handler/robotrenderer.py,sha256=20nReXjdLh6yoyO9oumroAwrNBEx5Z6MLhQn_PsYKEI,3412
 ipandora/core/engine/generator/model/handler/robotrendererlegacy.py,sha256=RT0BohHmN8MHCHqSxpytqhOV56lVmNc2bpDClttVRaE,1932
 ipandora/core/engine/generator/provider/__init__.py,sha256=DvEZBI8XxHtdB6HDWo_cw8KdMoQtyRx0G9PgWdTJkUI,95
 ipandora/core/engine/generator/provider/caseprovider.py,sha256=4RKSJxbMUO1jFnGTOpMY9PdDJ7YekDnWv1b-PNX3UfQ,825
 ipandora/core/engine/generator/provider/robotbaseprovider.py,sha256=HCVSuo1NHf7toI-Uo4h2qtj6oUoLB4iKo-5rjijOjYs,838
 ipandora/core/engine/generator/provider/robotprovider.py,sha256=eHUIyjVZFRnwG500zclftbDXTxxcjWtEGaPgSLP8UfM,2854
 ipandora/core/engine/generator/repository/__init__.py,sha256=blbxfw0bVwgaNND_ck7NednAuFmPJ29r8_kGc2_d94w,95
-ipandora/core/engine/generator/repository/modulerepository.py,sha256=6LAALSz-sg7JRu-qY001LDxBaJLZqYIcwy4FXgzPjRY,1418
-ipandora/core/engine/generator/repository/projectrepository.py,sha256=zg_AbsEx2kmLc38p7Xz7CYY-EzBTK47j_S6bJqQzsgg,1496
-ipandora/core/engine/generator/repository/submodulerepository.py,sha256=crdEyA6n3dS3mQAde48I-3eGOLiw1YzKC28GHh8YlkM,1708
-ipandora/core/engine/generator/repository/tagcategoryrepository.py,sha256=VCGIvlAZyyQqYwFV7AnCY7S1KxPd_W8QQALHEoPzupU,2450
-ipandora/core/engine/generator/repository/tagrepository.py,sha256=oXzub_vQS5KQndCTA9ZlJv_eBP20GjbhC_e6fQ0wWeY,3131
-ipandora/core/engine/generator/repository/testcaserepository.py,sha256=VgQzqkSFZo5m1XjfI9pIjnuBnhOIUQcbDA6P6SZRwAI,12370
-ipandora/core/engine/generator/repository/testcasetagsrepository.py,sha256=MHNO-1BA6efoZZaBLC-2ftEFNEC59Q26520AYPUAJl8,2788
-ipandora/core/engine/generator/repository/teststeprepository.py,sha256=mIUYyBdQ6xuqKm0Vi0vKk2pzsjd9k7DvfgIvm4aEEYg,2568
+ipandora/core/engine/generator/repository/modulerepository.py,sha256=vip57EGAerQonNMdMXXLAE5ywhkoyLdR9YEJT6pba_I,1084
+ipandora/core/engine/generator/repository/projectrepository.py,sha256=QDsmRCHsYRfjXq3r2gT8MEOFiFJjU7wiVzAAOZH4boc,1122
+ipandora/core/engine/generator/repository/submodulerepository.py,sha256=tWJ50MH-G_zPFPgwfKuMOWjCkvp7jZuURsWJrfXO1QA,1329
+ipandora/core/engine/generator/repository/tagcategoryrepository.py,sha256=u0WC728JlVzhH2C28U5TJZFFAqMUh7XVTi61zWRfkRQ,2120
+ipandora/core/engine/generator/repository/tagrepository.py,sha256=sTFZCCmn6Vnxa2pRgZxaElNgfHPqpL6robpza2nzotw,2584
+ipandora/core/engine/generator/repository/testcaseattachment.py,sha256=K2gNg_-yE-Lhe8hMtSjU5mypPq7fvMUp2-trTK2VIN8,1934
+ipandora/core/engine/generator/repository/testcaserepository.py,sha256=z0wVLlG-ytbnJhZgGEHENcnWuHJzU7VzNCH3v3tBCrY,11804
+ipandora/core/engine/generator/repository/testcasetagsrepository.py,sha256=lIKRU3A4SdMS5sakDPIVCa40fy41bqrUELGh6ZCY3I0,2663
+ipandora/core/engine/generator/repository/teststeprepository.py,sha256=qqB5XFae9aUhNVdMPEmrZ0u4_xq_vCHlY45xtnXbEM4,2314
 ipandora/core/engine/generator/service/__init__.py,sha256=5qpoXr2BaGPd7DpBvjlVAA8oDIZU2S2YHYY0mcPbaCg,95
 ipandora/core/engine/generator/service/robotcaseservice.py,sha256=YKaD1m5hQQg0eVZGn0zLtsnAFDLlxGyyiUGqdEcliZg,2813
-ipandora/core/engine/generator/service/testcaseserivce.py,sha256=_OroZQk3AStAk2286Q7-4zxHAQIvbyH_ez3CxzC981Q,9692
+ipandora/core/engine/generator/service/testcaseserivce.py,sha256=TKcDP_K8uupl0uUqXgWeC4rbWiVYZhEwbWu1bSN0Ou0,11131
 ipandora/core/plugin/__init__.py,sha256=tHpWtfnDG64k3GDFQYRPuVM7u6gswbdLFl_6mKVvao8,314
 ipandora/core/plugin/innerplugin.py,sha256=5jMV_85IvmSQ0btaeD8DzN2hH7_v9WxZ31V01wTOoAA,1038
 ipandora/core/plugin/pluginmanager.py,sha256=zQ8sNJLVweG7gkLJASG8Ryvcan5eSSIcoHXLFhGvQEc,1169
 ipandora/core/plugin/specificationsbuilder.py,sha256=B0n76SmST6GyRVNusGqEshAW2N9uMCpW0lOD85kASFg,3045
 ipandora/core/plugin/interface/__init__.py,sha256=7C65JZ9J_-KseBNo8MQF9mtQwiFRRxXIZDynxyWOIsw,411
 ipandora/core/plugin/interface/endpointsinterface.py,sha256=jf2Adn2GyaVxs_64ro5oTgK2MF2rJhYOdww2L32T06E,231
 ipandora/core/plugin/interface/httpregisterinterface.py,sha256=btfN6z_MIf4BHoIb9bWZiS_dFFjZexaFKHAWsq0-DNI,235
@@ -110,14 +112,14 @@
 ipandora/utils/importpath.py,sha256=8yDKTlVjwxGETrLmBC6Jccoyirx-JUTy6-5Wp7zhCkk,1805
 ipandora/utils/log.py,sha256=eWhReua7bBuSEbnfRQM1WADjO8YUbHmC-9hbama2jHI,3269
 ipandora/utils/match.py,sha256=42mLplqpxF_NFDPSGxhztBow3WaVbPWnVQ9LJGQhPdI,2408
 ipandora/utils/niceline.py,sha256=w_VIC_i6rmC0r5uaE_lxef0kEy9mfkYUn7wqYBzQkFY,521
 ipandora/utils/pathutils.py,sha256=GpmnARi_OiqdQQQRopiikLRHkhAuVplDDrRwv7NmA5k,3650
 ipandora/utils/robotlogparser.py,sha256=ybqwG0vVEu9Vf6yDDbBDt7RyTVVvTk_HTC-pxK8ToqE,4769
 ipandora/utils/variable.py,sha256=DPGdOa2Zf8aZJgXZBv0yETfjgqMe7UI8I_4BYToqv8M,2183
-intellipandora-1.0.8.dist-info/AUTHORS.rst,sha256=FKR3o3pakwdsG63888OhufBDR4E-GKQmpVDsL7HOCdw,479
-intellipandora-1.0.8.dist-info/LICENSE,sha256=t-0geih-ExGDCpCpE0YPuwA8pqA3vDt7l76v0jXiGo4,11342
-intellipandora-1.0.8.dist-info/METADATA,sha256=xl1IQ6iPRsJH41J-ZJEMAJAxJvEURW9QMkFQpbfY7YQ,3471
-intellipandora-1.0.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-intellipandora-1.0.8.dist-info/entry_points.txt,sha256=pw27C7OcHWLb7to_EkzyC9uc3Fdg8_pUrjjQ1kNQtfE,55
-intellipandora-1.0.8.dist-info/top_level.txt,sha256=bTT1b-jSKiifyEy34Li89A7IZQ3Q8oYjxB3bRGi9i0g,9
-intellipandora-1.0.8.dist-info/RECORD,,
+intellipandora-1.0.9.dist-info/AUTHORS.rst,sha256=FKR3o3pakwdsG63888OhufBDR4E-GKQmpVDsL7HOCdw,479
+intellipandora-1.0.9.dist-info/LICENSE,sha256=t-0geih-ExGDCpCpE0YPuwA8pqA3vDt7l76v0jXiGo4,11342
+intellipandora-1.0.9.dist-info/METADATA,sha256=NHhJTx0ViCWs2V_d3NsKu1mx6IRYharidu6-7T6j01o,3680
+intellipandora-1.0.9.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+intellipandora-1.0.9.dist-info/entry_points.txt,sha256=pw27C7OcHWLb7to_EkzyC9uc3Fdg8_pUrjjQ1kNQtfE,55
+intellipandora-1.0.9.dist-info/top_level.txt,sha256=bTT1b-jSKiifyEy34Li89A7IZQ3Q8oYjxB3bRGi9i0g,9
+intellipandora-1.0.9.dist-info/RECORD,,
```

