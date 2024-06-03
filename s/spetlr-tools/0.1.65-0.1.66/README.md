# Comparing `tmp/spetlr-tools-0.1.65.tar.gz` & `tmp/spetlr-tools-0.1.66.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spetlr-tools-0.1.65.tar", last modified: Mon Feb 19 19:44:13 2024, max compression
+gzip compressed data, was "spetlr-tools-0.1.66.tar", last modified: Mon Jun  3 13:18:09 2024, max compression
```

## Comparing `spetlr-tools-0.1.65.tar` & `spetlr-tools-0.1.66.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 19:44:13.193387 spetlr-tools-0.1.65/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-02-19 19:44:13.193387 spetlr-tools-0.1.65/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-02-19 19:44:13.193387 spetlr-tools-0.1.65/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 19:44:13.185387 spetlr-tools-0.1.65/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 19:44:13.185387 spetlr-tools-0.1.65/src/spetlr_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-02-19 19:44:13.000000 spetlr-tools-0.1.65/src/spetlr_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-02-19 19:44:13.000000 spetlr-tools-0.1.65/src/spetlr_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 19:44:13.000000 spetlr-tools-0.1.65/src/spetlr_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-02-19 19:44:13.000000 spetlr-tools-0.1.65/src/spetlr_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 19:44:13.000000 spetlr-tools-0.1.65/src/spetlr_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-19 19:44:13.000000 spetlr-tools-0.1.65/src/spetlr_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-19 19:44:13.000000 spetlr-tools-0.1.65/src/spetlr_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 19:44:13.185387 spetlr-tools-0.1.65/src/spetlrtools/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 19:44:13.189387 spetlr-tools-0.1.65/src/spetlrtools/az_databricks_token/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/az_databricks_token/AuthLinkOpener.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/az_databricks_token/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/az_databricks_token/get_ad_access_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/az_databricks_token/get_impersonation_authorization_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/az_databricks_token/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/az_databricks_token/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 19:44:13.189387 spetlr-tools-0.1.65/src/spetlrtools/cli_install/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/cli_install/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/cli_install/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/cli_install/install.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/cli_install/latest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/cli_install/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/cli_install/uninstall.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 19:44:13.189387 spetlr-tools-0.1.65/src/spetlrtools/diagrams/
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/diagrams/DiagramMarkupLibraryParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/diagrams/DrawioDiagramParser.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/diagrams/Edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/diagrams/HTMLStripper.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/diagrams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/diagrams/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 19:44:13.189387 spetlr-tools-0.1.65/src/spetlrtools/entry_points/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/entry_points/task_entry_point_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 19:44:13.189387 spetlr-tools-0.1.65/src/spetlrtools/format/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/format/validate_camelcased_cols.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 19:44:13.189387 spetlr-tools-0.1.65/src/spetlrtools/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/helpers/ExtractEncodedBody.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/helpers/get_difference_between_two_dfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/helpers/module_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/manipulate_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/requirements.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 19:44:13.193387 spetlr-tools-0.1.65/src/spetlrtools/test_job/
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/test_job/RunDetails.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/test_job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/test_job/dbcli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/test_job/dbfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/test_job/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/test_job/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    17562 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/test_job/submit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/test_job/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 19:44:13.193387 spetlr-tools-0.1.65/src/spetlrtools/testing/
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/testing/DataframeTestCase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/testing/TestHandle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/testing/TupleComparer.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 19:44:13.193387 spetlr-tools-0.1.65/src/spetlrtools/time/
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/time/TimeSequence.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-02-19 19:44:04.000000 spetlr-tools-0.1.65/src/spetlrtools/time/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:18:08.995766 spetlr-tools-0.1.66/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-06-03 13:18:08.995766 spetlr-tools-0.1.66/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-06-03 13:18:08.995766 spetlr-tools-0.1.66/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:18:08.983766 spetlr-tools-0.1.66/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:18:08.987766 spetlr-tools-0.1.66/src/spetlr_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-06-03 13:18:08.000000 spetlr-tools-0.1.66/src/spetlr_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-06-03 13:18:08.000000 spetlr-tools-0.1.66/src/spetlr_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 13:18:08.000000 spetlr-tools-0.1.66/src/spetlr_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-06-03 13:18:08.000000 spetlr-tools-0.1.66/src/spetlr_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 13:18:08.000000 spetlr-tools-0.1.66/src/spetlr_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-06-03 13:18:08.000000 spetlr-tools-0.1.66/src/spetlr_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-06-03 13:18:08.000000 spetlr-tools-0.1.66/src/spetlr_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:18:08.987766 spetlr-tools-0.1.66/src/spetlrtools/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:18:08.987766 spetlr-tools-0.1.66/src/spetlrtools/az_databricks_token/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/az_databricks_token/AuthLinkOpener.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/az_databricks_token/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/az_databricks_token/get_ad_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/az_databricks_token/get_impersonation_authorization_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/az_databricks_token/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/az_databricks_token/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:18:08.991766 spetlr-tools-0.1.66/src/spetlrtools/cli_install/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/cli_install/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/cli_install/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/cli_install/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/cli_install/latest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/cli_install/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/cli_install/uninstall.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:18:08.991766 spetlr-tools-0.1.66/src/spetlrtools/diagrams/
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/diagrams/DiagramMarkupLibraryParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/diagrams/DrawioDiagramParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/diagrams/Edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/diagrams/HTMLStripper.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/diagrams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/diagrams/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:18:08.991766 spetlr-tools-0.1.66/src/spetlrtools/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/entry_points/task_entry_point_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:18:08.991766 spetlr-tools-0.1.66/src/spetlrtools/format/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/format/validate_camelcased_cols.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:18:08.991766 spetlr-tools-0.1.66/src/spetlrtools/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/helpers/ExtractEncodedBody.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/helpers/get_difference_between_two_dfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/helpers/module_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/manipulate_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:18:08.995766 spetlr-tools-0.1.66/src/spetlrtools/test_job/
+-rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/test_job/RemoteLocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/test_job/RunDetails.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/test_job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/test_job/dbcli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/test_job/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/test_job/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16986 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/test_job/submit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/test_job/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:18:08.995766 spetlr-tools-0.1.66/src/spetlrtools/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/testing/DataframeTestCase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/testing/TestHandle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/testing/TupleComparer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:18:08.995766 spetlr-tools-0.1.66/src/spetlrtools/time/
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/time/TimeSequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-06-03 13:17:49.000000 spetlr-tools-0.1.66/src/spetlrtools/time/__init__.py
```

### Comparing `spetlr-tools-0.1.65/LICENSE` & `spetlr-tools-0.1.66/LICENSE`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.65/PKG-INFO` & `spetlr-tools-0.1.66/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spetlr-tools
-Version: 0.1.65
+Version: 0.1.66
 Summary: Supplements to the python SPark ETL libRary (SPETLR) for Databricks.
 Home-page: https://github.com/spetlr-org/spetlr-tools
 Author: Spetlr.Org
 Author-email: spetlr.org@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/spetlr-org/spetlr-tools
 Project-URL: Bug Reports, https://github.com/spetlr-org/spetlr-tools/issues
```

### Comparing `spetlr-tools-0.1.65/README.md` & `spetlr-tools-0.1.66/README.md`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.65/setup.cfg` & `spetlr-tools-0.1.66/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 	spetlr
 	pyyaml
 	importlib_metadata
 	dateparser
 	pytest
 	packaging
 	requests
+	databricks-sdk
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 dev = 
 	check-manifest
@@ -49,18 +50,18 @@
 [options.package_data]
 * = *.json, *.sql, *.yaml
 
 [options.entry_points]
 console_scripts = 
 	spetlr-freeze-req = spetlrtools.requirements:main
 	spetlr-az-databricks-token = spetlrtools.az_databricks_token.main:main
-	spetlr-test-job = spetlrtools.test_job.main:main
 	spetlr-manipulate-version = spetlrtools.manipulate_version:main
 	spetlr-check-diagram = spetlrtools.diagrams.main:main
 	spetlr-databricks-cli = spetlrtools.cli_install.main:main
+	spetlr-test-job = spetlrtools.test_job.main:main
 
 [flake8]
 exclude = .git,__pycache__,docs,build,dist,venv
 ignore = E501, W503
 max-line-length = 88
 extend-ignore = E203
```

### Comparing `spetlr-tools-0.1.65/src/spetlr_tools.egg-info/PKG-INFO` & `spetlr-tools-0.1.66/src/spetlr_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spetlr-tools
-Version: 0.1.65
+Version: 0.1.66
 Summary: Supplements to the python SPark ETL libRary (SPETLR) for Databricks.
 Home-page: https://github.com/spetlr-org/spetlr-tools
 Author: Spetlr.Org
 Author-email: spetlr.org@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/spetlr-org/spetlr-tools
 Project-URL: Bug Reports, https://github.com/spetlr-org/spetlr-tools/issues
```

### Comparing `spetlr-tools-0.1.65/src/spetlr_tools.egg-info/SOURCES.txt` & `spetlr-tools-0.1.66/src/spetlr_tools.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -35,18 +35,18 @@
 src/spetlrtools/entry_points/task_entry_point_helper.py
 src/spetlrtools/format/__init__.py
 src/spetlrtools/format/validate_camelcased_cols.py
 src/spetlrtools/helpers/ExtractEncodedBody.py
 src/spetlrtools/helpers/__init__.py
 src/spetlrtools/helpers/get_difference_between_two_dfs.py
 src/spetlrtools/helpers/module_helper.py
+src/spetlrtools/test_job/RemoteLocation.py
 src/spetlrtools/test_job/RunDetails.py
 src/spetlrtools/test_job/__init__.py
 src/spetlrtools/test_job/dbcli.py
-src/spetlrtools/test_job/dbfs.py
 src/spetlrtools/test_job/fetch.py
 src/spetlrtools/test_job/main.py
 src/spetlrtools/test_job/submit.py
 src/spetlrtools/test_job/test_main.py
 src/spetlrtools/testing/DataframeTestCase.py
 src/spetlrtools/testing/TestHandle.py
 src/spetlrtools/testing/TupleComparer.py
```

### Comparing `spetlr-tools-0.1.65/src/spetlrtools/az_databricks_token/AuthLinkOpener.py` & `spetlr-tools-0.1.66/src/spetlrtools/az_databricks_token/AuthLinkOpener.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.65/src/spetlrtools/az_databricks_token/__init__.py` & `spetlr-tools-0.1.66/src/spetlrtools/az_databricks_token/__init__.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.65/src/spetlrtools/az_databricks_token/get_ad_access_token.py` & `spetlr-tools-0.1.66/src/spetlrtools/az_databricks_token/get_ad_access_token.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.65/src/spetlrtools/az_databricks_token/get_impersonation_authorization_code.py` & `spetlr-tools-0.1.66/src/spetlrtools/az_databricks_token/get_impersonation_authorization_code.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.65/src/spetlrtools/az_databricks_token/main.py` & `spetlr-tools-0.1.66/src/spetlrtools/az_databricks_token/main.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.65/src/spetlrtools/az_databricks_token/server.py` & `spetlr-tools-0.1.66/src/spetlrtools/az_databricks_token/server.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.65/src/spetlrtools/cli_install/defaults.py` & `spetlr-tools-0.1.66/src/spetlrtools/cli_install/defaults.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.65/src/spetlrtools/cli_install/install.py` & `spetlr-tools-0.1.66/src/spetlrtools/cli_install/install.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.65/src/spetlrtools/cli_install/latest.py` & `spetlr-tools-0.1.66/src/spetlrtools/cli_install/latest.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.65/src/spetlrtools/cli_install/main.py` & `spetlr-tools-0.1.66/src/spetlrtools/cli_install/main.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.65/src/spetlrtools/cli_install/uninstall.py` & `spetlr-tools-0.1.66/src/spetlrtools/cli_install/uninstall.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.65/src/spetlrtools/diagrams/DiagramMarkupLibraryParser.py` & `spetlr-tools-0.1.66/src/spetlrtools/diagrams/DiagramMarkupLibraryParser.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.65/src/spetlrtools/diagrams/DrawioDiagramParser.py` & `spetlr-tools-0.1.66/src/spetlrtools/diagrams/DrawioDiagramParser.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.65/src/spetlrtools/diagrams/Edge.py` & `spetlr-tools-0.1.66/src/spetlrtools/diagrams/Edge.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.65/src/spetlrtools/diagrams/HTMLStripper.py` & `spetlr-tools-0.1.66/src/spetlrtools/diagrams/HTMLStripper.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.65/src/spetlrtools/diagrams/main.py` & `spetlr-tools-0.1.66/src/spetlrtools/diagrams/main.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.65/src/spetlrtools/entry_points/task_entry_point_helper.py` & `spetlr-tools-0.1.66/src/spetlrtools/entry_points/task_entry_point_helper.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.65/src/spetlrtools/format/validate_camelcased_cols.py` & `spetlr-tools-0.1.66/src/spetlrtools/format/validate_camelcased_cols.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.65/src/spetlrtools/helpers/ExtractEncodedBody.py` & `spetlr-tools-0.1.66/src/spetlrtools/helpers/ExtractEncodedBody.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.65/src/spetlrtools/helpers/get_difference_between_two_dfs.py` & `spetlr-tools-0.1.66/src/spetlrtools/helpers/get_difference_between_two_dfs.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.65/src/spetlrtools/helpers/module_helper.py` & `spetlr-tools-0.1.66/src/spetlrtools/helpers/module_helper.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.65/src/spetlrtools/manipulate_version.py` & `spetlr-tools-0.1.66/src/spetlrtools/manipulate_version.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.65/src/spetlrtools/requirements.py` & `spetlr-tools-0.1.66/src/spetlrtools/requirements.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.65/src/spetlrtools/test_job/fetch.py` & `spetlr-tools-0.1.66/src/spetlrtools/test_job/fetch.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 import json
 import sys
 import time
 from collections import defaultdict
 from dataclasses import dataclass
 from typing import IO, List, Optional
 
-from spetlrtools.test_job.dbcli import dbcli
+from databricks.sdk.service import jobs
+
 from spetlrtools.test_job.RunDetails import RunDetails
 
 
 def setup_fetch_parser(subparsers):
     """
     Adds a subparser for the command 'fetch'.
     :param subparsers: must be the object returned by ArgumentParser().add_subparsers()
@@ -69,25 +70,78 @@
 
 def fetch_main(args):
     """
     Main function of the 'fetch' command. Only to be used via the cli.
     :param args: the parsed arguments from the fetch subparser
     :return:
     """
-    dbcli.check_connection()
 
     # Post process the arguments
     if args.runid is None:
         args.runid = json.load(args.runid_json)["run_id"]
 
     if fetch(args.runid, args.stdout, args.failfast):
         print("Run failed")
         sys.exit(-1)
 
 
+def fetch(run_id: int, stdout_file: IO[str] = None, failfast=False):
+    """Fetch main function.
+    See the cli help for parameter descriptions and functionality.
+    Can be used programmatically."""
+
+    run = RunDetails(run_id)
+
+    last_state = None
+    stdouts = {}
+    while True:
+        state = MultiTaskState.fromRun(run.details)
+        # state = MultiTaskState.fromJson(run.details.as_dict())
+        if last_state is None or state != last_state:
+            last_state = state
+            state.print_status()
+
+        if failfast:
+            if any(task.ended and not task.success for task in state.tasks):
+                break
+
+        for task in state.tasks:
+            if task.ended and task.task_key not in stdouts:
+                out = run.get_stdout(task.task_key)
+                if stdout_file is None:
+                    print(out)
+                stdouts[task.task_key] = out
+
+        if state.overall.ended:
+            break
+        time.sleep(5)
+        run.refresh()
+
+    if stdout_file is not None:
+        for k, v in stdouts.items():
+            stdout_file.write("=" * 50 + f"\nTask Output from {k}\n" + "=" * 50 + "\n")
+            stdout_file.write(v)
+
+    if last_state.overall.success:
+        print("Run result SUCCESS!")
+        return 0
+    else:
+        if not (last_state.overall.ended):
+            print("A task failed. Cancelling test run.")
+            run.cancel()
+        return 1
+
+
+def enumNameOrNone(obj):
+    if obj is None:
+        return ""
+    else:
+        return obj.name
+
+
 @dataclass
 class TaskState:
     """The result state of any workflow or task"""
 
     task_key: str
     life_cycle_state: str
     result_state: str
@@ -108,41 +162,53 @@
 
     @property
     def success(self):
         """Has the workflow or task succeeded?"""
         return self.result_state.upper() == "SUCCESS"
 
     @classmethod
-    def fromJson(cls, jobj):
+    def fromTask(cls, task: jobs.RunTask):
+        """Create the result state of the workflow or task from the json object
+        returned by the databricks api."""
+
+        return cls(
+            task_key=task.task_key,
+            life_cycle_state=enumNameOrNone(task.state.life_cycle_state),
+            result_state=enumNameOrNone(task.state.result_state),
+            end_time=task.end_time,
+        )
+
+    @classmethod
+    def fromRun(cls, run: jobs.Run):
         """Create the result state of the workflow or task from the json object
         returned by the databricks api."""
-        state = jobj["state"]
+
         return cls(
-            task_key=jobj["task_key"] if "task_key" in jobj else jobj["run_name"],
-            life_cycle_state=state["life_cycle_state"],
-            result_state=state["result_state"] if "result_state" in state else "",
-            end_time=jobj["end_time"] if "end_time" in jobj else 0,
+            task_key=run.run_name,
+            life_cycle_state=enumNameOrNone(run.state.life_cycle_state),
+            result_state=enumNameOrNone(run.state.result_state),
+            end_time=run.end_time,
         )
 
 
 @dataclass
 class MultiTaskState:
     """Result state of a multiTask workflow"""
 
     overall: Optional[TaskState]
     tasks: List[TaskState]
 
     @classmethod
-    def fromJson(cls, jobj):
+    def fromRun(cls, run: jobs.Run):
         """Create the Result state of a multiTask workflow from the json object returned
         by the databricks api."""
 
         return cls(
-            overall=TaskState.fromJson(jobj),
-            tasks=[TaskState.fromJson(task) for task in jobj["tasks"]],
+            overall=TaskState.fromRun(run),
+            tasks=[TaskState.fromTask(task) for task in run.tasks],
         )
 
     def accumulate(self):
         """return a dictionary of {'STATE STRING':counts} where counts represents the
         number of sub-tasks that share the same run state."""
         counts = defaultdict(int)
         for task in self.tasks:
@@ -153,51 +219,7 @@
         """Print the overall result state represented by this object."""
         print(
             "Overall state:",
             self.overall.result,
             "| Task states:",
             " | ".join(f"{k}: {v}" for k, v in self.accumulate().items()),
         )
-
-
-def fetch(run_id: int, stdout_file: IO[str] = None, failfast=False):
-    """Fetch main function.
-    See the cli help for parameter descriptions and functionality.
-    Can be used programmatically."""
-    run = RunDetails(run_id)
-    last_state = None
-    stdouts = {}
-    while True:
-        state = MultiTaskState.fromJson(run.details)
-        if last_state is None or state != last_state:
-            last_state = state
-            state.print_status()
-
-        if failfast:
-            if any(task.ended and not task.success for task in state.tasks):
-                break
-
-        for task in state.tasks:
-            if task.ended and task.task_key not in stdouts:
-                out = run.get_stdout(task.task_key)
-                if stdout_file is None:
-                    print(out)
-                stdouts[task.task_key] = out
-
-        if state.overall.ended:
-            break
-        time.sleep(5)
-        run.refresh()
-
-    if stdout_file is not None:
-        for k, v in stdouts.items():
-            stdout_file.write("=" * 50 + f"\nTask Output from {k}\n" + "=" * 50 + "\n")
-            stdout_file.write(v)
-
-    if last_state.overall.success:
-        print("Run result SUCCESS!")
-        return 0
-    else:
-        if not (last_state.overall.ended):
-            print("A task failed. Cancelling test run.")
-            run.cancel()
-        return 1
```

### Comparing `spetlr-tools-0.1.65/src/spetlrtools/test_job/submit.py` & `spetlr-tools-0.1.66/src/spetlrtools/test_job/submit.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 usage: spetlr-test-job submit [-h] [--dry-run] [--wheels WHEELS] --tests TESTS [--task TASK] [--tasks-from TASKS_FROM] (--cluster CLUSTER | --cluster-file CLUSTER_FILE)
                               [--sparklibs SPARKLIBS | --sparklibs-file SPARKLIBS_FILE] [--requirement REQUIREMENT | --requirements-file REQUIREMENTS_FILE] [--main-script MAIN_SCRIPT] [--pytest-args PYTEST_ARGS]
-                              [--out-json OUT_JSON] [--wait WAIT]
+                              [--out-json OUT_JSON] [--wait-for-job]
 
 Run Test Cases on databricks cluster.
 
 optional arguments:
   -h, --help            show this help message and exit
   --dry-run             Don't do anything, only report
   --wheels WHEELS       The glob paths of all wheels under test.
@@ -25,36 +25,48 @@
   --requirements-file REQUIREMENTS_FILE
                         File with python dependencies, specified like for pip
   --main-script MAIN_SCRIPT
                         Your own test_main.py script file, to add custom functionality.
   --pytest-args PYTEST_ARGS
                         Additional arguments to pass to pytest in each test job.
   --out-json OUT_JSON   File to store the RunID for future queries.
-  --wait WAIT           After upload, wait this many seconds for it to settle.
+  --upload-to {workspace,dbfs}
+                        Where to upload test job files.
+  --wait-for-job        After submission, wait for result using cli v2.
+
 
 """
 
 import argparse
-import copy
-import datetime
 import inspect
 import json
 import re
 import shutil
 import subprocess
 import tempfile
-import time
-import uuid
-from pathlib import Path
+from pathlib import Path, PosixPath
 from typing import Dict, List, Union
 from typing.io import IO
 
-from . import test_main
-from .dbcli import dbcli
-from .dbfs import DbfsLocation
+from spetlrtools.test_job import test_main
+from spetlrtools.test_job.dbcli import DbCli
+from spetlrtools.test_job.RemoteLocation import (
+    DbfsLocation,
+    RemoteLocation,
+    StageArea,
+    WorkspaceLocation,
+)
+
+
+# Custom action to handle the deprecation warning
+class DeprecatedAction(argparse.Action):
+    def __call__(self, parser, namespace, values, option_string=None):
+        print(
+            f"WARNING: {option_string} is deprecated and will be removed in future versions."
+        )
 
 
 def setup_submit_parser(subparsers):
     """
     Adds a subparser for the command 'submit'.
     :param subparsers: must be the object returned by ArgumentParser().add_subparsers()
     :return:
@@ -145,19 +157,26 @@
     parser.add_argument(
         "--out-json",
         type=argparse.FileType("w"),
         help="File to store the RunID for future queries.",
     )
 
     parser.add_argument(
-        "--wait",
-        type=int,
-        help="After upload, wait this many seconds for it to settle.",
-        default=60,
+        "--upload-to",
+        choices=["workspace", "dbfs"],
+        help="Where to upload test job files.",
+        default="dbfs",
+    )
+
+    parser.add_argument(
+        "--wait-for-job",
+        action="store_true",
+        help="After submission, wait for result using cli v2.",
     )
+    parser.add_argument("--wait", action=DeprecatedAction, help=argparse.SUPPRESS)
 
     return
 
 
 def collect_arguments(args):
     """
     Post process the parsed arguments of the 'submit' command argument parser.
@@ -187,15 +206,14 @@
     args.pytest_args = (args.pytest_args or "").split()
 
     return args
 
 
 def submit_main(args):
     """the main function of the cli command 'submit'. Not to be used directly."""
-    dbcli.check_connection()
 
     args = collect_arguments(args)
 
     submit(
         test_path=args.tests,
         cluster=args.cluster,
         wheels=args.wheels,
@@ -203,47 +221,23 @@
         tasks_from=args.tasks_from,
         requirement=args.requirement,
         sparklibs=args.sparklibs,
         out_json=args.out_json,
         main_script=args.main_script,
         pytest_args=args.pytest_args,
         dry_run=args.dry_run,
-        wait=args.wait,
+        upload_to=args.upload_to,
+        wait_for_job=args.wait_for_job,
     )
 
 
-class DbTestFolder:
-    """Context manager that creates a unique test folder on dbfs."""
-
-    def __init__(self):
-        self._test_path_base = DbfsLocation(
-            "/".join(
-                [
-                    "test",
-                    datetime.datetime.now(datetime.timezone.utc).strftime(
-                        "%Y%m%d-%H%M%S"
-                    ),
-                    uuid.uuid4().hex,
-                ]
-            )
-        )
-
-    def __enter__(self):
-        print(f"Making dbfs test folder {self._test_path_base.remote}")
-        dbcli.dbcall(f"fs mkdirs {self._test_path_base.remote}")
-        return self._test_path_base
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        pass
-
+def verify_and_resolve_task(test_path: str, task: Union[str, PosixPath]):
+    test_archive = PosixPath(test_path).resolve().absolute()
 
-def verify_and_resolve_task(test_path: str, task: Union[str, Path]):
-    test_archive = Path(test_path).resolve().absolute()
-
-    task_path = Path(task)
+    task_path = PosixPath(task)
     if not task_path.is_absolute():
         task_path = (test_archive.parent / task_path).resolve().absolute()
 
     task_path = task_path.resolve().absolute()
 
     if not (test_archive == task_path or test_archive in task_path.parents):
         raise AssertionError(f"task {task} is not contained in {test_path}")
@@ -259,15 +253,15 @@
 
 def discover_job_tasks(test_path: str, folder: str):
     """If folder is given, create parallel tasks from this level.
     Otherwise, simply return the top folder as the single task.
     Returns a list of strings with the subfolders to process.
     """
 
-    test_archive_parent = Path(test_path).resolve().absolute().parent
+    test_archive_parent = PosixPath(test_path).resolve().absolute().parent
 
     subfolders = [
         verify_and_resolve_task(test_path, x)
         for x in (test_archive_parent / folder).iterdir()
         if (x.is_dir() and not x.stem.startswith("_"))
     ]
     return subfolders
@@ -288,16 +282,16 @@
             # if this throws a KeyError, we are right to abort execution since the input is invalid.
         else:
             # No Marker = no lookup
             return pool_id
 
     def get_instance_pools(self) -> Dict[str, str]:
         pool_lookup = {
-            pool["instance_pool_name"]: pool["instance_pool_id"]
-            for pool in dbcli.list_instance_pools()
+            pool.instance_pool_name: pool.instance_pool_id
+            for pool in DbCli().list_instance_pools()
         }
         return pool_lookup
 
 
 def submit(
     test_path: str,
     cluster: dict,
@@ -306,15 +300,16 @@
     tasks_from: List[str] = None,
     requirement: List[str] = None,
     sparklibs: List[dict] = None,
     out_json: IO[str] = None,
     main_script: IO[str] = None,
     pytest_args: List[str] = None,
     dry_run=False,
-    wait=60,
+    upload_to="dbfs",
+    wait_for_job=False,
 ):
     """
     --dry-run             Don't do anything, only report
     --wheels WHEELS       The glob paths of all wheels under test.
     --tests TESTS         Location of the tests folder. Will be sent to databricks as a whole.
     --task TASK           Single Test file or folder to execute.
     --tasks-from TASKS_FROM
@@ -331,184 +326,165 @@
     --requirements-file REQUIREMENTS_FILE
                           File with python dependencies, specified like for pip
     --main-script MAIN_SCRIPT
                           Your own test_main.py script file, to add custom functionality.
     --pytest-args PYTEST_ARGS
                           Additional arguments to pass to pytest in each test job.
     --out-json OUT_JSON   File to store the RunID for future queries.
-    --wait WAIT           After upload, wait this many seconds for it to settle.
+    --upload-to {workspace,dbfs}
+                          Where to upload test job files.
+    --wait-for-job        After submission, wait for result using cli v2.
     """
     if requirement is None:
         requirement = []
     if sparklibs is None:
         sparklibs = []
     if pytest_args is None:
         pytest_args = []
     if tasks is None:
         tasks = []
     if tasks_from is None:
         tasks_from = []
     if not (tasks or tasks_from):
         raise ValueError("No tasks given")
+    upload_to = upload_to.lower()
 
     # check the structure of the cluster object
     if not isinstance(cluster, dict):
         raise AssertionError("invalid cluster specification")
 
     # check the structure of the sparklibs object
     if not isinstance(sparklibs, list):
         raise AssertionError("invalid sparklibs specification")
 
     for py_requirement in requirement:
         sparklibs.append({"pypi": {"package": py_requirement}})
 
-    pools = PoolBoy()
-
-    with DbTestFolder() as test_folder:
-        for wheel in discover_and_push_wheels(wheels, test_folder):
-            sparklibs.append({"whl": wheel})
+    dbcli = DbCli()
 
-        archive_local = archive_and_push(test_path, test_folder, dry_run=dry_run)
-        main_file = push_main_file(test_folder, main_script, dry_run=dry_run)
-
-        print(f"copied everything to {test_folder.remote}")
+    # create everything in a temporary directory.
+    # for dry-runs, keep make it a local directory and keep it
+    with StageArea(dry_run) as stage:
+        if upload_to == "workspace":
+            remote: RemoteLocation = WorkspaceLocation(stage)
+        elif upload_to == "dbfs":
+            remote: RemoteLocation = DbfsLocation(stage)
+        else:
+            raise ValueError("unsupported upload")
 
-        if not dry_run:
-            print(f"Wait {wait}s for uploading test folder...")
-            time.sleep(wait)
-            print(f"Waited {wait}s successfully!")
+        wheels = discover_wheels(wheels, remote)
+        for wheel in wheels:
+            sparklibs.append({"whl": wheel})
 
-        # construct the workflow object
-        workflow = dict(run_name="Testing Run", format="MULTI_TASK", tasks=[])
+        prepare_archive(test_path, remote)
+        main_file = prepare_main_file(remote, main_script)
 
         resolved_tasks = [verify_and_resolve_task(test_path, task) for task in tasks]
         for task in tasks_from:
             # subtasks will be ['tests/cluster/job1', 'tests/cluster/job2'] or similar
             resolved_tasks += discover_job_tasks(test_path, task)
 
         if dry_run:
             print(resolved_tasks)
 
+        if "instance_pool_id" in cluster:
+            cluster["instance_pool_id"] = PoolBoy().lookup(cluster["instance_pool_id"])
+
+        # construct the workflow object
+        workflow = dict(run_name="Testing Run", format="MULTI_TASK", tasks=[])
+
         for task in resolved_tasks:
+            # construct a task name from the test task file path
             task_sub = re.sub(r"[^a-zA-Z0-9_-]", "_", task)
 
-            # prepare cluster
-            task_cluster = copy.deepcopy(cluster)
-            task_cluster["cluster_log_conf"] = {
-                "dbfs": {"destination": f"{test_folder.remote}/{task_sub}"}
-            }
-            if "instance_pool_id" in task_cluster:
-                task_cluster["instance_pool_id"] = pools.lookup(
-                    task_cluster["instance_pool_id"]
-                )
-
             workflow["tasks"].append(
                 dict(
                     task_key=task_sub,
                     libraries=sparklibs,
                     spark_python_task=dict(
-                        python_file=main_file.remote,
+                        python_file=main_file,
                         parameters=[
                             # running in the spark python interpreter, the python __file__ variable does not
                             # work. Hence, we need to tell the script where the test area is.
-                            f"--basedir={test_folder.local}/{task_sub}",
-                            # all tests will be unpacked from here
-                            f"--archive={archive_local}",
+                            f"--basedir={remote.remote_base()}",
                             # we can actually run any part of our test suite, but some files need the full repo.
                             # Only run tests from this folder.
                             f"--folder={task}",
                             # additional arguments to pass to pytest
                             f"--pytestargs={json.dumps(pytest_args)}",
                         ],
                     ),
-                    new_cluster=task_cluster,
+                    new_cluster=cluster,
                 )
             )
 
-    print("Submitting test...")
-    with tempfile.TemporaryDirectory() as tmp:
-        jobfile = f"{tmp}/job.json"
+        jobfile = remote.new_local_file("job.json").local
 
         with open(jobfile, "w") as f:
-            json.dump(workflow, f)
+            json.dump(workflow, f, indent=2)
 
-        if dry_run:
-            with open(jobfile) as f:
-                print("DEBUG: workflow:")
-                print(f.read())
+        remote.upload(dry_run)
+
+        if wait_for_job:
+            print("handing control to databricks jobs submit ...")
+            dbcli.execv_run_file(jobfile, dry_run=dry_run)
+            # the above function ends python and does not return
+            return
 
         try:
-            if not dry_run:
-                res = dbcli.submit_run_file(jobfile)
-            else:
-                print(f"DRY-RUN: Call: databricks runs submit --json-file {jobfile}")
-                print("DRY-RUN COMPLETED")
-                return
+            print("Submitting job...")
+            run_id = dbcli.submit(workflow, dry_run=dry_run)
         except subprocess.CalledProcessError:
             print("Json contents:")
             print(json.dumps(workflow, indent=4))
             raise
 
-        try:
-            run_id = res["run_id"]
-        except KeyError:
-            print(res)
-            raise
-
     # now we have the run_id
     print(f"Started run with ID {run_id}")
-    details = dbcli.get_run(run_id)
-    print(f"Follow job details at {details['run_page_url']}")
+    print(f"Follow job details at {dbcli.get_run(run_id).run_page_url}")
 
     if out_json:
         json.dump({"run_id": run_id}, out_json)
 
 
-def discover_and_push_wheels(globpath: str, test_folder: DbfsLocation) -> List[str]:
+def discover_wheels(globpath: str, remote: RemoteLocation) -> List[str]:
+    """Find all wheel files in the globpath and add them to the remote location."""
     result = []
     for item in Path().glob(globpath):
-        remote_path = f"{test_folder.remote}/{item.parts[-1]}"
-        print(f"pushing {item} to test folder")
-        dbcli.dbcall(f"fs cp {item} {remote_path}")
-        result.append(remote_path)
+        result.append(remote.add_local_path(str(item), "libs"))
 
     return result
 
 
-def archive_and_push(test_path: str, test_folder: DbfsLocation, dry_run=False):
-    with tempfile.TemporaryDirectory() as tmp:
-        test_path = Path(test_path)
-        print(f"now archiving {test_path}")
-        archive_path = shutil.make_archive(
-            str(Path(tmp) / "tests"),
+def prepare_archive(test_path: str, remote: RemoteLocation):
+    """Zip the test archive and add it to the staging area"""
+    print(f"now archiving {test_path}")
+
+    with tempfile.TemporaryDirectory() as tempdir:
+        real_archive_path = shutil.make_archive(
+            str(Path(tempdir) / "tests"),
             "zip",
-            test_path / "..",
-            base_dir=test_path.parts[-1],
+            Path(test_path) / "..",
+            base_dir=Path(test_path).parts[-1],
         )
-        print("now pushing test archive to test folder")
 
-        if not dry_run:
-            dbcli.dbcall(f"fs cp {archive_path} {test_folder.remote}/tests.zip")
-        else:
-            print(
-                f"DRY-RUN: Call: dbfs cp {archive_path} {test_folder.remote}/tests.zip"
-            )
-    return f"{test_folder.local}/tests.zip"
+        # it seems the doing a workspace import-dir on a zip archive will unpack it locally to upload.
+        # so we need to trick it by renaming the file
+        renamed_archive_path = Path(real_archive_path).with_suffix(".archive")
+        shutil.move(real_archive_path, renamed_archive_path)
+
+        return remote.add_local_path(str(renamed_archive_path))
+
 
+def prepare_main_file(remote: RemoteLocation, main_script: IO[str] = None) -> str:
+    print("now preparing test main file")
 
-def push_main_file(
-    test_folder: DbfsLocation, main_script: IO[str] = None, dry_run=False
-) -> DbfsLocation:
-    print("now pushing test main file")
-    main_file = test_folder / "main.py"
-    with tempfile.TemporaryDirectory() as tmp:
-        with open(Path(tmp) / "main.py", "w") as f:
-            if main_script:
-                f.write(main_script.read())
-            else:
-                print("Using default main script test_main.py")
-                f.write(inspect.getsource(test_main))
-        if not dry_run:
-            dbcli.dbcall(f"fs cp {tmp}/main.py {main_file.remote}")
+    main_ref = remote.new_local_file("main.py")
+
+    with open(main_ref.local, "w") as f:
+        if main_script:
+            f.write(main_script.read())
         else:
-            print(f"DRY-RUN: Call: dbfs cp {tmp}/main.py {main_file.remote}")
-    return main_file
+            print("Using default main script test_main.py")
+            f.write(inspect.getsource(test_main))
+
+    return main_ref.remote
```

### Comparing `spetlr-tools-0.1.65/src/spetlrtools/test_job/test_main.py` & `spetlr-tools-0.1.66/src/spetlrtools/test_job/test_main.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,67 +9,62 @@
 """
 
 import argparse
 import json
 import os
 import shutil
 import sys
-from hashlib import sha1
 from pathlib import Path
+from tempfile import TemporaryDirectory
 
 import pytest
 
-# print a marker message to screen to mark the start of python output
-# make it invisible using only "\u200E\u200F\u2060" https://invisible-characters.com/
-marker = "".join(list("\u200E\u200F\u2060")[i % 3] for i in sha1(b"my marker").digest())
-
 
 def test_main():
     """Main function to be called inside the test job task. Do not use directly."""
     parser = argparse.ArgumentParser(description="Run Test Cases.")
 
     # location to use for current run. Usually the cluster logs base folder
     parser.add_argument("--basedir")
 
     # relative path of test folder in test archive
     parser.add_argument("--folder")
 
     # archive of test files to use
-    parser.add_argument("--archive")
-
-    # archive of test files to use
     parser.add_argument("--pytestargs")
 
     args = parser.parse_args()
 
     extra_args = json.loads(args.pytestargs)
 
+    # move to basedir so that simple imports from one test to another work
+    basedir: str = args.basedir
+    if basedir.startswith("dbfs:"):
+        basedir = "/dbfs" + basedir[5:]
     # the basedir folder should exist because it is also the log destination
     # however we have seen cases where it does not exist yet at the start of the job,
     # so let's create it.
-    Path(args.basedir).mkdir(parents=True, exist_ok=True)
 
-    # move to basedir so that simple imports from one test to another work
-    os.chdir(args.basedir)
-    sys.path = [os.getcwd()] + sys.path
+    with TemporaryDirectory() as tmpdir:
+        os.chdir(tmpdir)
 
-    # unzip test archive to base folder
-    shutil.unpack_archive(args.archive)
+        sys.path = [tmpdir] + sys.path
 
-    # Ensure Spark is initialized before any tests are run
-    # the import statement is inside the function so that the outer file
-    # can be imported even where pyspark may not be available
-    from spetlr.spark import Spark
-
-    Spark.get()
-
-    print()
-    print(marker)
-    print()
-
-    retcode = pytest.main(["-x", args.folder, *extra_args])
-    if retcode.value:
-        raise Exception("Pytest failed")
+        # unzip test archive to base folder
+        shutil.copy(Path(basedir) / "tests.archive", "tests.zip")
+        shutil.unpack_archive("tests.zip")
+        os.unlink("tests.zip")
+
+        # Ensure Spark is initialized before any tests are run
+        # the import statement is inside the function so that the outer file
+        # can be imported even where pyspark may not be available
+        from spetlr.spark import Spark
+
+        Spark.get()
+
+        retcode = pytest.main(["-x", args.folder, *extra_args])
+        if retcode.value:
+            raise Exception("Pytest failed")
 
 
 if __name__ == "__main__":
     test_main()
```

### Comparing `spetlr-tools-0.1.65/src/spetlrtools/testing/DataframeTestCase.py` & `spetlr-tools-0.1.66/src/spetlrtools/testing/DataframeTestCase.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.65/src/spetlrtools/testing/TestHandle.py` & `spetlr-tools-0.1.66/src/spetlrtools/testing/TestHandle.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.65/src/spetlrtools/testing/TupleComparer.py` & `spetlr-tools-0.1.66/src/spetlrtools/testing/TupleComparer.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.65/src/spetlrtools/time/TimeSequence.py` & `spetlr-tools-0.1.66/src/spetlrtools/time/TimeSequence.py`

 * *Files identical despite different names*

