# Comparing `tmp/owega-5.9.2.tar.gz` & `tmp/owega-5.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owega-5.9.2.tar", last modified: Sun Jun  2 14:24:30 2024, max compression
+gzip compressed data, was "owega-5.9.3.tar", last modified: Sun Jun  2 22:07:49 2024, max compression
```

## Comparing `owega-5.9.2.tar` & `owega-5.9.3.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-06-02 14:24:30.937275 owega-5.9.2/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6076 2024-06-02 14:18:55.000000 owega-5.9.2/LICENSE
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    17508 2024-06-02 14:24:30.936275 owega-5.9.2/PKG-INFO
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5261 2024-06-02 14:18:55.000000 owega-5.9.2/README.md
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-06-02 14:24:30.928275 owega-5.9.2/owega/
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-06-02 14:24:30.933275 owega-5.9.2/owega/OweHandlers/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      156 2024-05-06 16:07:08.000000 owega-5.9.2/owega/OweHandlers/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1309 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_add_sysmem.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1661 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_commands.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1453 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_context.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1895 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_del_sysmem.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2090 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_dinput.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3905 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_edit.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1373 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_estimation.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5526 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_finput.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2194 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_frequency.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      647 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_genconf.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      621 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_history.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3633 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_image.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1460 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_load.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2031 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_model.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2167 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_presence.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      698 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_quit.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1431 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_save.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1273 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_system.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2071 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_temperature.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1456 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_time.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1585 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_tokens.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1846 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_top_p.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1316 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handle_tts.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2609 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OweHandlers/handlers.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-06-02 14:24:30.933275 owega-5.9.2/owega/OwegaFun/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      897 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OwegaFun/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3963 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OwegaFun/functions.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     4383 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OwegaFun/longTermSouvenirs.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5837 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OwegaFun/utility.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-06-02 14:24:30.934275 owega-5.9.2/owega/OwegaSession/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      100 2024-04-17 02:21:38.000000 owega-5.9.2/owega/OwegaSession/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3653 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OwegaSession/main_bottom_toolbar.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6574 2024-06-02 14:18:55.000000 owega-5.9.2/owega/OwegaSession/promptsession.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      247 2024-06-02 14:18:55.000000 owega-5.9.2/owega/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       94 2024-04-17 02:21:38.000000 owega-5.9.2/owega/__main__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10471 2024-06-02 14:18:55.000000 owega-5.9.2/owega/ask.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-06-02 14:24:30.934275 owega-5.9.2/owega/changelog/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       80 2024-05-06 16:07:08.000000 owega-5.9.2/owega/changelog/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    26935 2024-06-02 14:24:00.000000 owega-5.9.2/owega/changelog/changelog.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1581 2024-06-02 14:18:55.000000 owega-5.9.2/owega/changelog/changelogEntry.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3388 2024-06-02 14:18:55.000000 owega-5.9.2/owega/changelog/version.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-06-02 14:24:30.935275 owega-5.9.2/owega/config/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       86 2024-04-17 02:21:38.000000 owega-5.9.2/owega/config/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2659 2024-06-02 14:18:55.000000 owega-5.9.2/owega/config/baseConf.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-06-02 14:24:30.935275 owega-5.9.2/owega/conversation/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       83 2024-04-17 02:21:38.000000 owega-5.9.2/owega/conversation/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10316 2024-06-02 14:18:55.000000 owega-5.9.2/owega/conversation/conversation.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1464 2024-06-02 14:18:55.000000 owega-5.9.2/owega/getLogger.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       64 2024-04-17 02:21:38.000000 owega-5.9.2/owega/handlerBase.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6059 2024-06-02 14:18:55.000000 owega-5.9.2/owega/license.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    12123 2024-06-02 14:18:55.000000 owega-5.9.2/owega/owega.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     7822 2024-06-02 14:21:12.000000 owega-5.9.2/owega/utils.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-06-02 14:24:30.936275 owega-5.9.2/owega.egg-info/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    17508 2024-06-02 14:24:30.000000 owega-5.9.2/owega.egg-info/PKG-INFO
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1689 2024-06-02 14:24:30.000000 owega-5.9.2/owega.egg-info/SOURCES.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        1 2024-06-02 14:24:30.000000 owega-5.9.2/owega.egg-info/dependency_links.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       43 2024-06-02 14:24:30.000000 owega-5.9.2/owega.egg-info/entry_points.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      173 2024-06-02 14:24:30.000000 owega-5.9.2/owega.egg-info/requires.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        6 2024-06-02 14:24:30.000000 owega-5.9.2/owega.egg-info/top_level.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       90 2024-04-17 02:21:38.000000 owega-5.9.2/pyproject.toml
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       38 2024-06-02 14:24:30.937275 owega-5.9.2/setup.cfg
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2573 2024-06-02 14:24:15.000000 owega-5.9.2/setup.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-06-02 22:07:49.842663 owega-5.9.3/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6076 2024-06-02 14:25:55.000000 owega-5.9.3/LICENSE
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    17560 2024-06-02 22:07:49.842663 owega-5.9.3/PKG-INFO
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5261 2024-06-02 14:25:55.000000 owega-5.9.3/README.md
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-06-02 22:07:49.837663 owega-5.9.3/owega/
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-06-02 22:07:49.840663 owega-5.9.3/owega/OweHandlers/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      212 2024-06-02 22:06:03.000000 owega-5.9.3/owega/OweHandlers/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1309 2024-06-02 14:25:55.000000 owega-5.9.3/owega/OweHandlers/handle_add_sysmem.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1661 2024-06-02 14:25:55.000000 owega-5.9.3/owega/OweHandlers/handle_commands.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1453 2024-06-02 14:25:55.000000 owega-5.9.3/owega/OweHandlers/handle_context.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1895 2024-06-02 14:25:55.000000 owega-5.9.3/owega/OweHandlers/handle_del_sysmem.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2090 2024-06-02 14:25:55.000000 owega-5.9.3/owega/OweHandlers/handle_dinput.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3905 2024-06-02 14:25:55.000000 owega-5.9.3/owega/OweHandlers/handle_edit.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1373 2024-06-02 14:25:55.000000 owega-5.9.3/owega/OweHandlers/handle_estimation.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5526 2024-06-02 14:25:55.000000 owega-5.9.3/owega/OweHandlers/handle_finput.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2194 2024-06-02 14:25:55.000000 owega-5.9.3/owega/OweHandlers/handle_frequency.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      647 2024-06-02 14:25:55.000000 owega-5.9.3/owega/OweHandlers/handle_genconf.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      621 2024-06-02 14:25:55.000000 owega-5.9.3/owega/OweHandlers/handle_history.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3633 2024-06-02 14:25:55.000000 owega-5.9.3/owega/OweHandlers/handle_image.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1460 2024-06-02 14:25:55.000000 owega-5.9.3/owega/OweHandlers/handle_load.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2031 2024-06-02 14:25:55.000000 owega-5.9.3/owega/OweHandlers/handle_model.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2167 2024-06-02 14:25:55.000000 owega-5.9.3/owega/OweHandlers/handle_presence.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      698 2024-06-02 14:25:55.000000 owega-5.9.3/owega/OweHandlers/handle_quit.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1431 2024-06-02 14:25:55.000000 owega-5.9.3/owega/OweHandlers/handle_save.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1273 2024-06-02 14:25:55.000000 owega-5.9.3/owega/OweHandlers/handle_system.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2071 2024-06-02 14:25:55.000000 owega-5.9.3/owega/OweHandlers/handle_temperature.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1456 2024-06-02 14:25:55.000000 owega-5.9.3/owega/OweHandlers/handle_time.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1585 2024-06-02 14:25:55.000000 owega-5.9.3/owega/OweHandlers/handle_tokens.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1846 2024-06-02 14:25:55.000000 owega-5.9.3/owega/OweHandlers/handle_top_p.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1316 2024-06-02 14:25:55.000000 owega-5.9.3/owega/OweHandlers/handle_tts.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2609 2024-06-02 14:25:55.000000 owega-5.9.3/owega/OweHandlers/handlers.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-06-02 22:07:49.840663 owega-5.9.3/owega/OwegaFun/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1055 2024-06-02 22:04:59.000000 owega-5.9.3/owega/OwegaFun/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3963 2024-06-02 14:25:55.000000 owega-5.9.3/owega/OwegaFun/functions.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     4383 2024-06-02 14:25:55.000000 owega-5.9.3/owega/OwegaFun/longTermSouvenirs.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5837 2024-06-02 14:25:55.000000 owega-5.9.3/owega/OwegaFun/utility.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-06-02 22:07:49.841663 owega-5.9.3/owega/OwegaSession/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      138 2024-06-02 22:05:23.000000 owega-5.9.3/owega/OwegaSession/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3653 2024-06-02 14:25:55.000000 owega-5.9.3/owega/OwegaSession/main_bottom_toolbar.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6574 2024-06-02 14:25:55.000000 owega-5.9.3/owega/OwegaSession/promptsession.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      276 2024-06-02 22:00:27.000000 owega-5.9.3/owega/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       94 2024-04-17 02:21:38.000000 owega-5.9.3/owega/__main__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10471 2024-06-02 14:25:55.000000 owega-5.9.3/owega/ask.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-06-02 22:07:49.841663 owega-5.9.3/owega/changelog/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      134 2024-06-02 22:02:28.000000 owega-5.9.3/owega/changelog/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    27076 2024-06-02 22:07:33.000000 owega-5.9.3/owega/changelog/changelog.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1581 2024-06-02 14:25:55.000000 owega-5.9.3/owega/changelog/changelogEntry.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3388 2024-06-02 14:25:55.000000 owega-5.9.3/owega/changelog/version.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-06-02 22:07:49.841663 owega-5.9.3/owega/config/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      152 2024-06-02 22:03:02.000000 owega-5.9.3/owega/config/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2659 2024-06-02 14:25:55.000000 owega-5.9.3/owega/config/baseConf.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-06-02 22:07:49.841663 owega-5.9.3/owega/conversation/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      132 2024-06-02 22:03:24.000000 owega-5.9.3/owega/conversation/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10316 2024-06-02 14:25:55.000000 owega-5.9.3/owega/conversation/conversation.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1464 2024-06-02 14:25:55.000000 owega-5.9.3/owega/getLogger.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       64 2024-04-17 02:21:38.000000 owega-5.9.3/owega/handlerBase.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6059 2024-06-02 14:25:55.000000 owega-5.9.3/owega/license.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    12123 2024-06-02 14:25:55.000000 owega-5.9.3/owega/owega.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     7822 2024-06-02 14:25:55.000000 owega-5.9.3/owega/utils.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-06-02 22:07:49.842663 owega-5.9.3/owega.egg-info/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    17560 2024-06-02 22:07:49.000000 owega-5.9.3/owega.egg-info/PKG-INFO
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1689 2024-06-02 22:07:49.000000 owega-5.9.3/owega.egg-info/SOURCES.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        1 2024-06-02 22:07:49.000000 owega-5.9.3/owega.egg-info/dependency_links.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       43 2024-06-02 22:07:49.000000 owega-5.9.3/owega.egg-info/entry_points.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      173 2024-06-02 22:07:49.000000 owega-5.9.3/owega.egg-info/requires.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        6 2024-06-02 22:07:49.000000 owega-5.9.3/owega.egg-info/top_level.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       90 2024-04-17 02:21:38.000000 owega-5.9.3/pyproject.toml
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       38 2024-06-02 22:07:49.842663 owega-5.9.3/setup.cfg
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2573 2024-06-02 22:07:41.000000 owega-5.9.3/setup.py
```

### Comparing `owega-5.9.2/LICENSE` & `owega-5.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/PKG-INFO` & `owega-5.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owega
-Version: 5.9.2
+Version: 5.9.3
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
-OWEGA v5.9.2 CHANGELOG:
+OWEGA v5.9.3 CHANGELOG:
 
 
 2.0.0: WTFPL license
 2.0.1: added genconf command
 
 2.1.0: added file_input command
 2.1.1: added file_input in help command
@@ -398,9 +398,10 @@
 5.8.6: Updated the README with 5.7.5 demos.
 
 5.9.0: Fixed a huge issue where owega couldn't be imported if
        the terminal wasn't interactive.
        Added owega.__version__
 5.9.1: Changed type hinting and fixed some code style!
 5.9.2: Added a tts_to_opus function in owega.utils.
+5.9.3: Added __all__ variable to __init__.py files.
 
 ```
```

### Comparing `owega-5.9.2/README.md` & `owega-5.9.3/README.md`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/owega/OweHandlers/handle_add_sysmem.py` & `owega-5.9.3/owega/OweHandlers/handle_add_sysmem.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/owega/OweHandlers/handle_commands.py` & `owega-5.9.3/owega/OweHandlers/handle_commands.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/owega/OweHandlers/handle_context.py` & `owega-5.9.3/owega/OweHandlers/handle_context.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/owega/OweHandlers/handle_del_sysmem.py` & `owega-5.9.3/owega/OweHandlers/handle_del_sysmem.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/owega/OweHandlers/handle_dinput.py` & `owega-5.9.3/owega/OweHandlers/handle_dinput.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/owega/OweHandlers/handle_edit.py` & `owega-5.9.3/owega/OweHandlers/handle_edit.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/owega/OweHandlers/handle_estimation.py` & `owega-5.9.3/owega/OweHandlers/handle_estimation.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/owega/OweHandlers/handle_finput.py` & `owega-5.9.3/owega/OweHandlers/handle_finput.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/owega/OweHandlers/handle_frequency.py` & `owega-5.9.3/owega/OweHandlers/handle_frequency.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/owega/OweHandlers/handle_genconf.py` & `owega-5.9.3/owega/OweHandlers/handle_genconf.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/owega/OweHandlers/handle_history.py` & `owega-5.9.3/owega/OweHandlers/handle_history.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/owega/OweHandlers/handle_image.py` & `owega-5.9.3/owega/OweHandlers/handle_image.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/owega/OweHandlers/handle_load.py` & `owega-5.9.3/owega/OweHandlers/handle_load.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/owega/OweHandlers/handle_model.py` & `owega-5.9.3/owega/OweHandlers/handle_model.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/owega/OweHandlers/handle_presence.py` & `owega-5.9.3/owega/OweHandlers/handle_presence.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/owega/OweHandlers/handle_quit.py` & `owega-5.9.3/owega/OweHandlers/handle_quit.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/owega/OweHandlers/handle_save.py` & `owega-5.9.3/owega/OweHandlers/handle_save.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/owega/OweHandlers/handle_system.py` & `owega-5.9.3/owega/OweHandlers/handle_system.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/owega/OweHandlers/handle_temperature.py` & `owega-5.9.3/owega/OweHandlers/handle_temperature.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/owega/OweHandlers/handle_time.py` & `owega-5.9.3/owega/OweHandlers/handle_time.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/owega/OweHandlers/handle_tokens.py` & `owega-5.9.3/owega/OweHandlers/handle_tokens.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/owega/OweHandlers/handle_top_p.py` & `owega-5.9.3/owega/OweHandlers/handle_top_p.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/owega/OweHandlers/handle_tts.py` & `owega-5.9.3/owega/OweHandlers/handle_tts.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/owega/OweHandlers/handlers.py` & `owega-5.9.3/owega/OweHandlers/handlers.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/owega/OwegaFun/__init__.py` & `owega-5.9.3/owega/OwegaFun/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,7 +27,18 @@
 
 def functionlist_to_toollist(fun_lst) -> list:
     """Convert a old functions as a tools."""
     tool_lst = []
     for fun in fun_lst:
         tool_lst.append(function_to_tool(fun))
     return tool_lst
+
+
+__all__ = [
+    'lts',
+    'Functions',
+    'Utility',
+    'existingFunctions',
+    'connectLTS',
+    'function_to_tool',
+    'functionlist_to_toollist',
+]
```

### Comparing `owega-5.9.2/owega/OwegaFun/functions.py` & `owega-5.9.3/owega/OwegaFun/functions.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/owega/OwegaFun/longTermSouvenirs.py` & `owega-5.9.3/owega/OwegaFun/longTermSouvenirs.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/owega/OwegaFun/utility.py` & `owega-5.9.3/owega/OwegaFun/utility.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/owega/OwegaSession/main_bottom_toolbar.py` & `owega-5.9.3/owega/OwegaSession/main_bottom_toolbar.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/owega/OwegaSession/promptsession.py` & `owega-5.9.3/owega/OwegaSession/promptsession.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/owega/ask.py` & `owega-5.9.3/owega/ask.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/owega/changelog/changelog.py` & `owega-5.9.3/owega/changelog/changelog.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,18 @@
         self.version = Version(0, 0, 0)
         self.initLogs()
         self.genLog()
 
     def initLogs(self) -> None:
         """Fill the changelog."""
         self.logs.append(
+            ChangelogEntry(5, 9, 3)
+            .addLine("Added __all__ variable to __init__.py files.")
+        )
+        self.logs.append(
             ChangelogEntry(5, 9, 2)
             .addLine("Added a tts_to_opus function in owega.utils.")
         )
         self.logs.append(
             ChangelogEntry(5, 9, 1)
             .addLine("Changed type hinting and fixed some code style!")
         )
```

### Comparing `owega-5.9.2/owega/changelog/changelogEntry.py` & `owega-5.9.3/owega/changelog/changelogEntry.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/owega/changelog/version.py` & `owega-5.9.3/owega/changelog/version.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/owega/config/baseConf.py` & `owega-5.9.3/owega/config/baseConf.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/owega/conversation/conversation.py` & `owega-5.9.3/owega/conversation/conversation.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/owega/getLogger.py` & `owega-5.9.3/owega/getLogger.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/owega/license.py` & `owega-5.9.3/owega/license.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/owega/owega.py` & `owega-5.9.3/owega/owega.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/owega/utils.py` & `owega-5.9.3/owega/utils.py`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/owega.egg-info/PKG-INFO` & `owega-5.9.3/owega.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owega
-Version: 5.9.2
+Version: 5.9.3
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
-OWEGA v5.9.2 CHANGELOG:
+OWEGA v5.9.3 CHANGELOG:
 
 
 2.0.0: WTFPL license
 2.0.1: added genconf command
 
 2.1.0: added file_input command
 2.1.1: added file_input in help command
@@ -398,9 +398,10 @@
 5.8.6: Updated the README with 5.7.5 demos.
 
 5.9.0: Fixed a huge issue where owega couldn't be imported if
        the terminal wasn't interactive.
        Added owega.__version__
 5.9.1: Changed type hinting and fixed some code style!
 5.9.2: Added a tts_to_opus function in owega.utils.
+5.9.3: Added __all__ variable to __init__.py files.
 
 ```
```

### Comparing `owega-5.9.2/owega.egg-info/SOURCES.txt` & `owega-5.9.3/owega.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `owega-5.9.2/setup.py` & `owega-5.9.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """Setup config for installing the package."""
 
 from setuptools import setup
 
-oc_version = '5.9.2'
+oc_version = '5.9.3'
 
 desc = open('README.md').read()
 try:
     changelog = open('CHANGELOG').read()
     desc += '\n\n'
     desc += "## CHANGELOG: "
     desc += '\n```\n'
```

