# Comparing `tmp/pyasdb-2024.5.31.3.tar.gz` & `tmp/pyasdb-2024.6.3.1.tar.gz`

## Comparing `pyasdb-2024.5.31.3.tar` & `pyasdb-2024.6.3.1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pyasdb-2024.5.31.3/src/pyasdb/__init__.py
--rw-r--r--   0        0        0     6363 2020-02-02 00:00:00.000000 pyasdb-2024.5.31.3/src/pyasdb/pyasdb.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pyasdb-2024.5.31.3/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pyasdb-2024.5.31.3/LICENSE
--rw-r--r--   0        0        0     7367 2020-02-02 00:00:00.000000 pyasdb-2024.5.31.3/README.md
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 pyasdb-2024.5.31.3/pyproject.toml
--rw-r--r--   0        0        0    48543 2020-02-02 00:00:00.000000 pyasdb-2024.5.31.3/PKG-INFO
+-rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 pyasdb-2024.6.3.1/src/test.db
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 pyasdb-2024.6.3.1/src/pyasdb/__init__.py
+-rw-r--r--   0        0        0     7416 2020-02-02 00:00:00.000000 pyasdb-2024.6.3.1/src/pyasdb/pyasdb.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pyasdb-2024.6.3.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pyasdb-2024.6.3.1/LICENSE
+-rw-r--r--   0        0        0     8145 2020-02-02 00:00:00.000000 pyasdb-2024.6.3.1/README.md
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 pyasdb-2024.6.3.1/pyproject.toml
+-rw-r--r--   0        0        0    49320 2020-02-02 00:00:00.000000 pyasdb-2024.6.3.1/PKG-INFO
```

### Comparing `pyasdb-2024.5.31.3/src/pyasdb/pyasdb.py` & `pyasdb-2024.6.3.1/src/pyasdb/pyasdb.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import shelve
 import atexit
+from threading import Lock
 
 class Query:
     """
     Query Class For Making And Managing Results of Queries.
 
     """
     def __init__(self, table, results):
@@ -63,21 +64,32 @@
 
     def __setitem__(self, key, value):
         """
         :param key(str): primary key of result
         :param key(int): list index of result
         :return:
         """
+        if not isinstance(value, dict):
+            raise TypeError("Value must be a dictionary")
         if isinstance(key, int):
             self.table[self.results[key]] = value
         elif isinstance(key, str):
             self.table[key] = value
         else:
             raise KeyError
 
+    def update(self, key, obj):
+        self.table.update(key, obj)
+
+    def __delitem__(self, key):
+        self.table.__delitem__(key)
+
+    def __contains__(self, key):
+        return key in self.results
+
     def __repr__(self):
         return "<pyasdb.DB.Table.Query: " + self.table.name + " - " + ','.join(self.results) + ">"
 
 
 class Table:
     """Table class for managing individual database tables"""
     def __init__(self, parent, name):
@@ -116,17 +128,36 @@
 
     def __setitem__(self, key, value, sync=False):
         """
         :param key: primary key of entry
         :param value: new contents
         :param sync: boolean specifying to immediately sync if in writeback mode
         """
-        self.parent.shelf['.'.join((self.name, key))] = value
-        if sync:
-            self.parent.sync()
+        if not isinstance(value, dict):
+            raise TypeError("Value must be a dictionary")
+        with self.parent.lock:
+            self.parent.shelf['.'.join((self.name, key))] = value
+            if sync:
+                self.parent.sync()
+
+    def update(self, key, obj):
+        """
+        Applies partial updates without erasing data via the dict.update mechanism
+        :param key: primary key of entry
+        :param obj: dictionary containing new values to be merged with entry
+        """
+        tmpx = self[key]
+        tmpx.update(obj)
+        self[key] = tmpx
+
+    def __delitem__(self, key):
+        del self.parent.shelf['.'.join((self.name, key))]
+
+    def __contains__(self, key):
+        return '.'.join((self.name, key)) in self.parent.shelf
 
     def __iter__(self):
         self.index = 0
         self.parent.tables[self.name] = self
         self.__keycache = self.keys()
         return self
 
@@ -161,14 +192,15 @@
         Database constructor
         :param filename: Path and filename of the database file to use (will append .db to end)
         :param flag: flag passed through to Shelve.open
         :param writeback: Whether to enable writeback mode
         """
         self.shelf = shelve.open(filename, flag, writeback=writeback)
         self.writeback = writeback
+        self.lock = Lock()
 
         tableNames = list(set(map(lambda key: key.split('.')[0], list(self.shelf))))
         self.tables = {}
 
         for table in tableNames:
             self.tables[table] = Table(self, table)
 
@@ -180,16 +212,17 @@
         """
         return list(self.tables.keys())
 
     def sync(self):
         """
         If writeback enabled, manually sync
         """
-        if self.writeback:
-            self.shelf.sync()
+        with self.lock:
+            if self.writeback:
+                self.shelf.sync()
 
     def __getitem__(self, key):
         """
         Returns a Table, will create a new Table if one does not already exist.
         :param key:
         :return:
         """
```

### Comparing `pyasdb-2024.5.31.3/LICENSE` & `pyasdb-2024.6.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyasdb-2024.5.31.3/README.md` & `pyasdb-2024.6.3.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -64,15 +64,16 @@
 - [x] Query Type Checking (to prevent TypeError if field has been assigned different types)
 - [ ] Subfield queries (your lambda can reference subfields, but the query function doesn't check to make sure they 
 exist)
 - [ ] Key type agnosticism (the key in the backend must be a string, but it can be handy to just str() all keys to allow
 different types)
 - [x] Available on PyPi (pip install pyasdb)
 - [x] Add help() data
-- [ ] Add thread safety
+- [x] Add thread safety (automatically includes locks to secure writes)
+- [x] Update Routine that connects to dict.update
 
 ### PyDoc
 ```
 Python Library Documentation: module pyasdb
 
 NAME
     pyasdb
@@ -144,14 +145,23 @@
      |  __repr__(self)
      |      Return repr(self).
      |  
      |  __setitem__(self, key, value)
      |      :param key(str): primary key of result
      |      :param key(int): list index of result
      |      :return:
+     |
+     |  def update(self, key, obj)
+     |      Applies partial updates without erasing data via the dict.update mechanism
+     |      :param key: primary key of entry
+     |      :param obj: dictionary containing new values to be merged with entry
+     |
+     |  def __delitem__(self, key)
+     |
+     |  def __contains__(self, key)
      |  
      |  query(self, field, func, checktype=None)
      |      Make a sub-query and return a new narrower Query object
      |      :param field: the field being searched, will only parse entries that have this field
      |      :param func: a function reference applied to a filter query (ie. lambda x: x > 5)
      |      :param checktype: if passed a type will automatically narrow results to that type to prevent TypeError
      |      :return: A new query object containing the results of the given query
@@ -186,14 +196,23 @@
      |  __repr__(self)
      |      Return repr(self).
      |  
      |  __setitem__(self, key, value, sync=False)
      |      :param key: primary key of entry
      |      :param value: new contents
      |      :param sync: boolean specifying to immediately sync if in writeback mode
+     |
+     |  def update(self, key, obj)
+     |      Applies partial updates without erasing data via the dict.update mechanism
+     |      :param key: primary key of entry
+     |      :param obj: dictionary containing new values to be merged with entry
+     |
+     |  def __delitem__(self, key)
+     |
+     |  def __contains__(self, key)
      |  
      |  keys(self)
      |      Returns a list of primary keys in the Table
      |      :return: list of keys
      |  
      |  query(self, field, func)
      |      Generates an initial query and returns a Query object.
```

### Comparing `pyasdb-2024.5.31.3/pyproject.toml` & `pyasdb-2024.6.3.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyasdb"
-version = "2024.05.31.3"
+version = "2024.06.03.1"
 authors = [
   { name="Shiri Bailem", email="shiri@bailem.me" },
 ]
 description = "A simplified NoSQL offline database built on top of shelve/pickle"
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = ["database", "offline", "NoSQL"]
```

### Comparing `pyasdb-2024.5.31.3/PKG-INFO` & `pyasdb-2024.6.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyasdb
-Version: 2024.5.31.3
+Version: 2024.6.3.1
 Summary: A simplified NoSQL offline database built on top of shelve/pickle
 Project-URL: Homepage, https://github.com/shiribailem/pyasdb
 Project-URL: Issues, https://github.com/shiribailem/pyasdb/issues
 Author-email: Shiri Bailem <shiri@bailem.me>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -754,15 +754,16 @@
 - [x] Query Type Checking (to prevent TypeError if field has been assigned different types)
 - [ ] Subfield queries (your lambda can reference subfields, but the query function doesn't check to make sure they 
 exist)
 - [ ] Key type agnosticism (the key in the backend must be a string, but it can be handy to just str() all keys to allow
 different types)
 - [x] Available on PyPi (pip install pyasdb)
 - [x] Add help() data
-- [ ] Add thread safety
+- [x] Add thread safety (automatically includes locks to secure writes)
+- [x] Update Routine that connects to dict.update
 
 ### PyDoc
 ```
 Python Library Documentation: module pyasdb
 
 NAME
     pyasdb
@@ -834,14 +835,23 @@
      |  __repr__(self)
      |      Return repr(self).
      |  
      |  __setitem__(self, key, value)
      |      :param key(str): primary key of result
      |      :param key(int): list index of result
      |      :return:
+     |
+     |  def update(self, key, obj)
+     |      Applies partial updates without erasing data via the dict.update mechanism
+     |      :param key: primary key of entry
+     |      :param obj: dictionary containing new values to be merged with entry
+     |
+     |  def __delitem__(self, key)
+     |
+     |  def __contains__(self, key)
      |  
      |  query(self, field, func, checktype=None)
      |      Make a sub-query and return a new narrower Query object
      |      :param field: the field being searched, will only parse entries that have this field
      |      :param func: a function reference applied to a filter query (ie. lambda x: x > 5)
      |      :param checktype: if passed a type will automatically narrow results to that type to prevent TypeError
      |      :return: A new query object containing the results of the given query
@@ -876,14 +886,23 @@
      |  __repr__(self)
      |      Return repr(self).
      |  
      |  __setitem__(self, key, value, sync=False)
      |      :param key: primary key of entry
      |      :param value: new contents
      |      :param sync: boolean specifying to immediately sync if in writeback mode
+     |
+     |  def update(self, key, obj)
+     |      Applies partial updates without erasing data via the dict.update mechanism
+     |      :param key: primary key of entry
+     |      :param obj: dictionary containing new values to be merged with entry
+     |
+     |  def __delitem__(self, key)
+     |
+     |  def __contains__(self, key)
      |  
      |  keys(self)
      |      Returns a list of primary keys in the Table
      |      :return: list of keys
      |  
      |  query(self, field, func)
      |      Generates an initial query and returns a Query object.
```

