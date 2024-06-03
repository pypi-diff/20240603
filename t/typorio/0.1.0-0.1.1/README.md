# Comparing `tmp/typorio-0.1.0.tar.gz` & `tmp/typorio-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typorio-0.1.0.tar", max compression
+gzip compressed data, was "typorio-0.1.1.tar", max compression
```

## Comparing `typorio-0.1.0.tar` & `typorio-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,11 @@
--rw-r--r--   0        0        0        0 2024-05-29 13:39:02.093207 typorio-0.1.0/README.md
--rw-r--r--   0        0        0      288 2024-05-29 13:39:45.841679 typorio-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-29 13:39:02.093207 typorio-0.1.0/typorio/__init__.py
--rw-r--r--   0        0        0      430 1970-01-01 00:00:00.000000 typorio-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-29 13:39:02.093207 typorio-0.1.1/README.md
+-rw-r--r--   0        0        0      456 2024-06-03 09:50:06.594865 typorio-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-29 14:11:08.015867 typorio-0.1.1/typorio/__init__.py
+-rw-r--r--   0        0        0       28 2024-06-02 11:08:30.605338 typorio-0.1.1/typorio/core/__init__.py
+-rw-r--r--   0        0        0     2063 2024-06-03 05:07:59.222404 typorio-0.1.1/typorio/core/commands.py
+-rw-r--r--   0        0        0      109 2024-06-03 01:52:16.961897 typorio-0.1.1/typorio/core/constants.py
+-rw-r--r--   0        0        0       86 2024-06-03 02:33:47.535641 typorio-0.1.1/typorio/core/models.py
+-rw-r--r--   0        0        0     5473 2024-06-03 09:49:25.631722 typorio-0.1.1/typorio/core/worker.py
+-rw-r--r--   0        0        0      304 2024-06-02 11:08:30.605338 typorio-0.1.1/typorio/main.py
+-rw-r--r--   0        0        0      252 2024-06-02 15:24:08.540873 typorio-0.1.1/typorio/utils/__init__.py
+-rw-r--r--   0        0        0      589 1970-01-01 00:00:00.000000 typorio-0.1.1/PKG-INFO
```

