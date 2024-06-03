# Comparing `tmp/validation_framework-0.1.0.tar.gz` & `tmp/validation_framework-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "validation_framework-0.1.0.tar", last modified: Mon Jun  3 01:39:03 2024, max compression
+gzip compressed data, was "validation_framework-0.1.1.tar", last modified: Mon Jun  3 02:13:59 2024, max compression
```

## Comparing `validation_framework-0.1.0.tar` & `validation_framework-0.1.1.tar`

### file list

```diff
@@ -1,82 +1,81 @@
-drwxrwxrwx   0        0        0        0 2024-06-03 01:39:03.584156 validation_framework-0.1.0/
--rw-rw-rw-   0        0        0      570 2024-06-03 01:39:03.566158 validation_framework-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-06-03 00:57:05.000000 validation_framework-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-06-03 01:39:03.585157 validation_framework-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      879 2024-06-03 01:38:02.000000 validation_framework-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-03 01:39:02.950611 validation_framework-0.1.0/validation/
--rw-rw-rw-   0        0        0        0 2024-06-03 01:38:34.000000 validation_framework-0.1.0/validation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-03 01:39:02.968139 validation_framework-0.1.0/validation/aider/
--rw-rw-rw-   0        0        0        0 2024-06-03 01:37:12.000000 validation_framework-0.1.0/validation/aider/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-03 01:39:03.157350 validation_framework-0.1.0/validation/aider/aider/
--rw-rw-rw-   0        0        0       28 2024-06-03 01:29:25.000000 validation_framework-0.1.0/validation/aider/aider/__init__.py
--rw-rw-rw-   0        0        0    13976 2024-06-03 01:29:25.000000 validation_framework-0.1.0/validation/aider/aider/args.py
-drwxrwxrwx   0        0        0        0 2024-06-03 01:39:03.314252 validation_framework-0.1.0/validation/aider/aider/coders/
--rw-rw-rw-   0        0        0      624 2024-06-03 01:29:25.000000 validation_framework-0.1.0/validation/aider/aider/coders/__init__.py
--rw-rw-rw-   0        0        0    45295 2024-06-03 01:29:25.000000 validation_framework-0.1.0/validation/aider/aider/coders/base_coder.py
--rw-rw-rw-   0        0        0     1625 2024-06-03 01:29:25.000000 validation_framework-0.1.0/validation/aider/aider/coders/base_prompts.py
--rw-rw-rw-   0        0        0    15675 2024-06-03 01:29:25.000000 validation_framework-0.1.0/validation/aider/aider/coders/editblock_coder.py
--rw-rw-rw-   0        0        0      368 2024-06-03 01:29:25.000000 validation_framework-0.1.0/validation/aider/aider/coders/editblock_fenced_coder.py
--rw-rw-rw-   0        0        0     1887 2024-06-03 01:29:25.000000 validation_framework-0.1.0/validation/aider/aider/coders/editblock_fenced_prompts.py
--rw-rw-rw-   0        0        0     5458 2024-06-03 01:29:25.000000 validation_framework-0.1.0/validation/aider/aider/coders/editblock_func_coder.py
--rw-rw-rw-   0        0        0      913 2024-06-03 01:29:26.000000 validation_framework-0.1.0/validation/aider/aider/coders/editblock_func_prompts.py
--rw-rw-rw-   0        0        0     4498 2024-06-03 01:29:26.000000 validation_framework-0.1.0/validation/aider/aider/coders/editblock_prompts.py
--rw-rw-rw-   0        0        0    20773 2024-06-03 01:29:26.000000 validation_framework-0.1.0/validation/aider/aider/coders/search_replace.py
--rw-rw-rw-   0        0        0     3508 2024-06-03 01:29:26.000000 validation_framework-0.1.0/validation/aider/aider/coders/single_wholefile_func_coder.py
--rw-rw-rw-   0        0        0      894 2024-06-03 01:29:26.000000 validation_framework-0.1.0/validation/aider/aider/coders/single_wholefile_func_prompts.py
--rw-rw-rw-   0        0        0    11127 2024-06-03 01:29:26.000000 validation_framework-0.1.0/validation/aider/aider/coders/udiff_coder.py
--rw-rw-rw-   0        0        0     3316 2024-06-03 01:29:26.000000 validation_framework-0.1.0/validation/aider/aider/coders/udiff_prompts.py
--rw-rw-rw-   0        0        0     5293 2024-06-03 01:29:26.000000 validation_framework-0.1.0/validation/aider/aider/coders/wholefile_coder.py
--rw-rw-rw-   0        0        0     4367 2024-06-03 01:29:26.000000 validation_framework-0.1.0/validation/aider/aider/coders/wholefile_func_coder.py
--rw-rw-rw-   0        0        0      895 2024-06-03 01:29:26.000000 validation_framework-0.1.0/validation/aider/aider/coders/wholefile_func_prompts.py
--rw-rw-rw-   0        0        0     1913 2024-06-03 01:29:26.000000 validation_framework-0.1.0/validation/aider/aider/coders/wholefile_prompts.py
--rw-rw-rw-   0        0        0    24693 2024-06-03 01:29:26.000000 validation_framework-0.1.0/validation/aider/aider/commands.py
--rw-rw-rw-   0        0        0     3189 2024-06-03 01:29:26.000000 validation_framework-0.1.0/validation/aider/aider/diffs.py
--rw-rw-rw-   0        0        0      682 2024-06-03 01:29:26.000000 validation_framework-0.1.0/validation/aider/aider/dump.py
--rw-rw-rw-   0        0        0    17857 2024-06-03 01:29:26.000000 validation_framework-0.1.0/validation/aider/aider/gui.py
--rw-rw-rw-   0        0        0     3831 2024-06-03 01:29:26.000000 validation_framework-0.1.0/validation/aider/aider/history.py
--rw-rw-rw-   0        0        0    12525 2024-06-03 01:29:26.000000 validation_framework-0.1.0/validation/aider/aider/io.py
--rw-rw-rw-   0        0        0     6603 2024-06-03 01:29:26.000000 validation_framework-0.1.0/validation/aider/aider/linter.py
--rw-rw-rw-   0        0        0      316 2024-06-03 01:29:26.000000 validation_framework-0.1.0/validation/aider/aider/litellm.py
--rw-rw-rw-   0        0        0    14170 2024-06-03 01:29:26.000000 validation_framework-0.1.0/validation/aider/aider/main.py
--rw-rw-rw-   0        0        0     3047 2024-06-03 01:29:26.000000 validation_framework-0.1.0/validation/aider/aider/mdstream.py
--rw-rw-rw-   0        0        0    16123 2024-06-03 01:29:26.000000 validation_framework-0.1.0/validation/aider/aider/models.py
--rw-rw-rw-   0        0        0     2174 2024-06-03 01:29:26.000000 validation_framework-0.1.0/validation/aider/aider/prompts.py
--rw-rw-rw-   0        0        0     8129 2024-06-03 01:29:26.000000 validation_framework-0.1.0/validation/aider/aider/repo.py
--rw-rw-rw-   0        0        0    16125 2024-06-03 01:29:26.000000 validation_framework-0.1.0/validation/aider/aider/repomap.py
--rw-rw-rw-   0        0        0     5621 2024-06-03 01:29:26.000000 validation_framework-0.1.0/validation/aider/aider/scrape.py
--rw-rw-rw-   0        0        0     2239 2024-06-03 01:29:26.000000 validation_framework-0.1.0/validation/aider/aider/sendchat.py
--rw-rw-rw-   0        0        0     4413 2024-06-03 01:29:26.000000 validation_framework-0.1.0/validation/aider/aider/utils.py
--rw-rw-rw-   0        0        0     1052 2024-06-03 01:29:26.000000 validation_framework-0.1.0/validation/aider/aider/versioncheck.py
--rw-rw-rw-   0        0        0     2817 2024-06-03 01:29:26.000000 validation_framework-0.1.0/validation/aider/aider/voice.py
-drwxrwxrwx   0        0        0        0 2024-06-03 01:39:03.404450 validation_framework-0.1.0/validation/aider/benchmark/
--rw-rw-rw-   0        0        0        0 2024-06-03 01:29:27.000000 validation_framework-0.1.0/validation/aider/benchmark/__init__.py
--rw-rw-rw-   0        0        0    22214 2024-06-03 01:29:27.000000 validation_framework-0.1.0/validation/aider/benchmark/benchmark.py
--rw-rw-rw-   0        0        0     1885 2024-06-03 01:29:27.000000 validation_framework-0.1.0/validation/aider/benchmark/over_time.py
--rw-rw-rw-   0        0        0    11842 2024-06-03 01:29:27.000000 validation_framework-0.1.0/validation/aider/benchmark/plots.py
--rw-rw-rw-   0        0        0      469 2024-06-03 01:29:27.000000 validation_framework-0.1.0/validation/aider/benchmark/prompts.py
--rw-rw-rw-   0        0        0     6662 2024-06-03 01:29:27.000000 validation_framework-0.1.0/validation/aider/benchmark/refactor_tools.py
--rw-rw-rw-   0        0        0     1415 2024-06-03 01:29:27.000000 validation_framework-0.1.0/validation/aider/benchmark/rungrid.py
--rw-rw-rw-   0        0        0     3752 2024-06-03 01:29:27.000000 validation_framework-0.1.0/validation/aider/benchmark/swe_bench.py
--rw-rw-rw-   0        0        0     1582 2024-06-03 01:29:27.000000 validation_framework-0.1.0/validation/aider/benchmark/test_benchmark.py
--rw-rw-rw-   0        0        0     1532 2024-06-03 01:29:28.000000 validation_framework-0.1.0/validation/aider/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-03 01:39:03.510772 validation_framework-0.1.0/validation/aider/tests/
--rw-rw-rw-   0        0        0        0 2024-06-03 01:29:28.000000 validation_framework-0.1.0/validation/aider/tests/__init__.py
--rw-rw-rw-   0        0        0    19321 2024-06-03 01:29:28.000000 validation_framework-0.1.0/validation/aider/tests/test_coder.py
--rw-rw-rw-   0        0        0    20626 2024-06-03 01:29:28.000000 validation_framework-0.1.0/validation/aider/tests/test_commands.py
--rw-rw-rw-   0        0        0    11695 2024-06-03 01:29:28.000000 validation_framework-0.1.0/validation/aider/tests/test_editblock.py
--rw-rw-rw-   0        0        0     2664 2024-06-03 01:29:28.000000 validation_framework-0.1.0/validation/aider/tests/test_io.py
--rw-rw-rw-   0        0        0     9531 2024-06-03 01:29:28.000000 validation_framework-0.1.0/validation/aider/tests/test_main.py
--rw-rw-rw-   0        0        0      830 2024-06-03 01:29:28.000000 validation_framework-0.1.0/validation/aider/tests/test_models.py
--rw-rw-rw-   0        0        0    10570 2024-06-03 01:29:28.000000 validation_framework-0.1.0/validation/aider/tests/test_repo.py
--rw-rw-rw-   0        0        0     7271 2024-06-03 01:29:28.000000 validation_framework-0.1.0/validation/aider/tests/test_repomap.py
--rw-rw-rw-   0        0        0     1392 2024-06-03 01:29:28.000000 validation_framework-0.1.0/validation/aider/tests/test_sendchat.py
--rw-rw-rw-   0        0        0     3289 2024-06-03 01:29:28.000000 validation_framework-0.1.0/validation/aider/tests/test_udiff.py
--rw-rw-rw-   0        0        0    11658 2024-06-03 01:29:28.000000 validation_framework-0.1.0/validation/aider/tests/test_wholefile.py
--rw-rw-rw-   0        0        0     5134 2024-06-03 01:22:51.000000 validation_framework-0.1.0/validation/script.py
--rw-rw-rw-   0        0        0     1252 2024-06-03 01:24:15.000000 validation_framework-0.1.0/validation/validate.py
-drwxrwxrwx   0        0        0        0 2024-06-03 01:39:03.561029 validation_framework-0.1.0/validation_framework.egg-info/
--rw-rw-rw-   0        0        0      570 2024-06-03 01:39:00.000000 validation_framework-0.1.0/validation_framework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2797 2024-06-03 01:39:02.000000 validation_framework-0.1.0/validation_framework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 01:39:00.000000 validation_framework-0.1.0/validation_framework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-06-03 01:39:00.000000 validation_framework-0.1.0/validation_framework.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-06-03 01:39:00.000000 validation_framework-0.1.0/validation_framework.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-03 02:13:59.975747 validation_framework-0.1.1/
+-rw-rw-rw-   0        0        0      489 2024-06-03 02:13:59.966101 validation_framework-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-06-03 00:57:05.000000 validation_framework-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-03 02:13:59.977286 validation_framework-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      883 2024-06-03 02:13:47.000000 validation_framework-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 02:13:59.377354 validation_framework-0.1.1/validation/
+-rw-rw-rw-   0        0        0        0 2024-06-03 01:38:34.000000 validation_framework-0.1.1/validation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 02:13:59.391353 validation_framework-0.1.1/validation/aider/
+-rw-rw-rw-   0        0        0        0 2024-06-03 01:37:12.000000 validation_framework-0.1.1/validation/aider/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 02:13:59.581548 validation_framework-0.1.1/validation/aider/aider/
+-rw-rw-rw-   0        0        0       28 2024-06-03 01:29:25.000000 validation_framework-0.1.1/validation/aider/aider/__init__.py
+-rw-rw-rw-   0        0        0    13976 2024-06-03 01:29:25.000000 validation_framework-0.1.1/validation/aider/aider/args.py
+drwxrwxrwx   0        0        0        0 2024-06-03 02:13:59.736990 validation_framework-0.1.1/validation/aider/aider/coders/
+-rw-rw-rw-   0        0        0      624 2024-06-03 01:29:25.000000 validation_framework-0.1.1/validation/aider/aider/coders/__init__.py
+-rw-rw-rw-   0        0        0    45295 2024-06-03 01:29:25.000000 validation_framework-0.1.1/validation/aider/aider/coders/base_coder.py
+-rw-rw-rw-   0        0        0     1625 2024-06-03 01:29:25.000000 validation_framework-0.1.1/validation/aider/aider/coders/base_prompts.py
+-rw-rw-rw-   0        0        0    15675 2024-06-03 01:29:25.000000 validation_framework-0.1.1/validation/aider/aider/coders/editblock_coder.py
+-rw-rw-rw-   0        0        0      368 2024-06-03 01:29:25.000000 validation_framework-0.1.1/validation/aider/aider/coders/editblock_fenced_coder.py
+-rw-rw-rw-   0        0        0     1887 2024-06-03 01:29:25.000000 validation_framework-0.1.1/validation/aider/aider/coders/editblock_fenced_prompts.py
+-rw-rw-rw-   0        0        0     5458 2024-06-03 01:29:25.000000 validation_framework-0.1.1/validation/aider/aider/coders/editblock_func_coder.py
+-rw-rw-rw-   0        0        0      913 2024-06-03 01:29:26.000000 validation_framework-0.1.1/validation/aider/aider/coders/editblock_func_prompts.py
+-rw-rw-rw-   0        0        0     4498 2024-06-03 01:29:26.000000 validation_framework-0.1.1/validation/aider/aider/coders/editblock_prompts.py
+-rw-rw-rw-   0        0        0    20773 2024-06-03 01:29:26.000000 validation_framework-0.1.1/validation/aider/aider/coders/search_replace.py
+-rw-rw-rw-   0        0        0     3508 2024-06-03 01:29:26.000000 validation_framework-0.1.1/validation/aider/aider/coders/single_wholefile_func_coder.py
+-rw-rw-rw-   0        0        0      894 2024-06-03 01:29:26.000000 validation_framework-0.1.1/validation/aider/aider/coders/single_wholefile_func_prompts.py
+-rw-rw-rw-   0        0        0    11127 2024-06-03 01:29:26.000000 validation_framework-0.1.1/validation/aider/aider/coders/udiff_coder.py
+-rw-rw-rw-   0        0        0     3316 2024-06-03 01:29:26.000000 validation_framework-0.1.1/validation/aider/aider/coders/udiff_prompts.py
+-rw-rw-rw-   0        0        0     5293 2024-06-03 01:29:26.000000 validation_framework-0.1.1/validation/aider/aider/coders/wholefile_coder.py
+-rw-rw-rw-   0        0        0     4367 2024-06-03 01:29:26.000000 validation_framework-0.1.1/validation/aider/aider/coders/wholefile_func_coder.py
+-rw-rw-rw-   0        0        0      895 2024-06-03 01:29:26.000000 validation_framework-0.1.1/validation/aider/aider/coders/wholefile_func_prompts.py
+-rw-rw-rw-   0        0        0     1913 2024-06-03 01:29:26.000000 validation_framework-0.1.1/validation/aider/aider/coders/wholefile_prompts.py
+-rw-rw-rw-   0        0        0    24693 2024-06-03 01:29:26.000000 validation_framework-0.1.1/validation/aider/aider/commands.py
+-rw-rw-rw-   0        0        0     3189 2024-06-03 01:29:26.000000 validation_framework-0.1.1/validation/aider/aider/diffs.py
+-rw-rw-rw-   0        0        0      682 2024-06-03 01:29:26.000000 validation_framework-0.1.1/validation/aider/aider/dump.py
+-rw-rw-rw-   0        0        0    17857 2024-06-03 01:29:26.000000 validation_framework-0.1.1/validation/aider/aider/gui.py
+-rw-rw-rw-   0        0        0     3831 2024-06-03 01:29:26.000000 validation_framework-0.1.1/validation/aider/aider/history.py
+-rw-rw-rw-   0        0        0    12525 2024-06-03 01:29:26.000000 validation_framework-0.1.1/validation/aider/aider/io.py
+-rw-rw-rw-   0        0        0     6603 2024-06-03 01:29:26.000000 validation_framework-0.1.1/validation/aider/aider/linter.py
+-rw-rw-rw-   0        0        0      316 2024-06-03 01:29:26.000000 validation_framework-0.1.1/validation/aider/aider/litellm.py
+-rw-rw-rw-   0        0        0    14170 2024-06-03 01:29:26.000000 validation_framework-0.1.1/validation/aider/aider/main.py
+-rw-rw-rw-   0        0        0     3047 2024-06-03 01:29:26.000000 validation_framework-0.1.1/validation/aider/aider/mdstream.py
+-rw-rw-rw-   0        0        0    16123 2024-06-03 01:29:26.000000 validation_framework-0.1.1/validation/aider/aider/models.py
+-rw-rw-rw-   0        0        0     2174 2024-06-03 01:29:26.000000 validation_framework-0.1.1/validation/aider/aider/prompts.py
+-rw-rw-rw-   0        0        0     8129 2024-06-03 01:29:26.000000 validation_framework-0.1.1/validation/aider/aider/repo.py
+-rw-rw-rw-   0        0        0    16125 2024-06-03 01:29:26.000000 validation_framework-0.1.1/validation/aider/aider/repomap.py
+-rw-rw-rw-   0        0        0     5621 2024-06-03 01:29:26.000000 validation_framework-0.1.1/validation/aider/aider/scrape.py
+-rw-rw-rw-   0        0        0     2239 2024-06-03 01:29:26.000000 validation_framework-0.1.1/validation/aider/aider/sendchat.py
+-rw-rw-rw-   0        0        0     4413 2024-06-03 01:29:26.000000 validation_framework-0.1.1/validation/aider/aider/utils.py
+-rw-rw-rw-   0        0        0     1052 2024-06-03 01:29:26.000000 validation_framework-0.1.1/validation/aider/aider/versioncheck.py
+-rw-rw-rw-   0        0        0     2817 2024-06-03 01:29:26.000000 validation_framework-0.1.1/validation/aider/aider/voice.py
+drwxrwxrwx   0        0        0        0 2024-06-03 02:13:59.812269 validation_framework-0.1.1/validation/aider/benchmark/
+-rw-rw-rw-   0        0        0        0 2024-06-03 01:29:27.000000 validation_framework-0.1.1/validation/aider/benchmark/__init__.py
+-rw-rw-rw-   0        0        0    22214 2024-06-03 01:29:27.000000 validation_framework-0.1.1/validation/aider/benchmark/benchmark.py
+-rw-rw-rw-   0        0        0     1885 2024-06-03 01:29:27.000000 validation_framework-0.1.1/validation/aider/benchmark/over_time.py
+-rw-rw-rw-   0        0        0    11842 2024-06-03 01:29:27.000000 validation_framework-0.1.1/validation/aider/benchmark/plots.py
+-rw-rw-rw-   0        0        0      469 2024-06-03 01:29:27.000000 validation_framework-0.1.1/validation/aider/benchmark/prompts.py
+-rw-rw-rw-   0        0        0     6662 2024-06-03 01:29:27.000000 validation_framework-0.1.1/validation/aider/benchmark/refactor_tools.py
+-rw-rw-rw-   0        0        0     1415 2024-06-03 01:29:27.000000 validation_framework-0.1.1/validation/aider/benchmark/rungrid.py
+-rw-rw-rw-   0        0        0     3752 2024-06-03 01:29:27.000000 validation_framework-0.1.1/validation/aider/benchmark/swe_bench.py
+-rw-rw-rw-   0        0        0     1582 2024-06-03 01:29:27.000000 validation_framework-0.1.1/validation/aider/benchmark/test_benchmark.py
+-rw-rw-rw-   0        0        0     1532 2024-06-03 01:29:28.000000 validation_framework-0.1.1/validation/aider/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 02:13:59.917504 validation_framework-0.1.1/validation/aider/tests/
+-rw-rw-rw-   0        0        0        0 2024-06-03 01:29:28.000000 validation_framework-0.1.1/validation/aider/tests/__init__.py
+-rw-rw-rw-   0        0        0    19321 2024-06-03 01:29:28.000000 validation_framework-0.1.1/validation/aider/tests/test_coder.py
+-rw-rw-rw-   0        0        0    20626 2024-06-03 01:29:28.000000 validation_framework-0.1.1/validation/aider/tests/test_commands.py
+-rw-rw-rw-   0        0        0    11695 2024-06-03 01:29:28.000000 validation_framework-0.1.1/validation/aider/tests/test_editblock.py
+-rw-rw-rw-   0        0        0     2664 2024-06-03 01:29:28.000000 validation_framework-0.1.1/validation/aider/tests/test_io.py
+-rw-rw-rw-   0        0        0     9531 2024-06-03 01:29:28.000000 validation_framework-0.1.1/validation/aider/tests/test_main.py
+-rw-rw-rw-   0        0        0      830 2024-06-03 01:29:28.000000 validation_framework-0.1.1/validation/aider/tests/test_models.py
+-rw-rw-rw-   0        0        0    10570 2024-06-03 01:29:28.000000 validation_framework-0.1.1/validation/aider/tests/test_repo.py
+-rw-rw-rw-   0        0        0     7271 2024-06-03 01:29:28.000000 validation_framework-0.1.1/validation/aider/tests/test_repomap.py
+-rw-rw-rw-   0        0        0     1392 2024-06-03 01:29:28.000000 validation_framework-0.1.1/validation/aider/tests/test_sendchat.py
+-rw-rw-rw-   0        0        0     3289 2024-06-03 01:29:28.000000 validation_framework-0.1.1/validation/aider/tests/test_udiff.py
+-rw-rw-rw-   0        0        0    11658 2024-06-03 01:29:28.000000 validation_framework-0.1.1/validation/aider/tests/test_wholefile.py
+-rw-rw-rw-   0        0        0     5134 2024-06-03 01:22:51.000000 validation_framework-0.1.1/validation/script.py
+-rw-rw-rw-   0        0        0     1252 2024-06-03 01:24:15.000000 validation_framework-0.1.1/validation/validate.py
+drwxrwxrwx   0        0        0        0 2024-06-03 02:13:59.960100 validation_framework-0.1.1/validation_framework.egg-info/
+-rw-rw-rw-   0        0        0      489 2024-06-03 02:13:57.000000 validation_framework-0.1.1/validation_framework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2754 2024-06-03 02:13:59.000000 validation_framework-0.1.1/validation_framework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 02:13:57.000000 validation_framework-0.1.1/validation_framework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-06-03 02:13:57.000000 validation_framework-0.1.1/validation_framework.egg-info/top_level.txt
```

### Comparing `validation_framework-0.1.0/setup.py` & `validation_framework-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name='validation_framework',
-    version='0.1.0',
+    version='0.1.1',
     description='A framework for validating LLM responses on various criteria.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/yourusername/validation_framework',  # Update with your URL
     author='Your Name',
     author_email='your.email@example.com',
     license='MIT',  # Or any license you choose
     packages=find_packages(),
     install_requires=[
-        'some_dependency>=1.0.0',
-        'another_dependency>=2.0.0',
+        # 'some_dependency>=1.0.0',
+        # 'another_dependency>=2.0.0',
         # Add other dependencies here
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
```

### Comparing `validation_framework-0.1.0/validation/aider/aider/args.py` & `validation_framework-0.1.1/validation/aider/aider/args.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/aider/coders/__init__.py` & `validation_framework-0.1.1/validation/aider/aider/coders/__init__.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/aider/coders/base_coder.py` & `validation_framework-0.1.1/validation/aider/aider/coders/base_coder.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/aider/coders/base_prompts.py` & `validation_framework-0.1.1/validation/aider/aider/coders/base_prompts.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/aider/coders/editblock_coder.py` & `validation_framework-0.1.1/validation/aider/aider/coders/editblock_coder.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/aider/coders/editblock_fenced_prompts.py` & `validation_framework-0.1.1/validation/aider/aider/coders/editblock_fenced_prompts.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/aider/coders/editblock_func_coder.py` & `validation_framework-0.1.1/validation/aider/aider/coders/editblock_func_coder.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/aider/coders/editblock_func_prompts.py` & `validation_framework-0.1.1/validation/aider/aider/coders/editblock_func_prompts.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/aider/coders/editblock_prompts.py` & `validation_framework-0.1.1/validation/aider/aider/coders/editblock_prompts.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/aider/coders/search_replace.py` & `validation_framework-0.1.1/validation/aider/aider/coders/search_replace.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/aider/coders/single_wholefile_func_coder.py` & `validation_framework-0.1.1/validation/aider/aider/coders/single_wholefile_func_coder.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/aider/coders/single_wholefile_func_prompts.py` & `validation_framework-0.1.1/validation/aider/aider/coders/single_wholefile_func_prompts.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/aider/coders/udiff_coder.py` & `validation_framework-0.1.1/validation/aider/aider/coders/udiff_coder.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/aider/coders/udiff_prompts.py` & `validation_framework-0.1.1/validation/aider/aider/coders/udiff_prompts.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/aider/coders/wholefile_coder.py` & `validation_framework-0.1.1/validation/aider/aider/coders/wholefile_coder.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/aider/coders/wholefile_func_coder.py` & `validation_framework-0.1.1/validation/aider/aider/coders/wholefile_func_coder.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/aider/coders/wholefile_func_prompts.py` & `validation_framework-0.1.1/validation/aider/aider/coders/wholefile_func_prompts.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/aider/coders/wholefile_prompts.py` & `validation_framework-0.1.1/validation/aider/aider/coders/wholefile_prompts.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/aider/commands.py` & `validation_framework-0.1.1/validation/aider/aider/commands.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/aider/diffs.py` & `validation_framework-0.1.1/validation/aider/aider/diffs.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/aider/dump.py` & `validation_framework-0.1.1/validation/aider/aider/dump.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/aider/gui.py` & `validation_framework-0.1.1/validation/aider/aider/gui.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/aider/history.py` & `validation_framework-0.1.1/validation/aider/aider/history.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/aider/io.py` & `validation_framework-0.1.1/validation/aider/aider/io.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/aider/linter.py` & `validation_framework-0.1.1/validation/aider/aider/linter.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/aider/main.py` & `validation_framework-0.1.1/validation/aider/aider/main.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/aider/mdstream.py` & `validation_framework-0.1.1/validation/aider/aider/mdstream.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/aider/models.py` & `validation_framework-0.1.1/validation/aider/aider/models.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/aider/prompts.py` & `validation_framework-0.1.1/validation/aider/aider/prompts.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/aider/repo.py` & `validation_framework-0.1.1/validation/aider/aider/repo.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/aider/repomap.py` & `validation_framework-0.1.1/validation/aider/aider/repomap.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/aider/scrape.py` & `validation_framework-0.1.1/validation/aider/aider/scrape.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/aider/sendchat.py` & `validation_framework-0.1.1/validation/aider/aider/sendchat.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/aider/utils.py` & `validation_framework-0.1.1/validation/aider/aider/utils.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/aider/versioncheck.py` & `validation_framework-0.1.1/validation/aider/aider/versioncheck.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/aider/voice.py` & `validation_framework-0.1.1/validation/aider/aider/voice.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/benchmark/benchmark.py` & `validation_framework-0.1.1/validation/aider/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/benchmark/over_time.py` & `validation_framework-0.1.1/validation/aider/benchmark/over_time.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/benchmark/plots.py` & `validation_framework-0.1.1/validation/aider/benchmark/plots.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/benchmark/refactor_tools.py` & `validation_framework-0.1.1/validation/aider/benchmark/refactor_tools.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/benchmark/rungrid.py` & `validation_framework-0.1.1/validation/aider/benchmark/rungrid.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/benchmark/swe_bench.py` & `validation_framework-0.1.1/validation/aider/benchmark/swe_bench.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/benchmark/test_benchmark.py` & `validation_framework-0.1.1/validation/aider/benchmark/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/setup.py` & `validation_framework-0.1.1/validation/aider/setup.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/tests/test_coder.py` & `validation_framework-0.1.1/validation/aider/tests/test_coder.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/tests/test_commands.py` & `validation_framework-0.1.1/validation/aider/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/tests/test_editblock.py` & `validation_framework-0.1.1/validation/aider/tests/test_editblock.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/tests/test_io.py` & `validation_framework-0.1.1/validation/aider/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/tests/test_main.py` & `validation_framework-0.1.1/validation/aider/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/tests/test_models.py` & `validation_framework-0.1.1/validation/aider/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/tests/test_repo.py` & `validation_framework-0.1.1/validation/aider/tests/test_repo.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/tests/test_repomap.py` & `validation_framework-0.1.1/validation/aider/tests/test_repomap.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/tests/test_sendchat.py` & `validation_framework-0.1.1/validation/aider/tests/test_sendchat.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/tests/test_udiff.py` & `validation_framework-0.1.1/validation/aider/tests/test_udiff.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/aider/tests/test_wholefile.py` & `validation_framework-0.1.1/validation/aider/tests/test_wholefile.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/script.py` & `validation_framework-0.1.1/validation/script.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation/validate.py` & `validation_framework-0.1.1/validation/validate.py`

 * *Files identical despite different names*

### Comparing `validation_framework-0.1.0/validation_framework.egg-info/SOURCES.txt` & `validation_framework-0.1.1/validation_framework.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -64,9 +64,8 @@
 validation/aider/tests/test_repomap.py
 validation/aider/tests/test_sendchat.py
 validation/aider/tests/test_udiff.py
 validation/aider/tests/test_wholefile.py
 validation_framework.egg-info/PKG-INFO
 validation_framework.egg-info/SOURCES.txt
 validation_framework.egg-info/dependency_links.txt
-validation_framework.egg-info/requires.txt
 validation_framework.egg-info/top_level.txt
```

