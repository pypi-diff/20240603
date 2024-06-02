# Comparing `tmp/odeintw-1.0.0.tar.gz` & `tmp/odeintw-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odeintw-1.0.0.tar", last modified: Sun Sep  4 14:31:28 2022, max compression
+gzip compressed data, was "odeintw-1.0.2.tar", last modified: Sun Jun  2 22:51:38 2024, max compression
```

## Comparing `odeintw-1.0.0.tar` & `odeintw-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 warren    (1000) warren    (1000)        0 2022-09-04 14:31:28.424094 odeintw-1.0.0/
--rw-rw-r--   0 warren    (1000) warren    (1000)     1491 2022-09-03 17:35:07.000000 odeintw-1.0.0/LICENSE
--rw-rw-r--   0 warren    (1000) warren    (1000)     1022 2022-09-04 14:31:28.424094 odeintw-1.0.0/PKG-INFO
--rw-rw-r--   0 warren    (1000) warren    (1000)     4135 2022-09-03 17:35:07.000000 odeintw-1.0.0/README.md
-drwxrwxr-x   0 warren    (1000) warren    (1000)        0 2022-09-04 14:31:28.424094 odeintw-1.0.0/odeintw/
--rw-rw-r--   0 warren    (1000) warren    (1000)      166 2022-09-04 14:25:58.000000 odeintw-1.0.0/odeintw/__init__.py
--rw-rw-r--   0 warren    (1000) warren    (1000)    10354 2022-09-03 18:06:08.000000 odeintw-1.0.0/odeintw/_odeintw.py
-drwxrwxr-x   0 warren    (1000) warren    (1000)        0 2022-09-04 14:31:28.424094 odeintw-1.0.0/odeintw.egg-info/
--rw-rw-r--   0 warren    (1000) warren    (1000)     1022 2022-09-04 14:31:28.000000 odeintw-1.0.0/odeintw.egg-info/PKG-INFO
--rw-rw-r--   0 warren    (1000) warren    (1000)      220 2022-09-04 14:31:28.000000 odeintw-1.0.0/odeintw.egg-info/SOURCES.txt
--rw-rw-r--   0 warren    (1000) warren    (1000)        1 2022-09-04 14:31:28.000000 odeintw-1.0.0/odeintw.egg-info/dependency_links.txt
--rw-rw-r--   0 warren    (1000) warren    (1000)        6 2022-09-04 14:31:28.000000 odeintw-1.0.0/odeintw.egg-info/requires.txt
--rw-rw-r--   0 warren    (1000) warren    (1000)        8 2022-09-04 14:31:28.000000 odeintw-1.0.0/odeintw.egg-info/top_level.txt
--rw-rw-r--   0 warren    (1000) warren    (1000)       38 2022-09-04 14:31:28.424094 odeintw-1.0.0/setup.cfg
--rw-rw-r--   0 warren    (1000) warren    (1000)     1957 2022-09-03 17:35:07.000000 odeintw-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:51:38.153615 odeintw-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-06-02 22:51:33.000000 odeintw-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-06-02 22:51:38.153615 odeintw-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-06-02 22:51:33.000000 odeintw-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:51:38.149615 odeintw-1.0.2/odeintw/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-06-02 22:51:33.000000 odeintw-1.0.2/odeintw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-06-02 22:51:33.000000 odeintw-1.0.2/odeintw/_odeintw.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:51:38.153615 odeintw-1.0.2/odeintw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-06-02 22:51:38.000000 odeintw-1.0.2/odeintw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-06-02 22:51:38.000000 odeintw-1.0.2/odeintw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 22:51:38.000000 odeintw-1.0.2/odeintw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-02 22:51:38.000000 odeintw-1.0.2/odeintw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-02 22:51:38.000000 odeintw-1.0.2/odeintw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 22:51:38.153615 odeintw-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-06-02 22:51:33.000000 odeintw-1.0.2/setup.py
```

### Comparing `odeintw-1.0.0/LICENSE` & `odeintw-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `odeintw-1.0.0/PKG-INFO` & `odeintw-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: odeintw
-Version: 1.0.0
+Version: 1.0.2
 Summary: Solve complex and matrix differential equations with scipy.integrate.odeint.
 Home-page: https://github.com/WarrenWeckesser/odeintw
 Author: Warren Weckesser
 Keywords: scipy odeint
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
+Requires-Dist: scipy
 
 
 odeintw
 =======
 
 `odeintw` provides a wrapper of `scipy.integrate.odeint` that allows it to
 handle complex and matrix differential equations.  That is, it can solve
@@ -21,10 +22,10 @@
 
     dZ/dt = F(Z, t, param1, param2, ...)
 
 where `t` is real and `Z` is a real or complex array.
 
 Since `odeintw` is just a wrapper of `scipy.integrate.odeint`, it requires
 `scipy` to be installed.  SciPy 0.15 or greater is required, to avoid a
-bug in `scipy.stats.odeint` in older versions of SciPy.
+bug in `scipy.integrate.odeint` in older versions of SciPy.
 
 See README.md at https://github.com/WarrenWeckesser/odeintw for examples.
```

### Comparing `odeintw-1.0.0/README.md` & `odeintw-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     plt.xlabel('t')
     plt.grid(True)
     plt.legend(loc='best')
     plt.show()
 
 Plot:
 
-![](https://github.com/WarrenWeckesser/odeintw/blob/master/examples/odeintw_example1.png)
+![](https://github.com/WarrenWeckesser/odeintw/blob/main/examples/odeintw_example1.png)
 
 
 Example 2
 ---------
 
 We'll solve the matrix differential equation
 
@@ -141,14 +141,14 @@
     plt.plot(t, sol[:, 1, 1], '--', color=color2, linewidth=1.5, label='a[1,1]')
     plt.legend(loc='best')
     plt.grid(True)
     plt.show()
 
 Plot:
 
-![](https://github.com/WarrenWeckesser/odeintw/blob/master/examples/odeintw_example2.png)
+![](https://github.com/WarrenWeckesser/odeintw/blob/main/examples/odeintw_example2.png)
 
 
 *Copyright (c) 2015, Warren Weckesser*
 
 All rights reserved.
 See the LICENSE file for license information.
```

### Comparing `odeintw-1.0.0/odeintw/_odeintw.py` & `odeintw-1.0.2/odeintw/_odeintw.py`

 * *Files identical despite different names*

### Comparing `odeintw-1.0.0/odeintw.egg-info/PKG-INFO` & `odeintw-1.0.2/odeintw.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: odeintw
-Version: 1.0.0
+Version: 1.0.2
 Summary: Solve complex and matrix differential equations with scipy.integrate.odeint.
 Home-page: https://github.com/WarrenWeckesser/odeintw
 Author: Warren Weckesser
 Keywords: scipy odeint
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
+Requires-Dist: scipy
 
 
 odeintw
 =======
 
 `odeintw` provides a wrapper of `scipy.integrate.odeint` that allows it to
 handle complex and matrix differential equations.  That is, it can solve
@@ -21,10 +22,10 @@
 
     dZ/dt = F(Z, t, param1, param2, ...)
 
 where `t` is real and `Z` is a real or complex array.
 
 Since `odeintw` is just a wrapper of `scipy.integrate.odeint`, it requires
 `scipy` to be installed.  SciPy 0.15 or greater is required, to avoid a
-bug in `scipy.stats.odeint` in older versions of SciPy.
+bug in `scipy.integrate.odeint` in older versions of SciPy.
 
 See README.md at https://github.com/WarrenWeckesser/odeintw for examples.
```

### Comparing `odeintw-1.0.0/setup.py` & `odeintw-1.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 
-# Copyright (c) 2014, Warren Weckesser
+# Copyright (c) 2014, 2024 Warren Weckesser
 # All rights reserved.
 # See the LICENSE file for license information.
 
 from os import path
 from setuptools import setup
 
 
@@ -39,15 +39,15 @@
 
     dZ/dt = F(Z, t, param1, param2, ...)
 
 where `t` is real and `Z` is a real or complex array.
 
 Since `odeintw` is just a wrapper of `scipy.integrate.odeint`, it requires
 `scipy` to be installed.  SciPy 0.15 or greater is required, to avoid a
-bug in `scipy.stats.odeint` in older versions of SciPy.
+bug in `scipy.integrate.odeint` in older versions of SciPy.
 
 See README.md at https://github.com/WarrenWeckesser/odeintw for examples.
 """
 
 setup(name='odeintw',
       version=get_odeintw_version(),
       description=_descr,
```

