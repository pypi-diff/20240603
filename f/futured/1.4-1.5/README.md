# Comparing `tmp/futured-1.4.tar.gz` & `tmp/futured-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "futured-1.4.tar", last modified: Sat May  6 18:54:59 2023, max compression
+gzip compressed data, was "futured-1.5.tar", last modified: Sun Jun  2 23:22:44 2024, max compression
```

## Comparing `futured-1.4.tar` & `futured-1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 coady      (501) staff       (20)        0 2023-05-06 18:54:59.327152 futured-1.4/
--rw-r--r--   0 coady      (501) staff       (20)      576 2022-04-25 21:08:17.000000 futured-1.4/LICENSE.txt
--rw-r--r--   0 coady      (501) staff       (20)     7227 2023-05-06 18:54:59.327034 futured-1.4/PKG-INFO
--rw-r--r--   0 coady      (501) staff       (20)     5446 2023-05-06 18:19:03.000000 futured-1.4/README.md
-drwxr-xr-x   0 coady      (501) staff       (20)        0 2023-05-06 18:54:59.326251 futured-1.4/futured/
--rw-r--r--   0 coady      (501) staff       (20)     8771 2023-05-06 18:36:26.000000 futured-1.4/futured/__init__.py
--rw-r--r--   0 coady      (501) staff       (20)        0 2020-10-25 18:57:52.000000 futured-1.4/futured/py.typed
-drwxr-xr-x   0 coady      (501) staff       (20)        0 2023-05-06 18:54:59.326647 futured-1.4/futured.egg-info/
--rw-r--r--   0 coady      (501) staff       (20)     7227 2023-05-06 18:54:59.000000 futured-1.4/futured.egg-info/PKG-INFO
--rw-r--r--   0 coady      (501) staff       (20)      215 2023-05-06 18:54:59.000000 futured-1.4/futured.egg-info/SOURCES.txt
--rw-r--r--   0 coady      (501) staff       (20)        1 2023-05-06 18:54:59.000000 futured-1.4/futured.egg-info/dependency_links.txt
--rw-r--r--   0 coady      (501) staff       (20)        8 2023-05-06 18:54:59.000000 futured-1.4/futured.egg-info/top_level.txt
--rw-r--r--   0 coady      (501) staff       (20)     1491 2023-03-17 20:50:37.000000 futured-1.4/pyproject.toml
--rw-r--r--   0 coady      (501) staff       (20)       38 2023-05-06 18:54:59.327185 futured-1.4/setup.cfg
-drwxr-xr-x   0 coady      (501) staff       (20)        0 2023-05-06 18:54:59.326758 futured-1.4/tests/
--rw-r--r--   0 coady      (501) staff       (20)     4680 2022-11-19 03:19:34.000000 futured-1.4/tests/test_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 23:22:44.530806 futured-1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-06-02 23:22:20.000000 futured-1.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7044 2024-06-02 23:22:44.530806 futured-1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-06-02 23:22:20.000000 futured-1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 23:22:44.526806 futured-1.5/futured/
+-rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-06-02 23:22:20.000000 futured-1.5/futured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 23:22:20.000000 futured-1.5/futured/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 23:22:44.530806 futured-1.5/futured.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7044 2024-06-02 23:22:44.000000 futured-1.5/futured.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-06-02 23:22:44.000000 futured-1.5/futured.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 23:22:44.000000 futured-1.5/futured.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-02 23:22:44.000000 futured-1.5/futured.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-06-02 23:22:20.000000 futured-1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 23:22:44.530806 futured-1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 23:22:44.530806 futured-1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-06-02 23:22:20.000000 futured-1.5/tests/test_all.py
```

### Comparing `futured-1.4/LICENSE.txt` & `futured-1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `futured-1.4/PKG-INFO` & `futured-1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: futured
-Version: 1.4
-Summary: Functional interface for concurrent futures, including asynchronous I/O.
+Version: 1.5
+Summary: Functional interface for concurrent futures, including async coroutines.
 Author-email: Aric Coady <aric.coady@gmail.com>
 License: Copyright 2022 Aric Coady
         
            Licensed under the Apache License, Version 2.0 (the "License");
            you may not use this file except in compliance with the License.
            You may obtain a copy of the License at
         
@@ -15,43 +15,45 @@
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/coady/futured
 Project-URL: Documentation, https://coady.github.io/futured
+Project-URL: Changelog, https://github.com/coady/futured/blob/main/CHANGELOG.md
+Project-URL: Issues, https://github.com/coady/futured/issues
 Keywords: concurrent,futures,threads,processes,async,asyncio
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 [![image](https://img.shields.io/pypi/v/futured.svg)](https://pypi.org/project/futured/)
 ![image](https://img.shields.io/pypi/pyversions/futured.svg)
 [![image](https://pepy.tech/badge/futured)](https://pepy.tech/project/futured)
 ![image](https://img.shields.io/pypi/status/futured.svg)
 [![image](https://github.com/coady/futured/workflows/build/badge.svg)](https://github.com/coady/futured/actions)
 [![image](https://codecov.io/gh/coady/futured/branch/main/graph/badge.svg)](https://codecov.io/github/coady/futured)
 [![image](https://github.com/coady/futured/workflows/codeql/badge.svg)](https://github.com/coady/futured/security/code-scanning)
-[![image](https://img.shields.io/badge/code%20style-black-000000.svg)](https://pypi.org/project/black/)
-[![image](http://mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
+[![image](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+[![image](https://mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
 
-Futured provides a consistent interface for concurrent functional programming in Python. It wraps any callable to return a `concurrent.futures.Future`, wraps any async coroutine to return an `asyncio.Future`, and provides concurrent iterators and context managers for futures.
+Futured provides a consistent interface for concurrent functional programming in Python. It wraps any callable to return a `concurrent.futures.Future`, wraps any async coroutine with a compatible `Task` interface, and provides concurrent iterators and context managers for futures.
 
 ## Usage
 ### threaded, processed
 Transform any callable into one which runs in a thread or process pool, and returns a future.
 
 ```python
 from futured import threaded, processed
@@ -113,14 +115,21 @@
 ```python
 asynced.run(async_func, ...)  # call and run until complete
 asynced.run(async_gen, ...)  # call and run synchronous iterator
 with asynced.waiting(*fs) as tasks:  # concurrent coroutines completed in a block
 asynced.tasks(fs, timeout=...)  # mutable set of running tasks which iterate as completed
 ```
 
+### extensions
+There is also support for [dask distributed](https://distributed.dask.org/) clients and [gevent](http://www.gevent.org/) greenlets.
+
+```python
+from futured import distributed, greened
+```
+
 ### decorators
 Naturally `futured` wrappers can be used as decorators, but arguments can also be partially bound.
 
 ```python
 @threaded
 def slow():
    ...
@@ -174,44 +183,7 @@
 
 ## Tests
 100% branch coverage.
 
 ```console
 % pytest [--cov]
 ```
-
-## Changes
-1.4
-
-* Python >=3.8 required
-
-1.3
-
-* Python >=3.7 required
-* Python 3.10 event loop changes
-* Streams replaced with tasks
-
-1.2
-
-* Python >=3.6 required
-
-1.1
-
-* Stream completed futures from a pending pool
-
-1.0
-
-* Executed functions are context managers
-* `starmap` supported
-
-0.3
-
-* `forked` has optional maximum number of workers
-* `waiting` context manager
-* `command` pipes (`|`)
-* `distributed.Client` support
-
-0.2
-
-* `command.coroutine` creates asyncio subprocesses
-* `futured.mapzip` generates results zipped with arguments
-* `asynced.run` supports asynchronous iterators
```

### Comparing `futured-1.4/README.md` & `futured-1.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [![image](https://img.shields.io/pypi/v/futured.svg)](https://pypi.org/project/futured/)
 ![image](https://img.shields.io/pypi/pyversions/futured.svg)
 [![image](https://pepy.tech/badge/futured)](https://pepy.tech/project/futured)
 ![image](https://img.shields.io/pypi/status/futured.svg)
 [![image](https://github.com/coady/futured/workflows/build/badge.svg)](https://github.com/coady/futured/actions)
 [![image](https://codecov.io/gh/coady/futured/branch/main/graph/badge.svg)](https://codecov.io/github/coady/futured)
 [![image](https://github.com/coady/futured/workflows/codeql/badge.svg)](https://github.com/coady/futured/security/code-scanning)
-[![image](https://img.shields.io/badge/code%20style-black-000000.svg)](https://pypi.org/project/black/)
-[![image](http://mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
+[![image](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+[![image](https://mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
 
-Futured provides a consistent interface for concurrent functional programming in Python. It wraps any callable to return a `concurrent.futures.Future`, wraps any async coroutine to return an `asyncio.Future`, and provides concurrent iterators and context managers for futures.
+Futured provides a consistent interface for concurrent functional programming in Python. It wraps any callable to return a `concurrent.futures.Future`, wraps any async coroutine with a compatible `Task` interface, and provides concurrent iterators and context managers for futures.
 
 ## Usage
 ### threaded, processed
 Transform any callable into one which runs in a thread or process pool, and returns a future.
 
 ```python
 from futured import threaded, processed
@@ -74,14 +74,21 @@
 ```python
 asynced.run(async_func, ...)  # call and run until complete
 asynced.run(async_gen, ...)  # call and run synchronous iterator
 with asynced.waiting(*fs) as tasks:  # concurrent coroutines completed in a block
 asynced.tasks(fs, timeout=...)  # mutable set of running tasks which iterate as completed
 ```
 
+### extensions
+There is also support for [dask distributed](https://distributed.dask.org/) clients and [gevent](http://www.gevent.org/) greenlets.
+
+```python
+from futured import distributed, greened
+```
+
 ### decorators
 Naturally `futured` wrappers can be used as decorators, but arguments can also be partially bound.
 
 ```python
 @threaded
 def slow():
    ...
@@ -135,44 +142,7 @@
 
 ## Tests
 100% branch coverage.
 
 ```console
 % pytest [--cov]
 ```
-
-## Changes
-1.4
-
-* Python >=3.8 required
-
-1.3
-
-* Python >=3.7 required
-* Python 3.10 event loop changes
-* Streams replaced with tasks
-
-1.2
-
-* Python >=3.6 required
-
-1.1
-
-* Stream completed futures from a pending pool
-
-1.0
-
-* Executed functions are context managers
-* `starmap` supported
-
-0.3
-
-* `forked` has optional maximum number of workers
-* `waiting` context manager
-* `command` pipes (`|`)
-* `distributed.Client` support
-
-0.2
-
-* `command.coroutine` creates asyncio subprocesses
-* `futured.mapzip` generates results zipped with arguments
-* `asynced.run` supports asynchronous iterators
```

### Comparing `futured-1.4/futured/__init__.py` & `futured-1.5/futured/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import asyncio
 import contextlib
 import itertools
 import operator
 import os
 import subprocess
 import types
+from collections.abc import AsyncIterable, Callable, Iterable, Iterator
 from concurrent import futures
 from functools import partial
-from typing import AnyStr, AsyncIterable, Callable, Iterable, Iterator, Optional
-
-__version__ = '1.4'
+from typing import Union
 
 
 class futured(partial):
     """A partial function which returns futures."""
 
     as_completed: Callable = NotImplemented
 
@@ -75,28 +74,30 @@
             yield fs
         finally:
             fs[:] = cls.results(fs, **kwargs)
 
     class tasks(set):
         """A set of futures which iterate as completed, and can be updated while iterating."""
 
-        wait = staticmethod(futures.wait)
         TimeoutError = futures.TimeoutError
 
         def __init__(self, fs: Iterable, *, timeout=None):
             super().__init__(fs)
-            self.options = dict(return_when='FIRST_COMPLETED', timeout=timeout)
+            self.timeout = timeout
             self.it = self.iter()
 
+        def wait(self, fs: list) -> Iterable:
+            return futures.wait(fs, self.timeout, return_when='FIRST_COMPLETED').done
+
         def iter(self):
             while self:
-                done, _ = self.wait(list(super().__iter__()), **self.options)
+                done = self.wait(list(super().__iter__()))
                 if not done:
                     raise self.TimeoutError
-                self -= done
+                self.difference_update(done)
                 yield from done
 
         def __iter__(self):
             return self
 
         def __next__(self):
             return next(self.it)
@@ -137,18 +138,15 @@
     class distributed(executed):
         """A partial function executed by a dask distributed client."""
 
         from distributed import as_completed, Client as Executor  # type: ignore
 
 
 class asynced(futured):
-    """A partial coroutine.
-
-    Anywhere futures are expected, coroutines are also supported.
-    """
+    """A partial async coroutine."""
 
     @classmethod
     def results(cls, fs: Iterable, *, as_completed=False, **kwargs) -> Iterator:
         if as_completed or kwargs:
             return map(operator.methodcaller('result'), cls.tasks(fs, **kwargs))
         loop = asyncio.new_event_loop()
         tasks = list(map(loop.create_task, fs))
@@ -191,16 +189,46 @@
         def __init__(self, coros: Iterable, **kwargs):
             self.loop = asyncio.new_event_loop()
             super().__init__(map(self.loop.create_task, coros), **kwargs)
 
         def add(self, coro):
             super().add(self.loop.create_task(coro))
 
-        def wait(self, *args, **kwargs):
-            return self.loop.run_until_complete(asyncio.wait(*args, **kwargs))
+        def wait(self, fs: list) -> Iterable:
+            coro = asyncio.wait(fs, timeout=self.timeout, return_when='FIRST_COMPLETED')
+            return self.loop.run_until_complete(coro)[0]
+
+
+with contextlib.suppress(ImportError):
+    import gevent.pool  # type: ignore
+
+    class greened(futured):
+        """A partial gevent greenlet."""
+
+        def __new__(cls, *args, **kwargs):
+            if args:
+                return futured.__new__(cls, gevent.spawn, *args, **kwargs)
+            return partial(futured.__new__, cls, gevent.pool.Pool(**kwargs).spawn)
+
+        @classmethod
+        def results(cls, fs: Iterable, *, as_completed=False, **kwargs) -> Iterator:
+            tasks = cls.tasks(fs, **kwargs) if (as_completed or kwargs) else list(fs)
+            return map(operator.methodcaller('get'), tasks)
+
+        @classmethod
+        def items(cls, pairs: Iterable, **kwargs) -> Iterator:
+            keys = dict(map(reversed, pairs))  # type: ignore
+            return ((keys[future], future.get()) for future in cls.tasks(keys, **kwargs))
+
+        class tasks(futured.tasks):
+            __doc__ = futured.tasks.__doc__
+            TimeoutError = gevent.Timeout
+
+            def wait(self, fs: list) -> Iterable:
+                return gevent.wait(fs, self.timeout, count=1)
 
 
 class command(subprocess.Popen):
     """Asynchronous subprocess with a future compatible interface."""
 
     def __init__(self, *args, **kwargs):
         super().__init__(args, stdout=subprocess.PIPE, stderr=subprocess.PIPE, **kwargs)
@@ -213,15 +241,15 @@
     @classmethod
     async def coroutine(cls, *args, shell=False, **kwargs):
         """Create a subprocess coroutine, suitable for timeouts."""
         create = asyncio.create_subprocess_shell if shell else asyncio.create_subprocess_exec
         self = await create(*args, stdout=subprocess.PIPE, stderr=subprocess.PIPE, **kwargs)
         return cls.check(self, args, *(await self.communicate()))
 
-    def result(self, **kwargs) -> AnyStr:
+    def result(self, **kwargs) -> Union[str, bytes]:
         """Return stdout or raise stderr."""
         return self.check(self.args, *self.communicate(**kwargs))
 
     def pipe(self, *args, **kwargs) -> 'command':
         """Pipe stdout to the next command's stdin."""
         return type(self)(*args, stdin=self.stdout, **kwargs)
 
@@ -230,31 +258,30 @@
         return self.pipe(*other)
 
     def __iter__(self):
         """Return output lines."""
         return iter(self.result().splitlines())
 
 
-def forked(values: Iterable, max_workers: Optional[int] = None) -> Iterator:
+def forked(values: Iterable, max_workers: int = 0) -> Iterator:
     """Generate each value in its own child process and wait in the parent."""
     max_workers = max_workers or os.cpu_count() or 1  # same default as ProcessPoolExecutor
     workers: dict = {}
 
     def wait():
         pid, status = os.wait()
         if pid in workers:
             value = workers.pop(pid)
             if status:
                 raise OSError(status, value)
 
     for value in values:
         while len(workers) >= max_workers:
             wait()
-        pid = os.fork()
-        if pid:
+        if pid := os.fork():
             workers[pid] = value
         else:  # pragma: no cover
             yield value
             os._exit(0)
     while workers:
         wait()
```

### Comparing `futured-1.4/futured.egg-info/PKG-INFO` & `futured-1.5/futured.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: futured
-Version: 1.4
-Summary: Functional interface for concurrent futures, including asynchronous I/O.
+Version: 1.5
+Summary: Functional interface for concurrent futures, including async coroutines.
 Author-email: Aric Coady <aric.coady@gmail.com>
 License: Copyright 2022 Aric Coady
         
            Licensed under the Apache License, Version 2.0 (the "License");
            you may not use this file except in compliance with the License.
            You may obtain a copy of the License at
         
@@ -15,43 +15,45 @@
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/coady/futured
 Project-URL: Documentation, https://coady.github.io/futured
+Project-URL: Changelog, https://github.com/coady/futured/blob/main/CHANGELOG.md
+Project-URL: Issues, https://github.com/coady/futured/issues
 Keywords: concurrent,futures,threads,processes,async,asyncio
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 [![image](https://img.shields.io/pypi/v/futured.svg)](https://pypi.org/project/futured/)
 ![image](https://img.shields.io/pypi/pyversions/futured.svg)
 [![image](https://pepy.tech/badge/futured)](https://pepy.tech/project/futured)
 ![image](https://img.shields.io/pypi/status/futured.svg)
 [![image](https://github.com/coady/futured/workflows/build/badge.svg)](https://github.com/coady/futured/actions)
 [![image](https://codecov.io/gh/coady/futured/branch/main/graph/badge.svg)](https://codecov.io/github/coady/futured)
 [![image](https://github.com/coady/futured/workflows/codeql/badge.svg)](https://github.com/coady/futured/security/code-scanning)
-[![image](https://img.shields.io/badge/code%20style-black-000000.svg)](https://pypi.org/project/black/)
-[![image](http://mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
+[![image](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+[![image](https://mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
 
-Futured provides a consistent interface for concurrent functional programming in Python. It wraps any callable to return a `concurrent.futures.Future`, wraps any async coroutine to return an `asyncio.Future`, and provides concurrent iterators and context managers for futures.
+Futured provides a consistent interface for concurrent functional programming in Python. It wraps any callable to return a `concurrent.futures.Future`, wraps any async coroutine with a compatible `Task` interface, and provides concurrent iterators and context managers for futures.
 
 ## Usage
 ### threaded, processed
 Transform any callable into one which runs in a thread or process pool, and returns a future.
 
 ```python
 from futured import threaded, processed
@@ -113,14 +115,21 @@
 ```python
 asynced.run(async_func, ...)  # call and run until complete
 asynced.run(async_gen, ...)  # call and run synchronous iterator
 with asynced.waiting(*fs) as tasks:  # concurrent coroutines completed in a block
 asynced.tasks(fs, timeout=...)  # mutable set of running tasks which iterate as completed
 ```
 
+### extensions
+There is also support for [dask distributed](https://distributed.dask.org/) clients and [gevent](http://www.gevent.org/) greenlets.
+
+```python
+from futured import distributed, greened
+```
+
 ### decorators
 Naturally `futured` wrappers can be used as decorators, but arguments can also be partially bound.
 
 ```python
 @threaded
 def slow():
    ...
@@ -174,44 +183,7 @@
 
 ## Tests
 100% branch coverage.
 
 ```console
 % pytest [--cov]
 ```
-
-## Changes
-1.4
-
-* Python >=3.8 required
-
-1.3
-
-* Python >=3.7 required
-* Python 3.10 event loop changes
-* Streams replaced with tasks
-
-1.2
-
-* Python >=3.6 required
-
-1.1
-
-* Stream completed futures from a pending pool
-
-1.0
-
-* Executed functions are context managers
-* `starmap` supported
-
-0.3
-
-* `forked` has optional maximum number of workers
-* `waiting` context manager
-* `command` pipes (`|`)
-* `distributed.Client` support
-
-0.2
-
-* `command.coroutine` creates asyncio subprocesses
-* `futured.mapzip` generates results zipped with arguments
-* `asynced.run` supports asynchronous iterators
```

### Comparing `futured-1.4/pyproject.toml` & `futured-1.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,41 @@
-[build-system]
-requires = ["setuptools>=61", "wheel"]
-build-backend = "setuptools.build_meta"
-
 [project]
 name = "futured"
-dynamic = ["version"]
-description = "Functional interface for concurrent futures, including asynchronous I/O."
+version = "1.5"
+description = "Functional interface for concurrent futures, including async coroutines."
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 license = {file = "LICENSE.txt"}
 authors = [{name = "Aric Coady", email = "aric.coady@gmail.com"}]
 keywords = ["concurrent", "futures", "threads", "processes", "async", "asyncio"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Framework :: AsyncIO",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: 3.13",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
-    
+
 [project.urls]
 Homepage = "https://github.com/coady/futured"
 Documentation = "https://coady.github.io/futured"
+Changelog = "https://github.com/coady/futured/blob/main/CHANGELOG.md"
+Issues = "https://github.com/coady/futured/issues"
 
-[tool.setuptools]
-packages = ["futured"]
-
-[tool.setuptools.dynamic]
-version = {attr = "futured.__version__"}
-
-[tool.setuptools.package-data]
-futured = ["py.typed"]
-
-[tool.black]
+[tool.ruff]
 line-length = 100
-skip-string-normalization = true
+extend-include = ["*.ipynb"]
 
-[tool.ruff]
-ignore = ["E501"]
+[tool.ruff.format]
+quote-style = "single"
 
 [tool.coverage.run]
 source = ["futured"]
 branch = true
```

### Comparing `futured-1.4/tests/test_all.py` & `futured-1.5/tests/test_all.py`

 * *Files 6% similar despite different names*

```diff
@@ -150,7 +150,20 @@
     from futured import distributed
 
     with distributed(time.sleep) as dsleep:
         results = dsleep.map(delays, as_completed=True)
         assert list(dsleep.map(delays)) == list(results) == [None] * len(delays)
     with pytest.raises(Exception):
         dsleep(0)
+
+
+def test_gevent():
+    gevent = pytest.importorskip('gevent')
+    from futured import greened
+
+    sleep = greened(gevent.sleep)
+    assert list(sleep.map(delays)) == [None] * len(delays)
+    assert next(sleep.map(delays, as_completed=True)) is None
+    sleep = greened(size=len(delays))(gevent.sleep)
+    results = dict(sleep.mapzip(delays))
+    assert results == dict.fromkeys(delays)
+    assert list(results) == sorted(delays)
```

