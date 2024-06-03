# Comparing `tmp/high_order_layers_torch-2.4.2.tar.gz` & `tmp/high_order_layers_torch-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "high_order_layers_torch-2.4.2.tar", max compression
+gzip compressed data, was "high_order_layers_torch-2.5.0.tar", max compression
```

## Comparing `high_order_layers_torch-2.4.2.tar` & `high_order_layers_torch-2.5.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       75 2020-12-01 04:11:06.990013 high_order_layers_torch-2.4.2/AUTHORS
--rw-r--r--   0        0        0     1065 2020-12-01 04:11:06.990013 high_order_layers_torch-2.4.2/LICENSE
--rw-r--r--   0        0        0    16862 2024-05-18 17:50:24.922757 high_order_layers_torch-2.4.2/README.md
--rw-r--r--   0        0        0    15011 2023-12-17 04:34:43.639007 high_order_layers_torch-2.4.2/high_order_layers_torch/Basis.py
--rw-r--r--   0        0        0    17551 2022-12-03 04:01:25.774253 high_order_layers_torch-2.4.2/high_order_layers_torch/FunctionalConvolution.py
--rw-r--r--   0        0        0     5189 2022-12-03 04:01:25.774253 high_order_layers_torch-2.4.2/high_order_layers_torch/FunctionalConvolutionTranspose.py
--rw-r--r--   0        0        0     4353 2023-12-22 02:16:19.376958 high_order_layers_torch-2.4.2/high_order_layers_torch/LagrangePolynomial.py
--rw-r--r--   0        0        0    23810 2023-09-09 01:07:24.996672 high_order_layers_torch-2.4.2/high_order_layers_torch/PolynomialLayers.py
--rw-r--r--   0        0        0     1656 2022-12-03 04:01:25.774253 high_order_layers_torch-2.4.2/high_order_layers_torch/ProductLayer.py
--rw-r--r--   0        0        0        0 2020-12-01 04:11:06.994012 high_order_layers_torch-2.4.2/high_order_layers_torch/__init__.py
--rw-r--r--   0        0        0    22990 2023-04-21 03:06:49.131515 high_order_layers_torch-2.4.2/high_order_layers_torch/attentions.py
--rw-r--r--   0        0        0    10014 2023-12-30 15:03:34.401299 high_order_layers_torch-2.4.2/high_order_layers_torch/layers.py
--rw-r--r--   0        0        0     7417 2023-12-19 14:12:35.081663 high_order_layers_torch-2.4.2/high_order_layers_torch/modules.py
--rw-r--r--   0        0        0    33647 2023-12-22 02:16:19.376958 high_order_layers_torch-2.4.2/high_order_layers_torch/networks.py
--rw-r--r--   0        0        0     2488 2022-12-03 04:01:25.778253 high_order_layers_torch-2.4.2/high_order_layers_torch/positional_embeddings.py
--rw-r--r--   0        0        0       36 2023-12-30 15:03:34.401299 high_order_layers_torch-2.4.2/high_order_layers_torch/sparse_optimizers/__init__.py
--rw-r--r--   0        0        0     2708 2023-12-30 15:03:34.401299 high_order_layers_torch-2.4.2/high_order_layers_torch/sparse_optimizers/sparse_lion.py
--rw-r--r--   0        0        0     3782 2023-12-30 15:03:34.401299 high_order_layers_torch-2.4.2/high_order_layers_torch/utils.py
--rw-r--r--   0        0        0      729 2024-05-19 13:39:06.261983 high_order_layers_torch-2.4.2/pyproject.toml
--rw-r--r--   0        0        0    17703 1970-01-01 00:00:00.000000 high_order_layers_torch-2.4.2/PKG-INFO
+-rw-r--r--   0        0        0       75 2020-12-01 04:11:06.990013 high_order_layers_torch-2.5.0/AUTHORS
+-rw-r--r--   0        0        0     1065 2020-12-01 04:11:06.990013 high_order_layers_torch-2.5.0/LICENSE
+-rw-r--r--   0        0        0    17384 2024-05-29 03:40:25.856459 high_order_layers_torch-2.5.0/README.md
+-rw-r--r--   0        0        0    15011 2023-12-17 04:34:43.639007 high_order_layers_torch-2.5.0/high_order_layers_torch/Basis.py
+-rw-r--r--   0        0        0    17551 2022-12-03 04:01:25.774253 high_order_layers_torch-2.5.0/high_order_layers_torch/FunctionalConvolution.py
+-rw-r--r--   0        0        0     5189 2022-12-03 04:01:25.774253 high_order_layers_torch-2.5.0/high_order_layers_torch/FunctionalConvolutionTranspose.py
+-rw-r--r--   0        0        0     4353 2023-12-22 02:16:19.376958 high_order_layers_torch-2.5.0/high_order_layers_torch/LagrangePolynomial.py
+-rw-r--r--   0        0        0    26529 2024-06-02 13:53:30.931031 high_order_layers_torch-2.5.0/high_order_layers_torch/PolynomialLayers.py
+-rw-r--r--   0        0        0     1656 2022-12-03 04:01:25.774253 high_order_layers_torch-2.5.0/high_order_layers_torch/ProductLayer.py
+-rw-r--r--   0        0        0        0 2020-12-01 04:11:06.994012 high_order_layers_torch-2.5.0/high_order_layers_torch/__init__.py
+-rw-r--r--   0        0        0    22990 2023-04-21 03:06:49.131515 high_order_layers_torch-2.5.0/high_order_layers_torch/attentions.py
+-rw-r--r--   0        0        0    10014 2023-12-30 15:03:34.401299 high_order_layers_torch-2.5.0/high_order_layers_torch/layers.py
+-rw-r--r--   0        0        0     7417 2023-12-19 14:12:35.081663 high_order_layers_torch-2.5.0/high_order_layers_torch/modules.py
+-rw-r--r--   0        0        0    33647 2023-12-22 02:16:19.376958 high_order_layers_torch-2.5.0/high_order_layers_torch/networks.py
+-rw-r--r--   0        0        0     2488 2022-12-03 04:01:25.778253 high_order_layers_torch-2.5.0/high_order_layers_torch/positional_embeddings.py
+-rw-r--r--   0        0        0       36 2023-12-30 15:03:34.401299 high_order_layers_torch-2.5.0/high_order_layers_torch/sparse_optimizers/__init__.py
+-rw-r--r--   0        0        0     2708 2023-12-30 15:03:34.401299 high_order_layers_torch-2.5.0/high_order_layers_torch/sparse_optimizers/sparse_lion.py
+-rw-r--r--   0        0        0     3782 2023-12-30 15:03:34.401299 high_order_layers_torch-2.5.0/high_order_layers_torch/utils.py
+-rw-r--r--   0        0        0      729 2024-06-02 14:05:14.698236 high_order_layers_torch-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0    18225 1970-01-01 00:00:00.000000 high_order_layers_torch-2.5.0/PKG-INFO
```

### Comparing `high_order_layers_torch-2.4.2/LICENSE` & `high_order_layers_torch-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-2.4.2/README.md` & `high_order_layers_torch-2.5.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-
-<!---
 [![CI](https://github.com/jloveric/high-order-layers-torch/actions/workflows/python-app.yml/badge.svg)](https://github.com/jloveric/high-order-layers-torch/actions/workflows/python-app.yml)
---->
+
 
 # Piecewise Polynomial in PyTorch
 
 This is a PyTorch implementation of my tensorflow [repository](https://github.com/jloveric/high-order-layers) and is more complete due to the flexibility of PyTorch.
 
 Lagrange Polynomial, Piecewise Lagrange Polynomial, Discontinuous Piecewise Lagrange Polynomial, Fourier Series, sum and product layers in PyTorch.  The sparsity of using piecewise polynomial layers means that by adding new segments the representational power of your network increases, but the time to complete a forward step remains constant. Implementation includes simple fully connected layers, convolution layers and deconvolutional layers using these models. This is a PyTorch implementation of this [Discontinuous Piecewise Polynomial Neural Networks](https://www.researchgate.net/publication/276923198_Discontinuous_Piecewise_Polynomial_Neural_Networks) including huge number of extensions including continuous, Fourier series and convolutional neural networks... and many applications with varrying degrees of success.
 
@@ -208,14 +206,19 @@
 ```
 
 ## CIFAR100 (convolutional)
 
 ```
 python examples/cifar100.py -m max_epochs=20 train_fraction=1.0 layer_type=polynomial segments=2 n=7 nonlinearity=False rescale_output=False periodicity=2.0 lr=0.001 linear_output=False
 ```
+## Autoencoder (haven't finished implementing)
+
+```
+python examples/autoencoder.py -m max_epochs=300 train_fraction=1.0
+```
 
 ## Variational Autoencoder
 Still a WIP.  Does work, but needs improvement.
 ```
 python examples/variational_autoencoder.py -m max_epochs=300 train_fraction=1.0
 ```
 run with nevergrad for parameter tuning
@@ -318,12 +321,18 @@
   author={Loverich, John},
   journal={arXiv preprint arXiv:1505.04211},
   year={2015}
 }
 ```
 ## Notes
 
-Recently the paper [KAN: Kolmogorov–Arnold Networks](https://arxiv.org/pdf/2404.19756) was published (9 years after the original implementation of the technique in this repo), where B-splines were used on the grid. Looking at that repo, the real difference seems to be B-splines vs lagrange
+[KAN: Kolmogorov–Arnold Networks 2024](https://arxiv.org/pdf/2404.19756) was published (9 years after the original implementation of the technique in this repo), where B-splines were used on the grid. Looking at that repo, the real difference seems to be B-splines vs lagrange
 polynomials.
 
-This paper [Variations on the Chebyshev-Lagrange Activation Function](https://arxiv.org/abs/1906.10064) implements a linear extension 
-to the values beyond [-1,1] so it might be interesting to implement
+[Variations on the Chebyshev-Lagrange Activation Function](https://arxiv.org/abs/1906.10064) implements a linear extension 
+to the values beyond [-1,1] which would solve the problem of polynomial growth outside that range.
+
+[KAN: Kolmogorov–Arnold Networks: A review 2024](https://vikasdhiman.info/reviews/KAN_a_review.pdf) A review of KANs with respect to other types of networks, especially spline networks
+
+[Linear spline networks 2020](https://arxiv.org/pdf/2001.06263) 
+
+[Learning Activation Functions in Deep (Spline) Neural Networks 2020](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9264754) using B splines
```

### Comparing `high_order_layers_torch-2.4.2/high_order_layers_torch/Basis.py` & `high_order_layers_torch-2.5.0/high_order_layers_torch/Basis.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-2.4.2/high_order_layers_torch/FunctionalConvolution.py` & `high_order_layers_torch-2.5.0/high_order_layers_torch/FunctionalConvolution.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-2.4.2/high_order_layers_torch/FunctionalConvolutionTranspose.py` & `high_order_layers_torch-2.5.0/high_order_layers_torch/FunctionalConvolutionTranspose.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-2.4.2/high_order_layers_torch/LagrangePolynomial.py` & `high_order_layers_torch-2.5.0/high_order_layers_torch/LagrangePolynomial.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-2.4.2/high_order_layers_torch/PolynomialLayers.py` & `high_order_layers_torch-2.5.0/high_order_layers_torch/PolynomialLayers.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,36 +4,52 @@
 import torch
 import torch.nn as nn
 from torch.autograd import Variable
 
 from .LagrangePolynomial import *
 from .utils import *
 
+def constant_random_initialization(w, out_features, in_features, weight_magnitude, device) :
+    random_values = (
+        torch.rand(out_features, in_features, device=device)
+        * weight_magnitude
+        / in_features
+    )
+
+    # Expand the random values to match the third dimension
+    with torch.no_grad():
+        w.copy_(random_values.unsqueeze(2).expand(-1, -1, w.size(2)))
 
 class Function(nn.Module):
     def __init__(
         self,
         n: int,
         in_features: int,
         out_features: int,
         basis,
         weight_magnitude: float = 1.0,
         periodicity: float = None,
+        initialize: str = "constant_random",
+        device: str = "cpu",
         **kwargs,
     ):
         super().__init__()
         self.poly = basis
         self.n = n
         self.periodicity = periodicity
         self.w = torch.nn.Parameter(
-            data=torch.empty(out_features, in_features, n), requires_grad=True
-        )
-        self.w.data.uniform_(
-            -weight_magnitude / in_features, weight_magnitude / in_features
+            data=torch.empty(out_features, in_features, n, device=device),
+            requires_grad=True,
         )
+        if initialize == "constant_random":
+            constant_random_initialization(self.w, out_features, in_features, weight_magnitude, device)
+        else:
+            self.w.data.uniform_(
+                -weight_magnitude / in_features, weight_magnitude / in_features
+            )
 
         self.result = torch.nn.Parameter(
             data=torch.empty(out_features), requires_grad=True
         )
 
     def forward(self, x: torch.Tensor):
         periodicity = self.periodicity
@@ -84,33 +100,59 @@
         out_features: int,
         segments: int,
         length: int = 2.0,
         weight_magnitude: float = 1.0,
         poly=None,
         periodicity: float = None,
         device: str = "cpu",
+        initialize: str = "constant_random",
         **kwargs,
     ):
+        """
+        :param n: number of interpolation points in polynomial
+        :param in_features: number of input features in layer
+        :param out_features: number of outputs features in layer
+        :param segments: number of segments per link in layer
+        (1 is just a polynomial, 2 is a piecewise polynomial with 2 pieces)
+        :param length: The scale of the polynomial, 2 means it's defined on [-1, 1]
+        it continues to be defined outside, but there are no additional segments and
+        the polynomial is defined by the last (or first) segment so it will grow with
+        that polynomial order. In general you'll want your inputs to be within the range
+        [-1,1]. If you the value is 4 then it would be defined in [-2,2]
+        :param weight_magnitude: The maximum value of initial weights during initialization.
+        :param poly: The polynomial function to use within each segment
+        :param periodicity: Tells which scale to provide mirror periodicity, if your length
+        is 2 then setting this value to 2 means it will be mirror periodic outside the
+        domain [-1,1]. This is an older approach I used, but instead I mainly use normalization
+        to keep the values within range
+        :param device: The device 'cpu' or 'cuda' in general
+        :param initialize: if set to "constant_random" then within each link the intial function will
+        be a constant, but it will be a random constant in each link. limit is set by weight_magnitude.
+        If not set, then it defaults to random uniform.
+        """
         super().__init__()
         self._poly = poly(n)
         self._n = n
         self._segments = segments
         self.in_features = in_features
         self.out_features = out_features
         self.periodicity = periodicity
         self.device = device
         self.w = torch.nn.Parameter(
             data=torch.empty(
                 out_features, in_features, ((n - 1) * segments + 1), device=device
             ),
             requires_grad=True,
         )
-        self.w.data.uniform_(
-            -weight_magnitude / in_features, weight_magnitude / in_features
-        )
+        if initialize == "constant_random":
+            constant_random_initialization(self.w, out_features, in_features, weight_magnitude, device)
+        else:
+            self.w.data.uniform_(
+                -weight_magnitude / in_features, weight_magnitude / in_features
+            )
         self.wrange = None
         self._length = length
         self._half = 0.5 * length
 
     def which_segment(self, x: torch.Tensor) -> Tensor:
         """
         Return the segment(s) the x are in.  This is being added for
@@ -287,29 +329,33 @@
         out_features: int,
         segments: int,
         length=2.0,
         weight_magnitude=1.0,
         poly=None,
         periodicity: float = None,
         device: str = "cpu",
+        initialize: str = "contant_random",
         **kwargs,
     ):
         super().__init__()
         self._n = n
         self.device = device
         self._poly = poly(self._n)
         self._segments = segments
         self.in_features = in_features
         self.out_features = out_features
         self.periodicity = periodicity
         self.w = torch.nn.Parameter(
             data=torch.empty(out_features, in_features, n * segments, device=device),
             requires_grad=True,
         )
-        self.w.data.uniform_(-1 / in_features, 1 / in_features)
+        if initialize == "constant_random":
+            constant_random_initialization(self.w, out_features, in_features, weight_magnitude, device)
+        else:
+            self.w.data.uniform_(-1 / in_features, 1 / in_features)
 
         self._length = length
         self._half = 0.5 * length
 
     @property
     def n(self) -> int:
         """
@@ -720,14 +766,15 @@
     if isinstance(layer_in, PiecewisePolynomial):
         nodes_per_segment = n_in - 1
         upper_limit = 1
     elif isinstance(layer_in, PiecewiseDiscontinuous):
         nodes_per_segment = n_in
         upper_limit = 0
 
+    # TODO: this is very slow, it needs to be sped up
     with torch.no_grad():  # No grad so we can assign leaf variable in place
         for inputs in range(w_in.shape[0]):
             for outputs in range(w_in.shape[1]):
                 a = max_slope * (random.random() * 2 - 1.0)
                 b = max_offset * (random.random() * 2 - 1.0)
 
                 for j in range(segments_in):
```

### Comparing `high_order_layers_torch-2.4.2/high_order_layers_torch/ProductLayer.py` & `high_order_layers_torch-2.5.0/high_order_layers_torch/ProductLayer.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-2.4.2/high_order_layers_torch/attentions.py` & `high_order_layers_torch-2.5.0/high_order_layers_torch/attentions.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-2.4.2/high_order_layers_torch/layers.py` & `high_order_layers_torch-2.5.0/high_order_layers_torch/layers.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-2.4.2/high_order_layers_torch/modules.py` & `high_order_layers_torch-2.5.0/high_order_layers_torch/modules.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-2.4.2/high_order_layers_torch/networks.py` & `high_order_layers_torch-2.5.0/high_order_layers_torch/networks.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-2.4.2/high_order_layers_torch/positional_embeddings.py` & `high_order_layers_torch-2.5.0/high_order_layers_torch/positional_embeddings.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-2.4.2/high_order_layers_torch/sparse_optimizers/sparse_lion.py` & `high_order_layers_torch-2.5.0/high_order_layers_torch/sparse_optimizers/sparse_lion.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-2.4.2/high_order_layers_torch/utils.py` & `high_order_layers_torch-2.5.0/high_order_layers_torch/utils.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-2.4.2/PKG-INFO` & `high_order_layers_torch-2.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: high-order-layers-torch
-Version: 2.4.2
+Version: 2.5.0
 Summary: High order layers in pytorch
 License: MIT
 Author: jloverich
 Author-email: john.loverich@gmail.com
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -17,18 +17,16 @@
 Requires-Dist: pytorch-lightning (>=2.0.0,<3.0.0)
 Requires-Dist: torch (>=2.1.1)
 Requires-Dist: torch-optimizer (>=0.3.0,<0.4.0)
 Requires-Dist: torchmetrics (>=1.2.1,<2.0.0)
 Requires-Dist: torchvision (>=0.18.0)
 Description-Content-Type: text/markdown
 
-
-<!---
 [![CI](https://github.com/jloveric/high-order-layers-torch/actions/workflows/python-app.yml/badge.svg)](https://github.com/jloveric/high-order-layers-torch/actions/workflows/python-app.yml)
---->
+
 
 # Piecewise Polynomial in PyTorch
 
 This is a PyTorch implementation of my tensorflow [repository](https://github.com/jloveric/high-order-layers) and is more complete due to the flexibility of PyTorch.
 
 Lagrange Polynomial, Piecewise Lagrange Polynomial, Discontinuous Piecewise Lagrange Polynomial, Fourier Series, sum and product layers in PyTorch.  The sparsity of using piecewise polynomial layers means that by adding new segments the representational power of your network increases, but the time to complete a forward step remains constant. Implementation includes simple fully connected layers, convolution layers and deconvolutional layers using these models. This is a PyTorch implementation of this [Discontinuous Piecewise Polynomial Neural Networks](https://www.researchgate.net/publication/276923198_Discontinuous_Piecewise_Polynomial_Neural_Networks) including huge number of extensions including continuous, Fourier series and convolutional neural networks... and many applications with varrying degrees of success.
 
@@ -231,14 +229,19 @@
 ```
 
 ## CIFAR100 (convolutional)
 
 ```
 python examples/cifar100.py -m max_epochs=20 train_fraction=1.0 layer_type=polynomial segments=2 n=7 nonlinearity=False rescale_output=False periodicity=2.0 lr=0.001 linear_output=False
 ```
+## Autoencoder (haven't finished implementing)
+
+```
+python examples/autoencoder.py -m max_epochs=300 train_fraction=1.0
+```
 
 ## Variational Autoencoder
 Still a WIP.  Does work, but needs improvement.
 ```
 python examples/variational_autoencoder.py -m max_epochs=300 train_fraction=1.0
 ```
 run with nevergrad for parameter tuning
@@ -341,12 +344,18 @@
   author={Loverich, John},
   journal={arXiv preprint arXiv:1505.04211},
   year={2015}
 }
 ```
 ## Notes
 
-Recently the paper [KAN: Kolmogorov–Arnold Networks](https://arxiv.org/pdf/2404.19756) was published (9 years after the original implementation of the technique in this repo), where B-splines were used on the grid. Looking at that repo, the real difference seems to be B-splines vs lagrange
+[KAN: Kolmogorov–Arnold Networks 2024](https://arxiv.org/pdf/2404.19756) was published (9 years after the original implementation of the technique in this repo), where B-splines were used on the grid. Looking at that repo, the real difference seems to be B-splines vs lagrange
 polynomials.
 
-This paper [Variations on the Chebyshev-Lagrange Activation Function](https://arxiv.org/abs/1906.10064) implements a linear extension 
-to the values beyond [-1,1] so it might be interesting to implement
+[Variations on the Chebyshev-Lagrange Activation Function](https://arxiv.org/abs/1906.10064) implements a linear extension 
+to the values beyond [-1,1] which would solve the problem of polynomial growth outside that range.
+
+[KAN: Kolmogorov–Arnold Networks: A review 2024](https://vikasdhiman.info/reviews/KAN_a_review.pdf) A review of KANs with respect to other types of networks, especially spline networks
+
+[Linear spline networks 2020](https://arxiv.org/pdf/2001.06263) 
+
+[Learning Activation Functions in Deep (Spline) Neural Networks 2020](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9264754) using B splines
```

