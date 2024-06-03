# Comparing `tmp/consensusgen-2.0.tar.gz` & `tmp/consensusgen-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "consensusgen-2.0.tar", last modified: Mon Jun  3 12:34:40 2024, max compression
+gzip compressed data, was "consensusgen-2.1.tar", last modified: Mon Jun  3 13:02:52 2024, max compression
```

## Comparing `consensusgen-2.0.tar` & `consensusgen-2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:40.630123 consensusgen-2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-06-03 12:34:32.000000 consensusgen-2.0/LICENCE.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:32.000000 consensusgen-2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-06-03 12:34:40.630123 consensusgen-2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-06-03 12:34:32.000000 consensusgen-2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:40.626123 consensusgen-2.0/consensusGen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-06-03 12:34:40.000000 consensusgen-2.0/consensusGen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-06-03 12:34:40.000000 consensusgen-2.0/consensusGen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 12:34:40.000000 consensusgen-2.0/consensusGen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-06-03 12:34:40.000000 consensusgen-2.0/consensusGen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-06-03 12:34:40.000000 consensusgen-2.0/consensusGen.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:40.626123 consensusgen-2.0/consensusgen/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 12:34:32.000000 consensusgen-2.0/consensusgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11044 2024-06-03 12:34:32.000000 consensusgen-2.0/consensusgen/consensusGen.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 12:34:40.630123 consensusgen-2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-06-03 12:34:32.000000 consensusgen-2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:02:52.052130 consensusgen-2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-06-03 13:02:30.000000 consensusgen-2.1/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:02:30.000000 consensusgen-2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-06-03 13:02:52.048130 consensusgen-2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-06-03 13:02:30.000000 consensusgen-2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:02:52.048130 consensusgen-2.1/consensusGen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-06-03 13:02:52.000000 consensusgen-2.1/consensusGen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-06-03 13:02:52.000000 consensusgen-2.1/consensusGen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 13:02:52.000000 consensusgen-2.1/consensusGen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-03 13:02:52.000000 consensusgen-2.1/consensusGen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-06-03 13:02:52.000000 consensusgen-2.1/consensusGen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:02:52.048130 consensusgen-2.1/consensusgen/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 13:02:30.000000 consensusgen-2.1/consensusgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-06-03 13:02:30.000000 consensusgen-2.1/consensusgen/consensusGen.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 13:02:52.052130 consensusgen-2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-06-03 13:02:30.000000 consensusgen-2.1/setup.py
```

### Comparing `consensusgen-2.0/LICENCE.md` & `consensusgen-2.1/LICENCE.md`

 * *Files identical despite different names*

### Comparing `consensusgen-2.0/PKG-INFO` & `consensusgen-2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consensusGen
-Version: 2.0
+Version: 2.1
 Summary: Genetic algorithm for consensus building
 Home-page: https://pypi.org/project/consensusGen/
 Author: RomainCoulon (Romain Coulon)
 Author-email: <romain.coulon@bipm.org>
 Project-URL: Documentation, https://github.com/RomainCoulon/consensusGen/
 Keywords: genetic algorithm,inter-laboratory comparison,consenus building
 Classifier: Development Status :: 4 - Beta
@@ -17,15 +17,14 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Scientific/Engineering :: Physics
 Description-Content-Type: text/markdown
 License-File: LICENCE.md
 Requires-Dist: numpy
 Requires-Dist: matplotlib
-Requires-Dist: collections
 Requires-Dist: math
 
 # consensusGen
 
 `consensusGen.py` is a Python code implementing an genetic algorithm allowing to build a consensus value from measurement results of an inter-laboratory comparison. 
 
 Details are provided in [Romain Coulon and Steven Judge 2021 Metrologia 58 065007](https://doi.org/10.1088/1681-7575/ac31c0)
```

### Comparing `consensusgen-2.0/consensusGen.egg-info/PKG-INFO` & `consensusgen-2.1/consensusGen.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consensusGen
-Version: 2.0
+Version: 2.1
 Summary: Genetic algorithm for consensus building
 Home-page: https://pypi.org/project/consensusGen/
 Author: RomainCoulon (Romain Coulon)
 Author-email: <romain.coulon@bipm.org>
 Project-URL: Documentation, https://github.com/RomainCoulon/consensusGen/
 Keywords: genetic algorithm,inter-laboratory comparison,consenus building
 Classifier: Development Status :: 4 - Beta
@@ -17,15 +17,14 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Scientific/Engineering :: Physics
 Description-Content-Type: text/markdown
 License-File: LICENCE.md
 Requires-Dist: numpy
 Requires-Dist: matplotlib
-Requires-Dist: collections
 Requires-Dist: math
 
 # consensusGen
 
 `consensusGen.py` is a Python code implementing an genetic algorithm allowing to build a consensus value from measurement results of an inter-laboratory comparison. 
 
 Details are provided in [Romain Coulon and Steven Judge 2021 Metrologia 58 065007](https://doi.org/10.1088/1681-7575/ac31c0)
```

### Comparing `consensusgen-2.0/consensusgen/consensusGen.py` & `consensusgen-2.1/consensusgen/consensusGen.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     
     if not magnitude1 or not magnitude2:
         return 0.0
     
     # Calculate cosine similarity
     return dot_product / (magnitude1 * magnitude2)
 
-def DoE(x,u,x_ref,ux_ref,*,w=[],k=2):
+def DoE(x,u,x_ref,ux_ref,*,w=[],uw=[],k=2):
     """This function aims to calculate Degrees of equivalence.
     
     References: 
         [Accred Qual Assur (2008)13:83-89, Metrologia 52(2015)S200]
         https://link.springer.com/article/10.1007/s00769-007-0330-1
         https://iopscience.iop.org/article/10.1088/0026-1394/52/3/S200/pdf
     
@@ -50,14 +50,16 @@
     :param x_ref: Estimation of the reference value
     :type x_ref: float
     :param ux_ref: Estimation of uncertainty of the reference value
     :type ux_ref: float
     
     :param w: (Optional) Weights associated to each data point.
     :type w: array of floats
+    :param uw: (Optional) Standard uncertainty associated to weights of each data point.
+    :type uw: array of floats
     :param k: (Optional) Coverage factor (set by default equal to 2)
     :type k: float    
     
     :param d: Estimation of the degrees of equivalence
     :type d: array of floats
     :param ud: Estimation of the uncertainties related to the degrees of equivalence
     :type ud: array of floats    
@@ -66,20 +68,23 @@
     :param udr: Estimation of the uncertainties related to the relative degrees of equivalence
     :type udr: array of floats  
     
     :return y: d, ud, dr, udr
     :rtype y: tuple
     """
     
-    x=np.asarray(x) # format input data
-    u=np.asarray(u) # format input data
-    w=np.asarray(w) # format input data
-    k=2
-    d=x-x_ref  # euclidian distance from the reference value
-    u2d=(1-2*w)*u**2+ux_ref**2 # variance associated with DE (the weight factor is available)
+    x = np.asarray(x) # format input data
+    u = np.asarray(u) # format input data
+    w = np.asarray(w) # format input data
+    uw = np.asarray(uw) # format input data
+    d = x - x_ref  # euclidian distance from the reference value
+    cov = np.empty(len(x))
+    for i in range(len(x)):
+        cov[i]=sum(x**2*uw[i]**2)
+    u2d=(1 - 2*w)*u**2 + ux_ref**2 + cov # variance associated with DE (the weight factor is available)
     ud=k*u2d**0.5     # enlarged standard deviation associated with DoE
     dr=d/x_ref        # relative DoE
     udr=ud/x_ref      # relative u(DoE)
     return d, ud, dr, udr
 
 def displayResult(X, u, result, *, lab=False):
     """
@@ -99,15 +104,15 @@
     Returns
     -------
     None.
     """
     mu_vec, u_mu_vec, g0pop, gLpop, w, u_w = result
     mu=mu_vec[-1]; u_mu=u_mu_vec[-1]
     nX = len(X)
-    d, ud, dr, udr = DoE(X,u,mu,u_mu,w=w)
+    d, ud, dr, udr = DoE(X,u,mu,u_mu,w=w,uw=u_w)
     MAD=np.median(abs(d)) # median of absolute value of degrees of equivalence
     x=d/MAD            # x-coordinates
     y=ud/MAD           # y-coordinates
     
     
     if not lab:
         lab = np.linspace(1, nX, nX)-1
```

### Comparing `consensusgen-2.0/setup.py` & `consensusgen-2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = "2.0"
+VERSION = "2.1"
 
 
 DESCRIPTION = "Genetic algorithm for consensus building"
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
@@ -19,15 +19,15 @@
     description = DESCRIPTION,
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://pypi.org/project/consensusGen/",
     py_modules=['consensusGen'], 
     project_urls={'Documentation': 'https://github.com/RomainCoulon/consensusGen/',},
     packages = find_packages(),
-    install_requires = ["numpy","matplotlib","collections","math"],
+    install_requires = ["numpy","matplotlib","math"],
     keywords = ["genetic algorithm","inter-laboratory comparison","consenus building"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Natural Language :: French",
```

