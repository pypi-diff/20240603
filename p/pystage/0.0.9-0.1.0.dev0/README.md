# Comparing `tmp/pystage-0.0.9.tar.gz` & `tmp/pystage-0.1.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/kai/daten/projekte/pystage/pystage-git/dist/tmpfv4foz05/pystage-0.0.9.tar", last modified: Wed Jul 21 19:33:23 2021, max compression
+gzip compressed data, was "pystage-0.1.0.dev0.tar", last modified: Mon Jun  3 10:48:21 2024, max compression
```

## Comparing `pystage-0.0.9.tar` & `pystage-0.1.0.dev0.tar`

### file list

```diff
@@ -1,69 +1,68 @@
-drwxr-xr-x   0 kai       (1000) kai       (1000)        0 2021-07-21 19:33:23.123508 pystage-0.0.9/
--rw-r--r--   0 kai       (1000) kai       (1000)     1050 2021-05-18 07:51:47.000000 pystage-0.0.9/LICENSE
--rw-r--r--   0 kai       (1000) kai       (1000)     2308 2021-07-21 19:33:23.123508 pystage-0.0.9/PKG-INFO
--rw-r--r--   0 kai       (1000) kai       (1000)     1780 2021-07-21 12:00:28.000000 pystage-0.0.9/README.md
--rw-r--r--   0 kai       (1000) kai       (1000)      104 2021-05-18 07:52:48.000000 pystage-0.0.9/pyproject.toml
--rw-r--r--   0 kai       (1000) kai       (1000)      742 2021-07-21 19:33:23.123508 pystage-0.0.9/setup.cfg
-drwxr-xr-x   0 kai       (1000) kai       (1000)        0 2021-07-21 19:33:23.106841 pystage-0.0.9/src/
-drwxr-xr-x   0 kai       (1000) kai       (1000)        0 2021-07-21 19:33:23.106841 pystage-0.0.9/src/pystage/
--rw-r--r--   0 kai       (1000) kai       (1000)      190 2021-07-09 21:02:48.000000 pystage-0.0.9/src/pystage/__init__.py
-drwxr-xr-x   0 kai       (1000) kai       (1000)        0 2021-07-21 19:33:23.110175 pystage-0.0.9/src/pystage/convert/
--rw-r--r--   0 kai       (1000) kai       (1000)       62 2021-06-01 14:53:05.000000 pystage-0.0.9/src/pystage/convert/__init__.py
--rw-r--r--   0 kai       (1000) kai       (1000)     9541 2021-07-20 09:41:29.000000 pystage-0.0.9/src/pystage/convert/code_writer.py
--rw-r--r--   0 kai       (1000) kai       (1000)    15979 2021-07-20 10:22:13.000000 pystage-0.0.9/src/pystage/convert/sb3.py
--rw-r--r--   0 kai       (1000) kai       (1000)     3358 2021-07-09 21:02:48.000000 pystage-0.0.9/src/pystage/convert/sb3_templates.py
-drwxr-xr-x   0 kai       (1000) kai       (1000)        0 2021-07-21 19:33:23.110175 pystage-0.0.9/src/pystage/core/
--rw-r--r--   0 kai       (1000) kai       (1000)      111 2021-07-13 07:10:01.000000 pystage-0.0.9/src/pystage/core/__init__.py
--rw-r--r--   0 kai       (1000) kai       (1000)      460 2021-07-21 16:48:35.000000 pystage-0.0.9/src/pystage/core/_base_sprite.py
--rw-r--r--   0 kai       (1000) kai       (1000)     1468 2021-07-20 04:44:42.000000 pystage-0.0.9/src/pystage/core/_control.py
--rw-r--r--   0 kai       (1000) kai       (1000)     3349 2021-07-20 08:09:05.000000 pystage-0.0.9/src/pystage/core/_events.py
--rw-r--r--   0 kai       (1000) kai       (1000)     9822 2021-07-21 16:48:06.000000 pystage-0.0.9/src/pystage/core/_looks.py
--rw-r--r--   0 kai       (1000) kai       (1000)     6339 2021-07-21 19:29:14.000000 pystage-0.0.9/src/pystage/core/_motion.py
--rw-r--r--   0 kai       (1000) kai       (1000)     1052 2021-07-09 21:02:48.000000 pystage-0.0.9/src/pystage/core/_operators.py
--rw-r--r--   0 kai       (1000) kai       (1000)     5981 2021-07-21 08:25:47.000000 pystage-0.0.9/src/pystage/core/_pen.py
--rw-r--r--   0 kai       (1000) kai       (1000)     6549 2021-07-20 10:41:51.000000 pystage-0.0.9/src/pystage/core/_sensing.py
--rw-r--r--   0 kai       (1000) kai       (1000)     4308 2021-07-12 15:33:41.000000 pystage-0.0.9/src/pystage/core/_sound.py
--rw-r--r--   0 kai       (1000) kai       (1000)     2329 2021-07-20 10:37:51.000000 pystage-0.0.9/src/pystage/core/_variables.py
--rw-r--r--   0 kai       (1000) kai       (1000)     8212 2021-07-21 19:26:14.000000 pystage-0.0.9/src/pystage/core/assets.py
--rw-r--r--   0 kai       (1000) kai       (1000)    10296 2021-07-21 13:28:35.000000 pystage-0.0.9/src/pystage/core/code_block.py
--rw-r--r--   0 kai       (1000) kai       (1000)     1128 2021-07-09 21:02:48.000000 pystage-0.0.9/src/pystage/core/constants.py
--rw-r--r--   0 kai       (1000) kai       (1000)     8754 2021-07-18 09:25:43.000000 pystage-0.0.9/src/pystage/core/gui.py
--rw-r--r--   0 kai       (1000) kai       (1000)      424 2021-07-13 13:57:29.000000 pystage-0.0.9/src/pystage/core/messages.py
--rw-r--r--   0 kai       (1000) kai       (1000)     1650 2021-07-21 13:47:02.000000 pystage-0.0.9/src/pystage/core/sprite.py
--rw-r--r--   0 kai       (1000) kai       (1000)     6263 2021-07-21 08:29:24.000000 pystage-0.0.9/src/pystage/core/stage.py
-drwxr-xr-x   0 kai       (1000) kai       (1000)        0 2021-07-21 19:33:23.110175 pystage-0.0.9/src/pystage/de/
--rw-r--r--   0 kai       (1000) kai       (1000)      126 2021-07-09 21:02:48.000000 pystage-0.0.9/src/pystage/de/__init__.py
--rw-r--r--   0 kai       (1000) kai       (1000)    62452 2021-07-20 11:55:36.000000 pystage-0.0.9/src/pystage/de/sprite.py
--rw-r--r--   0 kai       (1000) kai       (1000)    37451 2021-07-20 11:38:03.000000 pystage-0.0.9/src/pystage/de/stage.py
-drwxr-xr-x   0 kai       (1000) kai       (1000)        0 2021-07-21 19:33:23.110175 pystage-0.0.9/src/pystage/en/
--rw-r--r--   0 kai       (1000) kai       (1000)      126 2021-07-09 21:02:48.000000 pystage-0.0.9/src/pystage/en/__init__.py
--rw-r--r--   0 kai       (1000) kai       (1000)    53284 2021-07-13 22:56:55.000000 pystage-0.0.9/src/pystage/en/sprite.py
--rw-r--r--   0 kai       (1000) kai       (1000)    36449 2021-07-20 15:51:23.000000 pystage-0.0.9/src/pystage/en/stage.py
-drwxr-xr-x   0 kai       (1000) kai       (1000)        0 2021-07-21 19:33:23.113508 pystage-0.0.9/src/pystage/fonts/
--rw-r--r--   0 kai       (1000) kai       (1000)   167336 2013-01-08 23:00:00.000000 pystage-0.0.9/src/pystage/fonts/roboto-bold.ttf
--rw-r--r--   0 kai       (1000) kai       (1000)   167000 2013-01-08 23:00:00.000000 pystage-0.0.9/src/pystage/fonts/roboto-light.ttf
--rw-r--r--   0 kai       (1000) kai       (1000)   168260 2013-01-08 23:00:00.000000 pystage-0.0.9/src/pystage/fonts/roboto-regular.ttf
-drwxr-xr-x   0 kai       (1000) kai       (1000)        0 2021-07-21 19:33:23.116841 pystage-0.0.9/src/pystage/images/
--rw-r--r--   0 kai       (1000) kai       (1000)    26719 2021-06-03 22:03:09.000000 pystage-0.0.9/src/pystage/images/grid.svg
--rw-------   0 kai       (1000) kai       (1000)     2523 2021-06-03 09:02:21.000000 pystage-0.0.9/src/pystage/images/say.png
--rw-------   0 kai       (1000) kai       (1000)     2650 2021-06-03 09:01:36.000000 pystage-0.0.9/src/pystage/images/think.png
--rw-r--r--   0 kai       (1000) kai       (1000)     5177 2021-06-01 14:53:05.000000 pystage-0.0.9/src/pystage/images/zombie_idle.png
-drwxr-xr-x   0 kai       (1000) kai       (1000)        0 2021-07-21 19:33:23.116841 pystage-0.0.9/src/pystage/ja/
--rw-r--r--   0 kai       (1000) kai       (1000)      149 2021-07-20 16:31:04.000000 pystage-0.0.9/src/pystage/ja/__init__.py
--rw-r--r--   0 kai       (1000) kai       (1000)    62246 2021-07-20 16:30:51.000000 pystage-0.0.9/src/pystage/ja/sprite.py
--rw-r--r--   0 kai       (1000) kai       (1000)    37256 2021-07-20 16:28:49.000000 pystage-0.0.9/src/pystage/ja/stage.py
-drwxr-xr-x   0 kai       (1000) kai       (1000)        0 2021-07-21 19:33:23.116841 pystage-0.0.9/src/pystage/l10n/
--rw-r--r--   0 kai       (1000) kai       (1000)        0 2021-07-09 21:02:48.000000 pystage-0.0.9/src/pystage/l10n/__init__.py
--rw-r--r--   0 kai       (1000) kai       (1000)     7399 2021-07-20 10:31:53.000000 pystage-0.0.9/src/pystage/l10n/__main__.py
--rw-r--r--   0 kai       (1000) kai       (1000)     2925 2021-07-18 10:11:30.000000 pystage-0.0.9/src/pystage/l10n/api.py
--rw-r--r--   0 kai       (1000) kai       (1000)     2406 2021-07-13 10:01:53.000000 pystage-0.0.9/src/pystage/l10n/translations.py
-drwxr-xr-x   0 kai       (1000) kai       (1000)        0 2021-07-21 19:33:23.116841 pystage-0.0.9/src/pystage/sounds/
--rw-r--r--   0 kai       (1000) kai       (1000)    63036 2021-07-09 21:02:48.000000 pystage-0.0.9/src/pystage/sounds/dancehead2.wav
--rw-r--r--   0 kai       (1000) kai       (1000)   192012 2021-07-09 21:02:48.000000 pystage-0.0.9/src/pystage/sounds/guitar.wav
--rw-r--r--   0 kai       (1000) kai       (1000)     3623 2021-06-09 18:23:09.000000 pystage-0.0.9/src/pystage/util.py
-drwxr-xr-x   0 kai       (1000) kai       (1000)        0 2021-07-21 19:33:23.110175 pystage-0.0.9/src/pystage.egg-info/
--rw-r--r--   0 kai       (1000) kai       (1000)     2308 2021-07-21 19:33:23.000000 pystage-0.0.9/src/pystage.egg-info/PKG-INFO
--rw-r--r--   0 kai       (1000) kai       (1000)     1534 2021-07-21 19:33:23.000000 pystage-0.0.9/src/pystage.egg-info/SOURCES.txt
--rw-r--r--   0 kai       (1000) kai       (1000)        1 2021-07-21 19:33:23.000000 pystage-0.0.9/src/pystage.egg-info/dependency_links.txt
--rw-r--r--   0 kai       (1000) kai       (1000)       21 2021-07-21 19:33:23.000000 pystage-0.0.9/src/pystage.egg-info/requires.txt
--rw-r--r--   0 kai       (1000) kai       (1000)        8 2021-07-21 19:33:23.000000 pystage-0.0.9/src/pystage.egg-info/top_level.txt
+drwxr-xr-x   0 kai       (1000) kai       (1000)        0 2024-06-03 10:48:21.162715 pystage-0.1.0.dev0/
+-rw-r--r--   0 kai       (1000) kai       (1000)     1050 2023-07-05 07:39:47.000000 pystage-0.1.0.dev0/LICENSE
+-rw-r--r--   0 kai       (1000) kai       (1000)     5123 2024-06-03 10:48:21.162715 pystage-0.1.0.dev0/PKG-INFO
+-rw-r--r--   0 kai       (1000) kai       (1000)     4544 2024-05-31 21:01:15.000000 pystage-0.1.0.dev0/README.md
+-rw-r--r--   0 kai       (1000) kai       (1000)      104 2023-07-05 07:39:55.000000 pystage-0.1.0.dev0/pyproject.toml
+-rw-r--r--   0 kai       (1000) kai       (1000)      746 2024-06-03 10:48:21.162715 pystage-0.1.0.dev0/setup.cfg
+drwxr-xr-x   0 kai       (1000) kai       (1000)        0 2024-06-03 10:48:21.142715 pystage-0.1.0.dev0/src/
+drwxr-xr-x   0 kai       (1000) kai       (1000)        0 2024-06-03 10:48:21.146048 pystage-0.1.0.dev0/src/pystage/
+-rw-r--r--   0 kai       (1000) kai       (1000)      191 2024-05-31 23:16:47.000000 pystage-0.1.0.dev0/src/pystage/__init__.py
+drwxr-xr-x   0 kai       (1000) kai       (1000)        0 2024-06-03 10:48:21.146048 pystage-0.1.0.dev0/src/pystage/convert/
+-rw-r--r--   0 kai       (1000) kai       (1000)       62 2023-07-05 07:39:55.000000 pystage-0.1.0.dev0/src/pystage/convert/__init__.py
+-rw-r--r--   0 kai       (1000) kai       (1000)    10801 2024-05-31 21:01:15.000000 pystage-0.1.0.dev0/src/pystage/convert/code_writer.py
+-rw-r--r--   0 kai       (1000) kai       (1000)    19362 2024-06-03 10:20:37.000000 pystage-0.1.0.dev0/src/pystage/convert/sb3.py
+-rw-r--r--   0 kai       (1000) kai       (1000)     4037 2024-06-03 10:23:41.000000 pystage-0.1.0.dev0/src/pystage/convert/sb3_templates.py
+drwxr-xr-x   0 kai       (1000) kai       (1000)        0 2024-06-03 10:48:21.152715 pystage-0.1.0.dev0/src/pystage/core/
+-rw-r--r--   0 kai       (1000) kai       (1000)      111 2023-07-05 07:39:55.000000 pystage-0.1.0.dev0/src/pystage/core/__init__.py
+-rw-r--r--   0 kai       (1000) kai       (1000)      460 2023-07-05 07:39:55.000000 pystage-0.1.0.dev0/src/pystage/core/_base_sprite.py
+-rw-r--r--   0 kai       (1000) kai       (1000)     1506 2024-05-31 21:01:15.000000 pystage-0.1.0.dev0/src/pystage/core/_control.py
+-rw-r--r--   0 kai       (1000) kai       (1000)     3349 2023-07-05 14:24:46.000000 pystage-0.1.0.dev0/src/pystage/core/_events.py
+-rw-r--r--   0 kai       (1000) kai       (1000)    10035 2024-05-31 21:01:15.000000 pystage-0.1.0.dev0/src/pystage/core/_looks.py
+-rw-r--r--   0 kai       (1000) kai       (1000)     7045 2024-05-31 21:01:15.000000 pystage-0.1.0.dev0/src/pystage/core/_motion.py
+-rw-r--r--   0 kai       (1000) kai       (1000)     1681 2024-05-31 21:01:15.000000 pystage-0.1.0.dev0/src/pystage/core/_operators.py
+-rw-r--r--   0 kai       (1000) kai       (1000)     6930 2023-07-05 07:39:55.000000 pystage-0.1.0.dev0/src/pystage/core/_pen.py
+-rw-r--r--   0 kai       (1000) kai       (1000)     8278 2024-06-03 10:23:41.000000 pystage-0.1.0.dev0/src/pystage/core/_sensing.py
+-rw-r--r--   0 kai       (1000) kai       (1000)     4308 2023-07-05 14:24:46.000000 pystage-0.1.0.dev0/src/pystage/core/_sound.py
+-rw-r--r--   0 kai       (1000) kai       (1000)     3671 2023-07-05 14:24:46.000000 pystage-0.1.0.dev0/src/pystage/core/_variables.py
+-rw-r--r--   0 kai       (1000) kai       (1000)     4757 2023-07-05 07:39:55.000000 pystage-0.1.0.dev0/src/pystage/core/asking.py
+-rw-r--r--   0 kai       (1000) kai       (1000)     8454 2023-07-05 14:24:46.000000 pystage-0.1.0.dev0/src/pystage/core/assets.py
+-rw-r--r--   0 kai       (1000) kai       (1000)    11227 2023-07-05 14:24:46.000000 pystage-0.1.0.dev0/src/pystage/core/code_block.py
+-rw-r--r--   0 kai       (1000) kai       (1000)     1128 2023-07-05 07:39:55.000000 pystage-0.1.0.dev0/src/pystage/core/constants.py
+-rw-r--r--   0 kai       (1000) kai       (1000)     9007 2024-05-31 21:01:15.000000 pystage-0.1.0.dev0/src/pystage/core/gui.py
+-rw-r--r--   0 kai       (1000) kai       (1000)      424 2023-07-05 07:39:55.000000 pystage-0.1.0.dev0/src/pystage/core/messages.py
+-rw-r--r--   0 kai       (1000) kai       (1000)     5025 2023-07-05 07:39:55.000000 pystage-0.1.0.dev0/src/pystage/core/monitors.py
+-rw-r--r--   0 kai       (1000) kai       (1000)     1527 2023-07-05 14:24:46.000000 pystage-0.1.0.dev0/src/pystage/core/sprite.py
+-rw-r--r--   0 kai       (1000) kai       (1000)    10381 2024-05-31 21:01:15.000000 pystage-0.1.0.dev0/src/pystage/core/stage.py
+drwxr-xr-x   0 kai       (1000) kai       (1000)        0 2024-06-03 10:48:21.152715 pystage-0.1.0.dev0/src/pystage/de/
+-rw-r--r--   0 kai       (1000) kai       (1000)      126 2023-07-05 07:39:55.000000 pystage-0.1.0.dev0/src/pystage/de/__init__.py
+-rw-r--r--   0 kai       (1000) kai       (1000)    63933 2023-07-05 07:39:55.000000 pystage-0.1.0.dev0/src/pystage/de/sprite.py
+-rw-r--r--   0 kai       (1000) kai       (1000)    38628 2023-07-05 07:39:55.000000 pystage-0.1.0.dev0/src/pystage/de/stage.py
+drwxr-xr-x   0 kai       (1000) kai       (1000)        0 2024-06-03 10:48:21.156048 pystage-0.1.0.dev0/src/pystage/en/
+-rw-r--r--   0 kai       (1000) kai       (1000)      126 2023-07-05 07:39:55.000000 pystage-0.1.0.dev0/src/pystage/en/__init__.py
+-rw-r--r--   0 kai       (1000) kai       (1000)    52623 2023-07-05 14:24:46.000000 pystage-0.1.0.dev0/src/pystage/en/sprite.py
+-rw-r--r--   0 kai       (1000) kai       (1000)    36123 2023-07-05 14:24:46.000000 pystage-0.1.0.dev0/src/pystage/en/stage.py
+drwxr-xr-x   0 kai       (1000) kai       (1000)        0 2024-06-03 10:48:21.156048 pystage-0.1.0.dev0/src/pystage/fonts/
+-rw-r--r--   0 kai       (1000) kai       (1000)   167336 2023-07-05 07:39:55.000000 pystage-0.1.0.dev0/src/pystage/fonts/roboto-bold.ttf
+-rw-r--r--   0 kai       (1000) kai       (1000)   167000 2023-07-05 07:39:55.000000 pystage-0.1.0.dev0/src/pystage/fonts/roboto-light.ttf
+-rw-r--r--   0 kai       (1000) kai       (1000)   168260 2023-07-05 07:39:55.000000 pystage-0.1.0.dev0/src/pystage/fonts/roboto-regular.ttf
+drwxr-xr-x   0 kai       (1000) kai       (1000)        0 2024-06-03 10:48:21.159382 pystage-0.1.0.dev0/src/pystage/images/
+-rw-r--r--   0 kai       (1000) kai       (1000)    26719 2023-07-05 07:39:55.000000 pystage-0.1.0.dev0/src/pystage/images/grid.svg
+-rw-------   0 kai       (1000) kai       (1000)     1137 2023-07-05 07:39:55.000000 pystage-0.1.0.dev0/src/pystage/images/pen.png
+-rw-------   0 kai       (1000) kai       (1000)     2523 2023-07-05 07:39:55.000000 pystage-0.1.0.dev0/src/pystage/images/say.png
+-rw-------   0 kai       (1000) kai       (1000)     2650 2023-07-05 07:39:55.000000 pystage-0.1.0.dev0/src/pystage/images/think.png
+-rw-r--r--   0 kai       (1000) kai       (1000)     5177 2023-07-05 07:39:55.000000 pystage-0.1.0.dev0/src/pystage/images/zombie_idle.png
+drwxr-xr-x   0 kai       (1000) kai       (1000)        0 2024-06-03 10:48:21.159382 pystage-0.1.0.dev0/src/pystage/l10n/
+-rw-r--r--   0 kai       (1000) kai       (1000)        0 2023-07-05 07:39:55.000000 pystage-0.1.0.dev0/src/pystage/l10n/__init__.py
+-rw-r--r--   0 kai       (1000) kai       (1000)     7399 2023-07-05 07:39:55.000000 pystage-0.1.0.dev0/src/pystage/l10n/__main__.py
+-rw-r--r--   0 kai       (1000) kai       (1000)     2925 2023-07-05 07:39:55.000000 pystage-0.1.0.dev0/src/pystage/l10n/api.py
+-rw-r--r--   0 kai       (1000) kai       (1000)     2406 2023-07-05 07:39:55.000000 pystage-0.1.0.dev0/src/pystage/l10n/translations.py
+drwxr-xr-x   0 kai       (1000) kai       (1000)        0 2024-06-03 10:48:21.159382 pystage-0.1.0.dev0/src/pystage/sounds/
+-rw-r--r--   0 kai       (1000) kai       (1000)    63036 2023-07-05 07:39:55.000000 pystage-0.1.0.dev0/src/pystage/sounds/dancehead2.wav
+-rw-r--r--   0 kai       (1000) kai       (1000)   192012 2023-07-05 07:39:55.000000 pystage-0.1.0.dev0/src/pystage/sounds/guitar.wav
+-rw-r--r--   0 kai       (1000) kai       (1000)     3623 2023-07-05 07:39:55.000000 pystage-0.1.0.dev0/src/pystage/util.py
+drwxr-xr-x   0 kai       (1000) kai       (1000)        0 2024-06-03 10:48:21.162715 pystage-0.1.0.dev0/src/pystage.egg-info/
+-rw-r--r--   0 kai       (1000) kai       (1000)     5123 2024-06-03 10:48:21.000000 pystage-0.1.0.dev0/src/pystage.egg-info/PKG-INFO
+-rw-r--r--   0 kai       (1000) kai       (1000)     1541 2024-06-03 10:48:21.000000 pystage-0.1.0.dev0/src/pystage.egg-info/SOURCES.txt
+-rw-r--r--   0 kai       (1000) kai       (1000)        1 2024-06-03 10:48:21.000000 pystage-0.1.0.dev0/src/pystage.egg-info/dependency_links.txt
+-rw-r--r--   0 kai       (1000) kai       (1000)       21 2024-06-03 10:48:21.000000 pystage-0.1.0.dev0/src/pystage.egg-info/requires.txt
+-rw-r--r--   0 kai       (1000) kai       (1000)        8 2024-06-03 10:48:21.000000 pystage-0.1.0.dev0/src/pystage.egg-info/top_level.txt
```

### Comparing `pystage-0.0.9/LICENSE` & `pystage-0.1.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `pystage-0.0.9/setup.cfg` & `pystage-0.1.0.dev0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = pystage
-version = 0.0.9
+version = 0.1.0.dev
 author = Kai Eckert
-author_email = eckert@hdm-stuttgart.de
+author_email = k.eckert@hs-mannheim.de
 description = Scratch-like Python programming
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pystage/pystage
 license = MIT
 project_urls = 
 	Bug Tracker = https://github.com/pystage/pystage/issues
```

### Comparing `pystage-0.0.9/src/pystage/convert/code_writer.py` & `pystage-0.1.0.dev0/src/pystage/convert/code_writer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import io
-import sys
 import textwrap
 import re
 import logging
 import inspect
-import ast
 import importlib
 import dis
-from jinja2 import Template, Environment
+from jinja2 import Environment
 from jinja2.exceptions import UndefinedError
 logger = logging.getLogger(__name__)
 
 from pystage.core.sprite import CoreSprite
 from pystage.core.stage import CoreStage
 
+to_underscore = re.compile(r"[^A-Za-z0-9_]")
+valid_variable_start = re.compile(r"[a-zA-Z_]")
+multiple_underscores = re.compile(r"_+")
 
 
 def quoted(value):
     if not isinstance(value, str):
         return value
     if value.startswith("\""):
         return value
@@ -59,25 +59,34 @@
         self.comments = []
         self.last_id = 0
         self.current_sprite = ""
         self.jinja_environment = Environment(trim_blocks=True, lstrip_blocks=True)
         self.jinja_environment.filters["global_sound"] = lambda name: self.global_sound(name)
         self.jinja_environment.filters["global_costume"] = lambda name: self.global_costume(name)
         self.jinja_environment.filters["global_backdrop"] = lambda name: self.global_backdrop(name)
+        self.jinja_environment.filters["global_sprite"] = lambda name: self.get_sprite_var(unquoted(name))
         
         logger.debug("CodeWriter created.")
 
 
     def set_sprite(self, name):
         self.current_sprite = name
 
 
     def get_sprite_var(self, name=None):
         def to_python(name: str):
-            return name.lower().replace(" ", "_"). replace("-", "_")
+            vname = name.lower().strip()
+            # Replace everything that is not allowed in a 
+            # variable name with underscores
+            vname = to_underscore.sub("_", vname)
+            vname = multiple_underscores.sub("_", vname)
+            # Check of the variable does not start with a number
+            if not valid_variable_start.fullmatch(vname[0]):
+                vname = "_" + vname
+            return vname
         if name is None:
             return to_python(self.current_sprite)
         else:
             return to_python(name)
 
     def get_sprite_or_stage(self, name=None):
         if not name:
@@ -257,14 +266,27 @@
             if not "NEXT" in text:
                 text += "\n{{NEXT}}"
         for param in block["params"]:
             context[param] = self.process(block["params"][param])
         context["CURRENT_SPRITE"] = self.get_sprite_var()
         if "{{ID}}" in text:
             context["ID"] = self.get_id()
+
+        # if {{NEXT | indent (4)}} is still in text, but there is no
+        # NEXT in context, then it means the Scratch “hat” block is empty,
+        # so set NEXT to "pass", and the function is essentially empty.
+        if "indent(4)" in text:
+            if "NEXT" in text and not context.get("NEXT"):
+                context["NEXT"] = "pass"
+            if "SUBSTACK" in text and not context.get("SUBSTACK"):
+                context["SUBSTACK"] = "pass"
+            if "SUBSTACK2" in text and not context.get("SUBSTACK2"):
+                context["SUBSTACK2"] = "pass"
+        if "{{CONDITION}}" in text and not context.get("CONDITION"):
+            context["CONDITION"] = "None"
         template = self.jinja_environment.from_string(text)
         try:
             text = template.render(context)
         except UndefinedError as e:
             print(f"Template variable not available: {e}")
         return text
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pystage-0.0.9/src/pystage/convert/sb3.py` & `pystage-0.1.0.dev0/src/pystage/convert/sb3.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from pystage.l10n.api import get_translated_function
 
 from pystage.convert import CodeWriter, sb3_templates
 
 logger = logging.getLogger(__name__)
 
 '''
-For the conversion, we create a simplified version of the 
+For the conversion, we create a simplified version of the
 block trees that is used in the code template functions.
 '''
 
 
 # Target (intermediate) structure
 # project = {
 #         "costumes": {
@@ -67,17 +67,17 @@
 #                 "sounds": [{
 #                       "md5": "abcd..."
 #                       "local_name": "cat1",
 #                       },
 #                   ],
 #                 "currentCostume": 0
 #                 },
-# 
+#
 #             ],
-# 
+#
 #         }
 
 class DictClass(OrderedDict):
     '''
     A dictionary that can be accessed via dot notation for convenience.
     '''
 
@@ -96,20 +96,20 @@
     # 7: integer, 8: angle, 9: color, 10: string
     # 11: broadcast, 12: variable, 13: list
 
     input_type = i[0]
     value = i[1]
 
     if input_type in [4, 5, 8]:
-        if value.strip() == '':
+        if isinstance(value, str) and value.strip() == '':
             value = 0
         else:
             value = float(value)
     elif input_type in [6, 7]:
-        if value.strip() == '':
+        if isinstance(value, str) and value.strip() == '':
             value = 0
         else:
             value = int(value)
     elif input_type == 9:
         h = value.lstrip("#")
         value = tuple(int(h[i:i + 2], 16) for i in (0, 2, 4))
     elif input_type == 12:
@@ -145,14 +145,17 @@
         "next": False,
         "stage": stage
     })
     for f in block["fields"]:
         res["params"][f] = f'"{block["fields"][f][0]}"'
     for i in block["inputs"]:
         value = block["inputs"][i][1]
+        if not value:
+            # empty if condition
+            continue
         if isinstance(value, list):
             res["params"][i] = get_input_value(value, stage)
         else:
             res["params"][i] = get_block(blocks[value], blocks, stage)
     if block["next"]:
         res["next"] = get_block(blocks[block["next"]], blocks, stage)
     return res
@@ -175,14 +178,20 @@
     i = 2
     while f"{iname}.{ext}" in global_names:
         iname = f"{name}_{i}"
         i += 1
     global_names.add(f"{iname}.{ext}")
     return iname, ext
 
+def get_sb3_data(filename):
+    archive = zipfile.ZipFile(filename, 'r')
+    with archive.open("project.json") as f:
+        data = json.loads(f.read())
+    return data
+
 def get_intermediate(data, name):
     hat_blocks = [
         "event_whenthisspriteclicked",
         "event_whenbroadcastreceived",
         "event_whenflagclicked",
         "event_whenkeypressed",
         "event_whenbackdropswitchesto",
@@ -203,14 +212,15 @@
         sprite = DictClass()
         sprite.update({
             "name": target['name'],
             "blocks": [],
             "costumes": [],
             "sounds": [],
             "variables": {}, # name: value
+            "monitors": [], # name: value
             "currentCostume": target["currentCostume"],
             "layerOrder": target["layerOrder"],
             "visible": target["visible"] if "visible" in target else True,
             "x": target["x"] if "x" in target else 0,
             "y": target["y"] if "y" in target else 0,
             "size": target["size"] if "size" in target else 100,
             "volume": target["volume"] if "volume" in target else 100,
@@ -255,34 +265,61 @@
                 }
             sprite["sounds"].append({
                 "md5": s["assetId"],
                 "local_name": s["name"],
             })
         for key in target["variables"]:
             v = target["variables"][key]
+            variable = {}
             sprite["variables"][v[0]] = v[1]
 
+    for m in data["monitors"]:
+        if not m["visible"]:
+            continue
+        monitor = {}
+        if not m["spriteName"]:
+            sprite = project["stage"]
+        else:
+            for s in project["sprites"]:
+                if s["name"] == m["spriteName"]:
+                    sprite = sprite
+                    break
+        monitor["style"] = m["mode"]
+        if monitor["style"] == "default":
+            monitor["style"] == "normal"
+        monitor["x"] = m["x"]
+        monitor["y"] = m["y"]
+        monitor["opcode"] = m["opcode"]
+        if "VARIABLE" in m["params"]:
+            monitor["variable"] = m["params"]["VARIABLE"]
+        sprite["monitors"].append(monitor)
+
     return project
 
 
-def get_python(project, language="core"):
+def get_python(project, language="core", project_link=None):
     lang_module = importlib.import_module(f"pystage.{language}")
     sprite_class = lang_module.sprite_class.__name__
     stage_class = lang_module.stage_class.__name__
     add_backdrop = get_translated_function("pystage_addbackdrop", language, stage=True)
     add_costume = get_translated_function("pystage_addcostume", language)
     add_sound = get_translated_function("pystage_addsound", language)
     add_variable = get_translated_function("pystage_makevariable", language)
     create_sprite = get_translated_function("pystage_createsprite", language, stage=True)
     play = get_translated_function("pystage_play", language, stage=True)
-    res = textwrap.dedent(f'''\
+    res = ""
+    if project_link:
+        res += textwrap.dedent(f'''\
+        # Online Converter, URL: {project_link}
+        ''')
+    res += textwrap.dedent(f'''\
             # {project['name']} (pyStage, converted from Scratch 3)
-            
+
             from pystage.{language} import {sprite_class}, {stage_class}
-            
+
             ''')
     writer = CodeWriter(project, sb3_templates.templates, language)
     writer.set_sprite(project["stage"]["name"])
     stage_var = writer.get_sprite_var()
     backdrops = []
     for bd in project["stage"]["costumes"]:
         backdrops.append(writer.global_backdrop(bd["local_name"], False))
@@ -293,23 +330,42 @@
         res += textwrap.dedent(f'''\
                 {stage_var}.{add_backdrop}('{bd}')
                 ''')
     for v in project["stage"]["variables"]:
         res += textwrap.dedent(f'''\
                 {stage_var}.{add_variable}('{v}')
                 ''')
+    for monitor in project["stage"]["monitors"]:
+        # Only variable monitors are currently implemented
+        if not "variable" in monitor:
+            continue
+        res += textwrap.dedent(f'''\
+                {stage_var}.{get_translated_function("data_showvariable", language)}("{monitor["variable"]}")
+                {stage_var}.{get_translated_function("pystage_setmonitorposition", language)}("{monitor["variable"]}", {-240 + monitor["x"]}, {180 - monitor["y"]})
+                ''')
+        if monitor["style"] == "large":
+            res += textwrap.dedent(f'''\
+                    {stage_var}.{get_translated_function("pystage_setmonitorstyle_large", language)}("{monitor["variable"]}")
+                    ''')
     for block in project["stage"]["blocks"]:
         res += writer.process(block)
     for sprite in project["sprites"]:
         writer.set_sprite(sprite["name"])
         sprite_var = writer.get_sprite_var()
         costumes = [(writer.global_costume(c["local_name"], False), c) for c in sprite["costumes"]]
         sounds = [writer.global_sound(s["local_name"], False) for s in sprite["sounds"]]
+        
+        # Generate initialization code for each sprite.
+        res += textwrap.dedent(f"""\
+                
+                # Create and initialize sprite '{sprite_var}'
+                """)
         res += textwrap.dedent(f'''\
                 {sprite_var} = {stage_var}.{create_sprite}(None)
+                {sprite_var}.{get_translated_function("pystage_setname", language)}("{sprite["name"]}")
                 {sprite_var}.{get_translated_function("motion_setx", language)}({sprite["x"]})
                 {sprite_var}.{get_translated_function("motion_sety", language)}({sprite["y"]})
                 {sprite_var}.{get_translated_function("looks_gotofrontback_back", language)}()
                 {sprite_var}.{get_translated_function("looks_goforwardbackwardlayers_forward", language)}({sprite["layerOrder"]})
                 ''')
         if sprite["direction"] != 90:
             res += textwrap.dedent(f"""\
@@ -345,33 +401,82 @@
         for s in sounds:
             res += textwrap.dedent(f'''\
                 {sprite_var}.{add_sound}('{s}')
                 ''')
 
         for v in sprite["variables"]:
             res += textwrap.dedent(f'''\
-                    {stage_var}.{add_variable}('{v}')
+                    {sprite_var}.{add_variable}('{v}')
+                    ''')
+        for monitor in sprite["monitors"]:
+            # Only variable monitors are currently implemented
+            if not "variable" in monitor:
+                continue
+            res += textwrap.dedent(f'''\
+                    {sprite_var}.{get_translated_function("data_showvariable", language)}("{monitor["variable"]}")
+                    {sprite_var}.{get_translated_function("pystage_setmonitorposition", language)}("{monitor["variable"]}", {-240 + monitor["x"]}, {180 - monitor["y"]})
                     ''')
+            if monitor["style"] == "large":
+                res += textwrap.dedent(f'''\
+                        {sprite_var}.{get_translated_function("pystage_setmonitorstyle_large", language)}("{monitor["variable"]}")
+                        ''')
+    
+    # Now generate the code for each sprite.
+    for sprite in project["sprites"]:
+        writer.set_sprite(sprite["name"])
+        sprite_var = writer.get_sprite_var()
+        res += textwrap.dedent(f"""\
+                
+                # Scratch Blocks for '{sprite_var}'
+                """)
         for block in sprite["blocks"]:
             res += writer.process(block)
+
+
     res += textwrap.dedent(f'''\
-            
+
             {stage_var}.{play}()
             ''')
     return res
 
 
 def print_python(project, language="core"):
     print(get_python(project, language))
 
 
+def create_project(file_name, project_name, project, directory, language="core", project_link=None):
+    print(f"Creating project: {project_name}")
+    print(f"Exporting to: {directory}")
+    archive = zipfile.ZipFile(file_name, 'r')
+    dp = Path(directory)
+    if dp.exists():
+        raise("Directory must not exist at this point, but it does: {}".format(directory))
+    os.mkdir(dp)
+    os.mkdir(dp / "images")
+    os.mkdir(dp / "sounds")
+    for key in project["costumes"]:
+        c = project["costumes"][key]
+        with archive.open(f'{key}.{c["extension"]}') as infile:
+            with open(dp / "images" / f'{c["global_name"]}.{c["extension"]}', "wb") as outfile:
+                outfile.write(infile.read())
+    for key in project["sounds"]:
+        s = project["sounds"][key]
+        with archive.open(f'{key}.{s["extension"]}') as infile:
+            with open(dp / "sounds" / f'{s["global_name"]}.{s["extension"]}', "wb") as outfile:
+                outfile.write(infile.read())
+    with open(dp / f'{project_name}.py', "w", encoding="utf-8") as pyfile:
+        pyfile.write(get_python(project, language=language, project_link=project_link))
+
+
+
 ##
 # Main
 #
 
+
 if __name__ == "__main__":
 
     parser = argparse.ArgumentParser(
         prog="python -m pystage.convert.sb3",
         description="Convert Scratch 3 (sb3) files to Python.")
     parser.add_argument("file", metavar="FILE", type=str, help="the sb3 file to be converted")
     parser.add_argument("-i", "--intermediate", action="store_true", help="print intermediate code representation")
@@ -384,51 +489,33 @@
     args = parser.parse_args()
 
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
     elif args.verbose:
         logging.basicConfig(level=logging.INFO)
 
-    archive = zipfile.ZipFile(args.file, 'r')
-    with archive.open("project.json") as f:
-        project_name = to_filename(Path(args.file).stem)
-        data = json.loads(f.read())
-        if args.sb3_json:
-            print(json.dumps(data, indent=2))
-            sys.exit(0)
-        project = get_intermediate(data, project_name)
-        if args.intermediate:
-            print(json.dumps(project, indent=2))
+    project_name = to_filename(Path(args.file).stem)
+    data = get_sb3_data(args.file)
+    if args.sb3_json:
+        print(json.dumps(data, indent=2))
+        sys.exit(0)
+    project = get_intermediate(data, project_name)
+    if args.intermediate:
+        print(json.dumps(project, indent=2))
+        sys.exit(1)
+    elif args.python:
+        print_python(project, args.language)
+        sys.exit(1)
+    else:
+        directory = project_name
+        if args.directory:
+            directory = args.directory
+        print(f"Exporting to: {directory}")
+        dp = Path(directory)
+        if dp.exists() and not dp.is_dir:
+            print("Output directory exists, but is not a directory. Use -d to specify another directory.")
             sys.exit(1)
-        elif args.python:
-            print_python(project, args.language)
+        elif dp.exists() and next(dp.iterdir(), False):
+            print("Output directory is not empty. Use -d to specify another one.")
             sys.exit(1)
-        else:
-            print(f"Creating project: {project_name}")
-            directory = project_name
-            if args.directory:
-                directory = args.directory
-            print(f"Exporting to: {directory}")
-            dp = Path(directory)
-            if dp.exists() and not dp.is_dir:
-                print("Output directory exists, but is not a directory. Use -d to specify another directory.")
-                sys.exit(1)
-            elif dp.exists() and next(dp.iterdir(), False):
-                print("Output directory is not empty. Use -d to specify another one.")
-                sys.exit(1)
-            elif not dp.exists():
-                print(f"Creating directory: {dp}")
-                os.mkdir(dp)
-            os.mkdir(dp / "images")
-            os.mkdir(dp / "sounds")
-            for key in project["costumes"]:
-                c = project["costumes"][key]
-                with archive.open(f'{key}.{c["extension"]}') as infile:
-                    with open(dp / "images" / f'{c["global_name"]}.{c["extension"]}', "wb") as outfile:
-                        outfile.write(infile.read())
-            for key in project["sounds"]:
-                s = project["sounds"][key]
-                with archive.open(f'{key}.{s["extension"]}') as infile:
-                    with open(dp / "sounds" / f'{s["global_name"]}.{s["extension"]}', "wb") as outfile:
-                        outfile.write(infile.read())
-            with open(dp / f'{project_name}.py', "w", encoding="utf-8") as pyfile:
-                pyfile.write(get_python(project))
+        elif not dp.exists():
+            create_project(args.file, project_name, project, directory, args.language)
```

### Comparing `pystage-0.0.9/src/pystage/convert/sb3_templates.py` & `pystage-0.1.0.dev0/src/pystage/convert/sb3_templates.py`

 * *Files 13% similar despite different names*

```diff
@@ -38,15 +38,29 @@
 
                 def {{func}}_{{ID}}(self):
                     {{NEXT | indent(4)}}
 
                 {{CURRENT_SPRITE}}.{{func}}({{func}}_{{ID}})
                 
                 ''',
+
+        "event_whengreaterthan": '''\
+                def {{func}}_{{ID}}(self):
+                    {{NEXT | indent(4)}}
+                {{CURRENT_SPRITE}}.{{func}}({{VALUE}}, {{func}}_{{ID}})
                 
+                ''',
+
+        "event_whenbackdropswitchesto": '''\
+                def {{func}}_{{ID}}(self):
+                    {{NEXT | indent(4)}}
+                {{CURRENT_SPRITE}}.{{func}}({{BACKDROP | global_backdrop}}, {{func}}_{{ID}})
+                
+                ''',
+
         "control_start_as_clone": '''\
 
                 def {{func}}_{{ID}}(self):
                     {{NEXT | indent(4)}}
 
                 {{CURRENT_SPRITE}}.{{func}}({{func}}_{{ID}})
                 
@@ -101,10 +115,14 @@
         "operator_round": "round({{NUM}})",
         "operator_subtract": "({{NUM1}} - {{NUM2}})",
 
         "looks_costume": "{{COSTUME | global_costume}}",
         "looks_backdrops": "{{BACKDROP | global_backdrop}}",
         "sound_sounds_menu": "{{SOUND_MENU | global_sound }}",
 
+        "sensing_keyoptions": "{{KEY_OPTION}}",
+        "sensing_distancetomenu": "{{DISTANCETOMENU | global_sprite}}",
+        "sensing_touchingobjectmenu": "{{TOUCHINGOBJECTMENU | global_sprite}}",
+
                 }
```

### Comparing `pystage-0.0.9/src/pystage/core/_control.py` & `pystage-0.1.0.dev0/src/pystage/core/_control.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         pass
     control_stop_all.opcode="control_stop"
     control_stop_all.param="STOP_OPTION"
     control_stop_all.value="all"
 
     def control_stop_this(self):
         # This is equivalent to return
-        pass
+        self.code_manager.current_block.running = False
     control_stop_this.opcode="control_stop"
     control_stop_this.param="STOP_OPTION"
     control_stop_this.value="this script"
 
     def control_stop_other(self):
         pass
     control_stop_other.opcode="control_stop"
@@ -44,11 +44,11 @@
 
     def control_delete_this_clone(self):
         pass
     control_delete_this_clone.translation = "control_deletethisclone"
 
 
     # This is actually an event but Scratch has the hat block under "Control"
-    def control_start_as_clone(self, key, generator_function, name="", no_refresh=False):
+    def control_start_as_clone(self, generator_function, name="", no_refresh=False):
         pass
     control_start_as_clone.translation = "control_startasclone"
```

### Comparing `pystage-0.0.9/src/pystage/core/_events.py` & `pystage-0.1.0.dev0/src/pystage/core/_events.py`

 * *Files identical despite different names*

### Comparing `pystage-0.0.9/src/pystage/core/_looks.py` & `pystage-0.1.0.dev0/src/pystage/core/_looks.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     looks_seteffectto_brightness.opcode="looks_seteffectto"
     looks_seteffectto_brightness.param="EFFECT"
     looks_seteffectto_brightness.value="BRIGHTNESS"
     looks_seteffectto_brightness.translation="looks_effect_brightness"
     
 
     def looks_seteffectto_ghost(self, value):
-        pass
+        self.ghost = value
     
     looks_seteffectto_ghost.opcode="looks_seteffectto"
     looks_seteffectto_ghost.param="EFFECT"
     looks_seteffectto_ghost.value="GHOST"
     looks_seteffectto_ghost.translation="looks_effect_ghost"
     
 
@@ -129,15 +129,15 @@
     looks_changeeffectby_brightness.opcode="looks_changeeffectby"
     looks_changeeffectby_brightness.param="EFFECT"
     looks_changeeffectby_brightness.value="BRIGHTNESS"
     looks_changeeffectby_brightness.translation="looks_effect_brightness"
     
 
     def looks_changeeffectby_ghost(self, value):
-        pass
+        self.ghost += value
     
     looks_changeeffectby_ghost.opcode="looks_changeeffectby"
     looks_changeeffectby_ghost.param="EFFECT"
     looks_changeeffectby_ghost.value="GHOST"
     looks_changeeffectby_ghost.translation="looks_effect_ghost"
     
 
@@ -171,14 +171,15 @@
 
 class _LooksSprite(_Looks):
 
     def __init__(self):
         super().__init__()
         self.bubble_manager = BubbleManager(self)
         self.size = 100
+        self.ghost = 0 # 0 - visible / 100 - transparent
         self.visible = True
 
 
     def pystage_addcostume(self, name, center_x=None, center_y=None, factor=1):
         self.costume_manager.add_costume(name, center_x, center_y, factor)
 
     def pystage_replacecostume(self, index, name, center_x=None, center_y=None, factor=1):
@@ -195,15 +196,15 @@
         self.bubble_manager.say(text)
 
 
     def looks_thinkforsecs(self, text, secs):
         pass
 
     def looks_think(self, text):
-        self.bubble_manager.say(text, Bubble.THINK)
+        self.bubble_manager.think(text)
 
     def looks_switchcostumeto(self, costume):
         self.costume_manager.switch_costume(costume)
 
     def looks_nextcostume(self):
         self.costume_manager.next_costume()
 
@@ -212,15 +213,14 @@
         # this is percentage
         self.size += percent
 
 
     def looks_setsizeto(self, percent):
         self.size = percent
 
-
     def looks_show(self):
         print("Show", self)
         if self.visible:
             return
         self.visible = True
         self.stage._update_visible()
 
@@ -230,38 +230,38 @@
         if not self.visible:
             return
         self.visible = False
         self.stage._update_visible()
 
 
     def looks_gotofrontback_front(self):
-        pass
+        self.stage.sprites.to_front(self)
 
     looks_gotofrontback_front.opcode="looks_gotofrontback"
     looks_gotofrontback_front.param="FRONT_BACK"
     looks_gotofrontback_front.value="front"
 
     
     def looks_gotofrontback_back(self):
-        pass
+        self.stage.sprites.to_back(self)
 
     looks_gotofrontback_back.opcode="looks_gotofrontback"
     looks_gotofrontback_back.param="FRONT_BACK"
     looks_gotofrontback_back.value="back"
 
 
     def looks_goforwardbackwardlayers_forward(self, value):
-        pass
+        self.stage.sprites.layer_forward(self, value)
 
     looks_goforwardbackwardlayers_forward.opcode="looks_goforwardbackwardlayers"
     looks_goforwardbackwardlayers_forward.param="FORWARD_BACKWARD"
     looks_goforwardbackwardlayers_forward.value="forward"
 
     def looks_goforwardbackwardlayers_backward(self, value):
-        pass
+        self.stage.sprites.layer_backward(self, value)
 
     looks_goforwardbackwardlayers_backward.opcode="looks_goforwardbackwardlayers"
     looks_goforwardbackwardlayers_backward.param="FORWARD_BACKWARD"
     looks_goforwardbackwardlayers_backward.value="backward"
 
 
     def looks_costumenumbername_number(self):
```

### Comparing `pystage-0.0.9/src/pystage/core/_motion.py` & `pystage-0.1.0.dev0/src/pystage/core/_motion.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import pygame
 import enum
 import math
 from pystage.core._sensing import _Sensing
 from pystage.core._looks import _LooksSprite
 from pystage.core.assets import CostumeManager
 import random
 
@@ -11,31 +12,37 @@
 
 def _rad2deg(rad):
     return rad / (2 * math.pi) * 360
 
 class _Motion(_Sensing):
     def __init__(self):
         super().__init__()
-        self.x = 0.0
-        self.y = 0.0
-        self.direction = 90
+        # The direction is internally stored as common angle in degrees
+        # (counter-clockwise, 0 to the right)
+        # Scratch uses a clockwise angle with 0 pointing to top
+        self._direction = 0
+        # Position is stored internally as PyGame coordinates
+        # and refers to the center of the costume.
+        self._pos = pygame.Vector2(0, 0)
+        self.draggable = False
+        self.motion_setx(0)
+        self.motion_sety(0)
 
     def motion_turnleft(self, deg):
-        self.direction -= deg
+        self._direction += deg
 
 
     def motion_turnright(self, deg):
-        self.direction += deg
+        self._direction -= deg
 
 
     def motion_movesteps(self, steps):
-        old_x = self.x
-        old_y = self.y
-        self.x = self.x + steps * math.cos(_deg2rad(self.direction - 90))
-        self.y = self.y - steps * math.sin(_deg2rad(self.direction - 90))
+        dx = steps * math.cos(_deg2rad(self._direction))
+        dy = steps * math.sin(_deg2rad(self._direction))
+        self._pos += pygame.Vector2(dx, -dy) # PyGame has inverted y axis
 
 
     def motion_goto_random(self):
         half_width = int(self.stage.width/2)
         half_height = int(self.stage.height/2)
         x = random.randint(-half_width, half_width)
         y = random.randint(-half_height, half_height)
@@ -51,22 +58,22 @@
 
     motion_goto_pointer.opcode = "motion_goto"
     motion_goto_pointer.param = "TO"
     motion_goto_pointer.value = "_mouse_"
 
 
     def motion_goto_sprite(self, sprite):
-        self.motion_gotoxy(sprite.x, sprite.y)
+        self.motion_gotoxy(sprite.x_position(), sprite.y_position())
 
     motion_goto_sprite.opcode = "motion_goto"
 
 
     def motion_gotoxy(self, x, y):
-        self.x = x
-        self.y = y
+        self.motion_setx(x)
+        self.motion_sety(y)
 
 
     def motion_glideto_random(self, secs):
         half_width = int(self.stage.width/2)
         half_height = int(self.stage.height/2)
         x = random.randint(-half_width, half_width)
         y = random.randint(-half_height, half_height)
@@ -92,66 +99,73 @@
 
     motion_glideto_sprite.opcode = "motion_glideto"
 
 
     def motion_glidesecstoxy(self, secs, x, y):
         self.code_manager.current_block.gliding_seconds = secs
         self.code_manager.current_block.add_to_wait_time = secs
-        self.code_manager.current_block.gliding_start_position = (self.x, self.y)
+        self.code_manager.current_block.gliding_start_position = (self.motion_xposition(), self.motion_yposition())
         self.code_manager.current_block.gliding_end_position = (x, y)
         self.code_manager.current_block.gliding = True
 
     def motion_pointindirection(self, direction):
-        self.direction = direction
+        # Scratch uses clock-wise directions with 0 to the top
+        # We have anti-clockwise with 0 to the right
+        self._direction = 90 - direction
 
     def motion_pointtowards_pointer(self):
-        dx = self.sensing_mousex() - self.x
-        dy = self.sensing_mousey() - self.y
-        self.direction = 90 - _rad2deg(math.atan2(dy, dx))
+        dx = self.sensing_mousex() - self.motion_xposition()
+        dy = self.sensing_mousey() - self.motion_yposition()
+        self._direction = _rad2deg(math.atan2(dy, dx))
 
     motion_pointtowards_pointer.opcode = "motion_pointtowards"
     motion_pointtowards_pointer.param = "TOWARDS"
     motion_pointtowards_pointer.value = "_mouse_"
 
     def motion_pointtowards_sprite(self, sprite):
-        dx = sprite.x - self.x
-        dy = sprite.y - self.y
-        self.direction = 90 - _rad2deg(math.atan2(dy, dx))
+        dx = sprite.motion_xposition() - self.motion_xposition()
+        dy = sprite.motion_yposition() - self.motion_yposition()
+        self._direction = _rad2deg(math.atan2(dy, dx))
 
     motion_pointtowards_sprite.opcode = "motion_pointtowards"
 
+
     def motion_changexby(self, value):
-        self.x += value
+        self._pos.x += value
+
 
     def motion_setx(self, value):
-        self.x = value
+        self._pos.x = value + self.stage.center_x
+
 
     def motion_changeyby(self, value):
-        self.y += value
+        self._pos.y -= value # inverted y axis
+
 
     def motion_sety(self, value):
-        self.y = value
+        self._pos.y = -value + self.stage.center_y
+
 
     def motion_ifonedgebounce(self):
         if self.rect.left < 0:
-            self.direction = -self.direction
-            self.rect.left = 0
-            self._update_pos_from_rect()
+            self._direction = 180 - self._direction
+            self.costume_manager.update_sprite_image()
+            self._pos.x -= self.rect.left
         elif self.rect.right > self.stage.width:
-            self.direction = -self.direction
-            self.rect.right = self.stage.width
-            self._update_pos_from_rect()
+            self._direction = 180 - self._direction
+            self.costume_manager.update_sprite_image()
+            self._pos.x -= self.rect.right - self.stage.width
         elif self.rect.top < 0:
-            self.direction = 180 - self.direction
-            self.rect.top = 0
-            self._update_pos_from_rect()
+            self._direction = -self._direction
+            self.costume_manager.update_sprite_image()
+            self._pos.y -= self.rect.top
         elif self.rect.bottom > self.stage.height:
-            self.direction = 180 - self.direction
-            self.rect.bottom = self.stage.height
-            self._update_pos_from_rect()
+            self._direction = -self._direction
+            self.costume_manager.update_sprite_image()
+            self._pos.y -= self.rect.bottom - self.stage.height
 
 
     def motion_setrotationstyle_leftright(self):
         self.costume_manager.rotation_style = CostumeManager.LEFT_RIGHT
 
     motion_setrotationstyle_leftright.opcode = "motion_setrotationstyle"
     motion_setrotationstyle_leftright.param = "STYLE"
@@ -168,33 +182,29 @@
     def motion_setrotationstyle_allaround(self):
         self.costume_manager.rotation_style = CostumeManager.ALL_AROUND
 
     motion_setrotationstyle_allaround.opcode = "motion_setrotationstyle"
     motion_setrotationstyle_allaround.param = "STYLE"
     motion_setrotationstyle_allaround.value = "all around"
 
-    # Setters and getters are questionable, but 
-    # this way we would clearly adapt the Scratch API
-    # We could get rid of them for a direct access 
-    # to x, y, direction and so on. Direct access is of 
-    # course available anyway.
+
     def motion_xposition(self):
-        return self.x
+        return self._pos.x - self.stage.center_x
 
     motion_xposition.return_type = float
 
 
     def motion_yposition(self):
-        return self.y
+        return -self._pos.y + self.stage.center_y
 
     motion_yposition.return_type = float
 
 
     def motion_direction(self):
         # Scratch always keeps angles between -180 and 180
-        dir = self.direction % 360
+        dir = (90 - self._direction) % 360
         if dir <= 180:
             return dir
         else:
             return dir - 360
 
     motion_direction.return_type = float
```

### Comparing `pystage-0.0.9/src/pystage/core/_operators.py` & `pystage-0.1.0.dev0/src/pystage/core/_operators.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,19 +12,32 @@
         ops = {
                 'abs': abs,
                 'floor': math.floor,
                 'ceiling': math.ceil,
                 'sqrt': math.sqrt,
                 'sin': lambda n: math.sin((math.pi * n) / 180),
                 'cos': lambda n: math.cos((math.pi * n) / 180),
-                'tan': math.tan,
+                'tan': lambda n: math.tan((math.pi * n) / 180) if not n == 90 else float("inf"),
                 'asin': lambda n: (math.asin(n) * 180) / math.pi,
                 'acos': lambda n: (math.acos(n) * 180) / math.pi,
                 'atan': lambda n: (math.atan(n) * 180) / math.pi,
-                'ln': math.log,
-                'log': math.log,
+                'ln': lambda n : math.log(n) if not n == 0 else -float("inf"),
+                'log': lambda n: math.log10(n) if not n == 0 else -float("inf"),
                 'e ^': math.exp,
                 '10 ^': lambda n: math.pow(10, n),
                 }
         if operator not in ops:
             raise ValueError(f"Operator {operator} not supported.")
-        return ops[operator](number)
+        
+        try:
+            value = ops[operator](number)
+            if value == float("inf"):
+                return "Infinity"
+            elif value == -float("inf"):
+                return "-Infinity"
+            # avoid for situations like sin(30) == 0.49999999999999994
+            return round(value, 10)
+        except ValueError:
+            # print(f"ValueError: math domain error: {operator}({number})")
+            return "NaN"
+        except OverflowError:
+            return "Infinity"
```

### Comparing `pystage-0.0.9/src/pystage/core/_pen.py` & `pystage-0.1.0.dev0/src/pystage/core/_pen.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,148 +1,170 @@
 import pygame
 from pystage.core._base_sprite import BaseSprite
 
 
+
+def int2(vec2):
+    x = int(round(vec2[0]))
+    y = int(round(vec2[1]))
+    return pygame.Vector2(x, y)
+
+
 class _Pen(BaseSprite):
 
     def __init__(self):
         super().__init__()
 
         self.pen = False
-        self.pen_color = (255,0,0)
+        self.pen_color = pygame.Color(255,0,0)
         self.pen_size = 3
         self.old_position = (0,0)
         self.pen_up_at = (0,0)
 
 
     def _get_image(self):
         if not self in self.stage.pen_images:
             image = pygame.Surface((self.stage.width, self.stage.height), flags=pygame.SRCALPHA)
             self.stage.pen_images[self] = image
         return self.stage.pen_images[self]
 
     def _update_pen(self):
         if self.pen:
-            position = self._pg_pos()
-            if position == self.old_position:
+            if self.old_position == self._pos:
                 return
-            pygame.draw.line(self._get_image(), self.pen_color, self.old_position, position, width=self.pen_size)
-            self.old_position = position
+            pygame.draw.line(self._get_image(), self.pen_color, self.old_position, self._pos, width=int(self.pen_size))
+            self.old_position = list(self._pos)
         else:
             if self.pen_up_at != self.old_position:
-                pygame.draw.line(self._get_image(), self.pen_color, self.old_position, self.pen_up_at, width=self.pen_size)
+                pygame.draw.line(self._get_image(), self.pen_color, self.old_position, self.pen_up_at, width=int(self.pen_size))
                 self.pen_up_at = self.old_position
 
     def pen_clear(self):
         if self in self.stage.pen_images:
             del self.stage.pen_images[self]
 
 
     def pen_stamp(self):
         pass
 
 
     def pen_penDown(self):
         if not self.pen:
-            self.old_position = self._pg_pos()
+            self.old_position = list(self._pos)
         self.pen = True
 
 
     def pen_penUp(self):
-        self.pen_up_at = self._pg_pos()
+        self.pen_up_at = self._pos
         self.pen = False
 
 
     def pen_setPenColorToColor(self, color):
-        self.pen_color = color
+        self.pen_color = pygame.Color(color)
 
     pen_setPenColorToColor.translation = "pen_setcolor"
 
 
     def pen_changePenColorParamBy_color(self, value):
-        pass
+        hsva = list(self.pen_color.hsva)
+        hsva[0] = (hsva[0] + (value * 3.6)) % 360
+        self.pen_color.hsva = hsva
 
     pen_changePenColorParamBy_color.opcode="pen_changePenColorParamBy"
     pen_changePenColorParamBy_color.param="COLOR_PARAM"
     pen_changePenColorParamBy_color.value="color"
     pen_changePenColorParamBy_color.translation="pen_colormenu_color"
     pen_changePenColorParamBy_color.translation_hint="Needs to be distinguished from setPenColorToColor. This is only the hue value."
     pen_changePenColorParamBy_color.outer_translation="pen_changecolorparam"
     pen_changePenColorParamBy_color.position="[COLOR_PARAM]"
 
 
     def pen_changePenColorParamBy_saturation(self, value):
-        pass
+        hsva = list(self.pen_color.hsva)
+        hsva[1] = (hsva[1] + (value)) % 100
+        self.pen_color.hsva = hsva
 
     pen_changePenColorParamBy_saturation.opcode="pen_changePenColorParamBy"
     pen_changePenColorParamBy_saturation.param="COLOR_PARAM"
     pen_changePenColorParamBy_saturation.value="saturation"
     pen_changePenColorParamBy_saturation.translation="pen_colormenu_saturation"
     pen_changePenColorParamBy_saturation.outer_translation="pen_changecolorparam"
     pen_changePenColorParamBy_saturation.position="[COLOR_PARAM]"
     
 
     def pen_changePenColorParamBy_brightness(self, value):
-        pass
+        hsva = list(self.pen_color.hsva)
+        hsva[2] = (hsva[2] + (value)) % 100
+        self.pen_color.hsva = hsva
 
     pen_changePenColorParamBy_brightness.opcode="pen_changePenColorParamBy"
     pen_changePenColorParamBy_brightness.param="COLOR_PARAM"
     pen_changePenColorParamBy_brightness.value="brightness"
     pen_changePenColorParamBy_brightness.translation="pen_colormenu_brightness"
     pen_changePenColorParamBy_brightness.outer_translation="pen_changecolorparam"
     pen_changePenColorParamBy_brightness.position="[COLOR_PARAM]"
     
 
     def pen_changePenColorParamBy_transparency(self, value):
-        pass
+        hsva = list(self.pen_color.hsva)
+        hsva[3] = 100 - (((100 - hsva[3]) + (value)) % 100)
+        self.pen_color.hsva = hsva
 
     pen_changePenColorParamBy_transparency.opcode="pen_changePenColorParamBy"
     pen_changePenColorParamBy_transparency.param="COLOR_PARAM"
     pen_changePenColorParamBy_transparency.value="transparency"
     pen_changePenColorParamBy_transparency.translation="pen_colormenu_transparency"
     pen_changePenColorParamBy_transparency.outer_translation="pen_changecolorparam"
     pen_changePenColorParamBy_transparency.position="[COLOR_PARAM]"
 
 
     def pen_setPenColorParamTo_color(self, value):
-        pass
+        hsva = list(self.pen_color.hsva)
+        hsva[0] = (value * 3.6) % 360 
+        self.pen_color.hsva = hsva
 
     pen_setPenColorParamTo_color.opcode="pen_setPenColorParamTo"
     pen_setPenColorParamTo_color.param="COLOR_PARAM"
     pen_setPenColorParamTo_color.value="color"
     pen_setPenColorParamTo_color.translation="pen_colormenu_color"
     pen_setPenColorParamTo_color.translation_hint="Needs to be distinguished from setPenColorToColor. This is only the hue value."
     pen_setPenColorParamTo_color.outer_translation="pen_setcolorparam"
     pen_setPenColorParamTo_color.position="[COLOR_PARAM]"
 
 
     def pen_setPenColorParamTo_saturation(self, value):
-        pass
+        hsva = list(self.pen_color.hsva)
+        hsva[1] = value % 100
+        self.pen_color.hsva = hsva
 
     pen_setPenColorParamTo_saturation.opcode="pen_setPenColorParamTo"
     pen_setPenColorParamTo_saturation.param="COLOR_PARAM"
     pen_setPenColorParamTo_saturation.value="saturation"
     pen_setPenColorParamTo_saturation.translation="pen_colormenu_saturation"
     pen_setPenColorParamTo_saturation.outer_translation="pen_setcolorparam"
     pen_setPenColorParamTo_saturation.position="[COLOR_PARAM]"
     
 
     def pen_setPenColorParamTo_brightness(self, value):
-        pass
+        hsva = list(self.pen_color.hsva)
+        hsva[2] = value % 100
+        self.pen_color.hsva = hsva
 
     pen_setPenColorParamTo_brightness.opcode="pen_setPenColorParamTo"
     pen_setPenColorParamTo_brightness.param="COLOR_PARAM"
     pen_setPenColorParamTo_brightness.value="brightness"
     pen_setPenColorParamTo_brightness.translation="pen_colormenu_brightness"
     pen_setPenColorParamTo_brightness.outer_translation="pen_setcolorparam"
     pen_setPenColorParamTo_brightness.position="[COLOR_PARAM]"
     
 
     def pen_setPenColorParamTo_transparency(self, value):
-        pass
+        hsva = list(self.pen_color.hsva)
+        hsva[3] = 100 - (value % 100)
+        self.pen_color.hsva = hsva
 
     pen_setPenColorParamTo_transparency.opcode="pen_setPenColorParamTo"
     pen_setPenColorParamTo_transparency.param="COLOR_PARAM"
     pen_setPenColorParamTo_transparency.value="transparency"
     pen_setPenColorParamTo_transparency.translation="pen_colormenu_transparency"
     pen_setPenColorParamTo_transparency.outer_translation="pen_setcolorparam"
     pen_setPenColorParamTo_transparency.position="[COLOR_PARAM]"
```

### Comparing `pystage-0.0.9/src/pystage/core/_sound.py` & `pystage-0.1.0.dev0/src/pystage/core/_sound.py`

 * *Files identical despite different names*

### Comparing `pystage-0.0.9/src/pystage/core/assets.py` & `pystage-0.1.0.dev0/src/pystage/core/assets.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 import io
 import pygame
 import pkg_resources
 from svglib.svglib import svg2rlg
 from reportlab.graphics import renderPM
 import pystage
 
+_round = lambda v: pygame.Vector2(round(v.x), round(v.y))
+
 class CostumeManager():
 
     ALL_AROUND = 1
     LEFT_RIGHT = 2
     NO_ROTATION = 3
 
     def __init__(self, owner):
         self.owner = owner
         self.costumes = []
         self.current_costume = -1
-        self.offset = pygame.Vector2(0,0)
         self.rotation_style = CostumeManager.ALL_AROUND
 
     def add_costume(self, name, center_x=None, center_y=None, factor=1):
         if isinstance(name, str):
             costume = Costume(self, name, center_x, center_y, factor)
             self.costumes.append(costume)
             if self.current_costume==-1:
@@ -59,23 +60,26 @@
                 self.current_costume = i
                 self.update_sprite_image()
                 return
 
     def update_sprite_image(self):
         if isinstance(self.owner, pystage.core.CoreStage):
             return
-        image, origin = self.rotate_and_scale()
+        image, new_center = self.rotate_and_scale()
+        image.set_alpha((100-self.owner.ghost)/100*255)
         self.owner.image = image
+        self.owner.mask = pygame.mask.from_surface(image)
         self.owner.rect = image.get_rect()
-        self.owner.rect.topleft = origin
-        self.offset = self.owner._pg_pos() - origin
-
-
-    def get_offset(self):
-        return self.offset
+        self.owner.rect.topleft = _round(self.owner._pos) - new_center
+        new_center = _round(new_center)
+        if self.owner.stage.show_sprite_boundaries:
+            image.blit(self.owner.mask.to_surface(), (0,0))
+            pygame.draw.rect(image, "red", image.get_rect(), 1)
+            pygame.draw.line(image, "red", new_center - (10, 0), new_center + (10, 0), 1)
+            pygame.draw.line(image, "red", new_center - (0, 10), new_center + (0, 10), 1)
 
 
     def get_image(self):
         if self.current_costume == -1:
             return None
         return self.costumes[self.current_costume].image
 
@@ -89,54 +93,58 @@
     def get_center(self):
         if self.current_costume == -1:
             return 0, 0
         return pygame.Vector2(self.costumes[self.current_costume].center_x, self.costumes[self.current_costume].center_y)
 
 
     def rotate_and_scale(self):
+        # Based on:
         # https://stackoverflow.com/questions/54462645/how-to-rotate-an-image-around-its-center-while-its-scale-is-getting-largerin-py
-        pos = pygame.Vector2(self.owner._pg_pos())
-        originPos = self.get_center()
-        # Rotation
-        # Scratch is clockwise with 0 upwards
-        # pyGame is counterclockwise with 0 to the right
+        # Rotation settings
         flipped = False
         if self.rotation_style == CostumeManager.ALL_AROUND:
-            angle = 90-self.owner.direction
+            angle = self.owner._direction
         elif self.rotation_style == CostumeManager.NO_ROTATION:
             angle = 0
         else: # LEFT_RIGHT
             angle = 0
-            flipped = True if self.owner.direction % 360 > 180 else False 
-             
-        zoom = self.owner.size/100
-        image = self.get_image()
+            flipped = True if 90 < self.owner._direction % 360 < 270 else False 
+
+        # Zoom settings
+        scale = self.owner.size / 100
+
+        old_center = self.get_center()
+        old_center.y *= -1
+        center_rotated = old_center.rotate(angle)
 
-        # calcaulate the axis aligned bounding box of the rotated image
-        w, h       = image.get_size()
+        # Corner points of the current rect
+        w, h = self.get_image().get_size()
         box        = [pygame.math.Vector2(p) for p in [(0, 0), (w, 0), (w, -h), (0, -h)]]
         box_rotate = [p.rotate(angle) for p in box]
-        min_box    = (min(box_rotate, key=lambda p: p[0])[0], min(box_rotate, key=lambda p: p[1])[1])
-        max_box    = (max(box_rotate, key=lambda p: p[0])[0], max(box_rotate, key=lambda p: p[1])[1])
-
-        # calculate the translation of the pivot 
-        pivot        = pygame.math.Vector2(originPos[0], -originPos[1])
-        pivot_rotate = pivot.rotate(angle)
-        pivot_move   = pivot_rotate - pivot
-
-        # calculate the upper left origin of the rotated image
-        move   = (-originPos[0] + min_box[0] - pivot_move[0], -originPos[1] - max_box[1] + pivot_move[1])
-        origin = pygame.Vector2(pos[0] + zoom * move[0], pos[1] + zoom * move[1])
+        
+        # Axis aligned bounding box
+        minx = min(box_rotate, key=lambda p: p[0])[0]
+        maxx = max(box_rotate, key=lambda p: p[0])[0]
+        miny = min(box_rotate, key=lambda p: p[1])[1]
+        maxy = max(box_rotate, key=lambda p: p[1])[1]
+        topleft = pygame.Vector2(minx, maxy)
+
+        # new center
+        new_center = center_rotated - topleft
+        new_center.y *= -1
+        new_center *= scale
 
         # get a rotated image
-        rotozoom_image = pygame.transform.rotozoom(image, angle, zoom)
+        rotozoom_image = pygame.transform.rotozoom(self.get_image(), angle, scale)
         if flipped:
             rotozoom_image = pygame.transform.flip(rotozoom_image, True, False)
-      
-        return rotozoom_image, origin
+
+
+        return rotozoom_image, new_center
+
 
 class Costume():
     '''
     This class handles and manages costumes and backdrops.
     '''
     def __init__(self, sprite, name, center_x=None, center_y=None, factor=1):
         self.sprite = sprite
@@ -148,32 +156,33 @@
                 if os.path.exists(f"{folder}{name}{ext}"):
                     self.file = f"{folder}{name}{ext}"
                     break
             if self.file is not None:
                 break
         if self.file is None:
             self.file = pkg_resources.resource_filename("pystage", "images/zombie_idle.png")
-        if self.file.endswith(".svg"):
-            print(f"Converting SVG file: {self.file}")
-            print("\nWARNING: SVG conversion is for convenience only")
-            print("and might not work as expected. It is recommended")
-            print("to manually convert to bitmap graphics (png or jpg).\n")
-            # Deactivated for now because of Windows problems. See issue #10
-            # with stderr_redirector(io.BytesIO()):
-            rlg = svg2rlg(self.file)
-            pil = renderPM.drawToPIL(rlg)
-            self.image = pygame.image.frombuffer(pil.tobytes(), pil.size, pil.mode)
-        else:
-            self.image = pygame.image.load(self.file)
+        # if self.file.endswith(".svg"):
+        #     print(f"Converting SVG file: {self.file}")
+        #     print("\nWARNING: SVG conversion is for convenience only")
+        #     print("and might not work as expected. It is recommended")
+        #     print("to manually convert to bitmap graphics (png or jpg).\n")
+        #     # Deactivated for now because of Windows problems. See issue #10
+        #     # with stderr_redirector(io.BytesIO()):
+        #     rlg = svg2rlg(self.file)
+        #     pil = renderPM.drawToPIL(rlg)
+        #     self.image = pygame.image.frombuffer(pil.tobytes(), pil.size, pil.mode)
+        # else:
+        self.image = pygame.image.load(self.file)
         if factor!=1:
             self.image = pygame.transform.rotozoom(self.image, 0, 1.0/factor)
         self.image = self.image.subsurface(self.image.get_bounding_rect()) 
+        # The offset resulting from the image crop
         offset = pygame.Vector2(self.image.get_offset())
-        self.center_x = (self.image.get_parent().get_width() / 2) - offset.x if center_x is None else (center_x / factor) - offset.x 
-        self.center_y = (self.image.get_parent().get_height() / 2) - offset.y if center_y is None else (center_y / factor) - offset.y
+        self.center_x = (float(self.image.get_parent().get_width()) / 2) - offset.x if center_x is None else (float(center_x) / factor) - offset.x 
+        self.center_y = (float(self.image.get_parent().get_height()) / 2) - offset.y if center_y is None else (float(center_y) / factor) - offset.y
         print(f"New costume: {name} -> {self.file}")
 
 
     def __str__(self):
         return f"{self.name} ({self.center_x}, {self.center_y})"
```

### Comparing `pystage-0.0.9/src/pystage/core/code_block.py` & `pystage-0.1.0.dev0/src/pystage/core/code_block.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,81 +1,76 @@
-import inspect
 import ast
-import importlib
+import inspect
+
 from pystage.l10n.api import get_core_function_from_instance
 
 # Functions that need to be yielded for screen refresh
 yield_funcs = [
-        "control_wait",
-        "sound_playuntildone",
-        "motion_glidesecstoxy",
-        "motion_glideto_random",
-        "motion_glideto_sprite",
-        "motion_glideto_pointer",
-        ]
+    "control_wait",
+    "sound_playuntildone",
+    "motion_glidesecstoxy",
+    "motion_glideto_random",
+    "motion_glideto_sprite",
+    "motion_glideto_pointer",
+    "sensing_askandwait",
+]
+
 
 class CodeManager():
     def __init__(self, owner):
         # name: code_block
         self.code_blocks = {}
         # pygame.K_?: [name, ...]
         self.key_pressed_blocks = {}
         # message: [name, ...]
         self.broadcast_blocks = {}
         self.clicked_blocks = []
         # Name of the code block currently executed.
         # This way, state about the current execustion
         # can be stored safely where it belongs
-        self.current_block : CodeBlock = None
+        self.current_block: CodeBlock = None
         self.owner = owner
 
-
     def process_key_pressed(self, key):
         # key is a pygame constant, e.g. pygame.K_a
         # This hat block is special as it only fires again when the code block has ended. 
         # All other hat block methods stop the current execution and restart the block.
         if key in self.key_pressed_blocks:
             for name in self.key_pressed_blocks[key]:
                 self.code_blocks[name].start_if_not_running()
 
-
     def process_click(self):
         for block in self.clicked_blocks:
             block.start_or_restart()
 
-
     def process_broadcast(self, message):
         if message in self.broadcast_blocks:
             for name in self.broadcast_blocks[message]:
                 self.code_blocks[name].start_or_restart()
 
-
     def register_code_block(self, generator_function, name="", no_refresh=False):
         new_block = CodeBlock(self.owner, generator_function, name, no_refresh=no_refresh)
         self.code_blocks[new_block.name] = new_block
         print(f"New code block registered: {new_block.name}")
         return new_block
 
-
     def _update(self, dt):
         for name in self.code_blocks:
             self.current_block = self.code_blocks[name]
             self.code_blocks[name].update(dt)
 
 
-
 class CodeBlock():
     '''
     The CodeBlock encapsulates a generator and manages its state.
 
     
     '''
     last_id = -1
 
-
     def __init__(self, sprite_or_stage, generator_function, name="", no_refresh=False):
         '''
         Parameters
         ----------
         sprite_or_stage :
             The sprite or stage instance this code block is associated with
         generator_function : function
@@ -93,19 +88,24 @@
         Raises
         ------
         ValueError
             If the function does not get a single parameter (for the reference to 
             the sprite or stage) or if a generator function is supplied with no_refresh 
             set to True. 
         '''
-        if len(inspect.signature(generator_function).parameters)!=1:
-            raise ValueError(f"Your code block '{generator_function.__name__}' needs one parameter, usually called self.")
+        if len(inspect.signature(generator_function).parameters) == 0:
+            self.inject_instance = False
+        elif len(inspect.signature(generator_function).parameters) == 1:
+            self.inject_instance = True
+        else:
+            raise ValueError(
+                f"Your code block '{generator_function.__name__}' needs zero or one parameter. The parameter is usually called self.")
 
         self.sprite_or_stage = sprite_or_stage
-        if name!="" and name!=None:
+        if name != "" and name != None:
             name = f"-{name}"
         CodeBlock.last_id += 1
         # The name of a code block is unique with a global id.
         # A custom name may be provided to distinguish blocks
         # that use the same generator function.
         # This is not possible in Scratch (you only can copy blocks), 
         # but could be allowed here.
@@ -116,15 +116,16 @@
         self.generator_function = generator_function
         # The current state of a generator after it is started
         self.generator = None
         self.is_function = False
         self.no_refresh = no_refresh
         if inspect.isgeneratorfunction(generator_function):
             if no_refresh:
-                raise ValueError(f"Your code block '{generator_function.__name__}' is set to no refresh. In this case, yield must not be used.")
+                raise ValueError(
+                    f"Your code block '{generator_function.__name__}' is set to no refresh. In this case, yield must not be used.")
         else:
             if no_refresh:
                 # We support also plain functions, i.e. without yield
                 self.is_function = True
             else:
                 self.generator_function = self.add_yields(generator_function)
 
@@ -133,47 +134,59 @@
         self.add_to_wait_time = 0
         self.gliding = False
         self.gliding_seconds = 0
         self.gliding_start_position = (0, 0)
         self.gliding_end_position = (0, 0)
         # Flag indicating if the block is currently running
         self.running = False
+        # Ask mode (waiting for user input)
+        self.asking = False
+
+    def ask(self, question):
+        # Go into "ask" mode
+        self.asking = True
+        # Queue the question in the central input manager
+        self.sprite_or_stage.stage.input_manager.queue(question, self)
 
 
     def start_if_not_running(self):
         '''
         Start the code block. If the block is already started,
         this method does nothing.
         '''
         if self.running:
             return
         self.start_or_restart()
 
-
     def start_or_restart(self):
         '''
         (Re-)start the code block. If the block is already started,
         the current execution will not continue.
         '''
         self.running = True
         self.wait_time = 0
         if not self.is_function:
             target = self.sprite_or_stage
             if self.sprite_or_stage.facade:
                 target = self.sprite_or_stage.facade
-            self.generator = self.generator_function(target)
+            if self.inject_instance:
+                self.generator = self.generator_function(target)
+            else:
+                self.generator = self.generator_function()
         print(f"Start of {self.name} triggered.")
 
-
     def update(self, dt):
         '''
         Check if it is time for the next step and execute it.
         '''
         if not self.running:
             return
+        # Do nothing while waiting for an answer.
+        if self.asking:
+            return
         self.wait_time -= dt
         if self.wait_time < 0:
             if self.gliding:
                 self.x, self.y = self.gliding_end_position
                 self.gliding = False
             if self.is_function:
                 target = self.sprite_or_stage
@@ -192,76 +205,75 @@
                     if self.add_to_wait_time > 0:
                         self.wait_time += self.add_to_wait_time
                         self.add_to_wait_time = 0
                 except StopIteration:
                     print(f"CodeBlock {self.name} has finished.")
                     self.running = False
         elif self.gliding:
-            self.sprite_or_stage.x = self.gliding_end_position[0] - (self.gliding_end_position[0] - self.gliding_start_position[0]) * (self.wait_time / self.gliding_seconds)
-            self.sprite_or_stage.y = self.gliding_end_position[1] - (self.gliding_end_position[1] - self.gliding_start_position[1]) * (self.wait_time / self.gliding_seconds)
+            self.sprite_or_stage.motion_setx(
+                self.gliding_end_position[0] - (self.gliding_end_position[0] - self.gliding_start_position[0]) * (
+                            self.wait_time / self.gliding_seconds))
+            self.sprite_or_stage.motion_sety(
+                self.gliding_end_position[1] - (self.gliding_end_position[1] - self.gliding_start_position[1]) * (
+                            self.wait_time / self.gliding_seconds))
 
     def index_ast(self, func_ast):
         '''
         Helper function to (re-)generate for each node that is in
         a body or orelse field its parent, the field and its position 
         in the field.
 
         Parameters
         ----------
         func_ast : ast.AST
             The AST to be indexed.
         '''
-        
+
         for node in ast.walk(func_ast):
             for field in ["body", "orelse"]:
                 if hasattr(node, field):
                     for index, child in enumerate(getattr(node, field)):
                         child.parent = node
                         child.index = index
                         child.isin = field
 
-
     def add_yields(self, function):
         '''
         This function does the black magic and adds yields to the code so that
         the screen can update. This creates a generator function.
 
         Parameters
         ----------
         function : The function to be transformed to a generator function.
         '''
         func_ast = ast.parse(inspect.getsource(function))
-        
+
         # yield at the end of the function
         func_ast.body[0].body.append(ast.Expr(value=ast.Yield(value=ast.Constant(value=0))))
 
         self.index_ast(func_ast)
 
         for node in ast.walk(func_ast):
-            
+
             # yield at the end of for and while iterations
             if isinstance(node, ast.For):
                 node.body.append(ast.Expr(value=ast.Yield(value=ast.Constant(value=0))))
             if isinstance(node, ast.While):
                 node.body.append(ast.Expr(value=ast.Yield(value=ast.Constant(value=0))))
 
             # yield after certain calls defined in CodeBlock.yield_funcs
-            if isinstance(node, ast.Expr) and isinstance(node.value, ast.Call) and isinstance(node.value.func, ast.Attribute):
+            if isinstance(node, ast.Expr) and isinstance(node.value, ast.Call) and isinstance(node.value.func,
+                                                                                              ast.Attribute):
                 corefunc = get_core_function_from_instance(node.value.func.attr, self.sprite_or_stage.facade)
                 if corefunc in yield_funcs:
-                    getattr(node.parent, node.isin).insert(node.index + 1, ast.Expr(value=ast.Yield(value=ast.Constant(value=0))))
+                    getattr(node.parent, node.isin).insert(node.index + 1,
+                                                           ast.Expr(value=ast.Yield(value=ast.Constant(value=0))))
                     # We need to reindex so that further yields get the right position
                     self.index_ast(func_ast)
 
         ast.fix_missing_locations(func_ast)
         # print(ast.unparse(func_ast)) # outputs the transformed code
         namespace = {}
         namespace.update(function.__globals__)
         code = compile(func_ast, "<string>", mode="exec")
         exec(code, namespace)
-        return namespace[function.__name__] 
-
-
-
-
-
-
+        return namespace[function.__name__]
```

### Comparing `pystage-0.0.9/src/pystage/core/constants.py` & `pystage-0.1.0.dev0/src/pystage/core/constants.py`

 * *Files identical despite different names*

### Comparing `pystage-0.0.9/src/pystage/core/gui.py` & `pystage-0.1.0.dev0/src/pystage/core/gui.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,15 +103,15 @@
                     break
                 max_lw = max(max_lw, lw)
 
 
         # add a line consisting of those words
         line = ' '.join(line_words)
         lines.append(line)
-        print(lines, max_lw, max_lh)
+        # print(lines, max_lw, max_lh)
     return lines, max_lw, max_lh
 
 
 def render_lines(lines, font, color, lw, lh, lh_offset):
     # we'll render each line below the last, so we need to keep track of
     # the culmative height of the lines we've rendered so far
     surface = pygame.Surface((lw, (lh + lh_offset) * len(lines)), flags=pygame.SRCALPHA)
@@ -133,44 +133,44 @@
 
     def __init__(self, sprite, text: str, border: ResizableBorder):
         super().__init__()
         self.sprite = sprite
         self.text = text
         self.border = border
         self.flipped = False
-        self.sprite_x = self.sprite.x
-        self.sprite_y = self.sprite.y
-        self.x_offset = -0.1 # percent of sprite width based on lower right corner
-        self.y_offset = -0.5 # percent of sprite height based on lower right corner
+        self.sprite_x = self.sprite.motion_xposition()
+        self.sprite_y = self.sprite.motion_yposition()
+        self.x_offset = -0.2 # percent of sprite width based on lower right corner
+        self.y_offset = -0.2 # percent of sprite height based on lower right corner
         lh_offset = -1
         lines, lw, lh = wrap_text(self.text[:360], regular_font_14, 170)
         self.text_surface = render_lines(lines, regular_font_14, color1, lw+10, lh, lh_offset)
         self.image_normal = self.border.render(self.text_surface.get_width() + 26, self.text_surface.get_height() + 40)
         self.image_flipped = pygame.transform.flip(self.image_normal, True, False)
         self.image_normal.blit(self.text_surface, (13, 13))
         self.image_flipped.blit(self.text_surface, (13, 13))
         self.image = self.image_normal
         self.rect = self.image.get_rect()
         self.update(force=True)
 
 
     def update(self, force=False):
-        if not force and self.sprite.x == self.sprite_x and self.sprite.y == self.sprite_y:
+        if not force and self.sprite.motion_xposition() == self.sprite_x and self.sprite.motion_yposition() == self.sprite_y:
             return
-        y = max(0, self.sprite._pg_pos()[1] - self.image_normal.get_height() + self.sprite.costume_manager.get_image().get_height() * self.y_offset)
+        y = max(0, self.sprite.rect.top - self.image_normal.get_height() - self.sprite.costume_manager.get_image().get_height() * self.y_offset)
         if not self.flipped:
-            x = self.sprite._pg_pos()[0] - self.image_normal.get_width() + self.sprite.costume_manager.get_image().get_width() * self.x_offset
+            x = self.sprite.rect.left - self.image_normal.get_width() - self.sprite.costume_manager.get_image().get_width() * self.x_offset
             if x < 0:
                 self.flipped = True
-                x = self.sprite._pg_pos()[0] - self.sprite.costume_manager.get_image().get_width() * self.x_offset
+                x = self.sprite.rect.right + self.sprite.costume_manager.get_image().get_width() * self.x_offset
         else:
-            x = self.sprite._pg_pos()[0] - self.sprite.costume_manager.get_image().get_width() * self.x_offset
+            x = self.sprite.rect.right + self.sprite.costume_manager.get_image().get_width() * self.x_offset
             if x + self.image_normal.get_width() > self.sprite.stage.width:
                 self.flipped = False
-                x = self.sprite._pg_pos()[0] - self.image_normal.get_width() + self.sprite.costume_manager.get_image().get_width() * self.x_offset
+                x = self.sprite.rect.left - self.image_normal.get_width() - self.sprite.costume_manager.get_image().get_width() * self.x_offset
         self.image = self.image_flipped if self.flipped else self.image_normal
         self.rect.x = x
         self.rect.y = y
 
 
 
 
@@ -178,16 +178,21 @@
 
     def __init__(self, sprite):
         self.sprite = sprite
         self.flipped = False
         self.bubble = None
 
     def say(self, text: str, border=Bubble.SAY):
-        print(text)
+        # print(text)
+        if isinstance(text, (int, float)):
+            text = str(round(text, 2) if text % 1 > 0 else int(text))
         if self.bubble:
             self.bubble.kill()
             self.bubble = None
         if text is not None and text.strip() != "":
             self.bubble = Bubble(self.sprite, text, border)
             self.sprite.stage.bubbles.add(self.bubble)
+            
+    def think(self, text: str):
+        self.say(text, Bubble.THINK)
```

### Comparing `pystage-0.0.9/src/pystage/core/sprite.py` & `pystage-0.1.0.dev0/src/pystage/core/sprite.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,31 +19,29 @@
     def __init__(self, stage, costume="default"):
         self.stage = stage
         # Above attributes need to be set first so that mixins can access them properly
         super().__init__()
         default_file = pkg_resources.resource_filename("pystage", "images/zombie_idle.png")
         self.image = pygame.image.load(default_file)
         self.rect = self.image.get_rect()
+        self.mask = pygame.mask.from_surface(self.image)
         if costume:
             self.pystage_addcostume(costume)
+            self.name = "Sprite" if costume=="default" else costume 
+        else:
+            self.name = "Sprite"
         # The facade is the translated API
         self.facade = None
 
 
+    def pystage_setname(self, name):
+        self.name = name
+
+
     def update(self, dt):
         self.code_manager._update(dt)
         self.costume_manager.update_sprite_image()
         self._update_pen()
 
 
-    def _pg_pos(self):
-        return pygame.Vector2(self.x + self.stage.center_x, 
-                -self.y + self.stage.center_y)
-
-
-    def _update_pos_from_rect(self):
-        pos = self.rect.topleft + self.costume_manager.get_offset()
-        self.x = pos.x - self.stage.center_x
-        self.y = -pos.y + self.stage.center_y
-
     def __str__(self):
-        return self.costume_manager.get_costume().name
+        return self.name
```

### Comparing `pystage-0.0.9/src/pystage/de/sprite.py` & `pystage-0.1.0.dev0/src/pystage/de/sprite.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,35 +39,34 @@
 
         Returns
         -------
 
         """
         return self._core.control_delete_this_clone()
                 
-    def wenn_ich_als_klon_entstehe(self, key, generator_function, name='', no_refresh=False):
+    def wenn_ich_als_klon_entstehe(self, generator_function, name='', no_refresh=False):
         """Wenn ich als Klon entstehe
 
         Translation string: Wenn ich als Klon entstehe
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
         Parameters
         ----------
-        key : FILL
         generator_function : FILL
         name : FILL
         no_refresh : FILL
         
 
         Returns
         -------
 
         """
-        return self._core.control_start_as_clone(key, generator_function, name, no_refresh)
+        return self._core.control_start_as_clone(generator_function, name, no_refresh)
                 
     def stoppe_alles(self):
         """stoppe alles
 
         Translation string: stoppe alles
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
@@ -1930,14 +1929,71 @@
 
         Returns
         -------
 
         """
         return self._core.pystage_setmonitorposition(name, x, y)
                 
+    def pystage_setmonitorstyle_large(self, name):
+        """
+
+        Translation string: 
+        Engl. Translation for your reference: ...
+        Engl. Documentation when available...
+
+        
+        Parameters
+        ----------
+        name : FILL
+        
+
+        Returns
+        -------
+
+        """
+        return self._core.pystage_setmonitorstyle_large(name)
+                
+    def pystage_setmonitorstyle_normal(self, name):
+        """
+
+        Translation string: 
+        Engl. Translation for your reference: ...
+        Engl. Documentation when available...
+
+        
+        Parameters
+        ----------
+        name : FILL
+        
+
+        Returns
+        -------
+
+        """
+        return self._core.pystage_setmonitorstyle_normal(name)
+                
+    def pystage_setmonitorstyle_slider(self, name):
+        """
+
+        Translation string: 
+        Engl. Translation for your reference: ...
+        Engl. Documentation when available...
+
+        
+        Parameters
+        ----------
+        name : FILL
+        
+
+        Returns
+        -------
+
+        """
+        return self._core.pystage_setmonitorstyle_slider(name)
+                
     def antwort(self):
         """Antwort
 
         Translation string: Antwort
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -2749,7 +2805,25 @@
 
         Returns
         -------
 
         """
         return self._core.sound_volume()
                 
+    def setze_name(self, name):
+        """
+
+        Translation string: 
+        Engl. Translation for your reference: ...
+        Engl. Documentation when available...
+
+        
+        Parameters
+        ----------
+        name : FILL
+
+
+        Returns
+        -------
+
+        """
+        return self._core.pystage_setname(name)
```

### Comparing `pystage-0.0.9/src/pystage/de/stage.py` & `pystage-0.1.0.dev0/src/pystage/de/stage.py`

 * *Files 1% similar despite different names*

```diff
@@ -946,14 +946,71 @@
 
         Returns
         -------
 
         """
         return self._core.pystage_setmonitorposition(name, x, y)
                 
+    def pystage_setmonitorstyle_large(self, name):
+        """
+
+        Translation string: 
+        Engl. Translation for your reference: ...
+        Engl. Documentation when available...
+
+        
+        Parameters
+        ----------
+        name : FILL
+        
+
+        Returns
+        -------
+
+        """
+        return self._core.pystage_setmonitorstyle_large(name)
+                
+    def pystage_setmonitorstyle_normal(self, name):
+        """
+
+        Translation string: 
+        Engl. Translation for your reference: ...
+        Engl. Documentation when available...
+
+        
+        Parameters
+        ----------
+        name : FILL
+        
+
+        Returns
+        -------
+
+        """
+        return self._core.pystage_setmonitorstyle_normal(name)
+                
+    def pystage_setmonitorstyle_slider(self, name):
+        """
+
+        Translation string: 
+        Engl. Translation for your reference: ...
+        Engl. Documentation when available...
+
+        
+        Parameters
+        ----------
+        name : FILL
+        
+
+        Returns
+        -------
+
+        """
+        return self._core.pystage_setmonitorstyle_slider(name)
+                
     def antwort(self):
         """Antwort
 
         Translation string: Antwort
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
```

### Comparing `pystage-0.0.9/src/pystage/en/sprite.py` & `pystage-0.1.0.dev0/src/pystage/en/sprite.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-
 from pystage.core.sprite import CoreSprite
 
 
-class Sprite():
+class Sprite:
     def __init__(self, core_sprite):
-        self._core : CoreSprite = core_sprite
+        self._core: CoreSprite = core_sprite
         self._core.facade = self
 
-
-            
-    def create_clone_of(self, sprite='_myself_'):
+    def create_clone_of(self, sprite="_myself_"):
         """create clone of %1
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
         Parameters
@@ -21,93 +18,96 @@
         sprite : FILL
         
 
         Returns
         -------
 
         """
-        return self._core.control_create_clone_of(sprite='_my_')
-                
+        return self._core.control_create_clone_of(sprite="_my_")
+
     def delete_this_clone(self):
         """delete this clone
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.control_delete_this_clone()
-                
-    def when_i_start_as_a_clone(self, key, generator_function, name='', no_refresh=False):
+
+    def when_i_start_as_a_clone(
+        self, generator_function, name="", no_refresh=False
+    ):
         """when I start as a clone
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
         Parameters
         ----------
-        key : FILL
         generator_function : FILL
         name : FILL
         no_refresh : FILL
         
 
         Returns
         -------
 
         """
-        return self._core.control_start_as_clone(key, generator_function, name='', no_refresh=False)
-                
+        return self._core.control_start_as_clone(
+            generator_function, name="", no_refresh=False
+        )
+
     def stop_all(self):
         """stop all
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.control_stop_all()
-                
+
     def stop_other_scripts_in_sprite(self):
         """stop other scripts in sprite
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.control_stop_other()
-                
+
     def stop_this_script(self):
         """stop this script
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.control_stop_this()
-                
+
     def wait(self, secs):
         """wait %1 seconds
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -117,15 +117,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.control_wait(secs)
-                
+
     def change_variable_by(self, name, value):
         """change %1 by %2
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -136,15 +136,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.data_changevariableby(name, value)
-                
+
     def hide_variable(self, name):
         """hide variable %1
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -154,15 +154,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.data_hidevariable(name)
-                
+
     def set_variable(self, name, value):
         """set %1 to %2
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -173,15 +173,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.data_setvariableto(name, value)
-                
+
     def show_variable(self, name):
         """show variable %1
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -191,15 +191,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.data_showvariable(name)
-                
+
     def get_variable(self, name):
         """
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -209,15 +209,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.data_variable(name)
-                
+
     def broadcast(self, message):
         """broadcast %1
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -227,15 +227,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.event_broadcast(message)
-                
+
     def broadcast_and_wait(self, message):
         """broadcast %1 and wait
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -245,16 +245,18 @@
         
 
         Returns
         -------
 
         """
         return self._core.event_broadcastandwait(message)
-                
-    def when_backdrop_switches_to(self, backdrop, generator_function, name='', no_refresh=False):
+
+    def when_backdrop_switches_to(
+        self, backdrop, generator_function, name="", no_refresh=False
+    ):
         """when backdrop switches to %1
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
         Parameters
@@ -265,17 +267,21 @@
         no_refresh : FILL
         
 
         Returns
         -------
 
         """
-        return self._core.event_whenbackdropswitchesto(backdrop, generator_function, name='', no_refresh=False)
-                
-    def when_i_receive_message(self, message, generator_function, name='', no_refresh=False):
+        return self._core.event_whenbackdropswitchesto(
+            backdrop, generator_function, name="", no_refresh=False
+        )
+
+    def when_i_receive_message(
+        self, message, generator_function, name="", no_refresh=False
+    ):
         """when I receive %1
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
         Parameters
@@ -286,17 +292,19 @@
         no_refresh : FILL
         
 
         Returns
         -------
 
         """
-        return self._core.event_whenbroadcastreceived(message, generator_function, name='', no_refresh=False)
-                
-    def when_program_starts(self, generator_function, name='', no_refresh=False):
+        return self._core.event_whenbroadcastreceived(
+            message, generator_function, name="", no_refresh=False
+        )
+
+    def when_program_starts(self, generator_function, name="", no_refresh=False):
         """when <greenflag> clicked
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
         Parameters
@@ -306,17 +314,21 @@
         no_refresh : FILL
         
 
         Returns
         -------
 
         """
-        return self._core.event_whenflagclicked(generator_function, name='', no_refresh=False)
-                
-    def when_loudness_greater_than(self, value, generator_function, name='', no_refresh=False):
+        return self._core.event_whenflagclicked(
+            generator_function, name="", no_refresh=False
+        )
+
+    def when_loudness_greater_than(
+        self, value, generator_function, name="", no_refresh=False
+    ):
         """when loudness <greater> %2
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
         Parameters
@@ -327,17 +339,21 @@
         no_refresh : FILL
         
 
         Returns
         -------
 
         """
-        return self._core.event_whengreaterthan_loudness(value, generator_function, name='', no_refresh=False)
-                
-    def when_timer_greater_than(self, value, generator_function, name='', no_refresh=False):
+        return self._core.event_whengreaterthan_loudness(
+            value, generator_function, name="", no_refresh=False
+        )
+
+    def when_timer_greater_than(
+        self, value, generator_function, name="", no_refresh=False
+    ):
         """when timer <greater> %2
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
         Parameters
@@ -348,17 +364,19 @@
         no_refresh : FILL
         
 
         Returns
         -------
 
         """
-        return self._core.event_whengreaterthan_timer(value, generator_function, name='', no_refresh=False)
-                
-    def when_key_pressed(self, key, generator_function, name='', no_refresh=False):
+        return self._core.event_whengreaterthan_timer(
+            value, generator_function, name="", no_refresh=False
+        )
+
+    def when_key_pressed(self, key, generator_function, name="", no_refresh=False):
         """when %1 key pressed
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
         Parameters
@@ -369,17 +387,19 @@
         no_refresh : FILL
         
 
         Returns
         -------
 
         """
-        return self._core.event_whenkeypressed(key, generator_function, name='', no_refresh=False)
-                
-    def when_this_sprite_clicked(self, generator_function, name='', no_refresh=False):
+        return self._core.event_whenkeypressed(
+            key, generator_function, name="", no_refresh=False
+        )
+
+    def when_this_sprite_clicked(self, generator_function, name="", no_refresh=False):
         """when this sprite clicked
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
         Parameters
@@ -389,44 +409,46 @@
         no_refresh : FILL
         
 
         Returns
         -------
 
         """
-        return self._core.event_whenthisspriteclicked(generator_function, name='', no_refresh=False)
-                
+        return self._core.event_whenthisspriteclicked(
+            generator_function, name="", no_refresh=False
+        )
+
     def backdrop_name(self):
         """backdrop name
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.looks_backdropnumbername_name()
-                
+
     def backdrop_number(self):
         """backdrop number
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.looks_backdropnumbername_number()
-                
+
     def change_brightness_effect_by(self, value):
         """change brightness effect by %2
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -436,15 +458,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.looks_changeeffectby_brightness(value)
-                
+
     def change_color_effect_by(self, value):
         """change color effect by %2
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -454,15 +476,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.looks_changeeffectby_color(value)
-                
+
     def change_fisheye_effect_by(self, value):
         """change fisheye effect by %2
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -472,15 +494,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.looks_changeeffectby_fisheye(value)
-                
+
     def change_ghost_effect_by(self, value):
         """change ghost effect by %2
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -490,15 +512,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.looks_changeeffectby_ghost(value)
-                
+
     def change_mosaic_effect_by(self, value):
         """change mosaic effect by %2
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -508,15 +530,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.looks_changeeffectby_mosaic(value)
-                
+
     def change_pixelate_effect_by(self, value):
         """change pixelate effect by %2
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -526,15 +548,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.looks_changeeffectby_pixelate(value)
-                
+
     def change_whirl_effect_by(self, value):
         """change whirl effect by %2
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -544,15 +566,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.looks_changeeffectby_whirl(value)
-                
+
     def change_size_by(self, percent):
         """change size by %1
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -562,57 +584,57 @@
         
 
         Returns
         -------
 
         """
         return self._core.looks_changesizeby(percent)
-                
+
     def clear_graphic_effects(self):
         """clear graphic effects
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.looks_cleargraphiceffects()
-                
+
     def costume_name(self):
         """costume name
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.looks_costumenumbername_name()
-                
+
     def costume_number(self):
         """costume number
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.looks_costumenumbername_number()
-                
+
     def go_backward(self, value):
         """go backward %2 layers
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -622,15 +644,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.looks_goforwardbackwardlayers_backward(value)
-                
+
     def go_forward(self, value):
         """go forward %2 layers
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -640,85 +662,85 @@
         
 
         Returns
         -------
 
         """
         return self._core.looks_goforwardbackwardlayers_forward(value)
-                
+
     def go_to_back_layer(self):
         """go to back layer
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.looks_gotofrontback_back()
-                
+
     def go_to_front_layer(self):
         """go to front layer
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.looks_gotofrontback_front()
-                
+
     def hide(self):
         """hide
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.looks_hide()
-                
+
     def next_backdrop(self):
         """next backdrop
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.looks_nextbackdrop()
-                
+
     def next_costume(self):
         """next costume
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.looks_nextcostume()
-                
+
     def say(self, text):
         """say %1
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -728,15 +750,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.looks_say(text)
-                
+
     def say_for_seconds(self, text, secs):
         """say %1 for %2 seconds
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -747,15 +769,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.looks_sayforsecs(text, secs)
-                
+
     def set_brightness_effect_to(self, value):
         """set brightness effect to %2
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -765,15 +787,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.looks_seteffectto_brightness(value)
-                
+
     def set_color_effect_to(self, value):
         """set color effect to %2
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -783,15 +805,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.looks_seteffectto_color(value)
-                
+
     def set_fisheye_effect_to(self, value):
         """set fisheye effect to %2
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -801,15 +823,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.looks_seteffectto_fisheye(value)
-                
+
     def set_ghost_effect_to(self, value):
         """set ghost effect to %2
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -819,15 +841,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.looks_seteffectto_ghost(value)
-                
+
     def set_mosaic_effect_to(self, value):
         """set mosaic effect to %2
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -837,15 +859,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.looks_seteffectto_mosaic(value)
-                
+
     def set_pixelate_effect_to(self, value):
         """set pixelate effect to %2
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -855,15 +877,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.looks_seteffectto_pixelate(value)
-                
+
     def set_whirl_effect_to(self, value):
         """set whirl effect to %2
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -873,15 +895,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.looks_seteffectto_whirl(value)
-                
+
     def set_size_to(self, percent):
         """set size to %1 %
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -891,43 +913,43 @@
         
 
         Returns
         -------
 
         """
         return self._core.looks_setsizeto(percent)
-                
+
     def show(self):
         """show
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.looks_show()
-                
+
     def size(self):
         """size
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.looks_size()
-                
+
     def switch_backdrop_to(self, backdrop):
         """switch backdrop to %1
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -937,15 +959,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.looks_switchbackdropto(backdrop)
-                
+
     def switch_costume_to(self, costume):
         """switch costume to %1
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -955,15 +977,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.looks_switchcostumeto(costume)
-                
+
     def think(self, text):
         """think %1
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -973,15 +995,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.looks_think(text)
-                
+
     def think_for_seconds(self, text, secs):
         """think %1 for %2 seconds
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -992,15 +1014,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.looks_thinkforsecs(text, secs)
-                
+
     def change_x_by(self, value):
         """change x by %1
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -1010,15 +1032,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.motion_changexby(value)
-                
+
     def change_y_by(self, value):
         """change y by %1
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -1028,29 +1050,29 @@
         
 
         Returns
         -------
 
         """
         return self._core.motion_changeyby(value)
-                
+
     def direction(self):
         """direction
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.motion_direction()
-                
+
     def glide_to_x_y(self, secs, x, y):
         """glide %1 secs to x: %2 y: %3
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -1062,15 +1084,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.motion_glidesecstoxy(secs, x, y)
-                
+
     def glide_to_mouse_pointer(self, secs):
         """glide %1 secs to mouse-pointer
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -1080,15 +1102,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.motion_glideto_pointer(secs)
-                
+
     def glide_to_random_position(self, secs):
         """glide %1 secs to random position
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -1098,15 +1120,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.motion_glideto_random(secs)
-                
+
     def glide_to_sprite(self, secs, sprite):
         """glide %1 secs to %2
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -1117,43 +1139,43 @@
         
 
         Returns
         -------
 
         """
         return self._core.motion_glideto_sprite(secs, sprite)
-                
+
     def go_to_mouse_pointer(self):
         """go to mouse-pointer
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.motion_goto_pointer()
-                
+
     def go_to_random_position(self):
         """go to random position
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.motion_goto_random()
-                
+
     def go_to_sprite(self, sprite):
         """go to %1
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -1163,15 +1185,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.motion_goto_sprite(sprite)
-                
+
     def go_to_x_y(self, x, y):
         """go to x: %1 y: %2
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -1182,29 +1204,29 @@
         
 
         Returns
         -------
 
         """
         return self._core.motion_gotoxy(x, y)
-                
+
     def if_on_edge_bounce(self):
         """if on edge, bounce
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.motion_ifonedgebounce()
-                
+
     def move(self, steps):
         """move %1 steps
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -1214,15 +1236,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.motion_movesteps(steps)
-                
+
     def point_in_direction(self, direction):
         """point in direction %1
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -1232,29 +1254,29 @@
         
 
         Returns
         -------
 
         """
         return self._core.motion_pointindirection(direction)
-                
+
     def point_towards_mouse_pointer(self):
         """point towards mouse-pointer
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.motion_pointtowards_pointer()
-                
+
     def point_towards_sprite(self, sprite):
         """point towards %1
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -1264,47 +1286,44 @@
         
 
         Returns
         -------
 
         """
         return self._core.motion_pointtowards_sprite(sprite)
-                
 
     def set_rotation_style_none(self):
         """set rotation style %1
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         """
         return self._core.motion_setrotationstyle_dontrotate()
-                
+
     def set_rotation_style_left_right(self):
         """set rotation style %1
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
 
         """
         return self._core.motion_setrotationstyle_leftright()
 
-
     def set_rotation_style_around(self):
         """set rotation style %1
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
         """
         return self._core.motion_setrotationstyle_allaround()
 
-
     def set_x(self, value):
         """set x to %1
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -1314,15 +1333,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.motion_setx(value)
-                
+
     def set_y(self, value):
         """set y to %1
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -1332,15 +1351,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.motion_sety(value)
-                
+
     def turn_left(self, deg):
         """turn left %2 degrees
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -1350,15 +1369,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.motion_turnleft(deg)
-                
+
     def turn_right(self, deg):
         """turn right %2 degrees
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -1368,43 +1387,43 @@
         
 
         Returns
         -------
 
         """
         return self._core.motion_turnright(deg)
-                
+
     def x_position(self):
         """x position
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.motion_xposition()
-                
+
     def y_position(self):
         """y position
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.motion_yposition()
-                
+
     def calculate(self, operator, number):
         """%1 of %2
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -1415,15 +1434,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.operator_mathop(operator, number)
-                
+
     def pick_random(self, start, end):
         """pick random %1 to %2
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -1434,15 +1453,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.operator_random(start, end)
-                
+
     def change_pen_brightness_by(self, value):
         """change pen brightness by [VALUE]
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -1452,15 +1471,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.pen_changePenColorParamBy_brightness(value)
-                
+
     def change_pen_hue_by(self, value):
         """change pen color by [VALUE]
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -1470,15 +1489,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.pen_changePenColorParamBy_color(value)
-                
+
     def change_pen_saturation_by(self, value):
         """change pen saturation by [VALUE]
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -1488,15 +1507,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.pen_changePenColorParamBy_saturation(value)
-                
+
     def change_pen_transparency_by(self, value):
         """change pen transparency by [VALUE]
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -1506,15 +1525,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.pen_changePenColorParamBy_transparency(value)
-                
+
     def change_pen_size_by(self, value):
         """change pen size by [SIZE]
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -1524,57 +1543,57 @@
         
 
         Returns
         -------
 
         """
         return self._core.pen_changePenSizeBy(value)
-                
+
     def erase_all(self):
         """erase all
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.pen_clear()
-                
+
     def pen_down(self):
         """pen down
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.pen_penDown()
-                
+
     def pen_up(self):
         """pen up
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.pen_penUp()
-                
+
     def set_pen_brightness_to(self, value):
         """set pen brightness to [VALUE]
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -1584,15 +1603,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.pen_setPenColorParamTo_brightness(value)
-                
+
     def set_pen_hue_to(self, value):
         """set pen color to [VALUE]
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -1602,15 +1621,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.pen_setPenColorParamTo_color(value)
-                
+
     def set_pen_saturation_to(self, value):
         """set pen saturation to [VALUE]
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -1620,15 +1639,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.pen_setPenColorParamTo_saturation(value)
-                
+
     def set_pen_transparency_to(self, value):
         """set pen transparency to [VALUE]
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -1638,15 +1657,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.pen_setPenColorParamTo_transparency(value)
-                
+
     def set_pen_color(self, color):
         """set pen color to [COLOR]
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -1656,15 +1675,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.pen_setPenColorToColor(color)
-                
+
     def set_pen_size_to(self, value):
         """set pen size to [SIZE]
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -1674,29 +1693,29 @@
         
 
         Returns
         -------
 
         """
         return self._core.pen_setPenSizeTo(value)
-                
+
     def stamp(self):
         """stamp
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.pen_stamp()
-                
+
     def add_costume(self, name, center_x=None, center_y=None, factor=1):
         """
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -1709,15 +1728,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.pystage_addcostume(name, center_x, center_y, factor)
-                
+
     def add_sound(self, name):
         """
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -1727,15 +1746,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.pystage_addsound(name)
-                
+
     def insert_costume(self, index, name, center_x=None, center_y=None, factor=1):
         """
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -1748,15 +1767,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.pystage_insertcostume(index, name, center_x, center_y, factor)
-                
+
     def create_variable(self, name, all_sprites=True):
         """
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -1767,15 +1786,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.pystage_makevariable(name, all_sprites=True)
-                
+
     def replace_costume(self, index, name, center_x=None, center_y=None, factor=1):
         """
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -1787,16 +1806,18 @@
         center_y : FILL
         
 
         Returns
         -------
 
         """
-        return self._core.pystage_replacecostume(index, name, center_x, center_y, factor)
-                
+        return self._core.pystage_replacecostume(
+            index, name, center_x, center_y, factor
+        )
+
     def set_monitor_position(self, name, x, y):
         """
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -1808,29 +1829,86 @@
         
 
         Returns
         -------
 
         """
         return self._core.pystage_setmonitorposition(name, x, y)
-                
+
+    def pystage_setmonitorstyle_large(self, name):
+        """
+
+        Translation string: 
+        Engl. Translation for your reference: ...
+        Engl. Documentation when available...
+
+        
+        Parameters
+        ----------
+        name : FILL
+        
+
+        Returns
+        -------
+
+        """
+        return self._core.pystage_setmonitorstyle_large(name)
+
+    def pystage_setmonitorstyle_normal(self, name):
+        """
+
+        Translation string: 
+        Engl. Translation for your reference: ...
+        Engl. Documentation when available...
+
+        
+        Parameters
+        ----------
+        name : FILL
+        
+
+        Returns
+        -------
+
+        """
+        return self._core.pystage_setmonitorstyle_normal(name)
+
+    def pystage_setmonitorstyle_slider(self, name):
+        """
+
+        Translation string: 
+        Engl. Translation for your reference: ...
+        Engl. Documentation when available...
+
+        
+        Parameters
+        ----------
+        name : FILL
+        
+
+        Returns
+        -------
+
+        """
+        return self._core.pystage_setmonitorstyle_slider(name)
+
     def answer(self):
         """answer
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sensing_answer()
-                
+
     def ask_and_wait(self, question):
         """ask %1 and wait
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -1840,15 +1918,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.sensing_askandwait(question)
-                
+
     def color_is_touching(self, sprite_color, color):
         """color %1 is touching %2?
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -1859,155 +1937,159 @@
         
 
         Returns
         -------
 
         """
         return self._core.sensing_coloristouchingcolor(sprite_color, color)
-                
+
     def current_date(self):
         """current date
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sensing_current_date()
-                
+
     def current_day_of_week(self):
         """current day of week
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sensing_current_dayofweek()
-                
+
     def current_hour(self):
         """current hour
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sensing_current_hour()
-                
+
     def current_minute(self):
         """current minute
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sensing_current_minute()
-                
+
     def current_month(self):
         """current month
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sensing_current_month()
-                
+
     def current_second(self):
         """current second
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sensing_current_second()
-                
+
     def current_year(self):
         """current year
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sensing_current_year()
-                
+
     def days_since(self):
         """days since 2000
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sensing_dayssince2000()
-                
+
     def distance_to_mouse_pointer(self):
         """distance to mouse-pointer
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sensing_distanceto_pointer()
-                
+
     def distance_to_sprite(self, sprite):
         """distance to %1
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
+        Parameters
+        ----------
+        sprite : FILL
+        
 
         Returns
         -------
 
         """
         return self._core.sensing_distanceto_sprite(sprite)
-                
+
     def key_pressed(self, key):
         """key %1 pressed?
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -2017,72 +2099,72 @@
         
 
         Returns
         -------
 
         """
         return self._core.sensing_keypressed(key)
-                
+
     def loudness(self):
         """loudness
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sensing_loudness()
-                
+
     def mouse_down(self):
         """mouse down?
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sensing_mousedown()
-                
+
     def mouse_x(self):
         """mouse x
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sensing_mousex()
-                
+
     def mouse_y(self):
         """mouse y
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sensing_mousey()
-                
-    def backdrop_name_of(self, stage='_stage_'):
+
+    def backdrop_name_of(self, stage="_stage_"):
         """backdrop name of %2
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
         Parameters
@@ -2090,17 +2172,17 @@
         stage : FILL
         
 
         Returns
         -------
 
         """
-        return self._core.sensing_of_backdropname(stage='_stage_')
-                
-    def backdrop_of(self, stage='_stage_'):
+        return self._core.sensing_of_backdropname(stage="_stage_")
+
+    def backdrop_of(self, stage="_stage_"):
         """backdrop # of %2
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
         Parameters
@@ -2108,16 +2190,16 @@
         stage : FILL
         
 
         Returns
         -------
 
         """
-        return self._core.sensing_of_backdropnumber(stage='_stage_')
-                
+        return self._core.sensing_of_backdropnumber(stage="_stage_")
+
     def costume_name_of(self, sprite):
         """costume name of %2
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -2127,15 +2209,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.sensing_of_costumename(sprite)
-                
+
     def costume_of(self, sprite):
         """costume # of %2
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -2145,15 +2227,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.sensing_of_costumenumber(sprite)
-                
+
     def direction_of(self, sprite):
         """direction of %2
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -2163,15 +2245,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.sensing_of_direction(sprite)
-                
+
     def size_of(self, sprite):
         """size of %2
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -2181,16 +2263,16 @@
         
 
         Returns
         -------
 
         """
         return self._core.sensing_of_size(sprite)
-                
-    def get_variable_of(self, variable, sprite='_stage_'):
+
+    def get_variable_of(self, variable, sprite="_stage_"):
         """%1 of %2
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
         Parameters
@@ -2199,17 +2281,17 @@
         sprite : FILL
         
 
         Returns
         -------
 
         """
-        return self._core.sensing_of_variable(variable, sprite='_stage_')
-                
-    def volume_of(self, sprite='_stage_'):
+        return self._core.sensing_of_variable(variable, sprite="_stage_")
+
+    def volume_of(self, sprite="_stage_"):
         """volume of %2
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
         Parameters
@@ -2217,16 +2299,16 @@
         sprite : FILL
         
 
         Returns
         -------
 
         """
-        return self._core.sensing_of_volume(sprite='_stage_')
-                
+        return self._core.sensing_of_volume(sprite="_stage_")
+
     def x_position_of(self, sprite):
         """x position of %2
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -2236,15 +2318,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.sensing_of_xposition(sprite)
-                
+
     def y_position_of(self, sprite):
         """y position of %2
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -2254,71 +2336,71 @@
         
 
         Returns
         -------
 
         """
         return self._core.sensing_of_yposition(sprite)
-                
+
     def reset_timer(self):
         """reset timer
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sensing_resettimer()
-                
+
     def set_drag_mode_draggable(self):
         """set drag mode draggable
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sensing_setdragmode_draggable()
-                
+
     def set_drag_mode_not_draggable(self):
         """set drag mode not draggable
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sensing_setdragmode_notdraggable()
-                
+
     def timer(self):
         """timer
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sensing_timer()
-                
+
     def touching_color(self, color):
         """touching color %1?
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -2328,43 +2410,43 @@
         
 
         Returns
         -------
 
         """
         return self._core.sensing_touchingcolor(color)
-                
+
     def touching_edge(self):
         """touching edge?
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sensing_touchingobject_edge()
-                
+
     def touching_mouse_pointer(self):
         """touching mouse-pointer?
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sensing_touchingobject_pointer()
-                
+
     def touching(self, sprite):
         """touching %1?
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -2374,29 +2456,29 @@
         
 
         Returns
         -------
 
         """
         return self._core.sensing_touchingobject_sprite(sprite)
-                
+
     def username(self):
         """username
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sensing_username()
-                
+
     def change_pan_left_right_effect_by(self, value):
         """change pan left/right effect by %2
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -2406,15 +2488,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.sound_changeeffectby_pan(value)
-                
+
     def change_pitch_effect_by(self, value):
         """change pitch effect by %2
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -2424,15 +2506,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.sound_changeeffectby_pitch(value)
-                
+
     def change_volume_by(self, value):
         """change volume by %1
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -2442,29 +2524,29 @@
         
 
         Returns
         -------
 
         """
         return self._core.sound_changevolumeby(value)
-                
+
     def clear_sound_effects(self):
         """clear sound effects
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sound_cleareffects()
-                
+
     def start_sound(self, name, loop=0):
         """start sound %1
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -2475,15 +2557,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.sound_play(name, loop=0)
-                
+
     def play_sound_until_done(self, name):
         """play sound %1 until done
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -2493,15 +2575,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.sound_playuntildone(name)
-                
+
     def set_pan_left_right_effect_to(self, value):
         """set pan left/right effect to %2
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -2511,15 +2593,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.sound_seteffectto_pan(value)
-                
+
     def set_pitch_effect_to(self, value):
         """set pitch effect to %2
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -2529,15 +2611,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.sound_seteffectto_pitch(value)
-                
+
     def set_volume_to(self, value):
         """set volume to %1%
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -2547,36 +2629,53 @@
         
 
         Returns
         -------
 
         """
         return self._core.sound_setvolumeto(value)
-                
+
     def stop_all_sounds(self):
         """stop all sounds
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sound_stopallsounds()
-                
+
     def volume(self):
         """volume
 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sound_volume()
-                
+
+    def set_name(self, name):
+        """set name of the sprite to %1%
+
+        Engl. Translation for your reference: ...
+        Engl. Documentation when available...
+
+        
+        Parameters
+        ----------
+        name : FILL
+        
+
+        Returns
+        -------
+
+        """
+        return self._core.pystage_setname(name)
```

### Comparing `pystage-0.0.9/src/pystage/en/stage.py` & `pystage-0.1.0.dev0/src/pystage/en/stage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-
-from pystage.core.stage import CoreStage
-from pystage.en.sprite import Sprite
+from pystage.core import CoreStage
+from pystage.en import Sprite
 
 
 class Stage():
 
     def __init__(self):
         self._core = CoreStage()
         self._core.facade = self
         self._core.sprite_facade_class = Sprite
 
-    def add_a_sprite(self, costume="default"):
+    def add_a_sprite(self, costume="default") -> Sprite:
         return self._core.pystage_createsprite(costume=costume)
 
     def play(self):
         self._core.pystage_play()
-        
-            
+
     def create_clone_of(self, sprite='_myself_'):
         """create clone of %1
 
         Translation string: create clone of %1
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -31,60 +29,60 @@
         
 
         Returns
         -------
 
         """
         return self._core.control_create_clone_of(sprite)
-                
+
     def stop_all(self):
         """stop all
 
         Translation string: stop all
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.control_stop_all()
-                
+
     def stop_other_scripts_in_sprite(self):
         """stop other scripts in sprite
 
         Translation string: stop other scripts in sprite
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.control_stop_other()
-                
+
     def stop_this_script(self):
         """stop this script
 
         Translation string: stop this script
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.control_stop_this()
-                
+
     def wait_seconds(self, secs):
         """wait %1 seconds
 
         Translation string: wait %1 seconds
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -95,15 +93,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.control_wait(secs)
-                
+
     def change_by(self, name, value):
         """change %1 by %2
 
         Translation string: change %1 by %2
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -115,15 +113,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.data_changevariableby(name, value)
-                
+
     def hide_variable(self, name):
         """hide variable %1
 
         Translation string: hide variable %1
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -134,15 +132,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.data_hidevariable(name)
-                
+
     def set_variable(self, name, value):
         """set %1 to %2
 
         Translation string: set %1 to %2
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -154,15 +152,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.data_setvariableto(name, value)
-                
+
     def show_variable(self, name):
         """show variable %1
 
         Translation string: show variable %1
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -173,15 +171,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.data_showvariable(name)
-                
+
     def get_variable(self, name):
         """
 
         Translation string: 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -192,15 +190,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.data_variable(name)
-                
+
     def broadcast(self, message):
         """broadcast %1
 
         Translation string: broadcast %1
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -211,15 +209,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.event_broadcast(message)
-                
+
     def broadcast_and_wait(self, message):
         """broadcast %1 and wait
 
         Translation string: broadcast %1 and wait
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -230,15 +228,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.event_broadcastandwait(message)
-                
+
     def when_backdrop_switches_to(self, backdrop, generator_function, name='', no_refresh=False):
         """when backdrop switches to %1
 
         Translation string: when backdrop switches to %1
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -252,15 +250,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.event_whenbackdropswitchesto(backdrop, generator_function, name, no_refresh)
-                
+
     def when_i_receive(self, message, generator_function, name='', no_refresh=False):
         """when I receive %1
 
         Translation string: when I receive %1
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -274,15 +272,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.event_whenbroadcastreceived(message, generator_function, name, no_refresh)
-                
+
     def when_GREENFLAG_clicked(self, generator_function, name='', no_refresh=False):
         """when <greenflag> clicked
 
         Translation string: when <greenflag> clicked
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -295,15 +293,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.event_whenflagclicked(generator_function, name, no_refresh)
-                
+
     def when_loudness_GREATERTHAN(self, value, generator_function, name='', no_refresh=False):
         """when loudness <greater> %2
 
         Translation string: when loudness <greater> %2
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -317,15 +315,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.event_whengreaterthan_loudness(value, generator_function, name, no_refresh)
-                
+
     def when_timer_GREATERTHAN(self, value, generator_function, name='', no_refresh=False):
         """when timer <greater> %2
 
         Translation string: when timer <greater> %2
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -339,15 +337,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.event_whengreaterthan_timer(value, generator_function, name, no_refresh)
-                
+
     def when_key_pressed(self, key, generator_function, name='', no_refresh=False):
         """when %1 key pressed
 
         Translation string: when %1 key pressed
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -361,15 +359,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.event_whenkeypressed(key, generator_function, name, no_refresh)
-                
+
     def when_this_sprite_clicked(self, generator_function, name='', no_refresh=False):
         """when this sprite clicked
 
         Translation string: when this sprite clicked
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -382,45 +380,45 @@
         
 
         Returns
         -------
 
         """
         return self._core.event_whenthisspriteclicked(generator_function, name, no_refresh)
-                
+
     def backdrop_name(self):
         """backdrop name
 
         Translation string: backdrop name
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.looks_backdropnumbername_name()
-                
+
     def backdrop_number(self):
         """backdrop number
 
         Translation string: backdrop number
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.looks_backdropnumbername_number()
-                
+
     def change_brightness_effect_by(self, value):
         """change brightness effect by %2
 
         Translation string: change brightness effect by %2
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -431,15 +429,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.looks_changeeffectby_brightness(value)
-                
+
     def change_color_effect_by(self, value):
         """change color effect by %2
 
         Translation string: change color effect by %2
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -450,15 +448,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.looks_changeeffectby_color(value)
-                
+
     def change_fisheye_effect_by(self, value):
         """change fisheye effect by %2
 
         Translation string: change fisheye effect by %2
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -469,15 +467,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.looks_changeeffectby_fisheye(value)
-                
+
     def change_ghost_effect_by(self, value):
         """change ghost effect by %2
 
         Translation string: change ghost effect by %2
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -488,15 +486,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.looks_changeeffectby_ghost(value)
-                
+
     def change_mosaic_effect_by(self, value):
         """change mosaic effect by %2
 
         Translation string: change mosaic effect by %2
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -507,15 +505,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.looks_changeeffectby_mosaic(value)
-                
+
     def change_pixelate_effect_by(self, value):
         """change pixelate effect by %2
 
         Translation string: change pixelate effect by %2
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -526,15 +524,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.looks_changeeffectby_pixelate(value)
-                
+
     def change_whirl_effect_by(self, value):
         """change whirl effect by %2
 
         Translation string: change whirl effect by %2
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -545,45 +543,45 @@
         
 
         Returns
         -------
 
         """
         return self._core.looks_changeeffectby_whirl(value)
-                
+
     def clear_graphic_effects(self):
         """clear graphic effects
 
         Translation string: clear graphic effects
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.looks_cleargraphiceffects()
-                
+
     def next_backdrop(self):
         """next backdrop
 
         Translation string: next backdrop
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.looks_nextbackdrop()
-                
+
     def set_brightness_effect_to(self, value):
         """set brightness effect to %2
 
         Translation string: set brightness effect to %2
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -594,15 +592,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.looks_seteffectto_brightness(value)
-                
+
     def set_color_effect_to(self, value):
         """set color effect to %2
 
         Translation string: set color effect to %2
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -613,15 +611,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.looks_seteffectto_color(value)
-                
+
     def set_fisheye_effect_to(self, value):
         """set fisheye effect to %2
 
         Translation string: set fisheye effect to %2
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -632,15 +630,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.looks_seteffectto_fisheye(value)
-                
+
     def set_ghost_effect_to(self, value):
         """set ghost effect to %2
 
         Translation string: set ghost effect to %2
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -651,15 +649,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.looks_seteffectto_ghost(value)
-                
+
     def set_mosaic_effect_to(self, value):
         """set mosaic effect to %2
 
         Translation string: set mosaic effect to %2
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -670,15 +668,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.looks_seteffectto_mosaic(value)
-                
+
     def set_pixelate_effect_to(self, value):
         """set pixelate effect to %2
 
         Translation string: set pixelate effect to %2
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -689,15 +687,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.looks_seteffectto_pixelate(value)
-                
+
     def set_whirl_effect_to(self, value):
         """set whirl effect to %2
 
         Translation string: set whirl effect to %2
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -708,15 +706,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.looks_seteffectto_whirl(value)
-                
+
     def switch_backdrop_to(self, backdrop):
         """switch backdrop to %1
 
         Translation string: switch backdrop to %1
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -727,15 +725,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.looks_switchbackdropto(backdrop)
-                
+
     def switch_backdrop_to_and_wait(self, backdrop):
         """switch backdrop to %1 and wait
 
         Translation string: switch backdrop to %1 and wait
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -746,15 +744,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.looks_switchbackdroptoandwait(backdrop)
-                
+
     def of(self, operator, number):
         """%1 of %2
 
         Translation string: %1 of %2
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -766,15 +764,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.operator_mathop(operator, number)
-                
+
     def pick_random_to(self, start, end):
         """pick random %1 to %2
 
         Translation string: pick random %1 to %2
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -786,15 +784,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.operator_random(start, end)
-                
+
     def add_backdrop(self, name, center_x=None, center_y=None):
         """
 
         Translation string: 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -807,15 +805,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.pystage_addbackdrop(name, center_x, center_y)
-                
+
     def pystage_addsound(self, name):
         """
 
         Translation string: 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -826,15 +824,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.pystage_addsound(name)
-                
+
     def pystage_createsprite(self, costume='default'):
         """
 
         Translation string: 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -845,15 +843,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.pystage_createsprite(costume)
-                
+
     def pystage_insertbackdrop(self, index, name, center_x=None, center_y=None):
         """
 
         Translation string: 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -867,15 +865,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.pystage_insertbackdrop(index, name, center_x, center_y)
-                
+
     def create_variable(self, name, all_sprites=True):
         """
 
         Translation string: 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -887,30 +885,30 @@
         
 
         Returns
         -------
 
         """
         return self._core.pystage_makevariable(name, all_sprites)
-                
+
     def pystage_play(self):
         """
 
         Translation string: 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.pystage_play()
-                
+
     def pystage_replacebackdrop(self, index, name, center_x=None, center_y=None):
         """
 
         Translation string: 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -924,16 +922,16 @@
         
 
         Returns
         -------
 
         """
         return self._core.pystage_replacebackdrop(index, name, center_x, center_y)
-                
-    def pystage_setmonitorposition(self, name, x, y):
+
+    def set_monitor_position(self, name, x, y):
         """
 
         Translation string: 
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
@@ -945,29 +943,87 @@
         
 
         Returns
         -------
 
         """
         return self._core.pystage_setmonitorposition(name, x, y)
+
+    def pystage_setmonitorstyle_large(self, name):
+        """
+
+        Translation string: 
+        Engl. Translation for your reference: ...
+        Engl. Documentation when available...
+
+        
+        Parameters
+        ----------
+        name : FILL
+        
+
+        Returns
+        -------
+
+        """
+        return self._core.pystage_setmonitorstyle_large(name)
+
+    def pystage_setmonitorstyle_normal(self, name):
+        """
+
+        Translation string: 
+        Engl. Translation for your reference: ...
+        Engl. Documentation when available...
+
+        
+        Parameters
+        ----------
+        name : FILL
+        
+
+        Returns
+        -------
+
+        """
+        return self._core.pystage_setmonitorstyle_normal(name)
+
+    def pystage_setmonitorstyle_slider(self, name):
+        """
+
+        Translation string: 
+        Engl. Translation for your reference: ...
+        Engl. Documentation when available...
+
+        
+        Parameters
+        ----------
+        name : FILL
+        
+
+        Returns
+        -------
+
+        """
+        return self._core.pystage_setmonitorstyle_slider(name)
+
     def answer(self):
         """answer
 
         Translation string: answer
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sensing_answer()
-                
+
     def ask_and_wait(self, question):
         """ask %1 and wait
 
         Translation string: ask %1 and wait
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -978,135 +1034,135 @@
         
 
         Returns
         -------
 
         """
         return self._core.sensing_askandwait(question)
-                
+
     def current_date(self):
         """current date
 
         Translation string: current date
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sensing_current_date()
-                
+
     def current_day_of_week(self):
         """current day of week
 
         Translation string: current day of week
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sensing_current_dayofweek()
-                
+
     def current_hour(self):
         """current hour
 
         Translation string: current hour
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sensing_current_hour()
-                
+
     def current_minute(self):
         """current minute
 
         Translation string: current minute
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sensing_current_minute()
-                
+
     def current_month(self):
         """current month
 
         Translation string: current month
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sensing_current_month()
-                
+
     def current_second(self):
         """current second
 
         Translation string: current second
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sensing_current_second()
-                
+
     def current_year(self):
         """current year
 
         Translation string: current year
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sensing_current_year()
-                
+
     def days_since(self):
         """days since 2000
 
         Translation string: days since 2000
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sensing_dayssince2000()
-                
+
     def key_pressed(self, key):
         """key %1 pressed?
 
         Translation string: key %1 pressed?
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -1117,75 +1173,75 @@
         
 
         Returns
         -------
 
         """
         return self._core.sensing_keypressed(key)
-                
+
     def loudness(self):
         """loudness
 
         Translation string: loudness
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sensing_loudness()
-                
+
     def mouse_down(self):
         """mouse down?
 
         Translation string: mouse down?
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sensing_mousedown()
-                
+
     def mouse_x(self):
         """mouse x
 
         Translation string: mouse x
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sensing_mousex()
-                
+
     def mouse_y(self):
         """mouse y
 
         Translation string: mouse y
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sensing_mousey()
-                
+
     def backdrop_name_of(self, stage='_stage_'):
         """backdrop name of %2
 
         Translation string: backdrop name of %2
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -1196,15 +1252,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.sensing_of_backdropname(stage)
-                
+
     def backdrop_of(self, stage='_stage_'):
         """backdrop # of %2
 
         Translation string: backdrop # of %2
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -1215,15 +1271,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.sensing_of_backdropnumber(stage)
-                
+
     def costume_name_of(self, sprite):
         """costume name of %2
 
         Translation string: costume name of %2
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -1234,15 +1290,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.sensing_of_costumename(sprite)
-                
+
     def costume_of(self, sprite):
         """costume # of %2
 
         Translation string: costume # of %2
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -1253,15 +1309,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.sensing_of_costumenumber(sprite)
-                
+
     def direction_of(self, sprite):
         """direction of %2
 
         Translation string: direction of %2
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -1272,15 +1328,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.sensing_of_direction(sprite)
-                
+
     def size_of(self, sprite):
         """size of %2
 
         Translation string: size of %2
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -1291,15 +1347,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.sensing_of_size(sprite)
-                
+
     def of(self, variable, sprite='_stage_'):
         """%1 of %2
 
         Translation string: %1 of %2
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -1311,15 +1367,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.sensing_of_variable(variable, sprite)
-                
+
     def volume_of(self, sprite='_stage_'):
         """volume of %2
 
         Translation string: volume of %2
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -1330,15 +1386,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.sensing_of_volume(sprite)
-                
+
     def x_position_of(self, sprite):
         """x position of %2
 
         Translation string: x position of %2
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -1349,15 +1405,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.sensing_of_xposition(sprite)
-                
+
     def y_position_of(self, sprite):
         """y position of %2
 
         Translation string: y position of %2
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -1368,90 +1424,90 @@
         
 
         Returns
         -------
 
         """
         return self._core.sensing_of_yposition(sprite)
-                
+
     def reset_timer(self):
         """reset timer
 
         Translation string: reset timer
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sensing_resettimer()
-                
+
     def set_drag_mode_draggable(self):
         """set drag mode draggable
 
         Translation string: set drag mode draggable
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sensing_setdragmode_draggable()
-                
+
     def set_drag_mode_not_draggable(self):
         """set drag mode not draggable
 
         Translation string: set drag mode not draggable
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sensing_setdragmode_notdraggable()
-                
+
     def timer(self):
         """timer
 
         Translation string: timer
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sensing_timer()
-                
+
     def username(self):
         """username
 
         Translation string: username
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sensing_username()
-                
+
     def change_pan_left_right_effect_by(self, value):
         """change pan left/right effect by %2
 
         Translation string: change pan left/right effect by %2
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -1462,15 +1518,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.sound_changeeffectby_pan(value)
-                
+
     def change_pitch_effect_by(self, value):
         """change pitch effect by %2
 
         Translation string: change pitch effect by %2
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -1481,15 +1537,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.sound_changeeffectby_pitch(value)
-                
+
     def change_volume_by(self, value):
         """change volume by %1
 
         Translation string: change volume by %1
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -1500,30 +1556,30 @@
         
 
         Returns
         -------
 
         """
         return self._core.sound_changevolumeby(value)
-                
+
     def clear_sound_effects(self):
         """clear sound effects
 
         Translation string: clear sound effects
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sound_cleareffects()
-                
+
     def start_sound(self, name, loop=0):
         """start sound %1
 
         Translation string: start sound %1
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -1535,15 +1591,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.sound_play(name, loop)
-                
+
     def play_sound_until_done(self, name):
         """play sound %1 until done
 
         Translation string: play sound %1 until done
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -1554,15 +1610,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.sound_playuntildone(name)
-                
+
     def set_pan_left_right_effect_to(self, value):
         """set pan left/right effect to %2
 
         Translation string: set pan left/right effect to %2
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -1573,15 +1629,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.sound_seteffectto_pan(value)
-                
+
     def set_pitch_effect_to(self, value):
         """set pitch effect to %2
 
         Translation string: set pitch effect to %2
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -1592,15 +1648,15 @@
         
 
         Returns
         -------
 
         """
         return self._core.sound_seteffectto_pitch(value)
-                
+
     def set_volume_to(self, value):
         """set volume to %1%
 
         Translation string: set volume to %1%
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
@@ -1611,38 +1667,37 @@
         
 
         Returns
         -------
 
         """
         return self._core.sound_setvolumeto(value)
-                
+
     def stop_all_sounds(self):
         """stop all sounds
 
         Translation string: stop all sounds
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sound_stopallsounds()
-                
+
     def volume(self):
         """volume
 
         Translation string: volume
         Engl. Translation for your reference: ...
         Engl. Documentation when available...
 
         
 
         Returns
         -------
 
         """
         return self._core.sound_volume()
-
```

### Comparing `pystage-0.0.9/src/pystage/fonts/roboto-bold.ttf` & `pystage-0.1.0.dev0/src/pystage/fonts/roboto-bold.ttf`

 * *Files identical despite different names*

### Comparing `pystage-0.0.9/src/pystage/fonts/roboto-light.ttf` & `pystage-0.1.0.dev0/src/pystage/fonts/roboto-light.ttf`

 * *Files identical despite different names*

### Comparing `pystage-0.0.9/src/pystage/fonts/roboto-regular.ttf` & `pystage-0.1.0.dev0/src/pystage/fonts/roboto-regular.ttf`

 * *Files identical despite different names*

### Comparing `pystage-0.0.9/src/pystage/images/grid.svg` & `pystage-0.1.0.dev0/src/pystage/images/grid.svg`

 * *Files identical despite different names*

### Comparing `pystage-0.0.9/src/pystage/images/say.png` & `pystage-0.1.0.dev0/src/pystage/images/say.png`

 * *Files identical despite different names*

### Comparing `pystage-0.0.9/src/pystage/images/think.png` & `pystage-0.1.0.dev0/src/pystage/images/think.png`

 * *Files identical despite different names*

### Comparing `pystage-0.0.9/src/pystage/images/zombie_idle.png` & `pystage-0.1.0.dev0/src/pystage/images/zombie_idle.png`

 * *Files identical despite different names*

### Comparing `pystage-0.0.9/src/pystage/l10n/__main__.py` & `pystage-0.1.0.dev0/src/pystage/l10n/__main__.py`

 * *Files identical despite different names*

### Comparing `pystage-0.0.9/src/pystage/l10n/api.py` & `pystage-0.1.0.dev0/src/pystage/l10n/api.py`

 * *Files identical despite different names*

### Comparing `pystage-0.0.9/src/pystage/l10n/translations.py` & `pystage-0.1.0.dev0/src/pystage/l10n/translations.py`

 * *Files identical despite different names*

### Comparing `pystage-0.0.9/src/pystage/sounds/dancehead2.wav` & `pystage-0.1.0.dev0/src/pystage/sounds/dancehead2.wav`

 * *Files identical despite different names*

### Comparing `pystage-0.0.9/src/pystage/sounds/guitar.wav` & `pystage-0.1.0.dev0/src/pystage/sounds/guitar.wav`

 * *Files identical despite different names*

### Comparing `pystage-0.0.9/src/pystage/util.py` & `pystage-0.1.0.dev0/src/pystage/util.py`

 * *Files identical despite different names*

### Comparing `pystage-0.0.9/src/pystage.egg-info/SOURCES.txt` & `pystage-0.1.0.dev0/src/pystage.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -20,36 +20,36 @@
 src/pystage/core/_looks.py
 src/pystage/core/_motion.py
 src/pystage/core/_operators.py
 src/pystage/core/_pen.py
 src/pystage/core/_sensing.py
 src/pystage/core/_sound.py
 src/pystage/core/_variables.py
+src/pystage/core/asking.py
 src/pystage/core/assets.py
 src/pystage/core/code_block.py
 src/pystage/core/constants.py
 src/pystage/core/gui.py
 src/pystage/core/messages.py
+src/pystage/core/monitors.py
 src/pystage/core/sprite.py
 src/pystage/core/stage.py
 src/pystage/de/__init__.py
 src/pystage/de/sprite.py
 src/pystage/de/stage.py
 src/pystage/en/__init__.py
 src/pystage/en/sprite.py
 src/pystage/en/stage.py
 src/pystage/fonts/roboto-bold.ttf
 src/pystage/fonts/roboto-light.ttf
 src/pystage/fonts/roboto-regular.ttf
 src/pystage/images/grid.svg
+src/pystage/images/pen.png
 src/pystage/images/say.png
 src/pystage/images/think.png
 src/pystage/images/zombie_idle.png
-src/pystage/ja/__init__.py
-src/pystage/ja/sprite.py
-src/pystage/ja/stage.py
 src/pystage/l10n/__init__.py
 src/pystage/l10n/__main__.py
 src/pystage/l10n/api.py
 src/pystage/l10n/translations.py
 src/pystage/sounds/dancehead2.wav
 src/pystage/sounds/guitar.wav
```

