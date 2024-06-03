# Comparing `tmp/memvectordb_python-0.0.4.tar.gz` & `tmp/memvectordb_python-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memvectordb_python-0.0.4.tar", max compression
+gzip compressed data, was "memvectordb_python-0.0.5.tar", max compression
```

## Comparing `memvectordb_python-0.0.4.tar` & `memvectordb_python-0.0.5.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     2042 2024-05-22 16:42:04.800517 memvectordb_python-0.0.4/README.md
--rw-r--r--   0        0        0        0 2024-05-22 16:42:04.800517 memvectordb_python-0.0.4/memvectordb/__init__.py
--rw-r--r--   0        0        0     8100 2024-05-22 16:42:04.800517 memvectordb_python-0.0.4/memvectordb/collection.py
--rw-r--r--   0        0        0      445 2024-05-22 16:42:04.800517 memvectordb_python-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3076 1970-01-01 00:00:00.000000 memvectordb_python-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     2042 2024-06-03 06:36:45.305848 memvectordb_python-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2024-06-03 06:36:45.309848 memvectordb_python-0.0.5/memvectordb/__init__.py
+-rw-r--r--   0        0        0     8359 2024-06-03 06:36:45.309848 memvectordb_python-0.0.5/memvectordb/collection.py
+-rw-r--r--   0        0        0     6384 2024-06-03 06:36:45.309848 memvectordb_python-0.0.5/memvectordb/memvectordb_openai.py
+-rw-r--r--   0        0        0      445 2024-06-03 06:36:45.309848 memvectordb_python-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3076 1970-01-01 00:00:00.000000 memvectordb_python-0.0.5/PKG-INFO
```

### Comparing `memvectordb_python-0.0.4/README.md` & `memvectordb_python-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `memvectordb_python-0.0.4/memvectordb/collection.py` & `memvectordb_python-0.0.5/memvectordb/collection.py`

 * *Files 10% similar despite different names*

```diff
@@ -112,14 +112,16 @@
             vector_id (int): The unique identifier for the vector.
             vector (List[float]): The vector to be inserted.
             metadata (Optional[Dict]): Additional metadata associated with the vector.
 
         Returns:
             str: Status of the insertion operation.
         """
+        if metadata:
+            metadata = {str(key): str(value) for key, value in metadata.items()}
         embedding = {
             "id": str(vector_id),
             "vector": vector,
             "metadata": metadata
         }
         payload = {
             "collection_name": collection_name,
@@ -128,15 +130,15 @@
         headers = {"Content-Type": "application/json"}
         url = f"{self.base_url}/insert_embeddings"
         response = requests.put(url, json=payload, headers=headers)
         response_data = response.json()
         if response.status_code == 200:
             return response_data
         else:
-            raise Exception(f"Failed to insert embedding: {response.status_code}")
+            return f"Failed to insert embedding: {response_data}"
         
     def batch_insert_embeddings(
         self, 
         collection_name: str, 
         embeddings: List[Dict[str, Any]]
     ) -> str:
         """
@@ -170,14 +172,17 @@
                             }
                         ]
                 }
 
         Returns:
             str: Status message indicating the success of the insertion operation.
         """
+        for emb in embeddings:
+                if emb.get("metadata"):
+                    emb["metadata"] = {str(key): str(value) for key, value in emb["metadata"].items()}
         payload = {
             "collection_name": collection_name,
             "embeddings": embeddings
         }
         headers = {"Content-Type": "application/json"}
         url = f"{self.base_url}/batch_insert_embeddings"
         response = requests.put(url, json=payload, headers=headers)
```

### Comparing `memvectordb_python-0.0.4/PKG-INFO` & `memvectordb_python-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memvectordb-python
-Version: 0.0.4
+Version: 0.0.5
 Summary: memvectordb python client.
 Home-page: https://github.com/KevKibe/memvectordb-python-client
 License: MIT
 Author: Kevin Kibe
 Author-email: keviinkibe@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
```

