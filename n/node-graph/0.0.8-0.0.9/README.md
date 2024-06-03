# Comparing `tmp/node_graph-0.0.8.tar.gz` & `tmp/node_graph-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "node_graph-0.0.8.tar", last modified: Wed May 15 05:39:10 2024, max compression
+gzip compressed data, was "node_graph-0.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `node_graph-0.0.8.tar` & `node_graph-0.0.9.tar`

### file list

```diff
@@ -1,45 +1,21 @@
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-15 05:39:10.672942 node_graph-0.0.8/
--rw-rw-r--   0 xing      (1000) xing      (1000)     1064 2023-12-03 08:36:19.000000 node_graph-0.0.8/LICENSE
--rw-r--r--   0 xing      (1000) xing      (1000)     1572 2024-05-15 05:39:10.672942 node_graph-0.0.8/PKG-INFO
--rw-rw-r--   0 xing      (1000) xing      (1000)     1131 2024-05-15 05:38:38.000000 node_graph-0.0.8/README.md
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-15 05:39:10.672942 node_graph-0.0.8/node_graph/
--rw-rw-r--   0 xing      (1000) xing      (1000)       34 2023-12-03 08:36:19.000000 node_graph-0.0.8/node_graph/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    13105 2023-12-03 08:36:19.000000 node_graph-0.0.8/node_graph/analysis.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    13072 2024-04-26 12:04:23.000000 node_graph-0.0.8/node_graph/collection.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    10230 2024-05-15 05:38:38.000000 node_graph-0.0.8/node_graph/decorator.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     3473 2023-12-03 08:36:19.000000 node_graph-0.0.8/node_graph/link.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    18403 2024-04-22 09:09:57.000000 node_graph-0.0.8/node_graph/node.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    11430 2023-12-03 08:36:19.000000 node_graph-0.0.8/node_graph/node_graph.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-15 05:39:10.672942 node_graph-0.0.8/node_graph/nodes/
--rw-rw-r--   0 xing      (1000) xing      (1000)       85 2023-12-03 08:36:19.000000 node_graph-0.0.8/node_graph/nodes/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     4600 2023-12-03 08:36:19.000000 node_graph-0.0.8/node_graph/nodes/test_nodes.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-15 05:39:10.672942 node_graph-0.0.8/node_graph/properties/
--rw-rw-r--   0 xing      (1000) xing      (1000)       93 2023-12-03 08:36:19.000000 node_graph-0.0.8/node_graph/properties/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    11956 2023-12-03 08:36:19.000000 node_graph-0.0.8/node_graph/properties/builtin.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     3331 2024-04-22 09:09:57.000000 node_graph-0.0.8/node_graph/property.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1541 2023-12-03 08:36:19.000000 node_graph-0.0.8/node_graph/serializer.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     4066 2024-04-15 12:06:25.000000 node_graph-0.0.8/node_graph/socket.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-15 05:39:10.672942 node_graph-0.0.8/node_graph/sockets/
--rw-rw-r--   0 xing      (1000) xing      (1000)       89 2023-12-03 08:36:19.000000 node_graph-0.0.8/node_graph/sockets/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     3332 2023-12-03 08:36:19.000000 node_graph-0.0.8/node_graph/sockets/builtin.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2550 2023-12-03 08:36:19.000000 node_graph-0.0.8/node_graph/utils.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      103 2023-12-03 08:36:19.000000 node_graph-0.0.8/node_graph/version.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-15 05:39:10.672942 node_graph-0.0.8/node_graph.egg-info/
--rw-r--r--   0 xing      (1000) xing      (1000)     1572 2024-05-15 05:39:10.000000 node_graph-0.0.8/node_graph.egg-info/PKG-INFO
--rw-rw-r--   0 xing      (1000) xing      (1000)      889 2024-05-15 05:39:10.000000 node_graph-0.0.8/node_graph.egg-info/SOURCES.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)        1 2024-05-15 05:39:10.000000 node_graph-0.0.8/node_graph.egg-info/dependency_links.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)      212 2024-05-15 05:39:10.000000 node_graph-0.0.8/node_graph.egg-info/entry_points.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)       50 2024-05-15 05:39:10.000000 node_graph-0.0.8/node_graph.egg-info/requires.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)       11 2024-05-15 05:39:10.000000 node_graph-0.0.8/node_graph.egg-info/top_level.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)       38 2024-05-15 05:39:10.672942 node_graph-0.0.8/setup.cfg
--rw-rw-r--   0 xing      (1000) xing      (1000)     1361 2024-05-15 05:38:55.000000 node_graph-0.0.8/setup.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-15 05:39:10.672942 node_graph-0.0.8/tests/
--rw-rw-r--   0 xing      (1000) xing      (1000)      597 2023-12-03 08:36:19.000000 node_graph-0.0.8/tests/test_collection.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2465 2024-05-15 05:38:38.000000 node_graph-0.0.8/tests/test_decorator.py
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-12-03 08:36:19.000000 node_graph-0.0.8/tests/test_entry_point.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      632 2024-04-15 12:06:25.000000 node_graph-0.0.8/tests/test_hooks.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1731 2023-12-03 08:36:19.000000 node_graph-0.0.8/tests/test_node.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      616 2023-12-03 08:36:19.000000 node_graph-0.0.8/tests/test_nodetree.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2506 2023-12-03 08:36:19.000000 node_graph-0.0.8/tests/test_property.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2152 2023-12-03 08:36:19.000000 node_graph-0.0.8/tests/test_socket.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      378 2023-12-03 08:36:19.000000 node_graph-0.0.8/tests/test_yaml.py
+-rw-r--r--   0        0        0     1131 2024-05-15 05:38:38.459236 node_graph-0.0.9/README.md
+-rw-r--r--   0        0        0       34 2023-12-03 08:36:19.206789 node_graph-0.0.9/node_graph/__init__.py
+-rw-r--r--   0        0        0    13105 2023-12-03 08:36:19.206789 node_graph-0.0.9/node_graph/analysis.py
+-rw-r--r--   0        0        0    13072 2024-04-26 12:04:23.959767 node_graph-0.0.9/node_graph/collection.py
+-rw-r--r--   0        0        0    10230 2024-05-15 05:38:38.463236 node_graph-0.0.9/node_graph/decorator.py
+-rw-r--r--   0        0        0     3473 2023-12-03 08:36:19.206789 node_graph-0.0.9/node_graph/link.py
+-rw-r--r--   0        0        0    18403 2024-04-22 09:09:57.550038 node_graph-0.0.9/node_graph/node.py
+-rw-r--r--   0        0        0    11430 2023-12-03 08:36:19.206789 node_graph-0.0.9/node_graph/node_graph.py
+-rw-r--r--   0        0        0       85 2023-12-03 08:36:19.206789 node_graph-0.0.9/node_graph/nodes/__init__.py
+-rw-r--r--   0        0        0     4600 2023-12-03 08:36:19.206789 node_graph-0.0.9/node_graph/nodes/test_nodes.py
+-rw-r--r--   0        0        0       93 2023-12-03 08:36:19.206789 node_graph-0.0.9/node_graph/properties/__init__.py
+-rw-r--r--   0        0        0    12014 2024-06-03 12:17:00.232453 node_graph-0.0.9/node_graph/properties/builtin.py
+-rw-r--r--   0        0        0     3331 2024-04-22 09:09:57.550038 node_graph-0.0.9/node_graph/property.py
+-rw-r--r--   0        0        0     1541 2023-12-03 08:36:19.206789 node_graph-0.0.9/node_graph/serializer.py
+-rw-r--r--   0        0        0     4066 2024-04-15 12:06:25.464649 node_graph-0.0.9/node_graph/socket.py
+-rw-r--r--   0        0        0       89 2023-12-03 08:36:19.206789 node_graph-0.0.9/node_graph/sockets/__init__.py
+-rw-r--r--   0        0        0     3332 2023-12-03 08:36:19.206789 node_graph-0.0.9/node_graph/sockets/builtin.py
+-rw-r--r--   0        0        0     2550 2023-12-03 08:36:19.206789 node_graph-0.0.9/node_graph/utils.py
+-rw-r--r--   0        0        0      103 2023-12-03 08:36:19.206789 node_graph-0.0.9/node_graph/version.py
+-rw-r--r--   0        0        0     1327 2024-06-03 12:17:08.126039 node_graph-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2106 1970-01-01 00:00:00.000000 node_graph-0.0.9/PKG-INFO
```

### Comparing `node_graph-0.0.8/PKG-INFO` & `node_graph-0.0.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 Metadata-Version: 2.1
 Name: node_graph
-Version: 0.0.8
+Version: 0.0.9
 Summary: Create node-based workflow
-Home-page: https://github.com/scinode/node-graph
-Author: Xing Wang
-Author-email: xingwang1991@gmail.com
-License: MIT License
+Keywords: graph,workflows
+Author-email: Xing Wang <xingwang1991@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-License-File: LICENSE
+Classifier: Development Status :: 1 - Planning
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Scientific/Engineering
 Requires-Dist: numpy
 Requires-Dist: click
 Requires-Dist: pyyaml
 Requires-Dist: colorama
 Requires-Dist: termcolor
 Requires-Dist: cloudpickle
+Project-URL: Documentation, https://node-graph.readthedocs.io
+Project-URL: Source, https://github.com/scinode/node-graph
 
 # NodeGraph
 [![PyPI version](https://badge.fury.io/py/node-graph.svg)](https://badge.fury.io/py/node-graph)
 [![CI](https://github.com/scinode/node-graph/actions/workflows/ci.yaml/badge.svg)](https://github.com/scinode/node-graph/actions/workflows/ci.yaml)
 [![codecov](https://codecov.io/gh/scinode/node-graph/branch/main/graph/badge.svg)](https://codecov.io/gh/scinode/node-graph)
 [![Docs status](https://readthedocs.org/projects/node-graph/badge)](http://node-graph.readthedocs.io/)
 
@@ -47,7 +56,8 @@
 nt.links.new(float1.outputs[0], add1.inputs[0])
 nt.links.new(float2.outputs[0], add1.inputs[1])
 ntdata = nt.to_dict()
 ```
 
 ## License
 [MIT](http://opensource.org/licenses/MIT)
+
```

### Comparing `node_graph-0.0.8/README.md` & `node_graph-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.8/node_graph/analysis.py` & `node_graph-0.0.9/node_graph/analysis.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.8/node_graph/collection.py` & `node_graph-0.0.9/node_graph/collection.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.8/node_graph/decorator.py` & `node_graph-0.0.9/node_graph/decorator.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.8/node_graph/link.py` & `node_graph-0.0.9/node_graph/link.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.8/node_graph/node.py` & `node_graph-0.0.9/node_graph/node.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.8/node_graph/node_graph.py` & `node_graph-0.0.9/node_graph/node_graph.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.8/node_graph/nodes/test_nodes.py` & `node_graph-0.0.9/node_graph/nodes/test_nodes.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.8/node_graph/properties/builtin.py` & `node_graph-0.0.9/node_graph/properties/builtin.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,76 +14,76 @@
 
 class IntProperty(NodeProperty, SerializeJson):
     """A new class for integer type."""
 
     identifier: str = "Int"
     data_type = "Int"
 
-    def __init__(self, name, description="", default=0, update=None) -> None:
+    def __init__(self, name, description="", default=None, update=None) -> None:
         super().__init__(name, description, default, update)
 
     def set_value(self, value):
         # run the callback function
-        if isinstance(value, int):
+        if isinstance(value, (int, type(None))):
             self._value = value
             if self.update is not None:
                 self.update()
         else:
             raise Exception("{} is not a integer.".format(value))
 
 
 class FloatProperty(NodeProperty, SerializeJson):
     """A new class for float type."""
 
     identifier: str = "Float"
     data_type = "Float"
 
-    def __init__(self, name, description="", default=0.0, update=None) -> None:
+    def __init__(self, name, description="", default=None, update=None) -> None:
         super().__init__(name, description, default, update)
 
     def set_value(self, value):
         # run the callback function
-        if isinstance(value, (int, float)):
+        if isinstance(value, (int, float, type(None))):
             self._value = value
             if self.update is not None:
                 self.update()
         else:
             raise Exception("{} is not a float.".format(value))
 
 
 class BoolProperty(NodeProperty, SerializeJson):
     """A new class for bool type."""
 
     identifier: str = "Bool"
     data_type = "Bool"
 
-    def __init__(self, name, description="", default=True, update=None) -> None:
+    def __init__(self, name, description="", default=None, update=None) -> None:
         super().__init__(name, description, default, update)
 
     def set_value(self, value):
         # run the callback function
-        if isinstance(value, (bool, int)):
+        if isinstance(value, (bool, int, type(None))):
             self._value = bool(value)
             if self.update is not None:
                 self.update()
         else:
             raise Exception("{} is not a bool.".format(value))
 
 
 class StringProperty(NodeProperty, SerializeJson):
     """A new class for string type."""
 
     identifier: str = "String"
     data_type = "String"
 
-    def __init__(self, name, description="", default="", update=None) -> None:
+    def __init__(self, name, description="", default=None, update=None) -> None:
         super().__init__(name, description, default, update)
 
     def set_value(self, value):
-        if isinstance(value, str):
+        if isinstance(value, (str, type(None))):
             self._value = value
             # run the callback function
             if self.update is not None:
                 self.update()
         else:
             raise Exception("{} is not a string.".format(value))
```

### Comparing `node_graph-0.0.8/node_graph/property.py` & `node_graph-0.0.9/node_graph/property.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.8/node_graph/serializer.py` & `node_graph-0.0.9/node_graph/serializer.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.8/node_graph/socket.py` & `node_graph-0.0.9/node_graph/socket.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.8/node_graph/sockets/builtin.py` & `node_graph-0.0.9/node_graph/sockets/builtin.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.8/node_graph/utils.py` & `node_graph-0.0.9/node_graph/utils.py`

 * *Files identical despite different names*

