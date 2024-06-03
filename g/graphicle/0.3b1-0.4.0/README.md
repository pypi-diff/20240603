# Comparing `tmp/graphicle-0.3b1.tar.gz` & `tmp/graphicle-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphicle-0.3b1.tar", last modified: Mon Mar  4 13:31:14 2024, max compression
+gzip compressed data, was "graphicle-0.4.0.tar", last modified: Mon Jun  3 09:35:23 2024, max compression
```

## Comparing `graphicle-0.3b1.tar` & `graphicle-0.4.0.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:31:14.761495 graphicle-0.3b1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:31:14.753495 graphicle-0.3b1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:31:14.757495 graphicle-0.3b1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-03-04 13:31:08.000000 graphicle-0.3b1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-03-04 13:31:08.000000 graphicle-0.3b1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-03-04 13:31:08.000000 graphicle-0.3b1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-03-04 13:31:08.000000 graphicle-0.3b1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-04 13:31:08.000000 graphicle-0.3b1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-03-04 13:31:08.000000 graphicle-0.3b1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11248 2024-03-04 13:31:14.761495 graphicle-0.3b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8585 2024-03-04 13:31:08.000000 graphicle-0.3b1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:31:14.757495 graphicle-0.3b1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-04 13:31:08.000000 graphicle-0.3b1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-04 13:31:08.000000 graphicle-0.3b1/docs/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-04 13:31:08.000000 graphicle-0.3b1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-04 13:31:08.000000 graphicle-0.3b1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:31:14.757495 graphicle-0.3b1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:31:14.757495 graphicle-0.3b1/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 13:31:08.000000 graphicle-0.3b1/docs/source/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:31:14.757495 graphicle-0.3b1/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 13:31:08.000000 graphicle-0.3b1/docs/source/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-03-04 13:31:08.000000 graphicle-0.3b1/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6915 2024-03-04 13:31:08.000000 graphicle-0.3b1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-03-04 13:31:08.000000 graphicle-0.3b1/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:31:14.761495 graphicle-0.3b1/graphicle/
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-04 13:31:08.000000 graphicle-0.3b1/graphicle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-03-04 13:31:14.000000 graphicle-0.3b1/graphicle/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-03-04 13:31:08.000000 graphicle-0.3b1/graphicle/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    35355 2024-03-04 13:31:08.000000 graphicle-0.3b1/graphicle/calculate.py
--rw-r--r--   0 runner    (1001) docker     (127)    90678 2024-03-04 13:31:08.000000 graphicle-0.3b1/graphicle/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-03-04 13:31:08.000000 graphicle-0.3b1/graphicle/matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 13:31:08.000000 graphicle-0.3b1/graphicle/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    49418 2024-03-04 13:31:08.000000 graphicle-0.3b1/graphicle/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-03-04 13:31:08.000000 graphicle-0.3b1/graphicle/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:31:14.761495 graphicle-0.3b1/graphicle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11248 2024-03-04 13:31:14.000000 graphicle-0.3b1/graphicle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-03-04 13:31:14.000000 graphicle-0.3b1/graphicle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 13:31:14.000000 graphicle-0.3b1/graphicle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-04 13:31:14.000000 graphicle-0.3b1/graphicle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-04 13:31:14.000000 graphicle-0.3b1/graphicle.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-03-04 13:31:08.000000 graphicle-0.3b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 13:31:14.761495 graphicle-0.3b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-04 13:31:08.000000 graphicle-0.3b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:31:14.761495 graphicle-0.3b1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-03-04 13:31:08.000000 graphicle-0.3b1/tests/test_calculate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-03-04 13:31:08.000000 graphicle-0.3b1/tests/test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:35:23.394267 graphicle-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:35:23.386267 graphicle-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:35:23.386267 graphicle-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-06-03 09:35:18.000000 graphicle-0.4.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-06-03 09:35:18.000000 graphicle-0.4.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-06-03 09:35:18.000000 graphicle-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-06-03 09:35:18.000000 graphicle-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-06-03 09:35:18.000000 graphicle-0.4.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-06-03 09:35:18.000000 graphicle-0.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11248 2024-06-03 09:35:23.394267 graphicle-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8585 2024-06-03 09:35:18.000000 graphicle-0.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:35:23.390267 graphicle-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-06-03 09:35:18.000000 graphicle-0.4.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-06-03 09:35:18.000000 graphicle-0.4.0/docs/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-06-03 09:35:18.000000 graphicle-0.4.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-06-03 09:35:18.000000 graphicle-0.4.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:35:23.390267 graphicle-0.4.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:35:23.390267 graphicle-0.4.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:35:18.000000 graphicle-0.4.0/docs/source/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:35:23.390267 graphicle-0.4.0/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:35:18.000000 graphicle-0.4.0/docs/source/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-06-03 09:35:18.000000 graphicle-0.4.0/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6915 2024-06-03 09:35:18.000000 graphicle-0.4.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-06-03 09:35:18.000000 graphicle-0.4.0/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:35:23.390267 graphicle-0.4.0/graphicle/
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-06-03 09:35:18.000000 graphicle-0.4.0/graphicle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-03 09:35:23.000000 graphicle-0.4.0/graphicle/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-06-03 09:35:18.000000 graphicle-0.4.0/graphicle/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29314 2024-06-03 09:35:18.000000 graphicle-0.4.0/graphicle/calculate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    94543 2024-06-03 09:35:18.000000 graphicle-0.4.0/graphicle/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-06-03 09:35:18.000000 graphicle-0.4.0/graphicle/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:35:18.000000 graphicle-0.4.0/graphicle/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    49419 2024-06-03 09:35:18.000000 graphicle-0.4.0/graphicle/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8146 2024-06-03 09:35:18.000000 graphicle-0.4.0/graphicle/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:35:23.394267 graphicle-0.4.0/graphicle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11248 2024-06-03 09:35:23.000000 graphicle-0.4.0/graphicle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-06-03 09:35:23.000000 graphicle-0.4.0/graphicle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 09:35:23.000000 graphicle-0.4.0/graphicle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-06-03 09:35:23.000000 graphicle-0.4.0/graphicle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-03 09:35:23.000000 graphicle-0.4.0/graphicle.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-06-03 09:35:18.000000 graphicle-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 09:35:23.394267 graphicle-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-03 09:35:18.000000 graphicle-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:35:23.394267 graphicle-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-06-03 09:35:18.000000 graphicle-0.4.0/tests/test_calculate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-06-03 09:35:18.000000 graphicle-0.4.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-06-03 09:35:18.000000 graphicle-0.4.0/tests/test_transform.py
```

### Comparing `graphicle-0.3b1/.github/workflows/publish-to-pypi.yml` & `graphicle-0.4.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `graphicle-0.3b1/.github/workflows/tests.yml` & `graphicle-0.4.0/.github/workflows/tests.yml`

 * *Files 20% similar despite different names*

```diff
@@ -4,25 +4,26 @@
   - push
 
 jobs:
   test:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        os: [ubuntu-latest, macos-latest]
+        os: [ubuntu-latest, macos-13]
         pyver: ["3.8", "3.9", "3.10", "3.11"]
     steps:
       - uses: actions/checkout@v3
       - uses: mamba-org/setup-micromamba@v1
         with:
-          micromamba-version: '1.3.1-0'
+          micromamba-version: '1.5.6-0'
           environment-name: test-env
           create-args: >-
             python=${{ matrix.pyver }}
             pytest>=6.2.5
+            libtool
           init-shell: bash
           cache-environment: true
           post-cleanup: 'all'
 
       - name: Install graphicle
         shell: bash -el {0}
         run: pip install .
```

### Comparing `graphicle-0.3b1/.gitignore` & `graphicle-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `graphicle-0.3b1/.pre-commit-config.yaml` & `graphicle-0.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `graphicle-0.3b1/LICENSE.txt` & `graphicle-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `graphicle-0.3b1/PKG-INFO` & `graphicle-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphicle
-Version: 0.3b1
+Version: 0.4.0
 Summary: Encode particle physics data onto graph structures.
 Author: Jacan Chaplais
 Maintainer: Jacan Chaplais
 License: BSD 3-Clause License
         
         Copyright (c) 2021, Jacan Chaplais.
         All rights reserved.
```

### Comparing `graphicle-0.3b1/README.rst` & `graphicle-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `graphicle-0.3b1/docs/Makefile` & `graphicle-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `graphicle-0.3b1/docs/make.bat` & `graphicle-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `graphicle-0.3b1/docs/source/api.rst` & `graphicle-0.4.0/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `graphicle-0.3b1/docs/source/conf.py` & `graphicle-0.4.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `graphicle-0.3b1/docs/source/index.rst` & `graphicle-0.4.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `graphicle-0.3b1/graphicle/__init__.py` & `graphicle-0.4.0/graphicle/__init__.py`

 * *Files identical despite different names*

### Comparing `graphicle-0.3b1/graphicle/base.py` & `graphicle-0.4.0/graphicle/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -41,14 +41,43 @@
 AnyVector = npt.NDArray[ty.Any]
 VoidVector = npt.NDArray[np.void]
 MaskLike = ty.Union["MaskBase", BoolVector]
 DoubleUfunc = ty.TypeVar("DoubleUfunc", DoubleVector, np.float64)
 DataType = ty.TypeVar("DataType")
 
 
+class LheEventInterface(ty.Protocol):
+    """Interface for a generic Les Houches event.
+
+    :group: base
+
+    .. versionadded:: 0.4.0
+    """
+
+    @property
+    def pdg(self) -> IntVector:
+        ...
+
+    @property
+    def pmu(self) -> AnyVector:
+        ...
+
+    @property
+    def color(self) -> AnyVector:
+        ...
+
+    @property
+    def helicity(self) -> HalfIntVector:
+        ...
+
+    @property
+    def status(self) -> HalfIntVector:
+        ...
+
+
 class EventInterface(ty.Protocol):
     """Defines the interface for a generic event object expected by
     graphicle's routines. Attributes are stored as numpy arrays, with
     each element corresponding to a particle in an event. Attributes
     with 'fields' are numpy structured arrays.
 
     :group: base
```

### Comparing `graphicle-0.3b1/graphicle/calculate.py` & `graphicle-0.4.0/graphicle/calculate.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,140 +9,43 @@
 import contextlib as ctx
 import functools as fn
 import itertools as it
 import math
 import operator as op
 import typing as ty
 import warnings
-from functools import lru_cache, partial
 
-import networkx as nx
 import numba as nb
 import numpy as np
 import numpy.lib.recfunctions as rfn
 import scipy.optimize as spo
-from deprecation import deprecated
 
 from . import base
 
 if ty.TYPE_CHECKING is True:
     from graphicle.data import *
 
 __all__ = [
-    "azimuth_centre",
-    "pseudorapidity_centre",
-    "rapidity_centre",
     "weighted_centroid",
     "resultant_coords",
     "combined_mass",
-    "flow_trace",
     "aggregate_momenta",
     "cluster_coeff_distbn",
     "thrust",
     "spherocity",
     "c_parameter",
     "jaccard_distance",
 ]
 
 
 PMU_DTYPE = nb.typeof(
     np.empty(1, dtype=np.dtype(list(zip("xyze", ("<f8",) * 4))))
 )
 
 
-@deprecated(
-    deprecated_in="0.3.1",
-    removed_in="0.4.0",
-    details="Use ``weighted_centroid()`` or ``resultant_coords()`` instead.",
-)
-def azimuth_centre(pmu: "MomentumArray", pt_weight: bool = True) -> float:
-    """Calculates the central point in azimuth for a set of particles.
-
-    :group: calculate
-
-    .. versionadded:: 0.1.7
-
-    .. versionchanged:: 0.3.1
-       The ``pt_weight`` parameter implementation has been corrected.
-       Previous versions resulted in :math:`p_T`-weighting when
-       ``False``, and :math:`p_T^2`-weighting when ``True``.
-
-    Parameters
-    ----------
-    pmu : MomentumArray
-        Four-momenta of the particles.
-    pt_weight : bool
-        If ``True``, will weight the contributions of each particle by
-        transverse momentum. Similar to finding a centre-of-mass, but
-        for transverse momentum. Default is ``True``.
-
-    Returns
-    -------
-    float
-        The centre of the particle set in the azimuth dimension.
-    """
-    pol = pmu._xy_pol
-    if not pt_weight:
-        pol = pol / pmu.pt
-    return np.angle(pol.sum()).item()
-
-
-@deprecated(
-    deprecated_in="0.3.1",
-    removed_in="0.4.0",
-    details="Use ``weighted_centroid()`` or ``resultant_coords()`` instead.",
-)
-def pseudorapidity_centre(pmu: "MomentumArray") -> float:
-    """Calculates the central point in pseudorapidity for a set of
-    particles.
-
-    :group: calculate
-
-    .. versionadded:: 0.1.7
-
-    Parameters
-    ----------
-    pmu : MomentumArray
-        Four-momenta of the particles.
-
-    Returns
-    -------
-    float
-        The :math:`p_T` weighted centre of the particle set in the
-        pseudorapidity dimension.
-    """
-    return ((pmu.eta * pmu.pt).sum() / pmu.pt.sum()).item()
-
-
-@deprecated(
-    deprecated_in="0.3.1",
-    removed_in="0.4.0",
-    details="Use ``weighted_centroid()`` or ``resultant_coords()`` instead.",
-)
-def rapidity_centre(pmu: "MomentumArray") -> float:
-    """Calculates the central point in rapidity for a set of particles.
-
-    :group: calculate
-
-    .. versionadded:: 0.2.11
-
-    Parameters
-    ----------
-    pmu : MomentumArray
-        Four-momenta of the particles.
-
-    Returns
-    -------
-    float
-        The :math:`p_T` weighted centre of the particle set in the
-        rapidity dimension.
-    """
-    return (pmu.rapidity * pmu.pt).sum() / pmu.pt.sum()
-
-
 def weighted_centroid(
     pmu: "MomentumArray", pseudo: bool = True
 ) -> ty.Tuple[float, float]:
     """Calculates the :math:`p_T`-weighted centroid for a set of
     particles in the (pseudo)rapidity-azimuth plane.
 
     :group: calculate
@@ -282,153 +185,14 @@
         try:
             mass = np.sqrt((data.sum(axis=0) ** 2) @ minkowski)
         except RuntimeWarning:
             mass = 0.0  # if sqrt(pmu^2) < 0, return mass as 0.0
     return mass
 
 
-def _diffuse(colors: ty.List[base.AnyVector], feats: ty.List[base.AnyVector]):
-    color_shape = colors[0].shape
-    av_color = np.zeros((color_shape[0], color_shape[1]), dtype="<f8")
-    color_stack = np.dstack(colors)  # len_basis x feat_dim x num_in
-    feat_stack = np.vstack(feats).T  # feat_dim x num_in
-    feat_sum = np.sum(feat_stack, axis=1)
-    nonzero_mask = feat_sum != 0.0
-    av_color[:, nonzero_mask] = (
-        np.sum(
-            color_stack[:, nonzero_mask, :] * feat_stack[nonzero_mask], axis=2
-        )
-        / feat_sum[nonzero_mask]
-    )
-    return av_color
-
-
-@lru_cache(maxsize=None)
-def _trace_vector(
-    nx_graph: nx.DiGraph,
-    vertex: int,
-    basis: ty.Tuple[int, ...],
-    feat_dim: int,
-    is_structured: bool,
-    exclusive: bool = False,
-) -> base.AnyVector:
-    len_basis = len(basis)
-    feat_fmt = rfn.structured_to_unstructured if is_structured else lambda x: x
-    color = np.zeros((len_basis, feat_dim), dtype="<f8")
-    if vertex in basis:
-        color[basis.index(vertex)] = 1.0
-        if exclusive is True:
-            return color
-    in_edges = nx_graph.in_edges(vertex, data=True)
-    colors_in: list[base.AnyVector] = []
-    feats = []
-    for edge in in_edges:
-        feats.append(feat_fmt(edge[2]["feat"]))
-        in_vtx = edge[0]
-        colors_in.append(
-            _trace_vector(
-                nx_graph, in_vtx, basis, feat_dim, is_structured, exclusive
-            )
-        )
-    if colors_in:
-        color += _diffuse(colors_in, feats)
-    return color
-
-
-def flow_trace(
-    graph: "Graphicle",
-    mask: ty.Union[base.MaskBase, base.BoolVector],
-    prop: ty.Union[base.ArrayBase, base.AnyVector],
-    exclusive: bool = False,
-    target: ty.Optional[ty.Set[int]] = None,
-) -> ty.Dict[str, base.DoubleVector]:
-    """Performs flow tracing from specified particles in an event, back
-    to the hard partons.
-
-    :group: calculate
-
-    .. versionadded:: 0.1.0
-
-    Parameters
-    ----------
-    graph : Graphicle
-        Full particle event, containing hard partons, showering and
-        hadronisation.
-    mask : MaskArray or MaskGroup or ndarray[bool_]
-        Boolean mask identifying which particles should have their
-        ancestry traced.
-    prop : ArrayBase or ndarray[any]
-        Property to trace back, *eg.* 4-momentum, charge, *etc*. Must be
-        the same shape as arrays stored in graph. Can be structured,
-        unstructured, or a graphicle array, though unstructured arrays
-        must be 1D.
-    exclusive : bool
-        If ``True``, double counting from descendant particles in the
-        hard event will be switched off. *eg.* for event ``t > b W+``,
-        descendants of ``b`` will show no contribution from ``t``, as
-        ``b`` is a subset of ``t``. Default is ``False``.
-    target : set[int], optional
-        Highlights specific partons in the hard event to decompose
-        properties with respect to. If unset, will use all partons in
-        hard event, except for incoming partons.
-
-    Returns
-    -------
-    trace_array : dict[str, ndarray]
-        Keys are parton names, arrays represent the contributions of
-        hard partons traced down to the properties of the selected
-        subset of particles specified by mask.
-    """
-    if isinstance(prop, base.ArrayBase):
-        prop = prop.data
-    # encoding graph features onto NetworkX
-    nx_graph = nx.DiGraph()
-    graph_dict = graph.adj.to_dicts(edge_data={"feat": prop})
-    example_feat = graph_dict["edges"][0][2]["feat"]
-    try:
-        feat_dim = len(example_feat)
-        dtype = example_feat.dtype
-    except TypeError:
-        feat_dim = 1
-        dtype = np.dtype(type(example_feat))
-    is_structured = dtype.names is not None
-    nx_graph.add_edges_from(graph_dict["edges"])
-    # identify the hard ancestors to which we trace
-    hard_mask = graph.hard_mask.copy()
-    del hard_mask["incoming"]
-    hard_graph = graph[hard_mask.bitwise_or()]
-    if target:  # restrict hard partons to user specified pdgs
-        target_mask = hard_graph.pdg.mask(
-            list(target), blacklist=False, sign_sensitive=True
-        )
-        hard_graph = hard_graph[target_mask]
-    names, vtxs = tuple(hard_graph.pdg.name), tuple(hard_graph.edges["dst"])
-    # out vertices of user specified particles
-    focus_pcls = graph.edges[mask]["dst"]
-    trc = np.array(
-        [
-            _trace_vector(
-                nx_graph, pcl, vtxs, feat_dim, is_structured, exclusive
-            )
-            for pcl in focus_pcls
-        ]
-    )
-    _trace_vector.cache_clear()
-    traces = dict()
-    array_fmt: ty.Callable[[base.AnyVector], base.AnyVector] = (
-        partial(rfn.unstructured_to_structured, dtype=dtype)  # type: ignore
-        if is_structured
-        else lambda x: x.squeeze()
-    )
-
-    for i, name in enumerate(names):
-        traces[name] = array_fmt(trc[:, i, :])
-    return traces
-
-
 @nb.njit("float64[:](float64[:], float64[:], float64)", cache=True)
 def _rapidity(
     energy: base.DoubleVector, z: base.DoubleVector, zero_tol: float
 ) -> base.DoubleVector:
     """Calculate the rapidity of a set of particles using energy
     and longitudinal components of their four-momenta.
 
@@ -759,19 +523,59 @@
     func_val = abs_dot_sum / norm_sum
     grad_vec = (
         np.array([grad_phi_sum, grad_theta_sum], dtype=np.float64) / norm_sum
     )
     return -func_val, -grad_vec
 
 
+@ty.overload
+def thrust(
+    pmu: "MomentumArray",
+    return_axis: ty.Literal[False],
+    rng_seed: ty.Optional[int],
+) -> float:
+    ...
+
+
+@ty.overload
+def thrust(pmu: "MomentumArray", return_axis: ty.Literal[False]) -> float:
+    ...
+
+
+@ty.overload
+def thrust(pmu: "MomentumArray", rng_seed: ty.Optional[int]) -> float:
+    ...
+
+
+@ty.overload
+def thrust(pmu: "MomentumArray") -> float:
+    ...
+
+
+@ty.overload
+def thrust(
+    pmu: "MomentumArray",
+    return_axis: ty.Literal[True],
+    rng_seed: ty.Optional[int],
+) -> ty.Tuple[float, base.DoubleVector]:
+    ...
+
+
+@ty.overload
+def thrust(
+    pmu: "MomentumArray",
+    return_axis: ty.Literal[True],
+) -> ty.Tuple[float, base.DoubleVector]:
+    ...
+
+
 def thrust(
     pmu: "MomentumArray",
     return_axis: bool = False,
     rng_seed: ty.Optional[int] = None,
-    frame: ty.Optional["MomentumArray"] = None,
 ):
     """Computes the thrust of an event, from the final-state momenta.
 
     :group: calculate
 
     .. versionadded:: 0.3.8
 
@@ -809,15 +613,15 @@
         fun=_thrust_with_grad,
         x0=guess,
         bounds=(domain, domain),
         method="L-BFGS-B",
         jac=True,
         args=(pmu.data,),
     )
-    thrust_val: float = -optim.fun
+    thrust_val = -optim.fun
     if return_axis:
         return thrust_val, _angles_to_axis(optim.x)
     return thrust_val
 
 
 @nb.njit(
     nb.types.Tuple((nb.float64, nb.float64[:]))(nb.float64[:], PMU_DTYPE),
@@ -892,14 +696,55 @@
     scale_factor = (4.0 / (math.pi * norm_sum)) ** 2
     spherocity = scale_factor * cross_norm_sum * cross_norm_sum
     grad_phi = scale_factor * cross_norm_sum * grad_phi_sum
     grad_theta = scale_factor * cross_norm_sum * grad_theta_sum
     return spherocity, np.array([grad_phi, grad_theta], dtype=np.float64)
 
 
+@ty.overload
+def spherocity(
+    pmu: "MomentumArray",
+    return_axis: ty.Literal[False],
+    rng_seed: ty.Optional[int],
+) -> float:
+    ...
+
+
+@ty.overload
+def spherocity(pmu: "MomentumArray", return_axis: ty.Literal[False]) -> float:
+    ...
+
+
+@ty.overload
+def spherocity(pmu: "MomentumArray", rng_seed: ty.Optional[int]) -> float:
+    ...
+
+
+@ty.overload
+def spherocity(pmu: "MomentumArray") -> float:
+    ...
+
+
+@ty.overload
+def spherocity(
+    pmu: "MomentumArray",
+    return_axis: ty.Literal[True],
+    rng_seed: ty.Optional[int],
+) -> ty.Tuple[float, base.DoubleVector]:
+    ...
+
+
+@ty.overload
+def spherocity(
+    pmu: "MomentumArray",
+    return_axis: ty.Literal[True],
+) -> ty.Tuple[float, base.DoubleVector]:
+    ...
+
+
 def spherocity(
     pmu: "MomentumArray",
     return_axis: bool = False,
     rng_seed: ty.Optional[int] = None,
 ):
     """Computes the spherocity of an event, from final-state momenta.
 
@@ -940,15 +785,15 @@
     optim = spo.minimize(
         fun=_spherocity_with_grad,
         x0=guess,
         bounds=(domain, domain),
         jac=True,
         args=(pmu.data,),
     )
-    sph_val: float = optim.fun
+    sph_val = optim.fun
     if return_axis:
         return sph_val, _angles_to_axis(optim.x)
     return sph_val
 
 
 @nb.njit(nb.float64(PMU_DTYPE), cache=True)
 def _c_parameter(momenta: base.VoidVector) -> float:
```

### Comparing `graphicle-0.3b1/graphicle/data.py` & `graphicle-0.4.0/graphicle/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1329,14 +1329,92 @@
     _HANDLED_TYPES: ty.Tuple[ty.Type, ...] = field(init=False, repr=False)
 
     def __attrs_post_init__(self):
         self._data = self._data.reshape(-1, 4)
         self.dtype = np.dtype(list(zip("xyze", it.repeat("<f8"))))
         self._HANDLED_TYPES = (np.ndarray, nm.Number, cla.Sequence)
 
+    @classmethod
+    def from_spherical_uniform(
+        cls,
+        size: int,
+        max_energy: float,
+        massless: float = 0.0,
+        seed: ty.Optional[int] = None,
+    ) -> "MomentumArray":
+        """Returns a ``MomentumArray`` whose elements are sampled from
+        uniform distributions of energy and 3-momentum.
+
+        .. versionadded:: 0.4.0
+
+        Parameters
+        ----------
+        size : int
+            Number of elements.
+        max_energy : float
+            Upper bound for the energy of the momenta.
+        massless : float
+            Probability for any given momentum element to be massless.
+            Default is ``0.0``.
+        seed : int, optional
+            Random number generator seed. Use the same seed for
+            consistent results.
+
+        Returns
+        -------
+        MomentumArray
+            Set of momenta, sampled uniformly in the energy component,
+            and with uniform probability density over the surface of a
+            3-sphere for the spatial components.
+
+        Raises
+        ------
+        ValueError
+            If massless is not within the interval [0.0, 1.0].
+
+        Notes
+        -----
+        Some 'massless' particles may have small, but finite masses.
+        This is due to numerical errors associated with floating point
+        calculations.
+        """
+        if not (0.0 <= massless <= 1.0):
+            raise ValueError(
+                "Probability of massless particles must be in the "
+                "interval [0, 1]."
+            )
+        rng = np.random.default_rng(seed=seed)
+        energy = rng.uniform(0.0, max_energy, size)
+        p_mag = energy
+        if massless == 0.0:
+            mass = rng.uniform(0.0, energy)
+            p_mag = calculate._root_diff_two_squares(energy, mass)
+        elif massless < 1.0:
+            p_mag = p_mag.copy()
+            mask = rng.random(size) < massless
+            masked_e = energy[~mask]
+            mass = rng.uniform(0.0, masked_e)
+            p_mag[~mask] = calculate._root_diff_two_squares(masked_e, mass)
+        theta_polar = p_mag * np.exp(
+            1.0j * np.arccos(1.0 - 2.0 * rng.random(size, dtype=np.float64))
+        )
+        phi_polar = theta_polar.real * np.exp(
+            1.0j * rng.uniform(-np.pi, np.pi, size)
+        )
+        return cls(
+            np.hstack(
+                [
+                    phi_polar.real.reshape(-1, 1),
+                    phi_polar.imag.reshape(-1, 1),
+                    theta_polar.imag.reshape(-1, 1),
+                    energy.reshape(-1, 1),
+                ]
+            )
+        )
+
     @property
     def __array_interface__(self) -> ty.Dict[str, ty.Any]:
         return self._data.__array_interface__
 
     def __array_ufunc__(self, ufunc, method, *inputs, **kwargs):
         return _array_ufunc(self, ufunc, method, *inputs, **kwargs)
 
@@ -2215,14 +2293,44 @@
         return self._table_str(html=False)
 
     def copy(self) -> "ParticleSet":
         """Copies the underlying data into a new ParticleSet instance."""
         return _composite_copy(self)
 
     @classmethod
+    def from_lhe_event(cls, event: base.LheEventInterface) -> "ParticleSet":
+        """Creates a ParticleSet instance directly from a data structure
+        holding LHE data. This is useful when you want to study the hard
+        process, without needing to shower or hadronize.
+
+        .. versionadded:: 0.4.0
+
+        Parameters
+        ----------
+        event : LheEventInterface
+            A data structure with attributes "pdg", "pmu", "color",
+            "helicity", and "status". These attributes provide access to
+            numpy arrays, which hold the underlying Les Houches event
+            data.
+
+        Returns
+        -------
+        ParticleSet
+            A composite object, wrapping the data provided in Graphicle
+            objects, and providing a unified interface to them.
+        """
+        props = ("pdg", "pmu", "color", "helicity", "status")
+        pcls = cls.from_numpy(**{name: getattr(event, name) for name in props})
+        pcls.final = MaskArray(np.zeros(len(pcls), dtype=np.bool_))
+        status_map = {-1: -21, 1: -23, -2: -22, 2: -22, 3: -22, -9: -12}
+        for old_code, new_code in status_map.items():
+            pcls.status.data[pcls.status.data == old_code] = new_code
+        return pcls
+
+    @classmethod
     def from_numpy(
         cls,
         pdg: ty.Optional[base.IntVector] = None,
         pmu: ty.Optional[base.VoidVector] = None,
         color: ty.Optional[base.VoidVector] = None,
         helicity: ty.Optional[base.HalfIntVector] = None,
         status: ty.Optional[base.HalfIntVector] = None,
```

### Comparing `graphicle-0.3b1/graphicle/matrix.py` & `graphicle-0.4.0/graphicle/matrix.py`

 * *Files identical despite different names*

### Comparing `graphicle-0.3b1/graphicle/select.py` & `graphicle-0.4.0/graphicle/select.py`

 * *Files 0% similar despite different names*

```diff
@@ -1135,15 +1135,15 @@
     descendants tree of the bottom quark, spread over a wide region of
     the :math:`\\eta-\\phi` plane. This is when the ``radius`` parameter
     is applied, excluding all final state descendants whose distance
     from the hard bottom quark exceeds the value passed, cleaning up the
     signal.
     """
     hier_ = hierarchy(graph)
-    hier = partition_descendants(graph, hier_, 0.0)
+    hier = partition_descendants(graph, hier_, -0.1)
     leaves = leaf_masks(hier)
     color_keys = color_singlets(leaves, graph.status, graph.color, True)
     colored_leaves = map(
         op.getitem, it.repeat(leaves), it.chain.from_iterable(color_keys)
     )
     colored_leaves, colored_leaves_ = it.tee(colored_leaves, 2)
     hard_mask = graph.hard_mask["outgoing"]
```

### Comparing `graphicle-0.3b1/graphicle.egg-info/PKG-INFO` & `graphicle-0.4.0/graphicle.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphicle
-Version: 0.3b1
+Version: 0.4.0
 Summary: Encode particle physics data onto graph structures.
 Author: Jacan Chaplais
 Maintainer: Jacan Chaplais
 License: BSD 3-Clause License
         
         Copyright (c) 2021, Jacan Chaplais.
         All rights reserved.
```

### Comparing `graphicle-0.3b1/graphicle.egg-info/SOURCES.txt` & `graphicle-0.4.0/graphicle.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -27,8 +27,9 @@
 graphicle/transform.py
 graphicle.egg-info/PKG-INFO
 graphicle.egg-info/SOURCES.txt
 graphicle.egg-info/dependency_links.txt
 graphicle.egg-info/requires.txt
 graphicle.egg-info/top_level.txt
 tests/test_calculate.py
-tests/test_data.py
+tests/test_data.py
+tests/test_transform.py
```

### Comparing `graphicle-0.3b1/pyproject.toml` & `graphicle-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `graphicle-0.3b1/tests/test_calculate.py` & `graphicle-0.4.0/tests/test_calculate.py`

 * *Files identical despite different names*

### Comparing `graphicle-0.3b1/tests/test_data.py` & `graphicle-0.4.0/tests/test_data.py`

 * *Files identical despite different names*

