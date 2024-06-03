# Comparing `tmp/autogluon.common-1.1.1b20240601.tar.gz` & `tmp/autogluon.common-1.1.1b20240602.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.common-1.1.1b20240601.tar", last modified: Sat Jun  1 09:04:29 2024, max compression
+gzip compressed data, was "autogluon.common-1.1.1b20240602.tar", last modified: Sun Jun  2 09:03:56 2024, max compression
```

## Comparing `autogluon.common-1.1.1b20240601.tar` & `autogluon.common-1.1.1b20240602.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:04:29.580782 autogluon.common-1.1.1b20240601/
--rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)    11749 2024-06-01 09:04:29.580782 autogluon.common-1.1.1b20240601/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 09:04:29.580782 autogluon.common-1.1.1b20240601/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:04:29.568781 autogluon.common-1.1.1b20240601/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:04:29.568781 autogluon.common-1.1.1b20240601/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:04:29.572782 autogluon.common-1.1.1b20240601/src/autogluon/common/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:04:29.572782 autogluon.common-1.1.1b20240601/src/autogluon/common/features/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22823 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/features/feature_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/features/infer_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/features/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:04:29.572782 autogluon.common-1.1.1b20240601/src/autogluon/common/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9956 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/loaders/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/loaders/load_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/loaders/load_pd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/loaders/load_pkl.py
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/loaders/load_pointer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/loaders/load_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/loaders/load_str.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/loaders/load_zip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:04:29.576782 autogluon.common-1.1.1b20240601/src/autogluon/common/model_filter/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/model_filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/model_filter/_model_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:04:29.576782 autogluon.common-1.1.1b20240601/src/autogluon/common/savers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/savers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/savers/save_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     7646 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/savers/save_pd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/savers/save_pkl.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/savers/save_pointer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/savers/save_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/space.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:04:29.576782 autogluon.common-1.1.1b20240601/src/autogluon/common/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/utils/compression_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     9408 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/utils/deprecated_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/utils/distribute_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/utils/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/utils/lite.py
--rw-r--r--   0 runner    (1001) docker     (127)     6089 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/utils/multiprocessing_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/utils/nvutil.py
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/utils/pandas_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/utils/path_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7398 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/utils/resource_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15841 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/utils/s3_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/utils/simulation_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/utils/system_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     7275 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/utils/try_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     7325 2024-06-01 09:04:19.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-06-01 09:04:28.000000 autogluon.common-1.1.1b20240601/src/autogluon/common/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:04:29.572782 autogluon.common-1.1.1b20240601/src/autogluon.common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11749 2024-06-01 09:04:29.000000 autogluon.common-1.1.1b20240601/src/autogluon.common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-06-01 09:04:29.000000 autogluon.common-1.1.1b20240601/src/autogluon.common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 09:04:29.000000 autogluon.common-1.1.1b20240601/src/autogluon.common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-01 09:04:29.000000 autogluon.common-1.1.1b20240601/src/autogluon.common.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-06-01 09:04:29.000000 autogluon.common-1.1.1b20240601/src/autogluon.common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-01 09:04:29.000000 autogluon.common-1.1.1b20240601/src/autogluon.common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 09:04:29.000000 autogluon.common-1.1.1b20240601/src/autogluon.common.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 09:03:56.996502 autogluon.common-1.1.1b20240602/
+-rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)    11749 2024-06-02 09:03:56.996502 autogluon.common-1.1.1b20240602/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 09:03:56.996502 autogluon.common-1.1.1b20240602/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 09:03:56.988502 autogluon.common-1.1.1b20240602/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 09:03:56.988502 autogluon.common-1.1.1b20240602/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 09:03:56.988502 autogluon.common-1.1.1b20240602/src/autogluon/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 09:03:56.992502 autogluon.common-1.1.1b20240602/src/autogluon/common/features/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22823 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/features/feature_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/features/infer_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/features/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 09:03:56.992502 autogluon.common-1.1.1b20240602/src/autogluon/common/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9956 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/loaders/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/loaders/load_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/loaders/load_pd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/loaders/load_pkl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/loaders/load_pointer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/loaders/load_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/loaders/load_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/loaders/load_zip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 09:03:56.992502 autogluon.common-1.1.1b20240602/src/autogluon/common/model_filter/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/model_filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/model_filter/_model_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 09:03:56.992502 autogluon.common-1.1.1b20240602/src/autogluon/common/savers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/savers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/savers/save_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7646 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/savers/save_pd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/savers/save_pkl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/savers/save_pointer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/savers/save_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/space.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 09:03:56.996502 autogluon.common-1.1.1b20240602/src/autogluon/common/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/utils/compression_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9408 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/utils/deprecated_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/utils/distribute_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/utils/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/utils/lite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6089 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/utils/multiprocessing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/utils/nvutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/utils/pandas_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/utils/path_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7398 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/utils/resource_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15841 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/utils/s3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/utils/simulation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/utils/system_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7275 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/utils/try_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7325 2024-06-02 09:03:48.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-06-02 09:03:56.000000 autogluon.common-1.1.1b20240602/src/autogluon/common/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 09:03:56.988502 autogluon.common-1.1.1b20240602/src/autogluon.common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11749 2024-06-02 09:03:56.000000 autogluon.common-1.1.1b20240602/src/autogluon.common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-06-02 09:03:56.000000 autogluon.common-1.1.1b20240602/src/autogluon.common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 09:03:56.000000 autogluon.common-1.1.1b20240602/src/autogluon.common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-02 09:03:56.000000 autogluon.common-1.1.1b20240602/src/autogluon.common.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-06-02 09:03:56.000000 autogluon.common-1.1.1b20240602/src/autogluon.common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-02 09:03:56.000000 autogluon.common-1.1.1b20240602/src/autogluon.common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 09:03:56.000000 autogluon.common-1.1.1b20240602/src/autogluon.common.egg-info/zip-safe
```

### Comparing `autogluon.common-1.1.1b20240601/LICENSE` & `autogluon.common-1.1.1b20240602/LICENSE`

 * *Files identical despite different names*

### Comparing `autogluon.common-1.1.1b20240601/PKG-INFO` & `autogluon.common-1.1.1b20240602/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.common
-Version: 1.1.1b20240601
+Version: 1.1.1b20240602
 Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.common-1.1.1b20240601/setup.py` & `autogluon.common-1.1.1b20240602/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-1.1.1b20240601/src/autogluon/common/features/feature_metadata.py` & `autogluon.common-1.1.1b20240602/src/autogluon/common/features/feature_metadata.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-1.1.1b20240601/src/autogluon/common/features/infer_types.py` & `autogluon.common-1.1.1b20240602/src/autogluon/common/features/infer_types.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-1.1.1b20240601/src/autogluon/common/features/types.py` & `autogluon.common-1.1.1b20240602/src/autogluon/common/features/types.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-1.1.1b20240601/src/autogluon/common/loaders/_utils.py` & `autogluon.common-1.1.1b20240602/src/autogluon/common/loaders/_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-1.1.1b20240601/src/autogluon/common/loaders/load_json.py` & `autogluon.common-1.1.1b20240602/src/autogluon/common/loaders/load_json.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-1.1.1b20240601/src/autogluon/common/loaders/load_pd.py` & `autogluon.common-1.1.1b20240602/src/autogluon/common/loaders/load_pd.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-1.1.1b20240601/src/autogluon/common/loaders/load_pkl.py` & `autogluon.common-1.1.1b20240602/src/autogluon/common/loaders/load_pkl.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-1.1.1b20240601/src/autogluon/common/loaders/load_pointer.py` & `autogluon.common-1.1.1b20240602/src/autogluon/common/loaders/load_pointer.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-1.1.1b20240601/src/autogluon/common/loaders/load_s3.py` & `autogluon.common-1.1.1b20240602/src/autogluon/common/loaders/load_s3.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-1.1.1b20240601/src/autogluon/common/loaders/load_str.py` & `autogluon.common-1.1.1b20240602/src/autogluon/common/loaders/load_str.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-1.1.1b20240601/src/autogluon/common/model_filter/_model_filter.py` & `autogluon.common-1.1.1b20240602/src/autogluon/common/model_filter/_model_filter.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-1.1.1b20240601/src/autogluon/common/savers/save_json.py` & `autogluon.common-1.1.1b20240602/src/autogluon/common/savers/save_json.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-1.1.1b20240601/src/autogluon/common/savers/save_pd.py` & `autogluon.common-1.1.1b20240602/src/autogluon/common/savers/save_pd.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-1.1.1b20240601/src/autogluon/common/savers/save_pkl.py` & `autogluon.common-1.1.1b20240602/src/autogluon/common/savers/save_pkl.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-1.1.1b20240601/src/autogluon/common/savers/save_str.py` & `autogluon.common-1.1.1b20240602/src/autogluon/common/savers/save_str.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-1.1.1b20240601/src/autogluon/common/space.py` & `autogluon.common-1.1.1b20240602/src/autogluon/common/space.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-1.1.1b20240601/src/autogluon/common/utils/compression_utils.py` & `autogluon.common-1.1.1b20240602/src/autogluon/common/utils/compression_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-1.1.1b20240601/src/autogluon/common/utils/deprecated_utils.py` & `autogluon.common-1.1.1b20240602/src/autogluon/common/utils/deprecated_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-1.1.1b20240601/src/autogluon/common/utils/distribute_utils.py` & `autogluon.common-1.1.1b20240602/src/autogluon/common/utils/distribute_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-1.1.1b20240601/src/autogluon/common/utils/file_utils.py` & `autogluon.common-1.1.1b20240602/src/autogluon/common/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-1.1.1b20240601/src/autogluon/common/utils/log_utils.py` & `autogluon.common-1.1.1b20240602/src/autogluon/common/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-1.1.1b20240601/src/autogluon/common/utils/multiprocessing_utils.py` & `autogluon.common-1.1.1b20240602/src/autogluon/common/utils/multiprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-1.1.1b20240601/src/autogluon/common/utils/nvutil.py` & `autogluon.common-1.1.1b20240602/src/autogluon/common/utils/nvutil.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-1.1.1b20240601/src/autogluon/common/utils/pandas_utils.py` & `autogluon.common-1.1.1b20240602/src/autogluon/common/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-1.1.1b20240601/src/autogluon/common/utils/path_converter.py` & `autogluon.common-1.1.1b20240602/src/autogluon/common/utils/path_converter.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-1.1.1b20240601/src/autogluon/common/utils/resource_utils.py` & `autogluon.common-1.1.1b20240602/src/autogluon/common/utils/resource_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-1.1.1b20240601/src/autogluon/common/utils/s3_utils.py` & `autogluon.common-1.1.1b20240602/src/autogluon/common/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-1.1.1b20240601/src/autogluon/common/utils/simulation_utils.py` & `autogluon.common-1.1.1b20240602/src/autogluon/common/utils/simulation_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-1.1.1b20240601/src/autogluon/common/utils/system_info.py` & `autogluon.common-1.1.1b20240602/src/autogluon/common/utils/system_info.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-1.1.1b20240601/src/autogluon/common/utils/try_import.py` & `autogluon.common-1.1.1b20240602/src/autogluon/common/utils/try_import.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-1.1.1b20240601/src/autogluon/common/utils/utils.py` & `autogluon.common-1.1.1b20240602/src/autogluon/common/utils/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-1.1.1b20240601/src/autogluon.common.egg-info/PKG-INFO` & `autogluon.common-1.1.1b20240602/src/autogluon.common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.common
-Version: 1.1.1b20240601
+Version: 1.1.1b20240602
 Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.common-1.1.1b20240601/src/autogluon.common.egg-info/SOURCES.txt` & `autogluon.common-1.1.1b20240602/src/autogluon.common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

