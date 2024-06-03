# Comparing `tmp/cellpy-1.0.1b5.tar.gz` & `tmp/cellpy-1.0.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellpy-1.0.1b5.tar", last modified: Thu Mar  7 14:24:51 2024, max compression
+gzip compressed data, was "cellpy-1.0.2a1.tar", last modified: Mon Jun  3 08:28:32 2024, max compression
```

## Comparing `cellpy-1.0.1b5.tar` & `cellpy-1.0.2a1.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxrwxrwx   0        0        0        0 2024-03-07 14:24:51.418329 cellpy-1.0.1b5/
--rw-rw-rw-   0        0        0      459 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/AUTHORS.md
--rw-rw-rw-   0        0        0     3406 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/CONTRIBUTING.md
--rw-rw-rw-   0        0        0     5515 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/HISTORY.md
--rw-rw-rw-   0        0        0     1087 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/LICENSE.md
--rw-rw-rw-   0        0        0      521 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/MANIFEST.in
--rw-rw-rw-   0        0        0     9199 2024-03-07 14:24:51.417329 cellpy-1.0.1b5/PKG-INFO
--rw-rw-rw-   0        0        0     1798 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/README.md
-drwxrwxrwx   0        0        0        0 2024-03-07 14:24:51.230387 cellpy-1.0.1b5/cellpy/
--rw-rw-rw-   0        0        0     1163 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/cellpy/__init__.py
--rw-rw-rw-   0        0        0       25 2024-03-07 14:24:27.000000 cellpy-1.0.1b5/cellpy/_version.py
--rw-rw-rw-   0        0        0    63696 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/cellpy/cli.py
--rw-rw-rw-   0        0        0     1228 2024-02-18 15:23:05.000000 cellpy-1.0.1b5/cellpy/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-03-07 14:24:51.250306 cellpy-1.0.1b5/cellpy/internals/
--rw-rw-rw-   0        0        0        0 2024-02-18 15:23:05.000000 cellpy-1.0.1b5/cellpy/internals/__init__.py
--rw-rw-rw-   0        0        0    29493 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/cellpy/internals/core.py
--rw-rw-rw-   0        0        0     4833 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/cellpy/log.py
--rw-rw-rw-   0        0        0     1750 2021-12-21 09:11:58.000000 cellpy-1.0.1b5/cellpy/logging.json
-drwxrwxrwx   0        0        0        0 2024-03-07 14:24:51.260813 cellpy-1.0.1b5/cellpy/parameters/
--rw-rw-rw-   0        0        0     3513 2024-02-18 15:23:05.000000 cellpy-1.0.1b5/cellpy/parameters/.cellpy_prms_default.conf
--rw-rw-rw-   0        0        0        2 2024-02-18 15:23:05.000000 cellpy-1.0.1b5/cellpy/parameters/__init__.py
--rw-rw-rw-   0        0        0    24966 2024-03-07 14:13:43.000000 cellpy-1.0.1b5/cellpy/parameters/internal_settings.py
-drwxrwxrwx   0        0        0        0 2024-03-07 14:24:51.264812 cellpy-1.0.1b5/cellpy/parameters/legacy/
--rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.1b5/cellpy/parameters/legacy/__init__.py
--rw-rw-rw-   0        0        0    24148 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/cellpy/parameters/legacy/update_headers.py
--rw-rw-rw-   0        0        0    14964 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/cellpy/parameters/prmreader.py
--rw-rw-rw-   0        0        0    13581 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/cellpy/parameters/prms.py
-drwxrwxrwx   0        0        0        0 2024-03-07 14:24:51.281331 cellpy-1.0.1b5/cellpy/readers/
--rw-rw-rw-   0        0        0        2 2021-12-21 09:11:58.000000 cellpy-1.0.1b5/cellpy/readers/__init__.py
--rw-rw-rw-   0        0        0   281279 2024-03-07 14:23:42.000000 cellpy-1.0.1b5/cellpy/readers/cellreader.py
--rw-rw-rw-   0        0        0    46853 2024-03-03 20:04:34.000000 cellpy-1.0.1b5/cellpy/readers/core.py
--rw-rw-rw-   0        0        0    23045 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/cellpy/readers/dbreader.py
--rw-rw-rw-   0        0        0      594 2024-02-29 08:50:08.000000 cellpy-1.0.1b5/cellpy/readers/do.py
--rw-rw-rw-   0        0        0    18255 2024-02-29 08:50:08.000000 cellpy-1.0.1b5/cellpy/readers/filefinder.py
-drwxrwxrwx   0        0        0        0 2024-03-07 14:24:51.319329 cellpy-1.0.1b5/cellpy/readers/instruments/
--rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.1b5/cellpy/readers/instruments/__init__.py
--rw-rw-rw-   0        0        0    50060 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/cellpy/readers/instruments/arbin_res.py
--rw-rw-rw-   0        0        0    20270 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/cellpy/readers/instruments/arbin_sql.py
--rw-rw-rw-   0        0        0    21106 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/cellpy/readers/instruments/arbin_sql_7.py
--rw-rw-rw-   0        0        0    11088 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/cellpy/readers/instruments/arbin_sql_csv.py
--rw-rw-rw-   0        0        0     9389 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/cellpy/readers/instruments/arbin_sql_h5.py
--rw-rw-rw-   0        0        0     9921 2024-02-19 12:52:17.000000 cellpy-1.0.1b5/cellpy/readers/instruments/arbin_sql_xlsx.py
--rw-rw-rw-   0        0        0    28999 2024-03-06 08:45:46.000000 cellpy-1.0.1b5/cellpy/readers/instruments/base.py
--rw-rw-rw-   0        0        0    26718 2024-03-07 14:23:42.000000 cellpy-1.0.1b5/cellpy/readers/instruments/biologics_mpr.py
-drwxrwxrwx   0        0        0        0 2024-03-07 14:24:51.332331 cellpy-1.0.1b5/cellpy/readers/instruments/configurations/
--rw-rw-rw-   0        0        0     6631 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/cellpy/readers/instruments/configurations/__init__.py
--rw-rw-rw-   0        0        0     4332 2024-03-03 15:12:15.000000 cellpy-1.0.1b5/cellpy/readers/instruments/configurations/maccor_txt_one.py
--rw-rw-rw-   0        0        0     2020 2024-03-04 20:37:20.000000 cellpy-1.0.1b5/cellpy/readers/instruments/configurations/maccor_txt_three.py
--rw-rw-rw-   0        0        0     1961 2024-03-03 15:12:15.000000 cellpy-1.0.1b5/cellpy/readers/instruments/configurations/maccor_txt_two.py
--rw-rw-rw-   0        0        0     3549 2024-02-18 15:23:05.000000 cellpy-1.0.1b5/cellpy/readers/instruments/configurations/maccor_txt_zero.py
--rw-rw-rw-   0        0        0     2132 2024-02-18 15:23:05.000000 cellpy-1.0.1b5/cellpy/readers/instruments/configurations/neware_txt_zero.py
--rw-rw-rw-   0        0        0    10627 2024-03-06 09:48:13.000000 cellpy-1.0.1b5/cellpy/readers/instruments/custom.py
--rw-rw-rw-   0        0        0     3798 2024-02-19 12:52:17.000000 cellpy-1.0.1b5/cellpy/readers/instruments/ext_nda_reader.py
-drwxrwxrwx   0        0        0        0 2024-03-07 14:24:51.337331 cellpy-1.0.1b5/cellpy/readers/instruments/loader_specific_modules/
--rw-rw-rw-   0        0        0        0 2022-06-03 19:58:41.000000 cellpy-1.0.1b5/cellpy/readers/instruments/loader_specific_modules/__init__.py
--rw-rw-rw-   0        0        0    49457 2024-03-07 14:23:42.000000 cellpy-1.0.1b5/cellpy/readers/instruments/loader_specific_modules/biologic_file_format.py
--rw-rw-rw-   0        0        0     1430 2024-03-06 08:45:46.000000 cellpy-1.0.1b5/cellpy/readers/instruments/local_instrument.py
--rw-rw-rw-   0        0        0    14739 2024-03-03 15:12:15.000000 cellpy-1.0.1b5/cellpy/readers/instruments/maccor_txt.py
--rw-rw-rw-   0        0        0     3519 2024-03-03 20:04:34.000000 cellpy-1.0.1b5/cellpy/readers/instruments/neware_txt.py
--rw-rw-rw-   0        0        0    17041 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/cellpy/readers/instruments/neware_xlsx.py
--rw-rw-rw-   0        0        0    15973 2024-02-29 16:05:35.000000 cellpy-1.0.1b5/cellpy/readers/instruments/pec_csv.py
-drwxrwxrwx   0        0        0        0 2024-03-07 14:24:51.345332 cellpy-1.0.1b5/cellpy/readers/instruments/processors/
--rw-rw-rw-   0        0        0        0 2022-05-27 12:07:50.000000 cellpy-1.0.1b5/cellpy/readers/instruments/processors/__init__.py
--rw-rw-rw-   0        0        0    16213 2024-03-06 08:45:46.000000 cellpy-1.0.1b5/cellpy/readers/instruments/processors/post_processors.py
--rw-rw-rw-   0        0        0     1448 2024-02-28 15:42:14.000000 cellpy-1.0.1b5/cellpy/readers/instruments/processors/pre_processors.py
--rw-rw-rw-   0        0        0    27486 2024-02-29 08:50:08.000000 cellpy-1.0.1b5/cellpy/readers/sql_dbreader.py
-drwxrwxrwx   0        0        0        0 2024-03-07 14:24:51.379329 cellpy-1.0.1b5/cellpy/utils/
--rw-rw-rw-   0        0        0      192 2021-12-21 09:11:58.000000 cellpy-1.0.1b5/cellpy/utils/__init__.py
--rw-rw-rw-   0        0        0    64651 2024-02-28 15:42:14.000000 cellpy-1.0.1b5/cellpy/utils/batch.py
-drwxrwxrwx   0        0        0        0 2024-03-07 14:24:51.411331 cellpy-1.0.1b5/cellpy/utils/batch_tools/
--rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.1b5/cellpy/utils/batch_tools/__init__.py
--rw-rw-rw-   0        0        0     7578 2024-02-18 15:23:05.000000 cellpy-1.0.1b5/cellpy/utils/batch_tools/batch_analyzers.py
--rw-rw-rw-   0        0        0    19592 2024-02-18 15:23:05.000000 cellpy-1.0.1b5/cellpy/utils/batch_tools/batch_core.py
--rw-rw-rw-   0        0        0    42419 2024-02-28 15:42:14.000000 cellpy-1.0.1b5/cellpy/utils/batch_tools/batch_experiments.py
--rw-rw-rw-   0        0        0     2931 2024-02-18 15:23:05.000000 cellpy-1.0.1b5/cellpy/utils/batch_tools/batch_exporters.py
--rw-rw-rw-   0        0        0    14268 2024-02-28 15:42:14.000000 cellpy-1.0.1b5/cellpy/utils/batch_tools/batch_helpers.py
--rw-rw-rw-   0        0        0    28926 2024-02-19 12:52:17.000000 cellpy-1.0.1b5/cellpy/utils/batch_tools/batch_journals.py
--rw-rw-rw-   0        0        0    46212 2024-02-28 15:42:14.000000 cellpy-1.0.1b5/cellpy/utils/batch_tools/batch_plotters.py
--rw-rw-rw-   0        0        0      245 2021-12-21 09:11:58.000000 cellpy-1.0.1b5/cellpy/utils/batch_tools/batch_reporters.py
--rw-rw-rw-   0        0        0     3404 2024-02-18 15:23:05.000000 cellpy-1.0.1b5/cellpy/utils/batch_tools/dumpers.py
--rw-rw-rw-   0        0        0    10200 2024-02-19 12:52:17.000000 cellpy-1.0.1b5/cellpy/utils/batch_tools/engines.py
--rw-rw-rw-   0        0        0     5294 2024-02-18 15:23:05.000000 cellpy-1.0.1b5/cellpy/utils/batch_tools/sqlite_from_excel_db.py
--rw-rw-rw-   0        0        0    82304 2024-03-06 15:48:16.000000 cellpy-1.0.1b5/cellpy/utils/collectors.py
--rw-rw-rw-   0        0        0      260 2022-05-27 12:07:50.000000 cellpy-1.0.1b5/cellpy/utils/diagnostics.py
--rw-rw-rw-   0        0        0    78981 2024-02-28 15:42:14.000000 cellpy-1.0.1b5/cellpy/utils/easyplot.py
--rw-rw-rw-   0        0        0     9123 2024-03-06 08:45:46.000000 cellpy-1.0.1b5/cellpy/utils/example_data.py
--rw-rw-rw-   0        0        0    46313 2024-03-06 15:48:16.000000 cellpy-1.0.1b5/cellpy/utils/helpers.py
--rw-rw-rw-   0        0        0    39839 2024-02-28 15:42:14.000000 cellpy-1.0.1b5/cellpy/utils/ica.py
--rw-rw-rw-   0        0        0      189 2022-05-27 12:07:50.000000 cellpy-1.0.1b5/cellpy/utils/live.py
--rw-rw-rw-   0        0        0    32747 2024-02-18 15:23:05.000000 cellpy-1.0.1b5/cellpy/utils/ocv_rlx.py
--rw-rw-rw-   0        0        0    23825 2024-02-29 16:05:35.000000 cellpy-1.0.1b5/cellpy/utils/plotutils.py
--rw-rw-rw-   0        0        0     1789 2024-02-28 15:42:14.000000 cellpy-1.0.1b5/cellpy/utils/processor.py
-drwxrwxrwx   0        0        0        0 2024-03-07 14:24:51.414330 cellpy-1.0.1b5/cellpy.egg-info/
--rw-rw-rw-   0        0        0     9199 2024-03-07 14:24:51.000000 cellpy-1.0.1b5/cellpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3025 2024-03-07 14:24:51.000000 cellpy-1.0.1b5/cellpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-07 14:24:51.000000 cellpy-1.0.1b5/cellpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-03-07 14:24:51.000000 cellpy-1.0.1b5/cellpy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-03-07 14:24:50.000000 cellpy-1.0.1b5/cellpy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      404 2024-03-07 14:24:51.000000 cellpy-1.0.1b5/cellpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-03-07 14:24:51.000000 cellpy-1.0.1b5/cellpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      367 2024-02-28 15:42:19.000000 cellpy-1.0.1b5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-07 14:24:51.418329 cellpy-1.0.1b5/setup.cfg
--rw-rw-rw-   0        0        0     3150 2024-02-28 15:42:19.000000 cellpy-1.0.1b5/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:28:32.100035 cellpy-1.0.2a1/
+-rw-rw-rw-   0        0        0      459 2024-03-19 10:15:02.000000 cellpy-1.0.2a1/AUTHORS.md
+-rw-rw-rw-   0        0        0     3406 2024-03-19 10:15:02.000000 cellpy-1.0.2a1/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0     5258 2024-04-10 13:09:36.000000 cellpy-1.0.2a1/HISTORY.md
+-rw-rw-rw-   0        0        0     1087 2024-03-19 10:15:02.000000 cellpy-1.0.2a1/LICENSE.md
+-rw-rw-rw-   0        0        0      521 2024-03-19 10:15:02.000000 cellpy-1.0.2a1/MANIFEST.in
+-rw-rw-rw-   0        0        0     8942 2024-06-03 08:28:32.099042 cellpy-1.0.2a1/PKG-INFO
+-rw-rw-rw-   0        0        0     1798 2024-03-19 10:15:02.000000 cellpy-1.0.2a1/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 08:28:31.965961 cellpy-1.0.2a1/cellpy/
+-rw-rw-rw-   0        0        0     1163 2024-03-19 10:15:03.000000 cellpy-1.0.2a1/cellpy/__init__.py
+-rw-rw-rw-   0        0        0       25 2024-04-25 07:55:02.000000 cellpy-1.0.2a1/cellpy/_version.py
+-rw-rw-rw-   0        0        0    63696 2024-03-19 10:15:03.000000 cellpy-1.0.2a1/cellpy/cli.py
+-rw-rw-rw-   0        0        0     1228 2024-02-18 15:23:05.000000 cellpy-1.0.2a1/cellpy/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:28:31.977968 cellpy-1.0.2a1/cellpy/internals/
+-rw-rw-rw-   0        0        0        0 2024-02-18 15:23:05.000000 cellpy-1.0.2a1/cellpy/internals/__init__.py
+-rw-rw-rw-   0        0        0    34109 2024-06-03 08:03:19.000000 cellpy-1.0.2a1/cellpy/internals/core.py
+-rw-rw-rw-   0        0        0     4833 2024-03-19 10:15:03.000000 cellpy-1.0.2a1/cellpy/log.py
+-rw-rw-rw-   0        0        0     1750 2021-12-21 09:11:58.000000 cellpy-1.0.2a1/cellpy/logging.json
+drwxrwxrwx   0        0        0        0 2024-06-03 08:28:31.985961 cellpy-1.0.2a1/cellpy/parameters/
+-rw-rw-rw-   0        0        0     3513 2024-02-18 15:23:05.000000 cellpy-1.0.2a1/cellpy/parameters/.cellpy_prms_default.conf
+-rw-rw-rw-   0        0        0        2 2024-02-18 15:23:05.000000 cellpy-1.0.2a1/cellpy/parameters/__init__.py
+-rw-rw-rw-   0        0        0    24966 2024-03-19 10:15:03.000000 cellpy-1.0.2a1/cellpy/parameters/internal_settings.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:28:31.988961 cellpy-1.0.2a1/cellpy/parameters/legacy/
+-rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.2a1/cellpy/parameters/legacy/__init__.py
+-rw-rw-rw-   0        0        0    24148 2024-03-19 10:15:03.000000 cellpy-1.0.2a1/cellpy/parameters/legacy/update_headers.py
+-rw-rw-rw-   0        0        0    14964 2024-03-19 10:15:03.000000 cellpy-1.0.2a1/cellpy/parameters/prmreader.py
+-rw-rw-rw-   0        0        0    13581 2024-03-19 10:15:03.000000 cellpy-1.0.2a1/cellpy/parameters/prms.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:28:32.001960 cellpy-1.0.2a1/cellpy/readers/
+-rw-rw-rw-   0        0        0        2 2021-12-21 09:11:58.000000 cellpy-1.0.2a1/cellpy/readers/__init__.py
+-rw-rw-rw-   0        0        0   281279 2024-04-25 14:34:51.000000 cellpy-1.0.2a1/cellpy/readers/cellreader.py
+-rw-rw-rw-   0        0        0    46853 2024-03-19 10:15:03.000000 cellpy-1.0.2a1/cellpy/readers/core.py
+-rw-rw-rw-   0        0        0    23581 2024-03-23 09:21:26.000000 cellpy-1.0.2a1/cellpy/readers/dbreader.py
+-rw-rw-rw-   0        0        0      594 2024-03-19 10:15:03.000000 cellpy-1.0.2a1/cellpy/readers/do.py
+-rw-rw-rw-   0        0        0    18255 2024-03-19 10:15:03.000000 cellpy-1.0.2a1/cellpy/readers/filefinder.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:28:32.033036 cellpy-1.0.2a1/cellpy/readers/instruments/
+-rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.2a1/cellpy/readers/instruments/__init__.py
+-rw-rw-rw-   0        0        0    50060 2024-03-19 10:15:03.000000 cellpy-1.0.2a1/cellpy/readers/instruments/arbin_res.py
+-rw-rw-rw-   0        0        0    20270 2024-03-19 10:15:03.000000 cellpy-1.0.2a1/cellpy/readers/instruments/arbin_sql.py
+-rw-rw-rw-   0        0        0    21106 2024-03-19 10:15:03.000000 cellpy-1.0.2a1/cellpy/readers/instruments/arbin_sql_7.py
+-rw-rw-rw-   0        0        0    11088 2024-03-19 10:15:03.000000 cellpy-1.0.2a1/cellpy/readers/instruments/arbin_sql_csv.py
+-rw-rw-rw-   0        0        0     9389 2024-03-19 10:15:03.000000 cellpy-1.0.2a1/cellpy/readers/instruments/arbin_sql_h5.py
+-rw-rw-rw-   0        0        0     9921 2024-02-19 12:52:17.000000 cellpy-1.0.2a1/cellpy/readers/instruments/arbin_sql_xlsx.py
+-rw-rw-rw-   0        0        0    28999 2024-03-19 10:15:03.000000 cellpy-1.0.2a1/cellpy/readers/instruments/base.py
+-rw-rw-rw-   0        0        0    26718 2024-03-19 10:15:03.000000 cellpy-1.0.2a1/cellpy/readers/instruments/biologics_mpr.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:28:32.043043 cellpy-1.0.2a1/cellpy/readers/instruments/configurations/
+-rw-rw-rw-   0        0        0     6631 2024-03-19 10:15:03.000000 cellpy-1.0.2a1/cellpy/readers/instruments/configurations/__init__.py
+-rw-rw-rw-   0        0        0     4332 2024-03-19 10:15:03.000000 cellpy-1.0.2a1/cellpy/readers/instruments/configurations/maccor_txt_one.py
+-rw-rw-rw-   0        0        0     2020 2024-03-19 10:15:03.000000 cellpy-1.0.2a1/cellpy/readers/instruments/configurations/maccor_txt_three.py
+-rw-rw-rw-   0        0        0     1961 2024-03-19 10:15:03.000000 cellpy-1.0.2a1/cellpy/readers/instruments/configurations/maccor_txt_two.py
+-rw-rw-rw-   0        0        0     3549 2024-02-18 15:23:05.000000 cellpy-1.0.2a1/cellpy/readers/instruments/configurations/maccor_txt_zero.py
+-rw-rw-rw-   0        0        0     2132 2024-02-18 15:23:05.000000 cellpy-1.0.2a1/cellpy/readers/instruments/configurations/neware_txt_zero.py
+-rw-rw-rw-   0        0        0    10627 2024-03-19 10:15:03.000000 cellpy-1.0.2a1/cellpy/readers/instruments/custom.py
+-rw-rw-rw-   0        0        0     3798 2024-02-19 12:52:17.000000 cellpy-1.0.2a1/cellpy/readers/instruments/ext_nda_reader.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:28:32.046035 cellpy-1.0.2a1/cellpy/readers/instruments/loader_specific_modules/
+-rw-rw-rw-   0        0        0        0 2022-06-03 19:58:41.000000 cellpy-1.0.2a1/cellpy/readers/instruments/loader_specific_modules/__init__.py
+-rw-rw-rw-   0        0        0    49457 2024-03-19 10:15:03.000000 cellpy-1.0.2a1/cellpy/readers/instruments/loader_specific_modules/biologic_file_format.py
+-rw-rw-rw-   0        0        0     1430 2024-03-19 10:15:03.000000 cellpy-1.0.2a1/cellpy/readers/instruments/local_instrument.py
+-rw-rw-rw-   0        0        0    14747 2024-03-23 09:21:26.000000 cellpy-1.0.2a1/cellpy/readers/instruments/maccor_txt.py
+-rw-rw-rw-   0        0        0     3519 2024-03-19 10:15:03.000000 cellpy-1.0.2a1/cellpy/readers/instruments/neware_txt.py
+-rw-rw-rw-   0        0        0    17041 2024-03-19 10:15:03.000000 cellpy-1.0.2a1/cellpy/readers/instruments/neware_xlsx.py
+-rw-rw-rw-   0        0        0    15973 2024-03-19 10:15:03.000000 cellpy-1.0.2a1/cellpy/readers/instruments/pec_csv.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:28:32.051035 cellpy-1.0.2a1/cellpy/readers/instruments/processors/
+-rw-rw-rw-   0        0        0        0 2022-05-27 12:07:50.000000 cellpy-1.0.2a1/cellpy/readers/instruments/processors/__init__.py
+-rw-rw-rw-   0        0        0    17627 2024-04-28 11:07:34.000000 cellpy-1.0.2a1/cellpy/readers/instruments/processors/post_processors.py
+-rw-rw-rw-   0        0        0     1448 2024-03-19 10:15:03.000000 cellpy-1.0.2a1/cellpy/readers/instruments/processors/pre_processors.py
+-rw-rw-rw-   0        0        0    27486 2024-03-19 10:15:03.000000 cellpy-1.0.2a1/cellpy/readers/sql_dbreader.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:28:32.074036 cellpy-1.0.2a1/cellpy/utils/
+-rw-rw-rw-   0        0        0      192 2021-12-21 09:11:58.000000 cellpy-1.0.2a1/cellpy/utils/__init__.py
+-rw-rw-rw-   0        0        0    67863 2024-06-01 14:07:42.000000 cellpy-1.0.2a1/cellpy/utils/batch.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:28:32.095036 cellpy-1.0.2a1/cellpy/utils/batch_tools/
+-rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.2a1/cellpy/utils/batch_tools/__init__.py
+-rw-rw-rw-   0        0        0     7578 2024-02-18 15:23:05.000000 cellpy-1.0.2a1/cellpy/utils/batch_tools/batch_analyzers.py
+-rw-rw-rw-   0        0        0    19592 2024-02-18 15:23:05.000000 cellpy-1.0.2a1/cellpy/utils/batch_tools/batch_core.py
+-rw-rw-rw-   0        0        0    44218 2024-06-01 14:05:25.000000 cellpy-1.0.2a1/cellpy/utils/batch_tools/batch_experiments.py
+-rw-rw-rw-   0        0        0     2931 2024-02-18 15:23:05.000000 cellpy-1.0.2a1/cellpy/utils/batch_tools/batch_exporters.py
+-rw-rw-rw-   0        0        0    14268 2024-03-19 10:15:03.000000 cellpy-1.0.2a1/cellpy/utils/batch_tools/batch_helpers.py
+-rw-rw-rw-   0        0        0    29214 2024-03-23 09:21:26.000000 cellpy-1.0.2a1/cellpy/utils/batch_tools/batch_journals.py
+-rw-rw-rw-   0        0        0    47193 2024-04-30 13:01:22.000000 cellpy-1.0.2a1/cellpy/utils/batch_tools/batch_plotters.py
+-rw-rw-rw-   0        0        0      245 2021-12-21 09:11:58.000000 cellpy-1.0.2a1/cellpy/utils/batch_tools/batch_reporters.py
+-rw-rw-rw-   0        0        0     3404 2024-02-18 15:23:05.000000 cellpy-1.0.2a1/cellpy/utils/batch_tools/dumpers.py
+-rw-rw-rw-   0        0        0    10200 2024-02-19 12:52:17.000000 cellpy-1.0.2a1/cellpy/utils/batch_tools/engines.py
+-rw-rw-rw-   0        0        0     5294 2024-02-18 15:23:05.000000 cellpy-1.0.2a1/cellpy/utils/batch_tools/sqlite_from_excel_db.py
+-rw-rw-rw-   0        0        0    88256 2024-06-01 13:48:42.000000 cellpy-1.0.2a1/cellpy/utils/collectors.py
+-rw-rw-rw-   0        0        0      260 2022-05-27 12:07:50.000000 cellpy-1.0.2a1/cellpy/utils/diagnostics.py
+-rw-rw-rw-   0        0        0    78981 2024-03-19 10:15:03.000000 cellpy-1.0.2a1/cellpy/utils/easyplot.py
+-rw-rw-rw-   0        0        0     9123 2024-03-19 10:15:03.000000 cellpy-1.0.2a1/cellpy/utils/example_data.py
+-rw-rw-rw-   0        0        0    47050 2024-06-03 08:07:35.000000 cellpy-1.0.2a1/cellpy/utils/helpers.py
+-rw-rw-rw-   0        0        0    39839 2024-03-19 10:15:03.000000 cellpy-1.0.2a1/cellpy/utils/ica.py
+-rw-rw-rw-   0        0        0      189 2022-05-27 12:07:50.000000 cellpy-1.0.2a1/cellpy/utils/live.py
+-rw-rw-rw-   0        0        0    32747 2024-02-18 15:23:05.000000 cellpy-1.0.2a1/cellpy/utils/ocv_rlx.py
+-rw-rw-rw-   0        0        0    27347 2024-03-19 10:15:03.000000 cellpy-1.0.2a1/cellpy/utils/plotutils.py
+-rw-rw-rw-   0        0        0     1789 2024-03-19 10:15:03.000000 cellpy-1.0.2a1/cellpy/utils/processor.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:28:32.097043 cellpy-1.0.2a1/cellpy.egg-info/
+-rw-rw-rw-   0        0        0     8942 2024-06-03 08:28:31.000000 cellpy-1.0.2a1/cellpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3025 2024-06-03 08:28:31.000000 cellpy-1.0.2a1/cellpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 08:28:31.000000 cellpy-1.0.2a1/cellpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 08:28:31.000000 cellpy-1.0.2a1/cellpy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-06-03 08:28:31.000000 cellpy-1.0.2a1/cellpy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      404 2024-06-03 08:28:31.000000 cellpy-1.0.2a1/cellpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-06-03 08:28:31.000000 cellpy-1.0.2a1/cellpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      367 2024-03-19 10:15:09.000000 cellpy-1.0.2a1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-03 08:28:32.100035 cellpy-1.0.2a1/setup.cfg
+-rw-rw-rw-   0        0        0     3150 2024-03-19 10:15:09.000000 cellpy-1.0.2a1/setup.py
```

### Comparing `cellpy-1.0.1b5/CONTRIBUTING.md` & `cellpy-1.0.2a1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/HISTORY.md` & `cellpy-1.0.2a1/HISTORY.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # History
 
-## 1.0.1 (under development)
+## 1.0.1
 
 * Utils: `example_data` now includes auto-download of example data
 * General: supports only python 3.10 and up to 3.11
 * Batch: `naked` and `init(empty=True)` easier method for creating batch with empty pages
 * File handling: new fix in `find_files`
 * Batch / Utils: refactored and updated `Collectors` (using `plotly`)
 * Batch: new summary plotter (using `plotly`)
@@ -15,19 +15,17 @@
 * Added possibility to filter on C-rates (`c.get_cycles`)
 * Added experimental feature `c.total_time_at_voltage_level` for calculating total time at low/high voltage
 * Added experimental instrument reader for neware xlsx files (hopefully not used much because it is very slow)
 * Added try-except block for ica post-processing step and add if-clause (suggested by Vajee)
 * Fixed several smaller bugs and improved some of the functionality (most notably in `c.get_cap`)
 * Added CI for macOS
 * Added conda package including `sqlalchemy-access`
-* [under progress]: check how cycle_mode and specific is handled and possibly improve
-* [under progress]: start moving/implementing all methods that modify the data to the `do` module
-* [under progress]: improve plotting tools
-* [under progress]: improve documentation
-* [under progress]: improve feedback from the CLI
+* Improved plotting tools
+* Improved documentation
+* Improved feedback from the CLI
 
 ## 1.0.0 (2023)
 
 * Unit handling: new unit handling (using pint)
 * Unit handling: renaming summary headers
 * Unit handling: new cellpy-file-format version
 * Unit handling: tool for converting old to new format
```

### Comparing `cellpy-1.0.1b5/LICENSE.md` & `cellpy-1.0.2a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/MANIFEST.in` & `cellpy-1.0.2a1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/PKG-INFO` & `cellpy-1.0.2a1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellpy
-Version: 1.0.1b5
+Version: 1.0.2a1
 Summary: Extract and manipulate data from battery data testers.
 Home-page: https://github.com/jepegit/cellpy
 Author: Jan Petter Maehlen
 Author-email: jepe@ife.no
 License: MIT license
 Keywords: cellpy
 Classifier: Development Status :: 5 - Production/Stable
@@ -112,15 +112,15 @@
 Contributions are welcome, and they are greatly appreciated! Every
 little bit helps, and credit will always be given. If you want to contribute,
 please have a look at [Contributing Guidelines](CONTRIBUTING.md).
 
 
 # History
 
-## 1.0.1 (under development)
+## 1.0.1
 
 * Utils: `example_data` now includes auto-download of example data
 * General: supports only python 3.10 and up to 3.11
 * Batch: `naked` and `init(empty=True)` easier method for creating batch with empty pages
 * File handling: new fix in `find_files`
 * Batch / Utils: refactored and updated `Collectors` (using `plotly`)
 * Batch: new summary plotter (using `plotly`)
@@ -131,19 +131,17 @@
 * Added possibility to filter on C-rates (`c.get_cycles`)
 * Added experimental feature `c.total_time_at_voltage_level` for calculating total time at low/high voltage
 * Added experimental instrument reader for neware xlsx files (hopefully not used much because it is very slow)
 * Added try-except block for ica post-processing step and add if-clause (suggested by Vajee)
 * Fixed several smaller bugs and improved some of the functionality (most notably in `c.get_cap`)
 * Added CI for macOS
 * Added conda package including `sqlalchemy-access`
-* [under progress]: check how cycle_mode and specific is handled and possibly improve
-* [under progress]: start moving/implementing all methods that modify the data to the `do` module
-* [under progress]: improve plotting tools
-* [under progress]: improve documentation
-* [under progress]: improve feedback from the CLI
+* Improved plotting tools
+* Improved documentation
+* Improved feedback from the CLI
 
 ## 1.0.0 (2023)
 
 * Unit handling: new unit handling (using pint)
 * Unit handling: renaming summary headers
 * Unit handling: new cellpy-file-format version
 * Unit handling: tool for converting old to new format
```

### Comparing `cellpy-1.0.1b5/README.md` & `cellpy-1.0.2a1/README.md`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/__init__.py` & `cellpy-1.0.2a1/cellpy/__init__.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/cli.py` & `cellpy-1.0.2a1/cellpy/cli.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/exceptions.py` & `cellpy-1.0.2a1/cellpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/internals/core.py` & `cellpy-1.0.2a1/cellpy/internals/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,22 +25,137 @@
     cast,
 )
 
 import fabric
 
 from cellpy.exceptions import UnderDefined
 
+
 S = TypeVar("S", bound="OtherPath")
 URI_PREFIXES = ["ssh:", "sftp:", "scp:", "http:", "https:", "ftp:", "ftps:", "smb:"]
 IMPLEMENTED_PROTOCOLS = ["ssh:", "sftp:", "scp:"]
 # name of environment variable that holds the key file and password:
 ENV_VAR_CELLPY_KEY_FILENAME = "CELLPY_KEY_FILENAME"
 ENV_VAR_CELLPY_PASSWORD = "CELLPY_PASSWORD"
 
 
+def check_connection(
+    p=None,
+):
+    """Check if the connection works.
+
+    This is a helper function for cellpy v1.0 only and should be removed in later versions after
+    the OtherPath class has been updated to work with python >= 3.12.
+
+    Args:
+        p (str, pathlib.Path or OtherPath, optional): The path to check. Defaults to prms.Paths.rawdatadir.
+
+    """
+    # Note: users run this function from helpers.py
+    from pprint import pprint
+
+    logging.debug("checking connection")
+    if p is None:
+        print("No path given. Checking rawdatadir from prms.")
+
+        # need to import prms here to avoid circular imports:
+        from cellpy import prms
+
+        p = prms.Paths.rawdatadir
+
+    # recreating the OtherPath object to OtherPath since core is imported in the top __init__.py
+    # file resulting in isinstance(p, OtherPath) to be False
+    p = OtherPath(p)
+    logging.debug(f"p: {p}")
+
+    print("\nCollecting connection information:")
+
+    if not p.is_external:
+        print(f"   - {p} is not external. Returning.")
+        return {}
+
+    info = {
+        "is_external": p.is_external,
+        "uri_prefix": p.uri_prefix,
+        "location": p.location,
+        "raw_path": p.raw_path,
+        "full_path": p.full_path,
+        "host": p.location,
+    }
+
+    uri_prefix = p.uri_prefix.replace("//", "")
+    info["uri_prefix"] = uri_prefix
+    if uri_prefix not in URI_PREFIXES:
+        print(f"   - uri_prefix {uri_prefix} not recognized")
+    if uri_prefix not in IMPLEMENTED_PROTOCOLS:
+        print(f"   - uri_prefix {uri_prefix.replace(':', '')} not implemented yet")
+
+    password = os.getenv(ENV_VAR_CELLPY_PASSWORD, None)
+    info["password"] = "********" if password is not None else None
+
+    key_filename = os.getenv(ENV_VAR_CELLPY_KEY_FILENAME, None)
+    if password is None and key_filename is None:
+        print(
+            f"   - You must define either {ENV_VAR_CELLPY_PASSWORD} "
+            f"or {ENV_VAR_CELLPY_KEY_FILENAME} environment variables."
+        )
+    if key_filename is not None:
+        key_filename = pathlib.Path(key_filename).expanduser().resolve()
+        info["key_filename"] = str(key_filename)
+        if not pathlib.Path(key_filename).is_file():
+            print(f"   - Could not find key file {key_filename}")
+    else:
+        print("   - Using password")
+
+    for k, v in info.items():
+        print(f" {k}: {v}")
+
+    print("\nChecking connection:")
+    connect_kwargs, host = p.connection_info()
+
+    path_separator = "/"  # only supports unix-like systems
+    with fabric.Connection(host, connect_kwargs=connect_kwargs) as conn:
+        try:
+            t1 = time.perf_counter()
+            try:
+                sftp_conn = conn.sftp()
+            except Exception as e:
+                print(f"   - Could not connect to {host}")
+                print(f"     {e}")
+                return info
+
+            print(f" connecting     [{time.perf_counter() - t1:.2f} seconds] OK")
+            sftp_conn.chdir(p.raw_path)
+            print(f" chdir          [{time.perf_counter() - t1:.2f} seconds] OK")
+            files = [
+                f"{p.raw_path}{path_separator}{f}"
+                for f in sftp_conn.listdir()
+                if not stat.S_ISDIR(sftp_conn.stat(f).st_mode)
+            ]
+            print(f" listing files  [{time.perf_counter() - t1:.2f} seconds] OK")
+            sub_dirs = [
+                f"{p.raw_path}{path_separator}{f}"
+                for f in sftp_conn.listdir()
+                if stat.S_ISDIR(sftp_conn.stat(f).st_mode)
+            ]
+            n_files = len(files)
+            n_sub_dirs = len(sub_dirs)
+            info["number_of_files"] = n_files
+            info["number_of_sub_directories"] = n_sub_dirs
+            print(f" found {n_files} files and {n_sub_dirs} sub directories")
+
+        except FileNotFoundError as e:
+            print(
+                f"   - FileNotFoundError: Could not perform directory listing in {p.raw_path} on {host}."
+                f"\n     {e}"
+            )
+
+    return info
+
+
 @dataclass
 class ExternalStatResult:
     """Mock of os.stat_result."""
 
     # st_mode: int = 0
     # st_ino: int = 0
     # st_dev: int = 0
@@ -653,15 +768,15 @@
                         break
                     levels -= 1
 
                 logging.debug(f"globbing took {time.time() - t1:.2f} seconds")
                 return files
             except FileNotFoundError as e:
                 raise FileNotFoundError(
-                    f"Could not find file {self.raw_path} on {host}"
+                    f"Could not perform directory listing in {self.raw_path} on {host}.\n{e}"
                 ) from e
 
     def _glob_with_fabric(
         self: S,
         host: str,
         connect_kwargs: dict,
         glob_str: str,
@@ -734,7 +849,23 @@
                     filtered_files = fnmatch.filter(files, glob_str)
                 logging.debug(f"globbing took {time.time() - t1:.2f} seconds")
                 return filtered_files
             except FileNotFoundError as e:
                 raise FileNotFoundError(
                     f"Could not find file {self.raw_path} on {host}"
                 ) from e
+
+
+def _check():
+    print("Testing OtherPath-connection")
+    # info = check_connection()
+    p0 = "scp://odin/home/jepe@ad.ife.no/projects"
+    # info = check_connection(p0)
+    p1 = "scp://odin/home/jepe@ad.ife.no/this-folder-does-not-exist"
+    # info = check_connection(p1)
+    p2 = pathlib.Path(".").resolve()
+    info = check_connection(p2)
+
+
+if __name__ == "__main__":
+    logging.debug("testing OtherPath")
+    _check()
```

### Comparing `cellpy-1.0.1b5/cellpy/log.py` & `cellpy-1.0.2a1/cellpy/log.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/logging.json` & `cellpy-1.0.2a1/cellpy/logging.json`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/parameters/.cellpy_prms_default.conf` & `cellpy-1.0.2a1/cellpy/parameters/.cellpy_prms_default.conf`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/parameters/internal_settings.py` & `cellpy-1.0.2a1/cellpy/parameters/internal_settings.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/parameters/legacy/update_headers.py` & `cellpy-1.0.2a1/cellpy/parameters/legacy/update_headers.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/parameters/prmreader.py` & `cellpy-1.0.2a1/cellpy/parameters/prmreader.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/parameters/prms.py` & `cellpy-1.0.2a1/cellpy/parameters/prms.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/readers/cellreader.py` & `cellpy-1.0.2a1/cellpy/readers/cellreader.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/readers/core.py` & `cellpy-1.0.2a1/cellpy/readers/core.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/readers/dbreader.py` & `cellpy-1.0.2a1/cellpy/readers/dbreader.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,39 +111,51 @@
             f"<ExcelReader> (rows: {len(self.table)}, cols: {len(self.table.columns)})"
         )
 
     def _repr_html_(self):
         return f"<b>ExcelReader</b> (rows: {len(self.table)}, cols: {len(self.table.columns)})"
 
     def select_batch(
-        self, batch, batch_col_name=None, case_sensitive=True, drop=True
+        self,
+        batch,
+        batch_col_name=None,
+        case_sensitive=True,
+        drop=True,
+        clean=False,
+        **kwargs,
     ) -> List[int]:
         """Selects the rows in column batch_col_number.
 
         Args:
             batch: batch to select
             batch_col_name: column name to use for batch selection (default: DbSheetCols.batch).
             case_sensitive: if True, the batch name must match exactly (default: True).
             drop: if True, all un-selected rows are dropped from the table (default: True).
+            clean: if True and drop is True, the table is cleaned from duplicates and NaNs (default: False).
 
         Returns:
             List of row indices
         """
 
+        # including kwargs to avoid breaking if new kwargs are added
+
         if self.selected_batch is None:
             return self._select_batch(
                 batch,
                 batch_col_name=batch_col_name,
                 case_sensitive=case_sensitive,
                 drop=drop,
+                clean=clean,
             )
         else:
             return self.selected_batch
 
-    def _select_batch(self, batch, batch_col_name=None, case_sensitive=True, drop=True):
+    def _select_batch(
+        self, batch, batch_col_name=None, case_sensitive=True, drop=True, clean=False
+    ):
         if not batch_col_name:
             batch_col_name = self.db_sheet_cols.batch
         logging.debug("selecting batch - %s" % batch)
         sheet = self.table
         identity = self.db_sheet_cols.id
         exists_col_number = self.db_sheet_cols.exists
 
@@ -153,14 +165,19 @@
             criterion = (sheet.loc[:, batch_col_name]).upper() == batch.upper()
 
         exists = sheet.loc[:, exists_col_number] > 0
         # This will crash if the col is not of dtype number
         sheet = sheet[criterion & exists]
         if drop:
             self.table = sheet
+            if clean:
+                sheet = sheet.loc[:, identity]
+                sheet.drop_duplicates(inplace=True)
+                sheet.dropna(inplace=True)
+                return sheet.values.astype(int)
         return sheet.loc[:, identity].values.astype(int)
 
     def from_batch(
         self,
         batch_name: str,
         include_key: bool = False,
         include_individual_arguments: bool = False,
```

### Comparing `cellpy-1.0.1b5/cellpy/readers/do.py` & `cellpy-1.0.2a1/cellpy/readers/do.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/readers/filefinder.py` & `cellpy-1.0.2a1/cellpy/readers/filefinder.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/readers/instruments/arbin_res.py` & `cellpy-1.0.2a1/cellpy/readers/instruments/arbin_res.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/readers/instruments/arbin_sql.py` & `cellpy-1.0.2a1/cellpy/readers/instruments/arbin_sql.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/readers/instruments/arbin_sql_7.py` & `cellpy-1.0.2a1/cellpy/readers/instruments/arbin_sql_7.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/readers/instruments/arbin_sql_csv.py` & `cellpy-1.0.2a1/cellpy/readers/instruments/arbin_sql_csv.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/readers/instruments/arbin_sql_h5.py` & `cellpy-1.0.2a1/cellpy/readers/instruments/arbin_sql_h5.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/readers/instruments/arbin_sql_xlsx.py` & `cellpy-1.0.2a1/cellpy/readers/instruments/arbin_sql_xlsx.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/readers/instruments/base.py` & `cellpy-1.0.2a1/cellpy/readers/instruments/base.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/readers/instruments/biologics_mpr.py` & `cellpy-1.0.2a1/cellpy/readers/instruments/biologics_mpr.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/readers/instruments/configurations/__init__.py` & `cellpy-1.0.2a1/cellpy/readers/instruments/configurations/__init__.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/readers/instruments/configurations/maccor_txt_one.py` & `cellpy-1.0.2a1/cellpy/readers/instruments/configurations/maccor_txt_one.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/readers/instruments/configurations/maccor_txt_three.py` & `cellpy-1.0.2a1/cellpy/readers/instruments/configurations/maccor_txt_three.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/readers/instruments/configurations/maccor_txt_two.py` & `cellpy-1.0.2a1/cellpy/readers/instruments/configurations/maccor_txt_two.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/readers/instruments/configurations/maccor_txt_zero.py` & `cellpy-1.0.2a1/cellpy/readers/instruments/configurations/maccor_txt_zero.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/readers/instruments/configurations/neware_txt_zero.py` & `cellpy-1.0.2a1/cellpy/readers/instruments/configurations/neware_txt_zero.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/readers/instruments/custom.py` & `cellpy-1.0.2a1/cellpy/readers/instruments/custom.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/readers/instruments/ext_nda_reader.py` & `cellpy-1.0.2a1/cellpy/readers/instruments/ext_nda_reader.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/readers/instruments/loader_specific_modules/biologic_file_format.py` & `cellpy-1.0.2a1/cellpy/readers/instruments/loader_specific_modules/biologic_file_format.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/readers/instruments/local_instrument.py` & `cellpy-1.0.2a1/cellpy/readers/instruments/local_instrument.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/readers/instruments/maccor_txt.py` & `cellpy-1.0.2a1/cellpy/readers/instruments/maccor_txt.py`

 * *Files 1% similar despite different names*

```diff
@@ -423,17 +423,17 @@
     import pathlib
 
     import cellpy
     import pandas as pd
     import matplotlib.pyplot as plt
 
     DATADIR = r"C:\scripting\cellpy_dev_resources\dev_data\simba_Maccor\S4000"
-    FILENAME = "01_UBham_CD_M50_Validation_0deg_01.txt"
+    FILENAME = "KIT-CW-SIMBA-ET-FC-NAPF6-007.037-Full_data.txt"
     INSTRUMENT = "maccor_txt"
-    MODEL = "ONE"
+    MODEL = "TWO"
 
     pd.options.display.max_columns = 100
     datadir = pathlib.Path(DATADIR)
     name = datadir / FILENAME
     out = pathlib.Path(r"C:\scripting\trash")
     print(f"File exists? {name.is_file()}")
     if not name.is_file():
```

### Comparing `cellpy-1.0.1b5/cellpy/readers/instruments/neware_txt.py` & `cellpy-1.0.2a1/cellpy/readers/instruments/neware_txt.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/readers/instruments/neware_xlsx.py` & `cellpy-1.0.2a1/cellpy/readers/instruments/neware_xlsx.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/readers/instruments/pec_csv.py` & `cellpy-1.0.2a1/cellpy/readers/instruments/pec_csv.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/readers/instruments/processors/post_processors.py` & `cellpy-1.0.2a1/cellpy/readers/instruments/processors/post_processors.py`

 * *Files 2% similar despite different names*

```diff
@@ -363,24 +363,42 @@
 
             discharge = raw.loc[
                 (raw[state_column].isin(discharge_keys)) & (raw[cycle_index_hdr] == i),
                 [data_point, base_col_name],
             ]
 
             if not charge.empty:
+                # TODO: fix this warning
+                # FutureWarning: A value is trying to be set on a copy of a DataFrame or Series through
+                # chained assignment using an inplace method.
+                # The behavior will change in pandas 3.0. This inplace method will never work because the
+                # intermediate object on which we are setting values always behaves as a copy.
+                #  For example, when doing 'df[col].method(value, inplace=True)',
+                #  try using 'df.method({col: value}, inplace=True)' or
+                #  df[col] = df[col].method(value) instead,
+                #  to perform the operation inplace on the original object.
                 raw[temp_col_name_charge].update(n_charge * charge[base_col_name])
                 if propagate:
                     charge_last_index, charge_last_val = charge.iloc[-1]
                     raw.loc[
                         (raw[data_point] > charge_last_index)
                         & (raw[cycle_index_hdr] == i),
                         temp_col_name_charge,
                     ] = charge_last_val
 
             if not discharge.empty:
+                # TODO: fix this warning
+                # FutureWarning: A value is trying to be set on a copy of a DataFrame or Series through
+                # chained assignment using an inplace method.
+                # The behavior will change in pandas 3.0. This inplace method will never work because the
+                # intermediate object on which we are setting values always behaves as a copy.
+                #  For example, when doing 'df[col].method(value, inplace=True)',
+                #  try using 'df.method({col: value}, inplace=True)' or
+                #  df[col] = df[col].method(value) instead,
+                #  to perform the operation inplace on the original object.
                 raw[temp_col_name_discharge].update(
                     n_discharge * discharge[base_col_name]
                 )
                 if propagate:
                     (discharge_last_index, discharge_last_val) = discharge.iloc[-1]
                     raw.loc[
                         (raw[data_point] > discharge_last_index)
```

### Comparing `cellpy-1.0.1b5/cellpy/readers/instruments/processors/pre_processors.py` & `cellpy-1.0.2a1/cellpy/readers/instruments/processors/pre_processors.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/readers/sql_dbreader.py` & `cellpy-1.0.2a1/cellpy/readers/sql_dbreader.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/utils/batch.py` & `cellpy-1.0.2a1/cellpy/utils/batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import logging
 import os
 import pathlib
 import shutil
 import sys
 import warnings
+from typing import List, Optional, Any
 
 import pandas as pd
 from pandas import Index
 from tqdm.auto import tqdm
 
 import cellpy.exceptions
 from cellpy import log, prms
@@ -904,24 +905,37 @@
 
     def paginate(self) -> None:
         """Create the folders where cellpy will put its output."""
 
         self.experiment.journal.paginate()
         logging.info("created folders")
 
+    def save(self) -> None:
+        """Save journal and cellpy files.
+
+        The journal file will be saved in the project directory and in the
+        batch-file-directory (``prms.Paths.batchfiledir``). The latter is useful
+        for processing several batches using the ``iterate_batches`` functionality.
+
+        The name and location of the cellpy files is determined by the journal pages.
+        """
+
+        self.save_journal()
+        self.experiment.save_cells()
+
     def save_journal(self) -> None:
         """Save the journal (json-format).
 
         The journal file will be saved in the project directory and in the
         batch-file-directory (``prms.Paths.batchfiledir``). The latter is useful
         for processing several batches using the ``iterate_batches`` functionality.
 
         """
 
-        # Remark! Got an recursive error when running on mac.
+        # Remark! Got a recursive error when running on Mac.
         self.experiment.journal.to_file(to_project_folder=True, paginate=False)
         logging.info("saved journal pages to project folder")
         self.duplicate_journal(prms.Paths.batchfiledir)
         logging.info("duplicated journal pages to batch dir")
         self.duplicate_journal()
         logging.info("duplicated journal pages to current dir")
 
@@ -1011,26 +1025,32 @@
             logging.info("Modifying the cellpy-files.")
             logging.info(f"selector: {selector}")
             self.experiment.force_cellpy = True
             self.update(selector=selector, **kwargs)
 
     # TODO: list_journals?
 
-    def link(self, max_cycle=None, force_combine_summaries=False) -> None:
+    def link(
+        self,
+        max_cycle: Optional[int] = None,
+        mark_bad=False,
+        force_combine_summaries=False,
+    ) -> None:
         """Link journal content to the cellpy-files and load the step information.
 
         Args:
             max_cycle (int): set maximum cycle number to link to.
+            mark_bad (bool): mark cells as bad if they are not linked.
             force_combine_summaries (bool): automatically run combine_summaries (set this to True
                 if you are re-linking without max_cycle for a batch that previously were linked
                 with max_cycle)
 
         """
 
-        self.experiment.link(max_cycle=max_cycle)
+        self.experiment.link(max_cycle=max_cycle, mark_bad=mark_bad)
         if force_combine_summaries or max_cycle:
             self.summary_collector.do(reset=True)
 
     def load(self) -> None:
         """Load the selected datasets.
 
         Warnings:
@@ -1151,14 +1171,18 @@
             direction (str): plot charge or discharge (defaults to "charge")
             rate (bool): (defaults to False)
             ir (bool): (defaults to True)
 
             group_legends (bool): group the legends so that they can be turned visible/invisible
                 as a group (defaults to True) (only for plotly)
             base_template (str): template to use for the plot (only for plotly)
+
+            filter_by_group (int or list of ints): show only the selected group(s)
+            filter_by_name (str): show only cells containing this string
+
         """
 
         if reload_data or ("summary_engine" not in self.experiment.memory_dumped):
             logging.debug("running summary_collector")
             self.summary_collector.do(reset=True)
 
         if backend is None:
@@ -1280,16 +1304,37 @@
     Args:
         name (str): name of batch
         project (str): name of project
         batch_col (str): batch column identifier (only used for loading from db with simple_db_reader)
         allow_from_journal (bool): if True, the journal file will be loaded if it exists
         force_reload (bool): if True, the batch will be reloaded even if the journal file exists
         drop_bad_cells (bool): if True, bad cells will be dropped (only apply if journal file is loaded)
+        auto_use_file_list (bool): Experimental feature. If True, a file list will be generated and used
+            instead of searching for files in the folders.
         **kwargs: sent to Batch during initialization
 
+    Keyword Args:
+        db_reader (str): data-base reader to use (defaults to "default" as given
+          in the config-file or prm-class).
+        frame (pandas.DataFrame): load from given dataframe.
+        default_log_level (str): custom log-level (defaults to None (i.e. default log-level in cellpy)).
+        custom_log_dir (str or pathlib.Path): custom folder for putting the log-files.
+        force_raw_file (bool): load from raw regardless (defaults to False).
+        force_cellpy (bool): load cellpy-files regardless (defaults to False).
+        force_recalc (bool): Always recalculate (defaults to False).
+        export_cycles (bool): Extract and export individual cycles to csv (defaults to True).
+        export_raw (bool): Extract and export raw-data to csv (defaults to True).
+        export_ica (bool): Extract and export individual dQ/dV data to csv (defaults to True).
+        accept_errors (bool): Continue automatically to next file if error is raised (defaults to False).
+        nom_cap (float): give a nominal capacity if you want to use another value than
+          the one given in the config-file or prm-class.
+        max_cycle (int or None): maximum number of cycles to link up to (defaults to None).
+        force_combine_summaries (bool): automatically run combine_summaries when linking.
+
+
     Returns:
         populated Batch object (``cellpy.utils.batch.Batch``)
 
     """
 
     if allow_from_journal:
         b = Batch(name=name, project=project, batch_col=batch_col, db_reader=None)
@@ -1305,45 +1350,67 @@
                 print(f" - loading journal file {journal_file}")
                 b.experiment.journal.from_file(journal_file)
                 if force_reload:
                     print(f" - reloading")
                     b.update()
                 else:
                     print(f" - linking")
-                    b.link()
+                    b.link(
+                        max_cycle=kwargs.pop("max_cycle", None),
+                        mark_bad=True,
+                        force_combine_summaries=kwargs.pop(
+                            "force_combine_summaries", False
+                        ),
+                    )
+
                 if drop_bad_cells:
-                    print(f" - dropping bad cells")
+                    print(f" - dropping cells marked as bad")
                     b.drop_cells_marked_bad()
                 print("OK!")
                 return b
+
             else:
                 print(f" - journal file not found")
 
     auto_use_file_list = kwargs.pop("auto_use_file_list", None)
     try:
         print("loading information from db")
         if batch_col is None:
             batch_col = "b01"  # this is needed due to a bug in cellpy (will be fixed when new db reader is ready)
+        print("initializing batch object")
         b = init(name=name, project=project, batch_col=batch_col, **kwargs)
     except Exception as e:
         print(f"could not initialize batch: {e}")
         return None
+    print("processing batch")
+    try:
+        print("creating journal")
+        b.create_journal(auto_use_file_list=auto_use_file_list)
+        print(" - created journal")
+    except Exception as e:
+        print(f"could not create journal: {e}")
+        print("you might have duplicates in your database index or cell names")
+        return None
+    try:
+        b.duplicate_journal()
+        print(" - duplicated journal")
+        b.paginate()
+        print(" - paginated")
+        print(" - updating...")
+        b.update()
+        print(" - updated")
+        print("collecting and combining summaries")
+        b.combine_summaries()
+        print(" - collected and combined summaries")
+        print("OK!")
+    except Exception as e:
+        print("something went wrong")
+        print(e)
+        print("returning possibly incomplete batch")
 
-    b.create_journal(auto_use_file_list=auto_use_file_list)
-    print(" - created journal")
-    b.duplicate_journal()
-    print(" - duplicated journal")
-    b.paginate()
-    print(" - paginated")
-    print(" - updating...")
-    b.update()
-    print(" - updated")
-    b.combine_summaries()
-    print(" - collected and combined summaries")
-    print("OK!")
     return b
 
 
 def init(*args, empty=False, **kwargs) -> Batch:
     """Returns an initialized instance of the Batch class.
 
     Args:
```

### Comparing `cellpy-1.0.1b5/cellpy/utils/batch_tools/batch_analyzers.py` & `cellpy-1.0.2a1/cellpy/utils/batch_tools/batch_analyzers.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/utils/batch_tools/batch_core.py` & `cellpy-1.0.2a1/cellpy/utils/batch_tools/batch_core.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/utils/batch_tools/batch_experiments.py` & `cellpy-1.0.2a1/cellpy/utils/batch_tools/batch_experiments.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,14 +165,42 @@
                     except ValueError as e:
                         logging.warning(
                             f"ERROR! Could not convert from str to python object!"
                         )
                         logging.debug(e)
         return cell_spec
 
+    def save_cells(self, **kwargs):
+        """Save all cells in the experiment.
+
+        Args:
+            kwargs: passed to the save method of the CellpyData-object.
+
+        Returns:
+            None
+        """
+        errors = []
+        for row in self.journal.pages.iterrows():
+            cell_name = row[0]
+            c = self.data[cell_name]
+            try:
+                if self.custom_data_folder is not None:
+                    print("Save to custom data-folder not implemented yet")
+                    print(f"Saving to {row.cellpy_file_name} instead")
+                if row.fixed and Path(row.cellpy_file_name).is_file():
+                    logging.debug("saving cell skipped (set to 'fixed' in journal)")
+                else:
+                    logging.info(f"saving cell to {row.cellpy_file_name}")
+                    c.ensure_step_table = True
+                    c.save(row.cellpy_file_name, **kwargs)
+            except Exception as e:
+                errors.append(f"could not save {cell_name} - {e}")
+
+        self.errors["save_cells"] = errors
+
     def update(
         self,
         all_in_memory=None,
         cell_specs=None,
         logging_mode=None,
         accept_errors=None,
         **kwargs,
@@ -311,14 +339,20 @@
             l_txt += f" cell_spec: {cell_spec}"
             logging.debug(l_txt)
 
             # --- UPDATING ARGUMENTS ---
             filename = None
             instrument = None
             cellpy_file = OtherPath(row[hdr_journal.cellpy_file_name])
+            if force_cellpy and not cellpy_file.is_file():
+                logging.critical(
+                    f"Cellpy file not given in the journal.pages for index={index}"
+                )
+                errors.append(index)
+                continue
             _cellpy_file = None
             if not force_raw and cellpy_file.is_file():
                 _cellpy_file = cellpy_file
                 logging.debug(f"Got cellpy file: {_cellpy_file}")
             if not force_cellpy:
                 filename = row[hdr_journal.raw_file_names]
                 instrument = row[hdr_journal.instrument]
@@ -860,28 +894,35 @@
                 print(f" {{{key}}}")
         print(" memory dumped ".center(80, "-"))
         if self.memory_dumped is not None:
             for key in self.memory_dumped:
                 print(f"{key}: {type(self.memory_dumped[key])}")
         print(80 * "=")
 
-    def link(self, **kwargs):
+    def link(
+        self,
+        mark_bad=False,
+        **kwargs,
+    ):
         """Ensure that an appropriate link to the cellpy-files exists for
         each cell.
 
         The experiment will then contain a CellpyCell object for each cell
         (in the cell_data_frames attribute) with only the step-table stored.
 
         Remark that running update persists the summary frames instead (or
         everything in case you specify all_in_memory=True).
         This might be considered "a strange and unexpected behaviour". Sorry
         for that (but the authors of this package is also a bit strange...).
 
         (OK, I will change it. Soon.)
 
+        Args:
+            mark_bad (bool): mark bad cells (default: False)
+
         **kwargs: passed to _link_cellpy_file
             max_cycle (int): maximum cycle number to link/load (remark that the
                 cellpy objects will get the property overwrite_able set to False
                 if you give a max_cycle to prevent accidentally saving a "truncated"
                 file (use c.save(filename, overwrite=True) to force overwrite))
 
 
@@ -896,14 +937,19 @@
             try:
                 self._link_cellpy_file(cell_label, **kwargs)
             except IOError as e:
                 logging.warning(e)
                 e_txt = f"{cell_label}: links not established - try update instead"
                 logging.warning(e_txt)
                 errors.append(e_txt)
+                if mark_bad:
+                    if not self.journal.session["bad_cells"]:
+                        self.journal.session["bad_cells"] = []
+                    self.journal.session["bad_cells"].append(cell_label)
+                    logging.warning(f"Marked {cell_label} as bad")
 
         self.errors["link"] = errors
 
     def recalc(
         self,
         save=True,
         step_opts=None,
```

### Comparing `cellpy-1.0.1b5/cellpy/utils/batch_tools/batch_exporters.py` & `cellpy-1.0.2a1/cellpy/utils/batch_tools/batch_exporters.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/utils/batch_tools/batch_helpers.py` & `cellpy-1.0.2a1/cellpy/utils/batch_tools/batch_helpers.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/utils/batch_tools/batch_journals.py` & `cellpy-1.0.2a1/cellpy/utils/batch_tools/batch_journals.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,21 +145,24 @@
             file_name = file_name.with_suffix(".json").name
             project_dir = pathlib.Path(self.project_dir)
 
             file_name = project_dir / file_name
         self.file_name = file_name  # updates object (maybe not smart)
         return file_name
 
-    def from_db(self, project=None, name=None, batch_col=None, **kwargs):
+    def from_db(
+        self, project=None, name=None, batch_col=None, dbreader_kwargs=None, **kwargs
+    ):
         """populate journal from db.
 
         Args:
             project (str): project name.
             name (str): experiment name.
             batch_col (int): batch column.
+            dbreader_kwargs: sent to simple db_reader.
 
         **kwargs: sent to engine.
 
         simple_db-engine -> filefinder.search_for_files:
             run_name(str): run-file identification.
             raw_extension(str): optional, extension of run-files (without the '.').
             cellpy_file_extension(str): optional, extension for cellpy files
@@ -189,19 +192,27 @@
             batch_col = self.batch_col
         if project is not None:
             self.project = project
         if name is None:
             name = self.name
         else:
             self.name = name
-        logging.debug(f"batch_name, batch_col: {name}, {batch_col}")
+
+        if dbreader_kwargs is None:
+            dbreader_kwargs = {}
+
+        logging.debug(
+            f"batch_name, batch_col, dbreader_kwargs: {name}, {batch_col}, {dbreader_kwargs}"
+        )
 
         if self.db_reader is not None:
             if isinstance(self.db_reader, dbreader.Reader):  # Simple excel-db
-                id_keys = self.db_reader.select_batch(name, batch_col)
+                id_keys = self.db_reader.select_batch(
+                    name, batch_col, **dbreader_kwargs
+                )
                 logging.debug(f"id_keys: {id_keys}")
 
                 self.pages = self.engine(self.db_reader, id_keys, **kwargs)
             else:
                 logging.debug(
                     "creating journal pages using advanced reader methods (not simple excel-db)"
                 )
```

### Comparing `cellpy-1.0.1b5/cellpy/utils/batch_tools/batch_plotters.py` & `cellpy-1.0.2a1/cellpy/utils/batch_tools/batch_plotters.py`

 * *Files 3% similar despite different names*

```diff
@@ -745,15 +745,16 @@
                 logging.debug(f"skipping {experiment} - not a CyclingExperiment")
                 logging.debug(f"({type(experiment)})")
                 continue
             canvas = generate_summary_plots(
                 experiment=experiment, farms=farms, **kwargs
             )
             farms.append(canvas)
-            canvas.show()
+            if backend == "plotly":
+                canvas.show()
 
     return farms, barn
 
 
 def generate_summary_plots(experiment, **kwargs):
     pages = experiment.journal.pages
     backend = prms.Batch.backend
@@ -947,14 +948,16 @@
     max_cycle = kwargs.pop("max_cycle", None)
 
     title = kwargs.pop("title", "Cycle Summary")
     x_label = kwargs.pop("x_label", "Cycle Number")
     direction = kwargs.pop("direction", "charge")
     rate = kwargs.pop("rate", False)
     ir = kwargs.pop("ir", True)
+    filter_by_group = kwargs.pop("filter_by_group", None)
+    filter_by_name = kwargs.pop("filter_by_name", None)
 
     individual_plot_height = 250
     header_height = 200
     individual_legend_height = 20
     legend_header_height = 20
 
     hdr_cycle = hdr_summary["cycle_index"]
@@ -1011,14 +1014,23 @@
     sub_titles = ", ".join(sub_titles)
 
     number_of_cells = len(summaries.cell.unique())
     number_of_rows = len(plotted_summaries)
     legend_height = legend_header_height + individual_legend_height * number_of_cells
     plot_height = max(legend_height, individual_plot_height * number_of_rows)
     total_height = header_height + plot_height
+
+    if filter_by_group is not None:
+        if not isinstance(filter_by_group, (list, tuple)):
+            filter_by_group = [filter_by_group]
+        summaries = summaries.loc[summaries[hdr_group].isin([filter_by_group]), :]
+
+    if filter_by_name is not None:
+        summaries = summaries.loc[summaries.cell.str.contains(filter_by_name), :]
+
     canvas = px.line(
         summaries,
         x=hdr_cycle,
         y="value",
         facet_row="variable",
         color=hdr_group,
         symbol=hdr_sub_group,
@@ -1090,14 +1102,16 @@
     max_cycle = kwargs.pop("max_cycle", None)
 
     title = kwargs.pop("title", "Cycle Summary")
     x_label = kwargs.pop("x_label", "Cycle Number")
     direction = kwargs.pop("direction", "charge")
     rate = kwargs.pop("rate", False)
     ir = kwargs.pop("ir", True)
+    filter_by_group = kwargs.pop("filter_by_group", None)
+    filter_by_name = kwargs.pop("filter_by_name", None)
 
     hdr_cycle = hdr_summary["cycle_index"]
     hdr_charge = hdr_summary["charge_capacity_gravimetric"]
     hdr_discharge = hdr_summary["discharge_capacity_gravimetric"]
     hdr_ce = hdr_summary["coulombic_efficiency"]
     hdr_ir_charge = hdr_summary["ir_charge"]
     hdr_ir_discharge = hdr_summary["ir_discharge"]
@@ -1151,14 +1165,22 @@
     sub_titles = ", ".join(sub_titles)
 
     number_of_cells = len(summaries.cell.unique())
     number_of_rows = len(plotted_summaries)
 
     sns.set_theme(style="darkgrid")
 
+    if filter_by_group is not None:
+        if not isinstance(filter_by_group, (list, tuple)):
+            filter_by_group = [filter_by_group]
+        summaries = summaries.loc[summaries[hdr_group].isin([filter_by_group]), :]
+
+    if filter_by_name is not None:
+        summaries = summaries.loc[summaries.cell.str.contains(filter_by_name), :]
+
     canvas_grid = sns.relplot(
         data=summaries,
         kind="line",
         x=hdr_cycle,
         y="value",
         hue=hdr_group,
         style=hdr_sub_group,
```

### Comparing `cellpy-1.0.1b5/cellpy/utils/batch_tools/dumpers.py` & `cellpy-1.0.2a1/cellpy/utils/batch_tools/dumpers.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/utils/batch_tools/engines.py` & `cellpy-1.0.2a1/cellpy/utils/batch_tools/engines.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/utils/batch_tools/sqlite_from_excel_db.py` & `cellpy-1.0.2a1/cellpy/utils/batch_tools/sqlite_from_excel_db.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/utils/collectors.py` & `cellpy-1.0.2a1/cellpy/utils/collectors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """Collectors are used for simplifying plotting and exporting batch objects."""
 
 import functools
 import inspect
 import logging
 import math
+import pickle as pkl
 from pprint import pprint
 from pathlib import Path
 import textwrap
 from typing import Any
 import time
 from itertools import count
 from multiprocessing import Process
+import warnings
 
 import pandas as pd
+import matplotlib.pyplot as plt
 import numpy as np
 
 import cellpy
 from cellpy.readers.core import group_by_interpolate
 from cellpy.utils.batch import Batch
 from cellpy.utils.helpers import concat_summaries
 from cellpy.utils import ica
@@ -36,42 +39,80 @@
 try:
     import seaborn as sns
 
     supported_backends.append("seaborn")
 except ImportError:
     print("WARNING: seaborn not installed")
 
-
 DEFAULT_CYCLES = [1, 10, 20]
 CELLPY_MINIMUM_VERSION = "1.0.0"
 PLOTLY_BASE_TEMPLATE = "seaborn"
 IMAGE_TO_FILE_TIMEOUT = 30
 HDF_KEY = "collected_data"
+MAX_POINTS_SEABORN_FACET_GRID = 60_000
 
 
 def load_data(filename):
     """Load data from hdf5 file."""
     try:
         data = pd.read_hdf(filename, key=HDF_KEY)
     except Exception as e:
         print("Could not load data from hdf5 file")
         print(e)
         return None
     return data
 
 
-def load_figure(filename, backend="plotly"):
+def load_figure(filename, backend=None):
     """Load figure from file."""
+
+    filename = Path(filename)
+
+    if backend is None:
+        suffix = filename.suffix
+        if suffix in [".pkl", ".pickle"]:
+            backend = "matplotlib"
+        elif suffix in [".json", ".plotly", ".jsn"]:
+            backend = "plotly"
+        else:
+            backend = "plotly"
+
     if backend == "plotly":
         return load_plotly_figure(filename)
+    elif backend == "seaborn":
+        return load_matplotlib_figure(filename)
+    elif backend == "matplotlib":
+        return load_matplotlib_figure(filename)
     else:
-        print("WARNING: only plotly is supported at the moment")
+        print(f"WARNING: {backend=} is not supported at the moment")
         return None
 
 
+def save_matplotlib_figure(fig, filename):
+    pkl.dump(fig, open(filename, "wb"))
+
+
+def make_matplotlib_manager(fig):
+    """Create a new manager for a matplotlib figure."""
+    # create a dummy figure and use its
+    # manager to display "fig"  ; based on https://stackoverflow.com/a/54579616/8508004
+    dummy = plt.figure()
+    new_manager = dummy.canvas.manager
+    new_manager.canvas.figure = fig
+    fig.set_canvas(new_manager.canvas)
+    return fig
+
+
+def load_matplotlib_figure(filename, create_new_manager=False):
+    fig = pkl.load(open(filename, "rb"))
+    if create_new_manager:
+        fig = _make_matplotlib_manager(fig)
+    return fig
+
+
 def load_plotly_figure(filename):
     """Load plotly figure from file."""
     try:
         fig = pio.read_json(filename)
     except Exception as e:
         print("Could not load figure from json file")
         print(e)
@@ -359,21 +400,24 @@
 
         names = ["collector", self.collector_name]
         if self.nick:
             names.insert(0, self.nick)
         name = "_".join(names)
         return name
 
-    def render(self):
+    def render(self, **kwargs):
+        """Render the figure."""
+
+        kwargs = {**self.plotter_arguments, **kwargs}
         self.figure = self.plotter(
             self.data,
             backend=self.backend,
             journal=self.b.journal,
             units=self.units,
-            **self.plotter_arguments,
+            **kwargs,
         )
 
     def _parse_elevated_arguments(
         self, data_collector_arguments: dict = None, plotter_arguments: dict = None
     ):
         if data_collector_arguments is not None:
             logging.info(f"Updating elevated arguments")
@@ -436,14 +480,15 @@
         """Reset the arguments to the defaults.
 
         Args:
             data_collector_arguments (dict): optional additional keyword arguments for the data collector.
             plotter_arguments (dict): optional additional keyword arguments for the plotter.
 
         """
+        # warnings.warn("reset_arguments is deprecated", DeprecationWarning)
         self._data_collector_arguments = self._default_data_collector_arguments.copy()
         self._plotter_arguments = self._default_plotter_arguments.copy()
         self._update_arguments(data_collector_arguments, plotter_arguments)
 
     def parse_units(self, **kwargs):
         """Look through your cellpy objects and search for units."""
 
@@ -466,14 +511,25 @@
             print("WARNING: non-homogenous units found: cellpy_units")
         if len(r_units) > 1:
             print("WARNING: non-homogenous units found: raw_units")
         raw_units = r_units[0]
         cellpy_units = c_units[0]
         self.units = dict(raw_units=raw_units, cellpy_units=cellpy_units)
 
+    def collect(self, *args, **kwargs):
+        """Collect data."""
+        self.data = self.data_collector(
+            self.b, **self.data_collector_arguments, **kwargs
+        )
+        self.post_collect(*args, **kwargs)
+
+    def post_collect(self, *args, **kwargs):
+        """Perform post-operation after collecting the data"""
+        ...
+
     def update(
         self,
         data_collector_arguments: dict = None,
         plotter_arguments: dict = None,
         reset: bool = False,
         update_data: bool = False,
         update_name: bool = False,
@@ -492,15 +548,15 @@
         """
         if reset:
             self.reset_arguments(data_collector_arguments, plotter_arguments)
         else:
             self._update_arguments(data_collector_arguments, plotter_arguments)
         if update_data or self.data is None:
             try:
-                self.data = self.data_collector(self.b, **self.data_collector_arguments)
+                self.collect()
             except TypeError as e:
                 print("Type error:", e)
                 print("Registered data_collector_arguments:")
                 pprint(self.data_collector_arguments)
                 print("Hint: fix it and then re-run using reset=True")
                 return
         if update_plot:
@@ -522,15 +578,21 @@
             print("No figure to show!")
             return False
         return True
 
     def show(self, **kwargs):
         """Show the figure.
 
-        Notes:
+        Note:
+            If you are working in a Jupyter notebook and using a "matplotlib"-type backend,
+            the figure will most likely be shown automatically when the figure is rendered.
+            You should not need to use this method in that case, unless you want to
+            show the figure one extra time.
+
+        Note:
             The ``show`` method returns the ``figure`` object and  if the ``backend`` used
             does not provide automatic rendering in the editor / running environment you
             are using, you might have to issue the rendering yourself. For example, if you
             are using `plotly` and running it as a script in a typical command shell,
             you will have to issue ``.show()`` on the returned ``figure`` object.
 
         Args:
@@ -539,22 +601,31 @@
         Returns:
             Figure object
         """
 
         if not self._figure_valid():
             return
 
+        skip_render_for_seaborn = kwargs.pop("skip_render_for_seaborn", False)
+
         print(f"figure name: {self.name}")
         if kwargs:
             logging.info(f"updating figure with {kwargs}")
             self._update_arguments(plotter_arguments=kwargs)
             self.render()
 
         if self.backend == "seaborn":
-            return self.figure.figure
+            if not skip_render_for_seaborn:
+                return self.figure.figure
+            print(
+                "WARNING: skipping rendering for seaborn, assuming it is already rendered during the plotter call"
+            )
+            print(
+                "WARNING: if you want to show the figure, provide `skip_render_for_seaborn=False` as keyword argument"
+            )
         else:
             return self.figure
 
     def preprocess_data_for_csv(self):
         logging.debug(f"the data layout {self.csv_layout} is not supported yet!")
         return self.data
 
@@ -574,45 +645,45 @@
             data = self.data
 
         data.to_csv(
             filename,
             sep=self.sep,
             index=self.csv_include_index,
         )
-        print(f"saved csv file: {filename}")
+        print(f" - saved csv file: {filename}")
 
     def to_hdf5(self, serial_number=None):
         """Save to hdf5 file.
 
         Args:
             serial_number (int): serial number to append to the filename.
 
         """
 
         filename = self._output_path(serial_number)
         filename = filename.with_suffix(".h5")
         data = self.data
 
         data.to_hdf(filename, key=HDF_KEY, mode="w")
-        print(f"saved hdf5 file: {filename}")
+        print(f" - saved hdf5 file: {filename}")
 
     def _image_exporter_plotly(self, filename, timeout=IMAGE_TO_FILE_TIMEOUT, **kwargs):
         p = Process(
             target=self.figure.write_image,
             args=(filename,),
             name="save_plotly_image_to_file",
             kwargs=kwargs,
         )
         p.start()
         p.join(timeout=timeout)
         p.terminate()
         if p.exitcode is None:
             print(f"Oops, {p} timeouts! Could not save {filename}")
         if p.exitcode == 0:
-            print(f"saved image file: {filename}")
+            print(f" - saved image file: {filename}")
 
     def to_image_files(self, serial_number=None):
         """Save to image files (png, svg, json).
 
         Notes:
             This method requires ``kaleido`` for the plotly backend.
 
@@ -626,24 +697,32 @@
 
         if not self._figure_valid():
             return
         filename_pre = self._output_path(serial_number)
         filename_png = filename_pre.with_suffix(".png")
         filename_svg = filename_pre.with_suffix(".svg")
         filename_json = filename_pre.with_suffix(".json")
+        filename_pickle = filename_pre.with_suffix(".pickle")
 
         if self.backend == "plotly":
             self._image_exporter_plotly(filename_png, scale=3.0)
             self._image_exporter_plotly(filename_svg)
             self.figure.write_json(filename_json)
-            print(f"saved plotly json file: {filename_json}")
+            print(f" - saved plotly json file: {filename_json}")
         elif self.backend == "seaborn":
-            print(f"TODO: implement saving {filename_png}")
-            print(f"TODO: implement saving {filename_svg}")
-            print(f"TODO: implement saving {filename_json}")
+            self.figure.savefig(filename_png, dpi=self.dpi)
+            print(f" - saved png file: {filename_png}")
+            self.figure.savefig(filename_svg)
+            print(f" - saved svg file: {filename_svg}")
+            save_matplotlib_figure(self.figure, filename_pickle)
+            print(f" - pickled to file: {filename_pickle}")
+
+            # print(f"TODO: implement saving {filename_png}")
+            # print(f"TODO: implement saving {filename_svg}")
+            # print(f"TODO: implement saving {filename_json}")
         else:
             print(f"TODO: implement saving {filename_png}")
             print(f"TODO: implement saving {filename_svg}")
             print(f"TODO: implement saving {filename_json}")
 
     def save(self, serial_number=None):
         """Save to csv, hdf5 and image files.
@@ -1040,16 +1119,16 @@
             collector_type (str): how the curves are given
 
                 - "back-and-forth" - standard back and forth; discharge
                   (or charge) reversed from where charge (or discharge) ends.
                 - "forth" - discharge (or charge) continues along x-axis.
                 - "forth-and-forth" - discharge (or charge) also starts at 0.
 
-            data_collector_arguments (dict) - arguments transferred to the plotter
-            plotter_arguments (dict) - arguments transferred to the plotter
+            data_collector_arguments (dict) - arguments transferred to the to `CellpyCell.get_cap`.
+            plotter_arguments (dict) - arguments transferred to `cycles_plotter`.
             cycles (list): select these cycles (elevated data collector argument).
             max_cycle (int): drop all cycles above this value (elevated data collector argument).
             rate (float): filter on rate (C-rate) (elevated data collector argument).
             rate_on (str or list of str): only select cycles if based on the rate of this step-type (e.g. on="charge")
                 (elevated data collector argument).
             rate_std (float): allow for this inaccuracy when selecting cycles based on rate
                 (elevated data collector argument).
@@ -1057,15 +1136,15 @@
                 (elevated data collector argument).
             inverse (bool): select steps that do not have the given C-rate (elevated data collector argument).
             label_mapper (callable or dict): function (or dict) that changes the cell names
                 (elevated data collector argument).
                 The dictionary must have the cell labels as given in the `journal.pages` index and new label as values.
                 Similarly, if it is a function it takes the cell label as input and returns the new label.
                 Remark! No check are performed to ensure that the new cell labels are unique.
-            cycles_to_plot (int): plot points if True (elevated plotter argument).
+            cycles_to_plot (int): plot only these cycles (elevated plotter argument).
             width (float): width of plot (elevated plotter argument).
             legend_position (str): position of the legend (elevated plotter argument).
             show_legend (bool): set to False if you don't want to show legend (elevated plotter argument).
             fig_title (str): title (will be put above the figure) (elevated plotter argument).
             palette (str): color-map to use (elevated plotter argument).
             cols (int): number of columns (elevated plotter argument).
         """
@@ -1105,14 +1184,34 @@
             collector_name="cycles",
             elevated_data_collector_arguments=elevated_data_collector_arguments,
             elevated_plotter_arguments=elevated_plotter_arguments,
             *args,
             **kwargs,
         )
 
+    def post_collect(self, *args, **kwargs):
+        """Update the x-unit after collecting the data in case the mode has been set."""
+
+        logging.debug("updating the x-unit")
+        if m := self.data_collector_arguments.get("mode"):
+            if m == "gravimetric":
+                self.plotter_arguments["x_unit"] = (
+                    f'{self.units["cellpy_units"].charge}/{self.units["cellpy_units"].gravimetric}'
+                )
+            elif m == "areal":
+                self.plotter_arguments["x_unit"] = (
+                    f'{self.units["cellpy_units"].charge}/{self.units["cellpy_units"].areal}'
+                )
+            elif m == "volumetric":
+                self.plotter_arguments["x_unit"] = (
+                    f'{self.units["cellpy_units"].charge}/{self.units["cellpy_units"].volumetric}'
+                )
+            elif m == "absolute":
+                self.plotter_arguments["x_unit"] = self.units["cellpy_units"].charge
+
     def _dynamic_update_template_parameter(self, hv_opt, backend, *args, **kwargs):
         k = hv_opt.key
         if k == "NdLayout" and backend == "matplotlib":
             if self.plot_type != "fig_pr_cycle":
                 hv_opt.kwargs["fig_inches"] = self._max_letters_in_cell_names * 0.14
         return hv_opt
 
@@ -1206,14 +1305,15 @@
     inverse=False,
     interpolated=True,
     number_of_points=100,
     max_cycle=50,
     abort_on_missing=False,
     method="back-and-forth",
     label_mapper=None,
+    mode="gravimetric",
 ):
     """
     Collects cycles from all the cells in the batch object.
 
     Args:
         b: cellpy batch object
         cycles: list of cycle numbers to collect
@@ -1224,14 +1324,15 @@
         inverse: select steps that do not have the given C-rate.
         interpolated: if True, interpolate the data
         number_of_points: number of points to interpolate to
         max_cycle: drop all cycles above this value
         abort_on_missing: if True, abort if a cell is empty
         method: how the voltage curves are given (back-and-forth, forth, forth-and-forth)
         label_mapper: function (or dict) that changes the cell names.
+        mode (string): 'gravimetric', 'areal', 'volumetric' or 'absolute'.
 
     Returns:
         pd.DataFrame: collected data
     """
     if cycles is None:
         cycles = list(range(1, max_cycle + 1))
     all_curves = []
@@ -1248,14 +1349,15 @@
             cycles = list(set(filtered_cycles).intersection(set(cycles)))
         curves = c.get_cap(
             cycle=cycles,
             label_cycle_number=True,
             interpolated=interpolated,
             number_of_points=number_of_points,
             method=method,
+            mode=mode,
         )
         logging.debug(f"processing {n} (cell name: {c.cell_name})")
         if not curves.empty:
             curves = curves.assign(group=g, sub_group=sg)
             all_curves.append(curves)
             keys.append(n)
         else:
@@ -1530,15 +1632,15 @@
         histfunc (str): aggregation method.
         histscale (str): used for scaling the z-values for 2D array plots (heatmaps and similar).
         direction (str): "charge", "discharge", or "both".
         direction_col (str): name of columns containing information about direction ("charge" or "discharge").
         method: 'fig_pr_cell' or 'fig_pr_cycle'.
         markers: set to True if you want markers.
         group_cells (bool): give each cell within a group same color.
-        group_legend_muting (bool): if True, you can click on the legend to mute the whole group.
+        group_legend_muting (bool): if True, you can click on the legend to mute the whole group (only for plotly).
         backend (str): what backend to use.
         cycles: what cycles to include in the plot.
         palette_discrete: palette to use for discrete color mapping.
         palette_continuous: palette to use for continuous color mapping.
         palette_range (tuple): range of palette to use for continuous color mapping (from 0 to 1).
         facetplot (bool): square layout with group horizontally and subgroup vertically.
         cols (int): number of columns for layout.
@@ -1558,17 +1660,15 @@
         logging.debug(f"keyword argument sent to the backend: {k}")
     if backend not in supported_backends:
         print(f"Backend '{backend}' not supported", end="")
         print(f" - supported backends: {supported_backends}")
         return
     curves = None
 
-    plotly_arguments = dict()
-    seaborn_arguments = dict()
-    seaborn_post_plot_operations = dict()
+    # ----------------- parsing arguments -----------------------------
 
     if method == "film":
         labels = {
             f"{x}": f"{x_label} ({x_unit})",
             f"{z}": f"{z_label} ({z_unit})",
         }
         plotly_arguments = dict(
@@ -1577,41 +1677,45 @@
             z=y,
             labels=labels,
             facet_col_wrap=cols,
             nbinsx=nbinsx,
             histfunc=histfunc,
         )
 
+        seaborn_arguments = dict(x=x, y=z, z=y, labels=labels, row=g, col=subgroup)
+
     elif method == "summary":
         labels = {
             f"{x}": f"{x_label} ({x_unit})",
         }
         plotly_arguments = dict(x=x, y=y, labels=labels, markers=markers)
         seaborn_arguments = dict(x=x, y=y, markers=markers)
-        seaborn_post_plot_operations["labels"] = labels
+        seaborn_arguments["labels"] = labels
 
         if g == "variable" and len(collected_curves[g].unique()) > 1:
             plotly_arguments["facet_row"] = g
             seaborn_arguments["row"] = g
         if standard_deviation:
             plotly_arguments["error_y"] = standard_deviation
-            seaborn_post_plot_operations["error_y"] = standard_deviation
+            seaborn_arguments["error_y"] = standard_deviation
 
     else:
         labels = {
             f"{x}": f"{x_label} ({x_unit})",
             f"{y}": f"{y_label} ({y_unit})",
         }
         plotly_arguments = dict(x=x, y=y, labels=labels, facet_col_wrap=cols)
+        seaborn_arguments = dict(x=x, y=y, labels=labels, row=group, col=subgroup)
 
     if method in ["fig_pr_cell", "film"]:
         group_cells = False
         if method == "fig_pr_cell":
             plotly_arguments["markers"] = markers
             plotly_arguments["color"] = z
+            seaborn_arguments["hue"] = z
         if facetplot:
             plotly_arguments["facet_col"] = group
             plotly_arguments["facet_row"] = subgroup
             plotly_arguments["hover_name"] = g
         else:
             plotly_arguments["facet_col"] = g
 
@@ -1634,14 +1738,15 @@
                 curves[y] = curves[y].apply(np.abs)
             elif histscale == "norm":
                 curves[y] = curves[y].apply(np.abs)
 
     elif method == "fig_pr_cycle":
         z, g = g, z
         plotly_arguments["facet_col"] = g
+        seaborn_arguments["col"] = g
 
         if cycles is not None:
             curves = collected_curves.loc[collected_curves.cycle.isin(cycles), :]
         else:
             curves = collected_curves
 
         if group_cells:
@@ -1667,14 +1772,18 @@
             plotly_arguments["symbol"] = subgroup
             seaborn_arguments["hue"] = group
             seaborn_arguments["style"] = subgroup
         else:
             plotly_arguments["color"] = z
             seaborn_arguments["hue"] = z
 
+    # ----------------- individual plotting calls  -----------------------------
+    # TODO: move as much as possible up to the parsing of arguments
+    #   (i.e. prepare for future refactoring)
+
     if backend == "plotly":
         if method == "fig_pr_cell":
             start, end = 0.0, 1.0
             if palette_range is not None:
                 start, end = palette_range
             unique_cycle_numbers = curves[z].unique()
             number_of_colors = len(unique_cycle_numbers)
@@ -1803,111 +1912,139 @@
                         print(e)
 
         else:
             print(f"method '{method}' is not supported by plotly")
 
         return fig
 
-    elif backend == "seaborn":
-        # {'x': 'cycle', 'y': 'mean', 'labels': {'cycle': 'Cycle (n.)'}, 'markers': False, 'error_y': 'std'}
-        sns.set_theme(style="darkgrid")
-        # seaborn_arguments = dict(
-        #     data=curves,
-        #     x="cycle",
-        #     y="mean",
-        #     hue="cell",
-        #     size=None,
-        #     style=None,
-        #     units=None,
-        #     row=None,
-        #     col=None,
-        #     col_wrap=None,
-        #     row_order=None,
-        #     col_order=None,
-        #     palette="Set1",
-        #     hue_order=None,
-        #     hue_norm=None,
-        #     sizes=None,
-        #     size_order=None,
-        #     size_norm=None,
-        #     markers=True,
-        #     dashes=None,
-        #     style_order=None,
-        #     legend="auto",
-        #     kind="line",
-        #     height=3,
-        #     aspect=3,
-        #     facet_kws=None,
-        #     linewidth=2.0,
-        #     **kwargs,
-        # )
-
-        if not seaborn_arguments.get("marker"):
-            seaborn_arguments["dashes"] = False
-        seaborn_arguments["kind"] = "line"
-        seaborn_arguments["height"] = 3
-        seaborn_arguments["aspect"] = 3
-        seaborn_arguments["linewidth"] = 2.0
-        seaborn_arguments["facet_kws"] = {
-            "sharex": True,
-            "sharey": False,
-            "legend_out": True,
-        }
-        print(f"{seaborn_arguments=}\n{kwargs=}")
-        print(f"{seaborn_post_plot_operations=}")
-        print(curves)
-
-        fig_grid = sns.relplot(
-            data=curves,
-            **seaborn_arguments,
-            **kwargs,
-        )
+    if backend == "seaborn":
+        number_of_data_points = len(curves)
+        if number_of_data_points > MAX_POINTS_SEABORN_FACET_GRID:
+            print(
+                f"WARNING! Too many data points for seaborn to plot: {number_of_data_points}"
+            )
+            print(
+                f"  - Try to reduce the number of data points (e.g. by selecting fewer cycles and interpolating)"
+            )
+            return
+
+        if method == "fig_pr_cell":
+            seaborn_arguments["height"] = kwargs.pop("height", 3)
+            seaborn_arguments["aspect"] = kwargs.pop("height", 1)
+            sns.set_theme(style="darkgrid")
+            x = seaborn_arguments.get("x", "capacity")
+            y = seaborn_arguments.get("y", "voltage")
+            row = seaborn_arguments.get("row", "group")
+            hue = seaborn_arguments.get("hue", "cycle")
+            col = seaborn_arguments.get("col", "sub_group")
+            height = seaborn_arguments.get("height", 3)
+            aspect = seaborn_arguments.get("aspect", 1)
+
+            if palette_discrete is not None:
+                seaborn_arguments["palette"] = getattr(
+                    sns.color_palette, palette_discrete
+                )
+            g = sns.FacetGrid(
+                curves,
+                hue=hue,
+                row=row,
+                col=col,
+                height=height,
+                aspect=aspect,
+            )
+            g.map(plt.plot, x, y)
+            fig = g.fig
+            g.set_xlabels(labels[x])
+            g.set_ylabels(labels[y])
+            g.add_legend()
+            return fig
+
+        if method == "fig_pr_cycle":
+            sns.set_theme(style="darkgrid")
+            seaborn_arguments["height"] = 4
+            seaborn_arguments["aspect"] = 3
+            seaborn_arguments["linewidth"] = 2.0
+            g = sns.FacetGrid(
+                curves,
+                hue=z,
+                height=seaborn_arguments["height"],
+                aspect=seaborn_arguments["aspect"],
+            )
+            g.map(plt.plot, x, y)
+            fig = g.fig
+            g.set_xlabels(x_label)
+            g.set_ylabels(y_label)
+            g.add_legend()
+            return fig
+
+        if method == "film":
+            sns.set_theme(style="darkgrid")
+            seaborn_arguments["height"] = 4
+            seaborn_arguments["aspect"] = 3
+            seaborn_arguments["linewidth"] = 2.0
+            g = sns.FacetGrid(
+                curves,
+                hue=z,
+                height=seaborn_arguments["height"],
+                aspect=seaborn_arguments["aspect"],
+            )
+            g.map(
+                sns.kdeplot,
+                y,
+                x,
+                fill=True,
+                thresh=0,
+                levels=100,
+                cmap=palette_continuous,
+            )
+            fig = g.fig
+            g.set_xlabels(x_label)
+            g.set_ylabels(y_label)
+            g.add_legend()
+            return fig
+
+        if method == "summary":
+            sns.set_theme(style="darkgrid")
+            seaborn_arguments["height"] = 4
+            seaborn_arguments["aspect"] = 3
+            seaborn_arguments["linewidth"] = 2.0
+
+            x = seaborn_arguments.get("x", "cycle")
+            y = seaborn_arguments.get("y", "mean")
+            hue = seaborn_arguments.get("hue", None)
+
+            labels = seaborn_arguments.get("labels", None)
+            x_label = labels.get(x, x)
+
+            std = seaborn_arguments.get("error_y", None)
+            marker = "o" if seaborn_arguments.get("markers", False) else None
+            row = seaborn_arguments.get("row", None)
+
+            g = sns.FacetGrid(
+                curves,
+                hue=hue,
+                height=seaborn_arguments["height"],
+                aspect=seaborn_arguments["aspect"],
+                row=row,
+            )
 
-        # if group_cells:
-        #     try:
-        #         fig.for_each_trace(
-        #             functools.partial(
-        #                 legend_replacer,
-        #                 df=curves,
-        #                 group_legends=group_legend_muting,
-        #             )
-        #         )
-        #         if markers is not True:
-        #             fig.for_each_trace(remove_markers)
-        #     except Exception as e:
-        #         print("failed")
-        #         print(e)
-        #
-        # if y_label_mapper:
-        #     annotations = fig.layout.annotations
-        #     if annotations:
-        #         try:
-        #             # might consider a more robust method here - currently
-        #             # it assumes that the mapper is a list with same order
-        #             # and length as number of rows
-        #             for i, (a, la) in enumerate(zip(annotations, y_label_mapper)):
-        #                 row = i + 1
-        #                 fig.for_each_yaxis(
-        #                     functools.partial(y_axis_replacer, label=la),
-        #                     row=row,
-        #                 )
-        #             fig.update_annotations(text="")
-        #         except Exception as e:
-        #             print("failed")
-        #             print(e)
-        #     else:
-        #         try:
-        #             fig.for_each_yaxis(
-        #                 functools.partial(y_axis_replacer, label=y_label_mapper[0]),
-        #             )
-        #         except Exception as e:
-        #             print("failed")
-        #             print(e)
+            if std:
+                g.map(plt.errorbar, x, y, std, marker=marker, elinewidth=0.5, capsize=2)
+            else:
+                g.map(plt.plot, x, y, marker=marker)
+
+            fig = g.figure
+
+            g.set_xlabels(x_label)
+            if y_label_mapper:
+                for i, ax in enumerate(g.axes.flat):
+                    ax.set_ylabel(y_label_mapper[i])
+            g.add_legend()
+            return fig
 
-        return fig_grid
     elif backend == "matplotlib":
         print(f"{backend} not implemented yet")
 
     elif backend == "bokeh":
         print(f"{backend} not implemented yet")
 
     else:
@@ -1982,15 +2119,14 @@
     else:
         number_of_figs = 1
 
     no_rows = math.ceil(number_of_figs / no_cols)
 
     if not height:
         height = no_rows * sub_fig_min_height
-
     fig = sequence_plotter(
         collected_curves,
         x=x,
         y=y,
         z=z,
         g=g,
         standard_deviation=standard_deviation,
@@ -2040,15 +2176,14 @@
 def summary_plotter(collected_curves, cycles_to_plot=None, backend="plotly", **kwargs):
     """Plot summaries (value vs cycle number).
 
     Assuming data as pandas.DataFrame with either
     1) long format (where variables, for example charge capacity, are in the column "variable") or
     2) mixed long and wide format where the variables are own columns.
     """
-
     col_headers = collected_curves.columns.to_list()
     possible_id_vars = [
         "cell",
         "cycle",
         "equivalent_cycle",
         "value",
         "mean",
@@ -2138,53 +2273,68 @@
         default_title="Summary Plot",
         backend=backend,
         method="summary",
         cycles=cycles_to_plot,
         cols=cols,
         **kwargs,
     )
+
     if backend == "plotly":
         fig.update_yaxes(matches=None, showticklabels=True)
-    elif backend == "seaborn":
+        return fig
+    if backend == "seaborn":
         print("using seaborn (experimental feature)")
-    return fig
+        return fig
+    if backend == "matplotlib":
+        print("using matplotlib (experimental feature)")
+        return fig
+    if backend == "bokeh":
+        print("using bokeh (experimental feature)")
+        return fig
 
 
 def cycles_plotter(
     collected_curves,
     cycles_to_plot=None,
     backend="plotly",
     method="fig_pr_cell",
+    x_unit="mAh/g",
+    y_unit="V",
     **kwargs,
 ):
     """Plot charge-discharge curves.
 
     Args:
         collected_curves(pd.DataFrame): collected data in long format.
         cycles_to_plot (list): cycles to plot
         backend (str): what backend to use.
         method (str): 'fig_pr_cell' or 'fig_pr_cycle'.
+        x_unit (str): unit for x-axis.
+        y_unit (str): unit for y-axis.
 
         **kwargs: consumed first in current function, rest sent to backend in sequence_plotter.
 
     Returns:
         styled figure object
     """
 
     if cycles_to_plot is not None:
         unique_cycles = list(collected_curves.cycle.unique())
         if len(unique_cycles) > 50:
+            print(f"Too many cycles - setting it to default {DEFAULT_CYCLES}")
             cycles_to_plot = DEFAULT_CYCLES
 
     return _cycles_plotter(
         collected_curves,
         x="capacity",
         y="voltage",
         z="cycle",
         g="cell",
+        x_unit=x_unit,
+        y_unit=y_unit,
         default_title="Charge-Discharge Curves",
         backend=backend,
         method=method,
         cycles=cycles_to_plot,
         **kwargs,
     )
```

### Comparing `cellpy-1.0.1b5/cellpy/utils/easyplot.py` & `cellpy-1.0.2a1/cellpy/utils/easyplot.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/utils/example_data.py` & `cellpy-1.0.2a1/cellpy/utils/example_data.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/utils/helpers.py` & `cellpy-1.0.2a1/cellpy/utils/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     get_headers_journal,
     get_headers_summary,
     get_headers_step_table,
     get_headers_normal,
 )
 from cellpy.readers.cellreader import CellpyCell
 from cellpy.utils.batch import Batch
+from cellpy.internals.core import check_connection as _check_connection
 
 hdr_summary = get_headers_summary()
 hdr_steps = get_headers_step_table()
 hdr_normal = get_headers_normal()
 hdr_journal = get_headers_journal()
 
 
@@ -1310,14 +1311,18 @@
         cell.data.summary[norm_col_name] = (
             scale * cell.data.summary[col_name] / norm_value
         )
 
     return cell
 
 
+def check_connection(path=None):
+    return _check_connection(path)
+
+
 def load_and_save_resfile(filename, outfile=None, outdir=None, mass=1.00):
     """Load a raw data file and save it as cellpy-file.
 
     Args:
         mass (float): active material mass [mg].
         outdir (path): optional, path to directory for saving the hdf5-file.
         outfile (str): optional, name of hdf5-file.
@@ -1344,7 +1349,26 @@
     d.from_raw(filename)
     d.set_mass(mass)
     d.make_step_table()
     d.make_summary()
     d.save(filename=outfile)
     d.to_csv(datadir=outdir, cycles=True, raw=True, summary=True)
     return outfile
+
+
+def _check():
+    print("Testing OtherPath-connection")
+    info = check_connection()
+    # p0 = "scp://odin/home/jepe@ad.ife.no/projects"
+    # info = check_connection(p0)
+    # p1 = "scp://odin/home/jepe@ad.ife.no/this-folder-does-not-exist"
+    # info = check_connection(p1)
+    # p2 = pathlib.Path(".").resolve()
+    # info = check_connection(p2)
+    # p3 = "scp://odin/home/evil@ad.ife.no/projects"
+    # info = check_connection(p3)
+    # p4 = "scp://madmax/home/evil@ad.ife.no/projects"
+    # info = check_connection(p4)
+
+
+if __name__ == "__main__":
+    _check()
```

### Comparing `cellpy-1.0.1b5/cellpy/utils/ica.py` & `cellpy-1.0.2a1/cellpy/utils/ica.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/utils/ocv_rlx.py` & `cellpy-1.0.2a1/cellpy/utils/ocv_rlx.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy/utils/plotutils.py` & `cellpy-1.0.2a1/cellpy/utils/plotutils.py`

 * *Files 10% similar despite different names*

```diff
@@ -452,70 +452,167 @@
     cell,
     y=None,
     y_label=None,
     x=None,
     x_label=None,
     title=None,
     interactive=True,
+    plot_type="voltage-current",
+    double_y=True,
+    return_matplotlib_figure=False,
     **kwargs,
 ):
     """Plot raw data.
 
     Args:
         cell: cellpy object
-        y: y-axis column
-        y_label: label for y-axis
-        x: x-axis column
-        x_label: label for x-axis
-        title: title of the plot
-        interactive: use interactive plotting
+        y (str or list): y-axis column
+        y_label (str or list): label for y-axis
+        x (str): x-axis column
+        x_label (str): label for x-axis
+        title (str): title of the plot
+        interactive (bool): use interactive plotting
+        plot_type (str): type of plot (defaults to "voltage-current") (overrides given y if y is not None),
+          currently only "voltage-current" is supported.
+        double_y (bool): use double y-axis (only for matplotlib and when plot_type is used)
+        return_matplotlib_figure (bool): return a matplotlib figure (only for matplotlib)
         **kwargs: additional parameters for the plotting backend
 
     Returns:
         ``matplotlib`` figure or ``plotly`` figure
 
     """
 
+    _set_individual_y_labels = False
+
     raw = cell.data.raw.copy()
+    if y is not None:
+        if y_label is None:
+            y_label = y
+        y = [y]
+        y_label = [y_label]
+
+    elif plot_type is not None:
+        # special pre-defined plot types
+        if plot_type == "voltage-current":
+            y1 = _hdr_raw["voltage_txt"]
+            y1_label = f"Voltage ({cell.data.raw_units.voltage})"
+            y2 = _hdr_raw["current_txt"]
+            y2_label = f"Current ({cell.data.raw_units.current})"
+            y = [y1, y2]
+            y_label = [y1_label, y2_label]
+        else:
+            warnings.warn(f"Plot type {plot_type} not supported")
+            return None
+    else:
+        # default to voltage if y is not given
+        y = [_hdr_raw["voltage_txt"]]
+        y_label = [f"Voltage ({cell.data.raw_units.voltage})"]
 
-    if y is None:
-        y, y_label = ("voltage", f"Voltage ({cell.data.raw_units.voltage})")
     if x is None:
         x, x_label = ("test_time_hrs", "Time (hours)")
 
     if title is None:
         title = f"{cell.cell_name}"
 
     if x == "test_time_hrs":
         raw["test_time_hrs"] = raw[_hdr_raw["test_time_txt"]] / 3600
 
     if plotly_available and interactive:
-        import plotly.express as px
-
         title = f"<b>{title}</b>"
-        if x_label or y_label:
-            labels = {}
-            if x_label:
-                labels[x] = x_label
-            if y_label:
-                labels[y] = y_label
+        if len(y) == 1:
+            # single plot
+            import plotly.express as px
+
+            if x_label or y_label:
+                labels = {}
+                if x_label:
+                    labels[x] = x_label
+                if y_label:
+                    labels[y[0]] = y_label[0]
+            else:
+                labels = None
+            fig = px.line(raw, x=x, y=y[0], title=title, labels=labels, **kwargs)
+
         else:
-            labels = None
-        fig = px.line(raw, x=x, y=y, title=title, labels=labels, **kwargs)
+            # double plot
+            from plotly.subplots import make_subplots
+            import plotly.graph_objects as go
+
+            fig = make_subplots(
+                rows=2,
+                cols=1,
+                shared_xaxes=True,
+                vertical_spacing=0.02,
+                x_title=x_label,
+            )
+            x_values = raw[x]
+            fig.add_trace(
+                go.Scatter(x=x_values, y=raw[y[0]], name=y_label[0]),
+                row=1,
+                col=1,
+            )
+            fig.add_trace(
+                go.Scatter(x=x_values, y=raw[y[1]], name=y_label[1]),
+                row=2,
+                col=1,
+            )
+
+            fig.update_layout(height=600, title_text=title)
+            if _set_individual_y_labels:
+                fig.update_yaxes(title_text=y_label[0], row=1, col=1)
+                fig.update_yaxes(title_text=y_label[1], row=2, col=1)
 
         return fig
 
     # default to a simple matplotlib figure
-    fig, ax = plt.subplots()
-    ax.plot(raw[x], raw[y])
-    ax.set_xlabel(x_label)
-    ax.set_ylabel(y_label)
-    ax.set_title(title)
+    xlim = kwargs.get("xlim")
+    if len(y) == 1:
+        y = y[0]
+        y_label = y_label[0]
+        fig, ax = plt.subplots()
+        ax.plot(raw[x], raw[y])
+        ax.set_xlabel(x_label)
+        ax.set_ylabel(y_label)
+        ax.set_title(title)
+        ax.set_xlim(xlim)
+        if return_matplotlib_figure:
+            return fig
+        return
+
+    if not double_y:
+        fig, (ax_v, ax_c) = plt.subplots(nrows=2, ncols=1, figsize=(20, 8), sharex=True)
+        ax_v.plot(raw[x], raw[y[0]])
+        ax_c.plot(raw[x], raw[y[1]])
+        ax_v.set_ylabel(y_label[0])
+        ax_c.set_ylabel(y_label[1])
+        ax_c.set_xlabel(x_label)
+        ax_v.set_title(title)
+        ax_v.set_xlim(xlim)
+    else:
+        fig, ax_v = plt.subplots(figsize=(12, 4))
+
+        color = "tab:red"
+        ax_v.set_xlabel(x_label)
+        ax_v.set_ylabel(y_label[0], color=color)
+        ax_v.plot(raw[x], raw[y[0]], label=y_label[0], color=color)
+        ax_v.tick_params(axis="y", labelcolor=color)
+
+        ax_c = ax_v.twinx()
+
+        color = "tab:blue"
+        ax_c.set_ylabel(y_label[1], color=color)
+        ax_c.plot(raw[x], raw[y[1]], label=y_label[1], color=color)
+        ax_c.tick_params(axis="y", labelcolor=color)
+        ax_v.set_xlim(xlim)
 
-    return ax
+        fig.tight_layout()
+    if return_matplotlib_figure:
+        return fig
+    return
 
 
 def cycle_info_plot(
     cell,
     cycle=None,
     get_axes=False,
     interactive=True,
```

### Comparing `cellpy-1.0.1b5/cellpy/utils/processor.py` & `cellpy-1.0.2a1/cellpy/utils/processor.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/cellpy.egg-info/PKG-INFO` & `cellpy-1.0.2a1/cellpy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellpy
-Version: 1.0.1b5
+Version: 1.0.2a1
 Summary: Extract and manipulate data from battery data testers.
 Home-page: https://github.com/jepegit/cellpy
 Author: Jan Petter Maehlen
 Author-email: jepe@ife.no
 License: MIT license
 Keywords: cellpy
 Classifier: Development Status :: 5 - Production/Stable
@@ -112,15 +112,15 @@
 Contributions are welcome, and they are greatly appreciated! Every
 little bit helps, and credit will always be given. If you want to contribute,
 please have a look at [Contributing Guidelines](CONTRIBUTING.md).
 
 
 # History
 
-## 1.0.1 (under development)
+## 1.0.1
 
 * Utils: `example_data` now includes auto-download of example data
 * General: supports only python 3.10 and up to 3.11
 * Batch: `naked` and `init(empty=True)` easier method for creating batch with empty pages
 * File handling: new fix in `find_files`
 * Batch / Utils: refactored and updated `Collectors` (using `plotly`)
 * Batch: new summary plotter (using `plotly`)
@@ -131,19 +131,17 @@
 * Added possibility to filter on C-rates (`c.get_cycles`)
 * Added experimental feature `c.total_time_at_voltage_level` for calculating total time at low/high voltage
 * Added experimental instrument reader for neware xlsx files (hopefully not used much because it is very slow)
 * Added try-except block for ica post-processing step and add if-clause (suggested by Vajee)
 * Fixed several smaller bugs and improved some of the functionality (most notably in `c.get_cap`)
 * Added CI for macOS
 * Added conda package including `sqlalchemy-access`
-* [under progress]: check how cycle_mode and specific is handled and possibly improve
-* [under progress]: start moving/implementing all methods that modify the data to the `do` module
-* [under progress]: improve plotting tools
-* [under progress]: improve documentation
-* [under progress]: improve feedback from the CLI
+* Improved plotting tools
+* Improved documentation
+* Improved feedback from the CLI
 
 ## 1.0.0 (2023)
 
 * Unit handling: new unit handling (using pint)
 * Unit handling: renaming summary headers
 * Unit handling: new cellpy-file-format version
 * Unit handling: tool for converting old to new format
```

### Comparing `cellpy-1.0.1b5/cellpy.egg-info/SOURCES.txt` & `cellpy-1.0.2a1/cellpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b5/setup.py` & `cellpy-1.0.2a1/setup.py`

 * *Files identical despite different names*

