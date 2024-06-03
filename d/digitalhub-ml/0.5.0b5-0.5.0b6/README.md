# Comparing `tmp/digitalhub_ml-0.5.0b5.tar.gz` & `tmp/digitalhub_ml-0.5.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitalhub_ml-0.5.0b5.tar", last modified: Wed May 29 09:49:00 2024, max compression
+gzip compressed data, was "digitalhub_ml-0.5.0b6.tar", last modified: Mon Jun  3 07:26:32 2024, max compression
```

## Comparing `digitalhub_ml-0.5.0b5.tar` & `digitalhub_ml-0.5.0b6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-29 09:49:00.317700 digitalhub_ml-0.5.0b5/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)      946 2024-05-29 09:49:00.317700 digitalhub_ml-0.5.0b5/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      462 2024-04-23 09:36:04.000000 digitalhub_ml-0.5.0b5/README.md
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-29 09:49:00.317700 digitalhub_ml-0.5.0b5/digitalhub_ml/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      304 2024-05-27 14:03:58.000000 digitalhub_ml-0.5.0b5/digitalhub_ml/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-29 09:49:00.317700 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:38:37.000000 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      436 2024-05-06 11:22:14.000000 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/entity_types.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-29 09:49:00.317700 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/models/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:40:22.000000 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/models/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6328 2024-05-27 14:03:58.000000 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/models/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    12482 2024-05-28 10:51:37.000000 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/models/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      318 2024-04-23 09:36:04.000000 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/models/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1427 2024-05-28 09:49:46.000000 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/models/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      300 2024-05-28 09:45:24.000000 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/models/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-29 09:49:00.317700 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/projects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:33:48.000000 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/projects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6049 2024-05-27 14:03:58.000000 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/projects/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5869 2024-05-27 14:03:58.000000 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/projects/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      988 2024-05-27 14:03:58.000000 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/projects/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      730 2024-05-06 11:19:46.000000 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/registries.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-29 09:49:00.317700 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/runs/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-23 14:34:03.000000 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/runs/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      300 2024-03-07 13:39:55.000000 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/runs/models.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      405 2024-05-27 14:03:58.000000 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/runs/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      313 2024-03-14 13:46:16.000000 digitalhub_ml-0.5.0b5/digitalhub_ml/entities/runs/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-29 09:49:00.317700 digitalhub_ml-0.5.0b5/digitalhub_ml.egg-info/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)      946 2024-05-29 09:49:00.000000 digitalhub_ml-0.5.0b5/digitalhub_ml.egg-info/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      903 2024-05-29 09:49:00.000000 digitalhub_ml-0.5.0b5/digitalhub_ml.egg-info/SOURCES.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-05-29 09:49:00.000000 digitalhub_ml-0.5.0b5/digitalhub_ml.egg-info/dependency_links.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       29 2024-05-29 09:49:00.000000 digitalhub_ml-0.5.0b5/digitalhub_ml.egg-info/requires.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       19 2024-05-29 09:49:00.000000 digitalhub_ml-0.5.0b5/digitalhub_ml.egg-info/top_level.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1063 2024-05-28 11:34:48.000000 digitalhub_ml-0.5.0b5/pyproject.toml
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-05-29 09:49:00.317700 digitalhub_ml-0.5.0b5/setup.cfg
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-06-03 07:26:32.129791 digitalhub_ml-0.5.0b6/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)      946 2024-06-03 07:26:32.129791 digitalhub_ml-0.5.0b6/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      462 2024-04-23 09:36:04.000000 digitalhub_ml-0.5.0b6/README.md
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-06-03 07:26:32.125791 digitalhub_ml-0.5.0b6/digitalhub_ml/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      304 2024-05-30 06:51:20.000000 digitalhub_ml-0.5.0b6/digitalhub_ml/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-06-03 07:26:32.129791 digitalhub_ml-0.5.0b6/digitalhub_ml/entities/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:38:37.000000 digitalhub_ml-0.5.0b6/digitalhub_ml/entities/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      436 2024-05-06 11:22:14.000000 digitalhub_ml-0.5.0b6/digitalhub_ml/entities/entity_types.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-06-03 07:26:32.129791 digitalhub_ml-0.5.0b6/digitalhub_ml/entities/models/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:40:22.000000 digitalhub_ml-0.5.0b6/digitalhub_ml/entities/models/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6328 2024-05-30 06:51:22.000000 digitalhub_ml-0.5.0b6/digitalhub_ml/entities/models/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    12482 2024-05-30 06:51:22.000000 digitalhub_ml-0.5.0b6/digitalhub_ml/entities/models/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      318 2024-04-23 09:36:04.000000 digitalhub_ml-0.5.0b6/digitalhub_ml/entities/models/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1497 2024-05-30 07:12:14.000000 digitalhub_ml-0.5.0b6/digitalhub_ml/entities/models/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      301 2024-05-29 13:44:18.000000 digitalhub_ml-0.5.0b6/digitalhub_ml/entities/models/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-06-03 07:26:32.129791 digitalhub_ml-0.5.0b6/digitalhub_ml/entities/projects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:33:48.000000 digitalhub_ml-0.5.0b6/digitalhub_ml/entities/projects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6049 2024-05-30 06:51:21.000000 digitalhub_ml-0.5.0b6/digitalhub_ml/entities/projects/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5869 2024-05-30 06:51:21.000000 digitalhub_ml-0.5.0b6/digitalhub_ml/entities/projects/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      988 2024-05-30 06:51:21.000000 digitalhub_ml-0.5.0b6/digitalhub_ml/entities/projects/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      730 2024-05-06 11:19:46.000000 digitalhub_ml-0.5.0b6/digitalhub_ml/entities/registries.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-06-03 07:26:32.129791 digitalhub_ml-0.5.0b6/digitalhub_ml/entities/runs/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-23 14:34:03.000000 digitalhub_ml-0.5.0b6/digitalhub_ml/entities/runs/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      300 2024-03-07 13:39:55.000000 digitalhub_ml-0.5.0b6/digitalhub_ml/entities/runs/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      405 2024-05-30 06:51:21.000000 digitalhub_ml-0.5.0b6/digitalhub_ml/entities/runs/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      313 2024-03-14 13:46:16.000000 digitalhub_ml-0.5.0b6/digitalhub_ml/entities/runs/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-06-03 07:26:32.129791 digitalhub_ml-0.5.0b6/digitalhub_ml.egg-info/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)      946 2024-06-03 07:26:32.000000 digitalhub_ml-0.5.0b6/digitalhub_ml.egg-info/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      903 2024-06-03 07:26:32.000000 digitalhub_ml-0.5.0b6/digitalhub_ml.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-06-03 07:26:32.000000 digitalhub_ml-0.5.0b6/digitalhub_ml.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       29 2024-06-03 07:26:32.000000 digitalhub_ml-0.5.0b6/digitalhub_ml.egg-info/requires.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       19 2024-06-03 07:26:32.000000 digitalhub_ml-0.5.0b6/digitalhub_ml.egg-info/top_level.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1063 2024-06-03 07:25:28.000000 digitalhub_ml-0.5.0b6/pyproject.toml
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-06-03 07:26:32.129791 digitalhub_ml-0.5.0b6/setup.cfg
```

### Comparing `digitalhub_ml-0.5.0b5/PKG-INFO` & `digitalhub_ml-0.5.0b6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub-ml
-Version: 0.5.0b5
+Version: 0.5.0b6
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 Keywords: data,dataops,kubernetes
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
```

### Comparing `digitalhub_ml-0.5.0b5/digitalhub_ml/entities/models/crud.py` & `digitalhub_ml-0.5.0b6/digitalhub_ml/entities/models/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.5.0b5/digitalhub_ml/entities/models/entity.py` & `digitalhub_ml-0.5.0b6/digitalhub_ml/entities/models/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.5.0b5/digitalhub_ml/entities/models/spec.py` & `digitalhub_ml-0.5.0b6/digitalhub_ml/entities/models/spec.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,18 +7,21 @@
 
 
 class ModelSpec(Spec):
     """
     Model specifications.
     """
 
-    def __init__(self, path: str | None = None,
-                 framework: str | None = None,
-                 algorithm: str | None = None,
-                 **kwargs,) -> None:
+    def __init__(
+        self,
+        path: str | None = None,
+        framework: str | None = None,
+        algorithm: str | None = None,
+        **kwargs,
+    ) -> None:
         """
         Constructor.
         """
 
         self.path = path
         self.framework = framework
         self.algorithm = algorithm
@@ -65,11 +68,14 @@
 
 class ModelParamsModel(ModelParams):
     """
     Model parameters.
     """
 
     base_model: str = None
+    """Base model."""
 
     parameters: dict = None
+    """Model parameters."""
 
     metrics: dict = None
+    """Model metrics."""
```

### Comparing `digitalhub_ml-0.5.0b5/digitalhub_ml/entities/projects/crud.py` & `digitalhub_ml-0.5.0b6/digitalhub_ml/entities/projects/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.5.0b5/digitalhub_ml/entities/projects/entity.py` & `digitalhub_ml-0.5.0b6/digitalhub_ml/entities/projects/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.5.0b5/digitalhub_ml/entities/projects/spec.py` & `digitalhub_ml-0.5.0b6/digitalhub_ml/entities/projects/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.5.0b5/digitalhub_ml/entities/registries.py` & `digitalhub_ml-0.5.0b6/digitalhub_ml/entities/registries.py`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.5.0b5/digitalhub_ml.egg-info/PKG-INFO` & `digitalhub_ml-0.5.0b6/digitalhub_ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub-ml
-Version: 0.5.0b5
+Version: 0.5.0b6
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 Keywords: data,dataops,kubernetes
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
```

### Comparing `digitalhub_ml-0.5.0b5/digitalhub_ml.egg-info/SOURCES.txt` & `digitalhub_ml-0.5.0b6/digitalhub_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.5.0b5/pyproject.toml` & `digitalhub_ml-0.5.0b6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digitalhub-ml"
-version = "0.5.0b5"
+version = "0.5.0b6"
 description = "Python SDK for DHCore"
 readme = "README.md"
 authors = [
     { name = "Fondazione Bruno Kessler", email = "dslab@fbk.eu" },
     { name = "Matteo Martini", email = "mmartini@fbk.eu" }
 ]
 license = { file = "LICENSE.txt" }
@@ -23,15 +23,15 @@
     "digitalhub-data~=0.5.0b, <0.6",
 ]
 
 [tool.setuptools.packages.find]
 exclude = ["modules*"]
 
 [tool.bumpver]
-current_version = "0.5.0b5"
+current_version = "0.5.0b6"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = false
 tag             = false
 push            = false
 
 [tool.bumpver.file_patterns]
```

