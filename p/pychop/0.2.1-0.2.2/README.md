# Comparing `tmp/pychop-0.2.1.tar.gz` & `tmp/pychop-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pychop-0.2.1.tar", last modified: Sat Jan 20 07:58:18 2024, max compression
+gzip compressed data, was "pychop-0.2.2.tar", last modified: Mon Jun  3 11:24:08 2024, max compression
```

## Comparing `pychop-0.2.1.tar` & `pychop-0.2.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)        0 2024-01-20 07:58:18.590692 pychop-0.2.1/
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)     1088 2024-01-20 07:57:34.000000 pychop-0.2.1/LICENSE
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)     4206 2024-01-20 07:58:18.560835 pychop-0.2.1/PKG-INFO
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)     3522 2024-01-20 07:57:34.000000 pychop-0.2.1/README.md
-drwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)        0 2024-01-20 07:58:17.286466 pychop-0.2.1/pychop/
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)       92 2024-01-20 07:57:34.000000 pychop-0.2.1/pychop/__init__.py
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)     1338 2024-01-20 07:57:34.000000 pychop-0.2.1/pychop/demo_harmonic.py
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)     2793 2024-01-20 07:57:34.000000 pychop-0.2.1/pychop/float_params.py
-drwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)        0 2024-01-20 07:58:17.993866 pychop-0.2.1/pychop/numpy/
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)       46 2024-01-20 07:57:34.000000 pychop-0.2.1/pychop/numpy/__init__.py
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)    18683 2024-01-20 07:57:34.000000 pychop-0.2.1/pychop/numpy/chop.py
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)     1214 2024-01-20 07:57:34.000000 pychop-0.2.1/pychop/numpy/quant.py
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)     7074 2024-01-20 07:57:34.000000 pychop-0.2.1/pychop/numpy/roundit.py
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)     6751 2024-01-20 07:57:34.000000 pychop-0.2.1/pychop/simulate.py
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)        0 2024-01-20 07:57:34.000000 pychop-0.2.1/pychop/test_chop.py
-drwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)        0 2024-01-20 07:58:18.457640 pychop-0.2.1/pychop/torch/
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)       46 2024-01-20 07:57:34.000000 pychop-0.2.1/pychop/torch/__init__.py
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)    18419 2024-01-20 07:57:34.000000 pychop-0.2.1/pychop/torch/chop.py
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)      618 2024-01-20 07:57:34.000000 pychop-0.2.1/pychop/torch/layers.py
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)      349 2024-01-20 07:57:34.000000 pychop-0.2.1/pychop/torch/quant.py
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)     4664 2024-01-20 07:57:34.000000 pychop-0.2.1/pychop/torch/roundit.py
-drwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)        0 2024-01-20 07:58:17.607708 pychop-0.2.1/pychop.egg-info/
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)     4206 2024-01-20 07:58:16.000000 pychop-0.2.1/pychop.egg-info/PKG-INFO
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)      487 2024-01-20 07:58:16.000000 pychop-0.2.1/pychop.egg-info/SOURCES.txt
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)        1 2024-01-20 07:58:16.000000 pychop-0.2.1/pychop.egg-info/dependency_links.txt
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)       13 2024-01-20 07:58:16.000000 pychop-0.2.1/pychop.egg-info/requires.txt
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)        7 2024-01-20 07:58:16.000000 pychop-0.2.1/pychop.egg-info/top_level.txt
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)       38 2024-01-20 07:58:18.594712 pychop-0.2.1/setup.cfg
--rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)     3185 2024-01-20 07:57:34.000000 pychop-0.2.1/setup.py
+drwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)        0 2024-06-03 11:24:08.859320 pychop-0.2.2/
+-rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)     1088 2024-06-03 11:22:53.000000 pychop-0.2.2/LICENSE
+-rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)     4602 2024-06-03 11:24:08.855538 pychop-0.2.2/PKG-INFO
+-rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)     3925 2024-06-03 11:22:53.000000 pychop-0.2.2/README.md
+drwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)        0 2024-06-03 11:24:08.627318 pychop-0.2.2/pychop/
+-rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)       92 2024-06-03 11:22:53.000000 pychop-0.2.2/pychop/__init__.py
+-rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)     1338 2024-06-03 11:22:53.000000 pychop-0.2.2/pychop/demo_harmonic.py
+-rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)     2793 2024-06-03 11:22:53.000000 pychop-0.2.2/pychop/float_params.py
+drwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)        0 2024-06-03 11:24:08.751887 pychop-0.2.2/pychop/numpy/
+-rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)       46 2024-06-03 11:22:53.000000 pychop-0.2.2/pychop/numpy/__init__.py
+-rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)    18633 2024-06-03 11:22:53.000000 pychop-0.2.2/pychop/numpy/chop.py
+-rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)     4145 2024-06-03 11:22:53.000000 pychop-0.2.2/pychop/numpy/quant.py
+-rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)     7074 2024-06-03 11:22:53.000000 pychop-0.2.2/pychop/numpy/roundit.py
+-rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)     6751 2024-06-03 11:22:53.000000 pychop-0.2.2/pychop/simulate.py
+-rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)        0 2024-06-03 11:22:53.000000 pychop-0.2.2/pychop/test_chop.py
+drwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)        0 2024-06-03 11:24:08.839391 pychop-0.2.2/pychop/torch/
+-rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)       46 2024-06-03 11:22:53.000000 pychop-0.2.2/pychop/torch/__init__.py
+-rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)    18419 2024-06-03 11:22:53.000000 pychop-0.2.2/pychop/torch/chop.py
+-rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)      618 2024-06-03 11:22:53.000000 pychop-0.2.2/pychop/torch/layers.py
+-rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)      349 2024-06-03 11:22:53.000000 pychop-0.2.2/pychop/torch/quant.py
+-rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)     4664 2024-06-03 11:22:53.000000 pychop-0.2.2/pychop/torch/roundit.py
+drwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)        0 2024-06-03 11:24:08.684511 pychop-0.2.2/pychop.egg-info/
+-rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)     4602 2024-06-03 11:24:08.000000 pychop-0.2.2/pychop.egg-info/PKG-INFO
+-rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)      487 2024-06-03 11:24:08.000000 pychop-0.2.2/pychop.egg-info/SOURCES.txt
+-rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)        1 2024-06-03 11:24:08.000000 pychop-0.2.2/pychop.egg-info/dependency_links.txt
+-rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)       13 2024-06-03 11:24:08.000000 pychop-0.2.2/pychop.egg-info/requires.txt
+-rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)        7 2024-06-03 11:24:08.000000 pychop-0.2.2/pychop.egg-info/top_level.txt
+-rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)       38 2024-06-03 11:24:08.860065 pychop-0.2.2/setup.cfg
+-rwxrwxrwx   0 chenxinye  (1000) chenxinye  (1000)     3185 2024-06-03 11:22:53.000000 pychop-0.2.2/setup.py
```

### Comparing `pychop-0.2.1/LICENSE` & `pychop-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pychop-0.2.1/PKG-INFO` & `pychop-0.2.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychop
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python code for simulating low precision floating-point arithmetic
 Home-page: https://github.com/chenxinye/pychop.git
 Author: Xinye Chen
 Author-email: xinyechenai@gmail.com
 Maintainer: Xinye Chen
 Maintainer-email: xinyechenai@gmail.com
 License: MIT License
@@ -83,14 +83,21 @@
 
 `pip install pychop`
 
 
 ### Contributing
 We welcome contributions in any form! Assistance with documentation is always welcome. To contribute, feel free to open an issue or please fork the project make your changes and submit a pull request. We will do our best to work through any issues and requests.
 
+
+### Acknowledgement
+This project is supported by the European Union (ERC, [InEXASCALE](https://www.karlin.mff.cuni.cz/~carson/inexascale), 101075632). Views and opinions
+ expressed are those of the authors only and do not necessarily reflect those of the European
+ Union or the European Research Council. Neither the European Union nor the granting
+ authority can be held responsible for them.
+
 ### References
 
 [1] Nicholas J. Higham and Srikara Pranesh, Simulating Low Precision Floating-Point Arithmetic, SIAM J. Sci. Comput., 2019.
 
 [2] IEEE Standard for Floating-Point Arithmetic, IEEE Std 754-2019 (revision of IEEE Std 754-2008), IEEE, 2019.
 
 [3] Intel Corporation, BFLOAT16---hardware numerics definition,  2018
```

### Comparing `pychop-0.2.1/README.md` & `pychop-0.2.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -61,14 +61,21 @@
 
 `pip install pychop`
 
 
 ### Contributing
 We welcome contributions in any form! Assistance with documentation is always welcome. To contribute, feel free to open an issue or please fork the project make your changes and submit a pull request. We will do our best to work through any issues and requests.
 
+
+### Acknowledgement
+This project is supported by the European Union (ERC, [InEXASCALE](https://www.karlin.mff.cuni.cz/~carson/inexascale), 101075632). Views and opinions
+ expressed are those of the authors only and do not necessarily reflect those of the European
+ Union or the European Research Council. Neither the European Union nor the granting
+ authority can be held responsible for them.
+
 ### References
 
 [1] Nicholas J. Higham and Srikara Pranesh, Simulating Low Precision Floating-Point Arithmetic, SIAM J. Sci. Comput., 2019.
 
 [2] IEEE Standard for Floating-Point Arithmetic, IEEE Std 754-2019 (revision of IEEE Std 754-2008), IEEE, 2019.
 
 [3] Intel Corporation, BFLOAT16---hardware numerics definition,  2018
```

### Comparing `pychop-0.2.1/pychop/demo_harmonic.py` & `pychop-0.2.2/pychop/demo_harmonic.py`

 * *Files identical despite different names*

### Comparing `pychop-0.2.1/pychop/float_params.py` & `pychop-0.2.2/pychop/float_params.py`

 * *Files identical despite different names*

### Comparing `pychop-0.2.1/pychop/numpy/chop.py` & `pychop-0.2.2/pychop/numpy/chop.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     Methods
     ----------
     chop(x):
         Method that convert ``x`` to the user-specific arithmetic format.
         
     """
 
-    def __init__(self, prec='s', subnormal=None, rmode=1, flip=False, explim=1, inplace=False,
+    def __init__(self, prec='h', subnormal=None, rmode=1, flip=False, explim=1,
                  p=0.5, randfunc=None, customs=None, random_state=0):
         
         np.random.seed(random_state)
         
         self.prec = prec
         
         if subnormal is not None:
@@ -103,16 +103,14 @@
             
         self.rmode = rmode
         self.flip = flip
         self.explim = explim
         self.p = p
         
         self.randfunc = randfunc
-        self.inplace = inplace
-        
         if self.rmode == 1:
             self._chop = _chop_round_to_nearest
             
         elif self.rmode == 2:
             self._chop = _chop_round_towards_plus_inf
             
         elif self.rmode == 3:
@@ -172,15 +170,15 @@
                 self.maxfraction = (x.dtype == 'float32')  * 11 + (x.dtype == 'float64')  * 25
             else:
                 self.maxfraction = (x.dtype == 'float32')  * 23 + (x.dtype == 'float64') * 52
                 
             if self.t > self.maxfraction:
                 raise ValueError('Precision of the custom format must be at most')
                 
-        y = self.chop_wrapper(x)
+        y = self.chop_wrapper(x.copy())
         return y
         
 
     
     def chop_wrapper(self, x):
         return self._chop(x, t=self.t, emax=self.emax, subnormal=self.subnormal, flip=self.flip, 
                                 explim=self.explim, p=self.p)
```

### Comparing `pychop-0.2.1/pychop/numpy/roundit.py` & `pychop-0.2.2/pychop/numpy/roundit.py`

 * *Files identical despite different names*

### Comparing `pychop-0.2.1/pychop/simulate.py` & `pychop-0.2.2/pychop/simulate.py`

 * *Files identical despite different names*

### Comparing `pychop-0.2.1/pychop/torch/chop.py` & `pychop-0.2.2/pychop/torch/chop.py`

 * *Files identical despite different names*

### Comparing `pychop-0.2.1/pychop/torch/layers.py` & `pychop-0.2.2/pychop/torch/layers.py`

 * *Files identical despite different names*

### Comparing `pychop-0.2.1/pychop/torch/roundit.py` & `pychop-0.2.2/pychop/torch/roundit.py`

 * *Files identical despite different names*

### Comparing `pychop-0.2.1/pychop.egg-info/PKG-INFO` & `pychop-0.2.2/pychop.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychop
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python code for simulating low precision floating-point arithmetic
 Home-page: https://github.com/chenxinye/pychop.git
 Author: Xinye Chen
 Author-email: xinyechenai@gmail.com
 Maintainer: Xinye Chen
 Maintainer-email: xinyechenai@gmail.com
 License: MIT License
@@ -83,14 +83,21 @@
 
 `pip install pychop`
 
 
 ### Contributing
 We welcome contributions in any form! Assistance with documentation is always welcome. To contribute, feel free to open an issue or please fork the project make your changes and submit a pull request. We will do our best to work through any issues and requests.
 
+
+### Acknowledgement
+This project is supported by the European Union (ERC, [InEXASCALE](https://www.karlin.mff.cuni.cz/~carson/inexascale), 101075632). Views and opinions
+ expressed are those of the authors only and do not necessarily reflect those of the European
+ Union or the European Research Council. Neither the European Union nor the granting
+ authority can be held responsible for them.
+
 ### References
 
 [1] Nicholas J. Higham and Srikara Pranesh, Simulating Low Precision Floating-Point Arithmetic, SIAM J. Sci. Comput., 2019.
 
 [2] IEEE Standard for Floating-Point Arithmetic, IEEE Std 754-2019 (revision of IEEE Std 754-2008), IEEE, 2019.
 
 [3] Intel Corporation, BFLOAT16---hardware numerics definition,  2018
```

### Comparing `pychop-0.2.1/setup.py` & `pychop-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import numpy
 import platform
 import importlib
 import logging
 
 PRJECT_NAME = "pychop"
 PACKAGE_NAME = "pychop"
-VERSION = "0.2.1"
+VERSION = "0.2.2"
 SETREQUIRES=["numpy", "torch"]
 MAINTAINER="Xinye Chen"
 EMAIL="xinyechenai@gmail.com"
 INREUIRES=["numpy>=1.7.2"]
 
 
 AUTHORS="Xinye Chen"
```

