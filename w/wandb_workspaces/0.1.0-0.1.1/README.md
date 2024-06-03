# Comparing `tmp/wandb_workspaces-0.1.0.tar.gz` & `tmp/wandb_workspaces-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wandb_workspaces-0.1.0.tar", max compression
+gzip compressed data, was "wandb_workspaces-0.1.1.tar", max compression
```

## Comparing `wandb_workspaces-0.1.0.tar` & `wandb_workspaces-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,37 @@
--rw-r--r--   0        0        0        0 2024-05-28 01:13:17.197701 wandb_workspaces-0.1.0/README.md
--rw-r--r--   0        0        0      283 2024-05-28 01:13:17.199082 wandb_workspaces-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-28 01:13:17.197654 wandb_workspaces-0.1.0/wandb_workspaces/__init__.py
--rw-r--r--   0        0        0      353 1970-01-01 00:00:00.000000 wandb_workspaces-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    10940 2024-06-02 02:32:37.083609 wandb_workspaces-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2331 2024-06-02 17:01:16.507346 wandb_workspaces-0.1.1/README.md
+-rw-r--r--   0        0        0     2710 2024-06-03 03:05:40.385277 wandb_workspaces-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       53 2024-06-01 12:29:32.391349 wandb_workspaces-0.1.1/wandb_workspaces/__init__.py
+-rw-r--r--   0        0        0     7747 2024-06-03 01:25:20.237045 wandb_workspaces-0.1.1/wandb_workspaces/expr.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:47:35.015419 wandb_workspaces-0.1.1/wandb_workspaces/reports/__init__.py
+-rw-r--r--   0        0        0      870 2024-02-05 03:20:39.009128 wandb_workspaces-0.1.1/wandb_workspaces/reports/v1/__init__.py
+-rw-r--r--   0        0        0    53756 2024-06-01 17:29:14.376358 wandb_workspaces-0.1.1/wandb_workspaces/reports/v1/_blocks.py
+-rw-r--r--   0        0        0     2136 2024-05-30 22:55:22.787427 wandb_workspaces-0.1.1/wandb_workspaces/reports/v1/_helpers.py
+-rw-r--r--   0        0        0    48383 2024-02-05 03:20:39.009474 wandb_workspaces-0.1.1/wandb_workspaces/reports/v1/_panels.py
+-rw-r--r--   0        0        0    18139 2024-05-24 12:38:19.597221 wandb_workspaces-0.1.1/wandb_workspaces/reports/v1/_templates.py
+-rw-r--r--   0        0        0      430 2024-02-05 03:20:39.009665 wandb_workspaces-0.1.1/wandb_workspaces/reports/v1/blocks.py
+-rw-r--r--   0        0        0       55 2024-02-05 03:20:39.009725 wandb_workspaces-0.1.1/wandb_workspaces/reports/v1/helpers.py
+-rw-r--r--   0        0        0     1291 2024-02-05 03:20:39.009789 wandb_workspaces-0.1.1/wandb_workspaces/reports/v1/mutations.py
+-rw-r--r--   0        0        0      337 2024-02-05 03:20:39.009853 wandb_workspaces-0.1.1/wandb_workspaces/reports/v1/panels.py
+-rw-r--r--   0        0        0     9375 2024-06-01 17:29:14.377632 wandb_workspaces-0.1.1/wandb_workspaces/reports/v1/report.py
+-rw-r--r--   0        0        0     4983 2024-05-30 22:55:22.145696 wandb_workspaces-0.1.1/wandb_workspaces/reports/v1/runset.py
+-rw-r--r--   0        0        0      161 2024-02-05 03:20:39.010216 wandb_workspaces-0.1.1/wandb_workspaces/reports/v1/templates.py
+-rw-r--r--   0        0        0    11950 2024-05-30 22:55:22.145413 wandb_workspaces-0.1.1/wandb_workspaces/reports/v1/util.py
+-rw-r--r--   0        0        0     4282 2024-02-05 03:20:39.010523 wandb_workspaces-0.1.1/wandb_workspaces/reports/v1/validators.py
+-rw-r--r--   0        0        0      384 2024-05-30 22:54:11.910046 wandb_workspaces-0.1.1/wandb_workspaces/reports/v2/__init__.py
+-rw-r--r--   0        0        0      382 2024-03-02 19:33:31.486920 wandb_workspaces-0.1.1/wandb_workspaces/reports/v2/blocks.py
+-rw-r--r--   0        0        0     8246 2024-05-29 11:41:39.111320 wandb_workspaces-0.1.1/wandb_workspaces/reports/v2/expr_parsing.py
+-rw-r--r--   0        0        0     1329 2024-05-14 19:20:57.137842 wandb_workspaces-0.1.1/wandb_workspaces/reports/v2/gql.py
+-rw-r--r--   0        0        0    57726 2024-06-01 17:29:14.378090 wandb_workspaces-0.1.1/wandb_workspaces/reports/v2/interface.py
+-rw-r--r--   0        0        0    27528 2024-06-03 02:09:27.847208 wandb_workspaces-0.1.1/wandb_workspaces/reports/v2/internal.py
+-rw-r--r--   0        0        0       85 2024-02-05 03:20:39.011674 wandb_workspaces-0.1.1/wandb_workspaces/reports/v2/metrics.py
+-rw-r--r--   0        0        0      266 2024-05-24 12:38:19.598024 wandb_workspaces-0.1.1/wandb_workspaces/reports/v2/panels.py
+-rw-r--r--   0        0        0        0 2024-06-01 12:30:01.819294 wandb_workspaces-0.1.1/wandb_workspaces/utils/__init__.py
+-rw-r--r--   0        0        0     2540 2024-06-03 00:23:00.552103 wandb_workspaces-0.1.1/wandb_workspaces/utils/data_generation.py
+-rw-r--r--   0        0        0     1284 2024-06-01 12:28:09.544631 wandb_workspaces-0.1.1/wandb_workspaces/utils/invertable_dict.py
+-rw-r--r--   0        0        0     1806 2024-06-03 02:17:43.085661 wandb_workspaces-0.1.1/wandb_workspaces/utils/validators.py
+-rw-r--r--   0        0        0       87 2024-06-01 02:25:22.012048 wandb_workspaces-0.1.1/wandb_workspaces/workspaces/__init__.py
+-rw-r--r--   0        0        0       84 2024-06-03 02:16:10.072891 wandb_workspaces-0.1.1/wandb_workspaces/workspaces/errors.py
+-rw-r--r--   0        0        0    20505 2024-06-03 02:18:32.343536 wandb_workspaces-0.1.1/wandb_workspaces/workspaces/interface.py
+-rw-r--r--   0        0        0     6939 2024-06-03 02:17:53.109563 wandb_workspaces-0.1.1/wandb_workspaces/workspaces/internal.py
+-rw-r--r--   0        0        0     3713 1970-01-01 00:00:00.000000 wandb_workspaces-0.1.1/PKG-INFO
```

