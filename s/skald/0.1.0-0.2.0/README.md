# Comparing `tmp/skald-0.1.0.tar.gz` & `tmp/skald-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skald-0.1.0.tar", max compression
+gzip compressed data, was "skald-0.2.0.tar", max compression
```

## Comparing `skald-0.1.0.tar` & `skald-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,8 @@
--rw-r--r--   0        0        0     1095 2024-05-03 07:52:57.220545 skald-0.1.0/LICENSE
--rw-r--r--   0        0        0     1862 2024-05-03 08:45:37.989687 skald-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1726 2024-05-03 09:05:25.330541 skald-0.1.0/README.md
--rw-r--r--   0        0        0       83 2024-05-03 07:58:56.827521 skald-0.1.0/skald/__init__.py
--rw-r--r--   0        0        0     2436 1970-01-01 00:00:00.000000 skald-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1095 2024-05-03 07:52:57.220545 skald-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1899 2024-06-03 11:39:30.374980 skald-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5743 2024-06-03 11:29:39.146545 skald-0.2.0/README.md
+-rw-r--r--   0        0        0     9946 2024-06-03 11:24:55.510614 skald-0.2.0/skald/__init__.py
+-rw-r--r--   0        0        0     1174 2024-06-03 11:24:55.509617 skald-0.2.0/skald/enums.py
+-rw-r--r--   0        0        0      281 2024-06-03 11:24:55.509617 skald-0.2.0/skald/exceptions.py
+-rw-r--r--   0        0        0      663 2024-06-03 09:33:22.208578 skald-0.2.0/skald/utils.py
+-rw-r--r--   0        0        0     6457 1970-01-01 00:00:00.000000 skald-0.2.0/PKG-INFO
```

### Comparing `skald-0.1.0/LICENSE` & `skald-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skald-0.1.0/pyproject.toml` & `skald-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "skald"
-version = "0.1.0"
+version = "0.2.0"
 description = "📟 a simple and efficient experiment logger for Python 🐍"
 keywords = ["logging", "tui"]
 authors = ["Laurenz Farthofer <laurenz@hey.com>"]
 repository = "https://github.com/laurenzbeck/skald"
 packages = [{ include = "skald" }]
 license = "MIT"
 readme = "README.md"
@@ -13,15 +13,17 @@
 test = "coverage run --source=skald -m pytest -vv --durations=8"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 rich = "^13.7.1"
 typer = "^0.12.3"
 polars = "^0.20.23"
+pandas = "^2.2.2"
 beartype = "^0.18.5"
+loguru = "^0.7.2"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.4.2"
 mkdocs = "^1.6.0"
 mkdocs-material = "^9.5.20"
 towncrier = "^23.11.0"
 pre-commit = "^3.7.0"
@@ -67,12 +69,12 @@
 directory = "fixed"
 name = "🐛 Fixed"
 showcontent = true
 
 [[tool.towncrier.type]]
 directory = "misc"
 name = "📦 Misc"
-showcontent = false
+showcontent = true
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

