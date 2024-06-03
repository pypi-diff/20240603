# Comparing `tmp/fluke_fl-0.0.5.tar.gz` & `tmp/fluke_fl-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluke_fl-0.0.5.tar", last modified: Wed May 22 10:15:37 2024, max compression
+gzip compressed data, was "fluke_fl-0.1.0.tar", last modified: Mon Jun  3 08:48:41 2024, max compression
```

## Comparing `fluke_fl-0.0.5.tar` & `fluke_fl-0.1.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-05-22 10:15:37.134829 fluke_fl-0.0.5/
--rw-r--r--   0 mirko      (501) staff       (20)    26083 2024-05-16 12:16:36.000000 fluke_fl-0.0.5/LICENSE
--rw-r--r--   0 mirko      (501) staff       (20)    34816 2024-05-22 10:15:37.134522 fluke_fl-0.0.5/PKG-INFO
--rw-r--r--   0 mirko      (501) staff       (20)     3585 2024-05-20 06:05:54.000000 fluke_fl-0.0.5/README.md
-drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-05-22 10:15:37.119082 fluke_fl-0.0.5/fluke/
--rw-r--r--   0 mirko      (501) staff       (20)     8686 2024-05-20 12:55:54.000000 fluke_fl-0.0.5/fluke/__init__.py
-drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-05-22 10:15:37.124249 fluke_fl-0.0.5/fluke/algorithms/
--rw-r--r--   0 mirko      (501) staff       (20)     9464 2024-05-21 10:25:58.000000 fluke_fl-0.0.5/fluke/algorithms/__init__.py
--rw-r--r--   0 mirko      (501) staff       (20)     4190 2024-05-22 09:54:10.000000 fluke_fl-0.0.5/fluke/algorithms/apfl.py
--rw-r--r--   0 mirko      (501) staff       (20)     6799 2024-05-22 10:05:38.000000 fluke_fl-0.0.5/fluke/algorithms/ccvr.py
--rw-r--r--   0 mirko      (501) staff       (20)     3525 2024-05-22 09:23:04.000000 fluke_fl-0.0.5/fluke/algorithms/ditto.py
--rw-r--r--   0 mirko      (501) staff       (20)     5320 2024-05-22 09:23:10.000000 fluke_fl-0.0.5/fluke/algorithms/fedamp.py
--rw-r--r--   0 mirko      (501) staff       (20)      469 2024-05-22 09:24:56.000000 fluke_fl-0.0.5/fluke/algorithms/fedavg.py
--rw-r--r--   0 mirko      (501) staff       (20)     3271 2024-05-22 09:23:25.000000 fluke_fl-0.0.5/fluke/algorithms/fedavgm.py
--rw-r--r--   0 mirko      (501) staff       (20)     4353 2024-05-22 09:23:33.000000 fluke_fl-0.0.5/fluke/algorithms/fedbabu.py
--rw-r--r--   0 mirko      (501) staff       (20)     1637 2024-05-22 09:29:52.000000 fluke_fl-0.0.5/fluke/algorithms/fedbn.py
--rwxr-xr-x   0 mirko      (501) staff       (20)     7778 2024-05-22 09:30:25.000000 fluke_fl-0.0.5/fluke/algorithms/feddyn.py
--rw-r--r--   0 mirko      (501) staff       (20)     2180 2024-05-22 09:32:13.000000 fluke_fl-0.0.5/fluke/algorithms/fedexp.py
--rw-r--r--   0 mirko      (501) staff       (20)     7055 2024-05-22 09:32:36.000000 fluke_fl-0.0.5/fluke/algorithms/fedhp.py
--rw-r--r--   0 mirko      (501) staff       (20)     2043 2024-05-22 09:33:04.000000 fluke_fl-0.0.5/fluke/algorithms/fedlc.py
--rw-r--r--   0 mirko      (501) staff       (20)     9460 2024-05-22 09:33:37.000000 fluke_fl-0.0.5/fluke/algorithms/fednh.py
--rw-r--r--   0 mirko      (501) staff       (20)     3035 2024-05-22 09:34:16.000000 fluke_fl-0.0.5/fluke/algorithms/fednova.py
--rw-r--r--   0 mirko      (501) staff       (20)     3857 2024-05-22 09:34:46.000000 fluke_fl-0.0.5/fluke/algorithms/fedopt.py
--rw-r--r--   0 mirko      (501) staff       (20)     2252 2024-05-22 09:35:13.000000 fluke_fl-0.0.5/fluke/algorithms/fedper.py
--rw-r--r--   0 mirko      (501) staff       (20)     7361 2024-05-22 09:35:49.000000 fluke_fl-0.0.5/fluke/algorithms/fedproto.py
--rw-r--r--   0 mirko      (501) staff       (20)     2404 2024-05-22 09:36:25.000000 fluke_fl-0.0.5/fluke/algorithms/fedprox.py
--rw-r--r--   0 mirko      (501) staff       (20)     4338 2024-05-22 09:37:49.000000 fluke_fl-0.0.5/fluke/algorithms/fedrep.py
--rw-r--r--   0 mirko      (501) staff       (20)     1189 2024-05-22 09:37:52.000000 fluke_fl-0.0.5/fluke/algorithms/fedsgd.py
--rw-r--r--   0 mirko      (501) staff       (20)     2625 2024-05-22 09:38:31.000000 fluke_fl-0.0.5/fluke/algorithms/lg_fedavg.py
--rw-r--r--   0 mirko      (501) staff       (20)     3452 2024-05-22 09:39:06.000000 fluke_fl-0.0.5/fluke/algorithms/moon.py
--rw-r--r--   0 mirko      (501) staff       (20)     6000 2024-05-22 09:39:47.000000 fluke_fl-0.0.5/fluke/algorithms/per_fedavg.py
--rw-r--r--   0 mirko      (501) staff       (20)     5345 2024-05-22 09:40:21.000000 fluke_fl-0.0.5/fluke/algorithms/pfedme.py
--rw-r--r--   0 mirko      (501) staff       (20)     7712 2024-05-22 10:07:02.000000 fluke_fl-0.0.5/fluke/algorithms/scaffold.py
--rw-r--r--   0 mirko      (501) staff       (20)     5841 2024-05-22 10:00:13.000000 fluke_fl-0.0.5/fluke/algorithms/superfed.py
--rw-r--r--   0 mirko      (501) staff       (20)    11606 2024-05-20 18:17:39.000000 fluke_fl-0.0.5/fluke/client.py
--rw-r--r--   0 mirko      (501) staff       (20)    10376 2024-05-16 11:01:26.000000 fluke_fl-0.0.5/fluke/comm.py
-drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-05-22 10:15:37.124797 fluke_fl-0.0.5/fluke/data/
--rw-r--r--   0 mirko      (501) staff       (20)    34115 2024-05-20 18:13:10.000000 fluke_fl-0.0.5/fluke/data/__init__.py
--rw-r--r--   0 mirko      (501) staff       (20)    32705 2024-05-22 09:08:12.000000 fluke_fl-0.0.5/fluke/data/datasets.py
--rw-r--r--   0 mirko      (501) staff       (20)     6875 2024-05-17 12:07:25.000000 fluke_fl-0.0.5/fluke/data/support.py
--rw-r--r--   0 mirko      (501) staff       (20)     7167 2024-05-16 11:01:26.000000 fluke_fl-0.0.5/fluke/evaluation.py
--rw-r--r--   0 mirko      (501) staff       (20)     1842 2024-05-22 07:24:47.000000 fluke_fl-0.0.5/fluke/get.py
--rw-r--r--   0 mirko      (501) staff       (20)    42854 2024-05-20 15:03:29.000000 fluke_fl-0.0.5/fluke/nets.py
--rw-r--r--   0 mirko      (501) staff       (20)     7923 2024-05-21 09:55:17.000000 fluke_fl-0.0.5/fluke/run.py
--rw-r--r--   0 mirko      (501) staff       (20)    15723 2024-05-20 18:19:27.000000 fluke_fl-0.0.5/fluke/server.py
-drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-05-22 10:15:37.125165 fluke_fl-0.0.5/fluke/utils/
--rw-r--r--   0 mirko      (501) staff       (20)    22022 2024-05-17 07:33:13.000000 fluke_fl-0.0.5/fluke/utils/__init__.py
--rw-r--r--   0 mirko      (501) staff       (20)    23035 2024-05-17 12:17:19.000000 fluke_fl-0.0.5/fluke/utils/model.py
-drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-05-22 10:15:37.134107 fluke_fl-0.0.5/fluke_fl.egg-info/
--rw-r--r--   0 mirko      (501) staff       (20)    34816 2024-05-22 10:15:37.000000 fluke_fl-0.0.5/fluke_fl.egg-info/PKG-INFO
--rw-r--r--   0 mirko      (501) staff       (20)     1398 2024-05-22 10:15:37.000000 fluke_fl-0.0.5/fluke_fl.egg-info/SOURCES.txt
--rw-r--r--   0 mirko      (501) staff       (20)        1 2024-05-22 10:15:37.000000 fluke_fl-0.0.5/fluke_fl.egg-info/dependency_links.txt
--rw-r--r--   0 mirko      (501) staff       (20)       68 2024-05-22 10:15:37.000000 fluke_fl-0.0.5/fluke_fl.egg-info/entry_points.txt
--rw-r--r--   0 mirko      (501) staff       (20)       96 2024-05-22 10:15:37.000000 fluke_fl-0.0.5/fluke_fl.egg-info/requires.txt
--rw-r--r--   0 mirko      (501) staff       (20)        6 2024-05-22 10:15:37.000000 fluke_fl-0.0.5/fluke_fl.egg-info/top_level.txt
--rw-r--r--   0 mirko      (501) staff       (20)     1752 2024-05-22 08:49:06.000000 fluke_fl-0.0.5/pyproject.toml
--rw-r--r--   0 mirko      (501) staff       (20)       38 2024-05-22 10:15:37.135011 fluke_fl-0.0.5/setup.cfg
-drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-05-22 10:15:37.133548 fluke_fl-0.0.5/tests/
--rw-r--r--   0 mirko      (501) staff       (20)    10293 2024-05-17 10:06:41.000000 fluke_fl-0.0.5/tests/test_alg.py
--rw-r--r--   0 mirko      (501) staff       (20)     4397 2024-05-16 11:01:26.000000 fluke_fl-0.0.5/tests/test_client.py
--rw-r--r--   0 mirko      (501) staff       (20)     3331 2024-05-16 11:01:26.000000 fluke_fl-0.0.5/tests/test_comm.py
--rw-r--r--   0 mirko      (501) staff       (20)     2130 2024-05-16 11:01:26.000000 fluke_fl-0.0.5/tests/test_core.py
--rw-r--r--   0 mirko      (501) staff       (20)    11108 2024-05-16 11:01:26.000000 fluke_fl-0.0.5/tests/test_data.py
--rw-r--r--   0 mirko      (501) staff       (20)    12738 2024-05-17 12:09:41.000000 fluke_fl-0.0.5/tests/test_datasets.py
--rw-r--r--   0 mirko      (501) staff       (20)     2895 2024-05-16 11:01:26.000000 fluke_fl-0.0.5/tests/test_eval.py
--rw-r--r--   0 mirko      (501) staff       (20)     4620 2024-05-16 11:01:26.000000 fluke_fl-0.0.5/tests/test_nets.py
--rw-r--r--   0 mirko      (501) staff       (20)     3716 2024-05-16 11:01:26.000000 fluke_fl-0.0.5/tests/test_server.py
--rw-r--r--   0 mirko      (501) staff       (20)    13910 2024-05-17 12:13:40.000000 fluke_fl-0.0.5/tests/test_utils.py
+drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-06-03 08:48:41.044742 fluke_fl-0.1.0/
+-rw-r--r--   0 mirko      (501) staff       (20)    26083 2024-05-16 12:16:36.000000 fluke_fl-0.1.0/LICENSE
+-rw-r--r--   0 mirko      (501) staff       (20)    35374 2024-06-03 08:48:41.044422 fluke_fl-0.1.0/PKG-INFO
+-rw-r--r--   0 mirko      (501) staff       (20)     4143 2024-05-22 10:19:59.000000 fluke_fl-0.1.0/README.md
+drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-06-03 08:48:41.027698 fluke_fl-0.1.0/fluke/
+-rw-r--r--   0 mirko      (501) staff       (20)     8686 2024-05-20 12:55:54.000000 fluke_fl-0.1.0/fluke/__init__.py
+drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-06-03 08:48:41.036624 fluke_fl-0.1.0/fluke/algorithms/
+-rw-r--r--   0 mirko      (501) staff       (20)     9464 2024-05-24 13:27:21.000000 fluke_fl-0.1.0/fluke/algorithms/__init__.py
+-rw-r--r--   0 mirko      (501) staff       (20)     4190 2024-05-22 09:54:10.000000 fluke_fl-0.1.0/fluke/algorithms/apfl.py
+-rw-r--r--   0 mirko      (501) staff       (20)     6799 2024-05-22 10:05:38.000000 fluke_fl-0.1.0/fluke/algorithms/ccvr.py
+-rw-r--r--   0 mirko      (501) staff       (20)     3525 2024-05-22 09:23:04.000000 fluke_fl-0.1.0/fluke/algorithms/ditto.py
+-rw-r--r--   0 mirko      (501) staff       (20)     5320 2024-05-22 09:23:10.000000 fluke_fl-0.1.0/fluke/algorithms/fedamp.py
+-rw-r--r--   0 mirko      (501) staff       (20)      469 2024-05-22 09:24:56.000000 fluke_fl-0.1.0/fluke/algorithms/fedavg.py
+-rw-r--r--   0 mirko      (501) staff       (20)     3271 2024-05-22 09:23:25.000000 fluke_fl-0.1.0/fluke/algorithms/fedavgm.py
+-rw-r--r--   0 mirko      (501) staff       (20)     4353 2024-05-22 09:23:33.000000 fluke_fl-0.1.0/fluke/algorithms/fedbabu.py
+-rw-r--r--   0 mirko      (501) staff       (20)     1637 2024-05-22 09:29:52.000000 fluke_fl-0.1.0/fluke/algorithms/fedbn.py
+-rwxr-xr-x   0 mirko      (501) staff       (20)     7778 2024-05-22 09:30:25.000000 fluke_fl-0.1.0/fluke/algorithms/feddyn.py
+-rw-r--r--   0 mirko      (501) staff       (20)     2180 2024-05-22 09:32:13.000000 fluke_fl-0.1.0/fluke/algorithms/fedexp.py
+-rw-r--r--   0 mirko      (501) staff       (20)     7055 2024-05-22 09:32:36.000000 fluke_fl-0.1.0/fluke/algorithms/fedhp.py
+-rw-r--r--   0 mirko      (501) staff       (20)     2240 2024-05-24 14:36:58.000000 fluke_fl-0.1.0/fluke/algorithms/fedlc.py
+-rw-r--r--   0 mirko      (501) staff       (20)     9460 2024-05-22 09:33:37.000000 fluke_fl-0.1.0/fluke/algorithms/fednh.py
+-rw-r--r--   0 mirko      (501) staff       (20)     3035 2024-05-22 09:34:16.000000 fluke_fl-0.1.0/fluke/algorithms/fednova.py
+-rw-r--r--   0 mirko      (501) staff       (20)     3857 2024-05-22 09:34:46.000000 fluke_fl-0.1.0/fluke/algorithms/fedopt.py
+-rw-r--r--   0 mirko      (501) staff       (20)     2252 2024-05-22 09:35:13.000000 fluke_fl-0.1.0/fluke/algorithms/fedper.py
+-rw-r--r--   0 mirko      (501) staff       (20)     7361 2024-05-22 09:35:49.000000 fluke_fl-0.1.0/fluke/algorithms/fedproto.py
+-rw-r--r--   0 mirko      (501) staff       (20)     2404 2024-05-22 09:36:25.000000 fluke_fl-0.1.0/fluke/algorithms/fedprox.py
+-rw-r--r--   0 mirko      (501) staff       (20)     4338 2024-05-22 09:37:49.000000 fluke_fl-0.1.0/fluke/algorithms/fedrep.py
+-rw-r--r--   0 mirko      (501) staff       (20)     1189 2024-05-22 09:37:52.000000 fluke_fl-0.1.0/fluke/algorithms/fedsgd.py
+-rw-r--r--   0 mirko      (501) staff       (20)     2625 2024-05-22 09:38:31.000000 fluke_fl-0.1.0/fluke/algorithms/lg_fedavg.py
+-rw-r--r--   0 mirko      (501) staff       (20)     3452 2024-05-22 09:39:06.000000 fluke_fl-0.1.0/fluke/algorithms/moon.py
+-rw-r--r--   0 mirko      (501) staff       (20)     6000 2024-05-22 09:39:47.000000 fluke_fl-0.1.0/fluke/algorithms/per_fedavg.py
+-rw-r--r--   0 mirko      (501) staff       (20)     5345 2024-05-22 09:40:21.000000 fluke_fl-0.1.0/fluke/algorithms/pfedme.py
+-rw-r--r--   0 mirko      (501) staff       (20)     7712 2024-05-22 10:07:02.000000 fluke_fl-0.1.0/fluke/algorithms/scaffold.py
+-rw-r--r--   0 mirko      (501) staff       (20)     5841 2024-05-22 10:00:13.000000 fluke_fl-0.1.0/fluke/algorithms/superfed.py
+-rw-r--r--   0 mirko      (501) staff       (20)    11606 2024-05-20 18:17:39.000000 fluke_fl-0.1.0/fluke/client.py
+-rw-r--r--   0 mirko      (501) staff       (20)    10376 2024-05-16 11:01:26.000000 fluke_fl-0.1.0/fluke/comm.py
+drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-06-03 08:48:41.037909 fluke_fl-0.1.0/fluke/data/
+-rw-r--r--   0 mirko      (501) staff       (20)    34140 2024-05-23 08:01:50.000000 fluke_fl-0.1.0/fluke/data/__init__.py
+-rw-r--r--   0 mirko      (501) staff       (20)    32718 2024-05-30 12:12:16.000000 fluke_fl-0.1.0/fluke/data/datasets.py
+-rw-r--r--   0 mirko      (501) staff       (20)     6875 2024-05-17 12:07:25.000000 fluke_fl-0.1.0/fluke/data/support.py
+-rw-r--r--   0 mirko      (501) staff       (20)     7167 2024-05-16 11:01:26.000000 fluke_fl-0.1.0/fluke/evaluation.py
+-rw-r--r--   0 mirko      (501) staff       (20)     1842 2024-05-22 07:24:47.000000 fluke_fl-0.1.0/fluke/get.py
+-rw-r--r--   0 mirko      (501) staff       (20)    42854 2024-05-20 15:03:29.000000 fluke_fl-0.1.0/fluke/nets.py
+-rw-r--r--   0 mirko      (501) staff       (20)     7963 2024-05-31 13:33:22.000000 fluke_fl-0.1.0/fluke/run.py
+-rw-r--r--   0 mirko      (501) staff       (20)    15723 2024-05-20 18:19:27.000000 fluke_fl-0.1.0/fluke/server.py
+drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-06-03 08:48:41.038721 fluke_fl-0.1.0/fluke/utils/
+-rw-r--r--   0 mirko      (501) staff       (20)    22714 2024-05-30 13:10:46.000000 fluke_fl-0.1.0/fluke/utils/__init__.py
+-rw-r--r--   0 mirko      (501) staff       (20)    23035 2024-05-17 12:17:19.000000 fluke_fl-0.1.0/fluke/utils/model.py
+drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-06-03 08:48:41.043902 fluke_fl-0.1.0/fluke_fl.egg-info/
+-rw-r--r--   0 mirko      (501) staff       (20)    35374 2024-06-03 08:48:41.000000 fluke_fl-0.1.0/fluke_fl.egg-info/PKG-INFO
+-rw-r--r--   0 mirko      (501) staff       (20)     1398 2024-06-03 08:48:41.000000 fluke_fl-0.1.0/fluke_fl.egg-info/SOURCES.txt
+-rw-r--r--   0 mirko      (501) staff       (20)        1 2024-06-03 08:48:41.000000 fluke_fl-0.1.0/fluke_fl.egg-info/dependency_links.txt
+-rw-r--r--   0 mirko      (501) staff       (20)       68 2024-06-03 08:48:41.000000 fluke_fl-0.1.0/fluke_fl.egg-info/entry_points.txt
+-rw-r--r--   0 mirko      (501) staff       (20)       96 2024-06-03 08:48:41.000000 fluke_fl-0.1.0/fluke_fl.egg-info/requires.txt
+-rw-r--r--   0 mirko      (501) staff       (20)        6 2024-06-03 08:48:41.000000 fluke_fl-0.1.0/fluke_fl.egg-info/top_level.txt
+-rw-r--r--   0 mirko      (501) staff       (20)     1752 2024-06-03 08:47:42.000000 fluke_fl-0.1.0/pyproject.toml
+-rw-r--r--   0 mirko      (501) staff       (20)       38 2024-06-03 08:48:41.044807 fluke_fl-0.1.0/setup.cfg
+drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-06-03 08:48:41.043465 fluke_fl-0.1.0/tests/
+-rw-r--r--   0 mirko      (501) staff       (20)    10293 2024-05-17 10:06:41.000000 fluke_fl-0.1.0/tests/test_alg.py
+-rw-r--r--   0 mirko      (501) staff       (20)     4397 2024-05-16 11:01:26.000000 fluke_fl-0.1.0/tests/test_client.py
+-rw-r--r--   0 mirko      (501) staff       (20)     3331 2024-05-16 11:01:26.000000 fluke_fl-0.1.0/tests/test_comm.py
+-rw-r--r--   0 mirko      (501) staff       (20)     2130 2024-05-16 11:01:26.000000 fluke_fl-0.1.0/tests/test_core.py
+-rw-r--r--   0 mirko      (501) staff       (20)    11108 2024-05-16 11:01:26.000000 fluke_fl-0.1.0/tests/test_data.py
+-rw-r--r--   0 mirko      (501) staff       (20)    12744 2024-05-30 12:13:31.000000 fluke_fl-0.1.0/tests/test_datasets.py
+-rw-r--r--   0 mirko      (501) staff       (20)     2895 2024-05-16 11:01:26.000000 fluke_fl-0.1.0/tests/test_eval.py
+-rw-r--r--   0 mirko      (501) staff       (20)     4620 2024-05-16 11:01:26.000000 fluke_fl-0.1.0/tests/test_nets.py
+-rw-r--r--   0 mirko      (501) staff       (20)     3716 2024-05-16 11:01:26.000000 fluke_fl-0.1.0/tests/test_server.py
+-rw-r--r--   0 mirko      (501) staff       (20)    14020 2024-05-29 07:57:12.000000 fluke_fl-0.1.0/tests/test_utils.py
```

### Comparing `fluke_fl-0.0.5/LICENSE` & `fluke_fl-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/PKG-INFO` & `fluke_fl-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluke-fl
-Version: 0.0.5
+Version: 0.1.0
 Summary: Federated Learning Utility framework for Experimentation and research.
 Author-email: Mirko Polato <mirko.polato@unito.it>
 License:                   GNU LESSER GENERAL PUBLIC LICENSE
                                Version 2.1, February 1999
         
          Copyright (C) 1991, 1999 Free Software Foundation, Inc.
          51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
@@ -573,14 +573,18 @@
 
 Tutorials on how to use ``fluke`` can be found [here](https://makgyver.github.io/fluke/tutorials.html). In the following, you can find some quick tutorials to get started with ``fluke``:
 
 - Getting started with `fluke` API [![Open in Colab](https://img.shields.io/badge/Open_in_Colab-blue?style=flat-square&logo=google-colab&logoColor=yellow&labelColor=gray)
 ](https://colab.research.google.com/github/makgyver/fluke/blob/main/tutorials/fluke_quick_api.ipynb)
 - Run your algorithm in ``fluke`` [![Open in Colab](https://img.shields.io/badge/Open_in_Colab-blue?style=flat-square&logo=google-colab&logoColor=yellow&labelColor=gray)
 ](https://colab.research.google.com/github/makgyver/fluke/blob/main/tutorials/fluke_custom_alg.ipynb)
+- Use your own model with `fluke` [![Open in Colab](https://img.shields.io/badge/Open_in_Colab-blue?style=flat-square&logo=google-colab&logoColor=yellow&labelColor=gray)
+](https://colab.research.google.com/github/makgyver/fluke/blob/main/tutorials/fluke_custom_nn.ipynb)
+- Add your dataset and use it with ``fluke`` [![Open in Colab](https://img.shields.io/badge/Open_in_Colab-blue?style=flat-square&logo=google-colab&logoColor=yellow&labelColor=gray)
+](https://colab.research.google.com/github/makgyver/fluke/blob/main/tutorials/fluke_custom_dataset.ipynb)
 
 ## Contributing
 
 If you have suggestions for how ``fluke`` could be improved, or want to report a bug, open an issue! We'd love all and any contributions.
 
 For more, check out the [Contributing Guide](CONTRIBUTING.md).
```

### Comparing `fluke_fl-0.0.5/README.md` & `fluke_fl-0.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -48,14 +48,18 @@
 
 Tutorials on how to use ``fluke`` can be found [here](https://makgyver.github.io/fluke/tutorials.html). In the following, you can find some quick tutorials to get started with ``fluke``:
 
 - Getting started with `fluke` API [![Open in Colab](https://img.shields.io/badge/Open_in_Colab-blue?style=flat-square&logo=google-colab&logoColor=yellow&labelColor=gray)
 ](https://colab.research.google.com/github/makgyver/fluke/blob/main/tutorials/fluke_quick_api.ipynb)
 - Run your algorithm in ``fluke`` [![Open in Colab](https://img.shields.io/badge/Open_in_Colab-blue?style=flat-square&logo=google-colab&logoColor=yellow&labelColor=gray)
 ](https://colab.research.google.com/github/makgyver/fluke/blob/main/tutorials/fluke_custom_alg.ipynb)
+- Use your own model with `fluke` [![Open in Colab](https://img.shields.io/badge/Open_in_Colab-blue?style=flat-square&logo=google-colab&logoColor=yellow&labelColor=gray)
+](https://colab.research.google.com/github/makgyver/fluke/blob/main/tutorials/fluke_custom_nn.ipynb)
+- Add your dataset and use it with ``fluke`` [![Open in Colab](https://img.shields.io/badge/Open_in_Colab-blue?style=flat-square&logo=google-colab&logoColor=yellow&labelColor=gray)
+](https://colab.research.google.com/github/makgyver/fluke/blob/main/tutorials/fluke_custom_dataset.ipynb)
 
 ## Contributing
 
 If you have suggestions for how ``fluke`` could be improved, or want to report a bug, open an issue! We'd love all and any contributions.
 
 For more, check out the [Contributing Guide](CONTRIBUTING.md).
```

#### html2text {}

```diff
@@ -34,14 +34,22 @@
 started with ``fluke``: - Getting started with `fluke` API [![Open in Colab]
 (https://img.shields.io/badge/Open_in_Colab-blue?style=flat-square&logo=google-
 colab&logoColor=yellow&labelColor=gray) ](https://colab.research.google.com/
 github/makgyver/fluke/blob/main/tutorials/fluke_quick_api.ipynb) - Run your
 algorithm in ``fluke`` [![Open in Colab](https://img.shields.io/badge/
 Open_in_Colab-blue?style=flat-square&logo=google-
 colab&logoColor=yellow&labelColor=gray) ](https://colab.research.google.com/
-github/makgyver/fluke/blob/main/tutorials/fluke_custom_alg.ipynb) ##
+github/makgyver/fluke/blob/main/tutorials/fluke_custom_alg.ipynb) - Use your
+own model with `fluke` [![Open in Colab](https://img.shields.io/badge/
+Open_in_Colab-blue?style=flat-square&logo=google-
+colab&logoColor=yellow&labelColor=gray) ](https://colab.research.google.com/
+github/makgyver/fluke/blob/main/tutorials/fluke_custom_nn.ipynb) - Add your
+dataset and use it with ``fluke`` [![Open in Colab](https://img.shields.io/
+badge/Open_in_Colab-blue?style=flat-square&logo=google-
+colab&logoColor=yellow&labelColor=gray) ](https://colab.research.google.com/
+github/makgyver/fluke/blob/main/tutorials/fluke_custom_dataset.ipynb) ##
 Contributing If you have suggestions for how ``fluke`` could be improved, or
 want to report a bug, open an issue! We'd love all and any contributions. For
 more, check out the [Contributing Guide](CONTRIBUTING.md). ## Authors -
 [**Mirko Polato**](https://makgyver.github.io) - *Idealization*, *Design*,
 *Development*, *Testing*, and *Documentation* - [**Roberto Esposito**]() -
 *Testing* - [**Samuele Fonio**]() - *Testing*
```

### Comparing `fluke_fl-0.0.5/fluke/__init__.py` & `fluke_fl-0.1.0/fluke/__init__.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/fluke/algorithms/__init__.py` & `fluke_fl-0.1.0/fluke/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/fluke/algorithms/apfl.py` & `fluke_fl-0.1.0/fluke/algorithms/apfl.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/fluke/algorithms/ccvr.py` & `fluke_fl-0.1.0/fluke/algorithms/ccvr.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/fluke/algorithms/ditto.py` & `fluke_fl-0.1.0/fluke/algorithms/ditto.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/fluke/algorithms/fedamp.py` & `fluke_fl-0.1.0/fluke/algorithms/fedamp.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/fluke/algorithms/fedavgm.py` & `fluke_fl-0.1.0/fluke/algorithms/fedavgm.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/fluke/algorithms/fedbabu.py` & `fluke_fl-0.1.0/fluke/algorithms/fedbabu.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/fluke/algorithms/fedbn.py` & `fluke_fl-0.1.0/fluke/algorithms/fedbn.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/fluke/algorithms/feddyn.py` & `fluke_fl-0.1.0/fluke/algorithms/feddyn.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/fluke/algorithms/fedexp.py` & `fluke_fl-0.1.0/fluke/algorithms/fedexp.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/fluke/algorithms/fedhp.py` & `fluke_fl-0.1.0/fluke/algorithms/fedhp.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/fluke/algorithms/fedlc.py` & `fluke_fl-0.1.0/fluke/algorithms/fedlc.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,46 +14,54 @@
 
 from ..utils import OptimizerConfigurator  # NOQA
 from ..client import Client  # NOQA
 from ..data import FastDataLoader  # NOQA
 from . import CentralizedFL  # NOQA
 
 
-class FedLCClient(Client):
+class CalibratedLoss(torch.nn.Module):
+
+    def __init__(self, tau: float, label_distrib: torch.Tensor):
+        super().__init__()
+        self.tau = tau
+        self.label_distrib = label_distrib
 
-    def __calibrated_loss(self, logit: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
+    def forward(self, logit: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
         cal_logit = torch.exp(
             logit
             - (
-                self.hyper_params.tau
+                self.tau
                 * torch.pow(self.label_distrib, -1 / 4)
                 .unsqueeze(0)
                 .expand((logit.shape[0], -1))
             )
         )
         y_logit = torch.gather(cal_logit, dim=-1, index=y.unsqueeze(1))
         loss = -torch.log(y_logit / cal_logit.sum(dim=-1, keepdim=True))
         return loss.sum() / logit.shape[0]
 
+
+class FedLCClient(Client):
+
     def __init__(self,
                  index: int,
                  train_set: FastDataLoader,
                  test_set: FastDataLoader,
                  optimizer_cfg: OptimizerConfigurator,
                  loss_fn: Callable,  # ignored
                  local_epochs: int,
                  tau: float):
-        super().__init__(index, train_set, test_set, optimizer_cfg, None, local_epochs)
+        super().__init__(index, train_set, test_set, optimizer_cfg, loss_fn, local_epochs)
         self.hyper_params.update(tau=tau)
         all_labels = self.train_set.tensors[1].tolist()
         label_counter = Counter(all_labels)
         self.label_distrib = torch.zeros(self.train_set.num_labels, device=self.device)
         for cls, count in label_counter.items():
             self.label_distrib[cls] = max(1e-8, count)
 
-        self.hyper_params.loss_fn = self.__calibrated_loss
+        self.hyper_params.loss_fn = CalibratedLoss(tau, self.label_distrib)
 
 
 class FedLC(CentralizedFL):
 
     def get_client_class(self) -> Client:
         return FedLCClient
```

### Comparing `fluke_fl-0.0.5/fluke/algorithms/fednh.py` & `fluke_fl-0.1.0/fluke/algorithms/fednh.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/fluke/algorithms/fednova.py` & `fluke_fl-0.1.0/fluke/algorithms/fednova.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/fluke/algorithms/fedopt.py` & `fluke_fl-0.1.0/fluke/algorithms/fedopt.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/fluke/algorithms/fedper.py` & `fluke_fl-0.1.0/fluke/algorithms/fedper.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/fluke/algorithms/fedproto.py` & `fluke_fl-0.1.0/fluke/algorithms/fedproto.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/fluke/algorithms/fedprox.py` & `fluke_fl-0.1.0/fluke/algorithms/fedprox.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/fluke/algorithms/fedrep.py` & `fluke_fl-0.1.0/fluke/algorithms/fedrep.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/fluke/algorithms/fedsgd.py` & `fluke_fl-0.1.0/fluke/algorithms/fedsgd.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/fluke/algorithms/lg_fedavg.py` & `fluke_fl-0.1.0/fluke/algorithms/lg_fedavg.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/fluke/algorithms/moon.py` & `fluke_fl-0.1.0/fluke/algorithms/moon.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/fluke/algorithms/per_fedavg.py` & `fluke_fl-0.1.0/fluke/algorithms/per_fedavg.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/fluke/algorithms/pfedme.py` & `fluke_fl-0.1.0/fluke/algorithms/pfedme.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/fluke/algorithms/scaffold.py` & `fluke_fl-0.1.0/fluke/algorithms/scaffold.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/fluke/algorithms/superfed.py` & `fluke_fl-0.1.0/fluke/algorithms/superfed.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/fluke/client.py` & `fluke_fl-0.1.0/fluke/client.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/fluke/comm.py` & `fluke_fl-0.1.0/fluke/comm.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/fluke/data/__init__.py` & `fluke_fl-0.1.0/fluke/data/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -436,22 +436,22 @@
     def quantity_skew(self,
                       X: torch.Tensor,
                       y: torch.Tensor,  # not used
                       n: int,
                       min_quantity: int = 2,
                       alpha: float = 4.) -> list[torch.Tensor]:
         r"""
-        Distribute the examples across the users according to the following probability density
+        Distribute the examples across the clients according to the following probability density
         function: :math:`P(x; a) = a x^{a-1}`
         where :math:`x` is the id of a client (:math:`x \in [0, n-1]`), and ``a = alpha > 0`` with
 
         - ``alpha = 1``: examples are equidistributed across clients;
-        - ``alpha = 2``: the examples are "linearly" distributed across users;
+        - ``alpha = 2``: the examples are "linearly" distributed across clients;
         - ``alpha >= 3``: the examples are power law distributed;
-        - ``alpha`` :math:`\rightarrow \infty`: all users but one have ``min_quantity`` examples,
+        - ``alpha`` :math:`\rightarrow \infty`: all clients but one have ``min_quantity`` examples,
           and the remaining user all the rest.
 
         Each client is guaranteed to have at least ``min_quantity`` examples.
 
         Args:
             X (torch.Tensor): The examples.
             y (torch.Tensor): The labels. Not used.
@@ -527,18 +527,18 @@
                             y: torch.Tensor,
                             n: int,
                             class_per_client: int = 2) -> list[torch.Tensor]:
         """
         This method distribute the data across client according to a specific type of skewness of
         the lables. Specifically:
         suppose each party only has data samples of ``class_per_client`` different labels.
-        We first randomly assign k different label IDs to each party. Then, for the samples of each
-        label, we randomly and equally divide them into the parties which own the label.
-        In this way, the number of labels in each party is fixed, and there is no overlap between
-        the samples of different parties.
+        We first randomly assign ``class_per_client`` different label IDs to each party.
+        Then, for the samples of each label, we randomly and equally divide them into the parties
+        which own the label. In this way, the number of labels in each party is fixed, and there is
+        no overlap between the samples of different parties.
         See: https://arxiv.org/pdf/2102.02079.pdf
 
         Args:
             X (torch.Tensor): The examples. Not used.
             y (torch.Tensor): The lables.
             n (int): The number of clients upon which the examples are distributed.
             class_per_client (int, optional): The number of classes per client. Defaults to 2.
```

### Comparing `fluke_fl-0.0.5/fluke/data/datasets.py` & `fluke_fl-0.1.0/fluke/data/datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         Raises:
             ValueError: If the dataset is not supported or the name is wrong.
         """
         if name not in Datasets._DATASET_MAP:
             try:
                 data_fun = get_class_from_qualified_name(name)
                 return data_fun(**kwargs)
-            except ModuleNotFoundError | TypeError:
+            except (ModuleNotFoundError, TypeError, ValueError):
                 raise ValueError(f"Dataset {name} not found. The supported datasets are: " +
                                  ", ".join(Datasets._DATASET_MAP.keys()) + ".")
 
         return Datasets._DATASET_MAP[name](**kwargs)
 
     @classmethod
     def MNIST(cls,
```

### Comparing `fluke_fl-0.0.5/fluke/data/support.py` & `fluke_fl-0.1.0/fluke/data/support.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/fluke/evaluation.py` & `fluke_fl-0.1.0/fluke/evaluation.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/fluke/get.py` & `fluke_fl-0.1.0/fluke/get.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/fluke/nets.py` & `fluke_fl-0.1.0/fluke/nets.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/fluke/run.py` & `fluke_fl-0.1.0/fluke/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,34 +38,39 @@
     GlobalSettings().set_seed(cfg.exp.seed)
     GlobalSettings().set_device(cfg.exp.device)
     data_container = Datasets.get(**cfg.data.dataset)
 
     device = GlobalSettings().get_device()
 
     train_loader = FastDataLoader(*data_container.train,
-                                  batch_size=cfg.method.hyperparameters.client.batch_size,
+                                  batch_size=cfg.client.batch_size,
                                   num_labels=data_container.num_classes,
                                   shuffle=True)
     test_loader = FastDataLoader(*data_container.test,
                                  batch_size=10,
                                  num_labels=data_container.num_classes,
                                  shuffle=False)
 
-    # , **cfg.method.hyperparameters.net_args)
-    model = get_model(mname=cfg.method.hyperparameters.model)
-    optimizer_cfg = OptimizerConfigurator(optimizer_cfg=cfg.method.hyperparameters.client.optimizer,
-                                          scheduler_cfg=cfg.method.hyperparameters.client.scheduler)
+    model = get_model(mname=cfg.model)
+    if "name" not in cfg.client.optimizer:
+        cfg.client.optimizer.name = torch.optim.SGD
+    optimizer_cfg = OptimizerConfigurator(optimizer_cfg=cfg.client.optimizer,
+                                          scheduler_cfg=cfg.client.scheduler)
     optimizer, scheduler = optimizer_cfg(model)
-    criterion = get_loss(cfg.method.hyperparameters.client.loss)
+    criterion = get_loss(cfg.client.loss)
     evaluator = ClassificationEval(criterion, data_container.num_classes, device)
     history = []
 
     model.to(device)
     epochs = epochs if epochs > 0 else int(
         max(1, cfg.protocol.n_rounds * cfg.protocol.eligible_perc))
+
+    rich.print(f"Centralized Learning [ #Epochs = {epochs} ]")
+    rich.print()
+
     for e in range(epochs):
         model.train()
         rich.print(f"Epoch {e+1}")
         loss = None
         for _, (X, y) in track(enumerate(train_loader), total=train_loader.n_batches):
             X, y = X.to(device), y.to(device)
             optimizer.zero_grad()
@@ -144,15 +149,15 @@
     if epochs == 0:
         epochs = max(100, int(cfg.protocol.n_rounds *
                               hp.client.local_epochs * cfg.protocol.eligible_perc))
     progress = track(enumerate(zip(clients_tr_data, clients_te_data)),
                      total=len(clients_tr_data),
                      description="Clients training...")
     for i, (train_loader, test_loader) in progress:
-        rich.print(f"Client [{i}]")
+        rich.print(f"Client [{i}/{cfg.protocol.n_clients}]")
         model = get_model(mname=hp.model)  # , **hp.net_args)
         hp.client.optimizer.name = torch.optim.SGD
         optimizer_cfg = OptimizerConfigurator(optimizer_cfg=hp.client.optimizer,
                                               scheduler_cfg=hp.client.scheduler)
         optimizer, scheduler = optimizer_cfg(model)
         evaluator = ClassificationEval(criterion,
                                        data_splitter.data_container.num_classes,
```

### Comparing `fluke_fl-0.0.5/fluke/server.py` & `fluke_fl-0.1.0/fluke/server.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/fluke/utils/__init__.py` & `fluke_fl-0.1.0/fluke/utils/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -528,14 +528,41 @@
         with open(config_alg_path) as f:
             config_alg = yaml.safe_load(f)
 
         self.update(**config_exp)
         self.update(method=config_alg)
         self._validate()
 
+    @property
+    def client(self) -> DDict:
+        """Get quick access to the client hyperparameters.
+
+        Returns:
+            DDict: The client hyperparameters.
+        """
+        return self.method.hyperparameters.client
+
+    @property
+    def server(self) -> DDict:
+        """Get quick access to the server hyperparameters.
+
+        Returns:
+            DDict: The server hyperparameters.
+        """
+        return self.method.hyperparameters.server
+
+    @property
+    def model(self) -> DDict:
+        """Get quick access to the model hyperparameters.
+
+        Returns:
+            DDict: The model hyperparameters.
+        """
+        return self.method.hyperparameters.model
+
     def _validate(self) -> bool:
 
         EXP_OPT_KEYS = {
             "device": "cpu",
             "seed": 42
         }
```

### Comparing `fluke_fl-0.0.5/fluke/utils/model.py` & `fluke_fl-0.1.0/fluke/utils/model.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/fluke_fl.egg-info/PKG-INFO` & `fluke_fl-0.1.0/fluke_fl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluke-fl
-Version: 0.0.5
+Version: 0.1.0
 Summary: Federated Learning Utility framework for Experimentation and research.
 Author-email: Mirko Polato <mirko.polato@unito.it>
 License:                   GNU LESSER GENERAL PUBLIC LICENSE
                                Version 2.1, February 1999
         
          Copyright (C) 1991, 1999 Free Software Foundation, Inc.
          51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
@@ -573,14 +573,18 @@
 
 Tutorials on how to use ``fluke`` can be found [here](https://makgyver.github.io/fluke/tutorials.html). In the following, you can find some quick tutorials to get started with ``fluke``:
 
 - Getting started with `fluke` API [![Open in Colab](https://img.shields.io/badge/Open_in_Colab-blue?style=flat-square&logo=google-colab&logoColor=yellow&labelColor=gray)
 ](https://colab.research.google.com/github/makgyver/fluke/blob/main/tutorials/fluke_quick_api.ipynb)
 - Run your algorithm in ``fluke`` [![Open in Colab](https://img.shields.io/badge/Open_in_Colab-blue?style=flat-square&logo=google-colab&logoColor=yellow&labelColor=gray)
 ](https://colab.research.google.com/github/makgyver/fluke/blob/main/tutorials/fluke_custom_alg.ipynb)
+- Use your own model with `fluke` [![Open in Colab](https://img.shields.io/badge/Open_in_Colab-blue?style=flat-square&logo=google-colab&logoColor=yellow&labelColor=gray)
+](https://colab.research.google.com/github/makgyver/fluke/blob/main/tutorials/fluke_custom_nn.ipynb)
+- Add your dataset and use it with ``fluke`` [![Open in Colab](https://img.shields.io/badge/Open_in_Colab-blue?style=flat-square&logo=google-colab&logoColor=yellow&labelColor=gray)
+](https://colab.research.google.com/github/makgyver/fluke/blob/main/tutorials/fluke_custom_dataset.ipynb)
 
 ## Contributing
 
 If you have suggestions for how ``fluke`` could be improved, or want to report a bug, open an issue! We'd love all and any contributions.
 
 For more, check out the [Contributing Guide](CONTRIBUTING.md).
```

### Comparing `fluke_fl-0.0.5/fluke_fl.egg-info/SOURCES.txt` & `fluke_fl-0.1.0/fluke_fl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/pyproject.toml` & `fluke_fl-0.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 where = ["."]  # list of folders that contain the packages (["."] by default)
 include = ["fluke", "fluke.data", "fluke.utils", "fluke.algorithms"]  # package names should match these glob patterns (["*"] by default)
 exclude = []  # exclude packages matching these glob patterns (empty by default)
 namespaces = false  # to disable scanning PEP 420 namespaces (true by default)
 
 [project]
 name = "fluke-fl"
-version = "0.0.5"
+version = "0.1.0"
 authors = [
   { name="Mirko Polato", email="mirko.polato@unito.it" },
 ]
 description = "Federated Learning Utility framework for Experimentation and research."
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
```

### Comparing `fluke_fl-0.0.5/tests/test_alg.py` & `fluke_fl-0.1.0/tests/test_alg.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/tests/test_client.py` & `fluke_fl-0.1.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/tests/test_comm.py` & `fluke_fl-0.1.0/tests/test_comm.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/tests/test_core.py` & `fluke_fl-0.1.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/tests/test_data.py` & `fluke_fl-0.1.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/tests/test_datasets.py` & `fluke_fl-0.1.0/tests/test_datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,25 +283,25 @@
     assert cinic.test[1].shape == torch.Size([90000])
     assert cinic.num_classes == len(
         set(cinic.train[1].unique().tolist() + cinic.test[1].unique().tolist()))
     assert cinic.num_classes == 10
 
 
 if __name__ == "__main__":
-    # test_mnist()
+    test_mnist()
     # test_mnist4d()
     # test_emnist()
     # test_svhn()
     # test_cifar10()
     # test_cifar100()
     # test_mnistm()
     # test_tinyimagenet()
-    test_femnist()
-    test_femnist_dig()
-    test_femnist_upp()
-    test_femnist_low()
+    # test_femnist()
+    # test_femnist_dig()
+    # test_femnist_upp()
+    # test_femnist_low()
     # test_shakespeare()
     # test_fashion_mnist()
     # test_cinic10()
 
     # 98% coverate on datasets.py
     # 88% coverage on support.py
```

### Comparing `fluke_fl-0.0.5/tests/test_eval.py` & `fluke_fl-0.1.0/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/tests/test_nets.py` & `fluke_fl-0.1.0/tests/test_nets.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/tests/test_server.py` & `fluke_fl-0.1.0/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.5/tests/test_utils.py` & `fluke_fl-0.1.0/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,14 +226,17 @@
     except Exception:
         pytest.fail("Unexpected error!")
 
     assert conf.protocol.n_clients == 100
     # assert conf.data.dataset.name == "mnist"
     assert conf.exp.seed == 42
     # assert conf.logger.name == "local"
+    assert conf.client.local_epochs == 5
+    assert conf.server.weighted
+    assert conf.model == "MNIST_2NN"
 
     assert str(conf) == "fluke.algorithms.fedavg.FedAVG" + \
         "_data(mnist, iid)_proto(C100, R50,E0.1)_seed(42)"
 
     cfg = dict({"protocol": {}, "data": {}, "exp": {}, "logger": {}})
     cfg_alg = dict({"name": "fluke.algorithms.fedavg.FedAVG", "hyperparameters": {
                    "server": {}, "client": {}, "model": "MNIST_2NN"}})
```

