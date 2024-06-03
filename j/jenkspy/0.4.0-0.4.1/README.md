# Comparing `tmp/jenkspy-0.4.0.tar.gz` & `tmp/jenkspy-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jenkspy-0.4.0.tar", last modified: Thu Nov 30 11:20:08 2023, max compression
+gzip compressed data, was "jenkspy-0.4.1.tar", last modified: Mon Jun  3 12:46:50 2024, max compression
```

## Comparing `jenkspy-0.4.0.tar` & `jenkspy-0.4.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 mthh      (1000) mthh      (1000)        0 2023-11-30 11:20:08.416013 jenkspy-0.4.0/
--rwxrwxr-x   0 mthh      (1000) mthh      (1000)     1075 2023-07-03 10:04:21.000000 jenkspy-0.4.0/LICENSE
--rwxrwxr-x   0 mthh      (1000) mthh      (1000)      125 2023-07-03 10:04:21.000000 jenkspy-0.4.0/MANIFEST.in
--rw-r--r--   0 mthh      (1000) mthh      (1000)     6089 2023-11-30 11:20:08.416013 jenkspy-0.4.0/PKG-INFO
--rw-rw-r--   0 mthh      (1000) mthh      (1000)     5164 2023-11-30 11:13:19.000000 jenkspy-0.4.0/README.rst
-drwxrwxr-x   0 mthh      (1000) mthh      (1000)        0 2023-11-30 11:20:08.416013 jenkspy-0.4.0/jenkspy/
--rw-rw-r--   0 mthh      (1000) mthh      (1000)      241 2023-11-30 11:14:27.000000 jenkspy-0.4.0/jenkspy/__init__.py
--rw-rw-r--   0 mthh      (1000) mthh      (1000)     8440 2023-07-03 10:15:47.000000 jenkspy-0.4.0/jenkspy/core.py
-drwxrwxr-x   0 mthh      (1000) mthh      (1000)        0 2023-11-30 11:20:08.416013 jenkspy-0.4.0/jenkspy/src/
--rw-rw-r--   0 mthh      (1000) mthh      (1000)     5730 2023-07-03 10:04:21.000000 jenkspy-0.4.0/jenkspy/src/_jenks.c
--rw-rw-r--   0 mthh      (1000) mthh      (1000)  1076924 2023-11-30 11:19:36.000000 jenkspy-0.4.0/jenkspy/src/jenks.c
--rwxrwxr-x   0 mthh      (1000) mthh      (1000)     4150 2023-07-03 10:04:21.000000 jenkspy-0.4.0/jenkspy/src/jenks.pyx
-drwxrwxr-x   0 mthh      (1000) mthh      (1000)        0 2023-11-30 11:20:08.416013 jenkspy-0.4.0/jenkspy.egg-info/
--rw-r--r--   0 mthh      (1000) mthh      (1000)     6089 2023-11-30 11:20:08.000000 jenkspy-0.4.0/jenkspy.egg-info/PKG-INFO
--rw-rw-r--   0 mthh      (1000) mthh      (1000)      363 2023-11-30 11:20:08.000000 jenkspy-0.4.0/jenkspy.egg-info/SOURCES.txt
--rw-rw-r--   0 mthh      (1000) mthh      (1000)        1 2023-11-30 11:20:08.000000 jenkspy-0.4.0/jenkspy.egg-info/dependency_links.txt
--rw-rw-r--   0 mthh      (1000) mthh      (1000)        6 2023-11-30 11:20:08.000000 jenkspy-0.4.0/jenkspy.egg-info/requires.txt
--rw-rw-r--   0 mthh      (1000) mthh      (1000)        8 2023-11-30 11:20:08.000000 jenkspy-0.4.0/jenkspy.egg-info/top_level.txt
--rw-rw-r--   0 mthh      (1000) mthh      (1000)        5 2023-07-03 10:04:21.000000 jenkspy-0.4.0/requirements.txt
--rw-rw-r--   0 mthh      (1000) mthh      (1000)       38 2023-11-30 11:20:08.416013 jenkspy-0.4.0/setup.cfg
--rw-rw-r--   0 mthh      (1000) mthh      (1000)     1829 2023-11-30 11:12:53.000000 jenkspy-0.4.0/setup.py
-drwxrwxr-x   0 mthh      (1000) mthh      (1000)        0 2023-11-30 11:20:08.416013 jenkspy-0.4.0/tests/
--rwxrwxr-x   0 mthh      (1000) mthh      (1000)        0 2023-07-03 10:04:21.000000 jenkspy-0.4.0/tests/__init__.py
--rw-rw-r--   0 mthh      (1000) mthh      (1000)    36567 2023-07-03 10:04:21.000000 jenkspy-0.4.0/tests/test.json
--rwxrwxr-x   0 mthh      (1000) mthh      (1000)    48973 2023-07-03 10:16:43.000000 jenkspy-0.4.0/tests/test_jenks.py
+drwxrwxr-x   0 mthh      (1000) mthh      (1000)        0 2024-06-03 12:46:50.701018 jenkspy-0.4.1/
+-rwxrwxr-x   0 mthh      (1000) mthh      (1000)     1075 2023-07-03 10:04:21.000000 jenkspy-0.4.1/LICENSE
+-rwxrwxr-x   0 mthh      (1000) mthh      (1000)       12 2024-06-03 12:38:29.000000 jenkspy-0.4.1/MANIFEST.in
+-rw-r--r--   0 mthh      (1000) mthh      (1000)     7101 2024-06-03 12:46:50.701018 jenkspy-0.4.1/PKG-INFO
+-rw-rw-r--   0 mthh      (1000) mthh      (1000)     4697 2024-06-03 12:38:29.000000 jenkspy-0.4.1/README.md
+drwxrwxr-x   0 mthh      (1000) mthh      (1000)        0 2024-06-03 12:46:50.701018 jenkspy-0.4.1/jenkspy/
+-rw-rw-r--   0 mthh      (1000) mthh      (1000)      241 2024-06-03 12:38:29.000000 jenkspy-0.4.1/jenkspy/__init__.py
+-rw-rw-r--   0 mthh      (1000) mthh      (1000)     8440 2023-07-03 10:15:47.000000 jenkspy-0.4.1/jenkspy/core.py
+drwxrwxr-x   0 mthh      (1000) mthh      (1000)        0 2024-06-03 12:46:50.701018 jenkspy-0.4.1/jenkspy/src/
+-rw-rw-r--   0 mthh      (1000) mthh      (1000)     5730 2023-07-03 10:04:21.000000 jenkspy-0.4.1/jenkspy/src/_jenks.c
+-rw-rw-r--   0 mthh      (1000) mthh      (1000)  1077026 2024-06-03 12:46:50.000000 jenkspy-0.4.1/jenkspy/src/jenks.c
+-rwxrwxr-x   0 mthh      (1000) mthh      (1000)     4150 2023-07-03 10:04:21.000000 jenkspy-0.4.1/jenkspy/src/jenks.pyx
+drwxrwxr-x   0 mthh      (1000) mthh      (1000)        0 2024-06-03 12:46:50.701018 jenkspy-0.4.1/jenkspy.egg-info/
+-rw-r--r--   0 mthh      (1000) mthh      (1000)     7101 2024-06-03 12:46:50.000000 jenkspy-0.4.1/jenkspy.egg-info/PKG-INFO
+-rw-rw-r--   0 mthh      (1000) mthh      (1000)      360 2024-06-03 12:46:50.000000 jenkspy-0.4.1/jenkspy.egg-info/SOURCES.txt
+-rw-rw-r--   0 mthh      (1000) mthh      (1000)        1 2024-06-03 12:46:50.000000 jenkspy-0.4.1/jenkspy.egg-info/dependency_links.txt
+-rw-rw-r--   0 mthh      (1000) mthh      (1000)        6 2024-06-03 12:46:50.000000 jenkspy-0.4.1/jenkspy.egg-info/requires.txt
+-rw-rw-r--   0 mthh      (1000) mthh      (1000)        8 2024-06-03 12:46:50.000000 jenkspy-0.4.1/jenkspy.egg-info/top_level.txt
+-rw-rw-r--   0 mthh      (1000) mthh      (1000)     1463 2024-06-03 12:38:29.000000 jenkspy-0.4.1/pyproject.toml
+-rw-rw-r--   0 mthh      (1000) mthh      (1000)       38 2024-06-03 12:46:50.701018 jenkspy-0.4.1/setup.cfg
+-rw-rw-r--   0 mthh      (1000) mthh      (1000)      356 2024-06-03 12:38:42.000000 jenkspy-0.4.1/setup.py
+drwxrwxr-x   0 mthh      (1000) mthh      (1000)        0 2024-06-03 12:46:50.701018 jenkspy-0.4.1/tests/
+-rwxrwxr-x   0 mthh      (1000) mthh      (1000)        0 2023-07-03 10:04:21.000000 jenkspy-0.4.1/tests/__init__.py
+-rw-rw-r--   0 mthh      (1000) mthh      (1000)    36567 2023-07-03 10:04:21.000000 jenkspy-0.4.1/tests/test.json
+-rwxrwxr-x   0 mthh      (1000) mthh      (1000)    48973 2023-07-03 10:16:43.000000 jenkspy-0.4.1/tests/test_jenks.py
```

### Comparing `jenkspy-0.4.0/LICENSE` & `jenkspy-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jenkspy-0.4.0/README.rst` & `jenkspy-0.4.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,123 +1,112 @@
-Fast Fisher-Jenks breaks for Python
-===================================
+# Jenkspy: Fast Fisher-Jenks breaks for Python
 
 Compute "natural breaks" (*Fisher-Jenks algorithm*) on list / tuple / array / numpy.ndarray of integers/floats.
 
 The algorithm implemented by this library is also sometimes referred to as *Fisher-Jenks algorithm*, *Jenks Optimisation Method* or *Fisher exact optimization method*. This is a deterministic method to calculate the optimal class boundaries.
 
-Intended compatibility: CPython 3.6+
+Intended compatibility: CPython 3.7+
 
 Wheels are provided via PyPI for Windows / MacOS / Linux users - Also available on conda-forge channel for Anaconda users.
 
-|Version| |Anaconda-Server Badge| |Build Status GH| |PyPI download month|
+[![](https://github.com/mthh/jenkspy/actions/workflows/wheel.yml/badge.svg)](https://github.com/mthh/jenkspy/actions/workflows/wheel.yml)
+[![](https://img.shields.io/pypi/v/jenkspy.svg?color=007ec6)](https://pypi.python.org/pypi/jenkspy)
+[![](https://anaconda.org/conda-forge/jenkspy/badges/version.svg)](https://anaconda.org/conda-forge/jenkspy)
+[![](https://img.shields.io/pypi/dm/jenkspy.svg)](https://pypi.python.org/pypi/jenkspy)
 
-Usage
------
+## Usage
 
 Two ways of using `jenkspy` are available:
 
-- by using the ``jenks_breaks`` function which takes as input a `list <https://docs.python.org/3/library/stdtypes.html#list>`_ / `tuple <https://docs.python.org/3/library/stdtypes.html#tuple>`_ / `array.array <https://docs.python.org/3/library/array.html#array.array>`_ / `numpy.ndarray <https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html>`_ of integers or floats and returns a list of values that correspond to the limits of the classes (starting with the minimum value of the series - the lower bound of the first class - and ending with its maximum value - the upper bound of the last class).
+- by using the `jenks_breaks` function which takes as input
+a [`list`](https://docs.python.org/3/library/stdtypes.html#list)
+/ [`tuple`](https://docs.python.org/3/library/stdtypes.html#tuple)
+/ [`array.array`](https://docs.python.org/3/library/array.html#array.array)
+/ [`numpy.ndarray`](https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html) of integers or floats and returns a list of values that correspond to the limits of the classes (starting with the minimum value of the series - the lower bound of the first class - and ending with its maximum value - the upper bound of the last class).
+
+```python
+>>> import jenkspy
+>>> import json
+
+>>> with open('tests/test.json', 'r') as f:
+...     # Read some data from a JSON file
+...     data = json.loads(f.read())
+...
+>>> jenkspy.jenks_breaks(data, n_classes=5) # Asking for 5 classes
+[0.0028109620325267315, 2.0935479691252112, 4.205495140049607, 6.178148351609707, 8.09175917180255, 9.997982932254672]
+# ^                      ^                    ^                 ^                  ^                 ^
+# Lower bound            Upper bound          Upper bound       Upper bound        Upper bound       Upper bound
+# 1st class              1st class            2nd class         3rd class          4th class         5th class
+# (Minimum value)                                                                                    (Maximum value)
+```
+
+- by using the `JenksNaturalBreaks` class that is inspired by `scikit-learn` classes.
+
+The `.fit` and `.group` behavior is slightly different from `jenks_breaks`,
+by accepting value outside the range of the minimum and maximum value of `breaks_`,
+retaining the input size. It means that fit and group will use only the `inner_breaks_`.
+All value below the min bound will be included in the first group and all value higher than the max bound will be included in the last group.
+
+```python
+>>> from jenkspy import JenksNaturalBreaks
+
+>>> x = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11]
+
+>>> jnb = JenksNaturalBreaks(4) # Asking for 4 clusters
+
+>>> jnb.fit(x) # Create the clusters according to values in 'x'
+>>> print(jnb.labels_) # Labels for fitted data
+... print(jnb.groups_) # Content of each group
+... print(jnb.breaks_) # Break values (including min and max)
+... print(jnb.inner_breaks_) # Inner breaks (ie breaks_[1:-1])
+[0 0 0 1 1 1 2 2 2 3 3 3]
+[array([0, 1, 2]), array([3, 4, 5]), array([6, 7, 8]), array([ 9, 10, 11])]
+[0.0, 2.0, 5.0, 8.0, 11.0]
+[2.0, 5.0, 8.0]
+
+>>> print(jnb.predict(15)) # Predict the group of a value
+3
+
+>>> print(jnb.predict([2.5, 3.5, 6.5])) # Predict the group of several values
+[1 1 2]
+
+>>> print(jnb.group([2.5, 3.5, 6.5])) # Group the elements into there groups
+[array([], dtype=float64), array([2.5, 3.5]), array([6.5]), array([], dtype=float64)]
+```
+
+## Installation
+
+- **From pypi**
+
+```shell
+pip install jenkspy
+```
+
+- **From source**
+
+```shell
+git clone http://github.com/mthh/jenkspy
+cd jenkspy/
+pip install .
+```
+
+- **For anaconda users**
+
+```shell
+conda install -c conda-forge jenkspy
+```
 
-.. code:: python
+## Requirements
 
-    >>> import jenkspy
-    >>> import json
-
-    >>> with open('tests/test.json', 'r') as f:
-    ...     # Read some data from a JSON file
-    ...     data = json.loads(f.read())
-    ...
-    >>> jenkspy.jenks_breaks(data, n_classes=5) # Asking for 5 classes
-    [0.0028109620325267315, 2.0935479691252112, 4.205495140049607, 6.178148351609707, 8.09175917180255, 9.997982932254672]
-    # ^                      ^                    ^                 ^                  ^                 ^
-    # Lower bound            Upper bound          Upper bound       Upper bound        Upper bound       Upper bound
-    # 1st class              1st class            2nd class         3rd class          4th class         5th class
-    # (Minimum value)                                                                                    (Maximum value)
-
-
-- by using the ``JenksNaturalBreaks`` class that is inspired by ``scikit-learn`` classes.
-
-The ``.fit`` and ``.group`` behavior is slightly different from ``jenks_breaks``, by accepting value outside the range of the minimum and maximum value of ``breaks_``, retaining the input size. It means that fit and group will use only the ``inner_breaks_``. All value below the min bound will be included in the first group and all value higher than the max bound will be included in the last group.
-
-.. code:: python
-
-    >>> from jenkspy import JenksNaturalBreaks
-
-    >>> x = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11]
-
-    >>> jnb = JenksNaturalBreaks(4) # Asking for 4 clusters
-
-    >>> jnb.fit(x) # Create the clusters according to values in 'x'
-    >>> print(jnb.labels_) # Labels for fitted data
-    ... print(jnb.groups_) # Content of each group
-    ... print(jnb.breaks_) # Break values (including min and max)
-    ... print(jnb.inner_breaks_) # Inner breaks (ie breaks_[1:-1])
-    [0 0 0 1 1 1 2 2 2 3 3 3]
-    [array([0, 1, 2]), array([3, 4, 5]), array([6, 7, 8]), array([ 9, 10, 11])]
-    [0.0, 2.0, 5.0, 8.0, 11.0]
-    [2.0, 5.0, 8.0]
-
-    >>> print(jnb.predict(15)) # Predict the group of a value
-    3
-
-    >>> print(jnb.predict([2.5, 3.5, 6.5])) # Predict the group of several values
-    [1 1 2]
-
-    >>> print(jnb.group([2.5, 3.5, 6.5])) # Group the elements into there groups
-    [array([], dtype=float64), array([2.5, 3.5]), array([6.5]), array([], dtype=float64)]
-
-
-Installation
-------------
-
-+ **From pypi**
-
-.. code:: shell
-
-    pip install jenkspy
-
-
-+ **From source**
-
-.. code:: shell
-
-    git clone http://github.com/mthh/jenkspy
-    cd jenkspy/
-    python setup.py install
-
-+ **For anaconda users**
-
-.. code:: shell
-
-    conda install -c conda-forge jenkspy
-
-
-Requirements :
---------------
-
-- `Numpy <https://numpy.org>`_
+- [Numpy](https://numpy.org)
 
 -  Only for building from source: C compiler, Python C headers, setuptools and Cython.
 
 
-Motivation :
-------------
+## Motivation:
 
 -  Making a painless installing C extension so it could be used more easily
    as a dependency in an other package (and so learning how to build wheels
    using *appveyor* / *travis* at first - now it uses *GitHub Actions*).
 -  Getting the break values! (and fast!). No fancy functionality provided,
    but contributions/forks/etc are welcome.
 -  Other python implementations are currently existing but not as fast or not available on PyPi.
-
-.. |Build status GH| image:: https://github.com/mthh/jenkspy/actions/workflows/wheel.yml/badge.svg
-   :target: https://github.com/mthh/jenkspy/actions/workflows/wheel.yml
-
-.. |Version| image:: https://img.shields.io/pypi/v/jenkspy.svg?color=007ec6
-   :target: https://pypi.python.org/pypi/jenkspy
-
-.. |Anaconda-Server Badge| image:: https://anaconda.org/conda-forge/jenkspy/badges/version.svg
-   :target: https://anaconda.org/conda-forge/jenkspy
-
-.. |PyPI download month| image:: https://img.shields.io/pypi/dm/jenkspy.svg
-   :target: https://pypi.python.org/pypi/jenkspy
```

### Comparing `jenkspy-0.4.0/jenkspy/core.py` & `jenkspy-0.4.1/jenkspy/core.py`

 * *Files identical despite different names*

### Comparing `jenkspy-0.4.0/jenkspy/src/_jenks.c` & `jenkspy-0.4.1/jenkspy/src/_jenks.c`

 * *Files identical despite different names*

### Comparing `jenkspy-0.4.0/jenkspy/src/jenks.c` & `jenkspy-0.4.1/jenkspy/src/jenks.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.6 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "jenkspy/src/_jenks.c"
         ],
@@ -39,18 +39,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_6" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030006F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -134,14 +134,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -195,14 +197,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -256,60 +260,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -392,14 +419,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -584,22 +614,22 @@
     static CYTHON_INLINE PyObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
         PyObject *exception_table = NULL;
         PyObject *types_module=NULL, *code_type=NULL, *result=NULL;
         #if __PYX_LIMITED_VERSION_HEX < 0x030B0000
-        PyObject *version_info; // borrowed
+        PyObject *version_info;
         PyObject *py_minor_version = NULL;
         #endif
         long minor_version = 0;
         PyObject *type, *value, *traceback;
         PyErr_Fetch(&type, &value, &traceback);
         #if __PYX_LIMITED_VERSION_HEX >= 0x030B0000
-        minor_version = 11; // we don't yet need to distinguish between versions > 11
+        minor_version = 11;
         #else
         if (!(version_info = PySys_GetObject("version_info"))) goto end;
         if (!(py_minor_version = PySequence_GetItem(version_info, 1))) goto end;
         minor_version = PyLong_AsLong(py_minor_version);
         Py_DECREF(py_minor_version);
         if (minor_version == -1 && PyErr_Occurred()) goto end;
         #endif
@@ -649,15 +679,15 @@
     #endif
 #elif PY_VERSION_HEX >= 0x030B0000
   static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
     PyCodeObject *result;
-    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);  // we don't have access to __pyx_empty_bytes here
+    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);
     if (!empty_bytes) return NULL;
     result =
       #if PY_VERSION_HEX >= 0x030C0000
         PyUnstable_Code_NewWithPosOnlyArgs
       #else
         PyCode_NewWithPosOnlyArgs
       #endif
@@ -735,16 +765,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -1088,15 +1123,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if PY_VERSION_HEX >= 0x030d00A1
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1175,15 +1210,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1282,32 +1317,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -1349,15 +1367,15 @@
     #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
   #else
     #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
     #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
   #endif
   typedef Py_ssize_t  __Pyx_compact_pylong;
   typedef size_t  __Pyx_compact_upylong;
-  #else  // Py < 3.12
+  #else
   #define __Pyx_PyLong_IsNeg(x)  (Py_SIZE(x) < 0)
   #define __Pyx_PyLong_IsNonNeg(x)  (Py_SIZE(x) >= 0)
   #define __Pyx_PyLong_IsZero(x)  (Py_SIZE(x) == 0)
   #define __Pyx_PyLong_IsPos(x)  (Py_SIZE(x) > 0)
   #define __Pyx_PyLong_CompactValueUnsigned(x)  ((Py_SIZE(x) == 0) ? 0 : __Pyx_PyLong_Digits(x)[0])
   #define __Pyx_PyLong_DigitCount(x)  __Pyx_sst_abs(Py_SIZE(x))
   #define __Pyx_PyLong_SignedDigitCount(x)  Py_SIZE(x)
@@ -1933,16 +1951,16 @@
 #else
     #define __Pyx_Arg_VARARGS(args, i) PyTuple_GetItem(args, i)
 #endif
 #if CYTHON_AVOID_BORROWED_REFS
     #define __Pyx_Arg_NewRef_VARARGS(arg) __Pyx_NewRef(arg)
     #define __Pyx_Arg_XDECREF_VARARGS(arg) Py_XDECREF(arg)
 #else
-    #define __Pyx_Arg_NewRef_VARARGS(arg) arg // no-op
-    #define __Pyx_Arg_XDECREF_VARARGS(arg) // no-op - arg is borrowed
+    #define __Pyx_Arg_NewRef_VARARGS(arg) arg
+    #define __Pyx_Arg_XDECREF_VARARGS(arg)
 #endif
 #define __Pyx_NumKwargs_VARARGS(kwds) PyDict_Size(kwds)
 #define __Pyx_KwValues_VARARGS(args, nargs) NULL
 #define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
 #define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
 #if CYTHON_METH_FASTCALL
     #define __Pyx_Arg_FASTCALL(args, i) args[i]
@@ -1950,16 +1968,17 @@
     #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
     static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
     CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues);
   #else
     #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
   #endif
-    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg // no-op, __Pyx_Arg_FASTCALL is direct and this needs
-    #define __Pyx_Arg_XDECREF_FASTCALL(arg)  // no-op - arg was returned from array
+    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg  /* no-op, __Pyx_Arg_FASTCALL is direct and this needs
+                                                   to have the same reference counting */
+    #define __Pyx_Arg_XDECREF_FASTCALL(arg)
 #else
     #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
     #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
     #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
     #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
     #define __Pyx_KwargsAsDict_FASTCALL __Pyx_KwargsAsDict_VARARGS
     #define __Pyx_Arg_NewRef_FASTCALL(arg) __Pyx_Arg_NewRef_VARARGS(arg)
@@ -2535,15 +2554,15 @@
     PyObject *func_code;
     PyObject *func_closure;
 #if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     PyObject *func_classobj;
 #endif
     void *defaults;
     int defaults_pyobjects;
-    size_t defaults_size;  // used by FusedFunction for copying defaults
+    size_t defaults_size;
     int flags;
     PyObject *defaults_tuple;
     PyObject *defaults_kwdict;
     PyObject *(*defaults_getter)(PyObject *);
     PyObject *func_annotations;
     PyObject *func_is_coroutine;
 } __pyx_CyFunctionObject;
@@ -20450,15 +20469,15 @@
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("jenks", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #elif CYTHON_USE_MODULE_STATE
   __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   {
     int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
-    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to jenks pseudovariable */
+    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to "jenks" pseudovariable */
     if (unlikely((add_module_result < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
     pystate_addmodule_run = 1;
   }
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
@@ -21528,19 +21547,19 @@
     {
         if (s == PyTuple_GET_ITEM(kwnames, i)) return kwvalues[i];
     }
     for (i = 0; i < n; i++)
     {
         int eq = __Pyx_PyUnicode_Equals(s, PyTuple_GET_ITEM(kwnames, i), Py_EQ);
         if (unlikely(eq != 0)) {
-            if (unlikely(eq < 0)) return NULL;  // error
+            if (unlikely(eq < 0)) return NULL;
             return kwvalues[i];
         }
     }
-    return NULL;  // not found (no exception set)
+    return NULL;
 }
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
 CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues) {
     Py_ssize_t i, nkwargs = PyTuple_GET_SIZE(kwnames);
     PyObject *dict;
     dict = PyDict_New();
     if (unlikely(!dict))
@@ -21645,15 +21664,15 @@
 #endif
         }
         name = first_kw_arg;
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-            Py_INCREF(value); // transfer ownership of value to values
+            Py_INCREF(value);
             Py_DECREF(key);
 #endif
             key = NULL;
             value = NULL;
             continue;
         }
 #if !CYTHON_AVOID_BORROWED_REFS
@@ -21664,15 +21683,15 @@
         #if PY_MAJOR_VERSION < 3
         if (likely(PyString_Check(key))) {
             while (*name) {
                 if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
                         && _PyString_Eq(**name, key)) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL;  // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -21696,15 +21715,15 @@
                 #endif
                     PyUnicode_Compare(**name, key)
                 );
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL; // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -25375,15 +25394,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
@@ -25834,15 +25853,15 @@
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
     #else
     py_code = PyCode_NewEmpty(filename, funcname, py_line);
     #endif
-    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
+    Py_XDECREF(py_funcname);
     return py_code;
 bad:
     Py_XDECREF(py_funcname);
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_srcfile);
     #endif
     return NULL;
```

### Comparing `jenkspy-0.4.0/jenkspy/src/jenks.pyx` & `jenkspy-0.4.1/jenkspy/src/jenks.pyx`

 * *Files identical despite different names*

### Comparing `jenkspy-0.4.0/tests/test.json` & `jenkspy-0.4.1/tests/test.json`

 * *Files identical despite different names*

### Comparing `jenkspy-0.4.0/tests/test_jenks.py` & `jenkspy-0.4.1/tests/test_jenks.py`

 * *Files identical despite different names*

