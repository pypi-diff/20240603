# Comparing `tmp/llama_index_graph_stores_neo4j-0.2.1.tar.gz` & `tmp/llama_index_graph_stores_neo4j-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_graph_stores_neo4j-0.2.1.tar", max compression
+gzip compressed data, was "llama_index_graph_stores_neo4j-0.2.2.tar", max compression
```

## Comparing `llama_index_graph_stores_neo4j-0.2.1.tar` & `llama_index_graph_stores_neo4j-0.2.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       45 2024-06-01 19:48:31.027687 llama_index_graph_stores_neo4j-0.2.1/README.md
--rw-r--r--   0        0        0      188 2024-06-01 19:48:31.027687 llama_index_graph_stores_neo4j-0.2.1/llama_index/graph_stores/neo4j/__init__.py
--rw-r--r--   0        0        0     9432 2024-06-01 19:48:31.027687 llama_index_graph_stores_neo4j-0.2.1/llama_index/graph_stores/neo4j/base.py
--rw-r--r--   0        0        0    33593 2024-06-01 19:48:31.027687 llama_index_graph_stores_neo4j-0.2.1/llama_index/graph_stores/neo4j/neo4j_property_graph.py
--rw-r--r--   0        0        0     1499 2024-06-01 19:48:31.027687 llama_index_graph_stores_neo4j-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      646 1970-01-01 00:00:00.000000 llama_index_graph_stores_neo4j-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       45 2024-06-03 01:35:58.465219 llama_index_graph_stores_neo4j-0.2.2/README.md
+-rw-r--r--   0        0        0      253 2024-06-03 01:35:58.465219 llama_index_graph_stores_neo4j-0.2.2/llama_index/graph_stores/neo4j/__init__.py
+-rw-r--r--   0        0        0     9432 2024-06-03 01:35:58.465219 llama_index_graph_stores_neo4j-0.2.2/llama_index/graph_stores/neo4j/base.py
+-rw-r--r--   0        0        0    33675 2024-06-03 01:35:58.465219 llama_index_graph_stores_neo4j-0.2.2/llama_index/graph_stores/neo4j/neo4j_property_graph.py
+-rw-r--r--   0        0        0     1510 2024-06-03 01:35:58.465219 llama_index_graph_stores_neo4j-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      646 1970-01-01 00:00:00.000000 llama_index_graph_stores_neo4j-0.2.2/PKG-INFO
```

### Comparing `llama_index_graph_stores_neo4j-0.2.1/llama_index/graph_stores/neo4j/base.py` & `llama_index_graph_stores_neo4j-0.2.2/llama_index/graph_stores/neo4j/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_graph_stores_neo4j-0.2.1/llama_index/graph_stores/neo4j/neo4j_property_graph.py` & `llama_index_graph_stores_neo4j-0.2.2/llama_index/graph_stores/neo4j/neo4j_property_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 UNWIND other AS other_node
 WITH * WHERE NOT label IN $EXCLUDED_LABELS
     AND NOT other_node IN $EXCLUDED_LABELS
 RETURN {start: label, type: property, end: toString(other_node)} AS output
 """
 
 
-class Neo4jPGStore(PropertyGraphStore):
+class Neo4jPropertyGraphStore(PropertyGraphStore):
     r"""
     Neo4j Property Graph Store.
 
     This class implements a Neo4j property graph store.
 
     If you are using local Neo4j instead of aura, here's a helpful
     command for launching the docker container:
@@ -98,18 +98,18 @@
         database (Optional[str]): The name of the database to connect to. Defaults to "neo4j".
 
     Examples:
         `pip install llama-index-graph-stores-neo4j`
 
         ```python
         from llama_index.core.indices.property_graph import PropertyGraphIndex
-        from llama_index.graph_stores.neo4j import Neo4jLPGStore
+        from llama_index.graph_stores.neo4j import Neo4jPropertyGraphStore
 
-        # Create a Neo4jLPGStore instance
-        graph_store = Neo4jLPGStore(
+        # Create a Neo4jPropertyGraphStore instance
+        graph_store = Neo4jPropertyGraphStore(
             username="neo4j",
             password="neo4j",
             url="bolt://localhost:7687",
             database="neo4j"
         )
 
         # create the index
@@ -861,7 +861,10 @@
                 "\n".join(formatted_node_props),
                 "Relationship properties:",
                 "\n".join(formatted_rel_props),
                 "The relationships:",
                 "\n".join(formatted_rels),
             ]
         )
+
+
+Neo4jPGStore = Neo4jPropertyGraphStore
```

### Comparing `llama_index_graph_stores_neo4j-0.2.1/pyproject.toml` & `llama_index_graph_stores_neo4j-0.2.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -9,30 +9,30 @@
 
 [tool.llamahub]
 contains_example = false
 import_path = "llama_index.graph_stores.neo4j"
 
 [tool.llamahub.class_authors]
 Neo4jGraphStore = "llama-index"
-Neo4jPGStore = "llama-index"
+Neo4jPropertyGraphStore = "llama-index"
 
 [tool.mypy]
 disallow_untyped_defs = true
 exclude = ["_static", "build", "examples", "notebooks", "venv"]
 ignore_missing_imports = true
 python_version = "3.8"
 
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index graph stores neo4j integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-graph-stores-neo4j"
 readme = "README.md"
-version = "0.2.1"
+version = "0.2.2"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.40"
 neo4j = "^5.16.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_graph_stores_neo4j-0.2.1/PKG-INFO` & `llama_index_graph_stores_neo4j-0.2.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-graph-stores-neo4j
-Version: 0.2.1
+Version: 0.2.2
 Summary: llama-index graph stores neo4j integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

