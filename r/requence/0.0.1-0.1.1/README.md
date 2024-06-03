# Comparing `tmp/requence-0.0.1.tar.gz` & `tmp/requence-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requence-0.0.1.tar", last modified: Tue May 21 12:55:55 2024, max compression
+gzip compressed data, was "requence-0.1.1.tar", last modified: Mon Jun  3 13:05:47 2024, max compression
```

## Comparing `requence-0.0.1.tar` & `requence-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,21 @@
-drwxr-xr-x   0 torstenblindert   (502) staff       (20)        0 2024-05-21 12:55:55.348310 requence-0.0.1/
--rw-r--r--   0 torstenblindert   (502) staff       (20)       89 2024-04-15 10:33:16.000000 requence-0.0.1/MANIFEST.in
--rw-r--r--   0 torstenblindert   (502) staff       (20)      320 2024-05-21 12:55:55.348149 requence-0.0.1/PKG-INFO
--rw-r--r--   0 torstenblindert   (502) staff       (20)       89 2024-05-07 13:32:20.000000 requence-0.0.1/README.md
--rw-r--r--   0 torstenblindert   (502) staff       (20)      105 2024-04-15 10:23:29.000000 requence-0.0.1/pyproject.toml
-drwxr-xr-x   0 torstenblindert   (502) staff       (20)        0 2024-05-21 12:55:55.347145 requence-0.0.1/requence/
--rw-r--r--   0 torstenblindert   (502) staff       (20)        0 2024-05-21 12:07:25.000000 requence-0.0.1/requence/__init__.py
--rw-r--r--   0 torstenblindert   (502) staff       (20)     9975 2024-05-21 12:07:14.000000 requence-0.0.1/requence/consumer.py
-drwxr-xr-x   0 torstenblindert   (502) staff       (20)        0 2024-05-21 12:55:55.348002 requence-0.0.1/requence.egg-info/
--rw-r--r--   0 torstenblindert   (502) staff       (20)      320 2024-05-21 12:55:55.000000 requence-0.0.1/requence.egg-info/PKG-INFO
--rw-r--r--   0 torstenblindert   (502) staff       (20)      246 2024-05-21 12:55:55.000000 requence-0.0.1/requence.egg-info/SOURCES.txt
--rw-r--r--   0 torstenblindert   (502) staff       (20)        1 2024-05-21 12:55:55.000000 requence-0.0.1/requence.egg-info/dependency_links.txt
--rw-r--r--   0 torstenblindert   (502) staff       (20)       26 2024-05-21 12:55:55.000000 requence-0.0.1/requence.egg-info/requires.txt
--rw-r--r--   0 torstenblindert   (502) staff       (20)        9 2024-05-21 12:55:55.000000 requence-0.0.1/requence.egg-info/top_level.txt
--rw-r--r--   0 torstenblindert   (502) staff       (20)       38 2024-05-21 12:55:55.348405 requence-0.0.1/setup.cfg
--rw-r--r--   0 torstenblindert   (502) staff       (20)      438 2024-05-21 12:07:14.000000 requence-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:05:47.882509 requence-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-06-03 13:05:28.000000 requence-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-06-03 13:05:47.882509 requence-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-06-03 13:05:28.000000 requence-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-06-03 13:05:28.000000 requence-0.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:05:47.878509 requence-0.1.1/requence/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:05:28.000000 requence-0.1.1/requence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6249 2024-06-03 13:05:28.000000 requence-0.1.1/requence/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-06-03 13:05:28.000000 requence-0.1.1/requence/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-06-03 13:05:28.000000 requence-0.1.1/requence/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-06-03 13:05:28.000000 requence-0.1.1/requence/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-06-03 13:05:28.000000 requence-0.1.1/requence/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-06-03 13:05:28.000000 requence-0.1.1/requence/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:05:47.878509 requence-0.1.1/requence.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-06-03 13:05:47.000000 requence-0.1.1/requence.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-06-03 13:05:47.000000 requence-0.1.1/requence.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 13:05:47.000000 requence-0.1.1/requence.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-06-03 13:05:47.000000 requence-0.1.1/requence.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-03 13:05:47.000000 requence-0.1.1/requence.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 13:05:47.882509 requence-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-06-03 13:05:28.000000 requence-0.1.1/setup.py
```

