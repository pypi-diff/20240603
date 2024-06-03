# Comparing `tmp/staffspy-0.1.0.tar.gz` & `tmp/staffspy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "staffspy-0.1.0.tar", max compression
+gzip compressed data, was "staffspy-0.1.1.tar", max compression
```

## Comparing `staffspy-0.1.0.tar` & `staffspy-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,9 @@
--rw-r--r--   0        0        0     1069 2024-06-01 18:51:36.162267 staffspy-0.1.0/LICENSE
--rw-r--r--   0        0        0     1503 2024-06-01 18:51:36.162267 staffspy-0.1.0/README.md
--rw-r--r--   0        0        0      406 2024-06-01 18:51:36.162267 staffspy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       39 2024-06-01 18:51:36.162267 staffspy-0.1.0/staffspy/__init__.py
--rw-r--r--   0        0        0     1933 1970-01-01 00:00:00.000000 staffspy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-06-03 05:22:43.493751 staffspy-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2898 2024-06-03 05:22:43.493751 staffspy-0.1.1/README.md
+-rw-r--r--   0        0        0      457 2024-06-03 05:22:43.493751 staffspy-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1044 2024-06-03 05:22:43.493751 staffspy-0.1.1/staffspy/__init__.py
+-rw-r--r--   0        0        0      121 2024-06-03 05:22:43.493751 staffspy-0.1.1/staffspy/exceptions.py
+-rw-r--r--   0        0        0    19294 2024-06-03 05:22:43.493751 staffspy-0.1.1/staffspy/linkedin/__init__.py
+-rw-r--r--   0        0        0     3696 2024-06-03 05:22:43.493751 staffspy-0.1.1/staffspy/models.py
+-rw-r--r--   0        0        0     3656 2024-06-03 05:22:43.493751 staffspy-0.1.1/staffspy/utils.py
+-rw-r--r--   0        0        0     3442 1970-01-01 00:00:00.000000 staffspy-0.1.1/PKG-INFO
```

### Comparing `staffspy-0.1.0/LICENSE` & `staffspy-0.1.1/LICENSE`

 * *Files identical despite different names*

