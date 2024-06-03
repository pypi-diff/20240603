# Comparing `tmp/torchtnt_nightly-2024.6.1.tar.gz` & `tmp/torchtnt_nightly-2024.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchtnt_nightly-2024.6.1.tar", last modified: Sat Jun  1 11:27:49 2024, max compression
+gzip compressed data, was "torchtnt_nightly-2024.6.2.tar", last modified: Sun Jun  2 11:26:30 2024, max compression
```

## Comparing `torchtnt_nightly-2024.6.1.tar` & `torchtnt_nightly-2024.6.2.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:27:49.252618 torchtnt_nightly-2024.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-06-01 11:27:49.252618 torchtnt_nightly-2024.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 11:27:49.252618 torchtnt_nightly-2024.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:27:49.236618 torchtnt_nightly-2024.6.1/torchtnt/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:27:49.236618 torchtnt_nightly-2024.6.1/torchtnt/framework/
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/framework/_callback_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/framework/_loop_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/framework/_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/framework/_unit_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    36138 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/framework/auto_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/framework/callback.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:27:49.240618 torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/_checkpoint_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19248 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/base_checkpointer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/base_csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/checkpointer_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    15782 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/dcp_saver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/empty_cuda_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/garbage_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     5604 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/iteration_time_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/lambda_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/learning_rate_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/memory_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/module_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/progress_reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/pytorch_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/slow_rank_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/system_resources_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8965 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/throughput_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/time_limit_interrupter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/time_wait_for_batch_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/torch_compile.py
--rw-r--r--   0 runner    (1001) docker     (127)    17312 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/torchsnapshot_saver.py
--rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/tqdm_progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/train_progress_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/framework/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/framework/fit.py
--rw-r--r--   0 runner    (1001) docker     (127)     7557 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/framework/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/framework/state.py
--rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/framework/train.py
--rw-r--r--   0 runner    (1001) docker     (127)    22471 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/framework/unit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/framework/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:27:49.244618 torchtnt_nightly-2024.6.1/torchtnt/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29240 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/checkpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:27:49.248618 torchtnt_nightly-2024.6.1/torchtnt/utils/data/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/data/data_prefetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    21149 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/data/iterators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/data/multi_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/data/profile_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/data/synthetic_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11546 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    23329 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)     9912 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/early_stop_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/flops.py
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/fsdp_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/fsspec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:27:49.248618 torchtnt_nightly-2024.6.1/torchtnt/utils/loggers/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/loggers/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/loggers/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/loggers/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/loggers/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/loggers/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/loggers/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/loggers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/memory_snapshot_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    27230 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/module_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/oom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/precision.py
--rw-r--r--   0 runner    (1001) docker     (127)    14932 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/prepare_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/rank_zero_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/stateful.py
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/swa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15408 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/tqdm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-06-01 11:25:48.000000 torchtnt_nightly-2024.6.1/torchtnt/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:27:49.248618 torchtnt_nightly-2024.6.1/torchtnt_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-06-01 11:27:49.000000 torchtnt_nightly-2024.6.1/torchtnt_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-06-01 11:27:49.000000 torchtnt_nightly-2024.6.1/torchtnt_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 11:27:49.000000 torchtnt_nightly-2024.6.1/torchtnt_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-06-01 11:27:49.000000 torchtnt_nightly-2024.6.1/torchtnt_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-01 11:27:49.000000 torchtnt_nightly-2024.6.1/torchtnt_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 11:27:49.000000 torchtnt_nightly-2024.6.1/torchtnt_nightly.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 11:26:30.076145 torchtnt_nightly-2024.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-06-02 11:26:30.076145 torchtnt_nightly-2024.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 11:26:30.076145 torchtnt_nightly-2024.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 11:26:30.064145 torchtnt_nightly-2024.6.2/torchtnt/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 11:26:30.064145 torchtnt_nightly-2024.6.2/torchtnt/framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/framework/_callback_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/framework/_loop_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/framework/_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/framework/_unit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36138 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/framework/auto_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/framework/callback.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 11:26:30.068145 torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/_checkpoint_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19248 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/base_checkpointer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/base_csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/checkpointer_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15782 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/dcp_saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/empty_cuda_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/garbage_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5604 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/iteration_time_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/lambda_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/learning_rate_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/memory_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/module_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/progress_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/pytorch_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/slow_rank_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/system_resources_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8965 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/throughput_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/time_limit_interrupter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/time_wait_for_batch_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/torch_compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17312 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/torchsnapshot_saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/tqdm_progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/train_progress_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/framework/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/framework/fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7557 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/framework/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/framework/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/framework/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22471 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/framework/unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/framework/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 11:26:30.072145 torchtnt_nightly-2024.6.2/torchtnt/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29240 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/checkpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 11:26:30.076145 torchtnt_nightly-2024.6.2/torchtnt/utils/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/data/data_prefetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21149 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/data/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/data/multi_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/data/profile_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/data/synthetic_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11546 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23329 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9912 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/early_stop_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/flops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/fsdp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/fsspec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 11:26:30.076145 torchtnt_nightly-2024.6.2/torchtnt/utils/loggers/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/loggers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/loggers/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/loggers/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/loggers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/loggers/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/loggers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/memory_snapshot_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27230 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/module_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/oom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14932 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/prepare_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/rank_zero_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/stateful.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/swa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15408 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-06-02 11:24:23.000000 torchtnt_nightly-2024.6.2/torchtnt/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 11:26:30.076145 torchtnt_nightly-2024.6.2/torchtnt_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-06-02 11:26:30.000000 torchtnt_nightly-2024.6.2/torchtnt_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-06-02 11:26:30.000000 torchtnt_nightly-2024.6.2/torchtnt_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 11:26:30.000000 torchtnt_nightly-2024.6.2/torchtnt_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-06-02 11:26:30.000000 torchtnt_nightly-2024.6.2/torchtnt_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-02 11:26:30.000000 torchtnt_nightly-2024.6.2/torchtnt_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 11:26:30.000000 torchtnt_nightly-2024.6.2/torchtnt_nightly.egg-info/zip-safe
```

### Comparing `torchtnt_nightly-2024.6.1/LICENSE` & `torchtnt_nightly-2024.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/PKG-INFO` & `torchtnt_nightly-2024.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchtnt-nightly
-Version: 2024.6.1
+Version: 2024.6.2
 Summary: A lightweight library for PyTorch training tools and utilities
 Home-page: https://github.com/pytorch/tnt
 Author: PyTorch
 Author-email: daniellepintz@fb.com
 License: BSD-3
 Keywords: pytorch,torch,training,tools,utilities
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2024.6.1 Summary: A
+Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2024.6.2 Summary: A
 lightweight library for PyTorch training tools and utilities Home-page: https:/
 /github.com/pytorch/tnt Author: PyTorch Author-email: daniellepintz@fb.com
 License: BSD-3 Keywords: pytorch,torch,training,tools,utilities Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Topic ::
```

### Comparing `torchtnt_nightly-2024.6.1/README.md` & `torchtnt_nightly-2024.6.2/README.md`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/setup.py` & `torchtnt_nightly-2024.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/framework/__init__.py` & `torchtnt_nightly-2024.6.2/torchtnt/framework/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/framework/_callback_handler.py` & `torchtnt_nightly-2024.6.2/torchtnt/framework/_callback_handler.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/framework/_loop_utils.py` & `torchtnt_nightly-2024.6.2/torchtnt/framework/_loop_utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/framework/_test_utils.py` & `torchtnt_nightly-2024.6.2/torchtnt/framework/_test_utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/framework/_unit_utils.py` & `torchtnt_nightly-2024.6.2/torchtnt/framework/_unit_utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/framework/auto_unit.py` & `torchtnt_nightly-2024.6.2/torchtnt/framework/auto_unit.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/framework/callback.py` & `torchtnt_nightly-2024.6.2/torchtnt/framework/callback.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/__init__.py` & `torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/_checkpoint_utils.py` & `torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/_checkpoint_utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/base_checkpointer.py` & `torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/base_checkpointer.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/base_csv_writer.py` & `torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/base_csv_writer.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/checkpointer_types.py` & `torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/checkpointer_types.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/dcp_saver.py` & `torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/dcp_saver.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/early_stopping.py` & `torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/early_stopping.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/empty_cuda_cache.py` & `torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/empty_cuda_cache.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/garbage_collector.py` & `torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/garbage_collector.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/iteration_time_logger.py` & `torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/iteration_time_logger.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/lambda_callback.py` & `torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/lambda_callback.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/learning_rate_monitor.py` & `torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/learning_rate_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/memory_snapshot.py` & `torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/memory_snapshot.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/module_summary.py` & `torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/module_summary.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/progress_reporter.py` & `torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/progress_reporter.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/pytorch_profiler.py` & `torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/pytorch_profiler.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/slow_rank_detector.py` & `torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/slow_rank_detector.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/system_resources_monitor.py` & `torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/system_resources_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py` & `torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/throughput_logger.py` & `torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/throughput_logger.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/time_limit_interrupter.py` & `torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/time_limit_interrupter.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/time_wait_for_batch_logger.py` & `torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/time_wait_for_batch_logger.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/torch_compile.py` & `torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/torch_compile.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/torchsnapshot_saver.py` & `torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/torchsnapshot_saver.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/tqdm_progress_bar.py` & `torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/tqdm_progress_bar.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/framework/callbacks/train_progress_monitor.py` & `torchtnt_nightly-2024.6.2/torchtnt/framework/callbacks/train_progress_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/framework/evaluate.py` & `torchtnt_nightly-2024.6.2/torchtnt/framework/evaluate.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/framework/fit.py` & `torchtnt_nightly-2024.6.2/torchtnt/framework/fit.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/framework/predict.py` & `torchtnt_nightly-2024.6.2/torchtnt/framework/predict.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/framework/state.py` & `torchtnt_nightly-2024.6.2/torchtnt/framework/state.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/framework/train.py` & `torchtnt_nightly-2024.6.2/torchtnt/framework/train.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/framework/unit.py` & `torchtnt_nightly-2024.6.2/torchtnt/framework/unit.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/framework/utils.py` & `torchtnt_nightly-2024.6.2/torchtnt/framework/utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/__init__.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/checkpoint.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/data/__init__.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/data/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/data/data_prefetcher.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/data/data_prefetcher.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/data/iterators.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/data/iterators.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/data/multi_dataloader.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/data/multi_dataloader.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/data/profile_dataloader.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/data/profile_dataloader.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/data/synthetic_data.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/data/synthetic_data.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/device.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/device.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/distributed.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/early_stop_checker.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/early_stop_checker.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/env.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/env.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/flops.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/flops.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/fsdp_utils.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/fsdp_utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/fsspec.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/fsspec.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/loggers/__init__.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/loggers/csv.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/loggers/csv.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/loggers/file.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/loggers/file.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/loggers/in_memory.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/loggers/in_memory.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/loggers/json.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/loggers/json.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/loggers/logger.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/loggers/stdout.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/loggers/tensorboard.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/loggers/utils.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/loggers/utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/lr_scheduler.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/memory.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/memory.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/memory_snapshot_profiler.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/memory_snapshot_profiler.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/misc.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/misc.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/module_summary.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/module_summary.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/oom.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/oom.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/optimizer.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/optimizer.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/precision.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/precision.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/prepare_module.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/prepare_module.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/progress.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/progress.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/rank_zero_log.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/rank_zero_log.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/stateful.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/stateful.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/swa.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/swa.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/test_utils.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/timer.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/timer.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/tqdm.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/tqdm.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt/utils/version.py` & `torchtnt_nightly-2024.6.2/torchtnt/utils/version.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.6.1/torchtnt_nightly.egg-info/PKG-INFO` & `torchtnt_nightly-2024.6.2/torchtnt_nightly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchtnt-nightly
-Version: 2024.6.1
+Version: 2024.6.2
 Summary: A lightweight library for PyTorch training tools and utilities
 Home-page: https://github.com/pytorch/tnt
 Author: PyTorch
 Author-email: daniellepintz@fb.com
 License: BSD-3
 Keywords: pytorch,torch,training,tools,utilities
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2024.6.1 Summary: A
+Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2024.6.2 Summary: A
 lightweight library for PyTorch training tools and utilities Home-page: https:/
 /github.com/pytorch/tnt Author: PyTorch Author-email: daniellepintz@fb.com
 License: BSD-3 Keywords: pytorch,torch,training,tools,utilities Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Topic ::
```

### Comparing `torchtnt_nightly-2024.6.1/torchtnt_nightly.egg-info/SOURCES.txt` & `torchtnt_nightly-2024.6.2/torchtnt_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

