# Comparing `tmp/pydatastreams-1.2.1.tar.gz` & `tmp/pydatastreams-1.2.2.tar.gz`

## Comparing `pydatastreams-1.2.1.tar` & `pydatastreams-1.2.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pydatastreams-1.2.1/datastream/__about__.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 pydatastreams-1.2.1/datastream/__init__.py
--rw-r--r--   0        0        0     7484 2020-02-02 00:00:00.000000 pydatastreams-1.2.1/datastream/base.py
--rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 pydatastreams-1.2.1/datastream/deserializing.py
--rw-r--r--   0        0        0     4168 2020-02-02 00:00:00.000000 pydatastreams-1.2.1/datastream/serializing.py
--rw-r--r--   0        0        0     3651 2020-02-02 00:00:00.000000 pydatastreams-1.2.1/datastream/twoway.py
--rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 pydatastreams-1.2.1/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 pydatastreams-1.2.1/LICENSE.txt
--rw-r--r--   0        0        0     6466 2020-02-02 00:00:00.000000 pydatastreams-1.2.1/README.md
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 pydatastreams-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     7214 2020-02-02 00:00:00.000000 pydatastreams-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pydatastreams-1.2.2/datastream/__about__.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 pydatastreams-1.2.2/datastream/__init__.py
+-rw-r--r--   0        0        0     7484 2020-02-02 00:00:00.000000 pydatastreams-1.2.2/datastream/base.py
+-rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 pydatastreams-1.2.2/datastream/deserializing.py
+-rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 pydatastreams-1.2.2/datastream/serializing.py
+-rw-r--r--   0        0        0     3651 2020-02-02 00:00:00.000000 pydatastreams-1.2.2/datastream/twoway.py
+-rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 pydatastreams-1.2.2/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 pydatastreams-1.2.2/LICENSE.txt
+-rw-r--r--   0        0        0     6466 2020-02-02 00:00:00.000000 pydatastreams-1.2.2/README.md
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 pydatastreams-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     7214 2020-02-02 00:00:00.000000 pydatastreams-1.2.2/PKG-INFO
```

### Comparing `pydatastreams-1.2.1/datastream/base.py` & `pydatastreams-1.2.2/datastream/base.py`

 * *Files identical despite different names*

### Comparing `pydatastreams-1.2.1/datastream/deserializing.py` & `pydatastreams-1.2.2/datastream/deserializing.py`

 * *Files identical despite different names*

### Comparing `pydatastreams-1.2.1/datastream/serializing.py` & `pydatastreams-1.2.2/datastream/serializing.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,36 +28,36 @@
     def __bytes__(self) -> bytes: # type: ignore
         return self.bytes()
 
     def write_format(self, fmt: str, value: typing.Any):
         self.write(struct.pack(self._byteorder + fmt, value))
 
     def write_int64(self, value: int):
-        self.write_format("q", value)
+        self.write_format("q", value & 0xFFFFFFFFFFFFFFFF)
 
     def write_uint64(self, value: int):
-        self.write_format("Q", value)
+        self.write_format("Q", value & 0xFFFFFFFFFFFFFFFF)
 
     def write_int32(self, value: int):
-        self.write_format("i", value)
+        self.write_format("i", value & 0xFFFFFFFF)
 
     def write_uint32(self, value: int):
-        self.write_format("I", value)
+        self.write_format("I", value & 0xFFFFFFFF)
 
     def write_int16(self, value: int):
-        self.write_format("h", value)
+        self.write_format("h", value & 0xFFFF)
 
     def write_uint16(self, value: int):
-        self.write_format("H", value)
+        self.write_format("H", value & 0xFFFF)
 
     def write_int8(self, value: int):
-        self.write_format("b", value)
+        self.write_format("b", value & 0xFF)
 
     def write_uint8(self, value: int):
-        self.write_format("B", value)
+        self.write_format("B", value & 0xFF)
 
     def write_float(self, value: float):
         self.write_format("f", value)
 
     def write_double(self, value: float):
         self.write_format("d", value)
```

### Comparing `pydatastreams-1.2.1/datastream/twoway.py` & `pydatastreams-1.2.2/datastream/twoway.py`

 * *Files identical despite different names*

### Comparing `pydatastreams-1.2.1/.gitignore` & `pydatastreams-1.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pydatastreams-1.2.1/LICENSE.txt` & `pydatastreams-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydatastreams-1.2.1/README.md` & `pydatastreams-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pydatastreams-1.2.1/pyproject.toml` & `pydatastreams-1.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydatastreams-1.2.1/PKG-INFO` & `pydatastreams-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pydatastreams
-Version: 1.2.1
+Version: 1.2.2
 Summary: A simple and easy to use library for reading and writing data streams.
 Project-URL: Homepage, https://github.com/yntha/datastream
 Project-URL: Repository, https://github.com/yntha/datastream.git
 Project-URL: Issues, https://github.com/yntha/datastream/issues
 Author-email: yntha <bguznvjk@gmail.com>
 License-File: LICENSE.txt
 Keywords: binary,data,file,io,stream
```
