# Comparing `tmp/kgraphservice-0.0.3.tar.gz` & `tmp/kgraphservice-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kgraphservice-0.0.3.tar", last modified: Fri May 31 01:49:00 2024, max compression
+gzip compressed data, was "kgraphservice-0.0.4.tar", last modified: Mon Jun  3 02:55:55 2024, max compression
```

## Comparing `kgraphservice-0.0.3.tar` & `kgraphservice-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,25 @@
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-31 01:49:00.267253 kgraphservice-0.0.3/
--rw-r--r--   0 hadfield   (501) staff       (20)    11357 2024-05-07 11:46:32.000000 kgraphservice-0.0.3/LICENSE
--rw-r--r--   0 hadfield   (501) staff       (20)      753 2024-05-31 01:49:00.267055 kgraphservice-0.0.3/PKG-INFO
--rw-r--r--   0 hadfield   (501) staff       (20)       15 2024-05-07 11:46:32.000000 kgraphservice-0.0.3/README.md
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-31 01:49:00.265893 kgraphservice-0.0.3/kgraphservice/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-07 11:50:04.000000 kgraphservice-0.0.3/kgraphservice/__init__.py
--rw-r--r--   0 hadfield   (501) staff       (20)      422 2024-05-31 01:46:46.000000 kgraphservice-0.0.3/kgraphservice/kg_comparator.py
--rw-r--r--   0 hadfield   (501) staff       (20)     4522 2024-05-31 01:46:01.000000 kgraphservice-0.0.3/kgraphservice/kgraph_service.py
--rw-r--r--   0 hadfield   (501) staff       (20)      163 2024-05-31 01:48:26.000000 kgraphservice-0.0.3/kgraphservice/kgslot_criterion.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-31 01:49:00.266812 kgraphservice-0.0.3/kgraphservice.egg-info/
--rw-r--r--   0 hadfield   (501) staff       (20)      753 2024-05-31 01:49:00.000000 kgraphservice-0.0.3/kgraphservice.egg-info/PKG-INFO
--rw-r--r--   0 hadfield   (501) staff       (20)      333 2024-05-31 01:49:00.000000 kgraphservice-0.0.3/kgraphservice.egg-info/SOURCES.txt
--rw-r--r--   0 hadfield   (501) staff       (20)        1 2024-05-31 01:49:00.000000 kgraphservice-0.0.3/kgraphservice.egg-info/dependency_links.txt
--rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-31 01:49:00.000000 kgraphservice-0.0.3/kgraphservice.egg-info/requires.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       14 2024-05-31 01:49:00.000000 kgraphservice-0.0.3/kgraphservice.egg-info/top_level.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       38 2024-05-31 01:49:00.267298 kgraphservice-0.0.3/setup.cfg
--rw-r--r--   0 hadfield   (501) staff       (20)      948 2024-05-31 01:42:40.000000 kgraphservice-0.0.3/setup.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-06-03 02:55:55.149612 kgraphservice-0.0.4/
+-rw-r--r--   0 hadfield   (501) staff       (20)    11357 2024-05-07 11:46:32.000000 kgraphservice-0.0.4/LICENSE
+-rw-r--r--   0 hadfield   (501) staff       (20)      753 2024-06-03 02:55:55.149406 kgraphservice-0.0.4/PKG-INFO
+-rw-r--r--   0 hadfield   (501) staff       (20)       15 2024-05-07 11:46:32.000000 kgraphservice-0.0.4/README.md
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-06-03 02:55:55.147110 kgraphservice-0.0.4/kgraphservice/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-07 11:50:04.000000 kgraphservice-0.0.4/kgraphservice/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-06-03 02:55:55.148186 kgraphservice-0.0.4/kgraphservice/frame/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-06-02 22:26:29.000000 kgraphservice-0.0.4/kgraphservice/frame/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      468 2024-06-02 22:49:42.000000 kgraphservice-0.0.4/kgraphservice/frame/frame_query_executor.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     5610 2024-06-03 00:31:04.000000 kgraphservice-0.0.4/kgraphservice/frame/frame_query_generator.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      979 2024-06-02 22:40:20.000000 kgraphservice-0.0.4/kgraphservice/frame/frame_query_processor.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      422 2024-05-31 01:46:46.000000 kgraphservice-0.0.4/kgraphservice/kg_comparator.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     5420 2024-06-02 21:54:02.000000 kgraphservice-0.0.4/kgraphservice/kgraph_service.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      265 2024-06-02 22:56:42.000000 kgraphservice-0.0.4/kgraphservice/kgslot_criterion.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-06-03 02:55:55.148413 kgraphservice-0.0.4/kgraphservice/query/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-06-02 22:13:46.000000 kgraphservice-0.0.4/kgraphservice/query/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      482 2024-06-02 22:59:53.000000 kgraphservice-0.0.4/kgraphservice/query/construct_query.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-06-03 02:55:55.148917 kgraphservice-0.0.4/kgraphservice.egg-info/
+-rw-r--r--   0 hadfield   (501) staff       (20)      753 2024-06-03 02:55:55.000000 kgraphservice-0.0.4/kgraphservice.egg-info/PKG-INFO
+-rw-r--r--   0 hadfield   (501) staff       (20)      570 2024-06-03 02:55:55.000000 kgraphservice-0.0.4/kgraphservice.egg-info/SOURCES.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)        1 2024-06-03 02:55:55.000000 kgraphservice-0.0.4/kgraphservice.egg-info/dependency_links.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-06-03 02:55:55.000000 kgraphservice-0.0.4/kgraphservice.egg-info/requires.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       14 2024-06-03 02:55:55.000000 kgraphservice-0.0.4/kgraphservice.egg-info/top_level.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       38 2024-06-03 02:55:55.149726 kgraphservice-0.0.4/setup.cfg
+-rw-r--r--   0 hadfield   (501) staff       (20)      948 2024-06-02 22:21:20.000000 kgraphservice-0.0.4/setup.py
```

### Comparing `kgraphservice-0.0.3/LICENSE` & `kgraphservice-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kgraphservice-0.0.3/PKG-INFO` & `kgraphservice-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: kgraphservice
-Version: 0.0.3
+Version: 0.0.4
 Summary: KGraph Service
 Home-page: https://github.com/vital-ai/kgraphservice
 Author: Marc Hadfield
 Author-email: marc@vital.ai
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: vital-ai-vitalsigns>=0.1.14
+Requires-Dist: vital-ai-vitalsigns>=0.1.16
 Requires-Dist: vital-ai-domain>=0.1.4
 Requires-Dist: six
 Requires-Dist: pyyaml
-Requires-Dist: vital-ai-haley-kg>=0.1.8
+Requires-Dist: vital-ai-haley-kg>=0.1.9
 Requires-Dist: rdflib==7.0.0
 Requires-Dist: SPARQLWrapper==2.0.0
 Requires-Dist: networkx
 Requires-Dist: matplotlib
 
 # kgraphservice
```

### Comparing `kgraphservice-0.0.3/kgraphservice/kgraph_service.py` & `kgraphservice-0.0.4/kgraphservice/kgraph_service.py`

 * *Files 17% similar despite different names*

```diff
@@ -50,24 +50,24 @@
 
     def update_object(self, graph_object: G, graph_uri: str) -> VitalServiceStatus:
         return self.vital_service.update_object(graph_object, graph_uri)
 
     def update_object_list(self, graph_object_list: List[G], graph_uri: str) -> VitalServiceStatus:
         return self.vital_service.update_object_list(graph_object_list, graph_uri)
 
-    def get_object(self, object_uri: str, graph_uri: str = None) -> G:
+    def get_object(self, object_uri: str, graph_uri: str | None = None) -> G:
         return self.vital_service.get_object(object_uri, graph_uri)
 
-    def get_object_list(self, object_uri_list: List[str], graph_uri: str = None) -> ResultList:
+    def get_object_list(self, object_uri_list: List[str], graph_uri: str | None = None) -> ResultList:
         return self.vital_service.get_object_list(object_uri_list, graph_uri)
 
-    def delete_object(self, object_uri: str, graph_uri: str = None) -> VitalServiceStatus:
+    def delete_object(self, object_uri: str, graph_uri: str | None = None) -> VitalServiceStatus:
         return self.vital_service.delete_object(object_uri, graph_uri)
 
-    def delete_object_list(self, object_uri_list: List[str], graph_uri: str = None) -> VitalServiceStatus:
+    def delete_object_list(self, object_uri_list: List[str], graph_uri: str | None = None) -> VitalServiceStatus:
         return self.vital_service.delete_object_list(object_uri_list, graph_uri)
 
     def filter_query(self, graph_uri: str, sparql_query: str) -> ResultList:
         return self.vital_service.filter_query(graph_uri, sparql_query)
 
     def query(self, graph_uri: str, sparql_query: str) -> ResultList:
         return self.vital_service.query(sparql_query, graph_uri)
@@ -90,14 +90,36 @@
 
     def get_frame(self, graph_uri: str, frame_uri: str, limit=100, offset=0) -> ResultList:
         pass
 
     def get_frames(self, graph_uri: str, frame_uri_list: List[str], limit=100, offset=0) -> ResultList:
         pass
 
+    def get_frame_id(self, graph_uri: str, frame_id: str, limit=100, offset=0) -> ResultList:
+        pass
+
+    def get_frames_id(self, graph_uri: str, frame_id_list: List[str], limit=100, offset=0) -> ResultList:
+        pass
+
     def get_frames_root(self, graph_uri: str, root_uri: str, limit=100, offset=0) -> ResultList:
         pass
 
     def get_graph_objects_type(self, graph_uri: str, class_uri: str, include_subclasses=True, limit=100, offset=0) -> ResultList:
         pass
 
+    def get_graph_objects_tag(self, graph_uri: str, kg_graph_uri: str, limit=100, offset=0) -> ResultList:
+        pass
+
+    def delete_frame(self, graph_uri: str, frame_uri: str) -> VitalServiceStatus:
+        pass
+
+    def delete_frames(self, graph_uri: str, frame_uri_list: List[str]) -> VitalServiceStatus:
+        pass
+
+    def delete_frame_id(self, graph_uri: str, frame_id: str) -> VitalServiceStatus:
+        pass
 
+    def delete_frames_id(self, graph_uri: str, frame_id_list: List[str]) -> VitalServiceStatus:
+        pass
+
+    def delete_graph_objects_tag(self, graph_uri: str, kg_graph_uri: str) -> VitalServiceStatus:
+        pass
```

### Comparing `kgraphservice-0.0.3/kgraphservice.egg-info/PKG-INFO` & `kgraphservice-0.0.4/kgraphservice.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: kgraphservice
-Version: 0.0.3
+Version: 0.0.4
 Summary: KGraph Service
 Home-page: https://github.com/vital-ai/kgraphservice
 Author: Marc Hadfield
 Author-email: marc@vital.ai
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: vital-ai-vitalsigns>=0.1.14
+Requires-Dist: vital-ai-vitalsigns>=0.1.16
 Requires-Dist: vital-ai-domain>=0.1.4
 Requires-Dist: six
 Requires-Dist: pyyaml
-Requires-Dist: vital-ai-haley-kg>=0.1.8
+Requires-Dist: vital-ai-haley-kg>=0.1.9
 Requires-Dist: rdflib==7.0.0
 Requires-Dist: SPARQLWrapper==2.0.0
 Requires-Dist: networkx
 Requires-Dist: matplotlib
 
 # kgraphservice
```

### Comparing `kgraphservice-0.0.3/setup.py` & `kgraphservice-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name='kgraphservice',
-    version='0.0.3',
+    version='0.0.4',
     author='Marc Hadfield',
     author_email='marc@vital.ai',
     description='KGraph Service',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/vital-ai/kgraphservice',
     packages=find_packages(exclude=["test"]),
     license='Apache License 2.0',
     install_requires=[
-            'vital-ai-vitalsigns>=0.1.14',
+            'vital-ai-vitalsigns>=0.1.16',
             'vital-ai-domain>=0.1.4',
             'six',
             'pyyaml',
-            'vital-ai-haley-kg>=0.1.8',
+            'vital-ai-haley-kg>=0.1.9',
             'rdflib==7.0.0',
             'SPARQLWrapper==2.0.0',
             'networkx',
             'matplotlib',
     ],
     classifiers=[
         "Programming Language :: Python :: 3.10",
```

