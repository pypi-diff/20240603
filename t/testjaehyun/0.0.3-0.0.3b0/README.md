# Comparing `tmp/testjaehyun-0.0.3.tar.gz` & `tmp/testjaehyun-0.0.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testjaehyun-0.0.3.tar", last modified: Mon Jun  3 14:43:02 2024, max compression
+gzip compressed data, was "testjaehyun-0.0.3b0.tar", last modified: Mon Jun  3 14:45:47 2024, max compression
```

## Comparing `testjaehyun-0.0.3.tar` & `testjaehyun-0.0.3b0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 yimjaehyun   (501) staff       (20)        0 2024-06-03 14:43:02.486336 testjaehyun-0.0.3/
--rw-r--r--   0 yimjaehyun   (501) staff       (20)      270 2024-06-03 14:43:02.486401 testjaehyun-0.0.3/PKG-INFO
--rw-r--r--   0 yimjaehyun   (501) staff       (20)        5 2024-06-03 11:29:32.000000 testjaehyun-0.0.3/README.md
--rw-r--r--   0 yimjaehyun   (501) staff       (20)       79 2024-06-03 14:43:02.486630 testjaehyun-0.0.3/setup.cfg
--rw-r--r--   0 yimjaehyun   (501) staff       (20)      483 2024-06-03 14:42:46.000000 testjaehyun-0.0.3/setup.py
-drwxr-xr-x   0 yimjaehyun   (501) staff       (20)        0 2024-06-03 14:43:02.485560 testjaehyun-0.0.3/testjaehyun/
--rw-r--r--   0 yimjaehyun   (501) staff       (20)       58 2024-06-03 11:29:56.000000 testjaehyun-0.0.3/testjaehyun/__init__.py
--rw-r--r--   0 yimjaehyun   (501) staff       (20)       22 2024-06-03 14:42:42.000000 testjaehyun-0.0.3/testjaehyun/__version__.py
--rw-r--r--   0 yimjaehyun   (501) staff       (20)       45 2024-06-03 14:40:18.000000 testjaehyun-0.0.3/testjaehyun/plus.py
-drwxr-xr-x   0 yimjaehyun   (501) staff       (20)        0 2024-06-03 14:43:02.486213 testjaehyun-0.0.3/testjaehyun.egg-info/
--rw-r--r--   0 yimjaehyun   (501) staff       (20)      270 2024-06-03 14:43:02.000000 testjaehyun-0.0.3/testjaehyun.egg-info/PKG-INFO
--rw-r--r--   0 yimjaehyun   (501) staff       (20)      239 2024-06-03 14:43:02.000000 testjaehyun-0.0.3/testjaehyun.egg-info/SOURCES.txt
--rw-r--r--   0 yimjaehyun   (501) staff       (20)        1 2024-06-03 14:43:02.000000 testjaehyun-0.0.3/testjaehyun.egg-info/dependency_links.txt
--rw-r--r--   0 yimjaehyun   (501) staff       (20)       12 2024-06-03 14:43:02.000000 testjaehyun-0.0.3/testjaehyun.egg-info/top_level.txt
+drwxr-xr-x   0 yimjaehyun   (501) staff       (20)        0 2024-06-03 14:45:47.425175 testjaehyun-0.0.3b0/
+-rw-r--r--   0 yimjaehyun   (501) staff       (20)      272 2024-06-03 14:45:47.425346 testjaehyun-0.0.3b0/PKG-INFO
+-rw-r--r--   0 yimjaehyun   (501) staff       (20)        5 2024-06-03 11:29:32.000000 testjaehyun-0.0.3b0/README.md
+-rw-r--r--   0 yimjaehyun   (501) staff       (20)       79 2024-06-03 14:45:47.425575 testjaehyun-0.0.3b0/setup.cfg
+-rw-r--r--   0 yimjaehyun   (501) staff       (20)      516 2024-06-03 14:45:23.000000 testjaehyun-0.0.3b0/setup.py
+drwxr-xr-x   0 yimjaehyun   (501) staff       (20)        0 2024-06-03 14:45:47.424463 testjaehyun-0.0.3b0/testjaehyun/
+-rw-r--r--   0 yimjaehyun   (501) staff       (20)       58 2024-06-03 11:29:56.000000 testjaehyun-0.0.3b0/testjaehyun/__init__.py
+-rw-r--r--   0 yimjaehyun   (501) staff       (20)       27 2024-06-03 14:45:38.000000 testjaehyun-0.0.3b0/testjaehyun/__version__.py
+-rw-r--r--   0 yimjaehyun   (501) staff       (20)       45 2024-06-03 14:40:18.000000 testjaehyun-0.0.3b0/testjaehyun/plus.py
+drwxr-xr-x   0 yimjaehyun   (501) staff       (20)        0 2024-06-03 14:45:47.425075 testjaehyun-0.0.3b0/testjaehyun.egg-info/
+-rw-r--r--   0 yimjaehyun   (501) staff       (20)      272 2024-06-03 14:45:47.000000 testjaehyun-0.0.3b0/testjaehyun.egg-info/PKG-INFO
+-rw-r--r--   0 yimjaehyun   (501) staff       (20)      239 2024-06-03 14:45:47.000000 testjaehyun-0.0.3b0/testjaehyun.egg-info/SOURCES.txt
+-rw-r--r--   0 yimjaehyun   (501) staff       (20)        1 2024-06-03 14:45:47.000000 testjaehyun-0.0.3b0/testjaehyun.egg-info/dependency_links.txt
+-rw-r--r--   0 yimjaehyun   (501) staff       (20)       12 2024-06-03 14:45:47.000000 testjaehyun-0.0.3b0/testjaehyun.egg-info/top_level.txt
```

