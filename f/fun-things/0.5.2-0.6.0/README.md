# Comparing `tmp/fun_things-0.5.2.tar.gz` & `tmp/fun_things-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fun_things-0.5.2.tar", max compression
+gzip compressed data, was "fun_things-0.6.0.tar", max compression
```

## Comparing `fun_things-0.5.2.tar` & `fun_things-0.6.0.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0        0 2024-04-15 03:49:51.312592 fun_things-0.5.2/README.md
--rw-r--r--   0        0        0      120 2024-05-16 00:42:36.895945 fun_things-0.5.2/fun_things/__init__.py
--rw-r--r--   0        0        0      330 2024-04-30 06:36:45.297965 fun_things-0.5.2/fun_things/generic_json_encoder.py
--rw-r--r--   0        0        0     1268 2024-04-17 08:24:16.933684 fun_things-0.5.2/fun_things/lazy.py
--rw-r--r--   0        0        0       57 2024-05-16 00:42:22.693915 fun_things-0.5.2/fun_things/math/__init__.py
--rw-r--r--   0        0        0     1184 2024-05-16 07:11:57.946887 fun_things-0.5.2/fun_things/math/weighted_distribution.py
--rw-r--r--   0        0        0     1193 2024-05-13 02:47:22.745222 fun_things-0.5.2/fun_things/proxy_uri.py
--rw-r--r--   0        0        0      277 2024-05-16 07:12:25.767262 fun_things-0.5.2/pyproject.toml
--rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 fun_things-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-15 03:49:51.312592 fun_things-0.6.0/README.md
+-rw-r--r--   0        0        0      190 2024-06-03 00:47:14.503818 fun_things-0.6.0/fun_things/__init__.py
+-rw-r--r--   0        0        0      330 2024-04-30 06:36:45.297965 fun_things-0.6.0/fun_things/generic_json_encoder.py
+-rw-r--r--   0        0        0     1268 2024-04-17 08:24:16.933684 fun_things-0.6.0/fun_things/lazy.py
+-rw-r--r--   0        0        0       57 2024-05-16 00:42:22.693915 fun_things-0.6.0/fun_things/math/__init__.py
+-rw-r--r--   0        0        0     1184 2024-05-16 07:11:57.946887 fun_things-0.6.0/fun_things/math/weighted_distribution.py
+-rw-r--r--   0        0        0     1193 2024-05-13 02:47:22.745222 fun_things-0.6.0/fun_things/proxy_uri.py
+-rw-r--r--   0        0        0     1450 2024-06-03 00:47:50.735439 fun_things-0.6.0/fun_things/retry.py
+-rw-r--r--   0        0        0      447 2024-05-29 08:17:51.671950 fun_things-0.6.0/fun_things/type.py
+-rw-r--r--   0        0        0      277 2024-06-03 00:49:37.606601 fun_things-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 fun_things-0.6.0/PKG-INFO
```

### Comparing `fun_things-0.5.2/fun_things/lazy.py` & `fun_things-0.6.0/fun_things/lazy.py`

 * *Files identical despite different names*

### Comparing `fun_things-0.5.2/fun_things/math/weighted_distribution.py` & `fun_things-0.6.0/fun_things/math/weighted_distribution.py`

 * *Files identical despite different names*

### Comparing `fun_things-0.5.2/fun_things/proxy_uri.py` & `fun_things-0.6.0/fun_things/proxy_uri.py`

 * *Files identical despite different names*

