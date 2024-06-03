# Comparing `tmp/libem-0.0.8.tar.gz` & `tmp/libem-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libem-0.0.8.tar", last modified: Fri May 24 00:41:39 2024, max compression
+gzip compressed data, was "libem-0.0.9.tar", last modified: Mon Jun  3 03:41:01 2024, max compression
```

## Comparing `libem-0.0.8.tar` & `libem-0.0.9.tar`

### file list

```diff
@@ -1,83 +1,107 @@
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-24 00:41:39.953794 libem-0.0.8/
--rw-r--r--   0 silv       (501) staff       (20)    11357 2024-05-01 02:16:29.000000 libem-0.0.8/LICENSE
--rw-r--r--   0 silv       (501) staff       (20)      272 2024-05-24 00:41:39.953636 libem-0.0.8/PKG-INFO
--rw-r--r--   0 silv       (501) staff       (20)     1343 2024-05-09 21:01:57.000000 libem-0.0.8/README.md
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-24 00:41:39.938987 libem-0.0.8/cli/
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-05 16:25:37.000000 libem-0.0.8/cli/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)     1366 2024-05-14 01:22:05.000000 libem-0.0.8/cli/libem
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-24 00:41:39.940860 libem-0.0.8/libem/
--rw-r--r--   0 silv       (501) staff       (20)      382 2024-05-14 16:05:14.000000 libem-0.0.8/libem/__init__.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-24 00:41:39.942602 libem-0.0.8/libem/browse/
--rw-r--r--   0 silv       (501) staff       (20)       92 2024-05-05 00:16:54.000000 libem-0.0.8/libem/browse/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)     3406 2024-05-14 16:05:14.000000 libem-0.0.8/libem/browse/function.py
--rw-r--r--   0 silv       (501) staff       (20)       99 2024-05-15 18:04:36.000000 libem-0.0.8/libem/browse/parameter.py
--rw-r--r--   0 silv       (501) staff       (20)      318 2024-05-09 21:57:54.000000 libem-0.0.8/libem/browse/prompt.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-24 00:41:39.943334 libem-0.0.8/libem/calibrate/
--rw-r--r--   0 silv       (501) staff       (20)      139 2024-05-09 20:29:02.000000 libem-0.0.8/libem/calibrate/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)     4420 2024-05-16 16:16:14.000000 libem-0.0.8/libem/calibrate/function.py
--rw-r--r--   0 silv       (501) staff       (20)      436 2024-05-09 22:15:40.000000 libem-0.0.8/libem/calibrate/interface.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-24 00:41:39.943885 libem-0.0.8/libem/calibrate/optimize/
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-12 21:34:51.000000 libem-0.0.8/libem/calibrate/optimize/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)      851 2024-05-14 16:08:26.000000 libem-0.0.8/libem/constant.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-24 00:41:39.946414 libem-0.0.8/libem/core/
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-03 06:45:38.000000 libem-0.0.8/libem/core/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)     3823 2024-05-08 06:37:24.000000 libem-0.0.8/libem/core/eval.py
--rw-r--r--   0 silv       (501) staff       (20)      159 2024-05-14 16:05:14.000000 libem-0.0.8/libem/core/exception.py
--rw-r--r--   0 silv       (501) staff       (20)     3779 2024-05-14 16:05:14.000000 libem-0.0.8/libem/core/log.py
--rw-r--r--   0 silv       (501) staff       (20)     4986 2024-05-17 06:11:45.000000 libem-0.0.8/libem/core/model.py
--rw-r--r--   0 silv       (501) staff       (20)     4870 2024-05-16 16:26:57.000000 libem-0.0.8/libem/core/struct.py
--rw-r--r--   0 silv       (501) staff       (20)      911 2024-05-15 18:14:15.000000 libem-0.0.8/libem/core/telemetry.py
--rw-r--r--   0 silv       (501) staff       (20)     2128 2024-05-17 06:17:04.000000 libem-0.0.8/libem/core/trace.py
--rw-r--r--   0 silv       (501) staff       (20)     1020 2024-05-09 21:08:05.000000 libem-0.0.8/libem/core/util.py
--rw-r--r--   0 silv       (501) staff       (20)       35 2024-05-07 06:37:47.000000 libem-0.0.8/libem/function.py
--rw-r--r--   0 silv       (501) staff       (20)      973 2024-05-14 16:15:38.000000 libem-0.0.8/libem/interface.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-24 00:41:39.947341 libem-0.0.8/libem/match/
--rw-r--r--   0 silv       (501) staff       (20)       90 2024-05-05 00:16:44.000000 libem-0.0.8/libem/match/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)     1666 2024-05-17 04:39:34.000000 libem-0.0.8/libem/match/function.py
--rw-r--r--   0 silv       (501) staff       (20)      211 2024-05-15 18:00:54.000000 libem-0.0.8/libem/match/parameter.py
--rw-r--r--   0 silv       (501) staff       (20)      684 2024-05-17 05:51:52.000000 libem-0.0.8/libem/match/prompt.py
--rw-r--r--   0 silv       (501) staff       (20)      204 2024-05-14 16:07:48.000000 libem-0.0.8/libem/parameter.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-24 00:41:39.948078 libem-0.0.8/libem/prepare/
--rw-r--r--   0 silv       (501) staff       (20)       94 2024-05-05 04:43:06.000000 libem-0.0.8/libem/prepare/__init__.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-24 00:41:39.949732 libem-0.0.8/libem/prepare/datasets/
--rw-r--r--   0 silv       (501) staff       (20)      134 2024-05-09 00:08:47.000000 libem-0.0.8/libem/prepare/datasets/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)     2954 2024-05-09 00:05:08.000000 libem-0.0.8/libem/prepare/datasets/abt_buy.py
--rw-r--r--   0 silv       (501) staff       (20)     2698 2024-05-09 00:06:05.000000 libem-0.0.8/libem/prepare/datasets/amazon_google.py
--rw-r--r--   0 silv       (501) staff       (20)     2764 2024-05-14 16:05:14.000000 libem-0.0.8/libem/prepare/datasets/dblp_acm.py
--rw-r--r--   0 silv       (501) staff       (20)     2760 2024-05-09 00:08:21.000000 libem-0.0.8/libem/prepare/datasets/dblp_scholar.py
--rw-r--r--   0 silv       (501) staff       (20)     2792 2024-05-09 00:08:37.000000 libem-0.0.8/libem/prepare/datasets/walmart_amazon.py
--rw-r--r--   0 silv       (501) staff       (20)       72 2024-05-08 23:56:27.000000 libem-0.0.8/libem/prepare/function.py
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-03 06:17:55.000000 libem-0.0.8/libem/prepare/parameter.py
--rw-r--r--   0 silv       (501) staff       (20)       38 2024-05-05 00:06:37.000000 libem-0.0.8/libem/prepare/prompt.py
--rw-r--r--   0 silv       (501) staff       (20)      204 2024-05-07 15:43:38.000000 libem-0.0.8/libem/prompt.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-24 00:41:39.950628 libem-0.0.8/libem/tune/
--rw-r--r--   0 silv       (501) staff       (20)      129 2024-05-08 00:48:47.000000 libem-0.0.8/libem/tune/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)       31 2024-05-14 16:19:43.000000 libem-0.0.8/libem/tune/catalog.py
--rw-r--r--   0 silv       (501) staff       (20)       37 2024-05-07 06:18:54.000000 libem-0.0.8/libem/tune/function.py
--rw-r--r--   0 silv       (501) staff       (20)      224 2024-05-09 21:34:22.000000 libem-0.0.8/libem/tune/interface.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-24 00:41:39.951691 libem-0.0.8/libem/tune/learn/
--rw-r--r--   0 silv       (501) staff       (20)      110 2024-05-07 23:38:41.000000 libem-0.0.8/libem/tune/learn/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)     3022 2024-05-16 16:16:36.000000 libem-0.0.8/libem/tune/learn/function.py
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-08 23:52:04.000000 libem-0.0.8/libem/tune/learn/interface.py
--rw-r--r--   0 silv       (501) staff       (20)      131 2024-05-15 17:57:55.000000 libem-0.0.8/libem/tune/learn/parameter.py
--rw-r--r--   0 silv       (501) staff       (20)      730 2024-05-09 23:34:00.000000 libem-0.0.8/libem/tune/learn/prompt.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-24 00:41:39.952150 libem-0.0.8/libem/tune/load/
--rw-r--r--   0 silv       (501) staff       (20)       93 2024-05-07 06:19:35.000000 libem-0.0.8/libem/tune/load/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)       37 2024-05-07 06:19:05.000000 libem-0.0.8/libem/tune/load/function.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-24 00:41:39.952585 libem-0.0.8/libem/tune/save/
--rw-r--r--   0 silv       (501) staff       (20)       93 2024-05-07 06:19:35.000000 libem-0.0.8/libem/tune/save/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)       37 2024-05-07 06:19:04.000000 libem-0.0.8/libem/tune/save/function.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-24 00:41:39.953042 libem-0.0.8/libem/tune/search/
--rw-r--r--   0 silv       (501) staff       (20)       97 2024-05-07 06:21:06.000000 libem-0.0.8/libem/tune/search/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)      139 2024-05-07 06:36:20.000000 libem-0.0.8/libem/tune/search/function.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-24 00:41:39.941591 libem-0.0.8/libem.egg-info/
--rw-r--r--   0 silv       (501) staff       (20)      272 2024-05-24 00:41:39.000000 libem-0.0.8/libem.egg-info/PKG-INFO
--rw-r--r--   0 silv       (501) staff       (20)     1575 2024-05-24 00:41:39.000000 libem-0.0.8/libem.egg-info/SOURCES.txt
--rw-r--r--   0 silv       (501) staff       (20)        1 2024-05-24 00:41:39.000000 libem-0.0.8/libem.egg-info/dependency_links.txt
--rw-r--r--   0 silv       (501) staff       (20)      127 2024-05-24 00:41:39.000000 libem-0.0.8/libem.egg-info/requires.txt
--rw-r--r--   0 silv       (501) staff       (20)       16 2024-05-24 00:41:39.000000 libem-0.0.8/libem.egg-info/top_level.txt
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-24 00:41:39.953331 libem-0.0.8/serve/
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-04 23:17:56.000000 libem-0.0.8/serve/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)      578 2024-05-04 23:21:19.000000 libem-0.0.8/serve/run.py
--rw-r--r--   0 silv       (501) staff       (20)       38 2024-05-24 00:41:39.953838 libem-0.0.8/setup.cfg
--rw-r--r--   0 silv       (501) staff       (20)      449 2024-05-24 00:31:37.000000 libem-0.0.8/setup.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-06-03 03:41:01.474617 libem-0.0.9/
+-rw-r--r--   0 silv       (501) staff       (20)    11357 2024-05-01 02:16:29.000000 libem-0.0.9/LICENSE
+-rw-r--r--   0 silv       (501) staff       (20)      272 2024-06-03 03:41:01.474499 libem-0.0.9/PKG-INFO
+-rw-r--r--   0 silv       (501) staff       (20)     1343 2024-05-09 21:01:57.000000 libem-0.0.9/README.md
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-06-03 03:41:01.456424 libem-0.0.9/benchmark/
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-31 05:11:53.000000 libem-0.0.9/benchmark/__init__.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-06-03 03:41:01.457731 libem-0.0.9/benchmark/classic/
+-rw-r--r--   0 silv       (501) staff       (20)      608 2024-05-31 05:11:53.000000 libem-0.0.9/benchmark/classic/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     2107 2024-05-31 05:11:53.000000 libem-0.0.9/benchmark/classic/abt_buy.py
+-rw-r--r--   0 silv       (501) staff       (20)     2365 2024-05-31 05:11:53.000000 libem-0.0.9/benchmark/classic/amazon_google.py
+-rw-r--r--   0 silv       (501) staff       (20)     2047 2024-05-31 05:11:53.000000 libem-0.0.9/benchmark/classic/beer.py
+-rw-r--r--   0 silv       (501) staff       (20)     2045 2024-05-31 05:11:53.000000 libem-0.0.9/benchmark/classic/dblp_acm.py
+-rw-r--r--   0 silv       (501) staff       (20)     2053 2024-05-31 05:11:53.000000 libem-0.0.9/benchmark/classic/dblp_scholar.py
+-rw-r--r--   0 silv       (501) staff       (20)     1936 2024-05-31 05:11:53.000000 libem-0.0.9/benchmark/classic/fodors_zagats.py
+-rw-r--r--   0 silv       (501) staff       (20)     1955 2024-05-31 05:11:53.000000 libem-0.0.9/benchmark/classic/itunes_amazon.py
+-rw-r--r--   0 silv       (501) staff       (20)     2439 2024-05-31 05:11:53.000000 libem-0.0.9/benchmark/classic/walmart_amazon.py
+-rw-r--r--   0 silv       (501) staff       (20)      527 2024-05-31 05:11:53.000000 libem-0.0.9/benchmark/explain.py
+-rw-r--r--   0 silv       (501) staff       (20)     2580 2024-05-31 05:11:53.000000 libem-0.0.9/benchmark/run.py
+-rw-r--r--   0 silv       (501) staff       (20)     4167 2024-05-31 05:11:53.000000 libem-0.0.9/benchmark/util.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-06-03 03:41:01.457922 libem-0.0.9/cli/
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-05 16:25:37.000000 libem-0.0.9/cli/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     1366 2024-05-14 01:22:05.000000 libem-0.0.9/cli/libem
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-06-03 03:41:01.459204 libem-0.0.9/libem/
+-rw-r--r--   0 silv       (501) staff       (20)      382 2024-05-14 16:05:14.000000 libem-0.0.9/libem/__init__.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-06-03 03:41:01.460530 libem-0.0.9/libem/browse/
+-rw-r--r--   0 silv       (501) staff       (20)       92 2024-05-05 00:16:54.000000 libem-0.0.9/libem/browse/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     3406 2024-05-14 16:05:14.000000 libem-0.0.9/libem/browse/function.py
+-rw-r--r--   0 silv       (501) staff       (20)       99 2024-05-15 18:04:36.000000 libem-0.0.9/libem/browse/parameter.py
+-rw-r--r--   0 silv       (501) staff       (20)      318 2024-05-09 21:57:54.000000 libem-0.0.9/libem/browse/prompt.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-06-03 03:41:01.461692 libem-0.0.9/libem/calibrate/
+-rw-r--r--   0 silv       (501) staff       (20)      139 2024-05-09 20:29:02.000000 libem-0.0.9/libem/calibrate/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     4420 2024-05-16 16:16:14.000000 libem-0.0.9/libem/calibrate/function.py
+-rw-r--r--   0 silv       (501) staff       (20)      436 2024-05-09 22:15:40.000000 libem-0.0.9/libem/calibrate/interface.py
+-rw-r--r--   0 silv       (501) staff       (20)      851 2024-05-14 16:08:26.000000 libem-0.0.9/libem/constant.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-06-03 03:41:01.464373 libem-0.0.9/libem/core/
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-03 06:45:38.000000 libem-0.0.9/libem/core/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     3823 2024-05-08 06:37:24.000000 libem-0.0.9/libem/core/eval.py
+-rw-r--r--   0 silv       (501) staff       (20)      159 2024-05-14 16:05:14.000000 libem-0.0.9/libem/core/exception.py
+-rw-r--r--   0 silv       (501) staff       (20)     3779 2024-05-14 16:05:14.000000 libem-0.0.9/libem/core/log.py
+-rw-r--r--   0 silv       (501) staff       (20)     4916 2024-06-03 02:15:03.000000 libem-0.0.9/libem/core/model.py
+-rw-r--r--   0 silv       (501) staff       (20)     4870 2024-05-16 16:26:57.000000 libem-0.0.9/libem/core/struct.py
+-rw-r--r--   0 silv       (501) staff       (20)      911 2024-05-15 18:14:15.000000 libem-0.0.9/libem/core/telemetry.py
+-rw-r--r--   0 silv       (501) staff       (20)     2128 2024-05-17 06:17:04.000000 libem-0.0.9/libem/core/trace.py
+-rw-r--r--   0 silv       (501) staff       (20)     1020 2024-05-09 21:08:05.000000 libem-0.0.9/libem/core/util.py
+-rw-r--r--   0 silv       (501) staff       (20)       35 2024-05-07 06:37:47.000000 libem-0.0.9/libem/function.py
+-rw-r--r--   0 silv       (501) staff       (20)      973 2024-05-14 16:15:38.000000 libem-0.0.9/libem/interface.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-06-03 03:41:01.465448 libem-0.0.9/libem/match/
+-rw-r--r--   0 silv       (501) staff       (20)       90 2024-05-05 00:16:44.000000 libem-0.0.9/libem/match/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     1666 2024-05-30 20:30:36.000000 libem-0.0.9/libem/match/function.py
+-rw-r--r--   0 silv       (501) staff       (20)      211 2024-05-15 18:00:54.000000 libem-0.0.9/libem/match/parameter.py
+-rw-r--r--   0 silv       (501) staff       (20)      684 2024-05-17 05:51:52.000000 libem-0.0.9/libem/match/prompt.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-06-03 03:41:01.466454 libem-0.0.9/libem/optimize/
+-rw-r--r--   0 silv       (501) staff       (20)       38 2024-05-29 23:20:43.000000 libem-0.0.9/libem/optimize/__init__.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-06-03 03:41:01.467223 libem-0.0.9/libem/optimize/cost/
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-29 23:25:32.000000 libem-0.0.9/libem/optimize/cost/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     1751 2024-05-29 23:46:35.000000 libem-0.0.9/libem/optimize/cost/cache.py
+-rw-r--r--   0 silv       (501) staff       (20)      821 2024-05-30 01:37:37.000000 libem-0.0.9/libem/optimize/cost/openai.py
+-rw-r--r--   0 silv       (501) staff       (20)      276 2024-05-30 01:39:51.000000 libem-0.0.9/libem/optimize/interface.py
+-rw-r--r--   0 silv       (501) staff       (20)      204 2024-05-14 16:07:48.000000 libem-0.0.9/libem/parameter.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-06-03 03:41:01.468017 libem-0.0.9/libem/prepare/
+-rw-r--r--   0 silv       (501) staff       (20)       94 2024-05-05 04:43:06.000000 libem-0.0.9/libem/prepare/__init__.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-06-03 03:41:01.469996 libem-0.0.9/libem/prepare/datasets/
+-rw-r--r--   0 silv       (501) staff       (20)      134 2024-05-09 00:08:47.000000 libem-0.0.9/libem/prepare/datasets/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     6253 2024-05-30 21:10:28.000000 libem-0.0.9/libem/prepare/datasets/abt_buy.py
+-rw-r--r--   0 silv       (501) staff       (20)     6456 2024-05-30 21:10:28.000000 libem-0.0.9/libem/prepare/datasets/amazon_google.py
+-rw-r--r--   0 silv       (501) staff       (20)     5274 2024-05-30 21:10:28.000000 libem-0.0.9/libem/prepare/datasets/beer.py
+-rw-r--r--   0 silv       (501) staff       (20)     5348 2024-05-30 21:10:28.000000 libem-0.0.9/libem/prepare/datasets/dblp_acm.py
+-rw-r--r--   0 silv       (501) staff       (20)     5348 2024-05-30 21:10:28.000000 libem-0.0.9/libem/prepare/datasets/dblp_scholar.py
+-rw-r--r--   0 silv       (501) staff       (20)     5177 2024-05-30 21:10:28.000000 libem-0.0.9/libem/prepare/datasets/fodors_zagats.py
+-rw-r--r--   0 silv       (501) staff       (20)     3381 2024-05-30 21:10:28.000000 libem-0.0.9/libem/prepare/datasets/format_datasets.py
+-rw-r--r--   0 silv       (501) staff       (20)     5692 2024-05-30 21:10:28.000000 libem-0.0.9/libem/prepare/datasets/itunes_amazon.py
+-rw-r--r--   0 silv       (501) staff       (20)     6519 2024-05-30 21:10:28.000000 libem-0.0.9/libem/prepare/datasets/walmart_amazon.py
+-rw-r--r--   0 silv       (501) staff       (20)       72 2024-05-08 23:56:27.000000 libem-0.0.9/libem/prepare/function.py
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-03 06:17:55.000000 libem-0.0.9/libem/prepare/parameter.py
+-rw-r--r--   0 silv       (501) staff       (20)       38 2024-05-05 00:06:37.000000 libem-0.0.9/libem/prepare/prompt.py
+-rw-r--r--   0 silv       (501) staff       (20)      204 2024-05-07 15:43:38.000000 libem-0.0.9/libem/prompt.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-06-03 03:41:01.470888 libem-0.0.9/libem/tune/
+-rw-r--r--   0 silv       (501) staff       (20)      129 2024-05-08 00:48:47.000000 libem-0.0.9/libem/tune/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)       31 2024-05-14 16:19:43.000000 libem-0.0.9/libem/tune/catalog.py
+-rw-r--r--   0 silv       (501) staff       (20)       37 2024-05-07 06:18:54.000000 libem-0.0.9/libem/tune/function.py
+-rw-r--r--   0 silv       (501) staff       (20)      224 2024-05-09 21:34:22.000000 libem-0.0.9/libem/tune/interface.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-06-03 03:41:01.471803 libem-0.0.9/libem/tune/learn/
+-rw-r--r--   0 silv       (501) staff       (20)      110 2024-05-07 23:38:41.000000 libem-0.0.9/libem/tune/learn/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     3022 2024-05-16 16:16:36.000000 libem-0.0.9/libem/tune/learn/function.py
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-08 23:52:04.000000 libem-0.0.9/libem/tune/learn/interface.py
+-rw-r--r--   0 silv       (501) staff       (20)      131 2024-05-15 17:57:55.000000 libem-0.0.9/libem/tune/learn/parameter.py
+-rw-r--r--   0 silv       (501) staff       (20)      730 2024-05-09 23:34:00.000000 libem-0.0.9/libem/tune/learn/prompt.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-06-03 03:41:01.473003 libem-0.0.9/libem/tune/load/
+-rw-r--r--   0 silv       (501) staff       (20)       93 2024-05-07 06:19:35.000000 libem-0.0.9/libem/tune/load/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)       37 2024-05-07 06:19:05.000000 libem-0.0.9/libem/tune/load/function.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-06-03 03:41:01.473431 libem-0.0.9/libem/tune/save/
+-rw-r--r--   0 silv       (501) staff       (20)       93 2024-05-07 06:19:35.000000 libem-0.0.9/libem/tune/save/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)       37 2024-05-07 06:19:04.000000 libem-0.0.9/libem/tune/save/function.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-06-03 03:41:01.473856 libem-0.0.9/libem/tune/search/
+-rw-r--r--   0 silv       (501) staff       (20)       97 2024-05-07 06:21:06.000000 libem-0.0.9/libem/tune/search/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)      139 2024-05-07 06:36:20.000000 libem-0.0.9/libem/tune/search/function.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-06-03 03:41:01.459793 libem-0.0.9/libem.egg-info/
+-rw-r--r--   0 silv       (501) staff       (20)      272 2024-06-03 03:41:01.000000 libem-0.0.9/libem.egg-info/PKG-INFO
+-rw-r--r--   0 silv       (501) staff       (20)     2205 2024-06-03 03:41:01.000000 libem-0.0.9/libem.egg-info/SOURCES.txt
+-rw-r--r--   0 silv       (501) staff       (20)        1 2024-06-03 03:41:01.000000 libem-0.0.9/libem.egg-info/dependency_links.txt
+-rw-r--r--   0 silv       (501) staff       (20)      136 2024-06-03 03:41:01.000000 libem-0.0.9/libem.egg-info/requires.txt
+-rw-r--r--   0 silv       (501) staff       (20)       26 2024-06-03 03:41:01.000000 libem-0.0.9/libem.egg-info/top_level.txt
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-06-03 03:41:01.474141 libem-0.0.9/serve/
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-04 23:17:56.000000 libem-0.0.9/serve/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)      578 2024-05-04 23:21:19.000000 libem-0.0.9/serve/run.py
+-rw-r--r--   0 silv       (501) staff       (20)       38 2024-06-03 03:41:01.474649 libem-0.0.9/setup.cfg
+-rw-r--r--   0 silv       (501) staff       (20)      449 2024-06-03 03:40:10.000000 libem-0.0.9/setup.py
```

### Comparing `libem-0.0.8/LICENSE` & `libem-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `libem-0.0.8/README.md` & `libem-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `libem-0.0.8/cli/libem` & `libem-0.0.9/cli/libem`

 * *Files identical despite different names*

### Comparing `libem-0.0.8/libem/browse/function.py` & `libem-0.0.9/libem/browse/function.py`

 * *Files identical despite different names*

### Comparing `libem-0.0.8/libem/calibrate/function.py` & `libem-0.0.9/libem/calibrate/function.py`

 * *Files identical despite different names*

### Comparing `libem-0.0.8/libem/constant.py` & `libem-0.0.9/libem/constant.py`

 * *Files identical despite different names*

### Comparing `libem-0.0.8/libem/core/eval.py` & `libem-0.0.9/libem/core/eval.py`

 * *Files identical despite different names*

### Comparing `libem-0.0.8/libem/core/log.py` & `libem-0.0.9/libem/core/log.py`

 * *Files identical despite different names*

### Comparing `libem-0.0.8/libem/core/model.py` & `libem-0.0.9/libem/core/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,28 +16,27 @@
 os.environ.setdefault(
     "OPENAI_API_KEY",
     libem.LIBEM_CONFIG.get("OPENAI_API_KEY", "")
 )
 
 
 # LLM call with multiple rounds of tool use
-def openai(prompt: str, tools: list[str],
-           model: str, temperature: float,
+def openai(prompt: str, tools: list[str] = None,
+           model: str = "gpt-4o", temperature: float = 0.0,
            max_model_call: int = 3,
            seed: int = None) -> str:
     if not os.environ.get("OPENAI_API_KEY"):
-        raise EnvironmentError(f"OPENAI_API_KEY is not set. "
-                               f"Check your environment or {libem.LIBEM_CONFIG_FILE}.")
+        raise EnvironmentError(f"OPENAI_API_KEY is not set.")
     client = OpenAI()
 
     # todo: simplify accounting using model response
     num_model_calls = 0
     num_input_tokens, num_output_tokens = 0, 0
 
-    if len(tools) == 0:
+    if not tools:
         """ Call with no tool use """
         try:
             response = client.chat.completions.create(
                 model=model,
                 messages=[{"role": "user", "content": prompt}],
                 seed=seed,
                 temperature=temperature,
@@ -90,18 +89,18 @@
                 function_to_call = available_functions[function_name]
                 function_args = json.loads(tool_call.function.arguments)
 
                 libem.info(f"Tool: {function_name} - running ..")
                 function_response = function_to_call(**function_args)
                 messages.append(
                     {
-                        "tool_call_id": tool_call.id,
                         "role": "tool",
                         "name": function_name,
                         "content": function_response,
+                        "tool_call_id": tool_call.id,
                     }
                 )
                 libem.trace.add({
                     'tool': {
                         "id": tool_call.id,
                         'name': function_name,
                         "arguments": function_args,
```

### Comparing `libem-0.0.8/libem/core/struct.py` & `libem-0.0.9/libem/core/struct.py`

 * *Files identical despite different names*

### Comparing `libem-0.0.8/libem/core/telemetry.py` & `libem-0.0.9/libem/core/telemetry.py`

 * *Files identical despite different names*

### Comparing `libem-0.0.8/libem/core/trace.py` & `libem-0.0.9/libem/core/trace.py`

 * *Files identical despite different names*

### Comparing `libem-0.0.8/libem/core/util.py` & `libem-0.0.9/libem/core/util.py`

 * *Files identical despite different names*

### Comparing `libem-0.0.8/libem/interface.py` & `libem-0.0.9/libem/interface.py`

 * *Files identical despite different names*

### Comparing `libem-0.0.8/libem/match/function.py` & `libem-0.0.9/libem/match/function.py`

 * *Files identical despite different names*

### Comparing `libem-0.0.8/libem/match/prompt.py` & `libem-0.0.9/libem/match/prompt.py`

 * *Files identical despite different names*

### Comparing `libem-0.0.8/libem/tune/learn/function.py` & `libem-0.0.9/libem/tune/learn/function.py`

 * *Files identical despite different names*

### Comparing `libem-0.0.8/libem/tune/learn/prompt.py` & `libem-0.0.9/libem/tune/learn/prompt.py`

 * *Files identical despite different names*

### Comparing `libem-0.0.8/libem.egg-info/SOURCES.txt` & `libem-0.0.9/libem.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,23 @@
 LICENSE
 README.md
 setup.py
+benchmark/__init__.py
+benchmark/explain.py
+benchmark/run.py
+benchmark/util.py
+benchmark/classic/__init__.py
+benchmark/classic/abt_buy.py
+benchmark/classic/amazon_google.py
+benchmark/classic/beer.py
+benchmark/classic/dblp_acm.py
+benchmark/classic/dblp_scholar.py
+benchmark/classic/fodors_zagats.py
+benchmark/classic/itunes_amazon.py
+benchmark/classic/walmart_amazon.py
 cli/__init__.py
 cli/libem
 libem/__init__.py
 libem/constant.py
 libem/function.py
 libem/interface.py
 libem/parameter.py
@@ -17,37 +30,45 @@
 libem/browse/__init__.py
 libem/browse/function.py
 libem/browse/parameter.py
 libem/browse/prompt.py
 libem/calibrate/__init__.py
 libem/calibrate/function.py
 libem/calibrate/interface.py
-libem/calibrate/optimize/__init__.py
 libem/core/__init__.py
 libem/core/eval.py
 libem/core/exception.py
 libem/core/log.py
 libem/core/model.py
 libem/core/struct.py
 libem/core/telemetry.py
 libem/core/trace.py
 libem/core/util.py
 libem/match/__init__.py
 libem/match/function.py
 libem/match/parameter.py
 libem/match/prompt.py
+libem/optimize/__init__.py
+libem/optimize/interface.py
+libem/optimize/cost/__init__.py
+libem/optimize/cost/cache.py
+libem/optimize/cost/openai.py
 libem/prepare/__init__.py
 libem/prepare/function.py
 libem/prepare/parameter.py
 libem/prepare/prompt.py
 libem/prepare/datasets/__init__.py
 libem/prepare/datasets/abt_buy.py
 libem/prepare/datasets/amazon_google.py
+libem/prepare/datasets/beer.py
 libem/prepare/datasets/dblp_acm.py
 libem/prepare/datasets/dblp_scholar.py
+libem/prepare/datasets/fodors_zagats.py
+libem/prepare/datasets/format_datasets.py
+libem/prepare/datasets/itunes_amazon.py
 libem/prepare/datasets/walmart_amazon.py
 libem/tune/__init__.py
 libem/tune/catalog.py
 libem/tune/function.py
 libem/tune/interface.py
 libem/tune/learn/__init__.py
 libem/tune/learn/function.py
```

### Comparing `libem-0.0.8/serve/run.py` & `libem-0.0.9/serve/run.py`

 * *Files identical despite different names*

