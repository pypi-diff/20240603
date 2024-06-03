# Comparing `tmp/ultralytics_thop-0.2.6.tar.gz` & `tmp/ultralytics_thop-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultralytics_thop-0.2.6.tar", last modified: Sat Jun  1 16:09:46 2024, max compression
+gzip compressed data, was "ultralytics_thop-0.2.7.tar", last modified: Mon Jun  3 01:35:56 2024, max compression
```

## Comparing `ultralytics_thop-0.2.6.tar` & `ultralytics_thop-0.2.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:09:46.455511 ultralytics_thop-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-06-01 16:08:43.000000 ultralytics_thop-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8511 2024-06-01 16:09:46.455511 ultralytics_thop-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7092 2024-06-01 16:08:43.000000 ultralytics_thop-0.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-06-01 16:08:43.000000 ultralytics_thop-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 16:09:46.455511 ultralytics_thop-0.2.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:09:46.451511 ultralytics_thop-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-06-01 16:08:43.000000 ultralytics_thop-0.2.6/tests/test_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-06-01 16:08:43.000000 ultralytics_thop-0.2.6/tests/test_matmul.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-06-01 16:08:43.000000 ultralytics_thop-0.2.6/tests/test_relu.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-06-01 16:08:43.000000 ultralytics_thop-0.2.6/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:09:46.451511 ultralytics_thop-0.2.6/thop/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-06-01 16:08:43.000000 ultralytics_thop-0.2.6/thop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8270 2024-06-01 16:08:43.000000 ultralytics_thop-0.2.6/thop/fx_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     7848 2024-06-01 16:08:43.000000 ultralytics_thop-0.2.6/thop/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6485 2024-06-01 16:08:43.000000 ultralytics_thop-0.2.6/thop/rnn_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-06-01 16:08:43.000000 ultralytics_thop-0.2.6/thop/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:09:46.455511 ultralytics_thop-0.2.6/thop/vision/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 16:08:43.000000 ultralytics_thop-0.2.6/thop/vision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-06-01 16:08:43.000000 ultralytics_thop-0.2.6/thop/vision/basic_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-06-01 16:08:43.000000 ultralytics_thop-0.2.6/thop/vision/calc_func.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:09:46.455511 ultralytics_thop-0.2.6/ultralytics_thop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8511 2024-06-01 16:09:46.000000 ultralytics_thop-0.2.6/ultralytics_thop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-06-01 16:09:46.000000 ultralytics_thop-0.2.6/ultralytics_thop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 16:09:46.000000 ultralytics_thop-0.2.6/ultralytics_thop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-06-01 16:09:46.000000 ultralytics_thop-0.2.6/ultralytics_thop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-06-01 16:09:46.000000 ultralytics_thop-0.2.6/ultralytics_thop.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:35:56.397052 ultralytics_thop-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-06-03 01:34:58.000000 ultralytics_thop-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8523 2024-06-03 01:35:56.397052 ultralytics_thop-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-06-03 01:34:58.000000 ultralytics_thop-0.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-06-03 01:34:58.000000 ultralytics_thop-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 01:35:56.397052 ultralytics_thop-0.2.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:35:56.393052 ultralytics_thop-0.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-06-03 01:34:58.000000 ultralytics_thop-0.2.7/tests/test_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-06-03 01:34:58.000000 ultralytics_thop-0.2.7/tests/test_matmul.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-06-03 01:34:58.000000 ultralytics_thop-0.2.7/tests/test_relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-06-03 01:34:58.000000 ultralytics_thop-0.2.7/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:35:56.393052 ultralytics_thop-0.2.7/thop/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-06-03 01:34:58.000000 ultralytics_thop-0.2.7/thop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8270 2024-06-03 01:34:58.000000 ultralytics_thop-0.2.7/thop/fx_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7848 2024-06-03 01:34:58.000000 ultralytics_thop-0.2.7/thop/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6485 2024-06-03 01:34:58.000000 ultralytics_thop-0.2.7/thop/rnn_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-06-03 01:34:58.000000 ultralytics_thop-0.2.7/thop/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:35:56.397052 ultralytics_thop-0.2.7/thop/vision/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 01:34:58.000000 ultralytics_thop-0.2.7/thop/vision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-06-03 01:34:58.000000 ultralytics_thop-0.2.7/thop/vision/basic_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-06-03 01:34:58.000000 ultralytics_thop-0.2.7/thop/vision/calc_func.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:35:56.397052 ultralytics_thop-0.2.7/ultralytics_thop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8523 2024-06-03 01:35:56.000000 ultralytics_thop-0.2.7/ultralytics_thop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-06-03 01:35:56.000000 ultralytics_thop-0.2.7/ultralytics_thop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 01:35:56.000000 ultralytics_thop-0.2.7/ultralytics_thop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-06-03 01:35:56.000000 ultralytics_thop-0.2.7/ultralytics_thop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-06-03 01:35:56.000000 ultralytics_thop-0.2.7/ultralytics_thop.egg-info/top_level.txt
```

### Comparing `ultralytics_thop-0.2.6/LICENSE` & `ultralytics_thop-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ultralytics_thop-0.2.6/PKG-INFO` & `ultralytics_thop-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultralytics-thop
-Version: 0.2.6
+Version: 0.2.7
 Summary: Ultralytics THOP package for fast computation of PyTorch model FLOPs and parameters.
 Author-email: Ligeng Zhu <ligeng.zhu+github@gmail.com>
 Maintainer: Glenn Jocher
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/thop/issues
 Project-URL: Funding, https://ultralytics.com
 Project-URL: Source, https://github.com/ultralytics/thop/
@@ -45,15 +45,15 @@
 
 THOP offers an intuitive API to profile PyTorch models by calculating the number of MACs and parameters. This functionality is crucial for assessing the computational efficiency and memory footprint of deep learning models.
 
 ## 📦 Installation
 
 You can install THOP via pip:
 
-[![PyPI - Version](https://img.shields.io/pypi/v/ultralytics-thop?logo=pypi&logoColor=white)](https://pypi.org/project/ultralytics-thop/) [![Downloads](https://static.pepy.tech/badge/ultralytics-thop)](https://pepy.tech/project/thop) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ultralytics-thop?logo=python&logoColor=gold)](https://pypi.org/project/ultralytics-thop/)
+[![PyPI - Version](https://img.shields.io/pypi/v/ultralytics-thop?logo=pypi&logoColor=white)](https://pypi.org/project/ultralytics-thop/) [![Downloads](https://static.pepy.tech/badge/ultralytics-thop)](https://pepy.tech/project/ultralytics-thop) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ultralytics-thop?logo=python&logoColor=gold)](https://pypi.org/project/ultralytics-thop/)
 
 ```bash
 pip install ultralytics-thop
 ```
 
 Alternatively, install the latest version directly from GitHub:
```

### Comparing `ultralytics_thop-0.2.6/README.md` & `ultralytics_thop-0.2.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 THOP offers an intuitive API to profile PyTorch models by calculating the number of MACs and parameters. This functionality is crucial for assessing the computational efficiency and memory footprint of deep learning models.
 
 ## 📦 Installation
 
 You can install THOP via pip:
 
-[![PyPI - Version](https://img.shields.io/pypi/v/ultralytics-thop?logo=pypi&logoColor=white)](https://pypi.org/project/ultralytics-thop/) [![Downloads](https://static.pepy.tech/badge/ultralytics-thop)](https://pepy.tech/project/thop) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ultralytics-thop?logo=python&logoColor=gold)](https://pypi.org/project/ultralytics-thop/)
+[![PyPI - Version](https://img.shields.io/pypi/v/ultralytics-thop?logo=pypi&logoColor=white)](https://pypi.org/project/ultralytics-thop/) [![Downloads](https://static.pepy.tech/badge/ultralytics-thop)](https://pepy.tech/project/ultralytics-thop) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ultralytics-thop?logo=python&logoColor=gold)](https://pypi.org/project/ultralytics-thop/)
 
 ```bash
 pip install ultralytics-thop
 ```
 
 Alternatively, install the latest version directly from GitHub:
```

### Comparing `ultralytics_thop-0.2.6/pyproject.toml` & `ultralytics_thop-0.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ultralytics_thop-0.2.6/tests/test_conv2d.py` & `ultralytics_thop-0.2.7/tests/test_conv2d.py`

 * *Files identical despite different names*

### Comparing `ultralytics_thop-0.2.6/tests/test_matmul.py` & `ultralytics_thop-0.2.7/tests/test_matmul.py`

 * *Files identical despite different names*

### Comparing `ultralytics_thop-0.2.6/tests/test_utils.py` & `ultralytics_thop-0.2.7/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics_thop-0.2.6/thop/fx_profile.py` & `ultralytics_thop-0.2.7/thop/fx_profile.py`

 * *Files identical despite different names*

### Comparing `ultralytics_thop-0.2.6/thop/profile.py` & `ultralytics_thop-0.2.7/thop/profile.py`

 * *Files identical despite different names*

### Comparing `ultralytics_thop-0.2.6/thop/rnn_hooks.py` & `ultralytics_thop-0.2.7/thop/rnn_hooks.py`

 * *Files identical despite different names*

### Comparing `ultralytics_thop-0.2.6/thop/utils.py` & `ultralytics_thop-0.2.7/thop/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics_thop-0.2.6/thop/vision/basic_hooks.py` & `ultralytics_thop-0.2.7/thop/vision/basic_hooks.py`

 * *Files identical despite different names*

### Comparing `ultralytics_thop-0.2.6/thop/vision/calc_func.py` & `ultralytics_thop-0.2.7/thop/vision/calc_func.py`

 * *Files identical despite different names*

### Comparing `ultralytics_thop-0.2.6/ultralytics_thop.egg-info/PKG-INFO` & `ultralytics_thop-0.2.7/ultralytics_thop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultralytics-thop
-Version: 0.2.6
+Version: 0.2.7
 Summary: Ultralytics THOP package for fast computation of PyTorch model FLOPs and parameters.
 Author-email: Ligeng Zhu <ligeng.zhu+github@gmail.com>
 Maintainer: Glenn Jocher
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/thop/issues
 Project-URL: Funding, https://ultralytics.com
 Project-URL: Source, https://github.com/ultralytics/thop/
@@ -45,15 +45,15 @@
 
 THOP offers an intuitive API to profile PyTorch models by calculating the number of MACs and parameters. This functionality is crucial for assessing the computational efficiency and memory footprint of deep learning models.
 
 ## 📦 Installation
 
 You can install THOP via pip:
 
-[![PyPI - Version](https://img.shields.io/pypi/v/ultralytics-thop?logo=pypi&logoColor=white)](https://pypi.org/project/ultralytics-thop/) [![Downloads](https://static.pepy.tech/badge/ultralytics-thop)](https://pepy.tech/project/thop) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ultralytics-thop?logo=python&logoColor=gold)](https://pypi.org/project/ultralytics-thop/)
+[![PyPI - Version](https://img.shields.io/pypi/v/ultralytics-thop?logo=pypi&logoColor=white)](https://pypi.org/project/ultralytics-thop/) [![Downloads](https://static.pepy.tech/badge/ultralytics-thop)](https://pepy.tech/project/ultralytics-thop) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ultralytics-thop?logo=python&logoColor=gold)](https://pypi.org/project/ultralytics-thop/)
 
 ```bash
 pip install ultralytics-thop
 ```
 
 Alternatively, install the latest version directly from GitHub:
```

