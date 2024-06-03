# Comparing `tmp/stablehash-0.1.1.tar.gz` & `tmp/stablehash-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stablehash-0.1.1.tar", max compression
+gzip compressed data, was "stablehash-0.1.2.tar", last modified: Mon Jun  3 00:55:24 2024, max compression
```

## Comparing `stablehash-0.1.1.tar` & `stablehash-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      998 2024-01-28 23:37:45.148755 stablehash-0.1.1/LICENSE
--rw-r--r--   0        0        0     1546 2024-01-29 00:30:56.875236 stablehash-0.1.1/README.md
--rw-r--r--   0        0        0     2094 2024-01-29 01:38:46.987257 stablehash-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      981 2024-01-29 01:38:46.987448 stablehash-0.1.1/src/stablehash/__init__.py
--rw-r--r--   0        0        0     2023 2024-01-29 01:38:44.361442 stablehash-0.1.1/src/stablehash/__init__test.py
--rw-r--r--   0        0        0     2991 2024-01-29 01:38:44.367724 stablehash-0.1.1/src/stablehash/_tokenize.py
--rw-r--r--   0        0        0        0 2024-01-28 23:37:45.173287 stablehash-0.1.1/src/stablehash/py.typed
--rw-r--r--   0        0        0     2673 1970-01-01 00:00:00.000000 stablehash-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      998 2024-06-03 00:35:50.749729 stablehash-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1546 2024-06-03 00:35:50.749729 stablehash-0.1.2/README.md
+-rw-r--r--   0        0        0     1674 2024-06-03 00:55:24.973818 stablehash-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      981 2024-06-03 00:53:32.930936 stablehash-0.1.2/src/stablehash/__init__.py
+-rw-r--r--   0        0        0     2022 2024-06-03 00:53:21.771050 stablehash-0.1.2/src/stablehash/__init__test.py
+-rw-r--r--   0        0        0     2987 2024-06-03 00:53:21.771050 stablehash-0.1.2/src/stablehash/_tokenize.py
+-rw-r--r--   0        0        0        0 2024-06-03 00:35:50.749729 stablehash-0.1.2/src/stablehash/py.typed
+-rw-r--r--   0        0        0     2658 1970-01-01 00:00:00.000000 stablehash-0.1.2/PKG-INFO
```

### Comparing `stablehash-0.1.1/LICENSE` & `stablehash-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stablehash-0.1.1/README.md` & `stablehash-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 # stablehash
 
-The `stablehash` module provides a "pure" hash function that is stable across Python processes and runs. This is in contrast to the builtin `hash()` function, which may return a different value for the same input in separate invokations even with the Python version.
-
-We support most Python built-in types, including mutable types such as `list` and `dict`, as well as dataclasses. The default internal hash algorithm is Blake2b, but this can be changed by passing a different `hashlib` algorithm to the `stablehash` function.
+The `stablehash` module provides a "pure" hash function that is stable across Python processes and runs. This is in
+contrast to the builtin `hash()` function, which may return a different value for the same input in separate
+invokations even with the Python version.
+
+We support most Python built-in types, including mutable types such as `list` and `dict`, as well as dataclasses. The
+default internal hash algorithm is Blake2b, but this can be changed by passing a different `hashlib` algorithm to the
+`stablehash` function.
 
 ## Usage
 
 ```python
 from stablehash import stablehash
 
 assert stablehash({"key": "value"}, algorithm="md5").hexdigest() == 'd5994850379366e314563ea555532052'
 ```
 
 ## API
 
 ### `stablehash(obj=..., *, algorithm="blake2b")`
 
-Returns a `hashlib`-compatible object with the given algorithm and the hash of the given object. The algorithm must be one of the algorithms supported by `hashlib`.
+Returns a `hashlib`-compatible object with the given algorithm and the hash of the given object. The algorithm must be
+one of the algorithms supported by `hashlib`.
 
 ### `stablehash.update(obj)`
 
 Updates the hash with the given object. If the object is not supported, a `TypeError` is raised.
 
 ### `stablehash.digest()`
```

### Comparing `stablehash-0.1.1/src/stablehash/__init__.py` & `stablehash-0.1.2/src/stablehash/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 
 import hashlib
 from typing import Any
 
 from ._tokenize import tokenize
 
 _sentinel = object()
```

### Comparing `stablehash-0.1.1/src/stablehash/__init__test.py` & `stablehash-0.1.2/src/stablehash/__init__test.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 @dataclass
 class MyDataclass:
     a: int
     b: str
 
 
 class Picklable:
-
     def __init__(self, a: int, b: str) -> None:
         self.a = a
         self.b = b
 
     def __getstate__(self) -> tuple[int, str]:
         return self.a, self.b
```

### Comparing `stablehash-0.1.1/src/stablehash/_tokenize.py` & `stablehash-0.1.2/src/stablehash/_tokenize.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 
 def fqn(x: type[Any]) -> str:
     return f"{x.__module__}.{x.__qualname__}"
 
 
 def tokenize(hasher: "Hasher", x: Any, *, header: bool = True) -> None:
-
     # Produce an opening/ending token to indicate the type of the object being hashed. This is
     # to minimize the chances that consecutive hashes of multiple objects imitate the hash of a
     # single object (e.g. "abc" vs. "ab" + "c"), as well as encoding the actual type of the object.
     if header:
         hasher.update(fqn(type(x)).encode("utf8"))
         hasher.update(b"[")
 
@@ -68,26 +67,23 @@
             raise TypeError(f"object of type {fqn(type(x))} is not consistent-hashable")
 
     if header:
         hasher.update(b"]")
 
 
 class Dataclass(DataclassInstance):
-
     @classmethod
     def __subclasshook__(cls, __subclass: type) -> bool:
         return is_dataclass(__subclass)
 
 
 class Picklable(ABC):
-
     @abc.abstractmethod
     def __getstate__(self) -> Any: ...
 
     @classmethod
     def __subclasshook__(cls, __subclass: type) -> bool:
         return hasattr(__subclass, "__getstate__")
 
 
 class Hasher(Protocol):
-
     def update(self, __data: bytes) -> None: ...
```

### Comparing `stablehash-0.1.1/PKG-INFO` & `stablehash-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,55 @@
 Metadata-Version: 2.1
 Name: stablehash
-Version: 0.1.1
-Summary: Stable hashing of Python data structures spanning invokations and platforms. 
-License: MIT
+Version: 0.1.2
+Summary: Stable hashing of Python data structures across separate processes and platforms.
 Keywords: hash,stable hash,hashlib,dataclasses,python hashing
-Author: Niklas Rosenstein
-Author-email: niklas.rosenstein@helsing.ai
-Requires-Python: >=3.10,<4.0
+Author-Email: Niklas Rosenstein <rosensteinniklas@gmail.com>
+License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
-Project-URL: Bug Tracker, https://github.com/NiklasRosenstein/python-stablehash/issues
 Project-URL: Repository, https://github.com/NiklasRosenstein/python-stablehash
+Project-URL: Issues, https://github.com/NiklasRosenstein/python-stablehash/issues
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # stablehash
 
-The `stablehash` module provides a "pure" hash function that is stable across Python processes and runs. This is in contrast to the builtin `hash()` function, which may return a different value for the same input in separate invokations even with the Python version.
-
-We support most Python built-in types, including mutable types such as `list` and `dict`, as well as dataclasses. The default internal hash algorithm is Blake2b, but this can be changed by passing a different `hashlib` algorithm to the `stablehash` function.
+The `stablehash` module provides a "pure" hash function that is stable across Python processes and runs. This is in
+contrast to the builtin `hash()` function, which may return a different value for the same input in separate
+invokations even with the Python version.
+
+We support most Python built-in types, including mutable types such as `list` and `dict`, as well as dataclasses. The
+default internal hash algorithm is Blake2b, but this can be changed by passing a different `hashlib` algorithm to the
+`stablehash` function.
 
 ## Usage
 
 ```python
 from stablehash import stablehash
 
 assert stablehash({"key": "value"}, algorithm="md5").hexdigest() == 'd5994850379366e314563ea555532052'
 ```
 
 ## API
 
 ### `stablehash(obj=..., *, algorithm="blake2b")`
 
-Returns a `hashlib`-compatible object with the given algorithm and the hash of the given object. The algorithm must be one of the algorithms supported by `hashlib`.
+Returns a `hashlib`-compatible object with the given algorithm and the hash of the given object. The algorithm must be
+one of the algorithms supported by `hashlib`.
 
 ### `stablehash.update(obj)`
 
 Updates the hash with the given object. If the object is not supported, a `TypeError` is raised.
 
 ### `stablehash.digest()`
 
@@ -70,8 +74,7 @@
 - `set`
 - `frozenset`
 - `dict`
 - `@dataclass` objects
 - `datetime` objects (`datetime`, `date`, `time` and `timedelta`)
 - `uuid.UUID`
 - Picklable objects (e.g. those that implement `__getstate__()`)
-
```

