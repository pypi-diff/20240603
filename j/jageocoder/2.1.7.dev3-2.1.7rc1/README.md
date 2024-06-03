# Comparing `tmp/jageocoder-2.1.7.dev3.tar.gz` & `tmp/jageocoder-2.1.7rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jageocoder-2.1.7.dev3.tar", max compression
+gzip compressed data, was "jageocoder-2.1.7rc1.tar", max compression
```

## Comparing `jageocoder-2.1.7.dev3.tar` & `jageocoder-2.1.7rc1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      113 2024-05-08 05:06:37.205667 jageocoder-2.1.7.dev3/LICENSE
--rw-r--r--   0        0        0    10479 2024-05-21 05:12:27.142531 jageocoder-2.1.7.dev3/README.md
--rw-r--r--   0        0        0     1571 2024-05-27 08:42:50.618126 jageocoder-2.1.7.dev3/jageocoder/__init__.py
--rw-r--r--   0        0        0     5759 2024-05-08 03:51:15.514717 jageocoder-2.1.7.dev3/jageocoder/__main__.py
--rw-r--r--   0        0        0     3489 2024-05-21 05:12:27.146530 jageocoder-2.1.7.dev3/jageocoder/address.py
--rw-r--r--   0        0        0     8320 2024-04-15 00:39:35.469528 jageocoder-2.1.7.dev3/jageocoder/aza_master.py
--rw-r--r--   0        0        0     1171 2024-05-02 04:32:53.380509 jageocoder-2.1.7.dev3/jageocoder/dataset.py
--rw-r--r--   0        0        0      837 2024-05-08 03:51:15.514717 jageocoder-2.1.7.dev3/jageocoder/exceptions.py
--rw-r--r--   0        0        0    19415 2024-04-15 00:39:35.469528 jageocoder-2.1.7.dev3/jageocoder/itaiji.py
--rw-r--r--   0        0        0    14220 2023-08-03 02:25:59.209435 jageocoder-2.1.7.dev3/jageocoder/itaiji_dic.json
--rw-r--r--   0        0        0    16470 2024-05-21 05:12:27.146530 jageocoder-2.1.7.dev3/jageocoder/module.py
--rw-r--r--   0        0        0    55833 2024-05-29 02:17:31.044550 jageocoder-2.1.7.dev3/jageocoder/node.py
--rw-r--r--   0        0        0    12219 2024-05-29 02:30:47.289873 jageocoder-2.1.7.dev3/jageocoder/remote.py
--rw-r--r--   0        0        0     3898 2024-05-08 03:51:15.514717 jageocoder-2.1.7.dev3/jageocoder/result.py
--rw-r--r--   0        0        0    20182 2024-05-28 09:35:05.185780 jageocoder-2.1.7.dev3/jageocoder/rtree.py
--rw-r--r--   0        0        0     7795 2023-09-27 08:08:26.315234 jageocoder-2.1.7.dev3/jageocoder/strlib.py
--rw-r--r--   0        0        0    44808 2024-05-29 02:36:07.055241 jageocoder-2.1.7.dev3/jageocoder/tree.py
--rw-r--r--   0        0        0     4995 2023-08-03 02:25:59.213435 jageocoder-2.1.7.dev3/jageocoder/trie.py
--rw-r--r--   0        0        0     1308 2024-05-27 08:42:50.626126 jageocoder-2.1.7.dev3/pyproject.toml
--rw-r--r--   0        0        0    12021 1970-01-01 00:00:00.000000 jageocoder-2.1.7.dev3/PKG-INFO
+-rw-r--r--   0        0        0      113 2024-05-08 05:06:37.205667 jageocoder-2.1.7rc1/LICENSE
+-rw-r--r--   0        0        0    10479 2024-05-21 05:12:27.142531 jageocoder-2.1.7rc1/README.md
+-rw-r--r--   0        0        0     1570 2024-06-03 07:24:20.820284 jageocoder-2.1.7rc1/jageocoder/__init__.py
+-rw-r--r--   0        0        0     5759 2024-05-08 03:51:15.514717 jageocoder-2.1.7rc1/jageocoder/__main__.py
+-rw-r--r--   0        0        0     3489 2024-05-21 05:12:27.146530 jageocoder-2.1.7rc1/jageocoder/address.py
+-rw-r--r--   0        0        0     8320 2024-04-15 00:39:35.469528 jageocoder-2.1.7rc1/jageocoder/aza_master.py
+-rw-r--r--   0        0        0     1171 2024-05-02 04:32:53.380509 jageocoder-2.1.7rc1/jageocoder/dataset.py
+-rw-r--r--   0        0        0      837 2024-05-08 03:51:15.514717 jageocoder-2.1.7rc1/jageocoder/exceptions.py
+-rw-r--r--   0        0        0    19415 2024-04-15 00:39:35.469528 jageocoder-2.1.7rc1/jageocoder/itaiji.py
+-rw-r--r--   0        0        0    14220 2023-08-03 02:25:59.209435 jageocoder-2.1.7rc1/jageocoder/itaiji_dic.json
+-rw-r--r--   0        0        0    16470 2024-05-21 05:12:27.146530 jageocoder-2.1.7rc1/jageocoder/module.py
+-rw-r--r--   0        0        0    55833 2024-05-29 03:50:14.310936 jageocoder-2.1.7rc1/jageocoder/node.py
+-rw-r--r--   0        0        0    12219 2024-05-29 03:50:14.314936 jageocoder-2.1.7rc1/jageocoder/remote.py
+-rw-r--r--   0        0        0     3898 2024-05-08 03:51:15.514717 jageocoder-2.1.7rc1/jageocoder/result.py
+-rw-r--r--   0        0        0    17708 2024-06-03 07:31:45.609424 jageocoder-2.1.7rc1/jageocoder/rtree.py
+-rw-r--r--   0        0        0     7795 2023-09-27 08:08:26.315234 jageocoder-2.1.7rc1/jageocoder/strlib.py
+-rw-r--r--   0        0        0    44811 2024-05-29 03:50:14.314936 jageocoder-2.1.7rc1/jageocoder/tree.py
+-rw-r--r--   0        0        0     4995 2023-08-03 02:25:59.213435 jageocoder-2.1.7rc1/jageocoder/trie.py
+-rw-r--r--   0        0        0     1307 2024-06-03 07:24:32.180521 jageocoder-2.1.7rc1/pyproject.toml
+-rw-r--r--   0        0        0    12019 1970-01-01 00:00:00.000000 jageocoder-2.1.7rc1/PKG-INFO
```

### Comparing `jageocoder-2.1.7.dev3/README.md` & `jageocoder-2.1.7rc1/README.md`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.7.dev3/jageocoder/__init__.py` & `jageocoder-2.1.7rc1/jageocoder/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 running the following steps.
 
     >>> import jageocoder
     >>> jageocoder.init()
     >>> jageocoder.searchNode('<Japanese-address>')
 """
 
-__version__ = '2.1.7.dev3'  # The package version
+__version__ = '2.1.7.rc1'  # The package version
 __dictionary_version__ = '20230927'  # Compatible dictionary version
 __author__ = 'Takeshi Sagara <sagara@info-proto.com>'
 
 __all__ = [
     'init',
     'free',
     'is_initialized',
```

### Comparing `jageocoder-2.1.7.dev3/jageocoder/__main__.py` & `jageocoder-2.1.7rc1/jageocoder/__main__.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.7.dev3/jageocoder/address.py` & `jageocoder-2.1.7rc1/jageocoder/address.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.7.dev3/jageocoder/aza_master.py` & `jageocoder-2.1.7rc1/jageocoder/aza_master.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.7.dev3/jageocoder/dataset.py` & `jageocoder-2.1.7rc1/jageocoder/dataset.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.7.dev3/jageocoder/exceptions.py` & `jageocoder-2.1.7rc1/jageocoder/exceptions.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.7.dev3/jageocoder/itaiji.py` & `jageocoder-2.1.7rc1/jageocoder/itaiji.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.7.dev3/jageocoder/itaiji_dic.json` & `jageocoder-2.1.7rc1/jageocoder/itaiji_dic.json`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.7.dev3/jageocoder/module.py` & `jageocoder-2.1.7rc1/jageocoder/module.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.7.dev3/jageocoder/node.py` & `jageocoder-2.1.7rc1/jageocoder/node.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.7.dev3/jageocoder/remote.py` & `jageocoder-2.1.7rc1/jageocoder/remote.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.7.dev3/jageocoder/result.py` & `jageocoder-2.1.7rc1/jageocoder/result.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.7.dev3/jageocoder/rtree.py` & `jageocoder-2.1.7rc1/jageocoder/rtree.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from abc import ABC
-import copy
 from logging import getLogger
 import os
 from typing import Iterable, List, Optional, Tuple
 
 from geographiclib.geodesic import Geodesic
 from rtree import index
 from rtree.exceptions import RTreeError
@@ -317,36 +316,88 @@
         index.Rtree
             Created rtree index.
         """
         file_idx = index.Rtree(str(treepath))
         node_table: AddressNodeTable = self._tree.address_nodes
 
         max_id = node_table.count_records()
+        registered_coordinates = set()
 
         logger.info("Building RTree for reverse geocoding...")
         id = AddressNode.ROOT_NODE_ID
         with tqdm(total=max_id, mininterval=0.5, ascii=True) as pbar:
             prev_id = 0
             while id < max_id:
                 pbar.update(id - prev_id)
                 prev_id = id
 
                 node = node_table.get_record(pos=id)
-                if node.level <= AddressLevel.WARD or node.level > AddressLevel.BLOCK:
+                if node.level <= AddressLevel.WARD:
+                    registered_coordinates.clear()
                     id += 1
                     continue
 
-                if not node.has_valid_coordinate_values():
-                    node = node.add_dummy_coordinates()
+                if node.sibling_id == node.id + 1:
+                    # The node has no child nodes
+
+                    if not node.has_valid_coordinate_values():
+                        id += 1
+                        continue
+
+                    key = (node.x, node.y)
+                    if key in registered_coordinates:
+                        id += 1
+                        continue
 
-                if node.has_valid_coordinate_values():
                     file_idx.insert(
                         id=id,
                         coordinates=(node.x, node.y, node.x, node.y),
                     )
+                    registered_coordinates.add(key)
+                    id += 1
+                    continue
+
+                # The node has 1 or more child nodes
+                if node.level == AddressLevel.BLOCK:
+                    # Get BDR of child nodes
+                    bdr = None
+                    for child_id in range(node.id + 1, node.sibling_id):
+                        child_node = node_table.get_record(child_id)
+                        if not child_node.has_valid_coordinate_values():
+                            continue
+
+                        if bdr is None:
+                            bdr = (child_node.x, child_node.y,
+                                   child_node.x, child_node.y)
+                        else:
+                            bdr = (
+                                min(child_node.x, bdr[0]),
+                                min(child_node.y, bdr[1]),
+                                max(child_node.x, bdr[2]),
+                                max(child_node.y, bdr[3]),
+                            )
+
+                    if bdr:
+                        file_idx.insert(
+                            id=id,
+                            coordinates=bdr,
+                        )
+                    else:
+                        # All child nodes have invalid coordinate values
+                        key = (node.x, node.y)
+                        if node.has_valid_coordinate_values() and \
+                                key not in registered_coordinates:
+                            file_idx.insert(
+                                id=id,
+                                coordinates=(node.x, node.y, node.x, node.y),
+                            )
+                            registered_coordinates.add(key)
+
+                    id = node.sibling_id
+                    continue
 
                 id += 1
 
         return file_idx
 
     def load_rtree(self, treepath: os.PathLike) -> index.Rtree:
         """
@@ -393,51 +444,43 @@
         results = tuple(self.idx.nearest((node.x, node.y, node.x, node.y), 20))
         return len(results) > 0 and node.id in results
 
     def _sort_by_dist(
         self,
         lon: float,
         lat: float,
-        id_list: Iterable[int],
-        node_map: Optional[dict] = None,
-    ) -> Tuple[List[NodeDist], dict]:
+        nodes: Iterable[AddressNode],
+    ) -> List[NodeDist]:
         """
         Sort nodes by real(projected) distance from the target point.
 
         Paramters
         ---------
         lon: float
             The longitude of the target point.
         lat: float
             The latitude of the target point.
-        id_list: Iterable[int]
-            The list of node-id.
+        nodes: Iterable[AddressNode]
+            The list of candidate node.
 
         Returns
         -------
-        Tuple[List[NodeDist], dict]
-            The sorted list of (distance, address node) and a node map.
+        List[NodeDist]
+            The sorted list of (distance, address node).
         """
-        node_map = node_map or {}
         results = []
-        for node_id in set(id_list):
-            node = self._tree.get_node_by_id(node_id=node_id)
+        for node in nodes:
             if not node.has_valid_coordinate_values():
-                node = node.add_dummy_coordinates()
+                continue
 
-            key = (node.x, node.y)
-            if key in node_map:
-                node_map[key].append(node)
-            else:
-                node_map[key] = [node]
-                dist = self.distance(node.x, node.y, lon, lat)
-                results.append(NodeDist(dist, node))
+            dist = self.distance(node.x, node.y, lon, lat)
+            results.append(NodeDist(dist, node))
 
         results.sort(key=lambda x: x.dist)
-        return (results, node_map)
+        return results
 
     def nearest(
         self,
         x: float,
         y: float,
         level: Optional[int] = None,
         as_dict: Optional[bool] = True,
@@ -459,125 +502,33 @@
             in the "candidate" field.
 
         Returns
         -------
         [{"candidate":AddressNode or dict, "dist":float}]
             Returns the results of retrieval up to 3 nodes.
         """
-
-        def _remove_parent_nodes(
-            candidates: Iterable[NodeDist]
-        ) -> List[NodeDist]:
-            ancestors = set()
-            max_level = 0
-            if len(candidates) == 0:
-                return []
-
-            nodes = []
-            for v in candidates:
-                dist, node = v.dist, v.node
-                if node.id in ancestors:
-                    continue
-
-                if not node.has_valid_coordinate_values():
-                    node = node.add_dummy_coordinates()
-
-                nodes.append(NodeDist(dist, node))
-                max_level = max(max_level, node.level)
-
-                # List ancestor nodes of registering node.
-                cur = node.parent
-                while cur is not None:
-                    # nodes = [node for node in nodes if node.id != cur.id]
-                    ancestors.add(cur.id)
-                    cur = cur.parent
-
-            # Exclude ancestor nodes
-            nodes = [node for node in nodes if node.node.id not in ancestors]
-            return nodes
-
-        def _get_k_nearest_child_nodes(
-            aza_node_dists: List[NodeDist],
-            *,
-            candidates: Optional[List[NodeDist]] = None,
-            node_map: Optional[dict] = None,
-            k: Optional[int] = 20,
-            min_k: Optional[int] = 0,
-            max_dist: Optional[float] = 500.0,
-        ) -> Tuple[List[NodeDist], dict]:
-            candidates = candidates or []
-            node_map = node_map or {}
-            for v in aza_node_dists:
-                dist, node = v.dist, v.node
-                child_id = node.id + 1
-                for child_id in range(node.id + 1, node.sibling_id):
-                    child_node = self._tree.get_node_by_id(
-                        node_id=child_id)
-                    if child_node.level > level:
-                        continue
-
-                    if not child_node.has_valid_coordinate_values():
-                        if child_node.level == level:
-                            continue
-
-                        child_node = child_node.add_dummy_coordinates()
-                        if not child_node.has_valid_coordinate_values():
-                            continue
-
-                    key = (child_node.x, child_node.y)
-                    if key in node_map:
-                        # A node with the same coordinates are already registered
-                        node_map[key].append(child_node)
-                        continue
-
-                    dist = self.distance(x, y, child_node.x, child_node.y)
-                    i = len(candidates)
-                    while i > 0:
-                        if dist >= candidates[i - 1].dist:
-                            break
-
-                        i -= 1
-
-                    if i < min_k or (i < k and dist <= max_dist):
-                        candidates.insert(i, NodeDist(dist, child_node))
-                        node_map[key] = [child_node]
-                        n = len(candidates)
-                        if n > k:
-                            delnode = candidates[k].node
-                            del candidates[k]
-                            delkey = (delnode.x, delnode.y)
-                            node_map[delkey].remove(delnode)
-                            if len(node_map[delkey]) == 0:
-                                del node_map[delkey]
-
-                        elif n > min_k and candidates[min_k].dist > max_dist:
-                            delnode = candidates[min_k].node
-                            del candidates[min_k]
-                            delkey = (delnode.x, delnode.y)
-                            node_map[delkey].remove(delnode)
-                            if len(node_map[delkey]) == 0:
-                                del node_map[delkey]
-
-            return (candidates, node_map)
-
         level = level or AddressLevel.AZA
 
         # Retrieve top k-nearest nodes using the R-tree index.
-        nearests = self.idx.nearest((x, y, x, y), 20)
-        node_dists, node_map = self._sort_by_dist(x, y, nearests)
-        node_dists = _remove_parent_nodes(node_dists)
-
-        if level > AddressLevel.BLOCK:
-            candidates, node_map = _get_k_nearest_child_nodes(
-                node_dists,
-                candidates=copy.copy(node_dists),
-                node_map=node_map,
-                min_k=1)
+        # If the node registered in the index is an intermediate node,
+        # expand its leaf nodes.
+        candidates = []
+        nearests = self.idx.nearest((x, y, x, y), 20, objects=True)
+        for item in nearests:
+            node = self._tree.get_node_by_id(item.id)
+            if item.bbox[0] == item.bbox[2] and item.bbox[1] == item.bbox[3]:
+                candidates.append(node)
+            else:
+                for child_id in range(node.id + 1, node.sibling_id):
+                    child_node = self._tree.get_node_by_id(child_id)
+                    if child_node.sibling_id == child_id + 1 and \
+                            child_node.has_valid_coordinate_values():
+                        candidates.append(child_node)
 
-            node_dists = _remove_parent_nodes(candidates)
+        node_dists = self._sort_by_dist(x, y, candidates)
 
         # Select the 3 nodes that make the smallest triangle
         # surrounding the target point
         if len(node_dists) == 0:
             return []
 
         if len(node_dists) <= 3 or node_dists[0].dist < 1.0e-02:
@@ -585,45 +536,25 @@
             # less than 1 cm, it returns three points in order of distance.
             # This is because the nearest point may not be included in
             # the search results due to a calculation error.
             node_dists = node_dists[0:3]
         else:
             node_dists = DelaunayTriangle.select(x, y, node_dists)
 
-        # Restore nodes with the same coordinates
-        if node_map is not None:
-            _node_dists = []
-            for v in node_dists:
-                dist, node = v.dist, v.node
-                key = (node.x, node.y)
-                for n in node_map[key]:
-                    _node_dists.append(NodeDist(dist, n))
-
-            node_dists = _node_dists
-
         # Convert nodes to the dict format.
         results = []
         registered = set()
         for v in node_dists:
             dist, node = v.dist, v.node
             while node.level > level:
                 node = node.parent
-                dist = None
-                if not node.has_valid_coordinate_values():
-                    node.x, node.y = v.node.x, v.node.y
 
             if node.id in registered:
                 continue
 
-            if dist is None:
-                dist = self.distance(x, y, node.x, node.y)
-
             results.append({
                 "candidate": node.as_dict() if as_dict else node,
                 "dist": dist
             })
             registered.add(node.id)
 
-        # Sort by distance
-        results = sorted(results, key=lambda r: r['dist'])
-
         return results
```

### Comparing `jageocoder-2.1.7.dev3/jageocoder/strlib.py` & `jageocoder-2.1.7rc1/jageocoder/strlib.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.7.dev3/jageocoder/tree.py` & `jageocoder-2.1.7rc1/jageocoder/tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -845,15 +845,15 @@
             logger.debug("Trie_id of key '{}' = {}".format(
                 k, trie_id))
             trie_node = self.trie_nodes.get_record(pos=trie_id)
             offset = self.converter.match_len(index, k)
             key = index[0:offset]
             rest_index = index[offset:]
             for node_id in trie_node.nodes:
-                node = self.get_address_node(id=node_id)
+                node = self.get_node_by_id(node_id=node_id)
 
                 if not node.has_valid_coordinate_values() \
                         and self.get_config('require_coordinates'):
                     node = node.add_dummy_coordinates()
 
                 if min_key == '' and node.level <= AddressLevel.WARD:
                     # To make the process quicker, once a node higher
```

### Comparing `jageocoder-2.1.7.dev3/jageocoder/trie.py` & `jageocoder-2.1.7rc1/jageocoder/trie.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.7.dev3/pyproject.toml` & `jageocoder-2.1.7rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jageocoder"
-version = "2.1.7.dev3"
+version = "2.1.7.rc1"
 description = "A Japanese-address geocoder for Python."
 authors = ["Takeshi Sagara <sagara@info-proto.com>"]
 repository = "https://github.com/t-sagara/jageocoder/"
 license = "The MIT License"
 readme = "README.md"
 documentation = "https://jageocoder.readthedocs.io/"
 packages = [
```

### Comparing `jageocoder-2.1.7.dev3/PKG-INFO` & `jageocoder-2.1.7rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jageocoder
-Version: 2.1.7.dev3
+Version: 2.1.7rc1
 Summary: A Japanese-address geocoder for Python.
 Home-page: https://github.com/t-sagara/jageocoder/
 License: The MIT License
 Author: Takeshi Sagara
 Author-email: sagara@info-proto.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

