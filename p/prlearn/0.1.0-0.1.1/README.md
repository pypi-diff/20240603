# Comparing `tmp/prlearn-0.1.0.tar.gz` & `tmp/prlearn-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prlearn-0.1.0.tar", max compression
+gzip compressed data, was "prlearn-0.1.1.tar", max compression
```

## Comparing `prlearn-0.1.0.tar` & `prlearn-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,21 @@
--rw-r--r--   0        0        0        0 2024-05-13 22:29:40.112633 prlearn-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-13 22:29:40.112518 prlearn-0.1.0/prlearn/__init__.py
--rw-r--r--   0        0        0      274 2024-05-13 22:33:31.281372 prlearn-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      295 1970-01-01 00:00:00.000000 prlearn-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2648 2024-06-03 13:29:44.230200 prlearn-0.1.1/README.md
+-rw-r--r--   0        0        0      328 2024-06-03 13:25:48.152357 prlearn-0.1.1/prlearn/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 04:05:19.314237 prlearn-0.1.1/prlearn/base/__init__.py
+-rw-r--r--   0        0        0      439 2024-06-03 00:41:33.044014 prlearn-0.1.1/prlearn/base/agent.py
+-rw-r--r--   0        0        0     1322 2024-06-03 13:21:58.612196 prlearn-0.1.1/prlearn/base/agent_combiner.py
+-rw-r--r--   0        0        0      568 2024-06-03 00:41:39.265172 prlearn-0.1.1/prlearn/base/environment.py
+-rw-r--r--   0        0        0     4399 2024-06-03 12:38:49.227503 prlearn-0.1.1/prlearn/base/experience.py
+-rw-r--r--   0        0        0    15287 2024-06-03 13:47:45.416867 prlearn-0.1.1/prlearn/base/trainer.py
+-rw-r--r--   0        0        0    12008 2024-06-03 13:43:44.936237 prlearn-0.1.1/prlearn/base/worker.py
+-rw-r--r--   0        0        0        0 2024-06-03 13:21:10.640434 prlearn-0.1.1/prlearn/collection/__init__.py
+-rw-r--r--   0        0        0     3787 2024-06-03 13:23:51.479467 prlearn-0.1.1/prlearn/collection/agent_combiners.py
+-rw-r--r--   0        0        0        0 2024-05-20 04:04:49.405597 prlearn-0.1.1/prlearn/common/__init__.py
+-rw-r--r--   0        0        0      124 2024-06-03 08:38:23.391077 prlearn-0.1.1/prlearn/common/config.py
+-rw-r--r--   0        0        0     1383 2024-06-03 00:25:01.691305 prlearn-0.1.1/prlearn/common/dataclasses.py
+-rw-r--r--   0        0        0     6335 2024-06-03 13:03:09.868813 prlearn-0.1.1/prlearn/common/pas.py
+-rw-r--r--   0        0        0        0 2024-05-13 22:18:29.935032 prlearn-0.1.1/prlearn/utils/__init__.py
+-rw-r--r--   0        0        0      345 2024-06-03 13:42:15.063365 prlearn-0.1.1/prlearn/utils/logger.py
+-rw-r--r--   0        0        0      781 2024-06-03 08:57:24.605186 prlearn-0.1.1/prlearn/utils/message_utils.py
+-rw-r--r--   0        0        0       88 2024-06-01 00:41:51.671228 prlearn-0.1.1/prlearn/utils/multiproc_lib.py
+-rw-r--r--   0        0        0      439 2024-06-03 14:04:02.170451 prlearn-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3046 1970-01-01 00:00:00.000000 prlearn-0.1.1/PKG-INFO
```

