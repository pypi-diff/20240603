# Comparing `tmp/libresvip-1.1.5.tar.gz` & `tmp/libresvip-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libresvip-1.1.5.tar", last modified: Sun Jun  2 10:14:13 2024, max compression
+gzip compressed data, was "libresvip-1.1.6.tar", last modified: Mon Jun  3 14:46:21 2024, max compression
```

## Comparing `libresvip-1.1.5.tar` & `libresvip-1.1.6.tar`

### file list

```diff
@@ -1,403 +1,403 @@
--rw-r--r--   0        0        0     1093 2024-02-22 15:40:21.193635 libresvip-1.1.5/LICENSE
--rw-r--r--   0        0        0     2562 2024-02-22 15:40:21.193635 libresvip-1.1.5/README.md
--rw-r--r--   0        0        0       87 2024-06-02 09:35:30.009268 libresvip-1.1.5/libresvip/__init__.py
--rw-r--r--   0        0        0      295 2024-04-04 15:32:50.232340 libresvip-1.1.5/libresvip/cli/__init__.py
--rw-r--r--   0        0        0       76 2024-02-22 15:40:21.198477 libresvip-1.1.5/libresvip/cli/__main__.py
--rw-r--r--   0        0        0      213 2024-02-22 15:40:21.198477 libresvip-1.1.5/libresvip/cli/app.py
--rw-r--r--   0        0        0      180 2024-02-22 15:40:21.198477 libresvip-1.1.5/libresvip/cli/commands/__init__.py
--rw-r--r--   0        0        0      862 2024-03-04 16:48:04.970405 libresvip-1.1.5/libresvip/cli/commands/conf.py
--rw-r--r--   0        0        0     6395 2024-03-09 15:39:33.257482 libresvip-1.1.5/libresvip/cli/commands/plugin.py
--rw-r--r--   0        0        0     9237 2024-04-04 15:32:50.233347 libresvip-1.1.5/libresvip/cli/commands/proj.py
--rw-r--r--   0        0        0     3231 2024-04-19 22:32:21.141370 libresvip-1.1.5/libresvip/cli/prompt.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.199452 libresvip-1.1.5/libresvip/core/__init__.py
--rw-r--r--   0        0        0      638 2024-05-30 22:39:39.428800 libresvip-1.1.5/libresvip/core/compat.py
--rw-r--r--   0        0        0     5142 2024-04-26 03:48:21.746001 libresvip-1.1.5/libresvip/core/config.py
--rw-r--r--   0        0        0      635 2024-03-02 16:03:26.993803 libresvip-1.1.5/libresvip/core/constants.py
--rw-r--r--   0        0        0      270 2024-03-04 16:48:04.971414 libresvip-1.1.5/libresvip/core/exceptions.py
--rw-r--r--   0        0        0        2 2024-02-22 15:40:21.201450 libresvip-1.1.5/libresvip/core/lyric_phoneme/__init__.py
--rw-r--r--   0        0        0     2988 2024-03-04 16:48:04.972451 libresvip-1.1.5/libresvip/core/lyric_phoneme/chinese/__init__.py
--rw-r--r--   0        0        0     9449 2024-03-04 16:48:04.973454 libresvip-1.1.5/libresvip/core/lyric_phoneme/chinese/vocaloid_xsampa.py
--rw-r--r--   0        0        0      464 2024-03-12 17:52:45.770726 libresvip-1.1.5/libresvip/core/lyric_phoneme/japanese/__init__.py
--rw-r--r--   0        0        0     2789 2024-03-04 16:48:04.974452 libresvip-1.1.5/libresvip/core/lyric_phoneme/japanese/vocaloid_xsampa.py
--rw-r--r--   0        0        0     1646 2024-02-24 21:21:43.979932 libresvip-1.1.5/libresvip/core/tick_counter.py
--rw-r--r--   0        0        0     5850 2024-03-04 16:48:04.975456 libresvip-1.1.5/libresvip/core/time_interval.py
--rw-r--r--   0        0        0     4280 2024-02-24 21:21:43.979932 libresvip-1.1.5/libresvip/core/time_sync.py
--rw-r--r--   0        0        0     1551 2024-04-04 15:32:50.235346 libresvip-1.1.5/libresvip/core/warning_types.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.203986 libresvip-1.1.5/libresvip/extension/__init__.py
--rw-r--r--   0        0        0      986 2024-03-09 15:39:33.261482 libresvip-1.1.5/libresvip/extension/base.py
--rw-r--r--   0        0        0     7583 2024-03-09 15:39:33.262482 libresvip-1.1.5/libresvip/extension/manager.py
--rw-r--r--   0        0        0     3700 2024-03-09 15:39:33.263482 libresvip-1.1.5/libresvip/extension/meta_info.py
--rw-r--r--   0        0        0    93857 2024-06-02 09:36:02.644492 libresvip-1.1.5/libresvip/gui/__init__.py
--rw-r--r--   0        0        0     1135 2024-05-24 23:54:47.730207 libresvip-1.1.5/libresvip/gui/__main__.py
--rw-r--r--   0        0        0        0 2024-04-04 15:32:50.238347 libresvip-1.1.5/libresvip/gui/models/__init__.py
--rw-r--r--   0        0        0      499 2024-04-04 15:32:50.238347 libresvip-1.1.5/libresvip/gui/models/base_task.py
--rw-r--r--   0        0        0     8893 2024-04-26 15:58:39.835740 libresvip-1.1.5/libresvip/gui/models/list_models.py
--rw-r--r--   0        0        0     7284 2024-04-27 00:43:36.532622 libresvip-1.1.5/libresvip/gui/models/table_models.py
--rw-r--r--   0        0        0      846 2024-05-24 23:18:09.405570 libresvip-1.1.5/libresvip/gui/modules/__init__.py
--rw-r--r--   0        0        0      518 2024-03-26 19:35:54.342244 libresvip-1.1.5/libresvip/gui/modules/application.py
--rw-r--r--   0        0        0      836 2024-05-24 23:45:11.210519 libresvip-1.1.5/libresvip/gui/modules/clipboard.py
--rw-r--r--   0        0        0     5454 2024-06-02 09:32:47.539571 libresvip-1.1.5/libresvip/gui/modules/config_items.py
--rw-r--r--   0        0        0      781 2024-05-24 23:42:54.851057 libresvip-1.1.5/libresvip/gui/modules/font_loader.py
--rw-r--r--   0        0        0     2533 2024-03-04 16:48:04.979510 libresvip-1.1.5/libresvip/gui/modules/frameless_window.py
--rw-r--r--   0        0        0     8815 2024-03-04 16:48:04.980438 libresvip-1.1.5/libresvip/gui/modules/frameless_window_win32.py
--rw-r--r--   0        0        0     2543 2024-05-24 23:53:02.699922 libresvip-1.1.5/libresvip/gui/modules/locale_switcher.py
--rw-r--r--   0        0        0     9920 2024-05-28 17:19:45.078112 libresvip-1.1.5/libresvip/gui/modules/notifier.py
--rw-r--r--   0        0        0    39755 2024-06-01 16:59:35.289899 libresvip-1.1.5/libresvip/gui/modules/task_manager.py
--rw-r--r--   0        0        0      390 2024-02-22 15:40:21.215023 libresvip-1.1.5/libresvip/gui/modules/url_opener.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.215023 libresvip-1.1.5/libresvip/gui/modules/vendor/__init__.py
--rw-r--r--   0        0        0    25262 2024-03-24 06:00:55.521020 libresvip-1.1.5/libresvip/gui/modules/vendor/qasync/__init__.py
--rw-r--r--   0        0        0      497 2024-03-04 16:48:04.983407 libresvip-1.1.5/libresvip/gui/modules/vendor/qasync/_common.py
--rw-r--r--   0        0        0     7507 2024-03-04 16:48:04.984405 libresvip-1.1.5/libresvip/gui/modules/vendor/qasync/_unix.py
--rw-r--r--   0        0        0     9343 2024-05-27 23:07:14.033631 libresvip-1.1.5/libresvip/gui/modules/vendor/qasync/_windows.py
--rw-r--r--   0        0        0      981 2024-02-22 15:40:21.217025 libresvip-1.1.5/libresvip/gui/modules/win32_constants.py
--rw-r--r--   0        0        0        0 2024-03-09 15:39:33.266482 libresvip-1.1.5/libresvip/middlewares/pitch_shift/__init__.py
--rw-r--r--   0        0        0      219 2024-03-09 15:39:33.266482 libresvip-1.1.5/libresvip/middlewares/pitch_shift/options.py
--rw-r--r--   0        0        0     2136 2024-03-09 15:39:33.267482 libresvip-1.1.5/libresvip/middlewares/pitch_shift/pitch_shift.py
--rw-r--r--   0        0        0      181 2024-03-09 15:39:33.267482 libresvip-1.1.5/libresvip/middlewares/pitch_shift/pitch_shift.yapsy-plugin
--rw-r--r--   0        0        0        0 2024-03-09 15:39:33.267482 libresvip-1.1.5/libresvip/middlewares/project_zoom/__init__.py
--rw-r--r--   0        0        0     1009 2024-03-09 15:39:33.267482 libresvip-1.1.5/libresvip/middlewares/project_zoom/options.py
--rw-r--r--   0        0        0      508 2024-03-09 15:39:33.267482 libresvip-1.1.5/libresvip/middlewares/project_zoom/project_zoom.py
--rw-r--r--   0        0        0      220 2024-03-09 15:39:33.269050 libresvip-1.1.5/libresvip/middlewares/project_zoom/project_zoom.yapsy-plugin
--rw-r--r--   0        0        0        0 2024-03-09 15:39:33.269050 libresvip-1.1.5/libresvip/middlewares/pronounciation_conversion/__init__.py
--rw-r--r--   0        0        0      791 2024-03-09 15:39:33.269050 libresvip-1.1.5/libresvip/middlewares/pronounciation_conversion/options.py
--rw-r--r--   0        0        0     1510 2024-03-09 15:39:33.269050 libresvip-1.1.5/libresvip/middlewares/pronounciation_conversion/pronounciation_conversion.py
--rw-r--r--   0        0        0      270 2024-03-09 15:39:33.269989 libresvip-1.1.5/libresvip/middlewares/pronounciation_conversion/pronounciation_conversion.yapsy-plugin
--rw-r--r--   0        0        0        0 2024-03-09 15:39:33.269989 libresvip-1.1.5/libresvip/middlewares/remove_short_silences/__init__.py
--rw-r--r--   0        0        0      882 2024-03-09 15:39:33.269989 libresvip-1.1.5/libresvip/middlewares/remove_short_silences/options.py
--rw-r--r--   0        0        0      953 2024-03-09 15:39:33.270989 libresvip-1.1.5/libresvip/middlewares/remove_short_silences/remove_short_silences.py
--rw-r--r--   0        0        0      243 2024-03-09 15:39:33.270989 libresvip-1.1.5/libresvip/middlewares/remove_short_silences/remove_short_silences.yapsy-plugin
--rw-r--r--   0        0        0        0 2024-04-17 19:53:22.520237 libresvip-1.1.5/libresvip/middlewares/replace_lyric/__init__.py
--rw-r--r--   0        0        0      212 2024-04-19 05:00:08.861563 libresvip-1.1.5/libresvip/middlewares/replace_lyric/options.py
--rw-r--r--   0        0        0     1326 2024-04-27 16:08:27.375841 libresvip-1.1.5/libresvip/middlewares/replace_lyric/replace_lyric.py
--rw-r--r--   0        0        0      319 2024-04-19 21:12:02.082450 libresvip-1.1.5/libresvip/middlewares/replace_lyric/replace_lyric.yapsy-plugin
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.217025 libresvip-1.1.5/libresvip/model/__init__.py
--rw-r--r--   0        0        0    10233 2024-05-19 09:55:57.177960 libresvip-1.1.5/libresvip/model/base.py
--rw-r--r--   0        0        0     1373 2024-03-23 15:29:05.921080 libresvip-1.1.5/libresvip/model/option_mixins.py
--rw-r--r--   0        0        0     3152 2024-02-24 21:21:43.981935 libresvip-1.1.5/libresvip/model/point.py
--rw-r--r--   0        0        0     7529 2024-05-03 03:31:10.216309 libresvip-1.1.5/libresvip/model/relative_pitch_curve.py
--rw-r--r--   0        0        0     7848 2024-03-18 14:03:10.224552 libresvip-1.1.5/libresvip/model/reset_time_axis.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.218004 libresvip-1.1.5/libresvip/plugins/acep/__init__.py
--rw-r--r--   0        0        0    54700 2024-02-22 15:40:21.219535 libresvip-1.1.5/libresvip/plugins/acep/ace-studio.yapsy-plugin
--rw-r--r--   0        0        0     1487 2024-02-22 15:40:21.219535 libresvip-1.1.5/libresvip/plugins/acep/ace_curve_utils.py
--rw-r--r--   0        0        0      949 2024-04-25 14:59:40.397933 libresvip-1.1.5/libresvip/plugins/acep/ace_studio_converter.py
--rw-r--r--   0        0        0    20307 2024-05-20 12:25:55.658809 libresvip-1.1.5/libresvip/plugins/acep/ace_studio_generator.py
--rw-r--r--   0        0        0    17695 2024-05-21 13:15:43.230816 libresvip-1.1.5/libresvip/plugins/acep/ace_studio_parser.py
--rw-r--r--   0        0        0     1620 2024-05-30 22:39:39.429851 libresvip-1.1.5/libresvip/plugins/acep/acep_io.py
--rw-r--r--   0        0        0     5339 2024-03-04 16:48:04.991428 libresvip-1.1.5/libresvip/plugins/acep/base_pitch_curve.py
--rw-r--r--   0        0        0      386 2024-02-22 15:40:21.221571 libresvip-1.1.5/libresvip/plugins/acep/color_pool.py
--rw-r--r--   0        0        0      565 2024-02-24 21:21:43.984931 libresvip-1.1.5/libresvip/plugins/acep/curve_segment_utils.py
--rw-r--r--   0        0        0    14273 2024-05-17 23:01:16.675271 libresvip-1.1.5/libresvip/plugins/acep/model.py
--rw-r--r--   0        0        0    11102 2024-04-04 15:32:50.247348 libresvip-1.1.5/libresvip/plugins/acep/options.py
--rw-r--r--   0        0        0     2518 2024-04-04 15:32:50.248346 libresvip-1.1.5/libresvip/plugins/acep/singers.py
--rw-r--r--   0        0        0     1215 2024-02-22 15:40:21.223573 libresvip-1.1.5/libresvip/plugins/acep/time_utils.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.223573 libresvip-1.1.5/libresvip/plugins/aisp/__init__.py
--rw-r--r--   0        0        0     1486 2024-05-30 22:39:39.430815 libresvip-1.1.5/libresvip/plugins/aisp/aisingers_converter.py
--rw-r--r--   0        0        0     9276 2024-03-04 16:48:04.992962 libresvip-1.1.5/libresvip/plugins/aisp/aisingers_generator.py
--rw-r--r--   0        0        0     4725 2024-03-23 15:29:05.925080 libresvip-1.1.5/libresvip/plugins/aisp/aisingers_parser.py
--rw-r--r--   0        0        0    23952 2024-02-22 15:40:21.224550 libresvip-1.1.5/libresvip/plugins/aisp/aisp.yapsy-plugin
--rw-r--r--   0        0        0     4713 2024-02-22 15:40:21.225582 libresvip-1.1.5/libresvip/plugins/aisp/model.py
--rw-r--r--   0        0        0      325 2024-04-22 06:45:10.507210 libresvip-1.1.5/libresvip/plugins/aisp/options.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.225582 libresvip-1.1.5/libresvip/plugins/ccs/__init__.py
--rw-r--r--   0        0        0    38382 2024-02-22 15:40:21.226575 libresvip-1.1.5/libresvip/plugins/ccs/ccs.yapsy-plugin
--rw-r--r--   0        0        0     1285 2024-05-23 20:52:25.468981 libresvip-1.1.5/libresvip/plugins/ccs/cevio_converter.py
--rw-r--r--   0        0        0     8349 2024-04-04 15:32:50.249954 libresvip-1.1.5/libresvip/plugins/ccs/cevio_generator.py
--rw-r--r--   0        0        0    10117 2024-04-30 12:50:10.287752 libresvip-1.1.5/libresvip/plugins/ccs/cevio_parser.py
--rw-r--r--   0        0        0    17562 2024-05-09 20:53:19.374299 libresvip-1.1.5/libresvip/plugins/ccs/cevio_pitch.py
--rw-r--r--   0        0        0      296 2024-02-22 15:40:21.228574 libresvip-1.1.5/libresvip/plugins/ccs/constants.py
--rw-r--r--   0        0        0    31340 2024-05-23 20:50:28.784086 libresvip-1.1.5/libresvip/plugins/ccs/model.py
--rw-r--r--   0        0        0      567 2024-03-23 15:29:05.927080 libresvip-1.1.5/libresvip/plugins/ccs/options.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.229551 libresvip-1.1.5/libresvip/plugins/ds/__init__.py
--rw-r--r--   0        0        0     6352 2024-02-22 15:40:21.230060 libresvip-1.1.5/libresvip/plugins/ds/dicts/opencpop-extension.txt
--rw-r--r--   0        0        0     4475 2024-02-22 15:40:21.230241 libresvip-1.1.5/libresvip/plugins/ds/dicts/opencpop-strict.txt
--rw-r--r--   0        0        0     4468 2024-02-22 15:40:21.230241 libresvip-1.1.5/libresvip/plugins/ds/dicts/opencpop.txt
--rw-r--r--   0        0        0     2051 2024-05-30 22:39:39.430815 libresvip-1.1.5/libresvip/plugins/ds/diffsinger_converter.py
--rw-r--r--   0        0        0     1846 2024-02-22 15:40:21.231089 libresvip-1.1.5/libresvip/plugins/ds/diffsinger_generator.py
--rw-r--r--   0        0        0     5222 2024-03-23 15:29:05.928079 libresvip-1.1.5/libresvip/plugins/ds/diffsinger_parser.py
--rw-r--r--   0        0        0    31348 2024-02-22 15:40:21.232090 libresvip-1.1.5/libresvip/plugins/ds/ds.yapsy-plugin
--rw-r--r--   0        0        0     3192 2024-02-22 15:40:21.232090 libresvip-1.1.5/libresvip/plugins/ds/model.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.232090 libresvip-1.1.5/libresvip/plugins/ds/models/__init__.py
--rw-r--r--   0        0        0     1292 2024-02-22 15:40:21.233090 libresvip-1.1.5/libresvip/plugins/ds/models/ds_note.py
--rw-r--r--   0        0        0      225 2024-02-22 15:40:21.233090 libresvip-1.1.5/libresvip/plugins/ds/models/ds_param_curve.py
--rw-r--r--   0        0        0      118 2024-02-22 15:40:21.233090 libresvip-1.1.5/libresvip/plugins/ds/models/ds_param_node.py
--rw-r--r--   0        0        0     3205 2024-02-22 15:40:21.233090 libresvip-1.1.5/libresvip/plugins/ds/models/ds_project.py
--rw-r--r--   0        0        0     1984 2024-05-30 22:39:39.431862 libresvip-1.1.5/libresvip/plugins/ds/options.py
--rw-r--r--   0        0        0      786 2024-02-24 21:21:43.986928 libresvip-1.1.5/libresvip/plugins/ds/phoneme_dict.py
--rw-r--r--   0        0        0        2 2024-02-22 15:40:21.234069 libresvip-1.1.5/libresvip/plugins/ds/utils/__init__.py
--rw-r--r--   0        0        0     1452 2024-03-04 16:48:04.996982 libresvip-1.1.5/libresvip/plugins/ds/utils/gender_param_utils.py
--rw-r--r--   0        0        0      294 2024-04-04 23:42:44.572812 libresvip-1.1.5/libresvip/plugins/ds/utils/lyric_util.py
--rw-r--r--   0        0        0     6771 2024-04-04 23:06:53.822302 libresvip-1.1.5/libresvip/plugins/ds/utils/note_list_util.py
--rw-r--r--   0        0        0     1380 2024-02-24 21:21:43.988828 libresvip-1.1.5/libresvip/plugins/ds/utils/pinyin_util.py
--rw-r--r--   0        0        0     1613 2024-02-24 21:21:43.988828 libresvip-1.1.5/libresvip/plugins/ds/utils/pitch_param_utils.py
--rw-r--r--   0        0        0     3990 2024-02-22 15:40:21.236071 libresvip-1.1.5/libresvip/plugins/ds/utils/project_util.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.236071 libresvip-1.1.5/libresvip/plugins/dv/__init__.py
--rw-r--r--   0        0        0    11432 2024-03-04 16:48:04.999015 libresvip-1.1.5/libresvip/plugins/dv/constants.py
--rw-r--r--   0        0        0      847 2024-02-22 15:40:21.237092 libresvip-1.1.5/libresvip/plugins/dv/deepvocal_converter.py
--rw-r--r--   0        0        0    10745 2024-02-22 23:04:58.757287 libresvip-1.1.5/libresvip/plugins/dv/deepvocal_pitch.py
--rw-r--r--   0        0        0     6453 2024-02-22 15:40:21.238069 libresvip-1.1.5/libresvip/plugins/dv/dv.yapsy-plugin
--rw-r--r--   0        0        0     8519 2024-02-24 21:21:43.989880 libresvip-1.1.5/libresvip/plugins/dv/dv_generator.py
--rw-r--r--   0        0        0     6800 2024-03-23 15:29:05.930098 libresvip-1.1.5/libresvip/plugins/dv/dv_parser.py
--rw-r--r--   0        0        0     4927 2024-02-22 15:40:21.239070 libresvip-1.1.5/libresvip/plugins/dv/model.py
--rw-r--r--   0        0        0      325 2024-03-23 15:29:05.931081 libresvip-1.1.5/libresvip/plugins/dv/options.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.239070 libresvip-1.1.5/libresvip/plugins/gj/__init__.py
--rw-r--r--   0        0        0     5113 2024-02-22 15:40:21.239070 libresvip-1.1.5/libresvip/plugins/gj/constants.py
--rw-r--r--   0        0        0    72345 2024-02-22 15:40:21.240660 libresvip-1.1.5/libresvip/plugins/gj/gjgj.yapsy-plugin
--rw-r--r--   0        0        0     1120 2024-05-30 22:39:39.431862 libresvip-1.1.5/libresvip/plugins/gj/gjgj_converter.py
--rw-r--r--   0        0        0    10541 2024-04-04 15:32:50.250856 libresvip-1.1.5/libresvip/plugins/gj/gjgj_generator.py
--rw-r--r--   0        0        0     8051 2024-03-23 15:29:05.933100 libresvip-1.1.5/libresvip/plugins/gj/gjgj_parser.py
--rw-r--r--   0        0        0     6172 2024-02-22 15:40:21.241591 libresvip-1.1.5/libresvip/plugins/gj/model.py
--rw-r--r--   0        0        0      784 2024-03-23 15:29:05.933100 libresvip-1.1.5/libresvip/plugins/gj/options.py
--rw-r--r--   0        0        0      303 2024-02-22 15:40:21.241591 libresvip-1.1.5/libresvip/plugins/gj/singers.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.241591 libresvip-1.1.5/libresvip/plugins/json/__init__.py
--rw-r--r--   0        0        0     1225 2024-02-22 15:40:21.242586 libresvip-1.1.5/libresvip/plugins/json/jsonsvip.yapsy-plugin
--rw-r--r--   0        0        0      965 2024-05-30 22:39:39.432869 libresvip-1.1.5/libresvip/plugins/json/jsonsvip_converter.py
--rw-r--r--   0        0        0      350 2024-02-22 15:40:21.243587 libresvip-1.1.5/libresvip/plugins/json/options.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.243587 libresvip-1.1.5/libresvip/plugins/lrc/__init__.py
--rw-r--r--   0        0        0     1400 2024-02-22 15:40:21.243587 libresvip-1.1.5/libresvip/plugins/lrc/lrc.yapsy-plugin
--rw-r--r--   0        0        0      484 2024-02-22 15:40:21.244588 libresvip-1.1.5/libresvip/plugins/lrc/lrc_converter.py
--rw-r--r--   0        0        0     4320 2024-02-24 21:21:43.990884 libresvip-1.1.5/libresvip/plugins/lrc/lrc_generator.py
--rw-r--r--   0        0        0      670 2024-02-22 15:40:21.244588 libresvip-1.1.5/libresvip/plugins/lrc/model.py
--rw-r--r--   0        0        0     2391 2024-02-22 15:40:21.244588 libresvip-1.1.5/libresvip/plugins/lrc/options.py
--rw-r--r--   0        0        0      692 2024-02-22 15:40:21.245587 libresvip-1.1.5/libresvip/plugins/lrc/template.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.245587 libresvip-1.1.5/libresvip/plugins/mid/__init__.py
--rw-r--r--   0        0        0     1990 2024-02-22 15:40:21.245587 libresvip-1.1.5/libresvip/plugins/mid/constants.py
--rw-r--r--   0        0        0     5992 2024-02-22 15:40:21.246587 libresvip-1.1.5/libresvip/plugins/mid/mid.yapsy-plugin
--rw-r--r--   0        0        0      982 2024-02-24 00:53:21.067110 libresvip-1.1.5/libresvip/plugins/mid/midi_converter.py
--rw-r--r--   0        0        0     6509 2024-03-04 16:48:04.999015 libresvip-1.1.5/libresvip/plugins/mid/midi_generator.py
--rw-r--r--   0        0        0    12410 2024-04-04 15:32:50.251856 libresvip-1.1.5/libresvip/plugins/mid/midi_parser.py
--rw-r--r--   0        0        0     2784 2024-03-04 16:48:05.001983 libresvip-1.1.5/libresvip/plugins/mid/midi_pitch.py
--rw-r--r--   0        0        0      485 2024-02-22 15:40:21.247587 libresvip-1.1.5/libresvip/plugins/mid/note_overlap.py
--rw-r--r--   0        0        0     3008 2024-03-23 15:29:05.936080 libresvip-1.1.5/libresvip/plugins/mid/options.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.247587 libresvip-1.1.5/libresvip/plugins/mtp/__init__.py
--rw-r--r--   0        0        0     5764 2024-02-22 15:40:21.247587 libresvip-1.1.5/libresvip/plugins/mtp/model.py
--rw-r--r--   0        0        0    63944 2024-02-22 15:40:21.248586 libresvip-1.1.5/libresvip/plugins/mtp/mtp.yapsy-plugin
--rw-r--r--   0        0        0      782 2024-02-22 15:40:21.249586 libresvip-1.1.5/libresvip/plugins/mtp/muta_converter.py
--rw-r--r--   0        0        0     7329 2024-05-01 15:16:27.115338 libresvip-1.1.5/libresvip/plugins/mtp/muta_generator.py
--rw-r--r--   0        0        0     5159 2024-05-01 15:02:14.057268 libresvip-1.1.5/libresvip/plugins/mtp/muta_parser.py
--rw-r--r--   0        0        0      495 2024-03-23 15:29:05.938080 libresvip-1.1.5/libresvip/plugins/mtp/options.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.249586 libresvip-1.1.5/libresvip/plugins/musicxml/__init__.py
--rw-r--r--   0        0        0     1375 2024-02-22 15:40:21.249586 libresvip-1.1.5/libresvip/plugins/musicxml/model.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.251137 libresvip-1.1.5/libresvip/plugins/musicxml/models/__init__.py
--rw-r--r--   0        0        0   375282 2024-05-23 20:55:28.214956 libresvip-1.1.5/libresvip/plugins/musicxml/models/mxml2.py
--rw-r--r--   0        0        0     1619 2024-05-23 20:53:46.293368 libresvip-1.1.5/libresvip/plugins/musicxml/models/xlink.py
--rw-r--r--   0        0        0      118 2024-02-22 15:40:21.253184 libresvip-1.1.5/libresvip/plugins/musicxml/models/xml.py
--rw-r--r--   0        0        0    17317 2024-02-22 15:40:21.253184 libresvip-1.1.5/libresvip/plugins/musicxml/musicxml.yapsy-plugin
--rw-r--r--   0        0        0     1634 2024-05-23 20:51:46.276329 libresvip-1.1.5/libresvip/plugins/musicxml/musicxml_converter.py
--rw-r--r--   0        0        0    14877 2024-02-24 21:21:43.993929 libresvip-1.1.5/libresvip/plugins/musicxml/musicxml_generator.py
--rw-r--r--   0        0        0     6295 2024-02-24 21:21:43.993929 libresvip-1.1.5/libresvip/plugins/musicxml/musicxml_parser.py
--rw-r--r--   0        0        0      125 2024-02-22 15:40:21.255194 libresvip-1.1.5/libresvip/plugins/musicxml/options.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.255194 libresvip-1.1.5/libresvip/plugins/nn/__init__.py
--rw-r--r--   0        0        0     4875 2024-02-22 15:40:21.255194 libresvip-1.1.5/libresvip/plugins/nn/model.py
--rw-r--r--   0        0        0     1068 2024-03-23 15:29:05.939080 libresvip-1.1.5/libresvip/plugins/nn/niaoniao_converter.py
--rw-r--r--   0        0        0     5374 2024-03-23 15:29:05.940080 libresvip-1.1.5/libresvip/plugins/nn/niaoniao_generator.py
--rw-r--r--   0        0        0     3564 2024-03-23 15:29:05.940080 libresvip-1.1.5/libresvip/plugins/nn/niaoniao_parser.py
--rw-r--r--   0        0        0    21285 2024-02-22 15:40:21.256182 libresvip-1.1.5/libresvip/plugins/nn/nn.yapsy-plugin
--rw-r--r--   0        0        0      467 2024-03-23 15:29:05.941583 libresvip-1.1.5/libresvip/plugins/nn/options.py
--rw-r--r--   0        0        0     1008 2024-02-22 15:40:21.257195 libresvip-1.1.5/libresvip/plugins/nn/template.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.257195 libresvip-1.1.5/libresvip/plugins/ppsf/__init__.py
--rw-r--r--   0        0        0     7813 2024-02-22 15:40:21.257195 libresvip-1.1.5/libresvip/plugins/ppsf/legacy_model.py
--rw-r--r--   0        0        0    12763 2024-02-22 15:40:21.258193 libresvip-1.1.5/libresvip/plugins/ppsf/model.py
--rw-r--r--   0        0        0      325 2024-03-23 15:29:05.942587 libresvip-1.1.5/libresvip/plugins/ppsf/options.py
--rw-r--r--   0        0        0     1931 2024-05-30 22:39:39.432869 libresvip-1.1.5/libresvip/plugins/ppsf/piapro_studio_converter.py
--rw-r--r--   0        0        0     8331 2024-03-09 15:39:33.271989 libresvip-1.1.5/libresvip/plugins/ppsf/piapro_studio_generator.py
--rw-r--r--   0        0        0     6809 2024-02-22 15:40:21.259204 libresvip-1.1.5/libresvip/plugins/ppsf/piapro_studio_legacy_parser.py
--rw-r--r--   0        0        0     5897 2024-03-23 15:29:05.943588 libresvip-1.1.5/libresvip/plugins/ppsf/piapro_studio_nt_parser.py
--rw-r--r--   0        0        0    19426 2024-02-22 15:40:21.260207 libresvip-1.1.5/libresvip/plugins/ppsf/ppsf.yapsy-plugin
--rw-r--r--   0        0        0     3256 2024-02-24 21:21:43.995835 libresvip-1.1.5/libresvip/plugins/ppsf/ppsf_interval_dict.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.260207 libresvip-1.1.5/libresvip/plugins/s5p/__init__.py
--rw-r--r--   0        0        0     6036 2024-05-08 21:54:55.423825 libresvip-1.1.5/libresvip/plugins/s5p/model.py
--rw-r--r--   0        0        0      344 2024-03-23 15:29:09.443412 libresvip-1.1.5/libresvip/plugins/s5p/options.py
--rw-r--r--   0        0        0    52233 2024-02-22 15:40:21.261194 libresvip-1.1.5/libresvip/plugins/s5p/s5p.yapsy-plugin
--rw-r--r--   0        0        0     1045 2024-05-30 22:39:39.433776 libresvip-1.1.5/libresvip/plugins/s5p/synthv_editor_converter.py
--rw-r--r--   0        0        0     5609 2024-05-08 21:58:19.283039 libresvip-1.1.5/libresvip/plugins/s5p/synthv_editor_generator.py
--rw-r--r--   0        0        0    11617 2024-05-08 21:58:19.283039 libresvip-1.1.5/libresvip/plugins/s5p/synthv_editor_parser.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.262203 libresvip-1.1.5/libresvip/plugins/srt/__init__.py
--rw-r--r--   0        0        0     1394 2024-02-22 15:40:21.262203 libresvip-1.1.5/libresvip/plugins/srt/options.py
--rw-r--r--   0        0        0     1285 2024-02-22 15:40:21.263187 libresvip-1.1.5/libresvip/plugins/srt/srt.yapsy-plugin
--rw-r--r--   0        0        0      503 2024-02-22 15:40:21.263187 libresvip-1.1.5/libresvip/plugins/srt/srt_converter.py
--rw-r--r--   0        0        0     2696 2024-02-24 21:21:43.996926 libresvip-1.1.5/libresvip/plugins/srt/srt_generator.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.263187 libresvip-1.1.5/libresvip/plugins/svg/__init__.py
--rw-r--r--   0        0        0     4552 2024-02-22 15:40:21.264194 libresvip-1.1.5/libresvip/plugins/svg/coordinate_helper.py
--rw-r--r--   0        0        0      279 2024-02-22 15:40:21.264194 libresvip-1.1.5/libresvip/plugins/svg/model.py
--rw-r--r--   0        0        0     3009 2024-02-22 15:40:21.264194 libresvip-1.1.5/libresvip/plugins/svg/options.py
--rw-r--r--   0        0        0    15147 2024-02-22 15:40:21.265188 libresvip-1.1.5/libresvip/plugins/svg/svg.yapsy-plugin
--rw-r--r--   0        0        0      568 2024-02-22 15:40:21.265188 libresvip-1.1.5/libresvip/plugins/svg/svg_converter.py
--rw-r--r--   0        0        0     6739 2024-02-22 15:40:21.265188 libresvip-1.1.5/libresvip/plugins/svg/svg_factory.py
--rw-r--r--   0        0        0     2422 2024-02-22 15:40:21.266243 libresvip-1.1.5/libresvip/plugins/svg/svg_generator.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.266243 libresvip-1.1.5/libresvip/plugins/svip/__init__.py
--rw-r--r--   0        0        0    15042 2024-02-22 15:40:21.266243 libresvip-1.1.5/libresvip/plugins/svip/binsvip.yapsy-plugin
--rw-r--r--   0        0        0     1561 2024-04-25 14:59:53.848685 libresvip-1.1.5/libresvip/plugins/svip/binsvip_converter.py
--rw-r--r--   0        0        0    11038 2024-04-04 23:08:50.052929 libresvip-1.1.5/libresvip/plugins/svip/binsvip_generator.py
--rw-r--r--   0        0        0     5944 2024-03-23 15:29:05.947587 libresvip-1.1.5/libresvip/plugins/svip/binsvip_parser.py
--rw-r--r--   0        0        0     1602 2024-05-30 22:39:39.434769 libresvip-1.1.5/libresvip/plugins/svip/models.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.267240 libresvip-1.1.5/libresvip/plugins/svip/msnrbf/__init__.py
--rw-r--r--   0        0        0    19970 2024-02-24 13:23:26.660918 libresvip-1.1.5/libresvip/plugins/svip/msnrbf/binary_models.py
--rw-r--r--   0        0        0      498 2024-03-04 16:48:05.006115 libresvip-1.1.5/libresvip/plugins/svip/msnrbf/constants.py
--rw-r--r--   0        0        0     1341 2024-03-04 16:48:05.007021 libresvip-1.1.5/libresvip/plugins/svip/msnrbf/nrbf_iobase.py
--rw-r--r--   0        0        0     4956 2024-03-04 16:48:05.007021 libresvip-1.1.5/libresvip/plugins/svip/msnrbf/svip_reader.py
--rw-r--r--   0        0        0    23277 2024-02-22 15:40:21.269238 libresvip-1.1.5/libresvip/plugins/svip/msnrbf/svip_writer.py
--rw-r--r--   0        0        0    15021 2024-04-04 15:32:50.256857 libresvip-1.1.5/libresvip/plugins/svip/msnrbf/xstudio_models.py
--rw-r--r--   0        0        0     3393 2024-03-23 15:29:05.948587 libresvip-1.1.5/libresvip/plugins/svip/options.py
--rw-r--r--   0        0        0     1857 2024-02-22 15:40:21.270241 libresvip-1.1.5/libresvip/plugins/svip/singers.json
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.270241 libresvip-1.1.5/libresvip/plugins/svip3/__init__.py
--rw-r--r--   0        0        0      397 2024-02-22 15:40:21.270241 libresvip-1.1.5/libresvip/plugins/svip3/color_pool.py
--rw-r--r--   0        0        0      396 2024-03-04 16:48:05.009732 libresvip-1.1.5/libresvip/plugins/svip3/constants.py
--rw-r--r--   0        0        0    12712 2024-04-26 16:10:27.006657 libresvip-1.1.5/libresvip/plugins/svip3/model.py
--rw-r--r--   0        0        0      325 2024-03-23 15:29:05.949587 libresvip-1.1.5/libresvip/plugins/svip3/options.py
--rw-r--r--   0        0        0     1647 2024-05-09 20:54:54.690502 libresvip-1.1.5/libresvip/plugins/svip3/singers.json
--rw-r--r--   0        0        0      243 2024-05-30 22:39:39.435769 libresvip-1.1.5/libresvip/plugins/svip3/singers.py
--rw-r--r--   0        0        0    13560 2024-02-22 15:40:21.272276 libresvip-1.1.5/libresvip/plugins/svip3/svip3.yapsy-plugin
--rw-r--r--   0        0        0      782 2024-03-23 15:29:05.950587 libresvip-1.1.5/libresvip/plugins/svip3/svip3_converter.py
--rw-r--r--   0        0        0    11203 2024-04-04 15:32:50.257857 libresvip-1.1.5/libresvip/plugins/svip3/svip3_generator.py
--rw-r--r--   0        0        0     8397 2024-03-23 15:29:05.951587 libresvip-1.1.5/libresvip/plugins/svip3/svip3_parser.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.273244 libresvip-1.1.5/libresvip/plugins/svp/__init__.py
--rw-r--r--   0        0        0      859 2024-02-22 15:40:21.273244 libresvip-1.1.5/libresvip/plugins/svp/constants.py
--rw-r--r--   0        0        0      361 2024-02-22 15:40:21.275243 libresvip-1.1.5/libresvip/plugins/svp/interpolation.py
--rw-r--r--   0        0        0      201 2024-03-14 11:33:30.285334 libresvip-1.1.5/libresvip/plugins/svp/interval_utils.py
--rw-r--r--   0        0        0     1457 2024-02-22 15:40:21.275243 libresvip-1.1.5/libresvip/plugins/svp/lambert_w.py
--rw-r--r--   0        0        0    18008 2024-03-14 13:43:05.687807 libresvip-1.1.5/libresvip/plugins/svp/layer_generator.py
--rw-r--r--   0        0        0    22729 2024-05-20 12:16:53.557264 libresvip-1.1.5/libresvip/plugins/svp/model.py
--rw-r--r--   0        0        0     5769 2024-03-23 15:29:05.952587 libresvip-1.1.5/libresvip/plugins/svp/options.py
--rw-r--r--   0        0        0     9582 2024-03-04 16:48:05.013673 libresvip-1.1.5/libresvip/plugins/svp/param_expression.py
--rw-r--r--   0        0        0     2901 2024-02-22 15:40:21.277240 libresvip-1.1.5/libresvip/plugins/svp/phoneme_categories.json
--rw-r--r--   0        0        0    57860 2024-02-22 15:40:21.278256 libresvip-1.1.5/libresvip/plugins/svp/phoneme_dictionary.json
--rw-r--r--   0        0        0     3281 2024-05-30 22:39:39.435769 libresvip-1.1.5/libresvip/plugins/svp/phoneme_utils.py
--rw-r--r--   0        0        0     3651 2024-02-24 21:21:44.000940 libresvip-1.1.5/libresvip/plugins/svp/pitch_simulator.py
--rw-r--r--   0        0        0      870 2024-02-22 15:40:21.279241 libresvip-1.1.5/libresvip/plugins/svp/pitch_slide.py
--rw-r--r--   0        0        0    41585 2024-02-22 15:40:21.279241 libresvip-1.1.5/libresvip/plugins/svp/svp.yapsy-plugin
--rw-r--r--   0        0        0    21945 2024-03-09 15:39:33.275988 libresvip-1.1.5/libresvip/plugins/svp/synthv_generator.py
--rw-r--r--   0        0        0    29652 2024-05-19 06:30:29.934521 libresvip-1.1.5/libresvip/plugins/svp/synthv_parser.py
--rw-r--r--   0        0        0     1182 2024-05-30 22:39:39.435769 libresvip-1.1.5/libresvip/plugins/svp/synthv_studio_converter.py
--rw-r--r--   0        0        0     7049 2024-03-04 16:48:05.016732 libresvip-1.1.5/libresvip/plugins/svp/track_merge_utils.py
--rw-r--r--   0        0        0        0 2024-04-20 08:41:44.970999 libresvip-1.1.5/libresvip/plugins/tlp/__init__.py
--rw-r--r--   0        0        0     5766 2024-06-01 11:50:47.704346 libresvip-1.1.5/libresvip/plugins/tlp/model.py
--rw-r--r--   0        0        0      325 2024-04-29 22:55:41.750988 libresvip-1.1.5/libresvip/plugins/tlp/options.py
--rw-r--r--   0        0        0      253 2024-04-30 20:13:41.439220 libresvip-1.1.5/libresvip/plugins/tlp/tlp.yapsy-plugin
--rw-r--r--   0        0        0     1016 2024-05-30 22:39:39.437283 libresvip-1.1.5/libresvip/plugins/tlp/tunelab_converter.py
--rw-r--r--   0        0        0     5345 2024-05-30 04:59:53.935499 libresvip-1.1.5/libresvip/plugins/tlp/tunelab_generator.py
--rw-r--r--   0        0        0     8532 2024-05-19 12:17:21.995853 libresvip-1.1.5/libresvip/plugins/tlp/tunelab_parser.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.281548 libresvip-1.1.5/libresvip/plugins/tssln/__init__.py
--rw-r--r--   0        0        0      258 2024-02-22 15:40:21.281548 libresvip-1.1.5/libresvip/plugins/tssln/constants.py
--rw-r--r--   0        0        0    14287 2024-03-04 16:48:05.018348 libresvip-1.1.5/libresvip/plugins/tssln/model.py
--rw-r--r--   0        0        0      325 2024-03-23 15:29:05.954587 libresvip-1.1.5/libresvip/plugins/tssln/options.py
--rw-r--r--   0        0        0    20418 2024-02-22 15:40:21.283497 libresvip-1.1.5/libresvip/plugins/tssln/tssln.yapsy-plugin
--rw-r--r--   0        0        0     3829 2024-02-24 13:21:27.902046 libresvip-1.1.5/libresvip/plugins/tssln/value_tree.py
--rw-r--r--   0        0        0     1032 2024-02-22 15:40:21.283497 libresvip-1.1.5/libresvip/plugins/tssln/voisona_converter.py
--rw-r--r--   0        0        0     6553 2024-04-04 15:32:50.258857 libresvip-1.1.5/libresvip/plugins/tssln/voisona_generator.py
--rw-r--r--   0        0        0     8686 2024-05-07 19:56:46.445386 libresvip-1.1.5/libresvip/plugins/tssln/voisona_parser.py
--rw-r--r--   0        0        0    17668 2024-05-09 20:53:32.087863 libresvip-1.1.5/libresvip/plugins/tssln/voisona_pitch.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.284496 libresvip-1.1.5/libresvip/plugins/ufdata/__init__.py
--rw-r--r--   0        0        0     1286 2024-04-04 15:32:50.261367 libresvip-1.1.5/libresvip/plugins/ufdata/model.py
--rw-r--r--   0        0        0      125 2024-02-22 15:40:21.285497 libresvip-1.1.5/libresvip/plugins/ufdata/options.py
--rw-r--r--   0        0        0    25204 2024-04-30 20:11:46.826346 libresvip-1.1.5/libresvip/plugins/ufdata/ufdata.yapsy-plugin
--rw-r--r--   0        0        0     1005 2024-05-30 22:39:39.437283 libresvip-1.1.5/libresvip/plugins/ufdata/ufdata_converter.py
--rw-r--r--   0        0        0     3019 2024-03-04 16:48:05.021992 libresvip-1.1.5/libresvip/plugins/ufdata/ufdata_generator.py
--rw-r--r--   0        0        0     4414 2024-04-04 15:32:50.263369 libresvip-1.1.5/libresvip/plugins/ufdata/ufdata_parser.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.287504 libresvip-1.1.5/libresvip/plugins/ust/__init__.py
--rw-r--r--   0        0        0      220 2024-02-22 15:40:21.287504 libresvip-1.1.5/libresvip/plugins/ust/constants.py
--rw-r--r--   0        0        0      859 2024-02-22 15:40:21.288508 libresvip-1.1.5/libresvip/plugins/ust/interpolation.py
--rw-r--r--   0        0        0    17060 2024-03-11 13:13:40.358282 libresvip-1.1.5/libresvip/plugins/ust/model.py
--rw-r--r--   0        0        0      614 2024-04-19 22:30:20.059096 libresvip-1.1.5/libresvip/plugins/ust/options.py
--rw-r--r--   0        0        0     2060 2024-04-04 15:32:50.264367 libresvip-1.1.5/libresvip/plugins/ust/pitch_mode1.py
--rw-r--r--   0        0        0     9626 2024-06-01 22:10:27.094691 libresvip-1.1.5/libresvip/plugins/ust/pitch_mode2.py
--rw-r--r--   0        0        0     1781 2024-02-22 15:40:21.289493 libresvip-1.1.5/libresvip/plugins/ust/rdp_simplification.py
--rw-r--r--   0        0        0     1076 2024-03-04 16:48:05.024002 libresvip-1.1.5/libresvip/plugins/ust/resampling.py
--rw-r--r--   0        0        0     3600 2024-02-22 15:40:21.290497 libresvip-1.1.5/libresvip/plugins/ust/template.py
--rw-r--r--   0        0        0     8187 2024-02-22 15:40:21.291513 libresvip-1.1.5/libresvip/plugins/ust/ust.yapsy-plugin
--rw-r--r--   0        0        0      940 2024-04-19 22:31:18.927764 libresvip-1.1.5/libresvip/plugins/ust/ust_converter.py
--rw-r--r--   0        0        0     4545 2024-03-11 21:42:10.409173 libresvip-1.1.5/libresvip/plugins/ust/ust_generator.py
--rw-r--r--   0        0        0     6093 2024-03-23 15:29:05.958094 libresvip-1.1.5/libresvip/plugins/ust/ust_parser.py
--rw-r--r--   0        0        0     3270 2024-06-01 22:20:22.609727 libresvip-1.1.5/libresvip/plugins/ust/vibrato_param.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.292072 libresvip-1.1.5/libresvip/plugins/ustx/__init__.py
--rw-r--r--   0        0        0     6283 2024-03-04 16:48:05.024934 libresvip-1.1.5/libresvip/plugins/ustx/model.py
--rw-r--r--   0        0        0      325 2024-03-23 15:29:05.959093 libresvip-1.1.5/libresvip/plugins/ustx/options.py
--rw-r--r--   0        0        0    45293 2024-02-22 15:40:21.294124 libresvip-1.1.5/libresvip/plugins/ustx/ustx.yapsy-plugin
--rw-r--r--   0        0        0     1061 2024-03-12 19:57:09.206525 libresvip-1.1.5/libresvip/plugins/ustx/ustx_converter.py
--rw-r--r--   0        0        0     8246 2024-04-04 23:03:45.113941 libresvip-1.1.5/libresvip/plugins/ustx/ustx_generator.py
--rw-r--r--   0        0        0     7048 2024-03-23 15:29:05.960094 libresvip-1.1.5/libresvip/plugins/ustx/ustx_parser.py
--rw-r--r--   0        0        0     4584 2024-03-11 13:13:40.361335 libresvip-1.1.5/libresvip/plugins/ustx/util.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.295117 libresvip-1.1.5/libresvip/plugins/ustx/utils/__init__.py
--rw-r--r--   0        0        0      407 2024-04-05 21:59:21.996830 libresvip-1.1.5/libresvip/plugins/ustx/utils/lyric_util.py
--rw-r--r--   0        0        0      634 2024-02-24 21:21:44.007536 libresvip-1.1.5/libresvip/plugins/ustx/utils/music_math.py
--rw-r--r--   0        0        0     6102 2024-02-22 15:40:21.296134 libresvip-1.1.5/libresvip/plugins/ustx/utils/time_axis.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.296134 libresvip-1.1.5/libresvip/plugins/vog/__init__.py
--rw-r--r--   0        0        0      766 2024-02-22 15:40:21.297120 libresvip-1.1.5/libresvip/plugins/vog/model.py
--rw-r--r--   0        0        0      359 2024-03-23 15:29:05.960094 libresvip-1.1.5/libresvip/plugins/vog/options.py
--rw-r--r--   0        0        0    63065 2024-02-22 15:40:21.298121 libresvip-1.1.5/libresvip/plugins/vog/vog.yapsy-plugin
--rw-r--r--   0        0        0     1347 2024-05-30 22:39:39.438300 libresvip-1.1.5/libresvip/plugins/vog/vogen_converter.py
--rw-r--r--   0        0        0     1922 2024-03-18 14:02:32.510275 libresvip-1.1.5/libresvip/plugins/vog/vogen_generator.py
--rw-r--r--   0        0        0     1658 2024-02-22 15:40:21.299208 libresvip-1.1.5/libresvip/plugins/vog/vogen_parser.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.299208 libresvip-1.1.5/libresvip/plugins/vpr/__init__.py
--rw-r--r--   0        0        0      434 2024-03-04 16:48:05.027944 libresvip-1.1.5/libresvip/plugins/vpr/constants.py
--rw-r--r--   0        0        0     9840 2024-02-22 15:40:21.300231 libresvip-1.1.5/libresvip/plugins/vpr/model.py
--rw-r--r--   0        0        0     1285 2024-03-23 15:29:05.962094 libresvip-1.1.5/libresvip/plugins/vpr/options.py
--rw-r--r--   0        0        0     4847 2024-03-04 16:48:05.029005 libresvip-1.1.5/libresvip/plugins/vpr/vocaloid_pitch.py
--rw-r--r--   0        0        0    14147 2024-02-22 15:40:21.300231 libresvip-1.1.5/libresvip/plugins/vpr/vpr.yapsy-plugin
--rw-r--r--   0        0        0     1515 2024-05-30 22:39:39.438300 libresvip-1.1.5/libresvip/plugins/vpr/vpr_converter.py
--rw-r--r--   0        0        0    10082 2024-04-04 15:32:50.267366 libresvip-1.1.5/libresvip/plugins/vpr/vpr_generator.py
--rw-r--r--   0        0        0     6440 2024-03-23 15:29:05.963094 libresvip-1.1.5/libresvip/plugins/vpr/vpr_parser.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.302894 libresvip-1.1.5/libresvip/plugins/vshp/__init__.py
--rw-r--r--   0        0        0     5774 2024-02-22 15:40:21.303892 libresvip-1.1.5/libresvip/plugins/vshp/model.py
--rw-r--r--   0        0        0      532 2024-02-22 15:40:21.303892 libresvip-1.1.5/libresvip/plugins/vshp/options.py
--rw-r--r--   0        0        0      351 2024-02-22 15:40:21.304891 libresvip-1.1.5/libresvip/plugins/vshp/utils.py
--rw-r--r--   0        0        0      522 2024-02-22 15:40:21.304891 libresvip-1.1.5/libresvip/plugins/vshp/vocalshifter_converter.py
--rw-r--r--   0        0        0     9770 2024-05-12 02:56:26.310999 libresvip-1.1.5/libresvip/plugins/vshp/vocalshifter_parser.py
--rw-r--r--   0        0        0     9560 2024-03-05 19:32:37.534334 libresvip-1.1.5/libresvip/plugins/vshp/vshp.yapsy-plugin
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.305892 libresvip-1.1.5/libresvip/plugins/vspx/__init__.py
--rw-r--r--   0        0        0    12260 2024-05-23 21:06:19.766400 libresvip-1.1.5/libresvip/plugins/vspx/model.py
--rw-r--r--   0        0        0      325 2024-03-23 15:29:05.965117 libresvip-1.1.5/libresvip/plugins/vspx/options.py
--rw-r--r--   0        0        0     2794 2024-05-23 20:51:26.669246 libresvip-1.1.5/libresvip/plugins/vspx/vocalsharp_converter.py
--rw-r--r--   0        0        0     5428 2024-02-22 15:40:21.307892 libresvip-1.1.5/libresvip/plugins/vspx/vspx.yapsy-plugin
--rw-r--r--   0        0        0     7072 2024-02-24 21:21:44.010521 libresvip-1.1.5/libresvip/plugins/vspx/vspx_generator.py
--rw-r--r--   0        0        0     8035 2024-03-04 16:48:05.031947 libresvip-1.1.5/libresvip/plugins/vspx/vspx_interval_dict.py
--rw-r--r--   0        0        0     5857 2024-03-23 15:29:05.966101 libresvip-1.1.5/libresvip/plugins/vspx/vspx_parser.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.308892 libresvip-1.1.5/libresvip/plugins/vsq/__init__.py
--rw-r--r--   0        0        0      246 2024-03-04 16:48:05.031947 libresvip-1.1.5/libresvip/plugins/vsq/constants.py
--rw-r--r--   0        0        0     1257 2024-03-23 15:29:05.966101 libresvip-1.1.5/libresvip/plugins/vsq/options.py
--rw-r--r--   0        0        0     5055 2024-03-04 16:48:05.032934 libresvip-1.1.5/libresvip/plugins/vsq/vocaloid_pitch.py
--rw-r--r--   0        0        0    49554 2024-02-22 15:40:21.310892 libresvip-1.1.5/libresvip/plugins/vsq/vsq.yapsy-plugin
--rw-r--r--   0        0        0      957 2024-02-22 15:40:21.310892 libresvip-1.1.5/libresvip/plugins/vsq/vsq_converter.py
--rw-r--r--   0        0        0     8510 2024-03-04 16:48:05.033991 libresvip-1.1.5/libresvip/plugins/vsq/vsq_generator.py
--rw-r--r--   0        0        0     8932 2024-05-13 23:51:28.744089 libresvip-1.1.5/libresvip/plugins/vsq/vsq_parser.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.310892 libresvip-1.1.5/libresvip/plugins/vsqx/__init__.py
--rw-r--r--   0        0        0      332 2024-03-04 16:48:05.034998 libresvip-1.1.5/libresvip/plugins/vsqx/constants.py
--rw-r--r--   0        0        0      566 2024-03-23 15:29:05.968632 libresvip-1.1.5/libresvip/plugins/vsqx/enums.py
--rw-r--r--   0        0        0     4400 2024-02-22 15:40:21.312399 libresvip-1.1.5/libresvip/plugins/vsqx/model.py
--rw-r--r--   0        0        0        2 2024-02-22 15:40:21.312399 libresvip-1.1.5/libresvip/plugins/vsqx/models/__init__.py
--rw-r--r--   0        0        0    36021 2024-05-23 20:45:39.085386 libresvip-1.1.5/libresvip/plugins/vsqx/models/vsqx3.py
--rw-r--r--   0        0        0    32062 2024-05-23 20:45:58.846501 libresvip-1.1.5/libresvip/plugins/vsqx/models/vsqx4.py
--rw-r--r--   0        0        0     1078 2024-03-23 15:29:05.969611 libresvip-1.1.5/libresvip/plugins/vsqx/options.py
--rw-r--r--   0        0        0     6353 2024-05-12 21:40:04.381986 libresvip-1.1.5/libresvip/plugins/vsqx/vocaloid_pitch.py
--rw-r--r--   0        0        0    10117 2024-04-04 15:32:50.268367 libresvip-1.1.5/libresvip/plugins/vsqx/vsq3_generator.py
--rw-r--r--   0        0        0    10118 2024-04-04 15:32:50.269366 libresvip-1.1.5/libresvip/plugins/vsqx/vsq4_generator.py
--rw-r--r--   0        0        0    49665 2024-02-22 15:40:21.315408 libresvip-1.1.5/libresvip/plugins/vsqx/vsqx.yapsy-plugin
--rw-r--r--   0        0        0     3151 2024-05-23 20:51:08.663436 libresvip-1.1.5/libresvip/plugins/vsqx/vsqx_converter.py
--rw-r--r--   0        0        0    13947 2024-05-12 21:44:45.964936 libresvip-1.1.5/libresvip/plugins/vsqx/vsqx_parser.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.316410 libresvip-1.1.5/libresvip/plugins/y77/__init__.py
--rw-r--r--   0        0        0      742 2024-02-22 15:40:21.316410 libresvip-1.1.5/libresvip/plugins/y77/model.py
--rw-r--r--   0        0        0      321 2024-03-23 15:29:05.971609 libresvip-1.1.5/libresvip/plugins/y77/options.py
--rw-r--r--   0        0        0    48980 2024-02-22 15:40:21.317409 libresvip-1.1.5/libresvip/plugins/y77/y77.yapsy-plugin
--rw-r--r--   0        0        0     1042 2024-05-30 22:39:39.439292 libresvip-1.1.5/libresvip/plugins/y77/y77_converter.py
--rw-r--r--   0        0        0     3963 2024-03-18 14:02:43.305455 libresvip-1.1.5/libresvip/plugins/y77/y77_generator.py
--rw-r--r--   0        0        0     3190 2024-03-23 15:29:05.973610 libresvip-1.1.5/libresvip/plugins/y77/y77_parser.py
--rw-r--r--   0        0        0        0 2024-04-03 00:40:49.030321 libresvip-1.1.5/libresvip/py.typed
--rw-r--r--   0        0        0   270398 2024-02-22 15:40:21.319450 libresvip-1.1.5/libresvip/res/libresvip.ico
--rw-r--r--   0        0        0    54799 2024-05-19 09:30:40.522879 libresvip-1.1.5/libresvip/res/locales/zh_CN/LC_MESSAGES/libresvip.mo
--rw-r--r--   0        0        0        0 2024-02-24 21:21:44.013149 libresvip-1.1.5/libresvip/utils/__init__.py
--rw-r--r--   0        0        0     1623 2024-05-30 19:32:16.905621 libresvip-1.1.5/libresvip/utils/audio.py
--rw-r--r--   0        0        0     2441 2024-03-04 16:48:05.048671 libresvip-1.1.5/libresvip/utils/module_loading.py
--rw-r--r--   0        0        0     3970 2024-03-04 16:48:05.049643 libresvip-1.1.5/libresvip/utils/music_math.py
--rw-r--r--   0        0        0     1129 2024-02-24 21:21:44.014264 libresvip-1.1.5/libresvip/utils/search.py
--rw-r--r--   0        0        0     3309 2024-05-19 06:30:15.423045 libresvip-1.1.5/libresvip/utils/text.py
--rw-r--r--   0        0        0     1627 2024-04-17 18:48:56.821252 libresvip-1.1.5/libresvip/utils/translation.py
--rw-r--r--   0        0        0     1015 2024-04-03 23:14:53.055643 libresvip-1.1.5/libresvip/utils/xmlutils/__init__.py
--rw-r--r--   0        0        0     1013 2024-04-19 21:54:15.974691 libresvip-1.1.5/libresvip/utils/xmlutils/native.py
--rw-r--r--   0        0        0      942 2024-03-12 20:28:45.735172 libresvip-1.1.5/libresvip/utils/yamlutils/__init__.py
--rw-r--r--   0        0        0     2833 2024-03-24 06:01:39.945387 libresvip-1.1.5/libresvip/utils/yamlutils/common.py
--rw-r--r--   0        0        0     3873 2024-03-24 06:01:51.194427 libresvip-1.1.5/libresvip/utils/yamlutils/dumper.py
--rw-r--r--   0        0        0     5052 2024-03-04 16:48:05.053289 libresvip-1.1.5/libresvip/utils/yamlutils/loader.py
--rw-r--r--   0        0        0      152 2024-04-17 14:03:30.170610 libresvip-1.1.5/libresvip/web/__init__.py
--rw-r--r--   0        0        0       97 2024-03-01 21:51:25.393182 libresvip-1.1.5/libresvip/web/__main__.py
--rw-r--r--   0        0        0     2344 2024-03-01 21:51:25.394220 libresvip-1.1.5/libresvip/web/elements.py
--rw-r--r--   0        0        0    96849 2024-05-28 17:11:01.243572 libresvip-1.1.5/libresvip/web/pages.py
--rw-r--r--   0        0        0     5338 2024-06-02 10:14:13.793532 libresvip-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     6029 1970-01-01 00:00:00.000000 libresvip-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1093 2024-02-22 15:40:21.193635 libresvip-1.1.6/LICENSE
+-rw-r--r--   0        0        0     2562 2024-02-22 15:40:21.193635 libresvip-1.1.6/README.md
+-rw-r--r--   0        0        0       87 2024-06-03 13:35:27.625554 libresvip-1.1.6/libresvip/__init__.py
+-rw-r--r--   0        0        0      295 2024-04-04 15:32:50.232340 libresvip-1.1.6/libresvip/cli/__init__.py
+-rw-r--r--   0        0        0       76 2024-02-22 15:40:21.198477 libresvip-1.1.6/libresvip/cli/__main__.py
+-rw-r--r--   0        0        0      213 2024-02-22 15:40:21.198477 libresvip-1.1.6/libresvip/cli/app.py
+-rw-r--r--   0        0        0      180 2024-02-22 15:40:21.198477 libresvip-1.1.6/libresvip/cli/commands/__init__.py
+-rw-r--r--   0        0        0      862 2024-03-04 16:48:04.970405 libresvip-1.1.6/libresvip/cli/commands/conf.py
+-rw-r--r--   0        0        0     6395 2024-03-09 15:39:33.257482 libresvip-1.1.6/libresvip/cli/commands/plugin.py
+-rw-r--r--   0        0        0     9237 2024-04-04 15:32:50.233347 libresvip-1.1.6/libresvip/cli/commands/proj.py
+-rw-r--r--   0        0        0     3231 2024-04-19 22:32:21.141370 libresvip-1.1.6/libresvip/cli/prompt.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.199452 libresvip-1.1.6/libresvip/core/__init__.py
+-rw-r--r--   0        0        0      638 2024-05-30 22:39:39.428800 libresvip-1.1.6/libresvip/core/compat.py
+-rw-r--r--   0        0        0     5142 2024-04-26 03:48:21.746001 libresvip-1.1.6/libresvip/core/config.py
+-rw-r--r--   0        0        0      635 2024-03-02 16:03:26.993803 libresvip-1.1.6/libresvip/core/constants.py
+-rw-r--r--   0        0        0      270 2024-03-04 16:48:04.971414 libresvip-1.1.6/libresvip/core/exceptions.py
+-rw-r--r--   0        0        0        2 2024-02-22 15:40:21.201450 libresvip-1.1.6/libresvip/core/lyric_phoneme/__init__.py
+-rw-r--r--   0        0        0     2988 2024-03-04 16:48:04.972451 libresvip-1.1.6/libresvip/core/lyric_phoneme/chinese/__init__.py
+-rw-r--r--   0        0        0     9449 2024-03-04 16:48:04.973454 libresvip-1.1.6/libresvip/core/lyric_phoneme/chinese/vocaloid_xsampa.py
+-rw-r--r--   0        0        0      464 2024-03-12 17:52:45.770726 libresvip-1.1.6/libresvip/core/lyric_phoneme/japanese/__init__.py
+-rw-r--r--   0        0        0     2789 2024-03-04 16:48:04.974452 libresvip-1.1.6/libresvip/core/lyric_phoneme/japanese/vocaloid_xsampa.py
+-rw-r--r--   0        0        0     1646 2024-02-24 21:21:43.979932 libresvip-1.1.6/libresvip/core/tick_counter.py
+-rw-r--r--   0        0        0     5850 2024-03-04 16:48:04.975456 libresvip-1.1.6/libresvip/core/time_interval.py
+-rw-r--r--   0        0        0     4280 2024-02-24 21:21:43.979932 libresvip-1.1.6/libresvip/core/time_sync.py
+-rw-r--r--   0        0        0     1551 2024-04-04 15:32:50.235346 libresvip-1.1.6/libresvip/core/warning_types.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.203986 libresvip-1.1.6/libresvip/extension/__init__.py
+-rw-r--r--   0        0        0      986 2024-03-09 15:39:33.261482 libresvip-1.1.6/libresvip/extension/base.py
+-rw-r--r--   0        0        0     7583 2024-03-09 15:39:33.262482 libresvip-1.1.6/libresvip/extension/manager.py
+-rw-r--r--   0        0        0     3700 2024-03-09 15:39:33.263482 libresvip-1.1.6/libresvip/extension/meta_info.py
+-rw-r--r--   0        0        0    93940 2024-06-03 13:28:08.958958 libresvip-1.1.6/libresvip/gui/__init__.py
+-rw-r--r--   0        0        0     1135 2024-05-24 23:54:47.730207 libresvip-1.1.6/libresvip/gui/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-04 15:32:50.238347 libresvip-1.1.6/libresvip/gui/models/__init__.py
+-rw-r--r--   0        0        0      499 2024-04-04 15:32:50.238347 libresvip-1.1.6/libresvip/gui/models/base_task.py
+-rw-r--r--   0        0        0     8893 2024-04-26 15:58:39.835740 libresvip-1.1.6/libresvip/gui/models/list_models.py
+-rw-r--r--   0        0        0     7284 2024-04-27 00:43:36.532622 libresvip-1.1.6/libresvip/gui/models/table_models.py
+-rw-r--r--   0        0        0      846 2024-05-24 23:18:09.405570 libresvip-1.1.6/libresvip/gui/modules/__init__.py
+-rw-r--r--   0        0        0      518 2024-03-26 19:35:54.342244 libresvip-1.1.6/libresvip/gui/modules/application.py
+-rw-r--r--   0        0        0      836 2024-05-24 23:45:11.210519 libresvip-1.1.6/libresvip/gui/modules/clipboard.py
+-rw-r--r--   0        0        0     4804 2024-06-03 13:24:06.931202 libresvip-1.1.6/libresvip/gui/modules/config_items.py
+-rw-r--r--   0        0        0      781 2024-05-24 23:42:54.851057 libresvip-1.1.6/libresvip/gui/modules/font_loader.py
+-rw-r--r--   0        0        0     2533 2024-03-04 16:48:04.979510 libresvip-1.1.6/libresvip/gui/modules/frameless_window.py
+-rw-r--r--   0        0        0     8815 2024-03-04 16:48:04.980438 libresvip-1.1.6/libresvip/gui/modules/frameless_window_win32.py
+-rw-r--r--   0        0        0     2543 2024-05-24 23:53:02.699922 libresvip-1.1.6/libresvip/gui/modules/locale_switcher.py
+-rw-r--r--   0        0        0     9920 2024-05-28 17:19:45.078112 libresvip-1.1.6/libresvip/gui/modules/notifier.py
+-rw-r--r--   0        0        0    40426 2024-06-03 13:25:23.581054 libresvip-1.1.6/libresvip/gui/modules/task_manager.py
+-rw-r--r--   0        0        0      390 2024-02-22 15:40:21.215023 libresvip-1.1.6/libresvip/gui/modules/url_opener.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.215023 libresvip-1.1.6/libresvip/gui/modules/vendor/__init__.py
+-rw-r--r--   0        0        0    25262 2024-03-24 06:00:55.521020 libresvip-1.1.6/libresvip/gui/modules/vendor/qasync/__init__.py
+-rw-r--r--   0        0        0      497 2024-03-04 16:48:04.983407 libresvip-1.1.6/libresvip/gui/modules/vendor/qasync/_common.py
+-rw-r--r--   0        0        0     7507 2024-03-04 16:48:04.984405 libresvip-1.1.6/libresvip/gui/modules/vendor/qasync/_unix.py
+-rw-r--r--   0        0        0     9343 2024-05-27 23:07:14.033631 libresvip-1.1.6/libresvip/gui/modules/vendor/qasync/_windows.py
+-rw-r--r--   0        0        0      981 2024-02-22 15:40:21.217025 libresvip-1.1.6/libresvip/gui/modules/win32_constants.py
+-rw-r--r--   0        0        0        0 2024-03-09 15:39:33.266482 libresvip-1.1.6/libresvip/middlewares/pitch_shift/__init__.py
+-rw-r--r--   0        0        0      219 2024-03-09 15:39:33.266482 libresvip-1.1.6/libresvip/middlewares/pitch_shift/options.py
+-rw-r--r--   0        0        0     2136 2024-03-09 15:39:33.267482 libresvip-1.1.6/libresvip/middlewares/pitch_shift/pitch_shift.py
+-rw-r--r--   0        0        0      181 2024-03-09 15:39:33.267482 libresvip-1.1.6/libresvip/middlewares/pitch_shift/pitch_shift.yapsy-plugin
+-rw-r--r--   0        0        0        0 2024-03-09 15:39:33.267482 libresvip-1.1.6/libresvip/middlewares/project_zoom/__init__.py
+-rw-r--r--   0        0        0     1009 2024-03-09 15:39:33.267482 libresvip-1.1.6/libresvip/middlewares/project_zoom/options.py
+-rw-r--r--   0        0        0      508 2024-03-09 15:39:33.267482 libresvip-1.1.6/libresvip/middlewares/project_zoom/project_zoom.py
+-rw-r--r--   0        0        0      220 2024-03-09 15:39:33.269050 libresvip-1.1.6/libresvip/middlewares/project_zoom/project_zoom.yapsy-plugin
+-rw-r--r--   0        0        0        0 2024-03-09 15:39:33.269050 libresvip-1.1.6/libresvip/middlewares/pronounciation_conversion/__init__.py
+-rw-r--r--   0        0        0      791 2024-03-09 15:39:33.269050 libresvip-1.1.6/libresvip/middlewares/pronounciation_conversion/options.py
+-rw-r--r--   0        0        0     1510 2024-03-09 15:39:33.269050 libresvip-1.1.6/libresvip/middlewares/pronounciation_conversion/pronounciation_conversion.py
+-rw-r--r--   0        0        0      270 2024-03-09 15:39:33.269989 libresvip-1.1.6/libresvip/middlewares/pronounciation_conversion/pronounciation_conversion.yapsy-plugin
+-rw-r--r--   0        0        0        0 2024-03-09 15:39:33.269989 libresvip-1.1.6/libresvip/middlewares/remove_short_silences/__init__.py
+-rw-r--r--   0        0        0      882 2024-03-09 15:39:33.269989 libresvip-1.1.6/libresvip/middlewares/remove_short_silences/options.py
+-rw-r--r--   0        0        0      953 2024-03-09 15:39:33.270989 libresvip-1.1.6/libresvip/middlewares/remove_short_silences/remove_short_silences.py
+-rw-r--r--   0        0        0      243 2024-03-09 15:39:33.270989 libresvip-1.1.6/libresvip/middlewares/remove_short_silences/remove_short_silences.yapsy-plugin
+-rw-r--r--   0        0        0        0 2024-04-17 19:53:22.520237 libresvip-1.1.6/libresvip/middlewares/replace_lyric/__init__.py
+-rw-r--r--   0        0        0      212 2024-04-19 05:00:08.861563 libresvip-1.1.6/libresvip/middlewares/replace_lyric/options.py
+-rw-r--r--   0        0        0     1326 2024-04-27 16:08:27.375841 libresvip-1.1.6/libresvip/middlewares/replace_lyric/replace_lyric.py
+-rw-r--r--   0        0        0      319 2024-04-19 21:12:02.082450 libresvip-1.1.6/libresvip/middlewares/replace_lyric/replace_lyric.yapsy-plugin
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.217025 libresvip-1.1.6/libresvip/model/__init__.py
+-rw-r--r--   0        0        0    10233 2024-05-19 09:55:57.177960 libresvip-1.1.6/libresvip/model/base.py
+-rw-r--r--   0        0        0     1373 2024-03-23 15:29:05.921080 libresvip-1.1.6/libresvip/model/option_mixins.py
+-rw-r--r--   0        0        0     3152 2024-02-24 21:21:43.981935 libresvip-1.1.6/libresvip/model/point.py
+-rw-r--r--   0        0        0     7529 2024-05-03 03:31:10.216309 libresvip-1.1.6/libresvip/model/relative_pitch_curve.py
+-rw-r--r--   0        0        0     7848 2024-03-18 14:03:10.224552 libresvip-1.1.6/libresvip/model/reset_time_axis.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.218004 libresvip-1.1.6/libresvip/plugins/acep/__init__.py
+-rw-r--r--   0        0        0    54700 2024-02-22 15:40:21.219535 libresvip-1.1.6/libresvip/plugins/acep/ace-studio.yapsy-plugin
+-rw-r--r--   0        0        0     1487 2024-02-22 15:40:21.219535 libresvip-1.1.6/libresvip/plugins/acep/ace_curve_utils.py
+-rw-r--r--   0        0        0      949 2024-04-25 14:59:40.397933 libresvip-1.1.6/libresvip/plugins/acep/ace_studio_converter.py
+-rw-r--r--   0        0        0    20307 2024-05-20 12:25:55.658809 libresvip-1.1.6/libresvip/plugins/acep/ace_studio_generator.py
+-rw-r--r--   0        0        0    17695 2024-05-21 13:15:43.230816 libresvip-1.1.6/libresvip/plugins/acep/ace_studio_parser.py
+-rw-r--r--   0        0        0     1620 2024-05-30 22:39:39.429851 libresvip-1.1.6/libresvip/plugins/acep/acep_io.py
+-rw-r--r--   0        0        0     5339 2024-03-04 16:48:04.991428 libresvip-1.1.6/libresvip/plugins/acep/base_pitch_curve.py
+-rw-r--r--   0        0        0      386 2024-02-22 15:40:21.221571 libresvip-1.1.6/libresvip/plugins/acep/color_pool.py
+-rw-r--r--   0        0        0      565 2024-02-24 21:21:43.984931 libresvip-1.1.6/libresvip/plugins/acep/curve_segment_utils.py
+-rw-r--r--   0        0        0    14273 2024-05-17 23:01:16.675271 libresvip-1.1.6/libresvip/plugins/acep/model.py
+-rw-r--r--   0        0        0    11102 2024-04-04 15:32:50.247348 libresvip-1.1.6/libresvip/plugins/acep/options.py
+-rw-r--r--   0        0        0     2518 2024-04-04 15:32:50.248346 libresvip-1.1.6/libresvip/plugins/acep/singers.py
+-rw-r--r--   0        0        0     1215 2024-02-22 15:40:21.223573 libresvip-1.1.6/libresvip/plugins/acep/time_utils.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.223573 libresvip-1.1.6/libresvip/plugins/aisp/__init__.py
+-rw-r--r--   0        0        0     1486 2024-05-30 22:39:39.430815 libresvip-1.1.6/libresvip/plugins/aisp/aisingers_converter.py
+-rw-r--r--   0        0        0     9421 2024-06-03 13:28:08.958958 libresvip-1.1.6/libresvip/plugins/aisp/aisingers_generator.py
+-rw-r--r--   0        0        0     4725 2024-03-23 15:29:05.925080 libresvip-1.1.6/libresvip/plugins/aisp/aisingers_parser.py
+-rw-r--r--   0        0        0    23952 2024-02-22 15:40:21.224550 libresvip-1.1.6/libresvip/plugins/aisp/aisp.yapsy-plugin
+-rw-r--r--   0        0        0     4713 2024-02-22 15:40:21.225582 libresvip-1.1.6/libresvip/plugins/aisp/model.py
+-rw-r--r--   0        0        0      325 2024-04-22 06:45:10.507210 libresvip-1.1.6/libresvip/plugins/aisp/options.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.225582 libresvip-1.1.6/libresvip/plugins/ccs/__init__.py
+-rw-r--r--   0        0        0    38382 2024-02-22 15:40:21.226575 libresvip-1.1.6/libresvip/plugins/ccs/ccs.yapsy-plugin
+-rw-r--r--   0        0        0     1285 2024-05-23 20:52:25.468981 libresvip-1.1.6/libresvip/plugins/ccs/cevio_converter.py
+-rw-r--r--   0        0        0     8349 2024-04-04 15:32:50.249954 libresvip-1.1.6/libresvip/plugins/ccs/cevio_generator.py
+-rw-r--r--   0        0        0    10117 2024-04-30 12:50:10.287752 libresvip-1.1.6/libresvip/plugins/ccs/cevio_parser.py
+-rw-r--r--   0        0        0    17562 2024-05-09 20:53:19.374299 libresvip-1.1.6/libresvip/plugins/ccs/cevio_pitch.py
+-rw-r--r--   0        0        0      296 2024-02-22 15:40:21.228574 libresvip-1.1.6/libresvip/plugins/ccs/constants.py
+-rw-r--r--   0        0        0    31340 2024-05-23 20:50:28.784086 libresvip-1.1.6/libresvip/plugins/ccs/model.py
+-rw-r--r--   0        0        0      567 2024-03-23 15:29:05.927080 libresvip-1.1.6/libresvip/plugins/ccs/options.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.229551 libresvip-1.1.6/libresvip/plugins/ds/__init__.py
+-rw-r--r--   0        0        0     6352 2024-02-22 15:40:21.230060 libresvip-1.1.6/libresvip/plugins/ds/dicts/opencpop-extension.txt
+-rw-r--r--   0        0        0     4475 2024-02-22 15:40:21.230241 libresvip-1.1.6/libresvip/plugins/ds/dicts/opencpop-strict.txt
+-rw-r--r--   0        0        0     4468 2024-02-22 15:40:21.230241 libresvip-1.1.6/libresvip/plugins/ds/dicts/opencpop.txt
+-rw-r--r--   0        0        0     2051 2024-05-30 22:39:39.430815 libresvip-1.1.6/libresvip/plugins/ds/diffsinger_converter.py
+-rw-r--r--   0        0        0     1846 2024-02-22 15:40:21.231089 libresvip-1.1.6/libresvip/plugins/ds/diffsinger_generator.py
+-rw-r--r--   0        0        0     5222 2024-03-23 15:29:05.928079 libresvip-1.1.6/libresvip/plugins/ds/diffsinger_parser.py
+-rw-r--r--   0        0        0    31348 2024-02-22 15:40:21.232090 libresvip-1.1.6/libresvip/plugins/ds/ds.yapsy-plugin
+-rw-r--r--   0        0        0     3192 2024-02-22 15:40:21.232090 libresvip-1.1.6/libresvip/plugins/ds/model.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.232090 libresvip-1.1.6/libresvip/plugins/ds/models/__init__.py
+-rw-r--r--   0        0        0     1292 2024-02-22 15:40:21.233090 libresvip-1.1.6/libresvip/plugins/ds/models/ds_note.py
+-rw-r--r--   0        0        0      225 2024-02-22 15:40:21.233090 libresvip-1.1.6/libresvip/plugins/ds/models/ds_param_curve.py
+-rw-r--r--   0        0        0      118 2024-02-22 15:40:21.233090 libresvip-1.1.6/libresvip/plugins/ds/models/ds_param_node.py
+-rw-r--r--   0        0        0     3205 2024-02-22 15:40:21.233090 libresvip-1.1.6/libresvip/plugins/ds/models/ds_project.py
+-rw-r--r--   0        0        0     1984 2024-05-30 22:39:39.431862 libresvip-1.1.6/libresvip/plugins/ds/options.py
+-rw-r--r--   0        0        0      786 2024-02-24 21:21:43.986928 libresvip-1.1.6/libresvip/plugins/ds/phoneme_dict.py
+-rw-r--r--   0        0        0        2 2024-02-22 15:40:21.234069 libresvip-1.1.6/libresvip/plugins/ds/utils/__init__.py
+-rw-r--r--   0        0        0     1452 2024-03-04 16:48:04.996982 libresvip-1.1.6/libresvip/plugins/ds/utils/gender_param_utils.py
+-rw-r--r--   0        0        0      294 2024-04-04 23:42:44.572812 libresvip-1.1.6/libresvip/plugins/ds/utils/lyric_util.py
+-rw-r--r--   0        0        0     6771 2024-04-04 23:06:53.822302 libresvip-1.1.6/libresvip/plugins/ds/utils/note_list_util.py
+-rw-r--r--   0        0        0     1380 2024-02-24 21:21:43.988828 libresvip-1.1.6/libresvip/plugins/ds/utils/pinyin_util.py
+-rw-r--r--   0        0        0     1613 2024-02-24 21:21:43.988828 libresvip-1.1.6/libresvip/plugins/ds/utils/pitch_param_utils.py
+-rw-r--r--   0        0        0     3990 2024-02-22 15:40:21.236071 libresvip-1.1.6/libresvip/plugins/ds/utils/project_util.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.236071 libresvip-1.1.6/libresvip/plugins/dv/__init__.py
+-rw-r--r--   0        0        0    11432 2024-03-04 16:48:04.999015 libresvip-1.1.6/libresvip/plugins/dv/constants.py
+-rw-r--r--   0        0        0      847 2024-02-22 15:40:21.237092 libresvip-1.1.6/libresvip/plugins/dv/deepvocal_converter.py
+-rw-r--r--   0        0        0    10745 2024-02-22 23:04:58.757287 libresvip-1.1.6/libresvip/plugins/dv/deepvocal_pitch.py
+-rw-r--r--   0        0        0     6453 2024-02-22 15:40:21.238069 libresvip-1.1.6/libresvip/plugins/dv/dv.yapsy-plugin
+-rw-r--r--   0        0        0     8519 2024-02-24 21:21:43.989880 libresvip-1.1.6/libresvip/plugins/dv/dv_generator.py
+-rw-r--r--   0        0        0     6800 2024-03-23 15:29:05.930098 libresvip-1.1.6/libresvip/plugins/dv/dv_parser.py
+-rw-r--r--   0        0        0     4927 2024-02-22 15:40:21.239070 libresvip-1.1.6/libresvip/plugins/dv/model.py
+-rw-r--r--   0        0        0      325 2024-03-23 15:29:05.931081 libresvip-1.1.6/libresvip/plugins/dv/options.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.239070 libresvip-1.1.6/libresvip/plugins/gj/__init__.py
+-rw-r--r--   0        0        0     5113 2024-02-22 15:40:21.239070 libresvip-1.1.6/libresvip/plugins/gj/constants.py
+-rw-r--r--   0        0        0    72345 2024-02-22 15:40:21.240660 libresvip-1.1.6/libresvip/plugins/gj/gjgj.yapsy-plugin
+-rw-r--r--   0        0        0     1120 2024-05-30 22:39:39.431862 libresvip-1.1.6/libresvip/plugins/gj/gjgj_converter.py
+-rw-r--r--   0        0        0    10541 2024-04-04 15:32:50.250856 libresvip-1.1.6/libresvip/plugins/gj/gjgj_generator.py
+-rw-r--r--   0        0        0     8051 2024-03-23 15:29:05.933100 libresvip-1.1.6/libresvip/plugins/gj/gjgj_parser.py
+-rw-r--r--   0        0        0     6172 2024-02-22 15:40:21.241591 libresvip-1.1.6/libresvip/plugins/gj/model.py
+-rw-r--r--   0        0        0      784 2024-03-23 15:29:05.933100 libresvip-1.1.6/libresvip/plugins/gj/options.py
+-rw-r--r--   0        0        0      303 2024-02-22 15:40:21.241591 libresvip-1.1.6/libresvip/plugins/gj/singers.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.241591 libresvip-1.1.6/libresvip/plugins/json/__init__.py
+-rw-r--r--   0        0        0     1225 2024-02-22 15:40:21.242586 libresvip-1.1.6/libresvip/plugins/json/jsonsvip.yapsy-plugin
+-rw-r--r--   0        0        0      965 2024-05-30 22:39:39.432869 libresvip-1.1.6/libresvip/plugins/json/jsonsvip_converter.py
+-rw-r--r--   0        0        0      350 2024-02-22 15:40:21.243587 libresvip-1.1.6/libresvip/plugins/json/options.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.243587 libresvip-1.1.6/libresvip/plugins/lrc/__init__.py
+-rw-r--r--   0        0        0     1400 2024-02-22 15:40:21.243587 libresvip-1.1.6/libresvip/plugins/lrc/lrc.yapsy-plugin
+-rw-r--r--   0        0        0      484 2024-02-22 15:40:21.244588 libresvip-1.1.6/libresvip/plugins/lrc/lrc_converter.py
+-rw-r--r--   0        0        0     4320 2024-02-24 21:21:43.990884 libresvip-1.1.6/libresvip/plugins/lrc/lrc_generator.py
+-rw-r--r--   0        0        0      670 2024-02-22 15:40:21.244588 libresvip-1.1.6/libresvip/plugins/lrc/model.py
+-rw-r--r--   0        0        0     2391 2024-02-22 15:40:21.244588 libresvip-1.1.6/libresvip/plugins/lrc/options.py
+-rw-r--r--   0        0        0      692 2024-02-22 15:40:21.245587 libresvip-1.1.6/libresvip/plugins/lrc/template.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.245587 libresvip-1.1.6/libresvip/plugins/mid/__init__.py
+-rw-r--r--   0        0        0     1990 2024-02-22 15:40:21.245587 libresvip-1.1.6/libresvip/plugins/mid/constants.py
+-rw-r--r--   0        0        0     5992 2024-02-22 15:40:21.246587 libresvip-1.1.6/libresvip/plugins/mid/mid.yapsy-plugin
+-rw-r--r--   0        0        0      982 2024-02-24 00:53:21.067110 libresvip-1.1.6/libresvip/plugins/mid/midi_converter.py
+-rw-r--r--   0        0        0     6509 2024-03-04 16:48:04.999015 libresvip-1.1.6/libresvip/plugins/mid/midi_generator.py
+-rw-r--r--   0        0        0    12410 2024-04-04 15:32:50.251856 libresvip-1.1.6/libresvip/plugins/mid/midi_parser.py
+-rw-r--r--   0        0        0     2784 2024-03-04 16:48:05.001983 libresvip-1.1.6/libresvip/plugins/mid/midi_pitch.py
+-rw-r--r--   0        0        0      485 2024-02-22 15:40:21.247587 libresvip-1.1.6/libresvip/plugins/mid/note_overlap.py
+-rw-r--r--   0        0        0     3008 2024-03-23 15:29:05.936080 libresvip-1.1.6/libresvip/plugins/mid/options.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.247587 libresvip-1.1.6/libresvip/plugins/mtp/__init__.py
+-rw-r--r--   0        0        0     5764 2024-02-22 15:40:21.247587 libresvip-1.1.6/libresvip/plugins/mtp/model.py
+-rw-r--r--   0        0        0    63944 2024-02-22 15:40:21.248586 libresvip-1.1.6/libresvip/plugins/mtp/mtp.yapsy-plugin
+-rw-r--r--   0        0        0      782 2024-02-22 15:40:21.249586 libresvip-1.1.6/libresvip/plugins/mtp/muta_converter.py
+-rw-r--r--   0        0        0     7329 2024-05-01 15:16:27.115338 libresvip-1.1.6/libresvip/plugins/mtp/muta_generator.py
+-rw-r--r--   0        0        0     5159 2024-05-01 15:02:14.057268 libresvip-1.1.6/libresvip/plugins/mtp/muta_parser.py
+-rw-r--r--   0        0        0      495 2024-03-23 15:29:05.938080 libresvip-1.1.6/libresvip/plugins/mtp/options.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.249586 libresvip-1.1.6/libresvip/plugins/musicxml/__init__.py
+-rw-r--r--   0        0        0     1375 2024-02-22 15:40:21.249586 libresvip-1.1.6/libresvip/plugins/musicxml/model.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.251137 libresvip-1.1.6/libresvip/plugins/musicxml/models/__init__.py
+-rw-r--r--   0        0        0   375282 2024-05-23 20:55:28.214956 libresvip-1.1.6/libresvip/plugins/musicxml/models/mxml2.py
+-rw-r--r--   0        0        0     1619 2024-05-23 20:53:46.293368 libresvip-1.1.6/libresvip/plugins/musicxml/models/xlink.py
+-rw-r--r--   0        0        0      118 2024-02-22 15:40:21.253184 libresvip-1.1.6/libresvip/plugins/musicxml/models/xml.py
+-rw-r--r--   0        0        0    17317 2024-02-22 15:40:21.253184 libresvip-1.1.6/libresvip/plugins/musicxml/musicxml.yapsy-plugin
+-rw-r--r--   0        0        0     1634 2024-05-23 20:51:46.276329 libresvip-1.1.6/libresvip/plugins/musicxml/musicxml_converter.py
+-rw-r--r--   0        0        0    14877 2024-02-24 21:21:43.993929 libresvip-1.1.6/libresvip/plugins/musicxml/musicxml_generator.py
+-rw-r--r--   0        0        0     6295 2024-02-24 21:21:43.993929 libresvip-1.1.6/libresvip/plugins/musicxml/musicxml_parser.py
+-rw-r--r--   0        0        0      125 2024-02-22 15:40:21.255194 libresvip-1.1.6/libresvip/plugins/musicxml/options.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.255194 libresvip-1.1.6/libresvip/plugins/nn/__init__.py
+-rw-r--r--   0        0        0     4875 2024-02-22 15:40:21.255194 libresvip-1.1.6/libresvip/plugins/nn/model.py
+-rw-r--r--   0        0        0     1068 2024-03-23 15:29:05.939080 libresvip-1.1.6/libresvip/plugins/nn/niaoniao_converter.py
+-rw-r--r--   0        0        0     5374 2024-03-23 15:29:05.940080 libresvip-1.1.6/libresvip/plugins/nn/niaoniao_generator.py
+-rw-r--r--   0        0        0     3564 2024-03-23 15:29:05.940080 libresvip-1.1.6/libresvip/plugins/nn/niaoniao_parser.py
+-rw-r--r--   0        0        0    21285 2024-02-22 15:40:21.256182 libresvip-1.1.6/libresvip/plugins/nn/nn.yapsy-plugin
+-rw-r--r--   0        0        0      467 2024-03-23 15:29:05.941583 libresvip-1.1.6/libresvip/plugins/nn/options.py
+-rw-r--r--   0        0        0     1008 2024-02-22 15:40:21.257195 libresvip-1.1.6/libresvip/plugins/nn/template.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.257195 libresvip-1.1.6/libresvip/plugins/ppsf/__init__.py
+-rw-r--r--   0        0        0     7813 2024-02-22 15:40:21.257195 libresvip-1.1.6/libresvip/plugins/ppsf/legacy_model.py
+-rw-r--r--   0        0        0    12763 2024-02-22 15:40:21.258193 libresvip-1.1.6/libresvip/plugins/ppsf/model.py
+-rw-r--r--   0        0        0      325 2024-03-23 15:29:05.942587 libresvip-1.1.6/libresvip/plugins/ppsf/options.py
+-rw-r--r--   0        0        0     1931 2024-05-30 22:39:39.432869 libresvip-1.1.6/libresvip/plugins/ppsf/piapro_studio_converter.py
+-rw-r--r--   0        0        0     8331 2024-03-09 15:39:33.271989 libresvip-1.1.6/libresvip/plugins/ppsf/piapro_studio_generator.py
+-rw-r--r--   0        0        0     6809 2024-02-22 15:40:21.259204 libresvip-1.1.6/libresvip/plugins/ppsf/piapro_studio_legacy_parser.py
+-rw-r--r--   0        0        0     5897 2024-03-23 15:29:05.943588 libresvip-1.1.6/libresvip/plugins/ppsf/piapro_studio_nt_parser.py
+-rw-r--r--   0        0        0    19426 2024-02-22 15:40:21.260207 libresvip-1.1.6/libresvip/plugins/ppsf/ppsf.yapsy-plugin
+-rw-r--r--   0        0        0     3256 2024-02-24 21:21:43.995835 libresvip-1.1.6/libresvip/plugins/ppsf/ppsf_interval_dict.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.260207 libresvip-1.1.6/libresvip/plugins/s5p/__init__.py
+-rw-r--r--   0        0        0     6036 2024-05-08 21:54:55.423825 libresvip-1.1.6/libresvip/plugins/s5p/model.py
+-rw-r--r--   0        0        0      344 2024-03-23 15:29:09.443412 libresvip-1.1.6/libresvip/plugins/s5p/options.py
+-rw-r--r--   0        0        0    52233 2024-02-22 15:40:21.261194 libresvip-1.1.6/libresvip/plugins/s5p/s5p.yapsy-plugin
+-rw-r--r--   0        0        0     1045 2024-05-30 22:39:39.433776 libresvip-1.1.6/libresvip/plugins/s5p/synthv_editor_converter.py
+-rw-r--r--   0        0        0     5609 2024-05-08 21:58:19.283039 libresvip-1.1.6/libresvip/plugins/s5p/synthv_editor_generator.py
+-rw-r--r--   0        0        0    11617 2024-05-08 21:58:19.283039 libresvip-1.1.6/libresvip/plugins/s5p/synthv_editor_parser.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.262203 libresvip-1.1.6/libresvip/plugins/srt/__init__.py
+-rw-r--r--   0        0        0     1394 2024-02-22 15:40:21.262203 libresvip-1.1.6/libresvip/plugins/srt/options.py
+-rw-r--r--   0        0        0     1285 2024-02-22 15:40:21.263187 libresvip-1.1.6/libresvip/plugins/srt/srt.yapsy-plugin
+-rw-r--r--   0        0        0      503 2024-02-22 15:40:21.263187 libresvip-1.1.6/libresvip/plugins/srt/srt_converter.py
+-rw-r--r--   0        0        0     2696 2024-02-24 21:21:43.996926 libresvip-1.1.6/libresvip/plugins/srt/srt_generator.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.263187 libresvip-1.1.6/libresvip/plugins/svg/__init__.py
+-rw-r--r--   0        0        0     4552 2024-02-22 15:40:21.264194 libresvip-1.1.6/libresvip/plugins/svg/coordinate_helper.py
+-rw-r--r--   0        0        0      279 2024-02-22 15:40:21.264194 libresvip-1.1.6/libresvip/plugins/svg/model.py
+-rw-r--r--   0        0        0     3009 2024-02-22 15:40:21.264194 libresvip-1.1.6/libresvip/plugins/svg/options.py
+-rw-r--r--   0        0        0    15147 2024-02-22 15:40:21.265188 libresvip-1.1.6/libresvip/plugins/svg/svg.yapsy-plugin
+-rw-r--r--   0        0        0      568 2024-02-22 15:40:21.265188 libresvip-1.1.6/libresvip/plugins/svg/svg_converter.py
+-rw-r--r--   0        0        0     6739 2024-02-22 15:40:21.265188 libresvip-1.1.6/libresvip/plugins/svg/svg_factory.py
+-rw-r--r--   0        0        0     2422 2024-02-22 15:40:21.266243 libresvip-1.1.6/libresvip/plugins/svg/svg_generator.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.266243 libresvip-1.1.6/libresvip/plugins/svip/__init__.py
+-rw-r--r--   0        0        0    15042 2024-02-22 15:40:21.266243 libresvip-1.1.6/libresvip/plugins/svip/binsvip.yapsy-plugin
+-rw-r--r--   0        0        0     1561 2024-04-25 14:59:53.848685 libresvip-1.1.6/libresvip/plugins/svip/binsvip_converter.py
+-rw-r--r--   0        0        0    11038 2024-04-04 23:08:50.052929 libresvip-1.1.6/libresvip/plugins/svip/binsvip_generator.py
+-rw-r--r--   0        0        0     5944 2024-03-23 15:29:05.947587 libresvip-1.1.6/libresvip/plugins/svip/binsvip_parser.py
+-rw-r--r--   0        0        0     1602 2024-05-30 22:39:39.434769 libresvip-1.1.6/libresvip/plugins/svip/models.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.267240 libresvip-1.1.6/libresvip/plugins/svip/msnrbf/__init__.py
+-rw-r--r--   0        0        0    19970 2024-02-24 13:23:26.660918 libresvip-1.1.6/libresvip/plugins/svip/msnrbf/binary_models.py
+-rw-r--r--   0        0        0      498 2024-03-04 16:48:05.006115 libresvip-1.1.6/libresvip/plugins/svip/msnrbf/constants.py
+-rw-r--r--   0        0        0     1341 2024-03-04 16:48:05.007021 libresvip-1.1.6/libresvip/plugins/svip/msnrbf/nrbf_iobase.py
+-rw-r--r--   0        0        0     4956 2024-03-04 16:48:05.007021 libresvip-1.1.6/libresvip/plugins/svip/msnrbf/svip_reader.py
+-rw-r--r--   0        0        0    23277 2024-02-22 15:40:21.269238 libresvip-1.1.6/libresvip/plugins/svip/msnrbf/svip_writer.py
+-rw-r--r--   0        0        0    15021 2024-04-04 15:32:50.256857 libresvip-1.1.6/libresvip/plugins/svip/msnrbf/xstudio_models.py
+-rw-r--r--   0        0        0     3393 2024-03-23 15:29:05.948587 libresvip-1.1.6/libresvip/plugins/svip/options.py
+-rw-r--r--   0        0        0     1857 2024-02-22 15:40:21.270241 libresvip-1.1.6/libresvip/plugins/svip/singers.json
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.270241 libresvip-1.1.6/libresvip/plugins/svip3/__init__.py
+-rw-r--r--   0        0        0      397 2024-02-22 15:40:21.270241 libresvip-1.1.6/libresvip/plugins/svip3/color_pool.py
+-rw-r--r--   0        0        0      396 2024-03-04 16:48:05.009732 libresvip-1.1.6/libresvip/plugins/svip3/constants.py
+-rw-r--r--   0        0        0    12712 2024-04-26 16:10:27.006657 libresvip-1.1.6/libresvip/plugins/svip3/model.py
+-rw-r--r--   0        0        0      325 2024-03-23 15:29:05.949587 libresvip-1.1.6/libresvip/plugins/svip3/options.py
+-rw-r--r--   0        0        0     1647 2024-05-09 20:54:54.690502 libresvip-1.1.6/libresvip/plugins/svip3/singers.json
+-rw-r--r--   0        0        0      243 2024-05-30 22:39:39.435769 libresvip-1.1.6/libresvip/plugins/svip3/singers.py
+-rw-r--r--   0        0        0    13560 2024-02-22 15:40:21.272276 libresvip-1.1.6/libresvip/plugins/svip3/svip3.yapsy-plugin
+-rw-r--r--   0        0        0      782 2024-03-23 15:29:05.950587 libresvip-1.1.6/libresvip/plugins/svip3/svip3_converter.py
+-rw-r--r--   0        0        0    11203 2024-04-04 15:32:50.257857 libresvip-1.1.6/libresvip/plugins/svip3/svip3_generator.py
+-rw-r--r--   0        0        0     8397 2024-03-23 15:29:05.951587 libresvip-1.1.6/libresvip/plugins/svip3/svip3_parser.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.273244 libresvip-1.1.6/libresvip/plugins/svp/__init__.py
+-rw-r--r--   0        0        0      859 2024-02-22 15:40:21.273244 libresvip-1.1.6/libresvip/plugins/svp/constants.py
+-rw-r--r--   0        0        0      361 2024-02-22 15:40:21.275243 libresvip-1.1.6/libresvip/plugins/svp/interpolation.py
+-rw-r--r--   0        0        0      201 2024-03-14 11:33:30.285334 libresvip-1.1.6/libresvip/plugins/svp/interval_utils.py
+-rw-r--r--   0        0        0     1457 2024-02-22 15:40:21.275243 libresvip-1.1.6/libresvip/plugins/svp/lambert_w.py
+-rw-r--r--   0        0        0    18008 2024-03-14 13:43:05.687807 libresvip-1.1.6/libresvip/plugins/svp/layer_generator.py
+-rw-r--r--   0        0        0    22728 2024-06-03 12:46:07.816896 libresvip-1.1.6/libresvip/plugins/svp/model.py
+-rw-r--r--   0        0        0     5769 2024-06-03 12:33:25.470237 libresvip-1.1.6/libresvip/plugins/svp/options.py
+-rw-r--r--   0        0        0     9582 2024-03-04 16:48:05.013673 libresvip-1.1.6/libresvip/plugins/svp/param_expression.py
+-rw-r--r--   0        0        0     2901 2024-02-22 15:40:21.277240 libresvip-1.1.6/libresvip/plugins/svp/phoneme_categories.json
+-rw-r--r--   0        0        0    57860 2024-02-22 15:40:21.278256 libresvip-1.1.6/libresvip/plugins/svp/phoneme_dictionary.json
+-rw-r--r--   0        0        0     3281 2024-05-30 22:39:39.435769 libresvip-1.1.6/libresvip/plugins/svp/phoneme_utils.py
+-rw-r--r--   0        0        0     3651 2024-02-24 21:21:44.000940 libresvip-1.1.6/libresvip/plugins/svp/pitch_simulator.py
+-rw-r--r--   0        0        0      870 2024-02-22 15:40:21.279241 libresvip-1.1.6/libresvip/plugins/svp/pitch_slide.py
+-rw-r--r--   0        0        0    41585 2024-02-22 15:40:21.279241 libresvip-1.1.6/libresvip/plugins/svp/svp.yapsy-plugin
+-rw-r--r--   0        0        0    21945 2024-03-09 15:39:33.275988 libresvip-1.1.6/libresvip/plugins/svp/synthv_generator.py
+-rw-r--r--   0        0        0    29652 2024-06-03 12:53:36.071949 libresvip-1.1.6/libresvip/plugins/svp/synthv_parser.py
+-rw-r--r--   0        0        0     1182 2024-06-03 12:45:07.833274 libresvip-1.1.6/libresvip/plugins/svp/synthv_studio_converter.py
+-rw-r--r--   0        0        0     7049 2024-03-04 16:48:05.016732 libresvip-1.1.6/libresvip/plugins/svp/track_merge_utils.py
+-rw-r--r--   0        0        0        0 2024-04-20 08:41:44.970999 libresvip-1.1.6/libresvip/plugins/tlp/__init__.py
+-rw-r--r--   0        0        0     5766 2024-06-01 11:50:47.704346 libresvip-1.1.6/libresvip/plugins/tlp/model.py
+-rw-r--r--   0        0        0      325 2024-04-29 22:55:41.750988 libresvip-1.1.6/libresvip/plugins/tlp/options.py
+-rw-r--r--   0        0        0      253 2024-04-30 20:13:41.439220 libresvip-1.1.6/libresvip/plugins/tlp/tlp.yapsy-plugin
+-rw-r--r--   0        0        0     1016 2024-05-30 22:39:39.437283 libresvip-1.1.6/libresvip/plugins/tlp/tunelab_converter.py
+-rw-r--r--   0        0        0     5345 2024-05-30 04:59:53.935499 libresvip-1.1.6/libresvip/plugins/tlp/tunelab_generator.py
+-rw-r--r--   0        0        0     8532 2024-05-19 12:17:21.995853 libresvip-1.1.6/libresvip/plugins/tlp/tunelab_parser.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.281548 libresvip-1.1.6/libresvip/plugins/tssln/__init__.py
+-rw-r--r--   0        0        0      258 2024-02-22 15:40:21.281548 libresvip-1.1.6/libresvip/plugins/tssln/constants.py
+-rw-r--r--   0        0        0    14287 2024-03-04 16:48:05.018348 libresvip-1.1.6/libresvip/plugins/tssln/model.py
+-rw-r--r--   0        0        0      325 2024-03-23 15:29:05.954587 libresvip-1.1.6/libresvip/plugins/tssln/options.py
+-rw-r--r--   0        0        0    20418 2024-02-22 15:40:21.283497 libresvip-1.1.6/libresvip/plugins/tssln/tssln.yapsy-plugin
+-rw-r--r--   0        0        0     3829 2024-02-24 13:21:27.902046 libresvip-1.1.6/libresvip/plugins/tssln/value_tree.py
+-rw-r--r--   0        0        0     1032 2024-02-22 15:40:21.283497 libresvip-1.1.6/libresvip/plugins/tssln/voisona_converter.py
+-rw-r--r--   0        0        0     6553 2024-04-04 15:32:50.258857 libresvip-1.1.6/libresvip/plugins/tssln/voisona_generator.py
+-rw-r--r--   0        0        0     8686 2024-05-07 19:56:46.445386 libresvip-1.1.6/libresvip/plugins/tssln/voisona_parser.py
+-rw-r--r--   0        0        0    17668 2024-05-09 20:53:32.087863 libresvip-1.1.6/libresvip/plugins/tssln/voisona_pitch.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.284496 libresvip-1.1.6/libresvip/plugins/ufdata/__init__.py
+-rw-r--r--   0        0        0     1286 2024-04-04 15:32:50.261367 libresvip-1.1.6/libresvip/plugins/ufdata/model.py
+-rw-r--r--   0        0        0      125 2024-02-22 15:40:21.285497 libresvip-1.1.6/libresvip/plugins/ufdata/options.py
+-rw-r--r--   0        0        0    25204 2024-04-30 20:11:46.826346 libresvip-1.1.6/libresvip/plugins/ufdata/ufdata.yapsy-plugin
+-rw-r--r--   0        0        0     1005 2024-05-30 22:39:39.437283 libresvip-1.1.6/libresvip/plugins/ufdata/ufdata_converter.py
+-rw-r--r--   0        0        0     3019 2024-03-04 16:48:05.021992 libresvip-1.1.6/libresvip/plugins/ufdata/ufdata_generator.py
+-rw-r--r--   0        0        0     4414 2024-04-04 15:32:50.263369 libresvip-1.1.6/libresvip/plugins/ufdata/ufdata_parser.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.287504 libresvip-1.1.6/libresvip/plugins/ust/__init__.py
+-rw-r--r--   0        0        0      220 2024-02-22 15:40:21.287504 libresvip-1.1.6/libresvip/plugins/ust/constants.py
+-rw-r--r--   0        0        0      859 2024-02-22 15:40:21.288508 libresvip-1.1.6/libresvip/plugins/ust/interpolation.py
+-rw-r--r--   0        0        0    17060 2024-03-11 13:13:40.358282 libresvip-1.1.6/libresvip/plugins/ust/model.py
+-rw-r--r--   0        0        0      614 2024-04-19 22:30:20.059096 libresvip-1.1.6/libresvip/plugins/ust/options.py
+-rw-r--r--   0        0        0     2060 2024-04-04 15:32:50.264367 libresvip-1.1.6/libresvip/plugins/ust/pitch_mode1.py
+-rw-r--r--   0        0        0     9626 2024-06-01 22:10:27.094691 libresvip-1.1.6/libresvip/plugins/ust/pitch_mode2.py
+-rw-r--r--   0        0        0     1781 2024-02-22 15:40:21.289493 libresvip-1.1.6/libresvip/plugins/ust/rdp_simplification.py
+-rw-r--r--   0        0        0     1076 2024-03-04 16:48:05.024002 libresvip-1.1.6/libresvip/plugins/ust/resampling.py
+-rw-r--r--   0        0        0     3600 2024-02-22 15:40:21.290497 libresvip-1.1.6/libresvip/plugins/ust/template.py
+-rw-r--r--   0        0        0     8187 2024-02-22 15:40:21.291513 libresvip-1.1.6/libresvip/plugins/ust/ust.yapsy-plugin
+-rw-r--r--   0        0        0      940 2024-04-19 22:31:18.927764 libresvip-1.1.6/libresvip/plugins/ust/ust_converter.py
+-rw-r--r--   0        0        0     4545 2024-03-11 21:42:10.409173 libresvip-1.1.6/libresvip/plugins/ust/ust_generator.py
+-rw-r--r--   0        0        0     6093 2024-03-23 15:29:05.958094 libresvip-1.1.6/libresvip/plugins/ust/ust_parser.py
+-rw-r--r--   0        0        0     3270 2024-06-01 22:20:22.609727 libresvip-1.1.6/libresvip/plugins/ust/vibrato_param.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.292072 libresvip-1.1.6/libresvip/plugins/ustx/__init__.py
+-rw-r--r--   0        0        0     6283 2024-03-04 16:48:05.024934 libresvip-1.1.6/libresvip/plugins/ustx/model.py
+-rw-r--r--   0        0        0      325 2024-03-23 15:29:05.959093 libresvip-1.1.6/libresvip/plugins/ustx/options.py
+-rw-r--r--   0        0        0    45293 2024-02-22 15:40:21.294124 libresvip-1.1.6/libresvip/plugins/ustx/ustx.yapsy-plugin
+-rw-r--r--   0        0        0     1061 2024-03-12 19:57:09.206525 libresvip-1.1.6/libresvip/plugins/ustx/ustx_converter.py
+-rw-r--r--   0        0        0     8246 2024-04-04 23:03:45.113941 libresvip-1.1.6/libresvip/plugins/ustx/ustx_generator.py
+-rw-r--r--   0        0        0     7048 2024-03-23 15:29:05.960094 libresvip-1.1.6/libresvip/plugins/ustx/ustx_parser.py
+-rw-r--r--   0        0        0     4584 2024-03-11 13:13:40.361335 libresvip-1.1.6/libresvip/plugins/ustx/util.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.295117 libresvip-1.1.6/libresvip/plugins/ustx/utils/__init__.py
+-rw-r--r--   0        0        0      407 2024-04-05 21:59:21.996830 libresvip-1.1.6/libresvip/plugins/ustx/utils/lyric_util.py
+-rw-r--r--   0        0        0      634 2024-02-24 21:21:44.007536 libresvip-1.1.6/libresvip/plugins/ustx/utils/music_math.py
+-rw-r--r--   0        0        0     6102 2024-02-22 15:40:21.296134 libresvip-1.1.6/libresvip/plugins/ustx/utils/time_axis.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.296134 libresvip-1.1.6/libresvip/plugins/vog/__init__.py
+-rw-r--r--   0        0        0      766 2024-02-22 15:40:21.297120 libresvip-1.1.6/libresvip/plugins/vog/model.py
+-rw-r--r--   0        0        0      359 2024-03-23 15:29:05.960094 libresvip-1.1.6/libresvip/plugins/vog/options.py
+-rw-r--r--   0        0        0    63065 2024-02-22 15:40:21.298121 libresvip-1.1.6/libresvip/plugins/vog/vog.yapsy-plugin
+-rw-r--r--   0        0        0     1347 2024-05-30 22:39:39.438300 libresvip-1.1.6/libresvip/plugins/vog/vogen_converter.py
+-rw-r--r--   0        0        0     1922 2024-03-18 14:02:32.510275 libresvip-1.1.6/libresvip/plugins/vog/vogen_generator.py
+-rw-r--r--   0        0        0     1658 2024-02-22 15:40:21.299208 libresvip-1.1.6/libresvip/plugins/vog/vogen_parser.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.299208 libresvip-1.1.6/libresvip/plugins/vpr/__init__.py
+-rw-r--r--   0        0        0      434 2024-03-04 16:48:05.027944 libresvip-1.1.6/libresvip/plugins/vpr/constants.py
+-rw-r--r--   0        0        0     9840 2024-02-22 15:40:21.300231 libresvip-1.1.6/libresvip/plugins/vpr/model.py
+-rw-r--r--   0        0        0     1285 2024-03-23 15:29:05.962094 libresvip-1.1.6/libresvip/plugins/vpr/options.py
+-rw-r--r--   0        0        0     4847 2024-03-04 16:48:05.029005 libresvip-1.1.6/libresvip/plugins/vpr/vocaloid_pitch.py
+-rw-r--r--   0        0        0    14147 2024-02-22 15:40:21.300231 libresvip-1.1.6/libresvip/plugins/vpr/vpr.yapsy-plugin
+-rw-r--r--   0        0        0     1515 2024-05-30 22:39:39.438300 libresvip-1.1.6/libresvip/plugins/vpr/vpr_converter.py
+-rw-r--r--   0        0        0    10082 2024-04-04 15:32:50.267366 libresvip-1.1.6/libresvip/plugins/vpr/vpr_generator.py
+-rw-r--r--   0        0        0     6440 2024-03-23 15:29:05.963094 libresvip-1.1.6/libresvip/plugins/vpr/vpr_parser.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.302894 libresvip-1.1.6/libresvip/plugins/vshp/__init__.py
+-rw-r--r--   0        0        0     5774 2024-02-22 15:40:21.303892 libresvip-1.1.6/libresvip/plugins/vshp/model.py
+-rw-r--r--   0        0        0      532 2024-02-22 15:40:21.303892 libresvip-1.1.6/libresvip/plugins/vshp/options.py
+-rw-r--r--   0        0        0      351 2024-02-22 15:40:21.304891 libresvip-1.1.6/libresvip/plugins/vshp/utils.py
+-rw-r--r--   0        0        0      522 2024-02-22 15:40:21.304891 libresvip-1.1.6/libresvip/plugins/vshp/vocalshifter_converter.py
+-rw-r--r--   0        0        0     9770 2024-05-12 02:56:26.310999 libresvip-1.1.6/libresvip/plugins/vshp/vocalshifter_parser.py
+-rw-r--r--   0        0        0     9560 2024-03-05 19:32:37.534334 libresvip-1.1.6/libresvip/plugins/vshp/vshp.yapsy-plugin
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.305892 libresvip-1.1.6/libresvip/plugins/vspx/__init__.py
+-rw-r--r--   0        0        0    12260 2024-05-23 21:06:19.766400 libresvip-1.1.6/libresvip/plugins/vspx/model.py
+-rw-r--r--   0        0        0      325 2024-03-23 15:29:05.965117 libresvip-1.1.6/libresvip/plugins/vspx/options.py
+-rw-r--r--   0        0        0     2794 2024-05-23 20:51:26.669246 libresvip-1.1.6/libresvip/plugins/vspx/vocalsharp_converter.py
+-rw-r--r--   0        0        0     5428 2024-02-22 15:40:21.307892 libresvip-1.1.6/libresvip/plugins/vspx/vspx.yapsy-plugin
+-rw-r--r--   0        0        0     7072 2024-02-24 21:21:44.010521 libresvip-1.1.6/libresvip/plugins/vspx/vspx_generator.py
+-rw-r--r--   0        0        0     8035 2024-03-04 16:48:05.031947 libresvip-1.1.6/libresvip/plugins/vspx/vspx_interval_dict.py
+-rw-r--r--   0        0        0     5857 2024-03-23 15:29:05.966101 libresvip-1.1.6/libresvip/plugins/vspx/vspx_parser.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.308892 libresvip-1.1.6/libresvip/plugins/vsq/__init__.py
+-rw-r--r--   0        0        0      246 2024-03-04 16:48:05.031947 libresvip-1.1.6/libresvip/plugins/vsq/constants.py
+-rw-r--r--   0        0        0     1257 2024-03-23 15:29:05.966101 libresvip-1.1.6/libresvip/plugins/vsq/options.py
+-rw-r--r--   0        0        0     5055 2024-03-04 16:48:05.032934 libresvip-1.1.6/libresvip/plugins/vsq/vocaloid_pitch.py
+-rw-r--r--   0        0        0    49554 2024-02-22 15:40:21.310892 libresvip-1.1.6/libresvip/plugins/vsq/vsq.yapsy-plugin
+-rw-r--r--   0        0        0      957 2024-02-22 15:40:21.310892 libresvip-1.1.6/libresvip/plugins/vsq/vsq_converter.py
+-rw-r--r--   0        0        0     8510 2024-03-04 16:48:05.033991 libresvip-1.1.6/libresvip/plugins/vsq/vsq_generator.py
+-rw-r--r--   0        0        0     8932 2024-05-13 23:51:28.744089 libresvip-1.1.6/libresvip/plugins/vsq/vsq_parser.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.310892 libresvip-1.1.6/libresvip/plugins/vsqx/__init__.py
+-rw-r--r--   0        0        0      332 2024-03-04 16:48:05.034998 libresvip-1.1.6/libresvip/plugins/vsqx/constants.py
+-rw-r--r--   0        0        0      566 2024-03-23 15:29:05.968632 libresvip-1.1.6/libresvip/plugins/vsqx/enums.py
+-rw-r--r--   0        0        0     4400 2024-02-22 15:40:21.312399 libresvip-1.1.6/libresvip/plugins/vsqx/model.py
+-rw-r--r--   0        0        0        2 2024-02-22 15:40:21.312399 libresvip-1.1.6/libresvip/plugins/vsqx/models/__init__.py
+-rw-r--r--   0        0        0    36021 2024-05-23 20:45:39.085386 libresvip-1.1.6/libresvip/plugins/vsqx/models/vsqx3.py
+-rw-r--r--   0        0        0    32062 2024-05-23 20:45:58.846501 libresvip-1.1.6/libresvip/plugins/vsqx/models/vsqx4.py
+-rw-r--r--   0        0        0     1078 2024-03-23 15:29:05.969611 libresvip-1.1.6/libresvip/plugins/vsqx/options.py
+-rw-r--r--   0        0        0     6353 2024-05-12 21:40:04.381986 libresvip-1.1.6/libresvip/plugins/vsqx/vocaloid_pitch.py
+-rw-r--r--   0        0        0    10117 2024-04-04 15:32:50.268367 libresvip-1.1.6/libresvip/plugins/vsqx/vsq3_generator.py
+-rw-r--r--   0        0        0    10118 2024-04-04 15:32:50.269366 libresvip-1.1.6/libresvip/plugins/vsqx/vsq4_generator.py
+-rw-r--r--   0        0        0    49665 2024-02-22 15:40:21.315408 libresvip-1.1.6/libresvip/plugins/vsqx/vsqx.yapsy-plugin
+-rw-r--r--   0        0        0     3151 2024-05-23 20:51:08.663436 libresvip-1.1.6/libresvip/plugins/vsqx/vsqx_converter.py
+-rw-r--r--   0        0        0    13947 2024-05-12 21:44:45.964936 libresvip-1.1.6/libresvip/plugins/vsqx/vsqx_parser.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.316410 libresvip-1.1.6/libresvip/plugins/y77/__init__.py
+-rw-r--r--   0        0        0      742 2024-02-22 15:40:21.316410 libresvip-1.1.6/libresvip/plugins/y77/model.py
+-rw-r--r--   0        0        0      321 2024-03-23 15:29:05.971609 libresvip-1.1.6/libresvip/plugins/y77/options.py
+-rw-r--r--   0        0        0    48980 2024-02-22 15:40:21.317409 libresvip-1.1.6/libresvip/plugins/y77/y77.yapsy-plugin
+-rw-r--r--   0        0        0     1042 2024-05-30 22:39:39.439292 libresvip-1.1.6/libresvip/plugins/y77/y77_converter.py
+-rw-r--r--   0        0        0     3963 2024-03-18 14:02:43.305455 libresvip-1.1.6/libresvip/plugins/y77/y77_generator.py
+-rw-r--r--   0        0        0     3190 2024-03-23 15:29:05.973610 libresvip-1.1.6/libresvip/plugins/y77/y77_parser.py
+-rw-r--r--   0        0        0        0 2024-04-03 00:40:49.030321 libresvip-1.1.6/libresvip/py.typed
+-rw-r--r--   0        0        0   270398 2024-02-22 15:40:21.319450 libresvip-1.1.6/libresvip/res/libresvip.ico
+-rw-r--r--   0        0        0    54799 2024-05-19 09:30:40.522879 libresvip-1.1.6/libresvip/res/locales/zh_CN/LC_MESSAGES/libresvip.mo
+-rw-r--r--   0        0        0        0 2024-02-24 21:21:44.013149 libresvip-1.1.6/libresvip/utils/__init__.py
+-rw-r--r--   0        0        0     1623 2024-05-30 19:32:16.905621 libresvip-1.1.6/libresvip/utils/audio.py
+-rw-r--r--   0        0        0     2441 2024-03-04 16:48:05.048671 libresvip-1.1.6/libresvip/utils/module_loading.py
+-rw-r--r--   0        0        0     3970 2024-03-04 16:48:05.049643 libresvip-1.1.6/libresvip/utils/music_math.py
+-rw-r--r--   0        0        0     1129 2024-02-24 21:21:44.014264 libresvip-1.1.6/libresvip/utils/search.py
+-rw-r--r--   0        0        0     3309 2024-05-19 06:30:15.423045 libresvip-1.1.6/libresvip/utils/text.py
+-rw-r--r--   0        0        0     1627 2024-04-17 18:48:56.821252 libresvip-1.1.6/libresvip/utils/translation.py
+-rw-r--r--   0        0        0     1015 2024-04-03 23:14:53.055643 libresvip-1.1.6/libresvip/utils/xmlutils/__init__.py
+-rw-r--r--   0        0        0     1013 2024-04-19 21:54:15.974691 libresvip-1.1.6/libresvip/utils/xmlutils/native.py
+-rw-r--r--   0        0        0      942 2024-03-12 20:28:45.735172 libresvip-1.1.6/libresvip/utils/yamlutils/__init__.py
+-rw-r--r--   0        0        0     2833 2024-03-24 06:01:39.945387 libresvip-1.1.6/libresvip/utils/yamlutils/common.py
+-rw-r--r--   0        0        0     3873 2024-03-24 06:01:51.194427 libresvip-1.1.6/libresvip/utils/yamlutils/dumper.py
+-rw-r--r--   0        0        0     5052 2024-03-04 16:48:05.053289 libresvip-1.1.6/libresvip/utils/yamlutils/loader.py
+-rw-r--r--   0        0        0      152 2024-04-17 14:03:30.170610 libresvip-1.1.6/libresvip/web/__init__.py
+-rw-r--r--   0        0        0       97 2024-03-01 21:51:25.393182 libresvip-1.1.6/libresvip/web/__main__.py
+-rw-r--r--   0        0        0     2344 2024-03-01 21:51:25.394220 libresvip-1.1.6/libresvip/web/elements.py
+-rw-r--r--   0        0        0    96849 2024-05-28 17:11:01.243572 libresvip-1.1.6/libresvip/web/pages.py
+-rw-r--r--   0        0        0     5344 2024-06-03 14:46:21.598179 libresvip-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0     6029 1970-01-01 00:00:00.000000 libresvip-1.1.6/PKG-INFO
```

### Comparing `libresvip-1.1.5/LICENSE` & `libresvip-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/README.md` & `libresvip-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/cli/commands/conf.py` & `libresvip-1.1.6/libresvip/cli/commands/conf.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/cli/commands/plugin.py` & `libresvip-1.1.6/libresvip/cli/commands/plugin.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/cli/commands/proj.py` & `libresvip-1.1.6/libresvip/cli/commands/proj.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/cli/prompt.py` & `libresvip-1.1.6/libresvip/cli/prompt.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/core/compat.py` & `libresvip-1.1.6/libresvip/core/compat.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/core/config.py` & `libresvip-1.1.6/libresvip/core/config.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/core/constants.py` & `libresvip-1.1.6/libresvip/core/constants.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/core/lyric_phoneme/chinese/__init__.py` & `libresvip-1.1.6/libresvip/core/lyric_phoneme/chinese/__init__.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/core/lyric_phoneme/chinese/vocaloid_xsampa.py` & `libresvip-1.1.6/libresvip/core/lyric_phoneme/chinese/vocaloid_xsampa.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/core/lyric_phoneme/japanese/vocaloid_xsampa.py` & `libresvip-1.1.6/libresvip/core/lyric_phoneme/japanese/vocaloid_xsampa.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/core/tick_counter.py` & `libresvip-1.1.6/libresvip/core/tick_counter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/core/time_interval.py` & `libresvip-1.1.6/libresvip/core/time_interval.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/core/time_sync.py` & `libresvip-1.1.6/libresvip/core/time_sync.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/core/warning_types.py` & `libresvip-1.1.6/libresvip/core/warning_types.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/extension/base.py` & `libresvip-1.1.6/libresvip/extension/base.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/extension/manager.py` & `libresvip-1.1.6/libresvip/extension/manager.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/extension/meta_info.py` & `libresvip-1.1.6/libresvip/extension/meta_info.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/gui/__init__.py` & `libresvip-1.1.6/libresvip/gui/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1594,293 +1594,294 @@
  iconButton.Mate\
 rial.elevation\x0d\x0a\
             roun\
 dedScale: iconBu\
 tton.background.\
 radius\x0d\x0a        \
 }\x0d\x0a    }\x0d\x0a}\
-\x00\x00\x11G\
+\x00\x00\x11U\
 \x00\
-\x00\xa1(x\xda\xed\x1dYs\xdb6\xfa\xbd3\xfd\x0f\
-\xa8vfG\x9a\xb5Y\x1fI\xdb\xf1\xae\xd3\xf1\x117\
-\x9eI\xe2\xd4v\x93\x87nG\x03\x93\x90\x845E0\
-$\xe4\xa3\x19\xfd\xf7\xfd>\x80\xa4(\x8a\x04A\x1d\x8e\
-cK\x0f\x1a\x09\xc4\xfd\xdd\x07@>\x0cE$\xc9\xef\
-\xf2HD\xec\xfb\xefx\xfa\xf7\xf7\x11w\xaf\x8b\xff\x9d\
-O<\xf0\xc4\xedL\xf1\x91\x08d$\xfc\xb8\xf2\x81\xf3\
-\x8eJ\x16q\xea\xcf\xd4xK\xef\xc5H\xce\xb6\xbcd\
-\xc3\xd0\x87F1\xa11\xb9\xcc=v|z\x15;\x9f\
-\x87\xfePx\x0c\x87\xfc\xfe\xbbc\xe8X\xf4\xc9\x97\xef\
-\xbf#\xf0\xe1\xde\x1e\x89\x99\x94<\xe8\xc7\xfa\x89.\xbf\
-\xdb#\xb7j\xfa\xce-\xf7\xe4\x80\xfcHv\xc8&\xc9\
-~\xebJ\xf7Y\xa5\x01\xe3\xfd\x81LjM\xfe\xe8j\
-\xaa\xd5\x1e\xf9ykK\xff\xd7\xcf\xf7\xc8\xcb\xb4 \xa4\
-\x9e\x07\x13\x80\x12\xfd_\x8a\xf0C\xaeH\x17\xf6F\x81\
-+\xb9\x08HLoX\xb7'|\x8fE]y\x1f\xb2\
-v\xae\xa0\x93\xae\x0b?>\x93$\x8c\x18,/yJ\
-\xf6I0\xf2\xfdI\x0d\xde#mO\xad:vt\x95\
-\x0f\xaa~\xfc\x96\xc7\xd2q\xc5(\x90\xe4\x15\xd9\x22\xff\
-\xfc'1T\x1bE\x11\x0b\xe4i\xe0\xb1;\xf2j\x9f\
-lMMB\xad\xaf0\x89\xea\xbe\x14\x98\x9c>\x93m\
-\xbb\xf1:NH\xe5`2\xdax\xf23\xbe\xe5\xd2\x1d\
-\x90\xca\xdd\xc1\x8fKcFZNk\xaf\xb4\xf8\xc7b\
-9~\x22&GQ@\xb6KZ\xa4S\x1eE\xfe\x0e\
-N\xab}!i\xe0\xd1\xc8\xfb\x00\x7fb'N\xfe\xbd\
-\x15.E@\xc6\x85\xe7\xc7,\xbe\x06\xc8\xa7\x8f;\x7f\
-n\xfd\xd5\xa9\x9e\xc0N\xc9\x04\xa6\xf6\xb9\xba\xe9\xee\xf4\
-\x13\x8f\xf5\xe8\xc8\x97\xd5\xf5_\xcc\xec\xef8Ed\x8a\
-\x03\x91#\xe1\x8f\x86\x81&\xce\xfc\x16\xeb\x12\xa7\xc7}\
-\xff\x93\xa6\x01\x19\x8d\xd8\xe4\xf9\xb9\xb8\x9dmd\xd3P\
-5f.l_\xdfg\xc5\xc6\x85\x0e\xde$\xd46\xdb\
-C\x8e6\xb7_\xce>r\x85/`q-\x19\xd1 \
-\x0e)\xe2\x5ck\xba\xd6\xb88\xeb+\xe6\x97\xcdF\xb2\
-;\x98\xc0\xe7\xf82j\xb7\xceB\x05\xfbVg\xb6Z\
-\x0f\xf8\x9fs\x05\xc0\xab\x9a\xac\xaa\x10\xf2;\xe6_\xf0\
-\xbf\xd9\x1e\xd9\xd92\xae\xbcr\xeb\x0a\xf3>uEp\
-8\x92\x12xK\xf5VR\x9f\xf7\x83!\xec\xc1\x1e\xb2\
-\xd5\x03\xfcw\x8e\x1b;\xdb\x80Cw\xdd\x80\x0ea\x82\
-\xad\xa1\xc7\x7fv\x5c_\xc4\xac5[\x11\xe8e\xc8$\
-\x22\xd0n\xc9B\x02v\xdb\xcd\x18\xe3O\xb3\xcfEp\
-\xe4\x03\xefg3\x0c\x5c\x8f\xd7\xee\x18\xd7\xbc\x5c\xec\xd9\
-Z\x10{r?+'f\x03\xd8T\xb2\x14\xb9S2\
-\x97\x7f\xb8\xae\xdb*#f\xfd\xe3H\x80\xd8\x0c`\xa2\
-\xf9\xa1Q@^\xd1\x98\xbb\x17\xc9&\x7f\xa0\xfd\xdc\xa8\
-U\xa4\x9f\x9b\xf1\x90F}\x1e\xc4\xb3D\xf6[$F\
-\xe1\xa1\xb8\xab\x01A\xe5j\xf1sE\xdd\xeb>\xf4\x13\
-\xc04\x8d0\xb5\x83I\x09\xa6\xd4\xad2\xfd\xd0\xc0\x1d\
-\x88(v|\xd6\x03\x08\xe8\xde\xd5\x1fs\xf5HC,\
-\xa9\x1f\x95\x93\x94\x91\xbb\x94q\x19P\xa5nX\x14\xa3\
-\xba\x90\xc2\xad\x8c\xe3Xs\x9e\x8a}12\xf1y\xc0\
-i\xbd\xd8\xe2\x82\x0fFRl\x1e\x037q%9\x0d\
-B\x98\xcd\x09\x07D\xb8\x04\xfd\xc8\xb4\xf0q\xf5#X\
-W\xdd\x04\x9a\xae\xca0\xda\x85\xd6Vj\x06t\x07L\
-s<`\xb1=\xde?\x95l\x18;\x14\x96\xde\xf5\xd4\
-\xd2\xbb\x1c\x97\x0e\x0a@4\xa4\xd2\xdcU\x8e}\xd6\x0c\
-\xaa)\xa7~<P\xec\x92\xf9\x99\xfb\x1b7\xde\xa0G\
-\x8dy\xe7\xa8s\x91K\x1a_\x13TO\xc9\xa7\x01\x0b\
-\xc8\xd1\x00\x18\x11P\xdds\xc3E\xad\x80J\xd8\x8c\xb8\
-\x0bZ\x80F\x0f\x177\x83\xad\x0a\x1d\x0dC>S\x8c\
-\x04\x8eO\xceF2C\xbc\xd7w\x92\x05J\x16 \x97\
-\x04J\xe5.\xf5\xfd\xfbg\xc1\x17\x117\x84\xda\x8b.\
-K\xb7a\xa5\x8c\xb1l\xc0%\xe0\xe1\x94~\xe6\xc0\x1c\
-\xe17\xd8\xf7\xcb\x9ceB4\x1e\xd8\xfdA\x00\xcc\xbd\
-M\xda7\xd4\x1f\xb1\x0e\xd9\x7fe3\x08~T\x03\xb2\
-\xbf\x9f-\x98\xfc\xaa\x5c\x0ed/+\xd8\xd7\x95\xea\xfb\
-\x1bw\x9e\x15\xd5\xbe\x03\x1b\x9co^\x0e\x224\xaa=\
-2\xd1\xe0\x9e:\x9d\x0eq\xe1]\x99,\xbc\xebf\x0b\
-_\x15\x9dV\x0e\xf8\xa0\xf2b\xbc\x14\xfb\xd4l\x1c\x89\
-\xc8c\x91\x93\x9a=>\x1a\x17\xfd\x88\xdd\x97\x18=\x15\
-\x96\xe3xm\xb1=\x90\xc5\x96\x08\xec\xe7a\xad\x1d3\
-\xea\x13\xe0\x18\x03ds= c\x19\x7f\x13\x5c\x0e\xa4\
-\xee\x95\xa8\xc0\xff)\x17X\xc2\xe2pe\x1f\x04|\xdf\
-\xab\x96\xe6F\x99\xb3k\xcbj=\xf6\x0e\xb9\x22\x14\xce\
-\x85\x8f\xbe9\xfc\xd92\xd7V\x92:\xa9\xae~\xd7\xd4\
-W\xee\xfb=\xf2g=?\xfe\xa2\xba\x83n\xcf\x80\xf7\
-\xdeF\x5c\xb2\xd6\xc64=d\xe5\x9d\xf1F\x83\xfe.\
-\xaeyX\xe8J\x155\xeb\xe5C\x04\xfa\x95,\xf4\x93\
-\x14vj\xd4\xb4\xbf\xea\xe4\xd6\x81+\xf9\x0dU\xba[\
-\x9b\xab(\x86\xa5\x86\x95\x17b)zuC\x85_(\
-\xbat\x5c\xe4c\xbdvU\xabg*\xfd\x0f\xdd\xd46\
-\xb3\x924\xea39%\xd3\xeb\x1be\xd1,Te\xa7\
-V\x92\xaa\xa1\xa9\xf2i\xa9y\xa6\xe1\x9ef\xad&\xd1\
-\x9e\x09\xbe\xed5m\xaa\xf0\xabq\xab\x04\x9b\x1a\xb4K\
-Q\xa0\xc0U\xa6\x03p\xfb\xa5U\x14\x9a\x9d\xf5\x14n\
-$[\xd4l\xdc+P\x96\xae\xed\x9a\x8c-T\xfb\xaf\
-e\x07M\xef\xd4\xd4\xae\x18\x88\xeby\x19\x22g!\x0b\
-2\xff\x81\x0e\xd9*\x9f\xd61\xec\xf9S\xb7E\x04\xac\
-\xbd\x9b\x0f\xb0\xa3Y\xacQl\x85\x06\x89y\xd4Gb\
-\x95XG\x8bp!\x18\xd1n\x1e0\x02\x0d\xdf-\xd3\
-\x80lpC\x070\x95\x81R\xb6\xfd\xe9\xc44B\xab\
-j\xc6\x90b\xfbJ\xf5g\x92\xcc\x98^\x01\x0c\xa5\x9b\
-\xf8<\x0a\xa9\x15e\xb2I\xf7\xe9 \xb1\x19%\x94\x12\
-\x10\x89\xeeB\x87\x0c\x93Z.\xc4(r\x81\xfcjq\
-+?\xa3\x96S\xa3\xaf\xd5p\xf5\xb1\xd5\x14\x93\xbc\x85\
-\x86s[A\xb2\xc4\x03\xacU\xe7\xa1$lq\xce\x15\
-/?\xebee\xcb=\x1a\xc5R\x0cI\xfb0\x12\xb7\
-P\xe88N\xc7b\xd1T\xeb\x8e\x0e\x98\xcb\x22f\x17\
-\x09;p$\x98\xca}\x16\xb5k\xe0\xa4\x93N\xe6\x9a\
-y\x9a\xc9\xd2\x04*y>\x9cc\xc1\xab\xd8\xdcq\x95\
-\x8f\xa3t\x06Z\xa3\xefV8K\xcd\xde\xa3:\xefG\
-]d^\xfbz\xb8g\xd6F\x9a\x88lD\xa0\xbdb\
-\xd2R\xce\xcb\x03\xd3\xad~~N=.\xaa3T\xe6\
-\xd7\x8cT}\x98\x9a\xd1\xe6N\xaa\xe9I\x1ak\xe6d\
-\x90\x83.\xae\xd0B\xe6L\x0b\xa8!;\x885\xabW\
-k\xb6s\x1d\x15eD3\x9d\xf31\xed\xed\xf6\xea\xf6\
-\xd6\xd3\x02\xa3\xc1\xb6fr\xed\xb1\xed\xe7\xf6c\xc0U\
-\x9dkX\xb3\x9d,\xa0W>\xaaS\x16I\xa6v@\
-)\x08\xe0\xeaF\x97B\xf8\x97<\xb4\xf1\xd4\xe5\x96\x92\
-\xb4\xaa\xf1\x8a\xf1\x98_\xa1O,\xd7\xd0\x19\x88\x1b\x16\
-1\x0fSeq\xbe\xe4\x87}\xd0\xbfZ\xab2d\x1f\
-(q\xd7\x04\x91\x07\xd7h\x96\xe18\x98\xcb\xb1U\xb6\
-\x84C\x19\xd4\x10I\x99\xa7K[\x17m\xeb}\xfe\xca\
-`V^\xe9\x19\xe2p\xbe\x1a\xf4\xf3\xdb\x92\xa7\xbd\xc4\
-<n\xb4\xae\xd4\x82+h\x5c\xf3h\x83e\xd3\xcbw\
-\x8b\xac\xa0b\x1b\x1bO\xd9\xac0V\x8c\xd2l\x88\xb1\
-}\xf5\xf1\xa3\xf1\x08.\x8d\xb0s\x18\xdc\x88\xb6\x8f\xa9\
-\xa4G\x89\xe7\x9a{w\xdb\x1b Z\xeev6H3\
-\x7f\xf4\x9a\xe0\x9b\x10|\xb3m@\xa8\xa0\x02\xd5\xa0\xd5\
-\x7fT\xab\x1d\xd5j\xcd]\x9e,w)\x90\xf29\xd8\
-\xaa\xe7l\x08\x0a\x9d\x22\xe5\x0d\xd2\xe3Q,7\x88O\
-c\xd9\x88\x92U;\x02\xf0Q\x04\x8b\xcd\xf1O\x1d}\
-o\x92\xed%\x11l\x9d\xfe\xb9\x0a\x99j\xf0f,\x8a\
-\xfd\x8fA\xda\x8c\xbf]cp\x85\xc6\xb5\xab\xfc\x84\x0d\
-l\xebR\xc7\xe2\xbcA\x0a\xb5\xd3u\x99DM\xf6\xb8\
-A\xde\x14~*r\xa7*fjF\x87\xea\xe4\x8e7\
-G\xf0\xb7\x8a\x5c\xa6\x12\x09i@\xfb,1\x91c\x92\
-0\x98\xaa\xed\xb5\x8bZ\x95\xf2\xac\xe4\xb8\x15F\xaf\xda\
-\x9d%\xe5\xbd\xd5hrV\xb9\x069V~\x91\x0b\xaa\
-\xd9\xe5\x15(\xa9\xcd|\x98\x03\xf3\xba<\x09\x14\xcf\x1c\
-\xb95\x85\xd0\x95\x80.\xf4\x00l\xdf\xcc\xd4g\x5c\x7f\
-\xce$_\xd6\x90\xe4E\x98\x0f\xe4S1\xe2\x8eq\xc4\
-\xbcCl\x09\x83\xed\x1a\x07+S\xde\xf4XU-\x8c\
-s0\xc5\xce&\xac\xc8nU+\x89\x81\x86\xfe\x08=\
-\xeb\xcdC\xa0oD\xc4\xff\x16\x81\xa4\xfe\x1bu\xb8\xf6\
-#g\xa5\xa1s\xd8O\xfe7:\xd7\x8eR\xdfy\x8f\
-\xc2\xce\xccV\x8c\xef\x03\x17;\xc9\xe6t\x89\xad\xb0d\
-\xfe\x14N\xd7\xe7a\xd530\x04X\x9fJf\x91\xdc\
-\xc9\x87!\xb0\x1e.\xdfd\xe7\xe1\x8d\xec8=li\
-\xc3\xb3\x93c\xf9\xe9E\x02\xce$\xe9\xf4\x98\x0f\x8f\xb0\
-\x8e1\xdf\xb4\xd8\x5c\xb3\xbf\xa4\xdd\x02\xb9\x1bi\x0a\xa9\
-\xabX\xf9i\x90f\x91\xd6\xca\xf0\xa6\xf2`\x9e\xc4\x0f\
-\x8f\xc7\xa1O\xeb\x92]2\xe7\xa7&}\xb4>v\xe7\
-\x0a\xd6\x99O\x1dO\xe1I\xf1@\xf1\x80\xf9\xe1\xa6\xcb\
-#\xd7g\x9b\xb0;>\x0f\xea\x12\x13'G\x8dw\xb6\
-jc\x83\xb1\x88\xba\xf1\x80\x86Lm\xf6\xa7\x01\x95\xf1\
-\xe5\x80\xc7G\xea\x89\xb9u\xaa\x80g\xbb\x94\xb8\x85\xed\
-ZM9\xba\x15\xb5\x12\x1e\xa7Nt\x22\x22\x12\x08I\
-\xdaJ^\x13)\x88\x82?a\x1eG\x1e\xa3r/;\
-\xadf\xd0\xdb\x9f\x0bz\x8d\x85z\xc6r\xaa23\x96\
-\xc7\x9a\xac\x8fnk\xad\xf8\xa2\x22\xe3$\x09Y\x9a\x1e\
-\x9b\x98 \xc2\xe4R\x87\xbb\x813g\xcbr.8\xf2\
-\xc3K\x1a\x86\x88\x12\xb3\xed\x92\xfc\xd9\xbc\xa5\xf4\x19\xbd\
-*-\xbdA]\x97\x06\x1e\xf7\xf0\xa2\x932@_\xb8\
-\x91\xf0\xfdC\x1a9\x80s\xea\x90\xd7\xde\xa4\x8c|\x19\
-\x9bZ\x0c2\xb9Slcb\xf1\xc7\xc9\xaf#\x15\xe9\
-\x8f\xaa\x089W\x8d\xbbf\xe9]\x1f\xb8j `\x8a\
-\x82&\xc1\x9c\x9d:\x1eP\x14L\xbb;5\xe9\x006\
-\x02j\xb9\x82jq\x81\xd5HL\xcc%*\xe6\x93x\
-K5\xc0\x9bc\xde\xf6*1o{\x8dy\xf3c^\
-\x82tO\x10\xe7vV\x89s?}M\x943\x09\xc9\
-5j~\x03\xa8\xb9\xbbJ\xd4\xfc\xf9yqCS\xfb\
-\x88}\x1eq\xcc\x1f\x09#\x11\x82\xf6v\x0f\xf3\x13~\
-\xaa\xdc/\x19]\xd1\xa0\xe2\xee\x09\xa8{o\x05:\x19\
-\x1c,hk\xdb\xaaE\xfeE\xec\xc5\xbb:\x8a\xd8\xa3\
-C\xee\xdf\x83q\x96.\x1b\xf0,\x06\x0bU\x99xq\
-\xcb\xb2\x97\xfc\xbdV;6\xf9\xf3\xa5\x1bN]\xb7\x96\
-\x9c\xe6'\xc4)\x13\xea\x87\x0c85\xb4[c\xfce\
-\xd6\x01\xf6w\x9c\x11\xd5\x11:\xaf,\xce\x1a\xaa\xcdH\
-\xcf2L\xce\xdf\xb7T\xd9\x95\xb8\xdb\x1c\xd2\x08\x9e\xb5\
-\xec\xf7\x04\x8d'\xfb\xfd\x10\xc1\xa5\xe8\xf7}\xcb\xc4\xa5\
-\xd4A\x9a7q\xa4j\xdf\xd56N\x1b\xcc\xaeN\xa3\
-\xa8\x13^\xfd\xa1}\xde\x91\x131\x1f0:\xb9\x90&\
-nw\xbe\xa9\x88\x91\x8d\xdfq\xe2\x1a\xad\xf4=\xfa\xf7\
-\x11w\xcf\x19P\xb0\xcb\xd0e\xb4\xfc\x8b\xbb\xac\x8cl\
-\xab;\xfcLN3[\x93\xbf\xeePn\xd9\x9e$\x11\
-\x8c\xb4iyC\xa4G\xaaH\xbdZ\x81\xc9\x9d\xa7M\
-\xb8f\x05\xa1U\x9a\xf6jj\xddh2\xb7nh\x8e\
-\xd84\xf31\x95\xfa\x96\xd4\x00\xd5\x11\xa1\x03`\xa2a\
-]*\xa2\x0ep\x07^[9;T\xb6\x01\xf2\x9d\xcd\
-\xfa\xe0u\x0d0\x92l\x12t\x92\xe4{\xaf\xf1c\xe6\
-\x98\xc0\x90{\x9e\xcfn\x81\x7fu\x85\xbem\xb1;\x0a\
-\xd1k\xe2\xb5;\xcb\xd2\xa4\xe68\xc5[\x5c\xf6\xf9\xc8\
-g\x13\x97W\xb2j\xf5\xad\xae\x94j/\x14\x0f\xad\xf7\
-\xae\xcexU\x87<\x18UI\xeb\xdcU\x8d/W\x85\
-\x95:\xe5\x22=\xa3\x99\x84\x8c\x16\x0b[\x22\x8e\xd6a\
-[2\xdee\x96\xb4\x9b\x9c\x22i-\x09\x8f#\xb5\xac\
-&\xd3\xe8,6l\xe1\x90\xeb\xd6\xe3!\x9c\xb2\xb8}\
-\xf5\xc9P[\xfe?.\x13\x1d\x06}x\xea\xda@\xcf\
-\xc3\x8bFI\x04\xb4X\x86j\xe3\xf9\xc4\x0d\xf5<\x0d\
-\x15\xb3\x80IV\x08\x98\xdec\x003/\xf5\x12U\x05\
-\xc2\xec.o\xb0\xbd\xb4!\x91H\x98y\xf4\x0e\x7f\x1a\
-3T\xa0\xd2k_\xa1\x1b\xf92\xb5\x83'x\xbb\x13\
-([\xee\xa0\xd5\xf97I\xefO\xe8Aik<O\
-\x7f\x07~8\x00\xe8I\xee\xe6\xfb\xa3\x93\xd2\xb9z}\
-/\x82MZ\xdas\x00\x5cp\xd1\xde\xcfY\x9f\xdd\xe5\
-;\x8dT\xc1\x02\x12eQ1\x92\x08\xcf\xfc\x95\x10\x0f\
--N\xec\x83t\xf5\xc2e\xbe\xa0\xdc\xe2\x22i\x82\x8c\
-{\xe4 \x0c}\xceb\x0c\xbcM\xf0\x05,/\x1aQ\
-\x17&\x1f;\xff\x0d\x10\xcb\xf2MNT\xc8.\x8fy\
-\xb9\xfa`n\x81\xb5\x8f\xa9*#u\x84\x95\xa0\x9d\x86\
-\xbd(l\xda\x03\xa38\x02>r\x03F\x19\xf3\xc8(\
-\xc6\x16\xea\xc6\x9c\xeb@\xdc\x82\xb5\xd5gD\xf4\x08 \
-\xda\xc8\xa7\x11aw(.cu\xec\x12\x04Wi\xfe\
-\x849F\xb7\xc2\xc4\x033\xc6~3i\x08\x96\xce\xab\
-u\xb6\xc2#\xcaV(z\x96\xb6\xb7\x1eA\xb4{U\
-\xf4\xf0\xe4b\xdf\xa8\x95\xc5\xe8\xccIL\xe2\x05\x95\xe8\
-u|\xdc2J\xb9\xb5\x8eR.\x16\x1f\x9f\xd1\xff\x95\
-Vq K\x1eL\xddA\x942\xb5\xce:\xb2^{\
-\x87\x83ed\xf11EC\x9fq\xc8i\xc5\x11\xd2\x87\
-\x0c\xcc\xa0t9\xe1\xcc\xf7lV?_LE\xef\x99\
-\xe5=\xc9\x13\xd1t0\xd1\xbbp\x92\xea\xeeyK\xf5\
-+\xdb\xc4D2Vw\xf5\xd1\xb6+\x11\xbc\xd6p8\
-\xe1\x01\x8f\x07\x0d\x02D\x09\xb2`\xde\xb6\xf5\xf9\xb2\xe4\
-:Vw\xc0}\x0f~\xfd\xb9\xf5Wz\x0a\xca\xae\x0f\
-\x8b\x18\xd0\x04!\xd4q\xfd!\x97\xd6+b\xd3;a\
-\x13\x98\x1a?\x93t\x955#_3\xf25#_3\
-\xf25#\x7fpF\xbe\xfb\x18\x18\xf9\xcb5#_3\
-\xf25#_3\xf25#\x9f\x9b\x91\xbfXk\xe4k\
-F\xbef\xe4kF\xbef\xe4\xdf6#\x7f\xb9>n\
-\xf1\xfc\x8e[\xb43\xa2\xc4\xf4\xc3?\xde\x9f\x1e\x9d\x1d\
-\xbfn\x91_gs\xf8\xc9^\xae\xec\xca\xa7\xc1u\x96\
-Z\xd3Y\x9f\xd6\xf8\x9a\x92k\xd1\xd3\x1a)\xd4\x1f\xcf\
-)\x0d\xbc\x08'\xbd\xfff\xb2\xea\x1b\xfcR\xc5xP\
-c#a\x5c\x96\xe7,\xacR\xd7b&\xf1.E\x9d\
-S\xbd\x91{\x8f\xe4\x842\x00yO\x7f{\x7fv\xfe\
-\xfa\xe8\xe0\xe2uk\x03\x93L\x8e5\x09a\xdacg\
-Q\xa9VK\xaf\xb99-\x99B\x1f\xafd\xfai\x95\
-\x92\xe9\x97u\xc2\xc1\xe4c\x95\x9b\xb58g\xb4\xbf\x7f\
-%\x83B1\xc5\x93F\xc0\x036G\x0d\xefb\x99\xa8\
-\xa2\xb6w\xb2\xa4\x9f\x80\xddv\xb3\xb7\xe4\xbd\xb0T\x0f\
-\xd3+\xc8\xf1\x0e\xcfW\xc4r\xa4f\xef\xf2i\xc6\xdf\
-ni\x88\xbc\x13\xefy\xdc\xc0Yu\x1e\xf2\x9a\xcb\xa5\
-A\x1d\xb0;x\xccp\x7f\x00\x08*\xe8\x81<\xd8\xfe\
-\xd6 h:\xe9\xf3\xe4\xa0\x85\xd2I\xb2\xf6C\x12\xda\
-c:\x0d\xaa\x0f\xf0\xc4\xcb?\x04\xba\x94\xb3\x9b\x86\xe3\
-?\xa9\xf0\xdeZ\xf2\x89\x9f\x91\x14Z[W\x19\xf6\x7f\
-\x84\x95\xd7)=\xd8i%\xf3\xfb\xea\xaa\xdfm\xaf\x9e\
-\xa8\xf4\xd8\x04\xc8\x8b\x1c\x95\xab\xef\xbd\xee=t\x0b\xdd\
-\xa4X\x8aMfS\x07\x08]\xe5\xe0N\x8f\xa1\xde\xa3\
-\x93 \xbb\xae1\xff\xd9\xe5\x99\x83Y\xa8\xa7N\xd7\x84\
-m\x93x\xd8\x0e\xf6M\x1f\xa5\xaaJ\xfcN\xd2\x9b\xa7\
-\xa7\xe6$\xcd\xdf\x95_7\x9f?\xc97\xdb4\xf7\xb0\
-L\xa5\xcc^\xa6Wh\x97\x94\x97\xbc\xfd.\xe2\xd0\x9f\
-:\x8b2Y\x8a\xf31\xf1Z\x96\xbd]\x1c\x94\xe2\xf8\
-\x90\x0d\xe8\x0dG\x95\xf7\x04\xb1\x0c\x99\xafs!Ex\
- \x0f\xd5\xf3\x92\xebY\xd3z\xc7<\xd2W\xbd\xe6\xdb\
-\x22}\xaa\x7f\xa7\xbd\xf7\x8cye\xc8\x16\x074\xc4\x1d\
-\xcb\xcd\xf2\x02\x8a.\x05B\xa1l+\x06\x00gu\x89\
-\xef;q\xc3\x8eGQ\xb2\xc6\x9d\xb2\xd0sV\xf7\x1c\
-\x0f\xba\xe4j\x9b\xea\x9e\x08\xdf\x17\xb7x\x18)\xca\x90\
-\xa1\x9c\xfc'\xdd\xe3e\xb4\x85U\xe0\x11\xa3{\xf5`\
-\xb6a\x86\x8bo\xd2\x1e\x0e\x190f\x90\xb0\xbf\xd8T\
-~\x8d\xaf[W,\x15\xf4Nlb\x98\xda\x1e\xc1\x15\
-T1\x0b+\x1b/\xbd\x12\xf9\x85\xc1lL\x18|\x01\
-=Uiu\xa3\xfb\x99\x06\xa1\x88\xb9~M\xe6\xfe>\
-\xb9t\x92\xd2\x13!\xf0r\xc4_\xc9\x16\xc9^\xd5\xae\
-'\x05\xeb\xd7?\xaa\x07\xb16\x1f\xa7M\xc7\xc2\xc4\x0a\
-^\xae\x1a\xdb\xd1\xeeM\xf7\x8d\xf9\xec\x14'xY\x04\
-;\xce\xb4R\x95DNzEc\xee\xa6\xba\xc3\xa1,\
-y-\xdfm\x8e5\x9a\xe4\xee!\xf6d|\xbd}\xca\
-\xed'A\x17\x1d\x0e\x99\xc0\xaf\xf0\xc0\xf8\x02\xcf\x0a\xe4\
-Lat!\xc1\xae\xb78*=\xbb\xb3\x0dw\xb0\xf8\
-6\xd4\x856\x11\xaf\xb3&\xd8\x9b\xd5F\x02\x17\x9e\x85\
-\xa0s%`\xba\xc3\x95l\x7fn\xe0wJm\xcc\xda\
-V\x0b\x9d\xc5 \xb6\xbd\x02\x88\x15\xeen^\x08`'\
-\xea\x22\x1a\xf2!\x127\x1c\xdf\x82\xa0ou-\x85Z\
-\xe6\xa8\xf8!\x7f$\xffj\x14\xdf\xd7@\xb8\x04\xc3\x9e\
-\x16\x90wV\x00\xe4\xaaKr\x16\x82\xf6[\xec\x94\xe4\
-z%\xca\x22\xad\xa5\xd1Y\x8c{Z\x00\xdc]\x01\x00\
-\x0bv\xedBpK\x8c@{\xa6j\xc0\x9e\xa7\x05\xb9\
-\x17s\xd8tF%\xd1\xca\xfc*W\xbcL\xaf\xe3\xc8\
-\x0d\xad\xd6ati,~oU\xde\xc8T\xe3\x15f\
-Z\x91@5m\xcfm\x15\xdf|a\xfb2\xc8)\x91\
-\x8e\x0e\x1d\xc7\x8d\x18 \xf0\xd9\xd5\xff`\xdb\xdbS\x13\
-+\xc1\xe4\xb2\xf7\xb37\xeb\xa1\xe4\xed\x06\xcd:0]\
-Q\xd6\xac\xa7\x12\xf7V\xb3\x0e\x16|_Q\xa9Kc\
-\xfc\x7f\x07uf\xdf\
+\x00\xa1\x1cx\xda\xed\x1dko\xdb\xb6\xf6\xfb\x80\xfd\x07\
+\xce\x17\x18l\xdcDK\xd2v\x1br\x97\x0d\x89\xd3\xac\
+\x05\xfaZ\x92\xb5\x1fv\x07\x83\x91h\x9b7\xb2\xa8J\
+t\x1e+\xfc\xdf\xef9\xa4$\xcb\xb2DQ~\xa4n\
+c\x7f0l\x8a\xcf\xc3\xf3>\x87\x14\x1f\x85\x22\x92\xe4\
+\x0f\xd9\x15\x11\xfb\xf6\x1b\x9e\xfe\xfdc\xcc\xdd\xeb\xe2\x7f\
+\xe7\x03\x0f<q;W\xdc\x15\x81\x8c\x84\x1fW>p\
+^S\xc9\x22N\xfd\xb9\x1a\xaf\xe8\xbd\x18\xcb\xf9\x96\x97\
+l\x14\xfa\xd0(&4&\x97\xb9\xc7\x8eO\xafb\xe7\
+\xe3\xc8\x1f\x09\x8f\xe1\x90\xdf~s\x0a\x1d\x8b\x01\xf9\xf4\
+\xed7\x04>\xdc;$1\x93\x92\x07\x83X?\xd1\xe5\
+w\x87\xe4VM\xdf\xb9\xe5\x9e\x1c\x92\x1f\xc8\x01\xd9%\
+\xd9o]\xe9>\xab4d|0\x94I\xad\xe9\x1f]\
+M\xb5:$?\xed\xed\xe9\xff\xfa\xf9!y\x96\x16\x84\
+\xd4\xf3`\x02P\xa2\xffK\x11\xbe\xcb\x15\xe9\xc2\xfe8\
+p%\x17\x01\x89\xe9\x0d\xeb\xf5\x85\xef\xb1\xa8'\xefC\
+\xd6\xce\x15t\xd2u\xe1\xc7g\x92\x84\x11\x83\xe5%O\
+\xc9\x11\x09\xc6\xbe?\xad\xc1\xfb\xa4\xed\xa9U\xc7\x8e\xae\
+\xf2N\xd5\x8f_\xf1X:\xae\x18\x07\x92\xfcJ\xf6\xc8\
+\xf7\xdf\x13C\xb5q\x14\xb1@\xbe\x0c<vG~=\
+\x22{3\x93P\xeb+L\xa2\xba/\xb5M\xce\x80\xc9\
+\xb6\xddx\x1d'\xa4r8\x1dm2\xfd\x19\xdfr\xe9\
+\x0eI%t\xf0\xe3\xd2\x98\x91\x96\xd3:,-\xfe\xa1\
+X\x8e\x9f\x88\xc9q\x14\x90\xfd\x92\x16\xe9\x94\xc7\x91\x7f\
+\x80\xd3j_H\x1ax4\xf2\xde\xc1\x9f\xd8\x89\x93\x7f\
+\xaf\x84Kq#\xe3\xc2\xf3S\x16_\xc3\xce\xa7\x8f;\
+\x7f\xed\xfd\xdd\xa9\x9e\xc0A\xc9\x04f\xe0\x5c\xdd\xf4\xc9\
+\xec\x13\x8f\xf5\xe9\xd8\x97\xd5\xf5\x9f\xce\xc1w\x92\x222\
+\xc5\x81HW\xf8\xe3Q\xa0\x893\x0fb]\xe2\xf4\xb9\
+\xef\x7f\xd04 \xa31\x9b>?\x17\xb7\xf3\x8dl\x1a\
+\xaa\xc6\xcc\x05\xf0\x0d|Vl\x5c\xe8\xe0EBm\xf3\
+=\xe4hs\xff\xd9\xfc#W\xf8\x02\x16\xd7\x92\x11\x0d\
+\xe2\x90\x22\xce\xb5fkM\x8a\xb3\xbeb~\xd9l$\
+\xbb\x83\x09|\x8c/\xa3v\xebm\xa8\xf6\xbe\xd5\x99\xaf\
+\xd6\x07\xfe\xe7\x5c\xc1\xe6UMVU\x08\xf9\x1d\xf3/\
+\xf8?\xec\x90\x1c\xec\x19W^\x09\xba\xc2\xbc_\xba\x22\
+8\x19K\x09\xbc\xa5\x1a\x94\xd4\xe7\x83`\x0408D\
+\xb6z\x8c\xff\xce\x11\xb0\xf3\x0d8t\xd7\x0b\xe8\x08&\
+\xd8\x1ay\xfc'\xc7\xf5E\xccZ\xf3\x15\x81^FL\
+\x22\x02=)YH\xc0n{\x19c\xfcq\xfe\xb9\x08\
+\xba>\xf0~6\xc7\xc0\xf5x\xed\x8eq\xcd\xab\xc5\x9e\
+\xbd%\xb1'\xf7\xb3rb6\x1b\x9bJ\x96\x22wJ\
+\xe6\xf2/\xd7u[e\xc4\xac\x7ft\x05\x88\xcd\x00&\
+\x9a\x1f\x1a\x05\xe4\x15\x8d\xb9{\x91\x00\xf9\x1d\x1d\xe4F\
+\xad\x22\xfd\xdc\x8cG4\x1a\xf0 \x9e'\xb2\xdf#1\
+\x0eO\xc4]\xcd\x16T\xae\x16?W\xd4\xbd\x1e@?\
+\x01L\xd3\xb8\xa7v{R\x82)u\xabL?4p\
+\x87\x22\x8a\x1d\x9f\xf5a\x07t\xef\xea\x8f\xb9z\xa4w\
+,\xa9\x1f\x95\x93\x94\x91\xbb\x94q\x19P\xa5nX\x14\
+\xa3\xba\x90\xee[\x19\xc7\xb1\xe6<\x15p12\xf1E\
+\xb6\xd3z\xb1\xc5\x05\x1f\x8f\xa5\xd8=\x05n\xe2J\xf2\
+2\x08a6g\x1c\x10\xe1\x12\xf4#\xd3\xc2'\xd5\x8f\
+`]u\x13h\xba*\xc3h\x17Z[\xa9\x19\xd0\x1d\
+2\xcd\xf1\x80\xc5\xf6\xf9\xe0\xa5d\xa3\xd8\xa1\xb0\xf4\x9e\
+\xa7\x96\xde\xe3\xb8tP\x00\xa2\x11\x95\xe6\xaer\xec\xb3\
+fPM9\xf5\xe3\x81b\x97\xcc\xcf\xdc\xdf\xa41\x80\
+6\x1a\xf3\xceQ\xe7\x22\x974\xbe&\xa8\x9e\x92\x0fC\
+\x16\x90\xee\x10\x18\x11P\xddc\xc3E\xad\x80J\x00F\
+\xdc\x03-@\xa3\x87\x8b\xc0`\xebBG\xc3\x90\x8f\x14\
+#\x81\xe3\x93\xb7c\x99!\xde\xf3;\xc9\x02%\x0b\x90\
+K\x02\xa5r\x97\xfa\xfe\xfd\xa3\xe0\x8b\x88\x1bB\xc1\xa2\
+\xc7R0\xac\x951\x96\x0d\xb8\x02<\x9c\xd1\xcf\x1c\x98\
+#\xfc\x06\xfb~\x95\xb3L\x88\xc6\x03\xbb?\x08\x80\xb9\
+\xb7I\xfb\x86\xfac\xd6!G\xbf\xda\x0c\x82\x1f\xd5\x80\
+\x1c\x1de\x0b&\xbf)\x97\x039\xcc\x0a\x8et\xa5\xfa\
+\xfe&\x9dGE\xb5\xaf\xc1\x06\xe7\xbb\x97\xc3\x08\x8dj\
+\x8fL5\xb8\xaf\x9dNG\xb8\xf0\x9eL\x16\xdes\xb3\
+\x85\xaf\x8bN+\x07|Py1Y\x89}j6\x8e\
+D\xe4\xb1\xc8I\xcd\x1e\x1f\x8d\x8bA\xc4\xeeK\x8c\x9e\
+\x0a\xcbq\xb2\xb5\xd8\x1e\xc8bK\x04\xf6\xe3\xb0\xd6N\
+\x19\xf5\x09p\x8c!\xb2\xb9>\x90\xb1\x8c\xbf\x08.\x07\
+R\xf7JT\xe0\xff\x8c\x0b,aq\xb8\xb2w\x02\xbe\
+\xefUKs\xa3\xcc\xd9\xb5g\xb5\x1e{\x87\x5cq\x17\
+\xce\x85\x8f\xbe9\xfc\xd92\xd7V\x92:\xa9\xae~\xd7\
+\xd4W\xee\xfbC\xf2W=?\xfe\xa4\xba\x83n\xdf\x02\
+\xef\xbd\x8d\xb8d\xad\x9dYz\xc8\xca;\x93\x9d\x06\xfd\
+]\x5c\xf3\xb0\xd0\x95*j\xd6\xcb\xbb\x08\xf4+Y\xe8\
+')\xec\xd4\xa8i\x7f\xd7\xc9\xadcW\xf2\x1b\xaat\
+\xb76WQ\x0cK\x0d+/\xc4R\xf4\xea\x85\x0a\xbf\
+Pt\xe9\xb8\xc8\xfbz\xed\xaaV\xcfT\xfa\x1f\xba\xa9\
+mf%i4`rF\xa6\xd77\xca\xa2Y\xa8\xca\
+\xce\xac$UCS\xe5\xd3R\xf3L\xc3=\xcdZM\
+\xa3=S|;l\xdaT\xe1W\xe3V\x0965h\
+\x97\xa2@\x81\xab\xcc\x06\xe0\x8eJ\xab(4{\xdbW\
+\xb8\x91\x80\xa8\xd9\xb8W\xa0,]\xdb5\x99X\xa8\xf6\
+\x9f\xcb\x0e\x9a\x85\xd4\x0cT\x0c\xc4\xf5\xb8\x0c\x91\xb7!\
+\x0b2\xff\x81\x0e\xd9*\x9f\xd6)\xc0\xfck\xb7E\x04\
+\xac\xbd\x97\x0f\xb0\xa3Y\xacQl\x8d\x06\x89y\xd4\x0d\
+\xb1J\xac\xa3E\xb8\x10\x8ch7\x0f\x18\x81\x86\xef\x96\
+i@6\xb8\xa1\x03\x98\xca@)\x03\x7f:1\x8d\xd0\
+\xaa\x9a1\xa4\xd8\xbeR\xfd\x99$3\xa6W\x00C\xe9\
+%>\x8fBjE\x99l\xd2}:HlF\x09\xa5\
+\x04D\xa2\xbb\xd0\x11\xc3\xa4\x96\x0b1\x8e\x5c \xbfZ\
+\xdc\xca\xcf\xa8\xe5\xd4\xe8k5\x5c}b5\xc5$o\
+\xa1\xe1\xdc\xd6\x90,\xf1\x00k\xd5y(\x09[\x5cp\
+\xc5\xab\xcfzY\xdbr\xbb\xe3X\x8a\x11i\x9fD\xe2\
+\x16\x0a\x1d\xc7\xe9X,\x9aj\xdd\xd1\x01sY\xc4\xec\
+\x22a\x07\x8e\x04Sy\xc0\xa2v\xcd>\xe9\xa4\x93\x85\
+f\x9ef\xb24\xd9\x95<\x1f\xce\xb1\xe0u\x00wR\
+\xe5\xe3(\x9d\x81\xd6\xe8{\x15\xceR\xb3\xf7\xa8\xce\xfb\
+Q\x17\x99\xd7\xbe\x1e\xee\x99\xb5\x91&\x22\x1b\x11\xe8\xb0\
+\x98\xb4\x94\xf3\xf2\xc0t\xab\x9f\x9fS\x8f\x8b\xea\x0c\x95\
+\xc55#U\x1f\xa6f\xb4\xb9\x93jz\x92\xc6\x9a9\
+\x19\xe4\xa0\x8b+\xb4\x909\xb3\x02j\xc4\x8ec\xcd\xea\
+\xd5\x9a\xed\x5cGE\x19\xd1L\xe7\xdc$\xd8\xee\xaf\x0f\
+\xb6\x9e\x16\x18\x0d\xc0\x9a\xc9\xb5M\x83\xe7\xfe&\xe0\xaa\
+\xce5\xac\x01'\x0b\xe8\x95\x8f\xea\x94E\x92\xa9\xdd\xa6\
+\x14\x04pu\xa3K!\xfcK\x1e\xdax\xearKI\
+Z\xd5x\xc5x\xcc\xaf\xd0'\x96k\xe8\x0c\xc5\x0d\x8b\
+\x98\x87\xa9\xb28_\xf2\xdd\x11\xe8_\xadu\x19\xb2\x0f\
+\x94\xb8k\xda\x91\x07\xd7hV\xe18X\xc8\xb1U\xb6\
+\x84\x13\x19\xd4\x10I\x99\xa7K[\x17mk8\x7f\xe6\
+mV^\xe99\xe2p>\xdb\xee\xe7\xc1\x92\xa7\xbd\xc4\
+<n\xb4\xae\xd4\x82+h\x5c\x8bh\x83e\xd3\xcbw\
+\x8b\xac\xa0\x02\x8c\x8d\xa7lV\x18+Fi6\xc4\xc4\
+\xbe\xfadc<\x82+#\xec\x1c\x067\xa2\xedS*\
+i7\xf1\x5cs\xefn\x7f\x07D\xcb\xdd\xc1\x0ei\xe6\
+\x8f\xde\x12|\x13\x82o\x06\x06\xdc\x15T\xa0\x1a\xb4\xfa\
+E\xb5:P\xad\xb6\xdc\xe5\xab\xe5.\x05R>\x07[\
+\xf5\x9c\x8d@\xa1S\xa4\xbcC\xfa<\x8a\xe5\x0e\xf1i\
+,\x1bQ\xb2jG`\x7f\x14\xc1bs\xfcSG\xdf\
+\xbbd\x7fE\x04[\xa7\x7f\xaeC\xa6\x1a\xbc\x19\xcbb\
+\xff&H\x9b\xc9\x97k\x0c\xae\xd1\xb8v\x95\x9f\xb0\x81\
+m]\xeaX\x5c4H\xa1 ]\x97I\xd4\x04\xc6\x0d\
+\xf2\xa6\xf0S\x91;U1S3:T'w\xbc\xe8\
+\xc2\xdf*r\x99I$\xa4\x01\x1d\xb0\xc4D\x8eI\xc2\
+`\xaa\xc0k\x17\xb5*\xe5Y\xc9q+\x8c^\xb5;\
++\xca{\xab\xd1\xe4\xacr\x0dr\xac\xfc\x22\x17T\xb3\
+\xcb+PR\x9b\xf90\x07\xe6\xf5x\x12(\x9e;r\
+k\x0a\xa1+\x01]\xe8\x01\xd8\xbe\x99\xa9\xcf\xb9\xfe\x9c\
+i\xbe\xac!\xc9\x8b0\x1f\xc8\xa7b\xc4\x03\xe3\x88y\
+\x87\xd8\x0a\x06{b\x1c\xacLy\xd3cU\xb50\xce\
+\xc1\x14;\x9b\xb2\x22\xbbU\xad%\x06\x1a\xfac\xf4\xac\
+7\x0f\x81\xbe\x10\x11\xffG\x04\x92\xfa/\xd4\xe1\xda\xf7\
+\x9c\x95\x86\xce\x01\x9e\xfc\x1ft\xaeuS\xdfy\x9f\x02\
+d\xe6+\xc6\xf7\x81\x8b\x9dds\xba\xc4VX\xb2x\
+\x0a\xa7\xeb\xf3\xb0\xea\x19\x18\x02l@%\xb3H\xee\xe4\
+\xa3\x10X\x0f\x97/\xb2\xf3\xf0Fv\x9c\x1e\xb6\xb4\xe1\
+\xd9\xc9\xb1\xfc\xf4\x22\x01g\x9atz\xcaG]\xacc\
+\xcc7-6\xd7\xec/i\xb7D\xeeF\x9aB\xea*\
+V\xfe2H\xb3HkexSy\xb0H\xe2\x87\xc7\
+\xe3\xd0\xa7u\xc9.\x99\xf3S\x93>Z\x1fO\x16\x0a\
+\xd6\x99O\x1d\xcf\xe0I\xf1@\xf1\x90\xf9\xe1\xae\xcb#\
+\xd7g\xbb\x00\x1d\x9f\x07u\x89\x89\xd3\xa3\xc6\x07{\xb5\
+\xb1\xc1XD\xbdxHC\xa6\x80\xfdaHe|9\
+\xe4qW=1\xb7N\x15\xf0\x0cJ\x89[\xd8\xae\xd5\
+\x8c\xa3[Q+\xe1q\xeaD'\x22\x22\x81\x90\xa4\xad\
+\xe45\x91\x82\xa8\xfd'\xcc\xe3\xc8cT\xeee\xa7\xd5\
+l\xf7\x8e\x16\xda\xbd\xc6B=c9U\x99\x19\xabc\
+M\xd6G\xb7\xb5V|Q\x91q\x92\x84,M\x8fM\
+L\x10\xf7\xe4R\x87\xbb\x813g\xcbr.8\xf2\xc3\
+K\x1a\x86\x88\x12\xf3\xed\x92\xfcY<\xcc\xa6\xb5\xb8\xc8\
+\xf9\x88^\x95\x96\x06P\xcf\xa5\x81\xc7=\xbc\xe8\xa4l\
+\xa3/\xdcH\xf8\xfe\x09\x8d\x1c\xc09u\xc8\xebpZ\
+F>ML-\x86\x99\xdc)\xb61\xb1\xf8\xd3\xe4W\
+WE\xfa\xa3*B\xceU\xe3\xaeYz\xd7\x07\xae\x1a\
+\x08\x98\xa2\xa0I0\xe7\xa0\x8e\x07\x14\x05\xd3\x93\x83\x9a\
+t\x00\x1b\x01\xb5ZA\xb5\xbc\xc0j$&\x16\x12\x15\
+\x8bI\xbc\x95\x1a\xe0\xcd1o\x7f\x9d\x98\xb7\xbf\xc5\xbc\
+\xc51/A\xba\xaf\x10\xe7\x0e\xd6\x89s?~N\x94\
+3\x09\xc9-j~\x01\xa8\xf9d\x9d\xa8\xf9\xd3\xe3\xe2\
+\x86\xa6\xf6\x11\xfb8\xe6\x98?\x12F\x22\x04\xed\xed\x1e\
+\xe6'\xfcT\xb9_1\xba\xa2A\xc5\xdd3P\xf7^\
+\x09t28X\xd0\xd6\xb6U\x8b\xfc\x9b\xd8\x8bwu\
+\x14\xb1OG\xdc\xbf\x07\xe3,]6\xe0Y\x0c\x16\xaa\
+2\xf1\xe2\x96e/\xf9{\xad\x0el\xf2\xe7K\x01N\
+]\xb7\x96\x9c\x16'\xc4\x19\x13\xea\xbblsjh\xb7\
+\xc6\xf8\xcb\xac\x03\xec\xef4#\xaa.:\xaf,\xce\x1a\
+*`\xa4g\x19\xa6\xe7\xef[\xaa\xecJ\xdc\xed\x8eh\
+\x04\xcfZ\xf60A\xe3\xc9\x1e\x1e\x22\xb8\x14\x83\x81o\
+\x99\xb8\xa4\x9d\xb8S\xf3F\xaa\xb6=m\xdf\xb4\xc1\xe4\
+\xealF\xf4\xc6\xc6\x078uSV\xfa\x01\xfd\xfb\x88\
+\xbb\xe7\x0c\xa8\xc9e\xe8\xbeY\xfd%ZV\x06\xaf\xd5\
+}z&\x07\x96\xad\xf9]w@\xb6\x0c&I4!\
+mZ\xde\x10i\x83*\xb2\xabV&rg[\x13\x0e\
+V\x81\xf4\x89\x99\x9d\x0fHj3[M\xad\x17M\xe7\
+\xd6\x0b\xcd\xd1\x93f\xfe\x9eR?\x8f\x1a\xa0::s\
+\x0c\x0c-\xacK\x0b\xd4\xc1\xe6\xc0k+\xc7\x83\x8a\xfc\
+#\x0f\xd8\xad\x0f$\xd7lF\x92\xd9\x81\x0e\x8b|\xef\
+5>\xc5\x1c}\x8f\xb8\xe7\xf9\xec\x16xIO\xe8\x9b\
+\x0f{\xe3\x10=\x18^\xbb\xb3*\xadf\x81\x13\xb5\xc5\
+e\x9f\x8f}6u?%\xabV\xdf\xeaz\xa7\xf6R\
+\xb1\xc9zO\xe7\x9c\x87s\xc4\x83q\x95\xe4\xcc]\x9b\
+\xf8l]X\xa9\xd3\x1f\xd2\xf3\x92I\xf8f\xb9\x10\x22\
+\xe2h\x1d\xb6%\xe3]f\x09\xb4\xc9\x89\x8e\xd6\x8a\xf0\
+8R\xcbj2\x8d\xcer\xc3\x16\x0e\x9c\xeem\x0e\xe1\
+\x94\xc5\xd0\xabOi\xda\xf2\xffI\x99\xe80\xe8\xa63\
+W\xf8y\x1e^\xfaI\x22\xa0\xc52T\x9b,&n\
+\xa8\xe7\xe9]1\x0b\x98d\x85\x80\xe9}\x06{\xe6\xa5\
+\x1e\x9b\xaa\xa0\x94\xddE\x0a\xb6\x17($\x12\x09\xb3\x80\
+^\xe3Oc\xb6\x08Tz\xee+t#\x9ff x\
+\x867-\x8d\xa8t\x87\xad\xce\x7fHz\x97A\x1fJ\
+[\x93E\xfa;\xf6\xc3!\xec\x9e\xe4n\xbe?:-\
+]\xa8\xd77\x22\xd8\xa5\xa5=\x07\xc0\x05\x97\xed\xfd\x9c\
+\x0d\xd8]\xbe\xd3H\x15,!Q\x96\x15#\x89\xf0\xcc\
+_\xcf\xf0\xd0\xe2\xc4>`V/\x5c\x16\x0b\x90-/\
+\x92\xa6\xc8xH\x8e\xc3\xd0\xe7,\xc6 \xd8\x14_\xc0\
+\x0a\xa2\x11ua\xf2\xb1\xf3\xdf\x00\xb1,\xdf\xe4L\x85\
+\xcf\xf2\x98\x97\xab\x0f\xa6\x0fX\xde\x9862V\xc7I\
+\x09\xdaL\xd8\x8b\xc2\xa6C0P#\xe0#7` \
+\x81\x85>\x8e\xb1\x85\xba\xbd\xe6:\x10\xb7`\xf9\x0c\x18\
+\x11}0\xe1\x07c\x9fF\x84\xdd\xa1\xb8\x8c\xd5\x11H\
+\x10\x5c\xa5\xb9\x0c\xe6x\xd9\x1a\x93\x00\xcc\x18\xfb\xc5\xa4\
+\x04X:\x92\xb6\x99\x03\x1b\x949P\xf4\xf2\xec\xefm\
+@\xe4y]\xf4\xf0U\xc4\xa1g\xaeYE\xc0\xe0M\
+\xbf\x89I\xbc\xa4\x12\xbd\x8dU[F\x0c\xf7\xb6\x11\xc3\
+\xe5b\xd5s\xfa\xbf\xd2*\x8ee\xc9\x83\x99\xfb\x80R\
+\xa6\xd6\xd9F\xb9k\xefS\xb0\x8c\xf2mRd\xf2\x11\
+\x87\x7f\xd6\x1c\xad|\xc8 \x09J\x973\xce|\xcff\
+\xf5\x8b\xc574\xcc,\xef,\x9e\x8a\xa6\xe3\xa9\xde\x85\
+\x93T\xf7\xc0[\xaa_\x19\x10\x13\xc9X\xdd\xd5{\xdb\
+\xaeD\xf0\x5c\xef\xc3\x19\x0fx<l\x10\xacI\x90\x05\
+s\xa8\xad\xcfz%W\xa3\xbaC\xee{\xf0\xeb\xaf\xbd\
+\xbf\xd3\x13Iv}X\x9c\xe0\x99\x22\x84::?\xe2\
+\xd2zEl\x16\x12\xed\xce\xe6\x9c\x17\xfa\xdc\xa9#[\
+F\xbee\xe4[F\xbee\xe4[F\xfe\xe0\x8c\xfc\xc9\
+&0\xf2g[F\xbee\xe4[F\xbee\xe4[F\
+\xbe0#\x7f\xba\xd5\xc8\xb7\x8c|\xcb\xc8\xb7\x8c|\xcb\
+\xc8\xbflF\xfel{\xf4\xe1\xf1\x1d}hgD\x89\
+\xe9\x87\x7f\xbey\xd9}{\xfa\xbcE~\x9b\xcf\xa7'\
+\x87\xb9\xb2+\x9f\x06\xd7YjMg{r\xe2sJ\
+\xaeeON\xa4\xbb\xbe9'&\xf0R\x9a\xf4.\x9a\
+\xe9\xaao\xf0K\x15\xe3\xc1\x89\x9d\x84qY\xbe\xd8\xc5\
+*u-f\x12\xef5\xd49\xd5;\xb9w:N)\
+\x03\x90\xf7\xe5\xefo\xde\x9e?\xef\x1e_<o\xed`\
+\x92\xc9\xa9&!L{\xec,+\xd5j\xe957\xa7\
+\x15S\xe8\xe6J\xa6\x1f\xd7)\x99~\xde&\x1cL?\
+V\xb9Y\xcbsF\xfb\xbbP\xb2](\xa6x\xd2\x08\
+x\xc0\xee\xb8\xe1\xbd(SU\xd4\xf6~\x94\xf4\x13\xb0\
+\xdb^\xf6\xc6\xba\xa7\x96o\x87M\x05\x00\xde\xa7\xf9+\
+\xb1\x1c\xa9\xd9{u\x9a\xf1\xb7[\x1a\x22\xef\xc4;\x17\
+w\x88\xdd\xe93K-z\xf2\x80\xbb\x0e\xd8\x1d|1\
+\xfb\xfe\x8b\xdd\xd6@\xd5.^\x87\xd9\xee\xe0\xe6l\x0c\
+\xa6(,\x01\xb9\xb3\xff\xa5a\x8a\xe9D\xd1\xe7\xc1\x8a\
+5\xee\x16JA\xc9\xda\x0fI\xd0\x9bt\xeaT\x1f\x14\
+\x8aW\x7f\xd8t%gD\x0d\xc7\x8cR%ao\xc5\
+'\x8b\xc6Rh\xab@e\xf2\xff\x19V^\xa1\xf4`\
+\xa7\xa2\xcc\xef\xa8\xab~\x9f\xbdz\xa2\xd2p\x93M^\
+\xe6H^}\xefu\xef\x9e[\xea\xf6\xc4Rl2\x9b\
+T@\xe8*\xd7wv\x0c\xf5\xee\x9c\x04\xd9u\x8d\xc5\
+\xcfH\xcf\x1d\x00C}x\xb6&\x80M\xe2\xa1>\x80\
+\x9b>\xb2U\x95`\x9e\xa4Q\xcfN\xcdI\x9a\xbf.\
+\xbfb>\x7fbp\xbei\xeea\x99\xea\x9a\xbd@\xaf\
+\xd0.)/y\xe3]\xc4\xa1?u\xe6e\xba\x14\xe7\
+}\xe2\x1d-{\xa38(\xdf\xf1\x09\x1b\xd2\x1b\x8e\xaa\
+\xf5\x19b\x192_\xe7B\x8a\xf0X\x9e\xa8\xe7%W\
+\xb2\xa6\xf5Ny\xa4\xafw\xcd\xb7E\xfaT\xff^\xf6\
+\xdf0\xe6\x95![\x1c\xd0\x10!\x96\x9b\xe5\x05\x14]\
+\x0a\xdc\x852P\x0ca\x9f\xd5\xc5\xbd\xaf\xc5\x0d;\x1d\
+G\xc9\x1a\x0f\xcaB\xdcY\xdds<P\x93\xabm\xaa\
+{&|_\xdc\xe2\xa1\xa7(C\x86r\xf2\x9fv\x8f\
+\x17\xd0\x16V\x81G\x99\xee\xd5\x83\xf9\x86\x19.\xbeH\
+{8a\xc0\x98A\xc2\xfelS\xf99\xbeb]\xb1\
+TP\xa1\xb0\x89aj\x87\x04WP\xc5,\xacl\xc9\
+\xf4\x1a\xe4\xa7\x06\xf34a\xf0\x05\xf4T\xa5\xd5\x8d\xee\
+\xe7\x1a\x84\x22\xe6\xfa\xd5\x98GG\xe4\xd2IJ\xcf\x84\
+\xc0\x0b\x11\x7f#{${=\xbb\x9e\x14\xac_\xff\xa8\
+\x1e\xc4\xdaL\x9d5Q\x0b\x13+x\xd3jlT\xbb\
+\xb7\xdb7\xe6\xb33\x9c\xe0Yq\xdbq\xa6\x95\xaa$\
+r\xd2+\x1as7\xd5\x1dNd\xc9\xab\xf8ns\xac\
+\xd1$wO\xb0'\xe3+\xedSn?\x0d\xee\xe8\xb0\
+\xcbt\xff\x0a\x0f\x8c/\xed\xac@\xcet\x8f.$u\
+\xaf-\x8ed\xcfC\xb6!\x04\x8bo@]\x0a\x88x\
+\x855\xc1\xde\xac\x00\x09\x5cx~\x07\x9d+\x01\xd3\x1d\
+\xad\x05\xfc\xb9\x81_+\xb51k[-t\x96\xdb\xb1\
+\xfd5\xecX\xe1\xbe\xe6\xa56\xecLD#*\xc9\xbb\
+H\xdcp|\xf3\x81\xbe\xc9\xb5t\xd7\xb2\xf7\xa3}\x97\
+?\xfa\x7f5\x8e\xefkv\xb8\x04\xc3\xbe\xaeM>X\
+\xc3&W]\xc6\xb3\xd4n\xbf\xc2NI\xaeW\xa2,\
+\xd2Z\x1a\x9d\xc7\xb8\xafk\x03\x9f\xaca\x03\x0bv\xed\
+R\xfb\x96\x18\x81\xf6L\xd5\x80=_\xd7\xce=]\xc0\
+\xa63*\x89V\xe6W\xb9\xe2ez\x05Gnh\xb5\
+\x0e\xa3Kc\xf9\xfb\xb1\xf2F\xa6\x1a\xaf0\xd3\x8aD\
+\xadY{n\xaf\xf8\xb6\x0b\xdb\x17@\xce\x88tt\xe8\
+8n\xc4\x00\x81\xdf^\xfd\x0f\xc0\xde\x9e\x99X\x09&\
+\x97\xbd\x93\xbdY\x0f%o4h\xd6\x81\xe9*\xb4f\
+=\x95\xb8\xb7\x9au\xb0\xe4;\x8aJ]\x1a\x93\xff\x03\
+\xfc\x5cl\xba\
 \x00\x00\x03\xb0\
 i\
 mport QtQuick\x0d\x0ai\
 mport QtQuick.Co\
 ntrols.Material\x0d\
 \x0aimport QtQuick.\
 Shapes\x0d\x0a\x0d\x0a// ada\
@@ -2373,37 +2374,37 @@
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00\x00\x00\x02\x00\x00\x00\x02\x00\x00\x00\x02\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00\x0c\x00\x02\x00\x00\x00\x0e\x00\x00\x00\x04\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00&\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
 \x00\x00\x01\x8f\xd8L\xcf\x5c\
-\x00\x00\x01\x82\x00\x00\x00\x00\x00\x01\x00\x00s\xb5\
+\x00\x00\x01\x82\x00\x00\x00\x00\x00\x01\x00\x00s\xc3\
 \x00\x00\x01\x8d\xe2\x17bW\
-\x00\x00\x02\x02\x00\x01\x00\x00\x00\x01\x00\x00\x85|\
+\x00\x00\x02\x02\x00\x01\x00\x00\x00\x01\x00\x00\x85\x8a\
 \x00\x00\x01\x8f\xac\xf8\xad\x92\
 \x00\x00\x01\x0e\x00\x01\x00\x00\x00\x01\x00\x00P\xf0\
-\x00\x00\x01\x8f\xd8L\xb4\xe6\
-\x00\x00\x01\xe6\x00\x01\x00\x00\x00\x01\x00\x00z\x8c\
+\x00\x00\x01\x8f\xde=m\xe0\
+\x00\x00\x01\xe6\x00\x01\x00\x00\x00\x01\x00\x00z\x9a\
 \x00\x00\x01\x8f\xad\x1a\x0d\x93\
 \x00\x00\x00f\x00\x01\x00\x00\x00\x01\x00\x00*S\
 \x00\x00\x01\x8f\xad\x0c\x00M\
 \x00\x00\x00\xe4\x00\x00\x00\x00\x00\x01\x00\x00NV\
 \x00\x00\x01\x8f\xac\xf8\xad\x94\
-\x00\x00\x02&\x00\x01\x00\x00\x00\x01\x00\x00\x89\x93\
+\x00\x00\x02&\x00\x01\x00\x00\x00\x01\x00\x00\x89\xa1\
 \x00\x00\x01\x8f\xad\x0c\x00K\
 \x00\x00\x00\x84\x00\x00\x00\x00\x00\x01\x00\x003v\
 \x00\x00\x01\x8d\xe2\x17b\x5c\
-\x00\x00\x01\xd4\x00\x00\x00\x00\x00\x01\x00\x00x\xba\
+\x00\x00\x01\xd4\x00\x00\x00\x00\x00\x01\x00\x00x\xc8\
 \x00\x00\x01\x8d\xe2\x17bZ\
 \x00\x00\x012\x00\x00\x00\x00\x00\x01\x00\x00\x5c\xfa\
 \x00\x00\x01\x8f\xac\xf8\xad\x8c\
 \x00\x00\x01V\x00\x01\x00\x00\x00\x01\x00\x00bj\
-\x00\x00\x01\x8f\xd8L\xd3\xba\
-\x00\x00\x01\xb0\x00\x01\x00\x00\x00\x01\x00\x00wi\
+\x00\x00\x01\x8f\xdeF\x16{\
+\x00\x00\x01\xb0\x00\x01\x00\x00\x00\x01\x00\x00ww\
 \x00\x00\x01\x8e#\xc6#s\
 \x00\x00\x00<\x00\x01\x00\x00\x00\x01\x00\x00\x0a\xb7\
 \x00\x00\x01\x8f\xd8L\xcfc\
 \x00\x00\x00\xb4\x00\x00\x00\x00\x00\x01\x00\x00B5\
 \x00\x00\x01\x8f\xac\xf8\xad\x95\
 "
```

### Comparing `libresvip-1.1.5/libresvip/gui/__main__.py` & `libresvip-1.1.6/libresvip/gui/__main__.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/gui/models/list_models.py` & `libresvip-1.1.6/libresvip/gui/models/list_models.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/gui/models/table_models.py` & `libresvip-1.1.6/libresvip/gui/models/table_models.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/gui/modules/__init__.py` & `libresvip-1.1.6/libresvip/gui/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/gui/modules/application.py` & `libresvip-1.1.6/libresvip/gui/modules/application.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/gui/modules/clipboard.py` & `libresvip-1.1.6/libresvip/gui/modules/clipboard.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/gui/modules/config_items.py` & `libresvip-1.1.6/libresvip/gui/modules/config_items.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,18 +17,15 @@
     LibreSvipSettings,
     save_settings,
     settings,
 )
 from libresvip.core.constants import res_dir
 from libresvip.extension.manager import plugin_manager
 from libresvip.gui.models.list_models import LyricReplacementPresetsModel, ModelProxy
-from libresvip.gui.models.table_models import (
-    LyricReplacementRulesTableModel,
-    PluginCadidatesTableModel,
-)
+from libresvip.gui.models.table_models import LyricReplacementRulesTableModel
 
 from .application import app
 
 QML_IMPORT_NAME = "LibreSVIP"
 QML_IMPORT_MAJOR_VERSION = 1
 QML_IMPORT_MINOR_VERSION = 0
 
@@ -65,15 +62,14 @@
 
     def __init__(self, parent: Optional[QObject] = None) -> None:
         super().__init__(parent=parent)
         self.folder_presets = ModelProxy({"path": ""})
         self.folder_presets.append_many(
             [{"path": self.posix_path(path)} for path in settings.folder_presets]
         )
-        self.plugin_candidates = PluginCadidatesTableModel()
         self.lyric_replacement_presets = LyricReplacementPresetsModel()
         app.aboutToQuit.connect(self.save_settings)
 
     def save_settings(self) -> None:
         settings.folder_presets = [pathlib.Path(item["path"]) for item in self.folder_presets.items]
         save_settings()
 
@@ -121,27 +117,14 @@
     def set_theme(self, theme: str) -> None:
         dark_mode = DarkMode(theme)
         settings.dark_mode = dark_mode
         self.theme_changed.emit(theme)
 
     theme = Property(str, get_theme, set_theme, notify=theme_changed)
 
-    @Slot(int, result=bool)
-    def toggle_plugin(self, index: int) -> bool:
-        key = plugin_manager._candidates[index][1].suffix
-        if key in plugin_manager.plugin_registry and key not in settings.disabled_plugins:
-            settings.disabled_plugins.append(key)
-        elif key in settings.disabled_plugins:
-            settings.disabled_plugins.remove(key)
-        else:
-            return False
-        plugin_manager.import_plugins(reload=True)
-        self.plugin_candidates.reload_formats()
-        return True
-
     @Slot(str, result=bool)
     def enabled(self, key: str) -> bool:
         return key in plugin_manager.plugin_registry
 
     @staticmethod
     def posix_path(path: pathlib.Path) -> str:
         return str(path.as_posix())
```

### Comparing `libresvip-1.1.5/libresvip/gui/modules/font_loader.py` & `libresvip-1.1.6/libresvip/gui/modules/font_loader.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/gui/modules/frameless_window.py` & `libresvip-1.1.6/libresvip/gui/modules/frameless_window.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/gui/modules/frameless_window_win32.py` & `libresvip-1.1.6/libresvip/gui/modules/frameless_window_win32.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/gui/modules/locale_switcher.py` & `libresvip-1.1.6/libresvip/gui/modules/locale_switcher.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/gui/modules/notifier.py` & `libresvip-1.1.6/libresvip/gui/modules/notifier.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/gui/modules/task_manager.py` & `libresvip-1.1.6/libresvip/gui/modules/task_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 from __feature__ import snake_case, true_property  # isort:skip # noqa: F401  # type: ignore[import-not-found,reportMissingImports]
 
 from libresvip.core.config import ConversionMode, get_ui_settings, settings
 from libresvip.core.warning_types import CatchWarnings
 from libresvip.extension.manager import middleware_manager, plugin_manager
 from libresvip.gui.models.base_task import BaseTask
 from libresvip.gui.models.list_models import ModelProxy
+from libresvip.gui.models.table_models import PluginCadidatesTableModel
 from libresvip.model.base import BaseComplexModel, BaseModel, Project
 from libresvip.utils.text import supported_charset_names
 
 from .url_opener import open_path
 
 QML_IMPORT_NAME = "LibreSVIP"
 QML_IMPORT_MAJOR_VERSION = 1
@@ -398,14 +399,28 @@
         self.output_format_changed.connect(self.set_output_fields)
         self.output_format_changed.connect(self.reset_output_ext)
         self._start_conversion.connect(self.start)
         self.timer = QTimer()
         self.timer.interval = 100
         self.timer.timeout.connect(self.check_busy)
         self.tasks.rowsAboutToBeRemoved.connect(self.delete_tmp_file)
+        self.plugin_candidates = PluginCadidatesTableModel()
+
+    @Slot(int)
+    def toggle_plugin(self, index: int) -> None:
+        key = plugin_manager._candidates[index][1].suffix
+        if key in plugin_manager.plugin_registry and key not in settings.disabled_plugins:
+            settings.disabled_plugins.append(key)
+        elif key in settings.disabled_plugins:
+            settings.disabled_plugins.remove(key)
+        else:
+            return
+        plugin_manager.import_plugins(reload=True)
+        self.plugin_candidates.reload_formats()
+        self.reload_formats()
 
     def _on_tasks_changed(self, index: QModelIndex, start: int, end: int) -> None:
         self.task_count_changed.emit(len(self.tasks))
 
     def get_conversion_mode(self) -> str:
         return self._conversion_mode.value
```

### Comparing `libresvip-1.1.5/libresvip/gui/modules/vendor/qasync/__init__.py` & `libresvip-1.1.6/libresvip/gui/modules/vendor/qasync/__init__.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/gui/modules/vendor/qasync/_unix.py` & `libresvip-1.1.6/libresvip/gui/modules/vendor/qasync/_unix.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/gui/modules/vendor/qasync/_windows.py` & `libresvip-1.1.6/libresvip/gui/modules/vendor/qasync/_windows.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/gui/modules/win32_constants.py` & `libresvip-1.1.6/libresvip/gui/modules/win32_constants.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/middlewares/pitch_shift/pitch_shift.py` & `libresvip-1.1.6/libresvip/middlewares/pitch_shift/pitch_shift.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/middlewares/project_zoom/options.py` & `libresvip-1.1.6/libresvip/middlewares/project_zoom/options.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/middlewares/pronounciation_conversion/options.py` & `libresvip-1.1.6/libresvip/middlewares/pronounciation_conversion/options.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/middlewares/pronounciation_conversion/pronounciation_conversion.py` & `libresvip-1.1.6/libresvip/middlewares/pronounciation_conversion/pronounciation_conversion.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/middlewares/remove_short_silences/options.py` & `libresvip-1.1.6/libresvip/middlewares/remove_short_silences/options.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/middlewares/remove_short_silences/remove_short_silences.py` & `libresvip-1.1.6/libresvip/middlewares/remove_short_silences/remove_short_silences.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/middlewares/replace_lyric/replace_lyric.py` & `libresvip-1.1.6/libresvip/middlewares/replace_lyric/replace_lyric.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/model/base.py` & `libresvip-1.1.6/libresvip/model/base.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/model/option_mixins.py` & `libresvip-1.1.6/libresvip/model/option_mixins.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/model/point.py` & `libresvip-1.1.6/libresvip/model/point.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/model/relative_pitch_curve.py` & `libresvip-1.1.6/libresvip/model/relative_pitch_curve.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/model/reset_time_axis.py` & `libresvip-1.1.6/libresvip/model/reset_time_axis.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/acep/ace-studio.yapsy-plugin` & `libresvip-1.1.6/libresvip/plugins/acep/ace-studio.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/acep/ace_curve_utils.py` & `libresvip-1.1.6/libresvip/plugins/acep/ace_curve_utils.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/acep/ace_studio_converter.py` & `libresvip-1.1.6/libresvip/plugins/acep/ace_studio_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/acep/ace_studio_generator.py` & `libresvip-1.1.6/libresvip/plugins/acep/ace_studio_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/acep/ace_studio_parser.py` & `libresvip-1.1.6/libresvip/plugins/acep/ace_studio_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/acep/acep_io.py` & `libresvip-1.1.6/libresvip/plugins/acep/acep_io.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/acep/base_pitch_curve.py` & `libresvip-1.1.6/libresvip/plugins/acep/base_pitch_curve.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/acep/curve_segment_utils.py` & `libresvip-1.1.6/libresvip/plugins/acep/curve_segment_utils.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/acep/model.py` & `libresvip-1.1.6/libresvip/plugins/acep/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/acep/options.py` & `libresvip-1.1.6/libresvip/plugins/acep/options.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/acep/singers.py` & `libresvip-1.1.6/libresvip/plugins/acep/singers.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/acep/time_utils.py` & `libresvip-1.1.6/libresvip/plugins/acep/time_utils.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/aisp/aisingers_converter.py` & `libresvip-1.1.6/libresvip/plugins/aisp/aisingers_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/aisp/aisingers_generator.py` & `libresvip-1.1.6/libresvip/plugins/aisp/aisingers_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import bisect
 import dataclasses
 from typing import Union
 
 from libresvip.core.constants import DEFAULT_PHONEME
+from libresvip.core.lyric_phoneme.chinese import get_pinyin_series
 from libresvip.core.time_sync import TimeSynchronizer
 from libresvip.model.base import (
     InstrumentalTrack,
     Note,
     ParamCurve,
     Project,
     SingingTrack,
@@ -168,15 +169,17 @@
         ais_notes = []
         for note in track.note_list:
             ais_note = AISNote(
                 midi_no=note.key_number - 12,
                 start=round(note.start_pos / 15),
                 length=round(note.length / 15),
                 lyric=note.lyric,
-                pinyin=note.pronunciation or DEFAULT_PHONEME,
+                pinyin=note.pronunciation
+                or " ".join(get_pinyin_series(note.lyric))
+                or DEFAULT_PHONEME,
                 triple=False,
                 pit="0x500",
             )
             if pitch_points := self.generate_pitch(track.edited_params.pitch, note):
                 ais_note.pit = pitch_points
             ais_notes.append(ais_note)
         return ais_notes
```

### Comparing `libresvip-1.1.5/libresvip/plugins/aisp/aisingers_parser.py` & `libresvip-1.1.6/libresvip/plugins/aisp/aisingers_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/aisp/aisp.yapsy-plugin` & `libresvip-1.1.6/libresvip/plugins/aisp/aisp.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/aisp/model.py` & `libresvip-1.1.6/libresvip/plugins/aisp/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ccs/ccs.yapsy-plugin` & `libresvip-1.1.6/libresvip/plugins/ccs/ccs.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ccs/cevio_converter.py` & `libresvip-1.1.6/libresvip/plugins/ccs/cevio_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ccs/cevio_generator.py` & `libresvip-1.1.6/libresvip/plugins/ccs/cevio_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ccs/cevio_parser.py` & `libresvip-1.1.6/libresvip/plugins/ccs/cevio_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ccs/cevio_pitch.py` & `libresvip-1.1.6/libresvip/plugins/ccs/cevio_pitch.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ccs/model.py` & `libresvip-1.1.6/libresvip/plugins/ccs/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ccs/options.py` & `libresvip-1.1.6/libresvip/plugins/ccs/options.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ds/dicts/opencpop-extension.txt` & `libresvip-1.1.6/libresvip/plugins/ds/dicts/opencpop-extension.txt`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ds/dicts/opencpop-strict.txt` & `libresvip-1.1.6/libresvip/plugins/ds/dicts/opencpop-strict.txt`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ds/dicts/opencpop.txt` & `libresvip-1.1.6/libresvip/plugins/ds/dicts/opencpop.txt`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ds/diffsinger_converter.py` & `libresvip-1.1.6/libresvip/plugins/ds/diffsinger_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ds/diffsinger_generator.py` & `libresvip-1.1.6/libresvip/plugins/ds/diffsinger_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ds/diffsinger_parser.py` & `libresvip-1.1.6/libresvip/plugins/ds/diffsinger_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ds/ds.yapsy-plugin` & `libresvip-1.1.6/libresvip/plugins/ds/ds.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ds/model.py` & `libresvip-1.1.6/libresvip/plugins/ds/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ds/models/ds_note.py` & `libresvip-1.1.6/libresvip/plugins/ds/models/ds_note.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ds/models/ds_project.py` & `libresvip-1.1.6/libresvip/plugins/ds/models/ds_project.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ds/options.py` & `libresvip-1.1.6/libresvip/plugins/ds/options.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ds/phoneme_dict.py` & `libresvip-1.1.6/libresvip/plugins/ds/phoneme_dict.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ds/utils/gender_param_utils.py` & `libresvip-1.1.6/libresvip/plugins/ds/utils/gender_param_utils.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ds/utils/note_list_util.py` & `libresvip-1.1.6/libresvip/plugins/ds/utils/note_list_util.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ds/utils/pinyin_util.py` & `libresvip-1.1.6/libresvip/plugins/ds/utils/pinyin_util.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ds/utils/pitch_param_utils.py` & `libresvip-1.1.6/libresvip/plugins/ds/utils/pitch_param_utils.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ds/utils/project_util.py` & `libresvip-1.1.6/libresvip/plugins/ds/utils/project_util.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/dv/constants.py` & `libresvip-1.1.6/libresvip/plugins/dv/constants.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/dv/deepvocal_converter.py` & `libresvip-1.1.6/libresvip/plugins/dv/deepvocal_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/dv/deepvocal_pitch.py` & `libresvip-1.1.6/libresvip/plugins/dv/deepvocal_pitch.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/dv/dv.yapsy-plugin` & `libresvip-1.1.6/libresvip/plugins/dv/dv.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/dv/dv_generator.py` & `libresvip-1.1.6/libresvip/plugins/dv/dv_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/dv/dv_parser.py` & `libresvip-1.1.6/libresvip/plugins/dv/dv_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/dv/model.py` & `libresvip-1.1.6/libresvip/plugins/dv/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/gj/constants.py` & `libresvip-1.1.6/libresvip/plugins/gj/constants.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/gj/gjgj.yapsy-plugin` & `libresvip-1.1.6/libresvip/plugins/gj/gjgj.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/gj/gjgj_converter.py` & `libresvip-1.1.6/libresvip/plugins/gj/gjgj_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/gj/gjgj_generator.py` & `libresvip-1.1.6/libresvip/plugins/gj/gjgj_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/gj/gjgj_parser.py` & `libresvip-1.1.6/libresvip/plugins/gj/gjgj_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/gj/model.py` & `libresvip-1.1.6/libresvip/plugins/gj/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/gj/options.py` & `libresvip-1.1.6/libresvip/plugins/gj/options.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/json/jsonsvip.yapsy-plugin` & `libresvip-1.1.6/libresvip/plugins/json/jsonsvip.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/json/jsonsvip_converter.py` & `libresvip-1.1.6/libresvip/plugins/json/jsonsvip_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/lrc/lrc.yapsy-plugin` & `libresvip-1.1.6/libresvip/plugins/lrc/lrc.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/lrc/lrc_generator.py` & `libresvip-1.1.6/libresvip/plugins/lrc/lrc_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/lrc/model.py` & `libresvip-1.1.6/libresvip/plugins/lrc/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/lrc/options.py` & `libresvip-1.1.6/libresvip/plugins/lrc/options.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/lrc/template.py` & `libresvip-1.1.6/libresvip/plugins/lrc/template.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/mid/constants.py` & `libresvip-1.1.6/libresvip/plugins/mid/constants.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/mid/mid.yapsy-plugin` & `libresvip-1.1.6/libresvip/plugins/mid/mid.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/mid/midi_converter.py` & `libresvip-1.1.6/libresvip/plugins/mid/midi_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/mid/midi_generator.py` & `libresvip-1.1.6/libresvip/plugins/mid/midi_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/mid/midi_parser.py` & `libresvip-1.1.6/libresvip/plugins/mid/midi_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/mid/midi_pitch.py` & `libresvip-1.1.6/libresvip/plugins/mid/midi_pitch.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/mid/options.py` & `libresvip-1.1.6/libresvip/plugins/mid/options.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/mtp/model.py` & `libresvip-1.1.6/libresvip/plugins/mtp/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/mtp/mtp.yapsy-plugin` & `libresvip-1.1.6/libresvip/plugins/mtp/mtp.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/mtp/muta_converter.py` & `libresvip-1.1.6/libresvip/plugins/mtp/muta_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/mtp/muta_generator.py` & `libresvip-1.1.6/libresvip/plugins/mtp/muta_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/mtp/muta_parser.py` & `libresvip-1.1.6/libresvip/plugins/mtp/muta_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/musicxml/model.py` & `libresvip-1.1.6/libresvip/plugins/musicxml/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/musicxml/models/mxml2.py` & `libresvip-1.1.6/libresvip/plugins/musicxml/models/mxml2.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/musicxml/models/xlink.py` & `libresvip-1.1.6/libresvip/plugins/musicxml/models/xlink.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/musicxml/musicxml.yapsy-plugin` & `libresvip-1.1.6/libresvip/plugins/musicxml/musicxml.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/musicxml/musicxml_converter.py` & `libresvip-1.1.6/libresvip/plugins/musicxml/musicxml_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/musicxml/musicxml_generator.py` & `libresvip-1.1.6/libresvip/plugins/musicxml/musicxml_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/musicxml/musicxml_parser.py` & `libresvip-1.1.6/libresvip/plugins/musicxml/musicxml_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/nn/model.py` & `libresvip-1.1.6/libresvip/plugins/nn/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/nn/niaoniao_converter.py` & `libresvip-1.1.6/libresvip/plugins/nn/niaoniao_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/nn/niaoniao_generator.py` & `libresvip-1.1.6/libresvip/plugins/nn/niaoniao_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/nn/niaoniao_parser.py` & `libresvip-1.1.6/libresvip/plugins/nn/niaoniao_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/nn/nn.yapsy-plugin` & `libresvip-1.1.6/libresvip/plugins/nn/nn.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/nn/template.py` & `libresvip-1.1.6/libresvip/plugins/nn/template.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ppsf/legacy_model.py` & `libresvip-1.1.6/libresvip/plugins/ppsf/legacy_model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ppsf/model.py` & `libresvip-1.1.6/libresvip/plugins/ppsf/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ppsf/piapro_studio_converter.py` & `libresvip-1.1.6/libresvip/plugins/ppsf/piapro_studio_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ppsf/piapro_studio_generator.py` & `libresvip-1.1.6/libresvip/plugins/ppsf/piapro_studio_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ppsf/piapro_studio_legacy_parser.py` & `libresvip-1.1.6/libresvip/plugins/ppsf/piapro_studio_legacy_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ppsf/piapro_studio_nt_parser.py` & `libresvip-1.1.6/libresvip/plugins/ppsf/piapro_studio_nt_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ppsf/ppsf.yapsy-plugin` & `libresvip-1.1.6/libresvip/plugins/ppsf/ppsf.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ppsf/ppsf_interval_dict.py` & `libresvip-1.1.6/libresvip/plugins/ppsf/ppsf_interval_dict.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/s5p/model.py` & `libresvip-1.1.6/libresvip/plugins/s5p/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/s5p/s5p.yapsy-plugin` & `libresvip-1.1.6/libresvip/plugins/s5p/s5p.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/s5p/synthv_editor_converter.py` & `libresvip-1.1.6/libresvip/plugins/s5p/synthv_editor_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/s5p/synthv_editor_generator.py` & `libresvip-1.1.6/libresvip/plugins/s5p/synthv_editor_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/s5p/synthv_editor_parser.py` & `libresvip-1.1.6/libresvip/plugins/s5p/synthv_editor_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/srt/options.py` & `libresvip-1.1.6/libresvip/plugins/srt/options.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/srt/srt.yapsy-plugin` & `libresvip-1.1.6/libresvip/plugins/srt/srt.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/srt/srt_generator.py` & `libresvip-1.1.6/libresvip/plugins/srt/srt_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/svg/coordinate_helper.py` & `libresvip-1.1.6/libresvip/plugins/svg/coordinate_helper.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/svg/options.py` & `libresvip-1.1.6/libresvip/plugins/svg/options.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/svg/svg.yapsy-plugin` & `libresvip-1.1.6/libresvip/plugins/svg/svg.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/svg/svg_converter.py` & `libresvip-1.1.6/libresvip/plugins/svg/svg_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/svg/svg_factory.py` & `libresvip-1.1.6/libresvip/plugins/svg/svg_factory.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/svg/svg_generator.py` & `libresvip-1.1.6/libresvip/plugins/svg/svg_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/svip/binsvip.yapsy-plugin` & `libresvip-1.1.6/libresvip/plugins/svip/binsvip.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/svip/binsvip_converter.py` & `libresvip-1.1.6/libresvip/plugins/svip/binsvip_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/svip/binsvip_generator.py` & `libresvip-1.1.6/libresvip/plugins/svip/binsvip_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/svip/binsvip_parser.py` & `libresvip-1.1.6/libresvip/plugins/svip/binsvip_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/svip/models.py` & `libresvip-1.1.6/libresvip/plugins/svip/models.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/svip/msnrbf/binary_models.py` & `libresvip-1.1.6/libresvip/plugins/svip/msnrbf/binary_models.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/svip/msnrbf/nrbf_iobase.py` & `libresvip-1.1.6/libresvip/plugins/svip/msnrbf/nrbf_iobase.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/svip/msnrbf/svip_reader.py` & `libresvip-1.1.6/libresvip/plugins/svip/msnrbf/svip_reader.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/svip/msnrbf/svip_writer.py` & `libresvip-1.1.6/libresvip/plugins/svip/msnrbf/svip_writer.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/svip/msnrbf/xstudio_models.py` & `libresvip-1.1.6/libresvip/plugins/svip/msnrbf/xstudio_models.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/svip/options.py` & `libresvip-1.1.6/libresvip/plugins/svip/options.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/svip/singers.json` & `libresvip-1.1.6/libresvip/plugins/svip/singers.json`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/svip3/model.py` & `libresvip-1.1.6/libresvip/plugins/svip3/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/svip3/singers.json` & `libresvip-1.1.6/libresvip/plugins/svip3/singers.json`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/svip3/svip3.yapsy-plugin` & `libresvip-1.1.6/libresvip/plugins/svip3/svip3.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/svip3/svip3_converter.py` & `libresvip-1.1.6/libresvip/plugins/svip3/svip3_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/svip3/svip3_generator.py` & `libresvip-1.1.6/libresvip/plugins/svip3/svip3_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/svip3/svip3_parser.py` & `libresvip-1.1.6/libresvip/plugins/svip3/svip3_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/svp/constants.py` & `libresvip-1.1.6/libresvip/plugins/svp/constants.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/svp/lambert_w.py` & `libresvip-1.1.6/libresvip/plugins/svp/lambert_w.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/svp/layer_generator.py` & `libresvip-1.1.6/libresvip/plugins/svp/layer_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/svp/model.py` & `libresvip-1.1.6/libresvip/plugins/svp/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -587,11 +587,11 @@
     name: str = "Track 1"
     render_enabled: bool = Field(default=True, alias="renderEnabled")
 
 
 class SVProject(BaseModel):
     library: list[SVGroup] = Field(default_factory=list)
     render_config: SVRenderConfig = Field(default_factory=SVRenderConfig, alias="renderConfig")
-    instant_mode_enabled: Optional[bool] = Field(False, alias="instantModeEnabled")
+    instant_mode_enabled: Optional[bool] = Field(True, alias="instantModeEnabled")
     time_sig: SVTime = Field(default_factory=SVTime, alias="time")
     tracks: list[SVTrack] = Field(default_factory=list)
     version: int = 113
```

### Comparing `libresvip-1.1.5/libresvip/plugins/svp/options.py` & `libresvip-1.1.6/libresvip/plugins/svp/options.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/svp/param_expression.py` & `libresvip-1.1.6/libresvip/plugins/svp/param_expression.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/svp/phoneme_categories.json` & `libresvip-1.1.6/libresvip/plugins/svp/phoneme_categories.json`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/svp/phoneme_dictionary.json` & `libresvip-1.1.6/libresvip/plugins/svp/phoneme_dictionary.json`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/svp/phoneme_utils.py` & `libresvip-1.1.6/libresvip/plugins/svp/phoneme_utils.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/svp/pitch_simulator.py` & `libresvip-1.1.6/libresvip/plugins/svp/pitch_simulator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/svp/pitch_slide.py` & `libresvip-1.1.6/libresvip/plugins/svp/pitch_slide.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/svp/svp.yapsy-plugin` & `libresvip-1.1.6/libresvip/plugins/svp/svp.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/svp/synthv_generator.py` & `libresvip-1.1.6/libresvip/plugins/svp/synthv_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/svp/synthv_parser.py` & `libresvip-1.1.6/libresvip/plugins/svp/synthv_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/svp/synthv_studio_converter.py` & `libresvip-1.1.6/libresvip/plugins/svp/synthv_studio_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/svp/track_merge_utils.py` & `libresvip-1.1.6/libresvip/plugins/svp/track_merge_utils.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/tlp/model.py` & `libresvip-1.1.6/libresvip/plugins/tlp/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/tlp/tunelab_converter.py` & `libresvip-1.1.6/libresvip/plugins/tlp/tunelab_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/tlp/tunelab_generator.py` & `libresvip-1.1.6/libresvip/plugins/tlp/tunelab_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/tlp/tunelab_parser.py` & `libresvip-1.1.6/libresvip/plugins/tlp/tunelab_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/tssln/model.py` & `libresvip-1.1.6/libresvip/plugins/tssln/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/tssln/tssln.yapsy-plugin` & `libresvip-1.1.6/libresvip/plugins/tssln/tssln.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/tssln/value_tree.py` & `libresvip-1.1.6/libresvip/plugins/tssln/value_tree.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/tssln/voisona_converter.py` & `libresvip-1.1.6/libresvip/plugins/tssln/voisona_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/tssln/voisona_generator.py` & `libresvip-1.1.6/libresvip/plugins/tssln/voisona_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/tssln/voisona_parser.py` & `libresvip-1.1.6/libresvip/plugins/tssln/voisona_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/tssln/voisona_pitch.py` & `libresvip-1.1.6/libresvip/plugins/tssln/voisona_pitch.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ufdata/model.py` & `libresvip-1.1.6/libresvip/plugins/ufdata/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ufdata/ufdata.yapsy-plugin` & `libresvip-1.1.6/libresvip/plugins/ufdata/ufdata.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ufdata/ufdata_converter.py` & `libresvip-1.1.6/libresvip/plugins/ufdata/ufdata_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ufdata/ufdata_generator.py` & `libresvip-1.1.6/libresvip/plugins/ufdata/ufdata_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ufdata/ufdata_parser.py` & `libresvip-1.1.6/libresvip/plugins/ufdata/ufdata_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ust/interpolation.py` & `libresvip-1.1.6/libresvip/plugins/ust/interpolation.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ust/model.py` & `libresvip-1.1.6/libresvip/plugins/ust/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ust/options.py` & `libresvip-1.1.6/libresvip/plugins/ust/options.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ust/pitch_mode1.py` & `libresvip-1.1.6/libresvip/plugins/ust/pitch_mode1.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ust/pitch_mode2.py` & `libresvip-1.1.6/libresvip/plugins/ust/pitch_mode2.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ust/rdp_simplification.py` & `libresvip-1.1.6/libresvip/plugins/ust/rdp_simplification.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ust/resampling.py` & `libresvip-1.1.6/libresvip/plugins/ust/resampling.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ust/template.py` & `libresvip-1.1.6/libresvip/plugins/ust/template.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ust/ust.yapsy-plugin` & `libresvip-1.1.6/libresvip/plugins/ust/ust.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ust/ust_converter.py` & `libresvip-1.1.6/libresvip/plugins/ust/ust_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ust/ust_generator.py` & `libresvip-1.1.6/libresvip/plugins/ust/ust_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ust/ust_parser.py` & `libresvip-1.1.6/libresvip/plugins/ust/ust_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ust/vibrato_param.py` & `libresvip-1.1.6/libresvip/plugins/ust/vibrato_param.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ustx/model.py` & `libresvip-1.1.6/libresvip/plugins/ustx/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ustx/ustx.yapsy-plugin` & `libresvip-1.1.6/libresvip/plugins/ustx/ustx.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ustx/ustx_converter.py` & `libresvip-1.1.6/libresvip/plugins/ustx/ustx_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ustx/ustx_generator.py` & `libresvip-1.1.6/libresvip/plugins/ustx/ustx_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ustx/ustx_parser.py` & `libresvip-1.1.6/libresvip/plugins/ustx/ustx_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ustx/util.py` & `libresvip-1.1.6/libresvip/plugins/ustx/util.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ustx/utils/music_math.py` & `libresvip-1.1.6/libresvip/plugins/ustx/utils/music_math.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/ustx/utils/time_axis.py` & `libresvip-1.1.6/libresvip/plugins/ustx/utils/time_axis.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/vog/model.py` & `libresvip-1.1.6/libresvip/plugins/vog/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/vog/vog.yapsy-plugin` & `libresvip-1.1.6/libresvip/plugins/vog/vog.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/vog/vogen_converter.py` & `libresvip-1.1.6/libresvip/plugins/vog/vogen_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/vog/vogen_generator.py` & `libresvip-1.1.6/libresvip/plugins/vog/vogen_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/vog/vogen_parser.py` & `libresvip-1.1.6/libresvip/plugins/vog/vogen_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/vpr/model.py` & `libresvip-1.1.6/libresvip/plugins/vpr/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/vpr/options.py` & `libresvip-1.1.6/libresvip/plugins/vpr/options.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/vpr/vocaloid_pitch.py` & `libresvip-1.1.6/libresvip/plugins/vpr/vocaloid_pitch.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/vpr/vpr.yapsy-plugin` & `libresvip-1.1.6/libresvip/plugins/vpr/vpr.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/vpr/vpr_converter.py` & `libresvip-1.1.6/libresvip/plugins/vpr/vpr_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/vpr/vpr_generator.py` & `libresvip-1.1.6/libresvip/plugins/vpr/vpr_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/vpr/vpr_parser.py` & `libresvip-1.1.6/libresvip/plugins/vpr/vpr_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/vshp/model.py` & `libresvip-1.1.6/libresvip/plugins/vshp/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/vshp/options.py` & `libresvip-1.1.6/libresvip/plugins/vshp/options.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/vshp/vocalshifter_converter.py` & `libresvip-1.1.6/libresvip/plugins/vshp/vocalshifter_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/vshp/vocalshifter_parser.py` & `libresvip-1.1.6/libresvip/plugins/vshp/vocalshifter_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/vshp/vshp.yapsy-plugin` & `libresvip-1.1.6/libresvip/plugins/vshp/vshp.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/vspx/model.py` & `libresvip-1.1.6/libresvip/plugins/vspx/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/vspx/vocalsharp_converter.py` & `libresvip-1.1.6/libresvip/plugins/vspx/vocalsharp_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/vspx/vspx.yapsy-plugin` & `libresvip-1.1.6/libresvip/plugins/vspx/vspx.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/vspx/vspx_generator.py` & `libresvip-1.1.6/libresvip/plugins/vspx/vspx_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/vspx/vspx_interval_dict.py` & `libresvip-1.1.6/libresvip/plugins/vspx/vspx_interval_dict.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/vspx/vspx_parser.py` & `libresvip-1.1.6/libresvip/plugins/vspx/vspx_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/vsq/options.py` & `libresvip-1.1.6/libresvip/plugins/vsq/options.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/vsq/vocaloid_pitch.py` & `libresvip-1.1.6/libresvip/plugins/vsq/vocaloid_pitch.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/vsq/vsq.yapsy-plugin` & `libresvip-1.1.6/libresvip/plugins/vsq/vsq.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/vsq/vsq_converter.py` & `libresvip-1.1.6/libresvip/plugins/vsq/vsq_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/vsq/vsq_generator.py` & `libresvip-1.1.6/libresvip/plugins/vsq/vsq_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/vsq/vsq_parser.py` & `libresvip-1.1.6/libresvip/plugins/vsq/vsq_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/vsqx/enums.py` & `libresvip-1.1.6/libresvip/plugins/vsqx/enums.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/vsqx/model.py` & `libresvip-1.1.6/libresvip/plugins/vsqx/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/vsqx/models/vsqx3.py` & `libresvip-1.1.6/libresvip/plugins/vsqx/models/vsqx3.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/vsqx/models/vsqx4.py` & `libresvip-1.1.6/libresvip/plugins/vsqx/models/vsqx4.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/vsqx/options.py` & `libresvip-1.1.6/libresvip/plugins/vsqx/options.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/vsqx/vocaloid_pitch.py` & `libresvip-1.1.6/libresvip/plugins/vsqx/vocaloid_pitch.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/vsqx/vsq3_generator.py` & `libresvip-1.1.6/libresvip/plugins/vsqx/vsq3_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/vsqx/vsq4_generator.py` & `libresvip-1.1.6/libresvip/plugins/vsqx/vsq4_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/vsqx/vsqx.yapsy-plugin` & `libresvip-1.1.6/libresvip/plugins/vsqx/vsqx.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/vsqx/vsqx_converter.py` & `libresvip-1.1.6/libresvip/plugins/vsqx/vsqx_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/vsqx/vsqx_parser.py` & `libresvip-1.1.6/libresvip/plugins/vsqx/vsqx_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/y77/model.py` & `libresvip-1.1.6/libresvip/plugins/y77/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/y77/y77.yapsy-plugin` & `libresvip-1.1.6/libresvip/plugins/y77/y77.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/y77/y77_converter.py` & `libresvip-1.1.6/libresvip/plugins/y77/y77_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/y77/y77_generator.py` & `libresvip-1.1.6/libresvip/plugins/y77/y77_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/plugins/y77/y77_parser.py` & `libresvip-1.1.6/libresvip/plugins/y77/y77_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/res/libresvip.ico` & `libresvip-1.1.6/libresvip/res/libresvip.ico`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/res/locales/zh_CN/LC_MESSAGES/libresvip.mo` & `libresvip-1.1.6/libresvip/res/locales/zh_CN/LC_MESSAGES/libresvip.mo`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/utils/audio.py` & `libresvip-1.1.6/libresvip/utils/audio.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/utils/module_loading.py` & `libresvip-1.1.6/libresvip/utils/module_loading.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/utils/music_math.py` & `libresvip-1.1.6/libresvip/utils/music_math.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/utils/search.py` & `libresvip-1.1.6/libresvip/utils/search.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/utils/text.py` & `libresvip-1.1.6/libresvip/utils/text.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/utils/translation.py` & `libresvip-1.1.6/libresvip/utils/translation.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/utils/xmlutils/__init__.py` & `libresvip-1.1.6/libresvip/utils/xmlutils/__init__.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/utils/xmlutils/native.py` & `libresvip-1.1.6/libresvip/utils/xmlutils/native.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/utils/yamlutils/__init__.py` & `libresvip-1.1.6/libresvip/utils/yamlutils/__init__.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/utils/yamlutils/common.py` & `libresvip-1.1.6/libresvip/utils/yamlutils/common.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/utils/yamlutils/dumper.py` & `libresvip-1.1.6/libresvip/utils/yamlutils/dumper.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/utils/yamlutils/loader.py` & `libresvip-1.1.6/libresvip/utils/yamlutils/loader.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/web/elements.py` & `libresvip-1.1.6/libresvip/web/elements.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/libresvip/web/pages.py` & `libresvip-1.1.6/libresvip/web/pages.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.5/pyproject.toml` & `libresvip-1.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     "zhon<3.0.0,>=2.0.2",
     "zstandard<0.23.0,>=0.22.0; platform_python_implementation == \"CPython\"",
 ]
 name = "libresvip"
 dynamic = []
 description = "Universal Converter for Singing Voice Projects"
 readme = "README.md"
-version = "1.1.5"
+version = "1.1.6"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 repository = "https://github.com/SoulMelody/LibreSVIP"
 documentation = "https://soulmelody.github.io/LibreSVIP"
@@ -124,15 +124,15 @@
     "proto-plus-stubs>=0.7.0",
     "types-lxml>=2024.4.14",
     "types-parsimonious>=0.10.0.20240331",
     "types-pyyaml>=6.0.12.20240311",
     "types-ujson>=5.10.0.20240515",
 ]
 packaging = [
-    "cx-Freeze>=7.1.0",
+    "cx-Freeze>=7.1.0.post0",
     "nuitka>=2.3",
     "pyinstaller>=6.7.0",
     "shellingham<2.0.0,>=1.5.4",
 ]
 docs = [
     "mkdocs-material<10.0.0,>=9.5.25",
 ]
```

### Comparing `libresvip-1.1.5/PKG-INFO` & `libresvip-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libresvip
-Version: 1.1.5
+Version: 1.1.6
 Summary: Universal Converter for Singing Voice Projects
 Author-Email: SoulMelody <yjxrtzyx@gmail.com>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3
```

