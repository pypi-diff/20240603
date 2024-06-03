# Comparing `tmp/stablehash-0.1.2.tar.gz` & `tmp/stablehash-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stablehash-0.1.2.tar", last modified: Mon Jun  3 00:55:24 2024, max compression
+gzip compressed data, was "stablehash-0.1.3.tar", last modified: Mon Jun  3 01:14:50 2024, max compression
```

## Comparing `stablehash-0.1.2.tar` & `stablehash-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      998 2024-06-03 00:35:50.749729 stablehash-0.1.2/LICENSE
--rw-r--r--   0        0        0     1546 2024-06-03 00:35:50.749729 stablehash-0.1.2/README.md
--rw-r--r--   0        0        0     1674 2024-06-03 00:55:24.973818 stablehash-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      981 2024-06-03 00:53:32.930936 stablehash-0.1.2/src/stablehash/__init__.py
--rw-r--r--   0        0        0     2022 2024-06-03 00:53:21.771050 stablehash-0.1.2/src/stablehash/__init__test.py
--rw-r--r--   0        0        0     2987 2024-06-03 00:53:21.771050 stablehash-0.1.2/src/stablehash/_tokenize.py
--rw-r--r--   0        0        0        0 2024-06-03 00:35:50.749729 stablehash-0.1.2/src/stablehash/py.typed
--rw-r--r--   0        0        0     2658 1970-01-01 00:00:00.000000 stablehash-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      998 2024-06-03 00:35:50.749729 stablehash-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1546 2024-06-03 00:35:50.749729 stablehash-0.1.3/README.md
+-rw-r--r--   0        0        0     1695 2024-06-03 01:14:50.418244 stablehash-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      981 2024-06-03 01:14:09.610654 stablehash-0.1.3/src/stablehash/__init__.py
+-rw-r--r--   0        0        0     2210 2024-06-03 01:12:26.135694 stablehash-0.1.3/src/stablehash/__init__test.py
+-rw-r--r--   0        0        0     3053 2024-06-03 01:12:26.135694 stablehash-0.1.3/src/stablehash/_tokenize.py
+-rw-r--r--   0        0        0        0 2024-06-03 00:35:50.749729 stablehash-0.1.3/src/stablehash/py.typed
+-rw-r--r--   0        0        0     2658 1970-01-01 00:00:00.000000 stablehash-0.1.3/PKG-INFO
```

### Comparing `stablehash-0.1.2/LICENSE` & `stablehash-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stablehash-0.1.2/README.md` & `stablehash-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `stablehash-0.1.2/pyproject.toml` & `stablehash-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "stablehash"
-version = "0.1.2"
+version = "0.1.3"
 description = "Stable hashing of Python data structures across separate processes and platforms."
 authors = [
     { name = "Niklas Rosenstein", email = "rosensteinniklas@gmail.com" },
 ]
 dependencies = []
 requires-python = ">=3.10"
 readme = "README.md"
@@ -46,14 +46,15 @@
 [tool.pdm]
 distribution = true
 
 [tool.pdm.dev-dependencies]
 dev = [
     "mypy>=1.10.0",
     "ruff>=0.4.7",
+    "pytest>=8.2.1",
 ]
 
 [tool.mypy]
 python_version = "3.10"
 explicit_package_bases = true
 mypy_path = [
     "src",
```

### Comparing `stablehash-0.1.2/src/stablehash/__init__.py` & `stablehash-0.1.3/src/stablehash/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 
 import hashlib
 from typing import Any
 
 from ._tokenize import tokenize
 
 _sentinel = object()
```

### Comparing `stablehash-0.1.2/src/stablehash/__init__test.py` & `stablehash-0.1.3/src/stablehash/__init__test.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,7 +37,9 @@
     assert stablehash(date(2021, 1, 1), algorithm="md5").hexdigest() == "a8d008bc6c73f527333b3d40726c7e1f"
     assert stablehash(time(0, 0, 0), algorithm="md5").hexdigest() == "531c98aced815358bb7375c5948d0d82"
     assert stablehash(timedelta(seconds=1), algorithm="md5").hexdigest() == "e5fe3b7bf1b4ca1fb9ba5bfe886fbff5"
     assert (
         stablehash(UUID("00000000-0000-0000-0000-000000000000"), algorithm="md5").hexdigest()
         == "34fa1fac0804eaebe1a8a3adce7cef3f"
     )
+    assert stablehash(int, algorithm="md5").hexdigest() == "21a85b46a16a64f9c58f5402c4c11bf1"
+    assert stablehash(str, algorithm="md5").hexdigest() == "fc1830dca524be291dcda6dbca7bd509"
```

### Comparing `stablehash-0.1.2/src/stablehash/_tokenize.py` & `stablehash-0.1.3/src/stablehash/_tokenize.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,16 +59,18 @@
             tokenize(hasher, x.isoformat(), header=False)
         case timedelta():
             tokenize(hasher, x.total_seconds(), header=False)
         case UUID():
             tokenize(hasher, x.int, header=False)
         case Picklable():
             tokenize(hasher, x.__getstate__())
+        case type():
+            hasher.update(fqn(x).encode("utf8"))
         case _:
-            raise TypeError(f"object of type {fqn(type(x))} is not consistent-hashable")
+            raise TypeError(f"object of type {fqn(type(x))} is not stable-hashable")
 
     if header:
         hasher.update(b"]")
 
 
 class Dataclass(DataclassInstance):
     @classmethod
```

### Comparing `stablehash-0.1.2/PKG-INFO` & `stablehash-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stablehash
-Version: 0.1.2
+Version: 0.1.3
 Summary: Stable hashing of Python data structures across separate processes and platforms.
 Keywords: hash,stable hash,hashlib,dataclasses,python hashing
 Author-Email: Niklas Rosenstein <rosensteinniklas@gmail.com>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

