# Comparing `tmp/ipyweb-1.0.7.tar.gz` & `tmp/ipyweb-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyweb-1.0.7.tar", last modified: Sat Jun  1 00:05:51 2024, max compression
+gzip compressed data, was "ipyweb-1.0.8.tar", last modified: Mon Jun  3 10:39:46 2024, max compression
```

## Comparing `ipyweb-1.0.7.tar` & `ipyweb-1.0.8.tar`

### file list

```diff
@@ -1,95 +1,97 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 00:05:51.422106 ipyweb-1.0.7/
--rw-rw-rw-   0        0        0     1547 2024-05-16 17:34:29.000000 ipyweb-1.0.7/LICENSE
--rw-rw-rw-   0        0        0     2193 2024-06-01 00:05:51.419093 ipyweb-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       43 2024-05-31 07:23:39.000000 ipyweb-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 00:05:51.270216 ipyweb-1.0.7/ipyweb/
--rw-rw-rw-   0        0        0        0 2024-05-31 04:11:12.000000 ipyweb-1.0.7/ipyweb/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 00:05:51.292123 ipyweb-1.0.7/ipyweb/addons/
--rw-rw-rw-   0        0        0     3561 2024-05-31 01:15:14.000000 ipyweb-1.0.7/ipyweb/addons/loadingGui.py
--rw-rw-rw-   0        0        0     3713 2024-05-30 23:10:57.000000 ipyweb-1.0.7/ipyweb/app.py
--rw-rw-rw-   0        0        0     4937 2024-05-31 12:45:56.000000 ipyweb-1.0.7/ipyweb/appRunner.py
-drwxrwxrwx   0        0        0        0 2024-06-01 00:05:51.295675 ipyweb-1.0.7/ipyweb/builds/
--rw-rw-rw-   0        0        0     7382 2024-05-31 17:08:44.000000 ipyweb-1.0.7/ipyweb/builds/builder.py
-drwxrwxrwx   0        0        0        0 2024-06-01 00:05:51.301669 ipyweb-1.0.7/ipyweb/builds/hooks/
--rw-rw-rw-   0        0        0     8819 2024-05-28 19:03:37.000000 ipyweb-1.0.7/ipyweb/builds/hooks/hook-cefpython3.py
--rw-rw-rw-   0        0        0      241 2024-05-31 17:04:35.000000 ipyweb-1.0.7/ipyweb/builds/hooks/hook-ipyweb.py
--rw-rw-rw-   0        0        0     4722 2024-05-31 18:04:56.000000 ipyweb-1.0.7/ipyweb/cache.py
--rw-rw-rw-   0        0        0      316 2024-05-31 07:19:21.000000 ipyweb-1.0.7/ipyweb/cli.py
--rw-rw-rw-   0        0        0     3568 2024-05-31 00:44:58.000000 ipyweb-1.0.7/ipyweb/command.py
-drwxrwxrwx   0        0        0        0 2024-06-01 00:05:51.308245 ipyweb-1.0.7/ipyweb/commands/
--rw-rw-rw-   0        0        0     1924 2024-05-31 23:58:13.000000 ipyweb-1.0.7/ipyweb/commands/ipywebBuilder.py
--rw-rw-rw-   0        0        0     2022 2024-05-31 23:58:27.000000 ipyweb-1.0.7/ipyweb/commands/ipywebRunner.py
--rw-rw-rw-   0        0        0     9804 2024-05-31 11:36:50.000000 ipyweb-1.0.7/ipyweb/config.py
-drwxrwxrwx   0        0        0        0 2024-06-01 00:05:51.335050 ipyweb-1.0.7/ipyweb/configs/
--rw-rw-rw-   0        0        0     1010 2024-05-28 16:39:36.000000 ipyweb-1.0.7/ipyweb/configs/app.py
--rw-rw-rw-   0        0        0      363 2024-05-30 15:55:41.000000 ipyweb-1.0.7/ipyweb/configs/build.py
--rw-rw-rw-   0        0        0      225 2024-05-12 09:40:00.000000 ipyweb-1.0.7/ipyweb/configs/cache.py
--rw-rw-rw-   0        0        0     1050 2024-05-12 09:51:21.000000 ipyweb-1.0.7/ipyweb/configs/database.py
--rw-rw-rw-   0        0        0       62 2024-05-10 17:35:35.000000 ipyweb-1.0.7/ipyweb/configs/jsonFile.py
--rw-rw-rw-   0        0        0     1130 2024-05-29 18:24:21.000000 ipyweb-1.0.7/ipyweb/configs/logger.py
--rw-rw-rw-   0        0        0     2881 2024-05-30 15:55:40.000000 ipyweb-1.0.7/ipyweb/configs/windows.py
-drwxrwxrwx   0        0        0        0 2024-06-01 00:05:51.356706 ipyweb-1.0.7/ipyweb/contracts/
--rw-rw-rw-   0        0        0      104 2024-05-30 15:55:41.000000 ipyweb-1.0.7/ipyweb/contracts/ipywebAddon.py
--rw-rw-rw-   0        0        0      641 2024-05-30 15:55:41.000000 ipyweb-1.0.7/ipyweb/contracts/ipywebController.py
--rw-rw-rw-   0        0        0      423 2024-05-31 18:08:29.000000 ipyweb-1.0.7/ipyweb/contracts/ipywebException.py
--rw-rw-rw-   0        0        0     1037 2024-05-31 12:37:53.000000 ipyweb-1.0.7/ipyweb/contracts/ipywebHttpController.py
--rw-rw-rw-   0        0        0      154 2024-05-30 15:55:41.000000 ipyweb-1.0.7/ipyweb/contracts/ipywebModel.py
--rw-rw-rw-   0        0        0      410 2024-05-30 15:55:41.000000 ipyweb-1.0.7/ipyweb/contracts/ipywebPreload.py
--rw-rw-rw-   0        0        0       93 2024-05-30 19:22:02.000000 ipyweb-1.0.7/ipyweb/contracts/ipywebQueue.py
--rw-rw-rw-   0        0        0      154 2024-05-31 01:10:19.000000 ipyweb-1.0.7/ipyweb/contracts/ipywebRunner.py
--rw-rw-rw-   0        0        0     6971 2024-05-31 06:56:48.000000 ipyweb-1.0.7/ipyweb/controller.py
-drwxrwxrwx   0        0        0        0 2024-06-01 00:05:51.359729 ipyweb-1.0.7/ipyweb/controllers/
--rw-rw-rw-   0        0        0     7422 2024-05-31 12:37:17.000000 ipyweb-1.0.7/ipyweb/controllers/ipyweb.py
--rw-rw-rw-   0        0        0     4646 2024-05-31 01:49:46.000000 ipyweb-1.0.7/ipyweb/db.py
--rw-rw-rw-   0        0        0    10557 2024-05-31 00:27:17.000000 ipyweb-1.0.7/ipyweb/event.py
-drwxrwxrwx   0        0        0        0 2024-06-01 00:05:51.191969 ipyweb-1.0.7/ipyweb/events/
-drwxrwxrwx   0        0        0        0 2024-06-01 00:05:51.362709 ipyweb-1.0.7/ipyweb/events/listener/
--rw-rw-rw-   0        0        0      453 2024-05-30 19:21:37.000000 ipyweb-1.0.7/ipyweb/events/listener/windows.py
-drwxrwxrwx   0        0        0        0 2024-06-01 00:05:51.365808 ipyweb-1.0.7/ipyweb/events/register/
--rw-rw-rw-   0        0        0      686 2024-05-30 19:21:42.000000 ipyweb-1.0.7/ipyweb/events/register/windows.py
--rw-rw-rw-   0        0        0     1699 2024-05-30 15:56:03.000000 ipyweb-1.0.7/ipyweb/gui.py
-drwxrwxrwx   0        0        0        0 2024-06-01 00:05:51.380910 ipyweb-1.0.7/ipyweb/guis/
--rw-rw-rw-   0        0        0      987 2024-05-30 15:55:41.000000 ipyweb-1.0.7/ipyweb/guis/BottleServer.py
--rw-rw-rw-   0        0        0     3822 2024-05-30 15:55:41.000000 ipyweb-1.0.7/ipyweb/guis/FlaskServer.py
--rw-rw-rw-   0        0        0     3922 2024-05-30 15:56:03.000000 ipyweb-1.0.7/ipyweb/guis/IpywebServer.py
--rw-rw-rw-   0        0        0     1491 2024-05-31 01:07:59.000000 ipyweb-1.0.7/ipyweb/guis/LocalServer.py
--rw-rw-rw-   0        0        0     1446 2024-05-30 19:21:31.000000 ipyweb-1.0.7/ipyweb/guis/RemoteServer.py
--rw-rw-rw-   0        0        0     6259 2024-05-31 18:08:21.000000 ipyweb-1.0.7/ipyweb/ipyweb.py
--rw-rw-rw-   0        0        0     2546 2024-05-31 00:12:02.000000 ipyweb-1.0.7/ipyweb/jsonFile.py
--rw-rw-rw-   0        0        0     2531 2024-05-31 18:28:49.000000 ipyweb-1.0.7/ipyweb/logger.py
--rw-rw-rw-   0        0        0     7935 2024-05-31 00:45:17.000000 ipyweb-1.0.7/ipyweb/module.py
--rw-rw-rw-   0        0        0      247 2024-05-05 11:24:12.000000 ipyweb-1.0.7/ipyweb/multiton.py
--rw-rw-rw-   0        0        0     8722 2024-05-31 00:04:40.000000 ipyweb-1.0.7/ipyweb/preload.py
-drwxrwxrwx   0        0        0        0 2024-06-01 00:05:51.197350 ipyweb-1.0.7/ipyweb/preloads/
-drwxrwxrwx   0        0        0        0 2024-06-01 00:05:51.388480 ipyweb-1.0.7/ipyweb/preloads/block/
--rw-rw-rw-   0        0        0     1555 2024-05-31 01:00:22.000000 ipyweb-1.0.7/ipyweb/preloads/block/controllerPreload.py
--rw-rw-rw-   0        0        0      404 2024-05-30 15:56:03.000000 ipyweb-1.0.7/ipyweb/preloads/block/guiPreload.py
--rw-rw-rw-   0        0        0      420 2024-05-30 15:56:03.000000 ipyweb-1.0.7/ipyweb/preloads/block/processPreload.py
-drwxrwxrwx   0        0        0        0 2024-06-01 00:05:51.393505 ipyweb-1.0.7/ipyweb/preloads/process/
--rw-rw-rw-   0        0        0      487 2024-05-30 19:20:37.000000 ipyweb-1.0.7/ipyweb/preloads/process/examplePreload.py
-drwxrwxrwx   0        0        0        0 2024-06-01 00:05:51.400039 ipyweb-1.0.7/ipyweb/preloads/thread/
--rw-rw-rw-   0        0        0     2981 2024-05-31 01:03:40.000000 ipyweb-1.0.7/ipyweb/preloads/thread/queuePreload.py
--rw-rw-rw-   0        0        0     2953 2024-05-31 01:04:52.000000 ipyweb-1.0.7/ipyweb/preloads/thread/socketPreload.py
--rw-rw-rw-   0        0        0     2216 2024-05-31 01:06:07.000000 ipyweb-1.0.7/ipyweb/preloads/thread/timerPreload.py
--rw-rw-rw-   0        0        0    10863 2024-05-31 18:12:07.000000 ipyweb-1.0.7/ipyweb/process.py
-drwxrwxrwx   0        0        0        0 2024-06-01 00:05:51.402044 ipyweb-1.0.7/ipyweb/pywebview/
--rw-rw-rw-   0        0        0     9284 2024-05-31 18:05:32.000000 ipyweb-1.0.7/ipyweb/pywebview/windows.py
--rw-rw-rw-   0        0        0     4587 2024-05-31 11:42:57.000000 ipyweb-1.0.7/ipyweb/service.py
-drwxrwxrwx   0        0        0        0 2024-06-01 00:05:51.411558 ipyweb-1.0.7/ipyweb/services/
--rw-rw-rw-   0        0        0     8227 2024-05-31 13:15:40.000000 ipyweb-1.0.7/ipyweb/services/queue.py
--rw-rw-rw-   0        0        0     7626 2024-05-31 13:15:03.000000 ipyweb-1.0.7/ipyweb/services/socketServer.py
--rw-rw-rw-   0        0        0     2671 2024-05-31 00:49:24.000000 ipyweb-1.0.7/ipyweb/services/timer.py
--rw-rw-rw-   0        0        0      470 2024-05-05 11:23:41.000000 ipyweb-1.0.7/ipyweb/singleton.py
--rw-rw-rw-   0        0        0     5026 2024-05-30 23:58:28.000000 ipyweb-1.0.7/ipyweb/thread.py
--rw-rw-rw-   0        0        0     4552 2024-05-31 18:20:45.000000 ipyweb-1.0.7/ipyweb/utils.py
-drwxrwxrwx   0        0        0        0 2024-06-01 00:05:51.414083 ipyweb-1.0.7/ipyweb/windowEvents/
--rw-rw-rw-   0        0        0     2163 2024-05-31 14:32:07.000000 ipyweb-1.0.7/ipyweb/windowEvents/main.py
-drwxrwxrwx   0        0        0        0 2024-06-01 00:05:51.417106 ipyweb-1.0.7/ipyweb.egg-info/
--rw-rw-rw-   0        0        0     2193 2024-06-01 00:05:51.000000 ipyweb-1.0.7/ipyweb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1888 2024-06-01 00:05:51.000000 ipyweb-1.0.7/ipyweb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 00:05:51.000000 ipyweb-1.0.7/ipyweb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-06-01 00:05:51.000000 ipyweb-1.0.7/ipyweb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       25 2024-06-01 00:05:51.000000 ipyweb-1.0.7/ipyweb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-06-01 00:05:51.000000 ipyweb-1.0.7/ipyweb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1209 2024-06-01 00:05:34.000000 ipyweb-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-06-01 00:05:51.422106 ipyweb-1.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-03 10:39:46.619290 ipyweb-1.0.8/
+-rw-rw-rw-   0        0        0     1547 2024-05-16 17:34:29.000000 ipyweb-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0     2193 2024-06-03 10:39:46.616289 ipyweb-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       43 2024-05-31 07:23:39.000000 ipyweb-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 10:39:46.438852 ipyweb-1.0.8/ipyweb/
+-rw-rw-rw-   0        0        0        0 2024-05-31 04:11:12.000000 ipyweb-1.0.8/ipyweb/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:39:46.458833 ipyweb-1.0.8/ipyweb/addons/
+-rw-rw-rw-   0        0        0     3759 2024-06-03 03:03:24.000000 ipyweb-1.0.8/ipyweb/addons/loadingGui.py
+-rw-rw-rw-   0        0        0     3744 2024-06-03 03:04:04.000000 ipyweb-1.0.8/ipyweb/app.py
+-rw-rw-rw-   0        0        0     4937 2024-05-31 12:45:56.000000 ipyweb-1.0.8/ipyweb/appRunner.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:39:46.462831 ipyweb-1.0.8/ipyweb/builds/
+-rw-rw-rw-   0        0        0     7376 2024-06-01 15:29:58.000000 ipyweb-1.0.8/ipyweb/builds/builder.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:39:46.468834 ipyweb-1.0.8/ipyweb/builds/hooks/
+-rw-rw-rw-   0        0        0     8819 2024-05-28 19:03:37.000000 ipyweb-1.0.8/ipyweb/builds/hooks/hook-cefpython3.py
+-rw-rw-rw-   0        0        0      241 2024-05-31 17:04:35.000000 ipyweb-1.0.8/ipyweb/builds/hooks/hook-ipyweb.py
+-rw-rw-rw-   0        0        0     4829 2024-06-01 15:19:06.000000 ipyweb-1.0.8/ipyweb/cache.py
+-rw-rw-rw-   0        0        0      316 2024-05-31 07:19:21.000000 ipyweb-1.0.8/ipyweb/cli.py
+-rw-rw-rw-   0        0        0     3568 2024-05-31 00:44:58.000000 ipyweb-1.0.8/ipyweb/command.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:39:46.475652 ipyweb-1.0.8/ipyweb/commands/
+-rw-rw-rw-   0        0        0     1924 2024-05-31 23:58:13.000000 ipyweb-1.0.8/ipyweb/commands/ipywebBuilder.py
+-rw-rw-rw-   0        0        0     2022 2024-05-31 23:58:27.000000 ipyweb-1.0.8/ipyweb/commands/ipywebRunner.py
+-rw-rw-rw-   0        0        0     9804 2024-05-31 11:36:50.000000 ipyweb-1.0.8/ipyweb/config.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:39:46.497670 ipyweb-1.0.8/ipyweb/configs/
+-rw-rw-rw-   0        0        0     1491 2024-06-01 15:06:52.000000 ipyweb-1.0.8/ipyweb/configs/app.py
+-rw-rw-rw-   0        0        0      363 2024-05-30 15:55:41.000000 ipyweb-1.0.8/ipyweb/configs/build.py
+-rw-rw-rw-   0        0        0      225 2024-05-12 09:40:00.000000 ipyweb-1.0.8/ipyweb/configs/cache.py
+-rw-rw-rw-   0        0        0     1050 2024-05-12 09:51:21.000000 ipyweb-1.0.8/ipyweb/configs/database.py
+-rw-rw-rw-   0        0        0       62 2024-05-10 17:35:35.000000 ipyweb-1.0.8/ipyweb/configs/jsonFile.py
+-rw-rw-rw-   0        0        0     1130 2024-05-29 18:24:21.000000 ipyweb-1.0.8/ipyweb/configs/logger.py
+-rw-rw-rw-   0        0        0     3066 2024-06-03 03:23:31.000000 ipyweb-1.0.8/ipyweb/configs/windows.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:39:46.523290 ipyweb-1.0.8/ipyweb/contracts/
+-rw-rw-rw-   0        0        0      104 2024-05-30 15:55:41.000000 ipyweb-1.0.8/ipyweb/contracts/ipywebAddon.py
+-rw-rw-rw-   0        0        0      641 2024-05-30 15:55:41.000000 ipyweb-1.0.8/ipyweb/contracts/ipywebController.py
+-rw-rw-rw-   0        0        0      423 2024-05-31 18:08:29.000000 ipyweb-1.0.8/ipyweb/contracts/ipywebException.py
+-rw-rw-rw-   0        0        0     1037 2024-05-31 12:37:53.000000 ipyweb-1.0.8/ipyweb/contracts/ipywebHttpController.py
+-rw-rw-rw-   0        0        0      154 2024-05-30 15:55:41.000000 ipyweb-1.0.8/ipyweb/contracts/ipywebModel.py
+-rw-rw-rw-   0        0        0      410 2024-05-30 15:55:41.000000 ipyweb-1.0.8/ipyweb/contracts/ipywebPreload.py
+-rw-rw-rw-   0        0        0       93 2024-05-30 19:22:02.000000 ipyweb-1.0.8/ipyweb/contracts/ipywebQueue.py
+-rw-rw-rw-   0        0        0      154 2024-05-31 01:10:19.000000 ipyweb-1.0.8/ipyweb/contracts/ipywebRunner.py
+-rw-rw-rw-   0        0        0     6971 2024-05-31 06:56:48.000000 ipyweb-1.0.8/ipyweb/controller.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:39:46.527292 ipyweb-1.0.8/ipyweb/controllers/
+-rw-rw-rw-   0        0        0     7529 2024-06-03 02:39:02.000000 ipyweb-1.0.8/ipyweb/controllers/ipyweb.py
+-rw-rw-rw-   0        0        0     4775 2024-06-01 15:19:50.000000 ipyweb-1.0.8/ipyweb/db.py
+-rw-rw-rw-   0        0        0    10557 2024-05-31 00:27:17.000000 ipyweb-1.0.8/ipyweb/event.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:39:46.354842 ipyweb-1.0.8/ipyweb/events/
+drwxrwxrwx   0        0        0        0 2024-06-03 10:39:46.531291 ipyweb-1.0.8/ipyweb/events/listener/
+-rw-rw-rw-   0        0        0      453 2024-05-30 19:21:37.000000 ipyweb-1.0.8/ipyweb/events/listener/windows.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:39:46.534290 ipyweb-1.0.8/ipyweb/events/register/
+-rw-rw-rw-   0        0        0      490 2024-06-03 01:58:43.000000 ipyweb-1.0.8/ipyweb/events/register/windows.py
+-rw-rw-rw-   0        0        0     1892 2024-06-03 03:30:56.000000 ipyweb-1.0.8/ipyweb/gui.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:39:46.553290 ipyweb-1.0.8/ipyweb/guis/
+-rw-rw-rw-   0        0        0      985 2024-06-01 13:31:51.000000 ipyweb-1.0.8/ipyweb/guis/BottleServer.py
+-rw-rw-rw-   0        0        0     3822 2024-05-30 15:55:41.000000 ipyweb-1.0.8/ipyweb/guis/FlaskServer.py
+-rw-rw-rw-   0        0        0     3922 2024-05-30 15:56:03.000000 ipyweb-1.0.8/ipyweb/guis/IpywebServer.py
+-rw-rw-rw-   0        0        0     1491 2024-05-31 01:07:59.000000 ipyweb-1.0.8/ipyweb/guis/LocalServer.py
+-rw-rw-rw-   0        0        0     1446 2024-05-30 19:21:31.000000 ipyweb-1.0.8/ipyweb/guis/RemoteServer.py
+-rw-rw-rw-   0        0        0     6255 2024-06-03 02:46:26.000000 ipyweb-1.0.8/ipyweb/ipyweb.py
+-rw-rw-rw-   0        0        0     2546 2024-05-31 00:12:02.000000 ipyweb-1.0.8/ipyweb/jsonFile.py
+-rw-rw-rw-   0        0        0     2531 2024-05-31 18:28:49.000000 ipyweb-1.0.8/ipyweb/logger.py
+-rw-rw-rw-   0        0        0     7967 2024-06-01 03:41:08.000000 ipyweb-1.0.8/ipyweb/module.py
+-rw-rw-rw-   0        0        0     7702 2024-06-01 15:06:13.000000 ipyweb-1.0.8/ipyweb/preload.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:39:46.361880 ipyweb-1.0.8/ipyweb/preloads/
+drwxrwxrwx   0        0        0        0 2024-06-03 10:39:46.564289 ipyweb-1.0.8/ipyweb/preloads/block/
+-rw-rw-rw-   0        0        0     1555 2024-05-31 01:00:22.000000 ipyweb-1.0.8/ipyweb/preloads/block/controllerPreload.py
+-rw-rw-rw-   0        0        0      404 2024-05-30 15:56:03.000000 ipyweb-1.0.8/ipyweb/preloads/block/guiPreload.py
+-rw-rw-rw-   0        0        0      420 2024-05-30 15:56:03.000000 ipyweb-1.0.8/ipyweb/preloads/block/processPreload.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:39:46.567289 ipyweb-1.0.8/ipyweb/preloads/process/
+-rw-rw-rw-   0        0        0      641 2024-06-01 14:47:21.000000 ipyweb-1.0.8/ipyweb/preloads/process/examplePreload.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:39:46.582293 ipyweb-1.0.8/ipyweb/preloads/thread/
+-rw-rw-rw-   0        0        0     3100 2024-06-01 15:02:53.000000 ipyweb-1.0.8/ipyweb/preloads/thread/crontabPreload.py
+-rw-rw-rw-   0        0        0     3327 2024-06-01 15:03:29.000000 ipyweb-1.0.8/ipyweb/preloads/thread/queuePreload.py
+-rw-rw-rw-   0        0        0     3596 2024-06-02 22:04:33.000000 ipyweb-1.0.8/ipyweb/preloads/thread/socketPreload.py
+-rw-rw-rw-   0        0        0     2437 2024-06-01 15:03:43.000000 ipyweb-1.0.8/ipyweb/preloads/thread/timerPreload.py
+-rw-rw-rw-   0        0        0    10967 2024-06-02 00:26:22.000000 ipyweb-1.0.8/ipyweb/process.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:39:46.586290 ipyweb-1.0.8/ipyweb/pywebview/
+-rw-rw-rw-   0        0        0     9257 2024-06-03 03:23:53.000000 ipyweb-1.0.8/ipyweb/pywebview/windows.py
+-rw-rw-rw-   0        0        0     4570 2024-06-01 00:28:38.000000 ipyweb-1.0.8/ipyweb/service.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:39:46.606291 ipyweb-1.0.8/ipyweb/services/
+-rw-rw-rw-   0        0        0     8143 2024-06-01 17:34:58.000000 ipyweb-1.0.8/ipyweb/services/crontab.py
+-rw-rw-rw-   0        0        0     8613 2024-06-02 01:54:38.000000 ipyweb-1.0.8/ipyweb/services/queue.py
+-rw-rw-rw-   0        0        0     2788 2024-06-02 23:42:58.000000 ipyweb-1.0.8/ipyweb/services/socketClient.py
+-rw-rw-rw-   0        0        0    18159 2024-06-02 23:22:17.000000 ipyweb-1.0.8/ipyweb/services/socketServer.py
+-rw-rw-rw-   0        0        0     3016 2024-06-01 17:28:09.000000 ipyweb-1.0.8/ipyweb/services/timer.py
+-rw-rw-rw-   0        0        0      470 2024-05-05 11:23:41.000000 ipyweb-1.0.8/ipyweb/singleton.py
+-rw-rw-rw-   0        0        0     5199 2024-06-02 00:27:10.000000 ipyweb-1.0.8/ipyweb/thread.py
+-rw-rw-rw-   0        0        0     4866 2024-06-03 03:37:14.000000 ipyweb-1.0.8/ipyweb/utils.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:39:46.610291 ipyweb-1.0.8/ipyweb/windowEvents/
+-rw-rw-rw-   0        0        0     2163 2024-05-31 14:32:07.000000 ipyweb-1.0.8/ipyweb/windowEvents/main.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:39:46.614289 ipyweb-1.0.8/ipyweb.egg-info/
+-rw-rw-rw-   0        0        0     2193 2024-06-03 10:39:46.000000 ipyweb-1.0.8/ipyweb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1969 2024-06-03 10:39:46.000000 ipyweb-1.0.8/ipyweb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 10:39:46.000000 ipyweb-1.0.8/ipyweb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-06-03 10:39:46.000000 ipyweb-1.0.8/ipyweb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       25 2024-06-03 10:39:46.000000 ipyweb-1.0.8/ipyweb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-06-03 10:39:46.000000 ipyweb-1.0.8/ipyweb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1209 2024-06-03 03:04:09.000000 ipyweb-1.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-03 10:39:46.619290 ipyweb-1.0.8/setup.cfg
```

### Comparing `ipyweb-1.0.7/LICENSE` & `ipyweb-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.7/PKG-INFO` & `ipyweb-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyweb
-Version: 1.0.7
+Version: 1.0.8
 Summary: A business framework for launching multiple services
 Author-email: sqwindows <sqwindows@qq.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2014-2017, Roman Sirokov
         All rights reserved.
```

### Comparing `ipyweb-1.0.7/ipyweb/addons/loadingGui.py` & `ipyweb-1.0.8/ipyweb/addons/loadingGui.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 import urllib.parse
+
+from ipyweb.config import config
 from ipyweb.logger import logger
 from ipyweb.singleton import singleton
 from ipyweb.utils import utils
 
 
 class loadingGui(metaclass=singleton):
 
     @classmethod
     def redirect(self, winCls=None, url=''):
         if winCls is None or winCls.windows == None or url == '':
             logger.console.error(f'An exception occurred while reloading the window parameters')
+        loadPageCfg = config.get('windows.localization.loadPage', {})
         try:
+
             domain, port = utils.getDomainPortByUrl(urllib.parse.quote(url, safe='/:?=&+'))
             if utils.checkUrl(domain, port) == True:
                 winCls.windows.load_url(url)
             else:
-                winCls.windows.load_html(self.html(f'网络异常无法加载请重试'))
+                winCls.windows.load_html(self.html(loadPageCfg.get('networkError', 'Network exception!')))
         except Exception as e:
-            winCls.windows.load_html(self.html(f'加载窗口地址异常请关闭重新打开再试'))
-            logger.console.error(f'An exception occurred while reloading the window url: {e}')
+            winCls.windows.load_html(self.html(loadPageCfg.get('loadError', 'Load exception!')))
+            logger.console.error(f'An exception occurred while loading the window url: {e}')
 
     @classmethod
     def load(self, winCls=None):
         try:
             if winCls:
-                winCls.setCreateParams({'html': self.html('正在加载中...')})
+                loadPageCfg = config.get('windows.localization.loadPage', {})
+                winCls.setCreateParams({'html': self.html(loadPageCfg.get('loading', 'loading...'))})
         except Exception as e:
             logger.console.error(f'An exception occurred while reading the login page: {e}')
 
     @classmethod
-    def html(self, message='正在加载中...'):
+    def html(self, message=''):
         return """<!DOCTYPE html><html lang="zh-CN"><head><meta charset="utf-8"><meta http-equiv="X-UA-Compatible" content="IE=edge"><meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=no, maximum-scale=1.0, minimum-scale=1.0" /><title></title>
  <style>html body{ overflow: hidden;}
       #loadingPage {background-color: #dedede;font-size: 12px;cursor: pointer;}
        #message{position: absolute;bottom:10px;width:100%;height:30px;line-height:30px;font-size:12px; text-align: center; color:#aaa; overflow: hidden;}
       .base {height: 9em;left: 50%;margin: -7.5em;padding: 3em;position: absolute;top: 50%; width: 9em;transform: rotateX(45deg) rotateZ(45deg);transform-style: preserve-3d;}
       .cube,
       .cube:after,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ipyweb-1.0.7/ipyweb/app.py` & `ipyweb-1.0.8/ipyweb/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 from pathlib import Path
 from ipyweb.singleton import singleton
 from ipyweb.utils import utils
 
 
 class app(metaclass=singleton):
-    ver = '1.0.3'
+    ver = '1.0.8'
     ipywebPath = 'ipyweb'
     appPath = 'app'
     rootPath = ''
     workRootPath = ''
     ipywebRootPath = ''
     appResourcesPath = ''
     exeResourcesPath = ''
@@ -25,14 +25,15 @@
     httpControllersName = 'httpControllers'
     eventsName = 'events'
     servicesName = 'services'
     preloadsName = 'preloads'
     commandsName = 'commands'
     socketsName = 'sockets'
     queuesName = 'queues'
+    crontabsName = 'crontabs'
     databasesName = 'databases'
     resourcesName = 'resources'
     ipywebAutoConfigName = 'ipywebAutoConfig'
     timersName = 'timers'
     windowEventsName = 'windowEvents'
     moduleJsonFileName = 'modules'
     bulidPathName = 'build'
```

### Comparing `ipyweb-1.0.7/ipyweb/appRunner.py` & `ipyweb-1.0.8/ipyweb/appRunner.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.7/ipyweb/builds/builder.py` & `ipyweb-1.0.8/ipyweb/builds/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     @classmethod
     def _isIncludeDirName(self):
         try:
             import PyInstaller
             version = PyInstaller.__version__
             match = re.search(r"^\d+\.\d+(\.\d+)?", version)
             if match.group(0) >= "6.0.0":
-                return '_' + self._name
+                return self._name
         except Exception as e:
             pass
 
         return ''
 
     @classmethod
     def getCmds(self):
```

### Comparing `ipyweb-1.0.7/ipyweb/builds/hooks/hook-cefpython3.py` & `ipyweb-1.0.8/ipyweb/builds/hooks/hook-cefpython3.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.7/ipyweb/cache.py` & `ipyweb-1.0.8/ipyweb/cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,14 +66,18 @@
                 logger.console.error(f'Unsupported database cache [{self._driver}]')
                 return self._diskcache
             if self._driver == 'diskcache':
                 from diskcache import Cache as DiskCache
                 self._diskcache = DiskCache(
                     app.path(f'{app.runtimePath}/{self._driverParams.get("path", self._config.get("path", ""))}'),
                     **self._driverParams)
+            else:
+                if self._driver:
+                    self._diskcache = self._driver
+
 
         except Exception as e:
             logger.console.error(f'An exception occurred while cache initialization ：{e}')
         return self._diskcache
 
     @classmethod
     def _setConfig(self, config={}):
```

### Comparing `ipyweb-1.0.7/ipyweb/command.py` & `ipyweb-1.0.8/ipyweb/command.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.7/ipyweb/commands/ipywebBuilder.py` & `ipyweb-1.0.8/ipyweb/commands/ipywebBuilder.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.7/ipyweb/commands/ipywebRunner.py` & `ipyweb-1.0.8/ipyweb/commands/ipywebRunner.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.7/ipyweb/config.py` & `ipyweb-1.0.8/ipyweb/config.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.7/ipyweb/configs/database.py` & `ipyweb-1.0.8/ipyweb/configs/database.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.7/ipyweb/configs/logger.py` & `ipyweb-1.0.8/ipyweb/configs/logger.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.7/ipyweb/configs/windows.py` & `ipyweb-1.0.8/ipyweb/configs/windows.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-title = '[ipyweb]一个快速启动多服务python业务框架'  # 窗口标题
+title = 'ipweb'  # 窗口标题
 debug = True  # 调试开关
 resizable = True  # 是否可以重设窗体尺寸
 text_select = False  # 文本是否可以选择
 confirm_close = False  # 退出是否弹出确认
 frameless = False  # 是否无边框
 easy_drag = False  # 无边框点窗体任意位置可拖动
 on_top = False  # 是否最上层
@@ -15,18 +15,24 @@
 background_color = '#FFFFFF'  # 背景颜色
 transparent = False  # 是否透明
 hidden = False  # 窗体打开后是否隐藏
 fullscreen = False  # 是否全屏
 private_mode = False  # 是否开启隐私模式 开启后缓存随着窗体关闭后销毁
 storage_path = 'cache'  # 浏览器引擎缓存目录 相对runtime目录下
 user_agent = None  # 浏览器请求头
+menu = []  # 菜单
 # 语言包
 localization = {
     'global': {
-        'quitConfirmation': '确定关闭吗？'
+        'quitConfirmation': 'Are you sure you want to quit?'
+    },
+    'loadPage': {
+        'loading': 'loading...',
+        'networkError': 'Network exception, unable to load. Please try again.',
+        'loadError': 'Unable to load. Please try again.'
     }
 }
 # gui设置为cef有效
 cef_settings = {
     'settings': {
         'locale': "zh-CN",
         'persist_session_cookies': True,
@@ -56,15 +62,15 @@
     'bottle': {
         'index_html': 'index.html',  # 首页文件 相对于resource目录
         'http_port': 8090,  # 端口
         'ssl': True,
     },
     'ipyweb': {
         'index_html': 'index.html',  # 首页文件 相对于resource目录
-        'http_port': 3456,  # 端口
+        'http_port': 8090,  # 端口
         'ssl': True,
     },
     'remote': {
         'loading': True,
         'url': 'https://saas.maoren.la/ipyweb',
         'http_server': False,  # 是否同时开启本地服务器
         'http_port': 8090,
```

### Comparing `ipyweb-1.0.7/ipyweb/contracts/ipywebController.py` & `ipyweb-1.0.8/ipyweb/contracts/ipywebController.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.7/ipyweb/contracts/ipywebHttpController.py` & `ipyweb-1.0.8/ipyweb/contracts/ipywebHttpController.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.7/ipyweb/controller.py` & `ipyweb-1.0.8/ipyweb/controller.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.7/ipyweb/controllers/ipyweb.py` & `ipyweb-1.0.8/ipyweb/controllers/ipyweb.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,200 +1,200 @@
 from ipyweb.app import app
 from ipyweb.singleton import singleton
 from ipyweb.contracts.ipywebController import ipywebController
 from ipyweb.pywebview.windows import windows
 
 
 class ipyweb(ipywebController, metaclass=singleton):
-    def version(self, window, *args):
+    def version(self, window, args):
         try:
 
-            return self.success('获取版本信息成功', {
+            return self.success('Version GET successful', {
                 'ver': app.ver,
                 'version': app.version
             })
         except Exception as e:
-            return self.error(f'获取版本信息异常:{e}')
+            return self.error(f'Version GET error:{e}')
 
     def create_window(self, window, args):
         try:
             if type(args) != dict:
-                return self.error('参数类型不正确')
+                return self.error('Parameter incorrect')
             args['target'] = True
             if args.get('url', '') == '' and args.get('html', '') == '':
-                return self.error('html和url必须设置一个')
+                return self.error('Parameter[html or url] must be set')
             flag = windows().run(args)
             if type(flag) == str:
                 return self.error(flag)
-            return self.success('打开成功')
+            return self.success('Window create successful')
         except Exception as e:
-            return self.error(f'获取版本信息异常:{e}')
+            return self.error(f'Window create error:{e}')
 
     def set_title(self, window, args):
         try:
             if type(args) == str:
                 title = args
             elif type(args) == dict:
                 title = args.get('title', '')
             else:
-                return self.error('标题不能为空')
+                return self.error('Parameter[title] must be set')
             window.set_title(title)
-            return self.success('更换窗口标题成功')
+            return self.success('Title set successfully')
         except Exception as e:
-            return self.error(f'更换窗口标题异常:{e}')
+            return self.error(f'Title set error:{e}')
 
     def change_url(self, window, args):
         try:
             if type(args) == str:
                 url = args
             elif type(args) == dict:
                 url = args.get('url', '')
             else:
-                return self.error('网址不能为空')
+                return self.error('Parameter[url] must be set')
             window.load_url(url)
-            return self.success('打开网址成功')
+            return self.success('Url change successfully')
         except Exception as e:
-            return self.error(f'打开网址异常:{e}')
+            return self.error(f'Url change Error:{e}')
 
     def load_css(self, window, args):
         try:
             if type(args) == str:
                 css = args
             elif type(args) == dict:
                 css = args.get('css', '')
             else:
-                return self.error('css不能为空')
+                return self.error('Parameter[css] must be set')
             window.load_css(css)
-            return self.success('加载css成功')
+            return self.success('Css load successfully')
         except Exception as e:
-            return self.error(f'加载css异常:{e}')
+            return self.error(f'Css load error:{e}')
 
     def load_html(self, window, args):
         try:
             if type(args) == str:
                 html = args
             elif type(args) == dict:
                 html = args.get('html', '')
             else:
-                return self.error('html不能为空')
+                return self.error('Parameter[html] must be set')
             window.load_html(html)
-            return self.success('加载html成功')
+            return self.success('Html load successfully')
         except Exception as e:
-            return self.error(f'加载html异常:{e}')
+            return self.error(f'Html load error:{e}')
 
     def evaluate_js(self, window, args):
         try:
             if type(args) == str:
                 js = args
             elif type(args) == dict:
                 js = args.get('js', '')
             else:
-                return self.error('js不能为空')
+                return self.error('Parameter[js] must be set')
             window.evaluate_js(js)
-            return self.success('执行js成功')
+            return self.success('Js evaluate successfully')
         except Exception as e:
-            return self.error(f'执行js异常:{e}')
+            return self.error(f'Js evaluate error:{e}')
 
-    def destroy(self, window, *args):
+    def destroy(self, window, args):
         try:
             window.destroy()
-            return self.success('窗体销毁成功')
+            return self.success('Window destroy successfully')
         except Exception as e:
-            return self.error(f'窗口销毁异常:{e}')
+            return self.error(f'Window destroy error:{e}')
 
-    def hide(self, window, *args):
+    def hide(self, window, args):
         try:
             window.hide()
-            return self.success('窗体隐藏成功')
+            return self.success('Window hide successfully')
         except Exception as e:
-            return self.error(f'窗口隐藏异常:{e}')
+            return self.error(f'Window hide error:{e}')
 
-    def show(self, window, *args):
+    def show(self, window, args):
         try:
             window.show()
-            return self.success('窗体显示成功')
+            return self.success('Window show successfully')
         except Exception as e:
-            return self.error(f'窗口显示异常:{e}')
+            return self.error(f'Window show error:{e}')
 
-    def minimize(self, window, *args):
+    def minimize(self, window, args):
         try:
             window.restore()
             window.minimize()
-            return self.success('窗体最小化成功')
+            return self.success('Window minimize successfully')
         except Exception as e:
-            return self.error(f'窗口最小化异常:{e}')
+            return self.error(f'Window minimize error:{e}')
 
-    def screens(self, window, *args):
+    def screens(self, window, args):
         try:
             import webview
             screens = webview.screens
             width, height = screens[0].width, screens[0].height
-            return self.success('获取屏幕信息', {'width': width, 'height': height})
+            return self.success('Screens GET successfully', {'width': width, 'height': height})
         except Exception as e:
-            return self.error(f'获取屏幕信息异常:{e}')
+            return self.error(f'Screens GET error:{e}')
 
-    def toggle_fullscreen(self, window, *args):
+    def toggle_fullscreen(self, window, args):
         try:
             window.toggle_fullscreen()
-            return self.success('切换全屏成功')
+            return self.success('Fullscreen toggle successfully')
         except Exception as e:
-            return self.error(f'切换全屏异常:{e}')
+            return self.error(f'Fullscreen toggle error:{e}')
 
-    def move(self, window, args=None):
+    def move(self, window, args):
         try:
             if type(args) == dict:
                 x = args.get('x', 0)
                 y = args.get('y', 0)
             else:
-                return self.error('xy坐标不能为空')
+                return self.error('Parameter[x and y] must be set')
             window.move(x, y)
-            return self.success('窗口移动成功')
+            return self.success('Window move successfully')
         except Exception as e:
-            return self.error(f'窗口移动异常:{e}')
+            return self.error(f'Window move error:{e}')
 
-    def resize(self, window, args=None):
+    def resize(self, window, args):
         try:
             if type(args) == dict:
                 width = args.get('width', 0)
                 height = args.get('height', 0)
             else:
-                return self.error('宽高坐标不能为空')
+                return self.error('Parameter[width and height] must be set')
             window.resize(width, height)
-            return self.success('窗口大小设置成功')
+            return self.success('Window resize successfully')
         except Exception as e:
-            return self.error(f'窗口大小设置异常:{e}')
+            return self.error(f'Window resize error:{e}')
 
-    def open_file_dialog(self, window, args=None):
+    def open_file_dialog(self, window, args):
         try:
             import webview
             if type(args) != dict:
-                return self.error('打开目录窗口参数异常')
+                return self.error('Parameter incorrect')
             file_type = args.get('file_type', 'Image Files (*.bmp;*.jpg;*.gif)')
             file_types = (file_type, 'All files (*.*)')
             allow_multiple = args.get('allow_multiple', True)
             files = window.create_file_dialog(
                 dialog_type=webview.OPEN_DIALOG,
                 allow_multiple=allow_multiple,
                 file_types=file_types
             )
 
-            return self.success('打开目录窗口获取文件成功', {files: files})
+            return self.success('open_file_dialog successfully', {files: files})
         except Exception as e:
-            return self.error(f'打开目录窗口异常:{e}')
+            return self.error(f'open_file_dialog error:{e}')
 
-    def save_file_dialog(self, window, args=None):
+    def save_file_dialog(self, window, args):
         try:
             import webview
             if type(args) != dict:
                 return self.error('保存文件参数异常')
             directory = args.get('directory', '/')
             filename = args.get('filename', 'file')
             allow_multiple = args.get('allow_multiple', False)
             files = window.create_file_dialog(
                 dialog_type=webview.SAVE_DIALOG,
                 directory=directory,
                 allow_multiple=allow_multiple,
                 save_filename=filename
             )
-            return self.success('保存文件成功', {files: files})
+            return self.success('save_file_dialog successfully', {files: files})
         except Exception as e:
-            return self.error(f'保存文件异常:{e}')
+            return self.error(f'save_file_dialog error:{e}')
```

### Comparing `ipyweb-1.0.7/ipyweb/db.py` & `ipyweb-1.0.8/ipyweb/db.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,17 +65,20 @@
 
             if self._driver == 'mysql':
                 from playhouse.pool import PooledMySQLDatabase
                 self._database = PooledMySQLDatabase(**self._driverParams)
             elif self._driver == 'postgresql':
                 from playhouse.pool import PostgresqlDatabase
                 self._database = PostgresqlDatabase(**self._driverParams)
-            else:
+            elif self._driver == 'sqlite':
                 from peewee import SqliteDatabase
                 self._database = SqliteDatabase(**self._driverParams)
+            else:
+                if self._driver:
+                    self._database = self._driver
         except Exception as e:
             logger.console.error(f'An exception occurred while database initialization ：{e}')
         return self._database
 
     def _setConfig(self, config={}):
         try:
             self._config = dict(self._config, **sysConfig.get('database', {}))
```

### Comparing `ipyweb-1.0.7/ipyweb/event.py` & `ipyweb-1.0.8/ipyweb/event.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.7/ipyweb/gui.py` & `ipyweb-1.0.8/ipyweb/gui.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from ipyweb.app import appIpyweb
 from ipyweb.config import config, configIpyweb
 from ipyweb.logger import loggerIpyweb
 from ipyweb.singleton import singleton
+from ipyweb.utils import utils
 
 
 class gui:
     guiDriver = None
 
 
 class guiIpyweb(metaclass=singleton):
@@ -17,26 +18,30 @@
         if appIpyweb._loaded == False: appIpyweb.load()
         if loggerIpyweb._loaded == False: loggerIpyweb.load()
         if configIpyweb._loaded == False: configIpyweb.load()
 
         if config.get('windows.guiDriverEnable', True) == False and reload == False:
             return None
         if self._loaded == False or reload == True:
-            guiDriver = config.get('windows.guiDriver', '')
+            guiDriver = config.get('windows.guiDriver', None)
             guiConfig = config.get(f'windows.guiDriverConfig.{guiDriver}', {})
             if guiDriver == 'remote':
                 from ipyweb.guis.RemoteServer import RemoteServer
                 self._guiDriver = RemoteServer(guiConfig).run()
             elif guiDriver == 'local':
                 from ipyweb.guis.LocalServer import LocalServer
                 self._guiDriver = LocalServer(guiConfig).run()
             elif guiDriver == 'flask':
                 from ipyweb.guis.FlaskServer import FlaskServer
                 self._guiDriver = FlaskServer(guiConfig).run()
             elif guiDriver == 'ipyweb':
                 from ipyweb.guis.IpywebServer import IpywebServer
                 self._guiDriver = IpywebServer(guiConfig).run()
-            else:
+            elif guiDriver == 'bottle':
                 from ipyweb.guis.BottleServer import BottleServer
                 self._guiDriver = BottleServer(guiConfig).run()
+            else:
+
+                if guiDriver and hasattr(guiDriver, 'run'):
+                    self._guiDriver = guiDriver.run()
 
         return self._guiDriver
```

### Comparing `ipyweb-1.0.7/ipyweb/guis/BottleServer.py` & `ipyweb-1.0.8/ipyweb/guis/BottleServer.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 class BottleServer:
     _config = {}
 
     def __init__(self, httpConfig={}):
         self._config = dict(self._config, **httpConfig)
 
     def run(self):
-
         event.on('windows_createBefore', self._onWindowsCreateBefore)
         event.on('windows_startBefore', self._onWindowsStartBefore)
 
     def _onWindowsCreateBefore(self, winCls, **kwargs):
         if kwargs.get('name', '') == 'main':
             winCls.setCreateParams({
                 'url': str(app.path(app.realResourcesPath + '/' + self._config.get('index_html', 'index.html'))),
```

### Comparing `ipyweb-1.0.7/ipyweb/guis/FlaskServer.py` & `ipyweb-1.0.8/ipyweb/guis/FlaskServer.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.7/ipyweb/guis/IpywebServer.py` & `ipyweb-1.0.8/ipyweb/guis/IpywebServer.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.7/ipyweb/guis/LocalServer.py` & `ipyweb-1.0.8/ipyweb/guis/LocalServer.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.7/ipyweb/guis/RemoteServer.py` & `ipyweb-1.0.8/ipyweb/guis/RemoteServer.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.7/ipyweb/ipyweb.py` & `ipyweb-1.0.8/ipyweb/ipyweb.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import time
 from ipyweb.app import app, appIpyweb
-from ipyweb.config import configIpyweb
+from ipyweb.config import config, configIpyweb
 from ipyweb.logger import logger
 from ipyweb.logger import loggerIpyweb
 from ipyweb.module import moduleIpyweb
 from ipyweb.preload import preloadIpyweb
 from ipyweb.event import eventIpyweb
 from ipyweb.appRunner import appRunner
 
@@ -104,18 +104,20 @@
     def bootAppRunner(self):
         self.bootTime['bootAppStart'] = time.time()
 
         def onWindowsOpened(appName):
             self.bootTime['bootAppEnd'] = time.time()
             self.bootTime['bootAppRun'] = self.bootTime['bootAppEnd'] - self.bootTime['bootAppStart']
             self.bootTime['totalTime'] = self.bootTime['ipywebRun'] + self.bootTime['bootAppRun']
+            preloadIpyweb.load().run(False)  # 窗口打开后启动预载器
             logger.console.error(
-                f'The time taken for loading basic:{round(self.bootTime["ipywebBoots"]["bootBaserRun"], 3)}s,'
-                f'The time taken for loading preload  (including application preload):{round(self.bootTime["ipywebBoots"]["bootPreloaderRun"], 3)}s,'
-                f'The time taken for windows:{round(self.bootTime["bootAppRun"], 3)}s')
+                f'basic[{round(self.bootTime["ipywebBoots"]["bootBaserRun"], 3)}s] '
+                f'preload[{round(self.bootTime["ipywebBoots"]["bootPreloaderRun"], 3)}s] '
+                f'window[{round(self.bootTime["bootAppRun"], 3)}s] ')
+
             if callable(self.onOpened): self.onOpened()
 
         appRunner.setOnWindowsOpened(onWindowsOpened).boot()
         return self
 
     @classmethod  # 应用启动回调生命周期事件
     def getAppRunerOnEvent(self):
@@ -138,15 +140,15 @@
         self.bootTime['ipywebBoots']['bootBaserRun'] = self.bootTime['ipywebBoots']['bootBaserEnd'] - \
                                                        self.bootTime['ipywebBoots']['bootBaserStart']
         return self
 
     @classmethod  # 启动预载模块
     def bootPreloader(self):
         self.bootTime['ipywebBoots']['bootPreloaderStart'] = time.time()
-        preloadIpyweb.load()
+        preloadIpyweb.load().run(True)
         self.bootTime['ipywebBoots']['bootPreloaderEnd'] = time.time()
         self.bootTime['ipywebBoots']['bootPreloaderRun'] = self.bootTime['ipywebBoots']['bootPreloaderEnd'] - \
                                                            self.bootTime['ipywebBoots']['bootPreloaderStart']
         return self
 
     @classmethod
     def setOnStart(self, onStart=None):
```

### Comparing `ipyweb-1.0.7/ipyweb/jsonFile.py` & `ipyweb-1.0.8/ipyweb/jsonFile.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.7/ipyweb/logger.py` & `ipyweb-1.0.8/ipyweb/logger.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.7/ipyweb/module.py` & `ipyweb-1.0.8/ipyweb/module.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,15 @@
         f'{app.eventsName}/listener',
         f'{app.preloadsName}/block',
         f'{app.preloadsName}/process',
         f'{app.preloadsName}/thread',
         f'{app.servicesName}',
         f'{app.socketsName}',
         f'{app.queuesName}',
+        f'{app.crontabsName}',
         f'{app.timersName}',
         f'{app.windowEventsName}',
     ]
     _maps = {
         'name': app.getName(),
         'app': {},
         'ipyweb': {},
```

### Comparing `ipyweb-1.0.7/ipyweb/preload.py` & `ipyweb-1.0.8/ipyweb/preload.py`

 * *Files 23% similar despite different names*

```diff
@@ -20,50 +20,55 @@
     @classmethod
     def getProcess(self, name=''):
         return preloadIpyweb.processes.get(name, None) if name else preloadIpyweb.processes
 
 
 class preloadIpyweb(metaclass=singleton):
     _loaded = False
+    _runAtBoot = ''
     ipyweb = None
     blocks = {}
     threads = {}
     processes = {}
     preloadBlocks = {}
     preloadThreads = {}
     preloadProcesss = {}
 
     @classmethod
     def load(self, reload=False):
 
         if self._loaded == True and reload == True:
             return self
-
         if appIpyweb._loaded == False: appIpyweb.load()
         if loggerIpyweb._loaded == False: loggerIpyweb.load()
         if configIpyweb._loaded == False: configIpyweb.load()
 
         self._loadFromPreloadBlocks(f'{app.ipywebPath}.{app.preloadsName}/block')
         self._loadFromPreloadThreads(f'{app.ipywebPath}.{app.preloadsName}/thread')
         self._loadFromPreloadProcess(f'{app.ipywebPath}.{app.preloadsName}/process')
 
         if config.get('app.autoLoad.loadPrelodsEnable', True):
             self._loadFromPreloadBlocks(f'{app.appPath}.{app.preloadsName}/block')
             self._loadFromPreloadThreads(f'{app.appPath}.{app.preloadsName}/thread')
             self._loadFromPreloadProcess(f'{app.appPath}.{app.preloadsName}/process')
+        self._loaded = True
+        if app.lifecycleDebug:
+            print('::::::::::::::::::::::::::preload loaded::::::::::::::::::::::::::')
+
+        return self
+
+    @classmethod
+    def run(self, runAtBoot=True):
+        self._runAtBoot = runAtBoot
         for name, module in self.preloadBlocks.items():
             self._runBlock(name, module)
         for name, module in self.preloadThreads.items():
             self._runThread(name, module)
         for name, module in self.preloadProcesss.items():
             self._runProcess(name, module)
-        if app.lifecycleDebug:
-            print('::::::::::::::::::::::::::preload loaded::::::::::::::::::::::::::')
-        self._loaded = True
-
         return self
 
     @classmethod
     def reload(self):
         self.load(True)
         return self
 
@@ -94,19 +99,24 @@
             for name, module in modules.items():
                 self.preloadProcesss[name] = module
         except Exception as e:
             logger.console.error(f'An exception occurred while parsing the process preloader:{e}')
         return self
 
     @classmethod
+    def _checkIsRun(self, windowsOpen):
+        return (self._runAtBoot == True and windowsOpen == False) or (self._runAtBoot == False and windowsOpen == True)
+
+    @classmethod
     def _runBlock(self, name='', module=None):
         try:
             moduleConfig = getattr(module, app.ipywebAutoConfigName, {})
             if moduleConfig.get('enable', False) != True:
                 return self
+
             if hasattr(module, 'run'):
                 self.blocks[name] = module.run
                 module.run()
         except Exception as e:
             logger.console.error(f'[{name}]An exception occurred while executing the blocking preloader:{e}')
         return self
 
@@ -114,39 +124,31 @@
     def _runThread(self, name='', module=None):
         try:
             if self.threads.get(name, None) is None:
                 moduleConfig = getattr(module, app.ipywebAutoConfigName, {})
                 usePool = moduleConfig.get('usePool', False)
                 if moduleConfig.get('enable', False) != True:
                     return self
+                isRun = self._checkIsRun(moduleConfig.get('windowsOpen', False))
+                if isRun != True:
+                    return self
                 threadName = moduleConfig.get('name', '')
                 threadName = threadName if threadName else module.__module__
-                if usePool == True:
-                    self.threads[name] = thread.runPool(
-                        name=threadName,
-                        target=module.run if hasattr(module, 'run') else None,
-                        onStart=module.onStart if hasattr(module, 'onStart') else None,
-                        onError=module.onError if hasattr(module, 'onError') else None,
-                        config={
-                            'max': moduleConfig.get('max', 1),
-                            'daemon': moduleConfig.get('daemon', True),
-                            'block': moduleConfig.get('block', False),
-                        })
-                else:
-                    self.threads[name] = thread.run(
-                        name=threadName,
-                        target=module.run if hasattr(module, 'run') else None,
-                        onStart=module.onStart if hasattr(module, 'onStart') else None,
-                        onError=module.onError if hasattr(module, 'onError') else None,
-                        config={
-                            'max': moduleConfig.get('max', 1),
-                            'daemon': moduleConfig.get('daemon', True),
-                            'block': moduleConfig.get('block', False),
-                        })
-
+                threadConfig = {
+                    'name': threadName,
+                    'target': module.run if hasattr(module, 'run') else None,
+                    'onStart': module.onStart if hasattr(module, 'onStart') else None,
+                    'onError': module.onError if hasattr(module, 'onError') else None,
+                    'config': {
+                        'max': moduleConfig.get('max', 1),
+                        'daemon': moduleConfig.get('daemon', True),
+                        'block': moduleConfig.get('block', False),
+                    }
+                }
+                self.threads[name] = thread.runPool(**threadConfig) if usePool == True else thread.run(**threadConfig)
         except Exception as e:
             logger.console.error(f'An exception occurred while executing the thread preloader:{e}')
         return self
 
     @classmethod
     def _runProcess(self, name='', module=None):
 
@@ -155,42 +157,29 @@
                 moduleConfig = getattr(module, app.ipywebAutoConfigName, {})
                 usePool = moduleConfig.get('usePool', False)
 
                 if moduleConfig.get('enable', False) != True:
                     return self
                 processName = moduleConfig.get('name', '')
                 processName = processName if processName else module.__module__
-                if usePool == True:
-                    self.processes[name] = process.runPool(
-                        name=processName,
-                        target=module.run,
-                        onStart=module.onStart if hasattr(module, 'onStart') else None,
-                        onError=module.onError if hasattr(module, 'onError') else None,
-                        onMessage=module.onMessage if hasattr(module, 'onMessage') else None,
-                        onIpc=module.onIpc if hasattr(module, 'onIpc') else None,
-                        onShare=module.onShare if hasattr(module, 'onShare') else None,
-                        config={
-                            'max': moduleConfig.get('max', 1),
-                            'daemon': moduleConfig.get('daemon', True),
-                            'block': moduleConfig.get('block', False),
-                            'reloadIpyweb': moduleConfig.get('reloadIpyweb', True),
-                        })
-                else:
-
-                    self.processes[name] = process.run(
-                        name=processName,
-                        target=module.run,
-                        onStart=module.onStart if hasattr(module, 'onStart') else None,
-                        onError=module.onError if hasattr(module, 'onError') else None,
-                        onMessage=module.onMessage if hasattr(module, 'onMessage') else None,
-                        onIpc=module.onIpc if hasattr(module, 'onIpc') else None,
-                        onShare=module.onShare if hasattr(module, 'onShare') else None,
-                        config={
-                            'max': moduleConfig.get('max', 1),
-                            'daemon': moduleConfig.get('daemon', True),
-                            'block': moduleConfig.get('block', False),
-                            'reloadIpyweb': moduleConfig.get('reloadIpyweb', True),
-                        })
+                processConfig = {
+                    'name': processName,
+                    'target': module.run,
+                    'onStart': module.onStart if hasattr(module, 'onStart') else None,
+                    'onError': module.onError if hasattr(module, 'onError') else None,
+                    'onMessage': module.onMessage if hasattr(module, 'onMessage') else None,
+                    'onIpc': module.onIpc if hasattr(module, 'onIpc') else None,
+                    'onShare': module.onShare if hasattr(module, 'onShare') else None,
+                    'config': {
+                        'max': moduleConfig.get('max', 1),
+                        'daemon': moduleConfig.get('daemon', True),
+                        'block': moduleConfig.get('block', False),
+                        'reloadIpyweb': moduleConfig.get('reloadIpyweb', True),
+                    }
+                }
+                self.processes[name] = process.runPool(**processConfig) if usePool == True else process.run(
+                    **processConfig)
+
 
         except Exception as e:
             logger.console.error(f'An exception occurred while executing the process preloader:{e}')
         return self
```

### Comparing `ipyweb-1.0.7/ipyweb/preloads/block/controllerPreload.py` & `ipyweb-1.0.8/ipyweb/preloads/block/controllerPreload.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.7/ipyweb/preloads/thread/queuePreload.py` & `ipyweb-1.0.8/ipyweb/preloads/thread/timerPreload.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,66 +1,60 @@
 from ipyweb.app import app
 from ipyweb.config import config
+from ipyweb.contracts.ipywebPreload import ipywebPreload
 from ipyweb.logger import logger
 from ipyweb.service import service
-from ipyweb.contracts.ipywebPreload import ipywebPreload
-from ipyweb.services.queue import queue, queueRunner
+from ipyweb.services.timer import timer
 
 
-class queuePreload(ipywebPreload):
-    # preload加载此模块时调用的配置信息
+class timerPreload(ipywebPreload):
+    timers = {}
     ipywebAutoConfig = {
         'enable': True,  # 是否关闭运行
-        'daemon': True,  # 是否守护执行
-        'block': False,  # 是否阻塞执行
-        'max': 1,  # 进程池或线程池数量
-        'usePool': False,  # 是否线程池
+        # 启动节点 True:窗口打开后 False:窗口打开前 默认 False
+        'windowsOpen': config.get('app.preload.timerPreloadAtWindowsOpen', False),
+        'daemon': True,  # 是否守护执行 默认True
+        'block': False,  # 是否阻塞执行 默认False
+        'max': 1,  # 进程池或线程池数量 默认1
+        'usePool': False,  # 是否线程池 默认False
     }
-    queues = {}
 
-    def run(self, **kwargs):
+    def run(self, **config):
         self.load()
-        return self
 
     def load(self):
-        self._loadFromQueques(f'{app.ipywebPath}.{app.queuesName}')
-        if config.get('app.autoLoad.loadQuequesEnable', False) == True:
-            self._loadFromQueques(f'{app.appPath}.{app.queuesName}')
+        self._loadFromTimesDir(f'{app.ipywebPath}.{app.timersName}')
+        if config.get('app.autoLoad.loadTimersEnable', False) == True:
+            self._loadFromTimesDir(f'{app.appPath}.{app.timersName}')
         try:
-            for name, module in self.queues.items():
+
+            for name, module in self.timers.items():
                 moduleConfig = getattr(module, app.ipywebAutoConfigName, {})
-                if moduleConfig.get('enable', False) == True: self.quequeRun(name, moduleConfig, module)
+                if moduleConfig.get('enable', False) == True: self.timerRun(name, moduleConfig, module)
         except Exception as e:
-            logger.console.error(f'An exception occurred while reading the queue dirs:{e}')
+            logger.console.error(f'An exception occurred while reading the timer dirs:{e}')
         return self
 
-    def _loadFromQueques(self, path=''):
+    def _loadFromTimesDir(self, dirs=''):
+
         try:
-            modules = service.module(path)
+            modules = service.module(dirs)
+
             for name, module in modules.items():
-                self.queues[name] = module
+                self.timers[name] = module
         except Exception as e:
-            logger.console.error(f'An exception occurred while reading the queue module:{e}')
+            logger.console.error(f'An exception occurred while reading the timer module:{e}')
         return self
 
-    def quequeRun(self, name='', moduleConfig={}, quequeModule=None):
+    def timerRun(self, name, moduleConfig, module):
         try:
-            config = dict(moduleConfig, **{
-                'name': quequeModule.__module__,
-                'run': moduleConfig.get('run', quequeModule.run if hasattr(quequeModule, 'run') else None),
-                'onStart': moduleConfig.get('onStart',
-                                            quequeModule.onStart if hasattr(quequeModule, 'onStart') else None),
-                'onRecv': moduleConfig.get(
-                    'onRecv',
-                    quequeModule.onRecv if hasattr(quequeModule, 'onRecv') else None),
-
-                'onEmpty': moduleConfig.get('onEmpty',
-                                            quequeModule.onEmpty if hasattr(quequeModule, 'onEmpty') else None),
-                'onFull': moduleConfig.get('onFull', quequeModule.onFull if hasattr(quequeModule, 'onFull') else None),
-                'onError': moduleConfig.get('onError',
-                                            quequeModule.onError if hasattr(quequeModule, 'onError') else None),
-            })
+            moduleConfig['name'] = moduleConfig.get('name', module.__module__)
+            moduleConfig['event'] = {
+                'run': module.run if hasattr(module, 'run') else None,
+                'onStart': module.onStart if hasattr(module, 'onStart') else None,
+                'onError': module.onError if hasattr(module, 'onError') else None
+            }
 
-            queueRunner().run(**config)
+            timer().run(**moduleConfig)
         except Exception as e:
-            logger.console.error(f'An exception occurred while starting the queue module [{name}]:{e}')
+            logger.console.error(f'An exception occurred while starting the timer module :{e}')
         return self
```

### Comparing `ipyweb-1.0.7/ipyweb/preloads/thread/socketPreload.py` & `ipyweb-1.0.8/ipyweb/preloads/thread/socketPreload.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,18 +6,20 @@
 from ipyweb.contracts.ipywebPreload import ipywebPreload
 
 
 class socketPreload(ipywebPreload):
     # preload加载此模块时调用的配置信息
     ipywebAutoConfig = {
         'enable': True,  # 是否关闭运行
-        'daemon': True,  # 是否守护执行
-        'block': False,  # 是否阻塞执行
-        'max': 1,  # 进程池或线程池数量
-        'usePool': False,  # 是否线程池
+        # 启动节点 True:窗口打开后 False:窗口打开前 默认 False
+        'windowsOpen': config.get('app.preload.socketPreloadAtWindowsOpen', False),
+        'daemon': True,  # 是否守护执行 默认True
+        'block': False,  # 是否阻塞执行 默认False
+        'max': 1,  # 进程池或线程池数量 默认1
+        'usePool': False,  # 是否线程池 默认False
     }
     sockets = {}
 
     def run(self, **kwargs):
         self.load()
         return self
 
@@ -42,22 +44,28 @@
             logger.console.error(f'An exception occurred while reading the socket module:{e}')
         return self
 
     def socketRun(self, module=None, moduleConfig={}, socketServe=None):
         try:
             config = dict(moduleConfig, **{
                 'name': module.__module__,
-                'onReady': moduleConfig.get('onReady',
-                                            socketServe.onReady if hasattr(socketServe, 'onReady') else None),
-                'onConnect': moduleConfig.get('onConnect',
-                                              socketServe.onConnect if hasattr(socketServe, 'onConnect') else None),
-                'onError': moduleConfig.get('onError',
-                                            socketServe.onError if hasattr(socketServe, 'onError') else None),
-                'onClosed': moduleConfig.get('onClosed',
-                                             socketServe.onClosed if hasattr(socketServe, 'onClosed') else None),
-                'onMessage': moduleConfig.get('onMessage',
-                                              socketServe.onMessage if hasattr(socketServe, 'onMessage') else None),
+                'event': {
+                    'onStart': moduleConfig.get('onStart',
+                                                socketServe.onStart if hasattr(socketServe, 'onStart') else None),
+                    'onStop': moduleConfig.get('onStop',
+                                               socketServe.onStop if hasattr(socketServe, 'onStop') else None),
+                    'onServe': moduleConfig.get('onServe',
+                                                 socketServe.onServe if hasattr(socketServe, 'onServe') else None),
+                    'onConnect': moduleConfig.get('onConnect',
+                                                  socketServe.onConnect if hasattr(socketServe, 'onConnect') else None),
+                    'onError': moduleConfig.get('onError',
+                                                socketServe.onError if hasattr(socketServe, 'onError') else None),
+                    'onClosed': moduleConfig.get('onClosed',
+                                                 socketServe.onClosed if hasattr(socketServe, 'onClosed') else None),
+                    'onMessage': moduleConfig.get('onMessage',
+                                                  socketServe.onMessage if hasattr(socketServe, 'onMessage') else None),
+                }
             })
             socketServerRunner().run(**config)
         except Exception as e:
             logger.console.error(f'An exception occurred while starting the socket module :{e}')
         return self
```

### Comparing `ipyweb-1.0.7/ipyweb/process.py` & `ipyweb-1.0.8/ipyweb/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,14 +215,16 @@
                         )
                         # pool.close()
                         # pool.join()
                     self.processes[name]['pid'] = 0
                     if callable(onStart): onStart(self.processes[name]['pool'])
 
             return self.processes[name]['pool']
+        except KeyboardInterrupt:
+            pass
         except pickle.PicklingError as e:
             msg = f'A serialization error occurred while starting the [{name}] process pool.'
             logger.console.error(msg)
             if callable(onError): onError(msg, e)
         except Exception as e:
             msg = f'An exception occurred while starting with the [{name}] process pool:{e}'
             logger.console.error(msg)
@@ -269,15 +271,16 @@
                     self.processes[name]['process'].start()
                     if config.get('block', False):  # 是否阻塞
                         self.processes[name]['process'].join()
                     self.processes[name]['pid'] = self.processes[name]['process'].pid
                     if callable(onStart): onStart(self.processes[name]['process'])
             return self.processes[name]['process']
 
-
+        except KeyboardInterrupt:
+            pass
         except pickle.PicklingError as e:
             msg = f'A serialization error occurred while starting the [{name}] process.'
             logger.console.error(msg)
             if callable(onError): onError(msg, e)
         except Exception as e:
             msg = f'An exception occurred while starting with the [{name}] process:{e}'
             logger.console.error(msg)
```

### Comparing `ipyweb-1.0.7/ipyweb/pywebview/windows.py` & `ipyweb-1.0.8/ipyweb/pywebview/windows.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,15 @@
             except ImportError:
                 logger.console.error(
                     'please installer the module: pycairo and pygobject (pip install pycairo pygobject)')
                 return False
         return True
 
     def _run(self):
+
         if self._checkGui() == False:
             return 'guiDriver module ImportError'
 
         self._parseParams()
         _checkParams = self._checkParams()
         if _checkParams != True and type(_checkParams) == str:
             return _checkParams
@@ -133,14 +134,15 @@
                 'func': self._onStartedCallable,
                 'args': self,
                 'storage_path': os.path.normpath(f'{app.runtimePath}/{str(self._params.get("storage_path", "cache"))}'),
             })
             if callable(self._onStartBefore): self._onStartBefore(self)
             event.emit('windows_startBefore', self, name=self.name, windows=self.windows)
             self._startParams = {k: v for k, v in self._startParams.items() if k in self._supportStartsParams}
+
             if self._tartget.get('enable', False):
                 self._startParams = dict(self._startParams, **{
                     "http_server": False,
                 })
             webview.start(**self._startParams)  # 启动窗口
 
         except Exception as e:
@@ -169,16 +171,15 @@
                 'http_server': False
             }
         self._createParams = {k: v for k, v in self._params.items() if k in self._supportWindowsParams}
 
         return self
 
     def _setParams(self, params={}):
-        self._params = config.get('windows', {})
-        self._params = dict(self._params, **params)
+        self._params = dict(self._params, **config.get('windows', {}))
         self.name = self._params.get('name', 'main')
         return self
 
     def _checkParams(self) -> bool or str:
         try:
             if self.name == '' or (self._tartget.get('enable', False) and self.name == 'main'):
                 return f'The window name must be unique '
```

### Comparing `ipyweb-1.0.7/ipyweb/service.py` & `ipyweb-1.0.8/ipyweb/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import importlib
 from ipyweb.app import app
 from ipyweb.utils import utils
 from ipyweb.logger import logger
 from ipyweb.singleton import singleton
 from ipyweb.module import module as moduleMap
```

### Comparing `ipyweb-1.0.7/ipyweb/services/queue.py` & `ipyweb-1.0.8/ipyweb/services/queue.py`

 * *Files 16% similar despite different names*

```diff
@@ -42,22 +42,26 @@
     def remove(self, name=''):
         return self.queueIpyweb._remove(name)
 
 
 class queueIpyweb():
     _name = 'default'
     _config = {}
+    _event = {}
+    _setting = {}
     _queue = None
     _thread = None
     _userQueue = None
     _runnding = True
 
     def run(self, config={}, userQueue=None):
         self._userQueue = userQueue
         self._config = dict(self._config, **config)
+        self._setting = dict(self._setting, **self._config.get('setting', {}))
+        self._event = dict(self._event, **self._config.get('event', {}))
         self._name = self._config.get('name', __name__)
         self._setQueue()
         return self
 
     def stop(self):
         self._runnding = False
         return self
@@ -72,92 +76,88 @@
                 if name and taskTuple[0] != name:
                     newItems.append(taskTuple)
                 else:
                     count += 1
             for taskTuple in newItems:
                 queue.put(
                     (taskTuple[0], taskTuple[1]),
-                    block=self._config.get('putBlock', False),
-                    timeout=self._config.get('putTimeout', None)
+                    block=self._setting.get('putBlock', False),
+                    timeout=self._setting.get('putTimeout', None)
                 )
         except pyqueue.Full:
-            onFull = self._config.get('onFull', None)
+            onFull = self._event.get('onFull', self._config.get('onFull', None))
             if callable(onFull): onFull()
         except Exception as e:
             msg = f"An exception occurred while deleting the queue: {e}"
-            onError = self._config.get('onError', None)
+            onError = self._event.get('onError', self._config.get('onError', None))
             if callable(onError): onError(msg, e)
             logger.console.error(msg)
         return count
 
     def _clear(self):
         queue = self._getQueue()
         count = 0
         try:
             while not queue.empty():
                 queue.get()
                 count += 1
         except Exception as e:
             msg = f"An exception occurred while clearing the queue: {e}"
-            onError = self._config.get('onError', None)
+            onError = self._event.get('onError', self._config.get('onError', None))
             if callable(onError): onError(msg, e)
             logger.console.error(msg)
         return count
 
     def _add(self, **task):
         name = task.get('name', '')
         if name == '':
             return False
         res = False
         try:
             self._getQueue().put((name, task))
             res = True
         except pyqueue.Full:
-            onFull = self._config.get('onFull', None)
+            onFull = self._event.get('onFull', self._config.get('onFull', None))
             if callable(onFull): onFull()
         except Exception as e:
             msg = f"An exception occurred while adding the queue: {e}"
-            onError = self._config.get('onError', None)
+            onError = self._event.get('onError', self._config.get('onError', None))
             if callable(onError): onError(msg, e)
             logger.console.error(msg)
         return res
 
     def _setQueue(self):
         try:
-            if self._config.get('queueType', '') == 'PriorityQueue':
-                self.queue = pyqueue.PriorityQueue(maxsize=self._config.get('maxsize', 0))
-            elif self._config.get('queueType', '') == 'LifoQueue':
-                self.queue = pyqueue.LifoQueue(maxsize=self._config.get('maxsize', 0))
-            elif self._config.get('queueType', '') == 'ProcessQueue':
-                self.queue = multiprocessing.Manager().Queue(maxsize=self._config.get('maxsize', 0))
+            if self._setting.get('queueType', '') == 'PriorityQueue':
+                self.queue = pyqueue.PriorityQueue(maxsize=self._setting.get('maxsize', 0))
+            elif self._setting.get('queueType', '') == 'LifoQueue':
+                self.queue = pyqueue.LifoQueue(maxsize=self._setting.get('maxsize', 0))
+            elif self._setting.get('queueType', '') == 'ProcessQueue':
+                self.queue = multiprocessing.Manager().Queue(maxsize=self._setting.get('maxsize', 0))
             else:
-                self.queue = pyqueue.Queue(maxsize=self._config.get('maxsize', 0))
+                self.queue = pyqueue.Queue(maxsize=self._setting.get('maxsize', 0))
 
             useProcess = self._config.get('useProcess', False)
             usePool = self._config.get('usePool', True)
             params = dict({
                 'name': self._name,
                 'target': self._run,
-                'config': {
-                    'max': self._config.get('max', 1),
-                    'daemon': self._config.get('daemon', True),
-                    'block': self._config.get('block', False),
-                }
+                'config': self._config
             })
             if useProcess:
                 (process.runPool if usePool else process.run)(**params)
             else:
                 (thread.runPool if usePool else thread.run)(**params)
 
-            onStart = self._config.get('onStart', None)
+            onStart = self._event.get('onStart', self._config.get('onStart', None))
             if callable(onStart): onStart(self._userQueue)
             logger.console.info(f"Queue [{self._name}] has been started")
         except Exception as e:
             msg = f"An exception occurred while starting  the queue: {e}"
-            onError = self._config.get('onError', None)
+            onError = self._event.get('onError', self._config.get('onError', None))
             if callable(onError): onError(msg, e)
             logger.console.error(msg)
 
         return self
 
     def _getQueue(self):
         if self.queue is None:
@@ -165,39 +165,39 @@
         return self.queue
 
     def _run(self, **kwargs):
         while self._runnding == True:
             queue = self._getQueue()
             try:
                 taskTuple = queue.get(
-                    block=self._config.get('getBlock', True),
-                    timeout=self._config.get('getTimeout', None)
+                    block=self._setting.get('getBlock', True),
+                    timeout=self._setting.get('getTimeout', None)
                 )
                 if len(taskTuple) == 2:
-                    onRecv = self._config.get('onRecv', None)
+                    onRecv = self._event.get('onRecv', self._config.get('onRecv', None))
                     if callable(onRecv): onRecv(taskTuple[1])
-                    run = self._config.get('run', None)
+                    run = self._event.get('run', None)
                     if callable(run):
                         run(taskTuple[1])
                     if hasattr(queue, 'task_done'): queue.task_done()
             except pyqueue.Empty:
-                onEmpty = self._config.get('onEmpty', None)
+                onEmpty = self._event.get('onEmpty', self._config.get('onEmpty', None))
                 if callable(onEmpty): onEmpty()
             except BrokenPipeError as e:
                 pass
             except EOFError as e:
                 pass
             except Exception as e:
                 msg = f"An exception occurred while executing  the queue: {e}"
-                onError = self._config.get('onError', None)
+                onError = self._event.get('onError', self._config.get('onError', None))
                 if callable(onError): onError(msg, e)
-                if self._config.get('excepTaskDone', True):
+                if self._setting.get('excepTaskDone', True):
                     try:
                         if hasattr(queue, 'task_done'): queue.task_done()
-                    except Exception as ex:
+                    except Exception:
                         pass
                 logger.console.debug(msg)
 
     def _size(self):
         return self._getQueue().qsize()
 
     def _qsize(self):
@@ -217,19 +217,22 @@
              config = {
                 'name':'socket',#队列名称 名称不能重复 否则以已存在的名称运行
                 'daemon': True,  # 是否守护执行
                 'block': False,  # 是否阻塞执行
                 'max': 1,  # 进程池或线程池数量
                 'useProcess': False,  # 是否使用独立进程 默认独立线程
                 'usePool': True,  # 是否线程池或进程池,
-                'onStart': onStart, #队列已启动
-                'onRecv':onRecv, #收到任务
-                'onEmpty': onEmpty,#队列为空
-                'onFull': onFull,#队列已满
-                'onError': onError#发生异常
+                'event':{
+                   'run': run, #执行回调
+                   'onStart': onStart, #队列已启动
+                   'onRecv':onRecv, #收到任务
+                   'onEmpty': onEmpty,#队列为空
+                   'onFull': onFull,#队列已满
+                   'onError': onError#发生异常
+                }
              }
                """
 
         try:
             queue().run(config)
         except Exception as e:
             logger.console.error(f'An exception occurred while starting  the queue:{e}')
```

### Comparing `ipyweb-1.0.7/ipyweb/services/socketServer.py` & `ipyweb-1.0.8/ipyweb/services/crontab.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,204 +1,195 @@
-import os
-import asyncio
+from apscheduler.schedulers.background import BackgroundScheduler, BlockingScheduler
 from ipyweb.logger import logger
 from ipyweb.process import process
 from ipyweb.thread import thread
+from ipyweb.utils import utils
 
 
-class socketServer():
-
-    def run(self, *args, **params):
-        # pool版携带参数嵌套kwargs
+class crontab():
+    def run(self, **params):
         params = params.get('kwargs', {}) if params.get('kwargs', None) is not None else params
-        return socketServerIpyweb()._run(**params)
+        crontabIpyweb()._run(params.get('config', {}))
+
 
+class crontabIpyweb():
+    _config = {}
+    _event = {}
+    _scheduler = None
+    _job = None
+
+    def _run(self, config={}):
+        self._config = dict(self._config, **config)
+        self._event = dict(self._event, **self._config.get('event', {}))
+        try:
+            self._start()
+        except Exception as e:
+            onError = self._event.get('onError', self._config.get('onError', None))
+            if callable(onError): onError(e)
+
+    def _start(self):
+        schedulerParams = utils.get(self._config, 'setting.schedulerParams', {})
+        if utils.get(self._config, 'setting.scheduler') == 'blocking':
+            self._scheduler = BlockingScheduler(**schedulerParams)
+        elif utils.get(self._config, 'setting.scheduler') == 'background':
+            self._scheduler = BackgroundScheduler(**schedulerParams)
+        else:
+            self._scheduler = utils.get(self._config, 'setting.scheduler')
+        if self._scheduler:
+            taskSetting = self._config.get('taskSetting', {})
+            if taskSetting.get('enable', False):
+                run = crontabTasker(taskSetting)._run
+            else:
+                run = self._event.get('run', self._config.get('run', None))
 
-class socketServerIpyweb():
-    websockets = set()
-    websocket = None
-    path = ''
-    name = ''
-    config = {
-        'host': 'localhost',
-        'port': 8765
-    }
-    _logUseTxt = ''
-
-    def _run(self, **params):
-        self.name = params.get("name", "")
-        self.config = dict(self.config, **params.get('config'))
-        useProcess = 'process' if self.config.get("useProcess", True) else 'thread'
-        usePool = 'pool' if self.config.get("usePool", True) else ''
-        self._logUseTxt = f'{useProcess}{usePool}'
-        if self.config.get('autoKill', True): self._autoKillPort()
-        asyncio.run(self._start())
+            onStart = self._event.get('onStart', self._config.get('onStart', None))
+            jobTrigger = utils.get(self._config, 'setting.jobTrigger', 'interval')
+            jobParams = utils.get(self._config, 'setting.jobParams', {})
+            if callable(run):
+                self._job = self._scheduler.add_job(run, jobTrigger, kwargs=self._config, **jobParams)
+                self._scheduler.start()
+                if callable(onStart): onStart(self._scheduler, self._job)
         return self
 
-    async def _runServe(self):
 
+class crontabTasker():
+    _config = {}
+    _onTasked = None
+
+    def __init__(self, taskSetting={}):
+        self._config = dict(self._config, **taskSetting)
+
+    def _run(self, **config):
+        self._onTasked = config.get('event',{}).get('onTasked', None)
         try:
-            import websockets
-            import psutil
-        except ImportError:
-            logger.console.error('please installer the module: websockets and psutil (pip install websockets psutil)')
-            return self
-
-        serveConfig = dict(self.config.get('serveConfig', {}), **{
-            'ws_handler': lambda wss, path: self._onMessage(wss, path),
-            'host': self.config.get('host'),
-            'port': self.config.get('port'),
-        })
-        if self.config.get('ssl', False) and self.config.get('serveConfig', {}).get('ssl', None) is None:
-            import ssl
-            from webview import generate_ssl_cert
-            ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS_SERVER)
-            keyfile, certfile = generate_ssl_cert()
-            ssl_context.load_cert_chain(certfile=certfile, keyfile=keyfile)
-            serveConfig['ssl'] = ssl_context
-
-        async with websockets.serve(**serveConfig) as server:
-            logger().console.info(
-                f'Socket [{self.name}][ws://{self.config.get("host")}:{self.config.get("port")}] use [{self._logUseTxt}] has been started [PID:{os.getpid()}]')
-            onReady = self.config.get('onReady', None)
-            if callable(onReady): await onReady(server)
-            await server.wait_closed()
-
-    async def _start(self):
-
-        try:
-            await  self._runServe()
-        except OSError as e:
-            if e.errno == 10048 and self.config.get('autoKill', True):
-                logger().console.debug(f'Socket [{self.name}] port is occupied')
-                self._autoKillPort()
-                await self._runServe()
+            self._start()
+        except Exception as e:
+            logger.console.error(f'An exception occurred while executing the scheduled task:{e}')
+
+    def _start(self):
+        if self._config.get('default', '') == 'openUrl':
+            self._openUrl()
+        elif self._config.get('default', '') == 'exeCommand':
+            self._exeCommand()
+        elif self._config.get('default', '') == 'exePython':
+            self._exePython()
+        elif self._config.get('default', '') == 'invokeCall':
+            self._invokeCall()
+
+    def _openUrl(self):
+        import requests
+        config = self._config.get('openUrl', {})
+        try:
+            type = config.get('type', 'get')
+            if 'type' in config:
+                del config['type']
+            if type == 'post':
+                response = requests.post(**config)
             else:
-                logger().console.error(
-                    f'An exception occurred while killing the socket [{self.name}] process:{e} ')
-            onError = self.config.get('onError', None)
-            if callable(onError): await onError(e)
-        except Exception as e:
-            logger().console.error(
-                f'An exception occurred while starting the socket [{self.name}] using  {self._logUseTxt}:{e} ')
-            onError = self.config.get('onError', None)
-            if callable(onError): await onError(e)
-
-    async def _onMessage(self, websocket, path):
-        self.websockets.add(websocket)
-        if self.websocket is None:
-            onConnect = self.config.get('onConnect', None)
-            if callable(onConnect): await onConnect(websocket, path)
-        self.websocket = websocket
-        self.path = path
-        onMessage = self.config.get('onMessage', None)
-        import websockets
-        try:
-            async for message in self.websocket:
-                try:
-                    if callable(onMessage): await onMessage(message)
-                except Exception as e:
-                    onError = self.config.get('onError', None)
-                    if callable(onError):
-                        await onError(e)
-        # except websockets.ConnectionClosed as e:
-        #     self.websocket = None
-        #     self.path = ''
-        #     onClosed = self.config.get('onClosed', None)
-        #     if callable(onClosed): await onClosed()
-        except Exception as e:
-            onError = self.config.get('onError', None)
-            if callable(onError): await onError(e)
-        finally:
-            self.websocket = None
-            self.path = ''
-            self.websockets.remove(websocket)
-            onClosed = self.config.get('onClosed', None)
-            if callable(onClosed): await onClosed()
-
-    def _autoKillPort(self):
-        try:
-            port = self.config.get('port')
-            if port and porter.isPort(port) and self.config.get('autoKill', True):
-                porter.closePort(port)
-        except Exception as ex:
-            pass
-        return self
+                response = requests.get(**config)
+            response.raise_for_status()
+        except Exception as e:
+            logger.file.error(f"An exception occurred while requesting access to the website:{e}")
+        except requests.exceptions.HTTPError as e:
+            logger.file.error(f"An exception occurred while requesting access to the website:{e}")
+        except requests.exceptions.RequestException as e:
+            logger.file.error(f"An exception occurred while requesting access to the website:{e}")
+        else:
+            if callable(self._onTasked): self._onTasked(response.text)
+
+    def _exeCommand(self):
+        try:
+            config = self._config.get('exeCommand')
+            runCommand = config.get('runCommand', [])
+            if runCommand and len(runCommand) > 0:
+                import subprocess
+                runParams = dict({
+                    'shell': utils.isWin(),
+                    'check': True,
+                    'text': True
+
+                }, **config.get('runParams', {}))
+                result = subprocess.run(runCommand, **runParams)
+                if callable(self._onTasked): self._onTasked(result)
+        except Exception as e:
+            logger.file.error(f"An exception occurred while executing the command:{e}")
+
+    def _exePython(self):
+        try:
+            exePython = self._config.get('exePython', '')
+            if exePython:
+                result = exec(exePython)
+                if callable(self._onTasked): self._onTasked(result)
+        except Exception as e:
+            logger.file.error(f"An exception occurred while executing the pythonCommand:{e}")
 
+    def _invokeCall(self):
+        try:
+            config = self._config.get('invokeCall')
+            moduleName = config.get('module', '')
+            className = config.get('class', '')
+            methodName = config.get('method', 'process')
+            methodParams = config.get('params', None)
+            import importlib
+            module = utils.smartImportModule(className, moduleName)
+            print(hasattr(module, className), module, className, moduleName)
+            if hasattr(module, className):
+                classAttr = getattr(module, className)
+                classInstance = classAttr()
+                if hasattr(classInstance, methodName):
+                    method = getattr(classInstance, methodName)
+                    result = method(methodParams) if methodParams else method()
+                    if callable(self._onTasked): self._onTasked(result)
+
+        except Exception as e:
+            print(type(e))
+            logger.file.error(f"An exception occurred while executing the command:{e}")
 
-class socketServerRunner():
+
+class crontabRunner():
 
     def run(self, **config):
         """
              config = {
-                'name':'socket',#定时器名称 名称不能重复 否则以已存在的名称运行
-                'daemon': True,  # 是否守护执行
-                'block': False,  # 是否阻塞执行
-                'max': 1,  # 进程池或线程池数量
-                'useProcess': False,  # 是否使用独立进程 默认独立线程
-                'usePool': True,  # 是否线程池或进程池,
-                'onReady': onReady, #准备连接
-                'onConnect':onConnect, #连接成功回调
-                'onError': onError,#错误回调
-                'onClosed': onClosed,#关闭回调
-                'onMessage': onMessage#消息回调
-             }
+                'name':'socket',#队列名称 名称不能重复 否则以已存在的名称运行
+                'daemon': True,  # 启动线程是否守护执行
+                'block': False,  # 启动线程是否阻塞执行
+                'usePool': False,  # 是否线程池启动
+                'useProcess': False,  # 是否使用进程
+                'max': 1,  # 启动线程数量
+                'event':{
+                   'run': run, #执行回调
+                   'onStart':onStart, #开始回调
+                   'onError': onError,#错误回调
+                   'onTasked': onTasked,#任务已执行
+                }
+                'setting': { # 配置选项
+                   'schedulerType': 'blocking',  #调度器类型 blocking:阻塞计划任务 background:非阻塞计划任务
+                   'schedulerParams': {},# 调度器参数
+                   'jobTrigger': 'interval',  # 任务触发类型  cron:定时任务  interval:间隔循环任务  date：在指定的时间点触发任务。
+                   'jobParams': {  # 任务触发参数
+                      'seconds': 3
+                     }
+                   },
+                'taskSetting':{
+
+                 }
+
+               }
                """
 
         try:
-            useProcess = config.get('useProcess', False)
-            usePool = config.get('usePool', False)
-            params = dict({
+            useProcess = config.get('useProcess', False)  # 默认线程
+            usePool = config.get('usePool', False)  # 默认进程
+            params = {
                 'name': config.get('name', __name__),
-                'target': socketServer().run,
+                'target': crontab().run,
                 'config': config
-            })
+            }
 
             if useProcess:
                 (process.runPool if usePool else process.run)(**params)
             else:
                 (thread.runPool if usePool else thread.run)(**params)
 
         except Exception as e:
-            logger.console.error(f'An exception occurred while starting the socket:{e}')
-
-
-class porter:
-
-    @classmethod
-    def closePort(self, port):
-        pid = 0
-        try:
-            process_info = self.findProcessByPort(port)
-            if process_info:
-                pid = process_info['pid']
-                self.killPid(pid)
-        except Exception as e:
-            pass
-        return pid
-
-    @classmethod
-    def killPid(self, pid, myself=False):
-        try:
-            if os.getpid() != pid or (myself == True and os.getpid() == pid):
-                os.kill(pid, 9)
-        except OSError:
-            pass
-
-    @classmethod
-    def findProcessByPort(self, port):
-        import psutil
-        for proc in psutil.process_iter(['pid', 'name']):
-            for conn in proc.connections():
-                if conn.laddr[1] == port:
-                    return proc.info
-        return None
-
-    @classmethod
-    def isPort(self, port, host='127.0.0.1') -> bool:
-        import socket
-        with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
-            try:
-                s.connect((host, port))
-                return True
-            except ConnectionRefusedError:
-                return False
+            logger.console.error(f'An exception occurred while starting  the crontab:{e}')
```

### Comparing `ipyweb-1.0.7/ipyweb/services/timer.py` & `ipyweb-1.0.8/ipyweb/services/timer.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,27 +16,30 @@
     def stop(self):
         self.running = False
         return self
 
     def start(self, **config):
 
         config = config.get('config', {})
-        run = config.get('run', None)
-        onStart = config.get('onStart', None)
-        onError = config.get('onError', None)
+        setting = config.get('setting', {})
+        event = config.get('event', {})
+        run = event.get('run', config.get('run', None))
+        onStart = event.get('onStart', config.get('onStart', None))
+        onError = event.get('onError', config.get('onError', None))
+
         try:
             self.running = True
             if callable(onStart): onStart(self)
-            time.sleep(config.get('sleep', self.defaultSleepTime))
+            time.sleep(setting.get('sleep', self.defaultSleepTime))
             while self.running == True and callable(run):
                 try:
                     run(self)
                 except TypeError as e:
                     run()
-                time.sleep(config.get('interval', self.defaultInterval))
+                time.sleep(setting.get('interval', self.defaultInterval))
         except KeyboardInterrupt as e:
             pass
         except Exception as e:
             logger.console.debug(f"An exception occurred while executing the timer:{e}")
             if callable(onError): onError(e)
         return self
 
@@ -44,22 +47,29 @@
 # 智能启动
 class timerRunner():
 
     def run(self, **config):
         """
        config = {
         'name':__name__,#定时器名称 名称不能重复 否则以已存在的名称运行
-        'run':run,#回调执行方法
         'daemon': True,  # 是否守护执行
         'block': False,  # 是否阻塞执行
         'max': 1,  # 进程池或线程池数量
         'useProcess': False,  # 是否使用独立进程 默认独立线程
         'usePool': False,  # 是否线程池或进程池
-        'interval': 5,  # 间隔时间
-        'sleep': 5,  # 延时执行
+        'run': run, #执行回调
+        'event':{
+           'run': run, #执行回调
+           'onStart':onStart, #开始回调
+           'onError': onError,#错误回调
+        }
+        'setting':{
+           'interval': 5,  # 间隔时间
+           'sleep': 5,  # 延时执行
+         }
        }
         """
         try:
 
             useProcess = config.get('useProcess', False)  # 默认线程
             usePool = config.get('usePool', False)  # 默认进程
             params = {
```

### Comparing `ipyweb-1.0.7/ipyweb/thread.py` & `ipyweb-1.0.8/ipyweb/thread.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,46 +42,51 @@
     @classmethod
     def _runPool(self, **params):
         name = params.get('name', 'default')
         target = params.get('target', None)
         config = params.get('config', {})
         onStart = params.get('onStart', None)
         onError = params.get('onError', None)
-
+        poolConfig = params.get('poolConfig', {})
         if target is None or callable(target) == False:
             return None
         try:
             if self.threads.get(name, None) is None:
                 self.threads[name] = {}
                 self.threads[name]['params'] = params
+
+                poolConfig = dict({
+                    'max_workers': config.get('max', 1),
+                    'thread_name_prefix': name
+                }, **poolConfig)
+
                 if config.get('block', False):  # 阻塞运行
 
-                    with ThreadPoolExecutor(max_workers=config.get('max', 1), thread_name_prefix=name) as executor:
+                    with ThreadPoolExecutor(**poolConfig) as executor:
                         self.threads[name]['thread'] = executor = executor.submit(
                             self._target,
                             **params  # 不要使用kwargs形式赋值**config 为了保持回调一致 这里不要改成 kwargs=config
                         )
                         # result = executor.result()
                         # done=executor.done()
                 else:  # 非阻塞运行
-                    self.threads[name]['thread'] = executor = ThreadPoolExecutor(
-                        max_workers=config.get('max', 1),
-                        thread_name_prefix=name
-                    )
+                    self.threads[name]['thread'] = executor = ThreadPoolExecutor(**poolConfig)
                     try:
                         self.threads[name]['thread'] = executor.submit(
                             self._target,
                             **params  # 不要使用kwargs形式赋值**config 为了保持回调一致 这里不要改成 kwargs=config
                         )
                     finally:
                         pass
                         # executor.shutdown()  # 参数True形成阻塞 非阻塞可自行关闭线程池
                 if callable(onStart): onStart(executor)
 
             return executor
+        except KeyboardInterrupt:
+            pass
         except pickle.PicklingError as e:
             msg = f'A serialization error occurred while starting the [{name}] thread pool.'
             logger.console.error(msg)
             if callable(onError): onError(msg, e)
         except Exception as e:
             msg = f'An exception occurred while starting with the [{name}] thread pool:{e}'
             logger.console.error(msg)
@@ -110,14 +115,16 @@
                 )
                 self.threads[name]['thread'].daemon = config.get('daemon', True)
                 self.threads[name]['thread'].start()
                 if config.get('block', False):  # 是否阻塞
                     self.threads[name]['thread'].join()
                 if callable(onStart): onStart(self.threads[name]['thread'])
             return self.threads[name]['thread']
+        except KeyboardInterrupt:
+            pass
         except pickle.PicklingError as e:
             msg = f'A serialization error occurred while starting the [{name}] thread.'
             logger.console.error(msg)
             if callable(onError): onError(msg, e)
         except Exception as e:
             msg = f'An exception occurred while starting with the [{name}] thread:{e}'
             logger.console.error(msg)
```

### Comparing `ipyweb-1.0.7/ipyweb/utils.py` & `ipyweb-1.0.8/ipyweb/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,35 @@
 import os
 import sys
 from urllib.parse import urlparse
 from ipyweb.singleton import singleton
 
 
 class utils(metaclass=singleton):
+
+    @classmethod
+    # 链式获取配置
+    def get(self, configData={}, key='', default=None):
+        try:
+            if key == '':
+                return configData;
+            if '.' in key:
+                keys = key.split('.')
+                dict = configData
+                for k in keys:
+                    if k in dict:
+                        dict = dict.get(k, default)
+                    else:
+                        return default  # 如果某个键不存在，返回None
+                return dict
+            else:
+                return configData.get(key, default)
+        except Exception as e:
+            return configData
+
     def isModuleInstalled(name='') -> bool:
         try:
             import importlib
             importlib.import_module(name)
             return True
         except ImportError:
             return False
@@ -39,32 +60,14 @@
     @classmethod
     def tuple(self, data=(), index=0, default=None):
         try:
             return data[index]
         except IndexError:
             return default
 
-    @classmethod
-    def get(self, data={}, key='', default=None):
-        try:
-            if key == '':
-                return data;
-            if '.' in key:
-                keys = key.split('.')
-                dict = data
-                for k in keys:
-                    if k in dict:
-                        dict = dict.get(k, default)
-                    else:
-                        return default  # 如果某个键不存在，返回None
-                return dict
-            else:
-                return data.get(key, default)
-        except Exception as e:
-            return data
 
     @classmethod
     def checkUrl(self, domain, port) -> bool:
         try:
             import socket
             socket.create_connection((domain, port), timeout=1).close()
             return True
@@ -77,14 +80,22 @@
         domain = parsed_url.hostname
         port = parsed_url.port
         if domain == None: domain = 'localhost'
         if port == None: port = 80
         return domain, port
 
     @classmethod
+    def isUrl(self, url):
+        import re
+        url_pattern = re.compile(
+            r'http[s]?://(?:[a-zA-Z]|[0-9]|[$-_@.&+]|[!*\\(\\),]|(?:%[0-9a-fA-F][0-9a-fA-F]))+'
+        )
+        return bool(url_pattern.match(url))
+
+    @classmethod
     def inJson(self, key, json) -> bool:
         return True if key in json else False
 
     @classmethod
     def isJson(self, strings='') -> bool:
         if isinstance(strings, str):
             try:
```

### Comparing `ipyweb-1.0.7/ipyweb/windowEvents/main.py` & `ipyweb-1.0.8/ipyweb/windowEvents/main.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.7/ipyweb.egg-info/PKG-INFO` & `ipyweb-1.0.8/ipyweb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyweb
-Version: 1.0.7
+Version: 1.0.8
 Summary: A business framework for launching multiple services
 Author-email: sqwindows <sqwindows@qq.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2014-2017, Roman Sirokov
         All rights reserved.
```

### Comparing `ipyweb-1.0.7/ipyweb.egg-info/SOURCES.txt` & `ipyweb-1.0.8/ipyweb.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 ipyweb/db.py
 ipyweb/event.py
 ipyweb/gui.py
 ipyweb/ipyweb.py
 ipyweb/jsonFile.py
 ipyweb/logger.py
 ipyweb/module.py
-ipyweb/multiton.py
 ipyweb/preload.py
 ipyweb/process.py
 ipyweb/service.py
 ipyweb/singleton.py
 ipyweb/thread.py
 ipyweb/utils.py
 ipyweb.egg-info/PKG-INFO
@@ -58,15 +57,18 @@
 ipyweb/guis/IpywebServer.py
 ipyweb/guis/LocalServer.py
 ipyweb/guis/RemoteServer.py
 ipyweb/preloads/block/controllerPreload.py
 ipyweb/preloads/block/guiPreload.py
 ipyweb/preloads/block/processPreload.py
 ipyweb/preloads/process/examplePreload.py
+ipyweb/preloads/thread/crontabPreload.py
 ipyweb/preloads/thread/queuePreload.py
 ipyweb/preloads/thread/socketPreload.py
 ipyweb/preloads/thread/timerPreload.py
 ipyweb/pywebview/windows.py
+ipyweb/services/crontab.py
 ipyweb/services/queue.py
+ipyweb/services/socketClient.py
 ipyweb/services/socketServer.py
 ipyweb/services/timer.py
 ipyweb/windowEvents/main.py
```

### Comparing `ipyweb-1.0.7/pyproject.toml` & `ipyweb-1.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ipyweb"
-version = "1.0.7"
+version = "1.0.8"
 description = "A business framework for launching multiple services"
 authors = [
     { name = "sqwindows", email = "sqwindows@qq.com" },
 ]
 
 keywords = ["gui", "webkit", "html", "web"]
 requires-python = ">=3.8"
```

