# Comparing `tmp/xbot.framework-0.1.0.tar.gz` & `tmp/xbot.framework-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/wan/CodeProjects/xbot/dist/tmprqriunw5/xbot.framework-0.1.0.tar", last modified: Fri May 31 05:11:36 2024, max compression
+gzip compressed data, was "/Users/wan/CodeProjects/xbot.framework/dist/tmpmrcpl002/xbot.framework-0.2.0.tar", last modified: Mon Jun  3 10:12:53 2024, max compression
```

## Comparing `xbot.framework-0.1.0.tar` & `xbot.framework-0.2.0.tar`

### file list

```diff
@@ -1,76 +1,116 @@
-drwxr-xr-x   0 wan        (501) staff       (20)        0 2024-05-31 05:11:36.000000 xbot.framework-0.1.0/
--rw-r--r--   0 wan        (501) staff       (20)     8828 2024-05-31 05:11:36.000000 xbot.framework-0.1.0/PKG-INFO
--rw-r--r--   0 wan        (501) staff       (20)     1325 2022-12-04 03:22:04.000000 xbot.framework-0.1.0/LICENSE
--rw-r--r--   0 wan        (501) staff       (20)       69 2024-05-30 15:02:39.000000 xbot.framework-0.1.0/requirements.txt
--rw-r--r--   0 wan        (501) staff       (20)       87 2024-05-30 03:56:33.000000 xbot.framework-0.1.0/pyproject.toml
-drwxr-xr-x   0 wan        (501) staff       (20)        0 2024-05-31 05:11:36.000000 xbot.framework-0.1.0/tests/
--rw-r--r--   0 wan        (501) staff       (20)     3700 2024-01-01 14:23:21.000000 xbot.framework-0.1.0/tests/test_utils.py
--rw-r--r--   0 wan        (501) staff       (20)        0 2022-12-04 09:50:25.000000 xbot.framework-0.1.0/tests/__init__.py
--rw-r--r--   0 wan        (501) staff       (20)      710 2024-05-31 01:50:41.000000 xbot.framework-0.1.0/tests/test_report.py
--rw-r--r--   0 wan        (501) staff       (20)     8242 2024-05-31 01:51:00.000000 xbot.framework-0.1.0/tests/test_testcase.py
--rw-r--r--   0 wan        (501) staff       (20)     2576 2024-05-31 01:50:47.000000 xbot.framework-0.1.0/tests/test_runner.py
--rw-r--r--   0 wan        (501) staff       (20)     5414 2024-05-31 01:51:18.000000 xbot.framework-0.1.0/tests/test_testset.py
--rw-r--r--   0 wan        (501) staff       (20)     1445 2023-12-05 09:22:03.000000 xbot.framework-0.1.0/tests/test_testbed.py
--rw-r--r--   0 wan        (501) staff       (20)     4173 2024-01-03 09:20:13.000000 xbot.framework-0.1.0/tests/test_main.py
--rw-r--r--   0 wan        (501) staff       (20)     3209 2023-12-05 07:47:28.000000 xbot.framework-0.1.0/tests/test_logger.py
--rw-r--r--   0 wan        (501) staff       (20)       58 2024-05-30 14:48:10.000000 xbot.framework-0.1.0/MANIFEST.in
--rw-r--r--   0 wan        (501) staff       (20)     2166 2024-05-31 04:35:18.000000 xbot.framework-0.1.0/setup.py
-drwxr-xr-x   0 wan        (501) staff       (20)        0 2024-05-31 05:11:36.000000 xbot.framework-0.1.0/xbot/
--rw-r--r--   0 wan        (501) staff       (20)     3867 2024-05-31 01:25:23.000000 xbot.framework-0.1.0/xbot/runner.py
-drwxr-xr-x   0 wan        (501) staff       (20)        0 2024-05-31 05:11:36.000000 xbot.framework-0.1.0/xbot/statics/
-drwxr-xr-x   0 wan        (501) staff       (20)        0 2024-05-31 05:11:36.000000 xbot.framework-0.1.0/xbot/statics/initdir/
-drwxr-xr-x   0 wan        (501) staff       (20)        0 2024-05-31 05:11:36.000000 xbot.framework-0.1.0/xbot/statics/initdir/testbeds/
--rw-r--r--   0 wan        (501) staff       (20)      262 2023-12-11 14:46:15.000000 xbot.framework-0.1.0/xbot/statics/initdir/testbeds/testbed_example.yml
--rw-r--r--   0 wan        (501) staff       (20)        5 2023-10-16 13:52:42.000000 xbot.framework-0.1.0/xbot/statics/initdir/requirements.txt
-drwxr-xr-x   0 wan        (501) staff       (20)        0 2024-05-31 05:11:36.000000 xbot.framework-0.1.0/xbot/statics/initdir/testsets/
--rw-r--r--   0 wan        (501) staff       (20)      338 2023-12-08 15:28:33.000000 xbot.framework-0.1.0/xbot/statics/initdir/testsets/testset_example.yml
--rw-r--r--   0 wan        (501) staff       (20)        0 2023-10-16 13:52:04.000000 xbot.framework-0.1.0/xbot/statics/initdir/README.md
--rw-r--r--   0 wan        (501) staff       (20)      233 2023-11-03 14:04:30.000000 xbot.framework-0.1.0/xbot/statics/initdir/.gitignore
-drwxr-xr-x   0 wan        (501) staff       (20)        0 2024-05-31 05:11:36.000000 xbot.framework-0.1.0/xbot/statics/initdir/lib/
--rw-r--r--   0 wan        (501) staff       (20)      132 2023-12-03 13:33:03.000000 xbot.framework-0.1.0/xbot/statics/initdir/lib/testcase.py
--rw-r--r--   0 wan        (501) staff       (20)        0 2023-10-16 08:58:32.000000 xbot.framework-0.1.0/xbot/statics/initdir/lib/__init__.py
--rw-r--r--   0 wan        (501) staff       (20)      131 2023-12-03 13:32:44.000000 xbot.framework-0.1.0/xbot/statics/initdir/lib/testbed.py
-drwxr-xr-x   0 wan        (501) staff       (20)        0 2024-05-31 05:11:36.000000 xbot.framework-0.1.0/xbot/statics/initdir/testcases/
--rw-r--r--   0 wan        (501) staff       (20)        0 2023-10-16 09:05:26.000000 xbot.framework-0.1.0/xbot/statics/initdir/testcases/__init__.py
-drwxr-xr-x   0 wan        (501) staff       (20)        0 2024-05-31 05:11:36.000000 xbot.framework-0.1.0/xbot/statics/initdir/testcases/examples/
-drwxr-xr-x   0 wan        (501) staff       (20)        0 2024-05-31 05:11:36.000000 xbot.framework-0.1.0/xbot/statics/initdir/testcases/examples/pass/
--rw-r--r--   0 wan        (501) staff       (20)     1282 2023-12-08 15:27:10.000000 xbot.framework-0.1.0/xbot/statics/initdir/testcases/examples/pass/tc_eg_pass_get_values_from_testbed.py
--rw-r--r--   0 wan        (501) staff       (20)        0 2023-11-15 14:42:48.000000 xbot.framework-0.1.0/xbot/statics/initdir/testcases/examples/pass/__init__.py
--rw-r--r--   0 wan        (501) staff       (20)     1489 2023-12-08 15:27:03.000000 xbot.framework-0.1.0/xbot/statics/initdir/testcases/examples/pass/tc_eg_pass_create_dirs_and_files.py
--rw-r--r--   0 wan        (501) staff       (20)        0 2023-11-15 14:42:48.000000 xbot.framework-0.1.0/xbot/statics/initdir/testcases/examples/__init__.py
-drwxr-xr-x   0 wan        (501) staff       (20)        0 2024-05-31 05:11:36.000000 xbot.framework-0.1.0/xbot/statics/initdir/testcases/examples/nonpass/
--rw-r--r--   0 wan        (501) staff       (20)      608 2023-12-11 10:02:31.000000 xbot.framework-0.1.0/xbot/statics/initdir/testcases/examples/nonpass/tc_eg_nonpass_skip_not_included.py
--rw-r--r--   0 wan        (501) staff       (20)      632 2023-12-11 10:50:26.000000 xbot.framework-0.1.0/xbot/statics/initdir/testcases/examples/nonpass/tc_eg_nonpass_error_syntax.py
--rw-r--r--   0 wan        (501) staff       (20)        0 2023-11-15 14:42:48.000000 xbot.framework-0.1.0/xbot/statics/initdir/testcases/examples/nonpass/__init__.py
--rw-r--r--   0 wan        (501) staff       (20)      803 2023-12-17 08:24:49.000000 xbot.framework-0.1.0/xbot/statics/initdir/testcases/examples/nonpass/tc_eg_nonpass_fail_setup_with_failfast_false.py
--rw-r--r--   0 wan        (501) staff       (20)      732 2023-12-17 08:24:18.000000 xbot.framework-0.1.0/xbot/statics/initdir/testcases/examples/nonpass/tc_eg_nonpass_fail_step_with_failfast_false.py
--rw-r--r--   0 wan        (501) staff       (20)      747 2023-12-13 14:38:59.000000 xbot.framework-0.1.0/xbot/statics/initdir/testcases/examples/nonpass/tc_eg_nonpass_timeout.py
--rw-r--r--   0 wan        (501) staff       (20)      746 2023-12-17 08:24:10.000000 xbot.framework-0.1.0/xbot/statics/initdir/testcases/examples/nonpass/tc_eg_nonpass_fail_step_with_failfast_true.py
--rw-r--r--   0 wan        (501) staff       (20)      605 2023-12-11 10:13:23.000000 xbot.framework-0.1.0/xbot/statics/initdir/testcases/examples/nonpass/tc_eg_nonpass_error_clsname.py
--rw-r--r--   0 wan        (501) staff       (20)      800 2023-12-17 08:24:41.000000 xbot.framework-0.1.0/xbot/statics/initdir/testcases/examples/nonpass/tc_eg_nonpass_fail_setup_with_failfast_true.py
--rw-r--r--   0 wan        (501) staff       (20)      615 2023-12-11 10:02:18.000000 xbot.framework-0.1.0/xbot/statics/initdir/testcases/examples/nonpass/tc_eg_nonpass_skip_excluded.py
--rw-r--r--   0 wan        (501) staff       (20)     6148 2023-10-10 12:55:57.000000 xbot.framework-0.1.0/xbot/statics/.DS_Store
--rw-r--r--   0 wan        (501) staff       (20)   171041 2024-05-30 09:50:47.000000 xbot.framework-0.1.0/xbot/statics/report_example.png
--rw-r--r--   0 wan        (501) staff       (20)     5313 2024-05-29 08:50:46.000000 xbot.framework-0.1.0/xbot/statics/log_template.html
--rw-r--r--   0 wan        (501) staff       (20)   147988 2024-05-29 08:55:55.000000 xbot.framework-0.1.0/xbot/statics/log_example.png
--rw-r--r--   0 wan        (501) staff       (20)     5394 2023-12-14 15:02:54.000000 xbot.framework-0.1.0/xbot/statics/report_template.html
--rw-r--r--   0 wan        (501) staff       (20)       83 2024-05-30 08:28:23.000000 xbot.framework-0.1.0/xbot/version.py
--rw-r--r--   0 wan        (501) staff       (20)     9560 2024-05-31 01:51:46.000000 xbot.framework-0.1.0/xbot/testcase.py
--rw-r--r--   0 wan        (501) staff       (20)        0 2023-11-06 10:52:40.000000 xbot.framework-0.1.0/xbot/__init__.py
--rw-r--r--   0 wan        (501) staff       (20)     4364 2024-05-29 08:50:07.000000 xbot.framework-0.1.0/xbot/logger.py
--rw-r--r--   0 wan        (501) staff       (20)     3200 2024-05-31 01:46:03.000000 xbot.framework-0.1.0/xbot/testset.py
--rw-r--r--   0 wan        (501) staff       (20)     1723 2024-05-31 02:30:34.000000 xbot.framework-0.1.0/xbot/testbed.py
--rw-r--r--   0 wan        (501) staff       (20)      375 2024-01-03 07:53:04.000000 xbot.framework-0.1.0/xbot/common.py
--rw-r--r--   0 wan        (501) staff       (20)    10110 2024-05-31 01:52:25.000000 xbot.framework-0.1.0/xbot/utils.py
--rw-r--r--   0 wan        (501) staff       (20)      340 2023-12-17 08:28:56.000000 xbot.framework-0.1.0/xbot/errors.py
--rw-r--r--   0 wan        (501) staff       (20)     2909 2024-05-31 02:21:10.000000 xbot.framework-0.1.0/xbot/main.py
--rw-r--r--   0 wan        (501) staff       (20)     2775 2024-05-31 01:51:33.000000 xbot.framework-0.1.0/xbot/report.py
--rw-r--r--   0 wan        (501) staff       (20)       38 2024-05-31 05:11:36.000000 xbot.framework-0.1.0/setup.cfg
--rw-r--r--   0 wan        (501) staff       (20)     7850 2024-05-31 05:07:07.000000 xbot.framework-0.1.0/README.rst
-drwxr-xr-x   0 wan        (501) staff       (20)        0 2024-05-31 05:11:36.000000 xbot.framework-0.1.0/xbot.framework.egg-info/
--rw-r--r--   0 wan        (501) staff       (20)     8828 2024-05-31 05:11:36.000000 xbot.framework-0.1.0/xbot.framework.egg-info/PKG-INFO
--rw-r--r--   0 wan        (501) staff       (20)     2280 2024-05-31 05:11:36.000000 xbot.framework-0.1.0/xbot.framework.egg-info/SOURCES.txt
--rw-r--r--   0 wan        (501) staff       (20)       41 2024-05-31 05:11:36.000000 xbot.framework-0.1.0/xbot.framework.egg-info/entry_points.txt
--rw-r--r--   0 wan        (501) staff       (20)       47 2024-05-31 05:11:36.000000 xbot.framework-0.1.0/xbot.framework.egg-info/requires.txt
--rw-r--r--   0 wan        (501) staff       (20)       11 2024-05-31 05:11:36.000000 xbot.framework-0.1.0/xbot.framework.egg-info/top_level.txt
--rw-r--r--   0 wan        (501) staff       (20)        1 2024-05-31 05:11:36.000000 xbot.framework-0.1.0/xbot.framework.egg-info/dependency_links.txt
+drwxr-xr-x   0 wan        (501) staff       (20)        0 2024-06-03 10:12:53.000000 xbot.framework-0.2.0/
+-rw-r--r--   0 wan        (501) staff       (20)     8878 2024-06-03 10:12:53.000000 xbot.framework-0.2.0/PKG-INFO
+-rw-r--r--   0 wan        (501) staff       (20)     1325 2022-12-04 03:22:04.000000 xbot.framework-0.2.0/LICENSE
+-rw-r--r--   0 wan        (501) staff       (20)       69 2024-05-30 15:02:39.000000 xbot.framework-0.2.0/requirements.txt
+-rw-r--r--   0 wan        (501) staff       (20)       87 2024-05-30 03:56:33.000000 xbot.framework-0.2.0/pyproject.toml
+drwxr-xr-x   0 wan        (501) staff       (20)        0 2024-06-03 10:12:53.000000 xbot.framework-0.2.0/tests/
+-rw-r--r--   0 wan        (501) staff       (20)     3710 2024-06-03 08:03:27.000000 xbot.framework-0.2.0/tests/test_utils.py
+-rw-r--r--   0 wan        (501) staff       (20)      256 2024-06-03 08:23:30.000000 xbot.framework-0.2.0/tests/run.py
+-rw-r--r--   0 wan        (501) staff       (20)        0 2022-12-04 09:50:25.000000 xbot.framework-0.2.0/tests/__init__.py
+-rw-r--r--   0 wan        (501) staff       (20)      720 2024-06-03 08:03:27.000000 xbot.framework-0.2.0/tests/test_report.py
+-rw-r--r--   0 wan        (501) staff       (20)     8292 2024-06-03 08:03:27.000000 xbot.framework-0.2.0/tests/test_testcase.py
+-rw-r--r--   0 wan        (501) staff       (20)     2636 2024-06-03 08:03:27.000000 xbot.framework-0.2.0/tests/test_runner.py
+-rw-r--r--   0 wan        (501) staff       (20)     5424 2024-06-03 08:03:27.000000 xbot.framework-0.2.0/tests/test_testset.py
+-rw-r--r--   0 wan        (501) staff       (20)     1455 2024-06-03 08:03:27.000000 xbot.framework-0.2.0/tests/test_testbed.py
+-rw-r--r--   0 wan        (501) staff       (20)     4233 2024-06-03 08:14:53.000000 xbot.framework-0.2.0/tests/test_main.py
+-rw-r--r--   0 wan        (501) staff       (20)     3219 2024-06-03 08:03:27.000000 xbot.framework-0.2.0/tests/test_logger.py
+-rw-r--r--   0 wan        (501) staff       (20)       68 2024-06-03 08:42:06.000000 xbot.framework-0.2.0/MANIFEST.in
+-rw-r--r--   0 wan        (501) staff       (20)     2274 2024-06-03 09:02:47.000000 xbot.framework-0.2.0/setup.py
+drwxr-xr-x   0 wan        (501) staff       (20)        0 2024-06-03 10:12:53.000000 xbot.framework-0.2.0/xbot/
+drwxr-xr-x   0 wan        (501) staff       (20)        0 2024-06-03 10:12:53.000000 xbot.framework-0.2.0/xbot/framework/
+-rw-r--r--   0 wan        (501) staff       (20)     3917 2024-06-03 08:03:27.000000 xbot.framework-0.2.0/xbot/framework/runner.py
+drwxr-xr-x   0 wan        (501) staff       (20)        0 2024-06-03 10:12:53.000000 xbot.framework-0.2.0/xbot/framework/statics/
+drwxr-xr-x   0 wan        (501) staff       (20)        0 2024-06-03 10:12:53.000000 xbot.framework-0.2.0/xbot/framework/statics/initdir/
+drwxr-xr-x   0 wan        (501) staff       (20)        0 2024-06-03 10:12:53.000000 xbot.framework-0.2.0/xbot/framework/statics/initdir/testbeds/
+-rw-r--r--   0 wan        (501) staff       (20)      262 2023-12-11 14:46:15.000000 xbot.framework-0.2.0/xbot/framework/statics/initdir/testbeds/testbed_example.yml
+-rw-r--r--   0 wan        (501) staff       (20)        5 2023-10-16 13:52:42.000000 xbot.framework-0.2.0/xbot/framework/statics/initdir/requirements.txt
+drwxr-xr-x   0 wan        (501) staff       (20)        0 2024-06-03 10:12:53.000000 xbot.framework-0.2.0/xbot/framework/statics/initdir/testsets/
+-rw-r--r--   0 wan        (501) staff       (20)      338 2023-12-08 15:28:33.000000 xbot.framework-0.2.0/xbot/framework/statics/initdir/testsets/testset_example.yml
+-rw-r--r--   0 wan        (501) staff       (20)        0 2023-10-16 13:52:04.000000 xbot.framework-0.2.0/xbot/framework/statics/initdir/README.md
+-rw-r--r--   0 wan        (501) staff       (20)      233 2023-11-03 14:04:30.000000 xbot.framework-0.2.0/xbot/framework/statics/initdir/.gitignore
+drwxr-xr-x   0 wan        (501) staff       (20)        0 2024-06-03 10:12:53.000000 xbot.framework-0.2.0/xbot/framework/statics/initdir/lib/
+-rw-r--r--   0 wan        (501) staff       (20)      142 2024-06-03 08:03:27.000000 xbot.framework-0.2.0/xbot/framework/statics/initdir/lib/testcase.py
+-rw-r--r--   0 wan        (501) staff       (20)        0 2023-10-16 08:58:32.000000 xbot.framework-0.2.0/xbot/framework/statics/initdir/lib/__init__.py
+-rw-r--r--   0 wan        (501) staff       (20)      141 2024-06-03 08:03:27.000000 xbot.framework-0.2.0/xbot/framework/statics/initdir/lib/testbed.py
+drwxr-xr-x   0 wan        (501) staff       (20)        0 2024-06-03 10:12:53.000000 xbot.framework-0.2.0/xbot/framework/statics/initdir/testcases/
+-rw-r--r--   0 wan        (501) staff       (20)        0 2023-10-16 09:05:26.000000 xbot.framework-0.2.0/xbot/framework/statics/initdir/testcases/__init__.py
+drwxr-xr-x   0 wan        (501) staff       (20)        0 2024-06-03 10:12:53.000000 xbot.framework-0.2.0/xbot/framework/statics/initdir/testcases/examples/
+drwxr-xr-x   0 wan        (501) staff       (20)        0 2024-06-03 10:12:53.000000 xbot.framework-0.2.0/xbot/framework/statics/initdir/testcases/examples/pass/
+-rw-r--r--   0 wan        (501) staff       (20)     1292 2024-06-03 08:03:27.000000 xbot.framework-0.2.0/xbot/framework/statics/initdir/testcases/examples/pass/tc_eg_pass_get_values_from_testbed.py
+-rw-r--r--   0 wan        (501) staff       (20)        0 2023-11-15 14:42:48.000000 xbot.framework-0.2.0/xbot/framework/statics/initdir/testcases/examples/pass/__init__.py
+-rw-r--r--   0 wan        (501) staff       (20)     1499 2024-06-03 08:03:27.000000 xbot.framework-0.2.0/xbot/framework/statics/initdir/testcases/examples/pass/tc_eg_pass_create_dirs_and_files.py
+-rw-r--r--   0 wan        (501) staff       (20)        0 2023-11-15 14:42:48.000000 xbot.framework-0.2.0/xbot/framework/statics/initdir/testcases/examples/__init__.py
+drwxr-xr-x   0 wan        (501) staff       (20)        0 2024-06-03 10:12:53.000000 xbot.framework-0.2.0/xbot/framework/statics/initdir/testcases/examples/nonpass/
+-rw-r--r--   0 wan        (501) staff       (20)      618 2024-06-03 08:03:27.000000 xbot.framework-0.2.0/xbot/framework/statics/initdir/testcases/examples/nonpass/tc_eg_nonpass_skip_not_included.py
+-rw-r--r--   0 wan        (501) staff       (20)      642 2024-06-03 08:03:27.000000 xbot.framework-0.2.0/xbot/framework/statics/initdir/testcases/examples/nonpass/tc_eg_nonpass_error_syntax.py
+-rw-r--r--   0 wan        (501) staff       (20)        0 2023-11-15 14:42:48.000000 xbot.framework-0.2.0/xbot/framework/statics/initdir/testcases/examples/nonpass/__init__.py
+-rw-r--r--   0 wan        (501) staff       (20)      813 2024-06-03 08:03:27.000000 xbot.framework-0.2.0/xbot/framework/statics/initdir/testcases/examples/nonpass/tc_eg_nonpass_fail_setup_with_failfast_false.py
+-rw-r--r--   0 wan        (501) staff       (20)      742 2024-06-03 08:03:27.000000 xbot.framework-0.2.0/xbot/framework/statics/initdir/testcases/examples/nonpass/tc_eg_nonpass_fail_step_with_failfast_false.py
+-rw-r--r--   0 wan        (501) staff       (20)      757 2024-06-03 08:03:27.000000 xbot.framework-0.2.0/xbot/framework/statics/initdir/testcases/examples/nonpass/tc_eg_nonpass_timeout.py
+-rw-r--r--   0 wan        (501) staff       (20)      756 2024-06-03 08:03:27.000000 xbot.framework-0.2.0/xbot/framework/statics/initdir/testcases/examples/nonpass/tc_eg_nonpass_fail_step_with_failfast_true.py
+-rw-r--r--   0 wan        (501) staff       (20)      615 2024-06-03 08:03:27.000000 xbot.framework-0.2.0/xbot/framework/statics/initdir/testcases/examples/nonpass/tc_eg_nonpass_error_clsname.py
+-rw-r--r--   0 wan        (501) staff       (20)      810 2024-06-03 08:03:27.000000 xbot.framework-0.2.0/xbot/framework/statics/initdir/testcases/examples/nonpass/tc_eg_nonpass_fail_setup_with_failfast_true.py
+-rw-r--r--   0 wan        (501) staff       (20)      625 2024-06-03 08:03:27.000000 xbot.framework-0.2.0/xbot/framework/statics/initdir/testcases/examples/nonpass/tc_eg_nonpass_skip_excluded.py
+-rw-r--r--   0 wan        (501) staff       (20)     6148 2023-10-10 12:55:57.000000 xbot.framework-0.2.0/xbot/framework/statics/.DS_Store
+-rw-r--r--   0 wan        (501) staff       (20)   160004 2024-06-03 08:54:49.000000 xbot.framework-0.2.0/xbot/framework/statics/report_example.png
+-rw-r--r--   0 wan        (501) staff       (20)     5317 2024-06-02 08:41:31.000000 xbot.framework-0.2.0/xbot/framework/statics/log_template.html
+-rw-r--r--   0 wan        (501) staff       (20)   160485 2024-06-03 08:54:49.000000 xbot.framework-0.2.0/xbot/framework/statics/log_example.png
+-rw-r--r--   0 wan        (501) staff       (20)     5394 2023-12-14 15:02:54.000000 xbot.framework-0.2.0/xbot/framework/statics/report_template.html
+-rw-r--r--   0 wan        (501) staff       (20)       83 2024-06-02 08:59:57.000000 xbot.framework-0.2.0/xbot/framework/version.py
+-rw-r--r--   0 wan        (501) staff       (20)     9649 2024-06-03 08:03:27.000000 xbot.framework-0.2.0/xbot/framework/testcase.py
+-rw-r--r--   0 wan        (501) staff       (20)        0 2023-11-06 10:52:40.000000 xbot.framework-0.2.0/xbot/framework/__init__.py
+-rw-r--r--   0 wan        (501) staff       (20)     4587 2024-06-02 08:58:00.000000 xbot.framework-0.2.0/xbot/framework/logger.py
+-rw-r--r--   0 wan        (501) staff       (20)     3220 2024-06-03 08:03:27.000000 xbot.framework-0.2.0/xbot/framework/testset.py
+-rw-r--r--   0 wan        (501) staff       (20)     1733 2024-06-03 08:03:27.000000 xbot.framework-0.2.0/xbot/framework/testbed.py
+-rw-r--r--   0 wan        (501) staff       (20)      375 2024-01-03 07:53:04.000000 xbot.framework-0.2.0/xbot/framework/common.py
+-rw-r--r--   0 wan        (501) staff       (20)    10122 2024-06-03 08:03:27.000000 xbot.framework-0.2.0/xbot/framework/utils.py
+-rw-r--r--   0 wan        (501) staff       (20)      340 2023-12-17 08:28:56.000000 xbot.framework-0.2.0/xbot/framework/errors.py
+-rw-r--r--   0 wan        (501) staff       (20)     2969 2024-06-03 08:03:27.000000 xbot.framework-0.2.0/xbot/framework/main.py
+-rw-r--r--   0 wan        (501) staff       (20)     2795 2024-06-03 08:03:27.000000 xbot.framework-0.2.0/xbot/framework/report.py
+-rw-r--r--   0 wan        (501) staff       (20)       38 2024-06-03 10:12:53.000000 xbot.framework-0.2.0/setup.cfg
+drwxr-xr-x   0 wan        (501) staff       (20)        0 2024-06-03 10:12:53.000000 xbot.framework-0.2.0/venv/
+drwxr-xr-x   0 wan        (501) staff       (20)        0 2024-06-03 10:12:53.000000 xbot.framework-0.2.0/venv/bin/
+-rwxr-xr-x   0 wan        (501) staff       (20)      912 2024-06-03 09:54:14.000000 xbot.framework-0.2.0/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 wan        (501) staff       (20)      832 2024-06-03 09:54:14.000000 xbot.framework-0.2.0/venv/bin/rst2latex.py
+-rwxr-xr-x   0 wan        (501) staff       (20)     1767 2024-06-03 09:54:14.000000 xbot.framework-0.2.0/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 wan        (501) staff       (20)      755 2024-06-03 09:54:14.000000 xbot.framework-0.2.0/venv/bin/rst2html4.py
+-rwxr-xr-x   0 wan        (501) staff       (20)     1123 2024-06-03 09:54:14.000000 xbot.framework-0.2.0/venv/bin/rst2html5.py
+-rwxr-xr-x   0 wan        (501) staff       (20)      643 2024-06-03 09:54:14.000000 xbot.framework-0.2.0/venv/bin/rst2xml.py
+-rwxr-xr-x   0 wan        (501) staff       (20)      805 2024-06-03 09:54:14.000000 xbot.framework-0.2.0/venv/bin/rst2odt.py
+-rwxr-xr-x   0 wan        (501) staff       (20)      642 2024-06-03 09:54:14.000000 xbot.framework-0.2.0/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 wan        (501) staff       (20)      678 2024-06-03 09:54:14.000000 xbot.framework-0.2.0/venv/bin/rst2s5.py
+-rwxr-xr-x   0 wan        (501) staff       (20)      635 2024-06-03 09:54:14.000000 xbot.framework-0.2.0/venv/bin/rst2html.py
+-rwxr-xr-x   0 wan        (501) staff       (20)      640 2024-06-03 09:54:14.000000 xbot.framework-0.2.0/venv/bin/rst2man.py
+-rwxr-xr-x   0 wan        (501) staff       (20)      711 2024-06-03 09:54:14.000000 xbot.framework-0.2.0/venv/bin/rstpep2html.py
+-rw-r--r--   0 wan        (501) staff       (20)     7870 2024-06-03 10:07:49.000000 xbot.framework-0.2.0/README.rst
+drwxr-xr-x   0 wan        (501) staff       (20)        0 2024-06-03 10:12:53.000000 xbot.framework-0.2.0/testproj/
+drwxr-xr-x   0 wan        (501) staff       (20)        0 2024-06-03 10:12:53.000000 xbot.framework-0.2.0/testproj/lib/
+-rw-r--r--   0 wan        (501) staff       (20)      142 2024-06-03 08:03:27.000000 xbot.framework-0.2.0/testproj/lib/testcase.py
+-rw-r--r--   0 wan        (501) staff       (20)        0 2023-10-16 08:58:32.000000 xbot.framework-0.2.0/testproj/lib/__init__.py
+-rw-r--r--   0 wan        (501) staff       (20)      141 2024-06-03 08:03:27.000000 xbot.framework-0.2.0/testproj/lib/testbed.py
+drwxr-xr-x   0 wan        (501) staff       (20)        0 2024-06-03 10:12:53.000000 xbot.framework-0.2.0/testproj/testcases/
+-rw-r--r--   0 wan        (501) staff       (20)        0 2023-10-16 09:05:26.000000 xbot.framework-0.2.0/testproj/testcases/__init__.py
+drwxr-xr-x   0 wan        (501) staff       (20)        0 2024-06-03 10:12:53.000000 xbot.framework-0.2.0/testproj/testcases/examples/
+drwxr-xr-x   0 wan        (501) staff       (20)        0 2024-06-03 10:12:53.000000 xbot.framework-0.2.0/testproj/testcases/examples/pass/
+-rw-r--r--   0 wan        (501) staff       (20)     1292 2024-06-03 08:03:27.000000 xbot.framework-0.2.0/testproj/testcases/examples/pass/tc_eg_pass_get_values_from_testbed.py
+-rw-r--r--   0 wan        (501) staff       (20)        0 2023-11-15 14:42:48.000000 xbot.framework-0.2.0/testproj/testcases/examples/pass/__init__.py
+-rw-r--r--   0 wan        (501) staff       (20)     1499 2024-06-03 08:03:27.000000 xbot.framework-0.2.0/testproj/testcases/examples/pass/tc_eg_pass_create_dirs_and_files.py
+-rw-r--r--   0 wan        (501) staff       (20)        0 2023-11-15 14:42:48.000000 xbot.framework-0.2.0/testproj/testcases/examples/__init__.py
+drwxr-xr-x   0 wan        (501) staff       (20)        0 2024-06-03 10:12:53.000000 xbot.framework-0.2.0/testproj/testcases/examples/nonpass/
+-rw-r--r--   0 wan        (501) staff       (20)      618 2024-06-03 08:03:27.000000 xbot.framework-0.2.0/testproj/testcases/examples/nonpass/tc_eg_nonpass_skip_not_included.py
+-rw-r--r--   0 wan        (501) staff       (20)      642 2024-06-03 08:03:27.000000 xbot.framework-0.2.0/testproj/testcases/examples/nonpass/tc_eg_nonpass_error_syntax.py
+-rw-r--r--   0 wan        (501) staff       (20)        0 2023-11-15 14:42:48.000000 xbot.framework-0.2.0/testproj/testcases/examples/nonpass/__init__.py
+-rw-r--r--   0 wan        (501) staff       (20)      813 2024-06-03 08:03:27.000000 xbot.framework-0.2.0/testproj/testcases/examples/nonpass/tc_eg_nonpass_fail_setup_with_failfast_false.py
+-rw-r--r--   0 wan        (501) staff       (20)      742 2024-06-03 08:03:27.000000 xbot.framework-0.2.0/testproj/testcases/examples/nonpass/tc_eg_nonpass_fail_step_with_failfast_false.py
+-rw-r--r--   0 wan        (501) staff       (20)      757 2024-06-03 08:03:27.000000 xbot.framework-0.2.0/testproj/testcases/examples/nonpass/tc_eg_nonpass_timeout.py
+-rw-r--r--   0 wan        (501) staff       (20)      756 2024-06-03 08:03:27.000000 xbot.framework-0.2.0/testproj/testcases/examples/nonpass/tc_eg_nonpass_fail_step_with_failfast_true.py
+-rw-r--r--   0 wan        (501) staff       (20)      615 2024-06-03 08:03:27.000000 xbot.framework-0.2.0/testproj/testcases/examples/nonpass/tc_eg_nonpass_error_clsname.py
+-rw-r--r--   0 wan        (501) staff       (20)      810 2024-06-03 08:03:27.000000 xbot.framework-0.2.0/testproj/testcases/examples/nonpass/tc_eg_nonpass_fail_setup_with_failfast_true.py
+-rw-r--r--   0 wan        (501) staff       (20)      625 2024-06-03 08:03:27.000000 xbot.framework-0.2.0/testproj/testcases/examples/nonpass/tc_eg_nonpass_skip_excluded.py
+drwxr-xr-x   0 wan        (501) staff       (20)        0 2024-06-03 10:12:53.000000 xbot.framework-0.2.0/xbot.framework.egg-info/
+-rw-r--r--   0 wan        (501) staff       (20)     8878 2024-06-03 10:12:53.000000 xbot.framework-0.2.0/xbot.framework.egg-info/PKG-INFO
+-rw-r--r--   0 wan        (501) staff       (20)     4004 2024-06-03 10:12:53.000000 xbot.framework-0.2.0/xbot.framework.egg-info/SOURCES.txt
+-rw-r--r--   0 wan        (501) staff       (20)       51 2024-06-03 10:12:53.000000 xbot.framework-0.2.0/xbot.framework.egg-info/entry_points.txt
+-rw-r--r--   0 wan        (501) staff       (20)       47 2024-06-03 10:12:53.000000 xbot.framework-0.2.0/xbot.framework.egg-info/requires.txt
+-rw-r--r--   0 wan        (501) staff       (20)       35 2024-06-03 10:12:53.000000 xbot.framework-0.2.0/xbot.framework.egg-info/top_level.txt
+-rw-r--r--   0 wan        (501) staff       (20)        1 2024-06-03 10:12:53.000000 xbot.framework-0.2.0/xbot.framework.egg-info/dependency_links.txt
```

### Comparing `xbot.framework-0.1.0/PKG-INFO` & `xbot.framework-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: xbot.framework
-Version: 0.1.0
+Version: 0.2.0
 Summary: A lightweight, easy-to-use, and extensible automation testing framework.
-Home-page: https://github.com/zhaowcheng/xbot
+Home-page: https://github.com/zhaowcheng/xbot.framework
 Author: zhaowcheng
 Author-email: zhaowcheng@163.com
 License: UNKNOWN
-Project-URL: Homepage, https://github.com/zhaowcheng/xbot
-Project-URL: Issues, https://github.com/zhaowcheng/xbot/issues
+Project-URL: Homepage, https://github.com/zhaowcheng/xbot.framework
+Project-URL: Issues, https://github.com/zhaowcheng/xbot.framework/issues
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -142,52 +142,53 @@
       - testcases/examples/nonpass/
 
 
 执行测试(测试工程目录下执行命令):
 
 .. code:: console
 
-    $ xbot run -b ./testbeds/testbed_example.yml -s testsets/testset_example.yml           
+    $ xbot run -b testbeds/testbed_example.yml -s testsets/testset_example.yml 
     (1/11)   PASS     0:00:01  tc_eg_pass_get_values_from_testbed
-    (4/11)   ERROR    0:00:00  tc_eg_nonpass_error_syntaxith_failfast_false
-    (3/11)   ERROR    0:00:00  tc_eg_nonpass_error_clsnamefiles
-    (5/11)   RUNNING  0:00:00  tc_eg_nonpass_fail_setup_with_failfast_false
+    (2/11)   PASS     0:00:01  tc_eg_pass_create_dirs_and_files
+    (3/11)   ERROR    0:00:00  tc_eg_nonpass_error_clsname
+    (4/11)   ERROR    0:00:00  tc_eg_nonpass_error_syntax
     (5/11)   FAIL     0:00:01  tc_eg_nonpass_fail_setup_with_failfast_false
     (6/11)   FAIL     0:00:01  tc_eg_nonpass_fail_setup_with_failfast_true
     (7/11)   FAIL     0:00:01  tc_eg_nonpass_fail_step_with_failfast_false
     (8/11)   FAIL     0:00:01  tc_eg_nonpass_fail_step_with_failfast_true
     (9/11)   SKIP     0:00:00  tc_eg_nonpass_skip_excluded
     (10/11)  SKIP     0:00:00  tc_eg_nonpass_skip_not_included
     (11/11)  TIMEOUT  0:00:03  tc_eg_nonpass_timeout
+    
+    report: /Users/wan/CodeProjects/xbot.framework/testproj/logs/testbed_example/2024-06-03_16-48-37/report.html 
 
-    report: /Users/wan/CodeProjects/xbot/testproj/logs/testbed_example/2024-05-29_16-51-09/report.html
 
 执行完成后会在测试工程下根据测试床名称和时间戳生成日志目录保存 html 格式的用例日志和测试报告。
 
 测试报告:
 
-.. image:: https://github.com/zhaowcheng/xbot/blob/v0.1.0/xbot/statics/report_example.png?raw=True
+.. image:: https://github.com/zhaowcheng/xbot.framework/blob/v0.2.0/xbot/framework/statics/report_example.png?raw=True
 
 用例日志:
 
-.. image:: https://github.com/zhaowcheng/xbot/blob/v0.1.0/xbot/statics/log_example.png?raw=True
+.. image:: https://github.com/zhaowcheng/xbot.framework/blob/v0.2.0/xbot/framework/statics/log_example.png?raw=True
 
 
 用例开发
 ---------
 
 测试用例存放在工程目录的 ``testcases`` 子目录下，以下为 ``testcases/examples/pass/tc_eg_pass_create_dirs_and_files.py`` 用例内容:
 
 .. code:: python
 
     import os
     import tempfile
     import shutil
 
-    from xbot.utils import assertx
+    from xbot.framework.utils import assertx
 
     from lib.testcase import TestCase
 
 
     class tc_eg_pass_create_dirs_and_files(TestCase):
         """
         测试创建目录和文件。
@@ -246,7 +247,8 @@
 
 
 测试库开发
 -----------
 
 测试库存放在工程目录的 ``lib`` 子目录下，根据业务开发所需测试库放入该目录下，然后在测试用例中导入使用即可。
 
+
```

### Comparing `xbot.framework-0.1.0/LICENSE` & `xbot.framework-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xbot.framework-0.1.0/tests/test_utils.py` & `xbot.framework-0.2.0/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import sys
 import os
 sys.path.append(os.path.abspath(f'{__file__}/../..'))
 
 from io import StringIO
 from unittest.mock import patch
 
-from xbot import utils
+from xbot.framework import utils
 
 
 def load_tests(loader, tests, ignore):
     tests.addTests(doctest.DocTestSuite(utils))
     return tests
```

### Comparing `xbot.framework-0.1.0/tests/test_report.py` & `xbot.framework-0.2.0/tests/test_report.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import unittest
 
-from xbot.report import gen_report
+from xbot.framework.report import gen_report
 
 
 LOGDIR = os.path.join(os.path.dirname(__file__), 'resources', 'logs')
 OKREPORT = os.path.join(LOGDIR, 'report.ok.html')
 
 
 class TestReport(unittest.TestCase):
```

### Comparing `xbot.framework-0.1.0/tests/test_testcase.py` & `xbot.framework-0.2.0/tests/test_testcase.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 import logging
 
 from importlib import util
 from io import StringIO
 from datetime import datetime, timedelta
 from unittest.mock import MagicMock
 
-from xbot.testcase import TestCase
-from xbot.testbed import TestBed
-from xbot.testset import TestSet
-from xbot.common import INIT_DIR
-from xbot.logger import ROOT_LOGGER
+from xbot.framework.testcase import TestCase
+from xbot.framework.testbed import TestBed
+from xbot.framework.testset import TestSet
+from xbot.framework.common import INIT_DIR
+from xbot.framework.logger import ROOT_LOGGER
 
 
 class TestTestCase(unittest.TestCase):
     """
     测试 “测试用例基类”。
     """
     @classmethod
```

### Comparing `xbot.framework-0.1.0/tests/test_runner.py` & `xbot.framework-0.2.0/tests/test_runner.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 import tempfile
 import shutil
 import logging
 
 from io import StringIO
 from unittest.mock import patch
 
-from xbot import utils
-from xbot.testbed import TestBed
-from xbot.testset import TestSet
-from xbot.runner import Runner
-from xbot.common import INIT_DIR
-from xbot.logger import ROOT_LOGGER
+from xbot.framework import utils
+from xbot.framework.testbed import TestBed
+from xbot.framework.testset import TestSet
+from xbot.framework.runner import Runner
+from xbot.framework.common import INIT_DIR
+from xbot.framework.logger import ROOT_LOGGER
 
 
 class TestRunner(unittest.TestCase):
     """
     测试 runner 模块。
     """
     @classmethod
```

### Comparing `xbot.framework-0.1.0/tests/test_testset.py` & `xbot.framework-0.2.0/tests/test_testset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import unittest
 import tempfile
 import shutil
 
 from unittest.mock import patch, mock_open
 
-from xbot.testset import TestSet, TestSetError
+from xbot.framework.testset import TestSet, TestSetError
 
 class TestTestSet(unittest.TestCase):
     """
     测试套单元测试。
     """
     @classmethod
     def setUpClass(cls):
```

### Comparing `xbot.framework-0.1.0/tests/test_testbed.py` & `xbot.framework-0.2.0/tests/test_testbed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import unittest
 
 from unittest.mock import patch, mock_open
 
-from xbot.testbed import TestBed
+from xbot.framework.testbed import TestBed
 
 class TestTestBed(unittest.TestCase):
     """
     测试床单元测试。
     """
     @classmethod
     def setUpClass(cls):
```

### Comparing `xbot.framework-0.1.0/tests/test_main.py` & `xbot.framework-0.2.0/tests/test_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 import shutil
 import filecmp
 import logging
 
 from io import StringIO
 from unittest.mock import patch, MagicMock
 
-from xbot import main, utils
-from xbot.common import INIT_DIR
-from xbot.logger import ROOT_LOGGER
-from xbot.version import __version__
+from xbot.framework import main, utils
+from xbot.framework.common import INIT_DIR
+from xbot.framework.logger import ROOT_LOGGER
+from xbot.framework.version import __version__
 
 
 class TestMain(unittest.TestCase):
     """
     测试 main 模块。
     """
     @classmethod
@@ -86,19 +86,19 @@
                     self.assertEqual(cm.exception.code, 1)
                     self.assertIn('Generating report...', mockout.getvalue())
                     report = re.search(r'Generating report...\s+(\S+report.html)', 
                                     mockout.getvalue()).group(1)
                     self.assertTrue(os.path.exists(report))
 
     def test_main(self):
-        with patch('xbot.main.init', new_callable=MagicMock) as mockinit:
+        with patch('xbot.framework.main.init', new_callable=MagicMock) as mockinit:
             sys.argv = ['xbot', 'init', '-d', 'myproj']
             main.main()
             mockinit.assert_called_once_with('myproj')
-        with patch('xbot.main.run', new_callable=MagicMock) as mockrun:
+        with patch('xbot.framework.main.run', new_callable=MagicMock) as mockrun:
             sys.argv = ['xbot', 'run', '-b', 'mytb.yml', '-s', 'myts.yml']
             main.main()
             mockrun.assert_called_once_with('mytb.yml', 'myts.yml', 'brief')
         with patch('sys.stdout', new_callable=StringIO) as mockout:
             sys.argv = ['xbot', '-v']
             with self.assertRaises(SystemExit) as cm:
                 main.main()
```

### Comparing `xbot.framework-0.1.0/tests/test_logger.py` & `xbot.framework-0.2.0/tests/test_logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 import sys
 import os
 sys.path.append(os.path.abspath(f'{__file__}/../..'))
 
 from io import StringIO
 
-from xbot.logger import (XLogger, StdoutFilter, CaseLogFilter, 
+from xbot.framework.logger import (XLogger, StdoutFilter, CaseLogFilter, 
                          CaseLogHandler, ROOT_LOGGER, getlogger)
 
 
 class TestLogger(unittest.TestCase):
     """
     logger 模块单元测试。
     """
```

### Comparing `xbot.framework-0.1.0/setup.py` & `xbot.framework-0.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Copyright (c) 2022-2023, zhaowcheng <zhaowcheng@163.com>
 
 import os
 
-from setuptools import setup, find_packages
+from setuptools import setup, find_packages, find_namespace_packages
 
 
 BASEDIR = os.path.abspath(os.path.dirname(__file__))
 
 
 def find_version():
-    verfile = os.path.join(BASEDIR, 'xbot', 'version.py')
+    verfile = os.path.join(BASEDIR, 'xbot', 'framework', 'version.py')
     with open(verfile, 'r', encoding='utf8') as f:
         for line in f.readlines():
             if line.startswith('__version__'):
                 return line.split('=')[1].strip().strip("'").strip('"')
 
 
 def find_requires():
@@ -21,32 +21,32 @@
     with open(reqfile, 'r', encoding='utf8') as f:
         return [r.strip() for r in f.readlines()]
     
 
 def find_long_description():
     with open('README.rst', encoding='utf8') as f:
         desc = f.read()
-        desc = desc.replace('github.com/zhaowcheng/xbot/blob/master',
-                            f'github.com/zhaowcheng/xbot/blob/v{find_version()}')
+        desc = desc.replace('github.com/zhaowcheng/xbot.framework/blob/master',
+                            f'github.com/zhaowcheng/xbot.framework/blob/v{find_version()}')
         return desc
 
 
 setup(
     name='xbot.framework',
     version=find_version(),
     description='A lightweight, easy-to-use, and extensible automation testing framework.',
     long_description=find_long_description(),
     long_description_content_type='text/x-rst',
     author='zhaowcheng',
     author_email='zhaowcheng@163.com',
     install_requires=find_requires(),
-    packages=find_packages(),
+    packages=find_namespace_packages(),
     entry_points={
         'console_scripts': [
-            'xbot = xbot.main:main'
+            'xbot = xbot.framework.main:main'
         ]
     },
     include_package_data=True,
     classifiers=[
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
@@ -54,14 +54,14 @@
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12"
     ],
-    url='https://github.com/zhaowcheng/xbot',
+    url='https://github.com/zhaowcheng/xbot.framework',
     python_requires='>=3.6',
     project_urls={
-        'Homepage': 'https://github.com/zhaowcheng/xbot',
-        'Issues': 'https://github.com/zhaowcheng/xbot/issues'
+        'Homepage': 'https://github.com/zhaowcheng/xbot.framework',
+        'Issues': 'https://github.com/zhaowcheng/xbot.framework/issues'
     }
 )
```

### Comparing `xbot.framework-0.1.0/xbot/runner.py` & `xbot.framework-0.2.0/xbot/framework/runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 import sys
 
 from importlib import import_module
 from datetime import datetime
 from threading import Thread
 from time import sleep
 
-from xbot.logger import getlogger, enable_console_logging
-from xbot.testbed import TestBed
-from xbot.testset import TestSet
-from xbot.testcase import TestCase, ErrorTestCase
-from xbot.utils import xprint
+from xbot.framework.logger import getlogger, enable_console_logging
+from xbot.framework.testbed import TestBed
+from xbot.framework.testset import TestSet
+from xbot.framework.testcase import TestCase, ErrorTestCase
+from xbot.framework.utils import xprint
 
 sys.path.insert(0, '.')
 
-logger = getlogger('runner')
+logger = getlogger(__name__)
 
 
 class Runner(object):
     """
     执行器。
     """
     def __init__(self, testbed: TestBed, testset: TestSet):
```

### Comparing `xbot.framework-0.1.0/xbot/statics/initdir/testcases/examples/pass/tc_eg_pass_get_values_from_testbed.py` & `xbot.framework-0.2.0/xbot/framework/statics/initdir/testcases/examples/pass/tc_eg_pass_get_values_from_testbed.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xbot.utils import assertx
+from xbot.framework.utils import assertx
 
 from lib.testcase import TestCase
 
 
 # 类名将被作为用例编号，且应与文件名保持一致。
 class tc_eg_pass_get_values_from_testbed(TestCase):
     """
```

### Comparing `xbot.framework-0.1.0/xbot/statics/initdir/testcases/examples/pass/tc_eg_pass_create_dirs_and_files.py` & `xbot.framework-0.2.0/xbot/framework/statics/initdir/testcases/examples/pass/tc_eg_pass_create_dirs_and_files.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import tempfile
 import shutil
 
-from xbot.utils import assertx
+from xbot.framework.utils import assertx
 
 from lib.testcase import TestCase
 
 
 class tc_eg_pass_create_dirs_and_files(TestCase):
     """
     测试创建目录和文件。
```

### Comparing `xbot.framework-0.1.0/xbot/statics/initdir/testcases/examples/nonpass/tc_eg_nonpass_skip_not_included.py` & `xbot.framework-0.2.0/xbot/framework/statics/initdir/testcases/examples/nonpass/tc_eg_nonpass_error_syntax.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-from xbot.utils import assertx
+from xbot.framework.utils import assertx
 
 from lib.testcase import TestCase
 
 
-class tc_eg_nonpass_skip_not_included(TestCase):
+class tc_eg_nonpass_error_syntax(TestCase):
     """
-    因不被 testset.tags.include 包含而跳过的测试用例。
+    存在语法错误的用例。
     """
     TIMEOUT = 60
-    FAILFAST = True
-    TAGS = []
+    FAILFAST = False
+    TAGS = ['tag1']
 
     def setup(self):
         """
         预置步骤。
         """
         self.info('开始执行预置步骤')
 
     def step1(self):
         """
         测试步骤 1。
         """
-        self.info('开始执行测试步骤 1')
+        # noinspection PyUnreachableCode
+        self.info('开始执行测试步骤 1'  # type: ignore
 
     def teardown(self):
         """
         清理步骤。
         """
         self.info('开始执行清理步骤')
```

### Comparing `xbot.framework-0.1.0/xbot/statics/initdir/testcases/examples/nonpass/tc_eg_nonpass_error_syntax.py` & `xbot.framework-0.2.0/xbot/framework/statics/initdir/testcases/examples/nonpass/tc_eg_nonpass_skip_excluded.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-from xbot.utils import assertx
+from xbot.framework.utils import assertx
 
 from lib.testcase import TestCase
 
 
-class tc_eg_nonpass_error_syntax(TestCase):
+class tc_eg_nonpass_skip_excluded(TestCase):
     """
-    存在语法错误的用例。
+    因被 testset.tags.exclude 包含而跳过的测试用例。
     """
     TIMEOUT = 60
-    FAILFAST = False
-    TAGS = ['tag1']
+    FAILFAST = True
+    TAGS = ['tag1', 'tag2']
 
     def setup(self):
         """
         预置步骤。
         """
         self.info('开始执行预置步骤')
 
     def step1(self):
         """
         测试步骤 1。
         """
-        # noinspection PyUnreachableCode
-        self.info('开始执行测试步骤 1'  # type: ignore
+        self.info('开始执行测试步骤 1')
 
     def teardown(self):
         """
         清理步骤。
         """
         self.info('开始执行清理步骤')
```

### Comparing `xbot.framework-0.1.0/xbot/statics/initdir/testcases/examples/nonpass/tc_eg_nonpass_fail_setup_with_failfast_false.py` & `xbot.framework-0.2.0/xbot/framework/statics/initdir/testcases/examples/nonpass/tc_eg_nonpass_fail_setup_with_failfast_false.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xbot.utils import assertx
+from xbot.framework.utils import assertx
 
 from lib.testcase import TestCase
 
 
 class tc_eg_nonpass_fail_setup_with_failfast_false(TestCase):
     """
     在 FAILFAST 为 False 的情况下预置步骤失败。
```

### Comparing `xbot.framework-0.1.0/xbot/statics/initdir/testcases/examples/nonpass/tc_eg_nonpass_fail_step_with_failfast_false.py` & `xbot.framework-0.2.0/xbot/framework/statics/initdir/testcases/examples/nonpass/tc_eg_nonpass_fail_step_with_failfast_false.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xbot.utils import assertx
+from xbot.framework.utils import assertx
 
 from lib.testcase import TestCase
 
 
 class tc_eg_nonpass_fail_step_with_failfast_false(TestCase):
     """
     在 FAILFAST 为 False 的情况下测试步骤失败。
```

### Comparing `xbot.framework-0.1.0/xbot/statics/initdir/testcases/examples/nonpass/tc_eg_nonpass_timeout.py` & `xbot.framework-0.2.0/xbot/framework/statics/initdir/testcases/examples/nonpass/tc_eg_nonpass_timeout.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xbot.utils import assertx
+from xbot.framework.utils import assertx
 
 from lib.testcase import TestCase
 
 
 class tc_eg_nonpass_timeout(TestCase):
     """
     超时的测试用例。
```

### Comparing `xbot.framework-0.1.0/xbot/statics/initdir/testcases/examples/nonpass/tc_eg_nonpass_fail_step_with_failfast_true.py` & `xbot.framework-0.2.0/xbot/framework/statics/initdir/testcases/examples/nonpass/tc_eg_nonpass_fail_step_with_failfast_true.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xbot.utils import assertx
+from xbot.framework.utils import assertx
 
 from lib.testcase import TestCase
 
 
 class tc_eg_nonpass_fail_step_with_failfast_true(TestCase):
     """
     在 FAILFAST 为 True 的情况下测试步骤失败。
```

### Comparing `xbot.framework-0.1.0/xbot/statics/initdir/testcases/examples/nonpass/tc_eg_nonpass_error_clsname.py` & `xbot.framework-0.2.0/xbot/framework/statics/initdir/testcases/examples/nonpass/tc_eg_nonpass_error_clsname.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xbot.utils import assertx
+from xbot.framework.utils import assertx
 
 from lib.testcase import TestCase
 
 
 class tc_eg_nonpass_class_name_incorrect(TestCase):
     """
     类名错误（与文件名不一致）的用例。
```

### Comparing `xbot.framework-0.1.0/xbot/statics/initdir/testcases/examples/nonpass/tc_eg_nonpass_fail_setup_with_failfast_true.py` & `xbot.framework-0.2.0/testproj/testcases/examples/nonpass/tc_eg_nonpass_fail_setup_with_failfast_false.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from xbot.utils import assertx
+from xbot.framework.utils import assertx
 
 from lib.testcase import TestCase
 
 
-class tc_eg_nonpass_fail_setup_with_failfast_true(TestCase):
+class tc_eg_nonpass_fail_setup_with_failfast_false(TestCase):
     """
-    在 FAILFAST 为 True 的情况下预置步骤失败。
+    在 FAILFAST 为 False 的情况下预置步骤失败。
     """
     TIMEOUT = 60
-    FAILFAST = True
+    FAILFAST = False
     TAGS = ['tag1']
 
     def setup(self):
         """
         断言 1 == 0。
         """
         # setup 出现失败，无论 FAILFAST 是何值，
```

### Comparing `xbot.framework-0.1.0/xbot/statics/initdir/testcases/examples/nonpass/tc_eg_nonpass_skip_excluded.py` & `xbot.framework-0.2.0/testproj/testcases/examples/nonpass/tc_eg_nonpass_skip_excluded.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xbot.utils import assertx
+from xbot.framework.utils import assertx
 
 from lib.testcase import TestCase
 
 
 class tc_eg_nonpass_skip_excluded(TestCase):
     """
     因被 testset.tags.exclude 包含而跳过的测试用例。
```

### Comparing `xbot.framework-0.1.0/xbot/statics/.DS_Store` & `xbot.framework-0.2.0/xbot/framework/statics/.DS_Store`

 * *Files identical despite different names*

### Comparing `xbot.framework-0.1.0/xbot/statics/log_template.html` & `xbot.framework-0.2.0/xbot/framework/statics/log_template.html`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
                     </tr>
                     {% for record in records %}
                     <tr class="{{record.levelname}}">
                         <td>{{record.asctime}}</td>
                         <td>{{record.levelname}}</td>
                         <td style="word-wrap: break-word;">{{record.filename}}:{{record.lineno}}</td>
                         <td style="padding-left: 0.5%;">
-                            <pre>{{record.msg.replace('<','&lt').replace('>','&gt')}}{% if 'hook' in record and 'more' in record.hook %}  <a id="a{{record.asctime}}" href="javascript:switchElementDisplayState('{{record.asctime}}');switchMoreOrLess('a{{record.asctime}}')">@more</a>{% endif %}</pre>
+                            <pre>{{record.message.replace('<','&lt').replace('>','&gt')}}{% if 'hook' in record and 'more' in record.hook %}  <a id="a{{record.asctime}}" href="javascript:switchElementDisplayState('{{record.asctime}}');switchMoreOrLess('a{{record.asctime}}')">@more</a>{% endif %}</pre>
                             {% if 'hook' in record and 'more' in record.hook %}
                             <pre id='{{record.asctime}}'
                                 style="display: none;font-family: monospace;">{{record.hook.more.replace('<','&lt').replace('>','&gt')}}</pre>
                             {% endif %}
                         </td>
                     </tr>
                     {% endfor %}
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 ?执?行?结?果 {{result}}
 ?开?始?时?间 {{starttime}} {{sourcecode}} {{testbed}}
 ?结?束?时?间 {{endtime}}
 ?执?行?时?长 {{duration}}
 {% for stage, records in stage_records.items() %}
 {{stage}}
 ttiimmee              lleevveell               llooccaattiioonn            mmeessssaaggee
-                                                          {{record.msg.replace
+                                                          {{record.message.replace
                                                           ('<','<').replace
                                                           ('>','>')}}{% if 'hook'
                                                           in record and 'more' in
                                                           record.hook %}  _@_m_o_r_e{%
                                       {                   endif %}
 {                 {                   {record.filename}}: {% if 'hook' in record
 {record.asctime}} {record.levelname}} {{record.lineno}}   and 'more' in record.hook
```

### Comparing `xbot.framework-0.1.0/xbot/statics/report_template.html` & `xbot.framework-0.2.0/xbot/framework/statics/report_template.html`

 * *Files identical despite different names*

### Comparing `xbot.framework-0.1.0/xbot/testcase.py` & `xbot.framework-0.2.0/xbot/framework/testcase.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 import sys
 import logging
 import traceback
 import re
 import time
 import inspect
 
-from typing import Any, List
+from typing import List
 from datetime import datetime, timedelta
 from importlib import import_module
 from threading import Thread
 
-from xbot import logger, common, utils
-from xbot.testbed import TestBed
-from xbot.testset import TestSet
-from xbot.errors import TestCaseTimeout, TestCaseError
+from xbot.framework import logger, common, utils
+from xbot.framework.testbed import TestBed
+from xbot.framework.testset import TestSet
+from xbot.framework.errors import TestCaseTimeout, TestCaseError
 
 
 class TestCase(object):
     """
     用例基类。
     """
     # 最大执行时长（单位：秒），超过该时长将会被强制结束。
@@ -45,14 +45,15 @@
         self.__starttime = None
         self.__endtime = None
         self.__duration = None
         self.__result = None
         self.__logger = logger.getlogger(self.caseid)
         self.__loghdlr = logger.CaseLogHandler(logging.DEBUG)
         self.__loghdlr.addFilter(logger.CaseLogFilter(self.caseid))
+        self.__loghdlr.setFormatter(logger.FORMATTER)
         logger.ROOT_LOGGER.addHandler(self.__loghdlr)
 
     @property
     def testbed(self) -> TestBed:
         """
         测试床实例。
         """
```

### Comparing `xbot.framework-0.1.0/xbot/logger.py` & `xbot.framework-0.2.0/xbot/framework/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -106,37 +106,46 @@
         self.stage = stage
         if self.stage not in self.records:
             self.records[self.stage] = []
 
     def emit(self, record):
         if self.stage not in self.records:
             self.records[self.stage] = []
-        record.msg = record.getMessage()
+        self.format(record)
         self.records[self.stage].append(record.__dict__)
 
 
+class ExtraAdapter(logging.LoggerAdapter):
+    """
+    日志消息包含额外信息（前缀）。
+    """
+    def process(self, msg, kwargs):
+        msg = '[{}] {}'.format(self.extra, msg) if self.extra else msg
+        return msg, kwargs
+
+
 ROOT_LOGGER = logging.getLogger('xbot')
 ROOT_LOGGER.setLevel('DEBUG')
+FORMATTER = logging.Formatter(
+    '[%(asctime)s] [%(levelname)s] [%(filename)s:%(lineno)s] %(message)s'
+)
 
 
 def enable_console_logging() -> None:
     """
     开启控制台日志输出。
     """
     if 'console_logging_enabled' in globals():
         return
     stdout = logging.StreamHandler(sys.stdout)
     stdout.addFilter(StdoutFilter())
     stderr = logging.StreamHandler(sys.stderr)
     stderr.setLevel('ERROR')
-    formater = logging.Formatter(
-        '[%(asctime)s] [%(levelname)s] [%(filename)s:%(lineno)s] %(message)s'
-    )
-    stdout.setFormatter(formater)
-    stderr.setFormatter(formater)
+    stdout.setFormatter(FORMATTER)
+    stderr.setFormatter(FORMATTER)
     ROOT_LOGGER.addHandler(stdout)
     ROOT_LOGGER.addHandler(stderr)
     global console_logging_enabled
     console_logging_enabled = True
 
 
 def getlogger(name) -> XLogger:
```

### Comparing `xbot.framework-0.1.0/xbot/testset.py` & `xbot.framework-0.2.0/xbot/framework/testset.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 """
 
 import os
 
 from ruamel import yaml
 from copy import deepcopy
 
-from xbot.utils import ordered_walk
-from xbot.errors import TestSetError
+from xbot.framework.utils import ordered_walk
+from xbot.framework.errors import TestSetError
 
 
 class TestSet(object):
     """
     测试套类。
     """
     def __init__(self, filepath: str):
```

### Comparing `xbot.framework-0.1.0/xbot/testbed.py` & `xbot.framework-0.2.0/xbot/framework/testbed.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 
 import os
 
 from typing import Any
 
 from ruamel import yaml
-from xbot.utils import deepget
+from xbot.framework.utils import deepget
 
 
 class TestBed(object):
     """
     测试床类。
     """
     def __init__(self, filepath: str):
```

### Comparing `xbot.framework-0.1.0/xbot/utils.py` & `xbot.framework-0.2.0/xbot/framework/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 
 import jinja2
 
 from typing import Any, Iterator, Tuple, List
 from functools import reduce, partial
 from contextlib import contextmanager
 
-from xbot.logger import getlogger
+from xbot.framework.logger import getlogger
 
 
-logger = getlogger('util')
+logger = getlogger(__name__)
 
 
 class ColorText(object):
     """
     给终端字符添加 ascii 颜色码。
     """
```

### Comparing `xbot.framework-0.1.0/xbot/main.py` & `xbot.framework-0.2.0/xbot/framework/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 import os
 import sys
 import shutil
 import argparse
 
 from importlib import import_module
 
-from xbot.version import __version__
-from xbot.testset import TestSet
-from xbot.runner import Runner
-from xbot.report import gen_report
-from xbot.utils import printerr, xprint
-from xbot.common import INIT_DIR
+from xbot.framework.version import __version__
+from xbot.framework.testset import TestSet
+from xbot.framework.runner import Runner
+from xbot.framework.report import gen_report
+from xbot.framework.utils import printerr, xprint
+from xbot.framework.common import INIT_DIR
 
 
 def create_parser() -> argparse.ArgumentParser:
     """
     创建命令行参数解析器。
     """
     parser = argparse.ArgumentParser(prog='xbot')
```

### Comparing `xbot.framework-0.1.0/xbot/report.py` & `xbot.framework-0.2.0/xbot/framework/report.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 import os
 import re
 
 from typing import Tuple
 from datetime import datetime
 
-from xbot import utils
-from xbot import common
+from xbot.framework import utils
+from xbot.framework import common
 
 
 def find_value(html: str, id_: str) -> str:
     """
     通过 id 获取 html 元素的文本。
 
     :param html: html 内容。
```

### Comparing `xbot.framework-0.1.0/README.rst` & `xbot.framework-0.2.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -117,52 +117,53 @@
       - testcases/examples/nonpass/
 
 
 执行测试(测试工程目录下执行命令):
 
 .. code:: console
 
-    $ xbot run -b ./testbeds/testbed_example.yml -s testsets/testset_example.yml           
+    $ xbot run -b testbeds/testbed_example.yml -s testsets/testset_example.yml 
     (1/11)   PASS     0:00:01  tc_eg_pass_get_values_from_testbed
-    (4/11)   ERROR    0:00:00  tc_eg_nonpass_error_syntaxith_failfast_false
-    (3/11)   ERROR    0:00:00  tc_eg_nonpass_error_clsnamefiles
-    (5/11)   RUNNING  0:00:00  tc_eg_nonpass_fail_setup_with_failfast_false
+    (2/11)   PASS     0:00:01  tc_eg_pass_create_dirs_and_files
+    (3/11)   ERROR    0:00:00  tc_eg_nonpass_error_clsname
+    (4/11)   ERROR    0:00:00  tc_eg_nonpass_error_syntax
     (5/11)   FAIL     0:00:01  tc_eg_nonpass_fail_setup_with_failfast_false
     (6/11)   FAIL     0:00:01  tc_eg_nonpass_fail_setup_with_failfast_true
     (7/11)   FAIL     0:00:01  tc_eg_nonpass_fail_step_with_failfast_false
     (8/11)   FAIL     0:00:01  tc_eg_nonpass_fail_step_with_failfast_true
     (9/11)   SKIP     0:00:00  tc_eg_nonpass_skip_excluded
     (10/11)  SKIP     0:00:00  tc_eg_nonpass_skip_not_included
     (11/11)  TIMEOUT  0:00:03  tc_eg_nonpass_timeout
+    
+    report: /Users/wan/CodeProjects/xbot.framework/testproj/logs/testbed_example/2024-06-03_16-48-37/report.html 
 
-    report: /Users/wan/CodeProjects/xbot/testproj/logs/testbed_example/2024-05-29_16-51-09/report.html
 
 执行完成后会在测试工程下根据测试床名称和时间戳生成日志目录保存 html 格式的用例日志和测试报告。
 
 测试报告:
 
-.. image:: https://github.com/zhaowcheng/xbot/blob/master/xbot/statics/report_example.png?raw=True
+.. image:: https://github.com/zhaowcheng/xbot.framework/blob/master/xbot/framework/statics/report_example.png?raw=True
 
 用例日志:
 
-.. image:: https://github.com/zhaowcheng/xbot/blob/master/xbot/statics/log_example.png?raw=True
+.. image:: https://github.com/zhaowcheng/xbot.framework/blob/master/xbot/framework/statics/log_example.png?raw=True
 
 
 用例开发
 ---------
 
 测试用例存放在工程目录的 ``testcases`` 子目录下，以下为 ``testcases/examples/pass/tc_eg_pass_create_dirs_and_files.py`` 用例内容:
 
 .. code:: python
 
     import os
     import tempfile
     import shutil
 
-    from xbot.utils import assertx
+    from xbot.framework.utils import assertx
 
     from lib.testcase import TestCase
 
 
     class tc_eg_pass_create_dirs_and_files(TestCase):
         """
         测试创建目录和文件。
@@ -219,8 +220,8 @@
 - ``FAILFAST`` 属性为 *True* 时，当某个测试步骤失败时，则会跳过后续测试步骤立即执行清理步骤；
 - ``TAGS`` 属性定义用例 *标签*，可用于测试套中对待执行测试用例列表进行筛选；
 
 
 测试库开发
 -----------
 
-测试库存放在工程目录的 ``lib`` 子目录下，根据业务开发所需测试库放入该目录下，然后在测试用例中导入使用即可。
+测试库存放在工程目录的 ``lib`` 子目录下，根据业务开发所需测试库放入该目录下，然后在测试用例中导入使用即可。
```

### Comparing `xbot.framework-0.1.0/xbot.framework.egg-info/PKG-INFO` & `xbot.framework-0.2.0/xbot.framework.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: xbot.framework
-Version: 0.1.0
+Version: 0.2.0
 Summary: A lightweight, easy-to-use, and extensible automation testing framework.
-Home-page: https://github.com/zhaowcheng/xbot
+Home-page: https://github.com/zhaowcheng/xbot.framework
 Author: zhaowcheng
 Author-email: zhaowcheng@163.com
 License: UNKNOWN
-Project-URL: Homepage, https://github.com/zhaowcheng/xbot
-Project-URL: Issues, https://github.com/zhaowcheng/xbot/issues
+Project-URL: Homepage, https://github.com/zhaowcheng/xbot.framework
+Project-URL: Issues, https://github.com/zhaowcheng/xbot.framework/issues
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -142,52 +142,53 @@
       - testcases/examples/nonpass/
 
 
 执行测试(测试工程目录下执行命令):
 
 .. code:: console
 
-    $ xbot run -b ./testbeds/testbed_example.yml -s testsets/testset_example.yml           
+    $ xbot run -b testbeds/testbed_example.yml -s testsets/testset_example.yml 
     (1/11)   PASS     0:00:01  tc_eg_pass_get_values_from_testbed
-    (4/11)   ERROR    0:00:00  tc_eg_nonpass_error_syntaxith_failfast_false
-    (3/11)   ERROR    0:00:00  tc_eg_nonpass_error_clsnamefiles
-    (5/11)   RUNNING  0:00:00  tc_eg_nonpass_fail_setup_with_failfast_false
+    (2/11)   PASS     0:00:01  tc_eg_pass_create_dirs_and_files
+    (3/11)   ERROR    0:00:00  tc_eg_nonpass_error_clsname
+    (4/11)   ERROR    0:00:00  tc_eg_nonpass_error_syntax
     (5/11)   FAIL     0:00:01  tc_eg_nonpass_fail_setup_with_failfast_false
     (6/11)   FAIL     0:00:01  tc_eg_nonpass_fail_setup_with_failfast_true
     (7/11)   FAIL     0:00:01  tc_eg_nonpass_fail_step_with_failfast_false
     (8/11)   FAIL     0:00:01  tc_eg_nonpass_fail_step_with_failfast_true
     (9/11)   SKIP     0:00:00  tc_eg_nonpass_skip_excluded
     (10/11)  SKIP     0:00:00  tc_eg_nonpass_skip_not_included
     (11/11)  TIMEOUT  0:00:03  tc_eg_nonpass_timeout
+    
+    report: /Users/wan/CodeProjects/xbot.framework/testproj/logs/testbed_example/2024-06-03_16-48-37/report.html 
 
-    report: /Users/wan/CodeProjects/xbot/testproj/logs/testbed_example/2024-05-29_16-51-09/report.html
 
 执行完成后会在测试工程下根据测试床名称和时间戳生成日志目录保存 html 格式的用例日志和测试报告。
 
 测试报告:
 
-.. image:: https://github.com/zhaowcheng/xbot/blob/v0.1.0/xbot/statics/report_example.png?raw=True
+.. image:: https://github.com/zhaowcheng/xbot.framework/blob/v0.2.0/xbot/framework/statics/report_example.png?raw=True
 
 用例日志:
 
-.. image:: https://github.com/zhaowcheng/xbot/blob/v0.1.0/xbot/statics/log_example.png?raw=True
+.. image:: https://github.com/zhaowcheng/xbot.framework/blob/v0.2.0/xbot/framework/statics/log_example.png?raw=True
 
 
 用例开发
 ---------
 
 测试用例存放在工程目录的 ``testcases`` 子目录下，以下为 ``testcases/examples/pass/tc_eg_pass_create_dirs_and_files.py`` 用例内容:
 
 .. code:: python
 
     import os
     import tempfile
     import shutil
 
-    from xbot.utils import assertx
+    from xbot.framework.utils import assertx
 
     from lib.testcase import TestCase
 
 
     class tc_eg_pass_create_dirs_and_files(TestCase):
         """
         测试创建目录和文件。
@@ -246,7 +247,8 @@
 
 
 测试库开发
 -----------
 
 测试库存放在工程目录的 ``lib`` 子目录下，根据业务开发所需测试库放入该目录下，然后在测试用例中导入使用即可。
 
+
```

