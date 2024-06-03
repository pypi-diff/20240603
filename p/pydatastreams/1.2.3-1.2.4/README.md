# Comparing `tmp/pydatastreams-1.2.3.tar.gz` & `tmp/pydatastreams-1.2.4.tar.gz`

## Comparing `pydatastreams-1.2.3.tar` & `pydatastreams-1.2.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pydatastreams-1.2.3/datastream/__about__.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 pydatastreams-1.2.3/datastream/__init__.py
--rw-r--r--   0        0        0     7484 2020-02-02 00:00:00.000000 pydatastreams-1.2.3/datastream/base.py
--rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 pydatastreams-1.2.3/datastream/deserializing.py
--rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 pydatastreams-1.2.3/datastream/serializing.py
--rw-r--r--   0        0        0     3651 2020-02-02 00:00:00.000000 pydatastreams-1.2.3/datastream/twoway.py
--rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 pydatastreams-1.2.3/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 pydatastreams-1.2.3/LICENSE.txt
--rw-r--r--   0        0        0     6466 2020-02-02 00:00:00.000000 pydatastreams-1.2.3/README.md
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 pydatastreams-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     7214 2020-02-02 00:00:00.000000 pydatastreams-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pydatastreams-1.2.4/datastream/__about__.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 pydatastreams-1.2.4/datastream/__init__.py
+-rw-r--r--   0        0        0     7468 2020-02-02 00:00:00.000000 pydatastreams-1.2.4/datastream/base.py
+-rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 pydatastreams-1.2.4/datastream/deserializing.py
+-rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 pydatastreams-1.2.4/datastream/serializing.py
+-rw-r--r--   0        0        0     3651 2020-02-02 00:00:00.000000 pydatastreams-1.2.4/datastream/twoway.py
+-rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 pydatastreams-1.2.4/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 pydatastreams-1.2.4/LICENSE.txt
+-rw-r--r--   0        0        0     6466 2020-02-02 00:00:00.000000 pydatastreams-1.2.4/README.md
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 pydatastreams-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0     7214 2020-02-02 00:00:00.000000 pydatastreams-1.2.4/PKG-INFO
```

### Comparing `pydatastreams-1.2.3/datastream/base.py` & `pydatastreams-1.2.4/datastream/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,18 +11,18 @@
     Attributes:
         LITTLE_ENDIAN (int): Represents little-endian byte order.
         BIG_ENDIAN (int): Represents big-endian byte order.
         NETWORK_ENDIAN (int): Represents network byte order.
         NATIVE_ENDIAN (int): Represents native byte order.
     """
 
-    LITTLE_ENDIAN = 0
-    BIG_ENDIAN = 1
-    NETWORK_ENDIAN = 2
-    NATIVE_ENDIAN = 3
+    NETWORK_ENDIAN = 0
+    NATIVE_ENDIAN = 1
+    LITTLE_ENDIAN = 2
+    BIG_ENDIAN = 3
 
 
 _byteorder_map = "!@<>"
 
 
 class BaseStream:
     """
@@ -32,15 +32,15 @@
         backing_stream (typing.IO[bytes]): The backing stream object.
         byteorder (int): The byte order of the stream.
     """
 
     def __init__(self, backing_stream: typing.IO[bytes], byteorder: int):
         if backing_stream is None:
             return
-        
+
         if not isinstance(backing_stream, io.BytesIO):
             raise ValueError("backing_stream must be a BytesIO object")
 
         self._backing_stream = backing_stream
         self._byteorder = _byteorder_map[byteorder]
 
     @property
@@ -253,15 +253,15 @@
             if chunk == data:
                 index = self.tell() - len(data)
                 self.seek(pos)
 
                 return index
 
             remaining -= len(data)
-        
+
         return -1
 
     def clear(self):
         """
         Clears the backing stream by truncating it to 0 bytes and resetting the stream
         position to the beginning.
         """
```

### Comparing `pydatastreams-1.2.3/datastream/deserializing.py` & `pydatastreams-1.2.4/datastream/deserializing.py`

 * *Files identical despite different names*

### Comparing `pydatastreams-1.2.3/datastream/serializing.py` & `pydatastreams-1.2.4/datastream/serializing.py`

 * *Files identical despite different names*

### Comparing `pydatastreams-1.2.3/datastream/twoway.py` & `pydatastreams-1.2.4/datastream/twoway.py`

 * *Files identical despite different names*

### Comparing `pydatastreams-1.2.3/.gitignore` & `pydatastreams-1.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pydatastreams-1.2.3/LICENSE.txt` & `pydatastreams-1.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydatastreams-1.2.3/README.md` & `pydatastreams-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pydatastreams-1.2.3/pyproject.toml` & `pydatastreams-1.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydatastreams-1.2.3/PKG-INFO` & `pydatastreams-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pydatastreams
-Version: 1.2.3
+Version: 1.2.4
 Summary: A simple and easy to use library for reading and writing data streams.
 Project-URL: Homepage, https://github.com/yntha/datastream
 Project-URL: Repository, https://github.com/yntha/datastream.git
 Project-URL: Issues, https://github.com/yntha/datastream/issues
 Author-email: yntha <bguznvjk@gmail.com>
 License-File: LICENSE.txt
 Keywords: binary,data,file,io,stream
```

