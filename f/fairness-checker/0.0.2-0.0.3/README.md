# Comparing `tmp/fairness_checker-0.0.2.tar.gz` & `tmp/fairness_checker-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fairness_checker-0.0.2.tar", last modified: Wed May 29 18:17:37 2024, max compression
+gzip compressed data, was "fairness_checker-0.0.3.tar", last modified: Mon Jun  3 13:28:00 2024, max compression
```

## Comparing `fairness_checker-0.0.2.tar` & `fairness_checker-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 rexyuan    (501) staff       (20)        0 2024-05-29 18:17:37.000000 fairness_checker-0.0.2/
--rw-r--r--   0 rexyuan    (501) staff       (20)     1211 2024-05-23 21:16:19.000000 fairness_checker-0.0.2/LICENSE
--rw-r--r--   0 rexyuan    (501) staff       (20)      477 2024-05-29 18:17:37.000000 fairness_checker-0.0.2/PKG-INFO
--rw-r--r--   0 rexyuan    (501) staff       (20)       12 2024-05-23 21:19:13.000000 fairness_checker-0.0.2/README.md
--rw-r--r--   0 rexyuan    (501) staff       (20)       38 2024-05-29 18:17:37.000000 fairness_checker-0.0.2/setup.cfg
--rw-r--r--   0 rexyuan    (501) staff       (20)      497 2024-05-29 18:17:00.000000 fairness_checker-0.0.2/setup.py
-drwxr-xr-x   0 rexyuan    (501) staff       (20)        0 2024-05-29 18:17:37.000000 fairness_checker-0.0.2/src/
-drwxr-xr-x   0 rexyuan    (501) staff       (20)        0 2024-05-29 18:17:37.000000 fairness_checker-0.0.2/src/fairness_checker/
--rw-r--r--   0 rexyuan    (501) staff       (20)       20 2024-05-23 20:38:54.000000 fairness_checker-0.0.2/src/fairness_checker/__init__.py
--rw-r--r--   0 rexyuan    (501) staff       (20)    59726 2024-05-29 18:10:29.000000 fairness_checker-0.0.2/src/fairness_checker/main.py
-drwxr-xr-x   0 rexyuan    (501) staff       (20)        0 2024-05-29 18:17:37.000000 fairness_checker-0.0.2/src/fairness_checker.egg-info/
--rw-r--r--   0 rexyuan    (501) staff       (20)      477 2024-05-29 18:17:37.000000 fairness_checker-0.0.2/src/fairness_checker.egg-info/PKG-INFO
--rw-r--r--   0 rexyuan    (501) staff       (20)      264 2024-05-29 18:17:37.000000 fairness_checker-0.0.2/src/fairness_checker.egg-info/SOURCES.txt
--rw-r--r--   0 rexyuan    (501) staff       (20)        1 2024-05-29 18:17:37.000000 fairness_checker-0.0.2/src/fairness_checker.egg-info/dependency_links.txt
--rw-r--r--   0 rexyuan    (501) staff       (20)       17 2024-05-29 18:17:37.000000 fairness_checker-0.0.2/src/fairness_checker.egg-info/top_level.txt
+drwxr-xr-x   0 rexyuan    (501) staff       (20)        0 2024-06-03 13:28:00.967287 fairness_checker-0.0.3/
+-rw-r--r--   0 rexyuan    (501) staff       (20)     1211 2024-05-23 21:16:19.000000 fairness_checker-0.0.3/LICENSE
+-rw-r--r--   0 rexyuan    (501) staff       (20)      500 2024-06-03 13:28:00.966441 fairness_checker-0.0.3/PKG-INFO
+-rw-r--r--   0 rexyuan    (501) staff       (20)       12 2024-05-23 21:19:13.000000 fairness_checker-0.0.3/README.md
+-rw-r--r--   0 rexyuan    (501) staff       (20)       38 2024-06-03 13:28:00.967487 fairness_checker-0.0.3/setup.cfg
+-rw-r--r--   0 rexyuan    (501) staff       (20)      526 2024-06-03 13:27:45.000000 fairness_checker-0.0.3/setup.py
+drwxr-xr-x   0 rexyuan    (501) staff       (20)        0 2024-06-03 13:28:00.952591 fairness_checker-0.0.3/src/
+drwxr-xr-x   0 rexyuan    (501) staff       (20)        0 2024-06-03 13:28:00.955907 fairness_checker-0.0.3/src/fairness_checker/
+-rw-r--r--   0 rexyuan    (501) staff       (20)       20 2024-05-23 20:38:54.000000 fairness_checker-0.0.3/src/fairness_checker/__init__.py
+-rw-r--r--   0 rexyuan    (501) staff       (20)    59726 2024-05-29 18:10:29.000000 fairness_checker-0.0.3/src/fairness_checker/main.py
+drwxr-xr-x   0 rexyuan    (501) staff       (20)        0 2024-06-03 13:28:00.965659 fairness_checker-0.0.3/src/fairness_checker.egg-info/
+-rw-r--r--   0 rexyuan    (501) staff       (20)      500 2024-06-03 13:28:00.000000 fairness_checker-0.0.3/src/fairness_checker.egg-info/PKG-INFO
+-rw-r--r--   0 rexyuan    (501) staff       (20)      264 2024-06-03 13:28:00.000000 fairness_checker-0.0.3/src/fairness_checker.egg-info/SOURCES.txt
+-rw-r--r--   0 rexyuan    (501) staff       (20)        1 2024-06-03 13:28:00.000000 fairness_checker-0.0.3/src/fairness_checker.egg-info/dependency_links.txt
+-rw-r--r--   0 rexyuan    (501) staff       (20)       17 2024-06-03 13:28:00.000000 fairness_checker-0.0.3/src/fairness_checker.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fairness_checker-0.0.2/LICENSE` & `fairness_checker-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fairness_checker-0.0.2/src/fairness_checker/main.py` & `fairness_checker-0.0.3/src/fairness_checker/main.py`

 * *Files identical despite different names*

