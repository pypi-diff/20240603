# Comparing `tmp/pbc_distance_calculator-1.3.2.tar.gz` & `tmp/pbc_distance_calculator-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbc_distance_calculator-1.3.2.tar", last modified: Fri May 10 17:55:53 2024, max compression
+gzip compressed data, was "pbc_distance_calculator-1.3.3.tar", last modified: Mon Jun  3 01:46:50 2024, max compression
```

## Comparing `pbc_distance_calculator-1.3.2.tar` & `pbc_distance_calculator-1.3.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:55:53.453881 pbc_distance_calculator-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-10 17:55:49.000000 pbc_distance_calculator-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-10 17:55:53.453881 pbc_distance_calculator-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-10 17:55:49.000000 pbc_distance_calculator-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:55:53.449881 pbc_distance_calculator-1.3.2/pbc_distance_calculator/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-10 17:55:49.000000 pbc_distance_calculator-1.3.2/pbc_distance_calculator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-05-10 17:55:49.000000 pbc_distance_calculator-1.3.2/pbc_distance_calculator/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-10 17:55:49.000000 pbc_distance_calculator-1.3.2/pbc_distance_calculator/checks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:55:53.449881 pbc_distance_calculator-1.3.2/pbc_distance_calculator/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-10 17:55:49.000000 pbc_distance_calculator-1.3.2/pbc_distance_calculator/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:55:53.449881 pbc_distance_calculator-1.3.2/pbc_distance_calculator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-10 17:55:53.000000 pbc_distance_calculator-1.3.2/pbc_distance_calculator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-10 17:55:53.000000 pbc_distance_calculator-1.3.2/pbc_distance_calculator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 17:55:53.000000 pbc_distance_calculator-1.3.2/pbc_distance_calculator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 17:55:53.000000 pbc_distance_calculator-1.3.2/pbc_distance_calculator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-10 17:55:53.000000 pbc_distance_calculator-1.3.2/pbc_distance_calculator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-10 17:55:53.453881 pbc_distance_calculator-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-10 17:55:49.000000 pbc_distance_calculator-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:46:50.841524 pbc_distance_calculator-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-06-03 01:46:43.000000 pbc_distance_calculator-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-06-03 01:46:50.841524 pbc_distance_calculator-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-06-03 01:46:43.000000 pbc_distance_calculator-1.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:46:50.837524 pbc_distance_calculator-1.3.3/pbc_distance_calculator/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-06-03 01:46:43.000000 pbc_distance_calculator-1.3.3/pbc_distance_calculator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-06-03 01:46:43.000000 pbc_distance_calculator-1.3.3/pbc_distance_calculator/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-06-03 01:46:43.000000 pbc_distance_calculator-1.3.3/pbc_distance_calculator/checks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:46:50.841524 pbc_distance_calculator-1.3.3/pbc_distance_calculator/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-06-03 01:46:43.000000 pbc_distance_calculator-1.3.3/pbc_distance_calculator/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:46:50.841524 pbc_distance_calculator-1.3.3/pbc_distance_calculator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-06-03 01:46:50.000000 pbc_distance_calculator-1.3.3/pbc_distance_calculator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-06-03 01:46:50.000000 pbc_distance_calculator-1.3.3/pbc_distance_calculator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 01:46:50.000000 pbc_distance_calculator-1.3.3/pbc_distance_calculator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-03 01:46:50.000000 pbc_distance_calculator-1.3.3/pbc_distance_calculator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-06-03 01:46:50.000000 pbc_distance_calculator-1.3.3/pbc_distance_calculator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-06-03 01:46:50.841524 pbc_distance_calculator-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-06-03 01:46:43.000000 pbc_distance_calculator-1.3.3/setup.py
```

### Comparing `pbc_distance_calculator-1.3.2/LICENSE` & `pbc_distance_calculator-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pbc_distance_calculator-1.3.2/PKG-INFO` & `pbc_distance_calculator-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbc_distance_calculator
-Version: 1.3.2
+Version: 1.3.3
 Summary: A package for computing distances accounting for periodic boundary conditions
 Home-page: https://github.com/muexly/pbc_distance_calculator
 Author: Jacob Jeffries
 Author-email: jwjeffr@clemson.edu
 License: MIT
 Keywords: periodic-boundary-conditions,distance-computation,simulation,molecular-dynamics,lattice-systems,neighbor-lists,periodic-images
 Requires-Python: <=3.12,>=3.8
```

### Comparing `pbc_distance_calculator-1.3.2/README.md` & `pbc_distance_calculator-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pbc_distance_calculator-1.3.2/pbc_distance_calculator/calculator.py` & `pbc_distance_calculator-1.3.3/pbc_distance_calculator/calculator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 module for getting pairwise distances
 """
 
 from types import ModuleType
-from typing import Callable
+from typing import Callable, no_type_check
 import warnings
 
 
 import numpy as np
 from numpy.typing import NDArray
 
 
@@ -21,19 +21,40 @@
 class WasteWarning(Warning):
 
     """
     warning for performing wasteful call to expensive engine
     """
 
 
+class UnfinishedWarning(Warning):
+
+    """
+    warning for function that isn't finished yet
+    """
+
+
+def unfinished(func: Callable) -> Callable:
+
+    """
+    decorator for warning the user that a function's implementation isn't finished
+    """
+
+    def wrapper(*args, **kwargs) -> Callable:
+        warnings.warn(
+            f"{func.__name__}'s implementation is not yet finished"
+        )
+        return func(*args, **kwargs)
+
+    return wrapper
+
+
 def private(func: Callable) -> Callable:
 
     """
     decorator for marking a function as private
-    just raises a PrivateWarning upon call
     """
 
     def wrapper(*args, **kwargs):
         warnings.warn(
             f"{func.__name__} is private and is subject to backwards-incompatible changes",
             PrivateWarning
         )
@@ -167,7 +188,51 @@
             engine=engine,
             dim_warn=dim_warn
         )
     distance = engine.linalg.norm(difference)
     if not isinstance(distance, float):
         return float(distance)
     return distance
+
+
+@no_type_check
+@unfinished
+def get_pairwise_distance_cascade(
+    positions: NDArray, cell_matrix: NDArray, engine: ModuleType, cutoff: float = np.inf
+) -> NDArray:
+
+    """
+    cascade-type algorithm for getting distances
+    work in progress
+    """
+
+    if engine.__name__ != "torch":
+        raise ValueError("cascade algorithm only works with PyTorch backend")
+
+    inverse_cell_matrix = engine.linalg.inv(cell_matrix)
+
+    sampled = set()
+    num_sites = len(positions)
+    flower = {0}
+
+    distance_tensor = engine.zeros((num_sites, num_sites))
+
+    while len(sampled) < num_sites:
+
+        differences = positions.unsqueeze(0) - positions[list(flower)].unsqueeze(1)
+        fractional_differences = engine.einsum(
+            "km,ijm->ijk", inverse_cell_matrix, differences
+        )
+        differences = differences \
+            - engine.einsum("km,ijm->ijk", cell_matrix, engine.round(fractional_differences))
+        distances = engine.linalg.norm(differences, dim=2)
+        neighbors = ((0 < distances) & (distances < cutoff)).int()
+        distances[engine.where(neighbors == 0)] = 0.0
+
+        distance_tensor[list(flower), :] = distances[..., :]
+
+        neighbor_indices = set(map(int, engine.nonzero(neighbors)[:, 1]))
+        sampled.update(flower)
+
+        flower = neighbor_indices - sampled
+
+    return distance_tensor
```

### Comparing `pbc_distance_calculator-1.3.2/pbc_distance_calculator/checks.py` & `pbc_distance_calculator-1.3.3/pbc_distance_calculator/checks.py`

 * *Files identical despite different names*

### Comparing `pbc_distance_calculator-1.3.2/pbc_distance_calculator.egg-info/PKG-INFO` & `pbc_distance_calculator-1.3.3/pbc_distance_calculator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbc_distance_calculator
-Version: 1.3.2
+Version: 1.3.3
 Summary: A package for computing distances accounting for periodic boundary conditions
 Home-page: https://github.com/muexly/pbc_distance_calculator
 Author: Jacob Jeffries
 Author-email: jwjeffr@clemson.edu
 License: MIT
 Keywords: periodic-boundary-conditions,distance-computation,simulation,molecular-dynamics,lattice-systems,neighbor-lists,periodic-images
 Requires-Python: <=3.12,>=3.8
```

### Comparing `pbc_distance_calculator-1.3.2/setup.cfg` & `pbc_distance_calculator-1.3.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = pbc_distance_calculator
 author = Jacob Jeffries
 author_email = jwjeffr@clemson.edu
 url = https://github.com/muexly/pbc_distance_calculator
 long_description_content_type = text/markdown
 long_description = file: README.md
 description = A package for computing distances accounting for periodic boundary conditions
-version = 1.3.2
+version = 1.3.3
 license = MIT
 license_files = LICENSE
 keywords = 
 	periodic-boundary-conditions
 	distance-computation
 	simulation
 	molecular-dynamics
```

