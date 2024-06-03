# Comparing `tmp/struuuctify-0.0.1.tar.gz` & `tmp/struuuctify-0.0.4.tar.gz`

## Comparing `struuuctify-0.0.1.tar` & `struuuctify-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,17 @@
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 struuuctify-0.0.1/.github/workflows/python-linter.yml
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 struuuctify-0.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 struuuctify-0.0.1/src/struuuctify/__init__.py
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 struuuctify-0.0.1/src/struuuctify/_structify.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 struuuctify-0.0.1/src/struuuctify/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 struuuctify-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 struuuctify-0.0.1/tests/conftest.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 struuuctify-0.0.1/tests/incorrect_function.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 struuuctify-0.0.1/tests/test_structify.py
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 struuuctify-0.0.1/LICENSE
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 struuuctify-0.0.1/README.md
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 struuuctify-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 struuuctify-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 struuuctify-0.0.4/.cruft.json
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 struuuctify-0.0.4/.dockerignore
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 struuuctify-0.0.4/noxfile.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 struuuctify-0.0.4/.github/workflows/python-linter.yml
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 struuuctify-0.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 struuuctify-0.0.4/src/structify/__init__.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 struuuctify-0.0.4/src/structify/_structify.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 struuuctify-0.0.4/src/structify/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 struuuctify-0.0.4/src/structify/py.typed
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 struuuctify-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 struuuctify-0.0.4/tests/incorrect_function.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 struuuctify-0.0.4/tests/test_structify.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 struuuctify-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 struuuctify-0.0.4/LICENSE
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 struuuctify-0.0.4/README.md
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 struuuctify-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 struuuctify-0.0.4/PKG-INFO
```

### Comparing `struuuctify-0.0.1/.github/workflows/python-linter.yml` & `struuuctify-0.0.4/.github/workflows/python-linter.yml`

 * *Files 14% similar despite different names*

```diff
@@ -24,15 +24,14 @@
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install -e .[dev]
-        if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
     - name: Mypy strict
       run: |
         # stop the build if there are Python syntax errors or undefined names
         mypy --strict .
     - name: ruff
       run: |
         ruff .
```

### Comparing `struuuctify-0.0.1/.github/workflows/python-publish.yml` & `struuuctify-0.0.4/.github/workflows/python-publish.yml`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     name: Publish Python 🐍 distribution 📦 to TestPyPI
     needs:
     - build-package
     runs-on: ubuntu-latest
 
     environment:
       name: testpypi
-      url: https://test.pypi.org/p/struct-ify
+      url: https://test.pypi.org/p/struuuctify
 
     permissions:
       id-token: write  # IMPORTANT: mandatory for trusted publishing
 
     steps:
     - name: Download all the dists
       uses: actions/download-artifact@v3
@@ -75,19 +75,19 @@
       Publish Python 🐍 distribution 📦 to PyPI
     if: startsWith(github.ref, 'refs/tags/')  # only publish to PyPI on tag pushes
     needs:
     - build-package
     runs-on: ubuntu-latest
     environment:
       name: pypi
-      url: https://pypi.org/p/struct-ify
+      url: https://pypi.org/p/struuuctify
     permissions:
       id-token: write  # IMPORTANT: mandatory for trusted publishing
 
     steps:
     - name: Download all the dists
       uses: actions/download-artifact@v3
       with:
         name: python-package-distributions
         path: dist/
     - name: Publish distribution 📦 to PyPI
-      uses: pypa/gh-action-pypi-publish@release/v1
+      uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `struuuctify-0.0.1/src/struuuctify/_structify.py` & `struuuctify-0.0.4/src/structify/_structify.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 from dataclasses import dataclass
 from functools import partial
 import inspect
-from typing import Callable, Protocol, Any, TypeVar, dataclass_transform
+from typing import Callable, Protocol, Any, TypeVar, dataclass_transform, final
 
 
 class _Method(Protocol):
     __name__: str
 
     def __call__(self, *args: Any, **kwargs: Any) -> Any: ...
 
 
-class _struuuctifyCls(Protocol):
+class _StruuuctifyCls(Protocol):
     __struuuctify__: dict[str, _Method]
 
 
-def _struct_get_attr(self: _struuuctifyCls, item: str) -> Callable[..., Any]:
+def _struct_get_attr(self: _StruuuctifyCls, item: str) -> Callable[..., Any]:
     method = self.__struuuctify__.get(item, None)
     if method is None:
-        print(dir(self))
         raise AttributeError(f"'{self.__class__.__name__}' object has no attribute '{item}'")
     return partial(method, self)
 
 
 T = TypeVar("T")
 
 
 @dataclass_transform()
 def struct(cls: type[T]) -> type[T]:
     setattr(cls, "__struuuctify__", {})
 
     setattr(cls, "__getattr__", _struct_get_attr)
-    return dataclass(cls)
+    return final(dataclass(cls))
 
 
 def impl(func: _Method) -> Callable[..., Any]:
     cls = func.__annotations__.get("self")
     if cls is None or not inspect.isclass(cls):
-        raise TypeError("self attribute should be a struct")
+        raise TypeError("self attribute should be a struct class")
 
-    print(func.__name__)
     cls.__struuuctify__[func.__name__] = func
     return func
```

### Comparing `struuuctify-0.0.1/tests/test_structify.py` & `struuuctify-0.0.4/tests/test_structify.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Callable, Any
 
 import pytest
 
-from struuuctify import struct, impl
+from structify import struct, impl
 from .incorrect_function import add_1, add_2
 
 
 def test_struuuctify() -> None:
     @struct
     class Point:
         x: float
```

### Comparing `struuuctify-0.0.1/LICENSE` & `struuuctify-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `struuuctify-0.0.1/pyproject.toml` & `struuuctify-0.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
-requires = ["hatchling", "hatch-vcs"]
+requires = ["hatchling>=1.24.2"]
 build-backend = "hatchling.build"
 
 [project]
 name = "struuuctify"
 authors = [
   { name="halbow" },
 ]
-version = "0.0.1"
 requires-python = ">=3.11"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
+    "Typing :: Typed",
 ]
-#dynamic = ["version"]
 
+dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/halbow/structify"
 "Bug Tracker" = "https://github.com/halbow/structify/issues"
 
 
 [project.optional-dependencies]
@@ -28,29 +28,26 @@
     "mypy",
     "pytest",
     "pytest-cov",
     "ruff",
 ]
 
 [tool.hatch.version]
-source = "vcs"
-raw-options = { local_scheme = "no-local-version" }
+path = "src/structify/_version.py"
 
-[tool.hatch.build.hooks.vcs]
-version-file = "src/struuuctify/_version.py"
-template = '''
-version = "{version}"
-'''
+
+[tool.hatch.build.targets.wheel]
+packages = ["src/structify"]
 
 [tool.ruff]
 line-length = 120
-target-version = 'py312'
+target-version = 'py311'
 
 [tool.ruff.lint.isort]
-known-local-folder=["struuuctify", "tests"]
+known-local-folder=["structify", "tests"]
 
 [tool.mypy]
-python_version = "3.12"
+python_version = "3.11"
 strict = true
 show_error_codes = true
```

