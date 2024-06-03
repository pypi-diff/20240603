# Comparing `tmp/pvat-0.0.0.dev0.tar.gz` & `tmp/pvat-0.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvat-0.0.0.dev0.tar", last modified: Thu May 30 14:55:32 2024, max compression
+gzip compressed data, was "pvat-0.0.0.dev1.tar", last modified: Mon Jun  3 06:15:28 2024, max compression
```

## Comparing `pvat-0.0.0.dev0.tar` & `pvat-0.0.0.dev1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-05-30 14:55:32.074555 pvat-0.0.0.dev0/
--rw-rw-r--   0 juho      (1000) juho      (1000)     1116 2024-05-20 00:24:45.000000 pvat-0.0.0.dev0/LICENSE
--rw-r--r--   0 juho      (1000) juho      (1000)     1746 2024-05-30 14:55:32.074555 pvat-0.0.0.dev0/PKG-INFO
--rw-rw-r--   0 juho      (1000) juho      (1000)      151 2024-05-30 14:48:10.000000 pvat-0.0.0.dev0/README.rst
-drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-05-30 14:55:32.074555 pvat-0.0.0.dev0/pvat/
--rw-rw-r--   0 juho      (1000) juho      (1000)     1018 2024-05-30 14:53:45.000000 pvat-0.0.0.dev0/pvat/__init__.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    13737 2024-05-30 14:51:56.000000 pvat-0.0.0.dev0/pvat/estimators.py
--rw-rw-r--   0 juho      (1000) juho      (1000)        0 2024-05-20 00:51:54.000000 pvat-0.0.0.dev0/pvat/py.typed
-drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-05-30 14:55:32.074555 pvat-0.0.0.dev0/pvat/tests/
--rw-rw-r--   0 juho      (1000) juho      (1000)       80 2024-05-30 14:49:38.000000 pvat-0.0.0.dev0/pvat/tests/__init__.py
--rw-rw-r--   0 juho      (1000) juho      (1000)     4106 2024-05-30 14:50:02.000000 pvat-0.0.0.dev0/pvat/tests/test_estimators.py
--rw-rw-r--   0 juho      (1000) juho      (1000)     6178 2024-05-30 14:52:03.000000 pvat-0.0.0.dev0/pvat/utilities.py
-drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-05-30 14:55:32.074555 pvat-0.0.0.dev0/pvat.egg-info/
--rw-r--r--   0 juho      (1000) juho      (1000)     1746 2024-05-30 14:55:32.000000 pvat-0.0.0.dev0/pvat.egg-info/PKG-INFO
--rw-rw-r--   0 juho      (1000) juho      (1000)      287 2024-05-30 14:55:32.000000 pvat-0.0.0.dev0/pvat.egg-info/SOURCES.txt
--rw-rw-r--   0 juho      (1000) juho      (1000)        1 2024-05-30 14:55:32.000000 pvat-0.0.0.dev0/pvat.egg-info/dependency_links.txt
--rw-rw-r--   0 juho      (1000) juho      (1000)       17 2024-05-30 14:55:32.000000 pvat-0.0.0.dev0/pvat.egg-info/requires.txt
--rw-rw-r--   0 juho      (1000) juho      (1000)        5 2024-05-30 14:55:32.000000 pvat-0.0.0.dev0/pvat.egg-info/top_level.txt
--rw-rw-r--   0 juho      (1000) juho      (1000)       38 2024-05-30 14:55:32.074555 pvat-0.0.0.dev0/setup.cfg
--rw-rw-r--   0 juho      (1000) juho      (1000)     2063 2024-05-30 14:55:06.000000 pvat-0.0.0.dev0/setup.py
+drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-06-03 06:15:28.383872 pvat-0.0.0.dev1/
+-rw-rw-r--   0 juho      (1000) juho      (1000)     1116 2024-05-20 00:24:45.000000 pvat-0.0.0.dev1/LICENSE
+-rw-r--r--   0 juho      (1000) juho      (1000)     1746 2024-06-03 06:15:28.383872 pvat-0.0.0.dev1/PKG-INFO
+-rw-rw-r--   0 juho      (1000) juho      (1000)      151 2024-05-30 14:48:10.000000 pvat-0.0.0.dev1/README.rst
+drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-06-03 06:15:28.379872 pvat-0.0.0.dev1/pvat/
+-rw-rw-r--   0 juho      (1000) juho      (1000)     1018 2024-05-30 14:53:45.000000 pvat-0.0.0.dev1/pvat/__init__.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    16222 2024-06-01 16:49:34.000000 pvat-0.0.0.dev1/pvat/estimators.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)        0 2024-05-20 00:51:54.000000 pvat-0.0.0.dev1/pvat/py.typed
+drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-06-03 06:15:28.383872 pvat-0.0.0.dev1/pvat/tests/
+-rw-rw-r--   0 juho      (1000) juho      (1000)       80 2024-05-30 14:49:38.000000 pvat-0.0.0.dev1/pvat/tests/__init__.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)      660 2024-06-02 04:29:32.000000 pvat-0.0.0.dev1/pvat/tests/test_estimators.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)      280 2024-06-02 04:28:04.000000 pvat-0.0.0.dev1/pvat/tests/test_utilities.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)     6232 2024-06-03 02:26:33.000000 pvat-0.0.0.dev1/pvat/utilities.py
+drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-06-03 06:15:28.383872 pvat-0.0.0.dev1/pvat.egg-info/
+-rw-r--r--   0 juho      (1000) juho      (1000)     1746 2024-06-03 06:15:28.000000 pvat-0.0.0.dev1/pvat.egg-info/PKG-INFO
+-rw-rw-r--   0 juho      (1000) juho      (1000)      316 2024-06-03 06:15:28.000000 pvat-0.0.0.dev1/pvat.egg-info/SOURCES.txt
+-rw-rw-r--   0 juho      (1000) juho      (1000)        1 2024-06-03 06:15:28.000000 pvat-0.0.0.dev1/pvat.egg-info/dependency_links.txt
+-rw-rw-r--   0 juho      (1000) juho      (1000)       17 2024-06-03 06:15:28.000000 pvat-0.0.0.dev1/pvat.egg-info/requires.txt
+-rw-rw-r--   0 juho      (1000) juho      (1000)        5 2024-06-03 06:15:28.000000 pvat-0.0.0.dev1/pvat.egg-info/top_level.txt
+-rw-rw-r--   0 juho      (1000) juho      (1000)       38 2024-06-03 06:15:28.383872 pvat-0.0.0.dev1/setup.cfg
+-rw-rw-r--   0 juho      (1000) juho      (1000)     2063 2024-06-03 06:15:07.000000 pvat-0.0.0.dev1/setup.py
```

### Comparing `pvat-0.0.0.dev0/LICENSE` & `pvat-0.0.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `pvat-0.0.0.dev0/PKG-INFO` & `pvat-0.0.0.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvat
-Version: 0.0.0.dev0
+Version: 0.0.0.dev1
 Summary: Python implementations of variance reduction techniques for extensive-form games
 Home-page: https://github.com/uoftcprg/pvat
 Author: University of Toronto Computer Poker Student Research Group
 Author-email: uoftcprg@studentorg.utoronto.ca
 License: MIT
 Project-URL: Documentation, https://pvat.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/uoftcprg/pvat
```

### Comparing `pvat-0.0.0.dev0/pvat/__init__.py` & `pvat-0.0.0.dev1/pvat/__init__.py`

 * *Files identical despite different names*

### Comparing `pvat-0.0.0.dev0/pvat/utilities.py` & `pvat-0.0.0.dev1/pvat/utilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """:mod:`pvat.utilities` implements classes related to utilities."""
 
 from __future__ import annotations
 
 from collections.abc import Callable, Iterable
 from dataclasses import dataclass
-from itertools import starmap
 from typing import Any, Protocol, TypeVar
 
-from numpy.linalg import inv
 import numpy as np
 
 _H = TypeVar('_H')
 _H_contra = TypeVar('_H_contra', contravariant=True)
 _A_co = TypeVar('_A_co', covariant=True)
 _A_contra = TypeVar('_A_contra', contravariant=True)
 _P_co = TypeVar('_P_co', covariant=True)
@@ -91,16 +89,16 @@
     """The function that maps histories to a vector of features."""
     parameters: Any
     """The parameters of the linear value function."""
 
     @classmethod
     def learn(
             cls,
-            base_term: Callable[[_H_contra], Any],
-            correction_term_sum: (
+            base_term_function: Callable[[_H_contra], Any],
+            correction_term_sum_function: (
                 Callable[[Callable[[_H_contra], Any], _H_contra], Any]
             ),
             feature_extractor: Callable[[_H_contra], Any],
             terminal_histories: Iterable[_H_contra],
             zero_sum: bool = False,
     ) -> LinearValueFunction[_H_contra]:
         """Solve the value estimator for the linear case.
@@ -113,47 +111,52 @@
 
         For n-player, general-sum games, a value function should be
         learned for each player. However, for n-player, zero-sum games,
         this approach would not give a zero-sum guarantee. As such,
         for the case of linear value functions in n-player, zero-sum
         games, the zero-sum option must be activated.
 
-        :param base_term: The base term function.
-        :param correction_term_sum: The correction term function.
+        :param base_term_function: The base term function.
+        :param correction_term_sum_function: The correction term
+                                             function.
         :param feature_extractor: The feature extractor function.
         :param terminal_histories: The terminal histories to learn from.
-        :param zero_sum: ``True`` to enable the zero-sum constraint, else
-                         ``False``. This is only relevant when value is a
-                         vector, not a scalar.
+        :param zero_sum: ``True`` to enable the zero-sum constraint,
+                         else ``False``. This is only relevant when
+                         value is a vector, not a scalar.
         :return: The solution to the value function for the linear case.
         """
-        b = []
-        A = []
+        b_t = []
+        A_t = []
 
         for terminal_history in terminal_histories:
-            b.append(base_term(terminal_history))
-            A.append(correction_term_sum(feature_extractor, terminal_history))
+            b_t.append(base_term_function(terminal_history))
+            A_t.append(
+                correction_term_sum_function(
+                    feature_extractor,
+                    terminal_history,
+                ),
+            )
+
+        b_bar = np.mean(b_t, 0)
+        A_bar = np.mean(A_t, 0)
+        b = np.subtract(b_bar, b_t)
+        A = np.subtract(A_t, A_bar)
 
-        b_bar = np.mean(b, 0)
-        A_bar = np.mean(A, 0)
-
-        A_t_A_t_T_mean = np.mean(tuple(starmap(np.outer, zip(A, A))), 0)
-        A_bar_A_bar_T = np.outer(A_bar, A_bar)
+        if zero_sum:
+            player_count = len(b_bar)
+            S = np.column_stack(
+                (np.eye(player_count - 1), -np.ones(player_count - 1)),
+            )
+            b = b @ S.T @ np.linalg.inv(S @ S.T)
 
-        A_bar_b_bar_T = np.outer(A_bar, b_bar)
-        A_t_b_t_T_mean = np.mean(tuple(starmap(np.outer, zip(A, b))), 0)
-
-        parameters = (
-            inv(A_t_A_t_T_mean - A_bar_A_bar_T)
-            @ (A_bar_b_bar_T - A_t_b_t_T_mean)
-        )
+        parameters = np.linalg.lstsq(A, b)[0]
 
         if zero_sum:
-            player_count = len(b_bar)
-            parameters @= np.eye(player_count) - 1 / player_count
+            parameters = parameters @ S
 
         return LinearValueFunction(feature_extractor, parameters)
 
     def __call__(self, terminal_history: _H_contra) -> Any:
         return self.parameters.T @ self.feature_extractor(terminal_history)
```

### Comparing `pvat-0.0.0.dev0/pvat.egg-info/PKG-INFO` & `pvat-0.0.0.dev1/pvat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvat
-Version: 0.0.0.dev0
+Version: 0.0.0.dev1
 Summary: Python implementations of variance reduction techniques for extensive-form games
 Home-page: https://github.com/uoftcprg/pvat
 Author: University of Toronto Computer Poker Student Research Group
 Author-email: uoftcprg@studentorg.utoronto.ca
 License: MIT
 Project-URL: Documentation, https://pvat.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/uoftcprg/pvat
```

### Comparing `pvat-0.0.0.dev0/setup.py` & `pvat-0.0.0.dev1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 
 from setuptools import find_packages, setup
 
 setup(
     name='pvat',
-    version='0.0.0.dev0',
+    version='0.0.0.dev1',
     description=(
         'Python implementations of variance reduction techniques for'
         ' extensive-form games'
     ),
     long_description=open('README.rst').read(),
     long_description_content_type='text/x-rst',
     url='https://github.com/uoftcprg/pvat',
```

