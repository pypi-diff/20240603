# Comparing `tmp/python_filewrap-0.1.0.1.tar.gz` & `tmp/python_filewrap-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_filewrap-0.1.0.1.tar", max compression
+gzip compressed data, was "python_filewrap-0.1.1.tar", max compression
```

## Comparing `python_filewrap-0.1.0.1.tar` & `python_filewrap-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_filewrap-0.1.0.1/LICENSE
--rwxr-xr-x   0        0        0    19762 2024-05-27 13:43:27.204764 python_filewrap-0.1.0.1/filewrap/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_filewrap-0.1.0.1/filewrap/py.typed
--rw-r--r--   0        0        0     1173 2024-05-27 13:43:54.527747 python_filewrap-0.1.0.1/pyproject.toml
--rw-r--r--   0        0        0      201 2024-05-14 10:43:51.477479 python_filewrap-0.1.0.1/readme.md
--rw-r--r--   0        0        0     1364 1970-01-01 00:00:00.000000 python_filewrap-0.1.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_filewrap-0.1.1/LICENSE
+-rwxr-xr-x   0        0        0    22066 2024-06-03 12:13:42.827180 python_filewrap-0.1.1/filewrap/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_filewrap-0.1.1/filewrap/py.typed
+-rw-r--r--   0        0        0     1171 2024-06-03 12:16:36.169402 python_filewrap-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      201 2024-05-14 10:43:51.477479 python_filewrap-0.1.1/readme.md
+-rw-r--r--   0        0        0     1362 1970-01-01 00:00:00.000000 python_filewrap-0.1.1/PKG-INFO
```

### Comparing `python_filewrap-0.1.0.1/LICENSE` & `python_filewrap-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_filewrap-0.1.0.1/filewrap/__init__.py` & `python_filewrap-0.1.1/filewrap/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 #!/usr/bin/env python3
 # encoding: utf-8
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
-__version__ = (0, 1)
+__version__ = (0, 1, 1)
 __all__ = [
     "Buffer", "SupportsRead", "SupportsReadinto", 
     "SupportsWrite", "SupportsSeek", 
     "bio_chunk_iter", "bio_chunk_async_iter", 
     "bio_skip_iter", "bio_skip_async_iter", 
     "bytes_iter_skip", "bytes_async_iter_skip", 
     "bytes_iter_to_reader", "bytes_iter_to_async_reader", 
     "bytes_to_chunk_iter", "bytes_to_chunk_async_iter", 
     "bytes_ensure_part_iter", "bytes_ensure_part_async_iter", 
+    "progress_bytes_iter", "progress_bytes_async_iter", 
 ]
 
 from asyncio import to_thread, Lock as AsyncLock
 from collections.abc import Awaitable, AsyncIterable, AsyncIterator, Callable, Iterable, Iterator
 from functools import update_wrapper
-from inspect import isawaitable, iscoroutinefunction
+from inspect import isawaitable, iscoroutinefunction, isasyncgen, isgenerator
 from itertools import chain
 from shutil import COPY_BUFSIZE # type: ignore
 from threading import Lock
-from typing import runtime_checkable, Any, Protocol, TypeVar
+from typing import runtime_checkable, Any, ParamSpec, Protocol, TypeVar
 
 try:
     from collections.abc import Buffer # type: ignore
 except ImportError:
     from abc import ABC, abstractmethod
     from array import array
 
@@ -55,18 +56,18 @@
             return NotImplemented
 
     Buffer.register(bytes)
     Buffer.register(bytearray)
     Buffer.register(memoryview)
     Buffer.register(array)
 
-
 from asynctools import async_chain, ensure_async, ensure_aiter
 
 
+Args = ParamSpec("Args")
 _T_co = TypeVar("_T_co", covariant=True)
 _T_contra = TypeVar("_T_contra", contravariant=True)
 
 
 @runtime_checkable
 class SupportsRead(Protocol[_T_co]):
     def read(self, /, __length: int = ...) -> _T_co: ...
@@ -651,7 +652,75 @@
                 m = m[partsize:]
             if m:
                 yield m
                 n = partsize - len(m)
             else:
                 n = partsize
 
+
+def progress_bytes_iter(
+    it: Iterable[Buffer], 
+    make_progress: None | Callable[Args, Any] = None, 
+    /, 
+    *args: Args.args, 
+    **kwds: Args.kwargs, 
+) -> Iterator[Buffer]:
+    update_progress: None | Callable = None
+    close_progress: None | Callable = None
+    if callable(make_progress):
+        progress = make_progress(*args, **kwds)
+        if isgenerator(progress):
+            next(progress)
+            update_progress = progress.send
+            close_progress = progress.close
+        else:
+            update_progress = progress
+            close_progress = getattr(progress, "close", None)
+    try:
+        if callable(update_progress):
+            for chunk in it:
+                yield chunk
+                update_progress(len(chunk))
+        else:
+            for chunk in it:
+                yield chunk
+    finally:
+        if callable(close_progress):
+            close_progress()
+
+
+async def progress_bytes_async_iter(
+    it: Iterable[Buffer] | AsyncIterable[Buffer], 
+    make_progress: None | Callable[Args, Any] = None, 
+    /, 
+    *args: Args.args, 
+    **kwds: Args.kwargs, 
+) -> AsyncIterator[Buffer]:
+    update_progress: None | Callable = None
+    close_progress: None | Callable = None
+    if callable(make_progress):
+        progress = make_progress(*args, **kwds)
+        if isgenerator(progress):
+            await ensure_async(next)(progress)
+            update_progress = progress.send
+            close_progress = progress.close
+        elif isasyncgen(progress):
+            await anext(progress)
+            update_progress = progress.asend
+            close_progress = progress.aclose
+        else:
+            update_progress = progress
+            close_progress = getattr(progress, "close", None)
+    try:
+        it = ensure_aiter(it)
+        if callable(update_progress):
+            update_progress = ensure_async(update_progress)
+            async for chunk in it:
+                yield chunk
+                await update_progress(len(chunk))
+        else:
+            async for chunk in it:
+                yield chunk
+    finally:
+        if callable(close_progress):
+            await ensure_async(close_progress)()
+
```

### Comparing `python_filewrap-0.1.0.1/pyproject.toml` & `python_filewrap-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-filewrap"
-version = "0.1.0.1"
+version = "0.1.1"
 description = "Python file wrappers."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-filewrap"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-filewrap"
 keywords = ["file", "wrapper"]
```

### Comparing `python_filewrap-0.1.0.1/PKG-INFO` & `python_filewrap-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-filewrap
-Version: 0.1.0.1
+Version: 0.1.1
 Summary: Python file wrappers.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-filewrap
 License: MIT
 Keywords: file,wrapper
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
```

