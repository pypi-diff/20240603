# Comparing `tmp/thoi-0.1.13.tar.gz` & `tmp/thoi-0.1.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thoi-0.1.13.tar", last modified: Sat Jun  1 05:34:09 2024, max compression
+gzip compressed data, was "thoi-0.1.14.tar", last modified: Sun Jun  2 23:17:07 2024, max compression
```

## Comparing `thoi-0.1.13.tar` & `thoi-0.1.14.tar`

### file list

```diff
@@ -1,29 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:34:09.853999 thoi-0.1.13/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:34:09.849999 thoi-0.1.13/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:34:09.853999 thoi-0.1.13/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-06-01 05:33:54.000000 thoi-0.1.13/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-06-01 05:33:54.000000 thoi-0.1.13/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-06-01 05:34:09.853999 thoi-0.1.13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-06-01 05:33:54.000000 thoi-0.1.13/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 05:33:54.000000 thoi-0.1.13/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 05:34:09.853999 thoi-0.1.13/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-06-01 05:33:54.000000 thoi-0.1.13/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:34:09.853999 thoi-0.1.13/thoi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 05:33:54.000000 thoi-0.1.13/thoi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-06-01 05:33:54.000000 thoi-0.1.13/thoi/collectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-06-01 05:33:54.000000 thoi-0.1.13/thoi/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-06-01 05:33:54.000000 thoi-0.1.13/thoi/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:34:09.853999 thoi-0.1.13/thoi/measures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 05:33:54.000000 thoi-0.1.13/thoi/measures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7268 2024-06-01 05:33:54.000000 thoi-0.1.13/thoi/measures/gaussian_copula.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:34:09.853999 thoi-0.1.13/thoi/synthetic_systems/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-06-01 05:33:54.000000 thoi-0.1.13/thoi/synthetic_systems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-06-01 05:33:54.000000 thoi-0.1.13/thoi/synthetic_systems/flat.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-06-01 05:33:54.000000 thoi-0.1.13/thoi/synthetic_systems/relu.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-06-01 05:33:54.000000 thoi-0.1.13/thoi/synthetic_systems/xor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:34:09.853999 thoi-0.1.13/thoi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-06-01 05:34:09.000000 thoi-0.1.13/thoi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-06-01 05:34:09.000000 thoi-0.1.13/thoi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 05:34:09.000000 thoi-0.1.13/thoi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-01 05:34:09.000000 thoi-0.1.13/thoi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-06-01 05:34:09.000000 thoi-0.1.13/thoi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 23:17:07.209483 thoi-0.1.14/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 23:17:07.201484 thoi-0.1.14/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 23:17:07.205484 thoi-0.1.14/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-06-02 23:17:02.000000 thoi-0.1.14/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-06-02 23:17:02.000000 thoi-0.1.14/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-06-02 23:17:02.000000 thoi-0.1.14/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-06-02 23:17:07.209483 thoi-0.1.14/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-06-02 23:17:02.000000 thoi-0.1.14/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 23:17:02.000000 thoi-0.1.14/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 23:17:07.209483 thoi-0.1.14/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-06-02 23:17:02.000000 thoi-0.1.14/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 23:17:07.205484 thoi-0.1.14/thoi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 23:17:02.000000 thoi-0.1.14/thoi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-06-02 23:17:02.000000 thoi-0.1.14/thoi/collectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-06-02 23:17:02.000000 thoi-0.1.14/thoi/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-06-02 23:17:02.000000 thoi-0.1.14/thoi/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 23:17:07.205484 thoi-0.1.14/thoi/heuristics/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-06-02 23:17:02.000000 thoi-0.1.14/thoi/heuristics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-06-02 23:17:02.000000 thoi-0.1.14/thoi/heuristics/greedy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-06-02 23:17:02.000000 thoi-0.1.14/thoi/heuristics/simulated_annealing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 23:17:07.205484 thoi-0.1.14/thoi/measures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 23:17:02.000000 thoi-0.1.14/thoi/measures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-06-02 23:17:02.000000 thoi-0.1.14/thoi/measures/gaussian_copula.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 23:17:07.209483 thoi-0.1.14/thoi/synthetic_systems/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-06-02 23:17:02.000000 thoi-0.1.14/thoi/synthetic_systems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-06-02 23:17:02.000000 thoi-0.1.14/thoi/synthetic_systems/flat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-06-02 23:17:02.000000 thoi-0.1.14/thoi/synthetic_systems/relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-06-02 23:17:02.000000 thoi-0.1.14/thoi/synthetic_systems/xor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 23:17:07.209483 thoi-0.1.14/thoi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-06-02 23:17:07.000000 thoi-0.1.14/thoi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-06-02 23:17:07.000000 thoi-0.1.14/thoi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 23:17:07.000000 thoi-0.1.14/thoi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-02 23:17:07.000000 thoi-0.1.14/thoi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-06-02 23:17:07.000000 thoi-0.1.14/thoi.egg-info/top_level.txt
```

### Comparing `thoi-0.1.13/.github/workflows/python-publish.yml` & `thoi-0.1.14/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `thoi-0.1.13/LICENSE` & `thoi-0.1.14/LICENSE`

 * *Files identical despite different names*

### Comparing `thoi-0.1.13/PKG-INFO` & `thoi-0.1.14/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thoi
-Version: 0.1.13
+Version: 0.1.14
 Summary: Torch - Higher Order Interactions
 Home-page: https://github.com/Laouen/THOI
 Author: Laouen Mayal Louan Belloli, Ruben Herzog
 Author-email: laouen.belloli@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -69,20 +69,42 @@
         ```
 
 ## Usage
 
 After installation, you can start using THOI in your projects. Here is a simple example:
 
 ```python
-from thoi.measures.gaussian_copula import multi_order_measures
+from thoi.measures.gaussian_copula import multi_order_measures, nplets_measures
+from thoi.heuristics import simulated_annealing, greedy
 import numpy as np
 
 X = np.random.normal(0,1, (1000, 10))
 
+# Computation of O information for the entire system
+measures = nplets_measures(X)
+
+# Computation of O info for the sub-system composed by 0, 1 and 3
+measures = nplets_measures(X, [0,1,3])
+
+# Computation of O info for the sub-system composed by 0, 1 and 3
+measures = nplets_measures(X, [[0,1,3],[3,7,4],[2,6,3]])
+
+# Extensive computation of O information measures over all combinations of X
 measures = multi_order_measures(X)
+
+# compute the best 10 combinations using greedy, starting by exaustive search in 
+# lower order and building from there. Result shows best O information for 
+# each built optimal orders
+best_partitions, best_scores = greedy(X, 3, 5, repeat=10)
+
+# compute the best 10 combinations using simulated annealing: There are two initialization options
+# 1. Starting by exaustive search in lower order, then building with gready.
+# 2. Selection random sample of initial solutions.
+# Result shows best O information for each built optimal orders
+best_partitions, best_scores = simulated_annealing(X, 5, repeat=10)
 ```
 
 For detailed usage and examples, please refer to the [documentation](https://github.com/Laouen/THOI).
 
 ## Contributing
 
 We welcome contributions from the community. If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request on GitHub.
```

### Comparing `thoi-0.1.13/README.md` & `thoi-0.1.14/thoi.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: thoi
+Version: 0.1.14
+Summary: Torch - Higher Order Interactions
+Home-page: https://github.com/Laouen/THOI
+Author: Laouen Mayal Louan Belloli, Ruben Herzog
+Author-email: laouen.belloli@gmail.com
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: tqdm
+Requires-Dist: scipy
+Requires-Dist: pandas
+Requires-Dist: networkx
+
 # THOI: Torch - Higher Order Interactions
 
 ## Description
 
 THOI is a Python package designed to compute O information in Higher Order Interactions using batch processing. This package leverages PyTorch for efficient tensor operations.
 
 ## Installation
@@ -48,20 +69,42 @@
         ```
 
 ## Usage
 
 After installation, you can start using THOI in your projects. Here is a simple example:
 
 ```python
-from thoi.measures.gaussian_copula import multi_order_measures
+from thoi.measures.gaussian_copula import multi_order_measures, nplets_measures
+from thoi.heuristics import simulated_annealing, greedy
 import numpy as np
 
 X = np.random.normal(0,1, (1000, 10))
 
+# Computation of O information for the entire system
+measures = nplets_measures(X)
+
+# Computation of O info for the sub-system composed by 0, 1 and 3
+measures = nplets_measures(X, [0,1,3])
+
+# Computation of O info for the sub-system composed by 0, 1 and 3
+measures = nplets_measures(X, [[0,1,3],[3,7,4],[2,6,3]])
+
+# Extensive computation of O information measures over all combinations of X
 measures = multi_order_measures(X)
+
+# compute the best 10 combinations using greedy, starting by exaustive search in 
+# lower order and building from there. Result shows best O information for 
+# each built optimal orders
+best_partitions, best_scores = greedy(X, 3, 5, repeat=10)
+
+# compute the best 10 combinations using simulated annealing: There are two initialization options
+# 1. Starting by exaustive search in lower order, then building with gready.
+# 2. Selection random sample of initial solutions.
+# Result shows best O information for each built optimal orders
+best_partitions, best_scores = simulated_annealing(X, 5, repeat=10)
 ```
 
 For detailed usage and examples, please refer to the [documentation](https://github.com/Laouen/THOI).
 
 ## Contributing
 
 We welcome contributions from the community. If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request on GitHub.
@@ -71,8 +114,8 @@
 This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
 
 ## Authors
 
 - [Laouen Mayal Louan Belloli](https://www.linkedin.com/in/laouen-belloli/)
 - [Ruben Herzog](https://www.linkedin.com/in/rherzoga/)
 
-For more details, visit the [GitHub repository](https://github.com/Laouen/THOI).
+For more details, visit the [GitHub repository](https://github.com/Laouen/THOI).
```

### Comparing `thoi-0.1.13/setup.py` & `thoi-0.1.14/setup.py`

 * *Files identical despite different names*

### Comparing `thoi-0.1.13/thoi/dataset.py` & `thoi-0.1.14/thoi/dataset.py`

 * *Files 23% similar despite different names*

```diff
@@ -25,7 +25,28 @@
                 - partition_covmat (np.ndarray): The submatrix of the covariance matrix corresponding to the current combination, shape (order, order).
         """
         for partition_idxs in self.partitions_generator:
             partition_idxs = np.array(partition_idxs)
 
             # (order, order)
             yield partition_idxs, self.matrix[partition_idxs][:,partition_idxs]
+
+
+class NpletsCovariancesDataset(IterableDataset):
+    def __init__(self, matrix: torch.tensor, nplets: torch.tensor):
+        self.matrix = matrix
+        self.nplets = nplets
+
+    def __len__(self):
+        """Returns the number of combinations of features of the specified order."""
+        return len(self.nplets)
+
+    def __iter__(self):
+        """
+        Iterate over all combinations of features in the dataset.
+
+        Yields:
+            tuple: A tuple containing:
+                partition_covmat (np.ndarray): The submatrix of the covariance matrix corresponding to the current combination, shape (order, order).
+        """
+        for partition_idxs in self.nplets:
+            yield self.matrix[partition_idxs][:,partition_idxs]
```

### Comparing `thoi-0.1.13/thoi/graph.py` & `thoi-0.1.14/thoi/graph.py`

 * *Files identical despite different names*

### Comparing `thoi-0.1.13/thoi/measures/gaussian_copula.py` & `thoi-0.1.14/thoi/measures/gaussian_copula.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from typing import Optional, Callable
+from typing import Optional, Callable, Union
 
 from tqdm.autonotebook import tqdm
 from functools import partial
 
 import pandas as pd
 import scipy as sp
 import numpy as np
 import torch
 from torch.utils.data import DataLoader
 
 from ..dataset import CovarianceDataset
 from ..collectors import batch_to_csv
 
 
-def gaussianCopula(X):
+def gaussian_copula(X):
     """
     Transform the data into a Gaussian copula and compute the covariance matrix.
     
     Parameters:
     - X: A 2D numpy array of shape (T, N) where T is the number of samples and N is the number of variables.
     
     Returns:
@@ -94,39 +94,79 @@
     nplet_o = nplet_tc - nplet_dtc
     # |bz|
     nplet_s = nplet_tc + nplet_dtc
 
     return nplet_tc, nplet_dtc, nplet_o, nplet_s
 
 
-def nplet_measures(X: np.ndarray):
-    device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
+def nplets_measures(X: Union[np.ndarray, torch.tensor],
+                    nplets: Optional[Union[np.ndarray,torch.tensor]] = None,
+                    T:int = None,
+                    covmat_precomputed:bool = False,
+                    use_cpu:bool = False):
+
+    # Handle different options for X parameter
+    # Accept multivariate data or covariance matrix
+    if covmat_precomputed:
+        N1, N = X.shape
+        assert N1 == N, 'Covariance matrix should be a squared matrix'
+        covmat = X if torch.is_tensor(X) else torch.tensor(X)
+    else:
+        assert not torch.is_tensor(X), 'Not precomputed covariance should be numpys'
+        T, N = X.shape
+        covmat = torch.tensor(gaussian_copula(X)[1])
+
+    # Handle different options for nplet parameter
+    # Compute for the entire systems
+    if nplets is None:
+        nplets = torch.arange(N)
+
+    # If nplets are not tensors, convert to tensor
+    if not torch.is_tensor(nplets):
+        nplets = torch.tensor(nplets)
+
+    # If only nplet to calculate
+    if len(nplets.shape) < 2:
+        nplets = torch.unsqueeze(nplets, dim=0)
 
-    T, N = np.shape(X)
 
-    covmat = gaussianCopula(X)[1]
-    covmat = torch.Tensor(np.expand_dims(covmat, axis=0))
-    covmat.to(device)
+    # Process in correct device
+    # Send elements to cuda if computing on GPU
+    using_GPU = torch.cuda.is_available() and not use_cpu
+    device = torch.device('cuda' if using_GPU else 'cpu')
+    covmat = covmat.to(device)
+    nplets = nplets.to(device)
 
-    allmin1 = _all_min_1_ids(N)
+    # Generate the covariance matrices for each nplet
+    # |batch_size| x |order| x |order|
+    nplets_covmat = torch.stack([
+        covmat[nplet_idxs][:,nplet_idxs]
+        for nplet_idxs in nplets
+    ])
+
+    # Compute measures
+    # Compute bias corrector
+    _, order = nplets.shape
+    allmin1 = _all_min_1_ids(order)
     bc1 = _gaussian_entropy_bias_correction(1,T)
-    bcN = _gaussian_entropy_bias_correction(N,T)
-    bcNmin1 = _gaussian_entropy_bias_correction(N-1,T)
+    bcN = _gaussian_entropy_bias_correction(order,T)
+    bcNmin1 = _gaussian_entropy_bias_correction(order-1,T)
 
-    nplet_tc, nplet_dtc, nplet_o, nplet_s = _get_tc_dtc_from_batched_covmat(
-        covmat, allmin1, bc1, bcN, bcNmin1
-    )
-
-    return (
-        nplet_tc.cpu().numpy()[0],
-        nplet_dtc.cpu().numpy()[0],
-        nplet_o.cpu().numpy()[0],
-        nplet_s.cpu().numpy()[0]
-    )
+    # Batch process all nplets at once
+    # batch_res = (nplet_tc, nplet_dtc, nplet_o, nplet_s)
+    results = torch.stack(_get_tc_dtc_from_batched_covmat(
+        nplets_covmat, allmin1, bc1, bcN, bcNmin1
+    )).T
+
+    # If only one result, return is as value not list
+    if results.shape[0] == 1:
+        results = torch.squeeze(results, dim=0)
 
+    return results
+    
 
 def multi_order_measures(X: np.ndarray,
                         min_order: int=3,
                         max_order: Optional[int]=None,
                         batch_size: int = 1000000,
                         use_cpu: bool = False,
                         batch_aggregation: Optional[Callable[[any],any]] = None,
@@ -158,15 +198,15 @@
     assert min_order <= max_order, f"min_order must be lower or equal than max_order. {min_order} > {max_order}"
 
     # make device cpu if not cuda available or cuda if available
     using_GPU = torch.cuda.is_available() and not use_cpu
     device = torch.device('cuda' if using_GPU else 'cpu')
 
     # Gaussian Copula of data
-    covmat = gaussianCopula(X)[1]
+    covmat = gaussian_copula(X)[1]
 
     # To compute using pytorch, we need to compute each order separately
     batched_data = []
     pbar_order = tqdm(range(min_order, max_order+1), leave=False, desc='Order', disable=(min_order==max_order))
     for order in pbar_order:
 
         # Calculate constant values valid for all n-plets of the current order
@@ -190,17 +230,17 @@
         for bn, (partition_idxs, partition_covmat) in enumerate(pbar):
             partition_covmat = partition_covmat.to(device)
             nplets_tc, nplets_dtc, nplets_o, nplets_s = _get_tc_dtc_from_batched_covmat(
                 partition_covmat, allmin1, bc1, bcN, bcNmin1
             )
 
             data = batch_data_collector(
-                partition_idxs.cpu().numpy(),
-                nplets_o.cpu().numpy(),
-                nplets_s.cpu().numpy(),
-                nplets_tc.cpu().numpy(),
-                nplets_dtc.cpu().numpy(),
+                partition_idxs,
+                nplets_o,
+                nplets_s,
+                nplets_tc,
+                nplets_dtc,
                 bn
             )
             batched_data.append(data)
 
     return batch_aggregation(batched_data)
```

### Comparing `thoi-0.1.13/thoi/synthetic_systems/flat.py` & `thoi-0.1.14/thoi/synthetic_systems/flat.py`

 * *Files identical despite different names*

### Comparing `thoi-0.1.13/thoi/synthetic_systems/relu.py` & `thoi-0.1.14/thoi/synthetic_systems/relu.py`

 * *Files identical despite different names*

