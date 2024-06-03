# Comparing `tmp/freeze_dried_data-2.2.5.tar.gz` & `tmp/freeze_dried_data-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeze_dried_data-2.2.5.tar", last modified: Wed May 29 02:54:32 2024, max compression
+gzip compressed data, was "freeze_dried_data-2.3.0.tar", last modified: Mon Jun  3 06:13:53 2024, max compression
```

## Comparing `freeze_dried_data-2.2.5.tar` & `freeze_dried_data-2.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 02:54:32.150724 freeze_dried_data-2.2.5/
--rwxr-xr-x   0 root         (0) root         (0)     1072 2024-05-29 02:54:15.000000 freeze_dried_data-2.2.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)    11553 2024-05-29 02:54:32.150724 freeze_dried_data-2.2.5/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)    10686 2024-05-29 02:54:15.000000 freeze_dried_data-2.2.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 02:54:32.150724 freeze_dried_data-2.2.5/freeze_dried_data/
--rwxr-xr-x   0 root         (0) root         (0)       33 2024-05-29 02:54:15.000000 freeze_dried_data-2.2.5/freeze_dried_data/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     5125 2024-05-29 02:54:15.000000 freeze_dried_data-2.2.5/freeze_dried_data/efficient_index.py
--rwxr-xr-x   0 root         (0) root         (0)    35115 2024-05-29 02:54:15.000000 freeze_dried_data-2.2.5/freeze_dried_data/freeze_dried_data.py
--rwxr-xr-x   0 root         (0) root         (0)    11613 2024-05-29 02:54:15.000000 freeze_dried_data-2.2.5/freeze_dried_data/freeze_dried_data_old.py
--rwxr-xr-x   0 root         (0) root         (0)     2233 2024-05-29 02:54:15.000000 freeze_dried_data-2.2.5/freeze_dried_data/test_efficient_index.py
--rwxr-xr-x   0 root         (0) root         (0)    39973 2024-05-29 02:54:15.000000 freeze_dried_data-2.2.5/freeze_dried_data/test_freeze_dried_data.py
--rwxr-xr-x   0 root         (0) root         (0)     7982 2024-05-29 02:54:15.000000 freeze_dried_data-2.2.5/freeze_dried_data/test_freeze_dried_data_old.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 02:54:32.150724 freeze_dried_data-2.2.5/freeze_dried_data.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11553 2024-05-29 02:54:32.000000 freeze_dried_data-2.2.5/freeze_dried_data.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      473 2024-05-29 02:54:32.000000 freeze_dried_data-2.2.5/freeze_dried_data.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 02:54:32.000000 freeze_dried_data-2.2.5/freeze_dried_data.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-05-29 02:54:32.000000 freeze_dried_data-2.2.5/freeze_dried_data.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 02:54:32.150724 freeze_dried_data-2.2.5/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1125 2024-05-29 02:54:15.000000 freeze_dried_data-2.2.5/setup.py
+drwxrwxr-x   0 tstand    (1000) tstand    (1000)        0 2024-06-03 06:13:53.534482 freeze_dried_data-2.3.0/
+-rwxrwxr-x   0 tstand    (1000) tstand    (1000)     1072 2024-06-01 06:33:35.000000 freeze_dried_data-2.3.0/LICENSE
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)    11553 2024-06-03 06:13:53.534482 freeze_dried_data-2.3.0/PKG-INFO
+-rwxrwxr-x   0 tstand    (1000) tstand    (1000)    10686 2024-06-01 06:33:35.000000 freeze_dried_data-2.3.0/README.md
+drwxrwxr-x   0 tstand    (1000) tstand    (1000)        0 2024-06-03 06:13:53.530482 freeze_dried_data-2.3.0/freeze_dried_data/
+-rwxrwxr-x   0 tstand    (1000) tstand    (1000)       33 2024-06-01 06:33:35.000000 freeze_dried_data-2.3.0/freeze_dried_data/__init__.py
+-rwxrwxr-x   0 tstand    (1000) tstand    (1000)     5345 2024-06-02 06:20:48.000000 freeze_dried_data-2.3.0/freeze_dried_data/efficient_index.py
+-rwxrwxr-x   0 tstand    (1000) tstand    (1000)    35520 2024-06-03 06:03:44.000000 freeze_dried_data-2.3.0/freeze_dried_data/freeze_dried_data.py
+-rwxrwxr-x   0 tstand    (1000) tstand    (1000)    11613 2024-06-01 06:33:35.000000 freeze_dried_data-2.3.0/freeze_dried_data/freeze_dried_data_old.py
+-rwxrwxr-x   0 tstand    (1000) tstand    (1000)     2233 2024-06-01 06:33:35.000000 freeze_dried_data-2.3.0/freeze_dried_data/test_efficient_index.py
+-rwxrwxr-x   0 tstand    (1000) tstand    (1000)    45800 2024-06-03 06:05:53.000000 freeze_dried_data-2.3.0/freeze_dried_data/test_freeze_dried_data.py
+-rwxrwxr-x   0 tstand    (1000) tstand    (1000)     7982 2024-06-01 06:33:35.000000 freeze_dried_data-2.3.0/freeze_dried_data/test_freeze_dried_data_old.py
+drwxrwxr-x   0 tstand    (1000) tstand    (1000)        0 2024-06-03 06:13:53.530482 freeze_dried_data-2.3.0/freeze_dried_data.egg-info/
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)    11553 2024-06-03 06:13:53.000000 freeze_dried_data-2.3.0/freeze_dried_data.egg-info/PKG-INFO
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)      473 2024-06-03 06:13:53.000000 freeze_dried_data-2.3.0/freeze_dried_data.egg-info/SOURCES.txt
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)        1 2024-06-03 06:13:53.000000 freeze_dried_data-2.3.0/freeze_dried_data.egg-info/dependency_links.txt
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)       18 2024-06-03 06:13:53.000000 freeze_dried_data-2.3.0/freeze_dried_data.egg-info/top_level.txt
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)       38 2024-06-03 06:13:53.534482 freeze_dried_data-2.3.0/setup.cfg
+-rwxrwxr-x   0 tstand    (1000) tstand    (1000)     1125 2024-06-03 06:13:00.000000 freeze_dried_data-2.3.0/setup.py
```

### Comparing `freeze_dried_data-2.2.5/LICENSE` & `freeze_dried_data-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `freeze_dried_data-2.2.5/PKG-INFO` & `freeze_dried_data-2.3.0/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeze_dried_data
-Version: 2.2.5
+Version: 2.3.0
 Summary: A simple format for machine learning datasets
 Home-page: https://github.com/tstandley/freeze_dried_data
 Author: Trevor Standley
 Author-email: trevor.standley@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `freeze_dried_data-2.2.5/README.md` & `freeze_dried_data-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `freeze_dried_data-2.2.5/freeze_dried_data/efficient_index.py` & `freeze_dried_data-2.3.0/freeze_dried_data/efficient_index.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 
 from bisect import bisect_left
 class FDDIntList:
-    def __init__(self, length, buffer, byte_width=5, start_in_buffer=0):
+    def __init__(self, length, buffer, byte_width=6, start_in_buffer=0):
         self.length = length
         self.buffer = buffer
         self.byte_width = byte_width
         self.start_in_buffer = start_in_buffer
 
     def __getitem__(self,idx):
+        if idx < 0:
+            idx = self.length + idx
         if idx >= self.length or idx < 0:
             raise IndexError('Index out of bounds', idx, self.length)
         buf = self.buffer[self.start_in_buffer + idx*self.byte_width:self.start_in_buffer + (idx+1)*self.byte_width]
         return int.from_bytes(buf, 'little')
     
     def __len__(self):
         return self.length
         
 
-
 class FDDIndexBase:
-    def __init__(self):
-        pass
+    pass
 
 class FDDIndexKeyless(FDDIndexBase):
-    def __init__(self, num_vals, byte_width=5):
+    def __init__(self, num_vals, byte_width=6):
         self.buffer=bytearray()
         self.num_vals = num_vals
         self.byte_width = byte_width
 
     def __getitem__(self, idx):
         if idx >= len(self) or idx < 0:
             raise IndexError('Index out of bounds', idx, len(self))
@@ -58,46 +58,46 @@
         if idx == len(self):
             for i in val:
                 self.buffer.extend(i.to_bytes(self.byte_width, 'little'))
         elif idx > len(self):
             raise IndexError('Index out of bounds', idx, len(self))
         else:
             for i, v in enumerate(val):
-                self.buffer[idx*self.num_vals*self.byte_width + i*self.byte_width:idx*self.num_vals*self.byte_width + (i+1)*self.byte_width] = v.to_bytes(5, 'little')
+                self.buffer[idx*self.num_vals*self.byte_width + i*self.byte_width:idx*self.num_vals*self.byte_width + (i+1)*self.byte_width] = v.to_bytes(self.byte_width, 'little')
             
 
 class FDDIndexComparableKey(FDDIndexBase):
-    def __init__(self, dict_index, byte_width=5):
+    def __init__(self, dict_index, byte_width=6):
         self._keys = list(dict_index.keys())
         self._keys.sort()
         self.num_vals = len(dict_index[self._keys[0]])
         self.buffer=bytearray()
         self.byte_width = byte_width
         for k in self._keys:
             for i in dict_index[k]:
-                self.buffer.extend(i.to_bytes(5, 'little'))
+                self.buffer.extend(i.to_bytes(self.byte_width, 'little'))
 
     def __getitem__(self, key):
         # idx = self.keys.index(key) #make it faster by doing a binary search
         idx = bisect_left(self._keys, key)
         if idx == len(self._keys) or self._keys[idx] != key:
             raise KeyError('Key not found', key)
         
         return FDDIntList(self.num_vals, self.buffer, byte_width=self.byte_width, start_in_buffer=idx*self.num_vals*self.byte_width)
 
     def keys(self):
         return self._keys
 
     def items(self):
-        for k in self._keys:
-            yield k, self[k]
+        for k, v in zip(self._keys, self.values()):
+            yield k, v
 
     def values(self):
-        for k in self._keys:
-            yield self[k]
+        for i in range(len(self._keys)):
+            yield FDDIntList(self.num_vals, self.buffer, byte_width=self.byte_width, start_in_buffer=i*self.num_vals*self.byte_width)
 
     def __contains__(self, key):
         try:
             idx = bisect_left(self._keys, key)
         except TypeError:
             return False
         return idx < len(self._keys) and self._keys[idx] == key    
@@ -106,15 +106,15 @@
         for k in self._keys:
             yield self[k]
 
     def __len__(self):
         return len(self._keys)
 
 class FDDIndexGeneral(FDDIndexBase):
-    def __init__(self, num_vals, byte_width=5):
+    def __init__(self, num_vals, byte_width=6):
         self.num_vals = num_vals
         #index maps keys to a single int into the array
         self.index = {}
         self.buffer = bytearray()
         self.byte_width = byte_width
 
 
@@ -127,19 +127,19 @@
         if len(val) != self.num_vals:
             raise ValueError('Incorrect length of val', len(val), self.num_vals)
 
 
         if key not in self.index:
             self.index[key] = len(self.index)
             for i in val:
-                self.buffer.extend(i.to_bytes(5, 'little'))
+                self.buffer.extend(i.to_bytes(self.byte_width, 'little'))
         else:
             idx = self.index[key]
             for i, v in enumerate(val):
-                self.buffer[idx*self.num_vals*self.byte_width + i*self.byte_width:idx*self.num_vals*self.byte_width + (i+1)*self.byte_width] = v.to_bytes(5, 'little')
+                self.buffer[idx*self.num_vals*self.byte_width + i*self.byte_width:idx*self.num_vals*self.byte_width + (i+1)*self.byte_width] = v.to_bytes(self.byte_width, 'little')
     
     def __len__(self):
         return len(self.index)
     
     def update(self, dict_index):
         for k in dict_index:
             self[k] = dict_index[k]
```

### Comparing `freeze_dried_data-2.2.5/freeze_dried_data/freeze_dried_data.py` & `freeze_dried_data-2.3.0/freeze_dried_data/freeze_dried_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,61 +1,47 @@
 import pickle as pkl
 import os
-from typing import Any, Dict, Iterator, Tuple, Optional, Union, List
+from typing import Any, Dict, Iterator, Tuple, Optional, Union, List, Iterable
 import sys
 import warnings
 import zlib
 import torch
 try:
     from .efficient_index import FDDIndexKeyless, FDDIndexComparableKey, FDDIntList, FDDIndexGeneral, FDDIndexBase
 except ImportError:
     from efficient_index import FDDIndexKeyless, FDDIndexComparableKey, FDDIntList, FDDIndexGeneral, FDDIndexBase
 
-
-# data is stored in the following format:
-# [record, record, ..., record], [custom_property, custom_property, ..., custom_property], [split, split, ..., split], [columns], index_index, 8 bytes for index_index length
-
-
-
-
 type_to_serializer = {
     'any': pkl.dumps,
     'str': lambda x: x.encode('utf-8'),
     'str_compressed': lambda x: zlib.compress(x.encode('utf-8')),
     'bytes': lambda x: x,
     'int128': lambda x: x.to_bytes(16, 'little'),
     'int64': lambda x: x.to_bytes(8, 'little'),
     'int': lambda x: x.to_bytes(8, 'little'),
     'int32': lambda x: x.to_bytes(4, 'little'),
     'int16': lambda x: x.to_bytes(2, 'little'),
     'int8': lambda x: x.to_bytes(1, 'little'),
-    'numpy': pkl.dumps,
     'torch': lambda x: pkl.dumps(x.cpu().numpy()),
-    'float': pkl.dumps
 }
 
 type_to_deserializer = {
     'any': pkl.loads,
     'str': lambda x: x.decode('utf-8'),
     'str_compressed': lambda x: zlib.decompress(x).decode('utf-8'),
     'bytes': lambda x: x,
     'int128': lambda x: int.from_bytes(x, 'little'),
     'int64': lambda x: int.from_bytes(x, 'little'),
     'int': lambda x: int.from_bytes(x, 'little'),
     'int32': lambda x: int.from_bytes(x, 'little'),
     'int16': lambda x: int.from_bytes(x, 'little'),
     'int8': lambda x: int.from_bytes(x, 'little'),
-    'numpy': pkl.loads,
     'torch': lambda x: torch.from_numpy(pkl.loads(x)),
-    'float': pkl.loads
 }
 
-
-
-
 class BaseFDD:
     """
     Base class for freeze-dried data. Should not be instantiated directly.
     There are two subclasses: RFDD (for reading) and WFDD (for writing).
 
     :param filename: The name of the file.
     """
@@ -117,29 +103,30 @@
         self.close()
     
     def close(self) -> None:
         if not self.file.closed:
             self.file.close()
 
 
-
 class RFDD(BaseFDD):
     """
     RFDD (Freeze Dried Data Reader) class for reading freeze-dried data files.
 
     :param filename: The path to the freeze-dried data file.
     :param split: The split name to load, defaults to the all rows split.
     :param system_deserialize: The function to use for deserializing the index, splits, and columns.
     :param column_to_deserialize: A tuple of functions to use for deserializing columns. There must be
         one function for each column.
     """
     def __init__(self,
                  filename: str,
                  split: str = 'all_rows',
                  system_deserialize: callable = pkl.loads) -> None:
+        if '^' in filename:
+            filename, split = filename.split('^')
         super().__init__(filename)
         self.file = open(filename, 'rb')
         self.system_deserialize = system_deserialize
         self.no_columns_deserialize = pkl.loads
         self.column_to_deserialize = None
         self.columns=None
         
@@ -187,24 +174,21 @@
         :param key: The key of the row.
         :return: The row with the specified key. 
         :raises KeyError: If the key is not found.
         """
         
         if key not in self.index:
             if isinstance(key, tuple):
-                if key in self.index:
-                    return self[key]
-                else:
-                    if key[0] in self.index:
-                        indices = self.index[key[0]]
-                        col_index = self.columns[key[1]]
-                        start = indices[col_index]
-                        end = indices[col_index+1]
-                        data = self.read_chunk(start, end)
-                        return self.column_to_deserialize[col_index](data)
+                if key[0] in self.index:
+                    indices = self.index[key[0]]
+                    col_index = self.columns[key[1]]
+                    start = indices[col_index]
+                    end = indices[col_index+1]
+                    data = self.read_chunk(start, end)
+                    return self.column_to_deserialize[col_index](data)
             else:
                 raise KeyError("Key not found.", key, self.index.keys())
         
         if self.columns is None:
             
             start, end = self.index[key]
             data = self.read_chunk(start, end)
@@ -329,15 +313,15 @@
     """
 
     def __init__(self, index: Tuple[Any], parent, ) -> None:
         self._fdd_row_index = index
         self._fdd_row_parent = parent
         self._fdd_row_cache = [None for _ in range(len(self._fdd_row_index) - 1)]
 
-    def get_dict(self):
+    def as_dict(self):
         """
         :return: A dictionary representation of the row.
         """
         return {k: self[i] for i, k in enumerate(self._fdd_row_parent.columns)}
     
     def __getitem__(self, key: int | str) -> Any:
         """
@@ -407,27 +391,73 @@
             raise AttributeError("Row has already been finalized.")
         columns = self._fdd_row_parent.columns
         if name not in columns:
             raise AttributeError(f"Column not found: {name}")
         
         index = columns[name] if isinstance(columns, dict) else columns.index(name)
         self._fdd_row_cache[index] = value
+
+    def __contains__(self, key: str) -> bool:
+        """
+        Checks if the row contains the specified column.
+
+        :param key: The name of the column.
+        :return: True if the column is found, False otherwise.
+        """
+        return key in self._fdd_row_parent.columns
+    
+    def __iter__(self) -> Iterator[Any]:
+        """
+        Yields the values for the row.
+        """
+        for i, key in enumerate(self._fdd_row_parent.columns):
+            yield key
+    
+    def __hasattr__(self, name: str) -> bool:
+        """
+        Checks if the row contains the specified column.
+
+        :param name: The name of the column.
+        :return: True if the column is found, False otherwise.
+        """
+        return name in self._fdd_row_parent.columns
+    
+    def items(self) -> Iterator[Tuple[str, Any]]:
+        """
+        Yields (column name, value) pairs for the row.
+        """
+        for i, key in enumerate(self._fdd_row_parent.columns):
+            yield key, self[i]
+
+    def keys(self) -> Iterator[str]:
+        """
+        Yields the column names for the row.
+        """
+        for key in self._fdd_row_parent.columns:
+            yield key
+    
+    def values(self) -> Iterator[Any]:
+        """
+        Yields the values for the row.
+        """
+        for i, key in enumerate(self._fdd_row_parent.columns):
+            yield self[i]
+
+    
     
     def __repr__(self) -> str:
         """
         :return: A human readable string representation of the row. One line per column.
         """
         rep = ""
         for i, key in enumerate(self._fdd_row_parent.columns):
             value = self[i]
             rep += f"{key}: {value}\n"
         return rep
 
-
-
 class WFDD(BaseFDD):
     """
     WFDD (Freeze Dried Data Writer) class for writing freeze-dried data files.
 
     :param filename: The path to the freeze-dried data file.
     :param columns: The column names for the data. If None, columns won't be used to store the data.
     :param overwrite: Whether to overwrite an existing file, default is False.
@@ -443,15 +473,14 @@
     def __init__(self,
                  filename: str,
                  columns: dict[str, str | tuple[callable, callable]] = None,
                  overwrite: bool = False,
                  reopen: bool = False,
                  system_serialize: callable = pkl.dumps,
                  system_deserialize: callable = pkl.loads,
-                 preserve_order=True,
                  ) -> None:
         self.__dict__['_initializing'] = True # Use self.__dict__ to bypass __setattr__
         super().__init__(filename)
         
         if not overwrite and not reopen and os.path.exists(filename):
             raise FileExistsError("File already exists.", filename)
         
@@ -461,32 +490,25 @@
         column_to_serialize = {v: type_to_serializer[t] if isinstance(t, str) else t[0] for v, t in columns.items()} if columns is not None else None
         
         column_to_deserialize = {v: type_to_deserializer[t] if isinstance(t, str) else t[1] for v, t in columns.items()} if columns is not None else None
         
         self.column_def = columns
 
         if columns is not None:
-            if column_to_deserialize is None:
-                self.column_to_deserialize = tuple(pkl.loads for i in range(len(columns)))
-            else:
-                self.column_to_deserialize = tuple(column_to_deserialize.values())
-            if column_to_serialize is None:
-                self.column_to_serialize = tuple(system_serialize for i in range(len(columns)))
-            else:
-                self.column_to_serialize = tuple(column_to_serialize.values())
+            self.column_to_deserialize = tuple(column_to_deserialize.values())
+            self.column_to_serialize = tuple(column_to_serialize.values())
         else:
             self.column_to_deserialize = None
             self.column_to_serialize = None
         
         
         self.system_serialize = system_serialize
         self.system_deserialize = system_deserialize
         self.no_columns_serialize = pkl.dumps
         self.no_columns_deserialize = pkl.loads
-        self.preserve_order = preserve_order
 
         if reopen:
             self.reopen()
         else:
             self.file = open(filename, 'wb+')
             self.unfinished_setters = {}
             
@@ -610,34 +632,34 @@
                     serialize = self.no_columns_serialize
                 data = serialize(v)
                 self.file.write(data)
             positions.append(self.file.tell())
             
         self.index[key] = tuple(positions)    
 
-    def make_split(self, split: str, rows: list | tuple | set | frozenset, overwrite=False, keyless=False) -> None:
+    def make_split(self, split: str, rows: Iterable, overwrite=False, keyless=False, preserve_order=True) -> None:
         """
         Create a split in the WFDD.
 
         :param split: The name of the split.
         :param rows: The iterable of keys for the split.
         """
         if split in self.split_to_index and not overwrite:
             raise ValueError("Split already exists.", split, 'Use overwrite=True to overwrite it.')
         
-        if isinstance(rows, (list, tuple, set, frozenset)):
+        if not isinstance(rows, str):
             
             if keyless:
                 split_index = FDDIndexKeyless(num_vals=len(self.columns)+1 if self.columns is not None else 2)
                 for i, key in enumerate(rows):
                     split_index[i] = self.index[key]
             else:
                 split_index_dict = {key: self.index[key] for key in rows}
                 try:
-                    if not self.preserve_order:
+                    if not preserve_order:
                         split_index = FDDIndexComparableKey(split_index_dict)
                     else:
                         raise ValueError("dummy error go to except block")
                 except:
                     split_index = FDDIndexGeneral(len(self.columns)+1 if self.columns is not None else 2)
                     for k,v in split_index_dict.items():
                         split_index[k] = v
@@ -700,16 +722,14 @@
         else:
             columns_start, columns_end = index_index['_columns_']
             earliest = min(columns_start, earliest)
             index_index.pop('_columns_')
 
             self.columns = self.system_deserialize(self.read_chunk(columns_start, columns_end))
             
-                
-
         self.custom_properties = {k[6:]:v for k,v in index_index.items() if k.startswith('_prop_')}
         
         # need to figure out where to seek so that we are at the end of the rows. Everything else shoudl be in ram.
         new_custom_properties = {}
         for k,v in self.custom_properties.items():
             prop_start, prop_end = v
             if prop_start < earliest:
@@ -740,16 +760,14 @@
             
             Writing {} unfinished setters to disk now.
             """.format(len(cpy)), UserWarning)
 
         for k in cpy:
             self.unfinished_setters[k].finalize()
 
-        
-        
         index_index = {}
         has_lambda = False
         if self.column_def is not None:
             for k,v in self.column_def.items():
                 if isinstance(v, tuple):
                     has_lambda = True
                     break
@@ -772,23 +790,14 @@
         for k,v in self.custom_properties.items():
             property_start = self.file.tell()
             property_data = self.system_serialize(v)
             self.file.write(property_data)
             property_end = self.file.tell()
             index_index["_prop_"+k] = (property_start, property_end)
 
-        if not isinstance(self.index, FDDIndexKeyless):
-            try:
-                if not self.preserve_order:
-                    self.index = FDDIndexComparableKey(self.index)
-            except:
-                pass
-        
-        
-
         self.split_to_index['all_rows'] = self.index
         for k,v in self.split_to_index.items():
             split_start = self.file.tell()
             split_data = self.system_serialize(v)
             self.file.write(split_data)
             split_end = self.file.tell()
             index_index["_split_"+k] = (split_start, split_end)
@@ -860,15 +869,15 @@
 
         :param key: The name of the column.
         :param value: The value to set.
         """
         self.__setattr__(key, value)
 
 
-def add_column(input_path, output_path, column_name, column_data, overwrite=False, column_serialize=pkl.dumps):
+def add_column(input_path, output_path, column_name, column_data, overwrite=False, column_type='any'):
     """
     Add a column to a freeze-dried data file.
 
     :param input_path: The path to the input freeze-dried data file.
     :param output_path: The path to the output freeze-dried data file.
     :param column_name: The name of the column to add.
     :param column_data: The data for the column.
@@ -877,17 +886,22 @@
     # if it has an items() funciton, call it
     if hasattr(column_data, 'items'):
         column_data = column_data.items()
 
     with RFDD(input_path) as rfdd:
         if column_name in rfdd.columns:
             raise ValueError("Column already exists.", column_name)
+        
+        column_def = rfdd.column_def
+        column_def[column_name] = column_type
+
+        column_serialize = type_to_serializer[column_type]
 
-        new_columns = list(rfdd.columns) + [column_name]
-        with WFDD(output_path, columns=new_columns, overwrite=overwrite) as wfdd:
+        
+        with WFDD(output_path, columns=column_def, overwrite=overwrite) as wfdd:
             
             for key, value in column_data:
                 row_index = rfdd.index[key]
                 start, end = row_index[0], row_index[-1]
 
                 row_data = rfdd.read_chunk(start, end)
```

### Comparing `freeze_dried_data-2.2.5/freeze_dried_data/freeze_dried_data_old.py` & `freeze_dried_data-2.3.0/freeze_dried_data/freeze_dried_data_old.py`

 * *Files identical despite different names*

### Comparing `freeze_dried_data-2.2.5/freeze_dried_data/test_efficient_index.py` & `freeze_dried_data-2.3.0/freeze_dried_data/test_efficient_index.py`

 * *Files identical despite different names*

### Comparing `freeze_dried_data-2.2.5/freeze_dried_data/test_freeze_dried_data.py` & `freeze_dried_data-2.3.0/freeze_dried_data/test_freeze_dried_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         # Read operations
         with RFDD(self.test_file) as rfdd:
             self.assertEqual(rfdd['hello'], 'world')
             self.assertEqual(rfdd['number'], 123)
 
     def test_basic_operations_with_columns(self):
         # Write operations
-        with WFDD(self.test_file, columns={'name':'str','area':'float', 'price':'float'}, overwrite=True) as wfdd:
+        with WFDD(self.test_file, columns={'name':'str','area':'any', 'price':'any'}, overwrite=True) as wfdd:
             wfdd['house1'] = {'name': 'house1', 'area': 100, 'price': 100000}
             wfdd['house2'] = {'name': 'house2', 'area': 200, 'price': 200000}
             wfdd['house3'] = ('house3', 300, 300000)
 
         # Read operations
         with RFDD(self.test_file) as rfdd:
             self.assertTrue('house1' in rfdd)
@@ -116,20 +116,20 @@
 
     def test_file_does_not_exist(self):
         with self.assertRaises(FileNotFoundError):
             with RFDD(self.test_file) as rfdd:
                 pass
 
     def test_modify_and_write(self):
-        with WFDD(self.test_file, columns={'name':'str','area':'float', 'price':'float'}, overwrite=True) as wfdd:
+        with WFDD(self.test_file, columns={'name':'str','area':'any', 'price':'any'}, overwrite=True) as wfdd:
             wfdd['house1'] = {'name': 'house1', 'area': 100, 'price': 100000}
             wfdd['house2'] = {'name': 'house2', 'area': 200, 'price': 200000}
             wfdd['house3'] = ('house3', 300, 300000)
 
-        with WFDD(self.test_file2, columns={'name':'str','area':'float', 'price':'float'}, overwrite=True) as wfdd,\
+        with WFDD(self.test_file2, columns={'name':'str','area':'any', 'price':'any'}, overwrite=True) as wfdd,\
              RFDD(self.test_file) as rfdd:
              for k,v in rfdd.items():
                 v.price = v.price * 1.5
                 wfdd[k+' with inflation'] = v
 
         with RFDD(self.test_file2) as rfdd:
             self.assertEqual(rfdd['house1 with inflation'].name, 'house1')
@@ -139,20 +139,20 @@
             self.assertEqual(rfdd['house2 with inflation'].area, 200)
             self.assertEqual(rfdd['house2 with inflation'].price, 300000)
             self.assertEqual(rfdd['house3 with inflation'].name, 'house3')
             self.assertEqual(rfdd['house3 with inflation'].area, 300)
             self.assertEqual(rfdd['house3 with inflation'].price, 450000)
 
     def test_modify_and_write_use_indices(self):
-        with WFDD(self.test_file, columns={'name':'str','area':'float', 'price':'float'}, overwrite=True) as wfdd:
+        with WFDD(self.test_file, columns={'name':'str','area':'any', 'price':'any'}, overwrite=True) as wfdd:
             wfdd['house1'] = {'name': 'house1', 'area': 100, 'price': 100000}
             wfdd['house2'] = {'name': 'house2', 'area': 200, 'price': 200000}
             wfdd['house3'] = ('house3', 300, 300000)
 
-        with WFDD(self.test_file2, columns={'name':'str','area':'float', 'price':'float'}, overwrite=True) as wfdd,\
+        with WFDD(self.test_file2, columns={'name':'str','area':'any', 'price':'any'}, overwrite=True) as wfdd,\
              RFDD(self.test_file) as rfdd:
              for k,v in rfdd.items():
                 v[2] = v[2] * 1.5
                 wfdd[k+' with inflation'] = v
 
         with RFDD(self.test_file2) as rfdd:
             self.assertEqual(rfdd['house1 with inflation'].name, 'house1')
@@ -199,15 +199,15 @@
             self.assertEqual(fdd.property_two, 'new')
             dct = {}
             for k,v in fdd.items():
                 dct[k] = v.value
             self.assertEqual(dct, {'key1': 'value1', 'key2': 'value2', 'key3': 'value3'})
 
     def test_incomplete_columns(self):
-        with WFDD(self.test_file, columns={'name':'str','area':'float', 'price':'float'}, overwrite=True) as wfdd:
+        with WFDD(self.test_file, columns={'name':'str','area':'any', 'price':'any'}, overwrite=True) as wfdd:
             wfdd['house1'] = {'name': 'house1', 'area': 100}
             wfdd['house2'] = {'name': 'house2', 'price': 200000}
             wfdd['house3'] = ('house3', 300, 300000)
         
         with RFDD(self.test_file) as rfdd:
             self.assertEqual(rfdd['house1'].name, 'house1')
             self.assertEqual(rfdd['house1'].area, 100)
@@ -233,34 +233,34 @@
             rfdd['key1'].value = 'new_value1'
             self.assertEqual(rfdd['key1'].value, 'new_value1')
 
             rfdd['key1']['value'] = 'new_value2'
             self.assertEqual(rfdd['key1'].value, 'new_value2')
 
     def test_set_all_of_column(self):
-        with WFDD(self.test_file, columns={'value':'float','area':'float'}, overwrite=True) as wfdd:
+        with WFDD(self.test_file, columns={'value':'any','area':'any'}, overwrite=True) as wfdd:
             for i in range(100):
                 wfdd[f'key{i}'].value = i
                 wfdd[f'key{i}'].area = i+1
         
         with RFDD(self.test_file) as rfdd:
-            with WFDD(self.test_file2, columns={'value':'float','area':'float'}, overwrite=True) as wfdd2:
+            with WFDD(self.test_file2, columns={'value':'any','area':'any'}, overwrite=True) as wfdd2:
                 for k,v in rfdd.items():
                     v.value = v.value * 1.1
                     wfdd2[k] = v
 
         with RFDD(self.test_file2) as rfdd2:
             for i, (k,v) in enumerate(rfdd2.items()):
                 self.assertEqual(v.value, i*1.1)
                 self.assertEqual(v.area, i+1)
 
 
 
     def test_set_columns_by_attribute_or_item(self):
-        with WFDD(self.test_file, columns={'name':'str','area':'float', 'price':'float'}, overwrite=True) as wfdd:
+        with WFDD(self.test_file, columns={'name':'str','area':'any', 'price':'any'}, overwrite=True) as wfdd:
             wfdd['house1'].name = 'house1'
             wfdd['house1'].area = 100
             wfdd['house1'].price = 100000
             wfdd['house2']["name"] = 'house2'
             wfdd['house2']["area"] = 200
             wfdd['house2']["price"] = 200000
             wfdd['house3'] = ('house3', 300, 300000)
@@ -338,15 +338,15 @@
             keys = wfdd.keys()
             self.assertEqual(len(keys), 3)
 
 
     def test_splits(self):
 
         
-        with WFDD(self.test_file, columns={'name':'str','area':'float', 'price':'float'}, overwrite=True) as wfdd:
+        with WFDD(self.test_file, columns={'name':'str','area':'any', 'price':'any'}, overwrite=True) as wfdd:
             for i in range(100):
                 wfdd[f'house_{i}'] = {'name': f'house_{i}', 'area': 100+10*i, 'price': 1000+100*i}
 
             wfdd.make_split('odds', [f'house_{i}' for i in range(1,100,2)])
             wfdd.make_split('evens', [f'house_{i}' for i in range(0,100,2)])
             wfdd.make_split('big houses', [f'house_{i}' for i in range(80,100)])
             wfdd.make_split('reverse_order', [f'house_{i}' for i in range(99,-1,-1)])
@@ -375,16 +375,15 @@
             rfdd.load_new_split('big houses')
             self.assertEqual(len(list(rfdd.keys())), 20)
             for i, (k,v) in enumerate(rfdd.items()):
                 self.assertEqual(k, f'house_{80+i}')
                 self.assertEqual(v.name, f'house_{80+i}')
                 self.assertEqual(v.area, 900+10*i)
                 self.assertEqual(v.price, 9000+100*i)
-
-            rfdd.load_new_split('reverse_order')
+        with RFDD(f"{self.test_file}^reverse_order") as rfdd:
             self.assertEqual(len(list(rfdd.keys())), 100)
             for i, (k,v) in enumerate(rfdd.items()):
                 self.assertEqual(k, f'house_{99-i}')
                 self.assertEqual(v.name, f'house_{99-i}')
                 self.assertEqual(v.area, 1090-10*i)
                 self.assertEqual(v.price, 10900-100*i)
 
@@ -418,15 +417,15 @@
 
         with RFDD(self.test_file) as rfdd:
             self.assertEqual(len(list(rfdd.keys())), num_records)
             for key, value in data.items():
                 self.assertEqual(rfdd[key], value)
 
     def test_column_not_found(self):
-        with WFDD(self.test_file, columns={'name':'str','area':'float', 'price':'float'}, overwrite=True) as wfdd:
+        with WFDD(self.test_file, columns={'name':'str','area':'any', 'price':'any'}, overwrite=True) as wfdd:
             wfdd['house1'] = {'name': 'house1', 'area': 100, 'price': 100000}
             wfdd['house2'] = {'name': 'house2', 'area': 200, 'price': 200000}
             wfdd['house3'] = ('house3', 300, 300000)
             wfdd['house4'].name = 'house4'
             with self.assertRaises(AttributeError):
                 wfdd['house4'].nonexistent = 3
 
@@ -438,15 +437,15 @@
                 _ = rfdd['house1'].nonexistent
             
             with self.assertRaises(AttributeError):
                 rfdd['house1'].nonexistent = 3
         
     def test_print_finalize_warning(self):
         with self.assertWarns(UserWarning):
-            with WFDD(self.test_file, columns={'name':'str','area':'float', 'price':'float'}, overwrite=True) as wfdd:
+            with WFDD(self.test_file, columns={'name':'str','area':'any', 'price':'any'}, overwrite=True) as wfdd:
                 for i in range(1100):
                     wfdd[f'house_{i}'].name = f'house_{i}' # we only set the name attribute
             # we should get a warning upon exiting the context
 
         # rows should be written to disk anyway
         with RFDD(self.test_file) as rfdd:
             for i in range(1100):
@@ -464,15 +463,15 @@
     def test_key_already_exists(self):
         with WFDD(self.test_file, overwrite=True) as wfdd:
             wfdd['key1']= 'value1'
             with self.assertRaises(KeyError):
                 wfdd['key1'] = 'value2'
             
     def test_invalid_object_for_column_mode(self):
-        with WFDD(self.test_file, columns={'name':'str','area':'float', 'price':'float'}, overwrite=True) as wfdd:
+        with WFDD(self.test_file, columns={'name':'str','area':'any', 'price':'any'}, overwrite=True) as wfdd:
             wfdd['house1'] = {'name': 'house1', 'area': 100, 'price': 100000}
             wfdd['house2'] = {'name': 'house2', 'area': 200, 'price': 200000}
             with self.assertRaises(ValueError):
                 wfdd['house3'] = 15
 
         with WFDD(self.test_file, overwrite=True) as wfdd:
             wfdd['house1'] = {'name': 'house1', 'area': 100, 'price': 100000}
@@ -488,32 +487,32 @@
 
         class Test2:
             def __init__(self, time, location):
                 self.time = time
                 self.location = location
 
 
-        with WFDD(self.test_file, columns={'name':'str','area':'float', 'price':'float'}, overwrite=True) as wfdd:
+        with WFDD(self.test_file, columns={'name':'str','area':'any', 'price':'any'}, overwrite=True) as wfdd:
             wfdd['house1'] = Test('house1', 100, 100000)
             wfdd['house2'] = Test('house2', 200, 200000)
             with self.assertRaises(ValueError):
                 wfdd['house3'] = Test2('house3', 300)
 
-        with WFDD(self.test_file, columns={'name':'str','area':'float', 'price':'float'}, overwrite=True) as wfdd:
+        with WFDD(self.test_file, columns={'name':'str','area':'any', 'price':'any'}, overwrite=True) as wfdd:
             with self.assertRaises(ValueError):
                 wfdd['house1'] = {"happy": "birthday"}
             
 
         
 
     def test_reaads_in_between_writes_with_columns(self):
         num_records = 1000
         data = {f'key{i}': {'name': f'name{i}', 'area': random.random(), 'price': random.random()} for i in range(num_records)}
         
-        with WFDD(self.test_file, columns={'name':'str','area':'float', 'price':'float'}, overwrite=True) as wfdd:
+        with WFDD(self.test_file, columns={'name':'str','area':'any', 'price':'any'}, overwrite=True) as wfdd:
             for i, (k, v) in enumerate(data.items()):
                 wfdd[k] = v
                 where_read = random.choice(list(data.keys())[:i+1])
                 self.assertEqual(wfdd[where_read].name, data[where_read]['name'])
                 self.assertEqual(wfdd[where_read].area, data[where_read]['area'])
                 self.assertEqual(wfdd[where_read].price, data[where_read]['price'])
 
@@ -731,15 +730,15 @@
             self.assertEqual(rfdd.custom_attribute1, 're-written custom1')
             self.assertEqual(rfdd.custom_attribute2, 'custom2')
             self.assertEqual(rfdd.custom_attribute3, 'custom3')
 
 
     def test_reopen_file_with_columns(self):
         data = {f'key{i}': {'name': f'name{i}', 'area': random.random(), 'price': random.random()} for i in range(1000)}
-        with WFDD(self.test_file, columns={'name':'str','area':'float', 'price':'float'}, overwrite=True) as wfdd:
+        with WFDD(self.test_file, columns={'name':'str','area':'any', 'price':'any'}, overwrite=True) as wfdd:
             for k, v in data.items():
                 wfdd[k] = v
 
             wfdd.custom_attribute1 = 'custom1'
             wfdd.custom_attribute2 = 'custom2'
             wfdd.make_split('evens', [f'key{i}' for i in range(0,1000,2)])
         with RFDD(self.test_file) as rfdd:
@@ -752,15 +751,15 @@
             for i, (k,v) in enumerate(rfdd.items()):
                 self.assertEqual(k, f'key{2*i}')
                 self.assertEqual(v.name, f'name{2*i}')
                 self.assertEqual(v.area, data[f'key{2*i}']['area'])
                 self.assertEqual(v.price, data[f'key{2*i}']['price'])
 
         data_2 = {f'key{i}': {'name': f'name{i}', 'area': random.random(), 'price': random.random()} for i in range(1000,2000)}
-        with WFDD(self.test_file, columns={'name':'str','area':'float', 'price':'float'}, reopen=True) as wfdd:
+        with WFDD(self.test_file, columns={'name':'str','area':'any', 'price':'any'}, reopen=True) as wfdd:
 
             for k, v in data_2.items():
                 wfdd[k] = v
             
             wfdd.custom_attribute1 = 're-written custom1'
             wfdd.custom_attribute3 = 'custom3'
             wfdd.add_to_split('evens', [f'key{i}' for i in range(1000,2000,2)])
@@ -768,78 +767,188 @@
                 wfdd.add_to_split('fake_split', ['key1'])
             with self.assertRaises(ValueError):
                 wfdd.add_to_split('evens', 234234)
             wfdd.make_split('odds', [f'key{i}' for i in range(1,2000,2)])
 
 
     def test_columns_with_partial_dicts(self):
-        with WFDD(self.test_file, columns={'name':'str','area':'float', 'price':'float'}, overwrite=True) as wfdd:
+        with WFDD(self.test_file, columns={'name':'str','area':'any', 'price':'any'}, overwrite=True) as wfdd:
             wfdd['house1'] = {'name': 'house1', 'area': 100}
             wfdd['house2'] = {'name': 'house2', 'price': 200000}
 
         with RFDD(self.test_file) as rfdd:
             self.assertEqual(rfdd['house1'].name, 'house1')
             self.assertEqual(rfdd['house1'].area, 100)
             self.assertEqual(rfdd['house1'].price, None)
             self.assertEqual(rfdd['house2'].name, 'house2')
             self.assertEqual(rfdd['house2'].area, None)
             self.assertEqual(rfdd['house2'].price, 200000)
 
     def test_columns_with_dicts_with_extra_keys(self):
         
-        with WFDD(self.test_file, columns={'name':'str','area':'float', 'price':'float'}, overwrite=True) as wfdd:
+        with WFDD(self.test_file, columns={'name':'str','area':'any', 'price':'any'}, overwrite=True) as wfdd:
             with self.assertRaises(ValueError):
                 wfdd['house1'] = {'name': 'house1', 'area': 100, 'extra': 'extra'}
             with self.assertRaises(ValueError):
                 wfdd['house2'] = {'name': 'house2', 'price': 200000, 'extra': 'extra'}
 
-    def test_get_dict(self):
+    def test_as_dict(self):
         
-        with WFDD(self.test_file, columns={'name':'str','area':'float', 'price':'float'}, overwrite=True) as wfdd:
+        with WFDD(self.test_file, columns={'name':'str','area':'any', 'price':'any'}, overwrite=True) as wfdd:
             wfdd['house1'] = {'name': 'house1', 'area': 100, 'price': 100000}
             wfdd['house2'] = {'name': 'house2', 'area': 200, 'price': 200000}
             wfdd['house3'] = ('house3', 300, 300000)
 
         with RFDD(self.test_file) as rfdd:
-            self.assertEqual(rfdd['house1'].get_dict(), {'name': 'house1', 'area': 100, 'price': 100000})
-            self.assertEqual(rfdd['house2'].get_dict(), {'name': 'house2', 'area': 200, 'price': 200000})
-            self.assertEqual(rfdd['house3'].get_dict(), {'name': 'house3', 'area': 300, 'price': 300000})
+            self.assertEqual(rfdd['house1'].as_dict(), {'name': 'house1', 'area': 100, 'price': 100000})
+            self.assertEqual(rfdd['house2'].as_dict(), {'name': 'house2', 'area': 200, 'price': 200000})
+            self.assertEqual(rfdd['house3'].as_dict(), {'name': 'house3', 'area': 300, 'price': 300000})
+
+    def test_read_row_features(self):
+        with WFDD(self.test_file, columns={'name':'str','area':'any', 'price':'any'}, overwrite=True) as wfdd:
+            wfdd['house1'] = {'name': 'house1', 'area': 100, 'price': 100000}
+            wfdd['house2'] = {'name': 'house2', 'area': 200, 'price': 200000}
+            wfdd['house3'] = ('house3', 300, 300000)
+
+        with RFDD(self.test_file) as rfdd:
+            self.assertIn('name', rfdd['house1'])
+            for k,v in rfdd['house1'].items():
+                self.assertIn(k, ['name', 'area', 'price'])
+                self.assertIn(v, ['house1', 100, 100000])
+                self.assertIn(k, rfdd['house1'])
+                
+            for k in rfdd['house1']:
+                self.assertIn(k, ['name', 'area', 'price'])
+            for k in rfdd['house1'].keys():
+                self.assertIn(k, ['name', 'area', 'price'])
+            for v in rfdd['house1'].values():
+                self.assertIn(v, ['house1', 100, 100000])
 
-    # def test_add_column(self):
-        
-    #     with WFDD(self.test_file, columns={'name':'str','area':'float'}, overwrite=True) as wfdd:
-    #         for i in range(100):
-    #             wfdd[f'house_{i}'] = {'name': f'house_{i}', 'area': 100+10*i}
 
-    #         wfdd.custom_attribute1 = 'custom1'
 
-    #         wfdd.make_split('evens', [f'house_{i}' for i in range(0,100,2)])
+    def test_alternative_indices(self):
+        for index_type in [(False, False), (True, False), (False, True), (True, True)]:
+            wfdd_dict = {}
+            with WFDD(self.test_file, columns={'name':'str','area':'any', 'price':'any'}, overwrite=True,) as wfdd:
+                for i in range(100):
+                    wfdd[f'house_{i}'] = {'name': f'house_{i}', 'area': 100+10*i, 'price': 1000+100*i}
+                    wfdd_dict[f'house_{i}'] = {'name': f'house_{i}', 'area': 100+10*i, 'price': 1000+100*i}
+
+                wfdd.make_split('odds', [f'house_{i}' for i in range(1,100,2)], keyless=index_type[0], preserve_order=index_type[1])
+                wfdd.make_split('evens', [f'house_{i}' for i in range(0,100,2)], keyless=index_type[0], preserve_order=index_type[1])
+                wfdd.make_split('big houses', [f'house_{i}' for i in range(80,100)], keyless=index_type[0], preserve_order=index_type[1])
+                wfdd.make_split('reverse_order', [f'house_{i}' for i in range(99,-1,-1)], keyless=index_type[0], preserve_order=index_type[1])
+                wfdd.make_split('all_rows', wfdd.keys(), overwrite=True, keyless=index_type[0], preserve_order=index_type[1])
+                with self.assertRaises(ValueError):
+                    wfdd.make_split('odds', [f'house_{i}' for i in range(1,100,2)], keyless=index_type[0], preserve_order=index_type[1])
+                with self.assertRaises(ValueError):
+                    wfdd.make_split('wrong', 'not_a_list', keyless=index_type[0], preserve_order=index_type[1])
+
+
+            with RFDD(self.test_file, split='all_rows') as rfdd:
+                self.assertEqual(len(list(rfdd.keys())), 100)
+                self.assertEqual(rfdd.get_available_splits(), ['odds', 'evens', 'big houses', 'reverse_order', 'all_rows'])
+
+                for i, (k,v) in enumerate(rfdd.items()):
+                    if index_type[0] == False:# keyless
+                        self.assertIn(k, wfdd_dict)
+                    if index_type[1] == True:# preserve_order
+                        
+                        self.assertEqual(v.name, f'house_{i}')
+                        self.assertEqual(v.area, 100+10*i)
+                        self.assertEqual(v.price, 1000+100*i)
+                    else:
+                        self.assertIn(v.as_dict(), wfdd_dict.values())
+                            
+                
+                rfdd.load_new_split('odds')
+                for i, (k,v) in enumerate(rfdd.items()):
+                    if index_type[0] == False:# keyless
+                        self.assertIn(k, wfdd_dict)
+                    if index_type[1] == True:# preserve_order
+                        self.assertEqual(v.name, f'house_{i*2+1}')
+                        self.assertEqual(v.area, 110+20*i)
+                        self.assertEqual(v.price, 1100+200*i)
+                    else:
+                        self.assertIn(v.as_dict(), wfdd_dict.values())
+                        
+                    
+
+                rfdd.load_new_split('evens')
+                self.assertEqual(len(list(rfdd.keys())), 50)
+                for i, (k,v) in enumerate(rfdd.items()):
+                    if index_type[0] == False:# keyless
+                        self.assertIn(k, wfdd_dict)
+                    if index_type[1] == True:# preserve_order
+                        self.assertEqual(v.name, f'house_{2*i}')
+                        self.assertEqual(v.area, 100+20*i)
+                        self.assertEqual(v.price, 1000+200*i)
+                    else:
+                        self.assertIn(v.as_dict(), wfdd_dict.values())
+
+                        
+                    
+
+                rfdd.load_new_split('big houses')
+                self.assertEqual(len(list(rfdd.keys())), 20)
+                for i, (k,v) in enumerate(rfdd.items()):
+                    if index_type[0] == False:# keyless
+                        self.assertIn(k, wfdd_dict)
+                    if index_type[1] == True:# preserve_order
+                        self.assertEqual(v.name, f'house_{80+i}')
+                        self.assertEqual(v.area, 900+10*i)
+                        self.assertEqual(v.price, 9000+100*i)
+                    else:
+                        self.assertIn(v.as_dict(), wfdd_dict.values())
+                        
+                    
+
+                rfdd.load_new_split('reverse_order')
+                self.assertEqual(len(list(rfdd.keys())), 100)
+                for i, (k,v) in enumerate(rfdd.items()):
+                    if index_type[0] == False:# keyless
+                        self.assertIn(k, wfdd_dict)
+                    if index_type[1] == True:# preserve_order
+                        self.assertEqual(v.name, f'house_{99-i}')
+                        self.assertEqual(v.area, 1090-10*i)
+                        self.assertEqual(v.price, 10900-100*i)
+                    else:
+                        self.assertIn(v.as_dict(), wfdd_dict.values())
+                        
+    def test_add_column(self):
+        with WFDD(self.test_file, columns={'name':'str','area':'any'}, overwrite=True) as wfdd:
+            for i in range(100):
+                wfdd[f'house_{i}'] = {'name': f'house_{i}', 'area': 100+10*i}
 
-    #     new_col = {}
-    #     for i in range(100):
-    #         new_col[f'house_{i}'] = 1000+100*i
+            wfdd.custom_attribute1 = 'custom1'
+
+            wfdd.make_split('evens', [f'house_{i}' for i in range(0,100,2)])
+
+        new_col = {}
+        for i in range(100):
+            new_col[f'house_{i}'] = 1000+100*i
         
         
-    #     if os.path.exists(self.test_file3):
-    #         os.remove(self.test_file3)
+        if os.path.exists(self.test_file3):
+            os.remove(self.test_file3)
 
-    #     add_column(self.test_file, self.test_file3, 'price', new_col)
+        add_column(self.test_file, self.test_file3, 'price', new_col)
 
-    #     with RFDD(self.test_file3) as rfdd:
-    #         for i in range(100):
-    #             self.assertEqual(rfdd[f'house_{i}'].price, 1000+100*i)
+        with RFDD(self.test_file3) as rfdd:
+            for i in range(100):
+                self.assertEqual(rfdd[f'house_{i}'].price, 1000+100*i)
 
-    #         rfdd.load_new_split('evens')
-    #         for i in range(50):
-    #             self.assertEqual(rfdd[f'house_{2*i}'].price, 1000+200*i)
+            rfdd.load_new_split('evens')
+            for i in range(50):
+                self.assertEqual(rfdd[f'house_{2*i}'].price, 1000+200*i)
 
-    #         self.assertEqual(rfdd.custom_attribute1, 'custom1')
+            self.assertEqual(rfdd.custom_attribute1, 'custom1')
 
-    #     with self.assertRaises(ValueError):
-    #         add_column(self.test_file3, self.test_file4, 'price', new_col)
+        with self.assertRaises(ValueError):
+            add_column(self.test_file3, self.test_file4, 'price', new_col)
 
             
 
     def test_dataloader_integration(self):
         from torch.utils.data import DataLoader, Dataset
 
         num_records = 100000
@@ -871,15 +980,15 @@
     def test_dataloader_integration_with_columns(self):
         from torch.utils.data import DataLoader, Dataset
         import torch
 
         num_records = 100000
         data = {f'key{i}': {'name': f'name{i}', 'area': random.random(), 'price': random.random()} for i in range(num_records)}
         
-        with WFDD(self.test_file, columns={'name':'str','area':'float', 'price':'float'}, overwrite=True) as wfdd:
+        with WFDD(self.test_file, columns={'name':'str','area':'any', 'price':'any'}, overwrite=True) as wfdd:
             for k, v in data.items():
                 wfdd[k] = v
 
         class FDDDataset(Dataset):
             def __init__(self, filename):
                 self.rfdd = RFDD(filename)
                 self.keys = list(self.rfdd.keys())
```

### Comparing `freeze_dried_data-2.2.5/freeze_dried_data/test_freeze_dried_data_old.py` & `freeze_dried_data-2.3.0/freeze_dried_data/test_freeze_dried_data_old.py`

 * *Files identical despite different names*

### Comparing `freeze_dried_data-2.2.5/freeze_dried_data.egg-info/PKG-INFO` & `freeze_dried_data-2.3.0/freeze_dried_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeze-dried-data
-Version: 2.2.5
+Version: 2.3.0
 Summary: A simple format for machine learning datasets
 Home-page: https://github.com/tstandley/freeze_dried_data
 Author: Trevor Standley
 Author-email: trevor.standley@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `freeze_dried_data-2.2.5/setup.py` & `freeze_dried_data-2.3.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your README file
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='freeze_dried_data',
-    version='2.2.5',
+    version='2.3.0',
     description='A simple format for machine learning datasets',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/tstandley/freeze_dried_data',
     author='Trevor Standley',
     author_email='trevor.standley@gmail.com',
     license='MIT',
```

