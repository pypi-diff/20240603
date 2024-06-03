# Comparing `tmp/fastmock-0.1.0.tar.gz` & `tmp/fastmock-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastmock-0.1.0.tar", last modified: Sun Jun  2 09:20:08 2024, max compression
+gzip compressed data, was "fastmock-0.1.1.tar", last modified: Mon Jun  3 09:39:54 2024, max compression
```

## Comparing `fastmock-0.1.0.tar` & `fastmock-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 09:20:08.901028 fastmock-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-06-02 09:20:04.000000 fastmock-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-06-02 09:20:04.000000 fastmock-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-06-02 09:20:08.901028 fastmock-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-06-02 09:20:04.000000 fastmock-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 09:20:08.897028 fastmock-0.1.0/fastmock/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 09:20:04.000000 fastmock-0.1.0/fastmock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-06-02 09:20:04.000000 fastmock-0.1.0/fastmock/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-06-02 09:20:04.000000 fastmock-0.1.0/fastmock/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-06-02 09:20:04.000000 fastmock-0.1.0/fastmock/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-06-02 09:20:04.000000 fastmock-0.1.0/fastmock/request_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-06-02 09:20:04.000000 fastmock-0.1.0/fastmock/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 09:20:08.901028 fastmock-0.1.0/fastmock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-06-02 09:20:08.000000 fastmock-0.1.0/fastmock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-06-02 09:20:08.000000 fastmock-0.1.0/fastmock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 09:20:08.000000 fastmock-0.1.0/fastmock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-02 09:20:08.000000 fastmock-0.1.0/fastmock.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 09:20:08.901028 fastmock-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-06-02 09:20:04.000000 fastmock-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 09:20:08.901028 fastmock-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 09:20:04.000000 fastmock-0.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 09:20:08.901028 fastmock-0.1.0/tests/clients/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 09:20:04.000000 fastmock-0.1.0/tests/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-06-02 09:20:04.000000 fastmock-0.1.0/tests/clients/decorator_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-06-02 09:20:04.000000 fastmock-0.1.0/tests/clients/decorator_initialization_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-06-02 09:20:04.000000 fastmock-0.1.0/tests/clients/header_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-06-02 09:20:04.000000 fastmock-0.1.0/tests/clients/middleware_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-06-02 09:20:04.000000 fastmock-0.1.0/tests/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-06-02 09:20:04.000000 fastmock-0.1.0/tests/test_fastmock_data_retrieve_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-06-02 09:20:04.000000 fastmock-0.1.0/tests/test_fastmock_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13452 2024-06-02 09:20:04.000000 fastmock-0.1.0/tests/test_fastmock_middleware_openapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-06-02 09:20:04.000000 fastmock-0.1.0/tests/test_fastmock_parameter_activate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-06-02 09:20:04.000000 fastmock-0.1.0/tests/test_fastmock_parameter_element_size.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-06-02 09:20:04.000000 fastmock-0.1.0/tests/test_fastmock_parameter_response_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-06-02 09:20:04.000000 fastmock-0.1.0/tests/test_fastmock_parameter_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-06-02 09:20:04.000000 fastmock-0.1.0/tests/test_fastmock_response_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:39:54.108004 fastmock-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-06-03 09:39:49.000000 fastmock-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-06-03 09:39:49.000000 fastmock-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-06-03 09:39:54.108004 fastmock-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-06-03 09:39:49.000000 fastmock-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:39:54.104004 fastmock-0.1.1/fastmock/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:39:49.000000 fastmock-0.1.1/fastmock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-06-03 09:39:49.000000 fastmock-0.1.1/fastmock/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-06-03 09:39:49.000000 fastmock-0.1.1/fastmock/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-06-03 09:39:49.000000 fastmock-0.1.1/fastmock/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-06-03 09:39:49.000000 fastmock-0.1.1/fastmock/request_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-06-03 09:39:49.000000 fastmock-0.1.1/fastmock/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:39:54.108004 fastmock-0.1.1/fastmock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-06-03 09:39:54.000000 fastmock-0.1.1/fastmock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-06-03 09:39:54.000000 fastmock-0.1.1/fastmock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 09:39:54.000000 fastmock-0.1.1/fastmock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-03 09:39:54.000000 fastmock-0.1.1/fastmock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 09:39:54.108004 fastmock-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-06-03 09:39:49.000000 fastmock-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:39:54.108004 fastmock-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:39:49.000000 fastmock-0.1.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:39:54.108004 fastmock-0.1.1/tests/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:39:49.000000 fastmock-0.1.1/tests/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-06-03 09:39:49.000000 fastmock-0.1.1/tests/clients/decorator_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-06-03 09:39:49.000000 fastmock-0.1.1/tests/clients/decorator_initialization_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-06-03 09:39:49.000000 fastmock-0.1.1/tests/clients/header_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-06-03 09:39:49.000000 fastmock-0.1.1/tests/clients/middleware_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-06-03 09:39:49.000000 fastmock-0.1.1/tests/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-06-03 09:39:49.000000 fastmock-0.1.1/tests/test_fastmock_data_retrieve_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-06-03 09:39:49.000000 fastmock-0.1.1/tests/test_fastmock_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13452 2024-06-03 09:39:49.000000 fastmock-0.1.1/tests/test_fastmock_middleware_openapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-06-03 09:39:49.000000 fastmock-0.1.1/tests/test_fastmock_parameter_activate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-06-03 09:39:49.000000 fastmock-0.1.1/tests/test_fastmock_parameter_element_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-06-03 09:39:49.000000 fastmock-0.1.1/tests/test_fastmock_parameter_response_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-06-03 09:39:49.000000 fastmock-0.1.1/tests/test_fastmock_parameter_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-06-03 09:39:49.000000 fastmock-0.1.1/tests/test_fastmock_response_type.py
```

### Comparing `fastmock-0.1.0/LICENSE` & `fastmock-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastmock-0.1.0/PKG-INFO` & `fastmock-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: fastmock
-Version: 0.1.0
+Version: 0.1.1
 Summary: FastAPI middleware for mocking responses based on Pydantic models response
 Home-page: https://github.com/tpemeja/fastmock
 Author: Tanguy PEMEJA
 Author-email: tanguy.pemeja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
-  <a href="https://tpemeja.github.io/fastmock"><img src="https://github.com/tpemeja/fastmock/blob/main/docs/FastMock-title.png" alt="fastmock" style="width: 300px; height: 300px;"></a>
+  <a href="https://tpemeja.github.io/fastmock"><img src="https://github.com/tpemeja/fastmock/blob/main/documentation/docs/img/title.png?raw=true" alt="fastmock" style="width: 300px; height: 300px;"></a>
 </p>
 <p align="center">
     FastMock framework, mock your FastAPI APIs
 </p>
 <p align="center">
-<a href="https://github.com/tpemeja/fastmock/workflows/Test/badge.svg" target="_blank">
+<a href="https://github.com/tpemeja/fastmock/actions/workflows/test.yml" target="_blank">
     <img src="https://github.com/tpemeja/fastmock/workflows/Test/badge.svg" alt="Test">
 </a>
-<a href="https://coveralls.io/repos/github/tpemeja/fastmock/badge.svg?branch=main" target="_blank">
+<a href="https://coveralls.io/github/tpemeja/fastmock?branch=main" target="_blank">
     <img src="https://coveralls.io/repos/github/tpemeja/fastmock/badge.svg?branch=main" alt="Coverage">
 </a>
+<a href="https://pypi.org/project/fastmock" target="_blank">
+    <img src="https://img.shields.io/pypi/v/fastmock?color=%2334D058&label=pypi%20package" alt="Package version">
+</a>
 </p>
 
 ---
 
 **Documentation**: <a href="https://tpemeja.github.io/fastmock" target="_blank">https://tpemeja.github.io/fastmock</a>
 
 **Source Code**: <a href="https://github.com/tpemeja/fastmock" target="_blank">https://github.com/tpemeja/fastmock</a>
```

### Comparing `fastmock-0.1.0/README.md` & `fastmock-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 <p align="center">
-  <a href="https://tpemeja.github.io/fastmock"><img src="https://github.com/tpemeja/fastmock/blob/main/docs/FastMock-title.png" alt="fastmock" style="width: 300px; height: 300px;"></a>
+  <a href="https://tpemeja.github.io/fastmock"><img src="https://github.com/tpemeja/fastmock/blob/main/documentation/docs/img/title.png?raw=true" alt="fastmock" style="width: 300px; height: 300px;"></a>
 </p>
 <p align="center">
     FastMock framework, mock your FastAPI APIs
 </p>
 <p align="center">
-<a href="https://github.com/tpemeja/fastmock/workflows/Test/badge.svg" target="_blank">
+<a href="https://github.com/tpemeja/fastmock/actions/workflows/test.yml" target="_blank">
     <img src="https://github.com/tpemeja/fastmock/workflows/Test/badge.svg" alt="Test">
 </a>
-<a href="https://coveralls.io/repos/github/tpemeja/fastmock/badge.svg?branch=main" target="_blank">
+<a href="https://coveralls.io/github/tpemeja/fastmock?branch=main" target="_blank">
     <img src="https://coveralls.io/repos/github/tpemeja/fastmock/badge.svg?branch=main" alt="Coverage">
 </a>
+<a href="https://pypi.org/project/fastmock" target="_blank">
+    <img src="https://img.shields.io/pypi/v/fastmock?color=%2334D058&label=pypi%20package" alt="Package version">
+</a>
 </p>
 
 ---
 
 **Documentation**: <a href="https://tpemeja.github.io/fastmock" target="_blank">https://tpemeja.github.io/fastmock</a>
 
 **Source Code**: <a href="https://github.com/tpemeja/fastmock" target="_blank">https://github.com/tpemeja/fastmock</a>
```

### Comparing `fastmock-0.1.0/fastmock/decorator.py` & `fastmock-0.1.1/fastmock/decorator.py`

 * *Files identical despite different names*

### Comparing `fastmock-0.1.0/fastmock/middleware.py` & `fastmock-0.1.1/fastmock/middleware.py`

 * *Files identical despite different names*

### Comparing `fastmock-0.1.0/fastmock/model.py` & `fastmock-0.1.1/fastmock/model.py`

 * *Files identical despite different names*

### Comparing `fastmock-0.1.0/fastmock/request_response.py` & `fastmock-0.1.1/fastmock/request_response.py`

 * *Files identical despite different names*

### Comparing `fastmock-0.1.0/fastmock/tools.py` & `fastmock-0.1.1/fastmock/tools.py`

 * *Files identical despite different names*

### Comparing `fastmock-0.1.0/fastmock.egg-info/PKG-INFO` & `fastmock-0.1.1/fastmock.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: fastmock
-Version: 0.1.0
+Version: 0.1.1
 Summary: FastAPI middleware for mocking responses based on Pydantic models response
 Home-page: https://github.com/tpemeja/fastmock
 Author: Tanguy PEMEJA
 Author-email: tanguy.pemeja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
-  <a href="https://tpemeja.github.io/fastmock"><img src="https://github.com/tpemeja/fastmock/blob/main/docs/FastMock-title.png" alt="fastmock" style="width: 300px; height: 300px;"></a>
+  <a href="https://tpemeja.github.io/fastmock"><img src="https://github.com/tpemeja/fastmock/blob/main/documentation/docs/img/title.png?raw=true" alt="fastmock" style="width: 300px; height: 300px;"></a>
 </p>
 <p align="center">
     FastMock framework, mock your FastAPI APIs
 </p>
 <p align="center">
-<a href="https://github.com/tpemeja/fastmock/workflows/Test/badge.svg" target="_blank">
+<a href="https://github.com/tpemeja/fastmock/actions/workflows/test.yml" target="_blank">
     <img src="https://github.com/tpemeja/fastmock/workflows/Test/badge.svg" alt="Test">
 </a>
-<a href="https://coveralls.io/repos/github/tpemeja/fastmock/badge.svg?branch=main" target="_blank">
+<a href="https://coveralls.io/github/tpemeja/fastmock?branch=main" target="_blank">
     <img src="https://coveralls.io/repos/github/tpemeja/fastmock/badge.svg?branch=main" alt="Coverage">
 </a>
+<a href="https://pypi.org/project/fastmock" target="_blank">
+    <img src="https://img.shields.io/pypi/v/fastmock?color=%2334D058&label=pypi%20package" alt="Package version">
+</a>
 </p>
 
 ---
 
 **Documentation**: <a href="https://tpemeja.github.io/fastmock" target="_blank">https://tpemeja.github.io/fastmock</a>
 
 **Source Code**: <a href="https://github.com/tpemeja/fastmock" target="_blank">https://github.com/tpemeja/fastmock</a>
```

### Comparing `fastmock-0.1.0/fastmock.egg-info/SOURCES.txt` & `fastmock-0.1.1/fastmock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastmock-0.1.0/setup.py` & `fastmock-0.1.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="fastmock",
-    version="0.1.0",
+    version="0.1.1",
     author="Tanguy PEMEJA",
     author_email="tanguy.pemeja@gmail.com",
     description="FastAPI middleware for mocking responses based on Pydantic models response",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/tpemeja/fastmock",
     packages=find_packages(),
```

### Comparing `fastmock-0.1.0/tests/clients/decorator_client.py` & `fastmock-0.1.1/tests/clients/decorator_client.py`

 * *Files identical despite different names*

### Comparing `fastmock-0.1.0/tests/clients/decorator_initialization_client.py` & `fastmock-0.1.1/tests/clients/decorator_initialization_client.py`

 * *Files identical despite different names*

### Comparing `fastmock-0.1.0/tests/clients/header_client.py` & `fastmock-0.1.1/tests/clients/header_client.py`

 * *Files identical despite different names*

### Comparing `fastmock-0.1.0/tests/clients/middleware_client.py` & `fastmock-0.1.1/tests/clients/middleware_client.py`

 * *Files identical despite different names*

### Comparing `fastmock-0.1.0/tests/device.py` & `fastmock-0.1.1/tests/device.py`

 * *Files identical despite different names*

### Comparing `fastmock-0.1.0/tests/test_fastmock_data_retrieve_order.py` & `fastmock-0.1.1/tests/test_fastmock_data_retrieve_order.py`

 * *Files identical despite different names*

### Comparing `fastmock-0.1.0/tests/test_fastmock_decorator.py` & `fastmock-0.1.1/tests/test_fastmock_decorator.py`

 * *Files identical despite different names*

### Comparing `fastmock-0.1.0/tests/test_fastmock_middleware_openapi.py` & `fastmock-0.1.1/tests/test_fastmock_middleware_openapi.py`

 * *Files identical despite different names*

### Comparing `fastmock-0.1.0/tests/test_fastmock_parameter_activate.py` & `fastmock-0.1.1/tests/test_fastmock_parameter_activate.py`

 * *Files identical despite different names*

### Comparing `fastmock-0.1.0/tests/test_fastmock_parameter_element_size.py` & `fastmock-0.1.1/tests/test_fastmock_parameter_element_size.py`

 * *Files identical despite different names*

### Comparing `fastmock-0.1.0/tests/test_fastmock_parameter_response_status.py` & `fastmock-0.1.1/tests/test_fastmock_parameter_response_status.py`

 * *Files identical despite different names*

### Comparing `fastmock-0.1.0/tests/test_fastmock_parameter_type.py` & `fastmock-0.1.1/tests/test_fastmock_parameter_type.py`

 * *Files identical despite different names*

### Comparing `fastmock-0.1.0/tests/test_fastmock_response_type.py` & `fastmock-0.1.1/tests/test_fastmock_response_type.py`

 * *Files identical despite different names*

