# Comparing `tmp/owega-5.9.1.tar.gz` & `tmp/owega-5.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owega-5.9.1.tar", last modified: Thu May 30 14:58:16 2024, max compression
+gzip compressed data, was "owega-5.9.2.tar", last modified: Sun Jun  2 14:24:30 2024, max compression
```

## Comparing `owega-5.9.1.tar` & `owega-5.9.2.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-30 14:58:16.048338 owega-5.9.1/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6076 2024-05-10 14:44:53.000000 owega-5.9.1/LICENSE
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    17456 2024-05-30 14:58:16.047338 owega-5.9.1/PKG-INFO
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5261 2024-05-24 17:59:52.000000 owega-5.9.1/README.md
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-30 14:58:16.045338 owega-5.9.1/owega/
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-30 14:58:16.047338 owega-5.9.1/owega/OweHandlers/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      156 2024-04-27 12:05:16.000000 owega-5.9.1/owega/OweHandlers/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1309 2024-05-30 14:39:04.000000 owega-5.9.1/owega/OweHandlers/handle_add_sysmem.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1661 2024-05-30 14:38:22.000000 owega-5.9.1/owega/OweHandlers/handle_commands.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1453 2024-05-30 14:39:02.000000 owega-5.9.1/owega/OweHandlers/handle_context.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1895 2024-05-30 14:38:59.000000 owega-5.9.1/owega/OweHandlers/handle_del_sysmem.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2090 2024-05-30 14:38:55.000000 owega-5.9.1/owega/OweHandlers/handle_dinput.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3905 2024-05-30 14:39:55.000000 owega-5.9.1/owega/OweHandlers/handle_edit.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1373 2024-05-30 14:40:38.000000 owega-5.9.1/owega/OweHandlers/handle_estimation.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5526 2024-05-30 14:41:06.000000 owega-5.9.1/owega/OweHandlers/handle_finput.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2194 2024-05-30 14:41:27.000000 owega-5.9.1/owega/OweHandlers/handle_frequency.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      647 2024-05-30 14:42:01.000000 owega-5.9.1/owega/OweHandlers/handle_genconf.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      621 2024-05-30 14:43:09.000000 owega-5.9.1/owega/OweHandlers/handle_history.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3633 2024-05-30 14:43:42.000000 owega-5.9.1/owega/OweHandlers/handle_image.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1460 2024-05-30 14:44:19.000000 owega-5.9.1/owega/OweHandlers/handle_load.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2031 2024-05-30 14:44:35.000000 owega-5.9.1/owega/OweHandlers/handle_model.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2167 2024-05-30 14:44:57.000000 owega-5.9.1/owega/OweHandlers/handle_presence.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      698 2024-05-30 14:45:28.000000 owega-5.9.1/owega/OweHandlers/handle_quit.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1431 2024-05-30 14:45:33.000000 owega-5.9.1/owega/OweHandlers/handle_save.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1273 2024-05-30 14:45:38.000000 owega-5.9.1/owega/OweHandlers/handle_system.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2071 2024-05-30 14:45:54.000000 owega-5.9.1/owega/OweHandlers/handle_temperature.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1456 2024-05-30 14:46:00.000000 owega-5.9.1/owega/OweHandlers/handle_time.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1585 2024-05-30 14:46:27.000000 owega-5.9.1/owega/OweHandlers/handle_tokens.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1846 2024-05-30 14:46:35.000000 owega-5.9.1/owega/OweHandlers/handle_top_p.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1316 2024-05-30 14:46:53.000000 owega-5.9.1/owega/OweHandlers/handle_tts.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2609 2024-05-30 14:48:39.000000 owega-5.9.1/owega/OweHandlers/handlers.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-30 14:58:16.047338 owega-5.9.1/owega/OwegaFun/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      897 2024-05-30 14:12:10.000000 owega-5.9.1/owega/OwegaFun/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3963 2024-05-30 14:16:49.000000 owega-5.9.1/owega/OwegaFun/functions.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     4383 2024-05-30 14:20:27.000000 owega-5.9.1/owega/OwegaFun/longTermSouvenirs.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5837 2024-05-30 14:21:06.000000 owega-5.9.1/owega/OwegaFun/utility.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-30 14:58:16.047338 owega-5.9.1/owega/OwegaSession/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      100 2024-04-17 02:21:38.000000 owega-5.9.1/owega/OwegaSession/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3653 2024-05-30 14:29:19.000000 owega-5.9.1/owega/OwegaSession/main_bottom_toolbar.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6574 2024-05-30 14:36:18.000000 owega-5.9.1/owega/OwegaSession/promptsession.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      247 2024-05-30 14:53:09.000000 owega-5.9.1/owega/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       94 2024-04-17 02:21:38.000000 owega-5.9.1/owega/__main__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10471 2024-05-30 13:44:26.000000 owega-5.9.1/owega/ask.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-30 14:58:16.047338 owega-5.9.1/owega/changelog/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       80 2024-04-27 12:05:16.000000 owega-5.9.1/owega/changelog/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    26794 2024-05-30 14:55:54.000000 owega-5.9.1/owega/changelog/changelog.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1581 2024-05-30 13:46:26.000000 owega-5.9.1/owega/changelog/changelogEntry.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3388 2024-05-30 13:49:06.000000 owega-5.9.1/owega/changelog/version.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-30 14:58:16.047338 owega-5.9.1/owega/config/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       86 2024-04-17 02:21:38.000000 owega-5.9.1/owega/config/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2659 2024-05-30 14:04:19.000000 owega-5.9.1/owega/config/baseConf.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-30 14:58:16.047338 owega-5.9.1/owega/conversation/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       83 2024-04-17 02:21:38.000000 owega-5.9.1/owega/conversation/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10316 2024-05-30 14:08:05.000000 owega-5.9.1/owega/conversation/conversation.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1464 2024-05-30 14:08:40.000000 owega-5.9.1/owega/getLogger.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       64 2024-04-17 02:21:38.000000 owega-5.9.1/owega/handlerBase.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6059 2024-05-30 14:11:24.000000 owega-5.9.1/owega/license.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    12123 2024-05-30 13:41:59.000000 owega-5.9.1/owega/owega.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     7645 2024-05-30 14:53:03.000000 owega-5.9.1/owega/utils.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-30 14:58:16.047338 owega-5.9.1/owega.egg-info/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    17456 2024-05-30 14:58:16.000000 owega-5.9.1/owega.egg-info/PKG-INFO
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1689 2024-05-30 14:58:16.000000 owega-5.9.1/owega.egg-info/SOURCES.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        1 2024-05-30 14:58:16.000000 owega-5.9.1/owega.egg-info/dependency_links.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       43 2024-05-30 14:58:16.000000 owega-5.9.1/owega.egg-info/entry_points.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      173 2024-05-30 14:58:16.000000 owega-5.9.1/owega.egg-info/requires.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        6 2024-05-30 14:58:16.000000 owega-5.9.1/owega.egg-info/top_level.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       90 2024-04-17 02:21:38.000000 owega-5.9.1/pyproject.toml
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       38 2024-05-30 14:58:16.048338 owega-5.9.1/setup.cfg
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2573 2024-05-30 14:58:09.000000 owega-5.9.1/setup.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-06-02 14:24:30.937275 owega-5.9.2/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6076 2024-06-02 14:18:55.000000 owega-5.9.2/LICENSE
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    17508 2024-06-02 14:24:30.936275 owega-5.9.2/PKG-INFO
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5261 2024-06-02 14:18:55.000000 owega-5.9.2/README.md
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-06-02 14:24:30.928275 owega-5.9.2/owega/
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-06-02 14:24:30.933275 owega-5.9.2/owega/OweHandlers/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      156 2024-05-06 16:07:08.000000 owega-5.9.2/owega/OweHandlers/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1309 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_add_sysmem.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1661 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_commands.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1453 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_context.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1895 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_del_sysmem.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2090 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_dinput.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3905 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_edit.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1373 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_estimation.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5526 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_finput.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2194 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_frequency.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      647 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_genconf.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      621 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_history.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3633 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_image.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1460 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_load.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2031 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_model.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2167 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_presence.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      698 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_quit.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1431 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_save.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1273 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_system.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2071 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_temperature.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1456 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_time.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1585 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_tokens.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1846 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_top_p.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1316 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_tts.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2609 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handlers.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-06-02 14:24:30.933275 owega-5.9.2/owega/OwegaFun/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      897 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OwegaFun/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3963 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OwegaFun/functions.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     4383 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OwegaFun/longTermSouvenirs.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5837 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OwegaFun/utility.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-06-02 14:24:30.934275 owega-5.9.2/owega/OwegaSession/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      100 2024-04-17 02:21:38.000000 owega-5.9.2/owega/OwegaSession/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3653 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OwegaSession/main_bottom_toolbar.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6574 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OwegaSession/promptsession.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      247 2024-06-02 14:18:55.000000 owega-5.9.2/owega/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       94 2024-04-17 02:21:38.000000 owega-5.9.2/owega/__main__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10471 2024-06-02 14:18:55.000000 owega-5.9.2/owega/ask.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-06-02 14:24:30.934275 owega-5.9.2/owega/changelog/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       80 2024-05-06 16:07:08.000000 owega-5.9.2/owega/changelog/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    26935 2024-06-02 14:24:00.000000 owega-5.9.2/owega/changelog/changelog.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1581 2024-06-02 14:18:55.000000 owega-5.9.2/owega/changelog/changelogEntry.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3388 2024-06-02 14:18:55.000000 owega-5.9.2/owega/changelog/version.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-06-02 14:24:30.935275 owega-5.9.2/owega/config/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       86 2024-04-17 02:21:38.000000 owega-5.9.2/owega/config/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2659 2024-06-02 14:18:55.000000 owega-5.9.2/owega/config/baseConf.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-06-02 14:24:30.935275 owega-5.9.2/owega/conversation/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       83 2024-04-17 02:21:38.000000 owega-5.9.2/owega/conversation/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10316 2024-06-02 14:18:55.000000 owega-5.9.2/owega/conversation/conversation.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1464 2024-06-02 14:18:55.000000 owega-5.9.2/owega/getLogger.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       64 2024-04-17 02:21:38.000000 owega-5.9.2/owega/handlerBase.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6059 2024-06-02 14:18:55.000000 owega-5.9.2/owega/license.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    12123 2024-06-02 14:18:55.000000 owega-5.9.2/owega/owega.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     7822 2024-06-02 14:21:12.000000 owega-5.9.2/owega/utils.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-06-02 14:24:30.936275 owega-5.9.2/owega.egg-info/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    17508 2024-06-02 14:24:30.000000 owega-5.9.2/owega.egg-info/PKG-INFO
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1689 2024-06-02 14:24:30.000000 owega-5.9.2/owega.egg-info/SOURCES.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        1 2024-06-02 14:24:30.000000 owega-5.9.2/owega.egg-info/dependency_links.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       43 2024-06-02 14:24:30.000000 owega-5.9.2/owega.egg-info/entry_points.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      173 2024-06-02 14:24:30.000000 owega-5.9.2/owega.egg-info/requires.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        6 2024-06-02 14:24:30.000000 owega-5.9.2/owega.egg-info/top_level.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       90 2024-04-17 02:21:38.000000 owega-5.9.2/pyproject.toml
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       38 2024-06-02 14:24:30.937275 owega-5.9.2/setup.cfg
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2573 2024-06-02 14:24:15.000000 owega-5.9.2/setup.py
```

### Comparing `owega-5.9.1/LICENSE` & `owega-5.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/PKG-INFO` & `owega-5.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owega
-Version: 5.9.1
+Version: 5.9.2
 Summary: A command-line interface for conversing with GPT models (from OpenAI)
 Home-page: https://git.pyrokinesis.fr/darkgeem/owega
 Author: darkgeem
 Author-email: darkgeem@pyrokinesis.fr
 License: DGPL-1.0
 Project-URL: Source, https://git.pyrokinesis.fr/darkgeem/owega
 Project-URL: Support, https://discord.gg/KdRmyRrA48
@@ -144,15 +144,15 @@
 ### Demos made with ΦωΦ 5.7.5
 [![asciicast](https://asciinema.org/a/659607.png)](https://asciinema.org/a/659607)
 [Youtube demo](https://youtu.be/_LGSc6mj-EM)
 
 
 ## CHANGELOG: 
 ```
-OWEGA v5.9.1 CHANGELOG:
+OWEGA v5.9.2 CHANGELOG:
 
 
 2.0.0: WTFPL license
 2.0.1: added genconf command
 
 2.1.0: added file_input command
 2.1.1: added file_input in help command
@@ -397,9 +397,10 @@
        files.
 5.8.6: Updated the README with 5.7.5 demos.
 
 5.9.0: Fixed a huge issue where owega couldn't be imported if
        the terminal wasn't interactive.
        Added owega.__version__
 5.9.1: Changed type hinting and fixed some code style!
+5.9.2: Added a tts_to_opus function in owega.utils.
 
 ```
```

### Comparing `owega-5.9.1/README.md` & `owega-5.9.2/README.md`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/owega/OweHandlers/handle_add_sysmem.py` & `owega-5.9.2/owega/OweHandlers/handle_add_sysmem.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/owega/OweHandlers/handle_commands.py` & `owega-5.9.2/owega/OweHandlers/handle_commands.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/owega/OweHandlers/handle_context.py` & `owega-5.9.2/owega/OweHandlers/handle_context.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/owega/OweHandlers/handle_del_sysmem.py` & `owega-5.9.2/owega/OweHandlers/handle_del_sysmem.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/owega/OweHandlers/handle_dinput.py` & `owega-5.9.2/owega/OweHandlers/handle_dinput.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/owega/OweHandlers/handle_edit.py` & `owega-5.9.2/owega/OweHandlers/handle_edit.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/owega/OweHandlers/handle_estimation.py` & `owega-5.9.2/owega/OweHandlers/handle_estimation.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/owega/OweHandlers/handle_finput.py` & `owega-5.9.2/owega/OweHandlers/handle_finput.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/owega/OweHandlers/handle_frequency.py` & `owega-5.9.2/owega/OweHandlers/handle_frequency.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/owega/OweHandlers/handle_genconf.py` & `owega-5.9.2/owega/OweHandlers/handle_genconf.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/owega/OweHandlers/handle_history.py` & `owega-5.9.2/owega/OweHandlers/handle_history.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/owega/OweHandlers/handle_image.py` & `owega-5.9.2/owega/OweHandlers/handle_image.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/owega/OweHandlers/handle_load.py` & `owega-5.9.2/owega/OweHandlers/handle_load.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/owega/OweHandlers/handle_model.py` & `owega-5.9.2/owega/OweHandlers/handle_model.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/owega/OweHandlers/handle_presence.py` & `owega-5.9.2/owega/OweHandlers/handle_presence.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/owega/OweHandlers/handle_quit.py` & `owega-5.9.2/owega/OweHandlers/handle_quit.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/owega/OweHandlers/handle_save.py` & `owega-5.9.2/owega/OweHandlers/handle_save.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/owega/OweHandlers/handle_system.py` & `owega-5.9.2/owega/OweHandlers/handle_system.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/owega/OweHandlers/handle_temperature.py` & `owega-5.9.2/owega/OweHandlers/handle_temperature.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/owega/OweHandlers/handle_time.py` & `owega-5.9.2/owega/OweHandlers/handle_time.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/owega/OweHandlers/handle_tokens.py` & `owega-5.9.2/owega/OweHandlers/handle_tokens.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/owega/OweHandlers/handle_top_p.py` & `owega-5.9.2/owega/OweHandlers/handle_top_p.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/owega/OweHandlers/handle_tts.py` & `owega-5.9.2/owega/OweHandlers/handle_tts.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/owega/OweHandlers/handlers.py` & `owega-5.9.2/owega/OweHandlers/handlers.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/owega/OwegaFun/__init__.py` & `owega-5.9.2/owega/OwegaFun/__init__.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/owega/OwegaFun/functions.py` & `owega-5.9.2/owega/OwegaFun/functions.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/owega/OwegaFun/longTermSouvenirs.py` & `owega-5.9.2/owega/OwegaFun/longTermSouvenirs.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/owega/OwegaFun/utility.py` & `owega-5.9.2/owega/OwegaFun/utility.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/owega/OwegaSession/main_bottom_toolbar.py` & `owega-5.9.2/owega/OwegaSession/main_bottom_toolbar.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/owega/OwegaSession/promptsession.py` & `owega-5.9.2/owega/OwegaSession/promptsession.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/owega/ask.py` & `owega-5.9.2/owega/ask.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/owega/changelog/changelog.py` & `owega-5.9.2/owega/changelog/changelog.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,18 @@
         self.version = Version(0, 0, 0)
         self.initLogs()
         self.genLog()
 
     def initLogs(self) -> None:
         """Fill the changelog."""
         self.logs.append(
+            ChangelogEntry(5, 9, 2)
+            .addLine("Added a tts_to_opus function in owega.utils.")
+        )
+        self.logs.append(
             ChangelogEntry(5, 9, 1)
             .addLine("Changed type hinting and fixed some code style!")
         )
         self.logs.append(
             ChangelogEntry(5, 9, 0)
             .addLine("Fixed a huge issue where owega couldn't be imported if")
             .addLine("the terminal wasn't interactive.")
```

### Comparing `owega-5.9.1/owega/changelog/changelogEntry.py` & `owega-5.9.2/owega/changelog/changelogEntry.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/owega/changelog/version.py` & `owega-5.9.2/owega/changelog/version.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/owega/config/baseConf.py` & `owega-5.9.2/owega/config/baseConf.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/owega/conversation/conversation.py` & `owega-5.9.2/owega/conversation/conversation.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/owega/getLogger.py` & `owega-5.9.2/owega/getLogger.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/owega/license.py` & `owega-5.9.2/owega/license.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/owega/owega.py` & `owega-5.9.2/owega/owega.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/owega/utils.py` & `owega-5.9.2/owega/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,28 +65,33 @@
         while pygame.mixer.get_busy():
             pygame.time.delay(100)
     except KeyboardInterrupt:
         pass
     pygame.mixer.quit()
 
 
+def tts_to_opus(loc: str, text: str, voice: str = 'nova') -> None:
+    """Generate TTS audio from given text and save it to an opus file."""
+    tts_answer = openai.audio.speech.create(
+        model='tts-1',
+        voice=voice,
+        input=text
+    )
+    tts_answer.write_to_file(loc)
+
+
 def play_tts(text: str, voice: str = 'nova') -> None:
     """Generate TTS audio from given text and play it."""
     tmpfile = tempfile.NamedTemporaryFile(
         prefix="owegatts.",
         suffix=".opus",
         delete=False
     )
     tmpfile.close()
-    tts_answer = openai.audio.speech.create(
-        model='tts-1',
-        voice=voice,
-        input=text
-    )
-    tts_answer.write_to_file(tmpfile.name)
+    tts_to_opus(tmpfile.name, text, voice)
     play_opus(tmpfile.name)
     os.remove(tmpfile.name)
 
 
 def estimated_tokens(ppt: str, messages: Conversation, functions: list) -> int:
     """Estimate the history tokens."""
     try:
```

### Comparing `owega-5.9.1/owega.egg-info/PKG-INFO` & `owega-5.9.2/owega.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owega
-Version: 5.9.1
+Version: 5.9.2
 Summary: A command-line interface for conversing with GPT models (from OpenAI)
 Home-page: https://git.pyrokinesis.fr/darkgeem/owega
 Author: darkgeem
 Author-email: darkgeem@pyrokinesis.fr
 License: DGPL-1.0
 Project-URL: Source, https://git.pyrokinesis.fr/darkgeem/owega
 Project-URL: Support, https://discord.gg/KdRmyRrA48
@@ -144,15 +144,15 @@
 ### Demos made with ΦωΦ 5.7.5
 [![asciicast](https://asciinema.org/a/659607.png)](https://asciinema.org/a/659607)
 [Youtube demo](https://youtu.be/_LGSc6mj-EM)
 
 
 ## CHANGELOG: 
 ```
-OWEGA v5.9.1 CHANGELOG:
+OWEGA v5.9.2 CHANGELOG:
 
 
 2.0.0: WTFPL license
 2.0.1: added genconf command
 
 2.1.0: added file_input command
 2.1.1: added file_input in help command
@@ -397,9 +397,10 @@
        files.
 5.8.6: Updated the README with 5.7.5 demos.
 
 5.9.0: Fixed a huge issue where owega couldn't be imported if
        the terminal wasn't interactive.
        Added owega.__version__
 5.9.1: Changed type hinting and fixed some code style!
+5.9.2: Added a tts_to_opus function in owega.utils.
 
 ```
```

### Comparing `owega-5.9.1/owega.egg-info/SOURCES.txt` & `owega-5.9.2/owega.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `owega-5.9.1/setup.py` & `owega-5.9.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """Setup config for installing the package."""
 
 from setuptools import setup
 
-oc_version = '5.9.1'
+oc_version = '5.9.2'
 
 desc = open('README.md').read()
 try:
     changelog = open('CHANGELOG').read()
     desc += '\n\n'
     desc += "## CHANGELOG: "
     desc += '\n```\n'
```

