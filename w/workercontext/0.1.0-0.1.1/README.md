# Comparing `tmp/workercontext-0.1.0.tar.gz` & `tmp/workercontext-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "workercontext-0.1.0.tar", last modified: Sat Jun  1 02:04:22 2024, max compression
+gzip compressed data, was "workercontext-0.1.1.tar", last modified: Mon Jun  3 02:17:02 2024, max compression
```

## Comparing `workercontext-0.1.0.tar` & `workercontext-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 02:04:22.549301 workercontext-0.1.0/
--rw-rw-rw-   0        0        0     1088 2023-04-26 08:49:47.000000 workercontext-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     7586 2024-06-01 02:04:22.547301 workercontext-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5722 2024-06-01 01:56:00.000000 workercontext-0.1.0/README.md
--rw-rw-rw-   0        0        0      738 2024-06-01 01:56:00.000000 workercontext-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-06-01 02:04:22.549301 workercontext-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-06-01 02:04:22.522301 workercontext-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-06-01 02:04:22.530300 workercontext-0.1.0/src/workercontext/
--rw-rw-rw-   0        0        0      137 2024-06-01 01:56:00.000000 workercontext-0.1.0/src/workercontext/__init__.py
--rw-rw-rw-   0        0        0    11020 2024-06-01 01:56:00.000000 workercontext-0.1.0/src/workercontext/multiworker.py
--rw-rw-rw-   0        0        0     4766 2024-06-01 01:56:00.000000 workercontext-0.1.0/src/workercontext/reductions.py
-drwxrwxrwx   0        0        0        0 2024-06-01 02:04:22.546300 workercontext-0.1.0/src/workercontext.egg-info/
--rw-rw-rw-   0        0        0     7586 2024-06-01 02:04:22.000000 workercontext-0.1.0/src/workercontext.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      456 2024-06-01 02:04:22.000000 workercontext-0.1.0/src/workercontext.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 02:04:22.000000 workercontext-0.1.0/src/workercontext.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-06-01 02:04:22.000000 workercontext-0.1.0/src/workercontext.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-06-01 02:04:22.545302 workercontext-0.1.0/tests/
--rw-rw-rw-   0        0        0     1943 2024-06-01 01:56:00.000000 workercontext-0.1.0/tests/test_auto_parallelise.py
--rw-rw-rw-   0        0        0     3248 2024-06-01 01:58:34.000000 workercontext-0.1.0/tests/test_multiworker.py
--rw-rw-rw-   0        0        0     1546 2024-06-01 01:56:00.000000 workercontext-0.1.0/tests/test_multiworker_async.py
--rw-rw-rw-   0        0        0     2261 2024-06-01 01:56:00.000000 workercontext-0.1.0/tests/test_parallelise.py
--rw-rw-rw-   0        0        0     1291 2023-04-26 09:06:41.000000 workercontext-0.1.0/tests/test_performance.py
--rw-rw-rw-   0        0        0     2450 2024-06-01 01:56:00.000000 workercontext-0.1.0/tests/test_reduction.py
+drwxr-xr-x   0 owenelliott   (501) staff       (20)        0 2024-06-03 02:17:02.971807 workercontext-0.1.1/
+-rw-r--r--   0 owenelliott   (501) staff       (20)     1068 2023-08-04 22:21:53.000000 workercontext-0.1.1/LICENSE
+-rw-r--r--   0 owenelliott   (501) staff       (20)     7361 2024-06-03 02:17:02.971556 workercontext-0.1.1/PKG-INFO
+-rw-r--r--   0 owenelliott   (501) staff       (20)     5533 2024-06-03 02:03:02.000000 workercontext-0.1.1/README.md
+-rw-r--r--   0 owenelliott   (501) staff       (20)      715 2024-06-03 02:06:39.000000 workercontext-0.1.1/pyproject.toml
+-rw-r--r--   0 owenelliott   (501) staff       (20)       38 2024-06-03 02:17:02.971860 workercontext-0.1.1/setup.cfg
+drwxr-xr-x   0 owenelliott   (501) staff       (20)        0 2024-06-03 02:17:02.966712 workercontext-0.1.1/src/
+drwxr-xr-x   0 owenelliott   (501) staff       (20)        0 2024-06-03 02:17:02.968070 workercontext-0.1.1/src/workercontext/
+-rw-r--r--   0 owenelliott   (501) staff       (20)      130 2024-06-03 02:03:02.000000 workercontext-0.1.1/src/workercontext/__init__.py
+-rw-r--r--   0 owenelliott   (501) staff       (20)    11043 2024-06-03 02:15:39.000000 workercontext-0.1.1/src/workercontext/multiworker.py
+-rw-r--r--   0 owenelliott   (501) staff       (20)     4566 2024-06-03 02:03:02.000000 workercontext-0.1.1/src/workercontext/reductions.py
+drwxr-xr-x   0 owenelliott   (501) staff       (20)        0 2024-06-03 02:17:02.971205 workercontext-0.1.1/src/workercontext.egg-info/
+-rw-r--r--   0 owenelliott   (501) staff       (20)     7361 2024-06-03 02:17:02.000000 workercontext-0.1.1/src/workercontext.egg-info/PKG-INFO
+-rw-r--r--   0 owenelliott   (501) staff       (20)      456 2024-06-03 02:17:02.000000 workercontext-0.1.1/src/workercontext.egg-info/SOURCES.txt
+-rw-r--r--   0 owenelliott   (501) staff       (20)        1 2024-06-03 02:17:02.000000 workercontext-0.1.1/src/workercontext.egg-info/dependency_links.txt
+-rw-r--r--   0 owenelliott   (501) staff       (20)       14 2024-06-03 02:17:02.000000 workercontext-0.1.1/src/workercontext.egg-info/top_level.txt
+drwxr-xr-x   0 owenelliott   (501) staff       (20)        0 2024-06-03 02:17:02.970792 workercontext-0.1.1/tests/
+-rw-r--r--   0 owenelliott   (501) staff       (20)     1877 2024-06-03 02:03:02.000000 workercontext-0.1.1/tests/test_auto_parallelise.py
+-rw-r--r--   0 owenelliott   (501) staff       (20)     3492 2024-06-03 02:15:39.000000 workercontext-0.1.1/tests/test_multiworker.py
+-rw-r--r--   0 owenelliott   (501) staff       (20)     1481 2024-06-03 02:03:02.000000 workercontext-0.1.1/tests/test_multiworker_async.py
+-rw-r--r--   0 owenelliott   (501) staff       (20)     2176 2024-06-03 02:03:02.000000 workercontext-0.1.1/tests/test_parallelise.py
+-rw-r--r--   0 owenelliott   (501) staff       (20)     1237 2023-08-04 22:21:53.000000 workercontext-0.1.1/tests/test_performance.py
+-rw-r--r--   0 owenelliott   (501) staff       (20)     2352 2024-06-03 02:03:02.000000 workercontext-0.1.1/tests/test_reduction.py
```

### Comparing `workercontext-0.1.0/LICENSE` & `workercontext-0.1.1/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Owen Elliott
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2023 Owen Elliott
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `workercontext-0.1.0/PKG-INFO` & `workercontext-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,225 +1,225 @@
-Metadata-Version: 2.1
-Name: workercontext
-Version: 0.1.0
-Summary: A small package that provides a context to spin up multiple workers to execute a function
-Author-email: Owen Elliott <none@none.com>
-License: MIT License
-        
-        Copyright (c) 2023 Owen Elliott
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-Project-URL: Homepage, https://github.com/OwenPendrighElliott/MultiWorker
-Project-URL: Bug Tracker, https://github.com/OwenPendrighElliott/MultiWorker/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Multi-Worker Context
-
-[![test](https://github.com/owenpendrighelliott/MultiWorker/actions/workflows/test.yml/badge.svg)](https://github.com/owenpendrighelliott/MultiWorker/actions/workflows/test.yml)
-
-
-This is a small project that create a context in python which can spin up multiple workers to do a task.
-
-The only requirement is that a the function you want to give multiple workers to has only one argument that you would like to batch on. It is up to you to ensure that creating independant batches for multiple workers makes sense with this argument.
-
-This makes refactoring code for multiprocessing a lot easier and should provide quick performance wins for time consuming functions with no interdependencies between elements.
-
-## Setup
-
-```
-pip install workercontext
-```
-
-## Example
-
-By default the work distribution will occur on the first parameter to the function.
-
-Take the following function:
-
-```python
-from typing import List
-
-def my_func(arr: List[int]) -> List[int]:
-    return [el*2 for el in arr]
-```
-
-This can be simply split across multiple workers as follows:
-
-```python
-from workercontext import MultiWorker
-
-arr = list(range(100))
-
-with MultiWorker(my_func, n_processes=8) as f:
-    res = f(arr)
-print(res)
-```
-
-`res` will be a list of lists of `ints` in this case, if you would like to reduce across all workers then you can pass a reduction:
-
-```python
-from workercontext import MultiWorker
-from workercontext.reductions import flatten_reduction
-
-arr = list(range(100))
-
-with MultiWorker(my_func, n_processes=8, reduction=flatten_reduction) as f:
-    res = f(arr)
-print(res)
-```
-
-`res` will now a list of `int`.
-
-You can also parallelise functions without using the context manager:
-
-```python
-from workercontext import parallelise
-
-arr = list(range(100))
-
-res = parallelise(my_func, n_processes=8)(arr) # res is list of list of int
-```
-
-If you have type hints on your function then auto parallelise will guess the reduction to apply as well:
-
-```python
-from workercontext import auto_parallelise
-
-arr = list(range(100))
-
-res = auto_parallelise(my_func)(arr) # res is list of int
-```
-
-If you wanted to combine multiple reductions then you can use the reduction composition class
-
-```python
-from workercontext import MultiWorker
-from workercontext.reductions import ReductionComposition, flatten_reduction, average_reduction
-
-reductions = ReductionComposition([flatten_reduction, average_reduction])
-
-with MultiWorker(my_func, n_processes=8, reduction=reductions) as f:
-    res = f(arr)
-print(res)
-```
-
-This makes res be a single `float`.
-
-### Using other parameters
-
-You can batch work on other parameters by specifying them in the constructor.
-
-```python
-from workercontext import MultiWorker
-from workercontext.reductions import flatten_reduction
-
-def my_func(l1: List[int], l2: List[int]) -> int:
-    for i in range(len(l2)):
-        for el1 in l1:
-            l2[i] += el1
-    return l2
-
-arr1 = list(range(100))
-arr2 = list(range(100))
-
-with MultiWorker(my_func, batched_arg='l2', n_processes=8, reduction=flatten_reduction) as f:
-    res = f(arr1, arr2)
-print(res)
-```
-
-## Async MultiWorker
-
-There is also an asynchroneous version of the MultiWorker context that does the processing async (non-blocking). You can either have it be async or have it converge when the context is exited.
-
-```python
-from workercontext import MultiWorkerAsync
-
-arr = list(range(100))
-
-res = [] # this is where the result will go
-
-with MultiWorkerAsync(my_func, n_processes=8, return_container=res) as f:
-    f(arr)
-    # do other things
-
-print(res) # res is gaurenteed to be populated AFTER context is exited
-```
-
-Or you can have no blocking by not specify a return container:
-
-```python
-from workercontext import MultiWorkerAsync, parallelise_async
-
-arr = list(range(100))
-
-# as a context 
-with MultiWorkerAsync(my_func, n_processes=8) as f:
-    f(arr)
-
-# or as a function
-parallelise_async(my_func, n_processes=8)(arr)
-```
-
-# Documentation
-
-## MultiWorker
-### parameters
-+ `function` (`Callable`): The function to create the context for.
-+ `n_processes` (`int`): The number of processes to spawn.
-+ `batched_arg` (`str`, `optional`): The argument to batch on, if None the the first arg is used. Defaults to None.
-+ `verbose` (`bool`, `optional`): Whether or not to print information about the processing. Defaults to False.
-+ `reduction` (`Callable[[List[Any]], Any]`, `optional`): A reduction function to be applied across the outputs of the pool. Defaults to None.
-## Supported Reductions
-+ `flatten_reduction`
-+ `histogram_reduction`
-+ `product_reduction`
-+ `string concatenation_reduction`
-+ `bitwise and_reduction`
-+ `bitwise or_reduction`
-+ `min_reduction`
-+ `max_reduction`
-
-## Testing
-```
-pytest
-```
-
-## Formatting
-```
-black .
-```
-
-## How it works
-
-TL;DR it does a bunch of introspection.
-
-1. The args to your function are introspected.
-2. The `self` arg is remove if you passed it a method from a class.
-3. If no batched arg was specified then the first one is selected.
-4. All args are converted into kwargs using the introspected arg names and the `*args` provided.
-5. The size of the batched arg is calculated and the chunk sizes are derived.
-6. The arg is batched and batches of kwargs are created.
-7. A pool is created with a partial for a wrapper function that allows for the batching to occur on the kwargs. The last parameter to the wrapper is a callback to your function.
-8. A reduction is applied (if specified)
-9. Results are returned.
-10. When you leave the context the pools are joined and closed.
+Metadata-Version: 2.1
+Name: workercontext
+Version: 0.1.1
+Summary: A small package that provides a context to spin up multiple workers to execute a function
+Author-email: Owen Elliott <none@none.com>
+License: MIT License
+        
+        Copyright (c) 2023 Owen Elliott
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+Project-URL: Homepage, https://github.com/OwenPendrighElliott/MultiWorker
+Project-URL: Bug Tracker, https://github.com/OwenPendrighElliott/MultiWorker/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Multi-Worker Context
+
+[![test](https://github.com/owenpendrighelliott/MultiWorker/actions/workflows/test.yml/badge.svg)](https://github.com/owenpendrighelliott/MultiWorker/actions/workflows/test.yml)
+
+
+This is a small project that create a context in python which can spin up multiple workers to do a task.
+
+The only requirement is that a the function you want to give multiple workers to has only one argument that you would like to batch on. It is up to you to ensure that creating independant batches for multiple workers makes sense with this argument.
+
+This makes refactoring code for multiprocessing a lot easier and should provide quick performance wins for time consuming functions with no interdependencies between elements.
+
+## Setup
+
+```
+pip install workercontext
+```
+
+## Example
+
+By default the work distribution will occur on the first parameter to the function.
+
+Take the following function:
+
+```python
+from typing import List
+
+def my_func(arr: List[int]) -> List[int]:
+    return [el*2 for el in arr]
+```
+
+This can be simply split across multiple workers as follows:
+
+```python
+from workercontext import MultiWorker
+
+arr = list(range(100))
+
+with MultiWorker(my_func, n_processes=8) as f:
+    res = f(arr)
+print(res)
+```
+
+`res` will be a list of lists of `ints` in this case, if you would like to reduce across all workers then you can pass a reduction:
+
+```python
+from workercontext import MultiWorker
+from workercontext.reductions import flatten_reduction
+
+arr = list(range(100))
+
+with MultiWorker(my_func, n_processes=8, reduction=flatten_reduction) as f:
+    res = f(arr)
+print(res)
+```
+
+`res` will now a list of `int`.
+
+You can also parallelise functions without using the context manager:
+
+```python
+from workercontext import parallelise
+
+arr = list(range(100))
+
+res = parallelise(my_func, n_processes=8)(arr) # res is list of list of int
+```
+
+If you have type hints on your function then auto parallelise will guess the reduction to apply as well:
+
+```python
+from workercontext import auto_parallelise
+
+arr = list(range(100))
+
+res = auto_parallelise(my_func)(arr) # res is list of int
+```
+
+If you wanted to combine multiple reductions then you can use the reduction composition class
+
+```python
+from workercontext import MultiWorker
+from workercontext.reductions import ReductionComposition, flatten_reduction, average_reduction
+
+reductions = ReductionComposition([flatten_reduction, average_reduction])
+
+with MultiWorker(my_func, n_processes=8, reduction=reductions) as f:
+    res = f(arr)
+print(res)
+```
+
+This makes res be a single `float`.
+
+### Using other parameters
+
+You can batch work on other parameters by specifying them in the constructor.
+
+```python
+from workercontext import MultiWorker
+from workercontext.reductions import flatten_reduction
+
+def my_func(l1: List[int], l2: List[int]) -> int:
+    for i in range(len(l2)):
+        for el1 in l1:
+            l2[i] += el1
+    return l2
+
+arr1 = list(range(100))
+arr2 = list(range(100))
+
+with MultiWorker(my_func, batched_arg='l2', n_processes=8, reduction=flatten_reduction) as f:
+    res = f(arr1, arr2)
+print(res)
+```
+
+## Async MultiWorker
+
+There is also an asynchroneous version of the MultiWorker context that does the processing async (non-blocking). You can either have it be async or have it converge when the context is exited.
+
+```python
+from workercontext import MultiWorkerAsync
+
+arr = list(range(100))
+
+res = [] # this is where the result will go
+
+with MultiWorkerAsync(my_func, n_processes=8, return_container=res) as f:
+    f(arr)
+    # do other things
+
+print(res) # res is gaurenteed to be populated AFTER context is exited
+```
+
+Or you can have no blocking by not specify a return container:
+
+```python
+from workercontext import MultiWorkerAsync, parallelise_async
+
+arr = list(range(100))
+
+# as a context 
+with MultiWorkerAsync(my_func, n_processes=8) as f:
+    f(arr)
+
+# or as a function
+parallelise_async(my_func, n_processes=8)(arr)
+```
+
+# Documentation
+
+## MultiWorker
+### parameters
++ `function` (`Callable`): The function to create the context for.
++ `n_processes` (`int`): The number of processes to spawn.
++ `batched_arg` (`str`, `optional`): The argument to batch on, if None the the first arg is used. Defaults to None.
++ `verbose` (`bool`, `optional`): Whether or not to print information about the processing. Defaults to False.
++ `reduction` (`Callable[[List[Any]], Any]`, `optional`): A reduction function to be applied across the outputs of the pool. Defaults to None.
+## Supported Reductions
++ `flatten_reduction`
++ `histogram_reduction`
++ `product_reduction`
++ `string concatenation_reduction`
++ `bitwise and_reduction`
++ `bitwise or_reduction`
++ `min_reduction`
++ `max_reduction`
+
+## Testing
+```
+pytest
+```
+
+## Formatting
+```
+black .
+```
+
+## How it works
+
+TL;DR it does a bunch of introspection.
+
+1. The args to your function are introspected.
+2. The `self` arg is remove if you passed it a method from a class.
+3. If no batched arg was specified then the first one is selected.
+4. All args are converted into kwargs using the introspected arg names and the `*args` provided.
+5. The size of the batched arg is calculated and the chunk sizes are derived.
+6. The arg is batched and batches of kwargs are created.
+7. A pool is created with a partial for a wrapper function that allows for the batching to occur on the kwargs. The last parameter to the wrapper is a callback to your function.
+8. A reduction is applied (if specified)
+9. Results are returned.
+10. When you leave the context the pools are joined and closed.
```

### Comparing `workercontext-0.1.0/pyproject.toml` & `workercontext-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-[project]
-name = "workercontext"
-version = "0.1.0"
-description = "A small package that provides a context to spin up multiple workers to execute a function"
-readme = "README.md"
-authors = [
-  { name = "Owen Elliott", email = "none@none.com" },
-]
-license = { file = "LICENSE" }
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-requires-python = ">=3.7"
-dependencies = []
-
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-[project.urls]
-"Homepage" = "https://github.com/OwenPendrighElliott/MultiWorker"
+[project]
+name = "workercontext"
+version = "0.1.1"
+description = "A small package that provides a context to spin up multiple workers to execute a function"
+readme = "README.md"
+authors = [
+  { name = "Owen Elliott", email = "none@none.com" },
+]
+license = { file = "LICENSE" }
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+requires-python = ">=3.7"
+dependencies = []
+
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+[project.urls]
+"Homepage" = "https://github.com/OwenPendrighElliott/MultiWorker"
 "Bug Tracker" = "https://github.com/OwenPendrighElliott/MultiWorker/issues"
```

### Comparing `workercontext-0.1.0/src/workercontext/multiworker.py` & `workercontext-0.1.1/src/workercontext/multiworker.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,303 +1,309 @@
-import multiprocessing
-from functools import partial
-import inspect
-from .reductions import (
-    flatten_reduction,
-    set_union_reduction,
-    dict_merge_reduction,
-    string_concatenation_reduction,
-)
-from typing import List, Any, Callable, Union
-
-
-def _worker(kwargs, function: Callable) -> Any:
-    """Helper to wrap a function for multiprocessing"""
-    return function(**kwargs)
-
-
-class MultiWorker:
-    def __init__(
-        self,
-        function: Callable,
-        n_processes: int,
-        batched_arg: str = None,
-        verbose: bool = False,
-        reduction: Callable[[List[Any]], Any] = None,
-    ):
-        """Create a multiprocessing context for functions
-
-        Args:
-            function (Callable): The function to create the context for.
-            n_processes (int): The number of processes to spawn.
-            batched_arg (str, optional): The argument to batch on, if None the the first arg is used. Defaults to None.
-            verbose (bool, optional): Whether or not to print information about the processing. Defaults to False.
-            reduction (Callable[[List[Any]], Any], optional): A reduction function to be applied across the outputs of the pool. Defaults to None.
-        """
-        self.function = function
-        self.batched_arg = batched_arg
-        self.n_processes = n_processes
-        self._verbose = verbose
-        self._reduction = reduction
-        self.pool = multiprocessing.Pool(self.n_processes)
-
-    def batchify(self, lst, chunk_size):
-        return [lst[i : i + chunk_size] for i in range(0, len(lst), chunk_size)]
-
-    def _batched_args(self, *args, **kwargs) -> List[Any]:
-        """Wrap any function in this batched version, converts all args into kwargs using introspection
-
-        Raises:
-            ValueError: If the batched args are not a list
-
-        Returns:
-            List[Any]: A list of outputs from each batch, ordered.
-        """
-
-        # Introspect the args to the function
-        argspec = inspect.getfullargspec(self.function)
-        func_args = argspec.args
-
-        annotations = argspec.annotations
-
-        # if the first arg is self then drop it because it is provided by its class
-        if func_args[0] == "self":
-            func_args = func_args[1:]
-
-        # if no batched arg is specified then try to determine it from the type hints or fall back to the first arg
-        if not self.batched_arg:
-            all_typed = all([arg in annotations for arg in func_args])
-            if not all_typed:
-                if self._verbose:
-                    print(
-                        f"No batched arg specified and not all args are typed, defaulting to first arg: {func_args[0]}"
-                    )
-                self.batched_arg = func_args[0]
-            else:
-                for arg in func_args:
-                    arg_type = annotations[arg]
-                    if isinstance(arg_type, list) or (
-                        hasattr(arg_type, "__origin__") and arg_type.__origin__ == list
-                    ):
-                        self.batched_arg = arg
-                        if self._verbose:
-                            print(
-                                f"Using argument type hints, automatically determined batched arg: {arg}"
-                            )
-                        break
-
-        # convert all args to kwargs using introspected args
-        for i, arg in enumerate(args):
-            kwargs[func_args[i]] = arg
-
-        if not isinstance(kwargs[self.batched_arg], list):
-            raise ValueError(
-                f"Batched arg {self.batched_arg} must be an instance of list"
-            )
-
-        # get size of batched arg
-        arg_size = len(kwargs[self.batched_arg])
-
-        processes_to_use = min(self.n_processes, arg_size)
-
-        if self._verbose:
-            print(
-                f"Executing {self.function.__name__} with {processes_to_use} workers evenly distributing work on parameter '{self.batched_arg}'"
-            )
-
-        # calculate chunksize
-        chunk_size = arg_size // processes_to_use
-
-        if self._verbose:
-            print(f"Workers will be assigned chunks of size {chunk_size}")
-
-        # convert the batched arg into batches
-        kwargs[self.batched_arg] = self.batchify(
-            kwargs[self.batched_arg], chunk_size=chunk_size
-        )
-
-        # create a list of kwargs with each batched_arg arg having a single batch
-        batched_args = []
-        for batch in kwargs[self.batched_arg]:
-            new_args = dict(kwargs)
-            new_args[self.batched_arg] = batch
-            batched_args.append(new_args)
-        return batched_args
-
-    def _batched_function(self, *args, **kwargs) -> List[Any]:
-        batched_args = self._batched_args(*args, **kwargs)
-
-        # create a pool - the function is wrapped up in a worker so we can pool on all args
-        func_outputs = self.pool.map(
-            partial(_worker, function=self.function), batched_args
-        )
-
-        if self._reduction:
-            func_outputs = self._reduction(func_outputs)
-
-        return func_outputs
-
-    def __enter__(self) -> Callable:
-        """Creates a temporary multiprocessing context for a function
-
-        Returns:
-            Callable: Return a batched version of the function with multiprocessing
-        """
-        return self._batched_function
-
-    def __exit__(self, exc_type, exc_val, exc_tb) -> None:
-        """Close the pool when done"""
-        self.pool.close()
-        self.pool.join()
-
-
-class MultiWorkerAsync(MultiWorker):
-    """
-    A special case of the MultiWorker that uses map_async instead of map to allow for async processing of the pool
-
-    This allows for async processing within the context and a gaurentee that at the end the end of the context
-    results will populate the return container
-    """
-
-    def __init__(
-        self,
-        function: Callable,
-        n_processes: int,
-        batched_arg: str = None,
-        verbose: bool = False,
-        return_container: list = None,
-    ):
-        super().__init__(function, n_processes, batched_arg, verbose, None)
-
-        self.func_outputs = None
-        self.return_container = return_container
-
-    def _batched_function(self, *args, **kwargs) -> None:
-        batched_args = self._batched_args(*args, **kwargs)
-
-        self.func_outputs = self.pool.map_async(
-            partial(_worker, function=self.function), batched_args
-        )
-
-    def __enter__(self) -> Callable:
-        """Creates a temporary multiprocessing context for a function
-
-        Returns:
-            Callable: Return a batched version of the function with multiprocessing
-        """
-        return self._batched_function
-
-    def __exit__(self, exc_type, exc_val, exc_tb) -> None:
-        """Close the pool when done and populate the return container if it is provided"""
-        results = self.func_outputs.get()
-        if self.return_container is not None:
-            for result in results:
-                self.return_container.append(result)
-
-        self.pool.close()
-        self.pool.join()
-
-
-def parallelise(
-    function: Callable,
-    n_processes: int,
-    batched_arg: str = None,
-    verbose: bool = False,
-    reduction: Callable[[List[Any]], Any] = None,
-) -> Callable:
-    """Parallelise a function without a context manager
-
-    Args:
-        function (Callable): The function to parallelise
-        n_processes (int): The number of processes to use
-        batched_arg (str, optional): The argument to batch on. Defaults to None.
-        verbose (bool, optional): Toggle verbose printing. Defaults to False.
-        reduction (Callable[[List[Any]], Any], optional): Reduction to apply to the output. Defaults to None.
-
-    Returns:
-        Callable: A parallelised function
-    """
-    return MultiWorker(
-        function, n_processes, batched_arg, verbose, reduction
-    ).__enter__()
-
-
-def auto_parallelise(
-    function: Callable,
-) -> Callable:
-    """Automatically parallelise a function based on type hints. Works like
-    parallelise but automatically determines the return type and applies a reduction if possible.
-
-    Args:
-        function (Callable): The function to parallelise
-
-    Raises:
-        ValueError: raised if the function has no type hints
-        ValueError: raised if the function has no return type hint
-
-    Returns:
-        Callable: a parallelised function
-    """
-
-    # automatically use the same number of processes as the number of cpus
-    n_processes = multiprocessing.cpu_count()
-
-    # introspect the function to determine the return type
-    argspec = inspect.getfullargspec(function)
-    if not argspec.annotations:
-        raise ValueError("Function must have type hints to use auto_parallelise")
-
-    annotations = argspec.annotations
-
-    if "return" not in annotations:
-        raise ValueError(
-            "Function must have a return type hint to use auto_parallelise"
-        )
-
-    return_type = annotations["return"]
-    print(f"Return type is annotated as {return_type}")
-
-    return_module = return_type.__module__
-
-    if return_module == "typing":
-        return_type = return_type.__origin__
-
-    reduction = None
-    if return_type == list:
-        reduction = flatten_reduction
-        print(
-            "Lists from each worker will be flattened into a single list with order preserved"
-        )
-    elif return_type == set:
-        reduction = set_union_reduction
-        print("Sets from each worker will be unioned into a single set")
-    elif return_type == dict:
-        reduction = dict_merge_reduction
-        print("Dictionaries from each worker will be merged into a single dictionary")
-    elif return_type == str:
-        reduction = string_concatenation_reduction
-        print(
-            "Strings from each worker will be concatenated into a single string with order preserved"
-        )
-    else:
-        print(
-            f"No reduction will be applied to the return type as we don't automatically know a smart thing to do for {return_type}"
-        )
-
-    return parallelise(function, n_processes, verbose=True, reduction=reduction)
-
-
-def parallelise_async(
-    function: Callable, n_processes: int, batched_arg: str = None, verbose: bool = False
-) -> Callable:
-    """Create an async parallelised function
-
-    Args:
-        function (Callable): The function to parallelise
-        n_processes (int): The number of processes to use
-        batched_arg (str, optional): The argument to batch on. Defaults to None.
-        verbose (bool, optional): Toggle verbose logging. Defaults to False.
-
-    Returns:
-        Callable: A parallelised function
-    """
-    return MultiWorkerAsync(function, n_processes, batched_arg, verbose).__enter__()
+import multiprocessing
+from functools import partial
+import inspect
+from .reductions import (
+    flatten_reduction,
+    set_union_reduction,
+    dict_merge_reduction,
+    string_concatenation_reduction,
+)
+from typing import List, Any, Callable, Union
+
+
+def _worker(kwargs, function: Callable) -> Any:
+    """Helper to wrap a function for multiprocessing"""
+    return function(**kwargs)
+
+
+class MultiWorker:
+    def __init__(
+        self,
+        function: Callable,
+        n_processes: int,
+        batched_arg: str = None,
+        verbose: bool = False,
+        reduction: Callable[[List[Any]], Any] = None,
+    ):
+        """Create a multiprocessing context for functions
+
+        Args:
+            function (Callable): The function to create the context for.
+            n_processes (int): The number of processes to spawn.
+            batched_arg (str, optional): The argument to batch on, if None the the first arg is used. Defaults to None.
+            verbose (bool, optional): Whether or not to print information about the processing. Defaults to False.
+            reduction (Callable[[List[Any]], Any], optional): A reduction function to be applied across the outputs of the pool. Defaults to None.
+        """
+        self.function = function
+        self.batched_arg = batched_arg
+        self.n_processes = n_processes
+        self._verbose = verbose
+        self._reduction = reduction
+        self.pool = multiprocessing.Pool(self.n_processes)
+
+    def batchify(self, lst, chunk_size):
+        return [lst[i : i + chunk_size] for i in range(0, len(lst), chunk_size)]
+
+    def _batched_args(self, *args, **kwargs) -> List[Any]:
+        """Wrap any function in this batched version, converts all args into kwargs using introspection
+
+        Raises:
+            ValueError: If the batched args are not a list
+
+        Returns:
+            List[Any]: A list of outputs from each batch, ordered.
+        """
+
+        # Introspect the args to the function
+        argspec = inspect.getfullargspec(self.function)
+        func_args = argspec.args
+
+        annotations = argspec.annotations
+
+        # if the first arg is self then drop it because it is provided by its class
+        if func_args[0] == "self":
+            func_args = func_args[1:]
+
+        # if no batched arg is specified then try to determine it from the type hints or fall back to the first arg
+        if not self.batched_arg:
+            all_typed = all([arg in annotations for arg in func_args])
+            if not all_typed:
+                if self._verbose:
+                    print(
+                        f"No batched arg specified and not all args are typed, defaulting to first arg: {func_args[0]}"
+                    )
+                self.batched_arg = func_args[0]
+            else:
+                for arg in func_args:
+                    arg_type = annotations[arg]
+                    if isinstance(arg_type, list) or (
+                        hasattr(arg_type, "__origin__") and arg_type.__origin__ == list
+                    ):
+                        self.batched_arg = arg
+                        if self._verbose:
+                            print(
+                                f"Using argument type hints, automatically determined batched arg: {arg}"
+                            )
+                        break
+
+                # if we still don't have a batched arg then raise an error
+                if not self.batched_arg:
+                    raise ValueError(
+                        "No batched arg specified and no args are typed as lists, please specify a batched arg or check your type hints are correct"
+                    )
+
+        # convert all args to kwargs using introspected args
+        for i, arg in enumerate(args):
+            kwargs[func_args[i]] = arg
+
+        if not isinstance(kwargs[self.batched_arg], list):
+            raise ValueError(
+                f"Batched arg {self.batched_arg} must be an instance of list"
+            )
+
+        # get size of batched arg
+        arg_size = len(kwargs[self.batched_arg])
+
+        processes_to_use = min(self.n_processes, arg_size)
+
+        if self._verbose:
+            print(
+                f"Executing {self.function.__name__} with {processes_to_use} workers evenly distributing work on parameter '{self.batched_arg}'"
+            )
+
+        # calculate chunksize
+        chunk_size = arg_size // processes_to_use
+
+        if self._verbose:
+            print(f"Workers will be assigned chunks of size {chunk_size}")
+
+        # convert the batched arg into batches
+        kwargs[self.batched_arg] = self.batchify(
+            kwargs[self.batched_arg], chunk_size=chunk_size
+        )
+
+        # create a list of kwargs with each batched_arg arg having a single batch
+        batched_args = []
+        for batch in kwargs[self.batched_arg]:
+            new_args = dict(kwargs)
+            new_args[self.batched_arg] = batch
+            batched_args.append(new_args)
+        return batched_args
+
+    def _batched_function(self, *args, **kwargs) -> List[Any]:
+        batched_args = self._batched_args(*args, **kwargs)
+
+        # create a pool - the function is wrapped up in a worker so we can pool on all args
+        func_outputs = self.pool.map(
+            partial(_worker, function=self.function), batched_args
+        )
+
+        if self._reduction:
+            func_outputs = self._reduction(func_outputs)
+
+        return func_outputs
+
+    def __enter__(self) -> Callable:
+        """Creates a temporary multiprocessing context for a function
+
+        Returns:
+            Callable: Return a batched version of the function with multiprocessing
+        """
+        return self._batched_function
+
+    def __exit__(self, exc_type, exc_val, exc_tb) -> None:
+        """Close the pool when done"""
+        self.pool.close()
+        self.pool.join()
+
+
+class MultiWorkerAsync(MultiWorker):
+    """
+    A special case of the MultiWorker that uses map_async instead of map to allow for async processing of the pool
+
+    This allows for async processing within the context and a gaurentee that at the end the end of the context
+    results will populate the return container
+    """
+
+    def __init__(
+        self,
+        function: Callable,
+        n_processes: int,
+        batched_arg: str = None,
+        verbose: bool = False,
+        return_container: list = None,
+    ):
+        super().__init__(function, n_processes, batched_arg, verbose, None)
+
+        self.func_outputs = None
+        self.return_container = return_container
+
+    def _batched_function(self, *args, **kwargs) -> None:
+        batched_args = self._batched_args(*args, **kwargs)
+
+        self.func_outputs = self.pool.map_async(
+            partial(_worker, function=self.function), batched_args
+        )
+
+    def __enter__(self) -> Callable:
+        """Creates a temporary multiprocessing context for a function
+
+        Returns:
+            Callable: Return a batched version of the function with multiprocessing
+        """
+        return self._batched_function
+
+    def __exit__(self, exc_type, exc_val, exc_tb) -> None:
+        """Close the pool when done and populate the return container if it is provided"""
+        results = self.func_outputs.get()
+        if self.return_container is not None:
+            for result in results:
+                self.return_container.append(result)
+
+        self.pool.close()
+        self.pool.join()
+
+
+def parallelise(
+    function: Callable,
+    n_processes: int,
+    batched_arg: str = None,
+    verbose: bool = False,
+    reduction: Callable[[List[Any]], Any] = None,
+) -> Callable:
+    """Parallelise a function without a context manager
+
+    Args:
+        function (Callable): The function to parallelise
+        n_processes (int): The number of processes to use
+        batched_arg (str, optional): The argument to batch on. Defaults to None.
+        verbose (bool, optional): Toggle verbose printing. Defaults to False.
+        reduction (Callable[[List[Any]], Any], optional): Reduction to apply to the output. Defaults to None.
+
+    Returns:
+        Callable: A parallelised function
+    """
+    return MultiWorker(
+        function, n_processes, batched_arg, verbose, reduction
+    ).__enter__()
+
+
+def auto_parallelise(
+    function: Callable,
+) -> Callable:
+    """Automatically parallelise a function based on type hints. Works like
+    parallelise but automatically determines the return type and applies a reduction if possible.
+
+    Args:
+        function (Callable): The function to parallelise
+
+    Raises:
+        ValueError: raised if the function has no type hints
+        ValueError: raised if the function has no return type hint
+
+    Returns:
+        Callable: a parallelised function
+    """
+
+    # automatically use the same number of processes as the number of cpus
+    n_processes = multiprocessing.cpu_count()
+
+    # introspect the function to determine the return type
+    argspec = inspect.getfullargspec(function)
+    if not argspec.annotations:
+        raise ValueError("Function must have type hints to use auto_parallelise")
+
+    annotations = argspec.annotations
+
+    if "return" not in annotations:
+        raise ValueError(
+            "Function must have a return type hint to use auto_parallelise"
+        )
+
+    return_type = annotations["return"]
+    print(f"Return type is annotated as {return_type}")
+
+    return_module = return_type.__module__
+
+    if return_module == "typing":
+        return_type = return_type.__origin__
+
+    reduction = None
+    if return_type == list:
+        reduction = flatten_reduction
+        print(
+            "Lists from each worker will be flattened into a single list with order preserved"
+        )
+    elif return_type == set:
+        reduction = set_union_reduction
+        print("Sets from each worker will be unioned into a single set")
+    elif return_type == dict:
+        reduction = dict_merge_reduction
+        print("Dictionaries from each worker will be merged into a single dictionary")
+    elif return_type == str:
+        reduction = string_concatenation_reduction
+        print(
+            "Strings from each worker will be concatenated into a single string with order preserved"
+        )
+    else:
+        print(
+            f"No reduction will be applied to the return type as we don't automatically know a smart thing to do for {return_type}"
+        )
+
+    return parallelise(function, n_processes, verbose=True, reduction=reduction)
+
+
+def parallelise_async(
+    function: Callable, n_processes: int, batched_arg: str = None, verbose: bool = False
+) -> Callable:
+    """Create an async parallelised function
+
+    Args:
+        function (Callable): The function to parallelise
+        n_processes (int): The number of processes to use
+        batched_arg (str, optional): The argument to batch on. Defaults to None.
+        verbose (bool, optional): Toggle verbose logging. Defaults to False.
+
+    Returns:
+        Callable: A parallelised function
+    """
+    return MultiWorkerAsync(function, n_processes, batched_arg, verbose).__enter__()
```

### Comparing `workercontext-0.1.0/src/workercontext/reductions.py` & `workercontext-0.1.1/src/workercontext/reductions.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,200 +1,200 @@
-from typing import List, Set, Dict, Union, Callable, Any
-
-
-class ReductionComposition:
-    """Compose multiple reductions into a pipeline"""
-
-    def __init__(self, reductions: List[Callable] = []):
-        self._reductions = reductions
-
-    def __call__(self, arg: Any) -> Any:
-        """Execute the reduction pipeline
-
-        Args:
-            arg (Any): The arg to reduce.
-
-        Returns:
-            Any: The output of the last reduction.
-        """
-        for reduction in self._reductions:
-            print(arg)
-            arg = reduction(arg)
-        return arg
-
-
-def flatten_reduction(lst: List[List[Any]]) -> List[Any]:
-    """
-    Flatten a list of lists into a single list.
-
-    Args:
-        lst (List[List[Any]]): A list of lists.
-
-    Returns:
-        List[Any]: A flattened list with the same ordering.
-    """
-    flattened = []
-    for sublist in lst:
-        flattened.extend(sublist)
-    return flattened
-
-
-def set_union_reduction(lst: List[Set[Any]]) -> Set[Any]:
-    """
-    Returns the union of all the sets in the input list.
-
-    Args:
-        lst (List[Set[Any]]): A list of sets.
-
-    Returns:
-        Set[Any]: The union of all the sets in the input list.
-    """
-    union = set()
-    for s in lst:
-        union |= s
-    return union
-
-
-def dict_merge_reduction(lst: List[Dict[Any, Any]]) -> Dict[Any, Any]:
-    """
-    Returns the merge of all the dictionaries in the input list.
-
-    Args:
-        lst (List[Dict[Any, Any]]): A list of dictionaries.
-
-    Returns:
-        Dict[Any, Any]: The merge of all the dictionaries in the input list.
-    """
-    merged = {}
-    for d in lst:
-        merged.update(d)
-    return merged
-
-
-def sum_reduction(arr: List[float]) -> float:
-    """
-    Returns the sum of all the elements in the input array.
-
-    Args:
-        arr (List[float]): A list of numbers.
-
-    Returns:
-        float: The sum of all the elements in the input array.
-    """
-    result = 0
-    for elem in arr:
-        result += elem
-    return result
-
-
-def average_reduction(lst: List[float]) -> float:
-    """
-    Average a list of numbers
-
-    Args:
-        lst (List[float]): A list of floats.
-
-    Returns:
-        float: Average.
-    """
-    return sum(lst) / len(lst)
-
-
-def histogram_reduction(arr: List[Union[int, str]]) -> Dict[Union[int, str], int]:
-    """Returns a dictionary containing the count of each unique element in the input array.
-
-    Args:
-        arr (List[int]): A list of integers.
-
-    Returns:
-        Dict[int, int]: A dictionary where keys are unique elements from the input array and values are their counts.
-    """
-    histogram = {}
-    for elem in arr:
-        if elem not in histogram:
-            histogram[elem] = 1
-        else:
-            histogram[elem] += 1
-    return histogram
-
-
-def product_reduction(arr: List[float]) -> float:
-    """Returns the product of all the elements in the input array.
-
-    Args:
-        arr (List[float]): A list of numbers.
-
-    Returns:
-        float: The product of all the elements in the input array.
-    """
-    result = 1
-    for elem in arr:
-        result *= elem
-    return result
-
-
-def string_concatenation_reduction(arr: List[str]) -> str:
-    """Returns the concatenation of all the strings in the input array.
-
-    Args:
-        arr (List[str]): A list of strings.
-
-    Returns:
-        str: The concatenation of all the strings in the input array.
-    """
-    return "".join(arr)
-
-
-def bitwise_and_reduction(arr: List[int]) -> int:
-    """Returns the bitwise AND of all the integers in the input array.
-
-    Args:
-        arr (List[int]): A list of integers.
-
-    Returns:
-        int: The bitwise AND of all the integers in the input array.
-    """
-    result = arr[0]
-    for elem in arr[1:]:
-        result &= elem
-    return result
-
-
-def bitwise_or_reduction(arr: List[int]) -> int:
-    """Returns the bitwise OR of all the integers in the input array.
-
-    Args:
-        arr (List[int]): A list of integers.
-
-    Returns:
-        int: The bitwise OR of all the integers in the input array.
-    """
-    result = arr[0]
-    for elem in arr[1:]:
-        result |= elem
-    return result
-
-
-def min_reduction(arr: List[float]) -> float:
-    """Returns the minimum of a result set.
-
-    Args:
-        arr (List[float]): A list of numbers.
-
-    Returns:
-        float: The mminimum.
-    """
-
-    return min(arr)
-
-
-def max_reduction(arr: List[float]) -> float:
-    """Returns the minimum of a result set.
-
-    Args:
-        arr (List[float]): A list of numbers.
-
-    Returns:
-        float: The mminimum.
-    """
-
-    return max(arr)
+from typing import List, Set, Dict, Union, Callable, Any
+
+
+class ReductionComposition:
+    """Compose multiple reductions into a pipeline"""
+
+    def __init__(self, reductions: List[Callable] = []):
+        self._reductions = reductions
+
+    def __call__(self, arg: Any) -> Any:
+        """Execute the reduction pipeline
+
+        Args:
+            arg (Any): The arg to reduce.
+
+        Returns:
+            Any: The output of the last reduction.
+        """
+        for reduction in self._reductions:
+            print(arg)
+            arg = reduction(arg)
+        return arg
+
+
+def flatten_reduction(lst: List[List[Any]]) -> List[Any]:
+    """
+    Flatten a list of lists into a single list.
+
+    Args:
+        lst (List[List[Any]]): A list of lists.
+
+    Returns:
+        List[Any]: A flattened list with the same ordering.
+    """
+    flattened = []
+    for sublist in lst:
+        flattened.extend(sublist)
+    return flattened
+
+
+def set_union_reduction(lst: List[Set[Any]]) -> Set[Any]:
+    """
+    Returns the union of all the sets in the input list.
+
+    Args:
+        lst (List[Set[Any]]): A list of sets.
+
+    Returns:
+        Set[Any]: The union of all the sets in the input list.
+    """
+    union = set()
+    for s in lst:
+        union |= s
+    return union
+
+
+def dict_merge_reduction(lst: List[Dict[Any, Any]]) -> Dict[Any, Any]:
+    """
+    Returns the merge of all the dictionaries in the input list.
+
+    Args:
+        lst (List[Dict[Any, Any]]): A list of dictionaries.
+
+    Returns:
+        Dict[Any, Any]: The merge of all the dictionaries in the input list.
+    """
+    merged = {}
+    for d in lst:
+        merged.update(d)
+    return merged
+
+
+def sum_reduction(arr: List[float]) -> float:
+    """
+    Returns the sum of all the elements in the input array.
+
+    Args:
+        arr (List[float]): A list of numbers.
+
+    Returns:
+        float: The sum of all the elements in the input array.
+    """
+    result = 0
+    for elem in arr:
+        result += elem
+    return result
+
+
+def average_reduction(lst: List[float]) -> float:
+    """
+    Average a list of numbers
+
+    Args:
+        lst (List[float]): A list of floats.
+
+    Returns:
+        float: Average.
+    """
+    return sum(lst) / len(lst)
+
+
+def histogram_reduction(arr: List[Union[int, str]]) -> Dict[Union[int, str], int]:
+    """Returns a dictionary containing the count of each unique element in the input array.
+
+    Args:
+        arr (List[int]): A list of integers.
+
+    Returns:
+        Dict[int, int]: A dictionary where keys are unique elements from the input array and values are their counts.
+    """
+    histogram = {}
+    for elem in arr:
+        if elem not in histogram:
+            histogram[elem] = 1
+        else:
+            histogram[elem] += 1
+    return histogram
+
+
+def product_reduction(arr: List[float]) -> float:
+    """Returns the product of all the elements in the input array.
+
+    Args:
+        arr (List[float]): A list of numbers.
+
+    Returns:
+        float: The product of all the elements in the input array.
+    """
+    result = 1
+    for elem in arr:
+        result *= elem
+    return result
+
+
+def string_concatenation_reduction(arr: List[str]) -> str:
+    """Returns the concatenation of all the strings in the input array.
+
+    Args:
+        arr (List[str]): A list of strings.
+
+    Returns:
+        str: The concatenation of all the strings in the input array.
+    """
+    return "".join(arr)
+
+
+def bitwise_and_reduction(arr: List[int]) -> int:
+    """Returns the bitwise AND of all the integers in the input array.
+
+    Args:
+        arr (List[int]): A list of integers.
+
+    Returns:
+        int: The bitwise AND of all the integers in the input array.
+    """
+    result = arr[0]
+    for elem in arr[1:]:
+        result &= elem
+    return result
+
+
+def bitwise_or_reduction(arr: List[int]) -> int:
+    """Returns the bitwise OR of all the integers in the input array.
+
+    Args:
+        arr (List[int]): A list of integers.
+
+    Returns:
+        int: The bitwise OR of all the integers in the input array.
+    """
+    result = arr[0]
+    for elem in arr[1:]:
+        result |= elem
+    return result
+
+
+def min_reduction(arr: List[float]) -> float:
+    """Returns the minimum of a result set.
+
+    Args:
+        arr (List[float]): A list of numbers.
+
+    Returns:
+        float: The mminimum.
+    """
+
+    return min(arr)
+
+
+def max_reduction(arr: List[float]) -> float:
+    """Returns the minimum of a result set.
+
+    Args:
+        arr (List[float]): A list of numbers.
+
+    Returns:
+        float: The mminimum.
+    """
+
+    return max(arr)
```

### Comparing `workercontext-0.1.0/src/workercontext.egg-info/PKG-INFO` & `workercontext-0.1.1/src/workercontext.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,225 +1,225 @@
-Metadata-Version: 2.1
-Name: workercontext
-Version: 0.1.0
-Summary: A small package that provides a context to spin up multiple workers to execute a function
-Author-email: Owen Elliott <none@none.com>
-License: MIT License
-        
-        Copyright (c) 2023 Owen Elliott
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-Project-URL: Homepage, https://github.com/OwenPendrighElliott/MultiWorker
-Project-URL: Bug Tracker, https://github.com/OwenPendrighElliott/MultiWorker/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Multi-Worker Context
-
-[![test](https://github.com/owenpendrighelliott/MultiWorker/actions/workflows/test.yml/badge.svg)](https://github.com/owenpendrighelliott/MultiWorker/actions/workflows/test.yml)
-
-
-This is a small project that create a context in python which can spin up multiple workers to do a task.
-
-The only requirement is that a the function you want to give multiple workers to has only one argument that you would like to batch on. It is up to you to ensure that creating independant batches for multiple workers makes sense with this argument.
-
-This makes refactoring code for multiprocessing a lot easier and should provide quick performance wins for time consuming functions with no interdependencies between elements.
-
-## Setup
-
-```
-pip install workercontext
-```
-
-## Example
-
-By default the work distribution will occur on the first parameter to the function.
-
-Take the following function:
-
-```python
-from typing import List
-
-def my_func(arr: List[int]) -> List[int]:
-    return [el*2 for el in arr]
-```
-
-This can be simply split across multiple workers as follows:
-
-```python
-from workercontext import MultiWorker
-
-arr = list(range(100))
-
-with MultiWorker(my_func, n_processes=8) as f:
-    res = f(arr)
-print(res)
-```
-
-`res` will be a list of lists of `ints` in this case, if you would like to reduce across all workers then you can pass a reduction:
-
-```python
-from workercontext import MultiWorker
-from workercontext.reductions import flatten_reduction
-
-arr = list(range(100))
-
-with MultiWorker(my_func, n_processes=8, reduction=flatten_reduction) as f:
-    res = f(arr)
-print(res)
-```
-
-`res` will now a list of `int`.
-
-You can also parallelise functions without using the context manager:
-
-```python
-from workercontext import parallelise
-
-arr = list(range(100))
-
-res = parallelise(my_func, n_processes=8)(arr) # res is list of list of int
-```
-
-If you have type hints on your function then auto parallelise will guess the reduction to apply as well:
-
-```python
-from workercontext import auto_parallelise
-
-arr = list(range(100))
-
-res = auto_parallelise(my_func)(arr) # res is list of int
-```
-
-If you wanted to combine multiple reductions then you can use the reduction composition class
-
-```python
-from workercontext import MultiWorker
-from workercontext.reductions import ReductionComposition, flatten_reduction, average_reduction
-
-reductions = ReductionComposition([flatten_reduction, average_reduction])
-
-with MultiWorker(my_func, n_processes=8, reduction=reductions) as f:
-    res = f(arr)
-print(res)
-```
-
-This makes res be a single `float`.
-
-### Using other parameters
-
-You can batch work on other parameters by specifying them in the constructor.
-
-```python
-from workercontext import MultiWorker
-from workercontext.reductions import flatten_reduction
-
-def my_func(l1: List[int], l2: List[int]) -> int:
-    for i in range(len(l2)):
-        for el1 in l1:
-            l2[i] += el1
-    return l2
-
-arr1 = list(range(100))
-arr2 = list(range(100))
-
-with MultiWorker(my_func, batched_arg='l2', n_processes=8, reduction=flatten_reduction) as f:
-    res = f(arr1, arr2)
-print(res)
-```
-
-## Async MultiWorker
-
-There is also an asynchroneous version of the MultiWorker context that does the processing async (non-blocking). You can either have it be async or have it converge when the context is exited.
-
-```python
-from workercontext import MultiWorkerAsync
-
-arr = list(range(100))
-
-res = [] # this is where the result will go
-
-with MultiWorkerAsync(my_func, n_processes=8, return_container=res) as f:
-    f(arr)
-    # do other things
-
-print(res) # res is gaurenteed to be populated AFTER context is exited
-```
-
-Or you can have no blocking by not specify a return container:
-
-```python
-from workercontext import MultiWorkerAsync, parallelise_async
-
-arr = list(range(100))
-
-# as a context 
-with MultiWorkerAsync(my_func, n_processes=8) as f:
-    f(arr)
-
-# or as a function
-parallelise_async(my_func, n_processes=8)(arr)
-```
-
-# Documentation
-
-## MultiWorker
-### parameters
-+ `function` (`Callable`): The function to create the context for.
-+ `n_processes` (`int`): The number of processes to spawn.
-+ `batched_arg` (`str`, `optional`): The argument to batch on, if None the the first arg is used. Defaults to None.
-+ `verbose` (`bool`, `optional`): Whether or not to print information about the processing. Defaults to False.
-+ `reduction` (`Callable[[List[Any]], Any]`, `optional`): A reduction function to be applied across the outputs of the pool. Defaults to None.
-## Supported Reductions
-+ `flatten_reduction`
-+ `histogram_reduction`
-+ `product_reduction`
-+ `string concatenation_reduction`
-+ `bitwise and_reduction`
-+ `bitwise or_reduction`
-+ `min_reduction`
-+ `max_reduction`
-
-## Testing
-```
-pytest
-```
-
-## Formatting
-```
-black .
-```
-
-## How it works
-
-TL;DR it does a bunch of introspection.
-
-1. The args to your function are introspected.
-2. The `self` arg is remove if you passed it a method from a class.
-3. If no batched arg was specified then the first one is selected.
-4. All args are converted into kwargs using the introspected arg names and the `*args` provided.
-5. The size of the batched arg is calculated and the chunk sizes are derived.
-6. The arg is batched and batches of kwargs are created.
-7. A pool is created with a partial for a wrapper function that allows for the batching to occur on the kwargs. The last parameter to the wrapper is a callback to your function.
-8. A reduction is applied (if specified)
-9. Results are returned.
-10. When you leave the context the pools are joined and closed.
+Metadata-Version: 2.1
+Name: workercontext
+Version: 0.1.1
+Summary: A small package that provides a context to spin up multiple workers to execute a function
+Author-email: Owen Elliott <none@none.com>
+License: MIT License
+        
+        Copyright (c) 2023 Owen Elliott
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+Project-URL: Homepage, https://github.com/OwenPendrighElliott/MultiWorker
+Project-URL: Bug Tracker, https://github.com/OwenPendrighElliott/MultiWorker/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Multi-Worker Context
+
+[![test](https://github.com/owenpendrighelliott/MultiWorker/actions/workflows/test.yml/badge.svg)](https://github.com/owenpendrighelliott/MultiWorker/actions/workflows/test.yml)
+
+
+This is a small project that create a context in python which can spin up multiple workers to do a task.
+
+The only requirement is that a the function you want to give multiple workers to has only one argument that you would like to batch on. It is up to you to ensure that creating independant batches for multiple workers makes sense with this argument.
+
+This makes refactoring code for multiprocessing a lot easier and should provide quick performance wins for time consuming functions with no interdependencies between elements.
+
+## Setup
+
+```
+pip install workercontext
+```
+
+## Example
+
+By default the work distribution will occur on the first parameter to the function.
+
+Take the following function:
+
+```python
+from typing import List
+
+def my_func(arr: List[int]) -> List[int]:
+    return [el*2 for el in arr]
+```
+
+This can be simply split across multiple workers as follows:
+
+```python
+from workercontext import MultiWorker
+
+arr = list(range(100))
+
+with MultiWorker(my_func, n_processes=8) as f:
+    res = f(arr)
+print(res)
+```
+
+`res` will be a list of lists of `ints` in this case, if you would like to reduce across all workers then you can pass a reduction:
+
+```python
+from workercontext import MultiWorker
+from workercontext.reductions import flatten_reduction
+
+arr = list(range(100))
+
+with MultiWorker(my_func, n_processes=8, reduction=flatten_reduction) as f:
+    res = f(arr)
+print(res)
+```
+
+`res` will now a list of `int`.
+
+You can also parallelise functions without using the context manager:
+
+```python
+from workercontext import parallelise
+
+arr = list(range(100))
+
+res = parallelise(my_func, n_processes=8)(arr) # res is list of list of int
+```
+
+If you have type hints on your function then auto parallelise will guess the reduction to apply as well:
+
+```python
+from workercontext import auto_parallelise
+
+arr = list(range(100))
+
+res = auto_parallelise(my_func)(arr) # res is list of int
+```
+
+If you wanted to combine multiple reductions then you can use the reduction composition class
+
+```python
+from workercontext import MultiWorker
+from workercontext.reductions import ReductionComposition, flatten_reduction, average_reduction
+
+reductions = ReductionComposition([flatten_reduction, average_reduction])
+
+with MultiWorker(my_func, n_processes=8, reduction=reductions) as f:
+    res = f(arr)
+print(res)
+```
+
+This makes res be a single `float`.
+
+### Using other parameters
+
+You can batch work on other parameters by specifying them in the constructor.
+
+```python
+from workercontext import MultiWorker
+from workercontext.reductions import flatten_reduction
+
+def my_func(l1: List[int], l2: List[int]) -> int:
+    for i in range(len(l2)):
+        for el1 in l1:
+            l2[i] += el1
+    return l2
+
+arr1 = list(range(100))
+arr2 = list(range(100))
+
+with MultiWorker(my_func, batched_arg='l2', n_processes=8, reduction=flatten_reduction) as f:
+    res = f(arr1, arr2)
+print(res)
+```
+
+## Async MultiWorker
+
+There is also an asynchroneous version of the MultiWorker context that does the processing async (non-blocking). You can either have it be async or have it converge when the context is exited.
+
+```python
+from workercontext import MultiWorkerAsync
+
+arr = list(range(100))
+
+res = [] # this is where the result will go
+
+with MultiWorkerAsync(my_func, n_processes=8, return_container=res) as f:
+    f(arr)
+    # do other things
+
+print(res) # res is gaurenteed to be populated AFTER context is exited
+```
+
+Or you can have no blocking by not specify a return container:
+
+```python
+from workercontext import MultiWorkerAsync, parallelise_async
+
+arr = list(range(100))
+
+# as a context 
+with MultiWorkerAsync(my_func, n_processes=8) as f:
+    f(arr)
+
+# or as a function
+parallelise_async(my_func, n_processes=8)(arr)
+```
+
+# Documentation
+
+## MultiWorker
+### parameters
++ `function` (`Callable`): The function to create the context for.
++ `n_processes` (`int`): The number of processes to spawn.
++ `batched_arg` (`str`, `optional`): The argument to batch on, if None the the first arg is used. Defaults to None.
++ `verbose` (`bool`, `optional`): Whether or not to print information about the processing. Defaults to False.
++ `reduction` (`Callable[[List[Any]], Any]`, `optional`): A reduction function to be applied across the outputs of the pool. Defaults to None.
+## Supported Reductions
++ `flatten_reduction`
++ `histogram_reduction`
++ `product_reduction`
++ `string concatenation_reduction`
++ `bitwise and_reduction`
++ `bitwise or_reduction`
++ `min_reduction`
++ `max_reduction`
+
+## Testing
+```
+pytest
+```
+
+## Formatting
+```
+black .
+```
+
+## How it works
+
+TL;DR it does a bunch of introspection.
+
+1. The args to your function are introspected.
+2. The `self` arg is remove if you passed it a method from a class.
+3. If no batched arg was specified then the first one is selected.
+4. All args are converted into kwargs using the introspected arg names and the `*args` provided.
+5. The size of the batched arg is calculated and the chunk sizes are derived.
+6. The arg is batched and batches of kwargs are created.
+7. A pool is created with a partial for a wrapper function that allows for the batching to occur on the kwargs. The last parameter to the wrapper is a callback to your function.
+8. A reduction is applied (if specified)
+9. Results are returned.
+10. When you leave the context the pools are joined and closed.
```

### Comparing `workercontext-0.1.0/tests/test_performance.py` & `workercontext-0.1.1/tests/test_performance.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-from workercontext import MultiWorker
-import pytest
-from typing import List, Union
-import time
-
-
-@pytest.fixture
-def long_int_list():
-    return list(range(10_000_000))
-
-
-@pytest.fixture
-def long_str_list():
-    return [str(n) for n in range(10_000_000)]
-
-
-def busy_func(l: List[Union[str, int]]):
-    for el in l:
-        for i in range(10):
-            el *= i
-
-
-def test_busy_spd(long_int_list, long_str_list):
-    start_single = time.perf_counter()
-    busy_func(long_int_list)
-    end_single = time.perf_counter()
-
-    total_single = end_single - start_single
-
-    start_multi = time.perf_counter()
-    with MultiWorker(busy_func, 8) as f:
-        f(long_int_list)
-    end_multi = time.perf_counter()
-
-    total_multi = end_multi - start_multi
-
-    print(total_multi, total_single)
-    assert total_multi < total_single
-
-    start_single = time.perf_counter()
-    busy_func(long_str_list)
-    end_single = time.perf_counter()
-
-    total_single = end_single - start_single
-
-    start_multi = time.perf_counter()
-    with MultiWorker(busy_func, 8) as f:
-        f(long_str_list)
-    end_multi = time.perf_counter()
-
-    total_multi = end_multi - start_multi
-
-    print(total_multi, total_single)
-    assert total_multi < total_single
+from workercontext import MultiWorker
+import pytest
+from typing import List, Union
+import time
+
+
+@pytest.fixture
+def long_int_list():
+    return list(range(10_000_000))
+
+
+@pytest.fixture
+def long_str_list():
+    return [str(n) for n in range(10_000_000)]
+
+
+def busy_func(l: List[Union[str, int]]):
+    for el in l:
+        for i in range(10):
+            el *= i
+
+
+def test_busy_spd(long_int_list, long_str_list):
+    start_single = time.perf_counter()
+    busy_func(long_int_list)
+    end_single = time.perf_counter()
+
+    total_single = end_single - start_single
+
+    start_multi = time.perf_counter()
+    with MultiWorker(busy_func, 8) as f:
+        f(long_int_list)
+    end_multi = time.perf_counter()
+
+    total_multi = end_multi - start_multi
+
+    print(total_multi, total_single)
+    assert total_multi < total_single
+
+    start_single = time.perf_counter()
+    busy_func(long_str_list)
+    end_single = time.perf_counter()
+
+    total_single = end_single - start_single
+
+    start_multi = time.perf_counter()
+    with MultiWorker(busy_func, 8) as f:
+        f(long_str_list)
+    end_multi = time.perf_counter()
+
+    total_multi = end_multi - start_multi
+
+    print(total_multi, total_single)
+    assert total_multi < total_single
```

### Comparing `workercontext-0.1.0/tests/test_reduction.py` & `workercontext-0.1.1/tests/test_reduction.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,98 +1,98 @@
-from workercontext import MultiWorker
-from workercontext.reductions import (
-    ReductionComposition,
-    flatten_reduction,
-    sum_reduction,
-    average_reduction,
-    histogram_reduction,
-    product_reduction,
-    string_concatenation_reduction,
-    min_reduction,
-    max_reduction,
-)
-import pytest
-from typing import List
-
-
-@pytest.fixture
-def short_list():
-    return [1, 2, 3, 4, 5, 6, 7, 8]
-
-
-@pytest.fixture
-def short_str_list():
-    return ["Hello", "World", "I", "Am", "A", "String"]
-
-
-@pytest.fixture
-def duplicated_list():
-    return [1, 1, 1, 1, 2, 2, 2, 2]
-
-
-def list_return(l: List[int]) -> List[int]:
-    return [el * 2 for el in l]
-
-
-def concat(l: List[str]) -> str:
-    return "".join(l)
-
-
-def int_return(l: List[int]) -> List[int]:
-    return sum(l)
-
-
-def do_nothing(l: List[int]) -> List[int]:
-    return l
-
-
-def test_flatten(short_list):
-    with MultiWorker(list_return, 4, reduction=flatten_reduction) as f:
-        res = f(short_list)
-    assert res[0] == 2 and res[-1] == 16
-    assert len(res) == len(short_list)
-
-
-def test_sum(short_list):
-    with MultiWorker(int_return, 4, reduction=sum_reduction) as f:
-        res = f(short_list)
-    assert res == sum(short_list)
-
-
-def test_average(short_list):
-    reductions = ReductionComposition([flatten_reduction, average_reduction])
-    with MultiWorker(do_nothing, 4, reduction=reductions) as f:
-        res = f(short_list)
-    assert res == sum(short_list) / len(short_list)
-
-
-def test_histogram(duplicated_list):
-    with MultiWorker(int_return, 4, reduction=histogram_reduction) as f:
-        res = f(duplicated_list)
-    print(res)
-    assert res[2] == 2
-
-
-def test_min(short_list):
-    with MultiWorker(int_return, 4, reduction=min_reduction) as f:
-        res = f(short_list)
-    assert res == 3
-
-
-def test_max(short_list):
-    with MultiWorker(int_return, 4, reduction=max_reduction) as f:
-        res = f(short_list)
-    assert res == 15
-
-
-def test_composed(short_list):
-    reductions = ReductionComposition([flatten_reduction, product_reduction])
-
-    with MultiWorker(list_return, 4, reduction=reductions) as f:
-        res = f(short_list)
-    assert res == 10321920
-
-
-def test_string_concat(short_str_list):
-    with MultiWorker(concat, 4, reduction=string_concatenation_reduction) as f:
-        res = f(short_str_list)
-    assert res == "".join(short_str_list)
+from workercontext import MultiWorker
+from workercontext.reductions import (
+    ReductionComposition,
+    flatten_reduction,
+    sum_reduction,
+    average_reduction,
+    histogram_reduction,
+    product_reduction,
+    string_concatenation_reduction,
+    min_reduction,
+    max_reduction,
+)
+import pytest
+from typing import List
+
+
+@pytest.fixture
+def short_list():
+    return [1, 2, 3, 4, 5, 6, 7, 8]
+
+
+@pytest.fixture
+def short_str_list():
+    return ["Hello", "World", "I", "Am", "A", "String"]
+
+
+@pytest.fixture
+def duplicated_list():
+    return [1, 1, 1, 1, 2, 2, 2, 2]
+
+
+def list_return(l: List[int]) -> List[int]:
+    return [el * 2 for el in l]
+
+
+def concat(l: List[str]) -> str:
+    return "".join(l)
+
+
+def int_return(l: List[int]) -> List[int]:
+    return sum(l)
+
+
+def do_nothing(l: List[int]) -> List[int]:
+    return l
+
+
+def test_flatten(short_list):
+    with MultiWorker(list_return, 4, reduction=flatten_reduction) as f:
+        res = f(short_list)
+    assert res[0] == 2 and res[-1] == 16
+    assert len(res) == len(short_list)
+
+
+def test_sum(short_list):
+    with MultiWorker(int_return, 4, reduction=sum_reduction) as f:
+        res = f(short_list)
+    assert res == sum(short_list)
+
+
+def test_average(short_list):
+    reductions = ReductionComposition([flatten_reduction, average_reduction])
+    with MultiWorker(do_nothing, 4, reduction=reductions) as f:
+        res = f(short_list)
+    assert res == sum(short_list) / len(short_list)
+
+
+def test_histogram(duplicated_list):
+    with MultiWorker(int_return, 4, reduction=histogram_reduction) as f:
+        res = f(duplicated_list)
+    print(res)
+    assert res[2] == 2
+
+
+def test_min(short_list):
+    with MultiWorker(int_return, 4, reduction=min_reduction) as f:
+        res = f(short_list)
+    assert res == 3
+
+
+def test_max(short_list):
+    with MultiWorker(int_return, 4, reduction=max_reduction) as f:
+        res = f(short_list)
+    assert res == 15
+
+
+def test_composed(short_list):
+    reductions = ReductionComposition([flatten_reduction, product_reduction])
+
+    with MultiWorker(list_return, 4, reduction=reductions) as f:
+        res = f(short_list)
+    assert res == 10321920
+
+
+def test_string_concat(short_str_list):
+    with MultiWorker(concat, 4, reduction=string_concatenation_reduction) as f:
+        res = f(short_str_list)
+    assert res == "".join(short_str_list)
```

