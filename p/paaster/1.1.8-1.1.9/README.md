# Comparing `tmp/paaster-1.1.8.tar.gz` & `tmp/paaster-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paaster-1.1.8.tar", max compression
+gzip compressed data, was "paaster-1.1.9.tar", max compression
```

## Comparing `paaster-1.1.8.tar` & `paaster-1.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-12-04 06:17:35.437155 paaster-1.1.8/LICENSE
--rw-r--r--   0        0        0     1060 2023-12-04 06:17:35.437155 paaster-1.1.8/README.md
--rw-r--r--   0        0        0     4188 2023-12-04 06:17:35.437155 paaster-1.1.8/paaster_cli/__init__.py
--rw-r--r--   0        0        0      332 2023-12-04 06:17:35.437155 paaster-1.1.8/paaster_cli/misc.py
--rw-r--r--   0        0        0     1445 2023-12-04 06:17:35.437155 paaster-1.1.8/paaster_cli/storage.py
--rw-r--r--   0        0        0      522 2023-12-04 06:17:35.441155 paaster-1.1.8/pyproject.toml
--rw-r--r--   0        0        0     1771 1970-01-01 00:00:00.000000 paaster-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-12 06:03:14.521216 paaster-1.1.9/LICENSE
+-rw-r--r--   0        0        0     1060 2024-04-12 06:03:14.521216 paaster-1.1.9/README.md
+-rw-r--r--   0        0        0     4188 2024-04-12 06:03:14.521216 paaster-1.1.9/paaster_cli/__init__.py
+-rw-r--r--   0        0        0      332 2024-04-12 06:03:14.521216 paaster-1.1.9/paaster_cli/misc.py
+-rw-r--r--   0        0        0     1445 2024-04-12 06:03:14.525216 paaster-1.1.9/paaster_cli/storage.py
+-rw-r--r--   0        0        0      522 2024-04-12 06:03:14.525216 paaster-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1771 1970-01-01 00:00:00.000000 paaster-1.1.9/PKG-INFO
```

### Comparing `paaster-1.1.8/LICENSE` & `paaster-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `paaster-1.1.8/README.md` & `paaster-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `paaster-1.1.8/paaster_cli/__init__.py` & `paaster-1.1.9/paaster_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `paaster-1.1.8/paaster_cli/storage.py` & `paaster-1.1.9/paaster_cli/storage.py`

 * *Files identical despite different names*

### Comparing `paaster-1.1.8/pyproject.toml` & `paaster-1.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "paaster"
-version = "1.1.8"
+version = "1.1.9"
 description = "Upload locally encrypted pastes from your terminal to Paaster"
 authors = ["WardPearce <wardpearce@protonmail.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 packages = [{include = "paaster_cli"}]
 
 [tool.poetry.dependencies]
```

### Comparing `paaster-1.1.8/PKG-INFO` & `paaster-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paaster
-Version: 1.1.8
+Version: 1.1.9
 Summary: Upload locally encrypted pastes from your terminal to Paaster
 License: GPL-3.0
 Author: WardPearce
 Author-email: wardpearce@protonmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

