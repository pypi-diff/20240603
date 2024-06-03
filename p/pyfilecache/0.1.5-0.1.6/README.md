# Comparing `tmp/pyfilecache-0.1.5.tar.gz` & `tmp/pyfilecache-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfilecache-0.1.5.tar", last modified: Sat Jun  1 11:45:03 2024, max compression
+gzip compressed data, was "pyfilecache-0.1.6.tar", last modified: Mon Jun  3 09:08:36 2024, max compression
```

## Comparing `pyfilecache-0.1.5.tar` & `pyfilecache-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 11:45:03.515094 pyfilecache-0.1.5/
--rw-rw-rw-   0        0        0       66 2024-05-30 12:31:32.000000 pyfilecache-0.1.5/.gitignore
--rw-rw-rw-   0        0        0     5464 2024-06-01 11:45:03.515094 pyfilecache-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     3290 2024-06-01 11:39:16.000000 pyfilecache-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 11:45:03.498098 pyfilecache-0.1.5/examples/
--rw-rw-rw-   0        0        0      235 2024-05-30 12:31:32.000000 pyfilecache-0.1.5/examples/add.py
--rw-rw-rw-   0        0        0      402 2024-05-30 12:31:32.000000 pyfilecache-0.1.5/examples/df.py
--rw-rw-rw-   0        0        0      633 2024-06-01 03:25:39.000000 pyfilecache-0.1.5/examples/process.py
--rw-rw-rw-   0        0        0      296 2024-06-01 11:35:01.000000 pyfilecache-0.1.5/examples/signatures.py
--rw-rw-rw-   0        0        0      294 2024-06-01 04:10:36.000000 pyfilecache-0.1.5/examples/versions.py
-drwxrwxrwx   0        0        0        0 2024-06-01 11:45:03.500093 pyfilecache-0.1.5/pyfilecache/
--rw-rw-rw-   0        0        0     4495 2024-06-01 11:33:38.000000 pyfilecache-0.1.5/pyfilecache/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 11:45:03.512095 pyfilecache-0.1.5/pyfilecache.egg-info/
--rw-rw-rw-   0        0        0     5464 2024-06-01 11:45:03.000000 pyfilecache-0.1.5/pyfilecache.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2024-06-01 11:45:03.000000 pyfilecache-0.1.5/pyfilecache.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 11:45:03.000000 pyfilecache-0.1.5/pyfilecache.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-06-01 11:45:03.000000 pyfilecache-0.1.5/pyfilecache.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-06-01 11:45:03.000000 pyfilecache-0.1.5/pyfilecache.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       93 2024-05-30 12:31:32.000000 pyfilecache-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-06-01 11:45:03.516092 pyfilecache-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      713 2024-06-01 11:43:30.000000 pyfilecache-0.1.5/setup.py
+drwxr-xr-x   0 didi       (601) staff       (20)        0 2024-06-03 09:08:36.948999 pyfilecache-0.1.6/
+-rw-r--r--   0 didi       (601) staff       (20)     3548 2024-06-03 09:08:36.948714 pyfilecache-0.1.6/PKG-INFO
+-rw-r--r--   0 didi       (601) staff       (20)     3084 2024-06-03 08:54:44.000000 pyfilecache-0.1.6/README.md
+drwxr-xr-x   0 didi       (601) staff       (20)        0 2024-06-03 09:08:36.945830 pyfilecache-0.1.6/pyfilecache/
+-rw-r--r--   0 didi       (601) staff       (20)     4521 2024-06-03 09:02:57.000000 pyfilecache-0.1.6/pyfilecache/__init__.py
+drwxr-xr-x   0 didi       (601) staff       (20)        0 2024-06-03 09:08:36.948241 pyfilecache-0.1.6/pyfilecache.egg-info/
+-rw-r--r--   0 didi       (601) staff       (20)     3548 2024-06-03 09:08:36.000000 pyfilecache-0.1.6/pyfilecache.egg-info/PKG-INFO
+-rw-r--r--   0 didi       (601) staff       (20)      231 2024-06-03 09:08:36.000000 pyfilecache-0.1.6/pyfilecache.egg-info/SOURCES.txt
+-rw-r--r--   0 didi       (601) staff       (20)        1 2024-06-03 09:08:36.000000 pyfilecache-0.1.6/pyfilecache.egg-info/dependency_links.txt
+-rw-r--r--   0 didi       (601) staff       (20)        9 2024-06-03 09:08:36.000000 pyfilecache-0.1.6/pyfilecache.egg-info/requires.txt
+-rw-r--r--   0 didi       (601) staff       (20)       12 2024-06-03 09:08:36.000000 pyfilecache-0.1.6/pyfilecache.egg-info/top_level.txt
+-rw-r--r--   0 didi       (601) staff       (20)       90 2024-06-03 08:54:44.000000 pyfilecache-0.1.6/pyproject.toml
+-rw-r--r--   0 didi       (601) staff       (20)       38 2024-06-03 09:08:36.949114 pyfilecache-0.1.6/setup.cfg
+-rw-r--r--   0 didi       (601) staff       (20)      692 2024-06-03 09:05:54.000000 pyfilecache-0.1.6/setup.py
```

### Comparing `pyfilecache-0.1.5/pyfilecache/__init__.py` & `pyfilecache-0.1.6/pyfilecache/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,129 +1,134 @@
-from io import TextIOWrapper
-from pathlib import Path
-from typing import Any, Hashable, Callable, Dict
-from functools import _make_key, partial
-import pickle, inspect
-import filelock
-
-__all__ = ['file_cache']
-
-CACHE_DIR = '__pyfilecache__'
-
-class _FileCached:
-    def __init__(
-            self,
-            user_function: Callable,
-            reader: Callable[[TextIOWrapper], Any],
-            writer: Callable[[Any, TextIOWrapper], None],
-            typed: bool = False,
-            version: str = None
-    ):
-        self.reader, self.writer = reader, writer
-        self.typed = typed
-        self.user_function = user_function
-        self._version = version
-
-        self._build()
-
-    def _build(self):
-        """
-        init the index of CACHE_DIR
-        """
-        self.code_path = Path(inspect.getfile(self.user_function))
-        self.cache_dir = self.code_path.parent.joinpath(CACHE_DIR)
-        self.cache_dir.mkdir(exist_ok=True)
-        self.funcache_dir = self.cache_dir.joinpath(f'{self.code_path.name}...{self.user_function.__qualname__}')
-        self.funcache_dir.mkdir(exist_ok=True)
-        self.index_dir = self.funcache_dir.joinpath('index')
-        if not self.index_dir.exists():
-            with open(self.index_dir, 'wb') as f:
-                pickle.dump({}, f)
-        self.lock_dir = self.index_dir.parent.joinpath('lock')
-        self.lock = filelock.FileLock(self.lock_dir)
-
-    def __call__(self, *args, **kwds):
-        """
-        wrapper of user_function
-        """
-        fidxp = self.fp(*args, **kwds)
-        with self.lock:
-            if fidxp.exists():
-                with open(fidxp, 'rb') as f:
-                    return self.reader(f)
-        result = self.user_function(*args, **kwds)
-        with self.lock:
-            with open(fidxp, 'wb') as f:
-                self.writer(result, f)
-        return result
-        
-    def fp(self, *args, **kwds):
-        """
-        the file path where the result of user_function(*args, **kwds) stored
-        """
-        func_identifier = (inspect.signature(self.user_function), self.user_function.__code__.co_code)
-        key = tuple(_make_key((func_identifier, *args), kwds, self.typed))
-        idx = self._key2findex(key)
-        return self.funcache_dir.joinpath(f'{self.version}_{idx}')
-
-    def _key2findex(self, key: Hashable) -> int:
-        with self.lock:
-            with open(self.index_dir, "rb") as f:
-                index: Dict[Any, int] = pickle.load(f)
-            result = index.get(key)
-            if result is None:
-                with open(self.index_dir, "wb") as f:
-                    index[key] = len(index)
-                    pickle.dump(index, f)
-        return index[key]
-    
-    def clear(self):
-        """
-        clear all stored results of this function
-        """
-        with self.lock:
-            for fp in self.funcache_dir.glob(f'{self.version}_*'): fp.unlink()
-        self._build()
-
-    @property
-    def version(self):
-        return "" if self._version is None else self._version
-    
-    def __getitem__(self, version: str):
-        if self._version is not None: raise RuntimeError(f'overwriting the existing version {self.version} with {version}')
-        if not (isinstance(version, str) and version.isalnum()): raise TypeError('version indices must be str that satisfy isalnum')
-        return _FileCached(self.user_function, self.reader, self.writer, self.typed, version)
-
-def file_cache(
-    user_function: Callable = None, *,
-    reader: Callable[[TextIOWrapper], Any] = pickle.load,
-    writer: Callable[[Any, TextIOWrapper], None] = pickle.dump,
-    typed: bool = False
-):
-    """
-    decorator of a slow function that stores the result to disk  
-
-    Usage Example:
-    ```py
-    import pandas as pd
-    from functools import partial
-    from pyfilecache import file_cache
-
-    @file_cache(
-        reader=partial(pd.read_csv, index_col=0),
-        writer=pd.DataFrame.to_csv
-    )
-    def func(a, b):
-        print("func called with args", a, b)
-        return pd.DataFrame(
-            data = {
-                'col1': [1, 2],
-                'col2': [a, b]
-            }
-        )
-
-    print(func(3, 4))
-    print(func(3, 4))
-    ```
-    """
-    if user_function is None: return partial(_FileCached, reader=reader, writer=writer, typed=typed)
+from io import TextIOWrapper
+from pathlib import Path
+from typing import Any, Hashable, Callable, Dict
+from functools import _make_key, partial
+import pickle, inspect
+import filelock
+
+__all__ = ['file_cache']
+
+CACHE_DIR = '__pyfilecache__'
+
+class _FileCached:
+    def __init__(
+            self,
+            user_function: Callable,
+            reader: Callable[[TextIOWrapper], Any],
+            writer: Callable[[Any, TextIOWrapper], None],
+            typed: bool = False,
+            version: str = None
+    ):
+        self.reader, self.writer = reader, writer
+        self.typed = typed
+        self.user_function = user_function
+        self._version = version
+
+        self._build()
+
+    def _build(self):
+        """
+        init the index of CACHE_DIR
+        """
+        self.code_path = Path(inspect.getfile(self.user_function))
+        self.cache_dir = self.code_path.parent.joinpath(CACHE_DIR)
+        self.cache_dir.mkdir(exist_ok=True)
+        self.funcache_dir = self.cache_dir.joinpath(f'{self.code_path.name}...{self.user_function.__qualname__}')
+        self.funcache_dir.mkdir(exist_ok=True)
+        self.index_dir = self.funcache_dir.joinpath('index')
+        if not self.index_dir.exists():
+            with open(self.index_dir, 'wb') as f:
+                pickle.dump({}, f)
+        self.lock_dir = self.index_dir.parent.joinpath('lock')
+        self.lock = filelock.FileLock(self.lock_dir)
+
+    def __call__(self, *args, **kwds):
+        """
+        wrapper of user_function
+        """
+        fidxp = self.fp(*args, **kwds)
+        with self.lock:
+            if fidxp.exists():
+                with open(fidxp, 'rb') as f:
+                    return self.reader(f)
+        result = self.user_function(*args, **kwds)
+        with self.lock:
+            flag = True
+            try:
+                with open(fidxp, 'wb') as f:
+                    self.writer(result, f)
+                flag = False
+            finally:
+                if flag: fidxp.unlink(missing_ok=True)
+        return result
+        
+    def fp(self, *args, **kwds):
+        """
+        the file path where the result of user_function(*args, **kwds) stored
+        """
+        func_identifier = (inspect.signature(self.user_function), self.user_function.__code__.co_code)
+        key = tuple(_make_key((func_identifier, *args), kwds, self.typed))
+        idx = self._key2findex(key)
+        return self.funcache_dir.joinpath(f'{self.version}_{idx}')
+
+    def _key2findex(self, key: Hashable) -> int:
+        with self.lock:
+            with open(self.index_dir, "rb") as f:
+                index: Dict[Any, int] = pickle.load(f)
+            result = index.get(key)
+            if result is None:
+                with open(self.index_dir, "wb") as f:
+                    index[key] = len(index)
+                    pickle.dump(index, f)
+        return index[key]
+    
+    def clear(self):
+        """
+        clear all stored results of this function
+        """
+        with self.lock:
+            for fp in self.funcache_dir.glob(f'{self.version}_*'): fp.unlink()
+        self._build()
+
+    @property
+    def version(self):
+        return "" if self._version is None else self._version
+    
+    def __getitem__(self, version: str):
+        if self._version is not None: raise RuntimeError(f'overwriting the existing version {self.version} with {version}')
+        if not (isinstance(version, str) and version.isalnum()): raise TypeError('version indices must be str that satisfy isalnum')
+        return _FileCached(self.user_function, self.reader, self.writer, self.typed, version)
+
+def file_cache(
+    user_function: Callable = None, *,
+    reader: Callable[[TextIOWrapper], Any] = pickle.load,
+    writer: Callable[[Any, TextIOWrapper], None] = pickle.dump,
+    typed: bool = False
+):
+    """
+    decorator of a slow function that stores the result to disk  
+
+    Usage Example:
+    ```py
+    import pandas as pd
+    from functools import partial
+    from pyfilecache import file_cache
+
+    @file_cache(
+        reader=partial(pd.read_csv, index_col=0),
+        writer=pd.DataFrame.to_csv
+    )
+    def func(a, b):
+        print("func called with args", a, b)
+        return pd.DataFrame(
+            data = {
+                'col1': [1, 2],
+                'col2': [a, b]
+            }
+        )
+
+    print(func(3, 4))
+    print(func(3, 4))
+    ```
+    """
+    if user_function is None: return partial(_FileCached, reader=reader, writer=writer, typed=typed)
     return _FileCached(user_function, reader, writer, typed)
```

